# Comparing `tmp/overloaded-iterables-0.6.1.tar.gz` & `tmp/overloaded-iterables-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overloaded-iterables-0.6.1.tar", last modified: Sun Apr 30 21:21:14 2023, max compression
+gzip compressed data, was "overloaded-iterables-0.6.2.tar", last modified: Sun Apr 30 21:49:20 2023, max compression
```

## Comparing `overloaded-iterables-0.6.1.tar` & `overloaded-iterables-0.6.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 21:21:14.487615 overloaded-iterables-0.6.1/
--rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.6.1/LICENSE
--rw-rw-rw-   0        0        0     7994 2023-04-30 21:21:14.487615 overloaded-iterables-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     7281 2023-04-30 21:17:53.000000 overloaded-iterables-0.6.1/README.md
--rw-rw-rw-   0        0        0      111 2023-04-30 21:21:14.489616 overloaded-iterables-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1477 2023-04-30 21:20:52.000000 overloaded-iterables-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:21:14.472617 overloaded-iterables-0.6.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 21:21:14.477615 overloaded-iterables-0.6.1/src/overloaded_iterables/
--rw-rw-rw-   0        0        0        0 2023-04-29 23:52:39.000000 overloaded-iterables-0.6.1/src/overloaded_iterables/__init__.py
--rw-rw-rw-   0        0        0    13051 2023-04-30 20:19:49.000000 overloaded-iterables-0.6.1/src/overloaded_iterables/classes.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:21:14.486618 overloaded-iterables-0.6.1/src/overloaded_iterables.egg-info/
--rw-rw-rw-   0        0        0     7994 2023-04-30 21:21:14.000000 overloaded-iterables-0.6.1/src/overloaded_iterables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-04-30 21:21:14.000000 overloaded-iterables-0.6.1/src/overloaded_iterables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 21:21:14.000000 overloaded-iterables-0.6.1/src/overloaded_iterables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-30 21:21:14.000000 overloaded-iterables-0.6.1/src/overloaded_iterables.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-30 21:21:14.000000 overloaded-iterables-0.6.1/src/overloaded_iterables.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 21:49:20.196779 overloaded-iterables-0.6.2/
+-rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0     8130 2023-04-30 21:49:20.196779 overloaded-iterables-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7417 2023-04-30 21:49:01.000000 overloaded-iterables-0.6.2/README.md
+-rw-rw-rw-   0        0        0      111 2023-04-30 21:49:20.203783 overloaded-iterables-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1477 2023-04-30 21:49:11.000000 overloaded-iterables-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:49:20.161779 overloaded-iterables-0.6.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 21:49:20.167775 overloaded-iterables-0.6.2/src/overloaded_iterables/
+-rw-rw-rw-   0        0        0        0 2023-04-29 23:52:39.000000 overloaded-iterables-0.6.2/src/overloaded_iterables/__init__.py
+-rw-rw-rw-   0        0        0    13051 2023-04-30 20:19:49.000000 overloaded-iterables-0.6.2/src/overloaded_iterables/classes.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:49:20.195776 overloaded-iterables-0.6.2/src/overloaded_iterables.egg-info/
+-rw-rw-rw-   0        0        0     8130 2023-04-30 21:49:20.000000 overloaded-iterables-0.6.2/src/overloaded_iterables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-04-30 21:49:20.000000 overloaded-iterables-0.6.2/src/overloaded_iterables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 21:49:20.000000 overloaded-iterables-0.6.2/src/overloaded_iterables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-30 21:49:20.000000 overloaded-iterables-0.6.2/src/overloaded_iterables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-30 21:49:20.000000 overloaded-iterables-0.6.2/src/overloaded_iterables.egg-info/top_level.txt
```

### Comparing `overloaded-iterables-0.6.1/LICENSE` & `overloaded-iterables-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.6.1/PKG-INFO` & `overloaded-iterables-0.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overloaded-iterables
-Version: 0.6.1
+Version: 0.6.2
 Summary: Overloaded version of the built-in python classes: list and set to include some extra functionalities.
 Home-page: https://github.com/Arkiralor/overloaded_iterables
 Author: Prithoo Medhi
 Author-email: prithoo11335@gmail.com
 License: MIT
 Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot
 Platform: windows
@@ -14,21 +14,27 @@
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Overloaded Iterables
 
-Overloaded versions of the built-in python classes: `<list>` and `<set>` to include some extra functionalities as an experiment.
+Overloaded versions of the built-in python classes: `<list>` and `<set>`, to include some extra functionalities as an experiment.
+
+An experimental Python package to extend the methods found in Python's built-in list and set classes to add some extra functionality that I, personally find useful in my day-to-day implementations and was too lazy to keep writing/copy-pasting again and again.
 
 ## Specifications
 
