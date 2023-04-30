# Comparing `tmp/ipfsspec-0.3.0.tar.gz` & `tmp/ipfsspec-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfsspec-0.3.0.tar", last modified: Tue May 31 16:37:52 2022, max compression
+gzip compressed data, was "ipfsspec-0.4.0.tar", last modified: Sun Apr 30 09:50:18 2023, max compression
```

## Comparing `ipfsspec-0.3.0.tar` & `ipfsspec-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 16:37:52.946589 ipfsspec-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-05-31 16:37:40.000000 ipfsspec-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-05-31 16:37:40.000000 ipfsspec-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-05-31 16:37:52.946589 ipfsspec-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-05-31 16:37:40.000000 ipfsspec-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 16:37:52.946589 ipfsspec-0.3.0/ipfsspec/
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-05-31 16:37:40.000000 ipfsspec-0.3.0/ipfsspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-05-31 16:37:52.946589 ipfsspec-0.3.0/ipfsspec/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    11461 2022-05-31 16:37:40.000000 ipfsspec-0.3.0/ipfsspec/async_ipfs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8635 2022-05-31 16:37:40.000000 ipfsspec-0.3.0/ipfsspec/core.py
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-05-31 16:37:40.000000 ipfsspec-0.3.0/ipfsspec/tracing.py
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-05-31 16:37:40.000000 ipfsspec-0.3.0/ipfsspec/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 16:37:52.946589 ipfsspec-0.3.0/ipfsspec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-05-31 16:37:52.000000 ipfsspec-0.3.0/ipfsspec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-05-31 16:37:52.000000 ipfsspec-0.3.0/ipfsspec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-31 16:37:52.000000 ipfsspec-0.3.0/ipfsspec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-05-31 16:37:52.000000 ipfsspec-0.3.0/ipfsspec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-05-31 16:37:52.000000 ipfsspec-0.3.0/ipfsspec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-31 16:37:52.000000 ipfsspec-0.3.0/ipfsspec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-05-31 16:37:52.946589 ipfsspec-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-05-31 16:37:40.000000 ipfsspec-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 16:37:52.946589 ipfsspec-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)     3391 2022-05-31 16:37:40.000000 ipfsspec-0.3.0/test/test_async.py
--rw-r--r--   0 runner    (1001) docker     (121)     2647 2022-05-31 16:37:40.000000 ipfsspec-0.3.0/test/test_async_fallback.py
--rw-r--r--   0 runner    (1001) docker     (121)     4806 2022-05-31 16:37:40.000000 ipfsspec-0.3.0/test/test_gateway.py
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-05-31 16:37:40.000000 ipfsspec-0.3.0/test/test_ipfs.py
--rw-r--r--   0 runner    (1001) docker     (121)    70144 2022-05-31 16:37:40.000000 ipfsspec-0.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:50:18.952803 ipfsspec-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-30 09:50:09.000000 ipfsspec-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-30 09:50:09.000000 ipfsspec-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-30 09:50:18.952803 ipfsspec-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-30 09:50:09.000000 ipfsspec-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:50:18.952803 ipfsspec-0.4.0/ipfsspec/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-30 09:50:09.000000 ipfsspec-0.4.0/ipfsspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-30 09:50:18.952803 ipfsspec-0.4.0/ipfsspec/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11461 2023-04-30 09:50:09.000000 ipfsspec-0.4.0/ipfsspec/async_ipfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-04-30 09:50:09.000000 ipfsspec-0.4.0/ipfsspec/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-30 09:50:09.000000 ipfsspec-0.4.0/ipfsspec/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-30 09:50:09.000000 ipfsspec-0.4.0/ipfsspec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:50:18.948803 ipfsspec-0.4.0/ipfsspec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-30 09:50:18.000000 ipfsspec-0.4.0/ipfsspec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-30 09:50:18.000000 ipfsspec-0.4.0/ipfsspec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 09:50:18.000000 ipfsspec-0.4.0/ipfsspec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-30 09:50:18.000000 ipfsspec-0.4.0/ipfsspec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-30 09:50:18.000000 ipfsspec-0.4.0/ipfsspec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-30 09:50:18.000000 ipfsspec-0.4.0/ipfsspec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-30 09:50:18.952803 ipfsspec-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-30 09:50:09.000000 ipfsspec-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:50:18.952803 ipfsspec-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-30 09:50:09.000000 ipfsspec-0.4.0/test/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-30 09:50:09.000000 ipfsspec-0.4.0/test/test_async_fallback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-30 09:50:09.000000 ipfsspec-0.4.0/test/test_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-30 09:50:09.000000 ipfsspec-0.4.0/test/test_ipfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-04-30 09:50:09.000000 ipfsspec-0.4.0/versioneer.py
```

### Comparing `ipfsspec-0.3.0/LICENSE` & `ipfsspec-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfsspec-0.3.0/PKG-INFO` & `ipfsspec-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: ipfsspec
-Version: 0.3.0
+Version: 0.4.0
 Summary: readonly implementation of fsspec for IPFS
 Home-page: https://github.com/fsspec/ipfsspec
 Author: Tobias Kölling
 Author-email: tobias.koelling@physik.uni-muenchen.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -26,9 +24,7 @@
 with fsspec.open("ipfs://QmZ4tDuvesekSs4qM5ZBKpXiZGun7S2CYtEZRB3DYXkjGx", "r") as f:
     print(f.read())
 ```
 
 The current implementation uses a HTTP gateway to access the data. It tries to use a local one (which is expected to be found at `http://127.0.0.1:8080`) and falls back to `ipfs.io` if the local gateway is not available.
 
 You can modify the list of gateways using the space separated environment variable `IPFSSPEC_GATEWAYS`.
