# Comparing `tmp/grill-0.9.1.tar.gz` & `tmp/grill-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "B:\write\code\git\grill\dist\tmpxjwt2y7_\grill-0.9.1.tar", last modified: Wed Apr 14 12:31:09 2021, max compression
+gzip compressed data, was "B:\write\code\git\grill\dist\tmpdaae_965\grill-0.9.2.tar", last modified: Fri Apr 16 23:14:08 2021, max compression
```

## Comparing `grill-0.9.1.tar` & `grill-0.9.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2021-04-14 12:31:09.039071 grill-0.9.1/
--rw-rw-rw-   0        0        0    35815 2019-10-14 10:47:05.000000 grill-0.9.1/LICENSE
--rw-rw-rw-   0        0        0       39 2021-04-13 14:09:25.000000 grill-0.9.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5098 2021-04-14 12:31:09.040051 grill-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     4016 2021-04-10 08:55:11.000000 grill-0.9.1/README.md
-drwxrwxrwx   0        0        0        0 2021-04-14 12:31:08.906053 grill-0.9.1/grill/
-drwxrwxrwx   0        0        0        0 2021-04-14 12:31:08.968053 grill-0.9.1/grill/logger/
--rw-rw-rw-   0        0        0       56 2020-12-20 02:38:02.000000 grill-0.9.1/grill/logger/__init__.py
--rw-rw-rw-   0        0        0      856 2020-12-20 02:38:02.000000 grill-0.9.1/grill/logger/controller.py
--rw-rw-rw-   0        0        0     1324 2020-12-20 02:38:02.000000 grill-0.9.1/grill/logger/model.py
-drwxrwxrwx   0        0        0        0 2021-04-14 12:31:08.974053 grill-0.9.1/grill/resources/
--rw-rw-rw-   0        0        0      421 2021-04-10 08:55:11.000000 grill-0.9.1/grill/resources/plugInfo.json
-drwxrwxrwx   0        0        0        0 2021-04-14 12:31:09.030066 grill-0.9.1/grill/views/
--rw-rw-rw-   0        0        0     1735 2021-01-07 10:53:18.000000 grill-0.9.1/grill/views/__main__.py
--rw-rw-rw-   0        0        0     3974 2021-04-10 08:55:11.000000 grill-0.9.1/grill/views/create.py
--rw-rw-rw-   0        0        0     1057 2021-03-07 06:48:08.000000 grill-0.9.1/grill/views/dearview.py
--rw-rw-rw-   0        0        0    15717 2021-04-10 08:55:11.000000 grill-0.9.1/grill/views/description.py
--rw-rw-rw-   0        0        0     1973 2021-04-10 08:55:11.000000 grill-0.9.1/grill/views/houdini.py
--rw-rw-rw-   0        0        0      296 2021-03-07 02:13:51.000000 grill-0.9.1/grill/views/quicklaunch.py
--rw-rw-rw-   0        0        0    30252 2021-04-10 08:55:11.000000 grill-0.9.1/grill/views/sheets.py
--rw-rw-rw-   0        0        0     3029 2021-04-10 12:21:58.000000 grill-0.9.1/grill/views/usdview.py
-drwxrwxrwx   0        0        0        0 2021-04-14 12:31:09.038071 grill-0.9.1/grill/write/
--rw-rw-rw-   0        0        0     8182 2021-04-10 08:55:11.000000 grill-0.9.1/grill/write/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-14 12:31:08.953066 grill-0.9.1/grill.egg-info/
--rw-rw-rw-   0        0        0     5098 2021-04-14 12:31:08.000000 grill-0.9.1/grill.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2021-04-14 12:31:08.000000 grill-0.9.1/grill.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-04-14 12:31:08.000000 grill-0.9.1/grill.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2021-04-14 12:31:08.000000 grill-0.9.1/grill.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2021-04-14 12:31:08.000000 grill-0.9.1/grill.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2020-12-20 02:38:02.000000 grill-0.9.1/pyproject.toml
--rw-rw-rw-   0        0        0      773 2021-04-14 12:31:09.049066 grill-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0     1463 2021-04-13 14:11:24.000000 grill-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2021-04-16 23:14:08.057912 grill-0.9.2/
+-rw-rw-rw-   0        0        0    35815 2019-10-14 10:47:05.000000 grill-0.9.2/LICENSE
+-rw-rw-rw-   0        0        0       39 2021-04-14 12:36:01.000000 grill-0.9.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5098 2021-04-16 23:14:08.057912 grill-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4016 2021-04-10 08:55:11.000000 grill-0.9.2/README.md
+drwxrwxrwx   0        0        0        0 2021-04-16 23:14:08.008911 grill-0.9.2/grill/
+drwxrwxrwx   0        0        0        0 2021-04-16 23:14:08.045911 grill-0.9.2/grill/logger/
+-rw-rw-rw-   0        0        0       56 2020-12-20 02:38:02.000000 grill-0.9.2/grill/logger/__init__.py
+-rw-rw-rw-   0        0        0      856 2020-12-20 02:38:02.000000 grill-0.9.2/grill/logger/controller.py
+-rw-rw-rw-   0        0        0     1324 2020-12-20 02:38:02.000000 grill-0.9.2/grill/logger/model.py
+drwxrwxrwx   0        0        0        0 2021-04-16 23:14:08.046912 grill-0.9.2/grill/resources/
+-rw-rw-rw-   0        0        0      421 2021-04-14 12:36:01.000000 grill-0.9.2/grill/resources/plugInfo.json
+drwxrwxrwx   0        0        0        0 2021-04-16 23:14:08.055913 grill-0.9.2/grill/views/
+-rw-rw-rw-   0        0        0     1735 2021-01-07 10:53:18.000000 grill-0.9.2/grill/views/__main__.py
+-rw-rw-rw-   0        0        0     3974 2021-04-10 08:55:11.000000 grill-0.9.2/grill/views/create.py
+-rw-rw-rw-   0        0        0     1057 2021-03-07 06:48:08.000000 grill-0.9.2/grill/views/dearview.py
+-rw-rw-rw-   0        0        0    15786 2021-04-16 22:43:04.000000 grill-0.9.2/grill/views/description.py
+-rw-rw-rw-   0        0        0     1973 2021-04-10 08:55:11.000000 grill-0.9.2/grill/views/houdini.py
+-rw-rw-rw-   0        0        0      296 2021-03-07 02:13:51.000000 grill-0.9.2/grill/views/quicklaunch.py
+-rw-rw-rw-   0        0        0    30252 2021-04-10 08:55:11.000000 grill-0.9.2/grill/views/sheets.py
+-rw-rw-rw-   0        0        0     3106 2021-04-16 23:01:28.000000 grill-0.9.2/grill/views/usdview.py
+drwxrwxrwx   0        0        0        0 2021-04-16 23:14:08.056914 grill-0.9.2/grill/write/
+-rw-rw-rw-   0        0        0     8182 2021-04-10 08:55:11.000000 grill-0.9.2/grill/write/__init__.py
+drwxrwxrwx   0        0        0        0 2021-04-16 23:14:08.039913 grill-0.9.2/grill.egg-info/
+-rw-rw-rw-   0        0        0     5098 2021-04-16 23:14:07.000000 grill-0.9.2/grill.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2021-04-16 23:14:08.000000 grill-0.9.2/grill.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-04-16 23:14:07.000000 grill-0.9.2/grill.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2021-04-16 23:14:07.000000 grill-0.9.2/grill.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2021-04-16 23:14:07.000000 grill-0.9.2/grill.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2020-12-20 02:38:02.000000 grill-0.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0      773 2021-04-16 23:14:08.059912 grill-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     1463 2021-04-14 12:36:01.000000 grill-0.9.2/setup.py
```

### Comparing `grill-0.9.1/LICENSE` & `grill-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grill-0.9.1/PKG-INFO` & `grill-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grill
-Version: 0.9.1
+Version: 0.9.2
 Summary: Pipeline tools for (but not limited to) audiovisual projects.
 Home-page: https://github.com/thegrill/grill
 Author: Christian López Barrón
 Author-email: chris.gfz@gmail.com
 License: UNKNOWN
 Description: # 👨‍🍳 The Grill
         [![Build Status](https://travis-ci.org/thegrill/grill.svg?branch=master)](https://travis-ci.org/thegrill/grill)
```

### Comparing `grill-0.9.1/README.md` & `grill-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `grill-0.9.1/grill/logger/controller.py` & `grill-0.9.2/grill/logger/controller.py`

 * *Files identical despite different names*

### Comparing `grill-0.9.1/grill/logger/model.py` & `grill-0.9.2/grill/logger/model.py`

 * *Files identical despite different names*

### Comparing `grill-0.9.1/grill/views/__main__.py` & `grill-0.9.2/grill/views/__main__.py`

 * *Files identical despite different names*

### Comparing `grill-0.9.1/grill/views/create.py` & `grill-0.9.2/grill/views/create.py`

 * *Files identical despite different names*

### Comparing `grill-0.9.1/grill/views/dearview.py` & `grill-0.9.2/grill/views/dearview.py`

 * *Files identical despite different names*

### Comparing `grill-0.9.1/grill/views/description.py` & `grill-0.9.2/grill/views/description.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,15 +284,17 @@
 
         self._paths = paths = defaultdict(set)  # {layer.identifier: {path1, ..., pathN}}
 
         def _layer_label(layer):
             return Path(layer.realPath).stem or layer.identifier
 
         def _walk_layer_tree(tree):
-            yield tree.layer
+            tree_layer = tree.layer
+            if tree_layer:
+                yield tree_layer
             for childtree in tree.childTrees:
                 yield from _walk_layer_tree(childtree)
 
         def _add_node(pcp_node):
             layer_stack = pcp_node.layerStack
             root_layer = layer_stack.identifier.rootLayer
             root_id = root_layer.identifier
```

### Comparing `grill-0.9.1/grill/views/houdini.py` & `grill-0.9.2/grill/views/houdini.py`

 * *Files identical despite different names*

### Comparing `grill-0.9.1/grill/views/sheets.py` & `grill-0.9.2/grill/views/sheets.py`

 * *Files identical despite different names*

### Comparing `grill-0.9.1/grill/views/usdview.py` & `grill-0.9.2/grill/views/usdview.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
+# USDView not on pypi yet, so not possible to test this on CI
 import types
 from functools import lru_cache, partial
 
 from pxr import Tf
 from pxr.Usdviewq.plugin import PluginContainer
 
 from PySide2 import QtWidgets
 
 from . import sheets as _sheets
 from . import description as _description
 from . import create as _create
 
 
-def _stage_on_widget(widgetCls):
+def _stage_on_widget(widget_creator):
     @lru_cache(maxsize=None)
     def _launcher(usdviewApi):
-        widget = widgetCls(parent=usdviewApi.qMainWindow)
+        widget = widget_creator(parent=usdviewApi.qMainWindow)
         widget.setStage(usdviewApi.stage)
         return widget
     return _launcher
 
 
 @lru_cache(maxsize=None)
 def prim_composition(usdviewApi):
@@ -41,26 +42,26 @@
                 usdviewApi.qMainWindow, "Save Changes", text
         ) == QtWidgets.QMessageBox.Yes:
             usdviewApi.stage.Save()
     return types.SimpleNamespace(show=show)
 
 
 def repository_path(usdviewApi):
-    parent = usdviewApi.qMainWindow
-    return types.SimpleNamespace(show=_create.CreateAssets._setRepositoryPath(parent))
+    show = partial(_create.CreateAssets._setRepositoryPath, usdviewApi.qMainWindow)
+    return types.SimpleNamespace(show=show)
 
 
 class GrillPlugin(PluginContainer):
 
     def registerPlugins(self, plugRegistry, usdviewApi):
         def show(_launcher, _usdviewAPI):
             return _launcher(_usdviewAPI).show()
 
         def _menu_item(title, _launcher):
-            # contract: each of these return an object which show a widget on `show()`
+            # contract: _launcher() returns an object that shows a widget on `show()`
             return plugRegistry.registerCommandPlugin(
                 f"Grill.{title.replace(' ', '_')}", title, partial(show, _launcher),
             )
 
         self._menu_items = [
             _menu_item(title, launcher)
             for (title, launcher) in (
```

### Comparing `grill-0.9.1/grill/write/__init__.py` & `grill-0.9.2/grill/write/__init__.py`

 * *Files identical despite different names*

### Comparing `grill-0.9.1/grill.egg-info/PKG-INFO` & `grill-0.9.2/grill.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grill
-Version: 0.9.1
+Version: 0.9.2
 Summary: Pipeline tools for (but not limited to) audiovisual projects.
 Home-page: https://github.com/thegrill/grill
 Author: Christian López Barrón
 Author-email: chris.gfz@gmail.com
 License: UNKNOWN
 Description: # 👨‍🍳 The Grill
         [![Build Status](https://travis-ci.org/thegrill/grill.svg?branch=master)](https://travis-ci.org/thegrill/grill)
```

### Comparing `grill-0.9.1/grill.egg-info/SOURCES.txt` & `grill-0.9.2/grill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grill-0.9.1/setup.cfg` & `grill-0.9.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 7269 6c6c 0d0a 7665 7273 696f   = grill..versio
-00000020: 6e20 3d20 302e 392e 310d 0a64 6573 6372  n = 0.9.1..descr
+00000020: 6e20 3d20 302e 392e 320d 0a64 6573 6372  n = 0.9.2..descr
 00000030: 6970 7469 6f6e 203d 2050 6970 656c 696e  iption = Pipelin
 00000040: 6520 746f 6f6c 7320 666f 7220 2862 7574  e tools for (but
 00000050: 206e 6f74 206c 696d 6974 6564 2074 6f29   not limited to)
 00000060: 2061 7564 696f 7669 7375 616c 2070 726f   audiovisual pro
 00000070: 6a65 6374 732e 0d0a 6c6f 6e67 5f64 6573  jects...long_des
 00000080: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
 00000090: 2052 4541 444d 452e 6d64 0d0a 6c6f 6e67   README.md..long
```

### Comparing `grill-0.9.1/setup.py` & `grill-0.9.2/setup.py`

 * *Files identical despite different names*

