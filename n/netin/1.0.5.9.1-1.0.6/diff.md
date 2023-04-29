# Comparing `tmp/netin-1.0.5.9.1.tar.gz` & `tmp/netin-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netin-1.0.5.9.1.tar", last modified: Wed Apr 26 22:57:57 2023, max compression
+gzip compressed data, was "netin-1.0.6.tar", last modified: Sat Apr 29 23:08:40 2023, max compression
```

## Comparing `netin-1.0.5.9.1.tar` & `netin-1.0.6.tar`

### file list

```diff
@@ -1,78 +1,82 @@
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/
--rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.9.1/LICENSE
--rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.9.1/MANIFEST.in
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3928 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2654 2023-04-25 12:36:58.000000 netin-1.0.5.9.1/README.rst
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.674023 netin-1.0.5.9.1/examples/
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.674023 netin-1.0.5.9.1/examples/directed/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.9.1/examples/directed/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.9.1/examples/directed/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.9.1/examples/directed/dpah.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.674023 netin-1.0.5.9.1/examples/notebooks/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2956 2023-04-24 13:06:53.000000 netin-1.0.5.9.1/examples/notebooks/deleteme.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.674023 netin-1.0.5.9.1/examples/undirected/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.9.1/examples/undirected/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.9.1/examples/undirected/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.9.1/examples/undirected/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.9.1/examples/undirected/patch.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.674023 netin-1.0.5.9.1/netin/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      479 2023-04-26 22:56:37.000000 netin-1.0.5.9.1/netin/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.674023 netin-1.0.5.9.1/netin/algorithms/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-25 16:30:10.000000 netin-1.0.5.9.1/netin/algorithms/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/netin/algorithms/sampling/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      280 2023-04-25 16:30:06.000000 netin-1.0.5.9.1/netin/algorithms/sampling/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-24 22:21:58.000000 netin-1.0.5.9.1/netin/algorithms/sampling/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2814 2023-04-25 10:52:24.000000 netin-1.0.5.9.1/netin/algorithms/sampling/degree_group_rank.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2414 2023-04-25 10:52:21.000000 netin-1.0.5.9.1/netin/algorithms/sampling/degree_rank.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3963 2023-04-25 10:52:17.000000 netin-1.0.5.9.1/netin/algorithms/sampling/partial_crawls.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1901 2023-04-25 10:52:13.000000 netin-1.0.5.9.1/netin/algorithms/sampling/random_edges.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2092 2023-04-25 10:52:10.000000 netin-1.0.5.9.1/netin/algorithms/sampling/random_neighbor.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1684 2023-04-25 10:52:06.000000 netin-1.0.5.9.1/netin/algorithms/sampling/random_nodes.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6171 2023-04-26 21:06:58.000000 netin-1.0.5.9.1/netin/algorithms/sampling/sampling.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/netin/generators/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      524 2023-04-26 20:32:15.000000 netin-1.0.5.9.1/netin/generators/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5521 2023-04-24 18:03:30.000000 netin-1.0.5.9.1/netin/generators/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    14272 2023-04-26 19:47:38.000000 netin-1.0.5.9.1/netin/generators/directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3434 2023-04-26 19:47:38.000000 netin-1.0.5.9.1/netin/generators/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5388 2023-04-26 19:47:38.000000 netin-1.0.5.9.1/netin/generators/dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    29353 2023-04-26 22:52:24.000000 netin-1.0.5.9.1/netin/generators/graph.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     8253 2023-04-26 21:06:58.000000 netin-1.0.5.9.1/netin/generators/h.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3619 2023-04-26 22:55:17.000000 netin-1.0.5.9.1/netin/generators/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     7340 2023-04-26 22:55:39.000000 netin-1.0.5.9.1/netin/generators/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     7812 2023-04-26 22:56:19.000000 netin-1.0.5.9.1/netin/generators/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6216 2023-04-26 19:47:38.000000 netin-1.0.5.9.1/netin/generators/patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     8299 2023-04-23 12:35:51.000000 netin-1.0.5.9.1/netin/generators/tc.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/netin/generators/tests/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.9.1/netin/generators/tests/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.9.1/netin/generators/tests/test_directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.9.1/netin/generators/tests/test_dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.9.1/netin/generators/tests/test_patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.9.1/netin/generators/tests/test_undirected.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     9948 2023-04-26 20:38:34.000000 netin-1.0.5.9.1/netin/generators/undirected.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/netin/stats/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      574 2023-04-26 19:48:59.000000 netin-1.0.5.9.1/netin/stats/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5041 2023-04-26 00:35:20.000000 netin-1.0.5.9.1/netin/stats/distributions.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5990 2023-04-26 20:37:47.000000 netin-1.0.5.9.1/netin/stats/networks.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5682 2023-04-24 10:42:53.000000 netin-1.0.5.9.1/netin/stats/ranking.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/netin/utils/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.9.1/netin/utils/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1447 2023-04-26 18:57:24.000000 netin-1.0.5.9.1/netin/utils/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      583 2023-04-25 21:31:19.000000 netin-1.0.5.9.1/netin/utils/io.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2184 2023-04-25 17:56:25.000000 netin-1.0.5.9.1/netin/utils/validator.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/netin/viz/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      462 2023-04-26 01:14:12.000000 netin-1.0.5.9.1/netin/viz/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      493 2023-04-26 01:13:59.000000 netin-1.0.5.9.1/netin/viz/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    27317 2023-04-26 22:50:16.000000 netin-1.0.5.9.1/netin/viz/handlers.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.674023 netin-1.0.5.9.1/netin.egg-info/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3928 2023-04-26 22:57:57.000000 netin-1.0.5.9.1/netin.egg-info/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1708 2023-04-26 22:57:57.000000 netin-1.0.5.9.1/netin.egg-info/SOURCES.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-26 22:57:57.000000 netin-1.0.5.9.1/netin.egg-info/dependency_links.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.9.1/netin.egg-info/not-zip-safe
--rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-26 22:57:57.000000 netin-1.0.5.9.1/netin.egg-info/requires.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-26 22:57:57.000000 netin-1.0.5.9.1/netin.egg-info/top_level.txt
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/requirements/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.9.1/requirements/default.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       60 2023-04-23 06:45:06.000000 netin-1.0.5.9.1/requirements/docs.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.9.1/requirements/test.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/setup.cfg
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4291 2023-04-26 19:17:45.000000 netin-1.0.5.9.1/setup.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.6/LICENSE
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.6/MANIFEST.in
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3924 2023-04-29 23:08:40.578252 netin-1.0.6/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2654 2023-04-25 12:36:58.000000 netin-1.0.6/README.rst
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.574252 netin-1.0.6/examples/
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.574252 netin-1.0.6/examples/deleteme/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2956 2023-04-24 13:06:53.000000 netin-1.0.6/examples/deleteme/deleteme.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.574252 netin-1.0.6/examples/deleteme/www/
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.574252 netin-1.0.6/examples/deleteme/www/data/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2043 2023-04-25 13:06:23.000000 netin-1.0.6/examples/deleteme/www/data/example.gt.gz
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    10988 2023-04-29 20:20:46.000000 netin-1.0.6/examples/deleteme/www/helper.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.574252 netin-1.0.6/examples/directed/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.6/examples/directed/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.6/examples/directed/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.6/examples/directed/dpah.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.574252 netin-1.0.6/examples/undirected/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.6/examples/undirected/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.6/examples/undirected/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.6/examples/undirected/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.6/examples/undirected/patch.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.574252 netin-1.0.6/netin/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      475 2023-04-29 17:53:11.000000 netin-1.0.6/netin/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/netin/algorithms/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-25 16:30:10.000000 netin-1.0.6/netin/algorithms/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/netin/algorithms/sampling/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      280 2023-04-25 16:30:06.000000 netin-1.0.6/netin/algorithms/sampling/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-24 22:21:58.000000 netin-1.0.6/netin/algorithms/sampling/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2814 2023-04-25 10:52:24.000000 netin-1.0.6/netin/algorithms/sampling/degree_group_rank.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2414 2023-04-25 10:52:21.000000 netin-1.0.6/netin/algorithms/sampling/degree_rank.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3963 2023-04-25 10:52:17.000000 netin-1.0.6/netin/algorithms/sampling/partial_crawls.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1901 2023-04-25 10:52:13.000000 netin-1.0.6/netin/algorithms/sampling/random_edges.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2092 2023-04-25 10:52:10.000000 netin-1.0.6/netin/algorithms/sampling/random_neighbor.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1684 2023-04-25 10:52:06.000000 netin-1.0.6/netin/algorithms/sampling/random_nodes.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6171 2023-04-26 21:06:58.000000 netin-1.0.6/netin/algorithms/sampling/sampling.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/netin/generators/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      341 2023-04-29 20:00:50.000000 netin-1.0.6/netin/generators/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5527 2023-04-29 17:51:16.000000 netin-1.0.6/netin/generators/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    13711 2023-04-29 21:01:01.000000 netin-1.0.6/netin/generators/directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3409 2023-04-29 17:52:09.000000 netin-1.0.6/netin/generators/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5394 2023-04-29 17:52:24.000000 netin-1.0.6/netin/generators/dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    30358 2023-04-29 22:06:42.000000 netin-1.0.6/netin/generators/graph.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8253 2023-04-26 21:06:58.000000 netin-1.0.6/netin/generators/h.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3619 2023-04-26 22:55:17.000000 netin-1.0.6/netin/generators/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     7346 2023-04-29 17:52:46.000000 netin-1.0.6/netin/generators/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     7818 2023-04-29 17:52:51.000000 netin-1.0.6/netin/generators/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6370 2023-04-29 17:51:07.000000 netin-1.0.6/netin/generators/patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8299 2023-04-23 12:35:51.000000 netin-1.0.6/netin/generators/tc.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/netin/generators/tests/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.6/netin/generators/tests/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.6/netin/generators/tests/test_directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.6/netin/generators/tests/test_dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.6/netin/generators/tests/test_patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.6/netin/generators/tests/test_undirected.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     9519 2023-04-29 19:35:57.000000 netin-1.0.6/netin/generators/undirected.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/netin/stats/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      574 2023-04-26 19:48:59.000000 netin-1.0.6/netin/stats/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5041 2023-04-26 00:35:20.000000 netin-1.0.6/netin/stats/distributions.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5990 2023-04-26 20:37:47.000000 netin-1.0.6/netin/stats/networks.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5682 2023-04-24 10:42:53.000000 netin-1.0.6/netin/stats/ranking.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/netin/utils/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.6/netin/utils/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1447 2023-04-26 18:57:24.000000 netin-1.0.6/netin/utils/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      583 2023-04-25 21:31:19.000000 netin-1.0.6/netin/utils/io.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2323 2023-04-29 19:27:11.000000 netin-1.0.6/netin/utils/validator.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/netin/viz/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      462 2023-04-26 01:14:12.000000 netin-1.0.6/netin/viz/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      493 2023-04-26 01:13:59.000000 netin-1.0.6/netin/viz/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    27663 2023-04-29 21:32:22.000000 netin-1.0.6/netin/viz/handlers.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/netin.egg-info/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3924 2023-04-29 23:08:40.000000 netin-1.0.6/netin.egg-info/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1780 2023-04-29 23:08:40.000000 netin-1.0.6/netin.egg-info/SOURCES.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-29 23:08:40.000000 netin-1.0.6/netin.egg-info/dependency_links.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.6/netin.egg-info/not-zip-safe
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-29 23:08:40.000000 netin-1.0.6/netin.egg-info/requires.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-29 23:08:40.000000 netin-1.0.6/netin.egg-info/top_level.txt
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-29 23:08:40.578252 netin-1.0.6/requirements/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.6/requirements/default.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       60 2023-04-23 06:45:06.000000 netin-1.0.6/requirements/docs.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.6/requirements/test.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-29 23:08:40.582252 netin-1.0.6/setup.cfg
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4291 2023-04-26 19:17:45.000000 netin-1.0.6/setup.py
```

### Comparing `netin-1.0.5.9.1/LICENSE` & `netin-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/PKG-INFO` & `netin-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.9.1
+Version: 1.0.6
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.5.9.1/README.rst` & `netin-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/examples/notebooks/deleteme.py` & `netin-1.0.6/examples/deleteme/deleteme.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/algorithms/sampling/degree_group_rank.py` & `netin-1.0.6/netin/algorithms/sampling/degree_group_rank.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/algorithms/sampling/degree_rank.py` & `netin-1.0.6/netin/algorithms/sampling/degree_rank.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/algorithms/sampling/partial_crawls.py` & `netin-1.0.6/netin/algorithms/sampling/partial_crawls.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/algorithms/sampling/random_edges.py` & `netin-1.0.6/netin/algorithms/sampling/random_edges.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/algorithms/sampling/random_neighbor.py` & `netin-1.0.6/netin/algorithms/sampling/random_neighbor.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/algorithms/sampling/random_nodes.py` & `netin-1.0.6/netin/algorithms/sampling/random_nodes.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/algorithms/sampling/sampling.py` & `netin-1.0.6/netin/algorithms/sampling/sampling.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/generators/dh.py` & `netin-1.0.6/netin/generators/dh.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         homophily within minority group (minimum=0, maximum=1)
 
     seed: object
         seed for random number generator
 
     Notes
     -----
