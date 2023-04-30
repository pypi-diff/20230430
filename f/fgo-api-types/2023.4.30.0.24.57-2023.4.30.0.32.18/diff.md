# Comparing `tmp/fgo_api_types-2023.4.30.0.24.57.tar.gz` & `tmp/fgo_api_types-2023.4.30.0.32.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2023.4.30.0.24.57.tar", max compression
+gzip compressed data, was "fgo_api_types-2023.4.30.0.32.18.tar", max compression
```

## Comparing `fgo_api_types-2023.4.30.0.24.57.tar` & `fgo_api_types-2023.4.30.0.32.18.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-04-30 00:24:32.475231 fgo_api_types-2023.4.30.0.24.57/LICENSE
--rw-r--r--   0        0        0      449 2023-04-30 00:24:32.475231 fgo_api_types-2023.4.30.0.24.57/README.md
--rw-r--r--   0        0        0        0 2023-04-30 00:24:57.983013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2023-04-30 00:24:57.983013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/base.py
--rw-r--r--   0        0        0     4195 2023-04-30 00:24:57.983013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3631 2023-04-30 00:24:57.983013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/common.py
--rw-r--r--   0        0        0    37809 2023-04-30 00:24:57.987013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/enums.py
--rw-r--r--   0        0        0   157289 2023-04-30 00:24:57.987013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    74847 2023-04-30 00:24:57.987013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/nice.py
--rw-r--r--   0        0        0    50178 2023-04-30 00:24:57.987013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4176 2023-04-30 00:24:57.987013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    18670 2023-04-30 00:24:57.987013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2023-04-30 00:24:58.311010 fgo_api_types-2023.4.30.0.24.57/pyproject.toml
--rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 fgo_api_types-2023.4.30.0.24.57/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-30 00:31:52.166432 fgo_api_types-2023.4.30.0.32.18/LICENSE
+-rw-r--r--   0        0        0      449 2023-04-30 00:31:52.166432 fgo_api_types-2023.4.30.0.32.18/README.md
+-rw-r--r--   0        0        0        0 2023-04-30 00:32:18.462728 fgo_api_types-2023.4.30.0.32.18/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2023-04-30 00:32:18.466728 fgo_api_types-2023.4.30.0.32.18/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4195 2023-04-30 00:32:18.466728 fgo_api_types-2023.4.30.0.32.18/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3631 2023-04-30 00:32:18.466728 fgo_api_types-2023.4.30.0.32.18/fgo_api_types/common.py
+-rw-r--r--   0        0        0    37809 2023-04-30 00:32:18.466728 fgo_api_types-2023.4.30.0.32.18/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   157289 2023-04-30 00:32:18.466728 fgo_api_types-2023.4.30.0.32.18/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    74891 2023-04-30 00:32:18.466728 fgo_api_types-2023.4.30.0.32.18/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    50178 2023-04-30 00:32:18.466728 fgo_api_types-2023.4.30.0.32.18/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4176 2023-04-30 00:32:18.466728 fgo_api_types-2023.4.30.0.32.18/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    18670 2023-04-30 00:32:18.466728 fgo_api_types-2023.4.30.0.32.18/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2023-04-30 00:32:18.858732 fgo_api_types-2023.4.30.0.32.18/pyproject.toml
+-rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 fgo_api_types-2023.4.30.0.32.18/PKG-INFO
```

### Comparing `fgo_api_types-2023.4.30.0.24.57/LICENSE` & `fgo_api_types-2023.4.30.0.32.18/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.30.0.24.57/fgo_api_types/basic.py` & `fgo_api_types-2023.4.30.0.32.18/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.30.0.24.57/fgo_api_types/common.py` & `fgo_api_types-2023.4.30.0.32.18/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.30.0.24.57/fgo_api_types/enums.py` & `fgo_api_types-2023.4.30.0.32.18/fgo_api_types/enums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.30.0.24.57/fgo_api_types/gameenums.py` & `fgo_api_types-2023.4.30.0.32.18/fgo_api_types/gameenums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.30.0.24.57/fgo_api_types/nice.py` & `fgo_api_types-2023.4.30.0.32.18/fgo_api_types/nice.py`

 * *Files 0% similar despite different names*

```diff
@@ -2272,14 +2272,15 @@
     releaseConditions: list[SupportServantRelease]
     lv: int
     atk: int
     hp: int
     traits: list[NiceTrait]
     skills: EnemySkill
     noblePhantasm: SupportServantTd
+    flags: list[NiceNpcServantFollowerFlag]
     equips: list[SupportServantEquip]
     script: SupportServantScript
     limit: SupportServantLimit
     misc: SupportServantMisc
 
 
 class NiceQuestPhaseAiNpc(BaseModelORJson):
```

### Comparing `fgo_api_types-2023.4.30.0.24.57/fgo_api_types/raw.py` & `fgo_api_types-2023.4.30.0.32.18/fgo_api_types/raw.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.30.0.24.57/fgo_api_types/rayshift.py` & `fgo_api_types-2023.4.30.0.32.18/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.30.0.24.57/fgo_api_types/search.py` & `fgo_api_types-2023.4.30.0.32.18/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.30.0.24.57/pyproject.toml` & `fgo_api_types-2023.4.30.0.32.18/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2023.04.30.00.24.57"
+version = "2023.04.30.00.32.18"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2023.4.30.0.24.57/PKG-INFO` & `fgo_api_types-2023.4.30.0.32.18/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2023.4.30.0.24.57
+Version: 2023.4.30.0.32.18
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

