# Comparing `tmp/terminalplay-1.0.25.tar.gz` & `tmp/terminalplay-1.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminalplay-1.0.25.tar", last modified: Sun Apr 30 07:47:50 2023, max compression
+gzip compressed data, was "terminalplay-1.0.26.tar", last modified: Sun Apr 30 07:55:20 2023, max compression
```

## Comparing `terminalplay-1.0.25.tar` & `terminalplay-1.0.26.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:47:50.636005 terminalplay-1.0.25/
--rw-rw-r--   0 merwin    (1000) merwin    (1000)     1065 2023-04-30 07:41:31.000000 terminalplay-1.0.25/LICENSE
--rw-rw-r--   0 merwin    (1000) merwin    (1000)     1557 2023-04-30 07:47:50.636005 terminalplay-1.0.25/PKG-INFO
--rw-rw-r--   0 merwin    (1000) merwin    (1000)      763 2023-04-30 07:42:48.000000 terminalplay-1.0.25/README.md
--rw-rw-r--   0 merwin    (1000) merwin    (1000)       38 2023-04-30 07:47:50.636005 terminalplay-1.0.25/setup.cfg
--rw-rw-r--   0 merwin    (1000) merwin    (1000)     1358 2023-04-30 07:47:17.000000 terminalplay-1.0.25/setup.py
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:47:50.636005 terminalplay-1.0.25/src/
--rw-rw-r--   0 merwin    (1000) merwin    (1000)     4949 2023-04-30 07:41:58.000000 terminalplay-1.0.25/src/__init__.py
--rw-rw-r--   0 merwin    (1000) merwin    (1000)     4949 2023-04-30 07:47:48.000000 terminalplay-1.0.25/src/terminalplay.py
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:47:50.636005 terminalplay-1.0.25/terminalplay.egg-info/
--rw-rw-r--   0 merwin    (1000) merwin    (1000)     1557 2023-04-30 07:47:50.000000 terminalplay-1.0.25/terminalplay.egg-info/PKG-INFO
--rw-rw-r--   0 merwin    (1000) merwin    (1000)      241 2023-04-30 07:47:50.000000 terminalplay-1.0.25/terminalplay.egg-info/SOURCES.txt
--rw-rw-r--   0 merwin    (1000) merwin    (1000)        1 2023-04-30 07:47:50.000000 terminalplay-1.0.25/terminalplay.egg-info/dependency_links.txt
--rw-rw-r--   0 merwin    (1000) merwin    (1000)       41 2023-04-30 07:47:50.000000 terminalplay-1.0.25/terminalplay.egg-info/requires.txt
--rw-rw-r--   0 merwin    (1000) merwin    (1000)        4 2023-04-30 07:47:50.000000 terminalplay-1.0.25/terminalplay.egg-info/top_level.txt
+drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:55:20.338799 terminalplay-1.0.26/
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     1065 2023-04-30 07:41:31.000000 terminalplay-1.0.26/LICENSE
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     1557 2023-04-30 07:55:20.338799 terminalplay-1.0.26/PKG-INFO
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)      763 2023-04-30 07:42:48.000000 terminalplay-1.0.26/README.md
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)       38 2023-04-30 07:55:20.338799 terminalplay-1.0.26/setup.cfg
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     1358 2023-04-30 07:55:18.000000 terminalplay-1.0.26/setup.py
+drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:55:20.338799 terminalplay-1.0.26/terminalplay/
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     4949 2023-04-30 07:41:58.000000 terminalplay-1.0.26/terminalplay/__init__.py
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     4949 2023-04-30 07:47:48.000000 terminalplay-1.0.26/terminalplay/terminalplay.py
+drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:55:20.338799 terminalplay-1.0.26/terminalplay.egg-info/
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     1557 2023-04-30 07:55:19.000000 terminalplay-1.0.26/terminalplay.egg-info/PKG-INFO
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)      259 2023-04-30 07:55:19.000000 terminalplay-1.0.26/terminalplay.egg-info/SOURCES.txt
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)        1 2023-04-30 07:55:19.000000 terminalplay-1.0.26/terminalplay.egg-info/dependency_links.txt
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)       41 2023-04-30 07:55:19.000000 terminalplay-1.0.26/terminalplay.egg-info/requires.txt
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)       13 2023-04-30 07:55:19.000000 terminalplay-1.0.26/terminalplay.egg-info/top_level.txt
```

### Comparing `terminalplay-1.0.25/LICENSE` & `terminalplay-1.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `terminalplay-1.0.25/PKG-INFO` & `terminalplay-1.0.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminalplay
-Version: 1.0.25
+Version: 1.0.26
 Summary: Play videos on your terminal; Works on windows as well as linux;The video played will also have color and sound :)
 Home-page: https://github.com/merwin-asm/Terminal_Play
 Author: Merwin JD
 Author-email: merwin@fbi.ac
 License: MIT
 Project-URL: Bug Tracker, https://github.com/merwin-asm/Terminal_Play/issues
 Keywords: terminalplay,play videos,terminal
```

### Comparing `terminalplay-1.0.25/README.md` & `terminalplay-1.0.26/README.md`

 * *Files identical despite different names*

### Comparing `terminalplay-1.0.25/setup.py` & `terminalplay-1.0.26/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.25'
+VERSION = '1.0.26'
 DESCRIPTION = "Play videos on your terminal; Works on windows as well as linux;The video played will also have color and sound :)"
 
 # Setting up
 setup(
     name="terminalplay",
     version=VERSION,
     author="Merwin JD",
```

### Comparing `terminalplay-1.0.25/src/__init__.py` & `terminalplay-1.0.26/terminalplay/__init__.py`

 * *Files identical despite different names*

### Comparing `terminalplay-1.0.25/src/terminalplay.py` & `terminalplay-1.0.26/terminalplay/terminalplay.py`

 * *Files identical despite different names*

### Comparing `terminalplay-1.0.25/terminalplay.egg-info/PKG-INFO` & `terminalplay-1.0.26/terminalplay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminalplay
-Version: 1.0.25
+Version: 1.0.26
 Summary: Play videos on your terminal; Works on windows as well as linux;The video played will also have color and sound :)
 Home-page: https://github.com/merwin-asm/Terminal_Play
 Author: Merwin JD
 Author-email: merwin@fbi.ac
 License: MIT
 Project-URL: Bug Tracker, https://github.com/merwin-asm/Terminal_Play/issues
 Keywords: terminalplay,play videos,terminal
```

