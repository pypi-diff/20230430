# Comparing `tmp/chapsnap-1.1.0.tar.gz` & `tmp/chapsnap-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chapsnap-1.1.0.tar", max compression
+gzip compressed data, was "chapsnap-1.2.0.tar", max compression
```

## Comparing `chapsnap-1.1.0.tar` & `chapsnap-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-04-26 16:15:52.298321 chapsnap-1.1.0/LICENSE
--rw-r--r--   0        0        0      468 2023-04-26 16:15:52.298321 chapsnap-1.1.0/README.md
--rw-r--r--   0        0        0       23 2023-04-26 16:15:52.298321 chapsnap-1.1.0/chapsnap/__init__.py
--rw-r--r--   0        0        0     7565 2023-04-26 16:15:52.298321 chapsnap-1.1.0/chapsnap/main.py
--rw-r--r--   0        0        0     1064 2023-04-26 16:15:52.298321 chapsnap-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1749 1970-01-01 00:00:00.000000 chapsnap-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-30 19:50:45.680073 chapsnap-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2348 2023-04-30 19:50:45.680073 chapsnap-1.2.0/README.md
+-rw-r--r--   0        0        0       23 2023-04-30 19:50:45.680073 chapsnap-1.2.0/chapsnap/__init__.py
+-rw-r--r--   0        0        0    10809 2023-04-30 19:50:45.684073 chapsnap-1.2.0/chapsnap/main.py
+-rw-r--r--   0        0        0     1088 2023-04-30 19:50:45.684073 chapsnap-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 chapsnap-1.2.0/PKG-INFO
```

### Comparing `chapsnap-1.1.0/LICENSE` & `chapsnap-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chapsnap-1.1.0/chapsnap/main.py` & `chapsnap-1.2.0/chapsnap/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,200 +1,258 @@
 from __future__ import annotations
 
+import shutil
 from datetime import datetime
-from functools import partial
 from pathlib import Path
 
 import click
 from rich.status import Status
 from rich.table import Table, Column
-from rich.progress import Progress
-from rich.progress import TextColumn, SpinnerColumn, BarColumn, TimeRemainingColumn
 from rich import print
+from pymediainfo import MediaInfo
 
-from utilities import get_chapters, get_scene_changes, format_timestamp, mux_chapters, load_chapters_file
+from utilities import get_chapters, get_scene_changes, format_timestamp, load_chapters_file, set_chapters
 
 
 @click.command()
 @click.argument("video", type=Path)
 @click.argument("chapters", type=Path, required=False)
 @click.option("-t", "--threshold", type=float, default=0.4,
               help="Threshold on Scene Change probability scores. The lower the value, the more unlikely the "
                    "frame is to be a Scene Change. Range: 0.0 (Impossible) - 1.0 (Definite).")
 @click.option("-o", "--offset", type=float, default=None,
               help="Offset to apply to each Chapter. A negative offset may result in fewer Chapters.")
+@click.option("--trim", type=int, multiple=True, default=None,
+              help="Remove n Chapters from the start of the Video. A negative value will remove n Chapters from "
+                   "the end of the Video. Timestamps will be offset respectively.")
 @click.option("-nf", "--no-forward", is_flag=True, default=False,
               help="Do not try to resync Chapters forward in time.")
 @click.option("-nb", "--no-backward", is_flag=True, default=False,
               help="Do not try to resync Chapters backward in time.")
 @click.option("-k", "--keyframes", is_flag=True, default=False,
               help="Only sync to Scene Changes on Keyframes (I-frames).")
+@click.option("-0", "--zero", is_flag=True, default=False,
+              help="Force the first chapter to be at `00:00:00.000`, even after offsets and trims.")
+@click.option("-c", "--chain", is_flag=True, default=False,
+              help="Chain sync adjustments from one Chapter to the next. E.g., Chapter 1 had -2, so Chapter 2 will "
+                   "begin with an offset of -2. Chapter 2 with -2 has a change of -1, so Chapter 3 will begin with "
+                   "an offset of -3 and so on.")
+@click.option("--overwrite", is_flag=True, default=False,
+              help="Apply new Chapters to the input video file in-place, without making a duplicate.")
 def main(
     video: Path,
     chapters: Path | None,
     threshold: float,
     offset: float | None,
+    trim: list[int],
     no_forward: bool,
     no_backward: bool,
-    keyframes: bool
+    keyframes: bool,
+    zero: bool,
+    chain: bool,
+    overwrite: bool
 ):
     """
     Snap Chapters to Scene Changes.
 
     \b
-    VIDEO       The video file to snap chapters to scene changes.
+    VIDEO       The video file to snap chapters to scene changes. All video formats are
+                supported. You may alternatively provide a directory path to process
+                video files in batch.
     [CHAPTERS]  Optional chapters file if you want to use chapters from a file
                 rather than ones already muxed with the video.
     """
     if offset is not None and not isinstance(offset, float):
         raise click.ClickException(f"Expected offset to be a {float} not {offset!r}")
 
