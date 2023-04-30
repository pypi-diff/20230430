# Comparing `tmp/luau-0.4.4.tar.gz` & `tmp/luau-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luau-0.4.4.tar", last modified: Sun Apr 30 00:30:04 2023, max compression
+gzip compressed data, was "luau-0.4.5.tar", last modified: Sun Apr 30 00:31:15 2023, max compression
```

## Comparing `luau-0.4.4.tar` & `luau-0.4.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 00:30:04.971490 luau-0.4.4/
--rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.4.4/LICENSE
--rw-rw-rw-   0        0        0      143 2023-04-29 22:40:12.000000 luau-0.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0      405 2023-04-30 00:30:04.970492 luau-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.4.4/README.md
--rw-rw-rw-   0        0        0      710 2023-04-30 00:28:36.000000 luau-0.4.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 00:30:04.971490 luau-0.4.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-30 00:30:04.930128 luau-0.4.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 00:30:04.943086 luau-0.4.4/src/luau/
--rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.4.4/src/luau/__init__.py
--rw-rw-rw-   0        0        0     5709 2023-04-15 01:24:18.000000 luau-0.4.4/src/luau/convert.py
--rw-rw-rw-   0        0        0     2627 2023-04-18 16:26:04.000000 luau-0.4.4/src/luau/path.py
-drwxrwxrwx   0        0        0        0 2023-04-30 00:30:04.968497 luau-0.4.4/src/luau/roblox/
--rw-rw-rw-   0        0        0     1005 2023-04-30 00:28:17.000000 luau-0.4.4/src/luau/roblox/__init__.py
--rw-rw-rw-   0        0        0   117192 2023-04-30 00:29:46.000000 luau-0.4.4/src/luau/roblox/api.py
--rw-rw-rw-   0        0        0     1769 2023-04-30 00:28:16.000000 luau-0.4.4/src/luau/roblox/rojo.py
--rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.4.4/src/luau/roblox/tool.py
--rw-rw-rw-   0        0        0     1256 2023-04-30 00:28:16.000000 luau-0.4.4/src/luau/roblox/util.py
--rw-rw-rw-   0        0        0     2726 2023-04-30 00:28:16.000000 luau-0.4.4/src/luau/roblox/wally.py
-drwxrwxrwx   0        0        0        0 2023-04-30 00:30:04.958524 luau-0.4.4/src/luau.egg-info/
--rw-rw-rw-   0        0        0      405 2023-04-30 00:30:04.000000 luau-0.4.4/src/luau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-04-30 00:30:04.000000 luau-0.4.4/src/luau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 00:30:04.000000 luau-0.4.4/src/luau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-04-30 00:30:04.000000 luau-0.4.4/src/luau.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-30 00:30:04.000000 luau-0.4.4/src/luau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 00:31:15.109279 luau-0.4.5/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0      143 2023-04-29 22:40:12.000000 luau-0.4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      405 2023-04-30 00:31:15.108283 luau-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.4.5/README.md
+-rw-rw-rw-   0        0        0      710 2023-04-30 00:30:54.000000 luau-0.4.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 00:31:15.109279 luau-0.4.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 00:31:15.009134 luau-0.4.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 00:31:15.070472 luau-0.4.5/src/luau/
+-rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.4.5/src/luau/__init__.py
+-rw-rw-rw-   0        0        0     5709 2023-04-15 01:24:18.000000 luau-0.4.5/src/luau/convert.py
+-rw-rw-rw-   0        0        0     2627 2023-04-18 16:26:04.000000 luau-0.4.5/src/luau/path.py
+drwxrwxrwx   0        0        0        0 2023-04-30 00:31:15.106288 luau-0.4.5/src/luau/roblox/
+-rw-rw-rw-   0        0        0     1005 2023-04-30 00:28:17.000000 luau-0.4.5/src/luau/roblox/__init__.py
+-rw-rw-rw-   0        0        0   117192 2023-04-30 00:30:57.000000 luau-0.4.5/src/luau/roblox/api.py
+-rw-rw-rw-   0        0        0     1769 2023-04-30 00:28:16.000000 luau-0.4.5/src/luau/roblox/rojo.py
+-rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.4.5/src/luau/roblox/tool.py
+-rw-rw-rw-   0        0        0     1256 2023-04-30 00:28:16.000000 luau-0.4.5/src/luau/roblox/util.py
+-rw-rw-rw-   0        0        0     2726 2023-04-30 00:28:16.000000 luau-0.4.5/src/luau/roblox/wally.py
+drwxrwxrwx   0        0        0        0 2023-04-30 00:31:15.096422 luau-0.4.5/src/luau.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-04-30 00:31:14.000000 luau-0.4.5/src/luau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-04-30 00:31:15.000000 luau-0.4.5/src/luau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 00:31:14.000000 luau-0.4.5/src/luau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-30 00:31:14.000000 luau-0.4.5/src/luau.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-30 00:31:14.000000 luau-0.4.5/src/luau.egg-info/top_level.txt
```

### Comparing `luau-0.4.4/LICENSE` & `luau-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `luau-0.4.4/pyproject.toml` & `luau-0.4.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 	requires = ["setuptools>=61.0"]
 	build-backend = "setuptools.build_meta"
 
 [project]
 	name = "luau"
-	version = "0.4.4"
+	version = "0.4.5"
 	authors = [
 		{ name="nightcycle", email="coyer@nightcycle.us" },
 	]
 	dependencies = [
 		"dpath~=2.1.5",
 		"toml~=0.10.2",
 		"requests~=2.28.2",
```

### Comparing `luau-0.4.4/src/luau/__init__.py` & `luau-0.4.5/src/luau/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.4/src/luau/convert.py` & `luau-0.4.5/src/luau/convert.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.4/src/luau/path.py` & `luau-0.4.5/src/luau/path.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.4/src/luau/roblox/__init__.py` & `luau-0.4.5/src/luau/roblox/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.4/src/luau/roblox/api.py` & `luau-0.4.5/src/luau/roblox/api.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.4/src/luau/roblox/rojo.py` & `luau-0.4.5/src/luau/roblox/rojo.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.4/src/luau/roblox/tool.py` & `luau-0.4.5/src/luau/roblox/tool.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.4/src/luau/roblox/util.py` & `luau-0.4.5/src/luau/roblox/util.py`

 * *Files identical despite different names*

### Comparing `luau-0.4.4/src/luau/roblox/wally.py` & `luau-0.4.5/src/luau/roblox/wally.py`

 * *Files identical despite different names*

