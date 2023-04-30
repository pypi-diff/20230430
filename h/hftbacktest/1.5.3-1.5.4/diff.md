# Comparing `tmp/hftbacktest-1.5.3.tar.gz` & `tmp/hftbacktest-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hftbacktest-1.5.3.tar", last modified: Fri Apr 28 14:15:39 2023, max compression
+gzip compressed data, was "hftbacktest-1.5.4.tar", last modified: Sun Apr 30 14:11:12 2023, max compression
```

## Comparing `hftbacktest-1.5.3.tar` & `hftbacktest-1.5.4.tar`

### file list

```diff
@@ -1,41 +1,51 @@
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-28 14:15:39.345537 hftbacktest-1.5.3/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1079 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/LICENSE
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6895 2023-04-28 14:15:39.345537 hftbacktest-1.5.3/PKG-INFO
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5786 2023-04-28 14:13:16.000000 hftbacktest-1.5.3/README.rst
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-28 14:15:39.344537 hftbacktest-1.5.3/hftbacktest/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11501 2023-04-28 13:24:01.000000 hftbacktest-1.5.3/hftbacktest/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1011 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/assettype.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    14547 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/backtest.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-28 14:15:39.344537 hftbacktest-1.5.3/hftbacktest/data/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1592 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/data/__init__.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-28 14:15:39.344537 hftbacktest-1.5.3/hftbacktest/data/utils/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       44 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/data/utils/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11484 2023-04-28 13:21:33.000000 hftbacktest-1.5.3/hftbacktest/data/utils/binancefutures.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2160 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/data/utils/snapshot.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6901 2023-04-28 13:18:47.000000 hftbacktest-1.5.3/hftbacktest/data/utils/tardis.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11553 2023-04-28 12:19:24.000000 hftbacktest-1.5.3/hftbacktest/data/validation.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6194 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/marketdepth.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-28 14:15:39.344537 hftbacktest-1.5.3/hftbacktest/models/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/models/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10007 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/models/latencies.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3305 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/models/queue.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4143 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/order.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-28 14:15:39.345537 hftbacktest-1.5.3/hftbacktest/proc/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/proc/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5866 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/proc/local.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    14794 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/proc/nopartialfillexchange.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    22145 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/proc/partialfillexchange.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5903 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/proc/proc.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3252 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/reader.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    13631 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/stat.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2149 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/state.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      876 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/typing.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-28 14:15:39.344537 hftbacktest-1.5.3/hftbacktest.egg-info/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6895 2023-04-28 14:15:39.000000 hftbacktest-1.5.3/hftbacktest.egg-info/PKG-INFO
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      908 2023-04-28 14:15:39.000000 hftbacktest-1.5.3/hftbacktest.egg-info/SOURCES.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.5.3/hftbacktest.egg-info/dependency_links.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.5.3/hftbacktest.egg-info/not-zip-safe
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       48 2023-04-28 14:15:39.000000 hftbacktest-1.5.3/hftbacktest.egg-info/requires.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       12 2023-04-28 14:15:39.000000 hftbacktest-1.5.3/hftbacktest.egg-info/top_level.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1249 2023-04-28 14:15:39.345537 hftbacktest-1.5.3/setup.cfg
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       61 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/setup.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-30 14:11:12.330382 hftbacktest-1.5.4/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1079 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/LICENSE
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6815 2023-04-30 14:11:12.330382 hftbacktest-1.5.4/PKG-INFO
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5706 2023-04-30 12:46:55.000000 hftbacktest-1.5.4/README.rst
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-30 14:11:12.329382 hftbacktest-1.5.4/hftbacktest/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11501 2023-04-30 14:07:40.000000 hftbacktest-1.5.4/hftbacktest/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1011 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/assettype.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    14547 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/backtest.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-30 14:11:12.329382 hftbacktest-1.5.4/hftbacktest/data/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1592 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/data/__init__.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-30 14:11:12.330382 hftbacktest-1.5.4/hftbacktest/data/utils/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       44 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/data/utils/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11484 2023-04-28 13:21:33.000000 hftbacktest-1.5.4/hftbacktest/data/utils/binancefutures.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2160 2023-04-30 14:00:09.000000 hftbacktest-1.5.4/hftbacktest/data/utils/snapshot.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6901 2023-04-28 13:18:47.000000 hftbacktest-1.5.4/hftbacktest/data/utils/tardis.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11553 2023-04-28 12:19:24.000000 hftbacktest-1.5.4/hftbacktest/data/validation.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-30 14:11:12.330382 hftbacktest-1.5.4/hftbacktest/experimental/
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.5.4/hftbacktest/experimental/__init__.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    14453 2023-04-29 10:30:43.000000 hftbacktest-1.5.4/hftbacktest/experimental/backtest.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-30 14:11:12.330382 hftbacktest-1.5.4/hftbacktest/experimental/live/
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.5.4/hftbacktest/experimental/live/__init__.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    19630 2023-04-29 10:30:43.000000 hftbacktest-1.5.4/hftbacktest/experimental/live/binancefutures.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)      333 2023-04-29 10:30:43.000000 hftbacktest-1.5.4/hftbacktest/experimental/live/custom_strategy.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     7792 2023-04-29 10:30:43.000000 hftbacktest-1.5.4/hftbacktest/experimental/live/ordermanager.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     3578 2023-04-29 10:30:43.000000 hftbacktest-1.5.4/hftbacktest/experimental/live/settings.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     6821 2023-04-29 10:30:43.000000 hftbacktest-1.5.4/hftbacktest/experimental/multiassetinit.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6194 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/marketdepth.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-30 14:11:12.330382 hftbacktest-1.5.4/hftbacktest/models/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/models/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10010 2023-04-29 14:47:02.000000 hftbacktest-1.5.4/hftbacktest/models/latencies.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3305 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/models/queue.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4143 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/order.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-30 14:11:12.330382 hftbacktest-1.5.4/hftbacktest/proc/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/proc/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5866 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/proc/local.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    14794 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/proc/nopartialfillexchange.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    22145 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/proc/partialfillexchange.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5903 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/proc/proc.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3252 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/reader.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    13631 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/stat.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2149 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/state.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      876 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/typing.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-30 14:11:12.329382 hftbacktest-1.5.4/hftbacktest.egg-info/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6815 2023-04-30 14:11:12.000000 hftbacktest-1.5.4/hftbacktest.egg-info/PKG-INFO
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1252 2023-04-30 14:11:12.000000 hftbacktest-1.5.4/hftbacktest.egg-info/SOURCES.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-30 14:11:12.000000 hftbacktest-1.5.4/hftbacktest.egg-info/dependency_links.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.5.4/hftbacktest.egg-info/not-zip-safe
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       48 2023-04-30 14:11:12.000000 hftbacktest-1.5.4/hftbacktest.egg-info/requires.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       12 2023-04-30 14:11:12.000000 hftbacktest-1.5.4/hftbacktest.egg-info/top_level.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1249 2023-04-30 14:11:12.331382 hftbacktest-1.5.4/setup.cfg
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       61 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/setup.py
```

### Comparing `hftbacktest-1.5.3/LICENSE` & `hftbacktest-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/PKG-INFO` & `hftbacktest-1.5.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.5.3
+Version: 1.5.4
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
@@ -84,19 +84,16 @@
         max_position = 5
         half_spread = hbt.tick_size * 20
         skew = 1
         order_qty = 0.1 
         last_order_id = -1
         order_id = 0
 
