# Comparing `tmp/autoread_dotenv-1.0.1.tar.gz` & `tmp/autoread_dotenv-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoread_dotenv-1.0.1.tar", max compression
+gzip compressed data, was "autoread_dotenv-1.0.2.tar", max compression
```

## Comparing `autoread_dotenv-1.0.1.tar` & `autoread_dotenv-1.0.2.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     2491 2023-03-30 11:41:10.336008 autoread_dotenv-1.0.1/docs/readme.md
--rw-r--r--   0        0        0     7629 2023-03-30 11:41:31.921667 autoread_dotenv-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2912 2023-03-30 11:41:10.336008 autoread_dotenv-1.0.1/src/autoread_dotenv/__init__.py
--rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 autoread_dotenv-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2492 2023-04-30 17:34:25.518911 autoread_dotenv-1.0.2/docs/readme.md
+-rw-r--r--   0        0        0     8132 2023-04-30 17:39:01.838889 autoread_dotenv-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3119 2023-04-30 17:39:01.838889 autoread_dotenv-1.0.2/src/autoread_dotenv/__init__.py
+-rw-r--r--   0        0        0      381 2023-04-22 12:14:09.181077 autoread_dotenv-1.0.2/src/autoread_dotenv/py.typed
+-rw-r--r--   0        0        0     4236 1970-01-01 00:00:00.000000 autoread_dotenv-1.0.2/PKG-INFO
```

### Comparing `autoread_dotenv-1.0.1/docs/readme.md` & `autoread_dotenv-1.0.2/docs/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 
 ## Installation
 
 Install via pip:
 
 ```bash
-> bin/pip install autoread_dotenv
+> bin/pip install autoread-dotenv
 ```
 
 Or add to your poetry-based project:
 
 ```bash
-> poetry add autoread_dotenv
+> poetry add autoread-dotenv
 ```
 
 
 ## Usage
 
 The only thing left to do for you is the create a ``.env`` in the root of your project.
 
