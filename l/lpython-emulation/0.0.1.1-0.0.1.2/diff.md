# Comparing `tmp/lpython_emulation-0.0.1.1.tar.gz` & `tmp/lpython_emulation-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpython_emulation-0.0.1.1.tar", last modified: Fri Apr 28 22:29:53 2023, max compression
+gzip compressed data, was "lpython_emulation-0.0.1.2.tar", last modified: Sun Apr 30 17:11:37 2023, max compression
```

## Comparing `lpython_emulation-0.0.1.1.tar` & `lpython_emulation-0.0.1.2.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-28 22:29:53.383647 lpython_emulation-0.0.1.1/
--rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-04-21 16:22:30.000000 lpython_emulation-0.0.1.1/LICENSE
--rw-r--r--   0 ubaid      (501) staff       (20)      551 2023-04-28 22:29:53.383472 lpython_emulation-0.0.1.1/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)       88 2023-04-28 22:01:10.000000 lpython_emulation-0.0.1.1/README.md
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-28 22:29:53.382659 lpython_emulation-0.0.1.1/lpython_emulation/
--rw-r--r--   0 ubaid      (501) staff       (20)       23 2023-04-28 22:23:09.000000 lpython_emulation-0.0.1.1/lpython_emulation/__init__.py
--rw-r--r--   0 ubaid      (501) staff       (20)     7587 2023-04-21 16:22:30.000000 lpython_emulation-0.0.1.1/lpython_emulation/goto.py
--rw-r--r--   0 ubaid      (501) staff       (20)    15500 2023-04-21 16:22:30.000000 lpython_emulation-0.0.1.1/lpython_emulation/lpython.py
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-28 22:29:53.383141 lpython_emulation-0.0.1.1/lpython_emulation.egg-info/
--rw-r--r--   0 ubaid      (501) staff       (20)      551 2023-04-28 22:29:53.000000 lpython_emulation-0.0.1.1/lpython_emulation.egg-info/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)      275 2023-04-28 22:29:53.000000 lpython_emulation-0.0.1.1/lpython_emulation.egg-info/SOURCES.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-04-28 22:29:53.000000 lpython_emulation-0.0.1.1/lpython_emulation.egg-info/dependency_links.txt
--rw-r--r--   0 ubaid      (501) staff       (20)       18 2023-04-28 22:29:53.000000 lpython_emulation-0.0.1.1/lpython_emulation.egg-info/top_level.txt
--rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-04-28 22:29:53.383692 lpython_emulation-0.0.1.1/setup.cfg
--rw-r--r--   0 ubaid      (501) staff       (20)     1835 2023-04-28 22:29:41.000000 lpython_emulation-0.0.1.1/setup.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-30 17:11:37.525072 lpython_emulation-0.0.1.2/
+-rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-04-21 16:22:30.000000 lpython_emulation-0.0.1.2/LICENSE
+-rw-r--r--   0 ubaid      (501) staff       (20)      551 2023-04-30 17:11:37.524948 lpython_emulation-0.0.1.2/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)       88 2023-04-28 22:01:10.000000 lpython_emulation-0.0.1.2/README.md
+-rw-r--r--   0 ubaid      (501) staff       (20)    15500 2023-04-30 17:09:04.000000 lpython_emulation-0.0.1.2/lpython.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-30 17:11:37.524771 lpython_emulation-0.0.1.2/lpython_emulation.egg-info/
+-rw-r--r--   0 ubaid      (501) staff       (20)      551 2023-04-30 17:11:37.000000 lpython_emulation-0.0.1.2/lpython_emulation.egg-info/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)      201 2023-04-30 17:11:37.000000 lpython_emulation-0.0.1.2/lpython_emulation.egg-info/SOURCES.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-04-30 17:11:37.000000 lpython_emulation-0.0.1.2/lpython_emulation.egg-info/dependency_links.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        8 2023-04-30 17:11:37.000000 lpython_emulation-0.0.1.2/lpython_emulation.egg-info/top_level.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-04-30 17:11:37.525107 lpython_emulation-0.0.1.2/setup.cfg
+-rw-r--r--   0 ubaid      (501) staff       (20)     1781 2023-04-30 17:09:42.000000 lpython_emulation-0.0.1.2/setup.py
```

### Comparing `lpython_emulation-0.0.1.1/LICENSE` & `lpython_emulation-0.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lpython_emulation-0.0.1.1/PKG-INFO` & `lpython_emulation-0.0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpython_emulation
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: Package for adding type information to python
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Ondrej Certik
 Author-email: ondrej@certik.us
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lpython_emulation-0.0.1.1/lpython_emulation/lpython.py` & `lpython_emulation-0.0.1.2/lpython.py`

 * *Files identical despite different names*

### Comparing `lpython_emulation-0.0.1.1/lpython_emulation.egg-info/PKG-INFO` & `lpython_emulation-0.0.1.2/lpython_emulation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpython-emulation
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: Package for adding type information to python
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Ondrej Certik
 Author-email: ondrej@certik.us
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lpython_emulation-0.0.1.1/setup.py` & `lpython_emulation-0.0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 
 import setuptools
 
 # Define required packages. Alternatively, these could be defined in a separate
 # file and read in here.
 REQUIRED_PACKAGES=[]
 
-VERSION="0.0.1.1"
+VERSION="0.0.1.2"
 
 # Read in the project description. We define this in the README file.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lpython_emulation",                                   # name of project
-    packages=['lpython_emulation'],
-    py_modules=['lpython_emulation.lpython'],
+    py_modules=['lpython'],
     install_requires=REQUIRED_PACKAGES,                         # all requirements used by this package
     version=VERSION,                                            # project version, read from version.py
     author="Ondrej Certik",                                     # Author, shown on PyPI
     author_email="ondrej@certik.us",                            # Author email
     description="Package for adding type information to python",# Short description of project
     long_description=long_description,                          # Long description, shown on PyPI
     long_description_content_type="text/markdown",              # Content type. Here, we used a markdown file.
```

