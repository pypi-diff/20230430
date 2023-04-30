# Comparing `tmp/sqlitemanager-0.7.0.tar.gz` & `tmp/sqlitemanager-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlitemanager-0.7.0.tar", last modified: Sun Apr 30 13:12:40 2023, max compression
+gzip compressed data, was "sqlitemanager-0.7.1.tar", last modified: Sun Apr 30 19:27:45 2023, max compression
```

## Comparing `sqlitemanager-0.7.0.tar` & `sqlitemanager-0.7.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 13:12:40.006251 sqlitemanager-0.7.0/
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)    35149 2023-04-30 08:48:58.000000 sqlitemanager-0.7.0/LICENSE
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     3037 2023-04-30 13:12:40.006251 sqlitemanager-0.7.0/PKG-INFO
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     2535 2023-04-30 08:51:23.000000 sqlitemanager-0.7.0/README.md
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)       38 2023-04-30 13:12:40.006251 sqlitemanager-0.7.0/setup.cfg
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)      717 2023-04-30 08:50:48.000000 sqlitemanager-0.7.0/setup.py
-drwxr-xr-x   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 13:12:40.004251 sqlitemanager-0.7.0/sqlitemanager/
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 08:48:58.000000 sqlitemanager-0.7.0/sqlitemanager/__init__.py
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)    32924 2023-04-30 08:49:16.000000 sqlitemanager-0.7.0/sqlitemanager/handler.py
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     7924 2023-04-30 08:49:16.000000 sqlitemanager-0.7.0/sqlitemanager/objects.py
-drwxr-xr-x   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 13:12:40.005251 sqlitemanager-0.7.0/sqlitemanager.egg-info/
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     3037 2023-04-30 13:12:39.000000 sqlitemanager-0.7.0/sqlitemanager.egg-info/PKG-INFO
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)      250 2023-04-30 13:12:39.000000 sqlitemanager-0.7.0/sqlitemanager.egg-info/SOURCES.txt
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)        1 2023-04-30 13:12:39.000000 sqlitemanager-0.7.0/sqlitemanager.egg-info/dependency_links.txt
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)       14 2023-04-30 13:12:39.000000 sqlitemanager-0.7.0/sqlitemanager.egg-info/top_level.txt
+drwxr-xr-x   0 yongshi-fedora  (1000) yongshi-fedora  (1000)        0 2023-04-30 19:27:45.216454 sqlitemanager-0.7.1/
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)    35149 2023-04-13 10:16:08.000000 sqlitemanager-0.7.1/LICENSE
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)     3532 2023-04-30 19:27:45.216454 sqlitemanager-0.7.1/PKG-INFO
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)     3030 2023-04-30 19:27:06.000000 sqlitemanager-0.7.1/README.md
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)       38 2023-04-30 19:27:45.216454 sqlitemanager-0.7.1/setup.cfg
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)      717 2023-04-30 19:24:45.000000 sqlitemanager-0.7.1/setup.py
+drwxr-xr-x   0 yongshi-fedora  (1000) yongshi-fedora  (1000)        0 2023-04-30 19:27:45.215454 sqlitemanager-0.7.1/sqlitemanager/
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)        0 2023-04-13 10:16:08.000000 sqlitemanager-0.7.1/sqlitemanager/__init__.py
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)    32924 2023-04-30 14:45:01.000000 sqlitemanager-0.7.1/sqlitemanager/handler.py
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)     7039 2023-04-30 18:25:11.000000 sqlitemanager-0.7.1/sqlitemanager/objects.py
+drwxr-xr-x   0 yongshi-fedora  (1000) yongshi-fedora  (1000)        0 2023-04-30 19:27:45.216454 sqlitemanager-0.7.1/sqlitemanager.egg-info/
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)     3532 2023-04-30 19:27:45.000000 sqlitemanager-0.7.1/sqlitemanager.egg-info/PKG-INFO
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)      250 2023-04-30 19:27:45.000000 sqlitemanager-0.7.1/sqlitemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)        1 2023-04-30 19:27:45.000000 sqlitemanager-0.7.1/sqlitemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)       14 2023-04-30 19:27:45.000000 sqlitemanager-0.7.1/sqlitemanager.egg-info/top_level.txt
```

### Comparing `sqlitemanager-0.7.0/LICENSE` & `sqlitemanager-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlitemanager-0.7.0/PKG-INFO` & `sqlitemanager-0.7.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,15 @@
-Metadata-Version: 2.1
-Name: sqlitemanager
-Version: 0.7.0
-Summary: Handler object for easy sqlite manipulation
-Home-page: https://github.com/Michael-Yongshi/SQLiteManager
-Author: Michael-Yongshi
-Author-email: 4registration@outlook.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # SQLiteManager
 Use a convenient SQLiteHandler object to manipulate SQLite(3) databases.
 
 ## Version
 
+### 0.7.1
+- added Record.values (list of values)
+
 ### 0.7.0
 - Completely redone, not backwards compatible at all
 - Contains most of the previous functionality
 
 ### 0.6.1
 - extra logging for printing path
 
@@ -58,15 +47,48 @@
 https://github.com/Michael-Yongshi/SQLiteManager/blob/master/unit_tests.py
 
 The sqlite handler is aware of the working directory, if paths are not given it will work from the current working directory.
 It prints the paths its using, so watch closely that its called from the correct one.
 
 ## Tests
 Run test_handler.py in order to test the package.
