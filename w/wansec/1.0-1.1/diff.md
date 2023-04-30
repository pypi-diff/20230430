# Comparing `tmp/wansec-1.0.tar.gz` & `tmp/wansec-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wansec-1.0.tar", last modified: Sun Apr 30 10:50:03 2023, max compression
+gzip compressed data, was "wansec-1.1.tar", last modified: Sun Apr 30 11:02:13 2023, max compression
```

## Comparing `wansec-1.0.tar` & `wansec-1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-30 10:50:03.071740 wansec-1.0/
--rw-rw----   0 root         (0) everybody  (9997)      373 2023-04-30 10:50:03.071740 wansec-1.0/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-30 10:50:03.071740 wansec-1.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      547 2023-04-30 10:49:55.000000 wansec-1.0/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-30 10:50:03.071740 wansec-1.0/wansec.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      373 2023-04-30 10:50:02.000000 wansec-1.0/wansec.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      157 2023-04-30 10:50:02.000000 wansec-1.0/wansec.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-30 10:50:02.000000 wansec-1.0/wansec.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       17 2023-04-30 10:50:02.000000 wansec-1.0/wansec.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-30 10:50:02.000000 wansec-1.0/wansec.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-30 11:02:13.091740 wansec-1.1/
+-rw-rw----   0 root         (0) everybody  (9997)      373 2023-04-30 11:02:13.091740 wansec-1.1/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-30 11:02:13.091740 wansec-1.1/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      547 2023-04-30 10:58:50.000000 wansec-1.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-30 11:02:13.091740 wansec-1.1/wansec.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      373 2023-04-30 11:02:12.000000 wansec-1.1/wansec.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      157 2023-04-30 11:02:12.000000 wansec-1.1/wansec.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-30 11:02:12.000000 wansec-1.1/wansec.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       17 2023-04-30 11:02:12.000000 wansec-1.1/wansec.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-30 11:02:12.000000 wansec-1.1/wansec.egg-info/top_level.txt
```

### Comparing `wansec-1.0/setup.py` & `wansec-1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='wansec',
-    version='1.0',
+    version='1.1',
     description='None',
     author='Aoda',
     author_email='febyzamsee@gmail.com',
     packages=find_packages(),
     install_requires=[
         'requests>=2.29.0',
     ],
```

