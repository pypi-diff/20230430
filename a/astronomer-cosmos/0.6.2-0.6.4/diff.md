# Comparing `tmp/astronomer_cosmos-0.6.2.tar.gz` & `tmp/astronomer_cosmos-0.6.4.tar.gz`

## Comparing `astronomer_cosmos-0.6.2.tar` & `astronomer_cosmos-0.6.4.tar`

### file list

```diff
@@ -1,38 +1,52 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/core/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/__init__.py
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/constants.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/dag.py
--rw-r--r--   0        0        0     9974 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/render.py
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/community/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/community/profiles/__init__.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/community/profiles/exasol.py
--rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/community/profiles/trino.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/__init__.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/operators/__init__.py
--rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/operators/base.py
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/operators/docker.py
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/operators/kubernetes.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/operators/lazy_load.py
--rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/operators/local.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/profiles/__init__.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/profiles/bigquery.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/profiles/databricks.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/profiles/postgres.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/profiles/redshift.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/profiles/snowflake.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/utils/__init__.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/utils/profiles_generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/parser/__init__.py
--rw-r--r--   0        0        0    11586 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/cosmos/providers/dbt/parser/project.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/LICENSE
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/README.rst
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/core/tests/test_airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/__init__.py
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/constants.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/dag.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/dataset.py
+-rw-r--r--   0        0        0    10099 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/render.py
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/community/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/community/profiles/__init__.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/community/profiles/exasol.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/community/profiles/spark.py
+-rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/community/profiles/trino.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/__init__.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/__init__.py
+-rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/base.py
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/docker.py
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/kubernetes.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/lazy_load.py
+-rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/local.py
+-rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/tests/test_docker.py
+-rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/tests/test_local.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/__init__.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/bigquery.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/databricks.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/postgres.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/redshift.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/snowflake.py
+-rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/tests/test_profiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/utils/__init__.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/utils/profiles_generator.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/parser/__init__.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/parser/project.py
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/parser/tests/test_project.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/tests/test_dataset.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/tests/test_export.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/tests/test_render.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/tests/test_version.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/LICENSE
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/README.rst
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     6665 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/PKG-INFO
```

### Comparing `astronomer_cosmos-0.6.2/cosmos/core/airflow.py` & `astronomer_cosmos-0.6.4/cosmos/core/airflow.py`

 * *Files 16% similar despite different names*

```diff
@@ -77,14 +77,24 @@
                     dag=dag,
                     task_group=self,
                 )
 
         # add dependencies
         for ent in cosmos_group.entities:
             for upstream_id in ent.upstream_entity_ids:
+                if upstream_id not in entities:
+                    raise ValueError(
+                        f"Entity {upstream_id} is not in the group {cosmos_group.id}"
+                    )
+
+                if ent.id not in entities:
+                    raise ValueError(
+                        f"Entity {ent.id} is not in the group {cosmos_group.id}"
+                    )
+
                 entities[upstream_id] >> entities[ent.id]
 
 
 def get_airflow_task(
     task: Task, dag: DAG, task_group: Optional[TaskGroup] = None
 ) -> BaseOperator:
     """
```

### Comparing `astronomer_cosmos-0.6.2/cosmos/core/graph/entities.py` & `astronomer_cosmos-0.6.4/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/__init__.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/dag.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def __init__(
         self,
         dbt_project_name: str,
         conn_id: str,
         dbt_args: Dict[str, Any] = {},
         operator_args: Dict[str, Any] = {},
         emit_datasets: bool = True,
-        dbt_root_path: str = "/usr/local/airflow/dbt",
+        dbt_root_path: str = "/usr/local/airflow/dags/dbt",
         dbt_models_dir: str = "models",
         dbt_seeds_dir: str = "seeds",
         test_behavior: Literal["none", "after_each", "after_all"] = "after_each",
         select: Dict[str, List[str]] = {},
         exclude: Dict[str, List[str]] = {},
         execution_mode: Literal["local", "docker", "kubernetes"] = "local",
         *args: Any,
