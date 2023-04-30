# Comparing `tmp/ReverseShell-0.0.1.tar.gz` & `tmp/ReverseShell-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseShell-0.0.1.tar", last modified: Sun Apr 30 17:53:45 2023, max compression
+gzip compressed data, was "ReverseShell-0.0.2.tar", last modified: Sun Apr 30 18:11:43 2023, max compression
```

## Comparing `ReverseShell-0.0.1.tar` & `ReverseShell-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,25 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-30 17:53:45.187068 ReverseShell-0.0.1/
--rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-30 22:05:34.000000 ReverseShell-0.0.1/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     6093 2023-04-30 17:53:45.187068 ReverseShell-0.0.1/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     5044 2023-04-30 23:50:08.000000 ReverseShell-0.0.1/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-30 17:53:45.187068 ReverseShell-0.0.1/ReverseShell.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     6093 2023-04-30 17:53:45.000000 ReverseShell-0.0.1/ReverseShell.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      264 2023-04-30 17:53:45.000000 ReverseShell-0.0.1/ReverseShell.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-30 17:53:45.000000 ReverseShell-0.0.1/ReverseShell.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       51 2023-04-30 17:53:45.000000 ReverseShell-0.0.1/ReverseShell.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-04-30 17:53:45.000000 ReverseShell-0.0.1/ReverseShell.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-04-30 17:53:45.000000 ReverseShell-0.0.1/ReverseShell.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    23199 2023-04-30 22:33:06.000000 ReverseShell-0.0.1/ReverseShell.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-30 17:53:45.187068 ReverseShell-0.0.1/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1746 2023-04-30 22:04:14.000000 ReverseShell-0.0.1/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-30 18:11:43.786099 ReverseShell-0.0.2/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35821 2023-04-30 18:10:03.000000 ReverseShell-0.0.2/LICENSE.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       51 2023-04-30 18:10:59.000000 ReverseShell-0.0.2/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     6119 2023-04-30 18:11:43.786099 ReverseShell-0.0.2/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     5044 2023-04-30 23:50:08.000000 ReverseShell-0.0.2/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-30 18:11:43.786099 ReverseShell-0.0.2/ReverseShell.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     6119 2023-04-30 18:11:43.000000 ReverseShell-0.0.2/ReverseShell.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      570 2023-04-30 18:11:43.000000 ReverseShell-0.0.2/ReverseShell.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-30 18:11:43.000000 ReverseShell-0.0.2/ReverseShell.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       51 2023-04-30 18:11:43.000000 ReverseShell-0.0.2/ReverseShell.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-04-30 18:11:43.000000 ReverseShell-0.0.2/ReverseShell.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-04-30 18:11:43.000000 ReverseShell-0.0.2/ReverseShell.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    23199 2023-04-30 18:10:40.000000 ReverseShell-0.0.2/ReverseShell.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-30 18:11:43.786099 ReverseShell-0.0.2/clients/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3258 2023-04-30 22:31:00.000000 ReverseShell-0.0.2/clients/shellclientdns.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3698 2023-04-30 22:30:50.000000 ReverseShell-0.0.2/clients/shellclienthttp_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3862 2023-04-30 22:30:42.000000 ReverseShell-0.0.2/clients/shellclienthttps_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4734 2023-04-30 22:30:26.000000 ReverseShell-0.0.2/clients/shellclienthttpsencrypt_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2941 2023-04-30 22:30:34.000000 ReverseShell-0.0.2/clients/shellclientsocketirc.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2153 2023-04-30 22:30:02.000000 ReverseShell-0.0.2/clients/shellclientsockettcp.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2114 2023-04-30 23:10:40.000000 ReverseShell-0.0.2/clients/shellclienttcp.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3125 2023-04-30 22:29:52.000000 ReverseShell-0.0.2/clients/shellclienttcp_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2176 2023-04-30 22:29:44.000000 ReverseShell-0.0.2/clients/shellclientudp.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-30 18:11:43.786099 ReverseShell-0.0.2/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1746 2023-04-30 18:11:12.000000 ReverseShell-0.0.2/setup.py
```

### Comparing `ReverseShell-0.0.1/PKG-INFO` & `ReverseShell-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseShell
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package implements an advanced reverse shell console (supports: TCP, UDP, IRC, HTTP and DNS).
 Home-page: https://github.com/mauricelambert/ReverseShell
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: System :: Networking
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Topic :: Security
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 ![ReverseShell logo](https://mauricelambert.github.io/info/python/code/ReverseShell_small.png "ReverseShell logo")
 
 # ReverseShell
 
 ## Description
```

### Comparing `ReverseShell-0.0.1/README.md` & `ReverseShell-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.1/ReverseShell.egg-info/PKG-INFO` & `ReverseShell-0.0.2/ReverseShell.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseShell
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package implements an advanced reverse shell console (supports: TCP, UDP, IRC, HTTP and DNS).
 Home-page: https://github.com/mauricelambert/ReverseShell
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: System :: Networking
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Topic :: Security
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 ![ReverseShell logo](https://mauricelambert.github.io/info/python/code/ReverseShell_small.png "ReverseShell logo")
 
 # ReverseShell
 
 ## Description
```

### Comparing `ReverseShell-0.0.1/ReverseShell.py` & `ReverseShell-0.0.2/ReverseShell.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ###################
 
 """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
 """
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
```

### Comparing `ReverseShell-0.0.1/setup.py` & `ReverseShell-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from glob import glob
 
 setup(
     name="ReverseShell",
-    version="0.0.1",
+    version="0.0.2",
     py_modules=["ReverseShell"],
     install_requires=["PythonToolsKit"],
     author="Maurice Lambert",
     author_email="mauricelambert434@gmail.com",
     maintainer="Maurice Lambert",
     maintainer_email="mauricelambert434@gmail.com",
     description=(
```

