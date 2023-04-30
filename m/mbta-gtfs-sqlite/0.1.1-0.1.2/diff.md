# Comparing `tmp/mbta-gtfs-sqlite-0.1.1.tar.gz` & `tmp/mbta-gtfs-sqlite-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbta-gtfs-sqlite-0.1.1.tar", max compression
+gzip compressed data, was "mbta-gtfs-sqlite-0.1.2.tar", max compression
```

## Comparing `mbta-gtfs-sqlite-0.1.1.tar` & `mbta-gtfs-sqlite-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       68 2023-04-30 02:24:02.217122 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/__init__.py
--rw-r--r--   0        0        0     1203 2023-04-30 02:31:00.196926 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/archive.py
--rw-r--r--   0        0        0      312 2023-04-30 02:20:13.261136 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/compact.py
--rw-r--r--   0        0        0      164 2023-04-30 01:39:28.291450 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/config.py
--rw-r--r--   0        0        0     4346 2023-04-30 03:18:02.390080 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/feed.py
--rw-r--r--   0        0        0     6569 2023-04-30 02:20:47.608682 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/ingest.py
--rw-r--r--   0        0        0      299 2023-04-30 02:17:41.015128 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/__init__.py
--rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/base.py
--rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/calendar.py
--rw-r--r--   0        0        0     1437 2023-04-30 02:21:50.513446 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/calendar_attributes.py
--rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/calendar_dates.py
--rw-r--r--   0        0        0      801 2023-04-30 02:22:10.347470 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/feed_info.py
--rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/lines.py
--rw-r--r--   0        0        0     1177 2023-04-30 02:22:19.299183 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/route_patterns.py
--rw-r--r--   0        0        0     1540 2023-04-30 02:22:29.021433 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/routes.py
--rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/shapes.py
--rw-r--r--   0        0        0      851 2023-04-30 02:22:40.117387 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/stop_times.py
--rw-r--r--   0        0        0     2209 2023-04-30 02:22:46.094390 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/stops.py
--rw-r--r--   0        0        0     1641 2023-04-30 02:22:51.048772 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/transfers.py
--rw-r--r--   0        0        0     1865 2023-04-30 02:22:59.207780 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/trips.py
--rw-r--r--   0        0        0     1503 2023-04-29 22:18:11.002315 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/reader.py
--rw-r--r--   0        0        0      311 2023-04-30 02:20:52.918874 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/session.py
--rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/utils/decorators.py
--rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/utils/enum.py
--rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/utils/time.py
--rw-r--r--   0        0        0      491 2023-04-30 03:19:29.643431 mbta-gtfs-sqlite-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      794 2023-04-30 03:19:40.468426 mbta-gtfs-sqlite-0.1.1/setup.py
--rw-r--r--   0        0        0      573 2023-04-30 03:19:40.468708 mbta-gtfs-sqlite-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       68 2023-04-30 02:24:02.217122 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/__init__.py
+-rw-r--r--   0        0        0     1203 2023-04-30 02:31:00.196926 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/archive.py
+-rw-r--r--   0        0        0      312 2023-04-30 02:20:13.261136 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/compact.py
+-rw-r--r--   0        0        0      164 2023-04-30 01:39:28.291450 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/config.py
+-rw-r--r--   0        0        0     4346 2023-04-30 03:26:50.789460 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/feed.py
+-rw-r--r--   0        0        0     6505 2023-04-30 03:27:20.093974 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/ingest.py
+-rw-r--r--   0        0        0      299 2023-04-30 02:17:41.015128 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/__init__.py
+-rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/base.py
+-rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/calendar.py
+-rw-r--r--   0        0        0     1437 2023-04-30 02:21:50.513446 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/calendar_attributes.py
+-rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/calendar_dates.py
+-rw-r--r--   0        0        0      801 2023-04-30 02:22:10.347470 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/feed_info.py
+-rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/lines.py
+-rw-r--r--   0        0        0     1177 2023-04-30 02:22:19.299183 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/route_patterns.py
+-rw-r--r--   0        0        0     1540 2023-04-30 02:22:29.021433 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/routes.py
+-rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/shapes.py
+-rw-r--r--   0        0        0      851 2023-04-30 02:22:40.117387 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/stop_times.py
+-rw-r--r--   0        0        0     2209 2023-04-30 02:22:46.094390 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/stops.py
+-rw-r--r--   0        0        0     1641 2023-04-30 02:22:51.048772 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/transfers.py
+-rw-r--r--   0        0        0     1865 2023-04-30 02:22:59.207780 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/trips.py
+-rw-r--r--   0        0        0     1503 2023-04-29 22:18:11.002315 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/reader.py
+-rw-r--r--   0        0        0      311 2023-04-30 02:20:52.918874 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/session.py
+-rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/utils/decorators.py
+-rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/utils/enum.py
+-rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/utils/time.py
+-rw-r--r--   0        0        0      491 2023-04-30 03:27:49.752418 mbta-gtfs-sqlite-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      794 2023-04-30 03:27:54.858659 mbta-gtfs-sqlite-0.1.2/setup.py
+-rw-r--r--   0        0        0      573 2023-04-30 03:27:54.858950 mbta-gtfs-sqlite-0.1.2/PKG-INFO
```

### Comparing `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/archive.py` & `mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/archive.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/feed.py` & `mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/feed.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/ingest.py` & `mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/ingest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sqlalchemy.orm import Session
 from typing import Dict, Any, Callable, List, Union, Type, Iterable
 
