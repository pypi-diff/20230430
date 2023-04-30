# Comparing `tmp/dndfog-0.6.1.tar.gz` & `tmp/dndfog-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dndfog-0.6.1.tar", max compression
+gzip compressed data, was "dndfog-0.6.2.tar", max compression
```

## Comparing `dndfog-0.6.1.tar` & `dndfog-0.6.2.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0        0 2022-07-16 18:14:13.435341 dndfog-0.6.1/dndfog/__init__.py
--rw-r--r--   0        0        0     3221 2023-03-03 21:08:09.362534 dndfog-0.6.1/dndfog/_aoe.py
--rw-r--r--   0        0        0     1663 2023-03-03 21:45:04.825940 dndfog-0.6.1/dndfog/camera.py
--rw-r--r--   0        0        0      673 2023-03-05 11:59:33.006790 dndfog-0.6.1/dndfog/draw/__init__.py
--rw-r--r--   0        0        0     1615 2023-03-05 11:50:47.883429 dndfog-0.6.1/dndfog/draw/generic.py
--rw-r--r--   0        0        0     2793 2023-03-05 13:04:18.410213 dndfog-0.6.1/dndfog/draw/map.py
--rw-r--r--   0        0        0     7133 2023-03-05 12:04:24.440504 dndfog-0.6.1/dndfog/draw/toolbar.py
--rw-r--r--   0        0        0     8610 2023-03-06 17:57:20.245104 dndfog-0.6.1/dndfog/event_handlers.py
--rw-r--r--   0        0        0     1188 2023-03-04 10:13:55.536095 dndfog-0.6.1/dndfog/fog.py
--rw-r--r--   0        0        0     1251 2023-03-04 09:41:04.665316 dndfog-0.6.1/dndfog/gameloop.py
--rw-r--r--   0        0        0      623 2023-03-03 21:45:05.195611 dndfog-0.6.1/dndfog/grid.py
--rw-r--r--   0        0        0      643 2023-03-04 09:41:04.676094 dndfog-0.6.1/dndfog/main.py
--rw-r--r--   0        0        0      746 2023-03-03 21:45:04.701005 dndfog-0.6.1/dndfog/map.py
--rw-r--r--   0        0        0     3097 2023-03-05 13:09:35.096950 dndfog-0.6.1/dndfog/markings.py
--rw-r--r--   0        0        0      477 2023-03-05 10:01:20.693142 dndfog-0.6.1/dndfog/math.py
--rw-r--r--   0        0        0     3283 2023-03-05 11:16:15.289422 dndfog-0.6.1/dndfog/piece.py
--rw-r--r--   0        0        0     6400 2023-03-05 13:30:06.685869 dndfog-0.6.1/dndfog/saving.py
--rw-r--r--   0        0        0     3631 2023-03-05 12:02:43.899586 dndfog-0.6.1/dndfog/toolbar.py
--rw-r--r--   0        0        0     7992 2023-03-05 13:23:14.983423 dndfog-0.6.1/dndfog/types.py
--rw-r--r--   0        0        0     1090 2022-01-21 22:49:34.887128 dndfog-0.6.1/LICENSE
--rw-r--r--   0        0        0     2643 2023-03-06 18:20:22.880763 dndfog-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     5461 2023-03-06 18:21:44.672857 dndfog-0.6.1/README.md
--rw-r--r--   0        0        0     6249 1970-01-01 00:00:00.000000 dndfog-0.6.1/setup.py
--rw-r--r--   0        0        0     6462 1970-01-01 00:00:00.000000 dndfog-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-07-16 18:14:13.435341 dndfog-0.6.2/dndfog/__init__.py
+-rw-r--r--   0        0        0     3221 2023-03-03 21:08:09.362534 dndfog-0.6.2/dndfog/_aoe.py
+-rw-r--r--   0        0        0     1663 2023-03-03 21:45:04.825940 dndfog-0.6.2/dndfog/camera.py
+-rw-r--r--   0        0        0      673 2023-04-30 05:40:21.761087 dndfog-0.6.2/dndfog/draw/__init__.py
+-rw-r--r--   0        0        0     1615 2023-03-05 11:50:47.883429 dndfog-0.6.2/dndfog/draw/generic.py
+-rw-r--r--   0        0        0     2793 2023-03-05 13:04:18.410213 dndfog-0.6.2/dndfog/draw/map.py
+-rw-r--r--   0        0        0     7133 2023-03-05 12:04:24.440504 dndfog-0.6.2/dndfog/draw/toolbar.py
+-rw-r--r--   0        0        0     8638 2023-04-30 05:39:32.017856 dndfog-0.6.2/dndfog/event_handlers.py
+-rw-r--r--   0        0        0     1188 2023-03-04 10:13:55.536095 dndfog-0.6.2/dndfog/fog.py
+-rw-r--r--   0        0        0     1251 2023-03-04 09:41:04.665316 dndfog-0.6.2/dndfog/gameloop.py
+-rw-r--r--   0        0        0      623 2023-03-03 21:45:05.195611 dndfog-0.6.2/dndfog/grid.py
+-rw-r--r--   0        0        0      641 2023-04-30 06:01:12.709340 dndfog-0.6.2/dndfog/main.py
+-rw-r--r--   0        0        0      746 2023-03-03 21:45:04.701005 dndfog-0.6.2/dndfog/map.py
+-rw-r--r--   0        0        0     3097 2023-03-05 13:09:35.096950 dndfog-0.6.2/dndfog/markings.py
+-rw-r--r--   0        0        0      477 2023-03-05 10:01:20.693142 dndfog-0.6.2/dndfog/math.py
+-rw-r--r--   0        0        0     3283 2023-03-05 11:16:15.289422 dndfog-0.6.2/dndfog/piece.py
+-rw-r--r--   0        0        0     6606 2023-04-30 05:39:50.391106 dndfog-0.6.2/dndfog/saving.py
+-rw-r--r--   0        0        0     3631 2023-03-05 12:02:43.899586 dndfog-0.6.2/dndfog/toolbar.py
+-rw-r--r--   0        0        0     7992 2023-03-05 13:23:14.983423 dndfog-0.6.2/dndfog/types.py
+-rw-r--r--   0        0        0     1090 2022-01-21 22:49:34.887128 dndfog-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2682 2023-04-30 05:40:37.925296 dndfog-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     5461 2023-03-06 18:21:44.672857 dndfog-0.6.2/README.md
+-rw-r--r--   0        0        0     6465 1970-01-01 00:00:00.000000 dndfog-0.6.2/PKG-INFO
```

### Comparing `dndfog-0.6.1/dndfog/_aoe.py` & `dndfog-0.6.2/dndfog/_aoe.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.1/dndfog/camera.py` & `dndfog-0.6.2/dndfog/camera.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.1/dndfog/draw/__init__.py` & `dndfog-0.6.2/dndfog/draw/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     draw_map(display, state.map)
 
     if state.show.grid:
         draw_grid(display, state.map)
 
     draw_pieces(display, state.map)
 
