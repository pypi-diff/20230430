# Comparing `tmp/unigui-1.3.7.tar.gz` & `tmp/unigui-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unigui-1.3.7.tar", last modified: Mon Apr 17 22:01:53 2023, max compression
+gzip compressed data, was "unigui-1.3.8.tar", last modified: Sun Apr 30 19:55:19 2023, max compression
```

## Comparing `unigui-1.3.7.tar` & `unigui-1.3.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-17 22:01:53.631464 unigui-1.3.7/
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.3.7/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.3.7/MANIFEST.in
--rw-r--r--   0 george    (1000) george    (1000)    18851 2023-04-17 22:01:53.631464 unigui-1.3.7/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)    18581 2023-03-08 16:33:36.000000 unigui-1.3.7/README.md
--rw-r--r--   0 george    (1000) george    (1000)       38 2023-04-17 22:01:53.631464 unigui-1.3.7/setup.cfg
--rw-r--r--   0 george    (1000) george    (1000)      565 2023-04-17 22:01:38.000000 unigui-1.3.7/setup.py
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-17 22:01:53.628131 unigui-1.3.7/unigui/
--rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:50.000000 unigui-1.3.7/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     7560 2023-04-17 20:46:05.000000 unigui-1.3.7/unigui/guielements.py
--rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.3.7/unigui/manager.py
--rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:40.000000 unigui-1.3.7/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.3.7/unigui/userset.py
--rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:22.000000 unigui-1.3.7/unigui/utils.py
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-17 22:01:53.628131 unigui-1.3.7/unigui/web/
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-17 22:01:53.628131 unigui-1.3.7/unigui/web/css/
--rw-r--r--   0 george    (1000) george    (1000)     3267 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/css/855.47c4761e.css
--rw-r--r--   0 george    (1000) george    (1000)        0 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/css/app.31d6cfe0.css
--rw-r--r--   0 george    (1000) george    (1000)   219590 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/css/vendor.49a52e8f.css
--rw-r--r--   0 george    (1000) george    (1000)    64483 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/favicon.ico
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-17 22:01:53.631464 unigui-1.3.7/unigui/web/fonts/
--rw-r--r--   0 george    (1000) george    (1000)    20436 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0 george    (1000) george    (1000)    20544 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0 george    (1000) george    (1000)    20416 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0 george    (1000) george    (1000)    20408 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0 george    (1000) george    (1000)    20424 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0 george    (1000) george    (1000)    20344 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0 george    (1000) george    (1000)   164912 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0 george    (1000) george    (1000)   128360 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-17 22:01:53.631464 unigui-1.3.7/unigui/web/icons/
--rw-r--r--   0 george    (1000) george    (1000)    12324 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/icons/favicon-128x128.png
--rw-r--r--   0 george    (1000) george    (1000)      859 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/icons/favicon-16x16.png
--rw-r--r--   0 george    (1000) george    (1000)     2039 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/icons/favicon-32x32.png
--rw-r--r--   0 george    (1000) george    (1000)     9643 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/icons/favicon-96x96.png
--rw-r--r--   0 george    (1000) george    (1000)      907 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/index.html
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-17 22:01:53.631464 unigui-1.3.7/unigui/web/js/
--rw-r--r--   0 george    (1000) george    (1000)      763 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/js/193.b4cc3ffe.js
--rw-r--r--   0 george    (1000) george    (1000)     6560 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/js/430.4be6e8a8.js
--rw-r--r--   0 george    (1000) george    (1000)    39631 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/js/855.e620c0f1.js
--rw-r--r--   0 george    (1000) george    (1000)     5868 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/js/app.ed80a2d1.js
--rw-r--r--   0 george    (1000) george    (1000)   847622 2023-04-17 21:42:41.000000 unigui-1.3.7/unigui/web/js/vendor.c0de6c67.js
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-17 22:01:53.628131 unigui-1.3.7/unigui.egg-info/
--rw-r--r--   0 george    (1000) george    (1000)    18851 2023-04-17 22:01:53.000000 unigui-1.3.7/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)     1194 2023-04-17 22:01:53.000000 unigui-1.3.7/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-04-17 22:01:53.000000 unigui-1.3.7/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.3.7/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-04-17 22:01:53.000000 unigui-1.3.7/unigui.egg-info/top_level.txt
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-30 19:55:19.702103 unigui-1.3.8/
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.3.8/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.3.8/MANIFEST.in
+-rw-r--r--   0 george    (1000) george    (1000)    19408 2023-04-30 19:55:19.702103 unigui-1.3.8/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)    19138 2023-04-30 19:49:37.000000 unigui-1.3.8/README.md
+-rw-r--r--   0 george    (1000) george    (1000)       38 2023-04-30 19:55:19.702103 unigui-1.3.8/setup.cfg
+-rw-r--r--   0 george    (1000) george    (1000)      565 2023-04-30 19:55:05.000000 unigui-1.3.8/setup.py
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-30 19:55:19.698769 unigui-1.3.8/unigui/
+-rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:50.000000 unigui-1.3.8/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     7695 2023-04-30 19:19:54.000000 unigui-1.3.8/unigui/guielements.py
+-rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.3.8/unigui/manager.py
+-rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:40.000000 unigui-1.3.8/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.3.8/unigui/userset.py
+-rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:22.000000 unigui-1.3.8/unigui/utils.py
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-30 19:55:19.698769 unigui-1.3.8/unigui/web/
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-30 19:55:19.698769 unigui-1.3.8/unigui/web/css/
+-rw-r--r--   0 george    (1000) george    (1000)     3267 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/css/855.47c4761e.css
+-rw-r--r--   0 george    (1000) george    (1000)        0 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/css/app.31d6cfe0.css
+-rw-r--r--   0 george    (1000) george    (1000)   219590 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/css/vendor.49a52e8f.css
+-rw-r--r--   0 george    (1000) george    (1000)    64483 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/favicon.ico
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-30 19:55:19.702103 unigui-1.3.8/unigui/web/fonts/
+-rw-r--r--   0 george    (1000) george    (1000)    20436 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0 george    (1000) george    (1000)    20544 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0 george    (1000) george    (1000)    20416 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0 george    (1000) george    (1000)    20408 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0 george    (1000) george    (1000)    20424 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0 george    (1000) george    (1000)    20344 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0 george    (1000) george    (1000)   164912 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0 george    (1000) george    (1000)   128360 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-30 19:55:19.702103 unigui-1.3.8/unigui/web/icons/
+-rw-r--r--   0 george    (1000) george    (1000)    12324 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/icons/favicon-128x128.png
+-rw-r--r--   0 george    (1000) george    (1000)      859 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/icons/favicon-16x16.png
+-rw-r--r--   0 george    (1000) george    (1000)     2039 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/icons/favicon-32x32.png
+-rw-r--r--   0 george    (1000) george    (1000)     9643 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/icons/favicon-96x96.png
+-rw-r--r--   0 george    (1000) george    (1000)      907 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/index.html
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-30 19:55:19.702103 unigui-1.3.8/unigui/web/js/
+-rw-r--r--   0 george    (1000) george    (1000)      763 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/js/193.b4cc3ffe.js
+-rw-r--r--   0 george    (1000) george    (1000)     6560 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/js/430.4be6e8a8.js
+-rw-r--r--   0 george    (1000) george    (1000)    39631 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/js/855.e620c0f1.js
+-rw-r--r--   0 george    (1000) george    (1000)     5868 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/js/app.ed80a2d1.js
+-rw-r--r--   0 george    (1000) george    (1000)   847622 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/js/vendor.c0de6c67.js
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-30 19:55:19.698769 unigui-1.3.8/unigui.egg-info/
+-rw-r--r--   0 george    (1000) george    (1000)    19408 2023-04-30 19:55:19.000000 unigui-1.3.8/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)     1194 2023-04-30 19:55:19.000000 unigui-1.3.8/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-04-30 19:55:19.000000 unigui-1.3.8/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.3.8/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-04-30 19:55:19.000000 unigui-1.3.8/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.3.7/LICENSE` & `unigui-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/PKG-INFO` & `unigui-1.3.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: unigui
-Version: 1.3.7
-Summary: Unigui - Universal app browser
-Home-page: https://github.com/Claus1/unigui
-Author: Georgii Dernovyi
-Author-email: g.dernovoy@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # unigui #
 Universal GUI and App Browser
     Python connector
 
 ### Purpose ###
 Provide a programming technology that does not require front-end programming, for a server written in any language, for displaying on any device, in any resolution, without any tuning. 
 
