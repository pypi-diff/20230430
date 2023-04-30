# Comparing `tmp/zmtools-2.0.3.tar.gz` & `tmp/zmtools-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zmtools-2.0.3.tar", max compression
+gzip compressed data, was "zmtools-2.0.4.tar", max compression
```

## Comparing `zmtools-2.0.3.tar` & `zmtools-2.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2022-02-06 01:51:30.000000 zmtools-2.0.3/LICENSE
--rw-r--r--   0        0        0      144 2022-02-06 01:51:30.000000 zmtools-2.0.3/README.md
--rw-r--r--   0        0        0      831 2022-02-06 01:52:19.859650 zmtools-2.0.3/pyproject.toml
--rw-r--r--   0        0        0       42 2022-02-06 01:52:19.861650 zmtools-2.0.3/zmtools/__init__.py
--rw-r--r--   0        0        0     6154 2022-02-06 01:51:30.000000 zmtools-2.0.3/zmtools/api.py
--rw-r--r--   0        0        0      797 2022-02-06 01:52:19.907306 zmtools-2.0.3/setup.py
--rw-r--r--   0        0        0      775 2022-02-06 01:52:19.907498 zmtools-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-02-28 00:00:47.000000 zmtools-2.0.4/LICENSE
+-rw-r--r--   0        0        0      145 2022-02-28 00:00:47.000000 zmtools-2.0.4/README.md
+-rw-r--r--   0        0        0      831 2022-02-28 00:01:24.699721 zmtools-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0      177 2022-02-28 00:01:24.700721 zmtools-2.0.4/zmtools/__init__.py
+-rw-r--r--   0        0        0     6161 2022-02-28 00:00:47.000000 zmtools-2.0.4/zmtools/api.py
+-rw-r--r--   0        0        0      798 2022-02-28 00:01:24.747883 zmtools-2.0.4/setup.py
+-rw-r--r--   0        0        0      776 2022-02-28 00:01:24.748262 zmtools-2.0.4/PKG-INFO
```

### Comparing `zmtools-2.0.3/LICENSE` & `zmtools-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zmtools-2.0.3/pyproject.toml` & `zmtools-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zmtools"
-version = "2.0.3"
+version = "2.0.4"
 description = "Various tools used across Zeke Marffy's programs"
 authors = ["Zeke Marffy <zmarffy@yahoo.com>"]
 readme = "README.md"
 repository = "https://github.com/zmarffy/zmtools"
 homepage = "https://github.com/zmarffy/zmtools"
 license = "MIT"
```

### Comparing `zmtools-2.0.3/zmtools/api.py` & `zmtools-2.0.4/zmtools/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 @contextmanager
 def dummy_context_manager(*args, **kwargs) -> None:
     """Useless context manager"""
     yield
 
 
 def get_dpkg_package_version(package_name: str) -> str:
-    """Get the version of an installed package.
+    """Get the version of an installed Debian package.
 
     Args:
         package_name (str): The package name
 
     Returns:
         str: The version of the package
     """
```

### Comparing `zmtools-2.0.3/setup.py` & `zmtools-2.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['click>=2.0.0']
 
 setup_kwargs = {
     'name': 'zmtools',
-    'version': '2.0.3',
+    'version': '2.0.4',
     'description': "Various tools used across Zeke Marffy's programs",
-    'long_description': '# zmtools\n\nA conglomeration of functions reused in my program; maybe they can help you too. The docstrings should explain all you need to know.\n',
+    'long_description': '# zmtools\n\nA conglomeration of functions reused in my programs; maybe they can help you too. The docstrings should explain all you need to know.\n',
     'author': 'Zeke Marffy',
     'author_email': 'zmarffy@yahoo.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/zmarffy/zmtools',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `zmtools-2.0.3/PKG-INFO` & `zmtools-2.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zmtools
-Version: 2.0.3
+Version: 2.0.4
 Summary: Various tools used across Zeke Marffy's programs
 Home-page: https://github.com/zmarffy/zmtools
 License: MIT
 Author: Zeke Marffy
 Author-email: zmarffy@yahoo.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,9 +14,9 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (>=2.0.0)
 Project-URL: Repository, https://github.com/zmarffy/zmtools
 Description-Content-Type: text/markdown
 
 # zmtools
 
-A conglomeration of functions reused in my program; maybe they can help you too. The docstrings should explain all you need to know.
+A conglomeration of functions reused in my programs; maybe they can help you too. The docstrings should explain all you need to know.
```

