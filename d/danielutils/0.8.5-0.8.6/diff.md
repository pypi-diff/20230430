# Comparing `tmp/danielutils-0.8.5.tar.gz` & `tmp/danielutils-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danielutils-0.8.5.tar", last modified: Thu Apr 20 20:48:55 2023, max compression
+gzip compressed data, was "danielutils-0.8.6.tar", last modified: Sat Apr 29 22:22:51 2023, max compression
```

## Comparing `danielutils-0.8.5.tar` & `danielutils-0.8.6.tar`

### file list

```diff
@@ -1,53 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 20:48:55.962430 danielutils-0.8.5/
--rw-rw-rw-   0        0        0      939 2023-04-20 20:48:55.962430 danielutils-0.8.5/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-04-20 20:48:55.000000 danielutils-0.8.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 20:48:55.930903 danielutils-0.8.5/danielutils/
-drwxrwxrwx   0        0        0        0 2023-04-20 20:48:55.947604 danielutils-0.8.5/danielutils/Classes/
--rw-rw-rw-   0        0        0      210 2023-04-20 17:59:42.000000 danielutils-0.8.5/danielutils/Classes/Convenience.py
--rw-rw-rw-   0        0        0     3904 2023-04-20 20:37:29.000000 danielutils-0.8.5/danielutils/Classes/TypedBuiltins.py
--rw-rw-rw-   0        0        0      107 2023-04-20 18:11:11.000000 danielutils-0.8.5/danielutils/Classes/__init__.py
--rw-rw-rw-   0        0        0     1027 2023-04-20 20:24:10.000000 danielutils-0.8.5/danielutils/Classes/frange.py
--rw-rw-rw-   0        0        0     3983 2023-04-20 17:12:55.000000 danielutils-0.8.5/danielutils/Colors.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:48:55.949101 danielutils-0.8.5/danielutils/Conversions/
--rw-rw-rw-   0        0        0     2227 2023-04-20 19:56:42.000000 danielutils-0.8.5/danielutils/Conversions/MainConversions.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:48:55.952538 danielutils-0.8.5/danielutils/Conversions/SpecializedConversions/
--rw-rw-rw-   0        0        0       46 2022-10-14 16:36:49.000000 danielutils-0.8.5/danielutils/Conversions/SpecializedConversions/__init__.py
--rw-rw-rw-   0        0        0      476 2023-04-20 20:15:32.000000 danielutils-0.8.5/danielutils/Conversions/SpecializedConversions/to_hex.py
--rw-rw-rw-   0        0        0      407 2023-04-20 17:57:46.000000 danielutils-0.8.5/danielutils/Conversions/SpecializedConversions/to_int.py
--rw-rw-rw-   0        0        0       71 2022-10-14 16:31:17.000000 danielutils-0.8.5/danielutils/Conversions/__init__.py
--rw-rw-rw-   0        0        0      631 2023-04-20 17:15:00.000000 danielutils-0.8.5/danielutils/Data.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:48:55.957603 danielutils-0.8.5/danielutils/DataStructures/
--rw-rw-rw-   0        0        0     1569 2023-04-20 20:36:21.000000 danielutils-0.8.5/danielutils/DataStructures/Comparer.py
--rw-rw-rw-   0        0        0     3299 2023-04-20 20:00:10.000000 danielutils-0.8.5/danielutils/DataStructures/Heap.py
--rw-rw-rw-   0        0        0    10238 2023-04-20 20:35:30.000000 danielutils-0.8.5/danielutils/DataStructures/Interface.py
--rw-rw-rw-   0        0        0      412 2023-04-20 20:11:14.000000 danielutils-0.8.5/danielutils/DataStructures/Node.py
--rw-rw-rw-   0        0        0     4364 2023-04-20 20:34:31.000000 danielutils-0.8.5/danielutils/DataStructures/Queue.py
--rw-rw-rw-   0        0        0      115 2023-04-20 20:05:37.000000 danielutils-0.8.5/danielutils/DataStructures/__init__.py
--rw-rw-rw-   0        0        0      607 2023-04-20 20:07:14.000000 danielutils-0.8.5/danielutils/DataStructures/functions.py
--rw-rw-rw-   0        0        0    16029 2023-04-20 20:29:28.000000 danielutils-0.8.5/danielutils/Decorators.py
--rw-rw-rw-   0        0        0     2127 2023-04-20 19:47:46.000000 danielutils-0.8.5/danielutils/Exceptions.py
--rw-rw-rw-   0        0        0     5372 2023-04-20 20:44:36.000000 danielutils-0.8.5/danielutils/Functions.py
--rw-rw-rw-   0        0        0     9251 2023-04-20 19:48:57.000000 danielutils-0.8.5/danielutils/IO.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:48:55.960923 danielutils-0.8.5/danielutils/Math/
--rw-rw-rw-   0        0        0     7682 2023-04-20 20:14:55.000000 danielutils-0.8.5/danielutils/Math/Constants.py
--rw-rw-rw-   0        0        0      347 2023-04-20 20:10:18.000000 danielutils-0.8.5/danielutils/Math/Functions.py
--rw-rw-rw-   0        0        0     1045 2023-04-20 18:34:15.000000 danielutils-0.8.5/danielutils/Math/MathPrint.py
--rw-rw-rw-   0        0        0     3779 2023-04-20 17:25:45.000000 danielutils-0.8.5/danielutils/Math/MathSymbols.py
--rw-rw-rw-   0        0        0       80 2023-04-03 18:56:40.000000 danielutils-0.8.5/danielutils/Math/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-01-12 01:01:37.000000 danielutils-0.8.5/danielutils/Path.py
--rw-rw-rw-   0        0        0     2686 2023-04-11 13:05:54.000000 danielutils-0.8.5/danielutils/Print.py
--rw-rw-rw-   0        0        0     6089 2023-04-20 19:51:00.000000 danielutils-0.8.5/danielutils/System.py
--rw-rw-rw-   0        0        0     4204 2023-04-20 18:50:09.000000 danielutils-0.8.5/danielutils/Text.py
--rw-rw-rw-   0        0        0      612 2023-04-20 19:52:02.000000 danielutils-0.8.5/danielutils/Threading.py
--rw-rw-rw-   0        0        0      426 2023-04-11 21:07:07.000000 danielutils-0.8.5/danielutils/Time.py
--rw-rw-rw-   0        0        0     2138 2023-04-20 19:32:32.000000 danielutils-0.8.5/danielutils/Windows.py
--rw-rw-rw-   0        0        0      555 2023-04-20 20:23:42.000000 danielutils-0.8.5/danielutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:48:55.945605 danielutils-0.8.5/danielutils.egg-info/
--rw-rw-rw-   0        0        0      939 2023-04-20 20:48:55.000000 danielutils-0.8.5/danielutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1320 2023-04-20 20:48:55.000000 danielutils-0.8.5/danielutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 20:48:55.000000 danielutils-0.8.5/danielutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-20 20:48:55.000000 danielutils-0.8.5/danielutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-20 20:48:55.000000 danielutils-0.8.5/danielutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      728 2023-04-20 20:48:55.000000 danielutils-0.8.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-20 20:48:55.962430 danielutils-0.8.5/setup.cfg
--rw-rw-rw-   0        0        0     1340 2023-04-20 20:48:55.000000 danielutils-0.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.977510 danielutils-0.8.6/
+-rw-rw-rw-   0        0        0     1967 2023-04-29 22:22:51.977510 danielutils-0.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1259 2023-04-29 22:22:51.000000 danielutils-0.8.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.915449 danielutils-0.8.6/danielutils/
+drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.941274 danielutils-0.8.6/danielutils/Classes/
+-rw-rw-rw-   0        0        0      210 2023-04-20 17:59:42.000000 danielutils-0.8.6/danielutils/Classes/Convenience.py
+-rw-rw-rw-   0        0        0     4612 2023-04-21 07:35:02.000000 danielutils-0.8.6/danielutils/Classes/TypedBuiltins.py
+-rw-rw-rw-   0        0        0      107 2023-04-20 18:11:11.000000 danielutils-0.8.6/danielutils/Classes/__init__.py
+-rw-rw-rw-   0        0        0     1027 2023-04-20 20:24:10.000000 danielutils-0.8.6/danielutils/Classes/frange.py
+-rw-rw-rw-   0        0        0     3992 2023-04-29 17:53:23.000000 danielutils-0.8.6/danielutils/Colors.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.943279 danielutils-0.8.6/danielutils/Conversions/
+-rw-rw-rw-   0        0        0     2227 2023-04-20 19:56:42.000000 danielutils-0.8.6/danielutils/Conversions/MainConversions.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.946339 danielutils-0.8.6/danielutils/Conversions/SpecializedConversions/
+-rw-rw-rw-   0        0        0       46 2022-10-14 16:36:49.000000 danielutils-0.8.6/danielutils/Conversions/SpecializedConversions/__init__.py
+-rw-rw-rw-   0        0        0      476 2023-04-20 20:15:32.000000 danielutils-0.8.6/danielutils/Conversions/SpecializedConversions/to_hex.py
+-rw-rw-rw-   0        0        0      407 2023-04-20 17:57:46.000000 danielutils-0.8.6/danielutils/Conversions/SpecializedConversions/to_int.py
+-rw-rw-rw-   0        0        0       71 2022-10-14 16:31:17.000000 danielutils-0.8.6/danielutils/Conversions/__init__.py
+-rw-rw-rw-   0        0        0      631 2023-04-20 17:15:00.000000 danielutils-0.8.6/danielutils/Data.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.951878 danielutils-0.8.6/danielutils/DataStructures/
+-rw-rw-rw-   0        0        0     1569 2023-04-20 20:36:21.000000 danielutils-0.8.6/danielutils/DataStructures/Comparer.py
+-rw-rw-rw-   0        0        0     3299 2023-04-20 20:00:10.000000 danielutils-0.8.6/danielutils/DataStructures/Heap.py
+-rw-rw-rw-   0        0        0      412 2023-04-20 20:11:14.000000 danielutils-0.8.6/danielutils/DataStructures/Node.py
+-rw-rw-rw-   0        0        0     4428 2023-04-27 14:48:46.000000 danielutils-0.8.6/danielutils/DataStructures/Queue.py
+-rw-rw-rw-   0        0        0       89 2023-04-29 16:43:01.000000 danielutils-0.8.6/danielutils/DataStructures/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-04-20 20:07:14.000000 danielutils-0.8.6/danielutils/DataStructures/functions.py
+-rw-rw-rw-   0        0        0      135 2023-04-21 22:43:20.000000 danielutils-0.8.6/danielutils/DateTime.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.964499 danielutils-0.8.6/danielutils/Decorators/
+-rw-rw-rw-   0        0        0      696 2023-04-29 17:38:05.000000 danielutils-0.8.6/danielutils/Decorators/PartiallyImplemented.py
+-rw-rw-rw-   0        0        0      335 2023-04-29 21:26:25.000000 danielutils-0.8.6/danielutils/Decorators/__init__.py
+-rw-rw-rw-   0        0        0      601 2023-04-29 17:43:40.000000 danielutils-0.8.6/danielutils/Decorators/atomic.py
+-rw-rw-rw-   0        0        0     1195 2023-04-29 17:44:07.000000 danielutils-0.8.6/danielutils/Decorators/attach.py
+-rw-rw-rw-   0        0        0      730 2023-04-29 17:58:20.000000 danielutils-0.8.6/danielutils/Decorators/chain_decorators.py
+-rw-rw-rw-   0        0        0      845 2023-04-29 17:44:22.000000 danielutils-0.8.6/danielutils/Decorators/decorate_conditionally.py
+-rw-rw-rw-   0        0        0      817 2023-04-29 18:02:16.000000 danielutils-0.8.6/danielutils/Decorators/delay_call.py
+-rw-rw-rw-   0        0        0     1479 2023-04-29 17:44:59.000000 danielutils-0.8.6/danielutils/Decorators/limit_recursion.py
+-rw-rw-rw-   0        0        0      622 2023-04-29 17:38:26.000000 danielutils-0.8.6/danielutils/Decorators/memo.py
+-rw-rw-rw-   0        0        0     3991 2023-04-29 17:46:01.000000 danielutils-0.8.6/danielutils/Decorators/overload.py
+-rw-rw-rw-   0        0        0      595 2023-04-29 17:59:44.000000 danielutils-0.8.6/danielutils/Decorators/threadify.py
+-rw-rw-rw-   0        0        0     1736 2023-04-29 21:25:16.000000 danielutils-0.8.6/danielutils/Decorators/timeout.py
+-rw-rw-rw-   0        0        0     9732 2023-04-29 17:50:06.000000 danielutils-0.8.6/danielutils/Decorators/validate.py
+-rw-rw-rw-   0        0        0     2127 2023-04-20 19:47:46.000000 danielutils-0.8.6/danielutils/Exceptions.py
+-rw-rw-rw-   0        0        0     5564 2023-04-21 15:43:35.000000 danielutils-0.8.6/danielutils/Functions.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.967499 danielutils-0.8.6/danielutils/Generators/
+-rw-rw-rw-   0        0        0       32 2023-04-29 22:08:49.000000 danielutils-0.8.6/danielutils/Generators/__init__.py
+-rw-rw-rw-   0        0        0     1025 2023-04-29 22:18:06.000000 danielutils-0.8.6/danielutils/Generators/join_generators.py
+-rw-rw-rw-   0        0        0     9257 2023-04-26 09:21:09.000000 danielutils-0.8.6/danielutils/IO.py
+-rw-rw-rw-   0        0        0     1846 2023-04-29 17:47:59.000000 danielutils-0.8.6/danielutils/Internet.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.973533 danielutils-0.8.6/danielutils/Math/
+-rw-rw-rw-   0        0        0     7682 2023-04-20 20:14:55.000000 danielutils-0.8.6/danielutils/Math/Constants.py
+-rw-rw-rw-   0        0        0      347 2023-04-20 20:10:18.000000 danielutils-0.8.6/danielutils/Math/Functions.py
+-rw-rw-rw-   0        0        0     1045 2023-04-20 18:34:15.000000 danielutils-0.8.6/danielutils/Math/MathPrint.py
+-rw-rw-rw-   0        0        0     3779 2023-04-20 17:25:45.000000 danielutils-0.8.6/danielutils/Math/MathSymbols.py
+-rw-rw-rw-   0        0        0       80 2023-04-03 18:56:40.000000 danielutils-0.8.6/danielutils/Math/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.976510 danielutils-0.8.6/danielutils/MetaClasses/
+-rw-rw-rw-   0        0        0      742 2023-04-29 17:55:43.000000 danielutils-0.8.6/danielutils/MetaClasses/AtomicClassMeta.py
+-rw-rw-rw-   0        0        0    10395 2023-04-29 17:55:35.000000 danielutils-0.8.6/danielutils/MetaClasses/Interface.py
+-rw-rw-rw-   0        0        0       58 2023-04-29 16:46:20.000000 danielutils-0.8.6/danielutils/MetaClasses/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-01-12 01:01:37.000000 danielutils-0.8.6/danielutils/Path.py
+-rw-rw-rw-   0        0        0     2686 2023-04-11 13:05:54.000000 danielutils-0.8.6/danielutils/Print.py
+-rw-rw-rw-   0        0        0     4529 2023-04-29 15:46:45.000000 danielutils-0.8.6/danielutils/Reflection.py
+-rw-rw-rw-   0        0        0     6089 2023-04-20 19:51:00.000000 danielutils-0.8.6/danielutils/System.py
+-rw-rw-rw-   0        0        0     4213 2023-04-29 18:00:25.000000 danielutils-0.8.6/danielutils/Text.py
+-rw-rw-rw-   0        0        0      426 2023-04-11 21:07:07.000000 danielutils-0.8.6/danielutils/Time.py
+-rw-rw-rw-   0        0        0     2254 2023-04-21 15:17:41.000000 danielutils-0.8.6/danielutils/Windows.py
+-rw-rw-rw-   0        0        0      664 2023-04-29 22:08:58.000000 danielutils-0.8.6/danielutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.935927 danielutils-0.8.6/danielutils.egg-info/
+-rw-rw-rw-   0        0        0     1967 2023-04-29 22:22:51.000000 danielutils-0.8.6/danielutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1986 2023-04-29 22:22:51.000000 danielutils-0.8.6/danielutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 22:22:51.000000 danielutils-0.8.6/danielutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-29 22:22:51.000000 danielutils-0.8.6/danielutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 22:22:51.000000 danielutils-0.8.6/danielutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      728 2023-04-29 22:22:51.000000 danielutils-0.8.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 22:22:51.978839 danielutils-0.8.6/setup.cfg
+-rw-rw-rw-   0        0        0     1389 2023-04-29 22:22:51.000000 danielutils-0.8.6/setup.py
```

### Comparing `danielutils-0.8.5/danielutils/Classes/TypedBuiltins.py` & `danielutils-0.8.6/danielutils/Classes/TypedBuiltins.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 from __future__ import annotations
-from typing import Any, Iterable
+from typing import Any, Iterable, TypeVar, Generator
 from ..Decorators import validate, overload
 from ..Functions import isoftype
 
 
