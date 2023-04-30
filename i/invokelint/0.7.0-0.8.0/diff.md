# Comparing `tmp/invokelint-0.7.0.tar.gz` & `tmp/invokelint-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invokelint-0.7.0.tar", last modified: Wed Apr 26 14:04:41 2023, max compression
+gzip compressed data, was "invokelint-0.8.0.tar", last modified: Sun Apr 30 12:39:16 2023, max compression
```

## Comparing `invokelint-0.7.0.tar` & `invokelint-0.8.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:04:41.937033 invokelint-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-26 14:03:10.000000 invokelint-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 14:03:10.000000 invokelint-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-04-26 14:04:41.937033 invokelint-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-04-26 14:03:10.000000 invokelint-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:04:41.933033 invokelint-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-26 14:03:10.000000 invokelint-0.7.0/docs/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:04:41.937033 invokelint-0.7.0/invokelint/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:04:41.937033 invokelint-0.7.0/invokelint/path/
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/path/filter_duplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/path/setuptools.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/ruff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:04:41.937033 invokelint-0.7.0/invokelint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-04-26 14:04:41.000000 invokelint-0.7.0/invokelint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-26 14:04:41.000000 invokelint-0.7.0/invokelint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:04:41.000000 invokelint-0.7.0/invokelint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:04:41.000000 invokelint-0.7.0/invokelint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-26 14:04:41.000000 invokelint-0.7.0/invokelint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 14:04:41.000000 invokelint-0.7.0/invokelint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-04-26 14:03:10.000000 invokelint-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 14:04:41.937033 invokelint-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 14:03:10.000000 invokelint-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:04:41.937033 invokelint-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-26 14:03:10.000000 invokelint-0.7.0/tests/test__clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-26 14:03:10.000000 invokelint-0.7.0/tests/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-26 14:03:10.000000 invokelint-0.7.0/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-26 14:03:10.000000 invokelint-0.7.0/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-26 14:03:10.000000 invokelint-0.7.0/tests/test_style.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-26 14:03:10.000000 invokelint-0.7.0/tests/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:39:16.731866 invokelint-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-30 12:38:15.000000 invokelint-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-30 12:38:15.000000 invokelint-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12388 2023-04-30 12:39:16.731866 invokelint-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-04-30 12:38:15.000000 invokelint-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:39:16.727865 invokelint-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-30 12:38:15.000000 invokelint-0.8.0/docs/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:39:16.731866 invokelint-0.8.0/invokelint/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:39:16.731866 invokelint-0.8.0/invokelint/path/
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/path/filter_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/path/setuptools.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/ruff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:39:16.731866 invokelint-0.8.0/invokelint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12388 2023-04-30 12:39:16.000000 invokelint-0.8.0/invokelint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-30 12:39:16.000000 invokelint-0.8.0/invokelint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:39:16.000000 invokelint-0.8.0/invokelint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:39:16.000000 invokelint-0.8.0/invokelint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-30 12:39:16.000000 invokelint-0.8.0/invokelint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 12:39:16.000000 invokelint-0.8.0/invokelint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-04-30 12:38:15.000000 invokelint-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-30 12:39:16.735865 invokelint-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-30 12:38:15.000000 invokelint-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:39:16.731866 invokelint-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-30 12:38:15.000000 invokelint-0.8.0/tests/test__clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-30 12:38:15.000000 invokelint-0.8.0/tests/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-30 12:38:15.000000 invokelint-0.8.0/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-30 12:38:15.000000 invokelint-0.8.0/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-30 12:38:15.000000 invokelint-0.8.0/tests/test_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-30 12:38:15.000000 invokelint-0.8.0/tests/test_test.py
```

### Comparing `invokelint-0.7.0/LICENSE` & `invokelint-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invokelint-0.7.0/PKG-INFO` & `invokelint-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invokelint
-Version: 0.7.0
+Version: 0.8.0
 Summary: Invokes Python dev tools at once.
 Author-email: Yukihiko Shinoda <yuk.hik.future@gmail.com>
 Maintainer-email: Yukihiko Shinoda <yuk.hik.future@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yukihiko Shinoda
         
@@ -83,22 +83,22 @@
 
 You can choose which dev tool you'll install, this package doesn't force to install each of dev tools. It helps you to avoid conflicts or breaking your project's dependencies.
 
 Supporting tools:
 
 Linters:
 
