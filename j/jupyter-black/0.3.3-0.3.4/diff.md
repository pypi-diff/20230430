# Comparing `tmp/jupyter-black-0.3.3.tar.gz` & `tmp/jupyter-black-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-black-0.3.3.tar", last modified: Sun Nov 20 17:34:48 2022, max compression
+gzip compressed data, was "jupyter-black-0.3.4.tar", last modified: Sun Apr 30 01:48:35 2023, max compression
```

## Comparing `jupyter-black-0.3.3.tar` & `jupyter-black-0.3.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-20 17:34:48.452733 jupyter-black-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-20 17:34:48.448733 jupyter-black-0.3.3/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      604 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (122)      650 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (122)      711 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (122)      797 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-20 17:34:48.448733 jupyter-black-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      983 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (122)      578 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)      527 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       35 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/.python-version
--rw-r--r--   0 runner    (1001) docker     (122)      167 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (122)      922 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     3893 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1845 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     6715 2022-11-20 17:34:48.452733 jupyter-black-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5012 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      278 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (122)     1925 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-20 17:34:48.452733 jupyter-black-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-20 17:34:48.444733 jupyter-black-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-20 17:34:48.448733 jupyter-black-0.3.3/src/jupyter_black/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/src/jupyter_black/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7537 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/src/jupyter_black/jupyter_black.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-20 17:34:48.448733 jupyter-black-0.3.3/src/jupyter_black.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6715 2022-11-20 17:34:48.000000 jupyter-black-0.3.3/src/jupyter_black.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      689 2022-11-20 17:34:48.000000 jupyter-black-0.3.3/src/jupyter_black.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-20 17:34:48.000000 jupyter-black-0.3.3/src/jupyter_black.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-20 17:34:21.000000 jupyter-black-0.3.3/src/jupyter_black.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      287 2022-11-20 17:34:48.000000 jupyter-black-0.3.3/src/jupyter_black.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2022-11-20 17:34:48.000000 jupyter-black-0.3.3/src/jupyter_black.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-20 17:34:48.452733 jupyter-black-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    12895 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1182 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/tests/test_jb_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2274 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/tests/test_lab.py
--rw-r--r--   0 runner    (1001) docker     (122)     2665 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/tests/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2022-11-20 17:34:09.000000 jupyter-black-0.3.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:48:35.898817 jupyter-black-0.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:48:35.894817 jupyter-black-0.3.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:48:35.894817 jupyter-black-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/.python-version
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-04-30 01:48:35.898817 jupyter-black-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 01:48:35.898817 jupyter-black-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:48:35.886817 jupyter-black-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:48:35.894817 jupyter-black-0.3.4/src/jupyter_black/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/src/jupyter_black/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/src/jupyter_black/jupyter_black.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:48:35.894817 jupyter-black-0.3.4/src/jupyter_black.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-04-30 01:48:35.000000 jupyter-black-0.3.4/src/jupyter_black.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-30 01:48:35.000000 jupyter-black-0.3.4/src/jupyter_black.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 01:48:35.000000 jupyter-black-0.3.4/src/jupyter_black.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 01:48:14.000000 jupyter-black-0.3.4/src/jupyter_black.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-30 01:48:35.000000 jupyter-black-0.3.4/src/jupyter_black.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-30 01:48:35.000000 jupyter-black-0.3.4/src/jupyter_black.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 01:48:35.898817 jupyter-black-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12896 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/tests/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/tests/test_jb_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/tests/test_lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/tests/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-30 01:48:00.000000 jupyter-black-0.3.4/tox.ini
```

### Comparing `jupyter-black-0.3.3/.github/FUNDING.yml` & `jupyter-black-0.3.4/.github/FUNDING.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # These are supported funding model platforms
 
 github: [n8henrie]
 custom: ["https://n8henrie.com/donate"]
-patreon: # Replace with a single Patreon username
+patreon: n8henrie
 open_collective: # Replace with a single Open Collective username
 ko_fi: # Replace with a single Ko-fi username
 tidelift: # Replace with a single Tidelift platform-name/package-name e.g., npm/babel
 community_bridge: # Replace with a single Community Bridge project-name e.g., cloud-foundry
 liberapay: # Replace with a single Liberapay username
 issuehunt: # Replace with a single IssueHunt username
 otechie: # Replace with a single Otechie username
