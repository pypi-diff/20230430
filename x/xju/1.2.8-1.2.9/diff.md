# Comparing `tmp/xju-1.2.8.tar.gz` & `tmp/xju-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xju-1.2.8.tar", last modified: Mon Apr  3 10:03:46 2023, max compression
+gzip compressed data, was "xju-1.2.9.tar", last modified: Sun Apr 30 10:52:37 2023, max compression
```

## Comparing `xju-1.2.8.tar` & `xju-1.2.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-04-03 10:03:46.093230 xju-1.2.8/
--rw-r--r--   0 xju       (1001) xju       (1001)     1064 2023-04-03 10:03:45.000000 xju-1.2.8/MIT-LICENCE
--rw-r--r--   0 xju       (1001) xju       (1001)     6028 2023-04-03 10:03:46.093230 xju-1.2.8/PKG-INFO
--rw-r--r--   0 xju       (1001) xju       (1001)     4492 2023-04-03 10:03:45.000000 xju-1.2.8/README.rst
--rw-r--r--   0 xju       (1001) xju       (1001)     1597 2023-04-03 10:03:45.000000 xju-1.2.8/pyproject.toml
--rw-r--r--   0 xju       (1001) xju       (1001)       38 2023-04-03 10:03:46.093230 xju-1.2.8/setup.cfg
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-04-03 10:03:46.085230 xju-1.2.8/src/
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-04-03 10:03:46.089230 xju-1.2.8/src/xju/
--rw-r--r--   0 xju       (1001) xju       (1001)     5803 2023-02-25 06:28:28.000000 xju-1.2.8/src/xju/assert_.py
--rw-r--r--   0 xju       (1001) xju       (1001)     5837 2023-03-18 10:37:15.000000 xju-1.2.8/src/xju/assert_.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-04-03 10:03:46.093230 xju-1.2.8/src/xju/cmc/
--rw-r--r--   0 xju       (1001) xju       (1001)     3356 2023-03-18 10:41:04.000000 xju-1.2.8/src/xju/cmc/AsyncServiceQueue.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     8726 2023-03-18 10:40:34.000000 xju-1.2.8/src/xju/cmc/Dict.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2295 2023-03-18 10:40:59.000000 xju-1.2.8/src/xju/cmc/ThreadMutexLockCondition.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    17022 2023-03-18 11:11:14.000000 xju-1.2.8/src/xju/cmc/__init__.py
--rw-r--r--   0 xju       (1001) xju       (1001)     2238 2023-03-18 10:40:23.000000 xju-1.2.8/src/xju/cmc/cmc.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    14656 2023-03-18 10:40:28.000000 xju-1.2.8/src/xju/cmc/cmclass.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-04-03 10:03:46.093230 xju-1.2.8/src/xju/cmc/io/
--rw-r--r--   0 xju       (1001) xju       (1001)     2279 2023-03-18 10:40:06.000000 xju-1.2.8/src/xju/cmc/io/FileLock.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1598 2023-03-18 10:39:38.000000 xju-1.2.8/src/xju/cmc/io/FileMode.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1801 2023-03-18 10:39:45.000000 xju-1.2.8/src/xju/cmc/io/FilePosition.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3935 2023-03-18 10:39:53.000000 xju-1.2.8/src/xju/cmc/io/FileReader.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     4407 2023-03-18 10:39:59.000000 xju-1.2.8/src/xju/cmc/io/FileWriter.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3806 2023-03-29 20:33:11.000000 xju-1.2.8/src/xju/cmc/io/Pipe.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     5008 2023-03-18 10:40:18.000000 xju-1.2.8/src/xju/cmc/io/UnixStreamSocket.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    18523 2023-03-11 11:23:08.000000 xju-1.2.8/src/xju/cmc/io/__init__.py
--rw-r--r--   0 xju       (1001) xju       (1001)    23724 2022-10-22 03:21:18.000000 xju-1.2.8/src/xju/cmc/perflog.py
--rw-r--r--   0 xju       (1001) xju       (1001)    16348 2023-03-18 10:40:54.000000 xju-1.2.8/src/xju/cmc/perflog.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2042 2023-03-11 11:25:32.000000 xju-1.2.8/src/xju/cmc/signal.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1460 2023-03-18 10:40:41.000000 xju-1.2.8/src/xju/cmc/signal.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    26119 2022-10-28 11:58:37.000000 xju-1.2.8/src/xju/cmc/tstore.py
--rw-r--r--   0 xju       (1001) xju       (1001)    12879 2023-03-18 10:40:48.000000 xju-1.2.8/src/xju/cmc/tstore.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2193 2022-10-22 04:11:35.000000 xju-1.2.8/src/xju/cmd.py
--rw-r--r--   0 xju       (1001) xju       (1001)     2132 2023-03-18 11:29:29.000000 xju-1.2.8/src/xju/cmd.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    20357 2023-03-29 10:24:05.000000 xju-1.2.8/src/xju/json_codec.py
--rwxr-xr-x   0 xju       (1001) xju       (1001)    26089 2023-03-29 10:50:09.000000 xju-1.2.8/src/xju/json_codec.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     8199 2023-03-11 10:40:25.000000 xju-1.2.8/src/xju/jsonschema.py
--rw-r--r--   0 xju       (1001) xju       (1001)     9298 2023-03-18 10:37:26.000000 xju-1.2.8/src/xju/jsonschema.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1278 2022-10-19 21:07:25.000000 xju-1.2.8/src/xju/misc.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1170 2023-03-18 10:38:39.000000 xju-1.2.8/src/xju/misc.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    21741 2023-02-09 11:29:02.000000 xju-1.2.8/src/xju/newtype.py
--rw-r--r--   0 xju       (1001) xju       (1001)    11849 2023-03-18 10:39:25.000000 xju-1.2.8/src/xju/newtype.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1340 2022-10-22 04:27:19.000000 xju-1.2.8/src/xju/patch.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1121 2023-03-18 10:38:49.000000 xju-1.2.8/src/xju/patch.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    18961 2023-03-11 11:12:57.000000 xju-1.2.8/src/xju/pq.py
--rw-r--r--   0 xju       (1001) xju       (1001)    11182 2023-03-18 10:39:02.000000 xju-1.2.8/src/xju/pq.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)        0 2023-04-03 10:03:45.000000 xju-1.2.8/src/xju/py.typed
--rw-r--r--   0 xju       (1001) xju       (1001)     1744 2022-10-19 21:07:30.000000 xju-1.2.8/src/xju/rfc2616.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1937 2023-03-18 10:39:11.000000 xju-1.2.8/src/xju/rfc2616.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3352 2023-03-10 23:13:51.000000 xju-1.2.8/src/xju/time.py
--rw-r--r--   0 xju       (1001) xju       (1001)     2402 2023-03-11 10:39:44.000000 xju-1.2.8/src/xju/time.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     7226 2023-01-22 04:53:39.000000 xju-1.2.8/src/xju/xn.py
--rw-r--r--   0 xju       (1001) xju       (1001)     5869 2023-03-18 10:41:39.000000 xju-1.2.8/src/xju/xn.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-04-03 10:03:46.089230 xju-1.2.8/src/xju.egg-info/
--rw-r--r--   0 xju       (1001) xju       (1001)     6028 2023-04-03 10:03:46.000000 xju-1.2.8/src/xju.egg-info/PKG-INFO
--rw-r--r--   0 xju       (1001) xju       (1001)     1215 2023-04-03 10:03:46.000000 xju-1.2.8/src/xju.egg-info/SOURCES.txt
--rw-r--r--   0 xju       (1001) xju       (1001)        1 2023-04-03 10:03:46.000000 xju-1.2.8/src/xju.egg-info/dependency_links.txt
--rw-r--r--   0 xju       (1001) xju       (1001)        4 2023-04-03 10:03:46.000000 xju-1.2.8/src/xju.egg-info/top_level.txt
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-04-30 10:52:37.663515 xju-1.2.9/
+-rw-r--r--   0 xju       (1001) xju       (1001)     1064 2023-04-30 10:52:36.000000 xju-1.2.9/MIT-LICENCE
+-rw-r--r--   0 xju       (1001) xju       (1001)     6560 2023-04-30 10:52:37.663515 xju-1.2.9/PKG-INFO
+-rw-r--r--   0 xju       (1001) xju       (1001)     5024 2023-04-30 10:52:36.000000 xju-1.2.9/README.rst
+-rw-r--r--   0 xju       (1001) xju       (1001)     1597 2023-04-30 10:52:36.000000 xju-1.2.9/pyproject.toml
+-rw-r--r--   0 xju       (1001) xju       (1001)       38 2023-04-30 10:52:37.663515 xju-1.2.9/setup.cfg
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-04-30 10:52:37.659515 xju-1.2.9/src/
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-04-30 10:52:37.659515 xju-1.2.9/src/xju/
+-rw-r--r--   0 xju       (1001) xju       (1001)     5803 2023-02-25 06:28:28.000000 xju-1.2.9/src/xju/assert_.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     5837 2023-03-18 10:37:15.000000 xju-1.2.9/src/xju/assert_.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-04-30 10:52:37.663515 xju-1.2.9/src/xju/cmc/
+-rw-r--r--   0 xju       (1001) xju       (1001)     3356 2023-03-18 10:41:04.000000 xju-1.2.9/src/xju/cmc/AsyncServiceQueue.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     8726 2023-03-18 10:40:34.000000 xju-1.2.9/src/xju/cmc/Dict.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2295 2023-03-18 10:40:59.000000 xju-1.2.9/src/xju/cmc/ThreadMutexLockCondition.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    17022 2023-03-18 11:11:14.000000 xju-1.2.9/src/xju/cmc/__init__.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     2238 2023-03-18 10:40:23.000000 xju-1.2.9/src/xju/cmc/cmc.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    14656 2023-03-18 10:40:28.000000 xju-1.2.9/src/xju/cmc/cmclass.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-04-30 10:52:37.663515 xju-1.2.9/src/xju/cmc/io/
+-rw-r--r--   0 xju       (1001) xju       (1001)     2279 2023-03-18 10:40:06.000000 xju-1.2.9/src/xju/cmc/io/FileLock.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1598 2023-03-18 10:39:38.000000 xju-1.2.9/src/xju/cmc/io/FileMode.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1801 2023-03-18 10:39:45.000000 xju-1.2.9/src/xju/cmc/io/FilePosition.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3935 2023-03-18 10:39:53.000000 xju-1.2.9/src/xju/cmc/io/FileReader.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     4407 2023-03-18 10:39:59.000000 xju-1.2.9/src/xju/cmc/io/FileWriter.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3806 2023-03-29 20:33:11.000000 xju-1.2.9/src/xju/cmc/io/Pipe.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     5008 2023-03-18 10:40:18.000000 xju-1.2.9/src/xju/cmc/io/UnixStreamSocket.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    18523 2023-03-11 11:23:08.000000 xju-1.2.9/src/xju/cmc/io/__init__.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    23724 2022-10-22 03:21:18.000000 xju-1.2.9/src/xju/cmc/perflog.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    16348 2023-03-18 10:40:54.000000 xju-1.2.9/src/xju/cmc/perflog.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2042 2023-03-11 11:25:32.000000 xju-1.2.9/src/xju/cmc/signal.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1460 2023-03-18 10:40:41.000000 xju-1.2.9/src/xju/cmc/signal.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    26119 2022-10-28 11:58:37.000000 xju-1.2.9/src/xju/cmc/tstore.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    12879 2023-03-18 10:40:48.000000 xju-1.2.9/src/xju/cmc/tstore.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2193 2022-10-22 04:11:35.000000 xju-1.2.9/src/xju/cmd.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     2132 2023-03-18 11:29:29.000000 xju-1.2.9/src/xju/cmd.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    49437 2023-04-30 10:42:18.000000 xju-1.2.9/src/xju/json_codec.py
+-rwxr-xr-x   0 xju       (1001) xju       (1001)    28466 2023-04-30 10:35:38.000000 xju-1.2.9/src/xju/json_codec.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     8199 2023-03-11 10:40:25.000000 xju-1.2.9/src/xju/jsonschema.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     9298 2023-03-18 10:37:26.000000 xju-1.2.9/src/xju/jsonschema.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1278 2022-10-19 21:07:25.000000 xju-1.2.9/src/xju/misc.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1170 2023-03-18 10:38:39.000000 xju-1.2.9/src/xju/misc.py.test
+-r--r--r--   0 xju       (1001) xju       (1001)    21254 2023-04-16 02:25:56.000000 xju-1.2.9/src/xju/newtype.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    11849 2023-03-18 10:39:25.000000 xju-1.2.9/src/xju/newtype.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1340 2022-10-22 04:27:19.000000 xju-1.2.9/src/xju/patch.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1121 2023-03-18 10:38:49.000000 xju-1.2.9/src/xju/patch.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    18970 2023-04-30 10:35:38.000000 xju-1.2.9/src/xju/pq.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    11182 2023-03-18 10:39:02.000000 xju-1.2.9/src/xju/pq.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)        0 2023-04-30 10:52:36.000000 xju-1.2.9/src/xju/py.typed
+-rw-r--r--   0 xju       (1001) xju       (1001)     1744 2022-10-19 21:07:30.000000 xju-1.2.9/src/xju/rfc2616.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1937 2023-03-18 10:39:11.000000 xju-1.2.9/src/xju/rfc2616.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3280 2023-04-30 10:35:38.000000 xju-1.2.9/src/xju/time.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     2402 2023-03-11 10:39:44.000000 xju-1.2.9/src/xju/time.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     7226 2023-01-22 04:53:39.000000 xju-1.2.9/src/xju/xn.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     5869 2023-03-18 10:41:39.000000 xju-1.2.9/src/xju/xn.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-04-30 10:52:37.663515 xju-1.2.9/src/xju.egg-info/
+-rw-r--r--   0 xju       (1001) xju       (1001)     6560 2023-04-30 10:52:37.000000 xju-1.2.9/src/xju.egg-info/PKG-INFO
+-rw-r--r--   0 xju       (1001) xju       (1001)     1215 2023-04-30 10:52:37.000000 xju-1.2.9/src/xju.egg-info/SOURCES.txt
+-rw-r--r--   0 xju       (1001) xju       (1001)        1 2023-04-30 10:52:37.000000 xju-1.2.9/src/xju.egg-info/dependency_links.txt
+-rw-r--r--   0 xju       (1001) xju       (1001)        4 2023-04-30 10:52:37.000000 xju-1.2.9/src/xju.egg-info/top_level.txt
```

### Comparing `xju-1.2.8/MIT-LICENCE` & `xju-1.2.9/MIT-LICENCE`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/PKG-INFO` & `xju-1.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xju
-Version: 1.2.8
+Version: 1.2.9
 Summary: xju library
 Author: Trevor Taylor
 License: Copyright © 2022 Trevor Taylor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -25,14 +25,16 @@
 Various modules implemented to some broad principles:
 
 * fine-grained static typing
 * pure context management
 * useful functionality that is hard to use incorrectly
 * 100% test coverage
 
+(see the bottom of this readme for release history)
+
 `xju.newtype <xju/newtype.py>`_ - static and dynamic distinct int, float and str types
 
 * unlike typing.NewType the new types are compatible with isinstance, so you
   can actually use them to do real stuff, like implement overloaded methods
 
 * see `xju/newtype.py.test <xju/newtype.py.test>`_ for sample code
 
@@ -130,14 +132,16 @@
 
 * designed to fit well with type checking
 
 * built in support for xju.newtype described above
 
 * generates json schema equivalent schemas for types
 
+* generates typescript code (types, type-guards and dynamic casts) equivalents
+
 * see `xju/json_codec.py.test <xju/json_codec.py.test>`_ for full sample code
 
 
 `xju.jsonschema <xju/jsonschema.py>`_
 
 * represents JSON schemas as straight-foward, easy-to-read python data structures, because life's too short for jsonschema.org
 
@@ -160,7 +164,16 @@
 
 `xju.xn <xju/xn.py>`_
 
 * Exception wrapping to provide human readable context gathering
 
 * see `xju/xn.py.test <xju/xn.py.test>`_ for sample code
 
+Release History
+
+- 1.2.9 xju.json_codec generates typescript equivalents
+- 1.2.9 xju.json_codec adds codec() convenience method
+- 1.2.9 xju.json_codec uses kw_args to construct classes
+
+- 1.2.8 xju.json_codec supports string type-hints (for foward definitions)
+- 1.2.8 xju.json_codec adds typing.Self support (for recursive types)
+- 1.2.8 xju.json_codec requires python 3.11, tested with mypy 1.1.1
```

