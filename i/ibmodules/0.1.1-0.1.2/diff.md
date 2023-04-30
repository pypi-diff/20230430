# Comparing `tmp/ibmodules-0.1.1.tar.gz` & `tmp/ibmodules-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibmodules-0.1.1.tar", last modified: Sat Apr 29 17:08:32 2023, max compression
+gzip compressed data, was "ibmodules-0.1.2.tar", last modified: Sun Apr 30 07:03:18 2023, max compression
```

## Comparing `ibmodules-0.1.1.tar` & `ibmodules-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vik        (501) staff       (20)        0 2023-04-29 17:08:32.141206 ibmodules-0.1.1/
--rw-r--r--   0 vik        (501) staff       (20)     1079 2023-04-29 15:50:16.000000 ibmodules-0.1.1/LICENSE
--rw-r--r--   0 vik        (501) staff       (20)       85 2023-04-29 15:50:16.000000 ibmodules-0.1.1/MANIFEST.in
--rw-r--r--   0 vik        (501) staff       (20)     1228 2023-04-29 17:08:32.141272 ibmodules-0.1.1/PKG-INFO
--rw-r--r--   0 vik        (501) staff       (20)      126 2023-04-29 15:57:31.000000 ibmodules-0.1.1/README.md
--rw-r--r--   0 vik        (501) staff       (20)       98 2023-04-29 15:50:16.000000 ibmodules-0.1.1/pyproject.toml
--rw-r--r--   0 vik        (501) staff       (20)      112 2023-04-29 17:08:32.141461 ibmodules-0.1.1/setup.cfg
--rw-r--r--   0 vik        (501) staff       (20)     1829 2023-04-29 16:13:11.000000 ibmodules-0.1.1/setup.py
-drwxr-xr-x   0 vik        (501) staff       (20)        0 2023-04-29 17:08:32.139623 ibmodules-0.1.1/src/
-drwxr-xr-x   0 vik        (501) staff       (20)        0 2023-04-29 17:08:32.140527 ibmodules-0.1.1/src/ibmodules/
--rw-r--r--   0 vik        (501) staff       (20)       41 2023-04-29 17:08:28.000000 ibmodules-0.1.1/src/ibmodules/__init__.py
--rw-r--r--   0 vik        (501) staff       (20)      588 2023-04-29 17:07:57.000000 ibmodules-0.1.1/src/ibmodules/op.py
-drwxr-xr-x   0 vik        (501) staff       (20)        0 2023-04-29 17:08:32.141089 ibmodules-0.1.1/src/ibmodules.egg-info/
--rw-r--r--   0 vik        (501) staff       (20)     1228 2023-04-29 17:08:32.000000 ibmodules-0.1.1/src/ibmodules.egg-info/PKG-INFO
--rw-r--r--   0 vik        (501) staff       (20)      293 2023-04-29 17:08:32.000000 ibmodules-0.1.1/src/ibmodules.egg-info/SOURCES.txt
--rw-r--r--   0 vik        (501) staff       (20)        1 2023-04-29 17:08:32.000000 ibmodules-0.1.1/src/ibmodules.egg-info/dependency_links.txt
--rw-r--r--   0 vik        (501) staff       (20)       22 2023-04-29 17:08:32.000000 ibmodules-0.1.1/src/ibmodules.egg-info/requires.txt
--rw-r--r--   0 vik        (501) staff       (20)       10 2023-04-29 17:08:32.000000 ibmodules-0.1.1/src/ibmodules.egg-info/top_level.txt
+drwxr-xr-x   0 vik        (501) staff       (20)        0 2023-04-30 07:03:18.235631 ibmodules-0.1.2/
+-rw-r--r--   0 vik        (501) staff       (20)     1079 2023-04-29 15:50:16.000000 ibmodules-0.1.2/LICENSE
+-rw-r--r--   0 vik        (501) staff       (20)       85 2023-04-29 15:50:16.000000 ibmodules-0.1.2/MANIFEST.in
+-rw-r--r--   0 vik        (501) staff       (20)     1228 2023-04-30 07:03:18.235702 ibmodules-0.1.2/PKG-INFO
+-rw-r--r--   0 vik        (501) staff       (20)      126 2023-04-29 15:57:31.000000 ibmodules-0.1.2/README.md
+-rw-r--r--   0 vik        (501) staff       (20)       98 2023-04-29 15:50:16.000000 ibmodules-0.1.2/pyproject.toml
+-rw-r--r--   0 vik        (501) staff       (20)      112 2023-04-30 07:03:18.235936 ibmodules-0.1.2/setup.cfg
+-rw-r--r--   0 vik        (501) staff       (20)     1829 2023-04-29 16:13:11.000000 ibmodules-0.1.2/setup.py
+drwxr-xr-x   0 vik        (501) staff       (20)        0 2023-04-30 07:03:18.233551 ibmodules-0.1.2/src/
+drwxr-xr-x   0 vik        (501) staff       (20)        0 2023-04-30 07:03:18.234524 ibmodules-0.1.2/src/ibmodules/
+-rw-r--r--   0 vik        (501) staff       (20)      213 2023-04-30 07:03:10.000000 ibmodules-0.1.2/src/ibmodules/__init__.py
+-rw-r--r--   0 vik        (501) staff       (20)      588 2023-04-29 17:07:57.000000 ibmodules-0.1.2/src/ibmodules/op.py
+drwxr-xr-x   0 vik        (501) staff       (20)        0 2023-04-30 07:03:18.235502 ibmodules-0.1.2/src/ibmodules.egg-info/
+-rw-r--r--   0 vik        (501) staff       (20)     1228 2023-04-30 07:03:18.000000 ibmodules-0.1.2/src/ibmodules.egg-info/PKG-INFO
+-rw-r--r--   0 vik        (501) staff       (20)      293 2023-04-30 07:03:18.000000 ibmodules-0.1.2/src/ibmodules.egg-info/SOURCES.txt
+-rw-r--r--   0 vik        (501) staff       (20)        1 2023-04-30 07:03:18.000000 ibmodules-0.1.2/src/ibmodules.egg-info/dependency_links.txt
+-rw-r--r--   0 vik        (501) staff       (20)       22 2023-04-30 07:03:18.000000 ibmodules-0.1.2/src/ibmodules.egg-info/requires.txt
+-rw-r--r--   0 vik        (501) staff       (20)       10 2023-04-30 07:03:18.000000 ibmodules-0.1.2/src/ibmodules.egg-info/top_level.txt
```

### Comparing `ibmodules-0.1.1/LICENSE` & `ibmodules-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ibmodules-0.1.1/PKG-INFO` & `ibmodules-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibmodules
-Version: 0.1.1
+Version: 0.1.2
 Summary: ibmodules for "interesting bit" operations
 Home-page: https://github.com/vin01/ibmodules
 Author: Bhou Gonzas
 Author-email: vhbhousuber@protonmail.com
 Project-URL: Documentation, https://github.com/vin01/ibmodules
 Project-URL: Bug Reports, https://github.com/vin01/ibmodules/issues
 Project-URL: Source Code, https://github.com/vin01/ibmodules
```

### Comparing `ibmodules-0.1.1/setup.py` & `ibmodules-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `ibmodules-0.1.1/src/ibmodules/op.py` & `ibmodules-0.1.2/src/ibmodules/op.py`

 * *Files identical despite different names*

### Comparing `ibmodules-0.1.1/src/ibmodules.egg-info/PKG-INFO` & `ibmodules-0.1.2/src/ibmodules.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibmodules
-Version: 0.1.1
+Version: 0.1.2
 Summary: ibmodules for "interesting bit" operations
 Home-page: https://github.com/vin01/ibmodules
 Author: Bhou Gonzas
 Author-email: vhbhousuber@protonmail.com
 Project-URL: Documentation, https://github.com/vin01/ibmodules
 Project-URL: Bug Reports, https://github.com/vin01/ibmodules/issues
 Project-URL: Source Code, https://github.com/vin01/ibmodules
```

