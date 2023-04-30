# Comparing `tmp/grai_source_flat_file-0.0.8.tar.gz` & `tmp/grai_source_flat_file-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_flat_file-0.0.8.tar", max compression
+gzip compressed data, was "grai_source_flat_file-0.0.9.tar", max compression
```

## Comparing `grai_source_flat_file-0.0.8.tar` & `grai_source_flat_file-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      713 2023-04-26 17:55:43.262066 grai_source_flat_file-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      147 2023-02-13 20:16:22.718033 grai_source_flat_file-0.0.8/src/grai_source_flat_file/__init__.py
--rw-r--r--   0        0        0     4437 2023-04-26 17:55:43.262318 grai_source_flat_file-0.0.8/src/grai_source_flat_file/adapters.py
--rw-r--r--   0        0        0      834 2023-02-13 20:16:22.718432 grai_source_flat_file-0.0.8/src/grai_source_flat_file/base.py
--rw-r--r--   0        0        0     2029 2023-04-17 19:49:39.123184 grai_source_flat_file-0.0.8/src/grai_source_flat_file/loader.py
--rw-r--r--   0        0        0      978 2023-02-13 20:16:22.718610 grai_source_flat_file-0.0.8/src/grai_source_flat_file/models.py
--rw-r--r--   0        0        0      188 2023-02-13 20:16:22.718657 grai_source_flat_file-0.0.8/src/grai_source_flat_file/package_definitions.py
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 grai_source_flat_file-0.0.8/setup.py
--rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 grai_source_flat_file-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      165 2023-04-29 00:58:02.883973 grai_source_flat_file-0.0.9/README.md
+-rw-r--r--   0        0        0      908 2023-04-30 17:37:11.522290 grai_source_flat_file-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      147 2023-02-13 20:16:22.718033 grai_source_flat_file-0.0.9/src/grai_source_flat_file/__init__.py
+-rw-r--r--   0        0        0     4437 2023-04-29 00:19:10.366840 grai_source_flat_file-0.0.9/src/grai_source_flat_file/adapters.py
+-rw-r--r--   0        0        0      834 2023-02-13 20:16:22.718432 grai_source_flat_file-0.0.9/src/grai_source_flat_file/base.py
+-rw-r--r--   0        0        0     2029 2023-04-17 19:49:39.123184 grai_source_flat_file-0.0.9/src/grai_source_flat_file/loader.py
+-rw-r--r--   0        0        0      978 2023-02-13 20:16:22.718610 grai_source_flat_file-0.0.9/src/grai_source_flat_file/models.py
+-rw-r--r--   0        0        0      188 2023-02-13 20:16:22.718657 grai_source_flat_file-0.0.9/src/grai_source_flat_file/package_definitions.py
+-rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 grai_source_flat_file-0.0.9/setup.py
+-rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 grai_source_flat_file-0.0.9/PKG-INFO
```

### Comparing `grai_source_flat_file-0.0.8/pyproject.toml` & `grai_source_flat_file-0.0.9/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 [tool.poetry]
 name = "grai_source_flat_file"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_flat_file", from = "src" },
 ]
+readme = "README.md"
+homepage = "https://www.grai.io/"
+repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-flat-file"
+documentation = "https://docs.grai.io/"
+
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
 grai-client = "^0.2.0"
 PyYAML = "^6.0"
 multimethod = "^1.8"
 pandas = "^1.4.4"
```

### Comparing `grai_source_flat_file-0.0.8/src/grai_source_flat_file/adapters.py` & `grai_source_flat_file-0.0.9/src/grai_source_flat_file/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_flat_file-0.0.8/src/grai_source_flat_file/base.py` & `grai_source_flat_file-0.0.9/src/grai_source_flat_file/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_flat_file-0.0.8/src/grai_source_flat_file/loader.py` & `grai_source_flat_file-0.0.9/src/grai_source_flat_file/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_flat_file-0.0.8/src/grai_source_flat_file/models.py` & `grai_source_flat_file-0.0.9/src/grai_source_flat_file/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_flat_file-0.0.8/PKG-INFO` & `grai_source_flat_file-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: grai-source-flat-file
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
+Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -14,7 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: grai-client (>=0.2.0,<0.3.0)
 Requires-Dist: grai-schemas (>=0.1.10,<0.2.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pandas (>=1.4.4,<2.0.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
+Project-URL: Documentation, https://docs.grai.io/
+Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-flat-file
+Description-Content-Type: text/markdown
+
+# Grai Flat File Integration
+
+The Flat File integration synchronizes metadata from flat files including csv, feather, and parquet into your Grai data lineage graph.
+
```

