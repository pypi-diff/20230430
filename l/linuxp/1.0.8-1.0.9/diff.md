# Comparing `tmp/linuxp-1.0.8.tar.gz` & `tmp/linuxp-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linuxp-1.0.8.tar", last modified: Tue Oct 18 00:29:48 2022, max compression
+gzip compressed data, was "linuxp-1.0.9.tar", last modified: Sun Dec 18 06:58:40 2022, max compression
```

## Comparing `linuxp-1.0.8.tar` & `linuxp-1.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 fernandocelmer  (1000) fernandocelmer  (1000)        0 2022-10-18 00:29:48.786371 linuxp-1.0.8/
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     1070 2022-10-11 00:09:57.000000 linuxp-1.0.8/LICENSE
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     5505 2022-10-18 00:29:48.782371 linuxp-1.0.8/PKG-INFO
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     4732 2022-10-17 01:10:47.000000 linuxp-1.0.8/README.md
-drwxrwxr-x   0 fernandocelmer  (1000) fernandocelmer  (1000)        0 2022-10-18 00:29:48.778371 linuxp-1.0.8/linux_profile/
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)       21 2022-10-18 00:28:11.000000 linuxp-1.0.8/linux_profile/__init__.py
-drwxrwxr-x   0 fernandocelmer  (1000) fernandocelmer  (1000)        0 2022-10-18 00:29:48.782371 linuxp-1.0.8/linux_profile/base/
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     4242 2022-10-16 17:40:01.000000 linuxp-1.0.8/linux_profile/base/command.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     2933 2022-10-18 00:27:35.000000 linuxp-1.0.8/linux_profile/base/config.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     1559 2022-10-15 22:02:25.000000 linuxp-1.0.8/linux_profile/base/error.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     1291 2022-10-17 01:10:59.000000 linuxp-1.0.8/linux_profile/base/log.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     5424 2022-10-16 19:00:47.000000 linuxp-1.0.8/linux_profile/base/storage.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)      308 2022-10-13 00:56:21.000000 linuxp-1.0.8/linux_profile/base/system.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     3816 2022-10-15 22:02:25.000000 linuxp-1.0.8/linux_profile/base/validator.py
-drwxrwxr-x   0 fernandocelmer  (1000) fernandocelmer  (1000)        0 2022-10-18 00:29:48.782371 linuxp-1.0.8/linux_profile/commands/
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)        0 2022-10-13 00:56:21.000000 linuxp-1.0.8/linux_profile/commands/__init__.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     3469 2022-10-15 22:02:25.000000 linuxp-1.0.8/linux_profile/commands/add.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)      490 2022-10-16 17:21:44.000000 linuxp-1.0.8/linux_profile/commands/config.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     1564 2022-10-13 04:05:50.000000 linuxp-1.0.8/linux_profile/commands/install.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     1963 2022-10-16 17:23:31.000000 linuxp-1.0.8/linux_profile/commands/list.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)      927 2022-10-13 04:05:50.000000 linuxp-1.0.8/linux_profile/commands/uninstall.py
-drwxrwxr-x   0 fernandocelmer  (1000) fernandocelmer  (1000)        0 2022-10-18 00:29:48.782371 linuxp-1.0.8/linux_profile/handlers/
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)        0 2022-10-13 00:56:21.000000 linuxp-1.0.8/linux_profile/handlers/__init__.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)      977 2022-10-15 02:10:00.000000 linuxp-1.0.8/linux_profile/handlers/alias.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     2609 2022-10-18 00:27:35.000000 linuxp-1.0.8/linux_profile/handlers/package.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     1154 2022-10-18 00:27:35.000000 linuxp-1.0.8/linux_profile/handlers/script.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     1823 2022-10-17 01:10:59.000000 linuxp-1.0.8/linux_profile/main.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)      553 2022-10-18 00:27:35.000000 linuxp-1.0.8/linux_profile/settings.py
-drwxrwxr-x   0 fernandocelmer  (1000) fernandocelmer  (1000)        0 2022-10-18 00:29:48.782371 linuxp-1.0.8/linux_profile/utils/
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)        0 2022-10-13 00:56:21.000000 linuxp-1.0.8/linux_profile/utils/__init__.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     2526 2022-10-17 01:10:47.000000 linuxp-1.0.8/linux_profile/utils/file.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     1849 2022-10-15 22:02:25.000000 linuxp-1.0.8/linux_profile/utils/text.py
-drwxrwxr-x   0 fernandocelmer  (1000) fernandocelmer  (1000)        0 2022-10-18 00:29:48.782371 linuxp-1.0.8/linuxp.egg-info/
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     5505 2022-10-18 00:29:48.000000 linuxp-1.0.8/linuxp.egg-info/PKG-INFO
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)      903 2022-10-18 00:29:48.000000 linuxp-1.0.8/linuxp.egg-info/SOURCES.txt
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)        1 2022-10-18 00:29:48.000000 linuxp-1.0.8/linuxp.egg-info/dependency_links.txt
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)       51 2022-10-18 00:29:48.000000 linuxp-1.0.8/linuxp.egg-info/entry_points.txt
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)       14 2022-10-18 00:29:48.000000 linuxp-1.0.8/linuxp.egg-info/top_level.txt
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)        1 2022-10-17 02:45:12.000000 linuxp-1.0.8/linuxp.egg-info/zip-safe
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)       38 2022-10-18 00:29:48.786371 linuxp-1.0.8/setup.cfg
--rwxrwxr-x   0 fernandocelmer  (1000) fernandocelmer  (1000)     1407 2022-10-13 00:56:21.000000 linuxp-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 06:58:40.817531 linuxp-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-18 06:58:30.000000 linuxp-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2022-12-18 06:58:40.817531 linuxp-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2022-12-18 06:58:30.000000 linuxp-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 06:58:40.813531 linuxp-1.0.9/linux_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 06:58:40.813531 linuxp-1.0.9/linux_profile/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/base/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/base/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/base/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/base/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/base/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/base/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 06:58:40.813531 linuxp-1.0.9/linux_profile/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/commands/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/commands/uninstall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 06:58:40.813531 linuxp-1.0.9/linux_profile/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/handlers/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/handlers/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/handlers/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 06:58:40.817531 linuxp-1.0.9/linux_profile/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2022-12-18 06:58:30.000000 linuxp-1.0.9/linux_profile/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 06:58:40.817531 linuxp-1.0.9/linuxp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2022-12-18 06:58:40.000000 linuxp-1.0.9/linuxp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2022-12-18 06:58:40.000000 linuxp-1.0.9/linuxp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-18 06:58:40.000000 linuxp-1.0.9/linuxp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-18 06:58:40.000000 linuxp-1.0.9/linuxp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-18 06:58:40.000000 linuxp-1.0.9/linuxp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-18 06:58:40.000000 linuxp-1.0.9/linuxp.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-18 06:58:40.817531 linuxp-1.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1407 2022-12-18 06:58:30.000000 linuxp-1.0.9/setup.py
```

### Comparing `linuxp-1.0.8/LICENSE` & `linuxp-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `linuxp-1.0.8/PKG-INFO` & `linuxp-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxp
-Version: 1.0.8
+Version: 1.0.9
 Summary: Linux profile management tool
 Home-page: https://github.com/MyLinuxProfile/linux-profile
 Author: Fernando Celmer
 Author-email: email@fernandocelmer.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
@@ -23,16 +23,18 @@
 
 <img src="https://github.com/MyLinuxProfile/linux-profile/blob/master/docs/linuxp.png?raw=true">
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/MyLinuxProfile?label=LinuxProfile&style=flat-square)
 ![GitHub last commit](https://img.shields.io/github/last-commit/MyLinuxProfile/linux-profile-basic?style=flat-square)
 ![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/MyLinuxProfile/linux-profile?style=flat-square)
 ![PyPI](https://img.shields.io/pypi/v/linuxp)
+<br>
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/linuxp?style=flat-square)
 ![PyPI - Status](https://img.shields.io/pypi/status/linuxp?style=flat-square)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/linuxp?style=flat-square)
 
 # [Introduction](https://github.com/MyLinuxProfile/linux-profile/wiki)
 Linux Profile is a Linux profile management tool. With this project it is possible, from commands executed in the console, to create a 'json' file to store backup configurations. such as information about installed packages, alias, terminal settings. It also allows with a single command to restore saved configurations.
 
 ## [Installation](https://github.com/MyLinuxProfile/linux-profile/wiki/Installation)
 
 - **Install - Pypi/PIP**
```

