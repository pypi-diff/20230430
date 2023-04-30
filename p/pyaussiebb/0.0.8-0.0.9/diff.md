# Comparing `tmp/pyaussiebb-0.0.8.tar.gz` & `tmp/pyaussiebb-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaussiebb-0.0.8.tar", last modified: Fri Aug 27 05:12:42 2021, max compression
+gzip compressed data, was "pyaussiebb-0.0.9.tar", last modified: Sat Aug 28 06:57:56 2021, max compression
```

## Comparing `pyaussiebb-0.0.8.tar` & `pyaussiebb-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yaleman    (501) staff       (20)        0 2021-08-27 05:12:42.481174 pyaussiebb-0.0.8/
--rw-r--r--   0 yaleman    (501) staff       (20)     8015 2021-08-27 05:12:42.481048 pyaussiebb-0.0.8/PKG-INFO
--rw-r--r--   0 yaleman    (501) staff       (20)     7478 2021-08-27 05:11:41.000000 pyaussiebb-0.0.8/README.md
-drwxr-xr-x   0 yaleman    (501) staff       (20)        0 2021-08-27 05:12:42.480143 pyaussiebb-0.0.8/aussiebb/
--rw-r--r--   0 yaleman    (501) staff       (20)    13988 2021-08-27 05:11:41.000000 pyaussiebb-0.0.8/aussiebb/__init__.py
-drwxr-xr-x   0 yaleman    (501) staff       (20)        0 2021-08-27 05:12:42.480256 pyaussiebb-0.0.8/aussiebb/asyncio/
--rw-r--r--   0 yaleman    (501) staff       (20)    20237 2021-08-27 05:11:41.000000 pyaussiebb-0.0.8/aussiebb/asyncio/__init__.py
--rw-r--r--   0 yaleman    (501) staff       (20)     1733 2021-08-27 05:11:41.000000 pyaussiebb-0.0.8/aussiebb/const.py
--rw-r--r--   0 yaleman    (501) staff       (20)      399 2021-08-21 07:50:56.000000 pyaussiebb-0.0.8/aussiebb/exceptions.py
--rw-r--r--   0 yaleman    (501) staff       (20)      364 2021-08-27 05:11:41.000000 pyaussiebb-0.0.8/aussiebb/utils.py
-drwxr-xr-x   0 yaleman    (501) staff       (20)        0 2021-08-27 05:12:42.480894 pyaussiebb-0.0.8/pyaussiebb.egg-info/
--rw-r--r--   0 yaleman    (501) staff       (20)     8015 2021-08-27 05:12:42.000000 pyaussiebb-0.0.8/pyaussiebb.egg-info/PKG-INFO
--rw-r--r--   0 yaleman    (501) staff       (20)      296 2021-08-27 05:12:42.000000 pyaussiebb-0.0.8/pyaussiebb.egg-info/SOURCES.txt
--rw-r--r--   0 yaleman    (501) staff       (20)        1 2021-08-27 05:12:42.000000 pyaussiebb-0.0.8/pyaussiebb.egg-info/dependency_links.txt
--rw-r--r--   0 yaleman    (501) staff       (20)       16 2021-08-27 05:12:42.000000 pyaussiebb-0.0.8/pyaussiebb.egg-info/requires.txt
--rw-r--r--   0 yaleman    (501) staff       (20)        9 2021-08-27 05:12:42.000000 pyaussiebb-0.0.8/pyaussiebb.egg-info/top_level.txt
--rw-r--r--   0 yaleman    (501) staff       (20)       38 2021-08-27 05:12:42.481208 pyaussiebb-0.0.8/setup.cfg
--rw-r--r--   0 yaleman    (501) staff       (20)      826 2021-08-27 05:11:41.000000 pyaussiebb-0.0.8/setup.py
+drwxr-xr-x   0 yaleman    (501) staff       (20)        0 2021-08-28 06:57:56.181794 pyaussiebb-0.0.9/
+-rw-r--r--   0 yaleman    (501) staff       (20)     7787 2021-08-28 06:57:56.181672 pyaussiebb-0.0.9/PKG-INFO
+-rw-r--r--   0 yaleman    (501) staff       (20)     7250 2021-08-28 06:55:58.000000 pyaussiebb-0.0.9/README.md
+drwxr-xr-x   0 yaleman    (501) staff       (20)        0 2021-08-28 06:57:56.180518 pyaussiebb-0.0.9/aussiebb/
+-rw-r--r--   0 yaleman    (501) staff       (20)    16560 2021-08-28 06:55:58.000000 pyaussiebb-0.0.9/aussiebb/__init__.py
+drwxr-xr-x   0 yaleman    (501) staff       (20)        0 2021-08-28 06:57:56.180743 pyaussiebb-0.0.9/aussiebb/asyncio/
+-rw-r--r--   0 yaleman    (501) staff       (20)    22219 2021-08-28 06:32:04.000000 pyaussiebb-0.0.9/aussiebb/asyncio/__init__.py
+-rw-r--r--   0 yaleman    (501) staff       (20)     1733 2021-08-28 06:55:58.000000 pyaussiebb-0.0.9/aussiebb/const.py
+-rw-r--r--   0 yaleman    (501) staff       (20)      399 2021-08-21 07:50:56.000000 pyaussiebb-0.0.9/aussiebb/exceptions.py
+-rw-r--r--   0 yaleman    (501) staff       (20)      364 2021-08-27 05:11:41.000000 pyaussiebb-0.0.9/aussiebb/utils.py
+drwxr-xr-x   0 yaleman    (501) staff       (20)        0 2021-08-28 06:57:56.181513 pyaussiebb-0.0.9/pyaussiebb.egg-info/
+-rw-r--r--   0 yaleman    (501) staff       (20)     7787 2021-08-28 06:57:56.000000 pyaussiebb-0.0.9/pyaussiebb.egg-info/PKG-INFO
+-rw-r--r--   0 yaleman    (501) staff       (20)      296 2021-08-28 06:57:56.000000 pyaussiebb-0.0.9/pyaussiebb.egg-info/SOURCES.txt
+-rw-r--r--   0 yaleman    (501) staff       (20)        1 2021-08-28 06:57:56.000000 pyaussiebb-0.0.9/pyaussiebb.egg-info/dependency_links.txt
+-rw-r--r--   0 yaleman    (501) staff       (20)       24 2021-08-28 06:57:56.000000 pyaussiebb-0.0.9/pyaussiebb.egg-info/requires.txt
+-rw-r--r--   0 yaleman    (501) staff       (20)        9 2021-08-28 06:57:56.000000 pyaussiebb-0.0.9/pyaussiebb.egg-info/top_level.txt
+-rw-r--r--   0 yaleman    (501) staff       (20)       38 2021-08-28 06:57:56.181828 pyaussiebb-0.0.9/setup.cfg
+-rw-r--r--   0 yaleman    (501) staff       (20)      837 2021-08-28 06:56:41.000000 pyaussiebb-0.0.9/setup.py
```

### Comparing `pyaussiebb-0.0.8/PKG-INFO` & `pyaussiebb-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaussiebb
-Version: 0.0.8
+Version: 0.0.9
 Summary: Aussie Broadband API module
 Home-page: https://github.com/yaleman/aussiebb
 Author: James Hodgkinson
 Author-email: yaleman@ricetek.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -30,49 +30,45 @@
 python
 >>> from aussiebb import AussieBB
 >>> account = AussieBB(username, password)
 >>> account.get_services()
 [{allyourservicedetails}]
 ```
 
-For more, check out the module.
-
-
+For more, check out the docs.
 
 # AsyncIO version
 
 You can replace `from aussiebb import AussieBB` with `from aussiebb.asyncio import AussieBB` and you'll get an `aiohttp`-powered version. The only difference in this case is that you have to explicitly call `login()` for reasons.
 
+If you hit the rate limit it'll raise a `RateLimit` exception. I haven't put that functionality into the blocking version yet, since ... that tends not to hit it. 🤣
 
-# AsyncIO version
+# Development
 
-You can replace `from aussiebb import AussieBB` with `from aussiebb.asyncio import AussieBB` and you'll get an `aiohttp`-powered version. The only difference in this case is that you have to explicitly call `login()` for reasons.
 
-If you hit the rate limit it'll raise a `RateLimit` exception. I haven't put that functionality into the blocking version yet, since ... that tends not to hit it. 🤣
-
-# Example service tests I've seen
+## Example service tests I've seen
 
-All the "endpoints" should be tacked onto `aussiebb.BASEURL['api']`.
+All the "endpoints" below should be tacked onto `aussiebb.BASEURL['api']`.
 
-**Warning: `/nbn/{service_id}/connection` seems to have both a GET and POST method endpoint - tests on other endpoints may be similar.**
+**Warning:** `/nbn/{service_id}/connection` seems to have both a GET and POST method endpoint - tests on other endpoints may be similar.
 
 These can be run by using `AussieBB.run_test()` with the string after the last forward-slash as the "test" - ie, `connection` or `linestate`.
 
-## HFC 
+### HFC 
 
 These are entirely untested so far.
 
 | Endpoint | Method | Name | Description |
 | --- | --- | --- | --- |
 | `/nbn/{service_id}/connection` | Probably GET | Check Connection | Check to see if your service is currently connected |
 | `/nbn/{service_id}/connection` | Probably POST | Kick Connection | Kick your current session and force your device to reauthenticate |
 | `/tests/{service_id}/loopback` | Probably POST | Loopback Test | This will test the connectivity between the point NBN’s network transitions to ours and to the closest point to your property. Usually either the Network Termination Device or Node. |
 | `/tests/{service_id}/ntdstatus` | Probably POST | NTD Status | An NTD Status will show you the operational state of the Network Termination Device (NTD). The test will also show if the NTD is detecting the wired connection from your router. |
 
-## FTTC
+### FTTC
 
 | Endpoint | Method | Name | Description |
 | --- | --- | --- | --- |
 | `/nbn/{service_id}/connection` | GET |Check Connection | Check to see if your service is currently connected |
 | `/nbn/{service_id}/connection`  | Probably POST |Kick Connection | Kick your current session and force your device to reauthenticate |
 | `/tests/{service_id}/dpuportreset` | Probably POST |DPU Port Reset | Reset the Port on the DPU (Distribution Point Unit) along with clearing any errors that maybe causing issues with connectivity.  |
 | `/tests/{service_id}/dpuportstatus` | POST |DPU Port Status | A DPU (Distribution Point Unit) port status will show if the NCD (Network Connection Device) is providing power to the DPU. It will also state if the NCD (Network Connection Device) is in sync. |
@@ -117,7 +113,9 @@
     - added telephony_usage
     - added get_appointment which gets service appointments
     - updated get_usage so it checks the service list and will return telephony data if it's a PhoneMobile service
     - abstracted how URLS are generated so I don't have to keep adding them twice
     - added a filter on get_services which allows you to filter by type
 
 
+
+
```

