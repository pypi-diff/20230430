# Comparing `tmp/csle_common-0.1.9.tar.gz` & `tmp/csle_common-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_common-0.1.9.tar", last modified: Tue Mar 21 08:09:18 2023, max compression
+gzip compressed data, was "csle_common-0.2.0.tar", last modified: Sun Apr 30 12:36:20 2023, max compression
```

## Comparing `csle_common-0.1.9.tar` & `csle_common-0.2.0.tar`

### file list

```diff
@@ -1,288 +1,293 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:18.013213 csle_common-0.1.9/
--rw-rw-r--   0 kim       (1000) kim       (1000)      685 2023-03-21 08:09:18.013213 csle_common-0.1.9/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-02-11 20:28:41.000000 csle_common-0.1.9/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1476 2023-03-21 08:09:18.013213 csle_common-0.1.9/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2022-11-28 13:03:16.000000 csle_common-0.1.9/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.965213 csle_common-0.1.9/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.969213 csle_common-0.1.9/src/csle_common/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 csle_common-0.1.9/src/csle_common/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.969213 csle_common-0.1.9/src/csle_common/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    66639 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.969213 csle_common-0.1.9/src/csle_common/consumer_threads/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4795 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/aggregated_host_metrics_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2417 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/attacker_actions_consumer_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2807 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/avg_host_metrics_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3905 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/client_population_consumer_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2494 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/defender_actions_consumer_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2444 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/docker_host_stats_consumer_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4779 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/docker_stats_consumer_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2390 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/host_metrics_consumer_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3144 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/ossec_ids_log_consumer_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3197 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/snort_ids_log_consumer_thread.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.973213 csle_common-0.1.9/src/csle_common/controllers/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/controllers/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    37233 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/controllers/container_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    17707 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/controllers/elk_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    47786 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/controllers/emulation_env_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2255 2023-02-28 07:44:20.000000 csle_common-0.1.9/src/csle_common/controllers/flags_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    68167 2023-03-21 08:07:44.000000 csle_common-0.1.9/src/csle_common/controllers/host_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11832 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/controllers/installation_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    14738 2023-03-04 20:08:15.000000 csle_common-0.1.9/src/csle_common/controllers/kafka_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    19115 2023-02-28 07:08:18.000000 csle_common-0.1.9/src/csle_common/controllers/management_system_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    20424 2023-03-04 15:16:49.000000 csle_common-0.1.9/src/csle_common/controllers/ossec_ids_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5548 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/controllers/ovs_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3974 2023-02-28 07:45:45.000000 csle_common-0.1.9/src/csle_common/controllers/resource_constraints_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    14905 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/controllers/sdn_controller_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1214 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/controllers/simulation_env_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    20361 2023-03-04 09:58:52.000000 csle_common-0.1.9/src/csle_common/controllers/snort_ids_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11073 2023-02-28 07:45:56.000000 csle_common-0.1.9/src/csle_common/controllers/topology_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    34689 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/controllers/traffic_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3839 2023-02-28 07:42:55.000000 csle_common-0.1.9/src/csle_common/controllers/users_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2884 2023-02-28 07:44:20.000000 csle_common-0.1.9/src/csle_common/controllers/vulnerabilities_controller.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.973213 csle_common-0.1.9/src/csle_common/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/__init__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.973213 csle_common-0.1.9/src/csle_common/dao/datasets/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/datasets/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5914 2023-02-28 07:13:58.000000 csle_common-0.1.9/src/csle_common/dao/datasets/statistics_dataset.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5674 2023-02-28 07:14:17.000000 csle_common-0.1.9/src/csle_common/dao/datasets/traces_dataset.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.973213 csle_common-0.1.9/src/csle_common/dao/docker/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/docker/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6387 2023-02-28 07:15:04.000000 csle_common-0.1.9/src/csle_common/dao/docker/docker_container_metadata.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3595 2023-02-28 07:15:20.000000 csle_common-0.1.9/src/csle_common/dao/docker/docker_env_metadata.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.973213 csle_common-0.1.9/src/csle_common/dao/domain_randomization/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/domain_randomization/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2141 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/domain_randomization/node_randomizer_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      556 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/domain_randomization/randomization_space.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2900 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/domain_randomization/randomization_space_config.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.973213 csle_common-0.1.9/src/csle_common/dao/emulation_action/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/__init__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.977213 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11189 2023-03-17 07:49:22.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    19979 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2172 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_id.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      362 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_outcome.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      295 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1728 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_masscan_actions.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1517 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_network_service_actions.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1551 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nikto_actions.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    29225 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nmap_actions.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    12817 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_shell_actions.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2091 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_stopping_actions.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.977213 csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6875 2023-03-17 07:49:22.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/emulation_defender_action.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4050 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/emulation_defender_action_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      221 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/emulation_defender_action_id.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      286 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/emulation_defender_action_outcome.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      247 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/emulation_defender_action_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4705 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/emulation_defender_stopping_actions.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.981213 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      953 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nikto_scan_result.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1997 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nikto_vuln.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      192 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_addr_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1938 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_brute_credentials.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2523 2023-02-28 07:16:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_hop.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3104 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_host_result.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      199 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_host_status.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      395 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_http_enum.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      411 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_http_grep.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1174 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_os.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3715 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_port.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      199 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_port_status.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1007 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_scan_result.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2326 2023-02-28 07:16:37.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_trace.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2546 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_vuln.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      400 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_vulscan.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.993213 csle_common-0.1.9/src/csle_common/dao/emulation_config/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4068 2023-02-28 07:16:52.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/beats_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3182 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/client_managers_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8530 2023-02-28 07:42:55.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/client_population_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      299 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/client_population_process_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2576 2023-02-28 07:17:28.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/cluster_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2926 2023-02-28 07:17:43.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/cluster_node.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    37157 2023-03-06 06:25:37.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4143 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/connection_setup_dto.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4084 2023-02-28 07:18:18.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/container_network.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7691 2023-03-04 17:24:13.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/containers_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4325 2023-02-28 07:19:02.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/credential.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4829 2023-02-28 07:19:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/default_network_firewall_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5296 2023-02-28 07:19:34.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/docker_stats_manager_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3418 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/docker_stats_managers_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7236 2023-02-28 07:42:55.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/elk_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3730 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/elk_managers_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    21892 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_env_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7640 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_env_generation_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7410 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_env_state.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2392 2023-02-28 07:08:18.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_execution.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7851 2023-03-04 09:29:52.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_execution_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    15758 2023-02-28 07:20:20.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_metrics_time_series.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2768 2023-02-28 07:20:35.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_simulation_trace.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3406 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_statistics_windowed.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    42526 2022-11-28 17:19:23.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_trace.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3693 2023-02-28 07:21:01.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/flag.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3446 2023-02-28 07:21:17.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/flags_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4658 2023-02-28 07:21:32.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/host_manager_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3103 2022-12-01 06:44:23.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/host_managers_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7618 2023-03-17 07:49:22.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/kafka_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3108 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/kafka_managers_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3550 2023-02-28 07:21:58.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/kafka_topic.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5079 2023-02-28 07:22:17.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/network_service.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6950 2023-02-28 07:22:32.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_beats_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7334 2023-02-28 07:42:55.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_container_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8429 2023-02-28 07:44:20.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_firewall_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3630 2023-02-28 07:44:20.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_flags_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    15661 2023-02-28 07:24:01.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_network_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5446 2023-02-28 07:41:48.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_resources_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3052 2023-02-28 07:24:34.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_services_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5232 2023-02-28 07:42:55.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_traffic_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3633 2023-02-28 07:42:55.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_users_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5560 2023-02-28 07:45:02.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_vulnerability_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5008 2023-02-28 07:25:33.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/ossec_ids_manager_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3328 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/ossec_managers_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3057 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/ovs_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5399 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/ovs_switch_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      316 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/packet_delay_distribution_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      269 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/packet_loss_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3214 2023-02-28 07:26:29.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/resources_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3888 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/ryu_managers_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7312 2023-02-28 07:44:20.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/sdn_controller_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      205 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/sdn_controller_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3562 2023-02-28 07:27:00.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/services_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4910 2023-02-28 07:27:15.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/snort_ids_manager_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3618 2023-03-17 07:49:22.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/snort_managers_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      254 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/static_emulation_attacker_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3503 2023-02-28 07:27:24.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/topology_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4287 2023-03-03 06:17:37.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/traffic_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3216 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/traffic_managers_info.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      782 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/transport_protocol.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2435 2023-02-28 07:27:57.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/user.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3431 2023-02-28 07:28:10.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/users_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3787 2023-02-28 07:28:25.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/vulnerabilities_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      302 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/vulnerability_type.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.993213 csle_common-0.1.9/src/csle_common/dao/emulation_observation/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/__init__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.993213 csle_common-0.1.9/src/csle_common/dao/emulation_observation/attacker/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/attacker/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    20554 2023-02-28 07:28:42.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_machine_observation_state.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10470 2023-02-28 07:12:35.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_observation_state.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.993213 csle_common-0.1.9/src/csle_common/dao/emulation_observation/common/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/common/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6143 2023-02-28 07:09:18.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/common/emulation_connection_observation_state.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6055 2023-02-28 07:10:13.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/common/emulation_port_observation_state.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6278 2023-02-28 07:09:55.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/common/emulation_vulnerability_observation_state.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.993213 csle_common-0.1.9/src/csle_common/dao/emulation_observation/defender/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/defender/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8885 2023-02-28 07:14:44.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/defender/emulation_defender_machine_observation_state.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    19601 2023-02-28 07:29:48.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/defender/emulation_defender_observation_state.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.997213 csle_common-0.1.9/src/csle_common/dao/encoding/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/encoding/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      411 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/encoding/np_encoder.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.997213 csle_common-0.1.9/src/csle_common/dao/jobs/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/jobs/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7084 2023-02-28 07:30:15.000000 csle_common-0.1.9/src/csle_common/dao/jobs/data_collection_job_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4534 2023-02-28 07:30:39.000000 csle_common-0.1.9/src/csle_common/dao/jobs/system_identification_job_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5495 2023-02-28 07:30:52.000000 csle_common-0.1.9/src/csle_common/dao/jobs/training_job_config.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.997213 csle_common-0.1.9/src/csle_common/dao/management/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/management/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3542 2023-02-28 07:31:05.000000 csle_common-0.1.9/src/csle_common/dao/management/management_user.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2775 2023-02-28 07:31:19.000000 csle_common-0.1.9/src/csle_common/dao/management/session_token.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:18.001213 csle_common-0.1.9/src/csle_common/dao/simulation_config/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1073 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/action.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2022 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/action_space_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      483 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/agent_log.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      734 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/base_env.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1228 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/env_parameter.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1216 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/env_parameters_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1312 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/initial_state_distribution_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1302 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/joint_action_space_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1163 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/joint_observation_space_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1242 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/observation.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1505 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/observation_function_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5039 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/observation_space_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1226 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/player_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1271 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/players_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1047 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/reward_function_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11210 2023-03-07 11:00:13.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/simulation_env_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      337 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/simulation_env_input_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5489 2023-03-03 06:17:37.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/simulation_trace.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1451 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/state.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1274 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/state_space_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      157 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/state_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      166 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/time_step_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1121 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/transition_operator_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      159 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/value_type.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:18.001213 csle_common-0.1.9/src/csle_common/dao/system_identification/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2998 2023-02-28 07:31:32.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/empirical_conditional.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6116 2023-02-28 07:31:49.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/empirical_system_model.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    23200 2023-02-28 07:08:10.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/emulation_statistics.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7292 2023-02-28 07:32:31.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/gaussian_mixture_conditional.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6623 2023-02-28 07:32:47.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/gaussian_mixture_system_model.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5215 2023-02-28 07:34:58.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/gp_conditional.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6461 2023-02-28 07:35:13.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/gp_system_model.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3260 2023-02-28 07:35:27.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/system_identification_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      768 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/system_model.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      219 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/system_model_type.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:18.005213 csle_common-0.1.9/src/csle_common/dao/training/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/training/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      633 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/training/agent_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6605 2023-02-28 07:35:45.000000 csle_common-0.1.9/src/csle_common/dao/training/alpha_vectors_policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7357 2023-02-28 07:35:58.000000 csle_common-0.1.9/src/csle_common/dao/training/dqn_policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4362 2023-02-28 07:36:11.000000 csle_common-0.1.9/src/csle_common/dao/training/experiment_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3648 2023-02-28 07:36:25.000000 csle_common-0.1.9/src/csle_common/dao/training/experiment_execution.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3222 2023-02-28 07:36:36.000000 csle_common-0.1.9/src/csle_common/dao/training/experiment_result.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11482 2023-02-28 07:36:57.000000 csle_common-0.1.9/src/csle_common/dao/training/fnn_with_softmax_policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1959 2023-02-28 07:37:16.000000 csle_common-0.1.9/src/csle_common/dao/training/hparam.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    14043 2023-02-28 07:37:33.000000 csle_common-0.1.9/src/csle_common/dao/training/mixed_multi_threshold_stopping_policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    13851 2023-02-28 07:37:45.000000 csle_common-0.1.9/src/csle_common/dao/training/multi_threshold_stopping_policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      179 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/training/player_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      963 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/training/policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7424 2023-02-28 07:38:05.000000 csle_common-0.1.9/src/csle_common/dao/training/ppo_policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4560 2023-02-28 07:38:20.000000 csle_common-0.1.9/src/csle_common/dao/training/random_policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5276 2023-02-28 07:38:35.000000 csle_common-0.1.9/src/csle_common/dao/training/tabular_policy.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4634 2023-02-28 07:38:49.000000 csle_common-0.1.9/src/csle_common/dao/training/vector_policy.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:18.005213 csle_common-0.1.9/src/csle_common/logging/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/logging/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      624 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/logging/custom_formatter.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2646 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/logging/log.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:18.005213 csle_common-0.1.9/src/csle_common/metastore/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/metastore/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   219637 2023-02-28 07:42:55.000000 csle_common-0.1.9/src/csle_common/metastore/metastore_facade.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:18.009213 csle_common-0.1.9/src/csle_common/models/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-12-11 08:33:52.000000 csle_common-0.1.9/src/csle_common/models/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4091 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/models/fnn_w_softmax.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:18.009213 csle_common-0.1.9/src/csle_common/tunneling/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/tunneling/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2325 2022-12-03 10:35:18.000000 csle_common-0.1.9/src/csle_common/tunneling/forward_ssh_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      280 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/tunneling/forward_ssh_server.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1620 2022-12-03 09:27:05.000000 csle_common-0.1.9/src/csle_common/tunneling/forward_tunnel_thread.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:18.013213 csle_common-0.1.9/src/csle_common/util/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/util/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6225 2023-02-28 07:08:18.000000 csle_common-0.1.9/src/csle_common/util/cluster_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    35781 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/util/connection_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8718 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/util/docker_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    21262 2023-03-03 12:17:05.000000 csle_common-0.1.9/src/csle_common/util/emulation_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    37527 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/util/env_dynamics_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    16211 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/util/experiment_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    19037 2022-11-28 17:13:00.000000 csle_common-0.1.9/src/csle_common/util/export_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      809 2023-02-11 17:47:01.000000 csle_common-0.1.9/src/csle_common/util/general_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      533 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/util/grpc_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2514 2022-12-24 11:45:22.000000 csle_common-0.1.9/src/csle_common/util/import_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3542 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/util/management_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2165 2023-03-17 07:49:22.000000 csle_common-0.1.9/src/csle_common/util/plotting_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    17318 2023-03-17 07:49:22.000000 csle_common-0.1.9/src/csle_common/util/read_emulation_statistics_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2512 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/util/ssh_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.969213 csle_common-0.1.9/src/csle_common.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      685 2023-03-21 08:09:17.000000 csle_common-0.1.9/src/csle_common.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)    14558 2023-03-21 08:09:17.000000 csle_common-0.1.9/src/csle_common.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:09:17.000000 csle_common-0.1.9/src/csle_common.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:28:51.000000 csle_common-0.1.9/src/csle_common.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      399 2023-03-21 08:09:17.000000 csle_common-0.1.9/src/csle_common.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       12 2023-03-21 08:09:17.000000 csle_common-0.1.9/src/csle_common.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.864460 csle_common-0.2.0/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      685 2023-04-30 12:36:20.864460 csle_common-0.2.0/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-03-28 14:03:22.000000 csle_common-0.2.0/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1483 2023-04-30 12:36:20.864460 csle_common-0.2.0/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_common-0.2.0/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.804460 csle_common-0.2.0/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.808460 csle_common-0.2.0/src/csle_common/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-04-30 12:35:57.000000 csle_common-0.2.0/src/csle_common/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.808460 csle_common-0.2.0/src/csle_common/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    67243 2023-04-30 06:59:23.000000 csle_common-0.2.0/src/csle_common/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.812460 csle_common-0.2.0/src/csle_common/consumer_threads/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4795 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/aggregated_host_metrics_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3154 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/aggregated_ossec_ids_log_consumer_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3207 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/aggregated_snort_ids_log_consumer_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3202 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/aggregated_snort_ids_rule_log_consumer_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2417 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/attacker_actions_consumer_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2807 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/avg_host_metrics_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3905 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/client_population_consumer_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2494 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/defender_actions_consumer_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2444 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/docker_host_stats_consumer_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4779 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/docker_stats_consumer_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2390 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/host_metrics_consumer_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2564 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/ossec_ids_log_consumer_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2493 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/consumer_threads/snort_ids_log_consumer_thread.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.816460 csle_common-0.2.0/src/csle_common/controllers/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    37512 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/container_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17707 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/elk_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    48222 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/emulation_env_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2255 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/flags_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    71893 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/host_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11832 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/installation_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14738 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/kafka_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    23308 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/management_system_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    20424 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/ossec_ids_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5548 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/ovs_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3974 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/resource_constraints_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15201 2023-04-18 12:48:17.000000 csle_common-0.2.0/src/csle_common/controllers/sdn_controller_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1214 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/simulation_env_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    21969 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/snort_ids_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11243 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/topology_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    37012 2023-04-18 12:48:40.000000 csle_common-0.2.0/src/csle_common/controllers/traffic_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3839 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/users_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2884 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/controllers/vulnerabilities_controller.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.816460 csle_common-0.2.0/src/csle_common/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/__init__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.816460 csle_common-0.2.0/src/csle_common/dao/datasets/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/datasets/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5914 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/datasets/statistics_dataset.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5674 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/datasets/traces_dataset.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.816460 csle_common-0.2.0/src/csle_common/dao/docker/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/docker/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6387 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/docker/docker_container_metadata.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3595 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/docker/docker_env_metadata.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.820460 csle_common-0.2.0/src/csle_common/dao/domain_randomization/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/domain_randomization/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2141 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/domain_randomization/node_randomizer_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      556 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/domain_randomization/randomization_space.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2900 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/domain_randomization/randomization_space_config.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.820460 csle_common-0.2.0/src/csle_common/dao/emulation_action/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/__init__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.820460 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11189 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    19992 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2172 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_id.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      362 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_outcome.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      295 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1728 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_masscan_actions.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1517 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_network_service_actions.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1551 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nikto_actions.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    29225 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nmap_actions.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12817 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_shell_actions.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2091 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_stopping_actions.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.824460 csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6875 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/emulation_defender_action.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4063 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/emulation_defender_action_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      221 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/emulation_defender_action_id.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      286 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/emulation_defender_action_outcome.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      247 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/emulation_defender_action_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4705 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/emulation_defender_stopping_actions.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.828460 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      953 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nikto_scan_result.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1997 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nikto_vuln.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      192 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_addr_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1938 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_brute_credentials.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2523 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_hop.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3104 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_host_result.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      199 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_host_status.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      395 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_http_enum.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      411 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_http_grep.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1174 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_os.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3715 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_port.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      199 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_port_status.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1007 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_scan_result.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2326 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_trace.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2546 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_vuln.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      400 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_vulscan.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.840460 csle_common-0.2.0/src/csle_common/dao/emulation_config/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4068 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/beats_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3182 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/client_managers_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9637 2023-04-01 08:34:56.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/client_population_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      343 2023-04-01 08:34:56.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/client_population_process_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2576 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/cluster_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2926 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/cluster_node.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    37157 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4143 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/connection_setup_dto.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4084 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/container_network.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7691 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/containers_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4325 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/credential.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4829 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/default_network_firewall_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5296 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/docker_stats_manager_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3418 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/docker_stats_managers_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7236 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/elk_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3728 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/elk_managers_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    21925 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_env_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7640 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_env_generation_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7486 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_env_state.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2392 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_execution.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7851 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_execution_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18879 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_metrics_time_series.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2768 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_simulation_trace.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3406 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_statistics_windowed.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    42526 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_trace.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3693 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/flag.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3446 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/flags_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4658 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/host_manager_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3103 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/host_managers_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7618 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/kafka_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3108 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/kafka_managers_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3550 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/kafka_topic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5079 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/network_service.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6950 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_beats_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7334 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_container_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8495 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_firewall_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3630 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_flags_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15661 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_network_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5446 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_resources_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3052 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_services_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5232 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_traffic_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3633 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_users_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5560 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/node_vulnerability_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5008 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/ossec_ids_manager_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3328 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/ossec_managers_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3016 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/ovs_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5399 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/ovs_switch_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      316 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/packet_delay_distribution_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      269 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/packet_loss_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3214 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/resources_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3888 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/ryu_managers_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7312 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/sdn_controller_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      205 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/sdn_controller_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3562 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/services_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4910 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/snort_ids_manager_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3618 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/snort_managers_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      254 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/static_emulation_attacker_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3503 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/topology_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4287 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/traffic_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3216 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/traffic_managers_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      782 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/transport_protocol.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2435 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/user.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3431 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/users_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3787 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/vulnerabilities_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      302 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_config/vulnerability_type.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.840460 csle_common-0.2.0/src/csle_common/dao/emulation_observation/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/__init__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.844460 csle_common-0.2.0/src/csle_common/dao/emulation_observation/attacker/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/attacker/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    20660 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_machine_observation_state.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10470 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_observation_state.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.844460 csle_common-0.2.0/src/csle_common/dao/emulation_observation/common/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/common/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6143 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/common/emulation_connection_observation_state.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6055 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/common/emulation_port_observation_state.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6278 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/common/emulation_vulnerability_observation_state.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.844460 csle_common-0.2.0/src/csle_common/dao/emulation_observation/defender/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/defender/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12266 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/defender/emulation_defender_machine_observation_state.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    22453 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/emulation_observation/defender/emulation_defender_observation_state.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.844460 csle_common-0.2.0/src/csle_common/dao/encoding/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/encoding/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      411 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/encoding/np_encoder.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.844460 csle_common-0.2.0/src/csle_common/dao/jobs/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/jobs/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7391 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/jobs/data_collection_job_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4781 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/jobs/system_identification_job_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5823 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/jobs/training_job_config.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.844460 csle_common-0.2.0/src/csle_common/dao/management/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/management/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3542 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/management/management_user.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2775 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/management/session_token.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.852460 csle_common-0.2.0/src/csle_common/dao/simulation_config/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1073 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/action.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2022 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/action_space_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      483 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/agent_log.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      747 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/base_env.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1228 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/env_parameter.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1216 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/env_parameters_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1312 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/initial_state_distribution_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1302 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/joint_action_space_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1163 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/joint_observation_space_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1242 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/observation.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1505 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/observation_function_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5039 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/observation_space_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1226 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/player_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1271 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/players_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1047 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/reward_function_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11210 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/simulation_env_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      337 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/simulation_env_input_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5489 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/simulation_trace.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1451 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/state.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1274 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/state_space_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      157 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/state_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      166 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/time_step_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1121 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/transition_operator_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      159 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/simulation_config/value_type.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.852460 csle_common-0.2.0/src/csle_common/dao/system_identification/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2998 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/empirical_conditional.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6116 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/empirical_system_model.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    29651 2023-04-18 12:47:23.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/emulation_statistics.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7292 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/gaussian_mixture_conditional.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6623 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/gaussian_mixture_system_model.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5215 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/gp_conditional.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6461 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/gp_system_model.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3260 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/system_identification_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      768 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/system_model.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      219 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/system_identification/system_model_type.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.860460 csle_common-0.2.0/src/csle_common/dao/training/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/training/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      633 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/training/agent_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6794 2023-04-23 07:07:00.000000 csle_common-0.2.0/src/csle_common/dao/training/alpha_vectors_policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7536 2023-04-23 07:07:00.000000 csle_common-0.2.0/src/csle_common/dao/training/dqn_policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4362 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/training/experiment_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3648 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/training/experiment_execution.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3222 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/training/experiment_result.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11703 2023-04-23 07:07:00.000000 csle_common-0.2.0/src/csle_common/dao/training/fnn_with_softmax_policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1959 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/training/hparam.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7245 2023-04-30 06:59:23.000000 csle_common-0.2.0/src/csle_common/dao/training/linear_threshold_stopping_policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14240 2023-04-23 07:07:00.000000 csle_common-0.2.0/src/csle_common/dao/training/mixed_multi_threshold_stopping_policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14042 2023-04-23 07:07:00.000000 csle_common-0.2.0/src/csle_common/dao/training/multi_threshold_stopping_policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      179 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/training/player_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      963 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/dao/training/policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      320 2023-04-23 07:07:00.000000 csle_common-0.2.0/src/csle_common/dao/training/policy_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7603 2023-04-23 07:07:00.000000 csle_common-0.2.0/src/csle_common/dao/training/ppo_policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4763 2023-04-23 07:07:00.000000 csle_common-0.2.0/src/csle_common/dao/training/random_policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5459 2023-04-23 07:07:00.000000 csle_common-0.2.0/src/csle_common/dao/training/tabular_policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4809 2023-04-30 06:59:23.000000 csle_common-0.2.0/src/csle_common/dao/training/vector_policy.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.860460 csle_common-0.2.0/src/csle_common/logging/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/logging/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      624 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/logging/custom_formatter.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2646 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/logging/log.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.860460 csle_common-0.2.0/src/csle_common/metastore/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/metastore/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   228115 2023-04-30 06:59:23.000000 csle_common-0.2.0/src/csle_common/metastore/metastore_facade.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.860460 csle_common-0.2.0/src/csle_common/models/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/models/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4091 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/models/fnn_w_softmax.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.860460 csle_common-0.2.0/src/csle_common/tunneling/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/tunneling/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2325 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/tunneling/forward_ssh_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      280 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/tunneling/forward_ssh_server.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1620 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/tunneling/forward_tunnel_thread.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.864460 csle_common-0.2.0/src/csle_common/util/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6225 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/cluster_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    35781 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/connection_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8718 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/docker_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    21328 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/emulation_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    37779 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/env_dynamics_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    16211 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/experiment_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    19188 2023-04-18 12:45:40.000000 csle_common-0.2.0/src/csle_common/util/export_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2000 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/general_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      533 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/grpc_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2514 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/import_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3542 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/management_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2165 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/plotting_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    22141 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/read_emulation_statistics_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2512 2023-03-28 14:03:22.000000 csle_common-0.2.0/src/csle_common/util/ssh_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:20.808460 csle_common-0.2.0/src/csle_common.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      685 2023-04-30 12:36:20.000000 csle_common-0.2.0/src/csle_common.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14903 2023-04-30 12:36:20.000000 csle_common-0.2.0/src/csle_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-04-30 12:36:20.000000 csle_common-0.2.0/src/csle_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:28:51.000000 csle_common-0.2.0/src/csle_common.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      406 2023-04-30 12:36:20.000000 csle_common-0.2.0/src/csle_common.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       12 2023-04-30 12:36:20.000000 csle_common-0.2.0/src/csle_common.egg-info/top_level.txt
```

### Comparing `csle_common-0.1.9/PKG-INFO` & `csle_common-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_common
-Version: 0.1.9
+Version: 0.2.0
 Summary: Common functionality of the Cyber Security Learning Environment (CSLE)
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_common-0.1.9/pyproject.toml` & `csle_common-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/setup.cfg` & `csle_common-0.2.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	gym>=0.21
+	gymnasium>=0.27.1
 	pyglet>=2.0.0
 	numpy>=1.23.5
 	torch>=1.13.0
 	docker>=6.0.1
 	paramiko>=2.12.0
-	stable_baselines3>=0.14.4
+	stable_baselines3>=1.8.0
 	random_username>=1.0.2
-	psycopg>=3.1.4
+	psycopg==3.1.4
 	click>=8.1.3
 	flask>=2.2.2
 	waitress>=2.1.2
 	psutil>=5.9.4
 	csle_collector>=0.1.5
-	csle-ryu>=0.1.9
+	csle-ryu>=0.2.0
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_common-0.1.9/src/csle_common/constants/constants.py` & `csle_common-0.2.0/src/csle_common/constants/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,22 +71,23 @@
     TELNET_2 = "csle_telnet_2"
     TELNET_3 = "csle_telnet_3"
     FTP_2 = "csle_ftp_2"
     OVS_1 = "csle_ovs_1"
     RYU_1 = "csle_ryu_1"
     PENGINE_EXPLOIT_1 = "csle_pengine_exploit_1"
     CVE_2014_0160_1 = "csle_cve_2014_0160_1"
-    SNORT_IDS_IMAGES = ["csle_router_2"]
-    OVS_IMAGES = ["csle_ovs_1"]
-    OSSEC_IDS_IMAGES = ["csle_honeypot_1", "csle_honeypot_2", "csle_pengine_exploit_1", "csle_router_1",
-                        "csle_router_2", "csle_ssh_1", "csle_ssh_2",
-                        "csle_ssh_3", "csle_telnet_1", "csle_telnet_2", "csle_telnet_3"]
-    ROUTER_IMAGES = ["csle_router_1", "csle_router_2"]
-    HACKER_IMAGES = ["csle_hacker_kali_1"]
-    CLIENT_IMAGES = ["csle_client_1"]
+    SPARK_1 = "csle_spark_1"
+    SNORT_IDS_IMAGES = [ROUTER_2]
+    OVS_IMAGES = [OVS_1]
+    SPARK_IMAGES = [SPARK_1]
+    OSSEC_IDS_IMAGES = [HONEYPOT_1, HONEYPOT_2, PENGINE_EXPLOIT_1, ROUTER_1,
+                        ROUTER_2, SSH_1, SSH_2, SSH_3, TELNET_1, TELNET_2, TELNET_3, SPARK_1]
+    ROUTER_IMAGES = [ROUTER_1, ROUTER_2]
+    HACKER_IMAGES = [HACKER_KALI_1]
+    CLIENT_IMAGES = [CLIENT_1]
     CADVISOR = "cadvisor"
     PGADMIN = "pgadmin"
     GRAFANA = "grafana"
 
 
 class CONTAINER_OS:
     """
@@ -117,14 +118,15 @@
     SSH_2_OS = "ubuntu"
     SSH_3_OS = "ubuntu"
     TELNET_2_OS = "ubuntu"
     TELNET_3_OS = "ubuntu"
     FTP_2_OS = "ubuntu"
     PENGINE_EXPLOIT_1_OS = "ubuntu"
     CVE_2014_0160_1_OS = "debian"
+    SPARK_1_OS = "spark"
 
 
 class RENDERING:
     """
     Rendering constants
     """
     RECT_SIZE = 200
@@ -521,15 +523,15 @@
 class SSH:
     """
     Constants related to the SSH service
     """
     SERVICE_NAME = "ssh"
     DEFAULT_PORT = 22
     DIRECT_CHANNEL = "direct-tcpip"
-    MAX_FILE_READ_BYTES = 500000000
+    MAX_FILE_READ_BYTES = 50000
 
 
 class TELNET:
     """
     Constants related to the Telnet service
     """
     PROMPT = b':~$'
@@ -648,19 +650,29 @@
     """
     SERVICE_NAME = "snmp"
     DEFAULT_PORT = 161
 
 
 class HTTP:
     """
-    Constants related to the DNS service
+    Constants related to the HTTP service
     """
     SERVICE_NAME = "http"
     DEFAULT_PORT = 80
     HTTP_PROTOCOL_PREFIX = "http://"
+    DEFAULT_TIMEOUT = 5
+
+
+class SPARK:
+    """
+    Constants related to the spark service
+    """
+    SERVICE_NAME = "spark"
+    DEFAULT_PORT = 7077
+    SPARK_PROTOCOL_PREFIX = "spark://"
 
 
 class DNS:
     """
     Constants related to the DNS service
     """
     SERVICE_NAME = "dns"
@@ -1237,14 +1249,20 @@
             "\"src_text\": \"problem(1, [[_,_,_,_,_,_,_,_,_],[_,_,_,_,_,3,_,8,5],[_,_,1,_,2,_,_,_,_],"
             "[_,_,_,5,_,7,_,_,_],[_,_,4,_,_,_,1,_,_],[_,9,_,_,_,_,_,_,_],[5,_,_,_,_,_,_,7,3],"
             "[_,_,2,_,1,_,_,_,_],[_,_,_,_,4,_,_,_,9]]).\n\"}}' {}"
         ],
         f"{CONTAINER_IMAGES.CVE_2014_0160_1}": [
             "timeout 5 sshpass -p 'testcsleuser' ssh -oStrictHostKeyChecking=no {} > /dev/null 2>&1",
             "timeout 5 curl {}:443 > /dev/null 2>&1"],
