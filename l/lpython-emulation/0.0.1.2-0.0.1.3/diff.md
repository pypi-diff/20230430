# Comparing `tmp/lpython_emulation-0.0.1.2.tar.gz` & `tmp/lpython_emulation-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpython_emulation-0.0.1.2.tar", last modified: Sun Apr 30 17:11:37 2023, max compression
+gzip compressed data, was "lpython_emulation-0.0.1.3.tar", last modified: Sun Apr 30 17:17:19 2023, max compression
```

## Comparing `lpython_emulation-0.0.1.2.tar` & `lpython_emulation-0.0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-30 17:11:37.525072 lpython_emulation-0.0.1.2/
--rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-04-21 16:22:30.000000 lpython_emulation-0.0.1.2/LICENSE
--rw-r--r--   0 ubaid      (501) staff       (20)      551 2023-04-30 17:11:37.524948 lpython_emulation-0.0.1.2/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)       88 2023-04-28 22:01:10.000000 lpython_emulation-0.0.1.2/README.md
--rw-r--r--   0 ubaid      (501) staff       (20)    15500 2023-04-30 17:09:04.000000 lpython_emulation-0.0.1.2/lpython.py
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-30 17:11:37.524771 lpython_emulation-0.0.1.2/lpython_emulation.egg-info/
--rw-r--r--   0 ubaid      (501) staff       (20)      551 2023-04-30 17:11:37.000000 lpython_emulation-0.0.1.2/lpython_emulation.egg-info/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)      201 2023-04-30 17:11:37.000000 lpython_emulation-0.0.1.2/lpython_emulation.egg-info/SOURCES.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-04-30 17:11:37.000000 lpython_emulation-0.0.1.2/lpython_emulation.egg-info/dependency_links.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        8 2023-04-30 17:11:37.000000 lpython_emulation-0.0.1.2/lpython_emulation.egg-info/top_level.txt
--rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-04-30 17:11:37.525107 lpython_emulation-0.0.1.2/setup.cfg
--rw-r--r--   0 ubaid      (501) staff       (20)     1781 2023-04-30 17:09:42.000000 lpython_emulation-0.0.1.2/setup.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-30 17:17:19.719153 lpython_emulation-0.0.1.3/
+-rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-04-21 16:22:30.000000 lpython_emulation-0.0.1.3/LICENSE
+-rw-r--r--   0 ubaid      (501) staff       (20)      551 2023-04-30 17:17:19.719018 lpython_emulation-0.0.1.3/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)       88 2023-04-28 22:01:10.000000 lpython_emulation-0.0.1.3/README.md
+-rw-r--r--   0 ubaid      (501) staff       (20)    15499 2023-04-30 17:14:24.000000 lpython_emulation-0.0.1.3/lpython.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-30 17:17:19.718840 lpython_emulation-0.0.1.3/lpython_emulation.egg-info/
+-rw-r--r--   0 ubaid      (501) staff       (20)      551 2023-04-30 17:17:19.000000 lpython_emulation-0.0.1.3/lpython_emulation.egg-info/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)      201 2023-04-30 17:17:19.000000 lpython_emulation-0.0.1.3/lpython_emulation.egg-info/SOURCES.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-04-30 17:17:19.000000 lpython_emulation-0.0.1.3/lpython_emulation.egg-info/dependency_links.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        8 2023-04-30 17:17:19.000000 lpython_emulation-0.0.1.3/lpython_emulation.egg-info/top_level.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-04-30 17:17:19.719188 lpython_emulation-0.0.1.3/setup.cfg
+-rw-r--r--   0 ubaid      (501) staff       (20)     1781 2023-04-30 17:17:09.000000 lpython_emulation-0.0.1.3/setup.py
```

### Comparing `lpython_emulation-0.0.1.2/LICENSE` & `lpython_emulation-0.0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lpython_emulation-0.0.1.2/PKG-INFO` & `lpython_emulation-0.0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpython_emulation
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: Package for adding type information to python
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Ondrej Certik
 Author-email: ondrej@certik.us
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lpython_emulation-0.0.1.2/lpython.py` & `lpython_emulation-0.0.1.3/lpython.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from inspect import getfullargspec, getcallargs, isclass
 import os
 import ctypes
 import platform
 from dataclasses import dataclass as py_dataclass, is_dataclass as py_is_dataclass
-from .goto import with_goto
+from goto import with_goto
 
 # TODO: this does not seem to restrict other imports
 __slots__ = ["i8", "i16", "i32", "i64", "f32", "f64", "c32", "c64", "CPtr",
         "overload", "ccall", "TypeVar", "pointer", "c_p_pointer", "Pointer",
         "p_c_pointer", "vectorize", "inline", "Union", "static", "with_goto",
         "packed", "Const", "sizeof", "ccallable"]
```

### Comparing `lpython_emulation-0.0.1.2/lpython_emulation.egg-info/PKG-INFO` & `lpython_emulation-0.0.1.3/lpython_emulation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpython-emulation
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: Package for adding type information to python
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Ondrej Certik
 Author-email: ondrej@certik.us
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lpython_emulation-0.0.1.2/setup.py` & `lpython_emulation-0.0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import setuptools
 
 # Define required packages. Alternatively, these could be defined in a separate
 # file and read in here.
 REQUIRED_PACKAGES=[]
 
-VERSION="0.0.1.2"
+VERSION="0.0.1.3"
 
 # Read in the project description. We define this in the README file.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lpython_emulation",                                   # name of project
```

