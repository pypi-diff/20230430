# Comparing `tmp/aassddee-0.0.2.tar.gz` & `tmp/aassddee-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\aassddee-0.0.2.tar", last modified: Sun Apr 30 00:49:26 2023, max compression
+gzip compressed data, was "dist\aassddee-0.0.3.tar", last modified: Sun Apr 30 09:02:09 2023, max compression
```

## Comparing `aassddee-0.0.2.tar` & `aassddee-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 00:49:26.100933 aassddee-0.0.2/
--rw-rw-rw-   0        0        0      527 2023-04-30 00:49:26.100933 aassddee-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      446 2023-04-29 08:44:47.000000 aassddee-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 00:49:26.044192 aassddee-0.0.2/aassddee/
--rw-rw-rw-   0        0        0      153 2023-04-30 00:44:15.000000 aassddee-0.0.2/aassddee/RF.py
--rw-rw-rw-   0        0        0       25 2023-04-30 00:44:11.000000 aassddee-0.0.2/aassddee/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 00:49:26.096909 aassddee-0.0.2/aassddee.egg-info/
--rw-rw-rw-   0        0        0      527 2023-04-30 00:49:25.000000 aassddee-0.0.2/aassddee.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-04-30 00:49:25.000000 aassddee-0.0.2/aassddee.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 00:49:25.000000 aassddee-0.0.2/aassddee.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-30 00:49:25.000000 aassddee-0.0.2/aassddee.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-30 00:49:25.000000 aassddee-0.0.2/aassddee.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 00:49:26.100933 aassddee-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      651 2023-04-30 00:45:58.000000 aassddee-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 09:02:09.486869 aassddee-0.0.3/
+-rw-rw-rw-   0        0        0      527 2023-04-30 09:02:09.483315 aassddee-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2023-04-29 08:44:47.000000 aassddee-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 09:02:09.387453 aassddee-0.0.3/aassddee/
+-rw-rw-rw-   0        0        0      165 2023-04-30 09:00:44.000000 aassddee-0.0.3/aassddee/RF.py
+-rw-rw-rw-   0        0        0       25 2023-04-30 09:00:57.000000 aassddee-0.0.3/aassddee/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 09:02:09.471078 aassddee-0.0.3/aassddee.egg-info/
+-rw-rw-rw-   0        0        0      527 2023-04-30 09:02:08.000000 aassddee-0.0.3/aassddee.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-04-30 09:02:08.000000 aassddee-0.0.3/aassddee.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 09:02:08.000000 aassddee-0.0.3/aassddee.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-30 09:02:08.000000 aassddee-0.0.3/aassddee.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 09:02:08.000000 aassddee-0.0.3/aassddee.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 09:02:09.486869 aassddee-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      651 2023-04-30 08:58:08.000000 aassddee-0.0.3/setup.py
```

### Comparing `aassddee-0.0.2/PKG-INFO` & `aassddee-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aassddee
-Version: 0.0.2
+Version: 0.0.3
 Summary: for fun
 Home-page: UNKNOWN
 Author: Yizhan
 Author-email: boy87511@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: iris sklearn
```

### Comparing `aassddee-0.0.2/aassddee.egg-info/PKG-INFO` & `aassddee-0.0.3/aassddee.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aassddee
-Version: 0.0.2
+Version: 0.0.3
 Summary: for fun
 Home-page: UNKNOWN
 Author: Yizhan
 Author-email: boy87511@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: iris sklearn
```

### Comparing `aassddee-0.0.2/setup.py` & `aassddee-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aassddee',
-    version='0.0.2',
+    version='0.0.3',
     description='for fun',
     author='Yizhan',
     author_email='boy87511@gmail.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
```

