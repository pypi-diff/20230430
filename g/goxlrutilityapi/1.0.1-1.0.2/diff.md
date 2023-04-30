# Comparing `tmp/goxlrutilityapi-1.0.1.tar.gz` & `tmp/goxlrutilityapi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlrutilityapi-1.0.1.tar", last modified: Sun Apr 30 10:46:50 2023, max compression
+gzip compressed data, was "goxlrutilityapi-1.0.2.tar", last modified: Sun Apr 30 11:09:39 2023, max compression
```

## Comparing `goxlrutilityapi-1.0.1.tar` & `goxlrutilityapi-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:46:50.960217 goxlrutilityapi-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 10:46:50.960217 goxlrutilityapi-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:46:50.956217 goxlrutilityapi-1.0.1/goxlrutilityapi/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:46:50.960217 goxlrutilityapi-1.0.1/goxlrutilityapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/goxlrutilityapi/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:46:50.960217 goxlrutilityapi-1.0.1/goxlrutilityapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 10:46:50.000000 goxlrutilityapi-1.0.1/goxlrutilityapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-30 10:46:50.000000 goxlrutilityapi-1.0.1/goxlrutilityapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 10:46:50.000000 goxlrutilityapi-1.0.1/goxlrutilityapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 10:46:50.000000 goxlrutilityapi-1.0.1/goxlrutilityapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 10:46:50.000000 goxlrutilityapi-1.0.1/goxlrutilityapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 10:46:50.960217 goxlrutilityapi-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-30 10:46:37.000000 goxlrutilityapi-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:09:39.894906 goxlrutilityapi-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 11:09:39.894906 goxlrutilityapi-1.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:09:39.894906 goxlrutilityapi-1.0.2/goxlrutilityapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 11:09:25.000000 goxlrutilityapi-1.0.2/goxlrutilityapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-30 11:09:25.000000 goxlrutilityapi-1.0.2/goxlrutilityapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-30 11:09:25.000000 goxlrutilityapi-1.0.2/goxlrutilityapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 11:09:25.000000 goxlrutilityapi-1.0.2/goxlrutilityapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-30 11:09:25.000000 goxlrutilityapi-1.0.2/goxlrutilityapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 11:09:25.000000 goxlrutilityapi-1.0.2/goxlrutilityapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-30 11:09:25.000000 goxlrutilityapi-1.0.2/goxlrutilityapi/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-30 11:09:25.000000 goxlrutilityapi-1.0.2/goxlrutilityapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:09:39.894906 goxlrutilityapi-1.0.2/goxlrutilityapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-30 11:09:25.000000 goxlrutilityapi-1.0.2/goxlrutilityapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 11:09:25.000000 goxlrutilityapi-1.0.2/goxlrutilityapi/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-30 11:09:25.000000 goxlrutilityapi-1.0.2/goxlrutilityapi/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-30 11:09:25.000000 goxlrutilityapi-1.0.2/goxlrutilityapi/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-04-30 11:09:25.000000 goxlrutilityapi-1.0.2/goxlrutilityapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-04-30 11:09:25.000000 goxlrutilityapi-1.0.2/goxlrutilityapi/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:09:39.894906 goxlrutilityapi-1.0.2/goxlrutilityapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 11:09:39.000000 goxlrutilityapi-1.0.2/goxlrutilityapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-30 11:09:39.000000 goxlrutilityapi-1.0.2/goxlrutilityapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 11:09:39.000000 goxlrutilityapi-1.0.2/goxlrutilityapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 11:09:39.000000 goxlrutilityapi-1.0.2/goxlrutilityapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 11:09:39.000000 goxlrutilityapi-1.0.2/goxlrutilityapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-30 11:09:25.000000 goxlrutilityapi-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 11:09:39.894906 goxlrutilityapi-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-30 11:09:25.000000 goxlrutilityapi-1.0.2/setup.py
```

### Comparing `goxlrutilityapi-1.0.1/goxlrutilityapi/__main__.py` & `goxlrutilityapi-1.0.2/goxlrutilityapi/__main__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.1/goxlrutilityapi/const.py` & `goxlrutilityapi-1.0.2/goxlrutilityapi/const.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.1/goxlrutilityapi/helper.py` & `goxlrutilityapi-1.0.2/goxlrutilityapi/helper.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.1/goxlrutilityapi/models/status.py` & `goxlrutilityapi-1.0.2/goxlrutilityapi/models/status.py`

 * *Files 6% similar despite different names*

```diff
@@ -312,38 +312,38 @@
     mute_hold_duration: Optional[int]
     vc_mute_also_mute_cm: Optional[bool]
 
 
 class ButtonDown(DefaultBaseModel):
     """Button Down Model"""
 
