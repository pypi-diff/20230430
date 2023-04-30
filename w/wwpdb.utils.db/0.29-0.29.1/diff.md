# Comparing `tmp/wwpdb.utils.db-0.29.tar.gz` & `tmp/wwpdb.utils.db-0.29.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.db-0.29.tar", last modified: Fri Oct 28 01:52:47 2022, max compression
+gzip compressed data, was "wwpdb.utils.db-0.29.1.tar", last modified: Sun Apr 30 13:18:37 2023, max compression
```

## Comparing `wwpdb.utils.db-0.29.tar` & `wwpdb.utils.db-0.29.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-28 01:52:47.537093 wwpdb.utils.db-0.29/
--rw-r--r--   0 vsts      (1001) docker     (121)      719 2022-10-28 01:52:47.537093 wwpdb.utils.db-0.29/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      212 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/README.md
--rw-r--r--   0 vsts      (1001) docker     (121)      108 2022-10-28 01:52:47.537093 wwpdb.utils.db-0.29/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (121)     2165 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-28 01:52:47.525093 wwpdb.utils.db-0.29/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (121)       65 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-28 01:52:47.529093 wwpdb.utils.db-0.29/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (121)       65 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-28 01:52:47.537093 wwpdb.utils.db-0.29/wwpdb/utils/db/
--rw-r--r--   0 vsts      (1001) docker     (121)   237963 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/BirdSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (121)   150990 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/ChemCompSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4802 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/DBLoadUtil.py
--rw-r--r--   0 vsts      (1001) docker     (121)   260559 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/DaInternalSchemaDef.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)    22118 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/DbLoadingApi.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7042 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/MessageSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8889 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/MyConnectionBase.py
--rw-r--r--   0 vsts      (1001) docker     (121)    19146 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/MyDbAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (121)    30645 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/MyDbSqlGen.py
--rw-r--r--   0 vsts      (1001) docker     (121)    17636 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/MyDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (121)    23832 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/MyQueryDirectives.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4815 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/MysqlSchemaImporter.py
--rw-r--r--   0 vsts      (1001) docker     (121)   606730 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/PdbDistroSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (121)  3724930 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/PdbxSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (121)    12178 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/PdbxSchemaMapReader.py
--rw-r--r--   0 vsts      (1001) docker     (121)   150992 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/PrdChemCompSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (121)    15722 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/SchemaDefBase.py
--rw-r--r--   0 vsts      (1001) docker     (121)    26185 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/SchemaDefLoader.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7057 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/SqlLoader.py
--rw-r--r--   0 vsts      (1001) docker     (121)    12147 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/StatusHistory.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6744 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/StatusHistoryExec.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8873 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/StatusHistorySchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (121)    32566 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/StatusHistoryUtils.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1829 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/StatusLoadWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (121)    27651 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/WorkflowSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (121)      154 2022-10-28 01:51:48.000000 wwpdb.utils.db-0.29/wwpdb/utils/db/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-28 01:52:47.529093 wwpdb.utils.db-0.29/wwpdb.utils.db.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)      719 2022-10-28 01:52:47.000000 wwpdb.utils.db-0.29/wwpdb.utils.db.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1177 2022-10-28 01:52:47.000000 wwpdb.utils.db-0.29/wwpdb.utils.db.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-10-28 01:52:47.000000 wwpdb.utils.db-0.29/wwpdb.utils.db.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-10-28 01:52:19.000000 wwpdb.utils.db-0.29/wwpdb.utils.db.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)      139 2022-10-28 01:52:47.000000 wwpdb.utils.db-0.29/wwpdb.utils.db.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        6 2022-10-28 01:52:47.000000 wwpdb.utils.db-0.29/wwpdb.utils.db.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:18:37.564038 wwpdb.utils.db-0.29.1/
+-rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-04-30 13:18:37.564038 wwpdb.utils.db-0.29.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      212 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-04-30 13:18:37.564038 wwpdb.utils.db-0.29.1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2165 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:18:37.556038 wwpdb.utils.db-0.29.1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:18:37.556038 wwpdb.utils.db-0.29.1/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:18:37.564038 wwpdb.utils.db-0.29.1/wwpdb/utils/db/
+-rw-r--r--   0 vsts      (1001) docker     (123)   237963 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/BirdSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   150990 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/ChemCompSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4802 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/DBLoadUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   260559 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/DaInternalSchemaDef.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    22118 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/DbLoadingApi.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7042 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/MessageSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8889 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/MyConnectionBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19146 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/MyDbAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    30645 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/MyDbSqlGen.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17636 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/MyDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    23832 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/MyQueryDirectives.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4815 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/MysqlSchemaImporter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   606730 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/PdbDistroSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (123)  3724930 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/PdbxSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12178 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/PdbxSchemaMapReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   150992 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/PrdChemCompSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15722 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/SchemaDefBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    26185 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/SchemaDefLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7057 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/SqlLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12147 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/StatusHistory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6744 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/StatusHistoryExec.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8873 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/StatusHistorySchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    32566 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/StatusHistoryUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1829 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/StatusLoadWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    27651 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/WorkflowSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      156 2023-04-30 13:17:34.000000 wwpdb.utils.db-0.29.1/wwpdb/utils/db/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:18:37.556038 wwpdb.utils.db-0.29.1/wwpdb.utils.db.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-04-30 13:18:37.000000 wwpdb.utils.db-0.29.1/wwpdb.utils.db.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1177 2023-04-30 13:18:37.000000 wwpdb.utils.db-0.29.1/wwpdb.utils.db.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-30 13:18:37.000000 wwpdb.utils.db-0.29.1/wwpdb.utils.db.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-30 13:18:22.000000 wwpdb.utils.db-0.29.1/wwpdb.utils.db.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      139 2023-04-30 13:18:37.000000 wwpdb.utils.db-0.29.1/wwpdb.utils.db.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-04-30 13:18:37.000000 wwpdb.utils.db-0.29.1/wwpdb.utils.db.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.db-0.29/PKG-INFO` & `wwpdb.utils.db-0.29.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.db
-Version: 0.29
+Version: 0.29.1
 Summary: wwPDB Python DB Schema Utilities
 Home-page: https://github.com/rcsb/py-wwpdb_utils_db
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.db-0.29/setup.py` & `wwpdb.utils.db-0.29.1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/BirdSchemaDef.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/BirdSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/ChemCompSchemaDef.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/ChemCompSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/DBLoadUtil.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/DBLoadUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/DaInternalSchemaDef.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/DaInternalSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/DbLoadingApi.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/DbLoadingApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/MessageSchemaDef.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/MessageSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/MyConnectionBase.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/MyConnectionBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/MyDbAdapter.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/MyDbAdapter.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/MyDbSqlGen.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/MyDbSqlGen.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/MyDbUtil.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/MyDbUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/MyQueryDirectives.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/MyQueryDirectives.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/MysqlSchemaImporter.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/MysqlSchemaImporter.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/PdbDistroSchemaDef.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/PdbDistroSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/PdbxSchemaDef.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/PdbxSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/PdbxSchemaMapReader.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/PdbxSchemaMapReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/PrdChemCompSchemaDef.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/PrdChemCompSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/SchemaDefBase.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/SchemaDefBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/SchemaDefLoader.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/SchemaDefLoader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/SqlLoader.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/SqlLoader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/StatusHistory.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/StatusHistory.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/StatusHistoryExec.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/StatusHistoryExec.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/StatusHistorySchemaDef.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/StatusHistorySchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/StatusHistoryUtils.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/StatusHistoryUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/StatusLoadWrapper.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/StatusLoadWrapper.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb/utils/db/WorkflowSchemaDef.py` & `wwpdb.utils.db-0.29.1/wwpdb/utils/db/WorkflowSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.29/wwpdb.utils.db.egg-info/PKG-INFO` & `wwpdb.utils.db-0.29.1/wwpdb.utils.db.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.db
-Version: 0.29
+Version: 0.29.1
 Summary: wwPDB Python DB Schema Utilities
 Home-page: https://github.com/rcsb/py-wwpdb_utils_db
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.db-0.29/wwpdb.utils.db.egg-info/SOURCES.txt` & `wwpdb.utils.db-0.29.1/wwpdb.utils.db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

