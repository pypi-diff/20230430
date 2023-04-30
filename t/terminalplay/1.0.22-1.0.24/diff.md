# Comparing `tmp/terminalplay-1.0.22.tar.gz` & `tmp/terminalplay-1.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminalplay-1.0.22.tar", last modified: Sun Apr 30 07:29:23 2023, max compression
+gzip compressed data, was "terminalplay-1.0.24.tar", last modified: Sun Apr 30 07:43:16 2023, max compression
```

## Comparing `terminalplay-1.0.22.tar` & `terminalplay-1.0.24.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:29:23.854689 terminalplay-1.0.22/
--rw-rw-r--   0 merwin    (1000) merwin    (1000)     1065 2023-04-30 07:02:43.000000 terminalplay-1.0.22/LICENSE.txt
--rw-rw-r--   0 merwin    (1000) merwin    (1000)     1396 2023-04-30 07:29:23.854689 terminalplay-1.0.22/PKG-INFO
--rw-rw-r--   0 merwin    (1000) merwin    (1000)      731 2023-04-30 07:02:59.000000 terminalplay-1.0.22/README.rst
--rw-rw-r--   0 merwin    (1000) merwin    (1000)       38 2023-04-30 07:29:23.854689 terminalplay-1.0.22/setup.cfg
--rw-rw-r--   0 merwin    (1000) merwin    (1000)     1195 2023-04-30 07:29:05.000000 terminalplay-1.0.22/setup.py
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:29:23.838688 terminalplay-1.0.22/terminalplay/
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:29:23.838688 terminalplay-1.0.22/terminalplay/src/
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:29:23.854689 terminalplay-1.0.22/terminalplay/src/terminalplay.egg-info/
--rw-rw-r--   0 merwin    (1000) merwin    (1000)     1396 2023-04-30 07:29:23.000000 terminalplay-1.0.22/terminalplay/src/terminalplay.egg-info/PKG-INFO
--rw-rw-r--   0 merwin    (1000) merwin    (1000)      295 2023-04-30 07:29:23.000000 terminalplay-1.0.22/terminalplay/src/terminalplay.egg-info/SOURCES.txt
--rw-rw-r--   0 merwin    (1000) merwin    (1000)        1 2023-04-30 07:29:23.000000 terminalplay-1.0.22/terminalplay/src/terminalplay.egg-info/dependency_links.txt
--rw-rw-r--   0 merwin    (1000) merwin    (1000)       41 2023-04-30 07:29:23.000000 terminalplay-1.0.22/terminalplay/src/terminalplay.egg-info/requires.txt
--rw-rw-r--   0 merwin    (1000) merwin    (1000)        1 2023-04-30 07:29:23.000000 terminalplay-1.0.22/terminalplay/src/terminalplay.egg-info/top_level.txt
+drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:43:16.778442 terminalplay-1.0.24/
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     1065 2023-04-30 07:41:31.000000 terminalplay-1.0.24/LICENSE
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     1554 2023-04-30 07:43:16.778442 terminalplay-1.0.24/PKG-INFO
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)      763 2023-04-30 07:42:48.000000 terminalplay-1.0.24/README.md
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)       38 2023-04-30 07:43:16.778442 terminalplay-1.0.24/setup.cfg
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     1355 2023-04-30 07:40:43.000000 terminalplay-1.0.24/setup.py
+drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:43:16.778442 terminalplay-1.0.24/src/
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     4949 2023-04-30 07:41:58.000000 terminalplay-1.0.24/src/__init__.py
+drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:43:16.778442 terminalplay-1.0.24/terminalplay.egg-info/
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     1554 2023-04-30 07:43:16.000000 terminalplay-1.0.24/terminalplay.egg-info/PKG-INFO
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)      221 2023-04-30 07:43:16.000000 terminalplay-1.0.24/terminalplay.egg-info/SOURCES.txt
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)        1 2023-04-30 07:43:16.000000 terminalplay-1.0.24/terminalplay.egg-info/dependency_links.txt
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)       41 2023-04-30 07:43:16.000000 terminalplay-1.0.24/terminalplay.egg-info/requires.txt
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)        4 2023-04-30 07:43:16.000000 terminalplay-1.0.24/terminalplay.egg-info/top_level.txt
```

### Comparing `terminalplay-1.0.22/LICENSE.txt` & `terminalplay-1.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `terminalplay-1.0.22/PKG-INFO` & `terminalplay-1.0.24/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: terminalplay
-Version: 1.0.22
+Version: 1.0.24
 Summary: Play videos on your terminal; Works on windows as well as linux;The video played will also have color and sound :)
 Home-page: https://github.com/merwin-asm/Terminal_Play
-Author: Merwin JD
+Author: Merwin
 Author-email: merwin@fbi.ac
 License: MIT
 Project-URL: Bug Tracker, https://github.com/merwin-asm/Terminal_Play/issues
 Keywords: terminalplay,play videos,terminal
 Platform: windows
 Platform: linux
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
+
 
 # Terminal Play v 1.0.0
 <p float="left">
  <img src="https://komarev.com/ghpvc/?username=merwin-terminal-play&label=Project%20Views-Github&color=0e75b6&style=flat" alt="darkmash-org" /> 
 <img alt="" src="https://static.pepy.tech/personalized-badge/terminalplay?period=total&units=international_system&left_color=blue&right_color=orange&left_text=Downloads">
 
 </p>
@@ -33,13 +37,15 @@
 ```sh
 pip install terminalplay
 ```
 
 
 ## Usage
 
-```sh
+```python
+from terminalplay import *
+
 # Load the video , this may take time on the first run (for a specific video)
 tp = TerminalPlay("test.mp4", div=0.4)  # Div is for reducing the size of the frame , default 0.5
 tp.play() # Plays the video
 ```
