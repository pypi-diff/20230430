# Comparing `tmp/vents-0.0.5.tar.gz` & `tmp/vents-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vents-0.0.5.tar", last modified: Sun Apr 30 13:24:56 2023, max compression
+gzip compressed data, was "vents-0.0.6.tar", last modified: Sun Apr 30 16:19:51 2023, max compression
```

## Comparing `vents-0.0.5.tar` & `vents-0.0.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 13:24:56.908438 vents-0.0.5/
--rw-r--r--   0 mourad     (501) staff       (20)      172 2023-04-30 13:21:50.000000 vents-0.0.5/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-04-30 13:24:56.908567 vents-0.0.5/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1031 2023-04-30 13:24:56.909137 vents-0.0.5/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2695 2023-04-30 13:21:50.000000 vents-0.0.5/setup.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 13:24:56.900783 vents-0.0.5/vents/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 13:21:50.000000 vents-0.0.5/vents/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     5330 2023-04-30 13:21:50.000000 vents-0.0.5/vents/config.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 13:24:56.902852 vents-0.0.5/vents/connections/
--rw-r--r--   0 mourad     (501) staff       (20)      321 2023-04-30 13:21:50.000000 vents-0.0.5/vents/connections/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     2100 2023-04-30 13:21:50.000000 vents-0.0.5/vents/connections/catalog.py
--rw-r--r--   0 mourad     (501) staff       (20)     2888 2023-04-30 13:21:50.000000 vents-0.0.5/vents/connections/connection.py
--rw-r--r--   0 mourad     (501) staff       (20)     3301 2023-04-30 13:21:50.000000 vents-0.0.5/vents/connections/connection_schema.py
--rw-r--r--   0 mourad     (501) staff       (20)      438 2023-04-30 13:21:50.000000 vents-0.0.5/vents/connections/k8s_resource.py
--rw-r--r--   0 mourad     (501) staff       (20)       37 2023-04-30 13:21:50.000000 vents-0.0.5/vents/exceptions.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 13:24:56.905037 vents-0.0.5/vents/notifiers/
--rw-r--r--   0 mourad     (501) staff       (20)      866 2023-04-30 13:21:50.000000 vents-0.0.5/vents/notifiers/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     4589 2023-04-30 13:21:50.000000 vents-0.0.5/vents/notifiers/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1303 2023-04-30 13:21:50.000000 vents-0.0.5/vents/notifiers/discord_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1277 2023-04-30 13:21:50.000000 vents-0.0.5/vents/notifiers/hipchat_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1764 2023-04-30 13:21:50.000000 vents-0.0.5/vents/notifiers/mattermost_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1723 2023-04-30 13:21:50.000000 vents-0.0.5/vents/notifiers/pagerduty_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     2051 2023-04-30 13:21:50.000000 vents-0.0.5/vents/notifiers/slack_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)      372 2023-04-30 13:21:50.000000 vents-0.0.5/vents/notifiers/spec.py
--rw-r--r--   0 mourad     (501) staff       (20)     1847 2023-04-30 13:21:50.000000 vents-0.0.5/vents/notifiers/webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)      233 2023-04-30 13:21:50.000000 vents-0.0.5/vents/pkg.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 13:24:56.905662 vents-0.0.5/vents/providers/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/__init__.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 13:24:56.906509 vents-0.0.5/vents/providers/aws/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/aws/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     3724 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/aws/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1656 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/aws/s3.py
--rw-r--r--   0 mourad     (501) staff       (20)     3456 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/aws/service.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 13:24:56.907434 vents-0.0.5/vents/providers/azure/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/azure/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     2609 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/azure/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1831 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/azure/blob_storage.py
--rw-r--r--   0 mourad     (501) staff       (20)     2251 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/azure/service.py
--rw-r--r--   0 mourad     (501) staff       (20)     1620 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/base.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 13:24:56.908230 vents-0.0.5/vents/providers/gcp/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/gcp/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     3750 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/gcp/base.py
--rw-r--r--   0 mourad     (501) staff       (20)      995 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/gcp/gcs.py
--rw-r--r--   0 mourad     (501) staff       (20)     2513 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/gcp/service.py
--rw-r--r--   0 mourad     (501) staff       (20)     2337 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/kinds.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 13:21:50.000000 vents-0.0.5/vents/py.typed
--rw-r--r--   0 mourad     (501) staff       (20)      256 2023-04-30 13:21:50.000000 vents-0.0.5/vents/settings.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 13:24:56.901819 vents-0.0.5/vents.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-04-30 13:24:56.000000 vents-0.0.5/vents.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1209 2023-04-30 13:24:56.000000 vents-0.0.5/vents.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-30 13:24:56.000000 vents-0.0.5/vents.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)       66 2023-04-30 13:24:56.000000 vents-0.0.5/vents.egg-info/requires.txt
--rw-r--r--   0 mourad     (501) staff       (20)        6 2023-04-30 13:24:56.000000 vents-0.0.5/vents.egg-info/top_level.txt
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 16:19:51.200073 vents-0.0.6/
+-rw-r--r--   0 mourad     (501) staff       (20)      172 2023-04-30 16:18:52.000000 vents-0.0.6/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-04-30 16:19:51.200170 vents-0.0.6/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1031 2023-04-30 16:19:51.200667 vents-0.0.6/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2695 2023-04-30 16:18:52.000000 vents-0.0.6/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 16:19:51.193842 vents-0.0.6/vents/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 16:18:52.000000 vents-0.0.6/vents/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4857 2023-04-30 16:18:52.000000 vents-0.0.6/vents/config.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 16:19:51.195777 vents-0.0.6/vents/connections/
+-rw-r--r--   0 mourad     (501) staff       (20)      321 2023-04-30 16:18:52.000000 vents-0.0.6/vents/connections/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2100 2023-04-30 16:18:52.000000 vents-0.0.6/vents/connections/catalog.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2888 2023-04-30 16:18:52.000000 vents-0.0.6/vents/connections/connection.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3301 2023-04-30 16:18:52.000000 vents-0.0.6/vents/connections/connection_schema.py
+-rw-r--r--   0 mourad     (501) staff       (20)      438 2023-04-30 16:18:52.000000 vents-0.0.6/vents/connections/k8s_resource.py
+-rw-r--r--   0 mourad     (501) staff       (20)       37 2023-04-30 16:18:52.000000 vents-0.0.6/vents/exceptions.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 16:19:51.197362 vents-0.0.6/vents/notifiers/
+-rw-r--r--   0 mourad     (501) staff       (20)      866 2023-04-30 16:18:52.000000 vents-0.0.6/vents/notifiers/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4589 2023-04-30 16:18:52.000000 vents-0.0.6/vents/notifiers/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1303 2023-04-30 16:18:52.000000 vents-0.0.6/vents/notifiers/discord_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1277 2023-04-30 16:18:52.000000 vents-0.0.6/vents/notifiers/hipchat_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1764 2023-04-30 16:18:52.000000 vents-0.0.6/vents/notifiers/mattermost_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1723 2023-04-30 16:18:52.000000 vents-0.0.6/vents/notifiers/pagerduty_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2051 2023-04-30 16:18:52.000000 vents-0.0.6/vents/notifiers/slack_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      372 2023-04-30 16:18:52.000000 vents-0.0.6/vents/notifiers/spec.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1847 2023-04-30 16:18:52.000000 vents-0.0.6/vents/notifiers/webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      233 2023-04-30 16:18:52.000000 vents-0.0.6/vents/pkg.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 16:19:51.197876 vents-0.0.6/vents/providers/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 16:18:52.000000 vents-0.0.6/vents/providers/__init__.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 16:19:51.198554 vents-0.0.6/vents/providers/aws/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 16:18:52.000000 vents-0.0.6/vents/providers/aws/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3724 2023-04-30 16:18:52.000000 vents-0.0.6/vents/providers/aws/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1656 2023-04-30 16:18:52.000000 vents-0.0.6/vents/providers/aws/s3.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3456 2023-04-30 16:18:52.000000 vents-0.0.6/vents/providers/aws/service.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 16:19:51.199256 vents-0.0.6/vents/providers/azure/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 16:18:52.000000 vents-0.0.6/vents/providers/azure/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2609 2023-04-30 16:18:52.000000 vents-0.0.6/vents/providers/azure/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1831 2023-04-30 16:18:52.000000 vents-0.0.6/vents/providers/azure/blob_storage.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2251 2023-04-30 16:18:52.000000 vents-0.0.6/vents/providers/azure/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1620 2023-04-30 16:18:52.000000 vents-0.0.6/vents/providers/base.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 16:19:51.199921 vents-0.0.6/vents/providers/gcp/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 16:18:52.000000 vents-0.0.6/vents/providers/gcp/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3750 2023-04-30 16:18:52.000000 vents-0.0.6/vents/providers/gcp/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)      995 2023-04-30 16:18:52.000000 vents-0.0.6/vents/providers/gcp/gcs.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2513 2023-04-30 16:18:52.000000 vents-0.0.6/vents/providers/gcp/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2337 2023-04-30 16:18:52.000000 vents-0.0.6/vents/providers/kinds.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 16:18:52.000000 vents-0.0.6/vents/py.typed
+-rw-r--r--   0 mourad     (501) staff       (20)      256 2023-04-30 16:18:52.000000 vents-0.0.6/vents/settings.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 16:19:51.194835 vents-0.0.6/vents.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-04-30 16:19:51.000000 vents-0.0.6/vents.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1209 2023-04-30 16:19:51.000000 vents-0.0.6/vents.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-30 16:19:51.000000 vents-0.0.6/vents.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)       66 2023-04-30 16:19:51.000000 vents-0.0.6/vents.egg-info/requires.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        6 2023-04-30 16:19:51.000000 vents-0.0.6/vents.egg-info/top_level.txt
```

### Comparing `vents-0.0.5/PKG-INFO` & `vents-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vents
-Version: 0.0.5
+Version: 0.0.6
 Summary: Open source integrations, alerting, and notification library.
 Home-page: https://github.com/mmourafiq/vents
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

