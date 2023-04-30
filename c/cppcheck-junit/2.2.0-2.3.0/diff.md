# Comparing `tmp/cppcheck-junit-2.2.0.tar.gz` & `tmp/cppcheck-junit-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cppcheck-junit-2.2.0.tar", last modified: Tue Mar 29 23:27:25 2022, max compression
+gzip compressed data, was "cppcheck-junit-2.3.0.tar", last modified: Sun Apr 30 19:12:51 2023, max compression
```

## Comparing `cppcheck-junit-2.2.0.tar` & `cppcheck-junit-2.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-03-29 23:27:25.078405 cppcheck-junit-2.2.0/
--rw-rw-rw-   0        0        0     1070 2022-03-29 23:05:43.000000 cppcheck-junit-2.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0       46 2022-03-29 23:25:16.000000 cppcheck-junit-2.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4515 2022-03-29 23:27:25.078405 cppcheck-junit-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3467 2022-03-29 23:26:44.000000 cppcheck-junit-2.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-03-29 23:27:25.077407 cppcheck-junit-2.2.0/cppcheck_junit.egg-info/
--rw-rw-rw-   0        0        0     4515 2022-03-29 23:27:24.000000 cppcheck-junit-2.2.0/cppcheck_junit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2022-03-29 23:27:25.000000 cppcheck-junit-2.2.0/cppcheck_junit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-29 23:27:24.000000 cppcheck-junit-2.2.0/cppcheck_junit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2022-03-29 23:27:24.000000 cppcheck-junit-2.2.0/cppcheck_junit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-03-29 23:27:23.000000 cppcheck-junit-2.2.0/cppcheck_junit.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2022-03-29 23:27:24.000000 cppcheck-junit-2.2.0/cppcheck_junit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-03-29 23:27:24.000000 cppcheck-junit-2.2.0/cppcheck_junit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6416 2022-03-29 23:05:43.000000 cppcheck-junit-2.2.0/cppcheck_junit.py
--rw-rw-rw-   0        0        0      426 2022-03-29 23:22:24.000000 cppcheck-junit-2.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       17 2022-03-29 23:05:43.000000 cppcheck-junit-2.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-03-29 23:27:25.078405 cppcheck-junit-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1406 2022-03-29 23:26:03.000000 cppcheck-junit-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 19:12:51.057879 cppcheck-junit-2.3.0/
+-rw-rw-rw-   0        0        0     1070 2022-03-29 23:05:43.000000 cppcheck-junit-2.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       46 2022-03-29 23:25:16.000000 cppcheck-junit-2.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4590 2023-04-30 19:12:51.057879 cppcheck-junit-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3562 2023-04-30 19:12:05.000000 cppcheck-junit-2.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-30 19:12:51.055879 cppcheck-junit-2.3.0/cppcheck_junit.egg-info/
+-rw-rw-rw-   0        0        0     4590 2023-04-30 19:12:51.000000 cppcheck-junit-2.3.0/cppcheck_junit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-04-30 19:12:51.000000 cppcheck-junit-2.3.0/cppcheck_junit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 19:12:51.000000 cppcheck-junit-2.3.0/cppcheck_junit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-30 19:12:51.000000 cppcheck-junit-2.3.0/cppcheck_junit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-30 19:12:50.000000 cppcheck-junit-2.3.0/cppcheck_junit.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-04-30 19:12:51.000000 cppcheck-junit-2.3.0/cppcheck_junit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-30 19:12:51.000000 cppcheck-junit-2.3.0/cppcheck_junit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6416 2022-03-29 23:05:43.000000 cppcheck-junit-2.3.0/cppcheck_junit.py
+-rw-rw-rw-   0        0        0      486 2023-04-30 19:09:56.000000 cppcheck-junit-2.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       17 2022-03-29 23:05:43.000000 cppcheck-junit-2.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 19:12:51.057879 cppcheck-junit-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1407 2023-04-30 19:12:05.000000 cppcheck-junit-2.3.0/setup.py
```

### Comparing `cppcheck-junit-2.2.0/LICENSE.txt` & `cppcheck-junit-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cppcheck-junit-2.2.0/PKG-INFO` & `cppcheck-junit-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: cppcheck-junit
-Version: 2.2.0
+Version: 2.3.0
 Summary: Converts Cppcheck XML output to JUnit format.
 Home-page: https://github.com/johnthagen/cppcheck-junit
 Author: John Hagen
 Author-email: johnthagen@gmail.com
 License: MIT
 Keywords: Cppcheck C++ JUnit
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 
 cppcheck JUnit Converter
 ========================
 
 .. image:: https://github.com/johnthagen/cppcheck-junit/workflows/python/badge.svg
     :target: https://github.com/johnthagen/cppcheck-junit/actions
