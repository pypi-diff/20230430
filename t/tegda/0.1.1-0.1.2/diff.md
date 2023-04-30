# Comparing `tmp/tegda-0.1.1.tar.gz` & `tmp/tegda-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tegda-0.1.1.tar", last modified: Fri Apr 28 18:23:30 2023, max compression
+gzip compressed data, was "tegda-0.1.2.tar", last modified: Sun Apr 30 08:38:48 2023, max compression
```

## Comparing `tegda-0.1.1.tar` & `tegda-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-28 18:23:30.047798 tegda-0.1.1/
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      171 2023-04-27 17:07:12.000000 tegda-0.1.1/AUTHORS.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     3509 2023-04-27 17:07:12.000000 tegda-0.1.1/CONTRIBUTING.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      115 2023-04-27 17:58:03.000000 tegda-0.1.1/HISTORY.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     6131 2023-04-27 18:50:58.000000 tegda-0.1.1/LICENSE
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      262 2023-04-27 17:07:12.000000 tegda-0.1.1/MANIFEST.in
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     2348 2023-04-28 18:23:30.048799 tegda-0.1.1/PKG-INFO
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1091 2023-04-28 17:23:37.000000 tegda-0.1.1/README.rst
-drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-28 18:23:29.644834 tegda-0.1.1/docs/
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      606 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/Makefile
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       28 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/authors.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     4808 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/conf.py
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       33 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/contributing.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       28 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/history.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      310 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/index.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1134 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/installation.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      803 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/make.bat
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       27 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/readme.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       73 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/usage.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      422 2023-04-28 18:23:30.056316 tegda-0.1.1/setup.cfg
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1424 2023-04-28 18:22:22.000000 tegda-0.1.1/setup.py
-drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-28 18:23:29.757675 tegda-0.1.1/tegda/
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      384 2023-04-28 18:22:30.000000 tegda-0.1.1/tegda/__init__.py
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      393 2023-04-27 17:07:12.000000 tegda-0.1.1/tegda/cli.py
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       19 2023-04-27 17:07:12.000000 tegda-0.1.1/tegda/tegda.py
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1365 2023-04-27 19:21:00.000000 tegda-0.1.1/tegda/utils.py
-drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-28 18:23:29.965166 tegda-0.1.1/tegda.egg-info/
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     2348 2023-04-28 18:23:28.000000 tegda-0.1.1/tegda.egg-info/PKG-INFO
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      558 2023-04-28 18:23:29.000000 tegda-0.1.1/tegda.egg-info/SOURCES.txt
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)        1 2023-04-28 18:23:28.000000 tegda-0.1.1/tegda.egg-info/dependency_links.txt
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       42 2023-04-28 18:23:28.000000 tegda-0.1.1/tegda.egg-info/entry_points.txt
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)        1 2023-04-28 18:23:28.000000 tegda-0.1.1/tegda.egg-info/not-zip-safe
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       11 2023-04-28 18:23:28.000000 tegda-0.1.1/tegda.egg-info/requires.txt
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)        6 2023-04-28 18:23:28.000000 tegda-0.1.1/tegda.egg-info/top_level.txt
-drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-28 18:23:30.017511 tegda-0.1.1/tests/
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       35 2023-04-27 17:07:12.000000 tegda-0.1.1/tests/__init__.py
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      969 2023-04-27 17:07:12.000000 tegda-0.1.1/tests/test_tegda.py
+drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-30 08:38:48.483145 tegda-0.1.2/
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      171 2023-04-27 17:07:12.000000 tegda-0.1.2/AUTHORS.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     3509 2023-04-27 17:07:12.000000 tegda-0.1.2/CONTRIBUTING.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      115 2023-04-27 17:58:03.000000 tegda-0.1.2/HISTORY.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     6131 2023-04-27 18:50:58.000000 tegda-0.1.2/LICENSE
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      262 2023-04-27 17:07:12.000000 tegda-0.1.2/MANIFEST.in
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     2348 2023-04-30 08:38:48.485145 tegda-0.1.2/PKG-INFO
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1091 2023-04-28 17:23:37.000000 tegda-0.1.2/README.rst
+drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-30 08:38:48.171192 tegda-0.1.2/docs/
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      606 2023-04-27 17:07:12.000000 tegda-0.1.2/docs/Makefile
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       28 2023-04-27 17:07:12.000000 tegda-0.1.2/docs/authors.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     4808 2023-04-27 17:07:12.000000 tegda-0.1.2/docs/conf.py
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       33 2023-04-27 17:07:12.000000 tegda-0.1.2/docs/contributing.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       28 2023-04-27 17:07:12.000000 tegda-0.1.2/docs/history.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      310 2023-04-27 17:07:12.000000 tegda-0.1.2/docs/index.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1134 2023-04-27 17:07:12.000000 tegda-0.1.2/docs/installation.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      803 2023-04-27 17:07:12.000000 tegda-0.1.2/docs/make.bat
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       27 2023-04-27 17:07:12.000000 tegda-0.1.2/docs/readme.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       73 2023-04-27 17:07:12.000000 tegda-0.1.2/docs/usage.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      422 2023-04-30 08:38:48.492143 tegda-0.1.2/setup.cfg
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1424 2023-04-30 08:38:37.000000 tegda-0.1.2/setup.py
+drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-30 08:38:48.250142 tegda-0.1.2/tegda/
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      458 2023-04-30 08:38:16.000000 tegda-0.1.2/tegda/__init__.py
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      393 2023-04-27 17:07:12.000000 tegda-0.1.2/tegda/cli.py
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       19 2023-04-27 17:07:12.000000 tegda-0.1.2/tegda/tegda.py
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1326 2023-04-30 07:56:50.000000 tegda-0.1.2/tegda/utils.py
+drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-30 08:38:48.405142 tegda-0.1.2/tegda.egg-info/
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     2348 2023-04-30 08:38:47.000000 tegda-0.1.2/tegda.egg-info/PKG-INFO
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      558 2023-04-30 08:38:47.000000 tegda-0.1.2/tegda.egg-info/SOURCES.txt
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)        1 2023-04-30 08:38:47.000000 tegda-0.1.2/tegda.egg-info/dependency_links.txt
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       42 2023-04-30 08:38:47.000000 tegda-0.1.2/tegda.egg-info/entry_points.txt
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)        1 2023-04-30 08:38:47.000000 tegda-0.1.2/tegda.egg-info/not-zip-safe
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       11 2023-04-30 08:38:47.000000 tegda-0.1.2/tegda.egg-info/requires.txt
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)        6 2023-04-30 08:38:47.000000 tegda-0.1.2/tegda.egg-info/top_level.txt
+drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-30 08:38:48.457145 tegda-0.1.2/tests/
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       35 2023-04-27 17:07:12.000000 tegda-0.1.2/tests/__init__.py
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      969 2023-04-27 17:07:12.000000 tegda-0.1.2/tests/test_tegda.py
```

### Comparing `tegda-0.1.1/CONTRIBUTING.rst` & `tegda-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tegda-0.1.1/LICENSE` & `tegda-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tegda-0.1.1/PKG-INFO` & `tegda-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: tegda
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tegda creates customizable visual representations of data for exploratory analysis.
 Home-page: https://github.com/Robertoarce/tegda
 Author: Roberto Arce Aguirre
 Author-email: roberto_arce_@hotmail.com
 License: MIT license
 Description: =============
         Terrific EGDA
