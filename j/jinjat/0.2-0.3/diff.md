# Comparing `tmp/jinjat-0.2.tar.gz` & `tmp/jinjat-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinjat-0.2.tar", max compression
+gzip compressed data, was "jinjat-0.3.tar", max compression
```

## Comparing `jinjat-0.2.tar` & `jinjat-0.3.tar`

### file list

```diff
@@ -1,44 +1,29 @@
--rw-r--r--   0        0        0    11357 2022-12-14 00:06:29.861047 jinjat-0.2/LICENSE
--rw-r--r--   0        0        0     1612 2023-02-15 16:56:13.014837 jinjat-0.2/README.md
--rw-r--r--   0        0        0     2726 2023-03-23 01:49:29.188038 jinjat-0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-14 00:06:29.885463 jinjat-0.2/src/jinjat/__init__.py
--rw-r--r--   0        0        0       93 2023-02-08 01:26:18.226996 jinjat-0.2/src/jinjat/__main__.py
--rw-r--r--   0        0        0        0 2022-12-14 00:06:29.885825 jinjat-0.2/src/jinjat/core/__init__.py
--rw-r--r--   0        0        0        0 2023-01-14 02:35:10.375129 jinjat-0.2/src/jinjat/core/dbt/__init__.py
--rw-r--r--   0        0        0     2338 2023-01-14 02:44:23.141045 jinjat-0.2/src/jinjat/core/dbt/config.py
--rw-r--r--   0        0        0    23048 2023-02-13 23:57:13.201830 jinjat-0.2/src/jinjat/core/dbt/dbt_project.py
--rw-r--r--   0        0        0      929 2023-02-24 22:33:57.365697 jinjat-0.2/src/jinjat/core/exceptions.py
--rw-r--r--   0        0        0     2641 2023-02-08 01:26:18.210131 jinjat-0.2/src/jinjat/core/log_controller.py
--rw-r--r--   0        0        0     5403 2023-03-11 00:28:30.901310 jinjat-0.2/src/jinjat/core/models.py
--rw-r--r--   0        0        0        0 2023-01-06 14:11:33.672166 jinjat-0.2/src/jinjat/core/routes/__init__.py
--rw-r--r--   0        0        0     8772 2023-03-11 00:28:30.908888 jinjat-0.2/src/jinjat/core/routes/analysis.py
--rw-r--r--   0        0        0     8770 2023-02-25 01:34:25.594566 jinjat-0.2/src/jinjat/core/routes/project.py
--rw-r--r--   0        0        0        0 2023-01-13 04:14:51.352851 jinjat-0.2/src/jinjat/core/schema/__init__.py
--rw-r--r--   0        0        0      693 2023-01-13 04:55:28.632790 jinjat-0.2/src/jinjat/core/schema/validator.py
--rw-r--r--   0        0        0     3990 2023-03-09 00:22:08.266534 jinjat-0.2/src/jinjat/core/server.py
--rw-r--r--   0        0        0        0 2023-02-24 22:29:41.652308 jinjat-0.2/src/jinjat/core/util/__init__.py
--rw-r--r--   0        0        0     6907 2023-03-13 12:07:46.015041 jinjat-0.2/src/jinjat/core/util/api.py
--rw-r--r--   0        0        0      158 2023-02-24 22:34:56.920919 jinjat-0.2/src/jinjat/core/util/dbt.py
--rw-r--r--   0        0        0      868 2023-02-24 22:34:56.933299 jinjat-0.2/src/jinjat/core/util/filesystem.py
--rw-r--r--   0        0        0     1715 2023-02-24 23:23:24.209314 jinjat-0.2/src/jinjat/core/util/jmespath.py
--rw-r--r--   0        0        0        0 2022-12-14 00:06:29.885825 jinjat-0.2/src/jinjat/generator/__init__.py
--rw-r--r--   0        0        0      782 2023-02-08 01:51:41.621324 jinjat-0.2/src/jinjat/generator/compiler.py
--rw-r--r--   0        0        0        0 2023-02-08 01:55:24.037009 jinjat-0.2/src/jinjat/generator/crud/[[dbt.analysis_dir]]/[[vars.directory]]/create_[[vars.entity_name]].sql
--rw-r--r--   0        0        0        0 2023-02-08 01:55:24.037009 jinjat-0.2/src/jinjat/generator/crud/[[dbt.analysis_dir]]/[[vars.directory]]/delete_[[vars.entity_name]].sql
--rw-r--r--   0        0        0        0 2023-02-08 01:55:24.037009 jinjat-0.2/src/jinjat/generator/crud/[[dbt.analysis_dir]]/[[vars.directory]]/get_[[vars.entity_name]].sql
--rw-r--r--   0        0        0        0 2023-02-08 01:55:24.037009 jinjat-0.2/src/jinjat/generator/crud/[[dbt.analysis_dir]]/[[vars.directory]]/list_[[vars.entity_name]].sql
--rw-r--r--   0        0        0       44 2023-03-23 01:46:13.669949 jinjat-0.2/src/jinjat/jinjat-refine/.git
--rw-r--r--   0        0        0      366 2023-03-21 23:08:10.685010 jinjat-0.2/src/jinjat/jinjat-refine/asset-manifest.json
--rw-r--r--   0        0        0   101076 2023-03-21 23:08:10.685412 jinjat-0.2/src/jinjat/jinjat-refine/favicon.ico
--rw-r--r--   0        0        0     1000 2023-03-21 23:08:10.685672 jinjat-0.2/src/jinjat/jinjat-refine/index.html
--rw-r--r--   0        0        0     4341 2023-03-21 23:08:10.686055 jinjat-0.2/src/jinjat/jinjat-refine/static/js/787.35e3871e.chunk.js
--rw-r--r--   0        0        0     9899 2023-03-21 23:08:10.686294 jinjat-0.2/src/jinjat/jinjat-refine/static/js/787.35e3871e.chunk.js.map
--rw-r--r--   0        0        0  1772507 2023-03-21 23:08:10.693299 jinjat-0.2/src/jinjat/jinjat-refine/static/js/main.80ec5ce4.js
--rw-r--r--   0        0        0     3368 2023-03-21 23:08:10.693954 jinjat-0.2/src/jinjat/jinjat-refine/static/js/main.80ec5ce4.js.LICENSE.txt
--rw-r--r--   0        0        0  7728147 2023-03-21 23:08:10.717038 jinjat-0.2/src/jinjat/jinjat-refine/static/js/main.80ec5ce4.js.map
--rw-r--r--   0        0        0     4522 2023-03-05 22:24:22.730397 jinjat-0.2/src/jinjat/main.py
--rw-r--r--   0        0        0    10094 2023-02-08 01:26:18.201718 jinjat-0.2/src/jinjat/playground.py
--rw-r--r--   0        0        0      206 2023-02-08 01:26:28.625143 jinjat-0.2/src/jinjat/requirements.txt
--rw-r--r--   0        0        0        0 2023-03-23 01:44:58.605301 jinjat-0.2/src/jinjat/test
--rw-r--r--   0        0        0     3809 2023-03-23 01:49:38.066944 jinjat-0.2/setup.py
--rw-r--r--   0        0        0     4230 2023-03-23 01:49:38.067295 jinjat-0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-30 20:19:09.645611 jinjat-0.3/LICENSE
+-rw-r--r--   0        0        0     1612 2023-04-30 20:19:09.645611 jinjat-0.3/README.md
+-rw-r--r--   0        0        0     2648 2023-04-30 20:19:21.893707 jinjat-0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-30 20:19:09.645611 jinjat-0.3/src/jinjat/__init__.py
+-rw-r--r--   0        0        0       93 2023-04-30 20:19:09.645611 jinjat-0.3/src/jinjat/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-30 20:19:09.645611 jinjat-0.3/src/jinjat/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 20:19:09.645611 jinjat-0.3/src/jinjat/core/dbt/__init__.py
+-rw-r--r--   0        0        0     2348 2023-04-30 20:19:09.645611 jinjat-0.3/src/jinjat/core/dbt/config.py
+-rw-r--r--   0        0        0    23495 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/dbt/dbt_project.py
+-rw-r--r--   0        0        0      878 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/exceptions.py
+-rw-r--r--   0        0        0     4486 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/generator.py
+-rw-r--r--   0        0        0     2641 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/log_controller.py
+-rw-r--r--   0        0        0     5373 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/models.py
+-rw-r--r--   0        0        0        0 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/routes/__init__.py
+-rw-r--r--   0        0        0     8917 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/routes/admin.py
+-rw-r--r--   0        0        0     9164 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/routes/analysis.py
+-rw-r--r--   0        0        0        0 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/schema/__init__.py
+-rw-r--r--   0        0        0      693 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/schema/validator.py
+-rw-r--r--   0        0        0     5947 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/server.py
+-rw-r--r--   0        0        0        0 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/util/__init__.py
+-rw-r--r--   0        0        0     6947 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/util/api.py
+-rw-r--r--   0        0        0     1068 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/util/filesystem.py
+-rw-r--r--   0        0        0     2068 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/util/jmespath.py
+-rw-r--r--   0        0        0    12288 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/jaffle_shop.duckdb
+-rw-r--r--   0        0        0     5889 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/main.py
+-rw-r--r--   0        0        0    10094 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/playground.py
+-rw-r--r--   0        0        0      210 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/requirements.txt
+-rw-r--r--   0        0        0     3558 1970-01-01 00:00:00.000000 jinjat-0.3/setup.py
+-rw-r--r--   0        0        0     4401 1970-01-01 00:00:00.000000 jinjat-0.3/PKG-INFO
```

### Comparing `jinjat-0.2/LICENSE` & `jinjat-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jinjat-0.2/README.md` & `jinjat-0.3/README.md`

 * *Files identical despite different names*

### Comparing `jinjat-0.2/pyproject.toml` & `jinjat-0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jinjat"
-version = "0.2"
+version = "0.3"
 description = "A low-code data application framework that uses dbt Core and OpenAPI"
 authors = ["buremba <emrekabakci@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -17,47 +17,44 @@
     "Programming Language :: Python :: 3.10",
 ]
 keywords = ["dbt", "server", "streamlit", "git", "refine", "data-app", "snowflake"]
 documentation = "https://github.com/jinjat-data/jinjat"
 repository = "https://github.com/jinjat-data/jinjat"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.6,<4"
 click = ">7"
