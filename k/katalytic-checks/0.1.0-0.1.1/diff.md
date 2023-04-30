# Comparing `tmp/katalytic-checks-0.1.0.tar.gz` & `tmp/katalytic-checks-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-checks-0.1.0.tar", last modified: Sun Apr 30 05:55:13 2023, max compression
+gzip compressed data, was "katalytic-checks-0.1.1.tar", last modified: Sun Apr 30 07:30:53 2023, max compression
```

## Comparing `katalytic-checks-0.1.0.tar` & `katalytic-checks-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-checks-0.1.0/.coveragerc
--rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-checks-0.1.0/.gitignore
--rw-r--r--   0        0        0     3062 2023-04-30 05:48:57.335564 katalytic-checks-0.1.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      598 2023-04-30 05:54:56.055866 katalytic-checks-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-checks-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1990 2023-04-27 05:10:58.838831 katalytic-checks-0.1.0/README.md
--rw-r--r--   0        0        0     1257 2023-04-30 05:54:56.055866 katalytic-checks-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6052 2023-04-30 05:32:34.812039 katalytic-checks-0.1.0/src/katalytic/checks.py
--rw-r--r--   0        0        0    16322 2023-04-30 05:18:35.946848 katalytic-checks-0.1.0/tests/test_checks.py
--rw-r--r--   0        0        0     3095 1970-01-01 00:00:00.000000 katalytic-checks-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-checks-0.1.1/.coveragerc
+-rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-checks-0.1.1/.gitignore
+-rw-r--r--   0        0        0     3258 2023-04-30 07:06:11.215194 katalytic-checks-0.1.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      761 2023-04-30 07:30:50.798514 katalytic-checks-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-checks-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1948 2023-04-30 07:15:09.987879 katalytic-checks-0.1.1/README.md
+-rw-r--r--   0        0        0     1257 2023-04-30 07:30:50.798514 katalytic-checks-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6146 2023-04-30 07:27:47.285907 katalytic-checks-0.1.1/src/katalytic/checks.py
+-rw-r--r--   0        0        0    16322 2023-04-30 05:18:35.946848 katalytic-checks-0.1.1/tests/test_checks.py
+-rw-r--r--   0        0        0     3053 1970-01-01 00:00:00.000000 katalytic-checks-0.1.1/PKG-INFO
```

### Comparing `katalytic-checks-0.1.0/.gitignore` & `katalytic-checks-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-checks-0.1.0/.gitlab-ci.yml` & `katalytic-checks-0.1.1/.gitlab-ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -10,25 +10,31 @@
   - release
 
 variables:
   TOX_ENV: py39
   PIP_DISABLE_PIP_VERSION_CHECK: "1"
   PIP_NO_CACHE_DIR: "off"
 
-test_cov:
+coverage:
   image: python:3.6
   stage: coverage
   script:
     - pip install --upgrade pip
     - pip install -e .[dev]
-    - python -m pytest --cov-fail-under=100 --cov=src --cov-report term-missing || { echo "Tests failed. Exiting ..." && exit 1; }
+    - python -m pytest --cov-fail-under=100 --cov=src --cov-report=xml --cov-report=term-missing || { echo "Tests failed. Exiting ..." && exit 1; }
   rules:
     - if: '$CI_COMMIT_MESSAGE =~ /(feat|fix|refactor|perf|test|chore|style)/i'
       when: always
     - when: never
+  coverage: /(?i)total.*? (100(?:\.0+)?\%|[1-9]?\d(?:\.\d+)?\%)$/
+  artifacts:
+    reports:
+      coverage_report:
+        coverage_format: cobertura
+        path: "coverage.xml"
   allow_failure: false
 
 
 # test_py36:
 #   image: python:3.6
 #   stage: test
 #   script:
```

### Comparing `katalytic-checks-0.1.0/CHANGELOG.md` & `katalytic-checks-0.1.1/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.1.1 (2023-04-30)
+### fix
+- [[`cfde93d`](https://gitlab.com/katalytic/katalytic-checks/commit/cfde93d73b9f1f7f142168bf4743ba24d8819305)] missing __version__
+
+
 ## 0.1.0 (2023-04-30)
 ### feat
 - [[`0e81081`](https://gitlab.com/katalytic/katalytic-checks/commit/0e8108157478cc87e2f06724109136bf928a0d50)] add is_number()
 ### fix
 - [[`eeb80c0`](https://gitlab.com/katalytic/katalytic-checks/commit/eeb80c090e39e8e4ee292be075af47c4f32150f0)] is_generator(), is_iterable(), is_iterable_or_str(), is_iterator(), is_primitive() and use all_types/all_types_besides for test parametrization
```

### Comparing `katalytic-checks-0.1.0/LICENSE.txt` & `katalytic-checks-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-checks-0.1.0/README.md` & `katalytic-checks-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-checks)](https://pypi.org/project/katalytic-checks/)
-[![Build Status](https://app.travis-ci.com/katalytic/katalytic-checks.svg?branch=main)](https://app.travis-ci.com/gitlab/katalytic/katalytic-checks)
-[![Test Results](https://img.shields.io/travis/com/katalytic/katalytic-checks?label=tests)](https://app.travis-ci.com/gitlab/katalytic/katalytic-checks)
-[![Coverage Status](https://coveralls.io/repos/gitlab/katalytic/katalytic-checks/badge.svg?branch=main)](https://coveralls.io/gitlab/katalytic/katalytic-checks?branch=main)
-[![Docs Coverage](https://img.shields.io/readthedocs/katalytic-checks.svg)](https://katalytic-checks.readthedocs.io/en/latest/)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![pipeline](https://gitlab.com/katalytic/katalytic-checks/badges/main/pipeline.svg)](https://gitlab.com/katalytic/katalytic-checks/-/commits/main)
+[![coverage](https://gitlab.com/katalytic/katalytic-checks/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-checks/-/commits/main)
+[![tests](https://img.shields.io/travis/com/katalytic/katalytic-checks?label=tests)](https://app.travis-ci.com/gitlab/katalytic/katalytic-checks)
+[![docs](https://img.shields.io/readthedocs/katalytic-checks.svg)](https://katalytic-checks.readthedocs.io/en/latest/)
+[![license: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Installation
 By itself
 ```bash
 pip install katalytic-checks
 ```
```

### Comparing `katalytic-checks-0.1.0/pyproject.toml` & `katalytic-checks-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-checks"
-version = "0.1.0"
+version = "0.1.1"
 description = "This plugin adds utilities for working with data to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-checks-0.1.0/src/katalytic/checks.py` & `katalytic-checks-0.1.1/src/katalytic/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import collections
 import inspect
 from decimal import Decimal
 from fractions import Fraction
 
+from katalytic.pkg import get_version
+
+__version__, __version_info__ = get_version(__name__)
+
 
 def contains_all_of(haystack, needles):
     if not is_iterable(haystack):
         raise TypeError(f'<haystack> expects an iterable. Got {type(haystack).__name__}: {haystack!r}')
     elif not is_iterable(needles):
         raise TypeError(f'<needles> expects an iterable. Got {type(needles).__name__}: {needles!r}')
```

### Comparing `katalytic-checks-0.1.0/tests/test_checks.py` & `katalytic-checks-0.1.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `katalytic-checks-0.1.0/PKG-INFO` & `katalytic-checks-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-checks
-Version: 0.1.0
+Version: 0.1.1
 Summary: This plugin adds utilities for working with data to the katalytic namespace
 Keywords: high-level,data conversion
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -24,19 +24,19 @@
 Project-URL: repository, https://gitlab.com/katalytic/katalytic-checks.git
 Provides-Extra: dev
 
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-checks)](https://pypi.org/project/katalytic-checks/)
-[![Build Status](https://app.travis-ci.com/katalytic/katalytic-checks.svg?branch=main)](https://app.travis-ci.com/gitlab/katalytic/katalytic-checks)
-[![Test Results](https://img.shields.io/travis/com/katalytic/katalytic-checks?label=tests)](https://app.travis-ci.com/gitlab/katalytic/katalytic-checks)
-[![Coverage Status](https://coveralls.io/repos/gitlab/katalytic/katalytic-checks/badge.svg?branch=main)](https://coveralls.io/gitlab/katalytic/katalytic-checks?branch=main)
-[![Docs Coverage](https://img.shields.io/readthedocs/katalytic-checks.svg)](https://katalytic-checks.readthedocs.io/en/latest/)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![pipeline](https://gitlab.com/katalytic/katalytic-checks/badges/main/pipeline.svg)](https://gitlab.com/katalytic/katalytic-checks/-/commits/main)
+[![coverage](https://gitlab.com/katalytic/katalytic-checks/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-checks/-/commits/main)
+[![tests](https://img.shields.io/travis/com/katalytic/katalytic-checks?label=tests)](https://app.travis-ci.com/gitlab/katalytic/katalytic-checks)
+[![docs](https://img.shields.io/readthedocs/katalytic-checks.svg)](https://katalytic-checks.readthedocs.io/en/latest/)
+[![license: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Installation
 By itself
 ```bash
 pip install katalytic-checks
 ```
```