+        f"{CONTAINER_IMAGES.SPARK_1}": [
+            "timeout 5 sshpass -p 'testcsleuser' ssh -oStrictHostKeyChecking=no {} > /dev/null 2>&1",
+            "timeout 5 curl {}:8080 > /dev/null 2>&1",
+            "timeout 5 curl {}:8081 > /dev/null 2>&1",
+            "/root/miniconda3/bin/python3 /spark_job.py --sparkmaster {} > /dev/null 2>&1"
+        ]
     }
 
 
 class AGENT:
     USER = "agent"
     PW = "agent"
 
@@ -1576,14 +1594,15 @@
     SIMULATION_IMAGES_TABLE = "simulation_images"
     EMULATION_SIMULATION_TRACES_TABLE = "emulation_simulation_traces"
     EXPERIMENT_EXECUTIONS_TABLE = "experiment_executions"
     TRAINING_JOBS_TABLE = "training_jobs"
     SYSTEM_IDENTIFICATION_JOBS_TABLE = "system_identification_jobs"
     DATA_COLLECTION_JOBS_TABLE = "data_collection_jobs"
     MULTI_THRESHOLD_STOPPING_POLICIES_TABLE = "multi_threshold_stopping_policies"
+    LINEAR_THRESHOLD_STOPPING_POLICIES_TABLE = "linear_threshold_stopping_policies"
     PPO_POLICIES_TABLE = "ppo_policies"
     GAUSSIAN_MIXTURE_SYSTEM_MODELS_TABLE = "gaussian_mixture_system_models"
     TABULAR_POLICIES_TABLE = "tabular_policies"
     ALPHA_VEC_POLICIES_TABLE = "alpha_vec_policies"
     DQN_POLICIES_TABLE = "dqn_policies"
     FNN_W_SOFTMAX_POLICIES_TABLE = "fnn_w_softmax_policies"
     VECTOR_POLICIES_TABLE = "vector_policies"
@@ -1748,14 +1767,15 @@
 class T_SPSA:
     """
     String constants related to T-SPSA
     """
     a = "a"
     c = "c"
     LAMBDA = "lambda"
+    POLICY_TYPE = "policy_type"
     A = "A"
     EPSILON = "epsilon"
     N = "N"
     L = "L"
     THETA1 = "theta1"
     THETAS = "thetas"
     THRESHOLDS = "thresholds"
```

### Comparing `csle_common-0.1.9/src/csle_common/consumer_threads/aggregated_host_metrics_thread.py` & `csle_common-0.2.0/src/csle_common/consumer_threads/aggregated_host_metrics_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/consumer_threads/attacker_actions_consumer_thread.py` & `csle_common-0.2.0/src/csle_common/consumer_threads/attacker_actions_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/consumer_threads/avg_host_metrics_thread.py` & `csle_common-0.2.0/src/csle_common/consumer_threads/avg_host_metrics_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/consumer_threads/client_population_consumer_thread.py` & `csle_common-0.2.0/src/csle_common/consumer_threads/client_population_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/consumer_threads/defender_actions_consumer_thread.py` & `csle_common-0.2.0/src/csle_common/consumer_threads/defender_actions_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/consumer_threads/docker_host_stats_consumer_thread.py` & `csle_common-0.2.0/src/csle_common/consumer_threads/docker_host_stats_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/consumer_threads/docker_stats_consumer_thread.py` & `csle_common-0.2.0/src/csle_common/consumer_threads/docker_stats_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/consumer_threads/host_metrics_consumer_thread.py` & `csle_common-0.2.0/src/csle_common/consumer_threads/host_metrics_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/consumer_threads/ossec_ids_log_consumer_thread.py` & `csle_common-0.2.0/src/csle_common/consumer_threads/aggregated_ossec_ids_log_consumer_thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 from confluent_kafka import Consumer, KafkaError, KafkaException
 import csle_collector.constants.constants as collector_constants
 from csle_collector.ossec_ids_manager.ossec_ids_alert_counters import OSSECIdsAlertCounters
 from csle_common.logging.log import Logger
 
 
-class OSSECIdsLogConsumerThread(threading.Thread):
+class AggregatedOSSECIdsLogConsumerThread(threading.Thread):
     """
     Thread that polls the OSSEC IDS log to get the latest metrics
     """
 
     def __init__(self, kafka_server_ip: str, kafka_port: int, ossec_ids_alert_counters: OSSECIdsAlertCounters,
                  auto_offset_reset: str = "latest") -> None:
         """
```

### Comparing `csle_common-0.1.9/src/csle_common/consumer_threads/snort_ids_log_consumer_thread.py` & `csle_common-0.2.0/src/csle_common/consumer_threads/aggregated_snort_ids_log_consumer_thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 from confluent_kafka import Consumer, KafkaError, KafkaException
 import csle_collector.constants.constants as collector_constants
 from csle_collector.snort_ids_manager.snort_ids_alert_counters import SnortIdsAlertCounters
 from csle_common.logging.log import Logger
 
 
-class SnortIdsLogConsumerThread(threading.Thread):
+class AggregatedSnortIdsLogConsumerThread(threading.Thread):
     """
     Thread that polls the Snort IDS log to get the latest metrics
     """
 
     def __init__(self, kafka_server_ip: str, kafka_port: int, snort_ids_alert_counters: SnortIdsAlertCounters,
                  auto_offset_reset: str = "latest") -> None:
         """
```

### Comparing `csle_common-0.1.9/src/csle_common/controllers/container_controller.py` & `csle_common-0.2.0/src/csle_common/controllers/container_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,16 +361,18 @@
         :return: None
         """
         for c in containers_config.containers:
             for ip_net in c.ips_and_networks:
                 existing_networks = ContainerController.get_network_references()
                 existing_networks = list(map(lambda x: x.name, existing_networks))
                 ip, net = ip_net
-                ContainerController.create_network_from_dto(network_dto=net, existing_network_names=existing_networks,
-                                                            logger=logger)
+                if net.name != "":
+                    ContainerController.create_network_from_dto(network_dto=net,
+                                                                existing_network_names=existing_networks,
+                                                                logger=logger)
 
     @staticmethod
     def connect_containers_to_networks(emulation_env_config: EmulationEnvConfig, physical_server_ip: str,
                                        logger: logging.Logger) -> None:
         """
         Connects running containers to networks
 
@@ -463,14 +465,15 @@
         :param execution: the emulation execution
         :param physical_server_ip: the ip of the physical server
         :param logger: the logger to use for logging
         :return: None
         """
         if not ManagementSystemController.is_statsmanager_running():
             ManagementSystemController.start_docker_stats_manager(
+                logger=logger,
                 port=execution.emulation_env_config.docker_stats_manager_config.docker_stats_manager_port,
                 log_dir=execution.emulation_env_config.docker_stats_manager_config.docker_stats_manager_log_dir,
                 log_file=execution.emulation_env_config.docker_stats_manager_config.docker_stats_manager_log_file,
                 max_workers=execution.emulation_env_config.docker_stats_manager_config.docker_stats_manager_max_workers
             )
             time.sleep(5)
         ip = physical_server_ip
@@ -495,24 +498,27 @@
                 kafka_ip=execution.emulation_env_config.kafka_config.container.docker_gw_bridge_ip,
                 stats_queue_maxsize=1000,
                 time_step_len_seconds=execution.emulation_env_config.docker_stats_manager_config.time_step_len_seconds,
                 kafka_port=execution.emulation_env_config.kafka_config.kafka_port_external,
                 containers=container_ip_dtos, execution_first_ip_octet=execution.ip_first_octet)
 
     @staticmethod
-    def stop_docker_stats_thread(execution: EmulationExecution, physical_server_ip: str) -> None:
+    def stop_docker_stats_thread(execution: EmulationExecution, physical_server_ip: str,
+                                 logger: logging.Logger) -> None:
         """
         Sends a request to the docker stats manager on the docker host for stopping a docker stats monitor thread
 
+        :param logger: the logger to use for logging
         :param execution: the execution of the emulation for which the monitor should be stopped
         :param physical_server_ip: the ip of the physical server
         :return: None
         """
         if not ManagementSystemController.is_statsmanager_running():
             ManagementSystemController.start_docker_stats_manager(
+                logger=logger,
                 port=execution.emulation_env_config.docker_stats_manager_config.docker_stats_manager_port,
                 log_file=execution.emulation_env_config.docker_stats_manager_config.docker_stats_manager_log_file,
                 log_dir=execution.emulation_env_config.docker_stats_manager_config.docker_stats_manager_log_dir,
                 max_workers=execution.emulation_env_config.docker_stats_manager_config.docker_stats_manager_max_workers
             )
             time.sleep(5)
         ip = physical_server_ip
```

### Comparing `csle_common-0.1.9/src/csle_common/controllers/elk_controller.py` & `csle_common-0.2.0/src/csle_common/controllers/elk_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/controllers/emulation_env_controller.py` & `csle_common-0.2.0/src/csle_common/controllers/emulation_env_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,16 @@
         :return: None
         """
         executions = MetastoreFacade.list_emulation_executions_for_a_given_emulation(
             emulation_name=emulation_env_config.name)
         for exec in executions:
             EmulationEnvController.stop_containers(execution=exec, physical_server_ip=physical_server_ip,
                                                    logger=logger)
-            ContainerController.stop_docker_stats_thread(execution=exec, physical_server_ip=physical_server_ip)
+            ContainerController.stop_docker_stats_thread(execution=exec, physical_server_ip=physical_server_ip,
+                                                         logger=logger)
 
     @staticmethod
     def stop_execution_of_emulation(emulation_env_config: EmulationEnvConfig, execution_id: int,
                                     physical_server_ip: str, logger: logging.Logger) -> None:
         """
         Stops an execution of a given emulation
 
@@ -63,30 +64,32 @@
         :param logger: the logger to use for logging
         :return: None
         """
         execution = MetastoreFacade.get_emulation_execution(emulation_name=emulation_env_config.name,
                                                             ip_first_octet=execution_id)
         EmulationEnvController.stop_containers(execution=execution, physical_server_ip=physical_server_ip,
                                                logger=logger)
-        ContainerController.stop_docker_stats_thread(execution=execution, physical_server_ip=physical_server_ip)
+        ContainerController.stop_docker_stats_thread(execution=execution, physical_server_ip=physical_server_ip,
+                                                     logger=logger)
 
     @staticmethod
     def stop_all_executions(physical_server_ip: str, logger: logging.Logger) -> None:
         """
         Stops all emulation executions
 
         :param physical_server_ip: ip of the physical server
         :param logger: the logger to use for logging
         :return: None
         """
         executions = MetastoreFacade.list_emulation_executions()
         for exec in executions:
             EmulationEnvController.stop_containers(execution=exec, physical_server_ip=physical_server_ip,
                                                    logger=logger)
-            ContainerController.stop_docker_stats_thread(execution=exec, physical_server_ip=physical_server_ip)
+            ContainerController.stop_docker_stats_thread(execution=exec, physical_server_ip=physical_server_ip,
+                                                         logger=logger)
 
     @staticmethod
     def install_csle_collector_and_ryu_libraries(emulation_env_config: EmulationEnvConfig, physical_server_ip: str,
                                                  logger: logging.Logger) \
             -> None:
         """
         Installs the latest csle-collector and csle-ryu libraries on all nodes of a given emulation
@@ -542,15 +545,16 @@
         executions = MetastoreFacade.list_emulation_executions_for_a_given_emulation(
             emulation_name=emulation_env_config.name)
         for exec in executions:
             EmulationEnvController.stop_containers(execution=exec, physical_server_ip=physical_server_ip,
                                                    logger=logger)
             EmulationEnvController.rm_containers(execution=exec, physical_server_ip=physical_server_ip, logger=logger)
             try:
-                ContainerController.stop_docker_stats_thread(execution=exec, physical_server_ip=physical_server_ip)
+                ContainerController.stop_docker_stats_thread(execution=exec, physical_server_ip=physical_server_ip,
+                                                             logger=logger)
             except Exception:
                 pass
             EmulationEnvController.delete_networks_of_emulation_env_config(
                 emulation_env_config=exec.emulation_env_config, physical_server_ip=physical_server_ip, logger=logger,
                 leader=leader)
 
     @staticmethod
@@ -568,15 +572,16 @@
         """
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=execution_id,
                                                             emulation_name=emulation_env_config.name)
         EmulationEnvController.stop_containers(execution=execution, physical_server_ip=physical_server_ip,
                                                logger=logger)
         EmulationEnvController.rm_containers(execution=execution, physical_server_ip=physical_server_ip, logger=logger)
         try:
-            ContainerController.stop_docker_stats_thread(execution=execution, physical_server_ip=physical_server_ip)
+            ContainerController.stop_docker_stats_thread(execution=execution, physical_server_ip=physical_server_ip,
+                                                         logger=logger)
         except Exception:
             pass
         EmulationEnvController.delete_networks_of_emulation_env_config(
             emulation_env_config=execution.emulation_env_config, physical_server_ip=physical_server_ip, logger=logger,
             leader=leader)
 
     @staticmethod
@@ -591,15 +596,16 @@
         """
         executions = MetastoreFacade.list_emulation_executions()
         for exec in executions:
             EmulationEnvController.stop_containers(execution=exec, physical_server_ip=physical_server_ip,
                                                    logger=logger)
             EmulationEnvController.rm_containers(execution=exec, physical_server_ip=physical_server_ip, logger=logger)
             try:
-                ContainerController.stop_docker_stats_thread(execution=exec, physical_server_ip=physical_server_ip)
+                ContainerController.stop_docker_stats_thread(execution=exec, physical_server_ip=physical_server_ip,
+                                                             logger=logger)
             except Exception:
                 pass
             EmulationEnvController.delete_networks_of_emulation_env_config(
                 emulation_env_config=exec.emulation_env_config, physical_server_ip=physical_server_ip, logger=logger,
                 leader=leader)
             MetastoreFacade.remove_emulation_execution(emulation_execution=exec)
```

### Comparing `csle_common-0.1.9/src/csle_common/controllers/flags_controller.py` & `csle_common-0.2.0/src/csle_common/controllers/flags_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/controllers/host_controller.py` & `csle_common-0.2.0/src/csle_common/controllers/host_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,16 @@
         # Check if host_manager is already running
         cmd = (constants.COMMANDS.PS_AUX + " | " + constants.COMMANDS.GREP +
                constants.COMMANDS.SPACE_DELIM + constants.TRAFFIC_COMMANDS.HOST_MANAGER_FILE_NAME)
         o, e, _ = EmulationUtil.execute_ssh_cmd(cmd=cmd,
                                                 conn=emulation_env_config.get_connection(ip=ip))
 
         if constants.COMMANDS.SEARCH_HOST_MANAGER not in str(o):
-            logger.info(f"Host manager is not running on: {ip}, starting it. Output of {cmd} was: {str(o)}")
+            logger.info(f"Host manager is not running on: {ip}, starting it. Output of {cmd} was: {str(o)}, "
+                        f"err output was: {str(e)}")
 
             # Stop old background job if running
             cmd = (constants.COMMANDS.SUDO + constants.COMMANDS.SPACE_DELIM + constants.COMMANDS.PKILL +
                    constants.COMMANDS.SPACE_DELIM + constants.TRAFFIC_COMMANDS.HOST_MANAGER_FILE_NAME)
             o, e, _ = EmulationUtil.execute_ssh_cmd(cmd=cmd,
                                                     conn=emulation_env_config.get_connection(ip=ip))
 
@@ -213,16 +214,16 @@
                 emulation_env_config=emulation_env_config,
                 ips=([emulation_env_config.elk_config.container.docker_gw_bridge_ip] +
                      emulation_env_config.elk_config.container.get_ips()),
                 initial_start=initial_start, logger=logger)
 
         if emulation_env_config.sdn_controller_config is not None \
                 and emulation_env_config.sdn_controller_config.container.physical_host_ip == physical_server_ip:
-            # Start packetbeat on the SDN controller container
-            HostController.start_packetbeat(
+            # Start filebeat on the SDN controller container
+            HostController.start_filebeat(
                 emulation_env_config=emulation_env_config,
                 ips=([emulation_env_config.sdn_controller_config.container.docker_gw_bridge_ip] +
                      emulation_env_config.sdn_controller_config.container.get_ips()),
                 initial_start=initial_start, logger=logger)
 
     @staticmethod
     def start_packetbeats(emulation_env_config: EmulationEnvConfig, physical_server_ip: str, logger: logging.Logger,
@@ -699,16 +700,15 @@
         if initial_start:
             node_beats_config = emulation_env_config.beats_config.get_node_beats_config_by_ips(ips=ips)
             if node_beats_config is None or not node_beats_config.start_filebeat_automatically:
                 return
         host_monitor_dto = HostController.get_host_monitor_thread_status_by_port_and_ip(
             ip=ips[0], port=emulation_env_config.host_manager_config.host_manager_port)
         if not host_monitor_dto.filebeat_running:
-            logger.info(
-                f"Filebeat is not running on {ips[0]}, starting it.")
+            logger.info(f"Filebeat is not running on {ips[0]}, starting it.")
             # Open a gRPC session
             with grpc.insecure_channel(
                     f'{ips[0]}:{emulation_env_config.host_manager_config.host_manager_port}') as channel:
                 stub = csle_collector.host_manager.host_manager_pb2_grpc.HostManagerStub(channel)
                 csle_collector.host_manager.query_host_manager.start_filebeat(stub=stub)
 
     @staticmethod
@@ -796,14 +796,88 @@
             # Open a gRPC session
             with grpc.insecure_channel(
                     f'{ips[0]}:{emulation_env_config.host_manager_config.host_manager_port}') as channel:
                 stub = csle_collector.host_manager.host_manager_pb2_grpc.HostManagerStub(channel)
                 csle_collector.host_manager.query_host_manager.start_heartbeat(stub=stub)
 
     @staticmethod
+    def start_sparks(emulation_env_config: EmulationEnvConfig, physical_server_ip: str, logger: logging.Logger) -> None:
+        """
+        Utility function for starting Spark on compute nodes
+
+        :param emulation_config: the emulation env configuration
+        :param physical_server_ip: the ip of the phsyical server
+        :param logger: the logger to use for logging
+        :return: None
+        """
+        for c in emulation_env_config.containers_config.containers:
+            if c.physical_host_ip != physical_server_ip:
+                continue
+            for ids_image in constants.CONTAINER_IMAGES.SPARK_IMAGES:
+                if ids_image in c.name:
+                    logger.info(f"Starting Spark on IP: {c.docker_gw_bridge_ip}")
+                    HostController.start_spark(emulation_env_config=emulation_env_config, ips=[c.docker_gw_bridge_ip],
+                                               logger=logger)
+
+    @staticmethod
+    def stop_sparks(emulation_env_config: EmulationEnvConfig, physical_server_ip: str, logger: logging.Logger) -> None:
+        """
+        Utility function for stopping Spark on compute nodes
+
+        :param emulation_config: the emulation env configuration
+        :param physical_server_ip: the ip of the phsyical server
+        :param logger: the logger to use for logging
+        :return: None
+        """
+        for c in emulation_env_config.containers_config.containers:
+            if c.physical_host_ip != physical_server_ip:
+                continue
+            for ids_image in constants.CONTAINER_IMAGES.SPARK_IMAGES:
+                if ids_image in c.name:
+                    logger.info(f"Stopping Spark on IP: {c.docker_gw_bridge_ip}")
+                    HostController.stop_spark(emulation_env_config=emulation_env_config,
+                                              ips=[c.docker_gw_bridge_ip], logger=logger)
+
+    @staticmethod
+    def start_spark(emulation_env_config: EmulationEnvConfig, ips: List[str], logger: logging.Logger) -> None:
+        """
+        A method that sends a request to the HostManager on a specific IP
+        to start the Host manager and spark
+
+        :param emulation_env_config: the emulation env config
+        :param ips: IPs of the container
+        :param logger: the logger to use for logging
+        :return: None
+        """
+        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ips[0], logger=logger)
+        # Open a gRPC session
+        with grpc.insecure_channel(
+                f'{ips[0]}:{emulation_env_config.host_manager_config.host_manager_port}') as channel:
+            stub = csle_collector.host_manager.host_manager_pb2_grpc.HostManagerStub(channel)
+            csle_collector.host_manager.query_host_manager.start_spark(stub=stub)
+
+    @staticmethod
+    def stop_spark(emulation_env_config: EmulationEnvConfig, ips: List[str], logger: logging.Logger) -> None:
+        """
+        A method that sends a request to the HostManager on a specific IP
+        to stop spark
+
+        :param emulation_env_config: the emulation env config
+        :param ips: IPs of the container
+        :param logger: the logger to use for logging
+        :return: None
+        """
+        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ips[0], logger=logger)
+        # Open a gRPC session
+        with grpc.insecure_channel(
+                f'{ips[0]}:{emulation_env_config.host_manager_config.host_manager_port}') as channel:
+            stub = csle_collector.host_manager.host_manager_pb2_grpc.HostManagerStub(channel)
+            csle_collector.host_manager.query_host_manager.stop_spark(stub=stub)
+
+    @staticmethod
     def config_filebeat(emulation_env_config: EmulationEnvConfig, container: NodeContainerConfig,
                         logger: logging.Logger) -> None:
         """
         A method that sends a request to the HostManager on a specific container
         to setup the filebeat configuration
 
         :param emulation_env_config: the emulation env config
```

### Comparing `csle_common-0.1.9/src/csle_common/controllers/installation_controller.py` & `csle_common-0.2.0/src/csle_common/controllers/installation_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/controllers/kafka_controller.py` & `csle_common-0.2.0/src/csle_common/controllers/kafka_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/controllers/ossec_ids_controller.py` & `csle_common-0.2.0/src/csle_common/controllers/ossec_ids_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/controllers/ovs_controller.py` & `csle_common-0.2.0/src/csle_common/controllers/ovs_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/controllers/resource_constraints_controller.py` & `csle_common-0.2.0/src/csle_common/controllers/resource_constraints_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/controllers/sdn_controller_manager.py` & `csle_common-0.2.0/src/csle_common/controllers/sdn_controller_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import csle_collector.ryu_manager.ryu_manager_pb2
 import csle_collector.ryu_manager.query_ryu_server
 import csle_collector.ryu_manager.ryu_manager_util
 import csle_common.constants.constants as constants
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
 from csle_common.dao.emulation_config.ryu_managers_info import RyuManagersInfo
 from csle_common.util.emulation_util import EmulationUtil
-from csle_common.logging.log import Logger
 
 
 class SDNControllerManager:
     """
     Class managing interaction with the SDN controller
     """
 
@@ -35,14 +34,15 @@
         # Check if ryu_manager is already running
         cmd = (constants.COMMANDS.PS_AUX + " | " + constants.COMMANDS.GREP + constants.COMMANDS.SPACE_DELIM +
                constants.TRAFFIC_COMMANDS.RYU_MANAGER_FILE_NAME)
         o, e, _ = EmulationUtil.execute_ssh_cmd(
             cmd=cmd,
             conn=emulation_env_config.get_connection(
                 ip=emulation_env_config.sdn_controller_config.container.docker_gw_bridge_ip))
+        logger.info(f"Ryu manager running?, cmd: {cmd}, out:{o.decode()}, err: {e.decode()}")
 
         if constants.COMMANDS.SEARCH_RYU_MANAGER not in str(o):
             logger.info(
                 f"Starting ryu manager on node: "
                 f"{emulation_env_config.sdn_controller_config.container.docker_gw_bridge_ip}")
 
             # Stop old background job if running
@@ -59,41 +59,43 @@
                 emulation_env_config.sdn_controller_config.manager_log_dir,
                 emulation_env_config.sdn_controller_config.manager_log_file,
                 emulation_env_config.sdn_controller_config.manager_max_workers)
             o, e, _ = EmulationUtil.execute_ssh_cmd(
                 cmd=cmd,
                 conn=emulation_env_config.get_connection(
                     ip=emulation_env_config.sdn_controller_config.container.docker_gw_bridge_ip))
+            logger.info(f"Starting the Ryu manager, cmd: {cmd}, out:{o.decode()}, err: {e.decode()}")
             time.sleep(2)
 
     @staticmethod
-    def stop_ryu_manager(emulation_env_config: EmulationEnvConfig) -> None:
+    def stop_ryu_manager(emulation_env_config: EmulationEnvConfig, logger: logging.Logger) -> None:
         """
         Utility method for stopping the Ryu manager
 
         :param emulation_env_config: the emulation env config
+        :param logger: the logger to use for logging
         :return: None
         """
         # Connect
         EmulationUtil.connect_admin(emulation_env_config=emulation_env_config,
                                     ip=emulation_env_config.sdn_controller_config.container.docker_gw_bridge_ip,
                                     create_producer=False)
 
