# Comparing `tmp/mbta-gtfs-sqlite-0.1.0.tar.gz` & `tmp/mbta-gtfs-sqlite-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbta-gtfs-sqlite-0.1.0.tar", max compression
+gzip compressed data, was "mbta-gtfs-sqlite-0.1.1.tar", max compression
```

## Comparing `mbta-gtfs-sqlite-0.1.0.tar` & `mbta-gtfs-sqlite-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       68 2023-04-30 02:24:02.217122 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/__init__.py
--rw-r--r--   0        0        0     1203 2023-04-30 02:31:00.196926 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/archive.py
--rw-r--r--   0        0        0      312 2023-04-30 02:20:13.261136 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/compact.py
--rw-r--r--   0        0        0      164 2023-04-30 01:39:28.291450 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/config.py
--rw-r--r--   0        0        0     4344 2023-04-30 02:33:15.274472 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/feed.py
--rw-r--r--   0        0        0     6569 2023-04-30 02:20:47.608682 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/ingest.py
--rw-r--r--   0        0        0      299 2023-04-30 02:17:41.015128 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/__init__.py
--rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/base.py
--rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/calendar.py
--rw-r--r--   0        0        0     1437 2023-04-30 02:21:50.513446 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/calendar_attributes.py
--rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/calendar_dates.py
--rw-r--r--   0        0        0      801 2023-04-30 02:22:10.347470 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/feed_info.py
--rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/lines.py
--rw-r--r--   0        0        0     1177 2023-04-30 02:22:19.299183 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/route_patterns.py
--rw-r--r--   0        0        0     1540 2023-04-30 02:22:29.021433 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/routes.py
--rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/shapes.py
--rw-r--r--   0        0        0      851 2023-04-30 02:22:40.117387 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/stop_times.py
--rw-r--r--   0        0        0     2209 2023-04-30 02:22:46.094390 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/stops.py
--rw-r--r--   0        0        0     1641 2023-04-30 02:22:51.048772 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/transfers.py
--rw-r--r--   0        0        0     1865 2023-04-30 02:22:59.207780 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/trips.py
--rw-r--r--   0        0        0     1503 2023-04-29 22:18:11.002315 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/reader.py
--rw-r--r--   0        0        0      311 2023-04-30 02:20:52.918874 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/session.py
--rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/utils/decorators.py
--rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/utils/enum.py
--rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/utils/time.py
--rw-r--r--   0        0        0      491 2023-04-30 03:08:09.594517 mbta-gtfs-sqlite-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      794 2023-04-30 03:08:30.651248 mbta-gtfs-sqlite-0.1.0/setup.py
--rw-r--r--   0        0        0      573 2023-04-30 03:08:30.651550 mbta-gtfs-sqlite-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       68 2023-04-30 02:24:02.217122 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/__init__.py
+-rw-r--r--   0        0        0     1203 2023-04-30 02:31:00.196926 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/archive.py
+-rw-r--r--   0        0        0      312 2023-04-30 02:20:13.261136 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/compact.py
+-rw-r--r--   0        0        0      164 2023-04-30 01:39:28.291450 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/config.py
+-rw-r--r--   0        0        0     4346 2023-04-30 03:18:02.390080 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/feed.py
+-rw-r--r--   0        0        0     6569 2023-04-30 02:20:47.608682 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/ingest.py
+-rw-r--r--   0        0        0      299 2023-04-30 02:17:41.015128 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/__init__.py
+-rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/base.py
+-rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/calendar.py
+-rw-r--r--   0        0        0     1437 2023-04-30 02:21:50.513446 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/calendar_attributes.py
+-rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/calendar_dates.py
+-rw-r--r--   0        0        0      801 2023-04-30 02:22:10.347470 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/feed_info.py
+-rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/lines.py
+-rw-r--r--   0        0        0     1177 2023-04-30 02:22:19.299183 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/route_patterns.py
+-rw-r--r--   0        0        0     1540 2023-04-30 02:22:29.021433 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/routes.py
+-rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/shapes.py
+-rw-r--r--   0        0        0      851 2023-04-30 02:22:40.117387 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/stop_times.py
+-rw-r--r--   0        0        0     2209 2023-04-30 02:22:46.094390 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/stops.py
+-rw-r--r--   0        0        0     1641 2023-04-30 02:22:51.048772 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/transfers.py
+-rw-r--r--   0        0        0     1865 2023-04-30 02:22:59.207780 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/trips.py
+-rw-r--r--   0        0        0     1503 2023-04-29 22:18:11.002315 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/reader.py
+-rw-r--r--   0        0        0      311 2023-04-30 02:20:52.918874 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/session.py
+-rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/utils/decorators.py
+-rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/utils/enum.py
+-rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/utils/time.py
+-rw-r--r--   0        0        0      491 2023-04-30 03:19:29.643431 mbta-gtfs-sqlite-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      794 2023-04-30 03:19:40.468426 mbta-gtfs-sqlite-0.1.1/setup.py
+-rw-r--r--   0        0        0      573 2023-04-30 03:19:40.468708 mbta-gtfs-sqlite-0.1.1/PKG-INFO
```

### Comparing `mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/archive.py` & `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/archive.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/feed.py` & `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/feed.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,30 +110,30 @@
             zf = ZipFile(self.gtfs_zip_path)
             zf.extractall(self.gtfs_subdir_path)
         except BadZipFile:
             print(f"Bad zip file: {self.gtfs_zip_path}")
         return target_path
 
     def ingest_to_db(self):
