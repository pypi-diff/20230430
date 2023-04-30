# Comparing `tmp/geotoolkit-0.2.0.tar.gz` & `tmp/geotoolkit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geotoolkit-0.2.0.tar", last modified: Sun Apr 30 17:45:29 2023, max compression
+gzip compressed data, was "geotoolkit-0.2.1.tar", last modified: Sun Apr 30 17:48:41 2023, max compression
```

## Comparing `geotoolkit-0.2.0.tar` & `geotoolkit-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 17:45:29.195374 geotoolkit-0.2.0/
--rw-rw-rw-   0        0        0     1500 2023-04-30 17:45:29.195374 geotoolkit-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1281 2023-04-30 17:39:20.000000 geotoolkit-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 17:45:29.185376 geotoolkit-0.2.0/geotoolkit/
--rw-rw-rw-   0        0        0     2495 2023-04-30 17:39:57.000000 geotoolkit-0.2.0/geotoolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 17:45:29.195374 geotoolkit-0.2.0/geotoolkit.egg-info/
--rw-rw-rw-   0        0        0     1500 2023-04-30 17:45:29.000000 geotoolkit-0.2.0/geotoolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-04-30 17:45:29.000000 geotoolkit-0.2.0/geotoolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 17:45:29.000000 geotoolkit-0.2.0/geotoolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-30 17:45:29.000000 geotoolkit-0.2.0/geotoolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1073 2023-04-30 17:10:33.000000 geotoolkit-0.2.0/license.md
--rw-rw-rw-   0        0        0       42 2023-04-30 17:45:29.195374 geotoolkit-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      397 2023-04-30 17:44:50.000000 geotoolkit-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 17:48:41.368308 geotoolkit-0.2.1/
+-rw-rw-rw-   0        0        0     1541 2023-04-30 17:48:41.368308 geotoolkit-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1281 2023-04-30 17:39:20.000000 geotoolkit-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 17:48:41.353188 geotoolkit-0.2.1/geotoolkit/
+-rw-rw-rw-   0        0        0     2495 2023-04-30 17:39:57.000000 geotoolkit-0.2.1/geotoolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 17:48:41.368308 geotoolkit-0.2.1/geotoolkit.egg-info/
+-rw-rw-rw-   0        0        0     1541 2023-04-30 17:48:41.000000 geotoolkit-0.2.1/geotoolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-04-30 17:48:41.000000 geotoolkit-0.2.1/geotoolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 17:48:41.000000 geotoolkit-0.2.1/geotoolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-30 17:48:41.000000 geotoolkit-0.2.1/geotoolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1073 2023-04-30 17:10:33.000000 geotoolkit-0.2.1/license.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 17:48:41.368308 geotoolkit-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      449 2023-04-30 17:48:10.000000 geotoolkit-0.2.1/setup.py
```

### Comparing `geotoolkit-0.2.0/PKG-INFO` & `geotoolkit-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: geotoolkit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Peforming calculations with geographic points
 Home-page: https://github.com/TimHanewich/geotoolkit
 Author: Tim Hanewich
+Description-Content-Type: text/markdown
 License-File: license.md
 
 # geotoolkit
 A lightweight python library for working with geographic coordinates. This library can be used in things such as drone navigation, speed measurement, and more.
 
 ## Examples
 Measuring distance between two points:
```

### Comparing `geotoolkit-0.2.0/README.md` & `geotoolkit-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `geotoolkit-0.2.0/geotoolkit/__init__.py` & `geotoolkit-0.2.1/geotoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `geotoolkit-0.2.0/geotoolkit.egg-info/PKG-INFO` & `geotoolkit-0.2.1/geotoolkit.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: geotoolkit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Peforming calculations with geographic points
 Home-page: https://github.com/TimHanewich/geotoolkit
 Author: Tim Hanewich
+Description-Content-Type: text/markdown
 License-File: license.md
 
 # geotoolkit
 A lightweight python library for working with geographic coordinates. This library can be used in things such as drone navigation, speed measurement, and more.
 
 ## Examples
 Measuring distance between two points:
```

### Comparing `geotoolkit-0.2.0/license.md` & `geotoolkit-0.2.1/license.md`

 * *Files identical despite different names*

