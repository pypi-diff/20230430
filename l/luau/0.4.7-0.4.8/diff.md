# Comparing `tmp/luau-0.4.7.tar.gz` & `tmp/luau-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luau-0.4.7.tar", last modified: Sun Apr 30 00:44:35 2023, max compression
+gzip compressed data, was "luau-0.4.8.tar", last modified: Sun Apr 30 05:24:53 2023, max compression
```

## Comparing `luau-0.4.7.tar` & `luau-0.4.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 00:44:35.736862 luau-0.4.7/
--rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.4.7/LICENSE
--rw-rw-rw-   0        0        0      151 2023-04-30 00:43:57.000000 luau-0.4.7/MANIFEST.in
--rw-rw-rw-   0        0        0      405 2023-04-30 00:44:35.735866 luau-0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.4.7/README.md
--rw-rw-rw-   0        0        0      710 2023-04-30 00:44:16.000000 luau-0.4.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 00:44:35.736862 luau-0.4.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-30 00:44:35.672280 luau-0.4.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 00:44:35.684980 luau-0.4.7/src/luau/
--rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.4.7/src/luau/__init__.py
--rw-rw-rw-   0        0        0     5709 2023-04-15 01:24:18.000000 luau-0.4.7/src/luau/convert.py
-drwxrwxrwx   0        0        0        0 2023-04-30 00:44:35.717001 luau-0.4.7/src/luau/data/
--rwxrwxrwx   0        0        0  6183936 2022-02-01 23:24:24.000000 luau-0.4.7/src/luau/data/py_luau_rojo.exe
--rwxrwxrwx   0        0        0  6183936 2022-02-01 23:24:24.000000 luau-0.4.7/src/luau/data/py_luau_stylua.exe
--rwxrwxrwx   0        0        0  6183936 2022-02-01 23:24:24.000000 luau-0.4.7/src/luau/data/py_luau_wpt.exe
--rw-rw-rw-   0        0        0     2627 2023-04-18 16:26:04.000000 luau-0.4.7/src/luau/path.py
-drwxrwxrwx   0        0        0        0 2023-04-30 00:44:35.734867 luau-0.4.7/src/luau/roblox/
--rw-rw-rw-   0        0        0     1005 2023-04-30 00:28:17.000000 luau-0.4.7/src/luau/roblox/__init__.py
--rw-rw-rw-   0        0        0   117192 2023-04-30 00:44:18.000000 luau-0.4.7/src/luau/roblox/api.py
--rw-rw-rw-   0        0        0     1769 2023-04-30 00:28:16.000000 luau-0.4.7/src/luau/roblox/rojo.py
--rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.4.7/src/luau/roblox/tool.py
--rw-rw-rw-   0        0        0     1256 2023-04-30 00:28:16.000000 luau-0.4.7/src/luau/roblox/util.py
--rw-rw-rw-   0        0        0     2726 2023-04-30 00:28:16.000000 luau-0.4.7/src/luau/roblox/wally.py
-drwxrwxrwx   0        0        0        0 2023-04-30 00:44:35.699673 luau-0.4.7/src/luau.egg-info/
--rw-rw-rw-   0        0        0      405 2023-04-30 00:44:35.000000 luau-0.4.7/src/luau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      503 2023-04-30 00:44:35.000000 luau-0.4.7/src/luau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 00:44:35.000000 luau-0.4.7/src/luau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-04-30 00:44:35.000000 luau-0.4.7/src/luau.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-30 00:44:35.000000 luau-0.4.7/src/luau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 05:24:53.346729 luau-0.4.8/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.4.8/LICENSE
+-rw-rw-rw-   0        0        0      151 2023-04-30 00:43:57.000000 luau-0.4.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      405 2023-04-30 05:24:53.346729 luau-0.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.4.8/README.md
+-rw-rw-rw-   0        0        0      710 2023-04-30 05:24:06.000000 luau-0.4.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 05:24:53.347727 luau-0.4.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 05:24:53.268676 luau-0.4.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 05:24:53.282340 luau-0.4.8/src/luau/
+-rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.4.8/src/luau/__init__.py
+-rw-rw-rw-   0        0        0     5709 2023-04-15 01:24:18.000000 luau-0.4.8/src/luau/convert.py
+drwxrwxrwx   0        0        0        0 2023-04-30 05:24:53.328771 luau-0.4.8/src/luau/data/
+-rwxrwxrwx   0        0        0  6183936 2022-02-01 23:24:24.000000 luau-0.4.8/src/luau/data/py_luau_rojo.exe
+-rwxrwxrwx   0        0        0  6183936 2022-02-01 23:24:24.000000 luau-0.4.8/src/luau/data/py_luau_stylua.exe
+-rwxrwxrwx   0        0        0  6183936 2022-02-01 23:24:24.000000 luau-0.4.8/src/luau/data/py_luau_wpt.exe
+-rw-rw-rw-   0        0        0     2627 2023-04-18 16:26:04.000000 luau-0.4.8/src/luau/path.py
+drwxrwxrwx   0        0        0        0 2023-04-30 05:24:53.344735 luau-0.4.8/src/luau/roblox/
+-rw-rw-rw-   0        0        0     1005 2023-04-30 00:28:17.000000 luau-0.4.8/src/luau/roblox/__init__.py
+-rw-rw-rw-   0        0        0   117192 2023-04-30 05:24:32.000000 luau-0.4.8/src/luau/roblox/api.py
+-rw-rw-rw-   0        0        0     1769 2023-04-30 00:28:16.000000 luau-0.4.8/src/luau/roblox/rojo.py
+-rw-rw-rw-   0        0        0     1661 2023-04-30 05:22:44.000000 luau-0.4.8/src/luau/roblox/tool.py
+-rw-rw-rw-   0        0        0     1256 2023-04-30 00:28:16.000000 luau-0.4.8/src/luau/roblox/util.py
+-rw-rw-rw-   0        0        0     2736 2023-04-30 05:22:44.000000 luau-0.4.8/src/luau/roblox/wally.py
+drwxrwxrwx   0        0        0        0 2023-04-30 05:24:53.304856 luau-0.4.8/src/luau.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-04-30 05:24:53.000000 luau-0.4.8/src/luau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      503 2023-04-30 05:24:53.000000 luau-0.4.8/src/luau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 05:24:53.000000 luau-0.4.8/src/luau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-30 05:24:53.000000 luau-0.4.8/src/luau.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-30 05:24:53.000000 luau-0.4.8/src/luau.egg-info/top_level.txt
```

### Comparing `luau-0.4.7/LICENSE` & `luau-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `luau-0.4.7/pyproject.toml` & `luau-0.4.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 	requires = ["setuptools>=61.0"]
 	build-backend = "setuptools.build_meta"
 
 [project]
 	name = "luau"
-	version = "0.4.7"
+	version = "0.4.8"
 	authors = [
 		{ name="nightcycle", email="coyer@nightcycle.us" },
 	]
 	dependencies = [
 		"dpath~=2.1.5",
 		"toml~=0.10.2",
 		"requests~=2.28.2",
```

