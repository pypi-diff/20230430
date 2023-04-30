# Comparing `tmp/torchtnt-0.0.7.tar.gz` & `tmp/torchtnt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchtnt-0.0.7.tar", last modified: Thu Mar  2 20:51:20 2023, max compression
+gzip compressed data, was "dist/torchtnt-0.1.0.tar", last modified: Sun Apr 30 00:51:10 2023, max compression
```

## Comparing `torchtnt-0.0.7.tar` & `torchtnt-0.1.0.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:51:20.000000 torchtnt-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-02 20:50:24.000000 torchtnt-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-03-02 20:51:20.000000 torchtnt-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-02 20:50:24.000000 torchtnt-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-02 20:50:24.000000 torchtnt-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 20:51:20.000000 torchtnt-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-03-02 20:50:24.000000 torchtnt-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:51:20.000000 torchtnt-0.0.7/torchtnt/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:51:20.000000 torchtnt-0.0.7/torchtnt/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/auto_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:51:20.000000 torchtnt-0.0.7/torchtnt/framework/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/callbacks/base_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/callbacks/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/callbacks/learning_rate_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/callbacks/module_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/callbacks/pytorch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/callbacks/system_resources_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/callbacks/torchsnapshot_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/callbacks/tqdm_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:51:20.000000 torchtnt-0.0.7/torchtnt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:51:20.000000 torchtnt-0.0.7/torchtnt/utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/data/data_prefetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/data/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/data/multi_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/early_stop_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/fsspec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:51:20.000000 torchtnt-0.0.7/torchtnt/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/loggers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/loggers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/loggers/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/loggers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/loggers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/oom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/rank_zero_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-03-02 20:50:24.000000 torchtnt-0.0.7/torchtnt/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:51:20.000000 torchtnt-0.0.7/torchtnt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-03-02 20:51:20.000000 torchtnt-0.0.7/torchtnt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-03-02 20:51:20.000000 torchtnt-0.0.7/torchtnt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 20:51:20.000000 torchtnt-0.0.7/torchtnt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-02 20:51:20.000000 torchtnt-0.0.7/torchtnt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-02 20:51:20.000000 torchtnt-0.0.7/torchtnt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 20:51:20.000000 torchtnt-0.0.7/torchtnt.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:51:10.000000 torchtnt-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-30 00:49:44.000000 torchtnt-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-30 00:51:10.000000 torchtnt-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-30 00:49:44.000000 torchtnt-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-30 00:49:44.000000 torchtnt-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 00:51:10.000000 torchtnt-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-30 00:49:44.000000 torchtnt-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:51:10.000000 torchtnt-0.1.0/torchtnt/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:51:10.000000 torchtnt-0.1.0/torchtnt/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28872 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/auto_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:51:10.000000 torchtnt-0.1.0/torchtnt/framework/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/callbacks/base_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/callbacks/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/callbacks/learning_rate_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/callbacks/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/callbacks/pytorch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/callbacks/system_resources_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10455 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/callbacks/torchsnapshot_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/callbacks/tqdm_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/callbacks/train_progress_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:51:10.000000 torchtnt-0.1.0/torchtnt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:51:10.000000 torchtnt-0.1.0/torchtnt/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/data/data_prefetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/data/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/data/multi_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/early_stop_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/fsspec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:51:10.000000 torchtnt-0.1.0/torchtnt/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/loggers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/loggers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/loggers/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/loggers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/loggers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/oom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/rank_zero_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-30 00:49:44.000000 torchtnt-0.1.0/torchtnt/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:51:10.000000 torchtnt-0.1.0/torchtnt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-30 00:51:10.000000 torchtnt-0.1.0/torchtnt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-30 00:51:10.000000 torchtnt-0.1.0/torchtnt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 00:51:10.000000 torchtnt-0.1.0/torchtnt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-30 00:51:10.000000 torchtnt-0.1.0/torchtnt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-30 00:51:10.000000 torchtnt-0.1.0/torchtnt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 00:51:10.000000 torchtnt-0.1.0/torchtnt.egg-info/zip-safe
```

### Comparing `torchtnt-0.0.7/LICENSE` & `torchtnt-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/PKG-INFO` & `torchtnt-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt
-Version: 0.0.7
+Version: 0.1.0
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -23,28 +23,34 @@
 ==========
 
 **TNT** is a library for PyTorch **t**rai**n**ing **t**ools and utilities.
 
 <p align="center">
 <a href="https://github.com/pytorch/tnt/actions?query=branch%3Amaster"><img src="https://img.shields.io/github/actions/workflow/status/pytorch/tnt/test.yml?branch=master" alt="build status"></a>
 <a href="https://pypi.org/project/torchtnt"><img src="https://img.shields.io/pypi/v/torchtnt" alt="pypi version"></a>
+<a href="https://anaconda.org/conda-forge/torchtnt"><img src="https://img.shields.io/conda/vn/conda-forge/torchtnt" alt="pypi version"></a>
 <a href="https://pypi.org/project/torchtnt-nightly"><img src="https://img.shields.io/pypi/v/torchtnt-nightly?label=nightly" alt="pypi nightly version"></a>
 <a href="https://codecov.io/gh/pytorch/tnt"><img src="https://codecov.io/gh/pytorch/tnt/branch/master/graph/badge.svg?token=DR67Q6T7YF" alt="codecov"></a>
 <a href="https://github.com/pytorch/tnt/blob/master/LICENSE"><img src="https://img.shields.io/pypi/l/torchtnt" alt="bsd license"></a>
 <a href="https://pytorch.org/tnt/"><img src="https://img.shields.io/badge/dynamic/json.svg?label=docs&url=https%3A%2F%2Fpypi.org%2Fpypi%2Ftorchtnt%2Fjson&query=%24.info.version&colorB=brightgreen&prefix=v" alt="documentation status"></a>
 </div>
 
 
 ## Installation
 
-TNT can be installed with pip. To do so, run:
+TNT can be installed with pip:
 
 ```buildoutcfg
 pip install torchtnt
 ```
+Or, alternatively, via conda:
+
+```buildoutcfg
+conda install -c conda-forge torchtnt
+```
 
 If you run into issues, make sure that Pytorch is installed first.
 
 You can also install the latest version from master. Just run:
 
 ```buildoutcfg
 pip install git+https://github.com/pytorch/tnt.git@master
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: torchtnt Version: 0.0.7 Summary: A lightweight
+Metadata-Version: 2.1 Name: torchtnt Version: 0.1.0 Summary: A lightweight
 library for PyTorch training tools and utilities Home-page: https://github.com/
 pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com License: BSD-
 3 Keywords: pytorch,torch,training,tools,utilities Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev License-File: LICENSE TNT
 ========== **TNT** is a library for PyTorch **t**rai**n**ing **t**ools and
 utilities.
- [build_status] [pypi_version] [pypi_nightly_version] [codecov] [bsd_license]
-                            [documentation_status]
-## Installation TNT can be installed with pip. To do so, run: ```buildoutcfg
-pip install torchtnt ``` If you run into issues, make sure that Pytorch is
+[build_status] [pypi_version] [pypi_version] [pypi_nightly_version] [codecov]
+                     [bsd_license] [documentation_status]
+## Installation TNT can be installed with pip: ```buildoutcfg pip install
+torchtnt ``` Or, alternatively, via conda: ```buildoutcfg conda install -
+c conda-forge torchtnt ``` If you run into issues, make sure that Pytorch is
 installed first. You can also install the latest version from master. Just run:
 ```buildoutcfg pip install git+https://github.com/pytorch/tnt.git@master ``` To
 update to the latest version from master: ```buildoutcfg pip install --upgrade
 git+https://github.com/pytorch/tnt.git@master ```
```

### Comparing `torchtnt-0.0.7/README.md` & `torchtnt-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,34 @@
 ==========
 
 **TNT** is a library for PyTorch **t**rai**n**ing **t**ools and utilities.
 
 <p align="center">
 <a href="https://github.com/pytorch/tnt/actions?query=branch%3Amaster"><img src="https://img.shields.io/github/actions/workflow/status/pytorch/tnt/test.yml?branch=master" alt="build status"></a>
 <a href="https://pypi.org/project/torchtnt"><img src="https://img.shields.io/pypi/v/torchtnt" alt="pypi version"></a>
+<a href="https://anaconda.org/conda-forge/torchtnt"><img src="https://img.shields.io/conda/vn/conda-forge/torchtnt" alt="pypi version"></a>
 <a href="https://pypi.org/project/torchtnt-nightly"><img src="https://img.shields.io/pypi/v/torchtnt-nightly?label=nightly" alt="pypi nightly version"></a>
 <a href="https://codecov.io/gh/pytorch/tnt"><img src="https://codecov.io/gh/pytorch/tnt/branch/master/graph/badge.svg?token=DR67Q6T7YF" alt="codecov"></a>
 <a href="https://github.com/pytorch/tnt/blob/master/LICENSE"><img src="https://img.shields.io/pypi/l/torchtnt" alt="bsd license"></a>
 <a href="https://pytorch.org/tnt/"><img src="https://img.shields.io/badge/dynamic/json.svg?label=docs&url=https%3A%2F%2Fpypi.org%2Fpypi%2Ftorchtnt%2Fjson&query=%24.info.version&colorB=brightgreen&prefix=v" alt="documentation status"></a>
 </div>
 
 
 ## Installation
 
-TNT can be installed with pip. To do so, run:
+TNT can be installed with pip:
 
 ```buildoutcfg
 pip install torchtnt
 ```
+Or, alternatively, via conda:
+
+```buildoutcfg
+conda install -c conda-forge torchtnt
+```
 
 If you run into issues, make sure that Pytorch is installed first.
 
 You can also install the latest version from master. Just run:
 
 ```buildoutcfg
 pip install git+https://github.com/pytorch/tnt.git@master
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 TNT ========== **TNT** is a library for PyTorch **t**rai**n**ing **t**ools and
 utilities.
- [build_status] [pypi_version] [pypi_nightly_version] [codecov] [bsd_license]
-                            [documentation_status]
-## Installation TNT can be installed with pip. To do so, run: ```buildoutcfg
-pip install torchtnt ``` If you run into issues, make sure that Pytorch is
+[build_status] [pypi_version] [pypi_version] [pypi_nightly_version] [codecov]
+                     [bsd_license] [documentation_status]
+## Installation TNT can be installed with pip: ```buildoutcfg pip install
+torchtnt ``` Or, alternatively, via conda: ```buildoutcfg conda install -
+c conda-forge torchtnt ``` If you run into issues, make sure that Pytorch is
 installed first. You can also install the latest version from master. Just run:
 ```buildoutcfg pip install git+https://github.com/pytorch/tnt.git@master ``` To
 update to the latest version from master: ```buildoutcfg pip install --upgrade
 git+https://github.com/pytorch/tnt.git@master ```
```

### Comparing `torchtnt-0.0.7/setup.py` & `torchtnt-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/framework/__init__.py` & `torchtnt-0.1.0/torchtnt/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/framework/_test_utils.py` & `torchtnt-0.1.0/torchtnt/framework/_test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/framework/auto_unit.py` & `torchtnt-0.1.0/torchtnt/framework/auto_unit.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,63 +5,97 @@
 # LICENSE file in the root directory of this source tree.
 
 # ignore errors due to `Any` type
 # pyre-ignore-all-errors[2]
 # pyre-ignore-all-errors[3]
 
 import contextlib
-from abc import ABC, abstractmethod
+from abc import ABCMeta, abstractmethod
 from dataclasses import asdict, dataclass
-from typing import Any, Callable, Optional, Tuple, TypeVar, Union
+from typing import Any, Callable, Iterable, Iterator, Optional, Tuple, TypeVar, Union
 
 import torch
+import torch.distributed as dist
+
 from pyre_extensions import none_throws
 from torch.cuda.amp import GradScaler
 from torch.distributed import ProcessGroup
 from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
+from torch.distributed.fsdp.fully_sharded_data_parallel import (
+    BackwardPrefetch,
+    CPUOffload,
+    MixedPrecision,
+    ShardingStrategy,
+)
 from torch.nn.parallel import DistributedDataParallel as DDP
 from torch.optim.swa_utils import AveragedModel, SWALR
-from torchtnt.framework.state import EntryPoint, State
+from torch.profiler import record_function
+from torchtnt.framework.state import ActivePhase, State
 from torchtnt.framework.unit import EvalUnit, PredictUnit, TrainUnit
+from torchtnt.framework.utils import _is_fsdp_module, get_current_progress, StatefulInt
 from torchtnt.utils import (
-    copy_data_to_device,
     init_from_env,
     is_torch_version_geq_1_12,
     TLRScheduler,
     transfer_batch_norm_stats,
     transfer_weights,
 )
+from torchtnt.utils.device import copy_data_to_device, record_data_in_stream
 from torchtnt.utils.rank_zero_log import rank_zero_warn
 from torchtnt.utils.version import is_torch_version_ge_1_13_1
 from typing_extensions import Literal
 
 TSWA_avg_fn = Callable[[torch.Tensor, torch.Tensor, int], torch.Tensor]
 
 
 @dataclass
 class Strategy:
-    """Dataclass representing the parallelization strategy for the AutoParallelUnit"""
+    """Dataclass representing the parallelization strategy for the AutoUnit"""
 
     pass
 
 
 @dataclass
 class DDPStrategy(Strategy):
-    """Dataclass representing the `DistributedDataParallel <https://pytorch.org/docs/stable/generated/torch.nn.parallel.DistributedDataParallel.html>`_ strategy"""
+    """
+    Dataclass representing the `DistributedDataParallel <https://pytorch.org/docs/stable/generated/torch.nn.parallel.DistributedDataParallel.html>`_ strategy.
+    Includes params for registering `DDP communication hooks <https://pytorch.org/docs/stable/ddp_comm_hooks.html>`_.
+    """
 
     output_device: Optional[Union[int, torch.device]] = None
     dim: int = 0
     broadcast_buffers: bool = True
     process_group: Optional[ProcessGroup] = None
     bucket_cap_mb: int = 25
     find_unused_parameters: bool = False
     check_reduction: bool = False
     gradient_as_bucket_view: bool = False
     static_graph: bool = False
 
+    # DDP Comm Hook params
+    comm_state: Optional[object] = None
+    comm_hook: Optional[
+        Callable[[object, dist.GradBucket], torch.futures.Future[torch.Tensor]]
+    ] = None
+
+
+@dataclass
+class FSDPStrategy(Strategy):
+    """Dataclass representing the `FullyShardedDataParallel <https://pytorch.org/docs/stable/fsdp.html>`_ strategy"""
+
+    process_group: Optional[ProcessGroup] = None
+    sharding_strategy: Optional[ShardingStrategy] = None
+    cpu_offload: Optional[CPUOffload] = None
+    auto_wrap_policy: Optional[Callable[[torch.nn.Module, bool, int], bool]] = None
+    backward_prefetch: Optional[BackwardPrefetch] = None
+    ignored_modules: Optional[Iterable[torch.nn.Module]] = None
+    sync_module_states: bool = False
+    forward_prefetch: bool = False
+    limit_all_gathers: bool = False
+
 
 @dataclass
 class SWAParams:
     """
     Dataclass to store parameters for stochastic weight averaging.
 
     Args:
@@ -92,15 +126,53 @@
 
 
 # pyre-ignore: Invalid type parameters [24]
 TSelf = TypeVar("TSelf", bound="AutoUnit")
 TData = TypeVar("TData")
 
 
-class AutoUnit(TrainUnit[TData], EvalUnit[TData], PredictUnit[Any], ABC):
+class _ConfigureOptimizersCaller(ABCMeta):
+    def __call__(self, *args, **kwargs):
+        x = super().__call__(*args, **kwargs)
+        x.optimizer = None
+        x.lr_scheduler = None
+        x.swa_model = None
+        x.swa_scheduler = None
+
+        if x.training:
+            x.optimizer, x.lr_scheduler = x.configure_optimizers_and_lr_scheduler(
+                x.module
+            )
+
+            if x.swa_params:
+                if not x.swa_params.avg_fn:
+                    # pyre-ignore: Unexpected keyword [28]
+                    x.swa_model = AveragedModel(x.module, use_buffers=True)
+                else:
+                    # pyre-ignore: Unexpected keyword [28]
+                    x.swa_model = AveragedModel(
+                        x.module, avg_fn=x.swa_params.avg_fn, use_buffers=True
+                    )
+
+                x.swa_scheduler = SWALR(
+                    optimizer=x.optimizer,
+                    swa_lr=x.swa_params.lr,
+                    anneal_epochs=x.swa_params.anneal_epochs,
+                    anneal_strategy=x.swa_params.anneal_strategy,
+                )
+
+        return x
+
+
+class AutoUnit(
+    TrainUnit[TData],
+    EvalUnit[TData],
+    PredictUnit[Any],
+    metaclass=_ConfigureOptimizersCaller,
+):
     """
     The AutoUnit is a convenience for users who are training with stochastic gradient descent and would like to have model optimization
     and data parallel replication handled for them.
     The AutoUnit subclasses :class:`~torchtnt.framework.unit.TrainUnit`, :class:`~torchtnt.framework.unit.EvalUnit`, and :class:`~torchtnt.framework.unit.PredictUnit`,
     and implements the ``train_step``, ``eval_step``, and ``predict_step`` methods for the user.
 
     For the ``train_step`` it runs:
@@ -109,107 +181,137 @@
     - backward pass
     - optimizer step
 
     For the ``eval_step`` it only runs forward and loss computation.
 
     For the ``predict_step`` it only runs forward.
 
-    To benefit from the AutoUnit, the user must subclass it and implement the ``compute_loss`` method, and optionally the ``update_metrics`` and ``log_metrics`` methods.
+    To benefit from the AutoUnit, the user must subclass it and implement the ``compute_loss`` and ``configure_optimizers_and_lr_scheduler`` methods.
+    Additionally, the AutoUnit offers these optional hooks:
+
+    - ``on_train_step_end``
+    - ``on_eval_step_end``
+    - ``on_predict_step_end``
+
     Then use with the :py:func:`~torchtnt.framework.train`, :py:func:`~torchtnt.framework.evaluate`, :py:func:`~torchtnt.framework.predict`, or :py:func:`~torchtnt.framework.fit` entry point as normal.
 
     For more advanced customization, directly use the :class:`~torchtnt.framework.unit.TrainUnit`, :class:`~torchtnt.framework.unit.EvalUnit`, and :class:`~torchtnt.framework.unit.PredictUnit` interfaces.
 
     Args:
         module: module to be used during training.
         device: the device to be used.
-        strategy: the data parallelization strategy to be used
+        strategy: the data parallelization strategy to be used. if a string, must be one of ``ddp`` or ``fsdp``.
         step_lr_interval: whether to step lr_scheduler every step or every epoch. Defaults to every epoch.
-        log_frequency_steps: how often to log in terms of steps (parameter updates) during training.
         precision: the precision to use in training, as either a string or a torch.dtype.
         gradient_accumulation_steps: how many batches to accumulate gradients over.
         detect_anomaly: whether to enable anomaly detection for the autograd engine https://pytorch.org/docs/stable/autograd.html#anomaly-detection
         clip_grad_norm: max norm of the gradients for clipping https://pytorch.org/docs/stable/generated/torch.nn.utils.clip_grad_norm_.html
         clip_grad_value: max value of the gradients for clipping https://pytorch.org/docs/stable/generated/torch.nn.utils.clip_grad_value_.html
         swa_params: params for stochastic weight averaging https://pytorch.org/docs/stable/optim.html#stochastic-weight-averaging
-        torchdynamo_params: params for TorchDynamo https://pytorch.org/docs/master/dynamo/
+        torchdynamo_params: params for TorchDynamo https://pytorch.org/docs/stable/dynamo/index.html
+        training: if True, the optimizer and optionally LR scheduler will be created after the class is initialized.
+
+            Note:
+                Stochastic Weight Averaging is currently not supported with the FSDP strategy.
 
             Note:
                 TorchDynamo support is only available in PyTorch 2.0 or higher.
     """
 
     def __init__(
         self,
         *,
         module: torch.nn.Module,
         device: Optional[torch.device] = None,
-        strategy: Optional[Strategy] = None,
+        strategy: Optional[Union[Strategy, str]] = None,
         step_lr_interval: Literal["step", "epoch"] = "epoch",
-        log_frequency_steps: int = 1000,
         precision: Optional[Union[str, torch.dtype]] = None,
         gradient_accumulation_steps: int = 1,
-        detect_anomaly: bool = False,
+        detect_anomaly: Optional[bool] = None,
         clip_grad_norm: Optional[float] = None,
         clip_grad_value: Optional[float] = None,
         swa_params: Optional[SWAParams] = None,
         torchdynamo_params: Optional[TorchDynamoParams] = None,
+        training: bool = True,
     ) -> None:
         super().__init__()
         self.device: torch.device = device or init_from_env()
+        module = module.to(self.device)  # move module to device
+
+        self.precision: Optional[torch.dtype]
+        if isinstance(precision, str):
+            self.precision = _convert_precision_str_to_dtype(precision)
+        else:
+            self.precision = precision
 
         if strategy:
+            if isinstance(strategy, str):
+                strategy = _convert_str_to_strategy(strategy)
+
             if isinstance(strategy, DDPStrategy):
-                # move module to device
-                module = module.to(self.device)
                 # wrap module in DDP
                 device_ids = None
                 if self.device.type == "cuda":
                     device_ids = [self.device.index]
-                module = DDP(module, device_ids=device_ids, **asdict(strategy))
+                params_dict = asdict(strategy)
+                # remove ddp comm hook variables from params dict
+                del params_dict["comm_state"]
+                del params_dict["comm_hook"]
+                module = DDP(module, device_ids=device_ids, **params_dict)
                 if torchdynamo_params:
                     # TODO: Add support for dynamo and DDP
                     rank_zero_warn(
                         "Torchdynamo params has been set with DDP - Note that performance will likely be slower and we recommend using only one."
                     )
+                if strategy.comm_hook:
+                    module.register_comm_hook(
+                        state=strategy.comm_state, hook=strategy.comm_hook
+                    )
+            elif isinstance(strategy, FSDPStrategy):
+                if not is_torch_version_geq_1_12():
+                    raise RuntimeError(
+                        "Please install PyTorch 1.12 or higher to use FSDP: https://pytorch.org/get-started/locally/"
+                    )
+                elif swa_params:
+                    raise RuntimeError(
+                        "Stochastic Weight Averaging is currently not supported with the FSDP strategy"
+                    )
+                mixed_precision = None
+                if self.precision:
+                    mixed_precision = MixedPrecision(
+                        param_dtype=self.precision,
+                        reduce_dtype=self.precision,
+                        buffer_dtype=self.precision,
+                    )
 
-        else:
-            # move module to device
-            module = module.to(self.device)
+                # wrap module in FSDP
+                module = FSDP(
+                    module,
+                    device_id=self.device,
+                    mixed_precision=mixed_precision,
+                    **asdict(strategy),
+                )
 
         self.module: torch.nn.Module = module
 
         self.step_lr_interval = step_lr_interval
-        if not log_frequency_steps > 0:
-            raise ValueError(
-                f"log_frequency_steps must be > 0. Got {log_frequency_steps}"
-            )
-        self.log_frequency_steps: int = log_frequency_steps
-
-        if not precision:
-            self.precision: Optional[torch.dtype] = None
-            self.grad_scaler: Optional[GradScaler] = None
-        else:
-            if isinstance(precision, str):
-                self.precision: Optional[torch.dtype] = _convert_precision_str_to_dtype(
-                    precision
-                )
-            else:
-                self.precision = precision
 
+        self.grad_scaler: Optional[GradScaler] = None
+        if self.precision:
             self.grad_scaler = _get_grad_scaler_from_precision(
-                # pyre-ignore
                 self.precision,
                 self.module,
             )
 
         if not gradient_accumulation_steps > 0:
             raise ValueError(
                 f"gradient_accumulation_steps must be > 0. Got {gradient_accumulation_steps}"
             )
         self.gradient_accumulation_steps = gradient_accumulation_steps
-        self._num_optimizer_steps_completed: int = 0
+        self._num_optimizer_steps_completed: StatefulInt = StatefulInt(0)
 
         self.detect_anomaly = detect_anomaly
         self.clip_grad_norm = clip_grad_norm
         self.clip_grad_value = clip_grad_value
 
         # create autocast context based on precision and device type
         self.maybe_autocast_precision = torch.autocast(
@@ -224,21 +326,28 @@
             if not is_torch_version_ge_1_13_1():
                 raise RuntimeError(
                     "TorchDynamo support is available only in PyTorch 2.0 or higher. "
                     "Please install PyTorch 2.0 or higher to continue: https://pytorch.org/get-started/locally/"
                 )
             # pyre-ignore
             self.compute_loss = _dynamo_wrapper(self.compute_loss, torchdynamo_params)
-            # pyre-ignore
-            self._forward_and_backward = _dynamo_wrapper(
-                self._forward_and_backward, torchdynamo_params
-            )
             self.module = _dynamo_wrapper(self.module, torchdynamo_params)
 
-        # TODO: Make AutoTrainUnit work when data type is Iterator
+        self.training = training
+
+        # cuda stream to use for moving data to device
+        self._prefetch_stream: Optional[torch.cuda.streams.Stream] = (
+            torch.cuda.Stream() if self.device.type == "cuda" else None
+        )
+        # the next batch which has been prefetched and is ready to be used
+        self._next_batch: Optional[TData] = None
+        # whether the next batch has been prefetched and is ready to be used
+        self._prefetched: bool = False
+        # whether the current batch is the last train batch
+        self._is_last_train_batch: bool = False
 
     @abstractmethod
     def configure_optimizers_and_lr_scheduler(
         self, module: torch.nn.Module
     ) -> Tuple[torch.optim.Optimizer, TLRScheduler]:
         """
         The user should implement this method with their optimizer and learning rate scheduler construction code. This will be called upon initialization of
