# Comparing `tmp/nure-2023.4.27.tar.gz` & `tmp/nure-2023.4.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nure-2023.4.27.tar", last modified: Thu Apr 27 06:52:27 2023, max compression
+gzip compressed data, was "nure-2023.4.30.tar", last modified: Sun Apr 30 02:30:15 2023, max compression
```

## Comparing `nure-2023.4.27.tar` & `nure-2023.4.30.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-27 06:52:26.389725 nure-2023.4.27/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)    35149 2021-05-21 04:50:18.000000 nure-2023.4.27/LICENSE
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      612 2023-04-27 06:52:26.390870 nure-2023.4.27/PKG-INFO
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)       30 2021-05-21 04:25:06.000000 nure-2023.4.27/README.md
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-27 06:52:25.875040 nure-2023.4.27/nure/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2021-05-21 05:41:00.000000 nure-2023.4.27/nure/__init__.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2523 2021-11-20 09:30:50.000000 nure-2023.4.27/nure/archive.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2379 2021-11-30 04:05:06.000000 nure-2023.4.27/nure/array.py
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-27 06:52:25.915948 nure-2023.4.27/nure/code/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)       62 2021-07-13 10:11:18.000000 nure-2023.4.27/nure/code/__init__.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1353 2021-07-13 16:16:01.000000 nure-2023.4.27/nure/code/label_coder.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     4912 2022-07-29 07:41:08.000000 nure-2023.4.27/nure/dataframe.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1263 2021-07-21 05:24:39.000000 nure-2023.4.27/nure/datetime.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      106 2021-05-21 06:28:06.000000 nure-2023.4.27/nure/debug.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1325 2022-11-14 10:39:27.000000 nure-2023.4.27/nure/dict.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      487 2021-11-30 04:03:48.000000 nure-2023.4.27/nure/func.py
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-27 06:52:26.005656 nure-2023.4.27/nure/image/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2022-04-14 09:32:11.000000 nure-2023.4.27/nure/image/__init__.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)    10331 2022-04-14 09:44:09.000000 nure-2023.4.27/nure/image/annotate.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     6438 2022-04-14 09:32:48.000000 nure-2023.4.27/nure/image/func.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     5944 2023-04-27 06:39:33.000000 nure-2023.4.27/nure/image/pil.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1457 2022-03-22 08:57:21.000000 nure-2023.4.27/nure/meta.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      445 2021-05-21 04:25:40.000000 nure-2023.4.27/nure/path.py
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-27 06:52:26.176942 nure-2023.4.27/nure/sync/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2021-05-21 05:53:57.000000 nure-2023.4.27/nure/sync/__init__.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      457 2021-05-21 09:16:57.000000 nure-2023.4.27/nure/sync/bigquery.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1628 2021-11-30 04:09:01.000000 nure-2023.4.27/nure/sync/cache.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3249 2021-07-23 06:18:01.000000 nure-2023.4.27/nure/sync/googlesheet.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      706 2021-05-21 09:17:03.000000 nure-2023.4.27/nure/sync/postgre.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3055 2023-04-27 06:21:53.000000 nure-2023.4.27/nure/sync/s3.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1806 2022-09-18 04:11:30.000000 nure-2023.4.27/nure/sync/sql.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1450 2021-09-17 11:26:33.000000 nure-2023.4.27/nure/sync/suffix.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2872 2021-11-05 14:16:28.000000 nure-2023.4.27/nure/volatitle.py
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-27 06:52:26.254263 nure-2023.4.27/nure.egg-info/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      612 2023-04-27 06:52:25.000000 nure-2023.4.27/nure.egg-info/PKG-INFO
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      842 2023-04-27 06:52:25.000000 nure-2023.4.27/nure.egg-info/SOURCES.txt
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        1 2023-04-27 06:52:25.000000 nure-2023.4.27/nure.egg-info/dependency_links.txt
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      145 2023-04-27 06:52:25.000000 nure-2023.4.27/nure.egg-info/requires.txt
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        5 2023-04-27 06:52:25.000000 nure-2023.4.27/nure.egg-info/top_level.txt
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      103 2021-05-21 04:28:28.000000 nure-2023.4.27/pyproject.toml
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      849 2023-04-27 06:52:26.396545 nure-2023.4.27/setup.cfg
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-27 06:52:26.372464 nure-2023.4.27/tests/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1011 2021-11-20 09:51:16.000000 nure-2023.4.27/tests/test_archive.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1225 2021-09-17 11:28:32.000000 nure-2023.4.27/tests/test_bigquery.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2890 2021-07-13 16:25:33.000000 nure-2023.4.27/tests/test_coder.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      792 2021-07-23 06:18:01.000000 nure-2023.4.27/tests/test_googlesheet.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3698 2021-11-30 04:05:08.000000 nure-2023.4.27/tests/test_parallel.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      708 2021-09-17 11:49:25.000000 nure-2023.4.27/tests/test_postgre.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      655 2021-10-08 07:11:48.000000 nure-2023.4.27/tests/test_s3.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-30 02:30:15.631868 nure-2023.4.30/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)    35149 2021-05-21 04:50:18.000000 nure-2023.4.30/LICENSE
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      612 2023-04-30 02:30:15.632721 nure-2023.4.30/PKG-INFO
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)       30 2021-05-21 04:25:06.000000 nure-2023.4.30/README.md
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-30 02:30:12.644657 nure-2023.4.30/nure/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2021-05-21 05:41:00.000000 nure-2023.4.30/nure/__init__.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2523 2021-11-20 09:30:50.000000 nure-2023.4.30/nure/archive.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2379 2021-11-30 04:05:06.000000 nure-2023.4.30/nure/array.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-30 02:30:12.911885 nure-2023.4.30/nure/code/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)       62 2021-07-13 10:11:18.000000 nure-2023.4.30/nure/code/__init__.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1353 2021-07-13 16:16:01.000000 nure-2023.4.30/nure/code/label_coder.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     4912 2022-07-29 07:41:08.000000 nure-2023.4.30/nure/dataframe.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1263 2021-07-21 05:24:39.000000 nure-2023.4.30/nure/datetime.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      106 2021-05-21 06:28:06.000000 nure-2023.4.30/nure/debug.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1325 2022-11-14 10:39:27.000000 nure-2023.4.30/nure/dict.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      487 2021-11-30 04:03:48.000000 nure-2023.4.30/nure/func.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-30 02:30:13.560700 nure-2023.4.30/nure/image/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2022-04-14 09:32:11.000000 nure-2023.4.30/nure/image/__init__.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)    10331 2022-04-14 09:44:09.000000 nure-2023.4.30/nure/image/annotate.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     6438 2022-04-14 09:32:48.000000 nure-2023.4.30/nure/image/func.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     6060 2023-04-29 16:36:51.000000 nure-2023.4.30/nure/image/pil.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1457 2022-03-22 08:57:21.000000 nure-2023.4.30/nure/meta.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      445 2021-05-21 04:25:40.000000 nure-2023.4.30/nure/path.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-30 02:30:14.592020 nure-2023.4.30/nure/sync/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2021-05-21 05:53:57.000000 nure-2023.4.30/nure/sync/__init__.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      457 2021-05-21 09:16:57.000000 nure-2023.4.30/nure/sync/bigquery.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1628 2021-11-30 04:09:01.000000 nure-2023.4.30/nure/sync/cache.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3249 2021-07-23 06:18:01.000000 nure-2023.4.30/nure/sync/googlesheet.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      706 2021-05-21 09:17:03.000000 nure-2023.4.30/nure/sync/postgre.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3481 2023-04-29 16:38:30.000000 nure-2023.4.30/nure/sync/s3.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1806 2022-09-18 04:11:30.000000 nure-2023.4.30/nure/sync/sql.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1450 2021-09-17 11:26:33.000000 nure-2023.4.30/nure/sync/suffix.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2872 2021-11-05 14:16:28.000000 nure-2023.4.30/nure/volatitle.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-30 02:30:14.982812 nure-2023.4.30/nure.egg-info/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      612 2023-04-30 02:30:08.000000 nure-2023.4.30/nure.egg-info/PKG-INFO
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      842 2023-04-30 02:30:10.000000 nure-2023.4.30/nure.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        1 2023-04-30 02:30:08.000000 nure-2023.4.30/nure.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      145 2023-04-30 02:30:09.000000 nure-2023.4.30/nure.egg-info/requires.txt
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        5 2023-04-30 02:30:09.000000 nure-2023.4.30/nure.egg-info/top_level.txt
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      103 2021-05-21 04:28:28.000000 nure-2023.4.30/pyproject.toml
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      849 2023-04-30 02:30:15.644622 nure-2023.4.30/setup.cfg
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-30 02:30:15.560696 nure-2023.4.30/tests/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1011 2021-11-20 09:51:16.000000 nure-2023.4.30/tests/test_archive.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1225 2021-09-17 11:28:32.000000 nure-2023.4.30/tests/test_bigquery.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2890 2021-07-13 16:25:33.000000 nure-2023.4.30/tests/test_coder.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      792 2021-07-23 06:18:01.000000 nure-2023.4.30/tests/test_googlesheet.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3698 2021-11-30 04:05:08.000000 nure-2023.4.30/tests/test_parallel.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      708 2021-09-17 11:49:25.000000 nure-2023.4.30/tests/test_postgre.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      655 2021-10-08 07:11:48.000000 nure-2023.4.30/tests/test_s3.py
```

### Comparing `nure-2023.4.27/LICENSE` & `nure-2023.4.30/LICENSE`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/PKG-INFO` & `nure-2023.4.30/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nure
-Version: 2023.4.27
+Version: 2023.4.30
 Summary: Data Science Utilities
 Home-page: https://github.com/tranduytrung/nure
 Author: Trung Tran
 Author-email: tranduytrung@outlook.com
 Project-URL: Bug Tracker, https://github.com/tranduytrung/nure/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `nure-2023.4.27/nure/archive.py` & `nure-2023.4.30/nure/archive.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/nure/array.py` & `nure-2023.4.30/nure/array.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/nure/code/label_coder.py` & `nure-2023.4.30/nure/code/label_coder.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/nure/dataframe.py` & `nure-2023.4.30/nure/dataframe.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/nure/datetime.py` & `nure-2023.4.30/nure/datetime.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/nure/dict.py` & `nure-2023.4.30/nure/dict.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/nure/image/annotate.py` & `nure-2023.4.30/nure/image/annotate.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/nure/image/func.py` & `nure-2023.4.30/nure/image/func.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/nure/image/pil.py` & `nure-2023.4.30/nure/image/pil.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import PIL.Image
 import PIL.ImageColor
 import PIL.ImageDraw
 import PIL.ImageFont
 from PIL.Image import Image
