# Comparing `tmp/vtece4564-websockets-11.0.2.post2.tar.gz` & `tmp/vtece4564-websockets-11.0.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtece4564-websockets-11.0.2.post2.tar", last modified: Sat Apr 29 14:57:54 2023, max compression
+gzip compressed data, was "vtece4564-websockets-11.0.2.post3.tar", last modified: Sun Apr 30 18:58:05 2023, max compression
```

## Comparing `vtece4564-websockets-11.0.2.post2.tar` & `vtece4564-websockets-11.0.2.post3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:54.839581 vtece4564-websockets-11.0.2.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-29 14:57:54.839581 vtece4564-websockets-11.0.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 14:57:54.839581 vtece4564-websockets-11.0.2.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:54.827581 vtece4564-websockets-11.0.2.post2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:54.831581 vtece4564-websockets-11.0.2.post2/src/vtece4564_websockets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-29 14:57:54.000000 vtece4564-websockets-11.0.2.post2/src/vtece4564_websockets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-29 14:57:54.000000 vtece4564-websockets-11.0.2.post2/src/vtece4564_websockets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 14:57:54.000000 vtece4564-websockets-11.0.2.post2/src/vtece4564_websockets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 14:57:54.000000 vtece4564-websockets-11.0.2.post2/src/vtece4564_websockets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:54.835581 vtece4564-websockets-11.0.2.post2/src/websockets/
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:54.835581 vtece4564-websockets-11.0.2.post2/src/websockets/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/extensions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24782 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/extensions/permessage_deflate.py
--rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    12565 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/http11.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:54.835581 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/async_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    26123 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/framing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/handshake.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    62936 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    44803 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    23822 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20857 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/speedups.c
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:54.839581 vtece4564-websockets-11.0.2.post2/src/websockets/sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/sync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29303 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/sync/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/sync/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    18290 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/sync/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/sync/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:58:05.677100 vtece4564-websockets-11.0.2.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-30 18:58:05.677100 vtece4564-websockets-11.0.2.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 18:58:05.677100 vtece4564-websockets-11.0.2.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:58:05.669100 vtece4564-websockets-11.0.2.post3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:58:05.673100 vtece4564-websockets-11.0.2.post3/src/vtece4564_websockets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-30 18:58:05.000000 vtece4564-websockets-11.0.2.post3/src/vtece4564_websockets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-30 18:58:05.000000 vtece4564-websockets-11.0.2.post3/src/vtece4564_websockets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:58:05.000000 vtece4564-websockets-11.0.2.post3/src/vtece4564_websockets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 18:58:05.000000 vtece4564-websockets-11.0.2.post3/src/vtece4564_websockets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:58:05.673100 vtece4564-websockets-11.0.2.post3/src/websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:58:05.673100 vtece4564-websockets-11.0.2.post3/src/websockets/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/extensions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24782 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/extensions/permessage_deflate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12565 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/http11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:58:05.673100 vtece4564-websockets-11.0.2.post3/src/websockets/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/legacy/async_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/legacy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26123 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/legacy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/legacy/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/legacy/framing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/legacy/handshake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/legacy/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62936 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/legacy/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44803 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/legacy/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23822 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20857 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/speedups.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:58:05.677100 vtece4564-websockets-11.0.2.post3/src/websockets/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/sync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29303 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/sync/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/sync/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/sync/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/sync/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-30 18:58:04.000000 vtece4564-websockets-11.0.2.post3/src/websockets/version.py
```

### Comparing `vtece4564-websockets-11.0.2.post2/LICENSE` & `vtece4564-websockets-11.0.2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/PKG-INFO` & `vtece4564-websockets-11.0.2.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtece4564-websockets
-Version: 11.0.2.post2
+Version: 11.0.2.post3
 Summary: An implementation of the WebSocket Protocol (RFC 6455 & 7692)
 Author-email: Aymeric Augustin <aymeric.augustin@m4x.org>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/ceharris/python-websockets
 Project-URL: Documentation, https://websockets.readthedocs.io/
 Keywords: WebSocket
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vtece4564-websockets-11.0.2.post2/README.rst` & `vtece4564-websockets-11.0.2.post3/README.rst`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/pyproject.toml` & `vtece4564-websockets-11.0.2.post3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 readme = "README.md"
-version = "11.0.2.post2"
+version = "11.0.2.post3"
 
 [project.urls]
 Homepage = "https://github.com/ceharris/python-websockets"
 #Changelog = "https://websockets.readthedocs.io/en/stable/project/changelog.html"
 Documentation = "https://websockets.readthedocs.io/"
 #Funding = "https://tidelift.com/subscription/pkg/pypi-websockets?utm_source=pypi-websockets&utm_medium=referral&utm_campaign=readme"
 #Tracker = "https://github.com/python-websockets/websockets/issues"
```

