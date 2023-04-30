# Comparing `tmp/nodered.py-0.1.1.tar.gz` & `tmp/nodered.py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodered.py-0.1.1.tar", last modified: Sat Apr 29 04:47:27 2023, max compression
+gzip compressed data, was "nodered.py-0.1.2.tar", last modified: Sun Apr 30 05:01:13 2023, max compression
```

## Comparing `nodered.py-0.1.1.tar` & `nodered.py-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-29 04:47:27.320000 nodered.py-0.1.1/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.1.1/LICENSE
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1900 2023-04-29 04:47:27.380000 nodered.py-0.1.1/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1584 2023-04-29 03:19:05.000000 nodered.py-0.1.1/README.md
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-29 04:47:27.320000 nodered.py-0.1.1/nodered.py.egg-info/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1900 2023-04-29 04:47:27.000000 nodered.py-0.1.1/nodered.py.egg-info/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      412 2023-04-29 04:47:27.000000 nodered.py-0.1.1/nodered.py.egg-info/SOURCES.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-29 04:47:27.000000 nodered.py-0.1.1/nodered.py.egg-info/dependency_links.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      163 2023-04-29 04:47:27.000000 nodered.py-0.1.1/nodered.py.egg-info/requires.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       37 2023-04-29 04:47:27.000000 nodered.py-0.1.1/nodered.py.egg-info/top_level.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.1.1/nodered.py.egg-info/zip-safe
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-29 04:47:27.320000 nodered.py-0.1.1/noderedpy/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      288 2023-04-29 04:45:51.000000 nodered.py-0.1.1/noderedpy/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     7510 2023-04-29 04:31:59.000000 nodered.py-0.1.1/noderedpy/_nodered.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     6406 2023-04-28 10:06:27.000000 nodered.py-0.1.1/noderedpy/_server.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     8536 2023-04-29 04:32:28.000000 nodered.py-0.1.1/noderedpy/_templates.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      794 2023-04-28 05:18:07.000000 nodered.py-0.1.1/noderedpy/decorator.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-29 04:47:27.320000 nodered.py-0.1.1/noderedpy/node-red-starter/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2398 2023-04-29 01:58:51.000000 nodered.py-0.1.1/noderedpy/node-red-starter/index.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      296 2023-04-27 11:00:04.000000 nodered.py-0.1.1/noderedpy/node-red-starter/package.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-04-29 04:47:27.380000 nodered.py-0.1.1/setup.cfg
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1044 2023-04-28 05:53:24.000000 nodered.py-0.1.1/setup.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-30 05:01:13.360000 nodered.py-0.1.2/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.1.2/LICENSE
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2074 2023-04-30 05:01:13.450000 nodered.py-0.1.2/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1758 2023-04-30 04:58:00.000000 nodered.py-0.1.2/README.md
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-30 05:01:13.360000 nodered.py-0.1.2/nodered.py.egg-info/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2074 2023-04-30 05:01:13.000000 nodered.py-0.1.2/nodered.py.egg-info/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      435 2023-04-30 05:01:13.000000 nodered.py-0.1.2/nodered.py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-30 05:01:13.000000 nodered.py-0.1.2/nodered.py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      163 2023-04-30 05:01:13.000000 nodered.py-0.1.2/nodered.py.egg-info/requires.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       37 2023-04-30 05:01:13.000000 nodered.py-0.1.2/nodered.py.egg-info/top_level.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.1.2/nodered.py.egg-info/zip-safe
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-30 05:01:13.360000 nodered.py-0.1.2/noderedpy/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      466 2023-04-30 03:51:45.000000 nodered.py-0.1.2/noderedpy/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     7628 2023-04-30 04:22:32.000000 nodered.py-0.1.2/noderedpy/_nodered.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3357 2023-04-30 04:55:12.000000 nodered.py-0.1.2/noderedpy/_property.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     6410 2023-04-30 03:53:02.000000 nodered.py-0.1.2/noderedpy/_server.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    10303 2023-04-30 04:47:34.000000 nodered.py-0.1.2/noderedpy/_templates.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      805 2023-04-30 03:52:23.000000 nodered.py-0.1.2/noderedpy/decorator.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-30 05:01:13.370000 nodered.py-0.1.2/noderedpy/node-red-starter/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2398 2023-04-29 01:58:51.000000 nodered.py-0.1.2/noderedpy/node-red-starter/index.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      296 2023-04-27 11:00:04.000000 nodered.py-0.1.2/noderedpy/node-red-starter/package.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-04-30 05:01:13.450000 nodered.py-0.1.2/setup.cfg
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1044 2023-04-28 05:53:24.000000 nodered.py-0.1.2/setup.py
```

### Comparing `nodered.py-0.1.1/LICENSE` & `nodered.py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.1/PKG-INFO` & `nodered.py-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.1.1
+Version: 0.1.2
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -72,14 +72,15 @@
 ```python
 @register("test")
 def test(props:dict, msg:dict) -> dict:
     # user codes here
     return msg
 ```
 - See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/decorator.py#L8">noredpy.decorator.register function</a> for details