-class tlist(list):
-    """tlist is same as builtin python list but with added type restriction
-
-    Args:
-        type (type): the allowed type, can be nested type
-        iterable (Iterable, optional): the value to create the tlist from. Defaults to None.
-    """
+class TypedClass:
+    def __init__(self, T: type):
+        self.T = T
 
     def _get_error_msg(self, v: Any) -> str:
         """generates the generic error message
 
         Args:
             v (Any): value to include in the message
 
         Returns:
             str: the error message
         """
         return f"A value is of the wrong type:\n'{v}' is of type '{type(v)}' but should be of type '{self.T}'"
 
+
+class tlist(list, TypedClass):
+    """tlist is same as builtin python list but with added type restriction
+
+    Args:
+        type (type): the allowed type, can be nested type
+        iterable (Iterable, optional): the value to create the tlist from. Defaults to None.
+    """
+
     @validate
     def __init__(self, T: type, iterable: Iterable = None):
         """_summary_
 
         Args:
             type (type): the allowed type, can be nested type
         iterable (Iterable, optional): the value to create the tlist from. Defaults to None.
 
         Raises:
             TypeError: _description_
         """
-        self.T = T
+        TypedClass.__init__(T)
         if iterable is not None:
             for v in iterable:
                 if not isoftype(v, T):
                     raise TypeError(self._get_error_msg(v))
