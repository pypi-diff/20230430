# Comparing `tmp/weatherly-0.4.0.tar.gz` & `tmp/weatherly-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weatherly-0.4.0.tar", last modified: Sun Apr 30 20:28:02 2023, max compression
+gzip compressed data, was "weatherly-0.5.0.tar", last modified: Sun Apr 30 21:53:06 2023, max compression
```

## Comparing `weatherly-0.4.0.tar` & `weatherly-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-04-30 20:28:02.519968 weatherly-0.4.0/
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     1076 2023-04-14 20:22:17.000000 weatherly-0.4.0/LICENSE
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     2979 2023-04-30 20:28:02.519968 weatherly-0.4.0/PKG-INFO
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     1912 2023-04-24 19:20:20.000000 weatherly-0.4.0/README.rst
--rw-rw-r--   0 konrad    (1000) konrad    (1000)       38 2023-04-30 20:28:02.519968 weatherly-0.4.0/setup.cfg
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     1919 2023-04-27 19:25:17.000000 weatherly-0.4.0/setup.py
-drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-04-30 20:28:02.503968 weatherly-0.4.0/weatherly/
--rw-rw-r--   0 konrad    (1000) konrad    (1000)      783 2023-04-25 20:17:26.000000 weatherly-0.4.0/weatherly/__init__.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)    15185 2023-04-24 19:44:41.000000 weatherly-0.4.0/weatherly/abc.py
-drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-04-30 20:28:02.519968 weatherly-0.4.0/weatherly/api/
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     1228 2023-04-16 19:16:10.000000 weatherly-0.4.0/weatherly/api/__init__.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)    16310 2023-04-25 20:14:50.000000 weatherly-0.4.0/weatherly/api/client.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     2657 2023-04-23 19:24:58.000000 weatherly-0.4.0/weatherly/api/core.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     4488 2023-04-16 21:05:46.000000 weatherly-0.4.0/weatherly/enums.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     3886 2023-04-25 19:59:06.000000 weatherly-0.4.0/weatherly/errors.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)    22175 2023-04-25 19:39:43.000000 weatherly-0.4.0/weatherly/responses.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     2798 2023-04-27 19:47:53.000000 weatherly-0.4.0/weatherly/utils.py
-drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-04-30 20:28:02.515968 weatherly-0.4.0/weatherly.egg-info/
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     2979 2023-04-30 20:28:02.000000 weatherly-0.4.0/weatherly.egg-info/PKG-INFO
--rw-rw-r--   0 konrad    (1000) konrad    (1000)      383 2023-04-30 20:28:02.000000 weatherly-0.4.0/weatherly.egg-info/SOURCES.txt
--rw-rw-r--   0 konrad    (1000) konrad    (1000)        1 2023-04-30 20:28:02.000000 weatherly-0.4.0/weatherly.egg-info/dependency_links.txt
--rw-rw-r--   0 konrad    (1000) konrad    (1000)       90 2023-04-30 20:28:02.000000 weatherly-0.4.0/weatherly.egg-info/requires.txt
--rw-rw-r--   0 konrad    (1000) konrad    (1000)       10 2023-04-30 20:28:02.000000 weatherly-0.4.0/weatherly.egg-info/top_level.txt
+drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-04-30 21:53:06.542178 weatherly-0.5.0/
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     1076 2023-04-14 20:22:17.000000 weatherly-0.5.0/LICENSE
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     2996 2023-04-30 21:53:06.542178 weatherly-0.5.0/PKG-INFO
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     1929 2023-04-30 21:48:52.000000 weatherly-0.5.0/README.rst
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)       38 2023-04-30 21:53:06.542178 weatherly-0.5.0/setup.cfg
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     1919 2023-04-27 19:25:17.000000 weatherly-0.5.0/setup.py
+drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-04-30 21:53:06.534179 weatherly-0.5.0/weatherly/
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)      783 2023-04-30 21:49:20.000000 weatherly-0.5.0/weatherly/__init__.py
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)    21660 2023-04-30 21:31:00.000000 weatherly-0.5.0/weatherly/abc.py
+drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-04-30 21:53:06.542178 weatherly-0.5.0/weatherly/api/
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     1227 2023-04-30 21:49:39.000000 weatherly-0.5.0/weatherly/api/__init__.py
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)    19278 2023-04-30 21:37:57.000000 weatherly-0.5.0/weatherly/api/client.py
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     2657 2023-04-23 19:24:58.000000 weatherly-0.5.0/weatherly/api/core.py
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     4488 2023-04-16 21:05:46.000000 weatherly-0.5.0/weatherly/enums.py
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     3905 2023-04-30 21:01:53.000000 weatherly-0.5.0/weatherly/errors.py
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)    31591 2023-04-30 21:45:33.000000 weatherly-0.5.0/weatherly/responses.py
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     2798 2023-04-27 19:47:53.000000 weatherly-0.5.0/weatherly/utils.py
+drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-04-30 21:53:06.538179 weatherly-0.5.0/weatherly.egg-info/
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)     2996 2023-04-30 21:53:06.000000 weatherly-0.5.0/weatherly.egg-info/PKG-INFO
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)      383 2023-04-30 21:53:06.000000 weatherly-0.5.0/weatherly.egg-info/SOURCES.txt
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)        1 2023-04-30 21:53:06.000000 weatherly-0.5.0/weatherly.egg-info/dependency_links.txt
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)       90 2023-04-30 21:53:06.000000 weatherly-0.5.0/weatherly.egg-info/requires.txt
+-rw-rw-r--   0 konrad    (1000) konrad    (1000)       10 2023-04-30 21:53:06.000000 weatherly-0.5.0/weatherly.egg-info/top_level.txt
```

### Comparing `weatherly-0.4.0/LICENSE` & `weatherly-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `weatherly-0.4.0/PKG-INFO` & `weatherly-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weatherly
-Version: 0.4.0
+Version: 0.5.0
 Summary: A simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more...
 Home-page: https://github.com/konradsic/weatherly
 Author: konradsic
 License: MIT
 Project-URL: Issues, https://github.com/konradsic/weatherly/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
@@ -39,23 +39,23 @@
     :alt: Supported Python versions
 .. image:: https://img.shields.io/github/actions/workflow/status/konradsic/weatherly/build.yml?style=for-the-badge
     :target: https://github.com/konradsic/weatherly
     :alt: Build status
 
 Weatherly is a simple package that retrieves weather data from WeatherAPI.com. It provides an easy to use interface to access current and historical weather data for a specific location.
 
-📜 Features
+Features
 ---------------
 * Easy to use,
 * Intuitive design,
 * Can provide current weather data aswell as forecast, historical data, future predictions and even more!
 * Modern and typed Python package,
 * Support for languages (provided by WeatherAPI)
 
-💻 Code example
+Code example
 ---------------------
 
 .. code:: python
 
     import weatherly
     
     client = weatherly.Client(api_key="your WeatherAPI key")
@@ -63,16 +63,16 @@
     client.set_language("fr")     # lang code
     client.set_language("German") # language full name
 
     # getting weather info
     current_weather = client.get_current_weather(query="London")
 
     # getting forecast info
-    forecast = client.get_forecast_data(query="Paris")
+    forecast = client.get_forecast_data(query="Paris", days=3)
 
     # historical data
-    history = client.get_historical_data(query="48.8567,2.3508") # query could also be latitude,longitude
+    history = client.get_historical_data(query="48.8567,2.3508", date="2010-01-01") # query could also be latitude,longitude
 
     # marine data
     marine = client.get_marine_data(query="Madrid")
```

