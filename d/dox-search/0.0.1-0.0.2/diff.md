# Comparing `tmp/dox-search-0.0.1.tar.gz` & `tmp/dox-search-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dox-search-0.0.1.tar", last modified: Sat Apr 29 17:47:15 2023, max compression
+gzip compressed data, was "dox-search-0.0.2.tar", last modified: Sun Apr 30 02:51:40 2023, max compression
```

## Comparing `dox-search-0.0.1.tar` & `dox-search-0.0.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-29 17:47:15.325028 dox-search-0.0.1/
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)    35149 2022-06-29 03:24:39.000000 dox-search-0.0.1/LICENSE
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     1293 2023-04-29 17:47:15.325028 dox-search-0.0.1/PKG-INFO
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      755 2023-04-27 23:20:15.000000 dox-search-0.0.1/README.md
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      103 2023-04-27 23:19:59.000000 dox-search-0.0.1/pyproject.toml
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      720 2023-04-29 17:47:15.325028 dox-search-0.0.1/setup.cfg
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       38 2023-04-27 23:19:59.000000 dox-search-0.0.1/setup.py
-drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-29 17:47:15.321695 dox-search-0.0.1/src/
-drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-29 17:47:15.321695 dox-search-0.0.1/src/dox/
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       20 2023-04-28 02:37:01.000000 dox-search-0.0.1/src/dox/__init__.py
-drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-29 17:47:15.321695 dox-search-0.0.1/src/dox/candidate_network/
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      110 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/candidate_network/__init__.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)    14511 2023-04-28 02:32:54.000000 dox-search-0.0.1/src/dox/candidate_network/candidate_network.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     7658 2023-04-28 02:32:44.000000 dox-search-0.0.1/src/dox/candidate_network/candidate_network_handler.py
-drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-29 17:47:15.321695 dox-search-0.0.1/src/dox/database/
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       39 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/database/__init__.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     4598 2023-04-28 02:33:07.000000 dox-search-0.0.1/src/dox/database/mongo_handler.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     2846 2023-04-28 02:33:16.000000 dox-search-0.0.1/src/dox/database/mongo_iter.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)    15031 2023-04-29 17:45:52.000000 dox-search-0.0.1/src/dox/dox.py
-drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-29 17:47:15.321695 dox-search-0.0.1/src/dox/evaluation/
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       91 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/evaluation/__init__.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)    14749 2023-04-28 02:33:35.000000 dox-search-0.0.1/src/dox/evaluation/evaluation_handler.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     3279 2023-04-28 02:33:47.000000 dox-search-0.0.1/src/dox/evaluation/evaluation_report.py
-drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-29 17:47:15.321695 dox-search-0.0.1/src/dox/index/
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      148 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/index/__init__.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     2069 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/index/babel_hash.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      832 2023-04-28 02:34:01.000000 dox-search-0.0.1/src/dox/index/index_build.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     9281 2023-04-29 05:11:05.000000 dox-search-0.0.1/src/dox/index/index_handler.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     1383 2023-04-28 02:34:13.000000 dox-search-0.0.1/src/dox/index/schema_graph.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     2611 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/index/schema_index.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     5846 2023-04-28 02:54:53.000000 dox-search-0.0.1/src/dox/index/value_index.py
-drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-29 17:47:15.321695 dox-search-0.0.1/src/dox/keyword_match/
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       94 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/keyword_match/__init__.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)    11547 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/keyword_match/keyword_match.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     9864 2023-04-28 02:34:30.000000 dox-search-0.0.1/src/dox/keyword_match/keyword_match_handler.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)    12253 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/mapper.py
-drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-29 17:47:15.321695 dox-search-0.0.1/src/dox/query_match/
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       86 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/query_match/__init__.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     4135 2023-04-28 02:34:35.000000 dox-search-0.0.1/src/dox/query_match/query_match.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     3413 2023-04-28 02:51:20.000000 dox-search-0.0.1/src/dox/query_match/query_match_handler.py
-drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-29 17:47:15.325028 dox-search-0.0.1/src/dox/utils/
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      794 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/utils/__init__.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     4185 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/utils/config_handler.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     9719 2023-04-28 02:34:49.000000 dox-search-0.0.1/src/dox/utils/document_traverser.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     6500 2023-04-28 02:35:01.000000 dox-search-0.0.1/src/dox/utils/generate_evaluation_report.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     5187 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/utils/graph.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      816 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/utils/keyword_query.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      206 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/utils/logger.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      147 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/utils/memory.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)    13905 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/utils/mongo_query_builder.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       78 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/utils/ordinal.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      777 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/utils/plots.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       95 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/utils/printmd.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     4955 2023-04-28 02:35:47.000000 dox-search-0.0.1/src/dox/utils/result.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       78 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/utils/shift_tab.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     2181 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/utils/similarity.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     1265 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/utils/tf_iaf.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       79 2023-04-27 23:19:59.000000 dox-search-0.0.1/src/dox/utils/timestr.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     3505 2023-04-28 02:36:20.000000 dox-search-0.0.1/src/dox/utils/tokenizer.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      100 2023-04-28 02:36:28.000000 dox-search-0.0.1/src/dox/utils/truncate.py
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     3539 2023-04-28 02:36:53.000000 dox-search-0.0.1/src/dox/utils/utils.py
-drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-29 17:47:15.325028 dox-search-0.0.1/src/dox_search.egg-info/
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     1293 2023-04-29 17:47:14.000000 dox-search-0.0.1/src/dox_search.egg-info/PKG-INFO
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     1626 2023-04-29 17:47:15.000000 dox-search-0.0.1/src/dox_search.egg-info/SOURCES.txt
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)        1 2023-04-29 17:47:14.000000 dox-search-0.0.1/src/dox_search.egg-info/dependency_links.txt
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       33 2023-04-29 17:47:15.000000 dox-search-0.0.1/src/dox_search.egg-info/requires.txt
--rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)        4 2023-04-29 17:47:15.000000 dox-search-0.0.1/src/dox_search.egg-info/top_level.txt
+drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-30 02:51:40.899865 dox-search-0.0.2/
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)    35149 2022-06-29 03:24:39.000000 dox-search-0.0.2/LICENSE
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     1293 2023-04-30 02:51:40.899865 dox-search-0.0.2/PKG-INFO
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      755 2023-04-27 23:20:15.000000 dox-search-0.0.2/README.md
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      103 2023-04-27 23:19:59.000000 dox-search-0.0.2/pyproject.toml
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      720 2023-04-30 02:51:40.899865 dox-search-0.0.2/setup.cfg
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       38 2023-04-27 23:19:59.000000 dox-search-0.0.2/setup.py
+drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-30 02:51:40.896532 dox-search-0.0.2/src/
+drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-30 02:51:40.899865 dox-search-0.0.2/src/dox/
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       20 2023-04-28 02:37:01.000000 dox-search-0.0.2/src/dox/__init__.py
+drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-30 02:51:40.899865 dox-search-0.0.2/src/dox/candidate_network/
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      110 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/candidate_network/__init__.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)    14511 2023-04-28 02:32:54.000000 dox-search-0.0.2/src/dox/candidate_network/candidate_network.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     7658 2023-04-28 02:32:44.000000 dox-search-0.0.2/src/dox/candidate_network/candidate_network_handler.py
+drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-30 02:51:40.899865 dox-search-0.0.2/src/dox/database/
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       39 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/database/__init__.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     4598 2023-04-28 02:33:07.000000 dox-search-0.0.2/src/dox/database/mongo_handler.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     2846 2023-04-28 02:33:16.000000 dox-search-0.0.2/src/dox/database/mongo_iter.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)    15031 2023-04-29 17:45:52.000000 dox-search-0.0.2/src/dox/dox.py
+drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-30 02:51:40.899865 dox-search-0.0.2/src/dox/evaluation/
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       91 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/evaluation/__init__.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)    14749 2023-04-28 02:33:35.000000 dox-search-0.0.2/src/dox/evaluation/evaluation_handler.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     3279 2023-04-28 02:33:47.000000 dox-search-0.0.2/src/dox/evaluation/evaluation_report.py
+drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-30 02:51:40.899865 dox-search-0.0.2/src/dox/index/
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      148 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/index/__init__.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     2069 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/index/babel_hash.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      832 2023-04-28 02:34:01.000000 dox-search-0.0.2/src/dox/index/index_build.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     9281 2023-04-29 05:11:05.000000 dox-search-0.0.2/src/dox/index/index_handler.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     1383 2023-04-28 02:34:13.000000 dox-search-0.0.2/src/dox/index/schema_graph.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     2611 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/index/schema_index.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     5846 2023-04-28 02:54:53.000000 dox-search-0.0.2/src/dox/index/value_index.py
+drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-30 02:51:40.899865 dox-search-0.0.2/src/dox/keyword_match/
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       94 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/keyword_match/__init__.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)    11547 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/keyword_match/keyword_match.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     9864 2023-04-28 02:34:30.000000 dox-search-0.0.2/src/dox/keyword_match/keyword_match_handler.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)    12253 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/mapper.py
+drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-30 02:51:40.899865 dox-search-0.0.2/src/dox/query_match/
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       86 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/query_match/__init__.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     4135 2023-04-28 02:34:35.000000 dox-search-0.0.2/src/dox/query_match/query_match.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     3413 2023-04-28 02:51:20.000000 dox-search-0.0.2/src/dox/query_match/query_match_handler.py
+drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-30 02:51:40.899865 dox-search-0.0.2/src/dox/utils/
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      794 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/utils/__init__.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     4127 2023-04-30 02:51:32.000000 dox-search-0.0.2/src/dox/utils/config_handler.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     9719 2023-04-28 02:34:49.000000 dox-search-0.0.2/src/dox/utils/document_traverser.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     6500 2023-04-28 02:35:01.000000 dox-search-0.0.2/src/dox/utils/generate_evaluation_report.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     5187 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/utils/graph.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      816 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/utils/keyword_query.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      206 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/utils/logger.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      147 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/utils/memory.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)    13905 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/utils/mongo_query_builder.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       78 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/utils/ordinal.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      777 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/utils/plots.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       95 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/utils/printmd.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     4955 2023-04-28 02:35:47.000000 dox-search-0.0.2/src/dox/utils/result.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       78 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/utils/shift_tab.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     2181 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/utils/similarity.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     1265 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/utils/tf_iaf.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       79 2023-04-27 23:19:59.000000 dox-search-0.0.2/src/dox/utils/timestr.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     3505 2023-04-28 02:36:20.000000 dox-search-0.0.2/src/dox/utils/tokenizer.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)      100 2023-04-28 02:36:28.000000 dox-search-0.0.2/src/dox/utils/truncate.py
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     3539 2023-04-28 02:36:53.000000 dox-search-0.0.2/src/dox/utils/utils.py
+drwxr-xr-x   0 arielafonso  (1000) arielafonso  (1000)        0 2023-04-30 02:51:40.899865 dox-search-0.0.2/src/dox_search.egg-info/
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     1293 2023-04-30 02:51:40.000000 dox-search-0.0.2/src/dox_search.egg-info/PKG-INFO
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)     1626 2023-04-30 02:51:40.000000 dox-search-0.0.2/src/dox_search.egg-info/SOURCES.txt
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)        1 2023-04-30 02:51:40.000000 dox-search-0.0.2/src/dox_search.egg-info/dependency_links.txt
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)       33 2023-04-30 02:51:40.000000 dox-search-0.0.2/src/dox_search.egg-info/requires.txt
+-rw-r--r--   0 arielafonso  (1000) arielafonso  (1000)        4 2023-04-30 02:51:40.000000 dox-search-0.0.2/src/dox_search.egg-info/top_level.txt
```

### Comparing `dox-search-0.0.1/LICENSE` & `dox-search-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/PKG-INFO` & `dox-search-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dox-search
-Version: 0.0.1
+Version: 0.0.2
 Summary: Keyword Exploration over Document Stores
 Home-page: https://github.com/bdri-ufam/dox
 Author: Ariel Afonso
 Author-email: ariel.afonso@icomp.ufam.edu.br
 Project-URL: Bug Tracker, https://github.com/bdri-ufam/dox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dox-search-0.0.1/README.md` & `dox-search-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/setup.cfg` & `dox-search-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dox-search
