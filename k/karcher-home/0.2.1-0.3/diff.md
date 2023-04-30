# Comparing `tmp/karcher-home-0.2.1.tar.gz` & `tmp/karcher-home-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karcher-home-0.2.1.tar", last modified: Thu Apr 27 21:12:37 2023, max compression
+gzip compressed data, was "karcher-home-0.3.tar", last modified: Sun Apr 30 14:48:35 2023, max compression
```

## Comparing `karcher-home-0.2.1.tar` & `karcher-home-0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-27 21:12:37.762225 karcher-home-0.2.1/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1066 2023-04-23 18:36:52.000000 karcher-home-0.2.1/LICENSE
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1309 2023-04-27 21:12:37.762225 karcher-home-0.2.1/PKG-INFO
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      920 2023-04-27 20:58:22.000000 karcher-home-0.2.1/README.md
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-27 21:12:37.758225 karcher-home-0.2.1/karcher/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        0 2023-04-26 11:31:28.000000 karcher-home-0.2.1/karcher/__init__.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2445 2023-04-25 13:06:17.000000 karcher-home-0.2.1/karcher/auth.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4967 2023-04-27 21:11:26.000000 karcher-home-0.2.1/karcher/cli.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2287 2023-04-27 20:58:22.000000 karcher-home-0.2.1/karcher/consts.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2401 2023-04-27 20:58:22.000000 karcher-home-0.2.1/karcher/countries.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4882 2023-04-27 20:58:22.000000 karcher-home-0.2.1/karcher/device.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1344 2023-04-26 12:09:27.000000 karcher-home-0.2.1/karcher/exception.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      592 2023-04-26 12:09:03.000000 karcher-home-0.2.1/karcher/identifiers.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)    13421 2023-04-27 21:11:19.000000 karcher-home-0.2.1/karcher/karcher.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      706 2023-04-26 12:09:49.000000 karcher-home-0.2.1/karcher/map.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     7843 2023-04-26 08:16:45.000000 karcher-home-0.2.1/karcher/mapdata_pb2.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3310 2023-04-27 21:11:19.000000 karcher-home-0.2.1/karcher/mqtt.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3030 2023-04-27 20:58:22.000000 karcher-home-0.2.1/karcher/utils.py
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-27 21:12:37.762225 karcher-home-0.2.1/karcher_home.egg-info/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1309 2023-04-27 21:12:37.000000 karcher-home-0.2.1/karcher_home.egg-info/PKG-INFO
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      514 2023-04-27 21:12:37.000000 karcher-home-0.2.1/karcher_home.egg-info/SOURCES.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        1 2023-04-27 21:12:37.000000 karcher-home-0.2.1/karcher_home.egg-info/dependency_links.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       54 2023-04-27 21:12:37.000000 karcher-home-0.2.1/karcher_home.egg-info/entry_points.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       45 2023-04-27 21:12:37.000000 karcher-home-0.2.1/karcher_home.egg-info/requires.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        8 2023-04-27 21:12:37.000000 karcher-home-0.2.1/karcher_home.egg-info/top_level.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       79 2023-04-27 21:12:37.762225 karcher-home-0.2.1/setup.cfg
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      844 2023-04-27 21:11:26.000000 karcher-home-0.2.1/setup.py
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-27 21:12:37.762225 karcher-home-0.2.1/tests/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4294 2023-04-23 21:35:44.000000 karcher-home-0.2.1/tests/test_enc.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-30 14:48:35.279430 karcher-home-0.3/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1066 2023-04-23 18:36:52.000000 karcher-home-0.3/LICENSE
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1478 2023-04-30 14:48:35.279430 karcher-home-0.3/PKG-INFO
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1095 2023-04-27 21:15:39.000000 karcher-home-0.3/README.md
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-30 14:48:35.271429 karcher-home-0.3/karcher/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        0 2023-04-26 11:31:28.000000 karcher-home-0.3/karcher/__init__.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2147 2023-04-30 14:40:55.000000 karcher-home-0.3/karcher/auth.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4967 2023-04-27 21:11:26.000000 karcher-home-0.3/karcher/cli.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2287 2023-04-28 20:14:55.000000 karcher-home-0.3/karcher/consts.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5705 2023-04-28 20:58:15.000000 karcher-home-0.3/karcher/countries.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5060 2023-04-28 20:50:00.000000 karcher-home-0.3/karcher/device.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1663 2023-04-28 20:58:33.000000 karcher-home-0.3/karcher/exception.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      592 2023-04-26 12:09:03.000000 karcher-home-0.3/karcher/identifiers.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)    13754 2023-04-30 14:46:08.000000 karcher-home-0.3/karcher/karcher.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      706 2023-04-28 20:53:12.000000 karcher-home-0.3/karcher/map.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     7843 2023-04-26 08:16:45.000000 karcher-home-0.3/karcher/mapdata_pb2.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3354 2023-04-28 20:53:54.000000 karcher-home-0.3/karcher/mqtt.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3192 2023-04-28 20:55:32.000000 karcher-home-0.3/karcher/utils.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-30 14:48:35.275430 karcher-home-0.3/karcher_home.egg-info/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1478 2023-04-30 14:48:35.000000 karcher-home-0.3/karcher_home.egg-info/PKG-INFO
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      514 2023-04-30 14:48:35.000000 karcher-home-0.3/karcher_home.egg-info/SOURCES.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        1 2023-04-30 14:48:35.000000 karcher-home-0.3/karcher_home.egg-info/dependency_links.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       54 2023-04-30 14:48:35.000000 karcher-home-0.3/karcher_home.egg-info/entry_points.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       45 2023-04-30 14:48:35.000000 karcher-home-0.3/karcher_home.egg-info/requires.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        8 2023-04-30 14:48:35.000000 karcher-home-0.3/karcher_home.egg-info/top_level.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       79 2023-04-30 14:48:35.279430 karcher-home-0.3/setup.cfg
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      838 2023-04-28 20:56:11.000000 karcher-home-0.3/setup.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-30 14:48:35.275430 karcher-home-0.3/tests/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4294 2023-04-23 21:35:44.000000 karcher-home-0.3/tests/test_enc.py
```

### Comparing `karcher-home-0.2.1/LICENSE` & `karcher-home-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `karcher-home-0.2.1/PKG-INFO` & `karcher-home-0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: karcher-home
-Version: 0.2.1
+Version: 0.3
 Summary: Kärcher Home Robots client
 Home-page: https://github.com/lafriks/python-karcher
-Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.2.1/karcher-home-0.2.1.tar.gz
+Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.3/karcher-home-0.3.tar.gz
 Author: Lauris BH
 Author-email: lauris@nix.lv
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -27,23 +27,25 @@
 
 ```console
 Usage: karcher-home [OPTIONS] COMMAND [ARGS]...
 
   Tool for connectiong and getting information from Kärcher Home Robots.
 
 Options:
-  -d, --debug
+  -d, --debug                     Enable debug mode.
   -o, --output [json|json_pretty]
-  -r, --region [eu|us|cn]         Region of the server to query. Default: 'eu'
+                                  Output format. Default: "json"
+  -r, --region [eu|us|cn]         Region of the server to query. Default: "eu"
   --help                          Show this message and exit.
 
 Commands:
-  devices   List all devices.
-  get-urls  Get region information.
-  login     Get user session tokens.
+  device-properties  Get device properties.
+  devices            List all devices.
+  login              Get user session tokens.
+  urls               Get region information.
 ```
 
 ### From code
 
 ```python
 from karcher.karcher import KarcherHome
```

### Comparing `karcher-home-0.2.1/README.md` & `karcher-home-0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 
 ```console
 Usage: karcher-home [OPTIONS] COMMAND [ARGS]...
 
   Tool for connectiong and getting information from Kärcher Home Robots.
 
 Options:
-  -d, --debug
+  -d, --debug                     Enable debug mode.
   -o, --output [json|json_pretty]
-  -r, --region [eu|us|cn]         Region of the server to query. Default: 'eu'
+                                  Output format. Default: "json"
+  -r, --region [eu|us|cn]         Region of the server to query. Default: "eu"
   --help                          Show this message and exit.
 
 Commands:
-  devices   List all devices.
-  get-urls  Get region information.
-  login     Get user session tokens.
+  device-properties  Get device properties.
+  devices            List all devices.
+  login              Get user session tokens.
+  urls               Get region information.
 ```
 
 ### From code
 
 ```python
 from karcher.karcher import KarcherHome
```