### Comparing `weatherly-0.4.0/README.rst` & `weatherly-0.5.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,23 @@
     :alt: Supported Python versions
 .. image:: https://img.shields.io/github/actions/workflow/status/konradsic/weatherly/build.yml?style=for-the-badge
     :target: https://github.com/konradsic/weatherly
     :alt: Build status
 
 Weatherly is a simple package that retrieves weather data from WeatherAPI.com. It provides an easy to use interface to access current and historical weather data for a specific location.
 
-📜 Features
+Features
 ---------------
 * Easy to use,
 * Intuitive design,
 * Can provide current weather data aswell as forecast, historical data, future predictions and even more!
 * Modern and typed Python package,
 * Support for languages (provided by WeatherAPI)
 
-💻 Code example
+Code example
 ---------------------
 
 .. code:: python
 
     import weatherly
     
     client = weatherly.Client(api_key="your WeatherAPI key")
@@ -35,14 +35,14 @@
     client.set_language("fr")     # lang code
     client.set_language("German") # language full name
 
     # getting weather info
     current_weather = client.get_current_weather(query="London")
 
     # getting forecast info
-    forecast = client.get_forecast_data(query="Paris")
+    forecast = client.get_forecast_data(query="Paris", days=3)
 
     # historical data
-    history = client.get_historical_data(query="48.8567,2.3508") # query could also be latitude,longitude
+    history = client.get_historical_data(query="48.8567,2.3508", date="2010-01-01") # query could also be latitude,longitude
 
     # marine data
     marine = client.get_marine_data(query="Madrid")
