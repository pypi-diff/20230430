# Comparing `tmp/tkreform-0.3.5.tar.gz` & `tmp/tkreform-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkreform-0.3.5.tar", last modified: Sun Apr 30 13:06:02 2023, max compression
+gzip compressed data, was "tkreform-0.3.6.tar", last modified: Sun Apr 30 13:25:29 2023, max compression
```

## Comparing `tkreform-0.3.5.tar` & `tkreform-0.3.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:06:02.605682 tkreform-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-30 13:05:57.000000 tkreform-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-30 13:06:02.605682 tkreform-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-30 13:05:57.000000 tkreform-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 13:06:02.605682 tkreform-0.3.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-04-30 13:05:57.000000 tkreform-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:06:02.601682 tkreform-0.3.5/tkreform/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-30 13:05:57.000000 tkreform-0.3.5/tkreform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-30 13:05:57.000000 tkreform-0.3.5/tkreform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-04-30 13:05:57.000000 tkreform-0.3.5/tkreform/declarative.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-30 13:05:57.000000 tkreform-0.3.5/tkreform/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-30 13:05:57.000000 tkreform-0.3.5/tkreform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-30 13:05:57.000000 tkreform-0.3.5/tkreform/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-30 13:05:57.000000 tkreform-0.3.5/tkreform/menu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:06:02.605682 tkreform-0.3.5/tkreform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-30 13:06:02.000000 tkreform-0.3.5/tkreform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-30 13:06:02.000000 tkreform-0.3.5/tkreform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 13:06:02.000000 tkreform-0.3.5/tkreform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-30 13:06:02.000000 tkreform-0.3.5/tkreform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-30 13:06:02.000000 tkreform-0.3.5/tkreform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:25:29.600220 tkreform-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-30 13:25:20.000000 tkreform-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-30 13:25:29.600220 tkreform-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-30 13:25:21.000000 tkreform-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 13:25:29.600220 tkreform-0.3.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1020 2023-04-30 13:25:21.000000 tkreform-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:25:29.600220 tkreform-0.3.6/tkreform/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-30 13:25:21.000000 tkreform-0.3.6/tkreform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17837 2023-04-30 13:25:21.000000 tkreform-0.3.6/tkreform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-04-30 13:25:21.000000 tkreform-0.3.6/tkreform/declarative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-30 13:25:21.000000 tkreform-0.3.6/tkreform/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-30 13:25:21.000000 tkreform-0.3.6/tkreform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-30 13:25:21.000000 tkreform-0.3.6/tkreform/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-30 13:25:21.000000 tkreform-0.3.6/tkreform/menu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:25:29.600220 tkreform-0.3.6/tkreform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-30 13:25:29.000000 tkreform-0.3.6/tkreform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-30 13:25:29.000000 tkreform-0.3.6/tkreform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 13:25:29.000000 tkreform-0.3.6/tkreform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-30 13:25:29.000000 tkreform-0.3.6/tkreform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-30 13:25:29.000000 tkreform-0.3.6/tkreform.egg-info/top_level.txt
```

### Comparing `tkreform-0.3.5/LICENSE` & `tkreform-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.5/PKG-INFO` & `tkreform-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkreform
-Version: 0.3.5
+Version: 0.3.6
 Summary: Reformed tkinter coding tool.
 Home-page: https://github.com/tkinguist/tkreform
 Author: HivertMoZara
 Author-email: worldmozara@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tkreform-0.3.5/setup.py` & `tkreform-0.3.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tkreform',
-    version=open("VERSION").read(),
+    version="0.3.6",
     description='Reformed tkinter coding tool.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='HivertMoZara',
     author_email='worldmozara@gmail.com',
     url='https://github.com/tkinguist/tkreform',
     python_requires=">=3.7",
```

### Comparing `tkreform-0.3.5/tkreform/__init__.py` & `tkreform-0.3.6/tkreform/__init__.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.5/tkreform/base.py` & `tkreform-0.3.6/tkreform/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     HAS_PIL = True
 except ImportError:
     from tkinter import PhotoImage
     HAS_PIL = False
 
 WidgetType = Union[tk.Widget, ttk.Widget]
 WindowType = Union[tk.Tk, tk.Toplevel]
-HasText = Union[tk.Label, tk.Button, ttk.Label, ttk.Button, tk.Message]
 
 _T = TypeVar("_T", bound=Union[WidgetType, WindowType])
 _WidgetT = TypeVar("_WidgetT", bound=WidgetType)
 _WindowT = TypeVar("_WindowT", bound=WindowType)
 
 
 class _Base(Generic[_T], metaclass=ABCMeta):
@@ -145,16 +144,14 @@
     def __init__(self, widget: _WidgetT) -> None:
         # To keep the content image alive, here gives a slot to add a
         # reference to the image so that the image wouldn't be recycled by GC
         # at the moment the image adder finishes its work.
         self._image_slot = None
         super().__init__(widget)
         self.base = widget
-        if isinstance(widget, HasText):
-            self._raw_text = self.text
 
     def grid(self, **kwargs):
         """
         Position a widget in the parent widget in a grid.
 
         - column: `int` - use cell identified with given column (starting
             with 0)
@@ -280,25 +277,25 @@
                         pass
 
     def __mul__(self, other: Union[dec.Gridder, dec.Packer, dec.Placer]):
         self.apply(other)
         return self
 
     def update_translation(self):
-        if not self._sub_widget and hasattr(self, "_raw_text"):
-            self.text = self._raw_text
+        # if not self._sub_widget and hasattr(self, "_raw_text"):
+        #     self.text = self._raw_text
+        pass
 
     @property
     def text(self) -> str:
         """The text of the widget."""
         return self.base["text"]
 
     @text.setter
     def text(self, txt: str):
-        self._raw_text = txt
         try:
             self.base["text"] = txt
         except MessageNotFound:
             pass
 
     @property
     def image(self) -> PhotoImage:  # type: ignore
```

### Comparing `tkreform-0.3.5/tkreform/declarative.py` & `tkreform-0.3.6/tkreform/declarative.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.5/tkreform/events.py` & `tkreform-0.3.6/tkreform/events.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.5/tkreform/groups.py` & `tkreform-0.3.6/tkreform/groups.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.5/tkreform/menu.py` & `tkreform-0.3.6/tkreform/menu.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.5/tkreform.egg-info/PKG-INFO` & `tkreform-0.3.6/tkreform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkreform
-Version: 0.3.5
+Version: 0.3.6
 Summary: Reformed tkinter coding tool.
 Home-page: https://github.com/tkinguist/tkreform
 Author: HivertMoZara
 Author-email: worldmozara@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

