# Comparing `tmp/pyella-1.2.0.tar.gz` & `tmp/pyella-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyella-1.2.0.tar", max compression
+gzip compressed data, was "pyella-1.3.0.tar", max compression
```

## Comparing `pyella-1.2.0.tar` & `pyella-1.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    16725 2023-04-18 17:29:28.482503 pyella-1.2.0/LICENSE
--rw-r--r--   0        0        0     1847 2023-04-18 17:29:28.482503 pyella-1.2.0/README.md
--rw-r--r--   0        0        0     2530 2023-04-18 17:29:57.291034 pyella-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      159 2023-04-18 17:29:28.482503 pyella-1.2.0/src/pyella/__init__.py
--rw-r--r--   0        0        0     4715 2023-04-18 17:29:28.482503 pyella-1.2.0/src/pyella/either.py
--rw-r--r--   0        0        0     2781 2023-04-18 17:29:28.482503 pyella-1.2.0/src/pyella/maybe.py
--rw-r--r--   0        0        0      142 2023-04-18 17:29:28.482503 pyella-1.2.0/src/pyella/shared.py
--rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 pyella-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-04-30 13:31:56.361709 pyella-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1847 2023-04-30 13:31:56.361709 pyella-1.3.0/README.md
+-rw-r--r--   0        0        0     2575 2023-04-30 13:32:25.834115 pyella-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      159 2023-04-30 13:31:56.361709 pyella-1.3.0/src/pyella/__init__.py
+-rw-r--r--   0        0        0     4987 2023-04-30 13:31:56.361709 pyella-1.3.0/src/pyella/either.py
+-rw-r--r--   0        0        0     3139 2023-04-30 13:31:56.361709 pyella-1.3.0/src/pyella/maybe.py
+-rw-r--r--   0        0        0      265 2023-04-30 13:31:56.361709 pyella-1.3.0/src/pyella/shared.py
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 pyella-1.3.0/PKG-INFO
```

### Comparing `pyella-1.2.0/LICENSE` & `pyella-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyella-1.2.0/README.md` & `pyella-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyella-1.2.0/pyproject.toml` & `pyella-1.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -22,42 +22,45 @@
 keywords = [
 ]
 license = "MPL-2.0"
 maintainers = ["Ely Deckers"]
 name = "pyella"
 readme = "README.md"
 repository = "https://github.com/edeckers/pyella.git"
-version = "1.2.0"
+version = "1.3.0"
+
+[tool.poetry.dependencies]
+python = ">=3.7"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 bandit = "^1.7"
 coverage = {extras = ["toml"], version = "^6.3.2"}
 isort = "^5.10.1"
 mypy = "^0.931"
 nox = "^2022.1.7"
 pre-commit = "^2.17"
 pre-commit-hooks = "^4.1"
 pytest = "^7"
-pytest-cov = "^3"
+pytest-cov = "^4"
 python-semantic-release = "^7.25.2"
 
 #########################################################################################
 # Testing
 #########################################################################################
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "INFO"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(name)s: %(message)s (%(filename)s:%(lineno)s)"
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.coverage.report]
 show_missing = true
-fail_under = 94
+fail_under = 98
 
 [tool.coverage.html]
 directory = "reports/coverage/html"
 
 [tool.coverage.xml]
 output = "reports/coverage/coverage.xml"
```

### Comparing `pyella-1.2.0/src/pyella/either.py` & `pyella-1.3.0/src/pyella/either.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 from argparse import ArgumentTypeError
 from typing import Callable, Generic, Iterable, List, Optional, TypeVar, Union, cast
 
 from pyella.maybe import Maybe, nothing
 from pyella.shared import _const
 
-TA = TypeVar("TA")
-TB = TypeVar("TB")
-TC = TypeVar("TC")
-TD = TypeVar("TD")
+TA = TypeVar("TA")  # pylint: disable=invalid-name
+TB = TypeVar("TB")  # pylint: disable=invalid-name
+TC = TypeVar("TC")  # pylint: disable=invalid-name
+TD = TypeVar("TD")  # pylint: disable=invalid-name
 
 
 class Either(Generic[TA, TB]):  # pylint: disable=too-few-public-methods
     value: Union[TA, TB]  # pylint: disable=unsubscriptable-object
 
     def bind(self, map_: Callable[[TB], Either[TA, TC]]) -> Either[TA, TC]:
         return bind(self, map_)
@@ -40,25 +40,28 @@
     def map_left(self, map_: Callable[[TA], TC]) -> Either[TC, TB]:
         return map_left(self, map_)
 
     def replace(self, value: TC) -> Either[TA, TC]:
         return replace(self, value)
 
     def if_left(self, fallback: TB) -> TB:
-        return fallback if self.is_left() else cast(TB, self.value)
+        return if_left(self, fallback)
 
     def if_right(self, fallback: TA) -> TA:
-        return fallback if self.is_right() else cast(TA, self.value)
+        return if_right(self, fallback)
 
     def is_left(self) -> bool:
         return is_left(self)
 
     def is_right(self) -> bool:
         return is_right(self)
 
+    def to_maybe(self) -> Maybe[TB]:
+        return to_maybe(self)
+
     def to_optional(self) -> Optional[TB]:  # pylint: disable=unsubscriptable-object
         return to_optional(self)
 
     @staticmethod
     def pure(value: TB) -> Either[TA, TB]:  # pylint: disable=invalid-name
         return pure(value)
 
@@ -117,27 +120,31 @@
     return bind(em0, lambda m0: pure(map_(m0)))
 
 
 def map_left(em0: Either[TA, TB], map_: Callable[[TA], TC]) -> Either[TC, TB]:
     return either(lambda e: left(map_(e)), right, em0)
 
 