+- See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/_property.py">noderedpy._property</a> for details of "Property"
 <br/>
 
 ### start server
 - default server
 ```python
 server.start("{port}")
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.1.1 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.1.2 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
 
@@ -16,12 +16,12 @@
 ## ð  usage ### server initialize - default server ```python from noderedpy
 import Server, RED server = Server( RED( os.path.join(__dirname, ".node-red"),
 "/node-red", 1880 ) ) ``` - standalone(with webview) ```python from noderedpy
 import StandaloneServer, RED server = StandaloneServer( RED( os.path.join
 (__dirname, ".node-red"), "/node-red", 1880 ) ) ```
 ### register Node ```python @register("test") def test(props:dict, msg:dict) -
 > dict: # user codes here return msg ``` - See noredpy.decorator.register
-function for details
+function for details - See noderedpy._property for details of "Property"
 ### start server - default server ```python server.start("{port}") ``` -
 standalone(with webview) ```python server.start("{title}") ```
 
 ## Todos [x] type support for "list" and "dict"
```

### Comparing `nodered.py-0.1.1/README.md` & `nodered.py-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 ```python
 @register("test")
 def test(props:dict, msg:dict) -> dict:
     # user codes here
     return msg
 ```
 - See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/decorator.py#L8">noredpy.decorator.register function</a> for details
+- See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/_property.py">noderedpy._property</a> for details of "Property"
 <br/>
 
 ### start server
 - default server
 ```python
 server.start("{port}")
 ```
```

#### html2text {}

```diff
@@ -11,12 +11,12 @@
 ## ð  usage ### server initialize - default server ```python from noderedpy
 import Server, RED server = Server( RED( os.path.join(__dirname, ".node-red"),
 "/node-red", 1880 ) ) ``` - standalone(with webview) ```python from noderedpy
 import StandaloneServer, RED server = StandaloneServer( RED( os.path.join
 (__dirname, ".node-red"), "/node-red", 1880 ) ) ```
 ### register Node ```python @register("test") def test(props:dict, msg:dict) -
 > dict: # user codes here return msg ``` - See noredpy.decorator.register
-function for details
+function for details - See noderedpy._property for details of "Property"
 ### start server - default server ```python server.start("{port}") ``` -
 standalone(with webview) ```python server.start("{title}") ```
 
 ## Todos [x] type support for "list" and "dict"
```

### Comparing `nodered.py-0.1.1/nodered.py.egg-info/PKG-INFO` & `nodered.py-0.1.2/nodered.py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.1.1
+Version: 0.1.2
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -72,14 +72,15 @@
 ```python
 @register("test")
 def test(props:dict, msg:dict) -> dict:
     # user codes here
     return msg
 ```
 - See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/decorator.py#L8">noredpy.decorator.register function</a> for details
+- See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/_property.py">noderedpy._property</a> for details of "Property"
 <br/>
 
 ### start server
 - default server
 ```python
 server.start("{port}")
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.1.1 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.1.2 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
 
@@ -16,12 +16,12 @@
 ## ð  usage ### server initialize - default server ```python from noderedpy
 import Server, RED server = Server( RED( os.path.join(__dirname, ".node-red"),
 "/node-red", 1880 ) ) ``` - standalone(with webview) ```python from noderedpy
 import StandaloneServer, RED server = StandaloneServer( RED( os.path.join
 (__dirname, ".node-red"), "/node-red", 1880 ) ) ```
 ### register Node ```python @register("test") def test(props:dict, msg:dict) -
 > dict: # user codes here return msg ``` - See noredpy.decorator.register
-function for details
+function for details - See noderedpy._property for details of "Property"
 ### start server - default server ```python server.start("{port}") ``` -
 standalone(with webview) ```python server.start("{title}") ```
 
 ## Todos [x] type support for "list" and "dict"
