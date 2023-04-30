# Comparing `tmp/gold-miner-1.1.tar.gz` & `tmp/gold-miner-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gold-miner-1.1.tar", last modified: Fri Apr 28 08:55:00 2023, max compression
+gzip compressed data, was "gold-miner-1.2.tar", last modified: Sun Apr 30 13:01:05 2023, max compression
```

## Comparing `gold-miner-1.1.tar` & `gold-miner-1.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.498841 gold-miner-1.1/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1069 2023-04-28 08:32:13.000000 gold-miner-1.1/LICENSE
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1216 2023-04-28 08:55:00.498841 gold-miner-1.1/PKG-INFO
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      810 2023-04-28 08:32:13.000000 gold-miner-1.1/README.md
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.495842 gold-miner-1.1/apropos/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/__init__.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.495842 gold-miner-1.1/apropos/goldminer/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/__init__.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.496842 gold-miner-1.1/apropos/goldminer/output/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/output/__init__.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3305 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/output/goldCurses.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1607 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/output/goldFsdb.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2100 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/output/goldHighLowWatermark.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1917 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/output/goldJson.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1252 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/output/goldOutput.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      532 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/output/goldTextDump.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      325 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/output/noop.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.496842 gold-miner-1.1/apropos/goldminer/pickaxe/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/pickaxe/__init__.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)    32568 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/pickaxe/pickaxe.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.497841 gold-miner-1.1/apropos/goldminer/reports/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/reports/__init__.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.497841 gold-miner-1.1/apropos/goldminer/tests/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/tests/__init__.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      406 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/tests/test_loads.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2118 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/tests/test_pickaxe_math.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.497841 gold-miner-1.1/apropos/goldminer/tools/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/tools/__init__.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2609 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/tools/aggregator.py
--rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)     8901 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/tools/goldminer.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     5107 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/tools/smelter.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2336 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/tools/trainer.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.498841 gold-miner-1.1/apropos/goldminer/trainer/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     7390 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/trainer/__init__.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3805 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/trainer/widthtrainer.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.498841 gold-miner-1.1/gold_miner.egg-info/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1216 2023-04-28 08:55:00.000000 gold-miner-1.1/gold_miner.egg-info/PKG-INFO
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1087 2023-04-28 08:55:00.000000 gold-miner-1.1/gold_miner.egg-info/SOURCES.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)        1 2023-04-28 08:55:00.000000 gold-miner-1.1/gold_miner.egg-info/dependency_links.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      258 2023-04-28 08:55:00.000000 gold-miner-1.1/gold_miner.egg-info/entry_points.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       29 2023-04-28 08:55:00.000000 gold-miner-1.1/gold_miner.egg-info/requires.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)        8 2023-04-28 08:55:00.000000 gold-miner-1.1/gold_miner.egg-info/top_level.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-04-28 08:55:00.498841 gold-miner-1.1/setup.cfg
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1203 2023-04-28 08:54:55.000000 gold-miner-1.1/setup.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-30 13:01:05.353773 gold-miner-1.2/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1069 2023-04-28 08:32:13.000000 gold-miner-1.2/LICENSE
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1216 2023-04-30 13:01:05.352774 gold-miner-1.2/PKG-INFO
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      810 2023-04-28 08:32:13.000000 gold-miner-1.2/README.md
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-30 13:01:05.349774 gold-miner-1.2/apropos/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/__init__.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-30 13:01:05.350773 gold-miner-1.2/apropos/goldminer/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/__init__.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-30 13:01:05.350773 gold-miner-1.2/apropos/goldminer/output/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/output/__init__.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3305 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/output/goldCurses.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1607 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/output/goldFsdb.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2100 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/output/goldHighLowWatermark.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1917 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/output/goldJson.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1252 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/output/goldOutput.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      532 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/output/goldTextDump.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      325 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/output/noop.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-30 13:01:05.351774 gold-miner-1.2/apropos/goldminer/pickaxe/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/pickaxe/__init__.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)    32625 2023-04-30 06:20:25.000000 gold-miner-1.2/apropos/goldminer/pickaxe/pickaxe.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-30 13:01:05.351774 gold-miner-1.2/apropos/goldminer/reports/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/reports/__init__.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-30 13:01:05.351774 gold-miner-1.2/apropos/goldminer/tests/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/tests/__init__.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      406 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/tests/test_loads.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2118 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/tests/test_pickaxe_math.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-30 13:01:05.351774 gold-miner-1.2/apropos/goldminer/tools/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/tools/__init__.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2609 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/tools/aggregator.py
+-rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)     8901 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/tools/goldminer.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     5111 2023-04-30 06:18:21.000000 gold-miner-1.2/apropos/goldminer/tools/smelter.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2336 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/tools/trainer.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-30 13:01:05.352774 gold-miner-1.2/apropos/goldminer/trainer/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     7401 2023-04-30 06:18:45.000000 gold-miner-1.2/apropos/goldminer/trainer/__init__.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3805 2023-04-28 08:30:54.000000 gold-miner-1.2/apropos/goldminer/trainer/widthtrainer.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-30 13:01:05.352774 gold-miner-1.2/gold_miner.egg-info/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1216 2023-04-30 13:01:04.000000 gold-miner-1.2/gold_miner.egg-info/PKG-INFO
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1087 2023-04-30 13:01:05.000000 gold-miner-1.2/gold_miner.egg-info/SOURCES.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)        1 2023-04-30 13:01:04.000000 gold-miner-1.2/gold_miner.egg-info/dependency_links.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      258 2023-04-30 13:01:05.000000 gold-miner-1.2/gold_miner.egg-info/entry_points.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       29 2023-04-30 13:01:05.000000 gold-miner-1.2/gold_miner.egg-info/requires.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)        8 2023-04-30 13:01:05.000000 gold-miner-1.2/gold_miner.egg-info/top_level.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-04-30 13:01:05.353773 gold-miner-1.2/setup.cfg
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1163 2023-04-30 13:00:25.000000 gold-miner-1.2/setup.py
```

### Comparing `gold-miner-1.1/LICENSE` & `gold-miner-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gold-miner-1.1/PKG-INFO` & `gold-miner-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gold-miner
-Version: 1.1
+Version: 1.2
 Summary: A encrypted tunnel identification research package
 Home-page: https://gitlab.com/isi-apropos/gold-miner
 Author: Wes Hardaker
 Author-email: opensource@hardakers.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `gold-miner-1.1/README.md` & `gold-miner-1.2/README.md`

 * *Files identical despite different names*

