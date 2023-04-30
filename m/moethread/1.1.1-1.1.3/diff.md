# Comparing `tmp/moethread-1.1.1.tar.gz` & `tmp/moethread-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\moethread-1.1.1.tar", last modified: Fri Dec 16 07:26:50 2022, max compression
+gzip compressed data, was "dist\moethread-1.1.3.tar", last modified: Sun Apr 30 06:02:37 2023, max compression
```

## Comparing `moethread-1.1.1.tar` & `moethread-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-12-16 07:26:50.000000 moethread-1.1.1/
--rw-rw-rw-   0        0        0     7856 2022-12-16 07:26:50.000000 moethread-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5823 2022-11-06 03:31:44.000000 moethread-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-12-16 07:26:50.000000 moethread-1.1.1/moethread/
--rw-rw-rw-   0        0        0       31 2022-11-02 09:17:33.000000 moethread-1.1.1/moethread/__init__.py
--rw-rw-rw-   0        0        0     2340 2022-11-27 05:31:15.000000 moethread-1.1.1/moethread/main.py
-drwxrwxrwx   0        0        0        0 2022-12-16 07:26:50.000000 moethread-1.1.1/moethread.egg-info/
--rw-rw-rw-   0        0        0     7856 2022-12-16 07:26:50.000000 moethread-1.1.1/moethread.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2022-12-16 07:26:50.000000 moethread-1.1.1/moethread.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-16 07:26:50.000000 moethread-1.1.1/moethread.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-12-16 07:26:50.000000 moethread-1.1.1/moethread.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-12-16 07:26:50.000000 moethread-1.1.1/other/
--rw-rw-rw-   0        0        0       31 2022-11-02 09:17:33.000000 moethread-1.1.1/other/__init__.py
--rw-rw-rw-   0        0        0     2340 2022-11-27 05:31:15.000000 moethread-1.1.1/other/main.py
--rw-rw-rw-   0        0        0       42 2022-12-16 07:26:50.000000 moethread-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1139 2022-12-16 07:24:44.000000 moethread-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:02:37.000000 moethread-1.1.3/
+-rw-rw-rw-   0        0        0     7855 2023-04-30 06:02:37.000000 moethread-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5823 2022-11-06 03:31:44.000000 moethread-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 06:02:37.000000 moethread-1.1.3/moethread/
+-rw-rw-rw-   0        0        0      134 2023-02-22 01:29:53.000000 moethread-1.1.3/moethread/__init__.py
+-rw-rw-rw-   0        0        0     3529 2023-04-30 05:57:01.000000 moethread-1.1.3/moethread/main.py
+-rw-rw-rw-   0        0        0     1196 2023-04-30 05:59:40.000000 moethread-1.1.3/moethread/version.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:02:37.000000 moethread-1.1.3/moethread.egg-info/
+-rw-rw-rw-   0        0        0     7855 2023-04-30 06:02:37.000000 moethread-1.1.3/moethread.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-04-30 06:02:37.000000 moethread-1.1.3/moethread.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 06:02:37.000000 moethread-1.1.3/moethread.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-30 06:02:37.000000 moethread-1.1.3/moethread.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 06:02:37.000000 moethread-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1166 2023-04-30 06:02:33.000000 moethread-1.1.3/setup.py
```

### Comparing `moethread-1.1.1/PKG-INFO` & `moethread-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: moethread
-Version: 1.1.1
+Version: 1.1.3
 Summary: Python wrapper for ThreadPoolExecutor to easily multithread resource bound tasks
 Home-page: https://github.com/mhamdan91/moethread
 Author: mhamdan91 (Hamdan, Muhammad)
-Author-email: <mhamdan-91@hotmail.com>
+Author-email: <mhamdan.dev@gmail.com>
 License: UNKNOWN
 Description: Moethread
         =======================================
         ## Table of Contents
         
          * [Overview](#overview)
          * [Library Installalion](#library-installalion)
```

### Comparing `moethread-1.1.1/README.md` & `moethread-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `moethread-1.1.1/moethread.egg-info/PKG-INFO` & `moethread-1.1.3/moethread.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: moethread
-Version: 1.1.1
+Version: 1.1.3
 Summary: Python wrapper for ThreadPoolExecutor to easily multithread resource bound tasks
 Home-page: https://github.com/mhamdan91/moethread
 Author: mhamdan91 (Hamdan, Muhammad)
-Author-email: <mhamdan-91@hotmail.com>
+Author-email: <mhamdan.dev@gmail.com>
 License: UNKNOWN
 Description: Moethread
         =======================================
         ## Table of Contents
         
          * [Overview](#overview)
          * [Library Installalion](#library-installalion)
```

### Comparing `moethread-1.1.1/setup.py` & `moethread-1.1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '1.1.1'
+from moethread.version import __version__
 DESCRIPTION = 'Python wrapper for ThreadPoolExecutor to easily multithread resource bound tasks'
 LONG_DESCRIPTION = open('README.md').read()
 # Setting up
 setup(
     name="moethread",
-    version=VERSION,
+    version=__version__,
     author="mhamdan91 (Hamdan, Muhammad)",
-    author_email="<mhamdan-91@hotmail.com>",
+    author_email="<mhamdan.dev@gmail.com>",
     url='https://github.com/mhamdan91/moethread',
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python', 'multithreading', 'wrappers', 'decorator', 'pool', 'multitasking',
```