-    The initialization is a directed with n nodes and no edges.
+    The initialization is a directed graph with n nodes and no edges.
     Source nodes are selected based on their activity given by plo_M (if majority) or plo_m (if minority).
     Target nodes are selected via homophily, see [Espin-Noboa2022]_.
     """
 
     ############################################################
     # Constructor
     ############################################################
```

### Comparing `netin-1.0.5.9.1/netin/generators/directed.py` & `netin-1.0.6/netin/generators/directed.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         activity (out-degree power law exponent) minority group (minimum=1)
 
     seed: object
         seed for random number generator
 
     Notes
     -----
-    The initialization is a directed with n nodes and no edges.
+    The initialization is a directed graph with n nodes and no edges.
     Source nodes are selected based on their activity given by plo_M (if majority) or plo_m (if minority).
     Target nodes are selected depending on the chosen mechanism of edge formation.
 
     - DPAH: preferential attachment (in-degree) and homophily (h**), see :class:`netin.DPAH`
     - DPA: preferential attachment (in-degree), see :class:`netin.DPA`
     - DH: homophily (h**), see :class:`netin.DH`
 
@@ -172,20 +172,28 @@
         kwargs: dict
             additional parameters
 
         Returns
         -------
         Union[None, int]
             target node
+
+        Notes
+        -----
+        The target node must have out_degree > 0 (the older the node in the network, the more likely to get more links)
         """
         one_percent = self.n * 1 / 100.
         if np.count_nonzero(self.out_degrees) > one_percent:
-            targets = [n for n in np.arange(self.n) if n not in edge_list[source]]
+            # if there are enough edges, then select only nodes with out_degree > 0 that are not already
+            # connected to the source.
+            # Having out_degree > 0 means they are nodes that have been in the network for at least one time step
+            targets = [n for n in np.arange(self.n) if n not in edge_list[source] and self.out_degrees[n] > 0]
         else:
-            targets = np.arange(self.n)
+            # if there are no enough edges, then select all nodes that are not already connected to the source.
+            targets = [n for n in np.arange(self.n) if n not in edge_list[source]]
         targets = np.delete(targets, np.where(targets == source))
 
         if targets.shape[0] == 0:
             return None
 
         probs = self.get_target_probabilities(source, targets, **kwargs)
         return np.random.choice(a=targets, size=1, replace=False, p=probs)[0]
@@ -260,15 +268,15 @@
         Returns the power law exponents for the in-degree distribution of the majority and minority class.
 
         Returns
         -------
         Tuple[float, float]
             power law exponents for the in-degree distribution of the majority and minority class
         """
-        pl_M, pl_m = calculate_in_degree_powerlaw_exponents(self)
+        pl_M, pl_m = self.calculate_powerlaw_exponents(metric='in_degree')
 
         # fit_M, fit_m = self.fit_powerlaw(metric='in_degree')
         # pl_M = fit_M.power_law.alpha
         # pl_m = fit_m.power_law.alpha
 
         return pl_M, pl_m
 
@@ -277,15 +285,15 @@
         Returns the power law exponents for the out-degree distribution of the majority and minority class.
 
         Returns
         -------
         Tuple[float, float]
             power law exponents for the out-degree distribution of the majority and minority class
         """
