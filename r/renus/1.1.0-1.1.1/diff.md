# Comparing `tmp/renus-1.1.0.tar.gz` & `tmp/renus-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renus-1.1.0.tar", last modified: Thu Apr 20 05:38:00 2023, max compression
+gzip compressed data, was "renus-1.1.1.tar", last modified: Sun Apr 30 01:03:54 2023, max compression
```

## Comparing `renus-1.1.0.tar` & `renus-1.1.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.844318 renus-1.1.0/
--rw-rw-rw-   0        0        0     1539 2022-12-08 07:04:23.000000 renus-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       37 2023-04-20 05:31:47.000000 renus-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      220 2023-04-20 05:38:00.844318 renus-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.378322 renus-1.1.0/renus/
--rw-rw-rw-   0        0        0        0 2023-04-20 05:37:22.000000 renus-1.1.0/renus/__init__.py
--rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.1.0/renus/app.py
-drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.490378 renus-1.1.0/renus/commands/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.545339 renus-1.1.0/renus/commands/app/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/commands/app/__init__.py
--rw-rw-rw-   0        0        0     1787 2023-04-18 05:34:21.000000 renus-1.1.0/renus/commands/app/controller.temp
--rw-rw-rw-   0        0        0      979 2023-04-18 05:34:20.000000 renus-1.1.0/renus/commands/app/model.temp
--rw-rw-rw-   0        0        0      518 2023-03-14 08:51:15.000000 renus-1.1.0/renus/commands/app/route.temp
--rw-rw-rw-   0        0        0     4144 2022-10-15 05:56:43.000000 renus-1.1.0/renus/commands/app/run.py
--rw-rw-rw-   0        0        0      211 2022-10-09 08:00:32.000000 renus-1.1.0/renus/commands/app/vue.temp
-drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.567322 renus-1.1.0/renus/commands/backup/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/commands/backup/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.1.0/renus/commands/backup/run.py
-drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.585327 renus-1.1.0/renus/commands/copy/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/commands/copy/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.1.0/renus/commands/copy/run.py
-drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.588322 renus-1.1.0/renus/commands/default/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/commands/default/__init__.py
--rw-rw-rw-   0        0        0     2153 2023-04-20 05:35:39.000000 renus-1.1.0/renus/commands/default/run.py
--rw-rw-rw-   0        0        0     1416 2023-04-15 07:24:18.000000 renus-1.1.0/renus/commands/help.py
-drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.615321 renus-1.1.0/renus/commands/install/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/commands/install/__init__.py
--rw-rw-rw-   0        0        0     4079 2023-03-12 17:31:41.000000 renus-1.1.0/renus/commands/install/build.py
--rw-rw-rw-   0        0        0     3946 2023-03-12 07:22:04.000000 renus-1.1.0/renus/commands/install/run.py
--rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.1.0/renus/commands/install/service.py
-drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.617324 renus-1.1.0/renus/commands/permission/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/commands/permission/__init__.py
--rw-rw-rw-   0        0        0      704 2023-04-20 05:35:39.000000 renus-1.1.0/renus/commands/permission/run.py
--rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.1.0/renus/commands/run.py
-drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.812322 renus-1.1.0/renus/core/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/core/__init__.py
--rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.1.0/renus/core/cache.py
--rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.1.0/renus/core/concurrency.py
--rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.1.0/renus/core/config.py
--rw-rw-rw-   0        0        0     2098 2023-04-15 09:01:12.000000 renus-1.1.0/renus/core/crypt.py
--rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.1.0/renus/core/datastructures.py
--rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.1.0/renus/core/exception.py
--rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.1.0/renus/core/formparsers.py
--rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.1.0/renus/core/injection.py
--rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.1.0/renus/core/log.py
--rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.1.0/renus/core/middleware.py
--rw-rw-rw-   0        0        0    14287 2023-04-18 05:31:57.000000 renus-1.1.0/renus/core/model.py
--rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.1.0/renus/core/request.py
--rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.1.0/renus/core/response.py
--rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.1.0/renus/core/routing.py
--rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.1.0/renus/core/schedule.py
--rw-rw-rw-   0        0        0     1448 2023-01-22 09:14:04.000000 renus-1.1.0/renus/core/serialize.py
--rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.1.0/renus/core/status.py
-drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.832318 renus-1.1.0/renus/core/validation/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/core/validation/__init__.py
--rw-rw-rw-   0        0        0     8773 2022-10-23 08:35:28.000000 renus-1.1.0/renus/core/validation/rules.py
--rw-rw-rw-   0        0        0     3235 2022-08-31 08:30:44.000000 renus-1.1.0/renus/core/validation/validate.py
--rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.1.0/renus/core/websockets.py
-drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.842318 renus-1.1.0/renus/util/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/util/__init__.py
--rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.1.0/renus/util/helper.py
-drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.426356 renus-1.1.0/renus.egg-info/
--rw-rw-rw-   0        0        0      220 2023-04-20 05:38:00.000000 renus-1.1.0/renus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1405 2023-04-20 05:38:00.000000 renus-1.1.0/renus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 05:38:00.000000 renus-1.1.0/renus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-20 05:38:00.000000 renus-1.1.0/renus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 05:38:00.845319 renus-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      334 2023-04-20 05:37:22.000000 renus-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:03:54.803207 renus-1.1.1/
+-rw-rw-rw-   0        0        0     1539 2022-12-08 07:04:23.000000 renus-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-04-20 05:31:47.000000 renus-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      220 2023-04-30 01:03:54.802196 renus-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 01:03:53.806980 renus-1.1.1/renus/
+-rw-rw-rw-   0        0        0        0 2023-04-20 05:37:22.000000 renus-1.1.1/renus/__init__.py
+-rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.1.1/renus/app.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:03:53.909525 renus-1.1.1/renus/commands/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:03:53.987582 renus-1.1.1/renus/commands/app/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/commands/app/__init__.py
+-rw-rw-rw-   0        0        0     1787 2023-04-18 05:34:21.000000 renus-1.1.1/renus/commands/app/controller.temp
+-rw-rw-rw-   0        0        0     1033 2023-04-20 17:58:46.000000 renus-1.1.1/renus/commands/app/model.temp
+-rw-rw-rw-   0        0        0      518 2023-03-14 08:51:15.000000 renus-1.1.1/renus/commands/app/route.temp
+-rw-rw-rw-   0        0        0     4144 2022-10-15 05:56:43.000000 renus-1.1.1/renus/commands/app/run.py
+-rw-rw-rw-   0        0        0      211 2022-10-09 08:00:32.000000 renus-1.1.1/renus/commands/app/vue.temp
+drwxrwxrwx   0        0        0        0 2023-04-30 01:03:54.016918 renus-1.1.1/renus/commands/backup/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/commands/backup/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.1.1/renus/commands/backup/run.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:03:54.035919 renus-1.1.1/renus/commands/copy/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/commands/copy/__init__.py
+-rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.1.1/renus/commands/copy/run.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:03:54.074492 renus-1.1.1/renus/commands/default/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/commands/default/__init__.py
+-rw-rw-rw-   0        0        0     2153 2023-04-20 05:35:39.000000 renus-1.1.1/renus/commands/default/run.py
+-rw-rw-rw-   0        0        0     1416 2023-04-15 07:24:18.000000 renus-1.1.1/renus/commands/help.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:03:54.171744 renus-1.1.1/renus/commands/install/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/commands/install/__init__.py
+-rw-rw-rw-   0        0        0     4079 2023-03-12 17:31:41.000000 renus-1.1.1/renus/commands/install/build.py
+-rw-rw-rw-   0        0        0     3946 2023-03-12 07:22:04.000000 renus-1.1.1/renus/commands/install/run.py
+-rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.1.1/renus/commands/install/service.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:03:54.197297 renus-1.1.1/renus/commands/permission/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/commands/permission/__init__.py
+-rw-rw-rw-   0        0        0      704 2023-04-20 05:35:39.000000 renus-1.1.1/renus/commands/permission/run.py
+-rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.1.1/renus/commands/run.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:03:54.716928 renus-1.1.1/renus/core/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/core/__init__.py
+-rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.1.1/renus/core/cache.py
+-rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.1.1/renus/core/concurrency.py
+-rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.1.1/renus/core/config.py
+-rw-rw-rw-   0        0        0     2098 2023-04-15 09:01:12.000000 renus-1.1.1/renus/core/crypt.py
+-rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.1.1/renus/core/datastructures.py
+-rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.1.1/renus/core/exception.py
+-rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.1.1/renus/core/formparsers.py
+-rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.1.1/renus/core/injection.py
+-rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.1.1/renus/core/log.py
+-rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.1.1/renus/core/middleware.py
+-rw-rw-rw-   0        0        0    14800 2023-04-20 18:01:14.000000 renus-1.1.1/renus/core/model.py
+-rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.1.1/renus/core/request.py
+-rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.1.1/renus/core/response.py
+-rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.1.1/renus/core/routing.py
+-rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.1.1/renus/core/schedule.py
+-rw-rw-rw-   0        0        0     1448 2023-01-22 09:14:04.000000 renus-1.1.1/renus/core/serialize.py
+-rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.1.1/renus/core/status.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:03:54.779210 renus-1.1.1/renus/core/validation/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/core/validation/__init__.py
+-rw-rw-rw-   0        0        0     8773 2022-10-23 08:35:28.000000 renus-1.1.1/renus/core/validation/rules.py
+-rw-rw-rw-   0        0        0     3235 2022-08-31 08:30:44.000000 renus-1.1.1/renus/core/validation/validate.py
+-rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.1.1/renus/core/websockets.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:03:54.799195 renus-1.1.1/renus/util/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/util/__init__.py
+-rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.1.1/renus/util/helper.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:03:53.838979 renus-1.1.1/renus.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-04-30 01:03:53.000000 renus-1.1.1/renus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1405 2023-04-30 01:03:53.000000 renus-1.1.1/renus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 01:03:53.000000 renus-1.1.1/renus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-30 01:03:53.000000 renus-1.1.1/renus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 01:03:54.804209 renus-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      334 2023-04-30 01:02:27.000000 renus-1.1.1/setup.py
```

### Comparing `renus-1.1.0/LICENSE` & `renus-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/app.py` & `renus-1.1.1/renus/app.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/commands/app/controller.temp` & `renus-1.1.1/renus/commands/app/controller.temp`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/commands/app/model.temp` & `renus-1.1.1/renus/commands/app/model.temp`

 * *Files 6% similar despite different names*