### Comparing `xju-1.2.8/README.rst` & `xju-1.2.9/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 Various modules implemented to some broad principles:
 
 * fine-grained static typing
 * pure context management
 * useful functionality that is hard to use incorrectly
 * 100% test coverage
 
+(see the bottom of this readme for release history)
+
 `xju.newtype <xju/newtype.py>`_ - static and dynamic distinct int, float and str types
 
 * unlike typing.NewType the new types are compatible with isinstance, so you
   can actually use them to do real stuff, like implement overloaded methods
 
 * see `xju/newtype.py.test <xju/newtype.py.test>`_ for sample code
 
@@ -109,14 +111,16 @@
 
 * designed to fit well with type checking
 
 * built in support for xju.newtype described above
 
 * generates json schema equivalent schemas for types
 
+* generates typescript code (types, type-guards and dynamic casts) equivalents
+
 * see `xju/json_codec.py.test <xju/json_codec.py.test>`_ for full sample code
 
 
 `xju.jsonschema <xju/jsonschema.py>`_
 
 * represents JSON schemas as straight-foward, easy-to-read python data structures, because life's too short for jsonschema.org
 
@@ -139,7 +143,16 @@
 
 `xju.xn <xju/xn.py>`_
 
 * Exception wrapping to provide human readable context gathering
 
 * see `xju/xn.py.test <xju/xn.py.test>`_ for sample code
 
