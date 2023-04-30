# Comparing `tmp/sqlite_database-0.2.1.tar.gz` & `tmp/sqlite_database-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlite_database-0.2.1.tar", last modified: Wed Apr 26 06:19:30 2023, max compression
+gzip compressed data, was "sqlite_database-0.3.0.tar", last modified: Sun Apr 30 09:24:13 2023, max compression
```

## Comparing `sqlite_database-0.2.1.tar` & `sqlite_database-0.3.0.tar`

### file list

```diff
@@ -1,42 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:30.017416 sqlite_database-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:30.013416 sqlite_database-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:30.013416 sqlite_database-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:30.013416 sqlite_database-0.2.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/Features.md
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/History.md
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-26 06:19:30.017416 sqlite_database-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20541 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/pylint.toml
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-26 06:19:30.017416 sqlite_database-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:30.017416 sqlite_database-0.2.1/sqlite_database/
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/locals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    13963 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/typings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:30.017416 sqlite_database-0.2.1/sqlite_database.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-26 06:19:29.000000 sqlite_database-0.2.1/sqlite_database.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-26 06:19:30.000000 sqlite_database-0.2.1/sqlite_database.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:19:29.000000 sqlite_database-0.2.1/sqlite_database.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 06:19:29.000000 sqlite_database-0.2.1/sqlite_database.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:19:29.000000 sqlite_database-0.2.1/sqlite_database.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:30.017416 sqlite_database-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/tests/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:24:13.343809 sqlite_database-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:24:13.339809 sqlite_database-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:24:13.339809 sqlite_database-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:24:13.339809 sqlite_database-0.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/Features.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/History.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-30 09:24:13.343809 sqlite_database-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/TODO.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:24:13.339809 sqlite_database-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/docs/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/docs/sqlite_database.column.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/docs/sqlite_database.csv.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/docs/sqlite_database.errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/docs/sqlite_database.locals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/docs/sqlite_database.operators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/docs/sqlite_database.query_builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/docs/sqlite_database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/docs/sqlite_database.signature.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/docs/sqlite_database.table.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/docs/sqlite_database.typings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20541 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/pylint.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-30 09:24:13.343809 sqlite_database-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:24:13.343809 sqlite_database-0.3.0/sqlite_database/
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/sqlite_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/sqlite_database/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/sqlite_database/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/sqlite_database/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/sqlite_database/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/sqlite_database/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/sqlite_database/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/sqlite_database/locals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/sqlite_database/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/sqlite_database/query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/sqlite_database/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/sqlite_database/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/sqlite_database/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/sqlite_database/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:24:13.343809 sqlite_database-0.3.0/sqlite_database.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-30 09:24:13.000000 sqlite_database-0.3.0/sqlite_database.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-30 09:24:13.000000 sqlite_database-0.3.0/sqlite_database.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 09:24:13.000000 sqlite_database-0.3.0/sqlite_database.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 09:24:13.000000 sqlite_database-0.3.0/sqlite_database.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 09:24:13.000000 sqlite_database-0.3.0/sqlite_database.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:24:13.343809 sqlite_database-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-04-30 09:24:02.000000 sqlite_database-0.3.0/tests/test_database.py
```

### Comparing `sqlite_database-0.2.1/.github/workflows/pylint.yml` & `sqlite_database-0.3.0/.github/workflows/pylint.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 name: Pylint
 
-on: [push]
+on:
+  push:
+    branches:
+      - 'main'
+    paths:
+      - '**.py'
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.11"]
```

### Comparing `sqlite_database-0.2.1/.github/workflows/python-app.yml` & `sqlite_database-0.3.0/.github/workflows/python-app.yml`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
 
 name: Python application
 
 on:
   push:
     branches: [ "main" ]
+    paths:
+      - '**.py'
   pull_request:
     branches: [ "main" ]
+    paths:
+     - '**.py'
 
 permissions:
   contents: read
 
 jobs:
   build:
```

### Comparing `sqlite_database-0.2.1/.github/workflows/python-publish.yml` & `sqlite_database-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.1/.gitignore` & `sqlite_database-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.1/Features.md` & `sqlite_database-0.3.0/Features.md`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
 `offset` isn't available as parameter yet but exists for `select` method.
 
 ### Update
 
 ```python
 table.update({
-    'row': 1 # What data should change, param name: filter
+    'row': 1 # What data should change
 }, {
     'row': 2 # New data
 })
 ```
 
 You can use `update_one` and `update`. The only difference is that, `update_one` have 3 parameters. (yes, excluding `limit` param.)
 
@@ -184,15 +184,15 @@
 
 ```python
 from sqlite_database.csv import to_csv_file, to_csv_string
 ```
 
 You can use `to_csv_string` than `to_csv_file`, all you need is to pass the table or database.
 
-**Note**: Return type for database is tuple indicating `(name, csv)`,and by that, to_csv_file would make sure that filename passed is a directory and the content will be all table files. E.g: `/path/database/table.csv`
+**Note**: Return type for database is tuple indicating `(name, csv)`,and by that, `to_csv_file` would make sure that filename passed is a directory and the content will be all table files. E.g: `/path/database/table.csv`
 
 ### Export Table
 
 ```python
 # To String
 csv = to_csv_string(db.table("table"))
```