```

### Comparing `weatherly-0.4.0/setup.py` & `weatherly-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `weatherly-0.4.0/weatherly/__init__.py` & `weatherly-0.5.0/weatherly/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 :license: MIT license, see LICENSE for details
 """
 
 __title__ = 'weatherly'
 __author__ = 'konradsic'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023-present konradsic'
-__version__ = '0.4.0'
+__version__ = '0.5.0'
 
 from typing import NamedTuple, Literal
 
 from .api import *
 from .errors import *
 from .enums import *
 from .responses import *
@@ -25,10 +25,10 @@
 
 class VersionInfo(NamedTuple):
     major: int
     minor: int
     micro: int
     release_type: Literal["alpha", "beta", "candidate", "final"]
     
-version_info = VersionInfo(major=0, minor=4, micro=0, release_type="final")
+version_info = VersionInfo(major=0, minor=5, micro=0, release_type="final")
 
 del NamedTuple, Literal, VersionInfo
```

### Comparing `weatherly-0.4.0/weatherly/abc.py` & `weatherly-0.5.0/weatherly/abc.py`

 * *Files 16% similar despite different names*

```diff
@@ -507,8 +507,240 @@
     forecast_days: List[:class:`ForecastDayModel`]
         A list of forecast days
     alerts: List[:class:`AlertModel`]
         A list of alerts, this list can be empty
     """
     location: LocationModel
     forecast_days: List[ForecastDayModel]
-    alerts: List[AlertModel]
+    alerts: List[AlertModel]
+
+class FutureHourModel(ResponseModel):
+    """
+    An ABC defining a base future hour model from WeatherAPI
+
+    The following classes implement this ABC:
+    - :class:`~weatherly.FutureHour`
+
+    Attributes
+    -------------
+    time_epoch: :class:`int`
+        Time as epoch
+    time: :class:`str`
+        Date and time
+    temp_c: :class:`float`
+        Temperature in celsius
+    temp_f: :class:`float`
+        Temperature in fahrenheit
+    condition_text: :class:`str`
+        Weather condition text
+    condition_icon: :class:`str`
+        Weather condition icons
+    condition_code: :class:`int`
+        Weather condition code
+    wind_mph: :class:`float`
+        Maximum wind speed in miles per hour
+    wind_kph: :class:`float`
+        Maximum wind speed in kilometer per hour
+    wind_degree: :class:`int`
+        Wind direction in degrees
+    wind_dir: :class:`str`
+        Wind direction as 16 point compass. e.g.: NSW
+    pressure_mb: :class:`float`
+        Pressure in millibars
+    pressure_in: :class:`float`
+        Pressure in inches
+    precip_mm: :class:`float`
+        Precipitation amount in millimeters
+    precip_in: :class:`float`
+        Precipitation amount in inches
+    humidity: :class:`int`
+        Humidity as percentage
+    cloud: :class:`int`
+        Cloud cover as percentage
+    feelslike_c: :class:`float`
+        Feels like temperature as celcius
+    feelslike_f: :class:`float`
+        Feels like temperature as fahrenheit
+    windchill_c: :class:`float`
+        Windchill temperature in celcius
+    windchill_f: :class:`float`
+        Windchill temperature in fahrenheit
+    headindex_c: :class:`float`
+        Heat index in celcius
+    headindex_f: :class:`float`
+        Heat index in fahrenheit
+    dewpoint_c: :class:`float`
+        Dew point in celcius
+    dewpoint_f: :class:`float`
+        Dew point in fahrenheit
+    will_it_rain: :class:`bool`
+        Will it will rain or not
+    will_it_snow: :class:`bool`
+        Will it will snow or not
+    is_day: :class:`bool`
+        Whether to show day condition icon or night icon
+    vis_km: :class:`float`
+        Visibility in kilometer
+    vis_miles: :class:`float`
+        Visibility in miles
+    chance_of_rain: :class:`int`
+        Chance of rain as percentage
+    chance_of_snow: :class:`int`
+        Chance of snow as percentage
+    gust_mph: :class:`float`
+        Wind gust in miles per hour
+    gust_kph: :class:`float`
+        Wind gust in kilometer per hour
+    """
+    time_epoch: int
+    time: str
+    temp_c: float
+    temp_f: float
+    condition_text: str
+    condition_icon: str
+    condition_code: int
+    wind_mph: float
+    wind_kph: float
+    wind_degree: int
+    wind_dir: str
+    pressure_mb: float
+    pressure_in: float
+    precip_mm: float
+    precip_in: float
+    humidity: int
+    cloud: int
+    feelslike_c: float
+    feelslike_f: float
+    windchill_c: float
+    windchill_f: float
+    headindex_c: float
+    headindex_f: float
+    dewpoint_c: float
+    dewpoint_f: float
+    will_it_rain: bool
+    will_it_snow: bool
+    is_day: bool
+    vis_km: float
+    vis_miles: float
+    chance_of_rain: int
+    chance_of_snow: int
+    gust_mph: float
+    gust_kph: float
+    
+
+class FutureDayModel(ResponseModel):
+    """
+    An ABC defining a base future day model from WeatherAPI
+
+    The following classes implement this ABC:
+    - :class:`~weatherly.FutureDay`
+
+    Attributes
+    -------------
+    date: :class:`str`
+        Future date
+    date_epoch: :class:`int`
+        Future date as unix time.
+    maxtemp_c: :class:`float`
+        Maximum temperature in celsius for the day.
+    maxtemp_f: :class:`float`
+        Maximum temperature in fahrenheit for the day
+    mintemp_c: :class:`float`
+        Minimum temperature in celsius for the day
+    mintemp_f: :class:`float`
+        Minimum temperature in fahrenheit for the day
+    avgtemp_c: :class:`float`
+        Average temperature in celsius for the day
+    avgtemp_f: :class:`float`
+        Average temperature in fahrenheit for the day
+    maxwind_mph: :class:`float`
+        Maximum wind speed in miles per hour
+    maxwind_mph: :class:`float`
+        Maximum wind speed in kilometer per hour
+    totalprecip_mm: :class:`float`
+        Total precipitation in milimeter
+    totalprecip_in: :class:`float`
+        Total precipitation in inches
+    avgvis_km: :class:`float`
+        Average visibility in kilometer
+    avgvis_miles: :class:`float`
+        Average visibility in miles
+    avghumidity: :class:`int`
+        Average humidity as percentage
+    condition_text: :class:`str`
+        Weather condition text
+    condition_icon: :class:`str`
+        Weather condition icon
+    condition_code: :class:`int`
+        Weather condition code
+    hour_data: List[:class:`FutureHourModel`]
+        A list of :class:`FutureHourModel` objects representing hourly weather data.
+    sunrise: :class:`str`
+        Sunrise time
+    sunset: :class:`str`
+        Sunset time
+    moonrise: :class:`str`
+        Moonrise time
+    moonset: :class:`str`
+        Moonset time
+    moon_phase: :class:`str`
+        Moon phases. Value returned:
+        * New Moon
+        * Waxing Crescent
+        * First Quarter
+        * Waxing Gibbous
+        * Full Moon
+        * Waning Gibbous
+        * Last Quarter
+        * Waning Crescent
+    moon_illumination: :class:`float`
+        Moon illumination as %
+    """
+    date: str
+    date_epoch: int
+    # day
+    maxtemp_c: float
+    maxtemp_f: float
+    mintemp_c: float
+    mintemp_f: float
+    avgtemp_c: float
+    avgtemp_f: float
+
+    maxwind_mph: float
+    maxwind_mph: float
+
+    totalprecip_mm: float
+    totalprecip_in: float
+
+    avgvis_km: float
+    avgvis_miles: float
+    avghumidity: int
+
+    condition_text: str
+    condition_icon: str
+    condition_code: int
+    # astro data
+    sunrise: Optional[str]
+    sunset: Optional[str]
+    moonrise: Optional[str]
+    moonset: Optional[str]
+    moon_phase: Optional[str]
+    moon_illumination: Optional[float]
+
+    hour_data: List[FutureHourModel]
+
+class FutureModel(ResponseModel):
+    """
+    An ABC defining a base response from Future API. Similiar to :class:`weatherly.ForecastModel`
+
+    The following classes implement this ABC:
+    - :class:`~weatherly.FutureData`
+    
+    Attributes
+    -------------
+    location: :class:`LocationModel`
+        Location of the forecast data.
+    forecast_days: :class:`FutureDayModel`
+        Day data
+    """
+    location: LocationModel
+    day: FutureDayModel
```