-        pl_M, pl_m = calculate_out_degree_powerlaw_exponents(self)
+        pl_M, pl_m = self.calculate_powerlaw_exponents(metric='out_degree')
 
         # fit_M, fit_m = self.fit_powerlaw(metric='out_degree')
         # pl_M = fit_M.power_law.alpha
         # pl_m = fit_m.power_law.alpha
 
         return pl_M, pl_m
 
@@ -358,46 +366,7 @@
                              d=self.d,
                              f_m=self.f_m,
                              plo_M=self.plo_M,
                              plo_m=self.plo_m,
                              seed=self.seed)
         return obj
 
-
-def calculate_in_degree_powerlaw_exponents(g: DiGraph) -> Tuple[float, float]:
-    """
-    Returns the power law exponents for the in-degree distribution of the majority and minority class.
-
-    Parameters
-    ----------
-    g: DiGraph
-        Graph to calculate the power law exponents for
-
-    Returns
-    -------
-    Tuple[float, float]
-        power law exponents for the in-degree distribution of the majority and minority class
-    """
-    fit_M, fit_m = g.fit_powerlaw(metric='in_degree')
-    pl_M = fit_M.power_law.alpha
-    pl_m = fit_m.power_law.alpha
-    return pl_M, pl_m
-
-
-def calculate_out_degree_powerlaw_exponents(g: DiGraph) -> Tuple[float, float]:
-    """
-    Returns the power law exponents for the out-degree distribution of the majority and minority class.
-
-    Parameters
-    ----------
-    g: DiGraph
-        Graph to calculate the power law exponents for
-
-    Returns
-    -------
-    Tuple[float, float]
-        power law exponents for the out-degree distribution of the majority and minority class
-    """
-    fit_M, fit_m = g.fit_powerlaw(metric='out_degree')
-    pl_M = fit_M.power_law.alpha
-    pl_m = fit_m.power_law.alpha
-    return pl_M, pl_m
```

### Comparing `netin-1.0.5.9.1/netin/generators/dpa.py` & `netin-1.0.6/netin/generators/dpa.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,20 +27,17 @@
         activity (out-degree power law exponent) minority group (minimum=1)
 
     seed: object
         seed for random number generator
 
     Notes
     -----
