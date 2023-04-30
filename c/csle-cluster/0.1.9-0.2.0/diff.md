# Comparing `tmp/csle_cluster-0.1.9.tar.gz` & `tmp/csle_cluster-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_cluster-0.1.9.tar", last modified: Tue Mar 21 08:10:49 2023, max compression
+gzip compressed data, was "csle_cluster-0.2.0.tar", last modified: Sun Apr 30 12:38:13 2023, max compression
```

## Comparing `csle_cluster-0.1.9.tar` & `csle_cluster-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:49.085291 csle_cluster-0.1.9/
--rw-rw-r--   0 kim       (1000) kim       (1000)      804 2023-03-21 08:10:49.085291 csle_cluster-0.1.9/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     4256 2023-03-04 16:33:53.000000 csle_cluster-0.1.9/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      672 2023-02-13 15:55:11.000000 csle_cluster-0.1.9/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1406 2023-03-21 08:10:49.085291 csle_cluster-0.1.9/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-02-13 15:55:11.000000 csle_cluster-0.1.9/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:49.077291 csle_cluster-0.1.9/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:49.081291 csle_cluster-0.1.9/src/csle_cluster/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-02-13 15:55:11.000000 csle_cluster-0.1.9/src/csle_cluster/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 csle_cluster-0.1.9/src/csle_cluster/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:49.081291 csle_cluster-0.1.9/src/csle_cluster/cluster_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-02-13 15:55:11.000000 csle_cluster-0.1.9/src/csle_cluster/cluster_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   222811 2023-03-21 06:33:58.000000 csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   260635 2023-03-21 08:07:44.000000 csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   189531 2023-03-21 06:33:58.000000 csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   339988 2023-03-17 07:49:22.000000 csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   185021 2023-03-21 06:33:58.000000 csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   182935 2023-03-17 07:49:22.000000 csle_cluster-0.1.9/src/csle_cluster/cluster_manager/query_cluster_manager.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:49.081291 csle_cluster-0.1.9/src/csle_cluster/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-03 14:11:41.000000 csle_cluster-0.1.9/src/csle_cluster/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      375 2023-03-17 07:49:22.000000 csle_cluster-0.1.9/src/csle_cluster/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:49.081291 csle_cluster-0.1.9/src/csle_cluster.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      804 2023-03-21 08:10:48.000000 csle_cluster-0.1.9/src/csle_cluster.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      805 2023-03-21 08:10:49.000000 csle_cluster-0.1.9/src/csle_cluster.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:10:48.000000 csle_cluster-0.1.9/src/csle_cluster.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-04 13:33:55.000000 csle_cluster-0.1.9/src/csle_cluster.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      251 2023-03-21 08:10:48.000000 csle_cluster-0.1.9/src/csle_cluster.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       13 2023-03-21 08:10:49.000000 csle_cluster-0.1.9/src/csle_cluster.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:38:13.032987 csle_cluster-0.2.0/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      804 2023-04-30 12:38:13.032987 csle_cluster-0.2.0/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4256 2023-03-28 14:03:22.000000 csle_cluster-0.2.0/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      672 2023-03-28 14:03:22.000000 csle_cluster-0.2.0/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1406 2023-04-30 12:38:13.032987 csle_cluster-0.2.0/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_cluster-0.2.0/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:38:13.024987 csle_cluster-0.2.0/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:38:13.024987 csle_cluster-0.2.0/src/csle_cluster/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_cluster-0.2.0/src/csle_cluster/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-04-30 12:35:57.000000 csle_cluster-0.2.0/src/csle_cluster/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:38:13.032987 csle_cluster-0.2.0/src/csle_cluster/cluster_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_cluster-0.2.0/src/csle_cluster/cluster_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   229247 2023-04-18 12:47:23.000000 csle_cluster-0.2.0/src/csle_cluster/cluster_manager/cluster_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   269065 2023-04-01 09:31:08.000000 csle_cluster-0.2.0/src/csle_cluster/cluster_manager/cluster_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   197343 2023-03-28 14:03:22.000000 csle_cluster-0.2.0/src/csle_cluster/cluster_manager/cluster_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   349502 2023-03-28 14:03:22.000000 csle_cluster-0.2.0/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   202990 2023-03-28 14:03:22.000000 csle_cluster-0.2.0/src/csle_cluster/cluster_manager/cluster_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   188175 2023-04-18 12:48:07.000000 csle_cluster-0.2.0/src/csle_cluster/cluster_manager/query_cluster_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:38:13.032987 csle_cluster-0.2.0/src/csle_cluster/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_cluster-0.2.0/src/csle_cluster/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      375 2023-03-28 14:03:22.000000 csle_cluster-0.2.0/src/csle_cluster/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:38:13.024987 csle_cluster-0.2.0/src/csle_cluster.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      804 2023-04-30 12:38:12.000000 csle_cluster-0.2.0/src/csle_cluster.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      805 2023-04-30 12:38:13.000000 csle_cluster-0.2.0/src/csle_cluster.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-04-30 12:38:12.000000 csle_cluster-0.2.0/src/csle_cluster.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-04 13:33:55.000000 csle_cluster-0.2.0/src/csle_cluster.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      251 2023-04-30 12:38:12.000000 csle_cluster-0.2.0/src/csle_cluster.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       13 2023-04-30 12:38:12.000000 csle_cluster-0.2.0/src/csle_cluster.egg-info/top_level.txt
```

### Comparing `csle_cluster-0.1.9/PKG-INFO` & `csle_cluster-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_cluster
-Version: 0.1.9
+Version: 0.2.0
 Summary: Scripts for cluster management in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cluster-0.1.9/README.md` & `csle_cluster-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.1.9/pyproject.toml` & `csle_cluster-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.1.9/setup.cfg` & `csle_cluster-0.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	grpcio>=1.27.2
 	grpcio-tools>=1.27.2
-	csle-collector>=0.1.9
-	csle-common>=0.1.9
-	csle-ryu>=0.1.9
+	csle-collector>=0.2.0
+	csle-common>=0.2.0
+	csle-ryu>=0.2.0
 python_requires = >=3.5
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_controller.py` & `csle_cluster-0.2.0/src/csle_cluster/cluster_manager/cluster_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -3618,15 +3618,15 @@
                 stub=stub, ip_first_octet=ip_first_octet, emulation=emulation)
             return operation_outcome_dto
 
     @staticmethod
     def run_emulation(execution: EmulationExecution, physical_servers: List[str],
                       no_traffic: bool = False, no_clients: bool = False):
         ip = physical_servers[0]
-        steps = 39
+        steps = 41
         if no_traffic:
             steps = steps - 1
         if no_clients:
             execution.emulation_env_config.traffic_config.client_population_config = \
                 execution.emulation_env_config.traffic_config.client_population_config.no_clients()
 
         current_step = 1
@@ -3635,14 +3635,15 @@
             Logger.__call__().get_logger().info(f"-- Starting containers of "
                                                 f"emulation: {execution.emulation_env_config.name} "
                                                 f"on server: {ip}--")
             ClusterController.start_containers_in_execution(ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
                                                             emulation=execution.emulation_name,
                                                             ip_first_octet=execution.ip_first_octet)
 
+        current_step += 1
         Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Creating networks for emulation: "
                                             f"{execution.emulation_env_config.name} --")
         config = MetastoreFacade.get_config(id=1)
         for node in config.cluster_config.cluster_nodes:
             if node.leader:
                 ClusterController.create_emulation_networks(
                     ip=node.ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT, emulation=execution.emulation_name,
@@ -3661,22 +3662,33 @@
         # Update execution config with the new IPs for the docker-gw
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=execution.ip_first_octet,
                                                             emulation_name=execution.emulation_name)
         execution = EmulationEnvController.update_execution_config_w_docker_gw_bridge_ip(
             execution=execution)
 
         current_step += 1