### Comparing `weatherly-0.4.0/weatherly/api/__init__.py` & `weatherly-0.5.0/weatherly/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 weatherly/api
 --------------
-An package extension to weatherly providing access to WeatherAPI (requests, client, etc.)
+A package extension to weatherly providing access to WeatherAPI (requests, client, etc.)
 
 
 MIT License
 
 Copyright (c) 2023 Konrad (@konradsic)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `weatherly-0.4.0/weatherly/api/client.py` & `weatherly-0.5.0/weatherly/api/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from typing import Any, Dict, List, Literal, Optional, Union
 
 from .. import utils as utils
 from ..enums import Languages
 from ..errors import (AccessDenied, APIKeyDisabled, APILimitExceeded,
                       InternalApplicationError, InvalidAPIKey, InvalidDate,
                       NoLocationFound, WeatherAPIException)
-from ..responses import CurrentWeatherData, ForecastData, LocationData
+from ..responses import CurrentWeatherData, ForecastData, LocationData, FutureData
 from .core import BaseAPIClient
 
 WEATHERAPI_BASE_URL = "http://api.weatherapi.com/v1/"
 BOOL_REPLACE = {True: "yes", False: "no"}
 
 __all__ = (
     "Client",
@@ -399,14 +399,89 @@
         now = datetime.datetime.timestamp(datetime.datetime.utcnow())
 
         if epoch > now: raise InvalidDate("Date should be before current time, switch from History API to Future to use future dates.")
 
         resp = self._call_request("history.json", options)
         history = ForecastData(resp[0], resp[1].status_code, None)
         return history
+        
+    def get_future_data(
+        self,
+        query: str,
+        date: str,
+        *,
+        lang: Optional[Union[str, Languages]] = None,
+        **kwargs: Dict[str, Any]
+    ) -> FutureData:
+        """
+        Retrieve future data for given day and query. Uses Future API.
+
+        Parameters
+        -----------------
+        query: :class:`str`
+            Query string, location you want to get forecast data for
+        date: :class:`str`
+            A date string in format yyyy-mm-dd representing the day you want to get data for
+        lang: Optional[Union[:class`str`, :class`Languages`]]
+            Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
+            To get a list of languages visit :class:`Languages`.
+        kwargs: Dict[:class:`str`, Any]
+            Additional keyword arguments that will be passed to the request.
+        
+        Returns
+        ----------
+        :class:`FutureData`
+            Forecast data for given day and query.
+
+        Raises
+        ---------
+        :exc:`NoLocationFound`
+            Raised when no location for given query was found
+        :exc:`InvalidAPIKey`
+            Raised when the API key is invalid
+        :exc:`APILimitExceeded`
+            Raised when API key calls limit was exceeded
+        :exc:`APIKeyDisabled`
+            Raised when API key is disabled
+        :exc:`AccessDenied`
+            Raised when access to given resource was denied
+        :exc:`InternalApplicationError`
+            Raised when there was a very rare internal application error
+        :exc:`WeatherAPIException`
+            Raised when something else went wrong, that does not have a specific exception class.
+        :exc:`InvalidDate`
+            Raised when the ``date`` parameter is invalid (doesn't match the format or isn't a date after today)
+        """
+        options = {
+            "q": query,
+            "dt": date,
+            **kwargs
+        }
+        if lang is not None: options["lang"] = lang
+
+        # check if given date is really "historical"
+        try:
+            splitted = date.split("-")
+            datetuple = datetime.datetime(
+                int(splitted[0]), 
+                int(splitted[1][1:]) if splitted[1].startswith("0") else int(splitted[1]), 
+                int(splitted[2][1:]) if splitted[2].startswith("0") else int(splitted[2]),
+                0,0)
+            epoch = datetuple.timestamp()
+        except Exception as exc:
+            raise InvalidDate(f"Failed to convert date {date}: Invalid format") from exc
+
+        now = datetime.datetime.timestamp(datetime.datetime.utcnow())
+
+        if epoch < now: raise InvalidDate("Date should be after current time, switch from Future API to History to use past dates.")
+
+        resp = self._call_request("future.json", options)
+        future = FutureData(resp[0], resp[1].status_code, None)
+        return future
+        
     
     def __str__(self):
         return f"<{self.__class__.__name__} api_key={self.default_options['key']} lang={self.lang}>"
     
     def __repr__(self):
         return repr(self.__str__())
```