### Comparing `karcher-home-0.2.1/karcher/auth.py` & `karcher-home-0.3/karcher/auth.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # SPDX-License-Identifier: MIT
 # -----------------------------------------------------------
 
 import base64
 from dataclasses import dataclass, fields
 import json
 
-from karcher.countries import COUNTRIES
 
 @dataclass(init=False)
 class Domains:
     """Domains URLs class.
 
     This class represents a Karcher Home access URLs.
     """
@@ -23,29 +22,28 @@
         for k, v in kwargs.items():
             k = k.lower()
             if k in names:
                 if k == 'app_api':
                     v = 'https://' + v
                 setattr(self, k, v)
 
+
 @dataclass(init=False)
 class Session:
     """Authorized user session class.
-    
+
     This class represents a Karcher Home authorized user session.
     """
 
     register_id: str
     user_id: str
     auth_token: str
     mqtt_token: str
-    country_code: str
 
     def __init__(self, **kwargs):
-        setattr(self, 'country_code', None)
         names = set([f.name for f in fields(self)])
         if 'id' in kwargs:
             setattr(self, 'user_id', kwargs['id'])
         if 'data' in kwargs:
             kwargs = kwargs['data']
         for k, v in kwargs.items():
             k = k.lower()
@@ -58,20 +56,14 @@
 
     def reset(self):
         """Reset session."""
         self.user_id = ''
         self.auth_token = ''
         self.mqtt_token = ''
 
-    def get_country_code(self):
-        """Get country code."""
-        if self.country_code in COUNTRIES:
-            return COUNTRIES[self.country_code]
-        return self.country_code
-
     @staticmethod
     def from_token(auth_token: str, mqtt_token: str):
         """Create session from auth and MQTT tokens."""
         sess = Session()
 
         # Get user ID from auth token
         token_data = auth_token.split(".")[1]
```

### Comparing `karcher-home-0.2.1/karcher/cli.py` & `karcher-home-0.3/karcher/cli.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.2.1/karcher/consts.py` & `karcher-home-0.3/karcher/consts.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.2.1/karcher/device.py` & `karcher-home-0.3/karcher/device.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,21 +138,27 @@
     quiet_status: DevicePropertiesQuiet = DevicePropertiesQuiet()
     last_update_time: int = 0
 
     def __init__(self, **kwargs):
         setattr(self, 'cur_path', [])
         self.update(kwargs)
 
-    def update(self, data: dict[str, Any]):
+    def update(self, data: dict[str, Any]) -> bool:
+        """Update device properties."""
+
+        updated = False
         names = set([f.name for f in fields(self)])
         for k, v in data.items():
             if k in names:
                 if k == 'firmware_code':
                     v = int(v)
