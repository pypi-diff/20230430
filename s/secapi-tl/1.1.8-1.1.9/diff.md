# Comparing `tmp/secapi-tl-1.1.8.tar.gz` & `tmp/secapi-tl-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secapi-tl-1.1.8.tar", last modified: Sun Apr 23 19:25:10 2023, max compression
+gzip compressed data, was "secapi-tl-1.1.9.tar", last modified: Mon Apr 24 07:48:09 2023, max compression
```

## Comparing `secapi-tl-1.1.8.tar` & `secapi-tl-1.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-23 19:25:10.049290 secapi-tl-1.1.8/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1063 2022-10-14 12:06:38.000000 secapi-tl-1.1.8/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)     4873 2023-04-23 19:25:10.049290 secapi-tl-1.1.8/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     3434 2023-04-23 18:15:51.000000 secapi-tl-1.1.8/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)      391 2023-04-23 18:15:51.000000 secapi-tl-1.1.8/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-23 19:25:10.049290 secapi-tl-1.1.8/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-23 19:25:10.049290 secapi-tl-1.1.8/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-23 19:25:10.049290 secapi-tl-1.1.8/src/secapi_tl/
--rw-rw-r--   0 tom       (1000) tom       (1000)      307 2023-04-23 18:15:51.000000 secapi-tl-1.1.8/src/secapi_tl/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6136 2023-04-15 21:09:49.000000 secapi-tl-1.1.8/src/secapi_tl/filing.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4041 2023-04-23 18:15:51.000000 secapi-tl-1.1.8/src/secapi_tl/filing_query.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      977 2023-04-23 16:14:09.000000 secapi-tl-1.1.8/src/secapi_tl/key_mapper.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      824 2023-04-23 19:21:29.000000 secapi-tl-1.1.8/src/secapi_tl/request.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-23 19:25:10.049290 secapi-tl-1.1.8/src/secapi_tl.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)     4873 2023-04-23 19:25:10.000000 secapi-tl-1.1.8/src/secapi_tl.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      349 2023-04-23 19:25:10.000000 secapi-tl-1.1.8/src/secapi_tl.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-23 19:25:10.000000 secapi-tl-1.1.8/src/secapi_tl.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       42 2023-04-23 19:25:10.000000 secapi-tl-1.1.8/src/secapi_tl.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       10 2023-04-23 19:25:10.000000 secapi-tl-1.1.8/src/secapi_tl.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 07:48:09.373637 secapi-tl-1.1.9/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1063 2022-10-14 12:06:38.000000 secapi-tl-1.1.9/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4873 2023-04-24 07:48:09.373637 secapi-tl-1.1.9/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3434 2023-04-23 18:15:51.000000 secapi-tl-1.1.9/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)      391 2023-04-24 07:47:45.000000 secapi-tl-1.1.9/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-24 07:48:09.373637 secapi-tl-1.1.9/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 07:48:09.373637 secapi-tl-1.1.9/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 07:48:09.373637 secapi-tl-1.1.9/src/secapi_tl/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      307 2023-04-23 18:15:51.000000 secapi-tl-1.1.9/src/secapi_tl/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6136 2023-04-15 21:09:49.000000 secapi-tl-1.1.9/src/secapi_tl/filing.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4041 2023-04-23 18:15:51.000000 secapi-tl-1.1.9/src/secapi_tl/filing_query.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      977 2023-04-23 16:14:09.000000 secapi-tl-1.1.9/src/secapi_tl/key_mapper.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      916 2023-04-24 07:47:07.000000 secapi-tl-1.1.9/src/secapi_tl/request.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 07:48:09.373637 secapi-tl-1.1.9/src/secapi_tl.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4873 2023-04-24 07:48:09.000000 secapi-tl-1.1.9/src/secapi_tl.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      349 2023-04-24 07:48:09.000000 secapi-tl-1.1.9/src/secapi_tl.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-24 07:48:09.000000 secapi-tl-1.1.9/src/secapi_tl.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       42 2023-04-24 07:48:09.000000 secapi-tl-1.1.9/src/secapi_tl.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       10 2023-04-24 07:48:09.000000 secapi-tl-1.1.9/src/secapi_tl.egg-info/top_level.txt
```

### Comparing `secapi-tl-1.1.8/LICENSE` & `secapi-tl-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.8/PKG-INFO` & `secapi-tl-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secapi-tl
-Version: 1.1.8
+Version: 1.1.9
 License: MIT License
         
         Copyright (c) 2022 tlie03
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `secapi-tl-1.1.8/README.md` & `secapi-tl-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.8/src/secapi_tl/filing.py` & `secapi-tl-1.1.9/src/secapi_tl/filing.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.8/src/secapi_tl/filing_query.py` & `secapi-tl-1.1.9/src/secapi_tl/filing_query.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.8/src/secapi_tl/key_mapper.py` & `secapi-tl-1.1.9/src/secapi_tl/key_mapper.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.8/src/secapi_tl/request.py` & `secapi-tl-1.1.9/src/secapi_tl/request.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,13 +16,17 @@
 
 
 @sleep_and_retry
 @limits(calls=SEC_REQUEST_COUNT, period=SEC_PERIOD)
 def sec_request(url: str):
     header = {"User-Agent": choice(USER_AGENTS)}
     SEMAPHORE.acquire()
-    response = requests.get(url=url, headers=header)
-    SEMAPHORE.release()
+    try:
+        response = requests.get(url=url, headers=header)
+        SEMAPHORE.release()
+    except Exception as err:
+        SEMAPHORE.release()
+        raise err
 
     if response.status_code != 200:
         raise ConnectionError(f"invalid response status code {response.status_code}")
     return response
```

### Comparing `secapi-tl-1.1.8/src/secapi_tl.egg-info/PKG-INFO` & `secapi-tl-1.1.9/src/secapi_tl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secapi-tl
-Version: 1.1.8
+Version: 1.1.9
 License: MIT License
         
         Copyright (c) 2022 tlie03
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

