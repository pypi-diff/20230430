# Comparing `tmp/pyhrp-0.6.4.tar.gz` & `tmp/pyhrp-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhrp-0.6.4.tar", max compression
+gzip compressed data, was "pyhrp-0.6.5.tar", max compression
```

## Comparing `pyhrp-0.6.4.tar` & `pyhrp-0.6.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1083 2023-04-30 05:00:52.619491 pyhrp-0.6.4/LICENSE.txt
--rw-r--r--   0        0        0     1515 2023-04-30 05:00:52.619491 pyhrp-0.6.4/README.md
--rwxr-xr-x   0        0        0        0 2023-04-30 05:00:52.619491 pyhrp-0.6.4/pyhrp/__init__.py
--rw-r--r--   0        0        0     3047 2023-04-30 05:00:52.619491 pyhrp-0.6.4/pyhrp/cluster.py
--rw-r--r--   0        0        0      309 2023-04-30 05:00:52.619491 pyhrp-0.6.4/pyhrp/graph.py
--rw-r--r--   0        0        0     2559 2023-04-30 05:00:52.619491 pyhrp-0.6.4/pyhrp/hrp.py
--rw-r--r--   0        0        0     2250 2023-04-30 05:00:52.619491 pyhrp-0.6.4/pyhrp/marcos.py
--rw-r--r--   0        0        0      479 2023-04-30 05:01:12.179659 pyhrp-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 pyhrp-0.6.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1083 2023-04-30 05:07:48.641823 pyhrp-0.6.5/LICENSE.txt
+-rw-r--r--   0        0        0     1515 2023-04-30 05:07:48.641823 pyhrp-0.6.5/README.md
+-rwxr-xr-x   0        0        0        0 2023-04-30 05:07:48.641823 pyhrp-0.6.5/pyhrp/__init__.py
+-rw-r--r--   0        0        0     3047 2023-04-30 05:07:48.641823 pyhrp-0.6.5/pyhrp/cluster.py
+-rw-r--r--   0        0        0      309 2023-04-30 05:07:48.641823 pyhrp-0.6.5/pyhrp/graph.py
+-rw-r--r--   0        0        0     2559 2023-04-30 05:07:48.641823 pyhrp-0.6.5/pyhrp/hrp.py
+-rw-r--r--   0        0        0     2250 2023-04-30 05:07:48.641823 pyhrp-0.6.5/pyhrp/marcos.py
+-rw-r--r--   0        0        0      479 2023-04-30 05:08:08.937996 pyhrp-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 pyhrp-0.6.5/PKG-INFO
```

### Comparing `pyhrp-0.6.4/LICENSE.txt` & `pyhrp-0.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyhrp-0.6.4/README.md` & `pyhrp-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `pyhrp-0.6.4/pyhrp/cluster.py` & `pyhrp-0.6.5/pyhrp/cluster.py`

 * *Files identical despite different names*

### Comparing `pyhrp-0.6.4/pyhrp/hrp.py` & `pyhrp-0.6.5/pyhrp/hrp.py`

 * *Files identical despite different names*

### Comparing `pyhrp-0.6.4/pyhrp/marcos.py` & `pyhrp-0.6.5/pyhrp/marcos.py`

 * *Files identical despite different names*

### Comparing `pyhrp-0.6.4/PKG-INFO` & `pyhrp-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhrp
-Version: 0.6.4
+Version: 0.6.5
 Summary: ...
 Home-page: https://github.com/tschm/pyhrp
 Author: Thomas Schmelzer
 Requires-Python: >=3.9.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

