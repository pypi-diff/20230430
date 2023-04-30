# Comparing `tmp/devpytools-0.1.0.dev3.tar.gz` & `tmp/devpytools-0.1.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\devpytools-0.1.0.dev3.tar", last modified: Mon Oct 10 20:08:30 2022, max compression
+gzip compressed data, was "dist\devpytools-0.1.0.dev4.tar", last modified: Sun Apr 30 16:03:47 2023, max compression
```

## Comparing `devpytools-0.1.0.dev3.tar` & `devpytools-0.1.0.dev4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-10-10 20:08:30.535954 devpytools-0.1.0.dev3/
--rw-rw-rw-   0        0        0     1950 2022-10-05 19:38:35.000000 devpytools-0.1.0.dev3/.gitignore
--rw-rw-rw-   0        0        0     1085 2022-04-16 14:06:14.000000 devpytools-0.1.0.dev3/LICENSE
--rw-rw-rw-   0        0        0     1012 2022-10-10 20:08:30.533773 devpytools-0.1.0.dev3/PKG-INFO
--rw-rw-rw-   0        0        0     2090 2022-10-10 18:08:47.000000 devpytools-0.1.0.dev3/README.md
-drwxrwxrwx   0        0        0        0 2022-10-10 20:08:30.409270 devpytools-0.1.0.dev3/devpytools/
--rw-rw-rw-   0        0        0       45 2022-04-23 18:37:52.000000 devpytools-0.1.0.dev3/devpytools/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-10 20:08:30.514479 devpytools-0.1.0.dev3/devpytools/cacher/
--rw-rw-rw-   0        0        0      154 2022-10-09 09:16:26.000000 devpytools-0.1.0.dev3/devpytools/cacher/__init__.py
--rw-rw-rw-   0        0        0     2785 2022-10-10 18:41:26.000000 devpytools-0.1.0.dev3/devpytools/cacher/cache_provider.py
--rw-rw-rw-   0        0        0     8101 2022-10-10 19:19:51.000000 devpytools-0.1.0.dev3/devpytools/cacher/cacher.py
--rw-rw-rw-   0        0        0      654 2022-10-05 20:22:46.000000 devpytools-0.1.0.dev3/devpytools/cacher/extensions.py
--rw-rw-rw-   0        0        0       72 2022-10-09 09:13:32.000000 devpytools-0.1.0.dev3/devpytools/cacher/general.py
-drwxrwxrwx   0        0        0        0 2022-10-10 20:08:30.520328 devpytools-0.1.0.dev3/devpytools/other/
--rw-rw-rw-   0        0        0       34 2022-04-23 18:37:34.000000 devpytools-0.1.0.dev3/devpytools/other/__init__.py
--rw-rw-rw-   0        0        0     1408 2022-10-10 19:40:39.000000 devpytools-0.1.0.dev3/devpytools/other/replace.py
-drwxrwxrwx   0        0        0        0 2022-10-10 20:08:30.463344 devpytools-0.1.0.dev3/devpytools.egg-info/
--rw-rw-rw-   0        0        0     1012 2022-10-10 20:08:29.000000 devpytools-0.1.0.dev3/devpytools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      541 2022-10-10 20:08:29.000000 devpytools-0.1.0.dev3/devpytools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-10 20:08:29.000000 devpytools-0.1.0.dev3/devpytools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-10-10 20:08:29.000000 devpytools-0.1.0.dev3/devpytools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2022-10-10 20:08:29.000000 devpytools-0.1.0.dev3/devpytools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-10-10 20:08:29.000000 devpytools-0.1.0.dev3/devpytools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-10 20:08:30.535954 devpytools-0.1.0.dev3/setup.cfg
--rw-rw-rw-   0        0        0     1305 2022-10-10 18:29:53.000000 devpytools-0.1.0.dev3/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-10 20:08:30.530777 devpytools-0.1.0.dev3/tests/
--rw-rw-rw-   0        0        0        0 2022-04-18 15:01:59.000000 devpytools-0.1.0.dev3/tests/__init__.py
--rw-rw-rw-   0        0        0     7239 2022-10-10 19:45:53.000000 devpytools-0.1.0.dev3/tests/test_cacher.py
--rw-rw-rw-   0        0        0      720 2022-10-10 19:39:51.000000 devpytools-0.1.0.dev3/tests/test_other.py
--rw-rw-rw-   0        0        0      183 2022-10-10 19:56:35.000000 devpytools-0.1.0.dev3/tox.ini
+drwxrwxrwx   0        0        0        0 2023-04-30 16:03:47.615880 devpytools-0.1.0.dev4/
+-rw-rw-rw-   0        0        0     1950 2022-10-05 19:38:35.000000 devpytools-0.1.0.dev4/.gitignore
+-rw-rw-rw-   0        0        0     1085 2022-04-16 14:06:14.000000 devpytools-0.1.0.dev4/LICENSE
+-rw-rw-rw-   0        0        0     3950 2023-04-30 16:03:47.609894 devpytools-0.1.0.dev4/PKG-INFO
+-rw-rw-rw-   0        0        0     2144 2023-04-30 14:53:21.000000 devpytools-0.1.0.dev4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 16:03:47.484230 devpytools-0.1.0.dev4/devpytools/
+-rw-rw-rw-   0        0        0       45 2022-04-23 18:37:52.000000 devpytools-0.1.0.dev4/devpytools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:03:47.586961 devpytools-0.1.0.dev4/devpytools/cacher/
+-rw-rw-rw-   0        0        0      154 2022-10-09 09:16:26.000000 devpytools-0.1.0.dev4/devpytools/cacher/__init__.py
+-rw-rw-rw-   0        0        0     2785 2022-10-10 18:41:26.000000 devpytools-0.1.0.dev4/devpytools/cacher/cache_provider.py
+-rw-rw-rw-   0        0        0     8201 2023-04-30 14:44:50.000000 devpytools-0.1.0.dev4/devpytools/cacher/cacher.py
+-rw-rw-rw-   0        0        0      654 2022-10-05 20:22:46.000000 devpytools-0.1.0.dev4/devpytools/cacher/extensions.py
+-rw-rw-rw-   0        0        0       72 2022-10-09 09:13:32.000000 devpytools-0.1.0.dev4/devpytools/cacher/general.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:03:47.592940 devpytools-0.1.0.dev4/devpytools/other/
+-rw-rw-rw-   0        0        0       34 2022-04-23 18:37:34.000000 devpytools-0.1.0.dev4/devpytools/other/__init__.py
+-rw-rw-rw-   0        0        0     1408 2022-10-10 19:40:39.000000 devpytools-0.1.0.dev4/devpytools/other/replace.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:03:47.564017 devpytools-0.1.0.dev4/devpytools.egg-info/
+-rw-rw-rw-   0        0        0     3950 2023-04-30 16:03:46.000000 devpytools-0.1.0.dev4/devpytools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      541 2023-04-30 16:03:47.000000 devpytools-0.1.0.dev4/devpytools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 16:03:46.000000 devpytools-0.1.0.dev4/devpytools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-10-10 20:08:29.000000 devpytools-0.1.0.dev4/devpytools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-04-30 16:03:46.000000 devpytools-0.1.0.dev4/devpytools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-30 16:03:46.000000 devpytools-0.1.0.dev4/devpytools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 16:03:47.616879 devpytools-0.1.0.dev4/setup.cfg
+-rw-rw-rw-   0        0        0     1426 2023-04-30 16:03:24.000000 devpytools-0.1.0.dev4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:03:47.606902 devpytools-0.1.0.dev4/tests/
+-rw-rw-rw-   0        0        0        0 2022-04-18 15:01:59.000000 devpytools-0.1.0.dev4/tests/__init__.py
+-rw-rw-rw-   0        0        0     7239 2022-10-10 19:45:53.000000 devpytools-0.1.0.dev4/tests/test_cacher.py
+-rw-rw-rw-   0        0        0      720 2022-10-10 19:39:51.000000 devpytools-0.1.0.dev4/tests/test_other.py
+-rw-rw-rw-   0        0        0      183 2022-10-10 19:56:35.000000 devpytools-0.1.0.dev4/tox.ini
```

### Comparing `devpytools-0.1.0.dev3/.gitignore` & `devpytools-0.1.0.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `devpytools-0.1.0.dev3/LICENSE` & `devpytools-0.1.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `devpytools-0.1.0.dev3/README.md` & `devpytools-0.1.0.dev4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -61,22 +61,22 @@
     ...
 
 # cache only those calls that return more than 0 elements
 @devCacher.cache(isSavable=lambda result: result['count'] > 0)
 def a3(b):
     ...
 
