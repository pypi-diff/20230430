# Comparing `tmp/beginai-2.0.0.tar.gz` & `tmp/beginai-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beginai-2.0.0.tar", last modified: Wed Apr 26 22:08:40 2023, max compression
+gzip compressed data, was "beginai-2.0.1.tar", last modified: Sun Apr 30 00:58:36 2023, max compression
```

## Comparing `beginai-2.0.0.tar` & `beginai-2.0.1.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-26 22:08:40.980579 beginai-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-26 22:08:28.000000 beginai-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.976579 beginai-2.0.0/beginai/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.976579 beginai-2.0.0/beginai/conn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/conn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/conn/mqtt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.976579 beginai-2.0.0/beginai/exec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.976579 beginai-2.0.0/beginai/exec/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17506 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/apply.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/beginai/exec/embeddings/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/category.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/date.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/beginai/exec/embeddings/instructions/deep_text/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/deep_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/deep_text/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/parse_and_execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/master.py
--rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/execute_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/remote_compute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/beginai/orchapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/orchapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/orchapi/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/beginai/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/storage/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/storage/sqllite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/beginai/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/beginai/tests/exec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/beginai/tests/exec/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/boolean_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/category_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/date_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/interaction_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/location_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/number_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16533 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/parse_and_execute_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/text_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/mock_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/worker_methods_validation_interaction_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/worker_methods_validation_labels_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/worker_methods_validation_object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/worker_methods_validation_user_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20805 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/worker_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/beginai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/utils/syft.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.976579 beginai-2.0.0/beginai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-26 22:08:40.000000 beginai-2.0.0/beginai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-26 22:08:40.000000 beginai-2.0.0/beginai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 22:08:40.000000 beginai-2.0.0/beginai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-26 22:08:40.000000 beginai-2.0.0/beginai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 22:08:40.000000 beginai-2.0.0/beginai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-26 22:08:40.980579 beginai-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-26 22:08:39.000000 beginai-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.701349 beginai-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-30 00:58:36.701349 beginai-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-30 00:58:25.000000 beginai-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.673349 beginai-2.0.1/beginai/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.677349 beginai-2.0.1/beginai/conn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/conn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/conn/mqtt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.681349 beginai-2.0.1/beginai/exec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.681349 beginai-2.0.1/beginai/exec/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17674 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/apply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.689349 beginai-2.0.1/beginai/exec/embeddings/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/date.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.689349 beginai-2.0.1/beginai/exec/embeddings/instructions/deep_text/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/deep_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/deep_text/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17517 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/execute_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/remote_compute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.689349 beginai-2.0.1/beginai/orchapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/orchapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/orchapi/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.693349 beginai-2.0.1/beginai/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/storage/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/storage/sqllite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.693349 beginai-2.0.1/beginai/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.693349 beginai-2.0.1/beginai/tests/exec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.697349 beginai-2.0.1/beginai/tests/exec/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.701349 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/boolean_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/category_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/date_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/interaction_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/location_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/number_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/text_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/mock_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_interaction_attributes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_interaction_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_labels_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_user_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/worker_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.701349 beginai-2.0.1/beginai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/utils/syft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.677349 beginai-2.0.1/beginai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-30 00:58:36.000000 beginai-2.0.1/beginai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-30 00:58:36.000000 beginai-2.0.1/beginai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 00:58:36.000000 beginai-2.0.1/beginai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-30 00:58:36.000000 beginai-2.0.1/beginai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 00:58:36.000000 beginai-2.0.1/beginai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-30 00:58:36.701349 beginai-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-30 00:58:35.000000 beginai-2.0.1/setup.py
```

### Comparing `beginai-2.0.0/PKG-INFO` & `beginai-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beginai
-Version: 2.0.0
+Version: 2.0.1
 Summary: A library to interact with Begin AI platform in order to build personalisation algorithms.
 Home-page: https://docs.begin.ai
 Author: Begin AI Research & Engineering
 Author-email: engineering@begin.ai
 License: Proprietary
 Description: 
                 This is Begin AI python SDK for both batch processing and application integration.
```

### Comparing `beginai-2.0.0/beginai/conn/mqtt.py` & `beginai-2.0.1/beginai/conn/mqtt.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/exec/embeddings/apply.py` & `beginai-2.0.1/beginai/exec/embeddings/apply.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from beginai.utils.date import parse_date_to_format
-from . import ParseAndExecute
+from . import Parser
 from ...orchapi.api import OrchAPI
 from tqdm import tqdm
 import pandas as pd
 import datetime
 from beginai.exec.embeddings.instructions.utils import sort_instructions
 
 
@@ -13,17 +13,18 @@
 
     INTERACTIONS = 'interactions'
     CREATED_AT = 'beginai_created_at'
     INTERVENTION_TIMESTAMP = 'intervention_timestamp'
     LABELS = 'labels'
     BATCH_SIZE = 20000
 
-    def __init__(self, app_id, license_key, host=None):
+    def __init__(self, app_id, license_key, host=None, debug=False):
         self.orchapi = OrchAPI()
         self.orchapi.configure_orch_connection(host or self.host)
+        self.orchapi.set_debug(debug)
         self.orchapi.set_app_id_and_license_key(
             app_id=app_id, license_key=license_key)
         self._submission_in_progress = False
 
         self.embeddings = {}
         self.files = {}
 
@@ -93,68 +94,65 @@
             return
 
         print("Start time: ", datetime.datetime.now())
 
         instructions_id, current_embeddings_version, instructions = \
             self._get_instructions()
 
-        self._generate_signatures(instructions)
+        self._generate_embeddings(instructions)
 
         self._submit_embeddings(instructions_id, current_embeddings_version, update)
 
         print("End time: ", datetime.datetime.now())
         self.flush_memory()
 
     def flush_memory(self):
         self.embeddings = {}
         self.files = {}
 
-    def _generate_signatures(self, instructions):
-        parser = ParseAndExecute(instructions)
+    def _generate_embeddings(self, instructions):
+        parser = Parser(instructions)
 
         for object_key in self.files.keys():
             object_config = self.files[object_key]
 
             df: pd.DataFrame = object_config['data']
             uuid_column = object_config['uuid_column']
 
             df = self._preparing_dataframe(
                 df, object_config, object_key, instructions)
 
             dictionary = df.to_dict(orient='records')
 