-from PIL.ImageFont import ImageFont
+from PIL.ImageFont import ImageFont, FreeTypeFont
 
 from . import func
 
 
 def wrap_text(text, font: ImageFont, width):
     w, _ = font.getsize(text)
     max_char = int((width / w) * len(text))
@@ -163,16 +163,20 @@
     # get font
     if font is None:
         font = PIL.ImageFont.load_default()
 
     if pos in [EDGE_TOP, EDGE_BOTTOM]:
         text_width = image.size[0]
 
-    wrapped_text = wrap_text(text, font, text_width)
-    _, text_height = font.getsize_multiline(wrapped_text)
+    if isinstance(font, FreeTypeFont):
+        wrapped_text = wrap_text(text, font, text_width)
+        _, text_height = font.getsize_multiline(wrapped_text)
+    else:
+        _, text_height = font.getsize(text)
+
     if pos in [EDGE_TOP, EDGE_BOTTOM]:
         image_width = image.size[0]
         image_height = image.size[1] + text_height
     else:
         image_width = image.size[0] + text_width
         image_height = max(image.size[1], text_height)
```

### Comparing `nure-2023.4.27/nure/meta.py` & `nure-2023.4.30/nure/meta.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/nure/sync/cache.py` & `nure-2023.4.30/nure/sync/cache.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/nure/sync/googlesheet.py` & `nure-2023.4.30/nure/sync/googlesheet.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/nure/sync/postgre.py` & `nure-2023.4.30/nure/sync/postgre.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/nure/sync/s3.py` & `nure-2023.4.30/nure/sync/s3.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 import re
-from typing import Union
+from io import BytesIO
+from typing import Union, BinaryIO
 
 import boto3
