# Comparing `tmp/geomapdemo-0.3.0.tar.gz` & `tmp/geomapdemo-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomapdemo-0.3.0.tar", last modified: Fri Apr 28 23:50:35 2023, max compression
+gzip compressed data, was "geomapdemo-0.3.1.tar", last modified: Sun Apr 30 03:43:43 2023, max compression
```

## Comparing `geomapdemo-0.3.0.tar` & `geomapdemo-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:50:35.397118 geomapdemo-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-28 23:50:25.000000 geomapdemo-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-28 23:50:25.000000 geomapdemo-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-28 23:50:35.397118 geomapdemo-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-28 23:50:25.000000 geomapdemo-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:50:35.393118 geomapdemo-0.3.0/geomapdemo/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-28 23:50:25.000000 geomapdemo-0.3.0/geomapdemo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-28 23:50:25.000000 geomapdemo-0.3.0/geomapdemo/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-04-28 23:50:25.000000 geomapdemo-0.3.0/geomapdemo/foliumap.py
--rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-04-28 23:50:25.000000 geomapdemo-0.3.0/geomapdemo/geomapdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:50:35.397118 geomapdemo-0.3.0/geomapdemo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-28 23:50:35.000000 geomapdemo-0.3.0/geomapdemo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-28 23:50:35.000000 geomapdemo-0.3.0/geomapdemo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-28 23:50:35.000000 geomapdemo-0.3.0/geomapdemo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:50:35.000000 geomapdemo-0.3.0/geomapdemo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 23:50:35.000000 geomapdemo-0.3.0/geomapdemo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 23:50:35.000000 geomapdemo-0.3.0/geomapdemo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 23:50:25.000000 geomapdemo-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-28 23:50:35.397118 geomapdemo-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-28 23:50:25.000000 geomapdemo-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:43:43.130481 geomapdemo-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-30 03:43:28.000000 geomapdemo-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-30 03:43:28.000000 geomapdemo-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-30 03:43:43.130481 geomapdemo-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-30 03:43:28.000000 geomapdemo-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:43:43.130481 geomapdemo-0.3.1/geomapdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 03:43:28.000000 geomapdemo-0.3.1/geomapdemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-30 03:43:28.000000 geomapdemo-0.3.1/geomapdemo/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-04-30 03:43:28.000000 geomapdemo-0.3.1/geomapdemo/foliumap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-04-30 03:43:28.000000 geomapdemo-0.3.1/geomapdemo/geomapdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:43:43.130481 geomapdemo-0.3.1/geomapdemo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-30 03:43:43.000000 geomapdemo-0.3.1/geomapdemo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-30 03:43:43.000000 geomapdemo-0.3.1/geomapdemo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-30 03:43:43.000000 geomapdemo-0.3.1/geomapdemo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 03:43:43.000000 geomapdemo-0.3.1/geomapdemo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 03:43:43.000000 geomapdemo-0.3.1/geomapdemo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 03:43:43.000000 geomapdemo-0.3.1/geomapdemo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 03:43:28.000000 geomapdemo-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-30 03:43:43.130481 geomapdemo-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-30 03:43:28.000000 geomapdemo-0.3.1/setup.py
```

### Comparing `geomapdemo-0.3.0/LICENSE` & `geomapdemo-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.3.0/PKG-INFO` & `geomapdemo-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.3.0
+Version: 0.3.1
 Summary: A python package for interactive mapping.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -45,15 +46,17 @@
 -   Basic Mapping and drawing
 -   Vector and raster layer function available
 -   Ipyleaflet based interactive map function
 -   Folium based interactive map function
 
 
 ## Supported Python Version
+- Python 3
 - Python 3.7
+- Python 3.8
 - Python 3.9
 - Python 3.10
 - Python 3.11
```

### Comparing `geomapdemo-0.3.0/README.md` & `geomapdemo-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 -   Basic Mapping and drawing
 -   Vector and raster layer function available
 -   Ipyleaflet based interactive map function
 -   Folium based interactive map function
 
 
 ## Supported Python Version
+- Python 3
 - Python 3.7
+- Python 3.8
 - Python 3.9
 - Python 3.10
 - Python 3.11
```

### Comparing `geomapdemo-0.3.0/geomapdemo/foliumap.py` & `geomapdemo-0.3.1/geomapdemo/foliumap.py`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.3.0/geomapdemo/geomapdemo.py` & `geomapdemo-0.3.1/geomapdemo/geomapdemo.py`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.3.0/geomapdemo.egg-info/PKG-INFO` & `geomapdemo-0.3.1/geomapdemo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.3.0
+Version: 0.3.1
 Summary: A python package for interactive mapping.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -45,15 +46,17 @@
 -   Basic Mapping and drawing
 -   Vector and raster layer function available
 -   Ipyleaflet based interactive map function
 -   Folium based interactive map function
 
 
 ## Supported Python Version
+- Python 3
 - Python 3.7
+- Python 3.8
 - Python 3.9
 - Python 3.10
 - Python 3.11
```

### Comparing `geomapdemo-0.3.0/setup.py` & `geomapdemo-0.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     description="A python package for interactive mapping.",
     install_requires=install_requires,
     dependency_links=dependency_links,
@@ -49,10 +50,10 @@
     keywords='geomapdemo',
     name='geomapdemo',
     packages=find_packages(include=['geomapdemo', 'geomapdemo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/zyang91/geomapdemo',
-    version='0.3.0',
+    version='0.3.1',
     zip_safe=False,
 )
```

