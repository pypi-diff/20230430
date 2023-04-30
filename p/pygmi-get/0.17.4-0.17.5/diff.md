# Comparing `tmp/pygmi-get-0.17.4.tar.gz` & `tmp/pygmi-get-0.17.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmi-get-0.17.4.tar", last modified: Sun Apr 30 11:58:14 2023, max compression
+gzip compressed data, was "pygmi-get-0.17.5.tar", last modified: Sun Apr 30 12:10:21 2023, max compression
```

## Comparing `pygmi-get-0.17.4.tar` & `pygmi-get-0.17.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:58:14.988236 pygmi-get-0.17.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-30 11:58:14.984236 pygmi-get-0.17.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-30 11:58:04.000000 pygmi-get-0.17.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:58:14.984236 pygmi-get-0.17.4/pygmi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 11:58:04.000000 pygmi-get-0.17.4/pygmi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-30 11:58:04.000000 pygmi-get-0.17.4/pygmi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-30 11:58:04.000000 pygmi-get-0.17.4/pygmi/pygmi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:58:14.984236 pygmi-get-0.17.4/pygmi_get.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-30 11:58:14.000000 pygmi-get-0.17.4/pygmi_get.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-30 11:58:14.000000 pygmi-get-0.17.4/pygmi_get.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 11:58:14.000000 pygmi-get-0.17.4/pygmi_get.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-30 11:58:14.000000 pygmi-get-0.17.4/pygmi_get.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 11:58:14.000000 pygmi-get-0.17.4/pygmi_get.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 11:58:14.000000 pygmi-get-0.17.4/pygmi_get.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-30 11:58:04.000000 pygmi-get-0.17.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 11:58:14.988236 pygmi-get-0.17.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-30 11:58:04.000000 pygmi-get-0.17.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:10:21.956001 pygmi-get-0.17.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-30 12:10:21.956001 pygmi-get-0.17.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-30 12:10:12.000000 pygmi-get-0.17.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:10:21.952001 pygmi-get-0.17.5/pygmi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 12:10:12.000000 pygmi-get-0.17.5/pygmi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-30 12:10:12.000000 pygmi-get-0.17.5/pygmi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-30 12:10:12.000000 pygmi-get-0.17.5/pygmi/pygmi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:10:21.956001 pygmi-get-0.17.5/pygmi_get.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-30 12:10:21.000000 pygmi-get-0.17.5/pygmi_get.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-30 12:10:21.000000 pygmi-get-0.17.5/pygmi_get.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:10:21.000000 pygmi-get-0.17.5/pygmi_get.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-30 12:10:21.000000 pygmi-get-0.17.5/pygmi_get.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 12:10:21.000000 pygmi-get-0.17.5/pygmi_get.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 12:10:21.000000 pygmi-get-0.17.5/pygmi_get.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-30 12:10:12.000000 pygmi-get-0.17.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 12:10:21.956001 pygmi-get-0.17.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-30 12:10:12.000000 pygmi-get-0.17.5/setup.py
```

### Comparing `pygmi-get-0.17.4/PKG-INFO` & `pygmi-get-0.17.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmi-get
-Version: 0.17.4
+Version: 0.17.5
 Summary: A simple package installer for Python that eliminates the need for venvs.
 Home-page: https://github.com/AquaQuokka/pygmi
 Author: AquaQuokka
 License: BSD-3-Clause
 
 Pygmi
 =====
@@ -94,7 +94,28 @@
    py setup.py sdist bdist_wheel
 
 2. Then, install it using the following command:
 
 .. code:: bash
 
    pip install dist/SOME_NAME_HERE.whl
+
+
+Nothing in the module?
+~~~~~~~~~~~~~~~~~~~~~~
+
+Did you remove the leading and trailing string determiners?
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+E.g.
+
+1. Before:
+
+.. code:: python
+
+   b"Text here"
+
+2. After:
+
+.. code:: python
+
+   Text here
```

### Comparing `pygmi-get-0.17.4/README.md` & `pygmi-get-0.17.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Pygmi
 
 Welcome to Pygmi, a package manager that is completely file-based and local, so no need to worry about virtual environments and the like.
 
-
 ## Installation
 
 ### Using PIP
 
 Using PIP is a great way to install Pygmi if you are a beginner and don't want to have to manage Pygmi yourself.
 However, PIP installations are hard to troubleshoot if you run into issues.
 
@@ -75,7 +74,25 @@
 ```
 
 2. Then, install it using the following command:
 
 ```bash
 pip install dist/SOME_NAME_HERE.whl
 ```
+
+### Nothing in the module?
+
+#### Did you remove the leading and trailing string determiners?
+
+
+1. Before:
+
+```py
+b"Text here"
+```
+
+
+2. After:
+
+```py
+b"Text here"
+```
```

### Comparing `pygmi-get-0.17.4/pygmi/pygmi.py` & `pygmi-get-0.17.5/pygmi/pygmi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 #!/usr/bin/env python
 # -*- mode: python ; coding: utf-8 -*-
 
 import click
 import os
 from urllib.request import urlopen
 
-__version__ = "0.17.4"
+__version__ = "0.17.5"
 
 @click.group()
 def cli():
     pass
 
 @click.command(name='install')
 @click.argument('package')
 def install(package):
         
     if package:
 
         with urlopen(f"https://raw.githubusercontent.com/AquaQuokka/pygmi-pkgs/main/packages/{package}/{package}.py") as u:
+            pkgu = str(u.read())
+            
+            """
+            # This was gonna help, but it doesn't work with escapes
             pkgu = str(u.read())[1:]
             pkgu = str(pkgu[1:])
             pkgu = str(pkgu[:-1])
             pkgu = str(pkgu.replace('\\n', '\n'))
             pkgu = str(pkgu.replace('\\"', '\"'))
             pkgu = str(pkgu.replace("\\'", "\'"))
+            """
 
         if pkgu != "404: Not Found":
         
             if not os.path.exists(f"pygmipkgs"):
                 os.mkdir(f"pygmipkgs")
 
             if not os.path.exists(os.path.join(f"pygmipkgs", f"{package}.py")):
```

### Comparing `pygmi-get-0.17.4/pygmi_get.egg-info/PKG-INFO` & `pygmi-get-0.17.5/pygmi_get.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmi-get
-Version: 0.17.4
+Version: 0.17.5
 Summary: A simple package installer for Python that eliminates the need for venvs.
 Home-page: https://github.com/AquaQuokka/pygmi
 Author: AquaQuokka
 License: BSD-3-Clause
 
 Pygmi
 =====
@@ -94,7 +94,28 @@
    py setup.py sdist bdist_wheel
 
 2. Then, install it using the following command:
 
 .. code:: bash
 
    pip install dist/SOME_NAME_HERE.whl
+
+
+Nothing in the module?
+~~~~~~~~~~~~~~~~~~~~~~
+
+Did you remove the leading and trailing string determiners?
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+E.g.
+
+1. Before:
+
+.. code:: python
+
+   b"Text here"
+
+2. After:
+
+.. code:: python
+
+   Text here
```

### Comparing `pygmi-get-0.17.4/setup.py` & `pygmi-get-0.17.5/setup.py`

 * *Files identical despite different names*

