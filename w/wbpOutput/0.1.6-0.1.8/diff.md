# Comparing `tmp/wbpOutput-0.1.6.tar.gz` & `tmp/wbpOutput-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpOutput-0.1.6.tar", last modified: Sat Jan 28 11:19:12 2023, max compression
+gzip compressed data, was "wbpOutput-0.1.8.tar", last modified: Sun Apr 30 09:18:53 2023, max compression
```

## Comparing `wbpOutput-0.1.6.tar` & `wbpOutput-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 11:19:12.240907 wbpOutput-0.1.6/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-01-28 11:19:10.000000 wbpOutput-0.1.6/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 11:19:12.236907 wbpOutput-0.1.6/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 11:19:12.238907 wbpOutput-0.1.6/Lib/wbpOutput/
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-01-28 11:19:10.000000 wbpOutput-0.1.6/Lib/wbpOutput/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5004 2023-01-28 11:19:10.000000 wbpOutput-0.1.6/Lib/wbpOutput/outputwin.py
--rw-rw-rw-   0 root         (0) root         (0)     2542 2023-01-28 11:19:10.000000 wbpOutput-0.1.6/Lib/wbpOutput/preferences.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 11:19:12.240907 wbpOutput-0.1.6/Lib/wbpOutput.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1002 2023-01-28 11:19:12.000000 wbpOutput-0.1.6/Lib/wbpOutput.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      342 2023-01-28 11:19:12.000000 wbpOutput-0.1.6/Lib/wbpOutput.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-28 11:19:12.000000 wbpOutput-0.1.6/Lib/wbpOutput.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-01-28 11:19:12.000000 wbpOutput-0.1.6/Lib/wbpOutput.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-01-28 11:19:12.000000 wbpOutput-0.1.6/Lib/wbpOutput.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-01-28 11:19:12.000000 wbpOutput-0.1.6/Lib/wbpOutput.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1002 2023-01-28 11:19:12.240907 wbpOutput-0.1.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-01-28 11:19:10.000000 wbpOutput-0.1.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1555 2023-01-28 11:19:12.241907 wbpOutput-0.1.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-01-28 11:19:10.000000 wbpOutput-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 09:18:53.410019 wbpOutput-0.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-30 09:18:51.000000 wbpOutput-0.1.8/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 09:18:53.406018 wbpOutput-0.1.8/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 09:18:53.408018 wbpOutput-0.1.8/Lib/wbpOutput/
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-04-30 09:18:51.000000 wbpOutput-0.1.8/Lib/wbpOutput/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5004 2023-04-30 09:18:51.000000 wbpOutput-0.1.8/Lib/wbpOutput/outputwin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2542 2023-04-30 09:18:51.000000 wbpOutput-0.1.8/Lib/wbpOutput/preferences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 09:18:53.410019 wbpOutput-0.1.8/Lib/wbpOutput.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1616 2023-04-30 09:18:53.000000 wbpOutput-0.1.8/Lib/wbpOutput.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      342 2023-04-30 09:18:53.000000 wbpOutput-0.1.8/Lib/wbpOutput.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 09:18:53.000000 wbpOutput-0.1.8/Lib/wbpOutput.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-30 09:18:53.000000 wbpOutput-0.1.8/Lib/wbpOutput.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-30 09:18:53.000000 wbpOutput-0.1.8/Lib/wbpOutput.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-30 09:18:53.000000 wbpOutput-0.1.8/Lib/wbpOutput.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1616 2023-04-30 09:18:53.410019 wbpOutput-0.1.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-04-30 09:18:51.000000 wbpOutput-0.1.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1701 2023-04-30 09:18:53.411019 wbpOutput-0.1.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-30 09:18:51.000000 wbpOutput-0.1.8/setup.py
```

### Comparing `wbpOutput-0.1.6/LICENSE` & `wbpOutput-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpOutput-0.1.6/Lib/wbpOutput/outputwin.py` & `wbpOutput-0.1.8/Lib/wbpOutput/outputwin.py`

 * *Files identical despite different names*

### Comparing `wbpOutput-0.1.6/Lib/wbpOutput/preferences.py` & `wbpOutput-0.1.8/Lib/wbpOutput/preferences.py`

 * *Files identical despite different names*

