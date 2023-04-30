# Comparing `tmp/csle_ryu-0.1.9.tar.gz` & `tmp/csle_ryu-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_ryu-0.1.9.tar", last modified: Tue Mar 21 08:08:59 2023, max compression
+gzip compressed data, was "csle_ryu-0.2.0.tar", last modified: Sun Apr 30 12:36:01 2023, max compression
```

## Comparing `csle_ryu-0.1.9.tar` & `csle_ryu-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:08:59.841196 csle_ryu-0.1.9/
--rw-rw-r--   0 kim       (1000) kim       (1000)      639 2023-03-21 08:08:59.841196 csle_ryu-0.1.9/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     3913 2023-01-03 16:53:35.000000 csle_ryu-0.1.9/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      669 2023-02-11 20:28:41.000000 csle_ryu-0.1.9/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1244 2023-03-21 08:08:59.841196 csle_ryu-0.1.9/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2022-11-28 13:03:16.000000 csle_ryu-0.1.9/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:08:59.837195 csle_ryu-0.1.9/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:08:59.841196 csle_ryu-0.1.9/src/csle_ryu/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2022-11-28 13:03:16.000000 csle_ryu-0.1.9/src/csle_ryu/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 csle_ryu-0.1.9/src/csle_ryu/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:08:59.841196 csle_ryu-0.1.9/src/csle_ryu/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_ryu-0.1.9/src/csle_ryu/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2466 2023-03-21 07:10:46.000000 csle_ryu-0.1.9/src/csle_ryu/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:08:59.841196 csle_ryu-0.1.9/src/csle_ryu/controllers/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_ryu-0.1.9/src/csle_ryu/controllers/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8323 2022-11-28 13:03:16.000000 csle_ryu-0.1.9/src/csle_ryu/controllers/learning_switch_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11773 2022-12-11 08:32:31.000000 csle_ryu-0.1.9/src/csle_ryu/controllers/learning_switch_stp_controller.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:08:59.841196 csle_ryu-0.1.9/src/csle_ryu/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_ryu-0.1.9/src/csle_ryu/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4608 2023-02-28 07:39:18.000000 csle_ryu-0.1.9/src/csle_ryu/dao/agg_flow_statistic.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8639 2023-02-28 07:39:45.000000 csle_ryu-0.1.9/src/csle_ryu/dao/avg_flow_statistic.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    15112 2023-02-28 07:39:59.000000 csle_ryu-0.1.9/src/csle_ryu/dao/avg_port_statistic.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7034 2023-02-28 07:40:12.000000 csle_ryu-0.1.9/src/csle_ryu/dao/flow_statistic.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10610 2023-03-17 07:49:22.000000 csle_ryu-0.1.9/src/csle_ryu/dao/port_statistic.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      253 2022-11-28 13:03:16.000000 csle_ryu-0.1.9/src/csle_ryu/dao/ryu_controller_type.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:08:59.841196 csle_ryu-0.1.9/src/csle_ryu/monitor/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_ryu-0.1.9/src/csle_ryu/monitor/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    14351 2022-12-11 08:32:31.000000 csle_ryu-0.1.9/src/csle_ryu/monitor/flow_and_port_stats_monitor.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:08:59.841196 csle_ryu-0.1.9/src/csle_ryu.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      639 2023-03-21 08:08:59.000000 csle_ryu-0.1.9/src/csle_ryu.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      873 2023-03-21 08:08:59.000000 csle_ryu-0.1.9/src/csle_ryu.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:08:59.000000 csle_ryu-0.1.9/src/csle_ryu.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:28.000000 csle_ryu-0.1.9/src/csle_ryu.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      230 2023-03-21 08:08:59.000000 csle_ryu-0.1.9/src/csle_ryu.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        9 2023-03-21 08:08:59.000000 csle_ryu-0.1.9/src/csle_ryu.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:01.548368 csle_ryu-0.2.0/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      639 2023-04-30 12:36:01.548368 csle_ryu-0.2.0/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3913 2023-03-28 14:03:22.000000 csle_ryu-0.2.0/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      669 2023-03-28 14:03:22.000000 csle_ryu-0.2.0/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1244 2023-04-30 12:36:01.548368 csle_ryu-0.2.0/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_ryu-0.2.0/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:01.544368 csle_ryu-0.2.0/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:01.544368 csle_ryu-0.2.0/src/csle_ryu/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_ryu-0.2.0/src/csle_ryu/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-04-30 12:35:57.000000 csle_ryu-0.2.0/src/csle_ryu/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:01.548368 csle_ryu-0.2.0/src/csle_ryu/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.2.0/src/csle_ryu/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2484 2023-03-28 14:03:22.000000 csle_ryu-0.2.0/src/csle_ryu/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:01.548368 csle_ryu-0.2.0/src/csle_ryu/controllers/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.2.0/src/csle_ryu/controllers/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8323 2023-03-28 14:03:22.000000 csle_ryu-0.2.0/src/csle_ryu/controllers/learning_switch_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11773 2023-03-28 14:03:22.000000 csle_ryu-0.2.0/src/csle_ryu/controllers/learning_switch_stp_controller.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:01.548368 csle_ryu-0.2.0/src/csle_ryu/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.2.0/src/csle_ryu/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4598 2023-03-28 14:03:22.000000 csle_ryu-0.2.0/src/csle_ryu/dao/agg_flow_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8629 2023-03-28 14:03:22.000000 csle_ryu-0.2.0/src/csle_ryu/dao/avg_flow_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15102 2023-03-28 14:03:22.000000 csle_ryu-0.2.0/src/csle_ryu/dao/avg_port_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7004 2023-03-28 14:03:22.000000 csle_ryu-0.2.0/src/csle_ryu/dao/flow_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10600 2023-03-28 14:03:22.000000 csle_ryu-0.2.0/src/csle_ryu/dao/port_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      253 2023-03-28 14:03:22.000000 csle_ryu-0.2.0/src/csle_ryu/dao/ryu_controller_type.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:01.548368 csle_ryu-0.2.0/src/csle_ryu/monitor/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.2.0/src/csle_ryu/monitor/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14663 2023-03-28 14:03:22.000000 csle_ryu-0.2.0/src/csle_ryu/monitor/flow_and_port_stats_monitor.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:01.548368 csle_ryu-0.2.0/src/csle_ryu.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      639 2023-04-30 12:36:01.000000 csle_ryu-0.2.0/src/csle_ryu.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      873 2023-04-30 12:36:01.000000 csle_ryu-0.2.0/src/csle_ryu.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-04-30 12:36:01.000000 csle_ryu-0.2.0/src/csle_ryu.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:28.000000 csle_ryu-0.2.0/src/csle_ryu.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      230 2023-04-30 12:36:01.000000 csle_ryu-0.2.0/src/csle_ryu.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        9 2023-04-30 12:36:01.000000 csle_ryu-0.2.0/src/csle_ryu.egg-info/top_level.txt
```

### Comparing `csle_ryu-0.1.9/PKG-INFO` & `csle_ryu-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_ryu
-Version: 0.1.9
+Version: 0.2.0
 Summary: RYU SDN Controllers in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_ryu-0.1.9/README.md` & `csle_ryu-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.1.9/pyproject.toml` & `csle_ryu-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.1.9/setup.cfg` & `csle_ryu-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-collector>=0.1.9
