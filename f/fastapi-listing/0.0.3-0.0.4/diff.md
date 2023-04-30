# Comparing `tmp/fastapi-listing-0.0.3.tar.gz` & `tmp/fastapi-listing-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-listing-0.0.3.tar", last modified: Sat Apr 29 18:29:23 2023, max compression
+gzip compressed data, was "fastapi-listing-0.0.4.tar", last modified: Sun Apr 30 13:27:15 2023, max compression
```

## Comparing `fastapi-listing-0.0.3.tar` & `fastapi-listing-0.0.4.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.429780 fastapi-listing-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-29 18:29:23.429780 fastapi-listing-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.421779 fastapi-listing-0.0.3/fastapi_listing/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.421779 fastapi-listing-0.0.3/fastapi_listing/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/abstracts/base_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/abstracts/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/abstracts/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/abstracts/listing.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/abstracts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/abstracts/sorter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.421779 fastapi-listing-0.0.3/fastapi_listing/dao/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/dao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/dao/generic_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.425780 fastapi-listing-0.0.3/fastapi_listing/factory/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/factory/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/factory/generic_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/factory/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.425780 fastapi-listing-0.0.3/fastapi_listing/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/filters/generic_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.425780 fastapi-listing-0.0.3/fastapi_listing/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/interface/listing_meta_info.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.425780 fastapi-listing-0.0.3/fastapi_listing/mechanics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/mechanics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/mechanics/filter_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/mechanics/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/mechanics/sorter_mechanics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.425780 fastapi-listing-0.0.3/fastapi_listing/paginator/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/paginator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/paginator/naive_page_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.425780 fastapi-listing-0.0.3/fastapi_listing/service/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/service/listing_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.425780 fastapi-listing-0.0.3/fastapi_listing/sorter/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/sorter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/sorter/naive_page_sorter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.425780 fastapi-listing-0.0.3/fastapi_listing/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/strategies/query_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.421779 fastapi-listing-0.0.3/fastapi_listing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-29 18:29:23.000000 fastapi-listing-0.0.3/fastapi_listing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-29 18:29:23.000000 fastapi-listing-0.0.3/fastapi_listing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:29:23.000000 fastapi-listing-0.0.3/fastapi_listing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-29 18:29:23.000000 fastapi-listing-0.0.3/fastapi_listing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 18:29:23.000000 fastapi-listing-0.0.3/fastapi_listing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 18:29:23.429780 fastapi-listing-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.470801 fastapi-listing-0.0.4/fastapi_listing/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/abstracts/base_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/abstracts/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/abstracts/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/abstracts/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/abstracts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/abstracts/sorter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/dao/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/dao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/dao/generic_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/factory/_generic_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/factory/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/factory/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/filters/generic_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/interface/listing_meta_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/mechanics/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/mechanics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/mechanics/iterative_filter_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/mechanics/singleton_sorter_mechanics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/paginator/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/paginator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/paginator/naive_page_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13822 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/service/listing_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/sorter/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/sorter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/sorter/naive_page_sorter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/strategies/query_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.470801 fastapi-listing-0.0.4/fastapi_listing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-30 13:27:15.000000 fastapi-listing-0.0.4/fastapi_listing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-30 13:27:15.000000 fastapi-listing-0.0.4/fastapi_listing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 13:27:15.000000 fastapi-listing-0.0.4/fastapi_listing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-30 13:27:15.000000 fastapi-listing-0.0.4/fastapi_listing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 13:27:15.000000 fastapi-listing-0.0.4/fastapi_listing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/setup.py
```

### Comparing `fastapi-listing-0.0.3/PKG-INFO` & `fastapi-listing-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fastapi-listing
-Version: 0.0.3
+Version: 0.0.4
 Summary: Data Listing Library for FastAPI
 Home-page: https://github.com/danielhasan1/fastapi-listing
 Author: Danish Hasan
 Author-email: dh813030@gmail.com
 Keywords: starlette,fastapi,starlite,pydantic
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `fastapi-listing-0.0.3/fastapi_listing/abstracts/dao.py` & `fastapi-listing-0.0.4/fastapi_listing/abstracts/dao.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.3/fastapi_listing/abstracts/listing.py` & `fastapi-listing-0.0.4/fastapi_listing/abstracts/listing.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     @abstractmethod
     def _apply_filters(self, query: Query, listing_meta_info: ListingMetaInfo) -> Query:
         pass
 
     @abstractmethod
     def _paginate(self, query: Query, paginate_strategy: TableDataPaginatingStrategy,
-                 extra_context: dict) -> ListingResponseType:
+                  extra_context: dict) -> ListingResponseType:
         pass
 
     @abstractmethod
     def get_response(self, listing_meta_info: ListingMetaInfo) -> ListingResponseType:
         pass
 
 
@@ -83,8 +83,7 @@
     @abstractmethod
     def dao_kls(self) -> str:  # type:ignore # noqa
         ...
 
     @abstractmethod
     def get_listing(self):
         ...
-
```

