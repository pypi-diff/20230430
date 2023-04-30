# Comparing `tmp/force-relative-import-0.0.1.tar.gz` & `tmp/force-relative-import-0.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "force-relative-import-0.0.1.tar", last modified: Sun Apr 30 10:38:56 2023, max compression
+gzip compressed data, was "force-relative-import-0.0.1.post1.tar", last modified: Sun Apr 30 10:50:10 2023, max compression
```

## Comparing `force-relative-import-0.0.1.tar` & `force-relative-import-0.0.1.post1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 10:38:56.324059 force-relative-import-0.0.1/
--rw-rw-rw-   0        0        0     1066 2019-06-16 06:53:07.000000 force-relative-import-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      280 2023-04-30 10:38:56.322495 force-relative-import-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1891 2023-04-30 10:19:10.000000 force-relative-import-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 10:38:56.286483 force-relative-import-0.0.1/force_relative_import/
--rw-rw-rw-   0        0        0     2542 2023-04-30 10:26:53.000000 force-relative-import-0.0.1/force_relative_import/__init__.py
--rw-rw-rw-   0        0        0      183 2023-04-30 05:25:44.000000 force-relative-import-0.0.1/force_relative_import/enable_now.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:38:56.290475 force-relative-import-0.0.1/force_relative_import.egg-info/
--rw-rw-rw-   0        0        0      280 2023-04-30 10:38:56.000000 force-relative-import-0.0.1/force_relative_import.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-04-30 10:38:56.000000 force-relative-import-0.0.1/force_relative_import.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 10:38:56.000000 force-relative-import-0.0.1/force_relative_import.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-30 10:38:56.000000 force-relative-import-0.0.1/force_relative_import.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 10:38:56.324059 force-relative-import-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      448 2023-04-30 09:24:37.000000 force-relative-import-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:50:05.175541 force-relative-import-0.0.1.post1/
+-rw-rw-rw-   0        0        0     1066 2019-06-16 06:53:07.000000 force-relative-import-0.0.1.post1/LICENSE
+-rw-rw-rw-   0        0        0     2406 2023-04-30 10:50:10.608086 force-relative-import-0.0.1.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     1891 2023-04-30 10:19:10.000000 force-relative-import-0.0.1.post1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 10:50:05.169662 force-relative-import-0.0.1.post1/force_relative_import/
+-rw-rw-rw-   0        0        0     2542 2023-04-30 10:26:53.000000 force-relative-import-0.0.1.post1/force_relative_import/__init__.py
+-rw-rw-rw-   0        0        0      183 2023-04-30 05:25:44.000000 force-relative-import-0.0.1.post1/force_relative_import/enable_now.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:50:10.607088 force-relative-import-0.0.1.post1/force_relative_import.egg-info/
+-rw-rw-rw-   0        0        0     2406 2023-04-30 10:50:10.000000 force-relative-import-0.0.1.post1/force_relative_import.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-04-30 10:50:10.000000 force-relative-import-0.0.1.post1/force_relative_import.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 10:50:10.000000 force-relative-import-0.0.1.post1/force_relative_import.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-30 10:50:10.000000 force-relative-import-0.0.1.post1/force_relative_import.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 10:50:10.609084 force-relative-import-0.0.1.post1/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-04-30 10:48:34.000000 force-relative-import-0.0.1.post1/setup.py
```

### Comparing `force-relative-import-0.0.1/LICENSE` & `force-relative-import-0.0.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `force-relative-import-0.0.1/README.md` & `force-relative-import-0.0.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `force-relative-import-0.0.1/force_relative_import/__init__.py` & `force-relative-import-0.0.1.post1/force_relative_import/__init__.py`

 * *Files identical despite different names*