```

### Comparing `tegda-0.1.1/README.rst` & `tegda-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `tegda-0.1.1/docs/Makefile` & `tegda-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tegda-0.1.1/docs/conf.py` & `tegda-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tegda-0.1.1/docs/installation.rst` & `tegda-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tegda-0.1.1/docs/make.bat` & `tegda-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tegda-0.1.1/setup.py` & `tegda-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='tegda',
     name='tegda',
     packages=find_packages(include=['tegda', 'tegda.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Robertoarce/tegda',
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

### Comparing `tegda-0.1.1/tegda/utils.py` & `tegda-0.1.2/tegda/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 #This file is for all non-core functions
-import pandas as pd
-import numpy as np
 
 """ Basic utility functions """
 
 def create_fake_dataset(period = 365, frequency = 'D') -> pd.Dataframe:
     """
     Creates a fake data set for testing purposes.
```

### Comparing `tegda-0.1.1/tegda.egg-info/PKG-INFO` & `tegda-0.1.2/tegda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: tegda
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tegda creates customizable visual representations of data for exploratory analysis.
 Home-page: https://github.com/Robertoarce/tegda
 Author: Roberto Arce Aguirre
 Author-email: roberto_arce_@hotmail.com
 License: MIT license
 Description: =============
         Terrific EGDA
```

### Comparing `tegda-0.1.1/tegda.egg-info/SOURCES.txt` & `tegda-0.1.2/tegda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tegda-0.1.1/tests/test_tegda.py` & `tegda-0.1.2/tests/test_tegda.py`

 * *Files identical despite different names*

