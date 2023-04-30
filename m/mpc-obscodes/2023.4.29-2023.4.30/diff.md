# Comparing `tmp/mpc_obscodes-2023.4.29.tar.gz` & `tmp/mpc_obscodes-2023.4.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpc_obscodes-2023.4.29.tar", last modified: Sat Apr 29 02:26:52 2023, max compression
+gzip compressed data, was "mpc_obscodes-2023.4.30.tar", last modified: Sun Apr 30 18:02:28 2023, max compression
```

## Comparing `mpc_obscodes-2023.4.29.tar` & `mpc_obscodes-2023.4.30.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:26:52.489684 mpc_obscodes-2023.4.29/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-29 02:26:37.000000 mpc_obscodes-2023.4.29/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-29 02:26:52.489684 mpc_obscodes-2023.4.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-29 02:26:37.000000 mpc_obscodes-2023.4.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:26:52.489684 mpc_obscodes-2023.4.29/mpc_obscodes/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-29 02:26:37.000000 mpc_obscodes-2023.4.29/mpc_obscodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-29 02:26:37.000000 mpc_obscodes-2023.4.29/mpc_obscodes/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-29 02:26:37.000000 mpc_obscodes-2023.4.29/mpc_obscodes/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)   245280 2023-04-29 02:26:40.000000 mpc_obscodes-2023.4.29/mpc_obscodes/obscodes_extended.json
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-29 02:26:40.000000 mpc_obscodes-2023.4.29/mpc_obscodes/obscodes_extended.md5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:26:52.489684 mpc_obscodes-2023.4.29/mpc_obscodes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 02:26:37.000000 mpc_obscodes-2023.4.29/mpc_obscodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-29 02:26:37.000000 mpc_obscodes-2023.4.29/mpc_obscodes/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-29 02:26:37.000000 mpc_obscodes-2023.4.29/mpc_obscodes/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-29 02:26:37.000000 mpc_obscodes-2023.4.29/mpc_obscodes/tests/test_mpc_obscodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:26:52.489684 mpc_obscodes-2023.4.29/mpc_obscodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-29 02:26:52.000000 mpc_obscodes-2023.4.29/mpc_obscodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-29 02:26:52.000000 mpc_obscodes-2023.4.29/mpc_obscodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 02:26:52.000000 mpc_obscodes-2023.4.29/mpc_obscodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 02:26:52.000000 mpc_obscodes-2023.4.29/mpc_obscodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 02:26:52.000000 mpc_obscodes-2023.4.29/mpc_obscodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-29 02:26:40.000000 mpc_obscodes-2023.4.29/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 02:26:52.489684 mpc_obscodes-2023.4.29/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:02:28.016862 mpc_obscodes-2023.4.30/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-30 18:02:05.000000 mpc_obscodes-2023.4.30/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-30 18:02:28.016862 mpc_obscodes-2023.4.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-30 18:02:05.000000 mpc_obscodes-2023.4.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:02:28.012863 mpc_obscodes-2023.4.30/mpc_obscodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-30 18:02:05.000000 mpc_obscodes-2023.4.30/mpc_obscodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-30 18:02:05.000000 mpc_obscodes-2023.4.30/mpc_obscodes/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-30 18:02:05.000000 mpc_obscodes-2023.4.30/mpc_obscodes/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)   245280 2023-04-30 18:02:12.000000 mpc_obscodes-2023.4.30/mpc_obscodes/obscodes_extended.json
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-30 18:02:12.000000 mpc_obscodes-2023.4.30/mpc_obscodes/obscodes_extended.md5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:02:28.016862 mpc_obscodes-2023.4.30/mpc_obscodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 18:02:05.000000 mpc_obscodes-2023.4.30/mpc_obscodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-30 18:02:05.000000 mpc_obscodes-2023.4.30/mpc_obscodes/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-30 18:02:05.000000 mpc_obscodes-2023.4.30/mpc_obscodes/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-30 18:02:05.000000 mpc_obscodes-2023.4.30/mpc_obscodes/tests/test_mpc_obscodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:02:28.012863 mpc_obscodes-2023.4.30/mpc_obscodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-30 18:02:28.000000 mpc_obscodes-2023.4.30/mpc_obscodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-30 18:02:28.000000 mpc_obscodes-2023.4.30/mpc_obscodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:02:28.000000 mpc_obscodes-2023.4.30/mpc_obscodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 18:02:28.000000 mpc_obscodes-2023.4.30/mpc_obscodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-30 18:02:28.000000 mpc_obscodes-2023.4.30/mpc_obscodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-30 18:02:12.000000 mpc_obscodes-2023.4.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 18:02:28.016862 mpc_obscodes-2023.4.30/setup.cfg
```

### Comparing `mpc_obscodes-2023.4.29/PKG-INFO` & `mpc_obscodes-2023.4.30/mpc_obscodes.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
-Name: mpc_obscodes
-Version: 2023.4.29
+Name: mpc-obscodes
+Version: 2023.4.30
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
-# Minor Planet Center Observatory Codes
+# mpc_obscodes: Minor Planet Center Observatory Codes File
+#### A Python package by the Asteroid Institute, a program of the B612 Foundation
 
 [![Python 3.7+](https://img.shields.io/badge/Python-3.7%2B-blue)](https://img.shields.io/badge/Python-3.7%2B-blue)
 [![PyPI version](https://img.shields.io/pypi/v/mpc-obscodes)](https://img.shields.io/pypi/v/mpc-obscodes)
 [![PyPi downloads](https://img.shields.io/pypi/dm/mpc-obscodes)](https://img.shields.io/pypi/dm/mpc-obscodes)  
-[![Build, Test, & Publish](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test_publish.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test_publish.yml)  
+[![Build and Test](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test.yml)
+[![Build, Test, & Publish](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test_publish.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test_publish.yml)
+[![Compare Upstream](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/compare_upstream.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/compare_upstream.yml)  
 
 This package ships the Minor Planet Center's [file](https://minorplanetcenter.net/Extended_Files/obscodes_extended.json.gz) of observatory codes and their geodetic coordinates.
 
-This is not an official MPC package. It is an automatically generated mirror of the file so that it is
+**This is not an official MPC package**. It is an automatically generated mirror of the file so that it is
 installable via `pip`.
 
 Every night at around 2:15 AM UTC, the MPC observatory code file is downloaded and compared (via md5 checksum) to the current version of this package. If the checksums are different, a new package will be published.
 
 ## Installation
 
 The latest version of the file can be install via pip:
```

### Comparing `mpc_obscodes-2023.4.29/README.md` & `mpc_obscodes-2023.4.30/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-# Minor Planet Center Observatory Codes
+# mpc_obscodes: Minor Planet Center Observatory Codes File
+#### A Python package by the Asteroid Institute, a program of the B612 Foundation
 
 [![Python 3.7+](https://img.shields.io/badge/Python-3.7%2B-blue)](https://img.shields.io/badge/Python-3.7%2B-blue)
 [![PyPI version](https://img.shields.io/pypi/v/mpc-obscodes)](https://img.shields.io/pypi/v/mpc-obscodes)
 [![PyPi downloads](https://img.shields.io/pypi/dm/mpc-obscodes)](https://img.shields.io/pypi/dm/mpc-obscodes)  
-[![Build, Test, & Publish](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test_publish.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test_publish.yml)  
+[![Build and Test](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test.yml)
+[![Build, Test, & Publish](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test_publish.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test_publish.yml)
+[![Compare Upstream](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/compare_upstream.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/compare_upstream.yml)  
 
 This package ships the Minor Planet Center's [file](https://minorplanetcenter.net/Extended_Files/obscodes_extended.json.gz) of observatory codes and their geodetic coordinates.
 
-This is not an official MPC package. It is an automatically generated mirror of the file so that it is
+**This is not an official MPC package**. It is an automatically generated mirror of the file so that it is
 installable via `pip`.
 
 Every night at around 2:15 AM UTC, the MPC observatory code file is downloaded and compared (via md5 checksum) to the current version of this package. If the checksums are different, a new package will be published.
 
 ## Installation
 
 The latest version of the file can be install via pip:
```

### Comparing `mpc_obscodes-2023.4.29/mpc_obscodes/compare.py` & `mpc_obscodes-2023.4.30/mpc_obscodes/compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.29/mpc_obscodes/fetch.py` & `mpc_obscodes-2023.4.30/mpc_obscodes/fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.29/mpc_obscodes/obscodes_extended.json` & `mpc_obscodes-2023.4.30/mpc_obscodes/obscodes_extended.json`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.29/mpc_obscodes/tests/test_compare.py` & `mpc_obscodes-2023.4.30/mpc_obscodes/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.29/mpc_obscodes/tests/test_fetch.py` & `mpc_obscodes-2023.4.30/mpc_obscodes/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.29/mpc_obscodes/tests/test_mpc_obscodes.py` & `mpc_obscodes-2023.4.30/mpc_obscodes/tests/test_mpc_obscodes.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.29/mpc_obscodes.egg-info/PKG-INFO` & `mpc_obscodes-2023.4.30/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
-Name: mpc-obscodes
-Version: 2023.4.29
+Name: mpc_obscodes
+Version: 2023.4.30
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
-# Minor Planet Center Observatory Codes
+# mpc_obscodes: Minor Planet Center Observatory Codes File
+#### A Python package by the Asteroid Institute, a program of the B612 Foundation
 
 [![Python 3.7+](https://img.shields.io/badge/Python-3.7%2B-blue)](https://img.shields.io/badge/Python-3.7%2B-blue)
 [![PyPI version](https://img.shields.io/pypi/v/mpc-obscodes)](https://img.shields.io/pypi/v/mpc-obscodes)
 [![PyPi downloads](https://img.shields.io/pypi/dm/mpc-obscodes)](https://img.shields.io/pypi/dm/mpc-obscodes)  
-[![Build, Test, & Publish](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test_publish.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test_publish.yml)  
+[![Build and Test](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test.yml)
+[![Build, Test, & Publish](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test_publish.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test_publish.yml)
+[![Compare Upstream](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/compare_upstream.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/compare_upstream.yml)  
 
 This package ships the Minor Planet Center's [file](https://minorplanetcenter.net/Extended_Files/obscodes_extended.json.gz) of observatory codes and their geodetic coordinates.
 
-This is not an official MPC package. It is an automatically generated mirror of the file so that it is
+**This is not an official MPC package**. It is an automatically generated mirror of the file so that it is
 installable via `pip`.
 
 Every night at around 2:15 AM UTC, the MPC observatory code file is downloaded and compared (via md5 checksum) to the current version of this package. If the checksums are different, a new package will be published.
 
 ## Installation
 
 The latest version of the file can be install via pip:
```

### Comparing `mpc_obscodes-2023.4.29/pyproject.toml` & `mpc_obscodes-2023.4.30/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires =  ["setuptools>=45", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpc_obscodes"
-version = "2023.04.29"
+version = "2023.04.30"
 authors = [
     {name = "B612 Asteroid Institute", email = "info@b612foundation.org"},
 ]
 description = "Minor Planet Center Observatory Codes"
 readme = "README.md"
 requires-python = ">=3.7"
```

