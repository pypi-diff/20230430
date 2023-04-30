# Comparing `tmp/excel-sql-engine-1.6.2.tar.gz` & `tmp/excel-sql-engine-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excel-sql-engine-1.6.2.tar", last modified: Tue Apr 25 06:57:24 2023, max compression
+gzip compressed data, was "excel-sql-engine-1.6.3.tar", last modified: Tue Apr 25 15:57:08 2023, max compression
```

## Comparing `excel-sql-engine-1.6.2.tar` & `excel-sql-engine-1.6.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 06:57:24.798802 excel-sql-engine-1.6.2/
--rw-rw-rw-   0        0        0       83 2023-04-23 21:39:10.000000 excel-sql-engine-1.6.2/LICENCE
--rw-rw-rw-   0        0        0     8286 2023-04-25 06:57:24.796764 excel-sql-engine-1.6.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-25 06:57:24.765663 excel-sql-engine-1.6.2/PyxlSql/
--rw-rw-rw-   0        0        0      496 2023-04-24 07:16:16.000000 excel-sql-engine-1.6.2/PyxlSql/__init__.py
--rw-rw-rw-   0        0        0      481 2023-04-24 15:44:58.000000 excel-sql-engine-1.6.2/PyxlSql/__main__.py
--rw-rw-rw-   0        0        0     7162 2023-04-24 08:11:45.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlAbstracts.py
--rw-rw-rw-   0        0        0    15468 2023-04-18 13:41:16.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlArgs.py
--rw-rw-rw-   0        0        0    37463 2023-04-24 12:07:56.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlEngine.py
--rw-rw-rw-   0        0        0     3450 2023-04-24 15:42:26.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlErrors.py
--rw-rw-rw-   0        0        0     9367 2023-04-24 18:03:18.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlFullHelp.py
--rw-rw-rw-   0        0        0    26457 2023-04-24 17:57:14.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlGrammar.py
--rw-rw-rw-   0        0        0      115 2023-04-23 21:45:08.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlLicence.py
--rw-rw-rw-   0        0        0     9159 2023-04-21 18:05:53.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlPivot.py
--rw-rw-rw-   0        0        0     7231 2023-03-21 21:57:15.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlResults.py
--rw-rw-rw-   0        0        0    14165 2023-04-21 18:17:44.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlSheets.py
--rw-rw-rw-   0        0        0    14617 2023-04-24 18:07:21.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlSql.py
--rw-rw-rw-   0        0        0    14413 2023-03-20 16:49:03.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlStages.py
--rw-rw-rw-   0        0        0      493 2023-04-25 06:57:23.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlVersion.py
--rw-rw-rw-   0        0        0    18371 2023-04-24 12:47:48.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlWorkbook.py
--rw-rw-rw-   0        0        0     7585 2023-04-21 09:26:14.000000 excel-sql-engine-1.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 06:57:24.785652 excel-sql-engine-1.6.2/excel_sql_engine.egg-info/
--rw-rw-rw-   0        0        0     8286 2023-04-25 06:57:24.000000 excel-sql-engine-1.6.2/excel_sql_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      664 2023-04-25 06:57:24.000000 excel-sql-engine-1.6.2/excel_sql_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 06:57:24.000000 excel-sql-engine-1.6.2/excel_sql_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-25 06:57:24.000000 excel-sql-engine-1.6.2/excel_sql_engine.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      196 2023-04-20 15:20:18.000000 excel-sql-engine-1.6.2/excel_sql_engine.egg-info/setup.cfg
--rw-rw-rw-   0        0        0        8 2023-04-25 06:57:24.000000 excel-sql-engine-1.6.2/excel_sql_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 06:57:24.798802 excel-sql-engine-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1306 2023-04-25 06:57:23.000000 excel-sql-engine-1.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:57:24.792764 excel-sql-engine-1.6.2/tests/
--rw-rw-rw-   0        0        0     7751 2023-04-24 18:02:02.000000 excel-sql-engine-1.6.2/tests/test_Northwind.py
--rw-rw-rw-   0        0        0     6411 2023-04-24 18:02:02.000000 excel-sql-engine-1.6.2/tests/test_tooling.py
+drwxrwxrwx   0        0        0        0 2023-04-25 15:57:08.350695 excel-sql-engine-1.6.3/
+-rw-rw-rw-   0        0        0    14408 2023-03-13 18:23:44.000000 excel-sql-engine-1.6.3/LICENCE
+-rw-rw-rw-   0        0        0     8286 2023-04-25 15:57:08.348696 excel-sql-engine-1.6.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-25 15:57:08.288695 excel-sql-engine-1.6.3/PyxlSql/
+-rw-rw-rw-   0        0        0      496 2023-04-24 07:16:16.000000 excel-sql-engine-1.6.3/PyxlSql/__init__.py
+-rw-rw-rw-   0        0        0      481 2023-04-24 15:44:58.000000 excel-sql-engine-1.6.3/PyxlSql/__main__.py
+-rw-rw-rw-   0        0        0     7162 2023-04-24 08:11:45.000000 excel-sql-engine-1.6.3/PyxlSql/pyxlAbstracts.py
+-rw-rw-rw-   0        0        0    15468 2023-04-18 13:41:16.000000 excel-sql-engine-1.6.3/PyxlSql/pyxlArgs.py
+-rw-rw-rw-   0        0        0    37463 2023-04-24 12:07:56.000000 excel-sql-engine-1.6.3/PyxlSql/pyxlEngine.py
+-rw-rw-rw-   0        0        0     3450 2023-04-24 15:42:26.000000 excel-sql-engine-1.6.3/PyxlSql/pyxlErrors.py
+-rw-rw-rw-   0        0        0     9367 2023-04-24 18:03:18.000000 excel-sql-engine-1.6.3/PyxlSql/pyxlFullHelp.py
+-rw-rw-rw-   0        0        0    26457 2023-04-24 17:57:14.000000 excel-sql-engine-1.6.3/PyxlSql/pyxlGrammar.py
+-rw-rw-rw-   0        0        0    22568 2023-04-24 18:03:18.000000 excel-sql-engine-1.6.3/PyxlSql/pyxlLicence.py
+-rw-rw-rw-   0        0        0     9159 2023-04-21 18:05:53.000000 excel-sql-engine-1.6.3/PyxlSql/pyxlPivot.py
+-rw-rw-rw-   0        0        0     7231 2023-03-21 21:57:15.000000 excel-sql-engine-1.6.3/PyxlSql/pyxlResults.py
+-rw-rw-rw-   0        0        0    14165 2023-04-21 18:17:44.000000 excel-sql-engine-1.6.3/PyxlSql/pyxlSheets.py
+-rw-rw-rw-   0        0        0    14524 2023-04-25 07:12:29.000000 excel-sql-engine-1.6.3/PyxlSql/pyxlSql.py
+-rw-rw-rw-   0        0        0    14413 2023-03-20 16:49:03.000000 excel-sql-engine-1.6.3/PyxlSql/pyxlStages.py
+-rw-rw-rw-   0        0        0      493 2023-04-25 15:57:07.000000 excel-sql-engine-1.6.3/PyxlSql/pyxlVersion.py
+-rw-rw-rw-   0        0        0    18371 2023-04-24 12:47:48.000000 excel-sql-engine-1.6.3/PyxlSql/pyxlWorkbook.py
+-rw-rw-rw-   0        0        0     7585 2023-04-21 09:26:14.000000 excel-sql-engine-1.6.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 15:57:08.336697 excel-sql-engine-1.6.3/excel_sql_engine.egg-info/
+-rw-rw-rw-   0        0        0     8286 2023-04-25 15:57:08.000000 excel-sql-engine-1.6.3/excel_sql_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      664 2023-04-25 15:57:08.000000 excel-sql-engine-1.6.3/excel_sql_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 15:57:08.000000 excel-sql-engine-1.6.3/excel_sql_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-25 15:57:08.000000 excel-sql-engine-1.6.3/excel_sql_engine.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      196 2023-04-20 15:20:18.000000 excel-sql-engine-1.6.3/excel_sql_engine.egg-info/setup.cfg
+-rw-rw-rw-   0        0        0        8 2023-04-25 15:57:08.000000 excel-sql-engine-1.6.3/excel_sql_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 15:57:08.351699 excel-sql-engine-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1306 2023-04-25 15:57:07.000000 excel-sql-engine-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 15:57:08.344696 excel-sql-engine-1.6.3/tests/
+-rw-rw-rw-   0        0        0     7751 2023-04-24 18:02:02.000000 excel-sql-engine-1.6.3/tests/test_Northwind.py
+-rw-rw-rw-   0        0        0     6411 2023-04-24 18:02:02.000000 excel-sql-engine-1.6.3/tests/test_tooling.py
```

### Comparing `excel-sql-engine-1.6.2/PKG-INFO` & `excel-sql-engine-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel-sql-engine
-Version: 1.6.2
+Version: 1.6.3
 Summary: A tiny SQL engine for Excel files, based on Openpyxl
 Home-page: https://gitlab.com/fabien.battini/pyxlsql
 Author: Fabien BATTINI
 Author-email: fabien.battini@gmail.com
 Keywords: excel sql
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
```

### Comparing `excel-sql-engine-1.6.2/PyxlSql/pyxlAbstracts.py` & `excel-sql-engine-1.6.3/PyxlSql/pyxlAbstracts.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.2/PyxlSql/pyxlArgs.py` & `excel-sql-engine-1.6.3/PyxlSql/pyxlArgs.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.2/PyxlSql/pyxlEngine.py` & `excel-sql-engine-1.6.3/PyxlSql/pyxlEngine.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.2/PyxlSql/pyxlErrors.py` & `excel-sql-engine-1.6.3/PyxlSql/pyxlErrors.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.2/PyxlSql/pyxlFullHelp.py` & `excel-sql-engine-1.6.3/PyxlSql/pyxlFullHelp.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.2/PyxlSql/pyxlGrammar.py` & `excel-sql-engine-1.6.3/PyxlSql/pyxlGrammar.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.2/PyxlSql/pyxlPivot.py` & `excel-sql-engine-1.6.3/PyxlSql/pyxlPivot.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.2/PyxlSql/pyxlResults.py` & `excel-sql-engine-1.6.3/PyxlSql/pyxlResults.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.2/PyxlSql/pyxlSheets.py` & `excel-sql-engine-1.6.3/PyxlSql/pyxlSheets.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.2/PyxlSql/pyxlSql.py` & `excel-sql-engine-1.6.3/PyxlSql/pyxlSql.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,26 +44,28 @@
 # Req 0007: Use API token to upload on Pypi. see  https://pyptoxi.org/help/#apitoken and https://pypi.org/manage/account/token/
 # REQ 0008: Generate to do.rst through tox, using parse_requirements.py
 # REQ 0009: publish also htmlcov on gitlab.io  # noqa
 # REQ 0010: create a downloadable executable for windows user : python -m pip install PyInstaller #
 # TODO: REQ 0011: create a doc specific to windows user that do not know python
 # REQ 0012: manage also .ods files from LibreOffice: NO, this is NOT possible, OpenPyxl does NOT read .ods format
 # REQ 0013: LAZY reading of sheets: only sheets that are referred by the SQL commands are read.