-    with Status("Getting Chapters..."):
-        if chapters:
-            chapters = load_chapters_file(chapters)
-        else:
-            chapters = get_chapters(video)
-        chapter_table = Table(title="Chapters")
-        chapter_table.add_column("#", justify="right")
-        chapter_table.add_column("Name")
-        chapter_table.add_column("Timestamp")
-        for i, chapter in enumerate(chapters, start=1):
-            name = chapter.get("tags", {}).get("title")
-            timestamp = format_timestamp(float(chapter["start_time"]))
-            chapter_table.add_row(f"{i:02}", name or "—", timestamp)
-        print(chapter_table)
-
-    with Status("Analyzing Video for Scene Changes (this could take a while)..."):
-        scene_changes = get_scene_changes(video, threshold)
-        scene_change_table = Table(
-            Column("#", justify="right"),
-            "Timestamp",
-            "Type",
-            "Score",
-            title="Scene Changes"
-        )
-        for i, scene_change in enumerate(scene_changes, start=1):
-            timestamp = format_timestamp(float(scene_change["best_effort_timestamp_time"]))
-            scene_change_table.add_row(
-                f"{i:02}",
-                timestamp,
-                scene_change["pict_type"],
-                scene_change["tags"]["lavfi.scene_score"]
-            )
-        print(scene_change_table)
+    chapters_ = chapters
 
-    new_chapter_table = Table(
-        Column("#", justify="right"),
-        "Before",
-        "After",
-        "Change",
-        "Closest Scene Changes",
-        title="Chapter Modifications"
-    )
-
-    new_chapter_timestamps = {}
-
-    for i, chapter in enumerate(chapters, start=1):
-        start_time = float(chapter["start_time"])
-        if offset:
-            start_time = max(start_time + offset, 0)
-
-        name = chapter.get("tags", {}).get("title")
-
-        is_already_timed = any(float(x["best_effort_timestamp_time"]) == start_time for x in scene_changes)
-
-        if is_already_timed:
-            new_chapter_table.add_row(
-                f"{i:02}",
-                format_timestamp(start_time),
-                format_timestamp(start_time),
-                "0.00",
-                "Already synced, skipped..."
-            )
-        else:
-            if no_forward:
-                closest_forward = 0.0
-            else:
-                closest_forward = next((
-                    float(x["best_effort_timestamp_time"])
-                    for x in scene_changes
-                    if float(x["best_effort_timestamp_time"]) > start_time and
-                    (not keyframes or x["pict_type"] == "I")
-                ), 0.0)
+    if video.is_file():
+        videos = [video]
+    else:
+        videos = [
+            x
+            for x in video.glob("**/*.*")
+            if not x.stem.endswith(" (Resynced)") and MediaInfo.parse(x).video_tracks
+        ]
 
-            if no_backward or start_time == 0.0:
-                closest_backward = 0.0
+    for video in videos:
+        print(f"Processing {video.stem}...")
+        with Status("Getting Chapters..."):
+            if chapters_:
+                chapters = load_chapters_file(chapters_)
             else:
