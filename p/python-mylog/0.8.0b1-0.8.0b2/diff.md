# Comparing `tmp/python-mylog-0.8.0b1.tar.gz` & `tmp/python-mylog-0.8.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-mylog-0.8.0b1.tar", last modified: Sat Apr 29 13:13:55 2023, max compression
+gzip compressed data, was "python-mylog-0.8.0b2.tar", last modified: Sun Apr 30 11:30:21 2023, max compression
```

## Comparing `python-mylog-0.8.0b1.tar` & `python-mylog-0.8.0b2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:13:55.737707 python-mylog-0.8.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-29 13:13:42.000000 python-mylog-0.8.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-29 13:13:55.737707 python-mylog-0.8.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-29 13:13:42.000000 python-mylog-0.8.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-29 13:13:42.000000 python-mylog-0.8.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-29 13:13:55.737707 python-mylog-0.8.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-29 13:13:42.000000 python-mylog-0.8.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:13:55.725706 python-mylog-0.8.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:13:55.733706 python-mylog-0.8.0b1/src/mylog/
--rw-r--r--   0 runner    (1001) docker     (123)    21786 2023-04-29 13:13:42.000000 python-mylog-0.8.0b1/src/mylog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 13:13:42.000000 python-mylog-0.8.0b1/src/mylog/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:13:55.737707 python-mylog-0.8.0b1/src/python_mylog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-29 13:13:55.000000 python-mylog-0.8.0b1/src/python_mylog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-29 13:13:55.000000 python-mylog-0.8.0b1/src/python_mylog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:13:55.000000 python-mylog-0.8.0b1/src/python_mylog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:13:55.000000 python-mylog-0.8.0b1/src/python_mylog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-29 13:13:55.000000 python-mylog-0.8.0b1/src/python_mylog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 13:13:55.000000 python-mylog-0.8.0b1/src/python_mylog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:13:55.737707 python-mylog-0.8.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21858 2023-04-29 13:13:42.000000 python-mylog-0.8.0b1/tests/test_mylog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:30:21.451933 python-mylog-0.8.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-30 11:30:10.000000 python-mylog-0.8.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-30 11:30:21.451933 python-mylog-0.8.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-30 11:30:10.000000 python-mylog-0.8.0b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-30 11:30:10.000000 python-mylog-0.8.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-30 11:30:21.451933 python-mylog-0.8.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-30 11:30:10.000000 python-mylog-0.8.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:30:21.447933 python-mylog-0.8.0b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:30:21.451933 python-mylog-0.8.0b2/src/mylog/
+-rw-r--r--   0 runner    (1001) docker     (123)    21476 2023-04-30 11:30:10.000000 python-mylog-0.8.0b2/src/mylog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 11:30:10.000000 python-mylog-0.8.0b2/src/mylog/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:30:21.451933 python-mylog-0.8.0b2/src/python_mylog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-30 11:30:21.000000 python-mylog-0.8.0b2/src/python_mylog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-30 11:30:21.000000 python-mylog-0.8.0b2/src/python_mylog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 11:30:21.000000 python-mylog-0.8.0b2/src/python_mylog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 11:30:21.000000 python-mylog-0.8.0b2/src/python_mylog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-30 11:30:21.000000 python-mylog-0.8.0b2/src/python_mylog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 11:30:21.000000 python-mylog-0.8.0b2/src/python_mylog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:30:21.451933 python-mylog-0.8.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21931 2023-04-30 11:30:10.000000 python-mylog-0.8.0b2/tests/test_mylog.py
```

### Comparing `python-mylog-0.8.0b1/LICENSE` & `python-mylog-0.8.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-mylog-0.8.0b1/PKG-INFO` & `python-mylog-0.8.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mylog
-Version: 0.8.0b1
+Version: 0.8.0b2
 Summary: My logger library.
 Home-page: https://github.com/koviubi56/mylog
 Author: Koviubi56
 Author-email: koviubi56@duck.com
 License: LGPL-3.0
 Project-URL: Release notes, https://github.com/koviubi56/mylog/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/koviubi56/mylog
```

### Comparing `python-mylog-0.8.0b1/README.md` & `python-mylog-0.8.0b2/README.md`

 * *Files identical despite different names*

### Comparing `python-mylog-0.8.0b1/pyproject.toml` & `python-mylog-0.8.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-mylog-0.8.0b1/setup.cfg` & `python-mylog-0.8.0b2/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-mylog-0.8.0b1/src/mylog/__init__.py` & `python-mylog-0.8.0b2/src/mylog/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 GNU Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # ruff: noqa: SLF001
 