-dbt-core = "=1.3.0"
+dbt-core = "=1.4.5"
 watchdog = ">=2.2.1"
 "ruamel.yaml" = ">=0.17"
 rich = ">=10"
 pydantic = "^1.9.1"
-GitPython = "^3.1.27"
 bottle = "^0.12.23"
 orjson = "^3.8.0"
 fastapi = "^0.85.0"
 openapi-schema-pydantic = "^1.2.4"
 deepmerge = "^1.1.0"
 jsonschema = "^3.0"
-fastapi-crudrouter = "^0.8.5"
 uvicorn = { extras = ["standard"], version = "^0.18.3" }
 jinja2-simple-tags = "^0.4.0"
 jsonref = "^1.1.0"
-cookiecutter = "^2.1.1"
+jmespath = "^1.0.1"
 # Streamlit Playground Dependencies
 streamlit = { version = ">=1.0.0", optional = true }
 streamlit-ace = { version = ">=0.1.0", optional = true }
 graphviz = { version = ">=0.17", optional = true }
 pydot = { version = ">=1.4.2", optional = true }
 streamlit-agraph = { version = ">=0.0.35", optional = true }
 streamlit-pandas-profiling = { version = ">=0.1.3", optional = true }
 streamlit-aggrid = { version = ">=0.2.2", optional = true }
 scipy = { version = "^1.3.1", optional = true }
 feedparser = { version = "^6.0.10", optional = true }
 # Testing duckdb
 duckcli = { version = "^0.2.1", optional = true }
-dbt-duckdb = { version = "^1.2.0", optional = true }
-jmespath = "^1.0.1"
+dbt-duckdb = { version = "^1.4.1", optional = true }
 pandas = "^1.5.3"
 
 [tool.poetry.dev-dependencies]
 black = ">=21.9b0"
 mypy = ">=0.910"
 pytest = ">=6.2.5"
 coverage = ">=5.5"
@@ -76,14 +73,15 @@
     "streamlit-agraph",
     "streamlit-pandas-profiling",
     "streamlit-aggrid",
     "scipy",
     "feedparser",
 ]
 
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 100
```

### Comparing `jinjat-0.2/src/jinjat/core/dbt/config.py` & `jinjat-0.3/src/jinjat/core/dbt/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dbt.flags import DEFAULT_PROFILES_DIR
 from dbt.tracking import disable_tracking
 from dbt.version import __version__ as dbt_version
 from ruamel.yaml import YAML
 
 CACHE = {}
 CACHE_VERSION = 1
-JINJAT_MACRO_NAME = "request"
+JINJAT_REQUEST_VAR_NAME = "jinjat_request"
 
 DBT_MAJOR_VER, DBT_MINOR_VER, DBT_PATCH_VER = (int(v) for v in dbt_version.split("."))
 RAW_CODE = "raw_code" if DBT_MAJOR_VER >= 1 and DBT_MINOR_VER >= 3 else "raw_sql"
 COMPILED_CODE = "compiled_code" if DBT_MAJOR_VER >= 1 and DBT_MINOR_VER >= 3 else "compiled_sql"
 
 JINJA_CONTROL_SEQS = ["{{", "}}", "{%", "%}", "{#", "#}"]
 T = TypeVar("T")
