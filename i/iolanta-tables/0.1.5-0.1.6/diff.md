# Comparing `tmp/iolanta_tables-0.1.5.tar.gz` & `tmp/iolanta_tables-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iolanta_tables-0.1.5.tar", max compression
+gzip compressed data, was "iolanta_tables-0.1.6.tar", max compression
```

## Comparing `iolanta_tables-0.1.5.tar` & `iolanta_tables-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0       18 2023-02-11 19:52:34.300405 iolanta_tables-0.1.5/README.md
--rw-r--r--   0        0        0       48 2023-02-11 20:05:39.844838 iolanta_tables-0.1.5/iolanta_tables/__init__.py
--rw-r--r--   0        0        0      691 2023-03-05 09:23:42.346754 iolanta_tables-0.1.5/iolanta_tables/data/context.yaml
--rw-r--r--   0        0        0     3211 2023-04-25 14:59:20.183870 iolanta_tables-0.1.5/iolanta_tables/data/iolanta-tables.yaml
--rw-r--r--   0        0        0        0 2023-02-12 10:28:34.764205 iolanta_tables-0.1.5/iolanta_tables/facets/__init__.py
--rw-r--r--   0        0        0        0 2023-02-11 20:58:23.763324 iolanta_tables-0.1.5/iolanta_tables/facets/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-02-11 20:58:45.467496 iolanta_tables-0.1.5/iolanta_tables/facets/csv/__init__.py
--rw-r--r--   0        0        0      279 2023-02-12 10:28:34.744205 iolanta_tables-0.1.5/iolanta_tables/facets/html/__init__.py
--rw-r--r--   0        0        0     3506 2023-04-25 15:11:09.275971 iolanta_tables-0.1.5/iolanta_tables/facets/html/base.py
--rw-r--r--   0        0        0     1341 2023-04-25 14:59:20.183870 iolanta_tables-0.1.5/iolanta_tables/facets/html/body_class.py
--rw-r--r--   0        0        0     1297 2023-04-25 14:59:20.183870 iolanta_tables-0.1.5/iolanta_tables/facets/html/body_rows.py
--rw-r--r--   0        0        0      665 2023-02-11 20:03:08.695985 iolanta_tables-0.1.5/iolanta_tables/facets/html/errors.py
--rw-r--r--   0        0        0     1227 2023-04-03 17:34:11.170056 iolanta_tables-0.1.5/iolanta_tables/facets/html/header.py
--rw-r--r--   0        0        0      477 2023-02-11 20:08:32.117810 iolanta_tables-0.1.5/iolanta_tables/facets/html/models.py
--rw-r--r--   0        0        0      162 2023-02-11 20:03:08.695985 iolanta_tables-0.1.5/iolanta_tables/facets/html/queries.py
--rw-r--r--   0        0        0     1854 2023-02-11 20:10:49.701422 iolanta_tables-0.1.5/iolanta_tables/facets/html/row.py
--rw-r--r--   0        0        0      858 2023-03-04 17:03:47.999569 iolanta_tables-0.1.5/iolanta_tables/facets/html/self.py
--rw-r--r--   0        0        0      153 2023-01-22 07:56:04.628617 iolanta_tables-0.1.5/iolanta_tables/facets/html/sparql/column_list_by_row_list.sparql
--rw-r--r--   0        0        0      239 2023-04-01 12:57:42.462631 iolanta_tables-0.1.5/iolanta_tables/facets/html/sparql/columns.sparql
--rw-r--r--   0        0        0       68 2023-01-16 16:45:28.154620 iolanta_tables-0.1.5/iolanta_tables/facets/html/sparql/columns_list.sparql
--rw-r--r--   0        0        0       60 2023-01-21 14:26:14.887559 iolanta_tables-0.1.5/iolanta_tables/facets/html/sparql/instance_class.sparql
--rw-r--r--   0        0        0       78 2023-01-21 14:15:53.187926 iolanta_tables-0.1.5/iolanta_tables/facets/html/sparql/instances-class.sparql
--rw-r--r--   0        0        0      513 2023-01-22 15:03:52.693068 iolanta_tables-0.1.5/iolanta_tables/facets/html/sparql/order-by.sparql
--rw-r--r--   0        0        0       47 2023-01-17 18:49:02.284586 iolanta_tables-0.1.5/iolanta_tables/facets/html/sparql/table_rows.sparql
--rw-r--r--   0        0        0       61 2023-01-15 18:53:42.263646 iolanta_tables-0.1.5/iolanta_tables/facets/html/sparql/tr.sparql
--rw-r--r--   0        0        0     5434 2023-03-04 17:05:30.196165 iolanta_tables-0.1.5/iolanta_tables/facets/html/table.py
--rw-r--r--   0        0        0        0 2023-02-11 20:58:53.471559 iolanta_tables-0.1.5/iolanta_tables/facets/json/__init__.py
--rw-r--r--   0        0        0        0 2023-02-11 20:58:32.603394 iolanta_tables-0.1.5/iolanta_tables/facets/tex/__init__.py
--rw-r--r--   0        0        0     1093 2023-04-03 17:38:30.490692 iolanta_tables-0.1.5/iolanta_tables/models.py
--rw-r--r--   0        0        0      102 2023-02-11 20:03:58.312265 iolanta_tables-0.1.5/iolanta_tables/plugin.py
--rw-r--r--   0        0        0      611 2023-04-25 15:12:23.056384 iolanta_tables-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1046 1970-01-01 00:00:00.000000 iolanta_tables-0.1.5/setup.py
--rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 iolanta_tables-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       18 2023-02-11 19:52:34.300405 iolanta_tables-0.1.6/README.md
+-rw-r--r--   0        0        0       48 2023-02-11 20:05:39.844838 iolanta_tables-0.1.6/iolanta_tables/__init__.py
+-rw-r--r--   0        0        0      691 2023-03-05 09:23:42.346754 iolanta_tables-0.1.6/iolanta_tables/data/context.yaml
+-rw-r--r--   0        0        0     3211 2023-04-25 14:59:20.183870 iolanta_tables-0.1.6/iolanta_tables/data/iolanta-tables.yaml
+-rw-r--r--   0        0        0        0 2023-02-12 10:28:34.764205 iolanta_tables-0.1.6/iolanta_tables/facets/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-11 20:58:23.763324 iolanta_tables-0.1.6/iolanta_tables/facets/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-11 20:58:45.467496 iolanta_tables-0.1.6/iolanta_tables/facets/csv/__init__.py
+-rw-r--r--   0        0        0      279 2023-02-12 10:28:34.744205 iolanta_tables-0.1.6/iolanta_tables/facets/html/__init__.py
+-rw-r--r--   0        0        0     3506 2023-04-25 15:11:09.275971 iolanta_tables-0.1.6/iolanta_tables/facets/html/base.py
+-rw-r--r--   0        0        0     1341 2023-04-25 14:59:20.183870 iolanta_tables-0.1.6/iolanta_tables/facets/html/body_class.py
+-rw-r--r--   0        0        0     1297 2023-04-25 14:59:20.183870 iolanta_tables-0.1.6/iolanta_tables/facets/html/body_rows.py
+-rw-r--r--   0        0        0      665 2023-02-11 20:03:08.695985 iolanta_tables-0.1.6/iolanta_tables/facets/html/errors.py
+-rw-r--r--   0        0        0     1227 2023-04-03 17:34:11.170056 iolanta_tables-0.1.6/iolanta_tables/facets/html/header.py
+-rw-r--r--   0        0        0      477 2023-02-11 20:08:32.117810 iolanta_tables-0.1.6/iolanta_tables/facets/html/models.py
+-rw-r--r--   0        0        0      162 2023-02-11 20:03:08.695985 iolanta_tables-0.1.6/iolanta_tables/facets/html/queries.py
+-rw-r--r--   0        0        0     1864 2023-04-30 14:02:48.799756 iolanta_tables-0.1.6/iolanta_tables/facets/html/row.py
+-rw-r--r--   0        0        0      858 2023-03-04 17:03:47.999569 iolanta_tables-0.1.6/iolanta_tables/facets/html/self.py
+-rw-r--r--   0        0        0      153 2023-01-22 07:56:04.628617 iolanta_tables-0.1.6/iolanta_tables/facets/html/sparql/column_list_by_row_list.sparql
+-rw-r--r--   0        0        0      239 2023-04-01 12:57:42.462631 iolanta_tables-0.1.6/iolanta_tables/facets/html/sparql/columns.sparql
+-rw-r--r--   0        0        0       68 2023-01-16 16:45:28.154620 iolanta_tables-0.1.6/iolanta_tables/facets/html/sparql/columns_list.sparql
+-rw-r--r--   0        0        0       60 2023-01-21 14:26:14.887559 iolanta_tables-0.1.6/iolanta_tables/facets/html/sparql/instance_class.sparql
+-rw-r--r--   0        0        0       78 2023-01-21 14:15:53.187926 iolanta_tables-0.1.6/iolanta_tables/facets/html/sparql/instances-class.sparql
+-rw-r--r--   0        0        0      513 2023-01-22 15:03:52.693068 iolanta_tables-0.1.6/iolanta_tables/facets/html/sparql/order-by.sparql
+-rw-r--r--   0        0        0       47 2023-01-17 18:49:02.284586 iolanta_tables-0.1.6/iolanta_tables/facets/html/sparql/table_rows.sparql
+-rw-r--r--   0        0        0       61 2023-01-15 18:53:42.263646 iolanta_tables-0.1.6/iolanta_tables/facets/html/sparql/tr.sparql
+-rw-r--r--   0        0        0     4919 2023-04-30 14:02:23.883592 iolanta_tables-0.1.6/iolanta_tables/facets/html/table.py
+-rw-r--r--   0        0        0        0 2023-02-11 20:58:53.471559 iolanta_tables-0.1.6/iolanta_tables/facets/json/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-11 20:58:32.603394 iolanta_tables-0.1.6/iolanta_tables/facets/tex/__init__.py
+-rw-r--r--   0        0        0     1093 2023-04-03 17:38:30.490692 iolanta_tables-0.1.6/iolanta_tables/models.py
+-rw-r--r--   0        0        0      102 2023-02-11 20:03:58.312265 iolanta_tables-0.1.6/iolanta_tables/plugin.py
+-rw-r--r--   0        0        0      611 2023-04-30 14:18:24.505506 iolanta_tables-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1046 1970-01-01 00:00:00.000000 iolanta_tables-0.1.6/setup.py
+-rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 iolanta_tables-0.1.6/PKG-INFO
```

### Comparing `iolanta_tables-0.1.5/iolanta_tables/data/context.yaml` & `iolanta_tables-0.1.6/iolanta_tables/data/context.yaml`

 * *Files identical despite different names*

### Comparing `iolanta_tables-0.1.5/iolanta_tables/data/iolanta-tables.yaml` & `iolanta_tables-0.1.6/iolanta_tables/data/iolanta-tables.yaml`

 * *Files identical despite different names*

### Comparing `iolanta_tables-0.1.5/iolanta_tables/facets/html/base.py` & `iolanta_tables-0.1.6/iolanta_tables/facets/html/base.py`

 * *Files identical despite different names*

### Comparing `iolanta_tables-0.1.5/iolanta_tables/facets/html/body_class.py` & `iolanta_tables-0.1.6/iolanta_tables/facets/html/body_class.py`

 * *Files identical despite different names*

### Comparing `iolanta_tables-0.1.5/iolanta_tables/facets/html/body_rows.py` & `iolanta_tables-0.1.6/iolanta_tables/facets/html/body_rows.py`

 * *Files identical despite different names*

### Comparing `iolanta_tables-0.1.5/iolanta_tables/facets/html/errors.py` & `iolanta_tables-0.1.6/iolanta_tables/facets/html/errors.py`

 * *Files identical despite different names*

### Comparing `iolanta_tables-0.1.5/iolanta_tables/facets/html/header.py` & `iolanta_tables-0.1.6/iolanta_tables/facets/html/header.py`

 * *Files identical despite different names*

### Comparing `iolanta_tables-0.1.5/iolanta_tables/facets/html/row.py` & `iolanta_tables-0.1.6/iolanta_tables/facets/html/row.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,14 @@
             row_value_by_column.get(column) for column in columns
         ]
 
         cells = [
             td(
                 self.render(
                     cell_value,
-                    environments=[IOLANTA.html],
+                    environments=[TABLE.td, IOLANTA.html],
                 ),
             ) if cell_value is not None else td()
             for cell_value in maybe_cell_values
         ]
 
         return tr(*cells)