-def if_left(em0: Either[TA, TB]) -> bool:
-    return isinstance(em0, Left)
+def if_left(em0: Either[TA, TB], fallback: TB) -> TB:
+    return fallback if em0.is_left() else cast(TB, em0.value)
+
+
+def if_right(em0: Either[TA, TB], fallback: TA) -> TA:
+    return fallback if em0.is_right() else cast(TA, em0.value)
 
 
 def is_left(em0: Either[TA, TB]) -> bool:
     return isinstance(em0, Left)
 
 
 def is_right(em0: Either[TA, TB]) -> bool:
     return not is_left(em0)
 
 
-def left(value: TA) -> Either[TA, TB]:
+def left(value: TA) -> Left[TA, TB]:
     return Left(value)
 
 
 def lefts(eithers: Iterable[Either[TA, TB]]) -> List[TA]:
     return list(map(lambda either: cast(TA, either.value), filter(is_left, eithers)))
 
 
@@ -145,24 +152,24 @@
     return fmap(self, _const(value))
 
 
 def rights(eithers: Iterable[Either[TA, TB]]) -> List[TB]:
     return list(map(lambda either: cast(TB, either.value), filter(is_right, eithers)))
 
 
-def right(value: TB) -> Either[TA, TB]:
-    return Right(value)
-
-
-def to_optional(
-    em0: Either[TA, TB]
-) -> Optional[TB]:  # pylint: disable=unsubscriptable-object
-    return either(lambda _: None, lambda v: cast(TB, v), em0)
+def right(value: TB) -> Right[TA, TB]:
+    return pure(value)
 
 
 def to_maybe(
     em0: Either[TA, TB]
 ) -> Maybe[TB]:  # pylint: disable=unsubscriptable-object
     return either(lambda _: nothing, lambda v: Maybe.of(cast(TB, v)), em0)
 
 
+def to_optional(
+    em0: Either[TA, TB]
+) -> Optional[TB]:  # pylint: disable=unsubscriptable-object
+    return to_maybe(em0).to_optional()
+
+
 pure = Right  # pylint: disable=invalid-name
```

### Comparing `pyella-1.2.0/src/pyella/maybe.py` & `pyella-1.3.0/src/pyella/maybe.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 #
 # This source code is licensed under the MPL-2.0 license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 from argparse import ArgumentTypeError
-from typing import Callable, Generic, TypeVar
+from typing import Callable, Generic, Optional, TypeVar
 
-from pyella.shared import _const
+from pyella.shared import _const, _identity
 
-TA = TypeVar("TA")
-TB = TypeVar("TB")
+TA = TypeVar("TA")  # pylint: disable=invalid-name
+TB = TypeVar("TB")  # pylint: disable=invalid-name
 
 
 class Maybe(Generic[TA]):  # pylint: disable=too-few-public-methods
     value: TA
 
     def bind(self, map_: Callable[[TA], Maybe[TB]]) -> Maybe[TB]:
         return bind(self, map_)
@@ -31,14 +31,17 @@
 
     def maybe(self: Maybe[TA], fallback: TB, map_: Callable[[TA], TB]) -> TB:
         return maybe(fallback, map_, self)
 
     def replace(self, value: TB) -> Maybe[TB]:
         return replace(self, value)
 
+    def to_optional(self) -> Optional[TA]:  # pylint: disable=unsubscriptable-object
+        return to_optional(self)
+
     @staticmethod
     def of(value: TA):  # pylint: disable=invalid-name
         return Maybe.pure(value)
 
     @staticmethod
     def pure(value: TA):
         return pure(value)
@@ -64,15 +67,15 @@
 
 
 class Nothing(Maybe[TA]):  # pylint: disable=too-few-public-methods
     def __str__(self) -> str:
         return "Nothing"
 
 
-nothing: Maybe = Nothing()
+nothing: Nothing = Nothing()
 
 
 def __identity(value):
     return value
 
 
 def bind(em0: Maybe[TA], map_: Callable[[TA], Maybe[TB]]) -> Maybe[TB]:
@@ -83,15 +86,15 @@
     if not isinstance(result, Maybe):
         raise ArgumentTypeError("Bind should return Maybe")
 
     return result
 
 
 def fmap(em0: Maybe[TA], map_: Callable[[TA], TB]) -> Maybe[TB]:
-    return bind(em0, lambda m0: pure(map_(m0)))
+    return bind(em0, lambda m0: Just(map_(m0)))
 
 
 def from_maybe(fallback: TB, em0: Maybe[TA]) -> TB:
     return maybe(fallback, __identity, em0)
 
 
 def is_nothing(em0: Maybe[TA]) -> bool:
@@ -102,12 +105,18 @@
     return fallback if is_nothing(em0) else map_(em0.value)
 
 
 def replace(self, value: TB) -> Maybe[TB]:
     return fmap(self, _const(value))
 
 
-def of(value: TA):  # pylint: disable=invalid-name
+def to_optional(
+    em0: Maybe[TA],
+) -> Optional[TA]:  # pylint: disable=unsubscriptable-object
+    return maybe(None, _identity, em0)
+
+
+def of(value: TA) -> Maybe[TA]:  # pylint: disable=invalid-name
     return nothing if value is None else Just(value)
 
 
 pure = of  # pylint: disable=invalid-name
```

### Comparing `pyella-1.2.0/PKG-INFO` & `pyella-1.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: pyella
-Version: 1.2.0
+Version: 1.3.0
 Summary: This library brings common monads such `Maybe` and `Either` to your Python projects.
 Home-page: https://github.com/edeckers/pyella.git
 License: MPL-2.0
 Author: Ely Deckers
 Maintainer: Ely Deckers
+Requires-Python: >=3.7
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

