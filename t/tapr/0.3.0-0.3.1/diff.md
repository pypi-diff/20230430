# Comparing `tmp/tapr-0.3.0.tar.gz` & `tmp/tapr-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapr-0.3.0.tar", last modified: Sun Apr 30 01:04:09 2023, max compression
+gzip compressed data, was "tapr-0.3.1.tar", last modified: Sun Apr 30 03:00:35 2023, max compression
```

## Comparing `tapr-0.3.0.tar` & `tapr-0.3.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:04:09.749797 tapr-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-30 01:03:55.000000 tapr-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-30 01:04:09.749797 tapr-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-30 01:03:55.000000 tapr-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-30 01:03:55.000000 tapr-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 01:04:09.749797 tapr-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:04:09.745797 tapr-0.3.0/tapr/
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:04:09.745797 tapr-0.3.0/tapr/io_/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/io_/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3782 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/io_/ntableio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/io_/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:04:09.749797 tapr-0.3.0/tapr/main/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2177 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/alchemy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7109 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      452 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/defs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1899 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/engines.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      892 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/filtering.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1626 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/handling.py
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/ntable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2250 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/qol.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7750 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/structure.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2063 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/tabularization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      186 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/ttypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:04:09.749797 tapr-0.3.0/tapr/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:04:09.749797 tapr-0.3.0/tapr/visualization/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/visualization/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/visualization/matplotlib/pyplot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:04:09.749797 tapr-0.3.0/tapr/visualization/plotly/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/visualization/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/visualization/plotly/express.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/visualization/plotly/graph_objs.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/visualization/plotly/offline.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-30 01:03:55.000000 tapr-0.3.0/tapr/visualization/plotly/subplots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:04:09.745797 tapr-0.3.0/tapr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-30 01:04:09.000000 tapr-0.3.0/tapr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-30 01:04:09.000000 tapr-0.3.0/tapr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 01:04:09.000000 tapr-0.3.0/tapr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-30 01:04:09.000000 tapr-0.3.0/tapr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 01:04:09.000000 tapr-0.3.0/tapr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:04:09.749797 tapr-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-30 01:03:55.000000 tapr-0.3.0/tests/testing_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:00:35.748622 tapr-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-30 03:00:20.000000 tapr-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-30 03:00:35.748622 tapr-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-30 03:00:20.000000 tapr-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-30 03:00:20.000000 tapr-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 03:00:35.748622 tapr-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:00:35.744622 tapr-0.3.1/tapr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:00:35.744622 tapr-0.3.1/tapr/io_/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/io_/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3782 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/io_/ntableio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/io_/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:00:35.748622 tapr-0.3.1/tapr/main/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/main/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2177 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/main/alchemy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7109 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/main/conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      452 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/main/defs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1933 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/main/engines.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      892 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/main/filtering.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1626 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/main/handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/main/ntable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2250 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/main/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/main/qol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7750 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/main/structure.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2063 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/main/tabularization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      186 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/main/ttypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:00:35.748622 tapr-0.3.1/tapr/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:00:35.748622 tapr-0.3.1/tapr/visualization/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/visualization/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/visualization/matplotlib/pyplot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:00:35.748622 tapr-0.3.1/tapr/visualization/plotly/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/visualization/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/visualization/plotly/express.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/visualization/plotly/graph_objs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/visualization/plotly/offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-30 03:00:20.000000 tapr-0.3.1/tapr/visualization/plotly/subplots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:00:35.744622 tapr-0.3.1/tapr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-30 03:00:35.000000 tapr-0.3.1/tapr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-30 03:00:35.000000 tapr-0.3.1/tapr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 03:00:35.000000 tapr-0.3.1/tapr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-30 03:00:35.000000 tapr-0.3.1/tapr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 03:00:35.000000 tapr-0.3.1/tapr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:00:35.748622 tapr-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-30 03:00:20.000000 tapr-0.3.1/tests/testing_utils.py
```

### Comparing `tapr-0.3.0/LICENSE` & `tapr-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tapr-0.3.0/PKG-INFO` & `tapr-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapr
-Version: 0.3.0
+Version: 0.3.1
 Summary: TAbular PRogramming in Python
 Author-email: thecodedog <elcodedog@gmail.com>
 Project-URL: Homepage, https://github.com/thecodedog/tapr
 Project-URL: Bug Tracker, https://github.com/thecodedog/tapr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tapr-0.3.0/README.md` & `tapr-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tapr-0.3.0/pyproject.toml` & `tapr-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [project]
 name = "tapr"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="thecodedog", email="elcodedog@gmail.com" },
 ]
 description = "TAbular PRogramming in Python"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "dask==2023.4.0",
     "h5py==3.8.0",
     "numpy==1.24.3",
     "pandas==2.0.1",
     "plotly==5.14.1",
     "xarray==2023.4.2",
 ]
