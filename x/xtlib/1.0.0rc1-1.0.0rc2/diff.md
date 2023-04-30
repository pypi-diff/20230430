# Comparing `tmp/xtlib-1.0.0rc1.tar.gz` & `tmp/xtlib-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xtlib-1.0.0rc1.tar", last modified: Fri May 29 23:22:25 2020, max compression
+gzip compressed data, was "dist/xtlib-1.0.0rc2.tar", last modified: Wed Jun 10 00:16:44 2020, max compression
```

## Comparing `xtlib-1.0.0rc1.tar` & `xtlib-1.0.0rc2.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/xtlib/
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/xtlib/psm/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    12415 2020-05-27 21:50:00.000000 xtlib-1.0.0rc1/xtlib/psm/remote_psm_client.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     6865 2020-05-27 21:50:00.000000 xtlib-1.0.0rc1/xtlib/psm/psm.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     7426 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/psm/local_psm_client.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     6278 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/tensorboard_reader.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     6204 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/capture.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)    10748 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/box_information.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    28113 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/impl_utilities.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/xtlib/hparams/
--rw-r--r--   0 xavier    (1000) xavier    (1000)      170 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/hparams/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     3567 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/hparams/hp_helper.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     8993 2020-05-21 21:07:51.000000 xtlib-1.0.0rc1/xtlib/hparams/hparam_search.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2173 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/hparams/hp_search_interface.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4307 2020-05-21 21:07:51.000000 xtlib-1.0.0rc1/xtlib/hparams/hp_search_bayesian.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     8203 2020-05-21 21:07:51.000000 xtlib-1.0.0rc1/xtlib/hparams/hp_client.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    32572 2020-05-21 17:33:34.000000 xtlib-1.0.0rc1/xtlib/hparams/hyperex.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    16859 2020-05-21 21:07:51.000000 xtlib-1.0.0rc1/xtlib/hparams/hp_search_dgd.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1530 2020-04-22 19:07:42.000000 xtlib-1.0.0rc1/xtlib/hparams/hp_search_random.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)    11019 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/hparams/hp_process.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      295 2020-04-15 20:09:22.000000 xtlib-1.0.0rc1/xtlib/__init__.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    13988 2020-05-28 17:02:49.000000 xtlib-1.0.0rc1/xtlib/client.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    11871 2020-04-28 19:53:31.000000 xtlib-1.0.0rc1/xtlib/run_info.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     5623 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/xt_server.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    46196 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/runner.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     9668 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/attach.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     7280 2020-05-21 17:33:34.000000 xtlib-1.0.0rc1/xtlib/xt_vault.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/xtlib/storage/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    49194 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/storage/store.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     9806 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/storage/store_azure_blob21.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1674 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/storage/fixup_mongo_jobs.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     6605 2020-05-27 21:50:00.000000 xtlib-1.0.0rc1/xtlib/storage/mongo_run_index.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     8623 2020-05-26 21:42:09.000000 xtlib-1.0.0rc1/xtlib/storage/store_file.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    48199 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/storage/store_objects.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2239 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/storage/fixup_mongo_runs.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2763 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/storage/store_interface.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    26554 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/storage/mongo_db.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      362 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/box_helper.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    25790 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/run_helper.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     3624 2020-04-28 19:53:31.000000 xtlib-1.0.0rc1/xtlib/errors.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1253 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/xt_dict.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    20187 2020-05-21 17:33:34.000000 xtlib-1.0.0rc1/xtlib/run.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4961 2020-05-26 21:42:09.000000 xtlib-1.0.0rc1/xtlib/console.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    59304 2020-05-27 21:50:00.000000 xtlib-1.0.0rc1/xtlib/controller.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     3693 2020-05-19 00:07:35.000000 xtlib-1.0.0rc1/xtlib/impl_shared.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    22482 2020-05-21 21:07:51.000000 xtlib-1.0.0rc1/xtlib/impl_help.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4178 2020-05-29 23:21:45.000000 xtlib-1.0.0rc1/xtlib/constants.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1330 2020-04-21 16:48:40.000000 xtlib-1.0.0rc1/xtlib/box_secrets.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    11971 2020-05-26 21:42:09.000000 xtlib-1.0.0rc1/xtlib/file_utils.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     6123 2020-05-28 17:02:49.000000 xtlib-1.0.0rc1/xtlib/mirror_worker.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     3055 2020-05-21 17:33:34.000000 xtlib-1.0.0rc1/xtlib/cache_server.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    29691 2020-05-20 22:29:59.000000 xtlib-1.0.0rc1/xtlib/report_builder.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/xtlib/demo_files/
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/xtlib/demo_files/code/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    29680 2020-05-21 21:07:50.000000 xtlib-1.0.0rc1/xtlib/demo_files/code/miniMnist.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)       81 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/demo_files/code/empty.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2297 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/demo_files/commands_basic.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     8277 2020-05-28 22:50:04.000000 xtlib-1.0.0rc1/xtlib/demo_files/commands_advanced.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     9224 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/demo_files/xt_demo.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    47967 2020-05-21 21:07:51.000000 xtlib-1.0.0rc1/xtlib/qfe.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/xtlib/helpers/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     3645 2020-05-26 21:42:09.000000 xtlib-1.0.0rc1/xtlib/helpers/yaml_dump.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     9662 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/helpers/validator.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2020-05-29 22:34:41.000000 xtlib-1.0.0rc1/xtlib/helpers/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1186 2020-04-15 20:09:22.000000 xtlib-1.0.0rc1/xtlib/helpers/stream_capture.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      609 2020-04-15 20:09:22.000000 xtlib-1.0.0rc1/xtlib/helpers/dot_dict.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1258 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/helpers/hexdump.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      723 2020-04-15 20:09:22.000000 xtlib-1.0.0rc1/xtlib/helpers/part_scanner.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1352 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/helpers/feedbackParts.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    23183 2020-05-29 22:45:48.000000 xtlib-1.0.0rc1/xtlib/helpers/xt_config.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     5204 2020-04-15 20:09:22.000000 xtlib-1.0.0rc1/xtlib/helpers/scanner.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2217 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/helpers/feedbackProgress.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1796 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/helpers/notebook_builder.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     4170 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/helpers/file_helper.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2838 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/helpers/key_press_checker.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      423 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/helpers/dir_change.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      569 2020-04-15 20:09:22.000000 xtlib-1.0.0rc1/xtlib/helpers/bag.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4919 2020-04-28 19:53:31.000000 xtlib-1.0.0rc1/xtlib/pc_utils.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    14517 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/job_helper.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    14869 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/utils.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     4817 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/repair_runs.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      841 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/impl_base.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    92179 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/impl_storage.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    44846 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/impl_compute.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1963 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/metric_set.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)    10938 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/scriptor.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     9154 2020-05-06 18:30:18.000000 xtlib-1.0.0rc1/xtlib/process_utils.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    29711 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/cmd_core.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4668 2020-05-18 23:47:37.000000 xtlib-1.0.0rc1/xtlib/cache_client.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      821 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/mirror.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/xtlib/templates/
--rw-r--r--   0 xavier    (1000) xavier    (1000)      174 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/templates/__init__.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/xtlib/backends/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    10419 2020-04-28 19:53:31.000000 xtlib-1.0.0rc1/xtlib/backends/backend_interface.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      171 2020-04-20 18:20:00.000000 xtlib-1.0.0rc1/xtlib/backends/__init__.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      447 2020-05-27 21:50:00.000000 xtlib-1.0.0rc1/xtlib/backends/aml_shim.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    26763 2020-05-27 21:50:00.000000 xtlib-1.0.0rc1/xtlib/backends/backend_base.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    23814 2020-05-27 21:50:00.000000 xtlib-1.0.0rc1/xtlib/backends/backend_pool.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    44266 2020-05-28 17:15:33.000000 xtlib-1.0.0rc1/xtlib/backends/backend_aml.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    56221 2020-05-27 21:50:00.000000 xtlib-1.0.0rc1/xtlib/backends/backend_batch.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4888 2020-05-19 00:07:35.000000 xtlib-1.0.0rc1/xtlib/xt_run.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     5928 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/xt_cmds.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    25713 2020-05-28 22:19:43.000000 xtlib-1.0.0rc1/xtlib/plot_builder.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     5590 2020-05-28 17:02:49.000000 xtlib-1.0.0rc1/xtlib/xt_client.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2098 2020-04-15 20:09:22.000000 xtlib-1.0.0rc1/README.md
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     3832 2020-05-29 23:21:57.000000 xtlib-1.0.0rc1/setup.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2933 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/PKG-INFO
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       38 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/setup.cfg
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/xtlib.egg-info/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2566 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/xtlib.egg-info/SOURCES.txt
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       42 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/xtlib.egg-info/entry_points.txt
--rw-rw-r--   0 xavier    (1000) xavier    (1000)        1 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/xtlib.egg-info/dependency_links.txt
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      404 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/xtlib.egg-info/requires.txt
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      127 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/xtlib.egg-info/top_level.txt
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2933 2020-05-29 23:22:25.000000 xtlib-1.0.0rc1/xtlib.egg-info/PKG-INFO
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-06-10 00:16:44.000000 xtlib-1.0.0rc2/
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-06-10 00:16:44.000000 xtlib-1.0.0rc2/xtlib/
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-06-10 00:16:44.000000 xtlib-1.0.0rc2/xtlib/psm/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)    12744 2020-06-09 19:45:09.000000 xtlib-1.0.0rc2/xtlib/psm/remote_psm_client.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     6935 2020-06-10 00:01:55.000000 xtlib-1.0.0rc2/xtlib/psm/psm.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     7403 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/psm/local_psm_client.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     6278 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/tensorboard_reader.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     6315 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/capture.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)    10748 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/box_information.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    30884 2020-06-10 00:01:55.000000 xtlib-1.0.0rc2/xtlib/impl_utilities.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-06-10 00:16:44.000000 xtlib-1.0.0rc2/xtlib/hparams/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      170 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/hparams/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     3567 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/hparams/hp_helper.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     8993 2020-05-21 21:07:51.000000 xtlib-1.0.0rc2/xtlib/hparams/hparam_search.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2173 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/hparams/hp_search_interface.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4307 2020-05-21 21:07:51.000000 xtlib-1.0.0rc2/xtlib/hparams/hp_search_bayesian.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     8203 2020-05-21 21:07:51.000000 xtlib-1.0.0rc2/xtlib/hparams/hp_client.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    32572 2020-05-21 17:33:34.000000 xtlib-1.0.0rc2/xtlib/hparams/hyperex.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    16859 2020-05-21 21:07:51.000000 xtlib-1.0.0rc2/xtlib/hparams/hp_search_dgd.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1530 2020-04-22 19:07:42.000000 xtlib-1.0.0rc2/xtlib/hparams/hp_search_random.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)    11019 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/hparams/hp_process.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      295 2020-04-15 20:09:22.000000 xtlib-1.0.0rc2/xtlib/__init__.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    13988 2020-06-08 20:45:05.000000 xtlib-1.0.0rc2/xtlib/client.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    11871 2020-04-28 19:53:31.000000 xtlib-1.0.0rc2/xtlib/run_info.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     5623 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/xt_server.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)    45986 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/runner.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     9668 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/attach.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     7280 2020-05-21 17:33:34.000000 xtlib-1.0.0rc2/xtlib/xt_vault.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-06-10 00:16:44.000000 xtlib-1.0.0rc2/xtlib/storage/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)    49447 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/storage/store.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     9903 2020-06-09 19:45:09.000000 xtlib-1.0.0rc2/xtlib/storage/store_azure_blob21.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1708 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/storage/fixup_mongo_jobs.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     6605 2020-05-27 21:50:00.000000 xtlib-1.0.0rc2/xtlib/storage/mongo_run_index.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     8623 2020-05-26 21:42:09.000000 xtlib-1.0.0rc2/xtlib/storage/store_file.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)    48754 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/storage/store_objects.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2239 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/storage/fixup_mongo_runs.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2763 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/storage/store_interface.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)    27917 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/storage/mongo_db.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      362 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/box_helper.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)    26105 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/run_helper.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     3624 2020-04-28 19:53:31.000000 xtlib-1.0.0rc2/xtlib/errors.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1253 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/xt_dict.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    20187 2020-05-21 17:33:34.000000 xtlib-1.0.0rc2/xtlib/run.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4961 2020-05-26 21:42:09.000000 xtlib-1.0.0rc2/xtlib/console.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    59304 2020-05-27 21:50:00.000000 xtlib-1.0.0rc2/xtlib/controller.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     3693 2020-05-19 00:07:35.000000 xtlib-1.0.0rc2/xtlib/impl_shared.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    22482 2020-05-21 21:07:51.000000 xtlib-1.0.0rc2/xtlib/impl_help.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4254 2020-06-10 00:16:19.000000 xtlib-1.0.0rc2/xtlib/constants.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1330 2020-04-21 16:48:40.000000 xtlib-1.0.0rc2/xtlib/box_secrets.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    11971 2020-05-26 21:42:09.000000 xtlib-1.0.0rc2/xtlib/file_utils.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     6123 2020-05-28 17:02:49.000000 xtlib-1.0.0rc2/xtlib/mirror_worker.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     3055 2020-05-21 17:33:34.000000 xtlib-1.0.0rc2/xtlib/cache_server.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    29691 2020-05-20 22:29:59.000000 xtlib-1.0.0rc2/xtlib/report_builder.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-06-10 00:16:44.000000 xtlib-1.0.0rc2/xtlib/demo_files/
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-06-10 00:16:44.000000 xtlib-1.0.0rc2/xtlib/demo_files/code/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    29680 2020-05-21 21:07:50.000000 xtlib-1.0.0rc2/xtlib/demo_files/code/miniMnist.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)       81 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/demo_files/code/empty.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     3690 2020-06-10 00:01:55.000000 xtlib-1.0.0rc2/xtlib/demo_files/commands_basic.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     8519 2020-06-09 21:01:18.000000 xtlib-1.0.0rc2/xtlib/demo_files/commands_advanced.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     9860 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/demo_files/xt_demo.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    47967 2020-05-21 21:07:51.000000 xtlib-1.0.0rc2/xtlib/qfe.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-06-10 00:16:44.000000 xtlib-1.0.0rc2/xtlib/helpers/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     3721 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/helpers/yaml_dump.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     9662 2020-06-04 22:04:08.000000 xtlib-1.0.0rc2/xtlib/helpers/validator.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2020-06-09 19:45:09.000000 xtlib-1.0.0rc2/xtlib/helpers/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1186 2020-04-15 20:09:22.000000 xtlib-1.0.0rc2/xtlib/helpers/stream_capture.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      609 2020-04-15 20:09:22.000000 xtlib-1.0.0rc2/xtlib/helpers/dot_dict.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1258 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/helpers/hexdump.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      723 2020-04-15 20:09:22.000000 xtlib-1.0.0rc2/xtlib/helpers/part_scanner.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1352 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/helpers/feedbackParts.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)    23321 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/helpers/xt_config.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     5204 2020-04-15 20:09:22.000000 xtlib-1.0.0rc2/xtlib/helpers/scanner.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2217 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/helpers/feedbackProgress.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1796 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/helpers/notebook_builder.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     4170 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/helpers/file_helper.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2712 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/helpers/key_press_checker.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      423 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/helpers/dir_change.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      569 2020-04-15 20:09:22.000000 xtlib-1.0.0rc2/xtlib/helpers/bag.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4919 2020-04-28 19:53:31.000000 xtlib-1.0.0rc2/xtlib/pc_utils.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)    15053 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/job_helper.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    15011 2020-06-10 00:01:55.000000 xtlib-1.0.0rc2/xtlib/utils.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     4817 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/repair_runs.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      841 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/impl_base.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    86177 2020-06-10 00:01:55.000000 xtlib-1.0.0rc2/xtlib/impl_storage.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)    44413 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/impl_compute.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1963 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/metric_set.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    10954 2020-06-10 00:01:55.000000 xtlib-1.0.0rc2/xtlib/scriptor.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     9154 2020-05-06 18:30:18.000000 xtlib-1.0.0rc2/xtlib/process_utils.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)    29715 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/cmd_core.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4668 2020-05-18 23:47:37.000000 xtlib-1.0.0rc2/xtlib/cache_client.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      821 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/mirror.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-06-10 00:16:44.000000 xtlib-1.0.0rc2/xtlib/templates/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      174 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/templates/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)    21331 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/impl_storage_api.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-06-10 00:16:44.000000 xtlib-1.0.0rc2/xtlib/backends/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    10419 2020-04-28 19:53:31.000000 xtlib-1.0.0rc2/xtlib/backends/backend_interface.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      171 2020-04-20 18:20:00.000000 xtlib-1.0.0rc2/xtlib/backends/__init__.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      447 2020-05-27 21:50:00.000000 xtlib-1.0.0rc2/xtlib/backends/aml_shim.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    26793 2020-06-10 00:01:55.000000 xtlib-1.0.0rc2/xtlib/backends/backend_base.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)    24243 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/backends/backend_pool.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    44266 2020-05-28 17:15:33.000000 xtlib-1.0.0rc2/xtlib/backends/backend_aml.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    56221 2020-05-27 21:50:00.000000 xtlib-1.0.0rc2/xtlib/backends/backend_batch.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4888 2020-05-19 00:07:35.000000 xtlib-1.0.0rc2/xtlib/xt_run.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     5939 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/xt_cmds.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)    25921 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/xtlib/plot_builder.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     5590 2020-05-28 17:02:49.000000 xtlib-1.0.0rc2/xtlib/xt_client.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2172 2020-06-09 20:58:19.000000 xtlib-1.0.0rc2/README.md
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     3832 2020-06-10 00:16:19.000000 xtlib-1.0.0rc2/setup.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2967 2020-06-10 00:16:44.000000 xtlib-1.0.0rc2/PKG-INFO
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       38 2020-06-10 00:16:44.000000 xtlib-1.0.0rc2/setup.cfg
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2020-06-10 00:16:44.000000 xtlib-1.0.0rc2/xtlib.egg-info/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2592 2020-06-10 00:16:43.000000 xtlib-1.0.0rc2/xtlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       42 2020-06-10 00:16:43.000000 xtlib-1.0.0rc2/xtlib.egg-info/entry_points.txt
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)        1 2020-06-10 00:16:43.000000 xtlib-1.0.0rc2/xtlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      404 2020-06-10 00:16:43.000000 xtlib-1.0.0rc2/xtlib.egg-info/requires.txt
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      127 2020-06-10 00:16:43.000000 xtlib-1.0.0rc2/xtlib.egg-info/top_level.txt
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2967 2020-06-10 00:16:43.000000 xtlib-1.0.0rc2/xtlib.egg-info/PKG-INFO
```

### Comparing `xtlib-1.0.0rc1/xtlib/psm/remote_psm_client.py` & `xtlib-1.0.0rc2/xtlib/psm/remote_psm_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,24 @@
         self.home = self.run_cmd("echo $HOME").strip()
         self.psm_queue_path = self.expand_remote_path(constants.PSM_QUEUE)
         self.xt_path = self.expand_remote_path(constants.XT_HOME)
         self.cwd_path = self.expand_remote_path(constants.CWD)
         self.psm_logdir = self.expand_remote_path(constants.PSM_LOGDIR)
         self.controller_cwd = self.expand_remote_path(utils.get_controller_cwd(self.box_is_windows, is_local=False))
 
+    def remote_file_exists(self, fn):
+        exists = False
+        try:
+            result = self.ftp_client.stat(fn)
+            exists = True
+        except IOError:
+            exists = False
+
+        return exists
+
     def expand_remote_path(self, fn):
         fn_expand = fn.replace("~/", self.home + "/")
         return fn_expand
 
     def start_ssh_session(self):
         self.ssh_client = paramiko.SSHClient()
         self.ssh_client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
@@ -187,24 +197,26 @@
 
         running = bool(self._get_psm_process_id())
         #print("PSM running=", running)
 
         if running:
             # do file contents match?
             text_src = file_utils.read_text_file(fn_src)
+            text_dest = ""
 
-            # read text of fn_dest on remote box
-            with self.ftp_client.open(fn_dest, "rb") as infile:
-                bytes_dest = infile.read()
-                text_dest = bytes_dest.decode()
-
-            # normalize NEWLINE chars before comparison 
-            # (ftp_client seems to add CR when called frm windows)
-            text_src = text_src.replace("\r\n", "\n")
-            text_dest = text_dest.replace("\r\n", "\n")
+            if self.remote_file_exists(fn_dest):
+                # read text of fn_dest on remote box
+                with self.ftp_client.open(fn_dest, "rb") as infile:
+                    bytes_dest = infile.read()
+                    text_dest = bytes_dest.decode()
+
+                # normalize NEWLINE chars before comparison 
+                # (ftp_client seems to add CR when called frm windows)
+                text_src = text_src.replace("\r\n", "\n")
+                text_dest = text_dest.replace("\r\n", "\n")
 
             if text_src != text_dest:
                 kill_needed = True
         else:
             start_needed = True
 
         if kill_needed:
```

### Comparing `xtlib-1.0.0rc1/xtlib/psm/psm.py` & `xtlib-1.0.0rc2/xtlib/psm/psm.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,20 @@
 import subprocess
 
 is_windows = (os.name == "nt")
 #log_print("is_windows:", is_windows)
 
 PSM_QUEUE = os.path.expanduser("~/.xt/psm_queue")
 PSM_LOGDIR = os.path.expanduser("~/.xt/psm_logs")
-CWD = "c:/xt_controller/xt/cwd" if is_windows else  os.path.expanduser("~/.xt/cwd")
+
+if is_windows:
+    sys_drive = os.getenv("SystemDrive")
+    CWD = os.path.join(sys_drive + "/xt", "cwd")
+else:
+    CWD = os.path.expanduser("~/.xt/cwd")
 
 PSM = "psm.py"
 CURRENT_RUNNING_ENTRY = "_current_running_entry_.txt"
 FN_WRAPPER = os.path.join(CWD, "wrapped.bat" if is_windows else "wrapped.sh")
 CONTROLLER_NAME_PATTERN = "xtlib.controller"
 PY_RUN_CONTROLLER ="__run_controller__.py"
```

### Comparing `xtlib-1.0.0rc1/xtlib/psm/local_psm_client.py` & `xtlib-1.0.0rc2/xtlib/psm/local_psm_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
         running = self._is_psm_running()
         #print("PSM running=", running)
 
         if running:
             # do file contents match?
             text_src = file_utils.read_text_file(fn_src)
-            text_dest = file_utils.read_text_file(fn_dest)
+            text_dest = file_utils.read_text_file(fn_dest) if os.path.exists(fn_dest) else None
             if text_src != text_dest:
                 kill_needed = True
         else:
             start_needed = True
 
         if kill_needed:
             p = self._get_psm_process()
@@ -157,19 +157,17 @@
             # run psm
             fn_log = os.path.join(self.cwd_path, constants.PSMLOG)
 
             if self.box_is_windows:
                 cmd_parts = ["cmd", "/c", "python -u {} > {}".format(fn_dest, fn_log)]
             else:
                 cmd_parts = ["bash", "-c", "python -u {} > {}".format(fn_dest, fn_log)]
-            
-            # put log in known dir
-            fn_run_log = os.path.expanduser("~/.xt/cwd/runpsm.log")
-            
-            process_utils.start_async_run_detached(cmd_parts, self.cwd_path, fn_run_log)
+
+            fn_psm_log = os.path.expanduser("~/.xt/cwd/runpsm.log")
+            process_utils.start_async_run_detached(cmd_parts, self.cwd_path, fn_psm_log)
 
     def get_running_entry_name(self):
         text = None
 
         controller_cwd = utils.get_controller_cwd(self.box_is_windows, is_local=True)
 
         fn_current = os.path.join(controller_cwd, constants.CURRENT_RUNNING_ENTRY)
```

### Comparing `xtlib-1.0.0rc1/xtlib/tensorboard_reader.py` & `xtlib-1.0.0rc2/xtlib/tensorboard_reader.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/capture.py` & `xtlib-1.0.0rc2/xtlib/capture.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,40 +75,46 @@
                 copied_files += store.upload_files_to_run(ws_name, run_name, store_dest, input_wildcard, exclude_dirs_and_files=omit_files)
                 dest_name = "run"
                 elapsed = time.time() - started
                 store.log_run_event(ws_name, run_name, "capture_before", {"elapsed": elapsed, "count": len(copied_files)})
 
     return copied_files
 
-def download_before_files(store, job_id, ws_name, run_name, dest_dir, silent=False):
+def download_before_files(store, job_id, ws_name, run_name, dest_dir, silent=False, log_events=True):
     files = []
 
     if job_id:
         # all files contained in JOB BEFORE
         files += store.download_files_from_job(job_id, "before/code/**", dest_dir)
         count = len(files)
         if not silent:
             console.print("  {} CODE files downloaded from store (JOB dir)".format(count))
-        store.log_run_event(ws_name, run_name, "download_before", {"source": "job", "count": count})
+
+        if log_events:
+            store.log_run_event(ws_name, run_name, "download_before", {"source": "job", "count": count})
     else:
         if "." in run_name:
             # download from parent's RUN before files
             parent_name = run_name.split(".")[0]
             files += store.download_files_from_run(ws_name, parent_name, "before/**", dest_dir)
             count = len(files)
             if not silent:
                 console.print("  {} files downloaded from store (PARENT'S RUN dir)".format(count))
-            store.log_run_event(ws_name, run_name, "download_before", {"source": "parent-run", "count": count})
+
+            if log_events:
+                store.log_run_event(ws_name, run_name, "download_before", {"source": "parent-run", "count": count})
         
         # download from normal/child RUN before files
         files += store.download_files_from_run(ws_name, run_name, "before/**", dest_dir)
         count = len(files)
         if not silent:
             console.print("  {} files downloaded from store (RUN dir)".format(count))
-        store.log_run_event(ws_name, run_name, "download_before", {"source": "run", "count": count})
+
+        if log_events:
+            store.log_run_event(ws_name, run_name, "download_before", {"source": "run", "count": count})
 
     unzip_before_if_found(dest_dir, silent=silent)
 
     return files
 
 def unzip_before_if_found(dest_dir, remove_after=True, silent=False):
     fn_zip = dest_dir + "/" + constants.CODE_ZIP_FN
```

### Comparing `xtlib-1.0.0rc1/xtlib/box_information.py` & `xtlib-1.0.0rc2/xtlib/box_information.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/impl_utilities.py` & `xtlib-1.0.0rc2/xtlib/impl_utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,24 +6,28 @@
 import os
 import re
 import sys
 import copy
 import time
 import shutil
 import logging
+import yaml
 
 from xtlib import qfe
 from xtlib.console import console
 from xtlib.cmd_core import CmdCore
 from xtlib.helpers import xt_config
 from xtlib.impl_base import ImplBase
 from xtlib.helpers import file_helper
 from xtlib.helpers.hexdump import hex_dump
+from xtlib.helpers import yaml_dump
 from xtlib.qfe import inner_dispatch, see_also
+from xtlib.impl_storage_api import ImplStorageApi
 from xtlib.helpers.xt_config import get_default_config_path
+from xtlib.helpers.xt_config import get_default_config_template_path
 from xtlib.qfe import command, argument, option, flag, root, example, command_help
 
 from xtlib import utils
 from xtlib import errors
 from xtlib import pc_utils
 from xtlib import constants
 from xtlib import run_helper
@@ -190,14 +194,15 @@
     @example(task="get a directory listing of files on box 'vm23''", text="xt ssh vm10 ls -l")
     @command(options_before_args=True, help="executes the specified command, on begins a console session, with the specified box")
     def ssh(self, name, cmd, workspace, output):
         capture_output = True if cmd else False
 
         if name.startswith("run"):
             # assume it's a RUN name
