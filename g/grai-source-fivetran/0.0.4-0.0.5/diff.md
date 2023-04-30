# Comparing `tmp/grai_source_fivetran-0.0.4.tar.gz` & `tmp/grai_source_fivetran-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_fivetran-0.0.4.tar", max compression
+gzip compressed data, was "grai_source_fivetran-0.0.5.tar", max compression
```

## Comparing `grai_source_fivetran-0.0.4.tar` & `grai_source_fivetran-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      879 2023-04-26 17:55:43.261436 grai_source_fivetran-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      119 2023-02-14 16:39:18.542655 grai_source_fivetran-0.0.4/src/grai_source_fivetran/__init__.py
--rw-r--r--   0        0        0     6644 2023-04-26 17:55:43.261675 grai_source_fivetran-0.0.4/src/grai_source_fivetran/adapters.py
--rw-r--r--   0        0        0     1425 2023-02-14 16:39:18.543003 grai_source_fivetran-0.0.4/src/grai_source_fivetran/base.py
--rw-r--r--   0        0        0        0 2023-02-14 16:39:18.543040 grai_source_fivetran-0.0.4/src/grai_source_fivetran/fivetran_api/__init__.py
--rw-r--r--   0        0        0   436632 2023-02-14 16:39:18.545031 grai_source_fivetran-0.0.4/src/grai_source_fivetran/fivetran_api/api_models.py
--rw-r--r--   0        0        0    42232 2023-02-14 16:39:18.545359 grai_source_fivetran-0.0.4/src/grai_source_fivetran/fivetran_api/main.py
--rw-r--r--   0        0        0    12057 2023-02-14 16:39:18.545562 grai_source_fivetran-0.0.4/src/grai_source_fivetran/loader.py
--rw-r--r--   0        0        0     1668 2023-02-14 16:39:18.545711 grai_source_fivetran-0.0.4/src/grai_source_fivetran/mock_tools.py
--rw-r--r--   0        0        0     4751 2023-02-14 16:39:18.545877 grai_source_fivetran-0.0.4/src/grai_source_fivetran/models.py
--rw-r--r--   0        0        0      186 2023-02-14 16:39:18.546106 grai_source_fivetran-0.0.4/src/grai_source_fivetran/package_definitions.py
--rw-r--r--   0        0        0        0 2023-02-14 16:39:18.546143 grai_source_fivetran-0.0.4/src/grai_source_fivetran/py.typed
--rw-r--r--   0        0        0      888 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.4/setup.py
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      139 2023-04-29 00:58:02.889481 grai_source_fivetran-0.0.5/README.md
+-rw-r--r--   0        0        0     1073 2023-04-30 17:37:05.396093 grai_source_fivetran-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-02-14 16:39:18.542655 grai_source_fivetran-0.0.5/src/grai_source_fivetran/__init__.py
+-rw-r--r--   0        0        0     6644 2023-04-29 00:19:10.366197 grai_source_fivetran-0.0.5/src/grai_source_fivetran/adapters.py
+-rw-r--r--   0        0        0     1425 2023-02-14 16:39:18.543003 grai_source_fivetran-0.0.5/src/grai_source_fivetran/base.py
+-rw-r--r--   0        0        0        0 2023-02-14 16:39:18.543040 grai_source_fivetran-0.0.5/src/grai_source_fivetran/fivetran_api/__init__.py
+-rw-r--r--   0        0        0   436632 2023-02-14 16:39:18.545031 grai_source_fivetran-0.0.5/src/grai_source_fivetran/fivetran_api/api_models.py
+-rw-r--r--   0        0        0    42232 2023-02-14 16:39:18.545359 grai_source_fivetran-0.0.5/src/grai_source_fivetran/fivetran_api/main.py
+-rw-r--r--   0        0        0    12057 2023-02-14 16:39:18.545562 grai_source_fivetran-0.0.5/src/grai_source_fivetran/loader.py
+-rw-r--r--   0        0        0     1668 2023-02-14 16:39:18.545711 grai_source_fivetran-0.0.5/src/grai_source_fivetran/mock_tools.py
+-rw-r--r--   0        0        0     4751 2023-02-14 16:39:18.545877 grai_source_fivetran-0.0.5/src/grai_source_fivetran/models.py
+-rw-r--r--   0        0        0      186 2023-02-14 16:39:18.546106 grai_source_fivetran-0.0.5/src/grai_source_fivetran/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-02-14 16:39:18.546143 grai_source_fivetran-0.0.5/src/grai_source_fivetran/py.typed
+-rw-r--r--   0        0        0     1042 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.5/setup.py
+-rw-r--r--   0        0        0     1044 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.5/PKG-INFO
```

### Comparing `grai_source_fivetran-0.0.4/pyproject.toml` & `grai_source_fivetran-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 [tool.poetry]
 name = "grai_source_fivetran"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_fivetran", from = "src" },
 ]
+readme = "README.md"
+homepage = "https://www.grai.io/"
+repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-fivetran"
+documentation = "https://docs.grai.io/"
+
 [tool.poetry.dependencies]
 python = "^3.9.13"
 pydantic = "^1.9.1"
 grai-client = "^0.2.0"
 multimethod = "^1.8"
 fivetran = "^0.7.0"
 requests = "^2.28.1"
```

### Comparing `grai_source_fivetran-0.0.4/src/grai_source_fivetran/adapters.py` & `grai_source_fivetran-0.0.5/src/grai_source_fivetran/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.4/src/grai_source_fivetran/base.py` & `grai_source_fivetran-0.0.5/src/grai_source_fivetran/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.4/src/grai_source_fivetran/fivetran_api/api_models.py` & `grai_source_fivetran-0.0.5/src/grai_source_fivetran/fivetran_api/api_models.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.4/src/grai_source_fivetran/fivetran_api/main.py` & `grai_source_fivetran-0.0.5/src/grai_source_fivetran/fivetran_api/main.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.4/src/grai_source_fivetran/loader.py` & `grai_source_fivetran-0.0.5/src/grai_source_fivetran/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.4/src/grai_source_fivetran/mock_tools.py` & `grai_source_fivetran-0.0.5/src/grai_source_fivetran/mock_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.4/src/grai_source_fivetran/models.py` & `grai_source_fivetran-0.0.5/src/grai_source_fivetran/models.py`

 * *Files identical despite different names*