@@ -262,207 +371,223 @@
             data: a batch of data which is passed from the ``train_step``/``eval_step``
 
         Returns:
             Tuple containing the loss and the output of the model
         """
         ...
 
-    def update_metrics(
-        self, state: State, data: TData, loss: torch.Tensor, outputs: Any
-    ) -> None:
-        """
-        The user should implement this method with code to update metrics. This will be called every ``train_step``/``eval_step``.
-
-        Args:
-            state: a State object which is passed from the ``train_step``/``eval_step``
-            data: a batch of data which is passed from the ``train_step``/``eval_step``
-            outputs: the outputs of the model forward pass
-        """
-        pass
-
-    def log_metrics(
-        self, state: State, step: int, interval: Literal["step", "epoch"]
-    ) -> None:
-        """
-        The user should implement this method with their code to log metrics. This will be called:
-
-        - every ``train_step`` based on ``log_frequency_steps`` and how many parameter updates have been run on the model
-        - in ``on_train_epoch_end`` and ``on_eval_epoch_end``
-
-        Args:
-            state: a State object which is passed from ``train_step``/``on_train_epoch_end``/``on_eval_epoch_end``
-            step: how many steps have been completed (i.e. how many parameter updates have been run on the model)
-            interval: whether ``log_metrics`` is called at the end of a step or at the end of an epoch
-        """
-        pass
-
     def move_data_to_device(self, state: State, data: TData) -> TData:
         """
         The user can override this method with custom code to copy data to device. This will be called at the start of every ``train_step``/``eval_step``/``predict_step``.
         By default this uses the utility function :py:func:`~torchtnt.utils.copy_data_to_device`.
 
+        If on GPU, this method will be called on a separate CUDA stream.
+
         Args:
             state: a State object which is passed from the ``train_step``/``eval_step``/``predict_step``
             data: a batch of data which is passed from the ``train_step``/``eval_step``/``predict_step``
 
         Returns:
             A batch of data which is on the device
         """
-        return copy_data_to_device(data, self.device)
-
-    def on_train_start(self, state: State) -> None:
-        """
-        Note that if implementing `on_train_start()`, you must call `super().on_train_start()`.
-        """
-        optimizer, lr_scheduler = self.configure_optimizers_and_lr_scheduler(
-            self.module
+        non_blocking = (
+            True
+            if state.active_phase == ActivePhase.TRAIN
+            and self.device.type == "cuda"
+            and self._prefetched
+            else False
         )
-        self.optimizer: torch.optim.optimizer.Optimizer = optimizer
-        self.lr_scheduler: TLRScheduler = lr_scheduler
-
-        self.swa_model: Optional[AveragedModel] = None
-        self.swa_scheduler: Optional[SWALR] = None
+        return copy_data_to_device(data, self.device, non_blocking=non_blocking)
 
-        if self.swa_params:
-            if not self.swa_params.avg_fn:
-                # pyre-ignore: Unexpected keyword [28]
-                self.swa_model = AveragedModel(self.module, use_buffers=True)
-            else:
-                # pyre-ignore: Unexpected keyword [28]
-                self.swa_model = AveragedModel(
-                    self.module, avg_fn=self.swa_params.avg_fn, use_buffers=True
-                )
+    def prefetch_next_batch(self, state: State, data_iter: Iterator[TData]) -> None:
+        """Prefetch the next batch on a separate CUDA stream."""
+        try:
+            with record_function(__name__ + ".next(data_iter)"):
+                next_batch = next(data_iter)
+        except StopIteration:
+            self._next_batch = None
+            self._is_last_train_batch = True
+            return
+
+        # if on cpu, self._prefetch_stream is None so the torch.cuda.stream call is a no-op
+        with torch.cuda.stream(self._prefetch_stream), record_function(
+            __name__ + ".move_data_to_device"
+        ):
+            self._next_batch = self.move_data_to_device(state, next_batch)
 
-            self.swa_scheduler = SWALR(
-                optimizer=self.optimizer,
-                # pyre-ignore: Undefined attribute [16]
-                swa_lr=self.swa_params.lr,
-                # pyre-ignore: Undefined attribute [16]
-                anneal_epochs=self.swa_params.anneal_epochs,
-                # pyre-ignore: Undefined attribute [16]
-                anneal_strategy=self.swa_params.anneal_strategy,
-            )
+    def train_step(
+        self, state: State, data: Iterator[TData]
+    ) -> Tuple[torch.Tensor, Any]:
+        train_state = none_throws(state.train_state)
+        if not self._prefetched:
+            self.prefetch_next_batch(state, data)
+            self._prefetched = True
+
+        if self._prefetch_stream:
+            with record_function(__name__ + ".wait_stream"):
+                # wait on the CUDA stream to complete the host to device copy
+                torch.cuda.current_stream().wait_stream(self._prefetch_stream)
+
+        # get the next batch which was stored by prefetch_next_batch
+        batch = self._next_batch
+        if not batch:
+            self._prefetched = False
+            self._is_last_train_batch = False
+            raise StopIteration
+
+        if self._prefetch_stream:
+            with record_function(__name__ + ".record_data_in_stream"):
+                # record the batch in the current stream
+                record_data_in_stream(batch, torch.cuda.current_stream())
 
-    def train_step(self, state: State, data: TData) -> Tuple[torch.Tensor, Any]:
-        data = self.move_data_to_device(state, data)
+        # prefetch the next batch
+        self.prefetch_next_batch(state, data)
 
-        train_state = none_throws(state.train_state)
         should_update_weights = (
             train_state.progress.num_steps_completed_in_epoch + 1
-        ) % self.gradient_accumulation_steps == 0 or train_state.is_last_batch
+        ) % self.gradient_accumulation_steps == 0 or self._is_last_train_batch
 
-        loss, outputs = self._forward_and_backward(state, data, should_update_weights)
-
-        # users can override this, by default this is a no-op
-        self.update_metrics(state, data, loss, outputs)
+        loss, outputs = self._forward_and_backward(state, batch, should_update_weights)
 
         if should_update_weights:
             # TODO try to use dynamo here
             self._run_optimizer_lr_scheduler_step(state)
 
-            # log metrics only after an optimizer step
-            if self.num_optimizer_steps_completed % self.log_frequency_steps == 0:
-                self.log_metrics(state, self.num_optimizer_steps_completed - 1, "step")
+        step = get_current_progress(state).num_steps_completed
+        # users can override this, by default this is a no-op
+        self.on_train_step_end(state, batch, step, loss, outputs)
         return loss, outputs
 
     def _forward_and_backward(
         self, state: State, data: TData, should_update_weights: bool
     ) -> Tuple[torch.Tensor, Any]:
-        # if using gradient accumulation and DDP or FSDP, when in a step where we will not update the weights,
+        # if using gradient accumulation with either DDP or FSDP, when in a step where we will not update the weights,
         # run forward and backward in no_sync context
         # https://pytorch.org/docs/stable/_modules/torch/nn/parallel/distributed.html#DistributedDataParallel.no_sync
         # https://pytorch.org/docs/stable/fsdp.html#torch.distributed.fsdp.FullyShardedDataParallel.no_sync
         maybe_no_sync = (
+            # pyre-ignore[29]
             self.module.no_sync()
-            if not should_update_weights and isinstance(self.module, (DDP, FSDP))
+            if not should_update_weights
+            and (isinstance(self.module, DDP) or _is_fsdp_module(self.module))
             else contextlib.nullcontext()
         )
 
         # if detect_anomaly is true, run forward and backward pass in detect_anomaly context
-        with maybe_no_sync, torch.autograd.set_detect_anomaly(self.detect_anomaly):
+        detect_anomaly = self.detect_anomaly
+        maybe_detect_anomaly = (
+            torch.autograd.set_detect_anomaly(detect_anomaly)
+            if detect_anomaly is not None
+            else contextlib.nullcontext()
+        )
+        with maybe_no_sync, maybe_detect_anomaly:
             with self.maybe_autocast_precision:
-                # users must override this
-                loss, outputs = self.compute_loss(state, data)
+                with record_function(__name__ + ".compute_loss"):
+                    # users must override this
+                    loss, outputs = self.compute_loss(state, data)
 
             # normalize loss to account for gradient accumulation
             loss = loss / self.gradient_accumulation_steps
 
             grad_scaler = self.grad_scaler
-            if grad_scaler:
-                loss = grad_scaler.scale(loss)
-            loss.backward()
+            with record_function(__name__ + ".backward"):
+                if grad_scaler:
+                    grad_scaler.scale(loss).backward()
+                else:
+                    loss.backward()
         return loss, outputs
 
     def _run_optimizer_lr_scheduler_step(self, state: State) -> None:
-        """Runs the optimizer step, sets gradients to zero, runs lr scheduler step, and calls `log_metrics`"""
+        """Runs the optimizer step, sets gradients to zero, and runs lr scheduler step."""
         # optimizer step
         grad_scaler = self.grad_scaler
         clip_grad_norm = self.clip_grad_norm
         clip_grad_value = self.clip_grad_value
         if grad_scaler and (clip_grad_norm or clip_grad_value):
             # unscale the gradients of optimizer's assigned params in-place in preparation for gradient clipping
             grad_scaler.unscale_(self.optimizer)
 
         # gradient norm clipping
         if clip_grad_norm:
-            if isinstance(self.module, FSDP):
-                self.module.clip_grad_norm_(max_norm=clip_grad_norm)
+            if _is_fsdp_module(self.module):
+                if isinstance(self.module, FSDP):
+                    self.module.clip_grad_norm_(max_norm=clip_grad_norm)
+                else:
+                    raise RuntimeError(
+                        "Composable FSDP clip_grad_norm is not yet implemented: https://github.com/pytorch/pytorch/issues/97271"
+                    )
             else:
                 torch.nn.utils.clip_grad_norm_(
                     parameters=self.module.parameters(),
                     max_norm=clip_grad_norm,
                 )
         # gradient value clipping
         if clip_grad_value:
             torch.nn.utils.clip_grad_value_(
                 parameters=self.module.parameters(),
                 clip_value=clip_grad_value,
             )
 
-        # optimizer step
-        if grad_scaler:
-            grad_scaler.step(self.optimizer)
-            # update the scale for next iteration
-            grad_scaler.update()
-        else:
-            self.optimizer.step()
+        with record_function(__name__ + ".optimizer_step"):
+            if grad_scaler:
+                grad_scaler.step(self.optimizer)
+                # update the scale for next iteration
+                grad_scaler.update()
+            else:
+                self.optimizer.step()
 
         self._num_optimizer_steps_completed += 1
 
         # sets gradients to zero
         self.optimizer.zero_grad(set_to_none=True)
 
         # optionally step lr scheduler if SWA not in use
         train_state = none_throws(state.train_state)
         if (
             self.swa_params is None
             or train_state.progress.num_epochs_completed < self.swa_params.epoch_start
         ):
             lr_scheduler = self.lr_scheduler
             if lr_scheduler and self.step_lr_interval == "step":
-                lr_scheduler.step()
+                with record_function(__name__ + ".lr_scheduler_step"):
+                    lr_scheduler.step()
 
-    def on_train_epoch_end(self, state: State) -> None:
-        # note: if user wants to override on_train_epoch_end themselves, they should remember to call up to this method via super().on_train_epoch_end()
+    def on_train_step_end(
+        self, state: State, data: TData, step: int, loss: torch.Tensor, outputs: Any
+    ) -> None:
+        """
+        This will be called at the end of every ``train_step`` before returning. The user can implement this method with code to update and log their metrics,
+        or do anything else.
+
+        Args:
+            state: a State object which is passed from the ``train_step``
+            data: a batch of data which is passed from the ``train_step``
+            step: how many ``train_step``s have been completed
+            loss: the loss computed in the ``compute_loss`` function
+            outputs: the outputs of the model forward pass
+        """
+        pass
 
+    def on_train_epoch_end(self, state: State) -> None:
+        """
+        Note: if overriding ``on_train_epoch_end``, remember to call ``super().on_train_epoch_end()``
+        """
         train_state = none_throws(state.train_state)
 
         if (
             self.swa_model
             and self.swa_params
             and train_state.progress.num_epochs_completed >= self.swa_params.epoch_start
         ):
             self.swa_model.update_parameters(self.module)
             none_throws(self.swa_scheduler).step()
         elif self.lr_scheduler and self.step_lr_interval == "epoch":
             # optionally step lr scheduler
-            self.lr_scheduler.step()
-
-        # users can override this, by default this is a no-op
-        self.log_metrics(state, self.num_optimizer_steps_completed, "epoch")
+            with record_function(__name__ + ".lr_scheduler_step"):
+                self.lr_scheduler.step()
 
     def on_train_end(self, state: State) -> None:
         """
         Note that if using SWA and implementing `on_train_end()`, must call `super().on_train_end()`.
         """
         swa_model = self.swa_model
         if swa_model:
@@ -472,73 +597,117 @@
     def eval_step(self, state: State, data: TData) -> Tuple[torch.Tensor, Any]:
         data = self.move_data_to_device(state, data)
 
         with self.maybe_autocast_precision:
             # users must override this
             loss, outputs = self.compute_loss(state, data)
 
+        step = get_current_progress(state).num_steps_completed
         # users can override this, by default this is a no-op
-        self.update_metrics(state, data, loss, outputs)
+        self.on_eval_step_end(state, data, step, loss, outputs)
         return loss, outputs
 
-    def on_eval_epoch_end(self, state: State) -> None:
-        # note: if user wants to override on_eval_epoch_end themselves, they should remember to call up to this method via super().on_eval_epoch_end()
-        if state.entry_point == EntryPoint.FIT:
-            # if in fit, use the number of optimizer steps completed
-            # users can override this, by default this is a no-op
-            self.log_metrics(state, self.num_optimizer_steps_completed, "epoch")
-        else:
-            eval_state = none_throws(state.eval_state)
+    def on_eval_step_end(
+        self, state: State, data: TData, step: int, loss: torch.Tensor, outputs: Any
+    ) -> None:
+        """
+        This will be called at the end of every ``eval_step`` before returning. The user can implement this method with code to update and log their metrics,
+        or do anything else.
 
