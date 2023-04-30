# Comparing `tmp/botfleet-0.0.2-py3-none-any.whl.zip` & `tmp/botfleet-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2783 bytes, number of entries: 7
--rw-rw-r--  2.0 unx      466 b- defN 23-Mar-09 07:11 botfleet/__init__.py
--rw-rw-r--  2.0 unx      992 b- defN 23-Mar-08 19:36 botfleet/request.py
--rw-rw-r--  2.0 unx     1070 b- defN 23-Mar-09 07:12 botfleet-0.0.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx      235 b- defN 23-Mar-09 07:12 botfleet-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-09 07:12 botfleet-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Mar-09 07:12 botfleet-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      540 b- defN 23-Mar-09 07:12 botfleet-0.0.2.dist-info/RECORD
-7 files, 3404 bytes uncompressed, 1823 bytes compressed:  46.4%
+Zip file size: 2700 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx      185 b- defN 23-Apr-30 08:45 botfleet/__init__.py
+-rw-rw-r--  2.0 unx      992 b- defN 23-Apr-22 08:52 botfleet/request.py
+-rw-rw-r--  2.0 unx     1070 b- defN 23-Apr-30 08:51 botfleet-0.0.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      238 b- defN 23-Apr-30 08:51 botfleet-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-30 08:51 botfleet-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Apr-30 08:51 botfleet-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      540 b- defN 23-Apr-30 08:51 botfleet-0.0.3.dist-info/RECORD
+7 files, 3126 bytes uncompressed, 1740 bytes compressed:  44.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: botfleet/__init__.py
 Comment: 
 
 Filename: botfleet/request.py
 Comment: 
 
-Filename: botfleet-0.0.2.dist-info/LICENSE
+Filename: botfleet-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: botfleet-0.0.2.dist-info/METADATA
+Filename: botfleet-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: botfleet-0.0.2.dist-info/WHEEL
+Filename: botfleet-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: botfleet-0.0.2.dist-info/top_level.txt
+Filename: botfleet-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: botfleet-0.0.2.dist-info/RECORD
+Filename: botfleet-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## botfleet/__init__.py

```diff
@@ -1,17 +1,8 @@
 import os
-from pgdict import ConnectionConfig, Transaction, Store
+from storedict import create_store
 from .request import Request
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
-store = Store(
-    ConnectionConfig(
-        database=os.getenv("__BOTFLEET__DATABASE"),
-        table=os.getenv("__BOTFLEET__TABLE"),
-        user=os.getenv("__BOTFLEET__USER"),
-        password=os.getenv("__BOTFLEET__PASSWORD"),
-        host=os.getenv("__BOTFLEET__HOST"),
-        port=os.getenv("__BOTFLEET__PORT"),
-    )
-)
+store = create_store(os.getenv("__BOTFLEET__DATASTORE_PROXY_URL"))
 request = Request()
```

## Comparing `botfleet-0.0.2.dist-info/LICENSE` & `botfleet-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