### Comparing `pyaussiebb-0.0.8/README.md` & `pyaussiebb-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -13,49 +13,45 @@
 python
 >>> from aussiebb import AussieBB
 >>> account = AussieBB(username, password)
 >>> account.get_services()
 [{allyourservicedetails}]
 ```
 
-For more, check out the module.
-
-
+For more, check out the docs.
 
 # AsyncIO version
 
 You can replace `from aussiebb import AussieBB` with `from aussiebb.asyncio import AussieBB` and you'll get an `aiohttp`-powered version. The only difference in this case is that you have to explicitly call `login()` for reasons.
 
+If you hit the rate limit it'll raise a `RateLimit` exception. I haven't put that functionality into the blocking version yet, since ... that tends not to hit it. 🤣
 
-# AsyncIO version
+# Development
 
-You can replace `from aussiebb import AussieBB` with `from aussiebb.asyncio import AussieBB` and you'll get an `aiohttp`-powered version. The only difference in this case is that you have to explicitly call `login()` for reasons.
 
-If you hit the rate limit it'll raise a `RateLimit` exception. I haven't put that functionality into the blocking version yet, since ... that tends not to hit it. 🤣
-
-# Example service tests I've seen
+## Example service tests I've seen
 
-All the "endpoints" should be tacked onto `aussiebb.BASEURL['api']`.
+All the "endpoints" below should be tacked onto `aussiebb.BASEURL['api']`.
 
-**Warning: `/nbn/{service_id}/connection` seems to have both a GET and POST method endpoint - tests on other endpoints may be similar.**
+**Warning:** `/nbn/{service_id}/connection` seems to have both a GET and POST method endpoint - tests on other endpoints may be similar.
 
 These can be run by using `AussieBB.run_test()` with the string after the last forward-slash as the "test" - ie, `connection` or `linestate`.
 
-## HFC 
+### HFC 
 
 These are entirely untested so far.
 
 | Endpoint | Method | Name | Description |
 | --- | --- | --- | --- |
 | `/nbn/{service_id}/connection` | Probably GET | Check Connection | Check to see if your service is currently connected |
 | `/nbn/{service_id}/connection` | Probably POST | Kick Connection | Kick your current session and force your device to reauthenticate |
 | `/tests/{service_id}/loopback` | Probably POST | Loopback Test | This will test the connectivity between the point NBN’s network transitions to ours and to the closest point to your property. Usually either the Network Termination Device or Node. |
 | `/tests/{service_id}/ntdstatus` | Probably POST | NTD Status | An NTD Status will show you the operational state of the Network Termination Device (NTD). The test will also show if the NTD is detecting the wired connection from your router. |
 
-## FTTC
+### FTTC
 
 | Endpoint | Method | Name | Description |
 | --- | --- | --- | --- |
 | `/nbn/{service_id}/connection` | GET |Check Connection | Check to see if your service is currently connected |
 | `/nbn/{service_id}/connection`  | Probably POST |Kick Connection | Kick your current session and force your device to reauthenticate |
 | `/tests/{service_id}/dpuportreset` | Probably POST |DPU Port Reset | Reset the Port on the DPU (Distribution Point Unit) along with clearing any errors that maybe causing issues with connectivity.  |
 | `/tests/{service_id}/dpuportstatus` | POST |DPU Port Status | A DPU (Distribution Point Unit) port status will show if the NCD (Network Connection Device) is providing power to the DPU. It will also state if the NCD (Network Connection Device) is in sync. |
@@ -98,7 +94,9 @@
     - renamed serviceid to service_id to match the api
     - added request_get_json to the sync class
     - added telephony_usage
     - added get_appointment which gets service appointments
     - updated get_usage so it checks the service list and will return telephony data if it's a PhoneMobile service
     - abstracted how URLS are generated so I don't have to keep adding them twice
     - added a filter on get_services which allows you to filter by type
+
+
```