-    The initialization is a directed with n nodes and no edges.
-    Source nodes are selected based on their activity given by plo_M (if majority) or plo_m (if minority) [Espin-Noboa2022]_.
-    Target nodes are selected via preferential attachment [BarabasiAlbert1999]_.
-
-    References
-    ----------
+    The initialization is a directed graph with n nodes and no edges.
+    Source nodes are selected based on their activity given by plo_M (if majority) or plo_m (if minority)
+    [Espin-Noboa2022]_. Target nodes are selected via preferential attachment [BarabasiAlbert1999]_.
 
     """
 
     ############################################################
     # Constructor
     ############################################################
```

### Comparing `netin-1.0.5.9.1/netin/generators/dpah.py` & `netin-1.0.6/netin/generators/dpah.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         homophily within minority group (minimum=0, maximum=1)
 
     seed: object
         seed for random number generator
 
     Notes
     -----
-    The initialization is a directed with n nodes where f_m are the minority.
+    The initialization is a directed graph with n nodes where f_m are the minority.
     Source nodes are selected based on their activity given by plo_M (if majority) or plo_m (if minority).
     Target nodes are selected via preferential attachment (in-degree) an homophily (h**).
     This model is based on [Espin-Noboa2022]_ which is the directed version of the "BA Homophily" model [Karimi2018]_.
     """
 
     ############################################################
     # Constructor
```

### Comparing `netin-1.0.5.9.1/netin/generators/graph.py` & `netin-1.0.6/netin/generators/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Parameters
     ----------
     n: int
         number of nodes (minimum=2)
 
     f_m: float
         fraction of minorities (minimum=1/n, maximum=(n-1)/n)
-
+cu
     seed: object
         seed for random number generator
 
     Notes
     -----
     The initialization is a graph with n nodes and fraction of minority f_m.
     Source nodes are selected one-by-one (if undirected) and based on their activity (if directed).
@@ -678,14 +678,40 @@
         # dm = [d for n, d in dist_fnc if self.nodes[n][self.class_attribute] != vM]
         #
         # fit_M = powerlaw.Fit(data=dM, discrete=True, xmin=min(dM), xmax=max(dM), verbose=False)
         # fit_m = powerlaw.Fit(data=dm, discrete=True, xmin=min(dm), xmax=max(dm), verbose=False)
 
         return fit_M, fit_m
 