-                setattr(self, k, v)
+                if v != getattr(self, k):
+                    setattr(self, k, v)
+                    updated = True
+        return updated
 
 
 @dataclass(init=False)
 class Device:
     """Device class.
 
     This class represents a Karcher Home device.
@@ -193,8 +199,9 @@
                 elif k == 'versions':
                     v = json.loads(v)
                     v = [DeviceVersion(**x) for x in v]
                 setattr(self, k, v)
 
     def is_online(self):
         """Get device status."""
+
         return self.status == DeviceStatus.Online
```

### Comparing `karcher-home-0.2.1/karcher/identifiers.py` & `karcher-home-0.3/karcher/identifiers.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.2.1/karcher/karcher.py` & `karcher-home-0.3/karcher/karcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,52 +2,56 @@
 # Copyright (c) 2023 Lauris BH
 # SPDX-License-Identifier: MIT
 # -----------------------------------------------------------
 
 import collections
 import json
 import threading
+from typing import List, Any
 import requests
 import urllib.parse
 
+
 from .auth import Domains, Session
+from .countries import get_country_code, get_region_by_country
 from .consts import APP_VERSION_CODE, APP_VERSION_NAME, PROJECT_TYPE, \
     PROTOCOL_VERSION, REGION_URLS, ROBOT_PROPERTIES, TENANT_ID, \
-    Region, Language
+    Language
 from .device import Device, DeviceProperties
 from .exception import KarcherHomeAccessDenied, KarcherHomeException, handle_error_code
 from .map import Map
 from .mqtt import MqttClient, get_device_topic_property_get_reply, get_device_topics
 from .utils import decrypt, decrypt_map, encrypt, get_nonce, get_random_string, \
     get_timestamp, get_timestamp_ms, is_email, md5
 
 
 class KarcherHome:
     """Main class to access Karcher Home Robots API"""
 
-    def __init__(self, region: Region = Region.EU):
+    def __init__(self, country: str = 'GB', language: Language = Language.EN):
         """Initialize Karcher Home Robots API"""
 
         super().__init__()
-        self._base_url = REGION_URLS[region]
+        self._country = country.upper()
+        self._base_url = REGION_URLS[get_region_by_country(self._country)]
         self._mqtt_url = None
-        self._language = Language.EN
+        self._language = language
         self._session = None
         self._mqtt = None
         self._device_props = {}
         self._wait_events = {}
 
         d = self.get_urls()
         # Update base URLs
         if d.app_api != '':
             self._base_url = d.app_api
         if d.mqtt != '':
             self._mqtt_url = d.mqtt
 
-    def _request(self, method: str, url: str, **kwargs):
+    def _request(self, method: str, url: str, **kwargs) -> requests.Response:
         session = requests.Session()
         # TODO: Fix SSL
         requests.packages.urllib3.disable_warnings()
         session.verify = False
 
         headers = {}
         if kwargs.get('headers') is not None:
@@ -92,28 +96,28 @@
         headers['sign'] = md5(auth + ts + nonce + data)
         headers['ts'] = ts
         headers['nonce'] = nonce
 
         kwargs['headers'] = headers
         return session.request(method, self._base_url + url, **kwargs)
 
-    def _download(self, url):
+    def _download(self, url) -> bytes:
         session = requests.Session()
         headers = {
             'User-Agent': 'Android_' + TENANT_ID,
         }
 
         resp = session.get(url, headers=headers)
         if resp.status_code != 200:
             raise KarcherHomeException(-1,
                                        'HTTP error: ' + str(resp.status_code))
 
         return resp.content
 
-    def _process_response(self, resp, prop=None):
+    def _process_response(self, resp, prop=None) -> Any:
         if resp.status_code != 200:
             raise KarcherHomeException(-1,
                                        'HTTP error: ' + str(resp.status_code))
         data = resp.json()
         # Check for error response
         if data['code'] != 0:
             handle_error_code(data['code'], data['msg'])
@@ -153,27 +157,27 @@
         self._mqtt.connect()
         self._mqtt.on_message = self._process_mqtt_message
 
         if wait_for_connect:
             event.wait()
             self._mqtt.on_connect = None
 
-    def get_urls(self):
+    def get_urls(self) -> Domains:
         """Get URLs for API and MQTT."""
 
         resp = self._request('GET', '/network-service/domains/list', params={
             'tenantId': TENANT_ID,
             'productModeCode': PROJECT_TYPE,
             'version': PROTOCOL_VERSION,
         })
 
         d = self._process_response(resp, 'domain')
         return Domains(**d)
 
-    def login(self, username, password, register_id=None):
+    def login(self, username, password, register_id=None) -> Session:
         """Login using provided credentials."""
 
         if register_id is None or register_id == '':
             register_id = get_random_string(19)
 
         if not is_email(username):
             username = '86-' + username
@@ -199,15 +203,19 @@
 
         d = self._process_response(resp)
         self._session = Session(**d)
         self._session.register_id = register_id
 
         return self._session
 
-    def login_token(self, auth_token: str, mqtt_token: str, register_id=None):
+    def login_token(
+            self,
+            auth_token: str,
+            mqtt_token: str,
+            register_id=None) -> Session:
         """Login using provided tokens."""
 
         if register_id is None or register_id == '':
             register_id = get_random_string(19)
 
         self._session = Session.from_token(auth_token, mqtt_token)
         self._session.register_id = register_id
@@ -228,15 +236,15 @@
             'POST', '/user-center/auth/logout'))
         self._session = None
 
         if self._mqtt is not None:
             self._mqtt.disconnect()
             self._mqtt = None
 
-    def get_devices(self):
+    def get_devices(self) -> List[Device]:
         """Get all user devices."""
 
         if self._session is None \
                 or self._session.auth_token == '' or self._session.user_id == '':
             raise KarcherHomeAccessDenied('Not authorized')
 
         resp = self._request(
@@ -252,15 +260,15 @@
             dev.sn + '/01-01-2022/map/temp/0046690461_' + \
             dev.sn + '_' + str(map)
 
         resp = self._request('POST',
                              '/storage-management/storage/aws/getAccessUrl',
                              json={
                                  'dir': mapDir,
-                                 'countryCode': self._session.get_country_code(),
+                                 'countryCode': get_country_code(self._country),
                                  'serviceType': 2,
                                  'tenantId': TENANT_ID,
                              })
 
         d = self._process_response(resp)
         downloadUrl = d['url']
         if 'cdnDomain' in d and d['cdnDomain'] != '':
@@ -366,15 +374,15 @@
                 "tenantId": TENANT_ID,
                 "version": "3.0",
                 "params": {
                     "property": ROBOT_PROPERTIES,
                 },
             }))
 
-    def get_device_properties(self, dev: Device):
+    def get_device_properties(self, dev: Device) -> DeviceProperties:
         """Get device properties if it has subscription."""
 
         if dev.sn in self._device_props:
             return self._device_props[dev.sn]
 
         if self._session is None \
                 or self._session.mqtt_token == '' or self._session.user_id == '':
```

### Comparing `karcher-home-0.2.1/karcher/map.py` & `karcher-home-0.3/karcher/map.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.2.1/karcher/mapdata_pb2.py` & `karcher-home-0.3/karcher/mapdata_pb2.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.2.1/karcher/mqtt.py` & `karcher-home-0.3/karcher/mqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import List
 import ssl
 from paho.mqtt.client import Client, MQTTv311
 
 from .utils import get_random_device_id
 
 
 class MqttClient:
@@ -72,24 +73,24 @@
         if self.on_message is not None:
             self.on_message(msg.topic, msg.payload)
 
     def __del__(self):
         self.disconnect()
 
 
-def get_device_topics(product_id: str, sn: str):
+def get_device_topics(product_id: str, sn: str) -> List[str]:
     return [
         '/mqtt/' + product_id + '/' + sn + '/thing/event/property/post',
         '/mqtt/' + product_id + '/' + sn + '/thing/service/property/set_reply',
         get_device_topic_property_get_reply(product_id, sn),
         '/mqtt/' + product_id + '/' + sn + '/thing/service_invoke',
         '/mqtt/' + product_id + '/' + sn + '/thing/service_invoke_reply/#',
         '/mqtt/' + product_id + '/' + sn + '/thing/event/cur_path/post',
         '/mqtt/' + product_id + '/' + sn + '/ota/service/upgrade/set_reply',
         '/mqtt/' + product_id + '/' + sn + '/ota/service/upgrade/post',
         '/mqtt/' + product_id + '/' + sn + '/ota/service/upgrade/get_reply',
         '/mqtt/' + product_id + '/' + sn + '/ota/service/version/post',
     ]
 
 
-def get_device_topic_property_get_reply(product_id: str, sn: str):
+def get_device_topic_property_get_reply(product_id: str, sn: str) -> str:
     return '/mqtt/' + product_id + '/' + sn + '/thing/service/property/get_reply'
```

### Comparing `karcher-home-0.2.1/karcher/utils.py` & `karcher-home-0.3/karcher/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,105 +5,106 @@
 
 import base64
 import hashlib
 import random
 import re
 import string
 import time
+from typing import Final
 import zlib
 from Crypto.Cipher import AES
 
 from .consts import TENANT_ID, Product
 
 
-EMAIL_REGEX = "^\\w+([-+.]\\w+)*@\\w+([-.]\\w+)*\\.\\w+([-.]\\w+)*$"
+EMAIL_REGEX: Final = "^\\w+([-+.]\\w+)*@\\w+([-.]\\w+)*\\.\\w+([-.]\\w+)*$"
 
 
-def get_random_string(length):
+def get_random_string(length: int) -> str:
     letters = string.digits + string.ascii_lowercase + string.ascii_uppercase
     return ''.join(random.choice(letters) for i in range(length))
 
 
-def get_random_device_id():
+def get_random_device_id() -> str:
     return ''.join(random.choice('0123456789abcdef') for i in range(16))
 
 
-def get_nonce():
+def get_nonce() -> str:
     return get_random_string(32)
 
 
-def get_timestamp():
+def get_timestamp() -> int:
     return int(time.time())
 
 
-def get_timestamp_ms():
+def get_timestamp_ms() -> int:
     return int(time.time() * 1000)
 
 
-def get_enc_key():
+def get_enc_key() -> bytes:
     m = hashlib.md5()
     m.update(bytes(TENANT_ID, 'utf-8'))
     h = m.hexdigest()
     return bytes(h[8:24], 'utf-8')
 
 
-def decrypt(data):
+def decrypt(data) -> str:
     cipher = AES.new(get_enc_key(), AES.MODE_ECB)
     buf = cipher.decrypt(base64.b64decode(data))
     return str(buf[:-ord(buf[-1:])], 'utf-8')
 
 
-def encrypt(data):
+def encrypt(data) -> str:
     cipher = AES.new(get_enc_key(), AES.MODE_ECB)
     buf = bytes(data, 'utf-8')
     pad_len = cipher.block_size - (len(buf) % cipher.block_size)
     buf = buf + bytes([pad_len]) * pad_len
     return base64.b64encode(cipher.encrypt(buf)).decode()
 
 
-def get_map_enc_key(sn: str, mac: str, product_id: Product):
+def get_map_enc_key(sn: str, mac: str, product_id: Product) -> bytes:
     sub_key = mac.replace(':', '').lower() + str(product_id.value)
     cipher = AES.new(bytes(sub_key[0:16], 'utf-8'), AES.MODE_ECB)
     buf = bytes(sn + '+' + str(product_id.value) + '+' + sn, 'utf-8')
     pad_len = cipher.block_size - (len(buf) % cipher.block_size)
     buf = buf + bytes([pad_len]) * pad_len
 
     key = base64.b64encode(cipher.encrypt(buf)).decode()
 
     m = hashlib.md5()
     m.update(bytes(key, 'utf-8'))
     h = m.hexdigest()
     return bytes(h[8:24], 'utf-8')
 
 
-def decrypt_map(sn: str, mac: str, product_id: Product, data: bytes):
+def decrypt_map(sn: str, mac: str, product_id: Product, data: bytes) -> bytes:
     cipher = AES.new(get_map_enc_key(sn, mac, product_id), AES.MODE_ECB)
     buf = cipher.decrypt(base64.b64decode(data))
     try:
         return zlib.decompress(bytes.fromhex(str(buf[:-ord(buf[-1:])], 'utf-8')))
     except Exception:
         return bytes.fromhex(str(buf[:-ord(buf[-1:])], 'utf-8'))
 
 
-def md5(data):
+def md5(data: str) -> str:
     m = hashlib.md5()
     m.update(bytes(data, 'utf-8'))
     return m.hexdigest()
 
 
-def is_email(email):
+def is_email(email: str) -> bool:
     return re.search(EMAIL_REGEX, email) is not None
 
 
-def snake_case(value):
+def snake_case(value: str) -> str:
     first_underscore = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', value)
     return re.sub('([a-z0-9])([A-Z])', r'\1_\2', first_underscore).lower()
 
 
-def snake_case_fields(data):
+def snake_case_fields(data: str) -> str:
     if type(data) is dict:
         n = {}
         for k, v in data.items():
             n[snake_case(k)] = snake_case_fields(v)
         return n
     elif type(data) is list:
         n = []
```

### Comparing `karcher-home-0.2.1/karcher_home.egg-info/PKG-INFO` & `karcher-home-0.3/karcher_home.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: karcher-home
-Version: 0.2.1
+Version: 0.3
 Summary: Kärcher Home Robots client
 Home-page: https://github.com/lafriks/python-karcher
-Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.2.1/karcher-home-0.2.1.tar.gz
+Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.3/karcher-home-0.3.tar.gz
 Author: Lauris BH
 Author-email: lauris@nix.lv
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -27,23 +27,25 @@
 
 ```console
 Usage: karcher-home [OPTIONS] COMMAND [ARGS]...
 
   Tool for connectiong and getting information from Kärcher Home Robots.
 
 Options:
-  -d, --debug
+  -d, --debug                     Enable debug mode.
   -o, --output [json|json_pretty]
-  -r, --region [eu|us|cn]         Region of the server to query. Default: 'eu'
+                                  Output format. Default: "json"
+  -r, --region [eu|us|cn]         Region of the server to query. Default: "eu"
   --help                          Show this message and exit.
 
 Commands:
-  devices   List all devices.
-  get-urls  Get region information.
-  login     Get user session tokens.
+  device-properties  Get device properties.
+  devices            List all devices.
+  login              Get user session tokens.
+  urls               Get region information.
 ```
 
 ### From code
 
 ```python
 from karcher.karcher import KarcherHome
```

### Comparing `karcher-home-0.2.1/karcher_home.egg-info/SOURCES.txt` & `karcher-home-0.3/karcher_home.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `karcher-home-0.2.1/setup.py` & `karcher-home-0.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 except ImportError:
     from distutils.core import setup
 
 setup(
     name='karcher-home',
     packages=['karcher'],
     include_package_data=True,
-    version='0.2.1',
+    version='0.3',
     license='MIT',
     description='Kärcher Home Robots client',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Lauris BH',
     author_email='lauris@nix.lv',
     url='https://github.com/lafriks/python-karcher',
-    download_url='https://github.com/lafriks/python-karcher/releases/download/v0.2.1/karcher-home-0.2.1.tar.gz',
+    download_url='https://github.com/lafriks/python-karcher/releases/download/v0.3/karcher-home-0.3.tar.gz',
     platforms='any',
     install_requires=[
         'requests',
         'tzlocal',
         'click',
         'pycryptodome',
         'protobuf'
```

### Comparing `karcher-home-0.2.1/tests/test_enc.py` & `karcher-home-0.3/tests/test_enc.py`

 * *Files identical despite different names*

