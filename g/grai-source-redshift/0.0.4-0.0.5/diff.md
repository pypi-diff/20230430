# Comparing `tmp/grai_source_redshift-0.0.4.tar.gz` & `tmp/grai_source_redshift-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_redshift-0.0.4.tar", max compression
+gzip compressed data, was "grai_source_redshift-0.0.5.tar", max compression
```

## Comparing `grai_source_redshift-0.0.4.tar` & `grai_source_redshift-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      777 2023-04-26 17:55:43.265533 grai_source_redshift-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      145 2023-04-25 21:23:43.339413 grai_source_redshift-0.0.4/src/grai_source_redshift/__init__.py
--rw-r--r--   0        0        0     6668 2023-04-26 17:55:43.265767 grai_source_redshift-0.0.4/src/grai_source_redshift/adapters.py
--rw-r--r--   0        0        0     1185 2023-04-25 21:23:43.339552 grai_source_redshift-0.0.4/src/grai_source_redshift/base.py
--rw-r--r--   0        0        0     7181 2023-04-25 21:23:43.339626 grai_source_redshift-0.0.4/src/grai_source_redshift/loader.py
--rw-r--r--   0        0        0     4369 2023-04-25 21:23:43.339688 grai_source_redshift-0.0.4/src/grai_source_redshift/models.py
--rw-r--r--   0        0        0      186 2023-04-25 21:23:43.339739 grai_source_redshift-0.0.4/src/grai_source_redshift/package_definitions.py
--rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.4/setup.py
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-04-29 00:58:02.887728 grai_source_redshift-0.0.5/README.md
+-rw-r--r--   0        0        0      970 2023-04-30 17:37:45.872292 grai_source_redshift-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-04-25 21:23:43.339413 grai_source_redshift-0.0.5/src/grai_source_redshift/__init__.py
+-rw-r--r--   0        0        0     6668 2023-04-29 00:19:10.370272 grai_source_redshift-0.0.5/src/grai_source_redshift/adapters.py
+-rw-r--r--   0        0        0     1185 2023-04-25 21:23:43.339552 grai_source_redshift-0.0.5/src/grai_source_redshift/base.py
+-rw-r--r--   0        0        0     7181 2023-04-25 21:23:43.339626 grai_source_redshift-0.0.5/src/grai_source_redshift/loader.py
+-rw-r--r--   0        0        0     4369 2023-04-25 21:23:43.339688 grai_source_redshift-0.0.5/src/grai_source_redshift/models.py
+-rw-r--r--   0        0        0      186 2023-04-25 21:23:43.339739 grai_source_redshift-0.0.5/src/grai_source_redshift/package_definitions.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.5/setup.py
+-rw-r--r--   0        0        0     1071 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.5/PKG-INFO
```

### Comparing `grai_source_redshift-0.0.4/pyproject.toml` & `grai_source_redshift-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,21 @@
- [tool.poetry]
+[tool.poetry]
 name = "grai_source_redshift"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_redshift", from = "src" },
 ]
+readme = "README.md"
+homepage = "https://www.grai.io/"
+repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-redshift"
+documentation = "https://docs.grai.io/"
+
 [tool.poetry.dependencies]
 python = "^3.8"
 grai-client = "^0.2.4"
 multimethod = "^1.8"
 grai-schemas = "^0.1.5"
 redshift-connector = "^2.0.910"
 pydantic = {extras = ["dotenv"], version = "^1.10.7"}
```

### Comparing `grai_source_redshift-0.0.4/src/grai_source_redshift/adapters.py` & `grai_source_redshift-0.0.5/src/grai_source_redshift/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_redshift-0.0.4/src/grai_source_redshift/base.py` & `grai_source_redshift-0.0.5/src/grai_source_redshift/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_redshift-0.0.4/src/grai_source_redshift/loader.py` & `grai_source_redshift-0.0.5/src/grai_source_redshift/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_redshift-0.0.4/src/grai_source_redshift/models.py` & `grai_source_redshift-0.0.5/src/grai_source_redshift/models.py`

 * *Files identical despite different names*