```

### Comparing `terminalplay-1.0.22/README.rst` & `terminalplay-1.0.24/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -15,12 +15,14 @@
 ```sh
 pip install terminalplay
 ```
 
 
 ## Usage
 
-```sh
+```python
+from terminalplay import *
+
 # Load the video , this may take time on the first run (for a specific video)
 tp = TerminalPlay("test.mp4", div=0.4)  # Div is for reducing the size of the frame , default 0.5
 tp.play() # Plays the video
 ```
```

### Comparing `terminalplay-1.0.22/setup.py` & `terminalplay-1.0.24/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 from setuptools import setup, find_packages
-import setuptools
+import codecs
+import os
 
-with open("README.rst", "r", encoding = "utf-8") as fh:
-    long_description = fh.read()
 
+here = os.path.abspath(os.path.dirname(__file__))
+
+with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
+    long_description = "\n" + fh.read()
+
+VERSION = '1.0.24'
+DESCRIPTION = "Play videos on your terminal; Works on windows as well as linux;The video played will also have color and sound :)"
+
+# Setting up
 setup(
-    name='terminalplay',
-    version='1.0.22',
+    name="terminalplay",
+    version=VERSION,
+    author="Merwin",
     license='MIT',
-    author="Merwin JD",
-    author_email='merwin@fbi.ac',
-    package_dir={'': 'terminalplay/src'},
+    author_email="merwin@fbi.ac",
+    description=DESCRIPTION,
+    long_description_content_type="text/markdown",
+    long_description=long_description,
+    packages=find_packages(),
+        project_urls = {
+        "Bug Tracker": "https://github.com/merwin-asm/Terminal_Play/issues",
+    },
     url='https://github.com/merwin-asm/Terminal_Play',
-    keywords='terminalplay, play videos, terminal',
-    packages = setuptools.find_packages(where="terminalplay/src"),
-    install_requires=[
-          'moviepy',
+
+    install_requires=['moviepy',
           'playsound',
           'rich',
           'sty',
-          'opencv-python'
-      ],
-      description="Play videos on your terminal; Works on windows as well as linux;The video played will also have color and sound :)",
-          long_description = long_description,
-    long_description_content_type = "text/markdown",
+          'opencv-python'],
+    keywords=['terminalplay', 'play videos', "terminal"],
       platforms= ["windows","linux"],
-    project_urls = {
-        "Bug Tracker": "https://github.com/merwin-asm/Terminal_Play/issues",
-    },
-    classifiers = [
+    classifiers=[
+        "Development Status :: 1 - Planning",
+        "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-
-      
-)
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+    ]
+)
```

### Comparing `terminalplay-1.0.22/terminalplay/src/terminalplay.egg-info/PKG-INFO` & `terminalplay-1.0.24/terminalplay.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: terminalplay
-Version: 1.0.22
+Version: 1.0.24
 Summary: Play videos on your terminal; Works on windows as well as linux;The video played will also have color and sound :)
 Home-page: https://github.com/merwin-asm/Terminal_Play
-Author: Merwin JD
+Author: Merwin
 Author-email: merwin@fbi.ac
 License: MIT
 Project-URL: Bug Tracker, https://github.com/merwin-asm/Terminal_Play/issues
 Keywords: terminalplay,play videos,terminal
 Platform: windows
 Platform: linux
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
+
 
 # Terminal Play v 1.0.0
 <p float="left">
  <img src="https://komarev.com/ghpvc/?username=merwin-terminal-play&label=Project%20Views-Github&color=0e75b6&style=flat" alt="darkmash-org" /> 
 <img alt="" src="https://static.pepy.tech/personalized-badge/terminalplay?period=total&units=international_system&left_color=blue&right_color=orange&left_text=Downloads">
 
 </p>
@@ -33,13 +37,15 @@
 ```sh
 pip install terminalplay
 ```
 
 
 ## Usage
 
-```sh
+```python
+from terminalplay import *
+
 # Load the video , this may take time on the first run (for a specific video)
 tp = TerminalPlay("test.mp4", div=0.4)  # Div is for reducing the size of the frame , default 0.5
 tp.play() # Plays the video
 ```
```

