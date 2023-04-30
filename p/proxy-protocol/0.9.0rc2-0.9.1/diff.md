# Comparing `tmp/proxy-protocol-0.9.0rc2.tar.gz` & `tmp/proxy-protocol-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxy-protocol-0.9.0rc2.tar", last modified: Fri Nov  4 03:07:00 2022, max compression
+gzip compressed data, was "proxy-protocol-0.9.1.tar", last modified: Sun Feb 12 14:15:54 2023, max compression
```

## Comparing `proxy-protocol-0.9.0rc2.tar` & `proxy-protocol-0.9.1.tar`

### file list

```diff
@@ -1,53 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 03:07:00.125602 proxy-protocol-0.9.0rc2/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7323 2022-11-04 03:07:00.125602 proxy-protocol-0.9.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5453 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 03:07:00.125602 proxy-protocol-0.9.0rc2/proxy_protocol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7323 2022-11-04 03:07:00.000000 proxy-protocol-0.9.0rc2/proxy_protocol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-11-04 03:07:00.000000 proxy-protocol-0.9.0rc2/proxy_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 03:07:00.000000 proxy-protocol-0.9.0rc2/proxy_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-11-04 03:07:00.000000 proxy-protocol-0.9.0rc2/proxy_protocol.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-04 03:07:00.000000 proxy-protocol-0.9.0rc2/proxy_protocol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-04 03:07:00.000000 proxy-protocol-0.9.0rc2/proxy_protocol.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 03:07:00.125602 proxy-protocol-0.9.0rc2/proxyprotocol/
--rw-r--r--   0 runner    (1001) docker     (121)     4253 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4102 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/build.py
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/checksum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/detect.py
--rw-r--r--   0 runner    (1001) docker     (121)     4556 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/dnsbl.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/noop.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    10988 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/result.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 03:07:00.125602 proxy-protocol-0.9.0rc2/proxyprotocol/server/
--rw-r--r--   0 runner    (1001) docker     (121)     3016 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2550 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/server/echo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2830 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/server/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     7190 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/server/protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)    11722 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/sock.py
--rw-r--r--   0 runner    (1001) docker     (121)    18314 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/tlv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3606 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     8229 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/v2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/proxyprotocol/version.py
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-04 03:07:00.125602 proxy-protocol-0.9.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 03:07:00.125602 proxy-protocol-0.9.0rc2/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/tasks/check.py
--rw-r--r--   0 runner    (1001) docker     (121)      753 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/tasks/doc.py
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/tasks/lint.py
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/tasks/test.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/tasks/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 03:07:00.125602 proxy-protocol-0.9.0rc2/test/
--rw-r--r--   0 runner    (1001) docker     (121)     4074 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (121)     3228 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/test/test_detect.py
--rw-r--r--   0 runner    (1001) docker     (121)     3787 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/test/test_dnsbl.py
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/test/test_noop.py
--rw-r--r--   0 runner    (1001) docker     (121)     4880 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/test/test_result.py
--rw-r--r--   0 runner    (1001) docker     (121)    10578 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/test/test_sock.py
--rw-r--r--   0 runner    (1001) docker     (121)     9751 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/test/test_tlv.py
--rw-r--r--   0 runner    (1001) docker     (121)     4722 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/test/test_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)    10192 2022-11-04 03:06:44.000000 proxy-protocol-0.9.0rc2/test/test_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:15:54.646860 proxy-protocol-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-02-12 14:15:54.642859 proxy-protocol-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:15:54.638859 proxy-protocol-0.9.1/proxy_protocol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-02-12 14:15:54.000000 proxy-protocol-0.9.1/proxy_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-02-12 14:15:54.000000 proxy-protocol-0.9.1/proxy_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 14:15:54.000000 proxy-protocol-0.9.1/proxy_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-12 14:15:54.000000 proxy-protocol-0.9.1/proxy_protocol.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-12 14:15:54.000000 proxy-protocol-0.9.1/proxy_protocol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-12 14:15:54.000000 proxy-protocol-0.9.1/proxy_protocol.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:15:54.642859 proxy-protocol-0.9.1/proxyprotocol/
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/dnsbl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:15:54.642859 proxy-protocol-0.9.1/proxyprotocol/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/server/echo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/server/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/server/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/sock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18314 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/tlv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/proxyprotocol/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-12 14:15:54.646860 proxy-protocol-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 14:15:54.642859 proxy-protocol-0.9.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/test/test_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/test/test_dnsbl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/test/test_noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/test/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/test/test_sock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/test/test_tlv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/test/test_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-02-12 14:15:40.000000 proxy-protocol-0.9.1/test/test_v2.py
```

### Comparing `proxy-protocol-0.9.0rc2/LICENSE.md` & `proxy-protocol-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/PKG-INFO` & `proxy-protocol-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxy-protocol
-Version: 0.9.0rc2
+Version: 0.9.1
 Summary: PROXY protocol library with asyncio server implementation
 Home-page: https://github.com/icgood/proxy-protocol/
 Author: Ian Good
 Author-email: ian@icgood.net
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `proxy-protocol-0.9.0rc2/README.md` & `proxy-protocol-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/proxy_protocol.egg-info/PKG-INFO` & `proxy-protocol-0.9.1/proxy_protocol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxy-protocol
-Version: 0.9.0rc2
+Version: 0.9.1
 Summary: PROXY protocol library with asyncio server implementation
 Home-page: https://github.com/icgood/proxy-protocol/
 Author: Ian Good
 Author-email: ian@icgood.net
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `proxy-protocol-0.9.0rc2/proxy_protocol.egg-info/SOURCES.txt` & `proxy-protocol-0.9.1/proxy_protocol.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -24,20 +24,14 @@
 proxyprotocol/v1.py
 proxyprotocol/v2.py
 proxyprotocol/version.py
 proxyprotocol/server/__init__.py
 proxyprotocol/server/echo.py
 proxyprotocol/server/main.py
 proxyprotocol/server/protocol.py
