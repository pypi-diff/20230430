# Comparing `tmp/pygmi-get-0.17.3.tar.gz` & `tmp/pygmi-get-0.17.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmi-get-0.17.3.tar", last modified: Sun Apr 30 11:54:40 2023, max compression
+gzip compressed data, was "pygmi-get-0.17.4.tar", last modified: Sun Apr 30 11:58:14 2023, max compression
```

## Comparing `pygmi-get-0.17.3.tar` & `pygmi-get-0.17.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:54:40.681260 pygmi-get-0.17.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-30 11:54:40.681260 pygmi-get-0.17.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-30 11:54:26.000000 pygmi-get-0.17.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:54:40.677260 pygmi-get-0.17.3/pygmi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 11:54:26.000000 pygmi-get-0.17.3/pygmi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-30 11:54:26.000000 pygmi-get-0.17.3/pygmi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-30 11:54:26.000000 pygmi-get-0.17.3/pygmi/pygmi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:54:40.681260 pygmi-get-0.17.3/pygmi_get.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-30 11:54:40.000000 pygmi-get-0.17.3/pygmi_get.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-30 11:54:40.000000 pygmi-get-0.17.3/pygmi_get.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 11:54:40.000000 pygmi-get-0.17.3/pygmi_get.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-30 11:54:40.000000 pygmi-get-0.17.3/pygmi_get.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 11:54:40.000000 pygmi-get-0.17.3/pygmi_get.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 11:54:40.000000 pygmi-get-0.17.3/pygmi_get.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-30 11:54:26.000000 pygmi-get-0.17.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 11:54:40.681260 pygmi-get-0.17.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-30 11:54:26.000000 pygmi-get-0.17.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:58:14.988236 pygmi-get-0.17.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-30 11:58:14.984236 pygmi-get-0.17.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-30 11:58:04.000000 pygmi-get-0.17.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:58:14.984236 pygmi-get-0.17.4/pygmi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 11:58:04.000000 pygmi-get-0.17.4/pygmi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-30 11:58:04.000000 pygmi-get-0.17.4/pygmi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-30 11:58:04.000000 pygmi-get-0.17.4/pygmi/pygmi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:58:14.984236 pygmi-get-0.17.4/pygmi_get.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-30 11:58:14.000000 pygmi-get-0.17.4/pygmi_get.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-30 11:58:14.000000 pygmi-get-0.17.4/pygmi_get.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 11:58:14.000000 pygmi-get-0.17.4/pygmi_get.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-30 11:58:14.000000 pygmi-get-0.17.4/pygmi_get.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 11:58:14.000000 pygmi-get-0.17.4/pygmi_get.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 11:58:14.000000 pygmi-get-0.17.4/pygmi_get.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-30 11:58:04.000000 pygmi-get-0.17.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 11:58:14.988236 pygmi-get-0.17.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-30 11:58:04.000000 pygmi-get-0.17.4/setup.py
```

### Comparing `pygmi-get-0.17.3/PKG-INFO` & `pygmi-get-0.17.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmi-get
-Version: 0.17.3
+Version: 0.17.4
 Summary: A simple package installer for Python that eliminates the need for venvs.
 Home-page: https://github.com/AquaQuokka/pygmi
 Author: AquaQuokka
 License: BSD-3-Clause
 
 Pygmi
 =====
```

### Comparing `pygmi-get-0.17.3/README.md` & `pygmi-get-0.17.4/README.md`

 * *Files identical despite different names*

### Comparing `pygmi-get-0.17.3/pygmi/pygmi.py` & `pygmi-get-0.17.4/pygmi/pygmi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- mode: python ; coding: utf-8 -*-
 
 import click
 import os
 from urllib.request import urlopen
 
-__version__ = "0.17.3"
+__version__ = "0.17.4"
 
 @click.group()
 def cli():
     pass
 
 @click.command(name='install')
 @click.argument('package')
@@ -17,15 +17,17 @@
         
     if package:
 
         with urlopen(f"https://raw.githubusercontent.com/AquaQuokka/pygmi-pkgs/main/packages/{package}/{package}.py") as u:
             pkgu = str(u.read())[1:]
             pkgu = str(pkgu[1:])
             pkgu = str(pkgu[:-1])
-            pkgu = pkgu.replace('\\n', '\n')
+            pkgu = str(pkgu.replace('\\n', '\n'))
+            pkgu = str(pkgu.replace('\\"', '\"'))
+            pkgu = str(pkgu.replace("\\'", "\'"))
 
         if pkgu != "404: Not Found":
         
             if not os.path.exists(f"pygmipkgs"):
                 os.mkdir(f"pygmipkgs")
 
             if not os.path.exists(os.path.join(f"pygmipkgs", f"{package}.py")):
```

### Comparing `pygmi-get-0.17.3/pygmi_get.egg-info/PKG-INFO` & `pygmi-get-0.17.4/pygmi_get.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmi-get
-Version: 0.17.3
+Version: 0.17.4
 Summary: A simple package installer for Python that eliminates the need for venvs.
 Home-page: https://github.com/AquaQuokka/pygmi
 Author: AquaQuokka
 License: BSD-3-Clause
 
 Pygmi
 =====
```

### Comparing `pygmi-get-0.17.3/setup.py` & `pygmi-get-0.17.4/setup.py`

 * *Files identical despite different names*

