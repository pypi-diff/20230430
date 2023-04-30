# Comparing `tmp/transitmatters-gtfs-0.1.1.tar.gz` & `tmp/transitmatters-gtfs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transitmatters-gtfs-0.1.1.tar", max compression
+gzip compressed data, was "transitmatters-gtfs-0.1.2.tar", max compression
```

## Comparing `transitmatters-gtfs-0.1.1.tar` & `transitmatters-gtfs-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      497 2023-04-30 02:18:34.451611 transitmatters-gtfs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       68 2023-04-30 02:18:05.644080 transitmatters-gtfs-0.1.1/transitmatters_gtfs/__init__.py
--rw-r--r--   0        0        0     1145 2023-04-30 01:46:13.753099 transitmatters-gtfs-0.1.1/transitmatters_gtfs/archive.py
--rw-r--r--   0        0        0      311 2023-04-30 01:46:20.093206 transitmatters-gtfs-0.1.1/transitmatters_gtfs/compact.py
--rw-r--r--   0        0        0      164 2023-04-30 01:39:28.291450 transitmatters-gtfs-0.1.1/transitmatters_gtfs/config.py
--rw-r--r--   0        0        0     4301 2023-04-30 01:48:22.201014 transitmatters-gtfs-0.1.1/transitmatters_gtfs/feed.py
--rw-r--r--   0        0        0     6553 2023-04-29 20:50:51.459384 transitmatters-gtfs-0.1.1/transitmatters_gtfs/ingest.py
--rw-r--r--   0        0        0      299 2023-04-30 02:17:41.015128 transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/__init__.py
--rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/base.py
--rw-r--r--   0        0        0     1425 2023-03-30 02:56:28.913999 transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/calendar.py
--rw-r--r--   0        0        0     1441 2023-03-30 20:23:01.651025 transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/calendar_attributes.py
--rw-r--r--   0        0        0      791 2023-04-29 21:48:26.317752 transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/calendar_dates.py
--rw-r--r--   0        0        0      807 2023-04-29 21:47:57.353684 transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/feed_info.py
--rw-r--r--   0        0        0      564 2023-03-30 02:52:49.339781 transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/lines.py
--rw-r--r--   0        0        0     1181 2023-03-30 20:23:23.703663 transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/route_patterns.py
--rw-r--r--   0        0        0     1544 2023-04-29 21:53:03.435048 transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/routes.py
--rw-r--r--   0        0        0      466 2023-03-30 20:23:34.688831 transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/shapes.py
--rw-r--r--   0        0        0      857 2023-03-31 02:58:26.702834 transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/stop_times.py
--rw-r--r--   0        0        0     2219 2023-04-29 21:55:20.302317 transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/stops.py
--rw-r--r--   0        0        0     1645 2023-03-31 02:48:43.538213 transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/transfers.py
--rw-r--r--   0        0        0     1875 2023-04-29 21:56:24.896980 transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/trips.py
--rw-r--r--   0        0        0     1503 2023-04-29 22:18:11.002315 transitmatters-gtfs-0.1.1/transitmatters_gtfs/reader.py
--rw-r--r--   0        0        0      310 2023-04-30 01:48:24.420010 transitmatters-gtfs-0.1.1/transitmatters_gtfs/session.py
--rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 transitmatters-gtfs-0.1.1/transitmatters_gtfs/utils/decorators.py
--rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 transitmatters-gtfs-0.1.1/transitmatters_gtfs/utils/enum.py
--rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 transitmatters-gtfs-0.1.1/transitmatters_gtfs/utils/time.py
--rw-r--r--   0        0        0      808 2023-04-30 02:18:39.936125 transitmatters-gtfs-0.1.1/setup.py
--rw-r--r--   0        0        0      576 2023-04-30 02:18:39.936382 transitmatters-gtfs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      497 2023-04-30 02:24:09.526619 transitmatters-gtfs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-04-30 02:24:02.217122 transitmatters-gtfs-0.1.2/transitmatters_gtfs/__init__.py
+-rw-r--r--   0        0        0     1148 2023-04-30 02:20:02.920626 transitmatters-gtfs-0.1.2/transitmatters_gtfs/archive.py
+-rw-r--r--   0        0        0      312 2023-04-30 02:20:13.261136 transitmatters-gtfs-0.1.2/transitmatters_gtfs/compact.py
+-rw-r--r--   0        0        0      164 2023-04-30 01:39:28.291450 transitmatters-gtfs-0.1.2/transitmatters_gtfs/config.py
+-rw-r--r--   0        0        0     4304 2023-04-30 02:20:22.143888 transitmatters-gtfs-0.1.2/transitmatters_gtfs/feed.py
+-rw-r--r--   0        0        0     6569 2023-04-30 02:20:47.608682 transitmatters-gtfs-0.1.2/transitmatters_gtfs/ingest.py
+-rw-r--r--   0        0        0      299 2023-04-30 02:17:41.015128 transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/__init__.py
+-rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/base.py
+-rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/calendar.py
+-rw-r--r--   0        0        0     1437 2023-04-30 02:21:50.513446 transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/calendar_attributes.py
+-rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/calendar_dates.py
+-rw-r--r--   0        0        0      801 2023-04-30 02:22:10.347470 transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/feed_info.py
+-rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/lines.py
+-rw-r--r--   0        0        0     1177 2023-04-30 02:22:19.299183 transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/route_patterns.py
+-rw-r--r--   0        0        0     1540 2023-04-30 02:22:29.021433 transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/routes.py
+-rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/shapes.py
+-rw-r--r--   0        0        0      851 2023-04-30 02:22:40.117387 transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/stop_times.py
+-rw-r--r--   0        0        0     2209 2023-04-30 02:22:46.094390 transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/stops.py
+-rw-r--r--   0        0        0     1641 2023-04-30 02:22:51.048772 transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/transfers.py
+-rw-r--r--   0        0        0     1865 2023-04-30 02:22:59.207780 transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/trips.py
+-rw-r--r--   0        0        0     1503 2023-04-29 22:18:11.002315 transitmatters-gtfs-0.1.2/transitmatters_gtfs/reader.py
+-rw-r--r--   0        0        0      311 2023-04-30 02:20:52.918874 transitmatters-gtfs-0.1.2/transitmatters_gtfs/session.py
+-rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 transitmatters-gtfs-0.1.2/transitmatters_gtfs/utils/decorators.py
+-rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 transitmatters-gtfs-0.1.2/transitmatters_gtfs/utils/enum.py
+-rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 transitmatters-gtfs-0.1.2/transitmatters_gtfs/utils/time.py
+-rw-r--r--   0        0        0      808 2023-04-30 02:24:13.942202 transitmatters-gtfs-0.1.2/setup.py
+-rw-r--r--   0        0        0      576 2023-04-30 02:24:13.942431 transitmatters-gtfs-0.1.2/PKG-INFO
```

### Comparing `transitmatters-gtfs-0.1.1/transitmatters_gtfs/archive.py` & `transitmatters-gtfs-0.1.2/transitmatters_gtfs/archive.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from datetime import date
 from typing import List, Union
 from csv import DictReader
 
 
 import requests
 