-        Logger.__call__().get_logger().info(
+        logger.info(
             f"Stopping ryu manager on node: "
             f"{emulation_env_config.sdn_controller_config.container.docker_gw_bridge_ip}")
 
         # Stop background job
         cmd = (constants.COMMANDS.SUDO + constants.COMMANDS.SPACE_DELIM + constants.COMMANDS.PKILL +
                constants.COMMANDS.SPACE_DELIM + constants.TRAFFIC_COMMANDS.RYU_MANAGER_FILE_NAME)
         o, e, _ = EmulationUtil.execute_ssh_cmd(
             cmd=cmd,
             conn=emulation_env_config.get_connection(
                 ip=emulation_env_config.sdn_controller_config.container.docker_gw_bridge_ip))
-
+        logger.info(f"Stopping the Ryu manager, cmd: {cmd}, out:{o.decode()}, err: {e.decode()}")
         time.sleep(2)
 
     @staticmethod
     def get_ryu_status(emulation_env_config: EmulationEnvConfig, logger: logging.Logger) -> \
             csle_collector.ryu_manager.ryu_manager_pb2.RyuDTO:
         """
         Method for querying the RyuManager about the status of the Ryu SDN controller
@@ -201,15 +203,15 @@
 
         # Open a gRPC session
         with grpc.insecure_channel(
                 f'{emulation_env_config.sdn_controller_config.container.docker_gw_bridge_ip}:'
                 f'{emulation_env_config.sdn_controller_config.manager_port}') as channel:
             stub = csle_collector.ryu_manager.ryu_manager_pb2_grpc.RyuManagerStub(channel)
             ryu_dto = csle_collector.ryu_manager.query_ryu_server.start_ryu_monitor(
-                stub, kafka_ip=emulation_env_config.kafka_config.container.docker_gw_bridge_ip,
+                stub, kafka_ip=emulation_env_config.kafka_config.container.get_ips()[0],
                 kafka_port=emulation_env_config.kafka_config.kafka_port,
                 time_step_len=emulation_env_config.sdn_controller_config.time_step_len_seconds)
             return ryu_dto
 
     @staticmethod
     def stop_ryu_monitor(emulation_env_config: EmulationEnvConfig, logger: logging.Logger) -> \
             csle_collector.ryu_manager.ryu_manager_pb2.RyuDTO:
```

### Comparing `csle_common-0.1.9/src/csle_common/controllers/simulation_env_controller.py` & `csle_common-0.2.0/src/csle_common/controllers/simulation_env_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/controllers/snort_ids_controller.py` & `csle_common-0.2.0/src/csle_common/controllers/snort_ids_controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,139 +7,151 @@
 import csle_common.constants.constants as constants
 import csle_collector.constants.constants as csle_collector_constants
 import csle_collector.snort_ids_manager.snort_ids_manager_pb2_grpc
 import csle_collector.snort_ids_manager.snort_ids_manager_pb2
 import csle_collector.snort_ids_manager.query_snort_ids_manager
 import csle_collector.snort_ids_manager.snort_ids_manager_util
 from csle_common.util.emulation_util import EmulationUtil
-from csle_common.logging.log import Logger
 
 
 class SnortIDSController:
     """
     Class managing operations related to Snort IDS Managers
     """
 
     @staticmethod
     def start_snort_idses(emulation_env_config: EmulationEnvConfig, physical_server_ip: str,
                           logger: logging.Logger) -> None:
         """
         Utility function for starting the Snort IDSes
 
-        :param emulation_config: the emulation env configuration
+        :param emulation_env_config: the emulation env configuration
         :param physical_server_ip: the ip of the phsyical server
         :param logger: the logger to use for logging
         :return: None
         """
         for c in emulation_env_config.containers_config.containers:
             if c.physical_host_ip != physical_server_ip:
                 continue
             for ids_image in constants.CONTAINER_IMAGES.SNORT_IDS_IMAGES:
                 if ids_image in c.name:
                     logger.info(f"Starting the Snort IDS on IP: {c.docker_gw_bridge_ip}")
                     SnortIDSController.start_snort_ids(emulation_env_config=emulation_env_config,
-                                                       ip=c.docker_gw_bridge_ip)
+                                                       ip=c.docker_gw_bridge_ip, logger=logger)
 
     @staticmethod
-    def stop_snort_idses(emulation_env_config: EmulationEnvConfig, physical_server_ip: str) -> None:
+    def stop_snort_idses(emulation_env_config: EmulationEnvConfig, physical_server_ip: str,
+                         logger: logging.Logger) -> None:
         """
         Utility function for stopping the Snort IDSes
 
-        :param emulation_config: the emulation env configuration
+        :param emulation_env_config: the emulation env configuration
         :param physical_server_ip: the ip of the physical server
+        :param logger: the logger to use for logging
         :return: None
         """
         for c in emulation_env_config.containers_config.containers:
             if c.physical_host_ip != physical_server_ip:
                 continue
             for ids_image in constants.CONTAINER_IMAGES.SNORT_IDS_IMAGES:
                 if ids_image in c.name:
                     SnortIDSController.stop_snort_ids(emulation_env_config=emulation_env_config,
-                                                      ip=c.docker_gw_bridge_ip)
+                                                      ip=c.docker_gw_bridge_ip, logger=logger)
 
     @staticmethod
-    def start_snort_ids(emulation_env_config: EmulationEnvConfig, ip: str) -> None:
+    def start_snort_ids(emulation_env_config: EmulationEnvConfig, ip: str, logger: logging.Logger) -> None:
         """
         Utility function for starting the Snort IDS on a specific IP
 
-        :param emulation_config: the emulation env configuration
+        :param emulation_env_config: the emulation env configuration
         :param ip: the ip of the container
+        :param logger: the logger to use for logging
         :return: None
         """
-        SnortIDSController.start_snort_manager(emulation_env_config=emulation_env_config, ip=ip)
+        SnortIDSController.start_snort_manager(emulation_env_config=emulation_env_config, ip=ip, logger=logger)
         ids_monitor_dto = SnortIDSController.get_snort_idses_monitor_threads_statuses_by_ip_and_port(
             port=emulation_env_config.snort_ids_manager_config.snort_ids_manager_port, ip=ip)
         if not ids_monitor_dto.snort_ids_running:
-            Logger.__call__().get_logger().info(
-                f"Snort IDS is not running on {ip}, starting it.")
+            logger.info(f"Snort IDS is not running on {ip}, starting it.")
+            subnetmask = f"{emulation_env_config.execution_id}.{emulation_env_config.level}" \
+                         f"{constants.CSLE.CSLE_LEVEL_SUBNETMASK_SUFFIX}"
+            ingress_interface = constants.NETWORKING.ETH2
+            egress_interface = constants.NETWORKING.ETH0
+            logger.info(f"Subnetmask: {subnetmask}, ingress interface: {ingress_interface}, "
+                        f"egress interface: {egress_interface}")
             # Open a gRPC session
             with grpc.insecure_channel(
                     f'{ip}:'
                     f'{emulation_env_config.snort_ids_manager_config.snort_ids_manager_port}') as channel:
                 stub = csle_collector.snort_ids_manager.snort_ids_manager_pb2_grpc.SnortIdsManagerStub(channel)
-                csle_collector.snort_ids_manager.query_snort_ids_manager.start_snort_ids(stub=stub)
+                csle_collector.snort_ids_manager.query_snort_ids_manager.start_snort_ids(
+                    stub=stub, ingress_interface=ingress_interface, egress_interface=egress_interface,
+                    subnetmask=subnetmask)
 
     @staticmethod
-    def stop_snort_ids(emulation_env_config: EmulationEnvConfig, ip: str) -> None:
+    def stop_snort_ids(emulation_env_config: EmulationEnvConfig, ip: str, logger: logging.Logger) -> None:
         """
         Utility function for stopping the Snort IDS on a specific IP
 
-        :param emulation_config: the emulation env configuration
+        :param emulation_env_config: the emulation env configuration
         :param ip: the ip of the container
+        :param logger: the logger to use for logging
         :return: None
         """
-        SnortIDSController.start_snort_manager(emulation_env_config=emulation_env_config, ip=ip)
+        SnortIDSController.start_snort_manager(emulation_env_config=emulation_env_config, ip=ip, logger=logger)
         ids_monitor_dto = SnortIDSController.get_snort_idses_monitor_threads_statuses_by_ip_and_port(
             port=emulation_env_config.snort_ids_manager_config.snort_ids_manager_port, ip=ip)
         if ids_monitor_dto.snort_ids_running:
-            Logger.__call__().get_logger().info(
-                f"Snort IDS is running on {ip}, stopping it.")
+            logger.info(f"Snort IDS is running on {ip}, stopping it.")
             # Open a gRPC session
             with grpc.insecure_channel(
                     f'{ip}:'
                     f'{emulation_env_config.snort_ids_manager_config.snort_ids_manager_port}') as channel:
                 stub = csle_collector.snort_ids_manager.snort_ids_manager_pb2_grpc.SnortIdsManagerStub(channel)
                 csle_collector.snort_ids_manager.query_snort_ids_manager.stop_snort_ids(stub=stub)
 
     @staticmethod
-    def start_snort_managers(emulation_env_config: EmulationEnvConfig, physical_server_ip: str) -> None:
+    def start_snort_managers(emulation_env_config: EmulationEnvConfig, physical_server_ip: str,
+                             logger: logging.Logger) -> None:
         """
         Utility function for starting snort IDS managers
 
         :param emulation_env_config: the emulation env config
         :param physical_server_ip: the physical server ip
+        :param logger: the logger to use for logging
         :return: None
         """
         for c in emulation_env_config.containers_config.containers:
             if c.physical_host_ip != physical_server_ip:
                 continue
             for ids_image in constants.CONTAINER_IMAGES.SNORT_IDS_IMAGES:
                 if ids_image in c.name:
                     SnortIDSController.start_snort_manager(emulation_env_config=emulation_env_config,
-                                                           ip=c.docker_gw_bridge_ip)
+                                                           ip=c.docker_gw_bridge_ip, logger=logger)
 
     @staticmethod
-    def start_snort_manager(emulation_env_config: EmulationEnvConfig, ip: str) -> None:
+    def start_snort_manager(emulation_env_config: EmulationEnvConfig, ip: str, logger: logging.Logger) -> None:
         """
         Utility function for starting the snort IDS manager on a specific IP
 
         :param emulation_env_config: the emulation env config
         :param ip: IP of the container
+        :param logger: the logger to use for logging
         :return: None
         """
         # Connect
         EmulationUtil.connect_admin(emulation_env_config=emulation_env_config, ip=ip)
 
         # Check if ids_manager is already running
         cmd = (constants.COMMANDS.PS_AUX + " | " + constants.COMMANDS.GREP + constants.COMMANDS.SPACE_DELIM +
                constants.TRAFFIC_COMMANDS.SNORT_IDS_MANAGER_FILE_NAME)
         o, e, _ = EmulationUtil.execute_ssh_cmd(cmd=cmd, conn=emulation_env_config.get_connection(ip=ip))
 
         if constants.COMMANDS.SEARCH_SNORT_IDS_MANAGER not in str(o):
-            Logger.__call__().get_logger().info(f"Starting Snort IDS manager on node {ip}")
+            logger.info(f"Starting Snort IDS manager on node {ip}")
 
             # Stop old background job if running
             cmd = (constants.COMMANDS.SUDO + constants.COMMANDS.SPACE_DELIM + constants.COMMANDS.PKILL +
                    constants.COMMANDS.SPACE_DELIM + constants.TRAFFIC_COMMANDS.SNORT_IDS_MANAGER_FILE_NAME)
             o, e, _ = EmulationUtil.execute_ssh_cmd(
                 cmd=cmd, conn=emulation_env_config.get_connection(ip=ip))
 
@@ -150,42 +162,45 @@
                 emulation_env_config.snort_ids_manager_config.snort_ids_manager_log_file,
                 emulation_env_config.snort_ids_manager_config.snort_ids_manager_max_workers)
             o, e, _ = EmulationUtil.execute_ssh_cmd(
                 cmd=cmd, conn=emulation_env_config.get_connection(ip=ip))
             time.sleep(2)
 
     @staticmethod
-    def stop_snort_managers(emulation_env_config: EmulationEnvConfig, physical_server_ip: str) -> None:
+    def stop_snort_managers(emulation_env_config: EmulationEnvConfig, physical_server_ip: str,
+                            logger: logging.Logger) -> None:
         """
         Utility function for stopping snort IDS managers
 
         :param emulation_env_config: the emulation env config
         :param physical_server_ip: the physical server ip
+        :param logger: the logger to use for logging
         :return: None
         """
         for c in emulation_env_config.containers_config.containers:
             if c.physical_host_ip != physical_server_ip:
                 continue
             for ids_image in constants.CONTAINER_IMAGES.SNORT_IDS_IMAGES:
                 if ids_image in c.name:
                     SnortIDSController.stop_snort_manager(emulation_env_config=emulation_env_config,
-                                                          ip=c.docker_gw_bridge_ip)
+                                                          ip=c.docker_gw_bridge_ip, logger=logger)
 
     @staticmethod
-    def stop_snort_manager(emulation_env_config: EmulationEnvConfig, ip: str) -> None:
+    def stop_snort_manager(emulation_env_config: EmulationEnvConfig, ip: str, logger: logging.Logger) -> None:
         """
         Utility function for stopping the snort IDS manager on a specific IP
 
         :param emulation_env_config: the emulation env config
         :param ip: the IP of the container
+        :param logger: the logger to use for logging
         :return: None
         """
         # Connect
         EmulationUtil.connect_admin(emulation_env_config=emulation_env_config, ip=ip)
-        Logger.__call__().get_logger().info(f"Stopping Snort IDS manager on node {ip}")
+        logger.info(f"Stopping Snort IDS manager on node {ip}")
 
         cmd = (constants.COMMANDS.SUDO + constants.COMMANDS.SPACE_DELIM + constants.COMMANDS.PKILL +
                constants.COMMANDS.SPACE_DELIM + constants.TRAFFIC_COMMANDS.SNORT_IDS_MANAGER_FILE_NAME)
         o, e, _ = EmulationUtil.execute_ssh_cmd(cmd=cmd, conn=emulation_env_config.get_connection(ip=ip))
 
         time.sleep(2)
 
@@ -204,99 +219,105 @@
         for c in emulation_env_config.containers_config.containers:
             if c.physical_host_ip != physical_server_ip:
                 continue
             for ids_image in constants.CONTAINER_IMAGES.SNORT_IDS_IMAGES:
                 if ids_image in c.name:
                     logger.info(f"Starting Snort IDS monitor thread on IP: {c.docker_gw_bridge_ip}")
                     SnortIDSController.start_snort_idses_monitor_thread(emulation_env_config=emulation_env_config,
-                                                                        ip=c.docker_gw_bridge_ip)
+                                                                        ip=c.docker_gw_bridge_ip, logger=logger)
 
     @staticmethod
-    def start_snort_idses_monitor_thread(emulation_env_config: EmulationEnvConfig, ip: str) -> None:
+    def start_snort_idses_monitor_thread(emulation_env_config: EmulationEnvConfig, ip: str,
+                                         logger: logging.Logger) -> None:
         """
         A method that sends a request to the SnortIDSManager on a specific container that runs
         an IDS to start the IDS manager and the monitor thread
 
         :param emulation_env_config: the emulation env config
         :param ip: the ip of the container
+        :param logger: the logger to use for logging
         :return: None
         """
-        SnortIDSController.start_snort_manager(emulation_env_config=emulation_env_config, ip=ip)
+        SnortIDSController.start_snort_manager(emulation_env_config=emulation_env_config, ip=ip, logger=logger)
 
         ids_monitor_dto = SnortIDSController.get_snort_idses_monitor_threads_statuses_by_ip_and_port(
             port=emulation_env_config.snort_ids_manager_config.snort_ids_manager_port, ip=ip)
         if not ids_monitor_dto.monitor_running:
-            Logger.__call__().get_logger().info(
-                f"Snort IDS monitor thread is not running on {ip}, starting it.")
+            logger.info(f"Snort IDS monitor thread is not running on {ip}, starting it.")
             # Open a gRPC session
             with grpc.insecure_channel(
                     f'{ip}:'
                     f'{emulation_env_config.snort_ids_manager_config.snort_ids_manager_port}') as channel:
                 stub = csle_collector.snort_ids_manager.snort_ids_manager_pb2_grpc.SnortIdsManagerStub(channel)
                 csle_collector.snort_ids_manager.query_snort_ids_manager.start_snort_ids_monitor(
                     stub=stub, kafka_ip=emulation_env_config.kafka_config.container.get_ips()[0],
                     kafka_port=emulation_env_config.kafka_config.kafka_port,
                     log_file_path=csle_collector_constants.SNORT_IDS_ROUTER.SNORT_FAST_LOG_FILE,
                     time_step_len_seconds=emulation_env_config.snort_ids_manager_config.time_step_len_seconds)
 
     @staticmethod
-    def stop_snort_idses_monitor_threads(emulation_env_config: EmulationEnvConfig, physical_server_ip: str) -> None:
+    def stop_snort_idses_monitor_threads(emulation_env_config: EmulationEnvConfig, physical_server_ip: str,
+                                         logger: logging.Logger) -> None:
         """
         A method that sends a request to the SnortIDSManager on every container that runs
         an IDS to stop the monitor threads
 
         :param emulation_env_config: the emulation env config
         :param physical_server_ip: the physical server ip
+        :param logger: the logger to use for logging
         :return: None
         """
         for c in emulation_env_config.containers_config.containers:
             if c.physical_host_ip != physical_server_ip:
                 continue
             for ids_image in constants.CONTAINER_IMAGES.SNORT_IDS_IMAGES:
                 if ids_image in c.name:
                     SnortIDSController.stop_snort_idses_monitor_thread(emulation_env_config=emulation_env_config,
-                                                                       ip=c.docker_gw_bridge_ip)
+                                                                       ip=c.docker_gw_bridge_ip, logger=logger)
 
     @staticmethod
-    def stop_snort_idses_monitor_thread(emulation_env_config: EmulationEnvConfig, ip: str) -> None:
+    def stop_snort_idses_monitor_thread(emulation_env_config: EmulationEnvConfig, ip: str,
+                                        logger: logging.Logger) -> None:
         """
         A method that sends a request to the SnortIDSManager on a specific container that runs
         an IDS to stop the monitor threads
 
         :param emulation_env_config: the emulation env config
         :param ip: the IP of the container
+        :param logger: the logger to use for logging
         :return: None
         """
-        SnortIDSController.start_snort_manager(emulation_env_config=emulation_env_config, ip=ip)
+        SnortIDSController.start_snort_manager(emulation_env_config=emulation_env_config, ip=ip, logger=logger)
         # Open a gRPC session
         with grpc.insecure_channel(
                 f'{ip}:'
                 f'{emulation_env_config.snort_ids_manager_config.snort_ids_manager_port}') as channel:
             stub = csle_collector.snort_ids_manager.snort_ids_manager_pb2_grpc.SnortIdsManagerStub(channel)
-            Logger.__call__().get_logger().info(
-                f"Stopping the Snort IDS monitor thread on {ip}.")
+            logger.info(f"Stopping the Snort IDS monitor thread on {ip}.")
             csle_collector.snort_ids_manager.query_snort_ids_manager.stop_snort_ids_monitor(stub=stub)
 
     @staticmethod
     def get_snort_idses_monitor_threads_statuses(emulation_env_config: EmulationEnvConfig, physical_server_ip: str,
-                                                 start_if_stopped: bool = True) -> \
+                                                 logger: logging.Logger, start_if_stopped: bool = True) -> \
             List[csle_collector.snort_ids_manager.snort_ids_manager_pb2.SnortIdsMonitorDTO]:
         """
         A method that sends a request to the SnortIDSManager on every container to get the status of the
         IDS monitor thread
 
         :param emulation_env_config: the emulation config
         :param start_if_stopped: whether to start the IDS monitor if it is stopped
         :param physical_server_ip: the physical server IP
+        :param logger: the logger to use for logging
         :return: List of monitor thread statuses
         """
         statuses = []
         if start_if_stopped:
             SnortIDSController.start_snort_managers(emulation_env_config=emulation_env_config,
-                                                    physical_server_ip=physical_server_ip)
+                                                    physical_server_ip=physical_server_ip,
+                                                    logger=logger)
 
         for c in emulation_env_config.containers_config.containers:
             if c.physical_host_ip != physical_server_ip:
                 continue
             for ids_image in constants.CONTAINER_IMAGES.SNORT_IDS_IMAGES:
                 if ids_image in c.name:
                     status = SnortIDSController.get_snort_idses_monitor_threads_statuses_by_ip_and_port(
```

### Comparing `csle_common-0.1.9/src/csle_common/controllers/topology_controller.py` & `csle_common-0.2.0/src/csle_common/controllers/topology_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,23 +31,25 @@
             ip = node_fw_config.docker_gw_bridge_ip
             logger.info(f"Connecting to node:{ip}")
             EmulationUtil.connect_admin(emulation_env_config=emulation_env_config, ip=ip)
 
             for route in node_fw_config.routes:
                 target, gw = route
                 cmd = f"{constants.COMMANDS.SUDO_ADD_ROUTE} {target} gw {gw}"
+                logger.info(f"Adding route: {cmd} to routing table of node: {ip}")
                 EmulationUtil.execute_ssh_cmd(cmd=cmd, conn=emulation_env_config.get_connection(ip=ip),
                                               wait_for_completion=True)
 
             for default_network_fw_config in node_fw_config.ips_gw_default_policy_networks:
                 if default_network_fw_config.default_gw is not None:
                     cmd = f"{constants.COMMANDS.SUDO_ADD_ROUTE} " \
-                          f"-net {default_network_fw_config.network.subnet_mask.replace('/24', '')} " \
+                          f"-net {default_network_fw_config.network.subnet_mask.split('/')[0]} " \
                           f"{constants.COMMANDS.NETMASK} {default_network_fw_config.network.bitmask} " \
                           f"gw {default_network_fw_config.default_gw}"
+                    logger.info(f"Adding default gw: {cmd} to routing table of node: {ip}")
                     EmulationUtil.execute_ssh_cmd(cmd=cmd, conn=emulation_env_config.get_connection(ip=ip),
                                                   wait_for_completion=True)
 
             cmd = constants.COMMANDS.CLEAR_IPTABLES
             EmulationUtil.execute_ssh_cmd(cmd=cmd, conn=emulation_env_config.get_connection(ip=ip),
                                           wait_for_completion=True)
```

### Comparing `csle_common-0.1.9/src/csle_common/controllers/traffic_controller.py` & `csle_common-0.2.0/src/csle_common/controllers/traffic_controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -347,24 +347,56 @@
                 time.sleep(2)
 
             # Start the client population
             sine_modulated = False
             if (emulation_env_config.traffic_config.client_population_config.client_process_type ==
                     ClientPopulationProcessType.SINE_MODULATED_POISSON):
                 sine_modulated = True
+            spiking = False
+            if (emulation_env_config.traffic_config.client_population_config.client_process_type ==
+                    ClientPopulationProcessType.SPIKING):
+                spiking = True
+            piece_wise_constant = False
+            if (emulation_env_config.traffic_config.client_population_config.client_process_type ==
+                    ClientPopulationProcessType.PIECE_WISE_CONSTANT):
+                piece_wise_constant = True
             time_step_len = emulation_env_config.traffic_config.client_population_config.client_time_step_len_seconds
+            logger.info(
+                f"Starting the client population, "
+                f"mu: {emulation_env_config.traffic_config.client_population_config.mu},\n"
+                f"lamb: {emulation_env_config.traffic_config.client_population_config.lamb},\n"
+                f"time_step_len_seconds: {time_step_len},\n"
+                f"commands: {commands},\n"
+                f"num_commands: {emulation_env_config.traffic_config.client_population_config.num_commands},\n"
+                f"sine_modulated: {sine_modulated},\n"
+                f"time_scaling_factor:"
+                f"{emulation_env_config.traffic_config.client_population_config.time_scaling_factor},\n"
+                f"period_scaling_factor: "
+                f"{emulation_env_config.traffic_config.client_population_config.period_scaling_factor},\n"
+                f"spiking: {spiking},\n piece_wise_constant: {piece_wise_constant},\n "
+                f"exponents: {emulation_env_config.traffic_config.client_population_config.exponents},\n "
+                f"factors: {emulation_env_config.traffic_config.client_population_config.factors},\n "
+                f"breakvalues: {emulation_env_config.traffic_config.client_population_config.breakvalues}, \n"
+                f"breakpoints: {emulation_env_config.traffic_config.client_population_config.breakpoints}"
+            )
             csle_collector.client_manager.query_clients.start_clients(
                 stub=stub, mu=emulation_env_config.traffic_config.client_population_config.mu,
                 lamb=emulation_env_config.traffic_config.client_population_config.lamb,
                 time_step_len_seconds=time_step_len,
                 commands=commands,
                 num_commands=emulation_env_config.traffic_config.client_population_config.num_commands,
                 sine_modulated=sine_modulated,
                 time_scaling_factor=emulation_env_config.traffic_config.client_population_config.time_scaling_factor,
-                period_scaling_factor=emulation_env_config.traffic_config.client_population_config.period_scaling_factor
+                period_scaling_factor=(
+                    emulation_env_config.traffic_config.client_population_config.period_scaling_factor),
+                spiking=spiking, piece_wise_constant=piece_wise_constant,
+                exponents=emulation_env_config.traffic_config.client_population_config.exponents,
+                factors=emulation_env_config.traffic_config.client_population_config.factors,
+                breakvalues=emulation_env_config.traffic_config.client_population_config.breakvalues,
+                breakpoints=emulation_env_config.traffic_config.client_population_config.breakpoints
             )
 
     @staticmethod
     def get_num_active_clients(emulation_env_config: EmulationEnvConfig, logger: logging.Logger) \
             -> csle_collector.client_manager.client_manager_pb2.ClientsDTO:
         """
         Gets the number of active clients
@@ -553,15 +585,15 @@
             status = None
             try:
                 status = TrafficController.get_clients_dto_by_ip_and_port(
                     ip=ip,
                     port=emulation_env_config.traffic_config.client_population_config.client_manager_port)
                 running = True
             except Exception as e:
-                logger.debug(
+                logger.info(
                     f"Could not fetch client manager status on IP:{ip}, error: {str(e)}, {repr(e)}")
             if status is not None:
                 client_managers_statuses.append(status)
             else:
                 client_managers_statuses.append(
                     csle_collector.client_manager.client_manager_util.ClientManagerUtil.clients_dto_empty())
             client_managers_running.append(running)
```

### Comparing `csle_common-0.1.9/src/csle_common/controllers/users_controller.py` & `csle_common-0.2.0/src/csle_common/controllers/users_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/controllers/vulnerabilities_controller.py` & `csle_common-0.2.0/src/csle_common/controllers/vulnerabilities_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/datasets/statistics_dataset.py` & `csle_common-0.2.0/src/csle_common/dao/datasets/statistics_dataset.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/datasets/traces_dataset.py` & `csle_common-0.2.0/src/csle_common/dao/datasets/traces_dataset.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/docker/docker_container_metadata.py` & `csle_common-0.2.0/src/csle_common/dao/docker/docker_container_metadata.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/docker/docker_env_metadata.py` & `csle_common-0.2.0/src/csle_common/dao/docker/docker_env_metadata.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/domain_randomization/node_randomizer_config.py` & `csle_common-0.2.0/src/csle_common/dao/domain_randomization/node_randomizer_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/domain_randomization/randomization_space.py` & `csle_common-0.2.0/src/csle_common/dao/domain_randomization/randomization_space.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/domain_randomization/randomization_space_config.py` & `csle_common-0.2.0/src/csle_common/dao/domain_randomization/randomization_space_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List
-import gym
+import gymnasium as gym
 from csle_common.dao.emulation_action.attacker.emulation_attacker_action import EmulationAttackerAction
 from csle_common.dao.emulation_action.attacker.emulation_attacker_action_id import EmulationAttackerActionId
 from csle_common.dao.emulation_action.attacker.emulation_attacker_nmap_actions import EmulationAttackerNMAPActions
 from csle_common.dao.emulation_action.attacker.emulation_attacker_nikto_actions import EmulationAttackerNIKTOActions
 from csle_common.dao.emulation_action.attacker.emulation_attacker_masscan_actions \
     import EmulationAttackerMasscanActions
 from csle_common.dao.emulation_action.attacker.emulation_attacker_network_service_actions \
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_id.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_id.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_masscan_actions.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_masscan_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_network_service_actions.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_network_service_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nikto_actions.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nikto_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nmap_actions.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nmap_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_shell_actions.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_shell_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_stopping_actions.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action/attacker/emulation_attacker_stopping_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/emulation_defender_action.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/emulation_defender_action.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/emulation_defender_action_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/emulation_defender_action_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List
-import gym
+import gymnasium as gym
 from csle_common.dao.emulation_action.defender.emulation_defender_action import EmulationDefenderAction
 from csle_common.dao.emulation_action.defender.emulation_defender_action_id import EmulationDefenderActionId
 from csle_common.dao.emulation_action.defender.emulation_defender_stopping_actions \
     import EmulationDefenderStoppingActions
 
 
 class EmulationDefenderActionConfig:
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/emulation_defender_stopping_actions.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action/defender/emulation_defender_stopping_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nikto_scan_result.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nikto_scan_result.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nikto_vuln.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nikto_vuln.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_brute_credentials.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_brute_credentials.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_hop.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_hop.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_host_result.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_host_result.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_os.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_os.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_port.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_port.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_scan_result.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_scan_result.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_trace.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_trace.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_vuln.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_action_result/nmap_vuln.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/beats_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/beats_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/client_managers_info.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/client_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/client_population_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/client_population_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     """
 
     def __init__(self, ip: str, networks: List[ContainerNetwork], client_process_type: ClientPopulationProcessType,
                  lamb: float, mu: float, client_manager_port: int, client_manager_log_file: str,
                  client_manager_log_dir: str, client_manager_max_workers: int,
                  num_commands: int = 5,
                  client_time_step_len_seconds: int = 1, time_scaling_factor: float = 0.01,
-                 period_scaling_factor: float = 20, docker_gw_bridge_ip: str = "", physical_host_ip: str = ""):
+                 period_scaling_factor: float = 20, docker_gw_bridge_ip: str = "", physical_host_ip: str = "",
+                 exponents=None, factors=None, breakpoints=None, breakvalues=None):
         """
         Creates a ClientPopulationConfig DTO Object
 
         :param ip: the ip of the client container
         :param networks: a list of networks in the emulation that are accessible for external networks
         :param client_process_type: the type of client arrival process (e.g. a Poisson process)
         :param lamb: the lambda parameter of the arrival process
@@ -27,14 +28,18 @@
         :param time_scaling_factor: the time-scaling factor for sine-modulated arrival processes
         :param period_scaling_factor: the period-scaling factor for sine-modulated arrival processes
         :param client_manager_log_file: the log file of the client manager
         :param client_manager_log_dir: the log dir of the client manager
         :param client_manager_max_workers: the maximum number of GRPC workers for the client manager
         :param docker_gw_bridge_ip: IP to reach the container from the host network
         :param physical_host_ip: IP of the physical host where the container is running
+        :param exponents: exponents for spike-moduldated arrival process
+        :param factors: factors for spike-moduldated arrival process
+        :param breakpoints: breakpoints for piece-wise constant arrival process
+        :param breakvalues: breakvalues for piece-wise constant arrival process
         """
         self.networks = networks
         self.ip = ip
         self.client_process_type = client_process_type
         self.lamb = lamb
         self.mu = mu
         self.client_manager_port = client_manager_port
@@ -43,14 +48,18 @@
         self.time_scaling_factor = time_scaling_factor
         self.period_scaling_factor = period_scaling_factor
         self.client_manager_log_dir = client_manager_log_dir
         self.client_manager_log_file = client_manager_log_file
         self.client_manager_max_workers = client_manager_max_workers
         self.docker_gw_bridge_ip = docker_gw_bridge_ip
         self.physical_host_ip = physical_host_ip
+        self.exponents = exponents
+        self.factors = factors
+        self.breakpoints = breakpoints
+        self.breakvalues = breakvalues
 
     @staticmethod
     def from_dict(d: Dict[str, Any]) -> "ClientPopulationConfig":
         """
         Converts a dict representation to an instance
 
         :param d: the dict to convert
@@ -61,15 +70,17 @@
             networks=list(map(lambda x: ContainerNetwork.from_dict(x), d["networks"])),
             client_process_type=d["client_process_type"],
             lamb=d["lamb"], mu=d["mu"], client_manager_port=d["client_manager_port"],
             num_commands=d["num_commands"], client_time_step_len_seconds=d["client_time_step_len_seconds"],
             period_scaling_factor=d["period_scaling_factor"], time_scaling_factor=d["time_scaling_factor"],
             client_manager_log_dir=d["client_manager_log_dir"], client_manager_log_file=d["client_manager_log_file"],
             client_manager_max_workers=d["client_manager_max_workers"],
-            docker_gw_bridge_ip=d["docker_gw_bridge_ip"], physical_host_ip=d["physical_host_ip"]
+            docker_gw_bridge_ip=d["docker_gw_bridge_ip"], physical_host_ip=d["physical_host_ip"],
+            exponents=d["exponents"], factors=d["factors"], breakpoints=d["breakpoints"],
+            breakvalues=d["breakvalues"]
         )
         return obj
 
     def no_clients(self) -> "ClientPopulationConfig":
         """
         :return: A version of the config with no clients
         """
@@ -77,15 +88,16 @@
             ip=self.ip,
             networks=self.networks,
             client_process_type=self.client_process_type,
             lamb=0, mu=0, client_manager_port=self.client_manager_port,
             num_commands=0, client_time_step_len_seconds=self.client_time_step_len_seconds,
             period_scaling_factor=self.period_scaling_factor, time_scaling_factor=self.time_scaling_factor,
             client_manager_log_file="client_manager.log", client_manager_log_dir="/", client_manager_max_workers=10,
-            docker_gw_bridge_ip=self.docker_gw_bridge_ip, physical_host_ip=self.physical_host_ip
+            docker_gw_bridge_ip=self.docker_gw_bridge_ip, physical_host_ip=self.physical_host_ip,
+            breakpoints=self.breakpoints, breakvalues=self.breakvalues, exponents=self.exponents, factors=self.factors
         )
 
     def to_dict(self) -> Dict[str, Any]:
         """
         :return: a dict representation of the object
         """
         d = {}
@@ -100,14 +112,18 @@
         d["time_scaling_factor"] = self.time_scaling_factor
         d["period_scaling_factor"] = self.period_scaling_factor
         d["client_manager_log_file"] = self.client_manager_log_file
         d["client_manager_log_dir"] = self.client_manager_log_dir
         d["client_manager_max_workers"] = self.client_manager_max_workers
         d["docker_gw_bridge_ip"] = self.docker_gw_bridge_ip
         d["physical_host_ip"] = self.physical_host_ip
+        d["exponents"] = self.exponents
+        d["factors"] = self.factors
+        d["breakpoints"] = self.breakpoints
+        d["breakvalues"] = self.breakvalues
         return d
 
     def __str__(self) -> str:
         """
         :return: a string representation of the object
         """
         return f"ip:{self.ip}, client_population_process_type: {self.client_process_type}, lamb:{self.lamb}, " \
@@ -115,15 +131,17 @@
                f"client_manager_port: {self.client_manager_port}, num_commands:{self.num_commands}, " \
                f"client_time_step_len_seconds: {self.client_time_step_len_seconds}," \
                f"time_scaling_factor: {self.time_scaling_factor}, " \
                f"period_scaling_factor: {self.period_scaling_factor}," \
                f"client_manager_log_file: {self.client_manager_log_file}, " \
                f"client_manager_log_dir: {self.client_manager_log_dir}, " \
                f"client_manager_max_workers: {self.client_manager_max_workers}, " \
-               f"docker_gw_bridge_ip:{self.docker_gw_bridge_ip}, physical_host_ip: {self.physical_host_ip}"
+               f"docker_gw_bridge_ip:{self.docker_gw_bridge_ip}, physical_host_ip: {self.physical_host_ip}, " \
+               f"exponents: {self.exponents}, factors: {self.factors}, breakpoints: {self.breakpoints}, " \
+               f"breakvalues: {self.breakvalues}"
 
     def to_json_str(self) -> str:
         """
         Converts the DTO into a json string
 
         :return: the json string representation of the DTO
         """
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/cluster_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/cluster_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/cluster_node.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/cluster_node.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/connection_setup_dto.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/connection_setup_dto.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/container_network.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/container_network.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/containers_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/containers_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/credential.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/credential.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/default_network_firewall_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/default_network_firewall_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/docker_stats_manager_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/docker_stats_manager_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/docker_stats_managers_info.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/docker_stats_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/elk_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/elk_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/elk_managers_info.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/elk_managers_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     DTO containing the status of the ELK managers for a given emulation execution
     """
 
     def __init__(self, ips: List[str], ports: List[int],
                  emulation_name: str, execution_id: int,
                  elk_managers_statuses: List[csle_collector.elk_manager.elk_manager_pb2.ElkDTO],
                  elk_managers_running: List[bool], local_kibana_port: int = -1,
-                 physical_server_ip = ""):
+                 physical_server_ip=""):
         """
         Initializes the DTO
 
         :param elk_managers_running: boolean list that indicate whether the elk managers are running
         :param ips: the list of IPs of the running ELK managers
         :param ports: the list of ports of the running ELK managers
         :param emulation_name: the name of the corresponding emulation
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_env_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_env_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
 
     def get_hacker_connection(self) -> paramiko.SSHClient:
         """
         Gets an SSH connection to the hacker agent, creates one if it does not exist
 
         :return: SSH connection to the hacker
         """
-        hacker_ip = self.containers_config.agent_ip
+        hacker_ip = self.containers_config.get_agent_container().docker_gw_bridge_ip
         if hacker_ip in self.connections and self.connections[hacker_ip] is not None \
                 and self.connections[hacker_ip].get_transport() is not None \
                 and self.connections[hacker_ip].get_transport().is_active():
             try:
                 SSHUtil.execute_ssh_cmds(cmds=["ls > /dev/null"], conn=self.connections[hacker_ip])
             except Exception as e:
                 Logger.__call__().get_logger().info(f"Reconnecting attacker, {str(e), repr(e)}")
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_env_generation_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_env_generation_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_env_state.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_env_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,28 +123,30 @@
         """
         Utility function for extracting the attacker machine from the attacker's observation
 
         :param ip: the ip of the attacker machine
         :return: the machine if is found, otherwise None
         """
         for m in self.attacker_obs_state.machines:
-            if ip in m.ips:
-                return m
+            for m_ip in m.ips:
+                if m_ip == ip:
+                    return m
         return None
 
     def get_defender_machine(self, ip: str) -> Union[EmulationDefenderMachineObservationState, None]:
         """
         Utility function for extracting the defender machine from the defender's observation given an IP
 
         :param ip: the ip of the machine
         :return: the machine if found otherwise None
         """
         for m in self.defender_obs_state.machines:
-            if m.ips == ip:
-                return m
+            for m_ip in m.ips:
+                if m_ip == ip:
+                    return m
         return None
 
     def copy(self) -> "EmulationEnvState":
         """
         :return: a copy of the env state
         """
         copy = EmulationEnvState(emulation_env_config=self.emulation_env_config)
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_execution.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_execution.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_execution_info.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_execution_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_metrics_time_series.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_metrics_time_series.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import List, Dict, Any
 from csle_collector.snort_ids_manager.snort_ids_alert_counters import SnortIdsAlertCounters
+from csle_collector.snort_ids_manager.snort_ids_ip_alert_counters import SnortIdsIPAlertCounters
+from csle_collector.snort_ids_manager.snort_ids_rule_counters import SnortIdsRuleCounters
 from csle_collector.ossec_ids_manager.ossec_ids_alert_counters import OSSECIdsAlertCounters
 from csle_collector.client_manager.client_population_metrics import ClientPopulationMetrics
 from csle_collector.docker_stats_manager.docker_stats import DockerStats
 from csle_collector.host_manager.host_metrics import HostMetrics
 from csle_ryu.dao.avg_port_statistic import AvgPortStatistic
 from csle_ryu.dao.avg_flow_statistic import AvgFlowStatistic
 from csle_ryu.dao.flow_statistic import FlowStatistic
@@ -19,72 +21,83 @@
     DTO containing time series data from the emulation
     """
 
     def __init__(self, client_metrics: List[ClientPopulationMetrics], aggregated_docker_stats: List[DockerStats],
                  docker_host_stats: Dict[str, List[DockerStats]], host_metrics: Dict[str, List[HostMetrics]],
                  aggregated_host_metrics: List[HostMetrics],
                  defender_actions: List[EmulationDefenderAction], attacker_actions: List[EmulationAttackerAction],
-                 snort_ids_metrics: List[SnortIdsAlertCounters], emulation_env_config: EmulationEnvConfig,
+                 agg_snort_ids_metrics: List[SnortIdsAlertCounters], emulation_env_config: EmulationEnvConfig,
                  ossec_host_alert_counters: Dict[str, List[OSSECIdsAlertCounters]],
                  aggregated_ossec_host_alert_counters: List[OSSECIdsAlertCounters],
                  openflow_flow_stats: List[FlowStatistic], openflow_port_stats: List[PortStatistic],
                  avg_openflow_flow_stats: List[AvgFlowStatistic], avg_openflow_port_stats: List[AvgPortStatistic],
                  openflow_flow_metrics_per_switch: Dict[str, List[FlowStatistic]],
                  openflow_port_metrics_per_switch: Dict[str, List[PortStatistic]],
                  openflow_flow_avg_metrics_per_switch: Dict[str, List[AvgFlowStatistic]],
                  openflow_port_avg_metrics_per_switch: Dict[str, List[AvgPortStatistic]],
                  agg_openflow_flow_metrics_per_switch: Dict[str, List[AggFlowStatistic]],
-                 agg_openflow_flow_stats: List[AggFlowStatistic]
-                 ):
+                 agg_openflow_flow_stats: List[AggFlowStatistic],
+                 snort_ids_ip_metrics: Dict[str, List[SnortIdsIPAlertCounters]],
+                 agg_snort_ids_rule_metrics: List[SnortIdsRuleCounters],
+                 snort_alert_metrics_per_ids: Dict[str, List[SnortIdsAlertCounters]],
+                 snort_rule_metrics_per_ids: Dict[str, List[SnortIdsRuleCounters]]):
         """
         Initializes the DTO
 
         :param client_metrics: Time series data with information about the client population
         :param aggregated_docker_stats: Time series data with average docker statistics
         :param docker_host_stats: Time series data with docker statistics per host
         :param host_metrics: Time series data with general host metrics
         :param aggregated_host_metrics: Time series data with aggregated host metrics
         :param defender_actions: Time series data with defender actions
         :param attacker_actions: Time series data with attacker actions
