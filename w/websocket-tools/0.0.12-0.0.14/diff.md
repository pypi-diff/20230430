# Comparing `tmp/websocket-tools-0.0.12.tar.gz` & `tmp/websocket-tools-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "websocket-tools-0.0.12.tar", last modified: Wed Jan 25 21:25:56 2023, max compression
+gzip compressed data, was "websocket-tools-0.0.14.tar", last modified: Sun Apr 30 08:35:39 2023, max compression
```

## Comparing `websocket-tools-0.0.12.tar` & `websocket-tools-0.0.14.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 eversin    (501) staff       (20)        0 2023-01-25 21:25:56.775948 websocket-tools-0.0.12/
--rw-r--r--   0 eversin    (501) staff       (20)     1073 2023-01-24 14:47:29.000000 websocket-tools-0.0.12/LICENCE
--rw-r--r--   0 eversin    (501) staff       (20)      687 2023-01-25 21:25:56.775609 websocket-tools-0.0.12/PKG-INFO
--rw-r--r--   0 eversin    (501) staff       (20)      218 2023-01-25 14:50:04.000000 websocket-tools-0.0.12/README.md
--rw-r--r--   0 eversin    (501) staff       (20)      568 2023-01-24 17:59:28.000000 websocket-tools-0.0.12/pyproject.toml
--rw-r--r--   0 eversin    (501) staff       (20)       38 2023-01-25 21:25:56.776041 websocket-tools-0.0.12/setup.cfg
-drwxr-xr-x   0 eversin    (501) staff       (20)        0 2023-01-25 21:25:56.770755 websocket-tools-0.0.12/websocket_tools/
--rw-r--r--   0 eversin    (501) staff       (20)        0 2023-01-24 14:46:08.000000 websocket-tools-0.0.12/websocket_tools/__init__.py
--rw-r--r--   0 eversin    (501) staff       (20)      779 2023-01-24 14:58:31.000000 websocket-tools-0.0.12/websocket_tools/websocket_loop.py
-drwxr-xr-x   0 eversin    (501) staff       (20)        0 2023-01-25 21:25:56.775148 websocket-tools-0.0.12/websocket_tools.egg-info/
--rw-r--r--   0 eversin    (501) staff       (20)      687 2023-01-25 21:25:56.000000 websocket-tools-0.0.12/websocket_tools.egg-info/PKG-INFO
--rw-r--r--   0 eversin    (501) staff       (20)      250 2023-01-25 21:25:56.000000 websocket-tools-0.0.12/websocket_tools.egg-info/SOURCES.txt
--rw-r--r--   0 eversin    (501) staff       (20)        1 2023-01-25 21:25:56.000000 websocket-tools-0.0.12/websocket_tools.egg-info/dependency_links.txt
--rw-r--r--   0 eversin    (501) staff       (20)       16 2023-01-25 21:25:56.000000 websocket-tools-0.0.12/websocket_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:35:39.462972 websocket-tools-0.0.14/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-30 08:35:28.000000 websocket-tools-0.0.14/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-30 08:35:39.462972 websocket-tools-0.0.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-30 08:35:28.000000 websocket-tools-0.0.14/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-30 08:35:28.000000 websocket-tools-0.0.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 08:35:39.462972 websocket-tools-0.0.14/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:35:39.458972 websocket-tools-0.0.14/websocket_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 08:35:28.000000 websocket-tools-0.0.14/websocket_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-30 08:35:28.000000 websocket-tools-0.0.14/websocket_tools/websocket_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:35:39.462972 websocket-tools-0.0.14/websocket_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-30 08:35:39.000000 websocket-tools-0.0.14/websocket_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-30 08:35:39.000000 websocket-tools-0.0.14/websocket_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 08:35:39.000000 websocket-tools-0.0.14/websocket_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 08:35:39.000000 websocket-tools-0.0.14/websocket_tools.egg-info/top_level.txt
```

### Comparing `websocket-tools-0.0.12/LICENCE` & `websocket-tools-0.0.14/LICENCE`

 * *Files identical despite different names*

### Comparing `websocket-tools-0.0.12/PKG-INFO` & `websocket-tools-0.0.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: websocket-tools
-Version: 0.0.12
+Version: 0.0.14
 Summary: A simple module to wrap web socket connection code.
 Author-email: sir even <sir_even@icloud.com>
 Project-URL: Homepage, https://github.com/sirEven/websocket-tools.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `websocket-tools-0.0.12/pyproject.toml` & `websocket-tools-0.0.14/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0", "websocket-client"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "websocket-tools"
-version = "0.0.12"
+version = "0.0.14"
 authors = [
   { name="sir even", email="sir_even@icloud.com"},
 ]
 description = "A simple module to wrap web socket connection code."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/sirEven/websocket-tools.git"
+"Homepage" = "https://github.com/sirEven/websocket-tools.git"
+
+[tool.mypy]
+ignore_missing_imports = true
```

### Comparing `websocket-tools-0.0.12/websocket_tools/websocket_loop.py` & `websocket-tools-0.0.14/websocket_tools/websocket_loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import websocket
 
+
 class WebsocketLoop:
     def __init__(
         self,
-        bot_id: str,
+        id: str,
         socket_host,
         on_open,
         on_message,
         on_error,
         on_close,
     ):
-        self.bot_id = bot_id
+        self.id = id
         self.socket_host = socket_host
         self.on_open = on_open
         self.on_message = on_message
         self.on_error = on_error
         self.on_close = on_close
         self.ws = None
 
@@ -26,8 +27,8 @@
             on_message=self.on_message,
             on_error=self.on_error,
             on_close=self.on_close,
         )
         self.ws.run_forever()
 
     def terminate(self):
-        self.ws.close()
+        self.ws.close()
```

### Comparing `websocket-tools-0.0.12/websocket_tools.egg-info/PKG-INFO` & `websocket-tools-0.0.14/websocket_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: websocket-tools
-Version: 0.0.12
+Version: 0.0.14
 Summary: A simple module to wrap web socket connection code.
 Author-email: sir even <sir_even@icloud.com>
 Project-URL: Homepage, https://github.com/sirEven/websocket-tools.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