```

### Comparing `iolanta_tables-0.1.5/iolanta_tables/facets/html/self.py` & `iolanta_tables-0.1.6/iolanta_tables/facets/html/self.py`

 * *Files identical despite different names*

### Comparing `iolanta_tables-0.1.5/iolanta_tables/facets/html/sparql/order-by.sparql` & `iolanta_tables-0.1.6/iolanta_tables/facets/html/sparql/order-by.sparql`

 * *Files identical despite different names*

### Comparing `iolanta_tables-0.1.5/iolanta_tables/facets/html/table.py` & `iolanta_tables-0.1.6/iolanta_tables/facets/html/table.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,36 +83,14 @@
         cell['column']: instance if (
             cell['column'] == TABLE.self
         ) else cell['value']
         for cell in cells
     }
 
 
-def render_row(
-    row: Row,
-    columns: List[URIRef],
-    iolanta: Iolanta,
-) -> Iterable[td]:
-    """Compile a sequence of table cells for a row."""
-    for column in columns:
-        try:
-            cell_value = row[column]
-        except KeyError:
-            yield td()
-            continue
-
-        cell_content = str(
-            iolanta.render(
-                node=cell_value,
-                environments=[column, TABLE.td, IOLANTA.html],
-            ),
-        )
-        yield td(raw(cell_content))
-
-
 def construct_sorter(order_by: List[Tuple[URIRef, bool]]):
     """Construct a sorting procedure for rows in a table."""
     def sorter(row: Row):   # noqa: WPS430
         return [
             row.get(order_field, None)    # FIXME descending?
             for order_field, is_ascending in order_by
         ]