+    def calculate_powerlaw_exponents(self, metric: str) -> Tuple[float, float]:
+        """
+        Returns the power law exponents for the ``metric`` distribution of the majority and minority class.
+
+        Parameters
+        ----------
+        metric: str
+            Metric to calculate the power law exponents for.
+
+        Returns
+        -------
+        Tuple[float, float]
+            power law exponents for the ``metric`` distribution of the majority and minority class
+
+        Raises
+        ------
+            ValueError: Value of ``metric`` ∈ ['in_degree', 'out_degree'] if the graph is directed,
+            otherwise it must be 'degree'.
+        """
+        metrics = ['in_degree', 'out_degree'] if self.is_directed() else ['degree']
+        val.validate_values(metric, metrics)
+        fit_M, fit_m = self.fit_powerlaw(metric=metric)
+        pl_M = fit_M.power_law.alpha
+        pl_m = fit_m.power_law.alpha
+        return pl_M, pl_m
+
     ############################################################
     # Metadata
     ############################################################
 
     def compute_node_stats(self, metric: str, **kwargs) -> List[Union[int, float]]:
         """
         Returns the property of each node in the graph based on the metric.
@@ -813,14 +839,16 @@
         netin.Graph
             copy of the current object
         """
         g = self._makecopy()
         g._init_graph(class_attribute=self.class_attribute,
                       class_values=self.class_values,
                       class_labels=self.class_labels)
+        g.set_model_name(self.get_model_name())
+
         g.graph.update(self.graph)
         g.add_nodes_from((n, d.copy()) for n, d in self._node.items())
         g.add_edges_from(
             (u, v, datadict.copy())
             for u, nbrs in self._adj.items()
             for v, datadict in nbrs.items()
         )
```

### Comparing `netin-1.0.5.9.1/netin/generators/h.py` & `netin-1.0.6/netin/generators/h.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/generators/pa.py` & `netin-1.0.6/netin/generators/pa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/generators/pah.py` & `netin-1.0.6/netin/generators/pah.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         homophily (similarity) between minority nodes (minimum=0, maximum=1.)
 
     seed: object
         seed for random number generator
 
     Notes
     -----
-    The initialization is an undirected with n nodes, where f_m are the minority.
+    The initialization is an undirected graph with n nodes, where f_m are the minority.
     Then, everytime a node is selected as source, it gets connected to k target nodes.
     Target nodes are selected via preferential attachment (in-degree) and homophily (h_**).
     This model is based on [Karimi2018]_ known as the "Barabasi model with homophily" or "BA Homophily".
     """
 
     ############################################################
     # Constructor
```

### Comparing `netin-1.0.5.9.1/netin/generators/patc.py` & `netin-1.0.6/netin/generators/patc.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         probability of a new edge to close a triad (minimum=0, maximum=1.)
 
     seed: object
         seed for random number generator
 
     Notes
     -----
-    The initialization is an undirected with n nodes and no edges.
+    The initialization is an undirected graph with n nodes and no edges.
     Then, everytime a node is selected as source, it gets connected to k target nodes.
     Target nodes are selected via preferential attachment `in-degree` [BarabasiAlbert1999]_, or
     triadic closure `tc` [HolmeKim2002]_.
     """
 
     ############################################################
     # Constructor
```

### Comparing `netin-1.0.5.9.1/netin/generators/patch.py` & `netin-1.0.6/netin/generators/patch.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,19 +28,21 @@
         homophily (similarity) between minority nodes (minimum=0, maximum=1.)
 
     tc: float
         probability of a new edge to close a triad (minimum=0, maximum=1.)
 
     Notes
     -----
-    The initialization is an undirected with n nodes and no edges.
+    The initialization is an undirected graph with n nodes and no edges.
     Then, everytime a node is selected as source, it gets connected to k target nodes.
