# Comparing `tmp/grai_source_dbt-0.2.8.tar.gz` & `tmp/grai_source_dbt-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_dbt-0.2.8.tar", max compression
+gzip compressed data, was "grai_source_dbt-0.2.9.tar", max compression
```

## Comparing `grai_source_dbt-0.2.8.tar` & `grai_source_dbt-0.2.9.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0      735 2023-04-26 17:55:43.260977 grai_source_dbt-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      187 2023-02-23 22:53:26.660798 grai_source_dbt-0.2.8/src/grai_source_dbt/__init__.py
--rw-r--r--   0        0        0      112 2023-02-23 22:53:26.660996 grai_source_dbt-0.2.8/src/grai_source_dbt/adapters/__init__.py
--rw-r--r--   0        0        0     5993 2023-04-26 17:55:43.261193 grai_source_dbt-0.2.8/src/grai_source_dbt/adapters/adapters.py
--rw-r--r--   0        0        0      531 2023-04-17 19:49:39.119946 grai_source_dbt-0.2.8/src/grai_source_dbt/adapters/v5.py
--rw-r--r--   0        0        0      802 2023-03-22 16:41:59.040971 grai_source_dbt-0.2.8/src/grai_source_dbt/base.py
--rw-r--r--   0        0        0    30063 2023-01-03 17:11:14.023697 grai_source_dbt-0.2.8/src/grai_source_dbt/data/graph.gpickle
--rw-r--r--   0        0        0   249725 2023-01-03 17:11:14.024284 grai_source_dbt-0.2.8/src/grai_source_dbt/data/manifest.json
--rw-r--r--   0        0        0      764 2023-02-23 22:53:26.661735 grai_source_dbt-0.2.8/src/grai_source_dbt/data_tools.py
--rw-r--r--   0        0        0     1881 2023-02-23 22:53:26.661938 grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/__init__.py
--rw-r--r--   0        0        0      940 2023-02-23 22:53:26.662122 grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/base.py
--rw-r--r--   0        0        0      199 2023-02-23 22:53:26.662264 grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/utils.py
--rw-r--r--   0        0        0     5493 2023-04-17 19:21:38.342251 grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/v1.py
--rw-r--r--   0        0        0     1032 2023-02-23 22:53:26.662601 grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/v2.py
--rw-r--r--   0        0        0     1033 2023-02-23 22:53:26.662723 grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/v3.py
--rw-r--r--   0        0        0     1109 2023-02-23 22:53:26.662932 grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/v4.py
--rw-r--r--   0        0        0     1108 2023-02-23 22:53:26.663082 grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/v5.py
--rw-r--r--   0        0        0     1108 2023-02-23 22:53:26.663291 grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/v6.py
--rw-r--r--   0        0        0     2172 2023-02-28 23:36:16.178370 grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/v7.py
--rw-r--r--   0        0        0      549 2023-02-23 22:53:26.663499 grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/v8.py
--rw-r--r--   0        0        0       48 2023-02-23 22:53:26.663732 grai_source_dbt-0.2.8/src/grai_source_dbt/models/__init__.py
--rw-r--r--   0        0        0     2182 2023-02-28 23:36:16.178561 grai_source_dbt-0.2.8/src/grai_source_dbt/models/grai.py
--rw-r--r--   0        0        0     2350 2023-02-13 20:16:22.716054 grai_source_dbt-0.2.8/src/grai_source_dbt/models/shared.py
--rw-r--r--   0        0        0      176 2023-02-13 20:16:22.716226 grai_source_dbt-0.2.8/src/grai_source_dbt/package_definitions.py
--rw-r--r--   0        0        0     1893 2023-02-28 23:36:16.178761 grai_source_dbt-0.2.8/src/grai_source_dbt/processor.py
--rw-r--r--   0        0        0        0 2023-01-03 17:11:14.024727 grai_source_dbt-0.2.8/src/grai_source_dbt/py.typed
--rw-r--r--   0        0        0      981 2023-02-28 23:34:46.003147 grai_source_dbt-0.2.8/src/grai_source_dbt/utils.py
--rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 grai_source_dbt-0.2.8/setup.py
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 grai_source_dbt-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      124 2023-04-29 00:58:02.883723 grai_source_dbt-0.2.9/README.md
+-rw-r--r--   0        0        0      924 2023-04-30 17:37:05.392599 grai_source_dbt-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      187 2023-02-23 22:53:26.660798 grai_source_dbt-0.2.9/src/grai_source_dbt/__init__.py
+-rw-r--r--   0        0        0      112 2023-02-23 22:53:26.660996 grai_source_dbt-0.2.9/src/grai_source_dbt/adapters/__init__.py
+-rw-r--r--   0        0        0     5993 2023-04-29 00:19:10.365667 grai_source_dbt-0.2.9/src/grai_source_dbt/adapters/adapters.py
+-rw-r--r--   0        0        0      531 2023-04-17 19:49:39.119946 grai_source_dbt-0.2.9/src/grai_source_dbt/adapters/v5.py
+-rw-r--r--   0        0        0      802 2023-03-22 16:41:59.040971 grai_source_dbt-0.2.9/src/grai_source_dbt/base.py
+-rw-r--r--   0        0        0    30063 2023-01-03 17:11:14.023697 grai_source_dbt-0.2.9/src/grai_source_dbt/data/graph.gpickle
+-rw-r--r--   0        0        0   249725 2023-01-03 17:11:14.024284 grai_source_dbt-0.2.9/src/grai_source_dbt/data/manifest.json
+-rw-r--r--   0        0        0      764 2023-02-23 22:53:26.661735 grai_source_dbt-0.2.9/src/grai_source_dbt/data_tools.py
+-rw-r--r--   0        0        0     1881 2023-02-23 22:53:26.661938 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/__init__.py
+-rw-r--r--   0        0        0      940 2023-02-23 22:53:26.662122 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/base.py
+-rw-r--r--   0        0        0      199 2023-02-23 22:53:26.662264 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/utils.py
+-rw-r--r--   0        0        0     5493 2023-04-17 19:21:38.342251 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v1.py
+-rw-r--r--   0        0        0     1032 2023-02-23 22:53:26.662601 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v2.py
+-rw-r--r--   0        0        0     1033 2023-02-23 22:53:26.662723 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v3.py
+-rw-r--r--   0        0        0     1109 2023-02-23 22:53:26.662932 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v4.py
+-rw-r--r--   0        0        0     1108 2023-02-23 22:53:26.663082 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v5.py
+-rw-r--r--   0        0        0     1108 2023-02-23 22:53:26.663291 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v6.py
+-rw-r--r--   0        0        0     2172 2023-02-28 23:36:16.178370 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v7.py
+-rw-r--r--   0        0        0      549 2023-02-23 22:53:26.663499 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v8.py
+-rw-r--r--   0        0        0       48 2023-02-23 22:53:26.663732 grai_source_dbt-0.2.9/src/grai_source_dbt/models/__init__.py
+-rw-r--r--   0        0        0     2182 2023-02-28 23:36:16.178561 grai_source_dbt-0.2.9/src/grai_source_dbt/models/grai.py
+-rw-r--r--   0        0        0     2350 2023-02-13 20:16:22.716054 grai_source_dbt-0.2.9/src/grai_source_dbt/models/shared.py
+-rw-r--r--   0        0        0      176 2023-02-13 20:16:22.716226 grai_source_dbt-0.2.9/src/grai_source_dbt/package_definitions.py
+-rw-r--r--   0        0        0     1893 2023-02-28 23:36:16.178761 grai_source_dbt-0.2.9/src/grai_source_dbt/processor.py
+-rw-r--r--   0        0        0        0 2023-01-03 17:11:14.024727 grai_source_dbt-0.2.9/src/grai_source_dbt/py.typed
+-rw-r--r--   0        0        0      981 2023-02-28 23:34:46.003147 grai_source_dbt-0.2.9/src/grai_source_dbt/utils.py
+-rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 grai_source_dbt-0.2.9/setup.py
+-rw-r--r--   0        0        0      996 1970-01-01 00:00:00.000000 grai_source_dbt-0.2.9/PKG-INFO
```

### Comparing `grai_source_dbt-0.2.8/pyproject.toml` & `grai_source_dbt-0.2.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 [tool.poetry]
 name = "grai_source_dbt"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_dbt", from = "src" },
 ]
