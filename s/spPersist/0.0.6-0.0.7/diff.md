# Comparing `tmp/spPersist-0.0.6.tar.gz` & `tmp/sppersist-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-0.0.6.tar", last modified: Sun Apr 30 20:10:36 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `spPersist-0.0.6.tar` & `sppersist-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,6 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 20:10:36.194794 spPersist-0.0.6/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-04-30 19:14:25.000000 spPersist-0.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      718 2023-04-30 20:10:36.194794 spPersist-0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      183 2023-04-30 19:13:31.000000 spPersist-0.0.6/README.md
--rw-r--r--   0 root         (0) root         (0)      597 2023-04-30 20:08:59.000000 spPersist-0.0.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-30 20:10:36.194794 spPersist-0.0.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 20:10:36.192794 spPersist-0.0.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 20:10:36.193794 spPersist-0.0.6/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-30 19:01:59.000000 spPersist-0.0.6/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2853 2023-04-30 19:07:07.000000 spPersist-0.0.6/src/spPersist/read.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 20:10:36.194794 spPersist-0.0.6/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      718 2023-04-30 20:10:36.000000 spPersist-0.0.6/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      228 2023-04-30 20:10:36.000000 spPersist-0.0.6/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 20:10:36.000000 spPersist-0.0.6/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-30 20:10:36.000000 spPersist-0.0.6/src/spPersist.egg-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.0.7/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 sppersist-0.0.7/src/spPersist/read.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.0.7/LICENSE
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sppersist-0.0.7/README.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sppersist-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 sppersist-0.0.7/PKG-INFO
```

### Comparing `spPersist-0.0.6/LICENSE` & `sppersist-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-0.0.6/pyproject.toml` & `sppersist-0.0.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial analysis package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `spPersist-0.0.6/src/spPersist/read.py` & `sppersist-0.0.7/src/spPersist/read.py`

 * *Files identical despite different names*