+- [Xenon]
 - [Ruff]
 - [Bandit]
 - [dodgy]
 - [Flake8]
 - [pydocstyle]
-- [Xenon]
-- [Pylint]
 - [mypy]
+- [Pylint]
 - [Semgrep]
 
 Formatters:
 
 - [docformatter]
 - [isort]
 - [autoflake]
@@ -124,52 +124,52 @@
 
 This doesn't pollute your comfortable namespaces of command line tools. Thanks to [Invoke], you can place commands into your selected namespace. (See: [Quickstart](#quickstart))
 
 ## Representative commands
 
 (Note that the namespaces of following commands can be changed as you like. See: [Quickstart](#quickstart))
 
+### `inv style`
+
+Formats code by following tools at once:
+
+1. [docformatter]
+2. [isort]
+3. [autoflake]
+4. [Black]
+5. [Ruff]
+
+- `inv style --check` can only check.
+- `inv style --ruff` can leave Ruff warnings.
+
 ### `inv lint`
 
 Runs following fast lints at once:
 
-1. [Ruff]
-2. [Bandit]
-3. [dodgy]
-4. [Flake8]
-5. [pydocstyle]
-6. [Xenon]
+1. [Xenon]
+2. [Ruff]
+3. [Bandit]
+4. [dodgy]
+5. [Flake8]
+6. [pydocstyle]
 
 The format task ([described later](#inv-style)) also run before run above lints. You can skip them by `--skip-format` option.
 
 ### `inv lint.deep`
 
 Runs following slow but detailed lints at once:
 
-1. [Pylint]
-2. [mypy]
+1. [mypy]
+2. [Pylint]
 3. [Semgrep]
 
 ### `inv radon`
 
 Reports [radon] both code complexity and maintainability index.
 
-### `inv style`
-
-Formats code by following tools at once:
-
-1. [docformatter]
-2. [isort]
-3. [autoflake]
-4. [Black]
-5. [Ruff] (optional)
-
-* `inv style --check` can only check.
-* `inv style --ruff` can fix Ruff warnings at once.
-
 ### `inv test`
 
 Runs fast tests (which is not marked `@pytest.mark.slow`) by [pytest].
 
 See:
 
 - [How to mark test functions with attributes — pytest documentation]
@@ -212,20 +212,22 @@
 build = "*"
 # Hotfix for Pipenv's Bug:
 # - Pipenv should prioritize more cross-platform sys_platform condition between packages when lock
 #   · Issue #4101 · pypa/pipenv
 #   https://github.com/pypa/pipenv/issues/4101
 colorama = "*"
 coverage = ">=3.5.4"
-dlint = "*"
+# The dlint less than 0.14.0 limits max version of flake8.
+dlint = ">=0.14.0"
 docformatter = {extras = ["tomli"], version = "*"}
 dodgy = "*"
 # Since Pipenv can't lock for too much combinations to attempt lock:
 # pip._vendor.resolvelib.resolvers.ResolutionTooDeep: 2000000
-flake8 = {version = "==4.0.1", markers="python_version >= '3.6'"}
+# The hacking depends flake8 ~=5.0.1 or ~=4.0.1.
+flake8 = {version = "<=6.0.0>=5.0.1,==4.0.1", markers="python_version >= '3.6'"}
 # To use flake8 --radon-show-closures
 flake8-polyfill = "*"
 # Latest hacking depends on legacy version of flake8, and legacy hacking doesn't narrow flake8 version.
 # When unpin hacking, it has possibility to install too legacy version of hacking.
 hacking = {version = ">=5.0.0", markers="python_version >= '3.8'"}
 invokelint = {version = "*", markers="python_version >= '3.7'"}
 isort = "*"
@@ -254,15 +256,15 @@
 ```python
 """Tasks for maintaining the project.
 
 Execute 'invoke --list' for guidance on using Invoke
 """
 from invoke import Collection
 
-from invokelint import _clean, dist, lint, path, style, test
+from invokelint import dist, lint, path, style, test
 
 ns = Collection()
 ns.add_collection(dist)
 ns.add_collection(lint)
 ns.add_collection(path)
 ns.add_collection(style)
 ns.add_collection(test)
```

### Comparing `invokelint-0.7.0/README.md` & `invokelint-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 
 You can choose which dev tool you'll install, this package doesn't force to install each of dev tools. It helps you to avoid conflicts or breaking your project's dependencies.
 
 Supporting tools:
 
 Linters:
 
+- [Xenon]
 - [Ruff]
 - [Bandit]
 - [dodgy]
 - [Flake8]
 - [pydocstyle]
-- [Xenon]
-- [Pylint]
 - [mypy]
+- [Pylint]
 - [Semgrep]
 
 Formatters:
 
 - [docformatter]
 - [isort]
 - [autoflake]
@@ -66,52 +66,52 @@
 
 This doesn't pollute your comfortable namespaces of command line tools. Thanks to [Invoke], you can place commands into your selected namespace. (See: [Quickstart](#quickstart))
 
 ## Representative commands
 
 (Note that the namespaces of following commands can be changed as you like. See: [Quickstart](#quickstart))
 
+### `inv style`
+
+Formats code by following tools at once:
+
+1. [docformatter]
+2. [isort]
+3. [autoflake]
+4. [Black]
+5. [Ruff]
+
+- `inv style --check` can only check.
+- `inv style --ruff` can leave Ruff warnings.
+
 ### `inv lint`
 
 Runs following fast lints at once:
 
-1. [Ruff]
-2. [Bandit]
-3. [dodgy]
-4. [Flake8]
-5. [pydocstyle]
-6. [Xenon]
+1. [Xenon]
+2. [Ruff]
+3. [Bandit]
+4. [dodgy]
+5. [Flake8]
+6. [pydocstyle]
 
 The format task ([described later](#inv-style)) also run before run above lints. You can skip them by `--skip-format` option.
 
 ### `inv lint.deep`
 
 Runs following slow but detailed lints at once:
 
-1. [Pylint]
-2. [mypy]
+1. [mypy]
+2. [Pylint]
 3. [Semgrep]
 
 ### `inv radon`
 
 Reports [radon] both code complexity and maintainability index.
 
-### `inv style`
-
-Formats code by following tools at once:
-
-1. [docformatter]
-2. [isort]
-3. [autoflake]
-4. [Black]
-5. [Ruff] (optional)
-
-* `inv style --check` can only check.
-* `inv style --ruff` can fix Ruff warnings at once.
-
 ### `inv test`
 
 Runs fast tests (which is not marked `@pytest.mark.slow`) by [pytest].
 
 See:
 
 - [How to mark test functions with attributes — pytest documentation]
@@ -154,20 +154,22 @@
 build = "*"
 # Hotfix for Pipenv's Bug:
 # - Pipenv should prioritize more cross-platform sys_platform condition between packages when lock
 #   · Issue #4101 · pypa/pipenv
 #   https://github.com/pypa/pipenv/issues/4101
 colorama = "*"
 coverage = ">=3.5.4"
-dlint = "*"
+# The dlint less than 0.14.0 limits max version of flake8.
+dlint = ">=0.14.0"
 docformatter = {extras = ["tomli"], version = "*"}
 dodgy = "*"
 # Since Pipenv can't lock for too much combinations to attempt lock:
 # pip._vendor.resolvelib.resolvers.ResolutionTooDeep: 2000000
-flake8 = {version = "==4.0.1", markers="python_version >= '3.6'"}
+# The hacking depends flake8 ~=5.0.1 or ~=4.0.1.
+flake8 = {version = "<=6.0.0>=5.0.1,==4.0.1", markers="python_version >= '3.6'"}
 # To use flake8 --radon-show-closures
 flake8-polyfill = "*"
 # Latest hacking depends on legacy version of flake8, and legacy hacking doesn't narrow flake8 version.
 # When unpin hacking, it has possibility to install too legacy version of hacking.
 hacking = {version = ">=5.0.0", markers="python_version >= '3.8'"}
 invokelint = {version = "*", markers="python_version >= '3.7'"}
 isort = "*"
@@ -196,15 +198,15 @@
 ```python
 """Tasks for maintaining the project.
 
 Execute 'invoke --list' for guidance on using Invoke
 """
 from invoke import Collection
 
-from invokelint import _clean, dist, lint, path, style, test
+from invokelint import dist, lint, path, style, test
 
 ns = Collection()
 ns.add_collection(dist)
 ns.add_collection(lint)
 ns.add_collection(path)
 ns.add_collection(style)
 ns.add_collection(test)
@@ -268,8 +270,8 @@
 [pytest]: https://pypi.org/project/pytest/
 [How to mark test functions with attributes — pytest documentation]: https://docs.pytest.org/en/latest/how-to/mark.html
 [Working with custom markers — pytest documentation]: https://docs.pytest.org/en/latest/example/markers.html
 [Coverage.py]: https://pypi.org/project/coverage/
 [build]: https://pypi.org/project/build/
 [Building and Distributing Packages with Setuptools - setuptools latest documentation]: https://setuptools.pypa.io/en/latest/setuptools.html
 [Package Discovery and Namespace Packages - setuptools latest documentation]: https://setuptools.pypa.io/en/latest/userguide/package_discovery.html
-[Constructing namespaces — Invoke documentation]: https://docs.pyinvoke.org/en/latest/concepts/namespaces.html#nesting-collections
+[Constructing namespaces — Invoke documentation]: https://docs.pyinvoke.org/en/latest/concepts/namespaces.html#nesting-collections
```

### Comparing `invokelint-0.7.0/docs/CONTRIBUTING.md` & `invokelint-0.8.0/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `invokelint-0.7.0/invokelint/_clean.py` & `invokelint-0.8.0/invokelint/_clean.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.7.0/invokelint/dist.py` & `invokelint-0.8.0/invokelint/dist.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.7.0/invokelint/lint.py` & `invokelint-0.8.0/invokelint/lint.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,17 +125,20 @@
 @task(
     help={
         "skip_format": "Lints without format style.",
         "ruff": "Leave ruff warnings",
     },
 )
 def fast(context: Context, *, skip_format: bool = False, ruff: bool = False) -> List[Result]:
-    """Runs fast linting (ruff, bandit, dodgy, flake8, pydocstyle, xenon)."""
+    """Runs fast linting (xenon, ruff, bandit, dodgy, flake8, pydocstyle).
+
+    Xenon is prioritized since it effects fundamental coding structure.
+    """
     list_result = [] if skip_format else fmt(context, ruff=ruff)
-    tasks = [call_ruff, call_bandit, call_dodgy, call_flake8, call_pydocstyle, call_xenon]
+    tasks = [call_xenon, call_ruff, call_bandit, call_dodgy, call_flake8, call_pydocstyle]
     list_result.extend(run_in_order(tasks, context))
     return list_result
 
 
 ns.add_task(ruff_task)
 ns.add_task(bandit)
 ns.add_task(dodgy)
```

### Comparing `invokelint-0.7.0/invokelint/path/__init__.py` & `invokelint-0.8.0/invokelint/path/__init__.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.7.0/invokelint/path/filter_duplication.py` & `invokelint-0.8.0/invokelint/path/filter_duplication.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.7.0/invokelint/path/setuptools.py` & `invokelint-0.8.0/invokelint/path/setuptools.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.7.0/invokelint/ruff.py` & `invokelint-0.8.0/invokelint/ruff.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.7.0/invokelint/run.py` & `invokelint-0.8.0/invokelint/run.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.7.0/invokelint/style.py` & `invokelint-0.8.0/invokelint/style.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.7.0/invokelint/test.py` & `invokelint-0.8.0/invokelint/test.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.7.0/invokelint.egg-info/PKG-INFO` & `invokelint-0.8.0/invokelint.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invokelint
-Version: 0.7.0
+Version: 0.8.0
 Summary: Invokes Python dev tools at once.
 Author-email: Yukihiko Shinoda <yuk.hik.future@gmail.com>
 Maintainer-email: Yukihiko Shinoda <yuk.hik.future@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yukihiko Shinoda
         
@@ -83,22 +83,22 @@
 
 You can choose which dev tool you'll install, this package doesn't force to install each of dev tools. It helps you to avoid conflicts or breaking your project's dependencies.
 
 Supporting tools:
 
 Linters:
 
+- [Xenon]
 - [Ruff]
 - [Bandit]
 - [dodgy]
 - [Flake8]
 - [pydocstyle]
-- [Xenon]
-- [Pylint]
 - [mypy]
+- [Pylint]
 - [Semgrep]
 
 Formatters:
 
 - [docformatter]
 - [isort]
 - [autoflake]
@@ -124,52 +124,52 @@
 
 This doesn't pollute your comfortable namespaces of command line tools. Thanks to [Invoke], you can place commands into your selected namespace. (See: [Quickstart](#quickstart))
 
 ## Representative commands
 
 (Note that the namespaces of following commands can be changed as you like. See: [Quickstart](#quickstart))
 
+### `inv style`
+
+Formats code by following tools at once:
+
+1. [docformatter]
+2. [isort]
+3. [autoflake]
+4. [Black]
+5. [Ruff]
+
+- `inv style --check` can only check.
+- `inv style --ruff` can leave Ruff warnings.
+
 ### `inv lint`
 
 Runs following fast lints at once:
 
-1. [Ruff]
-2. [Bandit]
-3. [dodgy]
-4. [Flake8]
-5. [pydocstyle]
-6. [Xenon]
+1. [Xenon]
+2. [Ruff]
+3. [Bandit]
+4. [dodgy]
+5. [Flake8]
+6. [pydocstyle]
 
 The format task ([described later](#inv-style)) also run before run above lints. You can skip them by `--skip-format` option.
 
 ### `inv lint.deep`
 
 Runs following slow but detailed lints at once:
 
-1. [Pylint]
-2. [mypy]
+1. [mypy]
+2. [Pylint]
 3. [Semgrep]
 
 ### `inv radon`
 
 Reports [radon] both code complexity and maintainability index.
 
-### `inv style`
-
-Formats code by following tools at once:
-
-1. [docformatter]
-2. [isort]
-3. [autoflake]
-4. [Black]
-5. [Ruff] (optional)
-
-* `inv style --check` can only check.
-* `inv style --ruff` can fix Ruff warnings at once.
-
 ### `inv test`
 
 Runs fast tests (which is not marked `@pytest.mark.slow`) by [pytest].
 
 See:
 
 - [How to mark test functions with attributes — pytest documentation]
@@ -212,20 +212,22 @@
 build = "*"
 # Hotfix for Pipenv's Bug:
 # - Pipenv should prioritize more cross-platform sys_platform condition between packages when lock
 #   · Issue #4101 · pypa/pipenv
 #   https://github.com/pypa/pipenv/issues/4101
 colorama = "*"
 coverage = ">=3.5.4"
-dlint = "*"
+# The dlint less than 0.14.0 limits max version of flake8.
+dlint = ">=0.14.0"
 docformatter = {extras = ["tomli"], version = "*"}
 dodgy = "*"
 # Since Pipenv can't lock for too much combinations to attempt lock:
 # pip._vendor.resolvelib.resolvers.ResolutionTooDeep: 2000000
-flake8 = {version = "==4.0.1", markers="python_version >= '3.6'"}
+# The hacking depends flake8 ~=5.0.1 or ~=4.0.1.
+flake8 = {version = "<=6.0.0>=5.0.1,==4.0.1", markers="python_version >= '3.6'"}
 # To use flake8 --radon-show-closures
 flake8-polyfill = "*"
 # Latest hacking depends on legacy version of flake8, and legacy hacking doesn't narrow flake8 version.
 # When unpin hacking, it has possibility to install too legacy version of hacking.
 hacking = {version = ">=5.0.0", markers="python_version >= '3.8'"}
 invokelint = {version = "*", markers="python_version >= '3.7'"}
 isort = "*"
@@ -254,15 +256,15 @@
 ```python
 """Tasks for maintaining the project.
 
 Execute 'invoke --list' for guidance on using Invoke
 """
 from invoke import Collection
 
-from invokelint import _clean, dist, lint, path, style, test
+from invokelint import dist, lint, path, style, test
 
 ns = Collection()
 ns.add_collection(dist)
 ns.add_collection(lint)
 ns.add_collection(path)
 ns.add_collection(style)
 ns.add_collection(test)
```

### Comparing `invokelint-0.7.0/invokelint.egg-info/SOURCES.txt` & `invokelint-0.8.0/invokelint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invokelint-0.7.0/pyproject.toml` & `invokelint-0.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "invokelint"
-version = "0.7.0"
+version = "0.8.0"
 description = "Invokes Python dev tools at once."
 readme = "README.md"
 # Dependency: setuptools>=61.0.0 requires Python 3.7
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = [
     "autoflake",
@@ -75,14 +75,20 @@
 # documentation = "https://readthedocs.org"
 repository = "https://github.com/yukihiko-shinoda/invoke-lint"
 # changelog = "https://github.com/me/spam/blob/master/CHANGELOG.md"
 
 [tool.setuptools]
 zip-safe = false
 
+[tool.bandit.assert_used]
+skips = [
+    "*_test.py",
+    "*/test_*.py",
+]
+
 # @see https://black.readthedocs.io/en/stable/pyproject_toml.html#configuration-format
 [tool.black]
 line-length = 119
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
@@ -219,8 +225,19 @@
     "RUF",  # Ruff-specific rules
 ]
 ignore = [
     "UP032",  # [*] Use f-string instead of `format` call
     "ANN101",  # Missing type annotation for `self` in method
     "ANN401",  # Dynamically typed expressions (typing.Any) are disallowed, These warnings are disabled by default
 ]
+fixable = [
+    "COM812",  # Trailing comma missing
+    "PT001",  # Use `@pytest.fixture()` over `@pytest.fixture`
+    "PT006",  # Wrong name(s) type in `@pytest.mark.parametrize`, expected `tuple`
+    "SIM108",  # Use ternary operator `extra_context = {} if extra_context is None else request.param` instead of `if`-`else`-block
+    "UP015",  # Unnecessary open mode parameters
+    "UP037",  # Remove quotes from type annotation
+]
 target-version = "py37"
+
+[tool.ruff.per-file-ignores]
+"tests/*" = ["S101"]
```

### Comparing `invokelint-0.7.0/tests/test__clean.py` & `invokelint-0.8.0/tests/test__clean.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.7.0/tests/test_dist.py` & `invokelint-0.8.0/tests/test_dist.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.7.0/tests/test_lint.py` & `invokelint-0.8.0/tests/test_lint.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,20 +92,20 @@
 
 
 def test_xenon(context: "Context") -> None:
     check_result(xenon(context), COMMAND_EXPECTED_XENON)
 
 
 LIST_COMMAND_EXPECTED = [
+    COMMAND_EXPECTED_XENON,
     COMMAND_EXPECTED_RUFF,
     COMMAND_EXPECTED_BANDIT,
     COMMAND_EXPECTED_DODGY,
     COMMAND_EXPECTED_FLAKE8,
     COMMAND_EXPECTED_PYDOCSTYLE,
-    COMMAND_EXPECTED_XENON,
 ]
 
 
 def test_fast(context: "Context") -> None:
     """Command should success and run appropriate commands."""
     list_result = fast(context)
     check_list_result(list_result, LIST_COMMAND_EXPECTED_STYLE + LIST_COMMAND_EXPECTED)
@@ -132,17 +132,17 @@
 def test_pylint(context: "Context") -> None:
     check_result(pylint(context), COMMAND_EXPECTED_PYLINT)
 
 
 @pytest.mark.slow()
 # - semgrep does not work on windows 10 · Issue #4295 · returntocorp/semgrep
 #   https://github.com/returntocorp/semgrep/issues/4295
-# - No module found: resource (ModuelNotFoundError) · Issue #7146 · returntocorp/semgrep
+# - No module found: resource (ModuleNotFoundError) · Issue #7146 · returntocorp/semgrep
 #   https://github.com/returntocorp/semgrep/issues/7146
-@pytest.mark.skipif(sys.platform == "win32", reason="Semgrep deosn't support Windows.")
+@pytest.mark.skipif(sys.platform == "win32", reason="Semgrep doesn't support Windows.")
 def test_semgrep(context: "Context") -> None:
     """Command should success and run appropriate commands."""
     check_result(semgrep(context), COMMAND_EXPECTED_SEMGREP)
 
 
 @pytest.mark.slow()
 def test_deep(context: "Context") -> None:
```

### Comparing `invokelint-0.7.0/tests/test_run.py` & `invokelint-0.8.0/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.7.0/tests/test_style.py` & `invokelint-0.8.0/tests/test_style.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.7.0/tests/test_test.py` & `invokelint-0.8.0/tests/test_test.py`

 * *Files identical despite different names*

