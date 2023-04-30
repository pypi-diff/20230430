# Comparing `tmp/grai_source_mysql-0.0.8.tar.gz` & `tmp/grai_source_mysql-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_mysql-0.0.8.tar", max compression
+gzip compressed data, was "grai_source_mysql-0.0.9.tar", max compression
```

## Comparing `grai_source_mysql-0.0.8.tar` & `grai_source_mysql-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      720 2023-03-22 03:31:10.823144 grai_source_mysql-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      139 2023-02-13 20:16:22.725826 grai_source_mysql-0.0.8/src/grai_source_mysql/__init__.py
--rw-r--r--   0        0        0     6109 2023-03-22 03:28:01.338626 grai_source_mysql-0.0.8/src/grai_source_mysql/adapters.py
--rw-r--r--   0        0        0     1054 2023-02-13 20:16:22.726027 grai_source_mysql-0.0.8/src/grai_source_mysql/base.py
--rw-r--r--   0        0        0     7576 2023-03-22 03:28:46.659513 grai_source_mysql-0.0.8/src/grai_source_mysql/loader.py
--rw-r--r--   0        0        0     4089 2023-03-22 03:28:01.339116 grai_source_mysql-0.0.8/src/grai_source_mysql/models.py
--rw-r--r--   0        0        0      180 2023-02-13 20:16:22.726524 grai_source_mysql-0.0.8/src/grai_source_mysql/package_definitions.py
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 grai_source_mysql-0.0.8/setup.py
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 grai_source_mysql-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      720 2023-03-22 04:18:10.608905 grai_source_mysql-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-02-13 20:16:22.725826 grai_source_mysql-0.0.9/src/grai_source_mysql/__init__.py
+-rw-r--r--   0        0        0     6109 2023-03-22 03:28:01.338626 grai_source_mysql-0.0.9/src/grai_source_mysql/adapters.py
+-rw-r--r--   0        0        0     1054 2023-02-13 20:16:22.726027 grai_source_mysql-0.0.9/src/grai_source_mysql/base.py
+-rw-r--r--   0        0        0     7687 2023-03-22 04:13:27.979101 grai_source_mysql-0.0.9/src/grai_source_mysql/loader.py
+-rw-r--r--   0        0        0     4089 2023-03-22 03:28:01.339116 grai_source_mysql-0.0.9/src/grai_source_mysql/models.py
+-rw-r--r--   0        0        0      180 2023-02-13 20:16:22.726524 grai_source_mysql-0.0.9/src/grai_source_mysql/package_definitions.py
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 grai_source_mysql-0.0.9/setup.py
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 grai_source_mysql-0.0.9/PKG-INFO
```

### Comparing `grai_source_mysql-0.0.8/pyproject.toml` & `grai_source_mysql-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_mysql"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["Tony Lewis <tony@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_mysql", from = "src" },
 ]
 [tool.poetry.dependencies]
```

### Comparing `grai_source_mysql-0.0.8/src/grai_source_mysql/adapters.py` & `grai_source_mysql-0.0.9/src/grai_source_mysql/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_mysql-0.0.8/src/grai_source_mysql/base.py` & `grai_source_mysql-0.0.9/src/grai_source_mysql/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_mysql-0.0.8/src/grai_source_mysql/loader.py` & `grai_source_mysql-0.0.9/src/grai_source_mysql/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,18 @@
 	    SELECT table_schema, table_name
             FROM information_schema.tables
             WHERE table_schema != 'information_schema'
 		    AND table_schema != 'performance_schema'
             ORDER BY table_schema, table_name
         """
         res = ({k.lower(): v for k, v in result.items()} for result in self.query_runner(query))
-        return [Table(**result, namespace=self.namespace) for result in res]
+        tables = [Table(**result, namespace=self.namespace) for result in res]
+        for table in tables:
+            table.columns = self.get_table_columns(table)
+        return tables
 
     @cached_property
     def columns(self) -> List[Column]:
         """
         Creates and returns a list of dictionaries for the specified
         schema.table in the database connected to.
         """
```

### Comparing `grai_source_mysql-0.0.8/src/grai_source_mysql/models.py` & `grai_source_mysql-0.0.9/src/grai_source_mysql/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_mysql-0.0.8/setup.py` & `grai_source_mysql-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'grai-schemas>=0.1.10,<0.2.0',
  'multimethod>=1.8,<2.0',
  'mysql-connector-python>=8.0.31,<9.0.0',
  'pydantic>=1.9.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'grai-source-mysql',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': '',
     'long_description': 'None',
     'author': 'Tony Lewis',
     'author_email': 'tony@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `grai_source_mysql-0.0.8/PKG-INFO` & `grai_source_mysql-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-mysql
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 License: Elastic-2.0
 Author: Tony Lewis
 Author-email: tony@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