-                closest_backward = next(
-                    float(x["best_effort_timestamp_time"])
-                    for x in reversed(scene_changes)
-                    if float(x["best_effort_timestamp_time"]) <= start_time and
-                    (not keyframes or x["pict_type"] == "I")
-                )
-
-            closest = min((closest_forward, closest_backward), key=lambda x: abs(x - start_time))
-            cb = [" ", "*"][closest == closest_backward]
-            cf = [" ", "*"][closest == closest_forward]
-
-            if closest in new_chapter_timestamps:
-                new_chapter_table.add_row(
-                    "--",
-                    format_timestamp(start_time),
-                    format_timestamp(closest),
-                    f"{closest - start_time:.2f}",
-                    "Removed, matched previous chapter"
+                chapters = get_chapters(video)
+            if trim:
+                for amount in trim:
+                    negative = amount < 0
+                    trim_offset = float(chapters[amount]["start_time"]) - float(chapters[amount - 1]["start_time"])
+                    if negative:
+                        chapters = chapters[:amount]
+                    else:
+                        chapters = chapters[amount:]
+                    for chapter in chapters:
+                        chapter["start_time"] = float(chapter["start_time"]) - trim_offset
+            if offset:
+                for chapter in chapters:
+                    chapter["start_time"] = max(float(chapter["start_time"]) + offset, 0)
+            if zero:
+                chapters[0]["start_time"] = 0.0
+            for chapter in chapters:
+                name = chapter.get("tags", {}).get("title")
+                try:
+                    datetime.strptime(name, "%H:%M:%S.%f")
+                except ValueError:
+                    pass
+                else:
+                    chapter["tags"]["title"] = format_timestamp(float(chapter["start_time"]))
+
+            chapter_table = Table(
+                Column("#", justify="right"),
+                "Name",
+                "Timestamp",
+                title="Chapters",
+                caption=f"offset: {offset:.3f}" if offset else None,
+                caption_justify="right"
+            )
+            for i, chapter in enumerate(chapters, start=1):
+                name = chapter.get("tags", {}).get("title")
+                timestamp = format_timestamp(float(chapter["start_time"]))
+                chapter_table.add_row(f"{i:02}", name or "—", timestamp)
+            print(chapter_table)
+
+        with Status("Analyzing Video for Scene Changes (this could take a while)..."):
+            scene_changes = get_scene_changes(video, threshold)
+            scene_change_table = Table(
+                Column("#", justify="right"),
+                "Timestamp",
+                "Type",
+                "Score",
+                title="Scene Changes"
+            )
+            for i, scene_change in enumerate(scene_changes, start=1):
+                timestamp = format_timestamp(float(scene_change["best_effort_timestamp_time"]))
+                scene_change_table.add_row(
+                    f"{i:02}",
+                    timestamp,
+                    scene_change["pict_type"],
+                    scene_change["tags"]["lavfi.scene_score"]
                 )
-                continue
+            print(scene_change_table)
 
-            new_chapter_table.add_row(
-                f"{i:02}",
-                format_timestamp(start_time),
-                format_timestamp(closest),
-                f"{closest - start_time:.2f}",
-                f"{format_timestamp(closest_backward)}{cb} <- | -> {format_timestamp(closest_forward)}{cf}"
-            )
+        new_chapter_table = Table(
+            Column("#", justify="right"),
+            "Before",
+            "After",
+            "Change",
+            "Closest Scene Changes",
+            title="Chapter Modifications",
+            caption_justify="right"
+        )
 
-            start_time = closest
+        new_chapter_timestamps = {}
+        offset_chains = []
 
-            if datetime.strptime(name, "%H:%M:%S.%f"):
-                name = format_timestamp(start_time)
+        for i, chapter in enumerate(chapters, start=1):
+            start_time = float(chapter["start_time"])
+            if offset_chains:
+                start_time = max(start_time + offset_chains[-1], 0)
 
-        new_chapter_timestamps[start_time] = name
+            name = chapter.get("tags", {}).get("title")
 
-    print(new_chapter_table)
+            is_already_timed = any(float(x["best_effort_timestamp_time"]) == start_time for x in scene_changes)
 
-    new_chapter_file = "\n".join([
-        line
-        for i, (timestamp, name) in enumerate(new_chapter_timestamps.items(), start=1)
-        for line in [
-            f"CHAPTER{i:02}={format_timestamp(timestamp)}",
-            f"CHAPTER{i:02}NAME={name or f'Chapter {i:02}'}"
-        ]
-    ])
+            if is_already_timed:
+                new_chapter_table.add_row(
+                    f"{i:02}",
+                    format_timestamp(start_time),
+                    format_timestamp(start_time),
+                    "0.00",
+                    "Already synced, skipped..."
+                )
+            else:
+                if no_forward:
+                    closest_forward = 0.0
+                else:
+                    closest_forward = next((
+                        float(x["best_effort_timestamp_time"])
+                        for x in scene_changes
+                        if float(x["best_effort_timestamp_time"]) > start_time and
+                        (not keyframes or x["pict_type"] == "I")
+                    ), 0.0)
+
+                if no_backward or start_time == 0.0:
+                    closest_backward = 0.0
+                else:
+                    closest_backward = next(
+                        float(x["best_effort_timestamp_time"])
+                        for x in reversed(scene_changes)
+                        if float(x["best_effort_timestamp_time"]) <= start_time and
+                        (not keyframes or x["pict_type"] == "I")
+                    )
+
+                closest = min((closest_forward, closest_backward), key=lambda x: abs(x - start_time))
+                cb = [" ", "*"][closest == closest_backward]
+                cf = [" ", "*"][closest == closest_forward]
+
+                if closest in new_chapter_timestamps:
+                    new_chapter_table.add_row(
+                        "--",
+                        format_timestamp(start_time),
+                        format_timestamp(closest),
+                        f"{closest - start_time:.2f}",
+                        "Removed, matched previous chapter"
+                    )
+                    continue
+
+                if chain and i != len(chapters):
+                    last_offset_chain = offset_chains[-1] if offset_chains else 0.0
+                    offset_chains.append(last_offset_chain + (closest - start_time))
+                    new_chapter_table.caption = f"offset chains: {','.join([f'{x:.3f}' for x in offset_chains])}"
 
-    chapters_file_path = video.with_suffix(f"{video.suffix}.retimed_chapters.txt")
-    chapters_file_path.write_text(new_chapter_file, encoding="utf8")
+                new_chapter_table.add_row(
+                    f"{i:02}",
+                    format_timestamp(start_time),
+                    format_timestamp(closest),
+                    f"{closest - start_time:.2f}",
+                    f"{format_timestamp(closest_backward)}{cb} <- | -> {format_timestamp(closest_forward)}{cf}"
+                )
 
-    if video.suffix.lower() == ".mkv":
-        muxing_progress = Progress(
-            TextColumn("[progress.description]{task.description}"),
-            SpinnerColumn(finished_text=""),
-            BarColumn(),
-            "•",
-            TimeRemainingColumn(compact=True, elapsed_when_finished=True)
-        )
+                start_time = closest
 
-        with muxing_progress:
-            task = muxing_progress.add_task("Multiplexing...", total=100, start=True)
-            out_path = video.with_stem(video.stem + " (Resynced)")
-            mux_chapters(
-                video,
-                chapters_file_path,
-                out_path,
-                progress=partial(muxing_progress.update, task_id=task)
-            )
+                try:
+                    datetime.strptime(name, "%H:%M:%S.%f")
+                except ValueError:
+                    pass
+                else:
+                    name = format_timestamp(start_time)
+
+            new_chapter_timestamps[start_time] = name
+
+        print(new_chapter_table)
+
+        new_chapter_file = "\n".join([
+            line
+            for i, (timestamp, name) in enumerate(new_chapter_timestamps.items(), start=1)
+            for line in [
+                f"CHAPTER{i:02}={format_timestamp(timestamp)}",
+                f"CHAPTER{i:02}NAME={name or f'Chapter {i:02}'}"
+            ]
+        ])
+
+        chapters_file_path = video.with_suffix(f"{video.suffix}.retimed_chapters.txt")
+        chapters_file_path.write_text(new_chapter_file, encoding="utf8")
+
+        if video.suffix.lower() == ".mkv":
+            with Status("Updating Chapters in MKV Container..."):
+                if overwrite:
+                    out_path = video
+                else:
+                    out_path = video.with_stem(video.stem + " (Resynced)")
+                    shutil.copy(video, out_path)
+                set_chapters(out_path, chapters_file_path)
 
     print(":tada: Done!")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `chapsnap-1.1.0/pyproject.toml` & `chapsnap-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ChapSnap"
-version = "1.1.0"
+version = "1.2.0"
 description = "Resync Chapters by snapping them to Scene Changes."
 authors = ["rlaphoenix <rlaphoenix@pm.me>"]
 readme = "README.md"
 repository = "https://github.com/rlaphoenix/ChapSnap"
 keywords = ["python", "chapters", "video", "analysis", "scene-detection"]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -25,10 +25,11 @@
 "Forums" = "https://github.com/rlaphoenix/ChapSnap/discussions"
 "Changelog" = "https://github.com/rlaphoenix/ChapSnap/blob/master/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.12"
 click = "^8.1.3"
 rich = "^13.3.4"
+pymediainfo = "^6.0.1"
 
 [tool.poetry.scripts]
 chapsnap = "chapsnap.main:main"
```

