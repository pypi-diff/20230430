# Comparing `tmp/grai_source_postgres-0.1.8.tar.gz` & `tmp/grai_source_postgres-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_postgres-0.1.8.tar", max compression
+gzip compressed data, was "grai_source_postgres-0.1.9.tar", max compression
```

## Comparing `grai_source_postgres-0.1.8.tar` & `grai_source_postgres-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      706 2023-01-27 10:18:19.658270 grai_source_postgres-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      145 2023-01-23 19:51:17.814721 grai_source_postgres-0.1.8/src/grai_source_postgres/__init__.py
--rw-r--r--   0        0        0     5861 2023-01-27 10:18:34.374981 grai_source_postgres-0.1.8/src/grai_source_postgres/adapters.py
--rw-r--r--   0        0        0     1150 2023-01-27 08:54:46.067365 grai_source_postgres-0.1.8/src/grai_source_postgres/base.py
--rw-r--r--   0        0        0     7185 2023-01-11 10:42:34.274803 grai_source_postgres-0.1.8/src/grai_source_postgres/loader.py
--rw-r--r--   0        0        0     4144 2022-12-07 15:33:50.248250 grai_source_postgres-0.1.8/src/grai_source_postgres/models.py
--rw-r--r--   0        0        0      148 2023-01-23 19:51:17.815063 grai_source_postgres-0.1.8/src/grai_source_postgres/package_definitions.py
--rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 grai_source_postgres-0.1.8/setup.py
--rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 grai_source_postgres-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      706 2023-01-27 12:50:31.332417 grai_source_postgres-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-01-23 19:51:17.814721 grai_source_postgres-0.1.9/src/grai_source_postgres/__init__.py
+-rw-r--r--   0        0        0     5861 2023-01-27 11:11:33.559126 grai_source_postgres-0.1.9/src/grai_source_postgres/adapters.py
+-rw-r--r--   0        0        0     1171 2023-01-27 12:45:33.465685 grai_source_postgres-0.1.9/src/grai_source_postgres/base.py
+-rw-r--r--   0        0        0     7185 2023-01-11 10:42:34.274803 grai_source_postgres-0.1.9/src/grai_source_postgres/loader.py
+-rw-r--r--   0        0        0     4144 2022-12-07 15:33:50.248250 grai_source_postgres-0.1.9/src/grai_source_postgres/models.py
+-rw-r--r--   0        0        0      148 2023-01-23 19:51:17.815063 grai_source_postgres-0.1.9/src/grai_source_postgres/package_definitions.py
+-rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 grai_source_postgres-0.1.9/setup.py
+-rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 grai_source_postgres-0.1.9/PKG-INFO
```

### Comparing `grai_source_postgres-0.1.8/pyproject.toml` & `grai_source_postgres-0.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_postgres"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_postgres", from = "src" },
 ]
 [tool.poetry.dependencies]
```

### Comparing `grai_source_postgres-0.1.8/src/grai_source_postgres/adapters.py` & `grai_source_postgres-0.1.9/src/grai_source_postgres/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_postgres-0.1.8/src/grai_source_postgres/base.py` & `grai_source_postgres-0.1.9/src/grai_source_postgres/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,12 +27,12 @@
     user: Optional[str] = None,
     password: Optional[str] = None,
     host: Optional[str] = None,
     port: Optional[str] = None,
 ):
 
     conn = PostgresConnector(
-        dbname=dbname, user=user, password=password, host=host, port=port
+        dbname=dbname, user=user, password=password, host=host, port=port, namespace=namespace
     )
     nodes, edges = get_nodes_and_edges(conn, client.id)
     update(client, nodes)
     update(client, edges)
```

### Comparing `grai_source_postgres-0.1.8/src/grai_source_postgres/loader.py` & `grai_source_postgres-0.1.9/src/grai_source_postgres/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_postgres-0.1.8/src/grai_source_postgres/models.py` & `grai_source_postgres-0.1.9/src/grai_source_postgres/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_postgres-0.1.8/setup.py` & `grai_source_postgres-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'grai-schemas>=0.1.5,<0.2.0',
  'multimethod>=1.8,<2.0',
  'psycopg2>=2.9.5,<3.0.0',
  'pydantic>=1.9.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'grai-source-postgres',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': 'None',
     'author': 'Ian Eaves',
     'author_email': 'ian@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `grai_source_postgres-0.1.8/PKG-INFO` & `grai_source_postgres-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-postgres
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