-    Target nodes are selected via preferential attachment (in-degree) [BarabasiAlbert1999]_,
-    homophily (h_**; see :class:`netin.Homophily`) [Karimi2018]_,
-    and triadic closure (see :class:`netin.TriadicClosure`) [HolmeKim2002]_.
+    Target nodes are selected via preferential attachment (in-degree) [BarabasiAlbert1999]_ and
+    homophily (h_**; see :class:`netin.Homophily`) [Karimi2018]_ with probability ``1-p_{TC}``,
+    and with probability ``p_{TC}`` via triadic closure (see :class:`netin.TriadicClosure`) [HolmeKim2002]_.
+
+    Note that this model is still work in progress and not fully implemented yet.
     """
 
     ############################################################
     # Constructor
     ############################################################
 
     def __init__(self, n: int, k: int, f_m: float, h_mm: float, h_MM: float, tc: float, seed: object = None):
```

### Comparing `netin-1.0.5.9.1/netin/generators/tc.py` & `netin-1.0.6/netin/generators/tc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/generators/tests/test_directed.py` & `netin-1.0.6/netin/generators/tests/test_directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/generators/tests/test_dpah.py` & `netin-1.0.6/netin/generators/tests/test_dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/generators/tests/test_patch.py` & `netin-1.0.6/netin/generators/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/generators/tests/test_undirected.py` & `netin-1.0.6/netin/generators/tests/test_undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/generators/undirected.py` & `netin-1.0.6/netin/generators/undirected.py`

 * *Files 4% similar despite different names*

```diff
@@ -209,63 +209,47 @@
         -------
         fit_M : powerlaw.Fit
             Powerlaw fit for the majority class
 
         fit_m: powerlaw.Fit
             Powerlaw fit for the minority class
         """
-        vM = self.get_majority_value()
-        dM = [d for n, d in self.degree() if self.nodes[n][self.class_attribute] == vM]
-        dm = [d for n, d in self.degree() if self.nodes[n][self.class_attribute] != vM]
+        fit_M, fit_m = self.fit_powerlaw(metric='degree')
+
+        # vM = self.get_majority_value()
+        # dM = [d for n, d in self.degree() if self.nodes[n][self.class_attribute] == vM]
+        # dm = [d for n, d in self.degree() if self.nodes[n][self.class_attribute] != vM]
+        #
+        # fit_M = powerlaw.Fit(data=dM, discrete=True, xmin=min(dM), xmax=max(dM))
+        # fit_m = powerlaw.Fit(data=dm, discrete=True, xmin=min(dm), xmax=max(dm))
 
-        fit_M = powerlaw.Fit(data=dM, discrete=True, xmin=min(dM), xmax=max(dM))
-        fit_m = powerlaw.Fit(data=dm, discrete=True, xmin=min(dm), xmax=max(dm))
         return fit_M, fit_m
 
     def calculate_degree_powerlaw_exponents(self) -> Tuple[float, float]:
         """
         Returns the powerlaw exponents for the majority and minority class.
 
         Returns
         -------
         pl_M : float
             Powerlaw exponent for the majority class
 
         pl_m: float
             Powerlaw exponent for the minority class
         """
-        pl_M, pl_m = calculate_degree_powerlaw_exponents(self)
+        pl_M, pl_m = self.calculate_powerlaw_exponents(metric='degree')
 
+        # pl_M, pl_m = calculate_degree_powerlaw_exponents(self)
         # fit_M, fit_m = self.fit_degree_powerlaw()
         # pl_M = fit_M.power_law.alpha
         # pl_m = fit_m.power_law.alpha
 
         return pl_M, pl_m
 
     def _makecopy(self):
         """
         Makes a copy of the current object.
         """
         return self.__class__(n=self.n,
                               k=self.k,
                               f_m=self.f_m,
                               seed=self.seed)
-
-
-def calculate_degree_powerlaw_exponents(g: UnDiGraph) -> Tuple[float, float]:
-    """
-    Returns the power law exponents for the in-degree distribution of the majority and minority class.
-
-    Parameters
-    ----------
-    g: DiGraph
-        Graph to calculate the power law exponents for
-
-    Returns
-    -------
-    Tuple[float, float]
-        power law exponents for the in-degree distribution of the majority and minority class
-    """
-    fit_M, fit_m = g.fit_powerlaw(metric='degree')
-    pl_M = fit_M.power_law.alpha
-    pl_m = fit_m.power_law.alpha
-    return pl_M, pl_m
```

### Comparing `netin-1.0.5.9.1/netin/stats/__init__.py` & `netin-1.0.6/netin/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/stats/distributions.py` & `netin-1.0.6/netin/stats/distributions.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/stats/networks.py` & `netin-1.0.6/netin/stats/networks.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/stats/ranking.py` & `netin-1.0.6/netin/stats/ranking.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/utils/constants.py` & `netin-1.0.6/netin/utils/constants.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/utils/io.py` & `netin-1.0.6/netin/utils/io.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9.1/netin/utils/validator.py` & `netin-1.0.6/netin/utils/validator.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,19 @@
         raise TypeError('value must be a float')
     if minimum in const.EMPTY and maximum in const.EMPTY:
         raise ValueError('At least one of minimum or maximum must be specified')
     if value < minimum or (maximum is not None and value > maximum):
         raise ValueError(f'Value is out of range.')
 
 
