# Comparing `tmp/hagis-0.4.5.tar.gz` & `tmp/hagis-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.4.5.tar", last modified: Thu Apr 27 13:12:19 2023, max compression
+gzip compressed data, was "hagis-0.4.6.tar", last modified: Sun Apr 30 17:54:31 2023, max compression
```

## Comparing `hagis-0.4.5.tar` & `hagis-0.4.6.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 13:12:19.898921 hagis-0.4.5/
--rw-rw-rw-   0        0        0      923 2023-04-27 13:12:19.897931 hagis-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-04-22 02:10:21.000000 hagis-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 13:12:19.884701 hagis-0.4.5/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.4.5/hagis/__init__.py
--rw-rw-rw-   0        0        0    15263 2023-04-27 13:10:10.000000 hagis-0.4.5/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-27 13:12:19.895884 hagis-0.4.5/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-04-27 13:12:19.000000 hagis-0.4.5/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-04-27 13:12:19.000000 hagis-0.4.5/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 13:12:19.000000 hagis-0.4.5/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-27 13:12:19.000000 hagis-0.4.5/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-27 13:10:27.000000 hagis-0.4.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 13:12:19.898921 hagis-0.4.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 17:54:31.293007 hagis-0.4.6/
+-rw-rw-rw-   0        0        0      923 2023-04-30 17:54:31.293007 hagis-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-04-22 02:10:21.000000 hagis-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 17:54:31.277005 hagis-0.4.6/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-04-30 17:54:31.000000 hagis-0.4.6/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-04-30 17:54:31.000000 hagis-0.4.6/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 17:54:31.000000 hagis-0.4.6/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-30 17:54:31.000000 hagis-0.4.6/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    15263 2023-04-30 17:52:36.000000 hagis-0.4.6/hagis.py
+-rw-rw-rw-   0        0        0      589 2023-04-30 17:53:24.000000 hagis-0.4.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 17:54:31.293007 hagis-0.4.6/setup.cfg
```

### Comparing `hagis-0.4.5/PKG-INFO` & `hagis-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.4.5
+Version: 0.4.6
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.4.5/hagis/hagis.py` & `hagis-0.4.6/hagis.py`

 * *Files identical despite different names*

### Comparing `hagis-0.4.5/hagis.egg-info/PKG-INFO` & `hagis-0.4.6/hagis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.4.5
+Version: 0.4.6
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.4.5/pyproject.toml` & `hagis-0.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.4.5"
+version = "0.4.6"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

