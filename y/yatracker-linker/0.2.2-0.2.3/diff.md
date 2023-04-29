# Comparing `tmp/yatracker_linker-0.2.2.tar.gz` & `tmp/yatracker_linker-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yatracker_linker-0.2.2.tar", max compression
+gzip compressed data, was "yatracker_linker-0.2.3.tar", max compression
```

## Comparing `yatracker_linker-0.2.2.tar` & `yatracker_linker-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2023-04-29 23:46:06.518482 yatracker_linker-0.2.2/LICENSE
--rw-r--r--   0        0        0      111 2023-04-29 23:46:06.518482 yatracker_linker-0.2.2/README.rst
--rw-r--r--   0        0        0     1051 2023-04-29 23:46:28.982818 yatracker_linker-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-29 23:46:06.518482 yatracker_linker-0.2.2/yatracker_linker/__init__.py
--rw-r--r--   0        0        0     1236 2023-04-29 23:46:06.518482 yatracker_linker-0.2.2/yatracker_linker/__main__.py
--rw-r--r--   0        0        0      825 2023-04-29 23:46:06.518482 yatracker_linker-0.2.2/yatracker_linker/args.py
--rw-r--r--   0        0        0      606 2023-04-29 23:46:06.518482 yatracker_linker-0.2.2/yatracker_linker/deps.py
--rw-r--r--   0        0        0      606 2023-04-29 23:46:06.518482 yatracker_linker-0.2.2/yatracker_linker/service.py
--rw-r--r--   0        0        0      852 2023-04-29 23:46:06.518482 yatracker_linker-0.2.2/yatracker_linker/st_client.py
--rw-r--r--   0        0        0        0 2023-04-29 23:46:06.518482 yatracker_linker-0.2.2/yatracker_linker/views/__init__.py
--rw-r--r--   0        0        0      429 2023-04-29 23:46:06.518482 yatracker_linker-0.2.2/yatracker_linker/views/base.py
--rw-r--r--   0        0        0     3248 2023-04-29 23:46:06.518482 yatracker_linker-0.2.2/yatracker_linker/views/events.py
--rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 yatracker_linker-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-29 23:47:16.459555 yatracker_linker-0.2.3/LICENSE
+-rw-r--r--   0        0        0      111 2023-04-29 23:47:16.459555 yatracker_linker-0.2.3/README.rst
+-rw-r--r--   0        0        0     1051 2023-04-29 23:47:43.239889 yatracker_linker-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-29 23:47:16.459555 yatracker_linker-0.2.3/yatracker_linker/__init__.py
+-rw-r--r--   0        0        0     1236 2023-04-29 23:47:16.459555 yatracker_linker-0.2.3/yatracker_linker/__main__.py
+-rw-r--r--   0        0        0      825 2023-04-29 23:47:16.459555 yatracker_linker-0.2.3/yatracker_linker/args.py
+-rw-r--r--   0        0        0      606 2023-04-29 23:47:16.459555 yatracker_linker-0.2.3/yatracker_linker/deps.py
+-rw-r--r--   0        0        0      606 2023-04-29 23:47:16.459555 yatracker_linker-0.2.3/yatracker_linker/service.py
+-rw-r--r--   0        0        0      852 2023-04-29 23:47:16.459555 yatracker_linker-0.2.3/yatracker_linker/st_client.py
+-rw-r--r--   0        0        0        0 2023-04-29 23:47:16.459555 yatracker_linker-0.2.3/yatracker_linker/views/__init__.py
+-rw-r--r--   0        0        0      429 2023-04-29 23:47:16.459555 yatracker_linker-0.2.3/yatracker_linker/views/base.py
+-rw-r--r--   0        0        0     3248 2023-04-29 23:47:16.459555 yatracker_linker-0.2.3/yatracker_linker/views/events.py
+-rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 yatracker_linker-0.2.3/PKG-INFO
```

### Comparing `yatracker_linker-0.2.2/LICENSE` & `yatracker_linker-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.2.2/pyproject.toml` & `yatracker_linker-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yatracker-linker"
-version = "0.2.2"
+version = "0.2.3"
 description = "Yandex Tracker issues integration"
 license = "MIT"
 authors = ["Alexander Vasin <hi@alvass.in>"]
 readme = "README.rst"
 packages = [{include = "yatracker_linker"}]
 
 [tool.poetry.scripts]
```

### Comparing `yatracker_linker-0.2.2/yatracker_linker/__main__.py` & `yatracker_linker-0.2.3/yatracker_linker/__main__.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.2.2/yatracker_linker/args.py` & `yatracker_linker-0.2.3/yatracker_linker/args.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.2.2/yatracker_linker/deps.py` & `yatracker_linker-0.2.3/yatracker_linker/deps.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.2.2/yatracker_linker/service.py` & `yatracker_linker-0.2.3/yatracker_linker/service.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.2.2/yatracker_linker/st_client.py` & `yatracker_linker-0.2.3/yatracker_linker/st_client.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.2.2/yatracker_linker/views/events.py` & `yatracker_linker-0.2.3/yatracker_linker/views/events.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.2.2/PKG-INFO` & `yatracker_linker-0.2.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yatracker-linker
-Version: 0.2.2
+Version: 0.2.3
 Summary: Yandex Tracker issues integration
 License: MIT
 Author: Alexander Vasin
 Author-email: hi@alvass.in
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

