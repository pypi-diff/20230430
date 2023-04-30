# Comparing `tmp/pymwp-0.4.0.tar.gz` & `tmp/pymwp-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymwp-0.4.0.tar", last modified: Sat Apr 29 20:56:47 2023, max compression
+gzip compressed data, was "pymwp-0.4.1.tar", last modified: Sun Apr 30 04:52:45 2023, max compression
```

## Comparing `pymwp-0.4.0.tar` & `pymwp-0.4.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:56:47.449555 pymwp-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-29 20:56:19.000000 pymwp-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-29 20:56:19.000000 pymwp-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-29 20:56:47.449555 pymwp-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-29 20:56:19.000000 pymwp-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:56:47.445554 pymwp-0.4.0/pymwp/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18891 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/bound.py
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/delta_graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/monomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/polynomial.py
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/relation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/semiring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:56:47.449555 pymwp-0.4.0/pymwp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-29 20:56:47.000000 pymwp-0.4.0/pymwp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-29 20:56:47.000000 pymwp-0.4.0/pymwp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 20:56:47.000000 pymwp-0.4.0/pymwp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-29 20:56:47.000000 pymwp-0.4.0/pymwp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-29 20:56:47.000000 pymwp-0.4.0/pymwp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 20:56:47.000000 pymwp-0.4.0/pymwp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-29 20:56:19.000000 pymwp-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 20:56:47.449555 pymwp-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-29 20:56:19.000000 pymwp-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:56:47.449555 pymwp-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:56:47.449555 pymwp-0.4.0/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/mocks/ast_mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_delta_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_monomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_polynomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_relation_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:52:45.978363 pymwp-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-30 04:52:13.000000 pymwp-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-30 04:52:13.000000 pymwp-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-04-30 04:52:45.978363 pymwp-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-30 04:52:13.000000 pymwp-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:52:45.974363 pymwp-0.4.1/pymwp/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18891 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/delta_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/monomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/relation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/semiring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:52:45.974363 pymwp-0.4.1/pymwp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-04-30 04:52:45.000000 pymwp-0.4.1/pymwp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-30 04:52:45.000000 pymwp-0.4.1/pymwp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 04:52:45.000000 pymwp-0.4.1/pymwp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-30 04:52:45.000000 pymwp-0.4.1/pymwp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-30 04:52:45.000000 pymwp-0.4.1/pymwp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 04:52:45.000000 pymwp-0.4.1/pymwp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-30 04:52:13.000000 pymwp-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 04:52:45.978363 pymwp-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-30 04:52:13.000000 pymwp-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:52:45.978363 pymwp-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:52:45.978363 pymwp-0.4.1/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/mocks/ast_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_delta_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_monomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_relation_list.py
```

### Comparing `pymwp-0.4.0/LICENSE` & `pymwp-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/PKG-INFO` & `pymwp-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymwp
-Version: 0.4.0
+Version: 0.4.1
 Summary: Implementation of MWP analysis on C code in Python.
 Home-page: https://github.com/statycc/pymwp
 Author: Clément Aubert, Thomas Rubiano, Neea Rusch, Thomas Seiller
 Author-email: nrusch@augusta.edu
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/statycc/pymwp/issues
 Project-URL: Documentation, https://statycc.github.io/pymwp/
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Typing :: Typed
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pymwp: MWP analysis in Python
 
 [![build](https://github.com/statycc/pymwp/actions/workflows/build.yaml/badge.svg)](https://github.com/statycc/pymwp/actions/workflows/build.yaml)
```

### Comparing `pymwp-0.4.0/README.md` & `pymwp-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/pymwp/__init__.py` & `pymwp-0.4.1/pymwp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 pymwp: implementation of MWP analysis on C code in Python.
 """
 
 __title__ = "pymwp"
 __author__ = "Clément Aubert, Thomas Rubiano, Neea Rusch, Thomas Seiller"
 __license__ = "GPLv3"
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 from pymwp.parser import Parser
 from pymwp.delta_graphs import DeltaGraph
 from pymwp.choice import Choices
 from pymwp.monomial import Monomial
 from pymwp.polynomial import Polynomial
 from pymwp.relation_list import RelationList
```

### Comparing `pymwp-0.4.0/pymwp/__main__.py` & `pymwp-0.4.1/pymwp/__main__.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/pymwp/analysis.py` & `pymwp-0.4.1/pymwp/analysis.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/pymwp/bound.py` & `pymwp-0.4.1/pymwp/bound.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/pymwp/choice.py` & `pymwp-0.4.1/pymwp/choice.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/pymwp/delta_graphs.py` & `pymwp-0.4.1/pymwp/delta_graphs.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/pymwp/file_io.py` & `pymwp-0.4.1/pymwp/file_io.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/pymwp/matrix.py` & `pymwp-0.4.1/pymwp/matrix.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/pymwp/monomial.py` & `pymwp-0.4.1/pymwp/monomial.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/pymwp/parser.py` & `pymwp-0.4.1/pymwp/parser.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/pymwp/polynomial.py` & `pymwp-0.4.1/pymwp/polynomial.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/pymwp/relation.py` & `pymwp-0.4.1/pymwp/relation.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/pymwp/relation_list.py` & `pymwp-0.4.1/pymwp/relation_list.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/pymwp/result.py` & `pymwp-0.4.1/pymwp/result.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/pymwp/semiring.py` & `pymwp-0.4.1/pymwp/semiring.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/pymwp.egg-info/PKG-INFO` & `pymwp-0.4.1/pymwp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymwp
-Version: 0.4.0
+Version: 0.4.1
 Summary: Implementation of MWP analysis on C code in Python.
 Home-page: https://github.com/statycc/pymwp
 Author: Clément Aubert, Thomas Rubiano, Neea Rusch, Thomas Seiller
 Author-email: nrusch@augusta.edu
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/statycc/pymwp/issues
 Project-URL: Documentation, https://statycc.github.io/pymwp/
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Typing :: Typed
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pymwp: MWP analysis in Python
 
 [![build](https://github.com/statycc/pymwp/actions/workflows/build.yaml/badge.svg)](https://github.com/statycc/pymwp/actions/workflows/build.yaml)
```

### Comparing `pymwp-0.4.0/pymwp.egg-info/SOURCES.txt` & `pymwp-0.4.1/pymwp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/setup.py` & `pymwp-0.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 __title__ = "pymwp"
 __author__ = "Clément Aubert, Thomas Rubiano, Neea Rusch, Thomas Seiller"
 __desc__ = "Implementation of MWP analysis on C code in Python."
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name=__title__,
     version=__version__,
@@ -38,14 +38,15 @@
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Operating System :: OS Independent',
         'Environment :: Console',
         'Typing :: Typed',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
+        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)'
     ],
     python_requires=">=3.7",
     install_requires=[
         'pycparser',
         'pycparser-fake-libc'
     ]
 )
```

### Comparing `pymwp-0.4.0/tests/mocks/ast_mocks.py` & `pymwp-0.4.1/tests/mocks/ast_mocks.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/tests/test_analysis.py` & `pymwp-0.4.1/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/tests/test_bound.py` & `pymwp-0.4.1/tests/test_bound.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/tests/test_choices.py` & `pymwp-0.4.1/tests/test_choices.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/tests/test_compare.py` & `pymwp-0.4.1/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/tests/test_delta_graph.py` & `pymwp-0.4.1/tests/test_delta_graph.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/tests/test_file_io.py` & `pymwp-0.4.1/tests/test_file_io.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/tests/test_matrix.py` & `pymwp-0.4.1/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/tests/test_monomial.py` & `pymwp-0.4.1/tests/test_monomial.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/tests/test_parser.py` & `pymwp-0.4.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/tests/test_polynomial.py` & `pymwp-0.4.1/tests/test_polynomial.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/tests/test_relation.py` & `pymwp-0.4.1/tests/test_relation.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.0/tests/test_relation_list.py` & `pymwp-0.4.1/tests/test_relation_list.py`

 * *Files identical despite different names*