```diff
@@ -15,21 +15,22 @@
             self[k]=v
 
     def __setitem__(self, key, value):
         self[key] = value
 
 
 class {name_camel}(ModelBase,CRUD):
-    _collection_name="{name_db}"
-    _base_model=_Base
+    collection_name="{name_db}"
+    document_model=_Base
 
     def __init__(self,request) -> None:
+        super().__init__()
         self.request=request
 
-    def get(self,police: bool = True) -> typing.List[_base_model]:
+    def get(self,police: bool = True) -> typing.List[document_model]:
         return self._get(police)
 
-    def first(self,police: bool = True) -> _base_model:
+    def first(self,police: bool = True) -> typing.Union[document_model,None]:
         return self._first(police)
 
     def boot_event(self, typ: str, old, new):
-        ActivityService().handle(typ, old, new, self.request, self._collection_name)
+        ActivityService().handle(typ, old, new, self.request, self.collection_name)
```

### Comparing `renus-1.1.0/renus/commands/app/route.temp` & `renus-1.1.1/renus/commands/app/route.temp`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/commands/app/run.py` & `renus-1.1.1/renus/commands/app/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/commands/backup/run.py` & `renus-1.1.1/renus/commands/backup/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/commands/copy/run.py` & `renus-1.1.1/renus/commands/copy/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/commands/default/run.py` & `renus-1.1.1/renus/commands/default/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/commands/help.py` & `renus-1.1.1/renus/commands/help.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/commands/install/build.py` & `renus-1.1.1/renus/commands/install/build.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/commands/install/run.py` & `renus-1.1.1/renus/commands/install/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/commands/install/service.py` & `renus-1.1.1/renus/commands/install/service.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/commands/permission/run.py` & `renus-1.1.1/renus/commands/permission/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/core/cache.py` & `renus-1.1.1/renus/core/cache.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/core/concurrency.py` & `renus-1.1.1/renus/core/concurrency.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/core/crypt.py` & `renus-1.1.1/renus/core/crypt.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/core/datastructures.py` & `renus-1.1.1/renus/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/core/exception.py` & `renus-1.1.1/renus/core/exception.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/core/formparsers.py` & `renus-1.1.1/renus/core/formparsers.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/core/injection.py` & `renus-1.1.1/renus/core/injection.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/core/log.py` & `renus-1.1.1/renus/core/log.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/core/model.py` & `renus-1.1.1/renus/core/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import os
 import typing