-    draw_markings(display, state.map)
-
     if state.show.fog:
         draw_fog(display, state.map)
 
+    draw_markings(display, state.map)
+
     draw_toolbar(display, loop.mouse_pos, state)
 
     pygame.display.flip()
```

### Comparing `dndfog-0.6.1/dndfog/draw/generic.py` & `dndfog-0.6.2/dndfog/draw/generic.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.1/dndfog/draw/map.py` & `dndfog-0.6.2/dndfog/draw/map.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.1/dndfog/draw/toolbar.py` & `dndfog-0.6.2/dndfog/draw/toolbar.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.1/dndfog/event_handlers.py` & `dndfog-0.6.2/dndfog/event_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     MouseWheelEvent,
     PlacingKey,
     ProgramState,
     Tool,
 )
 
 
-def handle_event(event: Event, loop: LoopData, state: ProgramState) -> None:
+def handle_event(event: Event, loop: LoopData, state: ProgramState) -> None:  # noqa: C901
     if event.type == pygame.QUIT:
         pygame.quit()
         sys.exit()
 
     elif event.type == pygame.KEYDOWN:
         handle_key_down(event, loop, state)
 
@@ -119,15 +119,15 @@
                 image=state.map.image,
                 original_image=state.map.original_image,
                 old_gridsize=old_gridsize,
                 new_gridsize=state.map.gridsize,
             )
 
 
-def handle_left_mouse_button_down(event: MouseButtonEvent, loop: LoopData, state: ProgramState) -> None:
+def handle_left_mouse_button_down(event: MouseButtonEvent, loop: LoopData, state: ProgramState) -> None:  # noqa: C901
     # Select a tool from the toolbar
     if state.show.toolbar and 0 <= loop.mouse_pos[1] < TOOLBAR_HEIGHT:
         item_clicked, _ = grid_position(loop.mouse_pos, (0, 0), TOOLBAR_HEIGHT)
         try:
             state.selected.tool = Tool(item_clicked)
         except ValueError:
             pass
