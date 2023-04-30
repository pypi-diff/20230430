# Comparing `tmp/sqlitemanager-0.6.1.tar.gz` & `tmp/sqlitemanager-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlitemanager-0.6.1.tar", last modified: Fri Jan  6 15:23:02 2023, max compression
+gzip compressed data, was "sqlitemanager-0.7.0.tar", last modified: Sun Apr 30 13:12:40 2023, max compression
```

## Comparing `sqlitemanager-0.6.1.tar` & `sqlitemanager-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwxrwxr-x   0 yongshi   (1000) yongshi   (1000)        0 2023-01-06 15:23:02.647632 sqlitemanager-0.6.1/
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)    35149 2021-09-07 17:32:09.000000 sqlitemanager-0.6.1/LICENSE
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)     2637 2023-01-06 15:23:02.647632 sqlitemanager-0.6.1/PKG-INFO
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)     2098 2023-01-06 15:08:42.000000 sqlitemanager-0.6.1/README.md
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)       38 2023-01-06 15:23:02.647632 sqlitemanager-0.6.1/setup.cfg
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)      717 2023-01-06 15:21:56.000000 sqlitemanager-0.6.1/setup.py
-drwxrwxr-x   0 yongshi   (1000) yongshi   (1000)        0 2023-01-06 15:23:02.647632 sqlitemanager-0.6.1/sqlitemanager/
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)        0 2021-09-07 17:32:09.000000 sqlitemanager-0.6.1/sqlitemanager/__init__.py
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)    14902 2023-01-06 14:23:30.000000 sqlitemanager-0.6.1/sqlitemanager/database.py
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)    21690 2023-01-06 15:21:26.000000 sqlitemanager-0.6.1/sqlitemanager/handler.py
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)     1568 2023-01-06 14:58:24.000000 sqlitemanager-0.6.1/sqlitemanager/helpers.py
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)    17725 2021-09-10 19:26:45.000000 sqlitemanager-0.6.1/sqlitemanager/mainwindow.py
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)    13802 2021-09-10 19:28:42.000000 sqlitemanager-0.6.1/sqlitemanager/widgets.py
-drwxrwxr-x   0 yongshi   (1000) yongshi   (1000)        0 2023-01-06 15:23:02.647632 sqlitemanager-0.6.1/sqlitemanager.egg-info/
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)     2637 2023-01-06 15:23:02.000000 sqlitemanager-0.6.1/sqlitemanager.egg-info/PKG-INFO
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)      329 2023-01-06 15:23:02.000000 sqlitemanager-0.6.1/sqlitemanager.egg-info/SOURCES.txt
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)        1 2023-01-06 15:23:02.000000 sqlitemanager-0.6.1/sqlitemanager.egg-info/dependency_links.txt
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)       14 2023-01-06 15:23:02.000000 sqlitemanager-0.6.1/sqlitemanager.egg-info/top_level.txt
+drwxr-xr-x   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 13:12:40.006251 sqlitemanager-0.7.0/
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)    35149 2023-04-30 08:48:58.000000 sqlitemanager-0.7.0/LICENSE
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     3037 2023-04-30 13:12:40.006251 sqlitemanager-0.7.0/PKG-INFO
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     2535 2023-04-30 08:51:23.000000 sqlitemanager-0.7.0/README.md
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)       38 2023-04-30 13:12:40.006251 sqlitemanager-0.7.0/setup.cfg
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)      717 2023-04-30 08:50:48.000000 sqlitemanager-0.7.0/setup.py
+drwxr-xr-x   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 13:12:40.004251 sqlitemanager-0.7.0/sqlitemanager/
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 08:48:58.000000 sqlitemanager-0.7.0/sqlitemanager/__init__.py
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)    32924 2023-04-30 08:49:16.000000 sqlitemanager-0.7.0/sqlitemanager/handler.py
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     7924 2023-04-30 08:49:16.000000 sqlitemanager-0.7.0/sqlitemanager/objects.py
+drwxr-xr-x   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 13:12:40.005251 sqlitemanager-0.7.0/sqlitemanager.egg-info/
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     3037 2023-04-30 13:12:39.000000 sqlitemanager-0.7.0/sqlitemanager.egg-info/PKG-INFO
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)      250 2023-04-30 13:12:39.000000 sqlitemanager-0.7.0/sqlitemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)        1 2023-04-30 13:12:39.000000 sqlitemanager-0.7.0/sqlitemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)       14 2023-04-30 13:12:39.000000 sqlitemanager-0.7.0/sqlitemanager.egg-info/top_level.txt
```

### Comparing `sqlitemanager-0.6.1/LICENSE` & `sqlitemanager-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlitemanager-0.6.1/PKG-INFO` & `sqlitemanager-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: sqlitemanager
-Version: 0.6.1
+Version: 0.7.0
 Summary: Handler object for easy sqlite manipulation
 Home-page: https://github.com/Michael-Yongshi/SQLiteManager
 Author: Michael-Yongshi
 Author-email: 4registration@outlook.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SQLiteManager
 Use a convenient SQLiteHandler object to manipulate SQLite(3) databases.
 
 ## Version
 
+### 0.7.0
+- Completely redone, not backwards compatible at all
+- Contains most of the previous functionality
+
+### 0.6.1
+- extra logging for printing path
+
 ### 0.6.0
 - Extension type can be given to the handler to discern between .sqlite and .sqlite3
 - changed many functions to depend on the location variables of the handler class (path, filename, extension)
 make sure the extension variable does not miss the dot!
 - removed redundent steps or functions, mostly from the database class and added to the handler
 - added some more comments for functions
 - other fixes
@@ -43,16 +48,21 @@
 
 ## Install
 ```
 pip install sqlitemanager
 ```
 
 ## How to