### Comparing `gold-miner-1.1/apropos/goldminer/output/goldCurses.py` & `gold-miner-1.2/apropos/goldminer/output/goldCurses.py`

 * *Files identical despite different names*

### Comparing `gold-miner-1.1/apropos/goldminer/output/goldFsdb.py` & `gold-miner-1.2/apropos/goldminer/output/goldFsdb.py`

 * *Files identical despite different names*

### Comparing `gold-miner-1.1/apropos/goldminer/output/goldHighLowWatermark.py` & `gold-miner-1.2/apropos/goldminer/output/goldHighLowWatermark.py`

 * *Files identical despite different names*

### Comparing `gold-miner-1.1/apropos/goldminer/output/goldJson.py` & `gold-miner-1.2/apropos/goldminer/output/goldJson.py`

 * *Files identical despite different names*

### Comparing `gold-miner-1.1/apropos/goldminer/output/goldOutput.py` & `gold-miner-1.2/apropos/goldminer/output/goldOutput.py`

 * *Files identical despite different names*

### Comparing `gold-miner-1.1/apropos/goldminer/output/goldTextDump.py` & `gold-miner-1.2/apropos/goldminer/output/goldTextDump.py`

 * *Files identical despite different names*

### Comparing `gold-miner-1.1/apropos/goldminer/pickaxe/pickaxe.py` & `gold-miner-1.2/apropos/goldminer/pickaxe/pickaxe.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         dig_for_gold: bool = True,
         skip_packets: int = 0,
     ) -> None:
 
         self.skip_packets = skip_packets
         pkt_count = max_packets + self.skip_packets
         info(
-            f"ANALYZING: {pcap_file} with {pkt_filter=} {max_packets=} {skip_packets=}"
+            f"ANALYZING: {pcap_file} with filter={pkt_filter} max={max_packets} skip={skip_packets}"
         )
 
         # open the pcap file
         pcap = dpkt.pcap.Reader(open(pcap_file, "rb"))
 
         # optionally set the filter
         if pkt_filter:
@@ -310,15 +310,17 @@
                     dirty_min,
                     gold_value,
                     dirty_max,
                     dirty_range_max,
                     dirty_range_min,
                 )
 
-                debug(f"{size}: {percents[size]}  ({gold_max}, {gold_min})")
+                debug(
+                    f"sz={size}: %s={percents[size]}  (max={gold_max}, min={gold_min})"
+                )
 
             # we're done build the trained results for this profile
             self.gold_mines[gold_profile] = percents
 
             debug("gold mines:")
             debug(pprint.pformat(self.gold_mines))
 
@@ -578,30 +580,30 @@
                         gold_value,
                         dirty_max,
                         dirty_range_max,
                         dirty_range_min,
                     ) = training_percents[pkt_size]
 
                     # debug(f"calculating '{mine}' distance: ")
-                    # debug(f"  {measured=}")
-                    # debug(f"  {gold_value=}")
-                    # debug(f"  {dirty_min=}")
-                    # debug(f"  {dirty_max=}")
+                    # debug(f"  {measured}")
+                    # debug(f"  {gold_value}")
+                    # debug(f"  {dirty_min}")
+                    # debug(f"  {dirty_max}")
                     difference = self.calculate_distance(
                         measured,
                         dirty_min,
                         gold_value,
                         dirty_max,
                         dirty_range_max,
                         dirty_range_min,
                     )
 
                     difference_total += difference
                     debug(
-                        f"{pkt_size}\tm={measured}, percents={training_percents[pkt_size]}\t result: {difference}"
+                        f"sz={pkt_size}\tm={measured}, percents={training_percents[pkt_size]}\t result: {difference}"
                     )
                     # debug(f"# {spi}\t{seen}\t{signal_importance}\t{deviation}")
 
                     # XXX: scale result by delta from 0 or from top other
                     # expected signal?
 
                     # msg = "  {} = seen={}, gold={}, dirt={}, rslt={}"
@@ -621,15 +623,15 @@
                         delta = self.missing_in_tunnel_penalty * (
                             len(training_percents) - len(tunnel)
                         )
                         difference_total += delta
                         number_of_sizes += delta
                     average_difference = 1 - (difference_total / number_of_sizes)
                     debug(
-                        f"diff total: {protocol_label=} {difference_total=} / {number_of_sizes=} = {average_difference=}"
+                        f"diff total: {protocol_label} {difference_total} / {number_of_sizes} = {average_difference}"
                     )
 
                     label = protocol_label
                     relabelled = label
                     if self.label_map and protocol_label in self.label_map:
                         relabelled = self.label_map[protocol_label]
 
@@ -767,15 +769,15 @@
             }
 
         if self.support_windowing:
             tunnel_size_data = self.tunnels[identifier][pkt_len]
             # spi, length, 'times' is an array of times up to its length 'length' index
             if tunnel_size_data["length"] >= tunnel_size_data["max_length"]:
                 warning(
-                    f"extending {identifier=} array size to {tunnel_size_data['max_length']*2}"
+                    f"extending {identifier} array size to {tunnel_size_data['max_length']*2}"
                 )
                 tunnel_size_data["times"] = np.hstack(
                     [
                         tunnel_size_data["times"],
                         np.empty(tunnel_size_data["max_length"]),
                     ]
                 )
@@ -854,15 +856,15 @@
                                 dirty_min,
                                 gold_value,
                                 dirty_max,
                                 dirty_range_max,
                                 dirty_range_min,
                             )
 
