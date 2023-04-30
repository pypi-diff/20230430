# Comparing `tmp/curl_arguments_url-0.1.2.tar.gz` & `tmp/curl_arguments_url-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curl_arguments_url-0.1.2.tar", last modified: Fri Apr 14 18:17:24 2023, max compression
+gzip compressed data, was "curl_arguments_url-0.1.3.tar", last modified: Sun Apr 30 18:00:15 2023, max compression
```

## Comparing `curl_arguments_url-0.1.2.tar` & `curl_arguments_url-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:24.600050 curl_arguments_url-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-04-14 18:17:24.600050 curl_arguments_url-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:24.600050 curl_arguments_url-0.1.2/curl_arguments_url/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/curl_arguments_url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/curl_arguments_url/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/curl_arguments_url/click_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    55084 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/curl_arguments_url/curl_arguments_url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:24.600050 curl_arguments_url-0.1.2/curl_arguments_url.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-04-14 18:17:24.000000 curl_arguments_url-0.1.2/curl_arguments_url.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-14 18:17:24.000000 curl_arguments_url-0.1.2/curl_arguments_url.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:17:24.000000 curl_arguments_url-0.1.2/curl_arguments_url.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 18:17:24.000000 curl_arguments_url-0.1.2/curl_arguments_url.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:17:24.000000 curl_arguments_url-0.1.2/curl_arguments_url.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 18:17:24.000000 curl_arguments_url-0.1.2/curl_arguments_url.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 18:17:24.000000 curl_arguments_url-0.1.2/curl_arguments_url.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-14 18:17:24.600050 curl_arguments_url-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:00:15.899566 curl_arguments_url-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-04-30 18:00:15.899566 curl_arguments_url-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:00:15.895566 curl_arguments_url-0.1.3/curl_arguments_url/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/curl_arguments_url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/curl_arguments_url/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/curl_arguments_url/click_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57514 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/curl_arguments_url/curl_arguments_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:00:15.899566 curl_arguments_url-0.1.3/curl_arguments_url/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/curl_arguments_url/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/curl_arguments_url/models/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/curl_arguments_url/models/open_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/curl_arguments_url/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:00:15.895566 curl_arguments_url-0.1.3/curl_arguments_url.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-04-30 18:00:15.000000 curl_arguments_url-0.1.3/curl_arguments_url.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-30 18:00:15.000000 curl_arguments_url-0.1.3/curl_arguments_url.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:00:15.000000 curl_arguments_url-0.1.3/curl_arguments_url.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-30 18:00:15.000000 curl_arguments_url-0.1.3/curl_arguments_url.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:00:15.000000 curl_arguments_url-0.1.3/curl_arguments_url.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-30 18:00:15.000000 curl_arguments_url-0.1.3/curl_arguments_url.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 18:00:15.000000 curl_arguments_url-0.1.3/curl_arguments_url.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-30 18:00:15.899566 curl_arguments_url-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/version.txt
```

### Comparing `curl_arguments_url-0.1.2/LICENSE` & `curl_arguments_url-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `curl_arguments_url-0.1.2/PKG-INFO` & `curl_arguments_url-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curl_arguments_url
-Version: 0.1.2
+Version: 0.1.3
 Summary: Curl with Arguments for Url
 Home-page: https://github.com/valmikirao/curl_arguments_url
 Author: Valmiki Rao
 Author-email: valmikirao@gmail.com
 License: Apache Software License 2.0
 Keywords: curl_arguments_url,carl,curl,zsh,completions,swagger,openapi
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: ryaml
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # AWS Cloudwatch Insights
 
 ![version](https://img.shields.io/pypi/v/curl_arguments_url)
 ![python versions](https://img.shields.io/pypi/pyversions/curl_arguments_url)
@@ -48,14 +49,20 @@
 % pip install 'curl_arguments_url'
 
 # to get the completions to work, add the following to your .zshrc
 eval "$(carl utils zsh-print-script)"
 
 # And copy the OpenAPI spec into ~/.carl/open_api to get the completions and curl-building working
 % cp open_api-spec.yml ~/.carl/open_api
+
+# if parsing of the open_api files is too slow for you, you can try installing the ryaml (Rust Yaml) extension. I
+# didn't include this by default because I'm afraid it might not install correctly on certain systems, but it's much
+# faster
+% pipx install 'curl_arguments_url[ryaml]'
+ 
 ```
 
 ### Examples
 
 These examples use [tests/resources/open_api/openapi-demo.yml](tests/resources/open_api/openapi-demo.yml)
 
 * Basic GET
@@ -180,14 +187,19 @@
 ```text
     CARL_DIR: Directory which contains files for carl. Default: ~/.carl
     CARL_OPEN_API_DIR: Directory containing the OpenApi specifications and
                         Yaml files. Default: $CARL_DIR/open_api
     CARL_CACHE_DIR: Directory containing the cache. Default $CARL_DIR/cache
 ```
 
+### Hints for finding OpenAPI specs
+
+The spec you're interested in might be on https://app.swaggerhub.com/.  Also, sometimes the doc/sandbox page, for an
+api, which gives you a gui for interacting with the api, loads the swagger spec in the background.  You can see this
+if you open the developer tools in Chrome under Network
 
 ## Development
 
 Requires make:
 
 ```shell
 # setting up dev environment
```

### Comparing `curl_arguments_url-0.1.2/README.md` & `curl_arguments_url-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 % pip install 'curl_arguments_url'
 
 # to get the completions to work, add the following to your .zshrc
 eval "$(carl utils zsh-print-script)"
 
 # And copy the OpenAPI spec into ~/.carl/open_api to get the completions and curl-building working
 % cp open_api-spec.yml ~/.carl/open_api
