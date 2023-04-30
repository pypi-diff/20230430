# Comparing `tmp/toml_tools-1.1.0.tar.gz` & `tmp/toml_tools-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toml_tools-1.1.0.tar", last modified: Sun Apr 30 21:22:52 2023, max compression
+gzip compressed data, was "toml_tools-1.1.1.tar", last modified: Sun Apr 30 21:27:57 2023, max compression
```

## Comparing `toml_tools-1.1.0.tar` & `toml_tools-1.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 21:22:52.692536 toml_tools-1.1.0/
--rw-rw-rw-   0        0        0     1093 2023-04-29 19:23:43.000000 toml_tools-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       88 2023-04-30 11:09:23.000000 toml_tools-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0    14622 2023-04-30 21:22:52.693535 toml_tools-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    13663 2023-04-29 22:35:27.000000 toml_tools-1.1.0/README.md
--rw-rw-rw-   0        0        0      115 2023-04-30 21:22:52.696540 toml_tools-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1282 2023-04-30 21:22:49.000000 toml_tools-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:22:52.647349 toml_tools-1.1.0/tests/
--rw-rw-rw-   0        0        0      425 2023-04-30 13:19:52.000000 toml_tools-1.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     4292 2023-04-30 21:03:53.000000 toml_tools-1.1.0/tests/burntsushi.py
--rw-rw-rw-   0        0        0     2750 2023-04-30 14:27:16.000000 toml_tools-1.1.0/tests/test_data.py
--rw-rw-rw-   0        0        0     2290 2023-04-30 13:05:45.000000 toml_tools-1.1.0/tests/test_error.py
--rw-rw-rw-   0        0        0      910 2023-04-30 13:43:35.000000 toml_tools-1.1.0/tests/test_for_profiler.py
--rw-rw-rw-   0        0        0      439 2023-04-30 13:09:48.000000 toml_tools-1.1.0/tests/test_invalid.py
--rw-rw-rw-   0        0        0     3971 2023-04-30 15:41:55.000000 toml_tools-1.1.0/tests/test_misc.py
--rw-rw-rw-   0        0        0     5612 2023-04-30 13:11:25.000000 toml_tools-1.1.0/tests/test_style.py
--rw-rw-rw-   0        0        0      757 2023-04-30 09:56:38.000000 toml_tools-1.1.0/tests/test_types.py
--rw-rw-rw-   0        0        0     2075 2023-04-30 21:09:47.000000 toml_tools-1.1.0/tests/test_valid.py
--rw-rw-rw-   0        0        0      301 2023-04-30 09:56:56.000000 toml_tools-1.1.0/tests/test_write_file.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:22:52.659540 toml_tools-1.1.0/toml_tools/
--rw-rw-rw-   0        0        0      421 2023-04-30 21:19:11.000000 toml_tools-1.1.0/toml_tools/__init__.py
--rw-rw-rw-   0        0        0      444 2023-04-29 21:12:30.000000 toml_tools-1.1.0/toml_tools/_helpers.py
--rw-rw-rw-   0        0        0    23870 2023-04-30 15:19:52.000000 toml_tools-1.1.0/toml_tools/_parser.py
--rw-rw-rw-   0        0        0     4285 2023-04-30 14:29:54.000000 toml_tools-1.1.0/toml_tools/_re.py
--rw-rw-rw-   0        0        0     6509 2023-04-30 11:54:56.000000 toml_tools-1.1.0/toml_tools/_writer.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:22:52.690541 toml_tools-1.1.0/toml_tools.egg-info/
--rw-rw-rw-   0        0        0    14622 2023-04-30 21:22:52.000000 toml_tools-1.1.0/toml_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      530 2023-04-30 21:22:52.000000 toml_tools-1.1.0/toml_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 21:22:52.000000 toml_tools-1.1.0/toml_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-30 21:22:52.000000 toml_tools-1.1.0/toml_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1271 2023-04-30 21:11:20.000000 toml_tools-1.1.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-04-30 21:27:57.933298 toml_tools-1.1.1/
+-rw-rw-rw-   0        0        0     1093 2023-04-29 19:23:43.000000 toml_tools-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       88 2023-04-30 11:09:23.000000 toml_tools-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    14844 2023-04-30 21:27:57.934291 toml_tools-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    13885 2023-04-30 21:27:23.000000 toml_tools-1.1.1/README.md
+-rw-rw-rw-   0        0        0      115 2023-04-30 21:27:57.937300 toml_tools-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1282 2023-04-30 21:22:49.000000 toml_tools-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:27:57.885291 toml_tools-1.1.1/tests/
+-rw-rw-rw-   0        0        0      425 2023-04-30 13:19:52.000000 toml_tools-1.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     4292 2023-04-30 21:03:53.000000 toml_tools-1.1.1/tests/burntsushi.py
+-rw-rw-rw-   0        0        0     2750 2023-04-30 14:27:16.000000 toml_tools-1.1.1/tests/test_data.py
+-rw-rw-rw-   0        0        0     2290 2023-04-30 13:05:45.000000 toml_tools-1.1.1/tests/test_error.py
+-rw-rw-rw-   0        0        0      910 2023-04-30 13:43:35.000000 toml_tools-1.1.1/tests/test_for_profiler.py
+-rw-rw-rw-   0        0        0      439 2023-04-30 13:09:48.000000 toml_tools-1.1.1/tests/test_invalid.py
+-rw-rw-rw-   0        0        0     3971 2023-04-30 15:41:55.000000 toml_tools-1.1.1/tests/test_misc.py
+-rw-rw-rw-   0        0        0     5612 2023-04-30 13:11:25.000000 toml_tools-1.1.1/tests/test_style.py
+-rw-rw-rw-   0        0        0      757 2023-04-30 09:56:38.000000 toml_tools-1.1.1/tests/test_types.py
+-rw-rw-rw-   0        0        0     2075 2023-04-30 21:09:47.000000 toml_tools-1.1.1/tests/test_valid.py
+-rw-rw-rw-   0        0        0      301 2023-04-30 09:56:56.000000 toml_tools-1.1.1/tests/test_write_file.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:27:57.901294 toml_tools-1.1.1/toml_tools/
+-rw-rw-rw-   0        0        0      421 2023-04-30 21:27:55.000000 toml_tools-1.1.1/toml_tools/__init__.py
+-rw-rw-rw-   0        0        0      444 2023-04-29 21:12:30.000000 toml_tools-1.1.1/toml_tools/_helpers.py
+-rw-rw-rw-   0        0        0    23870 2023-04-30 15:19:52.000000 toml_tools-1.1.1/toml_tools/_parser.py
+-rw-rw-rw-   0        0        0     4285 2023-04-30 14:29:54.000000 toml_tools-1.1.1/toml_tools/_re.py
+-rw-rw-rw-   0        0        0     6509 2023-04-30 11:54:56.000000 toml_tools-1.1.1/toml_tools/_writer.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:27:57.931288 toml_tools-1.1.1/toml_tools.egg-info/
+-rw-rw-rw-   0        0        0    14844 2023-04-30 21:27:57.000000 toml_tools-1.1.1/toml_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      530 2023-04-30 21:27:57.000000 toml_tools-1.1.1/toml_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 21:27:57.000000 toml_tools-1.1.1/toml_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-30 21:27:57.000000 toml_tools-1.1.1/toml_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1271 2023-04-30 21:11:20.000000 toml_tools-1.1.1/tox.ini
```

### Comparing `toml_tools-1.1.0/LICENSE` & `toml_tools-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `toml_tools-1.1.0/PKG-INFO` & `toml_tools-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toml_tools
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tomli and Tomli-W for Python 2 and Iron Python
 Home-page: https://github.com/JamesParrott/toml_tools
 Author: Taneli Hukkinen
 Author-email: hukkin@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,18 @@
 Classifier: Programming Language :: Python :: Implementation :: IronPython
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # toml_tools, Tomli and Tomli-W for Python 2 and Iron Python
 
-v1.0.0 is a complete overhaul.  toml_tools is now based on tomli and tomli-w.
+v1.1.1 - fit for purpose!  Passes 52 of Hukkin's unittest tests, in Python 2 and Iron Python 2.7
+
+v1.0.0 is a complete overhaul - toml_tools is now based on tomli and tomli-w.  Note, unlike toml_tools v0, toml and tomlkit, toml_tools v1 and tomli require files to be opened in bytes mode ('rb').
+
 
 # Parent Project number (1/2)'s Readme File (Tomli)
 
 > A lil' TOML parser
 
 **Table of Contents**  *generated with [mdformat-toc](https://github.com/hukkin/mdformat-toc)*
```

