# Comparing `tmp/grai_source_mssql-0.0.8.tar.gz` & `tmp/grai_source_mssql-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_mssql-0.0.8.tar", max compression
+gzip compressed data, was "grai_source_mssql-0.0.9.tar", max compression
```

## Comparing `grai_source_mssql-0.0.8.tar` & `grai_source_mssql-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      685 2023-04-26 17:55:43.262699 grai_source_mssql-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      139 2023-02-13 20:16:22.722173 grai_source_mssql-0.0.8/src/grai_source_mssql/__init__.py
--rw-r--r--   0        0        0     6461 2023-04-26 17:55:43.262901 grai_source_mssql-0.0.8/src/grai_source_mssql/adapters.py
--rw-r--r--   0        0        0     1302 2023-02-13 20:16:22.722839 grai_source_mssql-0.0.8/src/grai_source_mssql/base.py
--rw-r--r--   0        0        0    10658 2023-02-14 16:39:18.548229 grai_source_mssql-0.0.8/src/grai_source_mssql/loader.py
--rw-r--r--   0        0        0     4298 2023-02-14 16:39:18.548342 grai_source_mssql-0.0.8/src/grai_source_mssql/models.py
--rw-r--r--   0        0        0      180 2023-02-13 20:16:22.723121 grai_source_mssql-0.0.8/src/grai_source_mssql/package_definitions.py
--rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 grai_source_mssql-0.0.8/setup.py
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 grai_source_mssql-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      145 2023-04-29 00:58:02.883807 grai_source_mssql-0.0.9/README.md
+-rw-r--r--   0        0        0      876 2023-04-30 17:37:24.495159 grai_source_mssql-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-02-13 20:16:22.722173 grai_source_mssql-0.0.9/src/grai_source_mssql/__init__.py
+-rw-r--r--   0        0        0     6461 2023-04-29 00:19:10.367254 grai_source_mssql-0.0.9/src/grai_source_mssql/adapters.py
+-rw-r--r--   0        0        0     1302 2023-02-13 20:16:22.722839 grai_source_mssql-0.0.9/src/grai_source_mssql/base.py
+-rw-r--r--   0        0        0    10658 2023-02-14 16:39:18.548229 grai_source_mssql-0.0.9/src/grai_source_mssql/loader.py
+-rw-r--r--   0        0        0     4298 2023-02-14 16:39:18.548342 grai_source_mssql-0.0.9/src/grai_source_mssql/models.py
+-rw-r--r--   0        0        0      180 2023-02-13 20:16:22.723121 grai_source_mssql-0.0.9/src/grai_source_mssql/package_definitions.py
+-rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 grai_source_mssql-0.0.9/setup.py
+-rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 grai_source_mssql-0.0.9/PKG-INFO
```

### Comparing `grai_source_mssql-0.0.8/pyproject.toml` & `grai_source_mssql-0.0.9/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 [tool.poetry]
 name = "grai_source_mssql"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_mssql", from = "src" },
 ]
+readme = "README.md"
+homepage = "https://www.grai.io/"
+repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-mssql"
+documentation = "https://docs.grai.io/"
+
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
 grai-client = "^0.2.0"
 multimethod = "^1.8"
 grai-schemas = "^0.1.8"
 pyodbc = "^4.0.35"
```

### Comparing `grai_source_mssql-0.0.8/src/grai_source_mssql/adapters.py` & `grai_source_mssql-0.0.9/src/grai_source_mssql/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_mssql-0.0.8/src/grai_source_mssql/base.py` & `grai_source_mssql-0.0.9/src/grai_source_mssql/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_mssql-0.0.8/src/grai_source_mssql/loader.py` & `grai_source_mssql-0.0.9/src/grai_source_mssql/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_mssql-0.0.8/src/grai_source_mssql/models.py` & `grai_source_mssql-0.0.9/src/grai_source_mssql/models.py`

 * *Files identical despite different names*