-        :param snort_ids_metrics: Time series data with Snort IDS metrics
+        :param agg_snort_ids_metrics: Time series data with Snort IDS metrics
         :param emulation_env_config: the emulation config
         :param ossec_host_alert_counters: Time series data with ossec alert counters per host
         :param aggregated_ossec_host_alert_counters: Time series data with aggregated ossec alert counters
         :param openflow_flow_stats: openflow flow statistics
         :param openflow_port_stats: openflow port statistics
         :param avg_openflow_flow_stats: average openflow flow statistics per switch
         :param avg_openflow_port_stats: average openflow port statistics per switch
         :param openflow_flow_metrics_per_switch: openflow flow statistics per aggregated per switch
         :param openflow_port_metrics_per_switch: openflow port statistics per aggregated per switch
         :param openflow_flow_avg_metrics_per_switch: average openflow flow statistics per aggregated per switch
         :param openflow_port_avg_metrics_per_switch: average openflow port statistics per aggregated per switch
         :param agg_openflow_flow_stats: aggregated openflow flow statistics
         :param agg_openflow_flow_metrics_per_switch: aggregated openflow flow statistics aggregatd per switch
+        :param snort_ids_ip_metrics: Time series data with Snort IDS metrics per IP
+        :param agg_snort_ids_rule_metrics: Time series data with Snort IDS metrics per rule
+        :param snort_alert_metrics_per_ids: Time series data with Snort IDS alert metrics per IDS
+        :param snort_rule_metrics_per_ids: Time series data with Snort IDS rule metrics per IDS
         """
         self.client_metrics = client_metrics
         self.aggregated_docker_stats = aggregated_docker_stats
         self.docker_host_stats = docker_host_stats
         self.host_metrics = host_metrics
         self.defender_actions = defender_actions
         self.attacker_actions = attacker_actions
-        self.snort_ids_metrics = snort_ids_metrics
+        self.agg_snort_ids_metrics = agg_snort_ids_metrics
         self.aggregated_host_metrics = aggregated_host_metrics
         self.emulation_env_config = emulation_env_config
         self.ossec_host_alert_counters = ossec_host_alert_counters
         self.aggregated_ossec_host_alert_counters = aggregated_ossec_host_alert_counters
         self.openflow_flow_stats = openflow_flow_stats
         self.openflow_port_stats = openflow_port_stats
         self.avg_openflow_flow_stats = avg_openflow_flow_stats
         self.avg_openflow_port_stats = avg_openflow_port_stats
         self.openflow_flow_metrics_per_switch = openflow_flow_metrics_per_switch
         self.openflow_port_metrics_per_switch = openflow_port_metrics_per_switch
         self.openflow_flow_avg_metrics_per_switch = openflow_flow_avg_metrics_per_switch
         self.openflow_port_avg_metrics_per_switch = openflow_port_avg_metrics_per_switch
         self.agg_openflow_flow_stats = agg_openflow_flow_stats
         self.agg_openflow_flow_metrics_per_switch = agg_openflow_flow_metrics_per_switch
+        self.snort_ids_ip_metrics = snort_ids_ip_metrics
+        self.agg_snort_ids_rule_metrics = agg_snort_ids_rule_metrics
+        self.snort_alert_metrics_per_ids = snort_alert_metrics_per_ids
+        self.snort_rule_metrics_per_ids = snort_rule_metrics_per_ids
 
     @staticmethod
     def from_dict(d: Dict[str, Any]) -> "EmulationMetricsTimeSeries":
         """
         Converts a dict representation to an instance
 
         :param d: the dict to convert
@@ -116,37 +129,53 @@
         for k, v in d["openflow_port_avg_metrics_per_switch"].items():
             openflow_port_avg_metrics_per_switch[k] = list(map(lambda x: AvgPortStatistic.from_dict(x), v))
 
         agg_openflow_flow_metrics_per_switch = {}
         for k, v in d["agg_openflow_flow_metrics_per_switch"].items():
             agg_openflow_flow_metrics_per_switch[k] = list(map(lambda x: AggFlowStatistic.from_dict(x), v))
 
+        snort_ids_ip_metrics = {}
+        for k, v in d["snort_ids_ip_metrics"].items():
+            snort_ids_ip_metrics[k] = list(map(lambda x: SnortIdsIPAlertCounters.from_dict(x), v))
+
+        snort_alert_metrics_per_ids = {}
+        for k, v in d["snort_alert_metrics_per_ids"].items():
+            snort_alert_metrics_per_ids[k] = list(map(lambda x: SnortIdsAlertCounters.from_dict(x), v))
+
+        snort_rule_metrics_per_ids = {}
+        for k, v in d["snort_rule_metrics_per_ids"].items():
+            snort_rule_metrics_per_ids[k] = list(map(lambda x: SnortIdsRuleCounters.from_dict(x), v))
+
         obj = EmulationMetricsTimeSeries(
             client_metrics=list(map(lambda x: ClientPopulationMetrics.from_dict(x), d["client_metrics"])),
             aggregated_docker_stats=list(map(lambda x: DockerStats.from_dict(x), d["aggregated_docker_stats"])),
             docker_host_stats=docker_host_stats,
             host_metrics=host_metrics,
             defender_actions=list(map(lambda x: EmulationDefenderAction.from_dict(x), d["defender_actions"])),
             attacker_actions=list(map(lambda x: EmulationAttackerAction.from_dict(x), d["attacker_actions"])),
-            snort_ids_metrics=list(map(lambda x: SnortIdsAlertCounters.from_dict(x), d["snort_ids_metrics"])),
+            agg_snort_ids_metrics=list(map(lambda x: SnortIdsAlertCounters.from_dict(x), d["agg_snort_ids_metrics"])),
             aggregated_host_metrics=list(map(lambda x: HostMetrics.from_dict(x), d["aggregated_host_metrics"])),
             emulation_env_config=EmulationEnvConfig.from_dict(d["emulation_env_config"]),
             ossec_host_alert_counters=ossec_host_alerts,
             aggregated_ossec_host_alert_counters=d["aggregated_ossec_host_alert_counters"],
             openflow_flow_stats=list(map(lambda x: FlowStatistic.from_dict(x), d["openflow_flow_stats"])),
             openflow_port_stats=list(map(lambda x: PortStatistic.from_dict(x), d["openflow_port_stats"])),
             avg_openflow_flow_stats=list(map(lambda x: AvgFlowStatistic.from_dict(x), d["avg_openflow_flow_stats"])),
             avg_openflow_port_stats=list(map(lambda x: AvgPortStatistic.from_dict(x), d["avg_openflow_port_stats"])),
             openflow_flow_metrics_per_switch=openflow_flow_metrics_per_switch,
             openflow_port_metrics_per_switch=openflow_port_metrics_per_switch,
             openflow_flow_avg_metrics_per_switch=openflow_flow_avg_metrics_per_switch,
             openflow_port_avg_metrics_per_switch=openflow_port_avg_metrics_per_switch,
             agg_openflow_flow_stats=list(map(lambda x: AggFlowStatistic.from_dict(x), d["agg_openflow_flow_stats"])),
-            agg_openflow_flow_metrics_per_switch=agg_openflow_flow_metrics_per_switch
-        )
+            agg_openflow_flow_metrics_per_switch=agg_openflow_flow_metrics_per_switch,
+            snort_ids_ip_metrics=snort_ids_ip_metrics,
+            agg_snort_ids_rule_metrics=list(map(lambda x: SnortIdsRuleCounters.from_dict(x),
+                                                d["agg_snort_ids_rule_metrics"])),
+            snort_alert_metrics_per_ids=snort_alert_metrics_per_ids,
+            snort_rule_metrics_per_ids=snort_rule_metrics_per_ids)
         return obj
 
     def to_dict(self) -> Dict[str, Any]:
         """
         :return: a dict representation of the object
         """
         d = {}
@@ -156,15 +185,15 @@
         for k, v in self.docker_host_stats.items():
             d["docker_host_stats"][k] = list(map(lambda x: x.to_dict(), v))
         d["host_metrics"] = {}
         for k, v in self.host_metrics.items():
             d["host_metrics"][k] = list(map(lambda x: x.to_dict(), v))
         d["defender_actions"] = list(map(lambda x: x.to_dict(), self.defender_actions))
         d["attacker_actions"] = list(map(lambda x: x.to_dict(), self.attacker_actions))
-        d["snort_ids_metrics"] = list(map(lambda x: x.to_dict(), self.snort_ids_metrics))
+        d["agg_snort_ids_metrics"] = list(map(lambda x: x.to_dict(), self.agg_snort_ids_metrics))
         d["aggregated_host_metrics"] = list(map(lambda x: x.to_dict(), self.aggregated_host_metrics))
         d["emulation_env_config"] = self.emulation_env_config.to_dict()
         d["aggregated_ossec_host_alert_counters"] = list(map(lambda x: x.to_dict(),
                                                              self.aggregated_ossec_host_alert_counters))
         d["ossec_host_alert_counters"] = {}
         for k, v in self.ossec_host_alert_counters.items():
             d["ossec_host_alert_counters"][k] = list(map(lambda x: x.to_dict(), v))
@@ -190,40 +219,59 @@
             d["openflow_port_avg_metrics_per_switch"][k] = list(map(lambda x: x.to_dict(), v))
 
         d["agg_openflow_flow_metrics_per_switch"] = {}
         for k, v in self.agg_openflow_flow_metrics_per_switch.items():
             d["agg_openflow_flow_metrics_per_switch"][k] = list(map(lambda x: x.to_dict(), v))
 
         d["agg_openflow_flow_stats"] = list(map(lambda x: x.to_dict(), self.agg_openflow_flow_stats))
+
+        d["snort_ids_ip_metrics"] = {}
+        for k, v in self.snort_ids_ip_metrics.items():
+            d["snort_ids_ip_metrics"][k] = list(map(lambda x: x.to_dict(), v))
+
+        d["agg_snort_ids_rule_metrics"] = list(map(lambda x: x.to_dict(), self.agg_snort_ids_rule_metrics))
+
+        d["snort_alert_metrics_per_ids"] = {}
+        for k, v in self.snort_alert_metrics_per_ids.items():
+            d["snort_alert_metrics_per_ids"][k] = list(map(lambda x: x.to_dict(), v))
+
+        d["snort_rule_metrics_per_ids"] = {}
+        for k, v in self.snort_rule_metrics_per_ids.items():
+            d["snort_rule_metrics_per_ids"][k] = list(map(lambda x: x.to_dict(), v))
+
         return d
 
     def __str__(self) -> str:
         """
         :return: a string representation
         """
         return f"client_metrics: {list(map(lambda x: str(x), self.client_metrics))}," \
                f"aggregated_docker_stats: {list(map(lambda x: str(x), self.aggregated_docker_stats))}," \
                f"docker_host_stats: {list(map(lambda x: str(x), self.docker_host_stats))}," \
                f"host_metrics: {list(map(lambda x: str(x), self.host_metrics))}," \
                f"defender_actions: {list(map(lambda x: str(x), self.defender_actions))}," \
                f"attacker_actions: {list(map(lambda x: str(x), self.attacker_actions))}," \
-               f"snort_ids_metrics: {list(map(lambda x: str(x), self.snort_ids_metrics))}," \
+               f"agg_snort_ids_metrics: {list(map(lambda x: str(x), self.agg_snort_ids_metrics))}," \
                f"aggregated_host_metrics: {list(map(lambda x: str(x), self.aggregated_host_metrics))}," \
                f"config: {self.emulation_env_config}," \
                f"aggregated_ossec_host_alert_counters: {self.aggregated_ossec_host_alert_counters}," \
                f"ossec_host_alert_counters: {self.ossec_host_alert_counters}," \
                f"openflow_flow_stats: {self.openflow_flow_stats}, openflow_port_stats: {self.openflow_port_stats}," \
                f"avg_openflow_flow_stats: {self.avg_openflow_flow_stats}, " \
                f"avg_openflow_port_stats: {self.avg_openflow_port_stats}," \
                f"openflow_flow_metrics_per_switch: {self.openflow_flow_metrics_per_switch}," \
                f"openflow_port_metrics_per_switch: {self.openflow_port_metrics_per_switch}," \
                f"openflow_flow_avg_metrics_per_switch: {self.openflow_flow_avg_metrics_per_switch}," \
                f"openflow_port_avg_metrics_per_switch: {self.openflow_port_avg_metrics_per_switch}," \
                f"agg_openflow_flow_stats: {self.agg_openflow_flow_stats}," \
-               f"agg_openflow_flow_metrics_per_switch: {self.agg_openflow_flow_metrics_per_switch}"
+               f"agg_openflow_flow_metrics_per_switch: {self.agg_openflow_flow_metrics_per_switch}," \
+               f"snort_ids_ip_metrics: {self.snort_ids_ip_metrics}," \
+               f"agg_snort_ids_rule_metrics: {self.agg_snort_ids_rule_metrics}," \
+               f"snort_alert_metrics_per_ids: {self.snort_alert_metrics_per_ids}," \
+               f"snort_rule_metrics_per_ids: {self.snort_rule_metrics_per_ids}"
 
     def to_json_str(self) -> str:
         """
         Converts the DTO into a json string
 
         :return: the json string representation of the DTO
         """
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_simulation_trace.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_simulation_trace.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_statistics_windowed.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_statistics_windowed.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_trace.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/emulation_trace.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/flag.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/flag.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/flags_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/flags_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/host_manager_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/host_manager_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/host_managers_info.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/host_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/kafka_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/kafka_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/kafka_managers_info.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/kafka_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/kafka_topic.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/network_service.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/network_service.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_beats_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_beats_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_container_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_container_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_firewall_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_firewall_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Set, List, Dict, Any
+from typing import Set, List, Dict, Any, Tuple
 from csle_common.dao.emulation_config.default_network_firewall_config import DefaultNetworkFirewallConfig
 from csle_common.util.general_util import GeneralUtil
 
 
 class NodeFirewallConfig:
     """
     A DTO object representing a firewall configuration of a container in an emulation environment
     """
 
     def __init__(self, ips_gw_default_policy_networks: List[DefaultNetworkFirewallConfig],
                  hostname: str, output_accept: Set[str], input_accept: Set[str],
                  forward_accept: Set[str], output_drop: Set[str], input_drop: Set[str],
-                 forward_drop: Set[str], routes: Set[str], docker_gw_bridge_ip: str = "",
+                 forward_drop: Set[str], routes: Set[Tuple[str, str]], docker_gw_bridge_ip: str = "",
                  physical_host_ip: str = ""):
         """
         Initializes the DTO
 
         :param ips_gw_default_policy_networks: List of ip,gw,default policy, network
         :param ip: the ip of the node
         :param hostname: the hostname of the node
@@ -61,15 +61,15 @@
                                                     d["ips_gw_default_policy_networks"])),
             output_accept=set(d["output_accept"]),
             input_accept=set(d["input_accept"]),
             forward_accept=set(d["forward_accept"]),
             output_drop=set(d["output_drop"]),
             input_drop=set(d["input_drop"]),
             forward_drop=set(d["forward_drop"]),
-            routes=set(d["routes"]),
+            routes=set(list(map(lambda x: tuple(x), d["routes"]))),
             docker_gw_bridge_ip=d["docker_gw_bridge_ip"],
             physical_host_ip=d["physical_host_ip"]
         )
         return obj
 
     def to_dict(self) -> Dict[str, Any]:
         """
@@ -166,16 +166,16 @@
         config.input_drop = set(list(map(
             lambda x: GeneralUtil.replace_first_octet_of_ip(
                 ip=x, ip_first_octet=ip_first_octet), list(config.input_drop))))
         config.forward_drop = set(list(map(
             lambda x: GeneralUtil.replace_first_octet_of_ip(
                 ip=x, ip_first_octet=ip_first_octet), list(config.forward_drop))))
         config.routes = set(list(map(
-            lambda x: GeneralUtil.replace_first_octet_of_ip(
-                ip=x, ip_first_octet=ip_first_octet), list(config.routes))))
+            lambda x: GeneralUtil.replace_first_octet_of_ip_tuple(
+                tuple_of_ips=x, ip_first_octet=ip_first_octet), list(config.routes))))
         config.ips_gw_default_policy_networks = list(map(lambda x: x.create_execution_config(
             ip_first_octet=ip_first_octet), config.ips_gw_default_policy_networks))
         return config
 
     @staticmethod
     def schema() -> "NodeFirewallConfig":
         """
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_flags_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_flags_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_network_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_network_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_resources_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_resources_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_services_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_services_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_traffic_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_traffic_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_users_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_users_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_vulnerability_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/node_vulnerability_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/ossec_ids_manager_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/ossec_ids_manager_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/ossec_managers_info.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/ossec_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/ovs_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/ovs_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,10 +88,9 @@
 
         :param ip_first_octet: the first octet of the IP of the new execution
         :param physical_servers: the list of physical servers of the execution
         :return: the new config
         """
         config = self.copy()
         config.switch_configs = list(map(lambda x: x.create_execution_config(
-            ip_first_octet=ip_first_octet, physical_servers=physical_servers),
-                                         config.switch_configs))
+            ip_first_octet=ip_first_octet, physical_servers=physical_servers), config.switch_configs))
         return config
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/ovs_switch_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/ovs_switch_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/resources_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/resources_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/ryu_managers_info.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/ryu_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/sdn_controller_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/sdn_controller_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/services_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/services_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/snort_ids_manager_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/snort_ids_manager_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/snort_managers_info.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/snort_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/topology_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/topology_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/traffic_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/traffic_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/traffic_managers_info.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/traffic_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/transport_protocol.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/transport_protocol.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/user.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/user.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/users_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/users_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_config/vulnerabilities_config.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_config/vulnerabilities_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_machine_observation_state.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_machine_observation_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         m_copy.cve_2010_0426_tried = self.cve_2010_0426_tried
         m_copy.cve_2015_5602_tried = self.cve_2015_5602_tried
         return m_copy
 
     @staticmethod
     def from_nmap_result(nmap_host_result: NmapHostResult) -> "EmulationAttackerMachineObservationState":
         """
-        Converts the NmapHostResultDTO into a a AttackerMachineObservationState
+        Converts the NmapHostResultDTO into a AttackerMachineObservationState
 
         :return: the created AttackerMachineObservationState
         """
         m_obs = EmulationAttackerMachineObservationState(ips=nmap_host_result.ips)
         ports = list(map(lambda x: x.to_obs(), nmap_host_result.ports))
         m_obs.ports = ports
         if nmap_host_result.os is not None:
@@ -236,14 +236,16 @@
 
         :param ips: the list of ips to check
         :return:  True if they match, False otherwise
         """
         for ip in self.ips:
             if ip in ips:
                 return True
+            if ip.split(".")[-1] in list(map(lambda x: x.split(".")[-1], ips)):
+                return True
         return False
 
     @staticmethod
     def from_dict(d: Dict[str, Any]) -> "EmulationAttackerMachineObservationState":
         """
         Converts a dict representation to an instance
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_observation_state.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_observation_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_observation/common/emulation_connection_observation_state.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_observation/common/emulation_connection_observation_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_observation/common/emulation_port_observation_state.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_observation/common/emulation_port_observation_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_observation/common/emulation_vulnerability_observation_state.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_observation/common/emulation_vulnerability_observation_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_observation/defender/emulation_defender_machine_observation_state.py` & `csle_common-0.2.0/src/csle_common/dao/training/dqn_policy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,161 +1,167 @@
-from typing import List, Dict, Any
-from csle_common.dao.emulation_observation.common.emulation_port_observation_state \
-    import EmulationPortObservationState
-from csle_common.dao.emulation_observation.common.emulation_connection_observation_state \
-    import EmulationConnectionObservationState
-from csle_common.dao.emulation_config.node_container_config import NodeContainerConfig
-from csle_common.consumer_threads.host_metrics_consumer_thread import HostMetricsConsumerThread
-from csle_common.consumer_threads.docker_host_stats_consumer_thread import DockerHostStatsConsumerThread
-from csle_common.dao.emulation_config.kafka_config import KafkaConfig
-from csle_collector.host_manager.host_metrics import HostMetrics
-from csle_collector.docker_stats_manager.docker_stats import DockerStats
+from typing import List, Dict, Union
+import numpy as np
+import torch
+from stable_baselines3 import DQN
+from csle_common.dao.training.policy import Policy
+from csle_common.dao.training.agent_type import AgentType
+from csle_common.dao.training.player_type import PlayerType
+from csle_common.dao.simulation_config.state import State
+from csle_common.dao.simulation_config.state_type import StateType
+from csle_common.dao.simulation_config.action import Action
+from csle_common.dao.training.experiment_config import ExperimentConfig
+from csle_common.dao.training.policy_type import PolicyType
+from csle_common.logging.log import Logger
 
 
-class EmulationDefenderMachineObservationState:
+class DQNPolicy(Policy):
     """
-    Represents the defender's belief state of a component in the emulation
+    A neural network policy learned with DQN
     """
 
-    def __init__(self, ips: List[str], kafka_config: KafkaConfig,
-                 host_metrics: HostMetrics = None, docker_stats: DockerStats = None):
+    def __init__(self, model, simulation_name: str, save_path: str, player_type: PlayerType, states: List[State],
+                 actions: List[Action], experiment_config: ExperimentConfig, avg_R: float):
         """
-        Initializes the DTO
+        Initializes the policy
 
-        :param ips: the ip of the machine
-        :param kafka_config: the kafka config
-        :param host_metrics: the host metrics object
-        :param docker_stats: the docker stats object
-        """
-        self.ips = ips
-        self.os = "unknown"
-        self.ports: List[EmulationPortObservationState] = []
-        self.ssh_connections: List[EmulationConnectionObservationState] = []
-        self.kafka_config = kafka_config
-        self.host_metrics = host_metrics
-        if self.host_metrics is None:
-            self.host_metrics = HostMetrics()
-        self.docker_stats = docker_stats
-        if self.docker_stats is None:
-            self.docker_stats = DockerStats()
-        self.host_metrics_consumer_thread = None
-        self.docker_stats_consumer_thread = None
+        :param model: the DQN model
+        :param simulation_name: the simulation name
+        :param save_path: the path to save the model to
+        :param states: list of states (required for computing stage policies)
+        :param actions: list of actions
+        :param experiment_config: the experiment configuration for training the policy
+        :param avg_R: the average reward of the policy when evaluated in the simulation
+        """
+        super(DQNPolicy, self).__init__(agent_type=AgentType.DQN, player_type=player_type)
+        self.model = model
+        self.id = -1
+        self.simulation_name = simulation_name
+        self.save_path = save_path
+        if self.model is None:
+            try:
+                self.model = DQN.load(path=self.save_path)
+            except Exception as e:
+                Logger.__call__().get_logger().warning(
+                    f"There was an exception loading the model from path: {self.save_path}, "
+                    f"exception: {str(e)}, {repr(e)}")
+        self.states = states
+        self.actions = actions
+        self.experiment_config = experiment_config
+        self.avg_R = avg_R
+        self.policy_type = PolicyType.DQN
+
+    def action(self, o: List[float]) -> Union[int, List[int], np.ndarray]:
+        """
+        Multi-threshold stopping policy
+
+        :param o: the current observation
+        :return: the selected action
+        """
+        a, _ = self.model.predict(np.array(o), deterministic=False)
+        return a
+
+    def probability(self, o: List[float], a) -> Union[int, List[int], np.ndarray]:
+        """
+        Multi-threshold stopping policy
+
+        :param o: the current observation
+        :return: the selected action
+        """
+        actions = self.model.policy.forward(obs=torch.tensor(o).to(self.model.device))
+        action = actions[0]
+        if action == a:
+            return 1
+        else:
+            return 0
 
-    def start_monitor_threads(self) -> None:
+    def to_dict(self) -> Dict[str, Union[float, int, str]]:
         """
-        Starts the monitoring threads
-
-        :return: None
+        :return: a dict representation of the policy
         """
-        self.host_metrics_consumer_thread = HostMetricsConsumerThread(
-            host_ip=self.ips[0], kafka_server_ip=self.kafka_config.container.get_ips()[0],
-            kafka_port=self.kafka_config.kafka_port, host_metrics=self.host_metrics)
-        self.docker_stats_consumer_thread = DockerHostStatsConsumerThread(
-            host_ip=self.ips[0], kafka_server_ip=self.kafka_config.container.get_ips()[0],
-            kafka_port=self.kafka_config.kafka_port, docker_stats=self.docker_stats)
-        self.host_metrics_consumer_thread.start()
-        self.docker_stats_consumer_thread.start()
+        d = {}
+        d["id"] = self.id
+        d["simulation_name"] = self.simulation_name
+        d["save_path"] = self.save_path
+        if self.model is not None:
+            d["policy_kwargs"] = self.model.policy_kwargs
+            self.model.save(path=self.save_path)
+        else:
+            d["policy_kwargs"] = {}
+            d["policy_kwargs"]["net_arch"] = []
+        d["states"] = list(map(lambda x: x.to_dict(), self.states))
+        d["player_type"] = self.player_type
+        d["actions"] = list(map(lambda x: x.to_dict(), self.actions))
+        d["experiment_config"] = self.experiment_config.to_dict()
+        d["agent_type"] = self.agent_type
+        d["avg_R"] = self.avg_R
+        d["policy_type"] = self.policy_type
+        return d
 
     @staticmethod
-    def from_container(container: NodeContainerConfig, kafka_config: KafkaConfig):
+    def from_dict(d: Dict) -> "DQNPolicy":
         """
-        Creates an instance from a container configuration
+        Converst a dict representation of the object to an instance
 
-        :param container: the container to create the instance from
-        :param kafka_config: the kafka config
+        :param d: the dict to convert
         :return: the created instance
         """
-        obj = EmulationDefenderMachineObservationState(ips=container.get_ips(), kafka_config=kafka_config,
-                                                       host_metrics=None, docker_stats=None)
-        obj.os = container.os
+        obj = DQNPolicy(model=None, simulation_name=d["simulation_name"], save_path=d["save_path"],
+                        states=list(map(lambda x: State.from_dict(x), d["states"])), player_type=d["player_type"],
+                        actions=list(map(lambda x: Action.from_dict(x), d["actions"])),
+                        experiment_config=ExperimentConfig.from_dict(d["experiment_config"]), avg_R=d["avg_R"])
+        obj.id = d["id"]
         return obj
 
-    @staticmethod
-    def from_dict(d: Dict[str, Any]) -> "EmulationDefenderMachineObservationState":
+    def stage_policy(self, o: Union[List[Union[int, float]], int, float]) -> List[List[float]]:
         """
-        Converts a dict representation of the object to an instance
+        Gets the stage policy, i.e a |S|x|A| policy
 
-        :param d: the dict representation
-        :return: the object instance
+        :param o: the latest observation
+        :return: the |S|x|A| stage policy
         """
-        if "kafka_config" in d and d["kafka_config"] is not None:
-            kafka_config = KafkaConfig.from_dict(d["kafka_config"])
+        b1 = o[1]
+        l = int(o[0])
+        if not self.player_type == PlayerType.ATTACKER:
+            stage_policy = []
+            for _ in self.states:
+                stage_policy.append(self._get_attacker_stopping_dist(obs=o))
+            return stage_policy
         else:
-            kafka_config = None
-        obj = EmulationDefenderMachineObservationState(
-            ips=d["ips"], kafka_config=kafka_config,
-            host_metrics=HostMetrics.from_dict(d["host_metrics"]),
-            docker_stats=DockerStats.from_dict(d["docker_stats"]))
-        obj.os = d["os"]
-        obj.ports = list(map(lambda x: EmulationPortObservationState.from_dict(x), d["ports"]))
-        obj.ssh_connections = list(map(lambda x: EmulationConnectionObservationState.from_dict(x),
-                                       d["ssh_connections"]))
-        return obj
-
-    def to_dict(self) -> Dict[str, Any]:
-        """
-        :return: a dict representation of the object
-        """
-        d = {}
-        d["ips"] = self.ips
-        d["os"] = self.os
-        d["ports"] = list(map(lambda x: x.to_dict(), self.ports))
-        d["ssh_connections"] = list(map(lambda x: x.to_dict(), self.ssh_connections))
-        d["host_metrics"] = self.host_metrics.to_dict()
-        d["docker_stats"] = self.docker_stats.to_dict()
-        if self.kafka_config is not None:
-            d["kafka_config"] = self.kafka_config.to_dict()
+            stage_policy = []
+            for s in self.states:
+                if s.state_type != StateType.TERMINAL:
+                    o = [l, b1, s.id]
+                    stage_policy.append(self._get_attacker_stopping_dist(obs=o))
+                else:
+                    stage_policy.append([0.5, 0.5])
+            return stage_policy
+
+    def _get_attacker_stopping_dist(self, obs) -> List[float]:
+        """
+        Utility function for getting the stopping action distribution conditioned on a given observation
+
+        :param obs: the observation to condition on
+        :return: the conditional ation distribution
+        """
+        obs = np.array([obs])
+        actions = self.model.policy.forward(obs=torch.tensor(obs).to(self.model.device))
+        action = actions[0]
+        if action == 1:
+            stop_prob = 1
         else:
-            d["kafka_config"] = None
-        return d
+            stop_prob = 0
+        return [1 - stop_prob, stop_prob]
 
     def __str__(self) -> str:
         """
         :return: a string representation of the object
         """
-        return f"ips:{self.ips}, os:{self.os}, ports: {list(map(lambda x: str(x), self.ports))}, " \
-               f"ssh_connections: {list(map(lambda x: str(x), self.ssh_connections))}, " \
-               f"host_metrics: {self.host_metrics}, docker_stats: {self.docker_stats}"
-
-    def sort_ports(self) -> None:
-        """
-        Sorts the list of ports
-
-        :return: None
-        """
-        for p in self.ports:
-            p.port = int(p.port)
-        self.ports = sorted(self.ports, key=lambda x: x.kafka_port, reverse=False)
-
-    def cleanup(self) -> None:
-        """
-        Cleans up environment state. This method is particularly useful in emulation mode where there are
-        SSH/Telnet/FTP... connections that should be cleaned up, as well as background threads.
-
-        :return: None
-        """
-        if self.docker_stats_consumer_thread is not None:
-            self.docker_stats_consumer_thread.running = False
-            self.docker_stats_consumer_thread.consumer.close()
-        for c in self.ssh_connections:
-            c.cleanup()
-
-    def copy(self) -> "EmulationDefenderMachineObservationState":
-        """
-        :return: a copy of the object
-        """
-        m_copy = EmulationDefenderMachineObservationState(
-            ips=self.ips, kafka_config=self.kafka_config, host_metrics=self.host_metrics.copy(),
-            docker_stats=self.docker_stats.copy())
-        m_copy.os = self.os
-        m_copy.ports = list(map(lambda x: x.copy(), self.ports))
-        m_copy.ssh_connections = self.ssh_connections
-        m_copy.host_metrics = self.host_metrics.copy()
-        m_copy.docker_stats = self.docker_stats.copy()
-        return m_copy
+        return f"model: {self.model}, id: {self.id}, simulation_name: {self.simulation_name}, " \
+               f"save path: {self.save_path}, states: {self.states}, experiment_config: {self.experiment_config}," \
+               f"avg_R: {self.avg_R}, policy_type: {self.policy_type}"
 
     def to_json_str(self) -> str:
         """
         Converts the DTO into a json string
 
         :return: the json string representation of the DTO
         """
@@ -172,43 +178,25 @@
         """
         import io
         json_str = self.to_json_str()
         with io.open(json_file_path, 'w', encoding='utf-8') as f:
             f.write(json_str)
 
     @staticmethod
-    def from_json_file(json_file_path: str) -> "EmulationDefenderMachineObservationState":
+    def from_json_file(json_file_path: str) -> "DQNPolicy":
         """
         Reads a json file and converts it to a DTO
 
         :param json_file_path: the json file path
         :return: the converted DTO
         """
         import io
         import json
         with io.open(json_file_path, 'r') as f:
             json_str = f.read()
