# Comparing `tmp/autoadd_bindir-1.0.5.tar.gz` & `tmp/autoadd_bindir-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoadd_bindir-1.0.5.tar", max compression
+gzip compressed data, was "autoadd_bindir-1.0.6.tar", max compression
```

## Comparing `autoadd_bindir-1.0.5.tar` & `autoadd_bindir-1.0.6.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     3340 2023-03-30 07:51:28.321733 autoadd_bindir-1.0.5/docs/readme.md
--rw-r--r--   0        0        0     7299 2023-04-12 15:30:50.381455 autoadd_bindir-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      777 2023-04-12 15:30:50.381455 autoadd_bindir-1.0.5/src/autoadd_bindir/__init__.py
--rw-r--r--   0        0        0     5092 1970-01-01 00:00:00.000000 autoadd_bindir-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3340 2023-04-30 17:50:37.628813 autoadd_bindir-1.0.6/docs/readme.md
+-rw-r--r--   0        0        0     7277 2023-04-30 17:50:37.628813 autoadd_bindir-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      777 2023-04-30 17:50:37.628813 autoadd_bindir-1.0.6/src/autoadd_bindir/__init__.py
+-rw-r--r--   0        0        0      381 2023-04-30 17:50:37.628813 autoadd_bindir-1.0.6/src/autoadd_bindir/py.typed
+-rw-r--r--   0        0        0     5085 1970-01-01 00:00:00.000000 autoadd_bindir-1.0.6/PKG-INFO
```

### Comparing `autoadd_bindir-1.0.5/docs/readme.md` & `autoadd_bindir-1.0.6/docs/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 
 
 ## Installation
 
 Install via pip:
 
 ```bash
-> bin/pip install autoadd_bindir
+> bin/pip install autoadd-bindir
 ```
 
 Or add to your poetry-based project:
 
 ```bash
-> poetry add autoadd_bindir
+> poetry add autoadd-bindir
 ```
 
 
 ## Validate & Usage
 After installing this package there is nothing left to do explicitly.
 We can validate that the plugin work correctly by starting a python-session and checking the ``PATH``-environment-variable:
```

### Comparing `autoadd_bindir-1.0.5/pyproject.toml` & `autoadd_bindir-1.0.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 # [tool.nox.session]
 # python = ["3.10n", "3.11n"]
 
 
 [tool.poetry]
 name = "autoadd_bindir"
-version = "1.0.5" # version managed by poetry-version-plugin
+version = "1.0.6" # version managed by poetry-version-plugin
 license = "MIT"
 description = "Automatically add bin-dir to PATH for every process in your virtualenv."
 readme = "docs/readme.md"
 authors = ["Wouter Vanden Hove <wouter@libranet.eu>"]
 maintainers = ["Wouter Vanden Hove <wouter@libranet.eu>"]
 homepage = "https://github.com/libranet/autoadd_bindir"
 repository = "https://github.com/libranet/autoadd_bindir"
@@ -109,64 +109,66 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development",
     "Typing :: Typed",
 ]
 packages = [{ include = "autoadd_bindir", from = "src" }]
 
 [tool.poetry.dependencies]
-python = ">=3.8.0,<4.0"
-sitecustomize-entrypoints = ">=1.1.0"
+# python = ">=3.8.0,<4.0"
+python = ">=3.8.0"
+sitecustomize-entrypoints = ">=1.1"
 
 [tool.poetry.group.dev.dependencies]
-bandit = { extras = ["toml"], version = ">=1.7.4" }
-black = { version = ">=22.1.0", allow-prereleases = true }
-flake8 = ">=4.0.1"
-flake8-bugbear = ">=23.2.13"
-flake8-docstrings = ">=1.6.0"
-flake8-pyproject = ">=1.2.2"
-flake8-rst-docstrings = ">=0.2.5"
-isort = ">=5.10.1"
-pre-commit = ">=2.14.1"
-pre-commit-hooks = ">=4.1.0"
-pydocstyle = ">=6.3.0"
-pylint = ">=2.12.2"
-ruff = ">=0.0.254"
+bandit = { extras = ["toml"], version = ">=1.7" }
+black = { version = ">=22.1", allow-prereleases = true }
+flake8 = ">=4.0"
+flake8-bugbear = ">=23.2"
+flake8-docstrings = ">=1.6"
+flake8-pyproject = ">=1.2"
+flake8-rst-docstrings = ">=0.2"
+isort = ">=5.10"
+pre-commit = ">=2.14"
+pre-commit-hooks = ">=4.1"
+pydocstyle = ">=6.3"
+pylint = ">=2.12"
+ruff = ">=0.0"
 
 [tool.poetry.group.dist.dependencies]
 pyroma = ">=4.2"
