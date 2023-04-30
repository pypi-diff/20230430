# Comparing `tmp/omniValidator-0.0.15.tar.gz` & `tmp/omniValidator-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniValidator-0.0.15.tar", last modified: Wed Feb 15 12:35:32 2023, max compression
+gzip compressed data, was "omniValidator-0.0.16.tar", last modified: Sun Apr 30 13:23:40 2023, max compression
```

## Comparing `omniValidator-0.0.15.tar` & `omniValidator-0.0.16.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.275332 omniValidator-0.0.15/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)    11348 2023-02-13 08:22:41.000000 omniValidator-0.0.15/LICENSE
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       37 2023-02-13 08:53:45.000000 omniValidator-0.0.15/MANIFEST.in
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4758 2023-02-15 12:35:32.271332 omniValidator-0.0.15/PKG-INFO
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4251 2023-02-12 07:28:20.000000 omniValidator-0.0.15/README.md
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      100 2023-02-13 13:00:31.000000 omniValidator-0.0.15/pyproject.toml
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       94 2023-02-13 09:52:25.000000 omniValidator-0.0.15/requirements.txt
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       38 2023-02-15 12:35:32.275332 omniValidator-0.0.15/setup.cfg
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     9674 2023-02-15 12:34:48.000000 omniValidator-0.0.15/setup.py
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.259332 omniValidator-0.0.15/src/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.267332 omniValidator-0.0.15/src/omniValidator/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      141 2022-12-13 09:10:24.000000 omniValidator-0.0.15/src/omniValidator/__init__.py
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)    12429 2022-12-15 12:48:47.000000 omniValidator-0.0.15/src/omniValidator/core.py
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.263332 omniValidator-0.0.15/src/omniValidator/schemas/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.263332 omniValidator-0.0.15/src/omniValidator/schemas/omni_batch_py/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.263332 omniValidator-0.0.15/src/omniValidator/schemas/omni_batch_py/omni_batch_data/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.267332 omniValidator-0.0.15/src/omniValidator/schemas/omni_batch_py/omni_batch_data/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1600 2022-12-15 13:02:07.000000 omniValidator-0.0.15/src/omniValidator/schemas/omni_batch_py/omni_batch_data/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.263332 omniValidator-0.0.15/src/omniValidator/schemas/omni_batch_py/omni_batch_method/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.267332 omniValidator-0.0.15/src/omniValidator/schemas/omni_batch_py/omni_batch_method/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1549 2022-12-15 14:02:57.000000 omniValidator-0.0.15/src/omniValidator/schemas/omni_batch_py/omni_batch_method/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.263332 omniValidator-0.0.15/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.267332 omniValidator-0.0.15/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1163 2022-12-15 14:03:17.000000 omniValidator-0.0.15/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.263332 omniValidator-0.0.15/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.271332 omniValidator-0.0.15/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1698 2022-12-15 14:18:47.000000 omniValidator-0.0.15/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.263332 omniValidator-0.0.15/src/omniValidator/schemas/omni_clustering/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.263332 omniValidator-0.0.15/src/omniValidator/schemas/omni_clustering/omni_clustering_data/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.271332 omniValidator-0.0.15/src/omniValidator/schemas/omni_clustering/omni_clustering_data/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1536 2022-12-15 14:18:29.000000 omniValidator-0.0.15/src/omniValidator/schemas/omni_clustering/omni_clustering_data/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.263332 omniValidator-0.0.15/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.271332 omniValidator-0.0.15/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1447 2022-12-15 14:24:03.000000 omniValidator-0.0.15/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.263332 omniValidator-0.0.15/src/omniValidator/schemas/omni_clustering/omni_clustering_method/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.271332 omniValidator-0.0.15/src/omniValidator/schemas/omni_clustering/omni_clustering_method/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1207 2022-12-16 15:05:19.000000 omniValidator-0.0.15/src/omniValidator/schemas/omni_clustering/omni_clustering_method/output/requirements.json
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.263332 omniValidator-0.0.15/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.271332 omniValidator-0.0.15/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/output/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1273 2022-12-15 14:52:01.000000 omniValidator-0.0.15/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/output/requirements.json
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      148 2022-10-30 14:45:09.000000 omniValidator-0.0.15/src/omniValidator/utils.py
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      407 2022-11-10 08:45:24.000000 omniValidator-0.0.15/src/omniValidator/version.py
-drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-02-15 12:35:32.267332 omniValidator-0.0.15/src/omniValidator.egg-info/
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4758 2023-02-15 12:35:32.000000 omniValidator-0.0.15/src/omniValidator.egg-info/PKG-INFO
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1080 2023-02-15 12:35:32.000000 omniValidator-0.0.15/src/omniValidator.egg-info/SOURCES.txt
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)        1 2023-02-15 12:35:32.000000 omniValidator-0.0.15/src/omniValidator.egg-info/dependency_links.txt
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       52 2023-02-15 12:35:32.000000 omniValidator-0.0.15/src/omniValidator.egg-info/requires.txt
--rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       14 2023-02-15 12:35:32.000000 omniValidator-0.0.15/src/omniValidator.egg-info/top_level.txt
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)    11348 2023-02-13 08:22:41.000000 omniValidator-0.0.16/LICENSE
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       37 2023-02-13 08:53:45.000000 omniValidator-0.0.16/MANIFEST.in
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4743 2023-04-30 13:23:40.423234 omniValidator-0.0.16/PKG-INFO
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4236 2023-02-24 06:47:34.000000 omniValidator-0.0.16/README.md
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      100 2023-02-13 13:00:31.000000 omniValidator-0.0.16/pyproject.toml
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       94 2023-02-13 09:52:25.000000 omniValidator-0.0.16/requirements.txt
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       38 2023-04-30 13:23:40.423234 omniValidator-0.0.16/setup.cfg
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     9674 2023-04-30 13:19:05.000000 omniValidator-0.0.16/setup.py
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.415233 omniValidator-0.0.16/src/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      141 2022-12-13 09:10:24.000000 omniValidator-0.0.16/src/omniValidator/__init__.py
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)    12748 2023-04-30 13:18:26.000000 omniValidator-0.0.16/src/omniValidator/core.py
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_data/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_data/output/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1600 2022-12-15 13:02:07.000000 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_data/output/requirements.json
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_method/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_method/output/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1549 2022-12-15 14:02:57.000000 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_method/output/requirements.json
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/output/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1163 2022-12-15 14:03:17.000000 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/output/requirements.json
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/output/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1698 2022-12-15 14:18:47.000000 omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/output/requirements.json
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_data/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_data/output/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1536 2022-12-15 14:18:29.000000 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_data/output/requirements.json
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/output/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1447 2022-12-15 14:24:03.000000 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/output/requirements.json
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_method/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_method/output/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1207 2022-12-16 15:05:19.000000 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_method/output/requirements.json
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.419233 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/output/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1273 2022-12-15 14:52:01.000000 omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/output/requirements.json
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1840 2023-04-30 13:09:11.000000 omniValidator-0.0.16/src/omniValidator/utils.py
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)      407 2022-11-10 08:45:24.000000 omniValidator-0.0.16/src/omniValidator/version.py
+drwxrwxr-x   0 anthonys  (1000) anthonys  (1000)        0 2023-04-30 13:23:40.423234 omniValidator-0.0.16/src/omniValidator.egg-info/
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     4743 2023-04-30 13:23:40.000000 omniValidator-0.0.16/src/omniValidator.egg-info/PKG-INFO
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)     1080 2023-04-30 13:23:40.000000 omniValidator-0.0.16/src/omniValidator.egg-info/SOURCES.txt
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)        1 2023-04-30 13:23:40.000000 omniValidator-0.0.16/src/omniValidator.egg-info/dependency_links.txt
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       52 2023-04-30 13:23:40.000000 omniValidator-0.0.16/src/omniValidator.egg-info/requires.txt
+-rw-rw-r--   0 anthonys  (1000) anthonys  (1000)       14 2023-04-30 13:23:40.000000 omniValidator-0.0.16/src/omniValidator.egg-info/top_level.txt
```

### Comparing `omniValidator-0.0.15/LICENSE` & `omniValidator-0.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.15/PKG-INFO` & `omniValidator-0.0.16/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniValidator
-Version: 0.0.15
+Version: 0.0.16
 Summary: Validator of output files for Omnibencharmk.
 Home-page: https://github.com/omnibenchmark/omniValidator
 Author: A. Sonrel
 Author-email: anthony.sonrel@uzh.ch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -15,19 +15,19 @@
 
 # omniValidator
 
 `omniValidator` is a python module to control file requirements in an Omnibenchmark project. 
 
 ## Usage
 
