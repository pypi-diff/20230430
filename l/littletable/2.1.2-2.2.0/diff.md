# Comparing `tmp/littletable-2.1.2.tar.gz` & `tmp/littletable-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "littletable-2.1.2.tar", last modified: Mon Jan 23 23:09:40 2023, max compression
+gzip compressed data, was "littletable-2.2.0.tar", last modified: Sun Apr 30 13:19:15 2023, max compression
```

## Comparing `littletable-2.1.2.tar` & `littletable-2.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-01-23 23:09:40.195256 littletable-2.1.2/
--rw-rw-r--   0 paul      (1000) paul      (1000)    34377 2023-01-23 23:08:34.000000 littletable-2.1.2/CHANGES
--rw-rw-r--   0 paul      (1000) paul      (1000)      247 2022-11-26 14:32:06.000000 littletable-2.1.2/HowToUseLittletable.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)     1080 2022-11-26 14:32:06.000000 littletable-2.1.2/LICENSE
--rw-rw-r--   0 paul      (1000) paul      (1000)      222 2022-11-26 14:32:06.000000 littletable-2.1.2/MANIFEST.in
--rw-rw-r--   0 paul      (1000) paul      (1000)     7654 2023-01-23 23:09:40.195256 littletable-2.1.2/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)     6544 2022-11-26 14:32:06.000000 littletable-2.1.2/README.md
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-01-23 23:09:40.195256 littletable-2.1.2/littletable.egg-info/
--rw-rw-r--   0 paul      (1000) paul      (1000)     7654 2023-01-23 23:09:40.000000 littletable-2.1.2/littletable.egg-info/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)      249 2023-01-23 23:09:40.000000 littletable-2.1.2/littletable.egg-info/SOURCES.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)        1 2023-01-23 23:09:40.000000 littletable-2.1.2/littletable.egg-info/dependency_links.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       12 2023-01-23 23:09:40.000000 littletable-2.1.2/littletable.egg-info/top_level.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)   154133 2023-01-23 23:08:34.000000 littletable-2.1.2/littletable.py
--rw-rw-r--   0 paul      (1000) paul      (1000)       38 2023-01-23 23:09:40.195256 littletable-2.1.2/setup.cfg
--rw-rw-r--   0 paul      (1000) paul      (1000)     1515 2022-11-26 14:32:06.000000 littletable-2.1.2/setup.py
--rw-rw-r--   0 paul      (1000) paul      (1000)   102936 2022-11-30 00:36:09.000000 littletable-2.1.2/unit_tests.py
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-04-30 13:19:15.010700 littletable-2.2.0/
+-rw-rw-r--   0 paul      (1000) paul      (1000)    35549 2023-04-30 13:18:52.000000 littletable-2.2.0/CHANGES
+-rw-rw-r--   0 paul      (1000) paul      (1000)      247 2023-04-30 06:48:17.000000 littletable-2.2.0/HowToUseLittletable.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1080 2023-04-30 06:48:17.000000 littletable-2.2.0/LICENSE
+-rw-rw-r--   0 paul      (1000) paul      (1000)      222 2023-04-30 06:48:17.000000 littletable-2.2.0/MANIFEST.in
+-rw-rw-r--   0 paul      (1000) paul      (1000)     7490 2023-04-30 13:19:15.010700 littletable-2.2.0/PKG-INFO
+-rw-rw-r--   0 paul      (1000) paul      (1000)     6449 2023-04-30 06:48:17.000000 littletable-2.2.0/README.md
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-04-30 13:19:15.010700 littletable-2.2.0/littletable.egg-info/
+-rw-rw-r--   0 paul      (1000) paul      (1000)     7490 2023-04-30 13:19:14.000000 littletable-2.2.0/littletable.egg-info/PKG-INFO
+-rw-rw-r--   0 paul      (1000) paul      (1000)      249 2023-04-30 13:19:14.000000 littletable-2.2.0/littletable.egg-info/SOURCES.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)        1 2023-04-30 13:19:14.000000 littletable-2.2.0/littletable.egg-info/dependency_links.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)       12 2023-04-30 13:19:14.000000 littletable-2.2.0/littletable.egg-info/top_level.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)   160733 2023-04-30 06:48:17.000000 littletable-2.2.0/littletable.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)       38 2023-04-30 13:19:15.014700 littletable-2.2.0/setup.cfg
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1467 2023-04-30 06:48:17.000000 littletable-2.2.0/setup.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)   105877 2023-04-30 07:01:19.000000 littletable-2.2.0/unit_tests.py
```

### Comparing `littletable-2.1.2/CHANGES` & `littletable-2.2.0/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,50 @@
 Change History
 ==============
 
+NOTE: Deprecated features will be removed in the 3.0 release of littletable:
+- DataObject class, replace with typing.SimpleNamespace, dict, namedtuple, or
+  other user-defined class
+- Table.re_match(patt) comparator is deprecated, replace with
+  re.compile(patt).match
+
+
+Version 2.2.0
+-------------
+- BREAKING CHANGES:
+
+    - Support for Python versions <3.9 is dropped in this version. To run on
+      these older Python's, use `littletable` 2.1.2.
+
+    - The results from full text searches now return a Table by default.
+
+- Added `DeprecationWarning` for usage of `DataObject` class. New code should
+  use `types.SimpleNamespaces`, or just plain Python dicts (which get stored
+  as `SimpleNamespaces`), namedtuples, or other user-defined class.
+
+- Text search handles common English regular and irregular plural forms and
+  resolves to their singular forms for word searching.
+
+- The Table of results returned from a full text search now gets titled with
+  the search query string.
+
+- A new example for full text searches is included, `star_trek_tos.py`,
+  illustrating CSV import and table sorting, and searching episode descriptions
+  for keywords.
+
+
 Version 2.1.2
 -------------
 - Added `json_encoder` argument to `Table.json_export`, so that custom data
-  fields can get exported without raising JSONEncodeError. peps.py example
+  fields can get exported without raising `JSONEncodeError`. `peps.py` example
   has been modified to demonstrate this. The `json_encoder` argument can
-  take a single JSONEncoder subclass, or a tuple of subclasses, to be tried
+  take a single `JSONEncoder` subclass, or a tuple of subclasses, to be tried
   in sequence. Each should follow the pattern given in the online Python
   docs for the json module. (See updated code in examples/peps.py to see a
-  custom JSONEncoder.)
+  custom `JSONEncoder`.)
 
   Also added `json_decoder` argument to `Table.json_import`, though it only
   supports passing a single class.
 
 
 Version 2.1.1
 -------------
@@ -31,15 +62,15 @@
 
 - Added docstring and annotations for generated `table.search.<search_attr>` methods.
 
 - Added docstring for generated `table.by.<index_attr>` methods, and more explanation
   in `create_index()` docstring on how to use indexed fields.
 
 - Passing an unknown path element in `Table.json_import(path=path)` now raises
-  KeyError instead of unhelpful TypeError.
+  `KeyError` instead of unhelpful `TypeError`.
 
 
 Version 2.1.0
 -------------
 - BREAKING CHANGES:
 
   - littletable drops support for Python 3.6.
@@ -72,16 +103,16 @@
   the output destination (None is now the default), will return a string
   containing the exported data.
 
     # print first 10 rows of my_table as CSV data
     print(my_table[:10].csv_export())
 
 - `Table.json_export()` takes an optional parameter, `streaming` to control
-  whether the resulting JSON is a single JSON list element (if streaming is False),
-  or a separate JSON element per Table item (if streaming is True); the default
+  whether the resulting JSON is a single JSON list element (if `streaming` is False),
+  or a separate JSON element per Table item (if `streaming` is True); the default
   value is False. `streaming` is useful when passing data over a streaming protocol,
   so that the Table contents can be unmarshaled separately on the receiving end.
 
 - `Table.json_import()` takes two optional parameters:
 
   - `streaming` to indicate that the input stream contains multiple JSON objects
     (if streaming=True), or a single JSON list of objects (if streaming=False);
```

### Comparing `littletable-2.1.2/LICENSE` & `littletable-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `littletable-2.1.2/PKG-INFO` & `littletable-2.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: littletable
-Version: 2.1.2
+Version: 2.2.0
 Summary: Python in-memory ORM database
 Home-page: https://github.com/ptmcg/littletable/
+Download-URL: https://pypi.org/project/littletable/
 Author: Paul McGuire
 Author-email: ptmcg@austin.rr.com
 License: MIT License
-Download-URL: https://pypi.org/project/littletable/
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # littletable - a Python module to give ORM-like access to a collection of objects
 [![Build Status](https://travis-ci.org/ptmcg/littletable.svg?branch=master)](https://travis-ci.org/ptmcg/littletable) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ptmcg/littletable/master)
 
 - [Introduction](#introduction)
@@ -137,28 +135,31 @@
 Extended "getting started" notes at [how_to_use_littletable.md](https://github.com/ptmcg/littletable/blob/master/how_to_use_littletable.md).
 
 Sample Demo
 -----------
 Here is a simple littletable data storage/retrieval example:
 
 ```python
-from littletable import Table, DataObject
+from littletable import Table
 
 customers = Table('customers')
 customers.create_index("id", unique=True)
-customers.insert(DataObject(id="0010", name="George Jetson"))
-customers.insert(DataObject(id="0020", name="Wile E. Coyote"))
-customers.insert(DataObject(id="0030", name="Jonny Quest"))
+customers.csv_import("""\
+id,name
+0010,George Jetson
+0020,Wile E. Coyote
+0030,Jonny Quest
+""")
 
 catalog = Table('catalog')
 catalog.create_index("sku", unique=True)
-catalog.insert(DataObject(sku="ANVIL-001", descr="1000lb anvil", unitofmeas="EA",unitprice=100))
-catalog.insert(DataObject(sku="BRDSD-001", descr="Bird seed", unitofmeas="LB",unitprice=3))
-catalog.insert(DataObject(sku="MAGNT-001", descr="Magnet", unitofmeas="EA",unitprice=8))
-catalog.insert(DataObject(sku="MAGLS-001", descr="Magnifying glass", unitofmeas="EA",unitprice=12))
+catalog.insert({"sku": "ANVIL-001", "descr": "1000lb anvil", "unitofmeas": "EA","unitprice": 100})
+catalog.insert({"sku": "BRDSD-001", "descr": "Bird seed", "unitofmeas": "LB","unitprice": 3})
+catalog.insert({"sku": "MAGNT-001", "descr": "Magnet", "unitofmeas": "EA","unitprice": 8})
+catalog.insert({"sku": "MAGLS-001", "descr": "Magnifying glass", "unitofmeas": "EA","unitprice": 12})
 
 wishitems = Table('wishitems')
 wishitems.create_index("custid")
 wishitems.create_index("sku")
 
 # easy to import CSV data from a string or file
 wishitems.csv_import("""\
@@ -166,15 +167,15 @@
 0020,ANVIL-001
 0020,BRDSD-001
 0020,MAGNT-001
 0030,MAGNT-001
 0030,MAGLS-001
 """)
 
-# print a particular customer name 
+# print a particular customer name
 # (unique indexes will return a single item; non-unique
 # indexes will return a list of all matching items)
 print(customers.by.id["0030"].name)
 
 # see all customer names
 for name in customers.all.name:
     print(name)
@@ -205,9 +206,7 @@
 # print output as an HTML table
 print(wishlists().sort("unitprice desc")("Wishlists").as_html())
 
 # print output as a Markdown table
 print(wishlists().sort("unitprice desc")("Wishlists").as_markdown())
 
 ```
-
-
```

