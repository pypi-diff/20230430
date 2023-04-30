# Comparing `tmp/poetry_git_version_plugin-0.1.3.tar.gz` & `tmp/poetry_git_version_plugin-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_git_version_plugin-0.1.3.tar", max compression
+gzip compressed data, was "poetry_git_version_plugin-0.1.4.tar", max compression
```

## Comparing `poetry_git_version_plugin-0.1.3.tar` & `poetry_git_version_plugin-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1055 2023-04-16 19:45:04.526406 poetry_git_version_plugin-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2023-04-18 08:53:02.585461 poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/__init__.py
--rw-r--r--   0        0        0      310 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/commands.py
--rw-r--r--   0        0        0     1250 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/config.py
--rw-r--r--   0        0        0      758 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/exceptions.py
--rw-r--r--   0        0        0     1461 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/plugins.py
--rw-r--r--   0        0        0     4506 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/services.py
--rw-r--r--   0        0        0     2509 2023-04-18 08:29:46.694155 poetry_git_version_plugin-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1248 2023-04-16 19:55:03.123301 poetry_git_version_plugin-0.1.3/readme.md
--rw-r--r--   0        0        0     2844 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-04-30 18:01:24.998022 poetry_git_version_plugin-0.1.4/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-30 18:01:25.074022 poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/__init__.py
+-rw-r--r--   0        0        0      310 2023-04-16 20:16:12.153636 poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/commands.py
+-rw-r--r--   0        0        0     1651 2023-04-30 18:01:24.998022 poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/config.py
+-rw-r--r--   0        0        0      758 2023-04-16 20:16:12.153636 poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/exceptions.py
+-rw-r--r--   0        0        0     1550 2023-04-30 18:01:24.998022 poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/plugins.py
+-rw-r--r--   0        0        0     5240 2023-04-30 18:01:24.998022 poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/services.py
+-rw-r--r--   0        0        0     2837 2023-04-30 18:01:24.998022 poetry_git_version_plugin-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1639 2023-04-30 18:01:24.998022 poetry_git_version_plugin-0.1.4/readme.md
+-rw-r--r--   0        0        0     3235 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.4/PKG-INFO
```

### Comparing `poetry_git_version_plugin-0.1.3/LICENSE` & `poetry_git_version_plugin-0.1.4/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 Copyright (c) 2022 rocshers.com
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/config.py` & `poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,23 @@
     """Обертка над конфигурацией pyproject"""
 
     pyproject: PyProjectTOML
 
     _default_setting = {
         # Игнорирование отсутствия тега
         'ignore_errors': True,
-        # Использование ref без тега
+        # При отсутствии тега генерировать alpha version
         'make_alpha_version': True,
-        # Использование ref без тега
-        'format_alpha_version': '{version}.a{distance}+{commit_hash}',
+        # Alpha Version Format
+        'alpha_version_format': '{version}a{distance}',
+        # 'alpha_version_format': '{version}a{distance}+{commit_hash}',
+        # Ignore PEP440
+        'ignore_pep440': True,
+        # Ignore public format PEP440
+        'ignore_public_pep440': True,
     }
 
     def __init__(self, pyproject: PyProjectTOML) -> None:
         self.pyproject = pyproject
 
     @property
     def settings(self):
@@ -34,9 +39,17 @@
         return self.settings['ignore_errors']
 
     @property
     def make_alpha_version(self) -> bool:
         return self.settings['make_alpha_version']
 
     @property
-    def format_alpha_version(self) -> str:
-        return self.settings['format_alpha_version']
+    def alpha_version_format(self) -> str:
+        return self.settings['alpha_version_format']
+
+    @property
+    def ignore_pep440(self) -> bool:
+        return self.settings['ignore_pep440']
+
+    @property
+    def ignore_public_pep440(self) -> bool:
+        return self.settings['ignore_public_pep440']
```

### Comparing `poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/exceptions.py` & `poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/plugins.py` & `poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/plugins.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,39 +6,39 @@
 from poetry.plugins.plugin import Plugin
 from poetry.poetry import Poetry
 
 from poetry_git_version_plugin import config
 from poetry_git_version_plugin.commands import GitVersionCommand
 from poetry_git_version_plugin.exceptions import PluginException, plugin_exception_wrapper
 from poetry_git_version_plugin.services import GitVersionService