-The following sections assume that your working directory is an Omnibenchmark project associated to an **existing** Omnibenchmark and stage (data, method, metric, etc.).
+The following sections assume that your working directory is an Omnibenchmark project associated to an **existing** Omnibenchmark.
 
 You can check [here](https://github.com/ansonrel/omniValidator/tree/main/src/omniValidator/schemas) if the Omnibenchmark you are working on has available validators. 
 
-If you are working with an `Omnibenchmark` object, the main function (`omniValidator.validate_requirements`) can be used without other specifications. 
+If you are working with an `Omnibenchmark` object, the main function (`omniValidator.validate_requirements`) can be used directly on this object without other specifications. 
 
 ### Display the requirements
 
 The requirements for a given Omnibenchmark module can be visualized with the following function: 
 
 ```
 import omniValidator as ov
```

### Comparing `omniValidator-0.0.15/README.md` & `omniValidator-0.0.16/src/omniValidator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,33 @@
+Metadata-Version: 2.1
+Name: omniValidator
+Version: 0.0.16
+Summary: Validator of output files for Omnibencharmk.
+Home-page: https://github.com/omnibenchmark/omniValidator
+Author: A. Sonrel
+Author-email: anthony.sonrel@uzh.ch
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # omniValidator
 
 `omniValidator` is a python module to control file requirements in an Omnibenchmark project. 
 
 ## Usage
 
-The following sections assume that your working directory is an Omnibenchmark project associated to an **existing** Omnibenchmark and stage (data, method, metric, etc.).
+The following sections assume that your working directory is an Omnibenchmark project associated to an **existing** Omnibenchmark.
 
 You can check [here](https://github.com/ansonrel/omniValidator/tree/main/src/omniValidator/schemas) if the Omnibenchmark you are working on has available validators. 
 
-If you are working with an `Omnibenchmark` object, the main function (`omniValidator.validate_requirements`) can be used without other specifications. 
+If you are working with an `Omnibenchmark` object, the main function (`omniValidator.validate_requirements`) can be used directly on this object without other specifications. 
 
 ### Display the requirements
 
 The requirements for a given Omnibenchmark module can be visualized with the following function: 
 
 ```
 import omniValidator as ov
@@ -112,8 +127,8 @@
 
 Which returns a boolean (`True`) if your JSON is valid. 
 
 ## How to modify requirements
 
 You can modify existing requirements/ JSON schemas or add new ones using pull requests or by opening an issue on the Github page of the module. 
 
-All schemas and requirements are in the [`src/omniValidator/schemas`](https://github.com/ansonrel/omniValidator/tree/main/src/omniValidator/schemas) folder of the module. 
+All schemas and requirements are in the [`src/omniValidator/schemas`](https://github.com/ansonrel/omniValidator/tree/main/src/omniValidator/schemas) folder of the module.
```

### Comparing `omniValidator-0.0.15/setup.py` & `omniValidator-0.0.16/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     name="omniValidator",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.0.15",  # Required
+    version="0.0.16",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Validator of output files for Omnibencharmk.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `omniValidator-0.0.15/src/omniValidator/core.py` & `omniValidator-0.0.16/src/omniValidator/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import os as os
 from jsonschema import validate
 import jsonref
 import jsonschema # <--
-#import logging
 from os.path import dirname
 import re
 import warnings
 from json2table import convert
 from IPython.core.display import display, HTML
+from omniValidator.utils import get_avail_keywords, get_avail_benchmarks, schema_exist
 
 
 
 class ValidationError(Exception):
      def __init__(self, value):
          self.value = value
      def __str__(self):
@@ -108,14 +108,17 @@
     if omni_obj is None:
         if benchmark is None and keyword is None and data_folder is None: 
             msg = " if `omni_obj` is not specified, the other arguments are required."
             raise Exception(msg)
     if data_folder is not None and omni_obj is not None: 
         msg = "both `data_folder` and `omni_obj` are provided but only 1 required. Only `omni_obj` will be used."
         warnings.warn(msg)
+    if data_folder is None and omni_obj is None: 
+        msg = "An omni_obj or a data folder have to be specified to be validated."
+        raise Exception(msg)
     if omni_obj is not None: 
         if keyword is not None:
             msg = "both `omni_obj` and `keyword` are provided. Using `keyword` argument only."
             warnings.warn(msg)
         else: 
             if len(omni_obj.keyword) > 2: 
                 msg = "multiple keywords found in the `omni_obj`. Using the first one."
@@ -124,14 +127,17 @@
 
         if benchmark is not None: 
             msg = "both `omni_obj` and `benchmark` are provided. Using `benchmark` argument only."
             warnings.warn(msg)
         else: 
             benchmark = omni_obj.benchmark_name        
 
+    ## Checks validity of benchmark and keyword
+    schema_exist(benchmark, keyword)
+
     ## Loads requir file
     requir = os.path.join(omni_val_path[0], 'schemas', benchmark, keyword, 'output',  'requirements.json')
     f = open(requir)
     requir = json.load(f)
 
     ## Parse requirements into regex
     requir_names = list(requir['outputs_files'].keys())
```

### Comparing `omniValidator-0.0.15/src/omniValidator/schemas/omni_batch_py/omni_batch_data/output/requirements.json` & `omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_data/output/requirements.json`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.15/src/omniValidator/schemas/omni_batch_py/omni_batch_method/output/requirements.json` & `omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_method/output/requirements.json`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.15/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/output/requirements.json` & `omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_metric_py/output/requirements.json`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.15/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/output/requirements.json` & `omniValidator-0.0.16/src/omniValidator/schemas/omni_batch_py/omni_batch_processed/output/requirements.json`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.15/src/omniValidator/schemas/omni_clustering/omni_clustering_data/output/requirements.json` & `omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_data/output/requirements.json`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.15/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/output/requirements.json` & `omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_filter/output/requirements.json`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.15/src/omniValidator/schemas/omni_clustering/omni_clustering_method/output/requirements.json` & `omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_method/output/requirements.json`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.15/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/output/requirements.json` & `omniValidator-0.0.16/src/omniValidator/schemas/omni_clustering/omni_clustering_metric/output/requirements.json`

 * *Files identical despite different names*

### Comparing `omniValidator-0.0.15/src/omniValidator.egg-info/PKG-INFO` & `omniValidator-0.0.16/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,18 @@
-Metadata-Version: 2.1
-Name: omniValidator
-Version: 0.0.15
-Summary: Validator of output files for Omnibencharmk.
-Home-page: https://github.com/omnibenchmark/omniValidator
-Author: A. Sonrel
-Author-email: anthony.sonrel@uzh.ch
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # omniValidator
 
 `omniValidator` is a python module to control file requirements in an Omnibenchmark project. 
 
 ## Usage
 
-The following sections assume that your working directory is an Omnibenchmark project associated to an **existing** Omnibenchmark and stage (data, method, metric, etc.).
+The following sections assume that your working directory is an Omnibenchmark project associated to an **existing** Omnibenchmark.
 
 You can check [here](https://github.com/ansonrel/omniValidator/tree/main/src/omniValidator/schemas) if the Omnibenchmark you are working on has available validators. 
 
-If you are working with an `Omnibenchmark` object, the main function (`omniValidator.validate_requirements`) can be used without other specifications. 
+If you are working with an `Omnibenchmark` object, the main function (`omniValidator.validate_requirements`) can be used directly on this object without other specifications. 
 
 ### Display the requirements
 
 The requirements for a given Omnibenchmark module can be visualized with the following function: 
 
 ```
 import omniValidator as ov
@@ -127,8 +112,8 @@
 
 Which returns a boolean (`True`) if your JSON is valid. 
 
 ## How to modify requirements
 
 You can modify existing requirements/ JSON schemas or add new ones using pull requests or by opening an issue on the Github page of the module. 
 
-All schemas and requirements are in the [`src/omniValidator/schemas`](https://github.com/ansonrel/omniValidator/tree/main/src/omniValidator/schemas) folder of the module. 
+All schemas and requirements are in the [`src/omniValidator/schemas`](https://github.com/ansonrel/omniValidator/tree/main/src/omniValidator/schemas) folder of the module.
```

### Comparing `omniValidator-0.0.15/src/omniValidator.egg-info/SOURCES.txt` & `omniValidator-0.0.16/src/omniValidator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

