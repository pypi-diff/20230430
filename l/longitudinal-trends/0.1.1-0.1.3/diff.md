# Comparing `tmp/longitudinal_trends-0.1.1.tar.gz` & `tmp/longitudinal_trends-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longitudinal_trends-0.1.1.tar", last modified: Sat Apr 15 12:33:04 2023, max compression
+gzip compressed data, was "longitudinal_trends-0.1.3.tar", last modified: Sun Apr 30 17:14:37 2023, max compression
```

## Comparing `longitudinal_trends-0.1.1.tar` & `longitudinal_trends-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-15 12:33:04.224443 longitudinal_trends-0.1.1/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1104 2023-03-18 15:04:53.000000 longitudinal_trends-0.1.1/LICENSE
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       34 2023-03-18 16:38:44.000000 longitudinal_trends-0.1.1/MANIFEST.in
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9927 2023-04-15 12:33:04.213915 longitudinal_trends-0.1.1/PKG-INFO
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9349 2023-04-07 07:04:07.000000 longitudinal_trends-0.1.1/README.md
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-15 12:33:03.621832 longitudinal_trends-0.1.1/longitudinal_trends/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)    17412 2023-04-10 18:21:23.000000 longitudinal_trends-0.1.1/longitudinal_trends/__init__.py
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-15 12:33:04.122380 longitudinal_trends-0.1.1/longitudinal_trends.egg-info/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9927 2023-04-15 12:33:02.000000 longitudinal_trends-0.1.1/longitudinal_trends.egg-info/PKG-INFO
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)      307 2023-04-15 12:33:03.000000 longitudinal_trends-0.1.1/longitudinal_trends.egg-info/SOURCES.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)        1 2023-04-15 12:33:02.000000 longitudinal_trends-0.1.1/longitudinal_trends.egg-info/dependency_links.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       45 2023-04-15 12:33:02.000000 longitudinal_trends-0.1.1/longitudinal_trends.egg-info/requires.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       20 2023-04-15 12:33:02.000000 longitudinal_trends-0.1.1/longitudinal_trends.egg-info/top_level.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1141 2023-04-15 12:27:49.000000 longitudinal_trends-0.1.1/pyproject.toml
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)      136 2023-04-03 18:57:25.000000 longitudinal_trends-0.1.1/requirements.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       38 2023-04-15 12:33:04.229457 longitudinal_trends-0.1.1/setup.cfg
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-30 17:14:37.823988 longitudinal_trends-0.1.3/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1104 2023-03-18 15:04:53.000000 longitudinal_trends-0.1.3/LICENSE
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       34 2023-03-18 16:38:44.000000 longitudinal_trends-0.1.3/MANIFEST.in
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10037 2023-04-30 17:14:37.808386 longitudinal_trends-0.1.3/PKG-INFO
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9461 2023-04-29 14:14:41.000000 longitudinal_trends-0.1.3/README.md
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-30 17:14:37.479471 longitudinal_trends-0.1.3/longitudinal_trends/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)    18095 2023-04-28 12:55:14.000000 longitudinal_trends-0.1.3/longitudinal_trends/__init__.py
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-30 17:14:37.730332 longitudinal_trends-0.1.3/longitudinal_trends.egg-info/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10037 2023-04-30 17:14:36.000000 longitudinal_trends-0.1.3/longitudinal_trends.egg-info/PKG-INFO
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)      307 2023-04-30 17:14:37.000000 longitudinal_trends-0.1.3/longitudinal_trends.egg-info/SOURCES.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)        1 2023-04-30 17:14:36.000000 longitudinal_trends-0.1.3/longitudinal_trends.egg-info/dependency_links.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       45 2023-04-30 17:14:36.000000 longitudinal_trends-0.1.3/longitudinal_trends.egg-info/requires.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       20 2023-04-30 17:14:36.000000 longitudinal_trends-0.1.3/longitudinal_trends.egg-info/top_level.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1141 2023-04-29 11:13:53.000000 longitudinal_trends-0.1.3/pyproject.toml
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       44 2023-04-15 18:04:14.000000 longitudinal_trends-0.1.3/requirements.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       38 2023-04-30 17:14:37.823988 longitudinal_trends-0.1.3/setup.cfg
```

### Comparing `longitudinal_trends-0.1.1/LICENSE` & `longitudinal_trends-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `longitudinal_trends-0.1.1/PKG-INFO` & `longitudinal_trends-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: longitudinal_trends
-Version: 0.1.1
+Version: 0.1.3
 Summary: Generate long-term longitudinal Google Trends Data
 Author: Mohammad Saleh Ahsan Sakir, Taeyong Park
 Author-email: ahsansakir506@gmail.com, taeyongp@andrew.cmu.edu
 License: MIT
 Project-URL: homepage, https://github.com/Mohammad-sakir/longitudinalTrends
 Keywords: longitudinal-trends longitudinal data python google-trends-api google-trends search-data
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # longitudinal_trends
 
 ## Introduction
 
 This is a python library for downloading cross-section and time-series Google Trends and converting them to longitudinal data.
 
-Although Google Trends provides cross-section and time-series search data, longitudinal Google Trends data are not readily available. There exist several practical issues that make it difficult for researchers to generate longitudinal Google Trends data themselves. First, Google Trends provides normalized counts from zero to 100. As a result, combining different regions' time-series Google Trends data does not create desired longitudinal data. For the same reason, combining cross-sectional Google Trends data over time does not create desired longitudinal data. Second, Google Trends has restrictions on data formats and timeline. For instance, if you want to collect daily data for 2 years, you cannot do so. Google Trends automatically provides weekly data if your request timeline is more than 269 days. Similarly, Google Trends automatically provides monthly data if your request timeline is more than 269 weeks even though you want to collect weekly data. 
+Although Google Trends provides cross-section and time-series search data, longitudinal Google Trends data are not readily available. There exist several practical issues that make it difficult for researchers to generate longitudinal Google Trends data themselves. First, Google Trends provides normalized counts from zero to 100. As a result, combining different regions' time-series Google Trends data does not create desired longitudinal data. For the same reason, combining cross-sectional Google Trends data over time does not create desired longitudinal data. Second, Google Trends has restrictions on data formats and timeline. For instance, if you want to collect daily data for 2 years, you cannot do so. Google Trends automatically provides weekly data if your request timeline is more than 269 days. Similarly, Google Trends automatically provides monthly data if your request timeline is more than 269 weeks even though you want to collect weekly data.
 
-The longitudinal_trends library resolves the aforementioned issues and allows researchers to generate longitudinal Google Trends. 
+The longitudinal_trends library resolves the aforementioned issues and allows researchers to generate longitudinal Google Trends.
 
 This library is built on top of another library `pytrends` which also have few dependencies. As long as `Google Trends API`, `pytrends` and all their dependencies work, `longitudinal_trends` will also work!
 
 ***Note**: This library is still in planning phase and not fully tested.*
 
 ## Table of contents
 
@@ -42,24 +42,20 @@
   * `convert_cross_section`
   * `all_in_one_method`
 * Caveats
 * Credits
 
 ## Installation
 
-`pip install longitudinal-trend`
+`pip install longitudinal-trends`
 
 ## Requirements
 
-Download the `requirements.txt` file from github. Then run the following command:
-
 `pip install -r requiremnts.txt`
 
-The above command will install all the required modules. Check the `requirements.txt` file for more information.
-
 ## Initiate longitudinal_trends
 
 ```python
 from longitudinal_trends import RequestTrends
 import datetime as dt
 
 day_data = RequestTrends(keyword='Insomnia', topic='/m/0ddwt', folder_name='insomnia_save', start_date=dt.datetime(2021, 11, 1), end_date=dt.datetime(2022,10,24), data_format='daily')