-        return EmulationDefenderMachineObservationState.from_dict(json.loads(json_str))
-
-    def num_attributes(self) -> int:
-        """
-        :return: The number of attribute of the DTO
-        """
-        num_attributes = 2
-        if self.host_metrics is not None:
-            num_attributes = num_attributes + self.host_metrics.num_attributes()
-        if self.docker_stats is not None:
-            num_attributes = num_attributes + self.docker_stats.num_attributes()
-        if len(self.ports) > 0:
-            num_attributes = num_attributes + len(self.ports) * self.ports[0].num_attributes()
-        if len(self.ssh_connections) > 0:
-            num_attributes = num_attributes + len(self.ports) * self.ssh_connections[0].num_attributes()
-        return num_attributes
+        return DQNPolicy.from_dict(json.loads(json_str))
 
-    @staticmethod
-    def schema() -> "EmulationDefenderMachineObservationState":
+    def copy(self) -> "DQNPolicy":
         """
-        :return: get the schema of the DTO
+        :return: a copy of the DTO
         """
-        return EmulationDefenderMachineObservationState(ips=[""], kafka_config=KafkaConfig.schema(),
-                                                        host_metrics=HostMetrics.schema(),
-                                                        docker_stats=DockerStats.schema())
+        return self.from_dict(self.to_dict())
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/emulation_observation/defender/emulation_defender_observation_state.py` & `csle_common-0.2.0/src/csle_common/dao/emulation_observation/defender/emulation_defender_observation_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
 from csle_common.dao.emulation_observation.defender.emulation_defender_machine_observation_state \
     import EmulationDefenderMachineObservationState
 from csle_common.dao.emulation_action.defender.emulation_defender_action import EmulationDefenderAction
 from csle_common.dao.emulation_action.attacker.emulation_attacker_action import EmulationAttackerAction
 from csle_common.dao.emulation_config.kafka_config import KafkaConfig
 from csle_common.consumer_threads.docker_stats_consumer_thread import DockerStatsConsumerThread
-from csle_common.consumer_threads.snort_ids_log_consumer_thread import SnortIdsLogConsumerThread
-from csle_common.consumer_threads.ossec_ids_log_consumer_thread import OSSECIdsLogConsumerThread
+from csle_common.consumer_threads.aggregated_snort_ids_log_consumer_thread import AggregatedSnortIdsLogConsumerThread
+from csle_common.consumer_threads.aggregated_ossec_ids_log_consumer_thread import AggregatedOSSECIdsLogConsumerThread
+from csle_common.consumer_threads.aggregated_snort_ids_rule_log_consumer_thread \
+    import AggregatedSnortIdsRuleLogConsumerThread
 from csle_common.consumer_threads.client_population_consumer_thread import ClientPopulationConsumerThread
 from csle_common.consumer_threads.attacker_actions_consumer_thread import AttackerActionsConsumerThread
 from csle_common.consumer_threads.defender_actions_consumer_thread import DefenderActionsConsumerThread
 from csle_common.consumer_threads.aggregated_host_metrics_thread import AggregatedHostMetricsThread
 from csle_collector.client_manager.client_population_metrics import ClientPopulationMetrics
 from csle_collector.docker_stats_manager.docker_stats import DockerStats
 from csle_collector.snort_ids_manager.snort_ids_alert_counters import SnortIdsAlertCounters
+from csle_collector.snort_ids_manager.snort_ids_rule_counters import SnortIdsRuleCounters
 from csle_collector.ossec_ids_manager.ossec_ids_alert_counters import OSSECIdsAlertCounters
 from csle_collector.host_manager.host_metrics import HostMetrics
 
 
 class EmulationDefenderObservationState:
     """
     Represents the defender's agent's current belief state of the emulation
@@ -26,26 +29,29 @@
 
     def __init__(self, kafka_config: Union[KafkaConfig, None],
                  client_population_metrics: ClientPopulationMetrics = None, docker_stats: DockerStats = None,
                  snort_ids_alert_counters: SnortIdsAlertCounters = None,
                  ossec_ids_alert_counters: OSSECIdsAlertCounters = None,
                  aggregated_host_metrics: HostMetrics = None,
                  defender_actions: List[EmulationDefenderAction] = None,
-                 attacker_actions: List[EmulationAttackerAction] = None):
+                 attacker_actions: List[EmulationAttackerAction] = None,
+                 snort_ids_rule_counters: SnortIdsRuleCounters = None
+                 ):
         """
         Initializes the DTO
 
         :param kafka_config: the kafka config
         :param client_population_metrics: the client population metrics
         :param docker_stats: the docker stats
         :param snort_ids_alert_counters: the snort ids alert counters
         :param ossec_ids_alert_counters: the ossec ids alert counters
         :param defender_actions: the list of defender actions
         :param attacker_actions: the list of attacker actions
         :param aggregated_host_metrics: the aggregated host metrics
+        :param snort_ids_rule_counters: the aggregated snort IDS rule counters
         """
         self.kafka_config = kafka_config
         self.machines: List[EmulationDefenderMachineObservationState] = []
         self.actions_tried = set()
         self.client_population_metrics = client_population_metrics
         if self.client_population_metrics is None:
             self.client_population_metrics = ClientPopulationMetrics()
@@ -54,14 +60,18 @@
         if self.docker_stats is None:
             self.docker_stats = DockerStats()
         self.avg_docker_stats = self.docker_stats.copy()
         self.snort_ids_alert_counters = snort_ids_alert_counters
         if self.snort_ids_alert_counters is None:
             self.snort_ids_alert_counters = SnortIdsAlertCounters()
         self.avg_snort_ids_alert_counters = self.snort_ids_alert_counters.copy()
+        self.snort_ids_rule_counters = snort_ids_rule_counters
+        if self.snort_ids_rule_counters is None:
+            self.snort_ids_rule_counters = SnortIdsRuleCounters()
+        self.avg_snort_ids_rule_counters = self.snort_ids_rule_counters.copy()
         self.ossec_ids_alert_counters = ossec_ids_alert_counters
         if self.ossec_ids_alert_counters is None:
             self.ossec_ids_alert_counters = OSSECIdsAlertCounters()
         self.avg_ossec_ids_alert_counters = self.ossec_ids_alert_counters.copy()
         self.attacker_actions = attacker_actions
         if self.attacker_actions is None:
             self.attacker_actions = []
@@ -70,16 +80,17 @@
             self.defender_actions = []
         self.aggregated_host_metrics = aggregated_host_metrics
         if aggregated_host_metrics is None:
             self.aggregated_host_metrics = HostMetrics()
         self.avg_aggregated_host_metrics = self.aggregated_host_metrics.copy()
         self.docker_stats_consumer_thread = None
         self.client_population_consumer_thread = None
-        self.snort_ids_log_consumer_thread = None
-        self.ossec_ids_log_consumer_thread = None
+        self.aggregated_snort_ids_log_consumer_thread = None
+        self.aggregated_snort_ids_rule_log_consumer_thread = None
+        self.aggregated_ossec_ids_log_consumer_thread = None
         self.attacker_actions_consumer_thread = None
         self.defender_actions_consumer_thread = None
         self.aggregated_host_metrics_thread = None
 
     def start_monitoring_threads(self) -> None:
         """
         Starts the avg host metrics thread
@@ -88,102 +99,112 @@
         """
         self.aggregated_host_metrics_thread = AggregatedHostMetricsThread(
             host_metrics=self.aggregated_host_metrics,
             sleep_time=self.kafka_config.time_step_len_seconds,
             machines=self.machines
         )
         self.docker_stats_consumer_thread = DockerStatsConsumerThread(
-            kafka_server_ip=self.kafka_config.container.get_ips()[0],
-            kafka_port=self.kafka_config.kafka_port,
+            kafka_server_ip=self.kafka_config.container.docker_gw_bridge_ip,
+            kafka_port=self.kafka_config.kafka_port_external,
             docker_stats=self.docker_stats)
         self.client_population_consumer_thread = ClientPopulationConsumerThread(
-            kafka_server_ip=self.kafka_config.container.get_ips()[0],
-            kafka_port=self.kafka_config.kafka_port,
+            kafka_server_ip=self.kafka_config.container.docker_gw_bridge_ip,
+            kafka_port=self.kafka_config.kafka_port_external,
             client_population_metrics=self.client_population_metrics
         )
-        self.snort_ids_log_consumer_thread = SnortIdsLogConsumerThread(
-            kafka_server_ip=self.kafka_config.container.get_ips()[0],
-            kafka_port=self.kafka_config.kafka_port,
+        self.aggregated_snort_ids_log_consumer_thread = AggregatedSnortIdsLogConsumerThread(
+            kafka_server_ip=self.kafka_config.container.docker_gw_bridge_ip,
+            kafka_port=self.kafka_config.kafka_port_external,
             snort_ids_alert_counters=self.snort_ids_alert_counters
         )
-        self.ossec_ids_log_consumer_thread = OSSECIdsLogConsumerThread(
-            kafka_server_ip=self.kafka_config.container.get_ips()[0],
-            kafka_port=self.kafka_config.kafka_port,
+        self.aggregated_snort_ids_rule_log_consumer_thread = AggregatedSnortIdsRuleLogConsumerThread(
+            kafka_server_ip=self.kafka_config.container.docker_gw_bridge_ip,
+            kafka_port=self.kafka_config.kafka_port_external,
+            snort_ids_rule_counters=self.snort_ids_rule_counters
+        )
+        self.aggregated_ossec_ids_log_consumer_thread = AggregatedOSSECIdsLogConsumerThread(
+            kafka_server_ip=self.kafka_config.container.docker_gw_bridge_ip,
+            kafka_port=self.kafka_config.kafka_port_external,
             ossec_ids_alert_counters=self.ossec_ids_alert_counters
         )
         self.attacker_actions_consumer_thread = AttackerActionsConsumerThread(
-            kafka_server_ip=self.kafka_config.container.get_ips()[0],
-            kafka_port=self.kafka_config.kafka_port,
+            kafka_server_ip=self.kafka_config.container.docker_gw_bridge_ip,
+            kafka_port=self.kafka_config.kafka_port_external,
             attacker_actions=self.attacker_actions
         )
         self.defender_actions_consumer_thread = DefenderActionsConsumerThread(
-            kafka_server_ip=self.kafka_config.container.get_ips()[0],
-            kafka_port=self.kafka_config.kafka_port,
+            kafka_server_ip=self.kafka_config.container.docker_gw_bridge_ip,
+            kafka_port=self.kafka_config.kafka_port_external,
             defender_actions=self.defender_actions
         )
         self.aggregated_host_metrics_thread.start()
         self.docker_stats_consumer_thread.start()
         self.client_population_consumer_thread.start()
-        self.snort_ids_log_consumer_thread.start()
-        self.ossec_ids_log_consumer_thread.start()
+        self.aggregated_snort_ids_log_consumer_thread.start()
+        self.aggregated_snort_ids_rule_log_consumer_thread.start()
+        self.aggregated_ossec_ids_log_consumer_thread.start()
         self.attacker_actions_consumer_thread.start()
         self.defender_actions_consumer_thread.start()
         for m in self.machines:
             m.start_monitor_threads()
 
     @staticmethod
     def from_dict(d: Dict[str, Any]) -> "EmulationDefenderObservationState":
         """
         Converts a dict representation of the object to an instance
 
         :param d: the dict to convert
         :return: the created instance
         """
         try:
-            obj = EmulationDefenderObservationState(kafka_config=d["kafka_config"])
+            obj = EmulationDefenderObservationState(kafka_config=KafkaConfig.from_dict(d["kafka_config"]))
         except Exception:
             obj = EmulationDefenderObservationState(kafka_config=None)
         obj.machines = list(map(lambda x: EmulationDefenderMachineObservationState.from_dict(d=x), d["machines"]))
         obj.actions_tried = set(list(map(lambda x: tuple(x), d["actions_tried"])))
         obj.client_population_metrics = ClientPopulationMetrics.from_dict(d["client_population_metrics"])
         obj.docker_stats = DockerStats.from_dict(d["docker_stats"])
         obj.snort_ids_alert_counters = SnortIdsAlertCounters.from_dict(d["snort_ids_alert_counters"])
+        obj.snort_ids_rule_counters = SnortIdsRuleCounters.from_dict(d["snort_ids_rule_counters"])
         obj.ossec_ids_alert_counters = OSSECIdsAlertCounters.from_dict(d["ossec_ids_alert_counters"])
         obj.aggregated_host_metrics = HostMetrics.from_dict(d["aggregated_host_metrics"])
         obj.attacker_actions = list(map(lambda x: EmulationAttackerAction.from_dict(x), d["attacker_actions"]))
         obj.defender_actions = list(map(lambda x: EmulationDefenderAction.from_dict(x), d["defender_actions"]))
         obj.avg_aggregated_host_metrics = HostMetrics.from_dict(d["avg_aggregated_host_metrics"])
         obj.avg_docker_stats = DockerStats.from_dict(d["avg_docker_stats"])
         obj.avg_client_population_metrics = ClientPopulationMetrics.from_dict(d["avg_client_population_metrics"])
         obj.avg_snort_ids_alert_counters = SnortIdsAlertCounters.from_dict(d["avg_snort_ids_alert_counters"])
+        obj.avg_snort_ids_rule_counters = SnortIdsRuleCounters.from_dict(d["avg_snort_ids_rule_counters"])
         obj.avg_ossec_ids_alert_counters = OSSECIdsAlertCounters.from_dict(d["avg_ossec_ids_alert_counters"])
         return obj
 
     def to_dict(self) -> Dict[str, Any]:
         """
         :return: a dict representation of the object
         """
         d = {}
         d["machines"] = list(map(lambda x: x.to_dict(), self.machines))
         d["actions_tried"] = list(self.actions_tried)
         d["client_population_metrics"] = self.client_population_metrics.to_dict()
         d["docker_stats"] = self.docker_stats.to_dict()
         d["snort_ids_alert_counters"] = self.snort_ids_alert_counters.to_dict()
+        d["snort_ids_rule_counters"] = self.snort_ids_rule_counters.to_dict()
         d["ossec_ids_alert_counters"] = self.ossec_ids_alert_counters.to_dict()
         if self.kafka_config is not None:
             d["kafka_config"] = self.kafka_config.to_dict()
         else:
             d["kafka_config"] = None
         d["attacker_actions"] = list(map(lambda x: x.to_dict(), self.attacker_actions))
         d["defender_actions"] = list(map(lambda x: x.to_dict(), self.defender_actions))
         d["aggregated_host_metrics"] = self.aggregated_host_metrics.to_dict()
         d["avg_aggregated_host_metrics"] = self.avg_aggregated_host_metrics.to_dict()
         d["avg_client_population_metrics"] = self.avg_client_population_metrics.to_dict()
         d["avg_docker_stats"] = self.avg_docker_stats.to_dict()
         d["avg_snort_ids_alert_counters"] = self.avg_snort_ids_alert_counters.to_dict()
+        d["avg_snort_ids_rule_counters"] = self.avg_snort_ids_rule_counters.to_dict()
         d["avg_ossec_ids_alert_counters"] = self.avg_ossec_ids_alert_counters.to_dict()
         return d
 
     def sort_machines(self) -> None:
         """
         Sorts the machines in the observation
 
@@ -199,20 +220,23 @@
         """
         if self.docker_stats_consumer_thread is not None:
             self.docker_stats_consumer_thread.running = False
             self.docker_stats_consumer_thread.consumer.close()
         if self.client_population_consumer_thread is not None:
             self.client_population_consumer_thread.running = False
             self.client_population_consumer_thread.consumer.close()
-        if self.snort_ids_log_consumer_thread is not None:
-            self.snort_ids_log_consumer_thread.running = False
-            self.snort_ids_log_consumer_thread.consumer.close()
-        if self.ossec_ids_log_consumer_thread is not None:
-            self.ossec_ids_log_consumer_thread.running = False
-            self.ossec_ids_log_consumer_thread.consumer.close()
+        if self.aggregated_snort_ids_log_consumer_thread is not None:
+            self.aggregated_snort_ids_log_consumer_thread.running = False
+            self.aggregated_snort_ids_log_consumer_thread.consumer.close()
+        if self.aggregated_snort_ids_rule_log_consumer_thread is not None:
+            self.aggregated_snort_ids_rule_log_consumer_thread.running = False
+            self.aggregated_snort_ids_rule_log_consumer_thread.consumer.close()
+        if self.aggregated_ossec_ids_log_consumer_thread is not None:
+            self.aggregated_ossec_ids_log_consumer_thread.running = False
+            self.aggregated_ossec_ids_log_consumer_thread.consumer.close()
         if self.attacker_actions_consumer_thread is not None:
             self.attacker_actions_consumer_thread.running = False
             self.attacker_actions_consumer_thread.consumer.close()
         if self.defender_actions_consumer_thread is not None:
             self.defender_actions_consumer_thread.running = False
             self.defender_actions_consumer_thread.consumer.close()
         if self.aggregated_host_metrics_thread is not None:
@@ -222,26 +246,31 @@
 
     def reset_metric_lists(self) -> None:
         """
         Resets the metric lists
 
         :return: None
         """
-        self.snort_ids_log_consumer_thread.snort_ids_alert_counters_list = []
-        self.ossec_ids_log_consumer_thread.ossec_ids_alert_counters_list = []
+        self.aggregated_snort_ids_log_consumer_thread.snort_ids_alert_counters_list = []
+        self.aggregated_snort_ids_rule_log_consumer_thread.snort_ids_rule_counters_list = []
+        self.aggregated_ossec_ids_log_consumer_thread.ossec_ids_alert_counters_list = []
         self.docker_stats_consumer_thread.docker_stats_list = []
         self.client_population_consumer_thread.client_population_metrics_list = []
         self.aggregated_host_metrics_thread.host_metrics_list = []
 
     def average_metric_lists(self):
         """
         :return: computes the averages of the metric lists
         """
-        self.avg_snort_ids_alert_counters = self.snort_ids_log_consumer_thread.get_aggregated_ids_alert_counters()
-        self.avg_ossec_ids_alert_counters = self.ossec_ids_log_consumer_thread.get_aggregated_ids_alert_counters()
+        self.avg_snort_ids_alert_counters = \
+            self.aggregated_snort_ids_log_consumer_thread.get_aggregated_ids_alert_counters()
+        self.avg_snort_ids_rule_counters = \
+            self.aggregated_snort_ids_rule_log_consumer_thread.get_aggregated_ids_rule_counters()
+        self.avg_ossec_ids_alert_counters = \
+            self.aggregated_ossec_ids_log_consumer_thread.get_aggregated_ids_alert_counters()
         self.avg_docker_stats = self.docker_stats_consumer_thread.get_average_docker_stats()
         self.avg_aggregated_host_metrics = self.aggregated_host_metrics_thread.get_average_aggregated_host_metrics()
         self.avg_client_population_metrics = \
             self.client_population_consumer_thread.get_average_client_population_metrics()
 
     def get_action_ips(self, a: EmulationDefenderAction, emulation_env_config: EmulationEnvConfig) -> List[str]:
         """
@@ -263,17 +292,20 @@
         """
         c = EmulationDefenderObservationState(
             kafka_config=self.kafka_config,
             client_population_metrics=self.client_population_metrics.copy(), docker_stats=self.docker_stats.copy(),
             snort_ids_alert_counters=self.snort_ids_alert_counters.copy(),
             ossec_ids_alert_counters=self.ossec_ids_alert_counters.copy(),
             attacker_actions=self.attacker_actions.copy(),
-            defender_actions=self.defender_actions.copy(), aggregated_host_metrics=self.aggregated_host_metrics.copy())
+            defender_actions=self.defender_actions.copy(), aggregated_host_metrics=self.aggregated_host_metrics.copy(),
+            snort_ids_rule_counters=self.snort_ids_rule_counters.copy(),
+        )
         c.actions_tried = self.actions_tried.copy()
         c.avg_snort_ids_alert_counters = self.avg_snort_ids_alert_counters.copy()
+        c.avg_snort_ids_rule_counters = self.avg_snort_ids_rule_counters.copy()
         c.avg_ossec_ids_alert_counters = self.avg_ossec_ids_alert_counters.copy()
         c.avg_docker_stats = self.avg_docker_stats.copy()
         c.avg_aggregated_host_metrics = self.avg_aggregated_host_metrics.copy()
         c.avg_client_population_metrics = self.avg_client_population_metrics.copy()
 
         for m in self.machines:
             c.machines.append(m.copy())
@@ -282,19 +314,21 @@
     def __str__(self) -> str:
         """
         :return: a string representation of the object
         """
         return f"client_population_metrics: {self.client_population_metrics}," \
                f"docker_stats: {self.docker_stats}," \
                f"snort_ids_alert_counters: {self.snort_ids_alert_counters}," \
+               f"snort_ids_rule_counters: {self.snort_ids_rule_counters}," \
                f"ossec_ids_alert_counters: {self.ossec_ids_alert_counters}," \
                f"aggregated_host_metrics: {self.aggregated_host_metrics}" \
                f"attacker_actions: {list(map(lambda x: str(x), self.attacker_actions))}," \
                f"defender_actions: {list(map(lambda x: str(x), self.defender_actions))}\n," \
                f"avg_snort_ids_alert_counters: {self.avg_snort_ids_alert_counters}," \
+               f"avg_snort_ids_rule_counters: {self.avg_snort_ids_rule_counters}," \
                f"avg_ossec_ids_alert_counters: {self.avg_ossec_ids_alert_counters}," \
                f"avg_docker_stats: {self.avg_docker_stats}," \
                f"avg_aggregated_host_metrics: {self.avg_aggregated_host_metrics}," \
                f"avg_client_population_metrics: {self.avg_client_population_metrics}" \
                + "\n".join([str(i) + ":" + str(self.machines[i]) for i in range(len(self.machines))])
 
     def to_json_str(self) -> str:
@@ -340,14 +374,16 @@
         num_attributes = 0
         if self.client_population_metrics is not None:
             num_attributes = num_attributes + self.client_population_metrics.num_attributes()
         if self.docker_stats is not None:
             num_attributes = num_attributes + self.docker_stats.num_attributes()
         if self.snort_ids_alert_counters is not None:
             num_attributes = num_attributes + self.snort_ids_alert_counters.num_attributes()
+        if self.snort_ids_rule_counters is not None:
+            num_attributes = num_attributes + 1
         if self.ossec_ids_alert_counters is not None:
             num_attributes = num_attributes + self.ossec_ids_alert_counters.num_attributes()
         if self.aggregated_host_metrics is not None:
             num_attributes = num_attributes + self.aggregated_host_metrics.num_attributes()
         if len(self.defender_actions) > 0:
             num_attributes = num_attributes + len(self.defender_actions) * self.defender_actions[0].num_attributes()
         if len(self.attacker_actions) > 0:
@@ -362,8 +398,9 @@
         return EmulationDefenderObservationState(kafka_config=KafkaConfig.schema(),
                                                  client_population_metrics=ClientPopulationMetrics.schema(),
                                                  docker_stats=DockerStats.schema(),
                                                  snort_ids_alert_counters=SnortIdsAlertCounters.schema(),
                                                  ossec_ids_alert_counters=OSSECIdsAlertCounters.schema(),
                                                  aggregated_host_metrics=HostMetrics.schema(),
                                                  defender_actions=[EmulationDefenderAction.schema()],
-                                                 attacker_actions=[EmulationAttackerAction.schema()])
+                                                 attacker_actions=[EmulationAttackerAction.schema()],
+                                                 snort_ids_rule_counters=SnortIdsRuleCounters.schema())
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/jobs/data_collection_job_config.py` & `csle_common-0.2.0/src/csle_common/dao/jobs/data_collection_job_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     DTO representing the configuration of a data collection job
     """
 
     def __init__(self, emulation_env_name: str, num_collected_steps: int,
                  progress_percentage: float, attacker_sequence: List[EmulationAttackerAction], pid: int,
                  repeat_times: int, emulation_statistic_id: int, num_sequences_completed: int,
                  traces: List[EmulationTrace], save_emulation_traces_every: int, num_cached_traces: int,
-                 defender_sequence: List[EmulationDefenderAction], log_file_path: str,
+                 defender_sequence: List[EmulationDefenderAction], log_file_path: str, physical_host_ip: str,
                  descr: str = ""):
         """
         Initializes the DTO
 
         :param emulation_env_name: the emulation environment name
         :param num_collected_steps: number of collected steps in the emulation
         :param num_sequences_completed: number of sequences completed
@@ -26,14 +26,15 @@
         :param defender_sequence: the sequence of actions to emulate the defender
         :param repeat_times: the number of times to repeat the sequences
         :param traces: list of collected emulation traces
         :param descr: description of the job
         :param emulation_statistic_id: the id of the emulation statistic
         :param save_emulation_traces_every: the frequency to save emulation traces to the metastore
         :param num_cached_traces: the number of emulation traces to keep with the job metadata
+        :param physical_host_ip: the IP of the physical host where the job is running
         """
         self.emulation_env_name = emulation_env_name
         self.progress_percentage = round(progress_percentage, 3)
         self.pid = pid
         self.num_collected_steps = num_collected_steps
         self.progress_percentage = self.progress_percentage
         self.attacker_sequence = attacker_sequence
@@ -44,14 +45,15 @@
         self.repeat_times = repeat_times
         self.emulation_statistic_id = emulation_statistic_id
         self.num_sequences_completed = num_sequences_completed
         self.traces = traces
         self.save_emulation_traces_every = save_emulation_traces_every
         self.num_cached_traces = num_cached_traces
         self.log_file_path = log_file_path
+        self.physical_host_ip = physical_host_ip
 
     def to_dict(self) -> Dict[str, Any]:
         """
         :return: a dict representation of the object
         """
         d = {}
         d["emulation_env_name"] = self.emulation_env_name
@@ -67,14 +69,15 @@
         d["repeat_times"] = self.repeat_times
         d["emulation_statistic_id"] = self.emulation_statistic_id
         d["traces"] = list(map(lambda x: x.to_dict(), self.traces))
         d["num_sequences_completed"] = self.num_sequences_completed
         d["save_emulation_traces_every"] = self.save_emulation_traces_every
         d["num_cached_traces"] = self.num_cached_traces
         d["log_file_path"] = self.log_file_path
+        d["physical_host_ip"] = self.physical_host_ip
         return d
 
     @staticmethod
     def from_dict(d: Dict[str, Any]) -> "DataCollectionJobConfig":
         """
         Converts a dict representation of the object to an instance
 
@@ -86,16 +89,15 @@
             progress_percentage=d["progress_percentage"],
             attacker_sequence=list(map(lambda x: EmulationAttackerAction.from_dict(x), d["attacker_sequence"])),
             defender_sequence=list(map(lambda x: EmulationDefenderAction.from_dict(x), d["defender_sequence"])),
             descr=d["descr"], repeat_times=d["repeat_times"], emulation_statistic_id=d["emulation_statistic_id"],
             traces=list(map(lambda x: EmulationTrace.from_dict(x), d["traces"])),
             num_sequences_completed=d["num_sequences_completed"],
             save_emulation_traces_every=d["save_emulation_traces_every"], num_cached_traces=d["num_cached_traces"],
-            log_file_path=d["log_file_path"]
-        )
+            log_file_path=d["log_file_path"], physical_host_ip=d["physical_host_ip"])
         obj.id = d["id"]
         obj.running = d["running"]
         return obj
 
     def __str__(self) -> str:
         """
         :return: a string representation of the object
@@ -105,15 +107,16 @@
                f"attacker_sequence={list(map(lambda x: str(x), self.attacker_sequence))}," \
                f"defender_sequence={list(map(lambda x: str(x), self.defender_sequence))}, id: {self.id}," \
                f"running:{self.running}, descr: {self.descr}, repeat_times: {self.repeat_times}," \
                f"emulation_statistic_id: {self.emulation_statistic_id}, " \
                f"num_sequences_completed: {self.num_sequences_completed}, " \
                f"traces: {list(map(lambda x: str(x), self.traces))}, " \
                f"save_emulation_traces_every: {self.save_emulation_traces_every}, " \
-               f"num_cached_traces: {self.num_cached_traces}, log_file_path: {self.log_file_path}"
+               f"num_cached_traces: {self.num_cached_traces}, log_file_path: {self.log_file_path}, " \
+               f"physical_host_ip: {self.physical_host_ip}"
 
     def to_json_str(self) -> str:
         """
         Converts the DTO into a json string
 
         :return: the json string representation of the DTO
         """
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/jobs/system_identification_job_config.py` & `csle_common-0.2.0/src/csle_common/dao/jobs/system_identification_job_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,39 +7,40 @@
 class SystemIdentificationJobConfig:
     """
     DTO representing a system identification job
     """
 
     def __init__(self, emulation_env_name: str, emulation_statistics_id: int,
                  progress_percentage: float, pid: int, log_file_path: str,
-                 system_identification_config: SystemIdentificationConfig,
-                 descr: str = "",
-                 system_model: SystemModel = None):
+                 system_identification_config: SystemIdentificationConfig, physical_host_ip: str,
+                 descr: str = "", system_model: SystemModel = None):
         """
         Initializes the DTO
 
         :param emulation_env_name: the name of the emulation that the system identification concerns
         :param emulation_statistics_id: the id of the statistics data to train with
         :param progress_percentage: the progress percentage
         :param pid: the pid of the process
         :param log_file_path: path to the log file
         :param descr: a description of the job
         :param system_model: fitted system model
         :param system_identification_config: the config of the system identification algorithm
+        :param physical_host_ip: the IP of the physical host where the job is running
         """
         self.emulation_env_name = emulation_env_name
         self.emulation_statistics_id = emulation_statistics_id
         self.progress_percentage = progress_percentage
         self.pid = pid
         self.log_file_path = log_file_path
         self.descr = descr
         self.system_model = system_model
         self.system_identification_config = system_identification_config
         self.id = -1
         self.running = False
+        self.physical_host_ip = physical_host_ip
 
     def to_dict(self) -> Dict[str, Any]:
         """
         :return: a dict representation of the object
         """
         d = {}
         d["emulation_env_name"] = self.emulation_env_name
@@ -51,14 +52,15 @@
         if self.system_model is None:
             d["system_model"] = None
         else:
             d["system_model"] = self.system_model.to_dict()
         d["system_identification_config"] = self.system_identification_config.to_dict()
         d["id"] = self.id
         d["running"] = self.running
+        d["physical_host_ip"] = self.physical_host_ip
         return d
 
     @staticmethod
     def from_dict(d: Dict[str, Any]) -> "SystemIdentificationJobConfig":
         """
         Converts a dict representation of the object to an instance
 
@@ -67,15 +69,16 @@
         """
         system_model = None
         system_model = GaussianMixtureSystemModel.from_dict(d["system_model"])
         obj = SystemIdentificationJobConfig(
             emulation_env_name=d["emulation_env_name"], pid=d["pid"],
             progress_percentage=d["progress_percentage"], emulation_statistics_id=d["emulation_statistics_id"],
             descr=d["descr"], log_file_path=d["log_file_path"], system_model=system_model,
-            system_identification_config=SystemIdentificationConfig.from_dict(d["system_identification_config"])
+            system_identification_config=SystemIdentificationConfig.from_dict(d["system_identification_config"]),
+            physical_host_ip=d["physical_host_ip"]
         )
         if "id" in d:
             obj.id = d["id"]
         if "running" in d:
             obj.running = d["running"]
         return obj
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/jobs/training_job_config.py` & `csle_common-0.2.0/src/csle_common/dao/jobs/training_job_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,42 +8,44 @@
     """
     DTO representing the configuration of a training job
     """
 
     def __init__(self, simulation_env_name: str, experiment_config: ExperimentConfig,
                  progress_percentage: float, pid: int, experiment_result: ExperimentResult,
                  emulation_env_name: Union[str, None], simulation_traces: List[SimulationTrace],
-                 num_cached_traces: int, log_file_path: str, descr: str) -> None:
+                 num_cached_traces: int, log_file_path: str, descr: str, physical_host_ip: str) -> None:
         """
         Initializes the DTO
 
         :param simulation_env_name: the simulation environment name
         :param simulation_env_name: the emulation environment name
         :param experiment_config: the experiment configuration
         :param progress_percentage:the progress of the job in percentage
         :param pid: the pid of the process
         :param experiment_result: the result of the job
         :param emulation_env_config: the configuration of the emulation environment
         :param simulation_env_config: the configuration of the simulation environment
         :param simulation_traces: the list of simulation traces
         :param num_cached_traces: number of cached simulation traces
         :param descr: description of the job
+        :param physical_host_ip: the IP of the physical host where the job is running
         """
         self.simulation_env_name = simulation_env_name
         self.emulation_env_name = emulation_env_name
         self.experiment_config = experiment_config
         self.experiment_result = experiment_result
         self.progress_percentage = round(progress_percentage, 3)
         self.pid = pid
         self.id = -1
         self.running = False
         self.simulation_traces = simulation_traces
         self.num_cached_traces = num_cached_traces
         self.log_file_path = log_file_path
         self.descr = descr
+        self.physical_host_ip = physical_host_ip
 
     def to_dict(self) -> Dict[str, Any]:
         """
         :return: a dict representation of the object
         """
         d = {}
         d["simulation_env_name"] = self.simulation_env_name
@@ -54,14 +56,15 @@
         d["id"] = self.id
         d["experiment_result"] = self.experiment_result.to_dict()
         d["running"] = self.running
         d["simulation_traces"] = list(map(lambda x: x.to_dict(), self.simulation_traces))
         d["num_cached_traces"] = self.num_cached_traces
         d["log_file_path"] = self.log_file_path
         d["descr"] = self.descr
