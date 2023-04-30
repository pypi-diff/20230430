# Comparing `tmp/safenote-0.1.3.tar.gz` & `tmp/safenote-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safenote-0.1.3.tar", max compression
+gzip compressed data, was "safenote-0.1.4.tar", max compression
```

## Comparing `safenote-0.1.3.tar` & `safenote-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0      113 2023-04-30 04:52:02.581548 safenote-0.1.3/README.md
--rw-r--r--   0        0        0      578 2023-04-30 04:55:49.869392 safenote-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       26 2023-04-30 04:54:20.716767 safenote-0.1.3/safenote/__init__.py
--rw-r--r--   0        0        0     1001 2023-04-30 04:54:53.169508 safenote-0.1.3/safenote/core.py
--rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 safenote-0.1.3/setup.py
--rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 safenote-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      113 2023-04-30 04:52:02.581548 safenote-0.1.4/README.md
+-rw-r--r--   0        0        0      578 2023-04-30 05:00:11.743529 safenote-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1001 2023-04-30 05:00:05.191895 safenote-0.1.4/safenote/__init__.py
+-rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 safenote-0.1.4/setup.py
+-rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 safenote-0.1.4/PKG-INFO
```

### Comparing `safenote-0.1.3/pyproject.toml` & `safenote-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "safenote"
-version = "0.1.3"
+version = "0.1.4"
 description = "SafeNote (Safe Notebook) is a tool for injecting your secrets into Jupyter notebooks environment safer and easier."
 authors = ["Lingxi Li <lilingxi01@gmail.com>"]
 readme = "README.md"
 homepage = "https://safenote.lingxi.li/"
 repository = "https://github.com/lilingxi01/safenote"
 packages = [
     { include = "safenote" },
```

### Comparing `safenote-0.1.3/safenote/core.py` & `safenote-0.1.4/safenote/__init__.py`

 * *Files identical despite different names*

### Comparing `safenote-0.1.3/setup.py` & `safenote-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['safenote']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'safenote',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'SafeNote (Safe Notebook) is a tool for injecting your secrets into Jupyter notebooks environment safer and easier.',
     'long_description': '<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/b4e3b105-8503-43ac-9116-f51e401b6b00/HD" alt="Cover"/>',
     'author': 'Lingxi Li',
     'author_email': 'lilingxi01@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://safenote.lingxi.li/',
```

### Comparing `safenote-0.1.3/PKG-INFO` & `safenote-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safenote
-Version: 0.1.3
+Version: 0.1.4
 Summary: SafeNote (Safe Notebook) is a tool for injecting your secrets into Jupyter notebooks environment safer and easier.
 Home-page: https://safenote.lingxi.li/
 Author: Lingxi Li
 Author-email: lilingxi01@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