-                    debug(f"{windows_considered=} for {identifier=}")
+                    debug(f"{windows_considered} for {identifier}")
                     if windows_considered == 0:
                         continue
                     difference = difference / windows_considered
 
                     oh.append([mine, identifier_num, identifier, size, difference])
 
                 # for size in window_sizes:
```

### Comparing `gold-miner-1.1/apropos/goldminer/tests/test_pickaxe_math.py` & `gold-miner-1.2/apropos/goldminer/tests/test_pickaxe_math.py`

 * *Files identical despite different names*

### Comparing `gold-miner-1.1/apropos/goldminer/tools/aggregator.py` & `gold-miner-1.2/apropos/goldminer/tools/aggregator.py`

 * *Files identical despite different names*

### Comparing `gold-miner-1.1/apropos/goldminer/tools/goldminer.py` & `gold-miner-1.2/apropos/goldminer/tools/goldminer.py`

 * *Files identical despite different names*

### Comparing `gold-miner-1.1/apropos/goldminer/tools/smelter.py` & `gold-miner-1.2/apropos/goldminer/tools/smelter.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     gold_target=None,
     output_handle=sys.stdout,
     output_fsdb=False,
 ):
     for spi in spi_counts:
         tokens = list(current_values[spi].keys())
         if len(tokens) <= 1:
-            warning(f"Insufficient gold parameters identified for {timestamp=}")
+            warning(f"Insufficient gold parameters identified for time={timestamp}")
             warning(f"Only keys found: {tokens}")
             warning(f"skipping")
             return
             # exit(1)  # may be overkill for low volumes?
 
         best_value = -100000
         best_token = None
```

### Comparing `gold-miner-1.1/apropos/goldminer/tools/trainer.py` & `gold-miner-1.2/apropos/goldminer/tools/trainer.py`

 * *Files identical despite different names*

### Comparing `gold-miner-1.1/apropos/goldminer/trainer/__init__.py` & `gold-miner-1.2/apropos/goldminer/trainer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
         except Exception:
             warning(f"packet #{self.n} could not be parsed")
 
     def analyze_files(self, pcap_files: list, count: int = 0, pkt_filter: str = None):
         self.reset()
         for n, pcap_file in enumerate(pcap_files):
-            info(f"ANALYZING: {pcap_file} with {pkt_filter=} {count=}")
+            info(f"ANALYZING: {pcap_file} with filter={pkt_filter} count={count}")
 
             # open the pcap file
             pcap = dpkt.pcap.Reader(open(pcap_file, "rb"))
 
             # optionally set the filter
             if pkt_filter:
                 pcap.setfilter(pkt_filter)
```

### Comparing `gold-miner-1.1/apropos/goldminer/trainer/widthtrainer.py` & `gold-miner-1.2/apropos/goldminer/trainer/widthtrainer.py`

 * *Files identical despite different names*

### Comparing `gold-miner-1.1/gold_miner.egg-info/PKG-INFO` & `gold-miner-1.2/gold_miner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gold-miner
-Version: 1.1
+Version: 1.2
 Summary: A encrypted tunnel identification research package
 Home-page: https://gitlab.com/isi-apropos/gold-miner
 Author: Wes Hardaker
 Author-email: opensource@hardakers.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `gold-miner-1.1/gold_miner.egg-info/SOURCES.txt` & `gold-miner-1.2/gold_miner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gold-miner-1.1/setup.py` & `gold-miner-1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gold-miner",
-    version="1.1",
+    version="1.2",
     author="Wes Hardaker",
     author_email="opensource@hardakers.net",
     description="A encrypted tunnel identification research package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/isi-apropos/gold-miner",
     packages=setuptools.find_packages(),
     entry_points={
         "console_scripts": [
-            # migrating to pdb prefixes
             "gold-miner = apropos.goldminer.tools.goldminer:main",
             "gold-miner-trainer = apropos.goldminer.tools.trainer:main",
             "gold-miner-trainer-aggregator = apropos.goldminer.tools.aggregator:main",
             "gold-miner-smelter = apropos.goldminer.tools.smelter:main",
         ]
     },
     classifiers=[
```