### Comparing `luau-0.4.7/src/luau/__init__.py` & `luau-0.4.8/src/luau/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.7/src/luau/convert.py` & `luau-0.4.8/src/luau/convert.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.7/src/luau/data/py_luau_rojo.exe` & `luau-0.4.8/src/luau/data/py_luau_rojo.exe`

 * *Files identical despite different names*

### Comparing `luau-0.4.7/src/luau/data/py_luau_stylua.exe` & `luau-0.4.8/src/luau/data/py_luau_stylua.exe`

 * *Files identical despite different names*

### Comparing `luau-0.4.7/src/luau/data/py_luau_wpt.exe` & `luau-0.4.8/src/luau/data/py_luau_wpt.exe`

 * *Files identical despite different names*

### Comparing `luau-0.4.7/src/luau/path.py` & `luau-0.4.8/src/luau/path.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.7/src/luau/roblox/__init__.py` & `luau-0.4.8/src/luau/roblox/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.7/src/luau/roblox/api.py` & `luau-0.4.8/src/luau/roblox/api.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.7/src/luau/roblox/rojo.py` & `luau-0.4.8/src/luau/roblox/rojo.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.7/src/luau/roblox/util.py` & `luau-0.4.8/src/luau/roblox/util.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.7/src/luau/roblox/wally.py` & `luau-0.4.8/src/luau/roblox/wally.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 import toml
 from .util import run_bundled_exe
-from .tool import get_tool_name
+#from .tool import get_tool_name
 from .rojo import get_rojo_project_path, build_sourcemap
 
 WALLY_SOURCE = "UpliftGames/wally"
 WALLY_VERSION = "0.3.1"
 WPT_SOURCE = "JohnnyMorganz/wally-package-types"
 WPT_VERSION = "1.2.0"
 
 def get_wally_name():
-	return get_tool_name(WALLY_SOURCE, WALLY_VERSION)
+	return "wally" #get_tool_name(WALLY_SOURCE, WALLY_VERSION)
 
 def update_wally():
 
 	project_path = get_rojo_project_path()
 	wally_tool_name = get_wally_name()
 
 	os.system(f"{wally_tool_name} install")
```

