# Comparing `tmp/edge-tts-6.1.3.tar.gz` & `tmp/edge-tts-6.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge-tts-6.1.3.tar", last modified: Wed Jan 25 16:37:08 2023, max compression
+gzip compressed data, was "edge-tts-6.1.4.tar", last modified: Sun Apr 30 20:49:38 2023, max compression
```

## Comparing `edge-tts-6.1.3.tar` & `edge-tts-6.1.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-25 16:37:08.739426 edge-tts-6.1.3/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-25 16:37:08.735426 edge-tts-6.1.3/.github/
--rw-rw-r--   0 user      (1000) user      (1000)      106 2022-09-27 09:16:55.000000 edge-tts-6.1.3/.github/dependabot.yml
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-25 16:37:08.735426 edge-tts-6.1.3/.github/workflows/
--rw-rw-r--   0 user      (1000) user      (1000)      585 2023-01-05 05:52:51.000000 edge-tts-6.1.3/.github/workflows/code-quality.yml
--rw-rw-r--   0 user      (1000) user      (1000)     2277 2022-09-27 09:17:01.000000 edge-tts-6.1.3/.github/workflows/codeql-analysis.yml
--rw-rw-r--   0 user      (1000) user      (1000)     3078 2023-01-05 05:54:43.000000 edge-tts-6.1.3/.gitignore
--rw-rw-r--   0 user      (1000) user      (1000)      161 2023-01-04 23:46:51.000000 edge-tts-6.1.3/.isort.cfg
--rw-------   0 user      (1000) user      (1000)    35149 2021-12-03 12:08:58.000000 edge-tts-6.1.3/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     3873 2023-01-25 16:37:08.739426 edge-tts-6.1.3/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     3319 2023-01-05 23:12:21.000000 edge-tts-6.1.3/README.md
--rwx------   0 user      (1000) user      (1000)      136 2023-01-05 05:59:23.000000 edge-tts-6.1.3/build_and_publish.sh
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-25 16:37:08.735426 edge-tts-6.1.3/examples/
--rw-rw-r--   0 user      (1000) user      (1000)      894 2023-01-05 05:52:51.000000 edge-tts-6.1.3/examples/basic_audio_streaming.py
--rw-rw-r--   0 user      (1000) user      (1000)      381 2023-01-05 05:52:51.000000 edge-tts-6.1.3/examples/basic_generation.py
--rw-rw-r--   0 user      (1000) user      (1000)      643 2023-01-09 16:31:32.000000 edge-tts-6.1.3/examples/dynamic_voice_selection.py
--rw-rw-r--   0 user      (1000) user      (1000)      959 2023-01-05 05:52:51.000000 edge-tts-6.1.3/examples/streaming_with_subtitles.py
--rwxrwxr-x   0 user      (1000) user      (1000)       99 2023-01-04 23:47:18.000000 edge-tts-6.1.3/format.sh
--rwxrwxr-x   0 user      (1000) user      (1000)      108 2023-01-20 00:45:15.000000 edge-tts-6.1.3/lint.sh
--rw-rw-r--   0 user      (1000) user      (1000)      561 2023-01-04 23:38:10.000000 edge-tts-6.1.3/mypy.ini
--rw-rw-r--   0 user      (1000) user      (1000)    20395 2023-01-20 00:48:48.000000 edge-tts-6.1.3/pylintrc
--rw-rw-r--   0 user      (1000) user      (1000)      834 2023-01-25 16:37:08.739426 edge-tts-6.1.3/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      192 2023-01-04 23:17:58.000000 edge-tts-6.1.3/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-25 16:37:08.735426 edge-tts-6.1.3/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-25 16:37:08.739426 edge-tts-6.1.3/src/edge_playback/
--rw-rw-r--   0 user      (1000) user      (1000)      109 2023-01-05 05:52:51.000000 edge-tts-6.1.3/src/edge_playback/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2053 2023-01-10 14:38:06.000000 edge-tts-6.1.3/src/edge_playback/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-04 23:17:58.000000 edge-tts-6.1.3/src/edge_playback/py.typed
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-25 16:37:08.739426 edge-tts-6.1.3/src/edge_tts/
--rw-rw-r--   0 user      (1000) user      (1000)      317 2023-01-09 19:17:13.000000 edge-tts-6.1.3/src/edge_tts/__init__.py
--rw-------   0 user      (1000) user      (1000)       94 2021-12-07 19:17:40.000000 edge-tts-6.1.3/src/edge_tts/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)    16435 2023-01-20 01:42:56.000000 edge-tts-6.1.3/src/edge_tts/communicate.py
--rw-rw-r--   0 user      (1000) user      (1000)      416 2023-01-05 05:52:51.000000 edge-tts-6.1.3/src/edge_tts/constants.py
--rw-rw-r--   0 user      (1000) user      (1000)      558 2023-01-05 05:52:51.000000 edge-tts-6.1.3/src/edge_tts/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2587 2023-01-09 16:29:31.000000 edge-tts-6.1.3/src/edge_tts/list_voices.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-05 04:26:59.000000 edge-tts-6.1.3/src/edge_tts/py.typed
--rw-rw-r--   0 user      (1000) user      (1000)     3041 2023-01-19 23:57:04.000000 edge-tts-6.1.3/src/edge_tts/submaker.py
--rw-rw-r--   0 user      (1000) user      (1000)     3780 2023-01-25 16:36:12.000000 edge-tts-6.1.3/src/edge_tts/util.py
--rw-rw-r--   0 user      (1000) user      (1000)      128 2023-01-25 16:36:56.000000 edge-tts-6.1.3/src/edge_tts/version.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-25 16:37:08.739426 edge-tts-6.1.3/src/edge_tts.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3873 2023-01-25 16:37:08.000000 edge-tts-6.1.3/src/edge_tts.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      903 2023-01-25 16:37:08.000000 edge-tts-6.1.3/src/edge_tts.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-01-25 16:37:08.000000 edge-tts-6.1.3/src/edge_tts.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       98 2023-01-25 16:37:08.000000 edge-tts-6.1.3/src/edge_tts.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       46 2023-01-25 16:37:08.000000 edge-tts-6.1.3/src/edge_tts.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       23 2023-01-25 16:37:08.000000 edge-tts-6.1.3/src/edge_tts.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:49:38.163035 edge-tts-6.1.4/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:49:38.163035 edge-tts-6.1.4/.github/
+-rw-rw-r--   0 user      (1000) user      (1000)      106 2022-09-27 09:16:55.000000 edge-tts-6.1.4/.github/dependabot.yml
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:49:38.163035 edge-tts-6.1.4/.github/workflows/
+-rw-rw-r--   0 user      (1000) user      (1000)      585 2023-01-05 05:52:51.000000 edge-tts-6.1.4/.github/workflows/code-quality.yml
+-rw-rw-r--   0 user      (1000) user      (1000)     2277 2022-09-27 09:17:01.000000 edge-tts-6.1.4/.github/workflows/codeql-analysis.yml
+-rw-rw-r--   0 user      (1000) user      (1000)     3078 2023-01-05 05:54:43.000000 edge-tts-6.1.4/.gitignore
+-rw-rw-r--   0 user      (1000) user      (1000)      161 2023-01-04 23:46:51.000000 edge-tts-6.1.4/.isort.cfg
+-rw-------   0 user      (1000) user      (1000)    35149 2021-12-03 12:08:58.000000 edge-tts-6.1.4/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     3873 2023-04-30 20:49:38.163035 edge-tts-6.1.4/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     3319 2023-01-05 23:12:21.000000 edge-tts-6.1.4/README.md
+-rwx------   0 user      (1000) user      (1000)      136 2023-01-05 05:59:23.000000 edge-tts-6.1.4/build_and_publish.sh
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:49:38.163035 edge-tts-6.1.4/examples/
+-rw-rw-r--   0 user      (1000) user      (1000)      957 2023-04-26 22:07:39.000000 edge-tts-6.1.4/examples/basic_audio_streaming.py
+-rw-rw-r--   0 user      (1000) user      (1000)      444 2023-04-26 22:07:39.000000 edge-tts-6.1.4/examples/basic_generation.py
+-rw-rw-r--   0 user      (1000) user      (1000)      706 2023-04-26 22:07:39.000000 edge-tts-6.1.4/examples/dynamic_voice_selection.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1022 2023-04-26 22:07:39.000000 edge-tts-6.1.4/examples/streaming_with_subtitles.py
+-rwxrwxr-x   0 user      (1000) user      (1000)       99 2023-01-04 23:47:18.000000 edge-tts-6.1.4/format.sh
+-rwxrwxr-x   0 user      (1000) user      (1000)      108 2023-01-20 00:45:15.000000 edge-tts-6.1.4/lint.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      561 2023-01-04 23:38:10.000000 edge-tts-6.1.4/mypy.ini
+-rw-rw-r--   0 user      (1000) user      (1000)    20395 2023-04-30 20:48:15.000000 edge-tts-6.1.4/pylintrc
+-rw-rw-r--   0 user      (1000) user      (1000)      834 2023-04-30 20:49:38.163035 edge-tts-6.1.4/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      192 2023-01-04 23:17:58.000000 edge-tts-6.1.4/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:49:38.163035 edge-tts-6.1.4/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:49:38.163035 edge-tts-6.1.4/src/edge_playback/
+-rw-rw-r--   0 user      (1000) user      (1000)      109 2023-01-05 05:52:51.000000 edge-tts-6.1.4/src/edge_playback/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2053 2023-01-10 14:38:06.000000 edge-tts-6.1.4/src/edge_playback/__main__.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-04 23:17:58.000000 edge-tts-6.1.4/src/edge_playback/py.typed
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:49:38.163035 edge-tts-6.1.4/src/edge_tts/
+-rw-rw-r--   0 user      (1000) user      (1000)      317 2023-01-09 19:17:13.000000 edge-tts-6.1.4/src/edge_tts/__init__.py
+-rw-------   0 user      (1000) user      (1000)       94 2021-12-07 19:17:40.000000 edge-tts-6.1.4/src/edge_tts/__main__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17073 2023-04-30 20:46:32.000000 edge-tts-6.1.4/src/edge_tts/communicate.py
+-rw-rw-r--   0 user      (1000) user      (1000)      416 2023-01-05 05:52:51.000000 edge-tts-6.1.4/src/edge_tts/constants.py
+-rw-rw-r--   0 user      (1000) user      (1000)      558 2023-04-05 13:39:33.000000 edge-tts-6.1.4/src/edge_tts/exceptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2587 2023-01-09 16:29:31.000000 edge-tts-6.1.4/src/edge_tts/list_voices.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-05 04:26:59.000000 edge-tts-6.1.4/src/edge_tts/py.typed
+-rw-rw-r--   0 user      (1000) user      (1000)     3823 2023-04-05 14:00:08.000000 edge-tts-6.1.4/src/edge_tts/submaker.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4343 2023-04-30 20:40:58.000000 edge-tts-6.1.4/src/edge_tts/util.py
+-rw-rw-r--   0 user      (1000) user      (1000)      128 2023-04-30 20:49:15.000000 edge-tts-6.1.4/src/edge_tts/version.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:49:38.163035 edge-tts-6.1.4/src/edge_tts.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3873 2023-04-30 20:49:38.000000 edge-tts-6.1.4/src/edge_tts.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      903 2023-04-30 20:49:38.000000 edge-tts-6.1.4/src/edge_tts.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-30 20:49:38.000000 edge-tts-6.1.4/src/edge_tts.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       98 2023-04-30 20:49:38.000000 edge-tts-6.1.4/src/edge_tts.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       46 2023-04-30 20:49:38.000000 edge-tts-6.1.4/src/edge_tts.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       23 2023-04-30 20:49:38.000000 edge-tts-6.1.4/src/edge_tts.egg-info/top_level.txt
```

### Comparing `edge-tts-6.1.3/.github/workflows/code-quality.yml` & `edge-tts-6.1.4/.github/workflows/code-quality.yml`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.3/.github/workflows/codeql-analysis.yml` & `edge-tts-6.1.4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.3/.gitignore` & `edge-tts-6.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.3/LICENSE` & `edge-tts-6.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.3/PKG-INFO` & `edge-tts-6.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-tts
-Version: 6.1.3
+Version: 6.1.4
 Summary: Microsoft Edge's TTS
 Home-page: https://github.com/rany2/edge-tts
 Author: rany
 Author-email: ranygh@riseup.net
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/rany2/edge-tts/issues
 Platform: UNKNOWN
```

