# Comparing `tmp/construct-gallery-1.0.0.post3.tar.gz` & `tmp/construct-gallery-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "construct-gallery-1.0.0.post3.tar", last modified: Sat Feb 25 10:39:19 2023, max compression
+gzip compressed data, was "construct-gallery-1.1.0.tar", last modified: Sun Apr 30 12:11:03 2023, max compression
```

## Comparing `construct-gallery-1.0.0.post3.tar` & `construct-gallery-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 10:39:19.081690 construct-gallery-1.0.0.post3/
--rw-r--r--   0 runner    (1001) docker     (123)    20849 2023-02-25 10:39:08.000000 construct-gallery-1.0.0.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-02-25 10:39:19.081690 construct-gallery-1.0.0.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22779 2023-02-25 10:39:08.000000 construct-gallery-1.0.0.post3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 10:39:19.081690 construct-gallery-1.0.0.post3/construct_gallery/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-25 10:39:08.000000 construct-gallery-1.0.0.post3/construct_gallery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-02-25 10:39:08.000000 construct-gallery-1.0.0.post3/construct_gallery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-25 10:39:08.000000 construct-gallery-1.0.0.post3/construct_gallery/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-02-25 10:39:08.000000 construct-gallery-1.0.0.post3/construct_gallery/allow_python_expr_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-02-25 10:39:08.000000 construct-gallery-1.0.0.post3/construct_gallery/bleak_scanner_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)    67562 2023-02-25 10:39:08.000000 construct-gallery-1.0.0.post3/construct_gallery/construct_gallery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-02-25 10:39:08.000000 construct-gallery-1.0.0.post3/construct_gallery/decimal_convert_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-02-25 10:39:08.000000 construct-gallery-1.0.0.post3/construct_gallery/pyshell_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-02-25 10:39:08.000000 construct-gallery-1.0.0.post3/construct_gallery/string_convert_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-02-25 10:39:08.000000 construct-gallery-1.0.0.post3/construct_gallery/wx_logging_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 10:39:19.081690 construct-gallery-1.0.0.post3/construct_gallery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-02-25 10:39:19.000000 construct-gallery-1.0.0.post3/construct_gallery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-02-25 10:39:19.000000 construct-gallery-1.0.0.post3/construct_gallery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 10:39:19.000000 construct-gallery-1.0.0.post3/construct_gallery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-25 10:39:19.000000 construct-gallery-1.0.0.post3/construct_gallery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 10:39:19.000000 construct-gallery-1.0.0.post3/construct_gallery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-25 10:39:19.000000 construct-gallery-1.0.0.post3/construct_gallery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-25 10:39:19.000000 construct-gallery-1.0.0.post3/construct_gallery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-25 10:39:19.081690 construct-gallery-1.0.0.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-02-25 10:39:08.000000 construct-gallery-1.0.0.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:11:03.221702 construct-gallery-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    20849 2023-04-30 12:10:46.000000 construct-gallery-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-30 12:11:03.221702 construct-gallery-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27711 2023-04-30 12:10:46.000000 construct-gallery-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:11:03.221702 construct-gallery-1.1.0/construct_gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-30 12:10:46.000000 construct-gallery-1.1.0/construct_gallery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-30 12:10:46.000000 construct-gallery-1.1.0/construct_gallery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 12:10:46.000000 construct-gallery-1.1.0/construct_gallery/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-04-30 12:10:46.000000 construct-gallery-1.1.0/construct_gallery/allow_python_expr_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-04-30 12:10:46.000000 construct-gallery-1.1.0/construct_gallery/bleak_scanner_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-04-30 12:10:46.000000 construct-gallery-1.1.0/construct_gallery/config_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67562 2023-04-30 12:10:46.000000 construct-gallery-1.1.0/construct_gallery/construct_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-30 12:10:46.000000 construct-gallery-1.1.0/construct_gallery/decimal_convert_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-30 12:10:46.000000 construct-gallery-1.1.0/construct_gallery/pyshell_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-30 12:10:46.000000 construct-gallery-1.1.0/construct_gallery/string_convert_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-30 12:10:46.000000 construct-gallery-1.1.0/construct_gallery/wx_logging_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:11:03.221702 construct-gallery-1.1.0/construct_gallery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-30 12:11:03.000000 construct-gallery-1.1.0/construct_gallery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-30 12:11:03.000000 construct-gallery-1.1.0/construct_gallery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:11:03.000000 construct-gallery-1.1.0/construct_gallery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-30 12:11:03.000000 construct-gallery-1.1.0/construct_gallery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:11:03.000000 construct-gallery-1.1.0/construct_gallery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 12:11:03.000000 construct-gallery-1.1.0/construct_gallery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-30 12:11:03.000000 construct-gallery-1.1.0/construct_gallery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 12:11:03.221702 construct-gallery-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-30 12:10:46.000000 construct-gallery-1.1.0/setup.py
```

### Comparing `construct-gallery-1.0.0.post3/LICENSE` & `construct-gallery-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `construct-gallery-1.0.0.post3/PKG-INFO` & `construct-gallery-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: construct-gallery
-Version: 1.0.0.post3
+Version: 1.1.0
 Summary: construct-gallery GUI (based on wxPython) and development modules
 Home-page: https://github.com/Ircama/construct-gallery
 Author: Ircama
 License: CC-BY-NC-SA-4.0
 Keywords: construct-gallery,construct-editor,module,gui,wx,wxpython,widget,binary,editorconstruct,bleak,BLE,bluetooth,plugin
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -29,14 +29,20 @@
   
   *construct* is a powerful, declarative, symmetrical parser and builder for binary data.
   
   `construct_gallery.py` is based on [wxPython](https://www.wxpython.org/) and [construct-editor](https://github.com/timrid/construct-editor): it relies on the excellent editing widgets provided by the *construct-editor* module and offers a superset of features compared with its standard [GUI](https://github.com/timrid/construct-editor/blob/main/construct_editor/main.py).
   
   This module can be directly used in GUI programs, or can be further extended with `bleak_scanner_construct.py`.
 
+- `config_editor.py`, providing the `ConfigEditorPanel()` class (widget).
+
+  This widget implements an editing GUI composed by a form including multiple byte structures, each one related to its own *construct* data model.
+  
+  The structure of this form is described by the "editing_structure" parameter.
+
 - `bleak_scanner_construct.py`, providing the `BleakScannerConstruct()` class.
 
   The component implements a [Bluetooth Low Energy](https://en.wikipedia.org/wiki/Bluetooth_Low_Energy) (BLE) GUI client to log, browse, test and edit [BLE advertisements](https://en.wikipedia.org/wiki/Bluetooth_Low_Energy#Advertising_and_discovery).
   
   This module extends `construct_gallery.py`, offering a skeleton of BLE Advertiser scanner.
   
   [bleak](https://bleak.readthedocs.io/en/latest/) is needed (`pip3 install bleak`)
```