+        d["physical_host_ip"] = self.physical_host_ip
         return d
 
     @staticmethod
     def from_dict(d: Dict[str, Any]) -> "TrainingJobConfig":
         """
         Converts a dict representation of the object to an instance
         :param d: the dict to convert
@@ -70,29 +73,31 @@
         obj = TrainingJobConfig(
             simulation_env_name=d["simulation_env_name"],
             experiment_config=ExperimentConfig.from_dict(d["experiment_config"]),
             progress_percentage=d["progress_percentage"], pid=d["pid"],
             experiment_result=ExperimentResult.from_dict(d["experiment_result"]),
             emulation_env_name=d["emulation_env_name"],
             simulation_traces=list(map(lambda x: SimulationTrace.from_dict(x), d["simulation_traces"])),
-            num_cached_traces=d["num_cached_traces"], log_file_path=d["log_file_path"], descr=d["descr"])
+            num_cached_traces=d["num_cached_traces"], log_file_path=d["log_file_path"], descr=d["descr"],
+            physical_host_ip=d["physical_host_ip"])
         obj.id = d["id"]
         obj.running = d["running"]
         return obj
 
     def __str__(self) -> str:
         """
         :return: a string representation of the object
         """
         return f"simulation_env_name: {self.simulation_env_name}, experiment_config: {self.experiment_config}, " \
                f"progress_percentage: {self.progress_percentage}, pid: {self.pid}," \
                f"id: {self.id}, experiment_result: {self.experiment_result}, running: {self.running}, " \
                f"emulation_env_name: {self.emulation_env_name}, " \
                f"simulation_traces: {list(map(lambda x: str(x), self.simulation_traces))}," \
-               f"num_cached_traces: {self.num_cached_traces}, log_file_path: {self.log_file_path}, descr: {self.descr}"
+               f"num_cached_traces: {self.num_cached_traces}, log_file_path: {self.log_file_path}, " \
+               f"descr: {self.descr}, physical_host_ip: {self.physical_host_ip}"
 
     def to_json_str(self) -> str:
         """
         Converts the DTO into a json string
 
         :return: the json string representation of the DTO
         """
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/management/management_user.py` & `csle_common-0.2.0/src/csle_common/dao/management/management_user.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/management/session_token.py` & `csle_common-0.2.0/src/csle_common/dao/management/session_token.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/action.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/action.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/action_space_config.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/action_space_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/base_env.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/base_env.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 from abc import ABC, abstractmethod
-import gym
+import gymnasium as gym
 from csle_common.dao.simulation_config.simulation_trace import SimulationTrace
 
 
 class BaseEnv(gym.Env, ABC):
     """
     Abstract class representing a csle Environment
     """
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/env_parameter.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/env_parameter.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/env_parameters_config.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/env_parameters_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/initial_state_distribution_config.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/initial_state_distribution_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/joint_action_space_config.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/joint_action_space_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/joint_observation_space_config.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/joint_observation_space_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/observation.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/observation.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/observation_function_config.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/observation_function_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/observation_space_config.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/observation_space_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/player_config.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/player_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/players_config.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/players_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/reward_function_config.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/reward_function_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/simulation_env_config.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/simulation_env_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/simulation_trace.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/simulation_trace.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/state.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/state_space_config.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/state_space_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/simulation_config/transition_operator_config.py` & `csle_common-0.2.0/src/csle_common/dao/simulation_config/transition_operator_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/system_identification/empirical_conditional.py` & `csle_common-0.2.0/src/csle_common/dao/system_identification/empirical_conditional.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/system_identification/empirical_system_model.py` & `csle_common-0.2.0/src/csle_common/dao/system_identification/empirical_system_model.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/system_identification/emulation_statistics.py` & `csle_common-0.2.0/src/csle_common/dao/system_identification/emulation_statistics.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,20 +21,22 @@
 
         :param emulation_name: the name of the emulation that the statistics is linked to
         :param descr: a free text description of the statistics
         """
         self.emulation_name = emulation_name
         self.descr = descr
         self.initial_distributions_counts = self.initialize_counters(
-            d={}, labels=collector_constants.KAFKA_CONFIG.ALL_INITIAL_LABELS)
+            d={}, agg_labels=collector_constants.KAFKA_CONFIG.ALL_INITIAL_AGG_LABELS)
         self.conditionals_counts = {}
         self.conditionals_counts[constants.SYSTEM_IDENTIFICATION.INTRUSION_CONDITIONAL] = \
-            EmulationStatistics.initialize_counters(d={}, labels=collector_constants.KAFKA_CONFIG.ALL_DELTA_LABELS)
+            EmulationStatistics.initialize_counters(d={},
+                                                    agg_labels=collector_constants.KAFKA_CONFIG.ALL_DELTA_AGG_LABELS)
         self.conditionals_counts[constants.SYSTEM_IDENTIFICATION.NO_INTRUSION_CONDITIONAL] = \
-            EmulationStatistics.initialize_counters(d={}, labels=collector_constants.KAFKA_CONFIG.ALL_DELTA_LABELS)
+            EmulationStatistics.initialize_counters(d={},
+                                                    agg_labels=collector_constants.KAFKA_CONFIG.ALL_DELTA_AGG_LABELS)
         self.id = -1
         self.means = {}
         self.stds = {}
         self.mins = {}
         self.maxs = {}
         self.conditionals_probs = {}
         self.initial_distributions_probs = {}
@@ -46,26 +48,68 @@
         self.num_metrics = 0
         self.num_measurements = 0
         self.num_conditions = 0
         self.conditions = []
         self.metrics = []
 
     @staticmethod
-    def initialize_counters(d: Dict[str, Dict[int, int]], labels: List[str]) -> Dict[str, Dict[int, int]]:
+    def initialize_counters(d: Dict[str, Dict[int, int]], agg_labels: List[str]) \
+            -> Dict[str, Dict[int, int]]:
         """
         Initializes counters for a given dict
-        :param d: the dict to initialzie
-        :return: the initialized dict
-        """
 
-        for label in labels:
+        :param d: the dict to initialize
+        :param agg_labels: the labels
+        :return: the updated dict
+        """
+        for label in agg_labels:
             d[label] = {}
 
         return d
 
+    @staticmethod
+    def initialize_machine_counters(d: Dict[str, Dict[int, int]], s: EmulationEnvState, labels: List[str]) \
+            -> Dict[str, Dict[int, int]]:
+        """
+        Initializes counters for a given dict
+
+        :param d: the dict to initialize
+        :param s: the state with the list of machines
+        :param labels: the labels to initialize
+        :return: the initialized dict
+        """
+        labels = collector_constants.KAFKA_CONFIG.ALL_INITIAL_MACHINE_LABELS
+        for label in labels:
+            for machine in s.defender_obs_state.machines:
+                lbl = f"{label}_{machine.ips[0]}"
+                d[lbl] = {}
+        return d
+
+    def initialize_machines(self, s: EmulationEnvState) -> None:
+        """
+        Initializes counters for a given dict
+
+        :param d: the dict to initialize
+        :param s: the state with the list of machines
+        :return: the initialized dict
+        """
+        self.initial_distributions_counts = EmulationStatistics.initialize_machine_counters(
+            d=self.initial_distributions_counts, s=s,
+            labels=collector_constants.KAFKA_CONFIG.ALL_INITIAL_MACHINE_LABELS)
+        self.conditionals_counts[constants.SYSTEM_IDENTIFICATION.INTRUSION_CONDITIONAL] = \
+            EmulationStatistics.initialize_machine_counters(
+                s=s,
+                d=self.conditionals_counts[constants.SYSTEM_IDENTIFICATION.INTRUSION_CONDITIONAL],
+                labels=collector_constants.KAFKA_CONFIG.ALL_DELTA_MACHINE_LABELS)
+        self.conditionals_counts[constants.SYSTEM_IDENTIFICATION.NO_INTRUSION_CONDITIONAL] = \
+            EmulationStatistics.initialize_machine_counters(
+                s=s,
+                d=self.conditionals_counts[constants.SYSTEM_IDENTIFICATION.NO_INTRUSION_CONDITIONAL],
+                labels=collector_constants.KAFKA_CONFIG.ALL_DELTA_MACHINE_LABELS)
+
     def update_counters(self, d: Dict, s: EmulationEnvState, s_prime: EmulationEnvState) -> None:
         """
         Updates the delta counters for a specific dict based on a state transition s->s'
 
         :param d: the dict to update
         :param s: the current state
         :param s_prime: the new state
@@ -76,33 +120,65 @@
         snort_alert_deltas, snort_alert_labels = s.defender_obs_state.avg_snort_ids_alert_counters.get_deltas(
             s_prime.defender_obs_state.avg_snort_ids_alert_counters)
         for i in range(len(snort_alert_deltas)):
             if snort_alert_deltas[i] in d[snort_alert_labels[i]]:
                 d[snort_alert_labels[i]][snort_alert_deltas[i]] += 1
             else:
                 d[snort_alert_labels[i]][snort_alert_deltas[i]] = 1
+        for machine in s.defender_obs_state.machines:
+            s_prime_machine = s_prime.get_defender_machine(ip=machine.ips[0])
+            snort_alert_deltas, snort_alert_labels = machine.snort_ids_ip_alert_counters.get_deltas(
+                s_prime_machine.snort_ids_ip_alert_counters)
+            for i in range(len(snort_alert_deltas)):
+                lbl = f"{snort_alert_labels[i]}_{machine.ips[0]}"
+                if snort_alert_deltas[i] in d[lbl]:
+                    d[lbl][snort_alert_deltas[i]] += 1
+                else:
+                    d[lbl][snort_alert_deltas[i]] = 1
 
         # OSSEC alerts
         ossec_alert_deltas, ossec_alert_labels = s.defender_obs_state.avg_ossec_ids_alert_counters.get_deltas(
             s_prime.defender_obs_state.avg_ossec_ids_alert_counters)
         for i in range(len(ossec_alert_deltas)):
             if ossec_alert_deltas[i] in d[ossec_alert_labels[i]]:
                 d[ossec_alert_labels[i]][ossec_alert_deltas[i]] += 1
             else:
                 d[ossec_alert_labels[i]][ossec_alert_deltas[i]] = 1
 
+        for machine in s.defender_obs_state.machines:
+            s_prime_machine = s_prime.get_defender_machine(ip=machine.ips[0])
+            ossec_alert_deltas, ossec_alert_labels = machine.ossec_ids_alert_counters.get_deltas(
+                s_prime_machine.ossec_ids_alert_counters)
+            for i in range(len(ossec_alert_deltas)):
+                lbl = f"{ossec_alert_labels[i]}_{machine.ips[0]}"
+                if ossec_alert_deltas[i] in d[lbl]:
+                    d[lbl][ossec_alert_deltas[i]] += 1
+                else:
+                    d[lbl][ossec_alert_deltas[i]] = 1
+
         # Docker stats
         docker_stats_deltas, docker_stats_labels = s.defender_obs_state.avg_docker_stats.get_deltas(
             stats_prime=s_prime.defender_obs_state.avg_docker_stats)
         for i in range(len(docker_stats_deltas)):
             if docker_stats_deltas[i] in d[docker_stats_labels[i]]:
                 d[docker_stats_labels[i]][docker_stats_deltas[i]] += 1
             else:
                 d[docker_stats_labels[i]][docker_stats_deltas[i]] = 1
 
+        for machine in s.defender_obs_state.machines:
+            s_prime_machine = s_prime.get_defender_machine(ip=machine.ips[0])
+            docker_stats_deltas, docker_stats_labels = machine.docker_stats.get_deltas(
+                stats_prime=s_prime_machine.docker_stats)
+            for i in range(len(docker_stats_deltas)):
+                lbl = f"{docker_stats_labels[i]}_{machine.ips[0]}"
+                if docker_stats_deltas[i] in d[lbl]:
+                    d[lbl][docker_stats_deltas[i]] += 1
+                else:
+                    d[lbl][docker_stats_deltas[i]] = 1
+
         # Client metrics
         client_population_metrics_deltas, client_population_metrics_labels = (
             s.defender_obs_state.avg_client_population_metrics.get_deltas(
                 stats_prime=s_prime.defender_obs_state.avg_client_population_metrics))
         for i in range(len(client_population_metrics_deltas)):
             if client_population_metrics_deltas[i] in d[client_population_metrics_labels[i]]:
                 d[client_population_metrics_labels[i]][client_population_metrics_deltas[i]] += 1
@@ -115,14 +191,25 @@
                 stats_prime=s_prime.defender_obs_state.avg_aggregated_host_metrics)
         for i in range(len(aggregated_host_metrics_deltas)):
             if aggregated_host_metrics_deltas[i] in d[aggregated_host_metrics_labels[i]]:
                 d[aggregated_host_metrics_labels[i]][aggregated_host_metrics_deltas[i]] += 1
             else:
                 d[aggregated_host_metrics_labels[i]][aggregated_host_metrics_deltas[i]] = 1
 
+        for machine in s.defender_obs_state.machines:
+            s_prime_machine = s_prime.get_defender_machine(ip=machine.ips[0])
+            host_metrics_deltas, host_metrics_labels = machine.host_metrics.get_deltas(
+                stats_prime=s_prime_machine.host_metrics)
+            for i in range(len(host_metrics_deltas)):
+                lbl = f"{host_metrics_labels[i]}_{machine.ips[0]}"
+                if host_metrics_deltas[i] in d[lbl]:
+                    d[lbl][host_metrics_deltas[i]] += 1
+                else:
+                    d[lbl][host_metrics_deltas[i]] = 1
+
     def update_delta_statistics(self, s: EmulationEnvState, s_prime: EmulationEnvState, a1: EmulationDefenderAction,
                                 a2: EmulationAttackerAction) -> None:
         """
         Updates the emulation statistics (delta counters) with a given transition (s, a1, a2) -> (s')
 
         :param s: the previous state
         :param s_prime: the new state
@@ -141,15 +228,21 @@
 
         logged_in_ips = list(map(lambda x: "_".join(x.ips), filter(
             lambda x: x.logged_in and x.tools_installed and x.backdoor_installed and x.root,
             s.attacker_obs_state.machines)))
         # Action conditionals
         if f"A:{a2.name}_D:{a1.name}_M:{logged_in_ips}" not in self.conditionals_counts:
             self.conditionals_counts[f"A:{a2.name}_D:{a1.name}_M:{logged_in_ips}"] = \
-                EmulationStatistics.initialize_counters(d={}, labels=collector_constants.KAFKA_CONFIG.ALL_DELTA_LABELS)
+                EmulationStatistics.initialize_counters(
+                    d={}, agg_labels=collector_constants.KAFKA_CONFIG.ALL_DELTA_AGG_LABELS)
+            self.conditionals_counts[f"A:{a2.name}_D:{a1.name}_M:{logged_in_ips}"] = \
+                EmulationStatistics.initialize_machine_counters(
+                    s=s,
+                    d=self.conditionals_counts[f"A:{a2.name}_D:{a1.name}_M:{logged_in_ips}"],
+                    labels=collector_constants.KAFKA_CONFIG.ALL_DELTA_MACHINE_LABELS)
         self.update_counters(
             d=self.conditionals_counts[f"A:{a2.name}_D:{a1.name}_M:{logged_in_ips}"], s=s, s_prime=s_prime)
 
     def update_initial_statistics(self, s: EmulationEnvState) -> None:
         """
         Updates the emulation statistics for the initial state
 
@@ -158,50 +251,80 @@
         """
         snort_alert_labels = collector_constants.KAFKA_CONFIG.SNORT_IDS_ALERTS_LABELS
         for i in range(len(snort_alert_labels)):
             if 0 in self.initial_distributions_counts[snort_alert_labels[i]]:
                 self.initial_distributions_counts[snort_alert_labels[i]][0] += 1
             else:
                 self.initial_distributions_counts[snort_alert_labels[i]][0] = 1
+            for machine in s.defender_obs_state.machines:
+                lbl = f"{snort_alert_labels[i]}_{machine.ips[0]}"
+                if 0 in self.initial_distributions_counts[lbl]:
+                    self.initial_distributions_counts[lbl][0] += 1
+                else:
+                    self.initial_distributions_counts[lbl][0] = 1
 
         ossec_alert_labels = collector_constants.KAFKA_CONFIG.OSSEC_IDS_ALERTS_LABELS
         for i in range(len(ossec_alert_labels)):
             if 0 in self.initial_distributions_counts[ossec_alert_labels[i]]:
                 self.initial_distributions_counts[ossec_alert_labels[i]][0] += 1
             else:
                 self.initial_distributions_counts[ossec_alert_labels[i]][0] = 1
+            for machine in s.defender_obs_state.machines:
+                lbl = f"{ossec_alert_labels[i]}_{machine.ips[0]}"
+                if 0 in self.initial_distributions_counts[lbl]:
+                    self.initial_distributions_counts[lbl][0] += 1
+                else:
+                    self.initial_distributions_counts[lbl][0] = 1
 
         docker_stats_values, docker_stats_labels = s.defender_obs_state.docker_stats.get_values()
         for i in range(len(docker_stats_values)):
             if docker_stats_values[i] in self.initial_distributions_counts[docker_stats_labels[i]]:
                 self.initial_distributions_counts[docker_stats_labels[i]][docker_stats_values[i]] += 1
             else:
                 self.initial_distributions_counts[docker_stats_labels[i]][docker_stats_values[i]] = 1
+        for machine in s.defender_obs_state.machines:
+            m_values, m_labels = machine.docker_stats.get_values()
+            for i in range(len(m_values)):
+                lbl = f"{m_labels[i]}_{machine.ips[0]}"
+                if m_values[i] in self.initial_distributions_counts[lbl]:
+                    self.initial_distributions_counts[lbl][m_values[i]] += 1
+                else:
+                    self.initial_distributions_counts[lbl][m_values[i]] = 1
 
         client_population_metrics_values, client_population_metrics_labels = \
             s.defender_obs_state.client_population_metrics.get_values()
         for i in range(len(client_population_metrics_values)):
             if (client_population_metrics_values[i] in
                     self.initial_distributions_counts[client_population_metrics_labels[i]]):
                 self.initial_distributions_counts[
                     client_population_metrics_labels[i]][client_population_metrics_values[i]] += 1
             else:
                 self.initial_distributions_counts[
                     client_population_metrics_labels[i]][client_population_metrics_values[i]] = 1
+
         aggregated_host_metrics_values, aggregated_host_metrics_labels = \
             s.defender_obs_state.aggregated_host_metrics.get_values()
         for i in range(len(aggregated_host_metrics_values)):
             if (aggregated_host_metrics_values[i] in
                     self.initial_distributions_counts[aggregated_host_metrics_labels[i]]):
                 self.initial_distributions_counts[
                     aggregated_host_metrics_labels[i]][aggregated_host_metrics_values[i]] += 1
             else:
                 self.initial_distributions_counts[aggregated_host_metrics_labels[i]][
                     aggregated_host_metrics_values[i]] = 1
 
+        for machine in s.defender_obs_state.machines:
+            m_values, m_labels = machine.host_metrics.get_values()
+            for i in range(len(m_values)):
+                lbl = f"{m_labels[i]}_{machine.ips[0]}"
+                if (m_values[i] in self.initial_distributions_counts[lbl]):
+                    self.initial_distributions_counts[lbl][m_values[i]] += 1
+                else:
+                    self.initial_distributions_counts[lbl][m_values[i]] = 1
+
     def compute_descriptive_statistics_and_distributions(self) -> None:
         """
         Computes descriptive statistics and empirical probability distributions based on the counters.
 
         :return: None
         """
         self.num_measurements = 0
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/system_identification/gaussian_mixture_conditional.py` & `csle_common-0.2.0/src/csle_common/dao/system_identification/gaussian_mixture_conditional.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/system_identification/gaussian_mixture_system_model.py` & `csle_common-0.2.0/src/csle_common/dao/system_identification/gaussian_mixture_system_model.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/system_identification/gp_conditional.py` & `csle_common-0.2.0/src/csle_common/dao/system_identification/gp_conditional.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/system_identification/gp_system_model.py` & `csle_common-0.2.0/src/csle_common/dao/system_identification/gp_system_model.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/system_identification/system_identification_config.py` & `csle_common-0.2.0/src/csle_common/dao/system_identification/system_identification_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/system_identification/system_model.py` & `csle_common-0.2.0/src/csle_common/dao/system_identification/system_model.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/training/agent_type.py` & `csle_common-0.2.0/src/csle_common/dao/training/agent_type.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/training/alpha_vectors_policy.py` & `csle_common-0.2.0/src/csle_common/dao/training/alpha_vectors_policy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Union, List, Dict, Any
 import numpy as np
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.dao.training.player_type import PlayerType
 from csle_common.dao.training.policy import Policy
 from csle_common.dao.simulation_config.action import Action
 from csle_common.dao.simulation_config.state import State
+from csle_common.dao.training.policy_type import PolicyType
 
 
 class AlphaVectorsPolicy(Policy):
     """
     Object representing a policy based on alpha vectors for a POMDP (Sondik 1971)
     """
 
@@ -33,14 +34,15 @@
         self.alpha_vectors = alpha_vectors
         self.simulation_name = simulation_name
         self.id = -1
         self.avg_R = avg_R
         self.transition_tensor = transition_tensor
         self.reward_tensor = reward_tensor
         self.states = states
+        self.policy_type = PolicyType.ALPHA_VECTORS
 
     def action(self, o: Union[List[Union[int, float]], int, float]) -> Union[int, float]:
         """
         Selects the next action
 
         :param o: the belief
         :return: the next action and its probability
@@ -104,14 +106,15 @@
         d["alpha_vectors"] = self.alpha_vectors
         d["simulation_name"] = self.simulation_name
         d["id"] = self.id
         d["avg_R"] = self.avg_R
         d["transition_tensor"] = self.transition_tensor
         d["states"] = list(map(lambda x: x.to_dict(), self.states))
         d["reward_tensor"] = self.reward_tensor
+        d["policy_type"] = self.policy_type
         return d
 
     def stage_policy(self, o: Union[List[Union[int, float]], int, float]) -> List[List[float]]:
         """
         Gets the stage policy, i.e a |S|x|A| policy
 
         :param o: the latest observation
@@ -123,15 +126,15 @@
         """
         :return: a string representation of the policy
         """
         return f"agent_type: {self.agent_type}, player_type: {self.player_type}, " \
                f"actions: {list(map(lambda x: str(x), self.actions))}, alpha_vectors: {self.alpha_vectors}, " \
                f"simulation_name: {self.simulation_name}, id: {self.id}, avg_R: {self.avg_R}," \
                f"transition_tensor: {self.transition_tensor}, states: {self.states}, " \
-               f"reward_tensor: {self.reward_tensor}"
+               f"reward_tensor: {self.reward_tensor}, policy_type: {self.policy_type}"
 
     def to_json_str(self) -> str:
         """
         Converts the DTO into a json string
 
         :return: the json string representation of the DTO
         """
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/training/dqn_policy.py` & `csle_common-0.2.0/src/csle_common/dao/training/ppo_policy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 from typing import List, Dict, Union
 import numpy as np
 import torch
-from stable_baselines3 import DQN
+import math
+from stable_baselines3 import PPO
 from csle_common.dao.training.policy import Policy
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.dao.training.player_type import PlayerType
 from csle_common.dao.simulation_config.state import State
 from csle_common.dao.simulation_config.state_type import StateType
 from csle_common.dao.simulation_config.action import Action
 from csle_common.dao.training.experiment_config import ExperimentConfig
+from csle_common.dao.training.policy_type import PolicyType
 from csle_common.logging.log import Logger
 
 
-class DQNPolicy(Policy):
+class PPOPolicy(Policy):
     """
-    A neural network policy learned with DQN
+    A neural network policy learned with PPO
     """
 
     def __init__(self, model, simulation_name: str, save_path: str, player_type: PlayerType, states: List[State],
                  actions: List[Action], experiment_config: ExperimentConfig, avg_R: float):
         """
         Initializes the policy
 
-        :param model: the DQN model
+        :param model: the PPO model
         :param simulation_name: the simulation name
         :param save_path: the path to save the model to
         :param states: list of states (required for computing stage policies)
         :param actions: list of actions
         :param experiment_config: the experiment configuration for training the policy
         :param avg_R: the average reward of the policy when evaluated in the simulation
         """
-        super(DQNPolicy, self).__init__(agent_type=AgentType.DQN, player_type=player_type)
+        super(PPOPolicy, self).__init__(agent_type=AgentType.PPO, player_type=player_type)
         self.model = model
         self.id = -1
         self.simulation_name = simulation_name
         self.save_path = save_path
         if self.model is None:
             try:
-                self.model = DQN.load(path=self.save_path)
+                self.model = PPO.load(path=self.save_path)
             except Exception as e:
                 Logger.__call__().get_logger().warning(
                     f"There was an exception loading the model from path: {self.save_path}, "
                     f"exception: {str(e)}, {repr(e)}")
         self.states = states
         self.actions = actions
         self.experiment_config = experiment_config
         self.avg_R = avg_R
+        self.policy_type = PolicyType.PPO
 
     def action(self, o: List[float]) -> Union[int, List[int], np.ndarray]:
         """
         Multi-threshold stopping policy
 
         :param o: the current observation
         :return: the selected action
@@ -60,18 +63,18 @@
     def probability(self, o: List[float], a) -> Union[int, List[int], np.ndarray]:
         """
         Multi-threshold stopping policy
 
         :param o: the current observation
         :return: the selected action
         """
-        actions = self.model.policy.forward(obs=torch.tensor(o).to(self.model.device))
+        actions, values, log_prob = self.model.policy.forward(obs=torch.tensor(o).to(self.model.device))
         action = actions[0]
         if action == a:
-            return 1
+            return math.exp(log_prob)
         else:
             return 0
 
     def to_dict(self) -> Dict[str, Union[float, int, str]]:
         """
         :return: a dict representation of the policy
         """
@@ -87,25 +90,26 @@
             d["policy_kwargs"]["net_arch"] = []
         d["states"] = list(map(lambda x: x.to_dict(), self.states))
         d["player_type"] = self.player_type
         d["actions"] = list(map(lambda x: x.to_dict(), self.actions))
         d["experiment_config"] = self.experiment_config.to_dict()
         d["agent_type"] = self.agent_type
         d["avg_R"] = self.avg_R
+        d["policy_type"] = self.policy_type
         return d
 
     @staticmethod
-    def from_dict(d: Dict) -> "DQNPolicy":
+    def from_dict(d: Dict) -> "PPOPolicy":
         """
         Converst a dict representation of the object to an instance
 
         :param d: the dict to convert
         :return: the created instance
         """