### Comparing `sqlite_database-0.2.1/History.md` & `sqlite_database-0.3.0/History.md`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.1/LICENSE` & `sqlite_database-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.1/PKG-INFO` & `sqlite_database-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 Metadata-Version: 2.1
 Name: sqlite_database
-Version: 0.2.1
+Version: 0.3.0
 Summary: A weird wrapper for SQLite Connection
 Home-page: https://github.com/RimuEirnarn/sqlite_database
 Author: RimuEirnarn
-Author-email: rimuru720@proton.me
+Author-email: Rimu Eirnarn <rimuru720@proton.me>
 License: BSD 3-Clause License
-Project-URL: Source Code, https://github.com/RimuEirnarn/sqlite_database
-Classifier: Programming Language :: Python :: 3
+Project-URL: homepage, https://github.com/RimuEirnarn/sqlite_database
+Project-URL: documentation, https://sqlite-database.rtfd.io
+Project-URL: repository, https://github.com/RimuEirnarn/sqlite_database.git
+Keywords: sqlite,sqlite3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SQLite Database
 
 <div align="center">
 
 ![GitHub forks](https://img.shields.io/github/forks/RimuEirnarn/sqlite_database?style=social)
 ![GitHub Repo stars](https://img.shields.io/github/stars/RimuEirnarn/sqlite_database?style=social)
 
+![GitHub commits difference between two branches/tags/commits](https://img.shields.io/github/commits-difference/RimuEirnarn/sqlite_database?base=main&head=development&label=dev%20-%3E%20main%20%28commits%29)
 ![GitHub closed issues](https://img.shields.io/github/issues-closed-raw/RimuEirnarn/sqlite_database)
 ![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/RimuEirnarn/sqlite_database)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/RimuEirnarn/sqlite_database)
+![Lines of code](https://img.shields.io/tokei/lines/github/RimuEirnarn/sqlite_database)
 ![GitHub all releases](https://img.shields.io/github/downloads/RimuEirnarn/sqlite_database/total)
 ![GitHub Workflow(pylint) Status](https://img.shields.io/github/actions/workflow/status/RimuEirnarn/sqlite_database/pylint.yml?label=lint)
 ![GitHub Workflow(pytest) Status](https://img.shields.io/github/actions/workflow/status/RimuEirnarn/sqlite_database/python-app.yml?label=tests)
 ![GitHub Workflow(pypi) Status](https://img.shields.io/github/actions/workflow/status/RimuEirnarn/sqlite_database/python-publish.yml)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/RimuEirnarn/sqlite_database)
+[![Documentation Status](https://readthedocs.org/projects/sqlite-database/badge/?version=latest)](https://sqlite-database.readthedocs.io/en/latest/?badge=latest)
 ![GitHub](https://img.shields.io/github/license/RimuEirnarn/sqlite_database)
 ![GitHub last commit](https://img.shields.io/github/last-commit/RimuEirnarn/sqlite_database)
     
 ![PyPI - Format](https://img.shields.io/pypi/format/sqlite-database)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sqlite-database)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/sqlite-database)
 
@@ -48,15 +55,15 @@
 
 ## Features
 
 Feature overview can be found in [Features.md](https://github.com/RimuEirnarn/sqlite_database/blob/main/Features.md)
 
 ## History & Pre-contributors
 
-You can read why this library exists by reading [the history](https://github.com/RimuEirnarn/sqlite_database/blob/main/History.md). The pre-contributor is only ChatGPT.
+You can read why this library exists by reading [the history](History.md). The pre-contributor is only ChatGPT.
 
 ## Contributing
 
 You can submit any issue if you found a good issue. You can submit a pull request as long as the thing you want complies with what this project aims for.
 
 ## License
```

### Comparing `sqlite_database-0.2.1/README.md` & `sqlite_database-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # SQLite Database
 
 <div align="center">
 
 ![GitHub forks](https://img.shields.io/github/forks/RimuEirnarn/sqlite_database?style=social)
 ![GitHub Repo stars](https://img.shields.io/github/stars/RimuEirnarn/sqlite_database?style=social)
 
+![GitHub commits difference between two branches/tags/commits](https://img.shields.io/github/commits-difference/RimuEirnarn/sqlite_database?base=main&head=development&label=dev%20-%3E%20main%20%28commits%29)
 ![GitHub closed issues](https://img.shields.io/github/issues-closed-raw/RimuEirnarn/sqlite_database)
 ![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/RimuEirnarn/sqlite_database)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/RimuEirnarn/sqlite_database)
+![Lines of code](https://img.shields.io/tokei/lines/github/RimuEirnarn/sqlite_database)
 ![GitHub all releases](https://img.shields.io/github/downloads/RimuEirnarn/sqlite_database/total)
 ![GitHub Workflow(pylint) Status](https://img.shields.io/github/actions/workflow/status/RimuEirnarn/sqlite_database/pylint.yml?label=lint)
 ![GitHub Workflow(pytest) Status](https://img.shields.io/github/actions/workflow/status/RimuEirnarn/sqlite_database/python-app.yml?label=tests)
 ![GitHub Workflow(pypi) Status](https://img.shields.io/github/actions/workflow/status/RimuEirnarn/sqlite_database/python-publish.yml)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/RimuEirnarn/sqlite_database)
+[![Documentation Status](https://readthedocs.org/projects/sqlite-database/badge/?version=latest)](https://sqlite-database.readthedocs.io/en/latest/?badge=latest)
 ![GitHub](https://img.shields.io/github/license/RimuEirnarn/sqlite_database)
 ![GitHub last commit](https://img.shields.io/github/last-commit/RimuEirnarn/sqlite_database)
     
 ![PyPI - Format](https://img.shields.io/pypi/format/sqlite-database)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sqlite-database)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/sqlite-database)
 
@@ -34,15 +37,15 @@
 
 ## Features
 
 Feature overview can be found in [Features.md](https://github.com/RimuEirnarn/sqlite_database/blob/main/Features.md)
 
 ## History & Pre-contributors
 
-You can read why this library exists by reading [the history](https://github.com/RimuEirnarn/sqlite_database/blob/main/History.md). The pre-contributor is only ChatGPT.
+You can read why this library exists by reading [the history](History.md). The pre-contributor is only ChatGPT.
 
 ## Contributing
 
 You can submit any issue if you found a good issue. You can submit a pull request as long as the thing you want complies with what this project aims for.
 
 ## License
```

### Comparing `sqlite_database-0.2.1/pylint.toml` & `sqlite_database-0.3.0/pylint.toml`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.1/setup.cfg` & `sqlite_database-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.1/sqlite_database/__init__.py` & `sqlite_database-0.3.0/sqlite_database/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,38 +8,40 @@
                      sqlite_multithread_check, AttrDict)
 from .column import BuilderColumn, Column, text, integer, blob, real
 from .locals import this
 from .query_builder import extract_table_creations
 from .signature import op
 from .table import Table
 from .errors import DatabaseExistsError, DatabaseMissingError
+from .config import Config
 Columns = Iterable[Column] | Iterable[BuilderColumn]
 
 IGNORE_TABLE_CHECKS = (
     "sqlite_master", "sqlite_temp_schema", "sqlite_temp_master")
 
 
 class Database:
     """Sqlite3 database, this provide basic integration."""
 
     _active: Mapping[str, "Database"] = WeakValueDictionary()
 
-    def __new__(cls, path: str, **kwargs): # pylint: disable=unused-argument
+    def __new__(cls, path: str, _config: Config | None = None, **kwargs): # pylint: disable=unused-argument
         if path in cls._active:
             return cls._active[path]
         self = object.__new__(cls)
         if path != ":memory:":
-            cls._active[str(path)] = self
+            cls._active[str(path)] = self # type: ignore
         return self
 
-    def __init__(self, path: str, **kwargs) -> None:
+    def __init__(self, path: str, _config: Config | None = None, **kwargs) -> None:
         kwargs['check_same_thread'] = sqlite_multithread_check() != 3
         self._path = path
         self._database = connect(path, **kwargs)
         self._database.row_factory = dict_factory
+        self._config = _config or Config(crunch=False)
         self._closed = False
         self._table_instances: dict[str, Table] = {}
         if not self._closed or self.__dict__.get("_initiated", False) is False:
             self._finalizer_fn = finalize(self, self.close)
             self._initiated = True
 
     def _finalizer(self):
@@ -89,15 +91,15 @@
 
     def table(self, table: str, __columns: Optional[Iterable[Column]] = None):
         """fetch table"""
         if self._table_instances.get(table, None) is not None:
             return self._table_instances[table]
 
         try:
-            this_table = Table(self, table, __columns)
+            this_table = Table(self, table, self._config, __columns)
         except OperationalError as exc:
             raise DatabaseMissingError(f"table {table} does not exists") from exc
         self._table_instances[table] = this_table
         return this_table
 
     def reset_table(self, table: str, columns: Columns) -> Table:
         """Reset existing table with new, this rewrote entire table than altering it."""
@@ -133,18 +135,17 @@
         if self._closed:
             return
         self._database.close()
         if self.path == ":memory:":
             self._closed = True
             return
         if self.path in self._active:
-            del type(self)._active[self.path]
+            del type(self)._active[self.path] # type: ignore
         self._closed = True
 
-    @property
     def tables(self) -> tuple[Table, ...]:
         """Return tuple containing all table except internal tables"""
         master = self.table("sqlite_master")
         listed = []
         for table in master.select():
             if table.type == "table":
                 listed.append(self.table(table.name))
@@ -170,10 +171,10 @@
 
     @property
     def sql(self):
         """SQL Connection"""
         return self._database
 
 
-__version__ = "0.2.1"
+__version__ = "0.3.0"
 __all__ = ["Database", "Table", "op",
            "Column", "null", 'AttrDict', 'text', 'integer', 'real', 'blob']
```

### Comparing `sqlite_database-0.2.1/sqlite_database/_debug.py` & `sqlite_database-0.3.0/sqlite_database/_debug.py`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.1/sqlite_database/_utils.py` & `sqlite_database-0.3.0/sqlite_database/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     _null = object()
     def __init__(self):
         self._ref = self._null
 
     def __get__(self, obj, objtype=None):
         if self._ref is self._null:
             raise ValueError("Reference is null, no object is specified")
-        if (object_ := self._ref()):
+        if (object_ := self._ref()): # type: ignore
             return object_
         raise ObjectRemovedError("object is removed")
 
     def __set__(self, obj, value):
         self._ref = ref(value)
 
 def future_class_var_isdefined(type_: Type[Any], future_attr: str):
```

### Comparing `sqlite_database-0.2.1/sqlite_database/column.py` & `sqlite_database-0.3.0/sqlite_database/column.py`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.1/sqlite_database/csv.py` & `sqlite_database-0.3.0/sqlite_database/csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         selected = selecteds[0]
         csv_writer.writerow(selected)
     return data.getvalue()
 
 
 def _export_database(database: Database) -> list[tuple[str, str]]:
     exported = []
-    for table in database.tables:
+    for table in database.tables():
         exported.append((table.name, _export_table(table)))
     return exported
 
 def _process_database(filename: str, data: list[tuple[str, str]]):
     for table in data:
         base = join_path(filename, f"{table[0]}.csv")
         with open(base, 'w', encoding='utf-8') as file:
```

### Comparing `sqlite_database-0.2.1/sqlite_database/errors.py` & `sqlite_database-0.3.0/sqlite_database/errors.py`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.1/sqlite_database/locals.py` & `sqlite_database-0.3.0/sqlite_database/locals.py`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.1/sqlite_database/operators.py` & `sqlite_database-0.3.0/sqlite_database/operators.py`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.1/sqlite_database/signature.py` & `sqlite_database-0.3.0/sqlite_database/signature.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,44 +6,38 @@
 from .errors import SecurityError
 from .locals import _NO_UNLIKE
 
 
 class Signature:
     """Signature
 
-    This class is used at most filter_ parameters at `Table` class.
+    This class is used at most filter parameters at `Table` class.
 
     You can use variable op (operator) to do all conditional logic or operator.
     There are ==, <=, <, !=, >, and >=
 
     .negate() adds 'not' to the operator, so from == would equal to != when used with
     .negate()
 
     .like() only search for alike characters. Please refer to sqlite like command.
 
     .between() is a ranging operator, there's low and high value.
 
     Example of everything:
-        op == 5
+        >>> op == 5
+        >>> op <= 2
+        >>> op < 2
+        >>> op != 5
+        >>> op > 7
+        >>> op >= 7
+        >>> op.like('Ar%')
+        >>> op.like('Ar_')
+        >>>op.between(1, 10)
 
-        op <= 2
-
-        op < 2
-
-        op != 5
-
-        op > 7
-
-        op >= 7
-
-        op.like('Ar%')
-
-        op.like('Ar_')
-
-        op.between(1, 10)"""
+    You can now use function from :operators:"""
 
     def __init__(self,
                  value: Any = null,
                  operator: Optional[str] = None,
                  data: Optional[tuple[int, int] | str] = None,
                  negate=False) -> None:
         self._value = value
@@ -122,12 +116,15 @@
 
     def generate(self):
         """Generate operator string"""
         string = "not " if self.negated else ""
         string += self._operator
         return string
 
+    def __hash__(self):
+        return hash((self._value, self._data, self._negate, self._operator))
+
     def __repr__(self) -> str:
         return f"<Signature -> {self._operator}>"
 
 
 op = Signature()
```

### Comparing `sqlite_database-0.2.1/sqlite_database/table.py` & `sqlite_database-0.3.0/sqlite_database/table.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 """Table"""
 
-from sqlite3 import OperationalError
+from sqlite3 import Connection, OperationalError
 from typing import Any, Generator, Iterable, NamedTuple, Optional, Type
 
 import weakref
 
-from ._utils import AttrDict, WithCursor, check_iter, check_one, Ref
+
+from .utils import crunch
+from ._utils import check_iter, check_one
 from .column import BuilderColumn, Column
 from .errors import TableRemovedError, UnexpectedResultError
 from .locals import SQLITEPYTYPES
-from .query_builder import (Condition, build_update_data, combine_keyvals,
-                            extract_signature, extract_single_column,
-                            fetch_columns, format_paramable)
+from .query_builder import (Condition, extract_single_column,
+                            fetch_columns, build_select,
+                            build_insert, build_delete,
+                            build_update)
 from .signature import op
 from .typings import (Data, Orders, Queries, Query, TypicalNamedTuple,
-                      _MasterQuery)
+                      _MasterQuery, OnlyColumn)
+from .config import Config
 
 # Let's add a little bit of 'black' magic here.
 
 
 @classmethod
-def get_table(cls):
-    """Get table"""
+def get_table(cls):  # pylint: disable=missing-function-docstring
     return getattr(cls, '_table', None)
 
 
 class Table:
     """Table. Make sure you remember how the table goes."""
 
     _ns: dict[str, Type[NamedTuple]] = {}
-    _parent = Ref()
 
     def __init__(self,
                  parent,  # type: ignore
                  table: str,
+                 db_config: Config | None = None,
                  __columns: Optional[Iterable[Column]] = None) -> None:
-        self._parent = parent
+        self._parent_repr = repr(parent)
+        self._sql: Connection = parent.sql
         self._deleted = False
         self._table = check_one(table)
+        self._config = db_config or Config(crunch=False)
         self._columns: Optional[list[Column]] = list(
             __columns) if __columns else None
         weakref.finalize(self, self._finalize)
 
         if self._columns is None and table != "sqlite_master":
             self._fetch_columns()
 
@@ -53,270 +58,233 @@
             self.select()
         except OperationalError:
             self._deleted = True
 
     def _fetch_columns(self):
         table = self._table
         try:
-            master = self._parent.table("sqlite_master")
-            tabl = master.select_one(
-                {"type": op == "table", "name": op == table})
+            query, data = build_select("sqlite_master",
+                                       {"type": op == "table", "name": op == table})
+            tabl = self._sql.execute(query, data).fetchone()
             if tabl is None:
                 raise ValueError("What the hell?")
             cols = fetch_columns(_MasterQuery(**tabl))
             self._columns = cols
             return 0
         except Exception:  # pylint: disable=broad-except
             return 1
 
-    def _raw_exec(self, query: str, data: dict[str, Any]) -> WithCursor:
+    def _raw_exec(self, query: str, data: dict[str, Any]):
         """No thread safe :("""
-        cursor = self._parent.cursor()
+        cursor = self._sql.cursor()
         cursor.execute(query, data)
         return cursor
 
-    def _mksquery(self,
-                  filter_: Condition = None,
-                  limit: int = 0,
-                  offset: int = 0,
-                  order: Optional[Orders] = None):
-        cond, data = extract_signature(filter_)
-        query = f"select * from {self._table}{' '+cond if cond else ''}"
-        if limit:
-            query += f" limit {limit}"
-        if offset:
-            query += f" offset {offset}"
-        if order:
-            query += " order by"
-            for ord_, order_by in order.items():
-                query += f" {ord_} {order_by},"
-            query = query[:-1]
-        # print(query, data)
-        return query, data
-
-    def _mkuquery(self,
-                  new_data: Data,
-                  filter_: Condition = None,
-                  limit: int = 0,
-                  order: Optional[Orders] = None):
-        cond, data = extract_signature(filter_)
-        new_str, updated = build_update_data(new_data)
-        query = f"update {self._table} set {new_str} {cond}"
-        if limit:
-            query += f" limit {limit}"
-        if order:
-            query += " order by"
-            for ord_, order_by in order.items():
-                query += f" {ord_} {order_by},"
-            query = query[:-1]
-        # print(query, data | _combine_keyvals(updated, new_data))
-        return query, data | combine_keyvals(updated, new_data)
-
-    def _mkdquery(self,
-                  filter_: Condition = None,
-                  limit: int = 0,
-                  order: Optional[Orders] = None):
-        cond, data = extract_signature(filter_)
-        query = f"delete from {self._table} {cond}"
-        if limit:
-            query += f" limit {limit}"
-        if order:
-            query += " order by"
-            for ord_, order_by in order.items():
-                query += f" {ord_} {order_by}"
-            query = query[:-1]
-        # print(query, data)
-        return query, data
-
-    def _mkiquery(self, data: Data):
-        converged = format_paramable(data)
-        query = f"insert into {self._table} ({', '.join(val for val in converged)}) \
-values ({', '.join(val for _,val in converged.items())})"
-        # print(query, data)
-        return query, data
 
     def _control(self):
         if self._deleted:
             raise TableRemovedError(f"{self._table} is already removed")
-        if self._parent.closed:
-            raise ConnectionError("Connection to database was closed.\
- A operation was held but database is already closed.")
 
     def force_nodelete(self):
         """Force "undelete" table. Used if table was mistakenly assigned as
         deleted."""
         self._deleted = True
 
-    def delete(self, filter_: Condition = None, limit: int = 0, order: Optional[Orders] = None):
+    def delete(self, condition: Condition = None, limit: int = 0, order: Optional[Orders] = None):
         """Delete row or rows
 
         Args:
-            filter_ (Condition, optional): Condition to determine deletion
-            See `Signature` class about conditional stuff. Defaults to None.
+            condition (Condition, optional): Condition to determine deletion
+                See `Signature` class about conditional stuff. Defaults to None.
             limit (int, optional): Limit deletion by integer. Defaults to 0.
             order (Optional[Orders], optional): Order of deletion. Defaults to None.
 
         Returns:
             int: Rows affected
         """
-        query, data = self._mkdquery(filter_, limit, order)
+        query, data = build_delete(
+            self._table, condition, limit, order)  # type: ignore
         self._control()
-        cursor = self._parent.sql.execute(query, data)
+        cursor = self._sql.execute(query, data)
         rcount = cursor.rowcount
-        self._parent.sql.commit()
+        self._sql.commit()
         return rcount
 
-    def delete_one(self, filter_: Condition = None, order: Optional[Orders] = None):
+    def delete_one(self, condition: Condition = None, order: Optional[Orders] = None):
         """Delete a row
 
         Args:
-            filter_ (Condition, optional): Conditional to determine deletion.
+            condition (Condition, optional): Conditional to determine deletion.
             Defaults to None.
             order (Optional[Orders], optional): Order of deletion. Defaults to None.
         """
-        return self.delete(filter_, 1, order)
+        return self.delete(condition, 1, order)
 
     def insert(self, data: Data):
         """Insert data to current table
 
         Args:
             data (Data): Data to insert. Make sure it's compatible with the table.
 
         Returns:
             int: Last rowid
         """
-        query, _ = self._mkiquery(data)
+        query, _ = build_insert(self._table, data)  # type: ignore
         self._control()
-        cursor = self._parent.sql.execute(query, data)
+        cursor = self._sql.execute(query, data)
         rlastrowid = cursor.lastrowid
-        self._parent.sql.commit()
+        self._sql.commit()
         return rlastrowid
 
-    def insert_multiple(self, datas: Iterable[Data]):
+    def insert_multiple(self, datas: list[Data]):
         """Insert multiple values
 
         Args:
             datas (Iterable[Data]): Data to be inserted.
         """
         self._control()
-        query, _ = self._mkiquery(datas[0])
-        self._parent.sql.executemany(query, datas)
-        self._parent.sql.commit()
+        query, _ = build_insert(self._table, datas[0])  # type: ignore
+        self._sql.executemany(query, datas)
+        self._sql.commit()
 
-    def insert_many(self, datas: Iterable[Data]):
+    def insert_many(self, datas: list[Data]):
         """Alias to `insert_multiple`"""
         return self.insert_multiple(datas)
 
     def update(self,
-               filter_: Condition | None = None,
+               condition: Condition | None = None,
                data: Data | None = None,
                limit: int = 0,
                order: Optional[Orders] = None):
         """Update rows of current table
 
         Args:
             data (Data): New data to update
-            filter_ (Condition, optional): Condition dictionary
-            See `Signature` about how filter_ works. Defaults to None.
+            condition (Condition, optional): Condition dictionary. 
+                See `Signature` about how condition works. Defaults to None.
             limit (int, optional): Limit updates. Defaults to 0.
             order (Optional[Orders], optional): Order of change. Defaults to None.
 
         Returns:
             int: Rows affected
         """
         if data is None:
             raise ValueError("data parameter must not be None")
-        query, data = self._mkuquery(data, filter_, limit, order)
+        query, data = build_update(
+            self._table, data, condition, limit, order)  # type: ignore
         self._control()
-        cursor = self._parent.sql.execute(query, data)
+        cursor = self._sql.execute(query, data)
         rcount = cursor.rowcount
-        self._parent.sql.commit()
+        self._sql.commit()
         return rcount
 
     def update_one(self,
-                   filter_: Condition | None = None,
+                   condition: Condition | None = None,
                    new_data: Data | None = None,
                    order: Orders | None = None) -> int:
         """Update 1 data only"""
-        return self.update(filter_, new_data, 1, order)
+        return self.update(condition, new_data, 1, order)
 
-    def select(self,
-               filter_: Condition = None,
+    def select(self, # pylint: disable=too-many-arguments
+               condition: Condition = None,
+               only: tuple[str, ...] | None = None,
                limit: int = 0,
                offset: int = 0,
                order: Optional[Orders] = None) -> Queries:
         """Select data in current table. Bare .select() returns all data.
 
         Args:
-            filter_ (Condition, optional): Conditions to used. Defaults to None.
+            condition (Condition, optional): Conditions to used. Defaults to None.
+            only: (OnlyColumn, optional): Select what you want. Default to None.
             limit (int, optional): Limit of select. Defaults to 0.
             offset (int, optional): Offset. Defaults to 0
             order (Optional[Orders], optional): Selection order. Defaults to None.
 
         Returns:
             Queries: Selected data
         """
         self._control()
-        query, data = self._mksquery(filter_, limit, offset, order)
-        with self._parent.sql:
-            return self._parent.sql.execute(query, data).fetchall()
+        query, data = build_select(self._table,
+                                   condition,
+                                   only,
+                                   limit,
+                                   offset,
+                                   order)  # type: ignore
+        with self._sql:
+            data = self._sql.execute(query, data).fetchall()
+            if self._config['crunch']:
+                return crunch(data)
+            return data
 
     def paginate_select(self,
-                        filter_: Condition = None,
+                        condition: Condition = None,
+                        only: OnlyColumn = None,
                         length: int = 10,
                         order: Optional[Orders] = None) -> Generator[Queries, None, None]:
         """Paginate select
 
         Args:
-            filter_ (Condition, optional): Confitions to use. Defaults to None.
+            condition (Condition, optional): Confitions to use. Defaults to None.
+            only: (OnlyColumn, optional): Select what you want. Default to None.
             length (int, optional): Pagination length. Defaults to 10.
             order (Optional[Orders], optional): Order. Defaults to None.
 
         Yields:
             Generator[Queries, None, None]: Step-by-step paginated result.
         """
         self._control()
         start = 0
         while True:
-            query, data = self._mksquery(filter_, length, start, order)
-            with self._parent.sql:
-                fetched: list[AttrDict] = self._parent.sql.execute(
+            query, data = build_select(self._table,
+                                       condition,
+                                       only,
+                                       length,
+                                       start,
+                                       order)  # type: ignore
+            crunched = self._config["crunch"]
+            with self._sql:
+                fetched = self._sql.execute(
                     query, data).fetchmany(length)
                 if len(fetched) == 0:
                     return
+                if crunched:
+                    fetched = crunch(fetched)
                 if len(fetched) != length:
                     yield fetched
                     return
                 yield fetched
                 start += length
 
     def select_one(self,
-                   filter_: Condition = None,
+                   condition: Condition = None,
+                   only: OnlyColumn = None,
                    order: Optional[Orders] = None) -> Query | None:
         """Select one data
 
         Args:
-            filter_ (Condition, optional): Condition to use. Defaults to None.
+            condition (Condition, optional): Condition to use. Defaults to None.
+            only: (OnlyColumn, optional): Select what you want. Default to None.
             order (Optional[Orders], optional): Order of selection. Defaults to None.
 
         Returns:
             Query: Selected data
         """
         self._control()
-        query, data = self._mksquery(filter_, 1, 0, order)
-        with self._parent.sql:
-            return self._parent.sql.execute(query, data).fetchone()
+        query, data = build_select(
+            self._table, condition, only, 1, 0, order)  # type: ignore
+        with self._sql:
+            return self._sql.execute(query, data).fetchone()
 
-    def exists(self, filter_: Condition = None):
+    def exists(self, condition: Condition = None):
         """Check if data is exists or not.
 
         Args:
-            filter_ (Condition, optional): Condition to use. Defaults to None.
+            condition (Condition, optional): Condition to use. Defaults to None.
         """
-        data = self.select_one(filter_)
+        data = self.select_one(condition)
         if data is None:
             return False
         return True
 
     def get_namespace(self) -> Type[TypicalNamedTuple]:
         """Generate or return pre-existed namespace/table."""
         if self._ns.get(self._table, None):
@@ -341,34 +309,34 @@
         for column in self._columns:
             datatypes[column.name] = SQLITEPYTYPES[column.type]
         namedtupled = NamedTuple(self._table.title()+"Table", **datatypes)
 
         self._ns[self._table] = namedtupled
         return namedtupled
 
-    @property
     def columns(self):
         """Table columns"""
         if self._columns is None:
             raise AttributeError("columns is undefined.")
+
         return tuple(self._columns)
 
     @property
     def deleted(self):
         """Is table deleted"""
         return self._deleted
 
     @property
     def name(self):
         """Table name"""
         return self._table
 
     def add_column(self, column: Column | BuilderColumn):
         """Add column to table"""
-        sql = self._parent.sql
+        sql = self._sql
         column = column.to_column() if isinstance(column, BuilderColumn) else column
         if column.primary or column.unique:
             raise OperationalError(
                 "New column cannot have primary or unique constraint")
         if column.nullable is False and column.default is None:
             raise OperationalError("New column cannot be not null while default value is \
 set to null")
@@ -380,14 +348,14 @@
             self._columns.append(column)
         sql.execute(query)
 
     def rename_column(self, old_column: str, new_column: str):
         """Rename existing column to new column"""
         check_iter((old_column, new_column))
         query = f"alter table {self._table} rename column {old_column} to {new_column}"
-        self._parent.sql.execute(query)
+        self._sql.execute(query)
 
     def __repr__(self) -> str:
-        return f"<Table({self._table}) -> {self._parent}>"
+        return f"<Table({self._table}) -> {self._parent_repr}>"
 
 
-__all__ = ['Table', 'get_table']
+__all__ = ['Table']
```

### Comparing `sqlite_database-0.2.1/sqlite_database/typings.py` & `sqlite_database-0.3.0/sqlite_database/typings.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from typing import Any, Literal, Protocol, SupportsIndex, TypedDict
 
 from ._utils import AttrDict
 
 Orders = dict[str, Literal['asc'] | Literal['desc']]
 Data = dict[str, Any]
 Query = AttrDict[str, Any]  # type: ignore
-Queries = list[Query]
+OnlyColumn = tuple[str, ...] | None
+Queries = list[Query] | AttrDict[str, list[Any]] # type: ignore
 null = object()
 
 
 class _MasterQuery(TypedDict):
     """Master Query"""
     type: str
     name: str
```

### Comparing `sqlite_database-0.2.1/sqlite_database.egg-info/PKG-INFO` & `sqlite_database-0.3.0/sqlite_database.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 Metadata-Version: 2.1
 Name: sqlite-database
-Version: 0.2.1
+Version: 0.3.0
 Summary: A weird wrapper for SQLite Connection
 Home-page: https://github.com/RimuEirnarn/sqlite_database
 Author: RimuEirnarn
-Author-email: rimuru720@proton.me
+Author-email: Rimu Eirnarn <rimuru720@proton.me>
 License: BSD 3-Clause License
-Project-URL: Source Code, https://github.com/RimuEirnarn/sqlite_database
-Classifier: Programming Language :: Python :: 3
+Project-URL: homepage, https://github.com/RimuEirnarn/sqlite_database
+Project-URL: documentation, https://sqlite-database.rtfd.io
+Project-URL: repository, https://github.com/RimuEirnarn/sqlite_database.git
+Keywords: sqlite,sqlite3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SQLite Database
 
 <div align="center">
 
 ![GitHub forks](https://img.shields.io/github/forks/RimuEirnarn/sqlite_database?style=social)
 ![GitHub Repo stars](https://img.shields.io/github/stars/RimuEirnarn/sqlite_database?style=social)
 
+![GitHub commits difference between two branches/tags/commits](https://img.shields.io/github/commits-difference/RimuEirnarn/sqlite_database?base=main&head=development&label=dev%20-%3E%20main%20%28commits%29)
 ![GitHub closed issues](https://img.shields.io/github/issues-closed-raw/RimuEirnarn/sqlite_database)
 ![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/RimuEirnarn/sqlite_database)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/RimuEirnarn/sqlite_database)
+![Lines of code](https://img.shields.io/tokei/lines/github/RimuEirnarn/sqlite_database)
 ![GitHub all releases](https://img.shields.io/github/downloads/RimuEirnarn/sqlite_database/total)
 ![GitHub Workflow(pylint) Status](https://img.shields.io/github/actions/workflow/status/RimuEirnarn/sqlite_database/pylint.yml?label=lint)
 ![GitHub Workflow(pytest) Status](https://img.shields.io/github/actions/workflow/status/RimuEirnarn/sqlite_database/python-app.yml?label=tests)
 ![GitHub Workflow(pypi) Status](https://img.shields.io/github/actions/workflow/status/RimuEirnarn/sqlite_database/python-publish.yml)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/RimuEirnarn/sqlite_database)
+[![Documentation Status](https://readthedocs.org/projects/sqlite-database/badge/?version=latest)](https://sqlite-database.readthedocs.io/en/latest/?badge=latest)
 ![GitHub](https://img.shields.io/github/license/RimuEirnarn/sqlite_database)
 ![GitHub last commit](https://img.shields.io/github/last-commit/RimuEirnarn/sqlite_database)
     
 ![PyPI - Format](https://img.shields.io/pypi/format/sqlite-database)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sqlite-database)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/sqlite-database)
 
@@ -48,15 +55,15 @@
 
 ## Features
 
 Feature overview can be found in [Features.md](https://github.com/RimuEirnarn/sqlite_database/blob/main/Features.md)
 
 ## History & Pre-contributors
 
-You can read why this library exists by reading [the history](https://github.com/RimuEirnarn/sqlite_database/blob/main/History.md). The pre-contributor is only ChatGPT.
+You can read why this library exists by reading [the history](History.md). The pre-contributor is only ChatGPT.
 
 ## Contributing
 
 You can submit any issue if you found a good issue. You can submit a pull request as long as the thing you want complies with what this project aims for.
 
 ## License
```

### Comparing `sqlite_database-0.2.1/tests/test_database.py` & `sqlite_database-0.3.0/tests/test_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 from tempfile import mkdtemp
 from pathlib import Path
 
 from pytest import raises
 
 
 from sqlite_database import Column, Database, integer, text
+from sqlite_database.config import Config
 from sqlite_database.signature import op
 from sqlite_database.operators import eq
 from sqlite_database.errors import TableRemovedError
 from sqlite_database.csv import to_csv_string, to_csv_file
+from sqlite_database.utils import crunch
 
 
 def parse(data):
     """parse"""
     return dumps(data, indent=2)
 
 temp_dir = Path(mkdtemp())
@@ -30,14 +32,23 @@
 GROUP_BASE = [{
     "id": 0,
     "name": "root"
 }, {
     "id": 1,
     "name": "user"
 }]
+
+GROUP_BASE_CRUNCHED = crunch(GROUP_BASE)
+
+GROUP_NAMEBASE = [{
+    "name": "root"
+}, {
+    "name": "user"
+}]
+
 USER_BASE = [{
     "id": 0,
     "username": "root",
     "role": "root",
     "gid": 0
 }, {
     "id": 1,
@@ -97,15 +108,15 @@
     groups = database.create_table("groups", [
         integer('id').primary(),
         text('name')
     ])
     groups.insert_many(GROUP_BASE)
     users.insert_many(USER_BASE)
 
-database = Database(temp_dir / "test.db")
+database = Database(temp_dir / "test.db") # type: ignore
 setup_database_builder(database)
 users = database.table('users')
 groups = database.table('groups')
 
 
 def save_report(tid, database, grouptb, usertb):
     """save report"""
@@ -141,14 +152,25 @@
     """Test 002 select"""
     assert groups.select_one({'id': 0}) == GROUP_BASE[0]
     assert groups.select() == GROUP_BASE
     assert users.select_one({'id': 0}) == USER_BASE[0]
     assert users.select() == USER_BASE
     assert save_report("00_test", database, groups, users)
 
+def test_003_select_only():
+    """Test 003 select only"""
+    assert groups.select_one({"id": 0}, ('name',)) == GROUP_NAMEBASE[0]
+    assert save_report("00_test", database, groups, users)
+
+def test_004_select_crunch():
+    """Test 004 select with crunch"""
+    database = Database(":memory:", Config(crunch=True))
+    groups = database.table('groups')
+    setup_database(database)
+    assert groups.select() == GROUP_BASE_CRUNCHED
 
 def test_01_insert():
     """test 01 insert"""
     assert groups.insert_many(GROUP_NEW) is None
     assert users.insert_many(USER_NEW) is None
     assert save_report("01_insert", database, groups, users)
 
@@ -212,19 +234,19 @@
     assert csv
 
 
 def test_08_export_file():
     """Export to CSV file"""
     database = Database(":memory:")
     setup_database(database)
-    assert to_csv_file(database.table('users'), temp_dir / "users.csv")
+    assert to_csv_file(database.table('users'), temp_dir / "users.csv") # type: ignore
 
 def test_09_export_directory():
     """Export to CSV as directory"""
     database = Database(":memory:")
     setup_database(database)
-    assert to_csv_file(database, temp_dir / "MemDB")
+    assert to_csv_file(database, temp_dir / "MemDB") # type: ignore
 
 def test_99_save_report():
     """Save reports"""
     with open(file, "w", encoding="utf-8") as xfile:
         xfile.write(pstdout.getvalue())
```

