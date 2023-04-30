# Comparing `tmp/csle_collector-0.1.9.tar.gz` & `tmp/csle_collector-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_collector-0.1.9.tar", last modified: Tue Mar 21 08:09:08 2023, max compression
+gzip compressed data, was "csle_collector-0.2.0.tar", last modified: Sun Apr 30 12:36:11 2023, max compression
```

## Comparing `csle_collector-0.1.9.tar` & `csle_collector-0.2.0.tar`

### file list

```diff
@@ -1,92 +1,94 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.025203 csle_collector-0.1.9/
--rw-rw-r--   0 kim       (1000) kim       (1000)      803 2023-03-21 08:09:08.025203 csle_collector-0.1.9/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     5807 2023-03-04 17:48:16.000000 csle_collector-0.1.9/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      674 2023-02-11 20:28:41.000000 csle_collector-0.1.9/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1454 2023-03-21 08:09:08.025203 csle_collector-0.1.9/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2022-11-28 13:03:16.000000 csle_collector-0.1.9/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.009203 csle_collector-0.1.9/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.009203 csle_collector-0.1.9/src/csle_collector/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 csle_collector-0.1.9/src/csle_collector/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.013203 csle_collector-0.1.9/src/csle_collector/client_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/client_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    16588 2023-03-21 06:33:58.000000 csle_collector-0.1.9/src/csle_collector/client_manager/client_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4671 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/client_manager/client_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8592 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/client_manager/client_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2179 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/client_manager/client_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3633 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/client_manager/client_population_metrics.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4292 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/client_manager/query_clients.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.013203 csle_collector-0.1.9/src/csle_collector/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    33268 2023-03-21 07:35:53.000000 csle_collector-0.1.9/src/csle_collector/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.013203 csle_collector-0.1.9/src/csle_collector/docker_stats_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/docker_stats_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    12394 2023-03-17 07:49:22.000000 csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    13540 2023-03-06 06:25:37.000000 csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4589 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6193 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8801 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3994 2023-03-17 14:04:50.000000 csle_collector-0.1.9/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.017203 csle_collector-0.1.9/src/csle_collector/elk_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/elk_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10730 2023-03-21 06:33:58.000000 csle_collector-0.1.9/src/csle_collector/elk_manager/elk_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5923 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/elk_manager/elk_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    14300 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1540 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/elk_manager/elk_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5768 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/elk_manager/query_elk_server.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.017203 csle_collector-0.1.9/src/csle_collector/host_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/host_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      875 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/host_manager/failed_login_attempt.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    60179 2023-03-21 07:55:28.000000 csle_collector-0.1.9/src/csle_collector/host_manager/host_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    12978 2022-12-02 11:02:24.000000 csle_collector-0.1.9/src/csle_collector/host_manager/host_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    25786 2022-12-02 11:02:35.000000 csle_collector-0.1.9/src/csle_collector/host_manager/host_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    33850 2023-03-04 10:28:54.000000 csle_collector-0.1.9/src/csle_collector/host_manager/host_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7783 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/host_manager/host_metrics.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    15344 2022-12-02 15:50:47.000000 csle_collector-0.1.9/src/csle_collector/host_manager/query_host_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1292 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/host_manager/successful_login.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.017203 csle_collector-0.1.9/src/csle_collector/kafka_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/kafka_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6606 2023-03-21 06:33:58.000000 csle_collector-0.1.9/src/csle_collector/kafka_manager/kafka_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4116 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/kafka_manager/kafka_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8484 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1442 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/kafka_manager/kafka_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3233 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/kafka_manager/query_kafka_server.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.021203 csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2931 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10847 2023-03-17 07:49:22.000000 csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11376 2023-03-21 06:33:58.000000 csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7479 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10801 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    13329 2022-12-01 06:44:23.000000 csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5377 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.021203 csle_collector-0.1.9/src/csle_collector/ryu_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-12-11 08:32:31.000000 csle_collector-0.1.9/src/csle_collector/ryu_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3936 2022-12-11 08:32:31.000000 csle_collector-0.1.9/src/csle_collector/ryu_manager/query_ryu_server.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    12104 2023-03-21 06:33:58.000000 csle_collector-0.1.9/src/csle_collector/ryu_manager/ryu_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4363 2022-12-11 08:32:31.000000 csle_collector-0.1.9/src/csle_collector/ryu_manager/ryu_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8368 2022-12-11 08:32:31.000000 csle_collector-0.1.9/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2086 2022-12-11 08:32:31.000000 csle_collector-0.1.9/src/csle_collector/ryu_manager/ryu_manager_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.021203 csle_collector-0.1.9/src/csle_collector/snort_ids_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/snort_ids_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5390 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7053 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_alert.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11754 2023-03-17 07:49:22.000000 csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11533 2023-03-21 06:33:58.000000 csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8152 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10801 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    15997 2022-12-01 06:44:23.000000 csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.025203 csle_collector-0.1.9/src/csle_collector/traffic_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/traffic_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2534 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/traffic_manager/query_traffic_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7482 2023-03-21 06:33:58.000000 csle_collector-0.1.9/src/csle_collector/traffic_manager/traffic_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3087 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/traffic_manager/traffic_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5596 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1477 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/traffic_manager/traffic_manager_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.013203 csle_collector-0.1.9/src/csle_collector.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      803 2023-03-21 08:09:07.000000 csle_collector-0.1.9/src/csle_collector.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     3954 2023-03-21 08:09:08.000000 csle_collector-0.1.9/src/csle_collector.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:09:07.000000 csle_collector-0.1.9/src/csle_collector.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:37.000000 csle_collector-0.1.9/src/csle_collector.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      293 2023-03-21 08:09:07.000000 csle_collector-0.1.9/src/csle_collector.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       15 2023-03-21 08:09:07.000000 csle_collector-0.1.9/src/csle_collector.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:11.220414 csle_collector-0.2.0/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      803 2023-04-30 12:36:11.220414 csle_collector-0.2.0/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5807 2023-03-28 14:03:22.000000 csle_collector-0.2.0/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      674 2023-03-28 14:03:22.000000 csle_collector-0.2.0/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1454 2023-04-30 12:36:11.220414 csle_collector-0.2.0/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_collector-0.2.0/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:11.204414 csle_collector-0.2.0/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:11.204414 csle_collector-0.2.0/src/csle_collector/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-04-30 12:35:57.000000 csle_collector-0.2.0/src/csle_collector/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:11.208414 csle_collector-0.2.0/src/csle_collector/client_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/client_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    19240 2023-04-18 12:47:23.000000 csle_collector-0.2.0/src/csle_collector/client_manager/client_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4934 2023-04-01 08:34:56.000000 csle_collector-0.2.0/src/csle_collector/client_manager/client_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8592 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/client_manager/client_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2179 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/client_manager/client_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4200 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/client_manager/client_population_metrics.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5214 2023-04-18 12:47:23.000000 csle_collector-0.2.0/src/csle_collector/client_manager/query_clients.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:11.208414 csle_collector-0.2.0/src/csle_collector/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    36309 2023-04-18 12:48:07.000000 csle_collector-0.2.0/src/csle_collector/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:11.208414 csle_collector-0.2.0/src/csle_collector/docker_stats_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/docker_stats_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12394 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/docker_stats_manager/docker_stats.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13540 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/docker_stats_manager/docker_stats_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4589 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6193 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8801 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/docker_stats_manager/docker_stats_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3994 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:11.208414 csle_collector-0.2.0/src/csle_collector/elk_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/elk_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10740 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/elk_manager/elk_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5923 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/elk_manager/elk_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14300 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1540 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/elk_manager/elk_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5768 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/elk_manager/query_elk_server.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:11.212414 csle_collector-0.2.0/src/csle_collector/host_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/host_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      875 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/host_manager/failed_login_attempt.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    65375 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/host_manager/host_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13966 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/host_manager/host_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    28800 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/host_manager/host_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    33850 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/host_manager/host_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7783 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/host_manager/host_metrics.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    16572 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/host_manager/query_host_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1292 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/host_manager/successful_login.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:11.212414 csle_collector-0.2.0/src/csle_collector/kafka_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/kafka_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6616 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/kafka_manager/kafka_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4116 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/kafka_manager/kafka_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8484 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1442 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/kafka_manager/kafka_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3233 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/kafka_manager/query_kafka_server.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:11.216414 csle_collector-0.2.0/src/csle_collector/ossec_ids_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/ossec_ids_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2931 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10847 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11386 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7479 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10801 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13329 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5377 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:11.216414 csle_collector-0.2.0/src/csle_collector/ryu_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/ryu_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3936 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/ryu_manager/query_ryu_server.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18068 2023-04-18 12:46:51.000000 csle_collector-0.2.0/src/csle_collector/ryu_manager/ryu_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4363 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/ryu_manager/ryu_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8368 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2086 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/ryu_manager/ryu_manager_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:11.220414 csle_collector-0.2.0/src/csle_collector/snort_ids_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/snort_ids_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5787 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7996 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/snort_ids_manager/snort_ids_alert.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11779 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9176 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/snort_ids_manager/snort_ids_ip_alert_counters.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13005 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/snort_ids_manager/snort_ids_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8283 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10801 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    16748 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4288 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/snort_ids_manager/snort_ids_rule_counters.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:11.220414 csle_collector-0.2.0/src/csle_collector/traffic_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/traffic_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2534 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/traffic_manager/query_traffic_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7492 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/traffic_manager/traffic_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3087 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/traffic_manager/traffic_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5596 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1477 2023-03-28 14:03:22.000000 csle_collector-0.2.0/src/csle_collector/traffic_manager/traffic_manager_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:11.204414 csle_collector-0.2.0/src/csle_collector.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      803 2023-04-30 12:36:10.000000 csle_collector-0.2.0/src/csle_collector.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4086 2023-04-30 12:36:11.000000 csle_collector-0.2.0/src/csle_collector.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-04-30 12:36:10.000000 csle_collector-0.2.0/src/csle_collector.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:37.000000 csle_collector-0.2.0/src/csle_collector.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      293 2023-04-30 12:36:11.000000 csle_collector-0.2.0/src/csle_collector.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       15 2023-04-30 12:36:11.000000 csle_collector-0.2.0/src/csle_collector.egg-info/top_level.txt
```

### Comparing `csle_collector-0.1.9/PKG-INFO` & `csle_collector-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_collector
-Version: 0.1.9
+Version: 0.2.0
 Summary: Scripts for data collection in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_collector-0.1.9/README.md` & `csle_collector-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/pyproject.toml` & `csle_collector-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/setup.cfg` & `csle_collector-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/client_manager/client_manager.py` & `csle_collector-0.2.0/src/csle_collector/client_manager/client_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,41 +61,84 @@
 class ArrivalThread(threading.Thread):
     """
     Thread that generates client arrivals (starts client threads according to a Poisson process)
     """
 
     def __init__(self, commands: List[str], time_step_len_seconds: float = 1, lamb: float = 10, mu: float = 0.1,
                  num_commands: int = 2, sine_modulated: bool = False,
-                 time_scaling_factor: float = 0.01, period_scaling_factor: float = 20):
+                 time_scaling_factor: float = 0.01, period_scaling_factor: float = 20,
+                 exponents: List[float] = None, factors: List[float] = None, spiking: bool = False,
+                 piece_wise_constant: bool = False, breakpoints: List[float] = None, breakvalues: List[float] = None):
         """
         Initializes the arrival thread
 
+        :param commands: the list of commands that clients can use
         :param time_step_len_seconds: the number of seconds that one time-unit of the Poisson process corresponds to
         :param lamb: the lambda parameter of the Poisson process for arrivals
         :param mu: the mu parameter of the service times of the clients
-        :param commands: the list of commands that clients can use
         :param num_commands: the number of commands per client
         :param sine_modulated: boolean flag whether the rate of the arrival process is sine-modulated or not
+        :param time_scaling_factor: parameter for sine-modulated rate
+        :param period_scaling_factor: parameter for sine-modulated rate
+        :param exponents: parameters for spiking rate
+        :param factors: parameters for spiking rate
+        :param spiking: boolean flag indicating whether spiking rate should be used
+        :param piece_wise_constant: boolean flag indicating whether spiking piece-wise constant rate should be used.
         """
         threading.Thread.__init__(self)
         self.time_step_len_seconds = time_step_len_seconds
         self.client_threads = []
         self.t = 0
         self.lamb = lamb
         self.mu = mu
         self.stopped = False
         self.commands = commands
         self.num_commands = num_commands
         self.sine_modulated = sine_modulated
         self.rate = self.lamb
         self.time_scaling_factor = time_scaling_factor
         self.period_scaling_factor = period_scaling_factor
-        logging.info(f"Starting arrival thread, lambda:{lamb}, mu:{mu}, num:commands:{num_commands}, "
+        self.exponents = exponents
+        self.factors = factors
+        self.spiking = spiking
+        self.piece_wise_constant = piece_wise_constant
+        self.breakpoints = breakpoints
+        self.breakvalues = breakvalues
+        logging.info(f"Starting arrival thread, lambda:{lamb}, mu:{mu}, num_commands:{num_commands}, "
                      f"commands:{commands}, sine_modulated: {sine_modulated}, "
-                     f"time_scaling_factor: {time_scaling_factor}, period_scaling_factor: {period_scaling_factor}")
+                     f"time_scaling_factor: {time_scaling_factor}, period_scaling_factor: {period_scaling_factor},"
+                     f"spiking: {spiking}, exponents: {exponents}, factors: {factors}, breakpoints: {breakpoints}, "
+                     f"breakvalues: {breakvalues}, piece_wise_constant: {piece_wise_constant}")
+
+    def piece_wise_constant_rate(self, t) -> float:
+        """
+        Function that returns the rate of a piece-wise constant Poisson process
+
+        :param t: the time-step
+        :return: the rate
+        """
+        rate = 0
+        assert len(self.breakvalues) == len(self.breakpoints)
+        for i in range(len(self.breakvalues)):
+            if t >= self.breakpoints[i]:
+                rate = self.breakvalues[i]
+        return rate
+
+    def spiking_poisson_arrival_rate(self, t) -> float:
+        """
+        Function that returns the rate of a spiking Poisson process
+
+        :param t: the time-step
+        :return: the rate
+        """
+        rate = self.lamb
+        assert len(self.exponents) == len(self.factors)
+        for i in range(len(self.exponents)):
+            rate = self.factors[i] * math.exp(math.pow(-(t - self.exponents[i]), 2))
+        return rate
 
     def sine_modulated_poisson_rate(self, t) -> float:
         """
         Function that returns the rate of a sine-modulated Poisson process
 
         :param t: the time-step
         :return: the rate
@@ -150,15 +193,15 @@
         self.time_step_len_seconds = time_step_len_seconds
         self.stopped = False
         self.kafka_ip = ip
         self.port = port
         self.hostname = socket.gethostname()
         try:
             self.ip = netifaces.ifaddresses(constants.INTERFACES.ETH0)[netifaces.AF_INET][0][constants.INTERFACES.ADDR]
-        except:
+        except Exception:
             self.ip = socket.gethostbyname(self.hostname)
         self.conf = {
             constants.KAFKA.BOOTSTRAP_SERVERS_PROPERTY: f"{self.kafka_ip}:{self.port}",
             constants.KAFKA.CLIENT_ID_PROPERTY: self.hostname}
         self.producer = Producer(**self.conf)
         logging.info(f"Starting producer thread, ip:{self.ip}, kafka port:{self.port}, "
                      f"time_step_len:{self.time_step_len_seconds}, kafka_ip:{self.kafka_ip}")
@@ -171,16 +214,17 @@
         """
         while not self.stopped and self.arrival_thread is not None:
             time.sleep(self.time_step_len_seconds)
             if self.arrival_thread is not None:
                 ts = time.time()
                 num_clients = len(self.arrival_thread.client_threads)
                 rate = self.arrival_thread.rate
