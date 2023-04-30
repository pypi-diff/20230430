# Comparing `tmp/hyperfast_python_template-0.4.6.tar.gz` & `tmp/hyperfast_python_template-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfast_python_template-0.4.6.tar", max compression
+gzip compressed data, was "hyperfast_python_template-0.4.7.tar", max compression
```

## Comparing `hyperfast_python_template-0.4.6.tar` & `hyperfast_python_template-0.4.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-04-29 10:14:38.487161 hyperfast_python_template-0.4.6/LICENSE
--rw-r--r--   0        0        0     2573 2023-04-29 10:14:38.487161 hyperfast_python_template-0.4.6/README.md
--rw-r--r--   0        0        0     2968 2023-04-29 10:14:55.363051 hyperfast_python_template-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      323 2023-04-29 10:14:38.491161 hyperfast_python_template-0.4.6/src/hyperfastpy/__cli__.py
--rw-r--r--   0        0        0      135 2023-04-29 10:14:38.491161 hyperfast_python_template-0.4.6/src/hyperfastpy/__init__.py
--rw-r--r--   0        0        0       22 2023-04-29 10:14:55.315051 hyperfast_python_template-0.4.6/src/hyperfastpy/_version.py
--rw-r--r--   0        0        0      272 2023-04-29 10:14:55.315051 hyperfast_python_template-0.4.6/src/hyperfastpy/conf/about/__init__.yaml
--rw-r--r--   0        0        0      243 2023-04-29 10:14:38.491161 hyperfast_python_template-0.4.6/src/hyperfastpy/project.toml
--rw-r--r--   0        0        0        0 2023-04-29 10:14:38.491161 hyperfast_python_template-0.4.6/src/hyperfastpy/py.typed
--rw-r--r--   0        0        0      242 2023-04-29 10:14:38.491161 hyperfast_python_template-0.4.6/src/hyperfastpy/pyproject.toml
--rw-r--r--   0        0        0     3239 1970-01-01 00:00:00.000000 hyperfast_python_template-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-30 19:12:08.379012 hyperfast_python_template-0.4.7/LICENSE
+-rw-r--r--   0        0        0     2573 2023-04-30 19:12:08.379012 hyperfast_python_template-0.4.7/README.md
+-rw-r--r--   0        0        0     2968 2023-04-30 19:12:27.475321 hyperfast_python_template-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0      323 2023-04-30 19:12:08.379012 hyperfast_python_template-0.4.7/src/hyperfastpy/__cli__.py
+-rw-r--r--   0        0        0      135 2023-04-30 19:12:08.379012 hyperfast_python_template-0.4.7/src/hyperfastpy/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-30 19:12:27.423319 hyperfast_python_template-0.4.7/src/hyperfastpy/_version.py
+-rw-r--r--   0        0        0      272 2023-04-30 19:12:27.423319 hyperfast_python_template-0.4.7/src/hyperfastpy/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      243 2023-04-30 19:12:08.379012 hyperfast_python_template-0.4.7/src/hyperfastpy/project.toml
+-rw-r--r--   0        0        0        0 2023-04-30 19:12:08.379012 hyperfast_python_template-0.4.7/src/hyperfastpy/py.typed
+-rw-r--r--   0        0        0      242 2023-04-30 19:12:08.379012 hyperfast_python_template-0.4.7/src/hyperfastpy/pyproject.toml
+-rw-r--r--   0        0        0     3239 1970-01-01 00:00:00.000000 hyperfast_python_template-0.4.7/PKG-INFO
```

### Comparing `hyperfast_python_template-0.4.6/LICENSE` & `hyperfast_python_template-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.4.6/README.md` & `hyperfast_python_template-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.4.6/pyproject.toml` & `hyperfast_python_template-0.4.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperfast-python-template"
-version = "0.4.6"
+version = "0.4.7"
 description = "A python template that helps you jump start your project"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyperfast-python.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyperfast-python-template"
 readme = "README.md"
 packages = [{ include = "hyperfastpy", from = "src" }]
```

### Comparing `hyperfast_python_template-0.4.6/PKG-INFO` & `hyperfast_python_template-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfast-python-template
-Version: 0.4.6
+Version: 0.4.7
 Summary: A python template that helps you jump start your project
 Home-page: https://hyperfast-python.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

