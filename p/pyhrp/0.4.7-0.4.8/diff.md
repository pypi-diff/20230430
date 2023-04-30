# Comparing `tmp/pyhrp-0.4.7.tar.gz` & `tmp/pyhrp-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhrp-0.4.7.tar", max compression
+gzip compressed data, was "pyhrp-0.4.8.tar", max compression
```

## Comparing `pyhrp-0.4.7.tar` & `pyhrp-0.4.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1083 2023-04-30 02:42:16.962304 pyhrp-0.4.7/LICENSE.txt
--rw-r--r--   0        0        0     1515 2023-04-30 02:42:16.962304 pyhrp-0.4.7/README.md
--rwxr-xr-x   0        0        0        0 2023-04-30 02:42:16.962304 pyhrp-0.4.7/pyhrp/__init__.py
--rw-r--r--   0        0        0     3047 2023-04-30 02:42:16.962304 pyhrp-0.4.7/pyhrp/cluster.py
--rw-r--r--   0        0        0      309 2023-04-30 02:42:16.962304 pyhrp-0.4.7/pyhrp/graph.py
--rw-r--r--   0        0        0     2559 2023-04-30 02:42:16.962304 pyhrp-0.4.7/pyhrp/hrp.py
--rw-r--r--   0        0        0     2250 2023-04-30 02:42:16.962304 pyhrp-0.4.7/pyhrp/marcos.py
--rw-r--r--   0        0        0      479 2023-04-30 02:42:44.442068 pyhrp-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 pyhrp-0.4.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1083 2023-04-30 02:45:58.829421 pyhrp-0.4.8/LICENSE.txt
+-rw-r--r--   0        0        0     1515 2023-04-30 02:45:58.829421 pyhrp-0.4.8/README.md
+-rwxr-xr-x   0        0        0        0 2023-04-30 02:45:58.829421 pyhrp-0.4.8/pyhrp/__init__.py
+-rw-r--r--   0        0        0     3047 2023-04-30 02:45:58.829421 pyhrp-0.4.8/pyhrp/cluster.py
+-rw-r--r--   0        0        0      309 2023-04-30 02:45:58.829421 pyhrp-0.4.8/pyhrp/graph.py
+-rw-r--r--   0        0        0     2559 2023-04-30 02:45:58.829421 pyhrp-0.4.8/pyhrp/hrp.py
+-rw-r--r--   0        0        0     2250 2023-04-30 02:45:58.829421 pyhrp-0.4.8/pyhrp/marcos.py
+-rw-r--r--   0        0        0      479 2023-04-30 02:46:19.441474 pyhrp-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 pyhrp-0.4.8/PKG-INFO
```

### Comparing `pyhrp-0.4.7/LICENSE.txt` & `pyhrp-0.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyhrp-0.4.7/README.md` & `pyhrp-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `pyhrp-0.4.7/pyhrp/cluster.py` & `pyhrp-0.4.8/pyhrp/cluster.py`

 * *Files identical despite different names*

### Comparing `pyhrp-0.4.7/pyhrp/hrp.py` & `pyhrp-0.4.8/pyhrp/hrp.py`

 * *Files identical despite different names*

### Comparing `pyhrp-0.4.7/pyhrp/marcos.py` & `pyhrp-0.4.8/pyhrp/marcos.py`

 * *Files identical despite different names*

### Comparing `pyhrp-0.4.7/PKG-INFO` & `pyhrp-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhrp
-Version: 0.4.7
+Version: 0.4.8
 Summary: ...
 Home-page: https://github.com/tschm/pyhrp
 Author: Thomas Schmelzer
 Requires-Python: >=3.9.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

