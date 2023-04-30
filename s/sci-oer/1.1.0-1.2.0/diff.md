# Comparing `tmp/sci-oer-1.1.0.tar.gz` & `tmp/sci-oer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sci-oer-1.1.0.tar", last modified: Sat Feb 25 16:49:51 2023, max compression
+gzip compressed data, was "sci-oer-1.2.0.tar", last modified: Sun Apr 30 14:18:40 2023, max compression
```

## Comparing `sci-oer-1.1.0.tar` & `sci-oer-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 16:49:51.300720 sci-oer-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-25 16:49:41.000000 sci-oer-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20796 2023-02-25 16:49:41.000000 sci-oer-1.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-02-25 16:49:41.000000 sci-oer-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-25 16:49:41.000000 sci-oer-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-02-25 16:49:51.300720 sci-oer-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-02-25 16:49:41.000000 sci-oer-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-25 16:49:41.000000 sci-oer-1.1.0/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-02-25 16:49:41.000000 sci-oer-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-02-25 16:49:41.000000 sci-oer-1.1.0/pytype.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-02-25 16:49:41.000000 sci-oer-1.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 16:49:51.300720 sci-oer-1.1.0/sci_oer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-02-25 16:49:51.000000 sci-oer-1.1.0/sci_oer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-02-25 16:49:51.000000 sci-oer-1.1.0/sci_oer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 16:49:51.000000 sci-oer-1.1.0/sci_oer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-25 16:49:51.000000 sci-oer-1.1.0/sci_oer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-02-25 16:49:51.000000 sci-oer-1.1.0/sci_oer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-25 16:49:51.000000 sci-oer-1.1.0/sci_oer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 16:49:51.300720 sci-oer-1.1.0/scioer/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-25 16:49:41.000000 sci-oer-1.1.0/scioer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-25 16:49:51.000000 sci-oer-1.1.0/scioer/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-02-25 16:49:41.000000 sci-oer-1.1.0/scioer/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 16:49:51.300720 sci-oer-1.1.0/scioer/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 16:49:41.000000 sci-oer-1.1.0/scioer/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-02-25 16:49:41.000000 sci-oer-1.1.0/scioer/config/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-02-25 16:49:41.000000 sci-oer-1.1.0/scioer/config/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-02-25 16:49:41.000000 sci-oer-1.1.0/scioer/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-25 16:49:51.300720 sci-oer-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 16:49:51.300720 sci-oer-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-02-25 16:49:41.000000 sci-oer-1.1.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:18:40.671089 sci-oer-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-30 14:18:31.000000 sci-oer-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    23446 2023-04-30 14:18:31.000000 sci-oer-1.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-30 14:18:31.000000 sci-oer-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-30 14:18:31.000000 sci-oer-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-30 14:18:40.671089 sci-oer-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-04-30 14:18:31.000000 sci-oer-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-30 14:18:31.000000 sci-oer-1.2.0/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-30 14:18:31.000000 sci-oer-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-30 14:18:31.000000 sci-oer-1.2.0/pytype.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-30 14:18:31.000000 sci-oer-1.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:18:40.671089 sci-oer-1.2.0/sci_oer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-30 14:18:40.000000 sci-oer-1.2.0/sci_oer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-30 14:18:40.000000 sci-oer-1.2.0/sci_oer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 14:18:40.000000 sci-oer-1.2.0/sci_oer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-30 14:18:40.000000 sci-oer-1.2.0/sci_oer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-30 14:18:40.000000 sci-oer-1.2.0/sci_oer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-30 14:18:40.000000 sci-oer-1.2.0/sci_oer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:18:40.671089 sci-oer-1.2.0/scioer/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-30 14:18:31.000000 sci-oer-1.2.0/scioer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-30 14:18:40.000000 sci-oer-1.2.0/scioer/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-04-30 14:18:31.000000 sci-oer-1.2.0/scioer/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:18:40.671089 sci-oer-1.2.0/scioer/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 14:18:31.000000 sci-oer-1.2.0/scioer/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-30 14:18:31.000000 sci-oer-1.2.0/scioer/config/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-30 14:18:31.000000 sci-oer-1.2.0/scioer/config/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-04-30 14:18:31.000000 sci-oer-1.2.0/scioer/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 14:18:40.671089 sci-oer-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:18:40.671089 sci-oer-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-30 14:18:31.000000 sci-oer-1.2.0/tests/test_cli.py
```

### Comparing `sci-oer-1.1.0/CHANGELOG.md` & `sci-oer-1.2.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,34 @@
 # Changelog
 