@@ -34,24 +34,25 @@
     def __init__(
             self,
             threads: Optional[int] = 1,
             target: Optional[str] = None,
             profiles_dir: Optional[str] = None,
             project_dir: Optional[str] = None,
             vars: Optional[str] = "{}",
+            profile: Optional[str] = None,
     ):
         self.threads = threads
-        if target:
-            self.target = target  # We don't want target in args context if it is None
+        self.target = target
         self.profiles_dir = profiles_dir or DEFAULT_PROFILES_DIR
         self.project_dir = project_dir
         self.vars = vars  # json.dumps str
         self.dependencies = []
         self.single_threaded = threads == 1
         self.quiet = True
+        self.profile = profile
 
     @classmethod
     def from_str(cls, arguments: str) -> "ConfigInterface":
         import argparse
         import shlex
 
         parser = argparse.ArgumentParser()
```

### Comparing `jinjat-0.2/src/jinjat/core/dbt/dbt_project.py` & `jinjat-0.3/src/jinjat/core/dbt/dbt_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+import sys
+
 import dbt.adapters.factory
+from dbt.exceptions import CompilationError
+from pydantic import BaseModel
 
 from jinjat.core.exceptions import ExecuteSqlFailure
 
 # This is critical because `get_adapter` is all over dbt-core
 # as they expect a singleton adapter instance per plugin,
 # so dbt-niceDatabase will have one adapter instance named niceDatabase.
 # This makes sense in dbt-land where we have a single Project/Profile
 # combination executed in process from start to finish or a single tenant RPC
 # This doesn't fit our paradigm of one adapter per DbtProject in a multitenant server,
 # so we create an adapter instance **independent** of the FACTORY cache
 # and attach it directly to our RuntimeConfig which is passed through
 # anywhere dbt-core needs config including in all `get_adapter` calls
 dbt.adapters.factory.get_adapter = lambda config: config.adapter
 
-from jinjat.core.dbt.config import ConfigInterface, YamlHandler, JINJAT_MACRO_NAME, RAW_CODE, COMPILED_CODE, \
+from jinjat.core.dbt.config import ConfigInterface, YamlHandler, JINJAT_REQUEST_VAR_NAME, RAW_CODE, COMPILED_CODE, \
     has_jinja, T
 from jinjat.core.models import DbtQueryRequestContext, DbtAdapterExecutionResult, DbtAdapterCompilationResult
 import os
 import threading
 import time
 import uuid
 from collections import OrderedDict
@@ -38,15 +42,14 @@
 import agate
 from dbt.adapters.base import BaseRelation
 from dbt.adapters.factory import Adapter, get_adapter_class_by_name
 from dbt.config.runtime import RuntimeConfig
 from dbt.context.providers import generate_runtime_model_context
 from dbt.contracts.connection import AdapterResponse
 from dbt.contracts.graph.manifest import ManifestNode, MaybeNonSource, MaybeParsedSource
-from dbt.exceptions import RuntimeException
 from dbt.flags import set_from_args
 from dbt.node_types import NodeType
 from dbt.parser.manifest import ManifestLoader, process_node
 from dbt.parser.sql import SqlBlockParser, SqlMacroParser
 from dbt.task.parse import MANIFEST_FILE_NAME
 from dbt.task.sql import SqlCompileRunner, SqlExecuteRunner
 
@@ -62,21 +65,23 @@
     def __init__(
             self,
             target: Optional[str] = None,
             profiles_dir: Optional[str] = None,
             project_dir: Optional[str] = None,
             threads: Optional[int] = 1,
             vars: Optional[str] = "{}",
+            profile: Optional[str] = None,
     ):
         self.args = ConfigInterface(
             threads=threads,
             target=target,
             profiles_dir=profiles_dir,
             project_dir=project_dir,
             vars=vars,
+            profile=profile
         )
 
         self.parse_project(init=True)
 
         # Utilities
         self._yaml_handler: Optional[YamlHandler] = None
         self._sql_parser: Optional[SqlBlockParser] = None
@@ -125,15 +130,19 @@
             self.config = RuntimeConfig.from_args(self.args)
             self.init_adapter()
 
         project_parser = ManifestLoader(
             self.config, self.config.load_dependencies(), self.adapter.connections.set_query_header
         )
         # endpatched (https://github.com/dbt-labs/dbt-core/blob/main/core/dbt/parser/manifest.py#L545)
-        self.dbt = project_parser.load()
+        try:
+            self.dbt = project_parser.load()
+        except CompilationError as e:
+            logger().error(f"Encountered an error loading dbt module:\n{e}")
+            sys.exit(1)
         self.dbt.build_flat_graph()
         project_parser.save_macros_to_adapter(self.adapter)
         self._sql_parser = None
         self._macro_parser = None
         self._sql_compiler = None
         self._sql_runner = None
 
@@ -184,15 +193,15 @@
         """Verification for adapter + profile. Used as a passthrough,
         ie: `self.adapter = _verify_connection(get_adapter(...))`
         This also seeds the master connection"""
         try:
             adapter.connections.set_connection_name()
             adapter.debug_query()
         except Exception as query_exc:
-            raise RuntimeException(f"Could not connect to Database: {query_exc}") from query_exc
+            raise Exception(f"Could not connect to Database: {query_exc}") from query_exc
         else:
             return adapter
 
     def adapter_probe(self) -> bool:
         """Check adapter connection, useful for long running processes such as the server or playground"""
         if not hasattr(self, "adapter") or self.adapter is None:
             return False
@@ -327,24 +336,24 @@
             try:
                 compiled_node = self.compile_sql(raw_sql, ctx)
                 compiled_sql = compiled_node.compiled_sql
             except Exception as e:
                 raise ExecuteSqlFailure(raw_sql, None, e)
         try:
             table = self.adapter_execute(compiled_sql, fetch=fetch)
-        except RuntimeException as e:
+        except Exception as e:
             raise ExecuteSqlFailure(raw_sql, compiled_sql, e)
 
         return DbtAdapterExecutionResult(
             *table,
             raw_sql,
             compiled_sql,
         )
 
-    def compile_sql(self, raw_sql: str, ctx: DbtQueryRequestContext, retry: int = 3) -> DbtAdapterCompilationResult:
+    def compile_sql(self, raw_sql: str, ctx: Optional[DbtQueryRequestContext] = None, retry: int = 3) -> DbtAdapterCompilationResult:
         """Creates a node with `get_server_node` method. Compile generated node.
         Has a retry built in because even uuidv4 cannot gaurantee uniqueness at the speed
         in which we can call this function concurrently. A retry significantly increases the stability"""
         temp_node_id = str(uuid.uuid4())
         try:
             node = self.compile_node(self.get_server_node(raw_sql, temp_node_id), ctx)
         except Exception as exc:
@@ -352,21 +361,21 @@
                 return self.compile_sql(raw_sql, ctx, retry - 1)
             raise exc
         else:
             return node
         finally:
             self._clear_node(temp_node_id)
 
-    def compile_node(self, node: ManifestNode, ctx: DbtQueryRequestContext) -> DbtAdapterCompilationResult:
+    def compile_node(self, node: ManifestNode, ctx: Optional[DbtQueryRequestContext]) -> DbtAdapterCompilationResult:
         """Compiles existing node."""
         self.sql_compiler.node = node
         compiler = self.adapter.get_compiler()
         compiled_node = compiler.compile_node(self.sql_compiler.node,
                                               self.dbt,
-                                              {JINJAT_MACRO_NAME: lambda _=None: ctx},
+                                              {JINJAT_REQUEST_VAR_NAME: ctx} if ctx is not None else {},
                                               write=False)
         return DbtAdapterCompilationResult(
             getattr(compiled_node, RAW_CODE),
             getattr(compiled_node, COMPILED_CODE),
             compiled_node,
         )
 
@@ -429,14 +438,23 @@
             target=args.target,
             profiles_dir=args.profiles_dir,
             project_dir=args.project_dir,
             threads=args.threads,
         )
 
 
+class DbtTarget(BaseModel):
+    target: Optional[str] = None
+    profiles_dir: Optional[str] = None
+    project_dir: Optional[str] = None
+    refine: Optional[bool] = False
+    threads: Optional[int] = 1
+    vars: Optional[str] = "{}"
+
+
 class DbtProjectContainer:
     """This class manages multiple DbtProjects which each correspond
     to a single dbt project on disk. This is mostly for jinjat server use"""
 
     def __init__(self):
         self._projects: Dict[str, DbtProject] = OrderedDict()
         self._default_project: Optional[str] = None
@@ -460,23 +478,20 @@
     def get_default_project(self) -> Optional[DbtProject]:
         """Gets the default project which at any given time is the
         earliest project inserted into the container"""
         return self._projects.get(self._default_project)
 
     def add_project(
             self,
-            target: Optional[str] = None,
-            profiles_dir: Optional[str] = None,
-            project_dir: Optional[str] = None,
-            threads: Optional[int] = 1,
-            name_override: Optional[str] = "",
-            vars: Optional[str] = "{}",
+            dbt_target: DbtTarget,
+            name_override: Optional[str] = None
     ) -> DbtProject:
         """Add a DbtProject with arguments"""
-        project = DbtProject(target, profiles_dir, project_dir, threads, vars)
+        project = DbtProject(dbt_target.target, dbt_target.profiles_dir, dbt_target.project_dir, dbt_target.threads,
+                             dbt_target.vars)
         project_name = name_override or project.config.project_name
         if self._default_project is None:
             self._default_project = project_name
         self._projects[project_name] = project
         return project
 
     def add_parsed_project(self, project: DbtProject) -> DbtProject:
```

### Comparing `jinjat-0.2/src/jinjat/core/exceptions.py` & `jinjat-0.3/src/jinjat/core/exceptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Optional
 
-from dbt.exceptions import RuntimeException
 from pydantic import BaseModel
 
 class DbtExecutionError(BaseModel):
     raw_sql: str
     compiled_sql: Optional[str]
     error: str
 
@@ -14,15 +13,15 @@
         super().__init__(*args)
         self.schema_file_path = schema_file_path
         self.sql_file_path = sql_file_path
 
 
 class ExecuteSqlFailure(RuntimeError):
 
-    def __init__(self, raw_sql: str, compiled_sql: Optional[str], dbt_exception: RuntimeException):
+    def __init__(self, raw_sql: str, compiled_sql: Optional[str], dbt_exception: Exception):
         self.raw_sql = raw_sql
         self.compiled_sql = compiled_sql
         self.dbt_exception = dbt_exception
 
     def to_model(self) -> DbtExecutionError:
         return DbtExecutionError(raw_sql=self.raw_sql, compiled_sql=self.compiled_sql, error=str(self.dbt_exception))
```

### Comparing `jinjat-0.2/src/jinjat/core/log_controller.py` & `jinjat-0.3/src/jinjat/core/log_controller.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.2/src/jinjat/core/models.py` & `jinjat-0.3/src/jinjat/core/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-import functools
 import json
 import typing
 from collections import OrderedDict
 from typing import (
     Any,
     List,
     Optional,
     Mapping,
 )
 
 import agate
 from dbt.contracts.connection import AdapterResponse
 from dbt.contracts.graph.manifest import ManifestNode
 from jsonschema import validate
+from openapi_schema_pydantic import OpenAPI
 from openapi_schema_pydantic import Operation
 from pydantic import BaseModel, validator
 from starlette.requests import Request
 
-from openapi_schema_pydantic import OpenAPI
-
 LIMIT_QUERY_PARAM = '_limit'
 JSON_COLUMNS_QUERY_PARAM = '_json_columns'
 
 
+class CORS(BaseModel):
+    allowed_origins: Optional[str]
+
+
 class JinjatProjectConfig(BaseModel):
+    cors: Optional[CORS] = CORS(allowed_origins="*")
     max_limit: Optional[int] = 50000
     default_limit: Optional[int] = 500
     refine: Optional[dict]
     openapi: Optional[dict]
 
     @validator('openapi')
     def validate_openapi(cls, openapi):
@@ -48,29 +51,23 @@
     params: Mapping[str, Any] = {}
     query: Mapping[str, str] = {}
 
     def is_debug_enabled(self) -> bool:
         return self.query.get('_debug') is not None
 
 
-class Transform(BaseModel):
-    jmespath: str
-
-
 class JinjatAnalysisConfig(BaseModel):
     cors: Optional[bool]
     openapi: Optional[Operation] = Operation()
     method: Optional[str]
-    body: Optional[dict]
-    headers: Optional[dict]
     fetch: Optional[bool] = True
-    request_model : Optional[str]
+    request_model: Optional[str]
 
-    transform_response: Optional[List[Transform]]
-    transform_request: Optional[List[Transform]]
+    transform_response: Optional[str]
+    transform_request: Optional[str]
 
 
 async def generate_dbt_context_from_request(request: Request, openapi: dict,
                                             transform_request: typing.Callable[[dict], dict]):
     if request.method in ['PATCH', 'PUT', 'POST']:
         body = transform_request(await request.json())
         validate(instance=body, schema=openapi)
@@ -88,14 +85,15 @@
             self, adapter_response: AdapterResponse, table: agate.Table, raw_sql: str, compiled_sql: str
     ) -> None:
         self.adapter_response = adapter_response
         self.table = table
         self.raw_sql = raw_sql
         self.compiled_sql = compiled_sql
 
