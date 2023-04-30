# Comparing `tmp/goxlrutilityapi-1.0.3.tar.gz` & `tmp/goxlrutilityapi-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlrutilityapi-1.0.3.tar", last modified: Sun Apr 30 12:00:48 2023, max compression
+gzip compressed data, was "goxlrutilityapi-1.0.4.tar", last modified: Sun Apr 30 12:16:37 2023, max compression
```

## Comparing `goxlrutilityapi-1.0.3.tar` & `goxlrutilityapi-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:00:48.695866 goxlrutilityapi-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 12:00:48.695866 goxlrutilityapi-1.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:00:48.691865 goxlrutilityapi-1.0.3/goxlrutilityapi/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 12:00:30.000000 goxlrutilityapi-1.0.3/goxlrutilityapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-30 12:00:30.000000 goxlrutilityapi-1.0.3/goxlrutilityapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-30 12:00:30.000000 goxlrutilityapi-1.0.3/goxlrutilityapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 12:00:30.000000 goxlrutilityapi-1.0.3/goxlrutilityapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-30 12:00:30.000000 goxlrutilityapi-1.0.3/goxlrutilityapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 12:00:30.000000 goxlrutilityapi-1.0.3/goxlrutilityapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-30 12:00:30.000000 goxlrutilityapi-1.0.3/goxlrutilityapi/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-30 12:00:30.000000 goxlrutilityapi-1.0.3/goxlrutilityapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:00:48.695866 goxlrutilityapi-1.0.3/goxlrutilityapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-30 12:00:30.000000 goxlrutilityapi-1.0.3/goxlrutilityapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-30 12:00:30.000000 goxlrutilityapi-1.0.3/goxlrutilityapi/models/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 12:00:30.000000 goxlrutilityapi-1.0.3/goxlrutilityapi/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-30 12:00:30.000000 goxlrutilityapi-1.0.3/goxlrutilityapi/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-30 12:00:30.000000 goxlrutilityapi-1.0.3/goxlrutilityapi/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-04-30 12:00:30.000000 goxlrutilityapi-1.0.3/goxlrutilityapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-04-30 12:00:30.000000 goxlrutilityapi-1.0.3/goxlrutilityapi/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:00:48.695866 goxlrutilityapi-1.0.3/goxlrutilityapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 12:00:48.000000 goxlrutilityapi-1.0.3/goxlrutilityapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-30 12:00:48.000000 goxlrutilityapi-1.0.3/goxlrutilityapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:00:48.000000 goxlrutilityapi-1.0.3/goxlrutilityapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 12:00:48.000000 goxlrutilityapi-1.0.3/goxlrutilityapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 12:00:48.000000 goxlrutilityapi-1.0.3/goxlrutilityapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-30 12:00:30.000000 goxlrutilityapi-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 12:00:48.695866 goxlrutilityapi-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-30 12:00:30.000000 goxlrutilityapi-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:16:37.450669 goxlrutilityapi-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 12:16:37.450669 goxlrutilityapi-1.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:16:37.450669 goxlrutilityapi-1.0.4/goxlrutilityapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:16:37.450669 goxlrutilityapi-1.0.4/goxlrutilityapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/models/map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:16:37.450669 goxlrutilityapi-1.0.4/goxlrutilityapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 12:16:37.000000 goxlrutilityapi-1.0.4/goxlrutilityapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-30 12:16:37.000000 goxlrutilityapi-1.0.4/goxlrutilityapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:16:37.000000 goxlrutilityapi-1.0.4/goxlrutilityapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 12:16:37.000000 goxlrutilityapi-1.0.4/goxlrutilityapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 12:16:37.000000 goxlrutilityapi-1.0.4/goxlrutilityapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 12:16:37.450669 goxlrutilityapi-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/setup.py
```

### Comparing `goxlrutilityapi-1.0.3/goxlrutilityapi/__main__.py` & `goxlrutilityapi-1.0.4/goxlrutilityapi/__main__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.3/goxlrutilityapi/const.py` & `goxlrutilityapi-1.0.4/goxlrutilityapi/const.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """GoXLR Utility API: Constants"""
 
 from typing import Any, Final
 
