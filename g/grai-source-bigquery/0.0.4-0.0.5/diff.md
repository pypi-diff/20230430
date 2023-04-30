# Comparing `tmp/grai_source_bigquery-0.0.4.tar.gz` & `tmp/grai_source_bigquery-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_bigquery-0.0.4.tar", max compression
+gzip compressed data, was "grai_source_bigquery-0.0.5.tar", max compression
```

## Comparing `grai_source_bigquery-0.0.4.tar` & `grai_source_bigquery-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      738 2023-04-26 17:55:43.260206 grai_source_bigquery-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      145 2023-02-13 20:16:22.712224 grai_source_bigquery-0.0.4/src/grai_source_bigquery/__init__.py
--rw-r--r--   0        0        0     6659 2023-04-26 17:55:43.260599 grai_source_bigquery-0.0.4/src/grai_source_bigquery/adapters.py
--rw-r--r--   0        0        0     1192 2023-02-13 20:16:22.712633 grai_source_bigquery-0.0.4/src/grai_source_bigquery/base.py
--rw-r--r--   0        0        0     5547 2023-02-13 20:16:22.712831 grai_source_bigquery-0.0.4/src/grai_source_bigquery/loader.py
--rw-r--r--   0        0        0     4778 2023-04-13 22:32:27.123660 grai_source_bigquery-0.0.4/src/grai_source_bigquery/models.py
--rw-r--r--   0        0        0      186 2023-02-13 20:16:22.713174 grai_source_bigquery-0.0.4/src/grai_source_bigquery/package_definitions.py
--rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 grai_source_bigquery-0.0.4/setup.py
--rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 grai_source_bigquery-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-04-29 00:58:02.889530 grai_source_bigquery-0.0.5/README.md
+-rw-r--r--   0        0        0      932 2023-04-30 17:36:37.985912 grai_source_bigquery-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-02-13 20:16:22.712224 grai_source_bigquery-0.0.5/src/grai_source_bigquery/__init__.py
+-rw-r--r--   0        0        0     6659 2023-04-29 00:19:10.365235 grai_source_bigquery-0.0.5/src/grai_source_bigquery/adapters.py
+-rw-r--r--   0        0        0     1192 2023-02-13 20:16:22.712633 grai_source_bigquery-0.0.5/src/grai_source_bigquery/base.py
+-rw-r--r--   0        0        0     5547 2023-02-13 20:16:22.712831 grai_source_bigquery-0.0.5/src/grai_source_bigquery/loader.py
+-rw-r--r--   0        0        0     4778 2023-04-13 22:32:27.123660 grai_source_bigquery-0.0.5/src/grai_source_bigquery/models.py
+-rw-r--r--   0        0        0      186 2023-02-13 20:16:22.713174 grai_source_bigquery-0.0.5/src/grai_source_bigquery/package_definitions.py
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 grai_source_bigquery-0.0.5/setup.py
+-rw-r--r--   0        0        0     1114 1970-01-01 00:00:00.000000 grai_source_bigquery-0.0.5/PKG-INFO
```

### Comparing `grai_source_bigquery-0.0.4/pyproject.toml` & `grai_source_bigquery-0.0.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 [tool.poetry]
 name = "grai_source_bigquery"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_bigquery", from = "src" },
 ]
+readme = "README.md"
+homepage = "https://www.grai.io/"
+repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-bigquery"
+documentation = "https://docs.grai.io/"
+
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
 grai-client = "^0.2.0"
 multimethod = "^1.8"
 grai-schemas = "^0.1.9"
 google-cloud-bigquery = "^3.5.0"
```

### Comparing `grai_source_bigquery-0.0.4/src/grai_source_bigquery/adapters.py` & `grai_source_bigquery-0.0.5/src/grai_source_bigquery/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.0.4/src/grai_source_bigquery/base.py` & `grai_source_bigquery-0.0.5/src/grai_source_bigquery/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.0.4/src/grai_source_bigquery/loader.py` & `grai_source_bigquery-0.0.5/src/grai_source_bigquery/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.0.4/src/grai_source_bigquery/models.py` & `grai_source_bigquery-0.0.5/src/grai_source_bigquery/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.0.4/setup.py` & `grai_source_bigquery-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,22 +16,22 @@
  'grai-schemas>=0.1.9,<0.2.0',
  'multimethod>=1.8,<2.0',
  'pydantic>=1.9.1,<2.0.0',
  'setuptools>=67.1.0,<68.0.0']
 
 setup_kwargs = {
     'name': 'grai-source-bigquery',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': '',
-    'long_description': 'None',
+    'long_description': '# Grai BigQuery Integration\n\nThe BigQuery integration synchronizes metadata from a BigQuery datawarehouse into your Grai data lineage graph.\n',
     'author': 'Edward Louth',
     'author_email': 'edward@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://www.grai.io/',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