-            # if in evaluate, use the number of eval steps completed
-            # users can override this, by default this is a no-op
-            self.log_metrics(state, eval_state.progress.num_steps_completed, "epoch")
+        Args:
+            state: a State object which is passed from the ``eval_step``
+            data: a batch of data which is passed from the ``eval_step``
+            step: how many steps have been completed (``train_step``s when running fit and ``eval_step``s when running evaluation)
+            loss: the loss computed in the ``compute_loss`` function
+            outputs: the outputs of the model forward pass
+        """
+        pass
 
     def predict_step(self, state: State, data: Any) -> Any:
         data = self.move_data_to_device(state, data)
 
         with self.maybe_autocast_precision:
             outputs = self.module(data)
+
+        step = get_current_progress(state).num_steps_completed
+        # users can override this, by default this is a no-op
+        self.on_predict_step_end(state, data, step, outputs)
         return outputs
 
+    def on_predict_step_end(
+        self, state: State, data: TData, step: int, outputs: Any
+    ) -> None:
+        """
+        This will be called at the end of every ``predict_step`` before returning. The user can implement this method with code to update and log their metrics,
+        or do anything else.
+
+        Args:
+            state: a State object which is passed from the ``predict_step``
+            data: a batch of data which is passed from the ``predict_step``
+            step: how many ``predict_step``s have been completed
+            outputs: the outputs of the model forward pass
+        """
+        pass
+
     @property
     def num_optimizer_steps_completed(self) -> int:
-        return self._num_optimizer_steps_completed
+        return self._num_optimizer_steps_completed.val
 
 
-def _convert_precision_str_to_dtype(precision: str) -> torch.dtype:
+def _convert_precision_str_to_dtype(precision: str) -> Optional[torch.dtype]:
     """
     Converts precision as a string to a torch.dtype
 
     Args:
         precision: string containing the precision
 
     Raises:
         ValueError if an invalid precision string is passed.
 
     """
-    string_to_dtype_mapping = {"fp16": torch.float16, "bf16": torch.bfloat16}
+    string_to_dtype_mapping = {
+        "fp16": torch.float16,
+        "bf16": torch.bfloat16,
+        "fp32": None,
+    }
     if precision not in string_to_dtype_mapping.keys():
         raise ValueError(
-            f"Precision {precision} not supported. Please use one of `fp16` or `bf16`"
+            f"Precision {precision} not supported. Please use one of {list(string_to_dtype_mapping.keys())}"
         )
     return string_to_dtype_mapping[precision]
 
 
+def _convert_str_to_strategy(strategy: str) -> Union[DDPStrategy, FSDPStrategy]:
+    """
+    Converts strategy as a string to a default instance of the Strategy dataclass.
+
+    Args:
+        strategy: string specifying the distributed strategy to use
+
+    Raises:
+        ValueError if an invalid strategy string is passed.
+
+    """
+    string_to_strategy_mapping = {
+        "ddp": DDPStrategy(),
+        "fsdp": FSDPStrategy(),
+    }
+
+    if strategy not in string_to_strategy_mapping:
+        raise ValueError(
+            f"Strategy {strategy} not supported. Please use one of {list(string_to_strategy_mapping.keys())}"
+        )
+    return string_to_strategy_mapping[strategy]
+
+
 def _get_grad_scaler_from_precision(
     precision: torch.dtype, module: torch.nn.Module
 ) -> Optional[GradScaler]:
     if precision == torch.float16:
-        if isinstance(module, FSDP):
-            if not is_torch_version_geq_1_12():
-                raise RuntimeError(
-                    "Using float16 precision with torch.distributed.fsdp.FullyShardedDataParallel requires "
-                    "torch.distributed.fsdp.sharded_grad_scaler.ShardedGradScaler from PyTorch 1.12. "
-                    "Please install PyTorch 1.12 or higher to continue: https://pytorch.org/get-started/locally/"
-                )
+        if _is_fsdp_module(module):
             from torch.distributed.fsdp.sharded_grad_scaler import ShardedGradScaler
 
             return ShardedGradScaler()
         else:
             return GradScaler()
     return None
```

### Comparing `torchtnt-0.0.7/torchtnt/framework/callback.py` & `torchtnt-0.1.0/torchtnt/framework/callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/framework/callbacks/__init__.py` & `torchtnt-0.1.0/torchtnt/framework/callbacks/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 from .learning_rate_monitor import LearningRateMonitor
 from .module_summary import ModuleSummary
 from .pytorch_profiler import PyTorchProfiler
 from .system_resources_monitor import SystemResourcesMonitor
 from .tensorboard_parameter_monitor import TensorBoardParameterMonitor
 from .torchsnapshot_saver import TorchSnapshotSaver
 from .tqdm_progress_bar import TQDMProgressBar
-
+from .train_progress_monitor import TrainProgressMonitor
 
 __all__ = [
     "BaseCSVWriter",
     "GarbageCollector",
     "Lambda",
     "LearningRateMonitor",
     "ModuleSummary",
     "PyTorchProfiler",
     "SystemResourcesMonitor",
     "TensorBoardParameterMonitor",
     "TorchSnapshotSaver",
     "TQDMProgressBar",
+    "TrainProgressMonitor",
 ]
```

### Comparing `torchtnt-0.0.7/torchtnt/framework/callbacks/base_csv_writer.py` & `torchtnt-0.1.0/torchtnt/framework/callbacks/base_csv_writer.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/framework/callbacks/garbage_collector.py` & `torchtnt-0.1.0/torchtnt/framework/callbacks/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/framework/callbacks/lambda_callback.py` & `torchtnt-0.1.0/torchtnt/framework/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/framework/callbacks/learning_rate_monitor.py` & `torchtnt-0.1.0/torchtnt/framework/callbacks/learning_rate_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     lr_stats: Dict[str, float] = {}
 
     # go through tracked optimizers
     optimizers = unit.tracked_optimizers()
     for name, optim in optimizers.items():
         _extract_lr_from_optimizer(optim, f"optimizers/{name}", lr_stats)
 
-    # go through track schedulers
+    # go through tracked LR schedulers
     lr_schedulers = unit.tracked_lr_schedulers()
     for name, lr_scheduler in lr_schedulers.items():
         _extract_lr_from_optimizer(
             lr_scheduler.optimizer, f"lr_schedulers/{name}", lr_stats
         )
 
     return lr_stats
```

### Comparing `torchtnt-0.0.7/torchtnt/framework/callbacks/module_summary.py` & `torchtnt-0.1.0/torchtnt/framework/callbacks/module_summary.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/framework/callbacks/pytorch_profiler.py` & `torchtnt-0.1.0/torchtnt/framework/callbacks/pytorch_profiler.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/framework/callbacks/system_resources_monitor.py` & `torchtnt-0.1.0/torchtnt/framework/callbacks/system_resources_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py` & `torchtnt-0.1.0/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/framework/callbacks/torchsnapshot_saver.py` & `torchtnt-0.1.0/torchtnt/framework/callbacks/torchsnapshot_saver.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,16 +84,19 @@
         app_state = unit.app_state()
         _check_app_state_collision(app_state)
 
     def on_train_step_end(self, state: State, unit: TTrainUnit) -> None:
         train_state = none_throws(state.train_state)
 
         global_step = train_state.progress.num_steps_completed
-        every_n_train_steps = self._save_every_n_train_steps
-        if every_n_train_steps is None or global_step % every_n_train_steps != 0:
+        save_every_n_train_steps = self._save_every_n_train_steps
+        if (
+            save_every_n_train_steps is None
+            or global_step % save_every_n_train_steps != 0
+        ):
             return
 
         app_state = _get_app_state(state, unit, self._replicated, intra_epoch=True)
 
         # save snapshot to predetermined path
         # TODO: discuss whether this path should be customized
         epoch = train_state.progress.num_epochs_completed
@@ -101,16 +104,16 @@
         self._async_snapshot(snapshot_path, app_state, wait=False)
 
     def on_train_epoch_end(self, state: State, unit: TTrainUnit) -> None:
         train_state = none_throws(state.train_state)
 
         train_progress = train_state.progress
         epoch = train_progress.num_epochs_completed
-        every_n_epochs = self._save_every_n_epochs
-        if every_n_epochs is None or epoch % every_n_epochs != 0:
+        save_every_n_epochs = self._save_every_n_epochs
+        if save_every_n_epochs is None or epoch % save_every_n_epochs != 0:
             return
 
         app_state = _get_app_state(
             state, unit, replicated=self._replicated, intra_epoch=False
         )
 
         # save snapshot to predetermined path
```

### Comparing `torchtnt-0.0.7/torchtnt/framework/callbacks/tqdm_progress_bar.py` & `torchtnt-0.1.0/torchtnt/framework/callbacks/tqdm_progress_bar.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/framework/evaluate.py` & `torchtnt-0.1.0/torchtnt/framework/evaluate.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,60 +10,64 @@
 import torch
 from pyre_extensions import none_throws
 from torchtnt.framework.callback import Callback
 
 from torchtnt.framework.state import ActivePhase, EntryPoint, PhaseState, State
 from torchtnt.framework.unit import TEvalData, TEvalUnit
 from torchtnt.framework.utils import (
+    _get_timing_context,
     _is_epoch_done,
     _reset_module_training_mode,
     _run_callback_fn,
     _set_module_training_mode,
     _step_requires_iterator,
     log_api_usage,
 )
-from torchtnt.utils.timer import get_timer_summary
+from torchtnt.utils.timer import get_timer_summary, Timer
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def init_eval_state(
     *,
     dataloader: Iterable[TEvalData],
     max_steps_per_epoch: Optional[int] = None,
+    auto_timing: bool = False,
 ) -> State:
     """
     ``init_eval_state`` is a helper function that initializes a :class:`~torchtnt.framework.State` object for evaluation. This :class:`~torchtnt.framework.State` object
     can then be passed to the :func:`~torchtnt.framework.evaluate` entry point.
 
     Args:
         dataloader: dataloader to be used during evaluation, which can be *any* iterable, including PyTorch DataLoader, DataLoader2, etc.
         max_steps_per_epoch: the max number of steps to run per epoch. None means evaluate until the dataloader is exhausted.
+        auto_timing: whether to automatically time the evaluation loop, using the state's timer (enabling auto_timing may degrade performance).
 
     Returns:
         An initialized state object containing metadata.
 
     Below is an example of calling :py:func:`~torchtnt.framework.init_eval_state` and :py:func:`~torchtnt.framework.evaluate` together.
 
     .. code-block:: python
 
-      from torchtnt.framework import init_eval_state, evaluate
+        from torchtnt.framework import init_eval_state, evaluate
 
-      eval_unit = MyEvalUnit(module=..., optimizer=..., lr_scheduler=...)
-      dataloader = torch.utils.data.DataLoader(...)
-      state = init_eval_state(dataloader=dataloader, max_steps_per_epoch=20)
-      evaluate(state, eval_unit)
+        eval_unit = MyEvalUnit(module=..., optimizer=..., lr_scheduler=...)
+        dataloader = torch.utils.data.DataLoader(...)
+        state = init_eval_state(dataloader=dataloader, max_steps_per_epoch=20)
+        evaluate(state, eval_unit)
     """
 
     return State(
         entry_point=EntryPoint.EVALUATE,
         eval_state=PhaseState(
             dataloader=dataloader,
             max_steps_per_epoch=max_steps_per_epoch,
         ),
+        timer=None if not auto_timing else Timer(),
     )
 
 
 def evaluate(
     state: State,
     eval_unit: TEvalUnit,
     *,
@@ -78,28 +82,49 @@
         eval_unit: an instance of :class:`~torchtnt.framework.EvalUnit` which implements `eval_step`.
         callbacks: an optional list of callbacks.
 
     Below is an example of calling :py:func:`~torchtnt.framework.init_eval_state` and :py:func:`~torchtnt.framework.evaluate` together.
 
     .. code-block:: python
 
-      from torchtnt.framework import init_eval_state, evaluate
+        from torchtnt.framework import init_eval_state, evaluate
 
-      eval_unit = MyEvalUnit(module=..., optimizer=..., lr_scheduler=...)
-      dataloader = torch.utils.data.DataLoader(...)
-      state = init_eval_state(dataloader=dataloader, max_steps_per_epoch=20)
-      evaluate(state, eval_unit)
+        eval_unit = MyEvalUnit(module=..., optimizer=..., lr_scheduler=...)
+        dataloader = torch.utils.data.DataLoader(...)
+        state = init_eval_state(dataloader=dataloader, max_steps_per_epoch=20)
+        evaluate(state, eval_unit)
+
+    Below is pseudocode of what the :py:func:`~torchtnt.framework.evaluate` entry point does.
+
+    .. code-block:: text
+
+        set unit's tracked modules to eval mode
+        call on_eval_start on unit first and then callbacks
+        while not done:
+            call on_eval_epoch_start on unit first and then callbacks
+            try:
+                data = next(dataloader)
+                call on_eval_step_start on callbacks
+                call eval_step on unit
+                increment step counter
+                call on_eval_step_end on callbacks
+            except StopIteration:
+                break
+        increment epoch counter
+        call on_eval_epoch_end on unit first and then callbacks
+        call on_eval_end on unit first and then callbacks
     """
     log_api_usage("evaluate")
     callbacks = callbacks or []
     try:
         state._entry_point = EntryPoint.EVALUATE
         _evaluate_impl(state, eval_unit, callbacks)
         logger.info("Finished evaluation")
