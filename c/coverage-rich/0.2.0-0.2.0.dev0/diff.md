# Comparing `tmp/coverage_rich-0.2.0.tar.gz` & `tmp/coverage_rich-0.2.0.dev0.tar.gz`

## Comparing `coverage_rich-0.2.0.tar` & `coverage_rich-0.2.0.dev0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/coverage_rich/__about__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/coverage_rich/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/coverage_rich/__main__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/coverage_rich/config.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/coverage_rich/console.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/coverage_rich/report.py
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/coverage_rich/standard_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/coverage_rich/cli/__init__.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/coverage_rich/cli/app.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/coverage_rich/cli/common.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/coverage_rich/cli/config.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/coverage_rich/cli/report.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/coverage_rich/cli/tui.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/coverage_rich/tui/app.css
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/coverage_rich/tui/app.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/tests/test_report.py
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/README.md
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 coverage_rich-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/CHANGELOG.md
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/__about__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/__main__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/config.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/console.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/report.py
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/standard_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/cli/__init__.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/cli/app.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/cli/common.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/cli/config.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/cli/report.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/cli/tui.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/tui/app.css
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/tui/app.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/tests/__init__.py
+-rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/tests/test_report.py
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/LICENSE.txt
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/README.md
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/PKG-INFO
```

### Comparing `coverage_rich-0.2.0/coverage_rich/report.py` & `coverage_rich-0.2.0.dev0/coverage_rich/report.py`

 * *Files identical despite different names*

### Comparing `coverage_rich-0.2.0/coverage_rich/standard_config.py` & `coverage_rich-0.2.0.dev0/coverage_rich/standard_config.py`

 * *Files identical despite different names*

### Comparing `coverage_rich-0.2.0/coverage_rich/cli/app.py` & `coverage_rich-0.2.0.dev0/coverage_rich/cli/app.py`

 * *Files identical despite different names*

### Comparing `coverage_rich-0.2.0/coverage_rich/cli/config.py` & `coverage_rich-0.2.0.dev0/coverage_rich/cli/config.py`

 * *Files identical despite different names*

### Comparing `coverage_rich-0.2.0/coverage_rich/tui/app.py` & `coverage_rich-0.2.0.dev0/coverage_rich/tui/app.py`

 * *Files identical despite different names*

### Comparing `coverage_rich-0.2.0/tests/test_report.py` & `coverage_rich-0.2.0.dev0/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `coverage_rich-0.2.0/.gitignore` & `coverage_rich-0.2.0.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `coverage_rich-0.2.0/LICENSE.txt` & `coverage_rich-0.2.0.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coverage_rich-0.2.0/README.md` & `coverage_rich-0.2.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `coverage_rich-0.2.0/pyproject.toml` & `coverage_rich-0.2.0.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coverage_rich-0.2.0/PKG-INFO` & `coverage_rich-0.2.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coverage-rich
-Version: 0.2.0
+Version: 0.2.0.dev0
 Summary: A rich terminal report for coveragepy.
 Project-URL: Documentation, https://github.com/waylonwalker/coverage-rich#readme
 Project-URL: Issues, https://github.com/waylonwalker/coverage-rich/issues
 Project-URL: Source, https://github.com/waylonwalker/coverage-rich
 Project-URL: Changelog, https://github.com/waylonwalker/coverage-rich
 Author-email: "Waylon S. Walker" <waylon@waylonwalker.com>
 License-Expression: MIT
```