```

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/render.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     dbt_class: str,
 ) -> str:
     return f"cosmos.providers.dbt.core.operators.{execution_mode}.{dbt_class}{execution_mode.capitalize()}Operator"
 
 
 def render_project(
     dbt_project_name: str,
-    dbt_root_path: str = "/usr/local/airflow/dbt",
+    dbt_root_path: str = "/usr/local/airflow/dags/dbt",
     dbt_models_dir: str = "models",
     dbt_snapshots_dir: str = "snapshots",
     dbt_seeds_dir: str = "seeds",
     task_args: Dict[str, Any] = {},
     operator_args: Dict[str, Any] = {},
     test_behavior: Literal["none", "after_each", "after_all"] = "after_each",
     emit_datasets: bool = True,
@@ -42,15 +42,15 @@
     exclude: Dict[str, List[str]] = {},
     execution_mode: Literal["local", "docker", "kubernetes"] = "local",
 ) -> Group:
     """
     Turn a dbt project into a Group
 
     :param dbt_project_name: The name of the dbt project
-    :param dbt_root_path: The root path to your dbt folder. Defaults to /usr/local/airflow/dbt
+    :param dbt_root_path: The root path to your dbt folder. Defaults to /usr/local/airflow/dags/dbt
     :param task_args: Arguments to pass to the underlying dbt operators
     :param operator_args: Parameters to pass to the underlying operators, can include KubernetesPodOperator
         or DockerOperator parameters
     :param test_behavior: The behavior for running tests. Options are "none", "after_each", and "after_all".
         Defaults to "after_each"
     :param emit_datasets: If enabled test nodes emit Airflow Datasets for downstream cross-DAG dependencies
     :param conn_id: The Airflow connection ID to use in Airflow Datasets
@@ -112,30 +112,33 @@
             root_directories = [
                 project.project_dir / path.strip("/") for path in exclude.get("paths")
             ]
             if set(root_directories).intersection(model.path.parents):
                 continue
 
         if "configs" in select:
+            # TODO: coverme
             if not set(select["configs"]).intersection(model.config.config_selectors):
                 continue
 
         if "configs" in exclude:
+            # TODO: coverme
             if set(exclude["configs"]).intersection(model.config.config_selectors):
                 continue
 
         run_args: Dict[str, Any] = {**task_args, **operator_args, "models": model_name}
         test_args: Dict[str, Any] = {**task_args, **operator_args, "models": model_name}
 
         if emit_datasets:
             outlets = [get_dbt_dataset(conn_id, dbt_project_name, model_name)]
 
             if test_behavior == "after_each":
                 test_args["outlets"] = outlets
             else:
+                # TODO: coverme
                 run_args["outlets"] = outlets
 
         if model.type == DbtModelType.DBT_MODEL:
             # make the run task for model
             run_task = Task(
                 id=f"{model_name}_run",
                 operator_class=calculate_operator_class(
@@ -161,14 +164,15 @@
                 operator_class=calculate_operator_class(
                     execution_mode=execution_mode,
                     dbt_class="DbtSeed",
                 ),
                 arguments=run_args,
             )
         else:
+            # TODO: coverme
             logger.error("Unknown DBT type.")
 
         # if test_behavior isn't "after_each", we can just add the task to the
         # base group and do nothing else for now
         if test_behavior != "after_each":
             entities[model_name] = run_task
             base_group.add_entity(entity=run_task)
@@ -210,15 +214,14 @@
             try:
                 dep_task = entities[upstream_model_name]
                 entities[model_name].add_upstream(dep_task)
             except KeyError:
                 logger.error(
                     f"Dependency {upstream_model_name} not found for model {model}"
                 )
-
     if test_behavior == "after_all":
         # make a test task
         test_task = Task(
             id=f"{dbt_project_name}_test",
             operator_class=calculate_operator_class(
                 execution_mode=execution_mode,
                 dbt_class="DbtTest",
```

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/task_group.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/task_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     def __init__(
         self,
         dbt_project_name: str,
         conn_id: str,
         dbt_args: Dict[str, Any] = {},
         operator_args: Dict[str, Any] = {},
         emit_datasets: bool = True,
-        dbt_root_path: str = "/usr/local/airflow/dbt",
+        dbt_root_path: str = "/usr/local/airflow/dags/dbt",
         dbt_models_dir: str = "models",
         dbt_snapshots_dir: str = "snapshots",
         dbt_seeds_dir: str = "seeds",
         test_behavior: Literal["none", "after_each", "after_all"] = "after_each",
         select: Dict[str, List[str]] = {},
         exclude: Dict[str, List[str]] = {},
         execution_mode: Literal["local", "docker", "kubernetes"] = "local",
```

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/community/profiles/exasol.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/community/profiles/exasol.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/community/profiles/trino.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/community/profiles/trino.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
 from pathlib import Path
-from typing import TYPE_CHECKING, Dict, Union
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from airflow.models import Connection
 
 AVAILABLE_AUTH_TYPES = ("certs", "kerberos", "jwt", "ldap")
-TRINO_PROFILE_VARS_TYPE = Dict[str, Union[str, Path]]
 
 # Optional environment variables have to have a default value with the same data type that an expected value would have.
 trino_profile = {
     "outputs": {
         "dev": {
             "type": "trino",
             "method": "{{ env_var('TRINO_AUTH_TYPE') }}",
@@ -42,16 +41,17 @@
         }
     },
     "target": "dev",
 }
 
 
 def create_profile_vars_kerberos(
-    conn: Connection, common_profile_vars: TRINO_PROFILE_VARS_TYPE
-) -> TRINO_PROFILE_VARS_TYPE:
+    conn: Connection,
+    common_profile_vars: dict[str, str],
+) -> dict[str, str]:
     """
     Key tab is not supported by the Trino Airflow connection, in dbt it's set as an env var.
         https://github.com/starburstdata/dbt-trino/blob/v1.4.0/dbt/adapters/trino/connections.py#L204
     A key tab is used in place of a password, so we'll have to enforce that a password is present.
 
     Airflow: kerberos__config                                dbt: krb5_config
     Airflow: kerberos__principal                             dbt: principal
@@ -62,88 +62,91 @@
     Airflow: kerberos__sanitize_mutual_error_response | True dbt: sanitize_mutual_error_response
     Airflow: kerberos__delegate | False                      dbt: delegate
     Airflow: kerberos__ca_bundle                             dbt: cert
     """
     common_profile_vars["TRINO_AUTH_TYPE"] = "kerberos"
     extra_dejson = conn.extra_dejson
     # Mandatory fields
-    krb5_config = Path(extra_dejson.get("kerberos__config"))
-    principal = extra_dejson.get("kerberos__principal")
-    password = conn.password
-    if not all((krb5_config.exists(), principal, password)):
+    krb5_config = str(extra_dejson.get("kerberos__config"))
+    principal = str(extra_dejson.get("kerberos__principal"))
+    password = str(conn.password)
+    if not all((Path(krb5_config).exists(), principal, password)):
         raise ValueError(
             "One of kerberos__config, kerberos__principal or password is missing/incorrect"
         )
     common_profile_vars["TRINO_PASSWORD"] = password
     common_profile_vars["TRINO_KRB5_CONFIG"] = krb5_config
     common_profile_vars["TRINO_PRINCIPAL"] = principal
     # Optional fields
-    common_profile_vars["TRINO_SERVICE_NAME"] = extra_dejson.get(
-        "kerberos__service_name"
+    common_profile_vars["TRINO_SERVICE_NAME"] = str(
+        extra_dejson.get("kerberos__service_name")
     )
-    common_profile_vars["TRINO_MUTUAL_AUTHENTICATION"] = extra_dejson.get(
-        "kerberos__mutual_authentication"
+    common_profile_vars["TRINO_MUTUAL_AUTHENTICATION"] = str(
+        extra_dejson.get("kerberos__mutual_authentication")
     )
-    common_profile_vars["TRINO_FORCE_PREEMPTIVE"] = extra_dejson.get(
-        "kerberos__force_preemptive"
+    common_profile_vars["TRINO_FORCE_PREEMPTIVE"] = str(
+        extra_dejson.get("kerberos__force_preemptive")
     )
-    common_profile_vars["TRINO_HOSTNAME_OVERRIDE"] = extra_dejson.get(
-        "kerberos__hostname_override"
+    common_profile_vars["TRINO_HOSTNAME_OVERRIDE"] = str(
+        extra_dejson.get("kerberos__hostname_override")
     )
-    common_profile_vars["TRINO_SANITIZE_MUTUAL_ERROR_RESPONSE"] = extra_dejson.get(
-        "kerberos__sanitize_mutual_error_response"
+    common_profile_vars["TRINO_SANITIZE_MUTUAL_ERROR_RESPONSE"] = str(
+        extra_dejson.get("kerberos__sanitize_mutual_error_response")
     )
-    common_profile_vars["TRINO_DELEGATE"] = extra_dejson.get("kerberos__delegate")
+    common_profile_vars["TRINO_DELEGATE"] = str(extra_dejson.get("kerberos__delegate"))
     # Not sure if this is supposed to be a file or not.
     # https://github.com/trinodb/trino-python-client/blob/0.321.0/trino/auth.py#L84
-    common_profile_vars["TRINO_CA_BUNDLE"] = extra_dejson.get("kerberos__ca_bundle")
+    common_profile_vars["TRINO_CA_BUNDLE"] = str(
+        extra_dejson.get("kerberos__ca_bundle")
+    )
 
     return common_profile_vars
 
 
 def create_profile_vars_ldap(
-    conn: Connection, common_profile_vars: TRINO_PROFILE_VARS_TYPE
-) -> TRINO_PROFILE_VARS_TYPE:
+    conn: Connection,
+    common_profile_vars: dict[str, str],
+) -> dict[str, str]:
     """
     All we need here is a user and password.
     """
     common_profile_vars["TRINO_AUTH_TYPE"] = "ldap"
     # Validate mandatory fields
     if not all((conn.login, conn.password)):
         raise ValueError("Trino auth type: ldap, missing login or password")
     common_profile_vars["TRINO_USER"] = conn.login
     common_profile_vars["TRINO_PASSWORD"] = conn.password
 
     return common_profile_vars
 
 
 def create_profile_vars_certs(
-    conn: Connection, common_profile_vars: TRINO_PROFILE_VARS_TYPE
-) -> TRINO_PROFILE_VARS_TYPE:
+    conn: Connection, common_profile_vars: dict[str, str]
+) -> dict[str, str]:
     """
     Airflow: certs__client_cert_path = dbt: client_certificate
     Airflow: certs__client_key_path  = dbt: client_private_key
     """
     common_profile_vars["TRINO_AUTH_TYPE"] = "certificate"
     extra_dejson = conn.extra_dejson
-    cert_path = Path(extra_dejson.get("certs__client_cert_path"))
-    key_path = Path(extra_dejson.get("certs__client_key_path"))
+    cert_path = Path(str(extra_dejson.get("certs__client_cert_path")))
+    key_path = Path(str(extra_dejson.get("certs__client_key_path")))
     if not cert_path.exists():
         raise ValueError(f"certs__client_cert_path: {cert_path} does not exist")
     if not key_path.exists():
         raise ValueError(f"certs__client_key_path: {key_path} does not exist")
-    common_profile_vars["TRINO_CLIENT_CERTIFICATE"] = cert_path
-    common_profile_vars["TRINO_CLIENT_PRIVATE_KEY"] = key_path
+    common_profile_vars["TRINO_CLIENT_CERTIFICATE"] = str(cert_path)
+    common_profile_vars["TRINO_CLIENT_PRIVATE_KEY"] = str(key_path)
 
     return common_profile_vars
 
 
 def create_profile_vars_jwt(
-    conn: Connection, common_profile_vars: TRINO_PROFILE_VARS_TYPE
-) -> TRINO_PROFILE_VARS_TYPE:
+    conn: Connection, common_profile_vars: dict[str, str]
+) -> dict[str, str]:
     """
     Airflow: jwt__token = dbt: jwt_token
     """
     common_profile_vars["TRINO_AUTH_TYPE"] = "jwt"
     extra_dejson = conn.extra_dejson
     jwt_token = extra_dejson.get("jwt__token")
     if not jwt_token:
@@ -152,38 +155,43 @@
     return common_profile_vars
 
 
 def create_profile_vars_trino(
     conn: Connection,
     database_override: str | None = None,
     schema_override: str | None = None,
-) -> tuple[str, TRINO_PROFILE_VARS_TYPE]:
+) -> tuple[str, dict[str, str]]:
     """
     https://docs.getdbt.com/reference/warehouse-setups/trino-setup
     https://airflow.apache.org/docs/apache-airflow-providers-trino/stable/connections.html
 
     Airflow supports ldap, kerberos, jwt token and certificates.
     dbt additionally supports oauth and none which we will not support here.
     """
     extra_dejson = conn.extra_dejson
     auth_type = extra_dejson.get("auth", "ldap")
     if auth_type not in AVAILABLE_AUTH_TYPES:
         raise ValueError(
             f"Trino auth type: {auth_type} is not allowed, choose one of {AVAILABLE_AUTH_TYPES} or leave blank for ldap"
         )
     common_vars = {
-        "TRINO_HTTP_SCHEME": extra_dejson.get("protocol"),
+        "TRINO_HTTP_SCHEME": str(extra_dejson.get("protocol")),
         "TRINO_DATABASE": database_override
         if database_override is not None
-        else extra_dejson.get("catalog"),
+        else str(extra_dejson.get("catalog")),
         "TRINO_SCHEMA": schema_override if schema_override is not None else conn.schema,
         "TRINO_HOST": conn.host,
         "TRINO_PORT": str(conn.port),
-        "TRINO_SESSION_PROPERTIES": extra_dejson.get("session_properties"),
     }
+
+    if extra_dejson.get("session_properties"):
+        common_vars["TRINO_SESSION_PROPERTIES"] = str(
+            extra_dejson.get("session_properties")
+        )
+
     dispatch = {
         "ldap": create_profile_vars_ldap,
         "kerberos": create_profile_vars_kerberos,
         "certs": create_profile_vars_certs,
         "jwt": create_profile_vars_jwt,
     }
```

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/operators/__init__.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/operators/base.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/operators/docker.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/operators/kubernetes.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/kubernetes.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 logger = logging.getLogger(__name__)
 
 # kubernetes is an optional dependency, so we need to check if it's installed
 try:
     from airflow.providers.cncf.kubernetes.backcompat.backwards_compat_converters import (
         convert_env_vars,
     )
-    from airflow.providers.cncf.kubernetes.operators.kubernetes_pod import (
-        KubernetesPodOperator,
-    )
+    from airflow.providers.cncf.kubernetes.operators.pod import KubernetesPodOperator
     from kubernetes.client import models as k8s
 except ImportError:
     raise ImportError(
         "Could not import KubernetesPodOperator. Ensure you've installed the Kubernetes provider "
         "separately or with with `pip install astronomer-cosmos[...,kubernetes]`."
     )
```

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/operators/local.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/local.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/profiles/__init__.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Callable, Dict, Optional, Tuple
+from typing import TYPE_CHECKING, Callable, Optional
 
 from cosmos.providers.dbt.community.profiles.exasol import (
     create_profile_vars_exasol,
     exasol_profile,
 )
+from cosmos.providers.dbt.community.profiles.spark import (
+    create_profile_vars_spark_thrift,
+    spark_profile,
+)
 from cosmos.providers.dbt.community.profiles.trino import (
     create_profile_vars_trino,
     trino_profile,
 )
 from cosmos.providers.dbt.core.profiles.bigquery import (
     bigquery_profile,
     create_profile_vars_google_cloud_platform,
@@ -33,21 +39,21 @@
 if TYPE_CHECKING:
     from airflow.models import Connection
 
 
 @dataclass
 class AdapterConfig:
     profile_name: str
-    profile: Dict[str, str]
+    profile: dict[str, str]
     create_profile_function: Callable[
-        ["Connection", Optional[str], Optional[str]], Tuple[str, Dict[str, str]]
+        [Connection, Optional[str], Optional[str]], tuple[str, dict[str, str]]
     ]
 
 
-def get_available_adapters() -> Dict[str, AdapterConfig]:
+def get_available_adapters() -> dict[str, AdapterConfig]:
     return {
         "postgres": AdapterConfig(
             "postgres_profile", postgres_profile, create_profile_vars_postgres
         ),
         "redshift": AdapterConfig(
             "redshift_profile", redshift_profile, create_profile_vars_redshift
         ),
@@ -64,8 +70,11 @@
         ),
         "exasol": AdapterConfig(
             "exasol_profile", exasol_profile, create_profile_vars_exasol
         ),
         "trino": AdapterConfig(
             "trino_profile", trino_profile, create_profile_vars_trino
         ),
+        "spark": AdapterConfig(
+            "spark_profile", spark_profile, create_profile_vars_spark_thrift
+        ),
     }
```

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/profiles/bigquery.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/bigquery.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/profiles/databricks.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/databricks.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/profiles/postgres.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/postgres.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/profiles/redshift.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/redshift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/profiles/snowflake.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/snowflake.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/core/utils/profiles_generator.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/utils/profiles_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,45 @@
+from __future__ import annotations
+
 import fcntl
 import logging
 import sys
 from pathlib import Path
-from typing import Optional, Tuple
+from typing import Optional
 
-import pkg_resources
 import yaml
 from airflow.exceptions import AirflowNotFoundException
 from airflow.hooks.base import BaseHook
 
 from cosmos.providers.dbt.core.profiles import get_available_adapters
 
 logger = logging.getLogger(__name__)
 
 
+def cosmos_version() -> str:
+    """
+    Returns the current version of astronomer-cosmos.
+    """
+    import cosmos
+
+    return cosmos.__version__
+
+
 def create_default_profiles(profile_path: Path) -> None:
     """
     Write all the available profiles out to the profile path.
     :param profile_path: The path location to write all the profiles to.
     :return: Nothing
     """
     # get installed version of astronomer-cosmos
-    try:
-        package = pkg_resources.get_distribution("astronomer-cosmos")
-    except pkg_resources.DistributionNotFound:
-        package = None
     profiles = {}
     for adapter_config in get_available_adapters().values():
         profiles[adapter_config.profile_name] = adapter_config.profile
     write_file = False
-    package_comment_line = f"# {package}\n"
+    package_comment_line = f"# astronomer-cosmos {cosmos_version()}\n"
     if profile_path.exists():
         # check the version of cosmos when it was created
         with open(profile_path) as f:
             first_line = next(f)
         if first_line != package_comment_line:
             # if version of cosmos has been updated - re-write the profiles.yml file
             write_file = True
@@ -50,15 +56,15 @@
             fcntl.flock(file, fcntl.LOCK_UN)
 
 
 def map_profile(
     conn_id: str,
     db_override: Optional[str] = None,
     schema_override: Optional[str] = None,
-) -> Tuple[str, dict]:
+) -> tuple[str, dict[str, str]]:
     conn = BaseHook().get_connection(conn_id)
     connection_type = conn.conn_type
     adapters = get_available_adapters()
     if connection_type in adapters:
         return adapters[connection_type].create_profile_function(
             conn, db_override, schema_override
         )
