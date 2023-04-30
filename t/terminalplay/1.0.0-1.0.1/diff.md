# Comparing `tmp/terminalplay-1.0.0.tar.gz` & `tmp/terminalplay-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminalplay-1.0.0.tar", last modified: Sun Apr 30 07:10:44 2023, max compression
+gzip compressed data, was "terminalplay-1.0.1.tar", last modified: Sun Apr 30 07:14:33 2023, max compression
```

## Comparing `terminalplay-1.0.0.tar` & `terminalplay-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:10:43.990349 terminalplay-1.0.0/
--rw-rw-r--   0 merwin    (1000) merwin    (1000)     1065 2023-04-30 07:02:43.000000 terminalplay-1.0.0/LICENSE
--rw-rw-r--   0 merwin    (1000) merwin    (1000)      554 2023-04-30 07:10:43.990349 terminalplay-1.0.0/PKG-INFO
--rw-rw-r--   0 merwin    (1000) merwin    (1000)      731 2023-04-30 07:02:59.000000 terminalplay-1.0.0/README.md
--rw-rw-r--   0 merwin    (1000) merwin    (1000)       38 2023-04-30 07:10:43.990349 terminalplay-1.0.0/setup.cfg
--rw-rw-r--   0 merwin    (1000) merwin    (1000)      871 2023-04-30 07:10:12.000000 terminalplay-1.0.0/setup.py
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:10:43.986349 terminalplay-1.0.0/terminalplay/
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:10:43.986349 terminalplay-1.0.0/terminalplay/src/
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:10:43.990349 terminalplay-1.0.0/terminalplay/src/terminalplay.egg-info/
--rw-rw-r--   0 merwin    (1000) merwin    (1000)      554 2023-04-30 07:10:42.000000 terminalplay-1.0.0/terminalplay/src/terminalplay.egg-info/PKG-INFO
--rw-rw-r--   0 merwin    (1000) merwin    (1000)      290 2023-04-30 07:10:42.000000 terminalplay-1.0.0/terminalplay/src/terminalplay.egg-info/SOURCES.txt
--rw-rw-r--   0 merwin    (1000) merwin    (1000)        1 2023-04-30 07:10:42.000000 terminalplay-1.0.0/terminalplay/src/terminalplay.egg-info/dependency_links.txt
--rw-rw-r--   0 merwin    (1000) merwin    (1000)       41 2023-04-30 07:10:42.000000 terminalplay-1.0.0/terminalplay/src/terminalplay.egg-info/requires.txt
--rw-rw-r--   0 merwin    (1000) merwin    (1000)        1 2023-04-30 07:10:42.000000 terminalplay-1.0.0/terminalplay/src/terminalplay.egg-info/top_level.txt
+drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:14:33.168000 terminalplay-1.0.1/
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     1065 2023-04-30 07:02:43.000000 terminalplay-1.0.1/LICENSE
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)      554 2023-04-30 07:14:33.168000 terminalplay-1.0.1/PKG-INFO
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)      731 2023-04-30 07:02:59.000000 terminalplay-1.0.1/README.md
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)      103 2023-04-30 07:14:33.172000 terminalplay-1.0.1/setup.cfg
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)      879 2023-04-30 07:14:11.000000 terminalplay-1.0.1/setup.py
+drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:14:33.164000 terminalplay-1.0.1/terminalplay/
+drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:14:33.164000 terminalplay-1.0.1/terminalplay/src/
+drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:14:33.168000 terminalplay-1.0.1/terminalplay/src/terminalplay.egg-info/
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)      554 2023-04-30 07:14:33.000000 terminalplay-1.0.1/terminalplay/src/terminalplay.egg-info/PKG-INFO
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)      300 2023-04-30 07:14:33.000000 terminalplay-1.0.1/terminalplay/src/terminalplay.egg-info/SOURCES.txt
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)        1 2023-04-30 07:14:33.000000 terminalplay-1.0.1/terminalplay/src/terminalplay.egg-info/dependency_links.txt
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)       41 2023-04-30 07:14:33.000000 terminalplay-1.0.1/terminalplay/src/terminalplay.egg-info/requires.txt
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)        1 2023-04-30 07:14:33.000000 terminalplay-1.0.1/terminalplay/src/terminalplay.egg-info/top_level.txt
```

### Comparing `terminalplay-1.0.0/LICENSE` & `terminalplay-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `terminalplay-1.0.0/PKG-INFO` & `terminalplay-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminalplay
-Version: 1.0.0
+Version: 1.0.1
 Summary: Play videos on your terminal; Works on windows as well as linux
 Home-page: https://github.com/merwin-asm/Terminal_Play
 Author: Merwin JD
 Author-email: merwin@fbi.ac
 License: MIT
 Keywords: terminalplay,play videos,terminal
 Platform: windows
```

### Comparing `terminalplay-1.0.0/README.md` & `terminalplay-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `terminalplay-1.0.0/setup.py` & `terminalplay-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='terminalplay',
-    version='1.0.0',
+    version='1.0.1',
     license='MIT',
     author="Merwin JD",
     author_email='merwin@fbi.ac',
     packages=find_packages('terminalplay/src'),
     package_dir={'': 'terminalplay/src'},
     url='https://github.com/merwin-asm/Terminal_Play',
     keywords='terminalplay, play videos, terminal',
@@ -19,9 +19,10 @@
       ],
       description="Play videos on your terminal; Works on windows as well as linux",
       long_description="""
       The video played will also have color and sound :)
       Videos be converted into easily readable frames which will be printed on the terminal (This 
       conversion will only take place once).
       """,
-      platforms= ["windows","linux"]
+      platforms= ["windows","linux"],
+      
 )
```

### Comparing `terminalplay-1.0.0/terminalplay/src/terminalplay.egg-info/PKG-INFO` & `terminalplay-1.0.1/terminalplay/src/terminalplay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminalplay
-Version: 1.0.0
+Version: 1.0.1
 Summary: Play videos on your terminal; Works on windows as well as linux
 Home-page: https://github.com/merwin-asm/Terminal_Play
 Author: Merwin JD
 Author-email: merwin@fbi.ac
 License: MIT
 Keywords: terminalplay,play videos,terminal
 Platform: windows
```