-# use only args a and b to determine uniqueness
+# use only a and b arguments to determine unique key of the function call
 @devCacher.cache(uniqueKey=lambda args: args['a'] + args['b'])
 def a4(a: str, b: str, c: str):
     ...
 ```
 ```python
 c = getCacher()
-# use to determine uniqueness only args a and b
+# to determine the uniqueness of a function call use only a and b arguments
 @c.cache(uniqueKey=("a", "b"))
 def a(a, b, c):
     ...
 ```
 
 ### Other
 - replaceFunc
```

### Comparing `devpytools-0.1.0.dev3/devpytools/cacher/cache_provider.py` & `devpytools-0.1.0.dev4/devpytools/cacher/cache_provider.py`

 * *Files identical despite different names*

### Comparing `devpytools-0.1.0.dev3/devpytools/cacher/cacher.py` & `devpytools-0.1.0.dev4/devpytools/cacher/cacher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import hashlib
 import inspect
+import json
 from os import PathLike
-from typing import Any, Callable, Iterable, List, Optional, Dict, Tuple, TypeVar, Union, cast, overload
+import re
+from typing import Any, Callable, Iterable, List, Optional, Dict, Tuple, TypeVar, Union, cast, overload, Sequence
 from functools import wraps
 from collections import OrderedDict
 
 from pydashlite import pickPlain
 
 from .general import _NoValue
 from .cache_provider import CacheProviderABC, FileCacheProvider, InMemoryCacheProvider
