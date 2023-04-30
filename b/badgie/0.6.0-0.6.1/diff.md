# Comparing `tmp/badgie-0.6.0.tar.gz` & `tmp/badgie-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badgie-0.6.0.tar", last modified: Sun Apr 30 08:27:17 2023, max compression
+gzip compressed data, was "badgie-0.6.1.tar", last modified: Sun Apr 30 08:40:53 2023, max compression
```

## Comparing `badgie-0.6.0.tar` & `badgie-0.6.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:27:17.796867 badgie-0.6.0/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-30 08:27:13.000000 badgie-0.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4466 2023-04-30 08:27:17.796867 badgie-0.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3574 2023-04-30 08:27:13.000000 badgie-0.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:27:17.790866 badgie-0.6.0/badgie/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-30 08:27:14.000000 badgie-0.6.0/badgie/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:27:17.794866 badgie-0.6.0/badgie/badges/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/badges/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/badges/_base.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/badges/brettops.py
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/badges/codestyle.py
--rw-rw-rw-   0 root         (0) root         (0)     1466 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/badges/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/badges/precommit.py
--rw-rw-rw-   0 root         (0) root         (0)     5698 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:27:17.796867 badgie-0.6.0/badgie/finders/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/finders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1177 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/finders/files.py
--rw-rw-rw-   0 root         (0) root         (0)     2386 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/finders/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/finders/pre_commit_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1441 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/finders/remotes.py
--rw-rw-rw-   0 root         (0) root         (0)     2271 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1486 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1997 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/project.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-04-30 08:27:13.000000 badgie-0.6.0/badgie/tokens.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:27:17.792866 badgie-0.6.0/badgie.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4466 2023-04-30 08:27:17.000000 badgie-0.6.0/badgie.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      685 2023-04-30 08:27:17.000000 badgie-0.6.0/badgie.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 08:27:17.000000 badgie-0.6.0/badgie.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-30 08:27:17.000000 badgie-0.6.0/badgie.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-30 08:27:17.000000 badgie-0.6.0/badgie.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-30 08:27:17.000000 badgie-0.6.0/badgie.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-30 08:27:17.797867 badgie-0.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-30 08:27:14.000000 badgie-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:40:53.123413 badgie-0.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-30 08:40:48.000000 badgie-0.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4617 2023-04-30 08:40:53.123413 badgie-0.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3725 2023-04-30 08:40:48.000000 badgie-0.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:40:53.117412 badgie-0.6.1/badgie/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-30 08:40:50.000000 badgie-0.6.1/badgie/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:40:53.121413 badgie-0.6.1/badgie/badges/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/badges/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/badges/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/badges/brettops.py
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/badges/codestyle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/badges/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/badges/precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     5698 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:40:53.123413 badgie-0.6.1/badgie/finders/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/finders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/finders/files.py
+-rw-rw-rw-   0 root         (0) root         (0)     2386 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/finders/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/finders/pre_commit_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1441 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/finders/remotes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1997 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/project.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     1647 2023-04-30 08:40:48.000000 badgie-0.6.1/badgie/tokens.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:40:53.119412 badgie-0.6.1/badgie.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4617 2023-04-30 08:40:53.000000 badgie-0.6.1/badgie.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      685 2023-04-30 08:40:53.000000 badgie-0.6.1/badgie.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 08:40:53.000000 badgie-0.6.1/badgie.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-30 08:40:53.000000 badgie-0.6.1/badgie.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-30 08:40:53.000000 badgie-0.6.1/badgie.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-30 08:40:53.000000 badgie-0.6.1/badgie.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-30 08:40:53.124413 badgie-0.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-30 08:40:50.000000 badgie-0.6.1/setup.py
```

### Comparing `badgie-0.6.0/LICENSE` & `badgie-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `badgie-0.6.0/PKG-INFO` & `badgie-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badgie
-Version: 0.6.0
+Version: 0.6.1
 Summary: Add all the badges with Badgie!
 Home-page: https://gitlab.com/brettops/tools/badgie
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: badge,template,markdown
 Platform: UNKNOWN
@@ -24,16 +24,17 @@
 License-File: LICENSE
 
 # Badgie
 
 <!-- BADGIE TIME -->
 
 [![brettops tool](https://img.shields.io/badge/brettops-tool-209cdf?labelColor=162d50)](https://brettops.io)
+[![pipeline status](https://img.shields.io/gitlab/pipeline-status/brettops/tools/badgie)](https://gitlab.com/brettops/tools/badgie/-/commits/main)
+[![coverage report](https://img.shields.io/gitlab/pipeline-coverage/brettops/tools/badgie)](https://gitlab.com/brettops/tools/badgie/-/commits/main)
 [![latest release](https://img.shields.io/gitlab/v/release/brettops/tools/badgie)](https://gitlab.com/brettops/tools/badgie/-/releases)
-[![pipeline status](https://gitlab.com/brettops/tools/badgie/badges/main/pipeline.svg)](https://gitlab.com/brettops/tools/badgie/-/commits/main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![code style: black](https://img.shields.io/badge/code_style-black-000000.svg)](https://github.com/psf/black)
 [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
 
 <!-- END BADGIE TIME -->
 
 Add all the badges with Badgie!
```