+readme = "README.md"
+homepage = "https://www.grai.io/"
+repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-dbt"
+documentation = "https://docs.grai.io/"
+
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
 grai-client = "^0.2.0"
 grai-schemas = "^0.1.10"
 dbt-artifacts-parser = "^0.2.4"
```

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/adapters/adapters.py` & `grai_source_dbt-0.2.9/src/grai_source_dbt/adapters/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/adapters/v5.py` & `grai_source_dbt-0.2.9/src/grai_source_dbt/adapters/v5.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/base.py` & `grai_source_dbt-0.2.9/src/grai_source_dbt/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/data/graph.gpickle` & `grai_source_dbt-0.2.9/src/grai_source_dbt/data/graph.gpickle`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/data/manifest.json` & `grai_source_dbt-0.2.9/src/grai_source_dbt/data/manifest.json`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/data_tools.py` & `grai_source_dbt-0.2.9/src/grai_source_dbt/data_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/__init__.py` & `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/base.py` & `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/v1.py` & `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v1.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/v2.py` & `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v2.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/v3.py` & `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v3.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/v4.py` & `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v4.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/v5.py` & `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v5.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/v6.py` & `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v6.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/v7.py` & `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v7.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/loaders/v8.py` & `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v8.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/models/grai.py` & `grai_source_dbt-0.2.9/src/grai_source_dbt/models/grai.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/models/shared.py` & `grai_source_dbt-0.2.9/src/grai_source_dbt/models/shared.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/processor.py` & `grai_source_dbt-0.2.9/src/grai_source_dbt/processor.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.8/src/grai_source_dbt/utils.py` & `grai_source_dbt-0.2.9/src/grai_source_dbt/utils.py`

 * *Files identical despite different names*

