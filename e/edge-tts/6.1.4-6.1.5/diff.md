# Comparing `tmp/edge-tts-6.1.4.tar.gz` & `tmp/edge-tts-6.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge-tts-6.1.4.tar", last modified: Sun Apr 30 20:49:38 2023, max compression
+gzip compressed data, was "edge-tts-6.1.5.tar", last modified: Sun Apr 30 20:57:05 2023, max compression
```

## Comparing `edge-tts-6.1.4.tar` & `edge-tts-6.1.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:49:38.163035 edge-tts-6.1.4/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:49:38.163035 edge-tts-6.1.4/.github/
--rw-rw-r--   0 user      (1000) user      (1000)      106 2022-09-27 09:16:55.000000 edge-tts-6.1.4/.github/dependabot.yml
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:49:38.163035 edge-tts-6.1.4/.github/workflows/
--rw-rw-r--   0 user      (1000) user      (1000)      585 2023-01-05 05:52:51.000000 edge-tts-6.1.4/.github/workflows/code-quality.yml
--rw-rw-r--   0 user      (1000) user      (1000)     2277 2022-09-27 09:17:01.000000 edge-tts-6.1.4/.github/workflows/codeql-analysis.yml
--rw-rw-r--   0 user      (1000) user      (1000)     3078 2023-01-05 05:54:43.000000 edge-tts-6.1.4/.gitignore
--rw-rw-r--   0 user      (1000) user      (1000)      161 2023-01-04 23:46:51.000000 edge-tts-6.1.4/.isort.cfg
--rw-------   0 user      (1000) user      (1000)    35149 2021-12-03 12:08:58.000000 edge-tts-6.1.4/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     3873 2023-04-30 20:49:38.163035 edge-tts-6.1.4/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     3319 2023-01-05 23:12:21.000000 edge-tts-6.1.4/README.md
--rwx------   0 user      (1000) user      (1000)      136 2023-01-05 05:59:23.000000 edge-tts-6.1.4/build_and_publish.sh
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:49:38.163035 edge-tts-6.1.4/examples/
--rw-rw-r--   0 user      (1000) user      (1000)      957 2023-04-26 22:07:39.000000 edge-tts-6.1.4/examples/basic_audio_streaming.py
--rw-rw-r--   0 user      (1000) user      (1000)      444 2023-04-26 22:07:39.000000 edge-tts-6.1.4/examples/basic_generation.py
--rw-rw-r--   0 user      (1000) user      (1000)      706 2023-04-26 22:07:39.000000 edge-tts-6.1.4/examples/dynamic_voice_selection.py
--rw-rw-r--   0 user      (1000) user      (1000)     1022 2023-04-26 22:07:39.000000 edge-tts-6.1.4/examples/streaming_with_subtitles.py
--rwxrwxr-x   0 user      (1000) user      (1000)       99 2023-01-04 23:47:18.000000 edge-tts-6.1.4/format.sh
--rwxrwxr-x   0 user      (1000) user      (1000)      108 2023-01-20 00:45:15.000000 edge-tts-6.1.4/lint.sh
--rw-rw-r--   0 user      (1000) user      (1000)      561 2023-01-04 23:38:10.000000 edge-tts-6.1.4/mypy.ini
--rw-rw-r--   0 user      (1000) user      (1000)    20395 2023-04-30 20:48:15.000000 edge-tts-6.1.4/pylintrc
--rw-rw-r--   0 user      (1000) user      (1000)      834 2023-04-30 20:49:38.163035 edge-tts-6.1.4/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      192 2023-01-04 23:17:58.000000 edge-tts-6.1.4/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:49:38.163035 edge-tts-6.1.4/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:49:38.163035 edge-tts-6.1.4/src/edge_playback/
--rw-rw-r--   0 user      (1000) user      (1000)      109 2023-01-05 05:52:51.000000 edge-tts-6.1.4/src/edge_playback/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2053 2023-01-10 14:38:06.000000 edge-tts-6.1.4/src/edge_playback/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-04 23:17:58.000000 edge-tts-6.1.4/src/edge_playback/py.typed
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:49:38.163035 edge-tts-6.1.4/src/edge_tts/
--rw-rw-r--   0 user      (1000) user      (1000)      317 2023-01-09 19:17:13.000000 edge-tts-6.1.4/src/edge_tts/__init__.py
--rw-------   0 user      (1000) user      (1000)       94 2021-12-07 19:17:40.000000 edge-tts-6.1.4/src/edge_tts/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)    17073 2023-04-30 20:46:32.000000 edge-tts-6.1.4/src/edge_tts/communicate.py
--rw-rw-r--   0 user      (1000) user      (1000)      416 2023-01-05 05:52:51.000000 edge-tts-6.1.4/src/edge_tts/constants.py
--rw-rw-r--   0 user      (1000) user      (1000)      558 2023-04-05 13:39:33.000000 edge-tts-6.1.4/src/edge_tts/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2587 2023-01-09 16:29:31.000000 edge-tts-6.1.4/src/edge_tts/list_voices.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-05 04:26:59.000000 edge-tts-6.1.4/src/edge_tts/py.typed
--rw-rw-r--   0 user      (1000) user      (1000)     3823 2023-04-05 14:00:08.000000 edge-tts-6.1.4/src/edge_tts/submaker.py
--rw-rw-r--   0 user      (1000) user      (1000)     4343 2023-04-30 20:40:58.000000 edge-tts-6.1.4/src/edge_tts/util.py
--rw-rw-r--   0 user      (1000) user      (1000)      128 2023-04-30 20:49:15.000000 edge-tts-6.1.4/src/edge_tts/version.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:49:38.163035 edge-tts-6.1.4/src/edge_tts.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3873 2023-04-30 20:49:38.000000 edge-tts-6.1.4/src/edge_tts.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      903 2023-04-30 20:49:38.000000 edge-tts-6.1.4/src/edge_tts.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-30 20:49:38.000000 edge-tts-6.1.4/src/edge_tts.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       98 2023-04-30 20:49:38.000000 edge-tts-6.1.4/src/edge_tts.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       46 2023-04-30 20:49:38.000000 edge-tts-6.1.4/src/edge_tts.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       23 2023-04-30 20:49:38.000000 edge-tts-6.1.4/src/edge_tts.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:57:05.573858 edge-tts-6.1.5/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:57:05.573858 edge-tts-6.1.5/.github/
+-rw-rw-r--   0 user      (1000) user      (1000)      106 2022-09-27 09:16:55.000000 edge-tts-6.1.5/.github/dependabot.yml
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:57:05.573858 edge-tts-6.1.5/.github/workflows/
+-rw-rw-r--   0 user      (1000) user      (1000)      585 2023-01-05 05:52:51.000000 edge-tts-6.1.5/.github/workflows/code-quality.yml
+-rw-rw-r--   0 user      (1000) user      (1000)     2277 2022-09-27 09:17:01.000000 edge-tts-6.1.5/.github/workflows/codeql-analysis.yml
+-rw-rw-r--   0 user      (1000) user      (1000)     3078 2023-01-05 05:54:43.000000 edge-tts-6.1.5/.gitignore
+-rw-rw-r--   0 user      (1000) user      (1000)      161 2023-01-04 23:46:51.000000 edge-tts-6.1.5/.isort.cfg
+-rw-------   0 user      (1000) user      (1000)    35149 2021-12-03 12:08:58.000000 edge-tts-6.1.5/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     4031 2023-04-30 20:57:05.573858 edge-tts-6.1.5/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     3477 2023-04-30 20:56:25.000000 edge-tts-6.1.5/README.md
+-rwx------   0 user      (1000) user      (1000)      136 2023-01-05 05:59:23.000000 edge-tts-6.1.5/build_and_publish.sh
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:57:05.573858 edge-tts-6.1.5/examples/
+-rw-rw-r--   0 user      (1000) user      (1000)      957 2023-04-26 22:07:39.000000 edge-tts-6.1.5/examples/basic_audio_streaming.py
+-rw-rw-r--   0 user      (1000) user      (1000)      444 2023-04-26 22:07:39.000000 edge-tts-6.1.5/examples/basic_generation.py
+-rw-rw-r--   0 user      (1000) user      (1000)      706 2023-04-26 22:07:39.000000 edge-tts-6.1.5/examples/dynamic_voice_selection.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1022 2023-04-26 22:07:39.000000 edge-tts-6.1.5/examples/streaming_with_subtitles.py
+-rwxrwxr-x   0 user      (1000) user      (1000)       99 2023-01-04 23:47:18.000000 edge-tts-6.1.5/format.sh
+-rwxrwxr-x   0 user      (1000) user      (1000)      108 2023-01-20 00:45:15.000000 edge-tts-6.1.5/lint.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      561 2023-01-04 23:38:10.000000 edge-tts-6.1.5/mypy.ini
+-rw-rw-r--   0 user      (1000) user      (1000)    20395 2023-04-30 20:48:15.000000 edge-tts-6.1.5/pylintrc
+-rw-rw-r--   0 user      (1000) user      (1000)      834 2023-04-30 20:57:05.573858 edge-tts-6.1.5/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      192 2023-01-04 23:17:58.000000 edge-tts-6.1.5/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:57:05.573858 edge-tts-6.1.5/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:57:05.573858 edge-tts-6.1.5/src/edge_playback/
+-rw-rw-r--   0 user      (1000) user      (1000)      109 2023-01-05 05:52:51.000000 edge-tts-6.1.5/src/edge_playback/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2053 2023-01-10 14:38:06.000000 edge-tts-6.1.5/src/edge_playback/__main__.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-04 23:17:58.000000 edge-tts-6.1.5/src/edge_playback/py.typed
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:57:05.573858 edge-tts-6.1.5/src/edge_tts/
+-rw-rw-r--   0 user      (1000) user      (1000)      317 2023-01-09 19:17:13.000000 edge-tts-6.1.5/src/edge_tts/__init__.py
+-rw-------   0 user      (1000) user      (1000)       94 2021-12-07 19:17:40.000000 edge-tts-6.1.5/src/edge_tts/__main__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17073 2023-04-30 20:46:32.000000 edge-tts-6.1.5/src/edge_tts/communicate.py
+-rw-rw-r--   0 user      (1000) user      (1000)      416 2023-01-05 05:52:51.000000 edge-tts-6.1.5/src/edge_tts/constants.py
+-rw-rw-r--   0 user      (1000) user      (1000)      558 2023-04-05 13:39:33.000000 edge-tts-6.1.5/src/edge_tts/exceptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2587 2023-01-09 16:29:31.000000 edge-tts-6.1.5/src/edge_tts/list_voices.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-05 04:26:59.000000 edge-tts-6.1.5/src/edge_tts/py.typed
+-rw-rw-r--   0 user      (1000) user      (1000)     3823 2023-04-05 14:00:08.000000 edge-tts-6.1.5/src/edge_tts/submaker.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4343 2023-04-30 20:40:58.000000 edge-tts-6.1.5/src/edge_tts/util.py
+-rw-rw-r--   0 user      (1000) user      (1000)      128 2023-04-30 20:56:50.000000 edge-tts-6.1.5/src/edge_tts/version.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:57:05.573858 edge-tts-6.1.5/src/edge_tts.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     4031 2023-04-30 20:57:05.000000 edge-tts-6.1.5/src/edge_tts.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      903 2023-04-30 20:57:05.000000 edge-tts-6.1.5/src/edge_tts.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-30 20:57:05.000000 edge-tts-6.1.5/src/edge_tts.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       98 2023-04-30 20:57:05.000000 edge-tts-6.1.5/src/edge_tts.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       46 2023-04-30 20:57:05.000000 edge-tts-6.1.5/src/edge_tts.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       23 2023-04-30 20:57:05.000000 edge-tts-6.1.5/src/edge_tts.egg-info/top_level.txt
```

### Comparing `edge-tts-6.1.4/.github/workflows/code-quality.yml` & `edge-tts-6.1.5/.github/workflows/code-quality.yml`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.4/.github/workflows/codeql-analysis.yml` & `edge-tts-6.1.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.4/.gitignore` & `edge-tts-6.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.4/LICENSE` & `edge-tts-6.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.4/PKG-INFO` & `edge-tts-6.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-tts
-Version: 6.1.4
+Version: 6.1.5
 Summary: Microsoft Edge's TTS
 Home-page: https://github.com/rany2/edge-tts
 Author: rany
 Author-email: ranygh@riseup.net
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/rany2/edge-tts/issues
 Platform: UNKNOWN
@@ -32,15 +32,15 @@
 
 ## Usage
 
 ### Basic usage
 
 If you want to use the `edge-tts` command, you can simply run it with the following command:
 
-    $ edge-tts --text "Hello, world!" --write-media hello.mp3
+    $ edge-tts --text "Hello, world!" --write-media hello.mp3 --write-subtitles hello.vtt
 
 If you wish to play it back immediately with subtitles, you could use the `edge-playback` command:
 
     $ edge-playback --text "Hello, world!"
 
 Note the above requires the installation of the `mpv` command line player.
 
@@ -71,26 +71,26 @@
     Name: Microsoft Server Speech Text to Speech Voice (ar-SA, ZariyahNeural)
     ShortName: ar-SA-ZariyahNeural
     Gender: Female
     Locale: ar-SA
 
     ...
 
-    $ edge-tts --voice ar-EG-SalmaNeural --text "مرحبا كيف حالك؟" --write-media hello_in_arabic.mp3
+    $ edge-tts --voice ar-EG-SalmaNeural --text "مرحبا كيف حالك؟" --write-media hello_in_arabic.mp3 --write-subtitles hello_in_arabic.vtt
 
 ### Custom SSML
 
 Support for custom SSML has been removed since 5.0.0 because Microsoft has taken the initiative to prevent it from working. You cannot use custom SSML anymore.
 
 ### Changing rate and volume
 
 It is possible to make minor changes to the generated speech.
 
-    $ edge-tts --rate=-50% --text "Hello, world!" --write-media hello_with_rate_halved.mp3
-    $ edge-tts --volume=-50% --text "Hello, world!" --write-media hello_with_volume_halved.mp3
+    $ edge-tts --rate=-50% --text "Hello, world!" --write-media hello_with_rate_halved.mp3 --write-subtitles hello_with_rate_halved.vtt
+    $ edge-tts --volume=-50% --text "Hello, world!" --write-media hello_with_volume_halved.mp3 --write-subtitles hello_with_volume_halved.vtt
 
 In addition, it is required to use `--rate=-50%` instead of `--rate -50%` (note the lack of an equal sign) otherwise the `-50%` would be interpreted as just another argument.
 
 **NOTE**: `--pitch` was removed in 6.0.3 as it no longer appears to have any effect.
 
 ### Note on the `edge-playback` command
```