@@ -73,14 +69,15 @@
    **Parameters**
 
 - `keyword`
   - The keyword to be used for collecting google trends data
 - `topic`
   - The topic of the keyword. If any topic is to be used instead of search term.
     - For example, '/m/0ddwt' will give google trends data for Insomnia as topic of 'Disorder'.
+      - **NOTE**: URL's have certain codes for special characters. For example, `%20` = white space, `%2F` = / (forward slash) etc. 
     - If the topic and keyword are the same, then data provided will be for google trends search term and not any particular topic. So, `keyword='Insomnia', topic='Insomnia'` will provide google trends data for Insomnia as search term.
 - `folder_name`
   - Name of folder to be created to save all the data
 - `start_date`
   - Date to start from
 - `end_date`
   - Date to end at
@@ -89,27 +86,32 @@
   - Can choose only one from the list: ['daily', 'weekly', 'monthly']
 
 ## Methods
 
 ### cross_section
 
 ```python
-day_data.cross_section(geo='US')
+day_data.cross_section(geo='US', resolution="REGION")
 ```
 
 This method will collect cross section data of the given keyword and timeline. It calls `pytrends.interest_by_region()` method from pytrends. The data is automatically saved in →  'folder_name'/'data_format'/by_region. Each file has data for the given region/countries all the country/state google trends index for 1 day/week/month. The filenames tells the date of the data time period and also has an indication of number of day/week/month.
 
 For more information on pytrends `interest_by_region()` method, [check here](https://pypi.org/project/pytrends/#interest-by-region).
 
 **PS**: *This method takes a long time to finish running. For example, it takes around 5 hours to collect 350 days of daily data. The time is mainly due to Google Trends API rate limit.*
 
 **Parameters**
 
 - `geo`
   - Country/Region to collect data from. If left empty, then result will be worldwide i.e. data will be collected for all country. If left empty, defaults to worldwide country level.
+- `resolution`
+  - 'COUNTRY' returns country level data
+  - 'REGION' returns region level data
+  - 'CITY' returns city level data
+  - Defaults to country
 
 ### time_series
 
 ```python
 day_data.time_series(reference_geo='US-AL')
 ```
```

### Comparing `longitudinal_trends-0.1.1/README.md` & `longitudinal_trends-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # longitudinal_trends
 
 ## Introduction
 
 This is a python library for downloading cross-section and time-series Google Trends and converting them to longitudinal data.
 
-Although Google Trends provides cross-section and time-series search data, longitudinal Google Trends data are not readily available. There exist several practical issues that make it difficult for researchers to generate longitudinal Google Trends data themselves. First, Google Trends provides normalized counts from zero to 100. As a result, combining different regions' time-series Google Trends data does not create desired longitudinal data. For the same reason, combining cross-sectional Google Trends data over time does not create desired longitudinal data. Second, Google Trends has restrictions on data formats and timeline. For instance, if you want to collect daily data for 2 years, you cannot do so. Google Trends automatically provides weekly data if your request timeline is more than 269 days. Similarly, Google Trends automatically provides monthly data if your request timeline is more than 269 weeks even though you want to collect weekly data. 
+Although Google Trends provides cross-section and time-series search data, longitudinal Google Trends data are not readily available. There exist several practical issues that make it difficult for researchers to generate longitudinal Google Trends data themselves. First, Google Trends provides normalized counts from zero to 100. As a result, combining different regions' time-series Google Trends data does not create desired longitudinal data. For the same reason, combining cross-sectional Google Trends data over time does not create desired longitudinal data. Second, Google Trends has restrictions on data formats and timeline. For instance, if you want to collect daily data for 2 years, you cannot do so. Google Trends automatically provides weekly data if your request timeline is more than 269 days. Similarly, Google Trends automatically provides monthly data if your request timeline is more than 269 weeks even though you want to collect weekly data.
 
-The longitudinal_trends library resolves the aforementioned issues and allows researchers to generate longitudinal Google Trends. 
+The longitudinal_trends library resolves the aforementioned issues and allows researchers to generate longitudinal Google Trends.
 
 This library is built on top of another library `pytrends` which also have few dependencies. As long as `Google Trends API`, `pytrends` and all their dependencies work, `longitudinal_trends` will also work!
 
 ***Note**: This library is still in planning phase and not fully tested.*
 
 ## Table of contents
 
@@ -24,24 +24,20 @@
   * `convert_cross_section`
   * `all_in_one_method`
 * Caveats
 * Credits
 
 ## Installation
 
-`pip install longitudinal-trend`
+`pip install longitudinal-trends`
 
 ## Requirements
 
-Download the `requirements.txt` file from github. Then run the following command:
-
 `pip install -r requiremnts.txt`
 
-The above command will install all the required modules. Check the `requirements.txt` file for more information.
-
 ## Initiate longitudinal_trends
 
 ```python
 from longitudinal_trends import RequestTrends
 import datetime as dt
 
 day_data = RequestTrends(keyword='Insomnia', topic='/m/0ddwt', folder_name='insomnia_save', start_date=dt.datetime(2021, 11, 1), end_date=dt.datetime(2022,10,24), data_format='daily')
@@ -55,14 +51,15 @@
    **Parameters**
 
 - `keyword`
   - The keyword to be used for collecting google trends data
 - `topic`
   - The topic of the keyword. If any topic is to be used instead of search term.
     - For example, '/m/0ddwt' will give google trends data for Insomnia as topic of 'Disorder'.
+      - **NOTE**: URL's have certain codes for special characters. For example, `%20` = white space, `%2F` = / (forward slash) etc. 
     - If the topic and keyword are the same, then data provided will be for google trends search term and not any particular topic. So, `keyword='Insomnia', topic='Insomnia'` will provide google trends data for Insomnia as search term.
 - `folder_name`
   - Name of folder to be created to save all the data
 - `start_date`
   - Date to start from
 - `end_date`
   - Date to end at
@@ -71,27 +68,32 @@
   - Can choose only one from the list: ['daily', 'weekly', 'monthly']
 
 ## Methods
 
 ### cross_section
 
 ```python
-day_data.cross_section(geo='US')
+day_data.cross_section(geo='US', resolution="REGION")
 ```
 
 This method will collect cross section data of the given keyword and timeline. It calls `pytrends.interest_by_region()` method from pytrends. The data is automatically saved in →  'folder_name'/'data_format'/by_region. Each file has data for the given region/countries all the country/state google trends index for 1 day/week/month. The filenames tells the date of the data time period and also has an indication of number of day/week/month.
 
 For more information on pytrends `interest_by_region()` method, [check here](https://pypi.org/project/pytrends/#interest-by-region).
 
 **PS**: *This method takes a long time to finish running. For example, it takes around 5 hours to collect 350 days of daily data. The time is mainly due to Google Trends API rate limit.*
 
 **Parameters**
 
 - `geo`
   - Country/Region to collect data from. If left empty, then result will be worldwide i.e. data will be collected for all country. If left empty, defaults to worldwide country level.
+- `resolution`
+  - 'COUNTRY' returns country level data
+  - 'REGION' returns region level data
+  - 'CITY' returns city level data
+  - Defaults to country
 
 ### time_series
 
 ```python
 day_data.time_series(reference_geo='US-AL')
 ```
```

### Comparing `longitudinal_trends-0.1.1/longitudinal_trends/__init__.py` & `longitudinal_trends-0.1.3/longitudinal_trends/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 import time
 
 import logging
 from rich.console import Console
 from rich.logging import RichHandler
 
 from math import ceil
+import random
 
 console = Console()
 
-session = requests.Session()
-session.get('https://trends.google.com')
-cookies_map = session.cookies.get_dict()
-nid_cookie = cookies_map['NID']
+# session = requests.Session()
+# session.get('https://trends.google.com')
+# cookies_map = session.cookies.get_dict()
+# nid_cookie = cookies_map['NID']
 
 class RequestTrends:
 
     logging.basicConfig(
         level="INFO", format="%(message)s", datefmt="%d-%b-%Y %H:%M:%S", handlers=[RichHandler(rich_tracebacks=True)]
     )
 
@@ -92,15 +93,15 @@
         }
         params_fl = '{}/{}/params.txt'.format(folder_name, data_format)
         with open(params_fl, 'w') as fl:
             fl.write(json.dumps(params, indent=4, sort_keys=True, default=str))
         fl.close()
 
         # Initiaate pytrends request to enquire later
