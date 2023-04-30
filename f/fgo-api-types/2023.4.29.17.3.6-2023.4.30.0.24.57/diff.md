# Comparing `tmp/fgo_api_types-2023.4.29.17.3.6.tar.gz` & `tmp/fgo_api_types-2023.4.30.0.24.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2023.4.29.17.3.6.tar", max compression
+gzip compressed data, was "fgo_api_types-2023.4.30.0.24.57.tar", max compression
```

## Comparing `fgo_api_types-2023.4.29.17.3.6.tar` & `fgo_api_types-2023.4.30.0.24.57.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-04-29 17:02:43.279729 fgo_api_types-2023.4.29.17.3.6/LICENSE
--rw-r--r--   0        0        0      449 2023-04-29 17:02:43.279729 fgo_api_types-2023.4.29.17.3.6/README.md
--rw-r--r--   0        0        0        0 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/base.py
--rw-r--r--   0        0        0     4195 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3631 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/common.py
--rw-r--r--   0        0        0    37696 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/enums.py
--rw-r--r--   0        0        0   157289 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    74847 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/nice.py
--rw-r--r--   0        0        0    50178 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4176 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    18670 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2023-04-29 17:03:06.491740 fgo_api_types-2023.4.29.17.3.6/pyproject.toml
--rw-r--r--   0        0        0     1221 1970-01-01 00:00:00.000000 fgo_api_types-2023.4.29.17.3.6/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-30 00:24:32.475231 fgo_api_types-2023.4.30.0.24.57/LICENSE
+-rw-r--r--   0        0        0      449 2023-04-30 00:24:32.475231 fgo_api_types-2023.4.30.0.24.57/README.md
+-rw-r--r--   0        0        0        0 2023-04-30 00:24:57.983013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2023-04-30 00:24:57.983013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4195 2023-04-30 00:24:57.983013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3631 2023-04-30 00:24:57.983013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/common.py
+-rw-r--r--   0        0        0    37809 2023-04-30 00:24:57.987013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   157289 2023-04-30 00:24:57.987013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    74847 2023-04-30 00:24:57.987013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    50178 2023-04-30 00:24:57.987013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4176 2023-04-30 00:24:57.987013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    18670 2023-04-30 00:24:57.987013 fgo_api_types-2023.4.30.0.24.57/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2023-04-30 00:24:58.311010 fgo_api_types-2023.4.30.0.24.57/pyproject.toml
+-rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 fgo_api_types-2023.4.30.0.24.57/PKG-INFO
```

### Comparing `fgo_api_types-2023.4.29.17.3.6/LICENSE` & `fgo_api_types-2023.4.30.0.24.57/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.29.17.3.6/fgo_api_types/basic.py` & `fgo_api_types-2023.4.30.0.24.57/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.29.17.3.6/fgo_api_types/common.py` & `fgo_api_types-2023.4.30.0.24.57/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.29.17.3.6/fgo_api_types/enums.py` & `fgo_api_types-2023.4.30.0.24.57/fgo_api_types/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,14 +347,15 @@
     unknown = "unknown"
     agarthaPenth = "agarthaPenth"
     cccFinaleEmiyaAlter = "cccFinaleEmiyaAlter"
     salemAbby = "salemAbby"
     uOlgaMarie = "uOlgaMarie"
     uOlgaMarieAlienGod = "uOlgaMarieAlienGod"
     beast = "beast"
+    beastVI = "beastVI"
     atlasUnmappedClass = "atlasUnmappedClass"
     # OTHER = "OTHER"
     ALL = "ALL"
     # EXTRA = "EXTRA"
     # MIX = "MIX"
 
 
@@ -388,14 +389,15 @@
     27: SvtClass.beastUnknown,  # LB 5.2 beast
     28: SvtClass.pretender,
     29: SvtClass.beastIV,
     30: SvtClass.beastILost,
     31: SvtClass.uOlgaMarieAlienGod,
     32: SvtClass.uOlgaMarie,
     33: SvtClass.beast,
+    34: SvtClass.beastVI,
     97: SvtClass.unknown,
     # 98
     # 99
     # 100
     107: SvtClass.agarthaPenth,
     124: SvtClass.cccFinaleEmiyaAlter,
     125: SvtClass.salemAbby,
@@ -950,14 +952,15 @@
     chenGongNp = "chenGongNp"
     cantBeSacrificed = "cantBeSacrificed"
     gutsBlock = "gutsBlock"
     classBeastILost = "classBeastILost"
     holdingHolyGrail = "holdingHolyGrail"
     standardClassServant = "standardClassServant"
     classBeast = "classBeast"
+    classBeastVI = "classBeastVI"
 
 
 TRAIT_NAME: dict[int, Trait] = {
     1: Trait.genderMale,
     2: Trait.genderFemale,
     3: Trait.genderUnknown,
     100: Trait.classSaber,
@@ -981,14 +984,15 @@
     118: Trait.classBeastIIIL,
     119: Trait.classBeastUnknown,
     120: Trait.classPretender,
     121: Trait.classBeastIV,
     122: Trait.classBeastILost,
     123: Trait.classUOlgaMarie,
     124: Trait.classBeast,
+    125: Trait.classBeastVI,
     200: Trait.attributeSky,
     201: Trait.attributeEarth,
     202: Trait.attributeHuman,
     203: Trait.attributeStar,
     204: Trait.attributeBeast,
     300: Trait.alignmentLawful,
     301: Trait.alignmentChaotic,
```

### Comparing `fgo_api_types-2023.4.29.17.3.6/fgo_api_types/gameenums.py` & `fgo_api_types-2023.4.30.0.24.57/fgo_api_types/gameenums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.29.17.3.6/fgo_api_types/nice.py` & `fgo_api_types-2023.4.30.0.24.57/fgo_api_types/nice.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.29.17.3.6/fgo_api_types/raw.py` & `fgo_api_types-2023.4.30.0.24.57/fgo_api_types/raw.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.29.17.3.6/fgo_api_types/rayshift.py` & `fgo_api_types-2023.4.30.0.24.57/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.29.17.3.6/fgo_api_types/search.py` & `fgo_api_types-2023.4.30.0.24.57/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.29.17.3.6/pyproject.toml` & `fgo_api_types-2023.4.30.0.24.57/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2023.04.29.17.03.06"
+version = "2023.04.30.00.24.57"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2023.4.29.17.3.6/PKG-INFO` & `fgo_api_types-2023.4.30.0.24.57/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2023.4.29.17.3.6
+Version: 2023.4.30.0.24.57
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

