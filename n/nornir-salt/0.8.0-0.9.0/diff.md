# Comparing `tmp/nornir_salt-0.8.0.tar.gz` & `tmp/nornir_salt-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nornir_salt-0.8.0.tar", last modified: Tue Dec 21 01:48:08 2021, max compression
+gzip compressed data, was "dist\nornir_salt-0.9.0.tar", last modified: Sun Feb 13 05:06:06 2022, max compression
```

## Comparing `nornir_salt-0.8.0.tar` & `nornir_salt-0.9.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2021-12-21 01:48:08.000000 nornir_salt-0.8.0/
--rw-rw-rw-   0        0        0     1444 2021-12-21 01:48:08.000000 nornir_salt-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0      742 2021-12-21 01:31:19.000000 nornir_salt-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2021-12-21 01:48:07.000000 nornir_salt-0.8.0/nornir_salt/
--rw-rw-rw-   0        0        0     3413 2021-12-20 12:41:23.000000 nornir_salt-0.8.0/nornir_salt/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-21 01:48:08.000000 nornir_salt-0.8.0/nornir_salt/plugins/
--rw-rw-rw-   0        0        0        0 2021-12-20 12:45:47.000000 nornir_salt-0.8.0/nornir_salt/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-21 01:48:08.000000 nornir_salt-0.8.0/nornir_salt/plugins/connections/
--rw-rw-rw-   0        0        0     4409 2021-12-20 12:42:22.000000 nornir_salt-0.8.0/nornir_salt/plugins/connections/ConnectionsPool.py
--rw-rw-rw-   0        0        0     2641 2021-12-20 12:42:29.000000 nornir_salt-0.8.0/nornir_salt/plugins/connections/HTTPPlugin.py
--rw-rw-rw-   0        0        0     2005 2021-12-20 12:42:33.000000 nornir_salt-0.8.0/nornir_salt/plugins/connections/NcclientPlugin.py
--rw-rw-rw-   0        0        0     7196 2021-12-20 12:42:13.000000 nornir_salt-0.8.0/nornir_salt/plugins/connections/PyATSUnicon.py
--rw-rw-rw-   0        0        0     2056 2021-12-20 12:42:17.000000 nornir_salt-0.8.0/nornir_salt/plugins/connections/PyGNMIPlugin.py
--rw-rw-rw-   0        0        0      316 2021-12-20 12:42:19.000000 nornir_salt-0.8.0/nornir_salt/plugins/connections/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-21 01:48:08.000000 nornir_salt-0.8.0/nornir_salt/plugins/functions/
--rw-rw-rw-   0        0        0     5841 2021-12-20 12:43:12.000000 nornir_salt-0.8.0/nornir_salt/plugins/functions/DumpResults.py
--rw-rw-rw-   0        0        0    12155 2021-12-20 12:43:15.000000 nornir_salt-0.8.0/nornir_salt/plugins/functions/FFun.py
--rw-rw-rw-   0        0        0     4520 2021-12-20 12:43:18.000000 nornir_salt-0.8.0/nornir_salt/plugins/functions/HostsKeepalive.py
--rw-rw-rw-   0        0        0    11343 2021-12-21 01:20:42.000000 nornir_salt-0.8.0/nornir_salt/plugins/functions/InventoryFun.py
--rw-rw-rw-   0        0        0     9941 2021-12-21 01:20:42.000000 nornir_salt-0.8.0/nornir_salt/plugins/functions/ResultSerializer.py
--rw-rw-rw-   0        0        0     6357 2021-12-21 01:20:37.000000 nornir_salt-0.8.0/nornir_salt/plugins/functions/TabulateFormatter.py
--rw-rw-rw-   0        0        0      375 2021-12-20 12:43:07.000000 nornir_salt-0.8.0/nornir_salt/plugins/functions/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-21 01:48:08.000000 nornir_salt-0.8.0/nornir_salt/plugins/inventory/
--rw-rw-rw-   0        0        0     3921 2021-12-20 12:43:37.000000 nornir_salt-0.8.0/nornir_salt/plugins/inventory/DictInventory.py
--rw-rw-rw-   0        0        0       82 2021-12-20 12:43:41.000000 nornir_salt-0.8.0/nornir_salt/plugins/inventory/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-21 01:48:08.000000 nornir_salt-0.8.0/nornir_salt/plugins/processors/
--rw-rw-rw-   0        0        0    58187 2021-12-21 01:20:44.000000 nornir_salt-0.8.0/nornir_salt/plugins/processors/DataProcessor.py
--rw-rw-rw-   0        0        0     8034 2021-12-20 12:44:05.000000 nornir_salt-0.8.0/nornir_salt/plugins/processors/DiffProcessor.py
--rw-rw-rw-   0        0        0     1385 2021-12-21 01:20:42.000000 nornir_salt-0.8.0/nornir_salt/plugins/processors/N2GProcessor.py
--rw-rw-rw-   0        0        0     6600 2021-12-20 12:44:12.000000 nornir_salt-0.8.0/nornir_salt/plugins/processors/SaltEventProcessor.py
--rw-rw-rw-   0        0        0    38544 2021-12-21 01:20:37.000000 nornir_salt-0.8.0/nornir_salt/plugins/processors/TestsProcessor.py
--rw-rw-rw-   0        0        0     7680 2021-12-20 12:43:57.000000 nornir_salt-0.8.0/nornir_salt/plugins/processors/ToFileProcessor.py
--rw-rw-rw-   0        0        0      349 2021-12-20 12:43:59.000000 nornir_salt-0.8.0/nornir_salt/plugins/processors/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-21 01:48:08.000000 nornir_salt-0.8.0/nornir_salt/plugins/runners/
--rw-rw-rw-   0        0        0     2995 2021-12-20 12:41:49.000000 nornir_salt-0.8.0/nornir_salt/plugins/runners/QueueRunner.py
--rw-rw-rw-   0        0        0    19580 2021-12-20 12:41:52.000000 nornir_salt-0.8.0/nornir_salt/plugins/runners/RetryRunner.py
--rw-rw-rw-   0        0        0      116 2021-12-20 12:41:55.000000 nornir_salt-0.8.0/nornir_salt/plugins/runners/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-21 01:48:08.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/
--rw-rw-rw-   0        0        0     1596 2021-12-20 12:44:41.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/__init__.py
--rw-rw-rw-   0        0        0     2155 2021-12-20 12:44:48.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/connections.py
--rw-rw-rw-   0        0        0    15422 2021-12-21 01:20:37.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/files.py
--rw-rw-rw-   0        0        0     7725 2021-12-20 12:44:55.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/http_call.py
--rw-rw-rw-   0        0        0     2743 2021-12-20 12:44:58.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/napalm_configure.py
--rw-rw-rw-   0        0        0     5211 2021-12-21 01:20:37.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/napalm_send_commands.py
--rw-rw-rw-   0        0        0    10870 2021-12-21 01:20:44.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/ncclient_call.py
--rw-rw-rw-   0        0        0     7977 2021-12-20 12:45:06.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/netmiko_send_command_ps.py
--rw-rw-rw-   0        0        0     5161 2021-12-21 01:20:37.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/netmiko_send_commands.py
--rw-rw-rw-   0        0        0     6242 2021-12-20 12:45:12.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/netmiko_send_config.py
--rw-rw-rw-   0        0        0     2084 2021-12-21 01:20:37.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/nr_test.py
--rw-rw-rw-   0        0        0     1744 2021-12-21 01:20:37.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/pyats_genie_api.py
--rw-rw-rw-   0        0        0    10276 2021-12-21 01:20:37.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/pyats_send_commands.py
--rw-rw-rw-   0        0        0     4605 2021-12-20 12:45:22.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/pyats_send_config.py
--rw-rw-rw-   0        0        0     9589 2021-12-20 12:45:24.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/pygnmi_call.py
--rw-rw-rw-   0        0        0     1313 2021-12-20 12:45:28.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/salt_cfg_gen.py
--rw-rw-rw-   0        0        0     2282 2021-12-20 12:45:30.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/salt_clear_hcache.py
--rw-rw-rw-   0        0        0     8196 2021-12-21 01:20:44.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/scrapli_netconf_call.py
--rw-rw-rw-   0        0        0     4425 2021-12-21 01:20:37.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/scrapli_send_commands.py
--rw-rw-rw-   0        0        0     2852 2021-12-20 12:45:38.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/scrapli_send_config.py
--rw-rw-rw-   0        0        0      698 2021-12-20 12:44:34.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/sleep.py
--rw-rw-rw-   0        0        0     2376 2021-12-21 01:20:37.000000 nornir_salt-0.8.0/nornir_salt/plugins/tasks/tcp_ping.py
-drwxrwxrwx   0        0        0        0 2021-12-21 01:48:08.000000 nornir_salt-0.8.0/nornir_salt.egg-info/
--rw-rw-rw-   0        0        0     1444 2021-12-21 01:48:06.000000 nornir_salt-0.8.0/nornir_salt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2421 2021-12-21 01:48:07.000000 nornir_salt-0.8.0/nornir_salt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-21 01:48:07.000000 nornir_salt-0.8.0/nornir_salt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      414 2021-12-21 01:48:07.000000 nornir_salt-0.8.0/nornir_salt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2021-12-21 01:48:07.000000 nornir_salt-0.8.0/nornir_salt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2021-12-21 01:48:07.000000 nornir_salt-0.8.0/nornir_salt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-12-21 01:48:08.000000 nornir_salt-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1267 2021-12-21 01:23:58.000000 nornir_salt-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-02-13 05:06:06.000000 nornir_salt-0.9.0/
+-rw-rw-rw-   0        0        0     1546 2022-02-13 05:06:06.000000 nornir_salt-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      742 2021-12-21 01:31:19.000000 nornir_salt-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2022-02-13 05:06:05.000000 nornir_salt-0.9.0/nornir_salt/
+-rw-rw-rw-   0        0        0     3451 2022-02-13 03:56:43.000000 nornir_salt-0.9.0/nornir_salt/__init__.py
+drwxrwxrwx   0        0        0        0 2022-02-13 05:06:06.000000 nornir_salt-0.9.0/nornir_salt/plugins/
+-rw-rw-rw-   0        0        0        0 2021-12-20 12:45:47.000000 nornir_salt-0.9.0/nornir_salt/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2022-02-13 05:06:06.000000 nornir_salt-0.9.0/nornir_salt/plugins/connections/
+-rw-rw-rw-   0        0        0     4409 2021-12-20 12:42:22.000000 nornir_salt-0.9.0/nornir_salt/plugins/connections/ConnectionsPool.py
+-rw-rw-rw-   0        0        0     2641 2021-12-20 12:42:29.000000 nornir_salt-0.9.0/nornir_salt/plugins/connections/HTTPPlugin.py
+-rw-rw-rw-   0        0        0     2005 2021-12-20 12:42:33.000000 nornir_salt-0.9.0/nornir_salt/plugins/connections/NcclientPlugin.py
+-rw-rw-rw-   0        0        0     7311 2022-02-13 03:51:48.000000 nornir_salt-0.9.0/nornir_salt/plugins/connections/PyATSUnicon.py
+-rw-rw-rw-   0        0        0     2056 2021-12-20 12:42:17.000000 nornir_salt-0.9.0/nornir_salt/plugins/connections/PyGNMIPlugin.py
+-rw-rw-rw-   0        0        0      316 2021-12-20 12:42:19.000000 nornir_salt-0.9.0/nornir_salt/plugins/connections/__init__.py
+drwxrwxrwx   0        0        0        0 2022-02-13 05:06:06.000000 nornir_salt-0.9.0/nornir_salt/plugins/functions/
+-rw-rw-rw-   0        0        0     5841 2022-02-13 03:42:12.000000 nornir_salt-0.9.0/nornir_salt/plugins/functions/DumpResults.py
+-rw-rw-rw-   0        0        0    13359 2022-02-13 03:56:44.000000 nornir_salt-0.9.0/nornir_salt/plugins/functions/FFun.py
+-rw-rw-rw-   0        0        0     4520 2022-02-13 03:42:21.000000 nornir_salt-0.9.0/nornir_salt/plugins/functions/HostsKeepalive.py
+-rw-rw-rw-   0        0        0    11326 2022-02-13 04:00:18.000000 nornir_salt-0.9.0/nornir_salt/plugins/functions/InventoryFun.py
+-rw-rw-rw-   0        0        0     9731 2022-02-13 03:56:44.000000 nornir_salt-0.9.0/nornir_salt/plugins/functions/ResultSerializer.py
+-rw-rw-rw-   0        0        0     6357 2022-02-13 03:42:03.000000 nornir_salt-0.9.0/nornir_salt/plugins/functions/TabulateFormatter.py
+-rw-rw-rw-   0        0        0      413 2022-02-13 03:42:08.000000 nornir_salt-0.9.0/nornir_salt/plugins/functions/__init__.py
+drwxrwxrwx   0        0        0        0 2022-02-13 05:06:06.000000 nornir_salt-0.9.0/nornir_salt/plugins/inventory/
+-rw-rw-rw-   0        0        0     3921 2021-12-20 12:43:37.000000 nornir_salt-0.9.0/nornir_salt/plugins/inventory/DictInventory.py
+-rw-rw-rw-   0        0        0       82 2021-12-20 12:43:41.000000 nornir_salt-0.9.0/nornir_salt/plugins/inventory/__init__.py
+drwxrwxrwx   0        0        0        0 2022-02-13 05:06:06.000000 nornir_salt-0.9.0/nornir_salt/plugins/processors/
+-rw-rw-rw-   0        0        0    61904 2022-02-13 03:56:37.000000 nornir_salt-0.9.0/nornir_salt/plugins/processors/DataProcessor.py
+-rw-rw-rw-   0        0        0     8034 2022-02-13 03:43:10.000000 nornir_salt-0.9.0/nornir_salt/plugins/processors/DiffProcessor.py
+-rw-rw-rw-   0        0        0     1368 2022-02-13 04:00:28.000000 nornir_salt-0.9.0/nornir_salt/plugins/processors/N2GProcessor.py
+-rw-rw-rw-   0        0        0     6600 2022-02-13 03:43:04.000000 nornir_salt-0.9.0/nornir_salt/plugins/processors/SaltEventProcessor.py
+-rw-rw-rw-   0        0        0    41308 2022-02-13 03:56:46.000000 nornir_salt-0.9.0/nornir_salt/plugins/processors/TestsProcessor.py
+-rw-rw-rw-   0        0        0     8120 2022-02-13 03:56:44.000000 nornir_salt-0.9.0/nornir_salt/plugins/processors/ToFileProcessor.py
+-rw-rw-rw-   0        0        0      349 2022-02-13 03:43:17.000000 nornir_salt-0.9.0/nornir_salt/plugins/processors/__init__.py
+drwxrwxrwx   0        0        0        0 2022-02-13 05:06:06.000000 nornir_salt-0.9.0/nornir_salt/plugins/runners/
+-rw-rw-rw-   0        0        0     2995 2021-12-20 12:41:49.000000 nornir_salt-0.9.0/nornir_salt/plugins/runners/QueueRunner.py
+-rw-rw-rw-   0        0        0    21885 2022-02-13 03:56:45.000000 nornir_salt-0.9.0/nornir_salt/plugins/runners/RetryRunner.py
+-rw-rw-rw-   0        0        0      116 2021-12-20 12:41:55.000000 nornir_salt-0.9.0/nornir_salt/plugins/runners/__init__.py
+drwxrwxrwx   0        0        0        0 2022-02-13 05:06:06.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/
+-rw-rw-rw-   0        0        0     1596 2022-02-13 03:44:20.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/__init__.py
+-rw-rw-rw-   0        0        0     2155 2022-02-13 03:44:24.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/connections.py
+-rw-rw-rw-   0        0        0    15422 2022-02-13 03:44:27.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/files.py
+-rw-rw-rw-   0        0        0     7725 2022-02-13 03:44:30.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/http_call.py
+-rw-rw-rw-   0        0        0     2854 2022-02-13 03:44:34.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/napalm_configure.py
+-rw-rw-rw-   0        0        0     5211 2022-02-13 03:44:37.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/napalm_send_commands.py
+-rw-rw-rw-   0        0        0    10804 2022-02-13 03:58:19.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/ncclient_call.py
+-rw-rw-rw-   0        0        0     8143 2022-02-13 03:44:43.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/netmiko_send_command_ps.py
+-rw-rw-rw-   0        0        0     5161 2022-02-13 03:44:46.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/netmiko_send_commands.py
+-rw-rw-rw-   0        0        0     6353 2022-02-13 03:44:50.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/netmiko_send_config.py
+-rw-rw-rw-   0        0        0     2084 2022-02-13 03:44:52.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/nr_test.py
+-rw-rw-rw-   0        0        0     1744 2022-02-13 03:44:58.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/pyats_genie_api.py
+-rw-rw-rw-   0        0        0    10276 2022-02-13 03:45:01.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/pyats_send_commands.py
+-rw-rw-rw-   0        0        0     4716 2022-02-13 03:43:48.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/pyats_send_config.py
+-rw-rw-rw-   0        0        0     9589 2022-02-13 03:43:54.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/pygnmi_call.py
+-rw-rw-rw-   0        0        0     1424 2022-02-13 03:43:57.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/salt_cfg_gen.py
+-rw-rw-rw-   0        0        0     2282 2022-02-13 03:44:00.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/salt_clear_hcache.py
+-rw-rw-rw-   0        0        0     8232 2022-02-13 04:02:09.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/scrapli_netconf_call.py
+-rw-rw-rw-   0        0        0     4425 2022-02-13 03:44:06.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/scrapli_send_commands.py
+-rw-rw-rw-   0        0        0     2963 2022-02-13 03:44:09.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/scrapli_send_config.py
+-rw-rw-rw-   0        0        0     1211 2022-02-13 04:03:36.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/sleep.py
+-rw-rw-rw-   0        0        0     2376 2022-02-13 03:44:16.000000 nornir_salt-0.9.0/nornir_salt/plugins/tasks/tcp_ping.py
+drwxrwxrwx   0        0        0        0 2022-02-13 05:06:06.000000 nornir_salt-0.9.0/nornir_salt.egg-info/
+-rw-rw-rw-   0        0        0     1546 2022-02-13 05:06:05.000000 nornir_salt-0.9.0/nornir_salt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2421 2022-02-13 05:06:05.000000 nornir_salt-0.9.0/nornir_salt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-02-13 05:06:05.000000 nornir_salt-0.9.0/nornir_salt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      414 2022-02-13 05:06:05.000000 nornir_salt-0.9.0/nornir_salt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2022-02-13 05:06:05.000000 nornir_salt-0.9.0/nornir_salt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2022-02-13 05:06:05.000000 nornir_salt-0.9.0/nornir_salt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-02-13 05:06:06.000000 nornir_salt-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1365 2022-02-13 05:04:53.000000 nornir_salt-0.9.0/setup.py
```

### Comparing `nornir_salt-0.8.0/PKG-INFO` & `nornir_salt-0.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nornir_salt
-Version: 0.8.0
+Version: 0.9.0
 Summary: Nornir plugins used with SALTSTACK
 Home-page: https://github.com/dmulyalin/nornir-salt
 Author: Denis Mulyalin
 Author-email: d.mulyalin@gmail.com
 License: UNKNOWN
 Description: [![Downloads](https://pepy.tech/badge/nornir-salt)](https://pepy.tech/project/nornir-salt)
         [![PyPI versions](https://img.shields.io/pypi/pyversions/nornir-salt.svg)](https://pypi.python.org/pypi/nornir-salt/)
@@ -22,11 +22,13 @@
         
         Issues, bug reports and feature requests are welcomed.
         
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `nornir_salt-0.8.0/README.md` & `nornir_salt-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/__init__.py` & `nornir_salt-0.9.0/nornir_salt/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 be used standalone unless stated otherwise.
 
 While it was possible to include all the plugins into salt-nornir proxy module, decision was made
 that many of the plugins developed can be useful outside of salt-nornir proxy module scope.
 """
 # misc functions
 from .plugins.functions import ResultSerializer
-from .plugins.functions import FFun
+from .plugins.functions import FFun, FFun_functions
 from .plugins.functions import TabulateFormatter
 from .plugins.functions import DumpResults
 from .plugins.functions import InventoryFun
 
 # inventory plugins
 from .plugins.inventory import DictInventory
 
@@ -61,14 +61,15 @@
 from .plugins.processors import DiffProcessor
 from .plugins.processors import DataProcessor
 from .plugins.processors import SaltEventProcessor
 
 __all__ = (
     "ResultSerializer",
     "FFun",
+    "FFun_functions",
     "DictInventory",
     "QueueRunner",
     "RetryRunner",
     "tcp_ping",
     "netmiko_send_commands",
     "netmiko_send_command_ps",
     "nr_test",
```

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/connections/ConnectionsPool.py` & `nornir_salt-0.9.0/nornir_salt/plugins/connections/ConnectionsPool.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/connections/HTTPPlugin.py` & `nornir_salt-0.9.0/nornir_salt/plugins/connections/HTTPPlugin.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/connections/NcclientPlugin.py` & `nornir_salt-0.9.0/nornir_salt/plugins/connections/NcclientPlugin.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/connections/PyATSUnicon.py` & `nornir_salt-0.9.0/nornir_salt/plugins/connections/PyATSUnicon.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
     Where ``host-1-foo`` is Nornir invetory host name and ``host-1-bar`` is actual device prompt
     as seen on cli, these two keys must be of the same value.
 
     This plugin establishes all connections to device on startup.
 
     To use connections pool instead of single connection, need to provide ``pool`` argument integer
-    of value more or equal to 2 in connection's parametre, otherwise connection ignored::
+    of value more or equal to 2 in connection's parameters, otherwise connection ignored::
 
         host-1:
           hostname: 192.168.16.20
           username: admin
           password: admin
           connection_options:
             pyats:
@@ -158,14 +158,16 @@
                 device_data["credentials"] = {
                     "default": {"username": username, "password": password}
                 }
             if "connections" not in device_data:
                 device_data["connections"] = {
                     "default": {"protocol": "ssh", "ip": hostname, "port": port or 22}
                 }
+            if "telnet" in platform:
+                device_data["connections"]["default"]["protocol"] = "telnet"
             if "os" not in device_data and platform:
                 device_data["os"] = platform
 
             # add/extract data to/from connections
             for connection_name, connection_data in device_data["connections"].items():
                 # check if connection is a pool
                 pool_size = int(connection_data.pop("pool", 0))
```

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/connections/PyGNMIPlugin.py` & `nornir_salt-0.9.0/nornir_salt/plugins/connections/PyGNMIPlugin.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/functions/DumpResults.py` & `nornir_salt-0.9.0/nornir_salt/plugins/functions/DumpResults.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/functions/FFun.py` & `nornir_salt-0.9.0/nornir_salt/plugins/functions/FFun.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Nornir interacts with many devices and has it's own inventory. FFun is an extension
 that uses Nornir's built-in filtering capabilities to narrow down tasks execution
 to certain hosts/devices.
 
 Filtering order::
 
-    FO -> FB -> FC -> FR -> FG -> FP -> FL -> FN
+    FO -> FB -> FC -> FR -> FG -> FP -> FL -> FM -> FN
 
 .. note:: If multiple filters provided, hosts must pass all checks - ``AND`` logic - to succeed.
 
 
 FFun filters overview
 =====================
 
@@ -103,14 +103,25 @@
 FL - Filter List
 ----------------
 
 Match only hosts with names in provided list::
 
     filtered_hosts = FFun(NornirObj, FL="R1, R2")
 
+FM - Filter platforM
+--------------------
+
+Match only hosts with given platform name patterns::
+
+    filtered_hosts = FFun(NornirObj, FM="cisco*, huawei*")
+    filtered_hosts = FFun(NornirObj, FM="cisco*")
+    filtered_hosts = FFun(NornirObj, FM=["cisco*", "huawei*"])
+
+If list of patterns provided, host with platform matching at least one pattern passes this check.
+
 FN - Filter Negate
 ------------------
 
 Negate matching results if ``FN`` argument set to ``True``::
 
     # will match all hosts except R1 and R2
     filtered_hosts = FFun(NornirObj, FL="R1, R2", FN=True)
@@ -194,14 +205,17 @@
 import logging
 from fnmatch import fnmatchcase
 from nornir.core.filter import F
 
 
 log = logging.getLogger(__name__)
 
+# list that enumerates all available FFun functions, useful for arguments filtering
+FFun_functions = ["FO", "FB", "FC", "FR", "FG", "FP", "FL", "FM", "FN"]
+
 
 def FFun(nr, check_if_has_filter=False, **kwargs):
     """
     Inventory filters dispatcher function.
 
     :param nr: Nornir object
     :param kwargs: Dictionary with filtering parameters e.g. {"FB": "host1*", "FL": ["host1", "host2"]}
@@ -241,14 +255,17 @@
         has_filter = True
     if kwargs.get("FP"):
         ret = _filter_FP(ret, kwargs.pop("FP"))
         has_filter = True
     if "FL" in kwargs:
         ret = _filter_FL(ret, kwargs.pop("FL"))
         has_filter = True
+    if "FM" in kwargs:
+        ret = _filter_FM(ret, kwargs.pop("FM"))
+        has_filter = True
     if "FN" in kwargs:
         ret = _filter_FN(ret, nr, kwargs.pop("FN"))
     return (ret, has_filter) if check_if_has_filter else ret
 
 
 def _filter_FO(nr, filter_data):
     """
@@ -373,14 +390,32 @@
     )
     if "_all_" in names_list:
         return ret
     else:
         return ret.filter(filter_func=lambda h: h.name in names_list)
 
 
+def _filter_FM(ret, pattern):
+    """
+    Function to filter hosts by platform glob patterns
+    """
+    # check if comma separated list of patterns given
+    if isinstance(pattern, str) and "," in pattern:
+        pattern = [i.strip() for i in pattern.split(",")]
+    # run filtering
+    if isinstance(pattern, list):
+        return ret.filter(
+            filter_func=lambda h: any(
+                [fnmatchcase(h.platform, str(p)) for p in pattern]
+            )
+        )
+    else:
+        return ret.filter(filter_func=lambda h: fnmatchcase(h.platform, str(pattern)))
+
+
 def _filter_FN(ret, nr, FN):
     """
     Function to negate hosts' match results
     """
     if FN is not True:
         return ret
     all_hosts = set(nr.inventory.hosts.keys())
```

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/functions/HostsKeepalive.py` & `nornir_salt-0.9.0/nornir_salt/plugins/functions/HostsKeepalive.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/functions/InventoryFun.py` & `nornir_salt-0.9.0/nornir_salt/plugins/functions/InventoryFun.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,14 @@
 .. autofunction:: nornir_salt.plugins.functions.InventoryFun._read_inventory
 .. autofunction:: nornir_salt.plugins.functions.InventoryFun._update_host
 .. autofunction:: nornir_salt.plugins.functions.InventoryFun._delete_host
 .. autofunction:: nornir_salt.plugins.functions.InventoryFun._load
 .. autofunction:: nornir_salt.plugins.functions.InventoryFun._list_hosts
 """
 import logging
-import traceback
 
 from .FFun import FFun
 from nornir.core.inventory import Host, ConnectionOptions
 
 log = logging.getLogger(__name__)
```

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/functions/ResultSerializer.py` & `nornir_salt-0.9.0/nornir_salt/plugins/functions/ResultSerializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -205,19 +205,15 @@
         return nr_results
 
     # form nested dictionary structure
     if to_dict:
         ret = {}
         for hostname, results in nr_results.items():
             for i in results:
-                exception = (
-                    str(i.exception)
-                    if i.exception is not None
-                    else i.host.get("exception", None)
-                )
+                exception = str(i.exception) if i.exception is not None else None
                 # skip tasks such as _task_foo_bar unless exception
                 if i.name and i.name.startswith("_") and not exception:
                     continue
                 # skip tasks if signaled to do so
                 elif (
                     hasattr(i, "skip_results")
                     and i.skip_results is True
@@ -244,19 +240,15 @@
                     )
 
     # form plain list of results
     else:
         ret = []
         for hostname, results in nr_results.items():
             for i in results:
-                exception = (
-                    str(i.exception)
-                    if i.exception is not None
-                    else i.host.get("exception", None)
-                )
+                exception = str(i.exception) if i.exception is not None else None
                 # skip group tasks such as _task_foo_bar unless exception
                 if i.name and i.name.startswith("_") and not exception:
                     continue
                 # skip tasks if signalled to do so
                 elif (
                     hasattr(i, "skip_results")
                     and i.skip_results is True
```

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/functions/TabulateFormatter.py` & `nornir_salt-0.9.0/nornir_salt/plugins/functions/TabulateFormatter.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/inventory/DictInventory.py` & `nornir_salt-0.9.0/nornir_salt/plugins/inventory/DictInventory.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/processors/DataProcessor.py` & `nornir_salt-0.9.0/nornir_salt/plugins/processors/DataProcessor.py`

 * *Files 7% similar despite different names*

```diff
@@ -458,29 +458,101 @@
 
     This function is useful to explore deeply nested structures such as XML
     output obtained from devices over NETCONF.
 
     Another usecase is filtering of the keys in resulted dictionary, as
     they are the strings, glob or regex matching can be applied on them.
 
-    :param data: nested data to flatten
-    :param parent_key: string to prepend to dictionary's keys, used by recursion
-    :param separator: string to separate flattened keys
-    :return: flattened structure
+    :param data: (dict or list) nested data to flatten
+    :param parent_key: (str) string to prepend to dictionary's keys, used by recursion
+    :param separator: (str) string to separate flattened keys
+    :param kwargs: (dict) not in use
+    :return: ()dict flattened dictionary structure
 
     Based on Stackoverflow answer:
     https://stackoverflow.com/a/62186053/12300761
 
     All credits for the idea to https://github.com/ScriptSmith
 
-    Sample usage::
+    Example how to invoke ``flatten`` function directly::
 
-        flatten({'a': 1, 'c': {'a': 2, 'b': {'x': 5, 'y' : 10}}, 'd': [1, 2, 3] })
+        import pprint
+        from nornir_salt.plugins.processors.DataProcessor import flatten
 
-        >> {'a': 1, 'c.a': 2, 'c.b.x': 5, 'c.b.y': 10, 'd.0': 1, 'd.1': 2, 'd.2': 3}
+        nested_data = {'bgp_cfg': {'ASN': '12.34',
+                      'ipv4_afi': {'bgp_rid': '1.1.1.1'},
+                      'vrfs': [{'neighbors': [{'ipv4_afi': {'RPL_IN': 'vCE102-link1.102',
+                                                            'RPL_OUT': 'vCE102-link1.102',
+                                                            'send_community_ebgp': 'Enabled'},
+                                               'neighbor': '10.1.102.102',
+                                               'neighbor_asn': '102.103'},
+                                              {'ipv4_afi': {'RPL_IN': 'vCE102-link2.102',
+                                                            'RPL_OUT': 'vCE102-link2.102'},
+                                               'neighbor': '10.2.102.102',
+                                               'neighbor_asn': '102.103'}],
+                                'rd': '102:103',
+                                'vrf': 'CT2S2'},
+                               {'neighbors': [{'ipv4_afi': {'RPL_IN': 'PASS-ALL',
+                                                            'RPL_OUT': 'PASS-ALL'}},
+                                              {'neighbor': '10.1.37.7',
+                                               'neighbor_asn': '65000'}],
+                                'rd': '102:104',
+                                'vrf': 'AS65000'}]}}
+
+        flat_data = flatten(nested_data)
+
+        pprint.pprint(flat_data)
+
+        # prints:
+        # {'bgp_cfg.ASN': '12.34',
+        #  'bgp_cfg.ipv4_afi.bgp_rid': '1.1.1.1',
+        #  'bgp_cfg.vrfs.0.neighbors.0.ipv4_afi.RPL_IN': 'vCE102-link1.102',
+        #  'bgp_cfg.vrfs.0.neighbors.0.ipv4_afi.RPL_OUT': 'vCE102-link1.102',
+        #  'bgp_cfg.vrfs.0.neighbors.0.ipv4_afi.send_community_ebgp': 'Enabled',
+        #  'bgp_cfg.vrfs.0.neighbors.0.neighbor': '10.1.102.102',
+        #  'bgp_cfg.vrfs.0.neighbors.0.neighbor_asn': '102.103',
+        #  'bgp_cfg.vrfs.0.neighbors.1.ipv4_afi.RPL_IN': 'vCE102-link2.102',
+        #  'bgp_cfg.vrfs.0.neighbors.1.ipv4_afi.RPL_OUT': 'vCE102-link2.102',
+        #  'bgp_cfg.vrfs.0.neighbors.1.neighbor': '10.2.102.102',
+        #  'bgp_cfg.vrfs.0.neighbors.1.neighbor_asn': '102.103',
+        #  'bgp_cfg.vrfs.0.rd': '102:103',
+        #  'bgp_cfg.vrfs.0.vrf': 'CT2S2',
+        #  'bgp_cfg.vrfs.1.neighbors.0.ipv4_afi.RPL_IN': 'PASS-ALL',
+        #  'bgp_cfg.vrfs.1.neighbors.0.ipv4_afi.RPL_OUT': 'PASS-ALL',
+        #  'bgp_cfg.vrfs.1.neighbors.1.neighbor': '10.1.37.7',
+        #  'bgp_cfg.vrfs.1.neighbors.1.neighbor_asn': '65000',
+        #  'bgp_cfg.vrfs.1.rd': '102:104',
+        #  'bgp_cfg.vrfs.1.vrf': 'AS65000'}
+
+    To invoke flatten function as part of Nornir task run, need to make sure that task returns
+    list or dictionary structure, alternatively, if YAML/XML/JSON string returned, need to load it
+    first. For example, to flatten XML structure, first need to use `load_xml`_ function, next
+    pass dictionary produced by ``load_xml`` through ``flatten`` function::
+
+        from nornir import InitNornir
+        from nornir_salt import ncclient_call, DataProcessor
+
+        nr = InitNornir(config_file="config.yaml")
+
+        nr_with_processor = nr.with_processors([
+            DataProcessor(
+                [
+                    {"fun": "load_xml"},
+                    {"fun": "flatten"},
+                ]
+            )
+        ])
+
+        nr_with_processor.run(
+            task=ncclient_call,
+            call="get_config",
+            source="running"
+        )
+
+    Above example produces same result as to calling `xml_flatten`_ function.
     """
     items = []
     if isinstance(data, dict):
         for key, value in data.items():
             new_key = "{}{}{}".format(parent_key, separator, key) if parent_key else key
             items.extend(flatten(value, new_key, separator).items())
     elif isinstance(data, list):
@@ -574,15 +646,18 @@
     return to_json(data=load_xml(data, py_dict=False), **kwargs)
 
 
 def xml_flatten(data, **kwargs):
     """
     Reference name ``xml_flatten``
 
-    Dependencies: requires LXML library - ``pip install lxml``
+    Dependencies:
+
+    - requires LXML library - ``pip install lxml``
+    - requires xmltodict library - ``pip install xmltodict``
 
     Function to transform XML in a flattened python dictionary representation
 
     Steps are:
 
     1. Transform XML to Python dictionary using xmltodict by calling ``load_xml`` function
     2. Flatten python dictionary calling ``flatten`` function
```

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/processors/DiffProcessor.py` & `nornir_salt-0.9.0/nornir_salt/plugins/processors/DiffProcessor.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/processors/N2GProcessor.py` & `nornir_salt-0.9.0/nornir_salt/plugins/processors/N2GProcessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 N2GProcessor reference
 =========================
 
 .. autofunction:: nornir_salt.plugins.processors.N2GProcessor.N2GProcessor
 """
 import logging
-import traceback
 
 from nornir.core.inventory import Host
 from nornir.core.task import AggregatedResult, MultiResult, Task
 
 
 log = logging.getLogger(__name__)
```

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/processors/SaltEventProcessor.py` & `nornir_salt-0.9.0/nornir_salt/plugins/processors/SaltEventProcessor.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/processors/TestsProcessor.py` & `nornir_salt-0.9.0/nornir_salt/plugins/processors/TestsProcessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -464,28 +464,31 @@
     result,
     function_file=None,
     function_text=None,
     function_call=None,
     function_name="run",
     function_kwargs=None,
     globals_dictionary=None,
+    add_host=False,
     **kwargs
 ):
     """
     Wrapper around calling custom function to perform results checks.
 
     :param host: (obj) Nornir host object
     :param result: ``nornir.core.task.Result`` object
     :param function_name: (str) function name, default is ``run``
     :param function_file: (str) OS path to file with ``function_name`` function
     :param function_text: (str) Python code text for ``function_name`` function
     :param function_call: (callable) reference to callable python function
     :param globals_dictionary: (dict) dictionary to merge with global space of the custom function,
       used only if ``function_file`` or ``function_text`` arguments provided.
     :param function_kwargs: (dict) ``**function_kwargs`` to pass on to custom function
+    :param add_host: (bool) default is False, if True adds ``host`` argument to ``function_kwargs``
+      as a reference to Nornir Host object that this function executing for
     :param kwargs: (dict) any additional key word arguments to include in results
 
     .. warning:: ``function_file`` and ``function_text`` use ``exec`` function
        to compile python code, using test functions from untrusted sources can
        be dangerous.
 
     Custom functions should accept one positional argument for results following these rules:
@@ -549,14 +552,17 @@
                             "success": False
                         })
             return ret
     """
     function_kwargs = function_kwargs or {}
     globals_dictionary = globals_dictionary or {}
 
+    if add_host:
+        function_kwargs["host"] = host
+
     # form ret structure
     ret = test_result_template.copy()
     ret.update(kwargs)
 
     # load and compile custom function
     try:
         if function_text:
@@ -710,53 +716,77 @@
 
 def ContainsTest(
     host,
     result,
     pattern,
     use_re=False,
     count=None,
+    count_ge=None,
+    count_le=None,
     revert=False,
     err_msg=None,
     **kwargs
 ):
     """
     Function to check if pattern contained in output of given result.
 
     :param host: (obj) Nornir host object
     :param result: (obj) ``nornir.core.task.Result`` object
     :param pattern: (str) pattern to check containment for
     :param use_re: (bool) if True uses re.search to check for pattern in output
     :param count: (int) check exact number of pattern occurrences in the output
+    :param count_ge: (int) check number of pattern occurrences in the output is greater or equal to given value
+    :param count_le: (int) check number of pattern occurrences in the output is lower or equal to given value
     :param revert: (bool) if True, changes results to opposite - check lack of containment
     :param err_msg: (str) exception message to use on test failure
     :param kwargs: (dict) any additional ``**kwargs`` keyword arguments to include in return Result object
     :return result: ``nornir.core.task.Result`` object with test results
     """
+    pattern = str(pattern)
     # form ret structure
     ret = test_result_template.copy()
     ret.update(kwargs)
     ret["criteria"] = (
         pattern.replace("\n", "\\n")
         if len(pattern) < 25
         else pattern[0:24].replace("\n", "\\n")
     )
 
     # add count to return results
     if count:
         ret["count"] = count
+    if count_ge:
+        ret["count_ge"] = count_ge
+    if count_le:
+        ret["count_le"] = count_le
+
     # run the check
     if use_re:
         if not re.search(pattern, result.result):
             ret.update({"result": "FAIL", "success": False})
             ret["exception"] = err_msg if err_msg else "Regex pattern not in output"
     elif count and result.result.count(pattern) != count:
         ret.update({"result": "FAIL", "success": False})
         ret["exception"] = (
             err_msg if err_msg else "Pattern not in output {} times".format(count)
         )
+    elif count_ge and result.result.count(pattern) < count_ge:
+        ret.update({"result": "FAIL", "success": False})
+        ret["exception"] = (
+            err_msg
+            if err_msg
+            else "Pattern not in output greater or equal {} times".format(count_ge)
+        )
+    elif count_le and result.result.count(pattern) > count_le:
+        ret.update({"result": "FAIL", "success": False})
+        ret["exception"] = (
+            err_msg
+            if err_msg
+            else "Pattern not in output lower or equal {} times".format(count_le)
+        )
     elif pattern not in result.result:
         ret.update({"result": "FAIL", "success": False})
         ret["exception"] = err_msg if err_msg else "Pattern not in output"
     # revert results if requested to do so
     if revert:
         if ret["success"] is False:
             ret.update({"result": "PASS", "success": True})
@@ -765,14 +795,26 @@
             ret.update({"result": "FAIL", "success": False})
             if use_re:
                 ret["exception"] = err_msg if err_msg else "Regex pattern in output"
             elif count:
                 ret["exception"] = (
                     err_msg if err_msg else "Pattern in output {} times".format(count)
                 )
+            elif count_ge:
+                ret["exception"] = (
+                    err_msg
+                    if err_msg
+                    else "Pattern in output greater or equal {} times".format(count_ge)
+                )
+            elif count_le:
+                ret["exception"] = (
+                    err_msg
+                    if err_msg
+                    else "Pattern in output lower or equal {} times".format(count_le)
+                )
             else:
                 ret["exception"] = err_msg if err_msg else "Pattern in output"
     return Result(host=host, **ret)
 
 
 test_functions_dispatcher = {
     "contains": {"fun": ContainsTest, "kwargs": {}},
@@ -813,82 +855,102 @@
     :param kwargs: (any) if provided, ``**kwargs`` will form a single test item
     :param failed_only: (bool) if True, includes only failed tests in results, default is False
     """
 
     def __init__(self, tests=None, remove_tasks=True, failed_only=False, **kwargs):
         self.tests = tests if tests else [kwargs]
         self.remove_tasks = remove_tasks
-        self.len_tasks = None
+        self.len_tasks = 0
         self.failed_only = failed_only
 
     def task_started(self, task: Task) -> None:
         pass
 
     def task_instance_started(self, task: Task, host: Host) -> None:
         pass
 
     def task_instance_completed(
         self, task: Task, host: Host, result: MultiResult
     ) -> None:
         """
         Method to iterate over individual hosts's result after task/sub-tasks completion.
         """
+        # check if has failed tasks, do nothing in such a case
+        if result.failed:
+            log.error("nornir_salt:TestsProcessor has failed tasks, do nothing, return")
+            return
+
         try:
             # record the len of tasks to clean them up if required
             if self.remove_tasks:
                 self.len_tasks = len(result)
             # do the tests
             for test in self.tests:
+                # make a copy of test item to not iterfere with other hosts' testing
                 test = test.copy()
 
                 # if test item is a list, transform it to dictionary
                 if isinstance(test, list):
                     test = {
                         "task": test[0],
                         "test": test[1],
                         "pattern": test[2],
                         "name": test[3] if len(test) == 4 else None,
                     }
                     if test["test"] in ["eval", "EvalTest"]:
                         test["expr"] = test.pop("pattern")
 
+                # make sure has result item in a test
+                test["result"] = None
+
                 # make sure we have test name defined
                 if not test.get("name"):
                     test["name"] = "{} {} {}..".format(
-                        test["task"], test["test"], test.get("pattern", "")[:9]
+                        test["task"], test["test"], str(test.get("pattern", ""))[:9]
                     )
 
                 # get task results to use; use all results
                 if test.get("use_all_tasks") is True:
                     test["result"] = result
                 # use subset of task results
                 elif isinstance(test["task"], list):
                     test["result"] = []
-                    for task_result in result:
-                        if task_result.name in test["task"]:
-                            test["result"].append(task_result)
+                    for i in result:
+                        # check if need to skip this task
+                        if hasattr(i, "skip_results") and i.skip_results is True:
+                            continue
+                        if i.name in test["task"]:
+                            test["result"].append(i)
                 # use results for single task only
                 else:
                     # try to find task by matching it's name
-                    for task_result in result:
-                        if task_result.name == test["task"]:
-                            test["result"] = task_result
+                    for i in result:
+                        # check if need to skip this task
+                        if hasattr(i, "skip_results") and i.skip_results is True:
+                            continue
+                        if i.name == test["task"]:
+                            test["result"] = i
                             break
                     else:
                         # use first task if only one test and one task given
                         tasks = [t for t in result if not hasattr(t, "skip_results")]
                         if len(self.tests) == 1 and len(tasks) == 1:
                             test["result"] = tasks[0]
-                        else:
-                            log.warning(
-                                "nornir-salt:TestsProcessor: no results for task '{}'".format(
-                                    test["task"]
-                                )
-                            )
-                            continue
+
+                # check if found no task results for this test item
+                if test["result"] is None or test["result"] == []:
+                    test[
+                        "exception"
+                    ] = "Found no results to test - all tasks failed or test name does not match any of task names"
+                    test["result"] = "ERROR"
+                    test["success"] = False
+                    ret = {**test_result_template.copy(), **test}
+                    _ = ret.pop("expr", None)
+                    result.append(Result(host=host, **ret))
+                    continue
 
                 # get test function and function kwargs
                 if test["test"] in test_functions_dispatcher:
                     test_func = test_functions_dispatcher[test["test"]]["fun"]
                     test.update(test_functions_dispatcher[test["test"]]["kwargs"])
                 elif test["test"] in globals() and "Test" in test["test"]:
                     test_func = globals()[test["test"]]
@@ -896,14 +958,17 @@
                     raise NameError(
                         "nornir-salt:TestsProcessor unsupported test function '{}'".format(
                             test["test"]
                         )
                     )
 
                 # run the test
+                log.debug(
+                    "nornir-salt:TestsProcessor running test '{}'".format(test["name"])
+                )
                 try:
                     # run test for data at given path
                     if test.get("path"):
                         report_all = test.pop("report_all", False)
                         res = [
                             test_func(host=host, result=item, **test)
                             for item in _get_result_by_path(
```

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/processors/ToFileProcessor.py` & `nornir_salt-0.9.0/nornir_salt/plugins/processors/ToFileProcessor.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     ToFileProcessor can save task execution results to file on a per host basis.
     If multiple tasks present, results of all of them saved in same file.
 
     :param tf: (str) name of the file groups content
     :param base_url: (str) OS path to folder where to save files, default "/var/nornir-salt/"
     :param max_files: (int) default is 5, maximum number of file for given ``tf`` file group
     :param index: (str) index filename to read and store files data into
+    :param skip_failed: (bool) if True, do not save failed task results, default is False
 
     Files saved under ``base_url`` location, where individual filename formed using string::
 
         {tf}__{timestamp}__{rand}__{hostname}.txt
 
     Where:
 
@@ -85,19 +86,27 @@
     ``show run | inc ntp`` task results span indexes inside
     ``./tofile_outputs/config__22_August_2021_14_08_33__IOL1.txt`` text file.
 
     ``tf_index_{index}.json`` used by other plugins to retrieve previous results for the task,
     it could be considered as a simplified index database.
     """
 
-    def __init__(self, tf, base_url="/var/nornir-salt/", max_files=5, index=None):
+    def __init__(
+        self,
+        tf,
+        base_url="/var/nornir-salt/",
+        max_files=5,
+        index=None,
+        skip_failed=False,
+    ):
         self.tf = tf
         self.base_url = base_url
         self.max_files = max(1, max_files)
         self.index = index or "common"
+        self.skip_failed = skip_failed
 
         self.aliases_file = os.path.join(
             base_url, "tf_index_{}.json".format(self.index)
         )
         self.aliases_data = {}  # dictionary to store tf_index_{index}.json content
 
         self._load_aliases()
@@ -128,14 +137,21 @@
     def task_instance_started(self, task: Task, host: Host) -> None:
         pass  # ignore
 
     def task_instance_completed(
         self, task: Task, host: Host, result: MultiResult
     ) -> None:
         """save to file on a per-host basis"""
+        if result.failed and self.skip_failed:
+            log.warning(
+                "nornir_salt:ToFileProcessor '{}' has failed tasks and skip_failed is True, do nothing, return".format(
+                    host.name
+                )
+            )
+            return
 
         host_filename = "{tf}__{timestamp}__{rand}__{hostname}.txt".format(
             timestamp=time.strftime("%d_%B_%Y_%H_%M_%S"),
             rand=random.randint(0, 1000),  # nosec
             hostname=host.name,
             tf=self.tf,
         )
@@ -155,26 +171,25 @@
                     "tasks": {},
                     "timestamp": time.strftime("%d %b %Y %H:%M:%S %Z"),
                 },
             )
             span_start = 0
 
             for i in result:
-                # check if need to skip this task results
-                exception = (
-                    str(i.exception)
-                    if i.exception is not None
-                    else i.host.get("exception", None)
-                )
+                # skip if has skip_results and no exception
                 if (
                     hasattr(i, "skip_results")
                     and i.skip_results is True
-                    and not exception
+                    and not i.exception
                 ):
                     continue
+                # skip if has exception but skip_failed is True
+                if i.exception and self.skip_failed:
+                    continue
+
                 # save results to file
                 if isinstance(i.result, (str, int, float, bool)):
                     result_to_save = str(i.result)
                     self.aliases_data[self.tf][host.name][0]["tasks"][i.name] = {
                         "content_type": "str"
                     }
                 # convert structured data to json
```

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/runners/QueueRunner.py` & `nornir_salt-0.9.0/nornir_salt/plugins/runners/QueueRunner.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/runners/RetryRunner.py` & `nornir_salt-0.9.0/nornir_salt/plugins/runners/RetryRunner.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,38 @@
 
 .. warning:: For grouped tasks need to explicitly provide `connection_name` attribute
     such as `netmiko`, `napalm`, `scrapli`. Specifying `connection_name` attribute for
     standalone tasks not required. Lack of `connection_name` attribute will result in skipping
     connection retry logic and connections to all hosts initiated simultaneously up to the
     number of `num_workers`
 
+Primary motivation for RetryRunner is to make Nornir task execution as reliable as possible
+through retry mechanisms.
+
 RetryRunner Architecture
 ========================
 
+RetryRunner helps to control the rate of connections establishment by limiting the number of
+connector workers.
+
+For example, if ``num_connectors`` is 5, it means there are only 5 workers
+to establish connections to devices, even if there are 100 devices, RetryRunner will connect
+only with 5 of them at a time. This is very helpful when connections rate need to be limited
+due to operations restrictions like AAA (TACACS, RADIUS) servers load.
+
+When new task started and if no connection exist to device that this task makes the use of,
+RetryRunner attempts to connect to device retrying up to ``connect_retry`` times.
+
+Once connection established, task handed over to worker threads for execution, workers
+will retry up to ``task_retry`` if task fails.
+
+Connection parameters such as timeouts or usage of SSH keys handled by Nornir Connection plugins.
+RetryRunner calls Nornir to start the connection, further connection establishment details
+controlled by Connection plugin itself.
+
 .. image:: ../_images/RetryRunner_v0.png
 
 RetryRunner Sample Usage
 ========================
 
 Need to instruct Nornir to use RetryRunner on instantiation::
 
@@ -151,29 +172,29 @@
         data:
           jumphost:
             hostname: 10.1.1.1
             port: 22
             password: jump_host_password
             username: jump_host_user
 
-.. note:: Only Netmiko `connection_name="netmiko"` and Ncclient `connection_name="ncclient"`
+.. note:: Only Netmiko ``connection_name="netmiko"`` and Ncclient ``connection_name="ncclient"``
     tasks, support connecting to hosts behind Jumphosts using above inventory data.
 
 RetryRunner Reference
 =====================
 
 .. autoclass:: nornir_salt.plugins.runners.RetryRunner.RetryRunner
 """
 import threading
 import queue
 import logging
 import time
 import random
 from typing import List
-from nornir.core.task import AggregatedResult, Task
+from nornir.core.task import AggregatedResult, Task, MultiResult, Result
 from nornir.core.inventory import Host
 
 try:
     import paramiko
 
     HAS_PARAMIKO = True
 except ImportError:
@@ -195,29 +216,43 @@
 ):
     while not stop_event.is_set():
         try:
             work = work_q.get(block=True, timeout=0.1)
         except queue.Empty:
             continue
         task, host, params, result = work
-        # check if need backoff task retry for this host
-        if params["task_retry"] > 0:
-            elapsed = time.time() - params["timestamp"]
-            should_wait = (params["task_retry"] * task_backoff) / 1000
-            if elapsed < should_wait:
-                work_q.put(work)
-                work_q.task_done()
-                continue
-        log.info(
-            "nornir_salt:RetryRunner {} - running task '{}'".format(
-                host.name, task.name
+        # check if has exception recorded in params by connector thread
+        if params.get("connect_exception"):
+            work_result = MultiResult(task.name)
+            work_result.append(
+                Result(
+                    host,
+                    result=params["connect_exception"],
+                    failed=True,
+                    exception=params["connect_exception"],
+                    name=task.name,
+                )
             )
-        )
-        time.sleep(random.randrange(0, task_splay) / 1000)  # nosec
-        work_result = task.start(host)
+        else:
+            # check if need backoff task retry for this host
+            if params["task_retry"] > 0:
+                elapsed = time.time() - params["timestamp"]
+                should_wait = (params["task_retry"] * task_backoff) / 1000
+                if elapsed < should_wait:
+                    work_q.put(work)
+                    work_q.task_done()
+                    continue
+            log.info(
+                "nornir_salt:RetryRunner {} - running task '{}'".format(
+                    host.name, task.name
+                )
+            )
+            time.sleep(random.randrange(0, task_splay) / 1000)  # nosec
+            work_result = task.start(host)
+        # check if need to run task retry logic
         if task.results.failed:
             log.error(
                 "nornir_salt:RetryRunner {} - task execution retry attempt {} failed: '{}'".format(
                     host.name, params["task_retry"], work_result[0].exception
                 )
             )
             if (
@@ -305,25 +340,27 @@
                     "nornir_salt:RetryRunner {} - started connection: '{}'".format(
                         host.name, connection_name
                     )
                 )
             except Exception as e:
                 # close host connections to retry them
                 close_host_connection(host, connection_name)
-                log.error(
-                    "nornir_salt:RetryRunner {} - connection retry attempt {}, error: '{}'".format(
-                        host.name, params["connection_retry"], e
-                    )
+                err_msg = "nornir_salt:RetryRunner {} - connection retry attempt {}, error: '{}'".format(
+                    host.name, params["connection_retry"], e
                 )
+                log.error(err_msg)
                 if params["connection_retry"] < connect_retry:
                     params["connection_retry"] += 1
                     params["timestamp"] = time.time()
                     connectors_q.put(connection)
                     connectors_q.task_done()
                     continue
+                else:
+                    # record exception in params for worker thread to react on it
+                    params["connect_exception"] = err_msg
         connectors_q.task_done()
         work_q.put((task, host, params, result))
 
 
 def close_host_connection(host, connection_name):
     try:
         host.close_connection(connection_name)
@@ -384,47 +421,53 @@
         except Exception as e:
             with LOCK:
                 jumphosts_connections[jumphost["hostname"]] = "__failed__"
             # add exception info to host data to include in results
             error_msg = "nornir_salt:RetryRunner failed connection to jumphost '{}', error - {}".format(
                 host["jumphost"]["hostname"], e
             )
-            host["exception"] = error_msg
+            # host["exception"] = error_msg
             log.error(error_msg)
-            return
+            raise RuntimeError(error_msg)
     else:
         # sleep random time waiting for connection to jumphost to establish
         while jumphosts_connections[jumphost["hostname"]] == "__connecting__":
             time.sleep(random.randrange(0, 500) / 1000)  # nosec
         if jumphosts_connections[jumphost["hostname"]] == "__failed__":
             # add exception info to host data to include in results
             error_msg = "nornir_salt:RetryRunner failed connection to jumphost '{}' in another thread".format(
                 host["jumphost"]["hostname"]
             )
-            host["exception"] = error_msg
+            # host["exception"] = error_msg
             log.error(error_msg)
-            return
+            raise RuntimeError(error_msg)
     # connect to host
     channel_name = "jumphost_{}_channel".format(jumphost["hostname"])
+    jconn = jumphosts_connections[jumphost["hostname"]]
+    # check if connection to jumphost was closed, reconnect if so
+    if not jconn["jumphost_ssh_transport"].is_active():
+        log.debug(
+            "nornir_salt:RetryRunner jumphost '{}' disconnected, reconnecting".format(
+                jumphost["hostname"]
+            )
+        )
+        jconn["jumphost_ssh_client"].close()
+        jumphosts_connections.pop(jumphost["hostname"])
+        return connect_to_device_behind_jumphost(host, jumphosts_connections)
+    # proceed with openning new channel via jumphost
     if not host.connections.get(channel_name):
-        dest_addr = (host.hostname, host.port or 22)
-        channel = jumphosts_connections[jumphost["hostname"]][
-            "jumphost_ssh_transport"
-        ].open_channel(
+        host.connections[channel_name] = jconn["jumphost_ssh_transport"].open_channel(
             kind="direct-tcpip",
-            dest_addr=dest_addr,
+            dest_addr=(host.hostname, host.port or 22),
             src_addr=("localhost", 7777),
             timeout=3,
         )
-        host.connections[channel_name] = channel
         log.info(
             "nornir_salt:RetryRunner {} - started new channel via jumphost '{}' - '{}'".format(
-                host.name,
-                jumphost["hostname"],
-                jumphosts_connections[jumphost["hostname"]]["jumphost_ssh_client"],
+                host.name, jumphost["hostname"], jconn["jumphost_ssh_client"]
             )
         )
     return host.connections[channel_name]
 
 
 class RetryRunner:
     """
```

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/__init__.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/connections.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/connections.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/files.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/files.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/http_call.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/http_call.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/napalm_configure.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/napalm_configure.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,17 @@
         return Result(
             host=task.host,
             failed=True,
             exception="No nornir_napalm found, is it installed?",
         )
 
     # get configuration
-    if "commands" in task.host.data.get("__task__", {}):
+    if "config" in task.host.data.get("__task__", {}):
+        config = task.host.data["__task__"]["config"]
+    elif "commands" in task.host.data.get("__task__", {}):
         config = task.host.data["__task__"]["commands"]
     elif "filename" in task.host.data.get("__task__", {}):
         config = task.host.data["__task__"]["filename"]
 
     # transform configuration to string if list/tuple given
     if isinstance(config, (list, tuple)):
         config = "\n".join(config)
```

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/napalm_send_commands.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/napalm_send_commands.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/ncclient_call.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/ncclient_call.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,14 @@
 
     HAS_LXML = True
 except ImportError:
     HAS_LXML = False
 
 try:
     from ncclient.manager import OPERATIONS
-    from ncclient.operations.errors import MissingCapabilityError
 
     HAS_NCCLIENT = True
 except ImportError:
     HAS_NCCLIENT = False
 
 try:
     # this import should work for ncclient >=0.6.10
```

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/netmiko_send_command_ps.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/netmiko_send_command_ps.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,16 @@
     :param timeout: (int) Absolute timeout in seconds of overall wait, default 120s, if
         set to -1 will wait indefinitely
     :param inter_loop_sleep: (int) Interval in seconds to sleep between reading loops, default 0.1s
     :param initial_sleep: (int) time to sleep after sending command, default 0.1s
     :param strip_prompt: (bool) Remove the trailing router prompt from the output (default: True).
     :param strip_command: (bool) Remove the echo of the command from the output (default: True).
     :param normalize: (bool) Ensure the proper enter is sent at end of command (default: True).
+    :param cutoff: (int) used as difflib get_close_matches cutoff argument to check if last line
+        looks similar to any previously seen prompts, default is 0.6
     :param nowait: (bool) Default is False, if True sends command and returns immediately without
         waiting for prompt right after ``initial_sleep`` timer elapsed.
     """
     data_received = ""
     previous_last_line = ""
     no_data_elapsed = 0
     start_time = time.time()
```

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/netmiko_send_commands.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/netmiko_send_commands.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/netmiko_send_config.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/netmiko_send_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -115,15 +115,17 @@
     kwargs.setdefault("cmd_verify", False)
     commit_final_delay = int(commit_final_delay)
     batch = max(0, int(batch))
     task_result = Result(host=task.host, result=[], changed=True)
     conn = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
 
     # get configuration from host data if any
-    if "commands" in task.host.data.get("__task__", {}):
+    if "config" in task.host.data.get("__task__", {}):
+        config = task.host.data["__task__"]["config"]
+    elif "commands" in task.host.data.get("__task__", {}):
         config = task.host.data["__task__"]["commands"]
     elif "filename" in task.host.data.get("__task__", {}):
         config = task.host.data["__task__"]["filename"]
 
     # transform configuration to a list if string given
     if isinstance(config, str):
         config = config.splitlines()
```

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/nr_test.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/nr_test.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/pyats_genie_api.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/pyats_genie_api.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/pyats_send_commands.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/pyats_send_commands.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/pyats_send_config.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/pyats_send_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,17 @@
     task_result = Result(host=task.host, result=[], changed=True)
 
     # get PyATS testbed, device object
     testbed = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
     device = testbed.devices[task.host.name]
 
     # get configuration from host data if any
-    if "commands" in task.host.data.get("__task__", {}):
+    if "config" in task.host.data.get("__task__", {}):
+        config = task.host.data["__task__"]["config"]
+    elif "commands" in task.host.data.get("__task__", {}):
         config = task.host.data["__task__"]["commands"]
     elif "filename" in task.host.data.get("__task__", {}):
         config = task.host.data["__task__"]["filename"]
 
     # transform configuration to a list if string given
     if isinstance(config, str):
         config = config.splitlines()
```

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/pygnmi_call.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/pygnmi_call.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/salt_cfg_gen.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/salt_cfg_gen.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 
     :param config: (str) configuration string to return
     :return result: Nornir result object with task execution results
     """
     task.name = "salt_cfg_gen"
 
     # get configuration
-    if "commands" in task.host.data.get("__task__", {}):
+    if "config" in task.host.data.get("__task__", {}):
+        config = task.host.data["__task__"]["config"]
+    elif "commands" in task.host.data.get("__task__", {}):
         config = task.host.data["__task__"]["commands"]
     elif "filename" in task.host.data.get("__task__", {}):
         config = task.host.data["__task__"]["filename"]
 
     # transform configuration to string if list/tuple given
     if isinstance(config, (list, tuple)):
         config = "\n".join(config)
```

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/salt_clear_hcache.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/salt_clear_hcache.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/scrapli_netconf_call.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/scrapli_netconf_call.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,24 +121,26 @@
     8. Return results list of dictionaries keyed by step name
 
     Scrapli-netconf implementation lacks of support for commit confirmed operation
     as of creating this module.
     """
     failed = False
     result = []
-    can_validate, can_commit_confirmed, has_candidate_datastore = False, False, False
+    can_validate = False
+    can_commit_confirmed = False  # noqa: F841
+    has_candidate_datastore = False
 
     # get capabilities
     for i in conn.server_capabilities:
         if "urn:ietf:params:netconf:capability:validate" in i:
             can_validate = True
         elif "urn:ietf:params:netconf:capability:candidate" in i:
             has_candidate_datastore = True
         elif "urn:ietf:params:netconf:capability:confirmed-commit" in i:
-            can_commit_confirmed = True
+            can_commit_confirmed = True  # noqa: F841
 
     # decide on target configuration datastore
     kwargs["target"] = kwargs.get(
         "target", "candidate" if has_candidate_datastore else "running"
     )
 
     # run transaction
```

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/scrapli_send_commands.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/scrapli_send_commands.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/scrapli_send_config.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/scrapli_send_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,17 @@
         return Result(
             host=task.host,
             failed=True,
             exception="No nornir_scrapli found, is it installed?",
         )
 
     # get configuration
-    if "commands" in task.host.data.get("__task__", {}):
+    if "config" in task.host.data.get("__task__", {}):
+        config = task.host.data["__task__"]["config"]
+    elif "commands" in task.host.data.get("__task__", {}):
         config = task.host.data["__task__"]["commands"]
     elif "filename" in task.host.data.get("__task__", {}):
         config = task.host.data["__task__"]["filename"]
 
     # transform configuration to string if list/tuple given
     if isinstance(config, (list, tuple)):
         config = "\n".join(config)
```

### Comparing `nornir_salt-0.8.0/nornir_salt/plugins/tasks/tcp_ping.py` & `nornir_salt-0.9.0/nornir_salt/plugins/tasks/tcp_ping.py`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/nornir_salt.egg-info/PKG-INFO` & `nornir_salt-0.9.0/nornir_salt.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nornir-salt
-Version: 0.8.0
+Version: 0.9.0
 Summary: Nornir plugins used with SALTSTACK
 Home-page: https://github.com/dmulyalin/nornir-salt
 Author: Denis Mulyalin
 Author-email: d.mulyalin@gmail.com
 License: UNKNOWN
 Description: [![Downloads](https://pepy.tech/badge/nornir-salt)](https://pepy.tech/project/nornir-salt)
         [![PyPI versions](https://img.shields.io/pypi/pyversions/nornir-salt.svg)](https://pypi.python.org/pypi/nornir-salt/)
@@ -22,11 +22,13 @@
         
         Issues, bug reports and feature requests are welcomed.
         
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `nornir_salt-0.8.0/nornir_salt.egg-info/SOURCES.txt` & `nornir_salt-0.9.0/nornir_salt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nornir_salt-0.8.0/setup.py` & `nornir_salt-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 __author__ = "Denis Mulyalin"
 
 with open("README.md", "r") as f:
     README = f.read()
 
 setuptools.setup(
     name="nornir_salt",
@@ -17,14 +17,16 @@
     url="https://github.com/dmulyalin/nornir-salt",
     packages=setuptools.find_packages(),
     extras_require={},
     classifiers=[
         "Topic :: Utilities",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
     ],
     python_requires=">=3.6",
     install_requires=["nornir==3.*"],
     entry_points="""
     [nornir.plugins.inventory]
```