@@ -77,14 +76,19 @@
 
 If no ``cppcheck`` errors are generated, a single ``"Cppcheck success"`` test case is
 output so that CI tools like Bamboo will not fail on the JUnit task.
 
 Releases
 --------
 
+2.3.0 - 2023-04-30
+^^^^^^^^^^^^^^^^^^
+
+- Drop Python 3.7 support and support Python 3.11
+
 2.2.0 - 2022-03-29
 ^^^^^^^^^^^^^^^^^^
 
 - Add optional argument for setting return code when cppcheck found errors.
 - Drop Python 3.6 and support Python 3.10.
 
 2.1.0 - 2020-12-30
@@ -155,8 +159,7 @@
 
 Added severity to JUnit message, improved help description, handle XML parsing errors.
 
 0.1.0 - 2015-11-15
 ^^^^^^^^^^^^^^^^^^
 
 First release.
-
```

### Comparing `cppcheck-junit-2.2.0/README.rst` & `cppcheck-junit-2.3.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,19 @@
 
 If no ``cppcheck`` errors are generated, a single ``"Cppcheck success"`` test case is
 output so that CI tools like Bamboo will not fail on the JUnit task.
 
 Releases
 --------
 
+2.3.0 - 2023-04-30
+^^^^^^^^^^^^^^^^^^
+
+- Drop Python 3.7 support and support Python 3.11
+
 2.2.0 - 2022-03-29
 ^^^^^^^^^^^^^^^^^^
 
 - Add optional argument for setting return code when cppcheck found errors.
 - Drop Python 3.6 and support Python 3.10.
 
 2.1.0 - 2020-12-30
```

### Comparing `cppcheck-junit-2.2.0/cppcheck_junit.egg-info/PKG-INFO` & `cppcheck-junit-2.3.0/cppcheck_junit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: cppcheck-junit
-Version: 2.2.0
+Version: 2.3.0
 Summary: Converts Cppcheck XML output to JUnit format.
 Home-page: https://github.com/johnthagen/cppcheck-junit
 Author: John Hagen
 Author-email: johnthagen@gmail.com
 License: MIT
 Keywords: Cppcheck C++ JUnit
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 
 cppcheck JUnit Converter
 ========================
 
 .. image:: https://github.com/johnthagen/cppcheck-junit/workflows/python/badge.svg
     :target: https://github.com/johnthagen/cppcheck-junit/actions
@@ -77,14 +76,19 @@
 
 If no ``cppcheck`` errors are generated, a single ``"Cppcheck success"`` test case is
 output so that CI tools like Bamboo will not fail on the JUnit task.
 
 Releases
 --------
 
+2.3.0 - 2023-04-30
+^^^^^^^^^^^^^^^^^^
+
+- Drop Python 3.7 support and support Python 3.11
+
 2.2.0 - 2022-03-29
 ^^^^^^^^^^^^^^^^^^
 
 - Add optional argument for setting return code when cppcheck found errors.
 - Drop Python 3.6 and support Python 3.10.
 
 2.1.0 - 2020-12-30
@@ -155,8 +159,7 @@
 
 Added severity to JUnit message, improved help description, handle XML parsing errors.
 
 0.1.0 - 2015-11-15
 ^^^^^^^^^^^^^^^^^^
 
 First release.
-
```

### Comparing `cppcheck-junit-2.2.0/cppcheck_junit.py` & `cppcheck-junit-2.3.0/cppcheck_junit.py`

 * *Files identical despite different names*

### Comparing `cppcheck-junit-2.2.0/setup.py` & `cppcheck-junit-2.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from setuptools import setup
 
 setup(
     name="cppcheck-junit",
-    version="2.2.0",
+    version="2.3.0",
     description="Converts Cppcheck XML output to JUnit format.",
     long_description=open("README.rst").read(),
     keywords="Cppcheck C++ JUnit",
     author="John Hagen",
     author_email="johnthagen@gmail.com",
     url="https://github.com/johnthagen/cppcheck-junit",
     py_modules=["cppcheck_junit"],
     install_requires=open("requirements.txt").readlines(),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     zip_safe=False,
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: C++",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Quality Assurance",
     ],
     scripts=["cppcheck_junit.py"],
     entry_points={
         "console_scripts": [
             "cppcheck_junit = cppcheck_junit:main",
         ],
```