-tasks/__init__.py
-tasks/check.py
-tasks/doc.py
-tasks/lint.py
-tasks/test.py
-tasks/types.py
 test/test_build.py
 test/test_detect.py
 test/test_dnsbl.py
 test/test_noop.py
 test/test_result.py
 test/test_sock.py
 test/test_tlv.py
```

### Comparing `proxy-protocol-0.9.0rc2/proxyprotocol/__init__.py` & `proxy-protocol-0.9.1/proxyprotocol/__init__.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/proxyprotocol/build.py` & `proxy-protocol-0.9.1/proxyprotocol/build.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/proxyprotocol/checksum.py` & `proxy-protocol-0.9.1/proxyprotocol/checksum.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/proxyprotocol/detect.py` & `proxy-protocol-0.9.1/proxyprotocol/detect.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/proxyprotocol/dnsbl.py` & `proxy-protocol-0.9.1/proxyprotocol/dnsbl.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/proxyprotocol/noop.py` & `proxy-protocol-0.9.1/proxyprotocol/noop.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/proxyprotocol/reader.py` & `proxy-protocol-0.9.1/proxyprotocol/reader.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/proxyprotocol/result.py` & `proxy-protocol-0.9.1/proxyprotocol/result.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/proxyprotocol/server/__init__.py` & `proxy-protocol-0.9.1/proxyprotocol/server/__init__.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/proxyprotocol/server/echo.py` & `proxy-protocol-0.9.1/proxyprotocol/server/echo.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/proxyprotocol/server/main.py` & `proxy-protocol-0.9.1/proxyprotocol/server/main.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/proxyprotocol/server/protocol.py` & `proxy-protocol-0.9.1/proxyprotocol/server/protocol.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,35 +103,39 @@
     @abstractmethod
     def proxy_data(self, data: bytes) -> None:
         ...
 
 
 class DownstreamProtocol(_Base):
 
-    __slots__ = ['loop', 'dnsbl', 'upstream', 'id', '_dnsbl_task', '_waiting',
-                 '_waiting_closed', '_upstream', '_upstream_factory']
+    __slots__ = ['loop', 'dnsbl', 'upstream', 'id', '_waiting',
+                 '_waiting_closed', '_upstream', '_upstream_factory',
+                 '_dnsbl_task', '_connect_task']
 
     def __init__(self, upstream_protocol: Type[UpstreamProtocol],
                  loop: AbstractEventLoop, buf_len: int, dnsbl: Dnsbl,
                  upstream: Address) -> None:
         super().__init__(buf_len)
         self.loop: Final = loop
         self.dnsbl: Final = dnsbl
         self.upstream: Final = upstream
         self.id: Final = uuid4().bytes
         self._dnsbl_task: Optional[Task[Optional[str]]] = None