-        self.__pytrend = TrendReq(hl='en-US', tz=360, requests_args={'headers': {'Cookie': f'NID={nid_cookie}'}})
+        self.__pytrend = TrendReq(hl='en-US', tz=360)#, requests_args={'headers': {'Cookie': f'NID={nid_cookie}'}})
         self.__logger.info("Pytrend instance have been initiated for longitudinal_trend", extra={"markup": True})
 
     def __in_notebook(self):
         try:
             from IPython import get_ipython
             if 'IPKernelApp' not in get_ipython().config:  # pragma: no cover
                 return False                
@@ -119,20 +120,24 @@
 
     # This method provides list of time periods to fetch data for
     def __determine_time_periods(self):
         timeperiod = ceil(self.__num_of_days/self.TIME_WINDOW)
 
         self.__times = [self.start_date + dt.timedelta(days=x*self.TIME_WINDOW) for x in range(0, timeperiod+1)]
         self.__times[-1] = self.end_date
-   
 
-    def cross_section(self, geo=" "):
 
+    def cross_section(self, geo="", resolution="COUNTRY"):
         self.__logger.info("Collecting Cross Section Data now")
 
+        res = ["COUNTRY", "REGION", "CITY"]
+        if not geo.strip() or resolution not in res:
+            self.__logger.info("Incorrect Resolution Provided. Defaulting to 'COUNTRY'")
+            resolution = "COUNTRY"
+
         self.__create_required_directory("{}/{}/by_region".format(self.folder_name, self.data_format))
 
         if self.data_format == 'daily':
             chng_delta = relativedelta(days=1)
             end_delta = relativedelta(days=0)
             form = 'day'
         if self.data_format == 'weekly':
