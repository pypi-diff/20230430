# Comparing `tmp/poetry_plugin_pypi_mirror-0.3.0.tar.gz` & `tmp/poetry_plugin_pypi_mirror-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_pypi_mirror-0.3.0.tar", max compression
+gzip compressed data, was "poetry_plugin_pypi_mirror-0.3.1.tar", max compression
```

## Comparing `poetry_plugin_pypi_mirror-0.3.0.tar` & `poetry_plugin_pypi_mirror-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1457 2022-10-14 12:19:46.140089 poetry_plugin_pypi_mirror-0.3.0/LICENSE
--rw-r--r--   0        0        0     3180 2022-12-10 18:39:48.379582 poetry_plugin_pypi_mirror-0.3.0/README.md
--rw-r--r--   0        0        0     1126 2022-12-10 18:42:29.205101 poetry_plugin_pypi_mirror-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-04 03:47:49.589982 poetry_plugin_pypi_mirror-0.3.0/src/poetry_plugin_pypi_mirror/__init__.py
--rw-r--r--   0        0        0     4559 2022-12-10 18:39:48.382582 poetry_plugin_pypi_mirror-0.3.0/src/poetry_plugin_pypi_mirror/plugins.py
--rw-r--r--   0        0        0       48 2022-10-04 03:47:49.588982 poetry_plugin_pypi_mirror-0.3.0/src/poetry_plugin_pypi_mirror/py.typed
--rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 poetry_plugin_pypi_mirror-0.3.0/setup.py
--rw-r--r--   0        0        0     4046 1970-01-01 00:00:00.000000 poetry_plugin_pypi_mirror-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1457 2022-10-23 17:58:22.833789 poetry_plugin_pypi_mirror-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3180 2023-04-30 21:13:13.233149 poetry_plugin_pypi_mirror-0.3.1/README.md
+-rw-r--r--   0        0        0     1133 2023-04-30 21:13:36.699871 poetry_plugin_pypi_mirror-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-10-23 17:58:22.833789 poetry_plugin_pypi_mirror-0.3.1/src/poetry_plugin_pypi_mirror/__init__.py
+-rw-r--r--   0        0        0     4559 2023-04-30 20:53:03.808326 poetry_plugin_pypi_mirror-0.3.1/src/poetry_plugin_pypi_mirror/plugins.py
+-rw-r--r--   0        0        0       48 2022-10-23 17:58:22.833789 poetry_plugin_pypi_mirror-0.3.1/src/poetry_plugin_pypi_mirror/py.typed
+-rw-r--r--   0        0        0     4042 1970-01-01 00:00:00.000000 poetry_plugin_pypi_mirror-0.3.1/PKG-INFO
```

### Comparing `poetry_plugin_pypi_mirror-0.3.0/LICENSE` & `poetry_plugin_pypi_mirror-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_mirror-0.3.0/README.md` & `poetry_plugin_pypi_mirror-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -66,13 +66,13 @@
 
 *poetry-plugin-pypi-mirror* depends on poetry internals which can change between
 poetry releases. It's important to ensure compatibility between the poetry
 version in use and the plugin version in use.
 
 | Poetry version(s) | Compatible plugin version(s) |
 |-------------------|------------------------------|