### Comparing `littletable-2.1.2/README.md` & `littletable-2.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -108,28 +108,31 @@
 Extended "getting started" notes at [how_to_use_littletable.md](https://github.com/ptmcg/littletable/blob/master/how_to_use_littletable.md).
 
 Sample Demo
 -----------
 Here is a simple littletable data storage/retrieval example:
 
 ```python
-from littletable import Table, DataObject
+from littletable import Table
 
 customers = Table('customers')
 customers.create_index("id", unique=True)
-customers.insert(DataObject(id="0010", name="George Jetson"))
-customers.insert(DataObject(id="0020", name="Wile E. Coyote"))
-customers.insert(DataObject(id="0030", name="Jonny Quest"))
+customers.csv_import("""\
+id,name
+0010,George Jetson
+0020,Wile E. Coyote
+0030,Jonny Quest
+""")
 
 catalog = Table('catalog')
 catalog.create_index("sku", unique=True)
-catalog.insert(DataObject(sku="ANVIL-001", descr="1000lb anvil", unitofmeas="EA",unitprice=100))
-catalog.insert(DataObject(sku="BRDSD-001", descr="Bird seed", unitofmeas="LB",unitprice=3))
-catalog.insert(DataObject(sku="MAGNT-001", descr="Magnet", unitofmeas="EA",unitprice=8))
-catalog.insert(DataObject(sku="MAGLS-001", descr="Magnifying glass", unitofmeas="EA",unitprice=12))
+catalog.insert({"sku": "ANVIL-001", "descr": "1000lb anvil", "unitofmeas": "EA","unitprice": 100})
+catalog.insert({"sku": "BRDSD-001", "descr": "Bird seed", "unitofmeas": "LB","unitprice": 3})
+catalog.insert({"sku": "MAGNT-001", "descr": "Magnet", "unitofmeas": "EA","unitprice": 8})
+catalog.insert({"sku": "MAGLS-001", "descr": "Magnifying glass", "unitofmeas": "EA","unitprice": 12})
 
 wishitems = Table('wishitems')
 wishitems.create_index("custid")
 wishitems.create_index("sku")
 
 # easy to import CSV data from a string or file
 wishitems.csv_import("""\
@@ -137,15 +140,15 @@
 0020,ANVIL-001
 0020,BRDSD-001
 0020,MAGNT-001
 0030,MAGNT-001
 0030,MAGLS-001
 """)
 
-# print a particular customer name 
+# print a particular customer name
 # (unique indexes will return a single item; non-unique
 # indexes will return a list of all matching items)
 print(customers.by.id["0030"].name)
 
 # see all customer names
 for name in customers.all.name:
     print(name)
```

### Comparing `littletable-2.1.2/littletable.egg-info/PKG-INFO` & `littletable-2.2.0/littletable.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: littletable
-Version: 2.1.2
+Version: 2.2.0
 Summary: Python in-memory ORM database
 Home-page: https://github.com/ptmcg/littletable/
+Download-URL: https://pypi.org/project/littletable/
 Author: Paul McGuire
 Author-email: ptmcg@austin.rr.com
 License: MIT License
-Download-URL: https://pypi.org/project/littletable/
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # littletable - a Python module to give ORM-like access to a collection of objects
 [![Build Status](https://travis-ci.org/ptmcg/littletable.svg?branch=master)](https://travis-ci.org/ptmcg/littletable) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ptmcg/littletable/master)
 
 - [Introduction](#introduction)
@@ -137,28 +135,31 @@
 Extended "getting started" notes at [how_to_use_littletable.md](https://github.com/ptmcg/littletable/blob/master/how_to_use_littletable.md).
 
 Sample Demo
 -----------
 Here is a simple littletable data storage/retrieval example:
 
 ```python
-from littletable import Table, DataObject
+from littletable import Table
 
 customers = Table('customers')
 customers.create_index("id", unique=True)
-customers.insert(DataObject(id="0010", name="George Jetson"))
-customers.insert(DataObject(id="0020", name="Wile E. Coyote"))
-customers.insert(DataObject(id="0030", name="Jonny Quest"))
+customers.csv_import("""\
+id,name
+0010,George Jetson
+0020,Wile E. Coyote
+0030,Jonny Quest
+""")
 
 catalog = Table('catalog')
 catalog.create_index("sku", unique=True)
-catalog.insert(DataObject(sku="ANVIL-001", descr="1000lb anvil", unitofmeas="EA",unitprice=100))
-catalog.insert(DataObject(sku="BRDSD-001", descr="Bird seed", unitofmeas="LB",unitprice=3))
-catalog.insert(DataObject(sku="MAGNT-001", descr="Magnet", unitofmeas="EA",unitprice=8))
-catalog.insert(DataObject(sku="MAGLS-001", descr="Magnifying glass", unitofmeas="EA",unitprice=12))
+catalog.insert({"sku": "ANVIL-001", "descr": "1000lb anvil", "unitofmeas": "EA","unitprice": 100})
+catalog.insert({"sku": "BRDSD-001", "descr": "Bird seed", "unitofmeas": "LB","unitprice": 3})
+catalog.insert({"sku": "MAGNT-001", "descr": "Magnet", "unitofmeas": "EA","unitprice": 8})
+catalog.insert({"sku": "MAGLS-001", "descr": "Magnifying glass", "unitofmeas": "EA","unitprice": 12})
 
 wishitems = Table('wishitems')
 wishitems.create_index("custid")
 wishitems.create_index("sku")
 
 # easy to import CSV data from a string or file
 wishitems.csv_import("""\
@@ -166,15 +167,15 @@
 0020,ANVIL-001
 0020,BRDSD-001
 0020,MAGNT-001
 0030,MAGNT-001
 0030,MAGLS-001
 """)
 
-# print a particular customer name 
+# print a particular customer name
 # (unique indexes will return a single item; non-unique
 # indexes will return a list of all matching items)
 print(customers.by.id["0030"].name)
 
 # see all customer names
 for name in customers.all.name:
     print(name)
@@ -205,9 +206,7 @@
 # print output as an HTML table
 print(wishlists().sort("unitprice desc")("Wishlists").as_html())
 
 # print output as a Markdown table
 print(wishlists().sort("unitprice desc")("Wishlists").as_markdown())
 
 ```
-
-
```

### Comparing `littletable-2.1.2/littletable.py` & `littletable-2.2.0/littletable.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # littletable.py
 #
 # littletable is a simple in-memory database for ad-hoc or user-defined objects,
 # supporting simple query and join operations - useful for ORM-like access
 # to a collection of data objects, without dealing with SQL
 #
 #
-# Copyright (c) 2010-2022  Paul T. McGuire
+# Copyright (c) 2010-2023  Paul T. McGuire
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
@@ -29,42 +29,45 @@
 # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 __doc__ = r"""
 
 C{littletable} - a Python module to give ORM-like access to a collection of objects
 
 The C{littletable} module provides a low-overhead, schema-less, in-memory database access to a 
-collection of user objects.  C{littletable} provides a L{DataObject} class for ad hoc creation
-of semi-immutable objects that can be stored in a C{littletable} L{Table}. C{Table}s can also
+collection of user objects.  C{Table}s can
 contain user-defined objects, using those objects' C{__dict__}, C{__slots__}, or C{_fields}
 mappings to access object attributes. Table contents can thus also include namedtuples, 
 SimpleNamespaces, or dataclasses.
 
+C{Tables} can also be constructed using Python dicts. In this case, they are stored as 
+SimpleNamespaces.
+
 In addition to basic insert/remove/query/delete access to the contents of a 
 Table, C{littletable} offers:
- - simple indexing for improved retrieval performance, and optional enforcing key uniqueness
+ - indexing for improved retrieval performance, and optional enforcing key uniqueness
  - access to objects using indexed attributes
+ - full text search on attributes containing extended text content
  - simplified joins using '+' operator syntax between annotated Tables
  - the result of any query or join is a new first-class C{littletable} Table
  - pivot on one or two attributes to gather tabulated data summaries
  - easy import/export to CSV and JSON files
 
 C{littletable} Tables do not require an upfront schema definition, but simply work off of the
 attributes in the stored values, and those referenced in any query parameters.
 
 Here is a simple C{littletable} data storage/retrieval example::
 
-    from littletable import Table, DataObject
+    from littletable import Table
 
     # create table of customers
     customers = Table('customers')
     customers.create_index("id", unique=True)
-    customers.insert(DataObject(id="0010", name="George Jetson"))
-    customers.insert(DataObject(id="0020", name="Wile E. Coyote"))
-    customers.insert(DataObject(id="0030", name="Jonny Quest"))
+    customers.insert({id="0010", name="George Jetson"})
+    customers.insert({id="0020", name="Wile E. Coyote"})
+    customers.insert({id="0030", name="Jonny Quest"})
 
     # create table of product catalog (load from CSV data)
     catalog_data = '''\
     sku,descr,unitofmeas,unitprice
     BRDSD-001,Bird seed,LB,3
     BBS-001,Steel BB's,LB,5
     MAGNT-001,Magnet,EA,8
@@ -79,19 +82,19 @@
 
     print(catalog.by.sku["ANVIL-001"].descr)
 
     # create many-to-many link table of wishlist items
     wishitems = Table('wishitems')
     wishitems.create_index("custid")
     wishitems.create_index("sku")
-    wishitems.insert(DataObject(custid="0020", sku="ANVIL-001"))
-    wishitems.insert(DataObject(custid="0020", sku="BRDSD-001"))
-    wishitems.insert(DataObject(custid="0020", sku="MAGNT-001"))
-    wishitems.insert(DataObject(custid="0030", sku="MAGNT-001"))
-    wishitems.insert(DataObject(custid="0030", sku="MAGLS-001"))
+    wishitems.insert({custid="0020", sku="ANVIL-001"})
+    wishitems.insert({custid="0020", sku="BRDSD-001"})
+    wishitems.insert({custid="0020", sku="MAGNT-001"})
+    wishitems.insert({custid="0030", sku="MAGNT-001"})
+    wishitems.insert({custid="0030", sku="MAGLS-001"})
 
     # print a particular customer name 
     # (unique indexes will return a single item; non-unique
     # indexes will return a list of all matching items)
     print(customers.by.id["0030"].name)
 
     # print all items sold by the pound
@@ -137,40 +140,40 @@
 from contextlib import closing
 from functools import partial
 from itertools import repeat, takewhile, chain, product, tee, groupby
 from pathlib import Path
 from types import SimpleNamespace
 import urllib.request
 from typing import (
-    Tuple, List, Callable, Any, TextIO, Dict, Union, Optional, Iterable, Iterator, Set, Generic, TypeVar
+    Callable, Any, TextIO, Union, Optional, Iterable, Iterator, Generic, TypeVar
 )
 
 try:
     import rich
     from rich import box
 except ImportError:
     rich = None
     box = None
 
 version_info = namedtuple("version_info", "major minor micro release_level serial")
-__version_info__ = version_info(2, 1, 2, "final", 0)
+__version_info__ = version_info(2, 2, 0, "final", 0)
 __version__ = (
     "{}.{}.{}".format(*__version_info__[:3])
     + (f"{__version_info__.release_level[0]}{__version_info__.serial}", "")[
         __version_info__.release_level == "final"
     ]
 )
-__version_time__ = "23 Jan 2023 21:52 UTC"
+__version_time__ = "30 Apr 2023 06:40 UTC"
 __author__ = "Paul McGuire <ptmcg@austin.rr.com>"
 
 NL = os.linesep
 
 default_row_class = SimpleNamespace
 
-_numeric_type: Tuple = (int, float)
+_numeric_type: tuple = (int, float)
 right_justify_types = (int, float, datetime.timedelta)
 
 try:
     import numpy
 except ImportError:
     pass
 else:
@@ -179,15 +182,23 @@
 try:
     import openpyxl
 except ImportError:
     openpyxl = None
 
 PredicateFunction = Callable[[Any], bool]
 
-__all__ = ["DataObject", "Table", "FixedWidthReader"]
+__all__ = [
+    "__author__",
+    "__version__",
+    "__version_info__",
+    "__version_time__",
+    "DataObject",
+    "FixedWidthReader",
+    "Table",
+]
 
 # define default stopwords for full_text_search
 _stopwords = set(
     """\
 a about above after again against all am an and any are aren't as at be because been 
 before being below between both but by can't cannot could couldn't did didn't do does 
 doesn't doing don't down during each few for from further had hadn't has hasn't have 
@@ -197,14 +208,44 @@
 she'll she's should shouldn't so some such than that that's the their theirs them themselves 
 then there there's these they they'd they'll they're they've this those through to too under 
 until up very was wasn't we we'd we'll we're we've were weren't what what's when when's 
 where where's which while who who's whom why why's with won't would wouldn't you 
 you'd you'll you're you've your yours yourself yourselves""".split()
 )
 
+# irregular plurals and singulars for text search handling
+_common_english_irregular_plurals = {
+    'addenda': 'addendum', 'addendums': 'addendum', 'alumnae': 'alumna', 'alumni': 'alumnus', 'analyses': 'analysis',
+    'antennae': 'antenna', 'antennas': 'antenna', 'antitheses': 'antithesis',
+    'appendices': 'appendix', 'appendixes': 'appendix', 'bacilli': 'bacillus', 'bacteria': 'bacterium',
+    'cacti': 'cactus', 'calves': 'calf', 'children': 'child', 'corpora': 'corpus', 'crises': 'crisis',
+    'criteria': 'criterion', 'curricula': 'curriculum', 'diagnoses': 'diagnosis', 'dice': 'die',
+    'dwarves': 'dwarf', 'dwarfs': 'dwarf', 'elves': 'elf', 'ellipses': 'ellipsis', 'errata': 'erratum',
+    'firemen': 'fireman', 'foci': 'focus', 'feet': 'foot', 'formulae': 'formula', 'fungi': 'fungus', 'genera': 'genus',
+    'geese': 'goose', 'halves': 'half', 'hooves': 'hoof', 'hypotheses': 'hypothesis',
+    'indices': 'index', 'indexes': 'index', 'knives': 'knife', 'larvae': 'larva', 'leaves': 'leaf', 'lives': 'life',
+    'loaves': 'loaf', 'loci': 'locus', 'lice': 'louse', 'men': 'man', 'matrices': 'matrix', 'media': 'medium',
+    'memoranda': 'memorandum', 'minutiae': 'minutia', 'mice': 'mouse', 'nebulae': 'nebula', 'nuclei': 'nucleus',
+    'oases': 'oasis', 'opera': 'opus', 'ova': 'ovum', 'oxen': 'ox', 'parentheses': 'parenthesis',
+    'phenomena': 'phenomenon', 'phyla': 'phylum', 'quizzes': 'quiz', 'radii': 'radius', 'referenda': 'referendum',
+    'scarves': 'scarf', 'selves': 'self', 'shelves': 'shelf', 'staves': 'staff', 'stimuli': 'stimulus',
+    'strata': 'stratum', 'syllabi': 'syllabus', 'symposia': 'symposium', 'synopses': 'synopsis', 'tableaux': 'tableau',
+    'theses': 'thesis', 'thieves': 'thief', 'teeth': 'tooth', 'vertebrae': 'vertebra', 'vertices': 'vertex',
+    'vitae': 'vita', 'vortices': 'vortex', 'wharves': 'wharf', 'wives': 'wife', 'wolves': 'wolf', 'women': 'woman',
+}
+_singulars_that_look_like_plurals = [
+    'rabies', 'scabies', 'caries', 'aries', 'series', 'billiards', 'grits', 'pliers', 'whereabouts', 'jeans',
+    'binoculars', 'scissors', 'tidings', 'trousers', 'clothes', 'news', 'measles', 'mumps', 'calculus', 'molasses',
+    'tweezers', 'dominoes', 'pants', 'odds', 'riches', 'alms', 'barracks', 'chassis', 'corps', 'headquarters', 'ides',
+    'kudos', 'species'
+]
+_plurals_map = {
+    **_common_english_irregular_plurals,
+    **{s: s for s in _singulars_that_look_like_plurals}
+}
 
 class UnableToExtractAttributeNamesError(ValueError):
     """Exception raised when attributes cannot be determined from an object."""
 
 
 def _object_attrnames(obj):
     if hasattr(obj, "trait_names"):
@@ -257,14 +298,19 @@
     A generic semi-mutable object for storing data values in a table. Attributes
     can be set by passing in named arguments in the constructor, or by setting them
     as C{object.attribute = value}. New attributes can be added any time, but updates
     are ignored.  Table joins are returned as a Table of DataObjects.
     """
 
     def __init__(self, **kwargs):
+        warnings.warn(
+            "littletable.DataObject class is deprecated, use types.Simplenamespace or Python dict",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         if kwargs:
             self.__dict__.update(kwargs)
 
     def __repr__(self):
         return (
             "{"
             f"""{', '.join(f"{k!r}: {v!r}" for k, v in sorted(self.__dict__.items()))}"""
@@ -387,16 +433,15 @@
     def keys(self):
         return sorted(self.obs.keys()) + ([None, ] if self.none_values else [])
 
     def items(self):
         return ((k, [v]) for k, v in self.obs.items())
 
     def remove(self, obj):
-        k = getattr(obj, self.attr)
-        if k is not None:
+        if (k := getattr(obj, self.attr)) is not None:
             self.obs.pop(k, None)
         else:
             try:
                 self.none_values.remove(obj)
             except ValueError:
                 pass
 
@@ -698,17 +743,17 @@
 
     def close(self):
         if hasattr(self._iterobj, "close"):
             self._iterobj.close()
 
 
 FixedWidthParseSpec = Union[
-    Tuple[str, int],
-    Tuple[str, int, Optional[int]],
-    Tuple[str, int, Optional[int], Optional[Callable[[str], Any]]],
+    tuple[str, int],
+    tuple[str, int, Optional[int]],
+    tuple[str, int, Optional[int], Optional[Callable[[str], Any]]],
 ]
 
 
 class FixedWidthReader:
     """
     Helper class to read fixed-width data and yield a sequence of dicts
     representing each row of data.
@@ -726,21 +771,21 @@
           datetime, etc.; if omitted or None, str.strip() will be used
     - src_file: a string filename or a file-like object containing the
         fixed-width data to be loaded
     """
 
     def __init__(
         self,
-        slice_spec: List[FixedWidthParseSpec],
+        slice_spec: list[FixedWidthParseSpec],
         src_file: Union[str, Iterable, TextIO],
         encoding: str = "utf-8",
     ):
         def parse_spec(
-            spec: List[FixedWidthParseSpec],
-        ) -> List[Tuple[str, slice, Callable[[str], Any]]]:
+            spec: list[FixedWidthParseSpec],
+        ) -> list[tuple[str, slice, Callable[[str], Any]]]:
             ret = []
             for cur, next_ in zip(spec, spec[1:] + [("", sys.maxsize, None, None)]):
                 label, col, endcol, fn = (cur + (None, None,))[:4]
                 if label is None:
                     continue
                 if endcol is None:
                     endcol = next_[1]
@@ -866,15 +911,15 @@
 
 
 TableContent = TypeVar("TableContent")
 
 
 class Table(Generic[TableContent]):
     """
-    Table is the main class in C{littletable}, for representing a collection of DataObjects or
+    Table is the main class in C{littletable}, for representing a collection of SimpleNamespaces or
     user-defined objects with publicly accessible attributes or properties.  Tables can be:
      - created, with an optional name, using standard Python L{C{Table() constructor}<__init__>}
      - indexed, with multiple indexes, with unique or non-unique values, see L{create_index}
      - queried, specifying values to exact match in the desired records, see L{where}
      - filtered (using L{where}), using a simple predicate function to match desired records;
        useful for selecting using inequalities or compound conditions
      - accessed directly for keyed values, using C{table.indexattribute[key]} - see L{__getattr__}
@@ -1043,18 +1088,18 @@
     def __init__(self, table_name: str = ""):
         """
         Create a new, empty Table.
         @param table_name: name for Table
         @type table_name: string (optional)
         """
         self(table_name)
-        self.obs: List = []
-        self._indexes: Dict[str, _ObjIndex] = {}
-        self._uniqueIndexes: List[_UniqueObjIndex] = []
-        self._search_indexes: Dict[str, Dict[str, List]] = {}
+        self.obs: list = []
+        self._indexes: dict[str, _ObjIndex] = {}
+        self._uniqueIndexes: list[_UniqueObjIndex] = []
+        self._search_indexes: dict[str, dict[str, list]] = {}
 
         self.import_source_type: Optional[ImportSourceType] = None
         self.import_source: Optional[str] = None
 
         """
         C{'by'} is added as a pseudo-attribute on tables, to provide
         dict-like access to the underlying records in the table by index key, as in::
@@ -1208,15 +1253,15 @@
         @param table_name: name for Table
         @type table_name: string
         """
         if table_name is not None:
             self.table_name = table_name
         return self
 
-    def _attr_names(self) -> List[str]:
+    def _attr_names(self) -> list[str]:
         return list(
             _object_attrnames(self.obs[0]) if self.obs else self._indexes.keys()
         )
 
     def copy_template(self, name: str = None) -> "Table":
         """
         Create empty copy of the current table, with copies of all
@@ -1310,32 +1355,96 @@
                 ind for ind in self._indexes.values() if ind.is_unique
             ]
         return self
 
     def get_index(self, attr: str):
         return _ReadonlyObjIndexWrapper(self._indexes[attr], self.copy_template())
 
+    NON_WORD_STRIPPER_RE = re.compile(r"[^\w_]?([\w._-]*)[^\w.]*")
+    NON_WORD_STRIPPER2_RE = re.compile(r"[^\w_-]?((?:\w|[-_]\w)+)(!>_-)$")
+    PLURAL_ENDING_IN_IES = re.compile(r"(.*[^aeiouy])ies$")
+    PLURAL_ENDING_IN_ES = re.compile(r"(.*(?:ch|ss|sh|x))es$")
+    PLURAL_ENDING_IN_S = re.compile(r"(.*[^aeious])s$")
+    SINGULAR_ENDING_IN_S = re.compile(r"(.*(?:ness|ics))$")
+    ACRONYM_WITH_PERIODS = re.compile(r"((?:\w\.){2,})(!>\.)$")
+
     @staticmethod
     def _normalize_word(s: str) -> str:
         match_res = [
             # an acronym of 2 or more "X." sequences, such as G.E. or I.B.M.
             re.compile(r"((?:\w\.){2,})"),
             # words that may be hyphenated or snake-case
             # (strip off any leading single non-word character)
             re.compile(r"[^\w_-]?((?:\w|[-_]\w)+)"),
         ]
         for match_re in match_res:
-            match = match_re.match(s)
-            if match:
+            if match := match_re.match(s):
                 ret = match.group(1).lower().replace(".", "")
                 return ret
         return ""
 
-    def _normalize_split(self, s: str) -> Iterable[str]:
-        return filter(None, (self._normalize_word(wd) for wd in s.split()))
+    @staticmethod
+    def _normalize_word_gen(s: str) -> Iterable[str]:
+        # strip non-word chars from front and back
+        stripper = Table.NON_WORD_STRIPPER_RE
+        s = stripper.match(s).group(1)
+
+        # catch plurals
+        if s.isalpha():
+            s = s.lower()
+
+            # check common plurals - if not found, check common plural patterns
+            if not (sing := _plurals_map.get(s)):
+
+                match_subs = (
+                    (Table.PLURAL_ENDING_IN_IES, r"\1y"),
+                    (Table.PLURAL_ENDING_IN_ES, r"\1"),
+                    (Table.SINGULAR_ENDING_IN_S, r"\1"),
+                    (Table.PLURAL_ENDING_IN_S, r"\1"),
+                )
+                sing = next((sub_match[0] for re_sub, re_repl in match_subs
+                            if (sub_match := re_sub.subn(re_repl, s))[1]),
+                            s)
+
+            if sing and sing != s:
+                yield sing
+            yield s
+            return
+
+        match_res = [
+            # an acronym of 2 or more "X." sequences, such as G.E. or I.B.M.
+            Table.ACRONYM_WITH_PERIODS,
+            # words that may be hyphenated or snake-case
+            # (strip off any leading single non-word character)
+            Table.NON_WORD_STRIPPER2_RE,
+        ]
+        for match_re in match_res:
+            if match := match_re.match(s):
+                g1 = match.group(1).lower()
+                yield g1.replace(".", "")
+                for sep in "-":
+                    if sep in g1:
+                        yield from filter(None, g1.split(sep))
+                break
+        else:
+            for sep in ".-":
+                if sep in s:
+                    yield from (
+                        ss.lower() for ss in s.split(sep)
+                        if (ss.islower() or len(ss) > 1)
+                    )
+                    if sep == "." and all(len(ss) <= 1 for ss in s.split(".")):
+                        yield s.lower().replace(".", "")
+            yield s.lower()
+
+    @staticmethod
+    def _normalize_split(s: str) -> Iterable[str]:
+        return (
+            filter(None, (ss for wd in s.split() for ss in Table._normalize_word_gen(wd)))
+        )
 
     def create_search_index(
         self,
         attrname: str,
         stopwords: Optional[Iterable[str]] = None,
         force: bool = False,
     ) -> "Table":
@@ -1375,121 +1484,142 @@
         if attrname in self._search_indexes:
             if force or not self._search_indexes[attrname]["VALID"]:
                 # stale search index, rebuild
                 self._search_indexes.pop(attrname)
             else:
                 return self
 
-        stopwords_set: Set[str]
+        stopwords_set: set[str]
         if stopwords is None:
             stopwords_set = _stopwords
         else:
             stopwords_set = set(stopwords)
 
         self._search_indexes[attrname] = defaultdict(list)
-        new_index: Dict[str, Any] = self._search_indexes[attrname]
+        new_index: dict[str, Any] = self._search_indexes[attrname]
         for i, rec in enumerate(self.obs):
-            words = self._normalize_split(getattr(rec, attrname, ""))
+            if not (attrvalue := getattr(rec, attrname, "")):
+                continue
+            words = self._normalize_split(attrvalue)
             for wd in set(words) - stopwords_set:
                 new_index[wd].append(i)
 
         # use uppercase keys for index metadata, since they should not
         # overlap with any search terms
         new_index["STOPWORDS"] = stopwords_set
         new_index["VALID"] = True
 
         return self
 
     def _search(
-        self, attrname, query, limit=int(1e9), min_score=0, include_words=False, as_table=False
+        self, attrname, query, limit=int(1e9), min_score=0, include_words=False, as_table=True
     ):
         if attrname not in self._search_indexes:
             raise ValueError(f"no search index defined for attribute {attrname!r}")
 
         search_index = self._search_indexes[attrname]
         if not search_index["VALID"]:
             msg = (
                 f"table has been modified since the search index for {attrname!r} was created,"
                 " rebuild using create_search_index()"
             )
             raise SearchIndexInconsistentError(msg)
         stopwords = search_index["STOPWORDS"]
 
-        plus_matches = {}
-        minus_matches = {}
-        opt_matches = {}
-        reqd_matches = set()
-        excl_matches = set()
+        plus_matches: dict[str, set[int]] = {}
+        minus_matches: dict[str, list[int]] = {}
+        opt_matches: dict[str, list[int]] = {}
+        reqd_matches: set[int] = set()
+        excl_matches: set[int] = set()
+        reqd_words: dict[tuple[str], dict[str, set[int]]] = {}
 
         if isinstance(query, str):
             query = shlex.split(query.strip())
 
         for keyword in query:
             keyword = keyword.lower()
             if keyword.startswith("++"):
-                kwd = self._normalize_word(keyword[2:])
-                if kwd in stopwords:
-                    continue
-
-                if kwd not in plus_matches:
-                    plus_matches[kwd] = set(search_index.get(kwd, []))
+                kwds = tuple(self._normalize_word_gen(keyword[2:]))
+                reqd_words[kwds] = {}
+                for kwd in kwds:
+                    # kwd = self._normalize_word(keyword[2:])
+                    if kwd in stopwords:
+                        continue
+
+                    matched_entries = set(search_index.get(kwd, []))
+                    reqd_words[kwds][kwd] = matched_entries
+                    if not matched_entries:
+                        continue
 
-                if kwd in search_index:
-                    if reqd_matches:
-                        reqd_matches &= set(search_index.get(kwd, []))
-                    else:
-                        reqd_matches = set(search_index.get(kwd, []))
-                else:
-                    # required keyword is not present at all - define unmatchable required match and break
-                    reqd_matches = {-1}
-                    break
+                    if kwd not in plus_matches:
+                        plus_matches[kwd] = matched_entries
 
             elif keyword.startswith("--"):
-                kwd = self._normalize_word(keyword[2:])
-                if kwd in stopwords:
-                    continue
-                excl_matches |= set(search_index.get(kwd, []))
+                # kwd = self._normalize_word(keyword[2:])
+                for kwd in self._normalize_word_gen(keyword[2:]):
+                    if kwd in stopwords:
+                        continue
+                    excl_matches |= set(search_index.get(kwd, []))
 
             elif keyword.startswith("+"):
-                kwd = self._normalize_word(keyword[1:])
-                if kwd in stopwords:
-                    continue
-                minus_matches.pop(kwd, None)
-                if kwd not in plus_matches and kwd not in reqd_matches:
-                    plus_matches[kwd] = set(search_index.get(kwd, []))
+                # kwd = self._normalize_word(keyword[1:])
+                for kwd in self._normalize_word_gen(keyword[1:]):
+                    if kwd in stopwords:
+                        continue
+                    minus_matches.pop(kwd, None)
+                    if kwd not in plus_matches and kwd not in reqd_matches:
+                        plus_matches[kwd] = set(search_index.get(kwd, []))
 
             elif keyword.startswith("-"):
-                kwd = self._normalize_word(keyword[1:])
-                if kwd in stopwords:
-                    continue
-                plus_matches.pop(kwd, None)
-                if kwd not in minus_matches and kwd not in excl_matches:
-                    minus_matches[kwd] = set(search_index.get(kwd, []))
+                # kwd = self._normalize_word(keyword[1:])
+                for kwd in self._normalize_word_gen(keyword[1:]):
+                    if kwd in stopwords:
+                        continue
+                    plus_matches.pop(kwd, None)
+                    if kwd not in minus_matches and kwd not in excl_matches:
+                        minus_matches[kwd] = set(search_index.get(kwd, []))
 
             else:
-                kwd = self._normalize_word(keyword)
-                if kwd in stopwords:
-                    continue
-                if kwd in plus_matches or kwd in minus_matches:
-                    continue
-                opt_matches[kwd] = set(search_index.get(kwd, []))
+                # kwd = self._normalize_word(keyword)
+                for kwd in self._normalize_word_gen(keyword):
+                    if kwd in stopwords:
+                        continue
+                    if kwd in plus_matches or kwd in minus_matches:
+                        continue
+                    opt_matches[kwd] = set(search_index.get(kwd, []))
+
+        # process word groups to determine correct set of reqd_matches
+        if reqd_words:
+            reqd_matches = set(range(len(self.obs)))
+            for reqd_word_tuple, word_matches_tuples in reqd_words.items():
+                group_matches = set()
+                for _, submatch in word_matches_tuples.items():
+                    group_matches |= submatch
+                if not group_matches:
+                    # no possible match, force an impossible match set
+                    reqd_matches = {-1,}
+                    break
+                else:
+                    reqd_matches &= group_matches
 
+        # walk through plus, minus, and optional matches to build matching scores
         tally = Counter()
         for match_type, score in (
             (plus_matches, 1000),
             (minus_matches, -1000),
             (opt_matches, 100),
         ):
             for obj_set in match_type.values():
                 if reqd_matches:
                     obj_set &= reqd_matches
                 obj_set -= excl_matches
                 for obj in obj_set:
                     tally[obj] += score
 
+        # compose return structure, depending on whether the actual matched words in each entry should be included
         if include_words:
             ret = [
                 (self[rec_idx], score,
                  sorted({}.fromkeys(self._normalize_split(getattr(self[rec_idx], attrname, ""))).keys() - stopwords))
                 for rec_idx, score in tally.most_common(limit)
                 if score > min_score]
         else:
@@ -1498,14 +1628,15 @@
                 for rec_idx, score in tally.most_common(limit)
                 if score > min_score
             ]
 
         if as_table:
             tuple_ret = ret
             ret = self.copy_template()
+            ret.table_name = " ".join(query)
             ret.insert_many(copy.copy(rec[0]) for rec in tuple_ret)
             score_attr = f"{attrname}_search_score"
             words_attr = f"{attrname}_search_words"
             try:
                 for rec, tup in zip(ret, tuple_ret):
                     setattr(rec, score_attr, tup[1])
                     if len(tup) > 2:
@@ -1522,19 +1653,22 @@
         """
         self._search_indexes.pop(attrname, None)
 
     def insert(self, obj: Any) -> "Table":
         """
         Insert a new object into this Table.
         @param obj: any Python object -
-        Objects can be constructed using the defined DataObject type, or they can
-        be any Python object that does not use the Python C{__slots__} feature; C{littletable}
-        introspects the object's C{__dict__} or C{_fields} attributes to obtain join and
+        Objects can be constructed using any Python object; C{littletable}
+        introspects the object's C{__dict__}, C{__slots__}, or C{_fields} attributes
+        (or keys() result if pass a Python dict) to obtain join and
         index attributes and values.
 
+        If a table is constructed using Python dicts, they are stored as
+        C{types.SimpleNamespaces}, to support C{object.attribute} style access.
+
         If the table contains a unique index, and the record to be inserted would add
         a duplicate value for the indexed attribute, then C{KeyError} is raised, and the
         object is not inserted.
 
         If the table has no unique indexes, then it is possible to insert duplicate
         objects into the table.
         """
@@ -1656,15 +1790,15 @@
     def _contents_changed(self):
         """
         Internal method to be called whenever the contents of a table are modified.
         """
         for idx in self._search_indexes.values():
             idx["VALID"] = False
 
-    def _query_attr_sort_fn(self, attr_val: Tuple[str, Any]) -> int:
+    def _query_attr_sort_fn(self, attr_val: tuple[str, Any]) -> int:
         """Used to order where keys by most selective key first"""
         attr, v = attr_val
         if attr in self._indexes:
             idx = self._indexes[attr]
             if v in idx:
                 return len(idx[v])
             else:
@@ -1693,15 +1827,15 @@
         @return: a new Table containing the matching objects
         """
         if kwargs:
             # order query criteria in ascending order of number of matching items
             # for each individual given attribute; this will minimize the number
             # of filtering records that each subsequent attribute will have to
             # handle
-            kwargs_list: List[Tuple[str, Any]] = list(kwargs.items())
+            kwargs_list: list[tuple[str, Any]] = list(kwargs.items())
             if len(kwargs_list) > 1 and len(self) > 100:
                 kwargs_list.sort(key=self._query_attr_sort_fn)
 
             ret = self
             NO_SUCH_ATTR = object()
             for k, v in kwargs_list:
                 if callable(v):
@@ -1777,15 +1911,15 @@
            or field names with ' desc' appended; if it is a function, then it is the
            function to be used as the sort key function
         @param reverse: (default=False) set to True if results should be in reverse order
         @type reverse: bool
         @return: self
         """
         if isinstance(key, (str, list, tuple)):
-            attr_orders: List[List[str]]
+            attr_orders: list[list[str]]
             if isinstance(key, str):
                 attrdefs = [s.strip() for s in key.split(",")]
                 attr_orders = [(a.split() + ["asc", ])[:2] for a in attrdefs]
             else:
                 # attr definitions were already resolved to a sequence by the caller
                 if isinstance(key[0], str):
                     attr_orders = [(a.split() + ["asc", ])[:2] for a in key]
@@ -1931,15 +2065,15 @@
             (list may contain both strings and tuples)
         @param kwargs: attributes to join on, given as additional named arguments
             of the form C{table1attr="table2attr"}, or a dict mapping attribute names.
         @type auto_create_indexes: bool
         @param auto_create_indexes: flag to simplify joining tables, to automatically
             create necessary indexes instead of raising ValueError if a join field
             is not yet indexed (default=True)
-        @returns: a new Table containing the joined data as new DataObjects
+        @returns: a new Table containing the joined data as new SimpleNamespaces
         """
         if not kwargs:
             raise TypeError(
                 "must specify at least one join attribute as a named argument"
             )
         this_cols, other_cols = list(kwargs.keys()), list(kwargs.values())
 
@@ -1959,15 +2093,15 @@
             return Table(retname)
 
         attr_spec_list = attrlist
         if isinstance(attrlist, str):
             attr_spec_list = re.split(r"[,\s]+", attrlist)
 
         # expand attrlist to full (table, name, alias) tuples
-        full_attr_specs: List[Tuple[Table, str, str]]
+        full_attr_specs: list[tuple[Table, str, str]]
         if attr_spec_list is None:
             full_attr_specs = [(self, namestr, namestr) for namestr in self._attr_names()]
             full_attr_specs += [(other, namestr, namestr) for namestr in other._attr_names()]
         else:
             full_attr_specs = []
             this_attr_names = set(self._attr_names())
             other_attr_names = set(other._attr_names())
@@ -1998,15 +2132,15 @@
         if auto_create_indexes:
             for tbl, col_list in ((self, this_cols), (other, other_cols)):
                 for col in col_list:
                     if col not in tbl._indexes:
                         tbl.create_index(col)
         else:
             # make sure all join columns are indexed
-            unindexed_cols: List[str] = []
+            unindexed_cols: list[str] = []
             for tbl, col_list in ((self, this_cols), (other, other_cols)):
                 unindexed_cols.extend(
                     col for col in col_list if col not in tbl._indexes
                 )
             if unindexed_cols:
                 raise ValueError(
                     f"indexed attributes required for join: {','.join(unindexed_cols)}"
@@ -2086,15 +2220,15 @@
         @param attrlist: list of attributes to be copied to the new joined table; if
             none provided, all attributes of both tables will be used (taken from the first
             object in each table)
         @type attrlist: string, or list of strings or C{(table,attribute[,alias])} tuples
             (list may contain both strings and tuples)
         @param kwargs: attributes to join on, given as additional named arguments
             of the form C{table1attr="table2attr"}, or a dict mapping attribute names.
-        @returns: a new Table containing the joined data as new DataObjects
+        @returns: a new Table containing the joined data as new SimpleNamespaces
         """
         if join_type not in Table.OUTER_JOIN_TYPES:
             join_names = [
                 nm
                 for nm, join_var in vars(Table).items()
                 if join_var in Table.OUTER_JOIN_TYPES
             ]
@@ -2123,15 +2257,15 @@
             return self.clone()(retname)
 
         attr_spec_list = attrlist
         if isinstance(attrlist, str):
             attr_spec_list = re.split(r"[,\s]+", attrlist)
 
         # expand attrlist to full (table, name, alias) tuples
-        full_attr_specs: List[Tuple[Table, str, str]]
+        full_attr_specs: list[tuple[Table, str, str]]
         if attr_spec_list is None:
             full_attr_specs = [(self, namestr, namestr) for namestr in self._attr_names()]
             full_attr_specs += [(other, namestr, namestr) for namestr in other._attr_names()]
         else:
             full_attr_specs = []
             this_attr_names = set(self._attr_names())
             other_attr_names = set(other._attr_names())
@@ -2162,15 +2296,15 @@
         if auto_create_indexes:
             for tbl, col_list in ((self, this_cols), (other, other_cols)):
                 for col in col_list:
                     if col not in tbl._indexes:
                         tbl.create_index(col)
         else:
             # make sure all join columns are indexed
-            unindexed_cols: List[str] = []
+            unindexed_cols: list[str] = []
             for tbl, col_list in ((self, this_cols), (other, other_cols)):
                 unindexed_cols.extend(
                     col for col in col_list if col not in tbl._indexes
                 )
             if unindexed_cols:
                 raise ValueError(
                     f"indexed attributes required for join: {','.join(unindexed_cols)}"
@@ -2382,16 +2516,16 @@
 
         return self
 
     def csv_import(
         self,
         csv_source: _ImportExportDataContainer,
         encoding: str = "utf-8",
-        transforms: Dict = None,
-        filters: Dict = None,
+        transforms: dict = None,
+        filters: dict = None,
         row_class: type = None,
         limit: int = None,
         fieldnames: Union[Iterable[str], str] = None,
         **kwargs,
     ) -> "Table":
         """
         Imports the contents of a CSV-formatted file into this table.
@@ -2411,15 +2545,15 @@
         @type transforms: dict (optional)
         @param filters: dict of functions by attribute name; if given, each
             newly-read record will be filtered before being added to the table, with each
             filter function run using the corresponding attribute; if any filter function
             returns False, the record is not added to the table. Useful when reading large
             input files, to pre-screen only for data matching one or more filters
         @type filters: dict (optional)
-        @param row_class: class to construct for each imported row when populating table (default=DataObject)
+        @param row_class: class to construct for each imported row when populating table (default=SimpleNamespace)
         @type row_class: type
         @param limit: number of records to import
         @type limit: int (optional)
         @param kwargs: additional constructor arguments for csv C{DictReader} objects, such as C{delimiter}
             or C{fieldnames}; these are passed directly through to the csv C{DictReader} constructor
         @type kwargs: named arguments (optional)
         @param fieldnames: names for imported columns; used if there is no header line in the input file
@@ -2440,16 +2574,16 @@
             limit=limit,
         )
 
     def _xsv_import(
         self,
         xsv_source: _ImportExportDataContainer,
         encoding: str = "utf-8",
-        transforms: Dict = None,
-        filters: Dict = None,
+        transforms: dict = None,
+        filters: dict = None,
         row_class: type = None,
         limit: int = None,
         **kwargs,
     ):
         non_reader_args = "encoding xsv_source transforms row_class limit filters".split()
         reader_args = {
             k: v for k, v in kwargs.items() if k not in non_reader_args
@@ -2464,16 +2598,16 @@
             limit=limit,
         )
 
     def tsv_import(
         self,
         xsv_source: _ImportExportDataContainer,
         encoding: str = "utf-8",
-        transforms: Dict = None,
-        filters: Dict = None,
+        transforms: dict = None,
+        filters: dict = None,
         row_class: type = None,
         limit: int = None,
         fieldnames: Union[Iterable[str], str] = None,
         **kwargs,
     ) -> "Table":
         """
         Imports the contents of a tab-separated data file into this table.
@@ -2484,15 +2618,15 @@
         @param transforms: dict of functions by attribute name; if given, each
             attribute will be transformed using the corresponding transform; if there is no
             matching transform, the attribute will be read as a string (default); the
             transform function can also be defined as a (function, default-value) tuple; if
             there is an Exception raised by the transform function, then the attribute will
             be set to the given default value
         @type transforms: dict (optional)
-        @param row_class: class to construct for each imported row when populating table (default=DataObject)
+        @param row_class: class to construct for each imported row when populating table (default=SimpleNamespace)
         @type row_class: type
         @param limit: number of records to import
         @type limit: int (optional)
         @param fieldnames: names for imported columns; used if there is no header line in the input file
         @type fieldnames: list[str] or str
         """
         kwargs["fieldnames"] = fieldnames.split() if isinstance(fieldnames, str) else fieldnames
@@ -2506,24 +2640,24 @@
             delimiter="\t",
             **kwargs,
         )
 
     def _excel_import(
         self,
         excel_source: _ImportExportDataContainer,
-        transforms: Dict = None,
-        filters: Dict = None,
+        transforms: dict = None,
+        filters: dict = None,
         row_class: type = None,
         limit: int = None,
         **kwargs,
     ):
         if openpyxl is None:
             raise Exception("openpyxl module not installed")
 
-        def excel_as_dict(filename, **reader_args) -> Iterable[Dict[str, str]]:
+        def excel_as_dict(filename, **reader_args) -> Iterable[dict[str, str]]:
             with closing(openpyxl.load_workbook(filename, read_only=True)) as wb:
                 # read requested sheet if provided on kwargs, otherwise read active sheet
                 requested_sheet = reader_args.get("sheet")
                 ws = wb[requested_sheet] if requested_sheet else wb.active
 
                 rows_iter = iter(ws.rows)
 
@@ -2542,16 +2676,16 @@
             row_class=row_class,
             limit=limit,
         )
 
     def excel_import(
         self,
         excel_source: _ImportExportDataContainer,
-        transforms: Dict = None,
-        filters: Dict = None,
+        transforms: dict = None,
+        filters: dict = None,
         row_class: type = None,
         limit: int = None,
         fieldnames: Union[Iterable[str], str] = None,
         **kwargs,
     ) -> "Table":
         """
         Imports the contents of a Excel file into this table.
@@ -2568,15 +2702,15 @@
         @type transforms: dict (optional)
         @param filters: dict of functions by attribute name; if given, each
             newly-read record will be filtered before being added to the table, with each
             filter function run using the corresponding attribute; if any filter function
             returns False, the record is not added to the table. Useful when reading large
             input files, to pre-screen only for data matching one or more filters
         @type filters: dict (optional)
-        @param row_class: class to construct for each imported row when populating table (default=DataObject)
+        @param row_class: class to construct for each imported row when populating table (default=SimpleNamespace)
         @type row_class: type
         @param limit: number of records to import
         @type limit: int (optional)
         @param kwargs: additional arguments for the excel reader. Only available argument is "sheet" to select which
             sheet to read (defaults to active sheet)
         @type kwargs: named arguments (optional)
         @param fieldnames: names for imported columns; used if there is no header line in the input file
@@ -2677,15 +2811,15 @@
             tsv_dest, fieldnames=fieldnames, encoding=encoding, delimiter="\t", **kwargs
         )
 
     def json_import(
         self,
         source: _ImportExportDataContainer,
         encoding: str = "UTF-8",
-        transforms: Dict = None,
+        transforms: dict = None,
         row_class: type = None,
         streaming: bool = False,
         path: str = "",
         json_decoder: json.JSONDecoder = None,
     ) -> "Table":
         """
         Imports the contents of a JSON data file into this table.
@@ -2696,15 +2830,15 @@
         @param transforms: dict of functions by attribute name; if given, each
             attribute will be transformed using the corresponding transform; if there is no
             matching transform, the attribute will be read as a string (default); the
             transform function can also be defined as a (function, default-value) tuple; if
             there is an Exception raised by the transform function, then the attribute will
             be set to the given default value
         @type transforms: dict (optional)
-        @param row_class: class to construct for each imported row when populating table (default=DataObject)
+        @param row_class: class to construct for each imported row when populating table (default=SimpleNamespace)
         @type row_class: type
         @param streaming: boolean flag to indicate whether inbound JSON will be a stream of multiple objects
             or a single list object (default=False)
         @type streaming: bool
         @param path: (only valid if streaming=False) a '.'-delimited path into the inbound JSON, in case
             the objects to import are not in a top-level JSON list
         @type path: str
@@ -2964,15 +3098,15 @@
         for key, recs in sorted(grouped_obs.items()):
             group_obj = default_row_class(**dict(zip(keyattrs, key)))
             for subkey, expr in outexprs.items():
                 setattr(group_obj, subkey, expr(recs))
             tbl.insert(group_obj)
         return tbl
 
-    def splitby(self, pred: Union[str, PredicateFunction]) -> Tuple["Table", "Table"]:
+    def splitby(self, pred: Union[str, PredicateFunction]) -> tuple["Table", "Table"]:
         """
         Takes a predicate function (takes a table record and returns True or False)
         and returns two tables: a table with all the rows that returned False and
         a table with all the rows that returned True. Will also accept a string
         indicating a particular field name, and uses `bool(getattr(rec, field_name))`
         for the predicate function.
 
@@ -3016,15 +3150,15 @@
             else:
                 reckey = key(ob)
             if reckey not in seen:
                 seen.add(reckey)
                 ret.insert(ob)
         return ret
 
-    def info(self) -> Dict:
+    def info(self) -> dict:
         """
         Quick method to list informative table statistics
         :return: dict listing table information and statistics
         """
         unique_indexes = set(self._uniqueIndexes)
         return {
             "len": len(self),
@@ -3122,15 +3256,15 @@
             ret.create_index("stat", unique=True)
             ret.insert_many(default_row_class(stat=stat_name,
                                               **{fname: stat_fn(accum[fname])
                                                  for fname in field_names})
                             for stat_name, stat_fn in stat_fn_map)
         return ret
 
-    def _parse_fields_string(self, field_names: Union[str, Iterable[str]]) -> List[str]:
+    def _parse_fields_string(self, field_names: Union[str, Iterable[str]]) -> list[str]:
         """
         Convert raw string or list of names to actual column names:
         - names starting with '-' indicate to suppress that field
         - '*' means include all other field names
         - if no fields are specifically included, then all fields are used
         :param field_names: str or list
         :return: expanded list of field names
@@ -3271,16 +3405,16 @@
         table_kwargs = {"header_style": "bold yellow"}
         table_kwargs.update(kwargs)
         table = self._rich_table(fields, empty="", groupby=groupby, **table_kwargs)
         print()
         console.print(table)
 
     def as_html(
-        self, fields: Union[str, Iterable[str]] = "*", formats: Dict = None, groupby=None,
-            table_properties: Dict = None,
+        self, fields: Union[str, Iterable[str]] = "*", formats: dict = None, groupby=None,
+            table_properties: dict = None,
     ) -> str:
         """
         Output the table as a rudimentary HTML table.
         @param fields: fields in the table to be shown in the table
                        - listing '*' as a field will add all unnamed fields
                        - starting a field name with '-' will suppress that name
         @type fields: list of strings or a single space-delimited string
@@ -3356,15 +3490,15 @@
                 "</thead>\n<tbody>"
                 f"{''.join(rows)}"
                 "</tbody>\n</table>"
             )
         return ret
 
     def as_markdown(
-        self, fields: Union[str, Iterable[str]] = "*", formats: Dict = None, groupby=None,
+        self, fields: Union[str, Iterable[str]] = "*", formats: dict = None, groupby=None,
     ) -> str:
         """
         Output the table as a Markdown table.
         @param fields: fields in the table to be shown in the table
                        - listing '*' as a field will add all unnamed fields
                        - starting a field name with '-' will suppress that name
         @type fields: list of strings or a single space-delimited string
```

### Comparing `littletable-2.1.2/setup.py` & `littletable-2.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,26 +18,25 @@
     long_description_content_type='text/markdown',
     author="Paul McGuire",
     author_email="ptmcg@austin.rr.com",
     license="MIT License",
     url="https://github.com/ptmcg/littletable/",
     download_url="https://pypi.org/project/littletable/",
     py_modules=modules,
-    python_requires=">=3.7",
+    python_requires=">=3.9",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Database',
         ]
     )
```

### Comparing `littletable-2.1.2/unit_tests.py` & `littletable-2.2.0/unit_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -5970,465 +5970,649 @@
 00017510: 6f6e 202d 2d61 6e63 686f 7669 6573 222c  on --anchovies",
 00017520: 205b 392c 2035 2c20 362c 2038 2c20 3130   [9, 5, 6, 8, 10
 00017530: 2c20 3133 5d29 2c0a 2020 2020 2020 2020  , 13]),.        
 00017540: 5d3a 0a20 2020 2020 2020 2020 2020 206d  ]:.            m
 00017550: 6174 6368 6573 203d 2073 656c 662e 7265  atches = self.re
 00017560: 6369 7065 732e 7365 6172 6368 2e69 6e67  cipes.search.ing
 00017570: 7265 6469 656e 7473 2871 7565 7279 2c20  redients(query, 
-00017580: 6d69 6e5f 7363 6f72 653d 2d31 3030 3030  min_score=-10000
-00017590: 290a 2020 2020 2020 2020 2020 2020 6d61  ).            ma
-000175a0: 7463 685f 6964 7320 3d20 5b72 6563 6970  tch_ids = [recip
-000175b0: 652e 6964 2066 6f72 2072 6563 6970 652c  e.id for recipe,
-000175c0: 205f 2069 6e20 6d61 7463 6865 735d 0a20   _ in matches]. 
-000175d0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-000175e0: 2872 6570 7228 7175 6572 7929 2c20 272d  (repr(query), '-
-000175f0: 3e27 2c20 5b28 7265 6369 7065 2e69 642c  >', [(recipe.id,
-00017600: 2073 636f 7265 2920 666f 7220 7265 6369   score) for reci
-00017610: 7065 2c20 7363 6f72 6520 696e 206d 6174  pe, score in mat
-00017620: 6368 6573 5d29 0a20 2020 2020 2020 2020  ches]).         
-00017630: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-00017640: 5465 7374 2871 7565 7279 3d71 7565 7279  Test(query=query
-00017650: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00017660: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00017670: 7561 6c28 6578 7065 6374 6564 2c20 6d61  ual(expected, ma
-00017680: 7463 685f 6964 732c 0a20 2020 2020 2020  tch_ids,.       
-00017690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176a0: 2020 2020 2020 2020 2020 6622 696e 7661            f"inva
-000176b0: 6c69 6420 7265 7375 6c74 7320 666f 7220  lid results for 
-000176c0: 7175 6572 7920 7b71 7565 7279 2172 7d2c  query {query!r},
-000176d0: 2065 7870 6563 7465 6420 7b65 7870 6563   expected {expec
-000176e0: 7465 647d 2c20 676f 7420 7b6d 6174 6368  ted}, got {match
-000176f0: 5f69 6473 7d22 290a 0a20 2020 2040 616e  _ids}")..    @an
-00017700: 6e6f 756e 6365 5f74 6573 740a 2020 2020  nounce_test.    
-00017710: 6465 6620 7465 7374 5f69 6e76 616c 6964  def test_invalid
-00017720: 6174 655f 696e 6465 7828 7365 6c66 293a  ate_index(self):
-00017730: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00017740: 6369 7065 732e 706f 7028 3029 0a20 2020  cipes.pop(0).   
-00017750: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
-00017760: 7373 6572 7452 6169 7365 7328 6c74 2e53  ssertRaises(lt.S
-00017770: 6561 7263 6849 6e64 6578 496e 636f 6e73  earchIndexIncons
-00017780: 6973 7465 6e74 4572 726f 722c 0a20 2020  istentError,.   
-00017790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177a0: 2020 2020 2020 2020 2020 2020 6d73 673d              msg=
-000177b0: 2266 6169 6c65 6420 746f 2072 6169 7365  "failed to raise
-000177c0: 2065 7863 6570 7469 6f6e 2077 6865 6e20   exception when 
-000177d0: 7365 6172 6368 696e 6720 6d6f 6469 6669  searching modifi
-000177e0: 6564 2074 6162 6c65 2229 3a0a 2020 2020  ed table"):.    
-000177f0: 2020 2020 2020 2020 7365 6c66 2e72 6563          self.rec
-00017800: 6970 6573 2e73 6561 7263 682e 696e 6772  ipes.search.ingr
-00017810: 6564 6965 6e74 7328 2262 6163 6f6e 2229  edients("bacon")
-00017820: 0a0a 2020 2020 4061 6e6e 6f75 6e63 655f  ..    @announce_
-00017830: 7465 7374 0a20 2020 2064 6566 2074 6573  test.    def tes
-00017840: 745f 7365 6172 6368 5f77 6974 685f 6b65  t_search_with_ke
-00017850: 7977 6f72 6473 2873 656c 6629 3a0a 2020  ywords(self):.  
-00017860: 2020 2020 2020 666f 7220 7175 6572 792c        for query,
-00017870: 2065 7870 6563 7465 642c 2065 7870 6563   expected, expec
-00017880: 7465 645f 776f 7264 7320 696e 205b 0a20  ted_words in [. 
-00017890: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-000178a0: 2274 756e 6122 2c20 5b31 2c20 365d 2c20  "tuna", [1, 6], 
-000178b0: 5b7b 2774 756e 6127 2c20 2763 7265 616d  [{'tuna', 'cream
-000178c0: 272c 2027 736f 7570 272c 2027 6e6f 6f64  ', 'soup', 'nood
-000178d0: 6c65 7327 2c20 276d 7573 6872 6f6f 6d27  les', 'mushroom'
-000178e0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-000178f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017900: 2020 2020 207b 2774 6f6d 6174 6f27 2c20       {'tomato', 
-00017910: 2774 756e 6127 2c20 276d 6179 6f6e 6e61  'tuna', 'mayonna
-00017920: 6973 6527 2c20 2762 7265 6164 272c 2027  ise', 'bread', '
-00017930: 6368 6565 7365 277d 5d29 2c0a 2020 2020  cheese'}]),.    
-00017940: 2020 2020 2020 2020 2020 2020 5d3a 0a20              ]:. 
-00017950: 2020 2020 2020 2020 2020 206d 6174 6368             match
-00017960: 6573 203d 2073 656c 662e 7265 6369 7065  es = self.recipe
-00017970: 732e 7365 6172 6368 2e69 6e67 7265 6469  s.search.ingredi
-00017980: 656e 7473 2871 7565 7279 2c20 6d69 6e5f  ents(query, min_
-00017990: 7363 6f72 653d 2d31 3030 3030 2c20 696e  score=-10000, in
-000179a0: 636c 7564 655f 776f 7264 733d 5472 7565  clude_words=True
-000179b0: 290a 2020 2020 2020 2020 2020 2020 6d61  ).            ma
-000179c0: 7463 685f 6964 7320 3d20 5b72 6563 6970  tch_ids = [recip
-000179d0: 652e 6964 2066 6f72 2072 6563 6970 652c  e.id for recipe,
-000179e0: 2073 636f 7265 2c20 776f 7264 7320 696e   score, words in
-000179f0: 206d 6174 6368 6573 5d0a 2020 2020 2020   matches].      
-00017a00: 2020 2020 2020 7072 696e 7428 7265 7072        print(repr
-00017a10: 2871 7565 7279 292c 2027 2d3e 272c 205b  (query), '->', [
-00017a20: 2872 6563 6970 652e 6964 2c20 7363 6f72  (recipe.id, scor
-00017a30: 652c 2077 6f72 6473 2920 666f 7220 7265  e, words) for re
-00017a40: 6369 7065 2c20 7363 6f72 652c 2077 6f72  cipe, score, wor
-00017a50: 6473 2069 6e20 6d61 7463 6865 735d 290a  ds in matches]).
-00017a60: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00017a70: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-00017a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017a90: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00017aa0: 6c28 6578 7065 6374 6564 2c20 6d61 7463  l(expected, matc
-00017ab0: 685f 6964 732c 0a20 2020 2020 2020 2020  h_ids,.         
-00017ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ad0: 2020 2020 2020 2020 6622 696e 7661 6c69          f"invali
-00017ae0: 6420 7265 7375 6c74 7320 666f 7220 7175  d results for qu
-00017af0: 6572 7920 7b71 7565 7279 2172 7d2c 2065  ery {query!r}, e
-00017b00: 7870 6563 7465 6420 7b65 7870 6563 7465  xpected {expecte
-00017b10: 647d 2c20 676f 7420 7b6d 6174 6368 5f69  d}, got {match_i
-00017b20: 6473 7d22 290a 2020 2020 2020 2020 2020  ds}").          
-00017b30: 2020 6d61 7463 685f 776f 7264 7320 3d20    match_words = 
-00017b40: 5b73 6574 2877 6f72 6473 2920 666f 7220  [set(words) for 
-00017b50: 7265 6369 7065 2c20 7363 6f72 652c 2077  recipe, score, w
-00017b60: 6f72 6473 2069 6e20 6d61 7463 6865 735d  ords in matches]
-00017b70: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00017b80: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-00017b90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00017ba0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00017bb0: 616c 2865 7870 6563 7465 645f 776f 7264  al(expected_word
-00017bc0: 732c 206d 6174 6368 5f77 6f72 6473 2c0a  s, match_words,.
-00017bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017bf0: 2022 696e 7661 6c69 6420 6d61 7463 6820   "invalid match 
-00017c00: 776f 7264 7320 666f 7220 7175 6572 7920  words for query 
-00017c10: 7b21 727d 2c20 6578 7065 6374 6564 207b  {!r}, expected {
-00017c20: 7d2c 2067 6f74 207b 7d22 2e66 6f72 6d61  }, got {}".forma
-00017c30: 7428 7175 6572 792c 0a20 2020 2020 2020  t(query,.       
-00017c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017580: 6173 5f74 6162 6c65 3d46 616c 7365 2c20  as_table=False, 
+00017590: 6d69 6e5f 7363 6f72 653d 2d31 3030 3030  min_score=-10000
+000175a0: 290a 2020 2020 2020 2020 2020 2020 6d61  ).            ma
+000175b0: 7463 685f 6964 7320 3d20 5b72 6563 6970  tch_ids = [recip
+000175c0: 652e 6964 2066 6f72 2072 6563 6970 652c  e.id for recipe,
+000175d0: 205f 2069 6e20 6d61 7463 6865 735d 0a20   _ in matches]. 
+000175e0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000175f0: 2872 6570 7228 7175 6572 7929 2c20 272d  (repr(query), '-
+00017600: 3e27 2c20 5b28 7265 6369 7065 2e69 642c  >', [(recipe.id,
+00017610: 2073 636f 7265 2920 666f 7220 7265 6369   score) for reci
+00017620: 7065 2c20 7363 6f72 6520 696e 206d 6174  pe, score in mat
+00017630: 6368 6573 5d29 0a20 2020 2020 2020 2020  ches]).         
+00017640: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+00017650: 5465 7374 2871 7565 7279 3d71 7565 7279  Test(query=query
+00017660: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00017670: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00017680: 7561 6c28 6578 7065 6374 6564 2c20 6d61  ual(expected, ma
+00017690: 7463 685f 6964 732c 0a20 2020 2020 2020  tch_ids,.       
+000176a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000176b0: 2020 2020 2020 2020 2020 6622 696e 7661            f"inva
+000176c0: 6c69 6420 7265 7375 6c74 7320 666f 7220  lid results for 
+000176d0: 7175 6572 7920 7b71 7565 7279 2172 7d2c  query {query!r},
+000176e0: 2065 7870 6563 7465 6420 7b65 7870 6563   expected {expec
+000176f0: 7465 647d 2c20 676f 7420 7b6d 6174 6368  ted}, got {match
+00017700: 5f69 6473 7d22 290a 0a20 2020 2040 616e  _ids}")..    @an
+00017710: 6e6f 756e 6365 5f74 6573 740a 2020 2020  nounce_test.    
+00017720: 6465 6620 7465 7374 5f69 6e76 616c 6964  def test_invalid
+00017730: 6174 655f 696e 6465 7828 7365 6c66 293a  ate_index(self):
+00017740: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00017750: 6369 7065 732e 706f 7028 3029 0a20 2020  cipes.pop(0).   
+00017760: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
+00017770: 7373 6572 7452 6169 7365 7328 6c74 2e53  ssertRaises(lt.S
+00017780: 6561 7263 6849 6e64 6578 496e 636f 6e73  earchIndexIncons
+00017790: 6973 7465 6e74 4572 726f 722c 0a20 2020  istentError,.   
+000177a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000177b0: 2020 2020 2020 2020 2020 2020 6d73 673d              msg=
+000177c0: 2266 6169 6c65 6420 746f 2072 6169 7365  "failed to raise
+000177d0: 2065 7863 6570 7469 6f6e 2077 6865 6e20   exception when 
+000177e0: 7365 6172 6368 696e 6720 6d6f 6469 6669  searching modifi
+000177f0: 6564 2074 6162 6c65 2229 3a0a 2020 2020  ed table"):.    
+00017800: 2020 2020 2020 2020 7365 6c66 2e72 6563          self.rec
+00017810: 6970 6573 2e73 6561 7263 682e 696e 6772  ipes.search.ingr
+00017820: 6564 6965 6e74 7328 2262 6163 6f6e 2229  edients("bacon")
+00017830: 0a0a 2020 2020 4061 6e6e 6f75 6e63 655f  ..    @announce_
+00017840: 7465 7374 0a20 2020 2064 6566 2074 6573  test.    def tes
+00017850: 745f 7365 6172 6368 5f77 6974 685f 6b65  t_search_with_ke
+00017860: 7977 6f72 6473 2873 656c 6629 3a0a 2020  ywords(self):.  
+00017870: 2020 2020 2020 666f 7220 7175 6572 792c        for query,
+00017880: 2065 7870 6563 7465 642c 2065 7870 6563   expected, expec
+00017890: 7465 645f 776f 7264 7320 696e 205b 0a20  ted_words in [. 
+000178a0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+000178b0: 2274 756e 6122 2c20 5b31 2c20 365d 2c20  "tuna", [1, 6], 
+000178c0: 5b7b 2774 756e 6127 2c20 2763 7265 616d  [{'tuna', 'cream
+000178d0: 272c 2027 736f 7570 272c 2027 6e6f 6f64  ', 'soup', 'nood
+000178e0: 6c65 7327 2c20 276d 7573 6872 6f6f 6d27  les', 'mushroom'
+000178f0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+00017900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017910: 2020 2020 207b 2774 6f6d 6174 6f27 2c20       {'tomato', 
+00017920: 2774 756e 6127 2c20 276d 6179 6f6e 6e61  'tuna', 'mayonna
+00017930: 6973 6527 2c20 2762 7265 6164 272c 2027  ise', 'bread', '
+00017940: 6368 6565 7365 277d 5d29 2c0a 2020 2020  cheese'}]),.    
+00017950: 2020 2020 2020 2020 2020 2020 5d3a 0a20              ]:. 
+00017960: 2020 2020 2020 2020 2020 206d 6174 6368             match
+00017970: 6573 203d 2073 656c 662e 7265 6369 7065  es = self.recipe
+00017980: 732e 7365 6172 6368 2e69 6e67 7265 6469  s.search.ingredi
+00017990: 656e 7473 2871 7565 7279 2c20 6d69 6e5f  ents(query, min_
+000179a0: 7363 6f72 653d 2d31 3030 3030 2c20 6173  score=-10000, as
+000179b0: 5f74 6162 6c65 3d46 616c 7365 2c20 696e  _table=False, in
+000179c0: 636c 7564 655f 776f 7264 733d 5472 7565  clude_words=True
+000179d0: 290a 2020 2020 2020 2020 2020 2020 6d61  ).            ma
+000179e0: 7463 685f 6964 7320 3d20 5b72 6563 6970  tch_ids = [recip
+000179f0: 652e 6964 2066 6f72 2072 6563 6970 652c  e.id for recipe,
+00017a00: 2073 636f 7265 2c20 776f 7264 7320 696e   score, words in
+00017a10: 206d 6174 6368 6573 5d0a 2020 2020 2020   matches].      
+00017a20: 2020 2020 2020 7072 696e 7428 7265 7072        print(repr
+00017a30: 2871 7565 7279 292c 2027 2d3e 272c 205b  (query), '->', [
+00017a40: 2872 6563 6970 652e 6964 2c20 7363 6f72  (recipe.id, scor
+00017a50: 652c 2077 6f72 6473 2920 666f 7220 7265  e, words) for re
+00017a60: 6369 7065 2c20 7363 6f72 652c 2077 6f72  cipe, score, wor
+00017a70: 6473 2069 6e20 6d61 7463 6865 735d 290a  ds in matches]).
+00017a80: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00017a90: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
+00017aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017ab0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00017ac0: 6c28 6578 7065 6374 6564 2c20 6d61 7463  l(expected, matc
+00017ad0: 685f 6964 732c 0a20 2020 2020 2020 2020  h_ids,.         
+00017ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017af0: 2020 2020 2020 2020 6622 696e 7661 6c69          f"invali
+00017b00: 6420 7265 7375 6c74 7320 666f 7220 7175  d results for qu
+00017b10: 6572 7920 7b71 7565 7279 2172 7d2c 2065  ery {query!r}, e
+00017b20: 7870 6563 7465 6420 7b65 7870 6563 7465  xpected {expecte
+00017b30: 647d 2c20 676f 7420 7b6d 6174 6368 5f69  d}, got {match_i
+00017b40: 6473 7d22 290a 2020 2020 2020 2020 2020  ds}").          
+00017b50: 2020 6d61 7463 685f 776f 7264 7320 3d20    match_words = 
+00017b60: 5b73 6574 2877 6f72 6473 2920 666f 7220  [set(words) for 
+00017b70: 7265 6369 7065 2c20 7363 6f72 652c 2077  recipe, score, w
+00017b80: 6f72 6473 2069 6e20 6d61 7463 6865 735d  ords in matches]
+00017b90: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00017ba0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00017bb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017bc0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00017bd0: 616c 2865 7870 6563 7465 645f 776f 7264  al(expected_word
+00017be0: 732c 206d 6174 6368 5f77 6f72 6473 2c0a  s, match_words,.
+00017bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c10: 2022 696e 7661 6c69 6420 6d61 7463 6820   "invalid match 
+00017c20: 776f 7264 7320 666f 7220 7175 6572 7920  words for query 
+00017c30: 7b21 727d 2c20 6578 7065 6374 6564 207b  {!r}, expected {
+00017c40: 7d2c 2067 6f74 207b 7d22 2e66 6f72 6d61  }, got {}".forma
+00017c50: 7428 7175 6572 792c 0a20 2020 2020 2020  t(query,.       
 00017c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c90: 2020 2020 2020 2020 2020 2065 7870 6563             expec
-00017ca0: 7465 645f 776f 7264 732c 0a20 2020 2020  ted_words,.     
-00017cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017cb0: 2020 2020 2020 2020 2020 2065 7870 6563             expec
+00017cc0: 7465 645f 776f 7264 732c 0a20 2020 2020  ted_words,.     
 00017cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d00: 2020 2020 2020 2020 2020 2020 206d 6174               mat
-00017d10: 6368 5f77 6f72 6473 2929 0a0a 2020 2020  ch_words))..    
-00017d20: 4061 6e6e 6f75 6e63 655f 7465 7374 0a20  @announce_test. 
-00017d30: 2020 2064 6566 2074 6573 745f 7365 6172     def test_sear
-00017d40: 6368 5f77 6974 685f 6c69 6d69 7428 7365  ch_with_limit(se
-00017d50: 6c66 293a 0a20 2020 2020 2020 2066 6f72  lf):.        for
-00017d60: 2071 7565 7279 2c20 6578 7065 6374 6564   query, expected
-00017d70: 2069 6e20 5b0a 2020 2020 2020 2020 2020   in [.          
-00017d80: 2020 2822 222c 205b 5d29 2c0a 2020 2020    ("", []),.    
-00017d90: 2020 2020 2020 2020 2822 7475 6e61 222c          ("tuna",
-00017da0: 205b 312c 2036 5d29 2c0a 2020 2020 2020   [1, 6]),.      
-00017db0: 2020 2020 2020 2822 7475 6e61 202b 6368        ("tuna +ch
-00017dc0: 6565 7365 222c 205b 362c 2033 2c20 345d  eese", [6, 3, 4]
-00017dd0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-00017de0: 2270 696e 6561 7070 6c65 202b 6261 636f  "pineapple +baco
-00017df0: 6e20 6c65 7474 7563 6520 6265 6566 202d  n lettuce beef -
-00017e00: 7361 7565 726b 7261 7574 2074 6f6d 6174  sauerkraut tomat
-00017e10: 6f22 2c20 5b39 2c20 3133 2c20 325d 292c  o", [9, 13, 2]),
-00017e20: 0a20 2020 2020 2020 2020 2020 2028 2270  .            ("p
-00017e30: 697a 7a61 2064 6f75 6768 202d 7069 6e65  izza dough -pine
-00017e40: 6170 706c 6522 2c20 5b33 2c20 342c 2032  apple", [3, 4, 2
-00017e50: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-00017e60: 2822 7069 7a7a 6120 646f 7567 6820 2d2d  ("pizza dough --
-00017e70: 7069 6e65 6170 706c 6522 2c20 5b33 2c20  pineapple", [3, 
-00017e80: 345d 292c 0a20 2020 2020 2020 2020 2020  4]),.           
-00017e90: 2028 2262 7265 6164 2062 6163 6f6e 222c   ("bread bacon",
-00017ea0: 205b 392c 2035 2c20 365d 292c 0a20 2020   [9, 5, 6]),.   
-00017eb0: 2020 2020 2020 2020 2028 2262 7265 6164           ("bread
-00017ec0: 202b 2b62 6163 6f6e 222c 205b 392c 2031   ++bacon", [9, 1
-00017ed0: 335d 292c 0a20 2020 2020 2020 2020 2020  3]),.           
-00017ee0: 2028 2262 7265 6164 202b 2b61 6e63 686f   ("bread ++ancho
-00017ef0: 7669 6573 222c 205b 5d29 2c0a 2020 2020  vies", []),.    
-00017f00: 2020 2020 2020 2020 2822 6272 6561 6420          ("bread 
-00017f10: 2b2b 6261 636f 6e20 2b2b 616e 6368 6f76  ++bacon ++anchov
-00017f20: 6965 7322 2c20 5b5d 292c 0a20 2020 2020  ies", []),.     
-00017f30: 2020 2020 2020 2028 2262 7265 6164 2062         ("bread b
-00017f40: 6163 6f6e 202d 2d61 6e63 686f 7669 6573  acon --anchovies
-00017f50: 222c 205b 392c 2035 2c20 365d 292c 0a20  ", [9, 5, 6]),. 
-00017f60: 2020 2020 2020 205d 3a0a 2020 2020 2020         ]:.      
-00017f70: 2020 2020 2020 6d61 7463 6865 7320 3d20        matches = 
-00017f80: 7365 6c66 2e72 6563 6970 6573 2e73 6561  self.recipes.sea
-00017f90: 7263 682e 696e 6772 6564 6965 6e74 7328  rch.ingredients(
-00017fa0: 7175 6572 792c 206d 696e 5f73 636f 7265  query, min_score
-00017fb0: 3d2d 3130 3030 302c 206c 696d 6974 3d33  =-10000, limit=3
-00017fc0: 290a 2020 2020 2020 2020 2020 2020 6d61  ).            ma
-00017fd0: 7463 685f 6964 7320 3d20 5b72 6563 6970  tch_ids = [recip
-00017fe0: 652e 6964 2066 6f72 2072 6563 6970 652c  e.id for recipe,
-00017ff0: 205f 2069 6e20 6d61 7463 6865 735d 0a20   _ in matches]. 
-00018000: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00018010: 2872 6570 7228 7175 6572 7929 2c20 272d  (repr(query), '-
-00018020: 3e27 2c20 5b28 7265 6369 7065 2e69 642c  >', [(recipe.id,
-00018030: 2073 636f 7265 2920 666f 7220 7265 6369   score) for reci
-00018040: 7065 2c20 7363 6f72 6520 696e 206d 6174  pe, score in mat
-00018050: 6368 6573 5d29 0a20 2020 2020 2020 2020  ches]).         
-00018060: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-00018070: 5465 7374 2871 7565 7279 3d71 7565 7279  Test(query=query
-00018080: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00018090: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000180a0: 7561 6c28 6578 7065 6374 6564 2c20 6d61  ual(expected, ma
-000180b0: 7463 685f 6964 732c 0a20 2020 2020 2020  tch_ids,.       
-000180c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000180d0: 2020 2020 2020 2020 2020 6622 696e 7661            f"inva
-000180e0: 6c69 6420 7265 7375 6c74 7320 666f 7220  lid results for 
-000180f0: 7175 6572 7920 7b71 7565 7279 2172 7d2c  query {query!r},
-00018100: 2065 7870 6563 7465 6420 7b65 7870 6563   expected {expec
-00018110: 7465 647d 2c20 676f 7420 7b6d 6174 6368  ted}, got {match
-00018120: 5f69 6473 7d22 290a 0a20 2020 2040 616e  _ids}")..    @an
-00018130: 6e6f 756e 6365 5f74 6573 740a 2020 2020  nounce_test.    
-00018140: 6465 6620 7465 7374 5f73 6561 7263 685f  def test_search_
-00018150: 7769 7468 5f6d 696e 5f73 636f 7265 2873  with_min_score(s
-00018160: 656c 6629 3a0a 2020 2020 2020 2020 666f  elf):.        fo
-00018170: 7220 7175 6572 792c 2065 7870 6563 7465  r query, expecte
-00018180: 6420 696e 205b 0a20 2020 2020 2020 2020  d in [.         
-00018190: 2020 2028 2222 2c20 5b5d 292c 0a20 2020     ("", []),.   
-000181a0: 2020 2020 2020 2020 2028 2274 756e 6122           ("tuna"
-000181b0: 2c20 5b5d 292c 0a20 2020 2020 2020 2020  , []),.         
-000181c0: 2020 2028 2274 756e 6120 2b63 6865 6573     ("tuna +chees
-000181d0: 6522 2c20 5b36 2c5d 292c 0a20 2020 2020  e", [6,]),.     
-000181e0: 2020 2020 2020 2028 2270 696e 6561 7070         ("pineapp
-000181f0: 6c65 202b 6261 636f 6e20 6c65 7474 7563  le +bacon lettuc
-00018200: 6520 6265 6566 202d 7361 7565 726b 7261  e beef -sauerkra
-00018210: 7574 2074 6f6d 6174 6f22 2c20 5b39 2c20  ut tomato", [9, 
-00018220: 3133 5d29 2c0a 2020 2020 2020 2020 2020  13]),.          
-00018230: 2020 2822 7069 7a7a 6120 646f 7567 6820    ("pizza dough 
-00018240: 2d70 696e 6561 7070 6c65 222c 205b 5d29  -pineapple", [])
-00018250: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
-00018260: 7069 7a7a 6120 646f 7567 6820 2d2d 7069  pizza dough --pi
-00018270: 6e65 6170 706c 6522 2c20 5b5d 292c 0a20  neapple", []),. 
-00018280: 2020 2020 2020 2020 2020 2028 2262 7265             ("bre
-00018290: 6164 2062 6163 6f6e 222c 205b 5d29 2c0a  ad bacon", []),.
-000182a0: 2020 2020 2020 2020 2020 2020 2822 6272              ("br
-000182b0: 6561 6420 2b2b 6261 636f 6e22 2c20 5b39  ead ++bacon", [9
-000182c0: 2c5d 292c 0a20 2020 2020 2020 2020 2020  ,]),.           
-000182d0: 2028 2262 7265 6164 202b 2b61 6e63 686f   ("bread ++ancho
-000182e0: 7669 6573 222c 205b 5d29 2c0a 2020 2020  vies", []),.    
-000182f0: 2020 2020 2020 2020 2822 6272 6561 6420          ("bread 
-00018300: 2b2b 6261 636f 6e20 2b2b 616e 6368 6f76  ++bacon ++anchov
-00018310: 6965 7322 2c20 5b5d 292c 0a20 2020 2020  ies", []),.     
-00018320: 2020 2020 2020 2028 2262 7265 6164 2062         ("bread b
-00018330: 6163 6f6e 202d 2d61 6e63 686f 7669 6573  acon --anchovies
-00018340: 222c 205b 5d29 2c0a 2020 2020 2020 2020  ", []),.        
-00018350: 5d3a 0a20 2020 2020 2020 2020 2020 206d  ]:.            m
-00018360: 6174 6368 6573 203d 2073 656c 662e 7265  atches = self.re
-00018370: 6369 7065 732e 7365 6172 6368 2e69 6e67  cipes.search.ing
-00018380: 7265 6469 656e 7473 2871 7565 7279 2c20  redients(query, 
-00018390: 6d69 6e5f 7363 6f72 653d 3130 3030 290a  min_score=1000).
-000183a0: 2020 2020 2020 2020 2020 2020 6d61 7463              matc
-000183b0: 685f 6964 7320 3d20 5b72 6563 6970 652e  h_ids = [recipe.
-000183c0: 6964 2066 6f72 2072 6563 6970 652c 205f  id for recipe, _
-000183d0: 2069 6e20 6d61 7463 6865 735d 0a20 2020   in matches].   
-000183e0: 2020 2020 2020 2020 2070 7269 6e74 2872           print(r
-000183f0: 6570 7228 7175 6572 7929 2c20 272d 3e27  epr(query), '->'
-00018400: 2c20 5b28 7265 6369 7065 2e69 642c 2073  , [(recipe.id, s
-00018410: 636f 7265 2920 666f 7220 7265 6369 7065  core) for recipe
-00018420: 2c20 7363 6f72 6520 696e 206d 6174 6368  , score in match
-00018430: 6573 5d29 0a20 2020 2020 2020 2020 2020  es]).           
-00018440: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00018450: 7374 2871 7565 7279 3d71 7565 7279 293a  st(query=query):
-00018460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018470: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00018480: 6c28 6578 7065 6374 6564 2c20 6d61 7463  l(expected, matc
-00018490: 685f 6964 732c 0a20 2020 2020 2020 2020  h_ids,.         
-000184a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184b0: 2020 2020 2020 2020 6622 696e 7661 6c69          f"invali
-000184c0: 6420 7265 7375 6c74 7320 666f 7220 7175  d results for qu
-000184d0: 6572 7920 7b71 7565 7279 2172 7d2c 2065  ery {query!r}, e
-000184e0: 7870 6563 7465 6420 7b65 7870 6563 7465  xpected {expecte
-000184f0: 647d 2c20 676f 7420 7b6d 6174 6368 5f69  d}, got {match_i
-00018500: 6473 7d22 290a 0a20 2020 2040 616e 6e6f  ds}")..    @anno
-00018510: 756e 6365 5f74 6573 740a 2020 2020 6465  unce_test.    de
-00018520: 6620 7465 7374 5f73 6561 7263 685f 7769  f test_search_wi
-00018530: 7468 5f61 735f 7461 626c 6528 7365 6c66  th_as_table(self
-00018540: 293a 0a20 2020 2020 2020 2066 6f72 2071  ):.        for q
-00018550: 7565 7279 2c20 6578 7065 6374 6564 2069  uery, expected i
-00018560: 6e20 5b0a 2020 2020 2020 2020 2020 2020  n [.            
-00018570: 2822 222c 205b 5d29 2c0a 2020 2020 2020  ("", []),.      
-00018580: 2020 2020 2020 2822 7475 6e61 222c 205b        ("tuna", [
-00018590: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-000185a0: 2822 7475 6e61 202b 6368 6565 7365 222c  ("tuna +cheese",
-000185b0: 205b 362c 5d29 2c0a 2020 2020 2020 2020   [6,]),.        
-000185c0: 2020 2020 2822 7069 6e65 6170 706c 6520      ("pineapple 
-000185d0: 2b62 6163 6f6e 206c 6574 7475 6365 2062  +bacon lettuce b
-000185e0: 6565 6620 2d73 6175 6572 6b72 6175 7420  eef -sauerkraut 
-000185f0: 746f 6d61 746f 222c 205b 392c 2031 335d  tomato", [9, 13]
-00018600: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-00018610: 2270 697a 7a61 2064 6f75 6768 202d 7069  "pizza dough -pi
-00018620: 6e65 6170 706c 6522 2c20 5b5d 292c 0a20  neapple", []),. 
-00018630: 2020 2020 2020 2020 2020 2028 2270 697a             ("piz
-00018640: 7a61 2064 6f75 6768 202d 2d70 696e 6561  za dough --pinea
-00018650: 7070 6c65 222c 205b 5d29 2c0a 2020 2020  pple", []),.    
-00018660: 2020 2020 2020 2020 2822 6272 6561 6420          ("bread 
-00018670: 6261 636f 6e22 2c20 5b5d 292c 0a20 2020  bacon", []),.   
-00018680: 2020 2020 2020 2020 2028 2262 7265 6164           ("bread
-00018690: 202b 2b62 6163 6f6e 222c 205b 392c 5d29   ++bacon", [9,])
-000186a0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
-000186b0: 6272 6561 6420 2b2b 616e 6368 6f76 6965  bread ++anchovie
-000186c0: 7322 2c20 5b5d 292c 0a20 2020 2020 2020  s", []),.       
-000186d0: 2020 2020 2028 2262 7265 6164 202b 2b62       ("bread ++b
-000186e0: 6163 6f6e 202b 2b61 6e63 686f 7669 6573  acon ++anchovies
-000186f0: 222c 205b 5d29 2c0a 2020 2020 2020 2020  ", []),.        
-00018700: 2020 2020 2822 6272 6561 6420 6261 636f      ("bread baco
-00018710: 6e20 2d2d 616e 6368 6f76 6965 7322 2c20  n --anchovies", 
-00018720: 5b5d 292c 0a20 2020 2020 2020 205d 3a0a  []),.        ]:.
-00018730: 2020 2020 2020 2020 2020 2020 6d61 7463              matc
-00018740: 6865 7320 3d20 7365 6c66 2e72 6563 6970  hes = self.recip
-00018750: 6573 2e73 6561 7263 682e 696e 6772 6564  es.search.ingred
-00018760: 6965 6e74 7328 7175 6572 792c 206d 696e  ients(query, min
-00018770: 5f73 636f 7265 3d31 3030 302c 2061 735f  _score=1000, as_
-00018780: 7461 626c 653d 5472 7565 290a 2020 2020  table=True).    
-00018790: 2020 2020 2020 2020 6d61 7463 685f 6964          match_id
-000187a0: 7320 3d20 5b72 6563 6970 652e 6964 2066  s = [recipe.id f
-000187b0: 6f72 2072 6563 6970 6520 696e 206d 6174  or recipe in mat
-000187c0: 6368 6573 5d0a 2020 2020 2020 2020 2020  ches].          
-000187d0: 2020 7072 696e 7428 7265 7072 2871 7565    print(repr(que
-000187e0: 7279 292c 2027 2d3e 272c 205b 2872 6563  ry), '->', [(rec
-000187f0: 6970 652e 6964 2c20 7265 6369 7065 2e69  ipe.id, recipe.i
-00018800: 6e67 7265 6469 656e 7473 5f73 6561 7263  ngredients_searc
-00018810: 685f 7363 6f72 6529 2066 6f72 2072 6563  h_score) for rec
-00018820: 6970 6520 696e 206d 6174 6368 6573 5d29  ipe in matches])
-00018830: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00018840: 6820 7365 6c66 2e73 7562 5465 7374 2871  h self.subTest(q
-00018850: 7565 7279 3d71 7565 7279 293a 0a20 2020  uery=query):.   
-00018860: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018870: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
-00018880: 7065 6374 6564 2c20 6d61 7463 685f 6964  pected, match_id
-00018890: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-000188a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188b0: 2020 2020 6622 696e 7661 6c69 6420 7265      f"invalid re
-000188c0: 7375 6c74 7320 666f 7220 7175 6572 7920  sults for query 
-000188d0: 7b71 7565 7279 2172 7d2c 2065 7870 6563  {query!r}, expec
-000188e0: 7465 6420 7b65 7870 6563 7465 647d 2c20  ted {expected}, 
-000188f0: 676f 7420 7b6d 6174 6368 5f69 6473 7d22  got {match_ids}"
-00018900: 290a 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00018910: 636f 7265 5f61 7474 7220 3d20 2269 6e67  core_attr = "ing
-00018920: 7265 6469 656e 7473 5f73 6561 7263 685f  redients_search_
-00018930: 7363 6f72 6522 0a20 2020 2020 2020 2020  score".         
-00018940: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-00018950: 7565 280a 2020 2020 2020 2020 2020 2020  ue(.            
-00018960: 2020 2020 616c 6c28 0a20 2020 2020 2020      all(.       
-00018970: 2020 2020 2020 2020 2020 2020 2068 6173               has
-00018980: 6174 7472 286d 6174 6368 6573 2e62 792e  attr(matches.by.
-00018990: 6964 5b6d 6964 5d2c 2073 636f 7265 5f61  id[mid], score_a
-000189a0: 7474 7229 0a20 2020 2020 2020 2020 2020  ttr).           
-000189b0: 2020 2020 2020 2020 2066 6f72 206d 6964           for mid
-000189c0: 2069 6e20 6d61 7463 685f 6964 730a 2020   in match_ids.  
-000189d0: 2020 2020 2020 2020 2020 2020 2020 292c                ),
-000189e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000189f0: 2066 2261 735f 7461 626c 6520 6469 6420   f"as_table did 
-00018a00: 6e6f 7420 706f 7075 6c61 7465 2073 6f6d  not populate som
-00018a10: 6520 7365 6172 6368 2072 6563 6f72 6473  e search records
-00018a20: 2077 6974 6820 7b73 636f 7265 5f61 7474   with {score_att
-00018a30: 7221 727d 220a 2020 2020 2020 2020 2020  r!r}".          
-00018a40: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
-00018a50: 2073 656c 662e 6173 7365 7274 4661 6c73   self.assertFals
-00018a60: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00018a70: 2020 2061 6e79 280a 2020 2020 2020 2020     any(.        
-00018a80: 2020 2020 2020 2020 2020 2020 6861 7361              hasa
-00018a90: 7474 7228 7365 6c66 2e72 6563 6970 6573  ttr(self.recipes
-00018aa0: 2e62 792e 6964 5b6d 6964 5d2c 2073 636f  .by.id[mid], sco
-00018ab0: 7265 5f61 7474 7229 0a20 2020 2020 2020  re_attr).       
-00018ac0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00018ad0: 206d 6964 2069 6e20 6d61 7463 685f 6964   mid in match_id
-00018ae0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00018af0: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00018b00: 2020 2020 2066 2261 735f 7461 626c 6520       f"as_table 
-00018b10: 706f 7075 6c61 7465 6420 736f 6d65 206f  populated some o
-00018b20: 7269 6769 6e61 6c20 7265 636f 7264 7320  riginal records 
-00018b30: 7769 7468 207b 7363 6f72 655f 6174 7472  with {score_attr
-00018b40: 2172 7d22 0a20 2020 2020 2020 2020 2020  !r}".           
-00018b50: 2029 0a0a 636c 6173 7320 5461 626c 6553   )..class TableS
-00018b60: 6561 7263 6854 6573 7473 5f44 6174 614f  earchTests_DataO
-00018b70: 626a 6563 7473 2854 6162 6c65 5365 6172  bjects(TableSear
-00018b80: 6368 5465 7374 732c 2055 7369 6e67 4461  chTests, UsingDa
-00018b90: 7461 4f62 6a65 6374 7329 3a0a 2020 2020  taObjects):.    
-00018ba0: 7061 7373 0a0a 636c 6173 7320 5461 626c  pass..class Tabl
-00018bb0: 6553 6561 7263 6854 6573 7473 5f4e 616d  eSearchTests_Nam
-00018bc0: 6564 7475 706c 6573 2854 6162 6c65 5365  edtuples(TableSe
-00018bd0: 6172 6368 5465 7374 732c 2055 7369 6e67  archTests, Using
-00018be0: 4e61 6d65 6474 7570 6c65 7329 3a0a 2020  Namedtuples):.  
-00018bf0: 2020 7061 7373 0a0a 636c 6173 7320 5461    pass..class Ta
-00018c00: 626c 6553 6561 7263 6854 6573 7473 5f44  bleSearchTests_D
-00018c10: 6174 614e 616d 6564 7475 706c 6573 2854  ataNamedtuples(T
-00018c20: 6162 6c65 5365 6172 6368 5465 7374 732c  ableSearchTests,
-00018c30: 2055 7369 6e67 4461 7461 4e61 6d65 6474   UsingDataNamedt
-00018c40: 7570 6c65 7329 3a0a 2020 2020 7061 7373  uples):.    pass
-00018c50: 0a0a 636c 6173 7320 5461 626c 6553 6561  ..class TableSea
-00018c60: 7263 6854 6573 7473 5f53 6c6f 7474 6564  rchTests_Slotted
-00018c70: 2854 6162 6c65 5365 6172 6368 5465 7374  (TableSearchTest
-00018c80: 732c 2055 7369 6e67 536c 6f74 7465 644f  s, UsingSlottedO
-00018c90: 626a 6563 7473 293a 0a20 2020 2070 6173  bjects):.    pas
-00018ca0: 730a 0a63 6c61 7373 2054 6162 6c65 5365  s..class TableSe
-00018cb0: 6172 6368 5465 7374 735f 5369 6d70 6c65  archTests_Simple
-00018cc0: 4e61 6d65 7370 6163 6528 5461 626c 6553  Namespace(TableS
-00018cd0: 6561 7263 6854 6573 7473 2c20 5573 696e  earchTests, Usin
-00018ce0: 6753 696d 706c 654e 616d 6573 7061 6365  gSimpleNamespace
-00018cf0: 293a 0a20 2020 2070 6173 730a 0a69 6620  ):.    pass..if 
-00018d00: 6461 7461 636c 6173 7365 7320 6973 206e  dataclasses is n
-00018d10: 6f74 204e 6f6e 653a 0a20 2020 2063 6c61  ot None:.    cla
-00018d20: 7373 2054 6162 6c65 5365 6172 6368 5465  ss TableSearchTe
-00018d30: 7374 735f 4461 7461 636c 6173 7365 7328  sts_Dataclasses(
-00018d40: 5461 626c 6553 6561 7263 6854 6573 7473  TableSearchTests
-00018d50: 2c20 5573 696e 6744 6174 6163 6c61 7373  , UsingDataclass
-00018d60: 6573 293a 0a20 2020 2020 2020 2070 6173  es):.        pas
-00018d70: 730a 0a69 6620 7079 6461 6e74 6963 2069  s..if pydantic i
-00018d80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00018d90: 636c 6173 7320 5461 626c 6553 6561 7263  class TableSearc
-00018da0: 6854 6573 7473 5f50 7964 616e 7469 634d  hTests_PydanticM
-00018db0: 6f64 656c 7328 5461 626c 6553 6561 7263  odels(TableSearc
-00018dc0: 6854 6573 7473 2c20 5573 696e 6750 7964  hTests, UsingPyd
-00018dd0: 616e 7469 634d 6f64 656c 293a 0a20 2020  anticModel):.   
-00018de0: 2020 2020 2070 6173 730a 0a20 2020 2063       pass..    c
-00018df0: 6c61 7373 2054 6162 6c65 5365 6172 6368  lass TableSearch
-00018e00: 5465 7374 735f 5079 6461 6e74 6963 496d  Tests_PydanticIm
-00018e10: 6d75 7461 626c 654d 6f64 656c 7328 5461  mutableModels(Ta
-00018e20: 626c 6553 6561 7263 6854 6573 7473 2c20  bleSearchTests, 
-00018e30: 5573 696e 6750 7964 616e 7469 6349 6d6d  UsingPydanticImm
-00018e40: 7574 6162 6c65 4d6f 6465 6c29 3a0a 2020  utableModel):.  
-00018e50: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00018e60: 636c 6173 7320 5461 626c 6553 6561 7263  class TableSearc
-00018e70: 6854 6573 7473 5f50 7964 616e 7469 634f  hTests_PydanticO
-00018e80: 524d 4d6f 6465 6c73 2854 6162 6c65 5365  RMModels(TableSe
-00018e90: 6172 6368 5465 7374 732c 2055 7369 6e67  archTests, Using
-00018ea0: 5079 6461 6e74 6963 4f52 4d4d 6f64 656c  PydanticORMModel
-00018eb0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-00018ec0: 0a69 6620 6174 7472 2069 7320 6e6f 7420  .if attr is not 
-00018ed0: 4e6f 6e65 3a0a 2020 2020 636c 6173 7320  None:.    class 
-00018ee0: 5461 626c 6553 6561 7263 6854 6573 7473  TableSearchTests
-00018ef0: 5f41 7474 7243 6c61 7373 6573 2854 6162  _AttrClasses(Tab
-00018f00: 6c65 5365 6172 6368 5465 7374 732c 2055  leSearchTests, U
-00018f10: 7369 6e67 4174 7472 436c 6173 7329 3a0a  singAttrClass):.
-00018f20: 2020 2020 2020 2020 7061 7373 0a0a 6966          pass..if
-00018f30: 2074 7261 6974 6c65 7473 2069 7320 6e6f   traitlets is no
-00018f40: 7420 4e6f 6e65 3a0a 2020 2020 636c 6173  t None:.    clas
-00018f50: 7320 5461 626c 6553 6561 7263 6854 6573  s TableSearchTes
-00018f60: 7473 5f54 7261 6974 6c65 7473 436c 6173  ts_TraitletsClas
-00018f70: 7365 7328 5461 626c 6553 6561 7263 6854  ses(TableSearchT
-00018f80: 6573 7473 2c20 5573 696e 6754 7261 6974  ests, UsingTrait
-00018f90: 6c65 7473 436c 6173 7329 3a0a 2020 2020  letsClass):.    
-00018fa0: 2020 2020 7061 7373 0a0a 6966 2053 6c6f      pass..if Slo
-00018fb0: 7474 6564 5769 7468 4469 6374 2069 7320  ttedWithDict is 
-00018fc0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 636c  not None:.    cl
-00018fd0: 6173 7320 5461 626c 6553 6561 7263 6854  ass TableSearchT
-00018fe0: 6573 7473 5f53 6c6f 7474 6564 5769 7468  ests_SlottedWith
-00018ff0: 4469 6374 2854 6162 6c65 5365 6172 6368  Dict(TableSearch
-00019000: 5465 7374 732c 2055 7369 6e67 536c 6f74  Tests, UsingSlot
-00019010: 7465 6457 6974 6844 6963 744f 626a 6563  tedWithDictObjec
-00019020: 7473 293a 0a20 2020 2020 2020 2070 6173  ts):.        pas
-00019030: 730a 0a0a 636c 6173 7320 496e 6974 6961  s...class Initia
-00019040: 6c54 6573 7428 756e 6974 7465 7374 2e54  lTest(unittest.T
-00019050: 6573 7443 6173 6529 3a0a 2020 2020 6672  estCase):.    fr
-00019060: 6f6d 206c 6974 746c 6574 6162 6c65 2069  om littletable i
-00019070: 6d70 6f72 7420 280a 2020 2020 2020 2020  mport (.        
-00019080: 5f5f 7665 7273 696f 6e5f 5f20 6173 206c  __version__ as l
-00019090: 6974 746c 6574 6162 6c65 5f76 6572 7369  ittletable_versi
-000190a0: 6f6e 2c0a 2020 2020 2020 2020 5f5f 7665  on,.        __ve
-000190b0: 7273 696f 6e5f 7469 6d65 5f5f 2061 7320  rsion_time__ as 
-000190c0: 6c69 7474 6c65 7461 626c 655f 7665 7273  littletable_vers
-000190d0: 696f 6e5f 7469 6d65 2c0a 2020 2020 2020  ion_time,.      
-000190e0: 2020 5f5f 7665 7273 696f 6e5f 696e 666f    __version_info
-000190f0: 5f5f 2061 7320 6c69 7474 6c65 7461 626c  __ as littletabl
-00019100: 655f 7665 7273 696f 6e5f 696e 666f 2c0a  e_version_info,.
-00019110: 2020 2020 290a 0a20 2020 2070 7269 6e74      )..    print
-00019120: 280a 2020 2020 2020 2020 6622 4265 6769  (.        f"Begi
-00019130: 6e6e 696e 6720 7465 7374 206f 6620 6c69  nning test of li
-00019140: 7474 6c65 7461 626c 652c 2076 6572 7369  ttletable, versi
-00019150: 6f6e 207b 6c69 7474 6c65 7461 626c 655f  on {littletable_
-00019160: 7665 7273 696f 6e7d 2c20 7b6c 6974 746c  version}, {littl
-00019170: 6574 6162 6c65 5f76 6572 7369 6f6e 5f74  etable_version_t
-00019180: 696d 657d 222c 0a20 2020 2029 0a20 2020  ime}",.    ).   
-00019190: 2070 7269 6e74 286c 6974 746c 6574 6162   print(littletab
-000191a0: 6c65 5f76 6572 7369 6f6e 5f69 6e66 6f29  le_version_info)
-000191b0: 0a20 2020 2070 7269 6e74 2822 5079 7468  .    print("Pyth
-000191c0: 6f6e 2076 6572 7369 6f6e 222c 2073 7973  on version", sys
-000191d0: 2e76 6572 7369 6f6e 290a 2020 2020 7072  .version).    pr
-000191e0: 696e 7428 290a 0a0a 6966 205f 5f6e 616d  int()...if __nam
-000191f0: 655f 5f20 3d3d 2027 5f5f 6d61 696e 5f5f  e__ == '__main__
-00019200: 273a 0a0a 2020 2020 756e 6974 7465 7374  ':..    unittest
-00019210: 2e6d 6169 6e28 290a                      .main().
+00017d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d20: 2020 2020 2020 2020 2020 2020 206d 6174               mat
+00017d30: 6368 5f77 6f72 6473 2929 0a0a 2020 2020  ch_words))..    
+00017d40: 4061 6e6e 6f75 6e63 655f 7465 7374 0a20  @announce_test. 
+00017d50: 2020 2064 6566 2074 6573 745f 7365 6172     def test_sear
+00017d60: 6368 5f77 6974 685f 6c69 6d69 7428 7365  ch_with_limit(se
+00017d70: 6c66 293a 0a20 2020 2020 2020 2066 6f72  lf):.        for
+00017d80: 2071 7565 7279 2c20 6578 7065 6374 6564   query, expected
+00017d90: 2069 6e20 5b0a 2020 2020 2020 2020 2020   in [.          
+00017da0: 2020 2822 222c 205b 5d29 2c0a 2020 2020    ("", []),.    
+00017db0: 2020 2020 2020 2020 2822 7475 6e61 222c          ("tuna",
+00017dc0: 205b 312c 2036 5d29 2c0a 2020 2020 2020   [1, 6]),.      
+00017dd0: 2020 2020 2020 2822 7475 6e61 202b 6368        ("tuna +ch
+00017de0: 6565 7365 222c 205b 362c 2033 2c20 345d  eese", [6, 3, 4]
+00017df0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+00017e00: 2270 696e 6561 7070 6c65 202b 6261 636f  "pineapple +baco
+00017e10: 6e20 6c65 7474 7563 6520 6265 6566 202d  n lettuce beef -
+00017e20: 7361 7565 726b 7261 7574 2074 6f6d 6174  sauerkraut tomat
+00017e30: 6f22 2c20 5b39 2c20 3133 2c20 325d 292c  o", [9, 13, 2]),
+00017e40: 0a20 2020 2020 2020 2020 2020 2028 2270  .            ("p
+00017e50: 697a 7a61 2064 6f75 6768 202d 7069 6e65  izza dough -pine
+00017e60: 6170 706c 6522 2c20 5b33 2c20 342c 2032  apple", [3, 4, 2
+00017e70: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+00017e80: 2822 7069 7a7a 6120 646f 7567 6820 2d2d  ("pizza dough --
+00017e90: 7069 6e65 6170 706c 6522 2c20 5b33 2c20  pineapple", [3, 
+00017ea0: 345d 292c 0a20 2020 2020 2020 2020 2020  4]),.           
+00017eb0: 2028 2262 7265 6164 2062 6163 6f6e 222c   ("bread bacon",
+00017ec0: 205b 392c 2035 2c20 365d 292c 0a20 2020   [9, 5, 6]),.   
+00017ed0: 2020 2020 2020 2020 2028 2262 7265 6164           ("bread
+00017ee0: 202b 2b62 6163 6f6e 222c 205b 392c 2031   ++bacon", [9, 1
+00017ef0: 335d 292c 0a20 2020 2020 2020 2020 2020  3]),.           
+00017f00: 2028 2262 7265 6164 202b 2b61 6e63 686f   ("bread ++ancho
+00017f10: 7669 6573 222c 205b 5d29 2c0a 2020 2020  vies", []),.    
+00017f20: 2020 2020 2020 2020 2822 6272 6561 6420          ("bread 
+00017f30: 2b2b 6261 636f 6e20 2b2b 616e 6368 6f76  ++bacon ++anchov
+00017f40: 6965 7322 2c20 5b5d 292c 0a20 2020 2020  ies", []),.     
+00017f50: 2020 2020 2020 2028 2262 7265 6164 2062         ("bread b
+00017f60: 6163 6f6e 202d 2d61 6e63 686f 7669 6573  acon --anchovies
+00017f70: 222c 205b 392c 2035 2c20 365d 292c 0a20  ", [9, 5, 6]),. 
+00017f80: 2020 2020 2020 205d 3a0a 2020 2020 2020         ]:.      
+00017f90: 2020 2020 2020 6d61 7463 6865 7320 3d20        matches = 
+00017fa0: 7365 6c66 2e72 6563 6970 6573 2e73 6561  self.recipes.sea
+00017fb0: 7263 682e 696e 6772 6564 6965 6e74 7328  rch.ingredients(
+00017fc0: 7175 6572 792c 2061 735f 7461 626c 653d  query, as_table=
+00017fd0: 4661 6c73 652c 206d 696e 5f73 636f 7265  False, min_score
+00017fe0: 3d2d 3130 3030 302c 206c 696d 6974 3d33  =-10000, limit=3
+00017ff0: 290a 2020 2020 2020 2020 2020 2020 6d61  ).            ma
+00018000: 7463 685f 6964 7320 3d20 5b72 6563 6970  tch_ids = [recip
+00018010: 652e 6964 2066 6f72 2072 6563 6970 652c  e.id for recipe,
+00018020: 205f 2069 6e20 6d61 7463 6865 735d 0a20   _ in matches]. 
+00018030: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00018040: 2872 6570 7228 7175 6572 7929 2c20 272d  (repr(query), '-
+00018050: 3e27 2c20 5b28 7265 6369 7065 2e69 642c  >', [(recipe.id,
+00018060: 2073 636f 7265 2920 666f 7220 7265 6369   score) for reci
+00018070: 7065 2c20 7363 6f72 6520 696e 206d 6174  pe, score in mat
+00018080: 6368 6573 5d29 0a20 2020 2020 2020 2020  ches]).         
+00018090: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+000180a0: 5465 7374 2871 7565 7279 3d71 7565 7279  Test(query=query
+000180b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000180c0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000180d0: 7561 6c28 6578 7065 6374 6564 2c20 6d61  ual(expected, ma
+000180e0: 7463 685f 6964 732c 0a20 2020 2020 2020  tch_ids,.       
+000180f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018100: 2020 2020 2020 2020 2020 6622 696e 7661            f"inva
+00018110: 6c69 6420 7265 7375 6c74 7320 666f 7220  lid results for 
+00018120: 7175 6572 7920 7b71 7565 7279 2172 7d2c  query {query!r},
+00018130: 2065 7870 6563 7465 6420 7b65 7870 6563   expected {expec
+00018140: 7465 647d 2c20 676f 7420 7b6d 6174 6368  ted}, got {match
+00018150: 5f69 6473 7d22 290a 0a20 2020 2040 616e  _ids}")..    @an
+00018160: 6e6f 756e 6365 5f74 6573 740a 2020 2020  nounce_test.    
+00018170: 6465 6620 7465 7374 5f73 6561 7263 685f  def test_search_
+00018180: 7769 7468 5f6d 696e 5f73 636f 7265 2873  with_min_score(s
+00018190: 656c 6629 3a0a 2020 2020 2020 2020 666f  elf):.        fo
+000181a0: 7220 7175 6572 792c 2065 7870 6563 7465  r query, expecte
+000181b0: 6420 696e 205b 0a20 2020 2020 2020 2020  d in [.         
+000181c0: 2020 2028 2222 2c20 5b5d 292c 0a20 2020     ("", []),.   
+000181d0: 2020 2020 2020 2020 2028 2274 756e 6122           ("tuna"
+000181e0: 2c20 5b5d 292c 0a20 2020 2020 2020 2020  , []),.         
+000181f0: 2020 2028 2274 756e 6120 2b63 6865 6573     ("tuna +chees
+00018200: 6522 2c20 5b36 2c5d 292c 0a20 2020 2020  e", [6,]),.     
+00018210: 2020 2020 2020 2028 2270 696e 6561 7070         ("pineapp
+00018220: 6c65 202b 6261 636f 6e20 6c65 7474 7563  le +bacon lettuc
+00018230: 6520 6265 6566 202d 7361 7565 726b 7261  e beef -sauerkra
+00018240: 7574 2074 6f6d 6174 6f22 2c20 5b39 2c20  ut tomato", [9, 
+00018250: 3133 5d29 2c0a 2020 2020 2020 2020 2020  13]),.          
+00018260: 2020 2822 7069 7a7a 6120 646f 7567 6820    ("pizza dough 
+00018270: 2d70 696e 6561 7070 6c65 222c 205b 5d29  -pineapple", [])
+00018280: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
+00018290: 7069 7a7a 6120 646f 7567 6820 2d2d 7069  pizza dough --pi
+000182a0: 6e65 6170 706c 6522 2c20 5b5d 292c 0a20  neapple", []),. 
+000182b0: 2020 2020 2020 2020 2020 2028 2262 7265             ("bre
+000182c0: 6164 2062 6163 6f6e 222c 205b 5d29 2c0a  ad bacon", []),.
+000182d0: 2020 2020 2020 2020 2020 2020 2822 6272              ("br
+000182e0: 6561 6420 2b2b 6261 636f 6e22 2c20 5b39  ead ++bacon", [9
+000182f0: 2c5d 292c 0a20 2020 2020 2020 2020 2020  ,]),.           
+00018300: 2028 2262 7265 6164 202b 2b61 6e63 686f   ("bread ++ancho
+00018310: 7669 6573 222c 205b 5d29 2c0a 2020 2020  vies", []),.    
+00018320: 2020 2020 2020 2020 2822 6272 6561 6420          ("bread 
+00018330: 2b2b 6261 636f 6e20 2b2b 616e 6368 6f76  ++bacon ++anchov
+00018340: 6965 7322 2c20 5b5d 292c 0a20 2020 2020  ies", []),.     
+00018350: 2020 2020 2020 2028 2262 7265 6164 2062         ("bread b
+00018360: 6163 6f6e 202d 2d61 6e63 686f 7669 6573  acon --anchovies
+00018370: 222c 205b 5d29 2c0a 2020 2020 2020 2020  ", []),.        
+00018380: 5d3a 0a20 2020 2020 2020 2020 2020 206d  ]:.            m
+00018390: 6174 6368 6573 203d 2073 656c 662e 7265  atches = self.re
+000183a0: 6369 7065 732e 7365 6172 6368 2e69 6e67  cipes.search.ing
+000183b0: 7265 6469 656e 7473 2871 7565 7279 2c20  redients(query, 
+000183c0: 6173 5f74 6162 6c65 3d46 616c 7365 2c20  as_table=False, 
+000183d0: 6d69 6e5f 7363 6f72 653d 3130 3030 290a  min_score=1000).
+000183e0: 2020 2020 2020 2020 2020 2020 6d61 7463              matc
+000183f0: 685f 6964 7320 3d20 5b72 6563 6970 652e  h_ids = [recipe.
+00018400: 6964 2066 6f72 2072 6563 6970 652c 205f  id for recipe, _
+00018410: 2069 6e20 6d61 7463 6865 735d 0a20 2020   in matches].   
+00018420: 2020 2020 2020 2020 2070 7269 6e74 2872           print(r
+00018430: 6570 7228 7175 6572 7929 2c20 272d 3e27  epr(query), '->'
+00018440: 2c20 5b28 7265 6369 7065 2e69 642c 2073  , [(recipe.id, s
+00018450: 636f 7265 2920 666f 7220 7265 6369 7065  core) for recipe
+00018460: 2c20 7363 6f72 6520 696e 206d 6174 6368  , score in match
+00018470: 6573 5d29 0a20 2020 2020 2020 2020 2020  es]).           
+00018480: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+00018490: 7374 2871 7565 7279 3d71 7565 7279 293a  st(query=query):
+000184a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000184b0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000184c0: 6c28 6578 7065 6374 6564 2c20 6d61 7463  l(expected, matc
+000184d0: 685f 6964 732c 0a20 2020 2020 2020 2020  h_ids,.         
+000184e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000184f0: 2020 2020 2020 2020 6622 696e 7661 6c69          f"invali
+00018500: 6420 7265 7375 6c74 7320 666f 7220 7175  d results for qu
+00018510: 6572 7920 7b71 7565 7279 2172 7d2c 2065  ery {query!r}, e
+00018520: 7870 6563 7465 6420 7b65 7870 6563 7465  xpected {expecte
+00018530: 647d 2c20 676f 7420 7b6d 6174 6368 5f69  d}, got {match_i
+00018540: 6473 7d22 290a 0a20 2020 2040 616e 6e6f  ds}")..    @anno
+00018550: 756e 6365 5f74 6573 740a 2020 2020 6465  unce_test.    de
+00018560: 6620 7465 7374 5f73 6561 7263 685f 7769  f test_search_wi
+00018570: 7468 5f61 735f 7461 626c 6528 7365 6c66  th_as_table(self
+00018580: 293a 0a20 2020 2020 2020 2066 6f72 2071  ):.        for q
+00018590: 7565 7279 2c20 6578 7065 6374 6564 2069  uery, expected i
+000185a0: 6e20 5b0a 2020 2020 2020 2020 2020 2020  n [.            
+000185b0: 2822 222c 205b 5d29 2c0a 2020 2020 2020  ("", []),.      
+000185c0: 2020 2020 2020 2822 7475 6e61 222c 205b        ("tuna", [
+000185d0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+000185e0: 2822 7475 6e61 202b 6368 6565 7365 222c  ("tuna +cheese",
+000185f0: 205b 362c 5d29 2c0a 2020 2020 2020 2020   [6,]),.        
+00018600: 2020 2020 2822 7069 6e65 6170 706c 6520      ("pineapple 
+00018610: 2b62 6163 6f6e 206c 6574 7475 6365 2062  +bacon lettuce b
+00018620: 6565 6620 2d73 6175 6572 6b72 6175 7420  eef -sauerkraut 
+00018630: 746f 6d61 746f 222c 205b 392c 2031 335d  tomato", [9, 13]
+00018640: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+00018650: 2270 697a 7a61 2064 6f75 6768 202d 7069  "pizza dough -pi
+00018660: 6e65 6170 706c 6522 2c20 5b5d 292c 0a20  neapple", []),. 
+00018670: 2020 2020 2020 2020 2020 2028 2270 697a             ("piz
+00018680: 7a61 2064 6f75 6768 202d 2d70 696e 6561  za dough --pinea
+00018690: 7070 6c65 222c 205b 5d29 2c0a 2020 2020  pple", []),.    
+000186a0: 2020 2020 2020 2020 2822 6272 6561 6420          ("bread 
+000186b0: 6261 636f 6e22 2c20 5b5d 292c 0a20 2020  bacon", []),.   
+000186c0: 2020 2020 2020 2020 2028 2262 7265 6164           ("bread
+000186d0: 202b 2b62 6163 6f6e 222c 205b 392c 5d29   ++bacon", [9,])
+000186e0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
+000186f0: 6272 6561 6420 2b2b 616e 6368 6f76 6965  bread ++anchovie
+00018700: 7322 2c20 5b5d 292c 0a20 2020 2020 2020  s", []),.       
+00018710: 2020 2020 2028 2262 7265 6164 202b 2b62       ("bread ++b
+00018720: 6163 6f6e 202b 2b61 6e63 686f 7669 6573  acon ++anchovies
+00018730: 222c 205b 5d29 2c0a 2020 2020 2020 2020  ", []),.        
+00018740: 2020 2020 2822 6272 6561 6420 6261 636f      ("bread baco
+00018750: 6e20 2d2d 616e 6368 6f76 6965 7322 2c20  n --anchovies", 
+00018760: 5b5d 292c 0a20 2020 2020 2020 205d 3a0a  []),.        ]:.
+00018770: 2020 2020 2020 2020 2020 2020 6d61 7463              matc
+00018780: 6865 7320 3d20 7365 6c66 2e72 6563 6970  hes = self.recip
+00018790: 6573 2e73 6561 7263 682e 696e 6772 6564  es.search.ingred
+000187a0: 6965 6e74 7328 7175 6572 792c 206d 696e  ients(query, min
+000187b0: 5f73 636f 7265 3d31 3030 302c 2061 735f  _score=1000, as_
+000187c0: 7461 626c 653d 5472 7565 290a 2020 2020  table=True).    
+000187d0: 2020 2020 2020 2020 6d61 7463 685f 6964          match_id
+000187e0: 7320 3d20 5b72 6563 6970 652e 6964 2066  s = [recipe.id f
+000187f0: 6f72 2072 6563 6970 6520 696e 206d 6174  or recipe in mat
+00018800: 6368 6573 5d0a 2020 2020 2020 2020 2020  ches].          
+00018810: 2020 7072 696e 7428 7265 7072 2871 7565    print(repr(que
+00018820: 7279 292c 2027 2d3e 272c 205b 2872 6563  ry), '->', [(rec
+00018830: 6970 652e 6964 2c20 7265 6369 7065 2e69  ipe.id, recipe.i
+00018840: 6e67 7265 6469 656e 7473 5f73 6561 7263  ngredients_searc
+00018850: 685f 7363 6f72 6529 2066 6f72 2072 6563  h_score) for rec
+00018860: 6970 6520 696e 206d 6174 6368 6573 5d29  ipe in matches])
+00018870: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00018880: 6820 7365 6c66 2e73 7562 5465 7374 2871  h self.subTest(q
+00018890: 7565 7279 3d71 7565 7279 293a 0a20 2020  uery=query):.   
+000188a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000188b0: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
+000188c0: 7065 6374 6564 2c20 6d61 7463 685f 6964  pected, match_id
+000188d0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+000188e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188f0: 2020 2020 6622 696e 7661 6c69 6420 7265      f"invalid re
+00018900: 7375 6c74 7320 666f 7220 7175 6572 7920  sults for query 
+00018910: 7b71 7565 7279 2172 7d2c 2065 7870 6563  {query!r}, expec
+00018920: 7465 6420 7b65 7870 6563 7465 647d 2c20  ted {expected}, 
+00018930: 676f 7420 7b6d 6174 6368 5f69 6473 7d22  got {match_ids}"
+00018940: 290a 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00018950: 636f 7265 5f61 7474 7220 3d20 2269 6e67  core_attr = "ing
+00018960: 7265 6469 656e 7473 5f73 6561 7263 685f  redients_search_
+00018970: 7363 6f72 6522 0a20 2020 2020 2020 2020  score".         
+00018980: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+00018990: 7565 280a 2020 2020 2020 2020 2020 2020  ue(.            
+000189a0: 2020 2020 616c 6c28 0a20 2020 2020 2020      all(.       
+000189b0: 2020 2020 2020 2020 2020 2020 2068 6173               has
+000189c0: 6174 7472 286d 6174 6368 6573 2e62 792e  attr(matches.by.
+000189d0: 6964 5b6d 6964 5d2c 2073 636f 7265 5f61  id[mid], score_a
+000189e0: 7474 7229 0a20 2020 2020 2020 2020 2020  ttr).           
+000189f0: 2020 2020 2020 2020 2066 6f72 206d 6964           for mid
+00018a00: 2069 6e20 6d61 7463 685f 6964 730a 2020   in match_ids.  
+00018a10: 2020 2020 2020 2020 2020 2020 2020 292c                ),
+00018a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018a30: 2066 2261 735f 7461 626c 6520 6469 6420   f"as_table did 
+00018a40: 6e6f 7420 706f 7075 6c61 7465 2073 6f6d  not populate som
+00018a50: 6520 7365 6172 6368 2072 6563 6f72 6473  e search records
+00018a60: 2077 6974 6820 7b73 636f 7265 5f61 7474   with {score_att
+00018a70: 7221 727d 220a 2020 2020 2020 2020 2020  r!r}".          
+00018a80: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+00018a90: 2073 656c 662e 6173 7365 7274 4661 6c73   self.assertFals
+00018aa0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+00018ab0: 2020 2061 6e79 280a 2020 2020 2020 2020     any(.        
+00018ac0: 2020 2020 2020 2020 2020 2020 6861 7361              hasa
+00018ad0: 7474 7228 7365 6c66 2e72 6563 6970 6573  ttr(self.recipes
+00018ae0: 2e62 792e 6964 5b6d 6964 5d2c 2073 636f  .by.id[mid], sco
+00018af0: 7265 5f61 7474 7229 0a20 2020 2020 2020  re_attr).       
+00018b00: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00018b10: 206d 6964 2069 6e20 6d61 7463 685f 6964   mid in match_id
+00018b20: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00018b30: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+00018b40: 2020 2020 2066 2261 735f 7461 626c 6520       f"as_table 
+00018b50: 706f 7075 6c61 7465 6420 736f 6d65 206f  populated some o
+00018b60: 7269 6769 6e61 6c20 7265 636f 7264 7320  riginal records 
+00018b70: 7769 7468 207b 7363 6f72 655f 6174 7472  with {score_attr
+00018b80: 2172 7d22 0a20 2020 2020 2020 2020 2020  !r}".           
+00018b90: 2029 0a0a 636c 6173 7320 5461 626c 6553   )..class TableS
+00018ba0: 6561 7263 6854 6573 7473 5f44 6174 614f  earchTests_DataO
+00018bb0: 626a 6563 7473 2854 6162 6c65 5365 6172  bjects(TableSear
+00018bc0: 6368 5465 7374 732c 2055 7369 6e67 4461  chTests, UsingDa
+00018bd0: 7461 4f62 6a65 6374 7329 3a0a 2020 2020  taObjects):.    
+00018be0: 7061 7373 0a0a 636c 6173 7320 5461 626c  pass..class Tabl
+00018bf0: 6553 6561 7263 6854 6573 7473 5f4e 616d  eSearchTests_Nam
+00018c00: 6564 7475 706c 6573 2854 6162 6c65 5365  edtuples(TableSe
+00018c10: 6172 6368 5465 7374 732c 2055 7369 6e67  archTests, Using
+00018c20: 4e61 6d65 6474 7570 6c65 7329 3a0a 2020  Namedtuples):.  
+00018c30: 2020 7061 7373 0a0a 636c 6173 7320 5461    pass..class Ta
+00018c40: 626c 6553 6561 7263 6854 6573 7473 5f44  bleSearchTests_D
+00018c50: 6174 614e 616d 6564 7475 706c 6573 2854  ataNamedtuples(T
+00018c60: 6162 6c65 5365 6172 6368 5465 7374 732c  ableSearchTests,
+00018c70: 2055 7369 6e67 4461 7461 4e61 6d65 6474   UsingDataNamedt
+00018c80: 7570 6c65 7329 3a0a 2020 2020 7061 7373  uples):.    pass
+00018c90: 0a0a 636c 6173 7320 5461 626c 6553 6561  ..class TableSea
+00018ca0: 7263 6854 6573 7473 5f53 6c6f 7474 6564  rchTests_Slotted
+00018cb0: 2854 6162 6c65 5365 6172 6368 5465 7374  (TableSearchTest
+00018cc0: 732c 2055 7369 6e67 536c 6f74 7465 644f  s, UsingSlottedO
+00018cd0: 626a 6563 7473 293a 0a20 2020 2070 6173  bjects):.    pas
+00018ce0: 730a 0a63 6c61 7373 2054 6162 6c65 5365  s..class TableSe
+00018cf0: 6172 6368 5465 7374 735f 5369 6d70 6c65  archTests_Simple
+00018d00: 4e61 6d65 7370 6163 6528 5461 626c 6553  Namespace(TableS
+00018d10: 6561 7263 6854 6573 7473 2c20 5573 696e  earchTests, Usin
+00018d20: 6753 696d 706c 654e 616d 6573 7061 6365  gSimpleNamespace
+00018d30: 293a 0a20 2020 2070 6173 730a 0a69 6620  ):.    pass..if 
+00018d40: 6461 7461 636c 6173 7365 7320 6973 206e  dataclasses is n
+00018d50: 6f74 204e 6f6e 653a 0a20 2020 2063 6c61  ot None:.    cla
+00018d60: 7373 2054 6162 6c65 5365 6172 6368 5465  ss TableSearchTe
+00018d70: 7374 735f 4461 7461 636c 6173 7365 7328  sts_Dataclasses(
+00018d80: 5461 626c 6553 6561 7263 6854 6573 7473  TableSearchTests
+00018d90: 2c20 5573 696e 6744 6174 6163 6c61 7373  , UsingDataclass
+00018da0: 6573 293a 0a20 2020 2020 2020 2070 6173  es):.        pas
+00018db0: 730a 0a69 6620 7079 6461 6e74 6963 2069  s..if pydantic i
+00018dc0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00018dd0: 636c 6173 7320 5461 626c 6553 6561 7263  class TableSearc
+00018de0: 6854 6573 7473 5f50 7964 616e 7469 634d  hTests_PydanticM
+00018df0: 6f64 656c 7328 5461 626c 6553 6561 7263  odels(TableSearc
+00018e00: 6854 6573 7473 2c20 5573 696e 6750 7964  hTests, UsingPyd
+00018e10: 616e 7469 634d 6f64 656c 293a 0a20 2020  anticModel):.   
+00018e20: 2020 2020 2070 6173 730a 0a20 2020 2063       pass..    c
+00018e30: 6c61 7373 2054 6162 6c65 5365 6172 6368  lass TableSearch
+00018e40: 5465 7374 735f 5079 6461 6e74 6963 496d  Tests_PydanticIm
+00018e50: 6d75 7461 626c 654d 6f64 656c 7328 5461  mutableModels(Ta
+00018e60: 626c 6553 6561 7263 6854 6573 7473 2c20  bleSearchTests, 
+00018e70: 5573 696e 6750 7964 616e 7469 6349 6d6d  UsingPydanticImm
+00018e80: 7574 6162 6c65 4d6f 6465 6c29 3a0a 2020  utableModel):.  
+00018e90: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00018ea0: 636c 6173 7320 5461 626c 6553 6561 7263  class TableSearc
+00018eb0: 6854 6573 7473 5f50 7964 616e 7469 634f  hTests_PydanticO
+00018ec0: 524d 4d6f 6465 6c73 2854 6162 6c65 5365  RMModels(TableSe
+00018ed0: 6172 6368 5465 7374 732c 2055 7369 6e67  archTests, Using
+00018ee0: 5079 6461 6e74 6963 4f52 4d4d 6f64 656c  PydanticORMModel
+00018ef0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+00018f00: 0a69 6620 6174 7472 2069 7320 6e6f 7420  .if attr is not 
+00018f10: 4e6f 6e65 3a0a 2020 2020 636c 6173 7320  None:.    class 
+00018f20: 5461 626c 6553 6561 7263 6854 6573 7473  TableSearchTests
+00018f30: 5f41 7474 7243 6c61 7373 6573 2854 6162  _AttrClasses(Tab
+00018f40: 6c65 5365 6172 6368 5465 7374 732c 2055  leSearchTests, U
+00018f50: 7369 6e67 4174 7472 436c 6173 7329 3a0a  singAttrClass):.
+00018f60: 2020 2020 2020 2020 7061 7373 0a0a 6966          pass..if
+00018f70: 2074 7261 6974 6c65 7473 2069 7320 6e6f   traitlets is no
+00018f80: 7420 4e6f 6e65 3a0a 2020 2020 636c 6173  t None:.    clas
+00018f90: 7320 5461 626c 6553 6561 7263 6854 6573  s TableSearchTes
+00018fa0: 7473 5f54 7261 6974 6c65 7473 436c 6173  ts_TraitletsClas
+00018fb0: 7365 7328 5461 626c 6553 6561 7263 6854  ses(TableSearchT
+00018fc0: 6573 7473 2c20 5573 696e 6754 7261 6974  ests, UsingTrait
+00018fd0: 6c65 7473 436c 6173 7329 3a0a 2020 2020  letsClass):.    
+00018fe0: 2020 2020 7061 7373 0a0a 6966 2053 6c6f      pass..if Slo
+00018ff0: 7474 6564 5769 7468 4469 6374 2069 7320  ttedWithDict is 
+00019000: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 636c  not None:.    cl
+00019010: 6173 7320 5461 626c 6553 6561 7263 6854  ass TableSearchT
+00019020: 6573 7473 5f53 6c6f 7474 6564 5769 7468  ests_SlottedWith
+00019030: 4469 6374 2854 6162 6c65 5365 6172 6368  Dict(TableSearch
+00019040: 5465 7374 732c 2055 7369 6e67 536c 6f74  Tests, UsingSlot
+00019050: 7465 6457 6974 6844 6963 744f 626a 6563  tedWithDictObjec
+00019060: 7473 293a 0a20 2020 2020 2020 2070 6173  ts):.        pas
+00019070: 730a 0a0a 636c 6173 7320 496e 6974 6961  s...class Initia
+00019080: 6c54 6573 7428 756e 6974 7465 7374 2e54  lTest(unittest.T
+00019090: 6573 7443 6173 6529 3a0a 2020 2020 6672  estCase):.    fr
+000190a0: 6f6d 206c 6974 746c 6574 6162 6c65 2069  om littletable i
+000190b0: 6d70 6f72 7420 280a 2020 2020 2020 2020  mport (.        
+000190c0: 5f5f 7665 7273 696f 6e5f 5f20 6173 206c  __version__ as l
+000190d0: 6974 746c 6574 6162 6c65 5f76 6572 7369  ittletable_versi
+000190e0: 6f6e 2c0a 2020 2020 2020 2020 5f5f 7665  on,.        __ve
+000190f0: 7273 696f 6e5f 7469 6d65 5f5f 2061 7320  rsion_time__ as 
+00019100: 6c69 7474 6c65 7461 626c 655f 7665 7273  littletable_vers
+00019110: 696f 6e5f 7469 6d65 2c0a 2020 2020 2020  ion_time,.      
+00019120: 2020 5f5f 7665 7273 696f 6e5f 696e 666f    __version_info
+00019130: 5f5f 2061 7320 6c69 7474 6c65 7461 626c  __ as littletabl
+00019140: 655f 7665 7273 696f 6e5f 696e 666f 2c0a  e_version_info,.
+00019150: 2020 2020 290a 0a20 2020 2070 7269 6e74      )..    print
+00019160: 280a 2020 2020 2020 2020 6622 4265 6769  (.        f"Begi
+00019170: 6e6e 696e 6720 7465 7374 206f 6620 6c69  nning test of li
+00019180: 7474 6c65 7461 626c 652c 2076 6572 7369  ttletable, versi
+00019190: 6f6e 207b 6c69 7474 6c65 7461 626c 655f  on {littletable_
+000191a0: 7665 7273 696f 6e7d 2c20 7b6c 6974 746c  version}, {littl
+000191b0: 6574 6162 6c65 5f76 6572 7369 6f6e 5f74  etable_version_t
+000191c0: 696d 657d 222c 0a20 2020 2029 0a20 2020  ime}",.    ).   
+000191d0: 2070 7269 6e74 286c 6974 746c 6574 6162   print(littletab
+000191e0: 6c65 5f76 6572 7369 6f6e 5f69 6e66 6f29  le_version_info)
+000191f0: 0a20 2020 2070 7269 6e74 2822 5079 7468  .    print("Pyth
+00019200: 6f6e 2076 6572 7369 6f6e 222c 2073 7973  on version", sys
+00019210: 2e76 6572 7369 6f6e 290a 2020 2020 7072  .version).    pr
+00019220: 696e 7428 290a 0a0a 636c 6173 7320 5374  int()...class St
+00019230: 6f72 6167 6549 6e64 6570 656e 6465 6e74  orageIndependent
+00019240: 5465 7374 7328 756e 6974 7465 7374 2e54  Tests(unittest.T
+00019250: 6573 7443 6173 6529 3a0a 2020 2020 4061  estCase):.    @a
+00019260: 6e6e 6f75 6e63 655f 7465 7374 0a20 2020  nnounce_test.   
+00019270: 2064 6566 2074 6573 745f 6e6f 726d 616c   def test_normal
+00019280: 697a 655f 7374 7228 7365 6c66 293a 0a20  ize_str(self):. 
+00019290: 2020 2020 2020 2066 6f72 2069 6e5f 776f         for in_wo
+000192a0: 7264 2c20 6578 7065 6374 6564 5f77 6f72  rd, expected_wor
+000192b0: 6420 696e 205b 0a20 2020 2020 2020 2020  d in [.         
+000192c0: 2020 2028 226e 6f63 6861 6e67 6522 2c20     ("nochange", 
+000192d0: 226e 6f63 6861 6e67 6522 292c 0a20 2020  "nochange"),.   
+000192e0: 2020 2020 2020 2020 2028 2254 6f4c 6f77           ("ToLow
+000192f0: 6572 222c 2022 746f 6c6f 7765 7222 292c  er", "tolower"),
+00019300: 0a20 2020 2020 2020 2020 2020 2028 2249  .            ("I
+00019310: 2e42 2e4d 2e22 2c20 2269 626d 2229 2c0a  .B.M.", "ibm"),.
+00019320: 2020 2020 2020 2020 2020 2020 2822 472e              ("G.
+00019330: 452e 222c 2022 6765 2229 2c0a 2020 2020  E.", "ge"),.    
+00019340: 2020 2020 2020 2020 2822 4d2e 222c 2022          ("M.", "
+00019350: 6d22 292c 0a20 2020 2020 2020 2020 2020  m"),.           
+00019360: 2028 224d 2e78 797a 222c 2022 6d22 292c   ("M.xyz", "m"),
+00019370: 0a20 2020 2020 2020 2020 2020 2028 222a  .            ("*
+00019380: 7878 782d 6868 6822 2c20 2278 7878 2d68  xxx-hhh", "xxx-h
+00019390: 6868 2229 2c0a 2020 2020 2020 2020 2020  hh"),.          
+000193a0: 2020 2822 2b62 6c61 6846 6f6f 222c 2022    ("+blahFoo", "
+000193b0: 626c 6168 666f 6f22 292c 0a20 2020 2020  blahfoo"),.     
+000193c0: 2020 2020 2020 2023 2028 2266 6f78 6573         # ("foxes
+000193d0: 222c 2022 666f 7822 292c 0a20 2020 2020  ", "fox"),.     
+000193e0: 2020 2020 2020 2023 2028 2263 6875 7263         # ("churc
+000193f0: 6865 7322 2c20 2263 6875 7263 6822 292c  hes", "church"),
+00019400: 0a20 2020 2020 2020 2020 2020 2023 2028  .            # (
+00019410: 2264 7265 7373 6573 222c 2022 6472 6573  "dresses", "dres
+00019420: 7322 292c 0a20 2020 2020 2020 205d 3a0a  s"),.        ]:.
+00019430: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00019440: 2073 656c 662e 7375 6254 6573 7428 696e   self.subTest(in
+00019450: 5f77 6f72 6429 3a0a 2020 2020 2020 2020  _word):.        
+00019460: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00019470: 6572 7445 7175 616c 2865 7870 6563 7465  ertEqual(expecte
+00019480: 645f 776f 7264 2c20 6c74 2e54 6162 6c65  d_word, lt.Table
+00019490: 2e5f 6e6f 726d 616c 697a 655f 776f 7264  ._normalize_word
+000194a0: 2869 6e5f 776f 7264 2929 0a0a 2020 2020  (in_word))..    
+000194b0: 6465 6620 7465 7374 5f6e 6f72 6d61 6c69  def test_normali
+000194c0: 7a65 5f73 7472 5f67 656e 2873 656c 6629  ze_str_gen(self)
+000194d0: 3a0a 2020 2020 2020 2020 666f 7220 696e  :.        for in
+000194e0: 5f77 6f72 642c 2065 7870 6563 7465 645f  _word, expected_
+000194f0: 776f 7264 7320 696e 205b 0a20 2020 2020  words in [.     
+00019500: 2020 2020 2020 2028 226e 6f63 6861 6e67         ("nochang
+00019510: 6522 2c20 5b22 6e6f 6368 616e 6765 225d  e", ["nochange"]
+00019520: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+00019530: 2254 6f4c 6f77 6572 222c 205b 2274 6f6c  "ToLower", ["tol
+00019540: 6f77 6572 225d 292c 0a20 2020 2020 2020  ower"]),.       
+00019550: 2020 2020 2028 2249 2e42 2e4d 2e22 2c20       ("I.B.M.", 
+00019560: 5b22 692e 622e 6d2e 222c 2022 6962 6d22  ["i.b.m.", "ibm"
+00019570: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+00019580: 2822 472e 452e 222c 205b 2267 2e65 2e22  ("G.E.", ["g.e."
+00019590: 2c20 2267 6522 5d29 2c0a 2020 2020 2020  , "ge"]),.      
+000195a0: 2020 2020 2020 2822 412e 492e 222c 205b        ("A.I.", [
+000195b0: 2261 2e69 2e22 2c20 2261 6922 5d29 2c0a  "a.i.", "ai"]),.
+000195c0: 2020 2020 2020 2020 2020 2020 2822 4149              ("AI
+000195d0: 222c 205b 2261 6922 5d29 2c0a 2020 2020  ", ["ai"]),.    
+000195e0: 2020 2020 2020 2020 2822 4d2e 222c 205b          ("M.", [
+000195f0: 226d 222c 2022 6d2e 225d 292c 0a20 2020  "m", "m."]),.   
+00019600: 2020 2020 2020 2020 2028 226d 2e78 797a           ("m.xyz
+00019610: 222c 205b 226d 222c 2022 6d2e 7879 7a22  ", ["m", "m.xyz"
+00019620: 2c20 2278 797a 225d 292c 0a20 2020 2020  , "xyz"]),.     
+00019630: 2020 2020 2020 2028 224d 2e78 797a 222c         ("M.xyz",
+00019640: 205b 226d 2e78 797a 222c 2022 7879 7a22   ["m.xyz", "xyz"
+00019650: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+00019660: 2822 5468 7265 6164 696e 672e 6973 416c  ("Threading.isAl
+00019670: 6976 6528 2922 2c20 5b27 6973 616c 6976  ive()", ['isaliv
+00019680: 6527 2c20 2774 6872 6561 6469 6e67 272c  e', 'threading',
+00019690: 2027 7468 7265 6164 696e 672e 6973 616c   'threading.isal
+000196a0: 6976 6527 5d29 2c0a 2020 2020 2020 2020  ive']),.        
+000196b0: 2020 2020 2822 2a78 7878 2d68 6868 222c      ("*xxx-hhh",
+000196c0: 205b 2768 6868 272c 2027 7878 7827 2c20   ['hhh', 'xxx', 
+000196d0: 2778 7878 2d68 6868 275d 292c 0a20 2020  'xxx-hhh']),.   
+000196e0: 2020 2020 2020 2020 2028 222b 626c 6168           ("+blah
+000196f0: 466f 6f22 2c20 5b22 626c 6168 666f 6f22  Foo", ["blahfoo"
+00019700: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+00019710: 2822 7374 722e 6c73 7472 6970 222c 205b  ("str.lstrip", [
+00019720: 226c 7374 7269 7022 2c20 2273 7472 222c  "lstrip", "str",
+00019730: 2022 7374 722e 6c73 7472 6970 225d 292c   "str.lstrip"]),
+00019740: 0a20 2020 2020 2020 2020 2020 2028 2273  .            ("s
+00019750: 7472 2e6c 7374 7269 7028 2922 2c20 5b22  tr.lstrip()", ["
+00019760: 6c73 7472 6970 222c 2022 7374 7222 2c20  lstrip", "str", 
+00019770: 2273 7472 2e6c 7374 7269 7022 5d29 2c0a  "str.lstrip"]),.
+00019780: 2020 2020 2020 2020 2020 2020 2822 7365              ("se
+00019790: 6c66 2e61 7373 6572 7445 7175 616c 7322  lf.assertEquals"
+000197a0: 2c20 5b22 6173 7365 7274 6571 7561 6c73  , ["assertequals
+000197b0: 222c 2022 7365 6c66 222c 2022 7365 6c66  ", "self", "self
+000197c0: 2e61 7373 6572 7465 7175 616c 7322 5d29  .assertequals"])
+000197d0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
+000197e0: 5465 7374 4361 7365 2e61 7373 6572 7445  TestCase.assertE
+000197f0: 7175 616c 7322 2c20 5b22 6173 7365 7274  quals", ["assert
+00019800: 6571 7561 6c73 222c 2022 7465 7374 6361  equals", "testca
+00019810: 7365 222c 2022 7465 7374 6361 7365 2e61  se", "testcase.a
+00019820: 7373 6572 7465 7175 616c 7322 5d29 2c0a  ssertequals"]),.
+00019830: 2020 2020 2020 2020 2020 2020 2822 756e              ("un
+00019840: 6974 7465 7374 2e54 6573 7443 6173 652e  ittest.TestCase.
+00019850: 6173 7365 7274 4571 7561 6c73 222c 0a20  assertEquals",. 
+00019860: 2020 2020 2020 2020 2020 2020 5b22 6173              ["as
+00019870: 7365 7274 6571 7561 6c73 222c 2022 7465  sertequals", "te
+00019880: 7374 6361 7365 222c 2022 756e 6974 7465  stcase", "unitte
+00019890: 7374 222c 2022 756e 6974 7465 7374 2e74  st", "unittest.t
+000198a0: 6573 7463 6173 652e 6173 7365 7274 6571  estcase.asserteq
+000198b0: 7561 6c73 225d 292c 0a20 2020 2020 2020  uals"]),.       
+000198c0: 2020 2020 2028 2266 6f78 6573 222c 205b       ("foxes", [
+000198d0: 2266 6f78 222c 2022 666f 7865 7322 5d29  "fox", "foxes"])
+000198e0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
+000198f0: 6368 7572 6368 6573 222c 205b 2263 6875  churches", ["chu
+00019900: 7263 6822 2c20 2263 6875 7263 6865 7322  rch", "churches"
+00019910: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+00019920: 2822 6472 6573 7365 7322 2c20 5b22 6472  ("dresses", ["dr
+00019930: 6573 7322 2c20 2264 7265 7373 6573 225d  ess", "dresses"]
+00019940: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+00019950: 2264 7265 7373 222c 205b 2264 7265 7373  "dress", ["dress
+00019960: 222c 205d 292c 0a20 2020 2020 2020 2020  ", ]),.         
+00019970: 2020 2028 2262 6961 7322 2c20 5b22 6269     ("bias", ["bi
+00019980: 6173 222c 205d 292c 0a20 2020 2020 2020  as", ]),.       
+00019990: 2020 2020 2028 2274 6f79 7322 2c20 5b22       ("toys", ["
+000199a0: 746f 7922 2c20 2274 6f79 7322 5d29 2c0a  toy", "toys"]),.
+000199b0: 2020 2020 2020 2020 2020 2020 2822 6261              ("ba
+000199c0: 6269 6573 222c 205b 2262 6162 6965 7322  bies", ["babies"
+000199d0: 2c20 2262 6162 7922 5d29 2c0a 2020 2020  , "baby"]),.    
+000199e0: 2020 2020 2020 2020 2822 6164 6465 6e64          ("addend
+000199f0: 6122 2c20 5b22 6164 6465 6e64 6122 2c20  a", ["addenda", 
+00019a00: 2261 6464 656e 6475 6d22 5d29 2c0a 2020  "addendum"]),.  
+00019a10: 2020 2020 2020 2020 2020 2822 7261 6269            ("rabi
+00019a20: 6573 222c 205b 2272 6162 6965 7322 5d29  es", ["rabies"])
+00019a30: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
+00019a40: 6c61 7a69 6e65 7373 222c 205b 226c 617a  laziness", ["laz
+00019a50: 696e 6573 7322 5d29 2c0a 2020 2020 2020  iness"]),.      
+00019a60: 2020 2020 2020 2822 7068 7973 6963 7322        ("physics"
+00019a70: 2c20 5b22 7068 7973 6963 7322 5d29 2c0a  , ["physics"]),.
+00019a80: 2020 2020 2020 2020 2020 2020 2822 5079              ("Py
+00019a90: 7468 6f6e 2773 222c 205b 2270 7974 686f  thon's", ["pytho
+00019aa0: 6e22 5d29 2c0a 2020 2020 2020 2020 5d3a  n"]),.        ]:
+00019ab0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00019ac0: 6820 7365 6c66 2e73 7562 5465 7374 2869  h self.subTest(i
+00019ad0: 6e5f 776f 7264 293a 0a20 2020 2020 2020  n_word):.       
+00019ae0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00019af0: 7365 7274 4571 7561 6c28 6578 7065 6374  sertEqual(expect
+00019b00: 6564 5f77 6f72 6473 2c0a 2020 2020 2020  ed_words,.      
+00019b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b20: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
+00019b30: 6428 6c69 7374 286c 742e 5461 626c 652e  d(list(lt.Table.
+00019b40: 5f6e 6f72 6d61 6c69 7a65 5f77 6f72 645f  _normalize_word_
+00019b50: 6765 6e28 696e 5f77 6f72 6429 2929 290a  gen(in_word)))).
+00019b60: 0a20 2020 2040 616e 6e6f 756e 6365 5f74  .    @announce_t
+00019b70: 6573 740a 2020 2020 6465 6620 7465 7374  est.    def test
+00019b80: 5f6e 6f72 6d61 6c69 7a65 5f73 706c 6974  _normalize_split
+00019b90: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00019ba0: 666f 7220 696e 5f73 7472 2c20 6578 7065  for in_str, expe
+00019bb0: 6374 6564 5f73 7472 5f73 6574 2069 6e20  cted_str_set in 
+00019bc0: 5b0a 2020 2020 2020 2020 2020 2020 2822  [.            ("
+00019bd0: 7374 722e 6c73 7472 6970 2829 222c 205b  str.lstrip()", [
+00019be0: 226c 7374 7269 7022 2c20 2273 7472 222c  "lstrip", "str",
+00019bf0: 2022 7374 722e 6c73 7472 6970 225d 292c   "str.lstrip"]),
+00019c00: 0a20 2020 2020 2020 2020 2020 2028 2273  .            ("s
+00019c10: 7472 2e6c 7374 7269 7028 2920 7374 722e  tr.lstrip() str.
+00019c20: 7273 7472 6970 2829 222c 205b 226c 7374  rstrip()", ["lst
+00019c30: 7269 7022 2c20 2272 7374 7269 7022 2c20  rip", "rstrip", 
+00019c40: 2273 7472 222c 2022 7374 722e 6c73 7472  "str", "str.lstr
+00019c50: 6970 222c 2022 7374 722e 7273 7472 6970  ip", "str.rstrip
+00019c60: 225d 292c 0a20 2020 2020 2020 2020 2020  "]),.           
+00019c70: 2023 2028 2222 2c20 5b5d 292c 0a20 2020   # ("", []),.   
+00019c80: 2020 2020 2020 2020 2023 2028 2222 2c20           # ("", 
+00019c90: 5b5d 292c 0a20 2020 2020 2020 2020 2020  []),.           
+00019ca0: 2023 2028 2222 2c20 5b5d 292c 0a20 2020   # ("", []),.   
+00019cb0: 2020 2020 205d 3a0a 2020 2020 2020 2020       ]:.        
+00019cc0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+00019cd0: 6254 6573 7428 696e 5f73 7472 293a 0a20  bTest(in_str):. 
+00019ce0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019cf0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00019d00: 6578 7065 6374 6564 5f73 7472 5f73 6574  expected_str_set
+00019d10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00019d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d30: 2020 2073 6f72 7465 6428 7365 7428 6c74     sorted(set(lt
+00019d40: 2e54 6162 6c65 2e5f 6e6f 726d 616c 697a  .Table._normaliz
+00019d50: 655f 7370 6c69 7428 696e 5f73 7472 2929  e_split(in_str))
+00019d60: 2929 0a0a 0a69 6620 5f5f 6e61 6d65 5f5f  ))...if __name__
+00019d70: 203d 3d20 275f 5f6d 6169 6e5f 5f27 3a0a   == '__main__':.
+00019d80: 0a20 2020 2075 6e69 7474 6573 742e 6d61  .    unittest.ma
+00019d90: 696e 2829 0a                             in().
```

