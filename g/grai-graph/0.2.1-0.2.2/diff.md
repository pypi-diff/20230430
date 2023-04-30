# Comparing `tmp/grai_graph-0.2.1.tar.gz` & `tmp/grai_graph-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_graph-0.2.1.tar", max compression
+gzip compressed data, was "grai_graph-0.2.2.tar", max compression
```

## Comparing `grai_graph-0.2.1.tar` & `grai_graph-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      758 2023-03-30 13:07:01.120507 grai_graph-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       82 2023-02-14 12:06:39.086773 grai_graph-0.2.1/src/grai_graph/__init__.py
--rw-r--r--   0        0        0     7981 2023-03-30 13:02:21.405404 grai_graph-0.2.1/src/grai_graph/analysis.py
--rw-r--r--   0        0        0      357 2023-02-14 12:06:39.086918 grai_graph-0.2.1/src/grai_graph/client_monkeypatch.py
--rw-r--r--   0        0        0     4123 2023-02-14 12:06:39.086995 grai_graph-0.2.1/src/grai_graph/graph.py
--rw-r--r--   0        0        0     3375 2023-02-14 12:06:39.087066 grai_graph-0.2.1/src/grai_graph/utils.py
--rw-r--r--   0        0        0     2480 2023-02-14 12:06:39.087143 grai_graph-0.2.1/src/grai_graph/visualizations.py
--rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 grai_graph-0.2.1/setup.py
--rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 grai_graph-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      211 2023-04-29 00:58:02.888617 grai_graph-0.2.2/README.md
+-rw-r--r--   0        0        0      928 2023-04-30 17:36:11.765828 grai_graph-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-02-13 20:16:22.709007 grai_graph-0.2.2/src/grai_graph/__init__.py
+-rw-r--r--   0        0        0     7981 2023-03-30 16:50:54.361721 grai_graph-0.2.2/src/grai_graph/analysis.py
+-rw-r--r--   0        0        0      357 2023-02-13 20:16:22.709765 grai_graph-0.2.2/src/grai_graph/client_monkeypatch.py
+-rw-r--r--   0        0        0     4123 2023-02-13 20:16:22.710062 grai_graph-0.2.2/src/grai_graph/graph.py
+-rw-r--r--   0        0        0     3375 2023-02-13 20:16:22.710145 grai_graph-0.2.2/src/grai_graph/utils.py
+-rw-r--r--   0        0        0     2480 2023-02-13 20:16:22.710278 grai_graph-0.2.2/src/grai_graph/visualizations.py
+-rw-r--r--   0        0        0     1083 1970-01-01 00:00:00.000000 grai_graph-0.2.2/setup.py
+-rw-r--r--   0        0        0     1182 1970-01-01 00:00:00.000000 grai_graph-0.2.2/PKG-INFO
```

### Comparing `grai_graph-0.2.1/pyproject.toml` & `grai_graph-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 [tool.poetry]
 name = "grai-graph"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
+readme = "README.md"
+homepage = "https://www.grai.io/"
+repository = "https://github.com/grai-io/grai-core/tree/master/grai-graph"
+documentation = "https://docs.grai.io/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 networkx = "^2.8.5"
 pydantic = "^1.9.1"
 grai-client = "^0.2.0"
 matplotlib = {version = "^3.5.2", optional = true}
```

### Comparing `grai_graph-0.2.1/src/grai_graph/analysis.py` & `grai_graph-0.2.2/src/grai_graph/analysis.py`

 * *Files identical despite different names*

### Comparing `grai_graph-0.2.1/src/grai_graph/graph.py` & `grai_graph-0.2.2/src/grai_graph/graph.py`

 * *Files identical despite different names*

### Comparing `grai_graph-0.2.1/src/grai_graph/utils.py` & `grai_graph-0.2.2/src/grai_graph/utils.py`

 * *Files identical despite different names*

### Comparing `grai_graph-0.2.1/src/grai_graph/visualizations.py` & `grai_graph-0.2.2/src/grai_graph/visualizations.py`

 * *Files identical despite different names*

### Comparing `grai_graph-0.2.1/setup.py` & `grai_graph-0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,22 +17,22 @@
  'pydantic>=1.9.1,<2.0.0']
 
 extras_require = \
 {'vis': ['matplotlib>=3.5.2,<4.0.0', 'pydot>=1.4.2,<2.0.0']}
 
 setup_kwargs = {
     'name': 'grai-graph',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': '',
-    'long_description': 'None',
+    'long_description': '# Grai Graph\n\nThis project provides a variety of utilities for exploring your Grai data lineage graph including support\nfor counter factual tests to determine the impact of a data change on your infrastructure.\n',
     'author': 'Ian Eaves',
     'author_email': 'ian@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://www.grai.io/',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'python_requires': '>=3.8,<4.0',
 }
```