+
+# if parsing of the open_api files is too slow for you, you can try installing the ryaml (Rust Yaml) extension. I
+# didn't include this by default because I'm afraid it might not install correctly on certain systems, but it's much
+# faster
+% pipx install 'curl_arguments_url[ryaml]'
+ 
 ```
 
 ### Examples
 
 These examples use [tests/resources/open_api/openapi-demo.yml](tests/resources/open_api/openapi-demo.yml)
 
 * Basic GET
@@ -157,14 +163,19 @@
 ```text
     CARL_DIR: Directory which contains files for carl. Default: ~/.carl
     CARL_OPEN_API_DIR: Directory containing the OpenApi specifications and
                         Yaml files. Default: $CARL_DIR/open_api
     CARL_CACHE_DIR: Directory containing the cache. Default $CARL_DIR/cache
 ```
 
+### Hints for finding OpenAPI specs
+
+The spec you're interested in might be on https://app.swaggerhub.com/.  Also, sometimes the doc/sandbox page, for an
+api, which gives you a gui for interacting with the api, loads the swagger spec in the background.  You can see this
+if you open the developer tools in Chrome under Network
 
 ## Development
 
 Requires make:
 
 ```shell
 # setting up dev environment
```

### Comparing `curl_arguments_url-0.1.2/curl_arguments_url/cli.py` & `curl_arguments_url-0.1.3/curl_arguments_url/cli.py`

 * *Files identical despite different names*

### Comparing `curl_arguments_url-0.1.2/curl_arguments_url/click_test.py` & `curl_arguments_url-0.1.3/curl_arguments_url/click_test.py`

 * *Files identical despite different names*

### Comparing `curl_arguments_url-0.1.2/curl_arguments_url/curl_arguments_url.py` & `curl_arguments_url-0.1.3/curl_arguments_url/curl_arguments_url.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Main module."""
 import argparse
+import io
 import itertools
 import json
 import os
 import re
 import shutil
 import sys
 import textwrap
@@ -13,21 +14,24 @@
 from datetime import datetime
 from enum import Enum
 from hashlib import md5
 from typing import Iterable, NamedTuple, Tuple, Sequence, List, Union, Dict, Optional, TypeVar, Generic, \
     Callable, Any, MutableMapping, cast, Set
 
 from jsonref import replace_refs as replace_json_refs  # type: ignore
-from openapi_schema_pydantic import OpenAPI, Operation, RequestBody, Schema, Reference, Parameter, PathItem, Server
 from pydantic import BaseModel, validator
 from typing_extensions import Literal
 from urllib.parse import urlencode
 import yaml
 import yaml.parser
 
+from curl_arguments_url.models import open_api
+from curl_arguments_url.models.methods import Method
+from curl_arguments_url.yaml import load_yaml
+
 REMAINING_ARG = 'passed_to_curl'
 
 ParamValue = Union[str, int, float, Dict[str, Any], List[Any]]
 
 
 class EnvVariable:
     registry: List['EnvVariable'] = []
@@ -55,46 +59,33 @@
 OPEN_API_DIR = OPEN_API_DIR_ENV.get_value()
 CACHE_DIR_ENV = EnvVariable(
     'CARL_CACHE_DIR', os.path.join(CARL_DIR, 'cache'),
     description='Directory containing the cache. Default $CARL_DIR/cache'
 )
 CACHE_DIR = CACHE_DIR_ENV.get_value()
 
-
-class Method(Enum):
-    GET = 'GET'
-    PUT = 'PUT'
-    POST = 'POST'
-    DELETE = 'DELETE'
-    OPTIONS = 'OPTIONS'
-    HEAD = 'HEAD'
-    PATCH = 'PATCH'
-    TRACE = 'TRACE'
-
-
-METHODS: List[str] = list(Method.__members__.keys())
-
-
 T = TypeVar('T')
 V = TypeVar('V')
 U = TypeVar('U')
 ArgType = Callable[[str], T]
 
 
 class FileCache(ABC, Generic[T, V]):
+    __manually_close_file__ = False
+
     def __init__(self, dir_: str):
         self._dir = os.path.join(CACHE_DIR, dir_)
         self._process_cache: Dict[T, V] = {}
 
     @abstractmethod
     def freeze(self, value: V) -> str:
         ...
 
     @abstractmethod
-    def thaw(self, frozen_value: str) -> V:
+    def thaw(self, frozen_value: io.TextIOWrapper) -> V:
         ...
 
     @abstractmethod
     def freeze_key(self, key: T) -> str:
         ...
 
     def clear(self) -> None:
@@ -106,16 +97,20 @@
         key_hash = md5(key_stringified).hexdigest()
         return os.path.join(self._dir, key_hash)
 
     def __getitem__(self, key: T) -> V:
         if key not in self._process_cache:
             key_filename = self._get_key_filename(key)
             if os.path.exists(key_filename):
-                with open(key_filename, 'r') as fh:
-                    self._process_cache[key] = self.thaw(fh.read())
+                fh = open(key_filename, 'r')
+                try:
+                    self._process_cache[key] = self.thaw(fh)
+                finally:
+                    if not self.__manually_close_file__:
+                        fh.close()
             else:
                 raise KeyError(key)
         return self._process_cache[key]
 
     def __setitem__(self, key: T, value: V) -> None:
         self._process_cache[key] = value
         os.makedirs(self._dir, exist_ok=True)
@@ -384,57 +379,103 @@
 
 class UrlToCache(BaseModel):
     url: str
     summary: Optional[str]
     description: Optional[str]
 
 
-class RootCacheItem(BaseModel):
-    time: float
-    urls: List[UrlToCache]
-    params_with_cached_values: List[str] = []
+class TimeCache(FileCache[None, float]):
+    def freeze(self, value: float) -> str:
+        return str(value)
+
+    def thaw(self, frozen_value: io.TextIOWrapper) -> float:
+        return float(frozen_value.read())
 
+    def freeze_key(self, key: None) -> str:
+        return 'TIME-CACHE-KEY'
 
-class RootCache(FileCache[None, RootCacheItem]):
-    ROOT_CACHE_KEY = 'NO-KEY'
+    def get_value(self) -> float:
+        return self.get(None, 0)
 
-    def freeze(self, value: RootCacheItem) -> str:
-        return value.json()
+    def set_value(self, value: float) -> None:
+        self[None] = value
 
-    def thaw(self, frozen_value: str) -> RootCacheItem:
-        return RootCacheItem.parse_raw(frozen_value)
+
+class ParamsWithCachedValuesCache(FileCache[None, List[str]]):
+    def freeze(self, value: List[str]) -> str:
+        return json.dumps(value)
+
+    def thaw(self, frozen_value: io.TextIOWrapper) -> List[str]:
+        return json.loads(frozen_value.read())
 
     def freeze_key(self, key: None) -> str:
-        return self.ROOT_CACHE_KEY
+        return 'PARAMS-WITH-CACHED-VALUES-KEY'
+
+    def get_value(self) -> List[str]:
+        return self.get(None, [])
+
+    def set_value(self, value: List[str]) -> None:
+        self[None] = value
+
+
+class UrlsCache(FileCache[None, Iterable[UrlToCache]]):
+    __manually_close_file__ = True
+
+    def freeze(self, value: Iterable[UrlToCache]) -> str:
+        return_val = ''
+        for v in value:
+            # still json dumping, in cas there is a newline
+            return_val += v.json() + "\n"
+        return return_val
+
+    def thaw(self, frozen_value: io.TextIOWrapper) -> Iterable[UrlToCache]:
+        try:
+            for line in frozen_value:
+                yield UrlToCache.parse_raw(line)
+        finally:
+            frozen_value.close()
+
+    def freeze_key(self, key: T) -> str:
+        return 'URLS-KEY'
+
+    def get_value(self) -> Iterable[UrlToCache]:
+        # need to clear the process cache, since this might be an iterator
+        if None in self._process_cache:
+            del self._process_cache[None]
+        return self.get(None, [])
 
+    def set_value(self, value: Iterable[UrlToCache]) -> None:
+        self[None] = value
 
-class MethodsCache(FileCache[str, List[Method]]):
-    def freeze(self, value: List[Method]) -> str:
-        return json.dumps([
-            v.value for v in value
-        ])
-
-    def thaw(self, frozen_value: str) -> List[Method]:
-        return [
-            Method(v) for v in json.loads(frozen_value)
-        ]
+
+class MethodsToCache(BaseModel):
+    url: UrlToCache
+    methods: List[Method]
+
+
+class MethodsCache(FileCache[str, MethodsToCache]):
+    def freeze(self, value: MethodsToCache) -> str:
+        return value.json()
+
+    def thaw(self, frozen_value: io.TextIOWrapper) -> MethodsToCache:
+        return MethodsToCache.parse_raw(frozen_value.read())
 
     def freeze_key(self, key: str) -> str:
         return key
 
 
 EndpointKey = Tuple[str, Method]
 
 
 class EndpointCache(FileCache[EndpointKey, EndpointToCache]):
     def freeze(self, value: EndpointToCache) -> str:
         return value.json()
 
-    def thaw(self, frozen_value: str) -> EndpointToCache:
-        return EndpointToCache.parse_raw(frozen_value)
+    def thaw(self, frozen_value: io.TextIOWrapper) -> EndpointToCache:
+        return EndpointToCache.parse_raw(frozen_value.read())
 
     def freeze_key(self, key: EndpointKey) -> str:
         url, method = key
         method_str = method.value
         return json.dumps([url, method_str])
 
 
@@ -475,171 +516,188 @@
 
 
 class CarlServer(NamedTuple):
     url: str
     params: List[CarlParam]
 
 
+class MockSingletonCache(dict):
+    def __init__(self, default: Any, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._default = default
+
+    def get_value(self) -> Any:
+        return self.get(None, self._default)
+
+    def set_value(self, value: Any) -> None:
+        self[None] = value
+
+
 class SwaggerRepo:
 
     def __init__(self, files: Optional[List[str]] = None, ephemeral: bool = False, warnings: bool = True):
         if not ephemeral:
-            self.root_cache = RootCache('root')
+            self.time_cache = TimeCache('time')
+            self.urls_cache = UrlsCache('urls')
+            self.params_with_cached_values_cache = ParamsWithCachedValuesCache('params_with_cached_values')
             self.methods_cache = MethodsCache('methods')
             self.endpoint_cache = EndpointCache('endpoint')
             self.arg_value_cache = ArgCache('arg_values')
         else:
             # this is a testing case, so make all caches are ephemeral
             # casting dicts should be OK, since they should have a subset of the
             # functions implemented in FileCache
-            self.root_cache = cast(RootCache, {})
+            self.time_cache = cast(TimeCache, MockSingletonCache(0))
+            self.urls_cache = cast(UrlsCache, MockSingletonCache([]))
+            self.params_with_cached_values_cache = cast(ParamsWithCachedValuesCache, MockSingletonCache([]))
             self.methods_cache = cast(MethodsCache, {})
             self.endpoint_cache = cast(EndpointCache, {})
             self.arg_value_cache = cast(ArgCache, {})
 
         if files is None:
             os.makedirs(OPEN_API_DIR, exist_ok=True)
             swagger_files = list(get_files_in_dir(OPEN_API_DIR))
         else:
             swagger_files = files
 
-        root_cache_item = self.root_cache.get(None, None)
-
-        if len(swagger_files) == 0 and root_cache_item:
+        if len(swagger_files) == 0:
             # make sure the cached data is clear
-            if len(root_cache_item.urls) > 0:
-                self.clear_all_spec_caches()
-        elif len(swagger_files) == 0:
-            # nothing to clear
-            pass
+            self.clear_all_spec_caches()
         else:
-            if root_cache_item:
-                cache_time = root_cache_item.time
-            else:
-                cache_time = 0
+            cache_time = self.time_cache.get_value()
             yaml_files_time = max(os.path.getmtime(f) for f in swagger_files)
             if yaml_files_time > cache_time:
                 self.clear_all_spec_caches()
                 self.load_swagger_data(swagger_files=swagger_files, warnings=warnings)
 
     def clear_all_spec_caches(self) -> None:
-        self.root_cache.clear()
+        self.time_cache.clear()
+        self.urls_cache.clear()
         self.methods_cache.clear()
         self.endpoint_cache.clear()
 
     def load_swagger_data(self, swagger_files: Optional[Iterable[str]], warnings: bool = False):
         cache_time = datetime.now().timestamp()
-        multi_swagger_data: List[OpenAPI] = []
+        multi_swagger_data = self.parse_swagger_files(swagger_files, warnings=warnings)
+
+        urls_to_cache: MutableMapping[str, UrlToCache] = OrderedDict()
+        methods_to_cache: MutableMapping[str, MethodsToCache] = {}
+        for swagger_data_ in multi_swagger_data:
+            root_description = swagger_data_.info.description
+            root_summary = swagger_data_.info.summary or swagger_data_.info.title
+
+            carl_servers = list(self.to_carl_servers(swagger_data_.servers))
+            for path_str, path_spec in swagger_data_.get_lazy_paths(warnings=warnings):
+                # Note: this doesn't deal with relative servers, we might need to deal with that
+                # when fetching the spec
+                carl_servers_for_path: List[CarlServer]
+                if path_spec.servers:
+                    servers_for_path = list(self.to_carl_servers(path_spec.servers))
+                else:
+                    servers_for_path = carl_servers
+
+                path_description = path_spec.description or root_description
+                path_summary = path_spec.summary or root_summary
+
+                for method in Method.__members__.values():
+                    operation = self._get_operation(path_spec, method)
+                    if operation:
+                        if operation.servers:
+                            servers_for_op = list(self.to_carl_servers(operation.servers))
+                        else:
+                            servers_for_op = servers_for_path
+                        op_params: List[CarlParam] = []
+                        for parameter in operation.parameters or []:
+                            if isinstance(parameter, open_api.Parameter):
+                                param_type = self.schema_to_arg_type(parameter.param_schema)
+                                enums: Optional[ParamValue]
+                                if isinstance(parameter.param_schema, open_api.Schema):
+                                    enums = parameter.param_schema.enum
+                                else:
+                                    enums = None
+                                op_params.append(CarlParam(
+                                    name=parameter.name,
+                                    param_type=ParamType(parameter.param_in),
+                                    description=parameter.description,
+                                    required_=parameter.required,
+                                    type_=param_type,
+                                    enums=enums
+                                ))
+                            else:  # is a Reference
+                                # Hopefully we have already resolved the references
+                                pass
+                        if isinstance(operation.requestBody, open_api.RequestBody):
+                            params_from_body = self._get_params_from_body(operation.requestBody)
+                            op_params.extend(params_from_body)
+
+                        op_description = operation.description or path_description
+                        op_summary = operation.summary or path_summary
+                        for server in servers_for_op:
+                            endpoint_url = server.url + path_str
+                            parameters = server.params + op_params
+                            self.endpoint_cache[endpoint_url, method] = EndpointToCache(
+                                endpoint_url=endpoint_url,
+                                method=method,
+                                parameters=parameters,
+                                summary=op_summary,
+                                description=op_description
+                            )
+                            url_to_cache = UrlToCache(
+                                url=endpoint_url,
+                                summary=path_summary,
+                                description=path_description
+                            )
+                            if endpoint_url not in urls_to_cache:
+                                urls_to_cache[endpoint_url] = url_to_cache
+
+                            if endpoint_url in methods_to_cache:
+                                methods_to_cache[endpoint_url].methods.append(method)
+                            else:
+                                methods_to_cache[endpoint_url] = MethodsToCache(
+                                    url=url_to_cache,
+                                    methods=[method]
+                                )
+
+        for url, methods in methods_to_cache.items():
+            self.methods_cache[url] = methods
+
+        self.time_cache.set_value(cache_time)
+        self.urls_cache.set_value(urls_to_cache.values())
+
+    def parse_swagger_files(self, swagger_files: Optional[Iterable[str]], warnings: bool) \
+            -> Iterable[open_api.OpenApiLazy]:
         if swagger_files is not None:
             for file in swagger_files:
                 with open(file, 'r') as fh:
                     loaded: Optional[Dict[str, Any]]
                     try:
-                        loaded = yaml.safe_load(fh)
+                        loaded = load_yaml(fh)
                     except yaml.parser.ParserError as e:
                         if warnings:
                             print('WARNING: ' + str(e), file=sys.stderr)
                         loaded = None
                     if loaded is not None:
                         try:
-                            loaded = replace_json_refs(loaded, merge_props=True)
-                            multi_swagger_data.append(OpenAPI.parse_obj(loaded))
+                            loaded = cast(Dict[str, Any], replace_json_refs(loaded, merge_props=True))
+                            loaded['unparsed_paths'] = loaded.pop('paths', {})
+                            yield open_api.OpenApiLazy.parse_obj(loaded)
                         except Exception as e:
                             if warnings:
                                 print(f"WARNING: Error in file {file!r}: {str(e)}", file=sys.stderr)
                             else:
                                 # fail silently
                                 pass
                     elif warnings:
                         print(f"WARNING: Yaml error in file {file!r}", file=sys.stderr)
                     else:
                         # fail silently
                         pass
 
-        urls_to_cache: MutableMapping[str, UrlToCache] = OrderedDict()
-        methods_to_cache: MutableMapping[str, List[Method]] = defaultdict(list)
-        for swagger_data_ in multi_swagger_data:
-            root_description = swagger_data_.info.description
-            root_summary = swagger_data_.info.summary or swagger_data_.info.title
-
-            carl_servers = list(self.to_carl_servers(swagger_data_.servers))
-            if swagger_data_.paths:
-                for path_str, path_spec in swagger_data_.paths.items():
-                    # Note: this doesn't deal with relative servers, we might need to deal with that
-                    # when fetching the spec
-                    carl_servers_for_path: List[CarlServer]
-                    if path_spec.servers:
-                        servers_for_path = list(self.to_carl_servers(path_spec.servers))
-                    else:
-                        servers_for_path = carl_servers
-
-                    path_description = path_spec.description or root_description
-                    path_summary = path_spec.summary or root_summary
-
-                    for method in Method.__members__.values():
-                        operation = self._get_operation(path_spec, method)
-                        if operation:
-                            if operation.servers:
-                                servers_for_op = list(self.to_carl_servers(operation.servers))
-                            else:
-                                servers_for_op = servers_for_path
-                            op_params: List[CarlParam] = []
-                            for parameter in operation.parameters or []:
-                                if isinstance(parameter, Parameter):
-                                    param_type = self.schema_to_arg_type(parameter.param_schema)
-                                    enums: Optional[ParamValue]
-                                    if isinstance(parameter.param_schema, Schema):
-                                        enums = parameter.param_schema.enum
-                                    else:
-                                        enums = None
-                                    op_params.append(CarlParam(
-                                        name=parameter.name,
-                                        param_type=ParamType(parameter.param_in),
-                                        description=parameter.description,
-                                        required_=parameter.required,
-                                        type_=param_type,
-                                        enums=enums
-                                    ))
-                                else:  # is a Reference
-                                    # Hopefully we have already resolved the references
-                                    pass
-                            if isinstance(operation.requestBody, RequestBody):
-                                params_from_body = self._get_params_from_body(operation.requestBody)
-                                op_params.extend(params_from_body)
-
-                            op_description = operation.description or path_description
-                            op_summary = operation.summary or path_summary
-                            for server in servers_for_op:
-                                endpoint_url = server.url + path_str
-                                parameters = server.params + op_params
-                                self.endpoint_cache[endpoint_url, method] = EndpointToCache(
-                                    endpoint_url=endpoint_url,
-                                    method=method,
-                                    parameters=parameters,
-                                    summary=op_summary,
-                                    description=op_description
-                                )
-                                if endpoint_url not in urls_to_cache:
-                                    urls_to_cache[endpoint_url] = UrlToCache(
-                                        url=endpoint_url,
-                                        summary=path_summary,
-                                        description=path_description
-                                    )
-                                methods_to_cache[endpoint_url].append(method)
-
-        for url, methods in methods_to_cache.items():
-            self.methods_cache[url] = methods
-
-        self.root_cache[None] = RootCacheItem(
-            time=cache_time,
-            urls=list(urls_to_cache.values())
-        )
-
     @staticmethod
-    def to_carl_servers(servers: List[Server]) -> Iterable[CarlServer]:
+    def to_carl_servers(servers: List[open_api.Server]) -> Iterable[CarlServer]:
         for server in servers:
             server_params: List[CarlParam] = []
             defaulted_url: Optional[str] = None
             if server.variables is not None:
                 defaults: Dict[str, str] = {}
                 for variable_name, variable_spec in server.variables.items():
                     # this casting shouldn't be necessary, but mypy isn't happy it without it
@@ -648,31 +706,32 @@
                         name=variable_name,
                         param_type=ParamType.path,
                         description=variable_spec.description,
                         enums=variable_enums,
                         required_=False,
                         default=variable_spec.default
                     ))
-                    defaults[variable_name] = variable_spec.default
+                    if variable_spec.default is not None:
+                        defaults[variable_name] = variable_spec.default
                 try:
                     defaulted_url = server.url.format(**defaults)
                 except KeyError:
                     pass
             if defaulted_url is not None:
                 yield CarlServer(defaulted_url, [])
             yield CarlServer(server.url, server_params)
 
     @staticmethod
-    def _get_operation(path_spec: PathItem, method: Method) -> Optional[Operation]:
+    def _get_operation(path_spec: open_api.PathItem, method: Method) -> Optional[open_api.Operation]:
         # maybe someday make this more type-safe
         return getattr(path_spec, method.value.lower())
 
     @staticmethod
-    def schema_to_arg_type(schema: Union[Schema, Reference, None]) -> ArgTypeModel:
-        if schema is None or isinstance(schema, Reference):
+    def schema_to_arg_type(schema: Optional[open_api.Schema]) -> ArgTypeModel:
+        if schema is None:
             return ArgTypeModel(type_=ArgTypeEnum.string)
         schema_type = schema.type
         schema_items = schema.items
         if schema_type is None or schema_type == []:
             # default
             return ArgTypeModel(type_=ArgTypeEnum.string)
         else:
@@ -682,18 +741,18 @@
                 schema_type_ = schema_type[0]
             else:
                 schema_type_ = schema_type
 
             if schema_type_ == SpecialSwaggerTypeStrs.object:
                 return ArgTypeModel(type_=ArgTypeEnum.json)
             elif schema_type_ == SpecialSwaggerTypeStrs.array:
-                if schema_items is None or isinstance(schema_items, Reference):
+                if schema_items is None:
                     return ArgTypeModel(type_=ArgTypeEnum.string, is_array=True)
                 else:
-                    items_type = SwaggerRepo.schema_to_arg_type(Schema(
+                    items_type = SwaggerRepo.schema_to_arg_type(open_api.Schema(
                         type=schema_items.type,
                         items=None
                     ))
                     if items_type.is_array:
                         return ArgTypeModel(
                             type_=ArgTypeEnum.json,
                             is_array=True
@@ -706,26 +765,28 @@
             else:
                 arg_type_enum = ArgTypeEnum(schema_type_)
                 return ArgTypeModel(
                     type_=arg_type_enum,
                     is_array=False
                 )
 
-    def _get_params_from_body(self, request_body: RequestBody) -> Iterable[CarlParam]:
+    def _get_params_from_body(self, request_body: open_api.RequestBody) -> Iterable[CarlParam]:
         for json_mime_type in ('application/json', 'json'):
             if json_mime_type in request_body.content:
                 schema = request_body.content[json_mime_type].media_type_schema
-                if isinstance(schema, Schema) and schema.type == SpecialSwaggerTypeStrs.object and schema.properties:
+                if isinstance(schema, open_api.Schema) \
+                        and schema.type == SpecialSwaggerTypeStrs.object \
+                        and schema.properties:
                     if schema.required is not None:
                         required_props = set(schema.required)
                     else:
                         required_props = set()
                     for prop_name, prop_schema in schema.properties.items():
                         carl_param_type = self.schema_to_arg_type(prop_schema)
-                        if isinstance(prop_schema, Schema):
+                        if isinstance(prop_schema, open_api.Schema):
                             description = prop_schema.description
                             enums = prop_schema.enum
                         else:
                             description = None
                             enums = None
 
                         yield CarlParam(
@@ -744,86 +805,86 @@
                 pass
 
     def cli_args_to_cmd(self, cli_args: Sequence[str]) \
             -> Tuple[Sequence[str], GenericArgs]:
         # url is always the first arg
         url: Optional[str] = cli_args[0] if len(cli_args) >= 1 else None
 
-        root_cache_item = self.root_cache.get(None, None)
-        possible_urls: List[UrlToCache]
-        if root_cache_item:
-            possible_urls = root_cache_item.urls
-        else:
-            possible_urls = []
         valid_url_chosen: Optional[UrlToCache]
         if url is None:
             valid_url_chosen = None
         else:
-            for possible_url in possible_urls:
-                if possible_url.url == url:
-                    valid_url_chosen = possible_url
-                    break
+            cached_methods = self.methods_cache.get(url, None)
+            if cached_methods is not None:
+                valid_url_chosen = cached_methods.url
             else:
                 valid_url_chosen = None
 
-        if not valid_url_chosen:
+        if not valid_url_chosen and url != UTILS_COMPLETION_ITEM.tag:
             # either this is a --help request or an error
             no_url_parser = get_arg_parser()
             url_subparsers = no_url_parser.add_subparsers(dest='url', required=True)
 
             url_subparsers = add_utils_parser(url_subparsers)
+            possible_urls = self.urls_cache.get_value()
             for possible_url in possible_urls:
                 possible_url_desc = possible_url.description or possible_url.summary
                 url_subparsers.add_parser(possible_url.url, help=possible_url_desc)
 
             # This should give either the correct error or correct help message
+            no_url_parser.parse_args(cli_args)
+            raise AssertionError('Should not make it here')
+        elif not valid_url_chosen and url == UTILS_COMPLETION_ITEM.tag:
+            # this is a util request, will
+            no_url_parser = get_arg_parser()
+            url_subparsers = no_url_parser.add_subparsers(dest='url', required=True)
+            add_utils_parser(url_subparsers)
+
             parsed_args = no_url_parser.parse_args(cli_args)
 
-            if parsed_args.url == UTILS_COMPLETION_ITEM.tag:
-                # this is a util request, will
-                values_ls_for_param: Optional[str]
-                if parsed_args.util_type == VALUES_COMPLETION.tag \
-                        and parsed_args.cached_values_type == VALUES_LS_COMPLETION.tag:
-                    values_ls_for_param = parsed_args.param_name
-                else:
-                    values_ls_for_param = None
-                values_rm_args: Optional[ValuesRmArgs]
-                if parsed_args.util_type == VALUES_COMPLETION.tag \
-                        and parsed_args.cached_values_type == VALUES_RM_COMPLETION.tag:
-                    values_rm_args = ValuesRmArgs(
-                        param_name=parsed_args.param_name,
-                        value=parsed_args.value
-                    )
-                else:
-                    values_rm_args = None
-                values_add_args: Optional[ValuesAddArgs]
-                if parsed_args.util_type == VALUES_COMPLETION.tag and \
-                        parsed_args.cached_values_type == VALUES_ADD_COMPLETION.tag:
-                    values_add_args = ValuesAddArgs(
-                        param_name=parsed_args.param_name,
-                        values=parsed_args.value
-                    )
-                else:
-                    values_add_args = None
-                return [], GenericArgs(
-                    util=True,
-                    zsh_completion_args=namespace_to_zsh_completion_args(parsed_args),
-                    zsh_print_script=(parsed_args.util_type == ZSH_PRINT_SCRIPT_COMPLETION.tag),
-                    values_list_params=(
-                        parsed_args.util_type == VALUES_COMPLETION.tag
-                        and parsed_args.cached_values_type == VALUES_PARAMS_COMPLETION.tag
-                    ),
-                    values_ls_for_param=values_ls_for_param,
-                    values_rm_args=values_rm_args,
-                    values_add_args=values_add_args,
-                    rebuild_cache=(parsed_args.util_type == REBUILD_CACHE_COMPLETION.tag)
+            assert parsed_args.url == UTILS_COMPLETION_ITEM.tag
+
+            values_ls_for_param: Optional[str]
+            if parsed_args.util_type == VALUES_COMPLETION.tag \
+                    and parsed_args.cached_values_type == VALUES_LS_COMPLETION.tag:
+                values_ls_for_param = parsed_args.param_name
+            else:
+                values_ls_for_param = None
+            values_rm_args: Optional[ValuesRmArgs]
+            if parsed_args.util_type == VALUES_COMPLETION.tag \
+                    and parsed_args.cached_values_type == VALUES_RM_COMPLETION.tag:
+                values_rm_args = ValuesRmArgs(
+                    param_name=parsed_args.param_name,
+                    value=parsed_args.value
                 )
             else:
-                raise AssertionError('Should not make it here')
-        else:
+                values_rm_args = None
+            values_add_args: Optional[ValuesAddArgs]
+            if parsed_args.util_type == VALUES_COMPLETION.tag and \
+                    parsed_args.cached_values_type == VALUES_ADD_COMPLETION.tag:
+                values_add_args = ValuesAddArgs(
+                    param_name=parsed_args.param_name,
+                    values=parsed_args.value
+                )
+            else:
+                values_add_args = None
+            return [], GenericArgs(
+                util=True,
+                zsh_completion_args=namespace_to_zsh_completion_args(parsed_args),
+                zsh_print_script=(parsed_args.util_type == ZSH_PRINT_SCRIPT_COMPLETION.tag),
+                values_list_params=(
+                        parsed_args.util_type == VALUES_COMPLETION.tag
+                        and parsed_args.cached_values_type == VALUES_PARAMS_COMPLETION.tag
+                ),
+                values_ls_for_param=values_ls_for_param,
+                values_rm_args=values_rm_args,
+                values_add_args=values_add_args,
+                rebuild_cache=(parsed_args.util_type == REBUILD_CACHE_COMPLETION.tag)
+            )
+        elif valid_url_chosen is not None:
             url_desc = valid_url_chosen.description or valid_url_chosen.summary
             use_requires = get_use_requires(cli_args)
             arg_parser = self.get_path_arg_parser(
                 url=valid_url_chosen.url,
                 url_desc=url_desc,
                 use_requires=use_requires
             )
@@ -845,36 +906,35 @@
 
             generic_args = GenericArgs(
                 print_cmd=args.print_cmd,
                 run_cmd=args.run_cmd
             )
 
             return ['curl', '-X', method_, formatted_url, *headers, *post_data, *remaining], generic_args
+        else:
+            raise NotImplementedError()
 
     def cache_param_arg_pairs(self, param_args: ArgPairs) -> None:
         param_names: List[str] = []
         for param, value in param_args:
             key = param.name
             param_names.append(key)
             arg_history: List[ParamValue] = self.arg_value_cache.get(key, [])
 
             new_history: List[ParamValue] = [value] + [a for a in arg_history if a != value]
             new_history = new_history[:MAX_HISTORY]
             self.arg_value_cache[key] = new_history
-        root_cache_item = self.root_cache[None]
-        existing_param_names = root_cache_item.params_with_cached_values
+        existing_param_names = self.params_with_cached_values_cache.get_value()
         params_with_cached_values = list(set(param_names + existing_param_names))
         params_with_cached_values = sorted(params_with_cached_values)
-        root_cache_item.params_with_cached_values = params_with_cached_values
-        self.root_cache[None] = root_cache_item
+        self.params_with_cached_values_cache.set_value(params_with_cached_values)
 
     def get_path_arg_parser(self, url: str, use_requires: bool, url_desc: Optional[str] = None) \
             -> argparse.ArgumentParser:
-        url = url
-        methods = self.methods_cache[url]
+        methods = self.methods_cache[url].methods
         arg_parser = get_arg_parser()
         url_subparsers = arg_parser.add_subparsers(dest='url', required=True)
         url_parser = url_subparsers.add_parser(url, help=url_desc)
         method_subparsers = url_parser.add_subparsers(dest='method', required=True)
         for method in methods:
             endpoint = self.endpoint_cache[url, method]
             method_desc = endpoint.description or endpoint.summary
@@ -899,34 +959,35 @@
         if index == 0:
             items_to_return.append(CompletionItem(tag='carl', description=None))
         elif index == 1:
             # this means it's either the url or "utils"
             prefix: str = words_[1] or ''
             if UTILS_COMPLETION_ITEM.tag.lower().startswith(prefix.lower()):
                 items_to_return.append(UTILS_COMPLETION_ITEM)
-            root_cache = self.root_cache.get(None, None)
-            if root_cache:
-                possible_urls = root_cache.urls
-            else:
-                possible_urls = []
+            possible_urls = self.urls_cache.get_value()
             for possible_url in possible_urls:
                 if possible_url.url.lower().startswith(prefix.lower()):
                     description = possible_url.summary or possible_url.description
                     items_to_return.append(CompletionItem(
                         tag=possible_url.url,
                         description=description
                     ))
         elif index >= 2 and words_[1] == UTILS_COMPLETION_ITEM.tag:
             items_to_return = list(self.get_util_completions(index - 2, words_[2:]))
         elif index == 2:
             # this means it's a method
             url = words_[1]
             prefix = words_[2]
 
-            possible_methods: List[Method] = self.methods_cache.get(url, [])
+            cached_methods = self.methods_cache.get(url, None)
+            possible_methods: List[Method]
+            if cached_methods is not None:
+                possible_methods = cached_methods.methods
+            else:
+                possible_methods = []
 
             for method in possible_methods:
                 if method.value.lower().startswith(prefix.lower()):
                     endpoint = self.endpoint_cache[url, method]
                     description = endpoint.summary or endpoint.description
                     items_to_return.append(CompletionItem(
                         tag=method.value,
@@ -1040,32 +1101,31 @@
                     if tag.lower().startswith(prefix.lower()):
                         yield CompletionItem(
                             tag=tag,
                             description=param.description
                         )
 
     def get_params_with_cached_values(self) -> Iterable[str]:
-        root_cache_item = self.root_cache[None]
-        return root_cache_item.params_with_cached_values
+        return self.params_with_cached_values_cache.get_value()
 
     def get_util_completions(self, index: int, words: List[str]) -> Iterable[CompletionItem]:
         def _from_list(prefix: str, completions_list: List[CompletionItem]) -> Iterable[CompletionItem]:
             for completion in completions_list:
                 if completion.tag.startswith(prefix):
                     yield completion
 
         if index == 0:
             yield from _from_list(words[0], UTIL_TYPE_COMPLETIONS)
         elif index == 1 and words[0] == VALUES_COMPLETION.tag:
             yield from _from_list(words[1], VALUE_TYPES_COMPLETION)
         elif index == 2 and words[1] in (
                 VALUES_LS_COMPLETION.tag, VALUES_RM_COMPLETION.tag, VALUES_ADD_COMPLETION.tag
         ):
-            root_item = self.root_cache[None]
-            for param_name in root_item.params_with_cached_values:
+            params_with_cached_values = self.params_with_cached_values_cache.get_value()
+            for param_name in params_with_cached_values:
                 if param_name.startswith(words[2]):
                     yield CompletionItem(
                         tag=param_name,
                         description=None
                     )
         elif index == 3 and words[1] == VALUES_RM_COMPLETION.tag:
             yield from self.get_completions_for_values_for_param(
@@ -1088,19 +1148,19 @@
             existing_value_str = param_value_to_str(existing_value)
             if existing_value_str != value:
                 new_values.append(existing_value_str)
         self.arg_value_cache[param_name] = new_values
 
         if len(new_values) == 0:
             # remove from the list of params with cached values
-            root_cache_item = self.root_cache[None]
-            root_cache_item.params_with_cached_values = [
-                p for p in root_cache_item.params_with_cached_values if p != param_name
+            params_with_cached_values = self.params_with_cached_values_cache.get_value()
+            params_with_cached_values = [
+                p for p in params_with_cached_values if p != param_name
             ]
-            self.root_cache[None] = root_cache_item
+            self.params_with_cached_values_cache.set_value(params_with_cached_values)
 
     def add_values(self, param_name: str, values: List[str]) -> None:
         # it's easiest to use cache_param_arg_pairs() to be consistent
         # with how we cache these, though we might want to refactor this to be less awkward
         # at some point
         arg_pairs: ArgPairs = []
         param = CarlParam(
@@ -1259,16 +1319,16 @@
         return None
 
 
 class ArgCache(FileCache[str, List[ParamValue]]):
     def freeze(self, value: List[ParamValue]) -> str:
         return json.dumps(value)
 
-    def thaw(self, frozen_value: str) -> List[ParamValue]:
-        return cast(List[ParamValue], json.loads(frozen_value))
+    def thaw(self, frozen_value: io.TextIOWrapper) -> List[ParamValue]:
+        return cast(List[ParamValue], json.loads(frozen_value.read()))
 
     def freeze_key(self, key: str) -> str:
         return key
 
 
 def format_post_data(param_args: ArgPairs, initial_post_data: Dict[str, Any]) -> Tuple[List[str], ArgPairs]:
     remaining_argpairs: ArgPairs = []
```

### Comparing `curl_arguments_url-0.1.2/curl_arguments_url.egg-info/PKG-INFO` & `curl_arguments_url-0.1.3/curl_arguments_url.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curl-arguments-url
-Version: 0.1.2
+Version: 0.1.3
 Summary: Curl with Arguments for Url
 Home-page: https://github.com/valmikirao/curl_arguments_url
 Author: Valmiki Rao
 Author-email: valmikirao@gmail.com
 License: Apache Software License 2.0
 Keywords: curl_arguments_url,carl,curl,zsh,completions,swagger,openapi
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: ryaml
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # AWS Cloudwatch Insights
 
 ![version](https://img.shields.io/pypi/v/curl_arguments_url)
 ![python versions](https://img.shields.io/pypi/pyversions/curl_arguments_url)
@@ -48,14 +49,20 @@
 % pip install 'curl_arguments_url'
 
 # to get the completions to work, add the following to your .zshrc
 eval "$(carl utils zsh-print-script)"
 
 # And copy the OpenAPI spec into ~/.carl/open_api to get the completions and curl-building working
 % cp open_api-spec.yml ~/.carl/open_api
+
+# if parsing of the open_api files is too slow for you, you can try installing the ryaml (Rust Yaml) extension. I
+# didn't include this by default because I'm afraid it might not install correctly on certain systems, but it's much
+# faster
+% pipx install 'curl_arguments_url[ryaml]'
+ 
 ```
 
 ### Examples
 
 These examples use [tests/resources/open_api/openapi-demo.yml](tests/resources/open_api/openapi-demo.yml)
 
 * Basic GET
@@ -180,14 +187,19 @@
 ```text
     CARL_DIR: Directory which contains files for carl. Default: ~/.carl
     CARL_OPEN_API_DIR: Directory containing the OpenApi specifications and
                         Yaml files. Default: $CARL_DIR/open_api
     CARL_CACHE_DIR: Directory containing the cache. Default $CARL_DIR/cache
 ```
 
+### Hints for finding OpenAPI specs
+
+The spec you're interested in might be on https://app.swaggerhub.com/.  Also, sometimes the doc/sandbox page, for an
+api, which gives you a gui for interacting with the api, loads the swagger spec in the background.  You can see this
+if you open the developer tools in Chrome under Network
 
 ## Development
 
 Requires make:
 
 ```shell
 # setting up dev environment
```

### Comparing `curl_arguments_url-0.1.2/setup.py` & `curl_arguments_url-0.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,19 @@
 
 readme = _read_file('README.md')
 version = _read_file('version.txt')
 
 requirements = [
     'PyYAML>=6.0.0,<7.0.0',
     'jsonref>=1.1.0,<2.0.0',
-    'openapi-schema-pydantic>=1.2.4,<2.0.0'
+    'pydantic>=1.10.7,<2.0.0'
+]
+
+ryaml_requirements = [
+    'ryaml>=0.4.0,<1.0.0'
 ]
 
 setup(
     author="Valmiki Rao",
     author_email='valmikirao@gmail.com',
     python_requires='>=3.7',
     classifiers=[
@@ -42,14 +46,17 @@
     description="Curl with Arguments for Url",
     entry_points={
         'console_scripts': [
             'carl=curl_arguments_url.cli:main',
         ],
     },
     install_requires=requirements,
+    extras_require={
+        'ryaml': ryaml_requirements
+    },
     license="Apache Software License 2.0",
     long_description=readme,
     long_description_content_type='text/markdown',
     include_package_data=True,
     keywords='curl_arguments_url,carl,curl,zsh,completions,swagger,openapi',
     name='curl_arguments_url',
     packages=find_packages(include=['curl_arguments_url', 'curl_arguments_url.*']),
```