+            # from xtlib.backends.backend_philly import Philly
             # rr = run_helper.get_run_record(self.store, workspace, name)
             # if not "cluster" in rr:
             #     errors.store_error("only philly runs are currently supported for this cmd")
 
             # philly = Philly(core=self.core)
             # ssh_cmd = philly.get_ssh_for_run(workspace, name)
             # print("ssh_cmd: " + ssh_cmd)
@@ -221,15 +226,15 @@
                 outfile.write(ssh_output)
         elif capture_output:
             console.print(ssh_output)
 
     #---- SCP command ----
     @argument(name="cmd", help="the scp command to execute", type="text")
     @example(task="copy the local file 'miniMnist.py' to the outer directory of box 'vm10'", text="xt scp miniMnist.py vm10:~/")
-    @example(task="copy the all *.py files from the outer directory of box 'vm10' to the local directory c:\\zip", text="xt scp vm10:~/*.py /zip")
+    @example(task="copy the all *.py files from the outer directory of box 'vm10' to the local directory /zip", text="xt scp vm10:~/*.py /zip")
     @command(help="copy file(s) between the local machine and a remote box")
     def scp(self, cmd):
         # fixup the boxname:xxx patterns
         parts = cmd.split(" ")
         for i, part in enumerate(parts):
             if ":" in part:
                 # remove surrounding quotes
@@ -347,14 +352,42 @@
 
             config_lines.append(section + ":")
             config_lines += prop_lines
 
         text = "\n".join(config_lines)
         return text
 
+    def copy_and_merge_sections(self, default_sections, sections, update_keys=None):
+        if update_keys is None:
+            update_keys = dict()
+        new_config = dict()
+        for section in sections:
+            section_components = section.split(".")
+            current = new_config
+            current_default = default_sections
+            for section_component in section_components:
+                if section_component not in current and section_component != section_components[-1]:
+                    current[section_component] = dict()
+                elif section_component not in current and section_component == section_components[-1]:
+                    current[section_component] = current_default[section_component]
+                current = current[section_component]
+                current_default = current_default[section_component]
+
+        for section in update_keys.keys():
+            section_components = section.split(".")
+            current = new_config
+            for section_component in section_components:
+                if section_component == section_components[-1]:
+                    current[section_component] = update_keys[section]
+                current = current[section_component]
+
+        result = yaml_dump.pretty_yaml_dump(new_config, read_only_text=False)
+
+        return result
+
     def build_sections(self, lines):
         sections = {}
         props = None
 
         for line in lines:
             if re.match('^[a-zA-Z]+', line) is not None:
                 # line starts with a letter
@@ -364,20 +397,20 @@
             elif props is not None:
                 props.append(line)
 
         return sections
 
     def get_config_template(self, template):
         # load default config file as lines
-        fn = get_default_config_path()
+        fn = get_default_config_template_path()
         default_text = file_utils.read_text_file(fn)
         default_lines = default_text.split("\n")
 
         # convert lines to sections dict
-        sections = self.build_sections(default_lines)
+        sections = yaml.safe_load(default_text)
 
         if not template or template == "empty":
 
             # EMPTY
             hdr = \
                 "# local xt_config.yaml\n" + \
                 "# uncomment the below lines to start populating your config file\n\n" 
@@ -387,41 +420,52 @@
                 "    #workspace: 'ws1'\n" + \
                 "    #experiment: 'exper1'\n"
 
         elif template == "philly":
 
             # PHILLY
             hdr = "# local xt_config.yaml for Philly compute service\n\n"
-            text = self.copy_sections(sections, ["compute-targets.philly", "environments.philly-pytorch", 
-                "general", "code", "after-files", "data", "model", "logging", "hyperparameter-search",
-                "run-reports.columns", "job-reports.columns", "tensorboard"])
+            text = self.copy_and_merge_sections(sections, ["external-services.philly",
+                "external-services.philly-registry", "external-services.phoenixkeyvault", 
+                "external-services.phoenixmongodb", "external-services.phoenixregistry",
+                "external-services.phoenixstorage", "xt-services",
+                "compute-targets.philly", "setups.philly", "dockers.philly-pytorch", 
+                "general"], update_keys={"xt-services.target": "philly"})
 
         elif template == "batch":
 
             # BATCH
             hdr = "# local xt_config.yaml (for Azure Batch compute services)\n\n"
-            text = self.copy_sections(sections, ["external-services.xtsandboxbatch", "compute-targets.batch", "environments.philly-pytorch", 
-                "general", "code", "after-files", "data", "model", "logging", "hyperparameter-search",
-                "run-reports.columns", "job-reports.columns", "tensorboard", "azure-batch-images"])
+            text = self.copy_and_merge_sections(sections, ["external-services.phoenixbatch",
+                "external-services.phoenixkeyvault", 
+                "external-services.phoenixmongodb", "external-services.phoenixregistry",
+                "external-services.phoenixstorage",
+                "xt-services", "compute-targets.batch", "azure-batch-images",
+                "general"], update_keys={"xt-services.target": "batch"})
 
         elif template == "aml":
 
             # AML 
             hdr = "# local xt_config.yaml (for Azure ML compute service)\n\n"
-            text = self.copy_sections(sections, ["external-services.canadav100ws", "compute-targets.canada", "environments.philly-pytorch", 
-                "general", "code", "after-files", "data", "model", "logging", "aml-options", "early-stopping", "hyperparameter-search",
-                "run-reports.columns", "job-reports.columns", "tensorboard"])
+            text = self.copy_and_merge_sections(sections, ["external-services.phoenixaml", 
+                "external-services.phoenixkeyvault", 
+                "external-services.phoenixmongodb", "external-services.phoenixregistry",
+                "external-services.phoenixstorage", "xt-services",
+                "compute-targets.aml", "aml-options",
+                "general"], update_keys={"xt-services.target": "aml"})
 
         elif template == "pool":
 
             # POOL
             hdr = "# local xt_config.yaml (for local machine and Pool compute service)\n\n"
-            text = self.copy_sections(sections, ["compute-targets.local", "environments.pytorch-xtlib", 
-                "general", "code", "after-files", "data", "model", "logging", "hyperparameter-search",
-                "run-reports.columns", "job-reports.columns", "tensorboard", "boxes"])
+            text = self.copy_and_merge_sections(sections, ["external-services.phoenixkeyvault", 
+                "external-services.phoenixmongodb", "external-services.phoenixregistry",
+                "external-services.phoenixstorage",
+                "xt-services", "compute-targets.local", "compute-targets.local-docker", "boxes", "setups.local",
+                "dockers.pytorch-xtlib", "dockers.pytorch-xtlib-local", "general"])
 
         elif template == "all":
 
             # ALL
             hdr = "# local xt_config.yaml (for all compute services)\n\n"
             text = "\n".join(default_lines)
 
@@ -497,17 +541,18 @@
                 console.print("invoking your default .yaml editor on: {}".format(fn))
                 from xtlib import process_utils 
                 process_utils.open_file_with_default_app(fn)
 
     #---- CREATE DEMO command ----
     @argument(name="destination", help="the path in which the demo files should be created")
     @option("response", default=None, help="the response to be used to confirm the directory deletion")
-    @example(task="create a set of demo files in c:\\xtdemo", text="xt create demo c:/xtdemo")
+    @example(task="create a set of demo files in the subdirectory xtdemo", text="xt create demo ./xtdemo")
+    @flag("overwrite", help="When specified, any existing xtd-prefixed job names that match xt-demo job names will be overwritten")
     @command(help="creates a set of demo files that can be used to quickly try out various XT features")
-    def create_demo(self, destination, response):
+    def create_demo(self, destination, response, overwrite):
         '''
         This command will removed the specified destination directory if it exists (prompting the user for approval).
         Specifying the current directory as the destination will produce an error.
         '''
 
         # set up from_dir
         from_dir = file_utils.get_xtlib_dir() + "/demo_files"
@@ -527,14 +572,22 @@
 
         if create:
             file_utils.ensure_dir_deleted(dest_dir)
 
             shutil.copytree(from_dir, dest_dir)
             #file_utils.copy_tree(from_dir, dest_dir)
 
+            if not self.store.does_workspace_exist("xt-demo"):
+                # import xt-demo workspace from archive file
+                console.print("importing xt-demo workspace (usually takes about 30 seconds)")
+                impl_storage_api = ImplStorageApi(self.config, self.store)
+
+                fn_archive = os.path.join(file_utils.get_xtlib_dir(), "demo_files", "xt-demo-archive.zip")
+                impl_storage_api.import_workspace(fn_archive, "xt-demo", "xtd", overwrite=overwrite, show_output=False)
+
     def is_aml_ws(self, ws_name):
         return self.azure_ml.does_ws_exist(ws_name)
         
     def get_registry_creds(self, compute, env):
         registry_creds = None
 
         if not env:
@@ -556,36 +609,36 @@
         return registry_creds
 
     #---- DOCKER LOGIN command ----
     @option("docker", help="the docker environment that defines the docker registry for login")
     @option("target", default="$xt-services.target", help="one of the user-defined compute targets on which to run")
     @example(task="log user into docker", text="xt docker login")
     @command(kwgroup="docker", kwhelp="runs the specified docker command", help="logs the user into docker using docker credentials from the XT config file")
-    def docker_login(self, target, environment):
-        reg_creds = self.get_registry_creds(target, environment)
+    def docker_login(self, target, docker):
+        reg_creds = self.get_registry_creds(target, docker)
         if not reg_creds:
-            if environment:
-                errors.env_error("no docker environment defined for environment '{}'".format(environment))
+            if docker:
+                errors.env_error("no dockers entry defined for docker '{}'".format(docker))
             else:
-                errors.env_error("no docker environment defined for target '{}'".format(target))
+                errors.env_error("no docker property defined for target '{}'".format(target))
 
         server = reg_creds["login-server"]
         username = reg_creds["username"]
         password = reg_creds["password"]
 
         text = self.core.docker_login(server, username, password)
         console.print(text)
 
     #---- DOCKER LOGOUT command ----
     @option("docker", help="the docker environment that defines the docker registry for login")
     @option("target", default="$xt-services.target", help="one of the user-defined compute targets on which to run")
     @example(task="log the user out of docker", text="xt docker logout")
     @command(kwgroup="docker", help="logs the user out of docker")
-    def docker_logout(self, target, environment):
-        reg_creds = self.get_registry_creds(target, environment)
+    def docker_logout(self, target, docker):
+        reg_creds = self.get_registry_creds(target, docker)
         server = reg_creds["login-server"]
 
         text = self.core.docker_logout(server)
         console.print(text)
 
     #---- REPL command ----
     @example(task="initiate an XT repl session", text="xt repl")
```

### Comparing `xtlib-1.0.0rc1/xtlib/hparams/hp_helper.py` & `xtlib-1.0.0rc2/xtlib/hparams/hp_helper.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/hparams/hparam_search.py` & `xtlib-1.0.0rc2/xtlib/hparams/hparam_search.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/hparams/hp_search_interface.py` & `xtlib-1.0.0rc2/xtlib/hparams/hp_search_interface.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/hparams/hp_search_bayesian.py` & `xtlib-1.0.0rc2/xtlib/hparams/hp_search_bayesian.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/hparams/hp_client.py` & `xtlib-1.0.0rc2/xtlib/hparams/hp_client.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/hparams/hyperex.py` & `xtlib-1.0.0rc2/xtlib/hparams/hyperex.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/hparams/hp_search_dgd.py` & `xtlib-1.0.0rc2/xtlib/hparams/hp_search_dgd.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/hparams/hp_search_random.py` & `xtlib-1.0.0rc2/xtlib/hparams/hp_search_random.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/hparams/hp_process.py` & `xtlib-1.0.0rc2/xtlib/hparams/hp_process.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/client.py` & `xtlib-1.0.0rc2/xtlib/client.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/run_info.py` & `xtlib-1.0.0rc2/xtlib/run_info.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/xt_server.py` & `xtlib-1.0.0rc2/xtlib/xt_server.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/runner.py` & `xtlib-1.0.0rc2/xtlib/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,21 +31,22 @@
 from xtlib import constants
 from xtlib import file_utils
 from xtlib import process_utils
 from xtlib import box_information
 
 class Runner():
     ''' class to consolidate all shared code for run submission '''
-    def __init__(self, config, core):
+    def __init__(self, config, core, temp_dir):
         self.config = config
         self.core = core
         self.store = core.store
         self.backend = None
         self.is_docker = None
         self.target_dir = None
+        self.temp_dir = temp_dir
 
     def process_args(self, args):
 
         run_script = None
         parent_script = None
         run_cmd_from_script = None
         target_file = args["script"]
@@ -589,22 +590,21 @@
         pip_packages = utils.safe_value(setup_def, "pip-packages")
 
         args["conda_packages"] = conda_packages if conda_packages else []
         args["pip_packages"] = pip_packages if pip_packages else []
 
         self.adjust_pip_packages(args)
 
+        snapshot_dir = self.temp_dir
+
         if fake_submit:
-            snapshot_dir = "fake_temp_dir"
             script_dir = snapshot_dir
         else:
             # note: always create a snapshot dir for backends to add needed files
-            snapshot_dir = file_utils.make_tmp_dir("code-snapshot", fixed_name=False) 
             file_utils.ensure_dir_deleted(snapshot_dir)
-
             script_dir = self.snapshot_all_code(snapshot_dir, cmd_parts, args)
 
         self.script_dir = script_dir
         direct_run = args["direct_run"]
 
         # do we need to start the xt controller?
         use_controller = not direct_run
@@ -828,18 +828,14 @@
 
         # update job info 
         if not fake_submit:
             dd["service_job_info"] = service_job_info
             dd["service_info_by_node"] = service_info_by_node
             self.store.log_job_info(job_id, dd)
 
-        # remove temp files
-        # this is causing a permission denied error currently (due to Azure holding it open?)
-        #os.remove(snapshot_dir)
-
         # update lastrun/lastjob info
         xtd = xt_dict.read_xt_dict()
         xtd["last_run"] = last_run
         xtd["last_job"] = job_id
         xt_dict.write_xt_dict(xtd)
 
         # return values for API support (X)
```

### Comparing `xtlib-1.0.0rc1/xtlib/attach.py` & `xtlib-1.0.0rc2/xtlib/attach.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/xt_vault.py` & `xtlib-1.0.0rc2/xtlib/xt_vault.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/storage/store.py` & `xtlib-1.0.0rc2/xtlib/storage/store.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,17 @@
         self.store_type = storage_creds["provider"]
 
         self.cap_stdout = None
         self.cap_stderr = None
 
         self.helper.validate_storage_and_mongo(self.mongo)
 
+    def get_name(self):
+        return self.helper.get_name()
+        
     def get_mongo(self):
         return self.mongo
 
     def get_props_dict(self):
         pd = {"storage_creds": self.storage_creds, "mongo_conn_str": self.mongo_conn_str, 
             "run_cache_dir": self.run_cache_dir, "provider_code_path": self.provider_code_path}
         return pd
@@ -173,21 +176,32 @@
 
         # log some information
         self.log_workspace_event(ws_name, "created", {"description": description})
 
     def delete_workspace(self, ws_name):
         ''' delete the specified workspace, and all of the runs stored within it.
         '''
+        job_names = self.mongo.get_job_names({"ws_name": ws_name})
+
         result = self.helper.delete_workspace(ws_name)
         if result:
-            # remove associated mongo info
+            console.print("  workspace/run storage deleted")
+
+            # remove mongo workspace
             self.mongo.remove_workspace(ws_name)
+            console.print("  workspace/run mongo deleted")
+
+            # remove each job on store/mongo
+            for job_id in job_names:
+                self.helper.delete_job(job_id)
+                self.mongo.delete_job(job_id)
+                console.print("  {} deleted".format(job_id))
 
         return result
-    
+
     def log_workspace_event(self, ws_name, event_name, data_dict):
         ''' log the specifed event_name and key/value pairs in the data_dict to the workspace log file.
         '''
         record_dict = {"time": utils.get_time(), "event": event_name, "data": data_dict}
         rd_text = json.dumps(record_dict)
 
         # append to workspace log file
@@ -394,23 +408,15 @@
     def get_running_run(self):
         return os.getenv("XT_RUN_NAME", None)
 
     def does_run_exist(self, ws_name, run_name):
         return self.helper.does_run_exist(ws_name, run_name)
 
     def get_job_id_of_run(self, ws_name, run_name):
-        job_id = None
-        records = self.get_run_log(ws_name, run_name)
-        if len(records) > 0:
-            first = records[0]
-            if "event" in first and first["event"] == "created":
-                dd = first["data"]
-                if "job_id" in dd:
-                    job_id = dd["job_id"]
-
+        job_id = self.mongo.get_run_property(ws_name, run_name, "job_id")
         return job_id
 
     def _create_next_run_directory(self, ws_name, is_parent):
 
         # is this a legacy workspace?
         default_next = self.helper.get_legacy_next_run_id(ws_name)
         if not default_next:
```

### Comparing `xtlib-1.0.0rc1/xtlib/storage/store_azure_blob21.py` & `xtlib-1.0.0rc2/xtlib/storage/store_azure_blob21.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT license.
 #
 # store-azure-blob21: Azure Blob Storage API (based on azure-storage-blob==2.1.0)
 import logging
 from interface import implements
 from azure.storage.blob import AppendBlobService, BlockBlobService, PublicAccess
+from azure.storage.blob.models import DeleteSnapshot
 
 from xtlib import utils
 from xtlib.storage.store_interface import StoreInterface
 
 logger = logging.getLogger(__name__)
 
 class AzureBlobStore21(implements(StoreInterface)):
@@ -186,15 +187,16 @@
         if return_names:
             blobs = [blob.name for blob in blobs]
         else:
             blobs = list(blobs)
         return blobs
 
     def delete_blob(self, container, blob_path, snapshot=None):
-        return self.bs.delete_blob(container, blob_path, snapshot=snapshot)
+        dss = DeleteSnapshot()
+        return self.bs.delete_blob(container, blob_path, delete_snapshots=dss.Include)
 
     def get_blob_text(self, container, blob_path):
         # watch out for 0-length blobs - they trigger an Azure RETRY error
         text = ""
         # azure storage bug workaround: avoid RETRY errors for 0-length blob 
         blob = self.bs.get_blob_properties(container, blob_path)
         if blob.properties.content_length:
```

### Comparing `xtlib-1.0.0rc1/xtlib/storage/fixup_mongo_jobs.py` & `xtlib-1.0.0rc2/xtlib/storage/fixup_mongo_jobs.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 # Licensed under the MIT license.
 #
 # fixup_mongo_jobs.py: add "job_num" to JOB collection records, as needed
 import pymongo
 import time
 
 from xtlib import console
+from xtlib import job_helper
 
 batch_size = 100
 
 def process_job_batch(collection, records):
     '''
     due to UPDATE RATE restrictions on MongoDB/Cosmos, we must process in 
     batches (not all at once)
     '''
     updates = []
 
     for record in records:
         job_id = record["_id"]
-        if not job_id or not job_id.startswith("job"):
+        if not job_id or not job_helper.is_job_id(job_id):
             continue
 
         job_num = int(job_id[3:])
 
         fd = {"_id": job_id}
         ud = {"$set": {"job_num": job_num}}
```

### Comparing `xtlib-1.0.0rc1/xtlib/storage/mongo_run_index.py` & `xtlib-1.0.0rc2/xtlib/storage/mongo_run_index.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/storage/store_file.py` & `xtlib-1.0.0rc2/xtlib/storage/store_file.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/storage/store_objects.py` & `xtlib-1.0.0rc2/xtlib/storage/store_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,18 @@
 
         # Basic configuration: configure the root logger, including 'azure.storage'
         #logging.basicConfig(format='%(asctime)s %(name)-20s %(levelname)-5s %(message)s', level=logging.INFO)
 
         self.max_retries = max_retries
         self.set_retries(max_retries)
 
+    def get_name(self):
+        storage_name = self.provider.get_service_name()
+        return storage_name
+        
     def validate_storage_and_mongo(self, mongo):
         '''
         1. ensure storage has been initialized for XT
         2. ensure mongo and storage point to each other
         3. update storage format if needed
         4. update mongo format if needed
         '''
@@ -648,14 +652,23 @@
         experiments_holder_fn = constants.EXPERIMENTS_DIR + "/" + constants.HOLDER_FILE
         self._create_blob(ws_name, experiments_holder_fn, "1", True)
 
         # create NEXT_RUN_NAME (for extra safety, ensure file doesn't already exist)
         blob_fn = constants.WORKSPACE_DIR + "/" + constants.WORKSPACE_NEXT
         self._create_blob(ws_name, blob_fn, "1", True)
 
+    def delete_job(self, job_id):
+        '''
+        for use with "delete workspace" command, this
+        only deletes the storage directory for the specified job 
+        (not any of its runs or releated experiments).
+        '''
+        blob_names = self.provider.list_blobs(constants.INFO_CONTAINER, "jobs/" + job_id)
+        for name in blob_names:
+            self.provider.delete_blob(constants.INFO_CONTAINER, name)
 
     def delete_workspace(self, ws_name):
         result = self.provider.delete_container(ws_name)    
 
         if not result:
              errors.store_error("could not delete workspace: " + ws_name)
```

### Comparing `xtlib-1.0.0rc1/xtlib/storage/fixup_mongo_runs.py` & `xtlib-1.0.0rc2/xtlib/storage/fixup_mongo_runs.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/storage/store_interface.py` & `xtlib-1.0.0rc2/xtlib/storage/store_interface.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/storage/mongo_db.py` & `xtlib-1.0.0rc2/xtlib/storage/mongo_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,22 +90,37 @@
 
         # remove legacy counters for this workspace
         end_id = ws_name + "-end_id"
         cmd = lambda: self.mongo_db.ws_counters.remove( {"_id": end_id} )
         self.mongo_with_retries("remove_workspace", cmd)
 
     def remove_cache(self, ws_name):
-        # remove appropriate node of run_cache_dir
-        cache_fn = os.path.expanduser(self.run_cache_dir) + "/" + constants.RUN_SUMMARY_CACHE_FN
-        cache_fn = cache_fn.replace("$ws", ws_name)
-        cache_dir = os.path.dirname(cache_fn)
-
-        if os.path.exists(cache_dir):
-            console.print("  zapping cache_dir=", cache_dir)
-            file_utils.zap_dir(cache_dir)
+        if self.run_cache_dir:
+            # remove appropriate node of run_cache_dir
+            cache_fn = os.path.expanduser(self.run_cache_dir) + "/" + constants.RUN_SUMMARY_CACHE_FN
+            cache_fn = cache_fn.replace("$ws", ws_name)
+            cache_dir = os.path.dirname(cache_fn)
+
+            if os.path.exists(cache_dir):
+                console.print("  zapping cache_dir=", cache_dir)
+                file_utils.zap_dir(cache_dir)
+
+    def init_workspace_counters(self, ws_name, next_run, next_end):
+        update_doc = { "_id": ws_name, "next_run": next_run, "next_end": next_end, "next_child" : {} }
+
+        cmd = lambda: self.mongo_db.ws_counters.find_and_modify( {"_id": ws_name}, update=update_doc, upsert=True)
+        self.mongo_with_retries("init_workspace_counters", cmd)
+
+    def delete_job(self, job_id):
+        '''
+        for use with "delete workspace" cmd, this only deletes
+        the specified job (not its runs or related experiments).
+        '''
+        cmd_func = lambda: self.mongo_db["__jobs__"].delete_one( {"_id": job_id} )
+        jobs = self.mongo_with_retries("delete_job", cmd_func)
 
     def get_next_sequential_job_id(self, default_next):
         job_ws = "__jobs__"
         path = "next_job"
 
         db = self.mongo_db
 
@@ -539,14 +554,28 @@
         if cursor and cursor.count():
             result = list(cursor)[0]
             if "ws_name" in result:
                 ws_name = result["ws_name"]
 
         return ws_name
 
+    def get_run_property(self, ws_name, run_name, prop_name):
+        cmd = lambda: self.mongo_db[ws_name].find( {"_id": run_name}, {prop_name: 1})
+        cursor = self.mongo_with_retries("get_run_property", cmd)
+
+        value = utils.safe_cursor_value(cursor, prop_name)
+        return value
+        
+    def get_job_property(self, job_id, prop_name):
+        cmd = lambda: self.mongo_db["__jobs__"].find( {"_id": job_id}, {prop_name: 1})
+        cursor = self.mongo_with_retries("get_job_property", cmd)
+
+        value = utils.safe_cursor_value(cursor, prop_name)
+        return value
+
     def job_node_start(self, job_id):
         '''
         A job's node has started running.  We need to:
             - increment the job's "running_nodes" property
             - set the "job_status" property to "running"
         '''
         cmd = lambda: self.mongo_db["__jobs__"].find_and_modify( {"_id": job_id}, update={"$inc": {"running_nodes": 1} })
```

### Comparing `xtlib-1.0.0rc1/xtlib/run_helper.py` & `xtlib-1.0.0rc2/xtlib/run_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     run_list = []
     actual_ws = workspace
 
     if name_list:
         for entry in name_list:
             if entry.startswith("run"):
                 actual_ws = expand_run_entry(store, mongo, workspace, run_list, entry)
-            elif entry.startswith("job"):
+            elif job_helper.is_job_id(entry):
                 actual_ws = expand_job_entry(store, mongo, workspace, run_list, entry)
             else:
                 actual_ws = expand_experiment_name(store, mongo, workspace, run_list, entry)
 
     return run_list, actual_ws
 
 def expand_run_entry(store, mongo, workspace, run_list, name):
@@ -300,14 +300,16 @@
     user_to_actual, std_cols_desc = get_run_property_dicts()        
     actual_to_user = {value: key for key, value in user_to_actual.items()}
 
     builder = ReportBuilder(config, store, client=None)
 
     # get list of specified runs
     pure_run_list, actual_ws = expand_run_list(store, mongo, workspace, run_list)
+    if run_list and not pure_run_list:
+        errors.general_error("no run(s) found")
 
     # build a filter dict for all specified filters
     filter_dict = build_run_filter_dict(pure_run_list, user_to_actual, builder, args)
 
     # if show_gathering:
     #     console.print("gathering run data...", flush=True)
 
@@ -705,8 +707,18 @@
     rundir = None    # unknown
     log = True
     capture = True
 
     store.wrapup_run(context.ws, run_name, context.aggregate_dest, context.dest_name, 
         status, exit_code, context.primary_metric, context.maximize_metric, context.report_rollup, 
         rundir, context.after_files_list, log, capture, job_id=context.job_id, node_id=node_id,
-        run_index=run_index)    
+        run_index=run_index)    
+
+def get_parent_run_number(name):
+    num = 0
+    if name and name.startswith("run"):
+        part = name[3:]
+        if "." in part:
+            part = part.split(".")[0]
+        num = int(part)
+
+    return num
```

### Comparing `xtlib-1.0.0rc1/xtlib/errors.py` & `xtlib-1.0.0rc2/xtlib/errors.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/xt_dict.py` & `xtlib-1.0.0rc2/xtlib/xt_dict.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/run.py` & `xtlib-1.0.0rc2/xtlib/run.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/console.py` & `xtlib-1.0.0rc2/xtlib/console.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/controller.py` & `xtlib-1.0.0rc2/xtlib/controller.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/impl_shared.py` & `xtlib-1.0.0rc2/xtlib/impl_shared.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/impl_help.py` & `xtlib-1.0.0rc2/xtlib/impl_help.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/constants.py` & `xtlib-1.0.0rc2/xtlib/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 #
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT license.
 #
 # constants.py: constant strings and values share among multiple modules
 # sync this version with setup.py, CHANGELOG.md
