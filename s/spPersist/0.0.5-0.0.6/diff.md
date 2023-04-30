# Comparing `tmp/spPersist-0.0.5.tar.gz` & `tmp/spPersist-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-0.0.5.tar", last modified: Sun Apr 30 19:56:56 2023, max compression
+gzip compressed data, was "spPersist-0.0.6.tar", last modified: Sun Apr 30 20:10:36 2023, max compression
```

## Comparing `spPersist-0.0.5.tar` & `spPersist-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 19:56:56.220326 spPersist-0.0.5/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-04-30 19:14:25.000000 spPersist-0.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      738 2023-04-30 19:56:56.220326 spPersist-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      183 2023-04-30 19:13:31.000000 spPersist-0.0.5/README.md
--rw-r--r--   0 root         (0) root         (0)      597 2023-04-30 19:55:17.000000 spPersist-0.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      210 2023-04-30 19:56:56.220326 spPersist-0.0.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 19:56:56.220326 spPersist-0.0.5/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      738 2023-04-30 19:56:56.000000 spPersist-0.0.5/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      174 2023-04-30 19:56:56.000000 spPersist-0.0.5/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 19:56:56.000000 spPersist-0.0.5/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 19:56:56.000000 spPersist-0.0.5/spPersist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 20:10:36.194794 spPersist-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-04-30 19:14:25.000000 spPersist-0.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      718 2023-04-30 20:10:36.194794 spPersist-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      183 2023-04-30 19:13:31.000000 spPersist-0.0.6/README.md
+-rw-r--r--   0 root         (0) root         (0)      597 2023-04-30 20:08:59.000000 spPersist-0.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-30 20:10:36.194794 spPersist-0.0.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 20:10:36.192794 spPersist-0.0.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 20:10:36.193794 spPersist-0.0.6/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-30 19:01:59.000000 spPersist-0.0.6/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2853 2023-04-30 19:07:07.000000 spPersist-0.0.6/src/spPersist/read.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 20:10:36.194794 spPersist-0.0.6/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      718 2023-04-30 20:10:36.000000 spPersist-0.0.6/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      228 2023-04-30 20:10:36.000000 spPersist-0.0.6/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 20:10:36.000000 spPersist-0.0.6/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-30 20:10:36.000000 spPersist-0.0.6/src/spPersist.egg-info/top_level.txt
```

### Comparing `spPersist-0.0.5/LICENSE` & `spPersist-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-0.0.5/pyproject.toml` & `spPersist-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spPersist"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial analysis package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