+        self._connect_task: Optional[Task[_Connect]] = None
         self._waiting: Deque[bytes] = deque()
         self._waiting_closed = False
         self._upstream: Optional[UpstreamProtocol] = None
         self._upstream_factory = partial(upstream_protocol, self, buf_len,
                                          upstream.pp)
 
     def _set_client(self, result: ProxyResult,
                     connect_task: Task[_Connect]) -> None:
         dnsbl_task = self._dnsbl_task
+        self._dnsbl_task = None
+        self._connect_task = None
         assert dnsbl_task is not None
         try:
             _, upstream = connect_task.result()
         except OSError:
             self.close()
             dnsbl_task.cancel()
             _log.exception('[%s] Connection failed: %s',
@@ -153,15 +157,15 @@
 
     def connection_made(self, transport: BaseTransport) -> None:
         super().connection_made(transport)
         _log.info('[%s] Downstream connection received: %s',
                   self.id.hex(), self.sock_info)
         loop = self.loop
         self._dnsbl_task = loop.create_task(self.dnsbl.lookup(self.sock_info))
-        connect_task = loop.create_task(
+        self._connect_task = connect_task = loop.create_task(
             loop.create_connection(self._upstream_factory,
                                    self.upstream.host, self.upstream.port or 0,
                                    ssl=self.upstream.ssl))
         result = build_transport_result(transport, unique_id=self.id)
         connect_task.add_done_callback(partial(self._set_client, result))
 
     def connection_lost(self, exc: Optional[Exception]) -> None:
```

### Comparing `proxy-protocol-0.9.0rc2/proxyprotocol/sock.py` & `proxy-protocol-0.9.1/proxyprotocol/sock.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/proxyprotocol/tlv.py` & `proxy-protocol-0.9.1/proxyprotocol/tlv.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/proxyprotocol/typing.py` & `proxy-protocol-0.9.1/proxyprotocol/typing.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/proxyprotocol/v1.py` & `proxy-protocol-0.9.1/proxyprotocol/v1.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/proxyprotocol/v2.py` & `proxy-protocol-0.9.1/proxyprotocol/v2.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/proxyprotocol/version.py` & `proxy-protocol-0.9.1/proxyprotocol/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from __future__ import annotations
 
 from enum import Enum
-from typing import cast, Optional
+from typing import Optional
 
 from . import ProxyProtocol
 from .detect import ProxyProtocolDetect
 from .noop import ProxyProtocolNoop
 from .v1 import ProxyProtocolV1
 from .v2 import ProxyProtocolV2
 
@@ -40,8 +40,10 @@
 
         Raises:
             :exc:`KeyError`
 
         """
         if not name:
             return cls.NOOP.value
-        return cast(ProxyProtocol, cls[name.upper()].value)
+        pp = cls[name.upper()].value
+        assert isinstance(pp, ProxyProtocol)
+        return pp
```

### Comparing `proxy-protocol-0.9.0rc2/setup.py` & `proxy-protocol-0.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021 Ian C. Good
+# Copyright (c) 2023 Ian C. Good
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -24,15 +24,15 @@
 with open('README.md') as f:
     readme = f.read()
 
 with open('LICENSE.md') as f:
     license = f.read()
 
 setup(name='proxy-protocol',
-      version='0.9.0.rc2',
+      version='0.9.1',
       author='Ian Good',
       author_email='ian@icgood.net',
       description='PROXY protocol library with asyncio server implementation',
       long_description=readme + license,
       long_description_content_type='text/markdown',
       license='MIT',
       url='https://github.com/icgood/proxy-protocol/',
```

### Comparing `proxy-protocol-0.9.0rc2/test/test_build.py` & `proxy-protocol-0.9.1/test/test_build.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/test/test_detect.py` & `proxy-protocol-0.9.1/test/test_detect.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/test/test_dnsbl.py` & `proxy-protocol-0.9.1/test/test_dnsbl.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/test/test_noop.py` & `proxy-protocol-0.9.1/test/test_noop.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/test/test_result.py` & `proxy-protocol-0.9.1/test/test_result.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/test/test_sock.py` & `proxy-protocol-0.9.1/test/test_sock.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/test/test_tlv.py` & `proxy-protocol-0.9.1/test/test_tlv.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/test/test_v1.py` & `proxy-protocol-0.9.1/test/test_v1.py`

 * *Files identical despite different names*

### Comparing `proxy-protocol-0.9.0rc2/test/test_v2.py` & `proxy-protocol-0.9.1/test/test_v2.py`

 * *Files identical despite different names*

