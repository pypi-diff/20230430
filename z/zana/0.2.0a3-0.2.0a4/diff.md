# Comparing `tmp/zana-0.2.0a3.tar.gz` & `tmp/zana-0.2.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zana-0.2.0a3.tar", max compression
+gzip compressed data, was "zana-0.2.0a4.tar", max compression
```

## Comparing `zana-0.2.0a3.tar` & `zana-0.2.0a4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1067 2023-04-09 18:44:38.853773 zana-0.2.0a3/LICENSE.txt
--rw-r--r--   0        0        0     1261 2023-04-09 18:44:58.737624 zana-0.2.0a3/README.md
--rw-r--r--   0        0        0     2533 2023-04-09 18:44:38.853773 zana-0.2.0a3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/__init__.pyi
--rw-r--r--   0        0        0      949 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/canvas/__init__.py
--rw-r--r--   0        0        0     1126 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/canvas/__init__.pyi
--rw-r--r--   0        0        0    20972 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/canvas/core.py
--rw-r--r--   0        0        0    12892 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/canvas/operator.py
--rw-r--r--   0        0        0    12100 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/canvas/proxy.py
--rw-r--r--   0        0        0        0 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/canvas/py.typed
--rw-r--r--   0        0        0    13646 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/proxy/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/testing/__init__.py
--rw-r--r--   0        0        0      344 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/testing/mock.py
--rw-r--r--   0        0        0     7892 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/types/__init__.py
--rw-r--r--   0        0        0    11980 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/types/collections.py
--rw-r--r--   0        0        0     4123 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/types/enums.py
--rw-r--r--   0        0        0     9045 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/types/mypy_plugin.py
--rw-r--r--   0        0        0        0 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/types/py.typed
--rw-r--r--   0        0        0     7984 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/util/__init__.py
--rw-r--r--   0        0        0    12131 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/util/operator.py
--rw-r--r--   0        0        0      235 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/zana/__init__.py
--rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 zana-0.2.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-30 01:27:31.986843 zana-0.2.0a4/LICENSE.txt
+-rw-r--r--   0        0        0     1261 2023-04-30 01:27:51.047039 zana-0.2.0a4/README.md
+-rw-r--r--   0        0        0     2533 2023-04-30 01:27:31.990843 zana-0.2.0a4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-30 01:27:31.990843 zana-0.2.0a4/zana/__init__.pyi
+-rw-r--r--   0        0        0      949 2023-04-30 01:27:31.990843 zana-0.2.0a4/zana/canvas/__init__.py
+-rw-r--r--   0        0        0     1126 2023-04-30 01:27:31.990843 zana-0.2.0a4/zana/canvas/__init__.pyi
+-rw-r--r--   0        0        0    20972 2023-04-30 01:27:31.990843 zana-0.2.0a4/zana/canvas/core.py
+-rw-r--r--   0        0        0    12892 2023-04-30 01:27:31.990843 zana-0.2.0a4/zana/canvas/operator.py
+-rw-r--r--   0        0        0    12100 2023-04-30 01:27:31.990843 zana-0.2.0a4/zana/canvas/proxy.py
+-rw-r--r--   0        0        0        0 2023-04-30 01:27:31.990843 zana-0.2.0a4/zana/canvas/py.typed
+-rw-r--r--   0        0        0    13646 2023-04-30 01:27:31.990843 zana-0.2.0a4/zana/proxy/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 01:27:31.990843 zana-0.2.0a4/zana/testing/__init__.py
+-rw-r--r--   0        0        0      344 2023-04-30 01:27:31.990843 zana-0.2.0a4/zana/testing/mock.py
+-rw-r--r--   0        0        0     7892 2023-04-30 01:27:31.990843 zana-0.2.0a4/zana/types/__init__.py
+-rw-r--r--   0        0        0    11980 2023-04-30 01:27:31.990843 zana-0.2.0a4/zana/types/collections.py
+-rw-r--r--   0        0        0     4123 2023-04-30 01:27:31.990843 zana-0.2.0a4/zana/types/enums.py
+-rw-r--r--   0        0        0     9045 2023-04-30 01:27:31.990843 zana-0.2.0a4/zana/types/mypy_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-30 01:27:31.990843 zana-0.2.0a4/zana/types/py.typed
+-rw-r--r--   0        0        0     8485 2023-04-30 01:27:31.990843 zana-0.2.0a4/zana/util/__init__.py
+-rw-r--r--   0        0        0    12131 2023-04-30 01:27:31.990843 zana-0.2.0a4/zana/util/operator.py
+-rw-r--r--   0        0        0      235 2023-04-30 01:27:31.990843 zana-0.2.0a4/zana/zana/__init__.py
+-rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 zana-0.2.0a4/PKG-INFO
```

### Comparing `zana-0.2.0a3/LICENSE.txt` & `zana-0.2.0a4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a3/README.md` & `zana-0.2.0a4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -39,8 +39,8 @@
 [pyversions-link]: https://pypi.python.org/pypi/zana
 [ci-image]: https://github.com/python-zana/zana/actions/workflows/workflow.yaml/badge.svg?event=push&branch=main
 [ci-link]: https://github.com/python-zana/zana/actions?query=workflow%3ACI%2FCD+event%3Apush+branch%3Amain
 [codecov-image]: https://codecov.io/gh/python-zana/zana/branch/main/graph/badge.svg
 [codecov-link]: https://codecov.io/gh/python-zana/zana
 
 