@@ -49,14 +38,16 @@
 block = Block('X Block',
     [           
         Button('Clean table', icon = 'swipe'),
         Select('Select', value='All', options=['All','Based','Group'])
     ], table, icon = 'api')
 ```
 
+#### Screen function prepare() syncronizes GUI elements one to another and with the program/system data. prepare() is called when the screen open/loaded. prepare() is optional. ###
+
 ### Server start ###
 tests/run_hello.py
 ```
 import unigui
 #app name, port for initial connection and upload_dir folder are optional
 unigui.start('Test app') 
 ```
@@ -80,51 +71,59 @@
 ```
 def clean_table(_, value):
     table.rows = []
     return table
 clean_button = Button('Clean the table’, clean_table)
 ```
 
-‘changed’ handlers have to return Gui object or array of Gui objects that were changed by the handler and Unigui has to redraw or does nothing if all visible elements have the same state. Unigui will do all other jobs for synchronizing automatically. If a Gui object doesn't have 'changed' handler the object accepts incoming value automatically to the 'value' variable of gui object.
+| Handler returns |	Description |
+| :---: | :---: | 
+| Gui object |  Object to update |
+| Gui object array or tuple |  Objects to update |
+| None | Nothing to update, Ok |
+| Error(...), Warning(...), Info(...) | Show to user info about a problem. |
+| UpdateScreen, True | Redraw whole screen |
+| Dialog(..) | Open a dialog with parameters |
 
-If 'value' is not acceptable instead of returning an object possible to return Error or Warning or Info. That functions can update a list object after the message argument, and synchronize simultaneously.
+Unigui	synchronizes GUI state on frontend-end automatically after calling a handler.
 
-#### If a handler returns True or UpdateScreen constant the whole screen will be redrawn. Screen function prepare() syncronizes GUI elements one to another and with the program/system data. prepare() is called when the screen open/loaded. prepare() is optional.
+If a Gui object doesn't have 'changed' handler the object accepts incoming value automatically to the 'value' variable of gui object.
+
+If 'value' is not acceptable instead of returning an object possible to return Error or Warning or Info. That functions can update a object list passed after the message argument.
 
 ```
 def changed_range(_, value):
    if value < 0.5 and value > 1.0:
        #or Error(message, _) if we want to return the previous visible value to the field
        return Error(f‘The value of {_.name} has to be > 0.5 and < 1.0!') 
     #accept value othewise
     _.value = value
 
 edit = Edit('Range of involving', 0.6, changed_range)
 ```
-If the handler returns None (or does not return anything) Unigui considers it as Ok.
 
 ### Block details ###
-The width and height of blocks is calculated automatically depending on their children. It is possible to set the block width and make it scrollable in height, for example for images list. Possible to add MD icon to the header, if required. Width, scroll, .. are optional.
+The width and height of blocks is calculated automatically depending on their children. It is possible to set the block width, or make it scrollable , for example for images list. Possible to add MD icon to the header, if required. width, scroll, height, icon are optional.
 ```
 block = Block(‘Pictures’,add_button, *images, width = 500, scroll = True,icon = 'api')
 ```
  
-The second parameter of the Block constructor is an array of widgets which has to be in the header just after the name.
-Blocks can be shared between the user screens with its states. Such a block has to be located in the blocks folder of the python layer.
+The second parameter of the Block constructor is a widget(s) which are drawn in the block header just after its name.
+Blocks can be shared between the user screens with its states. Such a block has to be located in the 'blocks' folder .
 Examples of such block tests/blocks/tblock.py:
 ```
 from unigui import *
 ..
 concept_block = Block('Concept block',
    [   #some gui elements       
        Button('Run',run_proccess),
        Edit('Working folder','run_folder')
    ], result_table)
 ```
-If some elements are enumerated inside an array, Unigui will display them on a line, otherwise everyone will be displayed on a new own line(s).
+If some elements are enumerated inside an array, Unigui will display them on a line one after another, otherwise everyone will be displayed on a new own line(s).
  
 Using a shared block in some screen:
 ```
 from blocks.tblock import concept_block
 ...
 blocks = [.., concept_block]
 ```
@@ -147,200 +146,246 @@
 #### Example ####
 blocks = [ [b1,b2], [b3, [b4, b5]]]
 #[b1,b2] - the first vertical area, [b3, [b4, b5]] - the second one.
 
 ![alt text](https://github.com/Claus1/unigui/blob/main/tests/multiscreen.png?raw=true)
 
 ### Basic gui elements ###
-Normally they have type property which says unigui how to draw the element. If the type is omitting unigui can detect it by analyzing its content.
-#### If the element name starts from _ , Unigui will not show its name on the screen. ####
-if we need to paint an icon somewhere in the element, add 'icon': 'any MD icon name'.
+Normally they have type property which says unigui what data it contains and optionally how to draw the element. 
+#### If the element name starts from _ , unigui will hide its name on the screen. ####
+if we need to paint an icon in an element, add 'icon': 'any MD icon name' to the element constructor.
 
-#### All constructor parameters are optional for all Gui elements except the first one - name. ####
+#### Most constructor parameters are optional for Gui elements except the first one which is the element name. ####
 
 Common form for element constructors:
 ```
 Gui('Name', value = some_value, changed = changed_handler)
 #It is possible to use short form, that is equal:
 Gui('Name', some_value, changed_handler)
 ```
 calling the method 
 def accept(self, value) 
 causes  a call changed handler if it defined, otherwise just save value to self.value
 
-#### Button ####
+### Button ###
 Normal button.
 ```
 Button('Push me', changed = push_callback) 
 ```
 Short form
 ```
 Button('Push me', push_callback) 
 ```
 Icon button 
 ```
 Button('_Check', push_callback, icon = 'check')
 ```
-#### Load to server Button ####
+
+### Load to server Button ###
 Special button provides file loading from user device or computer to the Unigui server.
 ```
 UploadButton('Load', handler_when_loading_finish, icon='photo_library')
 ```
 handler_when_loading_finish(button_, the_loaded_file_filename) where the_loaded_file_filename is a file name in upload server folder. This folder name is optional upload_dir parameter in unigui.start.
 
-#### Camera Button ####
+### Camera Button ###
 Special button provides to make a photo on the user mobile device. 
 ```
 CameraButton('Make a photo', handler_when_shooting_finish, icon='camera_alt')
 ```
 handler_when_loading_finish(button_, name_of_loaded_file) where name_of_loaded_file is the made photo name in the server folder. This folder name is an
 optional upload_dir parameter in unigui.start.
 
-#### Edit and Text field. ####
+
+### Edit and Text field. ###
 ```
 Edit('Some field', '') #for string value
 Edit('Number field', 0.9) #for numbers
 ```
 If set edit = false it will be readonly field or text label.
 ```
 Edit('Some field', '', edit = false) 
 #is equal to
 Text('Some field')
 ```
-complete handler is optional function which accepts the current field value and returns a string list for autocomplete.
-```
-Edit('Edit me', value = '', complete = get_complete_list) #value has to be string or number
+complete handler is optional function which accepts the current edit value and returns a string list for autocomplete.
 
+```
 def get_complete_list(gui_element, current_value):
     return [s for s in vocab if current_value in s]    
+
+Edit('Edit me', value = '', complete = get_complete_list) #value has to be string or number
 ```
-Can contain optional 'update' handler which is called when the user press Enter in the field.
-It can return None or objects for updating as usual handler.
 
-Can contain optional selection property == (start, end) of selection in the input
-Can contain optional autogrow property, which uses for multiline fileds.
+Optional 'update' handler is called when the user press Enter in the field.
+It can return None if OK or objects for updating as usual 'changed' handler.
 
+Optional selection property with parameters (start, end) is called when selection is happened.
+Optional autogrow property uses for serving multiline fileds.
 
-#### Radio button ####
+
+### Radio button ###
 ```
-Switch('Radio button', value = True[,changed = .., type = ...]) #value has to be boolean, changed, type - optional
+Switch('Radio button', value = True[,changed = .., type = ...])
 
-type can be 'check' for a status button or 'switch' for a switcher . 
+Optional type can be 'check' for a status button or 'switch' for a switcher . 
 ```
 
-#### Select group. Contains options field. ####
+### Select group. Contains options field. ###
 ```
 Select('Select something', "choice1", selection_is_changed, options = ["choice1","choice2", "choice3"]) 
 ```
-can be such type 'toggles','list','dropdown'. Unigui automatically chooses between toogles and dropdown,
-but the user can set type = 'list' then Unigui build it as vertical select list.
+Optional type parameter can be 'toggles','list','dropdown'. Unigui automatically chooses between toogles and dropdown, if type is omitted,
+if type = 'list' then Unigui build it as vertical select list.
+
 
-#### Image. #### 
-width,changed and height are optional, changed is called if the user select/ or touch the image.
+### Image. ###
+width,changed,height,header are optional, changed is called if the user select or touch the image.
 ```
 Image(image_url, header = 'description', changed = selecting_changed, width = .., height = ..)
 ```
 
-#### Video. #### 
+
+### Video. ###
 width and height are optional.
 ```
 Video(video_url, width = .., height = ..)
 ```
 
-#### Tree. The element for tree-like data. ####
+### Tree. The element for tree-like data. ###
 ```
 Tree(name, selected_item_name, changed_handler, options = {name1: parent1, name2 : None, .})
 ```
-options for the data without repeating names, it is dictionary {item_name:parent_name}. 
+options is a tree structure, a dictionary {item_name:parent_name}. 
 
-parent_name and parent_key are None for root items. changed_handler gets item key (name) as value. 
+parent_name is None for root items. changed_handler gets item key (name) as value. 
 
 ### Table. ###
-Tables is common structure for presenting 2D data and charts. Can contain append, delete, update handlers, multimode parameter is True if allowed single and multi select mode. True by default. All of them are optional. When you add a handler for such action Unigui draws and activates an appropriate action icon button in the table header automatically.
+Tables is common structure for presenting 2D data and charts. 
+Optional append, delete, update handlers are called for adding, deleting and updating rows.
+
+
+Assigning a handler for such action causes Unigui to draw and activate an appropriate action icon button in the table header automatically.
 ```
 table = Table('Videos', [0], row_changed, headers = ['Video', 'Duration', 'Owner', 'Status'],  
   rows = [
     ['opt_sync1_3_0.mp4', '30 seconds', 'Admin', 'Processed'],
     ['opt_sync1_3_0.mp4', '37 seconds', 'Admin', 'Processed']
   ], 
   multimode = false, update = update)
 ```
 Unigui counts rows id as an index in a rows array. If table does not contain append, delete arguments, then it will be drawn without add and remove icons.  
 value = [0] means 0 row is selected in multiselect mode (in array). multimode is False so switch icon for single select mode will be not drawn and switching to single select mode is not allowed.
 
+| Table option parameter |	Description |
+| :---: | :---: | 
+| changed  | table handler accept the selected row number |
+| complete |  Autocomplete handler as with value type (string value, (row index, column index)) that returns a string list of possible complitions |
+| update | called when the user presses the Enter in a table cell |
+| modify | default = accept_rowvalue(table, value). called when the cell value is changed by the user |
+| edit   | default True. if true user can edit table, using standart or overloaded table methods |
+| tools  | default True, then  Table has toolbar with search field and icon action buttons. |
+| show   | default False, the table scrolls to (the first) selected row, if True and it is not visible |
+| multimode | default True, allows to select single or multi selection mode |
 
-By default Table has toolbar with search field and icon action buttons. It is possible to hide it if set 'tools = False' at a Table constructor.
-
-Table shows a paginator if all rows can not be drawn on the screen. Otherwise a table paginator is redundant and omitted.
-
-If the selected row is not on the currently visible page then setting 'show = True' table parameter causes Unigui to switch to the page with the selected row. 
 
 ### Table handlers. ###
 complete, modify and update have the same format as the others elements, but value is consisted from the cell value and its position in the table.
-'update' is called when the user presses the Enter, 'modify' when the cell value is changed by the user. By default it has standart modify method which updates rows data, it can be locked by
-setting 'edit = False' in Table constructor.
-They can return Error or Warning if the value is not accepted, othewise the handler has to call accept_rowvalue(table, value) for accepting the value.
+
+
 ```
 def table_updated(table_, tabval):
     value, position = tabval
     #check value
     ...
     if error_found:
         return Error('Can not accept the value!')
     accept_rowvalue(table_, tabval)
 ```
-The 'changed' table handler accept the selected row number or id as a value.
-
-'editing' handler is called when the user switches the table edit mode. it is optional and has signature editing(table, edit_mode_now) where the second parameter says the table is being edited or not.
 
 ### Chart ###
 Chart is a table with additional Table constructor parameter 'view' which explaines unigui how to draw a chart. The format is '{x index}-{y index1},{y index2}[,..]'. '0-1,2,3' means that x axis values will be taken from 0 column, and y values from 1,2,3 columns of row data.
 'i-3,5' means that x axis values will be equal the row indexes in rows, and y values from 3,5 columns of rows data. If a table constructor got view = '..' parameter then unigui displays a chart icon at the table header, pushing it switches table mode to the chart mode. If a table constructor got type = 'view' in addition to view parameter the table will be displayed as chart on start. In the chart mode pushing the icon button on the top right switches back to table row mode.
 
+### Graph ###
+Graph supports an interactive graph with optional draw methods.
+```
+graph = Graph('X graph', graph_value, graph_selection, 
+    nodes = [
+     { 'id' : 'node1', 'label': "Node 1" },
+     { 'id' : 'node2', 'label': "Node 2" },
+     { 'id' : 'node3', 'label': "Node 3" }    
+  ], edges = [
+     { 'id' : 'edge1', 'source': "node1", 'target': "node2", 'label' : 'extending' },
+     { 'id' :'edge2' , 'source': "node2", 'target': "node3" , 'label' : 'extending'}     
+  ])
+```
+where graph_value is a dictionary like {'nodes' : ["node1"], 'edges' : ['edge3']}, where enumerations are selected nodes and edges.
+Constant graph_default_value == {'nodes' : [], 'edges' : []} i.e. nothing to select.
+
+'changed' method graph_selector called when user (de)selected nodes or edges:
+```
+def graph_selection(_, val):
+    _.value = val
+    if 'nodes' in val:        
+        return Info(f'Nodes {val["nodes"]}') 
+    if 'edges' in val:
+        return Info(f"Edges {val['edges']}") 
+```
+
+Has optional draw 'method' with options 'random', 'circle', 'breadthfirst', by default 'random'.
+
 ### Signals ###
-Unigui supports a dedicated signal event handling mechanism. They are useful in table fields and shared blocks when the containing blocks and screens must respond to their elements without program linking. If a string in a table field started from @ then it considered as a signal. If the user clicks such field in non-edit mode then Unigui generates a signal event, which comes to dispatch function of its containters. First Unigui look at the element block, if not found than at the screen, if not found User.dispatch will be called, which can be redefined for such cases. Any handler can return Signal(element_that_generated_the_event, '@the_event_value') which will be processed.
+Unigui supports a dedicated signal event handling mechanism. It is useful with shared blocks when a containing external blocks screen must respond to their elements without hard program linking. If a string in a table field started from @ then it considered as a signal. If the user interact with such GUI object Unigui generates a signal event, which comes to dispatch function of the screen. First Unigui look at the element block, if not found than at the screen, if not found User.dispatch will be called, which can be redefined for such cases. Any handler can return Signal(element_that_generated_the_event, '@the_event_value') which will be processed.
 
 
 ### Dialog ###
 ```
 Dialog(name, text, callback, buttons, content = None)
 ```
 where buttons is a list of the dialog buttons like ['Yes','No', 'Cancel'].
-Dialog callback has the signature as other with value = pushed button name
+Dialog callback has the signature as other with a pushed button name value
 ```
 def dicallback(current_dialog, bname):
     if bname == 'Yes':
         do_this()
     elif ..
 ```
-content can be filled by any Gui element sequence for additional dialog functionality.
+content can be filled with Gui elements for additional dialog functionality.
+
 
 ### Popup windows ###
 They are intended for non-blocking displaying of error messages and informing about some events, for example, incorrect user input and the completion of a long process on the server.
 ```
 Info(info_message, *someGUIforUpdades)
 Warning(warning_message, *someGUIforUpdades)
 Error(error_message, *someGUIforUpdades)
 ```
 They are returned by handlers and cause appearing on the top screen colored rectangles window for 3 second. someGUIforUpdades is optional GUI enumeration for updating.
 
 For long time processes it is possible to create Progress window. It is just call user.progress in any place.
-Open window user.progress("Analyze .. Wait..")
-Update window message user.progress(" 1% is done..")
+Open window 
+```
+user.progress("Analyze .. Wait..")
+```
+Update window message 
+```
+user.progress(" 1% is done..")
+```
 Close window user.progress(None) or automatically when the handler returns something.
 
 ### Other subtle benefits of a Unigui protocol and technology. ###
-1. Possible to works with any set of resource process servers as a single system, within the same GUI user space, carries out any available operations, including cross, on the fly.
+1. Possible to work with any set of unigui resources as with a single system, within the same GUI user space, carries out any available operations, including crossing, on the fly.
 2. Reproduces and saves sequences of the user interaction with the system without programming. It can be used for complex testing, supporting of security protocols and more.
 3. Possible to mirror a session to other users, works simultaneously in one session for many users.
 
 
 ### Milti-user programming? You don't need it! ###
 Unigui automatically creates and serves an environment for every user.
-The management class is User which contains all required methods for processing and handling the user activity. A programmer can redefine methods in the inherited class, point it as system user class and that is all. Such methods suit for history navigation, undo/redo and initial operations. The screen folder contains screens which are recreated for every user. The same about blocks. The code and modules outside that folders are common for all users as usual. By default Unigui use the system User class and you do not need to point it. If we need special user class logic, we can define own inheritor User.
+The management class is User contains all required methods for processing and handling the user activity. A programmer can redefine methods in the inherited class, point it as system user class and that is all. Such methods suit for history navigation, undo/redo and initial operations. The screen folder contains screens which are recreated for every user. The same about blocks. The code and modules outside that folders are common for all users as usual. By default Unigui use the system User class and you do not need to point it. 
 ```
 class Hello_user(unigui.User):
     def __init__(self):
         super().__init__()
         print('New Hello user connected and created!')
     def dispatch(self, elem, ref):
         if http_link(ref[1:]):
```

### Comparing `unigui-1.3.7/README.md` & `unigui-1.3.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: unigui
+Version: 1.3.8
+Summary: Unigui - Universal app browser
+Home-page: https://github.com/Claus1/unigui
+Author: Georgii Dernovyi
+Author-email: g.dernovoy@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # unigui #
 Universal GUI and App Browser
     Python connector
 
 ### Purpose ###
 Provide a programming technology that does not require front-end programming, for a server written in any language, for displaying on any device, in any resolution, without any tuning. 
 
@@ -38,14 +49,16 @@
 block = Block('X Block',
     [           
         Button('Clean table', icon = 'swipe'),
         Select('Select', value='All', options=['All','Based','Group'])
     ], table, icon = 'api')
 ```
 
+#### Screen function prepare() syncronizes GUI elements one to another and with the program/system data. prepare() is called when the screen open/loaded. prepare() is optional. ###
+
 ### Server start ###
 tests/run_hello.py
 ```
 import unigui
 #app name, port for initial connection and upload_dir folder are optional
 unigui.start('Test app') 
 ```
@@ -69,51 +82,59 @@
 ```
 def clean_table(_, value):
     table.rows = []
     return table
 clean_button = Button('Clean the table’, clean_table)
 ```
 
-‘changed’ handlers have to return Gui object or array of Gui objects that were changed by the handler and Unigui has to redraw or does nothing if all visible elements have the same state. Unigui will do all other jobs for synchronizing automatically. If a Gui object doesn't have 'changed' handler the object accepts incoming value automatically to the 'value' variable of gui object.
+| Handler returns |	Description |
+| :---: | :---: | 
+| Gui object |  Object to update |
+| Gui object array or tuple |  Objects to update |
+| None | Nothing to update, Ok |
+| Error(...), Warning(...), Info(...) | Show to user info about a problem. |
+| UpdateScreen, True | Redraw whole screen |
+| Dialog(..) | Open a dialog with parameters |
 
-If 'value' is not acceptable instead of returning an object possible to return Error or Warning or Info. That functions can update a list object after the message argument, and synchronize simultaneously.
+Unigui	synchronizes GUI state on frontend-end automatically after calling a handler.
 
-#### If a handler returns True or UpdateScreen constant the whole screen will be redrawn. Screen function prepare() syncronizes GUI elements one to another and with the program/system data. prepare() is called when the screen open/loaded. prepare() is optional.
+If a Gui object doesn't have 'changed' handler the object accepts incoming value automatically to the 'value' variable of gui object.
+
+If 'value' is not acceptable instead of returning an object possible to return Error or Warning or Info. That functions can update a object list passed after the message argument.
 
 ```
 def changed_range(_, value):
    if value < 0.5 and value > 1.0:
        #or Error(message, _) if we want to return the previous visible value to the field
        return Error(f‘The value of {_.name} has to be > 0.5 and < 1.0!') 
     #accept value othewise
     _.value = value
 
 edit = Edit('Range of involving', 0.6, changed_range)
 ```
-If the handler returns None (or does not return anything) Unigui considers it as Ok.
 
 ### Block details ###
-The width and height of blocks is calculated automatically depending on their children. It is possible to set the block width and make it scrollable in height, for example for images list. Possible to add MD icon to the header, if required. Width, scroll, .. are optional.
+The width and height of blocks is calculated automatically depending on their children. It is possible to set the block width, or make it scrollable , for example for images list. Possible to add MD icon to the header, if required. width, scroll, height, icon are optional.
 ```
 block = Block(‘Pictures’,add_button, *images, width = 500, scroll = True,icon = 'api')
 ```
  
-The second parameter of the Block constructor is an array of widgets which has to be in the header just after the name.
-Blocks can be shared between the user screens with its states. Such a block has to be located in the blocks folder of the python layer.
+The second parameter of the Block constructor is a widget(s) which are drawn in the block header just after its name.
+Blocks can be shared between the user screens with its states. Such a block has to be located in the 'blocks' folder .
 Examples of such block tests/blocks/tblock.py:
 ```
 from unigui import *
 ..
 concept_block = Block('Concept block',
    [   #some gui elements       
        Button('Run',run_proccess),
        Edit('Working folder','run_folder')
    ], result_table)
 ```
-If some elements are enumerated inside an array, Unigui will display them on a line, otherwise everyone will be displayed on a new own line(s).
+If some elements are enumerated inside an array, Unigui will display them on a line one after another, otherwise everyone will be displayed on a new own line(s).
  
 Using a shared block in some screen:
 ```
 from blocks.tblock import concept_block
 ...
 blocks = [.., concept_block]
 ```
@@ -136,200 +157,246 @@
 #### Example ####
 blocks = [ [b1,b2], [b3, [b4, b5]]]
 #[b1,b2] - the first vertical area, [b3, [b4, b5]] - the second one.
 
 ![alt text](https://github.com/Claus1/unigui/blob/main/tests/multiscreen.png?raw=true)
 
 ### Basic gui elements ###
-Normally they have type property which says unigui how to draw the element. If the type is omitting unigui can detect it by analyzing its content.
-#### If the element name starts from _ , Unigui will not show its name on the screen. ####
-if we need to paint an icon somewhere in the element, add 'icon': 'any MD icon name'.
+Normally they have type property which says unigui what data it contains and optionally how to draw the element. 
+#### If the element name starts from _ , unigui will hide its name on the screen. ####
+if we need to paint an icon in an element, add 'icon': 'any MD icon name' to the element constructor.
 
-#### All constructor parameters are optional for all Gui elements except the first one - name. ####
+#### Most constructor parameters are optional for Gui elements except the first one which is the element name. ####
 
 Common form for element constructors:
 ```
 Gui('Name', value = some_value, changed = changed_handler)
 #It is possible to use short form, that is equal:
 Gui('Name', some_value, changed_handler)
 ```
 calling the method 
 def accept(self, value) 
 causes  a call changed handler if it defined, otherwise just save value to self.value
 
-#### Button ####
+### Button ###
 Normal button.
 ```
 Button('Push me', changed = push_callback) 
 ```
 Short form
 ```
 Button('Push me', push_callback) 
 ```
 Icon button 
 ```
 Button('_Check', push_callback, icon = 'check')
 ```
-#### Load to server Button ####
+
+### Load to server Button ###
 Special button provides file loading from user device or computer to the Unigui server.
 ```
 UploadButton('Load', handler_when_loading_finish, icon='photo_library')
 ```
 handler_when_loading_finish(button_, the_loaded_file_filename) where the_loaded_file_filename is a file name in upload server folder. This folder name is optional upload_dir parameter in unigui.start.
 
-#### Camera Button ####
+### Camera Button ###
 Special button provides to make a photo on the user mobile device. 
 ```
 CameraButton('Make a photo', handler_when_shooting_finish, icon='camera_alt')
 ```
 handler_when_loading_finish(button_, name_of_loaded_file) where name_of_loaded_file is the made photo name in the server folder. This folder name is an
 optional upload_dir parameter in unigui.start.
 
-#### Edit and Text field. ####
+
+### Edit and Text field. ###
 ```
 Edit('Some field', '') #for string value
 Edit('Number field', 0.9) #for numbers
 ```
 If set edit = false it will be readonly field or text label.
 ```
 Edit('Some field', '', edit = false) 
 #is equal to
 Text('Some field')
 ```
-complete handler is optional function which accepts the current field value and returns a string list for autocomplete.
-```
-Edit('Edit me', value = '', complete = get_complete_list) #value has to be string or number
+complete handler is optional function which accepts the current edit value and returns a string list for autocomplete.
 
+```
 def get_complete_list(gui_element, current_value):
     return [s for s in vocab if current_value in s]    
+
+Edit('Edit me', value = '', complete = get_complete_list) #value has to be string or number
 ```
-Can contain optional 'update' handler which is called when the user press Enter in the field.
-It can return None or objects for updating as usual handler.
 
-Can contain optional selection property == (start, end) of selection in the input
-Can contain optional autogrow property, which uses for multiline fileds.
+Optional 'update' handler is called when the user press Enter in the field.
+It can return None if OK or objects for updating as usual 'changed' handler.
 
+Optional selection property with parameters (start, end) is called when selection is happened.
+Optional autogrow property uses for serving multiline fileds.
 
-#### Radio button ####
+
+### Radio button ###
 ```
-Switch('Radio button', value = True[,changed = .., type = ...]) #value has to be boolean, changed, type - optional
+Switch('Radio button', value = True[,changed = .., type = ...])
 
-type can be 'check' for a status button or 'switch' for a switcher . 
+Optional type can be 'check' for a status button or 'switch' for a switcher . 
 ```
 
-#### Select group. Contains options field. ####
+### Select group. Contains options field. ###
 ```
 Select('Select something', "choice1", selection_is_changed, options = ["choice1","choice2", "choice3"]) 
 ```
-can be such type 'toggles','list','dropdown'. Unigui automatically chooses between toogles and dropdown,
-but the user can set type = 'list' then Unigui build it as vertical select list.
+Optional type parameter can be 'toggles','list','dropdown'. Unigui automatically chooses between toogles and dropdown, if type is omitted,
+if type = 'list' then Unigui build it as vertical select list.
+
 
-#### Image. #### 
-width,changed and height are optional, changed is called if the user select/ or touch the image.
+### Image. ###
+width,changed,height,header are optional, changed is called if the user select or touch the image.
 ```
 Image(image_url, header = 'description', changed = selecting_changed, width = .., height = ..)
 ```
 
-#### Video. #### 
+
+### Video. ###
 width and height are optional.
 ```
 Video(video_url, width = .., height = ..)
 ```
 
-#### Tree. The element for tree-like data. ####
+### Tree. The element for tree-like data. ###
 ```
 Tree(name, selected_item_name, changed_handler, options = {name1: parent1, name2 : None, .})
 ```
-options for the data without repeating names, it is dictionary {item_name:parent_name}. 
+options is a tree structure, a dictionary {item_name:parent_name}. 
 
-parent_name and parent_key are None for root items. changed_handler gets item key (name) as value. 
+parent_name is None for root items. changed_handler gets item key (name) as value. 
 
 ### Table. ###
-Tables is common structure for presenting 2D data and charts. Can contain append, delete, update handlers, multimode parameter is True if allowed single and multi select mode. True by default. All of them are optional. When you add a handler for such action Unigui draws and activates an appropriate action icon button in the table header automatically.
+Tables is common structure for presenting 2D data and charts. 
+Optional append, delete, update handlers are called for adding, deleting and updating rows.
+
+
+Assigning a handler for such action causes Unigui to draw and activate an appropriate action icon button in the table header automatically.
 ```
 table = Table('Videos', [0], row_changed, headers = ['Video', 'Duration', 'Owner', 'Status'],  
   rows = [
     ['opt_sync1_3_0.mp4', '30 seconds', 'Admin', 'Processed'],
     ['opt_sync1_3_0.mp4', '37 seconds', 'Admin', 'Processed']
   ], 
   multimode = false, update = update)
 ```
 Unigui counts rows id as an index in a rows array. If table does not contain append, delete arguments, then it will be drawn without add and remove icons.  
 value = [0] means 0 row is selected in multiselect mode (in array). multimode is False so switch icon for single select mode will be not drawn and switching to single select mode is not allowed.
 
+| Table option parameter |	Description |
+| :---: | :---: | 
+| changed  | table handler accept the selected row number |
+| complete |  Autocomplete handler as with value type (string value, (row index, column index)) that returns a string list of possible complitions |
+| update | called when the user presses the Enter in a table cell |
+| modify | default = accept_rowvalue(table, value). called when the cell value is changed by the user |
+| edit   | default True. if true user can edit table, using standart or overloaded table methods |
+| tools  | default True, then  Table has toolbar with search field and icon action buttons. |
+| show   | default False, the table scrolls to (the first) selected row, if True and it is not visible |
+| multimode | default True, allows to select single or multi selection mode |
 
-By default Table has toolbar with search field and icon action buttons. It is possible to hide it if set 'tools = False' at a Table constructor.
-
-Table shows a paginator if all rows can not be drawn on the screen. Otherwise a table paginator is redundant and omitted.
-
-If the selected row is not on the currently visible page then setting 'show = True' table parameter causes Unigui to switch to the page with the selected row. 
 
 ### Table handlers. ###
 complete, modify and update have the same format as the others elements, but value is consisted from the cell value and its position in the table.
-'update' is called when the user presses the Enter, 'modify' when the cell value is changed by the user. By default it has standart modify method which updates rows data, it can be locked by
-setting 'edit = False' in Table constructor.
-They can return Error or Warning if the value is not accepted, othewise the handler has to call accept_rowvalue(table, value) for accepting the value.
+
+
 ```
 def table_updated(table_, tabval):
     value, position = tabval
     #check value
     ...
     if error_found:
         return Error('Can not accept the value!')
     accept_rowvalue(table_, tabval)
 ```
-The 'changed' table handler accept the selected row number or id as a value.
-
-'editing' handler is called when the user switches the table edit mode. it is optional and has signature editing(table, edit_mode_now) where the second parameter says the table is being edited or not.
 
 ### Chart ###
 Chart is a table with additional Table constructor parameter 'view' which explaines unigui how to draw a chart. The format is '{x index}-{y index1},{y index2}[,..]'. '0-1,2,3' means that x axis values will be taken from 0 column, and y values from 1,2,3 columns of row data.
 'i-3,5' means that x axis values will be equal the row indexes in rows, and y values from 3,5 columns of rows data. If a table constructor got view = '..' parameter then unigui displays a chart icon at the table header, pushing it switches table mode to the chart mode. If a table constructor got type = 'view' in addition to view parameter the table will be displayed as chart on start. In the chart mode pushing the icon button on the top right switches back to table row mode.
 
+### Graph ###
+Graph supports an interactive graph with optional draw methods.
+```
+graph = Graph('X graph', graph_value, graph_selection, 
+    nodes = [
+     { 'id' : 'node1', 'label': "Node 1" },
+     { 'id' : 'node2', 'label': "Node 2" },
+     { 'id' : 'node3', 'label': "Node 3" }    
+  ], edges = [
+     { 'id' : 'edge1', 'source': "node1", 'target': "node2", 'label' : 'extending' },
+     { 'id' :'edge2' , 'source': "node2", 'target': "node3" , 'label' : 'extending'}     
+  ])
+```
+where graph_value is a dictionary like {'nodes' : ["node1"], 'edges' : ['edge3']}, where enumerations are selected nodes and edges.
+Constant graph_default_value == {'nodes' : [], 'edges' : []} i.e. nothing to select.
+
+'changed' method graph_selector called when user (de)selected nodes or edges:
+```
+def graph_selection(_, val):
+    _.value = val
+    if 'nodes' in val:        
+        return Info(f'Nodes {val["nodes"]}') 
+    if 'edges' in val:
+        return Info(f"Edges {val['edges']}") 
+```
+
+Has optional draw 'method' with options 'random', 'circle', 'breadthfirst', by default 'random'.
+
 ### Signals ###
-Unigui supports a dedicated signal event handling mechanism. They are useful in table fields and shared blocks when the containing blocks and screens must respond to their elements without program linking. If a string in a table field started from @ then it considered as a signal. If the user clicks such field in non-edit mode then Unigui generates a signal event, which comes to dispatch function of its containters. First Unigui look at the element block, if not found than at the screen, if not found User.dispatch will be called, which can be redefined for such cases. Any handler can return Signal(element_that_generated_the_event, '@the_event_value') which will be processed.
+Unigui supports a dedicated signal event handling mechanism. It is useful with shared blocks when a containing external blocks screen must respond to their elements without hard program linking. If a string in a table field started from @ then it considered as a signal. If the user interact with such GUI object Unigui generates a signal event, which comes to dispatch function of the screen. First Unigui look at the element block, if not found than at the screen, if not found User.dispatch will be called, which can be redefined for such cases. Any handler can return Signal(element_that_generated_the_event, '@the_event_value') which will be processed.
 
 
 ### Dialog ###
 ```
 Dialog(name, text, callback, buttons, content = None)
 ```
 where buttons is a list of the dialog buttons like ['Yes','No', 'Cancel'].
-Dialog callback has the signature as other with value = pushed button name
+Dialog callback has the signature as other with a pushed button name value
 ```
 def dicallback(current_dialog, bname):
     if bname == 'Yes':
         do_this()
     elif ..
 ```
-content can be filled by any Gui element sequence for additional dialog functionality.
+content can be filled with Gui elements for additional dialog functionality.
+
 
 ### Popup windows ###
 They are intended for non-blocking displaying of error messages and informing about some events, for example, incorrect user input and the completion of a long process on the server.
 ```
 Info(info_message, *someGUIforUpdades)
 Warning(warning_message, *someGUIforUpdades)
 Error(error_message, *someGUIforUpdades)
 ```
 They are returned by handlers and cause appearing on the top screen colored rectangles window for 3 second. someGUIforUpdades is optional GUI enumeration for updating.
 
 For long time processes it is possible to create Progress window. It is just call user.progress in any place.
-Open window user.progress("Analyze .. Wait..")
-Update window message user.progress(" 1% is done..")
+Open window 
+```
+user.progress("Analyze .. Wait..")
+```
+Update window message 
+```
+user.progress(" 1% is done..")
+```
 Close window user.progress(None) or automatically when the handler returns something.
 
 ### Other subtle benefits of a Unigui protocol and technology. ###
-1. Possible to works with any set of resource process servers as a single system, within the same GUI user space, carries out any available operations, including cross, on the fly.
+1. Possible to work with any set of unigui resources as with a single system, within the same GUI user space, carries out any available operations, including crossing, on the fly.
 2. Reproduces and saves sequences of the user interaction with the system without programming. It can be used for complex testing, supporting of security protocols and more.
 3. Possible to mirror a session to other users, works simultaneously in one session for many users.
 
 
 ### Milti-user programming? You don't need it! ###
 Unigui automatically creates and serves an environment for every user.
-The management class is User which contains all required methods for processing and handling the user activity. A programmer can redefine methods in the inherited class, point it as system user class and that is all. Such methods suit for history navigation, undo/redo and initial operations. The screen folder contains screens which are recreated for every user. The same about blocks. The code and modules outside that folders are common for all users as usual. By default Unigui use the system User class and you do not need to point it. If we need special user class logic, we can define own inheritor User.
+The management class is User contains all required methods for processing and handling the user activity. A programmer can redefine methods in the inherited class, point it as system user class and that is all. Such methods suit for history navigation, undo/redo and initial operations. The screen folder contains screens which are recreated for every user. The same about blocks. The code and modules outside that folders are common for all users as usual. By default Unigui use the system User class and you do not need to point it. 
 ```
 class Hello_user(unigui.User):
     def __init__(self):
         super().__init__()
         print('New Hello user connected and created!')
     def dispatch(self, elem, ref):
         if http_link(ref[1:]):
```

### Comparing `unigui-1.3.7/setup.py` & `unigui-1.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.3.7',      
+      version='1.3.8',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal app browser',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.3.7/unigui/guielements.py` & `unigui-1.3.8/unigui/guielements.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,19 +86,23 @@
         if not hasattr(self,'width'):
             self.width = 500.0              
         if not hasattr(self,'src'):
             raise "No video src reference!"
         if not hasattr(self,'ratio'):
             self.ratio = "9/9"
 
+graph_default_value = {'nodes' : [], 'edges' : []}
+
 class Graph(Gui):
     '''has to contain nodes, edges, see Readme'''
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.type='graph'
+        if not hasattr(self,'value'):
+            self.value = graph_default_value
         if not hasattr(self,'minwidth'):
             self.minwidth = 600.0              
         if not hasattr(self,'minheight'):
             self.minheight = 600.0              
         self.check('nodes', 'edges')
 
 class Switch(Gui):
```

### Comparing `unigui-1.3.7/unigui/manager.py` & `unigui-1.3.8/unigui/manager.py`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/server.py` & `unigui-1.3.8/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/utils.py` & `unigui-1.3.8/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/css/855.47c4761e.css` & `unigui-1.3.8/unigui/web/css/855.47c4761e.css`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.3.8/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/favicon.ico` & `unigui-1.3.8/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.3.8/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.3.8/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.3.8/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.3.8/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.3.8/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.3.8/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.3.8/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.3.8/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/icons/favicon-128x128.png` & `unigui-1.3.8/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/icons/favicon-16x16.png` & `unigui-1.3.8/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/icons/favicon-32x32.png` & `unigui-1.3.8/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/icons/favicon-96x96.png` & `unigui-1.3.8/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/index.html` & `unigui-1.3.8/unigui/web/index.html`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/js/193.b4cc3ffe.js` & `unigui-1.3.8/unigui/web/js/193.b4cc3ffe.js`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/js/430.4be6e8a8.js` & `unigui-1.3.8/unigui/web/js/430.4be6e8a8.js`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/js/855.e620c0f1.js` & `unigui-1.3.8/unigui/web/js/855.e620c0f1.js`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/js/app.ed80a2d1.js` & `unigui-1.3.8/unigui/web/js/app.ed80a2d1.js`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui/web/js/vendor.c0de6c67.js` & `unigui-1.3.8/unigui/web/js/vendor.c0de6c67.js`

 * *Files identical despite different names*

### Comparing `unigui-1.3.7/unigui.egg-info/PKG-INFO` & `unigui-1.3.8/unigui.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.3.7
+Version: 1.3.8
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -49,14 +49,16 @@
 block = Block('X Block',
     [           
         Button('Clean table', icon = 'swipe'),
         Select('Select', value='All', options=['All','Based','Group'])
     ], table, icon = 'api')
 ```
 
+#### Screen function prepare() syncronizes GUI elements one to another and with the program/system data. prepare() is called when the screen open/loaded. prepare() is optional. ###
+
 ### Server start ###
 tests/run_hello.py
 ```
 import unigui
 #app name, port for initial connection and upload_dir folder are optional
 unigui.start('Test app') 
 ```
@@ -80,51 +82,59 @@
 ```
 def clean_table(_, value):
     table.rows = []
     return table
 clean_button = Button('Clean the table’, clean_table)
 ```
 
-‘changed’ handlers have to return Gui object or array of Gui objects that were changed by the handler and Unigui has to redraw or does nothing if all visible elements have the same state. Unigui will do all other jobs for synchronizing automatically. If a Gui object doesn't have 'changed' handler the object accepts incoming value automatically to the 'value' variable of gui object.
+| Handler returns |	Description |
+| :---: | :---: | 
+| Gui object |  Object to update |
+| Gui object array or tuple |  Objects to update |
+| None | Nothing to update, Ok |
+| Error(...), Warning(...), Info(...) | Show to user info about a problem. |
+| UpdateScreen, True | Redraw whole screen |
+| Dialog(..) | Open a dialog with parameters |
+
+Unigui	synchronizes GUI state on frontend-end automatically after calling a handler.
 
-If 'value' is not acceptable instead of returning an object possible to return Error or Warning or Info. That functions can update a list object after the message argument, and synchronize simultaneously.
+If a Gui object doesn't have 'changed' handler the object accepts incoming value automatically to the 'value' variable of gui object.
 
-#### If a handler returns True or UpdateScreen constant the whole screen will be redrawn. Screen function prepare() syncronizes GUI elements one to another and with the program/system data. prepare() is called when the screen open/loaded. prepare() is optional.
+If 'value' is not acceptable instead of returning an object possible to return Error or Warning or Info. That functions can update a object list passed after the message argument.
 
 ```
 def changed_range(_, value):
    if value < 0.5 and value > 1.0:
        #or Error(message, _) if we want to return the previous visible value to the field
        return Error(f‘The value of {_.name} has to be > 0.5 and < 1.0!') 
     #accept value othewise
     _.value = value
 
 edit = Edit('Range of involving', 0.6, changed_range)
 ```
-If the handler returns None (or does not return anything) Unigui considers it as Ok.
 
 ### Block details ###
-The width and height of blocks is calculated automatically depending on their children. It is possible to set the block width and make it scrollable in height, for example for images list. Possible to add MD icon to the header, if required. Width, scroll, .. are optional.
+The width and height of blocks is calculated automatically depending on their children. It is possible to set the block width, or make it scrollable , for example for images list. Possible to add MD icon to the header, if required. width, scroll, height, icon are optional.
 ```
 block = Block(‘Pictures’,add_button, *images, width = 500, scroll = True,icon = 'api')
 ```
  
-The second parameter of the Block constructor is an array of widgets which has to be in the header just after the name.
-Blocks can be shared between the user screens with its states. Such a block has to be located in the blocks folder of the python layer.
+The second parameter of the Block constructor is a widget(s) which are drawn in the block header just after its name.
+Blocks can be shared between the user screens with its states. Such a block has to be located in the 'blocks' folder .
 Examples of such block tests/blocks/tblock.py:
 ```
 from unigui import *
 ..
 concept_block = Block('Concept block',
    [   #some gui elements       
        Button('Run',run_proccess),
        Edit('Working folder','run_folder')
    ], result_table)
 ```
-If some elements are enumerated inside an array, Unigui will display them on a line, otherwise everyone will be displayed on a new own line(s).
+If some elements are enumerated inside an array, Unigui will display them on a line one after another, otherwise everyone will be displayed on a new own line(s).
  
 Using a shared block in some screen:
 ```
 from blocks.tblock import concept_block
 ...
 blocks = [.., concept_block]
 ```
@@ -147,200 +157,246 @@
 #### Example ####
 blocks = [ [b1,b2], [b3, [b4, b5]]]
 #[b1,b2] - the first vertical area, [b3, [b4, b5]] - the second one.
 
 ![alt text](https://github.com/Claus1/unigui/blob/main/tests/multiscreen.png?raw=true)
 
 ### Basic gui elements ###
-Normally they have type property which says unigui how to draw the element. If the type is omitting unigui can detect it by analyzing its content.
-#### If the element name starts from _ , Unigui will not show its name on the screen. ####
-if we need to paint an icon somewhere in the element, add 'icon': 'any MD icon name'.
+Normally they have type property which says unigui what data it contains and optionally how to draw the element. 
+#### If the element name starts from _ , unigui will hide its name on the screen. ####
+if we need to paint an icon in an element, add 'icon': 'any MD icon name' to the element constructor.
 
-#### All constructor parameters are optional for all Gui elements except the first one - name. ####
+#### Most constructor parameters are optional for Gui elements except the first one which is the element name. ####
 
 Common form for element constructors:
 ```
 Gui('Name', value = some_value, changed = changed_handler)
 #It is possible to use short form, that is equal:
 Gui('Name', some_value, changed_handler)
 ```
 calling the method 
 def accept(self, value) 
 causes  a call changed handler if it defined, otherwise just save value to self.value
 
-#### Button ####
+### Button ###
 Normal button.
 ```
 Button('Push me', changed = push_callback) 
 ```
 Short form
 ```
 Button('Push me', push_callback) 
 ```
 Icon button 
 ```
 Button('_Check', push_callback, icon = 'check')
 ```
-#### Load to server Button ####
+
+### Load to server Button ###
 Special button provides file loading from user device or computer to the Unigui server.
 ```
 UploadButton('Load', handler_when_loading_finish, icon='photo_library')
 ```
 handler_when_loading_finish(button_, the_loaded_file_filename) where the_loaded_file_filename is a file name in upload server folder. This folder name is optional upload_dir parameter in unigui.start.
 
-#### Camera Button ####
+### Camera Button ###
 Special button provides to make a photo on the user mobile device. 
 ```
 CameraButton('Make a photo', handler_when_shooting_finish, icon='camera_alt')
 ```
 handler_when_loading_finish(button_, name_of_loaded_file) where name_of_loaded_file is the made photo name in the server folder. This folder name is an
 optional upload_dir parameter in unigui.start.
 
-#### Edit and Text field. ####
+
+### Edit and Text field. ###
 ```
 Edit('Some field', '') #for string value
 Edit('Number field', 0.9) #for numbers
 ```
 If set edit = false it will be readonly field or text label.
 ```
 Edit('Some field', '', edit = false) 
 #is equal to
 Text('Some field')
 ```
-complete handler is optional function which accepts the current field value and returns a string list for autocomplete.
-```
-Edit('Edit me', value = '', complete = get_complete_list) #value has to be string or number
+complete handler is optional function which accepts the current edit value and returns a string list for autocomplete.
 
+```
 def get_complete_list(gui_element, current_value):
     return [s for s in vocab if current_value in s]    
+
+Edit('Edit me', value = '', complete = get_complete_list) #value has to be string or number
 ```
-Can contain optional 'update' handler which is called when the user press Enter in the field.
-It can return None or objects for updating as usual handler.
 
-Can contain optional selection property == (start, end) of selection in the input
-Can contain optional autogrow property, which uses for multiline fileds.
+Optional 'update' handler is called when the user press Enter in the field.
+It can return None if OK or objects for updating as usual 'changed' handler.
 
+Optional selection property with parameters (start, end) is called when selection is happened.
+Optional autogrow property uses for serving multiline fileds.
 
-#### Radio button ####
+
+### Radio button ###
 ```
-Switch('Radio button', value = True[,changed = .., type = ...]) #value has to be boolean, changed, type - optional
+Switch('Radio button', value = True[,changed = .., type = ...])
 
-type can be 'check' for a status button or 'switch' for a switcher . 
+Optional type can be 'check' for a status button or 'switch' for a switcher . 
 ```
 
-#### Select group. Contains options field. ####
+### Select group. Contains options field. ###
 ```
 Select('Select something', "choice1", selection_is_changed, options = ["choice1","choice2", "choice3"]) 
 ```
-can be such type 'toggles','list','dropdown'. Unigui automatically chooses between toogles and dropdown,
-but the user can set type = 'list' then Unigui build it as vertical select list.
+Optional type parameter can be 'toggles','list','dropdown'. Unigui automatically chooses between toogles and dropdown, if type is omitted,
+if type = 'list' then Unigui build it as vertical select list.
+
 
-#### Image. #### 
-width,changed and height are optional, changed is called if the user select/ or touch the image.
+### Image. ###
+width,changed,height,header are optional, changed is called if the user select or touch the image.
 ```
 Image(image_url, header = 'description', changed = selecting_changed, width = .., height = ..)
 ```
 
-#### Video. #### 
+
+### Video. ###
 width and height are optional.
 ```
 Video(video_url, width = .., height = ..)
 ```
 
-#### Tree. The element for tree-like data. ####
+### Tree. The element for tree-like data. ###
 ```
 Tree(name, selected_item_name, changed_handler, options = {name1: parent1, name2 : None, .})
 ```
-options for the data without repeating names, it is dictionary {item_name:parent_name}. 
+options is a tree structure, a dictionary {item_name:parent_name}. 
 
-parent_name and parent_key are None for root items. changed_handler gets item key (name) as value. 
+parent_name is None for root items. changed_handler gets item key (name) as value. 
 
 ### Table. ###
-Tables is common structure for presenting 2D data and charts. Can contain append, delete, update handlers, multimode parameter is True if allowed single and multi select mode. True by default. All of them are optional. When you add a handler for such action Unigui draws and activates an appropriate action icon button in the table header automatically.
+Tables is common structure for presenting 2D data and charts. 
+Optional append, delete, update handlers are called for adding, deleting and updating rows.
+
+
+Assigning a handler for such action causes Unigui to draw and activate an appropriate action icon button in the table header automatically.
 ```
 table = Table('Videos', [0], row_changed, headers = ['Video', 'Duration', 'Owner', 'Status'],  
   rows = [
     ['opt_sync1_3_0.mp4', '30 seconds', 'Admin', 'Processed'],
     ['opt_sync1_3_0.mp4', '37 seconds', 'Admin', 'Processed']
   ], 
   multimode = false, update = update)
 ```
 Unigui counts rows id as an index in a rows array. If table does not contain append, delete arguments, then it will be drawn without add and remove icons.  
 value = [0] means 0 row is selected in multiselect mode (in array). multimode is False so switch icon for single select mode will be not drawn and switching to single select mode is not allowed.
 
+| Table option parameter |	Description |
+| :---: | :---: | 
+| changed  | table handler accept the selected row number |
+| complete |  Autocomplete handler as with value type (string value, (row index, column index)) that returns a string list of possible complitions |
+| update | called when the user presses the Enter in a table cell |
+| modify | default = accept_rowvalue(table, value). called when the cell value is changed by the user |
+| edit   | default True. if true user can edit table, using standart or overloaded table methods |
+| tools  | default True, then  Table has toolbar with search field and icon action buttons. |
+| show   | default False, the table scrolls to (the first) selected row, if True and it is not visible |
+| multimode | default True, allows to select single or multi selection mode |
 
-By default Table has toolbar with search field and icon action buttons. It is possible to hide it if set 'tools = False' at a Table constructor.
-
-Table shows a paginator if all rows can not be drawn on the screen. Otherwise a table paginator is redundant and omitted.
-
-If the selected row is not on the currently visible page then setting 'show = True' table parameter causes Unigui to switch to the page with the selected row. 
 
 ### Table handlers. ###
 complete, modify and update have the same format as the others elements, but value is consisted from the cell value and its position in the table.
-'update' is called when the user presses the Enter, 'modify' when the cell value is changed by the user. By default it has standart modify method which updates rows data, it can be locked by
-setting 'edit = False' in Table constructor.
-They can return Error or Warning if the value is not accepted, othewise the handler has to call accept_rowvalue(table, value) for accepting the value.
+
+
 ```
 def table_updated(table_, tabval):
     value, position = tabval
     #check value
     ...
     if error_found:
         return Error('Can not accept the value!')
     accept_rowvalue(table_, tabval)
 ```
-The 'changed' table handler accept the selected row number or id as a value.
-
-'editing' handler is called when the user switches the table edit mode. it is optional and has signature editing(table, edit_mode_now) where the second parameter says the table is being edited or not.
 
 ### Chart ###
 Chart is a table with additional Table constructor parameter 'view' which explaines unigui how to draw a chart. The format is '{x index}-{y index1},{y index2}[,..]'. '0-1,2,3' means that x axis values will be taken from 0 column, and y values from 1,2,3 columns of row data.
 'i-3,5' means that x axis values will be equal the row indexes in rows, and y values from 3,5 columns of rows data. If a table constructor got view = '..' parameter then unigui displays a chart icon at the table header, pushing it switches table mode to the chart mode. If a table constructor got type = 'view' in addition to view parameter the table will be displayed as chart on start. In the chart mode pushing the icon button on the top right switches back to table row mode.
 
+### Graph ###
+Graph supports an interactive graph with optional draw methods.
+```
+graph = Graph('X graph', graph_value, graph_selection, 
+    nodes = [
+     { 'id' : 'node1', 'label': "Node 1" },
+     { 'id' : 'node2', 'label': "Node 2" },
+     { 'id' : 'node3', 'label': "Node 3" }    
+  ], edges = [
+     { 'id' : 'edge1', 'source': "node1", 'target': "node2", 'label' : 'extending' },
+     { 'id' :'edge2' , 'source': "node2", 'target': "node3" , 'label' : 'extending'}     
+  ])
+```
+where graph_value is a dictionary like {'nodes' : ["node1"], 'edges' : ['edge3']}, where enumerations are selected nodes and edges.
+Constant graph_default_value == {'nodes' : [], 'edges' : []} i.e. nothing to select.
+
+'changed' method graph_selector called when user (de)selected nodes or edges:
+```
+def graph_selection(_, val):
+    _.value = val
+    if 'nodes' in val:        
+        return Info(f'Nodes {val["nodes"]}') 
+    if 'edges' in val:
+        return Info(f"Edges {val['edges']}") 
+```
+
+Has optional draw 'method' with options 'random', 'circle', 'breadthfirst', by default 'random'.
+
 ### Signals ###
-Unigui supports a dedicated signal event handling mechanism. They are useful in table fields and shared blocks when the containing blocks and screens must respond to their elements without program linking. If a string in a table field started from @ then it considered as a signal. If the user clicks such field in non-edit mode then Unigui generates a signal event, which comes to dispatch function of its containters. First Unigui look at the element block, if not found than at the screen, if not found User.dispatch will be called, which can be redefined for such cases. Any handler can return Signal(element_that_generated_the_event, '@the_event_value') which will be processed.
+Unigui supports a dedicated signal event handling mechanism. It is useful with shared blocks when a containing external blocks screen must respond to their elements without hard program linking. If a string in a table field started from @ then it considered as a signal. If the user interact with such GUI object Unigui generates a signal event, which comes to dispatch function of the screen. First Unigui look at the element block, if not found than at the screen, if not found User.dispatch will be called, which can be redefined for such cases. Any handler can return Signal(element_that_generated_the_event, '@the_event_value') which will be processed.
 
 
 ### Dialog ###
 ```
 Dialog(name, text, callback, buttons, content = None)
 ```
 where buttons is a list of the dialog buttons like ['Yes','No', 'Cancel'].
-Dialog callback has the signature as other with value = pushed button name
+Dialog callback has the signature as other with a pushed button name value
 ```
 def dicallback(current_dialog, bname):
     if bname == 'Yes':
         do_this()
     elif ..
 ```
-content can be filled by any Gui element sequence for additional dialog functionality.
+content can be filled with Gui elements for additional dialog functionality.
+
 
 ### Popup windows ###
 They are intended for non-blocking displaying of error messages and informing about some events, for example, incorrect user input and the completion of a long process on the server.
 ```
 Info(info_message, *someGUIforUpdades)
 Warning(warning_message, *someGUIforUpdades)
 Error(error_message, *someGUIforUpdades)
 ```
 They are returned by handlers and cause appearing on the top screen colored rectangles window for 3 second. someGUIforUpdades is optional GUI enumeration for updating.
 
 For long time processes it is possible to create Progress window. It is just call user.progress in any place.
-Open window user.progress("Analyze .. Wait..")
-Update window message user.progress(" 1% is done..")
+Open window 
+```
+user.progress("Analyze .. Wait..")
+```
+Update window message 
+```
+user.progress(" 1% is done..")
+```
 Close window user.progress(None) or automatically when the handler returns something.
 
 ### Other subtle benefits of a Unigui protocol and technology. ###
-1. Possible to works with any set of resource process servers as a single system, within the same GUI user space, carries out any available operations, including cross, on the fly.
+1. Possible to work with any set of unigui resources as with a single system, within the same GUI user space, carries out any available operations, including crossing, on the fly.
 2. Reproduces and saves sequences of the user interaction with the system without programming. It can be used for complex testing, supporting of security protocols and more.
 3. Possible to mirror a session to other users, works simultaneously in one session for many users.
 
 
 ### Milti-user programming? You don't need it! ###
 Unigui automatically creates and serves an environment for every user.
-The management class is User which contains all required methods for processing and handling the user activity. A programmer can redefine methods in the inherited class, point it as system user class and that is all. Such methods suit for history navigation, undo/redo and initial operations. The screen folder contains screens which are recreated for every user. The same about blocks. The code and modules outside that folders are common for all users as usual. By default Unigui use the system User class and you do not need to point it. If we need special user class logic, we can define own inheritor User.
+The management class is User contains all required methods for processing and handling the user activity. A programmer can redefine methods in the inherited class, point it as system user class and that is all. Such methods suit for history navigation, undo/redo and initial operations. The screen folder contains screens which are recreated for every user. The same about blocks. The code and modules outside that folders are common for all users as usual. By default Unigui use the system User class and you do not need to point it. 
 ```
 class Hello_user(unigui.User):
     def __init__(self):
         super().__init__()
         print('New Hello user connected and created!')
     def dispatch(self, elem, ref):
         if http_link(ref[1:]):
```

### Comparing `unigui-1.3.7/unigui.egg-info/SOURCES.txt` & `unigui-1.3.8/unigui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