-        logger.debug(get_timer_summary(state.timer))
+        if state.timer:
+            logger.info(get_timer_summary(state.timer))
     except Exception as e:
         # TODO: log for diagnostics
         logger.info(e)
         eval_unit.on_exception(state, e)
         _run_callback_fn(callbacks, "on_exception", state, eval_unit, e)
         raise e
 
@@ -119,23 +144,25 @@
     )
 
     # Set all modules to eval mode
     # access modules made available through _AppStateMixin
     tracked_modules = eval_unit.tracked_modules()
     prior_module_train_states = _set_module_training_mode(tracked_modules, False)
 
-    with state.timer.time(f"eval.{eval_unit.__class__.__name__}.on_eval_start"):
+    with _get_timing_context(
+        state, f"eval.{eval_unit.__class__.__name__}.on_eval_start"
+    ):
         eval_unit.on_eval_start(state)
     _run_callback_fn(callbacks, "on_eval_start", state, eval_unit)
 
     # Conditionally run this to avoid running this multiple times
     # in the case of resuming from a checkpoint mid-epoch
     if eval_state.progress.num_steps_completed_in_epoch == 0:
-        with state.timer.time(
-            f"eval.{eval_unit.__class__.__name__}.on_eval_epoch_start"
+        with _get_timing_context(
+            state, f"eval.{eval_unit.__class__.__name__}.on_eval_epoch_start"
         ):
             eval_unit.on_eval_epoch_start(state)
         _run_callback_fn(callbacks, "on_eval_epoch_start", state, eval_unit)
 
     data_iter = iter(eval_state.dataloader)
     step_input = data_iter
 
@@ -147,22 +174,29 @@
         or _is_epoch_done(
             eval_state.progress, eval_state.max_steps_per_epoch, eval_state.max_steps
         )
     ):
         try:
             if not pass_data_iter_to_step:
                 # get the next batch from the data iterator
-                with state.timer.time("eval.data_iter_next"):
+                with _get_timing_context(state, "eval.data_iter_next"):
                     step_input = next(data_iter)
             _run_callback_fn(callbacks, "on_eval_step_start", state, eval_unit)
-            with state.timer.time(f"eval.{eval_unit.__class__.__name__}.eval_step"):
+            with _get_timing_context(
+                state, f"eval.{eval_unit.__class__.__name__}.eval_step"
+            ):
                 eval_state._step_output = eval_unit.eval_step(state, step_input)
 
             eval_state.progress.increment_step()
-            _run_callback_fn(callbacks, "on_eval_step_end", state, eval_unit)
+            _run_callback_fn(
+                callbacks,
+                "on_eval_step_end",
+                state,
+                eval_unit,
+            )
             # clear step_output to avoid retaining extra memory
             eval_state._step_output = None
         except StopIteration:
             break
 
     # Possibly warn about an empty dataloader
     any_steps_completed = (
@@ -170,19 +204,21 @@
     )
     if not any_steps_completed:
         logger.warning("No steps completed during evaluate epoch!")
 
     # set progress counters for the next epoch
     eval_state.progress.increment_epoch()
 
-    with state.timer.time(f"eval.{eval_unit.__class__.__name__}.on_eval_epoch_end"):
+    with _get_timing_context(
+        state, f"eval.{eval_unit.__class__.__name__}.on_eval_epoch_end"
+    ):
         eval_unit.on_eval_epoch_end(state)
     _run_callback_fn(callbacks, "on_eval_epoch_end", state, eval_unit)
 
-    with state.timer.time(f"eval.{eval_unit.__class__.__name__}.on_eval_end"):
+    with _get_timing_context(state, f"eval.{eval_unit.__class__.__name__}.on_eval_end"):
         eval_unit.on_eval_end(state)
     _run_callback_fn(callbacks, "on_eval_end", state, eval_unit)
 
     # Reset training mode for modules at the end of the epoch
     # This ensures that side-effects made by the loop are reset before
     # returning back to the user
     _reset_module_training_mode(tracked_modules, prior_module_train_states)
```

### Comparing `torchtnt-0.0.7/torchtnt/framework/fit.py` & `torchtnt-0.1.0/torchtnt/framework/fit.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,57 +14,64 @@
 from torchtnt.framework.unit import (
     EvalUnit,
     TEvalData,
     TrainUnit,
     TTrainData,
     TTrainUnit,
 )
-from torchtnt.framework.utils import _is_done, _run_callback_fn, log_api_usage
-from torchtnt.utils.timer import get_timer_summary
+from torchtnt.framework.utils import (
+    _get_timing_context,
+    _is_done,
+    _run_callback_fn,
+    log_api_usage,
+)
+from torchtnt.utils.timer import get_timer_summary, Timer
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def init_fit_state(
     train_dataloader: Iterable[TTrainData],
     eval_dataloader: Iterable[TEvalData],
     max_epochs: Optional[int] = None,
     max_steps: Optional[int] = None,
     max_train_steps_per_epoch: Optional[int] = None,
     max_eval_steps_per_epoch: Optional[int] = None,
     evaluate_every_n_steps: Optional[int] = None,
     evaluate_every_n_epochs: Optional[int] = 1,
+    auto_timing: bool = False,
 ) -> State:
     """
     ``init_fit_state`` is a helper function that initializes a :class:`~torchtnt.framework.State` object for fitting. This :class:`~torchtnt.framework.State` object
     can then be passed to the :func:`~torchtnt.framework.fit` entry point.
 
     Args:
         train_dataloader: dataloader to be used during training, which can be *any* iterable, including PyTorch DataLoader, DataLoader2, etc.
         eval_dataloader: dataloader to be used during evaluation, which can be *any* iterable, including PyTorch DataLoader, DataLoader2, etc.
         max_epochs: the max number of epochs to run for training. ``None`` means no limit (infinite training) unless stopped by max_steps.
         max_steps: the max number of steps to run for training. ``None`` means no limit (infinite training) unless stopped by max_epochs.
         max_train_steps_per_epoch: the max number of steps to run per epoch for training. None means train until the dataloader is exhausted.
         evaluate_every_n_steps: how often to run the evaluation loop in terms of training steps.
         evaluate_every_n_epochs: how often to run the evaluation loop in terms of training epochs.
+        auto_timing: whether to automatically time the training and evaluation loop, using the state's timer (enabling auto_timing may degrade performance).
 
     Returns:
         An initialized state object containing metadata.
 
     Below is an example of calling :py:func:`~torchtnt.framework.init_fit_state` and :py:func:`~torchtnt.framework.fit` together.
 
     .. code-block:: python
 
-      from torchtnt.framework import fit, init_fit_state
+        from torchtnt.framework import fit, init_fit_state
 
-      fit_unit = MyFitUnit(module=..., optimizer=..., lr_scheduler=...)
-      train_dataloader = torch.utils.data.DataLoader(...)
-      eval_dataloader = torch.utils.data.DataLoader(...)
-      state = init_fit_state(train_dataloader=train_dataloader, eval_dataloader=eval_dataloader, max_epochs=4)
-      fit(state, fit_unit)
+        fit_unit = MyFitUnit(module=..., optimizer=..., lr_scheduler=...)
+        train_dataloader = torch.utils.data.DataLoader(...)
+        eval_dataloader = torch.utils.data.DataLoader(...)
+        state = init_fit_state(train_dataloader=train_dataloader, eval_dataloader=eval_dataloader, max_epochs=4)
+        fit(state, fit_unit)
     """
 
     return State(
         entry_point=EntryPoint.FIT,
         train_state=PhaseState(
             dataloader=train_dataloader,
             max_epochs=max_epochs,
@@ -73,19 +80,23 @@
         ),
         eval_state=PhaseState(
             dataloader=eval_dataloader,
             max_steps_per_epoch=max_eval_steps_per_epoch,
             evaluate_every_n_steps=evaluate_every_n_steps,
             evaluate_every_n_epochs=evaluate_every_n_epochs,
         ),
+        timer=None if not auto_timing else Timer(),
     )
 
 
 def fit(
-    state: State, unit: TTrainUnit, *, callbacks: Optional[List[Callback]] = None
+    state: State,
+    unit: TTrainUnit,
+    *,
+    callbacks: Optional[List[Callback]] = None,
 ) -> None:
     """
     The ``fit`` entry point interleaves training and evaluation loops.  It takes in a :class:`~torchtnt.framework.State` object, an object which subclasses both :class:`~torchtnt.framework.TrainUnit` and :class:`~torchtnt.framework.EvalUnit`,
     and an optional list of :class:`~torchtnt.framework.Callback` s, and runs the fit loop. The :class:`~torchtnt.framework.State` object can be initialized with :func:`~torchtnt.framework.init_fit_state`.
 
     Args:
         state: a :class:`~torchtnt.framework.State` object containing metadata about the fitting run.
@@ -94,29 +105,55 @@
          implementing :meth:`~torchtnt.framework.TrainUnit.train_step` and :meth:`~torchtnt.framework.EvalUnit.eval_step`.
         callbacks: an optional list of callbacks.
 
     Below is an example of calling :py:func:`~torchtnt.framework.init_fit_state` and :py:func:`~torchtnt.framework.fit` together.
 
     .. code-block:: python
 
-      from torchtnt.framework import fit, init_fit_state
+        from torchtnt.framework import fit, init_fit_state
 
-      fit_unit = MyFitUnit(module=..., optimizer=..., lr_scheduler=...)
-      train_dataloader = torch.utils.data.DataLoader(...)
-      eval_dataloader = torch.utils.data.DataLoader(...)
-      state = init_fit_state(train_dataloader=train_dataloader, eval_dataloader=eval_dataloader, max_epochs=4)
-      fit(state, fit_unit)
+        fit_unit = MyFitUnit(module=..., optimizer=..., lr_scheduler=...)
+        train_dataloader = torch.utils.data.DataLoader(...)
+        eval_dataloader = torch.utils.data.DataLoader(...)
+        state = init_fit_state(train_dataloader=train_dataloader, eval_dataloader=eval_dataloader, max_epochs=4)
+        fit(state, fit_unit)
+
+    Below is pseudocode of what the :py:func:`~torchtnt.framework.fit` entry point does.
+
+    .. code-block:: text
+
+        set unit's tracked modules to train mode
+        call on_train_start on unit first and then callbacks
+        while training is not done:
+            while epoch is not done:
+                call on_train_epoch_start on unit first and then callbacks
+                try:
+                    data = next(dataloader)
+                    call on_train_step_start on callbacks
+                    call train_step on unit
+                    increment step counter
+                    call on_train_step_end on callbacks
+                    if should evaluate after this step:
+                        run eval loops
+                except StopIteration:
+                    break
+            increment epoch counter
+            call on_train_epoch_end on unit first and then callbacks
+            if should evaluate after this epoch:
+                run eval loop
+        call on_train_end on unit first and then callbacks
     """
     log_api_usage("fit")
     callbacks = callbacks or []
 
     try:
         state._entry_point = EntryPoint.FIT
         _fit_impl(state, unit, callbacks)
-        logger.debug(get_timer_summary(state.timer))
+        if state.timer:
+            logger.info(get_timer_summary(state.timer))
     except Exception as e:
         # TODO: log for diagnostics
         logger.info(e)
         unit.on_exception(state, e)
         _run_callback_fn(callbacks, "on_exception", state, unit, e)
         raise e
 
@@ -140,20 +177,20 @@
         f"max_steps={train_state.max_steps} "
         f"max_train_steps_per_epoch={train_state.max_steps_per_epoch} "
         f"max_eval_steps_per_epoch={eval_state.max_steps_per_epoch} "
         f"evaluate_every_n_steps={eval_state.evaluate_every_n_steps} "
         f"evaluate_every_n_epochs={eval_state.evaluate_every_n_epochs} "
     )
 