-BUILD = "version: 1.0.0rc1, build: May-28-2020"
+BUILD = "version: 1.0.0.rc2, build: Jun-09-2020"
 
 INFO_CONTAINER = "xt-store-info"
 INFO_DIR = "__info__"
 STORAGE_VERSION = "1"
 STORAGE_INFO_FILE = INFO_DIR + "/storage_info.json"
 
 # XT inserted metrics
 INDEX = "__index__"
 STEP_NAME = "__step_name__"
 TIME = "__time__"
 
 FN_CONFIG_FILE = "xt_config.yaml"
 FN_DEFAULT_CONFIG = "default_config.yaml"
+FN_DEFAULT_TEMPLATE = "default_template.yaml"
 FN_ORIG_DEFAULT = "orig_default_config.yaml"
 FN_INTERNAL_CONFIG = "internal_config.yaml"
 
+CONFIG_FN = "xt_config.yaml"
 AZURE_ERRORS_FN = "azure_errors.txt"
 
 # workspace directory and files
 WORKSPACE_DIR = "__ws__"
 RUNS_DIR = "runs"
 EXPERIMENTS_DIR = "experiments"
 HOLDER_FILE = "__make_dir__"
```

### Comparing `xtlib-1.0.0rc1/xtlib/box_secrets.py` & `xtlib-1.0.0rc2/xtlib/box_secrets.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/file_utils.py` & `xtlib-1.0.0rc2/xtlib/file_utils.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/mirror_worker.py` & `xtlib-1.0.0rc2/xtlib/mirror_worker.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/cache_server.py` & `xtlib-1.0.0rc2/xtlib/cache_server.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/report_builder.py` & `xtlib-1.0.0rc2/xtlib/report_builder.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/demo_files/code/miniMnist.py` & `xtlib-1.0.0rc2/xtlib/demo_files/code/miniMnist.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/demo_files/commands_advanced.py` & `xtlib-1.0.0rc2/xtlib/demo_files/commands_advanced.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 # Licensed under the MIT license.
 #
 # commands_advanced.py: commands used in the advanced mode xt_demo
 
 def get_command_dicts(prev_exper, curr_exper, browse_flag, browse_opt, timeout_opt, templ, archives_dir, 
     monitor_opt):
 	return [
+      # PREREQS
+      {"title": "XT's advanced demo requires Azure Batch and Azure Machine Learning (AML) to be setup and added to xt_config.yaml "
+      + " to get a base template that you can use please run xt config --create batch and xt config --create aml "
+      + " or review the Creating Azure Cloud Services for XT topic on the documentation.", "xt_cmd" : "xt --version"},
+
 	    # OVERVIEW
 	    {"title": "show the XT about page", "xt_cmd": "xt help --about"},
-	    {"title": "show the help topic on the miniMnist app", "xt_cmd": "xt help topic mini_mnist"},
+	    {"title": "show the help topic on Getting Started with XT", "xt_cmd": "xt help topic getting_started"},
 
 	    # CONFIG FILES
 	    {"title": "view the XT default config file", "xt_cmd": "xt config --default"},
 	    {"title": "view the local XT config file", "xt_cmd": "xt config"},
 
 	    # HELP
 	    {"title": "display XT commands", "xt_cmd": "xt help"},
@@ -44,110 +49,115 @@
 	    {"title": "run script on AZURE ML", "xt_cmd": "xt run {}--target=aml --exper={} code\miniMnist.py".format(monitor_opt, curr_exper)},
 
 	    # REPORTS
 	    {"title": "OVERVIEW: status of jobs", "xt_cmd": "xt list jobs --last=4"},
 	    {"title": "ZOOM in on CURRENT experiment", "xt_cmd": "xt list runs --exper={}".format(curr_exper)},
 
 	    # TAGGING
-	    # {"title": "add tag 'good_run' to run5750, run5752", "xt_cmd": "xt set tags run5750, run5752 good_run"},
-	    # {"title": "list runs with the 'good_run' tag", "xt_cmd": "xt list runs --workspace=ws1 --tags=good_run"},
+	    {"title": "add tag 'good_run' to run1, run2", "xt_cmd": "xt set tags run1, run2 good_run"},
+	    {"title": "list runs with the 'good_run' tag", "xt_cmd": "xt list runs --tags=good_run"},
 
 	    # CMD LINE PIPING
-	    {"title": "the 'list runs' and 'list jobs' have powerful filtering and sorting options", "xt_cmd": "xt list runs --exper=miniSearch --sort=metrics.test-acc --last=5"},
+	    {"title": "the 'list runs' and 'list jobs' have powerful filtering and sorting options", "xt_cmd": "xt list runs --exper=search10 --sort=metrics.test-acc --last=5"},
 	    {
 		    "title": "you can leverage the 'list runs' cmd to feed runs into another cmd, using XT command piping", \
-		    "xt_cmd": "!xt list runs --exper=miniSearch --sort=metrics.test-acc --last=5 | xt set tags $ top5"
+		    "xt_cmd": "!xt list runs --exper=search10 --sort=metrics.test-acc --last=5 | xt set tags $ top5"
 		},
 	    # {"title": "let's see which runs are now tagged with 'top5", "xt_cmd": "xt list runs --tags=top5"},
 
 	    # VIEW PORTAL
 	    {"title": "Browse the portal for the 'philly' target", "xt_cmd": "xt view portal philly {}".format(browse_flag), "needs_philly": True},
 	    {"title": "Browse the portal for the 'aml' target", "xt_cmd": "xt view portal aml {}".format(browse_flag)},
 
 	    # TENSORBOARD
         {
 	        "title": "view LIVE tensorboard of cross-service experiments with custom path template",
-	        "xt_cmd": 'xt view tensorboard --work=ws1 --exper={} {} --template="{}"'.format(prev_exper, browse_flag, templ),
+	        "xt_cmd": 'xt view tensorboard --exper=search10 {} --template="{}"'.format(browse_flag, templ),
 	        "needs_gui": True
 	    },
 
 	    # LOG, CONSOLE, ARTIFACTS
-	    #{"title": "view log for run5751", "xt_cmd": "xt view log ws1/run5751"}
-	    # {"title": "view console output of run5751 (Azure ML run)", "xt_cmd": "xt view console ws1/run5751"},
+	    #{"title": "view log for run5751", "xt_cmd": "xt view log run5751"}
+	    {"title": "view console output of run2", "xt_cmd": "xt view console run2"},
 
-	    # {"title": "download all source code, output, and logs for run4940", "xt_cmd": "xt extract ws1/run4940 {}\\run4940 {}".format(archives_dir, browse_opt)},
+	    {"title": "download all source code, output, and logs for run2", "xt_cmd": "xt extract run2 {} {}".format(archives_dir, browse_opt)},
 
 	    # RERUN (monitor_opt is harder to apply here)
-	    # {"title": "rerun run4940, with original source code and hyperparameter settings", "xt_cmd": "xt rerun ws1/run4940"},
+	    {"title": "rerun run2, with original source code and hyperparameter settings", "xt_cmd": "xt rerun run2"},
 
 	    # MOUNT data and DOWNLOAD model
 	    {"title": "run script, mounting data and downloading model for eval", 
             "xt_cmd": "xt run {}--target=philly --data-action=mount --model-action=download code\miniMnist.py --auto-download=0 --eval-model=1". \
                 format(monitor_opt), "needs_philly": True},
 
 	    # DOCKER RUNS
 	    # {"title": "log in to azure docker registry", "xt_cmd": "xt docker login  --environment=pytorch-xtlib "}
 	    # {"title": "log out from docker registry", "xt_cmd": "xt docker logout  --environment=pytorch-xtlib "}
 	    # {"title": "run script in DOCKER container on LOCAL MACHINE", "xt_cmd": "xt --target=local --environment=pytorch-xtlib-local run code\miniMnist.py --no-cuda"}
 	    # {"title": "run script in DOCKER container on BATCH", "xt_cmd": "xt --target=batch --environment=pytorch-xtlib run code\miniMnist.py"}
 
 	    # PARALLEL TRAINING
-	    {
-		    "title": "run parallel training on Azure ML using 4 GPUs", 
-	        "xt_cmd": "xt run {}--target=aml4x code\miniMnist.py --train-percent=1 --test-percent=1 --epochs=100 --parallel=1".format(monitor_opt)
-	    },
+	    # {
+		  #   "title": "run parallel training on Azure ML using 4 GPUs", 
+	    #     "xt_cmd": "xt run {}--target=aml4x code\miniMnist.py --train-percent=1 --test-percent=1 --epochs=100 --parallel=1".format(monitor_opt)
+	    # },
 
 	    # DISTRIBUTED TRAINING
 	    {
 		    "title": "run distributed training on Azure ML using 8 boxes", 
 	        "xt_cmd": "xt run {}--target=aml --direct-run=true --nodes=8 --distributed code\miniMnist.py --train-percent=1 --test-percent=1  " \
                 "--epochs=100  --distributed=1".format(monitor_opt)
 	    },
 
 	    # HPARAM SEARCH
 	    {
 		    "title": "start a hyperparmeter search of 50 runs (5 boxes, 10 runs each) using Azure Batch", 
 	        "xt_cmd": "xt run {}--target=batch --runs=50 --nodes=5 --search-type=dgd --hp-config=code\miniSweeps.yaml code\miniMnist.py".format(monitor_opt)
 	    },
 
-	    # {"title": "view a report of previously completed HP search, ordered by test accuracy", "xt_cmd": "xt list runs --job=job1100 --sort=metrics.test-acc --last=20"},
-	    {"title": "view a report of previously completed HP search, ordered by test accuracy", "xt_cmd": "xt list runs --sort=metrics.test-acc --last=20"},
+	    {
+            "title": "view a report of previously completed HP search, ordered by test accuracy", 
+            "xt_cmd": "xt list runs --job=xtd_job10608 --sort=metrics.test-acc"
+        },
+
+        # HPARAM EXPLORER
+        # NOTE: turn back ON as soon as we merge in PR's #139, #143 
 	    # {
 		#     "title": "open Hyperparameter Explorer to compare the effect of hyperparameter settings on test accuracy, using a previously completed HP search", 
-	    #     "xt_cmd": "xt explore job2731 {}".format(timeout_opt),
+	    #     "xt_cmd": "xt explore xtd_job10608 {}".format(timeout_opt),
         #     "needs_gui": True
 	    # },
 
 	    # AD-HOC PLOTTING (run as external cmd due to problem closing 2nd matplotlib window)
         # SINGLE PLOT of 10 RUNS
-        # {
-	    #     "title": "display a plot of 10 runs",
-	    #     "xt_cmd": '!xt plot job9554 ' + "test-acc {}".format(timeout_opt),
-		# 	"needs_gui": True
-	    # },
+        {
+	        "title": "display a plot of 10 runs",
+	        "xt_cmd": '!xt plot xtd_job10608 ' + "test-acc {}".format(timeout_opt),
+			"needs_gui": True
+	    },
 
         # # APPLY SMOOTHING FACTOR
         # cmd = '!xt plot job9554 ' + \
         #     "test-acc --smooth=.85  {}".format(timeout_opt)
         # {"title": "apply a smoothing factor", cmd)
 
         # # AGGREGATE over runs
         # cmd = '!xt plot job9554 ' + \
         #     "test-acc --smooth=.85 --aggregate=mean --range-type=std {}".format(timeout_opt)
         # {"title": "plot the average the runs, using std as the range area", cmd)
 
         # 2 METRICS, 2x5 MATRIX (break on run)
-        # {
-	    #     "title": "alternatively, let's add a 2nd metric, train-acc, and show each run in its own plot",
-	    #     "xt_cmd": '!xt plot job9554 ' + \
-	    #         "train-acc, test-acc --break=run --layout=2x5 {}".format(timeout_opt),
-	    #     "needs_gui": True
-	    # },
+        {
+	        "title": "alternatively, let's add a 2nd metric, train-acc, and show each run in its own plot",
+	        "xt_cmd": '!xt plot xtd_job10608 ' + \
+	            "train-acc, test-acc --break=run --layout=2x5 {}".format(timeout_opt),
+	        "needs_gui": True
+	    },
 
         # 2 METRICS, 2x1 MATRIX (break on col)
-        # {
-	    #     "title": "finally, we can easily break on the col, instead of the run",
-	    #     "xt_cmd": '!xt plot job9554 ' + \
-	    #         "train-acc, test-acc --break=col --layout=2x1 {}".format(timeout_opt),
-	    #     "needs_gui": True
-	    # }
+        {
+	        "title": "finally, we can easily break on the col, instead of the run",
+	        "xt_cmd": '!xt plot xtd_job10608 ' + \
+	            "train-acc, test-acc --break=col --layout=2x1 {}".format(timeout_opt),
+	        "needs_gui": True
+	    }
 	]
```

### Comparing `xtlib-1.0.0rc1/xtlib/demo_files/xt_demo.py` & `xtlib-1.0.0rc2/xtlib/demo_files/xt_demo.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,27 +25,31 @@
 logger = logging.getLogger(__name__)
 
 cmds = []
 cmd_count = 0
 
 ARCHIVES_DIR = "..\\xt_demo_archives"
 
-def build_cmds(auto_mode, quick_test, nomonitor, nogui, philly=1):
+def build_cmds(auto_mode, quick_test, nomonitor, nogui, philly=1, basic_mode=None):
     config = xt_config.get_merged_config()
-    mini_mode = not config.get("general", "advanced-mode")
+
+    if basic_mode is None:
+        mini_mode = not config.get("general", "advanced-mode")
+    else:
+        mini_mode = basic_mode
 
     is_windows = (os.name == "nt")
     has_gui = pc_utils.has_gui() and not nogui
     browse_flag = "--browse" if has_gui else ""
     browse_opt = "" if auto_mode or not has_gui else "--browse"
     timeout_opt = "--timeout=5" if auto_mode else ""
     monitor_opt = "--monitor=none " if nomonitor else ""
     templ = "{run}_{target}_lr={hparams.lr}_mo={hparams.momentum}_opt={hparams.optimizer}_tt={logdir}"
 