+                mu = self.arrival_thread.mu
                 self.producer.produce(constants.KAFKA_CONFIG.CLIENT_POPULATION_TOPIC_NAME,
-                                      f"{ts},{self.ip},{num_clients},{rate}")
+                                      f"{ts},{self.ip},{num_clients},{rate},{mu}")
                 self.producer.poll(0)
 
 
 class ClientManagerServicer(csle_collector.client_manager.client_manager_pb2_grpc.ClientManagerServicer):
     """
     gRPC server for managing the running clients. Allows to start/stop clients remotely and also to query the
     state of the clients.
@@ -262,29 +306,35 @@
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a clients DTO with the state of the clients
         """
         logging.info(f"Starting clients, commands:{request.commands}, lamb: {request.lamb}, mu: {request.mu}, "
                      f"sine_modulated: {request.sine_modulated}, "
                      f"time_scaling_factor: {request.time_scaling_factor}, "
-                     f"period_scaling_factor: {request.period_scaling_factor}")
+                     f"period_scaling_factor: {request.period_scaling_factor}, spiking: {request.spiking}, "
+                     f"piece_wise_constant: {request.piece_wise_constant}, exponents: {request.exponents}, "
+                     f"factors: {request.factors}, breakvalues: {request.breakvalues}, "
+                     f"breakpoints: {request.breakpoints}")
 
         producer_time_step_len_seconds = 0
 
         if self.arrival_thread is not None:
             self.arrival_thread.stopped = True
             time.sleep(1)
 
         if request.time_step_len_seconds <= 0:
             request.time_step_len_seconds = 1
 
         arrival_thread = ArrivalThread(commands=request.commands, time_step_len_seconds=request.time_step_len_seconds,
                                        lamb=request.lamb, mu=request.mu, sine_modulated=request.sine_modulated,
                                        time_scaling_factor=request.time_scaling_factor,
-                                       period_scaling_factor=request.period_scaling_factor)
+                                       period_scaling_factor=request.period_scaling_factor,
+                                       piece_wise_constant=request.piece_wise_constant, breakvalues=request.breakvalues,
+                                       breakpoints=request.breakpoints, factors=request.factors,
+                                       exponents=request.exponents, spiking=request.spiking)
         arrival_thread.start()
         self.arrival_thread = arrival_thread
         clients_time_step_len_seconds = self.arrival_thread.time_step_len_seconds
 
         producer_active = False
         if self.producer_thread is not None:
             producer_active = True
```

### Comparing `csle_collector-0.1.9/src/csle_collector/client_manager/client_manager_pb2.py` & `csle_collector-0.2.0/src/csle_collector/client_manager/client_manager_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x63lient_manager.proto\"\x10\n\x0eStopClientsMsg\"\xc6\x01\n\x0fStartClientsMsg\x12\n\n\x02mu\x18\x01 \x01(\x02\x12\x0c\n\x04lamb\x18\x02 \x01(\x02\x12\x1d\n\x15time_step_len_seconds\x18\x03 \x01(\x05\x12\x10\n\x08\x63ommands\x18\x04 \x03(\t\x12\x14\n\x0cnum_commands\x18\x05 \x01(\x05\x12\x16\n\x0esine_modulated\x18\x06 \x01(\x08\x12\x1b\n\x13time_scaling_factor\x18\x07 \x01(\x02\x12\x1d\n\x15period_scaling_factor\x18\x08 \x01(\x02\"\x0f\n\rGetClientsMsg\"K\n\x10StartProducerMsg\x12\n\n\x02ip\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x1d\n\x15time_step_len_seconds\x18\x03 \x01(\x05\"\x11\n\x0fStopProducerMsg\"\xa8\x01\n\nClientsDTO\x12\x13\n\x0bnum_clients\x18\x01 \x01(\x05\x12\x1d\n\x15\x63lient_process_active\x18\x02 \x01(\x08\x12\x17\n\x0fproducer_active\x18\x03 \x01(\x08\x12%\n\x1d\x63lients_time_step_len_seconds\x18\x04 \x01(\x05\x12&\n\x1eproducer_time_step_len_seconds\x18\x05 \x01(\x05\x32\x80\x02\n\rClientManager\x12+\n\ngetClients\x12\x0e.GetClientsMsg\x1a\x0b.ClientsDTO\"\x00\x12-\n\x0bstopClients\x12\x0f.StopClientsMsg\x1a\x0b.ClientsDTO\"\x00\x12/\n\x0cstartClients\x12\x10.StartClientsMsg\x1a\x0b.ClientsDTO\"\x00\x12\x31\n\rstartProducer\x12\x11.StartProducerMsg\x1a\x0b.ClientsDTO\"\x00\x12/\n\x0cstopProducer\x12\x10.StopProducerMsg\x1a\x0b.ClientsDTO\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x63lient_manager.proto\"\x10\n\x0eStopClientsMsg\"\xc2\x02\n\x0fStartClientsMsg\x12\n\n\x02mu\x18\x01 \x01(\x02\x12\x0c\n\x04lamb\x18\x02 \x01(\x02\x12\x1d\n\x15time_step_len_seconds\x18\x03 \x01(\x05\x12\x10\n\x08\x63ommands\x18\x04 \x03(\t\x12\x14\n\x0cnum_commands\x18\x05 \x01(\x05\x12\x16\n\x0esine_modulated\x18\x06 \x01(\x08\x12\x1b\n\x13time_scaling_factor\x18\x07 \x01(\x02\x12\x1d\n\x15period_scaling_factor\x18\x08 \x01(\x02\x12\x0f\n\x07spiking\x18\t \x01(\x08\x12\x11\n\texponents\x18\n \x03(\x02\x12\x0f\n\x07\x66\x61\x63tors\x18\x0b \x03(\x02\x12\x13\n\x0b\x62reakpoints\x18\x0c \x03(\x05\x12\x13\n\x0b\x62reakvalues\x18\r \x03(\x02\x12\x1b\n\x13piece_wise_constant\x18\x0e \x01(\x08\"\x0f\n\rGetClientsMsg\"K\n\x10StartProducerMsg\x12\n\n\x02ip\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x1d\n\x15time_step_len_seconds\x18\x03 \x01(\x05\"\x11\n\x0fStopProducerMsg\"\xa8\x01\n\nClientsDTO\x12\x13\n\x0bnum_clients\x18\x01 \x01(\x05\x12\x1d\n\x15\x63lient_process_active\x18\x02 \x01(\x08\x12\x17\n\x0fproducer_active\x18\x03 \x01(\x08\x12%\n\x1d\x63lients_time_step_len_seconds\x18\x04 \x01(\x05\x12&\n\x1eproducer_time_step_len_seconds\x18\x05 \x01(\x05\x32\x80\x02\n\rClientManager\x12+\n\ngetClients\x12\x0e.GetClientsMsg\x1a\x0b.ClientsDTO\"\x00\x12-\n\x0bstopClients\x12\x0f.StopClientsMsg\x1a\x0b.ClientsDTO\"\x00\x12/\n\x0cstartClients\x12\x10.StartClientsMsg\x1a\x0b.ClientsDTO\"\x00\x12\x31\n\rstartProducer\x12\x11.StartProducerMsg\x1a\x0b.ClientsDTO\"\x00\x12/\n\x0cstopProducer\x12\x10.StopProducerMsg\x1a\x0b.ClientsDTO\"\x00\x62\x06proto3')
 
 
 
 _STOPCLIENTSMSG = DESCRIPTOR.message_types_by_name['StopClientsMsg']
 _STARTCLIENTSMSG = DESCRIPTOR.message_types_by_name['StartClientsMsg']
 _GETCLIENTSMSG = DESCRIPTOR.message_types_by_name['GetClientsMsg']
 _STARTPRODUCERMSG = DESCRIPTOR.message_types_by_name['StartProducerMsg']
@@ -69,19 +69,19 @@
 _CLIENTMANAGER = DESCRIPTOR.services_by_name['ClientManager']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _STOPCLIENTSMSG._serialized_start=24
   _STOPCLIENTSMSG._serialized_end=40
   _STARTCLIENTSMSG._serialized_start=43
-  _STARTCLIENTSMSG._serialized_end=241
-  _GETCLIENTSMSG._serialized_start=243
-  _GETCLIENTSMSG._serialized_end=258
-  _STARTPRODUCERMSG._serialized_start=260
-  _STARTPRODUCERMSG._serialized_end=335
-  _STOPPRODUCERMSG._serialized_start=337
-  _STOPPRODUCERMSG._serialized_end=354
-  _CLIENTSDTO._serialized_start=357
-  _CLIENTSDTO._serialized_end=525
-  _CLIENTMANAGER._serialized_start=528
-  _CLIENTMANAGER._serialized_end=784
+  _STARTCLIENTSMSG._serialized_end=365
+  _GETCLIENTSMSG._serialized_start=367
+  _GETCLIENTSMSG._serialized_end=382
+  _STARTPRODUCERMSG._serialized_start=384
+  _STARTPRODUCERMSG._serialized_end=459
+  _STOPPRODUCERMSG._serialized_start=461
+  _STOPPRODUCERMSG._serialized_end=478
+  _CLIENTSDTO._serialized_start=481
+  _CLIENTSDTO._serialized_end=649
+  _CLIENTMANAGER._serialized_start=652
+  _CLIENTMANAGER._serialized_end=908
 # @@protoc_insertion_point(module_scope)
```

### Comparing `csle_collector-0.1.9/src/csle_collector/client_manager/client_manager_pb2_grpc.py` & `csle_collector-0.2.0/src/csle_collector/client_manager/client_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/client_manager/client_manager_util.py` & `csle_collector-0.2.0/src/csle_collector/client_manager/client_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/client_manager/client_population_metrics.py` & `csle_collector-0.2.0/src/csle_collector/client_manager/client_population_metrics.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,119 +4,126 @@
 
 class ClientPopulationMetrics:
 
     """
     DTO representing information about the client population
     """
 
-    def __init__(self, ip: str = "", ts: float = time.time(), num_clients: int = 0, rate: float = 20):
+    def __init__(self, ip: str = "", ts: float = time.time(), num_clients: int = 0, rate: float = 20,
+                 service_time: float = 4):
         """
         Initializes the DTO
 
         :param ip: the ip address
         :param ts: the timestamp
         :param num_clients: the number of clients currently
         :param rate: the client arrival rate
+        :param mean_service_time: the average service time (in terms of time-steps)
         """
         self.ip = ip
         self.ts = ts
         self.num_clients = num_clients
         self.rate = rate
+        self.service_time = service_time
 
     @staticmethod
     def from_kafka_record(record: str) -> "ClientPopulationMetrics":
         """
         Converts a kafka record to a DTO
 
         :param record: the kafka record
         :return: the DTO
         """
         parts = record.split(",")
         obj = ClientPopulationMetrics(ts=float(parts[0]), ip=parts[1], num_clients=int(parts[2]),
-                                      rate=float(parts[3]))
+                                      rate=float(parts[3]), service_time=float(parts[4]))
         return obj
 
     def update_with_kafka_record(self, record: str) -> None:
         """
         Updates the DTO with a new kafka record
 
         :param record: the kafka record
         :return: None
         """
         parts = record.split(",")
         self.ts = float(parts[0])
         self.ip = parts[1]
         self.num_clients = int(parts[2])
         self.rate = float(parts[3])
+        self.service_time = float(parts[4])
 
     @staticmethod
     def from_dict(d: Dict[str, Any]) -> "ClientPopulationMetrics":
         """
         Converts a dict representation of the object into an instance
         :param d: the dict representation
         :return: the created instance
         """
         rate = 0
         if rate in d:
             rate = d["rate"]
         obj = ClientPopulationMetrics(
-            ts=d["ts"], ip=d["ip"], num_clients=d["num_clients"], rate=rate
-        )
+            ts=d["ts"], ip=d["ip"], num_clients=d["num_clients"], rate=rate, service_time=d["service_time"])
         return obj
 
     def to_dict(self) -> Dict[str, Any]:
         """
         :return: a dict representation of the object
         """
         d = {}
         d["ip"] = self.ip
         d["ts"] = self.ts
         d["num_clients"] = self.num_clients
         d["rate"] = self.rate
+        d["service_time"] = self.service_time
         return d
 
     def __str__(self):
         """
         :return: a string representation of the object
         """
-        return f"ip: {self.ip}, ts: {self.ts}, num_clients: {self.num_clients}, rate: {self.rate}"
+        return f"ip: {self.ip}, ts: {self.ts}, num_clients: {self.num_clients}, rate: {self.rate}, " \
+               f"avg service time: {self.service_time}"
 
     def copy(self) -> "ClientPopulationMetrics":
         """
         :return: a copy of the object
         """
-        c = ClientPopulationMetrics(ip=self.ip, ts=self.ts, num_clients=self.num_clients, rate=self.rate)
+        c = ClientPopulationMetrics(ip=self.ip, ts=self.ts, num_clients=self.num_clients, rate=self.rate,
+                                    service_time=self.service_time)
         return c
 
     def get_values(self) -> Tuple[List[float], List[str]]:
         """
         Get the current values
 
         :return: the values and the labels
         """
-        deltas = [int(self.num_clients), float(self.rate)]
-        labels = ["num_clients", "rate"]
+        deltas = [int(self.num_clients), float(self.rate), float(self.service_time)]
+        labels = ["num_clients", "rate", "service_time"]
         return deltas, labels
 
     def get_deltas(self, stats_prime: "ClientPopulationMetrics") -> Tuple[List[float], List[str]]:
         """
         Get the deltas between two stats objects
 
         :param stats_prime: the stats object to compare with
         :return: the deltas and the labels
         """
-        deltas = [int(stats_prime.num_clients - self.num_clients), float(stats_prime.rate - self.rate)]
-        labels = ["num_clients", "rate"]
+        deltas = [int(stats_prime.num_clients - self.num_clients), float(stats_prime.rate - self.rate),
+                  float(stats_prime.service_time - self.service_time)]
+        labels = ["num_clients", "rate", "service_time"]
         return deltas, labels
 
     def num_attributes(self) -> int:
         """
         :return: The number of attributes of the DTO
         """
-        return 4
+        return 5
 
     @staticmethod
     def schema() -> "ClientPopulationMetrics":
         """
         :return: get the schema of the DTO
         """
         return ClientPopulationMetrics()
```

### Comparing `csle_collector-0.1.9/src/csle_collector/client_manager/query_clients.py` & `csle_collector-0.2.0/src/csle_collector/client_manager/query_clients.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,56 +11,64 @@
     Queries the server for the client state
 
     :param stub: the stub to send the remote gRPC to the server
     :param timeout: the GRPC timeout (seconds)
     :return: a clientsDTO describing the state of the clients
     """
     get_clients_dto_msg = csle_collector.client_manager.client_manager_pb2.GetClientsMsg()
-    clients_dto = stub.getClients(get_clients_dto_msg)
+    clients_dto = stub.getClients(get_clients_dto_msg, timeout=timeout)
     return clients_dto
 
 
 def stop_clients(stub: csle_collector.client_manager.client_manager_pb2_grpc.ClientManagerStub,
                  timeout=constants.GRPC.TIMEOUT_SECONDS):
     """
     Stops the client arrival process
 
     :param stub: the stub to the gRPC server
     :param timeout: the GRPC timeout (seconds)
     :return: a clientsDTO describing the state of the clients
     """
     stop_clients_msg = csle_collector.client_manager.client_manager_pb2.StopClientsMsg()
-    clients_dto = stub.stopClients(stop_clients_msg)
+    clients_dto = stub.stopClients(stop_clients_msg, timeout=timeout)
     return clients_dto
 
 
 def start_clients(stub: csle_collector.client_manager.client_manager_pb2_grpc.ClientManagerStub,
                   mu: float, lamb: float, time_step_len_seconds: int, commands: List[str], num_commands: int = 2,
                   sine_modulated: bool = False, time_scaling_factor: float = 0.01, period_scaling_factor: float = 20,
+                  spiking: bool = False, exponents: List[float] = None, factors: List[float] = None,
+                  breakpoints: List[int] = None, breakvalues: List[float] = None, piece_wise_constant: bool = False,
                   timeout=constants.GRPC.TIMEOUT_SECONDS):
     """
     Starts the client arrival process
 
     :param stub: the stub to the gRPC server
     :param mu: the mu parameter for the Exponential service time
     :param lamb: the lambda parameter for the Poisson process
     :param time_step_len_seconds: the length of a time-step for simulating the arrival process
     :param num:commands: the number of commands that each client will use
     :param sine_modulated: whether the arrival process is sine modulated or not
     :param time_scaling_factor: the time scaling factor for the sine modulated arrival process
     :param period_scaling_factor: the period scaling factor for the sine modulated arrival process
     :param timeout: the GRPC timeout (seconds)
+    :param spiking: boolean flag indicating whether the arrival process is spiking or not
+    :param exponents: list of exponents for spiking arrival process
+    :param factors: list of factors for spiking arrival process
+    :param piece_wise_constant: boolean flag indicating whether the arrival process is piece-wise constant or not
+    :param breakpoints: list of breakpoints for piece-wise constant arrival process
+    :param breakvalues: list of breakvalues for piece-wise constant arrival process
     :return: a clientsDTO describing the state of the clients
     """
     start_clients_msg = csle_collector.client_manager.client_manager_pb2.StartClientsMsg(
         mu=mu, lamb=lamb, time_step_len_seconds=time_step_len_seconds, commands=commands,
         num_commands=num_commands, sine_modulated=sine_modulated, period_scaling_factor=period_scaling_factor,
-        time_scaling_factor=time_scaling_factor
-    )
-    clients_dto = stub.startClients(start_clients_msg)
+        time_scaling_factor=time_scaling_factor, spiking=spiking, exponents=exponents, factors=factors,
+        breakpoints=breakpoints, breakvalues=breakvalues, piece_wise_constant=piece_wise_constant)
+    clients_dto = stub.startClients(start_clients_msg, timeout=timeout)
     return clients_dto
 
 
 def stop_producer(stub: csle_collector.client_manager.client_manager_pb2_grpc.ClientManagerStub,
                   timeout=constants.GRPC.TIMEOUT_SECONDS):
     """
     Stops the producer process