-    fader1_mute: Optional[bool] = Field(None)
-    fader2_mute: Optional[bool] = Field(None)
-    fader3_mute: Optional[bool] = Field(None)
-    fader4_mute: Optional[bool] = Field(None)
-    bleep: Optional[bool] = Field(None)
-    cough: Optional[bool] = Field(None)
-    effect_select1: Optional[bool] = Field(None)
-    effect_select2: Optional[bool] = Field(None)
-    effect_select3: Optional[bool] = Field(None)
-    effect_select4: Optional[bool] = Field(None)
-    effect_select5: Optional[bool] = Field(None)
-    effect_select6: Optional[bool] = Field(None)
-    effect_fx: Optional[bool] = Field(None)
-    effect_megaphone: Optional[bool] = Field(None)
-    effect_robot: Optional[bool] = Field(None)
-    effect_hard_tune: Optional[bool] = Field(None)
-    sampler_select_a: Optional[bool] = Field(None)
-    sampler_select_b: Optional[bool] = Field(None)
-    sampler_select_c: Optional[bool] = Field(None)
-    sampler_top_left: Optional[bool] = Field(None)
-    sampler_top_right: Optional[bool] = Field(None)
-    sampler_bottom_left: Optional[bool] = Field(None)
-    sampler_bottom_right: Optional[bool] = Field(None)
-    sampler_clear: Optional[bool] = Field(None)
+    bleep: Optional[bool] = Field(None, alias="Bleep")
+    cough: Optional[bool] = Field(None, alias="Cough")
+    effect_fx: Optional[bool] = Field(None, alias="EffectFX")
+    effect_hard_tune: Optional[bool] = Field(None, alias="EffectHardTune")
+    effect_megaphone: Optional[bool] = Field(None, alias="EffectMegaphone")
+    effect_robot: Optional[bool] = Field(None, alias="EffectRobot")
+    effect_select1: Optional[bool] = Field(None, alias="EffectSelect1")
+    effect_select2: Optional[bool] = Field(None, alias="EffectSelect2")
+    effect_select3: Optional[bool] = Field(None, alias="EffectSelect3")
+    effect_select4: Optional[bool] = Field(None, alias="EffectSelect4")
+    effect_select5: Optional[bool] = Field(None, alias="EffectSelect5")
+    effect_select6: Optional[bool] = Field(None, alias="EffectSelect6")
+    fader1_mute: Optional[bool] = Field(None, alias="Fader1Mute")
+    fader2_mute: Optional[bool] = Field(None, alias="Fader2Mute")
+    fader3_mute: Optional[bool] = Field(None, alias="Fader3Mute")
+    fader4_mute: Optional[bool] = Field(None, alias="Fader4Mute")
+    sampler_bottom_left: Optional[bool] = Field(None, alias="SamplerBottomLeft")
+    sampler_bottom_right: Optional[bool] = Field(None, alias="SamplerBottomRight")
+    sampler_clear: Optional[bool] = Field(None, alias="SamplerClear")
+    sampler_select_a: Optional[bool] = Field(None, alias="SamplerSelectA")
+    sampler_select_b: Optional[bool] = Field(None, alias="SamplerSelectB")
+    sampler_select_c: Optional[bool] = Field(None, alias="SamplerSelectC")
+    sampler_top_left: Optional[bool] = Field(None, alias="SamplerTopLeft")
+    sampler_top_right: Optional[bool] = Field(None, alias="SamplerTopRight")
 
 
 class Mixer(DefaultBaseModel):
     """Mixer Model"""
 
     hardware: Hardware
     shutdown_commands: list
```

### Comparing `goxlrutilityapi-1.0.1/goxlrutilityapi/websocket_client.py` & `goxlrutilityapi-1.0.2/goxlrutilityapi/websocket_client.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.1/goxlrutilityapi.egg-info/SOURCES.txt` & `goxlrutilityapi-1.0.2/goxlrutilityapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.1/pyproject.toml` & `goxlrutilityapi-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.1/setup.py` & `goxlrutilityapi-1.0.2/setup.py`

 * *Files identical despite different names*