+	csle-collector>=0.2.0
 	ryu>=4.34
 	eventlet>=0.30.2
 	confluent-kafka>=1.9.2
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
```

### Comparing `csle_ryu-0.1.9/src/csle_ryu/constants/constants.py` & `csle_ryu-0.2.0/src/csle_ryu/constants/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,25 +43,26 @@
     CONTROLLER_APP = "controller_app"
     NETWORK_ID_THIRD_OCTET = 252
     NETWORK_ID_FOURTH_OCTET = 251
     SUFFIX = "_1"
     DEFAULT_PORT = 6633
     DEFAULT_TRANSPORT_PROTOCOL = "tcp"
     SUBNETMASK_SUFFIX = "/29"
-    FULL_SUBNETMASK_SUFFIX = "/24"
+    FULL_SUBNETMASK_SUFFIX = ".0/24"
     BITMASK = "255.255.255.248"
     FULL_BITMASK = "255.255.255.0"
     STPLIB = "stplib"
     BYTE_COUNT = "byte_count"
     PACKET_COUNT = "packet_count"
     FLOW_COUNT = "flow_count"
     IN_PORT = "in_port"
     ETH_DST = "eth_dst"
     PRODUCER_RUNNING = "producer_running"
     KAFKA_CONF = "kafka_conf"
+    TIMEOUT = 5
 
 
 class CONTROLLERS:
     """
     RYU Controllers in CSLE
     """
     LEARNING_SWITCH_CONTROLLER = "learning_switch_controller"