+from poetry.core.constraints.version import Version
 
 
 class PoetryGitVersionPlugin(Plugin):
     """Плагин определения версии по гит тегу"""
 
     @plugin_exception_wrapper
     def activate(self, poetry: Poetry, io: IO):
         io.write_line(f'<b>{config.PLUGIN_NAME}</b>: Init', Verbosity.VERBOSE)
 
         plugin_config = config.PluginConfig(poetry.pyproject)
 
         try:
-            tag = GitVersionService(io, plugin_config).get_version()
+            version = GitVersionService(io, plugin_config).get_version()
+            poetry.package.version = Version.parse(version)
 
         except Exception as ex:
             if plugin_config.ignore_errors:
                 if not isinstance(ex, PluginException):
                     ex = PluginException(ex)
 
-                io.write_error(f'{ex}. Ignore Exception\n', Verbosity.VERBOSE)
+                io.write_error_line(f'{ex}. Ignore Exception\n', Verbosity.VERBOSE)
 
                 return
 
             raise ex
 
-        poetry.package.version = tag
-
-        io.write_line(f'<b>{config.PLUGIN_NAME}</b>: Finished\n', Verbosity.VERBOSE)
+        io.write_error_line(f'<b>{config.PLUGIN_NAME}</b>: Finished\n', Verbosity.VERBOSE)
 
 
 class PoetryGitVersionApplicationPlugin(ApplicationPlugin):
     commands = [GitVersionCommand]
```

### Comparing `poetry_git_version_plugin-0.1.3/poetry_git_version_plugin/services.py` & `poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/services.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,94 +1,92 @@
 import re
 from pathlib import Path
-from typing import Callable, List
+from typing import List, Optional
 
 import git
+from git.objects import Commit
 from cleo.io.io import IO
 from cleo.io.outputs.output import Verbosity
 from packaging.version import VERSION_PATTERN
 
 from poetry_git_version_plugin import config
 from poetry_git_version_plugin.exceptions import PluginException
 
 VERSION_REGEX_COMPILE = re.compile(r'^\s*' + VERSION_PATTERN + r'\s*$', re.VERBOSE | re.IGNORECASE)
+VERSION_CANON_REGEX_COMPILE = re.compile(
+    r'^([1-9][0-9]*!)?(0|[1-9][0-9]*)(\.(0|[1-9][0-9]*))*((a|b|rc)(0|[1-9][0-9]*))?(\.post(0|[1-9][0-9]*))?(\.dev(0|[1-9][0-9]*))?$'
+)
 
 
 def validate_version(version_string: str):