### Comparing `fastapi-listing-0.0.3/fastapi_listing/dao/generic_dao.py` & `fastapi-listing-0.0.4/fastapi_listing/dao/generic_dao.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.3/fastapi_listing/factory/generic_factory.py` & `fastapi-listing-0.0.4/fastapi_listing/factory/_generic_factory.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.3/fastapi_listing/factory/strategy.py` & `fastapi-listing-0.0.4/fastapi_listing/factory/strategy.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.3/fastapi_listing/filters/generic_filters.py` & `fastapi-listing-0.0.4/fastapi_listing/filters/generic_filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from datetime import datetime
 
 from fastapi_listing.abstracts import FilterAbstract
 
 
 class CommonFilterImpl(FilterAbstract):
 
-    def __init__(self, dao=None, request=None, **kwargs):
+    def __init__(self, dao=None, request=None, extra_context=None):
         self.dao = dao
         self.request = request
+        self.extra_context = extra_context
 
     def filter(self, *, field: str = None, value: dict = None, query=None):
         raise NotImplementedError("To be implemented in child class!")
 
 
 class EqualityFilter(CommonFilterImpl):
```

### Comparing `fastapi-listing-0.0.3/fastapi_listing/interface/listing_meta_info.py` & `fastapi-listing-0.0.4/fastapi_listing/interface/listing_meta_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,19 @@
         ...
 
     @property
     def default_sort_val() -> dict[str, str]:  # type:ignore # noqa
         ...
 
     @property
-    def sorter_plugin() -> str:  # type:ignore # noqa
+    def sorter_mechanic() -> str:  # type:ignore # noqa
         ...
 
     @property
-    def filter_plugin() -> str:  # type:ignore # noqa
+    def filter_mechanic() -> str:  # type:ignore # noqa
         ...
 
     # @property
     # def router_params(self) -> dict:  # type: ignore # noqa
     #     ...
 
     @property
```

### Comparing `fastapi-listing-0.0.3/fastapi_listing/mechanics/loader.py` & `fastapi-listing-0.0.4/fastapi_listing/loader.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.3/fastapi_listing/paginator/naive_page_builder.py` & `fastapi-listing-0.0.4/fastapi_listing/paginator/naive_page_builder.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.3/fastapi_listing/service/listing_main.py` & `fastapi-listing-0.0.4/fastapi_listing/service/listing_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from fastapi import Request
 from sqlalchemy.orm import Query
 from json import JSONDecodeError
 from typing import Type, Optional
 
 from fastapi_listing import utils
 from fastapi_listing.abstracts import TableDataPaginatingStrategy
-from fastapi_listing.sorter import SortingOrderStrategy
-from fastapi_listing.typing import ListingResponseType, SqlAlchemyModel
+from fastapi_listing.typing import ListingResponseType
 from fastapi_listing.abstracts import ListingBase, ListingServiceBase
 from fastapi_listing.factory import strategy_factory
 from fastapi_listing.errors import ListingFilterError, ListingSorterError
 from fastapi_listing.dao.generic_dao import GenericDao
 from fastapi_listing.interface.listing_meta_info import ListingMetaInfo
