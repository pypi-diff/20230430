# Comparing `tmp/existenz_api_fetcher-0.0.8.tar.gz` & `tmp/existenz_api_fetcher-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "existenz_api_fetcher-0.0.8.tar", last modified: Mon Mar 13 14:47:23 2023, max compression
+gzip compressed data, was "existenz_api_fetcher-0.0.9.tar", last modified: Sun Apr 30 20:03:22 2023, max compression
```

## Comparing `existenz_api_fetcher-0.0.8.tar` & `existenz_api_fetcher-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2023-03-13 14:47:23.947574 existenz_api_fetcher-0.0.8/
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1073 2022-10-03 16:15:39.000000 existenz_api_fetcher-0.0.8/LICENSE.txt
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1399 2023-03-13 14:47:23.947574 existenz_api_fetcher-0.0.8/PKG-INFO
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)      918 2023-03-10 14:08:16.000000 existenz_api_fetcher-0.0.8/README.md
-drwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2023-03-13 14:47:23.648318 existenz_api_fetcher-0.0.8/existenz_api_fetcher/
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2022-09-21 17:33:00.000000 existenz_api_fetcher-0.0.8/existenz_api_fetcher/__init__.py
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)     3752 2022-10-19 10:50:04.000000 existenz_api_fetcher-0.0.8/existenz_api_fetcher/hydro.py
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1333 2023-03-07 09:59:47.000000 existenz_api_fetcher-0.0.8/existenz_api_fetcher/locations.py
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)    13936 2023-03-13 14:45:01.000000 existenz_api_fetcher-0.0.8/existenz_api_fetcher/meteo.py
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1695 2023-03-09 20:16:31.000000 existenz_api_fetcher-0.0.8/existenz_api_fetcher/pipelines.py
-drwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2023-03-13 14:47:23.806755 existenz_api_fetcher-0.0.8/existenz_api_fetcher.egg-info/
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1399 2023-03-13 14:47:23.000000 existenz_api_fetcher-0.0.8/existenz_api_fetcher.egg-info/PKG-INFO
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)      437 2023-03-13 14:47:23.000000 existenz_api_fetcher-0.0.8/existenz_api_fetcher.egg-info/SOURCES.txt
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)        1 2023-03-13 14:47:23.000000 existenz_api_fetcher-0.0.8/existenz_api_fetcher.egg-info/dependency_links.txt
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)       21 2023-03-13 14:47:23.000000 existenz_api_fetcher-0.0.8/existenz_api_fetcher.egg-info/top_level.txt
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)      592 2023-03-13 14:46:51.000000 existenz_api_fetcher-0.0.8/pyproject.toml
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)       38 2023-03-13 14:47:23.954470 existenz_api_fetcher-0.0.8/setup.cfg
-drwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2023-03-13 14:47:23.915875 existenz_api_fetcher-0.0.8/tests/
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)      345 2022-10-17 08:25:28.000000 existenz_api_fetcher-0.0.8/tests/test_hydro.py
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1037 2022-10-17 08:25:28.000000 existenz_api_fetcher-0.0.8/tests/test_meteo.py
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)      305 2022-10-17 08:25:28.000000 existenz_api_fetcher-0.0.8/tests/test_pipelines.py
+drwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2023-04-30 20:03:29.470936 existenz_api_fetcher-0.0.9/
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1073 2022-10-03 16:15:39.000000 existenz_api_fetcher-0.0.9/LICENSE.txt
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1481 2023-04-30 20:03:29.468681 existenz_api_fetcher-0.0.9/PKG-INFO
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)      918 2023-03-10 14:08:16.000000 existenz_api_fetcher-0.0.9/README.md
+drwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2023-04-30 20:03:29.331307 existenz_api_fetcher-0.0.9/existenz_api_fetcher/
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2022-09-21 17:33:00.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher/__init__.py
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)     3752 2022-10-19 10:50:04.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher/hydro.py
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1863 2023-04-29 11:39:56.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher/locations.py
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)    13936 2023-03-13 14:45:01.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher/meteo.py
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1695 2023-03-09 20:16:31.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher/pipelines.py
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)       80 2023-04-29 20:55:39.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher/test.py
+drwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2023-04-30 20:03:29.388149 existenz_api_fetcher-0.0.9/existenz_api_fetcher.egg-info/
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1481 2023-04-30 20:03:29.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher.egg-info/PKG-INFO
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)      536 2023-04-30 20:03:29.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher.egg-info/SOURCES.txt
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)        1 2023-04-30 20:03:29.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher.egg-info/dependency_links.txt
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)       69 2023-04-30 20:03:29.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher.egg-info/requires.txt
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)       27 2023-04-30 20:03:29.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher.egg-info/top_level.txt
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)      565 2023-04-29 21:08:06.000000 existenz_api_fetcher-0.0.9/pyproject.toml
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)       38 2023-04-30 20:03:29.471681 existenz_api_fetcher-0.0.9/setup.cfg
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)      872 2023-04-30 18:14:06.000000 existenz_api_fetcher-0.0.9/setup.py
+drwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2023-04-30 20:03:29.453176 existenz_api_fetcher-0.0.9/tests/
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2022-09-25 11:55:02.000000 existenz_api_fetcher-0.0.9/tests/__init__.py
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)      345 2022-10-17 08:25:28.000000 existenz_api_fetcher-0.0.9/tests/test_hydro.py
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1037 2022-10-17 08:25:28.000000 existenz_api_fetcher-0.0.9/tests/test_meteo.py
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)      305 2022-10-17 08:25:28.000000 existenz_api_fetcher-0.0.9/tests/test_pipelines.py
```

### Comparing `existenz_api_fetcher-0.0.8/LICENSE.txt` & `existenz_api_fetcher-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `existenz_api_fetcher-0.0.8/PKG-INFO` & `existenz_api_fetcher-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: existenz_api_fetcher
-Version: 0.0.8
+Version: 0.0.9
 Summary: Easily fetch swiss weather and hydrological data from the Existenz API
+Home-page: https://github.com/Lilian1510/ExistenzAPIFetcher/
+Author: Lilian Lonla
 Author-email: Lilian Lonla <lilianlonla15@gmail.com>
 Project-URL: Homepage, https://github.com/Lilian1510/ExistenzAPIFetcher/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `existenz_api_fetcher-0.0.8/README.md` & `existenz_api_fetcher-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `existenz_api_fetcher-0.0.8/existenz_api_fetcher/hydro.py` & `existenz_api_fetcher-0.0.9/existenz_api_fetcher/hydro.py`

 * *Files identical despite different names*

