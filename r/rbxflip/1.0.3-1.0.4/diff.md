# Comparing `tmp/rbxflip-1.0.3.tar.gz` & `tmp/rbxflip-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbxflip-1.0.3.tar", last modified: Sun Apr 30 16:19:09 2023, max compression
+gzip compressed data, was "rbxflip-1.0.4.tar", last modified: Sun Apr 30 16:21:10 2023, max compression
```

## Comparing `rbxflip-1.0.3.tar` & `rbxflip-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 16:19:09.611273 rbxflip-1.0.3/
--rw-rw-rw-   0        0        0      236 2023-04-30 16:19:09.609962 rbxflip-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1220 2023-04-30 15:05:56.000000 rbxflip-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 16:19:09.583466 rbxflip-1.0.3/rbxflip/
--rw-rw-rw-   0        0        0      241 2023-04-30 16:17:29.000000 rbxflip-1.0.3/rbxflip/__init__.py
--rw-rw-rw-   0        0        0       88 2023-04-30 14:21:56.000000 rbxflip-1.0.3/rbxflip/errors.py
--rw-rw-rw-   0        0        0      482 2023-04-30 15:55:59.000000 rbxflip-1.0.3/rbxflip/roulette.py
--rw-rw-rw-   0        0        0     1160 2023-04-30 16:16:49.000000 rbxflip-1.0.3/rbxflip/shop.py
--rw-rw-rw-   0        0        0     1288 2023-04-30 15:58:24.000000 rbxflip-1.0.3/rbxflip/user.py
--rw-rw-rw-   0        0        0     1877 2023-04-30 08:23:52.000000 rbxflip-1.0.3/rbxflip/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:19:09.606668 rbxflip-1.0.3/rbxflip.egg-info/
--rw-rw-rw-   0        0        0      236 2023-04-30 16:19:09.000000 rbxflip-1.0.3/rbxflip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-04-30 16:19:09.000000 rbxflip-1.0.3/rbxflip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 16:19:09.000000 rbxflip-1.0.3/rbxflip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-30 16:19:09.000000 rbxflip-1.0.3/rbxflip.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-30 16:19:09.000000 rbxflip-1.0.3/rbxflip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 16:19:09.611795 rbxflip-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      297 2023-04-30 16:18:14.000000 rbxflip-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:21:10.779745 rbxflip-1.0.4/
+-rw-rw-rw-   0        0        0      236 2023-04-30 16:21:10.777362 rbxflip-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1220 2023-04-30 15:05:56.000000 rbxflip-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 16:21:10.750707 rbxflip-1.0.4/rbxflip/
+-rw-rw-rw-   0        0        0      241 2023-04-30 16:20:37.000000 rbxflip-1.0.4/rbxflip/__init__.py
+-rw-rw-rw-   0        0        0       88 2023-04-30 14:21:56.000000 rbxflip-1.0.4/rbxflip/errors.py
+-rw-rw-rw-   0        0        0      482 2023-04-30 15:55:59.000000 rbxflip-1.0.4/rbxflip/roulette.py
+-rw-rw-rw-   0        0        0     1160 2023-04-30 16:20:57.000000 rbxflip-1.0.4/rbxflip/shop.py
+-rw-rw-rw-   0        0        0     1288 2023-04-30 15:58:24.000000 rbxflip-1.0.4/rbxflip/user.py
+-rw-rw-rw-   0        0        0     1877 2023-04-30 08:23:52.000000 rbxflip-1.0.4/rbxflip/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:21:10.774956 rbxflip-1.0.4/rbxflip.egg-info/
+-rw-rw-rw-   0        0        0      236 2023-04-30 16:21:10.000000 rbxflip-1.0.4/rbxflip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-04-30 16:21:10.000000 rbxflip-1.0.4/rbxflip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 16:21:10.000000 rbxflip-1.0.4/rbxflip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 16:21:10.000000 rbxflip-1.0.4/rbxflip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-30 16:21:10.000000 rbxflip-1.0.4/rbxflip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 16:21:10.780837 rbxflip-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      297 2023-04-30 16:21:06.000000 rbxflip-1.0.4/setup.py
```

### Comparing `rbxflip-1.0.3/README.md` & `rbxflip-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rbxflip-1.0.3/rbxflip/shop.py` & `rbxflip-1.0.4/rbxflip/shop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 from .errors import ItemNotFound
 
-class shop:
+class Shop:
     def __init__(self, id: int):
         self.id = id
         self.data = self.get_item_data()
 
     def __str__(self):
         return self.name
```

### Comparing `rbxflip-1.0.3/rbxflip/user.py` & `rbxflip-1.0.4/rbxflip/user.py`

 * *Files identical despite different names*

### Comparing `rbxflip-1.0.3/rbxflip/utils.py` & `rbxflip-1.0.4/rbxflip/utils.py`

 * *Files identical despite different names*