```

### Comparing `tapr-0.3.0/tapr/__init__.py` & `tapr-0.3.1/tapr/__init__.py`

 * *Files identical despite different names*

### Comparing `tapr-0.3.0/tapr/io_/ntableio.py` & `tapr-0.3.1/tapr/io_/ntableio.py`

 * *Files identical despite different names*

### Comparing `tapr-0.3.0/tapr/io_/serialization.py` & `tapr-0.3.1/tapr/io_/serialization.py`

 * *Files identical despite different names*

### Comparing `tapr-0.3.0/tapr/main/alchemy.py` & `tapr-0.3.1/tapr/main/alchemy.py`

 * *Files identical despite different names*

### Comparing `tapr-0.3.0/tapr/main/conversion.py` & `tapr-0.3.1/tapr/main/conversion.py`

 * *Files identical despite different names*

### Comparing `tapr-0.3.0/tapr/main/engines.py` & `tapr-0.3.1/tapr/main/engines.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from abc import ABC, abstractmethod
 from concurrent import futures as ft
-from dask.distributed import Client
+
+# from dask.distributed import Client
+
 
 class Engine(ABC):
     @abstractmethod
     def __tapr_engine_map__(self, func, *args):
         pass
 
+
 class ProcessEngine(Engine):
     def __init__(self, processes):
         self._processes = processes
 
     @property
     def processes(self):
         return self._processes
@@ -55,25 +58,25 @@
     def __str__(self):
         return "Standard (serial) Engine"
 
     def __repr__(self):
         return str(self)
 
 
-class DaskClientEngine(Engine):
-    def __init__(self, *client_args, **client_kwargs):
-        self._client = Client(*client_args, **client_kwargs)
+# class DaskClientEngine(Engine):
+#     def __init__(self, *client_args, **client_kwargs):
+#         self._client = Client(*client_args, **client_kwargs)
+
+#     @property
+#     def client(self):
+#         return self._client
+
+#     def __tapr_engine_map__(self, func, *args):
+#         args = [list(arg) for arg in args]
+#         futures = self._client.map(func, *args)
+#         return self._client.gather(futures)
 
-    @property
-    def client(self):
-        return self._client
+#     def __str__(self):
+#         return f"Dask Client Engine"
 
-    def __tapr_engine_map__(self, func, *args):
-        args = [list(arg) for arg in args]
-        futures = self._client.map(func, *args)
-        return self._client.gather(futures)
-
-    def __str__(self):
-        return f"Dask Client Engine"
-
-    def __repr__(self):
-        return str(self)
+#     def __repr__(self):
+#         return str(self)
```

### Comparing `tapr-0.3.0/tapr/main/filtering.py` & `tapr-0.3.1/tapr/main/filtering.py`

 * *Files identical despite different names*

### Comparing `tapr-0.3.0/tapr/main/handling.py` & `tapr-0.3.1/tapr/main/handling.py`

 * *Files identical despite different names*

### Comparing `tapr-0.3.0/tapr/main/ntable.py` & `tapr-0.3.1/tapr/main/ntable.py`

 * *Files identical despite different names*

### Comparing `tapr-0.3.0/tapr/main/processing.py` & `tapr-0.3.1/tapr/main/processing.py`

 * *Files identical despite different names*

### Comparing `tapr-0.3.0/tapr/main/qol.py` & `tapr-0.3.1/tapr/main/qol.py`

 * *Files identical despite different names*

### Comparing `tapr-0.3.0/tapr/main/structure.py` & `tapr-0.3.1/tapr/main/structure.py`

 * *Files identical despite different names*

### Comparing `tapr-0.3.0/tapr/main/tabularization.py` & `tapr-0.3.1/tapr/main/tabularization.py`

 * *Files identical despite different names*

### Comparing `tapr-0.3.0/tapr/main/utils.py` & `tapr-0.3.1/tapr/main/utils.py`

 * *Files identical despite different names*

### Comparing `tapr-0.3.0/tapr.egg-info/PKG-INFO` & `tapr-0.3.1/tapr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapr
-Version: 0.3.0
+Version: 0.3.1
 Summary: TAbular PRogramming in Python
 Author-email: thecodedog <elcodedog@gmail.com>
 Project-URL: Homepage, https://github.com/thecodedog/tapr
 Project-URL: Bug Tracker, https://github.com/thecodedog/tapr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tapr-0.3.0/tapr.egg-info/SOURCES.txt` & `tapr-0.3.1/tapr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tapr-0.3.0/tests/testing_utils.py` & `tapr-0.3.1/tests/testing_utils.py`

 * *Files identical despite different names*