-
 from bson import ObjectId
 from pymongo import MongoClient
 from datetime import datetime
 from renus.core.config import Config
-from renus.util.helper import dictAttribute
 
 class ModelBase:
     _client = MongoClient(Config('database').get('host', '127.0.0.1'),
                           Config('database').get('port', 27017),
                           username=Config('database').get('username', None),
                           password=Config('database').get('password', None))
 
     _database_name = Config('database').get('name', 'renus')
-    _collection_name=None
+    collection_name=None
     metro = None
-    _public_folder='public'
+    public_folder='public'
     hidden_fields = []
-    fields = {}
-    _base_model=dictAttribute
+    document_model=dict
+    add_time_fields=True
     def __init__(self) -> None:
+        if hasattr(self, '_collection_name'):
+            raise RuntimeError('_collection_name has expired. Use collection_name')
+        if hasattr(self, '_public_folder'):
+            raise RuntimeError('_public_folder has expired. Use public_folder')
         self._steps = None
         self._where = None
         self._distinct = None
         self._limit = None
         self._skip = None
         self._sort = None
         self._select = None
@@ -34,24 +36,24 @@
         return iter(self.get())
 
     def set_database(self, name: str):
         self._database_name = name
         return self
 
     def set_collection(self, name: str):
-        self._collection_name = name
+        self.collection_name = name
         return self
 
     @property
     def db(self):
         return self._client[self._database_name]
 
     def collection(self, name: str = None):
         if name is None:
-            name = self._collection_name
+            name = self.collection_name
 
         return self.db[name]
 
     def reset(self):
         self._steps = None
         self._where = None
         self._distinct = None
@@ -174,15 +176,15 @@
                 self._steps.append({'$unwind': f'${to}'})
         return self
 
     def steps(self):
         self._steps = []
         return self
 
-    def _get(self, police: bool = True) -> typing.List[_base_model]:
+    def _get(self, police: bool = True) -> typing.List[document_model]:
         if self._steps is not None:
             return self.aggregate(self._steps)
 
         where, select = self._base_gate(police)
 
         find = self.collection().find(where, select)
 
@@ -193,89 +195,94 @@
         if self._limit is not None:
             find = find.limit(self._limit)
         if self._distinct is not None:
             return find.distinct(self._distinct)
 
         return self.__police(find) if police else list(find)
 
-    def get(self,police: bool = True) -> typing.List[_base_model]:
+    def get(self,police: bool = True) -> typing.List[document_model]:
         return self._get(police)
 
-    def _first(self, police: bool = True) -> typing.Union[_base_model,None]:
+    def _first(self, police: bool = True) -> typing.Union[document_model,None]:
         self.limit(1)
         res = self.get(police)
         self._limit = None
         if len(res) == 1:
             return res[0]
         return None
 
-    def first(self, police: bool = True) -> typing.Union[_base_model, None]:
+    def first(self, police: bool = True) -> typing.Union[document_model, None]:
         return self._first(police)
 
     def create(self, document: dict) -> dict:
-        if "updated_at" not in document:
+        if self.add_time_fields and "updated_at" not in document:
             document["updated_at"] = datetime.utcnow()
 
-        if "created_at" not in document:
+        if self.add_time_fields and "created_at" not in document:
             document["created_at"] = datetime.utcnow()
 
         id = self.collection().insert_one(document).inserted_id
         document['_id'] = id
         self.boot_event('create', {}, document)
         return document
 
     def create_many(self, documents: typing.List) -> typing.List[ObjectId]:
-        for document in documents:
-            if "updated_at" not in document:
-                document["updated_at"] = datetime.utcnow()
+        if self.add_time_fields:
+            for document in documents:
+                if "updated_at" not in document:
+                    document["updated_at"] = datetime.utcnow()
 
-            if "created_at" not in document:
-                document["created_at"] = datetime.utcnow()
+                if "created_at" not in document:
+                    document["created_at"] = datetime.utcnow()
 
         ids = self.collection().insert_many(documents).inserted_ids
         self.boot_event('create_many', {}, ids)
         return ids
 
     def update(self, new: dict, upsert=False, get_old=False) -> bool:
         where = self.__ud_gate('update')
