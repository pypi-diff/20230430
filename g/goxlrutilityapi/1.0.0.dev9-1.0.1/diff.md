# Comparing `tmp/goxlrutilityapi-1.0.0.dev9.tar.gz` & `tmp/goxlrutilityapi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlrutilityapi-1.0.0.dev9.tar", last modified: Sat Apr 29 15:19:07 2023, max compression
+gzip compressed data, was "goxlrutilityapi-1.0.1.tar", last modified: Sun Apr 30 10:46:50 2023, max compression
```

## Comparing `goxlrutilityapi-1.0.0.dev9.tar` & `goxlrutilityapi-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:19:07.143836 goxlrutilityapi-1.0.0.dev9/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 15:19:07.143836 goxlrutilityapi-1.0.0.dev9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:19:07.143836 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-29 15:19:05.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:19:07.143836 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:19:07.143836 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 15:19:07.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-29 15:19:07.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:19:07.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-29 15:19:07.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 15:19:07.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:19:07.143836 goxlrutilityapi-1.0.0.dev9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:46:50.960217 goxlrutilityapi-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 10:46:50.960217 goxlrutilityapi-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:46:50.956217 goxlrutilityapi-1.0.1/goxlrutilityapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:46:50.960217 goxlrutilityapi-1.0.1/goxlrutilityapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:46:50.960217 goxlrutilityapi-1.0.1/goxlrutilityapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 10:46:50.000000 goxlrutilityapi-1.0.1/goxlrutilityapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-30 10:46:50.000000 goxlrutilityapi-1.0.1/goxlrutilityapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 10:46:50.000000 goxlrutilityapi-1.0.1/goxlrutilityapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 10:46:50.000000 goxlrutilityapi-1.0.1/goxlrutilityapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 10:46:50.000000 goxlrutilityapi-1.0.1/goxlrutilityapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 10:46:50.960217 goxlrutilityapi-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/setup.py
```

### Comparing `goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/__main__.py` & `goxlrutilityapi-1.0.1/goxlrutilityapi/__main__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/const.py` & `goxlrutilityapi-1.0.1/goxlrutilityapi/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 # Connection
 DEFAULT_HOST: Final[str] = "localhost"
 DEFAULT_PORT: Final[int] = 14564
 
 # Mixer
 VOLUME_MAX: Final[int] = 255
+MUTED_STATE: Final[str] = "MutedToX"
+UNMUTED_STATE: Final[str] = "Unmuted"
 
 # Request/Response Keys
 KEY_DATA: Final[str] = "data"
 KEY_ID: Final[str] = "id"
 KEY_TYPE: Final[str] = "type"
 
 # Request/Response Types
```

### Comparing `goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/models/status.py` & `goxlrutilityapi-1.0.1/goxlrutilityapi/models/status.py`

 * *Files 4% similar despite different names*

```diff
@@ -342,27 +342,27 @@
     sampler_clear: Optional[bool] = Field(None)
 
 
 class Mixer(DefaultBaseModel):
     """Mixer Model"""
 
     hardware: Hardware
-    shutdown_commands: Optional[list]
-    fader_status: Optional[FaderStatuses]
-    mic_status: Optional[MicStatus]
+    shutdown_commands: list
+    fader_status: FaderStatuses
+    mic_status: MicStatus
     levels: Levels
-    router: Optional[Router]
-    cough_button: Optional[CoughButton]
-    lighting: Optional[Lighting]
-    effects: Optional[Any]
-    sampler: Optional[Any]
-    settings: Optional[Settings]
-    button_down: Optional[ButtonDown]
-    profile_name: Optional[str]
-    mic_profile_name: Optional[str]
+    router: Router
+    cough_button: CoughButton
+    lighting: Lighting
+    effects: Any
+    sampler: Any
+    settings: Settings
+    button_down: ButtonDown
+    profile_name: str
+    mic_profile_name: str
 
 
 class Paths(DefaultBaseModel):
     """Paths Model"""
 
     profile_directory: Optional[str]
     mic_profile_directory: Optional[str]
```

### Comparing `goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/websocket_client.py` & `goxlrutilityapi-1.0.1/goxlrutilityapi/websocket_client.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev9/goxlrutilityapi.egg-info/SOURCES.txt` & `goxlrutilityapi-1.0.1/goxlrutilityapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev9/pyproject.toml` & `goxlrutilityapi-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev9/setup.py` & `goxlrutilityapi-1.0.1/setup.py`

 * *Files identical despite different names*