-from utils.time import date_from_string
-from feed import GtfsFeed
-from config import MBTA_GTFS_ARCHIVE_URL
+from .utils.time import date_from_string
+from .feed import GtfsFeed
+from .config import MBTA_GTFS_ARCHIVE_URL
 
 
 def list_feeds_from_archive(
     load_start_date: Union[date, None] = None,
     archive_url: str = MBTA_GTFS_ARCHIVE_URL,
 ) -> List[GtfsFeed]:
     req = requests.get(archive_url)
```

### Comparing `transitmatters-gtfs-0.1.1/transitmatters_gtfs/feed.py` & `transitmatters-gtfs-0.1.2/transitmatters_gtfs/feed.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from zipfile import ZipFile, BadZipFile
 from hashlib import md5
 
 
 import requests
 from tqdm import tqdm
 
-from utils.time import date_to_string
-from reader import GtfsReader
-from session import create_sqlalchemy_session
+from .utils.time import date_to_string
+from .reader import GtfsReader
+from .session import create_sqlalchemy_session
 
 
 class GtfsFeed:
     def __init__(
         self,
         feeds_root: str,
         start_date: date,
```

### Comparing `transitmatters-gtfs-0.1.1/transitmatters_gtfs/ingest.py` & `transitmatters-gtfs-0.1.2/transitmatters_gtfs/ingest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from sqlalchemy.orm import Session
 from typing import Dict, Any, Callable, List, Union, Type, Iterable
 
-from archive import GtfsFeedDownload
-from utils.time import date_from_string, seconds_from_string
-from utils.decorators import listify
-from models.base import Base
-from models.calendar_attributes import CalendarAttribute
-from models.calendar_dates import CalendarServiceException
-from models.calendar import CalendarService
-from models.feed_info import FeedInfo
-from models.lines import Line
-from models.route_patterns import RoutePattern
-from models.routes import Route
-from models.shapes import ShapePoint
-from models.stops import Stop
-from models.stop_times import StopTime
-from models.transfers import Transfer
-from models.trips import Trip
+from .archive import GtfsFeedDownload
+from .utils.time import date_from_string, seconds_from_string
+from .utils.decorators import listify
+from .models.base import Base
+from .models.calendar_attributes import CalendarAttribute
+from .models.calendar_dates import CalendarServiceException
+from .models.calendar import CalendarService
+from .models.feed_info import FeedInfo
+from .models.lines import Line
+from .models.route_patterns import RoutePattern
+from .models.routes import Route
+from .models.shapes import ShapePoint
+from .models.stops import Stop
+from .models.stop_times import StopTime
+from .models.transfers import Transfer
+from .models.trips import Trip
 
 RowTransform = Callable[[str], any]
 RowTransforms = Dict[str, RowTransform]
 
 
 def nullable(transform: RowTransform) -> RowTransform:
     def inner_transform(val: str):
```

### Comparing `transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/base.py` & `transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/base.py`

 * *Files identical despite different names*

### Comparing `transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/calendar.py` & `transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/calendar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from enum import Enum
 from datetime import date
 from typing import Literal
 
 from sqlalchemy.types import Date, String
 from sqlalchemy.orm import mapped_column, Mapped
 
-from models.base import Base
-from utils.enum import gtfs_enum_type
+from .base import Base
+from ..utils.enum import gtfs_enum_type
 
 
 class ServiceDayAvailability(Enum):
     NOT_AVAILABLE = "0"
     AVAILABLE = "1"
```

### Comparing `transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/calendar_attributes.py` & `transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/calendar_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from enum import Enum
 from typing import Literal
 from datetime import date
 
 from sqlalchemy.types import String, Date
 from sqlalchemy.orm import mapped_column, Mapped
 
-from models.base import Base
-from utils.enum import gtfs_enum_type
+from .base import Base
+from ..utils.enum import gtfs_enum_type
 
 
 class ServiceScheduleTypicality(Enum):
     NOT_DEFINED = "0"
     MINOR_MODIFICATIONS = "1"
     EXTRA_SERVICE = "2"
     REDUCED_TO_WEEKEND_SERVICE = "3"
```

### Comparing `transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/calendar_dates.py` & `transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/calendar_dates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from enum import Enum
 from typing import Literal
 import datetime
 
 from sqlalchemy.types import Date, String
 from sqlalchemy.orm import mapped_column, Mapped
 
-from models.base import Base
-from utils.enum import gtfs_enum_type
+from .base import Base
+from ..utils.enum import gtfs_enum_type
 
 
 class CalendarServiceExceptionType(Enum):
     ADDED = "1"
     REMOVED = "2"
```

### Comparing `transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/feed_info.py` & `transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/feed_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import date
 
 from sqlalchemy.types import Date, String
 from sqlalchemy.orm import mapped_column, Mapped
 
-from models.base import Base
+from .base import Base
 
 
 class FeedInfo(Base):
     feed_publisher_name: Mapped[str] = mapped_column(String)
     feed_publisher_url: Mapped[str] = mapped_column(String)
     feed_lang: Mapped[str] = mapped_column(String)
     feed_start_date: Mapped[date] = mapped_column(Date)
```

### Comparing `transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/lines.py` & `transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/lines.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sqlalchemy.types import String
 from sqlalchemy.orm import mapped_column, Mapped
 
-from models.base import Base
+from .base import Base
 
 
 class Line(Base):
     line_id: Mapped[str] = mapped_column(String)
     line_short_name: Mapped[str] = mapped_column(String)
     line_long_name: Mapped[str] = mapped_column(String)
     line_desc: Mapped[str] = mapped_column(String)
```

### Comparing `transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/route_patterns.py` & `transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/route_patterns.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 from typing import Literal
 
 from sqlalchemy.types import String, Integer
 from sqlalchemy.orm import mapped_column, Mapped
 
-from models.base import Base
-from utils.enum import gtfs_enum_type
+from .base import Base
+from ..utils.enum import gtfs_enum_type
 
 
 class RoutePatternTypicality(Enum):
     NOT_DEFINED = "0"
     TYPICAL = "1"
     DEVIATION = "2"
     HIGHLY_ATYPICAL = "3"
```

### Comparing `transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/routes.py` & `transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 from typing import Literal
 
 from sqlalchemy.types import String, Integer
 from sqlalchemy.orm import mapped_column, Mapped
 
-from models.base import Base
-from utils.enum import gtfs_enum_type
+from .base import Base
+from ..utils.enum import gtfs_enum_type
 
 
 class RouteType(Enum):
     NOT_SPECIFIED = ""  # Not in GTFS but seen in a lot of Trips
     TRAM = "0"
     METRO = "1"
     RAIL = "2"
```

### Comparing `transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/stop_times.py` & `transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/stop_times.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sqlalchemy.types import String, Integer
 from sqlalchemy.orm import mapped_column, Mapped
 
-from models.base import Base
+from .base import Base
 
 
 class StopTime(Base):
     trip_id: Mapped[str] = mapped_column(String, index=True)
     stop_id: Mapped[str] = mapped_column(String, index=True)
     arrival_time: Mapped[int] = mapped_column(Integer)
     departure_time: Mapped[int] = mapped_column(Integer)
```

### Comparing `transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/stops.py` & `transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/stops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from enum import Enum
 from typing import Literal
 
 from sqlalchemy.types import String, Float
 from sqlalchemy.orm import mapped_column, Mapped
 
-from models.base import Base
-from models.routes import RouteType, TRouteType
-from utils.enum import gtfs_enum_type
+from .base import Base
+from .routes import RouteType, TRouteType
+from ..utils.enum import gtfs_enum_type
 
 
 class LocationType(Enum):
     STOP = "0"
     STATION = "1"
     ENTRANCE_EXIT = "2"
     GENERIC_NODE = "3"
```

### Comparing `transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/transfers.py` & `transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/transfers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 from typing import Literal
 
 from sqlalchemy.types import String, Integer
 from sqlalchemy.orm import mapped_column, Mapped
 
-from models.base import Base
-from utils.enum import gtfs_enum_type
+from .base import Base
+from ..utils.enum import gtfs_enum_type
 
 
 class TransferType(Enum):
     RECOMMENDED = "0"
     TIMED = "1"
     REQUIRES_MINIMUM_TIME = "2"
     NOT_POSSIBLE = "3"
```

### Comparing `transitmatters-gtfs-0.1.1/transitmatters_gtfs/models/trips.py` & `transitmatters-gtfs-0.1.2/transitmatters_gtfs/models/trips.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from enum import Enum
 from typing import Literal
 
 from sqlalchemy.types import String, Integer
 from sqlalchemy.orm import mapped_column, Mapped
 
-from models.base import Base
-from models.routes import RouteType, TRouteType
-from utils.enum import gtfs_enum_type
+from .base import Base
+from .routes import RouteType, TRouteType
+from ..utils.enum import gtfs_enum_type
 
 
 class WheelchairAccessibility(Enum):
     NO_INFORMATION = "0"
     ACCESSIBLE = "1"
     NOT_ACCESSIBLE = "2"
```

### Comparing `transitmatters-gtfs-0.1.1/transitmatters_gtfs/reader.py` & `transitmatters-gtfs-0.1.2/transitmatters_gtfs/reader.py`

 * *Files identical despite different names*

### Comparing `transitmatters-gtfs-0.1.1/transitmatters_gtfs/utils/time.py` & `transitmatters-gtfs-0.1.2/transitmatters_gtfs/utils/time.py`

 * *Files identical despite different names*

### Comparing `transitmatters-gtfs-0.1.1/setup.py` & `transitmatters-gtfs-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ['SQLAlchemy>=2.0.7,<3.0.0',
  'boto3>=1.26.123,<2.0.0',
  'requests>=2.28.2,<3.0.0',
  'tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'transitmatters-gtfs',
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

### Comparing `transitmatters-gtfs-0.1.1/PKG-INFO` & `transitmatters-gtfs-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transitmatters-gtfs
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