-        obj = DQNPolicy(model=None, simulation_name=d["simulation_name"], save_path=d["save_path"],
+        obj = PPOPolicy(model=None, simulation_name=d["simulation_name"], save_path=d["save_path"],
                         states=list(map(lambda x: State.from_dict(x), d["states"])), player_type=d["player_type"],
                         actions=list(map(lambda x: Action.from_dict(x), d["actions"])),
                         experiment_config=ExperimentConfig.from_dict(d["experiment_config"]), avg_R=d["avg_R"])
         obj.id = d["id"]
         return obj
 
     def stage_policy(self, o: Union[List[Union[int, float]], int, float]) -> List[List[float]]:
@@ -116,49 +120,49 @@
         :return: the |S|x|A| stage policy
         """
         b1 = o[1]
         l = int(o[0])
         if not self.player_type == PlayerType.ATTACKER:
             stage_policy = []
             for _ in self.states:
-                stage_policy.append(self._get_attacker_stopping_dist(obs=o))
+                stage_policy.append(self._get_attacker_dist(obs=o))
             return stage_policy
         else:
             stage_policy = []
             for s in self.states:
                 if s.state_type != StateType.TERMINAL:
                     o = [l, b1, s.id]
-                    stage_policy.append(self._get_attacker_stopping_dist(obs=o))
+                    stage_policy.append(self._get_attacker_dist(obs=o))
                 else:
                     stage_policy.append([0.5, 0.5])
             return stage_policy
 
-    def _get_attacker_stopping_dist(self, obs) -> List[float]:
+    def _get_attacker_dist(self, obs) -> List[float]:
         """
-        Utility function for getting the stopping action distribution conditioned on a given observation
+        Utility function for getting the action distribution conditioned on a given observation
 
         :param obs: the observation to condition on
         :return: the conditional ation distribution
         """
         obs = np.array([obs])
-        actions = self.model.policy.forward(obs=torch.tensor(obs).to(self.model.device))
+        actions, values, log_prob = self.model.policy.forward(obs=torch.tensor(obs).to(self.model.device))
         action = actions[0]
         if action == 1:
-            stop_prob = 1
+            stop_prob = math.exp(log_prob)
         else:
-            stop_prob = 0
+            stop_prob = 1 - math.exp(log_prob)
         return [1 - stop_prob, stop_prob]
 
     def __str__(self) -> str:
         """
         :return: a string representation of the object
         """
         return f"model: {self.model}, id: {self.id}, simulation_name: {self.simulation_name}, " \
                f"save path: {self.save_path}, states: {self.states}, experiment_config: {self.experiment_config}," \
-               f"avg_R: {self.avg_R}"
+               f"avg_R: {self.avg_R}, policy type: {self.policy_type}"
 
     def to_json_str(self) -> str:
         """
         Converts the DTO into a json string
 
         :return: the json string representation of the DTO
         """
@@ -175,25 +179,25 @@
         """
         import io
         json_str = self.to_json_str()
         with io.open(json_file_path, 'w', encoding='utf-8') as f:
             f.write(json_str)
 
     @staticmethod
-    def from_json_file(json_file_path: str) -> "DQNPolicy":
+    def from_json_file(json_file_path: str) -> "PPOPolicy":
         """
         Reads a json file and converts it to a DTO
 
         :param json_file_path: the json file path
         :return: the converted DTO
         """
         import io
         import json
         with io.open(json_file_path, 'r') as f:
             json_str = f.read()
-        return DQNPolicy.from_dict(json.loads(json_str))
+        return PPOPolicy.from_dict(json.loads(json_str))
 
-    def copy(self) -> "DQNPolicy":
+    def copy(self) -> "PPOPolicy":
         """
         :return: a copy of the DTO
         """
         return self.from_dict(self.to_dict())
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/training/experiment_config.py` & `csle_common-0.2.0/src/csle_common/dao/training/experiment_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/training/experiment_execution.py` & `csle_common-0.2.0/src/csle_common/dao/training/experiment_execution.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/training/experiment_result.py` & `csle_common-0.2.0/src/csle_common/dao/training/experiment_result.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/training/fnn_with_softmax_policy.py` & `csle_common-0.2.0/src/csle_common/dao/training/fnn_with_softmax_policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from csle_common.dao.training.policy import Policy
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.dao.training.player_type import PlayerType
 from csle_common.dao.simulation_config.state import State
 from csle_common.dao.simulation_config.state_type import StateType
 from csle_common.dao.simulation_config.action import Action
 from csle_common.dao.training.experiment_config import ExperimentConfig
+from csle_common.dao.training.policy_type import PolicyType
 from csle_common.logging.log import Logger
 
 
 class FNNWithSoftmaxPolicy(Policy):
     """
     A feed-forward neural network policy with softmax output
     """
@@ -42,14 +43,15 @@
         self.save_path = save_path
         self.states = states
         self.actions = actions
         self.experiment_config = experiment_config
         self.avg_R = avg_R
         self.input_dim = input_dim
         self.output_dim = output_dim
+        self.policy_type = PolicyType.FNN_W_SOFTMAX
         if self.policy_network is None:
             try:
                 self.policy_network = FNNwithSoftmax(
                     input_dim=input_dim,
                     output_dim=output_dim,
                     hidden_dim=self.experiment_config.hparams[
                         constants.NEURAL_NETWORKS.NUM_NEURONS_PER_HIDDEN_LAYER].value,
@@ -147,14 +149,15 @@
         d["player_type"] = self.player_type
         d["actions"] = list(map(lambda x: x.to_dict(), self.actions))
         d["experiment_config"] = self.experiment_config.to_dict()
         d["agent_type"] = self.agent_type
         d["avg_R"] = self.avg_R
         d["input_dim"] = self.input_dim
         d["output_dim"] = self.output_dim
+        d["policy_type"] = self.policy_type
         return d
 
     @staticmethod
     def from_dict(d: Dict) -> "FNNWithSoftmaxPolicy":
         """
         Converst a dict representation of the object to an instance
 
@@ -163,15 +166,16 @@
         """
         obj = FNNWithSoftmaxPolicy(policy_network=None, simulation_name=d["simulation_name"],
                                    save_path=d["save_path"],
                                    states=list(map(lambda x: State.from_dict(x), d["states"])),
                                    player_type=d["player_type"],
                                    actions=list(map(lambda x: Action.from_dict(x), d["actions"])),
                                    experiment_config=ExperimentConfig.from_dict(d["experiment_config"]),
-                                   avg_R=d["avg_R"], input_dim=d["input_dim"], output_dim=d["output_dim"])
+                                   avg_R=d["avg_R"], input_dim=d["input_dim"], output_dim=d["output_dim"],
+                                   policy_type=d["policy_type"])
         obj.id = d["id"]
         return obj
 
     def stage_policy(self, o: Union[List[Union[int, float]], int, float]) -> List[List[float]]:
         """
         Gets the stage policy, i.e a |S|x|A| policy
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/training/hparam.py` & `csle_common-0.2.0/src/csle_common/dao/training/hparam.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/training/mixed_multi_threshold_stopping_policy.py` & `csle_common-0.2.0/src/csle_common/dao/training/mixed_multi_threshold_stopping_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from csle_common.dao.training.policy import Policy
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.dao.simulation_config.state import State
 from csle_common.dao.training.player_type import PlayerType
 from csle_common.dao.simulation_config.action import Action
 from csle_common.dao.training.experiment_config import ExperimentConfig
 from csle_common.dao.simulation_config.state_type import StateType
+from csle_common.dao.training.policy_type import PolicyType
 from csle_common.dao.training.multi_threshold_stopping_policy import MultiThresholdStoppingPolicy
 
 
 class MixedMultiThresholdStoppingPolicy(Policy):
     """
     A mixed multi-threshold stopping policy
     """
@@ -41,14 +42,15 @@
         self.simulation_name = simulation_name
         self.L = L
         self.states = states
         self.actions = actions
         self.experiment_config = experiment_config
         self.avg_R = avg_R
         self.opponent_strategy = opponent_strategy
+        self.policy_type = PolicyType.MIXED_MULTI_THRESHOLD
 
     def probability(self, o: List[float], a: int) -> int:
         """
         Probability of a given action
 
         :param o: the current observation
         :param a: a given action
@@ -146,14 +148,15 @@
         d["agent_type"] = self.agent_type
         d["L"] = self.L
         if self.experiment_config is not None:
             d["experiment_config"] = self.experiment_config.to_dict()
         else:
             d["experiment_config"] = None
         d["avg_R"] = self.avg_R
+        d["policy_type"] = self.policy_type
         return d
 
     @staticmethod
     def from_dict(d: Dict) -> "MixedMultiThresholdStoppingPolicy":
         """
         Converst a dict representation of the object to an instance
 
@@ -296,15 +299,15 @@
     def __str__(self) -> str:
         """
         :return: a string representation of the object
         """
         return f"Theta: {self.Theta}, id: {self.id}, simulation_name: {self.simulation_name}, " \
                f"player_type: {self.player_type}, " \
                f"L:{self.L}, states: {self.states}, agent_type: {self.agent_type}, actions: {self.actions}," \
-               f"experiment_config: {self.experiment_config}, avg_R: {self.avg_R}"
+               f"experiment_config: {self.experiment_config}, avg_R: {self.avg_R}, policy_type: {self.policy_type}"
 
     def to_json_str(self) -> str:
         """
         Converts the DTO into a json string
 
         :return: the json string representation of the DTO
         """
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/training/multi_threshold_stopping_policy.py` & `csle_common-0.2.0/src/csle_common/dao/training/multi_threshold_stopping_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from csle_common.dao.training.policy import Policy
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.dao.simulation_config.state import State
 from csle_common.dao.simulation_config.state_type import StateType
 from csle_common.dao.training.player_type import PlayerType
 from csle_common.dao.simulation_config.action import Action
 from csle_common.dao.training.experiment_config import ExperimentConfig
+from csle_common.dao.training.policy_type import PolicyType
 
 
 class MultiThresholdStoppingPolicy(Policy):
     """
     A multi-threshold stopping policy
     """
 
@@ -40,14 +41,15 @@
         self.simulation_name = simulation_name
         self.L = L
         self.states = states
         self.actions = actions
         self.experiment_config = experiment_config
         self.avg_R = avg_R
         self.opponent_strategy = opponent_strategy
+        self.policy_type = PolicyType.MULTI_THRESHOLD
 
     def action(self, o: List[float]) -> int:
         """
         Multi-threshold stopping policy
 
         :param o: the current observation
         :return: the selected action
@@ -229,14 +231,15 @@
         d["agent_type"] = self.agent_type
         d["L"] = self.L
         if self.experiment_config is not None:
             d["experiment_config"] = self.experiment_config.to_dict()
         else:
             d["experiment_config"] = None
         d["avg_R"] = self.avg_R
+        d["policy_type"] = self.policy_type
         return d
 
     @staticmethod
     def from_dict(d: Dict) -> "MultiThresholdStoppingPolicy":
         """
         Converst a dict representation of the object to an instance
 
@@ -294,15 +297,15 @@
     def __str__(self) -> str:
         """
         :return: a string representation of the object
         """
         return f"theta: {self.theta}, id: {self.id}, simulation_name: {self.simulation_name}, " \
                f"thresholds: {self.thresholds()}, player_type: {self.player_type}, " \
                f"L:{self.L}, states: {self.states}, agent_type: {self.agent_type}, actions: {self.actions}," \
-               f"experiment_config: {self.experiment_config}, avg_R: {self.avg_R}"
+               f"experiment_config: {self.experiment_config}, avg_R: {self.avg_R}, policy_type: {self.policy_type}"
 
     def to_json_str(self) -> str:
         """
         Converts the DTO into a json string
 
         :return: the json string representation of the DTO
         """
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/training/policy.py` & `csle_common-0.2.0/src/csle_common/dao/training/policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/dao/training/ppo_policy.py` & `csle_common-0.2.0/src/csle_common/dao/training/linear_threshold_stopping_policy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,165 +1,157 @@
-from typing import List, Dict, Union
-import numpy as np
-import torch
+from typing import List, Dict, Tuple, Union, Optional
 import math
-from stable_baselines3 import PPO
+import numpy as np
 from csle_common.dao.training.policy import Policy
 from csle_common.dao.training.agent_type import AgentType
-from csle_common.dao.training.player_type import PlayerType
 from csle_common.dao.simulation_config.state import State
-from csle_common.dao.simulation_config.state_type import StateType
+from csle_common.dao.training.player_type import PlayerType
 from csle_common.dao.simulation_config.action import Action
 from csle_common.dao.training.experiment_config import ExperimentConfig
-from csle_common.logging.log import Logger
+from csle_common.dao.training.policy_type import PolicyType
 
 
-class PPOPolicy(Policy):
+class LinearThresholdStoppingPolicy(Policy):
     """
-    A neural network policy learned with PPO
+    A linear threshold stopping policy
     """
 
-    def __init__(self, model, simulation_name: str, save_path: str, player_type: PlayerType, states: List[State],
-                 actions: List[Action], experiment_config: ExperimentConfig, avg_R: float):
+    def __init__(self, theta, simulation_name: str, L: int, states: List[State], player_type: PlayerType,
+                 actions: List[Action], experiment_config: Optional[ExperimentConfig], avg_R: float,
+                 agent_type: AgentType, opponent_strategy: Optional["LinearThresholdStoppingPolicy"] = None) -> None:
         """
         Initializes the policy
 
-        :param model: the PPO model
+        :param theta: the threshold vector
         :param simulation_name: the simulation name
-        :param save_path: the path to save the model to
+        :param attacker: whether it is an attacker or not
+        :param L: the number of stop actions
         :param states: list of states (required for computing stage policies)
         :param actions: list of actions
-        :param experiment_config: the experiment configuration for training the policy
+        :param experiment_config: the experiment configuration used for training the policy
         :param avg_R: the average reward of the policy when evaluated in the simulation
+        :param agent_type: the agent type
+        :param opponent_strategy: optionally an opponent strategy
         """
-        super(PPOPolicy, self).__init__(agent_type=AgentType.PPO, player_type=player_type)
-        self.model = model
+        super(LinearThresholdStoppingPolicy, self).__init__(agent_type=agent_type, player_type=player_type)
+        self.theta = theta
         self.id = -1
         self.simulation_name = simulation_name
-        self.save_path = save_path
-        if self.model is None:
-            try:
-                self.model = PPO.load(path=self.save_path)
-            except Exception as e:
-                Logger.__call__().get_logger().warning(
-                    f"There was an exception loading the model from path: {self.save_path}, "
-                    f"exception: {str(e)}, {repr(e)}")
+        self.L = L
         self.states = states
         self.actions = actions
         self.experiment_config = experiment_config
         self.avg_R = avg_R
+        self.opponent_strategy = opponent_strategy
+        self.policy_type = PolicyType.MULTI_THRESHOLD
 
-    def action(self, o: List[float]) -> Union[int, List[int], np.ndarray]:
+    def action(self, o: List[float]) -> int:
         """
         Multi-threshold stopping policy
 
         :param o: the current observation
         :return: the selected action
         """
-        a, _ = self.model.predict(np.array(o), deterministic=False)
-        return a
+        if self.player_type == PlayerType.DEFENDER:
+            a, _ = self._defender_action(o=o)
+            return a
+        else:
+            raise NotImplementedError("Attacker not implemented yet")
 
-    def probability(self, o: List[float], a) -> Union[int, List[int], np.ndarray]:
+    def probability(self, o: List[float], a: int) -> int:
         """
-        Multi-threshold stopping policy
+        Probability of a given action
 
         :param o: the current observation
-        :return: the selected action
+        :param a: a given action
+        :return: the probability of a
+        """
+        if self.player_type == PlayerType.DEFENDER:
+            _, prob = self._defender_action(o=o)
+            return prob
+        else:
+            raise NotImplementedError("Attacker not implemented yet")
+
+    def stage_policy(self, o: Union[List[Union[int, float]], int, float]) -> List[List[float]]:
+        """
+        Gets the stage policy, i.e a |S|x|A| policy
+
+        :param o: the latest observation
+        :return: the |S|x|A| stage policy
+        """
+        raise NotImplementedError("Not implemented")
+
+    def _defender_action(self, o) -> Tuple[int, float]:
+        """
+        Linear threshold stopping policy of the defender
+
+        :param o: the input observation
+        :return: the selected action (int) and its probability
         """
-        actions, values, log_prob = self.model.policy.forward(obs=torch.tensor(o).to(self.model.device))
-        action = actions[0]
-        if action == a:
-            return math.exp(log_prob)
+        coefficients = np.zeros(len(self.theta))
+        theta = self.theta
+        coefficients[-1] = math.pow(theta[-1], 2)
+        coefficients[-2] = 1 + math.pow(theta[-2], 2)
+        for i in range(0, len(theta) - 2):
+            coefficients[i] = coefficients[-2] * math.pow(math.sin(theta[i]), 2)
+        belief = o
+        x = np.append(np.array([0, 1]), np.array(coefficients))
+        y = np.append(np.array(belief), np.array([-1]))
+        d = np.dot(x, y)
+        if d > 0:
+            return 1, 1
         else:
-            return 0
+            return 0, 1
 
-    def to_dict(self) -> Dict[str, Union[float, int, str]]:
+    def to_dict(self) -> Dict[str, List[float]]:
         """
         :return: a dict representation of the policy
         """
         d = {}
+        d["theta"] = self.theta
         d["id"] = self.id
         d["simulation_name"] = self.simulation_name
-        d["save_path"] = self.save_path
-        if self.model is not None:
-            d["policy_kwargs"] = self.model.policy_kwargs
-            self.model.save(path=self.save_path)
-        else:
-            d["policy_kwargs"] = {}
-            d["policy_kwargs"]["net_arch"] = []
         d["states"] = list(map(lambda x: x.to_dict(), self.states))
-        d["player_type"] = self.player_type
         d["actions"] = list(map(lambda x: x.to_dict(), self.actions))
-        d["experiment_config"] = self.experiment_config.to_dict()
+        d["player_type"] = self.player_type
         d["agent_type"] = self.agent_type
+        d["L"] = self.L
+        if self.experiment_config is not None:
+            d["experiment_config"] = self.experiment_config.to_dict()
+        else:
+            d["experiment_config"] = None
         d["avg_R"] = self.avg_R
+        d["policy_type"] = self.policy_type
         return d
 
     @staticmethod
-    def from_dict(d: Dict) -> "PPOPolicy":
+    def from_dict(d: Dict) -> "LinearThresholdStoppingPolicy":
         """
         Converst a dict representation of the object to an instance
 
         :param d: the dict to convert
         :return: the created instance
         """
-        obj = PPOPolicy(model=None, simulation_name=d["simulation_name"], save_path=d["save_path"],
-                        states=list(map(lambda x: State.from_dict(x), d["states"])), player_type=d["player_type"],
-                        actions=list(map(lambda x: Action.from_dict(x), d["actions"])),
-                        experiment_config=ExperimentConfig.from_dict(d["experiment_config"]), avg_R=d["avg_R"])
+        obj = LinearThresholdStoppingPolicy(
+            theta=d["theta"], simulation_name=d["simulation_name"], L=d["L"],
+            states=list(map(lambda x: State.from_dict(x), d["states"])), player_type=d["player_type"],
+            actions=list(map(lambda x: Action.from_dict(x), d["actions"])),
+            experiment_config=ExperimentConfig.from_dict(d["experiment_config"]), avg_R=d["avg_R"],
+            agent_type=d["agent_type"])
         obj.id = d["id"]
         return obj
 
-    def stage_policy(self, o: Union[List[Union[int, float]], int, float]) -> List[List[float]]:
-        """
-        Gets the stage policy, i.e a |S|x|A| policy
-
-        :param o: the latest observation
-        :return: the |S|x|A| stage policy
-        """
-        b1 = o[1]
-        l = int(o[0])
-        if not self.player_type == PlayerType.ATTACKER:
-            stage_policy = []
-            for _ in self.states:
-                stage_policy.append(self._get_attacker_dist(obs=o))
-            return stage_policy
-        else:
-            stage_policy = []
-            for s in self.states:
-                if s.state_type != StateType.TERMINAL:
-                    o = [l, b1, s.id]
-                    stage_policy.append(self._get_attacker_dist(obs=o))
-                else:
-                    stage_policy.append([0.5, 0.5])
-            return stage_policy
-
-    def _get_attacker_dist(self, obs) -> List[float]:
-        """
-        Utility function for getting the action distribution conditioned on a given observation
-
-        :param obs: the observation to condition on
-        :return: the conditional ation distribution
-        """
-        obs = np.array([obs])
-        actions, values, log_prob = self.model.policy.forward(obs=torch.tensor(obs).to(self.model.device))
-        action = actions[0]
-        if action == 1:
-            stop_prob = math.exp(log_prob)
-        else:
-            stop_prob = 1 - math.exp(log_prob)
-        return [1 - stop_prob, stop_prob]
-
     def __str__(self) -> str:
         """
         :return: a string representation of the object
         """
-        return f"model: {self.model}, id: {self.id}, simulation_name: {self.simulation_name}, " \
-               f"save path: {self.save_path}, states: {self.states}, experiment_config: {self.experiment_config}," \
-               f"avg_R: {self.avg_R}"
+        return f"theta: {self.theta}, id: {self.id}, simulation_name: {self.simulation_name}, " \
+               f"player_type: {self.player_type}, " \
+               f"L:{self.L}, states: {self.states}, agent_type: {self.agent_type}, actions: {self.actions}," \
+               f"experiment_config: {self.experiment_config}, avg_R: {self.avg_R}, policy_type: {self.policy_type}"
 
     def to_json_str(self) -> str:
         """
         Converts the DTO into a json string
 
         :return: the json string representation of the DTO
         """
@@ -176,25 +168,25 @@
         """
         import io
         json_str = self.to_json_str()
         with io.open(json_file_path, 'w', encoding='utf-8') as f:
             f.write(json_str)
 
     @staticmethod
-    def from_json_file(json_file_path: str) -> "PPOPolicy":
+    def from_json_file(json_file_path: str) -> "LinearThresholdStoppingPolicy":
         """
         Reads a json file and converts it to a DTO
 
         :param json_file_path: the json file path
         :return: the converted DTO
         """
         import io
         import json
         with io.open(json_file_path, 'r') as f:
             json_str = f.read()
-        return PPOPolicy.from_dict(json.loads(json_str))
+        return LinearThresholdStoppingPolicy.from_dict(json.loads(json_str))
 
-    def copy(self) -> "PPOPolicy":
+    def copy(self) -> "LinearThresholdStoppingPolicy":
         """
         :return: a copy of the DTO
         """
         return self.from_dict(self.to_dict())
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/training/random_policy.py` & `csle_common-0.2.0/src/csle_common/dao/training/random_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Union, List, Dict, Optional, Tuple
 import random
 import numpy as np
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.dao.training.player_type import PlayerType
 from csle_common.dao.training.policy import Policy
 from csle_common.dao.simulation_config.action import Action
+from csle_common.dao.training.policy_type import PolicyType
 
 
 class RandomPolicy(Policy):
     """
     Object representing a static policy
     """
 
@@ -20,14 +21,15 @@
         :param actions: list of actions
         :param player_type: the player type
         :param stage_policy_tensor: the stage policy tensor
         """
         super(RandomPolicy, self).__init__(agent_type=AgentType.RANDOM, player_type=player_type)
         self.actions = actions
         self.stage_policy_tensor = stage_policy_tensor
+        self.policy_type = PolicyType.RANDOM
 
     def action(self, o: Union[List[Union[int, float]], int, float]) -> Union[int, float]:
         """
         Selects the next action
 
         :param o: the input observation
         :return: the next action and its probability
@@ -71,14 +73,15 @@
         :return: A dict representation of the function
         """
         d = {}
         d["agent_type"] = self.agent_type
         d["player_type"] = self.player_type
         d["actions"] = list(map(lambda x: x.to_dict(), self.actions))
         d["stage_policy_tensor"] = self.stage_policy_tensor
+        d["policy_type"] = self.policy_type
         return d
 
     def stage_policy(self, o: Union[List[Union[int, float]], int, float]) -> List[List[float]]:
         """
         Gets the stage policy, i.e a |S|x|A| policy
 
         :param o: the latest observation
@@ -87,15 +90,16 @@
         return np.array(self.stage_policy_tensor)
 
     def __str__(self) -> str:
         """
         :return: a string representation of the policy
         """
         return f"agent_type: {self.agent_type}, player_type: {self.player_type}, " \
-               f"actions: {list(map(lambda x: str(x), self.actions))}, stage_policy_tensor: {self.stage_policy_tensor}"
+               f"actions: {list(map(lambda x: str(x), self.actions))}, " \
+               f"stage_policy_tensor: {self.stage_policy_tensor}, policy_type: {self.policy_type}"
 
     def to_json_str(self) -> str:
         """
         Converts the DTO into a json string
 
         :return: the json string representation of the DTO
         """
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/training/tabular_policy.py` & `csle_common-0.2.0/src/csle_common/dao/training/tabular_policy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Union, List, Dict, Any, Optional
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.dao.training.player_type import PlayerType
 from csle_common.dao.training.policy import Policy
 from csle_common.dao.simulation_config.action import Action
+from csle_common.dao.training.policy_type import PolicyType
 
 
 class TabularPolicy(Policy):
     """
     Object representing a tabular policy
     """
 
@@ -28,14 +29,15 @@
         self.actions = actions
         self.lookup_table = lookup_table
         self.value_function = value_function
         self.q_table = q_table
         self.simulation_name = simulation_name
         self.id = -1
         self.avg_R = avg_R
+        self.policy_type = PolicyType.TABULAR
 
     def action(self, o: Union[List[Union[int, float]], int, float]) -> Union[int, float]:
         """
         Selects the next action
 
         :param o: the input observation
         :return: the next action and its probability
@@ -79,14 +81,15 @@
         d["actions"] = list(map(lambda x: x.to_dict(), self.actions))
         d["lookup_table"] = self.lookup_table
         d["value_function"] = self.value_function
         d["simulation_name"] = self.simulation_name
         d["id"] = self.id
         d["avg_R"] = self.avg_R
         d["q_table"] = self.q_table
+        d["policy_type"] = self.policy_type
         return d
 
     def stage_policy(self, o: Union[List[Union[int, float]], int, float]) -> List[List[float]]:
         """
         Gets the stage policy, i.e a |S|x|A| policy
 
         :param o: the latest observation
@@ -97,15 +100,15 @@
     def __str__(self) -> str:
         """
         :return: a string representation of the policy
         """
         return f"agent_type: {self.agent_type}, player_type: {self.player_type}, " \
                f"actions: {list(map(lambda x: str(x), self.actions))}, lookup_table: {self.lookup_table}, " \
                f"value_function: {self.value_function}, simulation_name: {self.simulation_name}, id: {self.id}, " \
-               f"avg_R: {self.avg_R}, q_table: {self.q_table}"
+               f"avg_R: {self.avg_R}, q_table: {self.q_table}, policy_type: {self.policy_type}"
 
     def to_json_str(self) -> str:
         """
         Converts the DTO into a json string
 
         :return: the json string representation of the DTO
         """
```

### Comparing `csle_common-0.1.9/src/csle_common/dao/training/vector_policy.py` & `csle_common-0.2.0/src/csle_common/dao/training/vector_policy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Union, List, Dict
 import numpy as np
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.dao.training.player_type import PlayerType
 from csle_common.dao.training.policy import Policy
+from csle_common.dao.training.policy_type import PolicyType
 
 
 class VectorPolicy(Policy):
     """
     Object representing a tabular policy
     """
 
@@ -23,14 +24,15 @@
         """
         super(VectorPolicy, self).__init__(agent_type=agent_type, player_type=player_type)
         self.actions = actions
         self.policy_vector = policy_vector
         self.simulation_name = simulation_name
         self.id = -1
         self.avg_R = avg_R
+        self.policy_type = PolicyType.VECTOR
 
     def action(self, o: Union[List[Union[int, float]], int, float]) -> Union[int, float]:
         """
         Selects the next action
 
         :param o: the input observation
         :return: the next action and its probability
@@ -71,14 +73,15 @@
         d["agent_type"] = self.agent_type
         d["player_type"] = self.player_type
         d["actions"] = self.actions
         d["policy_vector"] = self.policy_vector
         d["simulation_name"] = self.simulation_name
         d["id"] = self.id
         d["avg_R"] = self.avg_R
+        d["policy_type"] = self.policy_type
         return d
 
     def stage_policy(self, o: Union[List[Union[int, float]], int, float]) -> List[float]:
         """
         Gets the stage policy, i.e a |S|x|A| policy
 
         :param o: the latest observation
@@ -89,15 +92,15 @@
     def __str__(self) -> str:
         """
         :return: a string representation of the policy
         """
         return f"agent_type: {self.agent_type}, player_type: {self.player_type}, " \
                f"actions: {list(map(lambda x: str(x), self.actions))}, policy_vector: {self.policy_vector}, " \
                f"simulation_name: {self.simulation_name}, id: {self.id}, " \
-               f"avg_R: {self.avg_R}"
+               f"avg_R: {self.avg_R}, type: {self.policy_type}"
 
     def to_json_str(self) -> str:
         """
         Converts the DTO into a json string
 
         :return: the json string representation of the DTO
         """
```

### Comparing `csle_common-0.1.9/src/csle_common/logging/custom_formatter.py` & `csle_common-0.2.0/src/csle_common/logging/custom_formatter.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/logging/log.py` & `csle_common-0.2.0/src/csle_common/logging/log.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/metastore/metastore_facade.py` & `csle_common-0.2.0/src/csle_common/metastore/metastore_facade.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from csle_common.dao.emulation_config.emulation_trace import EmulationTrace
 from csle_common.dao.simulation_config.simulation_trace import SimulationTrace
 from csle_common.dao.emulation_config.emulation_simulation_trace import EmulationSimulationTrace
 from csle_common.logging.log import Logger
 from csle_common.dao.system_identification.emulation_statistics import EmulationStatistics
 from csle_common.dao.training.experiment_execution import ExperimentExecution
 from csle_common.dao.training.multi_threshold_stopping_policy import MultiThresholdStoppingPolicy
+from csle_common.dao.training.linear_threshold_stopping_policy import LinearThresholdStoppingPolicy
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
 from csle_common.dao.jobs.data_collection_job_config import DataCollectionJobConfig
 from csle_common.dao.jobs.system_identification_job_config import SystemIdentificationJobConfig
 from csle_common.dao.system_identification.gaussian_mixture_system_model import GaussianMixtureSystemModel
 from csle_common.dao.system_identification.empirical_system_model import EmpiricalSystemModel
 from csle_common.dao.system_identification.gp_system_model import GPSystemModel
 from csle_common.dao.encoding.np_encoder import NpEncoder
@@ -27,14 +28,15 @@
 from csle_common.dao.training.vector_policy import VectorPolicy
 from csle_common.dao.emulation_config.emulation_execution import EmulationExecution
 from csle_common.dao.management.management_user import ManagementUser
 from csle_common.dao.management.session_token import SessionToken
 from csle_common.dao.datasets.traces_dataset import TracesDataset
 from csle_common.dao.datasets.statistics_dataset import StatisticsDataset
 from csle_common.dao.emulation_config.config import Config
+from csle_common.util.general_util import GeneralUtil
 
 
 class MetastoreFacade:
     """
     Facade for the metastore, contains methods for querying the metastore
     """
 
@@ -381,17 +383,21 @@
         Logger.__call__().get_logger().debug(f"Installing emulation trace for "
                                              f"emulation:{emulation_trace.emulation_name} in the metastore")
         with psycopg.connect(f"{constants.METADATA_STORE.DB_NAME_PROPERTY}={constants.METADATA_STORE.DBNAME} "
                              f"{constants.METADATA_STORE.USER_PROPERTY}={constants.METADATA_STORE.USER} "
                              f"{constants.METADATA_STORE.PW_PROPERTY}={constants.METADATA_STORE.PASSWORD} "
                              f"{constants.METADATA_STORE.HOST_PROPERTY}={constants.METADATA_STORE.HOST}") as conn:
             with conn.cursor() as cur:
+                # Need to manually set the ID since CITUS does not handle serial columns on distributed tables properly
+                id = GeneralUtil.get_latest_table_id(cur=cur,
+                                                     table_name=constants.METADATA_STORE.EMULATION_TRACES_TABLE)
                 config_json_str = json.dumps(emulation_trace.to_dict(), indent=4, sort_keys=True, cls=NpEncoder)
-                cur.execute(f"INSERT INTO {constants.METADATA_STORE.EMULATION_TRACES_TABLE} (emulation_name, trace) "
-                            f"VALUES (%s, %s) RETURNING id", (emulation_trace.emulation_name, config_json_str))
+                cur.execute(f"INSERT INTO {constants.METADATA_STORE.EMULATION_TRACES_TABLE} "
+                            f"(id, emulation_name, trace) "
+                            f"VALUES (%s, %s, %s) RETURNING id", (id, emulation_trace.emulation_name, config_json_str))
                 id_of_new_row = cur.fetchone()[0]
                 conn.commit()
                 Logger.__call__().get_logger().debug(f"Emulation trace for "
                                                      f"emulation {emulation_trace.emulation_name} saved successfully")
                 return id_of_new_row
 
     @staticmethod
@@ -406,19 +412,23 @@
                                              f"for emulation:{emulation_statistics.emulation_name} in the metastore")
         emulation_statistics.compute_descriptive_statistics_and_distributions()
         with psycopg.connect(f"{constants.METADATA_STORE.DB_NAME_PROPERTY}={constants.METADATA_STORE.DBNAME} "
                              f"{constants.METADATA_STORE.USER_PROPERTY}={constants.METADATA_STORE.USER} "
                              f"{constants.METADATA_STORE.PW_PROPERTY}={constants.METADATA_STORE.PASSWORD} "
                              f"{constants.METADATA_STORE.HOST_PROPERTY}={constants.METADATA_STORE.HOST}") as conn:
             with conn.cursor() as cur:
+                # Need to manually set the ID since CITUS does not handle serial columns on distributed tables properly
+                id = GeneralUtil.get_latest_table_id(cur=cur,
+                                                     table_name=constants.METADATA_STORE.EMULATION_STATISTICS_TABLE)
                 config_json_str = json.dumps(emulation_statistics.to_dict(), indent=4, sort_keys=True, cls=NpEncoder)
                 cur.execute(f"INSERT INTO "
                             f"{constants.METADATA_STORE.EMULATION_STATISTICS_TABLE} "
-                            f"(emulation_name, statistics) "
-                            f"VALUES (%s, %s) RETURNING id", (emulation_statistics.emulation_name, config_json_str))
+                            f"(id, emulation_name, statistics) "
+                            f"VALUES (%s, %s, %s) RETURNING id", (id, emulation_statistics.emulation_name,
+                                                                  config_json_str))
                 id_of_new_row = cur.fetchone()[0]
                 conn.commit()
                 Logger.__call__().get_logger().debug(f"Statistics for emulation "
                                                      f"{emulation_statistics.emulation_name} saved successfully")
                 return id_of_new_row
 
     @staticmethod
@@ -1327,21 +1337,24 @@
         """
         Logger.__call__().get_logger().debug("Saving a data collection job in the metastore")
         with psycopg.connect(f"{constants.METADATA_STORE.DB_NAME_PROPERTY}={constants.METADATA_STORE.DBNAME} "
                              f"{constants.METADATA_STORE.USER_PROPERTY}={constants.METADATA_STORE.USER} "
                              f"{constants.METADATA_STORE.PW_PROPERTY}={constants.METADATA_STORE.PASSWORD} "
                              f"{constants.METADATA_STORE.HOST_PROPERTY}={constants.METADATA_STORE.HOST}") as conn:
             with conn.cursor() as cur:
+                # Need to manually set the ID since CITUS does not handle serial columns on distributed tables properly
+                id = GeneralUtil.get_latest_table_id(cur=cur,
+                                                     table_name=constants.METADATA_STORE.DATA_COLLECTION_JOBS_TABLE)
                 data_collection_job_json = json.dumps(data_collection_job.to_dict(), indent=4,
                                                       sort_keys=True, cls=NpEncoder)
                 cur.execute(f"INSERT INTO {constants.METADATA_STORE.DATA_COLLECTION_JOBS_TABLE} "
-                            f"(config, emulation_name, pid) "
-                            f"VALUES (%s, %s, %s) RETURNING id", (data_collection_job_json,
-                                                                  data_collection_job.emulation_env_name,
-                                                                  data_collection_job.pid))
+                            f"(id, config, emulation_name, pid) "
+                            f"VALUES (%s, %s, %s, %s) RETURNING id",
+                            (id, data_collection_job_json, data_collection_job.emulation_env_name,
+                             data_collection_job.pid))
                 id_of_new_row = cur.fetchone()[0]
                 conn.commit()
                 Logger.__call__().get_logger().debug("Data collection job saved successfully")
                 return id_of_new_row
 
     @staticmethod
     def update_training_job(training_job: TrainingJobConfig, id: int) -> None:
@@ -3610,7 +3623,124 @@
                              f"{constants.METADATA_STORE.PW_PROPERTY}={constants.METADATA_STORE.PASSWORD} "
                              f"{constants.METADATA_STORE.HOST_PROPERTY}={constants.METADATA_STORE.HOST}") as conn:
             with conn.cursor() as cur:
                 cur.execute(f"DELETE FROM {constants.METADATA_STORE.CONFIG_TABLE} WHERE id = %s", (config.id,))
                 conn.commit()
                 Logger.__call__().get_logger().debug(f"Config with "
                                                      f"id {config.id} deleted successfully")