```

### Comparing `astronomer_cosmos-0.6.2/cosmos/providers/dbt/parser/project.py` & `astronomer_cosmos-0.6.4/cosmos/providers/dbt/parser/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,15 @@
                                 if isinstance(extracted_config, (str, List))
                                 else set()
                             )
 
         # set the config and set the parsed file flag to true
         self.config = config
 
+    # TODO following needs coverage:
     def _extract_config(self, kwarg, config_name: str):
         if hasattr(kwarg, "key") and kwarg.key == config_name:
             try:
                 # try to convert it to a constant and get the value
                 value = kwarg.value.as_const()
                 if isinstance(value, List):
                     value = [f"{config_name}:{item}" for item in value]
@@ -193,15 +194,15 @@
     Represents a single dbt project.
     """
 
     # required, user-specified instance variables
     project_name: str
 
     # optional, user-specified instance variables
-    dbt_root_path: str = "/usr/local/airflow/dbt"
+    dbt_root_path: str = "/usr/local/airflow/dags/dbt"
     dbt_models_dir: str = "models"
     dbt_snapshots_dir: str = "snapshots"
     dbt_seeds_dir: str = "seeds"
 
     # private instance variables for managing state
     models: Dict[str, DbtModel] = field(default_factory=dict)
     snapshots: Dict[str, DbtModel] = field(default_factory=dict)
```

### Comparing `astronomer_cosmos-0.6.2/.gitignore` & `astronomer_cosmos-0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.2/LICENSE` & `astronomer_cosmos-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.2/README.rst` & `astronomer_cosmos-0.6.4/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,47 @@
-.. image:: https://github.com/astronomer/astronomer-cosmos/raw/main/docs/_static/banner.png
-  :align: center
-
 .. |fury| image:: https://badge.fury.io/py/astronomer-cosmos.svg
     :target: https://badge.fury.io/py/astronomer-cosmos
 
 .. |ossrank| image:: https://img.shields.io/endpoint?url=https://ossrank.com/shield/2121
     :target: https://ossrank.com/p/2121-astronomer-cosmos
 
 .. |downloads| image:: https://img.shields.io/pypi/dm/astronomer-cosmos.svg
     :target: https://img.shields.io/pypi/dm/astronomer-cosmos
 
 .. |pre-commit| image:: https://results.pre-commit.ci/badge/github/astronomer/astronomer-cosmos/main.svg
    :target: https://results.pre-commit.ci/latest/github/astronomer/astronomer-cosmos/main
    :alt: pre-commit.ci status
 
 
-Astronomer Cosmos |fury| |ossrank| |downloads| |pre-commit|
+
+.. image:: https://raw.githubusercontent.com/astronomer/astronomer-cosmos/main/docs/cosmos-logo.svg
+
+
 ===========================================================
 
-A framework for dynamically generating `Apache Airflow <https://airflow.apache.org/>`_ DAGs from other tools and frameworks. Develop your workflow in your tool of choice and render it in Airflow as a DAG or Task Group!
+|fury| |ossrank| |downloads| |pre-commit|
 
-Current support for:
- - dbt
+Run your dbt Core projects as `Apache Airflow <https://airflow.apache.org/>`_ DAGs and Task Groups with a few lines of code. Benefits include:
 
-Coming soon:
- - Jupyter
- - Hex
- - And more...open an issue if you have a request!
+- Run dbt projects against Airflow connections instead of dbt profiles
+- Native support for installing and running dbt in a virtual environment to avoid dependency conflicts with Airflow
+- Run tests immediately after a model is done to catch issues early
+- Utilize Airflow's data-aware scheduling to run models immediately after upstream ingestion
+- Turn each dbt model into a task/task group complete with retries, alerting, etc.
 
 Quickstart
 __________
 
 Check out the Quickstart guide on our `docs <https://astronomer.github.io/astronomer-cosmos/#quickstart>`_.
 
 
-Example Usage (dbt)
+Example Usage
 ___________________
 
-Cosmos lets you render dbt projects as Airflow DAGs and Task Groups. To render a DAG, import ``DbtDag`` and point it to your dbt project.
-
-.. code-block:: python
-
-    from pendulum import datetime
-    from airflow import DAG
-    from cosmos.providers.dbt.dag import DbtDag
-
-    # dag for the project jaffle_shop
-    jaffle_shop = DbtDag(
-        dbt_project_name="jaffle_shop",
-        conn_id="airflow_db",
-        dbt_args={
-            "schema": "public",
-        },
-        dag_id="jaffle_shop",
-        start_date=datetime(2022, 11, 27),
-    )
-
-Simiarly, you can render an Airflow TaskGroups using the ``DbtTaskGroup`` class. Here's an example with the jaffle_shop project:
+You can render an Airflow Task Group using the ``DbtTaskGroup`` class. Here's an example with the jaffle_shop project:
 
 .. code-block:: python
 
     from pendulum import datetime
 
     from airflow import DAG
     from airflow.operators.empty import EmptyOperator
@@ -69,29 +50,33 @@
 
     with DAG(
         dag_id="extract_dag",
         start_date=datetime(2022, 11, 27),
         schedule="@daily",
     ):
 
-        e1 = EmptyOperator(task_id="ingestion_workflow")
+        e1 = EmptyOperator(task_id="pre_dbt")
 
         dbt_tg = DbtTaskGroup(
-            group_id="dbt_tg",
             dbt_project_name="jaffle_shop",
             conn_id="airflow_db",
             dbt_args={
                 "schema": "public",
             },
         )
 
-        e2 = EmptyOperator(task_id="some_extraction")
+        e2 = EmptyOperator(task_id="post_dbt")
 
         e1 >> dbt_tg >> e2
 
+This will generate an Airflow Task Group that looks like this:
+
+.. image:: https://raw.githubusercontent.com/astronomer/astronomer-cosmos/main/docs/jaffle_shop_task_group.png
+
+
 Changelog
 _________
 
 We follow `Semantic Versioning <https://semver.org/>`_ for releases.
 Check `CHANGELOG.rst <https://github.com/astronomer/astronomer-cosmos/blob/main/CHANGELOG.rst>`_
 for the latest changes.
```

### Comparing `astronomer_cosmos-0.6.2/pyproject.toml` & `astronomer_cosmos-0.6.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -31,27 +31,28 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
-    "apache-airflow>=2.4",
+    "apache-airflow>=2.3.0",
     "Jinja2>=3.0.0",
     "typing-extensions; python_version < '3.8'",
 ]
 
 [project.optional-dependencies]
 dbt-all = [
     "dbt-bigquery",
     "dbt-databricks",
     "dbt-exasol",
     "dbt-postgres",
     "dbt-redshift",
     "dbt-snowflake",
+    "dbt-spark",
     "astronomer-cosmos[dbt-openlineage]"
 ]
 dbt-bigquery = [
     "dbt-bigquery",
 ]
 dbt-databricks = [
     "dbt-databricks",
@@ -64,14 +65,17 @@
 ]
 dbt-redshift = [
     "dbt-redshift",
 ]
 dbt-snowflake = [
     "dbt-snowflake",
 ]
+dbt-spark = [
+    "dbt-spark",
+]
 dbt-openlineage = [
     "dbt-core",
     "openlineage-dbt>=0.21.1"
 ]
 all = [
     "astronomer-cosmos[dbt-all]",
 ]
@@ -109,27 +113,71 @@
 path = "cosmos/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
     "/cosmos",
 ]
 
+######################################
+# TESTING
+######################################
+
+[tool.hatch.envs.tests]
+dependencies = [
+    "pytest>=6.0",
+    "pytest-split",
+    "pytest-dotenv",
+    "requests-mock",
+    "pytest-cov",
+    "pytest-describe",
+    "types-requests",
+    "mypy",
+    "sqlalchemy-stubs", # Change when sqlalchemy is upgraded https://docs.sqlalchemy.org/en/14/orm/extensions/mypy.html
+
+    "apache-airflow-providers-docker>=3.5.0",
+    "apache-airflow-providers-cncf-kubernetes>=5.1.1",
+]
+
+[[tool.hatch.envs.tests.matrix]]
+python = ["3.7", "3.8", "3.9", "3.10"]
+airflow = ["2.3", "2.4", "2.5"]
+
+[tool.hatch.envs.tests.overrides]
+matrix.airflow.dependencies = [
+    { value = "apache-airflow==2.3", if = ["2.3"] },
+    { value = "apache-airflow==2.4", if = ["2.4"] },
+    { value = "apache-airflow==2.5", if = ["2.5"] },
+]
+
+[tool.hatch.envs.tests.scripts]
+freeze = "pip freeze"
+test = "pytest ."
+test-cov = "pytest --cov=cosmos --cov-report=term-missing --cov-report=xml ."
+
+######################################
+# DOCS
+######################################
+
 [tool.hatch.envs.docs]
 dependencies = [
     "sphinx",
     "pydata-sphinx-theme",
     "sphinx-autobuild",
     "sphinx-tabs",
     "sphinx-autoapi"
 ]
 
 [tool.hatch.envs.docs.scripts]
 build = "sphinx-build -b html docs docs/_build"
 serve = "sphinx-autobuild docs docs/_build"
 
+######################################
+# THIRD PARTY TOOLS
+######################################
+
 [tool.isort]
 profile = "black"
 known_third_party = ["airflow", "jinja2"]
 
 [tool.mypy]
 strict = true
```

### Comparing `astronomer_cosmos-0.6.2/PKG-INFO` & `astronomer_cosmos-0.6.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-cosmos
-Version: 0.6.2
+Version: 0.6.4
 Summary: Render 3rd party workflows in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags,dbt
@@ -18,27 +18,28 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
-Requires-Dist: apache-airflow>=2.4
+Requires-Dist: apache-airflow>=2.3.0
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: typing-extensions; python_version < '3.8'
 Provides-Extra: all
 Requires-Dist: astronomer-cosmos[dbt-all]; extra == 'all'
 Provides-Extra: dbt-all
 Requires-Dist: astronomer-cosmos[dbt-openlineage]; extra == 'dbt-all'
 Requires-Dist: dbt-bigquery; extra == 'dbt-all'
 Requires-Dist: dbt-databricks; extra == 'dbt-all'
 Requires-Dist: dbt-exasol; extra == 'dbt-all'
 Requires-Dist: dbt-postgres; extra == 'dbt-all'
 Requires-Dist: dbt-redshift; extra == 'dbt-all'
 Requires-Dist: dbt-snowflake; extra == 'dbt-all'
+Requires-Dist: dbt-spark; extra == 'dbt-all'
 Provides-Extra: dbt-bigquery
 Requires-Dist: dbt-bigquery; extra == 'dbt-bigquery'
 Provides-Extra: dbt-databricks
 Requires-Dist: dbt-databricks; extra == 'dbt-databricks'
 Provides-Extra: dbt-exasol
 Requires-Dist: dbt-exasol; extra == 'dbt-exasol'
 Provides-Extra: dbt-openlineage
@@ -46,14 +47,16 @@
 Requires-Dist: openlineage-dbt>=0.21.1; extra == 'dbt-openlineage'
 Provides-Extra: dbt-postgres
 Requires-Dist: dbt-postgres; extra == 'dbt-postgres'
 Provides-Extra: dbt-redshift
 Requires-Dist: dbt-redshift; extra == 'dbt-redshift'
 Provides-Extra: dbt-snowflake
 Requires-Dist: dbt-snowflake; extra == 'dbt-snowflake'
+Provides-Extra: dbt-spark
+Requires-Dist: dbt-spark; extra == 'dbt-spark'
 Provides-Extra: docker
 Requires-Dist: apache-airflow-providers-docker>=3.5.0; extra == 'docker'
 Provides-Extra: docs
 Requires-Dist: pydata-sphinx-theme; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-autoapi; extra == 'docs'
 Requires-Dist: sphinx-autobuild; extra == 'docs'
@@ -68,73 +71,54 @@
 Requires-Dist: pytest-split; extra == 'tests'
 Requires-Dist: pytest>=6.0; extra == 'tests'
 Requires-Dist: requests-mock; extra == 'tests'
 Requires-Dist: sqlalchemy-stubs; extra == 'tests'
 Requires-Dist: types-requests; extra == 'tests'
 Description-Content-Type: text/x-rst
 
-.. image:: https://github.com/astronomer/astronomer-cosmos/raw/main/docs/_static/banner.png
-  :align: center
-
 .. |fury| image:: https://badge.fury.io/py/astronomer-cosmos.svg
     :target: https://badge.fury.io/py/astronomer-cosmos
 
 .. |ossrank| image:: https://img.shields.io/endpoint?url=https://ossrank.com/shield/2121
     :target: https://ossrank.com/p/2121-astronomer-cosmos
 
 .. |downloads| image:: https://img.shields.io/pypi/dm/astronomer-cosmos.svg
     :target: https://img.shields.io/pypi/dm/astronomer-cosmos
 
 .. |pre-commit| image:: https://results.pre-commit.ci/badge/github/astronomer/astronomer-cosmos/main.svg
    :target: https://results.pre-commit.ci/latest/github/astronomer/astronomer-cosmos/main
    :alt: pre-commit.ci status
 
 
-Astronomer Cosmos |fury| |ossrank| |downloads| |pre-commit|
+
+.. image:: https://raw.githubusercontent.com/astronomer/astronomer-cosmos/main/docs/cosmos-logo.svg
+
+
 ===========================================================
 
-A framework for dynamically generating `Apache Airflow <https://airflow.apache.org/>`_ DAGs from other tools and frameworks. Develop your workflow in your tool of choice and render it in Airflow as a DAG or Task Group!
+|fury| |ossrank| |downloads| |pre-commit|
 
-Current support for:
- - dbt
+Run your dbt Core projects as `Apache Airflow <https://airflow.apache.org/>`_ DAGs and Task Groups with a few lines of code. Benefits include:
 
-Coming soon:
- - Jupyter
- - Hex
- - And more...open an issue if you have a request!
+- Run dbt projects against Airflow connections instead of dbt profiles
+- Native support for installing and running dbt in a virtual environment to avoid dependency conflicts with Airflow
+- Run tests immediately after a model is done to catch issues early
+- Utilize Airflow's data-aware scheduling to run models immediately after upstream ingestion
+- Turn each dbt model into a task/task group complete with retries, alerting, etc.
 
 Quickstart
 __________
 
 Check out the Quickstart guide on our `docs <https://astronomer.github.io/astronomer-cosmos/#quickstart>`_.
 
 
-Example Usage (dbt)
+Example Usage
 ___________________
 
-Cosmos lets you render dbt projects as Airflow DAGs and Task Groups. To render a DAG, import ``DbtDag`` and point it to your dbt project.
-
-.. code-block:: python
-
-    from pendulum import datetime
-    from airflow import DAG
-    from cosmos.providers.dbt.dag import DbtDag
-
-    # dag for the project jaffle_shop
-    jaffle_shop = DbtDag(
-        dbt_project_name="jaffle_shop",
-        conn_id="airflow_db",
-        dbt_args={
-            "schema": "public",
-        },
-        dag_id="jaffle_shop",
-        start_date=datetime(2022, 11, 27),
-    )
-
-Simiarly, you can render an Airflow TaskGroups using the ``DbtTaskGroup`` class. Here's an example with the jaffle_shop project:
+You can render an Airflow Task Group using the ``DbtTaskGroup`` class. Here's an example with the jaffle_shop project:
 
 .. code-block:: python
 
     from pendulum import datetime
 
     from airflow import DAG
     from airflow.operators.empty import EmptyOperator
@@ -143,29 +127,33 @@
 
     with DAG(
         dag_id="extract_dag",
         start_date=datetime(2022, 11, 27),
         schedule="@daily",
     ):
 
-        e1 = EmptyOperator(task_id="ingestion_workflow")
+        e1 = EmptyOperator(task_id="pre_dbt")
 
         dbt_tg = DbtTaskGroup(
-            group_id="dbt_tg",
             dbt_project_name="jaffle_shop",
             conn_id="airflow_db",
             dbt_args={
                 "schema": "public",
             },
         )
 
-        e2 = EmptyOperator(task_id="some_extraction")
+        e2 = EmptyOperator(task_id="post_dbt")
 
         e1 >> dbt_tg >> e2
 
+This will generate an Airflow Task Group that looks like this:
+
+.. image:: https://raw.githubusercontent.com/astronomer/astronomer-cosmos/main/docs/jaffle_shop_task_group.png
+
+
 Changelog
 _________
 
 We follow `Semantic Versioning <https://semver.org/>`_ for releases.
 Check `CHANGELOG.rst <https://github.com/astronomer/astronomer-cosmos/blob/main/CHANGELOG.rst>`_
 for the latest changes.
```

