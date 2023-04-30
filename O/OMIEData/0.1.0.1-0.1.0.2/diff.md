# Comparing `tmp/OMIEData-0.1.0.1.tar.gz` & `tmp/OMIEData-0.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OMIEData-0.1.0.1.tar", last modified: Sat May  8 16:35:48 2021, max compression
+gzip compressed data, was "OMIEData-0.1.0.2.tar", last modified: Sat Apr 29 23:48:01 2023, max compression
```

## Comparing `OMIEData-0.1.0.1.tar` & `OMIEData-0.1.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2021-05-08 16:35:48.077485 OMIEData-0.1.0.1/
--rw-rw-rw-   0        0        0     1091 2021-02-14 14:15:40.000000 OMIEData-0.1.0.1/LICENSE
-drwxrwxrwx   0        0        0        0 2021-05-08 16:35:47.831398 OMIEData-0.1.0.1/OMIEData/
-drwxrwxrwx   0        0        0        0 2021-05-08 16:35:47.971303 OMIEData-0.1.0.1/OMIEData/DataImport/
--rw-rw-rw-   0        0        0        0 2021-05-02 18:02:18.000000 OMIEData-0.1.0.1/OMIEData/DataImport/__init__.py
--rw-rw-rw-   0        0        0      131 2021-05-02 18:09:14.000000 OMIEData-0.1.0.1/OMIEData/DataImport/omie_data_importer.py
--rw-rw-rw-   0        0        0     1155 2021-05-02 18:21:22.000000 OMIEData-0.1.0.1/OMIEData/DataImport/omie_data_importer_from_folder.py
--rw-rw-rw-   0        0        0     1481 2021-05-03 12:23:36.000000 OMIEData-0.1.0.1/OMIEData/DataImport/omie_data_importer_from_responses.py
--rw-rw-rw-   0        0        0      793 2021-05-03 20:37:16.000000 OMIEData-0.1.0.1/OMIEData/DataImport/omie_energy_by_technology_importer.py
--rw-rw-rw-   0        0        0      655 2021-05-08 15:57:07.000000 OMIEData-0.1.0.1/OMIEData/DataImport/omie_marginalprice_importer.py
--rw-rw-rw-   0        0        0     1027 2021-05-08 16:05:50.000000 OMIEData-0.1.0.1/OMIEData/DataImport/omie_supply_demand_curve_importer.py
-drwxrwxrwx   0        0        0        0 2021-05-08 16:35:48.008280 OMIEData-0.1.0.1/OMIEData/Downloaders/
--rw-rw-rw-   0        0        0        0 2020-11-12 18:38:09.000000 OMIEData-0.1.0.1/OMIEData/Downloaders/__init__.py
--rw-rw-rw-   0        0        0      842 2021-05-03 20:37:16.000000 OMIEData-0.1.0.1/OMIEData/Downloaders/energy_by_technology_downloader.py
--rw-rw-rw-   0        0        0     2332 2021-05-03 12:19:18.000000 OMIEData-0.1.0.1/OMIEData/Downloaders/general_omie_downloader.py
--rw-rw-rw-   0        0        0      754 2021-05-03 12:17:30.000000 OMIEData-0.1.0.1/OMIEData/Downloaders/intra_day_price_downloader.py
--rw-rw-rw-   0        0        0      483 2021-05-02 19:18:48.000000 OMIEData-0.1.0.1/OMIEData/Downloaders/marginal_price_downloader.py
--rw-rw-rw-   0        0        0      331 2021-05-03 12:17:12.000000 OMIEData-0.1.0.1/OMIEData/Downloaders/omie_downloader.py
--rw-rw-rw-   0        0        0      680 2021-05-04 20:21:58.000000 OMIEData-0.1.0.1/OMIEData/Downloaders/supply_demand_curve_downloader.py
-drwxrwxrwx   0        0        0        0 2021-05-08 16:35:48.012279 OMIEData-0.1.0.1/OMIEData/Enums/
--rw-rw-rw-   0        0        0        0 2021-05-03 19:51:18.000000 OMIEData-0.1.0.1/OMIEData/Enums/__init__.py
--rw-rw-rw-   0        0        0     2037 2021-05-03 20:37:16.000000 OMIEData-0.1.0.1/OMIEData/Enums/all_enums.py
-drwxrwxrwx   0        0        0        0 2021-05-08 16:35:48.048100 OMIEData-0.1.0.1/OMIEData/FileReaders/
--rw-rw-rw-   0        0        0        0 2020-11-12 18:38:09.000000 OMIEData-0.1.0.1/OMIEData/FileReaders/__init__.py
--rw-rw-rw-   0        0        0        6 2021-05-03 20:00:17.000000 OMIEData-0.1.0.1/OMIEData/FileReaders/data_types_energy_by_technology.py
--rw-rw-rw-   0        0        0        6 2021-05-03 20:00:17.000000 OMIEData-0.1.0.1/OMIEData/FileReaders/data_types_marginal_price_file.py
--rw-rw-rw-   0        0        0     2433 2021-05-03 20:37:16.000000 OMIEData-0.1.0.1/OMIEData/FileReaders/energy_by_technology_files_reader.py
--rw-rw-rw-   0        0        0     6005 2021-05-03 20:37:16.000000 OMIEData-0.1.0.1/OMIEData/FileReaders/marginal_price_file_reader.py
--rw-rw-rw-   0        0        0      316 2021-05-02 20:35:06.000000 OMIEData-0.1.0.1/OMIEData/FileReaders/omie_file_reader.py
--rw-rw-rw-   0        0        0     1718 2021-05-04 20:21:58.000000 OMIEData-0.1.0.1/OMIEData/FileReaders/supply_demand_curve_file_reader.py
--rw-rw-rw-   0        0        0        0 2021-02-07 14:01:25.000000 OMIEData-0.1.0.1/OMIEData/__init__.py
-drwxrwxrwx   0        0        0        0 2021-05-08 16:35:47.849374 OMIEData-0.1.0.1/OMIEData.egg-info/
--rw-rw-rw-   0        0        0     5002 2021-05-08 16:35:47.000000 OMIEData-0.1.0.1/OMIEData.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1464 2021-05-08 16:35:47.000000 OMIEData-0.1.0.1/OMIEData.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-08 16:35:47.000000 OMIEData-0.1.0.1/OMIEData.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2021-05-08 16:35:47.000000 OMIEData-0.1.0.1/OMIEData.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2021-05-08 16:35:47.000000 OMIEData-0.1.0.1/OMIEData.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5002 2021-05-08 16:35:48.076488 OMIEData-0.1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3582 2021-05-08 16:35:07.000000 OMIEData-0.1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2021-05-08 16:35:48.077485 OMIEData-0.1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      871 2021-05-08 16:35:31.000000 OMIEData-0.1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2021-05-08 16:35:48.049099 OMIEData-0.1.0.1/tests/
--rw-rw-rw-   0        0        0        0 2021-05-03 11:42:55.000000 OMIEData-0.1.0.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2021-05-08 16:35:48.075503 OMIEData-0.1.0.1/tests/filereaders_tests/
--rw-rw-rw-   0        0        0        0 2021-05-02 18:01:39.000000 OMIEData-0.1.0.1/tests/filereaders_tests/__init__.py
--rw-rw-rw-   0        0        0      893 2021-05-03 12:04:09.000000 OMIEData-0.1.0.1/tests/filereaders_tests/energy_by_technology_reader_test.py
--rw-rw-rw-   0        0        0    10294 2021-05-03 20:37:16.000000 OMIEData-0.1.0.1/tests/filereaders_tests/marginal_pricer_reader_test.py
+drwxrwxrwx   0        0        0        0 2023-04-29 23:48:01.057333 OMIEData-0.1.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-29 23:48:00.988201 OMIEData-0.1.0.2/OMIEData/
+drwxrwxrwx   0        0        0        0 2023-04-29 23:48:01.015313 OMIEData-0.1.0.2/OMIEData/DataImport/
+-rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/DataImport/__init__.py
+-rw-rw-rw-   0        0        0      131 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/DataImport/omie_data_importer.py
+-rw-rw-rw-   0        0        0     1155 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/DataImport/omie_data_importer_from_folder.py
+-rw-rw-rw-   0        0        0     1481 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/DataImport/omie_data_importer_from_responses.py
+-rw-rw-rw-   0        0        0      793 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/DataImport/omie_energy_by_technology_importer.py
+-rw-rw-rw-   0        0        0      655 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/DataImport/omie_marginalprice_importer.py
+-rw-rw-rw-   0        0        0     1027 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/DataImport/omie_supply_demand_curve_importer.py
+drwxrwxrwx   0        0        0        0 2023-04-29 23:48:01.029233 OMIEData-0.1.0.2/OMIEData/Downloaders/
+-rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/Downloaders/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/Downloaders/energy_by_technology_downloader.py
+-rw-rw-rw-   0        0        0     2332 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/Downloaders/general_omie_downloader.py
+-rw-rw-rw-   0        0        0      754 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/Downloaders/intra_day_price_downloader.py
+-rw-rw-rw-   0        0        0      483 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/Downloaders/marginal_price_downloader.py
+-rw-rw-rw-   0        0        0      331 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/Downloaders/omie_downloader.py
+-rw-rw-rw-   0        0        0      680 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/Downloaders/supply_demand_curve_downloader.py
+drwxrwxrwx   0        0        0        0 2023-04-29 23:48:01.033169 OMIEData-0.1.0.2/OMIEData/Enums/
+-rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/Enums/__init__.py
+-rw-rw-rw-   0        0        0     2037 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/Enums/all_enums.py
+drwxrwxrwx   0        0        0        0 2023-04-29 23:48:01.046944 OMIEData-0.1.0.2/OMIEData/FileReaders/
+-rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/FileReaders/__init__.py
+-rw-rw-rw-   0        0        0        6 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/FileReaders/data_types_energy_by_technology.py
+-rw-rw-rw-   0        0        0        6 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/FileReaders/data_types_marginal_price_file.py
+-rw-rw-rw-   0        0        0     2433 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/FileReaders/energy_by_technology_files_reader.py
+-rw-rw-rw-   0        0        0     6005 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/FileReaders/marginal_price_file_reader.py
+-rw-rw-rw-   0        0        0      316 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/FileReaders/omie_file_reader.py
+-rw-rw-rw-   0        0        0     1718 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/FileReaders/supply_demand_curve_file_reader.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 23:48:01.000664 OMIEData-0.1.0.2/OMIEData.egg-info/
+-rw-rw-rw-   0        0        0     5818 2023-04-29 23:48:00.000000 OMIEData-0.1.0.2/OMIEData.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1464 2023-04-29 23:48:00.000000 OMIEData-0.1.0.2/OMIEData.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 23:48:00.000000 OMIEData-0.1.0.2/OMIEData.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-29 23:48:00.000000 OMIEData-0.1.0.2/OMIEData.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-29 23:48:00.000000 OMIEData-0.1.0.2/OMIEData.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5818 2023-04-29 23:48:01.056239 OMIEData-0.1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5257 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-29 23:48:01.058333 OMIEData-0.1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      878 2023-04-29 23:47:27.000000 OMIEData-0.1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 23:48:01.048944 OMIEData-0.1.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 23:48:01.054239 OMIEData-0.1.0.2/tests/filereaders_tests/
+-rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/tests/filereaders_tests/__init__.py
+-rw-rw-rw-   0        0        0      893 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/tests/filereaders_tests/energy_by_technology_reader_test.py
+-rw-rw-rw-   0        0        0    10294 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/tests/filereaders_tests/marginal_pricer_reader_test.py
```

### Comparing `OMIEData-0.1.0.1/LICENSE` & `OMIEData-0.1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.1/OMIEData/DataImport/omie_data_importer_from_folder.py` & `OMIEData-0.1.0.2/OMIEData/DataImport/omie_data_importer_from_folder.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.1/OMIEData/DataImport/omie_data_importer_from_responses.py` & `OMIEData-0.1.0.2/OMIEData/DataImport/omie_data_importer_from_responses.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.1/OMIEData/DataImport/omie_energy_by_technology_importer.py` & `OMIEData-0.1.0.2/OMIEData/DataImport/omie_energy_by_technology_importer.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.1/OMIEData/DataImport/omie_marginalprice_importer.py` & `OMIEData-0.1.0.2/OMIEData/DataImport/omie_marginalprice_importer.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.1/OMIEData/DataImport/omie_supply_demand_curve_importer.py` & `OMIEData-0.1.0.2/OMIEData/DataImport/omie_supply_demand_curve_importer.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.1/OMIEData/Downloaders/energy_by_technology_downloader.py` & `OMIEData-0.1.0.2/OMIEData/Downloaders/energy_by_technology_downloader.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.1/OMIEData/Downloaders/general_omie_downloader.py` & `OMIEData-0.1.0.2/OMIEData/Downloaders/general_omie_downloader.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.1/OMIEData/Downloaders/intra_day_price_downloader.py` & `OMIEData-0.1.0.2/OMIEData/Downloaders/intra_day_price_downloader.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.1/OMIEData/Downloaders/supply_demand_curve_downloader.py` & `OMIEData-0.1.0.2/OMIEData/Downloaders/supply_demand_curve_downloader.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.1/OMIEData/Enums/all_enums.py` & `OMIEData-0.1.0.2/OMIEData/Enums/all_enums.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.1/OMIEData/FileReaders/energy_by_technology_files_reader.py` & `OMIEData-0.1.0.2/OMIEData/FileReaders/energy_by_technology_files_reader.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.1/OMIEData/FileReaders/marginal_price_file_reader.py` & `OMIEData-0.1.0.2/OMIEData/FileReaders/marginal_price_file_reader.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.1/OMIEData/FileReaders/supply_demand_curve_file_reader.py` & `OMIEData-0.1.0.2/OMIEData/FileReaders/supply_demand_curve_file_reader.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.1/OMIEData.egg-info/PKG-INFO` & `OMIEData-0.1.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,120 +1,143 @@
-Metadata-Version: 2.1
-Name: OMIEData
-Version: 0.1.0.1
-Summary: Package to download electricity time series from https://www.omie.es/
-Home-page: https://github.com/acruzgarcia/OMIEData
-Author: Alberto Cruz and Mirel Mora
-Author-email: a.cruz.garcia@gmail.com, mirel.mora@gmail.com
-License: UNKNOWN
-Description: # OMIEData: 
-        
-        [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-        [![PyPI version fury.io](https://img.shields.io/pypi/v/OMIEData.svg)](https://pypi.org/project/OMIEData/)
-        [![PyPI pyversions](https://img.shields.io/pypi/pyversions/OMIEData.svg)](https://www.python.org/)
-        
-        Python package to import data from OMIE (Iberian Peninsula's Electricity Market Operator): https://www.omie.es/
-        
-        Concretely, you can easily access to data for the following markets:
-        
-        - Daily market: hourly prices in Spain and Portugal, total hourly energy after auction (with/without billateral contracts), breakdown of the total hourly energy by technology and bid/ask curves.
-        - Intra-day market: hourly prices for the different sessions and total hourly energy.
-        - Additional data in next releases.
-        
-        
-        ## Installation 
-        
-        The package is uploaded at https://pypi.org/project/OMIEData/, so
-        
-        ```python
-        python -m pip install OMIEData
-        
-        ```
-        from the command line will install the last version uploaded to pypi. 
-        
-        Aternatively, to install it from GitHub repository, type:
-        
-        ```python
-        python -m pip install git+https://github.com/acruzgarcia/OMIEData
-        
-        ```
-        
-        in the command line. You can also install the .whl or .tar.gz files within [dist](https://github.com/acruzgarcia/OMIEData/tree/dev/dist) as:
-        
-        ```python
-        python -m pip install OMIEData-VERSION-py3-none-any.whl
-        
-        ```
-        or
-        
-        ```python
-        python -m pip install OMIEData-VERSION.tar.gz
-        
-        ```
-        
-        or to install a previous version from [dist_old](https://github.com/acruzgarcia/OMIEData/tree/dev/dist_old).
-        
-        ## Examples:
-        
-        A very simple example to download hourly electricity prices and demand:
-        
-        ```python
-        import datetime as dt
-        from OMIEData.DataImport.omie_marginalprice_importer import OMIEMarginalPriceFileImporter
-        
-        dateIni = dt.datetime(2012, 3, 11)
-        dateEnd = dt.datetime(2012, 4, 15)
-        
-        # This can take time, it is downloading the files from the website..
-        df = OMIEMarginalPriceFileImporter(date_ini=dateIni, date_end=dateEnd).read_to_dataframe(verbose=True)
-        df.sort_values(by='DATE', axis=0, inplace=True)
-        print(df)
-        ```
-        
-        Another example to download hourly demand resulting of the daily market auction, breakdown by technologies:
-        
-        ```python
-        import datetime as dt
-        from OMIEData.Enums.all_enums import SystemType
-        from OMIEData.DataImport.omie_energy_by_technology_importer import OMIEEnergyByTechnologyImporter
-        
-        dateIni = dt.datetime(2020, 6, 1)
-        dateEnd = dt.datetime(2020, 7, 30)
-        system_type = SystemType.SPAIN
-        
-        # This can take time, it is downloading the files from the website..
-        df = OMIEEnergyByTechnologyImporter(date_ini=dateIni,
-                                            date_end=dateEnd,
-                                            system_type=system_type).read_to_dataframe(verbose=True)
-        df.sort_values(by=['DATE', 'HOUR'], axis=0, inplace=True)
-        print(df)
-        ```
-        
-        Another example to download supply/demand curves:
-        
-        ```python
-        import datetime as dt
-        from OMIEData.DataImport.omie_supply_demand_curve_importer import OMIESupplyDemandCurvesImporter
-        
-        dateIni = dt.datetime(2020, 6, 1)
-        dateEnd = dt.datetime(2020, 6, 1)
-        hour = 1
-        
-        # This can take time, it is downloading the files from the website..
-        df = OMIESupplyDemandCurvesImporter(date_ini=dateIni, date_end=dateEnd, hour=hour).read_to_dataframe(verbose=True)
-        df.sort_values(by=['DATE', 'HOUR'], axis=0, inplace=True)
-        print(df)
-        ```
-        
-        Other examples that illustrate the use of the package in here:
-        
-        - [examples folder](https://github.com/acruzgarcia/OMIEData/tree/dev/examples)
-        
-        Enjoy!.
-        
-Keywords: OMIE,Electricity prices
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+# OMIEData: 
+
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+[![PyPI version fury.io](https://img.shields.io/pypi/v/OMIEData.svg)](https://pypi.org/project/OMIEData/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/OMIEData.svg)](https://www.python.org/)
+
+Python package to import data from OMIE (Iberian Peninsula's Electricity Market Operator): https://www.omie.es/
+
+Concretely, you can easily access to data for the following markets:
+
+- Daily market: hourly prices in Spain and Portugal, total hourly energy after auction (with/without billateral contracts), breakdown of the total hourly energy by technology and bid/ask curves.
+- Intra-day market: hourly prices for the different sessions and total hourly energy.
+- Additional data in next releases.
+
+
+## Installation 
+
+The package is uploaded at https://pypi.org/project/OMIEData/, so
+
+```python
+python -m pip install OMIEData
+
+```
+from the command line will install the last version uploaded to pypi. 
+
+Aternatively, to install it from GitHub repository, type:
+
+```python
+python -m pip install git+https://github.com/acruzgarcia/OMIEData
+
+```
+
+in the command line. You can also install the .whl or .tar.gz files within [dist](https://github.com/acruzgarcia/OMIEData/tree/dev/dist) as:
+
+```python
+python -m pip install OMIEData-VERSION-py3-none-any.whl
+
+```
+or
+
+```python
+python -m pip install OMIEData-VERSION.tar.gz
+
+```
+
+or to install a previous version from [dist_old](https://github.com/acruzgarcia/OMIEData/tree/dev/dist_old).
+
+## Examples:
+
+A very simple example to download hourly electricity prices and demand:
+
+```python
+import datetime as dt
+import matplotlib.pyplot as plt
+
+from OMIEData.DataImport.omie_marginalprice_importer import OMIEMarginalPriceFileImporter
+from OMIEData.Enums.all_enums import DataTypeInMarginalPriceFile
+
+dateIni = dt.datetime(2020, 1, 1)
+dateEnd = dt.datetime(2022, 3, 22)
+
+# This can take time, it is downloading the files from the website..
+df = OMIEMarginalPriceFileImporter(date_ini=dateIni, date_end=dateEnd).read_to_dataframe(verbose=True)
+df.sort_values(by='DATE', axis=0, inplace=True)
+print(df)
+```
+The code will generate a data-frame like the following one:
+
+```python
+            DATE         CONCEPT        H1  ...       H22       H23       H24
+0     2020-01-01        PRICE_SP     41.88  ...     45.60     42.90     37.55
+1     2020-01-01        PRICE_PT     41.88  ...     45.60     42.90     37.55
+2     2020-01-01         ENER_IB  18132.30  ...  22492.60  21800.90  19946.30
+3     2020-01-01  ENER_IB_BILLAT  26488.50  ...  32611.70  31523.70  29088.30
+4     2020-01-02        PRICE_SP     35.40  ...     42.00     38.60     33.39
+          ...             ...       ...  ...       ...       ...       ...
+3241  2022-03-21        PRICE_PT    218.69  ...    261.44    240.29    228.88
+3245  2022-03-22        PRICE_PT    223.00  ...    256.00    242.18    212.99
+3246  2022-03-22         ENER_IB  20652.20  ...  27113.50  24167.60  21841.50
+3244  2022-03-22        PRICE_SP    223.00  ...    256.00    242.18    212.99
+3247  2022-03-22  ENER_IB_BILLAT  29840.30  ...  38281.20  34781.90  31872.50
+[3248 rows x 26 columns]
+```
+
+You can filter the data-frame to have only the prices in spain, and then plot
+
+```python
+# Just prices in spain
+str_price_spain = str(DataTypeInMarginalPriceFile.PRICE_SPAIN)
+dfPrices = df[df.CONCEPT == str_price_spain]
+
+# Plotting
+plt.figure()
+plt.plot(dfPrices.DATE, dfPrices.H12, label='H12')
+plt.plot(dfPrices.DATE, dfPrices.H23, label='H23')
+plt.legend()
+plt.show()
+```
+
+which will produce the following plot:
+
+![alt text](https://github.com/acruzgarcia/OMIEData/blob/dev/images/PricesSP_H12_23.png)
+
+Another example to download hourly demand resulting of the daily market auction, breakdown by technologies:
+
+```python
+import datetime as dt
+from OMIEData.Enums.all_enums import SystemType
+from OMIEData.DataImport.omie_energy_by_technology_importer import OMIEEnergyByTechnologyImporter
+
+dateIni = dt.datetime(2020, 6, 1)
+dateEnd = dt.datetime(2020, 7, 30)
+system_type = SystemType.SPAIN
+
+# This can take time, it is downloading the files from the website..
+df = OMIEEnergyByTechnologyImporter(date_ini=dateIni,
+                                    date_end=dateEnd,
+                                    system_type=system_type).read_to_dataframe(verbose=True)
+df.sort_values(by=['DATE', 'HOUR'], axis=0, inplace=True)
+print(df)
+```
+
+Another example to download supply/demand curves:
+
+```python
+import datetime as dt
+from OMIEData.DataImport.omie_supply_demand_curve_importer import OMIESupplyDemandCurvesImporter
+
+dateIni = dt.datetime(2020, 6, 1)
+dateEnd = dt.datetime(2020, 6, 1)
+hour = 1
+
+# This can take time, it is downloading the files from the website..
+df = OMIESupplyDemandCurvesImporter(date_ini=dateIni, date_end=dateEnd, hour=hour).read_to_dataframe(verbose=True)
+df.sort_values(by=['DATE', 'HOUR'], axis=0, inplace=True)
+print(df)
+```
+
+Other examples that illustrate the use of the package in here:
+
+- [examples folder](https://github.com/acruzgarcia/OMIEData/tree/dev/examples)
+
+Enjoy!.
```

### Comparing `OMIEData-0.1.0.1/OMIEData.egg-info/SOURCES.txt` & `OMIEData-0.1.0.2/OMIEData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.1/setup.py` & `OMIEData-0.1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="OMIEData",
-    version="0.1.0.1",
+    version="0.1.0.2",
     author="Alberto Cruz and Mirel Mora",
     author_email="a.cruz.garcia@gmail.com, mirel.mora@gmail.com",
     description="Package to download electricity time series from https://www.omie.es/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/acruzgarcia/OMIEData",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(),
     python_requires='>=3.6',
     keywords=['OMIE', 'Electricity prices'],
-    install_requires=['pandas', 'requests', 'datetime']
+    install_requires=['pandas<=1.5.3', 'requests', 'datetime']
 )
```

### Comparing `OMIEData-0.1.0.1/tests/filereaders_tests/energy_by_technology_reader_test.py` & `OMIEData-0.1.0.2/tests/filereaders_tests/energy_by_technology_reader_test.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.1/tests/filereaders_tests/marginal_pricer_reader_test.py` & `OMIEData-0.1.0.2/tests/filereaders_tests/marginal_pricer_reader_test.py`

 * *Files identical despite different names*