+
 def _convert_table_to_dict(table: agate.Table, json_columns: List[str]):
     output = []
     json_funcs = [(lambda x: json.loads(col.jsonify(x))) if table.column_names[i] in json_columns else col.jsonify
                   for i, col in enumerate(table.column_types)]
     for row in table.rows:
         values = tuple(json_funcs[i](d) for i, d in enumerate(row))
         output.append(OrderedDict(zip(row.keys(), values)))
```

### Comparing `jinjat-0.2/src/jinjat/core/routes/analysis.py` & `jinjat-0.3/src/jinjat/core/routes/analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,35 +3,31 @@
 import re
 from copy import deepcopy
 from pathlib import Path
 from typing import List, Optional, Callable
 
 import jmespath
 import jsonref
-from dbt.clients.jinja import get_environment
-from dbt.context.context_config import ContextConfig
-from dbt.context.providers import generate_parser_model_context
 from dbt.node_types import NodeType
 from deepmerge import always_merger
 from fastapi import FastAPI
 from fastapi.openapi.models import Schema, Response as APIResponse
 from fastapi.openapi.utils import get_openapi
 from openapi_schema_pydantic import Parameter
 from pydantic import ValidationError
 from starlette.requests import Request
 from starlette.responses import JSONResponse
-from jinja2schema import infer, to_json_schema, infer_from_ast, parse
 
 from jinjat.core.dbt.dbt_project import DbtProject
 from jinjat.core.exceptions import InvalidJinjaConfig
-from jinjat.core.models import generate_dbt_context_from_request, JinjatExecutionResult, JinjatAnalysisConfig, Transform, \
+from jinjat.core.models import generate_dbt_context_from_request, JinjatExecutionResult, JinjatAnalysisConfig, \
     JinjatProjectConfig, JSON_COLUMNS_QUERY_PARAM
-from jinjat.core.routes.project import _execute_jinjat_query
+from jinjat.core.routes.admin import _execute_jinjat_query
 from jinjat.core.util.api import get_human_readable_error, rapidoc_html, register_jsonapi_exception_handlers, \