-Primarily use the handler to do database manipulation for you instead of directly edit the data objects. The handler is built to make manipulation of the objects even simpler. See the test_gui.py file for a complete example of how to use the SQLiteHandler.
-https://github.com/Michael-Yongshi/SQLiteManager/blob/master/test_gui.py
+Primarily use the handler to do database manipulation for you instead of directly edit the data objects. The handler is built to make manipulation of the objects even simpler. The Database object contains the actual connection to the database.
+
+See the [example.py](example.py) file for a list of examples of functionality.
+https://github.com/Michael-Yongshi/SQLiteManager/blob/master/unit_tests.py
+
+The sqlite handler is aware of the working directory, if paths are not given it will work from the current working directory.
+It prints the paths its using, so watch closely that its called from the correct one.
 
 ## Tests
 Run test_handler.py in order to test the package.
 For the Gui tests you need PyQt5 and pyqt-darktheme pip packages
 
 ## Licence
 
@@ -61,9 +71,7 @@
 Copyright © 2020 Michael-Yongshi.
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program. If not, see http://www.gnu.org/licenses/.
-
-
```

### Comparing `sqlitemanager-0.6.1/README.md` & `sqlitemanager-0.7.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 # SQLiteManager
 Use a convenient SQLiteHandler object to manipulate SQLite(3) databases.
 
 ## Version
 
+### 0.7.0
+- Completely redone, not backwards compatible at all
+- Contains most of the previous functionality
+
+### 0.6.1
+- extra logging for printing path
+
 ### 0.6.0
 - Extension type can be given to the handler to discern between .sqlite and .sqlite3
 - changed many functions to depend on the location variables of the handler class (path, filename, extension)
 make sure the extension variable does not miss the dot!
 - removed redundent steps or functions, mostly from the database class and added to the handler
 - added some more comments for functions
 - other fixes
@@ -27,16 +34,21 @@
 
 ## Install
 ```
 pip install sqlitemanager
 ```
 
 ## How to
-Primarily use the handler to do database manipulation for you instead of directly edit the data objects. The handler is built to make manipulation of the objects even simpler. See the test_gui.py file for a complete example of how to use the SQLiteHandler.
-https://github.com/Michael-Yongshi/SQLiteManager/blob/master/test_gui.py
+Primarily use the handler to do database manipulation for you instead of directly edit the data objects. The handler is built to make manipulation of the objects even simpler. The Database object contains the actual connection to the database.
+
+See the [example.py](example.py) file for a list of examples of functionality.
+https://github.com/Michael-Yongshi/SQLiteManager/blob/master/unit_tests.py
+
+The sqlite handler is aware of the working directory, if paths are not given it will work from the current working directory.
+It prints the paths its using, so watch closely that its called from the correct one.
 
 ## Tests
 Run test_handler.py in order to test the package.
 For the Gui tests you need PyQt5 and pyqt-darktheme pip packages
 
 ## Licence
```

### Comparing `sqlitemanager-0.6.1/setup.py` & `sqlitemanager-0.7.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sqlitemanager",
-    version="0.6.1",
+    version="0.7.0",
     author="Michael-Yongshi",
     author_email="4registration@outlook.com",
     description="Handler object for easy sqlite manipulation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Michael-Yongshi/SQLiteManager",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.5',
+    python_requires='>=3.7',
 )
```

### Comparing `sqlitemanager-0.6.1/sqlitemanager.egg-info/PKG-INFO` & `sqlitemanager-0.7.0/sqlitemanager.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: sqlitemanager
-Version: 0.6.1
+Version: 0.7.0
 Summary: Handler object for easy sqlite manipulation
 Home-page: https://github.com/Michael-Yongshi/SQLiteManager
 Author: Michael-Yongshi
 Author-email: 4registration@outlook.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SQLiteManager
 Use a convenient SQLiteHandler object to manipulate SQLite(3) databases.
 
 ## Version
 
+### 0.7.0
+- Completely redone, not backwards compatible at all
+- Contains most of the previous functionality
+
+### 0.6.1
+- extra logging for printing path
+
 ### 0.6.0
 - Extension type can be given to the handler to discern between .sqlite and .sqlite3
 - changed many functions to depend on the location variables of the handler class (path, filename, extension)
 make sure the extension variable does not miss the dot!
 - removed redundent steps or functions, mostly from the database class and added to the handler
 - added some more comments for functions
 - other fixes
@@ -43,16 +48,21 @@
 
 ## Install
 ```
 pip install sqlitemanager
 ```
 
 ## How to
-Primarily use the handler to do database manipulation for you instead of directly edit the data objects. The handler is built to make manipulation of the objects even simpler. See the test_gui.py file for a complete example of how to use the SQLiteHandler.
-https://github.com/Michael-Yongshi/SQLiteManager/blob/master/test_gui.py
+Primarily use the handler to do database manipulation for you instead of directly edit the data objects. The handler is built to make manipulation of the objects even simpler. The Database object contains the actual connection to the database.
+
+See the [example.py](example.py) file for a list of examples of functionality.
+https://github.com/Michael-Yongshi/SQLiteManager/blob/master/unit_tests.py
+
+The sqlite handler is aware of the working directory, if paths are not given it will work from the current working directory.
+It prints the paths its using, so watch closely that its called from the correct one.
 
 ## Tests
 Run test_handler.py in order to test the package.
 For the Gui tests you need PyQt5 and pyqt-darktheme pip packages
 
 ## Licence
 
@@ -61,9 +71,7 @@
 Copyright © 2020 Michael-Yongshi.
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program. If not, see http://www.gnu.org/licenses/.
-
-
```