-For the Gui tests you need PyQt5 and pyqt-darktheme pip packages
+
+# Build
+
+## Pypirc file
+Create a .pypirc file in home directory
+
+```
+[distutils]
+index-servers=
+    pypi
+    test
+
+[test]
+repository = https://test.pypi.org/legacy/
+username = __token__
+password = <PyPI token>
+
+[pypi]
+repository = https://upload.pypi.org/legacy/
+username = __token__
+password = <PyPI token>
+```
+
+## Distributions
+
+```
+python3 -m pip install --upgrade build && python3 -m build
+```
+
+## Upload
+
+```
+python3 -m pip install --upgrade twine && python3 -m twine upload --repository pypi dist/*
+```
 
 ## Licence
 
 Licensed under GPL-3.0-or-later, see LICENSE file for details.
 
 Copyright © 2020 Michael-Yongshi.
```

### Comparing `sqlitemanager-0.7.0/setup.py` & `sqlitemanager-0.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sqlitemanager",
-    version="0.7.0",
+    version="0.7.1",
     author="Michael-Yongshi",
     author_email="4registration@outlook.com",
     description="Handler object for easy sqlite manipulation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Michael-Yongshi/SQLiteManager",
     packages=setuptools.find_packages(),
```

### Comparing `sqlitemanager-0.7.0/sqlitemanager/handler.py` & `sqlitemanager-0.7.1/sqlitemanager/handler.py`

 * *Files identical despite different names*

### Comparing `sqlitemanager-0.7.0/sqlitemanager/objects.py` & `sqlitemanager-0.7.1/sqlitemanager/objects.py`

 * *Files 13% similar despite different names*

```diff
@@ -203,63 +203,36 @@
     name: str
     metadata: dict
     records: list
 
 @dataclass
 class Record:
     """
-    dict: dictionary with key and values
+    table: table name the record came from
+    columns: the (selection of) column names of the table
+    values: list of values
+    dict: for convenience, a dictionary of column / value pairs
 
     record.print() will print the record to the terminal and return the string printed
     """
 
     table: str
     columns: list
+    values: list
     dict: dict
 
     def create_from_sqlrecord(table_name, column_names, values):
 
         record_dict = dict(zip(column_names, values))
-        record_object = Record(table=table_name, columns=column_names, dict=record_dict)
+        record_object = Record(table=table_name, columns=column_names, values=values, dict=record_dict)
 
         return record_object
 
     def print(self):
 
         print_string = ""
         for column_name, value in self.dict.items():
             print_string += f"{column_name}: {value}, "
         print_string = print_string[:-2]
 
         print(print_string)
-        return print_string
-
-
-    # def setvaluepairs(self, column_names):
-    #     self.valuepairs = []
-    #     for index, name in enumerate(column_names[1:]):
-    #         valuepair = [name, self.recordarray[1:][index]]
-    #         self.valuepairs += [valuepair]
-    #     # print(f"set valuepairs {self.valuepairs}")
-
-    # def setrecorddict(self, column_names):
-    #     self.recorddict = {}
-    #     for index, name in enumerate(column_names[1:]):
-    #         self.recorddict.update({name: self.recordarray[1:][index]})
-    #     # print(f"set recorddict {self.recorddict}")
-
-    # def get_column_value(self, column_name):
-    #     """
-    #     method to easily retrieve a value for a specific column
-    #     """
-
-    #     # loop over all records valuepairs
-    #     for valuepair in self.valuepairs:
-            
-    #         # if column name is found return the value
-    #         if valuepair[0] == column_name:
-
-    #             column_value = valuepair[1]
-    #             return column_value
-
-    #     print("Column not found")
-    #     return "Column not found"
+        return print_string
```

### Comparing `sqlitemanager-0.7.0/sqlitemanager.egg-info/PKG-INFO` & `sqlitemanager-0.7.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlitemanager
-Version: 0.7.0
+Version: 0.7.1
 Summary: Handler object for easy sqlite manipulation
 Home-page: https://github.com/Michael-Yongshi/SQLiteManager
 Author: Michael-Yongshi
 Author-email: 4registration@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,17 @@
 License-File: LICENSE
 
 # SQLiteManager
 Use a convenient SQLiteHandler object to manipulate SQLite(3) databases.
 
 ## Version
 
+### 0.7.1
+- added Record.values (list of values)
+
 ### 0.7.0
 - Completely redone, not backwards compatible at all
 - Contains most of the previous functionality
 
 ### 0.6.1
 - extra logging for printing path
 
@@ -58,15 +61,48 @@
 https://github.com/Michael-Yongshi/SQLiteManager/blob/master/unit_tests.py
 
 The sqlite handler is aware of the working directory, if paths are not given it will work from the current working directory.
 It prints the paths its using, so watch closely that its called from the correct one.
 
 ## Tests
 Run test_handler.py in order to test the package.
-For the Gui tests you need PyQt5 and pyqt-darktheme pip packages
+
+# Build
+
+## Pypirc file
+Create a .pypirc file in home directory
+
+```
+[distutils]
+index-servers=
+    pypi
+    test
+
+[test]
+repository = https://test.pypi.org/legacy/
+username = __token__
+password = <PyPI token>
+
+[pypi]
+repository = https://upload.pypi.org/legacy/
+username = __token__
+password = <PyPI token>
+```
+
+## Distributions
+
+```
+python3 -m pip install --upgrade build && python3 -m build
+```
+
+## Upload
+
+```
+python3 -m pip install --upgrade twine && python3 -m twine upload --repository pypi dist/*
+```
 
 ## Licence
 
 Licensed under GPL-3.0-or-later, see LICENSE file for details.
 
 Copyright © 2020 Michael-Yongshi.
```