```

### Comparing `jupyter-black-0.3.3/.github/ISSUE_TEMPLATE.md` & `jupyter-black-0.3.4/.github/ISSUE_TEMPLATE.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 - **Python version**:
 - **jupyter-black version**:
 
 ## My Issue
 
 
 
-## [WHYT](http://mattgemmell.com/what-have-you-tried)
+## [WHYT](https://web.archive.org/web/20140712194323/http://mattgemmell.com/what-have-you-tried/)
 
 
 
 ---
 
 Please make sure you've taken these steps before submitting a new issue:
```

### Comparing `jupyter-black-0.3.3/.github/PULL_REQUEST_TEMPLATE.md` & `jupyter-black-0.3.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `jupyter-black-0.3.3/.github/stale.yml` & `jupyter-black-0.3.4/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `jupyter-black-0.3.3/.gitignore` & `jupyter-black-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter-black-0.3.3/CHANGELOG.md` & `jupyter-black-0.3.4/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # [Changelog](https://keepachangelog.com)
 
+## 0.3.4 :: 2023-04-27
+
+- Only pass to `black.Mode` options from `pyproject.toml` that are valid for
+  `black.Mode`. Thanks @rldotai, https://github.com/n8henrie/jupyter-black/issues/7
+
 ## 0.3.2, 0.3.3 :: 2022-11-20
 
 - Remove version constraints (thanks: @JakobGM, https://github.com/n8henrie/jupyter-black/issues/6)
 - Update CI to ensure publishing should work
 
 ## 0.3.1 :: 2022-03-08
```

### Comparing `jupyter-black-0.3.3/CONTRIBUTING.md` & `jupyter-black-0.3.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyter-black-0.3.3/LICENSE` & `jupyter-black-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-black-0.3.3/Makefile` & `jupyter-black-0.3.4/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter-black-0.3.3/PKG-INFO` & `jupyter-black-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-black
-Version: 0.3.3
+Version: 0.3.4
 Summary: A simple extension for Jupyter Notebook and Jupyter Lab to beautify Python code automatically using Black. Fork of dnanhkhoa/nb_black.
 Author-email: Nathan Henrie <nate@n8henrie.com>
 License: MIT
 Project-URL: homepage, https://github.com/n8henrie/jupyter-black
 Keywords: jupyter-black
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -177,14 +177,19 @@
 
 ## Buy Me a Coffee
 
 [☕️](https://n8henrie.com/donate)
 
 # [Changelog](https://keepachangelog.com)
 
+## 0.3.4 :: 2023-04-27
+
+- Only pass to `black.Mode` options from `pyproject.toml` that are valid for
+  `black.Mode`. Thanks @rldotai, https://github.com/n8henrie/jupyter-black/issues/7
+
 ## 0.3.2, 0.3.3 :: 2022-11-20
 
 - Remove version constraints (thanks: @JakobGM, https://github.com/n8henrie/jupyter-black/issues/6)
 - Update CI to ensure publishing should work
 
 ## 0.3.1 :: 2022-03-08
```

### Comparing `jupyter-black-0.3.3/README.md` & `jupyter-black-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-black-0.3.3/pyproject.toml` & `jupyter-black-0.3.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 follow_imports = "silent"
 ignore_missing_imports = true
-python_version = "3.10"
+python_version = "3.11"
 show_column_numbers = true
 warn_incomplete_stub = false
 warn_redundant_casts = true
 warn_unused_ignores = true
 
 [project]
 name = "jupyter-black"
@@ -44,30 +44,30 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "black >= 21.9b0",
-    "ipython >= 7.27.0",
-    "tokenize_rt >= 4.1.0",
+    "black >= 21",
+    "ipython >= 7",
+    "tokenize_rt >= 4",
 ]
 
 [project.optional-dependencies]
 test = [
-    "flake8 >= 3.9.2",
-    "flake8-docstrings >= 1.6.0",
-    "flake8-import-order >= 0.18.1",
-    "jupyterlab == 3.3.0",
-    "mypy >= 0.910",
-    "pep8-naming >= 0.12.1",
-    "playwright >= 1.14.1",
-    "pylint >= 2.10.2",
-    "pytest >= 6.2.5",
-    "tox >= 3.24.3",
+    "flake8 == 3.9.2",
+    "flake8-docstrings == 1.6.0",
+    "flake8-import-order == 0.18.1",
+    "isort == 5.11.5",
+    "jupyterlab == 3.6.3",
+    "mypy == 1.2.0",
+    "pep8-naming == 0.12.1",
+    "playwright == 1.14.1",
+    "pytest == 7.3.1",
+    "tox == 4.5.1",
 ]
 dev = [
-    "build >= 0.6.0.post1",
-    "twine >= 4.0.1",
-    "wheel >= 0.37.0",
+    "build == 0.9.0",
+    "twine == 4.0.1",
+    "wheel == 0.37.0",
 ]
```

### Comparing `jupyter-black-0.3.3/src/jupyter_black/jupyter_black.py` & `jupyter-black-0.3.4/src/jupyter_black/jupyter_black.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Beautify jupyter cells using black."""
 import json
 import logging
 import typing as t
 
 import black
 from IPython.core import getipython
+from IPython.core.display import HTML, Javascript
 from IPython.core.interactiveshell import ExecutionInfo
-from IPython.display import display, HTML, Javascript
+from IPython.display import display
 from IPython.terminal.interactiveshell import TerminalInteractiveShell as Ipt
 
 logging.basicConfig()
 LOGGER = logging.getLogger("jupyter_black")
 
 formatter = None
 
@@ -45,26 +46,26 @@
             black_config: Dictionary for black config options
         """
         self.shell = ip
 
         if black_config is None:
             black_config = {}
 
-        config = self._config_from_pyproject_toml()
+        mode_config = self._mode_config_from_pyproject_toml()
 
-        tv = config.pop("target_version", None)
+        tv = mode_config.pop("target_version", None)
         if tv is not None:
             versions = {black.TargetVersion[ver.upper()] for ver in tv}
-            config.update({"target_versions": versions})
+            mode_config.update({"target_versions": versions})
 
         # Override with passed-in config
-        config.update(black_config)
+        mode_config.update(black_config)
 
-        LOGGER.debug(f"config: {config}")
-        mode = black.Mode(**config)
+        LOGGER.debug("config: %s", mode_config)
+        mode = black.Mode(**mode_config)
         mode.is_ipynb = True
         self.mode = mode
 
         self.is_lab = is_lab
         if is_lab:
             js_func = """
                 <script type="application/javascript" id="jupyter_black">
@@ -93,38 +94,44 @@
                             return
                         }
                     }
                 }
                 </script>
                 """
         display(
-            HTML(js_func),
+            HTML(js_func),  # type: ignore
             display_id="jupyter_black",
             update=False,
         )
 
     @staticmethod
-    def _config_from_pyproject_toml() -> t.Dict[str, t.Any]:
+    def _mode_config_from_pyproject_toml() -> t.Dict[str, t.Any]:
+        """Return valid options for black.Mode from pyproject.toml."""
         toml_config = black.find_pyproject_toml((".",))
-        if toml_config:
-            LOGGER.debug(f"Using config from {toml_config}")
-            return black.parse_pyproject_toml(toml_config)
-        return {}
+        if not toml_config:
+            return {}
+
+        LOGGER.debug("Using config from %s", toml_config)
+        config = black.parse_pyproject_toml(toml_config)
+        valid_options = set(t.get_type_hints(black.Mode))
+        return {k: v for k, v in config.items() if k in valid_options}
 
     def _set_cell(self, cell_content: str) -> None:
         if self.is_lab:
             self.shell.set_next_input(cell_content, replace=True)
         else:
             js_code = f"""
             (function() {{
                 jb_set_cell({json.dumps(cell_content)})
             }})();
             """
-            display(
-                Javascript(js_code), display_id="jupyter_black", update=True
+            display(  # type: ignore
+                Javascript(js_code),  # type: ignore
+                display_id="jupyter_black",
+                update=True,
             )
 
     def _format_cell(self, cell_info: ExecutionInfo) -> None:
         cell_content = str(cell_info.raw_cell)
 
         try:
             # `fast=False` seems to make *at most* a few ns difference even on
@@ -161,15 +168,15 @@
     js_code = """
     (function(){
         var kernel = IPython.notebook.kernel;
         kernel.execute("jb_test_is_notebook = 1");
         console.log("I ran from javascrIpt");
     })();
     """
-    display(Javascript(js_code))
+    display(Javascript(js_code))  # type: ignore
     print("I ran from python")
 
 
 def load_ipython_extension(
     ip: Ipt,
 ) -> None:
     """Load the extension via `%load_ext jupyter_black`.
@@ -201,30 +208,32 @@
             https://github.com/psf/black/blob/911470a610e47d9da5ea938b0887c3df62819b85/src/black/mode.py#L99
     """
     global formatter
     global LOGGER
     LOGGER.setLevel(verbosity)
 
     if not ip:
-        ip = getipython.get_ipython()
+        ip = getipython.get_ipython()  # type: ignore
     if not ip:
         return
 
     if line_length:
         black_config.update({"line_length": line_length})
     if target_version:
         black_config.update({"target_versions": set([target_version])})
 
     if formatter is None:
         formatter = BlackFormatter(ip, is_lab=lab, black_config=black_config)
-    ip.events.register("pre_run_cell", formatter._format_cell)
+    ip.events.register("pre_run_cell", formatter._format_cell)  # type: ignore
 
 
 def unload_ipython_extension(ip: Ipt) -> None:
     """Unload the extension.
 
     https://ipython.readthedocs.io/en/stable/config/extensions/#writing-extensions
     """
     global formatter
     if formatter:
-        ip.events.unregister("pre_run_cell", formatter._format_cell)
+        ip.events.unregister(  # type: ignore
+            "pre_run_cell", formatter._format_cell
+        )
         formatter = None
```

### Comparing `jupyter-black-0.3.3/src/jupyter_black.egg-info/PKG-INFO` & `jupyter-black-0.3.4/src/jupyter_black.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-black
-Version: 0.3.3
+Version: 0.3.4
 Summary: A simple extension for Jupyter Notebook and Jupyter Lab to beautify Python code automatically using Black. Fork of dnanhkhoa/nb_black.
 Author-email: Nathan Henrie <nate@n8henrie.com>
 License: MIT
 Project-URL: homepage, https://github.com/n8henrie/jupyter-black
 Keywords: jupyter-black
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -177,14 +177,19 @@
 
 ## Buy Me a Coffee
 
 [☕️](https://n8henrie.com/donate)
 
 # [Changelog](https://keepachangelog.com)
 
+## 0.3.4 :: 2023-04-27
+
+- Only pass to `black.Mode` options from `pyproject.toml` that are valid for
+  `black.Mode`. Thanks @rldotai, https://github.com/n8henrie/jupyter-black/issues/7
+
 ## 0.3.2, 0.3.3 :: 2022-11-20
 
 - Remove version constraints (thanks: @JakobGM, https://github.com/n8henrie/jupyter-black/issues/6)
 - Update CI to ensure publishing should work
 
 ## 0.3.1 :: 2022-03-08
```

### Comparing `jupyter-black-0.3.3/src/jupyter_black.egg-info/SOURCES.txt` & `jupyter-black-0.3.4/src/jupyter_black.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 .python-version
 AUTHORS.md
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 Makefile
 README.md
-mypy.ini
 pyproject.toml
 tox.ini
 .github/FUNDING.yml
 .github/ISSUE_TEMPLATE.md
 .github/PULL_REQUEST_TEMPLATE.md
 .github/stale.yml
 .github/workflows/python-package.yml
@@ -20,10 +19,11 @@
 src/jupyter_black.egg-info/PKG-INFO
 src/jupyter_black.egg-info/SOURCES.txt
 src/jupyter_black.egg-info/dependency_links.txt
 src/jupyter_black.egg-info/not-zip-safe
 src/jupyter_black.egg-info/requires.txt
 src/jupyter_black.egg-info/top_level.txt
 tests/conftest.py
+tests/pyproject.toml
 tests/test_jb_helpers.py
 tests/test_lab.py
 tests/test_notebook.py
```

### Comparing `jupyter-black-0.3.3/tests/conftest.py` & `jupyter-black-0.3.4/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,15 +423,15 @@
         ]
     )
     context = browser.new_context()
 
     def teardown() -> None:
         context.close()
         proc.terminate()
-        proc.wait(timeout=5)
+        proc.wait(timeout=10)
 
     request.addfinalizer(teardown)
 
     _wait_for_server(
         browser,
         port=port,
     )
```

### Comparing `jupyter-black-0.3.3/tests/test_jb_helpers.py` & `jupyter-black-0.3.4/tests/test_jb_helpers.py`

 * *Files identical despite different names*

### Comparing `jupyter-black-0.3.3/tests/test_lab.py` & `jupyter-black-0.3.4/tests/test_lab.py`

 * *Files identical despite different names*