### Comparing `toml_tools-1.1.0/README.md` & `toml_tools-1.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # toml_tools, Tomli and Tomli-W for Python 2 and Iron Python
 
-v1.0.0 is a complete overhaul.  toml_tools is now based on tomli and tomli-w.
+v1.1.1 - fit for purpose!  Passes 52 of Hukkin's unittest tests, in Python 2 and Iron Python 2.7
+
+v1.0.0 is a complete overhaul - toml_tools is now based on tomli and tomli-w.  Note, unlike toml_tools v0, toml and tomlkit, toml_tools v1 and tomli require files to be opened in bytes mode ('rb').
+
 
 # Parent Project number (1/2)'s Readme File (Tomli)
 
 > A lil' TOML parser
 
 **Table of Contents**  *generated with [mdformat-toc](https://github.com/hukkin/mdformat-toc)*
```

### Comparing `toml_tools-1.1.0/setup.py` & `toml_tools-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `toml_tools-1.1.0/tests/burntsushi.py` & `toml_tools-1.1.1/tests/burntsushi.py`

 * *Files identical despite different names*

### Comparing `toml_tools-1.1.0/tests/test_data.py` & `toml_tools-1.1.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `toml_tools-1.1.0/tests/test_error.py` & `toml_tools-1.1.1/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `toml_tools-1.1.0/tests/test_for_profiler.py` & `toml_tools-1.1.1/tests/test_for_profiler.py`

 * *Files identical despite different names*

### Comparing `toml_tools-1.1.0/tests/test_misc.py` & `toml_tools-1.1.1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `toml_tools-1.1.0/tests/test_style.py` & `toml_tools-1.1.1/tests/test_style.py`

 * *Files identical despite different names*

### Comparing `toml_tools-1.1.0/tests/test_types.py` & `toml_tools-1.1.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `toml_tools-1.1.0/tests/test_valid.py` & `toml_tools-1.1.1/tests/test_valid.py`

 * *Files identical despite different names*

### Comparing `toml_tools-1.1.0/toml_tools/_parser.py` & `toml_tools-1.1.1/toml_tools/_parser.py`

 * *Files identical despite different names*

### Comparing `toml_tools-1.1.0/toml_tools/_re.py` & `toml_tools-1.1.1/toml_tools/_re.py`

 * *Files identical despite different names*

### Comparing `toml_tools-1.1.0/toml_tools/_writer.py` & `toml_tools-1.1.1/toml_tools/_writer.py`

 * *Files identical despite different names*

### Comparing `toml_tools-1.1.0/toml_tools.egg-info/PKG-INFO` & `toml_tools-1.1.1/toml_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toml-tools
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tomli and Tomli-W for Python 2 and Iron Python
 Home-page: https://github.com/JamesParrott/toml_tools
 Author: Taneli Hukkinen
 Author-email: hukkin@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,18 @@
 Classifier: Programming Language :: Python :: Implementation :: IronPython
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # toml_tools, Tomli and Tomli-W for Python 2 and Iron Python
 
-v1.0.0 is a complete overhaul.  toml_tools is now based on tomli and tomli-w.
+v1.1.1 - fit for purpose!  Passes 52 of Hukkin's unittest tests, in Python 2 and Iron Python 2.7
+
+v1.0.0 is a complete overhaul - toml_tools is now based on tomli and tomli-w.  Note, unlike toml_tools v0, toml and tomlkit, toml_tools v1 and tomli require files to be opened in bytes mode ('rb').
+
 
 # Parent Project number (1/2)'s Readme File (Tomli)
 
 > A lil' TOML parser
 
 **Table of Contents**  *generated with [mdformat-toc](https://github.com/hukkin/mdformat-toc)*
```

### Comparing `toml_tools-1.1.0/toml_tools.egg-info/SOURCES.txt` & `toml_tools-1.1.1/toml_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `toml_tools-1.1.0/tox.ini` & `toml_tools-1.1.1/tox.ini`

 * *Files identical despite different names*

