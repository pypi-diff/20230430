# Comparing `tmp/atppy-0.1.tar.gz` & `tmp/atppy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atppy-0.1.tar", last modified: Sat Apr 29 19:51:50 2023, max compression
+gzip compressed data, was "atppy-0.1.1.tar", last modified: Sun Apr 30 06:11:07 2023, max compression
```

## Comparing `atppy-0.1.tar` & `atppy-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxr-xr-x   0 josephfarrell   (501) staff       (20)        0 2023-04-29 19:51:50.896228 atppy-0.1/
--rw-r--r--   0 josephfarrell   (501) staff       (20)      597 2023-04-29 19:51:50.896270 atppy-0.1/PKG-INFO
-drwxr-xr-x   0 josephfarrell   (501) staff       (20)        0 2023-04-29 19:51:50.896199 atppy-0.1/atppy/
--rw-r--r--   0 josephfarrell   (501) staff       (20)      114 2023-04-29 03:40:42.255043 atppy-0.1/atppy/__init__.py
--rw-r--r--   0 josephfarrell   (501) staff       (20)       39 2023-04-29 04:24:57.772239 atppy-0.1/setup.cfg
--rw-r--r--   0 josephfarrell   (501) staff       (20)      654 2023-04-29 04:31:47.602906 atppy-0.1/setup.py
+drwxr-xr-x   0 josephfarrell   (501) staff       (20)        0 2023-04-30 06:11:07.707083 atppy-0.1.1/
+-rw-r--r--   0 josephfarrell   (501) staff       (20)      599 2023-04-30 06:11:07.707153 atppy-0.1.1/PKG-INFO
+drwxr-xr-x   0 josephfarrell   (501) staff       (20)        0 2023-04-30 06:11:07.707049 atppy-0.1.1/atppy/
+-rw-r--r--   0 josephfarrell   (501) staff       (20)      147 2023-04-30 06:05:47.458512 atppy-0.1.1/atppy/__init__.py
+-rw-r--r--   0 josephfarrell   (501) staff       (20)       39 2023-04-29 04:24:57.772239 atppy-0.1.1/setup.cfg
+-rw-r--r--   0 josephfarrell   (501) staff       (20)      656 2023-04-30 06:05:09.146827 atppy-0.1.1/setup.py
```

### Comparing `atppy-0.1/PKG-INFO` & `atppy-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: atppy
-Version: 0.1
+Version: 0.1.1
 Summary: Python library for AT Protocol
 Home-page: https://github.com/Gladdstone/atppy
 Author: Joseph Farrell
 Author-email: joe.farrell373@gmail.com
 License: MIT
 Download-URL: https://github.com/Gladdstone/atppy/archive/v_01.tar.gz
 Description: UNKNOWN
```

### Comparing `atppy-0.1/setup.py` & `atppy-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'atppy',
   packages = ['atppy'],
-  version = '0.1',
+  version = '0.1.1',
   license='MIT',
   description = 'Python library for AT Protocol',
   author = 'Joseph Farrell',
   author_email = 'joe.farrell373@gmail.com',
   url = 'https://github.com/Gladdstone/atppy',
   download_url = 'https://github.com/Gladdstone/atppy/archive/v_01.tar.gz',
   keywords = ['at protocol', 'bluesky', 'bsky'],
```