-| ~1.3.0            | ^0.3.0                       |
+| >= 1.3, < 1.5     | ^0.3.1                       |
 | ~1.2.1            | < 0.3.0                      |
 
 ## See also
 
 * [python-poetry/poetry#1632](https://github.com/python-poetry/poetry/issues/1632) - poetry feature request to add support for global repository URL replacement
```

### Comparing `poetry_plugin_pypi_mirror-0.3.0/pyproject.toml` & `poetry_plugin_pypi_mirror-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "poetry-plugin-pypi-mirror"
-version = "0.3.0"
+version = "0.3.1"
 description = "Poetry plugin that adds support for pypi.org mirrors and pull-through caches"
 authors = ["Jacob Henner <code@ventricle.us>"]
 license = "BSD-3-Clause"
 keywords = ["packaging", "poetry", "pypi"]
 readme = "README.md"
 homepage = "https://github.com/arcesium/poetry-plugin-pypi-mirror"
 repository = "https://github.com/arcesium/poetry-plugin-pypi-mirror"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-poetry = "~1.3.0"
+poetry = ">= 1.3, < 1.5"
 
 [tool.poetry.plugins."poetry.plugin"]
 demo = "poetry_plugin_pypi_mirror.plugins:PyPIMirrorPlugin"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 mypy = "^0.991"
```

### Comparing `poetry_plugin_pypi_mirror-0.3.0/src/poetry_plugin_pypi_mirror/plugins.py` & `poetry_plugin_pypi_mirror-0.3.1/src/poetry_plugin_pypi_mirror/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_mirror-0.3.0/setup.py` & `poetry_plugin_pypi_mirror-0.3.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,100 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: poetry-plugin-pypi-mirror
+Version: 0.3.1
+Summary: Poetry plugin that adds support for pypi.org mirrors and pull-through caches
+Home-page: https://github.com/arcesium/poetry-plugin-pypi-mirror
+License: BSD-3-Clause
+Keywords: packaging,poetry,pypi
+Author: Jacob Henner
+Author-email: code@ventricle.us
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: poetry (>=1.3,<1.5)
+Project-URL: Repository, https://github.com/arcesium/poetry-plugin-pypi-mirror
+Description-Content-Type: text/markdown
+
+# poetry-plugin-pypi-mirror
+
+## Description
+
+*poetry-plugin-pypi-mirror* is a
+[plugin](https://python-poetry.org/docs/master/plugins/) for
+[poetry](https://python-poetry.org/), the Python packaging and dependency
+manager. It enables poetry to substitute connections to pypi.org with
+connections to a pypi.org mirror or pull-through cache **without requiring
+project configuration changes**. This is ideal for situations where an
+access-restricted or otherwise unsuitable-for-general-use pypi.org mirror must
+be used by a subset of project contributors. For example:
+
+* A private PyPI mirror internal to a business, required by company policy
+* A limited-access PyPI mirror in a region where pypi.org is restricted
+* A regional mirror that is more performant for a few users, and less performant
+  for everyone else
+
+These mirrors can be used without this plugin by [adding them as project
+repositories](https://python-poetry.org/docs/repositories/). However, this
+requires the mirror to be included in the project's configuration, and this also
+results in source entries for the mirror appearing in `poetry.lock`. Since only
+a subset of project contributors can use these mirrors, that subset of users
+would need to replace and remove references to the mirror repository each time
+they want to contribute their changes back to the project. This is suboptimal.
+
+## Usage
+
+### Installation
+
+Follow poetry's [plugin installation instructions](https://python-poetry.org/docs/master/plugins/#using-plugins), replacing `poetry-plugin` with `poetry-plugin-pypi-mirror`.
+
+### Specifying a mirror
+
+To specify a mirror, you can either define `plugins.pypi_mirror.url` in poetry's
+[configuration](https://python-poetry.org/docs/configuration/), or set
+environment variable `POETRY_PYPI_MIRROR_URL` to the full URL for a [PEP
+503](https://peps.python.org/pep-0503/)-compatible mirror. When both are set the
+environment variable will be used.
+
+#### Poetry config example
+
+```toml
+[plugins]
+[plugins.pypi_mirror]
+url = "https://example.org/repository/pypi-proxy/simple/"
+```
+
+... in [either](https://python-poetry.org/docs/configuration/) a project's
+`poetry.toml` (for per-project configuration), or the user's `config.toml`.
+
+#### Environment variable example
+
+```shell
+POETRY_PYPI_MIRROR_URL=https://example.org/repository/pypi-proxy/simple/ poetry add pendulum
+```
+...or...
+
+```shell
+export POETRY_PYPI_MIRROR_URL=https://example.org/repository/pypi-proxy/simple/
+poetry add cleo # uses mirror specified in first line
+poetry lock     # also uses mirror specified in first line
+```
+
+## Compatibility
+
+*poetry-plugin-pypi-mirror* depends on poetry internals which can change between
+poetry releases. It's important to ensure compatibility between the poetry
+version in use and the plugin version in use.
+
+| Poetry version(s) | Compatible plugin version(s) |
+|-------------------|------------------------------|
+| >= 1.3, < 1.5     | ^0.3.1                       |
+| ~1.2.1            | < 0.3.0                      |
 
-package_dir = \
-{'': 'src'}
+## See also
 
-packages = \
-['poetry_plugin_pypi_mirror']
+* [python-poetry/poetry#1632](https://github.com/python-poetry/poetry/issues/1632) - poetry feature request to add support for global repository URL replacement
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['poetry>=1.3.0,<1.4.0']
-
-entry_points = \
-{'poetry.plugin': ['demo = poetry_plugin_pypi_mirror.plugins:PyPIMirrorPlugin']}
-
-setup_kwargs = {
-    'name': 'poetry-plugin-pypi-mirror',
-    'version': '0.3.0',
-    'description': 'Poetry plugin that adds support for pypi.org mirrors and pull-through caches',
-    'long_description': '# poetry-plugin-pypi-mirror\n\n## Description\n\n*poetry-plugin-pypi-mirror* is a\n[plugin](https://python-poetry.org/docs/master/plugins/) for\n[poetry](https://python-poetry.org/), the Python packaging and dependency\nmanager. It enables poetry to substitute connections to pypi.org with\nconnections to a pypi.org mirror or pull-through cache **without requiring\nproject configuration changes**. This is ideal for situations where an\naccess-restricted or otherwise unsuitable-for-general-use pypi.org mirror must\nbe used by a subset of project contributors. For example:\n\n* A private PyPI mirror internal to a business, required by company policy\n* A limited-access PyPI mirror in a region where pypi.org is restricted\n* A regional mirror that is more performant for a few users, and less performant\n  for everyone else\n\nThese mirrors can be used without this plugin by [adding them as project\nrepositories](https://python-poetry.org/docs/repositories/). However, this\nrequires the mirror to be included in the project\'s configuration, and this also\nresults in source entries for the mirror appearing in `poetry.lock`. Since only\na subset of project contributors can use these mirrors, that subset of users\nwould need to replace and remove references to the mirror repository each time\nthey want to contribute their changes back to the project. This is suboptimal.\n\n## Usage\n\n### Installation\n\nFollow poetry\'s [plugin installation instructions](https://python-poetry.org/docs/master/plugins/#using-plugins), replacing `poetry-plugin` with `poetry-plugin-pypi-mirror`.\n\n### Specifying a mirror\n\nTo specify a mirror, you can either define `plugins.pypi_mirror.url` in poetry\'s\n[configuration](https://python-poetry.org/docs/configuration/), or set\nenvironment variable `POETRY_PYPI_MIRROR_URL` to the full URL for a [PEP\n503](https://peps.python.org/pep-0503/)-compatible mirror. When both are set the\nenvironment variable will be used.\n\n#### Poetry config example\n\n```toml\n[plugins]\n[plugins.pypi_mirror]\nurl = "https://example.org/repository/pypi-proxy/simple/"\n```\n\n... in [either](https://python-poetry.org/docs/configuration/) a project\'s\n`poetry.toml` (for per-project configuration), or the user\'s `config.toml`.\n\n#### Environment variable example\n\n```shell\nPOETRY_PYPI_MIRROR_URL=https://example.org/repository/pypi-proxy/simple/ poetry add pendulum\n```\n...or...\n\n```shell\nexport POETRY_PYPI_MIRROR_URL=https://example.org/repository/pypi-proxy/simple/\npoetry add cleo # uses mirror specified in first line\npoetry lock     # also uses mirror specified in first line\n```\n\n## Compatibility\n\n*poetry-plugin-pypi-mirror* depends on poetry internals which can change between\npoetry releases. It\'s important to ensure compatibility between the poetry\nversion in use and the plugin version in use.\n\n| Poetry version(s) | Compatible plugin version(s) |\n|-------------------|------------------------------|\n| ~1.3.0            | ^0.3.0                       |\n| ~1.2.1            | < 0.3.0                      |\n\n## See also\n\n* [python-poetry/poetry#1632](https://github.com/python-poetry/poetry/issues/1632) - poetry feature request to add support for global repository URL replacement\n',
-    'author': 'Jacob Henner',
-    'author_email': 'code@ventricle.us',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/arcesium/poetry-plugin-pypi-mirror',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

