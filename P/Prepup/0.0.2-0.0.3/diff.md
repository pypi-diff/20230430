# Comparing `tmp/prepup-0.0.2.tar.gz` & `tmp/prepup-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prepup-0.0.2.tar", last modified: Sat Apr 29 23:02:06 2023, max compression
+gzip compressed data, was "Prepup-0.0.3.tar", last modified: Sun Apr 30 15:32:38 2023, max compression
```

## Comparing `prepup-0.0.2.tar` & `prepup-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 23:02:06.737571 prepup-0.0.2/
--rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 prepup-0.0.2/AUTHORS.rst
--rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 prepup-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 prepup-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1367 2023-04-29 23:02:06.738571 prepup-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-04-29 20:41:27.000000 prepup-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 23:02:06.714106 prepup-0.0.2/prepup/
--rw-rw-rw-   0        0        0      148 2023-04-29 20:41:27.000000 prepup-0.0.2/prepup/__init__.py
--rw-rw-rw-   0        0        0    27774 2023-04-29 22:23:28.000000 prepup-0.0.2/prepup/common.py
--rw-rw-rw-   0        0        0     5349 2023-04-29 22:20:45.000000 prepup-0.0.2/prepup/prepup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 23:02:06.734585 prepup-0.0.2/prepup.egg-info/
--rw-rw-rw-   0        0        0     1367 2023-04-29 23:02:06.000000 prepup-0.0.2/prepup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-04-29 23:02:06.000000 prepup-0.0.2/prepup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      348 2023-04-29 23:02:06.000000 prepup-0.0.2/prepup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-29 22:42:26.000000 prepup-0.0.2/prepup.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      348 2023-04-29 23:02:06.000000 prepup-0.0.2/prepup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-29 23:02:06.000000 prepup-0.0.2/prepup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      367 2023-04-29 23:00:31.000000 prepup-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0      414 2023-04-29 23:02:06.740574 prepup-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1864 2023-04-29 23:02:01.000000 prepup-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 23:02:06.736573 prepup-0.0.2/tests/
--rw-rw-rw-   0        0        0      403 2023-04-29 20:41:27.000000 prepup-0.0.2/tests/test_prepup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 15:32:38.523105 Prepup-0.0.3/
+-rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 Prepup-0.0.3/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 Prepup-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 Prepup-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      551 2023-04-30 15:32:38.523105 Prepup-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-30 15:32:38.505690 Prepup-0.0.3/Prepup.egg-info/
+-rw-rw-rw-   0        0        0      551 2023-04-30 15:32:38.000000 Prepup-0.0.3/Prepup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-04-30 15:32:38.000000 Prepup-0.0.3/Prepup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 15:32:38.000000 Prepup-0.0.3/Prepup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-30 15:32:38.000000 Prepup-0.0.3/Prepup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      219 2023-04-30 15:32:38.000000 Prepup-0.0.3/Prepup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-30 15:32:38.000000 Prepup-0.0.3/Prepup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      489 2023-04-29 20:41:27.000000 Prepup-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 15:32:38.513690 Prepup-0.0.3/prepup/
+-rw-rw-rw-   0        0        0      148 2023-04-29 20:41:27.000000 Prepup-0.0.3/prepup/__init__.py
+-rw-rw-rw-   0        0        0    27774 2023-04-29 22:23:28.000000 Prepup-0.0.3/prepup/common.py
+-rw-rw-rw-   0        0        0     5349 2023-04-29 22:20:45.000000 Prepup-0.0.3/prepup/prepup.py
+-rw-rw-rw-   0        0        0      367 2023-04-29 23:00:31.000000 Prepup-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0      414 2023-04-30 15:32:38.523105 Prepup-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     3239 2023-04-30 15:29:09.000000 Prepup-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 15:32:38.521690 Prepup-0.0.3/tests/
+-rw-rw-rw-   0        0        0       37 2023-04-29 20:41:27.000000 Prepup-0.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      403 2023-04-29 20:41:27.000000 Prepup-0.0.3/tests/test_prepup.py
```

### Comparing `prepup-0.0.2/LICENSE` & `Prepup-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prepup-0.0.2/prepup/common.py` & `Prepup-0.0.3/prepup/common.py`

 * *Files identical despite different names*

### Comparing `prepup-0.0.2/prepup/prepup.py` & `Prepup-0.0.3/prepup/prepup.py`

 * *Files identical despite different names*