### Comparing `pyaussiebb-0.0.8/aussiebb/__init__.py` & `pyaussiebb-0.0.9/aussiebb/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,60 @@
-""" class for interacting with Aussie Broadband APIs """
+""" A class for interacting with Aussie Broadband APIs """
 
 import inspect
 
 import json
 from time import time
 import sys
 
 from loguru import logger
 import requests
 
 from .const import BASEURL, API_ENDPOINTS, default_headers
-from .exceptions import AuthenticationException, RateLimitException
+from .exceptions import AuthenticationException, RateLimitException, RecursiveDepth
 from .utils import get_url
 
-#pylint: disable=too-many-public-methods
+#pylint: disable=too-many-public-methods,too-many-instance-attributes
 class AussieBB():
-    """ class for interacting with Aussie Broadband APIs """
-    def __init__(self, username: str, password: str, debug: bool=False):
-        """ class for interacting with Aussie Broadband APIs """
+    """ A class for interacting with Aussie Broadband APIs """
+    def __init__(self, username: str, password: str, debug: bool=False, **kwargs):
+        """ Setup function
+
+            ```
+            @param username: str - username for Aussie Broadband account
+            @param password: str - password for Aussie Broadband account
+            @param debug: bool - debug mode
+            @param services_cache_time: int
+                - seconds between caching get_services()
+                - defaults to 8 hours
+            ```
+        """
         self.username = username
         self.password = password
 
         self.debug = debug
+        # TODO: set the debug level in loguru when this is set to False
+
         if not (username and password):
             raise AuthenticationException("You need to supply both username and password")
         self.session = requests.Session()
 
         self.myaussie_cookie = ""
         self.token_expires = -1
 
-    def login(self):
-        """ does the login bit """
-        logger.debug("logging in...")
+        self.services_cache_time = kwargs.get('services_cache_time', 28800) # defaults to 8 hours
+        self.services_last_update = -1
+        self.services = None
+
+    def login(self, depth=0):
+        """ Logs into the account and caches the cookie.  """
+        if depth>2:
+            raise RecursiveDepth("Login recursion depth > 2")
+        logger.debug("Logging in...")
+
         url = BASEURL.get('login')
 
         payload = {
             'username' : self.username,
             'password' : self.password,
             }
         headers = default_headers()
@@ -47,183 +66,241 @@
         if response.status_code == 422:
             raise AuthenticationException(response.json())
         if response.status_code == 429:
             raise RateLimitException(response.json())
         response.raise_for_status()
 
         jsondata = response.json()
+
+        # we expire a little early just because
         self.token_expires = time() + jsondata.get('expiresIn') - 50
+
         self.myaussie_cookie = response.cookies.get('myaussie_cookie')
         if self.myaussie_cookie:
             logger.debug(f"Login Cookie: {self.myaussie_cookie}")
         return True
 
-    def has_token_expired(self):
-        """ returns bool if the token has expired """
+    def _has_token_expired(self):
+        """ Returns bool of if the token has expired """
         if time() > self.token_expires:
             return True
         return False
 
     def request_get(self, skip_login_check: bool = False, **kwargs):
-        """ does a GET request and logs in first if need be"""
+        """ Performs a GET request and logs in first if needed.
+
+        Returns the `requests.Response` object."""
         if not skip_login_check:
             logger.debug("skip_login_check false")
-            if self.has_token_expired():
+            if self._has_token_expired():
                 logger.debug("token has expired, logging in...")
                 self.login()
         if 'cookies' not in kwargs:
             kwargs['cookies'] = {'myaussie_cookie' : self.myaussie_cookie}
         response = self.session.get(**kwargs)
         response.raise_for_status()
         return response
 
     def request_get_json(self, skip_login_check: bool = False, **kwargs):
-        """ does a GET request and logs in first if need be, returns the JSON dict """
+        """ Performs a GET request and logs in first if needed.
+
+        Returns a dict of the JSON response.
+        """
         if not skip_login_check:
             logger.debug("skip_login_check false")
-            if self.has_token_expired():
+            if self._has_token_expired():
                 logger.debug("token has expired, logging in...")
                 self.login()
         if 'cookies' not in kwargs:
             kwargs['cookies'] = {'myaussie_cookie' : self.myaussie_cookie}
         response = self.session.get(**kwargs)
         response.raise_for_status()
         return response.json()
 
     def request_post(self, skip_login_check: bool = False, **kwargs):
-        """ does a POST request and logs in first if need be"""
+        """ Performs a POST request and logs in first if needed."""
         if not skip_login_check:
             logger.debug("skip_login_check false")
-            if self.has_token_expired():
+            if self._has_token_expired():
                 logger.debug("token has expired, logging in...")
                 self.login()
         if 'cookies' not in kwargs:
             kwargs['cookies'] = {'myaussie_cookie' : self.myaussie_cookie}
         if 'headers' not in kwargs:
             kwargs['headers'] = default_headers()
         response = self.session.post(**kwargs)
         response.raise_for_status()
         return response
 
     def get_customer_details(self):
-        """ grabs the customer details """
+        """ Grabs the customer details.
+
+        Returns a dict """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function)
         querystring = {"v":"2"}
         responsedata = self.request_get_json(url=url,
                                     params=querystring,
                                     )
         return responsedata
 
-    def get_services(self, page: int = 1, servicetypes: list=None):
-        """ returns a list of dicts of services associated with the account
 
-            if you want a specific kind of service, or services,
-            provide a list of matching strings in servicetypes
+    def _check_reload_cached_services(self):
+        """ If the age of the service data caching is too old, clear it and re-poll.
+
+        Returns bool - if it reloaded the cache.
         """
+        if not self.services:
+            self.get_services(use_cached=False)
+            return True
 
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function)
-        querystring = {'page' : page}
-        responsedata = self.request_get_json(url=url, params=querystring)
+        cache_expiry = self.services_last_update + self.services_cache_time
+        if time() >= cache_expiry:
+            self.get_services(use_cached=False)
+            return True
+        return False
+
+
+    def get_services(self, page: int = 1, servicetypes: list=None, use_cached: bool=False):
+        """ Returns a `list` of `dicts` of services associated with the account.
+
+            If you want a specific kind of service, or services,
+            provide a list of matching strings in servicetypes.
+
+            If you want to use cached data, call it with `use_cached=True`
+        """
+        if use_cached:
+            logger.debug("Using cached data for get_services.")
+            self._check_reload_cached_services()
+        else:
+            frame = inspect.currentframe()
+            url = get_url(inspect.getframeinfo(frame).function)
+            querystring = {'page' : page}
+
+            responsedata = self.request_get_json(url=url, params=querystring)
+            # cache the data
+            self.services_last_update = time()
+            self.services = responsedata.get('data')
 
         # only filter if we need to
-        if servicetypes and responsedata:
+        if servicetypes:
             logger.debug("Filtering services based on provided list: {}", servicetypes)
             filtered_responsedata = []
-            for service in responsedata.get('data'):
+            for service in self.services:
                 if service.get('type') in servicetypes:
                     filtered_responsedata.append(service)
                 else:
                     logger.debug("Skipping as type=={} - {}", service.get('type'), service)
-            # return the filtered responses to the source data
-            responsedata['data'] = filtered_responsedata
+            return filtered_responsedata
 
-        if responsedata.get('last_page') != responsedata.get('current_page'):
-            logger.debug("You've got a lot of services - please contact the package maintainer to test the multi-page functionality!") #pylint: disable=line-too-long
-        return responsedata.get('data')
+        return self.services
 
 
     def account_transactions(self):
-        """ pulls the json for transactions on your account
-            keys: ['current', 'pending', 'available', 'filters', 'typicalEveningSpeeds']
-            returns a dict where the key is the Month and year of the transaction, eg:
-            ```
+        """ Pulls the data for transactions on your account.
+
+            Returns a dict where the key is the month and year of the transaction.
+
+            Keys: `['current', 'pending', 'available', 'filters', 'typicalEveningSpeeds']`
+
+            Example output:
+
+            ``` json
             "August 2021": [
               {
                     "id": 12345,
                     "type": "receipt",
                     "time": "2021-08-06",
                     "description": "Payment #12345",
                     "amountCents": -8400,
                     "runningBalanceCents": 0
                 }
             ],
