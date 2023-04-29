# Comparing `tmp/luau-0.4.2.tar.gz` & `tmp/luau-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luau-0.4.2.tar", last modified: Sat Apr 29 22:41:09 2023, max compression
+gzip compressed data, was "luau-0.4.3.tar", last modified: Sat Apr 29 22:56:07 2023, max compression
```

## Comparing `luau-0.4.2.tar` & `luau-0.4.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 22:41:09.220904 luau-0.4.2/
--rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.4.2/LICENSE
--rw-rw-rw-   0        0        0      143 2023-04-29 22:40:12.000000 luau-0.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0      405 2023-04-29 22:41:09.219918 luau-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.4.2/README.md
--rw-rw-rw-   0        0        0      710 2023-04-29 22:40:30.000000 luau-0.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 22:41:09.220904 luau-0.4.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-29 22:41:09.147100 luau-0.4.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-29 22:41:09.159083 luau-0.4.2/src/luau/
--rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.4.2/src/luau/__init__.py
--rw-rw-rw-   0        0        0     5709 2023-04-15 01:24:18.000000 luau-0.4.2/src/luau/convert.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:41:09.199960 luau-0.4.2/src/luau/data/
--rwxrwxrwx   0        0        0  6183936 2022-02-01 23:24:24.000000 luau-0.4.2/src/luau/data/rojo.exe
--rwxrwxrwx   0        0        0  6183936 2022-02-01 23:24:24.000000 luau-0.4.2/src/luau/data/stylua.exe
--rwxrwxrwx   0        0        0  6183936 2022-02-01 23:24:24.000000 luau-0.4.2/src/luau/data/wally-package-types.exe
--rw-rw-rw-   0        0        0     2627 2023-04-18 16:26:04.000000 luau-0.4.2/src/luau/path.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:41:09.217918 luau-0.4.2/src/luau/roblox/
--rw-rw-rw-   0        0        0      997 2023-04-29 22:08:10.000000 luau-0.4.2/src/luau/roblox/__init__.py
--rw-rw-rw-   0        0        0   117136 2023-04-29 21:45:18.000000 luau-0.4.2/src/luau/roblox/api.py
--rw-rw-rw-   0        0        0     1761 2023-04-29 22:08:06.000000 luau-0.4.2/src/luau/roblox/rojo.py
--rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.4.2/src/luau/roblox/tool.py
--rw-rw-rw-   0        0        0     1689 2023-04-29 22:08:06.000000 luau-0.4.2/src/luau/roblox/util.py
--rw-rw-rw-   0        0        0     2734 2023-04-29 22:09:37.000000 luau-0.4.2/src/luau/roblox/wally.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:41:09.174030 luau-0.4.2/src/luau.egg-info/
--rw-rw-rw-   0        0        0      405 2023-04-29 22:41:09.000000 luau-0.4.2/src/luau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      495 2023-04-29 22:41:09.000000 luau-0.4.2/src/luau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 22:41:09.000000 luau-0.4.2/src/luau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-04-29 22:41:09.000000 luau-0.4.2/src/luau.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-29 22:41:09.000000 luau-0.4.2/src/luau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 22:56:07.538852 luau-0.4.3/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0      143 2023-04-29 22:40:12.000000 luau-0.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      405 2023-04-29 22:56:07.537867 luau-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.4.3/README.md
+-rw-rw-rw-   0        0        0      710 2023-04-29 22:55:39.000000 luau-0.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 22:56:07.538852 luau-0.4.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 22:56:07.467044 luau-0.4.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-29 22:56:07.479010 luau-0.4.3/src/luau/
+-rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.4.3/src/luau/__init__.py
+-rw-rw-rw-   0        0        0     5709 2023-04-15 01:24:18.000000 luau-0.4.3/src/luau/convert.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:56:07.516908 luau-0.4.3/src/luau/data/
+-rwxrwxrwx   0        0        0  6183936 2022-02-01 23:24:24.000000 luau-0.4.3/src/luau/data/rojo.exe
+-rwxrwxrwx   0        0        0  6183936 2022-02-01 23:24:24.000000 luau-0.4.3/src/luau/data/stylua.exe
+-rwxrwxrwx   0        0        0  6183936 2022-02-01 23:24:24.000000 luau-0.4.3/src/luau/data/wally-package-types.exe
+-rw-rw-rw-   0        0        0     2627 2023-04-18 16:26:04.000000 luau-0.4.3/src/luau/path.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:56:07.535867 luau-0.4.3/src/luau/roblox/
+-rw-rw-rw-   0        0        0      997 2023-04-29 22:08:10.000000 luau-0.4.3/src/luau/roblox/__init__.py
+-rw-rw-rw-   0        0        0   117136 2023-04-29 21:45:18.000000 luau-0.4.3/src/luau/roblox/api.py
+-rw-rw-rw-   0        0        0     1761 2023-04-29 22:08:06.000000 luau-0.4.3/src/luau/roblox/rojo.py
+-rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.4.3/src/luau/roblox/tool.py
+-rw-rw-rw-   0        0        0     1410 2023-04-29 22:55:31.000000 luau-0.4.3/src/luau/roblox/util.py
+-rw-rw-rw-   0        0        0     2734 2023-04-29 22:09:37.000000 luau-0.4.3/src/luau/roblox/wally.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:56:07.492973 luau-0.4.3/src/luau.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-04-29 22:56:07.000000 luau-0.4.3/src/luau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      495 2023-04-29 22:56:07.000000 luau-0.4.3/src/luau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 22:56:07.000000 luau-0.4.3/src/luau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-29 22:56:07.000000 luau-0.4.3/src/luau.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-29 22:56:07.000000 luau-0.4.3/src/luau.egg-info/top_level.txt
```

### Comparing `luau-0.4.2/LICENSE` & `luau-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `luau-0.4.2/pyproject.toml` & `luau-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 	requires = ["setuptools>=61.0"]
 	build-backend = "setuptools.build_meta"
 
 [project]
 	name = "luau"
-	version = "0.4.2"
+	version = "0.4.3"
 	authors = [
 		{ name="nightcycle", email="coyer@nightcycle.us" },
 	]
 	dependencies = [
 		"dpath~=2.1.5",
 		"toml~=0.10.2",
 		"requests~=2.28.2",
```

### Comparing `luau-0.4.2/src/luau/__init__.py` & `luau-0.4.3/src/luau/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.2/src/luau/convert.py` & `luau-0.4.3/src/luau/convert.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.2/src/luau/data/rojo.exe` & `luau-0.4.3/src/luau/data/rojo.exe`

 * *Files identical despite different names*

### Comparing `luau-0.4.2/src/luau/data/stylua.exe` & `luau-0.4.3/src/luau/data/stylua.exe`

 * *Files identical despite different names*

### Comparing `luau-0.4.2/src/luau/data/wally-package-types.exe` & `luau-0.4.3/src/luau/data/wally-package-types.exe`

 * *Files identical despite different names*

### Comparing `luau-0.4.2/src/luau/path.py` & `luau-0.4.3/src/luau/path.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.2/src/luau/roblox/__init__.py` & `luau-0.4.3/src/luau/roblox/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.2/src/luau/roblox/api.py` & `luau-0.4.3/src/luau/roblox/api.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.2/src/luau/roblox/rojo.py` & `luau-0.4.3/src/luau/roblox/rojo.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.2/src/luau/roblox/tool.py` & `luau-0.4.3/src/luau/roblox/tool.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.2/src/luau/roblox/wally.py` & `luau-0.4.3/src/luau/roblox/wally.py`

 * *Files identical despite different names*