@@ -161,32 +166,34 @@
                         self.__logger.info("Data for {}-{} already collected. Moving to next date...".format(current_time.strftime("%#d/%m/%#Y"), current_end_time.strftime("%#d/%m/%#Y")), extra={"markup": True})
                         current_time += chng_delta
                         i += 1
                 else:
                     try:
                         self.__pytrend.build_payload(kw_list=[self.topic], geo=geo, 
                                                         timeframe='%s %s' % (current_time.strftime("%Y-%m-%d"), current_end_time.strftime("%Y-%m-%d"))) 
-                        time.sleep(15)
-                        df = self.__pytrend.interest_by_region(resolution="REGION", inc_geo_code=True)
+                        time.sleep(5)
+                        df = self.__pytrend.interest_by_region(resolution=resolution, inc_geo_code=True, inc_low_vol=True)
                         df = df.rename(columns={self.topic:self.keyword})
                         i += 1
                     except ResponseError as e:
-                        time.sleep(15)
+
+                        self.__logger.info("Please have patience as we reset rate limit ... ", extra={"markup": True})
+                        time.sleep(5)
                         continue
                     except:
                         stats.stop() # Stop the animation
                         if not self.__in_notebook():
                             self.__logger.error("[bold red]Whoops![/]", exc_info=1, extra={"markup": True})
                             quit()
                         else:
                             self.__logger.error("[bold red]Whoops![/]", exc_info=1, extra={"markup": True})
                             self.__logger.error("[bold red]Don't worry about 'Assertion Error'. [/]", extra={"markup": True})
                             assert False
                         
