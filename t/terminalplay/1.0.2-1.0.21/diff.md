# Comparing `tmp/terminalplay-1.0.2.tar.gz` & `tmp/terminalplay-1.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminalplay-1.0.2.tar", last modified: Sun Apr 30 07:17:20 2023, max compression
+gzip compressed data, was "terminalplay-1.0.21.tar", last modified: Sun Apr 30 07:22:03 2023, max compression
```

## Comparing `terminalplay-1.0.2.tar` & `terminalplay-1.0.21.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:17:20.889234 terminalplay-1.0.2/
--rw-rw-r--   0 merwin    (1000) merwin    (1000)     1065 2023-04-30 07:02:43.000000 terminalplay-1.0.2/LICENSE.txt
--rw-rw-r--   0 merwin    (1000) merwin    (1000)      558 2023-04-30 07:17:20.889234 terminalplay-1.0.2/PKG-INFO
--rw-rw-r--   0 merwin    (1000) merwin    (1000)      731 2023-04-30 07:02:59.000000 terminalplay-1.0.2/README.rst
--rw-rw-r--   0 merwin    (1000) merwin    (1000)       38 2023-04-30 07:17:20.889234 terminalplay-1.0.2/setup.cfg
--rw-rw-r--   0 merwin    (1000) merwin    (1000)      879 2023-04-30 07:17:16.000000 terminalplay-1.0.2/setup.py
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:17:20.889234 terminalplay-1.0.2/terminalplay/
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:17:20.889234 terminalplay-1.0.2/terminalplay/src/
-drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:17:20.889234 terminalplay-1.0.2/terminalplay/src/terminalplay.egg-info/
--rw-rw-r--   0 merwin    (1000) merwin    (1000)      558 2023-04-30 07:17:20.000000 terminalplay-1.0.2/terminalplay/src/terminalplay.egg-info/PKG-INFO
--rw-rw-r--   0 merwin    (1000) merwin    (1000)      295 2023-04-30 07:17:20.000000 terminalplay-1.0.2/terminalplay/src/terminalplay.egg-info/SOURCES.txt
--rw-rw-r--   0 merwin    (1000) merwin    (1000)        1 2023-04-30 07:17:20.000000 terminalplay-1.0.2/terminalplay/src/terminalplay.egg-info/dependency_links.txt
--rw-rw-r--   0 merwin    (1000) merwin    (1000)       41 2023-04-30 07:17:20.000000 terminalplay-1.0.2/terminalplay/src/terminalplay.egg-info/requires.txt
--rw-rw-r--   0 merwin    (1000) merwin    (1000)        1 2023-04-30 07:17:20.000000 terminalplay-1.0.2/terminalplay/src/terminalplay.egg-info/top_level.txt
+drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:22:03.163345 terminalplay-1.0.21/
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     1065 2023-04-30 07:02:43.000000 terminalplay-1.0.21/LICENSE.txt
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     1396 2023-04-30 07:22:03.163345 terminalplay-1.0.21/PKG-INFO
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)      731 2023-04-30 07:02:59.000000 terminalplay-1.0.21/README.rst
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)       38 2023-04-30 07:22:03.163345 terminalplay-1.0.21/setup.cfg
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     1159 2023-04-30 07:21:59.000000 terminalplay-1.0.21/setup.py
+drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:22:03.163345 terminalplay-1.0.21/terminalplay/
+drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:22:03.163345 terminalplay-1.0.21/terminalplay/src/
+drwxrwxr-x   0 merwin    (1000) merwin    (1000)        0 2023-04-30 07:22:03.163345 terminalplay-1.0.21/terminalplay/src/terminalplay.egg-info/
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)     1396 2023-04-30 07:22:03.000000 terminalplay-1.0.21/terminalplay/src/terminalplay.egg-info/PKG-INFO
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)      295 2023-04-30 07:22:03.000000 terminalplay-1.0.21/terminalplay/src/terminalplay.egg-info/SOURCES.txt
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)        1 2023-04-30 07:22:03.000000 terminalplay-1.0.21/terminalplay/src/terminalplay.egg-info/dependency_links.txt
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)       41 2023-04-30 07:22:03.000000 terminalplay-1.0.21/terminalplay/src/terminalplay.egg-info/requires.txt
+-rw-rw-r--   0 merwin    (1000) merwin    (1000)        1 2023-04-30 07:22:03.000000 terminalplay-1.0.21/terminalplay/src/terminalplay.egg-info/top_level.txt
```

### Comparing `terminalplay-1.0.2/LICENSE.txt` & `terminalplay-1.0.21/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `terminalplay-1.0.2/README.rst` & `terminalplay-1.0.21/README.rst`

 * *Files identical despite different names*