```

### Comparing `nodered.py-0.1.1/noderedpy/_nodered.py` & `nodered.py-0.1.2/noderedpy/_nodered.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 import os, sys, subprocess, threading, traceback, noderedpy
 from types import MethodType
 from typing import Type, Literal, Any, List
 from ._templates import package_json, node_html, node_js
+from ._property import Property
 from . import __path__
 
 
 class RED:
     """
     Node-RED manager class
     """
@@ -123,68 +124,68 @@
         """
         if os.path.exists(self.__started_file):
             os.remove(self.__started_file)
 
         self.__stop()
 
 
-class NodeProperty:
-    """
-    Property for Node function
-    """
-    def __init__(self, name:str, type:Literal["str", "int", "float", "list", "dict"], default_value:Any = None, required:bool = False, display_icon:str = None):
-        """
-        Property information for Node function
-
-        Parameters
-        ----------
-        name: str, required
-            name of Property
-        type: Literal["str", "int", "float"], required
-            type of Property
-        default_value: Any, default None
-            default value of Property
-        required: bool, default False
-            set Property is required or not
-        display_icon: str, default None
-            icon for Node-RED node display
-        """
-        if " " in name.strip():
-            raise NameError("Property name cannot contain space!")
+# class NodeProperty:
+#     """
+#     Property for Node function
+#     """
+#     def __init__(self, name:str, type:Literal["str", "int", "float", "list", "dict"], default_value:Any = None, required:bool = False, display_icon:str = None):
+#         """
+#         Property information for Node function
+
+#         Parameters
+#         ----------
+#         name: str, required
+#             name of Property
+#         type: Literal["str", "int", "float"], required
+#             type of Property
+#         default_value: Any, default None
+#             default value of Property
+#         required: bool, default False
+#             set Property is required or not
+#         display_icon: str, default None
+#             icon for Node-RED node display
+#         """
+#         if " " in name.strip():
+#             raise NameError("Property name cannot contain space!")
         
-        if not type in ("str", "int", "float", "list", "dict"):
-            raise TypeError("Currently supported types: [ 'str', 'int', 'float', 'list', 'dict' ]")
+#         if not type in ("str", "int", "float", "list", "dict"):
+#             raise TypeError("Currently supported types: [ 'str', 'int', 'float', 'list', 'dict' ]")
         
-        if default_value is not None and not isinstance(default_value, ( str, int, float, list, dict )):
-            raise TypeError("Currently supported value types: [ str, int, float, list, dict ]")
+#         if default_value is not None and not isinstance(default_value, ( str, int, float, list, dict )):
+#             raise TypeError("Currently supported value types: [ str, int, float, list, dict ]")
 
-        self.name, self.type, self.default_value, self.required =\
-            name, type, default_value, required
+#         self.name, self.type, self.default_value, self.required =\
+#             name, type, default_value, required
         
-        if display_icon is None:
-            if type in ( "int", "float" ):
-                self.display_icon = "fa fa-sort-numeric-asc"
-            elif type == "str":
-                self.display_icon = "fa fa-font"
-            elif type == "list":
-                self.display_icon = "fa fa-list"
-            elif type == "dict":
-                self.display_icon = "fa fa-code"
-        else:
-            self.display_icon = display_icon
+#         if display_icon is None:
+#             if type in ( "int", "float" ):
+#                 self.display_icon = "fa fa-sort-numeric-asc"
+#             elif type == "str":
+#                 self.display_icon = "fa fa-font"
+#             elif type == "list":
+#                 self.display_icon = "fa fa-list"
+#             elif type == "dict":
+#                 self.display_icon = "fa fa-code"
+#         else:
+#             self.display_icon = display_icon
         
-    @property
-    def display_name(self) -> str:
-        return " ".join([
-            item.capitalize()
-            for item in self.name.split("_")
-        ])
+#     @property
+#     def display_name(self) -> str:
+#         return " ".join([
+#             item.capitalize()
+#             for item in self.name.split("_")
+#         ])
 
 class Node:
-    def __init__(self, name:str, category:str, properties:List[NodeProperty], node_func:MethodType):
+    def __init__(self, name:str, category:str, properties:List[Property], node_func:MethodType):
         if " " in name.strip():
             raise NameError("Node name cannot contain spaces!")
         
         if "-" in category.strip() or "," in category.strip():
             raise NameError("Category cannot contain '-' or ','!")
 
         self.name, self.category, self.properties =\
