# Comparing `tmp/tkreform-0.3.4.tar.gz` & `tmp/tkreform-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkreform-0.3.4.tar", last modified: Tue Apr 11 18:17:24 2023, max compression
+gzip compressed data, was "tkreform-0.3.5.tar", last modified: Sun Apr 30 13:06:02 2023, max compression
```

## Comparing `tkreform-0.3.4.tar` & `tkreform-0.3.5.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:17:24.202396 tkreform-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 18:17:21.000000 tkreform-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-11 18:17:24.202396 tkreform-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-11 18:17:21.000000 tkreform-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:17:24.202396 tkreform-0.3.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-04-11 18:17:21.000000 tkreform-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:17:24.198395 tkreform-0.3.4/tkreform/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-11 18:17:21.000000 tkreform-0.3.4/tkreform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18527 2023-04-11 18:17:21.000000 tkreform-0.3.4/tkreform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-04-11 18:17:21.000000 tkreform-0.3.4/tkreform/declarative.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-11 18:17:21.000000 tkreform-0.3.4/tkreform/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-11 18:17:21.000000 tkreform-0.3.4/tkreform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-11 18:17:21.000000 tkreform-0.3.4/tkreform/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-11 18:17:21.000000 tkreform-0.3.4/tkreform/linguist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-11 18:17:21.000000 tkreform-0.3.4/tkreform/menu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:17:24.202396 tkreform-0.3.4/tkreform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-11 18:17:24.000000 tkreform-0.3.4/tkreform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-11 18:17:24.000000 tkreform-0.3.4/tkreform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:17:24.000000 tkreform-0.3.4/tkreform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-11 18:17:24.000000 tkreform-0.3.4/tkreform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 18:17:24.000000 tkreform-0.3.4/tkreform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:06:02.605682 tkreform-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-30 13:05:57.000000 tkreform-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-30 13:06:02.605682 tkreform-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-30 13:05:57.000000 tkreform-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 13:06:02.605682 tkreform-0.3.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-04-30 13:05:57.000000 tkreform-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:06:02.601682 tkreform-0.3.5/tkreform/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-30 13:05:57.000000 tkreform-0.3.5/tkreform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-30 13:05:57.000000 tkreform-0.3.5/tkreform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-04-30 13:05:57.000000 tkreform-0.3.5/tkreform/declarative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-30 13:05:57.000000 tkreform-0.3.5/tkreform/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-30 13:05:57.000000 tkreform-0.3.5/tkreform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-30 13:05:57.000000 tkreform-0.3.5/tkreform/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-30 13:05:57.000000 tkreform-0.3.5/tkreform/menu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:06:02.605682 tkreform-0.3.5/tkreform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-30 13:06:02.000000 tkreform-0.3.5/tkreform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-30 13:06:02.000000 tkreform-0.3.5/tkreform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 13:06:02.000000 tkreform-0.3.5/tkreform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-30 13:06:02.000000 tkreform-0.3.5/tkreform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-30 13:06:02.000000 tkreform-0.3.5/tkreform.egg-info/top_level.txt
```

### Comparing `tkreform-0.3.4/LICENSE` & `tkreform-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.4/PKG-INFO` & `tkreform-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkreform
-Version: 0.3.4
+Version: 0.3.5
 Summary: Reformed tkinter coding tool.
 Home-page: https://github.com/tkinguist/tkreform
 Author: HivertMoZara
 Author-email: worldmozara@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tkreform-0.3.4/setup.py` & `tkreform-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.4/tkreform/__init__.py` & `tkreform-0.3.5/tkreform/__init__.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.4/tkreform/base.py` & `tkreform-0.3.5/tkreform/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from abc import ABCMeta, abstractmethod
 import sys
 import tkinter as tk
 from tkinter import TclError, ttk
 
 from tkreform.exceptions import MessageNotFound, WidgetNotArranged
-from tkreform.linguist import Linguist
 from tkreform.menu import MenuItem
 from . import declarative as dec
 from typing import (
     Any, Callable, Generic, Iterable, List, Optional, Tuple, Type, TypeVar, Union, cast,
     overload
 )
 