+            ```
             """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function)
         return self.request_get_json(url=url)
 
 
     def billing_invoice(self, invoice_id):
-        """ downloads an invoice
+        """ Downloads an invoice
 
-            this returns the bare response object, parsing the result is an exercise for the consumer
+            This returns the bare response object, parsing the result is an exercise for the consumer. It's a PDF file.
         """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'invoice_id' : invoice_id})
         return self.request_get_json(url=url)
 
     def account_paymentplans(self):
-        """ returns a json blob of payment plans for an account """
+        """ Returns a dict of payment plans for an account """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function)
         return self.request_get_json(url=url)
 
     def get_usage(self, service_id: int):
-        """ returns a json blob of usage for a service """
+        """
+        Returns a dict of usage for a service.
+
+        If it's a telephony service (`type=PhoneMobile`) it'll pull from the telephony endpoint.
+
+        """
+
+        if not self.services:
+            self.get_services(use_cached=True)
+        for service in self.services:
+            if service_id == service.get('service_id'):
+                if service.get('type') in ['PhoneMobile']:
+                    return self.telephony_usage(service_id)
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
         return self.request_get_json(url=url)
 
     def get_service_tests(self, service_id: int):
-        """ gets the available tests for a given service ID
-        returns list of dicts
+        """ Gets the available tests for a given service ID
+        Returns list of dicts
+
+        Example data:
+
+        ```
         [{
             'name' : str(),
             'description' : str',
             'link' : str(a url to the test)
         },]
