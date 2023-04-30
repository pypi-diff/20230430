# Comparing `tmp/lightning-template-1.0.0.tar.gz` & `tmp/lightning-template-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-template-1.0.0.tar", last modified: Sun Apr 30 10:33:11 2023, max compression
+gzip compressed data, was "lightning-template-1.0.1.tar", last modified: Sun Apr 30 11:18:16 2023, max compression
```

## Comparing `lightning-template-1.0.0.tar` & `lightning-template-1.0.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 10:33:11.964002 lightning-template-1.0.0/
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     1069 2023-04-30 06:59:59.000000 lightning-template-1.0.0/LICENSE
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     3638 2023-04-30 10:33:11.964002 lightning-template-1.0.0/PKG-INFO
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     2466 2023-04-30 06:58:39.000000 lightning-template-1.0.0/README.md
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 10:33:11.700004 lightning-template-1.0.0/lightning_template/
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)       16 2023-04-30 08:25:07.000000 lightning-template-1.0.0/lightning_template/__init__.py
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 10:33:11.808003 lightning-template-1.0.0/lightning_template/datasets/
--rwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)       61 2023-04-30 06:58:39.000000 lightning-template-1.0.0/lightning_template/datasets/__init__.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     7180 2023-04-30 08:37:59.000000 lightning-template-1.0.0/lightning_template/datasets/base.py
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 10:33:11.828003 lightning-template-1.0.0/lightning_template/models/
--rwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)       53 2023-04-30 06:58:40.000000 lightning-template-1.0.0/lightning_template/models/__init__.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     4286 2023-04-30 08:59:49.000000 lightning-template-1.0.0/lightning_template/models/base.py
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 10:33:11.856003 lightning-template-1.0.0/lightning_template/tools/
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)       16 2023-04-30 08:25:22.000000 lightning-template-1.0.0/lightning_template/tools/__init__.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)      127 2023-04-30 08:39:24.000000 lightning-template-1.0.0/lightning_template/tools/cli.py
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 10:33:11.864003 lightning-template-1.0.0/lightning_template/tools/model/
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)       16 2023-04-30 08:25:29.000000 lightning-template-1.0.0/lightning_template/tools/model/__init__.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)      936 2023-04-30 08:39:40.000000 lightning-template-1.0.0/lightning_template/tools/model/batch_size_finder.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     2057 2023-04-30 08:39:51.000000 lightning-template-1.0.0/lightning_template/tools/model/calculate_MACs_and_params.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)      460 2023-04-30 08:39:45.000000 lightning-template-1.0.0/lightning_template/tools/model/lr_finder.py
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 10:33:11.868003 lightning-template-1.0.0/lightning_template/utils/
--rwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)       35 2023-04-30 08:25:53.000000 lightning-template-1.0.0/lightning_template/utils/__init__.py
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 10:33:11.916002 lightning-template-1.0.0/lightning_template/utils/callbacks/
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)       16 2023-04-30 08:27:04.000000 lightning-template-1.0.0/lightning_template/utils/callbacks/__init__.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     1628 2023-04-30 06:58:40.000000 lightning-template-1.0.0/lightning_template/utils/callbacks/model_checkpoint.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)      548 2023-04-30 06:58:40.000000 lightning-template-1.0.0/lightning_template/utils/callbacks/save_and_log_config_callback.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     1731 2023-04-30 06:58:40.000000 lightning-template-1.0.0/lightning_template/utils/callbacks/set_precision_and_cudnn_callback.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)      912 2023-04-30 06:58:40.000000 lightning-template-1.0.0/lightning_template/utils/callbacks/set_sharing_strategy_callback.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     1451 2023-04-30 06:58:40.000000 lightning-template-1.0.0/lightning_template/utils/callbacks/set_wandb_logger_callback.py
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 10:33:11.932002 lightning-template-1.0.0/lightning_template/utils/cli/
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)      118 2023-04-30 08:38:56.000000 lightning-template-1.0.0/lightning_template/utils/cli/__init__.py
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 10:33:11.940002 lightning-template-1.0.0/lightning_template/utils/cli/argument_parsers/
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)      193 2023-04-30 06:58:41.000000 lightning-template-1.0.0/lightning_template/utils/cli/argument_parsers/__init__.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     5527 2023-04-30 06:58:41.000000 lightning-template-1.0.0/lightning_template/utils/cli/argument_parsers/deep_update.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     2315 2023-04-30 06:58:41.000000 lightning-template-1.0.0/lightning_template/utils/cli/argument_parsers/json_file_action.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     3934 2023-04-30 06:58:41.000000 lightning-template-1.0.0/lightning_template/utils/cli/argument_parsers/yaml_with_merge.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     3755 2023-04-30 08:38:38.000000 lightning-template-1.0.0/lightning_template/utils/cli/cli.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     1284 2023-04-30 06:58:41.000000 lightning-template-1.0.0/lightning_template/utils/cli/trainer.py
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 10:33:11.944002 lightning-template-1.0.0/lightning_template/utils/loggers/
--rwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)       36 2023-04-30 06:58:41.000000 lightning-template-1.0.0/lightning_template/utils/loggers/__init__.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)      681 2023-04-30 09:29:40.000000 lightning-template-1.0.0/lightning_template/utils/loggers/wandb.py
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 10:33:11.948002 lightning-template-1.0.0/lightning_template/utils/loop/
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)       28 2023-04-30 06:58:41.000000 lightning-template-1.0.0/lightning_template/utils/loop/__init__.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     3045 2023-04-30 06:58:41.000000 lightning-template-1.0.0/lightning_template/utils/loop/kfold.py
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 10:33:11.956002 lightning-template-1.0.0/lightning_template/utils/optim/
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)      197 2023-04-30 06:58:41.000000 lightning-template-1.0.0/lightning_template/utils/optim/__init__.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     5984 2023-04-30 09:07:29.000000 lightning-template-1.0.0/lightning_template/utils/optim/configure_optimizers.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     1166 2023-04-30 06:58:41.000000 lightning-template-1.0.0/lightning_template/utils/optim/keep_and_linearly_decay_lr_scheduler.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     1971 2023-04-30 06:58:41.000000 lightning-template-1.0.0/lightning_template/utils/optim/warmup_lr_scheduler.py
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 10:33:11.960002 lightning-template-1.0.0/lightning_template/utils/progress/
--rwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)       16 2023-04-30 08:27:24.000000 lightning-template-1.0.0/lightning_template/utils/progress/__init__.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     2089 2023-04-30 06:58:41.000000 lightning-template-1.0.0/lightning_template/utils/progress/rich_progress.py
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 10:33:11.748004 lightning-template-1.0.0/lightning_template.egg-info/
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     3638 2023-04-30 10:33:11.000000 lightning-template-1.0.0/lightning_template.egg-info/PKG-INFO
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     1991 2023-04-30 10:33:11.000000 lightning-template-1.0.0/lightning_template.egg-info/SOURCES.txt
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)        1 2023-04-30 10:33:11.000000 lightning-template-1.0.0/lightning_template.egg-info/dependency_links.txt
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)      190 2023-04-30 10:33:11.000000 lightning-template-1.0.0/lightning_template.egg-info/entry_points.txt
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)       48 2023-04-30 10:33:11.000000 lightning-template-1.0.0/lightning_template.egg-info/requires.txt
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)       19 2023-04-30 10:33:11.000000 lightning-template-1.0.0/lightning_template.egg-info/top_level.txt
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)       38 2023-04-30 10:33:11.964002 lightning-template-1.0.0/setup.cfg
--rwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)     1838 2023-04-30 10:29:31.000000 lightning-template-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:18:16.739256 lightning-template-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-30 11:17:58.000000 lightning-template-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-30 11:18:16.739256 lightning-template-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-30 11:17:58.000000 lightning-template-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:18:16.731255 lightning-template-1.0.1/lightning_template/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:18:16.731255 lightning-template-1.0.1/lightning_template/datasets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/datasets/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:18:16.731255 lightning-template-1.0.1/lightning_template/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:18:16.731255 lightning-template-1.0.1/lightning_template/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/tools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:18:16.735256 lightning-template-1.0.1/lightning_template/tools/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/tools/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/tools/model/batch_size_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/tools/model/calculate_MACs_and_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/tools/model/lr_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:18:16.735256 lightning-template-1.0.1/lightning_template/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       35 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:18:16.735256 lightning-template-1.0.1/lightning_template/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/callbacks/save_and_log_config_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/callbacks/set_precision_and_cudnn_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/callbacks/set_sharing_strategy_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/callbacks/set_wandb_logger_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:18:16.735256 lightning-template-1.0.1/lightning_template/utils/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:18:16.735256 lightning-template-1.0.1/lightning_template/utils/cli/argument_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/cli/argument_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/cli/argument_parsers/deep_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/cli/argument_parsers/json_file_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/cli/argument_parsers/yaml_with_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/cli/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:18:16.735256 lightning-template-1.0.1/lightning_template/utils/loggers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       36 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/loggers/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:18:16.735256 lightning-template-1.0.1/lightning_template/utils/loop/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/loop/kfold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:18:16.735256 lightning-template-1.0.1/lightning_template/utils/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/optim/configure_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/optim/keep_and_linearly_decay_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/optim/warmup_lr_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:18:16.735256 lightning-template-1.0.1/lightning_template/utils/progress/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       16 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-30 11:17:58.000000 lightning-template-1.0.1/lightning_template/utils/progress/rich_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:18:16.731255 lightning-template-1.0.1/lightning_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-30 11:18:16.000000 lightning-template-1.0.1/lightning_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-30 11:18:16.000000 lightning-template-1.0.1/lightning_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 11:18:16.000000 lightning-template-1.0.1/lightning_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-30 11:18:16.000000 lightning-template-1.0.1/lightning_template.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-30 11:18:16.000000 lightning-template-1.0.1/lightning_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 11:18:16.000000 lightning-template-1.0.1/lightning_template.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 11:18:16.739256 lightning-template-1.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1838 2023-04-30 11:17:58.000000 lightning-template-1.0.1/setup.py
```

### Comparing `lightning-template-1.0.0/LICENSE` & `lightning-template-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/PKG-INFO` & `lightning-template-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-template
-Version: 1.0.0
+Version: 1.0.1
 Summary: A template wrapper for pytorch-lightning.
 Home-page: https://github.com/shenmishajing/lightning_template
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/lightning_template
 Project-URL: Issue tracker, https://github.com/shenmishajing/lightning_template/issues
