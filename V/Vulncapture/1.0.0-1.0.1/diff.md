# Comparing `tmp/Vulncapture-1.0.0.tar.gz` & `tmp/Vulncapture-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Vulncapture-1.0.0.tar", last modified: Sat Apr 29 17:44:44 2023, max compression
+gzip compressed data, was "Vulncapture-1.0.1.tar", last modified: Sun Apr 30 04:05:41 2023, max compression
```

## Comparing `Vulncapture-1.0.0.tar` & `Vulncapture-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 17:44:44.206363 Vulncapture-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-04-26 08:28:29.000000 Vulncapture-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1238 2023-04-29 17:44:44.205361 Vulncapture-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      692 2023-04-29 17:43:46.000000 Vulncapture-1.0.0/README.md
--rw-rw-rw-   0        0        0      630 2023-04-29 17:44:27.000000 Vulncapture-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 17:44:44.206363 Vulncapture-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      189 2023-04-29 17:26:11.000000 Vulncapture-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:44:44.156981 Vulncapture-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-29 17:44:44.187357 Vulncapture-1.0.0/src/Vulncapture/
--rw-rw-rw-   0        0        0    18802 2023-04-29 17:41:21.000000 Vulncapture-1.0.0/src/Vulncapture/Vulncapture.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:29:13.000000 Vulncapture-1.0.0/src/Vulncapture/__init__.py
--rw-rw-rw-   0        0        0     1559 2022-11-09 05:08:38.000000 Vulncapture-1.0.0/src/Vulncapture/dialogui.png
--rw-rw-rw-   0        0        0 15044440 2022-11-09 06:03:08.000000 Vulncapture-1.0.0/src/Vulncapture/mshei.ttf
--rw-rw-rw-   0        0        0       30 2023-04-26 03:34:33.000000 Vulncapture-1.0.0/src/Vulncapture/requirements.txt
--rw-rw-rw-   0        0        0     7710 2022-11-09 05:30:26.000000 Vulncapture-1.0.0/src/Vulncapture/titlegui.png
-drwxrwxrwx   0        0        0        0 2023-04-29 17:44:44.204359 Vulncapture-1.0.0/src/Vulncapture.egg-info/
--rw-rw-rw-   0        0        0     1238 2023-04-29 17:44:44.000000 Vulncapture-1.0.0/src/Vulncapture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-04-29 17:44:44.000000 Vulncapture-1.0.0/src/Vulncapture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 17:44:44.000000 Vulncapture-1.0.0/src/Vulncapture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 17:44:44.000000 Vulncapture-1.0.0/src/Vulncapture.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 04:05:41.301985 Vulncapture-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2023-04-26 08:28:29.000000 Vulncapture-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1323 2023-04-30 04:05:41.300977 Vulncapture-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      776 2023-04-30 04:05:25.000000 Vulncapture-1.0.1/README.md
+-rw-rw-rw-   0        0        0      631 2023-04-30 04:04:29.000000 Vulncapture-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 04:05:41.301985 Vulncapture-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      189 2023-04-29 17:26:11.000000 Vulncapture-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 04:05:41.280537 Vulncapture-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 04:05:41.299968 Vulncapture-1.0.1/src/Vulncapture.egg-info/
+-rw-rw-rw-   0        0        0     1323 2023-04-30 04:05:41.000000 Vulncapture-1.0.1/src/Vulncapture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-04-30 04:05:41.000000 Vulncapture-1.0.1/src/Vulncapture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 04:05:41.000000 Vulncapture-1.0.1/src/Vulncapture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 04:05:41.000000 Vulncapture-1.0.1/src/Vulncapture.egg-info/top_level.txt
```

### Comparing `Vulncapture-1.0.0/LICENSE` & `Vulncapture-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Vulncapture-1.0.0/pyproject.toml` & `Vulncapture-1.0.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Vulncapture"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="jiangyangcreate", email="jiangyangcreate@gamil.com" },
 ]
-description = "A capture moudle return base64image"
+description = "A capture moudle return base64 image"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