-from .models.map import Map, MapItem
+from .models.map_item import MapItem
 from .models.patch import Patch
 from .models.request import Request
 from .models.response import Response
 from .models.status import Status
 
 # Connection
 DEFAULT_HOST: Final[str] = "localhost"
@@ -34,67 +34,57 @@
 MODEL_STATUS: type[Status] = Status
 
 MODEL_MAP: Final[dict[str, Any]] = {
     RESPONSE_TYPE_PATCH: MODEL_PATCH,
     RESPONSE_TYPE_STATUS: MODEL_STATUS,
 }
 
-NAME_MAP: Final[Map] = Map(
-    __root__={
-        "bleep": MapItem(name="Bleep", icon="bleep"),
-        "chat": MapItem(name="Chat", icon="mdi:chat"),
-        "console": MapItem(name="Console", icon="mdi:gamepad-variant"),
-        "cough": MapItem(name="Cough", icon="mdi:exclamation"),
-        "effect_fx": MapItem(name="Effect FX", icon="mdi:equalizer-outline"),
-        "effect_hard_tune": MapItem(name="Effect Hard Tune", icon="mdi:knob"),
-        "effect_megaphone": MapItem(
-            name="Effect Megaphone", icon="mdi:bullhorn-outline"
-        ),
-        "effect_robot": MapItem(name="Effect Robot", icon="mdi:robot-outline"),
-        "effect_select1": MapItem(name="Effect Select 1", icon="mdi:sawtooth-wave"),
-        "effect_select2": MapItem(name="Effect Select 2", icon="mdi:sawtooth-wave"),
-        "effect_select3": MapItem(name="Effect Select 3", icon="mdi:sawtooth-wave"),
-        "effect_select4": MapItem(name="Effect Select 4", icon="mdi:sawtooth-wave"),
-        "effect_select5": MapItem(name="Effect Select 5", icon="mdi:sawtooth-wave"),
-        "effect_select6": MapItem(name="Effect Select 6", icon="mdi:sawtooth-wave"),
-        "fader1_mute": MapItem(name="Fader 1 Mute", icon="mdi:microphone-off"),
-        "fader2_mute": MapItem(name="Fader 2 Mute", icon="mdi:microphone-off"),
-        "fader3_mute": MapItem(name="Fader 3 Mute", icon="mdi:microphone-off"),
-        "fader4_mute": MapItem(name="Fader 4 Mute", icon="mdi:microphone-off"),
-        "headphones": MapItem(name="Headphones", icon="mdi:headphones"),
-        "line_in": MapItem(name="Line In", icon="mdi:audio-input-stereo-minijack"),
-        "line_out": MapItem(name="Line In", icon="mdi:audio-input-stereo-minijack"),
-        "LineIn": MapItem(name="Line In", icon="mdi:audio-input-stereo-minijack"),
-        "LineOut": MapItem(name="Line In", icon="mdi:audio-input-stereo-minijack"),
-        "mic": MapItem(name="Microphone", icon="mdi:microphone"),
-        "mic_monitor": MapItem(
-            name="Microphone Monitor", icon="mdi:microphone-outline"
-        ),
-        "Mic": MapItem(name="Microphone", icon="mdi:microphone"),
-        "MicMonitor": MapItem(name="Microphone Monitor", icon="mdi:microphone-outline"),
-        "music": MapItem(name="Music", icon="mdi:music"),
-        "mute_all": MapItem(name="Mute All", icon="mdi:microphone-off"),
-        "mute_chat": MapItem(name="Mute Chat", icon="mdi:microphone-off"),
-        "mute_console": MapItem(name="Mute Console", icon="mdi:microphone-off"),
-        "mute_line_in": MapItem(name="Mute Line In", icon="mdi:microphone-off"),
-        "mute_line_out": MapItem(name="Mute Line Out", icon="mdi:microphone-off"),
-        "mute_mic": MapItem(name="Mute Microphone", icon="mdi:microphone-off"),
-        "mute_microphone": MapItem(name="Mute Microphone", icon="mdi:microphone-off"),
-        "mute_music": MapItem(name="Mute Music", icon="mdi:microphone-off"),
-        "mute_system": MapItem(name="Mute System", icon="mdi:microphone-off"),
-        "mute": MapItem(name="Mute", icon="mdi:microphone-off"),
-        "sample": MapItem(name="Sample", icon="mdi:music-note"),
-        "sampler_bottom_left": MapItem(
-            name="Sampler Bottom Left", icon="mdi:music-note"
-        ),
-        "sampler_bottom_right": MapItem(
-            name="Sampler Bottom Right", icon="mdi:music-note"
-        ),
-        "sampler_clear": MapItem(name="Sampler Clear", icon="mdi:music-note"),
-        "sampler_select_a": MapItem(name="Sampler Select A", icon="mdi:music-note"),
-        "sampler_select_b": MapItem(name="Sampler Select B", icon="mdi:music-note"),
-        "sampler_select_c": MapItem(name="Sampler Select C", icon="mdi:music-note"),
-        "sampler_top_left": MapItem(name="Sampler Top Left", icon="mdi:music-note"),
-        "sampler_top_right": MapItem(name="Sampler Top Right", icon="mdi:music-note"),
-        "system": MapItem(name="System", icon="mdi:music-box-outline"),
-    }
-)
+NAME_MAP: Final[dict[str, MapItem]] = {
+    "bleep": MapItem(name="Bleep", icon="bleep"),
+    "chat": MapItem(name="Chat", icon="mdi:chat"),
+    "console": MapItem(name="Console", icon="mdi:gamepad-variant"),
+    "cough": MapItem(name="Cough", icon="mdi:exclamation"),
+    "effect_fx": MapItem(name="Effect FX", icon="mdi:equalizer-outline"),
+    "effect_hard_tune": MapItem(name="Effect Hard Tune", icon="mdi:knob"),
+    "effect_megaphone": MapItem(name="Effect Megaphone", icon="mdi:bullhorn-outline"),
+    "effect_robot": MapItem(name="Effect Robot", icon="mdi:robot-outline"),
+    "effect_select1": MapItem(name="Effect Select 1", icon="mdi:sawtooth-wave"),
+    "effect_select2": MapItem(name="Effect Select 2", icon="mdi:sawtooth-wave"),
+    "effect_select3": MapItem(name="Effect Select 3", icon="mdi:sawtooth-wave"),
+    "effect_select4": MapItem(name="Effect Select 4", icon="mdi:sawtooth-wave"),
+    "effect_select5": MapItem(name="Effect Select 5", icon="mdi:sawtooth-wave"),
+    "effect_select6": MapItem(name="Effect Select 6", icon="mdi:sawtooth-wave"),
+    "fader1_mute": MapItem(name="Fader 1 Mute", icon="mdi:microphone-off"),
+    "fader2_mute": MapItem(name="Fader 2 Mute", icon="mdi:microphone-off"),
+    "fader3_mute": MapItem(name="Fader 3 Mute", icon="mdi:microphone-off"),
+    "fader4_mute": MapItem(name="Fader 4 Mute", icon="mdi:microphone-off"),
+    "headphones": MapItem(name="Headphones", icon="mdi:headphones"),
+    "line_in": MapItem(name="Line In", icon="mdi:audio-input-stereo-minijack"),
+    "line_out": MapItem(name="Line In", icon="mdi:audio-input-stereo-minijack"),
+    "LineIn": MapItem(name="Line In", icon="mdi:audio-input-stereo-minijack"),
+    "LineOut": MapItem(name="Line In", icon="mdi:audio-input-stereo-minijack"),
+    "mic_monitor": MapItem(name="Microphone Monitor", icon="mdi:microphone-outline"),
+    "mic": MapItem(name="Microphone", icon="mdi:microphone"),
+    "Mic": MapItem(name="Microphone", icon="mdi:microphone"),
+    "MicMonitor": MapItem(name="Microphone Monitor", icon="mdi:microphone-outline"),
+    "music": MapItem(name="Music", icon="mdi:music"),
+    "mute_all": MapItem(name="Mute All", icon="mdi:microphone-off"),
+    "mute_chat": MapItem(name="Mute Chat", icon="mdi:microphone-off"),
+    "mute_console": MapItem(name="Mute Console", icon="mdi:microphone-off"),
+    "mute_line_in": MapItem(name="Mute Line In", icon="mdi:microphone-off"),
+    "mute_line_out": MapItem(name="Mute Line Out", icon="mdi:microphone-off"),
+    "mute_mic": MapItem(name="Mute Microphone", icon="mdi:microphone-off"),
+    "mute_microphone": MapItem(name="Mute Microphone", icon="mdi:microphone-off"),
+    "mute_music": MapItem(name="Mute Music", icon="mdi:microphone-off"),
+    "mute_system": MapItem(name="Mute System", icon="mdi:microphone-off"),
+    "mute": MapItem(name="Mute", icon="mdi:microphone-off"),
+    "sample": MapItem(name="Sample", icon="mdi:music-note"),
+    "sampler_bottom_left": MapItem(name="Sampler Bottom Left", icon="mdi:music-note"),
+    "sampler_bottom_right": MapItem(name="Sampler Bottom Right", icon="mdi:music-note"),
+    "sampler_clear": MapItem(name="Sampler Clear", icon="mdi:music-note"),
+    "sampler_select_a": MapItem(name="Sampler Select A", icon="mdi:music-note"),
+    "sampler_select_b": MapItem(name="Sampler Select B", icon="mdi:music-note"),
+    "sampler_select_c": MapItem(name="Sampler Select C", icon="mdi:music-note"),
+    "sampler_top_left": MapItem(name="Sampler Top Left", icon="mdi:music-note"),
+    "sampler_top_right": MapItem(name="Sampler Top Right", icon="mdi:music-note"),
+    "system": MapItem(name="System", icon="mdi:music-box-outline"),
+}
```

### Comparing `goxlrutilityapi-1.0.3/goxlrutilityapi/helper.py` & `goxlrutilityapi-1.0.4/goxlrutilityapi/helper.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.3/goxlrutilityapi/models/status.py` & `goxlrutilityapi-1.0.4/goxlrutilityapi/models/status.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.3/goxlrutilityapi/websocket_client.py` & `goxlrutilityapi-1.0.4/goxlrutilityapi/websocket_client.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.3/goxlrutilityapi.egg-info/SOURCES.txt` & `goxlrutilityapi-1.0.4/goxlrutilityapi.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,12 +11,12 @@
 goxlrutilityapi/websocket_client.py
 goxlrutilityapi.egg-info/PKG-INFO
 goxlrutilityapi.egg-info/SOURCES.txt
 goxlrutilityapi.egg-info/dependency_links.txt
 goxlrutilityapi.egg-info/requires.txt
 goxlrutilityapi.egg-info/top_level.txt
 goxlrutilityapi/models/__init__.py
-goxlrutilityapi/models/map.py
+goxlrutilityapi/models/map_item.py
 goxlrutilityapi/models/patch.py
 goxlrutilityapi/models/request.py
 goxlrutilityapi/models/response.py
 goxlrutilityapi/models/status.py
```

### Comparing `goxlrutilityapi-1.0.3/pyproject.toml` & `goxlrutilityapi-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.3/setup.py` & `goxlrutilityapi-1.0.4/setup.py`

 * *Files identical despite different names*