+def validate_values(value: object, values: list):
+    if value not in values:
+        raise ValueError(f'Value must be one of {values}')
+
+
 def calibrate_null_probabilities(p: float) -> float:
     return const.EPSILON if p == 0 else 1 - const.EPSILON if p == 1 else p
 
 
 def validate_graph_metadata(g: Union[nx.Graph, nx.DiGraph]):
     err = []
     for gkey in ['class_attribute', 'class_values', 'class_labels']:
```

### Comparing `netin-1.0.5.9.1/netin/viz/handlers.py` & `netin-1.0.6/netin/viz/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     Resets the style of the plots to the default style.
 
     """
     sns.reset_orig()
 
 
 def set_paper_style(font_scale: float = 1.0):
-    """
+    """plot_graph
     Sets the style of the plots to the paper style.
     Font family serif, and allows to adjust the font scale.
 
     Parameters
     ----------
     font_scale: float
         A scale factor for the font size.
@@ -221,26 +221,30 @@
     maj_patch = mpatches.Patch(color=COLOR_MAJORITY, label='majority')
     min_patch = mpatches.Patch(color=COLOR_MINORITY, label='minority')
     bbox = kwargs.pop('bbox', (1.04, 1))
     loc = kwargs.pop('loc', "upper left")
     fig.legend(handles=[maj_patch, min_patch], bbox_to_anchor=bbox, loc=loc)
 
 
-def plot_graph(data: Union[Graph, Set[Graph], List[Graph]], share_pos: bool = False, fn: str = None, **kwargs):
+def plot_graph(data: Union[Graph, Set[Graph], List[Graph]], share_pos: bool = False, ignore_singletons: bool = False,
+               fn: str = None, **kwargs):
     """
     Plots one or multiple (netin.Graph) graphs as matplotlib figures.
 
     Parameters
     ----------
     data: Union[netin.Graph, Set[netin.Graph]]
         graph or set of graphs to plot
 
     share_pos: bool
         if True, the positions of the nodes are shared between the graphs
 
+    ignore_singletons: bool
+        if True, only nodes with degree > 0 are plotted
+
     fn: str
         filename to save the figure
 
     kwargs: dict
         Additional arguments for the ``subplots`` function of the figure.
 
         cell_size: float
@@ -290,15 +294,20 @@
     pos = None
     for cell in np.arange(nc * nr):
         row = cell // nc
         col = cell % nc
         ax = axes if nr == nc == 1 else axes[cell] if nr == 1 else axes[row, col]
 
         if cell < len(iter_graph):
-            g = iter_graph[cell]
+            g = iter_graph[cell].copy()
+
+            if ignore_singletons:
+                to_remove = [n for n in g.nodes() if g.degree(n) == 0]
+                if len(to_remove) > 0:
+                    g.remove_nodes_from(to_remove)
 
             if pos is None or not share_pos:
                 pos = nx.spring_layout(g)
 
             # title
             ax.set_title(g.get_model_name())
```

### Comparing `netin-1.0.5.9.1/netin.egg-info/PKG-INFO` & `netin-1.0.6/netin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.9.1
+Version: 1.0.6
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.5.9.1/netin.egg-info/SOURCES.txt` & `netin-1.0.6/netin.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
+examples/deleteme/deleteme.py
+examples/deleteme/www/helper.py
+examples/deleteme/www/data/example.gt.gz
 examples/directed/dh.py
 examples/directed/dpa.py
 examples/directed/dpah.py
-examples/notebooks/deleteme.py
 examples/undirected/pa.py
 examples/undirected/pah.py
 examples/undirected/patc.py
 examples/undirected/patch.py
 netin/__init__.py
 netin.egg-info/PKG-INFO
 netin.egg-info/SOURCES.txt
```

### Comparing `netin-1.0.5.9.1/setup.py` & `netin-1.0.6/setup.py`

 * *Files identical despite different names*