```

### Comparing `dndfog-0.6.1/dndfog/fog.py` & `dndfog-0.6.2/dndfog/fog.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.1/dndfog/gameloop.py` & `dndfog-0.6.2/dndfog/gameloop.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.1/dndfog/grid.py` & `dndfog-0.6.2/dndfog/grid.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.1/dndfog/main.py` & `dndfog-0.6.2/dndfog/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from dndfog.gameloop import run
 from dndfog.saving import open_file_dialog
 
 
 def start() -> None:
     parser = ArgumentParser()
-    parser.add_argument("--file", default=None)
+    parser.add_argument("file", default=None)
     args = parser.parse_args()
 
     if args.file is not None:
         map_file = str(args.file)
     else:
         map_file = open_file_dialog(
             title="Select a background map, or a json data file",
```

### Comparing `dndfog-0.6.1/dndfog/map.py` & `dndfog-0.6.2/dndfog/map.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.1/dndfog/markings.py` & `dndfog-0.6.2/dndfog/markings.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.1/dndfog/piece.py` & `dndfog-0.6.2/dndfog/piece.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.1/dndfog/saving.py` & `dndfog-0.6.2/dndfog/saving.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import base64
 import gzip
 import json
 import os
+from pathlib import Path
 from typing import Optional
 
 import pygame
 import pywintypes
 from win32con import OFN_ALLOWMULTISELECT, OFN_EXPLORER
 from win32gui import GetOpenFileNameW, GetSaveFileNameW
 
@@ -25,24 +26,30 @@
     "save_file_dialog",
     "open_data_file",
     "save_data_file",
 ]
 
 
 def load_map(map_file: str, state: ProgramState) -> None:
+    extension = Path(map_file).suffix
+
     # Load data file
-    if map_file[-5:] == ".json":
+    if extension in [".json", ".dndfog"]:
         state.file = map_file
         open_data_file(state)
         return
 
     # Load background image
-    state.map.image = pygame.image.load(map_file).convert_alpha()
-    state.map.image.set_colorkey((255, 255, 255))
-    state.map.original_image = state.map.image.copy()
+    elif extension in [".png", ".jpg", ".jpeg"]:
+        state.map.image = pygame.image.load(map_file).convert_alpha()
+        state.map.image.set_colorkey((255, 255, 255))
+        state.map.original_image = state.map.image.copy()
+        return
+
+    raise RuntimeError("Unsupported file type.")
 
 
 def open_file_dialog(
     title: str = None,
     directory: Optional[str] = None,
     default_name: str = "",
     default_ext: str = "",
```

### Comparing `dndfog-0.6.1/dndfog/toolbar.py` & `dndfog-0.6.2/dndfog/toolbar.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.1/dndfog/types.py` & `dndfog-0.6.2/dndfog/types.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.1/LICENSE` & `dndfog-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.1/pyproject.toml` & `dndfog-0.6.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dndfog"
-version = "0.6.1"
+version = "0.6.2"
 description = "DND battle map with fog of war"
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "dndfog" },
 ]
@@ -38,33 +38,33 @@
 ]
 exclude = [
     "tests",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
-pygame = "2.2.0"
-pywin32 = "305"
+pywin32 = "306"
+pygame-ce = ">=2.2.1"
 
 [tool.poetry.group.test.dependencies]
-pytest = "7.2.2 "
+pytest = "7.3.1"
 coverage = "6.5.0"
-pre-commit = "3.1.1"
-tox = "4.4.6"
-tox-gh-actions = "3.0.0"
+pre-commit = "3.2.2"
+tox = "4.5.1"
+tox-gh-actions = "3.1.0"
 coveralls = "3.3.1"
-pyinstaller = "5.8.0"
+pyinstaller = "5.10.1"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.4.2"
-pymdown-extensions = "9.9.2"
+pymdown-extensions = "9.11"
 mkdocs-mermaid2-plugin = "0.6.0"
 
 [tool.poetry.group.lint.dependencies]
-mypy = "1.0.1"
+mypy = "1.2.0"
 
 [tool.poetry.scripts]
 dndfog = "dndfog.main:start"
 
 [tool.black]
 line-length = 120
 
@@ -81,14 +81,17 @@
     "I",  # isort
     "S",  # flake8-bandit
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
     "T",  # flake8-print
     "W",  # pycodestyle warnings
 ]