```

### Comparing `csle_collector-0.1.9/src/csle_collector/constants/constants.py` & `csle_collector-0.2.0/src/csle_collector/constants/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -255,14 +255,22 @@
     HOST_MANAGER_DEFAULT_PORT = 50049
     SNORT_IDS_MANAGER_DEFAULT_PORT = 50048
     OSSEC_IDS_MANAGER_DEFAULT_PORT = 50047
     DOCKER_STATS_MANAGER_DEFAULT_PORT = 50046
     ELK_MANAGER_DEFAULT_PORT = 50045
     KAFKA_MANAGER_DEFAULT_PORT = 50051
 
+
+class GRPC_WORKERS:
+    """
+    Constants related to the number of GRPC workers
+    """
+    DEFAULT_MAX_NUM_WORKERS = 10
+
+
 class TRAFFIC_GENERATOR:
     """
     Constants related to the traffic generator
     """
     START_TRAFFIC_GENERATOR_CMD = "sudo nohup /traffic_generator.sh &"
     TRAFFIC_GENERATOR_FILE_NAME = "traffic_generator.sh"
     CREATE_TRAFFIC_GENERATOR_FILE = "sudo touch /traffic_generator.sh"
@@ -404,14 +412,16 @@
     SNORT_FAST_LOG_FILE = "/var/snort/fast.log"
     SNORT_ALERTS_FILE = "/var/snort/alert.csv"
     SNORT_STATS_FILE = "/var/snort/snort.stats"
     TAIL_ALERTS_COMMAND = "sudo tail -" + str(MAX_ALERTS)
     TAIL_FAST_LOG_COMMAND = "sudo tail -" + str(str(MAX_ALERTS))
     TAIL_ALERTS_LATEST_COMMAND = "sudo tail -1"
     PRIORITY_REGEX = re.compile(r"Priority: \d")
+    IPS_REGEX = re.compile(r"\d{1,3}.\d{1,3}\.\d{1,3}\.\d{1,3} -> \d{1,3}.\d{1,3}\.\d{1,3}\.\d{1,3}")
+    RULE_ID_REGEX = re.compile(r"\[\d{1,3}\:\d{1,3}")
     CLASSIFICATION_REGEX = re.compile(r"(?<=Classification: )(.*?)(?=])")
     SNORT_SEVERE_ALERT_PRIORITY_THRESHOLD = 2
     SNORT_ALERT_IDS_ID = {}
     SNORT_ALERT_IDS_ID["tcp-connection"] = 0
     SNORT_ALERT_IDS_ID["A TCP connection was detected"] = 0
     SNORT_ALERT_IDS_ID["unknown"] = 1
     SNORT_ALERT_IDS_ID["Unknown Traffic"] = 1
@@ -476,16 +486,17 @@
     SNORT_ALERT_IDS_ID["inappropriate-content"] = 31
     SNORT_ALERT_IDS_ID["Inappropriate Content was Detected"] = 31
     SNORT_ALERT_IDS_ID["attempted-user"] = 32
     SNORT_ALERT_IDS_ID["Attempted User Privilege Gain"] = 32
     SNORT_ALERT_IDS_ID["attempted-admin"] = 33
     SNORT_ALERT_IDS_ID["Attempted Administrator Privilege Gain"] = 33
     STOP_SNORT_IDS = "kill -9 $(pgrep snort)"
-    START_SNORT_IDS = "sudo snort -D -q -u snort -g snort -c /etc/snort/snort.conf -i eth1:eth0 -l " \
-                      "/var/snort/ -h 55.0.0.0/8 -Q -I --create-pidfile"
+    START_SNORT_IDS = "sudo snort -D -q -c /etc/snort/snort.conf -i {}:{} -l " \
+                      "/var/snort/ -h {} -Q -I --create-pidfile"
+    SNORT_LOG_DIR_PERMISSION_CMD = "sudo chmod -R 777 /var/snort"
     CHECK_IF_SNORT_IS_RUNNING_CMD = "ps -aux | grep snort.conf"
     PS_AUX_CMD = "ps -aux"
     GREP_SNORT_CONF = "grep snort.conf"
     SEARCH_SNORT_RUNNING = "/etc/snort/snort.conf"
 
 
 class HOST_METRICS:
@@ -516,19 +527,24 @@
     SUFFIX = "_1"
 
 
 class KAFKA_CONFIG:
     """
     Constants related to the kafka container configuration
     """
+    DEFAULT_NUM_PARTITIONS = 1
+    DEFAULT_NUM_REPLICAS = 1
+    DEFAULT_RETENTION_TIME_HOURS = 240
     NETWORK_ID_THIRD_OCTET = 253
     NETWORK_ID_FOURTH_OCTET = 253
     SUFFIX = "_1"
     CLIENT_POPULATION_TOPIC_NAME = "client_population"
     SNORT_IDS_LOG_TOPIC_NAME = "snort_ids_log"
+    SNORT_IDS_RULE_LOG_TOPIC_NAME = "snort_ids_rule_log"
+    SNORT_IDS_IP_LOG_TOPIC_NAME = "snort_ids_ip_log"
     OSSEC_IDS_LOG_TOPIC_NAME = "ossec_ids_log"
     HOST_METRICS_TOPIC_NAME = "host_metrics"
     DOCKER_STATS_TOPIC_NAME = "docker_stats"
     DOCKER_HOST_STATS_TOPIC_NAME = "docker_host_stats"
     OPENFLOW_FLOW_STATS_TOPIC_NAME = "openflow_flow_stats"
     OPENFLOW_PORT_STATS_TOPIC_NAME = "openflow_port_stats"
     OPENFLOW_AGG_FLOW_STATS_TOPIC_NAME = "openflow_flow_agg_stats"
@@ -556,14 +572,28 @@
                                       "level_6_alerts", "level_7_alerts", "level_8_alerts", "level_9_alerts",
                                       "level_10_alerts", "level_11_alerts", "level_12_alerts", "level_13_alerts",
                                       "level_14_alerts", "level_15_alerts", "invalid_login_alerts",
                                       "authentication_success_alerts", "authentication_failed_alerts",
                                       "connection_attempt_alerts", "attacks_alerts", "adduser_alerts", "sshd_alerts",
                                       "ids_alerts", "firewall_alerts", "squid_alerts",
                                       "apache_alerts", "syslog_alerts"]