```

### Comparing `nodered.py-0.1.1/noderedpy/_server.py` & `nodered.py-0.1.2/noderedpy/_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 import os, sys, json, shutil, asyncio
 from glob import glob
 from typing import List, Type
 from types import MethodType
 from aiohttp import web
-from ._nodered import RED, Node, NodeProperty
+from ._nodered import RED, Node
+from ._property import Property
 
 
 class Server(web.Application):
     """
     Server to communicate with Node-RED
     """
     registered_nodes:List[Node] = []
@@ -42,27 +43,27 @@
             import webbrowser
             webbrowser.open_new(f"http://127.0.0.1:{self.__red.port}/node-red")
 
         if self.__start_callback:
             self.__start_callback()
 
 
-    def register(self, node_func:MethodType, name:str, category:str = "nodered_py", properties:List[NodeProperty] = []):
+    def register(self, node_func:MethodType, name:str, category:str = "nodered_py", properties:List[Property] = []):
         """
         Function to register Node function
 
         Parameters
         ----------
         node_func: MethodType, required
             Node function to register
         name: str, required
             name of Node to register
         category: str, default nodered_py
             category of Node
-        properties: List[noderedpy._nodered.NodeProperty]
+        properties: List[noderedpy._property.Property]
             propertis of Node
         """
         node = Node(name if name.startswith("nodered-py") else f"nodered-py-{name}", category, properties, node_func)
         Server.registered_nodes.append(node)
 
     def start(self, port:int, show_browser:bool = True, callback:MethodType = None):
         """
@@ -135,27 +136,27 @@
         ----------
         node_red: RED, required
             Node-RED settings
         """
         self.__server = Server(node_red)
         self.__red = node_red
 
-    def register(self, node_func:MethodType, name:str, category:str = "nodered_py", properties:List[NodeProperty] = []):
+    def register(self, node_func:MethodType, name:str, category:str = "nodered_py", properties:List[Property] = []):
         """
         Function to register Node function
 
         Parameters
         ----------
         node_func: MethodType, required
             Node function to register
         name: str, required
             name of Node to register
         category: str, default nodered_py
             category of Node
-        properties: List[noderedpy._nodered.NodeProperty]
+        properties: List[noderedpy._property.Property]
             propertis of Node
         """
         self.__server.register(node_func, name, category, properties)
 
     def start(self, title:str, width:int = 1000, height:int = 650, x:int = None, y:int = None, debug:bool = False, port:int = 1881, default_root:str = None):
         """
         Start Server and show webview
```

### Comparing `nodered.py-0.1.1/noderedpy/_templates.py` & `nodered.py-0.1.2/noderedpy/_templates.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # -*- coding: utf-8 -*-
 import json, noderedpy
+from ._property import (
+    InputProperty, ListProperty, DictProperty,
+    SpinnerProperty, ComboBoxProperty
+)
 
 
 def package_json(node:"noderedpy._nodered.Node") -> str:
     return json.dumps({
         "name": node.name,
         "version": "1.0.0",
         "description": f"nodered.py {node.name} node",
@@ -14,25 +18,27 @@
                 node.name: f"lib/{node.name}.js"
             }
         }
     }, indent = 4)
 
 def node_html(node:"noderedpy._nodered.Node") -> str:
     properties_html, properties_js, properties_js_prepare, properties_js_cancel, properties_js_save = [], [], [], [], []
+    default_value = None
     for property in node.properties:
-        if property.type in ( "str", "int", "float" ):
+        if isinstance(property, InputProperty):
             properties_html.append(f"""
     <div class="form-row" style="margin-bottom:0px;">
         <label><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
     </div>
     <div class="form-row">
-        <input type="text" id="node-input-{property.name}">
+        <input type="text" id="node-input-{property.name}" style="width:100%;">
     </div>
 """)
-        elif property.type == "list":
+            default_value = f'"{property.default}"' if isinstance(property.default, str) else str(property.default)
+        elif isinstance(property, ListProperty):
             properties_html.append(f"""
     <div class="form-row" style="margin-bottom:0px;">
         <label><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
     </div>
     <div class="form-row node-input-{property.name}-container-row">
         <ol id="node-input-{property.name}-container" style="height:250px;"></ol>
     </div>
