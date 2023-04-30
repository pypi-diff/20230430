# Comparing `tmp/terminalplay-1.0.21.tar.gz` & `tmp/terminalplay-1.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminalplay-1.0.21.tar", last modified: Sun Apr 30 07:22:03 2023, max compression
+gzip compressed data, was "terminalplay-1.0.22.tar", last modified: Sun Apr 30 07:29:23 2023, max compression
```

## Comparing `terminalplay-1.0.21.tar` & `terminalplay-1.0.22.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:22:03.163345 terminalplay-1.0.21/
--rw-rw-r--   0 merwin    (1000) merwin    (1000)     1065 2023-04-30 07:02:43.000000 terminalplay-1.0.21/LICENSE.txt
--rw-rw-r--   0 merwin    (1000) merwin    (1000)     1396 2023-04-30 07:22:03.163345 terminalplay-1.0.21/PKG-INFO
--rw-rw-r--   0 merwin    (1000) merwin    (1000)      731 2023-04-30 07:02:59.000000 terminalplay-1.0.21/README.rst
--rw-rw-r--   0 merwin    (1000) merwin    (1000)       38 2023-04-30 07:22:03.163345 terminalplay-1.0.21/setup.cfg
--rw-rw-r--   0 merwin    (1000) merwin    (1000)     1159 2023-04-30 07:21:59.000000 terminalplay-1.0.21/setup.py
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:22:03.163345 terminalplay-1.0.21/terminalplay/
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:22:03.163345 terminalplay-1.0.21/terminalplay/src/
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:22:03.163345 terminalplay-1.0.21/terminalplay/src/terminalplay.egg-info/
--rw-rw-r--   0 merwin    (1000) merwin    (1000)     1396 2023-04-30 07:22:03.000000 terminalplay-1.0.21/terminalplay/src/terminalplay.egg-info/PKG-INFO
--rw-rw-r--   0 merwin    (1000) merwin    (1000)      295 2023-04-30 07:22:03.000000 terminalplay-1.0.21/terminalplay/src/terminalplay.egg-info/SOURCES.txt
--rw-rw-r--   0 merwin    (1000) merwin    (1000)        1 2023-04-30 07:22:03.000000 terminalplay-1.0.21/terminalplay/src/terminalplay.egg-info/dependency_links.txt
--rw-rw-r--   0 merwin    (1000) merwin    (1000)       41 2023-04-30 07:22:03.000000 terminalplay-1.0.21/terminalplay/src/terminalplay.egg-info/requires.txt
--rw-rw-r--   0 merwin    (1000) merwin    (1000)        1 2023-04-30 07:22:03.000000 terminalplay-1.0.21/terminalplay/src/terminalplay.egg-info/top_level.txt
+drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:29:23.854689 terminalplay-1.0.22/
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     1065 2023-04-30 07:02:43.000000 terminalplay-1.0.22/LICENSE.txt
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     1396 2023-04-30 07:29:23.854689 terminalplay-1.0.22/PKG-INFO
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)      731 2023-04-30 07:02:59.000000 terminalplay-1.0.22/README.rst
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)       38 2023-04-30 07:29:23.854689 terminalplay-1.0.22/setup.cfg
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     1195 2023-04-30 07:29:05.000000 terminalplay-1.0.22/setup.py
+drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:29:23.838688 terminalplay-1.0.22/terminalplay/
+drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:29:23.838688 terminalplay-1.0.22/terminalplay/src/
+drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:29:23.854689 terminalplay-1.0.22/terminalplay/src/terminalplay.egg-info/
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     1396 2023-04-30 07:29:23.000000 terminalplay-1.0.22/terminalplay/src/terminalplay.egg-info/PKG-INFO
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)      295 2023-04-30 07:29:23.000000 terminalplay-1.0.22/terminalplay/src/terminalplay.egg-info/SOURCES.txt
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)        1 2023-04-30 07:29:23.000000 terminalplay-1.0.22/terminalplay/src/terminalplay.egg-info/dependency_links.txt
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)       41 2023-04-30 07:29:23.000000 terminalplay-1.0.22/terminalplay/src/terminalplay.egg-info/requires.txt
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)        1 2023-04-30 07:29:23.000000 terminalplay-1.0.22/terminalplay/src/terminalplay.egg-info/top_level.txt
```

### Comparing `terminalplay-1.0.21/LICENSE.txt` & `terminalplay-1.0.22/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `terminalplay-1.0.21/PKG-INFO` & `terminalplay-1.0.22/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminalplay
-Version: 1.0.21
+Version: 1.0.22
 Summary: Play videos on your terminal; Works on windows as well as linux;The video played will also have color and sound :)
 Home-page: https://github.com/merwin-asm/Terminal_Play
 Author: Merwin JD
 Author-email: merwin@fbi.ac
 License: MIT
 Project-URL: Bug Tracker, https://github.com/merwin-asm/Terminal_Play/issues
 Keywords: terminalplay,play videos,terminal
```

### Comparing `terminalplay-1.0.21/README.rst` & `terminalplay-1.0.22/README.rst`

 * *Files identical despite different names*

### Comparing `terminalplay-1.0.21/setup.py` & `terminalplay-1.0.22/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
-
+import setuptools
 
 with open("README.rst", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='terminalplay',
-    version='1.0.21',
+    version='1.0.22',
     license='MIT',
     author="Merwin JD",
     author_email='merwin@fbi.ac',
-    packages=find_packages('terminalplay/src'),
     package_dir={'': 'terminalplay/src'},
     url='https://github.com/merwin-asm/Terminal_Play',
     keywords='terminalplay, play videos, terminal',
+    packages = setuptools.find_packages(where="terminalplay/src"),
     install_requires=[
           'moviepy',
           'playsound',
           'rich',
           'sty',
           'opencv-python'
       ],
```

### Comparing `terminalplay-1.0.21/terminalplay/src/terminalplay.egg-info/PKG-INFO` & `terminalplay-1.0.22/terminalplay/src/terminalplay.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminalplay
-Version: 1.0.21
+Version: 1.0.22
 Summary: Play videos on your terminal; Works on windows as well as linux;The video played will also have color and sound :)
 Home-page: https://github.com/merwin-asm/Terminal_Play
 Author: Merwin JD
 Author-email: merwin@fbi.ac
 License: MIT
 Project-URL: Bug Tracker, https://github.com/merwin-asm/Terminal_Play/issues
 Keywords: terminalplay,play videos,terminal
```

