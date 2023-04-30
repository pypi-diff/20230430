# Comparing `tmp/namefactory-1.0.2.tar.gz` & `tmp/namefactory-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "namefactory-1.0.2.tar", last modified: Sat Apr 29 18:41:03 2023, max compression
+gzip compressed data, was "namefactory-1.0.3.tar", last modified: Sun Apr 30 19:19:46 2023, max compression
```

## Comparing `namefactory-1.0.2.tar` & `namefactory-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 18:41:03.011200 namefactory-1.0.2/
--rw-rw-rw-   0        0        0      276 2023-04-29 18:41:03.010200 namefactory-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      548 2023-04-29 16:57:32.000000 namefactory-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 18:41:02.990170 namefactory-1.0.2/namefactory.egg-info/
--rw-rw-rw-   0        0        0      276 2023-04-29 18:41:02.000000 namefactory-1.0.2/namefactory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-04-29 18:41:02.000000 namefactory-1.0.2/namefactory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 18:41:02.000000 namefactory-1.0.2/namefactory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-29 18:41:02.000000 namefactory-1.0.2/namefactory.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 18:41:02.000000 namefactory-1.0.2/namefactory.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 18:41:03.011200 namefactory-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-04-29 18:36:50.000000 namefactory-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 19:19:46.188548 namefactory-1.0.3/
+-rw-rw-rw-   0        0        0      276 2023-04-30 19:19:46.186547 namefactory-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2023-04-29 16:57:32.000000 namefactory-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 19:19:46.178633 namefactory-1.0.3/namefactory.egg-info/
+-rw-rw-rw-   0        0        0      276 2023-04-30 19:19:46.000000 namefactory-1.0.3/namefactory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-04-30 19:19:46.000000 namefactory-1.0.3/namefactory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 19:19:46.000000 namefactory-1.0.3/namefactory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-30 19:19:46.000000 namefactory-1.0.3/namefactory.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 19:19:46.000000 namefactory-1.0.3/namefactory.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 19:19:46.188548 namefactory-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-04-30 19:17:10.000000 namefactory-1.0.3/setup.py
```

### Comparing `namefactory-1.0.2/README.md` & `namefactory-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `namefactory-1.0.2/setup.py` & `namefactory-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 PACKAGE_NAME = 'namefactory'
 AUTHOR = 'Alan Reynoso Jacuinde'
 AUTHOR_EMAIL = 'alanelhendakari@gmail.com'
 URL = 'https://www.instagram.com/aw.jacuxx/'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'Una libreria que genera nombres españoles de hombre y mujeres completas'
```