### Comparing `edge-tts-6.1.3/README.md` & `edge-tts-6.1.4/README.md`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.3/examples/basic_audio_streaming.py` & `edge-tts-6.1.4/examples/basic_audio_streaming.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,8 +27,12 @@
             if chunk["type"] == "audio":
                 file.write(chunk["data"])
             elif chunk["type"] == "WordBoundary":
                 print(f"WordBoundary: {chunk}")
 
 
 if __name__ == "__main__":
-    asyncio.get_event_loop().run_until_complete(_main())
+    loop = asyncio.get_event_loop()
+    try:
+        loop.run_until_complete(_main())
+    finally:
+        loop.close()
```

### Comparing `edge-tts-6.1.3/examples/dynamic_voice_selection.py` & `edge-tts-6.1.4/examples/dynamic_voice_selection.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,8 +21,12 @@
     # voice = voices.find(Gender="Female", Locale="es-AR")
 
     communicate = edge_tts.Communicate(TEXT, random.choice(voice)["Name"])
     await communicate.save(OUTPUT_FILE)
 
 
 if __name__ == "__main__":
-    asyncio.get_event_loop().run_until_complete(_main())
+    loop = asyncio.get_event_loop()
+    try:
+        loop.run_until_complete(_main())
+    finally:
+        loop.close()
```

### Comparing `edge-tts-6.1.3/examples/streaming_with_subtitles.py` & `edge-tts-6.1.4/examples/streaming_with_subtitles.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,8 +28,12 @@
                 submaker.create_sub((chunk["offset"], chunk["duration"]), chunk["text"])
 
     with open(WEBVTT_FILE, "w", encoding="utf-8") as file:
         file.write(submaker.generate_subs())
 
 
 if __name__ == "__main__":