### Comparing `weatherly-0.4.0/weatherly/api/core.py` & `weatherly-0.5.0/weatherly/api/core.py`

 * *Files identical despite different names*

### Comparing `weatherly-0.4.0/weatherly/enums.py` & `weatherly-0.5.0/weatherly/enums.py`

 * *Files identical despite different names*

### Comparing `weatherly-0.4.0/weatherly/errors.py` & `weatherly-0.5.0/weatherly/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     "WeatherAPIException",
     "NoLocationFound",
     "InvalidAPIKey",
     "APILimitExceeded",
     "APIKeyDisabled",
     "AccessDenied",
     "InternalApplicationError",
+    "InvalidDate",
 )
 
 class WeatherlyException(Exception):
     """
     A base class for all ``weatherly`` exceptions. Almost all exceptions of this module inherit from this class.
 
     Inherits from :class:`Exception`.
```

### Comparing `weatherly-0.4.0/weatherly/responses.py` & `weatherly-0.5.0/weatherly/responses.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,14 +26,17 @@
     CurrentWeather, 
     LocationModel, 
     AirQuality, 
     ForecastDayModel, 
     ForecastHourModel, 
     ForecastModel,
     AlertModel,
+    FutureDayModel,
+    FutureHourModel,
+    FutureModel
 )
 from typing import (
     Dict,
     Any,
     Union,
     Optional,
     List, 
@@ -44,14 +47,17 @@
     "CurrentWeatherData",
     "LocationData",
     "AirQualityData",
     "ForecastData",
     "ForecastDay",
     "ForecastHour",
     "AlertData",
+    "FutureDay",
+    "FutureHour",
+    "FutureData",
 )
 
 
 GB_DEFRA_BAND = ("Low", "Low", "Low", "Moderate", "Moderate", "Moderate", "High", "High", "High", "Very High")
 
 class CurrentWeatherData(CurrentWeather):
     """