-version = 0.0.1
+version = 0.0.2
 author = Ariel Afonso
 author_email = ariel.afonso@icomp.ufam.edu.br
 description = Keyword Exploration over Document Stores
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/bdri-ufam/dox
 project_urls =
```

### Comparing `dox-search-0.0.1/src/dox/candidate_network/candidate_network.py` & `dox-search-0.0.2/src/dox/candidate_network/candidate_network.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/candidate_network/candidate_network_handler.py` & `dox-search-0.0.2/src/dox/candidate_network/candidate_network_handler.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/database/mongo_handler.py` & `dox-search-0.0.2/src/dox/database/mongo_handler.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/database/mongo_iter.py` & `dox-search-0.0.2/src/dox/database/mongo_iter.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/dox.py` & `dox-search-0.0.2/src/dox/dox.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/evaluation/evaluation_handler.py` & `dox-search-0.0.2/src/dox/evaluation/evaluation_handler.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/evaluation/evaluation_report.py` & `dox-search-0.0.2/src/dox/evaluation/evaluation_report.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/index/babel_hash.py` & `dox-search-0.0.2/src/dox/index/babel_hash.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/index/index_build.py` & `dox-search-0.0.2/src/dox/index/index_build.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/index/index_handler.py` & `dox-search-0.0.2/src/dox/index/index_handler.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/index/schema_graph.py` & `dox-search-0.0.2/src/dox/index/schema_graph.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/index/schema_index.py` & `dox-search-0.0.2/src/dox/index/schema_index.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/index/value_index.py` & `dox-search-0.0.2/src/dox/index/value_index.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/keyword_match/keyword_match.py` & `dox-search-0.0.2/src/dox/keyword_match/keyword_match.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/keyword_match/keyword_match_handler.py` & `dox-search-0.0.2/src/dox/keyword_match/keyword_match_handler.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/mapper.py` & `dox-search-0.0.2/src/dox/mapper.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/query_match/query_match.py` & `dox-search-0.0.2/src/dox/query_match/query_match.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/query_match/query_match_handler.py` & `dox-search-0.0.2/src/dox/query_match/query_match_handler.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/utils/__init__.py` & `dox-search-0.0.2/src/dox/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/utils/config_handler.py` & `dox-search-0.0.2/src/dox/utils/config_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             if 'dataset' in kwargs:
                 self.dataset = kwargs.get('dataset')
 
             self.queryset_config = self.get_queryset_filepath(
                 self.dataset,
             )
 