-__version__ = "0.8.0-beta.1"
+__version__ = "0.8.0-beta.2"
 
 import abc
 import contextlib
 import dataclasses
 import datetime
 import sys
 import time
@@ -103,15 +103,15 @@
 @overload
 def to_level(
     lvl: Levelable, int_ok: Literal[False] = False
 ) -> Level:  # pragma: no cover
     ...
 
 
-def to_level(lvl: Levelable, int_ok=False):
+def to_level(lvl: Levelable, int_ok: bool = False) -> Union[Level, int]:
     """
     Convert a Levelable to a Level (or int).
 
     Args:
         lvl (Levelable): The levelable object to convert.
         int_ok (bool, optional): If there's no level, can this function return\
  an int? Defaults to False.
@@ -298,17 +298,15 @@
         "ERROR": ("red",),
         "CRITICAL": ("red", "on_yellow", ["bold", "underline", "blink"]),
     }
     level_name_width: ClassVar[int] = 8
 
     @classmethod
     def _thing_to_compare(cls, obj: "Logger") -> str:
-        if cls.compare_using_name:
-            return obj.name
-        return obj._id
+        return obj.name if cls.compare_using_name else str(obj._id)
 
     def __eq__(self, __o: object) -> bool:
         # sourcery skip: assign-if-exp, reintroduce-else
         if isinstance(
             __o, Logger  # Hardcoded, because class can be subclassed
         ):
             return self._thing_to_compare(self) == self._thing_to_compare(__o)
@@ -323,14 +321,15 @@
 
         return NotImplemented
 
     def __repr__(self) -> str:  # pragma: no cover
         return f"<{self.__class__.__qualname__} {self.name}>"
 
     def _inherit(self) -> None:  # noqa: PLR0912,C901  # pragma: no cover
+        # sourcery skip: assign-if-exp
         if self.higher is None:
             raise ValueError("Cannot inherit if higher is None.")
 
         if self.attributes_to_inherit.propagate:
             self.propagate = self.higher.propagate
         else:
             self.propagate = False
@@ -345,29 +344,29 @@
         if self.attributes_to_inherit.indent:
             self.indent = self.higher.indent
         else:
             self.indent = 0
         if self.attributes_to_inherit.enabled:
             self.enabled = self.higher.enabled
         else:
-            self.enabled: bool = True
+            self.enabled = True
         if self.attributes_to_inherit.ctxmgr:
             self.ctxmgr = self.higher.ctxmgr
         else:
             self.ctxmgr = IndentLogger(self)
         if self.attributes_to_inherit.format:
-            self.format: str = self.higher.format
+            self.format = self.higher.format
         else:
             self.format = DEFAULT_FORMAT
         if self.attributes_to_inherit.threshold:
             self.threshold: Union[Level, int] = self.higher.threshold
         else:
             self.threshold = DEFAULT_THRESHOLD
         if self.attributes_to_inherit.handlers:
-            self.handlers: List[Handler] = self.higher.handlers
+            self.handlers = self.higher.handlers
         else:
             self.handlers = self.get_default_handlers()
 
     @staticmethod
     def get_default_handlers() -> List[Handler]:
         """
         Get the default handlers. Please note, that overwriting this function\
@@ -440,15 +439,15 @@
         Args:
             lvl (Levelable): The level.
 
         Returns:
             str: The string.
         """
         try:
-            rv = to_level(lvl, False).name.upper()  # type: ignore
+            rv = to_level(lvl, False).name.upper()
         except (ValueError, AttributeError):
             rv = str(lvl).ljust(cls.level_name_width)
 
         if rv == "WARN":  # pragma: no cover
             rv = "WARNING"
         if rv == "FATAL":  # pragma: no cover
             rv = "CRITICAL"
@@ -531,31 +530,32 @@
         return event
 
     def log(
         self,
         lvl: Levelable,
         msg: Stringable,
         traceback: bool = False,
-        frame_depth: int = 3,
+        frame_depth: int = 4,
     ) -> Optional[LogEvent]:
         """
         Log the message. Checks if the logger is enabled, propagate, and stuff.
         This IS in the public api, but (unless you need it) use the methods
         debug, info, warning, error, critical.
 
         Args:
             lvl (Levelable): The level of the message.
             msg (Stringable): The message.
             traceback (bool): Whether to include the traceback.
             frame_depth (int): The depth of the frame. If you call this from\