-twine = ">=4.0.2"
+twine = ">=4.0"
 
 [tool.poetry.group.docs.dependencies]
-autoapi = ">=2.0.1"
-myst-parser = ">=1.0.0"
-recommonmark = ">=0.7.1"
-Sphinx = ">=4.4.0"
-sphinx-autoapi = ">=1.8.4"
-sphinx-rtd-theme = ">=1.0.0"
+autoapi = ">=2.0"
+myst-parser = ">=1.0"
+recommonmark = ">=0.7"
+Sphinx = ">=4.4"
+sphinx-autoapi = ">=1.8"
+sphinx-rtd-theme = ">=1.0"
 
 [tool.poetry.group.ipython.dependencies]
-ipdb = ">=0.13.9"
-ipython = ">=8.4.0"
+ipdb = ">=0.13"
+ipython = ">=8.4"
 
 [tool.poetry.group.profiling.dependencies]
-importtime-waterfall = ">=1.0.0"
-tuna = ">=0.5.11"
+importtime-waterfall = ">=1.0"
+tuna = ">=0.5"
 
 [tool.poetry.group.testing.dependencies]
 coverage = { extras = ["toml"], version = ">=6.2" }
-nox = ">=2022.11.21"
-nox-poetry = ">=1.0.2"
-pytest = ">=7.0.1"
-pytest-codecov = ">=0.5.1"
-pytest-cov = ">=3.0.0"
-tox = ">=4.4.7"
+hypothesis = ">=6.72"
+# nox = ">=2022.11"
+# nox-poetry = ">=1.0"
+pytest = ">=7.0"
+pytest-codecov = ">=0.5"
+pytest-cov = ">=3.0"
+# tox = ">=4.4"
 
 [tool.poetry.group.typing.dependencies]
-lxml = { version = ">=4.9.2", optional = true, allow-prereleases = false } # mypy coverage-report
-mypy = ">=0.931"
+lxml = { version = ">=4.9", optional = true, allow-prereleases = false } # mypy coverage-report
+mypy = ">=0.9"
 
 
 [tool.poetry.urls]
 Issues = "https://github.com/libranet/autoadd_bindir/issues"
 Changelog = "https://github.com/libranet/autoadd_bindir/releases"
```

### Comparing `autoadd_bindir-1.0.5/src/autoadd_bindir/__init__.py` & `autoadd_bindir-1.0.6/src/autoadd_bindir/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """autoadd_bindir.__init__."""
-__version__ = "1.0.5"
+__version__ = "1.0.7"
 __copyright__ = "Copyright 2023 Libranet."
 __license__ = "MIT License"
 
 import os
 import pathlib as pl
 import sys
```

### Comparing `autoadd_bindir-1.0.5/PKG-INFO` & `autoadd_bindir-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: autoadd-bindir
-Version: 1.0.5
+Version: 1.0.6
 Summary: Automatically add bin-dir to PATH for every process in your virtualenv.
 Home-page: https://github.com/libranet/autoadd_bindir
 License: MIT
 Keywords: entrypoints,sitecustomize
 Author: Wouter Vanden Hove
 Author-email: wouter@libranet.eu
 Maintainer: Wouter Vanden Hove
 Maintainer-email: wouter@libranet.eu
-Requires-Python: >=3.8.0,<4.0
+Requires-Python: >=3.8.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
-Requires-Dist: sitecustomize-entrypoints (>=1.1.0)
+Requires-Dist: sitecustomize-entrypoints (>=1.1)
 Project-URL: Changelog, https://github.com/libranet/autoadd_bindir/releases
 Project-URL: Documentation, https://autoadd-bindir.readthedocs.io
 Project-URL: Issues, https://github.com/libranet/autoadd_bindir/issues
 Project-URL: Repository, https://github.com/libranet/autoadd_bindir
 Description-Content-Type: text/markdown
 
 [![Testing](https://img.shields.io/github/actions/workflow/status/libranet/autoadd-bindir/testing.yaml?branch=main&longCache=true&style=flat-square&label=tests&logo=GitHub%20Actions&logoColor=fff")](https://github.com/libranet/autoadd-bindir/actions/workflows/testing.yaml)
@@ -63,21 +63,21 @@
 
 
 ## Installation
 
 Install via pip:
 
 ```bash
-> bin/pip install autoadd_bindir
+> bin/pip install autoadd-bindir
 ```
 
 Or add to your poetry-based project:
 
 ```bash
-> poetry add autoadd_bindir
+> poetry add autoadd-bindir
 ```
 
 
 ## Validate & Usage
 After installing this package there is nothing left to do explicitly.
 We can validate that the plugin work correctly by starting a python-session and checking the ``PATH``-environment-variable:
```

