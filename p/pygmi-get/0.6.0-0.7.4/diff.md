# Comparing `tmp/pygmi-get-0.6.0.tar.gz` & `tmp/pygmi-get-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmi-get-0.6.0.tar", last modified: Sun Apr 30 08:07:23 2023, max compression
+gzip compressed data, was "pygmi-get-0.7.4.tar", last modified: Sun Apr 30 08:08:36 2023, max compression
```

## Comparing `pygmi-get-0.6.0.tar` & `pygmi-get-0.7.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:07:23.830960 pygmi-get-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-30 08:07:23.830960 pygmi-get-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-30 08:07:09.000000 pygmi-get-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:07:23.826960 pygmi-get-0.6.0/pygmi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 08:07:09.000000 pygmi-get-0.6.0/pygmi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-30 08:07:09.000000 pygmi-get-0.6.0/pygmi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-30 08:07:09.000000 pygmi-get-0.6.0/pygmi/pygmi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:07:23.830960 pygmi-get-0.6.0/pygmi_get.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-30 08:07:23.000000 pygmi-get-0.6.0/pygmi_get.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-30 08:07:23.000000 pygmi-get-0.6.0/pygmi_get.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 08:07:23.000000 pygmi-get-0.6.0/pygmi_get.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-30 08:07:23.000000 pygmi-get-0.6.0/pygmi_get.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 08:07:23.000000 pygmi-get-0.6.0/pygmi_get.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 08:07:23.000000 pygmi-get-0.6.0/pygmi_get.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-30 08:07:09.000000 pygmi-get-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 08:07:23.830960 pygmi-get-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-30 08:07:09.000000 pygmi-get-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:08:36.809115 pygmi-get-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-30 08:08:36.809115 pygmi-get-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-30 08:08:24.000000 pygmi-get-0.7.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:08:36.805114 pygmi-get-0.7.4/pygmi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 08:08:24.000000 pygmi-get-0.7.4/pygmi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-30 08:08:24.000000 pygmi-get-0.7.4/pygmi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-30 08:08:24.000000 pygmi-get-0.7.4/pygmi/pygmi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:08:36.809115 pygmi-get-0.7.4/pygmi_get.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-30 08:08:36.000000 pygmi-get-0.7.4/pygmi_get.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-30 08:08:36.000000 pygmi-get-0.7.4/pygmi_get.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 08:08:36.000000 pygmi-get-0.7.4/pygmi_get.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-30 08:08:36.000000 pygmi-get-0.7.4/pygmi_get.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 08:08:36.000000 pygmi-get-0.7.4/pygmi_get.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 08:08:36.000000 pygmi-get-0.7.4/pygmi_get.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-30 08:08:24.000000 pygmi-get-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 08:08:36.809115 pygmi-get-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-30 08:08:24.000000 pygmi-get-0.7.4/setup.py
```

### Comparing `pygmi-get-0.6.0/PKG-INFO` & `pygmi-get-0.7.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmi-get
-Version: 0.6.0
+Version: 0.7.4
 Summary: A simple package installer for Python that eliminates the need for venvs.
 Home-page: https://github.com/AquaQuokka/pygmi
 Author: AquaQuokka
 License: BSD-3-Clause
 
 =============
 Pygmi
```

### Comparing `pygmi-get-0.6.0/pygmi/pygmi.py` & `pygmi-get-0.7.4/pygmi/pygmi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import click
 import os
 import urllib.request
 from urllib.request import urlopen
 import tarfile
 
-__version__ = "0.6.0"
+__version__ = "0.7.4"
 
 @click.group()
 def cli():
     pass
 
 @click.command(name='install')
 @click.argument('package', 'file')
```

### Comparing `pygmi-get-0.6.0/pygmi_get.egg-info/PKG-INFO` & `pygmi-get-0.7.4/pygmi_get.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmi-get
-Version: 0.6.0
+Version: 0.7.4
 Summary: A simple package installer for Python that eliminates the need for venvs.
 Home-page: https://github.com/AquaQuokka/pygmi
 Author: AquaQuokka
 License: BSD-3-Clause
 
 =============
 Pygmi
```

### Comparing `pygmi-get-0.6.0/setup.py` & `pygmi-get-0.7.4/setup.py`

 * *Files identical despite different names*