-        while hbt.run:
-            # Checks every 0.1s
-            if not hbt.elapse(0.1 * 1e6):
-                return False
-
+        # Checks every 0.1s
+        while hbt.elapse(100_000):
             # Clears cancelled, filled or expired orders.
             hbt.clear_inactive_orders()
 
             # Obtains the current mid-price and computes the reservation price.
             mid_price = (hbt.best_bid + hbt.best_ask) / 2.0
             reservation_price = mid_price - skew * hbt.position * hbt.tick_size
 
@@ -114,15 +111,15 @@
             # Waits until one of the order cancellation responses is received.
             if last_order_id >= 0:
                 hbt.wait_order_response(last_order_id)
 				
             # Clears cancelled, filled or expired orders.
             hbt.clear_inactive_orders()
 
-	    last_order_id = -1
+	        last_order_id = -1
             if hbt.position < max_position:
                 # Submits a new post-only limit bid order.
                 order_id += 1
                 hbt.submit_buy_order(
                     order_id,
                     buy_order_price,
                     order_qty,
@@ -144,15 +141,14 @@
             # All order requests are considered to be requested at the same time.
             # Waits until one of the order responses is received.
             if last_order_id >= 0:
                 hbt.wait_order_response(last_order_id)
 
             # Records the current state for stat calculation.
             stat.record(hbt)
-        return True
 
     
 Examples
 ========
 
 You can find more examples in `examples <https://github.com/nkaz001/hftbacktest/tree/master/examples>`_ directory.
```

### Comparing `hftbacktest-1.5.3/README.rst` & `hftbacktest-1.5.4/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -58,19 +58,16 @@
         max_position = 5
         half_spread = hbt.tick_size * 20
         skew = 1
         order_qty = 0.1 
         last_order_id = -1
         order_id = 0
 
-        while hbt.run:
-            # Checks every 0.1s
-            if not hbt.elapse(0.1 * 1e6):
-                return False
-
+        # Checks every 0.1s
+        while hbt.elapse(100_000):
             # Clears cancelled, filled or expired orders.
             hbt.clear_inactive_orders()
 
             # Obtains the current mid-price and computes the reservation price.
             mid_price = (hbt.best_bid + hbt.best_ask) / 2.0
             reservation_price = mid_price - skew * hbt.position * hbt.tick_size
 
@@ -88,15 +85,15 @@
             # Waits until one of the order cancellation responses is received.
             if last_order_id >= 0:
                 hbt.wait_order_response(last_order_id)
 				
             # Clears cancelled, filled or expired orders.
             hbt.clear_inactive_orders()
 
-	    last_order_id = -1
+	        last_order_id = -1
             if hbt.position < max_position:
                 # Submits a new post-only limit bid order.
                 order_id += 1
                 hbt.submit_buy_order(
                     order_id,
                     buy_order_price,
                     order_qty,
@@ -118,15 +115,14 @@
             # All order requests are considered to be requested at the same time.
             # Waits until one of the order responses is received.
             if last_order_id >= 0:
                 hbt.wait_order_response(last_order_id)
 
             # Records the current state for stat calculation.
             stat.record(hbt)
-        return True
 
     
 Examples
 ========
 
 You can find more examples in `examples <https://github.com/nkaz001/hftbacktest/tree/master/examples>`_ directory.
```

### Comparing `hftbacktest-1.5.3/hftbacktest/__init__.py` & `hftbacktest-1.5.4/hftbacktest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     'validate_data',
     'correct_local_timestamp',
     'correct_exch_timestamp',
     'correct_exch_timestamp_adjust',
     'correct'
 )
 
-__version__ = '1.5.3'
+__version__ = '1.5.4'
 
 
 # JIT'ed latency models
 ConstantLatency = jitclass()(ConstantLatency_)
 FeedLatency = jitclass()(FeedLatency_)
 ForwardFeedLatency = jitclass()(ForwardFeedLatency_)
 BackwardFeedLatency = jitclass()(BackwardFeedLatency_)
```

### Comparing `hftbacktest-1.5.3/hftbacktest/assettype.py` & `hftbacktest-1.5.4/hftbacktest/assettype.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/hftbacktest/backtest.py` & `hftbacktest-1.5.4/hftbacktest/backtest.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/hftbacktest/data/__init__.py` & `hftbacktest-1.5.4/hftbacktest/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/hftbacktest/data/utils/binancefutures.py` & `hftbacktest-1.5.4/hftbacktest/data/utils/binancefutures.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/hftbacktest/data/utils/snapshot.py` & `hftbacktest-1.5.4/hftbacktest/data/utils/snapshot.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/hftbacktest/data/utils/tardis.py` & `hftbacktest-1.5.4/hftbacktest/data/utils/tardis.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/hftbacktest/data/validation.py` & `hftbacktest-1.5.4/hftbacktest/data/validation.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/hftbacktest/marketdepth.py` & `hftbacktest-1.5.4/hftbacktest/marketdepth.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/hftbacktest/models/latencies.py` & `hftbacktest-1.5.4/hftbacktest/models/latencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
     Args:
         data (array): An (n, 3) array consisting of three columns: local timestamp when the request was made, exchange
             timestamp, and local timestamp when the response was received.
     """
 
     entry_rn: int64
     resp_rn: int64
-    data: float64[:]
+    data: float64[:, :]
     
     def __init__(self, data):
         self.entry_rn = 0
         self.resp_rn = 0
         self.data = data
 
     def __intp(self, x, x1, y1, x2, y2):
```

### Comparing `hftbacktest-1.5.3/hftbacktest/models/queue.py` & `hftbacktest-1.5.4/hftbacktest/models/queue.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/hftbacktest/order.py` & `hftbacktest-1.5.4/hftbacktest/order.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/hftbacktest/proc/local.py` & `hftbacktest-1.5.4/hftbacktest/proc/local.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/hftbacktest/proc/nopartialfillexchange.py` & `hftbacktest-1.5.4/hftbacktest/proc/nopartialfillexchange.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/hftbacktest/proc/partialfillexchange.py` & `hftbacktest-1.5.4/hftbacktest/proc/partialfillexchange.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/hftbacktest/proc/proc.py` & `hftbacktest-1.5.4/hftbacktest/proc/proc.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/hftbacktest/reader.py` & `hftbacktest-1.5.4/hftbacktest/reader.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/hftbacktest/stat.py` & `hftbacktest-1.5.4/hftbacktest/stat.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/hftbacktest/state.py` & `hftbacktest-1.5.4/hftbacktest/state.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/hftbacktest/typing.py` & `hftbacktest-1.5.4/hftbacktest/typing.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.3/hftbacktest.egg-info/PKG-INFO` & `hftbacktest-1.5.4/hftbacktest.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.5.3
+Version: 1.5.4
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
@@ -84,19 +84,16 @@
         max_position = 5
         half_spread = hbt.tick_size * 20
         skew = 1
         order_qty = 0.1 
         last_order_id = -1
         order_id = 0
 
-        while hbt.run:
-            # Checks every 0.1s
-            if not hbt.elapse(0.1 * 1e6):
-                return False
-
+        # Checks every 0.1s
+        while hbt.elapse(100_000):
             # Clears cancelled, filled or expired orders.
             hbt.clear_inactive_orders()
 
             # Obtains the current mid-price and computes the reservation price.
             mid_price = (hbt.best_bid + hbt.best_ask) / 2.0
             reservation_price = mid_price - skew * hbt.position * hbt.tick_size
 
@@ -114,15 +111,15 @@
             # Waits until one of the order cancellation responses is received.
             if last_order_id >= 0:
                 hbt.wait_order_response(last_order_id)
 				
             # Clears cancelled, filled or expired orders.
             hbt.clear_inactive_orders()
 
-	    last_order_id = -1
+	        last_order_id = -1
             if hbt.position < max_position:
                 # Submits a new post-only limit bid order.
                 order_id += 1
                 hbt.submit_buy_order(
                     order_id,
                     buy_order_price,
                     order_qty,
@@ -144,15 +141,14 @@
             # All order requests are considered to be requested at the same time.
             # Waits until one of the order responses is received.
             if last_order_id >= 0:
                 hbt.wait_order_response(last_order_id)
 
             # Records the current state for stat calculation.
             stat.record(hbt)
-        return True
 
     
 Examples
 ========
 
 You can find more examples in `examples <https://github.com/nkaz001/hftbacktest/tree/master/examples>`_ directory.
```

### Comparing `hftbacktest-1.5.3/hftbacktest.egg-info/SOURCES.txt` & `hftbacktest-1.5.4/hftbacktest.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,22 @@
 hftbacktest.egg-info/top_level.txt
 hftbacktest/data/__init__.py
 hftbacktest/data/validation.py
 hftbacktest/data/utils/__init__.py
 hftbacktest/data/utils/binancefutures.py
 hftbacktest/data/utils/snapshot.py
 hftbacktest/data/utils/tardis.py
+hftbacktest/experimental/__init__.py
+hftbacktest/experimental/backtest.py
+hftbacktest/experimental/multiassetinit.py
+hftbacktest/experimental/live/__init__.py
+hftbacktest/experimental/live/binancefutures.py
+hftbacktest/experimental/live/custom_strategy.py
+hftbacktest/experimental/live/ordermanager.py
+hftbacktest/experimental/live/settings.py
 hftbacktest/models/__init__.py
 hftbacktest/models/latencies.py
 hftbacktest/models/queue.py
 hftbacktest/proc/__init__.py
 hftbacktest/proc/local.py
 hftbacktest/proc/nopartialfillexchange.py
 hftbacktest/proc/partialfillexchange.py
```

### Comparing `hftbacktest-1.5.3/setup.cfg` & `hftbacktest-1.5.4/setup.cfg`

 * *Files identical despite different names*