-        from ingest import ingest_gtfs_csv_into_db
+        from .ingest import ingest_gtfs_csv_into_db
 
         try:
             self.unzip()
             target_path = self.sqlite_db_path
             if path.exists(target_path):
                 return target_path
             session = create_sqlalchemy_session(target_path)
             ingest_gtfs_csv_into_db(session, self)
             return target_path
         except Exception:
             remove(target_path)
             raise
 
     def compactify_db(self):
-        from compact import make_compact_db
+        from .compact import make_compact_db
 
         self.ingest_to_db()
         target_path = self.sqlite_compact_db_path
         if path.exists(target_path):
             return target_path
         try:
             copy(self.sqlite_db_path, target_path)
```

### Comparing `mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/ingest.py` & `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/ingest.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/base.py` & `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/base.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/calendar.py` & `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/calendar.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/calendar_attributes.py` & `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/calendar_attributes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/calendar_dates.py` & `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/calendar_dates.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/feed_info.py` & `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/feed_info.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/lines.py` & `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/lines.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/route_patterns.py` & `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/route_patterns.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/routes.py` & `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/routes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/stop_times.py` & `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/stop_times.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/stops.py` & `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/stops.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/transfers.py` & `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/transfers.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/models/trips.py` & `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/trips.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/reader.py` & `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/reader.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.0/mbta_gtfs_sqlite/utils/time.py` & `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/utils/time.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.0/setup.py` & `mbta-gtfs-sqlite-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['SQLAlchemy>=2.0.7,<3.0.0',
  'boto3>=1.26.123,<2.0.0',
  'requests>=2.28.2,<3.0.0',
  'tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'mbta-gtfs-sqlite',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': "Query the MBTA's static GTFS feeds using sqlite",
     'long_description': None,
     'author': 'Ian Reynolds',
     'author_email': 'ireynolds@transitmatters.info',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `mbta-gtfs-sqlite-0.1.0/PKG-INFO` & `mbta-gtfs-sqlite-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbta-gtfs-sqlite
-Version: 0.1.0
+Version: 0.1.1
 Summary: Query the MBTA's static GTFS feeds using sqlite
 Author: Ian Reynolds
 Author-email: ireynolds@transitmatters.info
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```