@@ -48,8 +48,8 @@
 
 ``autoread-dotenv``  works on Python 3.8+, including PyPy3. Tested until Python 3.11,
 
 
 ## Notable dependencies
 
 - [sitecustomize-entrypoints](http://pypi.python.org/pypi/sitecustomize-entrypoints)
-- [python-dotenv](http://pypi.python.org/pypi/python-dotenv)
+- [python-dotenv](http://pypi.python.org/pypi/python-dotenv)
```

### Comparing `autoread_dotenv-1.0.1/pyproject.toml` & `autoread_dotenv-1.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -17,32 +17,40 @@
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.bandit]
 # bandit does not use this config by default.
 # You need to invoke "bandit --configfile pyproject.toml"
 # see https://github.com/PyCQA/bandit/issues/318"
-baseline = "etc/bandit-baseline.json"
+# baseline = "etc/bandit-baseline.json"
 exclude_dirs = [".venv", "var"]
 recursive = true
-skips = ["B101"]
-targets = ["src", "tests"]
+skips = [
+    # see https://bandit.readthedocs.io/en/1.7.3/plugins/index.html#plugin-id-groupings
+    # "B101", # assert_used
+]
+targets = ["docs", "src", "tests"]
+
+[tool.bandit.assert_used]
+skips = ["*/test_*.py"]
 
 
 [tool.black]
 line-length = 120
 target_version = ["py310"]
 include = '\.py$'          # regex -> single-quotes
 
 
 [tool.coverage.html]
-directory = "var/coverage/html"
+# directory = "var/coverage/html"
+directory = "var/html/coverage"
 
 [tool.coverage.xml]
-output = "var/coverage/coverage.xml"
+# output = "var/coverage/coverage.xml"
+output = "var/html/coverage/coverage.xml"
 
 
 [tool.coverage.report]
 # cfr. https://coverage.readthedocs.io/en/coverage-4.2/excluding.html
 exclude_lines = [
     "pragma: no cover",
     "raise AssertionError",
@@ -50,22 +58,30 @@
     "if 0:",
     "if __name__ == .__main__.:",
 ]
 include = ["src/*"]
 
 [tool.coverage.run]
 branch = true
-data_file = "var/coverage/coverage.db"
+data_file = "var/cache/coverage/coverage.db"
 
 
 [tool.flake8]
+# Google Python style is not RST until after processed by Napoleon
+# See https://github.com/peterjc/flake8-rst-docstrings/issues/17
+extend-ignore = ["RST201", "RST203", "RST213", "RST301"]
+ignore = [
+    "D103", # Missing docstring in public function
+    "B028", # No explicit stacklevel argument found.
+    "W503", # incompatible with black, see https://github.com/psf/black/issues/52
+]
 max_line_length = 121
 per_file_ignores = [
     "tests/test_entrypoints.py:B011", # B011: Do not call assert False
-    "__init__.py:F401",               # F401: imported but unused
+    # "__init__.py:F401",               # F401: imported but unused
 ]
 
 
 [tool.isort]
 include_trailing_comma = true # corresponds to -tc flag
 known_third_party = []
 line_length = 120             # corresponds to -w  flag
@@ -84,23 +100,23 @@
 
 [tool.nox]
 envdir = "var/cache/nox"
 
 
 [tool.poetry]
 name = "autoread_dotenv"
-version = "1.0.1"
+version = "1.0.2"
 license = "MIT"
 description = "Automatically set env-vars at the beginning of every python-process in your in-project virtualenv."
 readme = "docs/readme.md"
 authors = ["Wouter Vanden Hove <wouter@libranet.eu>"]
 maintainers = ["Wouter Vanden Hove <wouter@libranet.eu>"]
-homepage = "https://github.com/libranet/autoread_dotenv"
-repository = "https://github.com/libranet/autoread_dotenv"
-documentation = "https://autoadd-bindir.readthedocs.io"
+homepage = "https://github.com/libranet/autoread-dotenv"
+repository = "https://github.com/libranet/autoread-dotenv"
+documentation = "https://autoread-dotenv.readthedocs.io"
 keywords = ["entrypoints", "dotenv", "sitecustomize"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
@@ -112,76 +128,77 @@
     "Programming Language :: Python :: Implementation :: PyPy",
     "Typing :: Typed",
 ]
 packages = [{ include = "autoread_dotenv", from = "src" }]
 
 
 [tool.poetry.dependencies]
-# These packages are mandatory and form the core of this package’s distribution.
-python = ">=3.8.0,<4.0"
+# python = ">=3.8.0,<4.0"
+python = ">=3.8.0"
 python-dotenv = ">=1.0.0"
-sitecustomize-entrypoints = ">=0.1.0"
+sitecustomize-entrypoints = ">=1.1.0"
 
 [tool.poetry.group.dev.dependencies]
-# poetry install --with | --without dev
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
-pylint = ">=2.12.2"
-ruff = ">=0.0.254"
+black = { version = ">=22.1", allow-prereleases = true }
+flake8 = ">=4.0"
+flake8-bugbear = ">=23.2"
+flake8-docstrings = ">=1.6"
+flake8-pyproject = ">=1.2"
+flake8-rst-docstrings = ">=0.2"
+isort = ">=5.10"
+pre-commit = ">=2.14"
+pre-commit-hooks = ">=4.1"
+pylint = ">=2.12"
+ruff = ">=0.0"
 
 [tool.poetry.group.dist.dependencies]
 pyroma = ">=4.2"
-twine = ">=4.0.2"
+twine = ">=4.0"
 
 [tool.poetry.group.docs.dependencies]
-# poetry install --with | --without docs
-autoapi = ">=2.0.1"
-markupsafe = ">=2.1.2"
-myst-parser = ">=1.0.0"
-recommonmark = ">=0.7.1"
-Sphinx = ">=4.4.0"
-sphinx-autoapi = ">=1.8.4"
-sphinx-rtd-theme = ">=1.0.0"
+autoapi = ">=2.0"
+markupsafe = ">=2.1"
+myst-parser = ">=1.0"
+recommonmark = ">=0.7"
+Sphinx = ">=4.4"
+sphinx-autoapi = ">=1.8"
+sphinx-rtd-theme = ">=1.0"
 
 [tool.poetry.group.ipython.dependencies]
-# poetry install --with | --without ipython
-ipdb = ">=0.13.9"
-ipython = ">=8.4.0"
+ipdb = ">=0.13"
+ipython = ">=8.4"
 
 [tool.poetry.group.profiling.dependencies]
-# poetry install --with | --without profiling
-importtime-waterfall = ">=1.0.0"
-tuna = ">=0.5.11"
+importtime-waterfall = ">=1.0"
+tuna = ">=0.5"
+
+[tool.poetry.group.security.dependencies]
+bandit = { extras = ["toml"], version = ">=1.7" }
+safety = ">=2.3"
+
 
 [tool.poetry.group.testing.dependencies]
-# poetry install --with | --without testing
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
-"Bug Tracker" = "https://github.com/Libranet/autoread_dotenv/issues"
-
+"Bug Tracker" = "https://github.com/libranet/autoread-dotenv/issues"
+repository = "https://github.com/libranet/autoread-dotenv"
+Docs = "https://autoread-dotenv.readthedocs.io"
 
 [tool.poetry2conda]
 # https://pypi.org/project/poetry2conda/
 # https://levelup.gitconnected.com/publishing-your-python-package-on-conda-and-conda-forge-309a405740cf
 name = "conda-base"
 
 
@@ -230,23 +247,24 @@
 ]
 
 [tool.pylint.messages_control]
 disable = [
     "C0116", # missing-function-docstring
 ]
 
+
 [tool.pytest.ini_options]
 cache_dir = "var/cache/pytest"
 log_cli = false                   # enable to show log-output
 log_cli_level = "NOTSET"
 filterwarnings = []
 markers = ["unit", "integration"]
 testpaths = ["tests"]
 # the junit-report is used to report coverage in gitlab
-addopts = "--color=yes --junit-xml='var/coverage/pytest.xml'"
+addopts = "--color=yes --junit-xml='var/cache/coverage/pytest.xml'"
 
 
 # [tool.tox.legacy_tox_ini]
 # # envlist = ["py38", "py39", "py310", "py311"]
 # # isolated_build = true
 # toxworkdir = "var/cache/tox"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `autoread_dotenv-1.0.1/src/autoread_dotenv/__init__.py` & `autoread_dotenv-1.0.2/src/autoread_dotenv/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,90 +11,99 @@
 
   <project-root>
       .env
       .venv/
           bin/
               python
           lib/
+          lib64/
           pyvenv.cfg
 
   We also support toplevel-symlinks to the corresponding .venv-files:
 
 .. code-block:: python
 
       bin/       -> .venv/bin/
       lib/       -> .venv/lib/
-      lib64/       -> .venv/lib64/
+      lib64/     -> .venv/lib64/
       pyvenv.cfg -> .venv/pyvenv.cfg
 
 """
 
-__version__ = "1.0.1"
-__copyright__ = "Copyright 2023 Libranet - MIT License."
+__version__ = "1.0.2"
+__copyright__ = "Copyright 2023 Libranet"
+__license__ = "MIT License"
 
 import os
 import pathlib as pl
 import sys
 import typing as tp
+import warnings
 
 try:
     import dotenv
 
-    dotenv_available = 1  # pylint: disable=invalid-name
+    DOTENV_INSTALLED = 1
 except ImportError:  # pragma: no cover
-    dotenv_available = 0  # pylint: disable=invalid-name
+    DOTENV_INSTALLED = 0
+
+
+class SimpleWarning:
+    """Simple warning-formatting ."""
+
+    def __init__(self) -> None:
+        """Initialize class."""
+        self.old_format: tp.Optional[tp.Callable] = warnings.formatwarning
+
+    def __enter__(self) -> "SimpleWarning":
+        """Enter contextmanager."""
+        warnings.formatwarning = self.simple_message  # type: ignore
+        return self
+
+    def __exit__(self, *args) -> None:
+        """Exit contextmanager."""
+        warnings.formatwarning = self.old_format  # type: ignore
+
+    @staticmethod
+    def simple_message(message: str, *args, **kwargs) -> str:  # pylint: disable=unused-argument
+        """Return a simple warning-message without any traceback-info."""
+        return f"Warning from {__name__}: {message}\n"
 
 
 def get_dotenv_path() -> tp.Optional[pl.Path]:
     """Return the location of the .env for in-project virtualenvs.
-    Return None of no .env-file is found.
+
+    Return None of the .env-file does not exist.
     """
     # sys.prefix is <project-root>/.venv or <project-root> when using toplevel symlinks to .venv
     prefix = pl.Path(sys.prefix)
     base_dir = prefix.parent if prefix.name == ".venv" else prefix
     dotenv_file = base_dir / ".env"
 
-    if not dotenv_file.exists():  # pragma: no cover
-        return None
+    if dotenv_file.exists():
+        return dotenv_file
 
-    return dotenv_file
+    return None
 
 
 def entrypoint() -> None:
     """Set environment-variable from the in-project .env-file."""
-    dotenv_file = get_dotenv_path()
-
-    enforce_dotenv = bool(os.getenv("ENFORCE_DOTENV", "1"))
-
-    if dotenv_file and dotenv_available:
-        try:
-            dotenv.load_dotenv(dotenv_file, override=enforce_dotenv, interpolate=True, verbose=True)
-        except AttributeError:  # pragma: no cover
-            # this happens when django-dotenv was installed
-            # while we depend on python-dotenv.
-            pass
-
+    dotenv_file: tp.Optional[pl.Path] = get_dotenv_path()
+    enforce_dotenv: bool = bool(os.getenv("ENFORCE_DOTENV", "1"))
 
-def cancel():
-    """No-op function that can be used the cancel a registered entrypoint.
-
-    Imagine you have multiple sitecustomize-entrypoints. If these entrypoints
-    are registered via third-party packages, you cannot control the order of execution.
-
-    Now suppose some of these entrypoints need an environment-variable that first need to be set
-    by ``autoread_dotenv`` needs to be executed before the others
-
-    entrypoint 1:  foo.needs_envvar:bar
-    entrypoint 2:  autoread_dotenv.autoread:autoread_dotenv
-
-    in your project's pyproject.toml:
-
-    [tool.poetry.plugins."sitecustomize"]
-
-    # cancel the first registration using the original name
-    autoread_dotenv = "autoread_dotenv.autoread:cancel"
-
-    # re-register the same function under different name
-    zz_autoread_dotenv = "autoread_dotenv.autoread:autoread_dotenv"
-
-    """
-    pass  # pylint: disable=unnecessary-pass
+    if not DOTENV_INSTALLED:  # pragma: no cover
+        with SimpleWarning():
+            warnings.warn("Module 'dotenv' not found. Please pip install 'python-dotenv'.")
+        return
+
+    if not dotenv_file:  # pragma: no cover
+        with SimpleWarning():
+            warnings.warn(f"{dotenv_file} does not yet exist, please create it.")
+        return
+
+    try:
+        dotenv.load_dotenv(dotenv_file, override=enforce_dotenv, interpolate=True, verbose=True)
+    except AttributeError:  # pragma: no cover
+        warnings.warn(
+            "Module 'dotenv.load_dotenv' not found."
+            + "This occurs when django-dotenv was installed while we depend on python-dotenv."
+        )
```

### Comparing `autoread_dotenv-1.0.1/PKG-INFO` & `autoread_dotenv-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: autoread-dotenv
-Version: 1.0.1
+Version: 1.0.2
 Summary: Automatically set env-vars at the beginning of every python-process in your in-project virtualenv.
-Home-page: https://github.com/libranet/autoread_dotenv
+Home-page: https://github.com/libranet/autoread-dotenv
 License: MIT
 Keywords: entrypoints,dotenv,sitecustomize
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
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -24,18 +24,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Typing :: Typed
 Requires-Dist: python-dotenv (>=1.0.0)
-Requires-Dist: sitecustomize-entrypoints (>=0.1.0)
-Project-URL: Bug Tracker, https://github.com/Libranet/autoread_dotenv/issues
-Project-URL: Documentation, https://autoadd-bindir.readthedocs.io
-Project-URL: Repository, https://github.com/libranet/autoread_dotenv
+Requires-Dist: sitecustomize-entrypoints (>=1.1.0)
+Project-URL: Bug Tracker, https://github.com/libranet/autoread-dotenv/issues
+Project-URL: Documentation, https://autoread-dotenv.readthedocs.io
+Project-URL: Docs, https://autoread-dotenv.readthedocs.io
+Project-URL: Repository, https://github.com/libranet/autoread-dotenv
+Project-URL: repository, https://github.com/libranet/autoread-dotenv
 Description-Content-Type: text/markdown
 
 [![Testing](https://img.shields.io/github/actions/workflow/status/libranet/autoread-dotenv/testing.yaml?branch=main&longCache=true&style=flat-square&label=tests&logo=GitHub%20Actions&logoColor=fff")](https://github.com/libranet/autoread-dotenv/actions/workflows/testing.yaml)
 [![Linting](https://img.shields.io/github/actions/workflow/status/libranet/autoread-dotenv/linting.yaml?branch=main&longCache=true&style=flat-square&label=linting&logo=GitHub%20Actions&logoColor=fff")](https://github.com/libranet/autoread-dotenv/actions/workflows/linting.yaml)
 [![Read the Docs](https://readthedocs.org/projects/autoread-dotenv/badge/?version=latest)](https://autoread-dotenv.readthedocs.io/en/latest/)
 [![Codecov](https://codecov.io/gh/libranet/autoread-dotenv/branch/main/graph/badge.svg?token=QTOWRXGH61)](https://codecov.io/gh/libranet/autoread-dotenv)
 [![PyPi Package](https://img.shields.io/pypi/v/autoread-dotenv?color=%2334D058&label=pypi%20package)](https://pypi.org/project/autoread-dotenv/)
@@ -44,21 +46,21 @@
 
 
 ## Installation
 
 Install via pip:
 
 ```bash
-> bin/pip install autoread_dotenv
+> bin/pip install autoread-dotenv
 ```
 
 Or add to your poetry-based project:
 
 ```bash
-> poetry add autoread_dotenv
+> poetry add autoread-dotenv
 ```
 
 
 ## Usage
 
 The only thing left to do for you is the create a ``.env`` in the root of your project.
 
@@ -85,7 +87,8 @@
 ``autoread-dotenv``  works on Python 3.8+, including PyPy3. Tested until Python 3.11,
 
 
 ## Notable dependencies
 
 - [sitecustomize-entrypoints](http://pypi.python.org/pypi/sitecustomize-entrypoints)
 - [python-dotenv](http://pypi.python.org/pypi/python-dotenv)
+
```