-
-
```

### Comparing `ipfsspec-0.3.0/README.md` & `ipfsspec-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ipfsspec-0.3.0/ipfsspec/async_ipfs.py` & `ipfsspec-0.4.0/ipfsspec/async_ipfs.py`

 * *Files identical despite different names*

### Comparing `ipfsspec-0.3.0/ipfsspec/core.py` & `ipfsspec-0.4.0/ipfsspec/core.py`

 * *Files identical despite different names*

### Comparing `ipfsspec-0.3.0/ipfsspec/tracing.py` & `ipfsspec-0.4.0/ipfsspec/tracing.py`

 * *Files identical despite different names*

### Comparing `ipfsspec-0.3.0/ipfsspec.egg-info/PKG-INFO` & `ipfsspec-0.4.0/ipfsspec.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: ipfsspec
-Version: 0.3.0
+Version: 0.4.0
 Summary: readonly implementation of fsspec for IPFS
 Home-page: https://github.com/fsspec/ipfsspec
 Author: Tobias Kölling
 Author-email: tobias.koelling@physik.uni-muenchen.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -26,9 +24,7 @@
 with fsspec.open("ipfs://QmZ4tDuvesekSs4qM5ZBKpXiZGun7S2CYtEZRB3DYXkjGx", "r") as f:
     print(f.read())
 ```
 
 The current implementation uses a HTTP gateway to access the data. It tries to use a local one (which is expected to be found at `http://127.0.0.1:8080`) and falls back to `ipfs.io` if the local gateway is not available.
 
 You can modify the list of gateways using the space separated environment variable `IPFSSPEC_GATEWAYS`.
-
-
```

### Comparing `ipfsspec-0.3.0/setup.py` & `ipfsspec-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `ipfsspec-0.3.0/test/test_async.py` & `ipfsspec-0.4.0/test/test_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import pytest
+import pytest_asyncio
 from ipfsspec.async_ipfs import AsyncIPFSGateway, MultiGateway, AsyncIPFSFileSystem
 import aiohttp
 
 TEST_ROOT = "QmW3CrGFuFyF3VH1wvrap4Jend5NRTgtESDjuQ7QhHD5dd"
 REF_CONTENT = b'ipfsspec test data'
 TEST_FILENAMES = ["default", "multi", "raw", "raw_multi", "write"]
 
 
-@pytest.fixture
+@pytest_asyncio.fixture
 async def session():
     async with aiohttp.ClientSession() as session:
         yield session
 
 
 @pytest.mark.local_gw
 @pytest.mark.parametrize("gw_host", ["http://127.0.0.1:8080"])
```

### Comparing `ipfsspec-0.3.0/test/test_async_fallback.py` & `ipfsspec-0.4.0/test/test_async_fallback.py`

 * *Files identical despite different names*

### Comparing `ipfsspec-0.3.0/test/test_gateway.py` & `ipfsspec-0.4.0/test/test_gateway.py`

 * *Files identical despite different names*

### Comparing `ipfsspec-0.3.0/test/test_ipfs.py` & `ipfsspec-0.4.0/test/test_ipfs.py`

 * *Files identical despite different names*

### Comparing `ipfsspec-0.3.0/versioneer.py` & `ipfsspec-0.4.0/versioneer.py`

 * *Files identical despite different names*