-        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Install csle-collector --")
+        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Installing python libraries --")
         for ip in physical_servers:
             Logger.__call__().get_logger().info(f"Installing libraries on containers in "
                                                 f"emulation {execution.emulation_env_config.name} "
                                                 f"deployed on server: {ip}")
             ClusterController.install_libraries(
                 ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
                 emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
+
+        current_step += 1
+        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Start Spark instances --")
+        for ip in physical_servers:
+            Logger.__call__().get_logger().info(f"-- Starting spark instances of"
+                                                f"emulation {execution.emulation_env_config.name}"
+                                                f" on server: {ip}--")
+            ClusterController.start_spark_servers(
+                ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT, emulation=execution.emulation_name,
+                ip_first_octet=execution.ip_first_octet)
+
         current_step += 1
         Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Apply kafka config --")
         for ip in physical_servers:
             if execution.emulation_env_config.kafka_config.container.physical_host_ip == ip:
                 Logger.__call__().get_logger().info(f"Applying Kafka config to containers in "
                                                     f"emulation: {execution.emulation_env_config.name} on server: {ip}")
                 ClusterController.apply_kafka_config(ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
@@ -3711,37 +3723,37 @@
             Logger.__call__().get_logger().info(f"Creating OVS switches on containers in "
                                                 f"emulation: {execution.emulation_env_config.name} on server: {ip}")
             ClusterController.create_ovs_switches(
                 ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
                 emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
 
         current_step += 1
-        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Tests connections with Ping --")
+        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Update OVS switches --")
         for ip in physical_servers:
-            Logger.__call__().get_logger().info(f"Testing Ping connections for containers in "
+            Logger.__call__().get_logger().info(f"Updating OVS switches on containers in "
                                                 f"emulation: {execution.emulation_env_config.name} on server: {ip}")
-            ClusterController.ping_execution(
+            ClusterController.create_ovs_switches(
                 ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
                 emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
 
         current_step += 1
-        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Configure OVS switches --")
+        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Creating topology --")
         for ip in physical_servers:
-            Logger.__call__().get_logger().info(f"Configuring OVS switches on containers in "
+            Logger.__call__().get_logger().info(f"Creating topology on containers in "
                                                 f"emulation: {execution.emulation_env_config.name} on server: {ip}")
-            ClusterController.configure_ovs(
+            ClusterController.create_topology(
                 ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
                 emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
 
         current_step += 1
-        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Tests connections with Ping --")
+        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Configure OVS switches --")
         for ip in physical_servers:
-            Logger.__call__().get_logger().info(f"Testing ping connections on containers "
-                                                f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
-            ClusterController.ping_execution(
+            Logger.__call__().get_logger().info(f"Configuring OVS switches on containers in "
+                                                f"emulation: {execution.emulation_env_config.name} on server: {ip}")
+            ClusterController.configure_ovs(
                 ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
                 emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
 
         current_step += 1
         Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Start SDN controller monitor --")
         if execution.emulation_env_config.sdn_controller_config is not None:
             for ip in physical_servers:
@@ -3777,23 +3789,14 @@
             Logger.__call__().get_logger().info(f"Creating flags on containers in "
                                                 f"emulation: {execution.emulation_env_config.name} on server: {ip}")
             ClusterController.create_flags(
                 ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
                 emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
 
         current_step += 1
-        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Creating topology --")
-        for ip in physical_servers:
-            Logger.__call__().get_logger().info(f"Creating topology on containers in "
-                                                f"emulation: {execution.emulation_env_config.name} on server: {ip}")
-            ClusterController.create_topology(
-                ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
-                emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
-
-        current_step += 1
         Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Starting traffic managers --")
         for ip in physical_servers:
             Logger.__call__().get_logger().info(f"Starting traffic managers on containers "
                                                 f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
             ClusterController.start_traffic_managers(
                 ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
                 emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
@@ -3938,45 +3941,45 @@
         current_step += 1
         Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Starting filebeats --")
         for ip in physical_servers:
             Logger.__call__().get_logger().info(f"Starting filebeats on containers "
                                                 f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
             ClusterController.start_filebeats(
                 ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
-                emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
+                emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet, initial_start=True)
         time.sleep(10)
 
         current_step += 1
         Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Starting packetbeats --")
         for ip in physical_servers:
             Logger.__call__().get_logger().info(f"Starting packetbeats on containers "
                                                 f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
             ClusterController.start_packetbeats(
                 ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
-                emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
+                emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet, initial_start=True)
         time.sleep(10)
 
         current_step += 1
         Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Starting metricbeats --")
         for ip in physical_servers:
             Logger.__call__().get_logger().info(f"Starting metricbeats on containers "
                                                 f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
             ClusterController.start_metricbeats(
                 ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
-                emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
+                emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet, initial_start=True)
         time.sleep(10)
 
         current_step += 1
         Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Starting heartbeats --")
         for ip in physical_servers:
             Logger.__call__().get_logger().info(f"Starting heartbeats on containers "
                                                 f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
             ClusterController.start_heartbeats(
                 ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
-                emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
+                emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet, initial_start=True)
         time.sleep(10)
 
         current_step += 1
         Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Starting the Docker stats monitor --")
         for ip in physical_servers:
             Logger.__call__().get_logger().info(f"Starting the Docker statsmanager on server: {ip}")
             ClusterController.start_docker_statsmanager(
@@ -4040,14 +4043,25 @@
         Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Starting Flask --")
         for ip in physical_servers:
             Logger.__call__().get_logger().info(f"Starting Flask on server: {ip}")
             ClusterController.start_flask(
                 ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT)
         time.sleep(2)
 
+        current_step += 1
+        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Starting the Host managers "
+                                            f"and host monitors --")
+        for ip in physical_servers:
+            Logger.__call__().get_logger().info(f"Starting the host managers on containers "
+                                                f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
+            ClusterController.start_host_managers(
+                ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
+                emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
+        time.sleep(10)
+
     @staticmethod
     def get_ryu_manager_logs(ip: str, port: int, emulation: str, ip_first_octet: int) \
             -> Dict[str, Any]:
         """
         Gets the logs of the Ryu manager of a specific execution
 
         :param ip: the ip of the physical node
@@ -4349,7 +4363,119 @@
         with grpc.insecure_channel(f'{ip}:{port}') as channel:
             stub = csle_cluster.cluster_manager.cluster_manager_pb2_grpc.ClusterManagerStub(channel)
             time_series_data_dto = csle_cluster.cluster_manager.query_cluster_manager.get_execution_time_series_data(
                 stub=stub, emulation=emulation, ip_first_octet=ip_first_octet, minutes=minutes
             )
             return ClusterManagerUtil.convert_emulation_metrics_time_series_dto_reverse(
                 time_series_dto=time_series_data_dto)
+
+    @staticmethod
+    def start_spark_servers(ip: str, port: int, emulation: str, ip_first_octet: int) \
+            -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
+        """
+        Sends a request to start the Spark servers of a given execution
+
+        :param ip: the ip of the node where to start the Snort IDSes
+        :param port: the port of the cluster manager
+        :param emulation: the emulation of the execution
+        :param ip_first_octet: the ID of the execution
+        :return: The operation outcome
+        """
+        # Open a gRPC session
+        with grpc.insecure_channel(f'{ip}:{port}') as channel:
+            stub = csle_cluster.cluster_manager.cluster_manager_pb2_grpc.ClusterManagerStub(channel)
+            operation_outcome_dto = csle_cluster.cluster_manager.query_cluster_manager.start_spark_servers(
+                stub=stub, emulation=emulation, ip_first_octet=ip_first_octet
+            )
+            return operation_outcome_dto
+
+    @staticmethod
+    def stop_spark_servers(ip: str, port: int, emulation: str, ip_first_octet: int) \
+            -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
+        """
+        Sends a request to stop the Spark servers of a given execution
+
+        :param ip: the ip of the node where to start the Snort IDSes
+        :param port: the port of the cluster manager
+        :param emulation: the emulation of the execution
+        :param ip_first_octet: the ID of the execution
+        :return: The operation outcome
+        """
+        # Open a gRPC session
+        with grpc.insecure_channel(f'{ip}:{port}') as channel:
+            stub = csle_cluster.cluster_manager.cluster_manager_pb2_grpc.ClusterManagerStub(channel)
+            operation_outcome_dto = csle_cluster.cluster_manager.query_cluster_manager.stop_spark_servers(
+                stub=stub, emulation=emulation, ip_first_octet=ip_first_octet
+            )
+            return operation_outcome_dto
+
+    @staticmethod
+    def start_spark_server(ip: str, port: int, emulation: str, ip_first_octet: int, container_ip: str) \
+            -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
+        """
+        Starts the Spark server on a specific container in a specific execution
+
+        :param ip: the ip of the physical node
+        :param port: the port of the cluster manager
+        :param emulation: the emulation of the execution
+        :param ip_first_octet: the ID of the execution
+        :param container_ip: the ip of the container
+        :return: The operation outcome
+        """
+        # Open a gRPC session
+        with grpc.insecure_channel(f'{ip}:{port}') as channel:
+            stub = csle_cluster.cluster_manager.cluster_manager_pb2_grpc.ClusterManagerStub(channel)
+            operation_outcome_dto = csle_cluster.cluster_manager.query_cluster_manager.start_spark_server(
+                stub=stub, ip_first_octet=ip_first_octet, emulation=emulation, container_ip=container_ip)
+            return operation_outcome_dto
+
+    @staticmethod
+    def stop_spark_server(ip: str, port: int, emulation: str, ip_first_octet: int, container_ip: str) \
+            -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
+        """
+        Stops the Spark server on a specific container in a specific execution
+
+        :param ip: the ip of the physical node
+        :param port: the port of the cluster manager
+        :param emulation: the emulation of the execution
+        :param ip_first_octet: the ID of the execution
+        :param container_ip: the ip of the container
+        :return: The operation outcome
+        """
+        # Open a gRPC session
+        with grpc.insecure_channel(f'{ip}:{port}') as channel:
+            stub = csle_cluster.cluster_manager.cluster_manager_pb2_grpc.ClusterManagerStub(channel)
+            operation_outcome_dto = csle_cluster.cluster_manager.query_cluster_manager.stop_spark_server(
+                stub=stub, ip_first_octet=ip_first_octet, emulation=emulation, container_ip=container_ip)
+            return operation_outcome_dto
+
+    @staticmethod
+    def check_pid(ip: str, port: int, pid: int) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
+        """
+        Checks the status of a PID of a specific server
+
+        :param ip: the ip of the physical node
+        :param port: the port of the cluster manager
+        :param pid: the PID to check
+        :return: The operation outcome
+        """
+        # Open a gRPC session
+        with grpc.insecure_channel(f'{ip}:{port}') as channel:
+            stub = csle_cluster.cluster_manager.cluster_manager_pb2_grpc.ClusterManagerStub(channel)
+            operation_outcome_dto = csle_cluster.cluster_manager.query_cluster_manager.check_pid(stub=stub, pid=pid)
+            return operation_outcome_dto
+
+    @staticmethod
+    def stop_pid(ip: str, port: int, pid: int) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
+        """
+        Stops a PID of a specific server
+
+        :param ip: the ip of the physical node
+        :param port: the port of the cluster manager
+        :param pid: the PID to check
+        :return: The operation outcome
+        """
+        # Open a gRPC session
+        with grpc.insecure_channel(f'{ip}:{port}') as channel:
+            stub = csle_cluster.cluster_manager.cluster_manager_pb2_grpc.ClusterManagerStub(channel)
+            operation_outcome_dto = csle_cluster.cluster_manager.query_cluster_manager.stop_pid(stub=stub, pid=pid)
+            return operation_outcome_dto
```

### Comparing `csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_manager.py` & `csle_cluster-0.2.0/src/csle_cluster/cluster_manager/cluster_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,105 +86,105 @@
         Starts Postgresql
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with the status of PostgreSQL
         """
         logging.info(f"Starting postgresql with command: {constants.COMMANDS.POSTGRESQL_START}")
-        operation_status, stdout, stderr = ManagementSystemController.start_postgresql()
+        operation_status, stdout, stderr = ManagementSystemController.start_postgresql(logger=logging.getLogger())
         logging.info(f"Started postgresql, stdout:{stdout}, stderr: {stderr}")
         return csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO(running=True)
 
     def stopPostgreSQL(self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopPostgreSQLMsg,
                        context: grpc.ServicerContext) \
             -> csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO:
         """
         Stops Postgresql
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with the status of PostgreSQL
         """
         logging.info(f"Stopping postgresql with command: {constants.COMMANDS.POSTGRESQL_STOP}")
-        operation_status, stdout, stderr = ManagementSystemController.stop_postgresql()
+        operation_status, stdout, stderr = ManagementSystemController.stop_postgresql(logger=logging.getLogger())
         logging.info(f"Stopped postgresql, stdout:{stdout}, stderr: {stderr}")
         return csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO(running=False)
 
     def startDockerEngine(self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StartDockerEngineMsg,
                           context: grpc.ServicerContext) \
             -> csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO:
         """
         Starts Docker Engine
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with the status of  the Docker egine
         """
         logging.info(f"Starting the docker engine with command: {constants.COMMANDS.DOCKER_ENGINE_START}")
-        operation_status, stdout, stderr = ManagementSystemController.start_docker_engine()
+        operation_status, stdout, stderr = ManagementSystemController.start_docker_engine(logger=logging.getLogger())
         logging.info(f"Started the docker engine, stdout:{stdout}, stderr: {stderr}")
         return csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO(running=True)
 
     def stopDockerEngine(self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopDockerEngineMsg,
                          context: grpc.ServicerContext) \
             -> csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO:
         """
         Stops the Docker Engine
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with the status of the Docker Engine
         """
         logging.info(f"Stopping the Docker engine with command: {constants.COMMANDS.DOCKER_ENGINE_STOP}")
-        operation_status, stdout, stderr = ManagementSystemController.stop_docker_engine()
+        operation_status, stdout, stderr = ManagementSystemController.stop_docker_engine(logger=logging.getLogger())
         logging.info(f"Stopped the Docker engine, stdout:{stdout}, stderr: {stderr}")
         return csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO(running=False)
 
     def startNginx(self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StartNginxMsg,
                    context: grpc.ServicerContext) \
             -> csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO:
         """
         Starts Nginx
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with the status of Nginx
         """
         logging.info(f"Starting nginx with command: {constants.COMMANDS.NGINX_START}")
-        operation_status, stdout, stderr = ManagementSystemController.start_nginx()
+        operation_status, stdout, stderr = ManagementSystemController.start_nginx(logger=logging.getLogger())
         logging.info(f"Started nginx, stdout:{stdout}, stderr: {stderr}")
         return csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO(running=True)
 
     def stopNginx(self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopNginxMsg,
                   context: grpc.ServicerContext) \
             -> csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO:
         """
         Stops Nginx
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with the status of Nginx
         """
         logging.info(f"Stopping Nginx with command: {constants.COMMANDS.NGINX_STOP}")
-        operation_status, stdout, stderr = ManagementSystemController.stop_nginx()
+        operation_status, stdout, stderr = ManagementSystemController.stop_nginx(logger=logging.getLogger())
         logging.info(f"Stopped Nginx, stdout:{stdout}, stderr: {stderr}")
         return csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO(running=False)
 
     def startCAdvisor(self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StartCAdvisorMsg,
                       context: grpc.ServicerContext) \
             -> csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO:
         """
         Starts cAdvisor
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with the status of cAdvisor
         """
         logging.info("Starting cAdvisor")
-        ManagementSystemController.start_cadvisor()
+        ManagementSystemController.start_cadvisor(logger=logging.getLogger())
         logging.info("Started cAdvisor")
         return csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO(running=True)
 
     def stopCAdvisor(self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopCAdvisorMsg,
                      context: grpc.ServicerContext) \
             -> csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO:
         """
@@ -206,45 +206,45 @@
         Starts node exporter
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with the status of node exporter
         """
         logging.info("Starting node exporter")
-        ManagementSystemController.start_node_exporter()
+        ManagementSystemController.start_node_exporter(logger=logging.getLogger())
         logging.info("Started node exporter")
         return csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO(running=True)
 
     def stopNodeExporter(self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopNodeExporterMsg,
                          context: grpc.ServicerContext) \
             -> csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO:
         """
         Stops node exporter
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with the status of node exporter
         """
         logging.info("Stopping node exporter")
-        ManagementSystemController.stop_node_exporter()
+        ManagementSystemController.stop_node_exporter(logger=logging.getLogger())
         logging.info("Stopped node exporter")
         return csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO(running=False)
 
     def startGrafana(self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StartGrafanaMsg,
                      context: grpc.ServicerContext) \
             -> csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO:
         """
         Starts grafana
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with the status of grafana
         """
         logging.info("Starting grafana")
-        ManagementSystemController.start_grafana()
+        ManagementSystemController.start_grafana(logger=logging.getLogger())
         logging.info("Started grafana")
         return csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO(running=True)
 
     def stopGrafana(self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopGrafanaMsg,
                     context: grpc.ServicerContext) \
             -> csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO:
         """
@@ -266,45 +266,45 @@
         Starts Prometheus
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with the status of Prometheus
         """
         logging.info("Starting Prometheus")
-        ManagementSystemController.start_prometheus()
+        ManagementSystemController.start_prometheus(logger=logging.getLogger())
         logging.info("Started Prometheus")
         return csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO(running=True)
 
     def stopPrometheus(self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopPrometheusMsg,
                        context: grpc.ServicerContext) \
             -> csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO:
         """
         Stops Prometheus
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with the status of Prometheus
         """
         logging.info("Stopping Prometheus")
-        ManagementSystemController.stop_prometheus()
+        ManagementSystemController.stop_prometheus(logger=logging.getLogger())
         logging.info("Stopped Prometheus")
         return csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO(running=False)
 
     def startPgAdmin(self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StartPgAdminMsg,
                      context: grpc.ServicerContext) \
             -> csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO:
         """
         Starts pgAdmin
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with the status of pgAdmin
         """
         logging.info("Starting pgAdmin")
-        ManagementSystemController.start_pgadmin()
+        ManagementSystemController.start_pgadmin(logger=logging.getLogger())
         logging.info("Started pgAdmin")
         return csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO(running=True)
 
     def stopPgAdmin(self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopPgAdminMsg,
                     context: grpc.ServicerContext) \
             -> csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO:
         """
@@ -326,60 +326,60 @@
         Starts Flask
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with the status of flask
         """
         logging.info("Starting flask")
-        ManagementSystemController.start_flask()
+        ManagementSystemController.start_flask(logger=logging.getLogger())
         logging.info("Started flask")
         return csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO(running=True)
 
     def stopFlask(self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopFlaskMsg,
                   context: grpc.ServicerContext) \
             -> csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO:
         """
         Stops Flask
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with the status of flask
         """
         logging.info("Stopping flask")
-        ManagementSystemController.stop_flask()
+        ManagementSystemController.stop_flask(logger=logging.getLogger())
         logging.info("Stopped flask")
         return csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO(running=False)
 
     def startDockerStatsManager(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StartDockerStatsManagerMsg,
             context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO:
         """
         Starts the docker statsmanager
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with the status of the docker statsmanager
         """
         logging.info("Starting the docker statsmanager")
-        ManagementSystemController.start_docker_stats_manager()
+        ManagementSystemController.start_docker_stats_manager(logger=logging.getLogger())
         logging.info("Started the docker statsmanager")
         return csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO(running=True)
 
     def stopDockerStatsManager(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopDockerStatsManagerMsg,
             context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO:
         """
         Stops the docker statsmanaager
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with the status of the docker statsmanager
         """
         logging.info("Stopping the Docker statsmanager")
-        ManagementSystemController.stop_docker_stats_manager()
+        ManagementSystemController.stop_docker_stats_manager(logger=logging.getLogger())
         logging.info("Stopped the Docker statsmanager")
         return csle_cluster.cluster_manager.cluster_manager_pb2.ServiceStatusDTO(running=False)
 
     def getLogFile(self, request: csle_cluster.cluster_manager.cluster_manager_pb2.GetLogFileMsg,
                    context: grpc.ServicerContext) \
             -> csle_cluster.cluster_manager.cluster_manager_pb2.LogsDTO:
         """
@@ -975,15 +975,15 @@
         """
         Starts the client population of a given execution
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: an OperationOutcomeDTO
         """
-        logging.info(f"Starts the client population in execution with id: {request.ipFirstOctet} "
+        logging.info(f"Starting the client population in execution with id: {request.ipFirstOctet} "
                      f"and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is None:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
         TrafficController.start_client_population(emulation_env_config=execution.emulation_env_config,
                                                   physical_server_ip=GeneralUtil.get_host_ip(),
@@ -1164,15 +1164,15 @@
         """
         Applies the filebeat configurations to a given execution
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: an OperationOutcomeDTO
         """
-        logging.info(f"Applies filebeat confgiurations to containers in execution with id: {request.ipFirstOctet} "
+        logging.info(f"Applies filebeat configurations to containers in execution with id: {request.ipFirstOctet} "
                      f"and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is None:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
         HostController.config_filebeats(emulation_env_config=execution.emulation_env_config,
                                         physical_server_ip=GeneralUtil.get_host_ip(),
@@ -1976,15 +1976,15 @@
         """
         logging.info(f"Creating networks for emulation: {request.emulation} and execution id:{request.ipFirstOctet}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         config = MetastoreFacade.get_config(id=1)
         leader = ClusterUtil.am_i_leader(ip=GeneralUtil.get_host_ip(), config=config)
         if execution is None or not leader:
-            logging.info(f"Not leader, skipping creating networks")
+            logging.info("Not leader, skipping creating networks")
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
         ContainerController.create_networks(containers_config=execution.emulation_env_config.containers_config,
                                             logger=logging.getLogger())
         return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
 
     def stopDockerStatsManagerThread(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopDockerStatsManagerThreadMsg,
@@ -1999,15 +1999,16 @@
         logging.info(f"Stopping the docker stats manager thread for execution with id: {request.ipFirstOctet} "
                      f"and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is None:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
         ContainerController.stop_docker_stats_thread(execution=execution,
-                                                     physical_server_ip=GeneralUtil.get_host_ip())
+                                                     physical_server_ip=GeneralUtil.get_host_ip(),
+                                                     logger=logging.getLogger())
         return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
 
     def getDockerStatsManagerStatus(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.GetDockerStatsManagerStatusMsg,
             context: grpc.ServicerContext) \
             -> csle_cluster.cluster_manager.cluster_manager_pb2.DockerStatsMonitorStatusDTO:
         """
@@ -3414,15 +3415,16 @@
         logging.info(f"Stopping the Ryu manager "
                      f"in execution with id: {request.ipFirstOctet} and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is None:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
         if execution.emulation_env_config.sdn_controller_config.container.physical_host_ip == GeneralUtil.get_host_ip():
-            SDNControllerManager.stop_ryu_manager(emulation_env_config=execution.emulation_env_config)
+            SDNControllerManager.stop_ryu_manager(emulation_env_config=execution.emulation_env_config,
+                                                  logger=logging.getLogger())
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
         else:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
 
     def getRyuStatus(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.GetRyuServiceStatusMsg,
             context: grpc.ServicerContext) \
@@ -3530,15 +3532,16 @@
         logging.info(f"Stopping the Snort IDSes "
                      f"in execution with id: {request.ipFirstOctet} and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is None:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
         SnortIDSController.stop_snort_idses(
-            emulation_env_config=execution.emulation_env_config, physical_server_ip=GeneralUtil.get_host_ip())
+            emulation_env_config=execution.emulation_env_config, physical_server_ip=GeneralUtil.get_host_ip(),
+            logger=logging.getLogger())
         return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
 
     def getSnortIdsMonitorThreadStatuses(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.GetSnortIdsMonitorThreadStatusesMsg,
             context: grpc.ServicerContext) \
             -> csle_cluster.cluster_manager.cluster_manager_pb2.SnortIdsMonitorThreadStatusesDTO:
         """
@@ -3550,25 +3553,24 @@
         """
         logging.info(f"Getting the Snort IDS monitor thread statuses "
                      f"in execution with id: {request.ipFirstOctet} and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is not None:
             status_dtos = SnortIDSController.get_snort_idses_monitor_threads_statuses(
-                emulation_env_config=execution.emulation_env_config, physical_server_ip=GeneralUtil.get_host_ip())
+                emulation_env_config=execution.emulation_env_config, physical_server_ip=GeneralUtil.get_host_ip(),
+                logger=logging.getLogger())
             status_dtos = list(
                 map(lambda x: ClusterManagerUtil.convert_snort_ids_monitor_dto_to_snort_ids_status_dto(x),
                     status_dtos))
             return csle_cluster.cluster_manager.cluster_manager_pb2.SnortIdsMonitorThreadStatusesDTO(
-                snortIDSStatuses=status_dtos
-            )
+                snortIDSStatuses=status_dtos)
         else:
             return csle_cluster.cluster_manager.cluster_manager_pb2.SnortIdsMonitorThreadStatusesDTO(
-                snortIDSStatuses=[]
-            )
+                snortIDSStatuses=[])
 
     def stopSnortIdsesMonitorThreads(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopSnortIdsesMonitorThreadsMsg,
             context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
         """
         Stops the Snort IDSes monitor threads for a specific execution
 
@@ -3579,15 +3581,16 @@
         logging.info(f"Stopping the Snort IDSes monitor threads  "
                      f"in execution with id: {request.ipFirstOctet} and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is None:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
         SnortIDSController.stop_snort_idses_monitor_threads(
-            emulation_env_config=execution.emulation_env_config, physical_server_ip=GeneralUtil.get_host_ip())
+            emulation_env_config=execution.emulation_env_config, physical_server_ip=GeneralUtil.get_host_ip(),
+            logger=logging.getLogger())
         return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
 
     def stopSnortIds(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopSnortMsg,
             context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
         """
         Stops the Snort IDS on a specific container
@@ -3601,15 +3604,16 @@
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is None:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
         container_config = ClusterManagerUtil.get_container_config(execution=execution, ip=request.containerIp)
         if container_config is not None:
             SnortIDSController.stop_snort_ids(emulation_env_config=execution.emulation_env_config,
-                                              ip=container_config.docker_gw_bridge_ip)
+                                              ip=container_config.docker_gw_bridge_ip,
+                                              logger=logging.getLogger())
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
         else:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
 
     def stopSnortIdsMonitorThread(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopSnortIdsMonitorThreadMsg,
             context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
@@ -3625,15 +3629,16 @@
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is None:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
         container_config = ClusterManagerUtil.get_container_config(execution=execution, ip=request.containerIp)
         if container_config is not None:
             SnortIDSController.stop_snort_idses_monitor_thread(emulation_env_config=execution.emulation_env_config,
-                                                               ip=container_config.docker_gw_bridge_ip)
+                                                               ip=container_config.docker_gw_bridge_ip,
+                                                               logger=logging.getLogger())
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
         else:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
 
     def startSnortIds(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StartSnortMsg,
             context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
@@ -3649,15 +3654,16 @@
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is None:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
         container_config = ClusterManagerUtil.get_container_config(execution=execution, ip=request.containerIp)
         if container_config is not None:
             SnortIDSController.start_snort_ids(emulation_env_config=execution.emulation_env_config,
-                                               ip=container_config.docker_gw_bridge_ip)
+                                               ip=container_config.docker_gw_bridge_ip,
+                                               logger=logging.getLogger())
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
         else:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
 
     def startSnortIdsMonitorThread(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StartSnortIdsMonitorThreadMsg,
             context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
@@ -3673,15 +3679,16 @@
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is None:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
         container_config = ClusterManagerUtil.get_container_config(execution=execution, ip=request.containerIp)
         if container_config is not None:
             SnortIDSController.start_snort_idses_monitor_thread(emulation_env_config=execution.emulation_env_config,
-                                                                ip=container_config.docker_gw_bridge_ip)
+                                                                ip=container_config.docker_gw_bridge_ip,
+                                                                logger=logging.getLogger())
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
         else:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
 
     def startSnortIdsMonitorThreads(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StartSnortIdsMonitorThreadsMsg,
             context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
@@ -3716,15 +3723,16 @@
         logging.info(f"Starting the Snort IDS managers "
                      f"in execution with id: {request.ipFirstOctet} and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is None:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
         SnortIDSController.start_snort_managers(emulation_env_config=execution.emulation_env_config,
-                                                physical_server_ip=GeneralUtil.get_host_ip())
+                                                physical_server_ip=GeneralUtil.get_host_ip(),
+                                                logger=logging.getLogger())
         return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
 
     def stopSnortIdsManagers(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopSnortIdsManagersMsg,
             context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
         """
         Stops the Snort IDS managers of a specific execution
@@ -3736,15 +3744,16 @@
         logging.info(f"Stopping the Snort IDS managers "
                      f"in execution with id: {request.ipFirstOctet} and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is None:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
         SnortIDSController.stop_snort_managers(emulation_env_config=execution.emulation_env_config,
-                                               physical_server_ip=GeneralUtil.get_host_ip())
+                                               physical_server_ip=GeneralUtil.get_host_ip(),
+                                               logger=logging.getLogger())
         return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
 
     def startSnortIdsManager(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StartSnortIdsManagerMsg,
             context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
         """
         Starts the Snort IDS manager at a specific container
@@ -3758,15 +3767,16 @@
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is None:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
         container_config = ClusterManagerUtil.get_container_config(execution=execution, ip=request.containerIp)
         if container_config is not None:
             SnortIDSController.start_snort_manager(emulation_env_config=execution.emulation_env_config,
-                                                   ip=container_config.docker_gw_bridge_ip)
+                                                   ip=container_config.docker_gw_bridge_ip,
+                                                   logger=logging.getLogger())
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
         else:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
 
     def stopSnortIdsManager(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopSnortIdsManagerMsg,
             context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
@@ -3782,15 +3792,16 @@
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is None:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
         container_config = ClusterManagerUtil.get_container_config(execution=execution, ip=request.containerIp)
         if container_config is not None:
             SnortIDSController.stop_snort_manager(emulation_env_config=execution.emulation_env_config,
-                                                  ip=container_config.docker_gw_bridge_ip)
+                                                  ip=container_config.docker_gw_bridge_ip,
+                                                  logger=logging.getLogger())
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
         else:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
 
     def stopSnortIdsMonitorThreads(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopSnortIdsMonitorThreadsMsg,
             context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
@@ -3804,15 +3815,16 @@
         logging.info(f"Stopping the Snort IDS monitor threads "
                      f"in execution with id: {request.ipFirstOctet} and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is None:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
         SnortIDSController.stop_snort_idses_monitor_threads(emulation_env_config=execution.emulation_env_config,
-                                                            physical_server_ip=GeneralUtil.get_host_ip())
+                                                            physical_server_ip=GeneralUtil.get_host_ip(),
+                                                            logger=logging.getLogger())
         return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
 
     def getSnortIdsManagersInfo(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.GetSnortIdsManagersInfoMsg,
             context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.SnortIdsManagersInfoDTO:
         """
         Gets the info of Snort IDS managers
@@ -4450,14 +4462,131 @@
             return ClusterManagerUtil.get_empty_emulation_metrics_time_series_dto()
         else:
             time_series = ReadEmulationStatisticsUtil.read_all(emulation_env_config=execution.emulation_env_config,
                                                                time_window_minutes=request.minutes,
                                                                logger=logging.getLogger())
             return ClusterManagerUtil.convert_emulation_metrics_time_series_dto(time_series_dto=time_series)
 
+    def startSparkServer(
+            self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StartSparkServerMsg,
+            context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
+        """
+        Starts the Spark server on a specific container in a specific execution
+
+        :param request: the gRPC request
+        :param context: the gRPC context
+        :return: an OperationOutcomeDTO
+        """
+        logging.info(f"Starting the Spark server on the container with ip: {request.containerIp}  "
+                     f"in execution with id: {request.ipFirstOctet} and emulation: {request.emulation}")
+        execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
+                                                            emulation_name=request.emulation)
+        if execution is None:
+            return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
+        container_config = ClusterManagerUtil.get_container_config(execution=execution, ip=request.containerIp)
+        if container_config is not None and container_config.physical_host_ip == GeneralUtil.get_host_ip():
+            HostController.start_spark(emulation_env_config=execution.emulation_env_config,
+                                       ips=[container_config.docker_gw_bridge_ip], logger=logging.getLogger())
+            return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
+        else:
+            return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
+
+    def stopSparkServer(
+            self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopSparkServerMsg,
+            context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
+        """
+        Stops the Spark server on a specific container in a specific execution
+
+        :param request: the gRPC request
+        :param context: the gRPC context
+        :return: an OperationOutcomeDTO
+        """
+        logging.info(f"Stopping the Spark server on the container with ip: {request.containerIp}  "
+                     f"in execution with id: {request.ipFirstOctet} and emulation: {request.emulation}")
+        execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
+                                                            emulation_name=request.emulation)
+        if execution is None:
+            return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
+        container_config = ClusterManagerUtil.get_container_config(execution=execution, ip=request.containerIp)
+        if container_config is not None and container_config.physical_host_ip == GeneralUtil.get_host_ip():
+            HostController.stop_spark(emulation_env_config=execution.emulation_env_config,
+                                      ips=[container_config.docker_gw_bridge_ip], logger=logging.getLogger())
+            return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
+        else:
+            return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
+
+    def startSparkServers(
+            self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StartSparkServersMsg,
+            context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
+        """
+        Starts the Spark servers in a specific execution
+
+        :param request: the gRPC request
+        :param context: the gRPC context
+        :return: an OperationOutcomeDTO
+        """
+        logging.info(f"Starting the Spark servers "
+                     f"in execution with id: {request.ipFirstOctet} and emulation: {request.emulation}")
+        execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
+                                                            emulation_name=request.emulation)
+        if execution is None:
+            return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
+        HostController.start_sparks(emulation_env_config=execution.emulation_env_config,
+                                    physical_server_ip=GeneralUtil.get_host_ip(),
+                                    logger=logging.getLogger())
+        return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
+
+    def stopSparkServers(
+            self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopSparkServersMsg,
+            context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
+        """
+        Stops the Spark servers in a specific execution
+
+        :param request: the gRPC request
+        :param context: the gRPC context
+        :return: an OperationOutcomeDTO
+        """
+        logging.info(f"Stopping the Spark servers "
+                     f"in execution with id: {request.ipFirstOctet} and emulation: {request.emulation}")
+        execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
+                                                            emulation_name=request.emulation)
+        if execution is None:
+            return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
+        HostController.stop_sparks(emulation_env_config=execution.emulation_env_config,
+                                   physical_server_ip=GeneralUtil.get_host_ip(), logger=logging.getLogger())
+        return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
+
+    def checkPid(
+            self, request: csle_cluster.cluster_manager.cluster_manager_pb2.CheckPidMsg,
+            context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
+        """
+        Checks the status of a PID
+
+        :param request: the gRPC request
+        :param context: the gRPC context
+        :return: an OperationOutcomeDTO
+        """
+        logging.info(f"Checking the status of PID: {request.pid}")
+        running = ManagementSystemController.is_pid_running(pid=request.pid)
+        return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=running)
+
+    def stopPid(
+            self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopPidMsg,
+            context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
+        """
+        Stops a PID
+
+        :param request: the gRPC request
+        :param context: the gRPC context
+        :return: an OperationOutcomeDTO
+        """
+        logging.info(f"Stopping PID: {request.pid}")
+        ManagementSystemController.stop_pid(pid=request.pid)
+        return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
+
 
 def serve(port: int = 50041, log_dir: str = "/var/log/csle/", max_workers: int = 10,
           log_file_name: str = "cluster_manager.log") -> None:
     """
     Starts the gRPC server for managing the cluster node
 
     :param port: the port that the server will listen to
```

### Comparing `csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_manager_pb2.py` & `csle_cluster-0.2.0/src/csle_cluster/cluster_manager/cluster_manager_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,24 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x63luster_manager.proto\"Y\n\x1dGetExecutionTimeSeriesDataMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x0f\n\x07minutes\x18\x03 \x01(\x05\"\xa3\t\n\x1d\x45mulationMetricsTimeSeriesDTO\x12\x33\n\x0e\x63lient_metrics\x18\x01 \x03(\x0b\x32\x1b.ClientPopulationMetricsDTO\x12\x30\n\x17\x61ggregated_docker_stats\x18\x02 \x03(\x0b\x32\x0f.DockerStatsDTO\x12+\n\x11\x64ocker_host_stats\x18\x03 \x03(\x0b\x32\x10.DockerStatsDict\x12&\n\x0chost_metrics\x18\x04 \x03(\x0b\x32\x10.HostMetricsDict\x12\x34\n\x17\x61ggregated_host_metrics\x18\x05 \x03(\x0b\x32\x13.HostMetricsDataDTO\x12\x35\n\x10\x64\x65\x66\x65nder_actions\x18\x06 \x03(\x0b\x32\x1b.EmulationDefenderActionDTO\x12\x35\n\x10\x61ttacker_actions\x18\x07 \x03(\x0b\x32\x1b.EmulationAttackerActionDTO\x12\x34\n\x11snort_ids_metrics\x18\x08 \x03(\x0b\x32\x19.SnortIdsAlertCountersDTO\x12\x14\n\x0c\x65mulation_id\x18\t \x01(\x05\x12=\n\x19ossec_host_alert_counters\x18\n \x03(\x0b\x32\x1a.OSSECIdsAlertCountersDict\x12G\n$aggregated_ossec_host_alert_counters\x18\x0b \x03(\x0b\x32\x19.OSSECIdsAlertCountersDTO\x12.\n\x13openflow_flow_stats\x18\x0c \x03(\x0b\x32\x11.FlowStatisticDTO\x12.\n\x13openflow_port_stats\x18\r \x03(\x0b\x32\x11.PortStatisticDTO\x12\x35\n\x17\x61vg_openflow_flow_stats\x18\x0e \x03(\x0b\x32\x14.AvgFlowStatisticDTO\x12\x35\n\x17\x61vg_openflow_port_stats\x18\x0f \x03(\x0b\x32\x14.AvgPortStatisticDTO\x12<\n openflow_flow_metrics_per_switch\x18\x10 \x03(\x0b\x32\x12.FlowStatisticDict\x12<\n openflow_port_metrics_per_switch\x18\x11 \x03(\x0b\x32\x12.PortStatisticDict\x12\x43\n$openflow_flow_avg_metrics_per_switch\x18\x12 \x03(\x0b\x32\x15.AvgFlowStatisticDict\x12\x43\n$openflow_port_avg_metrics_per_switch\x18\x13 \x03(\x0b\x32\x15.AvgPortStatisticDict\x12\x43\n$agg_openflow_flow_metrics_per_switch\x18\x14 \x03(\x0b\x32\x15.AggFlowStatisticDict\x12\x35\n\x17\x61gg_openflow_flow_stats\x18\x15 \x03(\x0b\x32\x14.AggFlowStatisticDTO\"G\n\x14\x41vgPortStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x14.AvgPortStatisticDTO\"G\n\x14\x41ggFlowStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x14.AggFlowStatisticDTO\"G\n\x14\x41vgFlowStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x14.AvgFlowStatisticDTO\"A\n\x11PortStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1f\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x11.PortStatisticDTO\"A\n\x11\x46lowStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1f\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x11.FlowStatisticDTO\"Q\n\x19OSSECIdsAlertCountersDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x19.OSSECIdsAlertCountersDTO\"A\n\x0fHostMetricsDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x13.HostMetricsDataDTO\"=\n\x0f\x44ockerStatsDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x0f.DockerStatsDTO\"\xbc\x04\n\x13\x41vgPortStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\x05\x12\"\n\x1atotal_num_received_packets\x18\x03 \x01(\x05\x12 \n\x18total_num_received_bytes\x18\x04 \x01(\x05\x12!\n\x19total_num_received_errors\x18\x05 \x01(\x05\x12%\n\x1dtotal_num_transmitted_packets\x18\x06 \x01(\x05\x12#\n\x1btotal_num_transmitted_bytes\x18\x07 \x01(\x05\x12$\n\x1ctotal_num_transmitted_errors\x18\x08 \x01(\x05\x12\"\n\x1atotal_num_received_dropped\x18\t \x01(\x05\x12%\n\x1dtotal_num_transmitted_dropped\x18\n \x01(\x05\x12\'\n\x1ftotal_num_received_frame_errors\x18\x0b \x01(\x05\x12)\n!total_num_received_overrun_errors\x18\x0c \x01(\x05\x12%\n\x1dtotal_num_received_crc_errors\x18\r \x01(\x05\x12\x1c\n\x14total_num_collisions\x18\x0e \x01(\x05\x12 \n\x18\x61vg_duration_nanoseconds\x18\x0f \x01(\x05\x12\x1c\n\x14\x61vg_duration_seconds\x18\x10 \x01(\x05\"\x8f\x02\n\x13\x41vgFlowStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\x05\x12\x19\n\x11total_num_packets\x18\x03 \x01(\x05\x12\x17\n\x0ftotal_num_bytes\x18\x04 \x01(\x05\x12 \n\x18\x61vg_duration_nanoseconds\x18\x05 \x01(\x05\x12\x1c\n\x14\x61vg_duration_seconds\x18\x06 \x01(\x05\x12\x18\n\x10\x61vg_hard_timeout\x18\x07 \x01(\x05\x12\x18\n\x10\x61vg_idle_timeout\x18\x08 \x01(\x05\x12\x14\n\x0c\x61vg_priority\x18\t \x01(\x05\x12\x12\n\navg_cookie\x18\n \x01(\x05\"\x8a\x01\n\x13\x41ggFlowStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\x05\x12\x19\n\x11total_num_packets\x18\x03 \x01(\x05\x12\x17\n\x0ftotal_num_bytes\x18\x04 \x01(\x05\x12\x17\n\x0ftotal_num_flows\x18\x05 \x01(\x05\"\xf7\x03\n\x10PortStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\x05\x12\x0c\n\x04port\x18\x03 \x01(\x05\x12\x1c\n\x14num_received_packets\x18\x04 \x01(\x05\x12\x1a\n\x12num_received_bytes\x18\x05 \x01(\x05\x12\x1b\n\x13num_received_errors\x18\x06 \x01(\x05\x12\x1f\n\x17num_transmitted_packets\x18\x07 \x01(\x05\x12\x1d\n\x15num_transmitted_bytes\x18\x08 \x01(\x05\x12\x1e\n\x16num_transmitted_errors\x18\t \x01(\x05\x12\x1c\n\x14num_received_dropped\x18\n \x01(\x05\x12\x1f\n\x17num_transmitted_dropped\x18\x0b \x01(\x05\x12!\n\x19num_received_frame_errors\x18\x0c \x01(\x05\x12#\n\x1bnum_received_overrun_errors\x18\r \x01(\x05\x12\x1f\n\x17num_received_crc_errors\x18\x0e \x01(\x05\x12\x16\n\x0enum_collisions\x18\x0f \x01(\x05\x12\x1c\n\x14\x64uration_nanoseconds\x18\x10 \x01(\x05\x12\x18\n\x10\x64uration_seconds\x18\x11 \x01(\x05\"\xa4\x02\n\x10\x46lowStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\x05\x12\x0f\n\x07in_port\x18\x03 \x01(\x05\x12\x10\n\x08out_port\x18\x04 \x01(\x05\x12\x17\n\x0f\x64st_mac_address\x18\x05 \x01(\t\x12\x13\n\x0bnum_packets\x18\x06 \x01(\x05\x12\x11\n\tnum_bytes\x18\x07 \x01(\x05\x12\x1c\n\x14\x64uration_nanoseconds\x18\x08 \x01(\x05\x12\x18\n\x10\x64uration_seconds\x18\t \x01(\x05\x12\x14\n\x0chard_timeout\x18\n \x01(\x05\x12\x14\n\x0cidle_timeout\x18\x0b \x01(\x05\x12\x10\n\x08priority\x18\x0c \x01(\x05\x12\x0e\n\x06\x63ookie\x18\r \x01(\x05\"\xc5\x01\n\x18OSSECIdsAlertCountersDTO\x12\x14\n\x0clevel_alerts\x18\x01 \x03(\x05\x12\x14\n\x0cgroup_alerts\x18\x02 \x03(\x05\x12\x15\n\rsevere_alerts\x18\x03 \x01(\x05\x12\x16\n\x0ewarning_alerts\x18\x04 \x01(\x05\x12\x14\n\x0ctotal_alerts\x18\x05 \x01(\x05\x12 \n\x18\x61lerts_weighted_by_level\x18\x06 \x01(\x02\x12\n\n\x02ip\x18\x07 \x01(\t\x12\n\n\x02ts\x18\x08 \x01(\x02\"\xb5\x01\n\x18SnortIdsAlertCountersDTO\x12\x17\n\x0fpriority_alerts\x18\x01 \x03(\x05\x12\x14\n\x0c\x63lass_alerts\x18\x02 \x03(\x05\x12\x15\n\rsevere_alerts\x18\x03 \x01(\x05\x12\x16\n\x0ewarning_alerts\x18\x04 \x01(\x05\x12#\n\x1b\x61lerts_weighted_by_priority\x18\x05 \x01(\x02\x12\n\n\x02ip\x18\x06 \x01(\t\x12\n\n\x02ts\x18\x07 \x01(\x02\"\xf4\x01\n\x1a\x45mulationAttackerActionDTO\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63mds\x18\x03 \x03(\t\x12\x0c\n\x04type\x18\x04 \x01(\x05\x12\r\n\x05\x64\x65scr\x18\x05 \x01(\t\x12\x0b\n\x03ips\x18\x06 \x03(\t\x12\r\n\x05index\x18\x07 \x01(\x05\x12\x16\n\x0e\x61\x63tion_outcome\x18\x08 \x01(\x05\x12\x10\n\x08\x61lt_cmds\x18\t \x03(\t\x12\x16\n\x0e\x65xecution_time\x18\n \x01(\x02\x12\n\n\x02ts\x18\x0b \x01(\x02\x12\x15\n\rvulnerability\x18\x0c \x01(\t\x12\x10\n\x08\x62\x61\x63kdoor\x18\r \x01(\x08\"\xcb\x01\n\x1a\x45mulationDefenderActionDTO\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63mds\x18\x03 \x03(\t\x12\x0c\n\x04type\x18\x04 \x01(\x05\x12\r\n\x05\x64\x65scr\x18\x05 \x01(\t\x12\x0b\n\x03ips\x18\x06 \x03(\t\x12\r\n\x05index\x18\x07 \x01(\x05\x12\x16\n\x0e\x61\x63tion_outcome\x18\x08 \x01(\x05\x12\x10\n\x08\x61lt_cmds\x18\t \x03(\t\x12\x16\n\x0e\x65xecution_time\x18\n \x01(\x02\x12\n\n\x02ts\x18\x0b \x01(\x02\"\xce\x01\n\x12HostMetricsDataDTO\x12\x1b\n\x13num_logged_in_users\x18\x01 \x01(\x05\x12!\n\x19num_failed_login_attempts\x18\x02 \x01(\x05\x12\x1c\n\x14num_open_connections\x18\x03 \x01(\x05\x12\x18\n\x10num_login_events\x18\x04 \x01(\x05\x12\x15\n\rnum_processes\x18\x05 \x01(\x05\x12\x11\n\tnum_users\x18\x06 \x01(\x05\x12\n\n\x02ip\x18\x07 \x01(\t\x12\n\n\x02ts\x18\x08 \x01(\x02\"\xf8\x01\n\x0e\x44ockerStatsDTO\x12\x0c\n\x04pids\x18\x01 \x01(\x02\x12\x11\n\ttimestamp\x18\x02 \x01(\t\x12\x13\n\x0b\x63pu_percent\x18\x03 \x01(\x02\x12\x13\n\x0bmem_current\x18\x04 \x01(\x02\x12\x11\n\tmem_total\x18\x05 \x01(\x02\x12\x13\n\x0bmem_percent\x18\x06 \x01(\x02\x12\x10\n\x08\x62lk_read\x18\x07 \x01(\x02\x12\x11\n\tblk_write\x18\x08 \x01(\x02\x12\x0e\n\x06net_rx\x18\t \x01(\x02\x12\x0e\n\x06net_tx\x18\n \x01(\x02\x12\x16\n\x0e\x63ontainer_name\x18\x0b \x01(\t\x12\n\n\x02ip\x18\x0c \x01(\t\x12\n\n\x02ts\x18\r \x01(\x02\"W\n\x1a\x43lientPopulationMetricsDTO\x12\n\n\x02ip\x18\x01 \x01(\t\x12\n\n\x02ts\x18\x02 \x01(\x02\x12\x13\n\x0bnum_clients\x18\x03 \x01(\x05\x12\x0c\n\x04rate\x18\x04 \x01(\x02\"\x1a\n\x18GetClusterManagerLogsMsg\"S\n\x13GetContainerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"B\n\x17GetClientManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16GetKafkaManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\":\n\x0fGetKafkaLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"R\n\x12GetSnortIdsLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"Y\n\x19GetSnortIdsManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"Y\n\x19GetOSSECIdsManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"R\n\x12GetOSSECIdsLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"U\n\x15GetHostManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"X\n\x18GetTrafficManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"?\n\x14GetElkManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"8\n\rGetElkLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14GetRyuManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17GetRyuControllerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17StopRyuMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18StartRyuMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19StopHostMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"X\n\x18StopHostMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"@\n\x15RemoveKibanaTunnelMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15\x43reateKibanaTunnelMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\x16\n\x14ListKibanaTunnelsMsg\"5\n\x10KibanaTunnelsDTO\x12!\n\x07tunnels\x18\x01 \x03(\x0b\x32\x10.KibanaTunnelDTO\"T\n\x0fKibanaTunnelDTO\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\n\n\x02ip\x18\x02 \x01(\t\x12\x11\n\temulation\x18\x03 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x04 \x01(\x05\"=\n\x12RemoveRyuTunnelMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12\x43reateRyuTunnelMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\x13\n\x11ListRyuTunnelsMsg\"/\n\rRyuTunnelsDTO\x12\x1e\n\x07tunnels\x18\x01 \x03(\x0b\x32\r.RyuTunnelDTO\"Q\n\x0cRyuTunnelDTO\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\n\n\x02ip\x18\x02 \x01(\t\x12\x11\n\temulation\x18\x03 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x04 \x01(\x05\"P\n SnortIdsMonitorThreadStatusesDTO\x12,\n\x10snortIDSStatuses\x18\x01 \x03(\x0b\x32\x12.SnortIdsStatusDTO\"E\n\x1aGetSnortIdsManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"N\n#GetSnortIdsMonitorThreadStatusesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"H\n\x1dStopSnortIdsMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"V\n\x16StopSnortIdsManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"W\n\x17StartSnortIdsManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"B\n\x17StopSnortIdsManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18StartSnortIdsManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"M\n\rStartSnortMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"]\n\x1dStartSnortIdsMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"I\n\x1eStartSnortIdsMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"L\n\x0cStopSnortMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"\\\n\x1cStopSnortIdsMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"<\n\x11StopSnortIdsesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"J\n\x1fStopSnortIdsesMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15GetRyuManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18StopRyuMonitorServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19StartRyuMonitorServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11StopRyuServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartRyuServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16GetRyuServiceStatusMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11StopRyuManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartRyuManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1aGetOSSECIDSManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"P\n OSSECIdsMonitorThreadStatusesDTO\x12,\n\x10ossecIDSStatuses\x18\x01 \x03(\x0b\x32\x12.OSSECIdsStatusDTO\"N\n#GetOSSECIDSMonitorThreadStatusesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"H\n\x1dStopOSSECIDSMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\\\n\x1cStopOSSECIDSMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"]\n\x1dStartOSSECIDSMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"S\n\x13StopOSSECIDSManager\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"T\n\x14StartOSSECIDSManager\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"?\n\x14StopOSSECIDSManagers\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StartOSSECIDSManagers\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"P\n\x10StartOSSECIDSMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"O\n\x0fStopOSSECIDSMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"=\n\x12StartOSSECIDSesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11StopOSSECIDSesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17GetKafkaManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\">\n\x13StartKafkaServerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StopKafkaServerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18GetKafkaManagerStatusMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14\x43reateKafkaTopicsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\">\n\x13StopKafkaManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14StartKafkaManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16GetHostManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"K\n GetHostMonitorThreadsStatusesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"V\n\x16\x41pplyFileBeatConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"X\n\x18\x41pplyPacketBeatConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"X\n\x18\x41pplyMetricBeatConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"W\n\x17\x41pplyHeartBeatConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"O\n\x0fStopFileBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"Q\n\x11StopPacketBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"Q\n\x11StopMetricBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"P\n\x10StopHeartBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"f\n\x10StartFileBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\x12\x13\n\x0b\x63ontainerIp\x18\x04 \x01(\t\"h\n\x12StartPacketBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\x12\x13\n\x0b\x63ontainerIp\x18\x04 \x01(\t\"h\n\x12StartMetricBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\x12\x13\n\x0b\x63ontainerIp\x18\x04 \x01(\t\"g\n\x11StartHeartBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\x12\x13\n\x0b\x63ontainerIp\x18\x04 \x01(\t\"Y\n\x19StartHostMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"<\n\x11StopHeartbeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StopPacketbeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\";\n\x10StopFilebeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StopMetricbeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1aStartHostMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"R\n\x12StopHostManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"S\n\x13StartHostManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\">\n\x13StopHostManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xad\x05\n\x10\x45xecutionInfoDTO\x12\x15\n\remulationName\x18\x01 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x02 \x01(\x05\x12\x36\n\x14snortIdsManagersInfo\x18\x03 \x01(\x0b\x32\x18.SnortIdsManagersInfoDTO\x12\x36\n\x14ossecIdsManagersInfo\x18\x04 \x01(\x0b\x32\x18.OSSECIdsManagersInfoDTO\x12\x30\n\x11kafkaManagersInfo\x18\x05 \x01(\x0b\x32\x15.KafkaManagersInfoDTO\x12.\n\x10hostManagersInfo\x18\x06 \x01(\x0b\x32\x14.HostManagersInfoDTO\x12\x32\n\x12\x63lientManagersInfo\x18\x07 \x01(\x0b\x32\x16.ClientManagersInfoDTO\x12<\n\x17\x64ockerStatsManagersInfo\x18\x08 \x01(\x0b\x32\x1b.DockerStatsManagersInfoDTO\x12\x30\n\x11runningContainers\x18\t \x01(\x0b\x32\x15.RunningContainersDTO\x12\x30\n\x11stoppedContainers\x18\n \x01(\x0b\x32\x15.StoppedContainersDTO\x12\x37\n\x16trafficManagersInfoDTO\x18\x0b \x01(\x0b\x32\x17.TrafficManagersInfoDTO\x12*\n\x0e\x61\x63tiveNetworks\x18\x0c \x01(\x0b\x32\x12.DockerNetworksDTO\x12/\n\x12\x65lkManagersInfoDTO\x18\r \x01(\x0b\x32\x13.ElkManagersInfoDTO\x12/\n\x12ryuManagersInfoDTO\x18\x0e \x01(\x0b\x32\x13.RyuManagersInfoDTO\"\xe5\x01\n\x12RyuManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1a\n\x12ryuManagersRunning\x18\x05 \x03(\x08\x12\x31\n\x13ryuManagersStatuses\x18\x06 \x03(\x0b\x32\x14.RyuManagerStatusDTO\x12\x1e\n\x16localControllerWebPort\x18\x07 \x01(\x05\x12\x18\n\x10physicalServerIp\x18\x08 \x01(\t\"\xb4\x01\n\x13RyuManagerStatusDTO\x12\x13\n\x0bryu_running\x18\x01 \x01(\x08\x12\x17\n\x0fmonitor_running\x18\x02 \x01(\x08\x12\x0c\n\x04port\x18\x03 \x01(\x05\x12\x10\n\x08web_port\x18\x04 \x01(\x05\x12\x12\n\ncontroller\x18\x05 \x01(\t\x12\x10\n\x08kafka_ip\x18\x06 \x01(\t\x12\x12\n\nkafka_port\x18\x07 \x01(\x05\x12\x15\n\rtime_step_len\x18\x08 \x01(\x05\"\xaf\x01\n\x13HostManagersInfoDTO\x12\x0b\n\x03ips\x18\x15 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1b\n\x13hostManagersRunning\x18\x05 \x03(\x08\x12\x33\n\x14hostManagersStatuses\x18\x06 \x03(\x0b\x32\x15.HostManagerStatusDTO\"L\n\x16HostManagerStatusesDTO\x12\x32\n\x13hostManagerStatuses\x18\x01 \x03(\x0b\x32\x15.HostManagerStatusDTO\"\xa8\x01\n\x14HostManagerStatusDTO\x12\x17\n\x0fmonitor_running\x18\x01 \x01(\x08\x12\x18\n\x10\x66ilebeat_running\x18\x02 \x01(\x08\x12\x1a\n\x12packetbeat_running\x18\x03 \x01(\x08\x12\x1a\n\x12metricbeat_running\x18\x04 \x01(\x08\x12\x19\n\x11heartbeat_running\x18\x05 \x01(\x08\x12\n\n\x02ip\x18\x06 \x01(\t\"\xac\x01\n\x14KafkaManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1c\n\x14kafkaManagersRunning\x18\x05 \x03(\x08\x12.\n\x15kafkaManagersStatuses\x18\x06 \x03(\x0b\x32\x0f.KafkaStatusDTO\"1\n\x0eKafkaStatusDTO\x12\x0f\n\x07running\x18\x01 \x01(\x08\x12\x0e\n\x06topics\x18\x02 \x03(\t\"\xb8\x01\n\x17OSSECIdsManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1f\n\x17ossecIdsManagersRunning\x18\x05 \x03(\x08\x12\x34\n\x18ossecIdsManagersStatuses\x18\x06 \x03(\x0b\x32\x12.OSSECIdsStatusDTO\"G\n\x11OSSECIdsStatusDTO\x12\x17\n\x0fmonitor_running\x18\x01 \x01(\x08\x12\x19\n\x11ossec_ids_running\x18\x02 \x01(\x08\"\xb8\x01\n\x17SnortIdsManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1f\n\x17snortIdsManagersRunning\x18\x05 \x03(\x08\x12\x34\n\x18snortIdsManagersStatuses\x18\x06 \x03(\x0b\x32\x12.SnortIdsStatusDTO\"G\n\x11SnortIdsStatusDTO\x12\x17\n\x0fmonitor_running\x18\x01 \x01(\x08\x12\x19\n\x11snort_ids_running\x18\x02 \x01(\x08\">\n\x13GetExecutionInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"G\n\x1cStopContainersOfExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"y\n\x0fRunContainerMsg\x12\r\n\x05image\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06memory\x18\x03 \x01(\x05\x12\x10\n\x08num_cpus\x18\x04 \x01(\x05\x12\x16\n\x0e\x63reate_network\x18\x05 \x01(\x08\x12\x0f\n\x07version\x18\x06 \x01(\t\"H\n\x1dStartContainersOfExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15GetElkManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xd7\x01\n\x12\x45lkManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1a\n\x12\x65lkManagersRunning\x18\x05 \x03(\x08\x12*\n\x13\x65lkManagersStatuses\x18\x06 \x03(\x0b\x32\r.ElkStatusDTO\x12\x17\n\x0flocalKibanaPort\x18\x07 \x01(\x05\x12\x18\n\x10physicalServerIp\x18\x08 \x01(\t\"A\n\x16StopLogstashServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17StartLogstashServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14StopKibanaServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StartKibanaServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StopElasticServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16StartElasticServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\":\n\x0fStopElkStackMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"V\n\x0c\x45lkStatusDTO\x12\x16\n\x0e\x65lasticRunning\x18\x01 \x01(\x08\x12\x15\n\rkibanaRunning\x18\x02 \x01(\x08\x12\x17\n\x0flogstashRunning\x18\x03 \x01(\x08\"?\n\x14GetElkStackStatusMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11StopElkManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartElkManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"H\n\x1dGetDockerStatsManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xcb\x01\n\x1a\x44ockerStatsManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\"\n\x1a\x64ockerStatsManagersRunning\x18\x05 \x03(\x08\x12\x41\n\x1b\x64ockerStatsManagersStatuses\x18\x06 \x03(\x0b\x32\x1c.DockerStatsMonitorStatusDTO\"\x1c\n\x1aRemoveAllDockerNetworksMsg\"+\n\x17RemoveDockerNetworksMsg\x12\x10\n\x08networks\x18\x01 \x03(\t\"e\n\x1b\x44ockerStatsMonitorStatusDTO\x12\x14\n\x0cnum_monitors\x18\x01 \x01(\x05\x12\x12\n\nemulations\x18\x02 \x03(\t\x12\x1c\n\x14\x65mulation_executions\x18\x03 \x03(\x05\".\n\x1eGetDockerStatsManagerStatusMsg\x12\x0c\n\x04port\x18\x01 \x01(\x05\"J\n\x1fStopDockerStatsManagerThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1a\x43reateEmulationNetworksMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\x1d\n\x1bListAllStoppedContainersMsg\"F\n\x14StoppedContainersDTO\x12.\n\x11stoppedContainers\x18\x01 \x03(\x0b\x32\x13.DockerContainerDTO\"\x1d\n\x1bListAllRunningEmulationsMsg\"1\n\x14RunningEmulationsDTO\x12\x19\n\x11runningEmulations\x18\x01 \x03(\t\"\x1d\n\x1bListAllRunningContainersMsg\"F\n\x14RunningContainersDTO\x12.\n\x11runningContainers\x18\x01 \x03(\x0b\x32\x13.DockerContainerDTO\"=\n\x12\x44ockerContainerDTO\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05image\x18\x02 \x01(\t\x12\n\n\x02ip\x18\x03 \x01(\t\"!\n\x11StartContainerMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1e\n\x1cStartAllStoppedContainersMsg\"\x1a\n\x18ListAllDockerNetworksMsg\":\n\x11\x44ockerNetworksDTO\x12\x10\n\x08networks\x18\x01 \x03(\t\x12\x13\n\x0bnetwork_ids\x18\x02 \x03(\x05\"8\n\x12\x43ontainerImagesDTO\x12\"\n\x06images\x18\x01 \x03(\x0b\x32\x12.ContainerImageDTO\"f\n\x11\x43ontainerImageDTO\x12\x10\n\x08repoTags\x18\x01 \x01(\t\x12\x0f\n\x07\x63reated\x18\x02 \x01(\t\x12\n\n\x02os\x18\x03 \x01(\t\x12\x14\n\x0c\x61rchitecture\x18\x04 \x01(\t\x12\x0c\n\x04size\x18\x05 \x01(\x03\"\x1b\n\x19ListAllContainerImagesMsg\"\'\n\x17RemoveContainerImageMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1d\n\x1bRemoveAllContainerImagesMsg\"\x1f\n\x1dRemoveAllStoppedContainersMsg\"\"\n\x12RemoveContainerMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\" \n\x10StopContainerMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1d\n\x1bStopAllRunningContainersMsg\"D\n\x19GetTrafficManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xb9\x01\n\x16TrafficManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1e\n\x16trafficManagersRunning\x18\x05 \x03(\x08\x12\x37\n\x17trafficManagersStatuses\x18\x06 \x03(\x0b\x32\x16.TrafficManagerInfoDTO\"8\n\x15TrafficManagerInfoDTO\x12\x0f\n\x07running\x18\x01 \x01(\x08\x12\x0e\n\x06script\x18\x02 \x01(\t\"\xb1\x01\n\x15\x43lientManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1d\n\x15\x63lientManagersRunning\x18\x05 \x03(\x08\x12\x31\n\x16\x63lientManagersStatuses\x18\x06 \x03(\x0b\x32\x11.GetNumClientsDTO\"C\n\x18GetClientManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"X\n\x18StartTrafficGeneratorMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"W\n\x17StopTrafficGeneratorMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"C\n\x18StopTrafficGeneratorsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xae\x01\n\x10GetNumClientsDTO\x12\x13\n\x0bnum_clients\x18\x01 \x01(\x05\x12\x1d\n\x15\x63lient_process_active\x18\x02 \x01(\x08\x12\x17\n\x0fproducer_active\x18\x03 \x01(\x08\x12%\n\x1d\x63lients_time_step_len_seconds\x18\x04 \x01(\x05\x12&\n\x1eproducer_time_step_len_seconds\x18\x05 \x01(\x05\"A\n\x16GetNumActiveClientsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17StopClientPopulationMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14StopClientManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StartClientManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16StopTrafficManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"U\n\x15StopTrafficManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"V\n\x16StartTrafficManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"\x17\n\x15\x43leanAllExecutionsMsg\"\x16\n\x14StopAllExecutionsMsg\";\n\x10StopExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11\x43leanExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"4\n\x1fStopAllExecutionsOfEmulationMsg\x12\x11\n\temulation\x18\x01 \x01(\t\"5\n CleanAllExecutionsOfEmulationMsg\x12\x11\n\temulation\x18\x01 \x01(\t\"\x14\n\x12GetCsleLogFilesMsg\"\x1d\n\rGetLogFileMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\"H\n\x1dStartContainersInExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"S\n(AttachContainersToNetworksInExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\">\n\x13InstallLibrariesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\">\n\x13\x41pplyKafkaConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StartSdnControllerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1a\x41pplyResouceConstraintsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14\x43reateOvsSwitchesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\";\n\x10PingExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\":\n\x0f\x43onfigureOvsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"G\n\x1cStartSdnControllerMonitorMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"9\n\x0e\x43reateUsersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"9\n\x0e\x43reateVulnsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"9\n\x0e\x43reateFlagsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11\x43reateTopologyMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17StartTrafficManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19StartTrafficGeneratorsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18StartClientPopulationMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"F\n\x1bStartKafkaClientProducerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1aStopKafkaClientProducerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartSnortIdsesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"K\n StartSnortIdsesMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartOSSECIdsesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"K\n StartOSSECIdsesMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\";\n\x10StartElkStackMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14StartHostManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17\x41pplyFileBeatConfigsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19\x41pplyPacketBeatConfigsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19\x41pplyMetricBeatConfigsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18\x41pplyHeartBeatConfigsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"R\n\x11StartFileBeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\"T\n\x13StartPacketBeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\"T\n\x13StartMetricBeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\"S\n\x12StartHeartBeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\"\x1e\n\x1cGetDockerStatsManagerLogsMsg\"\x16\n\x14GetPrometheusLogsMsg\"\x18\n\x16GetNodeExporterLogsMsg\"\x14\n\x12GetCAdvisorLogsMsg\"\x13\n\x11GetPgAdminLogsMsg\"\x13\n\x11GetGrafanaLogsMsg\"\x11\n\x0fGetNginxLogsMsg\"\x12\n\x10GetDockerLogsMsg\"\x16\n\x14GetPostgreSQLLogsMsg\"\x11\n\x0fGetFlaskLogsMsg\"\x17\n\x07LogsDTO\x12\x0c\n\x04logs\x18\x01 \x03(\t\"&\n\x13OperationOutcomeDTO\x12\x0f\n\x07outcome\x18\x01 \x01(\x08\"\x12\n\x10GetNodeStatusMsg\"\xb3\x02\n\rNodeStatusDTO\x12\n\n\x02ip\x18\x01 \x01(\t\x12\x0e\n\x06leader\x18\x02 \x01(\x08\x12\x17\n\x0f\x63\x41\x64visorRunning\x18\x03 \x01(\x08\x12\x19\n\x11prometheusRunning\x18\x04 \x01(\x08\x12\x16\n\x0egrafanaRunning\x18\x05 \x01(\x08\x12\x16\n\x0epgAdminRunning\x18\x06 \x01(\x08\x12\x14\n\x0cnginxRunning\x18\x07 \x01(\x08\x12\x14\n\x0c\x66laskRunning\x18\x08 \x01(\x08\x12!\n\x19\x64ockerStatsManagerRunning\x18\t \x01(\x08\x12\x1b\n\x13nodeExporterRunning\x18\n \x01(\x08\x12\x19\n\x11postgreSQLRunning\x18\x0b \x01(\x08\x12\x1b\n\x13\x64ockerEngineRunning\x18\x0c \x01(\x08\"#\n\x10ServiceStatusDTO\x12\x0f\n\x07running\x18\x01 \x01(\x08\"\x14\n\x12StartPostgreSQLMsg\"\x12\n\x10StartCAdvisorMsg\"\x16\n\x14StartNodeExporterMsg\"\x11\n\x0fStartGrafanaMsg\"\x14\n\x12StartPrometheusMsg\"\x11\n\x0fStartPgAdminMsg\"\x0f\n\rStartNginxMsg\"\x0f\n\rStartFlaskMsg\"\x1c\n\x1aStartDockerStatsManagerMsg\"K\n StartDockerStatsManagerThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\x16\n\x14StartDockerEngineMsg\"\x13\n\x11StopPostgreSQLMsg\"\x11\n\x0fStopCAdvisorMsg\"\x15\n\x13StopNodeExporterMsg\"\x10\n\x0eStopGrafanaMsg\"\x13\n\x11StopPrometheusMsg\"\x10\n\x0eStopPgAdminMsg\"\x0e\n\x0cStopNginxMsg\"\x0e\n\x0cStopFlaskMsg\"\x1b\n\x19StopDockerStatsManagerMsg\"\x15\n\x13StopDockerEngineMsg2\xd7o\n\x0e\x43lusterManager\x12\x34\n\rgetNodeStatus\x12\x11.GetNodeStatusMsg\x1a\x0e.NodeStatusDTO\"\x00\x12;\n\x0fstartPostgreSQL\x12\x13.StartPostgreSQLMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x37\n\rstartCAdvisor\x12\x11.StartCAdvisorMsg\x1a\x11.ServiceStatusDTO\"\x00\x12?\n\x11startNodeExporter\x12\x15.StartNodeExporterMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x35\n\x0cstartGrafana\x12\x10.StartGrafanaMsg\x1a\x11.ServiceStatusDTO\"\x00\x12;\n\x0fstartPrometheus\x12\x13.StartPrometheusMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x35\n\x0cstartPgAdmin\x12\x10.StartPgAdminMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x31\n\nstartNginx\x12\x0e.StartNginxMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x31\n\nstartFlask\x12\x0e.StartFlaskMsg\x1a\x11.ServiceStatusDTO\"\x00\x12K\n\x17startDockerStatsManager\x12\x1b.StartDockerStatsManagerMsg\x1a\x11.ServiceStatusDTO\"\x00\x12W\n\x1dstartDockerStatsManagerThread\x12!.StartDockerStatsManagerThreadMsg\x1a\x11.ServiceStatusDTO\"\x00\x12?\n\x11startDockerEngine\x12\x15.StartDockerEngineMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x39\n\x0estopPostgreSQL\x12\x12.StopPostgreSQLMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x35\n\x0cstopCAdvisor\x12\x10.StopCAdvisorMsg\x1a\x11.ServiceStatusDTO\"\x00\x12=\n\x10stopNodeExporter\x12\x14.StopNodeExporterMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x33\n\x0bstopGrafana\x12\x0f.StopGrafanaMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x39\n\x0estopPrometheus\x12\x12.StopPrometheusMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x33\n\x0bstopPgAdmin\x12\x0f.StopPgAdminMsg\x1a\x11.ServiceStatusDTO\"\x00\x12/\n\tstopNginx\x12\r.StopNginxMsg\x1a\x11.ServiceStatusDTO\"\x00\x12/\n\tstopFlask\x12\r.StopFlaskMsg\x1a\x11.ServiceStatusDTO\"\x00\x12I\n\x16stopDockerStatsManager\x12\x1a.StopDockerStatsManagerMsg\x1a\x11.ServiceStatusDTO\"\x00\x12=\n\x10stopDockerEngine\x12\x14.StopDockerEngineMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x32\n\x0fgetCsleLogFiles\x12\x13.GetCsleLogFilesMsg\x1a\x08.LogsDTO\"\x00\x12\x46\n\x19getDockerStatsManagerLogs\x12\x1d.GetDockerStatsManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x36\n\x11getPrometheusLogs\x12\x15.GetPrometheusLogsMsg\x1a\x08.LogsDTO\"\x00\x12:\n\x13getNodeExporterLogs\x12\x17.GetNodeExporterLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x32\n\x0fgetCadvisorLogs\x12\x13.GetCAdvisorLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x30\n\x0egetPgAdminLogs\x12\x12.GetPgAdminLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x30\n\x0egetGrafanaLogs\x12\x12.GetGrafanaLogsMsg\x1a\x08.LogsDTO\"\x00\x12,\n\x0cgetNginxLogs\x12\x10.GetNginxLogsMsg\x1a\x08.LogsDTO\"\x00\x12.\n\rgetDockerLogs\x12\x11.GetDockerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x37\n\x12getPostrgreSQLLogs\x12\x15.GetPostgreSQLLogsMsg\x1a\x08.LogsDTO\"\x00\x12,\n\x0cgetFlaskLogs\x12\x10.GetFlaskLogsMsg\x1a\x08.LogsDTO\"\x00\x12(\n\ngetLogFile\x12\x0e.GetLogFileMsg\x1a\x08.LogsDTO\"\x00\x12T\n\x1astartContainersInExecution\x12\x1e.StartContainersInExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12j\n%attachContainersInExecutionToNetworks\x12).AttachContainersToNetworksInExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10installLibraries\x12\x14.InstallLibrariesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10\x61pplyKafkaConfig\x12\x14.ApplyKafkaConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x12startSdnController\x12\x16.StartSdnControllerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12O\n\x18\x61pplyResourceConstraints\x12\x1b.ApplyResouceConstraintsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11\x63reateOvsSwitches\x12\x15.CreateOvsSwitchesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rpingExecution\x12\x11.PingExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x38\n\x0c\x63onfigureOvs\x12\x10.ConfigureOvsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12R\n\x19startSdnControllerMonitor\x12\x1d.StartSdnControllerMonitorMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x36\n\x0b\x63reateUsers\x12\x0f.CreateUsersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x15\x63reateVulnerabilities\x12\x0f.CreateVulnsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x36\n\x0b\x63reateFlags\x12\x0f.CreateFlagsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0e\x63reateTopology\x12\x12.CreateTopologyMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14startTrafficManagers\x12\x18.StartTrafficManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16startTrafficGenerators\x12\x1a.StartTrafficGeneratorsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15startClientPopulation\x12\x19.StartClientPopulationMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12P\n\x18startKafkaClientProducer\x12\x1c.StartKafkaClientProducerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12N\n\x17stopKafkaClientProducer\x12\x1b.StopKafkaClientProducerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstartSnortIdses\x12\x13.StartSnortIdsesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12Z\n\x1dstartSnortIdsesMonitorThreads\x12!.StartSnortIdsesMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstartOssecIdses\x12\x13.StartOSSECIdsesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12Z\n\x1dstartOssecIdsesMonitorThreads\x12!.StartOSSECIdsesMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstartElkStack\x12\x11.StartElkStackMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11startHostManagers\x12\x15.StartHostManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14\x61pplyFileBeatsConfig\x12\x18.ApplyFileBeatConfigsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16\x61pplyPacketBeatsConfig\x12\x1a.ApplyPacketBeatConfigsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16\x61pplyMetricBeatsConfig\x12\x1a.ApplyMetricBeatConfigsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15\x61pplyHeartBeatsConfig\x12\x19.ApplyHeartBeatConfigsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estartFilebeats\x12\x12.StartFileBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10startPacketbeats\x12\x14.StartPacketBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10startMetricbeats\x12\x14.StartMetricBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstartHeartbeats\x12\x13.StartHeartBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12X\n\x1cstopAllExecutionsOfEmulation\x12 .StopAllExecutionsOfEmulationMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstopExecution\x12\x11.StopExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11stopAllExecutions\x12\x15.StopAllExecutionsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x12\x63leanAllExecutions\x12\x16.CleanAllExecutionsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12Z\n\x1d\x63leanAllExecutionsOfEmulation\x12!.CleanAllExecutionsOfEmulationMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0e\x63leanExecution\x12\x12.CleanExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x46\n\x13startTrafficManager\x12\x17.StartTrafficManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x45\n\x12stopTrafficManager\x12\x17.StartTrafficManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12G\n\x13stopTrafficManagers\x12\x18.StartTrafficManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x12startClientManager\x12\x16.StartClientManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14stopClientPopulation\x12\x18.StopClientPopulationMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11stopClientManager\x12\x15.StopClientManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x43\n\x13getNumActiveClients\x12\x17.GetNumActiveClientsMsg\x1a\x11.GetNumClientsDTO\"\x00\x12J\n\x15startTrafficGenerator\x12\x19.StartTrafficGeneratorMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15stopTrafficGenerators\x12\x19.StopTrafficGeneratorsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14stopTrafficGenerator\x12\x18.StopTrafficGeneratorMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x15getClientManagersInfo\x12\x19.GetClientManagersInfoMsg\x1a\x16.ClientManagersInfoDTO\"\x00\x12N\n\x16getTrafficManagersInfo\x12\x1a.GetTrafficManagersInfoMsg\x1a\x16.TrafficManagerInfoDTO\"\x00\x12P\n\x18stopAllRunningContainers\x12\x1c.StopAllRunningContainersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstopContainer\x12\x11.StopContainerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1aremoveAllStoppedContainers\x12\x1e.RemoveAllStoppedContainersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fremoveContainer\x12\x13.RemoveContainerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12P\n\x18removeAllContainerImages\x12\x1c.RemoveAllContainerImagesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14removeContainerImage\x12\x18.RemoveContainerImageMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12K\n\x16listAllContainerImages\x12\x1a.ListAllContainerImagesMsg\x1a\x13.ContainerImagesDTO\"\x00\x12H\n\x15listAllDockerNetworks\x12\x19.ListAllDockerNetworksMsg\x1a\x12.DockerNetworksDTO\"\x00\x12R\n\x19startAllStoppedContainers\x12\x1d.StartAllStoppedContainersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estartContainer\x12\x12.StartContainerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12Q\n\x18listAllRunningContainers\x12\x1c.ListAllRunningContainersMsg\x1a\x15.RunningContainersDTO\"\x00\x12Q\n\x18listAllRunningEmulations\x12\x1c.ListAllRunningEmulationsMsg\x1a\x15.RunningEmulationsDTO\"\x00\x12Q\n\x18listAllStoppedContainers\x12\x1c.ListAllStoppedContainersMsg\x1a\x15.StoppedContainersDTO\"\x00\x12N\n\x17\x63reateEmulationNetworks\x12\x1b.CreateEmulationNetworksMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12X\n\x1cstopDockerStatsManagerThread\x12 .StopDockerStatsManagerThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12^\n\x1bgetDockerStatsManagerStatus\x12\x1f.GetDockerStatsManagerStatusMsg\x1a\x1c.DockerStatsMonitorStatusDTO\"\x00\x12H\n\x14removeDockerNetworks\x12\x18.RemoveDockerNetworksMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12N\n\x17removeAllDockerNetworks\x12\x1b.RemoveAllDockerNetworksMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12[\n\x1agetDockerStatsManagersInfo\x12\x1e.GetDockerStatsManagersInfoMsg\x1a\x1b.DockerStatsManagersInfoDTO\"\x00\x12>\n\x0fstartElkManager\x12\x13.StartElkManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopElkManager\x12\x12.StopElkManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x36\n\x0cgetElkStatus\x12\x15.GetElkStackStatusMsg\x1a\r.ElkStatusDTO\"\x00\x12\x38\n\x0cstopElkStack\x12\x10.StopElkStackMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0cstartElastic\x12\x17.StartElasticServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12=\n\x0bstopElastic\x12\x16.StopElasticServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12=\n\x0bstartKibana\x12\x16.StartKibanaServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12;\n\nstopKibana\x12\x15.StopKibanaServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x41\n\rstartLogstash\x12\x18.StartLogstashServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0cstopLogstash\x12\x17.StopLogstashServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x43\n\x12getElkManagersInfo\x12\x16.GetElkManagersInfoMsg\x1a\x13.ElkManagersInfoDTO\"\x00\x12T\n\x1astartContainersOfExecution\x12\x1e.StartContainersOfExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x38\n\x0crunContainer\x12\x10.RunContainerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12R\n\x19stopContainersOfExecution\x12\x1d.StopContainersOfExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10startHostManager\x12\x14.StartHostManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10stopHostManagers\x12\x14.StopHostManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstopHostManager\x12\x13.StopHostManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstopFilebeats\x12\x11.StopFilebeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstopPacketbeats\x12\x13.StopPacketbeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstopMetricbeats\x12\x13.StopMetricbeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopHeartbeats\x12\x12.StopHeartbeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12N\n\x17startHostMonitorThreads\x12\x1b.StartHostMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16startHostMonitorThread\x12\x1a.StartHostMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12;\n\rstartFilebeat\x12\x12.StartFileBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0fstartPacketbeat\x12\x14.StartPacketBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0fstartMetricbeat\x12\x14.StartMetricBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12=\n\x0estartHeartbeat\x12\x13.StartHeartBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x38\n\x0cstopFilebeat\x12\x10.StopFileBeatMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopPacketbeat\x12\x12.StopPacketBeatMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopMetricbeat\x12\x12.StopMetricBeatMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstopHeartbeat\x12\x11.StopHeartBeatMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x46\n\x13\x61pplyFileBeatConfig\x12\x17.ApplyFileBeatConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15\x61pplyPacketBeatConfig\x12\x19.ApplyPacketBeatConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15\x61pplyMetricBeatConfig\x12\x19.ApplyMetricBeatConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14\x61pplyHeartBeatConfig\x12\x18.ApplyHeartBeatConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12]\n\x1dgetHostMonitorThreadsStatuses\x12!.GetHostMonitorThreadsStatusesMsg\x1a\x17.HostManagerStatusesDTO\"\x00\x12\x46\n\x13getHostManagersInfo\x12\x17.GetHostManagersInfoMsg\x1a\x14.HostManagersInfoDTO\"\x00\x12@\n\x10stopKafkaManager\x12\x14.StopKafkaManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11startKafkaManager\x12\x15.StartKafkaManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11\x63reateKafkaTopics\x12\x15.CreateKafkaTopicsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0egetKafkaStatus\x12\x19.GetKafkaManagerStatusMsg\x1a\x0f.KafkaStatusDTO\"\x00\x12>\n\x0fstopKafkaServer\x12\x13.StopKafkaServerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x10startKafkaServer\x12\x13.StopKafkaServerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12I\n\x14getKafkaManagersInfo\x12\x18.GetKafkaManagersInfoMsg\x1a\x15.KafkaManagersInfoDTO\"\x00\x12<\n\x0estopOSSECIDSes\x12\x12.StopOSSECIDSesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstartOSSECIDSes\x12\x13.StartOSSECIDSesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x38\n\x0cstopOSSECIDS\x12\x10.StopOSSECIDSMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstartOSSECIDS\x12\x11.StartOSSECIDSMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12G\n\x15startOSSECIDSManagers\x12\x16.StartOSSECIDSManagers\x1a\x14.OperationOutcomeDTO\"\x00\x12\x45\n\x14stopOSSECIDSManagers\x12\x15.StopOSSECIDSManagers\x1a\x14.OperationOutcomeDTO\"\x00\x12\x45\n\x14startOSSECIDSManager\x12\x15.StartOSSECIDSManager\x1a\x14.OperationOutcomeDTO\"\x00\x12\x43\n\x13stopOSSECIDSManager\x12\x14.StopOSSECIDSManager\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1astartOSSECIDSMonitorThread\x12\x1e.StartOSSECIDSMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12R\n\x19stopOSSECIDSMonitorThread\x12\x1d.StopOSSECIDSMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1astopOSSECIDSMonitorThreads\x12\x1e.StopOSSECIDSMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12m\n getOSSECIDSMonitorThreadStatuses\x12$.GetOSSECIDSMonitorThreadStatusesMsg\x1a!.OSSECIdsMonitorThreadStatusesDTO\"\x00\x12R\n\x17getOSSECIdsManagersInfo\x12\x1b.GetOSSECIDSManagersInfoMsg\x1a\x18.OSSECIdsManagersInfoDTO\"\x00\x12>\n\x0fstartRyuManager\x12\x13.StartRyuManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopRyuManager\x12\x12.StopRyuManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0cgetRyuStatus\x12\x17.GetRyuServiceStatusMsg\x1a\x14.RyuManagerStatusDTO\"\x00\x12\x37\n\x08startRyu\x12\x13.StartRyuServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x35\n\x07stopRyu\x12\x12.StopRyuServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x43\n\x12getRyuManagersInfo\x12\x16.GetRyuManagersInfoMsg\x1a\x13.RyuManagersInfoDTO\"\x00\x12<\n\x0estopSnortIdses\x12\x12.StopSnortIdsesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12X\n\x1cstopSnortIdsesMonitorThreads\x12 .StopSnortIdsesMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x35\n\x0cstopSnortIds\x12\r.StopSnortMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12R\n\x19stopSnortIdsMonitorThread\x12\x1d.StopSnortIdsMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x37\n\rstartSnortIds\x12\x0e.StartSnortMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12V\n\x1bstartSnortIdsMonitorThreads\x12\x1f.StartSnortIdsMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1astartSnortIdsMonitorThread\x12\x1e.StartSnortIdsMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15startSnortIdsManagers\x12\x19.StartSnortIdsManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14stopSnortIdsManagers\x12\x18.StopSnortIdsManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14startSnortIdsManager\x12\x18.StartSnortIdsManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x46\n\x13stopSnortIdsManager\x12\x17.StopSnortIdsManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1astopSnortIdsMonitorThreads\x12\x1e.StopSnortIdsMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12m\n getSnortIdsMonitorThreadStatuses\x12$.GetSnortIdsMonitorThreadStatusesMsg\x1a!.SnortIdsMonitorThreadStatusesDTO\"\x00\x12R\n\x17getSnortIdsManagersInfo\x12\x1b.GetSnortIdsManagersInfoMsg\x1a\x18.SnortIdsManagersInfoDTO\"\x00\x12=\n\x10getExecutionInfo\x12\x14.GetExecutionInfoMsg\x1a\x11.ExecutionInfoDTO\"\x00\x12?\n\x11listKibanaTunnels\x12\x15.ListKibanaTunnelsMsg\x1a\x11.KibanaTunnelsDTO\"\x00\x12\x44\n\x12\x63reateKibanaTunnel\x12\x16.CreateKibanaTunnelMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x36\n\x0elistRyuTunnels\x12\x12.ListRyuTunnelsMsg\x1a\x0e.RyuTunnelsDTO\"\x00\x12\x41\n\x0f\x63reateRyuTunnel\x12\x16.CreateKibanaTunnelMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x12removeKibanaTunnel\x12\x16.RemoveKibanaTunnelMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fremoveRyuTunnel\x12\x13.RemoveRyuTunnelMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16stopHostMonitorThreads\x12\x1a.StopHostMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15stopHostMonitorThread\x12\x19.StopHostMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x0fstartRyuMonitor\x12\x19.StartRyuMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x0estopRyuMonitor\x12\x18.StopRyuMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x14getRyuControllerLogs\x12\x18.GetRyuControllerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x36\n\x11getRyuManagerLogs\x12\x15.GetRyuManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12(\n\ngetElkLogs\x12\x0e.GetElkLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x36\n\x11getElkManagerLogs\x12\x15.GetElkManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12>\n\x15getTrafficManagerLogs\x12\x19.GetTrafficManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x38\n\x12getHostManagerLogs\x12\x16.GetHostManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x32\n\x0fgetOSSECIdsLogs\x12\x13.GetOSSECIdsLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x43\n\x19getOSSECIdsManagerLogsMsg\x12\x1a.GetOSSECIdsManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x32\n\x0fgetSnortIdsLogs\x12\x13.GetSnortIdsLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x43\n\x19getSnortIdsManagerLogsMsg\x12\x1a.GetSnortIdsManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12,\n\x0cgetKafkaLogs\x12\x10.GetKafkaLogsMsg\x1a\x08.LogsDTO\"\x00\x12:\n\x13getKafkaManagerLogs\x12\x17.GetKafkaManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12?\n\x17getClientManagerLogsMsg\x12\x18.GetClientManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x34\n\x10getContainerLogs\x12\x14.GetContainerLogsMsg\x1a\x08.LogsDTO\"\x00\x12>\n\x15getClusterManagerLogs\x12\x19.GetClusterManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12^\n\x1agetExecutionTimeSeriesData\x12\x1e.GetExecutionTimeSeriesDataMsg\x1a\x1e.EmulationMetricsTimeSeriesDTO\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x63luster_manager.proto\"\x19\n\nStopPidMsg\x12\x0b\n\x03pid\x18\x01 \x01(\x05\"\x1a\n\x0b\x43heckPidMsg\x12\x0b\n\x03pid\x18\x01 \x01(\x05\"S\n\x13StartSparkServerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"R\n\x12StopSparkServerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"?\n\x14StartSparkServersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\">\n\x13StopSparkServersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"Y\n\x1dGetExecutionTimeSeriesDataMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x0f\n\x07minutes\x18\x03 \x01(\x05\"\xa1\x0b\n\x1d\x45mulationMetricsTimeSeriesDTO\x12\x33\n\x0e\x63lient_metrics\x18\x01 \x03(\x0b\x32\x1b.ClientPopulationMetricsDTO\x12\x30\n\x17\x61ggregated_docker_stats\x18\x02 \x03(\x0b\x32\x0f.DockerStatsDTO\x12+\n\x11\x64ocker_host_stats\x18\x03 \x03(\x0b\x32\x10.DockerStatsDict\x12&\n\x0chost_metrics\x18\x04 \x03(\x0b\x32\x10.HostMetricsDict\x12\x34\n\x17\x61ggregated_host_metrics\x18\x05 \x03(\x0b\x32\x13.HostMetricsDataDTO\x12\x35\n\x10\x64\x65\x66\x65nder_actions\x18\x06 \x03(\x0b\x32\x1b.EmulationDefenderActionDTO\x12\x35\n\x10\x61ttacker_actions\x18\x07 \x03(\x0b\x32\x1b.EmulationAttackerActionDTO\x12\x38\n\x15\x61gg_snort_ids_metrics\x18\x08 \x03(\x0b\x32\x19.SnortIdsAlertCountersDTO\x12\x14\n\x0c\x65mulation_id\x18\t \x01(\x05\x12=\n\x19ossec_host_alert_counters\x18\n \x03(\x0b\x32\x1a.OSSECIdsAlertCountersDict\x12G\n$aggregated_ossec_host_alert_counters\x18\x0b \x03(\x0b\x32\x19.OSSECIdsAlertCountersDTO\x12.\n\x13openflow_flow_stats\x18\x0c \x03(\x0b\x32\x11.FlowStatisticDTO\x12.\n\x13openflow_port_stats\x18\r \x03(\x0b\x32\x11.PortStatisticDTO\x12\x35\n\x17\x61vg_openflow_flow_stats\x18\x0e \x03(\x0b\x32\x14.AvgFlowStatisticDTO\x12\x35\n\x17\x61vg_openflow_port_stats\x18\x0f \x03(\x0b\x32\x14.AvgPortStatisticDTO\x12<\n openflow_flow_metrics_per_switch\x18\x10 \x03(\x0b\x32\x12.FlowStatisticDict\x12<\n openflow_port_metrics_per_switch\x18\x11 \x03(\x0b\x32\x12.PortStatisticDict\x12\x43\n$openflow_flow_avg_metrics_per_switch\x18\x12 \x03(\x0b\x32\x15.AvgFlowStatisticDict\x12\x43\n$openflow_port_avg_metrics_per_switch\x18\x13 \x03(\x0b\x32\x15.AvgPortStatisticDict\x12\x43\n$agg_openflow_flow_metrics_per_switch\x18\x14 \x03(\x0b\x32\x15.AggFlowStatisticDict\x12\x35\n\x17\x61gg_openflow_flow_stats\x18\x15 \x03(\x0b\x32\x14.AggFlowStatisticDTO\x12<\n\x1a\x61gg_snort_ids_rule_metrics\x18\x16 \x03(\x0b\x32\x18.SnortIdsRuleCountersDTO\x12:\n\x14snort_ids_ip_metrics\x18\x17 \x03(\x0b\x32\x1c.SnortIdsIpAlertCountersDict\x12=\n\x1asnort_rule_metrics_per_ids\x18\x18 \x03(\x0b\x32\x19.SnortIdsRuleCountersDict\x12?\n\x1bsnort_alert_metrics_per_ids\x18\x19 \x03(\x0b\x32\x1a.SnortIdsAlertCountersDict\"G\n\x14\x41vgPortStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x14.AvgPortStatisticDTO\"G\n\x14\x41ggFlowStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x14.AggFlowStatisticDTO\"G\n\x14\x41vgFlowStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x14.AvgFlowStatisticDTO\"A\n\x11PortStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1f\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x11.PortStatisticDTO\"A\n\x11\x46lowStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1f\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x11.FlowStatisticDTO\"Q\n\x19OSSECIdsAlertCountersDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x19.OSSECIdsAlertCountersDTO\"A\n\x0fHostMetricsDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x13.HostMetricsDataDTO\"=\n\x0f\x44ockerStatsDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x0f.DockerStatsDTO\"\xbc\x04\n\x13\x41vgPortStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\t\x12\"\n\x1atotal_num_received_packets\x18\x03 \x01(\x03\x12 \n\x18total_num_received_bytes\x18\x04 \x01(\x03\x12!\n\x19total_num_received_errors\x18\x05 \x01(\x03\x12%\n\x1dtotal_num_transmitted_packets\x18\x06 \x01(\x03\x12#\n\x1btotal_num_transmitted_bytes\x18\x07 \x01(\x03\x12$\n\x1ctotal_num_transmitted_errors\x18\x08 \x01(\x03\x12\"\n\x1atotal_num_received_dropped\x18\t \x01(\x03\x12%\n\x1dtotal_num_transmitted_dropped\x18\n \x01(\x03\x12\'\n\x1ftotal_num_received_frame_errors\x18\x0b \x01(\x03\x12)\n!total_num_received_overrun_errors\x18\x0c \x01(\x03\x12%\n\x1dtotal_num_received_crc_errors\x18\r \x01(\x03\x12\x1c\n\x14total_num_collisions\x18\x0e \x01(\x03\x12 \n\x18\x61vg_duration_nanoseconds\x18\x0f \x01(\x03\x12\x1c\n\x14\x61vg_duration_seconds\x18\x10 \x01(\x03\"\x8f\x02\n\x13\x41vgFlowStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\t\x12\x19\n\x11total_num_packets\x18\x03 \x01(\x03\x12\x17\n\x0ftotal_num_bytes\x18\x04 \x01(\x03\x12 \n\x18\x61vg_duration_nanoseconds\x18\x05 \x01(\x03\x12\x1c\n\x14\x61vg_duration_seconds\x18\x06 \x01(\x03\x12\x18\n\x10\x61vg_hard_timeout\x18\x07 \x01(\x03\x12\x18\n\x10\x61vg_idle_timeout\x18\x08 \x01(\x03\x12\x14\n\x0c\x61vg_priority\x18\t \x01(\x03\x12\x12\n\navg_cookie\x18\n \x01(\x03\"\x8a\x01\n\x13\x41ggFlowStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\t\x12\x19\n\x11total_num_packets\x18\x03 \x01(\x03\x12\x17\n\x0ftotal_num_bytes\x18\x04 \x01(\x03\x12\x17\n\x0ftotal_num_flows\x18\x05 \x01(\x03\"\xf7\x03\n\x10PortStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\t\x12\x0c\n\x04port\x18\x03 \x01(\x03\x12\x1c\n\x14num_received_packets\x18\x04 \x01(\x03\x12\x1a\n\x12num_received_bytes\x18\x05 \x01(\x03\x12\x1b\n\x13num_received_errors\x18\x06 \x01(\x03\x12\x1f\n\x17num_transmitted_packets\x18\x07 \x01(\x03\x12\x1d\n\x15num_transmitted_bytes\x18\x08 \x01(\x03\x12\x1e\n\x16num_transmitted_errors\x18\t \x01(\x03\x12\x1c\n\x14num_received_dropped\x18\n \x01(\x03\x12\x1f\n\x17num_transmitted_dropped\x18\x0b \x01(\x03\x12!\n\x19num_received_frame_errors\x18\x0c \x01(\x03\x12#\n\x1bnum_received_overrun_errors\x18\r \x01(\x03\x12\x1f\n\x17num_received_crc_errors\x18\x0e \x01(\x03\x12\x16\n\x0enum_collisions\x18\x0f \x01(\x03\x12\x1c\n\x14\x64uration_nanoseconds\x18\x10 \x01(\x03\x12\x18\n\x10\x64uration_seconds\x18\x11 \x01(\x03\"\xa4\x02\n\x10\x46lowStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\t\x12\x0f\n\x07in_port\x18\x03 \x01(\t\x12\x10\n\x08out_port\x18\x04 \x01(\t\x12\x17\n\x0f\x64st_mac_address\x18\x05 \x01(\t\x12\x13\n\x0bnum_packets\x18\x06 \x01(\x03\x12\x11\n\tnum_bytes\x18\x07 \x01(\x03\x12\x1c\n\x14\x64uration_nanoseconds\x18\x08 \x01(\x03\x12\x18\n\x10\x64uration_seconds\x18\t \x01(\x03\x12\x14\n\x0chard_timeout\x18\n \x01(\x03\x12\x14\n\x0cidle_timeout\x18\x0b \x01(\x03\x12\x10\n\x08priority\x18\x0c \x01(\x03\x12\x0e\n\x06\x63ookie\x18\r \x01(\x03\"\xc5\x01\n\x18OSSECIdsAlertCountersDTO\x12\x14\n\x0clevel_alerts\x18\x01 \x03(\x05\x12\x14\n\x0cgroup_alerts\x18\x02 \x03(\x05\x12\x15\n\rsevere_alerts\x18\x03 \x01(\x05\x12\x16\n\x0ewarning_alerts\x18\x04 \x01(\x05\x12\x14\n\x0ctotal_alerts\x18\x05 \x01(\x05\x12 \n\x18\x61lerts_weighted_by_level\x18\x06 \x01(\x02\x12\n\n\x02ip\x18\x07 \x01(\t\x12\n\n\x02ts\x18\x08 \x01(\x02\"\xb5\x01\n\x18SnortIdsAlertCountersDTO\x12\x17\n\x0fpriority_alerts\x18\x01 \x03(\x05\x12\x14\n\x0c\x63lass_alerts\x18\x02 \x03(\x05\x12\x15\n\rsevere_alerts\x18\x03 \x01(\x05\x12\x16\n\x0ewarning_alerts\x18\x04 \x01(\x05\x12#\n\x1b\x61lerts_weighted_by_priority\x18\x05 \x01(\x02\x12\n\n\x02ip\x18\x06 \x01(\t\x12\n\n\x02ts\x18\x07 \x01(\x02\"U\n\x1bSnortIdsIpAlertCountersDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x1b.SnortIdsIpAlertCountersDTO\"Q\n\x19SnortIdsAlertCountersDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x19.SnortIdsAlertCountersDTO\"O\n\x18SnortIdsRuleCountersDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x18.SnortIdsRuleCountersDTO\"\xc9\x01\n\x1aSnortIdsIpAlertCountersDTO\x12\x17\n\x0fpriority_alerts\x18\x01 \x03(\x05\x12\x14\n\x0c\x63lass_alerts\x18\x02 \x03(\x05\x12\x15\n\rsevere_alerts\x18\x03 \x01(\x05\x12\x16\n\x0ewarning_alerts\x18\x04 \x01(\x05\x12#\n\x1b\x61lerts_weighted_by_priority\x18\x05 \x01(\x02\x12\n\n\x02ip\x18\x06 \x01(\t\x12\n\n\x02ts\x18\x07 \x01(\x02\x12\x10\n\x08\x61lert_ip\x18\x08 \x01(\t\"^\n\x17SnortIdsRuleCountersDTO\x12\x10\n\x08rule_ids\x18\x01 \x03(\t\x12\x19\n\x11rule_alert_counts\x18\x02 \x03(\x05\x12\n\n\x02ip\x18\x03 \x01(\t\x12\n\n\x02ts\x18\x04 \x01(\x02\"\xf4\x01\n\x1a\x45mulationAttackerActionDTO\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63mds\x18\x03 \x03(\t\x12\x0c\n\x04type\x18\x04 \x01(\x05\x12\r\n\x05\x64\x65scr\x18\x05 \x01(\t\x12\x0b\n\x03ips\x18\x06 \x03(\t\x12\r\n\x05index\x18\x07 \x01(\x05\x12\x16\n\x0e\x61\x63tion_outcome\x18\x08 \x01(\x05\x12\x10\n\x08\x61lt_cmds\x18\t \x03(\t\x12\x16\n\x0e\x65xecution_time\x18\n \x01(\x02\x12\n\n\x02ts\x18\x0b \x01(\x02\x12\x15\n\rvulnerability\x18\x0c \x01(\t\x12\x10\n\x08\x62\x61\x63kdoor\x18\r \x01(\x08\"\xcb\x01\n\x1a\x45mulationDefenderActionDTO\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63mds\x18\x03 \x03(\t\x12\x0c\n\x04type\x18\x04 \x01(\x05\x12\r\n\x05\x64\x65scr\x18\x05 \x01(\t\x12\x0b\n\x03ips\x18\x06 \x03(\t\x12\r\n\x05index\x18\x07 \x01(\x05\x12\x16\n\x0e\x61\x63tion_outcome\x18\x08 \x01(\x05\x12\x10\n\x08\x61lt_cmds\x18\t \x03(\t\x12\x16\n\x0e\x65xecution_time\x18\n \x01(\x02\x12\n\n\x02ts\x18\x0b \x01(\x02\"\xce\x01\n\x12HostMetricsDataDTO\x12\x1b\n\x13num_logged_in_users\x18\x01 \x01(\x05\x12!\n\x19num_failed_login_attempts\x18\x02 \x01(\x05\x12\x1c\n\x14num_open_connections\x18\x03 \x01(\x05\x12\x18\n\x10num_login_events\x18\x04 \x01(\x05\x12\x15\n\rnum_processes\x18\x05 \x01(\x05\x12\x11\n\tnum_users\x18\x06 \x01(\x05\x12\n\n\x02ip\x18\x07 \x01(\t\x12\n\n\x02ts\x18\x08 \x01(\x02\"\xf8\x01\n\x0e\x44ockerStatsDTO\x12\x0c\n\x04pids\x18\x01 \x01(\x02\x12\x11\n\ttimestamp\x18\x02 \x01(\t\x12\x13\n\x0b\x63pu_percent\x18\x03 \x01(\x02\x12\x13\n\x0bmem_current\x18\x04 \x01(\x02\x12\x11\n\tmem_total\x18\x05 \x01(\x02\x12\x13\n\x0bmem_percent\x18\x06 \x01(\x02\x12\x10\n\x08\x62lk_read\x18\x07 \x01(\x02\x12\x11\n\tblk_write\x18\x08 \x01(\x02\x12\x0e\n\x06net_rx\x18\t \x01(\x02\x12\x0e\n\x06net_tx\x18\n \x01(\x02\x12\x16\n\x0e\x63ontainer_name\x18\x0b \x01(\t\x12\n\n\x02ip\x18\x0c \x01(\t\x12\n\n\x02ts\x18\r \x01(\x02\"m\n\x1a\x43lientPopulationMetricsDTO\x12\n\n\x02ip\x18\x01 \x01(\t\x12\n\n\x02ts\x18\x02 \x01(\x02\x12\x13\n\x0bnum_clients\x18\x03 \x01(\x05\x12\x0c\n\x04rate\x18\x04 \x01(\x02\x12\x14\n\x0cservice_time\x18\x05 \x01(\x02\"\x1a\n\x18GetClusterManagerLogsMsg\"S\n\x13GetContainerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"B\n\x17GetClientManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16GetKafkaManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\":\n\x0fGetKafkaLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"R\n\x12GetSnortIdsLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"Y\n\x19GetSnortIdsManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"Y\n\x19GetOSSECIdsManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"R\n\x12GetOSSECIdsLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"U\n\x15GetHostManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"X\n\x18GetTrafficManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"?\n\x14GetElkManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"8\n\rGetElkLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14GetRyuManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17GetRyuControllerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17StopRyuMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18StartRyuMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19StopHostMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"X\n\x18StopHostMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"@\n\x15RemoveKibanaTunnelMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15\x43reateKibanaTunnelMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\x16\n\x14ListKibanaTunnelsMsg\"5\n\x10KibanaTunnelsDTO\x12!\n\x07tunnels\x18\x01 \x03(\x0b\x32\x10.KibanaTunnelDTO\"T\n\x0fKibanaTunnelDTO\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\n\n\x02ip\x18\x02 \x01(\t\x12\x11\n\temulation\x18\x03 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x04 \x01(\x05\"=\n\x12RemoveRyuTunnelMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12\x43reateRyuTunnelMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\x13\n\x11ListRyuTunnelsMsg\"/\n\rRyuTunnelsDTO\x12\x1e\n\x07tunnels\x18\x01 \x03(\x0b\x32\r.RyuTunnelDTO\"Q\n\x0cRyuTunnelDTO\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\n\n\x02ip\x18\x02 \x01(\t\x12\x11\n\temulation\x18\x03 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x04 \x01(\x05\"P\n SnortIdsMonitorThreadStatusesDTO\x12,\n\x10snortIDSStatuses\x18\x01 \x03(\x0b\x32\x12.SnortIdsStatusDTO\"E\n\x1aGetSnortIdsManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"N\n#GetSnortIdsMonitorThreadStatusesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"H\n\x1dStopSnortIdsMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"V\n\x16StopSnortIdsManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"W\n\x17StartSnortIdsManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"B\n\x17StopSnortIdsManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18StartSnortIdsManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"M\n\rStartSnortMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"]\n\x1dStartSnortIdsMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"I\n\x1eStartSnortIdsMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"L\n\x0cStopSnortMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"\\\n\x1cStopSnortIdsMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"<\n\x11StopSnortIdsesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"J\n\x1fStopSnortIdsesMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15GetRyuManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18StopRyuMonitorServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19StartRyuMonitorServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11StopRyuServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartRyuServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16GetRyuServiceStatusMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11StopRyuManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartRyuManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1aGetOSSECIDSManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"P\n OSSECIdsMonitorThreadStatusesDTO\x12,\n\x10ossecIDSStatuses\x18\x01 \x03(\x0b\x32\x12.OSSECIdsStatusDTO\"N\n#GetOSSECIDSMonitorThreadStatusesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"H\n\x1dStopOSSECIDSMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\\\n\x1cStopOSSECIDSMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"]\n\x1dStartOSSECIDSMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"S\n\x13StopOSSECIDSManager\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"T\n\x14StartOSSECIDSManager\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"?\n\x14StopOSSECIDSManagers\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StartOSSECIDSManagers\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"P\n\x10StartOSSECIDSMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"O\n\x0fStopOSSECIDSMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"=\n\x12StartOSSECIDSesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11StopOSSECIDSesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17GetKafkaManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\">\n\x13StartKafkaServerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StopKafkaServerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18GetKafkaManagerStatusMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14\x43reateKafkaTopicsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\">\n\x13StopKafkaManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14StartKafkaManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16GetHostManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"K\n GetHostMonitorThreadsStatusesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"V\n\x16\x41pplyFileBeatConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"X\n\x18\x41pplyPacketBeatConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"X\n\x18\x41pplyMetricBeatConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"W\n\x17\x41pplyHeartBeatConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"O\n\x0fStopFileBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"Q\n\x11StopPacketBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"Q\n\x11StopMetricBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"P\n\x10StopHeartBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"f\n\x10StartFileBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\x12\x13\n\x0b\x63ontainerIp\x18\x04 \x01(\t\"h\n\x12StartPacketBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\x12\x13\n\x0b\x63ontainerIp\x18\x04 \x01(\t\"h\n\x12StartMetricBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\x12\x13\n\x0b\x63ontainerIp\x18\x04 \x01(\t\"g\n\x11StartHeartBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\x12\x13\n\x0b\x63ontainerIp\x18\x04 \x01(\t\"Y\n\x19StartHostMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"<\n\x11StopHeartbeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StopPacketbeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\";\n\x10StopFilebeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StopMetricbeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1aStartHostMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"R\n\x12StopHostManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"S\n\x13StartHostManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\">\n\x13StopHostManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xad\x05\n\x10\x45xecutionInfoDTO\x12\x15\n\remulationName\x18\x01 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x02 \x01(\x05\x12\x36\n\x14snortIdsManagersInfo\x18\x03 \x01(\x0b\x32\x18.SnortIdsManagersInfoDTO\x12\x36\n\x14ossecIdsManagersInfo\x18\x04 \x01(\x0b\x32\x18.OSSECIdsManagersInfoDTO\x12\x30\n\x11kafkaManagersInfo\x18\x05 \x01(\x0b\x32\x15.KafkaManagersInfoDTO\x12.\n\x10hostManagersInfo\x18\x06 \x01(\x0b\x32\x14.HostManagersInfoDTO\x12\x32\n\x12\x63lientManagersInfo\x18\x07 \x01(\x0b\x32\x16.ClientManagersInfoDTO\x12<\n\x17\x64ockerStatsManagersInfo\x18\x08 \x01(\x0b\x32\x1b.DockerStatsManagersInfoDTO\x12\x30\n\x11runningContainers\x18\t \x01(\x0b\x32\x15.RunningContainersDTO\x12\x30\n\x11stoppedContainers\x18\n \x01(\x0b\x32\x15.StoppedContainersDTO\x12\x37\n\x16trafficManagersInfoDTO\x18\x0b \x01(\x0b\x32\x17.TrafficManagersInfoDTO\x12*\n\x0e\x61\x63tiveNetworks\x18\x0c \x01(\x0b\x32\x12.DockerNetworksDTO\x12/\n\x12\x65lkManagersInfoDTO\x18\r \x01(\x0b\x32\x13.ElkManagersInfoDTO\x12/\n\x12ryuManagersInfoDTO\x18\x0e \x01(\x0b\x32\x13.RyuManagersInfoDTO\"\xe5\x01\n\x12RyuManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1a\n\x12ryuManagersRunning\x18\x05 \x03(\x08\x12\x31\n\x13ryuManagersStatuses\x18\x06 \x03(\x0b\x32\x14.RyuManagerStatusDTO\x12\x1e\n\x16localControllerWebPort\x18\x07 \x01(\x05\x12\x18\n\x10physicalServerIp\x18\x08 \x01(\t\"\xb4\x01\n\x13RyuManagerStatusDTO\x12\x13\n\x0bryu_running\x18\x01 \x01(\x08\x12\x17\n\x0fmonitor_running\x18\x02 \x01(\x08\x12\x0c\n\x04port\x18\x03 \x01(\x05\x12\x10\n\x08web_port\x18\x04 \x01(\x05\x12\x12\n\ncontroller\x18\x05 \x01(\t\x12\x10\n\x08kafka_ip\x18\x06 \x01(\t\x12\x12\n\nkafka_port\x18\x07 \x01(\x05\x12\x15\n\rtime_step_len\x18\x08 \x01(\x05\"\xaf\x01\n\x13HostManagersInfoDTO\x12\x0b\n\x03ips\x18\x15 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1b\n\x13hostManagersRunning\x18\x05 \x03(\x08\x12\x33\n\x14hostManagersStatuses\x18\x06 \x03(\x0b\x32\x15.HostManagerStatusDTO\"L\n\x16HostManagerStatusesDTO\x12\x32\n\x13hostManagerStatuses\x18\x01 \x03(\x0b\x32\x15.HostManagerStatusDTO\"\xa8\x01\n\x14HostManagerStatusDTO\x12\x17\n\x0fmonitor_running\x18\x01 \x01(\x08\x12\x18\n\x10\x66ilebeat_running\x18\x02 \x01(\x08\x12\x1a\n\x12packetbeat_running\x18\x03 \x01(\x08\x12\x1a\n\x12metricbeat_running\x18\x04 \x01(\x08\x12\x19\n\x11heartbeat_running\x18\x05 \x01(\x08\x12\n\n\x02ip\x18\x06 \x01(\t\"\xac\x01\n\x14KafkaManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1c\n\x14kafkaManagersRunning\x18\x05 \x03(\x08\x12.\n\x15kafkaManagersStatuses\x18\x06 \x03(\x0b\x32\x0f.KafkaStatusDTO\"1\n\x0eKafkaStatusDTO\x12\x0f\n\x07running\x18\x01 \x01(\x08\x12\x0e\n\x06topics\x18\x02 \x03(\t\"\xb8\x01\n\x17OSSECIdsManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1f\n\x17ossecIdsManagersRunning\x18\x05 \x03(\x08\x12\x34\n\x18ossecIdsManagersStatuses\x18\x06 \x03(\x0b\x32\x12.OSSECIdsStatusDTO\"G\n\x11OSSECIdsStatusDTO\x12\x17\n\x0fmonitor_running\x18\x01 \x01(\x08\x12\x19\n\x11ossec_ids_running\x18\x02 \x01(\x08\"\xb8\x01\n\x17SnortIdsManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1f\n\x17snortIdsManagersRunning\x18\x05 \x03(\x08\x12\x34\n\x18snortIdsManagersStatuses\x18\x06 \x03(\x0b\x32\x12.SnortIdsStatusDTO\"G\n\x11SnortIdsStatusDTO\x12\x17\n\x0fmonitor_running\x18\x01 \x01(\x08\x12\x19\n\x11snort_ids_running\x18\x02 \x01(\x08\">\n\x13GetExecutionInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"G\n\x1cStopContainersOfExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"y\n\x0fRunContainerMsg\x12\r\n\x05image\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06memory\x18\x03 \x01(\x05\x12\x10\n\x08num_cpus\x18\x04 \x01(\x05\x12\x16\n\x0e\x63reate_network\x18\x05 \x01(\x08\x12\x0f\n\x07version\x18\x06 \x01(\t\"H\n\x1dStartContainersOfExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15GetElkManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xd7\x01\n\x12\x45lkManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1a\n\x12\x65lkManagersRunning\x18\x05 \x03(\x08\x12*\n\x13\x65lkManagersStatuses\x18\x06 \x03(\x0b\x32\r.ElkStatusDTO\x12\x17\n\x0flocalKibanaPort\x18\x07 \x01(\x05\x12\x18\n\x10physicalServerIp\x18\x08 \x01(\t\"A\n\x16StopLogstashServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17StartLogstashServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14StopKibanaServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StartKibanaServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StopElasticServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16StartElasticServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\":\n\x0fStopElkStackMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"V\n\x0c\x45lkStatusDTO\x12\x16\n\x0e\x65lasticRunning\x18\x01 \x01(\x08\x12\x15\n\rkibanaRunning\x18\x02 \x01(\x08\x12\x17\n\x0flogstashRunning\x18\x03 \x01(\x08\"?\n\x14GetElkStackStatusMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11StopElkManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartElkManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"H\n\x1dGetDockerStatsManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xcb\x01\n\x1a\x44ockerStatsManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\"\n\x1a\x64ockerStatsManagersRunning\x18\x05 \x03(\x08\x12\x41\n\x1b\x64ockerStatsManagersStatuses\x18\x06 \x03(\x0b\x32\x1c.DockerStatsMonitorStatusDTO\"\x1c\n\x1aRemoveAllDockerNetworksMsg\"+\n\x17RemoveDockerNetworksMsg\x12\x10\n\x08networks\x18\x01 \x03(\t\"e\n\x1b\x44ockerStatsMonitorStatusDTO\x12\x14\n\x0cnum_monitors\x18\x01 \x01(\x05\x12\x12\n\nemulations\x18\x02 \x03(\t\x12\x1c\n\x14\x65mulation_executions\x18\x03 \x03(\x05\".\n\x1eGetDockerStatsManagerStatusMsg\x12\x0c\n\x04port\x18\x01 \x01(\x05\"J\n\x1fStopDockerStatsManagerThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1a\x43reateEmulationNetworksMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\x1d\n\x1bListAllStoppedContainersMsg\"F\n\x14StoppedContainersDTO\x12.\n\x11stoppedContainers\x18\x01 \x03(\x0b\x32\x13.DockerContainerDTO\"\x1d\n\x1bListAllRunningEmulationsMsg\"1\n\x14RunningEmulationsDTO\x12\x19\n\x11runningEmulations\x18\x01 \x03(\t\"\x1d\n\x1bListAllRunningContainersMsg\"F\n\x14RunningContainersDTO\x12.\n\x11runningContainers\x18\x01 \x03(\x0b\x32\x13.DockerContainerDTO\"=\n\x12\x44ockerContainerDTO\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05image\x18\x02 \x01(\t\x12\n\n\x02ip\x18\x03 \x01(\t\"!\n\x11StartContainerMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1e\n\x1cStartAllStoppedContainersMsg\"\x1a\n\x18ListAllDockerNetworksMsg\":\n\x11\x44ockerNetworksDTO\x12\x10\n\x08networks\x18\x01 \x03(\t\x12\x13\n\x0bnetwork_ids\x18\x02 \x03(\x05\"8\n\x12\x43ontainerImagesDTO\x12\"\n\x06images\x18\x01 \x03(\x0b\x32\x12.ContainerImageDTO\"f\n\x11\x43ontainerImageDTO\x12\x10\n\x08repoTags\x18\x01 \x01(\t\x12\x0f\n\x07\x63reated\x18\x02 \x01(\t\x12\n\n\x02os\x18\x03 \x01(\t\x12\x14\n\x0c\x61rchitecture\x18\x04 \x01(\t\x12\x0c\n\x04size\x18\x05 \x01(\x03\"\x1b\n\x19ListAllContainerImagesMsg\"\'\n\x17RemoveContainerImageMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1d\n\x1bRemoveAllContainerImagesMsg\"\x1f\n\x1dRemoveAllStoppedContainersMsg\"\"\n\x12RemoveContainerMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\" \n\x10StopContainerMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1d\n\x1bStopAllRunningContainersMsg\"D\n\x19GetTrafficManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xb9\x01\n\x16TrafficManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1e\n\x16trafficManagersRunning\x18\x05 \x03(\x08\x12\x37\n\x17trafficManagersStatuses\x18\x06 \x03(\x0b\x32\x16.TrafficManagerInfoDTO\"8\n\x15TrafficManagerInfoDTO\x12\x0f\n\x07running\x18\x01 \x01(\x08\x12\x0e\n\x06script\x18\x02 \x01(\t\"\xb1\x01\n\x15\x43lientManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1d\n\x15\x63lientManagersRunning\x18\x05 \x03(\x08\x12\x31\n\x16\x63lientManagersStatuses\x18\x06 \x03(\x0b\x32\x11.GetNumClientsDTO\"C\n\x18GetClientManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"X\n\x18StartTrafficGeneratorMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"W\n\x17StopTrafficGeneratorMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"C\n\x18StopTrafficGeneratorsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xae\x01\n\x10GetNumClientsDTO\x12\x13\n\x0bnum_clients\x18\x01 \x01(\x05\x12\x1d\n\x15\x63lient_process_active\x18\x02 \x01(\x08\x12\x17\n\x0fproducer_active\x18\x03 \x01(\x08\x12%\n\x1d\x63lients_time_step_len_seconds\x18\x04 \x01(\x05\x12&\n\x1eproducer_time_step_len_seconds\x18\x05 \x01(\x05\"A\n\x16GetNumActiveClientsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17StopClientPopulationMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14StopClientManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StartClientManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16StopTrafficManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"U\n\x15StopTrafficManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"V\n\x16StartTrafficManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"\x17\n\x15\x43leanAllExecutionsMsg\"\x16\n\x14StopAllExecutionsMsg\";\n\x10StopExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11\x43leanExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"4\n\x1fStopAllExecutionsOfEmulationMsg\x12\x11\n\temulation\x18\x01 \x01(\t\"5\n CleanAllExecutionsOfEmulationMsg\x12\x11\n\temulation\x18\x01 \x01(\t\"\x14\n\x12GetCsleLogFilesMsg\"\x1d\n\rGetLogFileMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\"H\n\x1dStartContainersInExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"S\n(AttachContainersToNetworksInExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\">\n\x13InstallLibrariesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\">\n\x13\x41pplyKafkaConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StartSdnControllerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1a\x41pplyResouceConstraintsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14\x43reateOvsSwitchesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\";\n\x10PingExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\":\n\x0f\x43onfigureOvsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"G\n\x1cStartSdnControllerMonitorMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"9\n\x0e\x43reateUsersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"9\n\x0e\x43reateVulnsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"9\n\x0e\x43reateFlagsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11\x43reateTopologyMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17StartTrafficManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19StartTrafficGeneratorsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18StartClientPopulationMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"F\n\x1bStartKafkaClientProducerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1aStopKafkaClientProducerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartSnortIdsesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"K\n StartSnortIdsesMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartOSSECIdsesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"K\n StartOSSECIdsesMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\";\n\x10StartElkStackMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14StartHostManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17\x41pplyFileBeatConfigsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19\x41pplyPacketBeatConfigsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19\x41pplyMetricBeatConfigsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18\x41pplyHeartBeatConfigsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"R\n\x11StartFileBeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\"T\n\x13StartPacketBeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\"T\n\x13StartMetricBeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\"S\n\x12StartHeartBeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\"\x1e\n\x1cGetDockerStatsManagerLogsMsg\"\x16\n\x14GetPrometheusLogsMsg\"\x18\n\x16GetNodeExporterLogsMsg\"\x14\n\x12GetCAdvisorLogsMsg\"\x13\n\x11GetPgAdminLogsMsg\"\x13\n\x11GetGrafanaLogsMsg\"\x11\n\x0fGetNginxLogsMsg\"\x12\n\x10GetDockerLogsMsg\"\x16\n\x14GetPostgreSQLLogsMsg\"\x11\n\x0fGetFlaskLogsMsg\"\x17\n\x07LogsDTO\x12\x0c\n\x04logs\x18\x01 \x03(\t\"&\n\x13OperationOutcomeDTO\x12\x0f\n\x07outcome\x18\x01 \x01(\x08\"\x12\n\x10GetNodeStatusMsg\"\xb3\x02\n\rNodeStatusDTO\x12\n\n\x02ip\x18\x01 \x01(\t\x12\x0e\n\x06leader\x18\x02 \x01(\x08\x12\x17\n\x0f\x63\x41\x64visorRunning\x18\x03 \x01(\x08\x12\x19\n\x11prometheusRunning\x18\x04 \x01(\x08\x12\x16\n\x0egrafanaRunning\x18\x05 \x01(\x08\x12\x16\n\x0epgAdminRunning\x18\x06 \x01(\x08\x12\x14\n\x0cnginxRunning\x18\x07 \x01(\x08\x12\x14\n\x0c\x66laskRunning\x18\x08 \x01(\x08\x12!\n\x19\x64ockerStatsManagerRunning\x18\t \x01(\x08\x12\x1b\n\x13nodeExporterRunning\x18\n \x01(\x08\x12\x19\n\x11postgreSQLRunning\x18\x0b \x01(\x08\x12\x1b\n\x13\x64ockerEngineRunning\x18\x0c \x01(\x08\"#\n\x10ServiceStatusDTO\x12\x0f\n\x07running\x18\x01 \x01(\x08\"\x14\n\x12StartPostgreSQLMsg\"\x12\n\x10StartCAdvisorMsg\"\x16\n\x14StartNodeExporterMsg\"\x11\n\x0fStartGrafanaMsg\"\x14\n\x12StartPrometheusMsg\"\x11\n\x0fStartPgAdminMsg\"\x0f\n\rStartNginxMsg\"\x0f\n\rStartFlaskMsg\"\x1c\n\x1aStartDockerStatsManagerMsg\"K\n StartDockerStatsManagerThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\x16\n\x14StartDockerEngineMsg\"\x13\n\x11StopPostgreSQLMsg\"\x11\n\x0fStopCAdvisorMsg\"\x15\n\x13StopNodeExporterMsg\"\x10\n\x0eStopGrafanaMsg\"\x13\n\x11StopPrometheusMsg\"\x10\n\x0eStopPgAdminMsg\"\x0e\n\x0cStopNginxMsg\"\x0e\n\x0cStopFlaskMsg\"\x1b\n\x19StopDockerStatsManagerMsg\"\x15\n\x13StopDockerEngineMsg2\xc1r\n\x0e\x43lusterManager\x12\x34\n\rgetNodeStatus\x12\x11.GetNodeStatusMsg\x1a\x0e.NodeStatusDTO\"\x00\x12;\n\x0fstartPostgreSQL\x12\x13.StartPostgreSQLMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x37\n\rstartCAdvisor\x12\x11.StartCAdvisorMsg\x1a\x11.ServiceStatusDTO\"\x00\x12?\n\x11startNodeExporter\x12\x15.StartNodeExporterMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x35\n\x0cstartGrafana\x12\x10.StartGrafanaMsg\x1a\x11.ServiceStatusDTO\"\x00\x12;\n\x0fstartPrometheus\x12\x13.StartPrometheusMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x35\n\x0cstartPgAdmin\x12\x10.StartPgAdminMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x31\n\nstartNginx\x12\x0e.StartNginxMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x31\n\nstartFlask\x12\x0e.StartFlaskMsg\x1a\x11.ServiceStatusDTO\"\x00\x12K\n\x17startDockerStatsManager\x12\x1b.StartDockerStatsManagerMsg\x1a\x11.ServiceStatusDTO\"\x00\x12W\n\x1dstartDockerStatsManagerThread\x12!.StartDockerStatsManagerThreadMsg\x1a\x11.ServiceStatusDTO\"\x00\x12?\n\x11startDockerEngine\x12\x15.StartDockerEngineMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x39\n\x0estopPostgreSQL\x12\x12.StopPostgreSQLMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x35\n\x0cstopCAdvisor\x12\x10.StopCAdvisorMsg\x1a\x11.ServiceStatusDTO\"\x00\x12=\n\x10stopNodeExporter\x12\x14.StopNodeExporterMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x33\n\x0bstopGrafana\x12\x0f.StopGrafanaMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x39\n\x0estopPrometheus\x12\x12.StopPrometheusMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x33\n\x0bstopPgAdmin\x12\x0f.StopPgAdminMsg\x1a\x11.ServiceStatusDTO\"\x00\x12/\n\tstopNginx\x12\r.StopNginxMsg\x1a\x11.ServiceStatusDTO\"\x00\x12/\n\tstopFlask\x12\r.StopFlaskMsg\x1a\x11.ServiceStatusDTO\"\x00\x12I\n\x16stopDockerStatsManager\x12\x1a.StopDockerStatsManagerMsg\x1a\x11.ServiceStatusDTO\"\x00\x12=\n\x10stopDockerEngine\x12\x14.StopDockerEngineMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x32\n\x0fgetCsleLogFiles\x12\x13.GetCsleLogFilesMsg\x1a\x08.LogsDTO\"\x00\x12\x46\n\x19getDockerStatsManagerLogs\x12\x1d.GetDockerStatsManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x36\n\x11getPrometheusLogs\x12\x15.GetPrometheusLogsMsg\x1a\x08.LogsDTO\"\x00\x12:\n\x13getNodeExporterLogs\x12\x17.GetNodeExporterLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x32\n\x0fgetCadvisorLogs\x12\x13.GetCAdvisorLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x30\n\x0egetPgAdminLogs\x12\x12.GetPgAdminLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x30\n\x0egetGrafanaLogs\x12\x12.GetGrafanaLogsMsg\x1a\x08.LogsDTO\"\x00\x12,\n\x0cgetNginxLogs\x12\x10.GetNginxLogsMsg\x1a\x08.LogsDTO\"\x00\x12.\n\rgetDockerLogs\x12\x11.GetDockerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x37\n\x12getPostrgreSQLLogs\x12\x15.GetPostgreSQLLogsMsg\x1a\x08.LogsDTO\"\x00\x12,\n\x0cgetFlaskLogs\x12\x10.GetFlaskLogsMsg\x1a\x08.LogsDTO\"\x00\x12(\n\ngetLogFile\x12\x0e.GetLogFileMsg\x1a\x08.LogsDTO\"\x00\x12T\n\x1astartContainersInExecution\x12\x1e.StartContainersInExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12j\n%attachContainersInExecutionToNetworks\x12).AttachContainersToNetworksInExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10installLibraries\x12\x14.InstallLibrariesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10\x61pplyKafkaConfig\x12\x14.ApplyKafkaConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x12startSdnController\x12\x16.StartSdnControllerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12O\n\x18\x61pplyResourceConstraints\x12\x1b.ApplyResouceConstraintsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11\x63reateOvsSwitches\x12\x15.CreateOvsSwitchesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rpingExecution\x12\x11.PingExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x38\n\x0c\x63onfigureOvs\x12\x10.ConfigureOvsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12R\n\x19startSdnControllerMonitor\x12\x1d.StartSdnControllerMonitorMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x36\n\x0b\x63reateUsers\x12\x0f.CreateUsersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x15\x63reateVulnerabilities\x12\x0f.CreateVulnsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x36\n\x0b\x63reateFlags\x12\x0f.CreateFlagsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0e\x63reateTopology\x12\x12.CreateTopologyMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14startTrafficManagers\x12\x18.StartTrafficManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16startTrafficGenerators\x12\x1a.StartTrafficGeneratorsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15startClientPopulation\x12\x19.StartClientPopulationMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12P\n\x18startKafkaClientProducer\x12\x1c.StartKafkaClientProducerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12N\n\x17stopKafkaClientProducer\x12\x1b.StopKafkaClientProducerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstartSnortIdses\x12\x13.StartSnortIdsesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12Z\n\x1dstartSnortIdsesMonitorThreads\x12!.StartSnortIdsesMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstartOssecIdses\x12\x13.StartOSSECIdsesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12Z\n\x1dstartOssecIdsesMonitorThreads\x12!.StartOSSECIdsesMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstartElkStack\x12\x11.StartElkStackMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11startHostManagers\x12\x15.StartHostManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14\x61pplyFileBeatsConfig\x12\x18.ApplyFileBeatConfigsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16\x61pplyPacketBeatsConfig\x12\x1a.ApplyPacketBeatConfigsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16\x61pplyMetricBeatsConfig\x12\x1a.ApplyMetricBeatConfigsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15\x61pplyHeartBeatsConfig\x12\x19.ApplyHeartBeatConfigsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estartFilebeats\x12\x12.StartFileBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10startPacketbeats\x12\x14.StartPacketBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10startMetricbeats\x12\x14.StartMetricBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstartHeartbeats\x12\x13.StartHeartBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12X\n\x1cstopAllExecutionsOfEmulation\x12 .StopAllExecutionsOfEmulationMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstopExecution\x12\x11.StopExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11stopAllExecutions\x12\x15.StopAllExecutionsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x12\x63leanAllExecutions\x12\x16.CleanAllExecutionsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12Z\n\x1d\x63leanAllExecutionsOfEmulation\x12!.CleanAllExecutionsOfEmulationMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0e\x63leanExecution\x12\x12.CleanExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x46\n\x13startTrafficManager\x12\x17.StartTrafficManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x45\n\x12stopTrafficManager\x12\x17.StartTrafficManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12G\n\x13stopTrafficManagers\x12\x18.StartTrafficManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x12startClientManager\x12\x16.StartClientManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14stopClientPopulation\x12\x18.StopClientPopulationMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11stopClientManager\x12\x15.StopClientManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x43\n\x13getNumActiveClients\x12\x17.GetNumActiveClientsMsg\x1a\x11.GetNumClientsDTO\"\x00\x12J\n\x15startTrafficGenerator\x12\x19.StartTrafficGeneratorMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15stopTrafficGenerators\x12\x19.StopTrafficGeneratorsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14stopTrafficGenerator\x12\x18.StopTrafficGeneratorMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x15getClientManagersInfo\x12\x19.GetClientManagersInfoMsg\x1a\x16.ClientManagersInfoDTO\"\x00\x12N\n\x16getTrafficManagersInfo\x12\x1a.GetTrafficManagersInfoMsg\x1a\x16.TrafficManagerInfoDTO\"\x00\x12P\n\x18stopAllRunningContainers\x12\x1c.StopAllRunningContainersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstopContainer\x12\x11.StopContainerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1aremoveAllStoppedContainers\x12\x1e.RemoveAllStoppedContainersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fremoveContainer\x12\x13.RemoveContainerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12P\n\x18removeAllContainerImages\x12\x1c.RemoveAllContainerImagesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14removeContainerImage\x12\x18.RemoveContainerImageMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12K\n\x16listAllContainerImages\x12\x1a.ListAllContainerImagesMsg\x1a\x13.ContainerImagesDTO\"\x00\x12H\n\x15listAllDockerNetworks\x12\x19.ListAllDockerNetworksMsg\x1a\x12.DockerNetworksDTO\"\x00\x12R\n\x19startAllStoppedContainers\x12\x1d.StartAllStoppedContainersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estartContainer\x12\x12.StartContainerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12Q\n\x18listAllRunningContainers\x12\x1c.ListAllRunningContainersMsg\x1a\x15.RunningContainersDTO\"\x00\x12Q\n\x18listAllRunningEmulations\x12\x1c.ListAllRunningEmulationsMsg\x1a\x15.RunningEmulationsDTO\"\x00\x12Q\n\x18listAllStoppedContainers\x12\x1c.ListAllStoppedContainersMsg\x1a\x15.StoppedContainersDTO\"\x00\x12N\n\x17\x63reateEmulationNetworks\x12\x1b.CreateEmulationNetworksMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12X\n\x1cstopDockerStatsManagerThread\x12 .StopDockerStatsManagerThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12^\n\x1bgetDockerStatsManagerStatus\x12\x1f.GetDockerStatsManagerStatusMsg\x1a\x1c.DockerStatsMonitorStatusDTO\"\x00\x12H\n\x14removeDockerNetworks\x12\x18.RemoveDockerNetworksMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12N\n\x17removeAllDockerNetworks\x12\x1b.RemoveAllDockerNetworksMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12[\n\x1agetDockerStatsManagersInfo\x12\x1e.GetDockerStatsManagersInfoMsg\x1a\x1b.DockerStatsManagersInfoDTO\"\x00\x12>\n\x0fstartElkManager\x12\x13.StartElkManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopElkManager\x12\x12.StopElkManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x36\n\x0cgetElkStatus\x12\x15.GetElkStackStatusMsg\x1a\r.ElkStatusDTO\"\x00\x12\x38\n\x0cstopElkStack\x12\x10.StopElkStackMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0cstartElastic\x12\x17.StartElasticServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12=\n\x0bstopElastic\x12\x16.StopElasticServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12=\n\x0bstartKibana\x12\x16.StartKibanaServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12;\n\nstopKibana\x12\x15.StopKibanaServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x41\n\rstartLogstash\x12\x18.StartLogstashServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0cstopLogstash\x12\x17.StopLogstashServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x43\n\x12getElkManagersInfo\x12\x16.GetElkManagersInfoMsg\x1a\x13.ElkManagersInfoDTO\"\x00\x12T\n\x1astartContainersOfExecution\x12\x1e.StartContainersOfExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x38\n\x0crunContainer\x12\x10.RunContainerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12R\n\x19stopContainersOfExecution\x12\x1d.StopContainersOfExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10startHostManager\x12\x14.StartHostManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10stopHostManagers\x12\x14.StopHostManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstopHostManager\x12\x13.StopHostManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstopFilebeats\x12\x11.StopFilebeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstopPacketbeats\x12\x13.StopPacketbeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstopMetricbeats\x12\x13.StopMetricbeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopHeartbeats\x12\x12.StopHeartbeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12N\n\x17startHostMonitorThreads\x12\x1b.StartHostMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16startHostMonitorThread\x12\x1a.StartHostMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12;\n\rstartFilebeat\x12\x12.StartFileBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0fstartPacketbeat\x12\x14.StartPacketBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0fstartMetricbeat\x12\x14.StartMetricBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12=\n\x0estartHeartbeat\x12\x13.StartHeartBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x38\n\x0cstopFilebeat\x12\x10.StopFileBeatMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopPacketbeat\x12\x12.StopPacketBeatMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopMetricbeat\x12\x12.StopMetricBeatMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstopHeartbeat\x12\x11.StopHeartBeatMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x46\n\x13\x61pplyFileBeatConfig\x12\x17.ApplyFileBeatConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15\x61pplyPacketBeatConfig\x12\x19.ApplyPacketBeatConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15\x61pplyMetricBeatConfig\x12\x19.ApplyMetricBeatConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14\x61pplyHeartBeatConfig\x12\x18.ApplyHeartBeatConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12]\n\x1dgetHostMonitorThreadsStatuses\x12!.GetHostMonitorThreadsStatusesMsg\x1a\x17.HostManagerStatusesDTO\"\x00\x12\x46\n\x13getHostManagersInfo\x12\x17.GetHostManagersInfoMsg\x1a\x14.HostManagersInfoDTO\"\x00\x12@\n\x10stopKafkaManager\x12\x14.StopKafkaManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11startKafkaManager\x12\x15.StartKafkaManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11\x63reateKafkaTopics\x12\x15.CreateKafkaTopicsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0egetKafkaStatus\x12\x19.GetKafkaManagerStatusMsg\x1a\x0f.KafkaStatusDTO\"\x00\x12>\n\x0fstopKafkaServer\x12\x13.StopKafkaServerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x10startKafkaServer\x12\x13.StopKafkaServerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12I\n\x14getKafkaManagersInfo\x12\x18.GetKafkaManagersInfoMsg\x1a\x15.KafkaManagersInfoDTO\"\x00\x12<\n\x0estopOSSECIDSes\x12\x12.StopOSSECIDSesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstartOSSECIDSes\x12\x13.StartOSSECIDSesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x38\n\x0cstopOSSECIDS\x12\x10.StopOSSECIDSMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstartOSSECIDS\x12\x11.StartOSSECIDSMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12G\n\x15startOSSECIDSManagers\x12\x16.StartOSSECIDSManagers\x1a\x14.OperationOutcomeDTO\"\x00\x12\x45\n\x14stopOSSECIDSManagers\x12\x15.StopOSSECIDSManagers\x1a\x14.OperationOutcomeDTO\"\x00\x12\x45\n\x14startOSSECIDSManager\x12\x15.StartOSSECIDSManager\x1a\x14.OperationOutcomeDTO\"\x00\x12\x43\n\x13stopOSSECIDSManager\x12\x14.StopOSSECIDSManager\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1astartOSSECIDSMonitorThread\x12\x1e.StartOSSECIDSMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12R\n\x19stopOSSECIDSMonitorThread\x12\x1d.StopOSSECIDSMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1astopOSSECIDSMonitorThreads\x12\x1e.StopOSSECIDSMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12m\n getOSSECIDSMonitorThreadStatuses\x12$.GetOSSECIDSMonitorThreadStatusesMsg\x1a!.OSSECIdsMonitorThreadStatusesDTO\"\x00\x12R\n\x17getOSSECIdsManagersInfo\x12\x1b.GetOSSECIDSManagersInfoMsg\x1a\x18.OSSECIdsManagersInfoDTO\"\x00\x12>\n\x0fstartRyuManager\x12\x13.StartRyuManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopRyuManager\x12\x12.StopRyuManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0cgetRyuStatus\x12\x17.GetRyuServiceStatusMsg\x1a\x14.RyuManagerStatusDTO\"\x00\x12\x37\n\x08startRyu\x12\x13.StartRyuServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x35\n\x07stopRyu\x12\x12.StopRyuServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x43\n\x12getRyuManagersInfo\x12\x16.GetRyuManagersInfoMsg\x1a\x13.RyuManagersInfoDTO\"\x00\x12<\n\x0estopSnortIdses\x12\x12.StopSnortIdsesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12X\n\x1cstopSnortIdsesMonitorThreads\x12 .StopSnortIdsesMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x35\n\x0cstopSnortIds\x12\r.StopSnortMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12R\n\x19stopSnortIdsMonitorThread\x12\x1d.StopSnortIdsMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x37\n\rstartSnortIds\x12\x0e.StartSnortMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12V\n\x1bstartSnortIdsMonitorThreads\x12\x1f.StartSnortIdsMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1astartSnortIdsMonitorThread\x12\x1e.StartSnortIdsMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15startSnortIdsManagers\x12\x19.StartSnortIdsManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14stopSnortIdsManagers\x12\x18.StopSnortIdsManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14startSnortIdsManager\x12\x18.StartSnortIdsManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x46\n\x13stopSnortIdsManager\x12\x17.StopSnortIdsManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1astopSnortIdsMonitorThreads\x12\x1e.StopSnortIdsMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12m\n getSnortIdsMonitorThreadStatuses\x12$.GetSnortIdsMonitorThreadStatusesMsg\x1a!.SnortIdsMonitorThreadStatusesDTO\"\x00\x12R\n\x17getSnortIdsManagersInfo\x12\x1b.GetSnortIdsManagersInfoMsg\x1a\x18.SnortIdsManagersInfoDTO\"\x00\x12=\n\x10getExecutionInfo\x12\x14.GetExecutionInfoMsg\x1a\x11.ExecutionInfoDTO\"\x00\x12?\n\x11listKibanaTunnels\x12\x15.ListKibanaTunnelsMsg\x1a\x11.KibanaTunnelsDTO\"\x00\x12\x44\n\x12\x63reateKibanaTunnel\x12\x16.CreateKibanaTunnelMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x36\n\x0elistRyuTunnels\x12\x12.ListRyuTunnelsMsg\x1a\x0e.RyuTunnelsDTO\"\x00\x12\x41\n\x0f\x63reateRyuTunnel\x12\x16.CreateKibanaTunnelMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x12removeKibanaTunnel\x12\x16.RemoveKibanaTunnelMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fremoveRyuTunnel\x12\x13.RemoveRyuTunnelMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16stopHostMonitorThreads\x12\x1a.StopHostMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15stopHostMonitorThread\x12\x19.StopHostMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x0fstartRyuMonitor\x12\x19.StartRyuMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x0estopRyuMonitor\x12\x18.StopRyuMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x14getRyuControllerLogs\x12\x18.GetRyuControllerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x36\n\x11getRyuManagerLogs\x12\x15.GetRyuManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12(\n\ngetElkLogs\x12\x0e.GetElkLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x36\n\x11getElkManagerLogs\x12\x15.GetElkManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12>\n\x15getTrafficManagerLogs\x12\x19.GetTrafficManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x38\n\x12getHostManagerLogs\x12\x16.GetHostManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x32\n\x0fgetOSSECIdsLogs\x12\x13.GetOSSECIdsLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x43\n\x19getOSSECIdsManagerLogsMsg\x12\x1a.GetOSSECIdsManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x32\n\x0fgetSnortIdsLogs\x12\x13.GetSnortIdsLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x43\n\x19getSnortIdsManagerLogsMsg\x12\x1a.GetSnortIdsManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12,\n\x0cgetKafkaLogs\x12\x10.GetKafkaLogsMsg\x1a\x08.LogsDTO\"\x00\x12:\n\x13getKafkaManagerLogs\x12\x17.GetKafkaManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12?\n\x17getClientManagerLogsMsg\x12\x18.GetClientManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x34\n\x10getContainerLogs\x12\x14.GetContainerLogsMsg\x1a\x08.LogsDTO\"\x00\x12>\n\x15getClusterManagerLogs\x12\x19.GetClusterManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12^\n\x1agetExecutionTimeSeriesData\x12\x1e.GetExecutionTimeSeriesDataMsg\x1a\x1e.EmulationMetricsTimeSeriesDTO\"\x00\x12\x42\n\x11startSparkServers\x12\x15.StartSparkServersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10stopSparkServers\x12\x14.StopSparkServersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10startSparkServer\x12\x14.StartSparkServerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstopSparkServer\x12\x13.StopSparkServerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x30\n\x08\x63heckPid\x12\x0c.CheckPidMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12.\n\x07stopPid\x12\x0b.StopPidMsg\x1a\x14.OperationOutcomeDTO\"\x00\x62\x06proto3')
 
 
 
+_STOPPIDMSG = DESCRIPTOR.message_types_by_name['StopPidMsg']
+_CHECKPIDMSG = DESCRIPTOR.message_types_by_name['CheckPidMsg']
+_STARTSPARKSERVERMSG = DESCRIPTOR.message_types_by_name['StartSparkServerMsg']
+_STOPSPARKSERVERMSG = DESCRIPTOR.message_types_by_name['StopSparkServerMsg']
+_STARTSPARKSERVERSMSG = DESCRIPTOR.message_types_by_name['StartSparkServersMsg']
+_STOPSPARKSERVERSMSG = DESCRIPTOR.message_types_by_name['StopSparkServersMsg']
 _GETEXECUTIONTIMESERIESDATAMSG = DESCRIPTOR.message_types_by_name['GetExecutionTimeSeriesDataMsg']
 _EMULATIONMETRICSTIMESERIESDTO = DESCRIPTOR.message_types_by_name['EmulationMetricsTimeSeriesDTO']
 _AVGPORTSTATISTICDICT = DESCRIPTOR.message_types_by_name['AvgPortStatisticDict']
 _AGGFLOWSTATISTICDICT = DESCRIPTOR.message_types_by_name['AggFlowStatisticDict']
 _AVGFLOWSTATISTICDICT = DESCRIPTOR.message_types_by_name['AvgFlowStatisticDict']
 _PORTSTATISTICDICT = DESCRIPTOR.message_types_by_name['PortStatisticDict']
 _FLOWSTATISTICDICT = DESCRIPTOR.message_types_by_name['FlowStatisticDict']
@@ -31,14 +37,19 @@
 _AVGPORTSTATISTICDTO = DESCRIPTOR.message_types_by_name['AvgPortStatisticDTO']
 _AVGFLOWSTATISTICDTO = DESCRIPTOR.message_types_by_name['AvgFlowStatisticDTO']
 _AGGFLOWSTATISTICDTO = DESCRIPTOR.message_types_by_name['AggFlowStatisticDTO']
 _PORTSTATISTICDTO = DESCRIPTOR.message_types_by_name['PortStatisticDTO']
 _FLOWSTATISTICDTO = DESCRIPTOR.message_types_by_name['FlowStatisticDTO']
 _OSSECIDSALERTCOUNTERSDTO = DESCRIPTOR.message_types_by_name['OSSECIdsAlertCountersDTO']
 _SNORTIDSALERTCOUNTERSDTO = DESCRIPTOR.message_types_by_name['SnortIdsAlertCountersDTO']
+_SNORTIDSIPALERTCOUNTERSDICT = DESCRIPTOR.message_types_by_name['SnortIdsIpAlertCountersDict']
+_SNORTIDSALERTCOUNTERSDICT = DESCRIPTOR.message_types_by_name['SnortIdsAlertCountersDict']
+_SNORTIDSRULECOUNTERSDICT = DESCRIPTOR.message_types_by_name['SnortIdsRuleCountersDict']
+_SNORTIDSIPALERTCOUNTERSDTO = DESCRIPTOR.message_types_by_name['SnortIdsIpAlertCountersDTO']
+_SNORTIDSRULECOUNTERSDTO = DESCRIPTOR.message_types_by_name['SnortIdsRuleCountersDTO']
 _EMULATIONATTACKERACTIONDTO = DESCRIPTOR.message_types_by_name['EmulationAttackerActionDTO']
 _EMULATIONDEFENDERACTIONDTO = DESCRIPTOR.message_types_by_name['EmulationDefenderActionDTO']
 _HOSTMETRICSDATADTO = DESCRIPTOR.message_types_by_name['HostMetricsDataDTO']
 _DOCKERSTATSDTO = DESCRIPTOR.message_types_by_name['DockerStatsDTO']
 _CLIENTPOPULATIONMETRICSDTO = DESCRIPTOR.message_types_by_name['ClientPopulationMetricsDTO']
 _GETCLUSTERMANAGERLOGSMSG = DESCRIPTOR.message_types_by_name['GetClusterManagerLogsMsg']
 _GETCONTAINERLOGSMSG = DESCRIPTOR.message_types_by_name['GetContainerLogsMsg']
@@ -282,14 +293,56 @@
 _STOPGRAFANAMSG = DESCRIPTOR.message_types_by_name['StopGrafanaMsg']
 _STOPPROMETHEUSMSG = DESCRIPTOR.message_types_by_name['StopPrometheusMsg']
 _STOPPGADMINMSG = DESCRIPTOR.message_types_by_name['StopPgAdminMsg']
 _STOPNGINXMSG = DESCRIPTOR.message_types_by_name['StopNginxMsg']
 _STOPFLASKMSG = DESCRIPTOR.message_types_by_name['StopFlaskMsg']
 _STOPDOCKERSTATSMANAGERMSG = DESCRIPTOR.message_types_by_name['StopDockerStatsManagerMsg']
 _STOPDOCKERENGINEMSG = DESCRIPTOR.message_types_by_name['StopDockerEngineMsg']
+StopPidMsg = _reflection.GeneratedProtocolMessageType('StopPidMsg', (_message.Message,), {
+  'DESCRIPTOR' : _STOPPIDMSG,
+  '__module__' : 'cluster_manager_pb2'
+  # @@protoc_insertion_point(class_scope:StopPidMsg)
+  })
+_sym_db.RegisterMessage(StopPidMsg)
+
+CheckPidMsg = _reflection.GeneratedProtocolMessageType('CheckPidMsg', (_message.Message,), {
+  'DESCRIPTOR' : _CHECKPIDMSG,
+  '__module__' : 'cluster_manager_pb2'
+  # @@protoc_insertion_point(class_scope:CheckPidMsg)
+  })
+_sym_db.RegisterMessage(CheckPidMsg)
+
+StartSparkServerMsg = _reflection.GeneratedProtocolMessageType('StartSparkServerMsg', (_message.Message,), {
+  'DESCRIPTOR' : _STARTSPARKSERVERMSG,
+  '__module__' : 'cluster_manager_pb2'
+  # @@protoc_insertion_point(class_scope:StartSparkServerMsg)
+  })
+_sym_db.RegisterMessage(StartSparkServerMsg)
+
+StopSparkServerMsg = _reflection.GeneratedProtocolMessageType('StopSparkServerMsg', (_message.Message,), {
+  'DESCRIPTOR' : _STOPSPARKSERVERMSG,
+  '__module__' : 'cluster_manager_pb2'
+  # @@protoc_insertion_point(class_scope:StopSparkServerMsg)
+  })
+_sym_db.RegisterMessage(StopSparkServerMsg)
+
+StartSparkServersMsg = _reflection.GeneratedProtocolMessageType('StartSparkServersMsg', (_message.Message,), {
+  'DESCRIPTOR' : _STARTSPARKSERVERSMSG,
+  '__module__' : 'cluster_manager_pb2'
+  # @@protoc_insertion_point(class_scope:StartSparkServersMsg)
+  })
+_sym_db.RegisterMessage(StartSparkServersMsg)
+
+StopSparkServersMsg = _reflection.GeneratedProtocolMessageType('StopSparkServersMsg', (_message.Message,), {
+  'DESCRIPTOR' : _STOPSPARKSERVERSMSG,
+  '__module__' : 'cluster_manager_pb2'
+  # @@protoc_insertion_point(class_scope:StopSparkServersMsg)
+  })
+_sym_db.RegisterMessage(StopSparkServersMsg)
+
 GetExecutionTimeSeriesDataMsg = _reflection.GeneratedProtocolMessageType('GetExecutionTimeSeriesDataMsg', (_message.Message,), {
   'DESCRIPTOR' : _GETEXECUTIONTIMESERIESDATAMSG,
   '__module__' : 'cluster_manager_pb2'
   # @@protoc_insertion_point(class_scope:GetExecutionTimeSeriesDataMsg)
   })
 _sym_db.RegisterMessage(GetExecutionTimeSeriesDataMsg)
 
@@ -401,14 +454,49 @@
 SnortIdsAlertCountersDTO = _reflection.GeneratedProtocolMessageType('SnortIdsAlertCountersDTO', (_message.Message,), {
   'DESCRIPTOR' : _SNORTIDSALERTCOUNTERSDTO,
   '__module__' : 'cluster_manager_pb2'
   # @@protoc_insertion_point(class_scope:SnortIdsAlertCountersDTO)
   })
 _sym_db.RegisterMessage(SnortIdsAlertCountersDTO)
 
+SnortIdsIpAlertCountersDict = _reflection.GeneratedProtocolMessageType('SnortIdsIpAlertCountersDict', (_message.Message,), {
+  'DESCRIPTOR' : _SNORTIDSIPALERTCOUNTERSDICT,
+  '__module__' : 'cluster_manager_pb2'
+  # @@protoc_insertion_point(class_scope:SnortIdsIpAlertCountersDict)
+  })
+_sym_db.RegisterMessage(SnortIdsIpAlertCountersDict)
+
+SnortIdsAlertCountersDict = _reflection.GeneratedProtocolMessageType('SnortIdsAlertCountersDict', (_message.Message,), {
+  'DESCRIPTOR' : _SNORTIDSALERTCOUNTERSDICT,
+  '__module__' : 'cluster_manager_pb2'
+  # @@protoc_insertion_point(class_scope:SnortIdsAlertCountersDict)
+  })
+_sym_db.RegisterMessage(SnortIdsAlertCountersDict)
+
+SnortIdsRuleCountersDict = _reflection.GeneratedProtocolMessageType('SnortIdsRuleCountersDict', (_message.Message,), {
+  'DESCRIPTOR' : _SNORTIDSRULECOUNTERSDICT,
+  '__module__' : 'cluster_manager_pb2'
+  # @@protoc_insertion_point(class_scope:SnortIdsRuleCountersDict)
+  })
+_sym_db.RegisterMessage(SnortIdsRuleCountersDict)
+
+SnortIdsIpAlertCountersDTO = _reflection.GeneratedProtocolMessageType('SnortIdsIpAlertCountersDTO', (_message.Message,), {
+  'DESCRIPTOR' : _SNORTIDSIPALERTCOUNTERSDTO,
+  '__module__' : 'cluster_manager_pb2'
+  # @@protoc_insertion_point(class_scope:SnortIdsIpAlertCountersDTO)
+  })
+_sym_db.RegisterMessage(SnortIdsIpAlertCountersDTO)
+
+SnortIdsRuleCountersDTO = _reflection.GeneratedProtocolMessageType('SnortIdsRuleCountersDTO', (_message.Message,), {
+  'DESCRIPTOR' : _SNORTIDSRULECOUNTERSDTO,
+  '__module__' : 'cluster_manager_pb2'
+  # @@protoc_insertion_point(class_scope:SnortIdsRuleCountersDTO)
+  })
+_sym_db.RegisterMessage(SnortIdsRuleCountersDTO)
+
 EmulationAttackerActionDTO = _reflection.GeneratedProtocolMessageType('EmulationAttackerActionDTO', (_message.Message,), {
   'DESCRIPTOR' : _EMULATIONATTACKERACTIONDTO,
   '__module__' : 'cluster_manager_pb2'
   # @@protoc_insertion_point(class_scope:EmulationAttackerActionDTO)
   })
 _sym_db.RegisterMessage(EmulationAttackerActionDTO)
 
@@ -2162,546 +2250,568 @@
   })
 _sym_db.RegisterMessage(StopDockerEngineMsg)
 
 _CLUSTERMANAGER = DESCRIPTOR.services_by_name['ClusterManager']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _GETEXECUTIONTIMESERIESDATAMSG._serialized_start=25
-  _GETEXECUTIONTIMESERIESDATAMSG._serialized_end=114
-  _EMULATIONMETRICSTIMESERIESDTO._serialized_start=117
-  _EMULATIONMETRICSTIMESERIESDTO._serialized_end=1304
-  _AVGPORTSTATISTICDICT._serialized_start=1306
-  _AVGPORTSTATISTICDICT._serialized_end=1377
-  _AGGFLOWSTATISTICDICT._serialized_start=1379
-  _AGGFLOWSTATISTICDICT._serialized_end=1450
-  _AVGFLOWSTATISTICDICT._serialized_start=1452
-  _AVGFLOWSTATISTICDICT._serialized_end=1523
-  _PORTSTATISTICDICT._serialized_start=1525
-  _PORTSTATISTICDICT._serialized_end=1590
-  _FLOWSTATISTICDICT._serialized_start=1592
-  _FLOWSTATISTICDICT._serialized_end=1657
-  _OSSECIDSALERTCOUNTERSDICT._serialized_start=1659
-  _OSSECIDSALERTCOUNTERSDICT._serialized_end=1740
-  _HOSTMETRICSDICT._serialized_start=1742
-  _HOSTMETRICSDICT._serialized_end=1807
-  _DOCKERSTATSDICT._serialized_start=1809
-  _DOCKERSTATSDICT._serialized_end=1870
-  _AVGPORTSTATISTICDTO._serialized_start=1873
-  _AVGPORTSTATISTICDTO._serialized_end=2445
-  _AVGFLOWSTATISTICDTO._serialized_start=2448
-  _AVGFLOWSTATISTICDTO._serialized_end=2719
-  _AGGFLOWSTATISTICDTO._serialized_start=2722
-  _AGGFLOWSTATISTICDTO._serialized_end=2860
-  _PORTSTATISTICDTO._serialized_start=2863
-  _PORTSTATISTICDTO._serialized_end=3366
-  _FLOWSTATISTICDTO._serialized_start=3369
-  _FLOWSTATISTICDTO._serialized_end=3661
-  _OSSECIDSALERTCOUNTERSDTO._serialized_start=3664
-  _OSSECIDSALERTCOUNTERSDTO._serialized_end=3861
-  _SNORTIDSALERTCOUNTERSDTO._serialized_start=3864
-  _SNORTIDSALERTCOUNTERSDTO._serialized_end=4045
-  _EMULATIONATTACKERACTIONDTO._serialized_start=4048
-  _EMULATIONATTACKERACTIONDTO._serialized_end=4292
-  _EMULATIONDEFENDERACTIONDTO._serialized_start=4295
-  _EMULATIONDEFENDERACTIONDTO._serialized_end=4498
-  _HOSTMETRICSDATADTO._serialized_start=4501
-  _HOSTMETRICSDATADTO._serialized_end=4707
-  _DOCKERSTATSDTO._serialized_start=4710
-  _DOCKERSTATSDTO._serialized_end=4958
-  _CLIENTPOPULATIONMETRICSDTO._serialized_start=4960
-  _CLIENTPOPULATIONMETRICSDTO._serialized_end=5047
-  _GETCLUSTERMANAGERLOGSMSG._serialized_start=5049
-  _GETCLUSTERMANAGERLOGSMSG._serialized_end=5075
-  _GETCONTAINERLOGSMSG._serialized_start=5077
-  _GETCONTAINERLOGSMSG._serialized_end=5160
-  _GETCLIENTMANAGERLOGSMSG._serialized_start=5162
-  _GETCLIENTMANAGERLOGSMSG._serialized_end=5228
-  _GETKAFKAMANAGERLOGSMSG._serialized_start=5230
-  _GETKAFKAMANAGERLOGSMSG._serialized_end=5295
-  _GETKAFKALOGSMSG._serialized_start=5297
-  _GETKAFKALOGSMSG._serialized_end=5355
-  _GETSNORTIDSLOGSMSG._serialized_start=5357
-  _GETSNORTIDSLOGSMSG._serialized_end=5439
-  _GETSNORTIDSMANAGERLOGSMSG._serialized_start=5441
-  _GETSNORTIDSMANAGERLOGSMSG._serialized_end=5530
-  _GETOSSECIDSMANAGERLOGSMSG._serialized_start=5532
-  _GETOSSECIDSMANAGERLOGSMSG._serialized_end=5621
-  _GETOSSECIDSLOGSMSG._serialized_start=5623
-  _GETOSSECIDSLOGSMSG._serialized_end=5705
-  _GETHOSTMANAGERLOGSMSG._serialized_start=5707
-  _GETHOSTMANAGERLOGSMSG._serialized_end=5792
-  _GETTRAFFICMANAGERLOGSMSG._serialized_start=5794
-  _GETTRAFFICMANAGERLOGSMSG._serialized_end=5882
-  _GETELKMANAGERLOGSMSG._serialized_start=5884
-  _GETELKMANAGERLOGSMSG._serialized_end=5947
-  _GETELKLOGSMSG._serialized_start=5949
-  _GETELKLOGSMSG._serialized_end=6005
-  _GETRYUMANAGERLOGSMSG._serialized_start=6007
-  _GETRYUMANAGERLOGSMSG._serialized_end=6070
-  _GETRYUCONTROLLERLOGSMSG._serialized_start=6072
-  _GETRYUCONTROLLERLOGSMSG._serialized_end=6138
-  _STOPRYUMONITORTHREADMSG._serialized_start=6140
-  _STOPRYUMONITORTHREADMSG._serialized_end=6206
-  _STARTRYUMONITORTHREADMSG._serialized_start=6208
-  _STARTRYUMONITORTHREADMSG._serialized_end=6275
-  _STOPHOSTMONITORTHREADSMSG._serialized_start=6277
-  _STOPHOSTMONITORTHREADSMSG._serialized_end=6345
-  _STOPHOSTMONITORTHREADMSG._serialized_start=6347
-  _STOPHOSTMONITORTHREADMSG._serialized_end=6435
-  _REMOVEKIBANATUNNELMSG._serialized_start=6437
-  _REMOVEKIBANATUNNELMSG._serialized_end=6501
-  _CREATEKIBANATUNNELMSG._serialized_start=6503
-  _CREATEKIBANATUNNELMSG._serialized_end=6567
-  _LISTKIBANATUNNELSMSG._serialized_start=6569
-  _LISTKIBANATUNNELSMSG._serialized_end=6591
-  _KIBANATUNNELSDTO._serialized_start=6593
-  _KIBANATUNNELSDTO._serialized_end=6646
-  _KIBANATUNNELDTO._serialized_start=6648
-  _KIBANATUNNELDTO._serialized_end=6732
-  _REMOVERYUTUNNELMSG._serialized_start=6734
-  _REMOVERYUTUNNELMSG._serialized_end=6795
-  _CREATERYUTUNNELMSG._serialized_start=6797
-  _CREATERYUTUNNELMSG._serialized_end=6858
-  _LISTRYUTUNNELSMSG._serialized_start=6860
-  _LISTRYUTUNNELSMSG._serialized_end=6879
-  _RYUTUNNELSDTO._serialized_start=6881
-  _RYUTUNNELSDTO._serialized_end=6928
-  _RYUTUNNELDTO._serialized_start=6930
-  _RYUTUNNELDTO._serialized_end=7011
-  _SNORTIDSMONITORTHREADSTATUSESDTO._serialized_start=7013
-  _SNORTIDSMONITORTHREADSTATUSESDTO._serialized_end=7093
-  _GETSNORTIDSMANAGERSINFOMSG._serialized_start=7095
-  _GETSNORTIDSMANAGERSINFOMSG._serialized_end=7164
-  _GETSNORTIDSMONITORTHREADSTATUSESMSG._serialized_start=7166
-  _GETSNORTIDSMONITORTHREADSTATUSESMSG._serialized_end=7244
-  _STOPSNORTIDSMONITORTHREADSMSG._serialized_start=7246
-  _STOPSNORTIDSMONITORTHREADSMSG._serialized_end=7318
-  _STOPSNORTIDSMANAGERMSG._serialized_start=7320
-  _STOPSNORTIDSMANAGERMSG._serialized_end=7406
-  _STARTSNORTIDSMANAGERMSG._serialized_start=7408
-  _STARTSNORTIDSMANAGERMSG._serialized_end=7495
-  _STOPSNORTIDSMANAGERSMSG._serialized_start=7497
-  _STOPSNORTIDSMANAGERSMSG._serialized_end=7563
-  _STARTSNORTIDSMANAGERSMSG._serialized_start=7565
-  _STARTSNORTIDSMANAGERSMSG._serialized_end=7632
-  _STARTSNORTMSG._serialized_start=7634
-  _STARTSNORTMSG._serialized_end=7711
-  _STARTSNORTIDSMONITORTHREADMSG._serialized_start=7713
-  _STARTSNORTIDSMONITORTHREADMSG._serialized_end=7806
-  _STARTSNORTIDSMONITORTHREADSMSG._serialized_start=7808
-  _STARTSNORTIDSMONITORTHREADSMSG._serialized_end=7881
-  _STOPSNORTMSG._serialized_start=7883
-  _STOPSNORTMSG._serialized_end=7959
-  _STOPSNORTIDSMONITORTHREADMSG._serialized_start=7961
-  _STOPSNORTIDSMONITORTHREADMSG._serialized_end=8053
-  _STOPSNORTIDSESMSG._serialized_start=8055
-  _STOPSNORTIDSESMSG._serialized_end=8115
-  _STOPSNORTIDSESMONITORTHREADSMSG._serialized_start=8117
-  _STOPSNORTIDSESMONITORTHREADSMSG._serialized_end=8191
-  _GETRYUMANAGERSINFOMSG._serialized_start=8193
-  _GETRYUMANAGERSINFOMSG._serialized_end=8257
-  _STOPRYUMONITORSERVICEMSG._serialized_start=8259
-  _STOPRYUMONITORSERVICEMSG._serialized_end=8326
-  _STARTRYUMONITORSERVICEMSG._serialized_start=8328
-  _STARTRYUMONITORSERVICEMSG._serialized_end=8396
-  _STOPRYUSERVICEMSG._serialized_start=8398
-  _STOPRYUSERVICEMSG._serialized_end=8458
-  _STARTRYUSERVICEMSG._serialized_start=8460
-  _STARTRYUSERVICEMSG._serialized_end=8521
-  _GETRYUSERVICESTATUSMSG._serialized_start=8523
-  _GETRYUSERVICESTATUSMSG._serialized_end=8588
-  _STOPRYUMANAGERMSG._serialized_start=8590
-  _STOPRYUMANAGERMSG._serialized_end=8650
-  _STARTRYUMANAGERMSG._serialized_start=8652
-  _STARTRYUMANAGERMSG._serialized_end=8713
-  _GETOSSECIDSMANAGERSINFOMSG._serialized_start=8715
-  _GETOSSECIDSMANAGERSINFOMSG._serialized_end=8784
-  _OSSECIDSMONITORTHREADSTATUSESDTO._serialized_start=8786
-  _OSSECIDSMONITORTHREADSTATUSESDTO._serialized_end=8866
-  _GETOSSECIDSMONITORTHREADSTATUSESMSG._serialized_start=8868
-  _GETOSSECIDSMONITORTHREADSTATUSESMSG._serialized_end=8946
-  _STOPOSSECIDSMONITORTHREADSMSG._serialized_start=8948
-  _STOPOSSECIDSMONITORTHREADSMSG._serialized_end=9020
-  _STOPOSSECIDSMONITORTHREADMSG._serialized_start=9022
-  _STOPOSSECIDSMONITORTHREADMSG._serialized_end=9114
-  _STARTOSSECIDSMONITORTHREADMSG._serialized_start=9116
-  _STARTOSSECIDSMONITORTHREADMSG._serialized_end=9209
-  _STOPOSSECIDSMANAGER._serialized_start=9211
-  _STOPOSSECIDSMANAGER._serialized_end=9294
-  _STARTOSSECIDSMANAGER._serialized_start=9296
-  _STARTOSSECIDSMANAGER._serialized_end=9380
-  _STOPOSSECIDSMANAGERS._serialized_start=9382
-  _STOPOSSECIDSMANAGERS._serialized_end=9445
-  _STARTOSSECIDSMANAGERS._serialized_start=9447
-  _STARTOSSECIDSMANAGERS._serialized_end=9511
-  _STARTOSSECIDSMSG._serialized_start=9513
-  _STARTOSSECIDSMSG._serialized_end=9593
-  _STOPOSSECIDSMSG._serialized_start=9595
-  _STOPOSSECIDSMSG._serialized_end=9674
-  _STARTOSSECIDSESMSG._serialized_start=9676
-  _STARTOSSECIDSESMSG._serialized_end=9737
-  _STOPOSSECIDSESMSG._serialized_start=9739
-  _STOPOSSECIDSESMSG._serialized_end=9799
-  _GETKAFKAMANAGERSINFOMSG._serialized_start=9801
-  _GETKAFKAMANAGERSINFOMSG._serialized_end=9867
-  _STARTKAFKASERVERMSG._serialized_start=9869
-  _STARTKAFKASERVERMSG._serialized_end=9931
-  _STOPKAFKASERVERMSG._serialized_start=9933
-  _STOPKAFKASERVERMSG._serialized_end=9994
-  _GETKAFKAMANAGERSTATUSMSG._serialized_start=9996
-  _GETKAFKAMANAGERSTATUSMSG._serialized_end=10063
-  _CREATEKAFKATOPICSMSG._serialized_start=10065
-  _CREATEKAFKATOPICSMSG._serialized_end=10128
-  _STOPKAFKAMANAGERMSG._serialized_start=10130
-  _STOPKAFKAMANAGERMSG._serialized_end=10192
-  _STARTKAFKAMANAGERMSG._serialized_start=10194
-  _STARTKAFKAMANAGERMSG._serialized_end=10257
-  _GETHOSTMANAGERSINFOMSG._serialized_start=10259
-  _GETHOSTMANAGERSINFOMSG._serialized_end=10324
-  _GETHOSTMONITORTHREADSSTATUSESMSG._serialized_start=10326
-  _GETHOSTMONITORTHREADSSTATUSESMSG._serialized_end=10401
-  _APPLYFILEBEATCONFIGMSG._serialized_start=10403
-  _APPLYFILEBEATCONFIGMSG._serialized_end=10489
-  _APPLYPACKETBEATCONFIGMSG._serialized_start=10491
-  _APPLYPACKETBEATCONFIGMSG._serialized_end=10579
-  _APPLYMETRICBEATCONFIGMSG._serialized_start=10581
-  _APPLYMETRICBEATCONFIGMSG._serialized_end=10669
-  _APPLYHEARTBEATCONFIGMSG._serialized_start=10671
-  _APPLYHEARTBEATCONFIGMSG._serialized_end=10758
-  _STOPFILEBEATMSG._serialized_start=10760
-  _STOPFILEBEATMSG._serialized_end=10839
-  _STOPPACKETBEATMSG._serialized_start=10841
-  _STOPPACKETBEATMSG._serialized_end=10922
-  _STOPMETRICBEATMSG._serialized_start=10924
-  _STOPMETRICBEATMSG._serialized_end=11005
-  _STOPHEARTBEATMSG._serialized_start=11007
-  _STOPHEARTBEATMSG._serialized_end=11087
-  _STARTFILEBEATMSG._serialized_start=11089
-  _STARTFILEBEATMSG._serialized_end=11191
-  _STARTPACKETBEATMSG._serialized_start=11193
-  _STARTPACKETBEATMSG._serialized_end=11297
-  _STARTMETRICBEATMSG._serialized_start=11299
-  _STARTMETRICBEATMSG._serialized_end=11403
-  _STARTHEARTBEATMSG._serialized_start=11405
-  _STARTHEARTBEATMSG._serialized_end=11508
-  _STARTHOSTMONITORTHREADMSG._serialized_start=11510
-  _STARTHOSTMONITORTHREADMSG._serialized_end=11599
-  _STOPHEARTBEATSMSG._serialized_start=11601
-  _STOPHEARTBEATSMSG._serialized_end=11661
-  _STOPPACKETBEATSMSG._serialized_start=11663
-  _STOPPACKETBEATSMSG._serialized_end=11724
-  _STOPFILEBEATSMSG._serialized_start=11726
-  _STOPFILEBEATSMSG._serialized_end=11785
-  _STOPMETRICBEATSMSG._serialized_start=11787
-  _STOPMETRICBEATSMSG._serialized_end=11848
-  _STARTHOSTMONITORTHREADSMSG._serialized_start=11850
-  _STARTHOSTMONITORTHREADSMSG._serialized_end=11919
-  _STOPHOSTMANAGERMSG._serialized_start=11921
-  _STOPHOSTMANAGERMSG._serialized_end=12003
-  _STARTHOSTMANAGERMSG._serialized_start=12005
-  _STARTHOSTMANAGERMSG._serialized_end=12088
-  _STOPHOSTMANAGERSMSG._serialized_start=12090
-  _STOPHOSTMANAGERSMSG._serialized_end=12152
-  _EXECUTIONINFODTO._serialized_start=12155
-  _EXECUTIONINFODTO._serialized_end=12840
-  _RYUMANAGERSINFODTO._serialized_start=12843
-  _RYUMANAGERSINFODTO._serialized_end=13072
-  _RYUMANAGERSTATUSDTO._serialized_start=13075
-  _RYUMANAGERSTATUSDTO._serialized_end=13255
-  _HOSTMANAGERSINFODTO._serialized_start=13258
-  _HOSTMANAGERSINFODTO._serialized_end=13433
-  _HOSTMANAGERSTATUSESDTO._serialized_start=13435
-  _HOSTMANAGERSTATUSESDTO._serialized_end=13511
-  _HOSTMANAGERSTATUSDTO._serialized_start=13514
-  _HOSTMANAGERSTATUSDTO._serialized_end=13682
-  _KAFKAMANAGERSINFODTO._serialized_start=13685
-  _KAFKAMANAGERSINFODTO._serialized_end=13857
-  _KAFKASTATUSDTO._serialized_start=13859
-  _KAFKASTATUSDTO._serialized_end=13908
-  _OSSECIDSMANAGERSINFODTO._serialized_start=13911
-  _OSSECIDSMANAGERSINFODTO._serialized_end=14095
-  _OSSECIDSSTATUSDTO._serialized_start=14097
-  _OSSECIDSSTATUSDTO._serialized_end=14168
-  _SNORTIDSMANAGERSINFODTO._serialized_start=14171
-  _SNORTIDSMANAGERSINFODTO._serialized_end=14355
-  _SNORTIDSSTATUSDTO._serialized_start=14357
-  _SNORTIDSSTATUSDTO._serialized_end=14428
-  _GETEXECUTIONINFOMSG._serialized_start=14430
-  _GETEXECUTIONINFOMSG._serialized_end=14492
-  _STOPCONTAINERSOFEXECUTIONMSG._serialized_start=14494
-  _STOPCONTAINERSOFEXECUTIONMSG._serialized_end=14565
-  _RUNCONTAINERMSG._serialized_start=14567
-  _RUNCONTAINERMSG._serialized_end=14688
-  _STARTCONTAINERSOFEXECUTIONMSG._serialized_start=14690
-  _STARTCONTAINERSOFEXECUTIONMSG._serialized_end=14762
-  _GETELKMANAGERSINFOMSG._serialized_start=14764
-  _GETELKMANAGERSINFOMSG._serialized_end=14828
-  _ELKMANAGERSINFODTO._serialized_start=14831
-  _ELKMANAGERSINFODTO._serialized_end=15046
-  _STOPLOGSTASHSERVICEMSG._serialized_start=15048
-  _STOPLOGSTASHSERVICEMSG._serialized_end=15113
-  _STARTLOGSTASHSERVICEMSG._serialized_start=15115
-  _STARTLOGSTASHSERVICEMSG._serialized_end=15181
-  _STOPKIBANASERVICEMSG._serialized_start=15183
-  _STOPKIBANASERVICEMSG._serialized_end=15246
-  _STARTKIBANASERVICEMSG._serialized_start=15248
-  _STARTKIBANASERVICEMSG._serialized_end=15312
-  _STOPELASTICSERVICEMSG._serialized_start=15314
-  _STOPELASTICSERVICEMSG._serialized_end=15378
-  _STARTELASTICSERVICEMSG._serialized_start=15380
-  _STARTELASTICSERVICEMSG._serialized_end=15445
-  _STOPELKSTACKMSG._serialized_start=15447
-  _STOPELKSTACKMSG._serialized_end=15505
-  _ELKSTATUSDTO._serialized_start=15507
-  _ELKSTATUSDTO._serialized_end=15593
-  _GETELKSTACKSTATUSMSG._serialized_start=15595
-  _GETELKSTACKSTATUSMSG._serialized_end=15658
-  _STOPELKMANAGERMSG._serialized_start=15660
-  _STOPELKMANAGERMSG._serialized_end=15720
-  _STARTELKMANAGERMSG._serialized_start=15722
-  _STARTELKMANAGERMSG._serialized_end=15783
-  _GETDOCKERSTATSMANAGERSINFOMSG._serialized_start=15785
-  _GETDOCKERSTATSMANAGERSINFOMSG._serialized_end=15857
-  _DOCKERSTATSMANAGERSINFODTO._serialized_start=15860
-  _DOCKERSTATSMANAGERSINFODTO._serialized_end=16063
-  _REMOVEALLDOCKERNETWORKSMSG._serialized_start=16065
-  _REMOVEALLDOCKERNETWORKSMSG._serialized_end=16093
-  _REMOVEDOCKERNETWORKSMSG._serialized_start=16095
-  _REMOVEDOCKERNETWORKSMSG._serialized_end=16138
-  _DOCKERSTATSMONITORSTATUSDTO._serialized_start=16140
-  _DOCKERSTATSMONITORSTATUSDTO._serialized_end=16241
-  _GETDOCKERSTATSMANAGERSTATUSMSG._serialized_start=16243
-  _GETDOCKERSTATSMANAGERSTATUSMSG._serialized_end=16289
-  _STOPDOCKERSTATSMANAGERTHREADMSG._serialized_start=16291
-  _STOPDOCKERSTATSMANAGERTHREADMSG._serialized_end=16365
-  _CREATEEMULATIONNETWORKSMSG._serialized_start=16367
-  _CREATEEMULATIONNETWORKSMSG._serialized_end=16436
-  _LISTALLSTOPPEDCONTAINERSMSG._serialized_start=16438
-  _LISTALLSTOPPEDCONTAINERSMSG._serialized_end=16467
-  _STOPPEDCONTAINERSDTO._serialized_start=16469
-  _STOPPEDCONTAINERSDTO._serialized_end=16539
-  _LISTALLRUNNINGEMULATIONSMSG._serialized_start=16541
-  _LISTALLRUNNINGEMULATIONSMSG._serialized_end=16570
-  _RUNNINGEMULATIONSDTO._serialized_start=16572
-  _RUNNINGEMULATIONSDTO._serialized_end=16621
-  _LISTALLRUNNINGCONTAINERSMSG._serialized_start=16623
-  _LISTALLRUNNINGCONTAINERSMSG._serialized_end=16652
-  _RUNNINGCONTAINERSDTO._serialized_start=16654
-  _RUNNINGCONTAINERSDTO._serialized_end=16724
-  _DOCKERCONTAINERDTO._serialized_start=16726
-  _DOCKERCONTAINERDTO._serialized_end=16787
-  _STARTCONTAINERMSG._serialized_start=16789
-  _STARTCONTAINERMSG._serialized_end=16822
-  _STARTALLSTOPPEDCONTAINERSMSG._serialized_start=16824
-  _STARTALLSTOPPEDCONTAINERSMSG._serialized_end=16854
-  _LISTALLDOCKERNETWORKSMSG._serialized_start=16856
-  _LISTALLDOCKERNETWORKSMSG._serialized_end=16882
-  _DOCKERNETWORKSDTO._serialized_start=16884
-  _DOCKERNETWORKSDTO._serialized_end=16942
-  _CONTAINERIMAGESDTO._serialized_start=16944
-  _CONTAINERIMAGESDTO._serialized_end=17000
-  _CONTAINERIMAGEDTO._serialized_start=17002
-  _CONTAINERIMAGEDTO._serialized_end=17104
-  _LISTALLCONTAINERIMAGESMSG._serialized_start=17106
-  _LISTALLCONTAINERIMAGESMSG._serialized_end=17133
-  _REMOVECONTAINERIMAGEMSG._serialized_start=17135
-  _REMOVECONTAINERIMAGEMSG._serialized_end=17174
-  _REMOVEALLCONTAINERIMAGESMSG._serialized_start=17176
-  _REMOVEALLCONTAINERIMAGESMSG._serialized_end=17205
-  _REMOVEALLSTOPPEDCONTAINERSMSG._serialized_start=17207
-  _REMOVEALLSTOPPEDCONTAINERSMSG._serialized_end=17238
-  _REMOVECONTAINERMSG._serialized_start=17240
-  _REMOVECONTAINERMSG._serialized_end=17274
-  _STOPCONTAINERMSG._serialized_start=17276
-  _STOPCONTAINERMSG._serialized_end=17308
-  _STOPALLRUNNINGCONTAINERSMSG._serialized_start=17310
-  _STOPALLRUNNINGCONTAINERSMSG._serialized_end=17339
-  _GETTRAFFICMANAGERSINFOMSG._serialized_start=17341
-  _GETTRAFFICMANAGERSINFOMSG._serialized_end=17409
-  _TRAFFICMANAGERSINFODTO._serialized_start=17412
-  _TRAFFICMANAGERSINFODTO._serialized_end=17597
-  _TRAFFICMANAGERINFODTO._serialized_start=17599
-  _TRAFFICMANAGERINFODTO._serialized_end=17655
-  _CLIENTMANAGERSINFODTO._serialized_start=17658
-  _CLIENTMANAGERSINFODTO._serialized_end=17835
-  _GETCLIENTMANAGERSINFOMSG._serialized_start=17837
-  _GETCLIENTMANAGERSINFOMSG._serialized_end=17904
-  _STARTTRAFFICGENERATORMSG._serialized_start=17906
-  _STARTTRAFFICGENERATORMSG._serialized_end=17994
-  _STOPTRAFFICGENERATORMSG._serialized_start=17996
-  _STOPTRAFFICGENERATORMSG._serialized_end=18083
-  _STOPTRAFFICGENERATORSMSG._serialized_start=18085
-  _STOPTRAFFICGENERATORSMSG._serialized_end=18152
-  _GETNUMCLIENTSDTO._serialized_start=18155
-  _GETNUMCLIENTSDTO._serialized_end=18329
-  _GETNUMACTIVECLIENTSMSG._serialized_start=18331
-  _GETNUMACTIVECLIENTSMSG._serialized_end=18396
-  _STOPCLIENTPOPULATIONMSG._serialized_start=18398
-  _STOPCLIENTPOPULATIONMSG._serialized_end=18464
-  _STOPCLIENTMANAGERMSG._serialized_start=18466
-  _STOPCLIENTMANAGERMSG._serialized_end=18529
-  _STARTCLIENTMANAGERMSG._serialized_start=18531
-  _STARTCLIENTMANAGERMSG._serialized_end=18595
-  _STOPTRAFFICMANAGERSMSG._serialized_start=18597
-  _STOPTRAFFICMANAGERSMSG._serialized_end=18662
-  _STOPTRAFFICMANAGERMSG._serialized_start=18664
-  _STOPTRAFFICMANAGERMSG._serialized_end=18749
-  _STARTTRAFFICMANAGERMSG._serialized_start=18751
-  _STARTTRAFFICMANAGERMSG._serialized_end=18837
-  _CLEANALLEXECUTIONSMSG._serialized_start=18839
-  _CLEANALLEXECUTIONSMSG._serialized_end=18862
-  _STOPALLEXECUTIONSMSG._serialized_start=18864
-  _STOPALLEXECUTIONSMSG._serialized_end=18886
-  _STOPEXECUTIONMSG._serialized_start=18888
-  _STOPEXECUTIONMSG._serialized_end=18947
-  _CLEANEXECUTIONMSG._serialized_start=18949
-  _CLEANEXECUTIONMSG._serialized_end=19009
-  _STOPALLEXECUTIONSOFEMULATIONMSG._serialized_start=19011
-  _STOPALLEXECUTIONSOFEMULATIONMSG._serialized_end=19063
-  _CLEANALLEXECUTIONSOFEMULATIONMSG._serialized_start=19065
-  _CLEANALLEXECUTIONSOFEMULATIONMSG._serialized_end=19118
-  _GETCSLELOGFILESMSG._serialized_start=19120
-  _GETCSLELOGFILESMSG._serialized_end=19140
-  _GETLOGFILEMSG._serialized_start=19142
-  _GETLOGFILEMSG._serialized_end=19171
-  _STARTCONTAINERSINEXECUTIONMSG._serialized_start=19173
-  _STARTCONTAINERSINEXECUTIONMSG._serialized_end=19245
-  _ATTACHCONTAINERSTONETWORKSINEXECUTIONMSG._serialized_start=19247
-  _ATTACHCONTAINERSTONETWORKSINEXECUTIONMSG._serialized_end=19330
-  _INSTALLLIBRARIESMSG._serialized_start=19332
-  _INSTALLLIBRARIESMSG._serialized_end=19394
-  _APPLYKAFKACONFIGMSG._serialized_start=19396
-  _APPLYKAFKACONFIGMSG._serialized_end=19458
-  _STARTSDNCONTROLLERMSG._serialized_start=19460
-  _STARTSDNCONTROLLERMSG._serialized_end=19524
-  _APPLYRESOUCECONSTRAINTSMSG._serialized_start=19526
-  _APPLYRESOUCECONSTRAINTSMSG._serialized_end=19595
-  _CREATEOVSSWITCHESMSG._serialized_start=19597
-  _CREATEOVSSWITCHESMSG._serialized_end=19660
-  _PINGEXECUTIONMSG._serialized_start=19662
-  _PINGEXECUTIONMSG._serialized_end=19721
-  _CONFIGUREOVSMSG._serialized_start=19723
-  _CONFIGUREOVSMSG._serialized_end=19781
-  _STARTSDNCONTROLLERMONITORMSG._serialized_start=19783
-  _STARTSDNCONTROLLERMONITORMSG._serialized_end=19854
-  _CREATEUSERSMSG._serialized_start=19856
-  _CREATEUSERSMSG._serialized_end=19913
-  _CREATEVULNSMSG._serialized_start=19915
-  _CREATEVULNSMSG._serialized_end=19972
-  _CREATEFLAGSMSG._serialized_start=19974
-  _CREATEFLAGSMSG._serialized_end=20031
-  _CREATETOPOLOGYMSG._serialized_start=20033
-  _CREATETOPOLOGYMSG._serialized_end=20093
-  _STARTTRAFFICMANAGERSMSG._serialized_start=20095
-  _STARTTRAFFICMANAGERSMSG._serialized_end=20161
-  _STARTTRAFFICGENERATORSMSG._serialized_start=20163
-  _STARTTRAFFICGENERATORSMSG._serialized_end=20231
-  _STARTCLIENTPOPULATIONMSG._serialized_start=20233
-  _STARTCLIENTPOPULATIONMSG._serialized_end=20300
-  _STARTKAFKACLIENTPRODUCERMSG._serialized_start=20302
-  _STARTKAFKACLIENTPRODUCERMSG._serialized_end=20372
-  _STOPKAFKACLIENTPRODUCERMSG._serialized_start=20374
-  _STOPKAFKACLIENTPRODUCERMSG._serialized_end=20443
-  _STARTSNORTIDSESMSG._serialized_start=20445
-  _STARTSNORTIDSESMSG._serialized_end=20506
-  _STARTSNORTIDSESMONITORTHREADSMSG._serialized_start=20508
-  _STARTSNORTIDSESMONITORTHREADSMSG._serialized_end=20583
-  _STARTOSSECIDSESMSG._serialized_start=20585
-  _STARTOSSECIDSESMSG._serialized_end=20646
-  _STARTOSSECIDSESMONITORTHREADSMSG._serialized_start=20648
-  _STARTOSSECIDSESMONITORTHREADSMSG._serialized_end=20723
-  _STARTELKSTACKMSG._serialized_start=20725
-  _STARTELKSTACKMSG._serialized_end=20784
-  _STARTHOSTMANAGERSMSG._serialized_start=20786
-  _STARTHOSTMANAGERSMSG._serialized_end=20849
-  _APPLYFILEBEATCONFIGSMSG._serialized_start=20851
-  _APPLYFILEBEATCONFIGSMSG._serialized_end=20917
-  _APPLYPACKETBEATCONFIGSMSG._serialized_start=20919
-  _APPLYPACKETBEATCONFIGSMSG._serialized_end=20987
-  _APPLYMETRICBEATCONFIGSMSG._serialized_start=20989
-  _APPLYMETRICBEATCONFIGSMSG._serialized_end=21057
-  _APPLYHEARTBEATCONFIGSMSG._serialized_start=21059
-  _APPLYHEARTBEATCONFIGSMSG._serialized_end=21126
-  _STARTFILEBEATSMSG._serialized_start=21128
-  _STARTFILEBEATSMSG._serialized_end=21210
-  _STARTPACKETBEATSMSG._serialized_start=21212
-  _STARTPACKETBEATSMSG._serialized_end=21296
-  _STARTMETRICBEATSMSG._serialized_start=21298
-  _STARTMETRICBEATSMSG._serialized_end=21382
-  _STARTHEARTBEATSMSG._serialized_start=21384
-  _STARTHEARTBEATSMSG._serialized_end=21467
-  _GETDOCKERSTATSMANAGERLOGSMSG._serialized_start=21469
-  _GETDOCKERSTATSMANAGERLOGSMSG._serialized_end=21499
-  _GETPROMETHEUSLOGSMSG._serialized_start=21501
-  _GETPROMETHEUSLOGSMSG._serialized_end=21523
-  _GETNODEEXPORTERLOGSMSG._serialized_start=21525
-  _GETNODEEXPORTERLOGSMSG._serialized_end=21549
-  _GETCADVISORLOGSMSG._serialized_start=21551
-  _GETCADVISORLOGSMSG._serialized_end=21571
-  _GETPGADMINLOGSMSG._serialized_start=21573
-  _GETPGADMINLOGSMSG._serialized_end=21592
-  _GETGRAFANALOGSMSG._serialized_start=21594
-  _GETGRAFANALOGSMSG._serialized_end=21613
-  _GETNGINXLOGSMSG._serialized_start=21615
-  _GETNGINXLOGSMSG._serialized_end=21632
-  _GETDOCKERLOGSMSG._serialized_start=21634
-  _GETDOCKERLOGSMSG._serialized_end=21652
-  _GETPOSTGRESQLLOGSMSG._serialized_start=21654
-  _GETPOSTGRESQLLOGSMSG._serialized_end=21676
-  _GETFLASKLOGSMSG._serialized_start=21678
-  _GETFLASKLOGSMSG._serialized_end=21695
-  _LOGSDTO._serialized_start=21697
-  _LOGSDTO._serialized_end=21720
-  _OPERATIONOUTCOMEDTO._serialized_start=21722
-  _OPERATIONOUTCOMEDTO._serialized_end=21760
-  _GETNODESTATUSMSG._serialized_start=21762
-  _GETNODESTATUSMSG._serialized_end=21780
-  _NODESTATUSDTO._serialized_start=21783
-  _NODESTATUSDTO._serialized_end=22090
-  _SERVICESTATUSDTO._serialized_start=22092
-  _SERVICESTATUSDTO._serialized_end=22127
-  _STARTPOSTGRESQLMSG._serialized_start=22129
-  _STARTPOSTGRESQLMSG._serialized_end=22149
-  _STARTCADVISORMSG._serialized_start=22151
-  _STARTCADVISORMSG._serialized_end=22169
-  _STARTNODEEXPORTERMSG._serialized_start=22171
-  _STARTNODEEXPORTERMSG._serialized_end=22193
-  _STARTGRAFANAMSG._serialized_start=22195
-  _STARTGRAFANAMSG._serialized_end=22212
-  _STARTPROMETHEUSMSG._serialized_start=22214
-  _STARTPROMETHEUSMSG._serialized_end=22234
-  _STARTPGADMINMSG._serialized_start=22236
-  _STARTPGADMINMSG._serialized_end=22253
-  _STARTNGINXMSG._serialized_start=22255
-  _STARTNGINXMSG._serialized_end=22270
-  _STARTFLASKMSG._serialized_start=22272
-  _STARTFLASKMSG._serialized_end=22287
-  _STARTDOCKERSTATSMANAGERMSG._serialized_start=22289
-  _STARTDOCKERSTATSMANAGERMSG._serialized_end=22317
-  _STARTDOCKERSTATSMANAGERTHREADMSG._serialized_start=22319
-  _STARTDOCKERSTATSMANAGERTHREADMSG._serialized_end=22394
-  _STARTDOCKERENGINEMSG._serialized_start=22396
-  _STARTDOCKERENGINEMSG._serialized_end=22418
-  _STOPPOSTGRESQLMSG._serialized_start=22420
-  _STOPPOSTGRESQLMSG._serialized_end=22439
-  _STOPCADVISORMSG._serialized_start=22441
-  _STOPCADVISORMSG._serialized_end=22458
-  _STOPNODEEXPORTERMSG._serialized_start=22460
-  _STOPNODEEXPORTERMSG._serialized_end=22481
-  _STOPGRAFANAMSG._serialized_start=22483
-  _STOPGRAFANAMSG._serialized_end=22499
-  _STOPPROMETHEUSMSG._serialized_start=22501
-  _STOPPROMETHEUSMSG._serialized_end=22520
-  _STOPPGADMINMSG._serialized_start=22522
-  _STOPPGADMINMSG._serialized_end=22538
-  _STOPNGINXMSG._serialized_start=22540
-  _STOPNGINXMSG._serialized_end=22554
-  _STOPFLASKMSG._serialized_start=22556
-  _STOPFLASKMSG._serialized_end=22570
-  _STOPDOCKERSTATSMANAGERMSG._serialized_start=22572
-  _STOPDOCKERSTATSMANAGERMSG._serialized_end=22599
-  _STOPDOCKERENGINEMSG._serialized_start=22601
-  _STOPDOCKERENGINEMSG._serialized_end=22622
-  _CLUSTERMANAGER._serialized_start=22625
-  _CLUSTERMANAGER._serialized_end=36920
+  _STOPPIDMSG._serialized_start=25
+  _STOPPIDMSG._serialized_end=50
+  _CHECKPIDMSG._serialized_start=52
+  _CHECKPIDMSG._serialized_end=78
+  _STARTSPARKSERVERMSG._serialized_start=80
+  _STARTSPARKSERVERMSG._serialized_end=163
+  _STOPSPARKSERVERMSG._serialized_start=165
+  _STOPSPARKSERVERMSG._serialized_end=247
+  _STARTSPARKSERVERSMSG._serialized_start=249
+  _STARTSPARKSERVERSMSG._serialized_end=312
+  _STOPSPARKSERVERSMSG._serialized_start=314
+  _STOPSPARKSERVERSMSG._serialized_end=376
+  _GETEXECUTIONTIMESERIESDATAMSG._serialized_start=378
+  _GETEXECUTIONTIMESERIESDATAMSG._serialized_end=467
+  _EMULATIONMETRICSTIMESERIESDTO._serialized_start=470
+  _EMULATIONMETRICSTIMESERIESDTO._serialized_end=1911
+  _AVGPORTSTATISTICDICT._serialized_start=1913
+  _AVGPORTSTATISTICDICT._serialized_end=1984
+  _AGGFLOWSTATISTICDICT._serialized_start=1986
+  _AGGFLOWSTATISTICDICT._serialized_end=2057
+  _AVGFLOWSTATISTICDICT._serialized_start=2059
+  _AVGFLOWSTATISTICDICT._serialized_end=2130
+  _PORTSTATISTICDICT._serialized_start=2132
+  _PORTSTATISTICDICT._serialized_end=2197
+  _FLOWSTATISTICDICT._serialized_start=2199
+  _FLOWSTATISTICDICT._serialized_end=2264
+  _OSSECIDSALERTCOUNTERSDICT._serialized_start=2266
+  _OSSECIDSALERTCOUNTERSDICT._serialized_end=2347
+  _HOSTMETRICSDICT._serialized_start=2349
+  _HOSTMETRICSDICT._serialized_end=2414
+  _DOCKERSTATSDICT._serialized_start=2416
+  _DOCKERSTATSDICT._serialized_end=2477
+  _AVGPORTSTATISTICDTO._serialized_start=2480
+  _AVGPORTSTATISTICDTO._serialized_end=3052
+  _AVGFLOWSTATISTICDTO._serialized_start=3055
+  _AVGFLOWSTATISTICDTO._serialized_end=3326
+  _AGGFLOWSTATISTICDTO._serialized_start=3329
+  _AGGFLOWSTATISTICDTO._serialized_end=3467
+  _PORTSTATISTICDTO._serialized_start=3470
+  _PORTSTATISTICDTO._serialized_end=3973
+  _FLOWSTATISTICDTO._serialized_start=3976
+  _FLOWSTATISTICDTO._serialized_end=4268
+  _OSSECIDSALERTCOUNTERSDTO._serialized_start=4271
+  _OSSECIDSALERTCOUNTERSDTO._serialized_end=4468
+  _SNORTIDSALERTCOUNTERSDTO._serialized_start=4471
+  _SNORTIDSALERTCOUNTERSDTO._serialized_end=4652
+  _SNORTIDSIPALERTCOUNTERSDICT._serialized_start=4654
+  _SNORTIDSIPALERTCOUNTERSDICT._serialized_end=4739
+  _SNORTIDSALERTCOUNTERSDICT._serialized_start=4741
+  _SNORTIDSALERTCOUNTERSDICT._serialized_end=4822
+  _SNORTIDSRULECOUNTERSDICT._serialized_start=4824
+  _SNORTIDSRULECOUNTERSDICT._serialized_end=4903
+  _SNORTIDSIPALERTCOUNTERSDTO._serialized_start=4906
+  _SNORTIDSIPALERTCOUNTERSDTO._serialized_end=5107
+  _SNORTIDSRULECOUNTERSDTO._serialized_start=5109
+  _SNORTIDSRULECOUNTERSDTO._serialized_end=5203
+  _EMULATIONATTACKERACTIONDTO._serialized_start=5206
+  _EMULATIONATTACKERACTIONDTO._serialized_end=5450
+  _EMULATIONDEFENDERACTIONDTO._serialized_start=5453
+  _EMULATIONDEFENDERACTIONDTO._serialized_end=5656
+  _HOSTMETRICSDATADTO._serialized_start=5659
+  _HOSTMETRICSDATADTO._serialized_end=5865
+  _DOCKERSTATSDTO._serialized_start=5868
+  _DOCKERSTATSDTO._serialized_end=6116
+  _CLIENTPOPULATIONMETRICSDTO._serialized_start=6118
+  _CLIENTPOPULATIONMETRICSDTO._serialized_end=6227
+  _GETCLUSTERMANAGERLOGSMSG._serialized_start=6229
+  _GETCLUSTERMANAGERLOGSMSG._serialized_end=6255
+  _GETCONTAINERLOGSMSG._serialized_start=6257
+  _GETCONTAINERLOGSMSG._serialized_end=6340
+  _GETCLIENTMANAGERLOGSMSG._serialized_start=6342
+  _GETCLIENTMANAGERLOGSMSG._serialized_end=6408
+  _GETKAFKAMANAGERLOGSMSG._serialized_start=6410
+  _GETKAFKAMANAGERLOGSMSG._serialized_end=6475
+  _GETKAFKALOGSMSG._serialized_start=6477
+  _GETKAFKALOGSMSG._serialized_end=6535
+  _GETSNORTIDSLOGSMSG._serialized_start=6537
+  _GETSNORTIDSLOGSMSG._serialized_end=6619
+  _GETSNORTIDSMANAGERLOGSMSG._serialized_start=6621
+  _GETSNORTIDSMANAGERLOGSMSG._serialized_end=6710
+  _GETOSSECIDSMANAGERLOGSMSG._serialized_start=6712
+  _GETOSSECIDSMANAGERLOGSMSG._serialized_end=6801
+  _GETOSSECIDSLOGSMSG._serialized_start=6803
+  _GETOSSECIDSLOGSMSG._serialized_end=6885
+  _GETHOSTMANAGERLOGSMSG._serialized_start=6887
+  _GETHOSTMANAGERLOGSMSG._serialized_end=6972
+  _GETTRAFFICMANAGERLOGSMSG._serialized_start=6974
+  _GETTRAFFICMANAGERLOGSMSG._serialized_end=7062
+  _GETELKMANAGERLOGSMSG._serialized_start=7064
+  _GETELKMANAGERLOGSMSG._serialized_end=7127
+  _GETELKLOGSMSG._serialized_start=7129
+  _GETELKLOGSMSG._serialized_end=7185
+  _GETRYUMANAGERLOGSMSG._serialized_start=7187
+  _GETRYUMANAGERLOGSMSG._serialized_end=7250
+  _GETRYUCONTROLLERLOGSMSG._serialized_start=7252
+  _GETRYUCONTROLLERLOGSMSG._serialized_end=7318
+  _STOPRYUMONITORTHREADMSG._serialized_start=7320
+  _STOPRYUMONITORTHREADMSG._serialized_end=7386
+  _STARTRYUMONITORTHREADMSG._serialized_start=7388
+  _STARTRYUMONITORTHREADMSG._serialized_end=7455
+  _STOPHOSTMONITORTHREADSMSG._serialized_start=7457
+  _STOPHOSTMONITORTHREADSMSG._serialized_end=7525
+  _STOPHOSTMONITORTHREADMSG._serialized_start=7527
+  _STOPHOSTMONITORTHREADMSG._serialized_end=7615
+  _REMOVEKIBANATUNNELMSG._serialized_start=7617
+  _REMOVEKIBANATUNNELMSG._serialized_end=7681
+  _CREATEKIBANATUNNELMSG._serialized_start=7683
+  _CREATEKIBANATUNNELMSG._serialized_end=7747
+  _LISTKIBANATUNNELSMSG._serialized_start=7749
+  _LISTKIBANATUNNELSMSG._serialized_end=7771
+  _KIBANATUNNELSDTO._serialized_start=7773
+  _KIBANATUNNELSDTO._serialized_end=7826
+  _KIBANATUNNELDTO._serialized_start=7828
+  _KIBANATUNNELDTO._serialized_end=7912
+  _REMOVERYUTUNNELMSG._serialized_start=7914
+  _REMOVERYUTUNNELMSG._serialized_end=7975
+  _CREATERYUTUNNELMSG._serialized_start=7977
+  _CREATERYUTUNNELMSG._serialized_end=8038
+  _LISTRYUTUNNELSMSG._serialized_start=8040
+  _LISTRYUTUNNELSMSG._serialized_end=8059
+  _RYUTUNNELSDTO._serialized_start=8061
+  _RYUTUNNELSDTO._serialized_end=8108
+  _RYUTUNNELDTO._serialized_start=8110
+  _RYUTUNNELDTO._serialized_end=8191
+  _SNORTIDSMONITORTHREADSTATUSESDTO._serialized_start=8193
+  _SNORTIDSMONITORTHREADSTATUSESDTO._serialized_end=8273
+  _GETSNORTIDSMANAGERSINFOMSG._serialized_start=8275
+  _GETSNORTIDSMANAGERSINFOMSG._serialized_end=8344
+  _GETSNORTIDSMONITORTHREADSTATUSESMSG._serialized_start=8346
+  _GETSNORTIDSMONITORTHREADSTATUSESMSG._serialized_end=8424
+  _STOPSNORTIDSMONITORTHREADSMSG._serialized_start=8426
+  _STOPSNORTIDSMONITORTHREADSMSG._serialized_end=8498
+  _STOPSNORTIDSMANAGERMSG._serialized_start=8500
+  _STOPSNORTIDSMANAGERMSG._serialized_end=8586
+  _STARTSNORTIDSMANAGERMSG._serialized_start=8588
+  _STARTSNORTIDSMANAGERMSG._serialized_end=8675
+  _STOPSNORTIDSMANAGERSMSG._serialized_start=8677
+  _STOPSNORTIDSMANAGERSMSG._serialized_end=8743
+  _STARTSNORTIDSMANAGERSMSG._serialized_start=8745
+  _STARTSNORTIDSMANAGERSMSG._serialized_end=8812
+  _STARTSNORTMSG._serialized_start=8814
+  _STARTSNORTMSG._serialized_end=8891
+  _STARTSNORTIDSMONITORTHREADMSG._serialized_start=8893
+  _STARTSNORTIDSMONITORTHREADMSG._serialized_end=8986
+  _STARTSNORTIDSMONITORTHREADSMSG._serialized_start=8988
+  _STARTSNORTIDSMONITORTHREADSMSG._serialized_end=9061
+  _STOPSNORTMSG._serialized_start=9063
+  _STOPSNORTMSG._serialized_end=9139
+  _STOPSNORTIDSMONITORTHREADMSG._serialized_start=9141
+  _STOPSNORTIDSMONITORTHREADMSG._serialized_end=9233
+  _STOPSNORTIDSESMSG._serialized_start=9235
+  _STOPSNORTIDSESMSG._serialized_end=9295
+  _STOPSNORTIDSESMONITORTHREADSMSG._serialized_start=9297
+  _STOPSNORTIDSESMONITORTHREADSMSG._serialized_end=9371
+  _GETRYUMANAGERSINFOMSG._serialized_start=9373
+  _GETRYUMANAGERSINFOMSG._serialized_end=9437
+  _STOPRYUMONITORSERVICEMSG._serialized_start=9439
+  _STOPRYUMONITORSERVICEMSG._serialized_end=9506
+  _STARTRYUMONITORSERVICEMSG._serialized_start=9508
+  _STARTRYUMONITORSERVICEMSG._serialized_end=9576
+  _STOPRYUSERVICEMSG._serialized_start=9578
+  _STOPRYUSERVICEMSG._serialized_end=9638
+  _STARTRYUSERVICEMSG._serialized_start=9640
+  _STARTRYUSERVICEMSG._serialized_end=9701
+  _GETRYUSERVICESTATUSMSG._serialized_start=9703
+  _GETRYUSERVICESTATUSMSG._serialized_end=9768
+  _STOPRYUMANAGERMSG._serialized_start=9770
+  _STOPRYUMANAGERMSG._serialized_end=9830
+  _STARTRYUMANAGERMSG._serialized_start=9832
+  _STARTRYUMANAGERMSG._serialized_end=9893
+  _GETOSSECIDSMANAGERSINFOMSG._serialized_start=9895
+  _GETOSSECIDSMANAGERSINFOMSG._serialized_end=9964
+  _OSSECIDSMONITORTHREADSTATUSESDTO._serialized_start=9966
+  _OSSECIDSMONITORTHREADSTATUSESDTO._serialized_end=10046
+  _GETOSSECIDSMONITORTHREADSTATUSESMSG._serialized_start=10048
+  _GETOSSECIDSMONITORTHREADSTATUSESMSG._serialized_end=10126
+  _STOPOSSECIDSMONITORTHREADSMSG._serialized_start=10128
+  _STOPOSSECIDSMONITORTHREADSMSG._serialized_end=10200
+  _STOPOSSECIDSMONITORTHREADMSG._serialized_start=10202
+  _STOPOSSECIDSMONITORTHREADMSG._serialized_end=10294
+  _STARTOSSECIDSMONITORTHREADMSG._serialized_start=10296
+  _STARTOSSECIDSMONITORTHREADMSG._serialized_end=10389
+  _STOPOSSECIDSMANAGER._serialized_start=10391
+  _STOPOSSECIDSMANAGER._serialized_end=10474
+  _STARTOSSECIDSMANAGER._serialized_start=10476
+  _STARTOSSECIDSMANAGER._serialized_end=10560
+  _STOPOSSECIDSMANAGERS._serialized_start=10562
+  _STOPOSSECIDSMANAGERS._serialized_end=10625
+  _STARTOSSECIDSMANAGERS._serialized_start=10627
+  _STARTOSSECIDSMANAGERS._serialized_end=10691
+  _STARTOSSECIDSMSG._serialized_start=10693
+  _STARTOSSECIDSMSG._serialized_end=10773
+  _STOPOSSECIDSMSG._serialized_start=10775
+  _STOPOSSECIDSMSG._serialized_end=10854
+  _STARTOSSECIDSESMSG._serialized_start=10856
+  _STARTOSSECIDSESMSG._serialized_end=10917
+  _STOPOSSECIDSESMSG._serialized_start=10919
+  _STOPOSSECIDSESMSG._serialized_end=10979
+  _GETKAFKAMANAGERSINFOMSG._serialized_start=10981
+  _GETKAFKAMANAGERSINFOMSG._serialized_end=11047
+  _STARTKAFKASERVERMSG._serialized_start=11049
+  _STARTKAFKASERVERMSG._serialized_end=11111
+  _STOPKAFKASERVERMSG._serialized_start=11113
+  _STOPKAFKASERVERMSG._serialized_end=11174
+  _GETKAFKAMANAGERSTATUSMSG._serialized_start=11176
+  _GETKAFKAMANAGERSTATUSMSG._serialized_end=11243
+  _CREATEKAFKATOPICSMSG._serialized_start=11245
+  _CREATEKAFKATOPICSMSG._serialized_end=11308
+  _STOPKAFKAMANAGERMSG._serialized_start=11310
+  _STOPKAFKAMANAGERMSG._serialized_end=11372
+  _STARTKAFKAMANAGERMSG._serialized_start=11374
+  _STARTKAFKAMANAGERMSG._serialized_end=11437
+  _GETHOSTMANAGERSINFOMSG._serialized_start=11439
+  _GETHOSTMANAGERSINFOMSG._serialized_end=11504
+  _GETHOSTMONITORTHREADSSTATUSESMSG._serialized_start=11506
+  _GETHOSTMONITORTHREADSSTATUSESMSG._serialized_end=11581
+  _APPLYFILEBEATCONFIGMSG._serialized_start=11583
+  _APPLYFILEBEATCONFIGMSG._serialized_end=11669
+  _APPLYPACKETBEATCONFIGMSG._serialized_start=11671
+  _APPLYPACKETBEATCONFIGMSG._serialized_end=11759
+  _APPLYMETRICBEATCONFIGMSG._serialized_start=11761
+  _APPLYMETRICBEATCONFIGMSG._serialized_end=11849
+  _APPLYHEARTBEATCONFIGMSG._serialized_start=11851
+  _APPLYHEARTBEATCONFIGMSG._serialized_end=11938
+  _STOPFILEBEATMSG._serialized_start=11940
+  _STOPFILEBEATMSG._serialized_end=12019
+  _STOPPACKETBEATMSG._serialized_start=12021
+  _STOPPACKETBEATMSG._serialized_end=12102
+  _STOPMETRICBEATMSG._serialized_start=12104
+  _STOPMETRICBEATMSG._serialized_end=12185
+  _STOPHEARTBEATMSG._serialized_start=12187
+  _STOPHEARTBEATMSG._serialized_end=12267
+  _STARTFILEBEATMSG._serialized_start=12269
+  _STARTFILEBEATMSG._serialized_end=12371
+  _STARTPACKETBEATMSG._serialized_start=12373
+  _STARTPACKETBEATMSG._serialized_end=12477
+  _STARTMETRICBEATMSG._serialized_start=12479
+  _STARTMETRICBEATMSG._serialized_end=12583
+  _STARTHEARTBEATMSG._serialized_start=12585
+  _STARTHEARTBEATMSG._serialized_end=12688
+  _STARTHOSTMONITORTHREADMSG._serialized_start=12690
+  _STARTHOSTMONITORTHREADMSG._serialized_end=12779
+  _STOPHEARTBEATSMSG._serialized_start=12781
+  _STOPHEARTBEATSMSG._serialized_end=12841
+  _STOPPACKETBEATSMSG._serialized_start=12843
+  _STOPPACKETBEATSMSG._serialized_end=12904
+  _STOPFILEBEATSMSG._serialized_start=12906
+  _STOPFILEBEATSMSG._serialized_end=12965
+  _STOPMETRICBEATSMSG._serialized_start=12967
+  _STOPMETRICBEATSMSG._serialized_end=13028
+  _STARTHOSTMONITORTHREADSMSG._serialized_start=13030
+  _STARTHOSTMONITORTHREADSMSG._serialized_end=13099
+  _STOPHOSTMANAGERMSG._serialized_start=13101
+  _STOPHOSTMANAGERMSG._serialized_end=13183
+  _STARTHOSTMANAGERMSG._serialized_start=13185
+  _STARTHOSTMANAGERMSG._serialized_end=13268
+  _STOPHOSTMANAGERSMSG._serialized_start=13270
+  _STOPHOSTMANAGERSMSG._serialized_end=13332
+  _EXECUTIONINFODTO._serialized_start=13335
+  _EXECUTIONINFODTO._serialized_end=14020
+  _RYUMANAGERSINFODTO._serialized_start=14023
+  _RYUMANAGERSINFODTO._serialized_end=14252
+  _RYUMANAGERSTATUSDTO._serialized_start=14255
+  _RYUMANAGERSTATUSDTO._serialized_end=14435
+  _HOSTMANAGERSINFODTO._serialized_start=14438
+  _HOSTMANAGERSINFODTO._serialized_end=14613
+  _HOSTMANAGERSTATUSESDTO._serialized_start=14615
+  _HOSTMANAGERSTATUSESDTO._serialized_end=14691
+  _HOSTMANAGERSTATUSDTO._serialized_start=14694
+  _HOSTMANAGERSTATUSDTO._serialized_end=14862
+  _KAFKAMANAGERSINFODTO._serialized_start=14865
+  _KAFKAMANAGERSINFODTO._serialized_end=15037
+  _KAFKASTATUSDTO._serialized_start=15039
+  _KAFKASTATUSDTO._serialized_end=15088
+  _OSSECIDSMANAGERSINFODTO._serialized_start=15091
+  _OSSECIDSMANAGERSINFODTO._serialized_end=15275
+  _OSSECIDSSTATUSDTO._serialized_start=15277
+  _OSSECIDSSTATUSDTO._serialized_end=15348
+  _SNORTIDSMANAGERSINFODTO._serialized_start=15351
+  _SNORTIDSMANAGERSINFODTO._serialized_end=15535
+  _SNORTIDSSTATUSDTO._serialized_start=15537
+  _SNORTIDSSTATUSDTO._serialized_end=15608
+  _GETEXECUTIONINFOMSG._serialized_start=15610
+  _GETEXECUTIONINFOMSG._serialized_end=15672
+  _STOPCONTAINERSOFEXECUTIONMSG._serialized_start=15674
+  _STOPCONTAINERSOFEXECUTIONMSG._serialized_end=15745
+  _RUNCONTAINERMSG._serialized_start=15747
+  _RUNCONTAINERMSG._serialized_end=15868
+  _STARTCONTAINERSOFEXECUTIONMSG._serialized_start=15870
+  _STARTCONTAINERSOFEXECUTIONMSG._serialized_end=15942
+  _GETELKMANAGERSINFOMSG._serialized_start=15944
+  _GETELKMANAGERSINFOMSG._serialized_end=16008
+  _ELKMANAGERSINFODTO._serialized_start=16011
+  _ELKMANAGERSINFODTO._serialized_end=16226
+  _STOPLOGSTASHSERVICEMSG._serialized_start=16228
+  _STOPLOGSTASHSERVICEMSG._serialized_end=16293
+  _STARTLOGSTASHSERVICEMSG._serialized_start=16295
+  _STARTLOGSTASHSERVICEMSG._serialized_end=16361
+  _STOPKIBANASERVICEMSG._serialized_start=16363
+  _STOPKIBANASERVICEMSG._serialized_end=16426
+  _STARTKIBANASERVICEMSG._serialized_start=16428
+  _STARTKIBANASERVICEMSG._serialized_end=16492
+  _STOPELASTICSERVICEMSG._serialized_start=16494
+  _STOPELASTICSERVICEMSG._serialized_end=16558
+  _STARTELASTICSERVICEMSG._serialized_start=16560
+  _STARTELASTICSERVICEMSG._serialized_end=16625
+  _STOPELKSTACKMSG._serialized_start=16627
+  _STOPELKSTACKMSG._serialized_end=16685
+  _ELKSTATUSDTO._serialized_start=16687
+  _ELKSTATUSDTO._serialized_end=16773
+  _GETELKSTACKSTATUSMSG._serialized_start=16775
+  _GETELKSTACKSTATUSMSG._serialized_end=16838
+  _STOPELKMANAGERMSG._serialized_start=16840
+  _STOPELKMANAGERMSG._serialized_end=16900
+  _STARTELKMANAGERMSG._serialized_start=16902
+  _STARTELKMANAGERMSG._serialized_end=16963
+  _GETDOCKERSTATSMANAGERSINFOMSG._serialized_start=16965
+  _GETDOCKERSTATSMANAGERSINFOMSG._serialized_end=17037
+  _DOCKERSTATSMANAGERSINFODTO._serialized_start=17040
+  _DOCKERSTATSMANAGERSINFODTO._serialized_end=17243
+  _REMOVEALLDOCKERNETWORKSMSG._serialized_start=17245
+  _REMOVEALLDOCKERNETWORKSMSG._serialized_end=17273
+  _REMOVEDOCKERNETWORKSMSG._serialized_start=17275
+  _REMOVEDOCKERNETWORKSMSG._serialized_end=17318
+  _DOCKERSTATSMONITORSTATUSDTO._serialized_start=17320
+  _DOCKERSTATSMONITORSTATUSDTO._serialized_end=17421
+  _GETDOCKERSTATSMANAGERSTATUSMSG._serialized_start=17423
+  _GETDOCKERSTATSMANAGERSTATUSMSG._serialized_end=17469
+  _STOPDOCKERSTATSMANAGERTHREADMSG._serialized_start=17471
+  _STOPDOCKERSTATSMANAGERTHREADMSG._serialized_end=17545
+  _CREATEEMULATIONNETWORKSMSG._serialized_start=17547
+  _CREATEEMULATIONNETWORKSMSG._serialized_end=17616
+  _LISTALLSTOPPEDCONTAINERSMSG._serialized_start=17618
+  _LISTALLSTOPPEDCONTAINERSMSG._serialized_end=17647
+  _STOPPEDCONTAINERSDTO._serialized_start=17649
+  _STOPPEDCONTAINERSDTO._serialized_end=17719
+  _LISTALLRUNNINGEMULATIONSMSG._serialized_start=17721
+  _LISTALLRUNNINGEMULATIONSMSG._serialized_end=17750
+  _RUNNINGEMULATIONSDTO._serialized_start=17752
+  _RUNNINGEMULATIONSDTO._serialized_end=17801
+  _LISTALLRUNNINGCONTAINERSMSG._serialized_start=17803
+  _LISTALLRUNNINGCONTAINERSMSG._serialized_end=17832
+  _RUNNINGCONTAINERSDTO._serialized_start=17834
+  _RUNNINGCONTAINERSDTO._serialized_end=17904
+  _DOCKERCONTAINERDTO._serialized_start=17906
+  _DOCKERCONTAINERDTO._serialized_end=17967
+  _STARTCONTAINERMSG._serialized_start=17969
+  _STARTCONTAINERMSG._serialized_end=18002
+  _STARTALLSTOPPEDCONTAINERSMSG._serialized_start=18004
+  _STARTALLSTOPPEDCONTAINERSMSG._serialized_end=18034
+  _LISTALLDOCKERNETWORKSMSG._serialized_start=18036
+  _LISTALLDOCKERNETWORKSMSG._serialized_end=18062
+  _DOCKERNETWORKSDTO._serialized_start=18064
+  _DOCKERNETWORKSDTO._serialized_end=18122
+  _CONTAINERIMAGESDTO._serialized_start=18124
+  _CONTAINERIMAGESDTO._serialized_end=18180
+  _CONTAINERIMAGEDTO._serialized_start=18182
+  _CONTAINERIMAGEDTO._serialized_end=18284
+  _LISTALLCONTAINERIMAGESMSG._serialized_start=18286
+  _LISTALLCONTAINERIMAGESMSG._serialized_end=18313
+  _REMOVECONTAINERIMAGEMSG._serialized_start=18315
+  _REMOVECONTAINERIMAGEMSG._serialized_end=18354
+  _REMOVEALLCONTAINERIMAGESMSG._serialized_start=18356
+  _REMOVEALLCONTAINERIMAGESMSG._serialized_end=18385
+  _REMOVEALLSTOPPEDCONTAINERSMSG._serialized_start=18387
+  _REMOVEALLSTOPPEDCONTAINERSMSG._serialized_end=18418
+  _REMOVECONTAINERMSG._serialized_start=18420
+  _REMOVECONTAINERMSG._serialized_end=18454
+  _STOPCONTAINERMSG._serialized_start=18456
+  _STOPCONTAINERMSG._serialized_end=18488
+  _STOPALLRUNNINGCONTAINERSMSG._serialized_start=18490
+  _STOPALLRUNNINGCONTAINERSMSG._serialized_end=18519
+  _GETTRAFFICMANAGERSINFOMSG._serialized_start=18521
+  _GETTRAFFICMANAGERSINFOMSG._serialized_end=18589
+  _TRAFFICMANAGERSINFODTO._serialized_start=18592
+  _TRAFFICMANAGERSINFODTO._serialized_end=18777
+  _TRAFFICMANAGERINFODTO._serialized_start=18779
+  _TRAFFICMANAGERINFODTO._serialized_end=18835
+  _CLIENTMANAGERSINFODTO._serialized_start=18838
+  _CLIENTMANAGERSINFODTO._serialized_end=19015
+  _GETCLIENTMANAGERSINFOMSG._serialized_start=19017
+  _GETCLIENTMANAGERSINFOMSG._serialized_end=19084
+  _STARTTRAFFICGENERATORMSG._serialized_start=19086
+  _STARTTRAFFICGENERATORMSG._serialized_end=19174
+  _STOPTRAFFICGENERATORMSG._serialized_start=19176
+  _STOPTRAFFICGENERATORMSG._serialized_end=19263
+  _STOPTRAFFICGENERATORSMSG._serialized_start=19265
+  _STOPTRAFFICGENERATORSMSG._serialized_end=19332
+  _GETNUMCLIENTSDTO._serialized_start=19335
+  _GETNUMCLIENTSDTO._serialized_end=19509
+  _GETNUMACTIVECLIENTSMSG._serialized_start=19511
+  _GETNUMACTIVECLIENTSMSG._serialized_end=19576
+  _STOPCLIENTPOPULATIONMSG._serialized_start=19578
+  _STOPCLIENTPOPULATIONMSG._serialized_end=19644
+  _STOPCLIENTMANAGERMSG._serialized_start=19646
+  _STOPCLIENTMANAGERMSG._serialized_end=19709
+  _STARTCLIENTMANAGERMSG._serialized_start=19711
+  _STARTCLIENTMANAGERMSG._serialized_end=19775
+  _STOPTRAFFICMANAGERSMSG._serialized_start=19777
+  _STOPTRAFFICMANAGERSMSG._serialized_end=19842
+  _STOPTRAFFICMANAGERMSG._serialized_start=19844
+  _STOPTRAFFICMANAGERMSG._serialized_end=19929
+  _STARTTRAFFICMANAGERMSG._serialized_start=19931
+  _STARTTRAFFICMANAGERMSG._serialized_end=20017
+  _CLEANALLEXECUTIONSMSG._serialized_start=20019
+  _CLEANALLEXECUTIONSMSG._serialized_end=20042
+  _STOPALLEXECUTIONSMSG._serialized_start=20044
+  _STOPALLEXECUTIONSMSG._serialized_end=20066
+  _STOPEXECUTIONMSG._serialized_start=20068
+  _STOPEXECUTIONMSG._serialized_end=20127
+  _CLEANEXECUTIONMSG._serialized_start=20129
+  _CLEANEXECUTIONMSG._serialized_end=20189
+  _STOPALLEXECUTIONSOFEMULATIONMSG._serialized_start=20191
+  _STOPALLEXECUTIONSOFEMULATIONMSG._serialized_end=20243
+  _CLEANALLEXECUTIONSOFEMULATIONMSG._serialized_start=20245
+  _CLEANALLEXECUTIONSOFEMULATIONMSG._serialized_end=20298
+  _GETCSLELOGFILESMSG._serialized_start=20300
+  _GETCSLELOGFILESMSG._serialized_end=20320
+  _GETLOGFILEMSG._serialized_start=20322
+  _GETLOGFILEMSG._serialized_end=20351
+  _STARTCONTAINERSINEXECUTIONMSG._serialized_start=20353
+  _STARTCONTAINERSINEXECUTIONMSG._serialized_end=20425
+  _ATTACHCONTAINERSTONETWORKSINEXECUTIONMSG._serialized_start=20427
+  _ATTACHCONTAINERSTONETWORKSINEXECUTIONMSG._serialized_end=20510
+  _INSTALLLIBRARIESMSG._serialized_start=20512
+  _INSTALLLIBRARIESMSG._serialized_end=20574
+  _APPLYKAFKACONFIGMSG._serialized_start=20576
+  _APPLYKAFKACONFIGMSG._serialized_end=20638
+  _STARTSDNCONTROLLERMSG._serialized_start=20640
+  _STARTSDNCONTROLLERMSG._serialized_end=20704
+  _APPLYRESOUCECONSTRAINTSMSG._serialized_start=20706
+  _APPLYRESOUCECONSTRAINTSMSG._serialized_end=20775
+  _CREATEOVSSWITCHESMSG._serialized_start=20777
+  _CREATEOVSSWITCHESMSG._serialized_end=20840
+  _PINGEXECUTIONMSG._serialized_start=20842
+  _PINGEXECUTIONMSG._serialized_end=20901
+  _CONFIGUREOVSMSG._serialized_start=20903
+  _CONFIGUREOVSMSG._serialized_end=20961
+  _STARTSDNCONTROLLERMONITORMSG._serialized_start=20963
+  _STARTSDNCONTROLLERMONITORMSG._serialized_end=21034
+  _CREATEUSERSMSG._serialized_start=21036
+  _CREATEUSERSMSG._serialized_end=21093
+  _CREATEVULNSMSG._serialized_start=21095
+  _CREATEVULNSMSG._serialized_end=21152
+  _CREATEFLAGSMSG._serialized_start=21154
+  _CREATEFLAGSMSG._serialized_end=21211
+  _CREATETOPOLOGYMSG._serialized_start=21213
+  _CREATETOPOLOGYMSG._serialized_end=21273
+  _STARTTRAFFICMANAGERSMSG._serialized_start=21275
+  _STARTTRAFFICMANAGERSMSG._serialized_end=21341
+  _STARTTRAFFICGENERATORSMSG._serialized_start=21343
+  _STARTTRAFFICGENERATORSMSG._serialized_end=21411
+  _STARTCLIENTPOPULATIONMSG._serialized_start=21413
+  _STARTCLIENTPOPULATIONMSG._serialized_end=21480
+  _STARTKAFKACLIENTPRODUCERMSG._serialized_start=21482
+  _STARTKAFKACLIENTPRODUCERMSG._serialized_end=21552
+  _STOPKAFKACLIENTPRODUCERMSG._serialized_start=21554
+  _STOPKAFKACLIENTPRODUCERMSG._serialized_end=21623
+  _STARTSNORTIDSESMSG._serialized_start=21625
+  _STARTSNORTIDSESMSG._serialized_end=21686
+  _STARTSNORTIDSESMONITORTHREADSMSG._serialized_start=21688
+  _STARTSNORTIDSESMONITORTHREADSMSG._serialized_end=21763
+  _STARTOSSECIDSESMSG._serialized_start=21765
+  _STARTOSSECIDSESMSG._serialized_end=21826
+  _STARTOSSECIDSESMONITORTHREADSMSG._serialized_start=21828
+  _STARTOSSECIDSESMONITORTHREADSMSG._serialized_end=21903
+  _STARTELKSTACKMSG._serialized_start=21905
+  _STARTELKSTACKMSG._serialized_end=21964
+  _STARTHOSTMANAGERSMSG._serialized_start=21966
+  _STARTHOSTMANAGERSMSG._serialized_end=22029
+  _APPLYFILEBEATCONFIGSMSG._serialized_start=22031
+  _APPLYFILEBEATCONFIGSMSG._serialized_end=22097
+  _APPLYPACKETBEATCONFIGSMSG._serialized_start=22099
+  _APPLYPACKETBEATCONFIGSMSG._serialized_end=22167
+  _APPLYMETRICBEATCONFIGSMSG._serialized_start=22169
+  _APPLYMETRICBEATCONFIGSMSG._serialized_end=22237
+  _APPLYHEARTBEATCONFIGSMSG._serialized_start=22239
+  _APPLYHEARTBEATCONFIGSMSG._serialized_end=22306
+  _STARTFILEBEATSMSG._serialized_start=22308
+  _STARTFILEBEATSMSG._serialized_end=22390
+  _STARTPACKETBEATSMSG._serialized_start=22392
+  _STARTPACKETBEATSMSG._serialized_end=22476
+  _STARTMETRICBEATSMSG._serialized_start=22478
+  _STARTMETRICBEATSMSG._serialized_end=22562
+  _STARTHEARTBEATSMSG._serialized_start=22564
+  _STARTHEARTBEATSMSG._serialized_end=22647
+  _GETDOCKERSTATSMANAGERLOGSMSG._serialized_start=22649
+  _GETDOCKERSTATSMANAGERLOGSMSG._serialized_end=22679
+  _GETPROMETHEUSLOGSMSG._serialized_start=22681
+  _GETPROMETHEUSLOGSMSG._serialized_end=22703
+  _GETNODEEXPORTERLOGSMSG._serialized_start=22705
+  _GETNODEEXPORTERLOGSMSG._serialized_end=22729
+  _GETCADVISORLOGSMSG._serialized_start=22731
+  _GETCADVISORLOGSMSG._serialized_end=22751
+  _GETPGADMINLOGSMSG._serialized_start=22753
+  _GETPGADMINLOGSMSG._serialized_end=22772
+  _GETGRAFANALOGSMSG._serialized_start=22774
+  _GETGRAFANALOGSMSG._serialized_end=22793
+  _GETNGINXLOGSMSG._serialized_start=22795
+  _GETNGINXLOGSMSG._serialized_end=22812
+  _GETDOCKERLOGSMSG._serialized_start=22814
+  _GETDOCKERLOGSMSG._serialized_end=22832
+  _GETPOSTGRESQLLOGSMSG._serialized_start=22834
+  _GETPOSTGRESQLLOGSMSG._serialized_end=22856
+  _GETFLASKLOGSMSG._serialized_start=22858
+  _GETFLASKLOGSMSG._serialized_end=22875
+  _LOGSDTO._serialized_start=22877
+  _LOGSDTO._serialized_end=22900
+  _OPERATIONOUTCOMEDTO._serialized_start=22902
+  _OPERATIONOUTCOMEDTO._serialized_end=22940
+  _GETNODESTATUSMSG._serialized_start=22942
+  _GETNODESTATUSMSG._serialized_end=22960
+  _NODESTATUSDTO._serialized_start=22963
+  _NODESTATUSDTO._serialized_end=23270
+  _SERVICESTATUSDTO._serialized_start=23272
+  _SERVICESTATUSDTO._serialized_end=23307
+  _STARTPOSTGRESQLMSG._serialized_start=23309
+  _STARTPOSTGRESQLMSG._serialized_end=23329
+  _STARTCADVISORMSG._serialized_start=23331
+  _STARTCADVISORMSG._serialized_end=23349
+  _STARTNODEEXPORTERMSG._serialized_start=23351
+  _STARTNODEEXPORTERMSG._serialized_end=23373
+  _STARTGRAFANAMSG._serialized_start=23375
+  _STARTGRAFANAMSG._serialized_end=23392
+  _STARTPROMETHEUSMSG._serialized_start=23394
+  _STARTPROMETHEUSMSG._serialized_end=23414
+  _STARTPGADMINMSG._serialized_start=23416
+  _STARTPGADMINMSG._serialized_end=23433
+  _STARTNGINXMSG._serialized_start=23435
+  _STARTNGINXMSG._serialized_end=23450
+  _STARTFLASKMSG._serialized_start=23452
+  _STARTFLASKMSG._serialized_end=23467
+  _STARTDOCKERSTATSMANAGERMSG._serialized_start=23469
+  _STARTDOCKERSTATSMANAGERMSG._serialized_end=23497
+  _STARTDOCKERSTATSMANAGERTHREADMSG._serialized_start=23499
+  _STARTDOCKERSTATSMANAGERTHREADMSG._serialized_end=23574
+  _STARTDOCKERENGINEMSG._serialized_start=23576
+  _STARTDOCKERENGINEMSG._serialized_end=23598
+  _STOPPOSTGRESQLMSG._serialized_start=23600
+  _STOPPOSTGRESQLMSG._serialized_end=23619
+  _STOPCADVISORMSG._serialized_start=23621
+  _STOPCADVISORMSG._serialized_end=23638
+  _STOPNODEEXPORTERMSG._serialized_start=23640
+  _STOPNODEEXPORTERMSG._serialized_end=23661
+  _STOPGRAFANAMSG._serialized_start=23663
+  _STOPGRAFANAMSG._serialized_end=23679
+  _STOPPROMETHEUSMSG._serialized_start=23681
+  _STOPPROMETHEUSMSG._serialized_end=23700
+  _STOPPGADMINMSG._serialized_start=23702
+  _STOPPGADMINMSG._serialized_end=23718
+  _STOPNGINXMSG._serialized_start=23720
+  _STOPNGINXMSG._serialized_end=23734
+  _STOPFLASKMSG._serialized_start=23736
+  _STOPFLASKMSG._serialized_end=23750
+  _STOPDOCKERSTATSMANAGERMSG._serialized_start=23752
+  _STOPDOCKERSTATSMANAGERMSG._serialized_end=23779
+  _STOPDOCKERENGINEMSG._serialized_start=23781
+  _STOPDOCKERENGINEMSG._serialized_end=23802
+  _CLUSTERMANAGER._serialized_start=23805
+  _CLUSTERMANAGER._serialized_end=38462
 # @@protoc_insertion_point(module_scope)
```

### Comparing `csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py` & `csle_cluster-0.2.0/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1051,14 +1051,44 @@
                 response_deserializer=cluster__manager__pb2.LogsDTO.FromString,
                 )
         self.getExecutionTimeSeriesData = channel.unary_unary(
                 '/ClusterManager/getExecutionTimeSeriesData',
                 request_serializer=cluster__manager__pb2.GetExecutionTimeSeriesDataMsg.SerializeToString,
                 response_deserializer=cluster__manager__pb2.EmulationMetricsTimeSeriesDTO.FromString,
                 )
+        self.startSparkServers = channel.unary_unary(
+                '/ClusterManager/startSparkServers',
+                request_serializer=cluster__manager__pb2.StartSparkServersMsg.SerializeToString,
+                response_deserializer=cluster__manager__pb2.OperationOutcomeDTO.FromString,
+                )
+        self.stopSparkServers = channel.unary_unary(
+                '/ClusterManager/stopSparkServers',
+                request_serializer=cluster__manager__pb2.StopSparkServersMsg.SerializeToString,
+                response_deserializer=cluster__manager__pb2.OperationOutcomeDTO.FromString,
+                )
+        self.startSparkServer = channel.unary_unary(
+                '/ClusterManager/startSparkServer',
+                request_serializer=cluster__manager__pb2.StartSparkServerMsg.SerializeToString,
+                response_deserializer=cluster__manager__pb2.OperationOutcomeDTO.FromString,
+                )
+        self.stopSparkServer = channel.unary_unary(
+                '/ClusterManager/stopSparkServer',
+                request_serializer=cluster__manager__pb2.StopSparkServerMsg.SerializeToString,
+                response_deserializer=cluster__manager__pb2.OperationOutcomeDTO.FromString,
+                )
+        self.checkPid = channel.unary_unary(
+                '/ClusterManager/checkPid',
+                request_serializer=cluster__manager__pb2.CheckPidMsg.SerializeToString,
+                response_deserializer=cluster__manager__pb2.OperationOutcomeDTO.FromString,
+                )
+        self.stopPid = channel.unary_unary(
+                '/ClusterManager/stopPid',
+                request_serializer=cluster__manager__pb2.StopPidMsg.SerializeToString,
+                response_deserializer=cluster__manager__pb2.OperationOutcomeDTO.FromString,
+                )
 
 
 class ClusterManagerServicer(object):
     """Interface exported by the server
     """
 
     def getNodeStatus(self, request, context):
@@ -2305,14 +2335,50 @@
 
     def getExecutionTimeSeriesData(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def startSparkServers(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def stopSparkServers(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def startSparkServer(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def stopSparkServer(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def checkPid(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def stopPid(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_ClusterManagerServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'getNodeStatus': grpc.unary_unary_rpc_method_handler(
                     servicer.getNodeStatus,
                     request_deserializer=cluster__manager__pb2.GetNodeStatusMsg.FromString,
                     response_serializer=cluster__manager__pb2.NodeStatusDTO.SerializeToString,
@@ -3348,14 +3414,44 @@
                     response_serializer=cluster__manager__pb2.LogsDTO.SerializeToString,
             ),
             'getExecutionTimeSeriesData': grpc.unary_unary_rpc_method_handler(
                     servicer.getExecutionTimeSeriesData,
                     request_deserializer=cluster__manager__pb2.GetExecutionTimeSeriesDataMsg.FromString,
                     response_serializer=cluster__manager__pb2.EmulationMetricsTimeSeriesDTO.SerializeToString,
             ),
+            'startSparkServers': grpc.unary_unary_rpc_method_handler(
+                    servicer.startSparkServers,
+                    request_deserializer=cluster__manager__pb2.StartSparkServersMsg.FromString,
+                    response_serializer=cluster__manager__pb2.OperationOutcomeDTO.SerializeToString,
+            ),
+            'stopSparkServers': grpc.unary_unary_rpc_method_handler(
+                    servicer.stopSparkServers,
+                    request_deserializer=cluster__manager__pb2.StopSparkServersMsg.FromString,
+                    response_serializer=cluster__manager__pb2.OperationOutcomeDTO.SerializeToString,
+            ),
+            'startSparkServer': grpc.unary_unary_rpc_method_handler(
+                    servicer.startSparkServer,
+                    request_deserializer=cluster__manager__pb2.StartSparkServerMsg.FromString,
+                    response_serializer=cluster__manager__pb2.OperationOutcomeDTO.SerializeToString,
+            ),
+            'stopSparkServer': grpc.unary_unary_rpc_method_handler(
+                    servicer.stopSparkServer,
+                    request_deserializer=cluster__manager__pb2.StopSparkServerMsg.FromString,
+                    response_serializer=cluster__manager__pb2.OperationOutcomeDTO.SerializeToString,
+            ),
+            'checkPid': grpc.unary_unary_rpc_method_handler(
+                    servicer.checkPid,
+                    request_deserializer=cluster__manager__pb2.CheckPidMsg.FromString,
+                    response_serializer=cluster__manager__pb2.OperationOutcomeDTO.SerializeToString,
+            ),
+            'stopPid': grpc.unary_unary_rpc_method_handler(
+                    servicer.stopPid,
+                    request_deserializer=cluster__manager__pb2.StopPidMsg.FromString,
+                    response_serializer=cluster__manager__pb2.OperationOutcomeDTO.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'ClusterManager', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -6894,7 +6990,109 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/ClusterManager/getExecutionTimeSeriesData',
             cluster__manager__pb2.GetExecutionTimeSeriesDataMsg.SerializeToString,
             cluster__manager__pb2.EmulationMetricsTimeSeriesDTO.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def startSparkServers(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ClusterManager/startSparkServers',
+            cluster__manager__pb2.StartSparkServersMsg.SerializeToString,
+            cluster__manager__pb2.OperationOutcomeDTO.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def stopSparkServers(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ClusterManager/stopSparkServers',
+            cluster__manager__pb2.StopSparkServersMsg.SerializeToString,
+            cluster__manager__pb2.OperationOutcomeDTO.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def startSparkServer(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ClusterManager/startSparkServer',
+            cluster__manager__pb2.StartSparkServerMsg.SerializeToString,
+            cluster__manager__pb2.OperationOutcomeDTO.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def stopSparkServer(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ClusterManager/stopSparkServer',
+            cluster__manager__pb2.StopSparkServerMsg.SerializeToString,
+            cluster__manager__pb2.OperationOutcomeDTO.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def checkPid(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ClusterManager/checkPid',
+            cluster__manager__pb2.CheckPidMsg.SerializeToString,
+            cluster__manager__pb2.OperationOutcomeDTO.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def stopPid(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ClusterManager/stopPid',
+            cluster__manager__pb2.StopPidMsg.SerializeToString,
+            cluster__manager__pb2.OperationOutcomeDTO.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_manager_util.py` & `csle_cluster-0.2.0/src/csle_cluster/cluster_manager/cluster_manager_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from csle_common.controllers.emulation_env_controller import EmulationEnvController
 from csle_common.util.general_util import GeneralUtil
 from csle_common.util.emulation_util import EmulationUtil
 from csle_common.dao.emulation_config.emulation_metrics_time_series import EmulationMetricsTimeSeries
 from csle_common.dao.emulation_action.attacker.emulation_attacker_action import EmulationAttackerAction
 from csle_common.dao.emulation_action.defender.emulation_defender_action import EmulationDefenderAction
 from csle_collector.snort_ids_manager.snort_ids_alert_counters import SnortIdsAlertCounters
+from csle_collector.snort_ids_manager.snort_ids_rule_counters import SnortIdsRuleCounters
+from csle_collector.snort_ids_manager.snort_ids_ip_alert_counters import SnortIdsIPAlertCounters
 from csle_collector.ossec_ids_manager.ossec_ids_alert_counters import OSSECIdsAlertCounters
 from csle_collector.client_manager.client_population_metrics import ClientPopulationMetrics
 from csle_collector.docker_stats_manager.docker_stats import DockerStats
 from csle_collector.host_manager.host_metrics import HostMetrics
 import csle_collector.client_manager.client_manager_pb2
 import csle_collector.traffic_manager.traffic_manager_pb2
 import csle_collector.docker_stats_manager.docker_stats_manager_pb2
@@ -1437,25 +1439,25 @@
     @staticmethod
     def get_empty_elk_managers_info_dto() -> cluster_manager_pb2.ElkManagersInfoDTO:
         """
         :return: an empty ElkManagersInfoDTO
         """
         return cluster_manager_pb2.ElkManagersInfoDTO(
             ips=[], ports=[], emulationName="", executionId="", elkManagersRunning=[], elkManagersStatuses=[],
-            localKibanaPort=-1, physicalServerIp = ""
+            localKibanaPort=-1, physicalServerIp=""
         )
 
     @staticmethod
     def get_empty_ryu_managers_info_dto() -> cluster_manager_pb2.RyuManagersInfoDTO:
         """
         :return: an empty RyuManagersInfoDTO
         """
         return cluster_manager_pb2.RyuManagersInfoDTO(
             ips=[], ports=[], emulationName="", executionId=-1, ryuManagersRunning=[], ryuManagersStatuses=[],
-            physicalServerIp = "", localControllerWebPort=-1
+            physicalServerIp="", localControllerWebPort=-1
         )
 
     @staticmethod
     def get_empty_host_managers_info_dto() -> cluster_manager_pb2.HostManagersInfoDTO:
         """
         :return: an empty HostManagersInfoDTO
         """
@@ -1610,15 +1612,15 @@
                         remote_ip=execution.emulation_env_config.elk_config.container.docker_gw_bridge_ip,
                         emulation=execution.emulation_name, execution_id=execution.ip_first_octet)
             else:
                 tunnel_thread_dict = cluster_constants.KIBANA_TUNNELS.KIBANA_TUNNELS_DICT[
                     execution.emulation_env_config.elk_config.container.docker_gw_bridge_ip]
                 try:
                     response = get(f'{constants.HTTP.HTTP_PROTOCOL_PREFIX}{constants.COMMON.LOCALHOST}:'
-                                   f'{local_kibana_port}')
+                                   f'{local_kibana_port}', timeout=constants.HTTP.DEFAULT_TIMEOUT)
                     if response.status_code != constants.HTTPS.OK_STATUS_CODE:
                         tunnel_thread_dict[cluster_constants.KIBANA_TUNNELS.THREAD_PROPERTY].shutdown()
                         del cluster_constants.KIBANA_TUNNELS.KIBANA_TUNNELS_DICT[
                             execution.emulation_env_config.elk_config.container.docker_gw_bridge_ip]
                         EmulationEnvController.create_ssh_tunnel(
                             tunnels_dict=cluster_constants.KIBANA_TUNNELS.KIBANA_TUNNELS_DICT,
                             local_port=local_kibana_port,
@@ -1690,15 +1692,15 @@
                                 execution.emulation_env_config.sdn_controller_config.container.docker_gw_bridge_ip),
                             emulation=execution.emulation_name, execution_id=execution.ip_first_octet)
                 else:
                     tunnel_thread_dict = cluster_constants.RYU_TUNNELS.RYU_TUNNELS_DICT[
                         execution.emulation_env_config.sdn_controller_config.container.docker_gw_bridge_ip]
                     try:
                         response = get(f'{constants.HTTP.HTTP_PROTOCOL_PREFIX}{constants.COMMON.LOCALHOST}:'
-                                       f'{local_ryu_port}')
+                                       f'{local_ryu_port}', timeout=constants.HTTP.DEFAULT_TIMEOUT)
                         if response.status_code != constants.HTTPS.OK_STATUS_CODE:
                             tunnel_thread_dict[cluster_constants.RYU_TUNNELS.THREAD_PROPERTY].shutdown()
                             del cluster_constants.RYU_TUNNELS.RYU_TUNNELS_DICT[
                                 execution.emulation_env_config.sdn_controller_config.container.docker_gw_bridge_ip]
                             EmulationEnvController.create_ssh_tunnel(
                                 tunnels_dict=cluster_constants.RYU_TUNNELS.RYU_TUNNELS_DICT,
                                 local_port=local_ryu_port,
@@ -2072,16 +2074,16 @@
         :return: the converted objected
         """
         if client_population_metrics is None:
             return ClusterManagerUtil.get_empty_client_population_metrics_dto()
         else:
             return cluster_manager_pb2.ClientPopulationMetricsDTO(
                 ip=client_population_metrics.ip, ts=client_population_metrics.ts,
-                num_clients=client_population_metrics.num_clients, rate=client_population_metrics.rate
-            )
+                num_clients=client_population_metrics.num_clients, rate=client_population_metrics.rate,
+                service_time=client_population_metrics.service_time)
 
     @staticmethod
     def convert_client_population_metrics_dto_reverse(
             client_population_metrics_dto: cluster_manager_pb2.ClientPopulationMetricsDTO) -> ClientPopulationMetrics:
         """
         Converts a ClientPopulationMetricsDTO to a ClientPopulationMetrics
 
@@ -2090,23 +2092,24 @@
         """
         if client_population_metrics_dto is None:
             return ClusterManagerUtil.convert_client_population_metrics_dto_reverse(
                 ClusterManagerUtil.get_empty_client_population_metrics_dto())
         else:
             return ClientPopulationMetrics(
                 ip=client_population_metrics_dto.ip, ts=client_population_metrics_dto.ts,
-                num_clients=client_population_metrics_dto.num_clients, rate=client_population_metrics_dto.rate
+                num_clients=client_population_metrics_dto.num_clients, rate=client_population_metrics_dto.rate,
+                service_time=client_population_metrics_dto.service_time
             )
 
     @staticmethod
     def get_empty_client_population_metrics_dto() -> cluster_manager_pb2.ClientPopulationMetricsDTO:
         """
         :return: an empty ClientPopulationMetricsDTO
         """
-        return cluster_manager_pb2.ClientPopulationMetricsDTO(ip="", ts=-1., num_clients=0, rate=0.)
+        return cluster_manager_pb2.ClientPopulationMetricsDTO(ip="", ts=-1., num_clients=0, rate=0., service_time=0.)
 
     @staticmethod
     def client_population_metrics_dto_to_dict(
             client_population_metrics_dto: cluster_manager_pb2.ClientPopulationMetricsDTO) -> Dict[str, Any]:
         """
         Converts a ClientPopulationMetricsDTO to a dict
 
@@ -2114,14 +2117,15 @@
         :return: a dict representation of the DTO
         """
         d = {}
         d["ip"] = client_population_metrics_dto.ip
         d["ts"] = client_population_metrics_dto.ts
         d["num_clients"] = client_population_metrics_dto.num_clients
         d["rate"] = client_population_metrics_dto.rate
+        d["service_time"] = client_population_metrics_dto.service_time
         return d
 
     @staticmethod
     def convert_docker_stats_dto(docker_stats: DockerStats) -> cluster_manager_pb2.DockerStatsDTO:
         """
         Converts a DockerStats object to a DockerStatsDTO
 
@@ -2417,18 +2421,18 @@
         :param snort_ids_alert_counters: the object to convert
         :return: the converted objected
         """
         if snort_ids_alert_counters is None:
             return ClusterManagerUtil.get_empty_snort_ids_alert_counters_dto()
         else:
             return cluster_manager_pb2.SnortIdsAlertCountersDTO(
-                priority_alerts=snort_ids_alert_counters.priority_alerts,
-                class_alerts=snort_ids_alert_counters.class_alerts,
-                severe_alerts=snort_ids_alert_counters.severe_alerts,
-                warning_alerts=snort_ids_alert_counters.warning_alerts,
+                priority_alerts=list(map(lambda x: int(x), snort_ids_alert_counters.priority_alerts)),
+                class_alerts=list(map(lambda x: int(x), snort_ids_alert_counters.class_alerts)),
+                severe_alerts=int(snort_ids_alert_counters.severe_alerts),
+                warning_alerts=int(snort_ids_alert_counters.warning_alerts),
                 alerts_weighted_by_priority=snort_ids_alert_counters.alerts_weighted_by_priority,
                 ip=snort_ids_alert_counters.ip, ts=snort_ids_alert_counters.ts
             )
 
     @staticmethod
     def convert_snort_ids_alert_counters_dto_reverse(
             snort_ids_alert_counters_dto: cluster_manager_pb2.SnortIdsAlertCountersDTO) -> SnortIdsAlertCounters:
@@ -2478,14 +2482,153 @@
         d["total_alerts"] = snort_ids_alert_counters_dto.total_alerts
         d["warning_alerts"] = snort_ids_alert_counters_dto.warning_alerts
         d["severe_alerts"] = snort_ids_alert_counters_dto.severe_alerts
         d["alerts_weighted_by_priority"] = snort_ids_alert_counters_dto.alerts_weighted_by_priority
         return d
 
     @staticmethod
+    def convert_snort_ids_rule_counters_dto(snort_ids_rule_counters: SnortIdsRuleCounters) \
+            -> cluster_manager_pb2.SnortIdsRuleCountersDTO:
+        """
+        Converts a SnortIdsRuleCounters object to a SnortIdsRuleCountersDTO
+
+        :param snort_ids_rule_counters: the object to convert
+        :return: the converted objected
+        """
+        if snort_ids_rule_counters is None:
+            return ClusterManagerUtil.get_empty_snort_ids_rule_counters_dto()
+        else:
+            rule_ids = list(snort_ids_rule_counters.rule_alerts.keys())
+            rule_counters = list(snort_ids_rule_counters.rule_alerts.values())
+            return cluster_manager_pb2.SnortIdsRuleCountersDTO(
+                rule_ids=rule_ids, rule_alert_counts=rule_counters, ip=snort_ids_rule_counters.ip,
+                ts=snort_ids_rule_counters.ts)
+
+    @staticmethod
+    def convert_snort_ids_rule_counters_dto_reverse(
+            snort_ids_rule_counters_dto: cluster_manager_pb2.SnortIdsRuleCountersDTO) -> SnortIdsRuleCounters:
+        """
+        Converts a SnortIdsRuleCountersDTO to a SnortIdsRuleCounters
+
+        :param snort_ids_rule_counters_dto: the DTO to convert
+        :return: the converted DTO
+        """
+        if snort_ids_rule_counters_dto is None:
+            return ClusterManagerUtil.convert_snort_ids_rule_counters_dto_reverse(
+                ClusterManagerUtil.get_empty_snort_ids_rule_counters_dto())
+        else:
+            dto = SnortIdsRuleCounters()
+            rule_alerts = {}
+            for i in range(len(snort_ids_rule_counters_dto.rule_ids)):
+                rule_alerts[snort_ids_rule_counters_dto.rule_ids[i]] = snort_ids_rule_counters_dto.rule_alert_counts[i]
+            dto.rule_alerts = rule_alerts
+            dto.ip = snort_ids_rule_counters_dto.ip
+            dto.ts = snort_ids_rule_counters_dto.ts
+            return dto
+
+    @staticmethod
+    def get_empty_snort_ids_rule_counters_dto() -> cluster_manager_pb2.SnortIdsRuleCountersDTO:
+        """
+        :return: an empty SnortIdsAlertCountersDTO
+        """
+        return cluster_manager_pb2.SnortIdsRuleCountersDTO(ip="", ts=0.0, rule_ids=[], rule_alert_counts=[])
+
+    @staticmethod
+    def snort_ids_rule_counters_dto_to_dict(
+            snort_ids_rule_counters_dto: cluster_manager_pb2.SnortIdsRuleCountersDTO) -> Dict[str, Any]:
+        """
+        Converts a SnortIdsRuleCountersDTO to a dict
+
+        :param snort_ids_rule_counters_dto: the dto to convert
+        :return: a dict representation of the DTO
+        """
+        d = {}
+        d["ip"] = snort_ids_rule_counters_dto.ip
+        d["ts"] = snort_ids_rule_counters_dto.ts
+        d["rule_ids"] = list(snort_ids_rule_counters_dto.rule_ids)
+        d["rule_alert_counts"] = list(snort_ids_rule_counters_dto.rule_alert_counts)
+        return d
+
+    @staticmethod
+    def convert_snort_ids_ip_alert_counters_dto(snort_ids_ip_alert_counters: SnortIdsIPAlertCounters) \
+            -> cluster_manager_pb2.SnortIdsIpAlertCountersDTO:
+        """
+        Converts a SnortIdsIPAlertCounters object to a SnortIdsIpAlertCountersDTO
+
+        :param snort_ids_ip_alert_counters: the object to convert
+        :return: the converted objected
+        """
+        if snort_ids_ip_alert_counters is None:
+            return ClusterManagerUtil.get_empty_snort_ids_ip_alert_counters_dto()
+        else:
+            return cluster_manager_pb2.SnortIdsIpAlertCountersDTO(
+                priority_alerts=snort_ids_ip_alert_counters.priority_alerts,
+                class_alerts=snort_ids_ip_alert_counters.class_alerts,
+                severe_alerts=snort_ids_ip_alert_counters.severe_alerts,
+                warning_alerts=snort_ids_ip_alert_counters.warning_alerts,
+                alerts_weighted_by_priority=snort_ids_ip_alert_counters.alerts_weighted_by_priority,
+                ip=snort_ids_ip_alert_counters.ip, ts=snort_ids_ip_alert_counters.ts,
+                alert_ip=snort_ids_ip_alert_counters.alert_ip
+            )
+
+    @staticmethod
+    def convert_snort_ids_ip_alert_counters_dto_reverse(
+            snort_ids_ip_alert_counters_dto: cluster_manager_pb2.SnortIdsIpAlertCountersDTO) -> SnortIdsIPAlertCounters:
+        """
+        Converts a SnortIdsIpAlertCountersDTO to a SnortIdsIPAlertCounters
+
+        :param snort_ids_ip_alert_counters_dto: the DTO to convert
+        :return: the converted DTO
+        """
+        if snort_ids_ip_alert_counters_dto is None:
+            return ClusterManagerUtil.convert_snort_ids_ip_alert_counters_dto_reverse(
+                ClusterManagerUtil.get_empty_snort_ids_ip_alert_counters_dto())
+        else:
+            dto = SnortIdsIPAlertCounters()
+            dto.priority_alerts = snort_ids_ip_alert_counters_dto.priority_alerts
+            dto.class_alerts = snort_ids_ip_alert_counters_dto.class_alerts
+            dto.severe_alerts = snort_ids_ip_alert_counters_dto.severe_alerts
+            dto.warning_alerts = snort_ids_ip_alert_counters_dto.warning_alerts
+            dto.alerts_weighted_by_priority = snort_ids_ip_alert_counters_dto.alerts_weighted_by_priority
+            dto.ip = snort_ids_ip_alert_counters_dto.ip
+            dto.ts = snort_ids_ip_alert_counters_dto.ts
+            dto.alert_ip = snort_ids_ip_alert_counters_dto.alert_ip
+            return dto
+
+    @staticmethod
+    def get_empty_snort_ids_ip_alert_counters_dto() -> cluster_manager_pb2.SnortIdsIpAlertCountersDTO:
+        """
+        :return: an empty SnortIdsAlertCountersDTO
+        """
+        return cluster_manager_pb2.SnortIdsIpAlertCountersDTO(
+            priority_alerts=[], class_alerts=[], severe_alerts=0, warning_alerts=0, alerts_weighted_by_priority=0.0,
+            ip="", ts=0.0, alert_ip="")
+
+    @staticmethod
+    def snort_ids_ip_alert_counters_dto_to_dict(
+            snort_ids_alert_counters_dto: cluster_manager_pb2.SnortIdsIpAlertCountersDTO) -> Dict[str, Any]:
+        """
+        Converts a SnortIdsAlertCountersDTO to a dict
+
+        :param snort_ids_alert_counters_dto: the dto to convert
+        :return: a dict representation of the DTO
+        """
+        d = {}
+        d["ip"] = snort_ids_alert_counters_dto.ip
+        d["alert_ip"] = snort_ids_alert_counters_dto.alert_ip
+        d["ts"] = snort_ids_alert_counters_dto.ts
+        d["class_alerts"] = snort_ids_alert_counters_dto.class_alerts
+        d["priority_alerts"] = snort_ids_alert_counters_dto.priority_alerts
+        d["total_alerts"] = snort_ids_alert_counters_dto.total_alerts
+        d["warning_alerts"] = snort_ids_alert_counters_dto.warning_alerts
+        d["severe_alerts"] = snort_ids_alert_counters_dto.severe_alerts
+        d["alerts_weighted_by_priority"] = snort_ids_alert_counters_dto.alerts_weighted_by_priority
+        return d
+
+    @staticmethod
     def convert_ossec_ids_alert_counters_dto(ossec_ids_alert_counters: OSSECIdsAlertCounters) \
             -> cluster_manager_pb2.OSSECIdsAlertCountersDTO:
         """
         Converts a OSSECIdsAlertCounters object to a OSSECIdsAlertCountersDTO
 
         :param ossec_ids_alert_counters: the object to convert
         :return: the converted objected
@@ -2600,15 +2743,15 @@
 
     @staticmethod
     def get_empty_flow_statistic_dto() -> cluster_manager_pb2.FlowStatisticDTO:
         """
         :return: an empty FlowStatisticDTO
         """
         return cluster_manager_pb2.FlowStatisticDTO(
-            timestamp=0.0, datapath_id=-1, in_port=-1, out_port=-1, dst_mac_address="", num_packets=-1,
+            timestamp=0.0, datapath_id="", in_port="", out_port="", dst_mac_address="", num_packets=-1,
             num_bytes=-1, duration_nanoseconds=-1, duration_seconds=-1, hard_timeout=-1, idle_timeout=-1,
             priority=-1, cookie=-1)
 
     @staticmethod
     def flow_statistic_dto_to_dict(flow_statistic_dto: cluster_manager_pb2.FlowStatisticDTO) -> Dict[str, Any]:
         """
         Converts a FlowStatisticDTO to a dict
@@ -2692,15 +2835,15 @@
 
     @staticmethod
     def get_empty_port_statistic_dto() -> cluster_manager_pb2.PortStatisticDTO:
         """
         :return: an empty PortStatisticDTO
         """
         return cluster_manager_pb2.PortStatisticDTO(
-            timestamp=0.0, datapath_id=-1, port=-1, num_received_packets=-1, num_received_bytes=-1,
+            timestamp=0.0, datapath_id="", port=-1, num_received_packets=-1, num_received_bytes=-1,
             num_received_errors=-1, num_transmitted_packets=-1, num_transmitted_bytes=-1, num_transmitted_errors=-1,
             num_received_dropped=-1, num_transmitted_dropped=-1, num_received_frame_errors=-1,
             num_received_overrun_errors=-1, num_received_crc_errors=-1, num_collisions=-1, duration_nanoseconds=-1,
             duration_seconds=-1)
 
     @staticmethod
     def port_statistic_dto_to_dict(port_statistic_dto: cluster_manager_pb2.PortStatisticDTO) -> Dict[str, Any]:
@@ -2769,15 +2912,15 @@
 
     @staticmethod
     def get_empty_agg_flow_statistic_dto() -> cluster_manager_pb2.AggFlowStatisticDTO:
         """
         :return: an empty AggFlowStatisticDTO
         """
         return cluster_manager_pb2.AggFlowStatisticDTO(
-            timestamp=0.0, datapath_id=-1, total_num_packets=-1, total_num_bytes=-1, total_num_flows=-1)
+            timestamp=0.0, datapath_id="", total_num_packets=-1, total_num_bytes=-1, total_num_flows=-1)
 
     @staticmethod
     def agg_flow_statistic_dto_to_dict(agg_flow_statistic_dto: cluster_manager_pb2.AggFlowStatisticDTO) \
             -> Dict[str, Any]:
         """
         Converts a AggFlowStatisticDTO to a dict
 
@@ -2841,15 +2984,15 @@
 
     @staticmethod
     def get_empty_avg_flow_statistic_dto() -> cluster_manager_pb2.AvgFlowStatisticDTO:
         """
         :return: an empty AvgFlowStatisticDTO
         """
         return cluster_manager_pb2.AvgFlowStatisticDTO(
-            timestamp=0.0, datapath_id=-1, total_num_packets=-1, total_num_bytes=-1,
+            timestamp=0.0, datapath_id="", total_num_packets=-1, total_num_bytes=-1,
             avg_duration_nanoseconds=-1, avg_duration_seconds=-1, avg_hard_timeout=-1, avg_idle_timeout=-1,
             avg_priority=-1, avg_cookie=-1)
 
     @staticmethod
     def avg_flow_statistic_dto_to_dict(avg_flow_statistic_dto: cluster_manager_pb2.AvgFlowStatisticDTO) \
             -> Dict[str, Any]:
         """
@@ -2931,15 +3074,15 @@
 
     @staticmethod
     def get_empty_avg_port_statistic_dto() -> cluster_manager_pb2.AvgPortStatisticDTO:
         """
         :return: an empty AvgPortStatisticDTO
         """
         return cluster_manager_pb2.AvgPortStatisticDTO(
-            timestamp=0.0, datapath_id=-1, total_num_received_packets=0, total_num_received_bytes=0,
+            timestamp=0.0, datapath_id="", total_num_received_packets=0, total_num_received_bytes=0,
             total_num_received_errors=0, total_num_transmitted_packets=0, total_num_transmitted_bytes=0,
             total_num_transmitted_errors=0, total_num_received_dropped=0, total_num_transmitted_dropped=0,
             total_num_received_frame_errors=0, total_num_received_overrun_errors=0,
             total_num_received_crc_errors=0,
             total_num_collisions=0, avg_duration_nanoseconds=0, avg_duration_seconds=0)
 
     @staticmethod
@@ -3027,14 +3170,203 @@
         dtos = []
         for dto in docker_stats_dict.dtos.items():
             dtos.append(ClusterManagerUtil.docker_stats_dto_to_dict(dto))
         d["dtos"] = dtos
         return d
 
     @staticmethod
+    def convert_snort_ids_ip_alert_counters_dict(
+            snort_ids_ip_alert_counters_d: Dict[str, List[SnortIdsIPAlertCounters]]) \
+            -> List[cluster_manager_pb2.SnortIdsIpAlertCountersDict]:
+        """
+        Converts a dict to list of SnortIdsIpAlertCountersDict
+
+        :param snort_ids_ip_alert_counters_d: the dict to convert
+        :return: the converted objected
+        """
+        if snort_ids_ip_alert_counters_d is None:
+            return ClusterManagerUtil.get_empty_snort_ids_ip_alert_counters_dict()
+        else:
+            snort_ids_ip_alerts_dict_list = []
+            for k, v in snort_ids_ip_alert_counters_d.items():
+                snort_ids_ip_alerts_dict_list.append(cluster_manager_pb2.SnortIdsIpAlertCountersDict(
+                    key=k, dtos=list(map(lambda x: ClusterManagerUtil.convert_snort_ids_ip_alert_counters_dto(x), v))))
+            return snort_ids_ip_alerts_dict_list
+
+    @staticmethod
+    def convert_snort_ids_ip_alert_counters_dict_reverse(
+            snort_ids_ip_alerts_counters_dict: List[cluster_manager_pb2.SnortIdsIpAlertCountersDict]) \
+            -> Dict[str, List[SnortIdsIPAlertCounters]]:
+        """
+        Converts a list of SnortIdsIpAlertCountersDict to a dict
+
+        :param snort_ids_ip_alerts_counters_dict: the list to convert
+        :return: the converted DTO
+        """
+        if snort_ids_ip_alerts_counters_dict is None:
+            return ClusterManagerUtil.convert_snort_ids_ip_alert_counters_dict_reverse(
+                ClusterManagerUtil.get_empty_snort_ids_ip_alert_counters_dict())
+        else:
+            d = {}
+            for ds in snort_ids_ip_alerts_counters_dict:
+                d[ds.key] = list(map(lambda x: ClusterManagerUtil.convert_snort_ids_ip_alert_counters_dto_reverse(x),
+                                     ds.dtos))
+            return d
+
+    @staticmethod
+    def get_empty_snort_ids_ip_alert_counters_dict() -> List[cluster_manager_pb2.SnortIdsIpAlertCountersDict]:
+        """
+        :return: an empty SnortIdsIpAlertCountersDict
+        """
+        return []
+
+    @staticmethod
+    def snort_ids_ip_alert_counters_dict_to_dict(
+            snort_ids_ip_alert_counters_dict: cluster_manager_pb2.SnortIdsIpAlertCountersDict) -> Dict[str, Any]:
+        """
+        Converts a DTO to a dict
+
+        :param snort_ids_ip_alert_counters_dict: the DTO to convert
+        :return: the dict
+        """
+        d = {}
+        d["key"] = snort_ids_ip_alert_counters_dict.key
+        dtos = []
+        for dto in snort_ids_ip_alert_counters_dict.dtos.items():
+            dtos.append(ClusterManagerUtil.snort_ids_ip_alert_counters_dto_to_dict(dto))
+        d["dtos"] = dtos
+        return d
+
+    @staticmethod
+    def convert_snort_ids_alert_counters_dict(
+            snort_ids_alert_counters_d: Dict[str, List[SnortIdsAlertCounters]]) \
+            -> List[cluster_manager_pb2.SnortIdsAlertCountersDict]:
+        """
+        Converts a dict to list of SnortIdsAlertCountersDict
+
+        :param snort_ids_alert_counters_d: the dict to convert
+        :return: the converted objected
+        """
+        if snort_ids_alert_counters_d is None:
+            return ClusterManagerUtil.get_empty_snort_ids_alert_counters_dict()
+        else:
+            snort_ids_alerts_dict_list = []
+            for k, v in snort_ids_alert_counters_d.items():
+                snort_ids_alerts_dict_list.append(cluster_manager_pb2.SnortIdsAlertCountersDict(
+                    key=k, dtos=list(map(lambda x: ClusterManagerUtil.convert_snort_ids_alert_counters_dto(x), v))))
+            return snort_ids_alerts_dict_list
+
+    @staticmethod
+    def convert_snort_ids_alert_counters_dict_reverse(
+            snort_ids_alerts_counters_dict: List[cluster_manager_pb2.SnortIdsAlertCountersDict]) \
+            -> Dict[str, List[SnortIdsAlertCounters]]:
+        """
+        Converts a list of SnortIdsIpAlertCountersDict to a dict
+
+        :param snort_ids_alerts_counters_dict: the list to convert
+        :return: the converted DTO
+        """
+        if snort_ids_alerts_counters_dict is None:
+            return ClusterManagerUtil.convert_snort_ids_alert_counters_dict_reverse(
+                ClusterManagerUtil.get_empty_snort_ids_alert_counters_dict())
+        else:
+            d = {}
+            for ds in snort_ids_alerts_counters_dict:
+                d[ds.key] = list(map(lambda x: ClusterManagerUtil.convert_snort_ids_alert_counters_dto_reverse(x),
+                                     ds.dtos))
+            return d
+
+    @staticmethod
+    def get_empty_snort_ids_alert_counters_dict() -> List[cluster_manager_pb2.SnortIdsAlertCountersDict]:
+        """
+        :return: an empty SnortIdsAlertCountersDict
+        """
+        return []
+
+    @staticmethod
+    def snort_ids_alert_counters_dict_to_dict(
+            snort_ids_alert_counters_dict: cluster_manager_pb2.SnortIdsAlertCountersDict) -> Dict[str, Any]:
+        """
+        Converts a DTO to a dict
+
+        :param snort_ids_alert_counters_dict: the DTO to convert
+        :return: the dict
+        """
+        d = {}
+        d["key"] = snort_ids_alert_counters_dict.key
+        dtos = []
+        for dto in snort_ids_alert_counters_dict.dtos.items():
+            dtos.append(ClusterManagerUtil.snort_ids_alert_counters_dto_to_dict(dto))
+        d["dtos"] = dtos
+        return d
+
+    @staticmethod
+    def convert_snort_ids_rule_counters_dict(
+            snort_ids_rule_counters_d: Dict[str, List[SnortIdsRuleCounters]]) \
+            -> List[cluster_manager_pb2.SnortIdsRuleCountersDict]:
+        """
+        Converts a dict to list of SnortIdsRuleCountersDict
+
+        :param snort_ids_rule_counters_d: the dict to convert
+        :return: the converted objected
+        """
+        if snort_ids_rule_counters_d is None:
+            return ClusterManagerUtil.get_empty_snort_ids_rule_counters_dict()
+        else:
+            snort_ids_rule_dict_list = []
+            for k, v in snort_ids_rule_counters_d.items():
+                snort_ids_rule_dict_list.append(cluster_manager_pb2.SnortIdsRuleCountersDict(
+                    key=k, dtos=list(map(lambda x: ClusterManagerUtil.convert_snort_ids_rule_counters_dto(x), v))))
+            return snort_ids_rule_dict_list
+
+    @staticmethod
+    def convert_snort_ids_rule_counters_dict_reverse(
+            snort_ids_rule_counters_dict: List[cluster_manager_pb2.SnortIdsRuleCountersDict]) \
+            -> Dict[str, List[SnortIdsRuleCounters]]:
+        """
+        Converts a list of SnortIdsRuleCountersDict to a dict
+
+        :param snort_ids_rule_counters_dict: the list to convert
+        :return: the converted DTO
+        """
+        if snort_ids_rule_counters_dict is None:
+            return ClusterManagerUtil.convert_snort_ids_rule_counters_dict_reverse(
+                ClusterManagerUtil.get_empty_snort_ids_rule_counters_dict())
+        else:
+            d = {}
+            for ds in snort_ids_rule_counters_dict:
+                d[ds.key] = list(map(lambda x: ClusterManagerUtil.convert_snort_ids_rule_counters_dto_reverse(x),
+                                     ds.dtos))
+            return d
+
+    @staticmethod
+    def get_empty_snort_ids_rule_counters_dict() -> List[cluster_manager_pb2.SnortIdsRuleCountersDict]:
+        """
+        :return: an empty SnortIdsRuleCountersDict
+        """
+        return []
+
+    @staticmethod
+    def snort_ids_rule_counters_dict_to_dict(
+            snort_ids_rule_counters_dict: cluster_manager_pb2.SnortIdsAlertCountersDict) -> Dict[str, Any]:
+        """
+        Converts a DTO to a dict
+
+        :param snort_ids_rule_counters_dict: the DTO to convert
+        :return: the dict
+        """
+        d = {}
+        d["key"] = snort_ids_rule_counters_dict.key
+        dtos = []
+        for dto in snort_ids_rule_counters_dict.dtos.items():
+            dtos.append(ClusterManagerUtil.snort_ids_rule_counters_dto_to_dict(dto))
+        d["dtos"] = dtos
+        return d
+
+    @staticmethod
     def convert_host_metrics_dict(host_metrics_dict: Dict[str, List[HostMetrics]]) \
             -> List[cluster_manager_pb2.HostMetricsDict]:
         """
         Converts a dict to list of HostMetricsDict
 
         :param host_metrics_dict: the dict to convert
         :return: the converted objected
@@ -3424,15 +3756,15 @@
         """
         if avg_port_statistics_dict is None:
             return ClusterManagerUtil.convert_avg_port_statistic_dict_reverse(
                 ClusterManagerUtil.get_empty_avg_port_statistic_dict())
         else:
             d = {}
             for ds in avg_port_statistics_dict:
-                d[ds.key] = list(map(lambda x: ClusterManagerUtil.convert_avg_port_statistic_dto_reverse(x), ds.dto))
+                d[ds.key] = list(map(lambda x: ClusterManagerUtil.convert_avg_port_statistic_dto_reverse(x), ds.dtos))
             return d
 
     @staticmethod
     def get_empty_avg_port_statistic_dict() -> List[cluster_manager_pb2.AvgPortStatisticDict]:
         """
         :return: an empty AvgPortStatisticDict
         """
@@ -3464,28 +3796,32 @@
             client_metrics=[ClusterManagerUtil.get_empty_client_population_metrics_dto()],
             aggregated_docker_stats=[ClusterManagerUtil.get_empty_docker_stats_dto()],
             docker_host_stats=ClusterManagerUtil.get_empty_docker_stats_dict(),
             host_metrics=ClusterManagerUtil.get_empty_host_metrics_dict(),
             aggregated_host_metrics=[ClusterManagerUtil.get_empty_host_metrics_dto()],
             defender_actions=[ClusterManagerUtil.get_empty_emulation_defender_action_dto()],
             attacker_actions=[ClusterManagerUtil.get_empty_emulation_attacker_action_dto()],
-            snort_ids_metrics=[ClusterManagerUtil.get_empty_snort_ids_alert_counters_dto()],
+            agg_snort_ids_metrics=[ClusterManagerUtil.get_empty_snort_ids_alert_counters_dto()],
             emulation_id=-1,
             ossec_host_alert_counters=ClusterManagerUtil.get_empty_ossec_ids_alert_counters_dict(),
             aggregated_ossec_host_alert_counters=[ClusterManagerUtil.get_empty_ossec_ids_alert_counters_dto()],
             openflow_flow_stats=[ClusterManagerUtil.get_empty_flow_statistic_dto()],
             openflow_port_stats=[ClusterManagerUtil.get_empty_port_statistic_dto()],
             avg_openflow_flow_stats=[ClusterManagerUtil.get_empty_avg_flow_statistic_dto()],
             avg_openflow_port_stats=[ClusterManagerUtil.get_empty_avg_port_statistic_dto()],
             openflow_flow_metrics_per_switch=ClusterManagerUtil.get_empty_flow_statistic_dict(),
             openflow_port_metrics_per_switch=ClusterManagerUtil.get_empty_port_statistic_dict(),
             openflow_flow_avg_metrics_per_switch=ClusterManagerUtil.get_empty_flow_statistic_dict(),
             openflow_port_avg_metrics_per_switch=ClusterManagerUtil.get_empty_avg_port_statistic_dict(),
             agg_openflow_flow_metrics_per_switch=ClusterManagerUtil.get_empty_avg_flow_statistic_dict(),
-            agg_openflow_flow_stats=[ClusterManagerUtil.get_empty_agg_flow_statistic_dto()]
+            agg_openflow_flow_stats=[ClusterManagerUtil.get_empty_agg_flow_statistic_dto()],
+            agg_snort_ids_rule_metrics=[ClusterManagerUtil.get_empty_snort_ids_rule_counters_dto()],
+            snort_ids_ip_metrics=ClusterManagerUtil.get_empty_snort_ids_ip_alert_counters_dict(),
+            snort_alert_metrics_per_ids=ClusterManagerUtil.get_empty_snort_ids_alert_counters_dict(),
+            snort_rule_metrics_per_ids=ClusterManagerUtil.get_empty_snort_ids_rule_counters_dict()
         )
 
     @staticmethod
     def convert_emulation_metrics_time_series_dto(time_series_dto: EmulationMetricsTimeSeries) \
             -> cluster_manager_pb2.EmulationMetricsTimeSeriesDTO:
         """
         Converts a EmulationMetricsTimeSeries to a EmulationMetricsTimeSeriesDTO
@@ -3505,16 +3841,16 @@
                 host_metrics=ClusterManagerUtil.convert_host_metrics_dict(time_series_dto.host_metrics),
                 aggregated_host_metrics=list(map(lambda x: ClusterManagerUtil.convert_host_metrics_dto(x),
                                                  time_series_dto.aggregated_host_metrics)),
                 defender_actions=list(map(lambda x: ClusterManagerUtil.convert_emulation_defender_action_dto(x),
                                           time_series_dto.defender_actions)),
                 attacker_actions=list(map(lambda x: ClusterManagerUtil.convert_emulation_attacker_action_dto(x),
                                           time_series_dto.attacker_actions)),
-                snort_ids_metrics=list(map(lambda x: ClusterManagerUtil.convert_snort_ids_alert_counters_dto(x),
-                                           time_series_dto.snort_ids_metrics)),
+                agg_snort_ids_metrics=list(map(lambda x: ClusterManagerUtil.convert_snort_ids_alert_counters_dto(x),
+                                               time_series_dto.agg_snort_ids_metrics)),
                 emulation_id=time_series_dto.emulation_env_config.id,
                 ossec_host_alert_counters=ClusterManagerUtil.convert_ossec_ids_alert_counters_dict(
                     time_series_dto.ossec_host_alert_counters),
                 aggregated_ossec_host_alert_counters=list(
                     map(lambda x: ClusterManagerUtil.convert_ossec_ids_alert_counters_dto(x),
                         time_series_dto.aggregated_ossec_host_alert_counters)),
                 openflow_flow_stats=list(map(lambda x: ClusterManagerUtil.convert_flow_statistics_dto(x),
@@ -3532,15 +3868,23 @@
                 openflow_flow_avg_metrics_per_switch=ClusterManagerUtil.convert_avg_flow_statistic_dict(
                     time_series_dto.openflow_flow_avg_metrics_per_switch),
                 openflow_port_avg_metrics_per_switch=ClusterManagerUtil.convert_avg_port_statistic_dict(
                     time_series_dto.openflow_port_avg_metrics_per_switch),
                 agg_openflow_flow_metrics_per_switch=ClusterManagerUtil.convert_agg_flow_statistic_dict(
                     time_series_dto.agg_openflow_flow_metrics_per_switch),
                 agg_openflow_flow_stats=list(map(lambda x: ClusterManagerUtil.convert_agg_flow_statistic_dto(x),
-                                                 time_series_dto.agg_openflow_flow_stats))
+                                                 time_series_dto.agg_openflow_flow_stats)),
+                agg_snort_ids_rule_metrics=list(map(lambda x: ClusterManagerUtil.convert_snort_ids_rule_counters_dto(x),
+                                                    time_series_dto.agg_snort_ids_rule_metrics)),
+                snort_ids_ip_metrics=ClusterManagerUtil.convert_snort_ids_ip_alert_counters_dict(
+                    time_series_dto.snort_ids_ip_metrics),
+                snort_rule_metrics_per_ids=ClusterManagerUtil.convert_snort_ids_rule_counters_dict(
+                    time_series_dto.snort_rule_metrics_per_ids),
+                snort_alert_metrics_per_ids=ClusterManagerUtil.convert_snort_ids_alert_counters_dict(
+                    time_series_dto.snort_alert_metrics_per_ids)
             )
 
     @staticmethod
     def convert_emulation_metrics_time_series_dto_reverse(
             time_series_dto: cluster_manager_pb2.EmulationMetricsTimeSeriesDTO) -> EmulationMetricsTimeSeries:
         """
         Converts a EmulationMetricsTimeSeriesDTO to a EmulationMetricsTimeSeries
@@ -3563,16 +3907,17 @@
                 host_metrics=ClusterManagerUtil.convert_host_metrics_dict_reverse(time_series_dto.host_metrics),
                 aggregated_host_metrics=list(map(lambda x: ClusterManagerUtil.convert_host_metrics_dto_reverse(x),
                                                  time_series_dto.aggregated_host_metrics)),
                 defender_actions=list(map(lambda x: ClusterManagerUtil.convert_emulation_defender_action_dto_reverse(x),
                                           time_series_dto.defender_actions)),
                 attacker_actions=list(map(lambda x: ClusterManagerUtil.convert_emulation_attacker_action_dto_reverse(x),
                                           time_series_dto.attacker_actions)),
-                snort_ids_metrics=list(map(lambda x: ClusterManagerUtil.convert_snort_ids_alert_counters_dto_reverse(x),
-                                           time_series_dto.snort_ids_metrics)),
+                agg_snort_ids_metrics=list(
+                    map(lambda x: ClusterManagerUtil.convert_snort_ids_alert_counters_dto_reverse(x),
+                        time_series_dto.agg_snort_ids_metrics)),
                 emulation_env_config=emulation_config,
                 ossec_host_alert_counters=ClusterManagerUtil.convert_ossec_ids_alert_counters_dict_reverse(
                     time_series_dto.ossec_host_alert_counters),
                 aggregated_ossec_host_alert_counters=list(
                     map(lambda x: ClusterManagerUtil.convert_ossec_ids_alert_counters_dto_reverse(x),
                         time_series_dto.aggregated_ossec_host_alert_counters)),
                 openflow_flow_stats=list(map(lambda x: ClusterManagerUtil.convert_flow_statistic_dto_reverse(x),
@@ -3590,15 +3935,24 @@
                 openflow_flow_avg_metrics_per_switch=ClusterManagerUtil.convert_avg_flow_statistic_dict_reverse(
                     time_series_dto.openflow_flow_avg_metrics_per_switch),
                 openflow_port_avg_metrics_per_switch=ClusterManagerUtil.convert_avg_port_statistic_dict_reverse(
                     time_series_dto.openflow_port_avg_metrics_per_switch),
                 agg_openflow_flow_metrics_per_switch=ClusterManagerUtil.convert_agg_flow_statistic_dict_reverse(
                     time_series_dto.agg_openflow_flow_metrics_per_switch),
                 agg_openflow_flow_stats=list(map(lambda x: ClusterManagerUtil.convert_agg_flow_statistic_dto_reverse(x),
-                                                 time_series_dto.agg_openflow_flow_stats))
+                                                 time_series_dto.agg_openflow_flow_stats)),
+                agg_snort_ids_rule_metrics=list(
+                    map(lambda x: ClusterManagerUtil.convert_snort_ids_rule_counters_dto_reverse(x),
+                        time_series_dto.agg_snort_ids_rule_metrics)),
+                snort_ids_ip_metrics=ClusterManagerUtil.convert_snort_ids_ip_alert_counters_dict_reverse(
+                    time_series_dto.snort_ids_ip_metrics),
+                snort_rule_metrics_per_ids=ClusterManagerUtil.convert_snort_ids_rule_counters_dict_reverse(
+                    time_series_dto.snort_rule_metrics_per_ids),
+                snort_alert_metrics_per_ids=ClusterManagerUtil.convert_snort_ids_alert_counters_dict_reverse(
+                    time_series_dto.snort_alert_metrics_per_ids)
             )
 
     @staticmethod
     def emulation_metrics_time_series_dto_to_dict(time_series_dto: cluster_manager_pb2.EmulationMetricsTimeSeriesDTO) \
             -> Dict[str, Any]:
         """
         Converts a EmulationMetricsTimeSeriesDTO to a dict
@@ -3617,16 +3971,16 @@
                                      time_series_dto.host_metrics))
         d["aggregated_host_metrics"] = list(map(lambda x: ClusterManagerUtil.host_metrics_dto_to_dict(x),
                                                 time_series_dto.aggregated_host_metrics))
         d["defender_actions"] = list(map(lambda x: ClusterManagerUtil.emulation_defender_action_dto_to_dict(x),
                                          time_series_dto.defender_actions))
         d["attacker_actions"] = list(map(lambda x: ClusterManagerUtil.emulation_attacker_action_dto_to_dict(x),
                                          time_series_dto.attacker_actions))
-        d["snort_ids_metrics"] = list(map(lambda x: ClusterManagerUtil.snort_ids_alert_counters_dto_to_dict(x),
-                                          time_series_dto.snort_ids_metrics))
+        d["agg_snort_ids_metrics"] = list(map(lambda x: ClusterManagerUtil.snort_ids_alert_counters_dto_to_dict(x),
+                                              time_series_dto.agg_snort_ids_metrics))
         d["emulation_id"] = time_series_dto.emulation_id
         d["ossec_host_alert_counters"] = list(map(lambda x: ClusterManagerUtil.ossec_ids_alert_counters_dict_to_dict(x),
                                                   time_series_dto.ossec_host_alert_counters))
         d["aggregated_ossec_host_alert_counters"] = list(
             map(lambda x: ClusterManagerUtil.ossec_ids_alert_counters_dto_to_dict(x),
                 time_series_dto.aggregated_ossec_host_alert_counters))
         d["openflow_flow_stats"] = list(map(lambda x: ClusterManagerUtil.flow_statistic_dto_to_dict(x),
@@ -3648,8 +4002,17 @@
             map(lambda x: ClusterManagerUtil.avg_port_statistics_dict_to_dict(x),
                 time_series_dto.openflow_port_avg_metrics_per_switch))
         d["agg_openflow_flow_metrics_per_switch"] = list(
             map(lambda x: ClusterManagerUtil.agg_flow_statistics_dict_to_dict(x),
                 time_series_dto.agg_openflow_flow_metrics_per_switch))
         d["agg_openflow_flow_stats"] = list(map(lambda x: ClusterManagerUtil.agg_flow_statistic_dto_to_dict(x),
                                                 time_series_dto.agg_openflow_flow_stats))
+        d["agg_snort_ids_rule_metrics"] = list(map(lambda x: ClusterManagerUtil.snort_ids_rule_counters_dto_to_dict(x),
+                                                   time_series_dto.agg_snort_ids_rule_metrics))
+        d["snort_ids_ip_metrics"] = list(map(lambda x: ClusterManagerUtil.snort_ids_ip_alert_counters_dict_to_dict(x),
+                                             time_series_dto.snort_ids_ip_metrics))
+        d["snort_rule_metrics_per_ids"] = list(map(lambda x: ClusterManagerUtil.snort_ids_rule_counters_dict_to_dict(x),
+                                                   time_series_dto.snort_rule_metrics_per_ids))
+        d["snort_alert_metrics_per_ids"] = list(
+            map(lambda x: ClusterManagerUtil.snort_ids_alert_counters_dict_to_dict(x),
+                time_series_dto.snort_alert_metrics_per_ids))
         return d
```

### Comparing `csle_cluster-0.1.9/src/csle_cluster/cluster_manager/query_cluster_manager.py` & `csle_cluster-0.2.0/src/csle_cluster/cluster_manager/query_cluster_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -4112,15 +4112,15 @@
     logs_dto = stub.getClusterManagerLogs(get_msg, timeout=timeout)
     return logs_dto
 
 
 def get_execution_time_series_data(
         stub: csle_cluster.cluster_manager.cluster_manager_pb2_grpc.ClusterManagerStub,
         emulation: str, ip_first_octet: int, minutes: int,
-        timeout=constants.GRPC.TIMEOUT_SECONDS) \
+        timeout=constants.GRPC.OPERATION_TIMEOUT_SECONDS) \
         -> csle_cluster.cluster_manager.cluster_manager_pb2.EmulationMetricsTimeSeriesDTO:
     """
     Fetches the logs of the cluster manager on a given physical node
 
     :param stub: the stub to send the remote gRPC to the server
     :param timeout: the GRPC timeout (seconds)
     :param emulation: the name of the emulation
@@ -4129,7 +4129,127 @@
     :return: a DTO with the time series data
     """
     get_msg = csle_cluster.cluster_manager.cluster_manager_pb2.GetExecutionTimeSeriesDataMsg(
         emulation=emulation, ipFirstOctet=ip_first_octet, minutes=minutes
     )
     logs_dto = stub.getExecutionTimeSeriesData(get_msg, timeout=timeout)
     return logs_dto
+
+
+def start_spark_servers(
+        stub: csle_cluster.cluster_manager.cluster_manager_pb2_grpc.ClusterManagerStub,
+        emulation: str, ip_first_octet: int,
+        timeout=constants.GRPC.OPERATION_TIMEOUT_SECONDS) \
+        -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
+    """
+    Starts the Spark servers of a given execution
+
+    :param stub: the stub to send the remote gRPC to the server
+    :param timeout: the GRPC timeout (seconds)
+    :param emulation: the name of the emulation
+    :param ip_first_octet: the first octet of the subnet of the execution
+    :return: an OperationOutcomeDTO with the outcome of the operation
+    """
+    operation_msg = csle_cluster.cluster_manager.cluster_manager_pb2.StartSparkServersMsg(
+        emulation=emulation, ipFirstOctet=ip_first_octet
+    )
+    operation_outcome_dto = stub.startSparkServers(operation_msg, timeout=timeout)
+    return operation_outcome_dto
+
+
+def stop_spark_servers(
+        stub: csle_cluster.cluster_manager.cluster_manager_pb2_grpc.ClusterManagerStub,
+        emulation: str, ip_first_octet: int,
+        timeout=constants.GRPC.OPERATION_TIMEOUT_SECONDS) \
+        -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
+    """
+    Stops the Spark servers of a given execution
+
+    :param stub: the stub to send the remote gRPC to the server
+    :param timeout: the GRPC timeout (seconds)
+    :param emulation: the name of the emulation
+    :param ip_first_octet: the first octet of the subnet of the execution
+    :return: an OperationOutcomeDTO with the outcome of the operation
+    """
+    operation_msg = csle_cluster.cluster_manager.cluster_manager_pb2.StopSparkServersMsg(
+        emulation=emulation, ipFirstOctet=ip_first_octet
+    )
+    operation_outcome_dto = stub.stopSparkServers(operation_msg, timeout=timeout)
+    return operation_outcome_dto
+
+
+def start_spark_server(
+        stub: csle_cluster.cluster_manager.cluster_manager_pb2_grpc.ClusterManagerStub,
+        emulation: str, ip_first_octet: int, container_ip: str,
+        timeout=constants.GRPC.OPERATION_TIMEOUT_SECONDS) \
+        -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
+    """
+    Starts the Spark server on a specific container in a specific execution
+
+    :param stub: the stub to send the remote gRPC to the server
+    :param timeout: the GRPC timeout (seconds)
+    :param container_ip: the ip of the container
+    :param emulation: the name of the emulation
+    :param ip_first_octet: the first octet of the subnet of the execution
+    :return: the operation outcome
+    """
+    operation_msg = csle_cluster.cluster_manager.cluster_manager_pb2.StartSparkServerMsg(
+        ipFirstOctet=ip_first_octet, emulation=emulation, containerIp=container_ip
+    )
+    operation_outcome = stub.startSparkServer(operation_msg, timeout=timeout)
+    return operation_outcome
+
+
+def stop_spark_server(
+        stub: csle_cluster.cluster_manager.cluster_manager_pb2_grpc.ClusterManagerStub,
+        emulation: str, ip_first_octet: int, container_ip: str,
+        timeout=constants.GRPC.OPERATION_TIMEOUT_SECONDS) \
+        -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
+    """
+    Stops the Spark server on a specific container in a specific execution
+
+    :param stub: the stub to send the remote gRPC to the server
+    :param timeout: the GRPC timeout (seconds)
+    :param container_ip: the ip of the container
+    :param emulation: the name of the emulation
+    :param ip_first_octet: the first octet of the subnet of the execution
+    :return: the operation outcome
+    """
+    operation_msg = csle_cluster.cluster_manager.cluster_manager_pb2.StopSparkServerMsg(
+        ipFirstOctet=ip_first_octet, emulation=emulation, containerIp=container_ip
+    )
+    operation_outcome = stub.stopSparkServer(operation_msg, timeout=timeout)
+    return operation_outcome
+
+
+def check_pid(
+        stub: csle_cluster.cluster_manager.cluster_manager_pb2_grpc.ClusterManagerStub,
+        pid: int, timeout=constants.GRPC.OPERATION_TIMEOUT_SECONDS) \
+        -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
+    """
+    Checks the status of a PID
+
+    :param stub: the stub to send the remote gRPC to the server
+    :param timeout: the GRPC timeout (seconds)
+    :param pid: the pid to check
+    :return: the operation outcome
+    """
+    operation_msg = csle_cluster.cluster_manager.cluster_manager_pb2.CheckPidMsg(pid=pid)
+    operation_outcome = stub.checkPid(operation_msg, timeout=timeout)
+    return operation_outcome
+
+
+def stop_pid(
+        stub: csle_cluster.cluster_manager.cluster_manager_pb2_grpc.ClusterManagerStub,
+        pid: int, timeout=constants.GRPC.OPERATION_TIMEOUT_SECONDS) \
+        -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
+    """
+    Stops a PID
+
+    :param stub: the stub to send the remote gRPC to the server
+    :param timeout: the GRPC timeout (seconds)
+    :param pid: the pid to check
+    :return: the operation outcome
+    """
+    operation_msg = csle_cluster.cluster_manager.cluster_manager_pb2.StopPidMsg(pid=pid)
+    operation_outcome = stub.stopPid(operation_msg, timeout=timeout)
+    return operation_outcome
```

### Comparing `csle_cluster-0.1.9/src/csle_cluster.egg-info/PKG-INFO` & `csle_cluster-0.2.0/src/csle_cluster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-cluster
-Version: 0.1.9
+Version: 0.2.0
 Summary: Scripts for cluster management in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cluster-0.1.9/src/csle_cluster.egg-info/SOURCES.txt` & `csle_cluster-0.2.0/src/csle_cluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