```

### Comparing `csle_ryu-0.1.9/src/csle_ryu/controllers/learning_switch_controller.py` & `csle_ryu-0.2.0/src/csle_ryu/controllers/learning_switch_controller.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.1.9/src/csle_ryu/controllers/learning_switch_stp_controller.py` & `csle_ryu-0.2.0/src/csle_ryu/controllers/learning_switch_stp_controller.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.1.9/src/csle_ryu/dao/agg_flow_statistic.py` & `csle_ryu-0.2.0/src/csle_ryu/dao/agg_flow_statistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 class AggFlowStatistic:
     """
     DTO containing aggregated flow statistics of an OpenFlow switch
     """
 
-    def __init__(self, timestamp: float, datapath_id: int, total_num_packets: int, total_num_bytes: int,
+    def __init__(self, timestamp: float, datapath_id: str, total_num_packets: int, total_num_bytes: int,
                  total_num_flows: int):
         """
         Initializes the DTO
 
         :param timestamp: the timestamp the data was received
         :param datapath_id: the datapath ID
         :param total_num_packets: the total number of packets
@@ -104,15 +104,15 @@
         """
         Converts a kafka record to a DTO
 
         :param record: the kafka record
         :return: the DTO
         """
         parts = record.split(",")
-        obj = AggFlowStatistic(timestamp=float(parts[0]), datapath_id=int(parts[1]), total_num_packets=int(parts[2]),
+        obj = AggFlowStatistic(timestamp=float(parts[0]), datapath_id=parts[1], total_num_packets=int(parts[2]),
                                total_num_bytes=int(parts[3]), total_num_flows=int(parts[4]))
         return obj
 
     def to_kafka_record(self) -> str:
         """
         Converts the DTO into a kafka record
 
@@ -126,11 +126,11 @@
         Updates the DTO with a new kafka record
 
         :param record: the kafka record
         :return: None
         """
         parts = record.split(",")
         self.timestamp = float(parts[0])
-        self.datapath_id = int(parts[1])
+        self.datapath_id = parts[1]
         self.total_num_packets = int(parts[2])
         self.total_num_bytes = int(parts[3])
         self.total_num_flows = int(parts[4])
```

### Comparing `csle_ryu-0.1.9/src/csle_ryu/dao/avg_flow_statistic.py` & `csle_ryu-0.2.0/src/csle_ryu/dao/avg_flow_statistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class AvgFlowStatistic:
     """
     DTO containing avg data of a flow statistics returned by an OpenFlow switch
     """
 
-    def __init__(self, timestamp: float, datapath_id: int,
+    def __init__(self, timestamp: float, datapath_id: str,
                  total_num_packets: int, total_num_bytes: int, avg_duration_nanoseconds: int, avg_duration_seconds: int,
                  avg_hard_timeout: int, avg_idle_timeout: int, avg_priority: int, avg_cookie: int):
         """
         Initializes the DTO
 
         :param timestamp: the timestamp the data was received
         :param datapath_id: the datapath ID
@@ -129,15 +129,15 @@
         """
         Converts a kafka record to a DTO
 
         :param record: the kafka record
         :return: the DTO
         """
         parts = record.split(",")
-        obj = AvgFlowStatistic(timestamp=float(parts[0]), datapath_id=int(parts[1]),
+        obj = AvgFlowStatistic(timestamp=float(parts[0]), datapath_id=parts[1],
                                total_num_packets=int(parts[2]),
                                total_num_bytes=int(parts[3]), avg_duration_nanoseconds=int(parts[4]),
                                avg_duration_seconds=int(parts[5]),
                                avg_hard_timeout=int(parts[6]), avg_idle_timeout=int(parts[7]),
                                avg_priority=int(parts[8]),
                                avg_cookie=int(parts[9]))
         return obj
@@ -158,26 +158,26 @@
         Updates the DTO with a new kafka record
 
         :param record: the kafka record
         :return: None
         """
         parts = record.split(",")
         self.timestamp = float(parts[0])
-        self.datapath_id = int(parts[1])
+        self.datapath_id = parts[1]
         self.total_num_packets = int(parts[2])
         self.total_num_bytes = int(parts[3])
         self.avg_duration_nanoseconds = int(parts[4])
         self.avg_duration_seconds = int(parts[5])
         self.avg_hard_timeout = int(parts[6])
         self.avg_idle_timeout = int(parts[7])
         self.avg_priority = int(parts[8])
         self.avg_cookie = int(parts[9])
 
     @staticmethod
-    def average_flow_statistics(timestamp: float, datapath_id: int,
+    def average_flow_statistics(timestamp: float, datapath_id: str,
                                 flow_statistics: List[FlowStatistic]) -> "AvgFlowStatistic":
         """
         Computes the average metrics from a list of flow statistics
 
         :param flow_statistics: the list of flow statistics to average
         :return: the computed averages
         """
```

### Comparing `csle_ryu-0.1.9/src/csle_ryu/dao/avg_port_statistic.py` & `csle_ryu-0.2.0/src/csle_ryu/dao/avg_port_statistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class AvgPortStatistic:
     """
     DTO containing data with average port statistics from an OpenFlow switch
     """
 
-    def __init__(self, timestamp: float, datapath_id: int, total_num_received_packets: int,
+    def __init__(self, timestamp: float, datapath_id: str, total_num_received_packets: int,
                  total_num_received_bytes: int, total_num_received_errors: int, total_num_transmitted_packets: int,
                  total_num_transmitted_bytes: int, total_num_transmitted_errors: int, total_num_received_dropped: int,
                  total_num_transmitted_dropped, total_num_received_frame_errors, total_num_received_overrun_errors,
                  total_num_received_crc_errors, total_num_collisions, avg_duration_nanoseconds, avg_duration_seconds):
         """
         Initializes the DTO
 
@@ -164,15 +164,15 @@
         """
         Converts a kafka record to a DTO
 
         :param record: the kafka record
         :return: the DTO
         """
         parts = record.split(",")
-        obj = AvgPortStatistic(timestamp=float(parts[0]), datapath_id=int(parts[1]),
+        obj = AvgPortStatistic(timestamp=float(parts[0]), datapath_id=parts[1],
                                total_num_received_packets=int(parts[2]),
                                total_num_received_bytes=int(parts[3]),
                                total_num_received_errors=int(parts[4]),
                                total_num_transmitted_packets=int(parts[5]),
                                total_num_transmitted_bytes=int(parts[6]),
                                total_num_transmitted_errors=int(parts[7]),
                                total_num_received_dropped=int(parts[8]),
@@ -207,15 +207,15 @@
         Updates the DTO with a new kafka record
 
         :param record: the kafka record
         :return: None
         """
         parts = record.split(",")
         self.timestamp = float(parts[0])
-        self.datapath_id = int(parts[1])
+        self.datapath_id = parts[1]
         self.total_num_received_packets = int(parts[2])
         self.total_num_received_bytes = int(parts[3])
         self.total_num_received_errors = int(parts[4])
         self.total_num_transmitted_packets = int(parts[5])
         self.total_num_transmitted_bytes = int(parts[6])
         self.total_num_transmitted_errors = int(parts[7])
         self.total_num_received_dropped = int(parts[8])
@@ -224,15 +224,15 @@
         self.total_num_received_overrun_errors = int(parts[11])
         self.total_num_received_crc_errors = int(parts[12])
         self.total_num_collisions = int(parts[13])
         self.avg_duration_nanoseconds = int(parts[14])
         self.avg_duration_seconds = int(parts[15])
 
     @staticmethod
-    def average_port_statistics(timestamp: float, datapath_id: int,
+    def average_port_statistics(timestamp: float, datapath_id: str,
                                 port_statistics: List[PortStatistic]) -> "AvgPortStatistic":
         """
         Computes the average metrics from a list of flow statistics
 
         :param port_statistics: the list of flow statistics to average
         :return: the computed averages
         """
```

### Comparing `csle_ryu-0.1.9/src/csle_ryu/dao/flow_statistic.py` & `csle_ryu-0.2.0/src/csle_ryu/dao/flow_statistic.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 class FlowStatistic:
     """
     DTO containing data of a flow statistic returned by an OpenFlow switch
     """
 
-    def __init__(self, timestamp: float, datapath_id: int, in_port: int, out_port: int, dst_mac_address: str,
+    def __init__(self, timestamp: float, datapath_id: str, in_port: str, out_port: str, dst_mac_address: str,
                  num_packets: int, num_bytes: int, duration_nanoseconds: int, duration_seconds: int, hard_timeout: int,
                  idle_timeout: int, priority: int, cookie: int):
         """
         Initializes the DTO
 
         :param timestamp: the timestamp the data was received
         :param datapath_id: the datapath ID
@@ -133,16 +133,16 @@
         """
         Converts a kafka record to a DTO
 
         :param record: the kafka record
         :return: the DTO
         """
         parts = record.split(",")
-        obj = FlowStatistic(timestamp=float(parts[0]), datapath_id=int(parts[1]), in_port=int(parts[2]),
-                            out_port=int(parts[3]), dst_mac_address=parts[4], num_packets=int(parts[5]),
+        obj = FlowStatistic(timestamp=float(parts[0]), datapath_id=parts[1], in_port=parts[2],
+                            out_port=parts[3], dst_mac_address=parts[4], num_packets=int(parts[5]),
                             num_bytes=int(parts[6]), duration_nanoseconds=int(parts[7]),
                             duration_seconds=int(parts[8]),
                             hard_timeout=int(parts[9]), idle_timeout=int(parts[10]), priority=int(parts[11]),
                             cookie=int(parts[12]))
         return obj
 
     def to_kafka_record(self) -> str:
@@ -160,17 +160,17 @@
         Updates the DTO with a new kafka record
 
         :param record: the kafka record
         :return: None
         """
         parts = record.split(",")
         self.timestamp = float(parts[0])
-        self.datapath_id = int(parts[1])
-        self.in_port = int(parts[2])
-        self.out_port = int(parts[3])
+        self.datapath_id = parts[1]
+        self.in_port = parts[2]
+        self.out_port = parts[3]
         self.dst_mac_address = int(parts[4])
         self.num_packets = int(parts[5])
         self.num_bytes = int(parts[6])
         self.duration_nanoseconds = int(parts[7])
         self.duration_seconds = int(parts[8])
         self.hard_timeout = int(parts[9])
         self.idle_timeout = int(parts[10])
```

### Comparing `csle_ryu-0.1.9/src/csle_ryu/dao/port_statistic.py` & `csle_ryu-0.2.0/src/csle_ryu/dao/port_statistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 class PortStatistic:
     """
     DTO containing data with port statistics from an OpenFlow switch
     """
 
-    def __init__(self, timestamp: float, datapath_id: int, port: int, num_received_packets: int,
+    def __init__(self, timestamp: float, datapath_id: str, port: int, num_received_packets: int,
                  num_received_bytes: int, num_received_errors: int, num_transmitted_packets: int,
                  num_transmitted_bytes: int, num_transmitted_errors: int, num_received_dropped: int,
                  num_transmitted_dropped: int, num_received_frame_errors: int, num_received_overrun_errors: int,
                  num_received_crc_errors: int, num_collisions: int, duration_nanoseconds: int, duration_seconds: int):
         """
         Initializes the DTO
 
@@ -161,15 +161,15 @@
         """
         Converts a kafka record to a DTO
 
         :param record: the kafka record
         :return: the DTO
         """
         parts = record.split(",")
-        obj = PortStatistic(timestamp=float(parts[0]), datapath_id=int(parts[1]), port=int(parts[2]),
+        obj = PortStatistic(timestamp=float(parts[0]), datapath_id=parts[1], port=int(parts[2]),
                             num_received_packets=int(parts[3]),
                             num_received_bytes=int(parts[4]), num_received_errors=int(parts[5]),
                             num_transmitted_packets=int(parts[6]), num_transmitted_bytes=int(parts[7]),
                             num_transmitted_errors=int(parts[8]), num_received_dropped=int(parts[9]),
                             num_transmitted_dropped=int(parts[10]), num_received_frame_errors=int(parts[11]),
                             num_received_overrun_errors=int(parts[12]), num_received_crc_errors=int(parts[13]),
                             num_collisions=int(parts[14]), duration_nanoseconds=int(parts[15]),
@@ -195,15 +195,15 @@
         Updates the DTO with a new kafka record
 
         :param record: the kafka record
         :return: None
         """
         parts = record.split(",")
         self.timestamp = float(parts[0])
-        self.datapath_id = int(parts[1])
+        self.datapath_id = parts[1]
         self.port = int(parts[2])
         self.num_received_packets = int(parts[3])
         self.num_received_bytes = int(parts[4])
         self.num_received_errors = int(parts[5])
         self.num_transmitted_packets = int(parts[6])
         self.num_transmitted_bytes = int(parts[7])
         self.num_transmitted_errors = int(parts[8])
```

### Comparing `csle_ryu-0.1.9/src/csle_ryu/monitor/flow_and_port_stats_monitor.py` & `csle_ryu-0.2.0/src/csle_ryu/monitor/flow_and_port_stats_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,26 +92,30 @@
 
         :return: None
         """
         while True:
             if self.producer_running:
                 for dp in self.datapaths.values():
                     self._request_stats(dp)
-                    response = requests.get(f"{collector_constants.HTTP.HTTP_PROTOCOL_PREFIX}"
-                                            f"{collector_constants.HTTP.LOCALHOST}:8080"
-                                            f"{constants.RYU.STATS_AGGREGATE_FLOW_RESOURCE}/{dp.id}")
-                    aggflows = json.loads(response.content)[str(dp.id)][0]
-                    agg_flow_stat = AggFlowStatistic(timestamp=time.time(), datapath_id=dp.id,
-                                                     total_num_bytes=aggflows[constants.RYU.BYTE_COUNT],
-                                                     total_num_packets=aggflows[constants.RYU.PACKET_COUNT],
-                                                     total_num_flows=aggflows[constants.RYU.FLOW_COUNT])
-                    if self.producer_running:
-                        self.producer.produce(collector_constants.KAFKA_CONFIG.OPENFLOW_AGG_FLOW_STATS_TOPIC_NAME,
-                                              agg_flow_stat.to_kafka_record())
-                        self.producer.poll(0)
+                    try:
+                        response = requests.get(f"{collector_constants.HTTP.HTTP_PROTOCOL_PREFIX}"
+                                                f"{collector_constants.HTTP.LOCALHOST}:8080"
+                                                f"{constants.RYU.STATS_AGGREGATE_FLOW_RESOURCE}/{dp.id}",
+                                                timeout=constants.RYU.TIMEOUT)
+                        aggflows = json.loads(response.content)[str(dp.id)][0]
+                        agg_flow_stat = AggFlowStatistic(timestamp=time.time(), datapath_id=dp.id,
+                                                         total_num_bytes=aggflows[constants.RYU.BYTE_COUNT],
+                                                         total_num_packets=aggflows[constants.RYU.PACKET_COUNT],
+                                                         total_num_flows=aggflows[constants.RYU.FLOW_COUNT])
+                        if self.producer_running:
+                            self.producer.produce(collector_constants.KAFKA_CONFIG.OPENFLOW_AGG_FLOW_STATS_TOPIC_NAME,
+                                                  agg_flow_stat.to_kafka_record())
+                            self.producer.poll(0)
+                    except Exception as e:
+                        self.logger.warning(f"There was an error parsing the flow statistics: {str(e)}, {repr(e)}")
             hub.sleep(self.time_step_len_seconds)
 
     def _request_stats(self, datapath) -> None:
         """
         Utility function for sending a request to a switch with a qiven datapath to return its flow and port statistics.
 
         :param datapath: the datapath, i.e. abstraction of the link to the switch
@@ -261,15 +265,15 @@
         :param req: the REST API request
         :param kwargs: WSGI arguments
         :return: the REST API response
         """
         try:
             kafka_conf = req.json if req.body else {}
         except ValueError:
-            raise Response(status=collector_constants.HTTP.BAD_REQUEST_RESPONSE_CODE)
+            return Response(status=collector_constants.HTTP.BAD_REQUEST_RESPONSE_CODE)
         if collector_constants.KAFKA.BOOTSTRAP_SERVERS_PROPERTY in kafka_conf \
                 and collector_constants.RYU.TIME_STEP_LEN_SECONDS in kafka_conf:
             self.controller_app.kafka_conf = {
                 collector_constants.KAFKA.BOOTSTRAP_SERVERS_PROPERTY: kafka_conf[
                     collector_constants.KAFKA.BOOTSTRAP_SERVERS_PROPERTY],
                 collector_constants.KAFKA.CLIENT_ID_PROPERTY: self.hostname}
             self.controller_app.logger.info(f"Starting Kafka producer with conf: {self.controller_app.kafka_conf}")
```

### Comparing `csle_ryu-0.1.9/src/csle_ryu.egg-info/PKG-INFO` & `csle_ryu-0.2.0/src/csle_ryu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-ryu
-Version: 0.1.9
+Version: 0.2.0
 Summary: RYU SDN Controllers in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_ryu-0.1.9/src/csle_ryu.egg-info/SOURCES.txt` & `csle_ryu-0.2.0/src/csle_ryu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

