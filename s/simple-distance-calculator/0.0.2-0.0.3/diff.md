# Comparing `tmp/simple_distance_calculator-0.0.2.tar.gz` & `tmp/simple_distance_calculator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_distance_calculator-0.0.2.tar", last modified: Sun Apr 30 11:57:33 2023, max compression
+gzip compressed data, was "simple_distance_calculator-0.0.3.tar", last modified: Sun Apr 30 12:03:09 2023, max compression
```

## Comparing `simple_distance_calculator-0.0.2.tar` & `simple_distance_calculator-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 11:57:33.672967 simple_distance_calculator-0.0.2/
--rw-rw-rw-   0        0        0     1092 2023-04-29 21:15:11.000000 simple_distance_calculator-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1096 2023-04-30 11:57:33.673965 simple_distance_calculator-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      652 2023-04-30 11:53:49.000000 simple_distance_calculator-0.0.2/README.txt
--rw-rw-rw-   0        0        0       95 2023-04-29 21:01:23.000000 simple_distance_calculator-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      378 2023-04-30 11:57:33.677470 simple_distance_calculator-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      476 2023-04-30 11:57:16.000000 simple_distance_calculator-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 11:57:33.647660 simple_distance_calculator-0.0.2/simple_distance_calculator/
--rw-rw-rw-   0        0        0        0 2023-04-27 17:58:57.000000 simple_distance_calculator-0.0.2/simple_distance_calculator/__init__.py
--rw-rw-rw-   0        0        0     1871 2023-04-28 19:34:41.000000 simple_distance_calculator-0.0.2/simple_distance_calculator/distance.py
-drwxrwxrwx   0        0        0        0 2023-04-30 11:57:33.666987 simple_distance_calculator-0.0.2/simple_distance_calculator.egg-info/
--rw-rw-rw-   0        0        0     1096 2023-04-30 11:57:33.000000 simple_distance_calculator-0.0.2/simple_distance_calculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-04-30 11:57:33.000000 simple_distance_calculator-0.0.2/simple_distance_calculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 11:57:33.000000 simple_distance_calculator-0.0.2/simple_distance_calculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-30 11:57:33.000000 simple_distance_calculator-0.0.2/simple_distance_calculator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-30 11:57:33.671306 simple_distance_calculator-0.0.2/tests/
--rw-rw-rw-   0        0        0        0 2023-04-27 17:58:57.000000 simple_distance_calculator-0.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0     2085 2023-04-29 21:05:06.000000 simple_distance_calculator-0.0.2/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:03:09.956183 simple_distance_calculator-0.0.3/
+-rw-rw-rw-   0        0        0     1092 2023-04-29 21:15:11.000000 simple_distance_calculator-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1302 2023-04-30 12:03:09.956757 simple_distance_calculator-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2023-04-30 12:02:21.000000 simple_distance_calculator-0.0.3/README.txt
+-rw-rw-rw-   0        0        0       95 2023-04-29 21:01:23.000000 simple_distance_calculator-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      378 2023-04-30 12:03:09.961679 simple_distance_calculator-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      476 2023-04-30 12:02:55.000000 simple_distance_calculator-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:03:09.929731 simple_distance_calculator-0.0.3/simple_distance_calculator/
+-rw-rw-rw-   0        0        0        0 2023-04-27 17:58:57.000000 simple_distance_calculator-0.0.3/simple_distance_calculator/__init__.py
+-rw-rw-rw-   0        0        0     1871 2023-04-28 19:34:41.000000 simple_distance_calculator-0.0.3/simple_distance_calculator/distance.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:03:09.950795 simple_distance_calculator-0.0.3/simple_distance_calculator.egg-info/
+-rw-rw-rw-   0        0        0     1302 2023-04-30 12:03:09.000000 simple_distance_calculator-0.0.3/simple_distance_calculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-04-30 12:03:09.000000 simple_distance_calculator-0.0.3/simple_distance_calculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 12:03:09.000000 simple_distance_calculator-0.0.3/simple_distance_calculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-30 12:03:09.000000 simple_distance_calculator-0.0.3/simple_distance_calculator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 12:03:09.954906 simple_distance_calculator-0.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-27 17:58:57.000000 simple_distance_calculator-0.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     2085 2023-04-29 21:05:06.000000 simple_distance_calculator-0.0.3/tests/test.py
```

### Comparing `simple_distance_calculator-0.0.2/LICENSE.txt` & `simple_distance_calculator-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_distance_calculator-0.0.2/PKG-INFO` & `simple_distance_calculator-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_distance_calculator
-Version: 0.0.2
+Version: 0.0.3
 Summary: A distance calculator
 Home-page: https://github.com/Aivcho/distance_calculator
 Author: Aivcho
 Author-email: achomskis@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,17 @@
 -Haversine formula - distance in km
 -Spherical Law of Cosines - distance in km
 -Equirectangular Approximation
 
 to calculate distances you need to use lat and lon
 
 ***HOW TO USE***