-                super().append(v)
+                list.append(v)
 
     def __setitem__(self, index: int, value: Any) -> None:
         if not isoftype(value, self.T):
             raise TypeError(self._get_error_msg(value))
         super()[index] = value
 
     def append(self, value: Any) -> None:
@@ -62,33 +67,34 @@
 
 
 class tdict(dict):
     """like builtin dict but only a specif type is allowed
     """
     @overload(None, type, type)
     def __init__(self, key_t: type, val_t: type):
+
         self.key_t = key_t
         self.val_t = val_t
         super().__init__()
 
     @overload(None, type, type, Iterable)
     def __init__(self, keyt: type, val_t: type, iterable: Iterable[tuple]):
         self.key_t = keyt
         self.val_t = val_t
         super().__init__(iterable)
 
     @overload(None, type, type, dict)
     def __init__(self, key_t: type, val_t: type, ** kwargs):
         """dict(type,type) -> new empty dictionary dict(mapping) -> new dictionary initialized from a mapping object's
-    (key, value) pairs
-dict(type,type,iterable) -> new dictionary initialized as if via:
-    d = {} for k, v in iterable:
-        d[k] = v
-dict(type,type,**kwargs) -> new dictionary initialized with the name=value pairs
-    in the keyword argument list. For example: dict(one=1, two=2)
+                (key, value) pairs
+            dict(type,type,iterable) -> new dictionary initialized as if via:
+                d = {} for k, v in iterable:
+                    d[k] = v
+            dict(type,type,**kwargs) -> new dictionary initialized with the name=value pairs
+                in the keyword argument list. For example: dict(one=1, two=2)
         """
         self.key_t = key_t
         self.val_t = val_t
         super().__init__(**kwargs)
 
     def __setitem__(self, key, value) -> None:
         if not isoftype(key, self.key_t):