### Comparing `construct-gallery-1.0.0.post3/README.md` & `construct-gallery-1.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,20 @@
   
   *construct* is a powerful, declarative, symmetrical parser and builder for binary data.
   
   `construct_gallery.py` is based on [wxPython](https://www.wxpython.org/) and [construct-editor](https://github.com/timrid/construct-editor): it relies on the excellent editing widgets provided by the *construct-editor* module and offers a superset of features compared with its standard [GUI](https://github.com/timrid/construct-editor/blob/main/construct_editor/main.py).
   
   This module can be directly used in GUI programs, or can be further extended with `bleak_scanner_construct.py`.
 
+- `config_editor.py`, providing the `ConfigEditorPanel()` class (widget).
+
+  This widget implements an editing GUI composed by a form including multiple byte structures, each one related to its own *construct* data model.
+  
+  The structure of this form is described by the "editing_structure" parameter.
+
 - `bleak_scanner_construct.py`, providing the `BleakScannerConstruct()` class.
 
   The component implements a [Bluetooth Low Energy](https://en.wikipedia.org/wiki/Bluetooth_Low_Energy) (BLE) GUI client to log, browse, test and edit [BLE advertisements](https://en.wikipedia.org/wiki/Bluetooth_Low_Energy#Advertising_and_discovery).
   
   This module extends `construct_gallery.py`, offering a skeleton of BLE Advertiser scanner.
   
   [bleak](https://bleak.readthedocs.io/en/latest/) is needed (`pip3 install bleak`)
@@ -60,16 +66,34 @@
 
 If the `bleak_scanner_construct.py` BLE module is also needed:
 
 ```shell
 python3 -m pip install bleak
 ```
 
+With Raspberry Pi, *bleak* will install *dbus-fast*, which needs to build the python *wheel* (related compilation takes some time).
+
 Prerequisite component: [construct_editor](https://github.com/timrid/construct-editor). *construct-editor* is automatically installed with the package, while *bleak* requires manual installation.
 
+Additional prerequisites for Raspberry Pi:
+
+```
+sudo apt-get install -y libgtk-3-dev
+python3 -m pip install attrdict
+```
+
+With Python 3.11 replace *attrdict* with *attrdict3*:
+
+```
+python3 -m pip uninstall attrdict
+python3 -m pip install attrdict3
+```
+
+The C compiler is needed too.
+
 Alternatively to the above mentioned installation method, the following steps allow installing the latest version from GitHub.
 
 - Optional preliminary configuration (if not already done):
 
   ```shell
   # Install Python anf Git
   sudo apt-get update
@@ -97,14 +121,16 @@
 
 Run `construct-gallery` from the command line. Follow the API Documentation for the rest.
 
 ## API Documentation
 
 ### ConstructGallery
 
+Test it with `python3 -m construct_gallery -c`.
+
 ```python
 import wx
 import construct as cs
 from construct_gallery import ConstructGallery, GalleryItem
 from collections import OrderedDict
 
 ...
@@ -383,16 +409,76 @@
     }
 
 note   "...
         ...
         ..."
 ```
 
+### ConfigEditorPanel
+
+This widget implements an editing GUI composed by a form including multiple structures, each one related to its own *construct* data model. All is described by the "editing_structure" dictionary.
+
+The object returned by "ConfigEditorPanel" can be used to read the edited structure via the included "editor_panel" array, like with the following:
+
+```python
+...
+config_editor_panel = ConfigEditorPanel(...)
+...
+app.MainLoop()
+
+for char in config_editor_panel.editor_panel:
+    print("Edited value:", config_editor_panel.editor_panel[char].binary)
+```
+
+Test it with `python3 -m construct_gallery -c`.
+
+The example below also describes the data model of the "editing_structure" structure.
+
+```python
+import wx
+from construct_gallery import ConfigEditorPanel
+from construct_editor.core.model import IntegerFormat
+import construct as cs
+
+editing_structure = {
+    0: {  # This must be numeric; multiple numbers can be included. The word "Characteristic 0" is written to the left side, as the first line.
+        "name": "A string",  # The bold name "A string" is written to the left side, as the second line.
+        "binary": b"My string",  # the "bytes" window is hidden by the fault ancd can be espanded through the GUI
+        "construct": cs.Struct(
+            "My string" / cs.GreedyString("utf8"),
+        ),
+        "read_only": True,  # (boolean) False or True. If True, "(read only)" is written to the left side, as the third line.
+        "size": 130,  # Number of verical pixels to show (if smallet than the minimum requested size, a scroll bar appears).
+        "IntegerFormat": IntegerFormat.Hex,  # Default format for integers: IntegerFormat.Hex or IntegerFormat.Dec
+    },
+}
+
+app = wx.App(False)
+frame = wx.Frame(
+    None, title="ConfigEditorPanelFrame demo", size=(1000, 300))
+frame.CreateStatusBar()
+main_panel = ConfigEditorPanel(frame,
+    editing_structure=editing_structure,
+    name_size=180,
+    type_size=160,
+    value_size=200)
+frame.Show(True)
+print(get_report())
+app.MainLoop()
+for char in main_panel.editor_panel:
+    editing_structure[char][
+        "new_binary"] = main_panel.editor_panel[char].binary
+for i in editing_structure:
+    print(i, editing_structure[i])
+```
+
 ### BleakScannerConstruct
 
+Test it with `python3 -m construct_gallery -b`.
+
 ```python
 import wx
 import construct as cs
 from construct_gallery import ConstructGallery, GalleryItem, BleakScannerConstruct
 from collections import OrderedDict
 from bleak import BleakScanner
 
@@ -611,7 +697,41 @@
 app = wx.App(False)
 frame = wx.Frame(None, title="Construct Hex Editor", size=(1000, 200))
 main_panel = ConstHexEditorPanel(frame)
 frame.Bind(wx.EVT_CLOSE, main_panel.on_close)
 frame.Show(True)
 app.MainLoop()
 ```
+
+## Installing wxPython with Python 3.11 on Windows
+
+At the moment of writing, the [Python wheel packaging](https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/#wheels) of wxPython for Python 3.11 is not yet available in [Pypi](https://pypi.org/). Follow this procedure to perform manual installation on Windows.
+
+As a prerequisite, if not already installed, you might need to install the
+[Visual C++ Redistributable for Visual Studio 2015](https://www.microsoft.com/en-us/download/details.aspx?id=48145). Example:
+
+```cmd
+curl "https://download.microsoft.com/download/9/3/F/93FCF1E7-E6A4-478B-96E7-D4B285925B00/vc_redist.x64.exe" --output vc_redist.x64.exe
+```
+
+Then run `vc_redist.x64.exe` and follow the installation steps.
+
+Download the right WHL of wxPython from the related [Windows artifacts](https://dev.azure.com/oleksis/wxPython/_build/results?buildId=132&view=artifacts&pathAsName=false&type=publishedArtifacts):
+
+Example:
+
+```cmd
+curl https://artprodcca1.artifacts.visualstudio.com/A09e3854d-7789-4d94-8809-7e11120c1549/40d5fac0-3bcd-4754-be87-d3ce7214bec4/_apis/artifact/cGlwZWxpbmVhcnRpZmFjdDovL29sZWtzaXMvcHJvamVjdElkLzQwZDVmYWMwLTNiY2QtNDc1NC1iZTg3LWQzY2U3MjE0YmVjNC9idWlsZElkLzEzMi9hcnRpZmFjdE5hbWUvd3hQeXRob24tcHkzLjExLXdpbl94NjQ1/content?format=zip --output wxPython-py3.11-win_x64.zip
+powershell -command "Expand-Archive -LiteralPath wxPython-py3.11-win_x64.zip -DestinationPath wxPython-py3.11-win_x64"
+```
+
+Install wxPython WHL with the same syntax of installing a standard package:
+
+```cmd
+pip install wxPython-py3.11-win_x64\wxPython-py3.11-win_x64\wxPython-4.2.1a1-cp311-cp311-win_amd64.whl
+```
+
+# Preview
+
+Preview of a sample usage of *construct_gallery* with all plugins:
+
+![Preview of a sample usage of construct_gallery with plugins](https://github.com/pvvx/ATC_MiThermometer/raw/master/python-interface/images/ble_browser.gif)
```

### Comparing `construct-gallery-1.0.0.post3/construct_gallery/allow_python_expr_plugin.py` & `construct-gallery-1.1.0/construct_gallery/allow_python_expr_plugin.py`

 * *Files identical despite different names*

### Comparing `construct-gallery-1.0.0.post3/construct_gallery/bleak_scanner_construct.py` & `construct-gallery-1.1.0/construct_gallery/bleak_scanner_construct.py`

 * *Files identical despite different names*

### Comparing `construct-gallery-1.0.0.post3/construct_gallery/construct_gallery.py` & `construct-gallery-1.1.0/construct_gallery/construct_gallery.py`

 * *Files identical despite different names*

### Comparing `construct-gallery-1.0.0.post3/construct_gallery/decimal_convert_plugin.py` & `construct-gallery-1.1.0/construct_gallery/decimal_convert_plugin.py`

 * *Files identical despite different names*

### Comparing `construct-gallery-1.0.0.post3/construct_gallery/pyshell_plugin.py` & `construct-gallery-1.1.0/construct_gallery/pyshell_plugin.py`

 * *Files identical despite different names*

### Comparing `construct-gallery-1.0.0.post3/construct_gallery/string_convert_plugin.py` & `construct-gallery-1.1.0/construct_gallery/string_convert_plugin.py`

 * *Files identical despite different names*

### Comparing `construct-gallery-1.0.0.post3/construct_gallery/wx_logging_plugin.py` & `construct-gallery-1.1.0/construct_gallery/wx_logging_plugin.py`

 * *Files identical despite different names*

### Comparing `construct-gallery-1.0.0.post3/construct_gallery.egg-info/PKG-INFO` & `construct-gallery-1.1.0/construct_gallery.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: construct-gallery
-Version: 1.0.0.post3
+Version: 1.1.0
 Summary: construct-gallery GUI (based on wxPython) and development modules
 Home-page: https://github.com/Ircama/construct-gallery
 Author: Ircama
 License: CC-BY-NC-SA-4.0
 Keywords: construct-gallery,construct-editor,module,gui,wx,wxpython,widget,binary,editorconstruct,bleak,BLE,bluetooth,plugin
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -29,14 +29,20 @@
   
   *construct* is a powerful, declarative, symmetrical parser and builder for binary data.
   
   `construct_gallery.py` is based on [wxPython](https://www.wxpython.org/) and [construct-editor](https://github.com/timrid/construct-editor): it relies on the excellent editing widgets provided by the *construct-editor* module and offers a superset of features compared with its standard [GUI](https://github.com/timrid/construct-editor/blob/main/construct_editor/main.py).
   
   This module can be directly used in GUI programs, or can be further extended with `bleak_scanner_construct.py`.
 
+- `config_editor.py`, providing the `ConfigEditorPanel()` class (widget).
+
+  This widget implements an editing GUI composed by a form including multiple byte structures, each one related to its own *construct* data model.
+  
+  The structure of this form is described by the "editing_structure" parameter.
+
 - `bleak_scanner_construct.py`, providing the `BleakScannerConstruct()` class.
 
   The component implements a [Bluetooth Low Energy](https://en.wikipedia.org/wiki/Bluetooth_Low_Energy) (BLE) GUI client to log, browse, test and edit [BLE advertisements](https://en.wikipedia.org/wiki/Bluetooth_Low_Energy#Advertising_and_discovery).
   
   This module extends `construct_gallery.py`, offering a skeleton of BLE Advertiser scanner.
   
   [bleak](https://bleak.readthedocs.io/en/latest/) is needed (`pip3 install bleak`)
```

### Comparing `construct-gallery-1.0.0.post3/construct_gallery.egg-info/SOURCES.txt` & `construct-gallery-1.1.0/construct_gallery.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 construct_gallery/__init__.py
 construct_gallery/__main__.py
 construct_gallery/__version__.py
 construct_gallery/allow_python_expr_plugin.py
 construct_gallery/bleak_scanner_construct.py
+construct_gallery/config_editor.py
 construct_gallery/construct_gallery.py
 construct_gallery/decimal_convert_plugin.py
 construct_gallery/pyshell_plugin.py
 construct_gallery/string_convert_plugin.py
 construct_gallery/wx_logging_plugin.py
 construct_gallery.egg-info/PKG-INFO
 construct_gallery.egg-info/SOURCES.txt
```

### Comparing `construct-gallery-1.0.0.post3/setup.py` & `construct-gallery-1.1.0/setup.py`

 * *Files identical despite different names*