-                    time.sleep(15)
+                    time.sleep(5)
                     df.to_csv("{}/{}/by_region/{}_{}-{}-{}.csv".format(self.keyword, self.data_format,  form, i, current_time.strftime("%Y%m%d"), current_end_time.strftime("%Y%m%d")))
 
                     current_time += chng_delta
 
             self.__logger.info("[bold green]Successfully Collected Required Data![/]", extra={"markup": True})
 
 
@@ -195,23 +202,23 @@
         if os.path.exists("{}/{}/over_time/{}/{}-{}.csv".format(self.folder_name, self.data_format, reference_geo_code, self.start_date.strftime("%Y%m%d"), self.end_date.strftime("%Y%m%d"))):
             stats.stop()
             self.__logger.info("All Data for current request is already collected", extra={"markup": True})
         else:
             try:
                 self.__pytrend.build_payload(kw_list=[self.topic], geo=reference_geo_code, 
                                     timeframe='%s %s' % (self.start_date.strftime("%Y-%m-%d"), self.end_date.strftime("%Y-%m-%d"))) 
-                time.sleep(15)
+                time.sleep(5)
                 df = self.__pytrend.interest_over_time()
 
                 df = df.rename(columns={self.topic:self.keyword})
                 df.to_csv("{}/{}/over_time/{}/{}-{}.csv".format(self.folder_name, self.data_format, reference_geo_code, self.start_date.strftime("%Y%m%d"), self.end_date.strftime("%Y%m%d")))
             
             except ResponseError as e:
                 self.__logger.info("Please have patience as we reset rate limit ... ", extra={"markup": True})
-                time.sleep(15)
+                time.sleep(5)
             except:
                 stats.stop()
                 self.__logger.error("[bold red]Whoops![/]", exc_info=1, extra={"markup": True})
 
 
     # Time Series Data collection method for 'weekly'/'daily'
     def __time_series_nmonthly(self, stats, reference_geo_code="US"):
@@ -226,20 +233,20 @@
             
             if os.path.exists("{}/{}/over_time/{}/{}-{}-{}.csv".format(self.folder_name, self.data_format, reference_geo_code, period+1, start.strftime("%Y%m%d"), end.strftime("%Y%m%d"))):
                 self.__logger.info("Data for {} to {} already collected. Moving to next date...".format(start.strftime("%#d/%m/%#Y"), end.strftime("%#d/%m/%#Y")), extra={"markup": True})
             else:
                 try:
                     self.__pytrend.build_payload(kw_list=[self.topic], geo=reference_geo_code, 
                                         timeframe='%s %s' % (start.strftime("%Y-%m-%d"), end.strftime("%Y-%m-%d"))) 