-from fastapi_listing.factory import generic_factory
-from fastapi_listing.mechanics import loader
+from fastapi_listing.factory import _generic_factory
 
 try:
     from pydantic import BaseModel
 
     HAS_PYDANTIC = True
 except ImportError:
     HAS_PYDANTIC = False
@@ -29,15 +27,15 @@
     def __init__(self, request: Request, dao: GenericDao, pydantic_serializer: Optional[Type[BaseModel]] = None,
                  custom_fields: Optional[bool] = False) -> None:
         self.request = request
         self.dao = dao
         if HAS_PYDANTIC and pydantic_serializer:
             self.fields_to_fetch = list(pydantic_serializer.__fields__.keys())
         else:
-            self.fields_to_fetch = None
+            self.fields_to_fetch = []
         self.custom_fields = custom_fields
 
     def _replace_aliases(self, mapper: dict[str, str], req_params: list[dict[str, str]]) -> list[dict[str, str]]:
         req_prms_cpy = req_params.copy()
         for param in req_prms_cpy:
             param["field"] = mapper[param["field"]]
         return req_prms_cpy
@@ -73,18 +71,18 @@
         #                                                request=self.request)
         # sorting_strategy.sort(query=query, value=default_val)
 
         # fix this code
         # query = sorting_strategy.sort(value=sorting_params[-1],
         #                               query=query)
         def launch_mechanics(qry):
-            # for mechanics in listing_meta_info.sorter_plugins:
+            # for mechanics in listing_meta_info.sorter_mechanics:
             #     mecha: str = mechanics.split(".")[-1]
-            mecha: str = listing_meta_info.sorter_plugin
-            mecha_obj = generic_factory.create(mecha)
+            mecha: str = listing_meta_info.sorter_mechanic
+            mecha_obj = strategy_factory.create(mecha)
             qry = mecha_obj.apply(query=qry, strategy=listing_meta_info.sorting_strategy,
                                   sorting_params=sorting_params, extra_context=listing_meta_info.extra_context)
             return qry
 
         query = launch_mechanics(query)
         return query
 
@@ -103,15 +101,15 @@
 
         if temp := set(item.get("field") for item in fltrs) - set(listing_meta_info.filter_column_mapper.keys()):
             raise ListingFilterError(f"Filter'(s) not registered with listing: {temp}, Did you forget to do it?")
 
         fltrs = self._replace_aliases(listing_meta_info.filter_column_mapper, fltrs)
 
         def launch_mechanics(qry):
-            mecha_obj = generic_factory.create(listing_meta_info.filter_plugin)
+            mecha_obj = strategy_factory.create(listing_meta_info.filter_mechanic)
             qry = mecha_obj.apply(query=qry, filter_params=fltrs, dao=self.dao,
                                   request=self.request, extra_context=listing_meta_info.extra_context)
             return qry
 
         query = launch_mechanics(query)
         return query
 
@@ -149,16 +147,16 @@
     # here resource creation should be based on factory and not inline as we are separating creation from usage.
     # factory should deliver sorting resource
     DEFAULT_SRT_ON: str = "created_at"
     DEFAULT_SRT_ORD: str = "dsc"
     PAGINATE_STRATEGY: str = "naive_paginator"
     QUERY_STRATEGY: str = "naive_query"
     SORTING_STRATEGY: str = "naive_sorter"
-    SORT_MECHA: str = "sorter_mechanics"
-    FILTER_MECHA: str = "filter_mechanics"
+    SORT_MECHA: str = "singleton_sorter_mechanics"
+    FILTER_MECHA: str = "iterative_filter_mechanics"
     dao_kls: GenericDao = GenericDao
 
     # pydantic_serializer: Type[BaseModel] = None
     # allowed_pydantic_custom_fields: bool = False
     # it is possible to have more than one serializer for particular endpoint depending upon
     # user or a query/path param condition we could switch json schema so allowing this
     # flexibility for the user to be able to switch between schema Fastapilisting object