@@ -40,15 +39,14 @@
         """
         Base type of Window / Widget.
 
         - base: `WindowType | WidgetType` - base window / widget type
         """
         self.base = base
         self._sub_widget: List["Widget"] = []
-        self._linguist: Optional[Linguist] = None
 
     @overload
     def __getitem__(self, it: int) -> "Widget":
         ...
 
     @overload
     def __getitem__(self, it: slice) -> List["Widget"]:
@@ -104,15 +102,14 @@
         - sub: `Iterable[dec.W]` - sub widget tree
         """
         for w in sub:
             if isinstance(w, MenuItem):
                 self.base.add(w.type, **w.data)  # type: ignore
             else:
                 _widget = self.add_widget(w.widget, **w.kwargs)
-                _widget.linguist = self.linguist
                 if isinstance(self.base, tk.Menu) and isinstance(w, dec.M):
                     self.base.add(w.it.type, menu=_widget.base, **w.it.data)
                 elif isinstance(self.base, tk.PanedWindow):
                     self.base.add(_widget.base)
                 elif isinstance(self.base, ttk.Notebook):
                     w.controller = cast(dec.NotebookAdder, w.controller)
                     self.base.add(
@@ -134,23 +131,14 @@
         """Destroy window / widget."""
         self.base.destroy()
 
     @abstractmethod
     def update_translation(self):
         raise NotImplementedError
 
-    @property
-    def linguist(self):
-        return self._linguist
-
-    @linguist.setter
-    def linguist(self, _l: Optional[Linguist]):
-        self._linguist = _l
-        self.update_translation()
-
 
 class Widget(_Base, Generic[_WidgetT]):
     """
     Reformed Widget type based on `tkinter`.
     """
     base: _WidgetT
 
@@ -294,27 +282,25 @@
     def __mul__(self, other: Union[dec.Gridder, dec.Packer, dec.Placer]):
         self.apply(other)
         return self
 
     def update_translation(self):
         if not self._sub_widget and hasattr(self, "_raw_text"):
             self.text = self._raw_text
-        for w in self._sub_widget:
-            w.linguist = self.linguist
 
     @property
     def text(self) -> str:
         """The text of the widget."""
         return self.base["text"]
 
     @text.setter
     def text(self, txt: str):
         self._raw_text = txt
         try:
-            self.base["text"] = self._linguist[txt] if self._linguist else txt
+            self.base["text"] = txt
         except MessageNotFound:
             pass
 
     @property
     def image(self) -> PhotoImage:  # type: ignore
         """The image of the widget."""
         return self.base["image"]
@@ -439,29 +425,27 @@
         def __wrapper(func: Callable[[], Any]):
             self.base.protocol(protocol, func)
             return func
         return __wrapper
 
     def update_translation(self):
         self.title = self._raw_title
-        for w in self._sub_widget:
-            w.linguist = self.linguist
+        # for w in self._sub_widget:
+        #     w.linguist = self.linguist
 
     @property
     def title(self):
         """Window title."""
         return self.base.title()
 
     @title.setter
     def title(self, title: str):
         self._raw_title = title
         try:
-            self.base.title(
-                self._linguist[title] if self._linguist else title
-            )
+            self.base.title(title)
         except MessageNotFound:
             pass
 
     @property
     def geometry(self):
         """Geometry string."""
         return self.base.geometry()
```

### Comparing `tkreform-0.3.4/tkreform/declarative.py` & `tkreform-0.3.5/tkreform/declarative.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.4/tkreform/events.py` & `tkreform-0.3.5/tkreform/events.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.4/tkreform/groups.py` & `tkreform-0.3.5/tkreform/groups.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.4/tkreform/menu.py` & `tkreform-0.3.5/tkreform/menu.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.4/tkreform.egg-info/PKG-INFO` & `tkreform-0.3.5/tkreform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkreform
-Version: 0.3.4
+Version: 0.3.5
 Summary: Reformed tkinter coding tool.
 Home-page: https://github.com/tkinguist/tkreform
 Author: HivertMoZara
 Author-email: worldmozara@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