-            object_data = []
-
             if object_key == self.INTERACTIONS:
                 target_object = object_config['target_object']
                 target_object_name = target_object['name']
                 user_interactions = self._parse_interactions(
-                    df, uuid_column, target_object)
+                    df, uuid_column, target_object, target_object_name)
 
                 grouped_interactions = {
-                    'interactions': [],
-                    'raw_interactions': []
+                    'interactions': []
                 }
 
                 for user_id in user_interactions.keys():
                     value = user_interactions[user_id]
                     parser.feed(value)
                     results = parser.parse(object_key)
                     if len(results) > 0:
                         grouped_interactions['interactions'].append(
                             [str(user_id), target_object_name, results[self.INTERACTIONS]])
-                        grouped_interactions['raw_interactions'].append(
-                            [str(user_id), target_object_name, results['raw_interactions']])
 
-                if len(grouped_interactions['interactions']) > 0 or len(grouped_interactions['raw_interactions']) > 0:
+                if len(grouped_interactions['interactions']) > 0:
                     if object_key not in self.embeddings:
                         self.embeddings[object_key] = []
                     self.embeddings[object_key] = grouped_interactions
 
             else:
+                object_data = []
+
                 for index, row in tqdm(enumerate(dictionary)):
                     parser.feed(row)
                     results = parser.parse(object_key)
                     if len(results) > 0:
                         key = row[uuid_column]
                         object_data.append([key, results])
 
@@ -192,53 +190,61 @@
         else:
             df[self.CREATED_AT] = datetime.datetime.now(
                 datetime.timezone.utc).timestamp()
 
         tokenize_instructions = instructions.get("tokenize", {})
         identifiers_instructions = instructions.get("identifiers", {})
 
-        is_object_key_text_tokenize = tokenize_instructions.get(object_key, None) is not None
-        is_object_key_id = identifiers_instructions.get(object_key, None) is not None
+        is_object_key_text_tokenize = tokenize_instructions.get(
+            object_key, None) is not None
+        is_object_key_id = identifiers_instructions.get(
+            object_key, None) is not None
         if object_key != self.INTERACTIONS and (is_object_key_text_tokenize == True or is_object_key_id == True):
             tokenize_properties = tokenize_instructions.get(object_key, [])
 
             for tokenize_property_name in tokenize_properties:
                 df[tokenize_property_name].fillna(value="", inplace=True)
 
-            identifier_properties = identifiers_instructions.get(object_key, [])
+            identifier_properties = identifiers_instructions.get(
+                object_key, [])
             for identifier_property_name in identifier_properties:
                 df[identifier_property_name].fillna(value="", inplace=True)
-
         return df
 
-    def _parse_interactions(self, df, uuid_column, target_object):
-        target_object_name = target_object['name']
-        interaction_column = target_object['interaction_column']
-        df = df.dropna().groupby(
-            [uuid_column, target_object['uuid_column']], as_index=False)
+    def _parse_interactions(self, df: pd.DataFrame, uuid_column: str, target_object: dict, target_object_name: str) -> dict:
+        interaction_column: str = target_object['interaction_column']
+        target_uuid_column = target_object['uuid_column']
+        df = df.rename(columns= {interaction_column: 'action', self.CREATED_AT: 'created_at'})
+        # Fill NA with '' to tell the parsers that the value doesn't exist
+        df = df.fillna('')
+        df = df.groupby(
+            [uuid_column, target_uuid_column], as_index=False)
 
-        user_interactions = {}
-        for key, group in tqdm(df):
+        interactions = {}
+        for key, group in tqdm(df, desc="Parsing Interactions"):
             uuid = key[0]
             target_uuid = key[1]
 
-            if uuid not in user_interactions:
-                user_interactions[uuid] = {}
+            if uuid not in interactions:
+                interactions[uuid] = {}
 
-            if target_object_name not in user_interactions[uuid]:
-                user_interactions[uuid][target_object_name] = {}
+            if target_object_name not in interactions[uuid]:
+                interactions[uuid][target_object_name] = {}
 
-            if target_uuid not in user_interactions[uuid][target_object_name]:
-                user_interactions[uuid][target_object_name][target_uuid] = []
+            if target_uuid not in interactions[uuid][target_object_name]:
+                interactions[uuid][target_object_name][target_uuid] = {}
 
-            for action_value in group.apply(lambda row: [{'value': row[interaction_column], 'created_at': row[self.CREATED_AT]}], axis=1):
-                user_interactions[uuid][target_object_name][target_uuid].append(
-                    action_value[0])
-
-        return user_interactions
+            grouped_columns = group[group.columns[~group.columns.isin([target_uuid_column, uuid_column])]]
+            
+            for data in grouped_columns.to_dict(orient='records'):
+                action = data['action']
+                del data['action']
+                interactions[uuid][target_object_name][target_uuid][action] = data
+        
+        return interactions
     
     def _submit_intervention_dates(self, data, object_name):
         if self._submission_in_progress:
             return
         
         self._submission_in_progress = True
 
