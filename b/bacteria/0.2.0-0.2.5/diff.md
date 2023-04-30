# Comparing `tmp/bacteria-0.2.0.tar.gz` & `tmp/bacteria-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacteria-0.2.0.tar", last modified: Sun Apr 30 12:57:51 2023, max compression
+gzip compressed data, was "bacteria-0.2.5.tar", last modified: Sun Apr 30 14:11:26 2023, max compression
```

## Comparing `bacteria-0.2.0.tar` & `bacteria-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 12:57:51.621000 bacteria-0.2.0/
--rw-rw-rw-   0        0        0      593 2023-04-30 12:57:51.465000 bacteria-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1312 2023-04-27 16:19:57.000000 bacteria-0.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-30 12:57:50.629000 bacteria-0.2.0/bacteria/
--rw-rw-rw-   0        0        0       34 2023-04-27 16:19:58.000000 bacteria-0.2.0/bacteria/__init__.py
--rw-rw-rw-   0        0        0   143037 2023-04-30 12:57:03.000000 bacteria-0.2.0/bacteria/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-30 12:57:51.414000 bacteria-0.2.0/bacteria.egg-info/
--rw-rw-rw-   0        0        0      593 2023-04-30 12:57:48.000000 bacteria-0.2.0/bacteria.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-30 12:57:48.000000 bacteria-0.2.0/bacteria.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 12:57:48.000000 bacteria-0.2.0/bacteria.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-04-30 12:57:48.000000 bacteria-0.2.0/bacteria.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-30 12:57:48.000000 bacteria-0.2.0/bacteria.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 12:57:51.581000 bacteria-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1097 2023-04-30 12:57:39.000000 bacteria-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 14:11:26.973000 bacteria-0.2.5/
+-rw-rw-rw-   0        0        0      593 2023-04-30 14:11:26.883000 bacteria-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      826 2023-04-30 14:09:49.000000 bacteria-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 14:11:26.441000 bacteria-0.2.5/bacteria/
+-rw-rw-rw-   0        0        0       34 2023-04-27 16:19:58.000000 bacteria-0.2.5/bacteria/__init__.py
+-rw-rw-rw-   0        0        0   143037 2023-04-30 12:57:03.000000 bacteria-0.2.5/bacteria/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-30 14:11:26.853000 bacteria-0.2.5/bacteria.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-04-30 14:11:25.000000 bacteria-0.2.5/bacteria.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-04-30 14:11:25.000000 bacteria-0.2.5/bacteria.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 14:11:25.000000 bacteria-0.2.5/bacteria.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-04-30 14:11:25.000000 bacteria-0.2.5/bacteria.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 14:11:25.000000 bacteria-0.2.5/bacteria.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 14:11:26.926000 bacteria-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1096 2023-04-30 14:11:19.000000 bacteria-0.2.5/setup.py
```

### Comparing `bacteria-0.2.0/PKG-INFO` & `bacteria-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.2.0
+Version: 0.2.5
 Summary: Super Segger Analysis in Python.
 Home-page: https://bacteria.readthedocs.io
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.2.0/bacteria/functions.py` & `bacteria-0.2.5/bacteria/functions.py`

 * *Files identical despite different names*

### Comparing `bacteria-0.2.0/bacteria.egg-info/PKG-INFO` & `bacteria-0.2.5/bacteria.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.2.0
+Version: 0.2.5
 Summary: Super Segger Analysis in Python.
 Home-page: https://bacteria.readthedocs.io
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.2.0/setup.py` & `bacteria-0.2.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import wheel
 import setuptools
  
-with open("README.rst", "r") as fh:
+with open("README.md", "r") as fh:
     long_description = fh.read()
   
 setuptools.setup(
     name = 'bacteria',         
     packages = ['bacteria'],   
-    version = '0.2.0',      
+    version = '0.2.5',      
     license='MIT',       
     description = 'Super Segger Analysis in Python.',
     long_description_content_type="text/x-rst",
     url = 'https://bacteria.readthedocs.io',  
     download_url = 'https://github.com/tuliofalmeida/bacteria',    
     keywords = ['Data analysis', 'Cell analysis', 'Bacteria', 'SuperSegger'],   
     install_requires=[
```