-
 # TODO: REQ 0014: 100% coverage: most of not covered lines are defensive code which is unreachable by design
 # DONE: Update current documentation xxx.rst because @ is often replaced by # in examples, due to more strict typing
-# TODO: REQ 0015 --max-errors = int, default = 20. Maximum number of errors
-# REQ 0016 --full-help : describes the grammar
+#
+
 
 # ----------------------- Cmdline arguments
-# REQ 1001: --dir/-d directory: processes all Excel files in the directory
-# REQ 1002: --file/-f file (multiple times): process this file
-# REQ 1003: --filepath/-p dir (multiple times): adds directory to path for included Excel files
-# REQ 1004: the directory of the file being processed is added in the filepath
+# REQ 1001: positional arguments:  files : file to be processed (multiple times)
+# REQ 1002:  -h, --help            show this help message and exit
+# REQ 1003: --licence, -l         prints the LICENCE
+# REQ 1004: --version             prints the version
+# REQ 1005: --full-help : describes the grammar
 # TODO: REQ 1005: --data-only: reads excel file with the data-only flag
+# TODO: REQ 1006: --max-errors = int, default = 20. Maximum number of errors
+# TODO: REQ 1007: --parse-only : parse commands, verifies syntax only, and exits
 
 # ----------------------- Commands
 
 # REQ 2001: Select_cmd     := "SELECT INTO"  dst_sheet: string  ("AS" Alias)
 #             SELECT INTO adds a FORMULA and a FORMAT clause if the 1st data line is filled with examples-2,
 #             then erases this line
 # REQ 2002: Update_cmd     := "UPDATE" dst_sheet: string