- your code, this (probably) should be 3.
+ your code, this (probably) should be 4.
 
         Returns:
             Optional[LogEvent]: The log event if created.
         """
+        # sourcery skip: assign-if-exp, reintroduce-else, swap-if-expression
         # Check if disabled
         if not self.enabled:
             return None
         # Check if we should log it
         if self.propagate:
             # Check if we are root
             if self.higher is None:
@@ -673,23 +673,14 @@
         Args:
             lvl (Levelable): The level to check.
 
         Returns:
             bool: Whether the logger is enabled for the given level.
         """
         lvl = to_level(lvl, True)
-        if not isinstance(self.threshold, Level):
-            warnings.warn(
-                "Logger threshold should be a Level, not"
-                f" {type(self.threshold)!r} ({self.threshold!r})."
-                " Converting threshold...",
-                UserWarning,
-                stacklevel=2,
-            )
-            self.threshold = to_level(self.threshold, True)
         return lvl >= self.threshold
 
 
 @dataclasses.dataclass(order=True)
 class IndentLogger:
     """Indent the logger."""
 
@@ -741,15 +732,15 @@
         """
         Change the threshold.
 
         Returns:
             Union[Level, int]: The old threshold.
         """
         self.old_level = self.logger.threshold
-        self.logger.threshold = self.level  # type: ignore
+        self.logger.threshold = self.level
         return self.old_level
 
     def __exit__(
         self,
         typ: Type[BaseException],
         value: BaseException,
         tb: TracebackType,
```

### Comparing `python-mylog-0.8.0b1/src/python_mylog.egg-info/PKG-INFO` & `python-mylog-0.8.0b2/src/python_mylog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mylog
-Version: 0.8.0b1
+Version: 0.8.0b2
 Summary: My logger library.
 Home-page: https://github.com/koviubi56/mylog
 Author: Koviubi56
 Author-email: koviubi56@duck.com
 License: LGPL-3.0
 Project-URL: Release notes, https://github.com/koviubi56/mylog/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/koviubi56/mylog
```

### Comparing `python-mylog-0.8.0b1/tests/test_mylog.py` & `python-mylog-0.8.0b2/tests/test_mylog.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,15 +319,15 @@
     assert not stream.flushed
 
 
 class TestLogger:
     @staticmethod
     def test_thing_to_compare(monkeypatch: pytest.MonkeyPatch):
         logger = mylog.root.get_child(random_logger_name())
-        assert logger._thing_to_compare(logger) == logger._id
+        assert logger._thing_to_compare(logger) == str(logger._id)
         with monkeypatch.context() as monkey:
             monkey.setattr(mylog.Logger, "compare_using_name", True)
             assert logger._thing_to_compare(logger) == logger.name
 
     @staticmethod
     def test_eq():
         l1 = l2 = mylog.root.get_child(random_logger_name())
@@ -576,15 +576,15 @@
         assert child.enabled is True
 
         assert child.format == parent.format
         assert child.threshold == parent.threshold
 
     @staticmethod
     def test_is_enabled_for():
-        logger = mylog.root
+        logger = mylog.root.get_child(random_logger_name())
 
         logger.threshold = mylog.Level.debug
         assert logger.is_enabled_for(mylog.Level.debug)
         assert logger.is_enabled_for(mylog.Level.info)
         assert logger.is_enabled_for(mylog.Level.warning)
         assert logger.is_enabled_for(mylog.Level.error)
         assert logger.is_enabled_for(mylog.Level.critical)
@@ -619,16 +619,17 @@
         assert not logger.is_enabled_for(mylog.Level.debug)
         assert not logger.is_enabled_for(mylog.Level.info)
         assert not logger.is_enabled_for(mylog.Level.warning)
         assert not logger.is_enabled_for(mylog.Level.error)
         assert logger.is_enabled_for(mylog.Level.critical)
 
         logger.threshold = "fatal"  # type: ignore
-        with pytest.warns(
-            UserWarning, match="Logger threshold should be a Level"
+        with pytest.raises(
+            TypeError,
+            match=r"'>=' not supported between instances of 'Level' and 'str'",
         ):
             logger.is_enabled_for(mylog.Level.critical)
 
     @staticmethod
     def test_enabled():
         logger = mylog.root.get_child(random_logger_name())
         logger.critical(random_anything())
```