### Comparing `edge-tts-6.1.4/README.md` & `edge-tts-6.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ## Usage
 
 ### Basic usage
 
 If you want to use the `edge-tts` command, you can simply run it with the following command:
 
-    $ edge-tts --text "Hello, world!" --write-media hello.mp3
+    $ edge-tts --text "Hello, world!" --write-media hello.mp3 --write-subtitles hello.vtt
 
 If you wish to play it back immediately with subtitles, you could use the `edge-playback` command:
 
     $ edge-playback --text "Hello, world!"
 
 Note the above requires the installation of the `mpv` command line player.
 
@@ -53,26 +53,26 @@
     Name: Microsoft Server Speech Text to Speech Voice (ar-SA, ZariyahNeural)
     ShortName: ar-SA-ZariyahNeural
     Gender: Female
     Locale: ar-SA
 
     ...
 
-    $ edge-tts --voice ar-EG-SalmaNeural --text "مرحبا كيف حالك؟" --write-media hello_in_arabic.mp3
+    $ edge-tts --voice ar-EG-SalmaNeural --text "مرحبا كيف حالك؟" --write-media hello_in_arabic.mp3 --write-subtitles hello_in_arabic.vtt
 
 ### Custom SSML
 
 Support for custom SSML has been removed since 5.0.0 because Microsoft has taken the initiative to prevent it from working. You cannot use custom SSML anymore.
 
 ### Changing rate and volume
 
 It is possible to make minor changes to the generated speech.
 
