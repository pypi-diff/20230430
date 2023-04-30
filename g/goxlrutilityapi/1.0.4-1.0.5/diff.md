# Comparing `tmp/goxlrutilityapi-1.0.4.tar.gz` & `tmp/goxlrutilityapi-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlrutilityapi-1.0.4.tar", last modified: Sun Apr 30 12:16:37 2023, max compression
+gzip compressed data, was "goxlrutilityapi-1.0.5.tar", last modified: Sun Apr 30 12:53:11 2023, max compression
```

## Comparing `goxlrutilityapi-1.0.4.tar` & `goxlrutilityapi-1.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:16:37.450669 goxlrutilityapi-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 12:16:37.450669 goxlrutilityapi-1.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:16:37.450669 goxlrutilityapi-1.0.4/goxlrutilityapi/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:16:37.450669 goxlrutilityapi-1.0.4/goxlrutilityapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/models/map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/goxlrutilityapi/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:16:37.450669 goxlrutilityapi-1.0.4/goxlrutilityapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 12:16:37.000000 goxlrutilityapi-1.0.4/goxlrutilityapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-30 12:16:37.000000 goxlrutilityapi-1.0.4/goxlrutilityapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:16:37.000000 goxlrutilityapi-1.0.4/goxlrutilityapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 12:16:37.000000 goxlrutilityapi-1.0.4/goxlrutilityapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 12:16:37.000000 goxlrutilityapi-1.0.4/goxlrutilityapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 12:16:37.450669 goxlrutilityapi-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-30 12:16:21.000000 goxlrutilityapi-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:53:11.324543 goxlrutilityapi-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 12:53:11.324543 goxlrutilityapi-1.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:53:11.324543 goxlrutilityapi-1.0.5/goxlrutilityapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:53:11.324543 goxlrutilityapi-1.0.5/goxlrutilityapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/models/map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/goxlrutilityapi/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:53:11.324543 goxlrutilityapi-1.0.5/goxlrutilityapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 12:53:11.000000 goxlrutilityapi-1.0.5/goxlrutilityapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-30 12:53:11.000000 goxlrutilityapi-1.0.5/goxlrutilityapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:53:11.000000 goxlrutilityapi-1.0.5/goxlrutilityapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 12:53:11.000000 goxlrutilityapi-1.0.5/goxlrutilityapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 12:53:11.000000 goxlrutilityapi-1.0.5/goxlrutilityapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 12:53:11.324543 goxlrutilityapi-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-30 12:52:52.000000 goxlrutilityapi-1.0.5/setup.py
```

### Comparing `goxlrutilityapi-1.0.4/goxlrutilityapi/__main__.py` & `goxlrutilityapi-1.0.5/goxlrutilityapi/__main__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.4/goxlrutilityapi/const.py` & `goxlrutilityapi-1.0.5/goxlrutilityapi/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 
 MODEL_MAP: Final[dict[str, Any]] = {
     RESPONSE_TYPE_PATCH: MODEL_PATCH,
     RESPONSE_TYPE_STATUS: MODEL_STATUS,
 }
 
 NAME_MAP: Final[dict[str, MapItem]] = {
-    "bleep": MapItem(name="Bleep", icon="bleep"),
+    "bleep": MapItem(name="Bleep", icon="mdi:exclamation"),
     "chat": MapItem(name="Chat", icon="mdi:chat"),
     "console": MapItem(name="Console", icon="mdi:gamepad-variant"),
-    "cough": MapItem(name="Cough", icon="mdi:exclamation"),
+    "cough": MapItem(name="Cough", icon="mdi:microphone-off"),
     "effect_fx": MapItem(name="Effect FX", icon="mdi:equalizer-outline"),
     "effect_hard_tune": MapItem(name="Effect Hard Tune", icon="mdi:knob"),
     "effect_megaphone": MapItem(name="Effect Megaphone", icon="mdi:bullhorn-outline"),
     "effect_robot": MapItem(name="Effect Robot", icon="mdi:robot-outline"),
     "effect_select1": MapItem(name="Effect Select 1", icon="mdi:sawtooth-wave"),
     "effect_select2": MapItem(name="Effect Select 2", icon="mdi:sawtooth-wave"),
     "effect_select3": MapItem(name="Effect Select 3", icon="mdi:sawtooth-wave"),
@@ -63,14 +63,15 @@
     "LineIn": MapItem(name="Line In", icon="mdi:audio-input-stereo-minijack"),
     "LineOut": MapItem(name="Line In", icon="mdi:audio-input-stereo-minijack"),
     "mic_monitor": MapItem(name="Microphone Monitor", icon="mdi:microphone-outline"),
     "mic": MapItem(name="Microphone", icon="mdi:microphone"),
     "Mic": MapItem(name="Microphone", icon="mdi:microphone"),
     "MicMonitor": MapItem(name="Microphone Monitor", icon="mdi:microphone-outline"),
     "music": MapItem(name="Music", icon="mdi:music"),
+    "Music": MapItem(name="Music", icon="mdi:music"),
     "mute_all": MapItem(name="Mute All", icon="mdi:microphone-off"),
     "mute_chat": MapItem(name="Mute Chat", icon="mdi:microphone-off"),
     "mute_console": MapItem(name="Mute Console", icon="mdi:microphone-off"),
     "mute_line_in": MapItem(name="Mute Line In", icon="mdi:microphone-off"),
     "mute_line_out": MapItem(name="Mute Line Out", icon="mdi:microphone-off"),
     "mute_mic": MapItem(name="Mute Microphone", icon="mdi:microphone-off"),
     "mute_microphone": MapItem(name="Mute Microphone", icon="mdi:microphone-off"),
@@ -83,8 +84,9 @@
     "sampler_clear": MapItem(name="Sampler Clear", icon="mdi:music-note"),
     "sampler_select_a": MapItem(name="Sampler Select A", icon="mdi:music-note"),
     "sampler_select_b": MapItem(name="Sampler Select B", icon="mdi:music-note"),
     "sampler_select_c": MapItem(name="Sampler Select C", icon="mdi:music-note"),
     "sampler_top_left": MapItem(name="Sampler Top Left", icon="mdi:music-note"),
     "sampler_top_right": MapItem(name="Sampler Top Right", icon="mdi:music-note"),
     "system": MapItem(name="System", icon="mdi:music-box-outline"),
+    "System": MapItem(name="System", icon="mdi:music-box-outline"),
 }