-See this release on GitHub: [v0.2.0a3](https://github.com/python-zana/zana/releases/tag/0.2.0a3)
+See this release on GitHub: [v0.2.0a4](https://github.com/python-zana/zana/releases/tag/0.2.0a4)
```

### Comparing `zana-0.2.0a3/pyproject.toml` & `zana-0.2.0a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zana"
-version = "0.2.0a3"
+version = "0.2.0a4"
 description = "general utility functions and types"
 authors = ["David Kyalo <davidmkyalo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/python-zana/zana"
 documentation = "https://python-zana.github.io/zana"
 classifiers = [
```

### Comparing `zana-0.2.0a3/zana/canvas/__init__.py` & `zana-0.2.0a4/zana/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a3/zana/canvas/__init__.pyi` & `zana-0.2.0a4/zana/canvas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a3/zana/canvas/core.py` & `zana-0.2.0a4/zana/canvas/core.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a3/zana/canvas/operator.py` & `zana-0.2.0a4/zana/canvas/operator.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a3/zana/canvas/proxy.py` & `zana-0.2.0a4/zana/canvas/proxy.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a3/zana/proxy/__init__.py` & `zana-0.2.0a4/zana/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a3/zana/types/__init__.py` & `zana-0.2.0a4/zana/types/__init__.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a3/zana/types/collections.py` & `zana-0.2.0a4/zana/types/collections.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a3/zana/types/enums.py` & `zana-0.2.0a4/zana/types/enums.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a3/zana/types/mypy_plugin.py` & `zana-0.2.0a4/zana/types/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a3/zana/util/__init__.py` & `zana-0.2.0a4/zana/util/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing as t
 from collections import abc
-from functools import reduce
+from functools import partial, reduce
 from importlib import import_module
 from threading import RLock
 from unittest import skip
 
 from typing_extensions import ParamSpec, Self
 
 from zana.types import NotSet
@@ -81,24 +81,37 @@
     except TypeError:
         raise self._dict_not_mutable_error(obj) from None
     except KeyError:
         pass
 
 
 def subclasses(*bases: type[_T], inclusive: bool = True, depth: int = -1, __skip=None, __lvl=0):
-    """ """
+    """A recursive iterator over given bases' subclasses.
+    By default, it yields all known types that can pass the
+    `issubclass(cls, bases)` test. And this includes the bases themselves.
+    """
     __skip = set() if __skip is None else __skip
     kwds = {"depth": depth, "__lvl": __lvl + 1, "__skip": __skip}
     for base in bases:
         if not (inclusive is False or base in __skip or __skip.add(base)):
             yield base
         if depth - __lvl:
             yield from subclasses(*base.__subclasses__(), **kwds)
 
 
+@t.overload
+def xsubclasses(*bases: type[_T], depth: int = -1) -> abc.Generator[type[_T]]:
+    """A recursive iterator over given classes' subclasses exclusive of the given `bases`.
+    Same as calling `subclasses(*bases, inclusive=False)`
+    """
+
+
+xsubclasses = partial(subclasses, inclusive=False)
+
+
 class class_property(t.Generic[_R]):
     attrname: str = None
 
     _dict_not_mutable_error = _dict_not_mutable_error
     _dict_not_set_error = _dict_not_set_error
 
     def __init__(
```

### Comparing `zana-0.2.0a3/zana/util/operator.py` & `zana-0.2.0a4/zana/util/operator.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a3/PKG-INFO` & `zana-0.2.0a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zana
-Version: 0.2.0a3
+Version: 0.2.0a4
 Summary: general utility functions and types
 Home-page: https://github.com/python-zana/zana
 License: MIT
 Keywords: zana,toolkit
 Author: David Kyalo
 Author-email: davidmkyalo@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -61,9 +61,9 @@
 [pyversions-link]: https://pypi.python.org/pypi/zana
 [ci-image]: https://github.com/python-zana/zana/actions/workflows/workflow.yaml/badge.svg?event=push&branch=main
 [ci-link]: https://github.com/python-zana/zana/actions?query=workflow%3ACI%2FCD+event%3Apush+branch%3Amain
 [codecov-image]: https://codecov.io/gh/python-zana/zana/branch/main/graph/badge.svg
 [codecov-link]: https://codecov.io/gh/python-zana/zana
 
 
-See this release on GitHub: [v0.2.0a3](https://github.com/python-zana/zana/releases/tag/0.2.0a3)
+See this release on GitHub: [v0.2.0a4](https://github.com/python-zana/zana/releases/tag/0.2.0a4)
```

