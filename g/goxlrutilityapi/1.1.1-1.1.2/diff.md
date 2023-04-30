# Comparing `tmp/goxlrutilityapi-1.1.1.tar.gz` & `tmp/goxlrutilityapi-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlrutilityapi-1.1.1.tar", last modified: Sun Apr 30 16:27:57 2023, max compression
+gzip compressed data, was "goxlrutilityapi-1.1.2.tar", last modified: Sun Apr 30 20:07:42 2023, max compression
```

## Comparing `goxlrutilityapi-1.1.1.tar` & `goxlrutilityapi-1.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:27:57.946578 goxlrutilityapi-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 16:27:57.946578 goxlrutilityapi-1.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:27:57.942578 goxlrutilityapi-1.1.1/goxlrutilityapi/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 16:27:46.000000 goxlrutilityapi-1.1.1/goxlrutilityapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-30 16:27:46.000000 goxlrutilityapi-1.1.1/goxlrutilityapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-30 16:27:46.000000 goxlrutilityapi-1.1.1/goxlrutilityapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 16:27:46.000000 goxlrutilityapi-1.1.1/goxlrutilityapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-04-30 16:27:46.000000 goxlrutilityapi-1.1.1/goxlrutilityapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 16:27:46.000000 goxlrutilityapi-1.1.1/goxlrutilityapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-30 16:27:46.000000 goxlrutilityapi-1.1.1/goxlrutilityapi/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-30 16:27:46.000000 goxlrutilityapi-1.1.1/goxlrutilityapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:27:57.946578 goxlrutilityapi-1.1.1/goxlrutilityapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-30 16:27:46.000000 goxlrutilityapi-1.1.1/goxlrutilityapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-30 16:27:46.000000 goxlrutilityapi-1.1.1/goxlrutilityapi/models/map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 16:27:46.000000 goxlrutilityapi-1.1.1/goxlrutilityapi/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-30 16:27:46.000000 goxlrutilityapi-1.1.1/goxlrutilityapi/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-30 16:27:46.000000 goxlrutilityapi-1.1.1/goxlrutilityapi/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-04-30 16:27:46.000000 goxlrutilityapi-1.1.1/goxlrutilityapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-04-30 16:27:46.000000 goxlrutilityapi-1.1.1/goxlrutilityapi/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:27:57.946578 goxlrutilityapi-1.1.1/goxlrutilityapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 16:27:57.000000 goxlrutilityapi-1.1.1/goxlrutilityapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-30 16:27:57.000000 goxlrutilityapi-1.1.1/goxlrutilityapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 16:27:57.000000 goxlrutilityapi-1.1.1/goxlrutilityapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 16:27:57.000000 goxlrutilityapi-1.1.1/goxlrutilityapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 16:27:57.000000 goxlrutilityapi-1.1.1/goxlrutilityapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-30 16:27:46.000000 goxlrutilityapi-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 16:27:57.946578 goxlrutilityapi-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-30 16:27:46.000000 goxlrutilityapi-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:07:42.758635 goxlrutilityapi-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 20:07:42.758635 goxlrutilityapi-1.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:07:42.758635 goxlrutilityapi-1.1.2/goxlrutilityapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:07:42.758635 goxlrutilityapi-1.1.2/goxlrutilityapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/models/map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:07:42.758635 goxlrutilityapi-1.1.2/goxlrutilityapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 20:07:42.000000 goxlrutilityapi-1.1.2/goxlrutilityapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-30 20:07:42.000000 goxlrutilityapi-1.1.2/goxlrutilityapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 20:07:42.000000 goxlrutilityapi-1.1.2/goxlrutilityapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 20:07:42.000000 goxlrutilityapi-1.1.2/goxlrutilityapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 20:07:42.000000 goxlrutilityapi-1.1.2/goxlrutilityapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 20:07:42.758635 goxlrutilityapi-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/setup.py
```

### Comparing `goxlrutilityapi-1.1.1/goxlrutilityapi/__main__.py` & `goxlrutilityapi-1.1.2/goxlrutilityapi/__main__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.1.1/goxlrutilityapi/const.py` & `goxlrutilityapi-1.1.2/goxlrutilityapi/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,63 +79,75 @@
 BUTTON_SAMPLER_CLEAR: Final[str] = "SamplerClear"
 BUTTON_SAMPLER_SELECT_A: Final[str] = "SamplerSelectA"
 BUTTON_SAMPLER_SELECT_B: Final[str] = "SamplerSelectB"
 BUTTON_SAMPLER_SELECT_C: Final[str] = "SamplerSelectC"
 BUTTON_SAMPLER_TOP_LEFT: Final[str] = "SamplerTopLeft"
 BUTTON_SAMPLER_TOP_RIGHT: Final[str] = "SamplerTopRight"
 