-1. __Python Version:__ Python v3.8+
-2. __Code Coverage:__ ![_code coverage_](https://github.com/Arkiralor/overloaded_iterables/blob/master/media/screenshots/coverage.PNG?raw=true)
-3. __Tests Status:__ ![_test status_](https://github.com/Arkiralor/overloaded_iterables/blob/master/media/screenshots/test_results.PNG?raw=true)
+1. __Python Version:__
+
+    _Python v3.8+_
+
+2. __Code Coverage:__
+
+    ![_code coverage_](https://github.com/Arkiralor/overloaded_iterables/blob/master/media/screenshots/coverage.PNG?raw=true)
 
 ## Python Package Index
 
 1. [Project Homepage](https://pypi.org/project/overloaded-iterables/)
 2. [Contents](https://pypi.org/project/overloaded-iterables/#files)
 
 ## Installation
```

### Comparing `overloaded-iterables-0.6.1/README.md` & `overloaded-iterables-0.6.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 # Overloaded Iterables
 
-Overloaded versions of the built-in python classes: `<list>` and `<set>` to include some extra functionalities as an experiment.
+Overloaded versions of the built-in python classes: `<list>` and `<set>`, to include some extra functionalities as an experiment.
+
+An experimental Python package to extend the methods found in Python's built-in list and set classes to add some extra functionality that I, personally find useful in my day-to-day implementations and was too lazy to keep writing/copy-pasting again and again.
 
 ## Specifications
 
-1. __Python Version:__ Python v3.8+
-2. __Code Coverage:__ ![_code coverage_](https://github.com/Arkiralor/overloaded_iterables/blob/master/media/screenshots/coverage.PNG?raw=true)
-3. __Tests Status:__ ![_test status_](https://github.com/Arkiralor/overloaded_iterables/blob/master/media/screenshots/test_results.PNG?raw=true)
+1. __Python Version:__
+
+    _Python v3.8+_
+
+2. __Code Coverage:__
+
+    ![_code coverage_](https://github.com/Arkiralor/overloaded_iterables/blob/master/media/screenshots/coverage.PNG?raw=true)
 
 ## Python Package Index
 
 1. [Project Homepage](https://pypi.org/project/overloaded-iterables/)
 2. [Contents](https://pypi.org/project/overloaded-iterables/#files)
 
 ## Installation
```

### Comparing `overloaded-iterables-0.6.1/setup.py` & `overloaded-iterables-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         encoding="utf-8"
     )as file_obj:
         data = file_obj.read()
     return data
 
 setup(
     name='overloaded-iterables',
-    version='0.6.1',
+    version='0.6.2',
     description="Overloaded version of the built-in python classes: list and set to include some extra functionalities.",
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     license='MIT',
     author="Prithoo Medhi",
     author_email='prithoo11335@gmail.com',
     packages=find_packages('src'),
```

### Comparing `overloaded-iterables-0.6.1/src/overloaded_iterables/classes.py` & `overloaded-iterables-0.6.2/src/overloaded_iterables/classes.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.6.1/src/overloaded_iterables.egg-info/PKG-INFO` & `overloaded-iterables-0.6.2/src/overloaded_iterables.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overloaded-iterables
-Version: 0.6.1
+Version: 0.6.2
 Summary: Overloaded version of the built-in python classes: list and set to include some extra functionalities.
 Home-page: https://github.com/Arkiralor/overloaded_iterables
 Author: Prithoo Medhi
 Author-email: prithoo11335@gmail.com
 License: MIT
 Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot
 Platform: windows
@@ -14,21 +14,27 @@
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Overloaded Iterables
 
-Overloaded versions of the built-in python classes: `<list>` and `<set>` to include some extra functionalities as an experiment.
+Overloaded versions of the built-in python classes: `<list>` and `<set>`, to include some extra functionalities as an experiment.
+
+An experimental Python package to extend the methods found in Python's built-in list and set classes to add some extra functionality that I, personally find useful in my day-to-day implementations and was too lazy to keep writing/copy-pasting again and again.
 
 ## Specifications
 
-1. __Python Version:__ Python v3.8+
-2. __Code Coverage:__ ![_code coverage_](https://github.com/Arkiralor/overloaded_iterables/blob/master/media/screenshots/coverage.PNG?raw=true)
-3. __Tests Status:__ ![_test status_](https://github.com/Arkiralor/overloaded_iterables/blob/master/media/screenshots/test_results.PNG?raw=true)
+1. __Python Version:__
+
+    _Python v3.8+_
+
+2. __Code Coverage:__
+
+    ![_code coverage_](https://github.com/Arkiralor/overloaded_iterables/blob/master/media/screenshots/coverage.PNG?raw=true)
 
 ## Python Package Index
 
 1. [Project Homepage](https://pypi.org/project/overloaded-iterables/)
 2. [Contents](https://pypi.org/project/overloaded-iterables/#files)
 
 ## Installation
```

