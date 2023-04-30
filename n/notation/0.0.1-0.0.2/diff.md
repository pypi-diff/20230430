# Comparing `tmp/notation-0.0.1.tar.gz` & `tmp/notation-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notation-0.0.1.tar", last modified: Sun Apr 30 17:32:00 2023, max compression
+gzip compressed data, was "notation-0.0.2.tar", last modified: Sun Apr 30 21:46:30 2023, max compression
```

## Comparing `notation-0.0.1.tar` & `notation-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 adpatter  (1000) adpatter  (1000)        0 2023-04-30 17:32:00.652947 notation-0.0.1/
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)     1081 2023-04-30 17:26:53.000000 notation-0.0.1/LICENSE
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)      575 2023-04-30 17:32:00.652947 notation-0.0.1/PKG-INFO
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)       17 2023-04-30 17:26:53.000000 notation-0.0.1/README.md
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)      630 2023-04-30 17:30:09.000000 notation-0.0.1/pyproject.toml
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)       38 2023-04-30 17:32:00.652947 notation-0.0.1/setup.cfg
-drwxrwxr-x   0 adpatter  (1000) adpatter  (1000)        0 2023-04-30 17:32:00.648947 notation-0.0.1/src/
-drwxrwxr-x   0 adpatter  (1000) adpatter  (1000)        0 2023-04-30 17:32:00.652947 notation-0.0.1/src/notation/
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)        0 2023-04-30 17:27:32.000000 notation-0.0.1/src/notation/__init__.py
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)      599 2023-04-30 17:28:05.000000 notation-0.0.1/src/notation/notation.py
-drwxrwxr-x   0 adpatter  (1000) adpatter  (1000)        0 2023-04-30 17:32:00.652947 notation-0.0.1/src/notation.egg-info/
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)      575 2023-04-30 17:32:00.000000 notation-0.0.1/src/notation.egg-info/PKG-INFO
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)      226 2023-04-30 17:32:00.000000 notation-0.0.1/src/notation.egg-info/SOURCES.txt
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)        1 2023-04-30 17:32:00.000000 notation-0.0.1/src/notation.egg-info/dependency_links.txt
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)        9 2023-04-30 17:32:00.000000 notation-0.0.1/src/notation.egg-info/top_level.txt
+drwxrwxr-x   0 adpatter  (1000) adpatter  (1000)        0 2023-04-30 21:46:30.220886 notation-0.0.2/
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)     1081 2023-04-30 17:26:53.000000 notation-0.0.2/LICENSE
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)      573 2023-04-30 21:46:30.220886 notation-0.0.2/PKG-INFO
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)       17 2023-04-30 17:26:53.000000 notation-0.0.2/README.md
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)      628 2023-04-30 21:44:53.000000 notation-0.0.2/pyproject.toml
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)       38 2023-04-30 21:46:30.220886 notation-0.0.2/setup.cfg
+drwxrwxr-x   0 adpatter  (1000) adpatter  (1000)        0 2023-04-30 21:46:30.220886 notation-0.0.2/src/
+drwxrwxr-x   0 adpatter  (1000) adpatter  (1000)        0 2023-04-30 21:46:30.220886 notation-0.0.2/src/notation/
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)        0 2023-04-30 17:27:32.000000 notation-0.0.2/src/notation/__init__.py
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)      666 2023-04-30 20:03:04.000000 notation-0.0.2/src/notation/notation.py
+drwxrwxr-x   0 adpatter  (1000) adpatter  (1000)        0 2023-04-30 21:46:30.220886 notation-0.0.2/src/notation.egg-info/
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)      573 2023-04-30 21:46:30.000000 notation-0.0.2/src/notation.egg-info/PKG-INFO
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)      226 2023-04-30 21:46:30.000000 notation-0.0.2/src/notation.egg-info/SOURCES.txt
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)        1 2023-04-30 21:46:30.000000 notation-0.0.2/src/notation.egg-info/dependency_links.txt
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)        9 2023-04-30 21:46:30.000000 notation-0.0.2/src/notation.egg-info/top_level.txt
```

### Comparing `notation-0.0.1/LICENSE` & `notation-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `notation-0.0.1/PKG-INFO` & `notation-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: notation
-Version: 0.0.1
-Summary: Notation is a decororator for annotating Python functions.
+Version: 0.0.2
+Summary: Notation is a decorator for annotating Python functions.
 Author-email: Adam Patterson <adam@faranalytics.net>
 Project-URL: Homepage, https://github.com/faranalytics/python_notation
 Project-URL: Bug Tracker, https://github.com/faranalytics/python_notation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `notation-0.0.1/pyproject.toml` & `notation-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "notation"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Adam Patterson", email="adam@faranalytics.net" },
 ]
-description = "Notation is a decororator for annotating Python functions."
+description = "Notation is a decorator for annotating Python functions."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `notation-0.0.1/src/notation/notation.py` & `notation-0.0.2/src/notation/notation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 class Notation:
 
     def __init__(self, annotation={}):
         self.__dict__ = annotation
 
-    def __getitem__(self, name):
-        return self.__dict__[name]
+    def __getitem__(self, key):
+        return self.__dict__[key]
 
-    def __setitem__(self, name, value):
+    def __setitem__(self, key, value):
         self.__dict__[name] = value
 
     def __str__(self):
         return str(self.__dict__)
 
     def __repr__(self):
         return f'{self.__class__.__name__}(annotation={self.__dict__})'
 
+    def __contains__(self, key):
+        return key in self.__dict__
+
     def __call__(self, *args, **kwargs):
         def decorator(fn):
             self.__dict__[fn] = {**{index:arg for index, arg in enumerate(args)}, **kwargs}
             return fn
         return decorator
```

### Comparing `notation-0.0.1/src/notation.egg-info/PKG-INFO` & `notation-0.0.2/src/notation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: notation
-Version: 0.0.1
-Summary: Notation is a decororator for annotating Python functions.
+Version: 0.0.2
+Summary: Notation is a decorator for annotating Python functions.
 Author-email: Adam Patterson <adam@faranalytics.net>
 Project-URL: Homepage, https://github.com/faranalytics/python_notation
 Project-URL: Bug Tracker, https://github.com/faranalytics/python_notation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