-BUTTON_MAP: Final[dict[str, str]] = {
+# Faders
+FADER_A: Final[str] = "A"
+FADER_B: Final[str] = "B"
+FADER_C: Final[str] = "C"
+FADER_D: Final[str] = "D"
+
+# Models
+MODEL_PATCH: type[Patch] = Patch
+MODEL_REQUEST: type[Request] = Request
+MODEL_RESPONSE: type[Response[Any]] = Response
+MODEL_STATUS: type[Status] = Status
+
+MODEL_MAP: Final[dict[str, Any]] = {
+    RESPONSE_TYPE_PATCH: MODEL_PATCH,
+    RESPONSE_TYPE_STATUS: MODEL_STATUS,
+}
+
+KEY_MAP: Final[dict[str, str]] = {
+    "a": FADER_A,
+    "b": FADER_B,
     "bleep": BUTTON_BLEEP,
+    "c": FADER_C,
     "cough": BUTTON_COUGH,
+    "d": FADER_D,
     "effect_fx": BUTTON_EFFECT_FX,
     "effect_hard_tune": BUTTON_EFFECT_HARD_TUNE,
     "effect_megaphone": BUTTON_EFFECT_MEGAPHONE,
     "effect_robot": BUTTON_EFFECT_ROBOT,
     "effect_select_1": BUTTON_EFFECT_SELECT_1,
     "effect_select_2": BUTTON_EFFECT_SELECT_2,
     "effect_select_3": BUTTON_EFFECT_SELECT_3,
     "effect_select_4": BUTTON_EFFECT_SELECT_4,
     "effect_select_5": BUTTON_EFFECT_SELECT_5,
     "effect_select_6": BUTTON_EFFECT_SELECT_6,
-    "fader_1_mute": BUTTON_FADER_1_MUTE,
-    "fader_2_mute": BUTTON_FADER_2_MUTE,
-    "fader_3_mute": BUTTON_FADER_3_MUTE,
-    "fader_4_mute": BUTTON_FADER_4_MUTE,
+    "fader1_mute": BUTTON_FADER_1_MUTE,
+    "fader2_mute": BUTTON_FADER_2_MUTE,
+    "fader3_mute": BUTTON_FADER_3_MUTE,
+    "fader4_mute": BUTTON_FADER_4_MUTE,
     "sampler_bottom_left": BUTTON_SAMPLER_BOTTOM_LEFT,
     "sampler_bottom_right": BUTTON_SAMPLER_BOTTOM_RIGHT,
     "sampler_clear": BUTTON_SAMPLER_CLEAR,
     "sampler_select_a": BUTTON_SAMPLER_SELECT_A,
     "sampler_select_b": BUTTON_SAMPLER_SELECT_B,
     "sampler_select_c": BUTTON_SAMPLER_SELECT_C,
     "sampler_top_left": BUTTON_SAMPLER_TOP_LEFT,
     "sampler_top_right": BUTTON_SAMPLER_TOP_RIGHT,
 }
 
-# Faders
-FADER_A: Final[str] = "A"
-FADER_B: Final[str] = "B"
-FADER_C: Final[str] = "C"
-FADER_D: Final[str] = "D"
-
-# Models
-MODEL_PATCH: type[Patch] = Patch
-MODEL_REQUEST: type[Request] = Request
-MODEL_RESPONSE: type[Response[Any]] = Response
-MODEL_STATUS: type[Status] = Status
-
-MODEL_MAP: Final[dict[str, Any]] = {
-    RESPONSE_TYPE_PATCH: MODEL_PATCH,
-    RESPONSE_TYPE_STATUS: MODEL_STATUS,
-}
-
 NAME_MAP: Final[dict[str, MapItem]] = {
+    "a": MapItem(name="Fader 1", icon="mdi:tune-vertical-variant"),
+    "A": MapItem(name="Fader 1", icon="mdi:tune-vertical-variant"),
+    "b": MapItem(name="Fader 2", icon="mdi:tune-vertical-variant"),
+    "B": MapItem(name="Fader 2", icon="mdi:tune-vertical-variant"),
     "bleep": MapItem(name=BUTTON_BLEEP, icon="mdi:exclamation"),
+    "c": MapItem(name="Fader 3", icon="mdi:tune-vertical-variant"),
+    "C": MapItem(name="Fader 3", icon="mdi:tune-vertical-variant"),
     "chat": MapItem(name="Chat", icon="mdi:chat"),
     "console": MapItem(name="Console", icon="mdi:gamepad-variant"),
     "cough": MapItem(name=BUTTON_COUGH, icon="mdi:microphone-off"),
+    "d": MapItem(name="Fader 4", icon="mdi:tune-vertical-variant"),
+    "D": MapItem(name="Fader 4", icon="mdi:tune-vertical-variant"),
     "effect_fx": MapItem(name="Effect FX", icon="mdi:equalizer-outline"),
     "effect_hard_tune": MapItem(name="Effect Hard Tune", icon="mdi:knob"),
     "effect_megaphone": MapItem(name="Effect Megaphone", icon="mdi:bullhorn-outline"),
     "effect_robot": MapItem(name="Effect Robot", icon="mdi:robot-outline"),
     "effect_select_1": MapItem(name="Effect Select 1", icon="mdi:sawtooth-wave"),
     "effect_select_2": MapItem(name="Effect Select 2", icon="mdi:sawtooth-wave"),
     "effect_select_3": MapItem(name="Effect Select 3", icon="mdi:sawtooth-wave"),
@@ -188,12 +200,8 @@
     "sampler_select_a": MapItem(name="Sampler Select A", icon="mdi:music-note"),
     "sampler_select_b": MapItem(name="Sampler Select B", icon="mdi:music-note"),
     "sampler_select_c": MapItem(name="Sampler Select C", icon="mdi:music-note"),
     "sampler_top_left": MapItem(name="Sampler Top Left", icon="mdi:music-note"),
     "sampler_top_right": MapItem(name="Sampler Top Right", icon="mdi:music-note"),
     "system": MapItem(name="System", icon="mdi:music-box-outline"),
     "System": MapItem(name="System", icon="mdi:music-box-outline"),
-    FADER_A: MapItem(name="Fader A", icon="mdi:tune-vertical-variant"),
-    FADER_B: MapItem(name="Fader B", icon="mdi:tune-vertical-variant"),
-    FADER_C: MapItem(name="Fader C", icon="mdi:tune-vertical-variant"),
-    FADER_D: MapItem(name="Fader D", icon="mdi:tune-vertical-variant"),
 }
```

### Comparing `goxlrutilityapi-1.1.1/goxlrutilityapi/helper.py` & `goxlrutilityapi-1.1.2/goxlrutilityapi/helper.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.1.1/goxlrutilityapi/models/status.py` & `goxlrutilityapi-1.1.2/goxlrutilityapi/models/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,15 +279,15 @@
     colour_one: Optional[str]
 
 
 class Simple(DefaultBaseModel):
     """Simple Model"""
 
     global_: Optional[Global] = Field(None, alias="Global")
-    accent: Optional[Accent] = Field(None, alias="Accent")
+    accent: Accent = Field(None, alias="Accent")
 
 
 class Lighting(DefaultBaseModel):
     """Lighting Model"""
 
     faders: Faders
     buttons: Buttons
```

### Comparing `goxlrutilityapi-1.1.1/goxlrutilityapi/websocket_client.py` & `goxlrutilityapi-1.1.2/goxlrutilityapi/websocket_client.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.1.1/goxlrutilityapi.egg-info/SOURCES.txt` & `goxlrutilityapi-1.1.2/goxlrutilityapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.1.1/pyproject.toml` & `goxlrutilityapi-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.1.1/setup.py` & `goxlrutilityapi-1.1.2/setup.py`

 * *Files identical despite different names*

