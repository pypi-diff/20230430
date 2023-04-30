# Comparing `tmp/rbxflip-1.0.6.tar.gz` & `tmp/rbxflip-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbxflip-1.0.6.tar", last modified: Sun Apr 30 19:53:24 2023, max compression
+gzip compressed data, was "rbxflip-1.0.7.tar", last modified: Sun Apr 30 19:57:23 2023, max compression
```

## Comparing `rbxflip-1.0.6.tar` & `rbxflip-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 19:53:24.203599 rbxflip-1.0.6/
--rw-rw-rw-   0        0        0      236 2023-04-30 19:53:24.201253 rbxflip-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1220 2023-04-30 15:05:56.000000 rbxflip-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 19:53:24.174087 rbxflip-1.0.6/rbxflip/
--rw-rw-rw-   0        0        0      271 2023-04-30 19:52:53.000000 rbxflip-1.0.6/rbxflip/__init__.py
--rw-rw-rw-   0        0        0       88 2023-04-30 14:21:56.000000 rbxflip-1.0.6/rbxflip/errors.py
--rw-rw-rw-   0        0        0      482 2023-04-30 15:55:59.000000 rbxflip-1.0.6/rbxflip/roulette.py
--rw-rw-rw-   0        0        0     1160 2023-04-30 16:20:57.000000 rbxflip-1.0.6/rbxflip/shop.py
--rw-rw-rw-   0        0        0     1288 2023-04-30 15:58:24.000000 rbxflip-1.0.6/rbxflip/user.py
--rw-rw-rw-   0        0        0     1877 2023-04-30 08:23:52.000000 rbxflip-1.0.6/rbxflip/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-30 19:53:24.199046 rbxflip-1.0.6/rbxflip.egg-info/
--rw-rw-rw-   0        0        0      236 2023-04-30 19:53:23.000000 rbxflip-1.0.6/rbxflip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-04-30 19:53:24.000000 rbxflip-1.0.6/rbxflip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 19:53:23.000000 rbxflip-1.0.6/rbxflip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-30 19:53:23.000000 rbxflip-1.0.6/rbxflip.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-30 19:53:23.000000 rbxflip-1.0.6/rbxflip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 19:53:24.203599 rbxflip-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      297 2023-04-30 19:53:18.000000 rbxflip-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 19:57:23.070604 rbxflip-1.0.7/
+-rw-rw-rw-   0        0        0      236 2023-04-30 19:57:23.069591 rbxflip-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1220 2023-04-30 15:05:56.000000 rbxflip-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 19:57:23.043403 rbxflip-1.0.7/rbxflip/
+-rw-rw-rw-   0        0        0      271 2023-04-30 19:52:53.000000 rbxflip-1.0.7/rbxflip/__init__.py
+-rw-rw-rw-   0        0        0       88 2023-04-30 14:21:56.000000 rbxflip-1.0.7/rbxflip/errors.py
+-rw-rw-rw-   0        0        0      562 2023-04-30 19:56:59.000000 rbxflip-1.0.7/rbxflip/roulette.py
+-rw-rw-rw-   0        0        0     1160 2023-04-30 16:20:57.000000 rbxflip-1.0.7/rbxflip/shop.py
+-rw-rw-rw-   0        0        0     1288 2023-04-30 15:58:24.000000 rbxflip-1.0.7/rbxflip/user.py
+-rw-rw-rw-   0        0        0     1877 2023-04-30 08:23:52.000000 rbxflip-1.0.7/rbxflip/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-30 19:57:23.067398 rbxflip-1.0.7/rbxflip.egg-info/
+-rw-rw-rw-   0        0        0      236 2023-04-30 19:57:22.000000 rbxflip-1.0.7/rbxflip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-04-30 19:57:22.000000 rbxflip-1.0.7/rbxflip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 19:57:22.000000 rbxflip-1.0.7/rbxflip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 19:57:22.000000 rbxflip-1.0.7/rbxflip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-30 19:57:22.000000 rbxflip-1.0.7/rbxflip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 19:57:23.070604 rbxflip-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      297 2023-04-30 19:57:17.000000 rbxflip-1.0.7/setup.py
```

### Comparing `rbxflip-1.0.6/README.md` & `rbxflip-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `rbxflip-1.0.6/rbxflip/shop.py` & `rbxflip-1.0.7/rbxflip/shop.py`

 * *Files identical despite different names*

### Comparing `rbxflip-1.0.6/rbxflip/user.py` & `rbxflip-1.0.7/rbxflip/user.py`

 * *Files identical despite different names*

### Comparing `rbxflip-1.0.6/rbxflip/utils.py` & `rbxflip-1.0.7/rbxflip/utils.py`

 * *Files identical despite different names*

