# Comparing `tmp/yatracker_linker-0.3.1.tar.gz` & `tmp/yatracker_linker-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yatracker_linker-0.3.1.tar", max compression
+gzip compressed data, was "yatracker_linker-0.3.2.tar", max compression
```

## Comparing `yatracker_linker-0.3.1.tar` & `yatracker_linker-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-04-30 06:30:56.274815 yatracker_linker-0.3.1/LICENSE
--rw-r--r--   0        0        0      111 2023-04-30 06:30:56.278816 yatracker_linker-0.3.1/README.rst
--rw-r--r--   0        0        0     1051 2023-04-30 06:31:30.255226 yatracker_linker-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-30 06:30:56.278816 yatracker_linker-0.3.1/yatracker_linker/__init__.py
--rw-r--r--   0        0        0     1236 2023-04-30 06:30:56.278816 yatracker_linker-0.3.1/yatracker_linker/__main__.py
--rw-r--r--   0        0        0      825 2023-04-30 06:30:56.278816 yatracker_linker-0.3.1/yatracker_linker/args.py
--rw-r--r--   0        0        0      621 2023-04-30 06:30:56.278816 yatracker_linker-0.3.1/yatracker_linker/deps.py
--rw-r--r--   0        0        0      621 2023-04-30 06:30:56.278816 yatracker_linker-0.3.1/yatracker_linker/service.py
--rw-r--r--   0        0        0      857 2023-04-30 06:30:56.278816 yatracker_linker-0.3.1/yatracker_linker/tracker_client.py
--rw-r--r--   0        0        0        0 2023-04-30 06:30:56.278816 yatracker_linker-0.3.1/yatracker_linker/views/__init__.py
--rw-r--r--   0        0        0      444 2023-04-30 06:30:56.278816 yatracker_linker-0.3.1/yatracker_linker/views/base.py
--rw-r--r--   0        0        0     3307 2023-04-30 06:30:56.278816 yatracker_linker-0.3.1/yatracker_linker/views/events.py
--rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 yatracker_linker-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-30 08:12:38.996625 yatracker_linker-0.3.2/LICENSE
+-rw-r--r--   0        0        0      111 2023-04-30 08:12:38.996625 yatracker_linker-0.3.2/README.rst
+-rw-r--r--   0        0        0     1051 2023-04-30 08:13:07.888745 yatracker_linker-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-30 08:12:38.996625 yatracker_linker-0.3.2/yatracker_linker/__init__.py
+-rw-r--r--   0        0        0     1236 2023-04-30 08:12:38.996625 yatracker_linker-0.3.2/yatracker_linker/__main__.py
+-rw-r--r--   0        0        0      825 2023-04-30 08:12:38.996625 yatracker_linker-0.3.2/yatracker_linker/args.py
+-rw-r--r--   0        0        0      621 2023-04-30 08:12:38.996625 yatracker_linker-0.3.2/yatracker_linker/deps.py
+-rw-r--r--   0        0        0      621 2023-04-30 08:12:38.996625 yatracker_linker-0.3.2/yatracker_linker/service.py
+-rw-r--r--   0        0        0      865 2023-04-30 08:12:38.996625 yatracker_linker-0.3.2/yatracker_linker/tracker_client.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:12:38.996625 yatracker_linker-0.3.2/yatracker_linker/utils.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:12:38.996625 yatracker_linker-0.3.2/yatracker_linker/views/__init__.py
+-rw-r--r--   0        0        0      444 2023-04-30 08:12:38.996625 yatracker_linker-0.3.2/yatracker_linker/views/base.py
+-rw-r--r--   0        0        0     4775 2023-04-30 08:12:38.996625 yatracker_linker-0.3.2/yatracker_linker/views/events.py
+-rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 yatracker_linker-0.3.2/PKG-INFO
```

### Comparing `yatracker_linker-0.3.1/LICENSE` & `yatracker_linker-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.1/pyproject.toml` & `yatracker_linker-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yatracker-linker"
-version = "0.3.1"
+version = "0.3.2"
 description = "Yandex Tracker issues integration"
 license = "MIT"
 authors = ["Alexander Vasin <hi@alvass.in>"]
 readme = "README.rst"
 packages = [{include = "yatracker_linker"}]
 
 [tool.poetry.scripts]
```

### Comparing `yatracker_linker-0.3.1/yatracker_linker/__main__.py` & `yatracker_linker-0.3.2/yatracker_linker/__main__.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.1/yatracker_linker/args.py` & `yatracker_linker-0.3.2/yatracker_linker/args.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.1/yatracker_linker/deps.py` & `yatracker_linker-0.3.2/yatracker_linker/deps.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.1/yatracker_linker/service.py` & `yatracker_linker-0.3.2/yatracker_linker/service.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.1/PKG-INFO` & `yatracker_linker-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yatracker-linker
-Version: 0.3.1
+Version: 0.3.2
 Summary: Yandex Tracker issues integration
 License: MIT
 Author: Alexander Vasin
 Author-email: hi@alvass.in
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

