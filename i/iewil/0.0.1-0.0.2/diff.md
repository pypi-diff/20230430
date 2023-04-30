# Comparing `tmp/iewil-0.0.1.tar.gz` & `tmp/iewil-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iewil-0.0.1.tar", last modified: Sun Apr 30 04:25:37 2023, max compression
+gzip compressed data, was "iewil-0.0.2.tar", last modified: Sun Apr 30 04:39:15 2023, max compression
```

## Comparing `iewil-0.0.1.tar` & `iewil-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 04:25:37.072002 iewil-0.0.1/
--rw-rw-rw-   0        0        0      452 2023-04-30 04:25:37.072002 iewil-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-30 04:25:37.052456 iewil-0.0.1/iewil/
--rw-rw-rw-   0        0        0       19 2023-04-30 03:23:06.000000 iewil-0.0.1/iewil/__init__.py
--rw-rw-rw-   0        0        0     3095 2023-04-30 03:22:32.000000 iewil-0.0.1/iewil/modul.py
-drwxrwxrwx   0        0        0        0 2023-04-30 04:25:37.071028 iewil-0.0.1/iewil.egg-info/
--rw-rw-rw-   0        0        0      452 2023-04-30 04:25:36.000000 iewil-0.0.1/iewil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-04-30 04:25:36.000000 iewil-0.0.1/iewil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 04:25:36.000000 iewil-0.0.1/iewil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-30 04:25:36.000000 iewil-0.0.1/iewil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 04:25:37.072951 iewil-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      666 2023-04-30 04:24:29.000000 iewil-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 04:39:15.909713 iewil-0.0.2/
+-rw-rw-rw-   0        0        0      452 2023-04-30 04:39:15.907765 iewil-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-30 04:39:15.889217 iewil-0.0.2/iewil/
+-rw-rw-rw-   0        0        0     3095 2023-04-30 04:38:01.000000 iewil-0.0.2/iewil/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 04:39:15.905836 iewil-0.0.2/iewil.egg-info/
+-rw-rw-rw-   0        0        0      452 2023-04-30 04:39:15.000000 iewil-0.0.2/iewil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2023-04-30 04:39:15.000000 iewil-0.0.2/iewil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 04:39:15.000000 iewil-0.0.2/iewil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-30 04:39:15.000000 iewil-0.0.2/iewil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 04:39:15.909713 iewil-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      666 2023-04-30 04:39:08.000000 iewil-0.0.2/setup.py
```

### Comparing `iewil-0.0.1/iewil/modul.py` & `iewil-0.0.2/iewil/__init__.py`

 * *Files identical despite different names*

### Comparing `iewil-0.0.1/setup.py` & `iewil-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Streaming video data via networks'
 
 # Setting up
 setup(
     name="iewil",
     version=VERSION,
     author="iewilmaestro",
```