+import botocore.exceptions
+
 import nure.path
 import nure.sync.cache
-import botocore.exceptions
 
 
 class S3Uri:
     def __init__(self, bucket: str, key: str) -> None:
         self.bucket = bucket
         self.key = key
 
@@ -39,14 +41,16 @@
     def __repr__(self) -> str:
         return f'S3Uri({self.bucket}, {self.key})'
 
 
 class S3(nure.sync.cache.LocalFileCache):
     def __init__(self, root_path='data/s3', ttl=None) -> None:
         super(S3, self).__init__(root_path, ttl)
+        s3 = boto3.resource('s3')
+        self.client = s3.meta.client
 
     @staticmethod
     def _to_s3uri_(s3_uri: Union[str, S3Uri]):
         # unify s3_uri type
         if isinstance(s3_uri, str):
             s3_uri = S3Uri.parse(s3_uri)
 
@@ -55,43 +59,51 @@
     def key_to_local_relative_path(self, s3_uri: Union[str, S3Uri], *args, **kargs) -> str:
         s3_uri = S3._to_s3uri_(s3_uri)
         return os.path.join(s3_uri.bucket, s3_uri.key)
 
     def retrieve(self, s3_uri: Union[str, S3Uri], local_file_path):
         s3_uri = S3._to_s3uri_(s3_uri)
 