-            self.dataset_config = self.default_settings['dataset_config']
+            self.dataset_config = deepcopy(self.default_settings['dataset_config'])
             self.update_config_paths(
                 self.dataset,
                 self.dataset_config,
             )
 
             self.connection['database'] = self.dataset
         else:
@@ -72,16 +72,14 @@
 
             self.create_index = config['create_index']
             self.plots_directory = config['plots_directory']
             self.results_directory = config['results_directory']
             self.logging_mode = self.set_logging_level(
                 config['logging_mode'],
             )
-        print('Default settings')
-        pp(self.default_settings)
 
     def load_config(self, filepath):
         with open(filepath, 'r') as f:
             config = json.load(f)
         return config
     
     def get_queryset_filepath(self, dataset):
```

### Comparing `dox-search-0.0.1/src/dox/utils/document_traverser.py` & `dox-search-0.0.2/src/dox/utils/document_traverser.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/utils/generate_evaluation_report.py` & `dox-search-0.0.2/src/dox/utils/generate_evaluation_report.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/utils/graph.py` & `dox-search-0.0.2/src/dox/utils/graph.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/utils/keyword_query.py` & `dox-search-0.0.2/src/dox/utils/keyword_query.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/utils/mongo_query_builder.py` & `dox-search-0.0.2/src/dox/utils/mongo_query_builder.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/utils/plots.py` & `dox-search-0.0.2/src/dox/utils/plots.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/utils/result.py` & `dox-search-0.0.2/src/dox/utils/result.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/utils/similarity.py` & `dox-search-0.0.2/src/dox/utils/similarity.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/utils/tf_iaf.py` & `dox-search-0.0.2/src/dox/utils/tf_iaf.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/utils/tokenizer.py` & `dox-search-0.0.2/src/dox/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox/utils/utils.py` & `dox-search-0.0.2/src/dox/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dox-search-0.0.1/src/dox_search.egg-info/PKG-INFO` & `dox-search-0.0.2/src/dox_search.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dox-search
-Version: 0.0.1
+Version: 0.0.2
 Summary: Keyword Exploration over Document Stores
 Home-page: https://github.com/bdri-ufam/dox
 Author: Ariel Afonso
 Author-email: ariel.afonso@icomp.ufam.edu.br
 Project-URL: Bug Tracker, https://github.com/bdri-ufam/dox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dox-search-0.0.1/src/dox_search.egg-info/SOURCES.txt` & `dox-search-0.0.2/src/dox_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

