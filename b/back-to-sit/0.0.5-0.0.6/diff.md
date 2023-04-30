# Comparing `tmp/back_to_sit-0.0.5.tar.gz` & `tmp/back_to_sit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "back_to_sit-0.0.5.tar", last modified: Sun Apr 30 15:29:38 2023, max compression
+gzip compressed data, was "back_to_sit-0.0.6.tar", last modified: Sun Apr 30 15:41:50 2023, max compression
```

## Comparing `back_to_sit-0.0.5.tar` & `back_to_sit-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 15:29:38.725558 back_to_sit-0.0.5/
--rw-r--r--   0 diegulio   (501) staff       (20)     1065 2023-03-16 05:01:50.000000 back_to_sit-0.0.5/LICENSE
--rw-r--r--   0 diegulio   (501) staff       (20)      281 2023-04-30 15:29:38.725385 back_to_sit-0.0.5/PKG-INFO
--rw-r--r--   0 diegulio   (501) staff       (20)       84 2023-03-16 05:01:50.000000 back_to_sit-0.0.5/README.md
-drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 15:29:38.724180 back_to_sit-0.0.5/back_to_sit/
--rw-r--r--   0 diegulio   (501) staff       (20)       59 2023-03-18 22:50:18.000000 back_to_sit-0.0.5/back_to_sit/__init__.py
--rw-r--r--   0 diegulio   (501) staff       (20)     1377 2023-04-30 15:23:05.000000 back_to_sit-0.0.5/back_to_sit/back_to_sit.py
-drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 15:29:38.725168 back_to_sit-0.0.5/back_to_sit.egg-info/
--rw-r--r--   0 diegulio   (501) staff       (20)      281 2023-04-30 15:29:38.000000 back_to_sit-0.0.5/back_to_sit.egg-info/PKG-INFO
--rw-r--r--   0 diegulio   (501) staff       (20)      266 2023-04-30 15:29:38.000000 back_to_sit-0.0.5/back_to_sit.egg-info/SOURCES.txt
--rw-r--r--   0 diegulio   (501) staff       (20)        1 2023-04-30 15:29:38.000000 back_to_sit-0.0.5/back_to_sit.egg-info/dependency_links.txt
--rw-r--r--   0 diegulio   (501) staff       (20)        9 2023-04-30 15:29:38.000000 back_to_sit-0.0.5/back_to_sit.egg-info/requires.txt
--rw-r--r--   0 diegulio   (501) staff       (20)       12 2023-04-30 15:29:38.000000 back_to_sit-0.0.5/back_to_sit.egg-info/top_level.txt
--rw-r--r--   0 diegulio   (501) staff       (20)      354 2023-04-30 15:21:22.000000 back_to_sit-0.0.5/pyproject.toml
--rw-r--r--   0 diegulio   (501) staff       (20)       38 2023-04-30 15:29:38.725621 back_to_sit-0.0.5/setup.cfg
--rw-r--r--   0 diegulio   (501) staff       (20)      732 2023-04-30 15:21:38.000000 back_to_sit-0.0.5/setup.py
+drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 15:41:50.593331 back_to_sit-0.0.6/
+-rw-r--r--   0 diegulio   (501) staff       (20)     1065 2023-03-16 05:01:50.000000 back_to_sit-0.0.6/LICENSE
+-rw-r--r--   0 diegulio   (501) staff       (20)      281 2023-04-30 15:41:50.593184 back_to_sit-0.0.6/PKG-INFO
+-rw-r--r--   0 diegulio   (501) staff       (20)       84 2023-03-16 05:01:50.000000 back_to_sit-0.0.6/README.md
+drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 15:41:50.592088 back_to_sit-0.0.6/back_to_sit/
+-rw-r--r--   0 diegulio   (501) staff       (20)       59 2023-03-18 22:50:18.000000 back_to_sit-0.0.6/back_to_sit/__init__.py
+-rw-r--r--   0 diegulio   (501) staff       (20)     1377 2023-04-30 15:23:05.000000 back_to_sit-0.0.6/back_to_sit/back_to_sit.py
+drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 15:41:50.592979 back_to_sit-0.0.6/back_to_sit.egg-info/
+-rw-r--r--   0 diegulio   (501) staff       (20)      281 2023-04-30 15:41:50.000000 back_to_sit-0.0.6/back_to_sit.egg-info/PKG-INFO
+-rw-r--r--   0 diegulio   (501) staff       (20)      266 2023-04-30 15:41:50.000000 back_to_sit-0.0.6/back_to_sit.egg-info/SOURCES.txt
+-rw-r--r--   0 diegulio   (501) staff       (20)        1 2023-04-30 15:41:50.000000 back_to_sit-0.0.6/back_to_sit.egg-info/dependency_links.txt
+-rw-r--r--   0 diegulio   (501) staff       (20)        9 2023-04-30 15:41:50.000000 back_to_sit-0.0.6/back_to_sit.egg-info/requires.txt
+-rw-r--r--   0 diegulio   (501) staff       (20)       12 2023-04-30 15:41:50.000000 back_to_sit-0.0.6/back_to_sit.egg-info/top_level.txt
+-rw-r--r--   0 diegulio   (501) staff       (20)      355 2023-04-30 15:41:38.000000 back_to_sit-0.0.6/pyproject.toml
+-rw-r--r--   0 diegulio   (501) staff       (20)       38 2023-04-30 15:41:50.593375 back_to_sit-0.0.6/setup.cfg
+-rw-r--r--   0 diegulio   (501) staff       (20)      732 2023-04-30 15:41:33.000000 back_to_sit-0.0.6/setup.py
```

### Comparing `back_to_sit-0.0.5/LICENSE` & `back_to_sit-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `back_to_sit-0.0.5/back_to_sit/back_to_sit.py` & `back_to_sit-0.0.6/back_to_sit/back_to_sit.py`

 * *Files identical despite different names*

### Comparing `back_to_sit-0.0.5/setup.py` & `back_to_sit-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5' 
+VERSION = '0.0.6' 
 DESCRIPTION = 'Back to sit when the your code is ready'
 LONG_DESCRIPTION = 'A package that send a message to your telegram when your code is ready'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="back_to_sit",
```

