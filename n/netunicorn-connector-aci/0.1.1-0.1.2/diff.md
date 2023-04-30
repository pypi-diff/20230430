# Comparing `tmp/netunicorn-connector-aci-0.1.1.tar.gz` & `tmp/netunicorn-connector-aci-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-connector-aci-0.1.1.tar", last modified: Wed Mar 22 22:59:08 2023, max compression
+gzip compressed data, was "netunicorn-connector-aci-0.1.2.tar", last modified: Sun Apr 30 06:58:59 2023, max compression
```

## Comparing `netunicorn-connector-aci-0.1.1.tar` & `netunicorn-connector-aci-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:59:08.363192 netunicorn-connector-aci-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-22 22:58:58.000000 netunicorn-connector-aci-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-22 22:59:08.363192 netunicorn-connector-aci-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-03-22 22:58:58.000000 netunicorn-connector-aci-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-22 22:58:58.000000 netunicorn-connector-aci-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 22:59:08.363192 netunicorn-connector-aci-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:59:08.363192 netunicorn-connector-aci-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:59:08.363192 netunicorn-connector-aci-0.1.1/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:59:08.363192 netunicorn-connector-aci-0.1.1/src/netunicorn/director/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:59:08.363192 netunicorn-connector-aci-0.1.1/src/netunicorn/director/infrastructure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:59:08.363192 netunicorn-connector-aci-0.1.1/src/netunicorn/director/infrastructure/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 22:58:58.000000 netunicorn-connector-aci-0.1.1/src/netunicorn/director/infrastructure/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-03-22 22:58:58.000000 netunicorn-connector-aci-0.1.1/src/netunicorn/director/infrastructure/connectors/aci.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:59:08.363192 netunicorn-connector-aci-0.1.1/src/netunicorn_connector_aci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-22 22:59:08.000000 netunicorn-connector-aci-0.1.1/src/netunicorn_connector_aci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-22 22:59:08.000000 netunicorn-connector-aci-0.1.1/src/netunicorn_connector_aci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 22:59:08.000000 netunicorn-connector-aci-0.1.1/src/netunicorn_connector_aci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-22 22:59:08.000000 netunicorn-connector-aci-0.1.1/src/netunicorn_connector_aci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-22 22:59:08.000000 netunicorn-connector-aci-0.1.1/src/netunicorn_connector_aci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:58:59.303641 netunicorn-connector-aci-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-30 06:58:47.000000 netunicorn-connector-aci-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-30 06:58:59.303641 netunicorn-connector-aci-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-30 06:58:47.000000 netunicorn-connector-aci-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-30 06:58:47.000000 netunicorn-connector-aci-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 06:58:59.303641 netunicorn-connector-aci-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:58:59.303641 netunicorn-connector-aci-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:58:59.303641 netunicorn-connector-aci-0.1.2/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:58:59.303641 netunicorn-connector-aci-0.1.2/src/netunicorn/director/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:58:59.303641 netunicorn-connector-aci-0.1.2/src/netunicorn/director/infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:58:59.303641 netunicorn-connector-aci-0.1.2/src/netunicorn/director/infrastructure/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:58:47.000000 netunicorn-connector-aci-0.1.2/src/netunicorn/director/infrastructure/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-04-30 06:58:47.000000 netunicorn-connector-aci-0.1.2/src/netunicorn/director/infrastructure/connectors/aci.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:58:59.303641 netunicorn-connector-aci-0.1.2/src/netunicorn_connector_aci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-30 06:58:59.000000 netunicorn-connector-aci-0.1.2/src/netunicorn_connector_aci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-30 06:58:59.000000 netunicorn-connector-aci-0.1.2/src/netunicorn_connector_aci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 06:58:59.000000 netunicorn-connector-aci-0.1.2/src/netunicorn_connector_aci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-30 06:58:59.000000 netunicorn-connector-aci-0.1.2/src/netunicorn_connector_aci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 06:58:59.000000 netunicorn-connector-aci-0.1.2/src/netunicorn_connector_aci.egg-info/top_level.txt
```

### Comparing `netunicorn-connector-aci-0.1.1/LICENSE` & `netunicorn-connector-aci-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-aci-0.1.1/PKG-INFO` & `netunicorn-connector-aci-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-aci
-Version: 0.1.1
+Version: 0.1.2
 Summary: Azure Container Instances connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `netunicorn-connector-aci-0.1.1/README.md` & `netunicorn-connector-aci-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-aci-0.1.1/pyproject.toml` & `netunicorn-connector-aci-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 name = "netunicorn-connector-aci"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "Azure Container Instances connector for netunicorn"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["netunicorn"]
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "netunicorn-director-infrastructure >= 0.2.0",
-    "netunicorn-base >= 0.2.0",
+    "netunicorn-base >= 0.3.0",
     "pyyaml",
     "returns",
     "azure-mgmt-resource",
     "azure-mgmt-containerinstance",
     "azure-identity",
 ]
```