+
+    @staticmethod
+    def list_linear_threshold_stopping_policies() -> List[LinearThresholdStoppingPolicy]:
+        """
+        :return: A list of Linear-threshold stopping policies in the metastore
+        """
+        with psycopg.connect(f"{constants.METADATA_STORE.DB_NAME_PROPERTY}={constants.METADATA_STORE.DBNAME} "
+                             f"{constants.METADATA_STORE.USER_PROPERTY}={constants.METADATA_STORE.USER} "
+                             f"{constants.METADATA_STORE.PW_PROPERTY}={constants.METADATA_STORE.PASSWORD} "
+                             f"{constants.METADATA_STORE.HOST_PROPERTY}={constants.METADATA_STORE.HOST}") as conn:
+            with conn.cursor() as cur:
+                cur.execute(f"SELECT * FROM {constants.METADATA_STORE.LINEAR_THRESHOLD_STOPPING_POLICIES_TABLE}")
+                records = cur.fetchall()
+                records = list(map(lambda x: MetastoreFacade._convert_linear_threshold_stopping_policy_record_to_dto(x),
+                                   records))
+                return records
+
+    @staticmethod
+    def list_linear_threshold_stopping_policies_ids() -> List[Dict]:
+        """
+        :return: A list of Linear-threshold stopping policies ids in the metastore
+        """
+        with psycopg.connect(f"{constants.METADATA_STORE.DB_NAME_PROPERTY}={constants.METADATA_STORE.DBNAME} "
+                             f"{constants.METADATA_STORE.USER_PROPERTY}={constants.METADATA_STORE.USER} "
+                             f"{constants.METADATA_STORE.PW_PROPERTY}={constants.METADATA_STORE.PASSWORD} "
+                             f"{constants.METADATA_STORE.HOST_PROPERTY}={constants.METADATA_STORE.HOST}") as conn:
+            with conn.cursor() as cur:
+                cur.execute(f"SELECT id,simulation_name FROM "
+                            f"{constants.METADATA_STORE.LINEAR_THRESHOLD_STOPPING_POLICIES_TABLE}")
+                records = cur.fetchall()
+                return records
+
+    @staticmethod
+    def _convert_linear_threshold_stopping_policy_record_to_dto(linear_threshold_stopping_policy_record) \
+            -> LinearThresholdStoppingPolicy:
+        """
+        Converts a Linear-threshold stopping policy record fetched from the metastore into a DTO
+
+        :param linear_threshold_stopping_policy_record: the record to convert
+        :return: the DTO representing the record
+        """
+        linear_threshold_stopping_policy_json = json.dumps(linear_threshold_stopping_policy_record[1], indent=4,
+                                                           sort_keys=True)
+        linear_threshold_stopping_policy: LinearThresholdStoppingPolicy = LinearThresholdStoppingPolicy.from_dict(
+            json.loads(linear_threshold_stopping_policy_json))
+        linear_threshold_stopping_policy.id = linear_threshold_stopping_policy_record[0]
+        return linear_threshold_stopping_policy
+
+    @staticmethod
+    def get_linear_threshold_stopping_policy(id: int) -> Union[None, LinearThresholdStoppingPolicy]:
+        """
+        Function for fetching a mult-threshold policy with a given id from the metastore
+
+        :param id: the id of the linear-threshold policy
+        :return: The mult-threshold policy or None if it could not be found
+        """
+        with psycopg.connect(f"{constants.METADATA_STORE.DB_NAME_PROPERTY}={constants.METADATA_STORE.DBNAME} "
+                             f"{constants.METADATA_STORE.USER_PROPERTY}={constants.METADATA_STORE.USER} "
+                             f"{constants.METADATA_STORE.PW_PROPERTY}={constants.METADATA_STORE.PASSWORD} "
+                             f"{constants.METADATA_STORE.HOST_PROPERTY}={constants.METADATA_STORE.HOST}") as conn:
+            with conn.cursor() as cur:
+                cur.execute(f"SELECT * FROM {constants.METADATA_STORE.LINEAR_THRESHOLD_STOPPING_POLICIES_TABLE} "
+                            f"WHERE id = %s", (id,))
+                record = cur.fetchone()
+                if record is not None:
+                    record = MetastoreFacade._convert_linear_threshold_stopping_policy_record_to_dto(
+                        linear_threshold_stopping_policy_record=record)
+                return record
+
+    @staticmethod
+    def remove_linear_threshold_stopping_policy(
+            linear_threshold_stopping_policy: LinearThresholdStoppingPolicy) -> None:
+        """
+        Removes a linear-threshold stopping policy from the metastore
+
+        :param linear_threshold_stopping_policy: the policy to remove
+        :return: None
+        """
+        Logger.__call__().get_logger().debug(f"Removing Linear-threshold stopping policy with "
+                                             f"id:{linear_threshold_stopping_policy.id} from the metastore")
+        with psycopg.connect(f"{constants.METADATA_STORE.DB_NAME_PROPERTY}={constants.METADATA_STORE.DBNAME} "
+                             f"{constants.METADATA_STORE.USER_PROPERTY}={constants.METADATA_STORE.USER} "
+                             f"{constants.METADATA_STORE.PW_PROPERTY}={constants.METADATA_STORE.PASSWORD} "
+                             f"{constants.METADATA_STORE.HOST_PROPERTY}={constants.METADATA_STORE.HOST}") as conn:
+            with conn.cursor() as cur:
+                cur.execute(f"DELETE FROM {constants.METADATA_STORE.LINEAR_THRESHOLD_STOPPING_POLICIES_TABLE} "
+                            f"WHERE id = %s",
+                            (linear_threshold_stopping_policy.id,))
+                conn.commit()
+                Logger.__call__().get_logger().debug(f"Linear-threshold stopping policy "
+                                                     f"with id {linear_threshold_stopping_policy.id} "
+                                                     f"deleted successfully")
+
+    @staticmethod
+    def save_linear_threshold_stopping_policy(linear_threshold_stopping_policy: LinearThresholdStoppingPolicy) \
+            -> Union[Any, int]:
+        """
+        Saves a linear-threshold stopping policy to the metastore
+
+        :param linear_threshold_stopping_policy: the policy to save
+        :return: id of the created record
+        """
+        Logger.__call__().get_logger().debug("Installing a linear-threshold stopping policy in the metastore")
+        with psycopg.connect(f"{constants.METADATA_STORE.DB_NAME_PROPERTY}={constants.METADATA_STORE.DBNAME} "
+                             f"{constants.METADATA_STORE.USER_PROPERTY}={constants.METADATA_STORE.USER} "
+                             f"{constants.METADATA_STORE.PW_PROPERTY}={constants.METADATA_STORE.PASSWORD} "
+                             f"{constants.METADATA_STORE.HOST_PROPERTY}={constants.METADATA_STORE.HOST}") as conn:
+            with conn.cursor() as cur:
+                policy_json_str = json.dumps(linear_threshold_stopping_policy.to_dict(), indent=4, sort_keys=True)
+                cur.execute(f"INSERT INTO {constants.METADATA_STORE.LINEAR_THRESHOLD_STOPPING_POLICIES_TABLE} "
+                            f"(policy, simulation_name) "
+                            f"VALUES (%s, %s) RETURNING id", (policy_json_str,
+                                                              linear_threshold_stopping_policy.simulation_name))
+                id_of_new_row = cur.fetchone()[0]
+                conn.commit()
+                Logger.__call__().get_logger().debug("Linear-threshold policy saved successfully")
+                return id_of_new_row
```

### Comparing `csle_common-0.1.9/src/csle_common/models/fnn_w_softmax.py` & `csle_common-0.2.0/src/csle_common/models/fnn_w_softmax.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/tunneling/forward_ssh_controller.py` & `csle_common-0.2.0/src/csle_common/tunneling/forward_ssh_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/tunneling/forward_tunnel_thread.py` & `csle_common-0.2.0/src/csle_common/tunneling/forward_tunnel_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/util/cluster_util.py` & `csle_common-0.2.0/src/csle_common/util/cluster_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/util/connection_util.py` & `csle_common-0.2.0/src/csle_common/util/connection_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/util/docker_util.py` & `csle_common-0.2.0/src/csle_common/util/docker_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/util/emulation_util.py` & `csle_common-0.2.0/src/csle_common/util/emulation_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,17 +61,18 @@
         :param create_producer: boolean flag whether to create a producer from the csle-admin
         :return: None
         """
         action.execution_time = total_time
         record = action.to_kafka_record()
         if emulation_env_config.producer is None and create_producer:
             emulation_env_config.create_producer()
-        emulation_env_config.producer.produce(collector_constants.KAFKA_CONFIG.ATTACKER_ACTIONS_TOPIC_NAME, record)
-        emulation_env_config.producer.poll(0)
-        emulation_env_config.producer.flush()
+        if emulation_env_config.producer is not None:
+            emulation_env_config.producer.produce(collector_constants.KAFKA_CONFIG.ATTACKER_ACTIONS_TOPIC_NAME, record)
+            emulation_env_config.producer.poll(0)
+            emulation_env_config.producer.flush()
 
     @staticmethod
     def _check_if_ssh_server_is_running(conn, telnet: bool = False) -> bool:
         """
         Checks if an ssh server is running on the machine
 
         :param conn: the connection to use for the command
```

### Comparing `csle_common-0.1.9/src/csle_common/util/env_dynamics_util.py` & `csle_common-0.2.0/src/csle_common/util/env_dynamics_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,27 +57,25 @@
         """
         new_machines_obs = EnvDynamicsUtil.merge_duplicate_machines(machines=new_machines_obs, action=action)
         attacker_machine_observations = []
         # Add updated machines to merged state
         for n_m in new_machines_obs:
             if emulation_env_config.containers_config.agent_ip in n_m.ips:
                 continue
-            exists = False
             merged_m = n_m
             for i, o_m in enumerate(old_machines_obs):
-                if n_m.ips == o_m.ips:
+                if n_m.ips_match(o_m.ips):
                     merged_m = EnvDynamicsUtil.merge_new_machine_obs_with_old_machine_obs(o_m, n_m, action)
-                    exists = True
             attacker_machine_observations.append(merged_m)
 
         # Add old machines to merged state
         for o_m in old_machines_obs:
             exists = False
             for m_m in attacker_machine_observations:
-                if o_m.ips == m_m.ips:
+                if o_m.ips_match(m_m.ips):
                     exists = True
             if not exists:
                 attacker_machine_observations.append(o_m)
 
         return attacker_machine_observations
 
     @staticmethod
@@ -747,15 +745,21 @@
         :param machines: list of machines (possibly with duplicates)
         :param action: the action that generated the new machines
         :return: the merged set of machines
         """
         merged_machines = []
         ips: Set[str] = set()
         for m in machines:
+            ip_suffixes = list(map(lambda x: x.split(".")[-1], m.ips))
+            for m1 in machines:
+                for ip in m1.ips:
+                    if ip.split(".")[-1] in ip_suffixes and ip not in m.ips:
+                        m.ips = list(set(m.ips + m1.ips))
+        for m in machines:
             if not m.ips_match(list(ips)):
                 merged_m = m
                 for m2 in machines:
                     if m2.ips == merged_m.ips:
                         merged_m = EnvDynamicsUtil.merge_new_machine_obs_with_old_machine_obs(merged_m, m2, action)
                 merged_machines.append(merged_m)
-                ips.union(set(m.ips))
+                ips = ips.union(set(m.ips))
         return merged_machines
```

### Comparing `csle_common-0.1.9/src/csle_common/util/experiment_util.py` & `csle_common-0.2.0/src/csle_common/util/experiment_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/util/export_util.py` & `csle_common-0.2.0/src/csle_common/util/export_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         :param file_path: the full path of the resulting zip file
         :return: None
         """
         Logger.__call__().get_logger().info(f"Zipping directory: {dir_path} to file: {file_path}")
         with zipfile.ZipFile(file_path, 'w', zipfile.ZIP_DEFLATED) as zipf:
             for root, dirs, files in os.walk(dir_path):
                 for i, file in enumerate(files):
-                    Logger.__call__().get_logger().info(f"Processing file {i+1}/{len(files)}, file name: {file}")
+                    Logger.__call__().get_logger().info(f"Processing file {i + 1}/{len(files)}, file name: {file}")
                     zipf.write(os.path.join(root, file),
                                os.path.relpath(os.path.join(root, file),
                                                os.path.join(dir_path, '..')))
 
     @staticmethod
     def get_dir_size_gb(dir_path: str = '.') -> float:
         """
@@ -48,34 +48,36 @@
                 elif entry.is_dir():
                     total += ExportUtil.get_dir_size(entry.path)
         return round((float(total) / 1000000000), 2)
 
     @staticmethod
     def export_emulation_traces_to_disk_json(num_traces_per_file: int, output_dir: str, zip_file_output: str,
                                              max_num_traces: int, added_by: str = "unknown", offset: int = 0,
-                                             file_start_id: int = 1) -> None:
+                                             file_start_id: int = 1, emulation_traces_ids=None) -> None:
         """
         Exports emulation traces from the metastore to disk
 
         :param num_traces_per_file: the number of traces per file in the output directory
         :param output_dir: the output directory
         :param zip_file_output: the compressed zip file path
         :param max_num_traces: maximum number of traces
         :param added_by: the person who added the dataset
         :param offset: the trace id offset
         :param file_start_id: the id of the first file to write
+        :param emulation_traces_ids: the ids of the traces to export
         :return: None
         """
         Logger.__call__().get_logger().info(f"Exporting emulation traces to disk (json), output dir: {output_dir}, "
                                             f"output zip file: {zip_file_output}, "
                                             f"num traces per file: {num_traces_per_file}")
         if not os.path.exists(output_dir):
             os.makedirs(output_dir)
-        emulation_traces_ids = MetastoreFacade.list_emulation_traces_ids()
-        emulation_traces_ids = emulation_traces_ids[offset:]
+        if emulation_traces_ids is None:
+            emulation_traces_ids = MetastoreFacade.list_emulation_traces_ids()
+            emulation_traces_ids = emulation_traces_ids[offset:]
         if len(emulation_traces_ids) > max_num_traces:
             emulation_traces_ids = emulation_traces_ids[0:max_num_traces]
         traces = []
         file_id = file_start_id
         file_name = f"{file_id}.json"
         columns = ""
         last_export = 0
@@ -92,15 +94,15 @@
                     constants.METADATA_STORE.TRACES_PROPERTY: [
                         tr.schema().to_dict()
                     ]
                 }
 
             traces.append(tr.to_dict())
             if i > 0 and ((i % num_traces_per_file == 0) or i == (len(emulation_traces_ids) - 1)):
-                Logger.__call__().get_logger().info(f"Exporting traces {last_export+1}-{i} to file: {file_name}")
+                Logger.__call__().get_logger().info(f"Exporting traces {last_export + 1}-{i} to file: {file_name}")
                 traces_dict = {constants.METADATA_STORE.TRACES_PROPERTY: traces}
                 traces_str = json.dumps(traces_dict, indent=4, sort_keys=True)
                 with io.open(f"{output_dir}{constants.COMMANDS.SLASH_DELIM}{file_name}", 'w', encoding='utf-8') as f:
                     f.write(traces_str)
                 file_id += 1
                 file_name = f"{file_id}.json"
                 traces = []
@@ -220,15 +222,15 @@
             if num_attributes_per_time_step == -1:
                 num_attributes_per_time_step = tr.num_attributes_per_time_step()
             if columns is None:
                 columns = tr_labels
 
             traces.append(tr_values)
             if i > 0 and ((i % num_traces_per_file == 0) or i == (len(emulation_traces_ids) - 1)):
-                Logger.__call__().get_logger().info(f"Exporting traces {last_export+1}-{i} to file: {file_name}")
+                Logger.__call__().get_logger().info(f"Exporting traces {last_export + 1}-{i} to file: {file_name}")
                 with io.open(f"{output_dir}{constants.COMMANDS.SLASH_DELIM}{file_name}", 'w', encoding='utf-8') as f:
                     writer = csv.writer(f)
                     writer.writerow(columns)
                     for row in traces:
                         writer.writerow(row)
                 file_id += 1
                 file_name = f"{file_id}.csv"
```

### Comparing `csle_common-0.1.9/src/csle_common/util/grpc_util.py` & `csle_common-0.2.0/src/csle_common/util/grpc_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/util/import_util.py` & `csle_common-0.2.0/src/csle_common/util/import_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/util/management_util.py` & `csle_common-0.2.0/src/csle_common/util/management_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/util/plotting_util.py` & `csle_common-0.2.0/src/csle_common/util/plotting_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common/util/read_emulation_statistics_util.py` & `csle_common-0.2.0/src/csle_common/util/read_emulation_statistics_util.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from csle_ryu.dao.avg_flow_statistic import AvgFlowStatistic
 from csle_ryu.dao.agg_flow_statistic import AggFlowStatistic
 from csle_ryu.dao.flow_statistic import FlowStatistic
 from csle_ryu.dao.port_statistic import PortStatistic
 import csle_collector.constants.constants as collector_constants
 import csle_common.constants.constants as constants
 from csle_collector.snort_ids_manager.snort_ids_alert_counters import SnortIdsAlertCounters
+from csle_collector.snort_ids_manager.snort_ids_rule_counters import SnortIdsRuleCounters
+from csle_collector.snort_ids_manager.snort_ids_ip_alert_counters import SnortIdsIPAlertCounters
 from csle_collector.ossec_ids_manager.ossec_ids_alert_counters import OSSECIdsAlertCounters
 from csle_collector.client_manager.client_population_metrics import ClientPopulationMetrics
 from csle_collector.docker_stats_manager.docker_stats import DockerStats
 from csle_collector.host_manager.host_metrics import HostMetrics
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
 from csle_common.dao.emulation_action.attacker.emulation_attacker_action import EmulationAttackerAction
 from csle_common.dao.emulation_action.defender.emulation_defender_action import EmulationDefenderAction
@@ -37,14 +39,20 @@
         agg_docker_stats = []
         docker_host_stats = {}
         host_metrics = {}
         aggregated_host_metrics = []
         defender_actions = []
         attacker_actions = []
         snort_ids_metrics = []
+        snort_ids_ip_metrics = {}
+        snort_ids_rule_metrics = []
+        snort_alert_metrics_per_ids = {}
+        snort_rule_metrics_per_ids = {}
+        total_snort_metrics = []
+        total_snort_rule_metrics = []
         total_host_metrics = []
         ossec_host_ids_metrics = {}
         total_ossec_metrics = []
         aggregated_ossec_metrics = []
         openflow_flow_stats = []
         openflow_port_stats = []
         avg_openflow_flow_stats = []
@@ -55,45 +63,57 @@
         openflow_port_avg_metrics_per_switch = {}
         agg_openflow_flow_stats = []
         agg_openflow_flow_metrics_per_switch = {}
 
         num_ossec_containers = len(list(filter(lambda x: x.name in constants.CONTAINER_IMAGES.OSSEC_IDS_IMAGES,
                                                emulation_env_config.containers_config.containers)))
 
+        num_snort_containers = len(list(filter(lambda x: x.name in constants.CONTAINER_IMAGES.SNORT_IDS_IMAGES,
+                                               emulation_env_config.containers_config.containers)))
+
         for c in emulation_env_config.containers_config.containers:
             docker_host_stats[c.get_full_name()] = []
             host_metrics[c.get_full_name()] = []
             ossec_host_ids_metrics[c.get_full_name()] = []
+            snort_ids_ip_metrics[c.get_full_name()] = []
+            for ids_image in constants.CONTAINER_IMAGES.SNORT_IDS_IMAGES:
+                if ids_image in c.name:
+                    snort_alert_metrics_per_ids[c.get_full_name()] = []
+                    snort_rule_metrics_per_ids[c.get_full_name()] = []
 
         host_metrics[emulation_env_config.kafka_config.container.get_full_name()] = []
         docker_host_stats[emulation_env_config.kafka_config.container.get_full_name()] = []
         ossec_host_ids_metrics[emulation_env_config.kafka_config.container.get_full_name()] = []
+        snort_ids_ip_metrics[emulation_env_config.kafka_config.container.get_full_name()] = []
         host_metrics[emulation_env_config.elk_config.container.get_full_name()] = []
         docker_host_stats[emulation_env_config.elk_config.container.get_full_name()] = []
         ossec_host_ids_metrics[emulation_env_config.elk_config.container.get_full_name()] = []
+        snort_ids_ip_metrics[emulation_env_config.elk_config.container.get_full_name()] = []
         if emulation_env_config.sdn_controller_config is not None:
             host_metrics[emulation_env_config.sdn_controller_config.container.get_full_name()] = []
             docker_host_stats[emulation_env_config.sdn_controller_config.container.get_full_name()] = []
             ossec_host_ids_metrics[emulation_env_config.sdn_controller_config.container.get_full_name()] = []
+            snort_ids_ip_metrics[emulation_env_config.sdn_controller_config.container.get_full_name()] = []
 
         topic_names = [collector_constants.KAFKA_CONFIG.ATTACKER_ACTIONS_TOPIC_NAME,
                        collector_constants.KAFKA_CONFIG.DOCKER_HOST_STATS_TOPIC_NAME,
                        collector_constants.KAFKA_CONFIG.DEFENDER_ACTIONS_TOPIC_NAME,
                        collector_constants.KAFKA_CONFIG.DOCKER_STATS_TOPIC_NAME,
                        collector_constants.KAFKA_CONFIG.SNORT_IDS_LOG_TOPIC_NAME,
                        collector_constants.KAFKA_CONFIG.HOST_METRICS_TOPIC_NAME,
                        collector_constants.KAFKA_CONFIG.CLIENT_POPULATION_TOPIC_NAME,
                        collector_constants.KAFKA_CONFIG.OSSEC_IDS_LOG_TOPIC_NAME,
                        collector_constants.KAFKA_CONFIG.OPENFLOW_FLOW_STATS_TOPIC_NAME,
                        collector_constants.KAFKA_CONFIG.OPENFLOW_PORT_STATS_TOPIC_NAME,
                        collector_constants.KAFKA_CONFIG.AVERAGE_OPENFLOW_FLOW_STATS_PER_SWITCH_TOPIC_NAME,
                        collector_constants.KAFKA_CONFIG.AVERAGE_OPENFLOW_PORT_STATS_PER_SWITCH_TOPIC_NAME,
-                       collector_constants.KAFKA_CONFIG.OPENFLOW_AGG_FLOW_STATS_TOPIC_NAME
-                       ]
-        logger.info(f"Reading time-series data for the last {time_window_minutes} from topics: {topic_names}")
+                       collector_constants.KAFKA_CONFIG.OPENFLOW_AGG_FLOW_STATS_TOPIC_NAME,
+                       collector_constants.KAFKA_CONFIG.SNORT_IDS_IP_LOG_TOPIC_NAME,
+                       collector_constants.KAFKA_CONFIG.SNORT_IDS_RULE_LOG_TOPIC_NAME]
+        logger.info(f"Reading time-series data for the last {time_window_minutes} minutes from topics: {topic_names}")
         start_consume_ts = time.time()
         kafka_conf = {
             collector_constants.KAFKA.BOOTSTRAP_SERVERS_PROPERTY:
                 f"{emulation_env_config.kafka_config.container.docker_gw_bridge_ip}:"
                 f"{emulation_env_config.kafka_config.kafka_port_external}",
             collector_constants.KAFKA.GROUP_ID_PROPERTY: f"emulation_data_consumer_thread_{start_consume_ts}",
             collector_constants.KAFKA.AUTO_OFFSET_RESET_PROPERTY: collector_constants.KAFKA.EARLIEST_OFFSET}
@@ -112,14 +132,16 @@
             consumer.assign(time_offsets_partitions)
 
         consumer.subscribe(topic_names, on_assign=on_assign)
         done = False
         num_msg = 0
         host_metrics_counter = 0
         ossec_host_metrics_counter = 0
+        snort_metrics_counter = 0
+        snort_rule_metrics_counter = 0
         while not done:
             msg = consumer.poll(timeout=1.0)
             if msg is not None:
                 num_msg += 1
                 if msg.error():
                     if msg.error().code() == KafkaError._PARTITION_EOF:
                         logger.warning(f"reached end of partition: {msg.topic(), msg.partition(), msg.offset()}")
@@ -146,15 +168,25 @@
                     elif topic == collector_constants.KAFKA_CONFIG.DEFENDER_ACTIONS_TOPIC_NAME:
                         defender_actions.append(EmulationDefenderAction.from_kafka_record(record=msg.value().decode()))
                     elif topic == collector_constants.KAFKA_CONFIG.DOCKER_HOST_STATS_TOPIC_NAME:
                         stats = DockerStats.from_kafka_record(record=msg.value().decode())
                         c = emulation_env_config.get_container_from_ip(stats.ip)
                         docker_host_stats[c.get_full_name()].append(stats)
                     elif topic == collector_constants.KAFKA_CONFIG.SNORT_IDS_LOG_TOPIC_NAME:
-                        snort_ids_metrics.append(SnortIdsAlertCounters.from_kafka_record(record=msg.value().decode()))
+                        metrics = SnortIdsAlertCounters.from_kafka_record(record=msg.value().decode())
+                        c = emulation_env_config.get_container_from_ip(metrics.ip)
+                        snort_alert_metrics_per_ids[c.get_full_name()].append(metrics)
+                        snort_metrics_counter += 1
+                        total_snort_metrics.append(metrics)
+                    elif topic == collector_constants.KAFKA_CONFIG.SNORT_IDS_RULE_LOG_TOPIC_NAME:
+                        metrics = SnortIdsRuleCounters.from_kafka_record(record=msg.value().decode())
+                        c = emulation_env_config.get_container_from_ip(metrics.ip)
+                        snort_rule_metrics_per_ids[c.get_full_name()].append(metrics)
+                        snort_rule_metrics_counter += 1
+                        total_snort_rule_metrics.append(metrics)
                     elif topic == collector_constants.KAFKA_CONFIG.CLIENT_POPULATION_TOPIC_NAME:
                         client_metrics.append(ClientPopulationMetrics.from_kafka_record(record=msg.value().decode()))
                     elif topic == collector_constants.KAFKA_CONFIG.OPENFLOW_FLOW_STATS_TOPIC_NAME:
                         flow_metrics_record = FlowStatistic.from_kafka_record(record=msg.value().decode())
                         openflow_flow_stats.append(flow_metrics_record)
                         if str(flow_metrics_record.datapath_id) not in openflow_flow_metrics_per_switch:
                             openflow_flow_metrics_per_switch[str(flow_metrics_record.datapath_id)] = []
@@ -184,43 +216,64 @@
                     elif topic == collector_constants.KAFKA_CONFIG.OPENFLOW_AGG_FLOW_STATS_TOPIC_NAME:
                         agg_flow_statistics_record = AggFlowStatistic.from_kafka_record(record=msg.value().decode())
                         agg_openflow_flow_stats.append(agg_flow_statistics_record)
                         if str(agg_flow_statistics_record.datapath_id) not in agg_openflow_flow_metrics_per_switch:
                             agg_openflow_flow_metrics_per_switch[str(agg_flow_statistics_record.datapath_id)] = []
                         agg_openflow_flow_metrics_per_switch[str(agg_flow_statistics_record.datapath_id)].append(
                             agg_flow_statistics_record)
+                    elif topic == collector_constants.KAFKA_CONFIG.SNORT_IDS_IP_LOG_TOPIC_NAME:
+                        metrics = SnortIdsIPAlertCounters.from_kafka_record(record=msg.value().decode())
+                        c = emulation_env_config.get_container_from_ip(metrics.alert_ip)
+                        if c is not None:
+                            snort_ids_ip_metrics[c.get_full_name()].append(metrics)
                     if host_metrics_counter >= len(emulation_env_config.containers_config.containers):
                         agg_host_metrics_dto = ReadEmulationStatisticsUtil.average_host_metrics(
                             host_metrics=total_host_metrics)
                         aggregated_host_metrics.append(agg_host_metrics_dto)
                         host_metrics_counter = 0
                         total_host_metrics = []
                     if ossec_host_metrics_counter >= num_ossec_containers:
                         agg_ossec_metrics_dto = ReadEmulationStatisticsUtil.average_ossec_metrics(
                             ossec_metrics=total_ossec_metrics)
                         aggregated_ossec_metrics.append(agg_ossec_metrics_dto)
                         ossec_host_metrics_counter = 0
                         total_ossec_metrics = []
+                    if snort_metrics_counter >= num_snort_containers:
+                        agg_snort_metrics_dto = ReadEmulationStatisticsUtil.average_snort_metrics(
+                            snort_metrics=total_snort_metrics)
+                        snort_ids_metrics.append(agg_snort_metrics_dto)
+                        snort_metrics_counter = 0
+                        total_snort_metrics = []
+                    if snort_rule_metrics_counter >= num_snort_containers:
+                        agg_snort_rule_metrics_dto = ReadEmulationStatisticsUtil.average_snort_rule_metrics(
+                            snort_metrics=total_snort_rule_metrics)
+                        snort_ids_rule_metrics.append(agg_snort_rule_metrics_dto)
+                        snort_rule_metrics_counter = 0
+                        total_snort_rule_metrics = []
             else:
                 done = True
         consumer.close()
         dto = EmulationMetricsTimeSeries(
             client_metrics=client_metrics, aggregated_docker_stats=agg_docker_stats, host_metrics=host_metrics,
-            docker_host_stats=docker_host_stats, snort_ids_metrics=snort_ids_metrics, attacker_actions=attacker_actions,
+            docker_host_stats=docker_host_stats, agg_snort_ids_metrics=snort_ids_metrics,
+            attacker_actions=attacker_actions,
             defender_actions=defender_actions, aggregated_host_metrics=aggregated_host_metrics,
             emulation_env_config=emulation_env_config, aggregated_ossec_host_alert_counters=aggregated_ossec_metrics,
             ossec_host_alert_counters=ossec_host_ids_metrics,
             avg_openflow_flow_stats=avg_openflow_flow_stats, avg_openflow_port_stats=avg_openflow_port_stats,
             openflow_port_stats=openflow_port_stats, openflow_flow_stats=openflow_flow_stats,
             openflow_flow_metrics_per_switch=openflow_flow_metrics_per_switch,
             openflow_port_metrics_per_switch=openflow_port_metrics_per_switch,
             openflow_flow_avg_metrics_per_switch=openflow_flow_avg_metrics_per_switch,
             openflow_port_avg_metrics_per_switch=openflow_port_avg_metrics_per_switch,
             agg_openflow_flow_stats=agg_openflow_flow_stats,
-            agg_openflow_flow_metrics_per_switch=agg_openflow_flow_metrics_per_switch
+            agg_openflow_flow_metrics_per_switch=agg_openflow_flow_metrics_per_switch,
+            agg_snort_ids_rule_metrics=snort_ids_rule_metrics, snort_ids_ip_metrics=snort_ids_ip_metrics,
+            snort_rule_metrics_per_ids=snort_rule_metrics_per_ids,
+            snort_alert_metrics_per_ids=snort_alert_metrics_per_ids
         )
         return dto
 
     @staticmethod
     def average_host_metrics(host_metrics: List[HostMetrics]) -> HostMetrics:
         """
         Computes the average metrics from a list of host metrics
@@ -258,7 +311,33 @@
         :param ossec_metrics: the list of OSSEC metrics
         :return: the computed averages
         """
         aggregated_ossec_ids_alert_counters = OSSECIdsAlertCounters()
         for alert_counters in ossec_metrics:
             aggregated_ossec_ids_alert_counters.add(alert_counters)
         return aggregated_ossec_ids_alert_counters
+
+    @staticmethod
+    def average_snort_metrics(snort_metrics: List[SnortIdsAlertCounters]) -> SnortIdsAlertCounters:
+        """
+        Computes the average metrics from a list of Snort metrics
+
+        :param snort_metrics: the list of Snort metrics
+        :return: the computed averages
+        """
+        aggregated_snort_ids_alert_counters = SnortIdsAlertCounters()
+        for alert_counters in snort_metrics:
+            aggregated_snort_ids_alert_counters.add(alert_counters)
+        return aggregated_snort_ids_alert_counters
+
+    @staticmethod
+    def average_snort_rule_metrics(snort_metrics: List[SnortIdsRuleCounters]) -> SnortIdsRuleCounters:
+        """
+        Computes the average metrics from a list of Snort rule metrics
+
+        :param snort_metrics: the list of Snort rule metrics
+        :return: the computed averages
+        """
+        aggregated_snort_ids_rule_counters = SnortIdsRuleCounters()
+        for alert_counters in snort_metrics:
+            aggregated_snort_ids_rule_counters.add(alert_counters)
+        return aggregated_snort_ids_rule_counters
```

### Comparing `csle_common-0.1.9/src/csle_common/util/ssh_util.py` & `csle_common-0.2.0/src/csle_common/util/ssh_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.9/src/csle_common.egg-info/PKG-INFO` & `csle_common-0.2.0/src/csle_common.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-common
-Version: 0.1.9
+Version: 0.2.0
 Summary: Common functionality of the Cyber Security Learning Environment (CSLE)
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_common-0.1.9/src/csle_common.egg-info/SOURCES.txt` & `csle_common-0.2.0/src/csle_common.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 src/csle_common.egg-info/not-zip-safe
 src/csle_common.egg-info/requires.txt
 src/csle_common.egg-info/top_level.txt
 src/csle_common/constants/__init__.py
 src/csle_common/constants/constants.py
 src/csle_common/consumer_threads/__init__.py
 src/csle_common/consumer_threads/aggregated_host_metrics_thread.py
+src/csle_common/consumer_threads/aggregated_ossec_ids_log_consumer_thread.py
+src/csle_common/consumer_threads/aggregated_snort_ids_log_consumer_thread.py
+src/csle_common/consumer_threads/aggregated_snort_ids_rule_log_consumer_thread.py
 src/csle_common/consumer_threads/attacker_actions_consumer_thread.py
 src/csle_common/consumer_threads/avg_host_metrics_thread.py
 src/csle_common/consumer_threads/client_population_consumer_thread.py
 src/csle_common/consumer_threads/defender_actions_consumer_thread.py
 src/csle_common/consumer_threads/docker_host_stats_consumer_thread.py
 src/csle_common/consumer_threads/docker_stats_consumer_thread.py
 src/csle_common/consumer_threads/host_metrics_consumer_thread.py
@@ -216,18 +219,20 @@
 src/csle_common/dao/training/alpha_vectors_policy.py
 src/csle_common/dao/training/dqn_policy.py
 src/csle_common/dao/training/experiment_config.py
 src/csle_common/dao/training/experiment_execution.py
 src/csle_common/dao/training/experiment_result.py
 src/csle_common/dao/training/fnn_with_softmax_policy.py
 src/csle_common/dao/training/hparam.py
+src/csle_common/dao/training/linear_threshold_stopping_policy.py
 src/csle_common/dao/training/mixed_multi_threshold_stopping_policy.py
 src/csle_common/dao/training/multi_threshold_stopping_policy.py
 src/csle_common/dao/training/player_type.py
 src/csle_common/dao/training/policy.py
+src/csle_common/dao/training/policy_type.py
 src/csle_common/dao/training/ppo_policy.py
 src/csle_common/dao/training/random_policy.py
 src/csle_common/dao/training/tabular_policy.py
 src/csle_common/dao/training/vector_policy.py
 src/csle_common/logging/__init__.py
 src/csle_common/logging/custom_formatter.py
 src/csle_common/logging/log.py
```