### Comparing `linuxp-1.0.8/README.md` & `linuxp-1.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 
 <img src="https://github.com/MyLinuxProfile/linux-profile/blob/master/docs/linuxp.png?raw=true">
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/MyLinuxProfile?label=LinuxProfile&style=flat-square)
 ![GitHub last commit](https://img.shields.io/github/last-commit/MyLinuxProfile/linux-profile-basic?style=flat-square)
 ![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/MyLinuxProfile/linux-profile?style=flat-square)
 ![PyPI](https://img.shields.io/pypi/v/linuxp)
+<br>
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/linuxp?style=flat-square)
 ![PyPI - Status](https://img.shields.io/pypi/status/linuxp?style=flat-square)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/linuxp?style=flat-square)
 
 # [Introduction](https://github.com/MyLinuxProfile/linux-profile/wiki)
 Linux Profile is a Linux profile management tool. With this project it is possible, from commands executed in the console, to create a 'json' file to store backup configurations. such as information about installed packages, alias, terminal settings. It also allows with a single command to restore saved configurations.
 
 ## [Installation](https://github.com/MyLinuxProfile/linux-profile/wiki/Installation)
 
 - **Install - Pypi/PIP**
```

### Comparing `linuxp-1.0.8/linux_profile/base/command.py` & `linuxp-1.0.9/linux_profile/base/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from linux_profile import __version__
+from linux_profile import (
+    __version__,
+    __info__
+)
 from linux_profile.base.error import (
     ErrorInvalidValue,
     ErrorParameterIsMissing,
     ErrorLoadSettings,
     ErrorOptionIsMissing,
     ErrorOptionIsInvalid,
     print_warning,
@@ -94,14 +97,16 @@
         self.cmd_list.add_argument('-i', '--item')
 
     def run(self):
         try:
             arguments = self.parser.parse_args()
             if  hasattr(arguments, 'exec'):
                 arguments.exec(parser=self.parser, arguments=arguments)
+            else:
+                print(__info__)
 
         except ErrorParameterIsMissing as error:
             print_warning(str(error))
 
         except ErrorOptionIsMissing as error:
             print_warning(str(error))
```

### Comparing `linuxp-1.0.8/linux_profile/base/config.py` & `linuxp-1.0.9/linux_profile/base/config.py`

 * *Files identical despite different names*

### Comparing `linuxp-1.0.8/linux_profile/base/error.py` & `linuxp-1.0.9/linux_profile/base/error.py`

 * *Files identical despite different names*

### Comparing `linuxp-1.0.8/linux_profile/base/log.py` & `linuxp-1.0.9/linux_profile/base/log.py`

 * *Files identical despite different names*

### Comparing `linuxp-1.0.8/linux_profile/base/storage.py` & `linuxp-1.0.9/linux_profile/base/storage.py`

 * *Files identical despite different names*

### Comparing `linuxp-1.0.8/linux_profile/base/validator.py` & `linuxp-1.0.9/linux_profile/base/validator.py`

 * *Files identical despite different names*

### Comparing `linuxp-1.0.8/linux_profile/commands/add.py` & `linuxp-1.0.9/linux_profile/commands/add.py`

 * *Files identical despite different names*

### Comparing `linuxp-1.0.8/linux_profile/commands/install.py` & `linuxp-1.0.9/linux_profile/commands/install.py`

 * *Files identical despite different names*

### Comparing `linuxp-1.0.8/linux_profile/commands/list.py` & `linuxp-1.0.9/linux_profile/commands/list.py`

 * *Files identical despite different names*

### Comparing `linuxp-1.0.8/linux_profile/commands/uninstall.py` & `linuxp-1.0.9/linux_profile/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `linuxp-1.0.8/linux_profile/handlers/alias.py` & `linuxp-1.0.9/linux_profile/handlers/alias.py`

 * *Files identical despite different names*

### Comparing `linuxp-1.0.8/linux_profile/handlers/package.py` & `linuxp-1.0.9/linux_profile/handlers/package.py`

 * *Files identical despite different names*

### Comparing `linuxp-1.0.8/linux_profile/handlers/script.py` & `linuxp-1.0.9/linux_profile/handlers/script.py`

 * *Files identical despite different names*

### Comparing `linuxp-1.0.8/linux_profile/main.py` & `linuxp-1.0.9/linux_profile/main.py`

 * *Files identical despite different names*

### Comparing `linuxp-1.0.8/linux_profile/settings.py` & `linuxp-1.0.9/linux_profile/settings.py`

 * *Files identical despite different names*

### Comparing `linuxp-1.0.8/linux_profile/utils/file.py` & `linuxp-1.0.9/linux_profile/utils/file.py`

 * *Files identical despite different names*

### Comparing `linuxp-1.0.8/linux_profile/utils/text.py` & `linuxp-1.0.9/linux_profile/utils/text.py`

 * *Files identical despite different names*

### Comparing `linuxp-1.0.8/linuxp.egg-info/PKG-INFO` & `linuxp-1.0.9/linuxp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxp
-Version: 1.0.8
+Version: 1.0.9
 Summary: Linux profile management tool
 Home-page: https://github.com/MyLinuxProfile/linux-profile
 Author: Fernando Celmer
 Author-email: email@fernandocelmer.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
@@ -23,16 +23,18 @@
 
 <img src="https://github.com/MyLinuxProfile/linux-profile/blob/master/docs/linuxp.png?raw=true">
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/MyLinuxProfile?label=LinuxProfile&style=flat-square)
 ![GitHub last commit](https://img.shields.io/github/last-commit/MyLinuxProfile/linux-profile-basic?style=flat-square)
 ![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/MyLinuxProfile/linux-profile?style=flat-square)
 ![PyPI](https://img.shields.io/pypi/v/linuxp)
+<br>
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/linuxp?style=flat-square)
 ![PyPI - Status](https://img.shields.io/pypi/status/linuxp?style=flat-square)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/linuxp?style=flat-square)
 
 # [Introduction](https://github.com/MyLinuxProfile/linux-profile/wiki)
 Linux Profile is a Linux profile management tool. With this project it is possible, from commands executed in the console, to create a 'json' file to store backup configurations. such as information about installed packages, alias, terminal settings. It also allows with a single command to restore saved configurations.
 
 ## [Installation](https://github.com/MyLinuxProfile/linux-profile/wiki/Installation)
 
 - **Install - Pypi/PIP**
```

### Comparing `linuxp-1.0.8/linuxp.egg-info/SOURCES.txt` & `linuxp-1.0.9/linuxp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linuxp-1.0.8/setup.py` & `linuxp-1.0.9/setup.py`

 * *Files identical despite different names*