### Comparing `existenz_api_fetcher-0.0.8/existenz_api_fetcher/locations.py` & `existenz_api_fetcher-0.0.9/existenz_api_fetcher/locations.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pandas as pd
+import geopandas as gpd
 
 
 def geolocate(station: str) -> list:
     """
     Function to geolocate MeteoSwiss or FOEN hydrology stations.
     Args: station code (str)
     Returns: list with latitude, longitude, elevation (x, y, z) for MeteoSwiss and latitude, longitude (x, y) for FOEN
@@ -16,14 +17,26 @@
     elif station in hydro_df['station_id'].to_numpy():
         result = hydro_df.loc[hydro_df['station_id'] == station]
         return [result['lat'].to_numpy()[0], result['lon'].to_numpy()[0]]
     else:
         raise ValueError("Please enter a valid station code.")
 
 
-def maps():
+def show_maps() -> None:
+    """
+    In process...
+    """
+    meteo_df = pd.read_csv('https://api-datasette.konzept.space/existenz-api/smn_locations.csv?_size=max')
+    hydro_df = pdf.read_csv('https://api-datasette.konzept.space/existenz-api/hydro_locations.csv?_size=max')
+    crs = {'init': 'epsg:4326'}
+    meteo_gdf = gpd.GeoDataFrame(meteo_df, crs=crs).set_geometry('geometry')
+    hydro_gdf = gpd.GeoDataFrame(hydro_df, crs=crs).set_geometry('geometry')
+    print(meteo_gdf)
+
+
+def maps() -> None:
     """
     Function to help find the station code using a map.
     Prints two clickable links, one for the MeteoSwiss stations, one for the FOEN ones
     """
     print("https://api-datasette.konzept.space/existenz-api/smn_locations")
     print("https://api-datasette.konzept.space/existenz-api/hydro_locations")
```

### Comparing `existenz_api_fetcher-0.0.8/existenz_api_fetcher/meteo.py` & `existenz_api_fetcher-0.0.9/existenz_api_fetcher/meteo.py`

 * *Files identical despite different names*

### Comparing `existenz_api_fetcher-0.0.8/existenz_api_fetcher/pipelines.py` & `existenz_api_fetcher-0.0.9/existenz_api_fetcher/pipelines.py`

 * *Files identical despite different names*

### Comparing `existenz_api_fetcher-0.0.8/existenz_api_fetcher.egg-info/PKG-INFO` & `existenz_api_fetcher-0.0.9/existenz_api_fetcher.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: existenz-api-fetcher
-Version: 0.0.8
+Version: 0.0.9
 Summary: Easily fetch swiss weather and hydrological data from the Existenz API
+Home-page: https://github.com/Lilian1510/ExistenzAPIFetcher/
+Author: Lilian Lonla
 Author-email: Lilian Lonla <lilianlonla15@gmail.com>
 Project-URL: Homepage, https://github.com/Lilian1510/ExistenzAPIFetcher/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `existenz_api_fetcher-0.0.8/tests/test_meteo.py` & `existenz_api_fetcher-0.0.9/tests/test_meteo.py`

 * *Files identical despite different names*