@@ -13,21 +15,23 @@
 
 UniqueKeyType = Callable[["OrderedDict[str, Any]"], str]
 
 FuncType = TypeVar('FuncType', bound=Callable[..., Any])
 
 CACHER_MAP: Dict[Optional[str], "Cacher"] = {}
 
+FuncResult = Any
+
 
 class Cacher:
     def __init__(self, *, name: Optional[str] = None, tmpDirPath: Optional[Union[str, PathLike]] = None,
                  isExpired: Optional[Callable[[int, Any], bool]] = None, isLocal=False,
-                 uniqueKey: Optional[Union[UniqueKeyType, Iterable[str]]] = None, isEnable: bool = True,
+                 uniqueKey: Optional[Union[UniqueKeyType, Sequence[str]]] = None, isEnable: bool = True,
                  cacheProvider: Optional[CacheProviderABC] = None,
-                 isSavable: Optional[Callable[[Any], bool]] = lambda x: bool(x),
+                 isSavable: Optional[Callable[[FuncResult], bool]] = lambda x: bool(x),
                  version=1,
                  **kwargs) -> None:
         '''
         caches results of wrapped time consuming function to accelerate development process
         for other dependent functions
         @param name:
             name what will be used to get this cacher by getCacher, should be unique
@@ -94,52 +98,53 @@
             return self._getArgsHash(self._getArgs(arguments))
 
     def _getArgs(self, arguments) -> List[Tuple]:
         res = []
         for k, v in arguments.items():
             if k == 'self':
                 continue
-            if isinstance(v, (str, int, float)):
-                res.append((k, v))
-                continue
-            try:
-                v = tuple(v)
-                if any(not isinstance(x, (str, int, float)) for x in v):
-                    continue
-                res.append((k, v))
-            except:  # noqa
-                res.append((k,))
+            res.append((k, v))
         return res
 
+    delMemPat = re.compile(r'object at (\S+)>')
+
+    def __defaultSerializeArgs(self, value):
+        try:
+            return value.__dict__
+        except:  # noqa
+            pass
+        return self.delMemPat.sub('', str(value))
+
     def _getArgsHash(self, arguments) -> str:
-        return hashlib.sha256((";".join(map(str, arguments))).encode()).hexdigest()
+        return hashlib.sha256((";".join(map(lambda x: json.dumps(x, default=self.__defaultSerializeArgs),
+                                            arguments))).encode()).hexdigest()
 
     @overload
     def cache(self, func: FuncType, *, tmpDirPath: Optional[Union[str, PathLike]] = None,
               isExpired: Optional[Callable[[int, Any], bool]] = None,
               uniqueKey: Optional[Union[UniqueKeyType, Iterable[str]]] = None, isEnable: bool = True,
               cacheProvider: Optional[CacheProviderABC] = None,
-              isSavable: Optional[Callable[[Any], bool]] = None,
+              isSavable: Optional[Callable[[FuncResult], bool]] = None,
               version=1,) -> FuncType:
         ...
 
     @overload
     def cache(self, func=None, *, tmpDirPath: Optional[Union[str, PathLike]] = None,
               isExpired: Optional[Callable[[int, Any], bool]] = None,
               uniqueKey: Optional[Union[UniqueKeyType, Iterable[str]]] = None, isEnable: bool = True,
               cacheProvider: Optional[CacheProviderABC] = None,
-              isSavable: Optional[Callable[[Any], bool]] = None,
+              isSavable: Optional[Callable[[FuncResult], bool]] = None,
               version=1,) -> Callable[[FuncType], FuncType]:
         ...
 
     def cache(self, func: Optional[FuncType] = None, *, tmpDirPath: Optional[Union[str, PathLike]] = None,
               isExpired: Optional[Callable[[int, Any], bool]] = None,
               uniqueKey: Optional[Union[UniqueKeyType, Iterable[str]]] = None, isEnable: bool = True,
               cacheProvider: Optional[CacheProviderABC] = None,
-              isSavable: Optional[Callable[[Any], bool]] = None,
+              isSavable: Optional[Callable[[FuncResult], bool]] = None,
               version=1,):
         '''
         when additional params is passed creates new local Cacher object that merges original Cacher params and the new
         '''
         if not func:
             signature = inspect.signature(self.cache)
             kwargs = {k: v for k, v in locals().items() if k in signature.parameters}
@@ -175,15 +180,15 @@
 
 
 CACHER_MAP[None] = Cacher()
 
 
 def getCacher(name: Optional[str] = None):
     '''