### Comparing `netunicorn-connector-aci-0.1.1/src/netunicorn/director/infrastructure/connectors/aci.py` & `netunicorn-connector-aci-0.1.2/src/netunicorn/director/infrastructure/connectors/aci.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,23 +14,27 @@
 from netunicorn.base.architecture import Architecture
 
 from netunicorn.base.deployment import Deployment
 from netunicorn.base.environment_definitions import DockerImage
 from netunicorn.base.nodes import Node, UncountableNodePool
 from returns.result import Result, Success, Failure
 
-from netunicorn.director.infrastructure.connectors.protocol import (
+from netunicorn.director.base.connectors.protocol import (
     NetunicornConnectorProtocol,
 )
-from netunicorn.director.infrastructure.connectors.types import StopExecutorRequest
+from netunicorn.director.base.connectors.types import StopExecutorRequest
 
 
-class AzureContainerInstances(NetunicornConnectorProtocol):  # type: ignore
+class AzureContainerInstances(NetunicornConnectorProtocol):
     def __init__(
-        self, connector_name: str, config_file: str | None, netunicorn_gateway: str, logger: Optional[logging.Logger] = None,
+        self,
+        connector_name: str,
+        config_file: str | None,
+        netunicorn_gateway: str,
+        logger: Optional[logging.Logger] = None,
     ):
         self.connector_name = connector_name
         self.netunicorn_gateway = netunicorn_gateway
 
         if config_file is not None:
             with open(config_file, "r") as f:
                 self.config = yaml.safe_load(f)
@@ -62,37 +66,37 @@
 
         # noinspection PyTypeChecker
         self.client = ContainerInstanceManagementClient(
             credential=ClientSecretCredential(
                 tenant_id=self.azure_tenant_id,
                 client_id=self.azure_client_id,
                 client_secret=self.azure_client_secret,
-            ), subscription_id=self.subscription_id
+            ),
+            subscription_id=self.subscription_id,
         )
 
         if not logger:
             logging.basicConfig()
             logger = logging.getLogger(__name__)
             logger.setLevel(logging.INFO)
 
         self.logger = logger
 
     async def __cleaner(self) -> NoReturn:
         """
-        This is a temporary crutch for removing container groups for finished experiments.
-        Yes, I'm ashamed of myself.
-        But it's better than nothing for now, I'll implement a proper system-level finalization later.
-
-        Theoretically, Azure Container Instances wouldn't charge for the container groups that are not running,
-        but just in case.
+        This is a backup cleaner that will delete all container groups that are not running.
+        These groups should be deleted by cleanup, but something can go wrong and we want
+        to avoid having orphaned container groups.
         """
         self.logger.info("Starting Azure Container Instances cleaner")
         while True:
             try:
-                container_groups: Iterable[ContainerGroup] = self.client.container_groups.list_by_resource_group(
+                container_groups: Iterable[
+                    ContainerGroup
+                ] = self.client.container_groups.list_by_resource_group(
                     self.resource_group_name
                 )
 
                 # if all containers in the group are not running, delete the group
                 for group in container_groups:
                     group_name: str = group.name  # type: ignore
                     group_containers: list[Container] = group.containers  # type: ignore
@@ -122,38 +126,51 @@
 
     async def health(self) -> Tuple[bool, str]:
         return True, "Cannot check if Azure Container Instances is healthy"
 
     async def shutdown(self) -> None:
         pass
 
-    async def get_nodes(self, username: str, *args, **kwargs) -> UncountableNodePool:
+    async def get_nodes(
+            self,
+            username: str,
+            authentication_context: Optional[dict[str, str]] = None,
+            *args: Any,
+            **kwargs: Any,
+    ) -> UncountableNodePool:
         available_node_types = [
             Node(
                 name="aci-",
                 architecture=Architecture.LINUX_AMD64,
                 properties={
                     "memory_in_gb": 1,
                     "cpu": 1,
-                }
+                },
             )
         ]
         return UncountableNodePool(node_template=available_node_types)
 
     async def deploy(
-        self, username: str, experiment_id: str, deployments: list[Deployment], *args, **kwargs
-    ) -> dict[str, Result[None, str]]:
+        self,
+        username: str,
+        experiment_id: str,
+        deployments: list[Deployment],
+        deployment_context: Optional[dict[str, str]],
+        authentication_context: Optional[dict[str, str]] = None,
+        *args: Any,
+        **kwargs: Any,
+    ) -> dict[str, Result[Optional[str], str]]:
         """
         Azure Container Instances automatically starts the container when it is created
         (seriously: https://stackoverflow.com/questions/67385581/deploying-azure-container-s-without-running-them),
         so this function only checks that all deployments are of DockerImage type,
         as it is the only type supported by Azure Container Instances.
         """
 
