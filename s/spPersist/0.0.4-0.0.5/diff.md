# Comparing `tmp/sppersist-0.0.4.tar.gz` & `tmp/spPersist-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "spPersist-0.0.5.tar", last modified: Sun Apr 30 19:56:56 2023, max compression
```

## Comparing `sppersist-0.0.4.tar` & `spPersist-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.0.4/src/spPersist/__init__.py
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 sppersist-0.0.4/src/spPersist/read.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.0.4/LICENSE
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sppersist-0.0.4/README.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 sppersist-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 sppersist-0.0.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 19:56:56.220326 spPersist-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-04-30 19:14:25.000000 spPersist-0.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      738 2023-04-30 19:56:56.220326 spPersist-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      183 2023-04-30 19:13:31.000000 spPersist-0.0.5/README.md
+-rw-r--r--   0 root         (0) root         (0)      597 2023-04-30 19:55:17.000000 spPersist-0.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      210 2023-04-30 19:56:56.220326 spPersist-0.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 19:56:56.220326 spPersist-0.0.5/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      738 2023-04-30 19:56:56.000000 spPersist-0.0.5/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      174 2023-04-30 19:56:56.000000 spPersist-0.0.5/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 19:56:56.000000 spPersist-0.0.5/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 19:56:56.000000 spPersist-0.0.5/spPersist.egg-info/top_level.txt
```

### Comparing `sppersist-0.0.4/LICENSE` & `spPersist-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-0.0.4/PKG-INFO` & `spPersist-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.0.4
-Summary: Spatial analysis with Persistent Homology
+Version: 0.0.5
+Summary: Spatial analysis package
+Author: Lirong Yang
+Author-email: Lirong Yang <lirong.yang@outlook.com>
+License: UNKNOWN
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Author-email: Lirong Yang <lirong.yang@outlook.com>
-License-File: LICENSE
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Spatial analysis package
 
 This is a simple example package. You can use
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
-to write your content.
+to write your content.
```

