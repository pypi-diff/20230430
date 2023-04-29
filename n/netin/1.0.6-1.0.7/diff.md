# Comparing `tmp/netin-1.0.6.tar.gz` & `tmp/netin-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netin-1.0.6.tar", last modified: Sat Apr 29 23:08:40 2023, max compression
+gzip compressed data, was "netin-1.0.7.tar", last modified: Sat Apr 29 23:23:01 2023, max compression
```

## Comparing `netin-1.0.6.tar` & `netin-1.0.7.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/
--rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.6/LICENSE
--rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.6/MANIFEST.in
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3924 2023-04-29 23:08:40.578252 netin-1.0.6/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2654 2023-04-25 12:36:58.000000 netin-1.0.6/README.rst
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.574252 netin-1.0.6/examples/
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.574252 netin-1.0.6/examples/deleteme/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2956 2023-04-24 13:06:53.000000 netin-1.0.6/examples/deleteme/deleteme.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.574252 netin-1.0.6/examples/deleteme/www/
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.574252 netin-1.0.6/examples/deleteme/www/data/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2043 2023-04-25 13:06:23.000000 netin-1.0.6/examples/deleteme/www/data/example.gt.gz
--rw-r--r--   0 espinl    (1001) espinl    (1001)    10988 2023-04-29 20:20:46.000000 netin-1.0.6/examples/deleteme/www/helper.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.574252 netin-1.0.6/examples/directed/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.6/examples/directed/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.6/examples/directed/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.6/examples/directed/dpah.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.574252 netin-1.0.6/examples/undirected/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.6/examples/undirected/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.6/examples/undirected/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.6/examples/undirected/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.6/examples/undirected/patch.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.574252 netin-1.0.6/netin/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      475 2023-04-29 17:53:11.000000 netin-1.0.6/netin/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/netin/algorithms/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-25 16:30:10.000000 netin-1.0.6/netin/algorithms/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/netin/algorithms/sampling/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      280 2023-04-25 16:30:06.000000 netin-1.0.6/netin/algorithms/sampling/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-24 22:21:58.000000 netin-1.0.6/netin/algorithms/sampling/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2814 2023-04-25 10:52:24.000000 netin-1.0.6/netin/algorithms/sampling/degree_group_rank.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2414 2023-04-25 10:52:21.000000 netin-1.0.6/netin/algorithms/sampling/degree_rank.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3963 2023-04-25 10:52:17.000000 netin-1.0.6/netin/algorithms/sampling/partial_crawls.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1901 2023-04-25 10:52:13.000000 netin-1.0.6/netin/algorithms/sampling/random_edges.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2092 2023-04-25 10:52:10.000000 netin-1.0.6/netin/algorithms/sampling/random_neighbor.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1684 2023-04-25 10:52:06.000000 netin-1.0.6/netin/algorithms/sampling/random_nodes.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6171 2023-04-26 21:06:58.000000 netin-1.0.6/netin/algorithms/sampling/sampling.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/netin/generators/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      341 2023-04-29 20:00:50.000000 netin-1.0.6/netin/generators/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5527 2023-04-29 17:51:16.000000 netin-1.0.6/netin/generators/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    13711 2023-04-29 21:01:01.000000 netin-1.0.6/netin/generators/directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3409 2023-04-29 17:52:09.000000 netin-1.0.6/netin/generators/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5394 2023-04-29 17:52:24.000000 netin-1.0.6/netin/generators/dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    30358 2023-04-29 22:06:42.000000 netin-1.0.6/netin/generators/graph.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     8253 2023-04-26 21:06:58.000000 netin-1.0.6/netin/generators/h.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3619 2023-04-26 22:55:17.000000 netin-1.0.6/netin/generators/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     7346 2023-04-29 17:52:46.000000 netin-1.0.6/netin/generators/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     7818 2023-04-29 17:52:51.000000 netin-1.0.6/netin/generators/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6370 2023-04-29 17:51:07.000000 netin-1.0.6/netin/generators/patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     8299 2023-04-23 12:35:51.000000 netin-1.0.6/netin/generators/tc.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/netin/generators/tests/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.6/netin/generators/tests/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.6/netin/generators/tests/test_directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.6/netin/generators/tests/test_dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.6/netin/generators/tests/test_patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.6/netin/generators/tests/test_undirected.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     9519 2023-04-29 19:35:57.000000 netin-1.0.6/netin/generators/undirected.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/netin/stats/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      574 2023-04-26 19:48:59.000000 netin-1.0.6/netin/stats/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5041 2023-04-26 00:35:20.000000 netin-1.0.6/netin/stats/distributions.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5990 2023-04-26 20:37:47.000000 netin-1.0.6/netin/stats/networks.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5682 2023-04-24 10:42:53.000000 netin-1.0.6/netin/stats/ranking.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/netin/utils/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.6/netin/utils/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1447 2023-04-26 18:57:24.000000 netin-1.0.6/netin/utils/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      583 2023-04-25 21:31:19.000000 netin-1.0.6/netin/utils/io.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2323 2023-04-29 19:27:11.000000 netin-1.0.6/netin/utils/validator.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/netin/viz/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      462 2023-04-26 01:14:12.000000 netin-1.0.6/netin/viz/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      493 2023-04-26 01:13:59.000000 netin-1.0.6/netin/viz/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    27663 2023-04-29 21:32:22.000000 netin-1.0.6/netin/viz/handlers.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/netin.egg-info/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3924 2023-04-29 23:08:40.000000 netin-1.0.6/netin.egg-info/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1780 2023-04-29 23:08:40.000000 netin-1.0.6/netin.egg-info/SOURCES.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-29 23:08:40.000000 netin-1.0.6/netin.egg-info/dependency_links.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.6/netin.egg-info/not-zip-safe
--rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-29 23:08:40.000000 netin-1.0.6/netin.egg-info/requires.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-29 23:08:40.000000 netin-1.0.6/netin.egg-info/top_level.txt
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/requirements/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.6/requirements/default.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       60 2023-04-23 06:45:06.000000 netin-1.0.6/requirements/docs.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.6/requirements/test.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-29 23:08:40.582252 netin-1.0.6/setup.cfg
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4291 2023-04-26 19:17:45.000000 netin-1.0.6/setup.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:23:01.750214 netin-1.0.7/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.7/LICENSE
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.7/MANIFEST.in
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3924 2023-04-29 23:23:01.750214 netin-1.0.7/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2654 2023-04-25 12:36:58.000000 netin-1.0.7/README.rst
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:23:01.742214 netin-1.0.7/examples/
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:23:01.746214 netin-1.0.7/examples/deleteme/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2956 2023-04-24 13:06:53.000000 netin-1.0.7/examples/deleteme/deleteme.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:23:01.746214 netin-1.0.7/examples/deleteme/www/
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:23:01.746214 netin-1.0.7/examples/deleteme/www/data/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2043 2023-04-25 13:06:23.000000 netin-1.0.7/examples/deleteme/www/data/example.gt.gz
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    10988 2023-04-29 20:20:46.000000 netin-1.0.7/examples/deleteme/www/helper.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:23:01.746214 netin-1.0.7/examples/directed/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.7/examples/directed/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.7/examples/directed/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.7/examples/directed/dpah.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:23:01.746214 netin-1.0.7/examples/undirected/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.7/examples/undirected/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.7/examples/undirected/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.7/examples/undirected/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.7/examples/undirected/patch.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:23:01.746214 netin-1.0.7/netin/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      475 2023-04-29 23:19:11.000000 netin-1.0.7/netin/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:23:01.746214 netin-1.0.7/netin/algorithms/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-25 16:30:10.000000 netin-1.0.7/netin/algorithms/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:23:01.746214 netin-1.0.7/netin/algorithms/sampling/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      280 2023-04-25 16:30:06.000000 netin-1.0.7/netin/algorithms/sampling/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-24 22:21:58.000000 netin-1.0.7/netin/algorithms/sampling/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2814 2023-04-25 10:52:24.000000 netin-1.0.7/netin/algorithms/sampling/degree_group_rank.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2414 2023-04-25 10:52:21.000000 netin-1.0.7/netin/algorithms/sampling/degree_rank.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3963 2023-04-25 10:52:17.000000 netin-1.0.7/netin/algorithms/sampling/partial_crawls.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1901 2023-04-25 10:52:13.000000 netin-1.0.7/netin/algorithms/sampling/random_edges.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2092 2023-04-25 10:52:10.000000 netin-1.0.7/netin/algorithms/sampling/random_neighbor.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1684 2023-04-25 10:52:06.000000 netin-1.0.7/netin/algorithms/sampling/random_nodes.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6171 2023-04-26 21:06:58.000000 netin-1.0.7/netin/algorithms/sampling/sampling.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:23:01.746214 netin-1.0.7/netin/generators/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      341 2023-04-29 20:00:50.000000 netin-1.0.7/netin/generators/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5527 2023-04-29 17:51:16.000000 netin-1.0.7/netin/generators/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    13711 2023-04-29 21:01:01.000000 netin-1.0.7/netin/generators/directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3409 2023-04-29 17:52:09.000000 netin-1.0.7/netin/generators/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5394 2023-04-29 17:52:24.000000 netin-1.0.7/netin/generators/dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    30358 2023-04-29 22:06:42.000000 netin-1.0.7/netin/generators/graph.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8253 2023-04-26 21:06:58.000000 netin-1.0.7/netin/generators/h.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3619 2023-04-26 22:55:17.000000 netin-1.0.7/netin/generators/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     7346 2023-04-29 17:52:46.000000 netin-1.0.7/netin/generators/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     7818 2023-04-29 17:52:51.000000 netin-1.0.7/netin/generators/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6370 2023-04-29 17:51:07.000000 netin-1.0.7/netin/generators/patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8299 2023-04-23 12:35:51.000000 netin-1.0.7/netin/generators/tc.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:23:01.746214 netin-1.0.7/netin/generators/tests/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.7/netin/generators/tests/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.7/netin/generators/tests/test_directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.7/netin/generators/tests/test_dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.7/netin/generators/tests/test_patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.7/netin/generators/tests/test_undirected.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     9519 2023-04-29 19:35:57.000000 netin-1.0.7/netin/generators/undirected.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:23:01.746214 netin-1.0.7/netin/stats/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      574 2023-04-26 19:48:59.000000 netin-1.0.7/netin/stats/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5041 2023-04-26 00:35:20.000000 netin-1.0.7/netin/stats/distributions.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5990 2023-04-26 20:37:47.000000 netin-1.0.7/netin/stats/networks.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5683 2023-04-29 23:17:54.000000 netin-1.0.7/netin/stats/ranking.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:23:01.750214 netin-1.0.7/netin/utils/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.7/netin/utils/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1447 2023-04-26 18:57:24.000000 netin-1.0.7/netin/utils/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      583 2023-04-25 21:31:19.000000 netin-1.0.7/netin/utils/io.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2323 2023-04-29 19:27:11.000000 netin-1.0.7/netin/utils/validator.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:23:01.750214 netin-1.0.7/netin/viz/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      462 2023-04-26 01:14:12.000000 netin-1.0.7/netin/viz/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      493 2023-04-26 01:13:59.000000 netin-1.0.7/netin/viz/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    27663 2023-04-29 21:32:22.000000 netin-1.0.7/netin/viz/handlers.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:23:01.746214 netin-1.0.7/netin.egg-info/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3924 2023-04-29 23:23:01.000000 netin-1.0.7/netin.egg-info/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1780 2023-04-29 23:23:01.000000 netin-1.0.7/netin.egg-info/SOURCES.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-29 23:23:01.000000 netin-1.0.7/netin.egg-info/dependency_links.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.7/netin.egg-info/not-zip-safe
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-29 23:23:01.000000 netin-1.0.7/netin.egg-info/requires.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-29 23:23:01.000000 netin-1.0.7/netin.egg-info/top_level.txt
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:23:01.750214 netin-1.0.7/requirements/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.7/requirements/default.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       60 2023-04-23 06:45:06.000000 netin-1.0.7/requirements/docs.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.7/requirements/test.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-29 23:23:01.750214 netin-1.0.7/setup.cfg
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4291 2023-04-26 19:17:45.000000 netin-1.0.7/setup.py
```

### Comparing `netin-1.0.6/LICENSE` & `netin-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/PKG-INFO` & `netin-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.6/README.rst` & `netin-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/examples/deleteme/deleteme.py` & `netin-1.0.7/examples/deleteme/deleteme.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/examples/deleteme/www/data/example.gt.gz` & `netin-1.0.7/examples/deleteme/www/data/example.gt.gz`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/examples/deleteme/www/helper.py` & `netin-1.0.7/examples/deleteme/www/helper.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/algorithms/sampling/degree_group_rank.py` & `netin-1.0.7/netin/algorithms/sampling/degree_group_rank.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/algorithms/sampling/degree_rank.py` & `netin-1.0.7/netin/algorithms/sampling/degree_rank.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/algorithms/sampling/partial_crawls.py` & `netin-1.0.7/netin/algorithms/sampling/partial_crawls.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/algorithms/sampling/random_edges.py` & `netin-1.0.7/netin/algorithms/sampling/random_edges.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/algorithms/sampling/random_neighbor.py` & `netin-1.0.7/netin/algorithms/sampling/random_neighbor.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/algorithms/sampling/random_nodes.py` & `netin-1.0.7/netin/algorithms/sampling/random_nodes.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/algorithms/sampling/sampling.py` & `netin-1.0.7/netin/algorithms/sampling/sampling.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/generators/dh.py` & `netin-1.0.7/netin/generators/dh.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/generators/directed.py` & `netin-1.0.7/netin/generators/directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/generators/dpa.py` & `netin-1.0.7/netin/generators/dpa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/generators/dpah.py` & `netin-1.0.7/netin/generators/dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/generators/graph.py` & `netin-1.0.7/netin/generators/graph.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/generators/h.py` & `netin-1.0.7/netin/generators/h.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/generators/pa.py` & `netin-1.0.7/netin/generators/pa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/generators/pah.py` & `netin-1.0.7/netin/generators/pah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/generators/patc.py` & `netin-1.0.7/netin/generators/patc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/generators/patch.py` & `netin-1.0.7/netin/generators/patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/generators/tc.py` & `netin-1.0.7/netin/generators/tc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/generators/tests/test_directed.py` & `netin-1.0.7/netin/generators/tests/test_directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/generators/tests/test_dpah.py` & `netin-1.0.7/netin/generators/tests/test_dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/generators/tests/test_patch.py` & `netin-1.0.7/netin/generators/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/generators/tests/test_undirected.py` & `netin-1.0.7/netin/generators/tests/test_undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/generators/undirected.py` & `netin-1.0.7/netin/generators/undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/stats/__init__.py` & `netin-1.0.7/netin/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/stats/distributions.py` & `netin-1.0.7/netin/stats/distributions.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/stats/networks.py` & `netin-1.0.7/netin/stats/networks.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/stats/ranking.py` & `netin-1.0.7/netin/stats/ranking.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         The y values (Gini coefficients in each top-k rank).
 
     Returns
     -------
     float
         The Gini coefficient of the entire distribution (at op-100%).
     """
-    gini_global = ys[0]  # top-100%
+    gini_global = ys[-1]  # top-100%
     return gini_global
 
 
 def get_ranking_inequality_class(gini_global: float, cuts: Set[float] = const.INEQUALITY_CUTS) -> str:
     """
     Infers the inequality class label given the Gini coefficient of the entire distribution.
```

### Comparing `netin-1.0.6/netin/utils/constants.py` & `netin-1.0.7/netin/utils/constants.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/utils/io.py` & `netin-1.0.7/netin/utils/io.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/utils/validator.py` & `netin-1.0.7/netin/utils/validator.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin/viz/handlers.py` & `netin-1.0.7/netin/viz/handlers.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/netin.egg-info/PKG-INFO` & `netin-1.0.7/netin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.6/netin.egg-info/SOURCES.txt` & `netin-1.0.7/netin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netin-1.0.6/setup.py` & `netin-1.0.7/setup.py`

 * *Files identical despite different names*