-        result: dict[str, Result[None, str]] = {}
+        result: dict[str, Result[Optional[str], str]] = {}
         for deployment in deployments:
             if not deployment.prepared:
                 result[deployment.executor_id] = Failure("Deployment is not prepared")
                 continue
             if not isinstance(deployment.environment_definition, DockerImage):
                 result[deployment.executor_id] = Failure(
                     "Azure Container Instances only supports DockerImage deployments"
@@ -165,18 +182,27 @@
                 )
                 continue
             result[deployment.executor_id] = Success(None)
 
         return result
 
     async def execute(
-        self, username: str, experiment_id: str, deployments: list[Deployment], *args, **kwargs
-    ) -> dict[str, Result[None, str]]:
+        self,
+        username: str,
+        experiment_id: str,
+        deployments: list[Deployment],
+        execution_context: Optional[dict[str, str]],
+        authentication_context: Optional[dict[str, str]] = None,
+        *args: Any,
+        **kwargs: Any,
+    ) -> dict[str, Result[Optional[str], str]]:
         container_groups: dict[str, dict[str, Any]] = {}
         for deployment in deployments:
+            if not isinstance(deployment.environment_definition, DockerImage):
+                continue
             deployment.environment_definition.runtime_context.environment_variables[
                 "NETUNICORN_EXECUTOR_ID"
             ] = deployment.executor_id
             deployment.environment_definition.runtime_context.environment_variables[
                 "NETUNICORN_GATEWAY_ENDPOINT"
             ] = self.netunicorn_gateway
             deployment.environment_definition.runtime_context.environment_variables[
@@ -192,33 +218,40 @@
                 "restart_policy": "Never",
                 "os_type": "Linux",
                 "containers": [
                     {
                         "name": deployment.executor_id,
                         "image": deployment.environment_definition.image,
                         "environment_variables": environment_variables,
-                        "resources": {"requests": {
-                            "memory_in_gb": deployment.node.properties.get("memory_in_gb", 1),
-                            "cpu": deployment.node.properties.get("cpu", 1),
-                        }},
+                        "resources": {
+                            "requests": {
+                                "memory_in_gb": deployment.node.properties.get(
+                                    "memory_in_gb", 1
+                                ),
+                                "cpu": deployment.node.properties.get("cpu", 1),
+                            }
+                        },
                     }
                 ],
             }
 
         self.logger.info(f"Creating container groups: {container_groups}")
 
         # noinspection PyTypeChecker
         # trust me
-        values: tuple[Exception | Result[None, str], ...] = await asyncio.gather(*[
-            self._create_container_group(key, value) for key, value in container_groups.items()  # type: ignore
-        ], return_exceptions=True)
+        values: tuple[Exception | Result[None, str], ...] = await asyncio.gather(
+            *[
+                self._create_container_group(key, value) for key, value in container_groups.items()  # type: ignore
+            ],
+            return_exceptions=True,
+        )
 
         results = {}
         for i, key in enumerate(container_groups.keys()):
-            value: Exception | Result[None, str] = values[i]
+            value: Exception | Result[Optional[str], str] = values[i]
             if isinstance(value, Exception):
                 value = Failure(str(value))
             results[key] = value
 
         return results
 
     async def _create_container_group(
@@ -235,11 +268,38 @@
             await loop.run_in_executor(None, request.result)
             return Success(None)
         except Exception as e:
             self.logger.error(f"Error while creating container group: {e}")
             return Failure(str(e))
 
     async def stop_executors(
-        self, username: str, requests_list: list[StopExecutorRequest], *args, **kwargs
-    ) -> dict[str, Result[None, str]]:
+        self,
+        username: str,
+        requests_list: list[StopExecutorRequest],
+        cancellation_context: Optional[dict[str, str]],
+        authentication_context: Optional[dict[str, str]] = None,
+        *args: Any,
+        **kwargs: Any,
+    ) -> dict[str, Result[Optional[str], str]]:
         self.logger.warning("Stop executors called, but not implemented")
-        return {request["executor_id"]: Failure("Stop executor is not implemented") for request in requests_list}
+        return {
+            request["executor_id"]: Failure("Stop executor is not implemented")
+            for request in requests_list
+        }
+
+    async def cleanup(
+        self,
+        experiment_id: str,
+        deployments: list[Deployment],
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
+
+        for deployment in deployments:
+            # try to delete the container group
+            try:
+                self.client.container_groups.begin_delete(
+                    resource_group_name=self.resource_group_name,
+                    container_group_name=deployment.executor_id,
+                )
+            except Exception as e:
+                self.logger.error(f"Error while deleting container group: {e}")
```

### Comparing `netunicorn-connector-aci-0.1.1/src/netunicorn_connector_aci.egg-info/PKG-INFO` & `netunicorn-connector-aci-0.1.2/src/netunicorn_connector_aci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-aci
-Version: 0.1.1
+Version: 0.1.2
 Summary: Azure Container Instances connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