-    # SET THESE before each demo (exper24 should be a multi-service set of simple runs)
+    # SET THESE before each demo (exper26 should be a multi-service set of simple runs)
     prev_exper = "exper18"
     curr_exper = "exper26"
 
     if mini_mode:
         command_dicts = commands_basic.get_command_dicts(
             prev_exper,
             curr_exper,
@@ -68,17 +72,15 @@
 
     if not has_gui:
         command_dicts = list(filter(
             lambda c_dict: not utils.safe_value(c_dict, "needs_gui", default=False),
             command_dicts))
 
     if philly == 0:
-        command_dicts = filter(
-            lambda c_dict: not utils.safe_value(c_dict, "needs_philly", default=False),
-            command_dicts)
+        command_dicts = [ cd for cd in command_dicts if not utils.safe_value(cd, "needs_philly", default=False) ]
 
     list(map(
         lambda cmd_dict: add_cmd(cmd_dict["title"], cmd_dict["xt_cmd"]),
         command_dicts
     ))
 
 
@@ -86,32 +88,40 @@
 
     title = file_utils.fix_slashes(title)
     xt_cmd = file_utils.fix_slashes(xt_cmd)
 
     cmd = {"title": title, "xt_cmd": xt_cmd, "silent": silent}
     cmds.append(cmd)
 
-def wait_for_nav_key(auto_mode):
+def wait_for_nav_key(cmd_text, auto_mode):
+    print(" > " + cmd_text + " ", end="", flush=True)
+
     if auto_mode:
         response = "\r"
     else:
         # get KEYPRESS from user
         while True:
+    
             with KeyPressChecker() as kpc:
                 response = kpc.getch_wait()
-                #xtprint("got reponse=", response)
+                #print("getch: ord(response)={}".format(ord(response)))
+
+                if not response or ord(response) == 0:
+                    continue
 
-            # treat control-c as "q"
-            if response == b'\x03':
+            # treat control-c and ESCAPE as "q"
+            if ord(response) in [3, 27]:
                 response = "q"
 
             if response in ["\r", "\n", "s", "b", "q"]:
                 break
 
-            print("? ", end="", flush=True)
+            #print("? ", end="", flush=True)
+            print("(press ENTER to run, 'q' to quit, 's' for skip, or 'b' for back)")
+            print(" > " + cmd_text + " ", end="", flush=True)
 
     print()
     return response
 
 def wait_for_any_key(auto_mode):
     if auto_mode:
         response = "\r"
@@ -173,17 +183,16 @@
                 cmd_text += " --response=y"
             elif cmd_text.startswith("xt explore"):
                 cmd_text += " --timeout=5"
             # elif "--open" in cmd_text:
             #     cmd_text = cmd_text.replace("--open", "")
 
         print("xt demo {}/{}: {}".format(index+1, len(cmds), cmd["title"]))
-        print(" > " + cmd_text + " ", end="", flush=True)
 
-        response = wait_for_nav_key(auto_mode)
+        response = wait_for_nav_key(cmd_text, auto_mode)
         #print("response=", response, 'b"q"=', b"q", response == b"q")
 
         if response in ["\r", "\n"]:
             # ---- RUN COMMAND ---- 
             if cmd_text.startswith("xt "):
                 # run XT cmd internally
                 fb.reset_feedback()
@@ -228,14 +237,15 @@
     parser = argparse.ArgumentParser(description='XT Demo')
 
     parser.add_argument('--auto', action='store_true', default=False, help='runs the demo unattended')
     parser.add_argument('--nomonitor', action='store_true', default=False, help='prevents monitoring of XT run commands')
     parser.add_argument('--nogui', action='store_true', default=False, help='prevents running of GUI commands')
     parser.add_argument('--philly', default=0, type=int, help='should Philly tests be run')
     parser.add_argument('--quick-test', action='store_true', default=False, help='specifies we are running as part of the quick-test')
+    parser.add_argument('--basic-mode', default=None, type=int,  help='specifies if basic or advanced mode demo should be run')
     parser.add_argument("steps", nargs="*", help="the steps to be run")
 
     if not arg_list:
         arg_list = sys.argv[1:]
     args = parser.parse_args(arg_list)
 
     print("parsed xt_demo args:", args)
@@ -273,35 +283,37 @@
 
     args = parse_args(arg_list)
     auto_mode = args.auto
     nomonitor = args.nomonitor
     nogui = args.nogui
     quick_test = args.quick_test
     philly = args.philly
+    basic_mode = args.basic_mode
 
-    build_cmds(auto_mode, quick_test, nomonitor, nogui, philly=philly)
+    build_cmds(auto_mode, quick_test, nomonitor, nogui, philly=philly, basic_mode=basic_mode)
 
     steps = parse_steps(args.steps)
-    response = ""
+    response = "x"
 
     if not auto_mode:
         print()
         print("This demonstrates how to run common XT commands")
         print("Press ENTER to execute each command (or s=SKIP, b=BACK, q=QUIT)")
         print()
 
         print("hit any key to continue: ", end="", flush=True)
         response = wait_for_any_key(auto_mode)
 
-    if response != "q":
+        if response and response != "q" and not ord(response) in [3, 27]:
+            navigate(cmds, auto_mode, steps)
+    else:
         navigate(cmds, auto_mode, steps)
 
     # clean-up
     file_utils.ensure_dir_deleted(ARCHIVES_DIR)
 
     print("end of xt_demo")
 
     return cmd_count
 
 if __name__ == "__main__":
     main()
-
```

### Comparing `xtlib-1.0.0rc1/xtlib/qfe.py` & `xtlib-1.0.0rc2/xtlib/qfe.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/helpers/yaml_dump.py` & `xtlib-1.0.0rc2/xtlib/helpers/yaml_dump.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,30 +57,33 @@
         if isinstance(value, str):
             value = '"' + value + '"'
         line += str(value)
 
     text += line+ "]"
     return text
 
-def pretty_yaml_dump(dd):
+def pretty_yaml_dump(dd, read_only_text=True):
     '''
     dump the data dict "dd" as XT config style yaml text
     '''
-    text = '''#-------------------------------------------------------------------------------------------------------------------
+    if read_only_text:
+        text = '''#-------------------------------------------------------------------------------------------------------------------
 # DO NOT EDIT:
 #   - a new version of this file is released with each XTLib version; it will overwrite this file without warning.
 #   - to change a subset of these properties, use the "xt config" to create a LOCAL (current directory) config file.
 #-------------------------------------------------------------------------------------------------------------------
 # default_config.yaml: default configuration file for XT.  (READONLY)
 #    The contents of this file contain the default settings that define how XT operates.  Many of the settings can be 
 #    overridden by the various XT command  options (see "xt help commands" for more details). Detailed instructions 
 #    for getting started with this config file are available in the "XT Config File" help topic.
 #-------------------------------------------------------------------------------------------------------------------
 
 '''
+    else:
+        text = ''
 
     for key, value in dd.items():
         text += "{}:\n".format(key)
 
         # if key == "providers":
         #     print("asdf")
```

### Comparing `xtlib-1.0.0rc1/xtlib/helpers/validator.py` & `xtlib-1.0.0rc2/xtlib/helpers/validator.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/helpers/stream_capture.py` & `xtlib-1.0.0rc2/xtlib/helpers/stream_capture.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/helpers/dot_dict.py` & `xtlib-1.0.0rc2/xtlib/helpers/dot_dict.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/helpers/hexdump.py` & `xtlib-1.0.0rc2/xtlib/helpers/hexdump.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/helpers/part_scanner.py` & `xtlib-1.0.0rc2/xtlib/helpers/part_scanner.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/helpers/feedbackParts.py` & `xtlib-1.0.0rc2/xtlib/helpers/feedbackParts.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/helpers/xt_config.py` & `xtlib-1.0.0rc2/xtlib/helpers/xt_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -503,14 +503,17 @@
         shutil.copyfile(fn_source, fn)
 
         # make file readonly
         file_utils.make_readonly(fn)
 
     return fn
 
+def get_default_config_template_path():
+    return os.path.join(file_utils.get_xtlib_dir(), "helpers", constants.FN_DEFAULT_TEMPLATE)
+
 def load_and_validate_config(fn, validate_as_default):
 
     # load the config file
     config = XTConfig(fn=fn, create_if_needed=False)
 
     # load the validation schema
     fn_schema = os.path.join(file_utils.get_xtlib_dir(), "helpers", "xt_config_schema.yaml")
```

### Comparing `xtlib-1.0.0rc1/xtlib/helpers/scanner.py` & `xtlib-1.0.0rc2/xtlib/helpers/scanner.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/helpers/feedbackProgress.py` & `xtlib-1.0.0rc2/xtlib/helpers/feedbackProgress.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/helpers/notebook_builder.py` & `xtlib-1.0.0rc2/xtlib/helpers/notebook_builder.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/helpers/file_helper.py` & `xtlib-1.0.0rc2/xtlib/helpers/file_helper.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/helpers/key_press_checker.py` & `xtlib-1.0.0rc2/xtlib/helpers/key_press_checker.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,29 +22,40 @@
             self.old_settings = termios.tcgetattr(sys.stdin)
 
             # put stdin into CHAR mode
             tty.setcbreak(sys.stdin.fileno())
 
         return self
 
+    def _get_windows_char(self, encoding):
+        bb = msvcrt.getch()
+
+        if bb == '\000' or bb == '\xe0':
+            # special function key indicator; next keycode is actual key
+            bb = msvcrt.getch()
+
+        try:
+            ch = bb.decode(encoding)
+        except BaseException as ex:
+            #console.print("KeyPressChecker exception decoding bb={}: {}".format(bb, ex))
+            ch = ""
+
+        return ch
+
     def getch_wait(self, encoding='utf-8'):
         '''
         Returns:
             string of single key pressed
         Description:
             wait for single key press and return its identity
         '''
         ch = None
         if self.is_windows:
             import msvcrt
-            bb = msvcrt.getch()
-            if bb == '\000' or bb == '\xe0':
-                # special function key indicator; next keycode is actual key
-                bb = msvcrt.getch()
-            ch = bb.decode(encoding)
+            ch = self._get_windows_char(encoding)
         else:
             # linux
             ch = sys.stdin.read(1)
         return ch
 
     def getch_nowait(self, encoding='utf-8'):
         '''
@@ -53,23 +64,15 @@
         Description:
             check to see if a key has been pressed
         '''
         ch = None
         if self.is_windows:
             import msvcrt
             if msvcrt.kbhit():
-                bb = msvcrt.getch()
-                if bb == '\000' or bb == '\xe0':
-                    # special function key indicator; next keycode is actual key
-                    bb = msvcrt.getch()
-                try:
-                    ch = bb.decode(encoding)
-                except BaseException as ex:
-                    console.print("KeyPressChecker exception decoding bb={}: {}".format(bb, ex))
-                    ch = ""
+                ch = self._get_windows_char(encoding)
         else:
             # linux
             if select.select([sys.stdin], [], [], 0) == ([sys.stdin], [], []):
                 ch = sys.stdin.read(1)
         return ch
 
     def __exit__(self, type, value, traceback):
```

### Comparing `xtlib-1.0.0rc1/xtlib/helpers/bag.py` & `xtlib-1.0.0rc2/xtlib/helpers/bag.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/pc_utils.py` & `xtlib-1.0.0rc2/xtlib/pc_utils.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/job_helper.py` & `xtlib-1.0.0rc2/xtlib/job_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 
 from xtlib import qfe
 from xtlib import utils
 from xtlib import errors
 from xtlib import file_utils
 from xtlib.storage import fixup_mongo_jobs 
 
+def is_job_id(name):
+    part = name.split("_")[-1]
+    return part.startswith("job")
+
 def expand_job_list(store, mongo, workspace, name_list, can_mix=True):
     '''
     parse jobs, expand job ranges
     '''
     if name_list:
         first_name = name_list[0]
         if len(name_list)==1 and file_utils.has_wildcards(first_name):
@@ -72,15 +76,18 @@
                     console.print("  {}: {}".format(tag, tags[tag]))
     else:
         console.print("no matching jobs found")
 
 def build_filter_part(fd, args, arg_name, store_name):
     value = args[arg_name]
     if value:
-        fd[store_name] = value
+        if isinstance(value, list):
+            fd[store_name] = {"$in": value}
+        else:
+            fd[store_name] = value
 
 def build_job_filter_dict(job_list, user_to_actual, builder, workspace, args):
     fd = {}
     option_filters = ["experiment", "target", "service_type", "username"]   # "application"
 
     if job_list:
         # filter by specified job names
@@ -163,18 +170,17 @@
         "running_runs": "the number of this job's runs that are current running",
         "completed_runs": "the number of runs that have completed (with or without errors)",
         "error_runs": "the number of runs that have terminated with an error",
     }
 
     return user_to_actual, std_cols_desc
 
-def list_jobs(store, config, args):
+def get_list_jobs_records(store, config, args):
     job_list = args["job_list"]
     pool = args["target"]
-    available = args["available"]
 
     if job_list:
         # only use workspace if it was explictly set  
         workspace = None   
         explict = qfe.get_explicit_options()
         if "workspace" in explict:
             workspace = explict["workspace"]
@@ -199,14 +205,21 @@
 
     # have MONGO update any old JOB documents to new format
     fixup_mongo_jobs.fixup_jobs_if_needed(mongo.mongo_db)
 
     # get the mongo records for the matching JOBS
     #console.print("gathering job data...", flush=True)
     records, using_default_last, last = builder.get_mongo_records(mongo, filter_dict, workspace, "jobs", actual_to_user, args=args)
+    return records, using_default_last, last, user_to_actual, builder
+
+def list_jobs(store, config, args):
+    available = args["available"]
+
+    records, using_default_last, last, user_to_actual, builder \
+        = get_list_jobs_records(store, config, args)
 
     if available:
         std_cols = list(user_to_actual.keys())
         tag_cols = extract_tag_cols(records)
         lines = builder.available_cols_report("job", std_cols, std_cols_desc, tags_list=tag_cols)
 
         for line in lines:
@@ -246,15 +259,15 @@
             for tag in tags.keys():
                 tag_dict[tag] = 1
 
     return list(tag_dict.keys())
 
 def validate_job_name_with_ws(store, job_name, validate):
     job_name = job_name.lower()
-    if not job_name.startswith("job"):
+    if not is_job_id(job_name):
         return errors.syntax_error("Illegal job name: {}".format(job_name))
 
     ws = store.get_job_workspace(job_name)
     if validate and not ws:
         errors.store_error("job '{}' does not exist".format(job_name))
 
     return ws
@@ -269,18 +282,22 @@
     else:
         ws = actual_ws
         
     job_list.append(job)
     return ws if ws else actual_ws
 
 def get_job_number(job):
-    if not job.startswith("job"):
+    if not is_job_id(job):
         errors.syntax_error("illegal job name, must start with 'job'")
 
-    return int(job[3:])
+    # allow for import prefixes
+    part = job.split("_")[-1]  
+    if part.startswith("job"):
+        part = part[3:] 
+    return int(part)
 
 def parse_job_list(store, workspace, jobs, can_mix=False):
     actual_ws = None
     job_list = []
 
     if jobs:
         for job in jobs:
@@ -302,15 +319,15 @@
         
     #console.print("actual_ws=", actual_ws)
     return job_list, actual_ws
 
 def validate_job_name(job_id):
     if job_id:
         safe_job_id = str(job_id)
-        if not safe_job_id.startswith("job"):
+        if not is_job_id(safe_job_id):
             errors.syntax_error("job id must start with 'job': " + safe_job_id)
 
 def get_num_from_job_id(job_id):
     # job341
     return job_id[3:]
 
 def get_client_cs(core, job_id, node_index):
```

### Comparing `xtlib-1.0.0rc1/xtlib/utils.py` & `xtlib-1.0.0rc2/xtlib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import datetime
 import traceback
 import importlib
 
 from xtlib import errors
 from xtlib import constants
 from xtlib import file_utils
+from xtlib import job_helper
 
 from xtlib.console import console
 from xtlib.helpers.feedbackParts import feedback as fb
 
 class PropertyBag: pass
 
 # utils internal variables
@@ -60,15 +61,15 @@
 def is_azure_ml_box(box_name):
     return (box_name and "-aml-" in box_name)
 
 def is_philly_box(box_name):
     return (box_name and "-philly-" in box_name)
 
 def is_service_box(box_name):
-    return box_name and box_name.startswith("job") and "-" in box_name
+    return box_name and job_helper.is_job_id(box_name) and "-" in box_name
 
 def load_json_records(text):
     # each line is a JSON text record, with a newline at the end
     json_text = "[" + text.replace("\n", ",")[0:-1] + "]"
     records = json.loads(json_text)
     return records
 
@@ -401,19 +402,22 @@
             fnx = fn
         fn_dest = os.path.join(submit_logs, os.path.basename(fn))
         shutil.copyfile(fn, fn_dest)
         console.diag("copied {} to: {}".format(fn, fn_dest))
 
 def get_controller_cwd(is_windows, is_local=False):
     if is_windows:
+        # we only support windows as a local machine
+        #cwd = os.path.expanduser("~/.xt/cwd")
+
         # docker has problems mapping paths to user home directories (~/)
         # controller app has problems copying/deleting files in 'programdata' folder
-        # so, for windows, we use this
-        program_data = "c:\\xt_controller"
-        cwd = file_utils.path_join(program_data, "xt", "cwd")
+        # so, for windows, we use this:
+        sys_drive = os.getenv("SystemDrive")
+        cwd = file_utils.path_join(sys_drive + "/xt", "cwd")
     else:   
         cwd =  "~/.xt/cwd"
 
         # only safe to expand if local
         if is_local:
             cwd = os.path.expanduser(cwd)
 
@@ -510,7 +514,8 @@
 def find_by_property(elements, prop, target):
     result = next((elem for elem in elements if prop in elem and elem[prop] == target), None) 
     return result
 
 def report_elapsed(start, name):
     elapsed = time.time() - start
     print("{} took: {:.2f} secs".format(name, elapsed))
+
```

### Comparing `xtlib-1.0.0rc1/xtlib/repair_runs.py` & `xtlib-1.0.0rc2/xtlib/repair_runs.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/impl_base.py` & `xtlib-1.0.0rc2/xtlib/impl_base.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/impl_storage.py` & `xtlib-1.0.0rc2/xtlib/impl_storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,19 +26,20 @@
 from xtlib import box_information
 
 from xtlib.storage.store import Store
 from xtlib.client import Client
 from xtlib.console import console
 from xtlib.cmd_core import CmdCore
 from xtlib.impl_base import ImplBase
+from xtlib.helpers import file_helper
 from xtlib.backends import backend_aml 
 from xtlib.cache_client import CacheClient
 from xtlib.report_builder import ReportBuilder   
+from xtlib.impl_storage_api import ImplStorageApi
 from xtlib.hparams.hyperex import HyperparameterExplorer
-from xtlib.helpers.feedbackProgress import FeedbackProgress
 from xtlib.qfe import command, argument, keyword_arg, option
 from xtlib.qfe import flag, faq, root, example, clone, command_help, see_also
 
 '''
 This module implements the following commands:
 
 manage resources:
@@ -75,14 +76,15 @@
     def __init__(self, config, store):
         super(ImplStorage, self).__init__()
         self.config = config
         self.store = store
         self.core = CmdCore(self.config, self.store, None)
         self.client = Client(config, store, None)
         self.client.core = self.core
+        self.impl_storage_api = ImplStorageApi(self.config, self.store)
 
     def is_aml_ws(self, ws_name):
         return False  # self.azure_ml.does_ws_exist(ws_name)
 
     def get_first_last_filtered_names(self, names, first_count=None, last_count=None, top_adjust=0, bot_adjust=0):
         if first_count:
             names = names[:first_count]   #  + top_adjust]
@@ -150,22 +152,22 @@
         '''
         self.store.create_workspace(workspace)
         console.print("workspace created: " + workspace)
 
     #---- DELETE SHARE command ----
     @argument("share", help="the name of the share to be deleted")
     @option("response", default=None, help="the response to be used to confirm the share deletion")
-    @example(task="delete the share named 'trjectories'", text="xt delete share trajectories")
+    @example(task="delete the share named 'trajectories'", text="xt delete share trajectories")
     @command(kwgroup="delete", help="deletes the specified share")
     def delete_share(self, share, response):
         if not self.store.does_share_exist(share):
             errors.store_error("share not defined: " + share)
         else:
             # get top level folders
-            fs = self.create_file_accessor(use_blobs=True, share=share, ws_name=None, exper_name=None, job_name=None, run_name=None)
+            fs = self.impl_storage_api.create_file_accessor(use_blobs=True, share=share, ws_name=None, exper_name=None, job_name=None, run_name=None)
             dd = fs.list_directories("", subdirs=0)
             folders = dd["folders"]
             count = len(folders)
 
             answer = pc_utils.input_response("Enter '{}' to confirm deletion of share ({} top level folders): ".format(share, count), response)
             if answer == share:
                 self.store.delete_share(share)
@@ -178,18 +180,23 @@
     @option("response", default=None, help="the response to be used to confirm the workspace deletion")
     @example(task="delete the workspace named 'project-x'", text="xt delete work project-x")
     @command(kwgroup="delete", help="deletes the specified workspace")
     def delete_workspace(self, workspace, response):
         if not self.store.does_workspace_exist(workspace):
             errors.store_error("workspace not defined: " + workspace)
         else:
-            names = self.store.get_run_names(workspace)
-            count = len(names)
+            run_names = self.store.get_run_names(workspace)
+            run_count = len(run_names)
+
+            job_names = self.store.mongo.get_job_names({"ws_name": workspace})
+            job_count = len(job_names)
+
+            answer = pc_utils.input_response("Enter '{}' to confirm deletion of workspace ({} jobs, {} runs): ". \
+                format(workspace, job_count, run_count), response)
 
-            answer = pc_utils.input_response("Enter '{}' to confirm deletion of workspace ({} runs): ".format(workspace, count), response)
             if answer == workspace:
                 self.store.delete_workspace(workspace)
                 console.print("workspace deleted: " + workspace)
             else:
                 console.print("workspace not deleted")
 
     #---- LIST EXPERIMENTS command ----
@@ -269,15 +276,15 @@
     @argument(name="name", help="the name of the run or job")
     @option(name="workspace", default="$general.workspace", help="the workspace that the run resides in")
     @option(name="node-index", default=0, help="the node index for the specified job")
     @example(task="view the console output for run26 in the curious workspace", text="xt view console curions/run26")
     @example(task="view the console output for job201, node3", text="xt view console job201 --node-index=3")
     @command(kwgroup="view",  help="view console output for specified run")
     def view_console(self, name, workspace, node_index):
-        if name.startswith("job"):
+        if job_helper.is_job_id(name):
             # treat target as job_name
             job_name = name
             workspace = job_helper.validate_job_name_with_ws(self.store, job_name, True)
             fn = "node-{}/after/stdout.txt".format(node_index)
 
             if not self.store.does_job_file_exist(job_name, fn):
                 console.print("job '{}' has no file'{}'".format(job_name, fn))
@@ -303,42 +310,63 @@
             else:
                 console.print("{} for {}:\n".format(fn, full_run_name))
 
                 text = self.store.read_run_file(ws, run_name, fn)
                 text = pc_utils.make_text_display_safe(text)
                 console.print(text)
 
+    #---- EXPORT WORKSPACE command ----
+    @argument(name="output-file", help="the name of the output file to export workspace to")
+    @option(name="workspace", default="$general.workspace", help="the workspace that the run resides in")
+    @option(name="experiment", type="str_list", help="matches jobs belonging to the experiment name")
+    @option(name="tags-all", type="str_list", help="matches jobs containing all of the specified tags")
+    @option(name="tags-any", type="str_list", help="matches jobs containing any of the specified tags")
+    @option(name="jobs", type="str_list", help="list of jobs to include")
+    @example(task="export workspace ws5 to ws5_workspace.zip", text="xt export workspace ws5_workspace.zip --workspace=ws5")
+    @command(help="exports a workspace to a workspace archive file")
+    def export_workspace(self, output_file, workspace, tags_all, tags_any, jobs, experiment):
+        self.impl_storage_api.export_workspace(output_file, workspace, tags_all, tags_any, jobs, experiment, show_output=True)
+
+    #---- IMPORT WORKSPACE command ----
+    @argument(name="input-file", help="the name of the archive file (.zip) to import the workspace from")
+    @argument(name="new-workspace", required=False, help="the new name for the imported workspace")
+    @option(name="job-prefix", default="imp", help="the prefix to add to imported job names")
+    @flag("overwrite", help="When specified, any existing jobs with the same prefix and name will be overwritten")
+    @example(task="import workspace from workspace.zip as new_ws5", text="xt import workspace workspace.zip new_ws5")
+    @command(help="imports a workspace from a workspace archive file")
+    def import_workspace(self, input_file, new_workspace, job_prefix, overwrite):
+        self.impl_storage_api.import_workspace(input_file, new_workspace, job_prefix, overwrite, show_output=True)
+
     #---- VIEW RUN command ----
     @argument(name="run-name", help="the name of the run")
     @option(name="workspace", default="$general.workspace", help="the workspace that the run resides in")
     @example(task="view information for run26", text="xt view run26")
     @command(kwgroup="view",  help="view information for specified run")
     def view_run(self, run_name, workspace):
         console.print("run: {}".format(run_name))
-        
 
     #---- VIEW LOG command ----
     @argument(name="target", help="the name of the run or job")
     #@option(name="box", default="local", help="the name of the box to use (for the controller log)")
     @option(name="workspace", default="$general.workspace", help="the workspace that the run resides in")
     @example(task="view the log entries for run26 in the curious workspace", text="xt view log curious/run26")
     @command(kwgroup="view", help="view the run log for specified run")
-    def view_log(self, target, workspace, box):
+    def view_log(self, target, workspace):
         is_aml = self.is_aml_ws(workspace)
 
         # if target == "controller":
         #     # view CONTROLLER LOG from specified box
         #     if self.client.connect_to_controller(box):
         #         text = self.client.get_controller_log()
         #         console.print("box={}, controller log:".format(box.upper()))
         #         console.print(text)
         #     else:
         #         console.print("couldn't connect to controller for target: {}".format(target))
 
-        if target.startswith("job"):
+        if job_helper.is_job_id(target):
             # view JOB LOG
             records = self.store.get_job_log(target)
             console.print("log for {}:\n".format(target))
             for record in records:
                 console.print(record)
 
         else:
@@ -472,20 +500,21 @@
         # hand-validate break-on values
         if break_on:
             for value in break_on:
                 if not value in ["col", "run", "group"]:
                     errors.syntax_error("break-on values must be one of: col, run, or group")
 
         args = {"run_list": runs, "workspace": workspace, "all": True, "sort_col": "name", 
-            "max_runs": max_runs, "columns": ["run", "metrics.*"]}
+            "max_runs": max_runs, "columns": ["run", "metrics.*"] }
 
         x_col = x
         
         # store col names used here
-        col_dict = {"run_name": 1, "node_index": 1, "job_id": 1, "exper_name": 1, "ws": 1, "log_records": 1}
+        col_dict = {"run_name": 1, "node_index": 1, "job_id": 1, "exper_name": 1, "ws": 1, 
+            "search_style": 1, "log_records": 1}
 
         run_log_records, using_default_last, user_to_actual, available, builder, last, std_cols_desc = \
             run_helper.get_filtered_sorted_limit_runs(self.store, self.config, False, col_dict=col_dict, args=args)
 
         # metric string will later contain calculated expressions
         if not col_list:
             col_list = []
@@ -501,15 +530,15 @@
 
     #---- EXTRACT command ----
     @argument(name="runs", type="str_list", help="a comma separated list of runs, jobs, or experiments", required=True)
     @argument(name="dest-dir", help="the path of the directory")
     @flag(name="browse", help="specifies that an folder window should be opened for the dest_dir after the extraction has completed")
     @option(name="workspace", default="$general.workspace", help="the workspace that the runs resides in")
     @option("response", default=None, help="the response to be used to confirm the directory deletion")
-    @example(task="extract files from curious/run26 to c:\\run26_files", text="xt extract curious/run26 c:\\run26_files")
+    @example(task="extract files from curious/run26 to ./run26_files", text="xt extract curious/run26 ./run26_files")
     @command(help="download all files associated with the run to the specified directory")
     def extract(self, runs, dest_dir, workspace, response, browse):
         is_aml = self.is_aml_ws(workspace)
         #ws, run_name, full_run_name = run_helper.validate_run_name(self.store, workspace, run_name, parse_only=is_aml)
 
         console.print("extracting files for: {}...".format(runs))
 
@@ -523,15 +552,15 @@
         if extract:
             file_utils.ensure_dir_clean(dest_dir)
 
             # first, determine nodes to be added to dest_dir
             nodes = "run"   # default
 
             for name_entry in runs:
-                if name_entry.startswith("job"):
+                if job_helper.is_job_id(name_entry):
                     # if we find at least 1 job name specified, output to dest_dir/jobNNN/runNNN
                     if not nodes == "exper":
                         nodes = "job"
                 elif not name_entry.startswith("run"):
                     # if we find at least 1 experiment, output to dest_dir/experFoo/jobNNN/runNNN
                     # this takes priority over all other nodes values
                     nodes = "exper"
@@ -603,15 +632,15 @@
     @example(task="explore the results of all runs from job2998", text="xt explore job2998")
     @command(help="run the Hyperparameter Explorer on the specified job or experiment")
     def explore(self, aggregate_name, workspace, cache_dir, steps_name, log_interval_name, 
         primary_metric, step_name, time_name, success_rate_name, sample_efficiency_name, timeout): 
     
         # we need to respond to the job or experiment name user has specified
         dest_name = aggregate_name
-        aggregate_dest = "job" if dest_name.startswith("job") else "experiment"
+        aggregate_dest = "job" if job_helper.is_job_id(dest_name) else "experiment"
 
         #console.print("metric=", metric)
         if aggregate_dest == "job":
             _, filenames = self.store.get_job_filenames(dest_name, constants.HP_CONFIG_DIR)
             if not filenames:
                 errors.store_error("Missing hp-config file for job={}".format(dest_name))
         else:
@@ -622,18 +651,15 @@
         for f in filenames:
             if f.endswith('.yaml'):
                 filename = f
 
         fn_hp_config = constants.HP_CONFIG_DIR + "/" + filename
         #console.print("found hp-config file: ", fn_hp_config)
 
-        # plotted_metric is the Y axis for big HX plot
-        plotted_metric = primary_metric    # default value
-
-        if dest_name.startswith("job"):
+        if job_helper.is_job_id(dest_name):
             job_ws = self.store.get_job_workspace(dest_name)
             if job_ws:
                 console.diag("{} found in ws={}".format(dest_name, job_ws))
             console.diag("after get_job_workspace call (mongo-db)")
 
             # See if this job has tags for metric names needed by HX.
             filter_dict = {"job_id": dest_name}
@@ -670,15 +696,15 @@
     @option(name="run", help="the run name that the path is relative to")
     @option(name="experiment", help="the experiment that the path is relative to")
     @example(task="display the contents of the specified file from the 'after' snapshot for the specified run", text="xt view blob after/output/userapp.txt --run=curious/run14")
     @command(kwgroup="view", kwhelp="view the specified storage item", help="display the contents of the specified storage blob")
     def view_blob(self, path, share, workspace, job, experiment, run):
 
         use_blobs = True
-        fs = self.create_file_accessor(use_blobs=True, share=share, ws_name=workspace, 
+        fs = self.impl_storage_api.create_file_accessor(use_blobs=True, share=share, ws_name=workspace, 
             exper_name=experiment, job_name=job, run_name=run)
 
         text = fs.read_file(path)
         # if job:
         #     text = self.store.read_job_file(job, path)
         # elif experiment:
         #     text = self.store.read_experiment_file(workspace, experiment, path)
@@ -731,15 +757,15 @@
             username = self.config.expand_system_symbols("$username")
             if not cluster:
                 target = self.config.get_compute_def(target_name)
                 cluster = target["cluster"]
 
             url = "https://philly/#/jobSummary/{}/all/{}".format(cluster, username)
         elif service_type == "batch":
-            url = '"" "C:\\Program Files\\BatchExplorer\\BatchExplorer.exe"'
+            url = "BatchExplorer.exe"
         else:
             errors.syntax_error("Unrecognized service_type: " + service_type)
 
         if browse:
             import webbrowser
             webbrowser.open(url)
         else:
@@ -761,20 +787,20 @@
     def view_team(self, team):
         # for now, its just an echo of your CURRENT (or specified) team name
         console.print("team: {}".format(team))
 
     #---- LIST RUNS command ----
     @argument(name="run-list", type="str_list", help="a comma separated list of: run names, name ranges, or wildcard patterns", required=False)
     @option(name="workspace", default="$general.workspace", help="the workspace for the runs to be displayed")
-    @option(name="job", help="the job id(s) for the runs to be displayed (acts as a filter)")
-    @option(name="experiment", help="the experiment name for the runs to be displayed (acts as a filter)")
+    @option(name="job", type="str_list", help="a list of jobs names (acts as a runs filter)")
+    @option(name="experiment", type="str_list", help="a list of experiment names (acts as a runs filter)")
     #@option(name="application", help="the application name for the runs to be displayed (acts as a filter)")
-    @option(name="box", help="the name of the box on which the runs were running (acts as a filter)")
-    @option(name="target", help="the name of the compue target used by runs (acts as a filter)")
-    @option(name="service-type", help="the name of the back service on which the runs executed (acts as a filter)")
+    @option(name="box", type="str_list", help="a list of boxes on which the runs were running (acts as a filter)")
+    @option(name="target", type="str_list", help="a list of compute targets used by runs (acts as a filter)")
+    @option(name="service-type", type="str_list", help="a list of back services on which the runs executed (acts as a filter)")
 
     # report options 
     @flag(name="all", help="don't limit the output; show all records matching the specified filters")
     @option(name="add-columns", type="str_list", help="list of columns to add to those in config file")
     @option(name="first", type=int, help="limit the output to the first N items")
     @option(name="last", type=int, default="$run-reports.last", help="limit the output to the last N items")
     @option(name="filter", type="prop_op_value", multiple=True, help="a list of filter expressions used to include matching records")
@@ -786,15 +812,15 @@
     @option(name="max-width", type=int, default="$run-reports.max-width", help="set the maximum width of any column")
     @option(name="precision", type=int, default="$run-reports.precision", help="set the number of factional digits for float values")
     @option(name="columns", type="str_list", default="$run-reports.columns", help="specify list of columns to include")
     @option(name="export", type="str", help="will create a tab-separated file for the report contents")
     @option(name="status", type="str_list", default="$run-reports.status", 
         values= ["created", "allocating", "queued", "spawning", "running", "completed", "error", "cancelled", "aborted", "unknown"], 
         help="match runs whose status is one of the values in the list")
-    @option(name="username", type="str", help="only show runs for the specified username")
+    @option(name="username", type="str_list", help="a list of usernames to filter the runs")
     
     # report flags
     @flag(name="flat", help="do not group runs")
     @flag(name="reverse", help="reverse the sorted items")
     #@flag(name="boxout", help="only list the latest run record for each box")
     @flag(name="parent", help="only list parent runs")
     @flag(name="child", help="only list child runs")
@@ -832,32 +858,32 @@
             - To show runs where the repeat is set to something other than None, --filter="repeat!=$none".
         '''
         return run_helper.list_runs(self.store, self.config, args)
 
     #---- LIST JOBS command ----
     @argument(name="job-list", type="str_list", required=False, help="a comma separated list of job names, or a single wildcard pattern")
     @option(name="workspace", default="$general.workspace", help="the workspace for the job to be displayed")
-    @option(name="experiment", help="the experiment name for the runs to be displayed (acts as a filter)")
+    @option(name="experiment", type="str_list", help="a list of experiment names for the jobs to be displayed (acts as a filter)")
     #@option(name="application", help="the application name for the runs to be displayed (acts as a filter)")
-    @option(name="target", help="the name of the compute target associated with the jobs (acts as a filter)")
-    @option(name="service-type", help="the name of the backend service associated with the jobs (acts as a filter)")
+    @option(name="target", type="str_list", help="a list of compute target associated with the jobs (acts as a filter)")
+    @option(name="service-type", type="str_list", help="a list of backend services associated with the jobs (acts as a filter)")
 
     # report options 
     @flag(name="all", help="don't limit the output; show all records matching the specified filters")
     @option(name="first", type=int, help="limit the output to the first N items")
     @option(name="last", type=int, default="$job-reports.last", help="limit the output to the last N items")
     @option(name="filter", type="prop_op_value", multiple=True, help="a list of filter expressions used to include matching records")
     @option(name="tags-all", type="str_list", help="matches records containing all of the specified tags")
     @option(name="tags-any", type="str_list", help="matches records containing any of the specified tags")
     @option(name="sort", default="$run-reports.sort", help="the name of the report column to use in sorting the results")
     @option(name="max-width", type=int, default="$run-reports.max-width", help="set the maximum width of any column")
     @option(name="precision", type=int, default="$run-reports.precision", help="set the number of factional digits for float values")
     @option(name="columns", type="str_list", default="$job-reports.columns", help="specify list of columns to include")
     @option(name="export", type="str", help="will create a tab-separated file for the report contents")
-    @option(name="username", type="str", help="only show runs for the specified username")
+    @option(name="username", type="str_list", help="a list of usernames that started the jobs (acts as a filter)")
     
     # report flags
     @flag(name="reverse", help="reverse the sorted items")
     @flag(name="available", help="show the columns (name, target, search-type, etc.) available for jobs")
 
     # examples, FAQs
     @example(task="display a report of the last 5 jobs that were run", text="xt list jobs --last=5")
@@ -877,250 +903,44 @@
 
         Examples:
         
             - To show runs where the repeat is set to something other than None, --filter="repeat!=$none".
         '''
         return job_helper.list_jobs(self.store, self.config, args)
 
-    def create_file_accessor(self, use_blobs, share, ws_name, exper_name, job_name, run_name):
-        # use --experiment option only here
-        if share:
-            ws_name = utils.make_share_name(share)
-            fs = self.store.root_files(ws_name, use_blobs=use_blobs)
-        elif job_name:
-            fs = self.store.job_files(job_name, use_blobs=use_blobs)
-        elif exper_name:
-            fs = self.store.experiment_files(ws_name, exper_name, use_blobs=use_blobs)
-        elif run_name:
-            fs = self.store.run_files(ws_name, run_name, use_blobs=use_blobs)
-        else:
-            fs = self.store.workspace_files(ws_name, use_blobs=use_blobs)
-
-        return fs
-
-    def make_dest_fn(self, source_basepath, source_fn, dest_rel):
-        ''' combine the relative part of source_path with dest_rel
-        '''
-        slen = len(source_basepath)
-        source_rel = source_fn[1+slen:] 
-
-        dest_fn = os.path.join(dest_rel, source_rel)
-        return dest_fn
-
     #---- UPLOAD command ----
     @argument(name="local-path", help="the path for the local source file, directory, or wildcard")
     @argument(name="store-path", required=False, help="the path for the destination store blob or folder")
-    @option(name="share", help="the name of the share that the path is relative to")
+    @option(name="share", required=True, help="the name of the share that the path is relative to")
     @option(name="workspace", default="$general.workspace", help="the workspace name that the path is relative to")
     @option(name="job", help="the job id that the path is relative to")
     @option(name="experiment", help="the experiment that the path is relative to")
     @option(name="run", help="the run name that the path is relative to")
-    @flag(name="feedback", help="when True, incremental feedback will be displayed")
-    @example(task="copy python files from local directory to the BLOB store area associated with workspace 'curious'", text="xt upload *.py . --work=curious")
-    @example(task="copy the local file 'single_sweeps.txt' as 'sweeps.txt' in the BLOB store area for job2998", text="xt upload single_sweeps.txt sweeps.txt  --job=job2998")
-    @example(task="copy MNIST data from local dir to data upload folder name 'my-mnist'", text="xt upload c:/mnist/** my-mnist --share=data")
+    @flag(name="feedback", default=True, help="when True, incremental feedback will be displayed")
+    @example(task="copy python files from local directory to the BLOB store area associated with workspace 'curious'", text="xt upload *.py . --share=data --work=curious")
+    @example(task="copy the local file 'single_sweeps.txt' as 'sweeps.txt' in the BLOB store area for job2998", text="xt upload single_sweeps.txt sweeps.txt --share=data --job=job2998")
+    @example(task="copy MNIST data from local dir to data upload folder name 'my-mnist'", text="xt upload ./mnist/** my-mnist --share=data")
     @command(help="copy local files to an Azure storage location")
     def upload(self, local_path, store_path, share, workspace, experiment, job, run, feedback):
-
-        use_blobs = True
-        use_multi = True
-        upload_count = 0
-
-        # exapnd ~/ in front of local path
-        local_path = os.path.expanduser(local_path)
-
-        if os.path.exists(local_path) and os.path.isfile(local_path):
-            use_multi = False
-
-        #console.print("local_path=", local_path)
-
-        # if directory, default to copy nested
-        if os.path.isdir(local_path):
-            local_path += "/**"
-            use_multi = True
-
-        if not store_path or store_path == ".":
-            if not use_multi:
-                # single file defaults to the base name of the local file
-                store_path = os.path.basename(local_path)
-            else:
-                store_path = "."
-
-        fs = self.create_file_accessor(use_blobs, share, workspace, experiment, job, run)
-        uri = fs.get_uri(store_path)
-        actual_path, _ = file_utils.split_wc_path(local_path)
-
-        actual_path = file_utils.relative_path(actual_path)
-        actual_path = file_utils.fix_slashes(actual_path)
-
-        if not os.path.exists(actual_path):
-            errors.env_error("Cannot find the local file/folder: {}".format(actual_path))
-
-        feedback_progress = FeedbackProgress(feedback, not self.capture_output)
-        progress_callback = feedback_progress.progress if feedback else None
-
-        if use_multi:
-            # upload MULTIPLE files/blobs
-            file_names, local_path = file_utils.get_local_filenames(local_path)
-            what = "blobs" if use_blobs else "files"
-
-            if len(file_names) == 0:
-                console.print("no matching files found in: {}".format(what, actual_path))
-                return
-            elif len(file_names) == 1:
-                what = "blob" if use_blobs else "file"
-
-            console.print("\nto {}, uploading {} {}:".format(uri, len(file_names), what))
-
-            #file_utils.ensure_dir_exists(local_path)
-            max_name_len = max([len(name) for name in file_names])
-            name_width =  1 + max_name_len
-            #console.print("max_name_len=", max_name_len, ", name_width=", name_width)
-
-            for f, fn in enumerate(file_names):
-                blob_path = self.make_dest_fn(local_path, fn, store_path)
-                actual_fn = file_utils.fix_slashes(fn)
-
-                file_msg = "file {}/{}".format(1+f, len(file_names))
-                console.print("  {2:}: {1:<{0:}} ".format(name_width, actual_fn + ":", file_msg), end="", flush=True)
-
-                feedback_progress.start()
-                fs.upload_file(blob_path, actual_fn, progress_callback=progress_callback)
-                feedback_progress.end()
-
-                upload_count += 1
-        else:
-            # upload SINGLE file/blob
-            what = "blob" if use_blobs else "file"
-            console.print("\nto: {}, uploading {}:".format(uri, what))
-
-            blob_name = os.path.basename(local_path)
-            local_path = file_utils.fix_slashes(local_path)
-
-            #console.print("store_path=", store_path, ", local_path=", local_path)
-
-            console.print("  {}:    ".format(local_path), end="", flush=True)
-
-            feedback_progress.start()
-            fs.upload_file(store_path, local_path, progress_callback=progress_callback)
-            feedback_progress.end()
-
-            upload_count += 1
-
-        return upload_count
+        self.impl_storage_api.upload(local_path, store_path, share, workspace, experiment, job, run, feedback, show_output=True)
 
     #---- DOWNLOAD command ----
     @argument(name="store-path", help="the path for the source store blob or wildcard")
-    @argument(name="local-path", required=False,help="the path for the destination file or directory")
+    @argument(name="local-path", required=False, help="the path for the destination file (if downloading a single file) or directory (if downloading multiple files)")
     @option(name="share", help="the name of the share that the path is relative to")
     @option(name="workspace", default="$general.workspace", help="the workspace name that the path is relative to")
     @option(name="job", help="the job id that the path is relative to")
     @option(name="experiment", help="the experiment that the path is relative to")
     @option(name="run", help="the run name that the path is relative to")
-    @flag(name="feedback", help="when True, incremental feedback will be displayed")
+    @flag(name="feedback", default=True, help="when True, incremental feedback will be displayed")
     @flag(name="snapshot", help="when True, a temporary snapshot of store files will be used for their download")
-    @example(task="download all blobs in the 'myrecent' folder (and its children) of the BLOB store area for job2998 to local directory c:\zip", text="xt download myrecent/** c:\zip --job=job2998")
+    @example(task="download all blobs in the 'myrecent' folder (and its children) of the BLOB store area for job2998 to local directory ./zip", text="xt download myrecent/** ./zip --job=job2998")
     @command(help="copy Azure store blobs to local files/directory")
     def download(self, store_path, local_path, share, workspace, experiment, job, run, feedback, snapshot):
-        use_blobs = True 
-        use_multi = True     # default until we test if store_path exists as a file/blob
-        download_count = 0
-
-        #console.print("store_path=", store_path)
-
-        # if self.is_aml_ws(workspace): 
-        #     run_name = run
-        #     if not run_name:
-        #         errors.user_error("must specify --run=name option for azure ml workspaces")
-
-        #     self.azure_ml.download_run_files(workspace, run_name, store_path, local_path)
-        #     return
-
-        fs = self.create_file_accessor(use_blobs, share, workspace, experiment, job, run)
-
-        # test for existance of store_path as a blob/file
-        if not "*" in store_path and not "?" in store_path:
-            if fs.does_file_exist(store_path):
-                use_multi = False
-
-        if local_path:
-            # exapnd ~/ in front of local path
-            local_path = os.path.expanduser(local_path)
-        else:
-            # path not specified for local 
-            if use_multi:
-                local_path = "."
-            else:
-                local_path = "./" + os.path.basename(store_path)
-
-        uri = fs.get_uri(store_path)
-
-        # default store folder to recursive
-        if use_multi and not "*" in store_path and not "?" in store_path:
-            store_path += "/**"
-
-        use_snapshot = snapshot
-        
-        feedback_progress = FeedbackProgress(feedback, not self.capture_output)
-        progress_callback = feedback_progress.progress if feedback else None
-
-        if use_multi:
-            # download MULTI blobs/files
-
-            what = "blobs" if use_blobs else "files"
-            single_what = what[0:-1]
-
-            console.print("collecting {} names from: {}...".format(single_what, uri), end="")
-
-            _, blob_names = fs.get_filenames(store_path, full_paths=False)
-            console.print()
-
-            if len(blob_names) == 0:
-                console.print("no matching {} found in: {}".format(what, uri))
-                return 0
-            elif len(blob_names) == 1:
-                what = "blob" if use_blobs else "file"
-
-            console.print("\ndownloading {} {}...:".format(len(blob_names), what))
-
-            file_utils.ensure_dir_exists(local_path)
-            max_name_len = max([len(local_path + "/" + name) for name in blob_names])
-            name_width =  1 + max_name_len
-            #console.print("max_name_len=", max_name_len, ", name_width=", name_width)
-
-            for f, bn in enumerate(blob_names):
-                dest_fn = file_utils.fix_slashes(local_path + "/" + bn)
-
-                file_msg = "file {}/{}".format(1+f, len(blob_names))
-                console.print("  {2:}: {1:<{0:}} ".format(name_width, dest_fn + ":", file_msg), end="", flush=True)
-
-                feedback_progress.start()
-                full_bn = uri + "/" + bn if uri else bn
-                fs.download_file(full_bn, dest_fn, progress_callback=progress_callback, use_snapshot=use_snapshot)
-                feedback_progress.end()
-
-                download_count += 1
-        else:
-            # download SINGLE blobs/files
-            what = "blob" if use_blobs else "file"
-
-            if not fs.does_file_exist(store_path):
-                errors.store_error("{} not found: {}".format(what, uri))
-
-            local_path = file_utils.fix_slashes(local_path)
-            console.print("\nfrom {}, downloading {}:".format(uri, what))
-
-            console.print("  {}:    ".format(local_path), end="", flush=True)
-            feedback_progress.start()
-            fs.download_file(store_path, local_path, progress_callback=progress_callback, use_snapshot=use_snapshot)
-            feedback_progress.end()
-
-            download_count += 1
-
-        return download_count
+        self.impl_storage_api.download(store_path, local_path, share, workspace, experiment, job, run, feedback, snapshot, show_output=True)
 
     #---- LIST BLOBS command ----
     @argument(name="path", required=False, help="the path for the source store blob or wildcard")
     @option(name="share", help="the name of the share that the path is relative to")
     @option(name="workspace", default="$general.workspace", help="the workspace name that the path is relative to")
     @option(name="job", help="the job id that the path is relative to")
     @option(name="experiment", help="the experiment that the path is relative to")
@@ -1135,24 +955,15 @@
             subdirs = 0
         elif subdirs == -1:
             subdirs = True
 
         run_name = run
         use_blobs = True
 
-        # if self.is_aml_ws(workspace):
-        #     if not run_name:
-        #         errors.user_error("must specify the --run=name option for azure ML files")
-
-        #     files = self.azure_ml.get_run_files(workspace, run_name)
-        #     for file in files:
-        #         console.print(file)
-        #     return
-
-        fs = self.create_file_accessor(use_blobs, share, workspace, experiment, job, run)
+        fs = self.impl_storage_api.create_file_accessor(use_blobs, share, workspace, experiment, job, run)
 
         dd = fs.list_directories(path, subdirs)
         #console.print("dd[folders]=", dd["folders"])
 
         console.print("")
         console.print("Volume " + dd["store_name"])
 
@@ -1230,15 +1041,15 @@
         if not store_path:
             errors.syntax_error("must supply a STORE file path")
         #console.print("store_path=", store_path)
 
         # should the main dir and its child directories be removed?
         remove_dirs = store_path.endswith("**") or not "*" in store_path
 
-        fs = self.create_file_accessor(use_blobs, share, workspace, experiment, job, run)
+        fs = self.impl_storage_api.create_file_accessor(use_blobs, share, workspace, experiment, job, run)
 
         uri = fs.get_uri(store_path)
 
         if not "*" in store_path and not "?" in store_path and fs.does_file_exist(store_path):
             # special case: a named file
             fs.delete_file(store_path)
             if use_blobs:
@@ -1387,15 +1198,15 @@
 
             filter_dict["run_name"] = {"$in": run_names}
             mongo_docs = self.store.get_ws_runs(ws, filter_dict, include_log)
 
             for doc in mongo_docs:
                 #console.print("doc:")
                 self.dump_mongo_doc("\nMONGO-DB for " + full_run_name, doc, "")
-        elif name.startswith("job"):
+        elif job_helper.is_job_id(name):
             ws = job_helper.validate_job_name_with_ws(self.store, name, True)
 
             include_log = False         # can make this an option later
             job_names = [name]      # can support multiple runs later
             filter_dict = {}
 
             filter_dict["job_id"] = {"$in": job_names}
@@ -1703,15 +1514,15 @@
     @example(task="add the tag 'description' with the value 'explore effects of 5 hidden layers' to the jobs job3341 thru job3356", text="xt set tags job3341-job3356 description='explore effects of 5 hidden layers'")
     @command(help="set tags on the specified jobs or runs")
     def set_tags(self, name_list, tag_list, workspace):
         first_name = name_list[0]
         fd = self.build_tag_fd(tag_list)
         mongo = self.store.get_mongo()
 
-        if first_name.startswith("job"):
+        if job_helper.is_job_id(first_name):
             job_helper.set_job_tags(self.store, mongo, name_list, tag_list, workspace, fd, clear=False)
         elif first_name.startswith("run"):
             run_helper.set_run_tags(self.store, mongo, name_list, tag_list, workspace, fd, clear=False)
         else:
             errors.syntax_error("first name must start with 'run' or 'job', found '{}'".format(first_name))
 
     #---- CLEAR TAGS command ----
@@ -1722,15 +1533,15 @@
     @example(task="clears the tag 'description' for job3341 and job5535", text="xt clear tags job3341, job5535 description")
     @command(kwgroup="clear", help="clear tags on the specified jobs or runs")
     def clear_tags(self, name_list, tag_list, workspace):
         first_name = name_list[0]
         fd = self.build_tag_fd(tag_list)
         mongo = self.store.get_mongo()
 
-        if first_name.startswith("job"):
+        if job_helper.is_job_id(first_name):
             job_helper.set_job_tags(self.store, mongo, name_list, tag_list, workspace, fd, clear=True)
         elif first_name.startswith("run"):
             run_helper.set_run_tags(self.store, mongo, name_list, tag_list, workspace, fd, clear=True)
         else:
             errors.syntax_error("first name must start with 'run' or 'job'")
 
     #---- LIST TAGS command ----
@@ -1740,14 +1551,13 @@
     # examples, FAQs, command
     @example(task="list the tags for job3341 and job5535", text="xt list tags job3341, job5535")
     @command(kwgroup="list", help="list tags of the specified jobs or runs")
     def list_tags(self, name_list, tag_list, workspace):
         first_name = name_list[0]
         mongo = self.store.get_mongo()
 
-        if first_name.startswith("job"):
+        if job_helper.is_job_id(first_name):
             job_helper.list_job_tags(self.store, mongo, name_list, tag_list, workspace)
         elif first_name.startswith("run"):
             run_helper.list_run_tags(self.store, mongo, name_list, tag_list, workspace)
         else:
             errors.syntax_error("first name must start with 'run' or 'job'")
-
```

### Comparing `xtlib-1.0.0rc1/xtlib/impl_compute.py` & `xtlib-1.0.0rc2/xtlib/impl_compute.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,826 +1,836 @@
-#
-# Copyright (c) Microsoft Corporation.
-# Licensed under the MIT license.
-#
-# impl_compute.py: implementation of XT compute commands
-import os
-import sys
-import json
-import time
-import datetime
-import numpy as np 
-
-from xtlib.client import Client
-from xtlib.runner import Runner
-from xtlib.console import console
-from xtlib.storage.store import Store
-from xtlib.cmd_core import CmdCore
-from xtlib.impl_base import ImplBase
-from xtlib.backends import backend_aml 
-from xtlib.xt_client import XTClient
-from xtlib.helpers.scanner import Scanner
-from xtlib.qfe import inner_dispatch, get_dispatch_cmd, Dispatcher
-from xtlib.qfe import command, argument, option, flag, root, clone
-from xtlib.qfe import hidden, example, command_help, keyword_arg
-from xtlib.helpers.key_press_checker import KeyPressChecker, single_char_input
-
-from xtlib import qfe
-from xtlib import utils
-from xtlib import errors
-from xtlib import capture
-from xtlib import pc_utils
-from xtlib import constants
-from xtlib import file_utils
-from xtlib import job_helper
-from xtlib import run_helper
-from xtlib import process_utils
-from xtlib import box_information
-
-'''
-This module implements the following commands:
-
-run creation:
-     - xt <filename> <app args>                 # run file (.sh, .bat, .py) under control to xt on specified box/pool
-     - xt python <filename> <app args>          # run python on file 
-     - xt run app <app args>                    # run the app 
-     - xt docker run <args>                     # run the specified docker image 
-
-run control/information:
-     * xt start tensorboard [ <name> ]          # start tensorboard process for specified box or run
-     * xt stop tensorboard [ <name> ]           # stop tensorboard for specified box or run
-     * xt collect logs <log path> <runs>        # copy log files from specified runs (on blob store) to grok server
-
-     - xt monitor <name>                        # create a jupyter notebook to monitor an Azure ML run
-     - xt attach <name>                         # attach output of run to console (use ESC to detach)
-     - xt status                                # display the controller status on the specified box (flags: mirror, tensorboard, controller)
-     - xt rerun <name> [ <app args> ]           # rerun the specified run with optional new cmd args
-     - xt kill controller                       # terminates the controller on the specified box
-
-     - xt kill runs [ <name list> ]             # terminates the specifed runs or (--boxes, --job, --workspace)
-
-    (*) not yet completed
-'''     
-class ImplCompute(ImplBase):
-    def __init__(self, config, store=None):
-        super(ImplCompute, self).__init__()
-        self.config = config
-        self.store = store if store else Store(config=config)
-        self.client = Client(config, store, None)
-        self.core = CmdCore(self.config, self.store, self.client)
-        self.client.core = self.core
-        
-        #self.azure_ml = backend_aml.AzureML(self.core)
-
-    def is_aml_ws(self, ws_name):
-        return False  # self.azure_ml.does_ws_exist(ws_name)
-
-    def validate_and_add_defaults(self, cmd, args):
-        dispatcher = Dispatcher({}, self.config)
-        full_args = dispatcher.validate_and_add_defaults_for_cmd(cmd, args)
-
-        return full_args
-
-    #---- VIEW STATUS command ----
-    @argument(name="run-name", required=False, help="return status only for the specified run")
-
-    @option("cluster", help="the name of the cluster to be viewed")
-    @option("vc", default="all", help="the name of the virtual cluster")
-    @option("status", help="only show jobs with a matching status")
-    @option("max-finished", default=100, type=int, help="the maximum number of finished jobs to show")
-    @flag("tensorboard", help="shows the status of tensorboard processes on the box")
-    @flag("mirror", help="shows the status of mirror processes on the box")
-    @flag("monitor", help="continually monitor the status")
-    @flag("auto-start", help="when specified, the controller on the specified boxes will be started when needed")
-    @flag("queued", help="when specified, only queued runs are reported")
-    @flag("active", help="when specified, only active runs are reported")
-    @flag("completed", help="when specified, only completed runs are reported")
-    @option("escape-secs", type=int, help="how many seconds to wait before terminating the monitor loop")
-    @option("target", default="$xt-services.target", help="the name of the compute target to query for status")
-    @option("username", default="$general.username", type=str, help="the username used to filter runs")
-    @option("workspace", default="$general.workspace", type=str, help="the workspace used to filter runs")
-    @option(name="job", help="query all boxes defined for the specified job")
-    @example(task="show the status of runs on the local machine", text="xt view status")
-    @example(task="show the status of run68", text="xt view status curious/run68")
-    @command(kwgroup="view", help="displays the status of the specified compute target")
-    def view_status(self, run_name, tensorboard, mirror, target, workspace, job, monitor, escape_secs, auto_start, 
-            username, active, cluster, vc, status, max_finished, queued, completed):
-        '''The view status command is used to display status information about the XT controller process
-        running on a box (or pool of boxes).  
-        
-        The'tensorboard' flag is used to return information about the running tensorboard-related processes.
-        The 'mirror' flag is used to return information about Grok server mirroring processes.
-        '''
-
-        if tensorboard:
-            run_name = "tensorboard"
-        elif mirror:
-            run_name = "mirror"
-        elif run_name:
-            run_name, workspace = run_helper.parse_run_name(workspace, run_name)
-
-        if not queued and not active and not completed:
-            # if none of these are specified, it implies we want to see all info
-            stage_flags = "queued, active, completed"
-        else:
-            # at least one flag was specified, so logically "or" them
-            stage_flags = ""
-            if queued:
-                stage_flags += "queued, "
-            if active:
-                stage_flags += "active, "
-            if completed:
-                stage_flags += "completed, "
-
-        # active = self.config.get("general", "active")
-        # queued = self.config.get("general", "queued")
-
-        if target == "all":
-            # enumerate all registered targets and call their view_status method
-            targets = self.config.get_targets()
-
-            for target in targets:
-                print("\nSTATUS for target '{}':".format(target))
-
-                backend = self.core.create_backend(target, username=username)
-                backend.view_status(run_name, workspace, job, monitor, escape_secs, auto_start, 
-                    stage_flags, status, max_finished)
-        else:
-            # view status on a single target
-            backend = self.core.create_backend(target, username=username)
-            backend.view_status(run_name, workspace, job, monitor, escape_secs, auto_start, 
-                stage_flags, status, max_finished)
-
-    #---- MONITOR command ----
-    # other candidate names for this command: watch, attach
-    @argument(name="name", help="The name of the run or job to be monitored")
-    @option("escape", type=int, default=0, help="breaks out of attach or --monitor loop after specified # of seconds")
-    @flag("jupyter", help="to monitor a job from a jupyter notebook (AML only)")
-    @option("log-name", default=None, help="the name of the log file to be monitored")
-    @option("node-index", default=0, type=int, help="the node index for multi-node jobs")
-    @option("sleep", default=1, type=float, help="the number of seconds between download calls")
-    @option("workspace", default="$general.workspace", type=str, help="the workspace that the run resides within")
-    @example(task="monitor job3321's primary log file", text="xt monitor job3321")
-    @command(help="view a job's log file, as it grows in real-time")
-    def monitor(self, name, escape=None, jupyter=None, log_name=None, node_index=None, sleep=1, workspace=None):
-        if jupyter:
-            return self.monitor_with_jupyter(workspace, name)
-
-        if name.startswith("job"):
-            return self.monitor_job_node(name, jupyter, sleep, node_index, log_name, escape) 
-
-        if name.startswith("run"):
-            rr = run_helper.get_run_record(self.store, workspace, name)
-            job_id = rr["job_id"]
-            node_index = rr["node_index"]
-            return self.monitor_job_node(job_id, jupyter, sleep, node_index, log_name, escape) 
-
-        errors.syntax_error("name must be a job or run name: {}".format(name))
-
-    def monitor_job_node(self, job_id, jupyter, sleep, node_index, log_name, escape):
-
-        if node_index is None:
-            node_index = 0
-
-        backend, job_info = job_helper.get_job_backend(self.store, self.core, job_id)
-
-        node_id = utils.node_id(node_index)
-        service_info_by_node = job_info["service_info_by_node"]  
-        service_node_info = service_info_by_node[node_id]
-
-        service_name = backend.get_name()
-        node_count = len(job_info["service_info_by_node"])
-
-        console.print("==> monitoring: {}, node{} [{}] (press escape or control-c to exit, +/- to change node)" \
-            .format(job_id, node_index, service_name), flush=True)
-
-        # the monitoring loop
-        start_offset = 0
-        simple_status = None
-        service_status = None
-        kb_sleep = .1       # be quick to respond to user's key presses
-        sleeps_per_call = max(1, sleep//kb_sleep)
-        sleep_count = 0
-        ch = None
-        first_call = True
-        offset_by_node = {}
-        node_id = utils.node_id(node_index)
-        first_text_of_stream = True
-        display_count = 0
-        started = time.time()
-
-        try:
-            with KeyPressChecker() as checker:
-
-                while simple_status != "completed":
-                    ch = checker.getch_nowait()
-                    #print(ch, end=" ")
-
-                    if ch == constants.ESCAPE or ch == constants.CONTROL_C:
-                        break
-
-                    if ch in ["+", "-"] and node_count > 1:
-                        # save current context
-                        offset_by_node[node_id] = start_offset
-
-                        # increment node_index
-                        delta = 1 if ch == "+" else -1
-                        node_index = (delta + node_index) % node_count
-                        node_id = utils.node_id(node_index)
-
-                        # set new context
-                        service_node_info = service_info_by_node[node_id]
-                        start_offset = offset_by_node[node_id] if node_id in offset_by_node else 0
-                        first_text_of_stream = not start_offset
-                        console.print("==> switching to: node{}".format(node_index))
-
-                    if ch == "q":
-                        # diagnostic aid (undocumented, only for pool service)
-                        console.print("{} service queue:".format(node_id), flush=True)
-
-                        entries = backend.get_service_queue_entries(service_node_info)
-                        if entries is None:
-                            console.print("  <not supported for this service")
-                        else:
-                            if entries:
-                                for entry in entries:
-                                    marker = "*" if entry["current"] else " "
-                                    console.print("  {} {}".format(marker, entry["name"]))
-                            else:
-                                console.print("  <no entries>")
-
-                    if sleep_count == sleeps_per_call:
-
-                        # time to read the log file
-                        result = backend.read_log_file(service_node_info, log_name=log_name, start_offset=start_offset)
-
-                        new_text = result["new_text"]
-                        new_simple = result["simple_status"]
-                        new_service = result["service_status"]
-                        start_offset = result["next_offset"]
-                        new_log = result["log_name"]
-
-                        if new_log != log_name:
-                            log_name = new_log                
-                            console.print("==> node{} streaming log: {}".format(node_index, log_name))
-                            first_text_of_stream = True
-
-                        if new_service != service_status:
-                            service_status = new_service
-                            simple_status = new_simple
-                            console.print("==> node{} status: {} ({})".format(node_index, service_status, simple_status))
-
-                        if new_text:
-                            if node_count > 1:
-                                # prepend each new line with node_id
-                                prefix = node_id + ": "
-                                new_text = new_text.replace("\n", "\n" + prefix)
-
-                                if first_text_of_stream:
-                                    new_text = prefix + new_text
-                                    first_text_of_stream = False
-
-                            console.print(new_text, end="")
-                            display_count += 1
-
-                        first_call = False
-                        sleep_count = 0
-
-                    time.sleep(kb_sleep)
-                    sleep_count += 1
-
-                    if escape:
-                        # have we exceeded max time in monitoring?
-                        elapsed = time.time() - started
-                        if elapsed >= escape:
-                            break
-
-        except KeyboardInterrupt:
-           ch = constants.CONTROL_C
-
-        show_final_status = (display_count > 0)
-
-        if ch == constants.ESCAPE:
-            console.print("==> monitoring cancelled (escape key detected)")
-
-        elif ch == constants.CONTROL_C:
-            console.print("==> monitoring cancelled (control-c detected)")
-            ch = single_char_input("do you want to cancel the job? (y/n): ")
-            if ch == "y":
-                self.cancel_job(job_id)
-                show_final_status = False
-
-        if show_final_status:
-            console.print("==> node{} status: {} ({})".format(node_index, service_status, simple_status))
-
-    def monitor_with_jupyter(self, workspace, run_name):
-        if not self.is_aml_ws(workspace):
-            errors.combo_error("the monitor command is only supported for Azure ML runs")
-
-        run_name, actual_ws = run_helper.parse_run_name(workspace, run_name)
-
-        fn = self.azure_ml.make_monitor_notebook(actual_ws, run_name)
-        dir = os.path.dirname(fn)
-        #console.print("jupyter notebook written to: " + fn)
-        monitor_cmd = "jupyter notebook --notebook-dir=" + dir
-        console.print("monitoring notebook created; to run:")
-        console.print("  " + monitor_cmd)
-
-    #---- COLLECT LOGS command ----
-    @argument(name="run-names", type="str_list", help="comma-separated list of run names")
-    @argument(name="log_path", help="the wildcard path of the log files to collect")
-    @option("workspace", default="$general.workspace", type=str, help="the workspace that the runs reside within")
-    @example(task="collect the log files matching *tfevent* from run68", text="xt collect logs run68, run69 *tfevent* --work=curious")
-    @command(help="copy log files from specified runs (on blob store) to grok server")
-    def collect_logs(self, workspace, run_names, log_path):
-
-        run_names, actual_ws = run_helper.parse_run_list(self.store, workspace, run_names)
-        if len(run_names) == 0:
-            self.store_error("No matching runs found")
-
-        grok_server = None   # self.config.get("logging", "grok-server")
-
-        count = 0
-        for run_name in run_names:
-            count += self.core.collect_logs_for_run(actual_ws, run_name, log_path, grok_server)
-
-        console.print("{} log file collected to grok server: {}".format(count, grok_server))
-
-    #---- START TENSORBOARD command ----
-    @example(task="start tensorboard curious/run68", text="xt start tensorboard curious/run68")
-    @command(help="start tensorboard for the specified run")
-    def start_tensorboard(self):
-        console.print("start_tensorboard cmd goes here...")
-
-    #---- STOP TENSORBOARD command ----
-    @example(task="stop tensorboard curious/run68", text="xt stop tensorboard curious/run68")
-    @command(help="stop tensorboard for the specified run")
-    def stop_tensorboard(self):
-        console.print("stop_tensorboard cmd goes here...")
-
-    def get_info_for_run(self, ws, run_name):
-        cmdline = None
-        box_name = None
-        parent_name = None
-        node_index = None
-
-        records = self.store.get_run_log(ws, run_name)
-
-        # get cmdline
-        for record in records:
-            if record["event"] == "cmd":
-                dd = record["data"]
-                cmdline = dd["cmd"]
-                xt_cmdline = dd["xt_cmd"]
-                break
-
-        for record in records:
-            if record["event"] == "created":
-                dd = record["data"]
-                box_name = dd["box_name"]
-                node_index = dd["node_index"]
-                # looks like we no longer log the parent name
-                #parent_name = dd["parent_name"]
-                parent_name = run_name.split(".")[0] if "." in run_name else None
-                break
-
-        return cmdline, xt_cmdline, box_name, parent_name, node_index
-
-    #---- RERUN command ----
-    @argument("run-name", help="the name of the original run")
-    @option("workspace", default="$general.workspace", type=str, help="the workspace that the runs reside within")
-    @option("response", default=None, help="the automatic response to be used to supplement the cmd line args for the run")
-    @example(task="rerun run74", text="xt rerun curious/run74")
-    @command(help="submits a run to be run again")
-    def rerun(self, run_name, workspace, response):
-        # NOTE: validate_run_name() call must be AFTER we call process_named_options()
-        run_name, workspace = run_helper.parse_run_name(workspace, run_name)
-
-        # extract "prompt" and "args" from cmdline
-        cmdline, xt_cmdline, box_name, parent_name, node_index = self.get_info_for_run(workspace, run_name)
-
-        #console.print("cmdline=", cmdline)
-        prompt = ""
-
-        if xt_cmdline:
-            args = "  " + xt_cmdline
-        else:
-            # legacy run; just use subset of xt cmd
-            args = "  xt " + cmdline
-
-        console.print("edit/accept xt cmd for {}/{}".format(workspace, run_name))
-        if response:
-            # allow user to supplement the cmd with automation
-            if "$cmd" in response:
-                response = response.replace("$cmd", args)
-            console.print(response)
-        else:
-            response = pc_utils.input_with_default(prompt, args)
-
-        # keep RERUN cmd simple by reusing parse_python_or_run_cmd()
-        full_cmd = response.strip()
-        #console.print("  new_cmd=" + full_cmd)
-        if not full_cmd.startswith("xt "):
-            errors.syntax_error("command must start with 'xt ': {}".format(full_cmd))
-
-        tmp_dir = file_utils.make_tmp_dir("rerun_cmd")
-        job_id = self.store.get_job_id_of_run(workspace, run_name)
-        capture.download_before_files(self.store, job_id, workspace, run_name, tmp_dir, silent=True)
-         
-        # move to tmp_dir so files get captured correctly
-        prev_cwd = os.getcwd()
-        os.chdir(tmp_dir)
-
-        try:
-            # recursive invoke of QFE parser to parse command (orginal + user additions)
-            args = full_cmd.split(" ")
-            args = args[1:]    # drop the "xt" at beginning
-            inner_dispatch(args, is_rerun=True)
-        finally:
-            # change back to original dir
-            os.chdir(prev_cwd)
-
-    # #---- STOP CONTROLLER command ----
-    # @option("box", default="local", type=str, help="the name of the box")
-    # @option("pool", type=str, help="the name of the pool of boxes")
-    # @example(task="stop the controller process on the local machine", text="xt stop controller")
-    # @example(task="terminate the controller process on box 'vm10'", text="xt stop controller --box=vm10")
-    # @command(help="stops the XT controller process on the specified box")
-    # def stop_controller(self, box, pool):
-
-    #     boxes, pool_info, service_type = box_information.get_box_list(self.core, box=box, pool=pool)
-    #     #console.print("boxes=", boxes, ", is_azure_pool=", is_azure_pool)
-
-    #     self.client.cancel_controller_by_boxes(boxes)
-
-    def print_cancel_results(self, cancel_results_by_boxes, run_summary=None, is_aml=False):
-        #console.print("cancel_results_by_boxes=", cancel_results_by_boxes)
-
-        if run_summary:
-            console.print(run_summary)
-
-        if not cancel_results_by_boxes:
-            console.print("no matching runs found")
-            return
-            
-        for box_name, results in cancel_results_by_boxes.items():
-
-            # show box name as upper to emphasize where kill happened
-            box_name = box_name.upper()
-
-            if not run_summary:
-                # if is_aml:
-                #     console.print("Azure ML:")
-                # else:
-                #     console.print("box {}:".format(box_name))
-                console.print(box_name + ":")
-
-            if not results:
-                console.print("  no matching active runs found")
-            else:
-                for result in results:
-                    if not result:
-                        continue
-
-                    #console.print("result=", result)
-                    ws_name = result["workspace"]
-                    run_name = result["run_name"]
-                    exper_name = result["exper_name"] if "exper_name" in result else None
-                    killed = result["cancelled"]
-                    status = result["status"]
-                    before_status = result["before_status"]
-                        
-                    run_name = exper_name + "." + run_name if exper_name else run_name
-                    full_name = ws_name + "/" + run_name
-
-                    if killed:
-                        console.print("  {} cancelled (status was '{}')".format(full_name, before_status))
-                    else:
-                        console.print("  {} has already exited, status={}".format(full_name, status))
-
-    def print_cancel_all_results(self, cancel_results_by_boxes):
-        for target, results in cancel_results_by_boxes.items():
-            console.print("Target: {}".format(target))
-            for result in results:
-                console.print(
-                    "canceled: {}, service_status: {}, simple_status: {}".format(
-                        result.get("cancelled"),
-                        result.get("service_status"),
-                        result.get("simple_status")))
-
-    def get_runs_by_box(self, run_names, workspace=None):
-        run_names, actual_ws = run_helper.parse_run_list(self.store, workspace, run_names)
-
-        mongo = self.store.get_mongo()
-        fields_dict = {"box_name": 1, "compute": 1, "ws": 1, "run_name": 1}
-
-        filter_dict = {}
-        filter_dict["run_name"] = {"$in": run_names}
-
-        box_records = mongo.get_info_for_runs(actual_ws, filter_dict, fields_dict)
-
-        # group by box_name
-        runs_by_box = {}
-
-        for br in box_records:
-            if "box_name" in br:
-                box_name = br["box_name"] 
-                if not box_name in runs_by_box:
-                    runs_by_box[box_name] = []
-                runs_by_box[box_name].append(br)
-
-        return runs_by_box
-
-    #---- CANCEL RUN command ----
-    @argument("run-names", type="str_list", help="the list of run names to cancel")
-    @option("workspace", default="$general.workspace", type=str, help="the workspace that contains the runs")
-    @example(task="cancel run103 in curious workspace", text="xt cancel runs run103 --work=curious")
-    @command(kwgroup="cancel", help="cancels the specified run(s)")
-    def cancel_run(self, run_names, workspace):
-
-        runs_by_box = self.get_runs_by_box(run_names, workspace)
-
-        cancel_results_by_box = {}
-
-        for box_name, runs in runs_by_box.items():
-            first_run = runs[0]
-
-            ws_name = first_run["ws"]
-            # = [ws_name + "/" + run["run_name"] for run in runs]
-            run_names = [run["run_name"] for run in runs]
-            compute = first_run["compute"] if "compute" in first_run else "pool"    # some legacy support
-
-            backend = self.core.create_backend(compute)
-            cancel_results = backend.cancel_runs_by_names(workspace, run_names, box_name)
-
-            cancel_results_by_box[box_name] = cancel_results
-
-        self.print_cancel_all_results(cancel_results_by_box)
-
-    #---- CANCEL JOB command ----
-    @argument("job-id", help="the name of the job to cancel")
-    @example(task="cancel all runs in job3125", text="xt cancel job job3125")
-    @command(kwgroup="cancel", kwhelp="cancels active runs, specified by name, job, or target", help="cancels the specified job and its active or queued runs")
-    def cancel_job(self, job_id):
-
-        console.print("cancelling {}:".format(job_id))
-
-        service_job_info, service_info_by_node, backend = job_helper.get_service_job_info(self.store, self.core, job_id)
-        result_by_node = backend.cancel_job(service_job_info, service_info_by_node)
-
-        for node_id, result in result_by_node.items():
-            console.print("  {}: {}".format(node_id, result))
-
-        # wrap up runs associated with each node
-        wrapup_count = 0
-
-        for node_id, result in result_by_node.items():
-            runs = run_helper.wrapup_runs_by_node(self.store, job_id, node_id, result)
-            wrapup_count += len(runs)
-
-        console.print("  runs wrapped-up: {}".format(wrapup_count))
-
-    #---- CANCEL ALL command ----
-    @argument("target", help="the name of the compute target whose runs will be cancelled")
-    @hidden("username", default="$general.username", help="the username to log as the author of this run")
-    @example(task="cancel all runs for current user on Philly", text="xt cancel all philly")
-    @command(kwgroup="cancel", kwhelp="cancels active runs, specified by name, job, or target", help="cancels all queued/active runs on the specified compute target")
-    def cancel_all(self, target, username):
-
-        backend = self.core.create_backend(target, username)
-        cancel_results_by_box = {}
-
-        compute_info = self.config.get_compute_def(target)
-        service_name = compute_info["service"]
-
-        if service_name == "pool":
-            boxes = compute_info["boxes"]
-            for box_name in boxes:
-                cancel_results = backend.cancel_runs_by_user(box_name)
-            
-                cancel_results_by_box[box_name] = cancel_results
-        else:
-            cancel_results = backend.cancel_runs_by_user(None)
-            cancel_results_by_box[target] = cancel_results
-
-        self.print_cancel_all_results(cancel_results_by_box)
-
-    #---- RESTART CONTROLLER command ----
-    @argument("job-id", help="the name of the job whose node will be restarted")
-    @option("node-index", default=0, help="the 0-based node index to be restarted")
-    @option("delay", type=float, default=15, help="the number of seconds to delay after cancelling runs and before restarting the controller")
-    @example(task="simulate a service-level restart on job23, node 1", text="xt restart controller job23 --node=1")
-    @command(help="uses the XT controller to simulate a service-level restart on the specified job/node")
-    def restart_controller(self, job_id, node_index, delay):
-
-        result = None
-
-        # get the connection string for the job/node
-        cs_plus = job_helper.get_client_cs(self.core, job_id, node_index)
-        cs = cs_plus["cs"]
-        box_secret = cs_plus["box_secret"]
-
-        with XTClient(self.config, cs, box_secret) as xtc:
-            if xtc.connect():
-                result = xtc.restart_controller(delay)
-
-        if result:
-            console.print("controller restarted")
-        else:
-            console.print("could not connect to controller: ip={}, port={}".format(cs["ip"], cs["port"]))
-
-    #---- VIEW CONTROLLER STATUS command ----
-    @argument("job-id", help="the name of the job whose node will be restarted")
-    @option("node-index", default=0, help="the 0-based node index to be restarted")
-    @example(task="view the status of the 2nd node running job100", text="xt view controller status job100 --node=1")
-    @command(kwgroup="view", help="uses the XT controller to view the status of the specified job/node")
-    def view_controller_status(self, job_id, node_index):
-
-        # get the connection string for the job/node
-        cs_plus = job_helper.get_client_cs(self.core, job_id, node_index)
-        cs = cs_plus["cs"]
-        box_secret = cs_plus["box_secret"]
-        
-        job = cs_plus["job"]
-        compute = job["compute"]
-
-        if not cs:
-            console.print("could not find controller for job={}".format(job_id))
-        else:
-            stage_flags="queued, active, completed"
-
-            with XTClient(self.config, cs, box_secret) as xtc:
-                if xtc.connect():
-                    elapsed = xtc.get_controller_elapsed()
-                    xt_version = xtc.get_controller_xt_version()
-                    max_runs = xtc.get_controller_concurrent()
-                    ip_addr = xtc.get_controller_ip_addr()
-                    status_text = xtc.get_runs(stage_flags)
-
-                    elapsed = str(datetime.timedelta(seconds=elapsed))
-                    elapsed = elapsed.split(".")[0]   # get rid of decimal digits at end
-
-                    box_name = cs["box_name"]
-                    indent = "  "
-                    cname = "localhost" if box_name=="local" else box_name
-
-                    fmt_str = "XT controller:\n" + \
-                        indent + "{}:{}, {}, SSL, xtlib: {}\n" + \
-                        indent + "IP: {}:{}, running time: {}, max-runs: {}"
-                        
-                    text = fmt_str.format(job_id, cname, compute, xt_version, ip_addr, cs["port"], elapsed, max_runs)
-
-                    text +=  "\n\n" + stage_flags + " runs on " + box_name.upper() + ":\n"
-            
-                    report = self.core.build_jobs_report(status_text)
-
-                    console.print(text)
-                    console.print(report)
-                else:
-                    console.print("could not connect to controller")
-
-    #---- VIEW CONTROLLER LOG command ----
-    @argument("job-id", help="the name of the job whose node will be restarted")
-    @option("node-index", default=0, help="the 0-based node index to be restarted")
-    @example(task="view the conntroller log for single node job100", text="xt view controller status job100")
-    @command(kwgroup="view", kwhelp="view information about a node using the XT controller", help="uses the XT controller to view it's log on the specified job/node")
-    def view_controller_log(self, job_id, node_index):
-
-        result = None
-
-        # get the connection string for the job/node
-        cs_plus = job_helper.get_client_cs(self.core, job_id, node_index)
-        cs = cs_plus["cs"]
-        box_secret = cs_plus["box_secret"]
-        stage_flags="queued, active, completed"
-
-        with XTClient(self.config, cs, box_secret) as xtc:
-            if xtc.connect():
-                text = xtc.get_controller_log()
-
-                box = cs["box_name"]
-                console.print("box={}, controller log:".format(box.upper()))
-                console.print(text)
-            else:
-                console.print("could not connect to controller")
-
-    #---- RUN command ----
-    @argument("script", required=True, type=str, help="the name of the script to run")
-    @argument("script-args", required=False, type="text", help="the command line arguments for the script")
-
-    # visible and hidden options (currently=71 total, 41 visible)
-    @hidden("aggregate-dest", default="$hyperparameter-search.aggregate-dest", help="where hyperparameter searches should be aggregated for HX ('job' or 'experiment')")
-    @hidden("after-dirs", default="$after-files.after-dirs", help="the files and directories to upload after the run completes")
-    @hidden("after-omit", default="$after-files.after-omit", help="the files and directories to omit from after uploading")
-    @flag("after-upload", default="$after-files.after-upload", help="when true, the after files are upload when the run completes")
-    @hidden("option-prefix", default="$hyperparameter-search.option-prefix", help="the prefix to be used for specifying hyperparameter options to the script")
-    @option("cluster", help="the name of the Philly cluster to be used")
-    @hidden("code-dirs", default="$code.code-dirs", help="paths to the main code directory and dependent directories")
-    @hidden("code-omit", default="$code.code-omit", help="the list wildcard patterns to omit uploading from the code files")
-    @flag("code-upload", default="$code.code-upload", help="when true, code is uploaded to job and download for each run of job")
-    @hidden("code-zip", default="$code.code-zip", type=str, help="the type zip file to create for the CODE files: none/fast/compress")
-    @option("concurrent", default="$hyperparameter-search.concurrent", type=int, help="the maximum concurrent runs to be allowed on each node")
-    @option("data-action", default="$data.data-action", help="the data action to take on the target, before run is started")
-    @hidden("data-local", default="$data.data-local", help="the path on the local machine specifying where the data for this job resides")
-    @hidden("data-omit", default="$data.data-omit", help="the list wildcard patterns to omit uploading from the data files")
-    @hidden("data-share-path", default="$data.data-share-path", help="the path on the data share where data for this run will be stored")
-    @flag("data-upload", default="$data.data-upload", help="when true, the data for this job will be automatically upload when the job is submitted")
-    @flag("data-writable", default="$data.data-writable", help="when true, a mounted data path can be written to")
-    @hidden("delay-evaluation", default="$early-stopping.delay-evaluation", type=int, help="number of evals (metric loggings) to wait before applying early stopping policy")
-    @option("description", help="your description of this run")
-    @flag("direct-run", default="$general.direct-run", help="when True, the script is run without the controller (on Philly or AML)")
-    @flag("distributed", default="$general.distributed", help="when True, the multiple nodes will be put into distributed training mode")
-    @hidden("distributed-training", default="$aml-options.distributed-training", help="the name of the backend process to use for distributed training")
-    @option("docker", help="the docker entry to use with the target (from one of the entries in the config file [dockers] section")
-    @flag("dry-run", help="when True, the planned runs are displayed but not submitted")
-    @hidden("early-policy", default="$early-stopping.early-policy", help="the name of the early-stopping policy to use (bandit, median, truncation, none)")
-    @option("escape", type=int, default=0, help="breaks out of attach or --monitor loop after specified # of seconds")
-    @hidden("env-vars", default="$general.env-vars", help="the environment variable to be passed to the run when it is launched")
-    @hidden("evaluation-interval", default="$early-stopping.evaluation-interval", type=int, help="the frequencency (# of metric logs) for testing the policy")
-    @option("experiment", default="$general.experiment", type=str, help="the name of the experiment to create this run under")
-    @flag("fake-submit", help="when True, we skip creation of job and runs and the submit (used for internal testing)")
-    @hidden("fn_generated_config", default="$hyperparameter-search.fn-generated-config", type=str, help="the name for the generated HP config file")
-    @hidden("framework", default="$aml-options.framework", help="the name of the framework to be installed for the run (pytorch, tensorflow, chainer)")
-    @hidden("fw-version", default="$aml-options.fw-version", help="the framework version number")
-    #@hidden("grok-server", default="$logging.grok-server", help="the ip address of the grok-server to be used for mirroring")
-    @flag("hold", help="when True, the Azure Pool (VM's) are held open for debugging)")
-    @option("hp-config", default="$hyperparameter-search.hp-config", type=str, help="the path of the hyperparameter config file")
-    @hidden("log", default="$logging.log", help="specifes if run-related events should be logged")
-    @option("low-pri", type=bool, help="when true, use low-priority (preemptable) nodes for this job")
-    @option("max-minutes", default="$hyperparameter-search.max-minutes", type=int, help="the maximum number of minutes the run can execute before being terminated")
-    @hidden("max-seconds", type=int, default="$aml-options.max-seconds", help="the maximum number of seconds this run will execute before being terminated")
-    @option("max-runs", default="$hyperparameter-search.max-runs", type=int, help="the total number of runs across all nodes (for hyperparameter searches)")
-    @hidden("maximize-metric", default="$general.maximize-metric", help="whether to minimize or maximize value of primary metric")
-    @hidden("mirror-dest", default="$logging.mirror-dest", help="the location where mirrored information is store (none, storage, grok)")
-    @hidden("mirror-files", default="$logging.mirror-files", help="the wildcard path that specifies files to be mirrored")
-    @option("model-action", default="$model.model-action", help="the model action to take on the target, before run is started")
-    @hidden("model-local", default="$model.model-local", help="the path on the local machine specifying where the model for this job resides")
-    @hidden("model-share-path", default="$model.model-share-path", help="the model share name for the model")
-    @flag("model-writable", default="$model.model-writable", help="when true, a mounted model path can be written to")
-    @flag("jupyter-monitor", help="when True, a Jupyter notebook is created to monitor the run")
-    @option("monitor", default="$general.monitor", values=["new", "same", "none"], help="how to monitor primary run of the new job")
-    @flag("multi-commands"   , help="the script file contains multiple run commands (one per line)")
-    @option("nodes", type=int, help="the number of normal (non-preemptable) nodes to allocte for this run")
-    @option("parent-script", type=str, help="path of script used to initialize the target for repeated runs of primary script")
-    @hidden("pip-freeze", default="$internal.pip-freeze", help="when true, installed pip packges are included in the setup log")
-    @hidden("primary-metric", default="$general.primary-metric", help="the name of the metric to use for hyperparameter searching")
-    @option("queue", type=str, help="the name of the Philly queue to use when submitting this job")
-    #@option("repeat", type=int, help="the number of times to repeat the run, on each node")
-    @hidden("remote-control", default="$general.remote-control", help="specifies if XT controller will listen for XT client commands")
-    @hidden("report-rollup", default="$run-reports.report-rollup", help="whether to rollup metrics by primary metric or just use last reported metric set")
-    @option("resume-name", help="when resuming a run, this names the previous run")
-    @option("runs", default=None, type=int, help="the total number of runs across all nodes (for hyperparameter searches)")
-    @option("schedule", default="static", values=["static", "dynamic"], help="specifies if runs are pre-assigned to each node or allocate on demand")
-    @option("search-type", values=["random", "grid", "bayesian", "dgd"], default="$hyperparameter-search.search-type", help="the type of hyperparameter search to perform")
-    @option("seed", default=None, help="the random number seed that can be used for reproducible HP searches")
-    @option("sku", help="the name of the Philly SKU to be used (e.g, 'G1')")
-    @hidden("slack-factor", default="$early-stopping.slack-factor", type=float, help="(bandit only) specified as a ratio, the delta between this eval and the best performing eval")
-    @hidden("slack-amount", default="$early-stopping.slack-amount", type=float, help="(bandit only) specified as an amount, the delta between this eval and the best performing eval")
-    @hidden("storage", default="$xt-services.storage", help="name of storage service to be used for this run")
-    @option("submit-logs", default=None, help="specifies a directory to which log files for the submit are saved")
-    @option("target", default="$xt-services.target", help="one of the user-defined compute targets on which to run")
-    @hidden("truncation-percentage", default="$early-stopping.truncation-percentage", type=float, help="(truncation only) percent of runs to cancel at each eval interval")
-    @option("use-gpu", type=bool, default="$aml-options.use-gpu", help="when True, the gpu(s) on the nodes will be used by the run")
-    @option("username", default="$general.username", help="the username to log as the author of this run")
-    @hidden("user-managed", type=bool, default="$aml-options.user-managed", help="if true, it implies that the local machine or VM will be managed by the user")
-    @option("vc", help="the name of the Philly virtual cluster to be used")
-    @option("vm-size", help="the type of Azure VM computer to run on")
-    @hidden("working-dir", default="$code.working-dir", type=str, help="the run's working directory, relative to the code directory")
-    @option("workspace", default="$general.workspace", type=str, help="the workspace to create and manage the run")
-    @flag("xtlib-upload", default="$code.xtlib-upload", help="when True, local source code for xtlib is included in the source code snapshot ")
-    
-    @example(task="run the script miniMnist.py", text="xt run miniMnist.py")
-    @example(task="run the linux command 'sleep3d' on philly", text="xt run --target=philly --code-upload=0 sleep 3d")
-    @command(options_before_args=True, keyword_optional=False, pass_by_args=True, help="submits a script or executable file for running on the specified compute target")
-    def run(self, args):
-        '''
-        The run command is used to run a program, python script, batch file, or shell script on 
-        one of following compute services:
-
-        - local (the local machine)
-        - pool (a specified set of computers managed by the user)
-        - Azure Batch
-        - Azure ML
-        - Philly
-        '''
-        #console.diag("run_cmd")
-
-        # add xt cmd to args
-        cmd = get_dispatch_cmd()
-        args["xt_cmd"] = "xt " + cmd if cmd else ""
-
-        runner = Runner(self.config, self.core)
-
-        cmds, run_specs, using_hp, using_aml_hparam, sweeps_text, pool_info, job_id = \
-            runner.process_run_command(args)
-
-        monitor = args["monitor"]
-        escape = args["escape"]
-
-        if monitor == "same":
-            workspace = args["workspace"]
-            self.monitor(name=job_id, workspace=workspace, escape=escape)
-
-        elif monitor == "new":
-            cmd = "xt --echo monitor {}".format(job_id)
-            process_utils.run_cmd_in_new_console(cmd)
-
+#
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT license.
+#
+# impl_compute.py: implementation of XT compute commands
+import os
+import sys
+import json
+import time
+import datetime
+import tempfile
+import pprint
+import numpy as np 
+
+from xtlib.client import Client
+from xtlib.runner import Runner
+from xtlib.console import console
+from xtlib.storage.store import Store
+from xtlib.cmd_core import CmdCore
+from xtlib.impl_base import ImplBase
+from xtlib.backends import backend_aml 
+from xtlib.xt_client import XTClient
+from xtlib.helpers.scanner import Scanner
+from xtlib.qfe import inner_dispatch, get_dispatch_cmd, Dispatcher
+from xtlib.qfe import command, argument, option, flag, root, clone
+from xtlib.qfe import hidden, example, command_help, keyword_arg
+from xtlib.helpers.key_press_checker import KeyPressChecker, single_char_input
+
+from xtlib import qfe
+from xtlib import utils
+from xtlib import errors
+from xtlib import capture
+from xtlib import pc_utils
+from xtlib import constants
+from xtlib import file_utils
+from xtlib import job_helper
+from xtlib import run_helper
+from xtlib import process_utils
+from xtlib import box_information
+
+'''
+This module implements the following commands:
+
+run creation:
+     - xt <filename> <app args>                 # run file (.sh, .bat, .py) under control to xt on specified box/pool
+     - xt python <filename> <app args>          # run python on file 
+     - xt run app <app args>                    # run the app 
+     - xt docker run <args>                     # run the specified docker image 
+
+run control/information:
+     * xt start tensorboard [ <name> ]          # start tensorboard process for specified box or run
+     * xt stop tensorboard [ <name> ]           # stop tensorboard for specified box or run
+     * xt collect logs <log path> <runs>        # copy log files from specified runs (on blob store) to grok server
+
+     - xt monitor <name>                        # create a jupyter notebook to monitor an Azure ML run
+     - xt attach <name>                         # attach output of run to console (use ESC to detach)
+     - xt status                                # display the controller status on the specified box (flags: mirror, tensorboard, controller)
+     - xt rerun <name> [ <app args> ]           # rerun the specified run with optional new cmd args
+     - xt kill controller                       # terminates the controller on the specified box
+
+     - xt kill runs [ <name list> ]             # terminates the specifed runs or (--boxes, --job, --workspace)
+
+    (*) not yet completed
+'''     
+class ImplCompute(ImplBase):
+    def __init__(self, config, store=None):
+        super(ImplCompute, self).__init__()
+        self.config = config
+        self.store = store if store else Store(config=config)
+        self.client = Client(config, store, None)
+        self.core = CmdCore(self.config, self.store, self.client)
+        self.client.core = self.core
+        
+        #self.azure_ml = backend_aml.AzureML(self.core)
+
+    def is_aml_ws(self, ws_name):
+        return False  # self.azure_ml.does_ws_exist(ws_name)
+
+    def validate_and_add_defaults(self, cmd, args):
+        dispatcher = Dispatcher({}, self.config)
+        full_args = dispatcher.validate_and_add_defaults_for_cmd(cmd, args)
+
+        return full_args
+
+    #---- VIEW STATUS command ----
+    @argument(name="run-name", required=False, help="return status only for the specified run")
+
+    @option("cluster", help="the name of the cluster to be viewed")
+    @option("vc", default="all", help="the name of the virtual cluster")
+    @option("status", help="only show jobs with a matching status")
+    @option("max-finished", default=100, type=int, help="the maximum number of finished jobs to show")
+    @flag("tensorboard", help="shows the status of tensorboard processes on the box")
+    @flag("mirror", help="shows the status of mirror processes on the box")
+    @flag("monitor", help="continually monitor the status")
+    @flag("auto-start", help="when specified, the controller on the specified boxes will be started when needed")
+    @flag("queued", help="when specified, only queued runs are reported")
+    @flag("active", help="when specified, only active runs are reported")
+    @flag("completed", help="when specified, only completed runs are reported")
+    @option("escape-secs", type=int, help="how many seconds to wait before terminating the monitor loop")
+    @option("target", default="$xt-services.target", help="the name of the compute target to query for status")
+    @option("username", default="$general.username", type=str, help="the username used to filter runs")
+    @option("workspace", default="$general.workspace", type=str, help="the workspace used to filter runs")
+    @option(name="job", help="query all boxes defined for the specified job")
+    @example(task="show the status of runs on the local machine", text="xt view status")
+    @example(task="show the status of run68", text="xt view status curious/run68")
+    @command(kwgroup="view", help="displays the status of the specified compute target")
+    def view_status(self, run_name, tensorboard, mirror, target, workspace, job, monitor, escape_secs, auto_start, 
+            username, active, cluster, vc, status, max_finished, queued, completed):
+        '''The view status command is used to display status information about the XT controller process
+        running on a box (or pool of boxes).  
+        
+        The'tensorboard' flag is used to return information about the running tensorboard-related processes.
+        The 'mirror' flag is used to return information about Grok server mirroring processes.
+        '''
+
+        if tensorboard:
+            run_name = "tensorboard"
+        elif mirror:
+            run_name = "mirror"
+        elif run_name:
+            run_name, workspace = run_helper.parse_run_name(workspace, run_name)
+
+        if not queued and not active and not completed:
+            # if none of these are specified, it implies we want to see all info
+            stage_flags = "queued, active, completed"
+        else:
+            # at least one flag was specified, so logically "or" them
+            stage_flags = ""
+            if queued:
+                stage_flags += "queued, "
+            if active:
+                stage_flags += "active, "
+            if completed:
+                stage_flags += "completed, "
+
+        # active = self.config.get("general", "active")
+        # queued = self.config.get("general", "queued")
+        results = []
+
+        if target == "all":
+            # enumerate all registered targets and call their view_status method
+            targets = self.config.get_targets()
+
+            for target in targets:
+                print("\nSTATUS for target '{}':".format(target))
+
+                backend = self.core.create_backend(target, username=username)
+                results = backend.view_status(run_name, workspace, job, monitor, escape_secs, auto_start, 
+                    stage_flags, status, max_finished)
+        else:
+            # view status on a single target
+            backend = self.core.create_backend(target, username=username)
+            results = backend.view_status(run_name, workspace, job, monitor, escape_secs, auto_start, 
+                stage_flags, status, max_finished)
+
+        if results is not None:
+            for result in results:
+                pprint.pprint(result)
+
+    #---- MONITOR command ----
+    # other candidate names for this command: watch, attach
+    @argument(name="name", help="The name of the run or job to be monitored")
+    @option("escape", type=int, default=0, help="breaks out of attach or --monitor loop after specified # of seconds")
+    @flag("jupyter", help="to monitor a job from a jupyter notebook (AML only)")
+    @option("log-name", default=None, help="the name of the log file to be monitored")
+    @option("node-index", default=0, type=int, help="the node index for multi-node jobs")
+    @option("sleep", default=1, type=float, help="the number of seconds between download calls")
+    @option("workspace", default="$general.workspace", type=str, help="the workspace that the run resides within")
+    @example(task="monitor job3321's primary log file", text="xt monitor job3321")
+    @command(help="view a job's log file, as it grows in real-time")
+    def monitor(self, name, escape=None, jupyter=None, log_name=None, node_index=None, sleep=1, workspace=None):
+        if jupyter:
+            return self.monitor_with_jupyter(workspace, name)
+
+        if job_helper.is_job_id(name):
+            return self.monitor_job_node(name, jupyter, sleep, node_index, log_name, escape) 
+
+        if name.startswith("run"):
+            rr = run_helper.get_run_record(self.store, workspace, name)
+            job_id = rr["job_id"]
+            node_index = rr["node_index"]
+            return self.monitor_job_node(job_id, jupyter, sleep, node_index, log_name, escape) 
+
+        errors.syntax_error("name must be a job or run name: {}".format(name))
+
+    def monitor_job_node(self, job_id, jupyter, sleep, node_index, log_name, escape):
+
+        if node_index is None:
+            node_index = 0
+
+        backend, job_info = job_helper.get_job_backend(self.store, self.core, job_id)
+
+        node_id = utils.node_id(node_index)
+        service_info_by_node = job_info["service_info_by_node"]  
+        service_node_info = service_info_by_node[node_id]
+
+        service_name = backend.get_name()
+        node_count = len(job_info["service_info_by_node"])
+
+        console.print("==> monitoring: {}, node{} [{}] (press escape or control-c to exit, +/- to change node)" \
+            .format(job_id, node_index, service_name), flush=True)
+
+        # the monitoring loop
+        start_offset = 0
+        simple_status = None
+        service_status = None
+        kb_sleep = .1       # be quick to respond to user's key presses
+        sleeps_per_call = max(1, sleep//kb_sleep)
+        sleep_count = 0
+        ch = None
+        first_call = True
+        offset_by_node = {}
+        node_id = utils.node_id(node_index)
+        first_text_of_stream = True
+        display_count = 0
+        started = time.time()
+
+        try:
+            with KeyPressChecker() as checker:
+
+                while simple_status != "completed":
+                    ch = checker.getch_nowait()
+                    #print(ch, end=" ")
+
+                    if ch == constants.ESCAPE or ch == constants.CONTROL_C:
+                        break
+
+                    if ch in ["+", "-"] and node_count > 1:
+                        # save current context
+                        offset_by_node[node_id] = start_offset
+
+                        # increment node_index
+                        delta = 1 if ch == "+" else -1
+                        node_index = (delta + node_index) % node_count
+                        node_id = utils.node_id(node_index)
+
+                        # set new context
+                        service_node_info = service_info_by_node[node_id]
+                        start_offset = offset_by_node[node_id] if node_id in offset_by_node else 0
+                        first_text_of_stream = not start_offset
+                        console.print("==> switching to: node{}".format(node_index))
+
+                    if ch == "q":
+                        # diagnostic aid (undocumented, only for pool service)
+                        console.print("{} service queue:".format(node_id), flush=True)
+
+                        entries = backend.get_service_queue_entries(service_node_info)
+                        if entries is None:
+                            console.print("  <not supported for this service")
+                        else:
+                            if entries:
+                                for entry in entries:
+                                    marker = "*" if entry["current"] else " "
+                                    console.print("  {} {}".format(marker, entry["name"]))
+                            else:
+                                console.print("  <no entries>")
+
+                    if sleep_count == sleeps_per_call:
+
+                        # time to read the log file
+                        result = backend.read_log_file(service_node_info, log_name=log_name, start_offset=start_offset)
+
+                        new_text = result["new_text"]
+                        new_simple = result["simple_status"]
+                        new_service = result["service_status"]
+                        start_offset = result["next_offset"]
+                        new_log = result["log_name"]
+
+                        if new_log != log_name:
+                            log_name = new_log                
+                            console.print("==> node{} streaming log: {}".format(node_index, log_name))
+                            first_text_of_stream = True
+
+                        if new_service != service_status:
+                            service_status = new_service
+                            simple_status = new_simple
+                            console.print("==> node{} status: {} ({})".format(node_index, service_status, simple_status))
+
+                        if new_text:
+                            if node_count > 1:
+                                # prepend each new line with node_id
+                                prefix = node_id + ": "
+                                new_text = new_text.replace("\n", "\n" + prefix)
+
+                                if first_text_of_stream:
+                                    new_text = prefix + new_text
+                                    first_text_of_stream = False
+
+                            console.print(new_text, end="")
+                            display_count += 1
+
+                        first_call = False
+                        sleep_count = 0
+
+                    time.sleep(kb_sleep)
+                    sleep_count += 1
+
+                    if escape:
+                        # have we exceeded max time in monitoring?
+                        elapsed = time.time() - started
+                        if elapsed >= escape:
+                            break
+
+        except KeyboardInterrupt:
+           ch = constants.CONTROL_C
+
+        show_final_status = (display_count > 0)
+
+        if ch == constants.ESCAPE:
+            console.print("==> monitoring cancelled (escape key detected)")
+
+        elif ch == constants.CONTROL_C:
+            console.print("==> monitoring cancelled (control-c detected)")
+            ch = single_char_input("do you want to cancel the job? (y/n): ")
+            if ch == "y":
+                self.cancel_job(job_id)
+                show_final_status = False
+
+        if show_final_status:
+            console.print("==> node{} status: {} ({})".format(node_index, service_status, simple_status))
+
+    def monitor_with_jupyter(self, workspace, run_name):
+        if not self.is_aml_ws(workspace):
+            errors.combo_error("the monitor command is only supported for Azure ML runs")
+
+        run_name, actual_ws = run_helper.parse_run_name(workspace, run_name)
+
+        fn = self.azure_ml.make_monitor_notebook(actual_ws, run_name)
+        dir = os.path.dirname(fn)
+        #console.print("jupyter notebook written to: " + fn)
+        monitor_cmd = "jupyter notebook --notebook-dir=" + dir
+        console.print("monitoring notebook created; to run:")
+        console.print("  " + monitor_cmd)
+
+    #---- COLLECT LOGS command ----
+    @argument(name="run-names", type="str_list", help="comma-separated list of run names")
+    @argument(name="log_path", help="the wildcard path of the log files to collect")
+    @option("workspace", default="$general.workspace", type=str, help="the workspace that the runs reside within")
+    @example(task="collect the log files matching *tfevent* from run68", text="xt collect logs run68, run69 *tfevent* --work=curious")
+    @command(help="copy log files from specified runs (on blob store) to grok server")
+    def collect_logs(self, workspace, run_names, log_path):
+
+        run_names, actual_ws = run_helper.parse_run_list(self.store, workspace, run_names)
+        if len(run_names) == 0:
+            self.store_error("No matching runs found")
+
+        grok_server = None   # self.config.get("logging", "grok-server")
+
+        count = 0
+        for run_name in run_names:
+            count += self.core.collect_logs_for_run(actual_ws, run_name, log_path, grok_server)
+
+        console.print("{} log file collected to grok server: {}".format(count, grok_server))
+
+    #---- START TENSORBOARD command ----
+    @example(task="start tensorboard curious/run68", text="xt start tensorboard curious/run68")
+    @command(help="start tensorboard for the specified run")
+    def start_tensorboard(self):
+        console.print("start_tensorboard cmd goes here...")
+
+    #---- STOP TENSORBOARD command ----
+    @example(task="stop tensorboard curious/run68", text="xt stop tensorboard curious/run68")
+    @command(help="stop tensorboard for the specified run")
+    def stop_tensorboard(self):
+        console.print("stop_tensorboard cmd goes here...")
+
+    def get_info_for_run(self, ws, run_name):
+        cmdline = None
+        box_name = None
+        parent_name = None
+        node_index = None
+
+        records = self.store.get_run_log(ws, run_name)
+
+        # get cmdline
+        for record in records:
+            if record["event"] == "cmd":
+                dd = record["data"]
+                cmdline = dd["cmd"]
+                xt_cmdline = dd["xt_cmd"]
+                break
+
+        for record in records:
+            if record["event"] == "created":
+                dd = record["data"]
+                box_name = dd["box_name"]
+                node_index = dd["node_index"]
+                # looks like we no longer log the parent name
+                #parent_name = dd["parent_name"]
+                parent_name = run_name.split(".")[0] if "." in run_name else None
+                break
+
+        return cmdline, xt_cmdline, box_name, parent_name, node_index
+
+    #---- RERUN command ----
+    @argument("run-name", help="the name of the original run")
+    @option("workspace", default="$general.workspace", type=str, help="the workspace that the runs reside within")
+    @option("response", default=None, help="the automatic response to be used to supplement the cmd line args for the run")
+    @example(task="rerun run74", text="xt rerun curious/run74")
+    @command(help="submits a run to be run again")
+    def rerun(self, run_name, workspace, response):
+        # NOTE: validate_run_name() call must be AFTER we call process_named_options()
+        run_name, workspace = run_helper.parse_run_name(workspace, run_name)
+
+        # extract "prompt" and "args" from cmdline
+        cmdline, xt_cmdline, box_name, parent_name, node_index = self.get_info_for_run(workspace, run_name)
+
+        #console.print("cmdline=", cmdline)
+        prompt = ""
+
+        if xt_cmdline:
+            args = "  " + xt_cmdline
+        else:
+            # legacy run; just use subset of xt cmd
+            args = "  xt " + cmdline
+
+        console.print("edit/accept xt cmd for {}/{}".format(workspace, run_name))
+        if response:
+            # allow user to supplement the cmd with automation
+            if "$cmd" in response:
+                response = response.replace("$cmd", args)
+            console.print(response)
+        else:
+            response = pc_utils.input_with_default(prompt, args)
+
+        # keep RERUN cmd simple by reusing parse_python_or_run_cmd()
+        full_cmd = response.strip()
+        #console.print("  new_cmd=" + full_cmd)
+        if not full_cmd.startswith("xt "):
+            errors.syntax_error("command must start with 'xt ': {}".format(full_cmd))
+
+        # this temp dir cannot be removed immediately after job is submitted (TBD why)
+        tmp_dir = file_utils.make_tmp_dir("rerun_cmd")
+        job_id = self.store.get_job_id_of_run(workspace, run_name)
+        capture.download_before_files(self.store, job_id, workspace, run_name, tmp_dir, 
+            silent=True, log_events=False)
+         
+        # move to tmp_dir so files get captured correctly
+        prev_cwd = os.getcwd()
+        os.chdir(tmp_dir)
+
+        try:
+            # recursive invoke of QFE parser to parse command (orginal + user additions)
+            args = full_cmd.split(" ")
+            args = args[1:]    # drop the "xt" at beginning
+            inner_dispatch(args, is_rerun=True)
+        finally:
+            # change back to original dir
+            os.chdir(prev_cwd)
+
+    # #---- STOP CONTROLLER command ----
+    # @option("box", default="local", type=str, help="the name of the box")
+    # @option("pool", type=str, help="the name of the pool of boxes")
+    # @example(task="stop the controller process on the local machine", text="xt stop controller")
+    # @example(task="terminate the controller process on box 'vm10'", text="xt stop controller --box=vm10")
+    # @command(help="stops the XT controller process on the specified box")
+    # def stop_controller(self, box, pool):
+
+    #     boxes, pool_info, service_type = box_information.get_box_list(self.core, box=box, pool=pool)
+    #     #console.print("boxes=", boxes, ", is_azure_pool=", is_azure_pool)
+
+    #     self.client.cancel_controller_by_boxes(boxes)
+
+    def print_cancel_results(self, cancel_results_by_boxes, run_summary=None, is_aml=False):
+        #console.print("cancel_results_by_boxes=", cancel_results_by_boxes)
+
+        if run_summary:
+            console.print(run_summary)
+
+        if not cancel_results_by_boxes:
+            console.print("no matching runs found")
+            return
+            
+        for box_name, results in cancel_results_by_boxes.items():
+
+            # show box name as upper to emphasize where kill happened
+            box_name = box_name.upper()
+
+            if not run_summary:
+                # if is_aml:
+                #     console.print("Azure ML:")
+                # else:
+                #     console.print("box {}:".format(box_name))
+                console.print(box_name + ":")
+
+            if not results:
+                console.print("  no matching active runs found")
+            else:
+                for result in results:
+                    if not result:
+                        continue
+
+                    #console.print("result=", result)
+                    ws_name = result["workspace"]
+                    run_name = result["run_name"]
+                    exper_name = result["exper_name"] if "exper_name" in result else None
+                    killed = result["cancelled"]
+                    status = result["status"]
+                    before_status = result["before_status"]
+                        
+                    run_name = exper_name + "." + run_name if exper_name else run_name
+                    full_name = ws_name + "/" + run_name
+
+                    if killed:
+                        console.print("  {} cancelled (status was '{}')".format(full_name, before_status))
+                    else:
+                        console.print("  {} has already exited, status={}".format(full_name, status))
+
+    def print_cancel_all_results(self, cancel_results_by_boxes):
+        for target, results in cancel_results_by_boxes.items():
+            console.print("Target: {}".format(target))
+            for result in results:
+                console.print(
+                    "canceled: {}, service_status: {}, simple_status: {}".format(
+                        result.get("cancelled"),
+                        result.get("service_status"),
+                        result.get("simple_status")))
+
+    def get_runs_by_box(self, run_names, workspace=None):
+        run_names, actual_ws = run_helper.parse_run_list(self.store, workspace, run_names)
+
+        mongo = self.store.get_mongo()
+        fields_dict = {"box_name": 1, "compute": 1, "ws": 1, "run_name": 1}
+
+        filter_dict = {}
+        filter_dict["run_name"] = {"$in": run_names}
+
+        box_records = mongo.get_info_for_runs(actual_ws, filter_dict, fields_dict)
+
+        # group by box_name
+        runs_by_box = {}
+
+        for br in box_records:
+            if "box_name" in br:
+                box_name = br["box_name"] 
+                if not box_name in runs_by_box:
+                    runs_by_box[box_name] = []
+                runs_by_box[box_name].append(br)
+
+        return runs_by_box
+
+    #---- CANCEL RUN command ----
+    @argument("run-names", type="str_list", help="the list of run names to cancel")
+    @option("workspace", default="$general.workspace", type=str, help="the workspace that contains the runs")
+    @example(task="cancel run103 in curious workspace", text="xt cancel runs run103 --work=curious")
+    @command(kwgroup="cancel", help="cancels the specified run(s)")
+    def cancel_run(self, run_names, workspace):
+
+        runs_by_box = self.get_runs_by_box(run_names, workspace)
+
+        cancel_results_by_box = {}
+
+        for box_name, runs in runs_by_box.items():
+            first_run = runs[0]
+
+            ws_name = first_run["ws"]
+            # = [ws_name + "/" + run["run_name"] for run in runs]
+            run_names = [run["run_name"] for run in runs]
+            compute = first_run["compute"] if "compute" in first_run else "pool"    # some legacy support
+
+            backend = self.core.create_backend(compute)
+            cancel_results = backend.cancel_runs_by_names(workspace, run_names, box_name)
+
+            cancel_results_by_box[box_name] = cancel_results
+
+        self.print_cancel_all_results(cancel_results_by_box)
+
+    #---- CANCEL JOB command ----
+    @argument("job-id", help="the name of the job to cancel")
+    @example(task="cancel all runs in job3125", text="xt cancel job job3125")
+    @command(kwgroup="cancel", kwhelp="cancels active runs, specified by name, job, or target", help="cancels the specified job and its active or queued runs")
+    def cancel_job(self, job_id):
+
+        console.print("cancelling {}:".format(job_id))
+
+        service_job_info, service_info_by_node, backend = job_helper.get_service_job_info(self.store, self.core, job_id)
+        result_by_node = backend.cancel_job(service_job_info, service_info_by_node)
+
+        for node_id, result in result_by_node.items():
+            console.print("  {}: {}".format(node_id, result))
+
+        # wrap up runs associated with each node
+        wrapup_count = 0
+
+        for node_id, result in result_by_node.items():
+            runs = run_helper.wrapup_runs_by_node(self.store, job_id, node_id, result)
+            wrapup_count += len(runs)
+
+        console.print("  runs wrapped-up: {}".format(wrapup_count))
+
+    #---- CANCEL ALL command ----
+    @argument("target", help="the name of the compute target whose runs will be cancelled")
+    @hidden("username", default="$general.username", help="the username to log as the author of this run")
+    @example(task="cancel all runs for current user on Philly", text="xt cancel all philly")
+    @command(kwgroup="cancel", kwhelp="cancels active runs, specified by name, job, or target", help="cancels all queued/active runs on the specified compute target")
+    def cancel_all(self, target, username):
+
+        backend = self.core.create_backend(target, username)
+        cancel_results_by_box = {}
+
+        compute_info = self.config.get_compute_def(target)
+        service_name = compute_info["service"]
+
+        if service_name == "pool":
+            boxes = compute_info["boxes"]
+            for box_name in boxes:
+                cancel_results = backend.cancel_runs_by_user(box_name)
+            
+                cancel_results_by_box[box_name] = cancel_results
+        else:
+            cancel_results = backend.cancel_runs_by_user(None)
+            cancel_results_by_box[target] = cancel_results
+
+        self.print_cancel_all_results(cancel_results_by_box)
+
+    #---- RESTART CONTROLLER command ----
+    @argument("job-id", help="the name of the job whose node will be restarted")
+    @option("node-index", default=0, help="the 0-based node index to be restarted")
+    @option("delay", type=float, default=15, help="the number of seconds to delay after cancelling runs and before restarting the controller")
+    @example(task="simulate a service-level restart on job23, node 1", text="xt restart controller job23 --node=1")
+    @command(help="uses the XT controller to simulate a service-level restart on the specified job/node")
+    def restart_controller(self, job_id, node_index, delay):
+
+        result = None
+
+        # get the connection string for the job/node
+        cs_plus = job_helper.get_client_cs(self.core, job_id, node_index)
+        cs = cs_plus["cs"]
+        box_secret = cs_plus["box_secret"]
+
+        with XTClient(self.config, cs, box_secret) as xtc:
+            if xtc.connect():
+                result = xtc.restart_controller(delay)
+
+        if result:
+            console.print("controller restarted")
+        else:
+            console.print("could not connect to controller: ip={}, port={}".format(cs["ip"], cs["port"]))
+
+    #---- VIEW CONTROLLER STATUS command ----
+    @argument("job-id", help="the name of the job whose node will be restarted")
+    @option("node-index", default=0, help="the 0-based node index to be restarted")
+    @example(task="view the status of the 2nd node running job100", text="xt view controller status job100 --node=1")
+    @command(kwgroup="view", help="uses the XT controller to view the status of the specified job/node")
+    def view_controller_status(self, job_id, node_index):
+
+        # get the connection string for the job/node
+        cs_plus = job_helper.get_client_cs(self.core, job_id, node_index)
+        cs = cs_plus["cs"]
+        box_secret = cs_plus["box_secret"]
+        
+        job = cs_plus["job"]
+        compute = job["compute"]
+
+        if not cs:
+            console.print("could not find controller for job={}".format(job_id))
+        else:
+            stage_flags="queued, active, completed"
+
+            with XTClient(self.config, cs, box_secret) as xtc:
+                if xtc.connect():
+                    elapsed = xtc.get_controller_elapsed()
+                    xt_version = xtc.get_controller_xt_version()
+                    max_runs = xtc.get_controller_concurrent()
+                    ip_addr = xtc.get_controller_ip_addr()
+                    status_text = xtc.get_runs(stage_flags)
+
+                    elapsed = str(datetime.timedelta(seconds=elapsed))
+                    elapsed = elapsed.split(".")[0]   # get rid of decimal digits at end
+
+                    box_name = cs["box_name"]
+                    indent = "  "
+                    cname = "localhost" if box_name=="local" else box_name
+
+                    fmt_str = "XT controller:\n" + \
+                        indent + "{}:{}, {}, SSL, xtlib: {}\n" + \
+                        indent + "IP: {}:{}, running time: {}, max-runs: {}"
+                        
+                    text = fmt_str.format(job_id, cname, compute, xt_version, ip_addr, cs["port"], elapsed, max_runs)
+
+                    text +=  "\n\n" + stage_flags + " runs on " + box_name.upper() + ":\n"
+            
+                    report = self.core.build_jobs_report(status_text)
+
+                    console.print(text)
+                    console.print(report)
+                else:
+                    console.print("could not connect to controller")
+
+    #---- VIEW CONTROLLER LOG command ----
+    @argument("job-id", help="the name of the job whose node will be restarted")
+    @option("node-index", default=0, help="the 0-based node index to be restarted")
+    @example(task="view the conntroller log for single node job100", text="xt view controller status job100")
+    @command(kwgroup="view", kwhelp="view information about a node using the XT controller", help="uses the XT controller to view it's log on the specified job/node")
+    def view_controller_log(self, job_id, node_index):
+
+        result = None
+
+        # get the connection string for the job/node
+        cs_plus = job_helper.get_client_cs(self.core, job_id, node_index)
+        cs = cs_plus["cs"]
+        box_secret = cs_plus["box_secret"]
+        stage_flags="queued, active, completed"
+
+        with XTClient(self.config, cs, box_secret) as xtc:
+            if xtc.connect():
+                text = xtc.get_controller_log()
+
+                box = cs["box_name"]
+                console.print("box={}, controller log:".format(box.upper()))
+                console.print(text)
+            else:
+                console.print("could not connect to controller")
+
+    #---- RUN command ----
+    @argument("script", required=True, type=str, help="the name of the script to run")
+    @argument("script-args", required=False, type="text", help="the command line arguments for the script")
+
+    # visible and hidden options (currently=71 total, 41 visible)
+    @hidden("aggregate-dest", default="$hyperparameter-search.aggregate-dest", help="where hyperparameter searches should be aggregated for HX ('job' or 'experiment')")
+    @hidden("after-dirs", default="$after-files.after-dirs", help="the files and directories to upload after the run completes")
+    @hidden("after-omit", default="$after-files.after-omit", help="the files and directories to omit from after uploading")
+    @flag("after-upload", default="$after-files.after-upload", help="when true, the after files are upload when the run completes")
+    @hidden("option-prefix", default="$hyperparameter-search.option-prefix", help="the prefix to be used for specifying hyperparameter options to the script")
+    @option("cluster", help="the name of the Philly cluster to be used")
+    @hidden("code-dirs", default="$code.code-dirs", help="paths to the main code directory and dependent directories")
+    @hidden("code-omit", default="$code.code-omit", help="the list wildcard patterns to omit uploading from the code files")
+    @flag("code-upload", default="$code.code-upload", help="when true, code is uploaded to job and download for each run of job")
+    @hidden("code-zip", default="$code.code-zip", type=str, help="the type zip file to create for the CODE files: none/fast/compress")
+    @option("concurrent", default="$hyperparameter-search.concurrent", type=int, help="the maximum concurrent runs to be allowed on each node")
+    @option("data-action", default="$data.data-action", help="the data action to take on the target, before run is started")
+    @hidden("data-local", default="$data.data-local", help="the path on the local machine specifying where the data for this job resides")
+    @hidden("data-omit", default="$data.data-omit", help="the list wildcard patterns to omit uploading from the data files")
+    @hidden("data-share-path", default="$data.data-share-path", help="the path on the data share where data for this run will be stored")
+    @flag("data-upload", default="$data.data-upload", help="when true, the data for this job will be automatically upload when the job is submitted")
+    @flag("data-writable", default="$data.data-writable", help="when true, a mounted data path can be written to")
+    @hidden("delay-evaluation", default="$early-stopping.delay-evaluation", type=int, help="number of evals (metric loggings) to wait before applying early stopping policy")
+    @option("description", help="your description of this run")
+    @flag("direct-run", default="$general.direct-run", help="when True, the script is run without the controller (on Philly or AML)")
+    @flag("distributed", default="$general.distributed", help="when True, the multiple nodes will be put into distributed training mode")
+    @hidden("distributed-training", default="$aml-options.distributed-training", help="the name of the backend process to use for distributed training")
+    @option("docker", help="the docker entry to use with the target (from one of the entries in the config file [dockers] section")
+    @flag("dry-run", help="when True, the planned runs are displayed but not submitted")
+    @hidden("early-policy", default="$early-stopping.early-policy", help="the name of the early-stopping policy to use (bandit, median, truncation, none)")
+    @option("escape", type=int, default=0, help="breaks out of attach or --monitor loop after specified # of seconds")
+    @hidden("env-vars", default="$general.env-vars", help="the environment variable to be passed to the run when it is launched")
+    @hidden("evaluation-interval", default="$early-stopping.evaluation-interval", type=int, help="the frequencency (# of metric logs) for testing the policy")
+    @option("experiment", default="$general.experiment", type=str, help="the name of the experiment to create this run under")
+    @flag("fake-submit", help="when True, we skip creation of job and runs and the submit (used for internal testing)")
+    @hidden("fn_generated_config", default="$hyperparameter-search.fn-generated-config", type=str, help="the name for the generated HP config file")
+    @hidden("framework", default="$aml-options.framework", help="the name of the framework to be installed for the run (pytorch, tensorflow, chainer)")
+    @hidden("fw-version", default="$aml-options.fw-version", help="the framework version number")
+    #@hidden("grok-server", default="$logging.grok-server", help="the ip address of the grok-server to be used for mirroring")
+    @flag("hold", help="when True, the Azure Pool (VM's) are held open for debugging)")
+    @option("hp-config", default="$hyperparameter-search.hp-config", type=str, help="the path of the hyperparameter config file")
+    @hidden("log", default="$logging.log", help="specifes if run-related events should be logged")
+    @option("low-pri", type=bool, help="when true, use low-priority (preemptable) nodes for this job")
+    @option("max-minutes", default="$hyperparameter-search.max-minutes", type=int, help="the maximum number of minutes the run can execute before being terminated")
+    @hidden("max-seconds", type=int, default="$aml-options.max-seconds", help="the maximum number of seconds this run will execute before being terminated")
+    @option("max-runs", default="$hyperparameter-search.max-runs", type=int, help="the total number of runs across all nodes (for hyperparameter searches)")
+    @hidden("maximize-metric", default="$general.maximize-metric", help="whether to minimize or maximize value of primary metric")
+    @hidden("mirror-dest", default="$logging.mirror-dest", help="the location where mirrored information is store (none, storage, grok)")
+    @hidden("mirror-files", default="$logging.mirror-files", help="the wildcard path that specifies files to be mirrored")
+    @option("model-action", default="$model.model-action", help="the model action to take on the target, before run is started")
+    @hidden("model-local", default="$model.model-local", help="the path on the local machine specifying where the model for this job resides")
+    @hidden("model-share-path", default="$model.model-share-path", help="the model share name for the model")
+    @flag("model-writable", default="$model.model-writable", help="when true, a mounted model path can be written to")
+    @flag("jupyter-monitor", help="when True, a Jupyter notebook is created to monitor the run")
+    @option("monitor", default="$general.monitor", values=["new", "same", "none"], help="how to monitor primary run of the new job")
+    @flag("multi-commands"   , help="the script file contains multiple run commands (one per line)")
+    @option("nodes", type=int, help="the number of normal (non-preemptable) nodes to allocte for this run")
+    @option("parent-script", type=str, help="path of script used to initialize the target for repeated runs of primary script")
+    @hidden("pip-freeze", default="$internal.pip-freeze", help="when true, installed pip packges are included in the setup log")
+    @hidden("primary-metric", default="$general.primary-metric", help="the name of the metric to use for hyperparameter searching")
+    @option("queue", type=str, help="the name of the Philly queue to use when submitting this job")
+    #@option("repeat", type=int, help="the number of times to repeat the run, on each node")
+    @hidden("remote-control", default="$general.remote-control", help="specifies if XT controller will listen for XT client commands")
+    @hidden("report-rollup", default="$run-reports.report-rollup", help="whether to rollup metrics by primary metric or just use last reported metric set")
+    @option("resume-name", help="when resuming a run, this names the previous run")
+    @option("runs", default=None, type=int, help="the total number of runs across all nodes (for hyperparameter searches)")
+    @option("schedule", default="static", values=["static", "dynamic"], help="specifies if runs are pre-assigned to each node or allocate on demand")
+    @option("search-type", values=["random", "grid", "bayesian", "dgd"], default="$hyperparameter-search.search-type", help="the type of hyperparameter search to perform")
+    @option("seed", default=None, help="the random number seed that can be used for reproducible HP searches")
+    @option("sku", help="the name of the Philly SKU to be used (e.g, 'G1')")
+    @hidden("slack-factor", default="$early-stopping.slack-factor", type=float, help="(bandit only) specified as a ratio, the delta between this eval and the best performing eval")
+    @hidden("slack-amount", default="$early-stopping.slack-amount", type=float, help="(bandit only) specified as an amount, the delta between this eval and the best performing eval")
+    @hidden("storage", default="$xt-services.storage", help="name of storage service to be used for this run")
+    @option("submit-logs", default=None, help="specifies a directory to which log files for the submit are saved")
+    @option("target", default="$xt-services.target", help="one of the user-defined compute targets on which to run")
+    @hidden("truncation-percentage", default="$early-stopping.truncation-percentage", type=float, help="(truncation only) percent of runs to cancel at each eval interval")
+    @option("use-gpu", type=bool, default="$aml-options.use-gpu", help="when True, the gpu(s) on the nodes will be used by the run")
+    @option("username", default="$general.username", help="the username to log as the author of this run")
+    @hidden("user-managed", type=bool, default="$aml-options.user-managed", help="if true, it implies that the local machine or VM will be managed by the user")
+    @option("vc", help="the name of the Philly virtual cluster to be used")
+    @option("vm-size", help="the type of Azure VM computer to run on")
+    @hidden("working-dir", default="$code.working-dir", type=str, help="the run's working directory, relative to the code directory")
+    @option("workspace", default="$general.workspace", type=str, help="the workspace to create and manage the run")
+    @flag("xtlib-upload", default="$code.xtlib-upload", help="when True, local source code for xtlib is included in the source code snapshot ")
+    
+    @example(task="run the script miniMnist.py", text="xt run miniMnist.py")
+    @example(task="run the linux command 'sleep3d' on philly", text="xt run --target=philly --code-upload=0 sleep 3d")
+    @command(options_before_args=True, keyword_optional=False, pass_by_args=True, help="submits a script or executable file for running on the specified compute target")
+    def run(self, args):
+        '''
+        The run command is used to run a program, python script, batch file, or shell script on 
+        one of following compute services:
+
+        - local (the local machine)
+        - pool (a specified set of computers managed by the user)
+        - Azure Batch
+        - Azure ML
+        - Philly
+        '''
+        #console.diag("run_cmd")
+
+        # add xt cmd to args
+        cmd = get_dispatch_cmd()
+        args["xt_cmd"] = "xt " + cmd if cmd else ""
+
+        with tempfile.TemporaryDirectory(prefix="import-") as temp_dir:
+            runner = Runner(self.config, self.core, temp_dir)
+
+            cmds, run_specs, using_hp, using_aml_hparam, sweeps_text, pool_info, job_id = \
+                runner.process_run_command(args)
+
+        monitor = args["monitor"]
+        escape = args["escape"]
+
+        if monitor == "same":
+            workspace = args["workspace"]
+            self.monitor(name=job_id, workspace=workspace, escape=escape)
+
+        elif monitor == "new":
+            cmd = "xt --echo monitor {}".format(job_id)
+            process_utils.run_cmd_in_new_console(cmd)
+
```

### Comparing `xtlib-1.0.0rc1/xtlib/metric_set.py` & `xtlib-1.0.0rc2/xtlib/metric_set.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/scriptor.py` & `xtlib-1.0.0rc2/xtlib/scriptor.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,22 +63,22 @@
             script = on_linux
 
         if activate_cmd:
             script.insert(1, activate_cmd)
 
     setter = "@set" if for_windows else "export"
 
-    if config.get("code", "xtlib-upload"):
-        # add PYTHONPATH for XT dev work (use latest source for XT)
-        if for_windows:
-            # assume fixed location on windows
-            script.insert(-1, "@set PYTHONPATH=c:\\github\\ExperimentTools;%PYTHONPATH%")
-        else:
-            # assume fixed location on linux
-            script.insert(-1, "export PYTHONPATH=~/ExperimentTools:$PYTHONPATH")
+    # if config.get("code", "xtlib-upload"):
+    #     # add PYTHONPATH for XT dev work (use latest source for XT)
+    #     if for_windows:
+    #         # assume fixed location on windows
+    #         script.insert(-1, "@set PYTHONPATH=c:\\github\\ExperimentTools;%PYTHONPATH%")
+    #     else:
+    #         # assume fixed location on linux
+    #         script.insert(-1, "export PYTHONPATH=~/ExperimentTools:$PYTHONPATH")
 
     # add creds so that xt controller get download xt cert
     config.create_vault_if_needed()
     vault_url = config.get_vault_url()
     script.insert(-1, "{} XT_VAULT_URL={}".format(setter, vault_url))
 
     #xt_app_pw = config.vault.get_secret("xt_app_pw", None)
```

### Comparing `xtlib-1.0.0rc1/xtlib/process_utils.py` & `xtlib-1.0.0rc2/xtlib/process_utils.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/cmd_core.py` & `xtlib-1.0.0rc2/xtlib/cmd_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
             else:
                 ip_addr = box_addr
         return ip_addr
 
     def get_runs_by_boxes_from_job(self, job_id):
         cancel_results_by_boxes = {}
 
-        if not str(job_id).startswith("job"):
+        if not job_helper.is_job_id(str(job_id)):
             errors.syntax_error("not a valid job id: " + str(job_id))
 
         #console.print("job_id=", job_id)
         text = self.store.read_job_info_file(job_id)
         job_info = json.loads(text)
         runs_by_box = job_info["runs_by_box"]
```

### Comparing `xtlib-1.0.0rc1/xtlib/cache_client.py` & `xtlib-1.0.0rc2/xtlib/cache_client.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/mirror.py` & `xtlib-1.0.0rc2/xtlib/mirror.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/backends/backend_interface.py` & `xtlib-1.0.0rc2/xtlib/backends/backend_interface.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/backends/backend_base.py` & `xtlib-1.0.0rc2/xtlib/backends/backend_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,29 +370,29 @@
             if conda:
                 cmd = cmd.replace("$current_conda_env", conda)
         
         return cmd
 
     def add_first_cmds(self, cmds, script_name, change_dir):
 
-        if not pc_utils.is_windows():
-            self.append(cmds, "#!/bin/sh")
-
         self.append(cmds, 'echo ----- START of XT-level processing -----')
         self.append(cmds, "echo running: " + script_name)
 
         self.append(cmds, 'echo initial cwd: {}'.format("%cd%" if self.is_windows else "$PWD"))
         cwd = utils.get_controller_cwd(self.is_windows, False)
         cwd = file_utils.fix_slashes(cwd, is_linux=not self.is_windows)
 
         if self.is_windows:
             self.append(cmds, 'echo 1st ARG, node_id= %1%')
             self.append(cmds, 'echo 2nd ARG, run_name= %2%')
             self.append(cmds, "mkdir {} 2>nul".format(cwd), echo_before=True)
         else:
+            # echo commands as they are executed
+            self.append(cmds, 'set -x')
+
             self.append(cmds, 'echo 1st ARG, node_id= $1')
             self.append(cmds, 'echo 2nd ARG, run_name= $2')
             self.append(cmds, "mkdir {} -p".format(cwd), echo_before=True)
 
         if change_dir:
             self.append(cmds, "cd {}".format(cwd), echo_before=True)
             self.append(cmds, 'echo after cd, cwd: {}'.format("%cd%" if self.is_windows else "$PWD"))
@@ -438,16 +438,16 @@
         self.add_xt_setup_cmds(cmds, is_windows)
         self.add_report_cmds(cmds)
 
         if username:
             self.append(cmds, "$export USER=" + username, expand=True)
 
         self.append(cmds, "-------------- Data ACTIONS -------------")
-        data_mount_dir = "c:\\xt_mnt_data" if is_windows else "/mnt/data"
-        model_mount_dir = "c:\\xt_mnt_models" if is_windows else "/mnt/models"
+        data_mount_dir = "%SystemDrive%\\xt_mnt_data" if is_windows else "/mnt/data"
+        model_mount_dir = "%SystemDrive%\\xt_mnt_models" if is_windows else "/mnt/models"
 
         # emit cmds to MOUNT run store OUTPUT path
         if not self.is_windows:
             workspace = args["workspace"]
             store_path = "runs/$2/output"   # uses RUN_NAME arg (passed to script)
 
             self.emit_mount_cmds(cmds, storage_name, storage_key, container=workspace, store_path=store_path,
```

### Comparing `xtlib-1.0.0rc1/xtlib/backends/backend_pool.py` & `xtlib-1.0.0rc2/xtlib/backends/backend_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from xtlib import errors
 from xtlib import attach
 from xtlib import pc_utils
 from xtlib import scriptor
 from xtlib import constants
 from xtlib import file_utils
 from xtlib import run_helper
+from xtlib import job_helper
 from xtlib import process_utils
 from xtlib import box_information
 from xtlib.xt_client import XTClient
 
 from xtlib.console import console
 from xtlib.helpers.feedbackParts import feedback as fb
 from xtlib.psm.local_psm_client import LocalPsmClient
@@ -354,32 +355,40 @@
 
         cs = {"ip": box_addr, "port": controller_port, "box_name": box_name}
         return cs
     
     def view_status(self, run_name, workspace, job, monitor, escape_secs, auto_start, 
             stage_flags, status, max_finished):
 
-        boxes, pool_info, service_type = box_information.get_box_list(self.core, job_id=job, pool=self.compute)
+        # boxes, pool_info, service_type = box_information.get_box_list(self.core, job_id=job, pool=self.compute)
 
-        def monitor_work():
-            # BOX LOOP
-            text = ""
-            for b, box_name in enumerate(boxes):
-                # make everyone think box_name is our current controller 
-                self.client.change_box(box_name)
-
-                if run_name in ["tensorboard", "mirror"]:
-                    text += self.get_box_process_status_inner(box_name, wworkspaces, run_name)
-                else:
-                    text += self.core.get_box_run_status_inner(box_name, workspace, run_name, stage_flags)
+        # def monitor_work():
+        #     # BOX LOOP
+        #     text = ""
+        #     for b, box_name in enumerate(boxes):
+        #         # make everyone think box_name is our current controller 
+        #         self.client.change_box(box_name)
+
+        #         if run_name in ["tensorboard", "mirror"]:
+        #             text += self.get_box_process_status_inner(box_name, wworkspaces, run_name)
+        #         else:
+        #             text += self.core.get_box_run_status_inner(box_name, workspace, run_name, stage_flags)
+
+        #     return text
+
+        # # MONITOR-ENABLED COMMAND
+        # attach.monitor_loop(monitor, monitor_work, escape_secs=escape_secs)
+        results = []
+        job_info = job_helper.get_job_record(self.core.store, "job12070")
+        service_info_by_node = job_info.get("service_info_by_node", {})
+        for _, service_node_info in service_info_by_node.items():
+            result = self.get_service_queue_entries(service_node_info)
+            results.append(result)
 
-            return text
-
-        # MONITOR-ENABLED COMMAND
-        attach.monitor_loop(monitor, monitor_work, escape_secs=escape_secs)
+        return results
 
     def cancel_runs_by_names(self, workspace, run_names, box_name):
         '''
         Args:
             workspace: the name of the workspace containing the run_names
             run_names: a list of run names
             box_name: the name of the box the runs ran on (pool service)
```

### Comparing `xtlib-1.0.0rc1/xtlib/backends/backend_aml.py` & `xtlib-1.0.0rc2/xtlib/backends/backend_aml.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/backends/backend_batch.py` & `xtlib-1.0.0rc2/xtlib/backends/backend_batch.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/xt_run.py` & `xtlib-1.0.0rc2/xtlib/xt_run.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/xtlib/xt_cmds.py` & `xtlib-1.0.0rc2/xtlib/xt_cmds.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,17 +117,17 @@
         # a dict of commands + arg/options to be surfaced (None means use all args/options)
         show_commands = {
             "cancel_all": ["target"],
             "cancel_job": ["job-id"], 
             "cancel_run": ["run-names"],
             "clear_credentials": [],
             "config_cmd": ["default", "create", "reset"],
-            "create_demo": ["destination", "response"],
+            "create_demo": ["destination", "response", "overwrite"],
             "create_services_template": [],
-            "download": ["local-path", "storage-path"],
+            "download": ["local-path", "store-path"],
             "extract": ["runs", "dest-dir", "browse", "workspace"], 
             "help": ["command", "about", "browse", "version"],
             "help_topics": ["topic", "browse"],
             "list_blobs": ["path"],
             "list_jobs": ["job-list", "experiment", "all", "first", "last", "filter", "sort", "reverse", "status", "available"],
             "list_runs": ["run-list", "job", "experiment", "all", "first", "last", "filter", "sort", "reverse", "status", "available"],
             "monitor": ["name"],
```

### Comparing `xtlib-1.0.0rc1/xtlib/plot_builder.py` & `xtlib-1.0.0rc2/xtlib/plot_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,18 @@
         for i, record in enumerate(self.run_log_records):
             # extract metrics for this run
             run = record["_id"]
             node = utils.node_id(record["node_index"])
             job = record["job_id"]
             experiment = record["exper_name"]
             workspace = record["ws"]
+            search_style = utils.safe_value(record, "search_style")
+            if search_style and search_style != "single":
+                # parent run with children - skip it
+                continue
 
             log_records = record["log_records"]
 
             metric_sets = run_helper.build_metrics_sets(log_records)
             if not metric_sets:
                 no_metrics.append(run)
                 continue
```

### Comparing `xtlib-1.0.0rc1/xtlib/xt_client.py` & `xtlib-1.0.0rc2/xtlib/xt_client.py`

 * *Files identical despite different names*

### Comparing `xtlib-1.0.0rc1/README.md` & `xtlib-1.0.0rc2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 # XTlib: Experiment Tools Library
 
-XTlib is an API and command line tool for scaling and managing ML experiments.  
+XTlib is an API and command line tool for scaling and managing Machine Learning (ML) experiments.  
 
-The goal of XTLib is to enable you to effortlessly organize and scale your ML experiments.
-Our tools offer an incremental approach to adoption, so you can begin realizing benifits immediatly.
+XTLib enables you to efficiently organize and scale your ML experiments.
+Our tools offer an incremental approach to adoption, so you can immediately realize benefits to your research from using XTlib.
 
-XT Key Features
-  - Scale ML experiments across multiple COMPUTE services:
-      - local machine, VM's, Philly, Azure Batch, Azure AML
-  - Provide a consistent STORAGE model:
-      - workspaces, experiments, jobs, runs
-      - blob shares
-  - Provide related tooling:
-      - live tensorboard, hyperparameter searching, reporting, plotting, utilities
-
-XTLib provides an experiment STORE that enables you to easily track, compare, rerun, and share your ML experiments.  
-The STORE consists of user-defined workspaces, each of which can contain a set of user-run experiments.  
-XT currently supports 2 STORE services: local (folder-based) and azure (Azure Storage-based).
-
-In addition, XTLb also provides easy access to scalable COMPUTE resources so you can 
-easily run multiple experiments in parallel and on larger computers, as needed.  With this feature, 
-you can scale from running  experiments on your local machine, to multiple VM's under your control, to compute 
-services like Azure Batch and Azure ML.
-
-Finally, XTLib offers a few other experiment-related features to help maximize your ML agility:
-    - hyperparameter searching
-    - run and job reports
-    - ad-hoc plotting
+XTlib Key Features
+  - XTlib scales your ML experiments across multiple cloud compute services:
+      - Local machine and VM's, Philly, Azure Batch, and Azure Machine Learning (AML)
+  - XTlib provides a consistent storage model across services:
+      - Workspaces, experiments, jobs, and runs
+      - Blob shares
+  - XTLib also offers several experiment-related tools to expand your ML projects:
+    - Composable Tensorboard views (live and post-training)
+    - Hyperparameter searching
+    - Run and job reports
+    - Ad-hoc plotting
+
+XTLib provides an experiment store to track, compare, plot, rerun, and share your Machine Learning (ML) experiments.  
+The store consists of user-defined workspaces. Each workspace contains a set of user-run experiments.  
+XTlib supports flexible storage capabilities: local (folder-based) and Azure Storage services (cloud-based).
 
-For more information, run: xt --help
+XTLib also uses scalable cloud compute resources, so you can run multiple experiments in parallel and on larger computers, as needed. With this feature, you can scale experiments from your local machine, to multiple VM's under your control, to compute services like Azure Batch and Azure ML.
+
+For more information, run: xt --help, [or see our documentation](https://xtdocs.z22.web.core.windows.net/).
 
 # Contributing
 
 Check [CONTRIBUTING](CONTRIBUTING.md) page.
 
 # Microsoft Open Source Code of Conduct
```

### Comparing `xtlib-1.0.0rc1/setup.py` & `xtlib-1.0.0rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import platform
 import setuptools
 from setuptools import setup
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 
 # this must be incremented every time we push an update to pypi (but not before)
-VERSION ="1.0.0rc1"
+VERSION ="1.0.0rc2"
 
 # supply contents of our README file as our package's long description
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requirements = [
     # azure SDK
```

### Comparing `xtlib-1.0.0rc1/PKG-INFO` & `xtlib-1.0.0rc2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 Metadata-Version: 2.1
 Name: xtlib
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: A set of tools for organizing and scaling ML experiments
 Home-page: https://github.com/rfernand2
 Author: Roland Fernandez
 Author-email: rfernand@microsoft.com
 License: UNKNOWN
 Description: # XTlib: Experiment Tools Library
         
-        XTlib is an API and command line tool for scaling and managing ML experiments.  
+        XTlib is an API and command line tool for scaling and managing Machine Learning (ML) experiments.  
         
-        The goal of XTLib is to enable you to effortlessly organize and scale your ML experiments.
-        Our tools offer an incremental approach to adoption, so you can begin realizing benifits immediatly.
+        XTLib enables you to efficiently organize and scale your ML experiments.
+        Our tools offer an incremental approach to adoption, so you can immediately realize benefits to your research from using XTlib.
         
-        XT Key Features
-          - Scale ML experiments across multiple COMPUTE services:
-              - local machine, VM's, Philly, Azure Batch, Azure AML
-          - Provide a consistent STORAGE model:
-              - workspaces, experiments, jobs, runs
-              - blob shares
-          - Provide related tooling:
-              - live tensorboard, hyperparameter searching, reporting, plotting, utilities
-        
-        XTLib provides an experiment STORE that enables you to easily track, compare, rerun, and share your ML experiments.  
-        The STORE consists of user-defined workspaces, each of which can contain a set of user-run experiments.  
-        XT currently supports 2 STORE services: local (folder-based) and azure (Azure Storage-based).
-        
-        In addition, XTLb also provides easy access to scalable COMPUTE resources so you can 
-        easily run multiple experiments in parallel and on larger computers, as needed.  With this feature, 
-        you can scale from running  experiments on your local machine, to multiple VM's under your control, to compute 
-        services like Azure Batch and Azure ML.
-        
-        Finally, XTLib offers a few other experiment-related features to help maximize your ML agility:
-            - hyperparameter searching
-            - run and job reports
-            - ad-hoc plotting
+        XTlib Key Features
+          - XTlib scales your ML experiments across multiple cloud compute services:
+              - Local machine and VM's, Philly, Azure Batch, and Azure Machine Learning (AML)
+          - XTlib provides a consistent storage model across services:
+              - Workspaces, experiments, jobs, and runs
+              - Blob shares
+          - XTLib also offers several experiment-related tools to expand your ML projects:
+            - Composable Tensorboard views (live and post-training)
+            - Hyperparameter searching
+            - Run and job reports
+            - Ad-hoc plotting
+        
+        XTLib provides an experiment store to track, compare, plot, rerun, and share your Machine Learning (ML) experiments.  
+        The store consists of user-defined workspaces. Each workspace contains a set of user-run experiments.  
+        XTlib supports flexible storage capabilities: local (folder-based) and Azure Storage services (cloud-based).
         
-        For more information, run: xt --help
+        XTLib also uses scalable cloud compute resources, so you can run multiple experiments in parallel and on larger computers, as needed. With this feature, you can scale experiments from your local machine, to multiple VM's under your control, to compute services like Azure Batch and Azure ML.
+        
+        For more information, run: xt --help, [or see our documentation](https://xtdocs.z22.web.core.windows.net/).
         
         # Contributing
         
         Check [CONTRIBUTING](CONTRIBUTING.md) page.
         
         # Microsoft Open Source Code of Conduct
```

### Comparing `xtlib-1.0.0rc1/xtlib.egg-info/SOURCES.txt` & `xtlib-1.0.0rc2/xtlib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 xtlib/errors.py
 xtlib/file_utils.py
 xtlib/impl_base.py
 xtlib/impl_compute.py
 xtlib/impl_help.py
 xtlib/impl_shared.py
 xtlib/impl_storage.py
+xtlib/impl_storage_api.py
 xtlib/impl_utilities.py
 xtlib/job_helper.py
 xtlib/metric_set.py
 xtlib/mirror.py
 xtlib/mirror_worker.py
 xtlib/pc_utils.py
 xtlib/plot_builder.py
```

### Comparing `xtlib-1.0.0rc1/xtlib.egg-info/PKG-INFO` & `xtlib-1.0.0rc2/xtlib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 Metadata-Version: 2.1
 Name: xtlib
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: A set of tools for organizing and scaling ML experiments
 Home-page: https://github.com/rfernand2
 Author: Roland Fernandez
 Author-email: rfernand@microsoft.com
 License: UNKNOWN
 Description: # XTlib: Experiment Tools Library
         
-        XTlib is an API and command line tool for scaling and managing ML experiments.  
+        XTlib is an API and command line tool for scaling and managing Machine Learning (ML) experiments.  
         
-        The goal of XTLib is to enable you to effortlessly organize and scale your ML experiments.
-        Our tools offer an incremental approach to adoption, so you can begin realizing benifits immediatly.
+        XTLib enables you to efficiently organize and scale your ML experiments.
+        Our tools offer an incremental approach to adoption, so you can immediately realize benefits to your research from using XTlib.
         
-        XT Key Features
-          - Scale ML experiments across multiple COMPUTE services:
-              - local machine, VM's, Philly, Azure Batch, Azure AML
-          - Provide a consistent STORAGE model:
-              - workspaces, experiments, jobs, runs
-              - blob shares
-          - Provide related tooling:
-              - live tensorboard, hyperparameter searching, reporting, plotting, utilities
-        
-        XTLib provides an experiment STORE that enables you to easily track, compare, rerun, and share your ML experiments.  
-        The STORE consists of user-defined workspaces, each of which can contain a set of user-run experiments.  
-        XT currently supports 2 STORE services: local (folder-based) and azure (Azure Storage-based).
-        
-        In addition, XTLb also provides easy access to scalable COMPUTE resources so you can 
-        easily run multiple experiments in parallel and on larger computers, as needed.  With this feature, 
-        you can scale from running  experiments on your local machine, to multiple VM's under your control, to compute 
-        services like Azure Batch and Azure ML.
-        
-        Finally, XTLib offers a few other experiment-related features to help maximize your ML agility:
-            - hyperparameter searching
-            - run and job reports
-            - ad-hoc plotting
+        XTlib Key Features
+          - XTlib scales your ML experiments across multiple cloud compute services:
+              - Local machine and VM's, Philly, Azure Batch, and Azure Machine Learning (AML)
+          - XTlib provides a consistent storage model across services:
+              - Workspaces, experiments, jobs, and runs
+              - Blob shares
+          - XTLib also offers several experiment-related tools to expand your ML projects:
+            - Composable Tensorboard views (live and post-training)
+            - Hyperparameter searching
+            - Run and job reports
+            - Ad-hoc plotting
+        
+        XTLib provides an experiment store to track, compare, plot, rerun, and share your Machine Learning (ML) experiments.  
+        The store consists of user-defined workspaces. Each workspace contains a set of user-run experiments.  
+        XTlib supports flexible storage capabilities: local (folder-based) and Azure Storage services (cloud-based).
         
-        For more information, run: xt --help
+        XTLib also uses scalable cloud compute resources, so you can run multiple experiments in parallel and on larger computers, as needed. With this feature, you can scale experiments from your local machine, to multiple VM's under your control, to compute services like Azure Batch and Azure ML.
+        
+        For more information, run: xt --help, [or see our documentation](https://xtdocs.z22.web.core.windows.net/).
         
         # Contributing
         
         Check [CONTRIBUTING](CONTRIBUTING.md) page.
         
         # Microsoft Open Source Code of Conduct
```

