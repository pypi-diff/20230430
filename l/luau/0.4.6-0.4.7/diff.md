# Comparing `tmp/luau-0.4.6.tar.gz` & `tmp/luau-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luau-0.4.6.tar", last modified: Sun Apr 30 00:42:05 2023, max compression
+gzip compressed data, was "luau-0.4.7.tar", last modified: Sun Apr 30 00:44:35 2023, max compression
```

## Comparing `luau-0.4.6.tar` & `luau-0.4.7.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 00:42:05.851933 luau-0.4.6/
--rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.4.6/LICENSE
--rw-rw-rw-   0        0        0       37 2023-04-30 00:41:23.000000 luau-0.4.6/MANIFEST.in
--rw-rw-rw-   0        0        0      405 2023-04-30 00:42:05.850937 luau-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.4.6/README.md
--rw-rw-rw-   0        0        0      710 2023-04-30 00:41:39.000000 luau-0.4.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 00:42:05.851933 luau-0.4.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-30 00:42:05.795114 luau-0.4.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 00:42:05.807292 luau-0.4.6/src/luau/
--rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.4.6/src/luau/__init__.py
--rw-rw-rw-   0        0        0     5709 2023-04-15 01:24:18.000000 luau-0.4.6/src/luau/convert.py
--rw-rw-rw-   0        0        0     2627 2023-04-18 16:26:04.000000 luau-0.4.6/src/luau/path.py
-drwxrwxrwx   0        0        0        0 2023-04-30 00:42:05.848942 luau-0.4.6/src/luau/roblox/
--rw-rw-rw-   0        0        0     1005 2023-04-30 00:28:17.000000 luau-0.4.6/src/luau/roblox/__init__.py
--rw-rw-rw-   0        0        0   117192 2023-04-30 00:41:42.000000 luau-0.4.6/src/luau/roblox/api.py
--rw-rw-rw-   0        0        0     1769 2023-04-30 00:28:16.000000 luau-0.4.6/src/luau/roblox/rojo.py
--rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.4.6/src/luau/roblox/tool.py
--rw-rw-rw-   0        0        0     1256 2023-04-30 00:28:16.000000 luau-0.4.6/src/luau/roblox/util.py
--rw-rw-rw-   0        0        0     2726 2023-04-30 00:28:16.000000 luau-0.4.6/src/luau/roblox/wally.py
-drwxrwxrwx   0        0        0        0 2023-04-30 00:42:05.840075 luau-0.4.6/src/luau.egg-info/
--rw-rw-rw-   0        0        0      405 2023-04-30 00:42:05.000000 luau-0.4.6/src/luau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-04-30 00:42:05.000000 luau-0.4.6/src/luau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 00:42:05.000000 luau-0.4.6/src/luau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-04-30 00:42:05.000000 luau-0.4.6/src/luau.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-30 00:42:05.000000 luau-0.4.6/src/luau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 00:44:35.736862 luau-0.4.7/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.4.7/LICENSE
+-rw-rw-rw-   0        0        0      151 2023-04-30 00:43:57.000000 luau-0.4.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      405 2023-04-30 00:44:35.735866 luau-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.4.7/README.md
+-rw-rw-rw-   0        0        0      710 2023-04-30 00:44:16.000000 luau-0.4.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 00:44:35.736862 luau-0.4.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 00:44:35.672280 luau-0.4.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 00:44:35.684980 luau-0.4.7/src/luau/
+-rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.4.7/src/luau/__init__.py
+-rw-rw-rw-   0        0        0     5709 2023-04-15 01:24:18.000000 luau-0.4.7/src/luau/convert.py
+drwxrwxrwx   0        0        0        0 2023-04-30 00:44:35.717001 luau-0.4.7/src/luau/data/
+-rwxrwxrwx   0        0        0  6183936 2022-02-01 23:24:24.000000 luau-0.4.7/src/luau/data/py_luau_rojo.exe
+-rwxrwxrwx   0        0        0  6183936 2022-02-01 23:24:24.000000 luau-0.4.7/src/luau/data/py_luau_stylua.exe
+-rwxrwxrwx   0        0        0  6183936 2022-02-01 23:24:24.000000 luau-0.4.7/src/luau/data/py_luau_wpt.exe
+-rw-rw-rw-   0        0        0     2627 2023-04-18 16:26:04.000000 luau-0.4.7/src/luau/path.py
+drwxrwxrwx   0        0        0        0 2023-04-30 00:44:35.734867 luau-0.4.7/src/luau/roblox/
+-rw-rw-rw-   0        0        0     1005 2023-04-30 00:28:17.000000 luau-0.4.7/src/luau/roblox/__init__.py
+-rw-rw-rw-   0        0        0   117192 2023-04-30 00:44:18.000000 luau-0.4.7/src/luau/roblox/api.py
+-rw-rw-rw-   0        0        0     1769 2023-04-30 00:28:16.000000 luau-0.4.7/src/luau/roblox/rojo.py
+-rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.4.7/src/luau/roblox/tool.py
+-rw-rw-rw-   0        0        0     1256 2023-04-30 00:28:16.000000 luau-0.4.7/src/luau/roblox/util.py
+-rw-rw-rw-   0        0        0     2726 2023-04-30 00:28:16.000000 luau-0.4.7/src/luau/roblox/wally.py
+drwxrwxrwx   0        0        0        0 2023-04-30 00:44:35.699673 luau-0.4.7/src/luau.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-04-30 00:44:35.000000 luau-0.4.7/src/luau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      503 2023-04-30 00:44:35.000000 luau-0.4.7/src/luau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 00:44:35.000000 luau-0.4.7/src/luau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-30 00:44:35.000000 luau-0.4.7/src/luau.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-30 00:44:35.000000 luau-0.4.7/src/luau.egg-info/top_level.txt
```

### Comparing `luau-0.4.6/LICENSE` & `luau-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `luau-0.4.6/pyproject.toml` & `luau-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 	requires = ["setuptools>=61.0"]
 	build-backend = "setuptools.build_meta"
 
 [project]
 	name = "luau"
-	version = "0.4.6"
+	version = "0.4.7"
 	authors = [
 		{ name="nightcycle", email="coyer@nightcycle.us" },
 	]
 	dependencies = [
 		"dpath~=2.1.5",
 		"toml~=0.10.2",
 		"requests~=2.28.2",
```

### Comparing `luau-0.4.6/src/luau/__init__.py` & `luau-0.4.7/src/luau/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.6/src/luau/convert.py` & `luau-0.4.7/src/luau/convert.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.6/src/luau/path.py` & `luau-0.4.7/src/luau/path.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.6/src/luau/roblox/__init__.py` & `luau-0.4.7/src/luau/roblox/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.6/src/luau/roblox/api.py` & `luau-0.4.7/src/luau/roblox/api.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.6/src/luau/roblox/rojo.py` & `luau-0.4.7/src/luau/roblox/rojo.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.6/src/luau/roblox/tool.py` & `luau-0.4.7/src/luau/roblox/tool.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.6/src/luau/roblox/util.py` & `luau-0.4.7/src/luau/roblox/util.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.6/src/luau/roblox/wally.py` & `luau-0.4.7/src/luau/roblox/wally.py`

 * *Files identical despite different names*

