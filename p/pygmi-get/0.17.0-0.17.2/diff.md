# Comparing `tmp/pygmi-get-0.17.0.tar.gz` & `tmp/pygmi-get-0.17.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmi-get-0.17.0.tar", last modified: Sun Apr 30 11:33:02 2023, max compression
+gzip compressed data, was "pygmi-get-0.17.2.tar", last modified: Sun Apr 30 11:44:34 2023, max compression
```

## Comparing `pygmi-get-0.17.0.tar` & `pygmi-get-0.17.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:33:02.373515 pygmi-get-0.17.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-30 11:33:02.373515 pygmi-get-0.17.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-30 11:32:51.000000 pygmi-get-0.17.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:33:02.373515 pygmi-get-0.17.0/pygmi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 11:32:51.000000 pygmi-get-0.17.0/pygmi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-30 11:32:51.000000 pygmi-get-0.17.0/pygmi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-30 11:32:51.000000 pygmi-get-0.17.0/pygmi/pygmi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:33:02.373515 pygmi-get-0.17.0/pygmi_get.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-30 11:33:02.000000 pygmi-get-0.17.0/pygmi_get.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-30 11:33:02.000000 pygmi-get-0.17.0/pygmi_get.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 11:33:02.000000 pygmi-get-0.17.0/pygmi_get.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-30 11:33:02.000000 pygmi-get-0.17.0/pygmi_get.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 11:33:02.000000 pygmi-get-0.17.0/pygmi_get.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 11:33:02.000000 pygmi-get-0.17.0/pygmi_get.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-30 11:32:51.000000 pygmi-get-0.17.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 11:33:02.373515 pygmi-get-0.17.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-30 11:32:51.000000 pygmi-get-0.17.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:44:34.774015 pygmi-get-0.17.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-30 11:44:34.774015 pygmi-get-0.17.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-30 11:44:24.000000 pygmi-get-0.17.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:44:34.774015 pygmi-get-0.17.2/pygmi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 11:44:24.000000 pygmi-get-0.17.2/pygmi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-30 11:44:24.000000 pygmi-get-0.17.2/pygmi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-30 11:44:24.000000 pygmi-get-0.17.2/pygmi/pygmi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:44:34.774015 pygmi-get-0.17.2/pygmi_get.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-30 11:44:34.000000 pygmi-get-0.17.2/pygmi_get.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-30 11:44:34.000000 pygmi-get-0.17.2/pygmi_get.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 11:44:34.000000 pygmi-get-0.17.2/pygmi_get.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-30 11:44:34.000000 pygmi-get-0.17.2/pygmi_get.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 11:44:34.000000 pygmi-get-0.17.2/pygmi_get.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 11:44:34.000000 pygmi-get-0.17.2/pygmi_get.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-30 11:44:24.000000 pygmi-get-0.17.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 11:44:34.774015 pygmi-get-0.17.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-30 11:44:24.000000 pygmi-get-0.17.2/setup.py
```

### Comparing `pygmi-get-0.17.0/PKG-INFO` & `pygmi-get-0.17.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmi-get
-Version: 0.17.0
+Version: 0.17.2
 Summary: A simple package installer for Python that eliminates the need for venvs.
 Home-page: https://github.com/AquaQuokka/pygmi
 Author: AquaQuokka
 License: BSD-3-Clause
 
 Pygmi
 =====
```

### Comparing `pygmi-get-0.17.0/README.md` & `pygmi-get-0.17.2/README.md`

 * *Files identical despite different names*

### Comparing `pygmi-get-0.17.0/pygmi/pygmi.py` & `pygmi-get-0.17.2/pygmi/pygmi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 #!/usr/bin/env python
 # -*- mode: python ; coding: utf-8 -*-
 
 import click
 import os
 from urllib.request import urlopen
 
-__version__ = "0.17.0"
+__version__ = "0.17.2"
 
 @click.group()
 def cli():
     pass
 
 @click.command(name='install')
 @click.argument('package')
 def install(package):
         
     if package:
 
         with urlopen(f"https://raw.githubusercontent.com/AquaQuokka/pygmi-pkgs/main/packages/{package}/{package}.py") as u:
-            pkgu = str(u.read())
+            pkgu = str(u.read())[1:]
 
         if pkgu != "404: Not Found":
         
             if not os.path.exists(f"pygmi"):
                 os.mkdir(f"pygmi")
 
             if not os.path.exists(os.path.join(f"pygmi", f"{package}.py")):
                 with open(os.path.join(f"pygmi", f"{package}.py"), 'w') as f:
-                    f.write(str(pkgu))
+                    f.write(pkgu)
                     click.echo(f"\033[33;1mPackage {package} installed successfully.\033[0m")
 
             else:
                 click.echo(f"\033[33;1m{package}.py already exists, are you sure you want to update it?\033[0m")
                 cfm = input(f"Update {package}.py? (Y/n): ")
                 
                 if cfm.strip().lower() in ["y", "yes"]:
                     with open(os.path.join(f"pygmi", f"{package}.py"), 'w') as f:
                         f.write('')
-                        f.write(str(pkgu))
+                        f.write(pkgu)
                         click.echo(f"\033[33;1mPackage {package} updated successfully.\033[0m")
                 
                 else:
                     click.echo(f"\033[31mSkipped package.\033[0m")
 
-
-    
         else:
             click.echo(f"\033[0;31mPackage {package} not found!\033[0m")
     
     else:
         click.echo(f"\033[0;31mFatal: Expected 1 argument: package\033[0m")
 
 cli.add_command(install)
```

### Comparing `pygmi-get-0.17.0/pygmi_get.egg-info/PKG-INFO` & `pygmi-get-0.17.2/pygmi_get.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmi-get
-Version: 0.17.0
+Version: 0.17.2
 Summary: A simple package installer for Python that eliminates the need for venvs.
 Home-page: https://github.com/AquaQuokka/pygmi
 Author: AquaQuokka
 License: BSD-3-Clause
 
 Pygmi
 =====
```

### Comparing `pygmi-get-0.17.0/setup.py` & `pygmi-get-0.17.2/setup.py`

 * *Files identical despite different names*