@@ -23,15 +23,15 @@
 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Introduction
 
-A generic project template based on [pytorch lightning](https://pytorch-lightning.readthedocs.io/en/stable/)
+A generic project template lib based on [pytorch lightning](https://pytorch-lightning.readthedocs.io/en/stable/) for [project-template](https://github.com/shenmishajing/project_template)
 
 ## Feature
 
 - All features from [pytorch lightning](https://pytorch-lightning.readthedocs.io/en/stable/) and [lightning CLI](https://pytorch-lightning.readthedocs.io/en/stable/cli/lightning_cli.html). Especially, experiment manager feature, auto implement multi-node, multi-device, multi-accelerator support, etc.
 - Powerful [deep update](docs/configs/deep_update.md) feature for config file inherit to manage your config files in a more hierarchical way, see also [recommand config file structure](docs/configs/config_file_structure.md).
 - Multi and complex optimizers and lr_scheduler from CLI config support, see [doc](docs/core/optimizer_config.md).
 - Powerful and flexible LightningModule and LightningDataModule base class.
```

### Comparing `lightning-template-1.0.0/README.md` & `lightning-template-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ## Introduction
 
-A generic project template based on [pytorch lightning](https://pytorch-lightning.readthedocs.io/en/stable/)
+A generic project template lib based on [pytorch lightning](https://pytorch-lightning.readthedocs.io/en/stable/) for [project-template](https://github.com/shenmishajing/project_template)
 
 ## Feature
 
 - All features from [pytorch lightning](https://pytorch-lightning.readthedocs.io/en/stable/) and [lightning CLI](https://pytorch-lightning.readthedocs.io/en/stable/cli/lightning_cli.html). Especially, experiment manager feature, auto implement multi-node, multi-device, multi-accelerator support, etc.
 - Powerful [deep update](docs/configs/deep_update.md) feature for config file inherit to manage your config files in a more hierarchical way, see also [recommand config file structure](docs/configs/config_file_structure.md).
 - Multi and complex optimizers and lr_scheduler from CLI config support, see [doc](docs/core/optimizer_config.md).
 - Powerful and flexible LightningModule and LightningDataModule base class.
```

### Comparing `lightning-template-1.0.0/lightning_template/datasets/base.py` & `lightning-template-1.0.1/lightning_template/datasets/base.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/models/base.py` & `lightning-template-1.0.1/lightning_template/models/base.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/tools/model/batch_size_finder.py` & `lightning-template-1.0.1/lightning_template/tools/model/batch_size_finder.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/tools/model/calculate_MACs_and_params.py` & `lightning-template-1.0.1/lightning_template/tools/model/calculate_MACs_and_params.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/utils/callbacks/model_checkpoint.py` & `lightning-template-1.0.1/lightning_template/utils/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/utils/callbacks/save_and_log_config_callback.py` & `lightning-template-1.0.1/lightning_template/utils/callbacks/save_and_log_config_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/utils/callbacks/set_precision_and_cudnn_callback.py` & `lightning-template-1.0.1/lightning_template/utils/callbacks/set_precision_and_cudnn_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/utils/callbacks/set_sharing_strategy_callback.py` & `lightning-template-1.0.1/lightning_template/utils/callbacks/set_sharing_strategy_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/utils/callbacks/set_wandb_logger_callback.py` & `lightning-template-1.0.1/lightning_template/utils/callbacks/set_wandb_logger_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/utils/cli/argument_parsers/deep_update.py` & `lightning-template-1.0.1/lightning_template/utils/cli/argument_parsers/deep_update.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/utils/cli/argument_parsers/json_file_action.py` & `lightning-template-1.0.1/lightning_template/utils/cli/argument_parsers/json_file_action.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/utils/cli/argument_parsers/yaml_with_merge.py` & `lightning-template-1.0.1/lightning_template/utils/cli/argument_parsers/yaml_with_merge.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/utils/cli/cli.py` & `lightning-template-1.0.1/lightning_template/utils/cli/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/utils/cli/trainer.py` & `lightning-template-1.0.1/lightning_template/utils/cli/trainer.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/utils/loggers/wandb.py` & `lightning-template-1.0.1/lightning_template/utils/loggers/wandb.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/utils/loop/kfold.py` & `lightning-template-1.0.1/lightning_template/utils/loop/kfold.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/utils/optim/configure_optimizers.py` & `lightning-template-1.0.1/lightning_template/utils/optim/configure_optimizers.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/utils/optim/keep_and_linearly_decay_lr_scheduler.py` & `lightning-template-1.0.1/lightning_template/utils/optim/keep_and_linearly_decay_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/utils/optim/warmup_lr_scheduler.py` & `lightning-template-1.0.1/lightning_template/utils/optim/warmup_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template/utils/progress/rich_progress.py` & `lightning-template-1.0.1/lightning_template/utils/progress/rich_progress.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/lightning_template.egg-info/PKG-INFO` & `lightning-template-1.0.1/lightning_template.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-template
-Version: 1.0.0
+Version: 1.0.1
 Summary: A template wrapper for pytorch-lightning.
 Home-page: https://github.com/shenmishajing/lightning_template
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/lightning_template
 Project-URL: Issue tracker, https://github.com/shenmishajing/lightning_template/issues
@@ -23,15 +23,15 @@
 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Introduction
 
-A generic project template based on [pytorch lightning](https://pytorch-lightning.readthedocs.io/en/stable/)
+A generic project template lib based on [pytorch lightning](https://pytorch-lightning.readthedocs.io/en/stable/) for [project-template](https://github.com/shenmishajing/project_template)
 
 ## Feature
 
 - All features from [pytorch lightning](https://pytorch-lightning.readthedocs.io/en/stable/) and [lightning CLI](https://pytorch-lightning.readthedocs.io/en/stable/cli/lightning_cli.html). Especially, experiment manager feature, auto implement multi-node, multi-device, multi-accelerator support, etc.
 - Powerful [deep update](docs/configs/deep_update.md) feature for config file inherit to manage your config files in a more hierarchical way, see also [recommand config file structure](docs/configs/config_file_structure.md).
 - Multi and complex optimizers and lr_scheduler from CLI config support, see [doc](docs/core/optimizer_config.md).
 - Powerful and flexible LightningModule and LightningDataModule base class.
```

### Comparing `lightning-template-1.0.0/lightning_template.egg-info/SOURCES.txt` & `lightning-template-1.0.1/lightning_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-template-1.0.0/setup.py` & `lightning-template-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lightning-template",
-    version="1.0.0",
+    version="1.0.1",
     description="A template wrapper for pytorch-lightning.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="shenmishajing",
     author_email="shenmishajing@gmail.com",
     url="https://github.com/shenmishajing/lightning_template",
     project_urls={
```