@@ -193,82 +191,93 @@
                         values["code"] = f'FANCY{values["id"]}CODE'
                 here code gets generated at runtime, code is not a table field, code is a custom field that is
                 deduced with the help of id.
         :return: page response for client to render
         """
         raise NotImplementedError("method should be implemented in child class and not here!")
 
-    def page_data_modifier(self, data: dict) -> dict:
-        raise NotImplementedError
+    # def page_data_modifier(self, data: dict) -> dict:
+    #     raise NotImplementedError
 
     class MetaInfo:
 
         def __init__(self, outer_instance):
-            self.paginating_strategy: TableDataPaginatingStrategy = strategy_factory.create(
+            self.paginating_strategy = strategy_factory.create(
                 outer_instance.PAGINATE_STRATEGY)
-            self.filter_column_mapper: dict = outer_instance.filter_mapper
-            self.query_strategy: Query = strategy_factory.create(outer_instance.QUERY_STRATEGY)
-            # self.sorting_column_mapper: dict = outer_instance.sort_mapper
-            self.default_sort_val: dict[str, str] = dict(type=outer_instance.DEFAULT_SRT_ORD,
-                                                         field=outer_instance.DEFAULT_SRT_ON)
-            self.sorting_strategy: SortingOrderStrategy = strategy_factory.create(
+            self.filter_column_mapper = outer_instance.filter_mapper
+            self.query_strategy = strategy_factory.create(outer_instance.QUERY_STRATEGY)
+            self.sorting_column_mapper = outer_instance.sort_mapper
+            self.default_sort_val = dict(type=outer_instance.DEFAULT_SRT_ORD,
+                                         field=outer_instance.DEFAULT_SRT_ON)
+            self.sorting_strategy = strategy_factory.create(
                 outer_instance.SORTING_STRATEGY,
                 model=outer_instance.dao.model,
                 request=outer_instance.request
             )
-            self.sorter_plugin: str = outer_instance.SORT_MECHA
-            self.filter_plugin: str = outer_instance.FILTER_MECHA
-            self.extra_context: dict = outer_instance.extra_context
+            self.sorter_mechanic = outer_instance.SORT_MECHA
+            self.filter_mechanic = outer_instance.FILTER_MECHA
+            self.extra_context = outer_instance.extra_context
 
     def meta_info_generator(self) -> ListingMetaInfo:
-        return ListingService.MetaInfo(self) # type:ignore # noqa # some issue is coming in pycharm for return types
+        return ListingService.MetaInfo(self)  # type:ignore # noqa # some issue is coming in pycharm for return types
 
     @classmethod
     def get_aliased_filter_mapper(cls) -> dict[str, str]:
         return {key: key for key, val in cls.filter_mapper.items()}
 
     @classmethod
     def get_aliased_sort_mapper(cls) -> dict[str, str]:
         return {key: key for key, val in cls.sort_mapper.items()}
 
-    @staticmethod
-    def get_sort_mecha_plugin_path() -> str:
-        """
-        hook to provide sort mecha plugin module path as py import path
-        overwrite allowed to provide custom path.
-        :return: import path as string ex. fastapi_listing.mechanics.sorter_mechanics.
-        """
-        return "fastapi_listing.mechanics.sorter_mechanics"
-
-    @staticmethod
-    def get_filter_mecha_plugin_path() -> str:
-        """
-       hook to provide filter mecha plugin module path as py import path
-       overwrite allowed to provide custom path.
-       :return: import path as string ex. fastapi_listing.mechanics.filter_mechanics.
-       """
-        return "fastapi_listing.mechanics.filter_mechanics"
-
-    @classmethod
-    def plugins_to_load(cls) -> list[str]:
-        """
-        Provided a hook to be called at module level of each listing service.
-        overwrite sort or filter plugin path getters to give your own custom
-        mechanic implementations.
-        refrain from overwriting it as this may change or it's fundamnetal
-        implementation is already broken down to pieces that can no longer
-        be broken any further. So instead of overwriting this
-        overwrite the individual pieces
-        :return: list plugins to load
-        currently only support sort/filter mecha loading
-        todo: can add pattern calling like %s_plugin_path for providing n number of plugin loading
-        """
-        return [cls.get_sort_mecha_plugin_path(), cls.get_filter_mecha_plugin_path()]
+    # @staticmethod
+    # def get_sort_mecha_plugin_path() -> str:
+    #     """
+    #     hook to provide sort mecha plugin module path as py import path
+    #     overwrite allowed to provide custom path.
+    #     :return: import path as string ex. fastapi_listing.mechanics.sorter_mechanics.
+    #     """
+    #     return "fastapi_listing.mechanics.sorter_mechanics"
+    #
+    # @staticmethod
+    # def get_filter_mecha_plugin_path() -> str:
+    #     """
+    #    hook to provide filter mecha plugin module path as py import path
+    #    overwrite allowed to provide custom path.
+    #    :return: import path as string ex. fastapi_listing.mechanics.filter_mechanics.
+    #    """
+    #     return "fastapi_listing.mechanics.filter_mechanics"
+    #
+    # @classmethod
+    # def plugins_to_load(cls) -> list[str]:
+    #     """
+    #     Provided a hook to be called at module level of each listing service.
+    #     overwrite sort or filter plugin path getters to give your own custom
+    #     mechanic implementations.
+    #     refrain from overwriting it as this may change or it's fundamnetal
+    #     implementation is already broken down to pieces that can no longer
+    #     be broken any further. So instead of overwriting this
+    #     overwrite the individual pieces
+    #     :return: list plugins to load
+    #     currently only support sort/filter mecha loading
+    #     todo: can add pattern calling like %s_plugin_path for providing n number of plugin loading
+    #     """
+    #     return [cls.get_sort_mecha_plugin_path(), cls.get_filter_mecha_plugin_path()]
 
 
 # calling loader at module level so once the module is loaded all plugins get loaded and not further loading is required
