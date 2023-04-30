# Comparing `tmp/rbxflip-1.0.7.tar.gz` & `tmp/rbxflip-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbxflip-1.0.7.tar", last modified: Sun Apr 30 19:57:23 2023, max compression
+gzip compressed data, was "rbxflip-1.0.8.tar", last modified: Sun Apr 30 20:37:55 2023, max compression
```

## Comparing `rbxflip-1.0.7.tar` & `rbxflip-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 19:57:23.070604 rbxflip-1.0.7/
--rw-rw-rw-   0        0        0      236 2023-04-30 19:57:23.069591 rbxflip-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1220 2023-04-30 15:05:56.000000 rbxflip-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 19:57:23.043403 rbxflip-1.0.7/rbxflip/
--rw-rw-rw-   0        0        0      271 2023-04-30 19:52:53.000000 rbxflip-1.0.7/rbxflip/__init__.py
--rw-rw-rw-   0        0        0       88 2023-04-30 14:21:56.000000 rbxflip-1.0.7/rbxflip/errors.py
--rw-rw-rw-   0        0        0      562 2023-04-30 19:56:59.000000 rbxflip-1.0.7/rbxflip/roulette.py
--rw-rw-rw-   0        0        0     1160 2023-04-30 16:20:57.000000 rbxflip-1.0.7/rbxflip/shop.py
--rw-rw-rw-   0        0        0     1288 2023-04-30 15:58:24.000000 rbxflip-1.0.7/rbxflip/user.py
--rw-rw-rw-   0        0        0     1877 2023-04-30 08:23:52.000000 rbxflip-1.0.7/rbxflip/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-30 19:57:23.067398 rbxflip-1.0.7/rbxflip.egg-info/
--rw-rw-rw-   0        0        0      236 2023-04-30 19:57:22.000000 rbxflip-1.0.7/rbxflip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-04-30 19:57:22.000000 rbxflip-1.0.7/rbxflip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 19:57:22.000000 rbxflip-1.0.7/rbxflip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-30 19:57:22.000000 rbxflip-1.0.7/rbxflip.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-30 19:57:22.000000 rbxflip-1.0.7/rbxflip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 19:57:23.070604 rbxflip-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      297 2023-04-30 19:57:17.000000 rbxflip-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 20:37:55.049644 rbxflip-1.0.8/
+-rw-rw-rw-   0        0        0      236 2023-04-30 20:37:55.049122 rbxflip-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1220 2023-04-30 20:37:37.000000 rbxflip-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 20:37:55.019088 rbxflip-1.0.8/rbxflip/
+-rw-rw-rw-   0        0        0      271 2023-04-30 19:52:53.000000 rbxflip-1.0.8/rbxflip/__init__.py
+-rw-rw-rw-   0        0        0       88 2023-04-30 14:21:56.000000 rbxflip-1.0.8/rbxflip/errors.py
+-rw-rw-rw-   0        0        0      529 2023-04-30 20:37:31.000000 rbxflip-1.0.8/rbxflip/roulette.py
+-rw-rw-rw-   0        0        0     1160 2023-04-30 16:20:57.000000 rbxflip-1.0.8/rbxflip/shop.py
+-rw-rw-rw-   0        0        0     1288 2023-04-30 15:58:24.000000 rbxflip-1.0.8/rbxflip/user.py
+-rw-rw-rw-   0        0        0     1877 2023-04-30 08:23:52.000000 rbxflip-1.0.8/rbxflip/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-30 20:37:55.046546 rbxflip-1.0.8/rbxflip.egg-info/
+-rw-rw-rw-   0        0        0      236 2023-04-30 20:37:54.000000 rbxflip-1.0.8/rbxflip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-04-30 20:37:54.000000 rbxflip-1.0.8/rbxflip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 20:37:54.000000 rbxflip-1.0.8/rbxflip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 20:37:54.000000 rbxflip-1.0.8/rbxflip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-30 20:37:54.000000 rbxflip-1.0.8/rbxflip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 20:37:55.050671 rbxflip-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      297 2023-04-30 20:37:47.000000 rbxflip-1.0.8/setup.py
```

### Comparing `rbxflip-1.0.7/README.md` & `rbxflip-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `rbxflip-1.0.7/rbxflip/roulette.py` & `rbxflip-1.0.8/rbxflip/roulette.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import requests
 
 class Roulette:
-    def __init__(self, data: dict):
-        roulette_data = data['roulette']
+    def __init__(self, roulette_data: dict):
         self.round = roulette_data['round']
         self.id = roulette_data['id']
         self.players = roulette_data['players']
         self.client_seed = roulette_data['clientSeed']
 
 
     def __str__(self):
```

### Comparing `rbxflip-1.0.7/rbxflip/shop.py` & `rbxflip-1.0.8/rbxflip/shop.py`

 * *Files identical despite different names*

### Comparing `rbxflip-1.0.7/rbxflip/user.py` & `rbxflip-1.0.8/rbxflip/user.py`

 * *Files identical despite different names*

### Comparing `rbxflip-1.0.7/rbxflip/utils.py` & `rbxflip-1.0.8/rbxflip/utils.py`

 * *Files identical despite different names*

