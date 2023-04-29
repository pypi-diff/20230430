# Comparing `tmp/poetry_source_env-1.0.0.tar.gz` & `tmp/poetry_source_env-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_source_env-1.0.0.tar", max compression
+gzip compressed data, was "poetry_source_env-1.0.1.tar", max compression
```

## Comparing `poetry_source_env-1.0.0.tar` & `poetry_source_env-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     2540 2023-04-29 22:07:27.371034 poetry_source_env-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-04-29 22:07:27.371034 poetry_source_env-1.0.0/poetry_source_env/__init__.py
--rw-r--r--   0        0        0     1175 2023-04-29 22:07:27.371034 poetry_source_env-1.0.0/poetry_source_env/plugin.py
--rw-r--r--   0        0        0      563 2023-04-29 22:07:27.371034 poetry_source_env-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 poetry_source_env-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-04-29 22:28:03.933338 poetry_source_env-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0     2540 2023-04-29 22:28:03.933338 poetry_source_env-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-29 22:28:03.937338 poetry_source_env-1.0.1/poetry_source_env/__init__.py
+-rw-r--r--   0        0        0     1175 2023-04-29 22:28:03.937338 poetry_source_env-1.0.1/poetry_source_env/plugin.py
+-rw-r--r--   0        0        0      695 2023-04-29 22:28:03.937338 poetry_source_env-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3287 1970-01-01 00:00:00.000000 poetry_source_env-1.0.1/PKG-INFO
```

### Comparing `poetry_source_env-1.0.0/README.md` & `poetry_source_env-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `poetry_source_env-1.0.0/poetry_source_env/plugin.py` & `poetry_source_env-1.0.1/poetry_source_env/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_source_env-1.0.0/pyproject.toml` & `poetry_source_env-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [tool.poetry]
 name = "poetry-source-env"
-version = "1.0.0"
+version = "1.0.1"
 description = "Load Poetry package sources from environment variables"
 authors = ["celsius narhwal <hello@celsiusnarhwal.dev>"]
 readme = "README.md"
 license = "MIT"
+homepage = "https://github.com/celsiusnarhwal/poetry-source-env"
+repository = "https://github.com/celsiusnarhwal/poetry-source-env"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 poetry = "^1.2"
 
 [tool.black]
 target-version = ["py38"]
```

### Comparing `poetry_source_env-1.0.0/PKG-INFO` & `poetry_source_env-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: poetry-source-env
-Version: 1.0.0
+Version: 1.0.1
 Summary: Load Poetry package sources from environment variables
+Home-page: https://github.com/celsiusnarhwal/poetry-source-env
 License: MIT
 Author: celsius narhwal
 Author-email: hello@celsiusnarhwal.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: poetry (>=1.2,<2.0)
+Project-URL: Repository, https://github.com/celsiusnarhwal/poetry-source-env
 Description-Content-Type: text/markdown
 
 # poetry-source-env
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/poetry-source-env?logo=python&logoColor=white&style=for-the-badge)](https://pypi.org/project/poetry-source-env)
 [![PyPI](https://img.shields.io/pypi/v/poetry-source-env?logo=pypi&color=green&logoColor=white&style=for-the-badge)](https://pypi.org/project/poetry-source-env)
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/celsiusnarhwal/poetry-source-env?logo=github&color=orange&logoColor=white&style=for-the-badge)](https://github.com/celsiusnarhwal/poetry-source-env/releases)
```