-    asyncio.get_event_loop().run_until_complete(_main())
+    loop = asyncio.get_event_loop()
+    try:
+        loop.run_until_complete(_main())
+    finally:
+        loop.close()
```

### Comparing `edge-tts-6.1.3/mypy.ini` & `edge-tts-6.1.4/mypy.ini`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.3/pylintrc` & `edge-tts-6.1.4/pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -279,18 +279,18 @@
 # Maximum number of attributes for a class (see R0902).
 max-attributes=7
 
 # Maximum number of boolean expressions in an if statement (see R0916).
 max-bool-expr=5
 
 # Maximum number of branch for function / method body.
-max-branches=16
+max-branches=20
 
 # Maximum number of locals for function / method body.
-max-locals=18
+max-locals=20
 
 # Maximum number of parents for a class (see R0901).
 max-parents=7
 
 # Maximum number of public methods for a class (see R0904).
 max-public-methods=20
 
@@ -323,15 +323,15 @@
 indent-after-paren=4
 
 # String used as indentation unit. This is usually "    " (4 spaces) or "\t" (1
 # tab).
 indent-string='    '
 
 # Maximum number of characters on a single line.
-max-line-length=100
+max-line-length=240
 
 # Maximum number of lines in a module.
 max-module-lines=1000
 
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
```

