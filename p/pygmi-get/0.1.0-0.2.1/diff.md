# Comparing `tmp/pygmi-get-0.1.0.tar.gz` & `tmp/pygmi-get-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmi-get-0.1.0.tar", last modified: Sun Apr 30 07:06:16 2023, max compression
+gzip compressed data, was "pygmi-get-0.2.1.tar", last modified: Sun Apr 30 07:13:23 2023, max compression
```

## Comparing `pygmi-get-0.1.0.tar` & `pygmi-get-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:06:15.999088 pygmi-get-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-30 07:06:15.999088 pygmi-get-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-30 07:05:59.000000 pygmi-get-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-30 07:05:59.000000 pygmi-get-0.1.0/pygmi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:06:15.999088 pygmi-get-0.1.0/pygmi_get.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-30 07:06:15.000000 pygmi-get-0.1.0/pygmi_get.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-30 07:06:15.000000 pygmi-get-0.1.0/pygmi_get.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 07:06:15.000000 pygmi-get-0.1.0/pygmi_get.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 07:06:15.000000 pygmi-get-0.1.0/pygmi_get.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 07:06:15.000000 pygmi-get-0.1.0/pygmi_get.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-30 07:05:59.000000 pygmi-get-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 07:06:15.999088 pygmi-get-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-30 07:05:59.000000 pygmi-get-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:13:23.034515 pygmi-get-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-30 07:13:23.034515 pygmi-get-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-30 07:13:02.000000 pygmi-get-0.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-30 07:13:02.000000 pygmi-get-0.2.1/pygmi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:13:23.034515 pygmi-get-0.2.1/pygmi_get.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-30 07:13:22.000000 pygmi-get-0.2.1/pygmi_get.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-30 07:13:23.000000 pygmi-get-0.2.1/pygmi_get.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 07:13:22.000000 pygmi-get-0.2.1/pygmi_get.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 07:13:22.000000 pygmi-get-0.2.1/pygmi_get.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 07:13:22.000000 pygmi-get-0.2.1/pygmi_get.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-30 07:13:02.000000 pygmi-get-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 07:13:23.034515 pygmi-get-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-30 07:13:02.000000 pygmi-get-0.2.1/setup.py
```

### Comparing `pygmi-get-0.1.0/PKG-INFO` & `pygmi-get-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmi-get
-Version: 0.1.0
+Version: 0.2.1
 Summary: A simple package installer for Python that eliminates the need for venvs.
 Home-page: https://github.com/AquaQuokka/pygmi
 Author: AquaQuokka
 License: BSD-3-Clause
 
 =============
 Pygmi
```

### Comparing `pygmi-get-0.1.0/pygmi.py` & `pygmi-get-0.2.1/pygmi.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     if package and file:
 
         with urlopen(f"https://raw.githubusercontent.com/AquaQuokka/pygmi-pkgs/main/packages/{package}/{file}.py") as u:
             pkgu = u.read()
 
         if pkgu != "404: Not Found":
         
-            if not os.path.exists(f"{package}"):
-                os.mkdir(f"{package}")
+            if not os.path.exists(f"pygmi"):
+                os.mkdir(f"pygmi")
 
-            with open(os.path.join(f"{package}", f"{file}.py"), 'w') as f:
+            with open(os.path.join(f"pygmi", f"{file}.py"), 'w') as f:
                 f.write(pkgu)
 
             click.echo(f"\033[33;1mPackage {package} installed successfully.\033[0m")
     
         else:
             click.echo(f"\033[0;31mPackage {package} not found!\033[0m")
```

### Comparing `pygmi-get-0.1.0/pygmi_get.egg-info/PKG-INFO` & `pygmi-get-0.2.1/pygmi_get.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmi-get
-Version: 0.1.0
+Version: 0.2.1
 Summary: A simple package installer for Python that eliminates the need for venvs.
 Home-page: https://github.com/AquaQuokka/pygmi
 Author: AquaQuokka
 License: BSD-3-Clause
 
 =============
 Pygmi
```