-    CustomButton, elements_html
+    CustomButton
 from jinjat.core.util.jmespath import extract_jmespath
 
 ANALYSIS_FILE_PATH_REGEX = re.compile(r"^analysis\/(.*)\.sql$")
 
 
 async def handle_analysis_api(project: DbtProject,
                               sql: str,
@@ -57,15 +53,15 @@
     schema_nodes = filter(
         lambda node: node.resource_type in ['model', 'seed', 'source'] and 'jinjat' in node.meta,
         project.dbt.nodes.values())
 
     components = {}
     for node in schema_nodes:
         jinjat = node.config.meta.get('jinjat')
-        if 'schema' in jinjat:
+        if jinjat is not None and 'schema' in jinjat:
             schema = Schema.parse_obj(jinjat.get('schema'))
         else:
             schema = Schema(type='object')
         schema.properties = {}
         for column in node.columns.values():
             openapi = column.meta.get('jinjat', {}).get('schema')
             if openapi is None:
@@ -86,64 +82,67 @@
         if path.startswith('_'):
             path_name = path[1:]
             paths[idx] = f'{{{path_name}}}'
             param_list.append(path_name)
     return '/'.join(paths), param_list
 
 
-def compile_transform(transform: Optional[List[Transform]]):
-    if transform is None or len(transform) == 0:
+def compile_transform(jmespath_exp: Optional[str]):
+    if jmespath_exp is None or len(jmespath_exp) == 0:
         return lambda body: body
 
-    compiled_transforms = [jmespath.compile(item.jmespath) for item in transform]
+    compiled_transforms = jmespath.compile(jmespath_exp)
 
     def transform_data(body: dict):
-        for transform in compiled_transforms:
-            body = transform.search(body)
-        return body
+        return compiled_transforms.search(body)
 
-    return transform_data
+    return compiled_transforms.search
 
 
 def create_analysis_apps(jinjat_project_config: JinjatProjectConfig, project: DbtProject) -> FastAPI:
     analysis_nodes = filter(lambda node: node.resource_type == NodeType.Analysis.value and node.language == 'sql',
                             project.dbt.nodes.values())
     api = FastAPI(redoc_url=None, docs_url=None, openapi_url=None)
     register_jsonapi_exception_handlers(api)
-    api.add_route("/", functools.partial(rapidoc_html, CustomButton("Admin APIs", "/")), include_in_schema=False)
-    api.add_route("/elements", functools.partial(elements_html, CustomButton("Admin APIs", "/")),
+    api.add_route("/docs", functools.partial(rapidoc_html, CustomButton("Admin APIs", "/admin/docs")),
                   include_in_schema=False)
 
+    # api.add_route("/elements", functools.partial(elements_html, CustomButton("Admin APIs", "/")),
+    #               include_in_schema=False)
+
     async def custom_openapi(req: Request) -> JSONResponse:
-        extract_path = req.query_params.getlist("jmespath")
+        extract_path = req.query_params.get("jmespath")
         if api.openapi_schema:
-            return JSONResponse(extract_jmespath(extract_path, api.openapi_schema))
+            return JSONResponse(extract_jmespath(extract_path, api.openapi_schema, project))
 
         openapi_schema = get_openapi(title=project.project_name, version=project.config.version, routes=api.routes,
                                      servers=[{"url": req.scope.get("root_path", "").rstrip("/")}])
 
         component_schemas = create_components_from_nodes(project)
         components = openapi_schema.setdefault('components', {})
         existing_schemas = components.setdefault('schemas', {})
         components['schemas'] = {**existing_schemas, **component_schemas}
 
         if jinjat_project_config.openapi is not None:
             always_merger.merge(openapi_schema, jinjat_project_config.openapi)
 
         openapi_schema = jsonref.replace_refs(deepcopy(openapi_schema), base_uri="", proxies=False, lazy_load=False)
         api.openapi_schema = openapi_schema
-        return JSONResponse(extract_jmespath(extract_path, api.openapi_schema))
+        return JSONResponse(extract_jmespath(extract_path, api.openapi_schema, project))
 
     api.add_route("/openapi.json", custom_openapi, include_in_schema=False)
 
     for node in analysis_nodes:
-        try:
-            jinjat_config = JinjatAnalysisConfig.parse_obj(node.config.extra['jinjat'])
-        except ValidationError as e:
-            raise InvalidJinjaConfig(node.patch_path, node.original_file_path, get_human_readable_error(e))
+        if 'jinjat' not in node.config.extra:
+            jinjat_config = JinjatAnalysisConfig()
+        else:
+            try:
+                jinjat_config = JinjatAnalysisConfig.parse_obj(node.config.extra['jinjat'])
+            except ValidationError as e:
+                raise InvalidJinjaConfig(node.patch_path, node.original_file_path, get_human_readable_error(e))
         sql = node.raw_code
 
         methods = [jinjat_config.method] if jinjat_config.method is not None else None
         openapi = jinjat_config.openapi
         fetch_enabled = jinjat_config.fetch
 
         if not jinjat_config.fetch:
@@ -167,18 +166,28 @@
         #                                                   project.project_name, ))
         # environment = get_environment(node=node, capture_macros=True)
         # inferred_schema = infer_from_ast(environment.from_string(sql, globals=ctx), ignore_constants=True)
         # inferred_schema_json = to_json_schema(inferred_schema)
         # if openapi.requestBody.content.get('application/json').schema()
 
         openapi_dict = openapi.dict(by_alias=True, exclude_none=True, exclude_unset=True)
+        try:
+            transform_request = compile_transform(jinjat_config.transform_request)
+        except Exception as e:
+            raise InvalidJinjaConfig(node.original_file_path, None, f"Unable to parse `transform_request` jmespath expression {jinjat_config.transform_request}: {e}")
+
+        try:
+            transform_response = compile_transform(jinjat_config.transform_response)
+        except Exception as e:
+            raise InvalidJinjaConfig(node.original_file_path, None, f"Unable to parse `transform_response` jmespath expression {jinjat_config.transform_response}: {e}")
+
         api.add_api_route(api_path,
                           endpoint=functools.partial(handle_analysis_api, project, sql, openapi_dict,
-                                                     compile_transform(jinjat_config.transform_request),
-                                                     compile_transform(jinjat_config.transform_response),
+                                                     transform_request,
+                                                     transform_response,
                                                      fetch_enabled,
                                                      jinjat_project_config),
                           tags=node.tags,
                           description=node.description,
                           summary=node.name,
                           methods=methods,
                           operation_id=node.unique_id,
```

### Comparing `jinjat-0.2/src/jinjat/core/routes/project.py` & `jinjat-0.3/src/jinjat/core/routes/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import asyncio
+import functools
 import json
 from datetime import datetime
 from typing import Optional, Union
 
-from fastapi import APIRouter
+from fastapi import FastAPI
 from pydantic import BaseModel, Field
 from starlette import status
 from starlette.background import BackgroundTasks
 from starlette.requests import Request
 from starlette.responses import Response
 
 from jinjat.core.dbt.dbt_project import DbtProjectContainer, DbtProject
 from jinjat.core.exceptions import ExecuteSqlFailure
 from jinjat.core.models import JinjatExecutionResult, DbtAdapterExecutionResult, generate_dbt_context_from_request, \
     DbtQueryRequestContext, JSON_COLUMNS_QUERY_PARAM
-from jinjat.core.util.api import JinjatErrorContainer, JinjatError, JinjatErrorCode, DBT_PROJECT_HEADER
+from jinjat.core.util.api import JinjatErrorContainer, JinjatError, JinjatErrorCode, DBT_PROJECT_HEADER, \
+    DBT_PROJECT_NAME
 from jinjat.core.util.jmespath import extract_jmespath
 
-router = APIRouter()
-
+app = FastAPI(redoc_url=None, docs_url=None, title="Admin API", version="0.1")
 
 class JinjatCompileResult(BaseModel):
     result: str
 
 
 class JinjatRefreshProjectResult(BaseModel):
     result: str
@@ -36,15 +37,15 @@
 
 class DbtAdhocQueryRequest(BaseModel):
     sql: str = Field(examples=["select 1"])
     request: DbtQueryRequestContext
     limit: Optional[int]
 
 
-@router.get(
+@app.get(
     "/manifest.json"
 )
 async def execute_manifest_query(
         request: Request,
         response: Response,
         jmespath: Optional[str] = None,
         # x_dbt_project: Optional[str] = Header(default=None),
@@ -52,22 +53,23 @@
     """Execute dbt SQL against a registered project as determined by X-dbt-Project header"""
     dbt_container: DbtProjectContainer = request.app.state.dbt_project_container
     project = dbt_container.get_project(None)
 
     if project is None:
         raise jinjat_project_not_found_error()
 
+
     manifest_file = project.dbt.writable_manifest().to_dict()
-    result = extract_jmespath([jmespath], manifest_file)
+    result = extract_jmespath(jmespath, manifest_file, project)
     response.headers[DBT_PROJECT_HEADER] = project.config.version
-    result
+    response.headers[DBT_PROJECT_NAME] = project.config.project_name
     return result
 
 
-@router.post(
+@app.post(
     "/execute",
     response_model=JinjatExecutionResult
 )
 async def execute_sql(
         request: Request,
         body: DbtAdhocQueryRequest,
         # x_dbt_project: Optional[str] = Header(default=None),
@@ -103,15 +105,15 @@
                 error=execution_err.to_model()
             )
         )
 
     return result
 
 
-@router.post(
+@app.post(
     "/compile",
     response_model=JinjatCompileResult
 )
 async def compile_sql(
         request: Request,
         body: DbtAdhocQueryRequest,
         # x_dbt_project: str = Header(),
@@ -148,15 +150,15 @@
                 error=str(compile_err),
             )
         )
 
     return JinjatCompileResult(result=compiled_query)
 
 
-@router.get(
+@app.get(
     "/refresh",
 )
 async def refresh(
         background_tasks: BackgroundTasks,
         request: Request,
         response: Response,
         reset: bool = False,
@@ -220,15 +222,15 @@
             )
         )
     finally:
         project.mutex.release()
     return rv
 
 
-@router.get("/health")
+@app.get("/health")
 async def health_check(
         request: Request,
         # x_dbt_project: str = Header(),
 ) -> dict:
     """Checks if the server is running and accepting requests"""
     dbt: DbtProjectContainer = request.app.state.dbt_project_container
     project = dbt.get_project(None)
```

### Comparing `jinjat-0.2/src/jinjat/core/schema/validator.py` & `jinjat-0.3/src/jinjat/core/schema/validator.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.2/src/jinjat/core/util/api.py` & `jinjat-0.3/src/jinjat/core/util/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pydantic import BaseModel, ValidationError
 from starlette.applications import Starlette
 from starlette.requests import Request
 from starlette.responses import HTMLResponse, Response, JSONResponse
 
 
 DBT_PROJECT_HEADER = 'x-dbt-project-version'
+DBT_PROJECT_NAME = 'x-dbt-project-name'
 
 def get_human_readable_error(validation_error: ValidationError) -> str:
     error_str = "Validation errors:\n"
     for error in validation_error.errors():
         error_str += f'-> {error.get("loc")}: {error.get("msg")}\n'
     return error_str
```

### Comparing `jinjat-0.2/src/jinjat/main.py` & `jinjat-0.3/src/jinjat/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,47 +4,67 @@
 import subprocess
 import sys
 from pathlib import Path
 from typing import Callable, Optional
 
 import click
 import uvicorn
+from dbt.cli.option_types import YAML
+from fal_serverless import sync_dir
 
 from jinjat.core.dbt.config import DEFAULT_PROFILES_DIR
+from jinjat.core.generator import compile_macro
 from jinjat.core.log_controller import logger
 from jinjat.core.server import DbtTarget, SERVER_OPT, app
 
 CONTEXT = {"max_content_width": 800}
 
 
 @click.group()
 @click.version_option()
 def cli():
     pass
 
+
 def shared_server_opts(func: Callable) -> Callable:
     @click.option(
         "--host",
         type=click.STRING,
         help="The host to serve the server on",
+        envvar="JINJAT_HOST",
         default="localhost",
     )
     @click.option(
         "--port",
         type=click.INT,
+        envvar="JINJAT_PORT",
         help="The port to serve the server on",
         default=8581,
     )
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         return func(*args, **kwargs)
 
     return wrapper
 
 
+def serve_project_opts(func: Callable) -> Callable:
+    @click.option(
+        "--refine",
+        is_flag=True,
+        help="Enable Refine UI",
+        default=False
+    )
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
 def shared_single_project_opts(func: Callable) -> Callable:
     @click.option(
         "--project-dir",
         type=click.Path(exists=True, dir_okay=True, file_okay=False),
         default=str(Path.cwd()),
         help="Which directory to look in for the dbt_project.yml file. Default is the current working directory and its parents.",
     )
@@ -56,59 +76,74 @@
     )
     @click.option(
         "-t",
         "--target",
         type=click.STRING,
         help="Which profile to load. Overrides setting in dbt_project.yml.",
     )
+    @click.option(
+        "--vars",
+        envvar=None,
+        default='{}',
+        help="Supply variables to the project. This argument overrides variables defined in your dbt_project.yml file. This argument should be a YAML string, eg. '{my_variable: my_value}'",
+    )
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         return func(*args, **kwargs)
 
     return wrapper
 
 
-def run_server(host="localhost", port=8581):
-    app.state.test = 1
-    uvicorn.run(
-        "jinjat.core.server:app",
-        host=host,
-        port=port,
-        log_level="info",
-        reload=False,
-        workers=1,
-    )
-
-
 @cli.command(context_settings=CONTEXT)
 @shared_single_project_opts
-@shared_server_opts
-def generate_crud(
+@click.argument(
+    "macro",
+    type=click.STRING,
+)
+@click.option(
+    "--args",
+    type=YAML(),
+    default="{}",
+    help="""Supply arguments to the macro. This dictionary will be mapped to the
+            keyword arguments defined in the selected macro. This argument should
+            be a YAML string, eg. '{my_variable: my_value}'
+            """,
+)
+@click.option(
+    "--dry-run",
+    is_flag=True
+)
+def generate(
+        macro: str,
+        args: dict,
+        dry_run: bool,
         project_dir: str,
         profiles_dir: str,
         target: Optional[str],
-        host: str,
-        port: int,
+        vars: str
 ):
-    logger().info(":water_wave: Executing jinjat in single-tenant mode")
-
+    dbt_target = DbtTarget(project_dir=project_dir, profiles_dir=profiles_dir, target=target, vars=vars)
+    compile_macro(dbt_target, macro, args, dry_run)
 
+@serve_project_opts
 @cli.command(context_settings=CONTEXT)
 @shared_single_project_opts
 @shared_server_opts
 def serve(
         project_dir: str,
         profiles_dir: str,
         target: Optional[str],
         host: str,
         port: int,
-):
+        vars: str,
+        refine: bool,
+) -> object:
     logger().info(":water_wave: Executing jinjat in single-tenant mode")
 
-    dbt_target = DbtTarget(project_dir=project_dir, profiles_dir=profiles_dir, target=target)
+    dbt_target = DbtTarget(project_dir=project_dir, profiles_dir=profiles_dir, target=target, vars=vars, refine=refine)
     os.environ[SERVER_OPT] = dbt_target.json()
 
     server = multiprocessing.Process(target=run_server, args=(host, port))
     server.start()
 
     import atexit
 
@@ -165,18 +200,30 @@
         script_args.append("--profiles-dir")
         script_args.append(profiles_dir)
     if target:
         script_args.append("--target")
         script_args.append(target)
 
     streamlit_command = ["streamlit", "run", "--runner.magicEnabled=false",
-                     Path(__file__).parent / "playground.py", ] + ctx.args + script_args
+                         Path(__file__).parent / "playground.py", ] + ctx.args + script_args
     print(streamlit_command)
     subprocess.run(
         streamlit_command,
         env=os.environ,
         cwd=Path.cwd(),
     )
 
 
+def run_server(host="localhost", port=8581):
+    app.state.test = 1
+    uvicorn.run(
+        "jinjat.core.server:app",
+        host=host,
+        port=port,
+        log_level="info",
+        reload=False,
+        workers=1,
+    )
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `jinjat-0.2/src/jinjat/playground.py` & `jinjat-0.3/src/jinjat/playground.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.2/setup.py` & `jinjat-0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,24 @@
 
 packages = \
 ['jinjat',
  'jinjat.core',
  'jinjat.core.dbt',
  'jinjat.core.routes',
  'jinjat.core.schema',
- 'jinjat.core.util',
- 'jinjat.generator']
+ 'jinjat.core.util']
 
 package_data = \
-{'': ['*'],
- 'jinjat': ['jinjat-refine/*', 'jinjat-refine/static/js/*'],
- 'jinjat.generator': ['crud/[[dbt.analysis_dir]]/[[vars.directory]]/*']}
+{'': ['*']}
 
 install_requires = \
-['GitPython>=3.1.27,<4.0.0',
- 'bottle>=0.12.23,<0.13.0',
+['bottle>=0.12.23,<0.13.0',
  'click>7',
- 'cookiecutter>=2.1.1,<3.0.0',
- 'dbt-core==1.3.0',
+ 'dbt-core==1.4.5',
  'deepmerge>=1.1.0,<2.0.0',
- 'fastapi-crudrouter>=0.8.5,<0.9.0',
  'fastapi>=0.85.0,<0.86.0',
  'jinja2-simple-tags>=0.4.0,<0.5.0',
  'jmespath>=1.0.1,<2.0.0',
  'jsonref>=1.1.0,<2.0.0',
  'jsonschema>=3.0,<4.0',
  'openapi-schema-pydantic>=1.2.4,<2.0.0',
  'orjson>=3.8.0,<4.0.0',
@@ -37,15 +31,15 @@
  'pydantic>=1.9.1,<2.0.0',
  'rich>=10',
  'ruamel.yaml>=0.17',
  'uvicorn[standard]>=0.18.3,<0.19.0',
  'watchdog>=2.2.1']
 
 extras_require = \
-{'duckdb': ['duckcli>=0.2.1,<0.3.0', 'dbt-duckdb>=1.2.0,<2.0.0'],
+{'duckdb': ['duckcli>=0.2.1,<0.3.0', 'dbt-duckdb>=1.4.1,<2.0.0'],
  'playground': ['streamlit>=1.0.0',
                 'streamlit-ace>=0.1.0',
                 'graphviz>=0.17',
                 'pydot>=1.4.2',
                 'streamlit-agraph>=0.0.35',
                 'streamlit-pandas-profiling>=0.1.3',
                 'streamlit-aggrid>=0.2.2',
@@ -53,26 +47,26 @@
                 'feedparser>=6.0.10,<7.0.0']}
 
 entry_points = \
 {'console_scripts': ['jinjat = jinjat.main:cli']}
 
 setup_kwargs = {
     'name': 'jinjat',
-    'version': '0.2',
+    'version': '0.3',
     'description': 'A low-code data application framework that uses dbt Core and OpenAPI',
     'long_description': '# Jinjat\n\n## Develop data applications with dbt, SQL, and OpenAPI\n\n### Installation\n\n```commandline\npip install jinjat\n```\n\n### Create your first API\n\nCreate an [analysis]() in `analysis/my_first_api.sql`:\n```sql\n{%- set query = request().query %}\n\nselect \'{{query.example}}\' as col1\n```\n\nAnd create a YML file in `analysis/schema.yml`:\n\n```yml\nversion: 2\n\nanalyses:\n  - name: my_first_api\n    config:\n      jinjat:\n        method: get\n        openapi:\n          parameters:\n            - in: query\n              name: example\n              schema:\n                type: number\n```\n\nStart Jinjat as follows:\n\n```commandline\njinjat serve --project-dir [YOUR_DBT_PROJECT_DIRECTORY]\n```\n\nAnd then run the following CURL command to test the API:\n\n```commandline\ncurl -XGET \'http://127.0.0.1:8581?example=value\'\n```\n\nIt should return the following response:\n\n```json\n[\n  "col1": "3"\n]\n```\n\nJinjat uses OpenAPI to validate the requests and create an API documentation automatically for your API.\n\n## Integrations\n\npoetry install --extras "duckdb"\n\n### Playground\n\npoetry install --extras "playground"\n\n\n#### Installation\n\n```commandline\npip install jinjat[playground]\n```\n\nJinjat Playground is a Streamlit app that lets you develop APIs in your browser.\nOnce you write the template, you can save it to your dbt project as an analysis and expose the API.\n\n### [Refine.dev](https://refine.dev) Integration\n\n#### Installation\n\n```commandline\npip install jinjat[refine]\n```\n\nJinjat Refine integration creates a Refine app from your OpenAPI spec \n\n\n> Jinjat is a fork of [dbt-osmosis](https://github.com/z3z1ma/dbt-osmosis)',
     'author': 'buremba',
     'author_email': 'emrekabakci@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/jinjat-data/jinjat',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.11',
+    'python_requires': '>=3.6,<4',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `jinjat-0.2/PKG-INFO` & `jinjat-0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 Metadata-Version: 2.1
 Name: jinjat
-Version: 0.2
+Version: 0.3
 Summary: A low-code data application framework that uses dbt Core and OpenAPI
 Home-page: https://github.com/jinjat-data/jinjat
 License: Apache 2.0
 Keywords: dbt,server,streamlit,git,refine,data-app,snowflake
 Author: buremba
 Author-email: emrekabakci@gmail.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.6,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Build Tools
 Provides-Extra: duckdb
 Provides-Extra: playground
-Requires-Dist: GitPython (>=3.1.27,<4.0.0)
 Requires-Dist: bottle (>=0.12.23,<0.13.0)
 Requires-Dist: click (>7)
-Requires-Dist: cookiecutter (>=2.1.1,<3.0.0)
-Requires-Dist: dbt-core (==1.3.0)
-Requires-Dist: dbt-duckdb (>=1.2.0,<2.0.0); extra == "duckdb"
+Requires-Dist: dbt-core (==1.4.5)
+Requires-Dist: dbt-duckdb (>=1.4.1,<2.0.0) ; extra == "duckdb"
 Requires-Dist: deepmerge (>=1.1.0,<2.0.0)
-Requires-Dist: duckcli (>=0.2.1,<0.3.0); extra == "duckdb"
+Requires-Dist: duckcli (>=0.2.1,<0.3.0) ; extra == "duckdb"
 Requires-Dist: fastapi (>=0.85.0,<0.86.0)
-Requires-Dist: fastapi-crudrouter (>=0.8.5,<0.9.0)
-Requires-Dist: feedparser (>=6.0.10,<7.0.0); extra == "playground"
-Requires-Dist: graphviz (>=0.17); extra == "playground"
+Requires-Dist: feedparser (>=6.0.10,<7.0.0) ; extra == "playground"
+Requires-Dist: graphviz (>=0.17) ; extra == "playground"
 Requires-Dist: jinja2-simple-tags (>=0.4.0,<0.5.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: jsonref (>=1.1.0,<2.0.0)
 Requires-Dist: jsonschema (>=3.0,<4.0)
 Requires-Dist: openapi-schema-pydantic (>=1.2.4,<2.0.0)
 Requires-Dist: orjson (>=3.8.0,<4.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
-Requires-Dist: pydot (>=1.4.2); extra == "playground"
+Requires-Dist: pydot (>=1.4.2) ; extra == "playground"
 Requires-Dist: rich (>=10)
 Requires-Dist: ruamel.yaml (>=0.17)
-Requires-Dist: scipy (>=1.3.1,<2.0.0); extra == "playground"
-Requires-Dist: streamlit (>=1.0.0); extra == "playground"
-Requires-Dist: streamlit-ace (>=0.1.0); extra == "playground"
-Requires-Dist: streamlit-aggrid (>=0.2.2); extra == "playground"
-Requires-Dist: streamlit-agraph (>=0.0.35); extra == "playground"
-Requires-Dist: streamlit-pandas-profiling (>=0.1.3); extra == "playground"
+Requires-Dist: scipy (>=1.3.1,<2.0.0) ; extra == "playground"
+Requires-Dist: streamlit (>=1.0.0) ; extra == "playground"
+Requires-Dist: streamlit-ace (>=0.1.0) ; extra == "playground"
+Requires-Dist: streamlit-aggrid (>=0.2.2) ; extra == "playground"
+Requires-Dist: streamlit-agraph (>=0.0.35) ; extra == "playground"
+Requires-Dist: streamlit-pandas-profiling (>=0.1.3) ; extra == "playground"
 Requires-Dist: uvicorn[standard] (>=0.18.3,<0.19.0)
 Requires-Dist: watchdog (>=2.2.1)
 Project-URL: Documentation, https://github.com/jinjat-data/jinjat
 Project-URL: Repository, https://github.com/jinjat-data/jinjat
 Description-Content-Type: text/markdown
 
 # Jinjat
```