-    $ edge-tts --rate=-50% --text "Hello, world!" --write-media hello_with_rate_halved.mp3
-    $ edge-tts --volume=-50% --text "Hello, world!" --write-media hello_with_volume_halved.mp3
+    $ edge-tts --rate=-50% --text "Hello, world!" --write-media hello_with_rate_halved.mp3 --write-subtitles hello_with_rate_halved.vtt
+    $ edge-tts --volume=-50% --text "Hello, world!" --write-media hello_with_volume_halved.mp3 --write-subtitles hello_with_volume_halved.vtt
 
 In addition, it is required to use `--rate=-50%` instead of `--rate -50%` (note the lack of an equal sign) otherwise the `-50%` would be interpreted as just another argument.
 
 **NOTE**: `--pitch` was removed in 6.0.3 as it no longer appears to have any effect.
 
 ### Note on the `edge-playback` command
```

### Comparing `edge-tts-6.1.4/examples/basic_audio_streaming.py` & `edge-tts-6.1.5/examples/basic_audio_streaming.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.4/examples/dynamic_voice_selection.py` & `edge-tts-6.1.5/examples/dynamic_voice_selection.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.4/examples/streaming_with_subtitles.py` & `edge-tts-6.1.5/examples/streaming_with_subtitles.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.4/mypy.ini` & `edge-tts-6.1.5/mypy.ini`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.4/pylintrc` & `edge-tts-6.1.5/pylintrc`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.4/setup.cfg` & `edge-tts-6.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.4/src/edge_playback/__main__.py` & `edge-tts-6.1.5/src/edge_playback/__main__.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.4/src/edge_tts/communicate.py` & `edge-tts-6.1.5/src/edge_tts/communicate.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.4/src/edge_tts/exceptions.py` & `edge-tts-6.1.5/src/edge_tts/exceptions.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.4/src/edge_tts/list_voices.py` & `edge-tts-6.1.5/src/edge_tts/list_voices.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.4/src/edge_tts/submaker.py` & `edge-tts-6.1.5/src/edge_tts/submaker.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.4/src/edge_tts/util.py` & `edge-tts-6.1.5/src/edge_tts/util.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.4/src/edge_tts.egg-info/PKG-INFO` & `edge-tts-6.1.5/src/edge_tts.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-tts
-Version: 6.1.4
+Version: 6.1.5
 Summary: Microsoft Edge's TTS
 Home-page: https://github.com/rany2/edge-tts
 Author: rany
 Author-email: ranygh@riseup.net
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/rany2/edge-tts/issues
 Platform: UNKNOWN