-                    time.sleep(15)
+                    time.sleep(5)
                     df = self.__pytrend.interest_over_time()
 
                 except ResponseError as e:
                     self.__logger.info("Please have patience as we reset rate limit ... ", extra={"markup": True})
-                    time.sleep(15)
+                    time.sleep(5)
                     continue
                 except:
                     stats.stop()
                     self.__logger.error("[bold red]Whoops![/]", exc_info=1, extra={"markup": True})
                     break
 
                 if df.empty:
@@ -332,21 +339,25 @@
                 conv = conv.assign(**kwarg)
 
             stats.stop()
             conv.to_csv("{}/{}/converted/{}/final-converted-{}-{}.csv".format(self.folder_name, self.data_format, reference_geo_code, self.start_date.strftime("%Y%m%d"), self.end_date.strftime("%Y%m%d")), index=False)
             self.__logger.info("[bold green]DONE Converting! :) [/]", extra={"markup": True})
     
 
-    def all_in_one_method(self, geo=" ", reference_geo_code="US", zero_replace=0.1):
+    def all_in_one_method(self, geo="", reference_geo_code="US", zero_replace=0.1):
         # At first collect across region data for the particular region/country/dma/city
         self.cross_section(geo)
 
         # Then Collect over the time longitudinal data
         self.time_series(reference_geo_code)
 
         # Next Merge/Concatenate over the time data into a single long term trend
         self.concat_time_series(reference_geo_code, zero_replace)
 
         # Finally rescale all across region data by converting them 
         self.convert_cross_section(reference_geo_code, zero_replace)
 
-        self.__logger.info("[bold green]DONE! :) [/]", extra={"markup": True})
+        self.__logger.info("[bold green]DONE! :) [/]", extra={"markup": True})
+
+# day_data = RequestTrends('UBI', 'UBI', 'UBI_folder', dt.datetime(2012, 1, 1), dt.datetime(2022,12,31), 'daily') #4017 days
+day_data = RequestTrends('UBI', 'UBI', 'UBI_folder', dt.datetime(2022, 12, 1), dt.datetime(2022,12,31), 'daily') #4017 days
+day_data.cross_section()
```

### Comparing `longitudinal_trends-0.1.1/longitudinal_trends.egg-info/PKG-INFO` & `longitudinal_trends-0.1.3/longitudinal_trends.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: longitudinal-trends
-Version: 0.1.1
+Version: 0.1.3
 Summary: Generate long-term longitudinal Google Trends Data
 Author: Mohammad Saleh Ahsan Sakir, Taeyong Park
 Author-email: ahsansakir506@gmail.com, taeyongp@andrew.cmu.edu
 License: MIT
 Project-URL: homepage, https://github.com/Mohammad-sakir/longitudinalTrends
 Keywords: longitudinal-trends longitudinal data python google-trends-api google-trends search-data
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # longitudinal_trends
 
 ## Introduction
 
 This is a python library for downloading cross-section and time-series Google Trends and converting them to longitudinal data.
 
-Although Google Trends provides cross-section and time-series search data, longitudinal Google Trends data are not readily available. There exist several practical issues that make it difficult for researchers to generate longitudinal Google Trends data themselves. First, Google Trends provides normalized counts from zero to 100. As a result, combining different regions' time-series Google Trends data does not create desired longitudinal data. For the same reason, combining cross-sectional Google Trends data over time does not create desired longitudinal data. Second, Google Trends has restrictions on data formats and timeline. For instance, if you want to collect daily data for 2 years, you cannot do so. Google Trends automatically provides weekly data if your request timeline is more than 269 days. Similarly, Google Trends automatically provides monthly data if your request timeline is more than 269 weeks even though you want to collect weekly data. 
+Although Google Trends provides cross-section and time-series search data, longitudinal Google Trends data are not readily available. There exist several practical issues that make it difficult for researchers to generate longitudinal Google Trends data themselves. First, Google Trends provides normalized counts from zero to 100. As a result, combining different regions' time-series Google Trends data does not create desired longitudinal data. For the same reason, combining cross-sectional Google Trends data over time does not create desired longitudinal data. Second, Google Trends has restrictions on data formats and timeline. For instance, if you want to collect daily data for 2 years, you cannot do so. Google Trends automatically provides weekly data if your request timeline is more than 269 days. Similarly, Google Trends automatically provides monthly data if your request timeline is more than 269 weeks even though you want to collect weekly data.
 
