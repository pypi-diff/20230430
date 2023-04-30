# Comparing `tmp/prepup-0.0.1.tar.gz` & `tmp/prepup-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prepup-0.0.1.tar", last modified: Sat Apr 29 22:42:27 2023, max compression
+gzip compressed data, was "prepup-0.0.2.tar", last modified: Sat Apr 29 23:02:06 2023, max compression
```

## Comparing `prepup-0.0.1.tar` & `prepup-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 22:42:27.079681 prepup-0.0.1/
--rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 prepup-0.0.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 prepup-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 prepup-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1367 2023-04-29 22:42:27.079681 prepup-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-04-29 20:41:27.000000 prepup-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 22:42:27.058837 prepup-0.0.1/prepup/
--rw-rw-rw-   0        0        0      148 2023-04-29 20:41:27.000000 prepup-0.0.1/prepup/__init__.py
--rw-rw-rw-   0        0        0    27774 2023-04-29 22:23:28.000000 prepup-0.0.1/prepup/common.py
--rw-rw-rw-   0        0        0     5349 2023-04-29 22:20:45.000000 prepup-0.0.1/prepup/prepup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:42:27.073162 prepup-0.0.1/prepup.egg-info/
--rw-rw-rw-   0        0        0     1367 2023-04-29 22:42:26.000000 prepup-0.0.1/prepup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-04-29 22:42:26.000000 prepup-0.0.1/prepup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      348 2023-04-29 22:42:26.000000 prepup-0.0.1/prepup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-29 22:42:26.000000 prepup-0.0.1/prepup.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      348 2023-04-29 22:42:26.000000 prepup-0.0.1/prepup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-29 22:42:26.000000 prepup-0.0.1/prepup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      367 2023-04-29 22:38:23.000000 prepup-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      414 2023-04-29 22:42:27.081693 prepup-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1864 2023-04-29 20:41:27.000000 prepup-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:42:27.076681 prepup-0.0.1/tests/
--rw-rw-rw-   0        0        0      403 2023-04-29 20:41:27.000000 prepup-0.0.1/tests/test_prepup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 23:02:06.737571 prepup-0.0.2/
+-rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 prepup-0.0.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 prepup-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 prepup-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1367 2023-04-29 23:02:06.738571 prepup-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-04-29 20:41:27.000000 prepup-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 23:02:06.714106 prepup-0.0.2/prepup/
+-rw-rw-rw-   0        0        0      148 2023-04-29 20:41:27.000000 prepup-0.0.2/prepup/__init__.py
+-rw-rw-rw-   0        0        0    27774 2023-04-29 22:23:28.000000 prepup-0.0.2/prepup/common.py
+-rw-rw-rw-   0        0        0     5349 2023-04-29 22:20:45.000000 prepup-0.0.2/prepup/prepup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 23:02:06.734585 prepup-0.0.2/prepup.egg-info/
+-rw-rw-rw-   0        0        0     1367 2023-04-29 23:02:06.000000 prepup-0.0.2/prepup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-04-29 23:02:06.000000 prepup-0.0.2/prepup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      348 2023-04-29 23:02:06.000000 prepup-0.0.2/prepup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-29 22:42:26.000000 prepup-0.0.2/prepup.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      348 2023-04-29 23:02:06.000000 prepup-0.0.2/prepup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-29 23:02:06.000000 prepup-0.0.2/prepup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      367 2023-04-29 23:00:31.000000 prepup-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0      414 2023-04-29 23:02:06.740574 prepup-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1864 2023-04-29 23:02:01.000000 prepup-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 23:02:06.736573 prepup-0.0.2/tests/
+-rw-rw-rw-   0        0        0      403 2023-04-29 20:41:27.000000 prepup-0.0.2/tests/test_prepup.py
```

### Comparing `prepup-0.0.1/LICENSE` & `prepup-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prepup-0.0.1/PKG-INFO` & `prepup-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prepup
-Version: 0.0.1
+Version: 0.0.2
 Summary: Prepup is a free, open-source package that lets you open, explore, visualize and pre-process datasets in your computer's terminal.
 Home-page: https://github.com/sudhanshumukherjeexx/prepup
 Author: Sudhanshu Mukherjee
 Author-email: sudhanshumukherjeexx@gmail.com
 License: MIT license
 Keywords: prepup
 Classifier: Intended Audience :: Developers
```

### Comparing `prepup-0.0.1/prepup/common.py` & `prepup-0.0.2/prepup/common.py`

 * *Files identical despite different names*

### Comparing `prepup-0.0.1/prepup/prepup.py` & `prepup-0.0.2/prepup/prepup.py`

 * *Files identical despite different names*

### Comparing `prepup-0.0.1/prepup.egg-info/PKG-INFO` & `prepup-0.0.2/prepup.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prepup
-Version: 0.0.1
+Version: 0.0.2
 Summary: Prepup is a free, open-source package that lets you open, explore, visualize and pre-process datasets in your computer's terminal.
 Home-page: https://github.com/sudhanshumukherjeexx/prepup
 Author: Sudhanshu Mukherjee
 Author-email: sudhanshumukherjeexx@gmail.com
 License: MIT license
 Keywords: prepup
 Classifier: Intended Audience :: Developers
```

### Comparing `prepup-0.0.1/setup.py` & `prepup-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='prepup',
     name='prepup',
     packages=find_packages(include=['prepup', 'prepup.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/sudhanshumukherjeexx/prepup',
-    version='0.0.1',
+    version='0.0.2',
     zip_safe=False,
 )
```

