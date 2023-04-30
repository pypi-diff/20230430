# Comparing `tmp/rbxflip-1.0.0.tar.gz` & `tmp/rbxflip-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbxflip-1.0.0.tar", last modified: Sun Apr 30 15:21:59 2023, max compression
+gzip compressed data, was "rbxflip-1.0.2.tar", last modified: Sun Apr 30 16:13:04 2023, max compression
```

## Comparing `rbxflip-1.0.0.tar` & `rbxflip-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 15:21:59.960405 rbxflip-1.0.0/
--rw-rw-rw-   0        0        0      236 2023-04-30 15:21:59.959127 rbxflip-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1220 2023-04-30 15:05:56.000000 rbxflip-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 15:21:59.933265 rbxflip-1.0.0/rbxflip/
--rw-rw-rw-   0        0        0      134 2023-04-30 08:25:55.000000 rbxflip-1.0.0/rbxflip/__init__.py
--rw-rw-rw-   0        0        0       88 2023-04-30 14:21:56.000000 rbxflip-1.0.0/rbxflip/errors.py
--rw-rw-rw-   0        0        0      478 2023-04-30 14:56:08.000000 rbxflip-1.0.0/rbxflip/roulette.py
--rw-rw-rw-   0        0        0     1160 2023-04-30 14:55:49.000000 rbxflip-1.0.0/rbxflip/shop.py
--rw-rw-rw-   0        0        0     1127 2023-04-30 15:00:41.000000 rbxflip-1.0.0/rbxflip/user.py
--rw-rw-rw-   0        0        0     1877 2023-04-30 08:23:52.000000 rbxflip-1.0.0/rbxflip/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-30 15:21:59.956514 rbxflip-1.0.0/rbxflip.egg-info/
--rw-rw-rw-   0        0        0      236 2023-04-30 15:21:59.000000 rbxflip-1.0.0/rbxflip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-04-30 15:21:59.000000 rbxflip-1.0.0/rbxflip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 15:21:59.000000 rbxflip-1.0.0/rbxflip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-30 15:21:59.000000 rbxflip-1.0.0/rbxflip.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-30 15:21:59.000000 rbxflip-1.0.0/rbxflip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 15:21:59.960917 rbxflip-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      297 2023-04-30 15:06:25.000000 rbxflip-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:13:04.263320 rbxflip-1.0.2/
+-rw-rw-rw-   0        0        0      236 2023-04-30 16:13:04.262192 rbxflip-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1220 2023-04-30 15:05:56.000000 rbxflip-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 16:13:04.243975 rbxflip-1.0.2/rbxflip/
+-rw-rw-rw-   0        0        0      241 2023-04-30 15:59:52.000000 rbxflip-1.0.2/rbxflip/__init__.py
+-rw-rw-rw-   0        0        0       88 2023-04-30 14:21:56.000000 rbxflip-1.0.2/rbxflip/errors.py
+-rw-rw-rw-   0        0        0      482 2023-04-30 15:55:59.000000 rbxflip-1.0.2/rbxflip/roulette.py
+-rw-rw-rw-   0        0        0     1160 2023-04-30 15:50:26.000000 rbxflip-1.0.2/rbxflip/shop.py
+-rw-rw-rw-   0        0        0     1288 2023-04-30 15:58:24.000000 rbxflip-1.0.2/rbxflip/user.py
+-rw-rw-rw-   0        0        0     1877 2023-04-30 08:23:52.000000 rbxflip-1.0.2/rbxflip/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:13:04.259660 rbxflip-1.0.2/rbxflip.egg-info/
+-rw-rw-rw-   0        0        0      236 2023-04-30 16:13:03.000000 rbxflip-1.0.2/rbxflip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-04-30 16:13:04.000000 rbxflip-1.0.2/rbxflip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 16:13:03.000000 rbxflip-1.0.2/rbxflip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 16:13:03.000000 rbxflip-1.0.2/rbxflip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-30 16:13:04.000000 rbxflip-1.0.2/rbxflip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 16:13:04.263320 rbxflip-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      297 2023-04-30 16:07:35.000000 rbxflip-1.0.2/setup.py
```

### Comparing `rbxflip-1.0.0/README.md` & `rbxflip-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rbxflip-1.0.0/rbxflip/shop.py` & `rbxflip-1.0.2/rbxflip/shop.py`

 * *Files identical despite different names*

### Comparing `rbxflip-1.0.0/rbxflip/utils.py` & `rbxflip-1.0.2/rbxflip/utils.py`

 * *Files identical despite different names*