-The longitudinal_trends library resolves the aforementioned issues and allows researchers to generate longitudinal Google Trends. 
+The longitudinal_trends library resolves the aforementioned issues and allows researchers to generate longitudinal Google Trends.
 
 This library is built on top of another library `pytrends` which also have few dependencies. As long as `Google Trends API`, `pytrends` and all their dependencies work, `longitudinal_trends` will also work!
 
 ***Note**: This library is still in planning phase and not fully tested.*
 
 ## Table of contents
 
@@ -42,24 +42,20 @@
   * `convert_cross_section`
   * `all_in_one_method`
 * Caveats
 * Credits
 
 ## Installation
 
-`pip install longitudinal-trend`
+`pip install longitudinal-trends`
 
 ## Requirements
 
-Download the `requirements.txt` file from github. Then run the following command:
-
 `pip install -r requiremnts.txt`
 
-The above command will install all the required modules. Check the `requirements.txt` file for more information.
-
 ## Initiate longitudinal_trends
 
 ```python
 from longitudinal_trends import RequestTrends
 import datetime as dt
 
 day_data = RequestTrends(keyword='Insomnia', topic='/m/0ddwt', folder_name='insomnia_save', start_date=dt.datetime(2021, 11, 1), end_date=dt.datetime(2022,10,24), data_format='daily')
@@ -73,14 +69,15 @@
    **Parameters**
 
 - `keyword`
   - The keyword to be used for collecting google trends data
 - `topic`
   - The topic of the keyword. If any topic is to be used instead of search term.
     - For example, '/m/0ddwt' will give google trends data for Insomnia as topic of 'Disorder'.
+      - **NOTE**: URL's have certain codes for special characters. For example, `%20` = white space, `%2F` = / (forward slash) etc. 
     - If the topic and keyword are the same, then data provided will be for google trends search term and not any particular topic. So, `keyword='Insomnia', topic='Insomnia'` will provide google trends data for Insomnia as search term.
 - `folder_name`
   - Name of folder to be created to save all the data
 - `start_date`
   - Date to start from
 - `end_date`
   - Date to end at
@@ -89,27 +86,32 @@
   - Can choose only one from the list: ['daily', 'weekly', 'monthly']
 
 ## Methods
 
 ### cross_section
 
 ```python
-day_data.cross_section(geo='US')
+day_data.cross_section(geo='US', resolution="REGION")
 ```
 
 This method will collect cross section data of the given keyword and timeline. It calls `pytrends.interest_by_region()` method from pytrends. The data is automatically saved in →  'folder_name'/'data_format'/by_region. Each file has data for the given region/countries all the country/state google trends index for 1 day/week/month. The filenames tells the date of the data time period and also has an indication of number of day/week/month.
 
 For more information on pytrends `interest_by_region()` method, [check here](https://pypi.org/project/pytrends/#interest-by-region).
 
 **PS**: *This method takes a long time to finish running. For example, it takes around 5 hours to collect 350 days of daily data. The time is mainly due to Google Trends API rate limit.*
 
 **Parameters**
 
 - `geo`
   - Country/Region to collect data from. If left empty, then result will be worldwide i.e. data will be collected for all country. If left empty, defaults to worldwide country level.
+- `resolution`
+  - 'COUNTRY' returns country level data
+  - 'REGION' returns region level data
+  - 'CITY' returns city level data
+  - Defaults to country
 
 ### time_series
 
 ```python
 day_data.time_series(reference_geo='US-AL')
 ```
```

### Comparing `longitudinal_trends-0.1.1/pyproject.toml` & `longitudinal_trends-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools"]#, "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "longitudinal_trends"
-version='0.1.1'
+version='0.1.3'
 description="Generate long-term longitudinal Google Trends Data"
 urls = {homepage = "https://github.com/Mohammad-sakir/longitudinalTrends"}
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 authors = [
     {name = "Mohammad Saleh Ahsan Sakir"},
     {name = "Taeyong Park"}, 
     {email="ahsansakir506@gmail.com"},    
     {email = "taeyongp@andrew.cmu.edu"}
 ]
 license = {text="MIT"}
```