```

### Comparing `goxlrutilityapi-1.0.4/goxlrutilityapi/helper.py` & `goxlrutilityapi-1.0.5/goxlrutilityapi/helper.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.4/goxlrutilityapi/models/status.py` & `goxlrutilityapi-1.0.5/goxlrutilityapi/models/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
 
 
 class ButtonDown(DefaultBaseModel):
     """Button Down Model"""
 
     bleep: Optional[bool] = Field(None, alias="Bleep")
     cough: Optional[bool] = Field(None, alias="Cough")
-    effect_fx: Optional[bool] = Field(None, alias="EffectFX")
+    effect_fx: Optional[bool] = Field(None, alias="EffectFx")
     effect_hard_tune: Optional[bool] = Field(None, alias="EffectHardTune")
     effect_megaphone: Optional[bool] = Field(None, alias="EffectMegaphone")
     effect_robot: Optional[bool] = Field(None, alias="EffectRobot")
     effect_select1: Optional[bool] = Field(None, alias="EffectSelect1")
     effect_select2: Optional[bool] = Field(None, alias="EffectSelect2")
     effect_select3: Optional[bool] = Field(None, alias="EffectSelect3")
     effect_select4: Optional[bool] = Field(None, alias="EffectSelect4")
```

### Comparing `goxlrutilityapi-1.0.4/goxlrutilityapi/websocket_client.py` & `goxlrutilityapi-1.0.5/goxlrutilityapi/websocket_client.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.4/goxlrutilityapi.egg-info/SOURCES.txt` & `goxlrutilityapi-1.0.5/goxlrutilityapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.4/pyproject.toml` & `goxlrutilityapi-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.4/setup.py` & `goxlrutilityapi-1.0.5/setup.py`

 * *Files identical despite different names*

