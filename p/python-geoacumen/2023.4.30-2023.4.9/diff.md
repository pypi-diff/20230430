# Comparing `tmp/python-geoacumen-2023.4.30.tar.gz` & `tmp/python-geoacumen-2023.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-geoacumen-2023.4.30.tar", last modified: Sun Apr 30 04:07:48 2023, max compression
+gzip compressed data, was "python-geoacumen-2023.4.9.tar", last modified: Sun Apr  9 04:07:51 2023, max compression
```

## Comparing `python-geoacumen-2023.4.30.tar` & `python-geoacumen-2023.4.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:07:48.750728 python-geoacumen-2023.4.30/
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-04-30 04:07:34.000000 python-geoacumen-2023.4.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 04:07:34.000000 python-geoacumen-2023.4.30/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-30 04:07:48.750728 python-geoacumen-2023.4.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-30 04:07:34.000000 python-geoacumen-2023.4.30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:07:48.738727 python-geoacumen-2023.4.30/geoacumen/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-30 04:07:44.000000 python-geoacumen-2023.4.30/geoacumen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:07:48.738727 python-geoacumen-2023.4.30/geoacumen/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 04:07:34.000000 python-geoacumen-2023.4.30/geoacumen/db/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123) 10111807 2023-04-30 04:07:48.000000 python-geoacumen-2023.4.30/geoacumen/db/Geoacumen-Country.mmdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:07:48.750728 python-geoacumen-2023.4.30/python_geoacumen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-30 04:07:48.000000 python-geoacumen-2023.4.30/python_geoacumen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-30 04:07:48.000000 python-geoacumen-2023.4.30/python_geoacumen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 04:07:48.000000 python-geoacumen-2023.4.30/python_geoacumen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 04:07:48.000000 python-geoacumen-2023.4.30/python_geoacumen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-30 04:07:48.000000 python-geoacumen-2023.4.30/python_geoacumen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 04:07:48.750728 python-geoacumen-2023.4.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-30 04:07:34.000000 python-geoacumen-2023.4.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:07:51.875707 python-geoacumen-2023.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-04-09 04:07:37.000000 python-geoacumen-2023.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-09 04:07:37.000000 python-geoacumen-2023.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-09 04:07:51.875707 python-geoacumen-2023.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-09 04:07:37.000000 python-geoacumen-2023.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:07:51.863706 python-geoacumen-2023.4.9/geoacumen/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-09 04:07:48.000000 python-geoacumen-2023.4.9/geoacumen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:07:51.863706 python-geoacumen-2023.4.9/geoacumen/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 04:07:37.000000 python-geoacumen-2023.4.9/geoacumen/db/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123) 10060855 2023-04-09 04:07:51.000000 python-geoacumen-2023.4.9/geoacumen/db/Geoacumen-Country.mmdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:07:51.875707 python-geoacumen-2023.4.9/python_geoacumen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-09 04:07:51.000000 python-geoacumen-2023.4.9/python_geoacumen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-09 04:07:51.000000 python-geoacumen-2023.4.9/python_geoacumen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 04:07:51.000000 python-geoacumen-2023.4.9/python_geoacumen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-09 04:07:51.000000 python-geoacumen-2023.4.9/python_geoacumen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 04:07:51.000000 python-geoacumen-2023.4.9/python_geoacumen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 04:07:51.875707 python-geoacumen-2023.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-09 04:07:37.000000 python-geoacumen-2023.4.9/setup.py
```

### Comparing `python-geoacumen-2023.4.30/LICENSE` & `python-geoacumen-2023.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-geoacumen-2023.4.30/PKG-INFO` & `python-geoacumen-2023.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-geoacumen
-Version: 2023.4.30
+Version: 2023.4.9
 Summary: Library to access/distribute Geoacumen IP databases
 Home-page: UNKNOWN
 Author: Kevin Chung
 Author-email: kchung@nyu.edu
 License: Apache 2.0
 Description: # python-geoacumen
```

### Comparing `python-geoacumen-2023.4.30/python_geoacumen.egg-info/PKG-INFO` & `python-geoacumen-2023.4.9/python_geoacumen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-geoacumen
-Version: 2023.4.30
+Version: 2023.4.9
 Summary: Library to access/distribute Geoacumen IP databases
 Home-page: UNKNOWN
 Author: Kevin Chung
 Author-email: kchung@nyu.edu
 License: Apache 2.0
 Description: # python-geoacumen
```

### Comparing `python-geoacumen-2023.4.30/setup.py` & `python-geoacumen-2023.4.9/setup.py`

 * *Files identical despite different names*

