# Comparing `tmp/safenote-0.1.2.tar.gz` & `tmp/safenote-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safenote-0.1.2.tar", max compression
+gzip compressed data, was "safenote-0.1.3.tar", max compression
```

## Comparing `safenote-0.1.2.tar` & `safenote-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      113 2023-04-30 04:52:02.581548 safenote-0.1.2/README.md
--rw-r--r--   0        0        0      538 2023-04-30 04:52:05.126634 safenote-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       25 2023-04-30 04:49:08.107328 safenote-0.1.2/safenote/__init__.py
--rw-r--r--   0        0        0      997 2023-04-30 04:50:44.169758 safenote-0.1.2/safenote/core.py
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 safenote-0.1.2/setup.py
--rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 safenote-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      113 2023-04-30 04:52:02.581548 safenote-0.1.3/README.md
+-rw-r--r--   0        0        0      578 2023-04-30 04:55:49.869392 safenote-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-04-30 04:54:20.716767 safenote-0.1.3/safenote/__init__.py
+-rw-r--r--   0        0        0     1001 2023-04-30 04:54:53.169508 safenote-0.1.3/safenote/core.py
+-rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 safenote-0.1.3/setup.py
+-rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 safenote-0.1.3/PKG-INFO
```

### Comparing `safenote-0.1.2/safenote/core.py` & `safenote-0.1.3/safenote/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from getpass import getpass
 from typing import List, Union
 
 
 def request(key: Union[str, None] = None,
             keys: Union[List[str], None] = None,
             inject_env: bool = True):
-    env = {}
+    env = dict()
     if key is not None:
         if type(key) == str:
             env[key] = _request_single(key, inject_env)
         else:
             raise TypeError('key must be a string or None')
     elif keys is not None:
         if type(keys) == list:
```

### Comparing `safenote-0.1.2/setup.py` & `safenote-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 ['safenote']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'safenote',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'SafeNote (Safe Notebook) is a tool for injecting your secrets into Jupyter notebooks environment safer and easier.',
     'long_description': '<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/b4e3b105-8503-43ac-9116-f51e401b6b00/HD" alt="Cover"/>',
     'author': 'Lingxi Li',
     'author_email': 'lilingxi01@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://github.com/lilingxi01/safenote',
+    'url': 'https://safenote.lingxi.li/',
     'packages': packages,
     'package_data': package_data,
     'python_requires': '>=3.8,<4',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `safenote-0.1.2/PKG-INFO` & `safenote-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: safenote
-Version: 0.1.2
+Version: 0.1.3
 Summary: SafeNote (Safe Notebook) is a tool for injecting your secrets into Jupyter notebooks environment safer and easier.
-Home-page: https://github.com/lilingxi01/safenote
+Home-page: https://safenote.lingxi.li/
 Author: Lingxi Li
 Author-email: lilingxi01@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Project-URL: Documentation, https://safenote.lingxi.li/
 Project-URL: Repository, https://github.com/lilingxi01/safenote
 Description-Content-Type: text/markdown
 
 <img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/b4e3b105-8503-43ac-9116-f51e401b6b00/HD" alt="Cover"/>
```

