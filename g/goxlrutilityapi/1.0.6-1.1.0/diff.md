# Comparing `tmp/goxlrutilityapi-1.0.6.tar.gz` & `tmp/goxlrutilityapi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlrutilityapi-1.0.6.tar", last modified: Sun Apr 30 14:01:18 2023, max compression
+gzip compressed data, was "goxlrutilityapi-1.1.0.tar", last modified: Sun Apr 30 16:06:32 2023, max compression
```

## Comparing `goxlrutilityapi-1.0.6.tar` & `goxlrutilityapi-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:01:18.893212 goxlrutilityapi-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 14:01:18.893212 goxlrutilityapi-1.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:01:18.893212 goxlrutilityapi-1.0.6/goxlrutilityapi/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:01:18.893212 goxlrutilityapi-1.0.6/goxlrutilityapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/models/map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/goxlrutilityapi/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:01:18.893212 goxlrutilityapi-1.0.6/goxlrutilityapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 14:01:18.000000 goxlrutilityapi-1.0.6/goxlrutilityapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-30 14:01:18.000000 goxlrutilityapi-1.0.6/goxlrutilityapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 14:01:18.000000 goxlrutilityapi-1.0.6/goxlrutilityapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 14:01:18.000000 goxlrutilityapi-1.0.6/goxlrutilityapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 14:01:18.000000 goxlrutilityapi-1.0.6/goxlrutilityapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 14:01:18.893212 goxlrutilityapi-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-30 14:01:07.000000 goxlrutilityapi-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:06:32.790843 goxlrutilityapi-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 16:06:32.790843 goxlrutilityapi-1.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:06:32.790843 goxlrutilityapi-1.1.0/goxlrutilityapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 16:06:16.000000 goxlrutilityapi-1.1.0/goxlrutilityapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-30 16:06:16.000000 goxlrutilityapi-1.1.0/goxlrutilityapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-30 16:06:16.000000 goxlrutilityapi-1.1.0/goxlrutilityapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 16:06:16.000000 goxlrutilityapi-1.1.0/goxlrutilityapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-04-30 16:06:16.000000 goxlrutilityapi-1.1.0/goxlrutilityapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 16:06:16.000000 goxlrutilityapi-1.1.0/goxlrutilityapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-30 16:06:16.000000 goxlrutilityapi-1.1.0/goxlrutilityapi/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-30 16:06:16.000000 goxlrutilityapi-1.1.0/goxlrutilityapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:06:32.790843 goxlrutilityapi-1.1.0/goxlrutilityapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-30 16:06:16.000000 goxlrutilityapi-1.1.0/goxlrutilityapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-30 16:06:16.000000 goxlrutilityapi-1.1.0/goxlrutilityapi/models/map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 16:06:16.000000 goxlrutilityapi-1.1.0/goxlrutilityapi/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-30 16:06:16.000000 goxlrutilityapi-1.1.0/goxlrutilityapi/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-30 16:06:16.000000 goxlrutilityapi-1.1.0/goxlrutilityapi/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-04-30 16:06:16.000000 goxlrutilityapi-1.1.0/goxlrutilityapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-04-30 16:06:16.000000 goxlrutilityapi-1.1.0/goxlrutilityapi/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:06:32.790843 goxlrutilityapi-1.1.0/goxlrutilityapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 16:06:32.000000 goxlrutilityapi-1.1.0/goxlrutilityapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-30 16:06:32.000000 goxlrutilityapi-1.1.0/goxlrutilityapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 16:06:32.000000 goxlrutilityapi-1.1.0/goxlrutilityapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 16:06:32.000000 goxlrutilityapi-1.1.0/goxlrutilityapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 16:06:32.000000 goxlrutilityapi-1.1.0/goxlrutilityapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-30 16:06:16.000000 goxlrutilityapi-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 16:06:32.790843 goxlrutilityapi-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-30 16:06:16.000000 goxlrutilityapi-1.1.0/setup.py
```

### Comparing `goxlrutilityapi-1.0.6/goxlrutilityapi/helper.py` & `goxlrutilityapi-1.1.0/goxlrutilityapi/helper.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.6/goxlrutilityapi/models/status.py` & `goxlrutilityapi-1.1.0/goxlrutilityapi/models/status.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.6/goxlrutilityapi/websocket_client.py` & `goxlrutilityapi-1.1.0/goxlrutilityapi/websocket_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,21 +8,27 @@
 
 import aiohttp
 import async_timeout
 from pydantic import ValidationError
 
 from .base import Base
 from .const import (
+    ACCENT,
+    COMMAND_TYPE_SET_BUTTON_COLOURS,
+    COMMAND_TYPE_SET_FADER_COLOURS,
+    COMMAND_TYPE_SET_SIMPLE_COLOUR,
     DEFAULT_HOST,
     DEFAULT_PORT,
     KEY_DATA,
     KEY_ID,
     KEY_TYPE,
     MODEL_MAP,
+    REQUEST_TYPE_COMMAND,
     REQUEST_TYPE_GET_STATUS,
+    RESPONSE_TYPE_OK,
     RESPONSE_TYPE_PATCH,
     RESPONSE_TYPE_STATUS,
 )
 from .exceptions import (
     BadMessageException,
     ConnectionClosedException,
     ConnectionErrorException,
@@ -36,14 +42,15 @@
 class WebsocketClient(Base):
     """Websocket Client"""
 
     def __init__(self) -> None:
         """Initialize Websocket Client"""
         super().__init__()
         self._current_id: int = 1
+        self._mixer_serial_number: Optional[str] = None
         self._responses: dict[
             int, tuple[asyncio.Future[Response[Any]], Optional[str]]
         ] = {}
         self._session: Optional[aiohttp.ClientSession] = None
         self._websocket: Optional[aiohttp.ClientWebSocketResponse] = None
 
     @property
@@ -125,16 +132,126 @@
             Request(data=REQUEST_TYPE_GET_STATUS),
             wait_for_response=True,
             response_type=RESPONSE_TYPE_STATUS,
         )
         if response.data is None:
             raise BadMessageException("Message data is missing")
         self._logger.debug("Status: %s", response.data)
