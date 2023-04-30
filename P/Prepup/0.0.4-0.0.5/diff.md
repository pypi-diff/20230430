# Comparing `tmp/prepup-0.0.4.tar.gz` & `tmp/Prepup-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Prepup-0.0.4.tar", last modified: Sun Apr 30 15:46:52 2023, max compression
+gzip compressed data, was "Prepup-0.0.5.tar", last modified: Sun Apr 30 17:20:39 2023, max compression
```

## Comparing `prepup-0.0.4.tar` & `Prepup-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 15:46:52.085579 Prepup-0.0.4/
--rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 Prepup-0.0.4/AUTHORS.rst
--rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 Prepup-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 Prepup-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      551 2023-04-30 15:46:52.086584 Prepup-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-30 15:46:52.073243 Prepup-0.0.4/Prepup.egg-info/
--rw-rw-rw-   0        0        0      551 2023-04-30 15:46:51.000000 Prepup-0.0.4/Prepup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-04-30 15:46:51.000000 Prepup-0.0.4/Prepup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 15:46:51.000000 Prepup-0.0.4/Prepup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-30 15:46:51.000000 Prepup-0.0.4/Prepup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      219 2023-04-30 15:46:51.000000 Prepup-0.0.4/Prepup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-30 15:46:51.000000 Prepup-0.0.4/Prepup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      489 2023-04-29 20:41:27.000000 Prepup-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 15:46:52.078128 Prepup-0.0.4/prepup/
--rw-rw-rw-   0        0        0      148 2023-04-29 20:41:27.000000 Prepup-0.0.4/prepup/__init__.py
--rw-rw-rw-   0        0        0    27774 2023-04-29 22:23:28.000000 Prepup-0.0.4/prepup/common.py
--rw-rw-rw-   0        0        0     5349 2023-04-29 22:20:45.000000 Prepup-0.0.4/prepup/prepup.py
--rw-rw-rw-   0        0        0      202 2023-04-30 15:45:11.000000 Prepup-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0      414 2023-04-30 15:46:52.088508 Prepup-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     3239 2023-04-30 15:45:34.000000 Prepup-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 15:46:52.084602 Prepup-0.0.4/tests/
--rw-rw-rw-   0        0        0       37 2023-04-29 20:41:27.000000 Prepup-0.0.4/tests/__init__.py
--rw-rw-rw-   0        0        0      403 2023-04-29 20:41:27.000000 Prepup-0.0.4/tests/test_prepup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 17:20:39.395629 Prepup-0.0.5/
+-rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 Prepup-0.0.5/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 Prepup-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 Prepup-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      929 2023-04-30 17:20:39.395629 Prepup-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-30 17:20:39.385038 Prepup-0.0.5/Prepup.egg-info/
+-rw-rw-rw-   0        0        0      929 2023-04-30 17:20:39.000000 Prepup-0.0.5/Prepup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-04-30 17:20:39.000000 Prepup-0.0.5/Prepup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 17:20:39.000000 Prepup-0.0.5/Prepup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-30 17:20:39.000000 Prepup-0.0.5/Prepup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      219 2023-04-30 17:20:39.000000 Prepup-0.0.5/Prepup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-30 17:20:39.000000 Prepup-0.0.5/Prepup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      489 2023-04-29 20:41:27.000000 Prepup-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 17:20:39.390745 Prepup-0.0.5/prepup/
+-rw-rw-rw-   0        0        0      148 2023-04-29 20:41:27.000000 Prepup-0.0.5/prepup/__init__.py
+-rw-rw-rw-   0        0        0    27774 2023-04-29 22:23:28.000000 Prepup-0.0.5/prepup/common.py
+-rw-rw-rw-   0        0        0     5349 2023-04-29 22:20:45.000000 Prepup-0.0.5/prepup/prepup.py
+-rw-rw-rw-   0        0        0      202 2023-04-30 15:45:11.000000 Prepup-0.0.5/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-04-30 17:20:39.397582 Prepup-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     3633 2023-04-30 17:20:10.000000 Prepup-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 17:20:39.394652 Prepup-0.0.5/tests/
+-rw-rw-rw-   0        0        0       37 2023-04-29 20:41:27.000000 Prepup-0.0.5/tests/__init__.py
+-rw-rw-rw-   0        0        0      403 2023-04-29 20:41:27.000000 Prepup-0.0.5/tests/test_prepup.py
```

### Comparing `Prepup-0.0.4/LICENSE` & `Prepup-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Prepup-0.0.4/prepup/common.py` & `Prepup-0.0.5/prepup/common.py`

 * *Files identical despite different names*

### Comparing `Prepup-0.0.4/prepup/prepup.py` & `Prepup-0.0.5/prepup/prepup.py`

 * *Files identical despite different names*

### Comparing `Prepup-0.0.4/setup.py` & `Prepup-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,27 +56,35 @@
 #     zip_safe=False,
 # )
 
 import setuptools
 
 setuptools.setup(
     name="Prepup",
-    version="0.0.4",
+    version="0.0.5",
+    license='MIT',
     author="Sudhanshu Mukherjee",
     author_email="sudhanshumukherjeexx@gmail.com",
     description="Prepup is a free, open-source package that lets you open, explore, visualize and pre-process datasets in your computer's terminal.",
+    url='https://github.com/sudhanshumukherjeexx/prepup',
+    keywords=['DATA PREPROCESSING','TERMINAL', 'DATA SCIENCE', 'EDA'],
     packages=setuptools.find_packages(),
     entry_points={
         "console_scripts": [
             "prepup = prepup.prepup:main",
         ]
     },
-    url='https://github.com/sudhanshumukherjeexx/prepup',
     classifiers=[
         "Programming Language :: Python :: 3",
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     install_requires=[
         "argparse",
         "polars",
```

