# Comparing `tmp/pvbm-1.3.0.tar.gz` & `tmp/pvbm-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvbm-1.3.0.tar", last modified: Sun Apr 30 11:55:20 2023, max compression
+gzip compressed data, was "pvbm-1.4.0.tar", last modified: Sun Apr 30 12:28:52 2023, max compression
```

## Comparing `pvbm-1.3.0.tar` & `pvbm-1.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-04-30 11:55:20.546619 pvbm-1.3.0/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     1253 2023-04-30 11:55:20.546490 pvbm-1.3.0/PKG-INFO
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      991 2023-04-30 11:08:42.000000 pvbm-1.3.0/README.md
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-04-30 11:55:20.546281 pvbm-1.3.0/pvbm.egg-info/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     1253 2023-04-30 11:55:20.000000 pvbm-1.3.0/pvbm.egg-info/PKG-INFO
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      157 2023-04-30 11:55:20.000000 pvbm-1.3.0/pvbm.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-04-30 11:55:20.000000 pvbm-1.3.0/pvbm.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-04-30 11:55:20.000000 pvbm-1.3.0/pvbm.egg-info/requires.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-04-30 11:55:20.000000 pvbm-1.3.0/pvbm.egg-info/top_level.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-04-30 11:55:20.546660 pvbm-1.3.0/setup.cfg
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-04-30 11:53:34.000000 pvbm-1.3.0/setup.py
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-04-30 12:28:52.968233 pvbm-1.4.0/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     1253 2023-04-30 12:28:52.968117 pvbm-1.4.0/PKG-INFO
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      991 2023-04-30 11:08:42.000000 pvbm-1.4.0/README.md
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-04-30 12:28:52.967942 pvbm-1.4.0/pvbm.egg-info/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     1253 2023-04-30 12:28:52.000000 pvbm-1.4.0/pvbm.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      157 2023-04-30 12:28:52.000000 pvbm-1.4.0/pvbm.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-04-30 12:28:52.000000 pvbm-1.4.0/pvbm.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-04-30 12:28:52.000000 pvbm-1.4.0/pvbm.egg-info/requires.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-04-30 12:28:52.000000 pvbm-1.4.0/pvbm.egg-info/top_level.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-04-30 12:28:52.968270 pvbm-1.4.0/setup.cfg
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-04-30 12:28:24.000000 pvbm-1.4.0/setup.py
```

### Comparing `pvbm-1.3.0/PKG-INFO` & `pvbm-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvbm
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python Vasculature Biomarker toolbox
 Home-page: https://github.com/aim-lab/PVBM
 Author: Jonathan Fhima, Yevgeniy Men
 Author-email: jonathanfh@campus.technion.ac.il
 Description-Content-Type: text/markdown
 
 # Python Vasculature BioMarker toolbox documentation
```

### Comparing `pvbm-1.3.0/README.md` & `pvbm-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pvbm-1.3.0/pvbm.egg-info/PKG-INFO` & `pvbm-1.4.0/pvbm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvbm
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python Vasculature Biomarker toolbox
 Home-page: https://github.com/aim-lab/PVBM
 Author: Jonathan Fhima, Yevgeniy Men
 Author-email: jonathanfh@campus.technion.ac.il
 Description-Content-Type: text/markdown
 
 # Python Vasculature BioMarker toolbox documentation
```

### Comparing `pvbm-1.3.0/setup.py` & `pvbm-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         return file.read()
 
 long_description = read_readme("README.md")
 
 
 setup(
     name='pvbm',
-    version='1.3.0',
+    version='1.4.0',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "scipy",
         "scikit-image",
         "pillow"
```

