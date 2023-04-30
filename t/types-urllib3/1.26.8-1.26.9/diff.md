# Comparing `tmp/types-urllib3-1.26.8.tar.gz` & `tmp/types-urllib3-1.26.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-urllib3-1.26.8.tar", last modified: Mon Jan 31 00:58:20 2022, max compression
+gzip compressed data, was "types-urllib3-1.26.9.tar", last modified: Thu Feb  3 00:58:22 2022, max compression
```

## Comparing `types-urllib3-1.26.8.tar` & `types-urllib3-1.26.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 00:58:20.907802 types-urllib3-1.26.8/
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-01-31 00:58:20.000000 types-urllib3-1.26.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-31 00:58:20.000000 types-urllib3-1.26.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-01-31 00:58:20.907802 types-urllib3-1.26.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-31 00:58:20.907802 types-urllib3-1.26.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1963 2022-01-31 00:58:20.000000 types-urllib3-1.26.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 00:58:20.903802 types-urllib3-1.26.8/types_urllib3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-01-31 00:58:20.000000 types-urllib3-1.26.8/types_urllib3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-01-31 00:58:20.000000 types-urllib3-1.26.8/types_urllib3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-31 00:58:20.000000 types-urllib3-1.26.8/types_urllib3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-31 00:58:20.000000 types-urllib3-1.26.8/types_urllib3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 00:58:20.907802 types-urllib3-1.26.8/urllib3-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-01-31 00:58:20.000000 types-urllib3-1.26.8/urllib3-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/_collections.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1976 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3170 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/connectionpool.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 00:58:20.907802 types-urllib3-1.26.8/urllib3-stubs/contrib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/contrib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2948 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/filepost.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 00:58:20.907802 types-urllib3-1.26.8/urllib3-stubs/packages/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/packages/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 00:58:20.907802 types-urllib3-1.26.8/urllib3-stubs/packages/ssl_match_hostname/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/packages/ssl_match_hostname/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/packages/ssl_match_hostname/_implementation.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/poolmanager.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/request.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3513 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/response.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 00:58:20.907802 types-urllib3-1.26.8/urllib3-stubs/util/
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/util/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/util/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/util/request.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/util/response.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3098 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/util/retry.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/util/ssl_.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/util/timeout.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-01-31 00:57:40.000000 types-urllib3-1.26.8/urllib3-stubs/util/url.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:58:22.287169 types-urllib3-1.26.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      663 2022-02-03 00:58:21.000000 types-urllib3-1.26.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-02-03 00:58:21.000000 types-urllib3-1.26.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-02-03 00:58:22.287169 types-urllib3-1.26.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-03 00:58:22.287169 types-urllib3-1.26.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1963 2022-02-03 00:58:21.000000 types-urllib3-1.26.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:58:22.283169 types-urllib3-1.26.9/types_urllib3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-02-03 00:58:22.000000 types-urllib3-1.26.9/types_urllib3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      925 2022-02-03 00:58:22.000000 types-urllib3-1.26.9/types_urllib3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-03 00:58:22.000000 types-urllib3-1.26.9/types_urllib3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-03 00:58:22.000000 types-urllib3-1.26.9/types_urllib3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:58:22.283169 types-urllib3-1.26.9/urllib3-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-02-03 00:58:21.000000 types-urllib3-1.26.9/urllib3-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      842 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/_collections.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1976 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3170 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/connectionpool.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:58:22.283169 types-urllib3-1.26.9/urllib3-stubs/contrib/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/contrib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2948 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/filepost.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:58:22.283169 types-urllib3-1.26.9/urllib3-stubs/packages/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/packages/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:58:22.283169 types-urllib3-1.26.9/urllib3-stubs/packages/ssl_match_hostname/
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/packages/ssl_match_hostname/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/packages/ssl_match_hostname/_implementation.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/poolmanager.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/request.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3544 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/response.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:58:22.287169 types-urllib3-1.26.9/urllib3-stubs/util/
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/util/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/util/request.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/util/response.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3098 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/util/retry.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      691 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/util/ssl_.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/util/timeout.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      492 2022-02-03 00:57:27.000000 types-urllib3-1.26.9/urllib3-stubs/util/url.pyi
```

### Comparing `types-urllib3-1.26.8/CHANGELOG.md` & `types-urllib3-1.26.9/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.26.9 (2022-02-03)
+
+Improve `__enter__` & constructor methods (#7114)
+
 ## 1.26.8 (2022-01-31)
 
 Upgrade black version (#7089)
 
 ## 1.26.7 (2022-01-13)
 
 urllib3: allow allowed_methods to be False (#6909)
```

### Comparing `types-urllib3-1.26.8/PKG-INFO` & `types-urllib3-1.26.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-urllib3
-Version: 1.26.8
+Version: 1.26.9
 Summary: Typing stubs for urllib3
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/urllib3.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -18,10 +18,10 @@
 This is a PEP 561 type stub package for the `urllib3` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `urllib3`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/urllib3. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `b88a6f19cdcf031be8135941b940f839e13064d8`.
+This package was generated from typeshed commit `fc60d02c3ea5ca006d0e8244c556f48d697a7c66`.
```

### Comparing `types-urllib3-1.26.8/setup.py` & `types-urllib3-1.26.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This is a PEP 561 type stub package for the `urllib3` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `urllib3`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/urllib3. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `b88a6f19cdcf031be8135941b940f839e13064d8`.
+This package was generated from typeshed commit `fc60d02c3ea5ca006d0e8244c556f48d697a7c66`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.26.8",
+      version="1.26.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/urllib3.md",
```

### Comparing `types-urllib3-1.26.8/types_urllib3.egg-info/PKG-INFO` & `types-urllib3-1.26.9/types_urllib3.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-urllib3
-Version: 1.26.8
+Version: 1.26.9
 Summary: Typing stubs for urllib3
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/urllib3.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -18,10 +18,10 @@
 This is a PEP 561 type stub package for the `urllib3` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `urllib3`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/urllib3. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `b88a6f19cdcf031be8135941b940f839e13064d8`.
+This package was generated from typeshed commit `fc60d02c3ea5ca006d0e8244c556f48d697a7c66`.
```

### Comparing `types-urllib3-1.26.8/types_urllib3.egg-info/SOURCES.txt` & `types-urllib3-1.26.9/types_urllib3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `types-urllib3-1.26.8/urllib3-stubs/__init__.pyi` & `types-urllib3-1.26.9/urllib3-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-urllib3-1.26.8/urllib3-stubs/_collections.pyi` & `types-urllib3-1.26.9/urllib3-stubs/_collections.pyi`

 * *Files identical despite different names*

### Comparing `types-urllib3-1.26.8/urllib3-stubs/connection.pyi` & `types-urllib3-1.26.9/urllib3-stubs/connection.pyi`

 * *Files identical despite different names*

### Comparing `types-urllib3-1.26.8/urllib3-stubs/connectionpool.pyi` & `types-urllib3-1.26.9/urllib3-stubs/connectionpool.pyi`

 * *Files identical despite different names*

### Comparing `types-urllib3-1.26.8/urllib3-stubs/exceptions.pyi` & `types-urllib3-1.26.9/urllib3-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-urllib3-1.26.8/urllib3-stubs/poolmanager.pyi` & `types-urllib3-1.26.9/urllib3-stubs/poolmanager.pyi`

 * *Files identical despite different names*

### Comparing `types-urllib3-1.26.8/urllib3-stubs/request.pyi` & `types-urllib3-1.26.9/urllib3-stubs/request.pyi`

 * *Files identical despite different names*

### Comparing `types-urllib3-1.26.8/urllib3-stubs/response.pyi` & `types-urllib3-1.26.9/urllib3-stubs/response.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import io
+from _typeshed import Self
 from http.client import HTTPMessage as _HttplibHTTPMessage, HTTPResponse as _HttplibHTTPResponse
 from typing import Any, Iterator, Mapping
 from typing_extensions import Literal
 
 from urllib3.connectionpool import HTTPConnection
 
 from . import HTTPConnectionPool, Retry
@@ -79,15 +80,15 @@
     @property
     def connection(self) -> HTTPConnection | Any: ...
     def isclosed(self) -> bool: ...
     def tell(self) -> int: ...
     def read(self, amt: int | None = ..., decode_content: bool | None = ..., cache_content: bool = ...) -> bytes: ...
     def stream(self, amt: int | None = ..., decode_content: bool | None = ...) -> Iterator[bytes]: ...
     @classmethod
-    def from_httplib(cls, r: _HttplibHTTPResponse, **response_kw: Any) -> HTTPResponse: ...
+    def from_httplib(cls: type[Self], r: _HttplibHTTPResponse, **response_kw: Any) -> Self: ...
     def getheaders(self) -> HTTPHeaderDict: ...
     def getheader(self, name, default=...) -> str | None: ...
     def info(self) -> HTTPHeaderDict: ...
     def close(self) -> None: ...
     @property
     def closed(self) -> bool: ...
     def fileno(self) -> int: ...
```

### Comparing `types-urllib3-1.26.8/urllib3-stubs/util/__init__.pyi` & `types-urllib3-1.26.9/urllib3-stubs/util/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-urllib3-1.26.8/urllib3-stubs/util/retry.pyi` & `types-urllib3-1.26.9/urllib3-stubs/util/retry.pyi`

 * *Files identical despite different names*

### Comparing `types-urllib3-1.26.8/urllib3-stubs/util/ssl_.pyi` & `types-urllib3-1.26.9/urllib3-stubs/util/ssl_.pyi`

 * *Files identical despite different names*