### Comparing `vtece4564-websockets-11.0.2.post2/setup.py` & `vtece4564-websockets-11.0.2.post3/setup.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/vtece4564_websockets.egg-info/PKG-INFO` & `vtece4564-websockets-11.0.2.post3/src/vtece4564_websockets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtece4564-websockets
-Version: 11.0.2.post2
+Version: 11.0.2.post3
 Summary: An implementation of the WebSocket Protocol (RFC 6455 & 7692)
 Author-email: Aymeric Augustin <aymeric.augustin@m4x.org>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/ceharris/python-websockets
 Project-URL: Documentation, https://websockets.readthedocs.io/
 Keywords: WebSocket
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vtece4564-websockets-11.0.2.post2/src/vtece4564_websockets.egg-info/SOURCES.txt` & `vtece4564-websockets-11.0.2.post3/src/vtece4564_websockets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/__init__.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/__main__.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/__main__.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/client.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/client.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/datastructures.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/datastructures.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/exceptions.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/exceptions.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/extensions/base.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/extensions/base.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/extensions/permessage_deflate.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/extensions/permessage_deflate.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/frames.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/frames.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/headers.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/headers.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/http.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/http.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/http11.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/http11.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/imports.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/imports.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/legacy/async_timeout.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/legacy/async_timeout.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/legacy/auth.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/legacy/auth.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/legacy/client.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/legacy/client.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/legacy/framing.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/legacy/framing.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/legacy/handshake.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/legacy/handshake.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/legacy/http.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/legacy/http.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/legacy/protocol.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/legacy/protocol.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/legacy/server.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/legacy/server.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/protocol.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/protocol.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/server.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/server.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/speedups.c` & `vtece4564-websockets-11.0.2.post3/src/websockets/speedups.c`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/streams.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/streams.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/sync/client.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/sync/client.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/sync/connection.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/sync/connection.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/sync/messages.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/sync/messages.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/sync/server.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/sync/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import http
 import logging
+import os
 import selectors
 import socket
 import ssl
+import sys
 import threading
 from types import TracebackType
 from typing import Any, Callable, Optional, Sequence, Type
 
 from ..extensions.base import ServerExtensionFactory
 from ..extensions.permessage_deflate import enable_server_permessage_deflate
 from ..headers import validate_subprotocols
@@ -194,14 +196,16 @@
         logger: Optional[LoggerLike] = None,
     ):
         self.socket = socket
         self.handler = handler
         if logger is None:
             logger = logging.getLogger("websockets.server")
         self.logger = logger
+        if sys.platform != "win32":
+            self.shutdown_watcher, self.shutdown_notifier = os.pipe()
 
     def serve_forever(self) -> None:
         """
         See :meth:`socketserver.BaseServer.serve_forever`.
 
         This method doesn't return. Calling :meth:`shutdown` from another thread
         stops the server.
@@ -210,14 +214,16 @@
 
             with serve(...) as server:
                 server.serve_forever()
 
         """
         poller = selectors.DefaultSelector()
         poller.register(self.socket, selectors.EVENT_READ)
+        if sys.platform != "win32":
+            poller.register(self.shutdown_watcher, selectors.EVENT_READ)
 
         while True:
             poller.select()
             try:
                 # If the socket is closed, this will raise an exception and exit
                 # the loop. So we don't need to check the return value of select().
                 sock, addr = self.socket.accept()
@@ -228,14 +234,16 @@
 
     def shutdown(self) -> None:
         """
         See :meth:`socketserver.BaseServer.shutdown`.
 
         """
         self.socket.close()
+        if sys.platform != "win32":
+            os.write(self.shutdown_notifier, b"x")
 
     def fileno(self) -> int:
         """
         See :meth:`socketserver.BaseServer.fileno`.
 
         """
         return self.socket.fileno()
```

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/sync/utils.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/sync/utils.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/typing.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/typing.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/uri.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/uri.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/utils.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/utils.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post2/src/websockets/version.py` & `vtece4564-websockets-11.0.2.post3/src/websockets/version.py`

 * *Files identical despite different names*