@@ -382,16 +388,15 @@
         """
         if len(self.files) == 0:
             return
 
         print("Start time: ", datetime.datetime.now())
 
         instructions_id, current_embeddings_version, instructions = self._get_instructions()
-
-        self._generate_signatures(instructions)
+        self._generate_embeddings(instructions)
         return self.embeddings
 
     def get_embedding_position_label(self, object_type):
         instructions_id, current_embeddings_version, data = self._get_instructions()
 
         position_label = []
```

### Comparing `beginai-2.0.0/beginai/exec/embeddings/instructions/__init__.py` & `beginai-2.0.1/beginai/exec/embeddings/instructions/__init__.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/exec/embeddings/instructions/date.py` & `beginai-2.0.1/beginai/exec/embeddings/instructions/date.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/exec/embeddings/instructions/deep_text/bpe.py` & `beginai-2.0.1/beginai/exec/embeddings/instructions/deep_text/bpe.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import defaultdict
 import json, re, string
 import urllib.request
 
 class BPE(object):
     def __init__(self):
-        vocab_location = "https://beginai-demo-datasets.s3.ca-central-1.amazonaws.com/vocab.json"
+        vocab_location = "https://storage.googleapis.com/beginai-demo-datasets/vocab.json"
         with urllib.request.urlopen(vocab_location) as url:
             data = json.loads(url.read().decode())
         vocab_stoi = data
 
         self.vocab_stoi = defaultdict(lambda: vocab_stoi['[UNK]'], vocab_stoi)
         self.vocab_itos = list(data.keys())
```

### Comparing `beginai-2.0.0/beginai/exec/embeddings/instructions/interaction.py` & `beginai-2.0.1/beginai/exec/embeddings/instructions/interaction.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/exec/embeddings/instructions/location.py` & `beginai-2.0.1/beginai/exec/embeddings/instructions/location.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/exec/embeddings/instructions/number.py` & `beginai-2.0.1/beginai/exec/embeddings/instructions/number.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/exec/embeddings/instructions/parse_and_execute.py` & `beginai-2.0.1/beginai/exec/embeddings/instructions/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,29 +11,27 @@
 from .interaction import InteractionEncoding
 from .utils import sort_instructions
 
 ERR_NUMBER = 0.00011
 EMPTY_NUMBER = 0.00012
 
 
-class ParseAndExecute(object):
+class Parser(object):
 
     INTERACTIONS_KEY = "interactions"
     LABELS_KEY = "labels"
     TOKENIZE_KEY = "tokenize"
     IDENTIFIERS_KEY = "identifiers"
-    RAW_INTERACTION_KEY = "raw_interactions"
 
     def __init__(self, data):
         self.instructions = self._group_and_sort_instructions(data)
         self.labels = self._retrieve_labels(data)
         self.tokenization_fields = self._retrieve_tokenization_fields(data)
         self.tokenize_instruction = instructions_map["Tokenize"]()
         self.identifiers = self._retrieve_identifiers(data)
-        self.raw_interactions = self._retrieve_raw_interactions(data)
 
     def _group_and_sort_instructions(self, data):
         return sort_instructions(data)
 
     def _retrieve(self, data, key):
         if len(data) == 0:
             return {}
@@ -44,31 +42,29 @@
 
     def _retrieve_tokenization_fields(self, data):
         return self._retrieve(data, self.TOKENIZE_KEY)
 
     def _retrieve_identifiers(self, data):
         return self._retrieve(data, self.IDENTIFIERS_KEY)
 
-    def _retrieve_raw_interactions(self, data):
-        return self._retrieve(data, self.RAW_INTERACTION_KEY)
-
     def feed(self, values_dict):
         self.values = values_dict
 
-    def _process_instruction(self, value, instruct):
+    def _process_instruction(self, value, instruct, provided_values_for_object):
         klass = instructions_map.get(instruct["instruct"])
         if not klass:
             return ERR_NUMBER
         # if instruction involves multiple fields.
         other_value = None
 
         instruct_params = instruct.get("params", {}).copy()
         # if params point to another field, get that field value too.
         if "field" in instruct_params:
-            other_value = self.values.get(instruct_params["field"])
+            other_value = provided_values_for_object.get(
+                instruct_params["field"])
             del instruct_params["field"]
 
         obj = klass(**instruct_params)
 
         try:
             if other_value:
                 # in case it involves two fields.
@@ -135,121 +131,117 @@
             return object_identifiers
 
         for identifier in identifiers_name:
             object_identifiers[identifier] = object_values.get(identifier, "")
 
         return object_identifiers
 
+    def _parse_interactions(self) -> dict:
+        return {
+            "interactions": self._get_interaction_embeddings_and_actions()
+        }
+
+    def _parse_object(self, object_name: str) -> dict:
+        labels = []
+        identifiers = {}
+        tokens = {"input_ids": [], "attention_mask": [], "len_": 0}
+
+        # At this point, created_at is used on batch processing only
+        created_at = self.values.get("beginai_created_at", None)
+
+        if self.labels.get(object_name) is not None:
+            labels = self._process_labels(object_name, self.values)
+
+        if self.tokenization_fields.get(object_name) is not None:
+            tokens = self._process_text_tokens(object_name, self.values)
+
+        if self.identifiers.get(object_name) is not None:
+            identifiers = self._process_identifiers(
+                object_name, self.values)
+
+        embedding = self._process_object_embedding(
+            self.instructions.get(object_name.lower()), self.values)
+
+        return {
+            "embedding": embedding,
+            "labels": labels,
+            "tokens": tokens,
+            "identifiers": identifiers,
+            "created_at": created_at,
+        }
+
     def parse(self, object_name):
         if self.instructions.get(object_name) == None:
             return {}
 
         if object_name == self.INTERACTIONS_KEY:
-            return {
-                "interactions": self._process_interactions(),
-                "raw_interactions": self._process_raw_interactions()
-            }
+            return self._parse_interactions()
         else:
-            embedding = []
-            labels = []
-            identifiers = {}
-            tokens = {"input_ids": [], "attention_mask": [], "len_": 0}
-
-            # At this point, created_at is used on batch processing only
-            created_at = self.values.get("beginai_created_at", None)
-
-            if self.labels.get(object_name) is not None:
-                labels = self._process_labels(object_name, self.values)
-
-            if self.tokenization_fields.get(object_name) is not None:
-                tokens = self._process_text_tokens(object_name, self.values)
-
-            if self.identifiers.get(object_name) is not None:
-                identifiers = self._process_identifiers(
-                    object_name, self.values)
-
-            for instruct in self.instructions.get(object_name.lower()):
-                chains = instruct.get("_chains", None)
-                value = self.values.get(instruct["f_id"].lower())
-
-                if not value and (value != 0 and instruct["instruct"] == "Boolean"):
-                    embedding.append(ERR_NUMBER)
-                    continue
-
-                if chains:
-                    for chain in chains:
-                        chain_list = sorted(chain, key=lambda k: k["order"])
-                        for item in chain_list:
-                            value = self._process_instruction(value, item)
-                        # last response in the chain is the return value.
-                        res = value
-                        embedding.append(res)
-                else:
-                    res = self._process_instruction(value, instruct)
-                    embedding.append(res)
-
-            return {
-                "embedding": embedding,
-                "labels": labels,
-                "tokens": tokens,
-                "identifiers": identifiers,
-                "created_at": created_at,
-            }
-
-    def _process_raw_interactions(self):
-        object_raw_interactions = {}
-        for object_key in self.values.keys():
-            available_raw_interactions = self.raw_interactions.get(
-                object_key, [])
+            return self._parse_object(object_name)
 
-            if len(available_raw_interactions) == 0:
+    def _process_object_embedding(self, instructions, provided_values_for_object):
+        embedding = []
+        # Get the instructions set for the object
+        for instruct in instructions:
+            # Get values set for this object
+            value = provided_values_for_object.get(instruct["f_id"].lower())
+            if not value and (value != 0 and instruct["instruct"] == "Boolean"):
+                embedding.append(ERR_NUMBER)
                 continue
 
-            object_raw_interactions[object_key] = {}
-
-            for action_object in self.values[object_key]:
-                actions = self.values[object_key][action_object]
-                processed_raw_interactions = self._get_raw_interactions(
-                    actions, available_raw_interactions)
-                if len(processed_raw_interactions) > 0:
-                    object_raw_interactions[object_key][action_object] = processed_raw_interactions
-
-        return object_raw_interactions
-
-    def _get_raw_interactions(self, actions, raw_interactions):
-        processed = []
-
-        if len(actions) == 0 or len(raw_interactions) == 0:
-            return processed
-
-        # `actions` contains a list of dictionaries with the action and when was created_at
-        for entry in actions:
-            action = entry["value"].upper()
-            if action in raw_interactions:
-                processed.append({
-                    "value": action,
-                    "created_at": entry["created_at"]
-                })
-
-        return processed
-
-    def _process_interactions(self):
-        embeddings_per_object = {}
-        for object_key in self.values.keys():
-            instruction = next(
-                (item for item in self.instructions[self.INTERACTIONS_KEY] if item["_with_object"] == object_key), None)
-
-            if instruction is None:
-                continue
-
-            embeddings_per_object[object_key] = {}
-
-            for action_object in self.values[object_key]:
-                actions = []
-                for entry in self.values[object_key][action_object]:
-                    actions.append(entry['value'])
-
-                result = self._process_instruction(actions, instruction)
+            embedding.append(self._process_object_instructions(
+                instruct=instruct, value=value, provided_values_for_object=provided_values_for_object))
+        return embedding
+
+    def _process_object_instructions(self, instruct, value, provided_values_for_object):
+        result = value
+        chains = instruct.get("_chains", None)
+
+        if chains:
+            for chain in chains:
+                chain_list = sorted(chain, key=lambda k: k["order"])
+                for item in chain_list:
+                    value = self._process_instruction(
+                        value, item, provided_values_for_object)
+                # last response in the chain is the return value.
+                result = value
+        else:
+            result = self._process_instruction(
+                value, instruct, provided_values_for_object)
 
-                embeddings_per_object[object_key][action_object] = result
+        return result
 
-        return embeddings_per_object
+    def _get_interaction_embeddings_and_actions(self):
+        embeddings = {}
+        object_keys = self.values.keys()
+
+        interactions_from_instruction = self.instructions[self.INTERACTIONS_KEY]
+
+        interaction_keys = interactions_from_instruction.keys()
+        matched_keys = list(set(object_keys).intersection(interaction_keys))
+
+        for matched_key in matched_keys:
+            actions_associated_with_provided_object = self.values.get(matched_key)
+            embeddings[matched_key] = {}
+
+            for target_object_id, actions in actions_associated_with_provided_object.items():
+                embeddings[matched_key][target_object_id] = {}
+
+                for action in actions:
+                    if action in interactions_from_instruction[matched_key]['with_embedding']:
+                        instructions = interactions_from_instruction[matched_key]['with_embedding'][action]
+                        provided_values_for_object = actions[action]
+                        processed_embedding = self._process_object_embedding(
+                            instructions, provided_values_for_object)
+
+                        embeddings[matched_key][target_object_id][action] = { 
+                            "embedding": processed_embedding,
+                            "created_at": provided_values_for_object['created_at'] if 'created_at' in provided_values_for_object else None
+                        }
+
+                    elif action in interactions_from_instruction[matched_key]['just_actions']:
+                        provided_values_for_object = actions[action]
+                        embeddings[matched_key][target_object_id][action] = { 
+                            "embedding": None,
+                            "created_at": provided_values_for_object['created_at'] if 'created_at' in provided_values_for_object else None
+                        }
+        return embeddings
```

### Comparing `beginai-2.0.0/beginai/exec/embeddings/instructions/text.py` & `beginai-2.0.1/beginai/exec/embeddings/instructions/text.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/exec/embeddings/worker.py` & `beginai-2.0.1/beginai/exec/embeddings/worker.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from beginai.utils.date import parse_date_to_format
 from ...orchapi.api import OrchAPI
-from . import ParseAndExecute
+from . import Parser
 import datetime
 
 
 class BeginWorker(object):
 
     host = "https://sdk-a1ummign.uc.gateway.dev"
+    INTERACTIONS = "interactions"
 
     def __init__(self, app_id, license_key, host=None):
         self.orchapi = OrchAPI()
         self.orchapi.configure_orch_connection(host or self.host)
         self.orchapi.set_app_id_and_license_key(
             app_id=app_id, license_key=license_key)
         self._reset_to_initial_state()
@@ -43,14 +44,17 @@
         self._validate_properties_for_user_object(user_id, field, value)
 
         if self._is_valid_type(value, str) == False:
             raise ValueError("Value must be a String")
 
         self._set_value(user_id, field, value, "user")
 
+    def update_user_category_field(self, user_id, field, value: str):
+        self.update_user_text_field(user_id, field, value)
+
     def update_user_boolean_field(self, user_id, field, value: bool):
         self._validate_properties_for_user_object(user_id, field, value)
 
         if self._is_valid_type(value, bool) == False:
             raise ValueError("Value must be a Boolean")
 
         self._set_value(user_id, field, value, "user")
@@ -96,14 +100,17 @@
             object_name, object_id, field, value)
 
         if self._is_valid_type(value, str) == False:
             raise ValueError("Value must be a String")
 
         self._set_value(object_id, field, value, object_name)
 
+    def update_object_category_field(self, object_name, object_id, field, value: str):
+        self.update_object_category_field(object_name, object_id, field, value)
+
     def update_object_boolean_field(self, object_name, object_id, field, value: bool):
         self._validate_properties_for_other_object(
             object_name, object_id, field, value)
 
         if self._is_valid_type(value, bool) == False:
             raise ValueError("Value must be Boolean")
 
@@ -152,33 +159,128 @@
 
     def _set_value(self, object_id, field, value, object_name):
         self.data[object_name.lower()][object_id][field.lower()] = value
 
     def _is_valid_type(self, value, clazz):
         return isinstance(value, clazz)
 
-    def register_interaction(self, user_id, object_name, action, object_id):
+    def _build_interaction_structure(self, user_id, object_name: str, object_id: str):
+        if user_id not in self.data[self.INTERACTIONS]:
+            self.data[self.INTERACTIONS][user_id] = {}
+
+        if object_name not in self.data[self.INTERACTIONS][user_id]:
+            self.data[self.INTERACTIONS][user_id][object_name] = {}
+
+        if object_id not in self.data[self.INTERACTIONS][user_id][object_name]:
+            self.data[self.INTERACTIONS][user_id][object_name][object_id] = []
+
+    def _find_or_register_interaction_by_action(self, user_id, object_name: str, action: str, object_id: str) -> int:
+        self._build_interaction_structure(
+            user_id, object_name, object_id)
+
+        interaction_index = next((i for i, item in enumerate(
+            self.data[self.INTERACTIONS][user_id][object_name][object_id]) if item["value"] == action.lower()), None)
+
+        if interaction_index is None:
+            return self._register_interaction(user_id, object_name, action, object_id)
+        else:
+            return interaction_index
+
+    def _register_interaction(self, user_id, object_name, action, object_id) -> int:
+        self.data[self.INTERACTIONS][user_id][object_name][object_id].append({
+            "action": action.lower(),
+            "properties": {},
+            "created_at": datetime.datetime.now(datetime.timezone.utc).timestamp()})
+
+        return len(self.data[self.INTERACTIONS][user_id][object_name][object_id]) - 1
+
+    def _update_interaction_attribute(self, user_id, object_name: str, action: str, object_id: str, interaction_attribute: str, attribute_value: any, type: str):
+        index = self._find_or_register_interaction_by_action(
+            user_id=user_id, object_name=object_name, object_id=object_id, action=action)
+
+        if index is None:
+            raise ValueError(
+                "Could not find an interaction with the provided parameters.")
+
+        interaction = self.data[self.INTERACTIONS][user_id][object_name][object_id][index]
+        interaction["properties"][interaction_attribute] = {
+            "type": type,
+            "value": attribute_value
+        }
+
+        self.data[self.INTERACTIONS][user_id][object_name][object_id][index] = interaction
+
+    def register_interaction(self, user_id: any, object_name: str, action: str, object_id: str):
         if (user_id == "" or user_id is None) or (object_name == "" or object_name is None) or (object_id == "" or object_id is None) or (action == "" or action is None):
             raise ValueError(
                 "User Id, Object name, Object id and action must be provided when registering an interaction")
 
-        if user_id not in self.data["interactions"]:
-            self.data["interactions"][user_id] = {}
+        object_name = object_name.lower()
+
+        self._build_interaction_structure(
+            user_id=user_id, object_name=object_name, object_id=object_id)
+        self._register_interaction(
+            user_id=user_id, object_name=object_name, action=action, object_id=object_id)
+
+    def _validate_interaction_fields(self, user_id, object_name: str, action: str, object_id: str, interaction_attribute: str) -> None:
+        if (user_id == "" or user_id is None) or (object_name == "" or object_name is None) or (object_id == "" or object_id is None) or (action == "" or action is None) or (interaction_attribute == '' or interaction_attribute is None):
+            raise ValueError(
+                "User Id, Object name, Object id, action and interaction attribute must be provided when registering an interaction")
+
+    def update_interaction_numerical_field(self, user_id, object_name: str, action: str, object_id: str, interaction_attribute: str, attribute_value: int or float = None):
+        self._validate_interaction_fields(
+            user_id=user_id, object_name=object_name, object_id=object_id, action=action, interaction_attribute=interaction_attribute)
+
+        if not self._is_valid_type(attribute_value, int) and not self._is_valid_type(attribute_value, float):
+            raise ValueError(
+                "Number Interaction Attribute values must be of type [int, float]")
 
         object_name = object_name.lower()
 
-        if object_name not in self.data["interactions"][user_id]:
-            self.data["interactions"][user_id][object_name] = {}
+        self._update_interaction_attribute(
+            user_id=user_id, object_name=object_name, object_id=object_id, action=action, interaction_attribute=interaction_attribute, attribute_value=attribute_value, type="number")
 
-        if object_id not in self.data["interactions"][user_id][object_name]:
-            self.data["interactions"][user_id][object_name][object_id] = []
+    def update_interaction_boolean_field(self, user_id, object_name: str, action: str, object_id: str, interaction_attribute: str, attribute_value: bool = None):
+        self._validate_interaction_fields(
+            user_id=user_id, object_name=object_name,  object_id=object_id, action=action, interaction_attribute=interaction_attribute)
 
-        self.data["interactions"][user_id][object_name][object_id].append({
-            "value": action.lower(),
-            "created_at": datetime.datetime.now(datetime.timezone.utc).timestamp()})
+        if not self._is_valid_type(attribute_value, bool):
+            raise ValueError(
+                "Boolean Interaction Attribute values must be of type [bool]")
+
+        self._update_interaction_attribute(
+            user_id=user_id, object_name=object_name, object_id=object_id, action=action, interaction_attribute=interaction_attribute, attribute_value=attribute_value, type="boolean")
+
+    def update_interaction_date_field(self, user_id, object_name: str, action: str, object_id: str, interaction_attribute: str, attribute_value: str = None):
+        self._validate_interaction_fields(
+            user_id=user_id, object_name=object_name,  object_id=object_id, action=action, interaction_attribute=interaction_attribute)
+
+        if not self._is_valid_type(attribute_value, str):
+            raise ValueError(
+                "Date Interaction Attribute values must be of type [str]")
+
+        try:
+            parse_date_to_format(attribute_value)
+        except:
+            raise ValueError(
+                f"Could not parse datetime string for interaction attribute [{interaction_attribute}]: [{attribute_value}]. Expected date in format dd-mm-YYYY")
+
+        self._update_interaction_attribute(
+            user_id=user_id, object_name=object_name, object_id=object_id, action=action, interaction_attribute=interaction_attribute, attribute_value=attribute_value, type="date")
+
+    def update_interaction_id_field(self, user_id, object_name: str, action: str, object_id: str, interaction_attribute: str, attribute_value: str or int = None):
+        self._validate_interaction_fields(
+            user_id=user_id, object_name=object_name,  object_id=object_id, action=action, interaction_attribute=interaction_attribute)
+
+        if not self._is_valid_type(attribute_value, str) and not self._is_valid_type(attribute_value, int):
+            raise ValueError(
+                "ID Interaction attribute values must be of type [int, str]")
+
+        self._update_interaction_attribute(
+            user_id=user_id, object_name=object_name, object_id=object_id, action=action, interaction_attribute=interaction_attribute, attribute_value=attribute_value, type="id")
 
     def add_label(self, object_name, object_id, label):
         if (object_name == "" or object_name is None) or (object_id == "" or object_id is None):
             raise ValueError("Object name and Object id must be provided")
 
         object_name = object_name.lower()
         if object_name not in self.data or object_id not in self.data[object_name]:
@@ -198,55 +300,67 @@
     def learn_from_data(self):
         if len(self.data) == 0:
             return
 
         instructions_id, current_embeddings_version, instructions = \
             self.orchapi.fetch_instructions()
 
-        self._generate_signatures(instructions)
+        self._generate_embeddings(instructions)
+
         self.orchapi.submit_embeddings(
             self.embeddings, instructions_id, current_embeddings_version)
 
         self._reset_to_initial_state()
 
-    def _generate_signatures(self, instructions):
-        parser = ParseAndExecute(instructions)
+    def _generate_interaction_embeddings(self, parser: Parser) -> dict:
+        user_interactions_embedding = {}
 
-        for object_key in self.data.keys():
+        user_interactions = self.data[self.INTERACTIONS]
 
-            object_data = {}
+        for user_id in user_interactions.keys():
+            value = self.data[self.INTERACTIONS][user_id]
+            parser.feed(value)
+            results = parser.parse(self.INTERACTIONS)
 
-            if object_key == "interactions":
-                user_interactions = self.data[object_key]
-                user_interactions_embedding = {}
-                for user_id in user_interactions.keys():
-                    value = self.data[object_key][user_id]
-                    parser.feed(value)
-                    results = parser.parse(object_key)
-                    if len(results) > 0:
-                        user_interactions_embedding[user_id] = results
+            if len(results) > 0:
+                user_interactions_embedding[user_id] = results
 
-                object_data = user_interactions_embedding
-            else:
-                for object_id in self.data[object_key].keys():
-                    value = self.data[object_key][object_id]
+        return user_interactions_embedding
+
+    def _generate_object_embeddings(self, parser: Parser, object_key: str) -> dict:
+        object_embedding = {}
+
+        for object_id in self.data[object_key].keys():
+            value = self.data[object_key][object_id]
+
+            if len(value) == 0:
+                continue
 
-                    if len(value) == 0:
-                        continue
+            parser.feed(value)
+            results = parser.parse(object_key)
+            if len(results) > 0:
+                object_embedding[object_id] = results
 
-                    parser.feed(value)
-                    results = parser.parse(object_key)
-                    if len(results) > 0:
-                        object_data[object_id] = results
-
-            if len(object_data) > 0:
-                if object_key not in self.embeddings:
-                    self.embeddings[object_key] = {}
+        return object_embedding
+
+    def _generate_embeddings(self, instructions):
+        parser = Parser(instructions)
+
+        for object_key in self.data.keys():
+            embeddings = {}
+
+            if object_key == self.INTERACTIONS:
+                embeddings = self._generate_interaction_embeddings(
+                    parser)
+            else:
+                embeddings = self._generate_object_embeddings(
+                    parser, object_key)
 
-                self.embeddings[object_key] = object_data
+            if len(embeddings) > 0:
+                self.embeddings[object_key] = embeddings
 
     def _reset_to_initial_state(self):
         self.data = {
             "user": {},
             "interactions": {}
         }
         self.embeddings = {}
```

### Comparing `beginai-2.0.0/beginai/exec/execute_compute.py` & `beginai-2.0.1/beginai/exec/execute_compute.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/exec/remote_compute.py` & `beginai-2.0.1/beginai/exec/remote_compute.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/orchapi/api.py` & `beginai-2.0.1/beginai/orchapi/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,40 +20,51 @@
     interacts with orchestrator end points.
     """
     def __init__(self):
         self.project_id = None
         self.compute_group_id = None
         self.host = None
         self.token = None