@@ -639,7 +645,277 @@
         Iterator[:class:`ForecastHour`]
             A generator object you can iterate over made of :class:`ForecastHour`
         """
 
         for day in self.forecast_days:
             for hour in day.hour_data:
                 yield hour
+
+class FutureHour(FutureHourModel):
+    """
+    Future hour, an element of :class:`FutureDay`
+    
+    Attributes
+    -------------
+    raw: Dict[:class:`str`, Any]
+        Raw response in a JSON-like format (converted to a python dictionary)
+    status: :class:`int`
+        HTTP status of the response. 200 is OK, and is the most common status.
+    code: Optional[:class:`int`]
+        Response code. In some cases this can be ``None``
+    time_epoch: :class:`int`
+        Time as epoch
+    time: :class:`str`
+        Date and time
+    temp_c: :class:`float`
+        Temperature in celsius
+    temp_f: :class:`float`
+        Temperature in fahrenheit
+    condition_text: :class:`str`
+        Weather condition text
+    condition_icon: :class:`str`
+        Weather condition icons
+    condition_code: :class:`int`
+        Weather condition code
+    wind_mph: :class:`float`
+        Maximum wind speed in miles per hour
+    wind_kph: :class:`float`
+        Maximum wind speed in kilometer per hour
+    wind_degree: :class:`int`
+        Wind direction in degrees
+    wind_dir: :class:`str`
+        Wind direction as 16 point compass. e.g.: NSW
+    pressure_mb: :class:`float`
+        Pressure in millibars
+    pressure_in: :class:`float`
+        Pressure in inches
+    precip_mm: :class:`float`
+        Precipitation amount in millimeters
+    precip_in: :class:`float`
+        Precipitation amount in inches
+    humidity: :class:`int`
+        Humidity as percentage
+    cloud: :class:`int`
+        Cloud cover as percentage
+    feelslike_c: :class:`float`
+        Feels like temperature as celcius
+    feelslike_f: :class:`float`
+        Feels like temperature as fahrenheit
+    windchill_c: :class:`float`
+        Windchill temperature in celcius
+    windchill_f: :class:`float`
+        Windchill temperature in fahrenheit
+    headindex_c: :class:`float`
+        Heat index in celcius
+    headindex_f: :class:`float`
+        Heat index in fahrenheit
+    dewpoint_c: :class:`float`
+        Dew point in celcius
+    dewpoint_f: :class:`float`
+        Dew point in fahrenheit
+    will_it_rain: :class:`bool`
+        Will it will rain or not
+    will_it_snow: :class:`bool`
+        Will it will snow or not
+    is_day: :class:`bool`
+        Whether to show day condition icon or night icon
+    vis_km: :class:`float`
+        Visibility in kilometer
+    vis_miles: :class:`float`
+        Visibility in miles
+    chance_of_rain: :class:`int`
+        Chance of rain as percentage
+    chance_of_snow: :class:`int`
+        Chance of snow as percentage
+    gust_mph: :class:`float`
+        Wind gust in miles per hour
+    gust_kph: :class:`float`
+        Wind gust in kilometer per hour
+    """
+    def __init__(
+        self,
+        raw: Dict[str, Any],
+        status: int,
+        code: Optional[int]
+    ) -> None:
+        self.raw = raw
+        self.status = status
+        self.code = code
+
+        self.time_epoch = raw["time_epoch"]
+        self.time = raw["time"]
+        self.temp_c = raw["temp_c"]
+        self.temp_f = raw["temp_f"]
+        self.condition_text = raw["condition"]["text"]
+        self.condition_icon = raw["condition"]["icon"]
+        self.condition_code = raw["condition"]["code"]
+        self.wind_mph = raw["wind_mph"]
+        self.wind_kph = raw["wind_kph"]
+        self.wind_degree = raw["wind_degree"]
+        self.wind_dir = raw["wind_dir"]
+        self.pressure_mb = raw["pressure_mb"]
+        self.pressure_in = raw["pressure_in"]
+        self.precip_mm = raw["precip_mm"]
+        self.precip_in = raw["precip_in"]
+        self.humidity = raw["humidity"]
+        self.cloud = raw["cloud"]
+        self.feelslike_c = raw["feelslike_c"]
+        self.feelslike_f = raw["feelslike_f"]
+        self.windchill_c = raw["windchill_c"]
+        self.windchill_f = raw["windchill_f"]
+        self.heatindex_c = raw["heatindex_c"]
+        self.heatindex_f = raw["heatindex_f"]
+        self.dewpoint_c = raw["dewpoint_c"]
+        self.dewpoint_f = raw["dewpoint_f"]
+        self.will_it_rain = bool(raw["will_it_rain"])
+        self.will_it_snow = bool(raw["will_it_snow"])
+        self.is_day = bool(raw["is_day"])
+        self.vis_km = raw["vis_km"]
+        self.vis_miles = raw["vis_miles"]
+        self.chance_of_rain = raw["chance_of_rain"]
+        self.chance_of_snow = raw["chance_of_snow"]
+        self.gust_mph = raw["gust_mph"]
+        self.gust_kph = raw["gust_kph"]
+
+class FutureDay(FutureDayModel):
+    """
+    A future day, element of :class:`FutureData`
+
+    Attributes
+    -------------
+    raw: Dict[:class:`str`, Any]
+        Raw response in a JSON-like format (converted to a python dictionary)
+    status: :class:`int`
+        HTTP status of the response. 200 is OK, and is the most common status.
+    code: Optional[:class:`int`]
+        Response code. In some cases this can be ``None``
+    date: :class:`str`
+        Forecast date
+    date_epoch: :class:`int`
+        Forecast date as unix time.
+    maxtemp_c: :class:`float`
+        Maximum temperature in celsius for the day.
+    maxtemp_f: :class:`float`
+        Maximum temperature in fahrenheit for the day
+    mintemp_c: :class:`float`
+        Minimum temperature in celsius for the day
+    mintemp_f: :class:`float`
+        Minimum temperature in fahrenheit for the day
+    avgtemp_c: :class:`float`
+        Average temperature in celsius for the day
+    avgtemp_f: :class:`float`
+        Average temperature in fahrenheit for the day
+    maxwind_mph: :class:`float`
+        Maximum wind speed in miles per hour
+    maxwind_kph: :class:`float`
+        Maximum wind speed in kilometer per hour
+    totalprecip_mm: :class:`float`
+        Total precipitation in milimeter
+    totalprecip_in: :class:`float`
+        Total precipitation in inches
+    avgvis_km: :class:`float`
+        Average visibility in kilometer
+    avgvis_miles: :class:`float`
+        Average visibility in miles
+    avghumidity: :class:`int`
+        Average humidity as percentage
+    condition_text: :class:`str`
+        Weather condition text
+    condition_icon: :class:`str`
+        Weather condition icon
+    condition_code: :class:`int`
+        Weather condition code
+    hour_data: List[:class:`FutureHour`]
+        A list of :class:`FutureHour` objects representing hourly weather data.
+    sunrise: :class:`str`
+        Sunrise time
+    sunset: :class:`str`
+        Sunset time
+    moonrise: :class:`str`
+        Moonrise time
+    moonset: :class:`str`
+        Moonset time
+    moon_phase: :class:`str`
+        Moon phases. Value returned:
+            * New Moon
+            * Waxing Crescent
+            * First Quarter
+            * Waxing Gibbous
+            * Full Moon
+            * Waning Gibbous
+            * Last Quarter
+            * Waning Crescent
+    moon_illumination: :class:`float`
+        Moon illumination as %
+    """
+    def __init__(
+        self,
+        raw: Dict[str, Any],
+        status: int,
+        code: Optional[int]
+    ) -> None:
+        self.raw = raw
+        self.status = status
+        self.code = code
+        self.date = raw["date"]
+        self.date_epoch = raw["date_epoch"]
+        
+        before_raw = raw.copy()
+        raw = raw["day"]
+        
+        self.maxtemp_c = raw["maxtemp_c"]
+        self.maxtemp_f = raw["maxtemp_f"]
+        self.mintemp_c = raw["mintemp_c"]
+        self.mintemp_f = raw["mintemp_f"]
+        self.avgtemp_c = raw["avgtemp_c"]
+        self.avgtemp_f = raw["avgtemp_f"]
+        self.maxwind_mph = raw["maxwind_mph"]
+        self.maxwind_kph = raw["maxwind_kph"]
+        self.totalprecip_in = raw["totalprecip_in"]
+        self.totalprecip_mm = raw["totalprecip_mm"]
+        self.avgvis_km = raw["avgvis_km"]
+        self.avgvis_miles = raw["avgvis_miles"]
+        self.avghumidity = raw["avghumidity"]
+        self.condition_text = raw["condition"]["text"]
+        self.condition_icon = raw["condition"]["icon"]
+        self.condition_code = raw["condition"]["code"]
+        
+        raw = before_raw
+        self.hour_data = list([
+            FutureHour(elem, status, code) for elem in raw["hour"]
+        ])
+        self.sunrise = raw["astro"]["sunrise"]
+        self.sunset = raw["astro"]["sunset"]
+        self.moonrise = raw["astro"]["moonrise"]
+        self.moonset = raw["astro"]["moonset"]
+        self.moon_phase = raw["astro"]["moon_phase"]
+        self.moon_illumination = raw["astro"]["moon_illumination"]
+
+class FutureData(FutureModel):
+    """
+    Forecast data returned from Future API
+    
+    Attributes
+    -------------
+    raw: Dict[:class:`str`, Any]
+        Raw response in a JSON-like format (converted to a python dictionary)
+    status: :class:`int`
+        HTTP status of the response. 200 is OK, and is the most common status.
+    code: Optional[:class:`int`]
+        Response code. In some cases this can be ``None``
+    location: :class:`LocationData`
+        Location of the forecast data.
+    day: :class:`FutureDay`
+        Day data for the requested future date.
+    """
+    def __init__(
+        self,
+        raw: Dict[str, Any],
+        status: int,
+        code: Optional[int]
+    ) -> None:
+        self.raw = raw
+        self.status = status
+        self.code = code
+        
+        self.location = LocationData(raw["location"], status, code)
+        self.day = FutureDay(raw["forecast"]["forecastday"][0], status, code)
```

### Comparing `weatherly-0.4.0/weatherly/utils.py` & `weatherly-0.5.0/weatherly/utils.py`

 * *Files identical despite different names*

### Comparing `weatherly-0.4.0/weatherly.egg-info/PKG-INFO` & `weatherly-0.5.0/weatherly.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weatherly
-Version: 0.4.0
+Version: 0.5.0
 Summary: A simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more...
 Home-page: https://github.com/konradsic/weatherly
 Author: konradsic
 License: MIT
 Project-URL: Issues, https://github.com/konradsic/weatherly/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
@@ -39,23 +39,23 @@
     :alt: Supported Python versions
 .. image:: https://img.shields.io/github/actions/workflow/status/konradsic/weatherly/build.yml?style=for-the-badge
     :target: https://github.com/konradsic/weatherly
     :alt: Build status
 
 Weatherly is a simple package that retrieves weather data from WeatherAPI.com. It provides an easy to use interface to access current and historical weather data for a specific location.
 
-📜 Features
+Features
 ---------------
 * Easy to use,
 * Intuitive design,
 * Can provide current weather data aswell as forecast, historical data, future predictions and even more!
 * Modern and typed Python package,
 * Support for languages (provided by WeatherAPI)
 
-💻 Code example
+Code example
 ---------------------
 
 .. code:: python
 
     import weatherly
     
     client = weatherly.Client(api_key="your WeatherAPI key")
@@ -63,16 +63,16 @@
     client.set_language("fr")     # lang code
     client.set_language("German") # language full name
 
     # getting weather info
     current_weather = client.get_current_weather(query="London")
 
     # getting forecast info
-    forecast = client.get_forecast_data(query="Paris")
+    forecast = client.get_forecast_data(query="Paris", days=3)
 
     # historical data
-    history = client.get_historical_data(query="48.8567,2.3508") # query could also be latitude,longitude
+    history = client.get_historical_data(query="48.8567,2.3508", date="2010-01-01") # query could also be latitude,longitude
 
     # marine data
     marine = client.get_marine_data(query="Madrid")
```

