# Comparing `tmp/tegda-0.1.3.tar.gz` & `tmp/tegda-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tegda-0.1.3.tar", last modified: Sun Apr 30 09:17:20 2023, max compression
+gzip compressed data, was "tegda-0.1.4.tar", last modified: Sun Apr 30 09:19:53 2023, max compression
```

## Comparing `tegda-0.1.3.tar` & `tegda-0.1.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-30 09:17:20.729453 tegda-0.1.3/
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      171 2023-04-27 17:07:12.000000 tegda-0.1.3/AUTHORS.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     3509 2023-04-27 17:07:12.000000 tegda-0.1.3/CONTRIBUTING.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      115 2023-04-27 17:58:03.000000 tegda-0.1.3/HISTORY.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     6131 2023-04-27 18:50:58.000000 tegda-0.1.3/LICENSE
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      262 2023-04-27 17:07:12.000000 tegda-0.1.3/MANIFEST.in
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     2348 2023-04-30 09:17:20.730456 tegda-0.1.3/PKG-INFO
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1091 2023-04-28 17:23:37.000000 tegda-0.1.3/README.rst
-drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-30 09:17:20.427632 tegda-0.1.3/docs/
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      606 2023-04-27 17:07:12.000000 tegda-0.1.3/docs/Makefile
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       28 2023-04-27 17:07:12.000000 tegda-0.1.3/docs/authors.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     4808 2023-04-27 17:07:12.000000 tegda-0.1.3/docs/conf.py
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       33 2023-04-27 17:07:12.000000 tegda-0.1.3/docs/contributing.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       28 2023-04-27 17:07:12.000000 tegda-0.1.3/docs/history.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      310 2023-04-27 17:07:12.000000 tegda-0.1.3/docs/index.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1134 2023-04-27 17:07:12.000000 tegda-0.1.3/docs/installation.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      803 2023-04-27 17:07:12.000000 tegda-0.1.3/docs/make.bat
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       27 2023-04-27 17:07:12.000000 tegda-0.1.3/docs/readme.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       73 2023-04-27 17:07:12.000000 tegda-0.1.3/docs/usage.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      422 2023-04-30 09:17:20.737452 tegda-0.1.3/setup.cfg
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1424 2023-04-30 09:16:49.000000 tegda-0.1.3/setup.py
-drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-30 09:17:20.504452 tegda-0.1.3/tegda/
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      562 2023-04-30 09:16:33.000000 tegda-0.1.3/tegda/__init__.py
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      393 2023-04-27 17:07:12.000000 tegda-0.1.3/tegda/cli.py
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       19 2023-04-27 17:07:12.000000 tegda-0.1.3/tegda/tegda.py
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1326 2023-04-30 07:56:50.000000 tegda-0.1.3/tegda/utils.py
-drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-30 09:17:20.662452 tegda-0.1.3/tegda.egg-info/
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     2348 2023-04-30 09:17:19.000000 tegda-0.1.3/tegda.egg-info/PKG-INFO
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      558 2023-04-30 09:17:20.000000 tegda-0.1.3/tegda.egg-info/SOURCES.txt
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)        1 2023-04-30 09:17:19.000000 tegda-0.1.3/tegda.egg-info/dependency_links.txt
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       42 2023-04-30 09:17:19.000000 tegda-0.1.3/tegda.egg-info/entry_points.txt
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)        1 2023-04-30 09:17:19.000000 tegda-0.1.3/tegda.egg-info/not-zip-safe
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       11 2023-04-30 09:17:19.000000 tegda-0.1.3/tegda.egg-info/requires.txt
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)        6 2023-04-30 09:17:19.000000 tegda-0.1.3/tegda.egg-info/top_level.txt
-drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-30 09:17:20.707451 tegda-0.1.3/tests/
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       35 2023-04-27 17:07:12.000000 tegda-0.1.3/tests/__init__.py
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      969 2023-04-27 17:07:12.000000 tegda-0.1.3/tests/test_tegda.py
+drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-30 09:19:53.962533 tegda-0.1.4/
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      171 2023-04-27 17:07:12.000000 tegda-0.1.4/AUTHORS.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     3509 2023-04-27 17:07:12.000000 tegda-0.1.4/CONTRIBUTING.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      115 2023-04-27 17:58:03.000000 tegda-0.1.4/HISTORY.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     6131 2023-04-27 18:50:58.000000 tegda-0.1.4/LICENSE
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      262 2023-04-27 17:07:12.000000 tegda-0.1.4/MANIFEST.in
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     2348 2023-04-30 09:19:53.963533 tegda-0.1.4/PKG-INFO
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1091 2023-04-28 17:23:37.000000 tegda-0.1.4/README.rst
+drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-30 09:19:53.674461 tegda-0.1.4/docs/
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      606 2023-04-27 17:07:12.000000 tegda-0.1.4/docs/Makefile
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       28 2023-04-27 17:07:12.000000 tegda-0.1.4/docs/authors.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     4808 2023-04-27 17:07:12.000000 tegda-0.1.4/docs/conf.py
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       33 2023-04-27 17:07:12.000000 tegda-0.1.4/docs/contributing.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       28 2023-04-27 17:07:12.000000 tegda-0.1.4/docs/history.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      310 2023-04-27 17:07:12.000000 tegda-0.1.4/docs/index.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1134 2023-04-27 17:07:12.000000 tegda-0.1.4/docs/installation.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      803 2023-04-27 17:07:12.000000 tegda-0.1.4/docs/make.bat
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       27 2023-04-27 17:07:12.000000 tegda-0.1.4/docs/readme.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       73 2023-04-27 17:07:12.000000 tegda-0.1.4/docs/usage.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      422 2023-04-30 09:19:53.969534 tegda-0.1.4/setup.cfg
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1424 2023-04-30 09:19:23.000000 tegda-0.1.4/setup.py
+drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-30 09:19:53.748915 tegda-0.1.4/tegda/
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      562 2023-04-30 09:16:33.000000 tegda-0.1.4/tegda/__init__.py
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      393 2023-04-27 17:07:12.000000 tegda-0.1.4/tegda/cli.py
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       19 2023-04-27 17:07:12.000000 tegda-0.1.4/tegda/tegda.py
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1326 2023-04-30 07:56:50.000000 tegda-0.1.4/tegda/utils.py
+drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-30 09:19:53.897665 tegda-0.1.4/tegda.egg-info/
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     2348 2023-04-30 09:19:52.000000 tegda-0.1.4/tegda.egg-info/PKG-INFO
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      558 2023-04-30 09:19:53.000000 tegda-0.1.4/tegda.egg-info/SOURCES.txt
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)        1 2023-04-30 09:19:52.000000 tegda-0.1.4/tegda.egg-info/dependency_links.txt
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       42 2023-04-30 09:19:52.000000 tegda-0.1.4/tegda.egg-info/entry_points.txt
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)        1 2023-04-30 09:19:52.000000 tegda-0.1.4/tegda.egg-info/not-zip-safe
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       11 2023-04-30 09:19:52.000000 tegda-0.1.4/tegda.egg-info/requires.txt
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)        6 2023-04-30 09:19:52.000000 tegda-0.1.4/tegda.egg-info/top_level.txt
+drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-30 09:19:53.939533 tegda-0.1.4/tests/
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       35 2023-04-27 17:07:12.000000 tegda-0.1.4/tests/__init__.py
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      969 2023-04-27 17:07:12.000000 tegda-0.1.4/tests/test_tegda.py
```

### Comparing `tegda-0.1.3/CONTRIBUTING.rst` & `tegda-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tegda-0.1.3/LICENSE` & `tegda-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tegda-0.1.3/PKG-INFO` & `tegda-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: tegda
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tegda creates customizable visual representations of data for exploratory analysis.
 Home-page: https://github.com/Robertoarce/tegda
 Author: Roberto Arce Aguirre
 Author-email: roberto_arce_@hotmail.com
 License: MIT license
 Description: =============
         Terrific EGDA
