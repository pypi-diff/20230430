# Comparing `tmp/stable-ts-2.5.2.tar.gz` & `tmp/stable-ts-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-2.5.2.tar", last modified: Fri Apr 28 17:09:10 2023, max compression
+gzip compressed data, was "stable-ts-2.5.3.tar", last modified: Sun Apr 30 06:29:08 2023, max compression
```

## Comparing `stable-ts-2.5.2.tar` & `stable-ts-2.5.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 17:09:10.134188 stable-ts-2.5.2/
--rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.5.2/LICENSE
--rw-rw-rw-   0        0        0     6890 2023-04-28 17:09:10.133186 stable-ts-2.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     6594 2023-04-04 01:04:16.000000 stable-ts-2.5.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 17:09:10.134188 stable-ts-2.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 17:09:10.076187 stable-ts-2.5.2/stable_ts.egg-info/
--rw-rw-rw-   0        0        0     6890 2023-04-28 17:09:09.000000 stable-ts-2.5.2/stable_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-04-28 17:09:09.000000 stable-ts-2.5.2/stable_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 17:09:09.000000 stable-ts-2.5.2/stable_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-04-28 17:09:09.000000 stable-ts-2.5.2/stable_ts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-04-28 17:09:09.000000 stable-ts-2.5.2/stable_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-28 17:09:09.000000 stable-ts-2.5.2/stable_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-28 17:09:10.131186 stable-ts-2.5.2/stable_whisper/
--rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.5.2/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.5.2/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       23 2023-04-28 17:07:38.000000 stable-ts-2.5.2/stable_whisper/_version.py
--rw-rw-rw-   0        0        0     7619 2023-04-28 17:05:35.000000 stable-ts-2.5.2/stable_whisper/audio.py
--rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.5.2/stable_whisper/decode.py
--rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.5.2/stable_whisper/enhancement.py
--rw-rw-rw-   0        0        0     1645 2023-03-10 21:20:52.000000 stable-ts-2.5.2/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0    34855 2023-04-24 05:25:29.000000 stable-ts-2.5.2/stable_whisper/result.py
--rw-rw-rw-   0        0        0    13168 2023-04-04 00:54:46.000000 stable-ts-2.5.2/stable_whisper/stabilization.py
--rw-rw-rw-   0        0        0    14331 2023-04-18 21:08:14.000000 stable-ts-2.5.2/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.5.2/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.5.2/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0    50492 2023-04-28 16:52:08.000000 stable-ts-2.5.2/stable_whisper/whisper_word_level.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:29:08.204617 stable-ts-2.5.3/
+-rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.5.3/LICENSE
+-rw-rw-rw-   0        0        0     6890 2023-04-30 06:29:08.203617 stable-ts-2.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6594 2023-04-04 01:04:16.000000 stable-ts-2.5.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 06:29:08.204617 stable-ts-2.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:29:08.129209 stable-ts-2.5.3/stable_ts.egg-info/
+-rw-rw-rw-   0        0        0     6890 2023-04-30 06:29:07.000000 stable-ts-2.5.3/stable_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-04-30 06:29:07.000000 stable-ts-2.5.3/stable_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 06:29:07.000000 stable-ts-2.5.3/stable_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-04-30 06:29:07.000000 stable-ts-2.5.3/stable_ts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-04-30 06:29:07.000000 stable-ts-2.5.3/stable_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-30 06:29:07.000000 stable-ts-2.5.3/stable_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 06:29:08.201616 stable-ts-2.5.3/stable_whisper/
+-rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.5.3/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.5.3/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-04-30 06:25:44.000000 stable-ts-2.5.3/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0     7619 2023-04-28 17:05:35.000000 stable-ts-2.5.3/stable_whisper/audio.py
+-rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.5.3/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.5.3/stable_whisper/enhancement.py
+-rw-rw-rw-   0        0        0     1645 2023-03-10 21:20:52.000000 stable-ts-2.5.3/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0    34855 2023-04-24 05:25:29.000000 stable-ts-2.5.3/stable_whisper/result.py
+-rw-rw-rw-   0        0        0    13214 2023-04-30 06:27:10.000000 stable-ts-2.5.3/stable_whisper/stabilization.py
+-rw-rw-rw-   0        0        0    14331 2023-04-18 21:08:14.000000 stable-ts-2.5.3/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.5.3/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.5.3/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0    50492 2023-04-28 16:52:08.000000 stable-ts-2.5.3/stable_whisper/whisper_word_level.py
```

### Comparing `stable-ts-2.5.2/LICENSE` & `stable-ts-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.2/PKG-INFO` & `stable-ts-2.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.5.2
+Version: 2.5.3
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.5.2/README.md` & `stable-ts-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.2/setup.py` & `stable-ts-2.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.2/stable_ts.egg-info/PKG-INFO` & `stable-ts-2.5.3/stable_ts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.5.2
+Version: 2.5.3
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.5.2/stable_ts.egg-info/SOURCES.txt` & `stable-ts-2.5.3/stable_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.2/stable_whisper/audio.py` & `stable-ts-2.5.3/stable_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.2/stable_whisper/decode.py` & `stable-ts-2.5.3/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.2/stable_whisper/enhancement.py` & `stable-ts-2.5.3/stable_whisper/enhancement.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.2/stable_whisper/quantization.py` & `stable-ts-2.5.3/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.2/stable_whisper/result.py` & `stable-ts-2.5.3/stable_whisper/result.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.2/stable_whisper/stabilization.py` & `stable-ts-2.5.3/stable_whisper/stabilization.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,14 +223,16 @@
 
     if q_levels:
         mask = mask.mul(q_levels).round()
 
     mask = mask.bool()
 
     temp_timings = mask2timing(mask)
+    if temp_timings is None:
+        return
     s, e = temp_timings
     se_mask = (e - s) > 0.1
     s = s[se_mask]
     e = e[se_mask]
     mask = ~timing2mask(s, e, loudness_tensor.shape[-1])
 
     if not mask.any():
```

### Comparing `stable-ts-2.5.2/stable_whisper/text_output.py` & `stable-ts-2.5.3/stable_whisper/text_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.2/stable_whisper/timing.py` & `stable-ts-2.5.3/stable_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.2/stable_whisper/video_output.py` & `stable-ts-2.5.3/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.2/stable_whisper/whisper_word_level.py` & `stable-ts-2.5.3/stable_whisper/whisper_word_level.py`

 * *Files identical despite different names*