### Comparing `badgie-0.6.0/README.md` & `badgie-0.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Badgie
 
 <!-- BADGIE TIME -->
 
 [![brettops tool](https://img.shields.io/badge/brettops-tool-209cdf?labelColor=162d50)](https://brettops.io)
+[![pipeline status](https://img.shields.io/gitlab/pipeline-status/brettops/tools/badgie)](https://gitlab.com/brettops/tools/badgie/-/commits/main)
+[![coverage report](https://img.shields.io/gitlab/pipeline-coverage/brettops/tools/badgie)](https://gitlab.com/brettops/tools/badgie/-/commits/main)
 [![latest release](https://img.shields.io/gitlab/v/release/brettops/tools/badgie)](https://gitlab.com/brettops/tools/badgie/-/releases)
-[![pipeline status](https://gitlab.com/brettops/tools/badgie/badges/main/pipeline.svg)](https://gitlab.com/brettops/tools/badgie/-/commits/main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![code style: black](https://img.shields.io/badge/code_style-black-000000.svg)](https://github.com/psf/black)
 [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
 
 <!-- END BADGIE TIME -->
 
 Add all the badges with Badgie!
```

### Comparing `badgie-0.6.0/badgie/badges/brettops.py` & `badgie-0.6.1/badgie/badges/brettops.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.0/badgie/badges/codestyle.py` & `badgie-0.6.1/badgie/badges/codestyle.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.0/badgie/badges/gitlab.py` & `badgie-0.6.1/badgie/badges/gitlab.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from ._base import register_badges
 
 register_badges(
     {
         to.GITLAB_COVERAGE: Badge(
             name="gitlab-coverage-report",
             description="Show the most recent coverage score on the default branch.",
-            example="https://img.shields.io/gitlab/pipeline-coverage/brettops/tools/badgie",
+            example="https://img.shields.io/gitlab/pipeline-coverage/brettops/tools/badgie?branch=main",
             title="coverage report",
             link="{node.url}/-/commits/{node.ref}",
-            image="https://img.shields.io/gitlab/pipeline-coverage/{node.full_path}",
+            image="https://img.shields.io/gitlab/pipeline-coverage/{node.full_path}?branch={node.ref}",
             weight=1,
         ),
         to.GITLAB_PIPELINE: Badge(
             name="gitlab-pipeline-status",
             description="Show the most recent pipeline status on the default branch.",
-            example="https://img.shields.io/gitlab/pipeline-status/brettops/tools/badgie",
+            example="https://img.shields.io/gitlab/pipeline-status/brettops/tools/badgie?branch=main",
             title="pipeline status",
             link="{node.url}/-/commits/{node.ref}",
-            image="https://img.shields.io/gitlab/pipeline-status/{node.full_path}",
+            image="https://img.shields.io/gitlab/pipeline-status/{node.full_path}?branch={node.ref}",
             weight=0,
         ),
         to.GITLAB_RELEASE: Badge(
             name="gitlab-latest-release",
             description="Show the latest GitLab release by date.",
             example="https://img.shields.io/gitlab/v/release/brettops/tools/badgie",
             title="latest release",
```

### Comparing `badgie-0.6.0/badgie/badges/precommit.py` & `badgie-0.6.1/badgie/badges/precommit.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.0/badgie/cli.py` & `badgie-0.6.1/badgie/cli.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.0/badgie/finders/files.py` & `badgie-0.6.1/badgie/finders/files.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.0/badgie/finders/gitlab.py` & `badgie-0.6.1/badgie/finders/gitlab.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.0/badgie/finders/pre_commit_config.py` & `badgie-0.6.1/badgie/finders/pre_commit_config.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.0/badgie/finders/remotes.py` & `badgie-0.6.1/badgie/finders/remotes.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.0/badgie/models.py` & `badgie-0.6.1/badgie/models.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.0/badgie/parser.py` & `badgie-0.6.1/badgie/parser.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.0/badgie/project.py` & `badgie-0.6.1/badgie/project.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.0/badgie/tokens.py` & `badgie-0.6.1/badgie/tokens.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 GITHUB = "github"
 GITHUB_ACTIONS = "github_actions"
 
 GITLAB = "gitlab"
 GITLAB_CI_FILE = "gitlab_ci_file"
 GITLAB_COVERAGE = "gitlab_coverage"
 GITLAB_ENVIRONMENT = "gitlab_environment"
+GITLAB_LICENSE = "gitlab_license"
 GITLAB_PAGES = "gitlab_pages"
 GITLAB_PIPELINE = "gitlab_pipeline"
 GITLAB_RELEASE = "gitlab_release"
 
 PRE_COMMIT = "pre_commit"
 PRE_COMMIT_CONFIG = "pre_commit_config"
 PRE_COMMIT_HOOKS = "pre_commit_hooks"
```

### Comparing `badgie-0.6.0/badgie.egg-info/PKG-INFO` & `badgie-0.6.1/badgie.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badgie
-Version: 0.6.0
+Version: 0.6.1
 Summary: Add all the badges with Badgie!
 Home-page: https://gitlab.com/brettops/tools/badgie
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: badge,template,markdown
 Platform: UNKNOWN
@@ -24,16 +24,17 @@
 License-File: LICENSE
 
 # Badgie
 
 <!-- BADGIE TIME -->
 
 [![brettops tool](https://img.shields.io/badge/brettops-tool-209cdf?labelColor=162d50)](https://brettops.io)
+[![pipeline status](https://img.shields.io/gitlab/pipeline-status/brettops/tools/badgie)](https://gitlab.com/brettops/tools/badgie/-/commits/main)
+[![coverage report](https://img.shields.io/gitlab/pipeline-coverage/brettops/tools/badgie)](https://gitlab.com/brettops/tools/badgie/-/commits/main)
 [![latest release](https://img.shields.io/gitlab/v/release/brettops/tools/badgie)](https://gitlab.com/brettops/tools/badgie/-/releases)
-[![pipeline status](https://gitlab.com/brettops/tools/badgie/badges/main/pipeline.svg)](https://gitlab.com/brettops/tools/badgie/-/commits/main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![code style: black](https://img.shields.io/badge/code_style-black-000000.svg)](https://github.com/psf/black)
 [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
 
 <!-- END BADGIE TIME -->
 
 Add all the badges with Badgie!
```

### Comparing `badgie-0.6.0/badgie.egg-info/SOURCES.txt` & `badgie-0.6.1/badgie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `badgie-0.6.0/setup.py` & `badgie-0.6.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 # injected version
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 # markdown readme
 long_description = open("README.md").read()
 
 # read requirements from requirements.in
 install_requires = open("requirements.in").read().splitlines()
```