+        self._mixer_serial_number = next(iter(response.data.mixers.keys()))
         return response.data
 
+    async def set_accent_color(
+        self,
+        color: str,
+    ) -> None:
+        """Set accent color"""
+        if self._mixer_serial_number is None:
+            raise BadMessageException(
+                "Mixer serial number is missing. Call get_status to set this."
+            )
+
+        self._logger.info(
+            "Setting accent color to '%s' for mixer '%s'",
+            color,
+            self._mixer_serial_number,
+        )
+        await self._send_message(
+            Request(
+                data={
+                    REQUEST_TYPE_COMMAND: [
+                        self._mixer_serial_number,
+                        {
+                            COMMAND_TYPE_SET_SIMPLE_COLOUR: [
+                                ACCENT,
+                                color,
+                            ],
+                        },
+                    ]
+                }
+            ),
+            wait_for_response=False,
+            response_type=RESPONSE_TYPE_OK,
+        )
+
+    async def set_button_color(
+        self,
+        name: str,
+        color_one: str,
+        color_two: str,
+    ) -> None:
+        """Set button color"""
+        if self._mixer_serial_number is None:
+            raise BadMessageException(
+                "Mixer serial number is missing. Call get_status to set this."
+            )
+
+        self._logger.info(
+            "Setting button '%s' color to '%s' and '%s' for mixer '%s'",
+            name,
+            color_one,
+            color_two,
+            self._mixer_serial_number,
+        )
+        await self._send_message(
+            Request(
+                data={
+                    REQUEST_TYPE_COMMAND: [
+                        self._mixer_serial_number,
+                        {
+                            COMMAND_TYPE_SET_BUTTON_COLOURS: [
+                                name,
+                                color_one,
+                                color_two,
+                            ],
+                        },
+                    ]
+                }
+            ),
+            wait_for_response=False,
+            response_type=RESPONSE_TYPE_OK,
+        )
+
+    async def set_fader_color(
+        self,
+        name: str,
+        color_top: str,
+        color_bottom: str,
+    ) -> None:
+        """Set fader color"""
+        if self._mixer_serial_number is None:
+            raise BadMessageException(
+                "Mixer serial number is missing. Call get_status to set this."
+            )
+
+        self._logger.info(
+            "Setting fader '%s' color to '%s' and '%s' for mixer '%s'",
+            name,
+            color_top,
+            color_bottom,
+            self._mixer_serial_number,
+        )
+        await self._send_message(
+            Request(
+                data={
+                    REQUEST_TYPE_COMMAND: [
+                        self._mixer_serial_number,
+                        {
+                            COMMAND_TYPE_SET_FADER_COLOURS: [
+                                name,
+                                color_top,
+                                color_bottom,
+                            ],
+                        },
+                    ]
+                }
+            ),
+            wait_for_response=False,
+            response_type=RESPONSE_TYPE_OK,
+        )
+
     async def listen(
         self,
         patch_callback: Optional[Callable[[Response[Patch]], Awaitable[None]]] = None,
     ) -> None:
         """Listen for patches from GoXLR"""
 
         async def _message_callback(message: dict) -> None:
```

### Comparing `goxlrutilityapi-1.0.6/goxlrutilityapi.egg-info/SOURCES.txt` & `goxlrutilityapi-1.1.0/goxlrutilityapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.6/pyproject.toml` & `goxlrutilityapi-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.6/setup.py` & `goxlrutilityapi-1.1.0/setup.py`

 * *Files identical despite different names*