```

### Comparing `iolanta_tables-0.1.5/iolanta_tables/models.py` & `iolanta_tables-0.1.6/iolanta_tables/models.py`

 * *Files identical despite different names*

### Comparing `iolanta_tables-0.1.5/pyproject.toml` & `iolanta_tables-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iolanta-tables"
-version = "0.1.5"
+version = "0.1.6"
 description = "Linked Data as tables"
 authors = ["Anatoly Scherbakov <altaisoft@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "iolanta_tables"}]
 
 [tool.poetry.dependencies]
```

### Comparing `iolanta_tables-0.1.5/setup.py` & `iolanta_tables-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ['dominate>=2.7.0,<3.0.0', 'iolanta>=1.0.11,<2.0.0']
 
 entry_points = \
 {'iolanta.plugins': ['tables = iolanta_tables:IolantaTables']}
 
 setup_kwargs = {
     'name': 'iolanta-tables',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Linked Data as tables',
     'long_description': '# iolanta-tables\n\n',
     'author': 'Anatoly Scherbakov',
     'author_email': 'altaisoft@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `iolanta_tables-0.1.5/PKG-INFO` & `iolanta_tables-0.1.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iolanta-tables
-Version: 0.1.5
+Version: 0.1.6
 Summary: Linked Data as tables
 License: MIT
 Author: Anatoly Scherbakov
 Author-email: altaisoft@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

