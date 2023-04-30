# Comparing `tmp/lpython_emulation-0.0.1.3.tar.gz` & `tmp/lpython_emulation-0.0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpython_emulation-0.0.1.3.tar", last modified: Sun Apr 30 17:17:19 2023, max compression
+gzip compressed data, was "lpython_emulation-0.0.1.4.tar", last modified: Sun Apr 30 17:35:52 2023, max compression
```

## Comparing `lpython_emulation-0.0.1.3.tar` & `lpython_emulation-0.0.1.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-30 17:17:19.719153 lpython_emulation-0.0.1.3/
--rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-04-21 16:22:30.000000 lpython_emulation-0.0.1.3/LICENSE
--rw-r--r--   0 ubaid      (501) staff       (20)      551 2023-04-30 17:17:19.719018 lpython_emulation-0.0.1.3/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)       88 2023-04-28 22:01:10.000000 lpython_emulation-0.0.1.3/README.md
--rw-r--r--   0 ubaid      (501) staff       (20)    15499 2023-04-30 17:14:24.000000 lpython_emulation-0.0.1.3/lpython.py
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-30 17:17:19.718840 lpython_emulation-0.0.1.3/lpython_emulation.egg-info/
--rw-r--r--   0 ubaid      (501) staff       (20)      551 2023-04-30 17:17:19.000000 lpython_emulation-0.0.1.3/lpython_emulation.egg-info/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)      201 2023-04-30 17:17:19.000000 lpython_emulation-0.0.1.3/lpython_emulation.egg-info/SOURCES.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-04-30 17:17:19.000000 lpython_emulation-0.0.1.3/lpython_emulation.egg-info/dependency_links.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        8 2023-04-30 17:17:19.000000 lpython_emulation-0.0.1.3/lpython_emulation.egg-info/top_level.txt
--rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-04-30 17:17:19.719188 lpython_emulation-0.0.1.3/setup.cfg
--rw-r--r--   0 ubaid      (501) staff       (20)     1781 2023-04-30 17:17:09.000000 lpython_emulation-0.0.1.3/setup.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-30 17:35:52.381497 lpython_emulation-0.0.1.4/
+-rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-04-21 16:22:30.000000 lpython_emulation-0.0.1.4/LICENSE
+-rw-r--r--   0 ubaid      (501) staff       (20)      551 2023-04-30 17:35:52.381341 lpython_emulation-0.0.1.4/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)       88 2023-04-28 22:01:10.000000 lpython_emulation-0.0.1.4/README.md
+-rw-r--r--   0 ubaid      (501) staff       (20)     7587 2023-04-21 16:22:30.000000 lpython_emulation-0.0.1.4/goto.py
+-rw-r--r--   0 ubaid      (501) staff       (20)    15499 2023-04-30 17:14:24.000000 lpython_emulation-0.0.1.4/lpython.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-30 17:35:52.381151 lpython_emulation-0.0.1.4/lpython_emulation.egg-info/
+-rw-r--r--   0 ubaid      (501) staff       (20)      551 2023-04-30 17:35:52.000000 lpython_emulation-0.0.1.4/lpython_emulation.egg-info/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)      209 2023-04-30 17:35:52.000000 lpython_emulation-0.0.1.4/lpython_emulation.egg-info/SOURCES.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-04-30 17:35:52.000000 lpython_emulation-0.0.1.4/lpython_emulation.egg-info/dependency_links.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)       13 2023-04-30 17:35:52.000000 lpython_emulation-0.0.1.4/lpython_emulation.egg-info/top_level.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-04-30 17:35:52.381536 lpython_emulation-0.0.1.4/setup.cfg
+-rw-r--r--   0 ubaid      (501) staff       (20)     1789 2023-04-30 17:20:37.000000 lpython_emulation-0.0.1.4/setup.py
```

### Comparing `lpython_emulation-0.0.1.3/LICENSE` & `lpython_emulation-0.0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lpython_emulation-0.0.1.3/PKG-INFO` & `lpython_emulation-0.0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpython_emulation
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: Package for adding type information to python
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Ondrej Certik
 Author-email: ondrej@certik.us
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lpython_emulation-0.0.1.3/lpython.py` & `lpython_emulation-0.0.1.4/lpython.py`

 * *Files identical despite different names*

### Comparing `lpython_emulation-0.0.1.3/lpython_emulation.egg-info/PKG-INFO` & `lpython_emulation-0.0.1.4/lpython_emulation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpython-emulation
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: Package for adding type information to python
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Ondrej Certik
 Author-email: ondrej@certik.us
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lpython_emulation-0.0.1.3/setup.py` & `lpython_emulation-0.0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 import setuptools
 
 # Define required packages. Alternatively, these could be defined in a separate
 # file and read in here.
 REQUIRED_PACKAGES=[]
 
-VERSION="0.0.1.3"
+VERSION="0.0.1.4"
 
 # Read in the project description. We define this in the README file.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lpython_emulation",                                   # name of project
-    py_modules=['lpython'],
+    py_modules=["lpython", "goto"],
     install_requires=REQUIRED_PACKAGES,                         # all requirements used by this package
     version=VERSION,                                            # project version, read from version.py
     author="Ondrej Certik",                                     # Author, shown on PyPI
     author_email="ondrej@certik.us",                            # Author email
     description="Package for adding type information to python",# Short description of project
     long_description=long_description,                          # Long description, shown on PyPI
     long_description_content_type="text/markdown",              # Content type. Here, we used a markdown file.
```