### Comparing `vents-0.0.5/setup.cfg` & `vents-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/setup.py` & `vents-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/config.py` & `vents-0.0.6/vents/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 from typing import Any, List, Optional, Set, Type, Union
 
 from clipped.config.parser import ConfigParser
 from clipped.config.schema import BaseSchemaModel
 from clipped.types import Uri
 from clipped.utils.paths import check_dirname_exists
-from pydantic import ValidationError
 
+from vents.connections import ConnectionCatalog
 from vents.connections.connection import Connection
 from vents.exceptions import VentError
 
 _logger = logging.getLogger("vents.config.reader")
 
 
 class AppConfig(BaseSchemaModel):
@@ -20,14 +20,19 @@
     project_url: Optional[Uri] = ""
     project_icon: Optional[Uri] = ""
     env_prefix: Optional[str] = "VENTS"
     context_path: Optional[str] = ""
     logger: Any = _logger
     exception: Type[Exception] = VentError
     config_parser: Type[ConfigParser] = ConfigParser
+    catalog: Optional[ConnectionCatalog]
+
+    def __init__(self, **data: Any):
+        super().__init__(**data)
+        self.catalog = self.catalog or self.load_connections_catalog()
 
     def get_from_env(self, keys: Union[Set[str], List[str], str]) -> Any:
         """
         Returns a variable from one of the list of keys based on the os.env.
         Args:
             keys: list(str). list of keys to check in the environment
 
@@ -88,60 +93,41 @@
                             return True
                         if value.lower() == "false":
                             return False
                         return value
 
         return None
 
-    def get_connection_context_path_env_name(self, name: str) -> str:
-        env_name = "CONNECTION_CONTEXT_PATH_".format(name.upper())
+    def get_connections_catalog_env_name(self) -> str:
+        env_name = "CONNECTIONS_CATALOG"
         if self.env_prefix:
             env_name = "{}_{}".format(self.env_prefix, env_name)
         return env_name
 
-    def get_connection_schema_env_name(self, name: str) -> str:
-        env_name = "CONNECTION_SCHEMA_".format(name.upper())
-        if self.env_prefix:
-            env_name = "{}_{}".format(self.env_prefix, env_name)
-        return env_name
-
-    def get_connection_context_path(self, name: Optional[str]) -> Optional[str]:
-        """Checks if a connection has a mount path exported"""
-        if not name:
+    @staticmethod
+    def get_connections_catalog(
+        connections: Optional[List[Connection]],
+    ) -> Optional[ConnectionCatalog]:
+        if not connections:
+            return None
+        return ConnectionCatalog(connections=connections)
+
+    def load_connections_catalog(self) -> Optional[ConnectionCatalog]:
+        catalog_env_name = self.get_connections_catalog_env_name()
+        connections_catalog = os.environ.get(catalog_env_name)
+        if not connections_catalog:
             return None
+        return ConnectionCatalog.read(connections_catalog, config_type=".json")
 
-        context_path = os.environ.get(self.get_connection_context_path_env_name(name))
-        if not context_path:
-            return None
-
-        if not os.path.exists(context_path):
-            self.logger.warning(
-                "A connection path was found for {}, "
-                "but a path the {} does not exist.".format(name, context_path)
-            )
-            return None
-        return context_path
-
-    def get_connection_type(self, name: Optional[str]) -> Optional[Connection]:
+    def get_connection_for(self, name: Optional[str]) -> Optional[Connection]:
         """Checks if a connection has a mount path exported"""
-        if not name:
+        if not name or not self.catalog:
             return None
 
-        spec = os.environ.get(self.get_connection_schema_env_name(name))
-        if not spec:
-            return None
-
-        try:
-            return Connection.read(spec, config_type=".json")
-        except ValidationError as e:
-            self.logger.warning(
-                "A connection spec was found for {}, "
-                "but the reading the spec raised an error {}.".format(name, repr(e))
-            )
-            return None
+        return self.catalog.connections_by_names.get(name)
 
     def read_keys(self, context_paths: List[str], keys: List[str]) -> Optional[Any]:
         """Returns a variable by checking first a context path and then in the environment."""
         keys = (
             {k.lower() for k in keys}
             | {k.upper() for k in keys}
             | {"".join(k.lower().split("_")) for k in keys}
```

### Comparing `vents-0.0.5/vents/connections/catalog.py` & `vents-0.0.6/vents/connections/catalog.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/connections/connection.py` & `vents-0.0.6/vents/connections/connection.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/connections/connection_schema.py` & `vents-0.0.6/vents/connections/connection_schema.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/notifiers/__init__.py` & `vents-0.0.6/vents/notifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/notifiers/base.py` & `vents-0.0.6/vents/notifiers/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/notifiers/discord_webhook.py` & `vents-0.0.6/vents/notifiers/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/notifiers/hipchat_webhook.py` & `vents-0.0.6/vents/notifiers/hipchat_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/notifiers/mattermost_webhook.py` & `vents-0.0.6/vents/notifiers/mattermost_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/notifiers/pagerduty_webhook.py` & `vents-0.0.6/vents/notifiers/pagerduty_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/notifiers/slack_webhook.py` & `vents-0.0.6/vents/notifiers/slack_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/notifiers/webhook.py` & `vents-0.0.6/vents/notifiers/webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/providers/aws/base.py` & `vents-0.0.6/vents/providers/aws/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/providers/aws/s3.py` & `vents-0.0.6/vents/providers/aws/s3.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/providers/aws/service.py` & `vents-0.0.6/vents/providers/aws/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/providers/azure/base.py` & `vents-0.0.6/vents/providers/azure/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/providers/azure/blob_storage.py` & `vents-0.0.6/vents/providers/azure/blob_storage.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/providers/azure/service.py` & `vents-0.0.6/vents/providers/azure/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/providers/base.py` & `vents-0.0.6/vents/providers/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/providers/gcp/base.py` & `vents-0.0.6/vents/providers/gcp/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/providers/gcp/gcs.py` & `vents-0.0.6/vents/providers/gcp/gcs.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/providers/gcp/service.py` & `vents-0.0.6/vents/providers/gcp/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents/providers/kinds.py` & `vents-0.0.6/vents/providers/kinds.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.5/vents.egg-info/PKG-INFO` & `vents-0.0.6/vents.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vents
-Version: 0.0.5
+Version: 0.0.6
 Summary: Open source integrations, alerting, and notification library.
 Home-page: https://github.com/mmourafiq/vents
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

### Comparing `vents-0.0.5/vents.egg-info/SOURCES.txt` & `vents-0.0.6/vents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