+    SNORT_IDS_RULE_LOG_ATTRIBUTES = ["timestamp", "ip", "alert_rule_id", "num_alerts"]
+    SNORT_IDS_IP_LOG_ATTRIBUTES = ["timestamp", "ip", "alert_ip", "attempted-admin", "attempted-user",
+                                   "inappropriate-content", "policy-violation", "shellcode-detect",
+                                   "successful-admin", "successful-user", "trojan-activity", "unsuccessful-user",
+                                   "web-application-attack", "attempted-dos", "attempted-recon", "bad-unknown",
+                                   "default-login-attempt", "denial-of-service", "misc-attack",
+                                   "non-standard-protocol", "rpc-portmap-decode", "successful-dos",
+                                   "successful-recon-largescale", "successful-recon-limited",
+                                   "suspicious-filename-detect", "suspicious-login", "system-call-detect",
+                                   "unusual-client-port-connection", "web-application-activity", "icmp-event",
+                                   "misc-activity", "network-scan", "not-suspicious", "protocol-command-decode",
+                                   "string-detect", "unknown", "tcp-connection", "priority_1", "priority_2",
+                                   "priority_3", "priority_4", "alerts_weighted_by_priority", "total_alerts",
+                                   "severe_alerts", "warning_alerts"]
     HOST_METRICS_TOPIC_ATTRIBUTES = ["timestamp", "ip", "num_logged_in_users", "num_failed_login_attempts",
                                      "num_open_connections", "num_login_events", "num_processes", "num_users"]
     DOCKER_STATS_TOPIC_ATTRIBUTES = ["timestamp", "ip", "cpu_percent", "mem_current", "mem_total",
                                      "mem_percent", "blk_read", "blk_write", "net_rc", "net_tx", "pids"]
     ATTACKER_ACTIONS_ATTRIBUTES = ["timestamp", "id", "description", "index", "name", "time", "ip", "cmd"]
     DEFENDER_ACTIONS_ATTRIBUTES = ["timestamp", "id", "description", "index", "name", "time", "ip", "cmd"]
     OPENFLOW_FLOW_STATS_TOPIC_ATTRIBUTES = ["timestamp", "datapath_id", "in_port", "out_port", "dst_mac_address",
@@ -624,19 +654,23 @@
     DOCKER_STATS_COUNTER_LABELS = [
         "pids", "cpu_percent", "mem_current", "mem_total",
         "mem_percent", "blk_read", "blk_write", "net_rx", "net_tx"
     ]
     DOCKER_STATS_PERCENT_LABELS = [
         "cpu_percent", "cpu_percent"
     ]
-    CLIENT_POPULATION_METRIC_LABELS = ["num_clients", "rate"]
-    ALL_DELTA_LABELS = (SNORT_IDS_ALERTS_LABELS + HOST_METRICS_LABELS + DOCKER_STATS_COUNTER_LABELS +
-                        DOCKER_STATS_PERCENT_LABELS + CLIENT_POPULATION_METRIC_LABELS + OSSEC_IDS_ALERTS_LABELS)
-    ALL_INITIAL_LABELS = (HOST_METRICS_LABELS + DOCKER_STATS_COUNTER_LABELS + DOCKER_STATS_PERCENT_LABELS +
-                          CLIENT_POPULATION_METRIC_LABELS + SNORT_IDS_ALERTS_LABELS + OSSEC_IDS_ALERTS_LABELS)
+    CLIENT_POPULATION_METRIC_LABELS = ["num_clients", "rate", "service_time"]
+    ALL_DELTA_AGG_LABELS = (SNORT_IDS_ALERTS_LABELS + HOST_METRICS_LABELS + DOCKER_STATS_COUNTER_LABELS +
+                            DOCKER_STATS_PERCENT_LABELS + CLIENT_POPULATION_METRIC_LABELS + OSSEC_IDS_ALERTS_LABELS)
+    ALL_DELTA_MACHINE_LABELS = (SNORT_IDS_ALERTS_LABELS + HOST_METRICS_LABELS + DOCKER_STATS_COUNTER_LABELS +
+                                DOCKER_STATS_PERCENT_LABELS + OSSEC_IDS_ALERTS_LABELS)
+    ALL_INITIAL_AGG_LABELS = (HOST_METRICS_LABELS + DOCKER_STATS_COUNTER_LABELS + DOCKER_STATS_PERCENT_LABELS +
+                              CLIENT_POPULATION_METRIC_LABELS + SNORT_IDS_ALERTS_LABELS + OSSEC_IDS_ALERTS_LABELS)
+    ALL_INITIAL_MACHINE_LABELS = (HOST_METRICS_LABELS + DOCKER_STATS_COUNTER_LABELS + DOCKER_STATS_PERCENT_LABELS +
+                                  SNORT_IDS_ALERTS_LABELS + OSSEC_IDS_ALERTS_LABELS)
 
 
 class KAFKA:
     """
     String constants for managing Kafka
     """
     KAFKA_STATUS = "service kafka status"
@@ -670,34 +704,51 @@
     LOGSTASH_START = "service logstash start"
     ELASTICSEARCH_STATUS = "service elasticsearch status"
     KIBANA_STATUS = "service kibana status"
     LOGSTASH_STATUS = "service logstash status"
     ELASTICSEARCH_LOG_DIR = "/var/log/elasticsearch/"
     LOGSTASH_LOG_DIR = "/var/log/logstash/"
     KIBANA_LOG_DIR = "/var/log/kibana/"
+    ELASTIC_PORT = 9200
+    KIBANA_PORT = 5601
+    LOGSTASH_PORT = 5044
 
 
 class RYU:
     """
     String constants for managing Ryu
     """
     CHECK_IF_RYU_CONTROLLER_IS_RUNNING = "ps -aux | grep ryu_controller.py"
     STOP_RYU_CONTROLLER = "sudo pkill -f ryu_controller.py"
+    STOP_RYU_CONTROLLER_MANAGER = "sudo pkill -f ryu-manager"
     RYU_CONTROLLER_FILENAME = "ryu_controller.py"
     SEARCH_CONTROLLER = "/root/miniconda3/bin/python3 /ryu_controller.py"
     START_RYU_CONTROLLER = "sudo nohup /root/miniconda3/bin/python3 /ryu_controller.py --port {} --webport {} " \
                            "--controller {} &"
     START_PRODUCER_HTTP_RESOURCE = "/cslenorthboundapi/producer/start"
     STOP_PRODUCER_HTTP_RESOURCE = "/cslenorthboundapi/producer/stop"
     STATUS_PRODUCER_HTTP_RESOURCE = "/cslenorthboundapi/producer/status"
     TIME_STEP_LEN_SECONDS = "time_step_len_seconds"
     PRODUCER_RUNNING = "producer_running"
     KAFKA_CONF = "kafka_conf"
+    REQUEST_TIMEOUT_S = 5
 
 
 class INTERFACES:
     """
     String constrants related to networking interfaces
     """
     ETH1 = "eth1"
     ETH0 = "eth0"
     ADDR = "addr"
+
+
+class SPARK:
+    """
+    Constants related to Spark
+    """
+    START_SPARK_MASTER = "/spark-3.3.2-bin-hadoop3/sbin/start-master.sh"
+    START_SPARK_WORKER = "/spark-3.3.2-bin-hadoop3/sbin/start-worker.sh spark://15.13.1.161:7077 -m 2G -c 1"
+    SPARK_MASTER_PID_FILE = "/tmp/spark--org.apache.spark.deploy.master.Master-1.pid"
+    SPARK_WORKER_PID_FILE = "/tmp/spark--org.apache.spark.deploy.worker.Worker-1.pid"
+    STOP_SPARK_WORKER = "sudo kill -9 {}"
+    STOP_SPARK_MASTER = "sudo kill -9 {}"
```

### Comparing `csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats.py` & `csle_collector-0.2.0/src/csle_collector/docker_stats_manager/docker_stats.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats_manager.py` & `csle_collector-0.2.0/src/csle_collector/docker_stats_manager/docker_stats_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py` & `csle_collector-0.2.0/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py` & `csle_collector-0.2.0/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats_util.py` & `csle_collector-0.2.0/src/csle_collector/docker_stats_manager/docker_stats_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py` & `csle_collector-0.2.0/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/elk_manager/elk_manager.py` & `csle_collector-0.2.0/src/csle_collector/elk_manager/elk_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         Initializes the server
         """
         logging.basicConfig(filename=f"{constants.LOG_FILES.ELK_MANAGER_LOG_DIR}"
                                      f"{constants.LOG_FILES.ELK_MANAGER_LOG_FILE}", level=logging.INFO)
         self.hostname = socket.gethostname()
         try:
             self.ip = netifaces.ifaddresses(constants.INTERFACES.ETH0)[netifaces.AF_INET][0][constants.INTERFACES.ADDR]
-        except:
+        except Exception:
             self.ip = socket.gethostbyname(self.hostname)
         logging.info(f"Setting up ElkManager hostname: {self.hostname} ip: {self.ip}")
 
     def _get_elk_status(self) -> Tuple[bool, bool, bool]:
         """
         Utility method to get the status of the ELK stack
```

### Comparing `csle_collector-0.1.9/src/csle_collector/elk_manager/elk_manager_pb2.py` & `csle_collector-0.2.0/src/csle_collector/elk_manager/elk_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py` & `csle_collector-0.2.0/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/elk_manager/elk_manager_util.py` & `csle_collector-0.2.0/src/csle_collector/elk_manager/elk_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/elk_manager/query_elk_server.py` & `csle_collector-0.2.0/src/csle_collector/elk_manager/query_elk_server.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/host_manager/failed_login_attempt.py` & `csle_collector-0.2.0/src/csle_collector/host_manager/failed_login_attempt.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/host_manager/host_manager.py` & `csle_collector-0.2.0/src/csle_collector/host_manager/host_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List
 import logging
 import socket
 import netifaces
 import time
 import grpc
+import os
 import threading
 from concurrent import futures
 import subprocess
 from confluent_kafka import Producer
 import csle_collector.host_manager.host_manager_pb2_grpc
 import csle_collector.host_manager.host_manager_pb2
 from csle_collector.host_manager.host_manager_util import HostManagerUtil
@@ -79,15 +80,15 @@
         Initializes the server
         """
         logging.basicConfig(filename=f"{constants.LOG_FILES.HOST_MANAGER_LOG_DIR}"
                                      f"{constants.LOG_FILES.HOST_MANAGER_LOG_FILE}", level=logging.INFO)
         self.hostname = socket.gethostname()
         try:
             self.ip = netifaces.ifaddresses(constants.INTERFACES.ETH0)[netifaces.AF_INET][0][constants.INTERFACES.ADDR]
-        except:
+        except Exception:
             self.ip = socket.gethostbyname(self.hostname)
         self.conf = {constants.KAFKA.BOOTSTRAP_SERVERS_PROPERTY: f"{self.ip}:{constants.KAFKA.PORT}",
                      constants.KAFKA.CLIENT_ID_PROPERTY: self.hostname}
         self.host_monitor_thread = None
         logging.info(f"Starting the HostManager hostname: {self.hostname} ip: {self.ip}")
 
     def getIdsAlerts(self, request: csle_collector.host_manager.host_manager_pb2.GetHostMetricsMsg,
@@ -499,14 +500,64 @@
         heartbeat_status = HostManagerServicer._get_heartbeat_status()
         return csle_collector.host_manager.host_manager_pb2.HostStatusDTO(monitor_running=monitor_running,
                                                                           filebeat_running=filebeat_running,
                                                                           packetbeat_running=packetbeat_status,
                                                                           metricbeat_running=metricbeat_status,
                                                                           heartbeat_running=heartbeat_status)
 
+    def startSpark(self, request: csle_collector.host_manager.host_manager_pb2.StartSparkMsg,
+                   context: grpc.ServicerContext) -> csle_collector.host_manager.host_manager_pb2.HostStatusDTO:
+        """
+        Starts Spark
+
+        :param request: the gRPC request
+        :param context: the gRPC context
+        :return: a DTO with the status of the Host
+        """
+        logging.info("Starting spark")
+        HostManagerServicer._start_spark()
+        logging.info("Started spark")
+        monitor_running = False
+        if self.host_monitor_thread is not None:
+            monitor_running = self.host_monitor_thread.running
+        packetbeat_status = HostManagerServicer._get_packetbeat_status()
+        filebeat_status = HostManagerServicer._get_filebeat_status()
+        metricbeat_status = HostManagerServicer._get_metricbeat_status()
+        heartbeat_status = HostManagerServicer._get_heartbeat_status()
+        return csle_collector.host_manager.host_manager_pb2.HostStatusDTO(monitor_running=monitor_running,
+                                                                          filebeat_running=filebeat_status,
+                                                                          packetbeat_running=packetbeat_status,
+                                                                          metricbeat_running=metricbeat_status,
+                                                                          heartbeat_running=heartbeat_status)
+
+    def stopSpark(self, request: csle_collector.host_manager.host_manager_pb2.StopSparkMsg,
+                  context: grpc.ServicerContext) -> csle_collector.host_manager.host_manager_pb2.HostStatusDTO:
+        """
+        Stops Spark
+
+        :param request: the gRPC request
+        :param context: the gRPC context
+        :return: a DTO with the status of the Host
+        """
+        logging.info("Stopping spark")
+        HostManagerServicer._stop_spark()
+        logging.info("Stopped spark")
+        monitor_running = False
+        if self.host_monitor_thread is not None:
+            monitor_running = self.host_monitor_thread.running
+        packetbeat_status = HostManagerServicer._get_packetbeat_status()
+        filebeat_status = HostManagerServicer._get_filebeat_status()
+        metricbeat_status = HostManagerServicer._get_metricbeat_status()
+        heartbeat_status = HostManagerServicer._get_heartbeat_status()
+        return csle_collector.host_manager.host_manager_pb2.HostStatusDTO(monitor_running=monitor_running,
+                                                                          filebeat_running=filebeat_status,
+                                                                          packetbeat_running=packetbeat_status,
+                                                                          metricbeat_running=metricbeat_status,
+                                                                          heartbeat_running=heartbeat_status)
+
     @staticmethod
     def _get_filebeat_status() -> bool:
         """
         Utility method to get the status of filebeat
 
         :return: status of filebeat
         """
@@ -986,14 +1037,60 @@
         :return: None
         """
         logging.info(f"Stopping heartbeat with command: {constants.HEARTBEAT.HEARTBEAT_STOP}")
         output = subprocess.run(constants.HEARTBEAT.HEARTBEAT_STOP.split(" "), capture_output=True, text=True)
         logging.info(f"Stopped heartbeat, output:{output.stdout}, err output: {output.stderr} ")
 
     @staticmethod
+    def _read_pid_file(path: str) -> int:
+        """
+        Reads the PID from a pidfile
+
+        :param path: the path to the file
+        :return: the parsed pid, or -1 if the pidfile could not be read
+        """
+        if os.path.exists(path):
+            pid = int(open(path, "r").read())
+            return pid
+        return -1
+
+    @staticmethod
+    def _start_spark() -> None:
+        """
+        Utility method to start spark
+
+        :return: None
+        """
+        logging.info(f"Starting spark master with command: {constants.SPARK.START_SPARK_MASTER}")
+        output = subprocess.run(constants.SPARK.START_SPARK_MASTER.split(" "), capture_output=True, text=True)
+        logging.info(f"Started spark master, stdout:{output.stdout}, stderr: {output.stderr}")
+        time.sleep(5)
+        logging.info(f"Starting spark worker with command: {constants.SPARK.START_SPARK_WORKER}")
+        output = subprocess.run(constants.SPARK.START_SPARK_WORKER.split(" "), capture_output=True, text=True)
+        logging.info(f"Started spark worker, stdout:{output.stdout}, stderr: {output.stderr}")
+
+    @staticmethod
+    def _stop_spark() -> None:
+        """
+        Utility method to stop spark
+
+        :return: None
+        """
+        worker_pid = HostManagerServicer._read_pid_file(constants.SPARK.SPARK_WORKER_PID_FILE)
+        logging.info(f"Stopping spark worker with command: {constants.SPARK.STOP_SPARK_WORKER.format(worker_pid)}")
+        output = subprocess.run(constants.SPARK.STOP_SPARK_WORKER.format(worker_pid).split(" "),
+                                capture_output=True, text=True)
+        logging.info(f"Stopped the spark worker, output:{output.stdout}, err output: {output.stderr} ")
+        master_pid = HostManagerServicer._read_pid_file(constants.SPARK.SPARK_MASTER_PID_FILE)
+        logging.info(f"Stopping spark master with command: {constants.SPARK.STOP_SPARK_MASTER.format(master_pid)}")
+        output = subprocess.run(constants.SPARK.STOP_SPARK_MASTER.format(master_pid).split(" "),
+                                capture_output=True, text=True)
+        logging.info(f"Stopped the spark master, output:{output.stdout}, err output: {output.stderr} ")
+
+    @staticmethod
     def _set_heartbeat_config(kibana_ip: str, kibana_port: int, elastic_ip: str,
                               elastic_port: int, num_elastic_shards: int, hosts_to_monitor: List[str]) -> None:
         """
         Updates the heartbeat configuration file
 
         :param hosts_to_monitor: the list of hosts to monitor
         :param kibana_ip: the IP of Kibana where the data should be visualized
```

### Comparing `csle_collector-0.1.9/src/csle_collector/host_manager/host_manager_pb2.py` & `csle_collector-0.2.0/src/csle_collector/host_manager/host_manager_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12host_manager.proto\"\x14\n\x12StopHostMonitorMsg\"Z\n\x13StartHostMonitorMsg\x12\x10\n\x08kafka_ip\x18\x01 \x01(\t\x12\x12\n\nkafka_port\x18\x02 \x01(\x05\x12\x1d\n\x15time_step_len_seconds\x18\x04 \x01(\x05\"\x11\n\x0fStopFilebeatMsg\"\x12\n\x10StartFilebeatMsg\"\x97\x02\n\x11\x43onfigFilebeatMsg\x12\x11\n\tkibana_ip\x18\x01 \x01(\t\x12\x13\n\x0bkibana_port\x18\x02 \x01(\x05\x12\x12\n\nelastic_ip\x18\x03 \x01(\t\x12\x14\n\x0c\x65lastic_port\x18\x04 \x01(\x05\x12\x1a\n\x12num_elastic_shards\x18\x05 \x01(\x05\x12\x16\n\x0ereload_enabled\x18\x06 \x01(\x08\x12\x10\n\x08kafka_ip\x18\x07 \x01(\t\x12\x12\n\nkafka_port\x18\x08 \x01(\x05\x12\r\n\x05kafka\x18\t \x01(\x08\x12\x14\n\x0ckafka_topics\x18\n \x03(\t\x12\x18\n\x10\x66ilebeat_modules\x18\x0b \x03(\t\x12\x17\n\x0flog_files_paths\x18\x0c \x03(\t\"\x13\n\x11StopPacketbeatMsg\"\x14\n\x12StartPacketbeatMsg\"\x83\x01\n\x13\x43onfigPacketbeatMsg\x12\x11\n\tkibana_ip\x18\x01 \x01(\t\x12\x13\n\x0bkibana_port\x18\x02 \x01(\x05\x12\x12\n\nelastic_ip\x18\x03 \x01(\t\x12\x14\n\x0c\x65lastic_port\x18\x04 \x01(\x05\x12\x1a\n\x12num_elastic_shards\x18\x05 \x01(\x05\"\x13\n\x11StopMetricbeatMsg\"\x14\n\x12StartMetricbeatMsg\"\xdd\x01\n\x13\x43onfigMetricbeatMsg\x12\x11\n\tkibana_ip\x18\x01 \x01(\t\x12\x13\n\x0bkibana_port\x18\x02 \x01(\x05\x12\x12\n\nelastic_ip\x18\x03 \x01(\t\x12\x14\n\x0c\x65lastic_port\x18\x04 \x01(\x05\x12\x1a\n\x12num_elastic_shards\x18\x05 \x01(\x05\x12\x10\n\x08kafka_ip\x18\x06 \x01(\t\x12\x12\n\nkafka_port\x18\x07 \x01(\x05\x12\x16\n\x0ereload_enabled\x18\x08 \x01(\x08\x12\x1a\n\x12metricbeat_modules\x18\x0c \x03(\t\"\x12\n\x10GetHostStatusMsg\"\x95\x01\n\rHostStatusDTO\x12\x17\n\x0fmonitor_running\x18\x01 \x01(\x08\x12\x18\n\x10\x66ilebeat_running\x18\x02 \x01(\x08\x12\x1a\n\x12packetbeat_running\x18\x03 \x01(\x08\x12\x1a\n\x12metricbeat_running\x18\x04 \x01(\x08\x12\x19\n\x11heartbeat_running\x18\x05 \x01(\x08\"G\n\x11GetHostMetricsMsg\x12\x1b\n\x13\x66\x61iled_auth_last_ts\x18\x01 \x01(\x02\x12\x15\n\rlogin_last_ts\x18\x02 \x01(\x02\"\xd1\x01\n\x0eHostMetricsDTO\x12\x1b\n\x13num_logged_in_users\x18\x01 \x01(\x05\x12!\n\x19num_failed_login_attempts\x18\x02 \x01(\x05\x12\x1c\n\x14num_open_connections\x18\x03 \x01(\x05\x12\x18\n\x10num_login_events\x18\x04 \x01(\x05\x12\x15\n\rnum_processes\x18\x05 \x01(\x05\x12\x11\n\tnum_users\x18\x06 \x01(\x05\x12\n\n\x02ip\x18\x07 \x01(\t\x12\x11\n\ttimestamp\x18\x08 \x01(\x02\"\x12\n\x10StopHeartbeatMsg\"\x13\n\x11StartHeartbeatMsg\"\x9c\x01\n\x12\x43onfigHeartbeatMsg\x12\x11\n\tkibana_ip\x18\x01 \x01(\t\x12\x13\n\x0bkibana_port\x18\x02 \x01(\x05\x12\x12\n\nelastic_ip\x18\x03 \x01(\t\x12\x14\n\x0c\x65lastic_port\x18\x04 \x01(\x05\x12\x1a\n\x12num_elastic_shards\x18\x05 \x01(\x05\x12\x18\n\x10hosts_to_monitor\x18\x06 \x03(\t2\x98\x07\n\x0bHostManager\x12\x38\n\x0fstopHostMonitor\x12\x13.StopHostMonitorMsg\x1a\x0e.HostStatusDTO\"\x00\x12:\n\x10startHostMonitor\x12\x14.StartHostMonitorMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x34\n\rgetHostStatus\x12\x11.GetHostStatusMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x37\n\x0egetHostMetrics\x12\x12.GetHostMetricsMsg\x1a\x0f.HostMetricsDTO\"\x00\x12\x32\n\x0cstopFilebeat\x12\x10.StopFilebeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x34\n\rstartFilebeat\x12\x11.StartFilebeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x36\n\x0e\x63onfigFilebeat\x12\x12.ConfigFilebeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x36\n\x0estopPacketbeat\x12\x12.StopPacketbeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x38\n\x0fstartPacketbeat\x12\x13.StartPacketbeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12:\n\x10\x63onfigPacketbeat\x12\x14.ConfigPacketbeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x36\n\x0estopMetricbeat\x12\x12.StopMetricbeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x38\n\x0fstartMetricbeat\x12\x13.StartMetricbeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12:\n\x10\x63onfigMetricbeat\x12\x14.ConfigMetricbeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x34\n\rstopHeartbeat\x12\x11.StopHeartbeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x36\n\x0estartHeartbeat\x12\x12.StartHeartbeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x38\n\x0f\x63onfigHeartbeat\x12\x13.ConfigHeartbeatMsg\x1a\x0e.HostStatusDTO\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12host_manager.proto\"\x0e\n\x0cStopSparkMsg\"\x0f\n\rStartSparkMsg\"\x14\n\x12StopHostMonitorMsg\"Z\n\x13StartHostMonitorMsg\x12\x10\n\x08kafka_ip\x18\x01 \x01(\t\x12\x12\n\nkafka_port\x18\x02 \x01(\x05\x12\x1d\n\x15time_step_len_seconds\x18\x04 \x01(\x05\"\x11\n\x0fStopFilebeatMsg\"\x12\n\x10StartFilebeatMsg\"\x97\x02\n\x11\x43onfigFilebeatMsg\x12\x11\n\tkibana_ip\x18\x01 \x01(\t\x12\x13\n\x0bkibana_port\x18\x02 \x01(\x05\x12\x12\n\nelastic_ip\x18\x03 \x01(\t\x12\x14\n\x0c\x65lastic_port\x18\x04 \x01(\x05\x12\x1a\n\x12num_elastic_shards\x18\x05 \x01(\x05\x12\x16\n\x0ereload_enabled\x18\x06 \x01(\x08\x12\x10\n\x08kafka_ip\x18\x07 \x01(\t\x12\x12\n\nkafka_port\x18\x08 \x01(\x05\x12\r\n\x05kafka\x18\t \x01(\x08\x12\x14\n\x0ckafka_topics\x18\n \x03(\t\x12\x18\n\x10\x66ilebeat_modules\x18\x0b \x03(\t\x12\x17\n\x0flog_files_paths\x18\x0c \x03(\t\"\x13\n\x11StopPacketbeatMsg\"\x14\n\x12StartPacketbeatMsg\"\x83\x01\n\x13\x43onfigPacketbeatMsg\x12\x11\n\tkibana_ip\x18\x01 \x01(\t\x12\x13\n\x0bkibana_port\x18\x02 \x01(\x05\x12\x12\n\nelastic_ip\x18\x03 \x01(\t\x12\x14\n\x0c\x65lastic_port\x18\x04 \x01(\x05\x12\x1a\n\x12num_elastic_shards\x18\x05 \x01(\x05\"\x13\n\x11StopMetricbeatMsg\"\x14\n\x12StartMetricbeatMsg\"\xdd\x01\n\x13\x43onfigMetricbeatMsg\x12\x11\n\tkibana_ip\x18\x01 \x01(\t\x12\x13\n\x0bkibana_port\x18\x02 \x01(\x05\x12\x12\n\nelastic_ip\x18\x03 \x01(\t\x12\x14\n\x0c\x65lastic_port\x18\x04 \x01(\x05\x12\x1a\n\x12num_elastic_shards\x18\x05 \x01(\x05\x12\x10\n\x08kafka_ip\x18\x06 \x01(\t\x12\x12\n\nkafka_port\x18\x07 \x01(\x05\x12\x16\n\x0ereload_enabled\x18\x08 \x01(\x08\x12\x1a\n\x12metricbeat_modules\x18\x0c \x03(\t\"\x12\n\x10GetHostStatusMsg\"\x95\x01\n\rHostStatusDTO\x12\x17\n\x0fmonitor_running\x18\x01 \x01(\x08\x12\x18\n\x10\x66ilebeat_running\x18\x02 \x01(\x08\x12\x1a\n\x12packetbeat_running\x18\x03 \x01(\x08\x12\x1a\n\x12metricbeat_running\x18\x04 \x01(\x08\x12\x19\n\x11heartbeat_running\x18\x05 \x01(\x08\"G\n\x11GetHostMetricsMsg\x12\x1b\n\x13\x66\x61iled_auth_last_ts\x18\x01 \x01(\x02\x12\x15\n\rlogin_last_ts\x18\x02 \x01(\x02\"\xd1\x01\n\x0eHostMetricsDTO\x12\x1b\n\x13num_logged_in_users\x18\x01 \x01(\x05\x12!\n\x19num_failed_login_attempts\x18\x02 \x01(\x05\x12\x1c\n\x14num_open_connections\x18\x03 \x01(\x05\x12\x18\n\x10num_login_events\x18\x04 \x01(\x05\x12\x15\n\rnum_processes\x18\x05 \x01(\x05\x12\x11\n\tnum_users\x18\x06 \x01(\x05\x12\n\n\x02ip\x18\x07 \x01(\t\x12\x11\n\ttimestamp\x18\x08 \x01(\x02\"\x12\n\x10StopHeartbeatMsg\"\x13\n\x11StartHeartbeatMsg\"\x9c\x01\n\x12\x43onfigHeartbeatMsg\x12\x11\n\tkibana_ip\x18\x01 \x01(\t\x12\x13\n\x0bkibana_port\x18\x02 \x01(\x05\x12\x12\n\nelastic_ip\x18\x03 \x01(\t\x12\x14\n\x0c\x65lastic_port\x18\x04 \x01(\x05\x12\x1a\n\x12num_elastic_shards\x18\x05 \x01(\x05\x12\x18\n\x10hosts_to_monitor\x18\x06 \x03(\t2\xf6\x07\n\x0bHostManager\x12\x38\n\x0fstopHostMonitor\x12\x13.StopHostMonitorMsg\x1a\x0e.HostStatusDTO\"\x00\x12:\n\x10startHostMonitor\x12\x14.StartHostMonitorMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x34\n\rgetHostStatus\x12\x11.GetHostStatusMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x37\n\x0egetHostMetrics\x12\x12.GetHostMetricsMsg\x1a\x0f.HostMetricsDTO\"\x00\x12\x32\n\x0cstopFilebeat\x12\x10.StopFilebeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x34\n\rstartFilebeat\x12\x11.StartFilebeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x36\n\x0e\x63onfigFilebeat\x12\x12.ConfigFilebeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x36\n\x0estopPacketbeat\x12\x12.StopPacketbeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x38\n\x0fstartPacketbeat\x12\x13.StartPacketbeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12:\n\x10\x63onfigPacketbeat\x12\x14.ConfigPacketbeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x36\n\x0estopMetricbeat\x12\x12.StopMetricbeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x38\n\x0fstartMetricbeat\x12\x13.StartMetricbeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12:\n\x10\x63onfigMetricbeat\x12\x14.ConfigMetricbeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x34\n\rstopHeartbeat\x12\x11.StopHeartbeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x36\n\x0estartHeartbeat\x12\x12.StartHeartbeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12\x38\n\x0f\x63onfigHeartbeat\x12\x13.ConfigHeartbeatMsg\x1a\x0e.HostStatusDTO\"\x00\x12,\n\tstopSpark\x12\r.StopSparkMsg\x1a\x0e.HostStatusDTO\"\x00\x12.\n\nstartSpark\x12\x0e.StartSparkMsg\x1a\x0e.HostStatusDTO\"\x00\x62\x06proto3')
 
 
 
+_STOPSPARKMSG = DESCRIPTOR.message_types_by_name['StopSparkMsg']
+_STARTSPARKMSG = DESCRIPTOR.message_types_by_name['StartSparkMsg']
 _STOPHOSTMONITORMSG = DESCRIPTOR.message_types_by_name['StopHostMonitorMsg']
 _STARTHOSTMONITORMSG = DESCRIPTOR.message_types_by_name['StartHostMonitorMsg']
 _STOPFILEBEATMSG = DESCRIPTOR.message_types_by_name['StopFilebeatMsg']
 _STARTFILEBEATMSG = DESCRIPTOR.message_types_by_name['StartFilebeatMsg']
 _CONFIGFILEBEATMSG = DESCRIPTOR.message_types_by_name['ConfigFilebeatMsg']
 _STOPPACKETBEATMSG = DESCRIPTOR.message_types_by_name['StopPacketbeatMsg']
 _STARTPACKETBEATMSG = DESCRIPTOR.message_types_by_name['StartPacketbeatMsg']
@@ -32,14 +34,28 @@
 _GETHOSTSTATUSMSG = DESCRIPTOR.message_types_by_name['GetHostStatusMsg']
 _HOSTSTATUSDTO = DESCRIPTOR.message_types_by_name['HostStatusDTO']
 _GETHOSTMETRICSMSG = DESCRIPTOR.message_types_by_name['GetHostMetricsMsg']
 _HOSTMETRICSDTO = DESCRIPTOR.message_types_by_name['HostMetricsDTO']
 _STOPHEARTBEATMSG = DESCRIPTOR.message_types_by_name['StopHeartbeatMsg']
 _STARTHEARTBEATMSG = DESCRIPTOR.message_types_by_name['StartHeartbeatMsg']
 _CONFIGHEARTBEATMSG = DESCRIPTOR.message_types_by_name['ConfigHeartbeatMsg']
+StopSparkMsg = _reflection.GeneratedProtocolMessageType('StopSparkMsg', (_message.Message,), {
+  'DESCRIPTOR' : _STOPSPARKMSG,
+  '__module__' : 'host_manager_pb2'
+  # @@protoc_insertion_point(class_scope:StopSparkMsg)
+  })
+_sym_db.RegisterMessage(StopSparkMsg)
+
+StartSparkMsg = _reflection.GeneratedProtocolMessageType('StartSparkMsg', (_message.Message,), {
+  'DESCRIPTOR' : _STARTSPARKMSG,
+  '__module__' : 'host_manager_pb2'
+  # @@protoc_insertion_point(class_scope:StartSparkMsg)
+  })
+_sym_db.RegisterMessage(StartSparkMsg)
+
 StopHostMonitorMsg = _reflection.GeneratedProtocolMessageType('StopHostMonitorMsg', (_message.Message,), {
   'DESCRIPTOR' : _STOPHOSTMONITORMSG,
   '__module__' : 'host_manager_pb2'
   # @@protoc_insertion_point(class_scope:StopHostMonitorMsg)
   })
 _sym_db.RegisterMessage(StopHostMonitorMsg)
 
@@ -162,46 +178,50 @@
   })
 _sym_db.RegisterMessage(ConfigHeartbeatMsg)
 
 _HOSTMANAGER = DESCRIPTOR.services_by_name['HostManager']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _STOPHOSTMONITORMSG._serialized_start=22
-  _STOPHOSTMONITORMSG._serialized_end=42
-  _STARTHOSTMONITORMSG._serialized_start=44
-  _STARTHOSTMONITORMSG._serialized_end=134
-  _STOPFILEBEATMSG._serialized_start=136
-  _STOPFILEBEATMSG._serialized_end=153
-  _STARTFILEBEATMSG._serialized_start=155
-  _STARTFILEBEATMSG._serialized_end=173
-  _CONFIGFILEBEATMSG._serialized_start=176
-  _CONFIGFILEBEATMSG._serialized_end=455
-  _STOPPACKETBEATMSG._serialized_start=457
-  _STOPPACKETBEATMSG._serialized_end=476
-  _STARTPACKETBEATMSG._serialized_start=478
-  _STARTPACKETBEATMSG._serialized_end=498
-  _CONFIGPACKETBEATMSG._serialized_start=501
-  _CONFIGPACKETBEATMSG._serialized_end=632
-  _STOPMETRICBEATMSG._serialized_start=634
-  _STOPMETRICBEATMSG._serialized_end=653
-  _STARTMETRICBEATMSG._serialized_start=655
-  _STARTMETRICBEATMSG._serialized_end=675
-  _CONFIGMETRICBEATMSG._serialized_start=678
-  _CONFIGMETRICBEATMSG._serialized_end=899
-  _GETHOSTSTATUSMSG._serialized_start=901
-  _GETHOSTSTATUSMSG._serialized_end=919
-  _HOSTSTATUSDTO._serialized_start=922
-  _HOSTSTATUSDTO._serialized_end=1071
-  _GETHOSTMETRICSMSG._serialized_start=1073
-  _GETHOSTMETRICSMSG._serialized_end=1144
-  _HOSTMETRICSDTO._serialized_start=1147
-  _HOSTMETRICSDTO._serialized_end=1356
-  _STOPHEARTBEATMSG._serialized_start=1358
-  _STOPHEARTBEATMSG._serialized_end=1376
-  _STARTHEARTBEATMSG._serialized_start=1378
-  _STARTHEARTBEATMSG._serialized_end=1397
-  _CONFIGHEARTBEATMSG._serialized_start=1400
-  _CONFIGHEARTBEATMSG._serialized_end=1556
-  _HOSTMANAGER._serialized_start=1559
-  _HOSTMANAGER._serialized_end=2479
+  _STOPSPARKMSG._serialized_start=22
+  _STOPSPARKMSG._serialized_end=36
+  _STARTSPARKMSG._serialized_start=38
+  _STARTSPARKMSG._serialized_end=53
+  _STOPHOSTMONITORMSG._serialized_start=55
+  _STOPHOSTMONITORMSG._serialized_end=75
+  _STARTHOSTMONITORMSG._serialized_start=77
+  _STARTHOSTMONITORMSG._serialized_end=167
+  _STOPFILEBEATMSG._serialized_start=169
+  _STOPFILEBEATMSG._serialized_end=186
+  _STARTFILEBEATMSG._serialized_start=188
+  _STARTFILEBEATMSG._serialized_end=206
+  _CONFIGFILEBEATMSG._serialized_start=209
+  _CONFIGFILEBEATMSG._serialized_end=488
+  _STOPPACKETBEATMSG._serialized_start=490
+  _STOPPACKETBEATMSG._serialized_end=509
+  _STARTPACKETBEATMSG._serialized_start=511
+  _STARTPACKETBEATMSG._serialized_end=531
+  _CONFIGPACKETBEATMSG._serialized_start=534
+  _CONFIGPACKETBEATMSG._serialized_end=665
+  _STOPMETRICBEATMSG._serialized_start=667
+  _STOPMETRICBEATMSG._serialized_end=686
+  _STARTMETRICBEATMSG._serialized_start=688
+  _STARTMETRICBEATMSG._serialized_end=708
+  _CONFIGMETRICBEATMSG._serialized_start=711
+  _CONFIGMETRICBEATMSG._serialized_end=932
+  _GETHOSTSTATUSMSG._serialized_start=934
+  _GETHOSTSTATUSMSG._serialized_end=952
+  _HOSTSTATUSDTO._serialized_start=955
+  _HOSTSTATUSDTO._serialized_end=1104
+  _GETHOSTMETRICSMSG._serialized_start=1106
+  _GETHOSTMETRICSMSG._serialized_end=1177
+  _HOSTMETRICSDTO._serialized_start=1180
+  _HOSTMETRICSDTO._serialized_end=1389
+  _STOPHEARTBEATMSG._serialized_start=1391
+  _STOPHEARTBEATMSG._serialized_end=1409
+  _STARTHEARTBEATMSG._serialized_start=1411
+  _STARTHEARTBEATMSG._serialized_end=1430
+  _CONFIGHEARTBEATMSG._serialized_start=1433
+  _CONFIGHEARTBEATMSG._serialized_end=1589
+  _HOSTMANAGER._serialized_start=1592
+  _HOSTMANAGER._serialized_end=2606
 # @@protoc_insertion_point(module_scope)
```

### Comparing `csle_collector-0.1.9/src/csle_collector/host_manager/host_manager_pb2_grpc.py` & `csle_collector-0.2.0/src/csle_collector/host_manager/host_manager_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,24 @@
                 response_deserializer=host__manager__pb2.HostStatusDTO.FromString,
                 )
         self.configHeartbeat = channel.unary_unary(
                 '/HostManager/configHeartbeat',
                 request_serializer=host__manager__pb2.ConfigHeartbeatMsg.SerializeToString,
                 response_deserializer=host__manager__pb2.HostStatusDTO.FromString,
                 )
+        self.stopSpark = channel.unary_unary(
+                '/HostManager/stopSpark',
+                request_serializer=host__manager__pb2.StopSparkMsg.SerializeToString,
+                response_deserializer=host__manager__pb2.HostStatusDTO.FromString,
+                )
+        self.startSpark = channel.unary_unary(
+                '/HostManager/startSpark',
+                request_serializer=host__manager__pb2.StartSparkMsg.SerializeToString,
+                response_deserializer=host__manager__pb2.HostStatusDTO.FromString,
+                )
 
 
 class HostManagerServicer(object):
     """Interface exported by the server
     """
 
     def stopHostMonitor(self, request, context):
@@ -193,14 +203,26 @@
 
     def configHeartbeat(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def stopSpark(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def startSpark(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_HostManagerServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'stopHostMonitor': grpc.unary_unary_rpc_method_handler(
                     servicer.stopHostMonitor,
                     request_deserializer=host__manager__pb2.StopHostMonitorMsg.FromString,
                     response_serializer=host__manager__pb2.HostStatusDTO.SerializeToString,
@@ -276,14 +298,24 @@
                     response_serializer=host__manager__pb2.HostStatusDTO.SerializeToString,
             ),
             'configHeartbeat': grpc.unary_unary_rpc_method_handler(
                     servicer.configHeartbeat,
                     request_deserializer=host__manager__pb2.ConfigHeartbeatMsg.FromString,
                     response_serializer=host__manager__pb2.HostStatusDTO.SerializeToString,
             ),
+            'stopSpark': grpc.unary_unary_rpc_method_handler(
+                    servicer.stopSpark,
+                    request_deserializer=host__manager__pb2.StopSparkMsg.FromString,
+                    response_serializer=host__manager__pb2.HostStatusDTO.SerializeToString,
+            ),
+            'startSpark': grpc.unary_unary_rpc_method_handler(
+                    servicer.startSpark,
+                    request_deserializer=host__manager__pb2.StartSparkMsg.FromString,
+                    response_serializer=host__manager__pb2.HostStatusDTO.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'HostManager', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -558,7 +590,41 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/HostManager/configHeartbeat',
             host__manager__pb2.ConfigHeartbeatMsg.SerializeToString,
             host__manager__pb2.HostStatusDTO.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def stopSpark(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/HostManager/stopSpark',
+            host__manager__pb2.StopSparkMsg.SerializeToString,
+            host__manager__pb2.HostStatusDTO.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def startSpark(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/HostManager/startSpark',
+            host__manager__pb2.StartSparkMsg.SerializeToString,
+            host__manager__pb2.HostStatusDTO.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `csle_collector-0.1.9/src/csle_collector/host_manager/host_manager_util.py` & `csle_collector-0.2.0/src/csle_collector/host_manager/host_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/host_manager/host_metrics.py` & `csle_collector-0.2.0/src/csle_collector/host_manager/host_metrics.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/host_manager/query_host_manager.py` & `csle_collector-0.2.0/src/csle_collector/host_manager/query_host_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -317,7 +317,38 @@
     """
     config_heartbeat_msg = \
         csle_collector.host_manager.host_manager_pb2.ConfigHeartbeatMsg(
             kibana_ip=kibana_ip, kibana_port=kibana_port, elastic_ip=elastic_ip,
             elastic_port=elastic_port, num_elastic_shards=num_elastic_shards, hosts_to_monitor=hosts_to_monitor)
     host_dto = stub.configHeartbeat(config_heartbeat_msg, timeout=timeout)
     return host_dto
+
+
+def start_spark(
+        stub: csle_collector.host_manager.host_manager_pb2_grpc.HostManagerStub,
+        timeout=constants.GRPC.TIMEOUT_SECONDS) -> csle_collector.host_manager.host_manager_pb2.HostStatusDTO:
+    """
+    Sends a request to the Host manager to start spark
+
+    :param stub: the stub to send the remote gRPC to the server
+    :param timeout: the GRPC timeout (seconds)
+    :return: a HostDTO describing the host status
+    """
+    start_spark_msg = csle_collector.host_manager.host_manager_pb2.StartSparkMsg()
+    host_dto = stub.startSpark(start_spark_msg, timeout=timeout)
+    return host_dto
+
+
+def stop_spark(
+        stub: csle_collector.host_manager.host_manager_pb2_grpc.HostManagerStub,
+        timeout=constants.GRPC.TIMEOUT_SECONDS) -> csle_collector.host_manager.host_manager_pb2.HostStatusDTO:
+    """
+    Sends a request to the Host manager to stop spark
+
+    :param stub: the stub to send the remote gRPC to the server
+    :param timeout: the GRPC timeout (seconds)
+    :return: a HostDTO describing the host status
+    """
+    stop_spark_msg = \
+        csle_collector.host_manager.host_manager_pb2.StopSparkMsg()
+    host_dto = stub.stopSpark(stop_spark_msg, timeout=timeout)
+    return host_dto
```

### Comparing `csle_collector-0.1.9/src/csle_collector/host_manager/successful_login.py` & `csle_collector-0.2.0/src/csle_collector/host_manager/successful_login.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/kafka_manager/kafka_manager.py` & `csle_collector-0.2.0/src/csle_collector/kafka_manager/kafka_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         Initializes the server
         """
         logging.basicConfig(filename=f"{constants.LOG_FILES.KAFKA_MANAGER_LOG_DIR}"
                                      f"{constants.LOG_FILES.KAFKA_MANAGER_LOG_FILE}", level=logging.INFO)
         self.hostname = socket.gethostname()
         try:
             self.ip = netifaces.ifaddresses(constants.INTERFACES.ETH0)[netifaces.AF_INET][0][constants.INTERFACES.ADDR]
-        except:
+        except Exception:
             self.ip = socket.gethostbyname(self.hostname)
         self.conf = {constants.KAFKA.BOOTSTRAP_SERVERS_PROPERTY: f"{self.ip}:{constants.KAFKA.PORT}",
                      constants.KAFKA.CLIENT_ID_PROPERTY: self.hostname}
         logging.info(f"Setting up KafkaManager hostname: {self.hostname} ip: {self.ip}")
 
     def _get_kafka_status_and_topics(self) -> Tuple[bool, List[str]]:
         """
```

### Comparing `csle_collector-0.1.9/src/csle_collector/kafka_manager/kafka_manager_pb2.py` & `csle_collector-0.2.0/src/csle_collector/kafka_manager/kafka_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py` & `csle_collector-0.2.0/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/kafka_manager/kafka_manager_util.py` & `csle_collector-0.2.0/src/csle_collector/kafka_manager/kafka_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/kafka_manager/query_kafka_server.py` & `csle_collector-0.2.0/src/csle_collector/kafka_manager/query_kafka_server.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py` & `csle_collector-0.2.0/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py` & `csle_collector-0.2.0/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py` & `csle_collector-0.2.0/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         Initializes the server
         """
         logging.basicConfig(filename=f"{constants.LOG_FILES.OSSEC_IDS_MANAGER_LOG_DIR}"
                                      f"{constants.LOG_FILES.OSSEC_IDS_MANAGER_LOG_FILE}", level=logging.INFO)
         self.hostname = socket.gethostname()
         try:
             self.ip = netifaces.ifaddresses(constants.INTERFACES.ETH0)[netifaces.AF_INET][0][constants.INTERFACES.ADDR]
-        except:
+        except Exception:
             self.ip = socket.gethostbyname(self.hostname)
         self.conf = {
             constants.KAFKA.BOOTSTRAP_SERVERS_PROPERTY: f"{self.ip}:{constants.KAFKA.PORT}",
             constants.KAFKA.CLIENT_ID_PROPERTY: self.hostname}
         self.ids_monitor_thread = None
         logging.info(f"Starting the OSSEC IDSManager hostname: {self.hostname} ip: {self.ip}")
```

### Comparing `csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py` & `csle_collector-0.2.0/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py` & `csle_collector-0.2.0/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py` & `csle_collector-0.2.0/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py` & `csle_collector-0.2.0/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/ryu_manager/query_ryu_server.py` & `csle_collector-0.2.0/src/csle_collector/ryu_manager/query_ryu_server.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/ryu_manager/ryu_manager.py` & `csle_collector-0.2.0/src/csle_collector/ryu_manager/ryu_manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,87 @@
 import logging
+import threading
+import time
 from concurrent import futures
 import grpc
 import socket
-import os
 import subprocess
 import json
 import netifaces
 import requests
 import csle_collector.ryu_manager.ryu_manager_pb2_grpc
 import csle_collector.ryu_manager.ryu_manager_pb2
 import csle_collector.constants.constants as constants
 
 
+class FailureDetector(threading.Thread):
+    """
+    Thread representing a client
+    """
+
+    def __init__(self, sleep_time: int, ip: str, ryu_web_port: int, ryu_port: int, controller: str, kafka_ip: str,
+                 kafka_port: int, time_step_len: int) -> None:
+        """
+        Initializes the failure detector
+
+        :param sleep_time: the period to check  for failures
+        :param ip: the ip of the host
+        :param ryu_web_port: the Ryu web port
+        :param ryu_port: the Ryu port
+        :param controller: the Ryu controller module
+        :param kafka_ip: the Kafka IP
+        :param kafka_port: the Kafka port
+        :param time_step_len: the time-step length for Kafka logging
+        """
+        threading.Thread.__init__(self)
+        self.sleep_time = sleep_time
+        self.ip = ip
+        self.ryu_web_port = ryu_web_port
+        self.ryu_port = ryu_port
+        self.controller = controller
+        self.kafka_ip = kafka_ip
+        self.kafka_port = kafka_port
+        self.time_step_len = time_step_len
+
+    def run(self) -> None:
+        """
+        The failure detector loop
+
+        :return: None
+        """
+        done = False
+        while not done:
+            status_url = f"{constants.HTTP.HTTP_PROTOCOL_PREFIX}{self.ip}:{self.ryu_web_port}" \
+                         f"{constants.RYU.STATUS_PRODUCER_HTTP_RESOURCE}"
+            try:
+                requests.get(status_url, timeout=constants.RYU.REQUEST_TIMEOUT_S)
+            except Exception:
+                logging.info("Restarting Ryu..")
+                cmd = constants.RYU.STOP_RYU_CONTROLLER
+                logging.info(f"Stopping ryu with command: {cmd}")
+                result = subprocess.run(cmd.split(" "), capture_output=True, text=True)
+                logging.info(f"Stdout: {result.stdout}, stderr: {result.stderr}")
+                cmd = constants.RYU.STOP_RYU_CONTROLLER_MANAGER
+                logging.info(f"Stopping ryu with command: {cmd}")
+                result = subprocess.run(cmd.split(" "), capture_output=True, text=True)
+                logging.info(f"Stdout: {result.stdout}, stderr: {result.stderr}")
+                cmd = constants.RYU.START_RYU_CONTROLLER.format(self.ryu_port, self.ryu_web_port, self.controller)
+                logging.info(f"Starting RYU controller with command: {cmd}")
+                subprocess.Popen(cmd, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+                time.sleep(5)
+                start_url = f"{constants.HTTP.HTTP_PROTOCOL_PREFIX}{self.ip}:{self.ryu_web_port}" \
+                            f"{constants.RYU.START_PRODUCER_HTTP_RESOURCE}"
+                logging.info(f"Starting the RYU monitor by sending a PUT request to: {start_url}")
+                requests.put(start_url, data=json.dumps({constants.KAFKA.BOOTSTRAP_SERVERS_PROPERTY: self.kafka_ip,
+                                                         constants.RYU.TIME_STEP_LEN_SECONDS: self.time_step_len}),
+                             timeout=constants.RYU.REQUEST_TIMEOUT_S)
+                logging.info("RYU monitor started")
+            time.sleep(self.sleep_time)
+
+
 class RyuManagerServicer(csle_collector.ryu_manager.ryu_manager_pb2_grpc.RyuManagerServicer):
     """
     gRPC server for managing a Ryu controller. Allows to start/stop the ryu controller remotely and also to query the
     state of the controller
     """
 
     def __init__(self) -> None:
@@ -23,22 +89,23 @@
         Initializes the server
         """
         logging.basicConfig(filename=f"{constants.LOG_FILES.RYU_MANAGER_LOG_DIR}"
                                      f"{constants.LOG_FILES.RYU_MANAGER_LOG_FILE}", level=logging.INFO)
         self.hostname = socket.gethostname()
         try:
             self.ip = netifaces.ifaddresses(constants.INTERFACES.ETH0)[netifaces.AF_INET][0][constants.INTERFACES.ADDR]
-        except:
+        except Exception:
             self.ip = socket.gethostbyname(self.hostname)
         self.ryu_port = 6633
         self.ryu_web_port = 8080
         self.controller = ""
         self.kafka_ip = ""
         self.kafka_port = 9092
         self.time_step_len = 30
+        self.fd = None
         logging.info(f"Setting up RyuManager hostname: {self.hostname} ip: {self.ip}")
 
     def _get_ryu_status(self) -> bool:
         """
         Utility method to get the status of Ryu
 
         :return: status
@@ -58,20 +125,41 @@
 
     def _get_monitor_status(self) -> bool:
         """
         Utility method to get the status of the monitor
 
         :return: status
         """
-        logging.info("Checking monitor status by sending a request to: "
-                     f"{constants.HTTP.HTTP_PROTOCOL_PREFIX}{self.ip}:{self.ryu_web_port}"
-                     f"{constants.RYU.STATUS_PRODUCER_HTTP_RESOURCE}")
-        response = requests.get(
-            f"{constants.HTTP.HTTP_PROTOCOL_PREFIX}{self.ip}:{self.ryu_web_port}"
-            f"{constants.RYU.STATUS_PRODUCER_HTTP_RESOURCE}")
+        status_url = f"{constants.HTTP.HTTP_PROTOCOL_PREFIX}{self.ip}:{self.ryu_web_port}" \
+                     f"{constants.RYU.STATUS_PRODUCER_HTTP_RESOURCE}"
+        logging.info(f"Checking monitor status by sending a request to: {status_url}")
+        try:
+            response = requests.get(status_url, timeout=constants.RYU.REQUEST_TIMEOUT_S)
+        except Exception as e:
+            logging.info(f"Timeout trying to check monitor status: {str(e)}, {repr(e)}")
+            logging.info("Restarting Ryu..")
+            cmd = constants.RYU.STOP_RYU_CONTROLLER
+            logging.info(f"Stopping ryu with command: {cmd}")
+            result = subprocess.run(cmd.split(" "), capture_output=True, text=True)
+            logging.info(f"Stdout: {result.stdout}, stderr: {result.stderr}")
+            cmd = constants.RYU.STOP_RYU_CONTROLLER_MANAGER
+            logging.info(f"Stopping ryu with command: {cmd}")
+            result = subprocess.run(cmd.split(" "), capture_output=True, text=True)
+            logging.info(f"Stdout: {result.stdout}, stderr: {result.stderr}")
+            cmd = constants.RYU.START_RYU_CONTROLLER.format(self.ryu_port, self.ryu_web_port, self.controller)
+            logging.info(f"Starting RYU controller with command: {cmd}")
+            subprocess.Popen(cmd, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+            start_url = f"{constants.HTTP.HTTP_PROTOCOL_PREFIX}{self.ip}:{self.ryu_web_port}" \
+                        f"{constants.RYU.START_PRODUCER_HTTP_RESOURCE}"
+            logging.info(f"Starting the RYU monitor by sending a PUT request to: {start_url}")
+            requests.put(start_url, data=json.dumps({constants.KAFKA.BOOTSTRAP_SERVERS_PROPERTY: self.kafka_ip,
+                                                     constants.RYU.TIME_STEP_LEN_SECONDS: self.time_step_len}),
+                         timeout=constants.RYU.REQUEST_TIMEOUT_S)
+            response = requests.get(status_url, timeout=constants.RYU.REQUEST_TIMEOUT_S)
+
         logging.info(f"Response: {response.json()}")
         monitor_running = response.json()[constants.RYU.PRODUCER_RUNNING]
         return monitor_running
 
     def getRyuStatus(self, request: csle_collector.ryu_manager.ryu_manager_pb2.GetRyuStatusMsg,
                      context: grpc.ServicerContext) \
             -> csle_collector.ryu_manager.ryu_manager_pb2.RyuDTO:
@@ -105,14 +193,18 @@
         :param context: the gRPC context
         :return: a clients DTO with the state of the ryu server
         """
         cmd = constants.RYU.STOP_RYU_CONTROLLER
         logging.info(f"Stopping ryu with command: {cmd}")
         result = subprocess.run(cmd.split(" "), capture_output=True, text=True)
         logging.info(f"Stdout: {result.stdout}, stderr: {result.stderr}")
+        cmd = constants.RYU.STOP_RYU_CONTROLLER_MANAGER
+        logging.info(f"Stopping ryu with command: {cmd}")
+        result = subprocess.run(cmd.split(" "), capture_output=True, text=True)
+        logging.info(f"Stdout: {result.stdout}, stderr: {result.stderr}")
         return csle_collector.ryu_manager.ryu_manager_pb2.RyuDTO(ryu_running=False, monitor_running=False,
                                                                  port=self.ryu_port,
                                                                  web_port=self.ryu_web_port,
                                                                  controller=self.controller,
                                                                  kafka_ip=self.kafka_ip,
                                                                  kafka_port=self.kafka_port,
                                                                  time_step_len=self.time_step_len)
@@ -133,18 +225,29 @@
         self.controller = request.controller
 
         # Check if controller is already running
         ryu_running = self._get_ryu_status()
         if not ryu_running:
             # Stop old background job if running
             cmd = constants.RYU.STOP_RYU_CONTROLLER
-            os.system(cmd)
+            subprocess.run(cmd.split(" "), capture_output=True, text=True)
+            cmd = constants.RYU.STOP_RYU_CONTROLLER_MANAGER
+            subprocess.run(cmd.split(" "), capture_output=True, text=True)
+            if self.fd is not None:
+                self.fd.done = True
+                self.fd = None
             cmd = constants.RYU.START_RYU_CONTROLLER.format(self.ryu_port, self.ryu_web_port, self.controller)
             logging.info(f"Starting RYU controller with command: {cmd}")
-            os.system(cmd)
+            subprocess.Popen(cmd, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+            logging.info("Starting the failure detector thread")
+            time.sleep(2)
+            fd = FailureDetector(sleep_time=30, ip=self.ip, ryu_web_port=self.ryu_web_port, ryu_port=self.ryu_port,
+                                 controller=self.controller, kafka_ip=self.kafka_ip, kafka_port=self.kafka_port,
+                                 time_step_len=self.time_step_len)
+            fd.start()
 
         ryu_dto = csle_collector.ryu_manager.ryu_manager_pb2.RyuDTO(ryu_running=True, monitor_running=False,
                                                                     port=self.ryu_port,
                                                                     web_port=self.ryu_web_port,
                                                                     controller=self.controller,
                                                                     kafka_ip=self.kafka_ip,
                                                                     kafka_port=self.kafka_port,
@@ -162,15 +265,15 @@
         """
         ryu_running = self._get_ryu_status()
         logging.info(f"Stopping Ryu monitor, sending a request to: "
                      f"{constants.HTTP.HTTP_PROTOCOL_PREFIX}{self.ip}:{self.ryu_web_port}"
                      f"{constants.RYU.STOP_PRODUCER_HTTP_RESOURCE} ryu_running: {ryu_running}")
         if ryu_running:
             requests.post(f"{constants.HTTP.HTTP_PROTOCOL_PREFIX}{self.ip}:{self.ryu_web_port}"
-                          f"{constants.RYU.STOP_PRODUCER_HTTP_RESOURCE}")
+                          f"{constants.RYU.STOP_PRODUCER_HTTP_RESOURCE}", timeout=constants.RYU.REQUEST_TIMEOUT_S)
         return csle_collector.ryu_manager.ryu_manager_pb2.RyuDTO(ryu_running=ryu_running, monitor_running=False,
                                                                  port=self.ryu_port,
                                                                  web_port=self.ryu_web_port,
                                                                  controller=self.controller,
                                                                  kafka_ip=self.kafka_ip,
                                                                  kafka_port=self.kafka_port,
                                                                  time_step_len=self.time_step_len)
@@ -195,15 +298,16 @@
         self.time_step_len = request.time_step_len
         monitor_running = False
         if ryu_running:
             response = requests.put(
                 f"{constants.HTTP.HTTP_PROTOCOL_PREFIX}{self.ip}:{self.ryu_web_port}"
                 f"{constants.RYU.START_PRODUCER_HTTP_RESOURCE}",
                 data=json.dumps({constants.KAFKA.BOOTSTRAP_SERVERS_PROPERTY: self.kafka_ip,
-                                 constants.RYU.TIME_STEP_LEN_SECONDS: self.time_step_len}))
+                                 constants.RYU.TIME_STEP_LEN_SECONDS: self.time_step_len}),
+                timeout=constants.RYU.REQUEST_TIMEOUT_S)
             monitor_running = response.status_code == constants.HTTP.OK_RESPONSE_CODE
         ryu_dto = csle_collector.ryu_manager.ryu_manager_pb2.RyuDTO(ryu_running=ryu_running,
                                                                     monitor_running=monitor_running,
                                                                     port=self.ryu_port,
                                                                     web_port=self.ryu_web_port,
                                                                     controller=self.controller,
                                                                     kafka_ip=self.kafka_ip,
```

### Comparing `csle_collector-0.1.9/src/csle_collector/ryu_manager/ryu_manager_pb2.py` & `csle_collector-0.2.0/src/csle_collector/ryu_manager/ryu_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py` & `csle_collector-0.2.0/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/ryu_manager/ryu_manager_util.py` & `csle_collector-0.2.0/src/csle_collector/ryu_manager/ryu_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py` & `csle_collector-0.2.0/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,25 +75,30 @@
         csle_collector.snort_ids_manager.snort_ids_manager_pb2.StopSnortIdsMsg()
     ids_monitor_dto = stub.stopSnortIds(stop_ids_msg, timeout=timeout)
     return ids_monitor_dto
 
 
 def start_snort_ids(
         stub: csle_collector.snort_ids_manager.snort_ids_manager_pb2_grpc.SnortIdsManagerStub,
-        timeout=constants.GRPC.TIMEOUT_SECONDS) \
+        ingress_interface: str, egress_interface: str, subnetmask: str, timeout=constants.GRPC.TIMEOUT_SECONDS) \
         -> csle_collector.snort_ids_manager.snort_ids_manager_pb2.SnortIdsMonitorDTO:
     """
     Sends a request to the IDS manager to start the Snort IDS
 
     :param stub: the stub to send the remote gRPC to the server
     :param timeout: the GRPC timeout (seconds)
+    :param ingress_interface: the ingress interface that Snort will listen to
+    :param egress_interface: the egress interface that Snort will listen to
+    :param subnetmask: the subnetmask that Snort will listen to
     :return: an IdsMonitorDTO describing the status of the IDS and its monitor thread
     """
     start_ids_msg = \
-        csle_collector.snort_ids_manager.snort_ids_manager_pb2.StartSnortIdsMsg()
+        csle_collector.snort_ids_manager.snort_ids_manager_pb2.StartSnortIdsMsg(
+            ingress_interface=ingress_interface, egress_interface=egress_interface, subnetmask=subnetmask
+        )
     ids_monitor_dto = stub.startSnortIds(start_ids_msg, timeout=timeout)
     return ids_monitor_dto
 
 
 def get_snort_ids_alerts(
         stub: csle_collector.snort_ids_manager.snort_ids_manager_pb2_grpc.SnortIdsManagerStub, timestamp: float,
         log_file_path: str, timeout=constants.GRPC.TIMEOUT_SECONDS) \
```

### Comparing `csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_alert.py` & `csle_collector-0.2.0/src/csle_collector/snort_ids_manager/snort_ids_alert.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,25 +4,32 @@
 
 
 class SnortIdsFastLogAlert:
     """
     DTO representing an alert entry in the fast log of Snort
     """
 
-    def __init__(self, timestamp: float, priority: int, class_id: int) -> None:
+    def __init__(self, timestamp: float, priority: int, class_id: int, source_ip: str, target_ip: str, rule_id: str) \
+            -> None:
         """
         Initializes the DTO
 
         :param timestamp: the timestamp of the record
         :param priority: the priority of the record
         :param class_id: the class id of the record
+        :param source_ip: the source ip of the record
+        :param target_ip: the target ip of the record
+        :param rule_id: the id of the Snort rule relating to the record
         """
         self.timestamp = timestamp
         self.priority = priority
         self.class_id = class_id
+        self.source_ip = source_ip
+        self.target_ip = target_ip
+        self.rule_id = rule_id
 
 
 class SnortIdsAlert:
     """
     Object representing an IDS Alert
     """
 
@@ -182,9 +189,24 @@
                 ts = str(year) + " " + ts
                 try:
                     ts = datetime.datetime.strptime(ts.strip(), '%Y %m/%d-%H:%M:%S.%f').timestamp()
                 except Exception:
                     ts = datetime.datetime.strptime("2010 04/20-08:46:14.094913", '%Y %m/%d-%H:%M:%S.%f').timestamp()
             else:
                 ts = datetime.datetime.strptime("2010 04/20-08:46:14.094913", '%Y %m/%d-%H:%M:%S.%f').timestamp()
-        fast_log_alert = SnortIdsFastLogAlert(timestamp=ts, priority=priority, class_id=alert_class_id)
+
+        source_ip = ""
+        target_ip = ""
+        ips_match = re.findall(constants.SNORT_IDS_ROUTER.IPS_REGEX, fast_log_str)
+        if len(ips_match) > 0:
+            ips = ips_match[0].replace(" ", "").split("->")
+            source_ip = ips[0]
+            target_ip = ips[1]
+
+        rule_id = ""
+        rule_match = re.findall(constants.SNORT_IDS_ROUTER.RULE_ID_REGEX, fast_log_str)
+        if len(rule_match) > 0:
+            rule_id = rule_match[0].replace("[", "").replace(":", "-")
+
+        fast_log_alert = SnortIdsFastLogAlert(timestamp=ts, priority=priority, class_id=alert_class_id,
+                                              source_ip=source_ip, target_ip=target_ip, rule_id=rule_id)
         return fast_log_alert
```

### Comparing `csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py` & `csle_collector-0.2.0/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,22 +27,22 @@
     def add(self, alert_counters: "SnortIdsAlertCounters") -> None:
         """
         Adds another alert counters object to this one
 
         :param alert_counters: the counters to add
         :return: None
         """
-        self.severe_alerts = self.severe_alerts + alert_counters.severe_alerts
-        self.warning_alerts = self.warning_alerts + alert_counters.warning_alerts
-        self.total_alerts = self.total_alerts + alert_counters.total_alerts
+        self.severe_alerts = int(self.severe_alerts + alert_counters.severe_alerts)
+        self.warning_alerts = int(self.warning_alerts + alert_counters.warning_alerts)
+        self.total_alerts = int(self.total_alerts + alert_counters.total_alerts)
         self.alerts_weighted_by_priority = self.alerts_weighted_by_priority + alert_counters.alerts_weighted_by_priority
         for idx in range(len(self.priority_alerts)):
-            self.priority_alerts[idx] = self.priority_alerts[idx] + alert_counters.priority_alerts[idx]
+            self.priority_alerts[idx] = int(self.priority_alerts[idx] + alert_counters.priority_alerts[idx])
         for idx in range(len(self.class_alerts)):
-            self.class_alerts[idx] = self.class_alerts[idx] + alert_counters.class_alerts[idx]
+            self.class_alerts[idx] = int(self.class_alerts[idx] + alert_counters.class_alerts[idx])
 
     def count(self, alerts: List[SnortIdsFastLogAlert]) -> None:
         """
         Counts the list of alerts
 
         :param alerts: list of alerts from the log
         :return: None
```

### Comparing `csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_manager.py` & `csle_collector-0.2.0/src/csle_collector/snort_ids_manager/snort_ids_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,18 +48,29 @@
         """
         Main loop of the thread. Parses the IDS log and pushes it to Kafka periodically
 
         :return: None
         """
         while self.running:
             time.sleep(self.time_step_len_seconds)
-            alert_counters = SnortIdsManagerUtil.read_snort_ids_data(self.latest_ts)
-            record = alert_counters.to_kafka_record(ip=self.ip)
-            self.producer.produce(constants.KAFKA_CONFIG.SNORT_IDS_LOG_TOPIC_NAME, record)
-            self.producer.poll(0)
+            try:
+                agg_alert_counters, rule_alert_counters, ip_alert_counters = \
+                    SnortIdsManagerUtil.read_snort_ids_data(self.latest_ts)
+                record = agg_alert_counters.to_kafka_record(ip=self.ip)
+                self.producer.produce(constants.KAFKA_CONFIG.SNORT_IDS_LOG_TOPIC_NAME, record)
+                self.producer.poll(0)
+                record = rule_alert_counters.to_kafka_record(ip=self.ip)
+                self.producer.produce(constants.KAFKA_CONFIG.SNORT_IDS_RULE_LOG_TOPIC_NAME, record)
+                self.producer.poll(0)
+                for ip_alert_counter in ip_alert_counters:
+                    record = ip_alert_counter.to_kafka_record(ip=self.ip)
+                    self.producer.produce(constants.KAFKA_CONFIG.SNORT_IDS_IP_LOG_TOPIC_NAME, record)
+                    self.producer.poll(0)
+            except Exception as e:
+                logging.info(f"There was an exception parsing the Snort logs: {str(e)}, {repr(e)}")
             self.latest_ts = time.time()
 
 
 class SnortIdsManagerServicer(csle_collector.snort_ids_manager.snort_ids_manager_pb2_grpc.SnortIdsManagerServicer):
     """
     gRPC server for collecting Snort IDS statistics.
     """
@@ -69,15 +80,15 @@
         Initializes the server
         """
         logging.basicConfig(filename=f"{constants.LOG_FILES.SNORT_IDS_MANAGER_LOG_DIR}"
                                      f"{constants.LOG_FILES.SNORT_IDS_MANAGER_LOG_FILE}", level=logging.INFO)
         self.hostname = socket.gethostname()
         try:
             self.ip = netifaces.ifaddresses(constants.INTERFACES.ETH0)[netifaces.AF_INET][0][constants.INTERFACES.ADDR]
-        except:
+        except Exception:
             self.ip = socket.gethostbyname(self.hostname)
         self.conf = {
             constants.KAFKA.BOOTSTRAP_SERVERS_PROPERTY: f"{self.ip}:{constants.KAFKA.PORT}",
             constants.KAFKA.CLIENT_ID_PROPERTY: self.hostname}
         self.ids_monitor_thread = None
         logging.info(f"Starting the SnortIDSManager hostname: {self.hostname} ip: {self.ip}")
 
@@ -103,16 +114,17 @@
         """
         Gets the statistics of the IDS log from a given timestamp
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with IDS statistics
         """
-        alert_counters = SnortIdsManagerUtil.read_snort_ids_data(request.timestamp)
-        ids_log_dto = alert_counters.to_dto(ip=self.ip)
+        agg_alert_counters, rule_alert_counters, ip_alert_counters = \
+            SnortIdsManagerUtil.read_snort_ids_data(request.timestamp)
+        ids_log_dto = agg_alert_counters.to_dto(ip=self.ip)
         return ids_log_dto
 
     def startSnortIdsMonitor(
             self, request: csle_collector.snort_ids_manager.snort_ids_manager_pb2.StartSnortIdsMonitorMsg,
             context: grpc.ServicerContext) -> csle_collector.snort_ids_manager.snort_ids_manager_pb2.SnortIdsMonitorDTO:
         """
         Starts the Snort IDS monitor thread
@@ -142,28 +154,35 @@
         """
         Starts the Snort IDS
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DTO with the status of the IDS and its monitor thread
         """
-        logging.info("Starting the SnortIDS")
+        logging.info(f"Starting the SnortIDS, ingress interface: {request.ingress_interface}, "
+                     f"egress interface: {request.egress_interface}, subnetmask: {request.subnetmask}")
         monitor_running = False
         if self.ids_monitor_thread is not None:
             monitor_running = self.ids_monitor_thread.running
         snort_running = self._is_snort_running()
         if snort_running:
-            result = subprocess.run(constants.SNORT_IDS_ROUTER.STOP_SNORT_IDS.split(" "),
+            cmd = constants.SNORT_IDS_ROUTER.STOP_SNORT_IDS
+            result = subprocess.run(cmd.split(" "),
                                     capture_output=True, text=True)
-            logging.info(f"Stopped the Snort IDS, stdout:{result.stdout}, stderr: {result.stderr}")
+            logging.info(f"Stopped the Snort IDS, stdout:{result.stdout}, stderr: {result.stderr}, cmd: {cmd}")
         if not snort_running:
-            result = subprocess.run(constants.SNORT_IDS_ROUTER.START_SNORT_IDS.split(" "),
-                                    capture_output=True, text=True)
-            logging.info(f"Started the Snort IDS, stdout:{result.stdout}, stderr: {result.stderr}")
+            cmd = constants.SNORT_IDS_ROUTER.START_SNORT_IDS.format(request.ingress_interface, request.egress_interface,
+                                                                    request.subnetmask)
+            result = subprocess.run(cmd.split(" "), capture_output=True, text=True)
+            logging.info(f"Started the Snort IDS, stdout:{result.stdout}, stderr: {result.stderr}, cmd: {cmd}")
         logging.info("Started the SnortIDS")
+        cmd = constants.SNORT_IDS_ROUTER.SNORT_LOG_DIR_PERMISSION_CMD
+        logging.info("Changing permissions of the snort log directory")
+        result = subprocess.run(cmd.split(" "), capture_output=True, text=True)
+        logging.info(f"Changed the log dir permissions, stdout:{result.stdout}, stderr: {result.stderr}, cmd: {cmd}")
         return csle_collector.snort_ids_manager.snort_ids_manager_pb2.SnortIdsMonitorDTO(
             monitor_running=monitor_running, snort_ids_running=True)
 
     def stopSnortIds(self, request: csle_collector.snort_ids_manager.snort_ids_manager_pb2.StartSnortIdsMsg,
                      context: grpc.ServicerContext) \
             -> csle_collector.snort_ids_manager.snort_ids_manager_pb2.SnortIdsMonitorDTO:
         """
```

### Comparing `csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py` & `csle_collector-0.2.0/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17snort_ids_manager.proto\"@\n\x14GetSnortIdsAlertsMsg\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x15\n\rlog_file_path\x18\x02 \x01(\t\"\x18\n\x16StopSnortIdsMonitorMsg\"u\n\x17StartSnortIdsMonitorMsg\x12\x10\n\x08kafka_ip\x18\x01 \x01(\t\x12\x12\n\nkafka_port\x18\x02 \x01(\x05\x12\x15\n\rlog_file_path\x18\x03 \x01(\t\x12\x1d\n\x15time_step_len_seconds\x18\x04 \x01(\x05\"\x11\n\x0fStopSnortIdsMsg\"\x12\n\x10StartSnortIdsMsg\"\x1d\n\x1bGetSnortIdsMonitorStatusMsg\"H\n\x12SnortIdsMonitorDTO\x12\x17\n\x0fmonitor_running\x18\x01 \x01(\x08\x12\x19\n\x11snort_ids_running\x18\x02 \x01(\x08\"\x8a\x0b\n\x0eSnortIdsLogDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\n\n\x02ip\x18\x02 \x01(\t\x12\x1e\n\x16\x61ttempted_admin_alerts\x18\x03 \x01(\x05\x12\x1d\n\x15\x61ttempted_user_alerts\x18\x04 \x01(\x05\x12$\n\x1cinappropriate_content_alerts\x18\x05 \x01(\x05\x12\x1f\n\x17policy_violation_alerts\x18\x06 \x01(\x05\x12\x1f\n\x17shellcode_detect_alerts\x18\x07 \x01(\x05\x12\x1f\n\x17successful_admin_alerts\x18\x08 \x01(\x05\x12\x1e\n\x16successful_user_alerts\x18\t \x01(\x05\x12\x1e\n\x16trojan_activity_alerts\x18\n \x01(\x05\x12 \n\x18unsuccessful_user_alerts\x18\x0b \x01(\x05\x12%\n\x1dweb_application_attack_alerts\x18\x0c \x01(\x05\x12\x1c\n\x14\x61ttempted_dos_alerts\x18\r \x01(\x05\x12\x1e\n\x16\x61ttempted_recon_alerts\x18\x0e \x01(\x05\x12\x1a\n\x12\x62\x61\x64_unknown_alerts\x18\x0f \x01(\x05\x12$\n\x1c\x64\x65\x66\x61ult_login_attempt_alerts\x18\x10 \x01(\x05\x12 \n\x18\x64\x65nial_of_service_alerts\x18\x11 \x01(\x05\x12\x1a\n\x12misc_attack_alerts\x18\x12 \x01(\x05\x12$\n\x1cnon_standard_protocol_alerts\x18\x13 \x01(\x05\x12!\n\x19rpc_portman_decode_alerts\x18\x14 \x01(\x05\x12\x1d\n\x15successful_dos_alerts\x18\x15 \x01(\x05\x12*\n\"successful_recon_largescale_alerts\x18\x16 \x01(\x05\x12\'\n\x1fsuccessful_recon_limited_alerts\x18\x17 \x01(\x05\x12)\n!suspicious_filename_detect_alerts\x18\x18 \x01(\x05\x12\x1f\n\x17suspicious_login_alerts\x18\x19 \x01(\x05\x12!\n\x19system_call_detect_alerts\x18\x1a \x01(\x05\x12-\n%unusual_client_port_connection_alerts\x18\x1b \x01(\x05\x12\'\n\x1fweb_application_activity_alerts\x18\x1c \x01(\x05\x12\x19\n\x11icmp_event_alerts\x18\x1d \x01(\x05\x12\x1c\n\x14misc_activity_alerts\x18\x1e \x01(\x05\x12\x1b\n\x13network_scan_alerts\x18\x1f \x01(\x05\x12\x1d\n\x15not_suspicious_alerts\x18  \x01(\x05\x12&\n\x1eprotocol_command_decode_alerts\x18! \x01(\x05\x12\x1c\n\x14string_detect_alerts\x18\" \x01(\x05\x12\x16\n\x0eunknown_alerts\x18# \x01(\x05\x12\x1d\n\x15tcp_connection_alerts\x18$ \x01(\x05\x12\x19\n\x11priority_1_alerts\x18% \x01(\x05\x12\x19\n\x11priority_2_alerts\x18& \x01(\x05\x12\x19\n\x11priority_3_alerts\x18\' \x01(\x05\x12\x19\n\x11priority_4_alerts\x18( \x01(\x05\x12\x14\n\x0ctotal_alerts\x18) \x01(\x05\x12\x16\n\x0ewarning_alerts\x18* \x01(\x05\x12\x15\n\rsevere_alerts\x18+ \x01(\x05\x12#\n\x1b\x61lerts_weighted_by_priority\x18, \x01(\x05\x32\xa5\x03\n\x0fSnortIdsManager\x12=\n\x11getSnortIdsAlerts\x12\x15.GetSnortIdsAlertsMsg\x1a\x0f.SnortIdsLogDTO\"\x00\x12\x45\n\x13stopSnortIdsMonitor\x12\x17.StopSnortIdsMonitorMsg\x1a\x13.SnortIdsMonitorDTO\"\x00\x12G\n\x14startSnortIdsMonitor\x12\x18.StartSnortIdsMonitorMsg\x1a\x13.SnortIdsMonitorDTO\"\x00\x12O\n\x18getSnortIdsMonitorStatus\x12\x1c.GetSnortIdsMonitorStatusMsg\x1a\x13.SnortIdsMonitorDTO\"\x00\x12\x37\n\x0cstopSnortIds\x12\x10.StopSnortIdsMsg\x1a\x13.SnortIdsMonitorDTO\"\x00\x12\x39\n\rstartSnortIds\x12\x11.StartSnortIdsMsg\x1a\x13.SnortIdsMonitorDTO\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17snort_ids_manager.proto\"@\n\x14GetSnortIdsAlertsMsg\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x15\n\rlog_file_path\x18\x02 \x01(\t\"\x18\n\x16StopSnortIdsMonitorMsg\"u\n\x17StartSnortIdsMonitorMsg\x12\x10\n\x08kafka_ip\x18\x01 \x01(\t\x12\x12\n\nkafka_port\x18\x02 \x01(\x05\x12\x15\n\rlog_file_path\x18\x03 \x01(\t\x12\x1d\n\x15time_step_len_seconds\x18\x04 \x01(\x05\"\x11\n\x0fStopSnortIdsMsg\"[\n\x10StartSnortIdsMsg\x12\x19\n\x11ingress_interface\x18\x01 \x01(\t\x12\x18\n\x10\x65gress_interface\x18\x02 \x01(\t\x12\x12\n\nsubnetmask\x18\x03 \x01(\t\"\x1d\n\x1bGetSnortIdsMonitorStatusMsg\"H\n\x12SnortIdsMonitorDTO\x12\x17\n\x0fmonitor_running\x18\x01 \x01(\x08\x12\x19\n\x11snort_ids_running\x18\x02 \x01(\x08\"\x8a\x0b\n\x0eSnortIdsLogDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\n\n\x02ip\x18\x02 \x01(\t\x12\x1e\n\x16\x61ttempted_admin_alerts\x18\x03 \x01(\x05\x12\x1d\n\x15\x61ttempted_user_alerts\x18\x04 \x01(\x05\x12$\n\x1cinappropriate_content_alerts\x18\x05 \x01(\x05\x12\x1f\n\x17policy_violation_alerts\x18\x06 \x01(\x05\x12\x1f\n\x17shellcode_detect_alerts\x18\x07 \x01(\x05\x12\x1f\n\x17successful_admin_alerts\x18\x08 \x01(\x05\x12\x1e\n\x16successful_user_alerts\x18\t \x01(\x05\x12\x1e\n\x16trojan_activity_alerts\x18\n \x01(\x05\x12 \n\x18unsuccessful_user_alerts\x18\x0b \x01(\x05\x12%\n\x1dweb_application_attack_alerts\x18\x0c \x01(\x05\x12\x1c\n\x14\x61ttempted_dos_alerts\x18\r \x01(\x05\x12\x1e\n\x16\x61ttempted_recon_alerts\x18\x0e \x01(\x05\x12\x1a\n\x12\x62\x61\x64_unknown_alerts\x18\x0f \x01(\x05\x12$\n\x1c\x64\x65\x66\x61ult_login_attempt_alerts\x18\x10 \x01(\x05\x12 \n\x18\x64\x65nial_of_service_alerts\x18\x11 \x01(\x05\x12\x1a\n\x12misc_attack_alerts\x18\x12 \x01(\x05\x12$\n\x1cnon_standard_protocol_alerts\x18\x13 \x01(\x05\x12!\n\x19rpc_portman_decode_alerts\x18\x14 \x01(\x05\x12\x1d\n\x15successful_dos_alerts\x18\x15 \x01(\x05\x12*\n\"successful_recon_largescale_alerts\x18\x16 \x01(\x05\x12\'\n\x1fsuccessful_recon_limited_alerts\x18\x17 \x01(\x05\x12)\n!suspicious_filename_detect_alerts\x18\x18 \x01(\x05\x12\x1f\n\x17suspicious_login_alerts\x18\x19 \x01(\x05\x12!\n\x19system_call_detect_alerts\x18\x1a \x01(\x05\x12-\n%unusual_client_port_connection_alerts\x18\x1b \x01(\x05\x12\'\n\x1fweb_application_activity_alerts\x18\x1c \x01(\x05\x12\x19\n\x11icmp_event_alerts\x18\x1d \x01(\x05\x12\x1c\n\x14misc_activity_alerts\x18\x1e \x01(\x05\x12\x1b\n\x13network_scan_alerts\x18\x1f \x01(\x05\x12\x1d\n\x15not_suspicious_alerts\x18  \x01(\x05\x12&\n\x1eprotocol_command_decode_alerts\x18! \x01(\x05\x12\x1c\n\x14string_detect_alerts\x18\" \x01(\x05\x12\x16\n\x0eunknown_alerts\x18# \x01(\x05\x12\x1d\n\x15tcp_connection_alerts\x18$ \x01(\x05\x12\x19\n\x11priority_1_alerts\x18% \x01(\x05\x12\x19\n\x11priority_2_alerts\x18& \x01(\x05\x12\x19\n\x11priority_3_alerts\x18\' \x01(\x05\x12\x19\n\x11priority_4_alerts\x18( \x01(\x05\x12\x14\n\x0ctotal_alerts\x18) \x01(\x05\x12\x16\n\x0ewarning_alerts\x18* \x01(\x05\x12\x15\n\rsevere_alerts\x18+ \x01(\x05\x12#\n\x1b\x61lerts_weighted_by_priority\x18, \x01(\x05\x32\xa5\x03\n\x0fSnortIdsManager\x12=\n\x11getSnortIdsAlerts\x12\x15.GetSnortIdsAlertsMsg\x1a\x0f.SnortIdsLogDTO\"\x00\x12\x45\n\x13stopSnortIdsMonitor\x12\x17.StopSnortIdsMonitorMsg\x1a\x13.SnortIdsMonitorDTO\"\x00\x12G\n\x14startSnortIdsMonitor\x12\x18.StartSnortIdsMonitorMsg\x1a\x13.SnortIdsMonitorDTO\"\x00\x12O\n\x18getSnortIdsMonitorStatus\x12\x1c.GetSnortIdsMonitorStatusMsg\x1a\x13.SnortIdsMonitorDTO\"\x00\x12\x37\n\x0cstopSnortIds\x12\x10.StopSnortIdsMsg\x1a\x13.SnortIdsMonitorDTO\"\x00\x12\x39\n\rstartSnortIds\x12\x11.StartSnortIdsMsg\x1a\x13.SnortIdsMonitorDTO\"\x00\x62\x06proto3')
 
 
 
 _GETSNORTIDSALERTSMSG = DESCRIPTOR.message_types_by_name['GetSnortIdsAlertsMsg']
 _STOPSNORTIDSMONITORMSG = DESCRIPTOR.message_types_by_name['StopSnortIdsMonitorMsg']
 _STARTSNORTIDSMONITORMSG = DESCRIPTOR.message_types_by_name['StartSnortIdsMonitorMsg']
 _STOPSNORTIDSMSG = DESCRIPTOR.message_types_by_name['StopSnortIdsMsg']
@@ -91,17 +91,17 @@
   _STOPSNORTIDSMONITORMSG._serialized_start=93
   _STOPSNORTIDSMONITORMSG._serialized_end=117
   _STARTSNORTIDSMONITORMSG._serialized_start=119
   _STARTSNORTIDSMONITORMSG._serialized_end=236
   _STOPSNORTIDSMSG._serialized_start=238
   _STOPSNORTIDSMSG._serialized_end=255
   _STARTSNORTIDSMSG._serialized_start=257
-  _STARTSNORTIDSMSG._serialized_end=275
-  _GETSNORTIDSMONITORSTATUSMSG._serialized_start=277
-  _GETSNORTIDSMONITORSTATUSMSG._serialized_end=306
-  _SNORTIDSMONITORDTO._serialized_start=308
-  _SNORTIDSMONITORDTO._serialized_end=380
-  _SNORTIDSLOGDTO._serialized_start=383
-  _SNORTIDSLOGDTO._serialized_end=1801
-  _SNORTIDSMANAGER._serialized_start=1804
-  _SNORTIDSMANAGER._serialized_end=2225
+  _STARTSNORTIDSMSG._serialized_end=348
+  _GETSNORTIDSMONITORSTATUSMSG._serialized_start=350
+  _GETSNORTIDSMONITORSTATUSMSG._serialized_end=379
+  _SNORTIDSMONITORDTO._serialized_start=381
+  _SNORTIDSMONITORDTO._serialized_end=453
+  _SNORTIDSLOGDTO._serialized_start=456
+  _SNORTIDSLOGDTO._serialized_end=1874
+  _SNORTIDSMANAGER._serialized_start=1877
+  _SNORTIDSMANAGER._serialized_end=2298
 # @@protoc_insertion_point(module_scope)
```

### Comparing `csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py` & `csle_collector-0.2.0/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py` & `csle_collector-0.2.0/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from typing import List, Dict, Any
+from typing import List, Dict, Any, Tuple
 import datetime
 import subprocess
 from csle_collector.snort_ids_manager.snort_ids_alert import SnortIdsAlert, SnortIdsFastLogAlert
 from csle_collector.snort_ids_manager.snort_ids_alert_counters import SnortIdsAlertCounters
+from csle_collector.snort_ids_manager.snort_ids_rule_counters import SnortIdsRuleCounters
+from csle_collector.snort_ids_manager.snort_ids_ip_alert_counters import SnortIdsIPAlertCounters
 import csle_collector.snort_ids_manager.snort_ids_manager_pb2
 import csle_collector.constants.constants as constants
 
 
 class SnortIdsManagerUtil:
     """
     Class with utility functions related to the Snort IDS Manager
@@ -75,15 +77,16 @@
                 return datetime.datetime.now().timestamp()
             else:
                 return alerts[0].timestamp
         else:
             return alerts[0].timestamp
 
     @staticmethod
-    def read_snort_ids_data(episode_last_alert_ts: datetime) -> SnortIdsAlertCounters:
+    def read_snort_ids_data(episode_last_alert_ts: datetime) -> Tuple[SnortIdsAlertCounters, SnortIdsRuleCounters,
+                                                                      List[SnortIdsIPAlertCounters]]:
         """
         Measures metrics from the Snort ids
 
         :param env_config: environment configuration
         :param episode_last_alert_ts: timestamp when the episode started
         :return: ids statistics
         """
@@ -92,18 +95,28 @@
         # alerts = IdsManagerUtil.check_ids_alerts()
         fast_logs = SnortIdsManagerUtil.check_snort_ids_fast_log()
 
         # Filter IDS data from beginning of episode
         # alerts = list(filter(lambda x: x.timestamp > episode_last_alert_ts, alerts))
         fast_logs = list(filter(lambda x: x.timestamp > episode_last_alert_ts, fast_logs))
 
-        counters = SnortIdsAlertCounters()
-        counters.count(fast_logs)
-
-        return counters
+        agg_counters = SnortIdsAlertCounters()
+        agg_counters.count(fast_logs)
+        rule_counters = SnortIdsRuleCounters()
+        rule_counters.count(fast_logs)
+        ip_counters = []
+        ips = set()
+        for fl in fast_logs:
+            ips.add(fl.target_ip)
+        for ip in ips:
+            ip_counter = SnortIdsIPAlertCounters()
+            ip_counter.alert_ip = ip
+            ip_counter.count(fast_logs)
+            ip_counters.append(ip_counter)
+        return agg_counters, rule_counters, ip_counters
 
     @staticmethod
     def snort_ids_monitor_dto_to_dict(
             snort_ids_monitor_dto: csle_collector.snort_ids_manager.snort_ids_manager_pb2.SnortIdsMonitorDTO) \
             -> Dict[str, Any]:
         """
         Converts a SnortIDSMonitorDTO to a dict
```

### Comparing `csle_collector-0.1.9/src/csle_collector/traffic_manager/query_traffic_manager.py` & `csle_collector-0.2.0/src/csle_collector/traffic_manager/query_traffic_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/traffic_manager/traffic_manager.py` & `csle_collector-0.2.0/src/csle_collector/traffic_manager/traffic_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         Initializes the server
         """
         logging.basicConfig(filename=f"{constants.LOG_FILES.TRAFFIC_MANAGER_LOG_DIR}"
                                      f"{constants.LOG_FILES.TRAFFIC_MANAGER_LOG_FILE}", level=logging.INFO)
         self.hostname = socket.gethostname()
         try:
             self.ip = netifaces.ifaddresses(constants.INTERFACES.ETH0)[netifaces.AF_INET][0][constants.INTERFACES.ADDR]
-        except:
+        except Exception:
             self.ip = socket.gethostbyname(self.hostname)
         logging.info(f"Setting up TrafficManager hostname: {self.hostname} ip: {self.ip}")
 
     def _get_traffic_status(self) -> bool:
         """
         Utility method to get the status of the traffic generator script
```

### Comparing `csle_collector-0.1.9/src/csle_collector/traffic_manager/traffic_manager_pb2.py` & `csle_collector-0.2.0/src/csle_collector/traffic_manager/traffic_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py` & `csle_collector-0.2.0/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector/traffic_manager/traffic_manager_util.py` & `csle_collector-0.2.0/src/csle_collector/traffic_manager/traffic_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.9/src/csle_collector.egg-info/PKG-INFO` & `csle_collector-0.2.0/src/csle_collector.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-collector
-Version: 0.1.9
+Version: 0.2.0
 Summary: Scripts for data collection in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_collector-0.1.9/src/csle_collector.egg-info/SOURCES.txt` & `csle_collector-0.2.0/src/csle_collector.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,19 @@
 src/csle_collector/ryu_manager/ryu_manager_pb2.py
 src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py
 src/csle_collector/ryu_manager/ryu_manager_util.py
 src/csle_collector/snort_ids_manager/__init__.py
 src/csle_collector/snort_ids_manager/query_snort_ids_manager.py
 src/csle_collector/snort_ids_manager/snort_ids_alert.py
 src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py
+src/csle_collector/snort_ids_manager/snort_ids_ip_alert_counters.py
 src/csle_collector/snort_ids_manager/snort_ids_manager.py
 src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py
 src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py
 src/csle_collector/snort_ids_manager/snort_ids_manager_util.py
+src/csle_collector/snort_ids_manager/snort_ids_rule_counters.py
 src/csle_collector/traffic_manager/__init__.py
 src/csle_collector/traffic_manager/query_traffic_manager.py
 src/csle_collector/traffic_manager/traffic_manager.py
 src/csle_collector/traffic_manager/traffic_manager_pb2.py
 src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py
 src/csle_collector/traffic_manager/traffic_manager_util.py
```