@@ -101,20 +107,42 @@
                 f" as value = '{value}' is not of type '{ self.val_t}'")
         super().__setitem__(key, value)
 
     def __str__(self):
         return f"dict[{self.key_t.__name__}, {self.val_t.__name__}]: {super().__str__()}"
 
 
-# TODO tset
-class tset(set):
+T = TypeVar("T")
+
+
+class tset(set, TypedClass):
     """like builtin set but only allows specified type
     """
 
-    def __init__(self):
-        pass
+    def __init__(self, T: T):
+        TypedClass.__init__(T)
+        set.__init__()
+
+    def add(self, v: Any):
+        if isoftype(v, self.T):
+            set.add(v)
+
+    def clone(self) -> tset:
+        res = tset(self.T)
+        for v in self:
+            res.add(v)
+        return res
+
+    def __iter__(self) -> Generator[T, None, None]:
+        yield from set.__iter__()
+
+    def union(self, other: tset) -> tset:
+        res = self.clone()
+        for v in other:
+            res.add(v)
+        return res
 
 
 __all__ = [
     "tlist",
     "tdict"
 ]
```

### Comparing `danielutils-0.8.5/danielutils/Classes/frange.py` & `danielutils-0.8.6/danielutils/Classes/frange.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.5/danielutils/Colors.py` & `danielutils-0.8.6/danielutils/Colors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .Decorators import validate
+from .Decorators.validate import validate
 
 
 class ColoredText:
     """static utility class with static functions:\n
         from_rgb,
         green,
         red,
```

### Comparing `danielutils-0.8.5/danielutils/Conversions/MainConversions.py` & `danielutils-0.8.6/danielutils/Conversions/MainConversions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.5/danielutils/Data.py` & `danielutils-0.8.6/danielutils/Data.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.5/danielutils/DataStructures/Comparer.py` & `danielutils-0.8.6/danielutils/DataStructures/Comparer.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.5/danielutils/DataStructures/Heap.py` & `danielutils-0.8.6/danielutils/DataStructures/Heap.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.5/danielutils/DataStructures/Interface.py` & `danielutils-0.8.6/danielutils/MetaClasses/Interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Callable, Iterable, Any, Generator
 import inspect
 import re
 import traceback
+import functools
+# from ..Decorators.decorate_conditionally import decorate_conditionally
 
 
 class InterfaceHelper:
     """a helper class for Interface metaclass
     """
     ORIGINAL_INIT = "__original_init__"
 
@@ -83,58 +85,54 @@
         """
         src = inspect.getsource(cls).splitlines()
         for line in src:
             if re.match(r".*def \w+\(.*\).*:", line):
                 func_name = re.findall(r".*def (\w+)\(.*", line)[0]
                 yield func_name
 