-from .archive import GtfsFeedDownload
+from .archive import GtfsFeed
 from .utils.time import date_from_string, seconds_from_string
 from .utils.decorators import listify
 from .models.base import Base
 from .models.calendar_attributes import CalendarAttribute
 from .models.calendar_dates import CalendarServiceException
 from .models.calendar import CalendarService
 from .models.feed_info import FeedInfo
@@ -70,25 +70,25 @@
         yield {
             **trip_row,
             "start_time": stop_times_for_trip[0]["arrival_time"],
             "end_time": stop_times_for_trip[-1]["arrival_time"],
         }
 
 
-def ingest_feed_info(session: Session, download: GtfsFeedDownload) -> FeedInfo:
+def ingest_feed_info(session: Session, feed: GtfsFeed) -> FeedInfo:
     num_feed_infos = session.query(FeedInfo).count()
     next_id = 1 + num_feed_infos
-    feed_info_dict_raw = next(download.reader.read_feed_info())
+    feed_info_dict_raw = next(feed.reader.read_feed_info())
     feed_info_dict = transform_row_dict(
         {
             **feed_info_dict_raw,
             "id": next_id,
             "feed_info_id": next_id,
-            "retrieved_from_url": download.feed.remote_url,
-            "zip_md5_checksum": download.zip_md5_checksum,
+            "retrieved_from_url": feed.url,
+            "zip_md5_checksum": feed.zip_md5_checksum,
         },
         {
             "feed_start_date": date_from_string,
             "feed_end_date": date_from_string,
         },
     )
     feed_info = FeedInfo(**feed_info_dict)
@@ -115,17 +115,17 @@
     if individually:
         for mapping in mappings:
             session.add(model(**mapping))
     else:
         session.bulk_insert_mappings(model, mappings)
 
 
-def ingest_gtfs_csv_into_db(session: Session, download: GtfsFeedDownload):
-    reader = download.reader
-    feed_info = ingest_feed_info(session, download)
+def ingest_gtfs_csv_into_db(session: Session, feed: GtfsFeed):
+    reader = feed.reader
+    feed_info = ingest_feed_info(session, feed)
     stop_times = list(reader.read_stop_times())
     trips = list(reader.read_trips())
     trip_rows = get_trip_rows_with_extra_time_fields(trips, stop_times)
     ingest_rows(
         session=session,
         model=CalendarService,
         feed_info=feed_info,
```

### Comparing `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/base.py` & `mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/base.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/calendar.py` & `mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/calendar.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/calendar_attributes.py` & `mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/calendar_attributes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/calendar_dates.py` & `mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/calendar_dates.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/feed_info.py` & `mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/feed_info.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/lines.py` & `mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/lines.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/route_patterns.py` & `mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/route_patterns.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/routes.py` & `mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/routes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/stop_times.py` & `mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/stop_times.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/stops.py` & `mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/stops.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/transfers.py` & `mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/transfers.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/models/trips.py` & `mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/models/trips.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/reader.py` & `mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/reader.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.1/mbta_gtfs_sqlite/utils/time.py` & `mbta-gtfs-sqlite-0.1.2/mbta_gtfs_sqlite/utils/time.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.1.1/setup.py` & `mbta-gtfs-sqlite-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['SQLAlchemy>=2.0.7,<3.0.0',
  'boto3>=1.26.123,<2.0.0',
  'requests>=2.28.2,<3.0.0',
  'tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'mbta-gtfs-sqlite',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': "Query the MBTA's static GTFS feeds using sqlite",
     'long_description': None,
     'author': 'Ian Reynolds',
     'author_email': 'ireynolds@transitmatters.info',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `mbta-gtfs-sqlite-0.1.1/PKG-INFO` & `mbta-gtfs-sqlite-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbta-gtfs-sqlite
-Version: 0.1.1
+Version: 0.1.2
 Summary: Query the MBTA's static GTFS feeds using sqlite
 Author: Ian Reynolds
 Author-email: ireynolds@transitmatters.info
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```

