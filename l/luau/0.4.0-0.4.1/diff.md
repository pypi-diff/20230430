# Comparing `tmp/luau-0.4.0.tar.gz` & `tmp/luau-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luau-0.4.0.tar", last modified: Sat Apr 29 22:13:29 2023, max compression
+gzip compressed data, was "luau-0.4.1.tar", last modified: Sat Apr 29 22:36:44 2023, max compression
```

## Comparing `luau-0.4.0.tar` & `luau-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 22:13:29.156001 luau-0.4.0/
--rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.4.0/LICENSE
--rw-rw-rw-   0        0        0      405 2023-04-29 22:13:29.155005 luau-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.4.0/README.md
--rw-rw-rw-   0        0        0      547 2023-04-29 22:13:02.000000 luau-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 22:13:29.156001 luau-0.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-29 22:13:29.102157 luau-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-29 22:13:29.117109 luau-0.4.0/src/luau/
--rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.4.0/src/luau/__init__.py
--rw-rw-rw-   0        0        0     5709 2023-04-15 01:24:18.000000 luau-0.4.0/src/luau/convert.py
--rw-rw-rw-   0        0        0     2627 2023-04-18 16:26:04.000000 luau-0.4.0/src/luau/path.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:13:29.152011 luau-0.4.0/src/luau/roblox/
--rw-rw-rw-   0        0        0      997 2023-04-29 22:08:10.000000 luau-0.4.0/src/luau/roblox/__init__.py
--rw-rw-rw-   0        0        0   117136 2023-04-29 21:45:18.000000 luau-0.4.0/src/luau/roblox/api.py
--rw-rw-rw-   0        0        0     1761 2023-04-29 22:08:06.000000 luau-0.4.0/src/luau/roblox/rojo.py
--rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.4.0/src/luau/roblox/tool.py
--rw-rw-rw-   0        0        0     1689 2023-04-29 22:08:06.000000 luau-0.4.0/src/luau/roblox/util.py
--rw-rw-rw-   0        0        0     2734 2023-04-29 22:09:37.000000 luau-0.4.0/src/luau/roblox/wally.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:13:29.141040 luau-0.4.0/src/luau.egg-info/
--rw-rw-rw-   0        0        0      405 2023-04-29 22:13:29.000000 luau-0.4.0/src/luau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2023-04-29 22:13:29.000000 luau-0.4.0/src/luau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 22:13:29.000000 luau-0.4.0/src/luau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-04-29 22:13:29.000000 luau-0.4.0/src/luau.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-29 22:13:29.000000 luau-0.4.0/src/luau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 22:36:44.615968 luau-0.4.1/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-04-29 22:36:44.614998 luau-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.4.1/README.md
+-rw-rw-rw-   0        0        0      710 2023-04-29 22:35:14.000000 luau-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 22:36:44.615968 luau-0.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 22:36:44.574081 luau-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-29 22:36:44.584059 luau-0.4.1/src/luau/
+-rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.4.1/src/luau/__init__.py
+-rw-rw-rw-   0        0        0     5709 2023-04-15 01:24:18.000000 luau-0.4.1/src/luau/convert.py
+-rw-rw-rw-   0        0        0     2627 2023-04-18 16:26:04.000000 luau-0.4.1/src/luau/path.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:36:44.610984 luau-0.4.1/src/luau/roblox/
+-rw-rw-rw-   0        0        0      997 2023-04-29 22:08:10.000000 luau-0.4.1/src/luau/roblox/__init__.py
+-rw-rw-rw-   0        0        0   117136 2023-04-29 21:45:18.000000 luau-0.4.1/src/luau/roblox/api.py
+-rw-rw-rw-   0        0        0     1761 2023-04-29 22:08:06.000000 luau-0.4.1/src/luau/roblox/rojo.py
+-rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.4.1/src/luau/roblox/tool.py
+-rw-rw-rw-   0        0        0     1689 2023-04-29 22:08:06.000000 luau-0.4.1/src/luau/roblox/util.py
+-rw-rw-rw-   0        0        0     2734 2023-04-29 22:09:37.000000 luau-0.4.1/src/luau/roblox/wally.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:36:44.601010 luau-0.4.1/src/luau.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-04-29 22:36:44.000000 luau-0.4.1/src/luau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-04-29 22:36:44.000000 luau-0.4.1/src/luau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 22:36:44.000000 luau-0.4.1/src/luau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-29 22:36:44.000000 luau-0.4.1/src/luau.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-29 22:36:44.000000 luau-0.4.1/src/luau.egg-info/top_level.txt
```

### Comparing `luau-0.4.0/LICENSE` & `luau-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `luau-0.4.0/pyproject.toml` & `luau-0.4.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 	requires = ["setuptools>=61.0"]
 	build-backend = "setuptools.build_meta"
 
 [project]
 	name = "luau"
-	version = "0.4.0"
+	version = "0.4.1"
 	authors = [
 		{ name="nightcycle", email="coyer@nightcycle.us" },
 	]
 	dependencies = [
 		"dpath~=2.1.5",
 		"toml~=0.10.2",
 		"requests~=2.28.2",
@@ -17,7 +17,12 @@
 	description = "a basic python package for writing luau scripts"
 	readme = "README.md"
 	requires-python = ">=3.10"
 	classifiers = [
 		"Programming Language :: Python :: 3",
 		"Operating System :: OS Independent",
 	]
+
+[options.package_data]
+rojo = ["src/luau/data/rojo.exe"]
+stylua = ["src/luau/data/stylua.exe"]
+wally-package-types = ["src/luau/data/wally-package-types.exe"]
```

### Comparing `luau-0.4.0/src/luau/__init__.py` & `luau-0.4.1/src/luau/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.0/src/luau/convert.py` & `luau-0.4.1/src/luau/convert.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.0/src/luau/path.py` & `luau-0.4.1/src/luau/path.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.0/src/luau/roblox/__init__.py` & `luau-0.4.1/src/luau/roblox/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.0/src/luau/roblox/api.py` & `luau-0.4.1/src/luau/roblox/api.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.0/src/luau/roblox/rojo.py` & `luau-0.4.1/src/luau/roblox/rojo.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.0/src/luau/roblox/tool.py` & `luau-0.4.1/src/luau/roblox/tool.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.0/src/luau/roblox/util.py` & `luau-0.4.1/src/luau/roblox/util.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.0/src/luau/roblox/wally.py` & `luau-0.4.1/src/luau/roblox/wally.py`

 * *Files identical despite different names*