-    __mro_dict = {}
-
     @staticmethod
-    def create_init_handler(cls_name, missing: list[str] = None):
+    def create_init_handler(cls_name, missing: list[str] = None, original: Callable = None):
         """this function will create the default interface __init__ function with the wanted behavior"""
-
+        # @decorate_conditionally(functools.wraps, original is not None, [original])  # TODO implement this decorator
         def __interface_init__(*args, **kwargs):
             instance = args[0]
-            if instance not in InterfaceHelper.__mro_dict:
-                InterfaceHelper.__mro_dict[instance] = 1
-            else:
-                InterfaceHelper.__mro_dict[instance] += 1
-
             caller_frame = traceback.format_stack()[-2]
             is_super_call = bool(re.match(
-                r"\s+File \".*\", line \d+, in __init__\n\s+super\(\)\.__init__\(.*\)\n", caller_frame))
+                fr"\s+File \".*\", line \d+, in __init__\n\s+(?:super\(\)|{cls_name})\.__init__\(.*\)\n", caller_frame))
             if is_super_call:
                 mro = instance.__class__.mro()
-                for cls in mro[InterfaceHelper.__mro_dict[instance]:]:
+                i = 0
+                for i, cls in enumerate(mro):
+                    if cls.__name__ == cls_name:
+                        break
+                mro = mro[i:]
+                for cls in mro:
                     if hasattr(cls, InterfaceHelper.ORIGINAL_INIT):
                         result = getattr(cls, InterfaceHelper.ORIGINAL_INIT)(
                             *args, **kwargs)
-                        if instance in InterfaceHelper.__mro_dict:
-                            del InterfaceHelper.__mro_dict[instance]
                         return result
                 raise NotImplementedError(
                     f"Can't use super().__init__(...) in {cls_name}.__init__(...) "
                     "if the __init__ function is not defined a parent interface")
 