-loader.load_plugins(ListingService.plugins_to_load())
+# loader.load_plugins(ListingService.plugins_to_load())
+
 
 
 # todo: how to provide a hook in listing service so a person can easily overwrite the data list or manipulate it easily
 # todo: before wrapping it up in page response
 
+
+# page modifier has become abstract method in child class
+#
+# metainfo is causing issue due to its attributes types
+#
+# plugin is causing issue becuase when we load plugin in our child class first the module loads default plugin then our child class loads plugin
+# if one plugin is already loaded from our core module then child module tries to load it again and it shows error
+
+
+#appr 1 - we could centralise the loading process but it would benefit if we could understand plugin pattern in more depth
```

### Comparing `fastapi-listing-0.0.3/fastapi_listing/sorter/naive_page_sorter.py` & `fastapi-listing-0.0.4/fastapi_listing/sorter/naive_page_sorter.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,16 @@
         return query
 
     @staticmethod
     def sort_dsc_util(query: SqlAlchemyQuery, inst_field: AnySqlAlchemyColumn) -> SqlAlchemyQuery:
         query = query.order_by(inst_field.desc())
         return query
 
-    def sort(self, *, query: SqlAlchemyQuery = None, value: dict[str, str] = None) -> SqlAlchemyQuery:
+    def sort(self, *, query: SqlAlchemyQuery = None, value: dict[str, str] = None,
+             extra_context: dict = None) -> SqlAlchemyQuery:
         assert value["type"] in ["asc", "dsc"]
         if value is None:
             raise ValueError("sort expects value with structure [type, field], none provided")
         inst_field: AnySqlAlchemyColumn = self.validate_srt_field(self.model, value["field"])
         if value["type"] == "asc":
             query = self.sort_asc_util(query, inst_field)
         else:
@@ -32,10 +33,10 @@
     @staticmethod
     def validate_srt_field(model: SqlAlchemyModel, sort_field: str):
         try:
             inst_field = getattr(model, sort_field)
         except AttributeError:
             inst_field = None
         if inst_field is None:
-            raise ValueError(f"Provided sort field is not an attribute of {model}")  # todo improve this by custom exception
+            raise ValueError(
+                f"Provided sort field is not an attribute of {model}")  # todo improve this by custom exception
         return inst_field
-
```

### Comparing `fastapi-listing-0.0.3/fastapi_listing/strategies/query_strategy.py` & `fastapi-listing-0.0.4/fastapi_listing/strategies/query_strategy.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from fastapi_listing.typing import SqlAlchemyQuery, FastapiRequest
 
 
 class NaiveQueryStrategy(QueryStrategy):
 
     def get_inst_attr_to_read(self, custom_fields: bool, field_list: list, dao: GenericDao):
         inst_fields = []
+
         if custom_fields:
             # ("BYPASS CUSTOM PYDANTIC FIELDS ALLOWED.")
             # when serializer contains fields that get filled via validators or at runtime
             # or fields that get generated from model fields.
             for field in field_list:
                 try:
                     inst_fields.append(getattr(field, dao.model))
```

### Comparing `fastapi-listing-0.0.3/fastapi_listing/typing.py` & `fastapi-listing-0.0.4/fastapi_listing/typing.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.3/fastapi_listing.egg-info/PKG-INFO` & `fastapi-listing-0.0.4/fastapi_listing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fastapi-listing
-Version: 0.0.3
+Version: 0.0.4
 Summary: Data Listing Library for FastAPI
 Home-page: https://github.com/danielhasan1/fastapi-listing
 Author: Danish Hasan
 Author-email: dh813030@gmail.com
 Keywords: starlette,fastapi,starlite,pydantic
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `fastapi-listing-0.0.3/fastapi_listing.egg-info/SOURCES.txt` & `fastapi-listing-0.0.4/fastapi_listing.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 README.md
 setup.py
 fastapi_listing/__init__.py
 fastapi_listing/errors.py
-fastapi_listing/logger.py
+fastapi_listing/loader.py
 fastapi_listing/py.typed
 fastapi_listing/typing.py
 fastapi_listing/utils.py
 fastapi_listing.egg-info/PKG-INFO
 fastapi_listing.egg-info/SOURCES.txt
 fastapi_listing.egg-info/dependency_links.txt
 fastapi_listing.egg-info/requires.txt
@@ -17,25 +17,24 @@
 fastapi_listing/abstracts/filter.py
 fastapi_listing/abstracts/listing.py
 fastapi_listing/abstracts/paginator.py
 fastapi_listing/abstracts/sorter.py
 fastapi_listing/dao/__init__.py
 fastapi_listing/dao/generic_dao.py
 fastapi_listing/factory/__init__.py
+fastapi_listing/factory/_generic_factory.py
 fastapi_listing/factory/filter.py
-fastapi_listing/factory/generic_factory.py
 fastapi_listing/factory/strategy.py
 fastapi_listing/filters/__init__.py
 fastapi_listing/filters/generic_filters.py
 fastapi_listing/interface/__init__.py
 fastapi_listing/interface/listing_meta_info.py
 fastapi_listing/mechanics/__init__.py
-fastapi_listing/mechanics/filter_mechanics.py
-fastapi_listing/mechanics/loader.py
-fastapi_listing/mechanics/sorter_mechanics.py
+fastapi_listing/mechanics/iterative_filter_mechanics.py
+fastapi_listing/mechanics/singleton_sorter_mechanics.py
 fastapi_listing/paginator/__init__.py
 fastapi_listing/paginator/naive_page_builder.py
 fastapi_listing/service/__init__.py
 fastapi_listing/service/listing_main.py
 fastapi_listing/sorter/__init__.py
 fastapi_listing/sorter/naive_page_sorter.py
 fastapi_listing/strategies/__init__.py
```