-        s3 = boto3.resource('s3')
-        s3.meta.client.download_file(s3_uri.bucket, s3_uri.key, local_file_path)
+        self.client.download_file(s3_uri.bucket, s3_uri.key, local_file_path)
 
     def _infer_s3uri_(self, local_file_path):
         relative_path = os.path.relpath(local_file_path, self.root_path)
         components = nure.path.splitall(relative_path)
         bucket = components[0]
         key = '/'.join(components[1:])
 
         return S3Uri(bucket, key)
 
-    def upload(self, local_file_path, s3_uri=None):
+    def upload(self, local_file_path, s3_uri: Union[str, S3Uri] = None):
         if s3_uri is None:
             s3_uri = self._infer_s3uri_(local_file_path)
         else:
             s3_uri = S3._to_s3uri_(s3_uri)
 
-        s3 = boto3.resource('s3')
-        s3.meta.client.upload_file(local_file_path, s3_uri.bucket, s3_uri.key)
+        self.client.upload_file(local_file_path, s3_uri.bucket, s3_uri.key)
 
         return s3_uri
 
+    def read(self, s3_uri: Union[str, S3Uri]):
+        s3_uri = S3._to_s3uri_(s3_uri)
+        buffer = BytesIO()
+        self.client.download_fileobj(s3_uri.bucket, s3_uri.key, buffer)
+        buffer.seek(0)
+        return buffer
+
+    def write(self, file_obj: BinaryIO, s3_uri: Union[str, S3Uri]):
+        s3_uri = S3._to_s3uri_(s3_uri)
+        self.client.upload_fileobj(file_obj, s3_uri.bucket, s3_uri.key)
+
     def metadata(self, s3_uri: Union[str, S3Uri]):
         if isinstance(s3_uri, str):
             s3_uri = S3Uri.parse(s3_uri)
 
-        s3 = boto3.resource('s3')
         try:
-            meta = s3.meta.client.head_object(Bucket=s3_uri.bucket, Key=s3_uri.key)
+            meta = self.client.head_object(Bucket=s3_uri.bucket, Key=s3_uri.key)
         except botocore.exceptions.ClientError as e:
             if e.response['Error']['Code'] == '404':
                 return None
 
             raise e
 
         return meta
```

### Comparing `nure-2023.4.27/nure/sync/sql.py` & `nure-2023.4.30/nure/sync/sql.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/nure/sync/suffix.py` & `nure-2023.4.30/nure/sync/suffix.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/nure/volatitle.py` & `nure-2023.4.30/nure/volatitle.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/nure.egg-info/PKG-INFO` & `nure-2023.4.30/nure.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nure
-Version: 2023.4.27
+Version: 2023.4.30
 Summary: Data Science Utilities
 Home-page: https://github.com/tranduytrung/nure
 Author: Trung Tran
 Author-email: tranduytrung@outlook.com
 Project-URL: Bug Tracker, https://github.com/tranduytrung/nure/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `nure-2023.4.27/nure.egg-info/SOURCES.txt` & `nure-2023.4.30/nure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/setup.cfg` & `nure-2023.4.30/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nure
-version = 2023.04.27
+version = 2023.04.30
 author = Trung Tran
 author_email = tranduytrung@outlook.com
 description = Data Science Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tranduytrung/nure
 project_urls =
```

### Comparing `nure-2023.4.27/tests/test_archive.py` & `nure-2023.4.30/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/tests/test_bigquery.py` & `nure-2023.4.30/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/tests/test_coder.py` & `nure-2023.4.30/tests/test_coder.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/tests/test_googlesheet.py` & `nure-2023.4.30/tests/test_googlesheet.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/tests/test_parallel.py` & `nure-2023.4.30/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/tests/test_postgre.py` & `nure-2023.4.30/tests/test_postgre.py`

 * *Files identical despite different names*

### Comparing `nure-2023.4.27/tests/test_s3.py` & `nure-2023.4.30/tests/test_s3.py`

 * *Files identical despite different names*