-            del InterfaceHelper.__mro_dict[instance]
             if missing:
                 raise NotImplementedError(f"Can't instantiate '{cls_name}' because it is an interface."
                                           f" It is missing implementations for {missing}")
             raise NotImplementedError(
                 f"'{cls_name}' is an interface, Can't create instances")
         return __interface_init__
 
     @staticmethod
-    def create_generic_handler(cls: str):
+    def create_generic_handler(cls: str, original: Callable):
         """this function will create the generic function handler
 
         Args:
             func_name (_type_): the name of the interface
         """
+        @functools.wraps(original)
         def __interface_handler__(*args, **kwargs):
             raise NotImplementedError(
                 f"Interface {cls} must be implemented")
         return __interface_handler__
 
 
 class Interface(type):
@@ -153,21 +151,23 @@
 
     def __new__(mcs, name: str, bases: tuple, namespace: dict):
         if len(bases) == 0:
             return mcs._handle_new_interface(mcs, name, bases, namespace)
         return mcs._handle_new_subclass(mcs, name, bases, namespace)
 
     def _handle_new_interface(cls, name: str, bases: tuple, namespace: dict[str, Any]):
+        namespace[InterfaceHelper.ORIGINAL_INIT] = None
         if "__init__" in namespace:
             namespace[InterfaceHelper.ORIGINAL_INIT] = namespace["__init__"]
-        namespace["__init__"] = InterfaceHelper.create_init_handler(name)
+        namespace["__init__"] = InterfaceHelper.create_init_handler(
+            name, original=namespace[InterfaceHelper.ORIGINAL_INIT])
         for k, v in namespace.items():
             if isinstance(v, Callable) and not k == "__init__":
                 if not InterfaceHelper.is_func_implemented(v):
-                    namespace[k] = InterfaceHelper.create_generic_handler(k)
+                    namespace[k] = InterfaceHelper.create_generic_handler(k, v)
         namespace[Interface.KEY] = True
         return super().__new__(cls, name, bases, namespace)
 
     def _handle_new_subclass(cls, name: str, bases: tuple, namespace: dict[str, Any]):
         need_to_be_implemented = set()
         ancestry = set()
         for base in bases:
@@ -231,17 +231,17 @@
             namespace[InterfaceHelper.ORIGINAL_INIT] = namespace["__init__"]
         else:
             if InterfaceHelper.ORIGINAL_INIT in namespace:
                 del namespace[InterfaceHelper.ORIGINAL_INIT]
 
         if missing:
             namespace[Interface.KEY] = True
-            if "__init__" in need_to_be_implemented:
-                namespace["__init__"] = InterfaceHelper.create_init_handler(
-                    name, missing)
+            # if "__init__" in need_to_be_implemented:
+            namespace["__init__"] = InterfaceHelper.create_init_handler(
+                name, missing)
         else:
             namespace[Interface.KEY] = False
             if "__init__" not in namespace:
                 namespace["__init__"] = object.__init__
 
         return super().__new__(cls, name, bases, namespace)
```

### Comparing `danielutils-0.8.5/danielutils/DataStructures/Queue.py` & `danielutils-0.8.6/danielutils/DataStructures/Queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,17 @@
         """returns whether the queue is empty
 
         Returns:
             bool: result
         """
         return len(self) == 0
 
+    def __str__(self) -> str:
+        return str(self.data)
+
 
 class PriorityQueue:
     """
     A priority queue implementation based on a binary heap.
 
     Args:
         weight_func (Callable[[T], int | float], optional): A function to calculate the weight of items added
```

### Comparing `danielutils-0.8.5/danielutils/DataStructures/functions.py` & `danielutils-0.8.6/danielutils/DataStructures/functions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.5/danielutils/Exceptions.py` & `danielutils-0.8.6/danielutils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.5/danielutils/Functions.py` & `danielutils-0.8.6/danielutils/Functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,53 +34,55 @@
     if not isinstance(strict, bool):
         raise TypeError("'strict' must be of type bool")
     obj_origin, obj_args, obj_hints = __isoftype_inquire(obj)
     t_origin, t_args, t_hints = __isoftype_inquire(T)
     if t_origin is not None:
         if t_origin in {list}:
             for sub_v in obj:
-                if not isoftype(sub_v, t_args[0]):
+                if not isoftype(sub_v, t_args[0], strict=strict):
                     return False
             return True
 
         if t_origin is dict:
             key_t, value_t,  = t_args[0], t_args[1]
             for k, v in obj.items():
-                if not isoftype(v, value_t):
+                if not isoftype(v, value_t, strict=strict):
                     return False
-                if not isoftype(k, key_t):
+                if not isoftype(k, key_t, strict=strict):
                     return False
             return True
 
         if t_origin in {Union}:
             for sub_t in t_args:
-                if isoftype(obj, sub_t):
+                if isoftype(obj, sub_t, strict=strict):
                     return True
             return False
 
         if t_origin in {Callable}:
             if obj.__name__ == "<lambda>":
-                print("using lambda function with isoftype is ambiguous")
+                if strict:
+                    from .Colors import warning
+                    warning("using lambda function with isoftype is ambiguous")
                 return not strict
-            tmp = list(obj_hints.values())
-            obj_return_type = tmp[-1]
-            obj_param_types = tuple(tmp[:-1])
-            del tmp
             if len(t_args) == 0:
                 return True
+            tmp = list(obj_hints.values())
+            obj_return_type = tmp[-1] if tmp else None
+            obj_param_types = tuple(tmp[:-1]) if tmp else None
+            del tmp
             t_return_type = t_args[1]
             t_param_types = tuple(t_args[0])
             return obj_return_type is t_return_type and obj_param_types == t_param_types
     else:
         if T is Any:
             return True
 
         if type(T) in {list}:
             for sub_t in T:
-                if isoftype(obj, sub_t):
+                if isoftype(obj, sub_t, strict=strict):
                     return True
             return False
 
         if obj_origin is not None:
             if obj_origin is Union:
                 return T is type(Union)
     return isinstance(obj, T)
```

### Comparing `danielutils-0.8.5/danielutils/IO.py` & `danielutils-0.8.6/danielutils/IO.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,17 +309,17 @@
             end (str, optional): the str to use as the final value. Defaults to "\n".
 
         Raises:
             ValueError: _description_
         """
         if self.output_stream is None:
             raise ValueError(
-                "Can't write to an empty stream. the stream must not be None either by set_stream or by initialization")
+                "Can't write to an empty stream. the stream must not be None: either by set_stream or by initialization")
         self.output_stream.write(
-            self.indent_level*self.indent_value + sep.join(args)+end)
+            str(self.indent_level*self.indent_value + sep.join(args)+end))
 
     def set_stream(self, stream: IO):
         """explicitly sets the stream
 
         Args:
             stream (IO): stream
         """
