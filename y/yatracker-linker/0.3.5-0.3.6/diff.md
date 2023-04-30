# Comparing `tmp/yatracker_linker-0.3.5.tar.gz` & `tmp/yatracker_linker-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yatracker_linker-0.3.5.tar", max compression
+gzip compressed data, was "yatracker_linker-0.3.6.tar", max compression
```

## Comparing `yatracker_linker-0.3.5.tar` & `yatracker_linker-0.3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-04-30 08:41:40.592194 yatracker_linker-0.3.5/LICENSE
--rw-r--r--   0        0        0      111 2023-04-30 08:41:40.592194 yatracker_linker-0.3.5/README.rst
--rw-r--r--   0        0        0     1051 2023-04-30 08:42:10.408424 yatracker_linker-0.3.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-30 08:41:40.592194 yatracker_linker-0.3.5/yatracker_linker/__init__.py
--rw-r--r--   0        0        0     1236 2023-04-30 08:41:40.592194 yatracker_linker-0.3.5/yatracker_linker/__main__.py
--rw-r--r--   0        0        0      825 2023-04-30 08:41:40.592194 yatracker_linker-0.3.5/yatracker_linker/args.py
--rw-r--r--   0        0        0      621 2023-04-30 08:41:40.596194 yatracker_linker-0.3.5/yatracker_linker/deps.py
--rw-r--r--   0        0        0      621 2023-04-30 08:41:40.596194 yatracker_linker-0.3.5/yatracker_linker/service.py
--rw-r--r--   0        0        0      865 2023-04-30 08:41:40.596194 yatracker_linker-0.3.5/yatracker_linker/tracker_client.py
--rw-r--r--   0        0        0        0 2023-04-30 08:41:40.596194 yatracker_linker-0.3.5/yatracker_linker/utils.py
--rw-r--r--   0        0        0        0 2023-04-30 08:41:40.596194 yatracker_linker-0.3.5/yatracker_linker/views/__init__.py
--rw-r--r--   0        0        0      444 2023-04-30 08:41:40.596194 yatracker_linker-0.3.5/yatracker_linker/views/base.py
--rw-r--r--   0        0        0     4775 2023-04-30 08:41:40.596194 yatracker_linker-0.3.5/yatracker_linker/views/events.py
--rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 yatracker_linker-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/LICENSE
+-rw-r--r--   0        0        0      111 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/README.rst
+-rw-r--r--   0        0        0     1051 2023-04-30 08:45:43.050813 yatracker_linker-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/__init__.py
+-rw-r--r--   0        0        0     1236 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/__main__.py
+-rw-r--r--   0        0        0      825 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/args.py
+-rw-r--r--   0        0        0      621 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/deps.py
+-rw-r--r--   0        0        0      621 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/service.py
+-rw-r--r--   0        0        0      865 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/tracker_client.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/utils.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/views/__init__.py
+-rw-r--r--   0        0        0      444 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/views/base.py
+-rw-r--r--   0        0        0     4775 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/views/events.py
+-rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 yatracker_linker-0.3.6/PKG-INFO
```

### Comparing `yatracker_linker-0.3.5/LICENSE` & `yatracker_linker-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.5/pyproject.toml` & `yatracker_linker-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yatracker-linker"
-version = "0.3.5"
+version = "0.3.6"
 description = "Yandex Tracker issues integration"
 license = "MIT"
 authors = ["Alexander Vasin <hi@alvass.in>"]
 readme = "README.rst"
 packages = [{include = "yatracker_linker"}]
 
 [tool.poetry.scripts]
```

### Comparing `yatracker_linker-0.3.5/yatracker_linker/__main__.py` & `yatracker_linker-0.3.6/yatracker_linker/__main__.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.5/yatracker_linker/args.py` & `yatracker_linker-0.3.6/yatracker_linker/args.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.5/yatracker_linker/deps.py` & `yatracker_linker-0.3.6/yatracker_linker/deps.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.5/yatracker_linker/service.py` & `yatracker_linker-0.3.6/yatracker_linker/service.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.5/yatracker_linker/tracker_client.py` & `yatracker_linker-0.3.6/yatracker_linker/tracker_client.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.5/yatracker_linker/views/events.py` & `yatracker_linker-0.3.6/yatracker_linker/views/events.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.5/PKG-INFO` & `yatracker_linker-0.3.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yatracker-linker
-Version: 0.3.5
+Version: 0.3.6
 Summary: Yandex Tracker issues integration
 License: MIT
 Author: Alexander Vasin
 Author-email: hi@alvass.in
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

