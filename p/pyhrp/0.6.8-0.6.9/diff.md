# Comparing `tmp/pyhrp-0.6.8.tar.gz` & `tmp/pyhrp-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhrp-0.6.8.tar", max compression
+gzip compressed data, was "pyhrp-0.6.9.tar", max compression
```

## Comparing `pyhrp-0.6.8.tar` & `pyhrp-0.6.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1083 2023-04-30 05:48:49.867034 pyhrp-0.6.8/LICENSE.txt
--rw-r--r--   0        0        0     1515 2023-04-30 05:48:49.867034 pyhrp-0.6.8/README.md
--rwxr-xr-x   0        0        0        0 2023-04-30 05:48:49.867034 pyhrp-0.6.8/pyhrp/__init__.py
--rw-r--r--   0        0        0     3047 2023-04-30 05:48:49.867034 pyhrp-0.6.8/pyhrp/cluster.py
--rw-r--r--   0        0        0      309 2023-04-30 05:48:49.867034 pyhrp-0.6.8/pyhrp/graph.py
--rw-r--r--   0        0        0     2559 2023-04-30 05:48:49.867034 pyhrp-0.6.8/pyhrp/hrp.py
--rw-r--r--   0        0        0     2250 2023-04-30 05:48:49.867034 pyhrp-0.6.8/pyhrp/marcos.py
--rw-r--r--   0        0        0      479 2023-04-30 05:49:09.667155 pyhrp-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 pyhrp-0.6.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1083 2023-04-30 13:18:13.179205 pyhrp-0.6.9/LICENSE.txt
+-rw-r--r--   0        0        0     1515 2023-04-30 13:18:13.179205 pyhrp-0.6.9/README.md
+-rwxr-xr-x   0        0        0        0 2023-04-30 13:18:13.179205 pyhrp-0.6.9/pyhrp/__init__.py
+-rw-r--r--   0        0        0     3047 2023-04-30 13:18:13.179205 pyhrp-0.6.9/pyhrp/cluster.py
+-rw-r--r--   0        0        0      309 2023-04-30 13:18:13.179205 pyhrp-0.6.9/pyhrp/graph.py
+-rw-r--r--   0        0        0     2559 2023-04-30 13:18:13.179205 pyhrp-0.6.9/pyhrp/hrp.py
+-rw-r--r--   0        0        0     2250 2023-04-30 13:18:13.179205 pyhrp-0.6.9/pyhrp/marcos.py
+-rw-r--r--   0        0        0      479 2023-04-30 13:18:37.759745 pyhrp-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 pyhrp-0.6.9/PKG-INFO
```

### Comparing `pyhrp-0.6.8/LICENSE.txt` & `pyhrp-0.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyhrp-0.6.8/README.md` & `pyhrp-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `pyhrp-0.6.8/pyhrp/cluster.py` & `pyhrp-0.6.9/pyhrp/cluster.py`

 * *Files identical despite different names*

### Comparing `pyhrp-0.6.8/pyhrp/hrp.py` & `pyhrp-0.6.9/pyhrp/hrp.py`

 * *Files identical despite different names*

### Comparing `pyhrp-0.6.8/pyhrp/marcos.py` & `pyhrp-0.6.9/pyhrp/marcos.py`

 * *Files identical despite different names*

### Comparing `pyhrp-0.6.8/PKG-INFO` & `pyhrp-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhrp
-Version: 0.6.8
+Version: 0.6.9
 Summary: ...
 Home-page: https://github.com/tschm/pyhrp
 Author: Thomas Schmelzer
 Requires-Python: >=3.9.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