### Comparing `edge-tts-6.1.3/setup.cfg` & `edge-tts-6.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.3/src/edge_playback/__main__.py` & `edge-tts-6.1.4/src/edge_playback/__main__.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.3/src/edge_tts/communicate.py` & `edge-tts-6.1.4/src/edge_tts/communicate.py`

 * *Files 3% similar despite different names*

```diff
@@ -410,19 +410,29 @@
                             )
                     elif received.type == aiohttp.WSMsgType.BINARY:
                         if not download_audio:
                             raise UnexpectedResponse(
                                 "We received a binary message, but we are not expecting one."
                             )
 
+                        if len(received.data) < 2:
+                            raise UnexpectedResponse(
+                                "We received a binary message, but it is missing the header length."
+                            )
+
+                        # See: https://github.com/microsoft/cognitive-services-speech-sdk-js/blob/d071d11/src/common.speech/WebsocketMessageFormatter.ts#L46
+                        header_length = int.from_bytes(received.data[:2], "big")
+                        if len(received.data) < header_length + 2:
+                            raise UnexpectedResponse(
+                                "We received a binary message, but it is missing the audio data."
+                            )
+
                         yield {
                             "type": "audio",
-                            "data": received.data[
-                                received.data.find(b"Path:audio\r\n") + 12 :
-                            ],
+                            "data": received.data[header_length + 2 :],
                         }
                         audio_was_received = True
                     elif received.type == aiohttp.WSMsgType.ERROR:
                         raise WebSocketError(
                             received.data if received.data else "Unknown error"
                         )
```

### Comparing `edge-tts-6.1.3/src/edge_tts/exceptions.py` & `edge-tts-6.1.4/src/edge_tts/exceptions.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.3/src/edge_tts/list_voices.py` & `edge-tts-6.1.4/src/edge_tts/list_voices.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.3/src/edge_tts/submaker.py` & `edge-tts-6.1.4/src/edge_tts/submaker.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 """
 
 import math
 from typing import List, Tuple
 from xml.sax.saxutils import escape, unescape
 
 
