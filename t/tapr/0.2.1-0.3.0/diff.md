# Comparing `tmp/tapr-0.2.1.tar.gz` & `tmp/tapr-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapr-0.2.1.tar", last modified: Wed Jul 13 01:23:21 2022, max compression
+gzip compressed data, was "tapr-0.3.0.tar", last modified: Sun Apr 30 01:04:09 2023, max compression
```

## Comparing `tapr-0.2.1.tar` & `tapr-0.3.0.tar`

### file list

```diff
@@ -1,64 +1,46 @@
-drwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)        0 2022-07-13 01:23:21.670351 tapr-0.2.1/
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)     1104 2022-01-21 05:43:08.000000 tapr-0.2.1/LICENSE
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)     1536 2022-07-13 01:23:21.670351 tapr-0.2.1/PKG-INFO
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)      867 2022-01-27 00:13:32.000000 tapr-0.2.1/README.md
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)      103 2022-01-21 05:42:46.000000 tapr-0.2.1/pyproject.toml
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)       38 2022-07-13 01:23:21.670351 tapr-0.2.1/setup.cfg
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)     1111 2022-07-13 01:20:59.000000 tapr-0.2.1/setup.py
-drwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)        0 2022-07-13 01:23:21.662351 tapr-0.2.1/tapr/
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)     1451 2022-01-21 05:43:08.000000 tapr-0.2.1/tapr/__init__.py
-drwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)        0 2022-07-13 01:23:21.666351 tapr-0.2.1/tapr/io/
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)       98 2022-01-21 05:43:08.000000 tapr-0.2.1/tapr/io/__init__.py
--rwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)     3782 2022-02-16 04:24:37.000000 tapr-0.2.1/tapr/io/ntableio.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)     5507 2022-01-21 05:43:08.000000 tapr-0.2.1/tapr/io/serialization.py
-drwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)        0 2022-07-13 01:23:21.666351 tapr-0.2.1/tapr/main/
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)      285 2022-01-21 05:43:08.000000 tapr-0.2.1/tapr/main/__init__.py
--rwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)     2177 2022-01-21 05:43:08.000000 tapr-0.2.1/tapr/main/alchemy.py
--rwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)     6809 2022-07-12 02:39:28.000000 tapr-0.2.1/tapr/main/conversion.py
--rwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)      452 2022-01-21 05:43:08.000000 tapr-0.2.1/tapr/main/defs.py
--rwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)     1899 2022-06-19 21:21:27.000000 tapr-0.2.1/tapr/main/engines.py
--rwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)      892 2022-01-21 05:43:08.000000 tapr-0.2.1/tapr/main/filtering.py
--rwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)     1626 2022-01-21 05:43:08.000000 tapr-0.2.1/tapr/main/handling.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)    15942 2022-07-12 02:05:54.000000 tapr-0.2.1/tapr/main/ntable.py
--rwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)     2250 2022-06-13 05:24:33.000000 tapr-0.2.1/tapr/main/processing.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)     3570 2022-01-21 05:43:08.000000 tapr-0.2.1/tapr/main/qol.py
--rwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)     7750 2022-01-21 05:43:08.000000 tapr-0.2.1/tapr/main/structure.py
--rwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)     2063 2022-02-16 04:14:41.000000 tapr-0.2.1/tapr/main/tabularization.py
--rwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)      186 2022-01-21 05:43:08.000000 tapr-0.2.1/tapr/main/ttypes.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)    11964 2022-07-12 03:01:57.000000 tapr-0.2.1/tapr/main/utils.py
-drwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)        0 2022-07-13 01:23:21.666351 tapr-0.2.1/tapr/visualization/
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)        0 2022-01-21 05:43:08.000000 tapr-0.2.1/tapr/visualization/__init__.py
-drwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)        0 2022-07-13 01:23:21.666351 tapr-0.2.1/tapr/visualization/matplotlib/
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)        0 2022-01-21 05:43:08.000000 tapr-0.2.1/tapr/visualization/matplotlib/__init__.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)      303 2022-02-16 04:26:06.000000 tapr-0.2.1/tapr/visualization/matplotlib/pyplot.py
-drwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)        0 2022-07-13 01:23:21.666351 tapr-0.2.1/tapr/visualization/plotly/
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)        0 2022-01-21 05:43:08.000000 tapr-0.2.1/tapr/visualization/plotly/__init__.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)      299 2022-02-16 04:25:33.000000 tapr-0.2.1/tapr/visualization/plotly/express.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)      302 2022-02-16 04:25:56.000000 tapr-0.2.1/tapr/visualization/plotly/graph_objs.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)      299 2022-02-16 04:25:56.000000 tapr-0.2.1/tapr/visualization/plotly/offline.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)      300 2022-02-16 04:25:56.000000 tapr-0.2.1/tapr/visualization/plotly/subplots.py
-drwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)        0 2022-07-13 01:23:21.662351 tapr-0.2.1/tapr.egg-info/
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)     1536 2022-07-13 01:23:21.000000 tapr-0.2.1/tapr.egg-info/PKG-INFO
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)     1380 2022-07-13 01:23:21.000000 tapr-0.2.1/tapr.egg-info/SOURCES.txt
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)        1 2022-07-13 01:23:21.000000 tapr-0.2.1/tapr.egg-info/dependency_links.txt
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)       43 2022-07-13 01:23:21.000000 tapr-0.2.1/tapr.egg-info/requires.txt
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)       11 2022-07-13 01:23:21.000000 tapr-0.2.1/tapr.egg-info/top_level.txt
-drwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)        0 2022-07-13 01:23:21.670351 tapr-0.2.1/tests/
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)        0 2022-01-21 05:43:08.000000 tapr-0.2.1/tests/__init__.py
-drwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)        0 2022-07-13 01:23:21.670351 tapr-0.2.1/tests/io/
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)        0 2022-01-21 05:43:08.000000 tapr-0.2.1/tests/io/__init__.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)     1811 2022-01-21 05:43:08.000000 tapr-0.2.1/tests/io/test_ntableio.py
-drwxrwxr-x   0 spacedoge  (1001) spacedoge  (1001)        0 2022-07-13 01:23:21.670351 tapr-0.2.1/tests/main/
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)        0 2022-01-21 05:43:08.000000 tapr-0.2.1/tests/main/__init__.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)     1146 2022-01-21 05:43:08.000000 tapr-0.2.1/tests/main/test_alchemy.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)     4325 2022-01-21 05:43:08.000000 tapr-0.2.1/tests/main/test_conversion.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)     2693 2022-07-13 00:35:59.000000 tapr-0.2.1/tests/main/test_engines.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)        0 2022-01-21 05:43:08.000000 tapr-0.2.1/tests/main/test_filtering.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)        0 2022-01-21 05:43:08.000000 tapr-0.2.1/tests/main/test_handling.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)    15490 2022-07-13 00:53:29.000000 tapr-0.2.1/tests/main/test_ntable.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)     3205 2022-01-21 05:43:08.000000 tapr-0.2.1/tests/main/test_processing.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)     1130 2022-07-13 00:44:13.000000 tapr-0.2.1/tests/main/test_qol.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)     2669 2022-01-21 05:43:08.000000 tapr-0.2.1/tests/main/test_structure.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)     1732 2022-02-16 04:06:38.000000 tapr-0.2.1/tests/main/test_tabularization.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)    55124 2022-07-13 01:14:36.000000 tapr-0.2.1/tests/main/test_utils.py
--rw-rw-r--   0 spacedoge  (1001) spacedoge  (1001)      770 2022-01-21 05:43:08.000000 tapr-0.2.1/tests/testing_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:04:09.749797 tapr-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-30 01:03:55.000000 tapr-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-30 01:04:09.749797 tapr-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-30 01:03:55.000000 tapr-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-30 01:03:55.000000 tapr-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 01:04:09.749797 tapr-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:04:09.745797 tapr-0.3.0/tapr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:04:09.745797 tapr-0.3.0/tapr/io_/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/io_/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3782 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/io_/ntableio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/io_/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:04:09.749797 tapr-0.3.0/tapr/main/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2177 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/alchemy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7109 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      452 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/defs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1899 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/engines.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      892 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/filtering.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1626 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/ntable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2250 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/qol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7750 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/structure.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2063 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/tabularization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      186 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/ttypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:04:09.749797 tapr-0.3.0/tapr/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:04:09.749797 tapr-0.3.0/tapr/visualization/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/visualization/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/visualization/matplotlib/pyplot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:04:09.749797 tapr-0.3.0/tapr/visualization/plotly/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/visualization/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/visualization/plotly/express.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/visualization/plotly/graph_objs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/visualization/plotly/offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/visualization/plotly/subplots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:04:09.745797 tapr-0.3.0/tapr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-30 01:04:09.000000 tapr-0.3.0/tapr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-30 01:04:09.000000 tapr-0.3.0/tapr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 01:04:09.000000 tapr-0.3.0/tapr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-30 01:04:09.000000 tapr-0.3.0/tapr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 01:04:09.000000 tapr-0.3.0/tapr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:04:09.749797 tapr-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-30 01:03:55.000000 tapr-0.3.0/tests/testing_utils.py
```

### Comparing `tapr-0.2.1/LICENSE` & `tapr-0.3.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 elspacedoge (https://bitbucket.org/elspacedoge/)
+Copyright (c) 2023 thecodedog (https://github.com/thecodedog)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `tapr-0.2.1/README.md` & `tapr-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tapr-0.2.1/tapr/__init__.py` & `tapr-0.3.0/tapr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 processing = il.import_module(".main.processing", package=__name__)
 qol = il.import_module(".main.qol", package=__name__)
 structure = il.import_module(".main.structure", package=__name__)
 tabularization = il.import_module(".main.tabularization", package=__name__)
 ttypes = il.import_module(".main.ttypes", package=__name__)
 utils = il.import_module(".main.utils", package=__name__)
 
-io = il.import_module(".io", package=__name__)
+io = il.import_module(".io_", package=__name__)
 
 from .main.conversion import ntable
 from .main.qol import blank, sblank, cartograph, count
 from .main.tabularization import tabularize
 from .main.utils import full, full_lite, full_like, concatenate_ntables as concatenate
 
-from .io.ntableio import save_ntable, load_ntable
+from .io_.ntableio import save_ntable, load_ntable
 
 _px = il.import_module(".visualization.plotly.express", package=__name__)
 # look for any tabularized plotly express functions and expose them here
 for name in dir(_px):
     value = getattr(_px,name)
     if isinstance(value, tabularization._Tabularized):
         globals()[name] = value
```

### Comparing `tapr-0.2.1/tapr/io/ntableio.py` & `tapr-0.3.0/tapr/io_/ntableio.py`

 * *Files identical despite different names*

### Comparing `tapr-0.2.1/tapr/io/serialization.py` & `tapr-0.3.0/tapr/io_/serialization.py`

 * *Files identical despite different names*

### Comparing `tapr-0.2.1/tapr/main/alchemy.py` & `tapr-0.3.0/tapr/main/alchemy.py`

 * *Files identical despite different names*

### Comparing `tapr-0.2.1/tapr/main/conversion.py` & `tapr-0.3.0/tapr/main/conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         if dims is None:
             dims = ("rows",)
         coords = {dims[0]: list(pds.index)}
     refmap = basic_refmap(coords, dims)
     return NTable(reflist, refmap, engine=engine, ttype=ttype)
 
 
-def ntable(obj, dims=None, engine=None, ttype=None):
+def ntable(obj, dims=None, engine=None, ttype=None, coords=None, shape=None):
     """
     Parameters
     ----------
     obj : Mapping, xr.DataArray, pd.DataFrame, NTable or container of NTable objects
         The object to create a NTable object from.
     dims : Sequence, optional
         The desired dimension names. If None, dim names will be dim0, dim1,
@@ -221,12 +221,20 @@
         return ntbl
     if isinstance(obj, pd.DataFrame) or isinstance(obj, pd.Series):
         ntbl = _pandas_to_ntable(obj, dims, engine=engine, ttype=ttype)
         return ntbl
     if isinstance(obj, NTable):
         ntbl = NTable(obj.reflist, obj.refmap, engine=engine, ttype=ttype)
         return ntbl
+
     try:
-        ntbl = tabulate(obj)
-        return ntbl
+        dlist = list(obj)
+        if coords is not None and dims is not None:
+            dmap  = basic_refmap(coords, dims)
+        elif shape is not None:
+            dmap = default_refmap(*shape)
+        else:
+            dmap = default_refmap(len(dlist))
+        return NTable(dlist, dmap, engine=engine, ttype=ttype)
+
     except TypeError:
         raise TypeError(f"Unable to convert {type(obj)} to NTable")
```

### Comparing `tapr-0.2.1/tapr/main/engines.py` & `tapr-0.3.0/tapr/main/engines.py`

 * *Files identical despite different names*

### Comparing `tapr-0.2.1/tapr/main/filtering.py` & `tapr-0.3.0/tapr/main/filtering.py`

 * *Files identical despite different names*

### Comparing `tapr-0.2.1/tapr/main/handling.py` & `tapr-0.3.0/tapr/main/handling.py`

 * *Files identical despite different names*

### Comparing `tapr-0.2.1/tapr/main/ntable.py` & `tapr-0.3.0/tapr/main/ntable.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from collections.abc import MutableMapping
 import itertools as it
 import operator as op
 
 import numpy as np
 import xarray as xr
 
@@ -67,35 +68,41 @@
         return NTableMapAlchemy(self)
 
     def __dir__(self):
         result = list(self.__dict__)
         result.extend(list(self.keys()))
         return result
 
-    # def _ipython_key_completions_(self, incomplete_key):
-    #     if not isinstance(incomplete_key, str):
-    #         return []
-    #     coords_dict = xarray_coords_to_dict(self._ntable.struct.coords)
-    #     dim_coords = coords_dict[self._dim]
-    #     result = []
-    #     for coord in dim_coords:
-    #         if isinstance(coord, str):
-    #             if coord.startswith(incomplete_key):
-    #                 result.append(coord)
-    #
-    #     return [coord for coord in dim_coords if coord.startswith(incomplete_key)]
+    def _ipython_key_completions_(self, incomplete_key):
+        if not isinstance(incomplete_key, str):
+            return []
+        return [coord for coord in self if (isinstance(coord, str) and coord.startswith(incomplete_key))]
 
     def __getattr__(self, attr):
         try:
             return self[attr]
         except KeyError:
             raise AttributeError(f"{attr} is not an attribute of NTable")
 
     def __str__(self):
-        return str(dict(**self))
+        keylist = list(self)
+        result = "{\n    "
+        if len(self) > 6:
+            topkeys = keylist[0:2]
+            botkeys = keylist[-2:]
+            for key in topkeys:
+                result += f"\n{key}:\n{self[key]}\n"
+            result += "\n.\n.\n.\n\n"
+            for key in botkeys:
+                result += f"\n{key}:\n{self[key]}\n"
+        else:
+            for key in keylist:
+                result += f"\n{key}:\n{self[key]}\n"
+        result = result.replace("\n", "\n    ")
+        return result + "\n}"
 
     def __repr__(self):
         return str(self)
 
     def __getitem__(self, key):
         return self._ntable.struct.loc[{self._dim: key}]
 
@@ -334,17 +341,18 @@
     @property
     def alchemy(self):
         """An object used for special types of lookups/operations."""
         return NTableAlchemy(self)
 
     def __dir__(self):
         result = list(self.__dict__)
+        result.extend(list(NTable.__dict__))
         result.extend(self.struct.dims)
         result.extend(ttype_to_attrs(self.ttype))
-        return result
+        return [item for item in result if not re.match(r"_|__.*", item)]
 
     def __getattr__(self, attr):
         try:
             return self.ntable_map(attr)
         except ValueError:
             attr_dict = ttype_to_attrs(self._ttype)
             if attr in attr_dict:
@@ -417,15 +425,15 @@
         """
         if dim not in self.struct.dims:
             raise ValueError(f"{dim} dimension does not exist")
         return NTableMap(self, dim)
 
     def to_dictionary(self, into=None, enforce_nested_typing=True):
         """
-        Convert a NTable object into a dictionary
+        Convert an NTable object into a dictionary
 
         Parameters
         ----------
         into : MutableMapping, optional
             A dictionary-like object to store elements into. If None,
             a new dictionary is created and returned.
 
@@ -455,15 +463,15 @@
             else:
                 into[k] = v
 
         return into
 
     def to_pandas(self, dtype="object"):
         """
-        Convert a NTable object into a Pandas object
+        Convert an NTable object into a Pandas object
         (Series or DataFrame depending on the shape of the NTable object.)
 
         Parameters
         ----------
         dtype : str, np.dtype, optional
             Data type that the resulting Pandas object should be.
             The default is "object".
@@ -484,15 +492,15 @@
         else:
             raise ValueError(
                 f"Unable to convert {self.struct.ndim} dimensional NTable to pandas object"
             )
 
     def to_data_array(self, dtype="object"):
         """
-        Convert a NTable object into a DataArray
+        Convert an NTable object into a DataArray
 
         Parameters
         ----------
         dtype : str, np.dtype, optional
             Data type that the resulting DataArray should be.
             The default is "object".
```

### Comparing `tapr-0.2.1/tapr/main/processing.py` & `tapr-0.3.0/tapr/main/processing.py`

 * *Files identical despite different names*

### Comparing `tapr-0.2.1/tapr/main/qol.py` & `tapr-0.3.0/tapr/main/qol.py`

 * *Files identical despite different names*

### Comparing `tapr-0.2.1/tapr/main/structure.py` & `tapr-0.3.0/tapr/main/structure.py`

 * *Files identical despite different names*

### Comparing `tapr-0.2.1/tapr/main/tabularization.py` & `tapr-0.3.0/tapr/main/tabularization.py`

 * *Files identical despite different names*

### Comparing `tapr-0.2.1/tapr/main/utils.py` & `tapr-0.3.0/tapr/main/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         if len(ntbl.struct.coords[dims[0]]) > max_rows:
             reduce_index[dims[0]] = np.r_[0:50, -50:0]
     except IndexError:
         pass
 
     try:
         if len(ntbl.struct.coords[dims[1]]) > max_cols:
-            reduce_index[dims[0]] = np.r_[0:10, -10:0]
+            reduce_index[dims[1]] = np.r_[0:10, -10:0]
     except IndexError:
         pass
 
     print_ellipsises = {}
 
     for dim in dims[2:]:
         if len(ntbl.struct.coords[dim]) > max_other:
@@ -185,15 +185,15 @@
             if (i == 4) and (print_ellipsises[dim]):
                 string += f". . .\n\n{sep}\n\n"
 
     elif ntbl.struct.ndim == 0:
         string = str(ntbl.struct.item())
     else:
         string = str(ntbl.to_pandas())
-        string = "\n".join(string.split("\n")[0:-1])
+        string = "\n".join(string.split("\n"))
     return string
 
 
 def any_ntables(iterable):
     from .ntable import NTable
 
     return any(isinstance(item, NTable) for item in iterable)
@@ -221,40 +221,14 @@
         if cls not in cls._instances:
             cls._instances[cls] = super(_Singleton, cls).__call__(
                 *args, **kwargs
             )
         return cls._instances[cls]
 
 
-# class SUPREMUM(metaclass=_Singleton):
-#     def __gt__(self, other):
-#         return True
-#
-#     def __ge__(self, other):
-#         return True
-#
-#     def __lt__(self, other):
-#         return False
-#
-#     def __le__(self, other):
-#         return False
-
-# class INFIMUM(metaclass=_Singleton):
-#     def __gt__(self, other):
-#         return False
-#
-#     def __ge__(self, other):
-#         return False
-#
-#     def __lt__(self, other):
-#         return True
-#
-#     def __le__(self, other):
-#         return True
-
 
 class NULL(np.lib.mixins.NDArrayOperatorsMixin, metaclass=_Singleton):
     def __str__(self):
         return "NULL"
 
     def __repr__(self):
         return "NULL"
@@ -345,26 +319,14 @@
         coords[dim] = [f"{dim}{i}" for i in range(size)]
 
     refarray = np.arange(np.prod(shape)).reshape(shape)
     refmap = xr.DataArray(refarray, coords, dims)
     return refmap
 
 
-# class _Shell:
-#     def __init__(self, obj):
-#         self._obj = obj
-#
-#     def __TAPR_PEEL__(self):
-#         return self._obj
-#
-#
-# def shell(obj, layers=1):
-#     return _Shell(obj)
-
-
 def expand(iterable):
     result = []
     for item in iterable:
         try:
             result.append(expand(item))
         except TypeError:
             result.append(item)
```

### Comparing `tapr-0.2.1/tests/testing_utils.py` & `tapr-0.3.0/tests/testing_utils.py`

 * *Files identical despite different names*

