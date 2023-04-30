# Comparing `tmp/pyxx-0.1.0.tar.gz` & `tmp/pyxx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxx-0.1.0.tar", last modified: Sat Mar 18 01:29:51 2023, max compression
+gzip compressed data, was "pyxx-0.2.0.tar", last modified: Sun Apr 30 12:51:08 2023, max compression
```

## Comparing `pyxx-0.1.0.tar` & `pyxx-0.2.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:29:51.648417 pyxx-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-03-18 01:29:04.000000 pyxx-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-18 01:29:04.000000 pyxx-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-03-18 01:29:51.648417 pyxx-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-03-18 01:29:04.000000 pyxx-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:29:51.644417 pyxx-0.1.0/pyxx/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:29:51.644417 pyxx-0.1.0/pyxx/arrays/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/arrays/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:29:51.644417 pyxx-0.1.0/pyxx/arrays/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/arrays/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/arrays/classes/typedlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:29:51.644417 pyxx-0.1.0/pyxx/arrays/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/arrays/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/arrays/functions/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/arrays/functions/equality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/arrays/functions/size.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:29:51.644417 pyxx-0.1.0/pyxx/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:29:51.644417 pyxx-0.1.0/pyxx/files/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/files/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/files/classes/binaryfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/files/classes/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    19237 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/files/classes/textfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/files/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:29:51.644417 pyxx-0.1.0/pyxx/files/functions/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/files/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/files/functions/hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:29:51.644417 pyxx-0.1.0/pyxx/numbers/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/numbers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:29:51.644417 pyxx-0.1.0/pyxx/numbers/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/numbers/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/numbers/functions/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:29:51.644417 pyxx-0.1.0/pyxx/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/strings/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:29:51.648417 pyxx-0.1.0/pyxx/strings/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/strings/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/strings/functions/brackets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/strings/functions/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/strings/functions/split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:29:51.648417 pyxx-0.1.0/pyxx/units/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:29:51.648417 pyxx-0.1.0/pyxx/units/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/units/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15073 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/units/classes/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    19259 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/units/classes/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    27942 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/units/classes/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    30680 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/units/classes/unitconverter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/units/classes/unitsystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/units/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:29:51.648417 pyxx-0.1.0/pyxx/units/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/units/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-03-18 01:29:04.000000 pyxx-0.1.0/pyxx/units/functions/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:29:51.644417 pyxx-0.1.0/pyxx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-03-18 01:29:51.000000 pyxx-0.1.0/pyxx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-18 01:29:51.000000 pyxx-0.1.0/pyxx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 01:29:51.000000 pyxx-0.1.0/pyxx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-18 01:29:51.000000 pyxx-0.1.0/pyxx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-18 01:29:51.000000 pyxx-0.1.0/pyxx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-18 01:29:51.000000 pyxx-0.1.0/pyxx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-18 01:29:04.000000 pyxx-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-18 01:29:51.648417 pyxx-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:51:08.129559 pyxx-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-30 12:50:06.000000 pyxx-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-30 12:50:06.000000 pyxx-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-30 12:51:08.129559 pyxx-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-30 12:50:06.000000 pyxx-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:51:08.125558 pyxx-0.2.0/pyxx/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:51:08.125558 pyxx-0.2.0/pyxx/arrays/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/arrays/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:51:08.125558 pyxx-0.2.0/pyxx/arrays/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/arrays/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/arrays/classes/typedlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:51:08.125558 pyxx-0.2.0/pyxx/arrays/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/arrays/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/arrays/functions/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/arrays/functions/equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/arrays/functions/size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:51:08.125558 pyxx-0.2.0/pyxx/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:51:08.125558 pyxx-0.2.0/pyxx/files/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/files/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/files/classes/binaryfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/files/classes/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19237 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/files/classes/textfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/files/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:51:08.125558 pyxx-0.2.0/pyxx/files/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/files/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/files/functions/hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:51:08.125558 pyxx-0.2.0/pyxx/numbers/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/numbers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:51:08.129559 pyxx-0.2.0/pyxx/numbers/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/numbers/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/numbers/functions/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:51:08.129559 pyxx-0.2.0/pyxx/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/strings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/strings/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:51:08.129559 pyxx-0.2.0/pyxx/strings/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/strings/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/strings/functions/brackets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/strings/functions/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/strings/functions/split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:51:08.129559 pyxx-0.2.0/pyxx/units/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:51:08.129559 pyxx-0.2.0/pyxx/units/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/units/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15073 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/units/classes/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19259 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/units/classes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27942 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/units/classes/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30885 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/units/classes/unitconverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/units/classes/unitsystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/units/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:51:08.129559 pyxx-0.2.0/pyxx/units/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/units/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-04-30 12:50:06.000000 pyxx-0.2.0/pyxx/units/functions/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:51:08.125558 pyxx-0.2.0/pyxx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-30 12:51:08.000000 pyxx-0.2.0/pyxx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-30 12:51:08.000000 pyxx-0.2.0/pyxx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:51:08.000000 pyxx-0.2.0/pyxx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-30 12:51:08.000000 pyxx-0.2.0/pyxx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-30 12:51:08.000000 pyxx-0.2.0/pyxx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 12:51:08.000000 pyxx-0.2.0/pyxx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-30 12:50:06.000000 pyxx-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-30 12:51:08.129559 pyxx-0.2.0/setup.cfg
```

### Comparing `pyxx-0.1.0/LICENSE` & `pyxx-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/PKG-INFO` & `pyxx-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pyxx
-Version: 0.1.0
-Summary: Collection of useful Python utilities and tools
+Version: 0.2.0
+Summary: Collection of utilities for Python code
 Home-page: https://github.com/nathan-hess/python-utilities
 Author: Nathan Hess
 License: MPL-2.0
 Project-URL: Documentation, https://pyxx.readthedocs.io
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyXX: Python Utilities Package
 
 [![CI/CD](https://github.com/nathan-hess/python-utilities/actions/workflows/cicd.yml/badge.svg)](https://github.com/nathan-hess/python-utilities/actions/workflows/cicd.yml)
+[![codecov](https://codecov.io/gh/nathan-hess/python-utilities/branch/main/graph/badge.svg)](https://codecov.io/gh/nathan-hess/python-utilities)
 [![Documentation Status](https://readthedocs.org/projects/pyxx/badge/?version=latest)](https://pyxx.readthedocs.io)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pyxx?label=PyPI%20downloads&logo=python&logoColor=yellow)](https://pypi.org/project/pyxx)
 
 
 ## Overview
 
 PyXX is a collection of Python classes and functions intended to accelerate development of Python code and avoid duplicating code between projects.
```

### Comparing `pyxx-0.1.0/README.md` & `pyxx-0.2.0/pyxx.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,23 @@
+Metadata-Version: 2.1
+Name: pyxx
+Version: 0.2.0
+Summary: Collection of utilities for Python code
+Home-page: https://github.com/nathan-hess/python-utilities
+Author: Nathan Hess
+License: MPL-2.0
+Project-URL: Documentation, https://pyxx.readthedocs.io
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyXX: Python Utilities Package
 
 [![CI/CD](https://github.com/nathan-hess/python-utilities/actions/workflows/cicd.yml/badge.svg)](https://github.com/nathan-hess/python-utilities/actions/workflows/cicd.yml)
+[![codecov](https://codecov.io/gh/nathan-hess/python-utilities/branch/main/graph/badge.svg)](https://codecov.io/gh/nathan-hess/python-utilities)
 [![Documentation Status](https://readthedocs.org/projects/pyxx/badge/?version=latest)](https://pyxx.readthedocs.io)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pyxx?label=PyPI%20downloads&logo=python&logoColor=yellow)](https://pypi.org/project/pyxx)
 
 
 ## Overview
 
 PyXX is a collection of Python classes and functions intended to accelerate development of Python code and avoid duplicating code between projects.
```

### Comparing `pyxx-0.1.0/pyxx/arrays/classes/typedlist.py` & `pyxx-0.2.0/pyxx/arrays/classes/typedlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         ----------
         *values : T
             Items to add to the list when initializing the list
         list_type : Type[T]
             The required type of all items in the list
         print_multiline : bool, optional
             Whether to return a printable string representation of the list in
-            multiline format (default is ``True``).  Multiline format places
+            multiline format (default is ``False``).  Multiline format places
             each item in the list on its own line
         multiline_padding : int, optional
             The amount of horizontal padding to place between brackets and
             list items when creating a printable string representation in
             multiline format (default is ``1``).  Only applicable if
             ``print_multiline`` is ``True``
         """
```

### Comparing `pyxx-0.1.0/pyxx/arrays/functions/convert.py` & `pyxx-0.2.0/pyxx/arrays/functions/convert.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx/arrays/functions/equality.py` & `pyxx-0.2.0/pyxx/arrays/functions/equality.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx/arrays/functions/size.py` & `pyxx-0.2.0/pyxx/arrays/functions/size.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx/files/__init__.py` & `pyxx-0.2.0/pyxx/files/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx/files/classes/file.py` & `pyxx-0.2.0/pyxx/files/classes/file.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx/files/classes/textfile.py` & `pyxx-0.2.0/pyxx/files/classes/textfile.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx/files/functions/hash.py` & `pyxx-0.2.0/pyxx/files/functions/hash.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx/numbers/functions/datatypes.py` & `pyxx-0.2.0/pyxx/numbers/functions/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx/strings/__init__.py` & `pyxx-0.2.0/pyxx/strings/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx/strings/functions/brackets.py` & `pyxx-0.2.0/pyxx/strings/functions/brackets.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx/strings/functions/content.py` & `pyxx-0.2.0/pyxx/strings/functions/content.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx/strings/functions/split.py` & `pyxx-0.2.0/pyxx/strings/functions/split.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx/units/__init__.py` & `pyxx-0.2.0/pyxx/units/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx/units/classes/cli.py` & `pyxx-0.2.0/pyxx/units/classes/cli.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx/units/classes/constants.py` & `pyxx-0.2.0/pyxx/units/classes/constants.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx/units/classes/unit.py` & `pyxx-0.2.0/pyxx/units/classes/unit.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx/units/classes/unitconverter.py` & `pyxx-0.2.0/pyxx/units/classes/unitconverter.py`

 * *Files 1% similar despite different names*

```diff
@@ -534,14 +534,17 @@
 
         Returns
         -------
         bool
             Whether all component unit(s) in ``unit`` are defined in the
             unit converter
         """
+        if unit.strip() == '':
+            return False
+
         component_units = parse_unit(str(unit)).keys()
 
         for component in component_units:
             if component not in self:
                 return False
 
         return True
@@ -734,14 +737,18 @@
 
         Returns
         -------
         Unit
             A :py:class:`Unit` object representation of the unit specified
             by ``unit``
         """
+        if unit.strip() == '':
+            raise UnitNotFoundError(
+                f'Unit "{unit}" consists only of whitespace and is not valid')
+
         parsed_unit = parse_unit(unit)
 
         # For special case of dimensionless units, output a constant unit
         if len(parsed_unit) == 0:
             return Unit(
                 unit_system        = self.unit_system,
                 base_unit_exps     = [0] * self.unit_system.num_base_units,
```

### Comparing `pyxx-0.1.0/pyxx/units/classes/unitsystem.py` & `pyxx-0.2.0/pyxx/units/classes/unitsystem.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx/units/exceptions.py` & `pyxx-0.2.0/pyxx/units/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx/units/functions/parser.py` & `pyxx-0.2.0/pyxx/units/functions/parser.py`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/pyxx.egg-info/PKG-INFO` & `pyxx-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,11 @@
-Metadata-Version: 2.1
-Name: pyxx
-Version: 0.1.0
-Summary: Collection of useful Python utilities and tools
-Home-page: https://github.com/nathan-hess/python-utilities
-Author: Nathan Hess
-License: MPL-2.0
-Project-URL: Documentation, https://pyxx.readthedocs.io
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyXX: Python Utilities Package
 
 [![CI/CD](https://github.com/nathan-hess/python-utilities/actions/workflows/cicd.yml/badge.svg)](https://github.com/nathan-hess/python-utilities/actions/workflows/cicd.yml)
+[![codecov](https://codecov.io/gh/nathan-hess/python-utilities/branch/main/graph/badge.svg)](https://codecov.io/gh/nathan-hess/python-utilities)
 [![Documentation Status](https://readthedocs.org/projects/pyxx/badge/?version=latest)](https://pyxx.readthedocs.io)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pyxx?label=PyPI%20downloads&logo=python&logoColor=yellow)](https://pypi.org/project/pyxx)
 
 
 ## Overview
 
 PyXX is a collection of Python classes and functions intended to accelerate development of Python code and avoid duplicating code between projects.
```

### Comparing `pyxx-0.1.0/pyxx.egg-info/SOURCES.txt` & `pyxx-0.2.0/pyxx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/requirements.txt` & `pyxx-0.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyxx-0.1.0/setup.cfg` & `pyxx-0.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = pyxx
 version = attr: pyxx.__version__
-description = Collection of useful Python utilities and tools
+description = Collection of utilities for Python code
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Nathan Hess
 license = MPL-2.0
 url = https://github.com/nathan-hess/python-utilities
 project_urls = 
 	Documentation = https://pyxx.readthedocs.io
```