-def formatter(offset1: float, offset2: float, subdata: str) -> str:
+def formatter(start_time: float, end_time: float, subdata: str) -> str:
     """
     formatter returns the timecode and the text of the subtitle.
     """
     return (
-        f"{mktimestamp(offset1)} --> {mktimestamp(offset2)}\r\n"
+        f"{mktimestamp(start_time)} --> {mktimestamp(end_time)}\r\n"
         f"{escape(subdata)}\r\n\r\n"
     )
 
 
 def mktimestamp(time_unit: float) -> str:
     """
     mktimestamp returns the timecode of the subtitle.
@@ -36,25 +36,20 @@
 
 
 class SubMaker:
     """
     SubMaker class
     """
 
-    def __init__(self, overlapping: int = 0) -> None:
+    def __init__(self) -> None:
         """
         SubMaker constructor.
-
-        Args:
-            overlapping (int): The amount of time in seconds that the
-                               subtitles should overlap.
         """
         self.offset: List[Tuple[float, float]] = []
         self.subs: List[str] = []
-        self.overlapping: int = overlapping * (10**7)
 
     def create_sub(self, timestamp: Tuple[float, float], text: str) -> None:
         """
         create_sub creates a subtitle with the given timestamp and text
         and adds it to the list of subtitles
 
         Args:
@@ -63,41 +58,68 @@
 
         Returns:
             None
         """
         self.offset.append((timestamp[0], timestamp[0] + timestamp[1]))
         self.subs.append(text)
 
-    def generate_subs(self) -> str:
+    def generate_subs(self, words_in_cue: int = 10) -> str:
         """
         generate_subs generates the complete subtitle file.
 
+        Args:
+            words_in_cue (int): defines the number of words in a given cue
+
         Returns:
             str: The complete subtitle file.
         """
-        if len(self.subs) == len(self.offset):
-            data = "WEBVTT\r\n\r\n"
-            for offset, subs in zip(self.offset, self.subs):
-                subs = unescape(subs)
+        if len(self.subs) != len(self.offset):
+            raise ValueError("subs and offset are not of the same length")
+
+        if words_in_cue <= 0:
+            raise ValueError("words_in_cue must be greater than 0")
+
+        data = "WEBVTT\r\n\r\n"
+        sub_state_count = 0
+        sub_state_start = -1.0
+        sub_state_subs = ""
+        for idx, (offset, subs) in enumerate(zip(self.offset, self.subs)):
+            start_time, end_time = offset
+            subs = unescape(subs)
+
+            # wordboundary is guaranteed not to contain whitespace
+            if len(sub_state_subs) > 0:
+                sub_state_subs += " "
+            sub_state_subs += subs
+
+            if sub_state_start == -1.0:
+                sub_state_start = start_time
+            sub_state_count += 1
+
+            if sub_state_count == words_in_cue or idx == len(self.offset) - 1:
+                subs = sub_state_subs
                 split_subs: List[str] = [
                     subs[i : i + 79] for i in range(0, len(subs), 79)
                 ]
-
                 for i in range(len(split_subs) - 1):
                     sub = split_subs[i]
                     split_at_word = True
                     if sub[-1] == " ":
                         split_subs[i] = sub[:-1]
                         split_at_word = False
 
                     if sub[0] == " ":
                         split_subs[i] = sub[1:]
                         split_at_word = False
 
                     if split_at_word:
                         split_subs[i] += "-"
 
-                subs = "\r\n".join(split_subs)
-
-                data += formatter(offset[0], offset[1] + self.overlapping, subs)
-            return data
-        return ""
+                data += formatter(
+                    start_time=sub_state_start,
+                    end_time=end_time,
+                    subdata="\r\n".join(split_subs),
+                )
+                sub_state_count = 0
+                sub_state_start = -1
+                sub_state_subs = ""
+        return data
```

### Comparing `edge-tts-6.1.3/src/edge_tts.egg-info/PKG-INFO` & `edge-tts-6.1.4/src/edge_tts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-tts
-Version: 6.1.3
+Version: 6.1.4
 Summary: Microsoft Edge's TTS
 Home-page: https://github.com/rany2/edge-tts
 Author: rany
 Author-email: ranygh@riseup.net
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/rany2/edge-tts/issues
 Platform: UNKNOWN
```

### Comparing `edge-tts-6.1.3/src/edge_tts.egg-info/SOURCES.txt` & `edge-tts-6.1.4/src/edge_tts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