+pip install simple-distance-calculator
+from simple_distance_calculator.distance import haversine_distance, get_coordinates, spherical_law_of_cosines_distance, get_address, equirectangular_approximation
+
 examples for caculating distances
 haversine_distance(54.9037, 23.9578, 54.9057, 23.9562)
 
 spherical_law_of_cosines_distance(54.9037, 23.9578, 54.9057, 23.9562)
 
 equirectangular_approximation(54.9037, 23.9578, 54.9057, 23.9562)
```

### Comparing `simple_distance_calculator-0.0.2/README.txt` & `simple_distance_calculator-0.0.3/README.txt`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 -Haversine formula - distance in km
 -Spherical Law of Cosines - distance in km
 -Equirectangular Approximation
 
 to calculate distances you need to use lat and lon
 
 ***HOW TO USE***
+pip install simple-distance-calculator
+from simple_distance_calculator.distance import haversine_distance, get_coordinates, spherical_law_of_cosines_distance, get_address, equirectangular_approximation
+
 examples for caculating distances
 haversine_distance(54.9037, 23.9578, 54.9057, 23.9562)
 
 spherical_law_of_cosines_distance(54.9037, 23.9578, 54.9057, 23.9562)
 
 equirectangular_approximation(54.9037, 23.9578, 54.9057, 23.9562)
```

### Comparing `simple_distance_calculator-0.0.2/simple_distance_calculator/distance.py` & `simple_distance_calculator-0.0.3/simple_distance_calculator/distance.py`

 * *Files identical despite different names*

### Comparing `simple_distance_calculator-0.0.2/simple_distance_calculator.egg-info/PKG-INFO` & `simple_distance_calculator-0.0.3/simple_distance_calculator.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-distance-calculator
-Version: 0.0.2
+Version: 0.0.3
 Summary: A distance calculator
 Home-page: https://github.com/Aivcho/distance_calculator
 Author: Aivcho
 Author-email: achomskis@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,17 @@
 -Haversine formula - distance in km
 -Spherical Law of Cosines - distance in km
 -Equirectangular Approximation
 
 to calculate distances you need to use lat and lon
 
 ***HOW TO USE***
+pip install simple-distance-calculator
+from simple_distance_calculator.distance import haversine_distance, get_coordinates, spherical_law_of_cosines_distance, get_address, equirectangular_approximation
+
 examples for caculating distances
 haversine_distance(54.9037, 23.9578, 54.9057, 23.9562)
 
 spherical_law_of_cosines_distance(54.9037, 23.9578, 54.9057, 23.9562)
 
 equirectangular_approximation(54.9037, 23.9578, 54.9057, 23.9562)
```

### Comparing `simple_distance_calculator-0.0.2/tests/test.py` & `simple_distance_calculator-0.0.3/tests/test.py`

 * *Files identical despite different names*