-    with state.timer.time(f"train.{unit.__class__.__name__}.on_train_start"):
+    with _get_timing_context(state, f"train.{unit.__class__.__name__}.on_train_start"):
         unit.on_train_start(state)
     _run_callback_fn(callbacks, "on_train_start", state, unit)
 
     while not (
         state.should_stop
         or _is_done(train_state.progress, train_state.max_epochs, train_state.max_steps)
     ):
         _train_epoch_impl(state, unit, callbacks)
 
-    with state.timer.time(f"train.{unit.__class__.__name__}.on_train_end"):
+    with _get_timing_context(state, f"train.{unit.__class__.__name__}.on_train_end"):
         unit.on_train_end(state)
     _run_callback_fn(callbacks, "on_train_end", state, unit)
```

### Comparing `torchtnt-0.0.7/torchtnt/framework/predict.py` & `torchtnt-0.1.0/torchtnt/framework/predict.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,61 +10,65 @@
 import torch
 from pyre_extensions import none_throws
 from torchtnt.framework.callback import Callback
 
 from torchtnt.framework.state import ActivePhase, EntryPoint, PhaseState, State
 from torchtnt.framework.unit import TPredictData, TPredictUnit
 from torchtnt.framework.utils import (
+    _get_timing_context,
     _is_epoch_done,
     _reset_module_training_mode,
     _run_callback_fn,
     _set_module_training_mode,
     _step_requires_iterator,
     log_api_usage,
 )
-from torchtnt.utils.timer import get_timer_summary
+from torchtnt.utils.timer import get_timer_summary, Timer
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def init_predict_state(
     *,
     dataloader: Iterable[TPredictData],
     max_steps_per_epoch: Optional[int] = None,
+    auto_timing: bool = False,
 ) -> State:
     """
     ``init_predict_state`` is a helper function that initializes a :class:`~torchtnt.framework.State` object for prediction. This :class:`~torchtnt.framework.State` object
     can then be passed to the :func:`~torchtnt.framework.predict` entry point.
 
     Args:
         dataloader: dataloader to be used during prediction, which can be *any* iterable, including PyTorch DataLoader, DataLoader2, etc.
         max_steps_per_epoch: the max number of steps to run per epoch. None means predict until the dataloader is exhausted.
+        auto_timing: whether to automatically time the prediction loop, using the state's timer (enabling auto_timing may degrade performance).
 
     Returns:
         An initialized state object containing metadata.
 
     Below is an example of calling :py:func:`~torchtnt.framework.init_predict_state` and :py:func:`~torchtnt.framework.predict` together.
 
     .. code-block:: python
 
-      from torchtnt.framework import init_predict_state, predict
+        from torchtnt.framework import init_predict_state, predict
 
-      predict_unit = MyPredictUnit(module=..., optimizer=..., lr_scheduler=...)
-      dataloader = torch.utils.data.DataLoader(...)
-      state = init_predict_state(dataloader=dataloader, max_steps_per_epoch=20)
-      predict(state, predict_unit)
+        predict_unit = MyPredictUnit(module=..., optimizer=..., lr_scheduler=...)
+        dataloader = torch.utils.data.DataLoader(...)
+        state = init_predict_state(dataloader=dataloader, max_steps_per_epoch=20)
+        predict(state, predict_unit)
 
     """
 
     return State(
         entry_point=EntryPoint.PREDICT,
         predict_state=PhaseState(
             dataloader=dataloader,
             max_steps_per_epoch=max_steps_per_epoch,
         ),
+        timer=None if not auto_timing else Timer(),
     )
 
 
 def predict(
     state: State,
     predict_unit: TPredictUnit,
     *,
@@ -79,28 +83,49 @@
         predict_unit: an instance of :class:`~torchtnt.framework.PredictUnit` which implements `predict_step`.
         callbacks: an optional list of callbacks.
 
     Below is an example of calling :py:func:`~torchtnt.framework.init_predict_state` and :py:func:`~torchtnt.framework.predict` together.
 
     .. code-block:: python
 
-      from torchtnt.framework import init_predict_state, predict
+        from torchtnt.framework import init_predict_state, predict
 
-      predict_unit = MyPredictUnit(module=..., optimizer=..., lr_scheduler=...)
-      dataloader = torch.utils.data.DataLoader(...)
-      state = init_predict_state(dataloader=dataloader, max_steps_per_epoch=20)
-      predict(state, predict_unit)
+        predict_unit = MyPredictUnit(module=..., optimizer=..., lr_scheduler=...)
+        dataloader = torch.utils.data.DataLoader(...)
+        state = init_predict_state(dataloader=dataloader, max_steps_per_epoch=20)
+        predict(state, predict_unit)
+
+    Below is pseudocode of what the :py:func:`~torchtnt.framework.predict` entry point does.
+
+    .. code-block:: text
+
+        set unit's tracked modules to eval mode
+        call on_predict_start on unit first and then callbacks
+        while not done:
+            call on_predict_epoch_start on unit first and then callbacks
+            try:
+                data = next(dataloader)
+                call on_predict_step_start on callbacks
+                call predict_step on unit
+                increment step counter
+                call on_predict_step_end on callbacks
+            except StopIteration:
+                break
+        increment epoch counter
+        call on_predict_epoch_end on unit first and then callbacks
+        call on_predict_end on unit first and then callbacks
     """
     log_api_usage("predict")
     callbacks = callbacks or []
     try:
         state._entry_point = EntryPoint.PREDICT
         _predict_impl(state, predict_unit, callbacks)
         logger.info("Finished predict")
-        logger.debug(get_timer_summary(state.timer))
+        if state.timer:
+            logger.info(get_timer_summary(state.timer))
     except Exception as e:
         # TODO: log for diagnostics
         logger.info(e)
         predict_unit.on_exception(state, e)
         _run_callback_fn(callbacks, "on_exception", state, predict_unit, e)
         raise e
 
@@ -120,25 +145,25 @@
     )
 
     # Set all modules to eval mode
     # access modules made available through _AppStateMixin
     tracked_modules = predict_unit.tracked_modules()
     prior_module_train_states = _set_module_training_mode(tracked_modules, False)
 
-    with state.timer.time(
-        f"predict.{predict_unit.__class__.__name__}.on_predict_start"
+    with _get_timing_context(
+        state, f"predict.{predict_unit.__class__.__name__}.on_predict_start"
     ):
         predict_unit.on_predict_start(state)
     _run_callback_fn(callbacks, "on_predict_start", state, predict_unit)
 
     # Conditionally run this to avoid running this multiple times
     # in the case of resuming from a checkpoint mid-epoch
     if predict_state.progress.num_steps_completed_in_epoch == 0:
-        with state.timer.time(
-            f"predict.{predict_unit.__class__.__name__}.on_predict_epoch_start"
+        with _get_timing_context(
+            state, f"predict.{predict_unit.__class__.__name__}.on_predict_epoch_start"
         ):
             predict_unit.on_predict_epoch_start(state)
         _run_callback_fn(callbacks, "on_predict_epoch_start", state, predict_unit)
 
     data_iter = iter(predict_state.dataloader)
     step_input = data_iter
 
@@ -152,20 +177,20 @@
             predict_state.max_steps_per_epoch,
             predict_state.max_steps,
         )
     ):
         try:
             if not pass_data_iter_to_step:
                 # get the next batch from the data iterator
-                with state.timer.time("predict.data_iter_next"):
+                with _get_timing_context(state, "predict.data_iter_next"):
                     step_input = next(data_iter)
 
             _run_callback_fn(callbacks, "on_predict_step_start", state, predict_unit)
-            with state.timer.time(
-                f"predict.{predict_unit.__class__.__name__}.predict_step"
+            with _get_timing_context(
+                state, f"predict.{predict_unit.__class__.__name__}.predict_step"
             ):
                 predict_state._step_output = predict_unit.predict_step(
                     state, step_input
                 )
             predict_state.progress.increment_step()
             _run_callback_fn(callbacks, "on_predict_step_end", state, predict_unit)
 
@@ -181,21 +206,23 @@
     )
     if not any_steps_completed:
         logger.warning("No steps completed during predict epoch!")
 
     # set progress counters for the next epoch
     predict_state.progress.increment_epoch()
 
-    with state.timer.time(
-        f"predict.{predict_unit.__class__.__name__}.on_predict_epoch_end"
+    with _get_timing_context(
+        state, f"predict.{predict_unit.__class__.__name__}.on_predict_epoch_end"
     ):
         predict_unit.on_predict_epoch_end(state)
     _run_callback_fn(callbacks, "on_predict_epoch_end", state, predict_unit)
 
-    with state.timer.time(f"predict.{predict_unit.__class__.__name__}.on_predict_end"):
+    with _get_timing_context(
+        state, f"predict.{predict_unit.__class__.__name__}.on_predict_end"
+    ):
         predict_unit.on_predict_end(state)
     _run_callback_fn(callbacks, "on_predict_end", state, predict_unit)
 
     # Reset training mode for modules at the end of the epoch
     # This ensures that side-effects made by the loop are reset before
     # returning back to the user
     _reset_module_training_mode(tracked_modules, prior_module_train_states)
```

### Comparing `torchtnt-0.0.7/torchtnt/framework/progress.py` & `torchtnt-0.1.0/torchtnt/framework/progress.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/framework/state.py` & `torchtnt-0.1.0/torchtnt/framework/state.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,15 +87,14 @@
         self._max_epochs = max_epochs
         self._max_steps = max_steps
         self._max_steps_per_epoch = max_steps_per_epoch
         self._evaluate_every_n_steps = evaluate_every_n_steps
         self._evaluate_every_n_epochs = evaluate_every_n_epochs
 
         self._step_output: Any = None
-        self._is_last_batch: bool = False  # only used for train
 
     @property
     def dataloader(self) -> Iterable[Any]:
         """Dataloader defined by the user."""
         return self._dataloader
 
     @property
@@ -129,19 +128,14 @@
         return self._evaluate_every_n_epochs
 
     @property
     def step_output(self) -> Any:
         """Output of the last step."""
         return self._step_output
 
-    @property
-    def is_last_batch(self) -> bool:
-        """Returns true if current batch of data is the last batch."""
-        return self._is_last_batch
-
 
 class State:
     """Parent State class which can contain up to 3 instances of PhaseState, for the 3 phases.
     Modified by the framework, read-only for the user.
     """
 
     def __init__(
@@ -150,15 +144,15 @@
         entry_point: EntryPoint,
         timer: Optional[Timer] = None,
         train_state: Optional[PhaseState] = None,
         eval_state: Optional[PhaseState] = None,
         predict_state: Optional[PhaseState] = None,
     ) -> None:
         self._entry_point = entry_point
-        self._timer: Timer = timer or Timer()
+        self._timer = timer
         self._train_state = train_state
         self._eval_state = eval_state
         self._predict_state = predict_state
         self._should_stop: bool = False
         self._active_phase: ActivePhase = ActivePhase.TRAIN
 
     @property
@@ -168,16 +162,16 @@
 
     @property
     def active_phase(self) -> ActivePhase:
         """Current active phase of the loop. (One of TRAIN, EVALUATE, PREDICT)."""
         return self._active_phase
 
     @property
-    def timer(self) -> Timer:
-        """A :class:`~torchtnt.framework.Timer` object which records latencies of key events during loop execution."""
+    def timer(self) -> Optional[Timer]:
+        """A :class:`~torchtnt.framework.Timer` object which can be used for debugging to record latencies of key events during loop execution."""
         return self._timer
 
     @property
     def train_state(self) -> Optional[PhaseState]:
         """A :class:`~torchtnt.framework.PhaseState` object which contains meta information about the train phase."""
         return self._train_state
```

### Comparing `torchtnt-0.0.7/torchtnt/framework/train.py` & `torchtnt-0.1.0/torchtnt/framework/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,74 +5,79 @@
 # LICENSE file in the root directory of this source tree.
 
 import logging
 from typing import Iterable, List, Optional
 
 import torch
 from pyre_extensions import none_throws
+from torch.profiler import record_function
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.evaluate import _evaluate_impl
 from torchtnt.framework.state import ActivePhase, EntryPoint, PhaseState, State
 from torchtnt.framework.unit import TTrainData, TTrainUnit
 from torchtnt.framework.utils import (
+    _get_timing_context,
     _is_done,
-    _is_last_batch_in_epoch,
+    _is_epoch_done,
     _maybe_set_distributed_sampler_epoch,
     _reset_module_training_mode,
     _run_callback_fn,
     _set_module_training_mode,
     _step_requires_iterator,
     log_api_usage,
 )
-from torchtnt.utils.timer import get_timer_summary
+from torchtnt.utils.timer import get_timer_summary, Timer
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def init_train_state(
     *,
     dataloader: Iterable[TTrainData],
     max_epochs: Optional[int] = None,
     max_steps: Optional[int] = None,
     max_steps_per_epoch: Optional[int] = None,
+    auto_timing: bool = False,
 ) -> State:
     """
     ``init_train_state`` is a helper function that initializes a :class:`~torchtnt.framework.State` object for training. This :class:`~torchtnt.framework.State` object
     can then be passed to the :func:`~torchtnt.framework.train` entry point.
 
     Args:
         dataloader: dataloader to be used during training, which can be *any* iterable, including PyTorch DataLoader, DataLoader2, etc.
         max_epochs: the max number of epochs to run. ``None`` means no limit (infinite training) unless stopped by max_steps.
         max_steps: the max number of steps to run. ``None`` means no limit (infinite training) unless stopped by max_epochs.
         max_steps_per_epoch: the max number of steps to run per epoch. None means train until the dataloader is exhausted.
+        auto_timing: whether to automatically time the training loop, using the state's timer (enabling auto_timing may degrade performance).
 
     Returns:
         An initialized state object containing metadata.
 
     Below is an example of calling :py:func:`~torchtnt.framework.init_train_state` and :py:func:`~torchtnt.framework.train` together.
 
     .. code-block:: python
 
-      from torchtnt.framework import init_train_state, train
+        from torchtnt.framework import init_train_state, train
 
-      train_unit = MyTrainUnit(module=..., optimizer=..., lr_scheduler=...)
-      dataloader = torch.utils.data.DataLoader(...)
-      state = init_train_state(dataloader=dataloader, max_epochs=4)
-      train(state, train_unit)
+        train_unit = MyTrainUnit(module=..., optimizer=..., lr_scheduler=...)
+        dataloader = torch.utils.data.DataLoader(...)
+        state = init_train_state(dataloader=dataloader, max_epochs=4)
+        train(state, train_unit)
 
     """
 
     return State(
         entry_point=EntryPoint.TRAIN,
         train_state=PhaseState(
             dataloader=dataloader,
             max_epochs=max_epochs,
             max_steps=max_steps,
             max_steps_per_epoch=max_steps_per_epoch,
         ),
+        timer=None if not auto_timing else Timer(),
     )
 
 
 @torch.enable_grad()
 def train(
     state: State,
     train_unit: TTrainUnit,
@@ -88,29 +93,50 @@
         train_unit: an instance of :class:`~torchtnt.framework.TrainUnit` which implements `train_step`.
         callbacks: an optional list of callbacks.
 
     Below is an example of calling :py:func:`~torchtnt.framework.init_train_state` and :py:func:`~torchtnt.framework.train` together.
 
     .. code-block:: python
 
-      from torchtnt.framework import init_train_state, train
-
-      train_unit = MyTrainUnit(module=..., optimizer=..., lr_scheduler=...)
-      dataloader = torch.utils.data.DataLoader(...)
-      state = init_train_state(dataloader=dataloader, max_epochs=4)
-      train(state, train_unit)
+        from torchtnt.framework import init_train_state, train
 
+        train_unit = MyTrainUnit(module=..., optimizer=..., lr_scheduler=...)
+        dataloader = torch.utils.data.DataLoader(...)
+        state = init_train_state(dataloader=dataloader, max_epochs=4)
+        train(state, train_unit)
+
+    Below is pseudocode of what the :py:func:`~torchtnt.framework.train` entry point does.
+
+    .. code-block:: text
+
+        set unit's tracked modules to train mode
+        call on_train_start on unit first and then callbacks
+        while training is not done:
+            while epoch is not done:
+                call on_train_epoch_start on unit first and then callbacks
+                try:
+                    data = next(dataloader)
+                    call on_train_step_start on callbacks
+                    call train_step on unit
+                    increment step counter
+                    call on_train_step_end on callbacks
+                except StopIteration:
+                    break
+            increment epoch counter
+            call on_train_epoch_end on unit first and then callbacks
+        call on_train_end on unit first and then callbacks
     """
     log_api_usage("train")
     callbacks = callbacks or []
     try:
         state._entry_point = EntryPoint.TRAIN
         _train_impl(state, train_unit, callbacks)
         logger.info("Finished train")
-        logger.debug(get_timer_summary(state.timer))
+        if state.timer:
+            logger.info(get_timer_summary(state.timer))
     except Exception as e:
         # TODO: log for diagnostics
         logger.info(f"Exception during train\n: {e}")
         train_unit.on_exception(state, e)
         _run_callback_fn(callbacks, "on_exception", state, train_unit, e)
         raise e
 
@@ -128,25 +154,29 @@
     state._active_phase = ActivePhase.TRAIN
 
     # Set all modules to train() mode
     # access modules made available through _AppStateMixin
     tracked_modules = train_unit.tracked_modules()
     prior_module_train_states = _set_module_training_mode(tracked_modules, True)
 
-    with state.timer.time(f"train.{train_unit.__class__.__name__}.on_train_start"):
+    with _get_timing_context(
+        state, f"train.{train_unit.__class__.__name__}.on_train_start"
+    ):
         train_unit.on_train_start(state)
     _run_callback_fn(callbacks, "on_train_start", state, train_unit)
 
     while not (
         state.should_stop
         or _is_done(train_state.progress, train_state.max_epochs, train_state.max_steps)
     ):
         _train_epoch_impl(state, train_unit, callbacks)
 
-    with state.timer.time(f"train.{train_unit.__class__.__name__}.on_train_end"):
+    with _get_timing_context(
+        state, f"train.{train_unit.__class__.__name__}.on_train_end"
+    ):
         train_unit.on_train_end(state)
     _run_callback_fn(callbacks, "on_train_end", state, train_unit)
 
     # Reset training mode for modules at the end of the epoch
     # This ensures that side-effects made by the loop are reset before
     # returning back to the user
     _reset_module_training_mode(tracked_modules, prior_module_train_states)
@@ -182,15 +212,16 @@
         )
         _train_epoch_impl(
             state,
             train_unit,
             callbacks,
         )
         logger.info("Finished train")