@@ -55,15 +61,16 @@
 ''')
             properties_js_save.append('''
             this.''' + property.name + ''' = [];
             $("#node-input-''' + property.name + '''-container").editableList("items").each((_, item) => {
                 this.''' + property.name + '''.push(item.find("input.input-list-item").val());
             });
 ''')
-        else:
+            default_value = str(property.default)
+        elif isinstance(property, DictProperty):
             properties_html.append(f"""
     <div class="form-row" style="margin-bottom:0px;">
         <label><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
     </div>
     <div class="form-row node-text-editor-row">
         <div style="height:250px;" class="node-text-editor" id="node-input-{property.name}"></div>
     </div>
@@ -81,24 +88,64 @@
             delete this.{property.name}Editor;
 """)
             properties_js_save.append(f"""
             $("#node-input-{property.name}").val(this.{property.name}Editor.getValue().trim());
             this.{property.name}Editor.destroy();
             delete this.{property.name}Editor;
 """)
-                                   
-        if property.default_value:
-            default_value = f'"{property.default_value}"' if property.type == "str" else f"`{json.dumps(property.default_value, indent = 4)}`" if property.type == "dict" else str(property.default_value)
-        else:
-            default_value = '""' if property.type == "str" else "[]" if property.type == "list" else '"{}"' if property.type == "dict" else "0"
+            default_value = f"`{json.dumps(property.default, indent = 4)}`"
+        elif isinstance(property, SpinnerProperty):
+            properties_html.append(f"""
+    <div class="form-row" style="margin-bottom:0px;">
+        <label><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
+    </div>
+    <div class="form-row">
+        <input type="text" id="node-input-{property.name}" style="width:calc(100% - 22px);">
+    </div>
+""")
+            properties_js_prepare.append('''
+            $("#node-input-''' + property.name + '''").spinner({ min: 0 });
+''')
+            default_value = str(property.default)
+        elif isinstance(property, ComboBoxProperty):
+            options = "\n".join([
+                f"""
+            <option value="{item}">{item}</option>
+"""
+                for item in property.items
+            ])
+            properties_html.append(f"""
+    <div class="form-row" style="margin-bottom:0px;">
+        <label><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
+    </div>
+    <div class="form-row">
+        <select id="node-input-{property.name}Select" style="width:100%;">
+{options}
+        </select>
+        <input type="text" id="node-input-{property.name}" style="display:none;">
+    </div>
+""")
+            properties_js_prepare.append('''
+            $("#node-input-''' + property.name + '''Select").val(this.''' + property.name + ''');
+''')
+            properties_js_save.append('''
+            $("#node-input-''' + property.name + '''").val($("#node-input-''' + property.name + ''';").val());
+''')
+            default_value = f'"{property.default}"' if isinstance(property.default, str) else str(property.default)
 
-        properties_js.append("            " + property.name + ': { value: ' + default_value + ' }')
+        if default_value:
+            properties_js.append("            " + property.name + ': { value: ' + default_value + ' }')
 
     return '''
 <script type="text/html" data-template-name="''' + node.name + '''">
+    <style>
+        span.ui-spinner {
+            width: 100%;
+        }
+    </style>
     <div class="form-row">
         <label for="node-input-name"><i class="fa fa-tag"></i> <span>Name</span></label>
         <input type="text" id="node-input-name" style="width:calc(100% - 105px);">
     </div>
     <hr>
     ''' + "".join(properties_html) + '''
 </script>
```

### Comparing `nodered.py-0.1.1/noderedpy/decorator.py` & `nodered.py-0.1.2/noderedpy/decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # -*- coding: utf-8 -*-
 from typing import List
 from types import MethodType
-from ._nodered import Node, NodeProperty
+from ._nodered import Node
+from ._property import Property
 from ._server import Server
 
 
-def register(name:str, category:str = "nodered_py", properties:List[NodeProperty] = []) -> MethodType:
+def register(name:str, category:str = "nodered_py", properties:List[Property] = []) -> MethodType:
     """
     Decorator to register Node function
 
     Parameters
     ----------
     name: str, required
         name of Node to register
     category: str, default nodered_py
         category of Node
-    properties: List[noderedpy._nodered.NodeProperty]
+    properties: List[noderedpy._property.Property]
         propertis of Node
     """
     def decorator(node_func:MethodType):
         node = Node(name if name.startswith("nodered-py") else f"nodered-py-{name}", category, properties, node_func)
         Server.registered_nodes.append(node)
 
         return node_func
```

### Comparing `nodered.py-0.1.1/noderedpy/node-red-starter/index.js` & `nodered.py-0.1.2/noderedpy/node-red-starter/index.js`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.1/setup.py` & `nodered.py-0.1.2/setup.py`

 * *Files identical despite different names*