```

### Comparing `danielutils-0.8.5/danielutils/Math/Constants.py` & `danielutils-0.8.6/danielutils/Math/Constants.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.5/danielutils/Math/MathPrint.py` & `danielutils-0.8.6/danielutils/Math/MathPrint.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.5/danielutils/Math/MathSymbols.py` & `danielutils-0.8.6/danielutils/Math/MathSymbols.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.5/danielutils/Path.py` & `danielutils-0.8.6/danielutils/Path.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.5/danielutils/Print.py` & `danielutils-0.8.6/danielutils/Print.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.5/danielutils/System.py` & `danielutils-0.8.6/danielutils/System.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.5/danielutils/Text.py` & `danielutils-0.8.6/danielutils/Text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 from typing import Union, TypeGuard
-from .Decorators import validate
+from .Decorators.validate import validate
 from .Functions import check_foreach
 HEBREW_LETTERS = ['\u05D0', '\u2135', '\uFB21', '\uFB2E', '\uFB2F',
                   '\uFB30', '\uFB4F', '\u05D1', '\u2136', '\uFB31',
                   '\uFB4C', '\u05D2', '\u2137', '\uFB32', '\u05D3',
                   '\u2138', '\uFB22', '\uFB33', '\u05D4', '\uFB23',
                   '\uFB34', '\u05D5', '\uFB4B', '\uFB35', '\u05F0',
                   '\u05F1', '\u05D6', '\uFB36', '\u05D7', '\u05D8',
```

### Comparing `danielutils-0.8.5/danielutils/Windows.py` & `danielutils-0.8.6/danielutils/Windows.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-from functools import partial
-from screeninfo import get_monitors
-import pyautogui
-from PIL import ImageGrab, Image
-ImageGrab.grab = partial(ImageGrab.grab, all_screens=True)
+# from functools import partial
+# from screeninfo import get_monitors
+# import pyautogui
+# from PIL import ImageGrab, Image
+# ImageGrab.grab = partial(ImageGrab.grab, all_screens=True)
 
 
-def screenshot(xy: tuple[int, int] = (0, 0), wh: tuple[int, int] = None) -> Image:
-    """creates a screenshot of the screen in an arbitrary location and size
+# def screenshot(xy: tuple[int, int] = (0, 0), wh: tuple[int, int] = None) -> Image:
+#     """creates a screenshot of the screen in an arbitrary location and size
 
-    Args:
-        xy (tuple[int, int], optional): the top left location of the screenshot. Defaults to (0, 0).
-        wh (tuple[int, int], optional): the size of the screenshot in pixels. Defaults to None. if None will 
-        create a screen shot of all monitors
-    Returns:
-        Image: _description_
-    """
-    if wh is None:
-        wh = (0, 0)
-        for monitor_index in range(get_monitor_count()):
-            size = get_monitor_size(monitor_index)
-            wh = (wh[0]+size[0], wh[1]+size[1])
-    return pyautogui.screenshot(None, (xy[0], xy[1], wh[0], wh[1]))
+#     Args:
+#         xy (tuple[int, int], optional): the top left location of the screenshot. Defaults to (0, 0).
+#         wh (tuple[int, int], optional): the size of the screenshot in pixels. Defaults to None. if None will 
+#         create a screen shot of all monitors
+#     Returns:
+#         Image: _description_
+#     """
+#     if wh is None:
+#         wh = (0, 0)
+#         for monitor_index in range(get_monitor_count()):
+#             size = get_monitor_size(monitor_index)
+#             wh = (wh[0]+size[0], wh[1]+size[1])
+#     return pyautogui.screenshot(None, (xy[0], xy[1], wh[0], wh[1]))
 
 
-def screenshot_monitor(index: int) -> Image:
-    """creates a screenshot of the monitor
+# def screenshot_monitor(index: int) -> Image:
+#     """creates a screenshot of the monitor
 
-    Args:
-        index (int): the monitor's index
+#     Args:
+#         index (int): the monitor's index
 
-    Returns:
-        Image: the screenshot
-    """
-    return screenshot(get_monitor_location(index), get_monitor_size(index))
+#     Returns:
+#         Image: the screenshot
+#     """
+#     return screenshot(get_monitor_location(index), get_monitor_size(index))
 
 
-def get_monitor_size(index: int) -> tuple[int, int]:
-    """returns the size of the monitor
+# def get_monitor_size(index: int) -> tuple[int, int]:
+#     """returns the size of the monitor
 
-    Args:
-        index (int): the monitor's index
+#     Args:
+#         index (int): the monitor's index
 
-    Returns:
-        tuple[int, int]: the size
-    """
-    monitor = get_monitors()[index]
-    return monitor.width, monitor.height
+#     Returns:
+#         tuple[int, int]: the size
+#     """
+#     monitor = get_monitors()[index]
+#     return monitor.width, monitor.height
 
 
-def get_monitor_location(index: int) -> tuple[int, int]:
-    """returns the coordinates of the location of the monitor
+# def get_monitor_location(index: int) -> tuple[int, int]:
+#     """returns the coordinates of the location of the monitor
 
-    Args:
-        index (int): the monitor's index
+#     Args:
+#         index (int): the monitor's index
 
-    Returns:
-        tuple[int, int]: the coordinates
-    """
-    monitor = get_monitors()[index]
-    return monitor.x, monitor.y
+#     Returns:
+#         tuple[int, int]: the coordinates
+#     """
+#     monitor = get_monitors()[index]
+#     return monitor.x, monitor.y
 
 
-def get_monitor_count() -> int:
-    """return the number of displays connected to this computer
+# def get_monitor_count() -> int:
+#     """return the number of displays connected to this computer
 
-    Returns:
-        int: amount of displays
-    """
-    return len(get_monitors())
+#     Returns:
+#         int: amount of displays
+#     """
+#     return len(get_monitors())
 
 
-__all__ = [
-    "screenshot",
-    "get_monitor_size",
-    "get_monitor_count",
-    "screenshot_monitor"
-]
+# __all__ = [
+#     "screenshot",
+#     "get_monitor_size",
+#     "get_monitor_count",
+#     "screenshot_monitor"
+# ]
```

### Comparing `danielutils-0.8.5/danielutils/__init__.py` & `danielutils-0.8.6/danielutils/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,16 +5,20 @@
 from .Decorators import *
 from .IO import *
 from .System import *
 from .Text import *
 from .Conversions import *
 from .Classes import *
 from .Time import *
-from .Threading import *
+# from .Threading import *
 from .Colors import *
 from .Data import *
 from .DataStructures import *
 from .Math import *
 from .Path import *
 from .Windows import *
 from .Print import *
 from .Exceptions import PrintCatch
+from .Reflection import *
+from .DateTime import *
+from .MetaClasses import *
+from .Generators import *
```

### Comparing `danielutils-0.8.5/pyproject.toml` & `danielutils-0.8.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "danielutils"
-version = "0.8.5"
+version = "0.8.6"
 authors = [
   { name="danielnachumdev", email="danielnachumdev@gmail.com" },
 ]
 description = "A python utils library for things I find useful"
 readme = "README.md"
 requires-python = ">=3.10.5"
 classifiers = [
```

### Comparing `danielutils-0.8.5/setup.py` & `danielutils-0.8.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,34 @@
 def read_file(path: str) -> "list[str]":
     with codecs.open(path, 'r', 'utf-8') as f:
         return [l.strip() for l in f.readlines()]
 
 
 README_PATH = 'README.md'
 DESCRIPTION = 'A python utils library for things I find useful'
-VERSION = "0.8.5"
+VERSION = "0.8.6"
 LONG_DESCRIPTION = '\n'.join(read_file(README_PATH))
 setup(
     name="danielutils",
     version=VERSION,
     author="danielnachumdev",
     author_email="<danielnachumdev@gmail.com>",
     description=DESCRIPTION,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/danielnachumdev/danielutils',
     license="MIT License",
     packages=find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests", "archive/"]),
-    install_requires=["bs4", "pyautogui", "screeninfo", "Pillow"],
+    install_requires=[
+        # "bs4",
+        #   "pyautogui",
+        "screeninfo",
+        "Pillow"
+    ],
     platforms=["All"],
     keywords=['functions', 'decorators', 'methods'],
     classifiers=[
         # "Development Status :: In development",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

