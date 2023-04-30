# Comparing `tmp/grai_source_snowflake-0.0.8.tar.gz` & `tmp/grai_source_snowflake-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_snowflake-0.0.8.tar", max compression
+gzip compressed data, was "grai_source_snowflake-0.0.9.tar", max compression
```

## Comparing `grai_source_snowflake-0.0.8.tar` & `grai_source_snowflake-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      754 2023-01-27 09:43:56.771279 grai_source_snowflake-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      147 2023-01-23 19:51:17.816018 grai_source_snowflake-0.0.8/src/grai_source_snowflake/__init__.py
--rw-r--r--   0        0        0     6117 2023-01-27 09:34:12.645810 grai_source_snowflake-0.0.8/src/grai_source_snowflake/adapters.py
--rw-r--r--   0        0        0     1445 2023-01-27 08:54:46.068017 grai_source_snowflake-0.0.8/src/grai_source_snowflake/base.py
--rw-r--r--   0        0        0     7587 2023-01-26 12:37:24.794449 grai_source_snowflake-0.0.8/src/grai_source_snowflake/loader.py
--rw-r--r--   0        0        0     4231 2023-01-24 13:52:31.071950 grai_source_snowflake-0.0.8/src/grai_source_snowflake/models.py
--rw-r--r--   0        0        0      150 2023-01-23 19:51:17.816234 grai_source_snowflake-0.0.8/src/grai_source_snowflake/package_definitions.py
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 grai_source_snowflake-0.0.8/setup.py
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 grai_source_snowflake-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      786 2023-01-27 22:50:29.542350 grai_source_snowflake-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      147 2023-01-18 14:35:11.047402 grai_source_snowflake-0.0.9/src/grai_source_snowflake/__init__.py
+-rw-r--r--   0        0        0     6102 2023-01-27 22:50:45.345199 grai_source_snowflake-0.0.9/src/grai_source_snowflake/adapters.py
+-rw-r--r--   0        0        0     1445 2023-01-27 01:14:06.496945 grai_source_snowflake-0.0.9/src/grai_source_snowflake/base.py
+-rw-r--r--   0        0        0     7587 2023-01-27 01:14:06.497042 grai_source_snowflake-0.0.9/src/grai_source_snowflake/loader.py
+-rw-r--r--   0        0        0     4231 2023-01-05 00:57:50.897741 grai_source_snowflake-0.0.9/src/grai_source_snowflake/models.py
+-rw-r--r--   0        0        0      188 2023-01-27 20:53:45.329460 grai_source_snowflake-0.0.9/src/grai_source_snowflake/package_definitions.py
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 grai_source_snowflake-0.0.9/setup.py
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 grai_source_snowflake-0.0.9/PKG-INFO
```

### Comparing `grai_source_snowflake-0.0.8/pyproject.toml` & `grai_source_snowflake-0.0.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 [tool.poetry]
 name = "grai_source_snowflake"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["Tony Lewis <tony@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "ELv2"
 packages = [
     { include = "grai_source_snowflake", from = "src" },
 ]
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
 grai-client = "^0.2.0"
 PyYAML = "^6.0"
 multimethod = "^1.8"
-snowflake-connector-python = "^2.8.3"
+snowflake-connector-python = "^3.0.0"
 grai-schemas = "^0.1.5"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 mypy = "^0.971"
 isort = "^5.10.1"
 types-PyYAML = "^6.0.11"
 pytest = "^7.2.0"
 python-dotenv = "^0.21.1"
 
 [tool.isort]
 profile = "black"
 known_first_party = "grai_source_snowflake"
 
+[tool.black]
+line-length = 120
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `grai_source_snowflake-0.0.8/src/grai_source_snowflake/adapters.py` & `grai_source_snowflake-0.0.9/src/grai_source_snowflake/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,25 @@
     EdgeTypeLabels,
     GenericEdgeMetadataV1,
     TableToColumnMetadata,
 )
 from grai_schemas.v1.metadata.nodes import ColumnMetadata, NodeTypeLabels, TableMetadata
 from multimethod import multimethod
 
-from grai_source_snowflake.models import ID, Column, Edge, Table
+from grai_source_snowflake.models import ID, Column, Constraint, Edge, Table
 from grai_source_snowflake.package_definitions import config
 
 
 @multimethod
 def build_grai_metadata(current: Any, desired: Any) -> None:
-    raise NotImplementedError(
-        f"No adapter between {type(current)} and {type(desired)} for value {current}"
-    )
+    raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
 
 
 @build_grai_metadata.register
-def build_grai_metadata_from_column(
-    current: Column, version: Literal["v1"] = "v1"
-) -> ColumnMetadata:
+def build_grai_metadata_from_column(current: Column, version: Literal["v1"] = "v1") -> ColumnMetadata:
 
     default_value = current.default_value
     if current.default_value is not None:
         default_value = DefaultValue(
             has_default_value=True,
             default_value=current.default_value,
             data_type=current.data_type,
@@ -47,53 +43,47 @@
             "is_primary_key": current.is_pk,
         },
     }
     return ColumnMetadata(**data)
 
 
 @build_grai_metadata.register
-def build_grai_metadata_from_table(
-    current: Table, version: Literal["v1"] = "v1"
-) -> TableMetadata:
+def build_grai_metadata_from_table(current: Table, version: Literal["v1"] = "v1") -> TableMetadata:
     data = {
         "version": version,
         "node_type": NodeTypeLabels.table.value,
         "node_attributes": {},
     }
 
     return TableMetadata(**data)
 
 
 @build_grai_metadata.register
-def build_grai_metadata_from_edge(
-    current: Edge, version: Literal["v1"] = "v1"
-) -> GenericEdgeMetadataV1:
+def build_grai_metadata_from_edge(current: Edge, version: Literal["v1"] = "v1") -> GenericEdgeMetadataV1:
     data = {"version": version}
 
-    # if isinstance(current.source, Table) and isinstance(current.destination, Column):
-    if current.constraint_type.value == "bt":
+    if isinstance(current.source, Table) and isinstance(current.destination, Column):
+        # if current.constraint_type.value == Constraint.belongs_to:
         data["edge_type"] = EdgeTypeLabels.table_to_column.value
         return TableToColumnMetadata(**data)
-    # elif isinstance(current.source, Column) and isinstance(current.destination, Column):
-    else:
+    elif isinstance(current.source, Column) and isinstance(current.destination, Column):
+        # else:
         data["edge_type"] = EdgeTypeLabels.column_to_column.value
         return ColumnToColumnMetadata(**data)
-    # else:
-    #     data["edge_type"] = EdgeTypeLabels.generic.value
-    #     return GenericEdgeMetadataV1(**data)
+    else:
+        data["edge_type"] = EdgeTypeLabels.generic.value
+        return GenericEdgeMetadataV1(**data)
 
 
 # ---
 
 
 @multimethod
 def build_snowflake_metadata(current: Any, desired: Any) -> None:
-    raise NotImplementedError(
-        f"No adapter between {type(current)} and {type(desired)} for value {current}"
-    )
+    raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
 
 
 @build_snowflake_metadata.register
 def build_metadata_from_column(current: Column, version: Literal["v1"] = "v1") -> Dict:
     data = {
         "table_name": current.table,
         "schema": current.column_schema,
```

### Comparing `grai_source_snowflake-0.0.8/src/grai_source_snowflake/base.py` & `grai_source_snowflake-0.0.9/src/grai_source_snowflake/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_snowflake-0.0.8/src/grai_source_snowflake/loader.py` & `grai_source_snowflake-0.0.9/src/grai_source_snowflake/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_snowflake-0.0.8/src/grai_source_snowflake/models.py` & `grai_source_snowflake-0.0.9/src/grai_source_snowflake/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_snowflake-0.0.8/setup.py` & `grai_source_snowflake-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
  'grai-client>=0.2.0,<0.3.0',
  'grai-schemas>=0.1.5,<0.2.0',
  'multimethod>=1.8,<2.0',
  'pydantic>=1.9.1,<2.0.0',
- 'snowflake-connector-python>=2.8.3,<3.0.0']
+ 'snowflake-connector-python>=3.0.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'grai-source-snowflake',
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

### Comparing `grai_source_snowflake-0.0.8/PKG-INFO` & `grai_source_snowflake-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-snowflake
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 License: ELv2
 Author: Tony Lewis
 Author-email: tony@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -13,8 +13,8 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: grai-client (>=0.2.0,<0.3.0)
 Requires-Dist: grai-schemas (>=0.1.5,<0.2.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
-Requires-Dist: snowflake-connector-python (>=2.8.3,<3.0.0)
+Requires-Dist: snowflake-connector-python (>=3.0.0,<4.0.0)
```

