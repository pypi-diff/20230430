# Comparing `tmp/tls_client-0.2.tar.gz` & `tmp/tls_client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tls_client-0.2.tar", last modified: Wed Mar 29 14:29:25 2023, max compression
+gzip compressed data, was "tls_client-0.2.1.tar", last modified: Sun Apr 30 10:23:07 2023, max compression
```

## Comparing `tls_client-0.2.tar` & `tls_client-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 14:29:25.927533 tls_client-0.2/
--rw-rw-rw-   0        0        0     1091 2022-09-21 09:12:33.000000 tls_client-0.2/LICENSE
--rw-rw-rw-   0        0        0     4587 2023-03-29 14:29:25.926985 tls_client-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3756 2023-03-17 19:21:33.000000 tls_client-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-03-29 14:29:25.927987 tls_client-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1432 2022-09-21 09:13:17.000000 tls_client-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-29 14:29:25.919479 tls_client-0.2/tls_client/
--rw-rw-rw-   0        0        0      669 2022-09-17 17:10:40.000000 tls_client-0.2/tls_client/__init__.py
--rw-rw-rw-   0        0        0      393 2023-03-29 14:28:53.000000 tls_client-0.2/tls_client/__version__.py
--rw-rw-rw-   0        0        0      896 2023-03-29 14:28:43.000000 tls_client-0.2/tls_client/cffi.py
--rw-rw-rw-   0        0        0    15867 2022-09-17 17:08:37.000000 tls_client-0.2/tls_client/cookies.py
-drwxrwxrwx   0        0        0        0 2023-03-29 14:29:25.925984 tls_client-0.2/tls_client/dependencies/
--rw-rw-rw-   0        0        0        0 2022-09-17 19:59:30.000000 tls_client-0.2/tls_client/dependencies/__init__.py
--rw-rw-rw-   0        0        0       80 2022-09-17 17:19:08.000000 tls_client-0.2/tls_client/exceptions.py
--rw-rw-rw-   0        0        0     2493 2023-03-17 20:28:53.000000 tls_client-0.2/tls_client/response.py
--rw-rw-rw-   0        0        0    16640 2023-03-29 14:28:43.000000 tls_client-0.2/tls_client/sessions.py
--rw-rw-rw-   0        0        0     2517 2022-09-17 16:56:57.000000 tls_client-0.2/tls_client/structures.py
-drwxrwxrwx   0        0        0        0 2023-03-29 14:29:25.924984 tls_client-0.2/tls_client.egg-info/
--rw-rw-rw-   0        0        0     4587 2023-03-29 14:29:25.000000 tls_client-0.2/tls_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-03-29 14:29:25.000000 tls_client-0.2/tls_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 14:29:25.000000 tls_client-0.2/tls_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-03-29 14:29:25.000000 tls_client-0.2/tls_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 10:23:07.852206 tls_client-0.2.1/
+-rw-rw-rw-   0        0        0     1091 2022-09-21 09:12:33.000000 tls_client-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4626 2023-04-30 10:23:07.851475 tls_client-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3792 2023-04-30 10:21:11.000000 tls_client-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 10:23:07.852206 tls_client-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1432 2022-09-21 09:13:17.000000 tls_client-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:23:07.839744 tls_client-0.2.1/tls_client/
+-rw-rw-rw-   0        0        0      669 2022-09-17 17:10:40.000000 tls_client-0.2.1/tls_client/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-04-30 10:17:20.000000 tls_client-0.2.1/tls_client/__version__.py
+-rw-rw-rw-   0        0        0      896 2023-03-29 14:28:43.000000 tls_client-0.2.1/tls_client/cffi.py
+-rw-rw-rw-   0        0        0    15867 2022-09-17 17:08:37.000000 tls_client-0.2.1/tls_client/cookies.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:23:07.850851 tls_client-0.2.1/tls_client/dependencies/
+-rw-rw-rw-   0        0        0        0 2022-09-17 19:59:30.000000 tls_client-0.2.1/tls_client/dependencies/__init__.py
+-rw-rw-rw-   0        0        0       80 2022-09-17 17:19:08.000000 tls_client-0.2.1/tls_client/exceptions.py
+-rw-rw-rw-   0        0        0     2493 2023-03-17 20:28:53.000000 tls_client-0.2.1/tls_client/response.py
+-rw-rw-rw-   0        0        0    17298 2023-04-30 10:14:24.000000 tls_client-0.2.1/tls_client/sessions.py
+-rw-rw-rw-   0        0        0     2517 2022-09-17 16:56:57.000000 tls_client-0.2.1/tls_client/structures.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:23:07.849850 tls_client-0.2.1/tls_client.egg-info/
+-rw-rw-rw-   0        0        0     4626 2023-04-30 10:23:07.000000 tls_client-0.2.1/tls_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-04-30 10:23:07.000000 tls_client-0.2.1/tls_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 10:23:07.000000 tls_client-0.2.1/tls_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-30 10:23:07.000000 tls_client-0.2.1/tls_client.egg-info/top_level.txt
```

### Comparing `tls_client-0.2/LICENSE` & `tls_client-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tls_client-0.2/PKG-INFO` & `tls_client-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tls_client
-Version: 0.2
+Version: 0.2.1
 Summary: Advanced Python HTTP Client.
 Home-page: UNKNOWN
 Author: Florian Zager
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -31,25 +31,26 @@
 The syntax is inspired by [requests](https://github.com/psf/requests), so its very similar and there are only very few things that are different.
 
 Example 1 - Preset:
 ```python
 import tls_client
 
 # You can also use the following as `client_identifier`:
-# Chrome --> chrome_103, chrome_104, chrome_105, chrome_106, chrome_107, chrome_108, chrome109, Chrome110
+# Chrome --> chrome_103, chrome_104, chrome_105, chrome_106, chrome_107, chrome_108, chrome109, Chrome110,
+#            chrome111, chrome112
 # Firefox --> firefox_102, firefox_104, firefox108, Firefox110
 # Opera --> opera_89, opera_90
 # Safari --> safari_15_3, safari_15_6_1, safari_16_0
 # iOS --> safari_ios_15_5, safari_ios_15_6, safari_ios_16_0
 # iPadOS --> safari_ios_15_6
 # Android --> okhttp4_android_7, okhttp4_android_8, okhttp4_android_9, okhttp4_android_10, okhttp4_android_11,
 #             okhttp4_android_12, okhttp4_android_13
 
 session = tls_client.Session(
-    client_identifier="chrome110",
+    client_identifier="chrome112",
     random_tls_extension_order=True
 )
 
 res = session.get(
     "https://www.example.com/",
     headers={
         "key1": "value1",
```

### Comparing `tls_client-0.2/README.md` & `tls_client-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 The syntax is inspired by [requests](https://github.com/psf/requests), so its very similar and there are only very few things that are different.
 
 Example 1 - Preset:
 ```python
 import tls_client
 
 # You can also use the following as `client_identifier`:
-# Chrome --> chrome_103, chrome_104, chrome_105, chrome_106, chrome_107, chrome_108, chrome109, Chrome110
+# Chrome --> chrome_103, chrome_104, chrome_105, chrome_106, chrome_107, chrome_108, chrome109, Chrome110,
+#            chrome111, chrome112
 # Firefox --> firefox_102, firefox_104, firefox108, Firefox110
 # Opera --> opera_89, opera_90
 # Safari --> safari_15_3, safari_15_6_1, safari_16_0
 # iOS --> safari_ios_15_5, safari_ios_15_6, safari_ios_16_0
 # iPadOS --> safari_ios_15_6
 # Android --> okhttp4_android_7, okhttp4_android_8, okhttp4_android_9, okhttp4_android_10, okhttp4_android_11,
 #             okhttp4_android_12, okhttp4_android_13
 
 session = tls_client.Session(
-    client_identifier="chrome110",
+    client_identifier="chrome112",
     random_tls_extension_order=True
 )
 
 res = session.get(
     "https://www.example.com/",
     headers={
         "key1": "value1",
```

### Comparing `tls_client-0.2/setup.py` & `tls_client-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `tls_client-0.2/tls_client/__init__.py` & `tls_client-0.2.1/tls_client/__init__.py`

 * *Files identical despite different names*

### Comparing `tls_client-0.2/tls_client/cffi.py` & `tls_client-0.2.1/tls_client/cffi.py`

 * *Files identical despite different names*

### Comparing `tls_client-0.2/tls_client/cookies.py` & `tls_client-0.2.1/tls_client/cookies.py`

 * *Files identical despite different names*

### Comparing `tls_client-0.2/tls_client/response.py` & `tls_client-0.2.1/tls_client/response.py`

 * *Files identical despite different names*

### Comparing `tls_client-0.2/tls_client/sessions.py` & `tls_client-0.2.1/tls_client/sessions.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         connection_flow: Optional[int] = None,
         priority_frames: Optional[list] = None,
         header_order: Optional[list] = None,  # Optional[list[str]]
         header_priority: Optional[dict] = None,  # Optional[list[str]]
         random_tls_extension_order: Optional = False,
         force_http1: Optional = False,
         catch_panics: Optional = False,
+        debug: Optional = False
     ) -> None:
         self._session_id = str(uuid.uuid4())
         # --- Standard Settings ----------------------------------------------------------------------------------------
 
         # Case-insensitive dictionary of headers, send on each request
         self.headers = CaseInsensitiveDict(
             {
@@ -59,14 +60,17 @@
         # Dictionary of querystring data to attach to each request. The dictionary values may be lists for representing
         # multivalued query parameters.
         self.params = {}
 
         # CookieJar containing all currently outstanding cookies set on this session
         self.cookies = cookiejar_from_dict({})
 
+        # Timeout
+        self.timeout_seconds = 30
+
         # --- Advanced Settings ----------------------------------------------------------------------------------------
 
         # Examples:
         # Chrome --> chrome_103, chrome_104, chrome_105, chrome_106
         # Firefox --> firefox_102, firefox_104
         # Opera --> opera_89, opera_90
         # Safari --> safari_15_3, safari_15_6_1, safari_16_0
@@ -260,26 +264,29 @@
         # force HTTP1
         self.force_http1 = force_http1
 
         # catch panics
         # avoid the tls client to print the whole stacktrace when a panic (critical go error) happens
         self.catch_panics = catch_panics
 
+        # debugging
+        self.debug = debug
+
     def execute_request(
         self,
         method: str,
         url: str,
         params: Optional[dict] = None,  # Optional[dict[str, str]]
         data: Optional[Union[str, dict]] = None,
         headers: Optional[dict] = None,  # Optional[dict[str, str]]
         cookies: Optional[dict] = None,  # Optional[dict[str, str]]
         json: Optional[dict] = None,  # Optional[dict]
         allow_redirects: Optional[bool] = False,
         insecure_skip_verify: Optional[bool] = False,
-        timeout_seconds: Optional[int] = 30,
+        timeout_seconds: Optional[int] = None,
         proxy: Optional[dict] = None  # Optional[dict[str, str]]
     ):
         # --- URL ------------------------------------------------------------------------------------------------------
         # Prepare URL - add params to url
         if params is not None:
             url = f"{url}?{urllib.parse.urlencode(params, doseq=True)}"
 
@@ -298,50 +305,62 @@
             request_body = data
             content_type = None
         # set content type if it isn't set
         if content_type is not None and "content-type" not in self.headers:
             self.headers["Content-Type"] = content_type
 
         # --- Headers --------------------------------------------------------------------------------------------------
-        # merge headers of session and of the request
-        if headers is not None:
-            for header_key, header_value in headers.items():
-                # check if all header keys and values are strings
-                if type(header_key) is str and type(header_value) is str:
-                    self.headers[header_key] = header_value
-                headers = self.headers
-        else:
+        if self.headers is None:
+            headers = CaseInsensitiveDict(headers)
+        elif headers is None:
             headers = self.headers
+        else:
+            merged_headers = CaseInsensitiveDict(self.headers)
+            merged_headers.update(headers)
+
+            # Remove items, where the key or value is set to None.
+            none_keys = [k for (k, v) in merged_headers.items() if v is None or k is None]
+            for key in none_keys:
+                del merged_headers[key]
+
+            headers = merged_headers
 
         # --- Cookies --------------------------------------------------------------------------------------------------
         cookies = cookies or {}
         # Merge with session cookies
         cookies = merge_cookies(self.cookies, cookies)
         # turn cookie jar into dict
+        # in the cookie value the " gets removed, because the fhttp library in golang doesn't accept the character
         request_cookies = [
-            {'domain': c.domain, 'expires': c.expires, 'name': c.name, 'path': c.path, 'value': c.value}
+            {'domain': c.domain, 'expires': c.expires, 'name': c.name, 'path': c.path, 'value': c.value.replace('"', "")}
             for c in cookies
         ]
 
         # --- Proxy ----------------------------------------------------------------------------------------------------
         proxy = proxy or self.proxies
         
         if type(proxy) is dict and "http" in proxy:
             proxy = proxy["http"]
         elif type(proxy) is str:
             proxy = proxy
         else:
             proxy = ""
 
+        # --- Timeout --------------------------------------------------------------------------------------------------
+        # maximum time to wait
+
+        timeout_seconds = timeout_seconds or self.timeout_seconds
+        
         # --- Request --------------------------------------------------------------------------------------------------
         is_byte_request = isinstance(request_body, (bytes, bytearray))
         request_payload = {
             "sessionId": self._session_id,
             "followRedirects": allow_redirects,
             "forceHttp1": self.force_http1,
+            "withDebug": self.debug,
             "catchPanics": self.catch_panics,
             "headers": dict(headers),
             "headerOrder": self.header_order,
             "insecureSkipVerify": insecure_skip_verify,
             "isByteRequest": is_byte_request,
             "additionalDecode": self.additional_decode,
             "proxyUrl": proxy,
@@ -441,15 +460,15 @@
     def patch(
         self,
         url: str,
         data: Optional[Union[str, dict]] = None,
         json: Optional[dict] = None,
         **kwargs: Any
     ):
-        """Sends a PUT request"""
+        """Sends a PATCH request"""
         return self.execute_request(method="PATCH", url=url, data=data, json=json, **kwargs)
 
     def delete(
         self,
         url: str,
         **kwargs: Any
     ):
```

### Comparing `tls_client-0.2/tls_client/structures.py` & `tls_client-0.2.1/tls_client/structures.py`

 * *Files identical despite different names*

### Comparing `tls_client-0.2/tls_client.egg-info/PKG-INFO` & `tls_client-0.2.1/tls_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tls-client
-Version: 0.2
+Version: 0.2.1
 Summary: Advanced Python HTTP Client.
 Home-page: UNKNOWN
 Author: Florian Zager
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -31,25 +31,26 @@
 The syntax is inspired by [requests](https://github.com/psf/requests), so its very similar and there are only very few things that are different.
 
 Example 1 - Preset:
 ```python
 import tls_client
 
 # You can also use the following as `client_identifier`:
-# Chrome --> chrome_103, chrome_104, chrome_105, chrome_106, chrome_107, chrome_108, chrome109, Chrome110
+# Chrome --> chrome_103, chrome_104, chrome_105, chrome_106, chrome_107, chrome_108, chrome109, Chrome110,
+#            chrome111, chrome112
 # Firefox --> firefox_102, firefox_104, firefox108, Firefox110
 # Opera --> opera_89, opera_90
 # Safari --> safari_15_3, safari_15_6_1, safari_16_0
 # iOS --> safari_ios_15_5, safari_ios_15_6, safari_ios_16_0
 # iPadOS --> safari_ios_15_6
 # Android --> okhttp4_android_7, okhttp4_android_8, okhttp4_android_9, okhttp4_android_10, okhttp4_android_11,
 #             okhttp4_android_12, okhttp4_android_13
 
 session = tls_client.Session(
-    client_identifier="chrome110",
+    client_identifier="chrome112",
     random_tls_extension_order=True
 )
 
 res = session.get(
     "https://www.example.com/",
     headers={
         "key1": "value1",
```