+## [v1.2.0](https://github.com/sci-oer/student-cli/releases/v1.2.0) (2023-04-30)
+
+[Full Changelog](https://github.com/sci-oer/student-cli/compare/v1.1.0...v1.2.0)
+
+**Implemented enhancements:**
+
+- feat: add readline so prompts can be edited [\#148](https://github.com/sci-oer/student-cli/pull/148) ([MarshallAsch](https://github.com/MarshallAsch))
+
+**Merged pull requests:**
+
+- chore!: turn off windows ci piplines that keep failing [\#147](https://github.com/sci-oer/student-cli/pull/147) ([MarshallAsch](https://github.com/MarshallAsch))
+- chore: update release notes template [\#146](https://github.com/sci-oer/student-cli/pull/146) ([MarshallAsch](https://github.com/MarshallAsch))
+- chore: auto tag renovate prs as dependancy updates [\#145](https://github.com/sci-oer/student-cli/pull/145) ([MarshallAsch](https://github.com/MarshallAsch))
+- chore\(deps\): update dependency attrs to v23 [\#144](https://github.com/sci-oer/student-cli/pull/144) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency packaging to v23.1 [\#143](https://github.com/sci-oer/student-cli/pull/143) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency black to v23.3.0 [\#142](https://github.com/sci-oer/student-cli/pull/142) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency pathspec to v0.11.1 [\#141](https://github.com/sci-oer/student-cli/pull/141) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency wheel to v0.40.0 [\#140](https://github.com/sci-oer/student-cli/pull/140) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update pypa/gh-action-pypi-publish action to v1.8.5 [\#139](https://github.com/sci-oer/student-cli/pull/139) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency setuptools to v67.7.2 [\#138](https://github.com/sci-oer/student-cli/pull/138) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency rich to v13.3.5 [\#137](https://github.com/sci-oer/student-cli/pull/137) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency platformdirs to v3.5.0 [\#136](https://github.com/sci-oer/student-cli/pull/136) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency pytest to v7.3.1 [\#135](https://github.com/sci-oer/student-cli/pull/135) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency pytype to v2023.4.27 [\#134](https://github.com/sci-oer/student-cli/pull/134) ([renovate[bot]](https://github.com/apps/renovate))
+
 ## [v1.1.0](https://github.com/sci-oer/student-cli/releases/v1.1.0) (2023-02-25)
 
 [Full Changelog](https://github.com/sci-oer/student-cli/compare/v1.0.2...v1.1.0)
 
 **Implemented enhancements:**
 
 - wiki and jupyter have a startup permissions issue [\#46](https://github.com/sci-oer/student-cli/issues/46)
```

### Comparing `sci-oer-1.1.0/LICENSE` & `sci-oer-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sci-oer-1.1.0/PKG-INFO` & `sci-oer-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sci-oer
-Version: 1.1.0
+Version: 1.2.0
 Summary: A cli application to help launch the sci-oer course container
 Author-email: Marshall Asch <masch@uoguelph.ca>
 Project-URL: Documentation, https://github.com/sci-oer/student-cli/blob/main/README.md
 Project-URL: Source, https://github.com/sci-oer/student-cli
 Project-URL: Bug Tracker, https://github.com/sci-oer/student-cli/issues
 Project-URL: Funding, https://github.com/sci-oer/student-cli/blob/main/.github/FUNDING.md
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sci-oer-1.1.0/README.md` & `sci-oer-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sci-oer-1.1.0/pyproject.toml` & `sci-oer-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sci-oer-1.1.0/pytype.cfg` & `sci-oer-1.2.0/pytype.cfg`

 * *Files identical despite different names*

### Comparing `sci-oer-1.1.0/sci_oer.egg-info/PKG-INFO` & `sci-oer-1.2.0/sci_oer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sci-oer
-Version: 1.1.0
+Version: 1.2.0
 Summary: A cli application to help launch the sci-oer course container
 Author-email: Marshall Asch <masch@uoguelph.ca>
 Project-URL: Documentation, https://github.com/sci-oer/student-cli/blob/main/README.md
 Project-URL: Source, https://github.com/sci-oer/student-cli
 Project-URL: Bug Tracker, https://github.com/sci-oer/student-cli/issues
 Project-URL: Funding, https://github.com/sci-oer/student-cli/blob/main/.github/FUNDING.md
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sci-oer-1.1.0/scioer/cli.py` & `sci-oer-1.2.0/scioer/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,26 @@
 import scioer.config.parse as parser
 import os
 import re
 from typing import Optional
 from pathlib import Path
 import logging
 
-__version__ = "UNKOWN"
+try:
+    import readline
+except:
+    import sys
+
+    if sys.platform == "win32" or sys.platform == "cygwin":
+        try:
+            from pyreadline3 import Readline
+        except:
+            pass
+
+__version__ = "UNKNOWN"
 try:
     from scioer.__version__ import __version__
 except:
     pass
 
 import scioer.docker as docker
```

### Comparing `sci-oer-1.1.0/scioer/config/load.py` & `sci-oer-1.2.0/scioer/config/load.py`

 * *Files identical despite different names*

### Comparing `sci-oer-1.1.0/scioer/config/parse.py` & `sci-oer-1.2.0/scioer/config/parse.py`

 * *Files identical despite different names*

### Comparing `sci-oer-1.1.0/scioer/docker.py` & `sci-oer-1.2.0/scioer/docker.py`

 * *Files identical despite different names*

