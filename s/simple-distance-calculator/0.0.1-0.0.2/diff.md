# Comparing `tmp/simple_distance_calculator-0.0.1.tar.gz` & `tmp/simple_distance_calculator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_distance_calculator-0.0.1.tar", last modified: Sat Apr 29 21:15:59 2023, max compression
+gzip compressed data, was "simple_distance_calculator-0.0.2.tar", last modified: Sun Apr 30 11:57:33 2023, max compression
```

## Comparing `simple_distance_calculator-0.0.1.tar` & `simple_distance_calculator-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 21:15:59.858299 simple_distance_calculator-0.0.1/
--rw-rw-rw-   0        0        0     1092 2023-04-29 21:15:11.000000 simple_distance_calculator-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      722 2023-04-29 21:15:59.859310 simple_distance_calculator-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-04-28 20:22:10.000000 simple_distance_calculator-0.0.1/README.txt
--rw-rw-rw-   0        0        0       95 2023-04-29 21:01:23.000000 simple_distance_calculator-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      378 2023-04-29 21:15:59.862574 simple_distance_calculator-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      476 2023-04-29 21:15:30.000000 simple_distance_calculator-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 21:15:59.828680 simple_distance_calculator-0.0.1/simple_distance_calculator/
--rw-rw-rw-   0        0        0        0 2023-04-27 17:58:57.000000 simple_distance_calculator-0.0.1/simple_distance_calculator/__init__.py
--rw-rw-rw-   0        0        0     1871 2023-04-28 19:34:41.000000 simple_distance_calculator-0.0.1/simple_distance_calculator/distance.py
-drwxrwxrwx   0        0        0        0 2023-04-29 21:15:59.852248 simple_distance_calculator-0.0.1/simple_distance_calculator.egg-info/
--rw-rw-rw-   0        0        0      722 2023-04-29 21:15:59.000000 simple_distance_calculator-0.0.1/simple_distance_calculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-04-29 21:15:59.000000 simple_distance_calculator-0.0.1/simple_distance_calculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 21:15:59.000000 simple_distance_calculator-0.0.1/simple_distance_calculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-29 21:15:59.000000 simple_distance_calculator-0.0.1/simple_distance_calculator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-29 21:15:59.856304 simple_distance_calculator-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-04-27 17:58:57.000000 simple_distance_calculator-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     2085 2023-04-29 21:05:06.000000 simple_distance_calculator-0.0.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-04-30 11:57:33.672967 simple_distance_calculator-0.0.2/
+-rw-rw-rw-   0        0        0     1092 2023-04-29 21:15:11.000000 simple_distance_calculator-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1096 2023-04-30 11:57:33.673965 simple_distance_calculator-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      652 2023-04-30 11:53:49.000000 simple_distance_calculator-0.0.2/README.txt
+-rw-rw-rw-   0        0        0       95 2023-04-29 21:01:23.000000 simple_distance_calculator-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      378 2023-04-30 11:57:33.677470 simple_distance_calculator-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      476 2023-04-30 11:57:16.000000 simple_distance_calculator-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 11:57:33.647660 simple_distance_calculator-0.0.2/simple_distance_calculator/
+-rw-rw-rw-   0        0        0        0 2023-04-27 17:58:57.000000 simple_distance_calculator-0.0.2/simple_distance_calculator/__init__.py
+-rw-rw-rw-   0        0        0     1871 2023-04-28 19:34:41.000000 simple_distance_calculator-0.0.2/simple_distance_calculator/distance.py
+drwxrwxrwx   0        0        0        0 2023-04-30 11:57:33.666987 simple_distance_calculator-0.0.2/simple_distance_calculator.egg-info/
+-rw-rw-rw-   0        0        0     1096 2023-04-30 11:57:33.000000 simple_distance_calculator-0.0.2/simple_distance_calculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-04-30 11:57:33.000000 simple_distance_calculator-0.0.2/simple_distance_calculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 11:57:33.000000 simple_distance_calculator-0.0.2/simple_distance_calculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-30 11:57:33.000000 simple_distance_calculator-0.0.2/simple_distance_calculator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 11:57:33.671306 simple_distance_calculator-0.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-27 17:58:57.000000 simple_distance_calculator-0.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     2085 2023-04-29 21:05:06.000000 simple_distance_calculator-0.0.2/tests/test.py
```

### Comparing `simple_distance_calculator-0.0.1/LICENSE.txt` & `simple_distance_calculator-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_distance_calculator-0.0.1/PKG-INFO` & `simple_distance_calculator-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_distance_calculator
-Version: 0.0.1
+Version: 0.0.2
 Summary: A distance calculator
 Home-page: https://github.com/Aivcho/distance_calculator
 Author: Aivcho
 Author-email: achomskis@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,7 +16,22 @@
 -convert address to lat and lon
 -covert lat and lon to address
 -Haversine formula - distance in km
 -Spherical Law of Cosines - distance in km
 -Equirectangular Approximation
 
 to calculate distances you need to use lat and lon
+
+***HOW TO USE***
+examples for caculating distances
+haversine_distance(54.9037, 23.9578, 54.9057, 23.9562)
+
+spherical_law_of_cosines_distance(54.9037, 23.9578, 54.9057, 23.9562)
+
+equirectangular_approximation(54.9037, 23.9578, 54.9057, 23.9562)
+
+examples of convertation
+
+get_address(54.686758350000005, 25.29068448063221)
+
+get_coordinates("Gedimino pilis")
+
```

### Comparing `simple_distance_calculator-0.0.1/simple_distance_calculator/distance.py` & `simple_distance_calculator-0.0.2/simple_distance_calculator/distance.py`

 * *Files identical despite different names*

### Comparing `simple_distance_calculator-0.0.1/simple_distance_calculator.egg-info/PKG-INFO` & `simple_distance_calculator-0.0.2/simple_distance_calculator.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-distance-calculator
-Version: 0.0.1
+Version: 0.0.2
 Summary: A distance calculator
 Home-page: https://github.com/Aivcho/distance_calculator
 Author: Aivcho
 Author-email: achomskis@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,7 +16,22 @@
 -convert address to lat and lon
 -covert lat and lon to address
 -Haversine formula - distance in km
 -Spherical Law of Cosines - distance in km
 -Equirectangular Approximation
 
 to calculate distances you need to use lat and lon
+
+***HOW TO USE***
+examples for caculating distances
+haversine_distance(54.9037, 23.9578, 54.9057, 23.9562)
+
+spherical_law_of_cosines_distance(54.9037, 23.9578, 54.9057, 23.9562)
+
+equirectangular_approximation(54.9037, 23.9578, 54.9057, 23.9562)
+
+examples of convertation
+
+get_address(54.686758350000005, 25.29068448063221)
+
+get_coordinates("Gedimino pilis")
+
```

### Comparing `simple_distance_calculator-0.0.1/tests/test.py` & `simple_distance_calculator-0.0.2/tests/test.py`

 * *Files identical despite different names*