-    returns previously initiated cacher by name or returns default if none found
+    returns previously initiated cacher by name or returns a default if none is found
     >>> cacher = getCacher()
 
     >>> @cacher.cache()
     >>> def a(b):
     >>>     ...
     # or
     >>> @cacher.cache(tmpDirPath='./tmp')
```

### Comparing `devpytools-0.1.0.dev3/devpytools/cacher/extensions.py` & `devpytools-0.1.0.dev4/devpytools/cacher/extensions.py`

 * *Files identical despite different names*

### Comparing `devpytools-0.1.0.dev3/devpytools/other/replace.py` & `devpytools-0.1.0.dev4/devpytools/other/replace.py`

 * *Files identical despite different names*

### Comparing `devpytools-0.1.0.dev3/devpytools.egg-info/SOURCES.txt` & `devpytools-0.1.0.dev4/devpytools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devpytools-0.1.0.dev3/setup.py` & `devpytools-0.1.0.dev4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='devpytools',
-    version='0.1.0.dev3',
+    version='0.1.0.dev4',
     description='Various dev tools.',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     url='https://github.com/glowlex/devpytools',
     author='glowlex',
     author_email='antonioavocado777@gmail.com',
     license='MIT',
-    packages=find_packages(exclude=['tests']),
+    packages=find_packages(include=['devpytools', 'devpytools.*']),
     zip_safe=False,
     test_suite="tests",
     setup_requires=['pytest-runner'],
     tests_require=['pytest'],
     install_requires=[
         "pydashlite",  # 0.1.5
     ],
```

### Comparing `devpytools-0.1.0.dev3/tests/test_cacher.py` & `devpytools-0.1.0.dev4/tests/test_cacher.py`

 * *Files identical despite different names*

### Comparing `devpytools-0.1.0.dev3/tests/test_other.py` & `devpytools-0.1.0.dev4/tests/test_other.py`

 * *Files identical despite different names*