+        ```
 
-        this is known to throw 400 errors if you query a VOIP service...
+        This has a habit of throwing 400 errors if you query a VOIP service...
         """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
         return self.request_get_json(url=url)
 
     def get_test_history(self, service_id: int):
-        """ gets the available tests for a given service ID
+        """ Gets the available tests for a given service ID
 
-        returns a list of dicts with tests which have been run
+        Returns a list of dicts with tests which have been run
         """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
         return self.request_get_json(url=url)
 
     def test_line_state(self, service_id: int):
-        """ tests the line state for a given service ID """
+        """ Tests the line state for a given service ID """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
         logger.debug("Testing line state, can take a few seconds...")
         response = self.request_post(url=url)
         return response.json()
 
     def run_test(self, service_id: int, test_name: str, test_method: str = 'post'):
-        """ run a test, but it checks it's valid first
+        """ Run a test, but it checks it's valid first
+
             There doesn't seem to be a valid way to identify what method you're supposed to use on each test.
+
             See the README for more analysis
 
             - 'status' of 'InProgress' use 'AussieBB.get_test_history()' and look for the 'id'
             - 'status' of 'Completed' means you've got the full response
         """
 
         test_links = [test for test in self.get_service_tests(service_id) if test.get('link', '').endswith(f'/{test_name}')] #pylint: disable=line-too-long
@@ -236,34 +313,57 @@
         test_name = test_links[0].get('name')
         logger.debug(f"Running {test_name}")
         if test_method == 'get':
             return self.request_get_json(url=test_links[0].get('link'))
         return self.request_post(url=test_links[0].get('link')).json()
 
     def service_plans(self, service_id: int):
-        """ pulls the JSON for the plan data
-            keys: ['current', 'pending', 'available', 'filters', 'typicalEveningSpeeds']
-            """
+        """ Pulls the plan data for a given service.
+
+            Keys: `['current', 'pending', 'available', 'filters', 'typicalEveningSpeeds']`
+
+        """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
         return self.request_get_json(url=url)
 
     def service_outages(self, service_id: int):
-        """ pulls the JSON for outages
-            keys: ['networkEvents', 'aussieOutages', 'currentNbnOutages', 'scheduledNbnOutages', 'resolvedScheduledNbnOutages', 'resolvedNbnOutages']
+        """ Pulls outages associated with a service.
+
+            Keys: `['networkEvents', 'aussieOutages', 'currentNbnOutages', 'scheduledNbnOutages', 'resolvedScheduledNbnOutages', 'resolvedNbnOutages']`
+
+            Example data:
+            ```
+            {
+                "networkEvents": [],
+                "aussieOutages": [],
+                "currentNbnOutages": [],
+                "scheduledNbnOutages": [],
+                "resolvedScheduledNbnOutages": [
+                    {
+                        "start_date": "2021-08-17T14:00:00Z",
+                        "end_date": "2021-08-17T20:00:00Z",
+                        "duration": "6.0"
+                    }
+                ],
+                "resolvedNbnOutages": []
+            }
+            ```
         """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
         return self.request_get_json(url=url)
 
     def service_boltons(self, service_id: int):
-        """ pulls the JSON for addons associated with the service
-            keys: ['id', 'name', 'description', 'costCents', 'additionalNote', 'active']
+        """ Pulls addons associated with the service.
+
+            Keys: `['id', 'name', 'description', 'costCents', 'additionalNote', 'active']`
+
+            Example data:
 
-            example data
             ```
             [{
                 "id": 4,
                 "name": "Small Change Big Change Donation",
                 "description": "Charitable donation to the Small Change Big Change program, part of the Telco Together Foundation, which helps build resilient young Australians",
                 "costCents": 100,
                 "additionalNote": null,
@@ -272,62 +372,67 @@
             ```
             """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
         return self.request_get_json(url=url)
 
     def service_datablocks(self, service_id: int):
-        """ pulls the JSON for datablocks associated with the service
-            keys: ['current', 'available']
+        """ Pulls datablocks associated with the service.
+
+            Keys: `['current', 'available']`
+
+            Example data:
 
-            example data
             ```
             {
                 "current": [],
                 "available": []
             }
             ```
-            """
+        """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
         return self.request_get_json(url=url)
 
     def telephony_usage(self, service_id: int):
-        """ pulls the JSON for telephony usage associated with the service
-            keys: ['national', 'mobile', 'international', 'sms', 'internet', 'voicemail', 'other', 'daysTotal', 'daysRemaining', 'historical']
+        """ Pulls the telephony usage associated with the service.
+
+            Keys: `['national', 'mobile', 'international', 'sms', 'internet', 'voicemail', 'other', 'daysTotal', 'daysRemaining', 'historical']`
+
+            Example data:
 
-            example data
             ```
             {"national":{"calls":0,"cost":0},"mobile":{"calls":0,"cost":0},"international":{"calls":0,"cost":0},"sms":{"calls":0,"cost":0},"internet":{"kbytes":0,"cost":0},"voicemail":{"calls":0,"cost":0},"other":{"calls":0,"cost":0},"daysTotal":31,"daysRemaining":2,"historical":[]}
             ```
             """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
         return self.request_get_json(url=url)
 
     def support_tickets(self):
-        """ pulls the support tickets associated with the account, returns a list of dicts
-            dict keys: ['ref', 'create', 'updated', 'service_id', 'type', 'subject', 'status', 'closed', 'awaiting_customer_reply', 'expected_response_minutes']
+        """ Pulls the support tickets associated with the account, returns a list of dicts.
+
+            Dict keys: `['ref', 'create', 'updated', 'service_id', 'type', 'subject', 'status', 'closed', 'awaiting_customer_reply', 'expected_response_minutes']`
 
             """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function)
         return self.request_get_json(url=url)
 
-    def get_appointment(self, ticketid):
-        """ pulls the support tickets associated with the account, returns a list of dicts
-            dict keys: ['ref', 'create', 'updated', 'service_id', 'type', 'subject', 'status', 'closed', 'awaiting_customer_reply', 'expected_response_minutes']
+    def get_appointment(self, ticketid: int):
+        """ Pulls the support tickets associated with the account, returns a list of dicts.
 
+            Dict keys: `['ref', 'create', 'updated', 'service_id', 'type', 'subject', 'status', 'closed', 'awaiting_customer_reply', 'expected_response_minutes']`
             """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'ticketid' : ticketid})
         return self.request_get_json(url=url)
 
 
     def account_contacts(self):
-        """ pulls the contacts with the account, returns a list of dicts
-            dict keys: ['id', 'first_name', 'last_name', 'email', 'dog', 'home_phone', 'work_phone', 'mobile_phone', 'work_mobile', 'primary_contact']
+        """ Pulls the contacts with the account, returns a list of dicts
 
+            Dict keys: `['id', 'first_name', 'last_name', 'email', 'dog', 'home_phone', 'work_phone', 'mobile_phone', 'work_mobile', 'primary_contact']`
             """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function)
         return self.request_get_json(url=url)
```

### Comparing `pyaussiebb-0.0.8/aussiebb/asyncio/__init__.py` & `pyaussiebb-0.0.9/aussiebb/asyncio/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,158 +7,182 @@
 import json
 from time import time
 
 import sys
 try:
     import aiohttp
 except ImportError as error_message:
-    print("Failed to import aiohttp, bailing: {error_message}", file=sys.stderr)
+    print(f"Failed to import aiohttp, bailing: {error_message}", file=sys.stderr)
     sys.exit(1)
 
 from ..const import BASEURL, default_headers, DEFAULT_BACKOFF_DELAY
 from ..exceptions import AuthenticationException, RateLimitException, RecursiveDepth
 from ..utils import get_url
 
-class AussieBB(): #pylint: disable=too-many-public-methods
+
+class AussieBB(): #pylint: disable=too-many-public-methods,too-many-instance-attributes
     """ aiohttp class for interacting with Aussie Broadband APIs """
-    def __init__(self, username: str, password: str, session: aiohttp.client.ClientSession=None, debug: bool=False ):
-        """ class for interacting with Aussie Broadband APIs """
+    def __init__(self, username: str, password: str, session: aiohttp.client.ClientSession=None, debug: bool=False, **kwargs):
+        """ Setup function
+
+            ```
+            @param username: str - username for Aussie Broadband account
+            @param password: str - password for Aussie Broadband account
+            @param debug: bool - debug mode
+            @param services_cache_time: int
+                - seconds between caching get_services()
+                - defaults to 8 hours
+            ```
+        """
         self.username = username
         self.password = password
         if not (username and password):
             raise AuthenticationException("You need to supply both username and password")
 
-        self.made_own_session = False
-        if session is None:
+        if not session:
             self.session = aiohttp.ClientSession()
-            self.made_own_session = True
         else:
             self.session = session
 
         self.myaussie_cookie = ""
         self.token_expires = -1
         self.debug = debug
 
+        self.services_cache_time = kwargs.get('services_cache_time', 28800) # defaults to 8 hours
+        self.services_last_update = -1
+        self.services = None
+
+
+    def _debug_print(self, message: str):
+        """ Prints a debug message to stderr if the class is in debug mode. """
+        if self.debug:
+            print(message, file=sys.stderr)
+
     async def login(self, depth=0):
-        """ does the login bit """
+        """ Logs into the account and caches the cookie.  """
         if depth>2:
             raise RecursiveDepth("Login recursion depth > 2")
-        print("logging in...")
+        self._debug_print("Logging in...")
 
         url = BASEURL.get('login')
 
-        if not self.has_token_expired():
+        if not self._has_token_expired():
             return True
 
         payload = {
             'username' : self.username,
             'password' : self.password,
             }
         headers = default_headers()
 
         async with self.session.post(url=url, headers=headers, json=payload) as response:
             try:
                 await self.handle_response_fail(response)
                 jsondata = await response.json()
             except RateLimitException:
                 return await self.login(depth+1)
-            if self.debug:
-                print(f"Login response status: {response.status}", file=sys.stderr)
-        if self.debug:
-            print(f"Dumping login response: {json.dumps(jsondata)}", file=sys.stderr)
+            self._debug_print(f"Login response status: {response.status}")
+        self._debug_print(f"Dumping login response: {json.dumps(jsondata)}")
+
+        # we expire a little early just because
         self.token_expires = time() + jsondata.get('expiresIn') - 50
         self.myaussie_cookie = response.cookies.get('myaussie_cookie')
         if self.myaussie_cookie:
-            if self.debug:
-                print(f"Login Cookie: {self.myaussie_cookie}", file=sys.stderr)
+            self._debug_print(f"Login Cookie: {self.myaussie_cookie}")
         return True
 
     async def handle_response_fail(self, response, wait_on_rate_limit: bool=True):
-        """ handles response status codes """
+        """ Handles response status codes. Tries to gracefully handle the rate limiting.
+
+        ```
+        @param response - aiohttp.Response - the full response object
+        @param wait_on_rate_limit - bool - if hitting a rate limit, async wait on the time limit
+        ```
+        """
         ratelimit_remaining = int(response.headers.get('x-ratelimit-remaining', -1))
-        if self.debug:
-            print(f"Rate limit header: {response.headers.get('x-ratelimit-remaining', -1)}", file=sys.stderr)
+        self._debug_print(f"Rate limit header: {response.headers.get('x-ratelimit-remaining', -1)}")
         if ratelimit_remaining < 5 and wait_on_rate_limit:
             print("Rate limit below 5, sleeping for 1 second.", file=sys.stderr)
             await asyncio.sleep(1)
 
         if response.status == 422:
             raise AuthenticationException(await response.json())
         if response.status == 429:
             jsondata = await response.json()
-            if self.debug:
-                print(f"Dumping headers: {response.headers}", file=sys.stderr)
-                print(f"Dumping response: {jsondata}", file=sys.stderr)
+            self._debug_print(f"Dumping headers: {response.headers}")
+            self._debug_print(f"Dumping response: {jsondata}")
             delay = DEFAULT_BACKOFF_DELAY
             if 'Please try again in ' in str(jsondata.get('errors')):
                 fallback_value = [f"default {DEFAULT_BACKOFF_DELAY} seconds"]
                 delay = jsondata.get('errors', {}).get('username', fallback_value)[0].split()[-2]
                 # give it some extra time to cool off
                 delay = int(delay)+5
 
                 if 0 < delay < 1000:
-                    if self.debug:
-                        print(f"Found delay: {delay}", file=sys.stderr)
+                    self._debug_print(f"Found delay: {delay}")
                     delay = int(delay)
-                elif self.debug:
-                    print(f"Couldn't parse delay, using default: {delay}", file=sys.stderr)
+                else:
+                    self._debug_print(f"Couldn't parse delay, using default: {delay}")
             else:
                 delay = DEFAULT_BACKOFF_DELAY
                 if self.debug:
                     print(f"Couldn't parse delay, using default: {delay}", file=sys.stderr)
             if wait_on_rate_limit:
                 print(f"Rate limit on Aussie API calls raised, sleeping for {delay} seconds.", file=sys.stderr)
                 await asyncio.sleep(delay)
             raise RateLimitException(jsondata)
         response.raise_for_status()
 
-    def has_token_expired(self):
-        """ returns bool if the token has expired """
+    def _has_token_expired(self):
+        """ Returns bool of if the token has expired """
         if time() > self.token_expires:
             return True
         return False
 
     async def request_get(self, skip_login_check: bool = False, **kwargs) -> dict:
-        """ does a GET request and logs in first if need be, returns the body bytes """
+        """ Performs a GET request and logs in first if needed. """
         depth = kwargs.get('depth', 0)
         if depth > 2:
             raise RecursiveDepth(f"depth: {depth}")
 
         if self.session is None:
             self.session = aiohttp.ClientSession()
 
         if not skip_login_check:
-            if self.has_token_expired():
+            if self._has_token_expired():
                 if self.debug:
                     print("token has expired, logging in...", file=sys.stderr)
                 await self.login()
 
         if 'cookies' not in kwargs:
             kwargs['cookies'] = {'myaussie_cookie' : self.myaussie_cookie}
         async with self.session.get(**kwargs) as response:
             try:
                 await self.handle_response_fail(response)
                 await response.read()
             except RateLimitException:
-                response = await self.request_get_json(skip_login_check, **kwargs)
+                response = await self.request_get(skip_login_check, **kwargs)
             return response
 
     async def request_get_json(self, skip_login_check: bool = False, **kwargs) -> dict:
-        """ does a GET request and logs in first if need be, returns a dict of json """
+        """ Performs a GET request and logs in first if needed.
+
+        Returns a dict of the JSON response.
+        """
         depth = kwargs.get('depth', 0)
         if depth > 2:
             raise RecursiveDepth(f"depth: {depth}")
 
         if self.session is None:
             self.session = aiohttp.ClientSession()
 
         if not skip_login_check:
             if self.debug:
                 print("skip_login_check false", file=sys.stderr)
-            if self.has_token_expired():
+            if self._has_token_expired():
                 if self.debug:
                     print("token has expired, logging in...", file=sys.stderr)
                 await self.login()
 
         if 'cookies' not in kwargs:
             kwargs['cookies'] = {'myaussie_cookie' : self.myaussie_cookie}
         async with self.session.get(**kwargs) as response:
@@ -166,26 +190,29 @@
                 await self.handle_response_fail(response)
                 jsondata = await response.json()
             except RateLimitException:
                 jsondata = await self.request_get_json(skip_login_check, **kwargs)
         return jsondata
 
     async def request_post_json(self, url, **kwargs):
-        """ does a POST request and logs in first if need be"""
+        """ Performs a POST request and logs in first if needed.
+
+        Returns a dict of the response data.
+        """
         depth = kwargs.get('depth', 0)
         if depth > 2:
             raise RecursiveDepth(f"depth: {depth}")
 
         if self.session is None:
             self.session = aiohttp.ClientSession()
 
         if not kwargs.get('skip_login_check', False):
             if self.debug:
                 print("skip_login_check false", file=sys.stderr)
-            if self.has_token_expired():
+            if self._has_token_expired():
                 if self.debug:
                     print("token has expired, logging in...", file=sys.stderr)
                 await self.login()
 
         #if 'cookies' not in kwargs:
         #    kwargs['cookies'] = {'myaussie_cookie' : self.myaussie_cookie}
         cookies = kwargs.get('cookies', {'myaussie_cookie' : self.myaussie_cookie})
@@ -195,151 +222,185 @@
                 await self.handle_response_fail(response)
                 jsondata = await response.json()
             except RateLimitException:
                 jsondata = await self.request_post_json(url=url, depth=depth+1, **kwargs)
         return jsondata
 
     async def get_customer_details(self) -> dict:
-        """ grabs the customer details, returns a dict """
+        """ Grabs the customer details.
+
+        Returns a dict """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function)
         params = {"v":"2"}
         return await self.request_get_json(url=url,
                                     params=params,
                                     )
 
-    async def get_services(self, page: int=1, servicetypes: list=None):
-        """ returns a list of dicts of services associated with the account
-            if you want a specific kind of service, or services,
-            provide a list of matching strings in servicetypes
+    async def _check_reload_cached_services(self):
+        """ If the age of the service data caching is too old, clear it and re-poll.
+
+        Returns bool - if it reloaded the cache.
         """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function)
-        params = {'page' : page}
+        if not self.services:
+            await self.get_services(use_cached=False)
+            return True
+        cache_expiry = self.services_last_update + self.services_cache_time
+        if time() >= cache_expiry:
+            await self.get_services(use_cached=False)
+            return True
+        return False
+
+    async def get_services(self, page: int=1, servicetypes: list=None, use_cached: bool=False):
+        """ Returns a `list` of `dicts` of services associated with the account.
+
+            If you want a specific kind of service, or services,
+            provide a list of matching strings in servicetypes.
+
+            If you want to use cached data, call it with `use_cached=True`
+        """
+        if use_cached:
+            self._debug_print("Using cached data for get_services.")
+            await self._check_reload_cached_services()
+        else:
+            frame = inspect.currentframe()
+            url = get_url(inspect.getframeinfo(frame).function)
+            params = {'page' : page}
+
+            responsedata = await self.request_get_json(url=url, params=params)
+            # cache the data
+            self.services_last_update = time()
+            self.services = responsedata.get('data')
 
-        responsedata = await self.request_get_json(url=url, params=params)
         # only filter if we need to
-        if servicetypes and responsedata:
-            if self.debug:
-                print(f"Filtering services based on provided list: {servicetypes}", file=sys.stderr)
+        if servicetypes:
+            self._debug_print(f"Filtering services based on provided list: {servicetypes}")
             filtered_responsedata = []
-            for service in responsedata.get('data'):
+            for service in self.services:
                 if service.get('type') in servicetypes:
                     filtered_responsedata.append(service)
                 else:
-                    if self.debug:
-                        print(f"Skipping as type=={service.get('type')} - {service}", file=sys.stderr)
-            # return the filtered responses to the source data
-            responsedata['data'] = filtered_responsedata
+                    self._debug_print(f"Skipping as type=={service.get('type')} - {service}")
+            return filtered_responsedata
 
-        if responsedata.get('last_page') != responsedata.get('current_page'):
-            if self.debug:
-                print("You've got a lot of services - please contact the package maintainer to test the multi-page functionality!", file=sys.stderr) #pylint: disable=line-too-long
-        return responsedata.get('data')
+        return self.services
 
     async def account_transactions(self):
-        """ pulls the json for transactions on your account
-            keys: ['current', 'pending', 'available', 'filters', 'typicalEveningSpeeds']
-            returns a dict where the key is the Month and year of the transaction, eg:
-            ```
+        """ Pulls the data for transactions on your account.
+
+            Returns a dict where the key is the month and year of the transaction.
+
+            Keys: `['current', 'pending', 'available', 'filters', 'typicalEveningSpeeds']`
+
+            Example output:
+
+            ``` json
             "August 2021": [
               {
                     "id": 12345,
                     "type": "receipt",
                     "time": "2021-08-06",
                     "description": "Payment #12345",
                     "amountCents": -8400,
                     "runningBalanceCents": 0
                 }
             ],
+            ```
             """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function)
         responsedata = await self.request_get_json(url=url)
         return responsedata
 
     async def billing_invoice(self, invoice_id):
-        """ downloads an invoice
+        """ Downloads an invoice
 
-            this returns the response object
+            This returns the bare response object, parsing the result is an exercise for the consumer. It's a PDF file.
         """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'invoice_id', invoice_id})
         responsedata = await self.request_get_json(url=url)
         return responsedata
 
     async def account_paymentplans(self):
-        """ returns a json blob of payment plans for an account """
+        """ Returns a dict of payment plans for an account """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function)
         responsedata = await self.request_get_json(url=url)
         return responsedata
 
     async def get_usage(self, service_id: int):
         """
-        returns a json blob of usage for a service
+        Returns a dict of usage for a service.
 
-        will double-check it's not a telephony service and pull the data for that if it is
+        If it's a telephony service (`type=PhoneMobile`) it'll pull from the telephony endpoint.
 
         """
-        services = await self.get_services()
+        services = await self.get_services(use_cached=True)
         for service in services:
             if service_id == service.get('service_id'):
                 if service.get('type') in ['PhoneMobile']:
                     return await self.telephony_usage(service_id)
 
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
         responsedata = await self.request_get_json(url=url)
         return responsedata
 
     async def get_service_tests(self, service_id: int):
-        """ gets the available tests for a given service ID
-        returns list of dicts
+        """ Gets the available tests for a given service ID
+        Returns list of dicts
+
+        Example data:
+
+        ```
         [{
             'name' : str(),
             'description' : str',
             'link' : str(a url to the test)
         },]
+        ```
 
-        this is known to throw 400 errors if you query a VOIP service...
+        This has a habit of throwing 400 errors if you query a VOIP service...
         """
         if self.debug:
             print(f"Getting service tests for {service_id}", file=sys.stderr)
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function)
         responsedata = await self.request_get_json(url=url)
         return responsedata
 
     async def get_test_history(self, service_id: int):
-        """ gets the available tests for a given service ID
+        """ Gets the available tests for a given service ID
 
-        returns a list of dicts with tests which have been run
+        Returns a list of dicts with tests which have been run
         """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
         responsedata = await self.request_get_json(url=url)
         return responsedata
 
     async def test_line_state(self, service_id: int):
-        """ tests the line state for a given service ID """
+        """ Tests the line state for a given service ID """
 
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
 
         if self.debug:
             print("Testing line state, can take a few seconds...")
         response = await self.request_post_json(url=url)
         if self.debug:
             print(f"Response: {response}", file=sys.stderr)
         return response
 
     async def run_test(self, service_id: int, test_name: str, test_method: str = 'post'):
-        """ run a test, but it checks it's valid first
+        """ Run a test, but it checks it's valid first
+
             There doesn't seem to be a valid way to identify what method you're supposed to use on each test.
+
             See the README for more analysis
 
             - 'status' of 'InProgress' use 'AussieBB.get_test_history()' and look for the 'id'
             - 'status' of 'Completed' means you've got the full response
         """
 
         service_tests = await self.get_service_tests(service_id)
@@ -357,30 +418,33 @@
         if test_method == 'get':
             result = await self.request_get_json(url=test_links[0].get('link'))
         else:
             result = await self.request_post_json(url=test_links[0].get('link'))
         return result
 
     async def service_plans(self, service_id: int):
-        """ pulls the JSON for the plan data
-            keys: ['current', 'pending', 'available', 'filters', 'typicalEveningSpeeds']
-            """
+        """ Pulls the plan data for a given service.
+
+            Keys: `['current', 'pending', 'available', 'filters', 'typicalEveningSpeeds']`
+
+        """
 
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
         responsedata = await self.request_get_json(url=url)
         if self.debug:
             print(responsedata, file=sys.stderr)
         return responsedata
 
     async def service_outages(self, service_id: int):
-        """ pulls the JSON for outages
-            keys: ['networkEvents', 'aussieOutages', 'currentNbnOutages', 'scheduledNbnOutages', 'resolvedScheduledNbnOutages', 'resolvedNbnOutages']
+        """ Pulls outages associated with a service.
 
-            example data
+            Keys: `['networkEvents', 'aussieOutages', 'currentNbnOutages', 'scheduledNbnOutages', 'resolvedScheduledNbnOutages', 'resolvedNbnOutages']`
+
+            Example data:
             ```
             {
                 "networkEvents": [],
                 "aussieOutages": [],
                 "currentNbnOutages": [],
                 "scheduledNbnOutages": [],
                 "resolvedScheduledNbnOutages": [
@@ -389,28 +453,30 @@
                         "end_date": "2021-08-17T20:00:00Z",
                         "duration": "6.0"
                     }
                 ],
                 "resolvedNbnOutages": []
             }
             ```
-            """
+        """
 
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
         responsedata = await self.request_get_json(url=url)
         if self.debug:
             print(responsedata, file=sys.stderr)
         return responsedata
 
     async def service_boltons(self, service_id: int):
-        """ pulls the JSON for addons associated with the service
-            keys: ['id', 'name', 'description', 'costCents', 'additionalNote', 'active']
+        """ Pulls addons associated with the service.
+
+            Keys: `['id', 'name', 'description', 'costCents', 'additionalNote', 'active']`
+
+            Example data:
 
-            example data
             ```
             [{
                 "id": 4,
                 "name": "Small Change Big Change Donation",
                 "description": "Charitable donation to the Small Change Big Change program, part of the Telco Together Foundation, which helps build resilient young Australians",
                 "costCents": 100,
                 "additionalNote": null,
@@ -423,65 +489,80 @@
         url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
         responsedata = await self.request_get_json(url=url)
         if self.debug:
             print(responsedata, file=sys.stderr)
         return responsedata
 
     async def service_datablocks(self, service_id: int):
-        """ pulls the JSON for datablocks associated with the service
-            keys: ['current', 'available']
+        """ Pulls datablocks associated with the service.
+
+            Keys: `['current', 'available']`
+
+            Example data:
 
-            example data
             ```
             {
                 "current": [],
                 "available": []
             }
             ```
-            """
+        """
 
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
         responsedata = await self.request_get_json(url=url)
         if self.debug:
             print(responsedata, file=sys.stderr)
         return responsedata
 
     async def telephony_usage(self, service_id: int):
-        """ pulls the JSON for telephony usage associated with the service
-            keys: ['national', 'mobile', 'international', 'sms', 'internet', 'voicemail', 'other', 'daysTotal', 'daysRemaining', 'historical']
+        """ Pulls the telephony usage associated with the service.
+
+            Keys: `['national', 'mobile', 'international', 'sms', 'internet', 'voicemail', 'other', 'daysTotal', 'daysRemaining', 'historical']`
+
+            Example data:
 
-            example data
             ```
             {"national":{"calls":0,"cost":0},"mobile":{"calls":0,"cost":0},"international":{"calls":0,"cost":0},"sms":{"calls":0,"cost":0},"internet":{"kbytes":0,"cost":0},"voicemail":{"calls":0,"cost":0},"other":{"calls":0,"cost":0},"daysTotal":31,"daysRemaining":2,"historical":[]}
             ```
             """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
         responsedata = await self.request_get_json(url=url)
         if self.debug:
             print(responsedata, file=sys.stderr)
         return responsedata
 
     async def support_tickets(self):
-        """ pulls the support tickets associated with the account, returns a list of dicts
-            dict keys: ['ref', 'create', 'updated', 'service_id', 'type', 'subject', 'status', 'closed', 'awaiting_customer_reply', 'expected_response_minutes']
+        """ Pulls the support tickets associated with the account, returns a list of dicts.
+
+            Dict keys: `['ref', 'create', 'updated', 'service_id', 'type', 'subject', 'status', 'closed', 'awaiting_customer_reply', 'expected_response_minutes']`
 
             """
 
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function)
         responsedata = await self.request_get_json(url=url)
         if self.debug:
             print(responsedata, file=sys.stderr)
         return responsedata
 
+    async def get_appointment(self, ticketid: int):
+        """ Pulls the support tickets associated with the account, returns a list of dicts.
+
+            Dict keys: `['ref', 'create', 'updated', 'service_id', 'type', 'subject', 'status', 'closed', 'awaiting_customer_reply', 'expected_response_minutes']`
+            """
+        frame = inspect.currentframe()
+        url = get_url(inspect.getframeinfo(frame).function, {'ticketid' : ticketid})
+        return await self.request_get_json(url=url)
+
     async def account_contacts(self):
-        """ pulls the contacts with the account, returns a list of dicts
-            dict keys: ['id', 'first_name', 'last_name', 'email', 'dog', 'home_phone', 'work_phone', 'mobile_phone', 'work_mobile', 'primary_contact']
+        """ Pulls the contacts with the account, returns a list of dicts
+
+            Dict keys: `['id', 'first_name', 'last_name', 'email', 'dog', 'home_phone', 'work_phone', 'mobile_phone', 'work_mobile', 'primary_contact']`
             """
         frame = inspect.currentframe()
         url = get_url(inspect.getframeinfo(frame).function)
         responsedata = await self.request_get_json(url=url)
         if self.debug:
             print(responsedata, file=sys.stderr)
         return responsedata
```

### Comparing `pyaussiebb-0.0.8/aussiebb/const.py` & `pyaussiebb-0.0.9/aussiebb/const.py`

 * *Files identical despite different names*

### Comparing `pyaussiebb-0.0.8/pyaussiebb.egg-info/PKG-INFO` & `pyaussiebb-0.0.9/pyaussiebb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaussiebb
-Version: 0.0.8
+Version: 0.0.9
 Summary: Aussie Broadband API module
 Home-page: https://github.com/yaleman/aussiebb
 Author: James Hodgkinson
 Author-email: yaleman@ricetek.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -30,49 +30,45 @@
 python
 >>> from aussiebb import AussieBB
 >>> account = AussieBB(username, password)
 >>> account.get_services()
 [{allyourservicedetails}]
 ```
 
-For more, check out the module.
-
-
+For more, check out the docs.
 
 # AsyncIO version
 
 You can replace `from aussiebb import AussieBB` with `from aussiebb.asyncio import AussieBB` and you'll get an `aiohttp`-powered version. The only difference in this case is that you have to explicitly call `login()` for reasons.
 
+If you hit the rate limit it'll raise a `RateLimit` exception. I haven't put that functionality into the blocking version yet, since ... that tends not to hit it. 🤣
 
-# AsyncIO version
+# Development
 
-You can replace `from aussiebb import AussieBB` with `from aussiebb.asyncio import AussieBB` and you'll get an `aiohttp`-powered version. The only difference in this case is that you have to explicitly call `login()` for reasons.
 
-If you hit the rate limit it'll raise a `RateLimit` exception. I haven't put that functionality into the blocking version yet, since ... that tends not to hit it. 🤣
-
-# Example service tests I've seen
+## Example service tests I've seen
 
-All the "endpoints" should be tacked onto `aussiebb.BASEURL['api']`.
+All the "endpoints" below should be tacked onto `aussiebb.BASEURL['api']`.
 
-**Warning: `/nbn/{service_id}/connection` seems to have both a GET and POST method endpoint - tests on other endpoints may be similar.**
+**Warning:** `/nbn/{service_id}/connection` seems to have both a GET and POST method endpoint - tests on other endpoints may be similar.
 
 These can be run by using `AussieBB.run_test()` with the string after the last forward-slash as the "test" - ie, `connection` or `linestate`.
 
-## HFC 
+### HFC 
 
 These are entirely untested so far.
 
 | Endpoint | Method | Name | Description |
 | --- | --- | --- | --- |
 | `/nbn/{service_id}/connection` | Probably GET | Check Connection | Check to see if your service is currently connected |
 | `/nbn/{service_id}/connection` | Probably POST | Kick Connection | Kick your current session and force your device to reauthenticate |
 | `/tests/{service_id}/loopback` | Probably POST | Loopback Test | This will test the connectivity between the point NBN’s network transitions to ours and to the closest point to your property. Usually either the Network Termination Device or Node. |
 | `/tests/{service_id}/ntdstatus` | Probably POST | NTD Status | An NTD Status will show you the operational state of the Network Termination Device (NTD). The test will also show if the NTD is detecting the wired connection from your router. |
 
-## FTTC
+### FTTC
 
 | Endpoint | Method | Name | Description |
 | --- | --- | --- | --- |
 | `/nbn/{service_id}/connection` | GET |Check Connection | Check to see if your service is currently connected |
 | `/nbn/{service_id}/connection`  | Probably POST |Kick Connection | Kick your current session and force your device to reauthenticate |
 | `/tests/{service_id}/dpuportreset` | Probably POST |DPU Port Reset | Reset the Port on the DPU (Distribution Point Unit) along with clearing any errors that maybe causing issues with connectivity.  |
 | `/tests/{service_id}/dpuportstatus` | POST |DPU Port Status | A DPU (Distribution Point Unit) port status will show if the NCD (Network Connection Device) is providing power to the DPU. It will also state if the NCD (Network Connection Device) is in sync. |
@@ -117,7 +113,9 @@
     - added telephony_usage
     - added get_appointment which gets service appointments
     - updated get_usage so it checks the service list and will return telephony data if it's a PhoneMobile service
     - abstracted how URLS are generated so I don't have to keep adding them twice
     - added a filter on get_services which allows you to filter by type
 
 
+
+
```

### Comparing `pyaussiebb-0.0.8/setup.py` & `pyaussiebb-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     LONGDESCRIPTION = fh.read()
 
 setuptools.setup(
     name="pyaussiebb",
-    version="0.0.8",
+    version="0.0.9",
     author="James Hodgkinson",
     author_email="yaleman@ricetek.net",
     description="Aussie Broadband API module",
     long_description=LONGDESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/yaleman/aussiebb",
     packages=setuptools.find_packages(),
-    install_requires=['requests', 'loguru'],
+    install_requires=['requests', 'loguru', 'aiohttp'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

