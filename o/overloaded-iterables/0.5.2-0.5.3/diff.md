# Comparing `tmp/overloaded-iterables-0.5.2.tar.gz` & `tmp/overloaded-iterables-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overloaded-iterables-0.5.2.tar", last modified: Sun Apr 30 00:39:58 2023, max compression
+gzip compressed data, was "overloaded-iterables-0.5.3.tar", last modified: Sun Apr 30 01:18:37 2023, max compression
```

## Comparing `overloaded-iterables-0.5.2.tar` & `overloaded-iterables-0.5.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 00:39:58.715029 overloaded-iterables-0.5.2/
--rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.5.2/LICENSE
--rw-rw-rw-   0        0        0      453 2023-04-30 00:39:58.715029 overloaded-iterables-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     2203 2023-04-29 23:51:55.000000 overloaded-iterables-0.5.2/README.md
--rw-rw-rw-   0        0        0      111 2023-04-30 00:39:58.717029 overloaded-iterables-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0      674 2023-04-30 00:39:53.000000 overloaded-iterables-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 00:39:58.694034 overloaded-iterables-0.5.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 00:39:58.699033 overloaded-iterables-0.5.2/src/overloaded_iterables/
--rw-rw-rw-   0        0        0        0 2023-04-29 23:52:39.000000 overloaded-iterables-0.5.2/src/overloaded_iterables/__init__.py
--rw-rw-rw-   0        0        0     2495 2023-04-29 23:53:26.000000 overloaded-iterables-0.5.2/src/overloaded_iterables/classes.py
-drwxrwxrwx   0        0        0        0 2023-04-30 00:39:58.712032 overloaded-iterables-0.5.2/src/overloaded_iterables.egg-info/
--rw-rw-rw-   0        0        0      453 2023-04-30 00:39:58.000000 overloaded-iterables-0.5.2/src/overloaded_iterables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-04-30 00:39:58.000000 overloaded-iterables-0.5.2/src/overloaded_iterables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 00:39:58.000000 overloaded-iterables-0.5.2/src/overloaded_iterables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-30 00:39:58.000000 overloaded-iterables-0.5.2/src/overloaded_iterables.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-30 00:39:58.714029 overloaded-iterables-0.5.2/src/tests/
--rw-rw-rw-   0        0        0        0 2023-04-29 11:33:17.000000 overloaded-iterables-0.5.2/src/tests/__init__.py
--rw-rw-rw-   0        0        0     3857 2023-04-29 21:09:32.000000 overloaded-iterables-0.5.2/src/tests/test_overloaded_iterables.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:18:37.050502 overloaded-iterables-0.5.3/
+-rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.5.3/LICENSE
+-rw-rw-rw-   0        0        0      614 2023-04-30 01:18:37.050502 overloaded-iterables-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2203 2023-04-29 23:51:55.000000 overloaded-iterables-0.5.3/README.md
+-rw-rw-rw-   0        0        0      111 2023-04-30 01:18:37.052502 overloaded-iterables-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      881 2023-04-30 01:18:29.000000 overloaded-iterables-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:18:37.018504 overloaded-iterables-0.5.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 01:18:37.027500 overloaded-iterables-0.5.3/src/overloaded_iterables/
+-rw-rw-rw-   0        0        0        0 2023-04-29 23:52:39.000000 overloaded-iterables-0.5.3/src/overloaded_iterables/__init__.py
+-rw-rw-rw-   0        0        0     2495 2023-04-29 23:53:26.000000 overloaded-iterables-0.5.3/src/overloaded_iterables/classes.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:18:37.046497 overloaded-iterables-0.5.3/src/overloaded_iterables.egg-info/
+-rw-rw-rw-   0        0        0      614 2023-04-30 01:18:36.000000 overloaded-iterables-0.5.3/src/overloaded_iterables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-04-30 01:18:36.000000 overloaded-iterables-0.5.3/src/overloaded_iterables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 01:18:36.000000 overloaded-iterables-0.5.3/src/overloaded_iterables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-30 01:18:36.000000 overloaded-iterables-0.5.3/src/overloaded_iterables.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 01:18:37.049502 overloaded-iterables-0.5.3/src/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-29 11:33:17.000000 overloaded-iterables-0.5.3/src/tests/__init__.py
+-rw-rw-rw-   0        0        0     3857 2023-04-29 21:09:32.000000 overloaded-iterables-0.5.3/src/tests/test_overloaded_iterables.py
```

### Comparing `overloaded-iterables-0.5.2/LICENSE` & `overloaded-iterables-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.5.2/README.md` & `overloaded-iterables-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.5.2/setup.py` & `overloaded-iterables-0.5.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='overloaded-iterables',
-    version='0.5.2',
+    version='0.5.3',
     description="Overloaded version of the built-in python classes: <list> and <set> to include some extra functionalities.",
+    long_description="Overloaded version of the built-in python classes: <list> and <set> to include some extra functionalities such as"\
+        "<class>.mean(), <class>.rms(), <class>.raise_to(), etc.",
     license='MIT',
     author="Prithoo Medhi",
     author_email='prithoo11335@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/Arkiralor/overloaded_iterables',
     keywords= [
```

### Comparing `overloaded-iterables-0.5.2/src/overloaded_iterables/classes.py` & `overloaded-iterables-0.5.3/src/overloaded_iterables/classes.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.5.2/src/tests/test_overloaded_iterables.py` & `overloaded-iterables-0.5.3/src/tests/test_overloaded_iterables.py`

 * *Files identical despite different names*