-        logger.debug(get_timer_summary(state.timer))
+        if state.timer:
+            logger.info(get_timer_summary(state.timer))
     except Exception as e:
         # TODO: log for diagnostics
         logger.info(f"Exception during train_epoch\n: {e}")
         train_unit.on_exception(state, e)
         _run_callback_fn(callbacks, "on_exception", state, train_unit, e)
         raise e
 
@@ -218,113 +249,98 @@
         if state.eval_state.evaluate_every_n_epochs:
             evaluate_every_n_epochs = state.eval_state.evaluate_every_n_epochs
 
     # Check the progress to conditionally run this
     # to avoid running this multiple times
     # in the case of resuming from a checkpoint mid-epoch
     if train_state.progress.num_steps_completed_in_epoch == 0:
-        with state.timer.time(
-            f"train.{train_unit.__class__.__name__}.on_train_epoch_start"
+        with _get_timing_context(
+            state, f"train.{train_unit.__class__.__name__}.on_train_epoch_start"
         ):
             train_unit.on_train_epoch_start(state)
         _run_callback_fn(callbacks, "on_train_epoch_start", state, train_unit)
 
     _maybe_set_distributed_sampler_epoch(
         train_state.dataloader, train_state.progress.num_epochs_completed
     )
 
-    data_iter = iter(train_state.dataloader)
+    with record_function(__name__ + ".iter(dataloader)"):
+        data_iter = iter(train_state.dataloader)
     step_input = data_iter
 
     pass_data_iter_to_step = _step_requires_iterator(train_unit.train_step)
     prev_steps_in_epoch = train_state.progress.num_steps_completed_in_epoch
 
-    # Prefetch each batch while iterating over the data, so that we can set the
-    # _is_last_batch field on the train_state and pass that metadata to the user
-    if not pass_data_iter_to_step:
-        try:
-            # get the first batch from the data iterator
-            step_input = next(data_iter)
-        except StopIteration:
-            raise RuntimeError("Dataloader is empty")
-
-    # set is_last_batch to False before starting the loop. it will only be modified inside the loop
-    train_state._is_last_batch = False
-
-    while not state.should_stop and not train_state.is_last_batch:
+    while not (
+        state.should_stop
+        or _is_epoch_done(
+            train_state.progress, train_state.max_steps_per_epoch, train_state.max_steps
+        )
+    ):
         try:
-            # get the next batch from the data iterator
             if not pass_data_iter_to_step:
-                next_step_input = next(data_iter)
-
-            # update train_state._is_last_batch
-            train_state._is_last_batch = _is_last_batch_in_epoch(
-                train_state.progress,
-                train_state.max_steps_per_epoch,
-                train_state.max_steps,
-            )
+                # get the next batch from the data iterator
+                with record_function(__name__ + ".next(data_iter)"):
+                    step_input = next(data_iter)
+
+            _run_callback_fn(callbacks, "on_train_step_start", state, train_unit)
+            with _get_timing_context(
+                state, f"train.{train_unit.__class__.__name__}.train_step"
+            ), record_function(__name__ + ".train_step"):
+                train_state._step_output = train_unit.train_step(state, step_input)
+            train_state.progress.increment_step()
+            _run_callback_fn(callbacks, "on_train_step_end", state, train_unit)
 
-        except StopIteration:
-            train_state._is_last_batch = True
+            # clear step_output to avoid retaining extra memory
+            train_state._step_output = None
 
-        _run_callback_fn(callbacks, "on_train_step_start", state, train_unit)
-        with state.timer.time(f"train.{train_unit.__class__.__name__}.train_step"):
-            try:
-                train_state._step_output = train_unit.train_step(state, step_input)
-            except StopIteration:
-                # catch a StopIteration for the case where the train_step takes in an iterator
-                break
-
-        train_state.progress.increment_step()
-        _run_callback_fn(callbacks, "on_train_step_end", state, train_unit)
-
-        # clear step_output to avoid retaining extra memory
-        train_state._step_output = None
-
-        if (
-            evaluate_every_n_steps
-            and train_state.progress.num_steps_completed_in_epoch
-            % evaluate_every_n_steps
-            == 0
-        ):
-            _evaluate_impl(
-                state,
-                # pyre-ignore: Incompatible parameter type [6]
-                train_unit,
-                callbacks,
-            )
+            if (
+                evaluate_every_n_steps
+                and train_state.progress.num_steps_completed % evaluate_every_n_steps
+                == 0
+            ):
+                _evaluate_impl(
+                    state,
+                    # pyre-ignore: Incompatible parameter type [6]
+                    train_unit,
+                    callbacks,
+                )
+                logger.info("Finished evaluation. Resuming training epoch")
+                state._active_phase = ActivePhase.TRAIN
 
-        if not pass_data_iter_to_step:
-            # pyre-ignore
-            step_input = next_step_input
+        except StopIteration:
+            break
 
     # Possibly warn about an empty dataloader
     any_steps_completed = (
         abs(train_state.progress.num_steps_completed_in_epoch - prev_steps_in_epoch) > 0
     )
     if not any_steps_completed:
         logger.warning("No steps completed during train epoch!")
 
     # set progress counters for the next epoch
     train_state.progress.increment_epoch()
 
-    with state.timer.time(f"train.{train_unit.__class__.__name__}.on_train_epoch_end"):
+    with _get_timing_context(
+        state, f"train.{train_unit.__class__.__name__}.on_train_epoch_end"
+    ):
         train_unit.on_train_epoch_end(state)
     _run_callback_fn(callbacks, "on_train_epoch_end", state, train_unit)
 
     if (
         evaluate_every_n_epochs
         and train_state.progress.num_epochs_completed % evaluate_every_n_epochs == 0
     ):
         _evaluate_impl(
             state,
             # pyre-ignore: Incompatible parameter type [6]
             train_unit,
             callbacks,
         )
+        state._active_phase = ActivePhase.TRAIN
 
     # Reset training mode for modules at the end of the epoch
     # This ensures that side-effects made by the loop are reset before
     # returning back to the user
     _reset_module_training_mode(tracked_modules, prior_module_train_states)
 
     logger.info("Ended train epoch")
```

### Comparing `torchtnt-0.0.7/torchtnt/framework/unit.py` & `torchtnt-0.1.0/torchtnt/framework/unit.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/framework/utils.py` & `torchtnt-0.1.0/torchtnt/framework/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,23 +3,33 @@
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import collections
 import inspect
 import logging
-from typing import Any, Callable, Dict, Iterable, List, Optional
+from typing import Any, Callable, ContextManager, Dict, Iterable, List, Optional
 
 import torch
 import torch.nn as nn
 import typing_extensions
+from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
 
+from torchtnt.utils.version import is_torch_version_geq_2_0
+
+if is_torch_version_geq_2_0():
+    from torch.distributed._composable_state import _get_module_state
+    from torch.distributed.fsdp._common_utils import _FSDPState
+
+import contextlib
+
+from pyre_extensions import none_throws
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.progress import Progress
-from torchtnt.framework.state import State
+from torchtnt.framework.state import ActivePhase, EntryPoint, State
 from typing_extensions import Self
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 # Helper functions common across the loops
 def _is_done(
@@ -35,25 +45,14 @@
 ) -> bool:
     return (max_steps is not None and progress.num_steps_completed >= max_steps) or (
         max_steps_per_epoch is not None
         and progress.num_steps_completed_in_epoch >= max_steps_per_epoch
     )
 
 
-def _is_last_batch_in_epoch(
-    progress: Progress, max_steps_per_epoch: Optional[int], max_steps: Optional[int]
-) -> bool:
-    return (
-        max_steps is not None and progress.num_steps_completed >= max_steps - 1
-    ) or (
-        max_steps_per_epoch is not None
-        and progress.num_steps_completed_in_epoch >= max_steps_per_epoch - 1
-    )
-
-
 def _maybe_set_distributed_sampler_epoch(
     # pyre-ignore: Missing parameter annotation [2]
     dataloader: Iterable[Any],
     current_epoch: int,
 ) -> None:
     """Set epoch of distributed sampler in dataloader, if applicable.
     See: https://pytorch.org/docs/stable/data.html#torch.utils.data.distributed.DistributedSampler
@@ -84,26 +83,30 @@
     # This ensures that side-effects made by the loop are reset before
     # returning back to the user
     for name, module in modules.items():
         if name in prior_modes:
             module.train(prior_modes[name])
 
 
+def _get_timing_context(state: State, event_name: str) -> ContextManager:
+    return state.timer.time(event_name) if state.timer else contextlib.nullcontext()
+
+
 def _run_callback_fn(
     callbacks: List[Callback],
     fn_name: str,
     state: State,
     *args: Any,
     **kwargs: Any,
 ) -> None:
     for cb in callbacks:
         fn = getattr(cb, fn_name)
         if not callable(fn):
             raise ValueError(f"Invalid callback method name provided: {fn_name}")
-        with state.timer.time(f"callback.{cb.name}.{fn_name}"):
+        with _get_timing_context(state, f"callback.{cb.name}.{fn_name}"):
             fn(state, *args, **kwargs)
 
 
 def log_api_usage(entry_point: str) -> None:
     torch._C._log_api_usage_once(f"torchtnt.framework.{entry_point}")
 
 
@@ -121,14 +124,41 @@
             f"Expected step function to have an annotated argument named ``data``. Found {annotations}."
         )
         return False
     annotated_type = annotations["data"]
     return typing_extensions.get_origin(annotated_type) is collections.abc.Iterator
 
 
+def _is_fsdp_module(module: torch.nn.Module) -> bool:
+    if isinstance(module, FSDP):
+        return True
+
+    if is_torch_version_geq_2_0():
+        # Also check for composable FSDP API
+        maybe_composable_state = _get_module_state(module)
+        if maybe_composable_state is not None:
+            return isinstance(maybe_composable_state, _FSDPState)
+
+    return False
+
+
+def get_current_progress(state: State) -> Progress:
+    """
+    If state's entry point is fit, returns train progress. During fit, we want to return training progress even during eval, so that metrics can be compared easily across train and eval.
+    Otherwise, checks the active phase, and returns the corresponding progress class.
+    """
+    if state.entry_point == EntryPoint.FIT or state.active_phase == ActivePhase.TRAIN:
+        return none_throws(state.train_state).progress
+
+    if state.active_phase == ActivePhase.EVALUATE:
+        return none_throws(state.eval_state).progress
+    else:
+        return none_throws(state.predict_state).progress
+
+
 class StatefulInt:
     """
     This wrapper is useful if there are additional values related to training
     progress that need to be saved during checkpointing.
     """
 
     def __init__(self, val: int) -> None:
```

### Comparing `torchtnt-0.0.7/torchtnt/utils/__init__.py` & `torchtnt-0.1.0/torchtnt/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     copy_data_to_device,
     CPUStats,
     get_device_from_env,
     get_nvidia_smi_gpu_stats,
     get_psutil_cpu_stats,
     GPUStats,
     maybe_enable_tf32,
+    record_data_in_stream,
 )
 from .distributed import (
     all_gather_tensors,
     get_global_rank,
     get_process_group_backend_from_device,
     get_world_size,
     PGWrapper,
@@ -57,14 +58,15 @@
     "copy_data_to_device",
     "CPUStats",
     "get_device_from_env",
     "get_nvidia_smi_gpu_stats",
     "get_psutil_cpu_stats",
     "GPUStats",
     "maybe_enable_tf32",
+    "record_data_in_stream",
     "all_gather_tensors",
     "get_global_rank",
     "get_process_group_backend_from_device",
     "get_world_size",
     "PGWrapper",
     "sync_bool",
     "EarlyStopChecker",
```

### Comparing `torchtnt-0.0.7/torchtnt/utils/data/__init__.py` & `torchtnt-0.1.0/torchtnt/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/data/data_prefetcher.py` & `torchtnt-0.1.0/torchtnt/utils/data/data_prefetcher.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/data/iterators.py` & `torchtnt-0.1.0/torchtnt/utils/data/iterators.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/data/multi_dataloader.py` & `torchtnt-0.1.0/torchtnt/utils/data/multi_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/device.py` & `torchtnt-0.1.0/torchtnt/utils/device.py`

 * *Files 20% similar despite different names*

```diff
@@ -119,14 +119,63 @@
                 )
         return new_data_class
     elif isinstance(data, _CopyableData):
         return data.to(device, *args, **kwargs)
     return data
 
 
+def record_data_in_stream(data: T, stream: torch.cuda.streams.Stream) -> None:
+    """
+    As mentioned in
+    https://pytorch.org/docs/stable/generated/torch.Tensor.record_stream.html, PyTorch
+    uses the "caching allocator" for memory allocation for tensors. When a tensor is
+    freed, its memory is likely to be reused by newly constructed tensors. By default,
+    this allocator traces whether a tensor is still in use by only the CUDA stream where
+    it was created. When a tensor is used by additional CUDA streams, we need to call
+    `record_stream` to tell the allocator about these streams. Otherwise, the allocator
+    might free the underlying memory of the tensor once it is no longer used by the
+    creator stream. This is a notable programming trick when we write programs using
+    multiple CUDA streams.
+
+    Args:
+        data: The data on which to call record_stream
+        stream: The CUDA stream with which to call record_stream
+    """
+
+    # Redundant isinstance(data, tuple) check is required here to make pyre happy
+    if _is_named_tuple(data) and isinstance(data, tuple):
+        record_data_in_stream(data._asdict(), stream)
+    elif isinstance(data, (list, tuple)):
+        for e in data:
+            record_data_in_stream(e, stream)
+    elif isinstance(data, Mapping):
+        for _, v in data.items():
+            record_data_in_stream(v, stream)
+    elif is_dataclass(data) and not isinstance(data, type):
+        for field in fields(data):
+            record_data_in_stream(getattr(data, field.name), stream)
+    elif isinstance(data, _MultistreamableData):
+        data.record_stream(stream)
+
+
+@runtime_checkable
+class _MultistreamableData(Protocol):
+    """
+    Objects implementing this interface are allowed to be transferred
+    from one CUDA stream to another.
+    torch.Tensor implements this interface.
+    """
+
+    def record_stream(self, stream: torch.cuda.streams.Stream) -> None:
+        """
+        See https://pytorch.org/docs/stable/generated/torch.Tensor.record_stream.html
+        """
+        ...
+
+
 class GPUStats(TypedDict):
     utilization_gpu_percent: float
     utilization_memory_percent: float
     fan_speed_percent: float
     memory_used_mb: int
     memory_free_mb: int
     temperature_gpu_celsius: float
```

### Comparing `torchtnt-0.0.7/torchtnt/utils/distributed.py` & `torchtnt-0.1.0/torchtnt/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/early_stop_checker.py` & `torchtnt-0.1.0/torchtnt/utils/early_stop_checker.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/env.py` & `torchtnt-0.1.0/torchtnt/utils/env.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/fsspec.py` & `torchtnt-0.1.0/torchtnt/utils/fsspec.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/loggers/__init__.py` & `torchtnt-0.1.0/torchtnt/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/loggers/csv.py` & `torchtnt-0.1.0/torchtnt/utils/loggers/csv.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/loggers/file.py` & `torchtnt-0.1.0/torchtnt/utils/loggers/file.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/loggers/in_memory.py` & `torchtnt-0.1.0/torchtnt/utils/loggers/in_memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/loggers/json.py` & `torchtnt-0.1.0/torchtnt/utils/loggers/json.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/loggers/logger.py` & `torchtnt-0.1.0/torchtnt/utils/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/loggers/tensorboard.py` & `torchtnt-0.1.0/torchtnt/utils/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/loggers/utils.py` & `torchtnt-0.1.0/torchtnt/utils/loggers/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/memory.py` & `torchtnt-0.1.0/torchtnt/utils/memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/misc.py` & `torchtnt-0.1.0/torchtnt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/oom.py` & `torchtnt-0.1.0/torchtnt/utils/oom.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/rank_zero_log.py` & `torchtnt-0.1.0/torchtnt/utils/rank_zero_log.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/seed.py` & `torchtnt-0.1.0/torchtnt/utils/seed.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/test_utils.py` & `torchtnt-0.1.0/torchtnt/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/timer.py` & `torchtnt-0.1.0/torchtnt/utils/timer.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt/utils/version.py` & `torchtnt-0.1.0/torchtnt/utils/version.py`

 * *Files identical despite different names*

### Comparing `torchtnt-0.0.7/torchtnt.egg-info/PKG-INFO` & `torchtnt-0.1.0/torchtnt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt
-Version: 0.0.7
+Version: 0.1.0
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -23,28 +23,34 @@
 ==========
 
 **TNT** is a library for PyTorch **t**rai**n**ing **t**ools and utilities.
 
 <p align="center">
 <a href="https://github.com/pytorch/tnt/actions?query=branch%3Amaster"><img src="https://img.shields.io/github/actions/workflow/status/pytorch/tnt/test.yml?branch=master" alt="build status"></a>
 <a href="https://pypi.org/project/torchtnt"><img src="https://img.shields.io/pypi/v/torchtnt" alt="pypi version"></a>
+<a href="https://anaconda.org/conda-forge/torchtnt"><img src="https://img.shields.io/conda/vn/conda-forge/torchtnt" alt="pypi version"></a>
 <a href="https://pypi.org/project/torchtnt-nightly"><img src="https://img.shields.io/pypi/v/torchtnt-nightly?label=nightly" alt="pypi nightly version"></a>
 <a href="https://codecov.io/gh/pytorch/tnt"><img src="https://codecov.io/gh/pytorch/tnt/branch/master/graph/badge.svg?token=DR67Q6T7YF" alt="codecov"></a>
 <a href="https://github.com/pytorch/tnt/blob/master/LICENSE"><img src="https://img.shields.io/pypi/l/torchtnt" alt="bsd license"></a>
 <a href="https://pytorch.org/tnt/"><img src="https://img.shields.io/badge/dynamic/json.svg?label=docs&url=https%3A%2F%2Fpypi.org%2Fpypi%2Ftorchtnt%2Fjson&query=%24.info.version&colorB=brightgreen&prefix=v" alt="documentation status"></a>
 </div>
 
 
 ## Installation
 
-TNT can be installed with pip. To do so, run:
+TNT can be installed with pip:
 
 ```buildoutcfg
 pip install torchtnt
 ```
+Or, alternatively, via conda:
+
+```buildoutcfg
+conda install -c conda-forge torchtnt
+```
 
 If you run into issues, make sure that Pytorch is installed first.
 
 You can also install the latest version from master. Just run:
 
 ```buildoutcfg
 pip install git+https://github.com/pytorch/tnt.git@master
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: torchtnt Version: 0.0.7 Summary: A lightweight
+Metadata-Version: 2.1 Name: torchtnt Version: 0.1.0 Summary: A lightweight
 library for PyTorch training tools and utilities Home-page: https://github.com/
 pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com License: BSD-
 3 Keywords: pytorch,torch,training,tools,utilities Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev License-File: LICENSE TNT
 ========== **TNT** is a library for PyTorch **t**rai**n**ing **t**ools and
 utilities.
- [build_status] [pypi_version] [pypi_nightly_version] [codecov] [bsd_license]
-                            [documentation_status]
-## Installation TNT can be installed with pip. To do so, run: ```buildoutcfg
-pip install torchtnt ``` If you run into issues, make sure that Pytorch is
+[build_status] [pypi_version] [pypi_version] [pypi_nightly_version] [codecov]
+                     [bsd_license] [documentation_status]
+## Installation TNT can be installed with pip: ```buildoutcfg pip install
+torchtnt ``` Or, alternatively, via conda: ```buildoutcfg conda install -
+c conda-forge torchtnt ``` If you run into issues, make sure that Pytorch is
 installed first. You can also install the latest version from master. Just run:
 ```buildoutcfg pip install git+https://github.com/pytorch/tnt.git@master ``` To
 update to the latest version from master: ```buildoutcfg pip install --upgrade
 git+https://github.com/pytorch/tnt.git@master ```
```

### Comparing `torchtnt-0.0.7/torchtnt.egg-info/SOURCES.txt` & `torchtnt-0.1.0/torchtnt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 torchtnt/framework/callbacks/learning_rate_monitor.py
 torchtnt/framework/callbacks/module_summary.py
 torchtnt/framework/callbacks/pytorch_profiler.py
 torchtnt/framework/callbacks/system_resources_monitor.py
 torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
 torchtnt/framework/callbacks/torchsnapshot_saver.py
 torchtnt/framework/callbacks/tqdm_progress_bar.py
+torchtnt/framework/callbacks/train_progress_monitor.py
 torchtnt/utils/__init__.py
 torchtnt/utils/device.py
 torchtnt/utils/distributed.py
 torchtnt/utils/early_stop_checker.py
 torchtnt/utils/env.py
 torchtnt/utils/fsspec.py
 torchtnt/utils/lr_scheduler.py
```