-        new["updated_at"] = datetime.utcnow()
+        if self.add_time_fields:
+            new["updated_at"] = datetime.utcnow()
         d = {"$set": new}
-        if "created_at" not in new:
+        if self.add_time_fields and "created_at" not in new:
             d["$setOnInsert"] = {'created_at': datetime.utcnow()}
         old = self.collection().find_one_and_update(where, d, upsert=upsert)
         self.boot_event('update', old, new)
         return old if get_old else True
 
     def update_opt(self, new: dict, upsert=False, get_old=False) -> bool:
         where = self.__ud_gate('update')
         if '$set' not in new:
             new['$set'] = {}
         if '$setOnInsert' not in new:
             new['$setOnInsert'] = {}
-        new['$set']["updated_at"] = datetime.utcnow()
-        new['$setOnInsert']['created_at'] = datetime.utcnow()
+        if self.add_time_fields:
+            new['$set']["updated_at"] = datetime.utcnow()
+            new['$setOnInsert']['created_at'] = datetime.utcnow()
         old = self.collection().find_one_and_update(where, new, upsert=upsert)
         self.boot_event('update', old, {k[1:]:v for k,v in new.items()})
         return old if get_old else True
 
     def update_opt_many(self, new: dict, upsert=False, get_old=False) -> bool:
         where = self.__ud_gate('update')
         if '$set' not in new:
             new['$set'] = {}
         if '$setOnInsert' not in new:
             new['$setOnInsert'] = {}
-        new['$set']["updated_at"] = datetime.utcnow()
-        new['$setOnInsert']['created_at'] = datetime.utcnow()
+        if self.add_time_fields:
+            new['$set']["updated_at"] = datetime.utcnow()
+            new['$setOnInsert']['created_at'] = datetime.utcnow()
         old = self.collection().update_many(where, new, upsert=upsert).raw_result
         self.boot_event('update', old, {k[1:]:v for k,v in new.items()})
         return old if get_old else True
 
     def update_many(self, new: dict) -> bool:
         where = self.__ud_gate('update')
-        new["updated_at"] = datetime.utcnow()
+        if self.add_time_fields:
+            new["updated_at"] = datetime.utcnow()
         old = self.collection().update_many(where, {"$set": new}).raw_result
         self.boot_event('update_many', old, str(new))
         return True
 
     def delete(self, all: bool = False) -> bool:
         where = self.__ud_gate('delete')
         if all is False:
@@ -327,15 +334,15 @@
         return document
 
     def __cleaner(self, document: dict):
         for field in self.hidden_fields:
             if field in document and field not in self.visible_fields:
                 del document[field]
 
-        return self._base_model(self.cast(document))
+        return self.document_model(self.cast(document))
 
     def __police(self, documents: typing.Any):
         if documents is None:
             return None
         res = []
         if type(documents) is dict:
             return self.__cleaner(documents)
@@ -410,14 +417,14 @@
             elif type(link) is dict:
                 link = link.get('url').replace('storage/img/', '', 1)
                 link = link.replace('storage/', '', 1)
             else:
                 raise RuntimeError(f"type {link} must be string or dict but its {type(link)}")
 
             try:
-                os.remove(f'storage/{self._public_folder}/' + link)
+                os.remove(f'storage/{self.public_folder}/' + link)
             except:
                 pass
 
     @property
     def database_name(self):
         return self._database_name
```

### Comparing `renus-1.1.0/renus/core/request.py` & `renus-1.1.1/renus/core/request.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/core/response.py` & `renus-1.1.1/renus/core/response.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/core/routing.py` & `renus-1.1.1/renus/core/routing.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/core/schedule.py` & `renus-1.1.1/renus/core/schedule.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/core/serialize.py` & `renus-1.1.1/renus/core/serialize.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/core/status.py` & `renus-1.1.1/renus/core/status.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/core/validation/rules.py` & `renus-1.1.1/renus/core/validation/rules.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/core/validation/validate.py` & `renus-1.1.1/renus/core/validation/validate.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/core/websockets.py` & `renus-1.1.1/renus/core/websockets.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus/util/helper.py` & `renus-1.1.1/renus/util/helper.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.0/renus.egg-info/SOURCES.txt` & `renus-1.1.1/renus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

