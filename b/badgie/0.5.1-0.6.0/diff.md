# Comparing `tmp/badgie-0.5.1.tar.gz` & `tmp/badgie-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badgie-0.5.1.tar", last modified: Wed Apr 19 05:53:50 2023, max compression
+gzip compressed data, was "badgie-0.6.0.tar", last modified: Sun Apr 30 08:27:17 2023, max compression
```

## Comparing `badgie-0.5.1.tar` & `badgie-0.6.0.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:53:50.019352 badgie-0.5.1/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-19 05:53:46.000000 badgie-0.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4482 2023-04-19 05:53:50.019352 badgie-0.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3590 2023-04-19 05:53:46.000000 badgie-0.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:53:50.013352 badgie-0.5.1/badgie/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-19 05:53:47.000000 badgie-0.5.1/badgie/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:53:50.017352 badgie-0.5.1/badgie/badges/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/badges/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/badges/_base.py
--rw-rw-rw-   0 root         (0) root         (0)      997 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/badges/brettops.py
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/badges/codestyle.py
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/badges/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      494 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/badges/precommit.py
--rw-rw-rw-   0 root         (0) root         (0)     5154 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:53:50.018352 badgie-0.5.1/badgie/detectors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/detectors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/detectors/precommit.py
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1524 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:53:50.018352 badgie-0.5.1/badgie/providers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/providers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/providers/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:53:50.019352 badgie-0.5.1/badgie/sources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/sources/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:53:50.015352 badgie-0.5.1/badgie.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4482 2023-04-19 05:53:49.000000 badgie-0.5.1/badgie.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      677 2023-04-19 05:53:50.000000 badgie-0.5.1/badgie.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 05:53:49.000000 badgie-0.5.1/badgie.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-19 05:53:49.000000 badgie-0.5.1/badgie.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-19 05:53:49.000000 badgie-0.5.1/badgie.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-19 05:53:49.000000 badgie-0.5.1/badgie.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-19 05:53:50.020352 badgie-0.5.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1429 2023-04-19 05:53:47.000000 badgie-0.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:27:17.796867 badgie-0.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-30 08:27:13.000000 badgie-0.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4466 2023-04-30 08:27:17.796867 badgie-0.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3574 2023-04-30 08:27:13.000000 badgie-0.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:27:17.790866 badgie-0.6.0/badgie/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-30 08:27:14.000000 badgie-0.6.0/badgie/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:27:17.794866 badgie-0.6.0/badgie/badges/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/badges/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/badges/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/badges/brettops.py
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/badges/codestyle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/badges/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/badges/precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     5698 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:27:17.796867 badgie-0.6.0/badgie/finders/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/finders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/finders/files.py
+-rw-rw-rw-   0 root         (0) root         (0)     2386 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/finders/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/finders/pre_commit_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1441 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/finders/remotes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1997 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/project.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/tokens.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:27:17.792866 badgie-0.6.0/badgie.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4466 2023-04-30 08:27:17.000000 badgie-0.6.0/badgie.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      685 2023-04-30 08:27:17.000000 badgie-0.6.0/badgie.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 08:27:17.000000 badgie-0.6.0/badgie.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-30 08:27:17.000000 badgie-0.6.0/badgie.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-30 08:27:17.000000 badgie-0.6.0/badgie.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-30 08:27:17.000000 badgie-0.6.0/badgie.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-30 08:27:17.797867 badgie-0.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-30 08:27:14.000000 badgie-0.6.0/setup.py
```

### Comparing `badgie-0.5.1/LICENSE` & `badgie-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `badgie-0.5.1/PKG-INFO` & `badgie-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: badgie
-Version: 0.5.1
+Version: 0.6.0
 Summary: Add all the badges with Badgie!
 Home-page: https://gitlab.com/brettops/tools/badgie
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
-Keywords: badge template markdown
+Keywords: badge,template,markdown
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -26,15 +26,15 @@
 # Badgie
 
 <!-- BADGIE TIME -->
 
 [![brettops tool](https://img.shields.io/badge/brettops-tool-209cdf?labelColor=162d50)](https://brettops.io)
 [![latest release](https://img.shields.io/gitlab/v/release/brettops/tools/badgie)](https://gitlab.com/brettops/tools/badgie/-/releases)
 [![pipeline status](https://gitlab.com/brettops/tools/badgie/badges/main/pipeline.svg)](https://gitlab.com/brettops/tools/badgie/-/commits/main)
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![code style: black](https://img.shields.io/badge/code_style-black-000000.svg)](https://github.com/psf/black)
 [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
 
 <!-- END BADGIE TIME -->
 
 Add all the badges with Badgie!
```

### Comparing `badgie-0.5.1/README.md` & `badgie-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Badgie
 
 <!-- BADGIE TIME -->
 
 [![brettops tool](https://img.shields.io/badge/brettops-tool-209cdf?labelColor=162d50)](https://brettops.io)
 [![latest release](https://img.shields.io/gitlab/v/release/brettops/tools/badgie)](https://gitlab.com/brettops/tools/badgie/-/releases)
 [![pipeline status](https://gitlab.com/brettops/tools/badgie/badges/main/pipeline.svg)](https://gitlab.com/brettops/tools/badgie/-/commits/main)
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![code style: black](https://img.shields.io/badge/code_style-black-000000.svg)](https://github.com/psf/black)
 [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
 
 <!-- END BADGIE TIME -->
 
 Add all the badges with Badgie!
```

### Comparing `badgie-0.5.1/badgie/parser.py` & `badgie-0.6.0/badgie/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import re
-from dataclasses import dataclass
 from typing import Optional
 
+from attrs import define
+
 from .constants import PATTERN_END, PATTERN_START
 
 
-@dataclass(frozen=True, kw_only=True)
+@define
 class Token:
     value: str
     line: int
     column: int
     type: Optional[str] = None
```

### Comparing `badgie-0.5.1/badgie.egg-info/PKG-INFO` & `badgie-0.6.0/badgie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: badgie
-Version: 0.5.1
+Version: 0.6.0
 Summary: Add all the badges with Badgie!
 Home-page: https://gitlab.com/brettops/tools/badgie
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
-Keywords: badge template markdown
+Keywords: badge,template,markdown
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -26,15 +26,15 @@
 # Badgie
 
 <!-- BADGIE TIME -->
 
 [![brettops tool](https://img.shields.io/badge/brettops-tool-209cdf?labelColor=162d50)](https://brettops.io)
 [![latest release](https://img.shields.io/gitlab/v/release/brettops/tools/badgie)](https://gitlab.com/brettops/tools/badgie/-/releases)
 [![pipeline status](https://gitlab.com/brettops/tools/badgie/badges/main/pipeline.svg)](https://gitlab.com/brettops/tools/badgie/-/commits/main)
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![code style: black](https://img.shields.io/badge/code_style-black-000000.svg)](https://github.com/psf/black)
 [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
 
 <!-- END BADGIE TIME -->
 
 Add all the badges with Badgie!
```

### Comparing `badgie-0.5.1/setup.py` & `badgie-0.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 # injected version
-__version__ = "0.5.1"
+__version__ = "0.6.0"
 
 # markdown readme
 long_description = open("README.md").read()
 
 # read requirements from requirements.in
 install_requires = open("requirements.in").read().splitlines()
 
@@ -24,15 +24,15 @@
     entry_points={
         "console_scripts": [
             "badgie = badgie.cli:main",
         ],
     },
     install_requires=install_requires,
     python_requires=">=3.9",
-    keywords="badge template markdown",
+    keywords=["badge", "template", "markdown"],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
```

