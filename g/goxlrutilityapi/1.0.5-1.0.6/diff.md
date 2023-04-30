# Comparing `tmp/goxlrutilityapi-1.0.5.tar.gz` & `tmp/goxlrutilityapi-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlrutilityapi-1.0.5.tar", last modified: Sun Apr 30 12:53:11 2023, max compression
+gzip compressed data, was "goxlrutilityapi-1.0.6.tar", last modified: Sun Apr 30 14:01:18 2023, max compression
```

## Comparing `goxlrutilityapi-1.0.5.tar` & `goxlrutilityapi-1.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:53:11.324543 goxlrutilityapi-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 12:53:11.324543 goxlrutilityapi-1.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:53:11.324543 goxlrutilityapi-1.0.5/goxlrutilityapi/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:53:11.324543 goxlrutilityapi-1.0.5/goxlrutilityapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/models/map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:53:11.324543 goxlrutilityapi-1.0.5/goxlrutilityapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 12:53:11.000000 goxlrutilityapi-1.0.5/goxlrutilityapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-30 12:53:11.000000 goxlrutilityapi-1.0.5/goxlrutilityapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:53:11.000000 goxlrutilityapi-1.0.5/goxlrutilityapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 12:53:11.000000 goxlrutilityapi-1.0.5/goxlrutilityapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 12:53:11.000000 goxlrutilityapi-1.0.5/goxlrutilityapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 12:53:11.324543 goxlrutilityapi-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:01:18.893212 goxlrutilityapi-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 14:01:18.893212 goxlrutilityapi-1.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:01:18.893212 goxlrutilityapi-1.0.6/goxlrutilityapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:01:18.893212 goxlrutilityapi-1.0.6/goxlrutilityapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/models/map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:01:18.893212 goxlrutilityapi-1.0.6/goxlrutilityapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 14:01:18.000000 goxlrutilityapi-1.0.6/goxlrutilityapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-30 14:01:18.000000 goxlrutilityapi-1.0.6/goxlrutilityapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 14:01:18.000000 goxlrutilityapi-1.0.6/goxlrutilityapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 14:01:18.000000 goxlrutilityapi-1.0.6/goxlrutilityapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 14:01:18.000000 goxlrutilityapi-1.0.6/goxlrutilityapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 14:01:18.893212 goxlrutilityapi-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/setup.py
```

### Comparing `goxlrutilityapi-1.0.5/goxlrutilityapi/__main__.py` & `goxlrutilityapi-1.0.6/goxlrutilityapi/__main__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.5/goxlrutilityapi/const.py` & `goxlrutilityapi-1.0.6/goxlrutilityapi/const.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.5/goxlrutilityapi/helper.py` & `goxlrutilityapi-1.0.6/goxlrutilityapi/helper.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.5/goxlrutilityapi/models/status.py` & `goxlrutilityapi-1.0.6/goxlrutilityapi/models/status.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.5/goxlrutilityapi/websocket_client.py` & `goxlrutilityapi-1.0.6/goxlrutilityapi/websocket_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,20 +78,15 @@
         try:
             self._websocket = await self._session.ws_connect(url=url, heartbeat=30)
         except (
             aiohttp.WSServerHandshakeError,
             aiohttp.ClientConnectionError,
             socket.gaierror,
         ) as error:
-            self._logger.warning(
-                "Failed to connect to WebSocket: %s - %s",
-                error.__class__.__name__,
-                error,
-            )
-            raise ConnectionErrorException from error
+            raise ConnectionErrorException(error) from error
         self._logger.info("Connected to WebSocket")
 
     async def _send_message(
         self,
         request: Request,
         wait_for_response: bool = True,
         response_type: Optional[str] = None,
```

### Comparing `goxlrutilityapi-1.0.5/goxlrutilityapi.egg-info/SOURCES.txt` & `goxlrutilityapi-1.0.6/goxlrutilityapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.5/pyproject.toml` & `goxlrutilityapi-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.5/setup.py` & `goxlrutilityapi-1.0.6/setup.py`

 * *Files identical despite different names*