@@ -253,19 +255,18 @@
     def __init__(self, arguments=None):
         super().__init__()
         self.parser = argparse.ArgumentParser(description='execute PyxlSql commands in Excel files')
         # -h, --help is implicit
         self.parser.add_argument('files', help="file to be processed (multiple times)",
                                  type=str, action='append')
 
-        self.parser.add_argument('--filepath', '-p', help="path for included files", type=str, action='append')
         self.parser.add_argument('--licence', '-l', help="prints the LICENCE", action='store_true')
         self.parser.add_argument('--version', help="prints the version", action='store_true')
         self.parser.add_argument('--full-help', help="prints the complete help, and exits", action='store_true')
-        # self.parser.add_argument('--parse-only', help="parse PyxlSql commands, verifies syntax only, and exits",
+        # self.parser.add_argument('--parse-only', help="parse commands, verifies syntax only, and exits",
         #                          action='store_true')
 
         self.args = self.parser.parse_args() if arguments is None else self.parser.parse_args(arguments)
 
         self.files = self.args.files
```

### Comparing `excel-sql-engine-1.6.2/PyxlSql/pyxlStages.py` & `excel-sql-engine-1.6.3/PyxlSql/pyxlStages.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.2/PyxlSql/pyxlWorkbook.py` & `excel-sql-engine-1.6.3/PyxlSql/pyxlWorkbook.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.2/README.md` & `excel-sql-engine-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.2/excel_sql_engine.egg-info/PKG-INFO` & `excel-sql-engine-1.6.3/excel_sql_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel-sql-engine
-Version: 1.6.2
+Version: 1.6.3
 Summary: A tiny SQL engine for Excel files, based on Openpyxl
 Home-page: https://gitlab.com/fabien.battini/pyxlsql
 Author: Fabien BATTINI
 Author-email: fabien.battini@gmail.com
 Keywords: excel sql
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
```

### Comparing `excel-sql-engine-1.6.2/excel_sql_engine.egg-info/SOURCES.txt` & `excel-sql-engine-1.6.3/excel_sql_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.2/setup.py` & `excel-sql-engine-1.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # CAVEAT : This file is edited by tests/patch_files.py to setup the version name from the latest tag
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # see https://setuptools.pypa.io/en/latest/references/keywords.html
 setuptools.setup(
     name="excel-sql-engine",
-    version="1.6.2",
+    version="1.6.3",
     author="Fabien BATTINI",
     author_email="fabien.battini@gmail.com",
     description="A tiny SQL engine for Excel files, based on Openpyxl",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/fabien.battini/pyxlsql",
     license_files=["LICENCE"],
```

### Comparing `excel-sql-engine-1.6.2/tests/test_Northwind.py` & `excel-sql-engine-1.6.3/tests/test_Northwind.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.2/tests/test_tooling.py` & `excel-sql-engine-1.6.3/tests/test_tooling.py`

 * *Files identical despite different names*