+extend-ignore = [
+    "S311",
+]
 
 [tool.mypy]
 python_version = "3.11"
 warn_return_any = "True"
 warn_unused_configs = "True"
 
 [tool.coverage.run]
```

### Comparing `dndfog-0.6.1/README.md` & `dndfog-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.1/setup.py` & `dndfog-0.6.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,149 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dndfog
+Version: 0.6.2
+Summary: DND battle map with fog of war
+Home-page: https://mrthearman.github.io/dndfog/
+License: MIT
+Keywords: dnd,fog,war,map,combat,infinite,gird
+Author: Matti Lamppu
+Author-email: lamppu.matti.akseli@gmail.com
+Requires-Python: >=3.10,<3.12
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pygame-ce (>=2.2.1)
+Requires-Dist: pywin32 (==306)
+Project-URL: Repository, https://github.com/MrThearMan/dndfog
+Description-Content-Type: text/markdown
+
+# DnD Fog
+
+[![GitHub Workflow Status][status-badge]][status]
+[![PyPI][pypi-badge]][pypi]
+[![GitHub][licence-badge]][licence]
+[![GitHub Last Commit][repo-badge]][repo]
+[![GitHub Issues][issues-badge]][issues]
+[![Downloads][downloads-badge]][pypi]
+[![Python Version][version-badge]][pypi]
+
+```shell
+pip install dndfog
+```
+
+---
+
+**Documentation**: [https://mrthearman.github.io/dndfog/](https://mrthearman.github.io/dndfog/)
+
+**Source Code**: [https://github.com/MrThearMan/dndfog/](https://github.com/MrThearMan/dndfog/)
+
+---
+
+Create battlemaps for tabletop RPGs, like [D&D](https://www.dndbeyond.com/).
+
+> Program is Windows only for now. This is due to the saving and loading widgets
+> being Windows only (using pywin32). You're free to modify the code to add file
+> loading and saving for other platforms.
+
+![Example Map](https://github.com/MrThearMan/dndfog/blob/main/docs/img/example-map.png?raw=true)
+
+## Features
+
+- Infinite grid
+- Add and remove a [fog of war](https://en.wikipedia.org/wiki/Fog_of_war) effect
+- Import maps from image files
+- Place, move and remove pieces on a grid (can be matched to image grid)
+- Place 1x1, 2x2, 3x3, or 4x4 pieces
+- Make markings on the map to show areas of effect or point out things to the players
+- Save and load file to a single JSON file (no need to keep the image file separately!)
+
+## How to use
+
+When installing from [pypi](https://pypi.org/), the library should come with a script
+named `dndfog` that you can run. It should be available in your environment if
+the `Python\Scripts` folder is set in PATH. You can also download an EXE from
+the [GitHub releases](https://github.com/MrThearMan/dndfog/releases).
+
+When the program opens, you need to select an image file to use as a background,
+or a JSON data file to load a map from. You can also lauch the program with
+`--file=<filepath>` to add an initial file.
+
+> The program does not autosave! You have to save (and override) the file yourself!
+
+### Keyboard shortcuts
+
+Toolbar:
+- Open/close the toolbar: `TAB`
+- Select tool from the toolbar: Quick select with the number keys `1-9` or click the
+  tool button with `Left mouse button` when the toolbar is open
+
+Camera:
+- Move camera: `Click and drag: Middle mouse button`
+- Zoom in: _Any tool except the `grid` tool_ selected from the toolbar + `Scroll wheel: Up`
+- Zoom out: _Any tool except the `grid` tool_ selected from the toolbar + `Scroll wheel: Down`
+
+Piece (quick select: `1`):
+- Add a piece: Select the `piece` tool from the toolbar + `Right mouse button` on an empty square
+- Remove a piece: Select the `piece` tool from the toolbar  + `Right mouse button` on a piece
+- Move a piece: Select the `piece` tool from the toolbar  + `Click and drag: Left mouse button`
+
+Fog (quick select: `2`):
+- Add fog: Select the `fog` tool from the toolbar  + `Left mouse button`
+- Remove fog: Select the `fog` tool from the toolbar  + `Right mouse button`
+- Show/hide fog: `F1` or the checkbox in the `fog` toolbar
+- Change fog size: Select the size to use from the `size` selector in the `fog` toolbar
+
+Map (quick select: `3`):
+- Move map image: Select the `map` tool from the toolbar + `Click and drag: Left mouse button`
+
+Grid (quick select: `4`):
+- Increase gridsize: Select the `grid` tool from the toolbar + `Scroll wheel: Up`
+- Decrease gridsize: Select the `grid` tool from the toolbar + `Scroll wheel: Down`
+- Show/hide grid: `F2` or the checkbox in the `fog` toolbar
+
+Mark (quick select: `5`):
+- Make markings: Select the `mark` tool from the toolbar + `Click and drag: Left mouse button`
+- Erase markings: Select the `mark` tool from the toolbar + `Click and drag: Right mouse button`
+- Clear markings: Click the `clear` button in the `mark` toolbar
+- Change marker color: Use the color selector in the `mark` toolbar
+
+Misc:
+- Save file: `CTRL + S` (will skip file dialog if json data file already exists)
+- Save file as: `CTRL + Shift + S` (will always open a file dialog)
+- Open file: `CTRL + O`
+- Quit program: Press the X mutton on the window
+
+## Known issues or lacking features
+
+- Matching program gridsize to background gridsize is a bit awkward
+- When zooming, the program grid and background map might not stay aligned
+- It's hard to keep track of combat, since there is no built-in turn order tracking
+- It's too easy to accidentally remove fog you didn't mean to. There should be some way to
+  layer fog, so that only some of it can be removed
+- Markings do not scale when zooming
+- There is no undo or redo
+- There is no way to add pictures to pieces to identify them better
+
+[status-badge]: https://img.shields.io/github/actions/workflow/status/MrThearMan/dndfog/test.yml?branch=main
+[pypi-badge]: https://img.shields.io/pypi/v/dndfog
+[licence-badge]: https://img.shields.io/github/license/MrThearMan/dndfog
+[repo-badge]: https://img.shields.io/github/last-commit/MrThearMan/dndfog
+[issues-badge]: https://img.shields.io/github/issues-raw/MrThearMan/dndfog
+[version-badge]: https://img.shields.io/pypi/pyversions/dndfog
+[downloads-badge]: https://img.shields.io/pypi/dm/dndfog
+
+[status]: https://github.com/MrThearMan/dndfog/actions/workflows/test.yml
+[pypi]: https://pypi.org/project/dndfog
+[licence]: https://github.com/MrThearMan/dndfog/blob/main/LICENSE
+[repo]: https://github.com/MrThearMan/dndfog/commits/main
+[issues]: https://github.com/MrThearMan/dndfog/issues
 
-packages = \
-['dndfog', 'dndfog.draw']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pygame==2.2.0', 'pywin32==305']
-
-entry_points = \
-{'console_scripts': ['dndfog = dndfog.main:start']}
-
-setup_kwargs = {
-    'name': 'dndfog',
-    'version': '0.6.1',
-    'description': 'DND battle map with fog of war',
-    'long_description': "# DnD Fog\n\n[![GitHub Workflow Status][status-badge]][status]\n[![PyPI][pypi-badge]][pypi]\n[![GitHub][licence-badge]][licence]\n[![GitHub Last Commit][repo-badge]][repo]\n[![GitHub Issues][issues-badge]][issues]\n[![Downloads][downloads-badge]][pypi]\n[![Python Version][version-badge]][pypi]\n\n```shell\npip install dndfog\n```\n\n---\n\n**Documentation**: [https://mrthearman.github.io/dndfog/](https://mrthearman.github.io/dndfog/)\n\n**Source Code**: [https://github.com/MrThearMan/dndfog/](https://github.com/MrThearMan/dndfog/)\n\n---\n\nCreate battlemaps for tabletop RPGs, like [D&D](https://www.dndbeyond.com/).\n\n> Program is Windows only for now. This is due to the saving and loading widgets\n> being Windows only (using pywin32). You're free to modify the code to add file\n> loading and saving for other platforms.\n\n![Example Map](https://github.com/MrThearMan/dndfog/blob/main/docs/img/example-map.png?raw=true)\n\n## Features\n\n- Infinite grid\n- Add and remove a [fog of war](https://en.wikipedia.org/wiki/Fog_of_war) effect\n- Import maps from image files\n- Place, move and remove pieces on a grid (can be matched to image grid)\n- Place 1x1, 2x2, 3x3, or 4x4 pieces\n- Make markings on the map to show areas of effect or point out things to the players\n- Save and load file to a single JSON file (no need to keep the image file separately!)\n\n## How to use\n\nWhen installing from [pypi](https://pypi.org/), the library should come with a script\nnamed `dndfog` that you can run. It should be available in your environment if\nthe `Python\\Scripts` folder is set in PATH. You can also download an EXE from\nthe [GitHub releases](https://github.com/MrThearMan/dndfog/releases).\n\nWhen the program opens, you need to select an image file to use as a background,\nor a JSON data file to load a map from. You can also lauch the program with\n`--file=<filepath>` to add an initial file.\n\n> The program does not autosave! You have to save (and override) the file yourself!\n\n### Keyboard shortcuts\n\nToolbar:\n- Open/close the toolbar: `TAB`\n- Select tool from the toolbar: Quick select with the number keys `1-9` or click the\n  tool button with `Left mouse button` when the toolbar is open\n\nCamera:\n- Move camera: `Click and drag: Middle mouse button`\n- Zoom in: _Any tool except the `grid` tool_ selected from the toolbar + `Scroll wheel: Up`\n- Zoom out: _Any tool except the `grid` tool_ selected from the toolbar + `Scroll wheel: Down`\n\nPiece (quick select: `1`):\n- Add a piece: Select the `piece` tool from the toolbar + `Right mouse button` on an empty square\n- Remove a piece: Select the `piece` tool from the toolbar  + `Right mouse button` on a piece\n- Move a piece: Select the `piece` tool from the toolbar  + `Click and drag: Left mouse button`\n\nFog (quick select: `2`):\n- Add fog: Select the `fog` tool from the toolbar  + `Left mouse button`\n- Remove fog: Select the `fog` tool from the toolbar  + `Right mouse button`\n- Show/hide fog: `F1` or the checkbox in the `fog` toolbar\n- Change fog size: Select the size to use from the `size` selector in the `fog` toolbar\n\nMap (quick select: `3`):\n- Move map image: Select the `map` tool from the toolbar + `Click and drag: Left mouse button`\n\nGrid (quick select: `4`):\n- Increase gridsize: Select the `grid` tool from the toolbar + `Scroll wheel: Up`\n- Decrease gridsize: Select the `grid` tool from the toolbar + `Scroll wheel: Down`\n- Show/hide grid: `F2` or the checkbox in the `fog` toolbar\n\nMark (quick select: `5`):\n- Make markings: Select the `mark` tool from the toolbar + `Click and drag: Left mouse button`\n- Erase markings: Select the `mark` tool from the toolbar + `Click and drag: Right mouse button`\n- Clear markings: Click the `clear` button in the `mark` toolbar\n- Change marker color: Use the color selector in the `mark` toolbar\n\nMisc:\n- Save file: `CTRL + S` (will skip file dialog if json data file already exists)\n- Save file as: `CTRL + Shift + S` (will always open a file dialog)\n- Open file: `CTRL + O`\n- Quit program: Press the X mutton on the window\n\n## Known issues or lacking features\n\n- Matching program gridsize to background gridsize is a bit awkward\n- When zooming, the program grid and background map might not stay aligned\n- It's hard to keep track of combat, since there is no built-in turn order tracking\n- It's too easy to accidentally remove fog you didn't mean to. There should be some way to\n  layer fog, so that only some of it can be removed\n- Markings do not scale when zooming\n- There is no undo or redo\n- There is no way to add pictures to pieces to identify them better\n\n[status-badge]: https://img.shields.io/github/actions/workflow/status/MrThearMan/dndfog/test.yml?branch=main\n[pypi-badge]: https://img.shields.io/pypi/v/dndfog\n[licence-badge]: https://img.shields.io/github/license/MrThearMan/dndfog\n[repo-badge]: https://img.shields.io/github/last-commit/MrThearMan/dndfog\n[issues-badge]: https://img.shields.io/github/issues-raw/MrThearMan/dndfog\n[version-badge]: https://img.shields.io/pypi/pyversions/dndfog\n[downloads-badge]: https://img.shields.io/pypi/dm/dndfog\n\n[status]: https://github.com/MrThearMan/dndfog/actions/workflows/test.yml\n[pypi]: https://pypi.org/project/dndfog\n[licence]: https://github.com/MrThearMan/dndfog/blob/main/LICENSE\n[repo]: https://github.com/MrThearMan/dndfog/commits/main\n[issues]: https://github.com/MrThearMan/dndfog/issues\n",
-    'author': 'Matti Lamppu',
-    'author_email': 'lamppu.matti.akseli@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://mrthearman.github.io/dndfog/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<3.12',
-}
-
-
-setup(**setup_kwargs)
```