```

### Comparing `tegda-0.1.3/README.rst` & `tegda-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `tegda-0.1.3/docs/Makefile` & `tegda-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tegda-0.1.3/docs/conf.py` & `tegda-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tegda-0.1.3/docs/installation.rst` & `tegda-0.1.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tegda-0.1.3/docs/make.bat` & `tegda-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tegda-0.1.3/setup.py` & `tegda-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='tegda',
     name='tegda',
     packages=find_packages(include=['tegda', 'tegda.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Robertoarce/tegda',
-    version='0.1.3',
+    version='0.1.4',
     zip_safe=False,
 )
```

### Comparing `tegda-0.1.3/tegda/__init__.py` & `tegda-0.1.4/tegda/__init__.py`

 * *Files identical despite different names*

### Comparing `tegda-0.1.3/tegda/utils.py` & `tegda-0.1.4/tegda/utils.py`

 * *Files identical despite different names*

### Comparing `tegda-0.1.3/tegda.egg-info/PKG-INFO` & `tegda-0.1.4/tegda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: tegda
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tegda creates customizable visual representations of data for exploratory analysis.
 Home-page: https://github.com/Robertoarce/tegda
 Author: Roberto Arce Aguirre
 Author-email: roberto_arce_@hotmail.com
 License: MIT license
 Description: =============
         Terrific EGDA
```

### Comparing `tegda-0.1.3/tegda.egg-info/SOURCES.txt` & `tegda-0.1.4/tegda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tegda-0.1.3/tests/test_tegda.py` & `tegda-0.1.4/tests/test_tegda.py`

 * *Files identical despite different names*