+        self.debug = False
 
     def configure_orch_connection(self, host, port = None):
         if port is None:
             self.host = host
         else:
             self.host = "{}:{}".format(host, port)
 
+    def set_debug(self, debug=False):
+        if self.host == 'http://localhost:9999':
+            self.debug = debug
+
     def set_app_id_and_license_key(self, license_key, app_id):
         self.app_id = app_id
         self.license_key = license_key
 
     def _get_oauth_header(self):
 
+        if self.debug == True:
+            return {
+                'appid': self.app_id
+            }
+
         data = {
             'app_id': self.app_id,
             'license_key': self.license_key
         }
 
         res = requests.post(self.host + _URL.AUTH.value, json = data)
 
         if res.status_code == 401:
             raise ValueError('App ID/License Key are invalid, please check your application credentials')
         
         access_token = res.json()['result']['access_token']
         return {
-            'Authorization': f'Bearer {access_token["itk"]}'
+            'Authorization': f'Bearer {access_token["itk"]}',
+            'appid': self.app_id
         }
     
     def _send_post(self, uri, msg):
 
         headers = self._get_oauth_header()        
 
         res = requests.post(self.host + uri, json = msg, headers=headers)
```

### Comparing `beginai-2.0.0/beginai/tests/exec/embeddings/instructions/boolean_test.py` & `beginai-2.0.1/beginai/tests/exec/embeddings/instructions/boolean_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/tests/exec/embeddings/instructions/category_test.py` & `beginai-2.0.1/beginai/tests/exec/embeddings/instructions/category_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/tests/exec/embeddings/instructions/date_test.py` & `beginai-2.0.1/beginai/tests/exec/embeddings/instructions/date_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/tests/exec/embeddings/instructions/interaction_test.py` & `beginai-2.0.1/beginai/tests/exec/embeddings/instructions/interaction_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/tests/exec/embeddings/instructions/location_test.py` & `beginai-2.0.1/beginai/tests/exec/embeddings/instructions/location_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/tests/exec/embeddings/instructions/number_test.py` & `beginai-2.0.1/beginai/tests/exec/embeddings/instructions/number_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/tests/exec/embeddings/instructions/text_test.py` & `beginai-2.0.1/beginai/tests/exec/embeddings/instructions/text_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/tests/exec/embeddings/mock_service.py` & `beginai-2.0.1/beginai/tests/exec/embeddings/mock_service.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,136 +21,174 @@
 class _FakeOrchAPI(OrchAPI):
 
     def fetch_instructions(self):
         instructions_id = 1
         version_number = 0
         instructions_list = {
             "instructions": {
-                "user": [
-                    {
-                        "instruct": "Age",
+                "objects": {
+                    "user": [
+                        {
+                            "instruct": "Age",
+                            "complexity": 1,
+                            "params": {},
+                            "f_id": "dateOfBirth",
+                        },
+                        {
+                            "_chains": [
+                                [
+                                    {
+                                        "instruct": "Age",
+                                        "complexity": 1,
+                                        "params": {
+
+                                        },
+                                        "order": 1
+                                    },
+                                    {
+                                        "instruct": "Slice",
+                                        "complexity": 1,
+                                        "params": {
+                                            "minv": 10,
+                                            "maxv": 100,
+                                            "num_slices": 10,
+                                            "skip_masking": False
+                                        },
+                                        "order": 2
+                                    }
+                                ]
+                            ],
+                            "f_id": "dateOfBirth",
+                        },
+                        {
+                            "instruct": "Slice",
+                            "complexity": 1,
+                            "params": {
+                                "minv": 0,
+                                "maxv": 255,
+                                "num_slices": 10,
+                                "skip_masking": False
+                            },
+                            "f_id": "numberField",
+                        },
+                        {
+                            "instruct": "Length",
+                            "complexity": 1,
+                            "params": {
+
+                            },
+                            "f_id": "textField",
+                        }
+                    ],
+                    "product": [{
+                        "instruct": "Length",
                         "complexity": 1,
                         "params": {
 
                         },
-                        "f_id": "dateOfBirth",
+                        "f_id": "description",
+                    },
+                        {
+                            "instruct": "Slice",
+                            "complexity": 1,
+                            "params": {
+                                "minv": 0,
+                                "maxv": 255,
+                                "num_slices": 10,
+                                "skip_masking": False
+                            },
+                            "f_id": "randomNumber",
+                    },
+                        {
+                            "instruct": "Age",
+                            "complexity": 1,
+                            "params": {
+
+                            },
+                            "f_id": "publishedDate",
+                    },
+                        {
+                            "instruct": "Slice",
+                            "complexity": 1,
+                            "params": {
+                                "minv": 0,
+                                "maxv": 255,
+                                "num_slices": 10,
+                                "skip_masking": True
+                            },
+                            "f_id": "randomnumberskippingmask",
+                    }
+                    ],
+                },
+                "interactions": {
+                    "noembedding": {
+                        "actions": ["just_action"],
+                        "instructions": {}
                     },
-                    {
-                        "_chains": [
-                            [
+                    "user": {
+                        "actions": ["followed", "report", "dosomething"],
+                        "instructions": {
+                            "followed": [
                                 {
                                     "instruct": "Age",
                                     "complexity": 1,
                                     "params": {
-
                                     },
-                                    "order": 1
-                                },
+                                    "f_id": "date",
+                                }
+                            ],
+                            "report": [
                                 {
-                                    "instruct": "Slice",
+                                    "instruct": "Age",
                                     "complexity": 1,
                                     "params": {
-                                        "minv": 10,
-                                        "maxv": 100,
-                                        "num_slices": 10,
-                                        "skip_masking": False
                                     },
-                                    "order": 2
+                                    "f_id": "date",
                                 }
                             ]
-                        ],
-                        "f_id": "dateOfBirth",
-                    },
-                    {
-                        "instruct": "Slice",
-                        "complexity": 1,
-                        "params": {
-                            "minv": 0,
-                            "maxv": 255,
-                            "num_slices": 10,
-                            "skip_masking": False
-                        },
-                        "f_id": "numberField",
-                    },
-                    {
-                        "instruct": "Length",
-                        "complexity": 1,
-                        "params": {
-
-                        },
-                        "f_id": "textField",
-                    }
-                ],
-                "product": [{
-                    "instruct": "Length",
-                    "complexity": 1,
-                    "params": {
-
-                    },
-                    "f_id": "description",
-                },
-                    {
-                        "instruct": "Slice",
-                        "complexity": 1,
-                        "params": {
-                            "minv": 0,
-                            "maxv": 255,
-                            "num_slices": 10,
-                            "skip_masking": False
-                        },
-                        "f_id": "randomNumber",
-                },
-                    {
-                        "instruct": "Age",
-                        "complexity": 1,
-                        "params": {
-
-                        },
-                        "f_id": "publishedDate",
-                },
-                    {
-                        "instruct": "Slice",
-                        "complexity": 1,
-                        "params": {
-                            "minv": 0,
-                            "maxv": 255,
-                            "num_slices": 10,
-                            "skip_masking": True
-                        },
-                        "f_id": "randomnumberskippingmask",
-                }
-                ],
-                "interactions": [{
-                    "instruct": "InteractionEncoding",
-                    "complexity": 1,
-                    "params": {
-                        "sequence_map": {
-                            "like": 5,
-                            "dislike": 1,
-                            "comment": 4,
-                            "_GB_EMPTY": 0.00011
                         }
                     },
-                    "higher_order": 1,
-                    "_with_object": "product"
+                    "product": {
+                        "actions": ["like", "dislike", "comment"],
+                        "instructions": {
+                            "like": [
+                                {
+                                    "instruct": "Age",
+                                    "complexity": 1,
+                                    "params": {
+                                    },
+                                    "f_id": "date",
+                                }
+                            ],
+                            "dislike": [
+                                {
+                                    "instruct": "Age",
+                                    "complexity": 1,
+                                    "params": {
+                                    },
+                                    "f_id": "date",
+                                }
+                            ],
+                            "comment": [
+                                {
+                                    "instruct": "Length",
+                                    "complexity": 1,
+                                    "params": {},
+                                    "f_id": "commentLength",
+                                },
+                                {
+                                    "instruct": "Age",
+                                    "complexity": 1,
+                                    "params": {
+                                    },
+                                    "f_id": "date",
+                                }
+                            ]
+                        }}
                 },
-                    {
-                        "instruct": "InteractionEncoding",
-                        "complexity": 1,
-                        "params": {
-                            "sequence_map": {
-                                "followed": 5,
-                                "report": 2,
-                                "_GB_EMPTY": 0.00011
-                            }
-                        },
-                        "higher_order": 2,
-                        "_with_object": "user"
-                }
-                ]
             },
             "tokenize": {
                 "user": [
                     "name",
                     "lastName"
                 ],
                 "product": [
@@ -163,19 +201,28 @@
                 "product": ["fiction", "comedy", "mystery"]
             },
             "identifiers": {
                 "user": ["user_specific_id", "another_user_specific_id"],
                 "product": ['product_specific_id']
             },
             "embedding_template": {
-                "user": ["dateOfBirth", "chain_instruction__Age__user__dateOfBirth", "chain_instruction__Slice__user__dateOfBirth", "numberField", "textField"],
-                "product": ["description", "randomNumber", "publishedDate", "randomnumberskippingmask"]
-            },
-            "raw_interactions": {
-                "product": ["LIKE", "DISLIKE"],
-                "user": ["FOLLOWED", "REPORT"]
+                "objects": {
+                    "user": ["dateOfBirth", "chain_instruction__Age__user__dateOfBirth", "chain_instruction__Slice__user__dateOfBirth", "numberField", "textField"],
+                    "product": ["description", "randomNumber", "publishedDate", "randomnumberskippingmask"]
+                },
+                "interactions": {
+                    "user": {
+                        "followed": ["date"],
+                        "report": ["date"]
+                    },
+                    "product": {
+                        "like": ["date"],
+                        "dislike": ["date"],
+                        "comment": ["date", "commentLength"]
+                    }
+                }
             }
         }
         return instructions_id, version_number, instructions_list
 
     def submit_embeddings(self, embeddings, instruction_id, version_number):
         self.embeddings = embeddings
```

### Comparing `beginai-2.0.0/beginai/tests/exec/embeddings/worker_methods_validation_interaction_test.py` & `beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_interaction_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .mock_service import BeginWorkerMock
 from freezegun import freeze_time
 
 APP_ID = 1
 LICENSE_KEY = 10
+USER_ID = 123
 
 
 def test_register_interaction_without_user_id():
     bw = BeginWorkerMock(APP_ID, LICENSE_KEY)
     try:
         bw.register_interaction(
             user_id='', object_name='', object_id=1, action='like')
@@ -23,15 +24,15 @@
         assert True
 
 
 def test_register_interaction_without_object_id():
     bw = BeginWorkerMock(APP_ID, LICENSE_KEY)
     try:
         bw.register_interaction(
-            user_id=1, object_name='product', object_id=None, action='like')
+            user_id=1, object_name='product', object_id="", action='like')
     except ValueError:
         assert True
 
 
 def test_register_interaction_without_action_id():
     bw = BeginWorkerMock(APP_ID, LICENSE_KEY)
     try:
@@ -49,25 +50,47 @@
     user_id = 1
 
     bw.register_interaction(user_id, object_name, 'like', object_id)
     bw.register_interaction(user_id, object_name, 'dislike', object_id)
 
     results = bw.get_data().get('interactions').get(user_id).get(object_name)
 
-    assert results == {object_id: [{'value': 'like', 'created_at': 1621123200.0}, {
-        'value': 'dislike', 'created_at': 1621123200.0}]}
+    assert results == {object_id: [
+        {
+            'action': 'like',
+            'properties': {},
+            'created_at': 1621123200.0},
+        {
+            'action': 'dislike',
+            'properties': {},
+            'created_at': 1621123200.0
+        }]}
 
 
 @freeze_time("2021-05-16")
 def test_register_interaction_with_different_product_id():
     bw = BeginWorkerMock(APP_ID, LICENSE_KEY)
     object_name = "product"
     object_id_one = 10
     object_id_two = 20
     user_id = 1
 
     bw.register_interaction(user_id, object_name, 'LIKE', object_id_one)
     bw.register_interaction(user_id, object_name, 'DISLIKE', object_id_two)
 
     results = bw.get_data().get('interactions').get(user_id).get(object_name)
-    assert results == {object_id_one: [
-        {'value': 'like', 'created_at': 1621123200.0}], object_id_two: [{'value': 'dislike', 'created_at': 1621123200.0}]}
+    assert results == {
+        object_id_one: [
+            {
+                'action': 'like',
+                'properties': {},
+                'created_at': 1621123200.0
+            }
+        ],
+        object_id_two: [
+            {
+                'action': 'dislike',
+                'properties': {},
+                'created_at': 1621123200.0
+            }
+        ]
+    }
```

### Comparing `beginai-2.0.0/beginai/tests/exec/embeddings/worker_methods_validation_labels_test.py` & `beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_labels_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/tests/exec/embeddings/worker_methods_validation_object_test.py` & `beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_object_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/tests/exec/embeddings/worker_methods_validation_user_test.py` & `beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_user_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai/utils/syft.py` & `beginai-2.0.1/beginai/utils/syft.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.0/beginai.egg-info/PKG-INFO` & `beginai-2.0.1/beginai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beginai
-Version: 2.0.0
+Version: 2.0.1
 Summary: A library to interact with Begin AI platform in order to build personalisation algorithms.
 Home-page: https://docs.begin.ai
 Author: Begin AI Research & Engineering
 Author-email: engineering@begin.ai
 License: Proprietary
 Description: 
                 This is Begin AI python SDK for both batch processing and application integration.
```

### Comparing `beginai-2.0.0/beginai.egg-info/SOURCES.txt` & `beginai-2.0.1/beginai.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,38 +20,39 @@
 beginai/exec/embeddings/instructions/__init__.py
 beginai/exec/embeddings/instructions/boolean.py
 beginai/exec/embeddings/instructions/category.py
 beginai/exec/embeddings/instructions/date.py
 beginai/exec/embeddings/instructions/interaction.py
 beginai/exec/embeddings/instructions/location.py
 beginai/exec/embeddings/instructions/number.py
-beginai/exec/embeddings/instructions/parse_and_execute.py
+beginai/exec/embeddings/instructions/parser.py
 beginai/exec/embeddings/instructions/text.py
 beginai/exec/embeddings/instructions/utils.py
 beginai/exec/embeddings/instructions/deep_text/__init__.py
 beginai/exec/embeddings/instructions/deep_text/bpe.py
 beginai/orchapi/__init__.py
 beginai/orchapi/api.py
 beginai/storage/__init__.py
 beginai/storage/s3.py
 beginai/storage/sqllite.py
 beginai/tests/__init__.py
 beginai/tests/exec/__init__.py
 beginai/tests/exec/embeddings/__init__.py
 beginai/tests/exec/embeddings/mock_service.py
+beginai/tests/exec/embeddings/worker_methods_validation_interaction_attributes_test.py
 beginai/tests/exec/embeddings/worker_methods_validation_interaction_test.py
 beginai/tests/exec/embeddings/worker_methods_validation_labels_test.py
 beginai/tests/exec/embeddings/worker_methods_validation_object_test.py
 beginai/tests/exec/embeddings/worker_methods_validation_user_test.py
 beginai/tests/exec/embeddings/worker_test.py
 beginai/tests/exec/embeddings/instructions/__init__.py
 beginai/tests/exec/embeddings/instructions/boolean_test.py
 beginai/tests/exec/embeddings/instructions/category_test.py
 beginai/tests/exec/embeddings/instructions/date_test.py
 beginai/tests/exec/embeddings/instructions/interaction_test.py
 beginai/tests/exec/embeddings/instructions/location_test.py
 beginai/tests/exec/embeddings/instructions/number_test.py
-beginai/tests/exec/embeddings/instructions/parse_and_execute_test.py
+beginai/tests/exec/embeddings/instructions/parser_test.py
 beginai/tests/exec/embeddings/instructions/text_test.py
 beginai/utils/__init__.py
 beginai/utils/date.py
 beginai/utils/syft.py
```

### Comparing `beginai-2.0.0/setup.py` & `beginai-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 REQ_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "pip-dep")
 core_reqs, core_dependency_links = get_requirements(os.path.join(REQ_DIR, "requirements.txt"))
 
 
 if __name__ == "__main__":
     setup(
         name="beginai",
-        version="2.0.0",
+        version="2.0.1",
         author="Begin AI Research & Engineering",
         author_email="engineering@begin.ai",
         description="A library to interact with Begin AI platform in order to build personalisation algorithms.",
         long_description="""
         This is Begin AI python SDK for both batch processing and application integration. 
         It can be used to integrate applications with Begin.ai orchestration platform to deliver applications with
         personalisation algorithms to do:
```