-    """Проверка версии на PEP 440
-
-    Копипаст метода: from poetry.core.version.pep440.parser import parse_pep440
+    """Проверка версии на PEP440
 
     Args:
         version_string (str): Версия
 
     Raises:
         PluginException: Версия не соответствует стандарту
 
     """
 
     if VERSION_REGEX_COMPILE.search(version_string) is None:
-        raise PluginException(f'Invalid PEP 440 version: "{version_string}"')
-
+        return 1
 
-def validate_version_decorator(func: Callable):
-    def inner(*args, **kwargs):
-        version = func(*args, **kwargs)
-        validate_version(version)
-        return version
+    if VERSION_CANON_REGEX_COMPILE.search(version_string) is None:
+        return 2
 
-    return inner
+    return 0
 
 
 class GitService(object):
     repo: git.Repo
 
     def __init__(self) -> None:
         path = Path.cwd()
         self.repo = git.Repo(path, search_parent_directories=True)
 
     @property
-    def commits(self) -> List[git.Commit]:
+    def commits(self) -> List[Commit]:
         return list(self.repo.iter_commits())
 
     @property
-    def current_commit(self) -> git.Commit:
+    def current_commit(self) -> Commit:
         return self.repo.head.commit
 
     @property
     def tags(self) -> List[git.Tag]:
         return list(self.repo.tags)[::-1]
 
-    def get_git_current_tag(self) -> git.Tag:
+    def get_current_tag(self) -> Optional[git.Tag]:
         """Получение тега нынешнего коммита"""
 
         tags = list(self.repo.tags)[::-1]
 
         for tag in tags:
             if tag.commit == self.repo.head.commit:
                 return tag
 
         return None
 
-    def get_alpha_version(self) -> git.Tag:
+    def get_last_tag(self) -> Optional[git.Tag]:
         """Получение последнего тега нынешней ветки"""
 
         commits = set(self.commits)
         tags = self.tags
 
         for tag in tags:
             if tag.commit in commits:
                 return tag
 
         return None
 
     def get_current_short_rev(self) -> str:
         return self.current_commit.name_rev[:7]
 
-    def get_distance(self, from_commit: git.Commit, to_commit: git.Commit) -> int:
+    def get_distance(self, from_commit: Commit, to_commit: Commit) -> int:
         return len(list(self.repo.iter_commits(f'{from_commit}..{to_commit}')))
 
 
 class GitVersionService(object):
     io: IO
     plugin_config: config.PluginConfig
 
@@ -97,41 +95,40 @@
     def __init__(self, io: IO, plugin_config: config.PluginConfig) -> None:
         self.io = io
         self.plugin_config = plugin_config
 
         self.git_service = GitService()
 
     def construct_alpha_version(self, version: str, distance: str, commit_hash: str):
-        return self.plugin_config.format_alpha_version.format(
+        return self.plugin_config.alpha_version_format.format(
             version=version,
             distance=distance,
             commit_hash=commit_hash,
         )
 
-    def get_main_version(self) -> str:
-        tag = self.git_service.get_git_current_tag()
+    def get_main_version(self) -> Optional[str]:
+        tag = self.git_service.get_current_tag()
         return tag.name if tag is not None else None
 
     def get_alpha_version(self):
-        tag = self.git_service.get_alpha_version()
+        tag = self.git_service.get_last_tag()
 
         version = '0.0.0'
         distance_from_commit = self.git_service.commits[-1]
 
         if tag is not None:
             distance_from_commit = tag.commit
             version = str(tag)
 
         distance = self.git_service.get_distance(distance_from_commit, self.git_service.current_commit)
         commit_hash = self.git_service.get_current_short_rev()
 
         return self.construct_alpha_version(version, distance, commit_hash)
 
-    @validate_version_decorator
-    def get_version(self) -> str:
+    def __get_version(self) -> str:
         self.io.write(f'<b>{config.PLUGIN_NAME}</b>: Find git <b>current tag</b>... ', verbosity=Verbosity.VERBOSE)
 
         version = self.get_main_version()
 
         if version is not None:
             self.io.write_line(f'success, setting dynamic version to: {version}', Verbosity.VERBOSE)
             return version
@@ -139,12 +136,37 @@
         self.io.write_line('fail', Verbosity.VERBOSE)
 
         if not self.plugin_config.make_alpha_version:
             raise PluginException('No Git version found, not extracting dynamic version')
 
         self.io.write(f'<b>{config.PLUGIN_NAME}</b>: Make <b>alpha version</b>... ', verbosity=Verbosity.VERBOSE)
 
-        tag = self.get_alpha_version()
+        version = self.get_alpha_version()
+
+        self.io.write_line(f'success, setting dynamic version to: {version}', Verbosity.VERBOSE)
 
-        self.io.write_line(f'success, setting dynamic version to: {tag}', Verbosity.VERBOSE)
+        return version
+
+    def validate_version(self, version: str):
+        is_valid = validate_version(version)
+
+        if is_valid == 0:
+            return version
 
-        return tag
+        if is_valid == 1:
+            self.io.write_line(f'Invalid PEP440 version: "{version}"', Verbosity.VERBOSE)
+
+            if not self.plugin_config.ignore_pep440:
+                raise PluginException(f'Invalid PEP440 version: "{version}"')
+
+        if is_valid == 2:
+            self.io.write_line(f'Invalid public PEP440 version: "{version}"', Verbosity.VERBOSE)
+
+            if not self.plugin_config.ignore_public_pep440:
+                raise PluginException(f'Invalid public PEP440 version: "{version}"')
+
+    def get_version(self) -> str:
+        version = self.__get_version()
+
+        self.validate_version(version)
+
+        return version
```

### Comparing `poetry_git_version_plugin-0.1.3/pyproject.toml` & `poetry_git_version_plugin-0.1.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 ruff = "^0.0.260"
 black = "^23.3.0"
 isort = "^5.12.0"
+pre-commit = "^3.2.2"
+mypy = "^1.2.0"
 
 [tool.black]
 skip-string-normalization = true
 line-length = 120
 
 [tool.isort]
 profile = "black"
@@ -78,8 +80,24 @@
     "def __repr__",
     "raise AssertionError",
     "raise NotImplementedError",
     "if __name__ == .__main__.:",
 ]
 
 [tool.poetry-git-version-plugin]
-ignore_errors = false
+ignore_errors = false
+
+[tool.pytest.ini_options]
+addopts = "-vvs --tb=short"
+xfail_strict = true
+testpaths = [
+    "tests",
+    "integration",
+]
+python_files = [
+    "tests/*.py",
+    "test_*.py"
+]
+filterwarnings = [
+    "ignore::DeprecationWarning",
+    "ignore:Module already imported:pytest.PytestWarning"
+]
```

### Comparing `poetry_git_version_plugin-0.1.3/PKG-INFO` & `poetry_git_version_plugin-0.1.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-git-version-plugin
-Version: 0.1.3
+Version: 0.1.4
 Summary: Poetry plugin to get package version from git
 Home-page: https://gitlab.com/rocshers/python/poetry-git-version-plugin
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -51,37 +51,65 @@
 poetry self add poetry-git-version-plugin
 poetry git-version # Write your git tag
 poetry -v git-version # print process
 ```
 
 ## Dependencies
 
+Installed `Git` and:
+
 ```toml
 [tool.poetry.dependencies]
-python = ">=3.7"
+python = ">=3.8"
 poetry = ">=1.2.0"
 ```
 
 ## Setup
 
 ```toml
 [tool.poetry-git-version-plugin]
-# Ignore "tag missing" errors and other errors
+# If the tag is not found on the HEAD,
+# then the version is built based on the last found tag and the HEAD
+# Example: 1.3.2a5
 # Default = true
-ignore_errors = true
-
-# If the tag is missing.
-# Returns a version, computed from the latest version tag.
-# It takes the version tag, increases the version tag by the number of commits since, adds a local label specifying the git commit hash and the dirty status.
-# Example: 1.3.2+5-5babef6
 make_alpha_version = true
 
 # Format for alpha version
-# Default = '{version}.a{distance}+{commit_hash}'
-format_alpha_version = '{version}+{distance}'
+# Default = '{version}a{distance}'
+# Example:
+alpha_version_format = '{version}+{distance}' # -> 1.3.2a5
+alpha_version_format = '{version}a{distance}+{commit_hash}' # -> 1.3.2a5-5babef6
+# Available variables:
+# - version: Last found tag
+# - distance: Distance from last found tag to HEAD
+# - commit_hash: Commit hash
+
+# Ignore mismatch error PEP440 version format
+# Default = true
+ignore_pep440 = true
+
+# Ignore mismatch error PEP440 public version format
+# Default = true
+ignore_public_pep440 = true
+
+# Ignore all errors
+# including version not found errors
+ignore_errors = true
 ```
 
 ## Contribute
 
 Issue Tracker: <https://gitlab.com/rocshers/python/poetry-git-version-plugin/-/issues>  
 Source Code: <https://gitlab.com/rocshers/python/poetry-git-version-plugin>
 
+Before adding changes:
+
+```bash
+make install
+```
+
+After changes:
+
+```bash
+make format test
+```
+
```

