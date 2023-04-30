# Comparing `tmp/linuxserver-0.1.1.tar.gz` & `tmp/linuxserver-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linuxserver-0.1.1.tar", last modified: Sun Apr 30 14:44:49 2023, max compression
+gzip compressed data, was "linuxserver-0.1.2.tar", last modified: Sun Apr 30 16:24:34 2023, max compression
```

## Comparing `linuxserver-0.1.1.tar` & `linuxserver-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:44:49.122911 linuxserver-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-30 14:44:39.000000 linuxserver-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-30 14:44:49.122911 linuxserver-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:44:49.122911 linuxserver-0.1.1/linuxserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-30 14:44:48.000000 linuxserver-0.1.1/linuxserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-30 14:44:49.000000 linuxserver-0.1.1/linuxserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 14:44:48.000000 linuxserver-0.1.1/linuxserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-30 14:44:48.000000 linuxserver-0.1.1/linuxserver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-30 14:44:48.000000 linuxserver-0.1.1/linuxserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 14:44:48.000000 linuxserver-0.1.1/linuxserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 14:44:49.122911 linuxserver-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-30 14:44:39.000000 linuxserver-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:44:49.122911 linuxserver-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:44:49.122911 linuxserver-0.1.1/src/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:44:49.122911 linuxserver-0.1.1/src/cli/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/docker/deluge-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/docker/gluetun-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/docker/heimdall-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/docker/jackett-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/docker/plex-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/docker/radarr-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/docker/sonarr-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 14:44:39.000000 linuxserver-0.1.1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:24:34.939962 linuxserver-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-30 16:24:22.000000 linuxserver-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-30 16:24:34.939962 linuxserver-0.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:24:34.939962 linuxserver-0.1.2/linuxserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-30 16:24:34.000000 linuxserver-0.1.2/linuxserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-30 16:24:34.000000 linuxserver-0.1.2/linuxserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 16:24:34.000000 linuxserver-0.1.2/linuxserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-30 16:24:34.000000 linuxserver-0.1.2/linuxserver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-30 16:24:34.000000 linuxserver-0.1.2/linuxserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 16:24:34.000000 linuxserver-0.1.2/linuxserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 16:24:34.939962 linuxserver-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-30 16:24:22.000000 linuxserver-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:24:34.935962 linuxserver-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:24:34.939962 linuxserver-0.1.2/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:24:22.000000 linuxserver-0.1.2/src/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-30 16:24:22.000000 linuxserver-0.1.2/src/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-30 16:24:22.000000 linuxserver-0.1.2/src/cli/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:24:34.939962 linuxserver-0.1.2/src/cli/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-30 16:24:22.000000 linuxserver-0.1.2/src/cli/docker/deluge-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-30 16:24:22.000000 linuxserver-0.1.2/src/cli/docker/gluetun-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-30 16:24:22.000000 linuxserver-0.1.2/src/cli/docker/heimdall-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-30 16:24:22.000000 linuxserver-0.1.2/src/cli/docker/jackett-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-30 16:24:22.000000 linuxserver-0.1.2/src/cli/docker/plex-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-30 16:24:22.000000 linuxserver-0.1.2/src/cli/docker/radarr-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-30 16:24:22.000000 linuxserver-0.1.2/src/cli/docker/sonarr-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 16:24:22.000000 linuxserver-0.1.2/version.py
```

### Comparing `linuxserver-0.1.1/LICENSE` & `linuxserver-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `linuxserver-0.1.1/PKG-INFO` & `linuxserver-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxserver
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple CLI to deploy linuxserver services
 Home-page: https://github.com/foprel/linuxserver
 Author: Frank Oprel
 Author-email: fj.oprel@gmail.com
 License: Copyright (c) 2012-2022 Scott Chacon and others
 
 Permission is hereby granted, free of charge, to any person obtaining
```

### Comparing `linuxserver-0.1.1/linuxserver.egg-info/PKG-INFO` & `linuxserver-0.1.2/linuxserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxserver
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple CLI to deploy linuxserver services
 Home-page: https://github.com/foprel/linuxserver
 Author: Frank Oprel
 Author-email: fj.oprel@gmail.com
 License: Copyright (c) 2012-2022 Scott Chacon and others
 
 Permission is hereby granted, free of charge, to any person obtaining
```

### Comparing `linuxserver-0.1.1/linuxserver.egg-info/SOURCES.txt` & `linuxserver-0.1.2/linuxserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linuxserver-0.1.1/setup.py` & `linuxserver-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `linuxserver-0.1.1/src/cli/cli.py` & `linuxserver-0.1.2/src/cli/cli.py`

 * *Files identical despite different names*

### Comparing `linuxserver-0.1.1/src/cli/config.py` & `linuxserver-0.1.2/src/cli/config.py`

 * *Files identical despite different names*

### Comparing `linuxserver-0.1.1/src/cli/docker/gluetun-compose.yml` & `linuxserver-0.1.2/src/cli/docker/gluetun-compose.yml`

 * *Files identical despite different names*

