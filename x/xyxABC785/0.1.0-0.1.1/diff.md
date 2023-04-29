# Comparing `tmp/xyxABC785-0.1.0.tar.gz` & `tmp/xyxABC785-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xyxABC785-0.1.0.tar", last modified: Sat Apr 29 22:37:18 2023, max compression
+gzip compressed data, was "xyxABC785-0.1.1.tar", last modified: Sat Apr 29 22:57:24 2023, max compression
```

## Comparing `xyxABC785-0.1.0.tar` & `xyxABC785-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 22:37:18.080487 xyxABC785-0.1.0/
--rw-rw-rw-   0        0        0      158 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3676 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1087 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1727 2023-04-29 22:37:18.081487 xyxABC785-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      919 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-29 22:37:18.018525 xyxABC785-0.1.0/docs/
--rw-rw-rw-   0        0        0      630 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/docs/authors.rst
--rw-rw-rw-   0        0        0     4960 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/docs/history.rst
--rw-rw-rw-   0        0        0      329 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/docs/index.rst
--rw-rw-rw-   0        0        0     1182 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/docs/installation.rst
--rwxrwxrwx   0        0        0      807 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/docs/readme.rst
--rw-rw-rw-   0        0        0       83 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/docs/usage.rst
--rw-rw-rw-   0        0        0      404 2023-04-29 22:37:18.084485 xyxABC785-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1286 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:37:18.022523 xyxABC785-0.1.0/tests/
--rw-rw-rw-   0        0        0       40 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      418 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/tests/test_xyxABC785.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:37:18.025521 xyxABC785-0.1.0/xyxABC785/
--rw-rw-rw-   0        0        0      124 2023-04-29 22:28:33.000000 xyxABC785-0.1.0/xyxABC785/__init__.py
--rw-rw-rw-   0        0        0      106 2023-04-29 22:34:04.000000 xyxABC785-0.1.0/xyxABC785/xyxABC785.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:37:18.079488 xyxABC785-0.1.0/xyxABC785.egg-info/
--rw-rw-rw-   0        0        0     1727 2023-04-29 22:37:17.000000 xyxABC785-0.1.0/xyxABC785.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2023-04-29 22:37:17.000000 xyxABC785-0.1.0/xyxABC785.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 22:37:17.000000 xyxABC785-0.1.0/xyxABC785.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-29 22:37:17.000000 xyxABC785-0.1.0/xyxABC785.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-04-29 22:37:17.000000 xyxABC785-0.1.0/xyxABC785.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 22:57:24.834492 xyxABC785-0.1.1/
+-rw-rw-rw-   0        0        0      158 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3676 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1087 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1727 2023-04-29 22:57:24.834492 xyxABC785-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      919 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-29 22:57:24.796516 xyxABC785-0.1.1/docs/
+-rw-rw-rw-   0        0        0      630 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/docs/authors.rst
+-rw-rw-rw-   0        0        0     4960 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/docs/history.rst
+-rw-rw-rw-   0        0        0      329 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/docs/index.rst
+-rw-rw-rw-   0        0        0     1182 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/docs/installation.rst
+-rwxrwxrwx   0        0        0      807 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/docs/readme.rst
+-rw-rw-rw-   0        0        0       83 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/docs/usage.rst
+-rw-rw-rw-   0        0        0      404 2023-04-29 22:57:24.838491 xyxABC785-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1286 2023-04-29 22:57:06.000000 xyxABC785-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:57:24.801513 xyxABC785-0.1.1/tests/
+-rw-rw-rw-   0        0        0       40 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      418 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/tests/test_xyxABC785.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:57:24.805510 xyxABC785-0.1.1/xyxABC785/
+-rw-rw-rw-   0        0        0      124 2023-04-29 22:28:33.000000 xyxABC785-0.1.1/xyxABC785/__init__.py
+-rw-rw-rw-   0        0        0      106 2023-04-29 22:34:04.000000 xyxABC785-0.1.1/xyxABC785/xyxABC785.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:57:24.832494 xyxABC785-0.1.1/xyxABC785.egg-info/
+-rw-rw-rw-   0        0        0     1727 2023-04-29 22:57:24.000000 xyxABC785-0.1.1/xyxABC785.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2023-04-29 22:57:24.000000 xyxABC785-0.1.1/xyxABC785.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 22:57:24.000000 xyxABC785-0.1.1/xyxABC785.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-29 22:37:17.000000 xyxABC785-0.1.1/xyxABC785.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-04-29 22:57:24.000000 xyxABC785-0.1.1/xyxABC785.egg-info/top_level.txt
```

### Comparing `xyxABC785-0.1.0/CONTRIBUTING.rst` & `xyxABC785-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xyxABC785-0.1.0/LICENSE` & `xyxABC785-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xyxABC785-0.1.0/PKG-INFO` & `xyxABC785-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyxABC785
-Version: 0.1.0
+Version: 0.1.1
 Summary: just testing, how to upload the package
 Home-page: https://github.com/abcXyz/xyxABC785
 Author: abcXyz
 Author-email: xyz@gmail.com
 License: MIT license
 Keywords: xyxABC785
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `xyxABC785-0.1.0/README.rst` & `xyxABC785-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `xyxABC785-0.1.0/docs/Makefile` & `xyxABC785-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xyxABC785-0.1.0/docs/conf.py` & `xyxABC785-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xyxABC785-0.1.0/docs/installation.rst` & `xyxABC785-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `xyxABC785-0.1.0/docs/make.bat` & `xyxABC785-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xyxABC785-0.1.0/setup.py` & `xyxABC785-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='xyxABC785',
     name='xyxABC785',
     packages=find_packages(include=['xyxABC785', 'xyxABC785.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/abcXyz/xyxABC785',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

### Comparing `xyxABC785-0.1.0/xyxABC785.egg-info/PKG-INFO` & `xyxABC785-0.1.1/xyxABC785.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyxABC785
-Version: 0.1.0
+Version: 0.1.1
 Summary: just testing, how to upload the package
 Home-page: https://github.com/abcXyz/xyxABC785
 Author: abcXyz
 Author-email: xyz@gmail.com
 License: MIT license
 Keywords: xyxABC785
 Classifier: Development Status :: 2 - Pre-Alpha
```