+Release History
+
+- 1.2.9 xju.json_codec generates typescript equivalents
+- 1.2.9 xju.json_codec adds codec() convenience method
+- 1.2.9 xju.json_codec uses kw_args to construct classes
+
+- 1.2.8 xju.json_codec supports string type-hints (for foward definitions)
+- 1.2.8 xju.json_codec adds typing.Self support (for recursive types)
+- 1.2.8 xju.json_codec requires python 3.11, tested with mypy 1.1.1
```

### Comparing `xju-1.2.8/pyproject.toml` & `xju-1.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "xju"
-version = "1.2.8"
+version = "1.2.9"
 description = "xju library"
 readme = "README.rst"
 authors = [{ name = "Trevor Taylor"}]
 license = { file = "MIT-LICENCE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `xju-1.2.8/src/xju/assert_.py` & `xju-1.2.9/src/xju/assert_.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/assert_.py.test` & `xju-1.2.9/src/xju/assert_.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/AsyncServiceQueue.py.test` & `xju-1.2.9/src/xju/cmc/AsyncServiceQueue.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/Dict.py.test` & `xju-1.2.9/src/xju/cmc/Dict.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/ThreadMutexLockCondition.py.test` & `xju-1.2.9/src/xju/cmc/ThreadMutexLockCondition.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/__init__.py` & `xju-1.2.9/src/xju/cmc/__init__.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/cmc.py.test` & `xju-1.2.9/src/xju/cmc/cmc.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/cmclass.py.test` & `xju-1.2.9/src/xju/cmc/cmclass.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/io/FileLock.py.test` & `xju-1.2.9/src/xju/cmc/io/FileLock.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/io/FileMode.py.test` & `xju-1.2.9/src/xju/cmc/io/FileMode.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/io/FilePosition.py.test` & `xju-1.2.9/src/xju/cmc/io/FilePosition.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/io/FileReader.py.test` & `xju-1.2.9/src/xju/cmc/io/FileReader.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/io/FileWriter.py.test` & `xju-1.2.9/src/xju/cmc/io/FileWriter.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/io/Pipe.py.test` & `xju-1.2.9/src/xju/cmc/io/Pipe.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/io/UnixStreamSocket.py.test` & `xju-1.2.9/src/xju/cmc/io/UnixStreamSocket.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/io/__init__.py` & `xju-1.2.9/src/xju/cmc/io/__init__.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/perflog.py` & `xju-1.2.9/src/xju/cmc/perflog.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/perflog.py.test` & `xju-1.2.9/src/xju/cmc/perflog.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/signal.py` & `xju-1.2.9/src/xju/cmc/signal.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/signal.py.test` & `xju-1.2.9/src/xju/cmc/signal.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/tstore.py` & `xju-1.2.9/src/xju/cmc/tstore.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmc/tstore.py.test` & `xju-1.2.9/src/xju/cmc/tstore.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmd.py` & `xju-1.2.9/src/xju/cmd.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/cmd.py.test` & `xju-1.2.9/src/xju/cmd.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/json_codec.py` & `xju-1.2.9/src/xju/pq.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,525 +1,565 @@
 # coding: utf-8
 #
-# Copyright (c) 2023 Trevor Taylor
+# Copyright (c) 2018 Trevor Taylor
 # 
 # Permission to use, copy, modify, and/or distribute this software for
 # any purpose with or without fee is hereby granted, provided that all
 # copyright notices and this permission notice appear in all copies.
 # 
 # THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 #
-# json schema represented as a python type var, e.g.:
+# jquery-like python library
 #
-# @dataclasses.dataclass
-# class Address:
-#  number: str|int
-#  street: str
+# parse a HTML text into a tree, with search, manipulation
+# and re-output as HTML text
 #
-# Codec[dict[str,int|Address]].decode({'fred':3, 'jock':{'number':32, 'street': 'asler'}})
+# parse() and parseFile() are the primary interface.
 #
-# For examples see json_codec.py.test
+# REVISIT: need better diags, eg:
+#  track selectors used to find/filter nodes and report them
+#  on failure eg replace/html
 #
+from __future__ import annotations
+from html.parser import HTMLParser
+from html.entities import entitydefs as htmlentitydefs
+from html.entities import name2codepoint as entities
+from html.entities import codepoint2name as reverseentities
+import sys
+import traceback
+import string
+from xju.xn import in_context,in_function_context
+
+class Pos:
+    def __init__(self, file, line, col):
+        self.file=file
+        self.line=line
+        self.col=col
+        return
+    def __str__(self):
+        return '%(file)s:%(line)s:%(col)s' % self.__dict__
+    pass
+
+class ParseFailed(Exception):
+    def __init__(self, cause, pos):
+        self.cause=cause
+        self.pos=pos
+        Exception.__init__(self,self.__str__())
+        return
+    def __str__(self):
+        return 'failed to parse html at %(pos)s because\n%(cause)s'%self.__dict__
+    pass
 
-from xju.xn import Xn,in_context,in_function_context,readable_repr
-from typing import TypeVar, Generic, Type, cast, Any, Protocol, Self, Callable
-from typing import _LiteralGenericAlias  # type: ignore  # mypy 1.1.1
-from typing import _UnionGenericAlias  # type: ignore  # mypy 1.1.1
-from types import GenericAlias, UnionType, NoneType
-import xju.newtype
-
-T=TypeVar('T')
-
-JsonType = None|bool|dict|list|float|str
-
-
-class Codec(Generic[T]):
-    t:Type[T]
-    def __init__(self, t: Type[T]):
-        'initialse json decoder for type %(t)r'
-        self.t=t
-        self.codec:CodecProto=_explodeSchema(self.t)
-        pass
 
+def encodeEntity(c):
+    x=reverseentities.get(ord(c),None)
+    if x is None: return c
+    return u'&%(x)s;'%vars()
+
+def encodeEntities(s:str)->str:
+    if s is None: return u''
+    x=u''.join([encodeEntity(_) for _ in s])
+    return x
+
+class Node:
+    def __init__(self, parent=None):
+        self.parent=parent
+        if parent:
+            parent.children.append(self)
+            pass
+        pass
+    def predecessor(self):
+        if self.parent:
+            i=self.parent.children.index(self)
+            if i>0:
+                return [self.parent.children[i-1]]
+            pass
+        return []
+    def successor(self):
+        if self.parent:
+            i=self.parent.children.index(self)+1
+            if i<len(self.parent.children):
+                return [self.parent.children[i]]
+            pass
+        return []
+    
+class Root(Node):
+    def __init__(self):
+        Node.__init__(self)
+        self.children:list[Node]=[]
+    def indexOf(self, child):
+        return [ _[0] for _ in zip(range(0,len(self.children)),
+                                   self.children) if _[1]==child][0]
+    def remove(self, node):
+        i=self.indexOf(node)
+        self.children=self.children[0:i]+self.children[i+1:]
+        node.parent=None
+        return self
+    pass
+
+endOptional=frozenset([
+        'body',
+        'colgroup',
+        'dd',
+        'dt',
+        'head',
+        'html',
+        'li',
+        'option',
+        'p',
+        'tbody',
+        'td',
+        'tfoot',
+        'th',
+        'thead',
+        'tr'])
+
+emptyTags=frozenset([
+        'area',
+        'base',
+        'basefont',
+        'br',
+        'col',
+        'frame',
+        'hr',
+        'img',
+        'input',
+        'isindex',
+        'link',
+        'meta',
+        'param'])
+
+class Tag(Node):
+    def __init__(self, tagName, attrs, parent, pos):
+        Node.__init__(self, parent)
+        self.pos=pos
+        self.tagName=tagName
+        self.attrs=dict(attrs)
+        self.children:list[Node]=[]
+        self.end=''
+        self.classes=set(self.attrs.get('class','').split())
+        return
     def __repr__(self):
-        return f'{self.t!r} json codec'
-
-    def encode(self,x:T) -> JsonType:
-        'encode {self.t} {x} to json'
-        return self.codec.encode(x,None)
-
-    def decode(self,x:JsonType) -> T:
-        'decode {x} to a {self.t}'
-        try:
-            return cast(T, self.codec.decode(x,None))
-        except Exception:
-            raise in_function_context(Codec.decode,vars()) from None
+        return '%(tagName)s at %(pos)s' % self.__dict__
+    def __str__(self):
+        encodedAttrs=['%s="%s"' % (_[0],encodeEntities(_[1])) for 
+                      _ in self.attrs.items()]
+        encodedAttrs.sort()
+        start=' '.join([self.tagName]+encodedAttrs)
+        if self.tagName in ['script','style']:
+            content=self.text()
+        else:
+            content=''.join([str(_) for _ in self.children])
+            pass
+        end=self.end
+        return '''<%(start)s>%(content)s%(end)s'''%vars()
+    def hasClass(self,c):
+        return c in self.classes
+    def addClass(self,c):
+        self.classes.add(c)
+        self.attrs['class']=' '.join(self.classes)
+        return self
+    def removeClass(self,c):
+        if c in self.classes:
+            self.classes.remove(c)
+            pass
+        self.attrs['class']=' '.join(self.classes)
+        if len(self.classes)==0:
+            del self.attrs['class']
+        return self
+    def attr(self, a, val=None):
+        if not val is None:
+            self.attrs[a]=str(val)
+        return self.attrs.get(a,'')
+    def removeAttr(self, a):
+        if a in self.attrs: del self.attrs[a]
+        return
+    def attrEquals(self, a, val):
+        return self.attrs.get(a,None)==val
+    def hasAttr(self, a):
+        return a in self.attrs
+    def indexOf(self, child):
+        return [ _[0] for _ in zip(range(0,len(self.children)),
+                                   self.children) if _[1]==child][0]
+    def remove(self, node):
+        i=self.indexOf(node)
+        self.children=self.children[0:i]+self.children[i+1:]
+        node.parent=None
+        return self
+    def replace(self, node, newNode):
+        if newNode.parent:
+            newNode.parent.remove(newNode)
+        self.children[self.indexOf(node)]=newNode
+        newNode.parent=self
+        return self
+    def clone(self, newParent):
+        result=Tag(self.tagName, self.attrs.items(), newParent, self.pos)
+        result.end=self.end
+        result.classes=set(self.classes)
+        for c in self.children:
+            assert isinstance(c,Tag) or \
+                isinstance(c,Data) or \
+                isinstance(c,Comment) or \
+                isinstance(c,Decl) or \
+                isinstance(c,PI)
+            c.clone(result)
+        return result
+    def text(self):
+        if self.tagName=='br':
+            return u'\n'
+        if self.tagName=='p':
+            return u''.join([_.text() for _ in self.children])+u'\n'
+        if self.tagName=='li':
+            return u''.join([_.text() for _ in self.children])+u'\n'
+        return u''.join([_.text() for _ in self.children])
+    pass
+
+class Data(Node):
+    '''CData, including <script> and <style> content'''
+    def __init__(self, data, parent, pos):
+        Node.__init__(self, parent)
+        self.pos=pos
+        self.data=data
         pass
-
-    def get_json_schema(self) -> dict:
-        definitions: dict[str,dict] = {}
-        result = self.codec.get_json_schema(definitions, None)
-        result.update({
-            "$id": "https://example.com/address.schema.json",
-            "$schema": "https://json-schema.org/draft/2020-12/schema"})
-        result.update({
-            'definitions':definitions
-        })
+    def __str__(self):
+        return encodeEntities(self.data)
+    def __repr__(self):
+        return 'data at %(pos)s, %(data)r' % self.__dict__
+    def clone(self, newParent):
+        result=Data(self.data, newParent, self.pos)
         return result
+    def text(self):
+        return self.data
     pass
 
-class CodecProto(Protocol):
-    def encode(self,x:Any,back_ref:None|Callable[[Any],JsonType])->JsonType:
-        pass
-    def decode(self,x:JsonType,back_ref:None|Callable[[JsonType],Any])->Any:
-        pass
-    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
-        pass
+class Comment(Node):
+    '''Comment'''
+    def __init__(self, comment, parent, pos):
+        Node.__init__(self, parent)
+        self.pos=pos
+        self.comment=comment
+    def __str__(self):
+        return '<!--%(comment)s-->' % self.__dict__
+    def __repr__(self):
+        return 'comment at %(pos)s' % self.__dict__
+    def clone(self, newParent):
+        result=Comment(self.comment, newParent, self.pos)
+        return result
+    def text(self):
+        return u''
     pass
 
-Atom=TypeVar('Atom',int,str,bool,float,None)
-
-NewInt=TypeVar('NewInt',bound=xju.newtype.Int)
-NewFloat=TypeVar('NewFloat',bound=xju.newtype.Float)
-NewStr=TypeVar('NewStr',bound=xju.newtype.Str)
-
-class NoopCodec(Generic[Atom]):
-    t:Type[Atom]
-    def __init__(self, t:Type[Atom]):
-        self.t=t
-    def encode(self, x:Atom, _:None|Callable[[Any],JsonType])->Atom:
-        if type(x) is not self.t and not (
-                self.t is float and type(x) is int):
-            raise Exception(f'{x!r} is not a {self.t}')
-        return x
-    def decode(self, x:Atom,_:None|Callable[[JsonType],Any])->Atom:
-        if type(x) is not self.t and not (
-                self.t is float and type(x) is int):
-            t=type(x)
-            raise Exception(f'{x!r} (of type {t}) is not a {self.t}')
-        return x
-    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
-        st: str
-        if self.t is int: st='integer'
-        if self.t is str: st='string'
-        if self.t is float: st='number'
-        if self.t is bool: st='boolean'
-        if self.t is None: st='null'
-        return { 'type': st }
-    pass
-
-class NoneCodec:
-    def encode(self, x:None,_:None|Callable[[Any],JsonType])->None:
-        if x is not None:
-            raise Exception(f'{x!r} is not None')
-        return x
-    def decode(self, x:None,_:None|Callable[[JsonType],Any])->None:
-        if x is not None:
-            raise Exception(f'{x!r} is not None')
-        return x
-    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
-        return { 'type': 'null' }
-    pass
-
-class ListCodec:
-    def __init__(self, value_codec:CodecProto):
-        self.value_codec=value_codec
-        pass
-    def encode(self,x,back_ref:None|Callable[[Any],JsonType]):
-        if type(x) is not list:
-            raise Exception(f'{x!r} is not a list')
-        return [self.value_codec.encode(_,back_ref) for _ in x]
-    def decode(self,x,back_ref:None|Callable[[JsonType],Any]):
-        if type(x) is not list:
-            raise Exception(f'{x!r} is not a list')
-        return [self.value_codec.decode(_,back_ref) for _ in x]
-    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
-        return {
-            "type": "array",
-            "items": self.value_codec.get_json_schema(definitions, self_ref)
-        }
+class Decl(Node):
+    '''Decl'''
+    def __init__(self, decl, parent, pos):
+        Node.__init__(self, parent)
+        self.pos=pos
+        self.decl=decl
+    def __str__(self):
+        return '<!%(decl)s>' % self.__dict__
+    def __repr__(self):
+        return 'decl at %(pos)s' % self.__dict__
+    def clone(self, newParent):
+        result=Decl(self.decl, newParent, self.pos)
+        return result
+    def text(self):
+        return u''
     pass
 
-class AnyListCodec:
-    def __init__(self):
-        self.value_codec=AnyJsonCodec()
-        pass
-    def encode(self,x,back_ref:None|Callable[[Any],JsonType]):
-        if type(x) is not list:
-            raise Exception(f'{x!r} is not a list')
-        return [self.value_codec.encode(_,back_ref) for _ in x]
-    def decode(self,x,back_ref:None|Callable[[JsonType],Any]):
-        if type(x) is not list:
-            raise Exception(f'{x!r} is not a list')
-        return [self.value_codec.decode(_,back_ref) for _ in x]
-    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
-        return {
-            "type": "array"
-        }
-    pass
-
-class TupleCodec:
-    def __init__(self,value_codecs):
-        self.value_codecs=value_codecs
-        self.number_of_codecs=len(value_codecs)
-        pass
-    def encode(self,x,back_ref:None|Callable[[Any],JsonType]) -> list:
-        'encode tuple {x} as a {self.number_of_codecs}-element list'
-        try:
-            if type(x) is not tuple:
-                raise Exception(f'{x!r} is not a tuple')
-            if len(x) != self.number_of_codecs:
-                l=len(x)
-                raise Exception(f'{x} does not have {self.number_of_codecs} items (it has {l} items)')
-            return [c.encode(v,back_ref) for c,v in zip(self.value_codecs,x)]
-        except Exception:
-            raise in_function_context(TupleCodec.encode,vars()) from None
-        pass
-    def decode(self,x,back_ref:None|Callable[[JsonType],Any]) -> tuple:
-        try:
-            if type(x) is not list:
-                raise Exception(f'{x!r} is not a list')
-            if len(x) != self.number_of_codecs:
-                l=len(x)
-                raise Exception(f'{x} does not have {self.number_of_codecs} items (it has {l} items)')
-            result=[c.decode(v,back_ref) for c,v in zip(self.value_codecs,x)]
-            return tuple(result)
-        except Exception:
-            raise in_function_context(TupleCodec.decode,vars()) from None
-        pass
-    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
-        return {
-            "type": "array",
-            "prefixItems": [
-                codec.get_json_schema(definitions, self_ref) for codec in self.value_codecs
-            ]
-        }
+class PI(Node):
+    '''Processing Instruction'''
+    def __init__(self, pi, parent, pos):
+        Node.__init__(self, parent)
+        self.pos=pos
+        self.pi=pi
+    def __str__(self):
+        return '<?%(pi)s>' % self.__dict__
+    def __repr__(self):
+        return 'processing instruction at %(pos)s' % self.__dict__
+    def clone(self, newParent):
+        result=PI(self.pi, newParent, self.pos)
+        return result
+    def text(self):
+        return u''
     pass
 
-class UnionCodec:
-    def __init__(self,allowed_types):
-        self.allowed_types=allowed_types
-        self.value_codecs={t:_explodeSchema(t) for t in allowed_types}
-        pass
-    def encode(self,x,back_ref:None|Callable[[Any],JsonType]) -> JsonType:
-        'encode {x!r} as one of {self.allowed_types}'
-        try:
-            exceptions=[]
-            for t, c in self.value_codecs.items():
-                try:
-                    return c.encode(x,back_ref)
-                except Exception as e:
-                    exceptions.append( (t, e) )
+class Parser(HTMLParser):
+    def __init__(self, fileName):
+        HTMLParser.__init__(self)
+        self.fileName=fileName
+        self.root=Root()
+        self.current:Root|Tag=self.root
+        return
+    def pos(self):
+        return Pos(self.fileName, *self.getpos())
+    def handle_starttag(self, tag, attrs):
+        if tag in emptyTags:
+            Tag(tag, attrs, self.current, self.pos())
+        else:
+            #end-optional tag ends current tag of same name, eg
+            #<li>x
+            #<li>y
+            if isinstance(self.current, Tag) and \
+                    tag in endOptional and \
+                    self.current.tagName == tag:
+                self.current=self.current.parent
+            self.current=Tag(tag, attrs, self.current, self.pos())
+        return
+    def handle_endtag(self, tag):
+        current=self.current
+        while not isinstance(current,Root) and current.tagName != tag:
+            current=current.parent
+            pass
+        if not isinstance(current,Root):
+            self.current=current
+            self.current.end=u'</%(tag)s>'%vars()
+            self.current=self.current.parent
+        return
+    def handle_data(self,data):
+        Data(data, self.current, self.pos())
+        return
+    def handle_comment(self,comment):
+        Comment(comment, self.current, self.pos())
+        return
+    def handle_decl(self,decl):
+        Decl(decl,self.current, self.pos())
+        return
+    def handle_pi(self,pi):
+        PI(pi,self.current, self.pos())
+        return
+
+def filter(node, predicate):
+    '''return [node if matches predicate] + all children that match'''
+    result=[_ for _ in [node] if predicate(_)]
+    if isinstance(node,Tag):
+        for c in node.children:
+            result.extend(filter(c, predicate))
+    return result
+        
+class Selection:
+    nodeList:list[Node]
+    def __init__(self, nodeList:Selection|Node|list[Node]):
+        if isinstance(nodeList,Selection):
+            self.nodeList=nodeList.nodeList
+        elif isinstance(nodeList,Node):
+            self.nodeList=[nodeList,]
+        else:
+            self.nodeList=nodeList[:]
+            pass
+        return
+    def find(self, predicate):
+        '''find all children of our nodes that match predicate'''
+        result=[]
+        for _ in self.nodeList:
+            result.extend(filter(_,predicate))
+        return Selection(result)
+    def filter(self, predicate):
+        '''nodes of ours that match predicate'''
+        return Selection([_ for _ in self.nodeList if predicate(_)])
+    def unless(self, predicate):
+        '''nodes of ours that don't match predicate'''
+        return Selection([_ for _ in self.nodeList if not predicate(_)])
+    def html(self, nodes):
+        '''replace our first node's children with the specified list of nodes/html string'''
+        if type(nodes)==str:
+            nodes=parse(nodes)
+            pass
+        if isinstance(nodes, Selection):
+            nodes=nodes.nodeList
+            pass
+        for n in nodes:
+            if n.parent: n.parent.remove(n)
+        for n in self.nodeList[0:1]:
+            n.children=nodes
+            for c in n.children:
+                c.parent=n
+        return self
+    def text(self, s=None):
+        '''replace our first node's children with the specified text string'''
+        '''or return concatenation of text content of children'''
+        if s is None:
+            return u''.join([_.text() for _ in self.nodeList])
+        ss=parse(encodeEntities(str(s)))
+        for n in self.nodeList:
+            Selection([n]).html(ss)
+        return self
+    def replace(self, nodes):
+        '''replace first of specified nodes with first of our nodes'''
+        if isinstance(nodes, Selection):
+            nodes=nodes.nodeList
+        nodes[0].parent.replace(nodes[0],self.nodeList[0])
+        return self
+    def appendTo(self, nodes):
+        '''append our nodes to children of first of specified nodes'''
+        if isinstance(nodes, Selection):
+            nodes=nodes.nodeList
+        for n in self.nodeList:
+            n.parent=nodes[0]
+            nodes[0].children.append(n)
+        return self
+    def addAfter(self, nodes):
+        '''add our nodes after first of specified nodes'''
+        if isinstance(nodes, Selection):
+            nodes=nodes.nodeList
+        parent=nodes[0].parent
+        index=parent.indexOf(nodes[0])
+        for n in self.nodeList:
+            n.parent=parent
+        parent.children[index+1:index+1]=self.nodeList
+        return self
+    def addBefore(self, nodes):
+        '''add our nodes before first of specified nodes'''
+        if isinstance(nodes, Selection):
+            nodes=nodes.nodeList
+        parent=nodes[0].parent
+        index=parent.indexOf(nodes[0])
+        for n in self.nodeList:
+            n.parent=parent
+        parent.children[index:index]=self.nodeList
+        return self
+    def detach(self):
+        '''remove each of our nodes from its parent'''
+        for n in self.nodeList:
+            if n.parent:
+                n.parent.remove(n)
+        return self
+    def remove(self):
+        return self.detach()
+    def empty(self):
+        '''remove all children from each of our nodes'''
+        for n in self.nodeList:
+            if isinstance(n,Tag):
+                for c in n.children:
+                    c.parent=None
                     pass
+                n.children=[]
                 pass
-            raise Exception(' and '.join([f'failed to encode as {t} because {e}' for t,e in exceptions]))
-                
-        except Exception:
-            raise in_function_context(UnionCodec.encode,vars()) from None
-        pass
-    def decode(self,x,back_ref:None|Callable[[JsonType],Any]) -> tuple:
-        try:
-            exceptions=[]
-            for t, c in self.value_codecs.items():
-                try:
-                    return c.decode(x,back_ref)
-                except Exception as e:
-                    exceptions.append( (t, e) )
-                    pass
+            pass
+        return self
+    def first(self):
+        '''return Selection containing first of our nodes'''
+        return Selection(self.nodeList[0:1])
+    def last(self):
+        '''return Selection containing first of our nodes'''
+        return Selection(self.nodeList[-1:])
+    def children(self):
+        '''return Selection containing children of our nodes'''
+        nodeList:list[Node]=[]
+        return Selection(sum([_.children for _ in self.nodeList],nodeList))
+    def predecessors(self):
+        '''return Selection containing predecessor of each of our nodes'''
+        nodeList:list[Node]=[]
+        return Selection(sum([_.predecessor() for _ in self.nodeList],nodeList))
+    def successors(self):
+        '''return Selection containing successor of each of our nodes'''
+        nodeList:list[Node]=[]
+        return Selection(sum([_.successor() for _ in self.nodeList],nodeList))
+    def clone(self):
+        '''return Selection containing a copy of our nodes'''
+        return Selection([_.clone(None) for _ in self.nodeList])
+    def addClass(self, name):
+        '''add class %(name)s to each of our children'''
+        for n in self.nodeList:
+            if isinstance(n,Tag):
+                n.addClass(name)
                 pass
-            raise Exception(' and '.join([f'failed to decode as {t} because {e}' for t,e in exceptions]))
-        except Exception:
-            raise in_function_context(UnionCodec.decode,vars()) from None
-        pass
-    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
-        return {
-            "oneOf": [ codec.get_json_schema(definitions, self_ref) for codec in self.value_codecs.values() ]
-        }
-    pass
-
-class DictCodec:
-    def __init__(self, key_codec, value_codec):
-        self.key_codec=key_codec
-        self.value_codec=value_codec
-    def encode(self,x:dict,back_ref:None|Callable[[Any],JsonType])->dict:
-        if type(x) is not dict:
-            raise Exception(f'{x!r} is not a dict')
-        result:dict={}
-        for k,v in x.items():
-            ek,ev=self.key_codec.encode(k,back_ref),self.value_codec.encode(v,back_ref)
-            if not isinstance(ek, str):
-                raise Exception(f'key encoder {self.key_codec} produced non-str {ek} from dict key {k}')
-            result[ek]=ev
             pass
-        return result
-    def decode(self,x,back_ref:None|Callable[[JsonType],Any])->dict:
-        if type(x) is not dict:
-            raise Exception(f'{x!r} is not a dict')
-        return {self.key_codec.decode(k,back_ref):self.value_codec.decode(v,back_ref)
-                for k,v in x.items()}
-    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
-        return {
-            'type': 'object',
-            'additionalProperties': self.value_codec.get_json_schema(definitions, self_ref)
-        }
-    pass
-
-class AnyDictCodec:
-    def __init__(self):
-        self.key_codec=NoopCodec[str](str)
-        self.value_codec=AnyJsonCodec()
-    def encode(self,x:dict,back_ref:None|Callable[[Any],JsonType])->dict:
-        if type(x) is not dict:
-            raise Exception(f'{x!r} is not a dict')
-        result:dict={}
-        for k,v in x.items():
-            ek,ev=self.key_codec.encode(k,back_ref),self.value_codec.encode(v,back_ref)
-            result[ek]=ev
+        return self
+    def removeClass(self, name):
+        '''remove class %(name)s from each of our children'''
+        for n in self.nodeList:
+            if isinstance(n,Tag):
+                n.removeClass(name)
+                pass
+            pass
+        return self
+    def hasClass(self,c):
+        '''True iff all our nodes have class c'''
+        each=[True for _ in self.nodeList if isinstance(_,Tag) and _.hasClass(c)]
+        return len(each)==len(self.nodeList)
+    def attr(self, name, value=None, joiner=u''):
+        '''attr('src') gets the values of the src attributes of our nodes and joins them with joiner, returning a single string'''
+        """attr('src','fred') sets the src attribute of our only node to 'fred'"""
+        if value is None:
+            return joiner.join([_.attr(name, value) for _ in self.nodeList if isinstance(_,Tag)])
+        [_.attr(name, value) for _ in self.nodeList if isinstance(_,Tag)]
+        return self
+    def attrs(self, name, value=None):
+        '''attrs('src') lists the values of the src attributes of each of our nodes'''
+        """attrs('src','fred.html') sets the src attribute of each of our nodes to 'html'"""
+        if value is None:
+            return [_.attr(name, value) for _ in self.nodeList if isinstance(_,Tag)]
+        [_.attr(name, value) for _ in self.nodeList if isinstance(_,Tag)]
+        return self
+    def removeAttr(self, name):
+        [_.removeAttr(name) for _ in self.nodeList if isinstance(_,Tag)]
+        return self
+    def join(self,nodes):
+        '''return new Selection containing nodes with each separated by a clone of our nodes'''
+        if isinstance(nodes, Selection):
+            nodes=nodes.nodeList
+            pass
+        resultNodes=[]
+        for i,n in enumerate(nodes):
+            resultNodes.append(n)
+            if i+1 < len(nodes): resultNodes.extend(self.clone().nodeList)
             pass
+        return Selection(resultNodes)
+    def __str__(self):
+        '''re-format as html'''
+        return ''.join([str(_) for _ in self.nodeList])
+    def __len__(self):
+        return len(self.nodeList)
+    def __getitem__(self, key):
+        return Selection(self.nodeList.__getitem__(key))
+    def __add__(self, b):
+        if isinstance(b,Selection):
+            return Selection(self.nodeList+b.nodeList)
+        return NotImplemented
+    def utf8(self):
+        return str(self).encode('utf-8')
+    pass
+
+# basic predicates
+def hasClass(c:str):
+    return lambda node: isinstance(node, Tag) and node.hasClass(c)
+def tagName(t:str):
+    return lambda node: isinstance(node, Tag) and node.tagName==t
+def attrEquals(attr:str,value:str):
+    return lambda node: isinstance(node, Tag) and node.attrEquals(attr,value)
+def hasAttr(attr):
+    return lambda node: isinstance(node, Tag) and node.hasAttr(attr)
+
+def parse(s:str, origin='unknown') -> Selection:
+    '''parse HTML string "%(origin)s"'''
+    parser=Parser(origin)
+    try:
+        u=str(s)
+        parser.feed(u)
+        parser.close()
+        result=Selection(parser.root.children)
+        result.detach()
         return result
-    def decode(self,x,back_ref:None|Callable[[JsonType],Any])->dict:
-        if type(x) is not dict:
-            raise Exception(f'{x!r} is not a dict')
-        return {self.key_codec.decode(k,back_ref):self.value_codec.decode(v,back_ref) for k,v in x.items()}
-    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
-        return {
-            'type': 'object'
-        }
-    pass
-
-class AnyJsonCodec:
-    def encode(self,x,_:None|Callable[[Any],JsonType]):
-        # we assume x will be subsequently json.dumps()ed so defer validation to that
-        return x
-    def decode(self,x,_:None|Callable[[JsonType],Any]):
-        # we assume x was json.loads()ed so assume it is appropriate
-        return x
-    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
-        return {
-            "oneOf": [ { 'type': t } for t in ['null','boolean','object','array','number','string'] ]
-        }
-    pass
-
-class NewIntCodec(Generic[NewInt]):
-    t:Type[NewInt]
-    def __init__(self,t:Type[NewInt]):
-        self.t=t
-        self.base_codec=NoopCodec[int](int)
-    def encode(self, x:NewInt,back_ref:None|Callable[[Any],JsonType])->int:
-        if not isinstance(x, xju.newtype.Int):
-            raise Exception(f'{x!r} is not a {self.t}')
-        return self.base_codec.encode(x.value(),back_ref)
-    def decode(self, x:JsonType,back_ref:None|Callable[[JsonType],Any])->NewInt:
-        if not isinstance(x, int):
-            t=type(x)
-            raise Exception(f'{x!r} (of type {t}) is not an int')
-        return self.t(self.base_codec.decode(x,back_ref))
-    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
-        return {
-            'description': self.t.__name__,
-            'type': 'integer'
-        }
-    pass
-
-class NewFloatCodec(Generic[NewFloat]):
-    t:Type[NewFloat]
-    def __init__(self,t:Type[NewFloat]):
-        self.t=t
-        self.base_codec=NoopCodec[float](float)
-    def encode(self, x:NewFloat,back_ref:None|Callable[[Any],JsonType])->float:
-        if not isinstance(x, xju.newtype.Float):
-            raise Exception(f'{x!r} is not a {self.t}')
-        return self.base_codec.encode(x.value(),back_ref)
-    def decode(self, x:JsonType,back_ref:None|Callable[[JsonType],Any])->NewFloat:
-        if type(x) is not float and type(x) is not int:
-            t=type(x)
-            raise Exception(f'{x!r} (of type {t}) is not a float (or an int)')
-        return self.t(self.base_codec.decode(x,back_ref))
-    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
-        return {
-            'description': self.t.__name__,
-            'type': 'number'
-        }
-    pass
-
-class NewStrCodec(Generic[NewStr]):
-    t:Type[NewStr]
-    def __init__(self,t:Type[NewStr]):
-        self.t=t
-        self.base_codec=NoopCodec[str](str)
-    def encode(self, x:NewStr,back_ref:None|Callable[[Any],JsonType])->str:
-        if not isinstance(x, xju.newtype.Str):
-            raise Exception(f'{x!r} is not a {self.t}')
-        return self.base_codec.encode(x.value(),back_ref)
-    def decode(self, x:JsonType,back_ref:None|Callable[[JsonType],Any])->NewStr:
-        if type(x) is not str:
-            t=type(x)
-            raise Exception(f'{x!r} (of type {t}) is not an str')
-        return self.t(self.base_codec.decode(x,back_ref))
-    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
-        return {
-            'description': self.t.__name__,
-            'type': 'string'
-        }
-    pass
-
-class LiteralStrCodec:
-    value:str
-    def __init__(self,value:str):
-        self.value=value
-    def encode(self, x:str, _:None|Callable[[Any],JsonType])->str:
-        if type(x) is not str or x != self.value:
-            raise Exception(f'{x!r} is not {self.value!r}')
-        return x
-    def decode(self, x:JsonType,_:None|Callable[[JsonType],Any])->str:
-        if type(x) is not str:
-            raise Exception(f'{x!r} is not a string')
-        if x != self.value:
-            raise Exception(f'{x!r} is not {self.value!r}')
-        return x
-    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
-        return {
-            'type': 'string',
-            'enum': [ self.value ]
-        }
-    pass
-
-class SelfCodec:
-    def encode(self,x,back_ref:None|Callable[[Any],JsonType]) -> JsonType:
-        'encode {x} as a Self'
-        try:
-            assert back_ref is not None
-            return back_ref(x)
-        except Exception:
-            raise in_function_context(SelfCodec.encode,vars()) from None
-        pass
-    def decode(self,x,back_ref:None|Callable[[JsonType],Any]) -> object:
-        'deocde {x} as a Self'
-        try:
-            assert back_ref is not None
-            return back_ref(x)
-        except Exception:
-            raise in_function_context(SelfCodec.decode,vars()) from None
-        pass
-    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
-        return {
-            '$ref': self_ref
-        }
+    except:
+        raise ParseFailed(str(''.join(traceback.format_tb(sys.exc_info()[2])))+'\n'+str(sys.exc_info()[1]), parser.pos()) from None
     pass
-    
-class ClassCodec:
-    t:type
-    attr_codecs:dict[str,Any]  # codec
-    def __init__(self, t:type, attr_codecs:dict[str,Any]):
-        self.t=t
-        self.attr_codecs=attr_codecs
-        pass
-    def encode(self,x,_:None|Callable[[Any],JsonType]) -> dict:
-        'encode {x} as a {self.t}'
-        try:
-            if type(x) is not self.t:
-                xt=type(x)
-                raise Exception(f'{x!r} (of type {xt}) is not a {self.t}')
-            def back_ref(x:Any) -> JsonType:
-                return self.encode(x,None)
-            result={}
-            for n, attr_codec in self.attr_codecs.items():
-                try:
-                    result[n]=attr_codec.encode(getattr(x,n),back_ref)
-                except Exception:
-                    raise in_context(f'encode attribute {n}') from None
-                pass
-            return result
-        except Exception:
-            raise in_function_context(ClassCodec.encode,vars()) from None
-        pass
-    def decode(self,x,_:None|Callable[[JsonType],Any]) -> object:
-        'deocde {x} as a {self.t}'
-        try:
-            def back_ref(x:JsonType) -> object:
-                return self.decode(x,None)
-            attr_values=[]
-            for n, attr_codec in self.attr_codecs.items():
-                try:
-                    if n not in x:
-                        raise Exception(f'{x!r} has no {n!r} attribute')
-                    value=attr_codec.decode(x[n],back_ref)
-                    if not isinstance(attr_codec,LiteralStrCodec):
-                        attr_values.append(value)
-                        pass
-                except Exception:
-                    raise in_context(f'decode attribute {n}') from None
-                pass
-            return self.t(*attr_values)
-        except Exception:
-            raise in_function_context(ClassCodec.decode,vars()) from None
-        pass
-    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
-        fqn=f'{self.t.__module__}.{self.t.__name__}'
-        self_ref=f'#/definitions/{fqn}'
-        if not fqn in definitions:
-            definitions[fqn]={
-                'description': self.t.__name__,
-                'type': 'object',
-                'properties': {
-                    n: attr_codec.get_json_schema(definitions, self_ref)
-                    for n, attr_codec in self.attr_codecs.items()
-                }
-            }
-            pass
-        return {
-            '$ref': self_ref
-        }
-    pass
-    
-def _explodeSchema(t:type):
-    '''explode type {t} into a tree of codecs'''
+
+def parseFile(fileName,encoding='utf-8') -> Selection:
+    '''parse {fileName} as HTML'''
     try:
-        if t is float:
-            return NoopCodec[float](float)
-        if t is int:
-            return NoopCodec[int](int)
-        if t is str:
-            return NoopCodec[str](str)
-        if t is bool:
-            return NoopCodec[bool](bool)
-        if t is None or t is NoneType:
-            return NoneCodec()
-        if t is list:
-            return AnyListCodec()
-        if type(t) is GenericAlias and getattr(t, '__origin__') is list:
-            return ListCodec(_explodeSchema(getattr(t,'__args__')[0]))
-        if type(t) is _LiteralGenericAlias:
-            value = t.__args__[0]
-            if not isinstance(value,str):
-                raise Exception(f'{t!r} literal type is not supported (only string is implemented)')
-            return LiteralStrCodec(value)
-        if type(t) is GenericAlias and getattr(t, '__origin__') is tuple:
-            return TupleCodec([_explodeSchema(_) for _ in getattr(t,'__args__')])
-        if t is dict:
-            return AnyDictCodec()
-        if type(t) is GenericAlias and getattr(t, '__origin__') is dict:
-            return DictCodec(*[_explodeSchema(_) for _ in getattr(t,'__args__')])
-        if type(t) is UnionType:
-            return UnionCodec(getattr(t,'__args__'))
-        if type(t) is _UnionGenericAlias:
-            return UnionCodec(getattr(t,'__args__'))
-        if t is Self:
-            return SelfCodec()
-        if issubclass(t,xju.newtype.Int):
-            return NewIntCodec(t)
-        if issubclass(t,xju.newtype.Float):
-            return NewFloatCodec(t)
-        if issubclass(t,xju.newtype.Str):
-            return NewStrCodec(t)
-        return ClassCodec(
-            t,{n: _explodeSchema(nt) for n,nt in
-               sum([list(getattr(c,'__annotations__',{}).items()) for c in reversed(t.__mro__)],[])})
+        with open(fileName,encoding=encoding) as f:
+            return parse(f.read(),fileName)
+        pass
     except Exception:
-        raise in_function_context(_explodeSchema,vars()) from None
+        raise in_function_context(parseFile,vars())
+    pass
+
+# deprecated, use parseFile
+def loadFile(fileName,encoding='utf-8'):
+    return parseFile(fileName,encoding)
     pass
```

### Comparing `xju-1.2.8/src/xju/json_codec.py.test` & `xju-1.2.9/src/xju/json_codec.py.test`

 * *Files 16% similar despite different names*

```diff
@@ -15,99 +15,99 @@
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 #
 from sys import path
 from os.path import dirname
 if path[0]==dirname(__file__): path.pop(0)
 
-from xju.json_codec import Codec, JsonType, AnyJsonCodec, SelfCodec
+from xju.json_codec import codec, Codec, JsonType, AnyJsonCodec, SelfCodec
 
 from typing import cast, Type, Literal, Any, Self
 from types import NoneType
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 import re
 import sys
 
 from xju.assert_ import Assert
 import xju.newtype
 from xju.xn import readable_repr
 
 x:Any
 
 
 # int,str,bool,float,None map directly
 
-Assert(Codec[int](int).decode(3))==3
-Assert(Codec[str](str).decode('fred'))=='fred'
-Assert(Codec[bool](bool).decode(True))==True
-Assert(Codec[float](float).decode(5.5))==5.5
-Assert(Codec[float](float).decode(5))==5
-
-Assert(Codec[int](int).encode(3))==3
-Assert(Codec[str](str).encode('fred'))=='fred'
-Assert(Codec[bool](bool).encode(True))==True
-Assert(Codec[float](float).encode(5.5))==5.5
-Assert(Codec[float](float).encode(5))==5
+Assert(codec(int).decode(3))==3
+Assert(codec(str).decode('fred'))=='fred'
+Assert(codec(bool).decode(True))==True
+Assert(codec(float).decode(5.5))==5.5
+Assert(codec(float).decode(5))==5
+
+Assert(codec(int).encode(3))==3
+Assert(codec(str).encode('fred'))=='fred'
+Assert(codec(bool).encode(True))==True
+Assert(codec(float).encode(5.5))==5.5
+Assert(codec(float).encode(5))==5
 
 # note None is a bit weird, sometimes it acts as as a type, others not
-Assert(Codec[None](type(None)).decode(None))==None
-Assert(Codec[None](type(None)).encode(None))==None
+Assert(codec(type(None)).decode(None))==None
+Assert(codec(type(None)).encode(None))==None
 
 
 # list maps to list...
-Assert(Codec[list](list).decode([5, 'fred']))==[5, 'fred']
-Assert(Codec[list](list).encode([5, 'fred']))==[5, 'fred']
+Assert(codec(list).decode([5, 'fred']))==[5, 'fred']
+Assert(codec(list).encode([5, 'fred']))==[5, 'fred']
 
 # ... but must be given a list
 try:
-    x=Codec[list](list).decode(8)
+    x=codec(list).decode(8)
 except Exception as e:
     Assert("8 is not a list").isIn(str(e))
 else:
     assert False, x
     pass
 # ... note element types are not checked (it is assumed
 # result will be given to json.dumps, which will fail), e.g.
 # we can happily put print, which has no mapping to a json type,
 # into a non-type-adorned list and encode that list:
-Assert(Codec[list](list).encode([print]))==[print]
+Assert(codec(list).encode([print]))==[print]
 
 
 # type-adorned list maps to list...
-Assert(Codec[list[int]](list[int]).decode([5, 6]))==[5, 6]
-Assert(Codec[list[int]](list[int]).encode([5, 6]))==[5, 6]
+Assert(codec(list[int]).decode([5, 6]))==[5, 6]
+Assert(codec(list[int]).encode([5, 6]))==[5, 6]
 
 # ... but must be given a list...
 try:
-    x=Codec[list[int]](list[int]).decode(8)
+    x=codec(list[int]).decode(8)
 except Exception as e:
     Assert("8 is not a list").isIn(str(e))
 else:
     assert False, x
     pass
 
 # ... and all values must have correct type
 try:        
-    x=Codec[list[int]](list[int]).decode([5, 'fred'])
+    x=codec(list[int]).decode([5, 'fred'])
 except Exception as e:
     Assert("'fred' (of type <class 'str'>) is not a <class 'int'>").isIn(str(e))
 else:
     assert False, x
     pass
 
 
 # tuple encodes as list (note, tuples without specific element types are disallowed)
 
 #mypy 1.0.0 bug:
-#c=Codec[tuple[int,str]](tuple[int,str])
+#c=codec(tuple[int,str])
 # ... says:
 # /home/xju/urnest/xju/json_codec.py.test:43: error: Argument 1 to "Codec" has incompatible type "Type[Tuple[Any, ...]]"; expected "Type[Tuple[int, str]]"  [arg-type]
 # ... but there are so many tuple-related bugs on github it's not really surprising
 
-tuple_codec=Codec[tuple[int,str]](cast(Type[tuple[int,str]],tuple[int,str]))  #mypy 1.0.0 bug
+tuple_codec=codec(cast(Type[tuple[int,str]],tuple[int,str]))  #mypy 1.0.0 bug
 Assert(tuple_codec.decode([5, 'fred']))==(5, 'fred')
 Assert(tuple_codec.encode((5, 'fred')))==[5, 'fred']
 
 # for list to decode as tuple, it must be a list in the first place...
 try:        
     x=tuple_codec.decode({'x':6, 'y':8})
 except Exception as e:
@@ -142,156 +142,157 @@
     Assert("(5, 6, 7) does not have 2 items (it has 3 items)").isIn(str(e))
 else:
     assert False, x
     pass
 
 
 # dict with no type hints allows any keys with any value types (key must be string)
-Assert(Codec[dict](dict).decode({'fred':5, 'jock': 'nine'}))=={'fred':5, 'jock':'nine'}
-Assert(Codec[dict](dict).encode({'fred':5, 'jock': 'nine'}))=={'fred':5, 'jock':'nine'}
+Assert(codec(dict).decode({'fred':5, 'jock': 'nine'}))=={'fred':5, 'jock':'nine'}
+Assert(codec(dict).encode({'fred':5, 'jock': 'nine'}))=={'fred':5, 'jock':'nine'}
 
 # dict with specific value type...
-Assert(Codec[dict[str,int]](dict[str,int]).decode({'fred':5, 'jock': 9}))=={'fred':5, 'jock':9}
-Assert(Codec[dict[str,int]](dict[str,int]).encode({'fred':5, 'jock': 9}))=={'fred':5, 'jock':9}
+Assert(codec(dict[str,int]).decode({'fred':5, 'jock': 9}))=={'fred':5, 'jock':9}
+Assert(codec(dict[str,int]).encode({'fred':5, 'jock': 9}))=={'fred':5, 'jock':9}
 
 # ... must be given a dict...
 try:
-    x=Codec[dict](dict).decode(7)
+    x=codec(dict).decode(7)
 except Exception as e:
     Assert("7 is not a dict").isIn(str(e))
 else:
     assert False, x
     pass
 try:
-    x=Codec[dict[str,int]](dict[str,int]).decode(7)
+    x=codec(dict[str,int]).decode(7)
 except Exception as e:
     Assert("7 is not a dict").isIn(str(e))
 else:
     assert False, x
     pass
 
 # ... expects all elements to have that value type incorrect dict value type
 try:
-    x=Codec[dict[str,int]](dict[str,int]).decode({'jock': 'fred'})
+    x=codec(dict[str,int]).decode({'jock': 'fred'})
 except Exception as e:
     Assert("'fred' (of type <class 'str'>) is not a <class 'int'>").isIn(str(e))
 else:
     assert False, x
     pass
 
 # dict keys must be strings...
 try:
-    x=Codec[dict](dict).encode({6: 'fred'})
+    x=codec(dict).encode({6: 'fred'})
 except Exception as e:
     Assert(str(e)).matches("6 is not a <class 'str'>")
 else:
     assert False, x
     pass
 try:
-    x=Codec[dict[int,int]](dict[int,int]).encode({7:5}) # type: ignore
+    x=codec(dict[int,int]).encode({7:5}) # type: ignore
 except Exception as e:
     Assert("produced non-str 7 from dict key 7").isIn(str(e))
 else:
     assert False, x
     pass
 
 # ... must be given a dict...
 try:
-    x=Codec[dict](dict).encode(7) # type: ignore
+    x=codec(dict).encode(7) # type: ignore
 except Exception as e:
     Assert("7 is not a dict").isIn(str(e))
 else:
     assert False, x
     pass
 try:
-    x=Codec[dict[str,int]](dict[str,int]).encode(7) # type: ignore
+    x=codec(dict[str,int]).encode(7) # type: ignore
 except Exception as e:
     Assert("7 is not a dict").isIn(str(e))
 else:
     assert False, x
     pass
 
 #xju.newtype.Int support
 class AgeInYearsTag:pass
 class AgeInYears(xju.newtype.Int[AgeInYearsTag]):pass
 
-Assert(Codec[AgeInYears](AgeInYears).decode(3))==AgeInYears(3)
-Assert(Codec[AgeInYears](AgeInYears).encode(AgeInYears(3)))==3
+Assert(codec(AgeInYears).decode(3))==AgeInYears(3)
+Assert(codec(AgeInYears).encode(AgeInYears(3)))==3
 
 try:
-    x=Codec[AgeInYears](AgeInYears).decode('fred')
+    x=codec(AgeInYears).decode('fred')
 except Exception as e:
     Assert("'fred' (of type <class 'str'>) is not an int").isIn(str(e))
 else:
     assert False, x
     pass
 
 try:        
-    x=Codec[AgeInYears](AgeInYears).encode(8) # type: ignore
+    x=codec(AgeInYears).encode(8) # type: ignore
 except Exception as e:
     Assert("8 is not a <class '__main__.AgeInYears'>").isIn(str(e))
 else:
     assert False, x
     pass
 
 #xju.newtype.Float support
 class MetresTag:pass
 class Metres(xju.newtype.Float[MetresTag]):pass
 
-Assert(Codec[Metres](Metres).decode(3.8))==Metres(3.8)
-Assert(Codec[Metres](Metres).encode(Metres(3.8)))==3.8
-Assert(Codec[Metres](Metres).decode(3))==Metres(3)
-Assert(Codec[Metres](Metres).encode(Metres(3)))==3
+Assert(codec(Metres).decode(3.8))==Metres(3.8)
+Assert(codec(Metres).encode(Metres(3.8)))==3.8
+Assert(codec(Metres).decode(3))==Metres(3)
+Assert(codec(Metres).encode(Metres(3)))==3
 
 try:
-    x=Codec[Metres](Metres).decode('fred')
+    x=codec(Metres).decode('fred')
 except Exception as e:
     Assert("'fred' (of type <class 'str'>) is not a float (or an int)").isIn(str(e))
 else:
     assert False, x
     pass
 
 try:
-    x=Codec[Metres](Metres).encode('fred') # type: ignore
+    x=codec(Metres).encode('fred') # type: ignore
 except Exception as e:
     Assert("'fred' is not a <class '__main__.Metres'>").isIn(str(e))
 else:
     assert False, x
     pass
 
 #xju.newtype.Str support
 class SurnameTag:pass
 class Surname(xju.newtype.Str[SurnameTag]):pass
 
-Assert(Codec[Surname](Surname).decode('Ang'))==Surname('Ang')
-Assert(Codec[Surname](Surname).encode(Surname('Ang')))=='Ang'
+Assert(codec(Surname).decode('Ang'))==Surname('Ang')
+Assert(codec(Surname).encode(Surname('Ang')))=='Ang'
 
 try:
-    x=Codec[Surname](Surname).decode(17)
+    x=codec(Surname).decode(17)
 except Exception as e:
     Assert("17 (of type <class 'int'>) is not an str").isIn(str(e))
 else:
     assert False, x
     pass
 
 try:
-    x=Codec[Surname](Surname).encode(17) # type: ignore
+    x=codec(Surname).encode(17) # type: ignore
 except Exception as e:
     Assert("17 is not a <class '__main__.Surname'>").isIn(str(e))
 else:
     assert False, x
     pass
 
+# type unions, e.g. str|int match either type
 
 #mypy 1.0.0 bug
 #union_codec=Codec[str|int](str|int)
 # says:
 #  error: Argument 1 to "Codec" has incompatible type "UnionType"; expected "Union[Type[str], Type[int]]"  [arg-type]
 
-union_codec=Codec[str|int](cast(Type[str|int],str|int))
+union_codec=codec(cast(Type[str|int],str|int))
 Assert(union_codec.decode('fred'))=='fred'
 Assert(union_codec.decode(9))==9
 Assert(union_codec.encode('fred'))=='fred'
 Assert(union_codec.encode(9))==9
 
 #incorrect dict value type
 try:
@@ -299,14 +300,17 @@
 except Exception as e:
     Assert(str(e)).matches("failed to decode 5.7 to a str | int because.*failed to decode as <class 'str'> because 5.7 (of type <class 'float'>) is not a <class 'str'> and failed to decode as <class 'int'> because 5.7 (of type <class 'float'>) is not a <class 'int'>")
 else:
     assert False, x
     pass
 
 
+# class (object) support:
+#   encoding is dictionary containing each objct attribute (except that string literal
+#   attributes are treated specially, see string literal attributes below)
 class StreetTag:pass
 class Street(xju.newtype.Str[StreetTag]):pass
 
 class SuburbTag:pass
 class Suburb(xju.newtype.Str[SuburbTag]):pass
 
 class PostcodeTag:pass
@@ -315,45 +319,45 @@
 @dataclass
 class Address:
     street:Street
     suburb:Suburb
     postcode:Postcode
 
 
-Assert(Codec[Address](Address).decode({
+Assert(codec(Address).decode({
     'street':'alba',
     'suburb': 'bocca',
     'postcode': 3365}))==Address(Street('alba'),Suburb('bocca'),Postcode(3365))
         
-Assert(Codec[Address](Address).encode(Address(Street('alba'),Suburb('bocca'),Postcode(3365))))=={
+Assert(codec(Address).encode(Address(Street('alba'),Suburb('bocca'),Postcode(3365))))=={
     'street':'alba',
     'suburb': 'bocca',
     'postcode': 3365}
         
 #incorrect Address value type
 try:
-    x=Codec[Address](Address).decode({'jock': 'fred'})
+    x=codec(Address).decode({'jock': 'fred'})
 except Exception as e:
     Assert(str(e)).matches(re.escape("failed to decode {'jock': 'fred'} to a <class '__main__.Address'> because"))
-    Assert(str(e)).endswith("{'jock': 'fred'} has no 'street' attribute")
+    Assert(str(e)).endswith("missing 3 required positional arguments: 'street', 'suburb', and 'postcode'")
 else:
     assert False, x
     pass
 
 try:
-    x=Codec[Address](Address).encode(7) # type: ignore
+    x=codec(Address).encode(7) # type: ignore
 except Exception as e:
     Assert(str(e)).endswith("7 (of type <class 'int'>) is not a <class '__main__.Address'>")
 else:
     assert False, x
     pass
 
 bad_postcode=Address(Street('alba'),Suburb('bocca'),3365)  # type: ignore
 try:
-    x=Codec[Address](Address).encode(bad_postcode)
+    x=codec(Address).encode(bad_postcode)
 except Exception as e:
     Assert(str(e)).endswith("3365 is not a <class '__main__.Postcode'>")
 else:
     assert False, x
     pass
 
 class UnitTag: pass
@@ -373,32 +377,32 @@
 # ... __init__ argument order is assumed to be that used by dataclass, i.e. classes in
 # reverse-mro (see python mro() and __mro__) with attributes of each class in usual order, so
 # order of UnitAddress __init__ args is
 # ManagerName attrs in order (i.e. a, b) then Address attrs in order (i.e. street, suburb, postcode)
 # then UnitAddress attributes in order (i.e. unit), so in total:
 # a, b, street, suburb, postcode.
 # Decode does not care about json dict order...
-Assert(Codec[UnitAddress](UnitAddress).decode({
+Assert(codec(UnitAddress).decode({
     'street':'alba',
     'suburb': 'bocca',
     'postcode': 3365,
     'unit': '17a',
     'a': 'fred',
     'b': 17}))==UnitAddress('fred',17,Street('alba'),Suburb('bocca'),Postcode(3365),Unit('17a'))
 
 # ... encode will order attrs per description above
-Assert(Codec[UnitAddress](UnitAddress).encode(
+Assert(codec(UnitAddress).encode(
     UnitAddress('fred',17,Street('alba'),Suburb('bocca'),Postcode(3365),unit=Unit('17a'))))=={
         'a': 'fred',
         'b': 17,
         'street':'alba',
         'suburb': 'bocca',
         'postcode': 3365,
         'unit': '17a'}
-Assert(list(cast(dict,Codec[UnitAddress](UnitAddress).encode(
+Assert(list(cast(dict,codec(UnitAddress).encode(
     UnitAddress('fred',17,Street('alba'),Suburb('bocca'),Postcode(3365),unit=Unit('17a')))).keys()))==[
         'a',
         'b',
         'street',
         'suburb',
         'postcode',
         'unit']
@@ -406,151 +410,170 @@
 
 # string Literal
 #mypy 1.0.0 bug:
 #Codec[Literal['fred']](Literal['fred'])
 # ... says:
 #  error: Argument 1 to "Codec" has incompatible type "object"; expected "Type[Literal['fred']]"  [arg-type]
 
-Assert(Codec[Literal['fred']](Literal['fred']).decode('fred'))=='fred' # type: ignore
-Assert(Codec[Literal['fred']](Literal['fred']).encode('fred'))=='fred' # type: ignore
+Assert(codec(Literal['fred']).decode('fred'))=='fred' # type: ignore
+Assert(codec(Literal['fred']).encode('fred'))=='fred' # type: ignore
 
 #non-string literal not yet implemented
 try:
-    x=Codec[Literal[7]](Literal[7]).decode(7) # type: ignore
+    x=codec(Literal[7]).decode(7) # type: ignore
 except Exception as e:
     Assert("typing.Literal[7] literal type is not supported (only string is implemented)").isIn(str(e))
 else:
     assert False, x
     pass
 
 
 #encode wrong type
 try:
-    x=Codec[Literal['fred']](Literal['fred']).encode(7) # type: ignore
+    x=codec(Literal['fred']).encode(7) # type: ignore
 except Exception as e:
     Assert("7 is not 'fred'").isIn(str(e))
 else:
     assert False, x
     pass
 #decode wrong type
 try:
-    x=Codec[Literal['fred']](Literal['fred']).decode(7) # type: ignore
+    x=codec(Literal['fred']).decode(7) # type: ignore
 except Exception as e:
     Assert("7 is not a string").isIn(str(e))
 else:
     assert False, x
     pass
 
-
+# string literal attributes match that string literal...
 @dataclass
 class Add:
     a:int
     b:int
-    op_type: Literal['add'] = 'add'
+    op_type: Literal['add'] = 'add'  # note default value not required but recommended, see below
 
-Assert(Codec[Add](Add).decode({
-    'op_type':'add',
-    'a': 7,
-    'b': 8}))==Add(7,8)
+Assert(codec(Add).decode(
+    {
+        'op_type':'add',
+        'a': 7,
+        'b': 8
+    }))==Add(7,8)
         
-Assert(Codec[Add](Add).decode({
+Assert(codec(Add).decode({
     'op_type':'add',
     'a': 7,
     'b': 8}).op_type)=='add'
         
-Assert(Codec[Add](Add).encode(Add(7,8))=={
+Assert(codec(Add).encode(Add(7,8))=={
     'op_type':'add',
     'a': 7,
     'b': 8})
         
-#incorrect value type
+# ... and rejected other values...
 try:
-    x=Codec[Add](Add).decode({
+    x=codec(Add).decode({
         'op_type':'subtract',
         'a': 7,
         'b': 8})
 except Exception as e:
     Assert(str(e)).contains("'subtract' is not 'add'")
 else:
     assert False, x
     pass
 
-
+# ... allowing them to be used as type descriminators...
 @dataclass
 class Sub:
     a:int
     b:int
     op_type: Literal['sub'] = 'sub'
 
-Assert(Codec[Add|Sub](Add|Sub).decode({  # type: ignore
+Assert(codec(Add|Sub).decode({  # type: ignore
     'op_type':'sub',
     'a': 7,
     'b': 8}))==Sub(7,8)
 
+# ... without defaults, string literal attributes still work...
+@dataclass
+class MissingDefault:
+    op_type: Literal['op']
+    sub_type: Literal['plus']
+    a:int
+    b:int
+    pass
+
+Assert(codec(MissingDefault).decode({
+    'op_type':'op',
+    'sub_type':'plus',
+    'a': 7,
+    'b': 8}))==MissingDefault('op', 'plus', 7, 8)
+
+# ... but always need to be passed literal value.
+
 
 # misc coverage
-Assert(repr(Codec[int](int)))=="<class 'int'> json codec"
+Assert(repr(codec(int)))=="<class 'int'> json codec"
 
 
-Assert(Codec[int|None](int|None).decode(None))==None # type: ignore
-Assert(Codec[int|None](int|None).encode(None))==None # type: ignore
+Assert(codec(int|None).decode(None))==None # type: ignore
+Assert(codec(int|None).encode(None))==None # type: ignore
 
 try:
-    x=Codec[int|None](int|None).decode('fred')  # type: ignore
+    x=codec(int|None).decode('fred')  # type: ignore
 except Exception as e:
     Assert(str(e)).contains("'fred' is not None")
 else:
     assert False, x
     pass
 
 try:
-    x=Codec[int|None](int|None).encode('fred')  # type: ignore
+    x=codec(int|None).encode('fred')  # type: ignore
 except Exception as e:
     Assert(str(e)).contains("'fred' is not None")
 else:
     assert False, x
     pass
 
 
 # Codec can generate corresponding json schema (http://json-schema.org)
 # "null", "boolean", "object", "array", "number", "string", or "integer"
-Assert(Codec[None](type(None)).get_json_schema())=={'type': 'null', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
-Assert(Codec[int](int).get_json_schema())=={'type': 'integer', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
-Assert(Codec[bool](bool).get_json_schema())=={'type': 'boolean', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
-Assert(Codec[str](str).get_json_schema())=={'type': 'string', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
-Assert(Codec[float](float).get_json_schema())=={'type': 'number', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
-Assert(Codec[list](list).get_json_schema())=={'type': 'array', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
-Assert(Codec[list[int]](list[int]).get_json_schema())=={'type': 'array', 'items': { 'type': 'integer'}, 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
+Assert(codec(type(None)).get_json_schema())=={'type': 'null', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
+Assert(codec(int).get_json_schema())=={'type': 'integer', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
+Assert(codec(bool).get_json_schema())=={'type': 'boolean', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
+Assert(codec(str).get_json_schema())=={'type': 'string', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
+Assert(codec(float).get_json_schema())=={'type': 'number', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
+Assert(codec(list).get_json_schema())=={'type': 'array', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
+Assert(codec(list[int]).get_json_schema())=={'type': 'array', 'items': { 'type': 'integer'}, 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 # mypy 1.0.0 + python 3.11 bug:
 # Argument 1 to "Codec" has incompatible type "Type[Tuple[Any, ...]]"; expected "Type[Tuple[int, str]]"  [arg-type]
-Assert(Codec[tuple[int,str]](tuple[int,str]).get_json_schema())=={'type': 'array', 'prefixItems': [ { 'type': 'integer'},{ 'type': 'string'}], 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'} # type: ignore
+Assert(codec(tuple[int,str]).get_json_schema())=={'type': 'array', 'prefixItems': [ { 'type': 'integer'},{ 'type': 'string'}], 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'} # type: ignore
 
 # mypy 1.0.0 + python 3.11 bug:
 # Argument 1 to "Codec" has incompatible type "<typing special form>"; expected "Union[Type[None], Type[bool], Type[Dict[Any, Any]], Type[List[Any]], Type[float], Type[str]]"  [arg-type]
-Assert(Codec[JsonType](JsonType).get_json_schema())=={'oneOf': [{'type': 'null'}, {'type': 'boolean'}, {'type': 'object'}, {'type': 'array'}, {'type': 'number'}, {'type': 'string'}], 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'} # type: ignore
+Assert(codec(JsonType).get_json_schema())=={'oneOf': [{'type': 'null'}, {'type': 'boolean'}, {'type': 'object'}, {'type': 'array'}, {'type': 'number'}, {'type': 'string'}], 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'} # type: ignore
 
-Assert(Codec[dict](dict).get_json_schema())=={'type': 'object', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
+Assert(codec(dict).get_json_schema())=={'type': 'object', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 
-Assert(Codec[dict[str,int]](dict[str,int]).get_json_schema())=={'type': 'object', 'additionalProperties': {'type': 'integer'}, 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
+Assert(codec(dict[str,int]).get_json_schema())=={'type': 'object', 'additionalProperties': {'type': 'integer'}, 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 
 Assert(AnyJsonCodec().get_json_schema({},None))== {'oneOf': [{'type': 'null'}, {'type': 'boolean'}, {'type': 'object'}, {'type': 'array'}, {'type': 'number'}, {'type': 'string'}]}
 
-Assert(Codec[AgeInYears](AgeInYears).get_json_schema())=={'description': 'AgeInYears', 'type': 'integer', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
+Assert(codec(AgeInYears).get_json_schema())=={'description': 'AgeInYears', 'type': 'integer', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 
-Assert(Codec[Street](Street).get_json_schema())=={'description': 'Street', 'type': 'string', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
+Assert(codec(Street).get_json_schema())=={'description': 'Street', 'type': 'string', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 
-Assert(Codec[Metres](Metres).get_json_schema())=={'description': 'Metres', 'type': 'number', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
+Assert(codec(Metres).get_json_schema())=={'description': 'Metres', 'type': 'number', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 
-Assert(Codec[Literal['fred']](Literal['fred']).get_json_schema())=={'type': 'string', 'enum': ['fred'], 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'} # type: ignore
+Assert(codec(Literal['fred']).get_json_schema())=={'type': 'string', 'enum': ['fred'], 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'} # type: ignore
 
-Assert(Codec[Address](Address).get_json_schema())=={
-    '$ref': '#/definitions/__main__.Address',
+Assert(codec(Address).get_json_schema())=={
+    '$ref': '#/definitions/Address',
     '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema',
     'definitions':{
-        '__main__.Address':{
+        'Address':{
             'description': 'Address',
             'type': 'object',
             'properties': {'street': {'description': 'Street', 'type': 'string'}, 'suburb': {'description': 'Suburb', 'type': 'string'}, 'postcode': {'description': 'Postcode', 'type': 'integer'}}}}}
 
 
 
 # recursive via Self
@@ -560,45 +583,45 @@
 @dataclass
 class Branch:
     shoots: list[Leaf|Self]
     pass
 
 Tree = Branch|Leaf
 
-Assert(Codec[Branch](Branch).encode(Branch([Branch([Leaf(1),Leaf(2)]),Leaf(3)])))=={'shoots':[{'shoots':[1,2]},3]}
-Assert(Codec[Branch](Branch).decode({'shoots':[{'shoots':[1,2]},3]}))==Branch([Branch([Leaf(1),Leaf(2)]),Leaf(3)])
-Assert(Codec[Branch](Branch).get_json_schema())=={
-    '$ref': '#/definitions/__main__.Branch',
+Assert(codec(Branch).encode(Branch([Branch([Leaf(1),Leaf(2)]),Leaf(3)])))=={'shoots':[{'shoots':[1,2]},3]}
+Assert(codec(Branch).decode({'shoots':[{'shoots':[1,2]},3]}))==Branch([Branch([Leaf(1),Leaf(2)]),Leaf(3)])
+Assert(codec(Branch).get_json_schema())=={
+    '$ref': '#/definitions/Branch',
     '$id': 'https://example.com/address.schema.json',
     '$schema': 'https://json-schema.org/draft/2020-12/schema',
     'definitions': {
-        '__main__.Branch': {'description': 'Branch', 'type': 'object', 'properties': {
+        'Branch': {'description': 'Branch', 'type': 'object', 'properties': {
             'shoots': {'type': 'array', 'items': {'oneOf': [
                 {'description': 'Leaf', 'type': 'integer'},
-                {'$ref': '#/definitions/__main__.Branch'}]}}}}}}
+                {'$ref': '#/definitions/Branch'}]}}}}}}
 
 @dataclass
 class Graph:
     value: int
     next: list[Self]
     pass
 
-Assert(Codec[Graph](Graph).encode(
+Assert(codec(Graph).encode(
     Graph(1, [Graph(2,[]),Graph(3,[])])))=={
         'value':1,'next':[
             {'value':2, 'next':[]},
             {'value':3, 'next':[]}]}
-Assert(Codec[Graph](Graph).get_json_schema())=={
-    '$ref': '#/definitions/__main__.Graph',
+Assert(codec(Graph).get_json_schema())=={
+    '$ref': '#/definitions/Graph',
     '$id': 'https://example.com/address.schema.json',
     '$schema': 'https://json-schema.org/draft/2020-12/schema',
     'definitions': {
-        '__main__.Graph': {'description': 'Graph', 'type': 'object', 'properties': {
+        'Graph': {'description': 'Graph', 'type': 'object', 'properties': {
             'value': {'type': 'integer'},
-            'next': {'type': 'array', 'items': {'$ref': '#/definitions/__main__.Graph'}}}}}}
+            'next': {'type': 'array', 'items': {'$ref': '#/definitions/Graph'}}}}}}
 
 def fail_back_ref_encode(x: Any) -> JsonType:
     raise Exception('back_ref fail')
 try:
     SelfCodec().encode(7,fail_back_ref_encode)
 except Exception as e:
     Assert(readable_repr(e))=='Failed to encode 7 as a Self because\nback_ref fail.'
@@ -699,30 +722,99 @@
     x=Codec[tuple[int]](tuple[int]).encode('fred') # type: ignore
 except Exception as e:
     Assert("'fred' is not a tuple").isIn(str(e))
 else:
     assert False, x
     pass
 
+
 # ensure JsonType (Union) selects correct codec to encode dict
 @dataclass
 class Y:
     x: JsonType
     pass
 
 Assert(Codec[Y](Y).encode(Y({ 'z': 'fred' })))=={'x':{'z':'fred'}}
 Assert(Codec[Y](Y).decode({'x':{'z':'fred'}}))==Y({ 'z': 'fred' })
 Assert(Codec[Y](Y).get_json_schema())=={
-    '$ref': '#/definitions/__main__.Y',
+    '$ref': '#/definitions/Y',
     '$id': 'https://example.com/address.schema.json',
     '$schema': 'https://json-schema.org/draft/2020-12/schema',
     'definitions': {
-        '__main__.Y': {
+        'Y': {
             'description': 'Y', 'type': 'object', 'properties': {
                 'x': {
                     'oneOf': [
                         {'type': 'null'},
                         {'type': 'boolean'},
                         {'type': 'object'},
                         {'type': 'array'},
                         {'type': 'number'},
                         {'type': 'string'}]}}}}}
+
+
+# type hint string are supported, allowing forward-decls
+@dataclass
+class ShirtSize:
+    size: 'SizeCode'
+    pass
+
+Small=Literal['S']
+Large=Literal['L']
+SizeCode=Small|Large
+
+Assert(Codec[ShirtSize](ShirtSize).decode(
+    {
+        'size': 'S',
+    }
+))==ShirtSize('S')
+
+
+# coverage of class decode initialisation failure
+class Fred:
+    x: str
+    def __init__(self, x:str):
+        if x=='jock':
+            raise Exception('jock forbidden')
+        pass
+    pass
+
+try:
+    codec(Fred).decode({'x':'jock'})
+except Exception as e:
+    Assert(readable_repr(e))=="Failed to decode {'x': 'jock'} to a <class '__main__.Fred'> because\nfailed to deocde {'x': 'jock'} as a <class '__main__.Fred'> because\nfailed to init <class '__main__.Fred'> with keyword arguments {'x': 'jock'} because\njock forbidden."
+else:
+    assert False
+    pass
+
+# multiple defaults values, including list type, can omit any or all defaulted attributes
+# use kw_only to allow any ordering of attributes in class definition
+# it seems clever but I don't think jsonschema or typescript generation works properly
+# (typescript and jsonschema will insist on the default fields being specified). Note
+# encoding from python will always include the value even if it came from default.
+@dataclass(kw_only=True)
+class Person:
+    first_name: str
+    middle_names: list[str] = field(default_factory=list)
+    last_name: str
+    phobias: list[str] = field(default_factory=list)
+    pass
+
+Assert(codec(Person).decode({'first_name':'fred','last_name':'jones'}))==Person(first_name='fred',last_name='jones')
+Assert(codec(Person).decode({'first_name':'fred','phobias':['spiders'],'last_name':'jones'}))==Person(first_name='fred',last_name='jones',phobias=['spiders'])
+Assert(codec(Person).decode({'first_name':'fred','middle_names':['arachnid'],'last_name':'jones'}))==Person(first_name='fred',last_name='jones',middle_names=['arachnid'])
+
+
+# not-present optional attribute must still appear in json (with value null)
+@dataclass
+class Opt:
+    x: str|None
+    pass
+
+Assert(codec(Opt).decode({'x':None}))==Opt(x=None)
+try:
+    codec(Opt).decode({})
+except Exception as e:
+    Assert(readable_repr(e)).contains("Failed to decode {} to a <class '__main__.Opt'> because\nfailed to deocde {} as a <class '__main__.Opt'> because\nfailed to init <class '__main__.Opt'> with keyword arguments {} because\nOpt.__init__() missing 1 required positional argument: 'x'.")
+else:
+    assert False
+    pass
```

### Comparing `xju-1.2.8/src/xju/jsonschema.py` & `xju-1.2.9/src/xju/jsonschema.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/jsonschema.py.test` & `xju-1.2.9/src/xju/jsonschema.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/misc.py` & `xju-1.2.9/src/xju/misc.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/misc.py.test` & `xju-1.2.9/src/xju/misc.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/newtype.py` & `xju-1.2.9/src/xju/newtype.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,40 +26,37 @@
 #  class HoursTag:pass
 #  class Hours(Int[HoursTag]):pass
 #
 # ... note do not use 'Hours=Int[HoursTag]' because that is an alias to a generic and
 # therefore has not run-time presence and therefore cannot be used with isinstance.
 #
 from typing import Iterable,Sized,Container,Collection,Reversible,Protocol,Type,overload,TypeVar
-from typing import Generic,Tuple,Mapping,Optional,List,Literal,Union,Any,SupportsRound
+from typing import Generic,Tuple,Mapping,Optional,List,Literal,Union,Any,Self
 
 Tag=TypeVar('Tag',covariant=True)
 
 def verify_same_type(x:Any,y:Any):
     if x.__class__ is not y.__class__:
         raise Exception(f"{x!r}'s type {x.__class__} is not the same as {y!r}'s type {y.__class__}")
     pass
 
 def eq(x:Any,y:Any)->bool:
     verify_same_type(x,y)
     return x.value().__eq__(y.value())
 
-class Int_(Generic[Tag]):
+class Int(Generic[Tag]):
     __value:int
 
     def __init__(self, value:int):
         self.__value=value
         pass
 
     def value(self)->int:
         return self.__value
 
-    pass
-
-class Int(Generic[Tag],Int_[Tag],SupportsRound):
     def __eq__(self,other)->bool:
         '''equality test, only valid for two object of exactly the same class; except that
            python insists supporting __eq__ for objects of any type, so this function's signature
            allows it and calls out all nonsense at runtime'''
         '''i.e. recommend stick to using Int[X] like:
               class Hours(Int[HoursTag]):pass
            ... and not inherit from Hours.
@@ -81,111 +78,111 @@
     def __float__(self)->float:
         return self.value().__float__()
     
     def conjugate(self):
         return self.value().conjugate()
 
     @overload
-    def __divmod__(self, x:int) -> 'Tuple[Int[Tag],Int[Tag]]':
+    def __divmod__(self, x:int) -> Tuple[Self,Self]:
         pass
     @overload
     def __divmod__(self, x:float) -> Tuple[float,float]:
         pass
     @overload
-    def __divmod__(self, x:'Int[Tag]') -> Tuple[int,int]:
+    def __divmod__(self, x:Self) -> Tuple[int,int]:
         pass
     def __divmod__(self, x):
         if isinstance(x,int):
             q,r=self.value().__divmod__(x)
             return self.__class__(q),self.__class__(r)
         if isinstance(x,float):
             return divmod(self.value(),x)
         else:
             return divmod(self.value(),x.value())
         pass
 
     @overload
-    def __floordiv__(self, x:int) -> 'Int[Tag]':
+    def __floordiv__(self, x:int) -> Self:
         pass
     @overload
     def __floordiv__(self, x:float) -> float:
         pass
     @overload
-    def __floordiv__(self, x:'Int[Tag]') -> int:
+    def __floordiv__(self, x:Self) -> int:
         pass
     def __floordiv__(self, x):
         if isinstance(x,int):
             return self.__class__(self.value()//x)
         elif isinstance(x,float):
             return self.value()//x
         else:
             return self.value()//x.value()
         pass
 
-    def __truediv__(self, x:Union[float,int,'Int[Tag]']) -> float:
+    def __truediv__(self, x:float|int|Self) -> float:
         if isinstance(x,float) or isinstance(x,int):
             return self.value()/x
         else:
             return self.value()/x.value()
         pass
     
     @overload
-    def __mul__(self, x:int) -> 'Int[Tag]':
+    def __mul__(self, x:int) -> Self:
         pass
     @overload
     def __mul__(self, x:Any):  # -> NotImplemented:
         pass
     def __mul__(self, x):
         if isinstance(x,int):
             return self.__class__(self.value()*x)
         else:
             return NotImplemented
         pass
 
     @overload
-    def __rmul__(self, x:int):  # -> Int[Tag]
+    def __rmul__(self, x:int):  # -> Self:
         pass
     @overload
     def __rmul__(self, x:Any):  # -> NotImplemented
         pass
     def __rmul__(self, x):
         if isinstance(x,int):
             return self.__class__(x*self.value())
         else:
             return NotImplemented
         pass
 
     @overload
-    def __mod__(self, other:int):  #->Int[Tag]
+    def __mod__(self, other:int)->Self:
         pass
     @overload
     def __mod__(self, other:float)->float:
         pass
     @overload
-    def __mod__(self, other:'Int[Tag]')->int:
+    def __mod__(self, other:Self)->int:
         pass
     def __mod__(self, other):
         if type(other) is int:
             return self.__class__(self.value()%other)
         if type(other) is float:
             return self.value()%other
         else:
             return self.value()%other.value()
 
-    def __round__(self, ndigits:int=0):  #->Int[Tag]
+    def __round__(self, ndigits:int=0)->Self:
         return self.__class__(self.value().__round__(ndigits))
 
     
-    def __abs__(self): # -> 'Int[Tag]':
+    def __abs__(self) -> Self:
         return self.__class__(self.value().__abs__())
-    def __invert__(self): # -> 'Int[Tag]':
+    def __invert__(self) -> Self:
         return self.__class__(self.value().__invert__())
-    def __neg__(self): # -> 'Int[Tag]':
+    def __neg__(self) -> Self:
         return self.__class__(self.value().__neg__())
-    def __pos__(self): # -> 'Int[Tag]':
+    def __pos__(self) -> Self:
         return self.__class__(self.value().__pos__())
     def __int__(self)->int:
         return self.value().__int__()
     def __sizeof__(self)->int:
         return self.value().__sizeof__()
     def bit_count(self)->int:
         return self.value().bit_count()
@@ -193,71 +190,68 @@
         return self.value().bit_length()
     def __index__(self)->int:
         return self.value().__index__()
     def __hash__(self)->int:
         return self.value().__hash__()
     def __bool__(self)->bool:
         return self.value().__bool__()
-    def __ror__(self,n:int): # -> 'Int[Tag]':
+    def __ror__(self,n:int) -> Self:
         return self.__class__(self.value().__ror__(n))
-    def __rrshift__(self,n:int): # -> 'Int[Tag]':
+    def __rrshift__(self,n:int) -> Self:
         return self.__class__(self.value().__rrshift__(n))
-    def __lshift__(self,n:int): # -> 'Int[Tag]':
+    def __lshift__(self,n:int) -> Self:
         return self.__class__(self.value().__lshift__(n))
-    def __rlshift__(self,n:int): # -> 'Int[Tag]':
+    def __rlshift__(self,n:int) -> Self:
         return self.__class__(self.value().__rlshift__(n))
-    def __rshift__(self,n:int): # -> 'Int[Tag]':
+    def __rshift__(self,n:int) -> Self:
         return self.__class__(self.value().__rshift__(n))
-    def __gt__(self,other:'Int[Tag]')->bool:
+    def __gt__(self,other:Self)->bool:
         return self.value().__gt__(other.value())
-    def __lt__(self,other:'Int[Tag]')->bool:
+    def __lt__(self,other:Self)->bool:
         return self.value().__lt__(other.value())
-    def __le__(self,other:'Int[Tag]')->bool:
+    def __le__(self,other:Self)->bool:
         return self.value().__le__(other.value())
-    def __ge__(self,other:'Int[Tag]')->bool:
+    def __ge__(self,other:Self)->bool:
         return self.value().__ge__(other.value())
-    def __add__(self,other:'Int[Tag]'): # -> 'Int[Tag]':
+    def __add__(self,other:Self)->Self:
         if type(other) is not type(self):
             return NotImplemented
         return self.__class__(self.value().__add__(other.value()))
-    def __sub__(self,other:'Int[Tag]'): # -> 'Int[Tag]':
+    def __sub__(self,other:Self)->Self:
         if type(other) is not type(self):
             return NotImplemented
         return self.__class__(self.value().__sub__(other.value()))
-    def __and__(self,other:'Int[Tag]'): # -> 'Int[Tag]':
+    def __and__(self,other:Self)->Self:
         if type(other) is not type(self):
             return NotImplemented
         return self.__class__(self.value().__and__(other.value()))
-    def __or__(self,other:'Int[Tag]'): # -> 'Int[Tag]':
+    def __or__(self,other:Self)->Self:
         if type(other) is not type(self):
             return NotImplemented
         return self.__class__(self.value().__or__(other.value()))
-    def __xor__(self,other:'Int[Tag]'): # -> 'Int[Tag]':
+    def __xor__(self,other:Self)->Self:
         if type(other) is not type(self):
             return NotImplemented
         return self.__class__(self.value().__xor__(other.value()))
     def as_integer_ratio(self)->Tuple[int,int]:
         return self.value().as_integer_ratio()
 
     pass
 
 
-class Float_(Generic[Tag]):
+class Float(Generic[Tag]):
     __value:float
 
     def __init__(self, value:float):
         self.__value=value
         pass
 
     def value(self)->float:
         return self.__value
 
-    pass
-
-class Float(Generic[Tag],Float_[Tag],SupportsRound):
     def __eq__(self,other)->bool:
         '''equality test, only valid for two object of exactly the same class; except
            that python insists on supporting __eq__ for objects of any type, so this
            function's signature allows it and calls out all nonsense at runtime'''
         '''i.e. recommend stick to using Float[X] like:
               class Timestamp(Float[TimestampTag]):pass
            ... and not inherit from Timestamp.
@@ -285,149 +279,147 @@
     def hex(self)->str:
         return self.value().hex()
     
     def conjugate(self):
         return self.value().conjugate()
 
     @overload
-    def __divmod__(self, x:int) -> Tuple:  # Tuple[Self,Self]
+    def __divmod__(self, x:int) -> Tuple[Self,Self]:
         pass
     @overload
-    def __divmod__(self, x:float) -> Tuple:  # Tuple[Self,Self]
+    def __divmod__(self, x:float) -> Tuple[Self,Self]:
         pass
     @overload
-    def __divmod__(self, x:Float_[Tag]) -> Tuple:  # Tuple[float,float]
+    def __divmod__(self, x:Self) -> Tuple[float,float]:
         pass
     def __divmod__(self, x):
         if isinstance(x,int) or isinstance(x,float):
             q,r=self.value().__divmod__(x)
             return self.__class__(q),self.__class__(r)
         else:
             return divmod(self.value(),x.value())
         pass
 
     @overload
-    def __floordiv__(self, x:int):  # -> Float[Tag]
+    def __floordiv__(self, x:int) -> Self:
         pass
     @overload
-    def __floordiv__(self, x:float):  # -> Float[Tag]
+    def __floordiv__(self, x:float) -> Self:
         pass
     @overload
-    def __floordiv__(self, x:Float_[Tag]) -> float:
+    def __floordiv__(self, x:Self) -> float:
         pass
     def __floordiv__(self, x):
         if isinstance(x,int) or isinstance(x,float):
             return self.__class__(self.value()//x)
         else:
             return self.value()//x.value()
         pass
 
     @overload
-    def __truediv__(self, x:Union[float,int]): # -> Float[Tag]
+    def __truediv__(self, x:Union[float,int]) -> Self:
         pass
     @overload
-    def __truediv__(self, x:Float_[Tag]) -> float:
+    def __truediv__(self, x:Self) -> float:
         pass
     def __truediv__(self, x):
         if isinstance(x,int) or isinstance(x,float):
             return self.__class__(self.value()/x)
         else:
             return self.value()/x.value()
         pass
     
     @overload
-    def __mul__(self, x:int):  # -> Float[Tag]
+    def __mul__(self, x:int) -> Self:
         pass
     @overload
-    def __mul__(self, x:float):  # -> Float[Tag]
+    def __mul__(self, x:float) -> Self:
         pass
     def __mul__(self, x):
         return self.__class__(self.value()*x)
 
     @overload
-    def __rmul__(self, x:int):  # -> Float[Tag]
+    def __rmul__(self, x:int) -> Self:
         pass
     @overload
-    def __rmul__(self, x:float):  # -> Float[Tag]
+    def __rmul__(self, x:float) -> Self:
         pass
     def __rmul__(self, x):
         return self.__class__(x*self.value())
 
     @overload
-    def __mod__(self, other:int):  #->Float[Tag]
+    def __mod__(self, other:int)->Self:
         pass
     @overload
-    def __mod__(self, other:float):  #->Float[Tag]
+    def __mod__(self, other:float)->Self:
         pass
     @overload
-    def __mod__(self, other:Float_[Tag])->float:
+    def __mod__(self, other:Self)->float:
         pass
     def __mod__(self, other):
         if isinstance(other,int) or isinstance(other,float):
             return self.__class__(self.value()%other)
         else:
             return self.value()%other.value()
 
-    def __round__(self, ndigits:int=0):  #->Float[Tag]
+    def __round__(self, ndigits:int=0)->Self:
         return self.__class__(self.value().__round__(ndigits))
 
     
-    def __abs__(self):
+    def __abs__(self)->Self:
         return self.__class__(self.value().__abs__())
-    def __neg__(self):
+    def __neg__(self)->Self:
         return self.__class__(self.value().__neg__())
-    def __pos__(self):
+    def __pos__(self)->Self:
         return self.__class__(self.value().__pos__())
-    def __trunc__(self):
+    def __trunc__(self)->Self:
         return self.__class__(self.value().__trunc__())
-    def __ceil__(self):
+    def __ceil__(self)->Self:
         return self.__class__(self.value().__ceil__())
-    def __floor__(self):
+    def __floor__(self)->Self:
         return self.__class__(self.value().__floor__())
     def __sizeof__(self)->int:
         return self.value().__sizeof__()
     def __hash__(self)->int:
         return self.value().__hash__()
     def __bool__(self)->bool:
         return float(self.value()).__bool__()
     def is_integer(self)->bool:
         return float(self.value()).is_integer()
-    def __gt__(self,other:Float_[Tag])->bool:
+    def __gt__(self,other:Self)->bool:
         return self.value().__gt__(other.value())
-    def __lt__(self,other:Float_[Tag])->bool:
+    def __lt__(self,other:Self)->bool:
         return self.value().__lt__(other.value())
-    def __le__(self,other:Float_[Tag])->bool:
+    def __le__(self,other:Self)->bool:
         return self.value().__le__(other.value())
-    def __ge__(self,other:Float_[Tag])->bool:
+    def __ge__(self,other:Self)->bool:
         return self.value().__ge__(other.value())
-    def __add__(self,other:Float_[Tag]):
+    def __add__(self,other:Self)->Self:
         if type(other) is not type(self):
             return NotImplemented
         return self.__class__(self.value().__add__(other.value()))
-    def __sub__(self,other:Float_[Tag]):
+    def __sub__(self,other:Self)->Self:
         if type(other) is not type(self):
             return NotImplemented
         return self.__class__(self.value().__sub__(other.value()))
     def as_integer_ratio(self)->Tuple[float,float]:
         return self.value().as_integer_ratio()
 
     pass
 
 
-class Str_(Generic[Tag]):
+class Str(Generic[Tag]):
     __value:str
     def __init__(self, value:str):
         self.__value=value
         pass
 
     def value(self)->str:
         return self.__value
-    pass
 
-class Str(Generic[Tag],Str_[Tag]):
     def __eq__(self,other)->bool:
         '''equality test ignores possible subclass relationships, i.e. only valid
            for two object of exactly the same class; except that python insists
            supporting __eq__ for objects of any type, so this functions allows
            comparing any Str[X] with anything but calls out nonsense at runtime'''
         '''i.e. recommend stick to using Str[X] like:
               class FirstName(Str[FirstNameTag]):pass
@@ -452,41 +444,41 @@
 
     def encode(self,encoding:str='utf-8', errors:str='strict')->bytes:
         return self.value().encode()
 
     def __contains__(self,other:str)->bool:
         return self.value().__contains__(other)
 
-    def zfill(self,width:int):
+    def zfill(self,width:int)->Self:
         return self.__class__(self.value().zfill(width))
 
     def format_map(self,mapping:Mapping):
         return self.__class__(self.value().format_map(mapping))
 
     def format(self,*args,**kwargs):
         return self.__class__(self.value().format(*args,**kwargs))
     
-    def expandtabs(self,tabsize=8):
+    def expandtabs(self,tabsize=8)->Self:
         return self.__class__(self.value().expandtabs(tabsize))
 
     def __getitem__(self,key):
         return self.value().__getitem__(key)
 
     
-    def capitalize(self):
+    def capitalize(self)->Self:
         return self.__class__(self.value().capitalize())
-    def lower(self):
+    def lower(self)->Self:
         return self.__class__(self.value().lower())
-    def swapcase(self):
+    def swapcase(self)->Self:
         return self.__class__(self.value().swapcase())
-    def title(self):
+    def title(self)->Self:
         return self.__class__(self.value().title())
-    def casefold(self):
+    def casefold(self)->Self:
         return self.__class__(self.value().casefold())
-    def upper(self):
+    def upper(self)->Self:
         return self.__class__(self.value().upper())
     def __len__(self)->int:
         return self.value().__len__()
     def __sizeof__(self)->int:
         return self.value().__sizeof__()
     def __hash__(self)->int:
         return self.value().__hash__()
@@ -510,25 +502,25 @@
         return self.value().isupper()
     def isalpha(self)->bool:
         return self.value().isalpha()
     def isdigit(self)->bool:
         return self.value().isdigit()
     def istitle(self)->bool:
         return self.value().istitle()
-    def __mul__(self,n:int):
+    def __mul__(self,n:int)->Self:
         return self.__class__(self.value().__mul__(n))
-    def __gt__(self,other:Str_[Tag])->bool:
+    def __gt__(self,other:Self)->bool:
         return self.value().__gt__(other.value())
-    def __lt__(self,other:Str_[Tag])->bool:
+    def __lt__(self,other:Self)->bool:
         return self.value().__lt__(other.value())
-    def __le__(self,other:Str_[Tag])->bool:
+    def __le__(self,other:Self)->bool:
         return self.value().__le__(other.value())
-    def __ge__(self,other:Str_[Tag])->bool:
+    def __ge__(self,other:Self)->bool:
         return self.value().__ge__(other.value())
-    def __add__(self,other:Str_[Tag]):
+    def __add__(self,other:Self)->Self:
         if type(other) is not type(self):
             return NotImplemented
         return self.__class__(self.value().__add__(other.value()))
     @overload
     def rfind(self, sub:str) -> int:
         pass
     @overload
@@ -612,36 +604,36 @@
     def startswith(self, s:str, start:int)->bool:
         pass
     @overload
     def startswith(self, s:str, start:int, end:int)->bool:
         pass
     def startswith(self, s, *args):
         return self.value().startswith(s,*args)
-    def strip(self, chars:Optional[str]=None):
+    def strip(self, chars:Optional[str]=None)->Self:
         return self.__class__(self.value().strip(chars))
-    def lstrip(self, chars:Optional[str]=None):
+    def lstrip(self, chars:Optional[str]=None)->Self:
         return self.__class__(self.value().lstrip(chars))
-    def rstrip(self, chars:Optional[str]=None):
+    def rstrip(self, chars:Optional[str]=None)->Self:
         return self.__class__(self.value().rstrip(chars))
-    def replace(self, old:str, new:str, count=-1):
+    def replace(self, old:str, new:str, count=-1)->Self:
         return self.__class__(self.value().replace(old,new,count))
     def split(self, sep:Optional[str]=None, max_split=-1)->List[str]:
         return self.value().split(sep,max_split)
     def rsplit(self, sep:Optional[str]=None, max_split=-1)->List[str]:
         return self.value().rsplit(sep,max_split)
     def partition(self,sep:str) -> Tuple[str,str,str]:
         return self.value().partition(sep)
     def rpartition(self,sep:str) -> Tuple[str,str,str]:
         return self.value().rpartition(sep)
-    def removeprefix(self,sub:str):
+    def removeprefix(self,sub:str)->Self:
         return self.__class__(self.value().removeprefix(sub))
-    def removesuffix(self,sub:str):
+    def removesuffix(self,sub:str)->Self:
         return self.__class__(self.value().removesuffix(sub))
-    def center(self,width:int,fillchar:str=' '):
+    def center(self,width:int,fillchar:str=' ')->Self:
         return self.__class__(self.value().center(width,fillchar))
-    def ljust(self,width:int,fillchar:str=' '):
+    def ljust(self,width:int,fillchar:str=' ')->Self:
         return self.__class__(self.value().ljust(width,fillchar))
-    def rjust(self,width:int,fillchar:str=' '):
+    def rjust(self,width:int,fillchar:str=' ')->Self:
         return self.__class__(self.value().rjust(width,fillchar))
 
     pass
```

### Comparing `xju-1.2.8/src/xju/newtype.py.test` & `xju-1.2.9/src/xju/newtype.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/patch.py` & `xju-1.2.9/src/xju/patch.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/patch.py.test` & `xju-1.2.9/src/xju/patch.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/pq.py.test` & `xju-1.2.9/src/xju/pq.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/rfc2616.py` & `xju-1.2.9/src/xju/rfc2616.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/rfc2616.py.test` & `xju-1.2.9/src/xju/rfc2616.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/time.py` & `xju-1.2.9/src/xju/time.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,30 +10,29 @@
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 #
 from xju.newtype import Int,Float,Union
-from typing import overload
+from typing import overload, Self
 import time
 
 class HoursTag:pass
 class MinutesTag:pass
 class SecondsTag:pass
 
 class Hours(Int[HoursTag]): pass
 class Minutes(Int[MinutesTag]): pass
 class Seconds(Int[SecondsTag]): pass
 
 class DurationTag:pass
 class Duration(Float[DurationTag]):pass
 
-class TimestampBase:pass  # until typing.Self
-class Timestamp(TimestampBase):
+class Timestamp():
     __value:float
     def __init__(self,value:float):
         self.__value=float(value)
         pass
     def value(self):
         return self.__value
     def __str__(self):
@@ -50,18 +49,18 @@
         if isinstance(x,Seconds):
             return Timestamp(self.value()+x.value())
         return Timestamp(self.value()+x.value())
     def __radd__(self, duration:Union[Duration,Hours,Minutes,Seconds]):
         return self.__add__(duration)
 
     @overload
-    def __sub__(self, t2:TimestampBase)->Duration:
+    def __sub__(self, t2:Self)->Duration:
         pass
     @overload
-    def __sub__(self, duration:Union[Duration,Hours,Minutes,Seconds]):  # -> Timestamp
+    def __sub__(self, duration:Union[Duration,Hours,Minutes,Seconds])->Self:
         pass
     def __sub__(self, x):
         if isinstance(x,Duration):
             return Timestamp(self.value()-x.value())
         if isinstance(x,Hours):
             return Timestamp(self.value()-x.value()*3600)
         if isinstance(x,Minutes):
```

### Comparing `xju-1.2.8/src/xju/time.py.test` & `xju-1.2.9/src/xju/time.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/xn.py` & `xju-1.2.9/src/xju/xn.py`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju/xn.py.test` & `xju-1.2.9/src/xju/xn.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.2.8/src/xju.egg-info/PKG-INFO` & `xju-1.2.9/src/xju.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xju
-Version: 1.2.8
+Version: 1.2.9
 Summary: xju library
 Author: Trevor Taylor
 License: Copyright © 2022 Trevor Taylor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -25,14 +25,16 @@
 Various modules implemented to some broad principles:
 
 * fine-grained static typing
 * pure context management
 * useful functionality that is hard to use incorrectly
 * 100% test coverage
 
+(see the bottom of this readme for release history)
+
 `xju.newtype <xju/newtype.py>`_ - static and dynamic distinct int, float and str types
 
 * unlike typing.NewType the new types are compatible with isinstance, so you
   can actually use them to do real stuff, like implement overloaded methods
 
 * see `xju/newtype.py.test <xju/newtype.py.test>`_ for sample code
 
@@ -130,14 +132,16 @@
 
 * designed to fit well with type checking
 
 * built in support for xju.newtype described above
 
 * generates json schema equivalent schemas for types
 
+* generates typescript code (types, type-guards and dynamic casts) equivalents
+
 * see `xju/json_codec.py.test <xju/json_codec.py.test>`_ for full sample code
 
 
 `xju.jsonschema <xju/jsonschema.py>`_
 
 * represents JSON schemas as straight-foward, easy-to-read python data structures, because life's too short for jsonschema.org
 
@@ -160,7 +164,16 @@
 
 `xju.xn <xju/xn.py>`_
 
 * Exception wrapping to provide human readable context gathering
 
 * see `xju/xn.py.test <xju/xn.py.test>`_ for sample code
 
+Release History
+
+- 1.2.9 xju.json_codec generates typescript equivalents
+- 1.2.9 xju.json_codec adds codec() convenience method
+- 1.2.9 xju.json_codec uses kw_args to construct classes
+
+- 1.2.8 xju.json_codec supports string type-hints (for foward definitions)
+- 1.2.8 xju.json_codec adds typing.Self support (for recursive types)
+- 1.2.8 xju.json_codec requires python 3.11, tested with mypy 1.1.1
```

### Comparing `xju-1.2.8/src/xju.egg-info/SOURCES.txt` & `xju-1.2.9/src/xju.egg-info/SOURCES.txt`

 * *Files identical despite different names*