@@ -32,15 +32,15 @@
 
 ## Usage
 
 ### Basic usage
 
 If you want to use the `edge-tts` command, you can simply run it with the following command:
 
-    $ edge-tts --text "Hello, world!" --write-media hello.mp3
+    $ edge-tts --text "Hello, world!" --write-media hello.mp3 --write-subtitles hello.vtt
 
 If you wish to play it back immediately with subtitles, you could use the `edge-playback` command:
 
     $ edge-playback --text "Hello, world!"
 
 Note the above requires the installation of the `mpv` command line player.
 
@@ -71,26 +71,26 @@
     Name: Microsoft Server Speech Text to Speech Voice (ar-SA, ZariyahNeural)
     ShortName: ar-SA-ZariyahNeural
     Gender: Female
     Locale: ar-SA
 
     ...
 
-    $ edge-tts --voice ar-EG-SalmaNeural --text "مرحبا كيف حالك؟" --write-media hello_in_arabic.mp3
+    $ edge-tts --voice ar-EG-SalmaNeural --text "مرحبا كيف حالك؟" --write-media hello_in_arabic.mp3 --write-subtitles hello_in_arabic.vtt
 
 ### Custom SSML
 
 Support for custom SSML has been removed since 5.0.0 because Microsoft has taken the initiative to prevent it from working. You cannot use custom SSML anymore.
 
 ### Changing rate and volume
 
 It is possible to make minor changes to the generated speech.
 
-    $ edge-tts --rate=-50% --text "Hello, world!" --write-media hello_with_rate_halved.mp3
-    $ edge-tts --volume=-50% --text "Hello, world!" --write-media hello_with_volume_halved.mp3
+    $ edge-tts --rate=-50% --text "Hello, world!" --write-media hello_with_rate_halved.mp3 --write-subtitles hello_with_rate_halved.vtt
+    $ edge-tts --volume=-50% --text "Hello, world!" --write-media hello_with_volume_halved.mp3 --write-subtitles hello_with_volume_halved.vtt
 
 In addition, it is required to use `--rate=-50%` instead of `--rate -50%` (note the lack of an equal sign) otherwise the `-50%` would be interpreted as just another argument.
 
 **NOTE**: `--pitch` was removed in 6.0.3 as it no longer appears to have any effect.
 
 ### Note on the `edge-playback` command
```

### Comparing `edge-tts-6.1.4/src/edge_tts.egg-info/SOURCES.txt` & `edge-tts-6.1.5/src/edge_tts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

