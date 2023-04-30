# Comparing `tmp/qtc-0.0.1.tar.gz` & `tmp/qtc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtc-0.0.1.tar", last modified: Wed Oct 19 03:06:05 2022, max compression
+gzip compressed data, was "qtc-0.0.2.tar", last modified: Sun Apr 30 15:12:40 2023, max compression
```

## Comparing `qtc-0.0.1.tar` & `qtc-0.0.2.tar`

### file list

```diff
@@ -1,82 +1,79 @@
-drwxrwxr-x   0 ahu       (1000) ahu       (1000)        0 2022-10-19 03:06:05.530600 qtc-0.0.1/
--rw-rw-r--   0 ahu       (1000) ahu       (1000)       62 2022-10-19 02:17:40.000000 qtc-0.0.1/MANIFEST.in
--rw-rw-r--   0 ahu       (1000) ahu       (1000)      157 2022-10-19 03:06:05.530600 qtc-0.0.1/PKG-INFO
--rw-rw-r--   0 ahu       (1000) ahu       (1000)       29 2022-10-19 02:18:27.000000 qtc-0.0.1/README.md
-drwxrwxr-x   0 ahu       (1000) ahu       (1000)        0 2022-10-19 03:06:05.526600 qtc-0.0.1/backup/
-drwxrwxr-x   0 ahu       (1000) ahu       (1000)        0 2022-10-19 03:06:05.526600 qtc-0.0.1/backup/calendar/
--rw-rw-r--   0 ahu       (1000) ahu       (1000)        0 2022-10-19 02:54:43.000000 qtc-0.0.1/backup/calendar/__init__.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     6923 2022-09-14 02:10:24.000000 qtc-0.0.1/backup/calendar/exchange_calendar.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)    11393 2022-10-19 01:39:50.000000 qtc-0.0.1/backup/calendar/factor_model_calendar.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     2010 2022-09-14 02:10:24.000000 qtc-0.0.1/backup/calendar/test_exchange_calendar.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     2903 2022-09-14 02:10:24.000000 qtc-0.0.1/backup/calendar/test_factor_model_calendar.py
-drwxrwxr-x   0 ahu       (1000) ahu       (1000)        0 2022-10-19 03:06:05.526600 qtc-0.0.1/backup/ext/
--rw-rw-r--   0 ahu       (1000) ahu       (1000)        0 2022-10-19 02:55:04.000000 qtc-0.0.1/backup/ext/__init__.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     4523 2022-10-19 01:47:43.000000 qtc-0.0.1/backup/ext/path.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     1311 2022-10-19 02:55:18.000000 qtc-0.0.1/backup/ext/test_path.py
-drwxrwxr-x   0 ahu       (1000) ahu       (1000)        0 2022-10-19 03:06:05.526600 qtc-0.0.1/backup/toolbox/
--rw-rw-r--   0 ahu       (1000) ahu       (1000)        0 2022-10-19 02:55:28.000000 qtc-0.0.1/backup/toolbox/__init__.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)    19589 2022-09-14 02:10:24.000000 qtc-0.0.1/backup/toolbox/factor_model_based_single_dt_analyzer.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)    10527 2022-10-19 02:55:06.000000 qtc-0.0.1/backup/toolbox/task_executor.py
-drwxrwxr-x   0 ahu       (1000) ahu       (1000)        0 2022-10-19 03:06:05.526600 qtc-0.0.1/qtc/
--rw-rw-r--   0 ahu       (1000) ahu       (1000)        0 2022-05-02 22:58:24.000000 qtc-0.0.1/qtc/__init__.py
-drwxrwxr-x   0 ahu       (1000) ahu       (1000)        0 2022-10-19 03:06:05.530600 qtc-0.0.1/qtc/calendar/
--rw-rw-r--   0 ahu       (1000) ahu       (1000)        0 2022-05-18 22:13:10.000000 qtc-0.0.1/qtc/calendar/__init__.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)    10261 2022-10-19 01:39:50.000000 qtc-0.0.1/qtc/calendar/calendar.py
-drwxrwxr-x   0 ahu       (1000) ahu       (1000)        0 2022-10-19 03:06:05.530600 qtc-0.0.1/qtc/consts/
--rw-rw-r--   0 ahu       (1000) ahu       (1000)        0 2022-05-04 16:17:02.000000 qtc-0.0.1/qtc/consts/__init__.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     2156 2022-10-19 01:42:01.000000 qtc-0.0.1/qtc/consts/enums.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)      368 2022-10-19 02:36:05.000000 qtc-0.0.1/qtc/env_config.cfg
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     5371 2022-10-19 02:34:48.000000 qtc-0.0.1/qtc/env_config.py
-drwxrwxr-x   0 ahu       (1000) ahu       (1000)        0 2022-10-19 03:06:05.530600 qtc-0.0.1/qtc/ext/
--rw-rw-r--   0 ahu       (1000) ahu       (1000)        0 2022-05-03 21:19:02.000000 qtc-0.0.1/qtc/ext/__init__.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     1459 2022-10-19 01:43:08.000000 qtc-0.0.1/qtc/ext/configurable.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     1145 2022-10-19 01:43:22.000000 qtc-0.0.1/qtc/ext/enum.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     1992 2022-10-19 01:43:38.000000 qtc-0.0.1/qtc/ext/inspect.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     2131 2022-10-19 01:43:51.000000 qtc-0.0.1/qtc/ext/logging.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     1453 2022-10-19 01:44:23.000000 qtc-0.0.1/qtc/ext/multiprocessing.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     1037 2022-10-19 01:47:51.000000 qtc-0.0.1/qtc/ext/unittest.py
-drwxrwxr-x   0 ahu       (1000) ahu       (1000)        0 2022-10-19 03:06:05.530600 qtc-0.0.1/qtc/file/
--rw-rw-r--   0 ahu       (1000) ahu       (1000)        0 2022-05-10 22:47:46.000000 qtc-0.0.1/qtc/file/__init__.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     9082 2022-10-19 01:50:29.000000 qtc-0.0.1/qtc/file/file_cache.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)    16274 2022-10-19 01:52:54.000000 qtc-0.0.1/qtc/file/file_manager.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)    29508 2022-10-19 01:55:38.000000 qtc-0.0.1/qtc/file/file_serialization.py
-drwxrwxr-x   0 ahu       (1000) ahu       (1000)        0 2022-10-19 03:06:05.530600 qtc-0.0.1/qtc/toolbox/
--rw-rw-r--   0 ahu       (1000) ahu       (1000)        0 2022-05-27 17:34:52.000000 qtc-0.0.1/qtc/toolbox/__init__.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     5483 2022-08-10 20:07:10.000000 qtc-0.0.1/qtc/toolbox/calcs.py
-drwxrwxr-x   0 ahu       (1000) ahu       (1000)        0 2022-10-19 03:06:05.530600 qtc-0.0.1/qtc/utils/
--rw-rw-r--   0 ahu       (1000) ahu       (1000)        0 2022-05-04 16:16:04.000000 qtc-0.0.1/qtc/utils/__init__.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)    10420 2022-10-19 01:58:27.000000 qtc-0.0.1/qtc/utils/datetime_utils.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)    30465 2022-10-19 01:58:39.000000 qtc-0.0.1/qtc/utils/db_utils.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     7717 2022-10-19 01:59:31.000000 qtc-0.0.1/qtc/utils/email_utils.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     4339 2022-10-19 02:02:19.000000 qtc-0.0.1/qtc/utils/endpoint_utils.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     7380 2022-10-19 02:02:48.000000 qtc-0.0.1/qtc/utils/file_system_utils.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     7840 2022-08-04 19:38:08.000000 qtc-0.0.1/qtc/utils/html_utils.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     6657 2022-10-19 02:03:59.000000 qtc-0.0.1/qtc/utils/misc_utils.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)    11393 2022-10-19 02:05:44.000000 qtc-0.0.1/qtc/utils/notebook_utils.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)       23 2022-09-14 03:01:55.000000 qtc-0.0.1/qtc/version.py
-drwxrwxr-x   0 ahu       (1000) ahu       (1000)        0 2022-10-19 03:06:05.530600 qtc-0.0.1/qtc.egg-info/
--rw-rw-r--   0 ahu       (1000) ahu       (1000)      157 2022-10-19 03:06:05.000000 qtc-0.0.1/qtc.egg-info/PKG-INFO
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     1604 2022-10-19 03:06:05.000000 qtc-0.0.1/qtc.egg-info/SOURCES.txt
--rw-rw-r--   0 ahu       (1000) ahu       (1000)        1 2022-10-19 03:06:05.000000 qtc-0.0.1/qtc.egg-info/dependency_links.txt
--rw-rw-r--   0 ahu       (1000) ahu       (1000)        1 2022-10-19 03:06:05.000000 qtc-0.0.1/qtc.egg-info/not-zip-safe
--rw-rw-r--   0 ahu       (1000) ahu       (1000)      138 2022-10-19 03:06:05.000000 qtc-0.0.1/qtc.egg-info/requires.txt
--rw-rw-r--   0 ahu       (1000) ahu       (1000)       17 2022-10-19 03:06:05.000000 qtc-0.0.1/qtc.egg-info/top_level.txt
--rw-rw-r--   0 ahu       (1000) ahu       (1000)       38 2022-10-19 03:06:05.530600 qtc-0.0.1/setup.cfg
--rw-rw-r--   0 ahu       (1000) ahu       (1000)      852 2022-10-19 03:06:03.000000 qtc-0.0.1/setup.py
-drwxrwxr-x   0 ahu       (1000) ahu       (1000)        0 2022-10-19 03:06:05.530600 qtc-0.0.1/tests/
--rw-rw-r--   0 ahu       (1000) ahu       (1000)        0 2022-05-03 22:30:08.000000 qtc-0.0.1/tests/__init__.py
-drwxrwxr-x   0 ahu       (1000) ahu       (1000)        0 2022-10-19 03:06:05.530600 qtc-0.0.1/tests/ext/
--rw-rw-r--   0 ahu       (1000) ahu       (1000)        0 2022-05-03 22:30:20.000000 qtc-0.0.1/tests/ext/__init__.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)      995 2022-10-19 02:56:32.000000 qtc-0.0.1/tests/ext/test_enum.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)      580 2022-10-19 02:14:05.000000 qtc-0.0.1/tests/ext/test_inspect.py
-drwxrwxr-x   0 ahu       (1000) ahu       (1000)        0 2022-10-19 03:06:05.530600 qtc-0.0.1/tests/file/
--rw-rw-r--   0 ahu       (1000) ahu       (1000)        0 2021-10-12 14:39:52.000000 qtc-0.0.1/tests/file/__init__.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     4834 2022-10-19 02:15:10.000000 qtc-0.0.1/tests/file/test_file_cache.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     3244 2022-10-19 02:15:26.000000 qtc-0.0.1/tests/file/test_file_manager.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     5806 2022-10-19 02:16:21.000000 qtc-0.0.1/tests/file/test_file_serialization.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)      431 2022-10-19 02:39:48.000000 qtc-0.0.1/tests/test_env_config.py
-drwxrwxr-x   0 ahu       (1000) ahu       (1000)        0 2022-10-19 03:06:05.530600 qtc-0.0.1/tests/utils/
--rw-rw-r--   0 ahu       (1000) ahu       (1000)        0 2022-05-04 21:02:04.000000 qtc-0.0.1/tests/utils/__init__.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     3935 2022-10-19 02:16:41.000000 qtc-0.0.1/tests/utils/test_datetime_utils.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     2604 2022-10-19 02:38:55.000000 qtc-0.0.1/tests/utils/test_db_utils.py
--rw-rw-r--   0 ahu       (1000) ahu       (1000)     1855 2022-10-19 02:17:06.000000 qtc-0.0.1/tests/utils/test_misc_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.668745 qtc-0.0.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-04-28 00:35:58.000000 qtc-0.0.2/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      157 2023-04-30 15:12:40.668745 qtc-0.0.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2023-04-28 00:35:58.000000 qtc-0.0.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.648744 qtc-0.0.2/qtc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.652744 qtc-0.0.2/qtc/app_configs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:20.000000 qtc-0.0.2/qtc/app_configs/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.652744 qtc-0.0.2/qtc/app_configs/bq/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:25.000000 qtc-0.0.2/qtc/app_configs/bq/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      247 2023-04-29 15:40:25.000000 qtc-0.0.2/qtc/app_configs/bq/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4648 2023-04-29 15:41:30.000000 qtc-0.0.2/qtc/app_configs/bq/params.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.652744 qtc-0.0.2/qtc/app_configs/bq_sim/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:22.000000 qtc-0.0.2/qtc/app_configs/bq_sim/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5745 2023-04-29 15:40:22.000000 qtc-0.0.2/qtc/app_configs/bq_sim/params.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.652744 qtc-0.0.2/qtc/calendar/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/calendar/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10261 2023-04-28 01:40:37.000000 qtc-0.0.2/qtc/calendar/calendar.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.652744 qtc-0.0.2/qtc/consts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/consts/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6908 2023-04-29 15:42:12.000000 qtc-0.0.2/qtc/consts/enums.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      370 2023-04-30 15:11:38.000000 qtc-0.0.2/qtc/env_config.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5371 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/env_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.656744 qtc-0.0.2/qtc/ext/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/ext/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1459 2023-04-28 01:41:03.000000 qtc-0.0.2/qtc/ext/configurable.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1145 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/ext/enum.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1992 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/ext/inspect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/ext/logging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1453 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/ext/multiprocessing.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1037 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/ext/unittest.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.656744 qtc-0.0.2/qtc/file/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/file/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9319 2023-04-28 01:57:29.000000 qtc-0.0.2/qtc/file/file_cache.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16376 2023-04-28 01:57:29.000000 qtc-0.0.2/qtc/file/file_manager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30307 2023-04-28 01:57:29.000000 qtc-0.0.2/qtc/file/file_serialization.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.656744 qtc-0.0.2/qtc/toolbox/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/toolbox/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5483 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/toolbox/calcs.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.660744 qtc-0.0.2/qtc/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2691 2023-04-28 02:42:24.000000 qtc-0.0.2/qtc/utils/cipher_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3944 2023-04-28 02:53:51.000000 qtc-0.0.2/qtc/utils/dash_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27303 2023-04-29 14:44:17.000000 qtc-0.0.2/qtc/utils/datetime_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30465 2023-04-28 01:46:30.000000 qtc-0.0.2/qtc/utils/db_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7567 2023-04-28 02:56:22.000000 qtc-0.0.2/qtc/utils/email_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4540 2023-04-28 01:49:03.000000 qtc-0.0.2/qtc/utils/endpoint_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6612 2023-04-28 03:01:16.000000 qtc-0.0.2/qtc/utils/file_system_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7840 2023-04-28 01:53:01.000000 qtc-0.0.2/qtc/utils/html_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6663 2023-04-28 01:57:29.000000 qtc-0.0.2/qtc/utils/misc_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11079 2023-04-28 01:57:29.000000 qtc-0.0.2/qtc/utils/notebook_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-04-28 01:40:20.000000 qtc-0.0.2/qtc/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.652744 qtc-0.0.2/qtc.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      157 2023-04-30 15:12:40.000000 qtc-0.0.2/qtc.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1500 2023-04-30 15:12:40.000000 qtc-0.0.2/qtc.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-30 15:12:40.000000 qtc-0.0.2/qtc.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-29 14:49:44.000000 qtc-0.0.2/qtc.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-04-30 15:12:40.000000 qtc-0.0.2/qtc.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-04-30 15:12:40.000000 qtc-0.0.2/qtc.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-30 15:12:40.668745 qtc-0.0.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      763 2023-04-28 03:01:16.000000 qtc-0.0.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.664744 qtc-0.0.2/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.664744 qtc-0.0.2/tests/ext/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/ext/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1003 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/ext/test_enum.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      580 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/ext/test_inspect.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.664744 qtc-0.0.2/tests/file/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/file/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4834 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/file/test_file_cache.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3244 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/file/test_file_manager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5806 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/file/test_file_serialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      431 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/test_env_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.668745 qtc-0.0.2/tests/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      558 2023-04-28 02:46:02.000000 qtc-0.0.2/tests/utils/test_cipher_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3939 2023-04-28 02:45:02.000000 qtc-0.0.2/tests/utils/test_datetime_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2604 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/utils/test_db_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1855 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/utils/test_misc_utils.py
```

### Comparing `qtc-0.0.1/qtc/calendar/calendar.py` & `qtc-0.0.2/qtc/calendar/calendar.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.1/qtc/env_config.py` & `qtc-0.0.2/qtc/env_config.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.1/qtc/ext/configurable.py` & `qtc-0.0.2/qtc/ext/configurable.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.1/qtc/ext/enum.py` & `qtc-0.0.2/qtc/ext/enum.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.1/qtc/ext/inspect.py` & `qtc-0.0.2/qtc/ext/inspect.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.1/qtc/ext/logging.py` & `qtc-0.0.2/qtc/ext/logging.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.1/qtc/ext/multiprocessing.py` & `qtc-0.0.2/qtc/ext/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.1/qtc/ext/unittest.py` & `qtc-0.0.2/qtc/ext/unittest.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.1/qtc/file/file_cache.py` & `qtc-0.0.2/qtc/file/file_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,19 +42,26 @@
         if isinstance(file_cache_name, str):
             try:
                 file_cache_name = FileCacheNameFormat.retrieve(file_cache_name)
             except:
                 pass
 
         if isinstance(file_cache_name, str):
-            if 'dateid' in kwargs:
-                file_cache_name = file_cache_name.replace('${date}', str(kwargs['dateid']))
-            elif 'date' in kwargs:
-                dateid = dtu.normalize_date_to_dateid(date=kwargs['date'])
-                file_cache_name = file_cache_name.replace('${date}', str(dateid))
+            for k, v in kwargs.items():
+                if v is None:
+                    continue
+                    
+                if k in ['dateid','date']:
+                    dateid = dtu.normalize_date_to_dateid(date=v)
+                    for field in ['dateid', 'date']:
+                        ks = '${' + field + '}'
+                        file_cache_name = file_cache_name.replace(ks, str(dateid))
+                else:
+                    ks = '${' + k + '}'
+                    file_cache_name = file_cache_name.replace(ks, str(v))
 
             return file_cache_name
 
         if file_cache_name==FileCacheNameFormat.FUNC_NAME:
             return self.func.__name__
         elif file_cache_name==FileCacheNameFormat.FUNC_NAME_DATEID:
             file_cache_name = self.func.__name__
```

### Comparing `qtc-0.0.1/qtc/file/file_manager.py` & `qtc-0.0.2/qtc/file/file_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,19 +198,21 @@
                      allow_as_of=False,
                      dt_col=None,
                      log_error=True,
                      ret_filepath=False,
                      **kwargs):
         file_serializer = self.get_file_serializer(file_serializer=file_serializer)
 
-        file_path = self.search_file(file_serializer=file_serializer,
-                                     dt=dt, subfolders=subfolders, is_subfolders_under_dt_folder=is_subfolders_under_dt_folder,
-                                     extra_filename_components=extra_filename_components,
-                                     allow_as_of=allow_as_of,
-                                     log_error=log_error)
+        file_path = kwargs.get('file_path', None)
+        if file_path is None:
+            file_path = self.search_file(file_serializer=file_serializer,
+                                         dt=dt, subfolders=subfolders, is_subfolders_under_dt_folder=is_subfolders_under_dt_folder,
+                                         extra_filename_components=extra_filename_components,
+                                         allow_as_of=allow_as_of,
+                                         log_error=log_error)
 
         data = file_serializer._deserialize(file_path=file_path, log_error=log_error)
 
         try:
             if dt_col is not None and dt_col not in data.columns:
                 data[dt_col] = dtu.normalize_dt(dt=dt, timezone=self.datetime_folders_builder.timezone)
         except:
```

### Comparing `qtc-0.0.1/qtc/file/file_serialization.py` & `qtc-0.0.2/qtc/file/file_serialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,21 +169,28 @@
     PICKLE_GZ = 'pickle.gz'
     LOG = 'log'
     HTML = 'html'
     FEATHER = 'feather'
     FTR = 'ftr'
     JAY = 'jay'
     JAY_GZ = 'jay.gz'
+    PDF = 'pdf'
 
     @staticmethod
     def suffix(protocol):
-        if isinstance(protocol, str):
-            protocol = FileSerializationProtocol.retrieve(protocol)
+        try:
+            if isinstance(protocol, str):
+                protocol = FileSerializationProtocol.retrieve(protocol)
 
-        return protocol.value
+            ret = protocol.value
+        except:
+            logger.warn(f'Faild to retrieve FileSerializationProtocol with value={protocol} !')
+            ret = protocol
+
+        return ret
 
     @staticmethod
     def protocol(suffix):
         if suffix.startswith('.'):
             suffix = suffix[1:]
 
         try:
@@ -247,14 +254,18 @@
 
 class FileSerializer:
     @property
     def filename_prefix(self):
         return self.__filename_prefix
 
     @property
+    def filename_exclude_str(self):
+        return self.__filename_exclude_str
+
+    @property
     def filename_dt_component_type(self):
         return self.__filename_dt_component_type
 
     @property
     def protocol(self):
         return self.__protocol
 
@@ -270,16 +281,18 @@
     def kwargs(self):
         return self.__kwargs
 
     def __init__(self, filename_prefix,
                  filename_dt_component_type,
                  protocol='PKL.GZ',
                  filename_component_sep='.',
+                 filename_exclude_str=None,
                  **kwargs):
         self.__filename_prefix = filename_prefix
+        self.__filename_exclude_str = filename_exclude_str
 
         if isinstance(filename_dt_component_type, str):
             filename_dt_component_type = FilenameDateTimeComponentType.retrieve(filename_dt_component_type)
 
         self.__filename_dt_component_type = filename_dt_component_type
 
         if isinstance(protocol, str):
@@ -366,15 +379,16 @@
         sep = f'{self.filename_component_sep}*'
         file_pattern = sep.join(filename_components)
         if len(filename_components)==1 and self.filename_dt_component_type!=FilenameDateTimeComponentType.NON_DATETIME:
             file_pattern += sep
 
         file_pattern = f'{file_pattern}.{self.suffix}'
 
-        files = fsu.search_files_by_pattern(file_patten=file_pattern, folder=folder)
+        files = fsu.search_files_by_pattern(file_patten=file_pattern, folder=folder,
+                                            exclude_str=self.filename_exclude_str)
 
         if allow_as_of:
             if self.filename_dt_component_type!=FilenameDateTimeComponentType.NON_DATETIME:
                 files = [f for f in files if fsu.is_earlier(path=f.replace(f'.{self.suffix}',''),
                                                             target_dt=dt,
                                                             filename_sep=self.filename_component_sep, timezone=timezone)]
             if len(files)>=1:
@@ -583,28 +597,30 @@
     __registry = dict()
     __named_registry = dict()
 
     @classmethod
     def get(cls, filename_prefix, filename_dt_component_type,
             protocol='PKL.GZ',
             filename_component_sep='.',
+            filename_exclude_str=None,
             **kwargs):
         if isinstance(filename_dt_component_type, str):
             filename_dt_component_type = FilenameDateTimeComponentType.retrieve(filename_dt_component_type)
 
         if isinstance(protocol, str):
             protocol = FileSerializationProtocol.retrieve(protocol)
 
-        key = (filename_prefix, filename_dt_component_type, protocol, filename_component_sep)
+        key = (filename_prefix, filename_dt_component_type, protocol, filename_component_sep, filename_exclude_str)
         if key not in FileSerializerManager.__registry:
             FileSerializerManager.__registry[key] = \
                 FileSerializer(filename_prefix=filename_prefix,
                                filename_dt_component_type=filename_dt_component_type,
                                protocol=protocol,
                                filename_component_sep=filename_component_sep,
+                               filename_exclude_str=filename_exclude_str,
                                **kwargs)
         # else:
         #     logger.warn(f'Skipping creating a new FileSerializer object since '
         #                 f'key=(filename_prefix={filename_prefix}, filename_dt_component_type={filename_dt_component_type}, protocol={protocol}, filename_component_sep={filename_component_sep}) '
         #                 f'has been registered!')
         #
         return FileSerializerManager.__registry[key]
@@ -619,18 +635,20 @@
 
         return FileSerializerManager.__named_registry[name]
 
     @classmethod
     def register(cls, name, filename_prefix, filename_dt_component_type,
                  protocol='PKL.GZ',
                  filename_component_sep='.',
+                 filename_exclude_str=None,
                  **kwargs):
         if name in FileSerializerManager.__named_registry:
             logger.error(f'name={name} exists in FileSerializerManager.__named_registry! Please choose another unique name!')
             return None
 
         FileSerializerManager.__named_registry[name] = FileSerializerManager.get(filename_prefix=filename_prefix,
                                                                                  filename_dt_component_type=filename_dt_component_type,
                                                                                  protocol=protocol,
                                                                                  filename_component_sep=filename_component_sep,
+                                                                                 filename_exclude_str=filename_exclude_str
                                                                                  **kwargs)
         return FileSerializerManager.__named_registry[name]
```

### Comparing `qtc-0.0.1/qtc/toolbox/calcs.py` & `qtc-0.0.2/qtc/toolbox/calcs.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.1/qtc/utils/db_utils.py` & `qtc-0.0.2/qtc/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.1/qtc/utils/email_utils.py` & `qtc-0.0.2/qtc/utils/email_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,22 @@
 from email.mime.application import MIMEApplication
 from email.mime.text import MIMEText
 import qtc.env_config as ecfg
 import qtc.utils.misc_utils as mu
 from qtc.ext.logging import set_logger
 logger = set_logger()
 
-USER_FULLNAME_MAP = {'ahu@bamfunds.com': 'Andrew Hu',
-                     'snindra@bamfunds.com': 'Sundeep Nindra',
-                     'mzhang@bamfunds.com': 'Minhua Zhang'}
+USER_FULLNAME_MAP = {}
 
 
-def normalize_email(email_address: str, domain='bamfunds.com') -> str:
+def normalize_email(email_address: str, domain: str) -> str:
     """
     >>> import qtc.utils.email_utils as emailu
     >>> emailu.normalize_email('ahu')
-    'ahu@bamfunds.com'
+    'ahu@***.com'
     """
     at_domain = f'@{domain}'
     if email_address.lower().endswith(at_domain):
         return email_address
 
     if '@' in email_address:
         raise Exception(f'Invalid character "@" found in email {email_address}. '
@@ -45,15 +43,15 @@
 def get_email_meta_field(field: str,
                          email_app=None,
                          default: str = None,
                          ) -> str:
     """
     >>> import qtc.utils.email_utils as emailu
     >>> emailu.get_email_meta_field(field='from', email_app='hedge_optimizer')
-    'RiskTechnology'
+    'QTHO'
     >>> emailu.get_email_meta_field(field='from')
     """
     cfg = ecfg.get_env_config()
     default = cfg.get(f'email.{field}', default)
     if email_app is None:
         return default
     #
@@ -113,15 +111,15 @@
 
 
 class HtmlEmail:
     def __init__(self,
                  subject: str,
                  email_app=None,
                  *,
-                 smtp_server = 'bamsmtp',
+                 smtp_server = 'smtp', # set default smtp_server here!!!
                  from_address = None,
                  to_address_list = None,
                  cc_address_list = None,
                  bcc_address_list = None
                  ) -> None:
         # self._email_app = email_app
         self._subject = format_email_subject(subject=subject, email_app=email_app)
```

### Comparing `qtc-0.0.1/qtc/utils/endpoint_utils.py` & `qtc-0.0.2/qtc/utils/endpoint_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,46 +45,52 @@
         if not response.ok:
             url_format = lambda x: x if len(x)<100 else x[0:100]+'...'
             logger.error(f'Failed with status code {response.status_code} for '
                          f'URL: {url_format(request_url)} with Body: {url_format(str(body))}')
             response.raise_for_status()
             return None
 
+        if data_transmission_protocol is None:
+            return response
+
         if isinstance(data_transmission_protocol, str):
             data_transmission_protocol = DataTransmissionProtocol.retrieve(data_transmission_protocol)
 
         if data_transmission_protocol==DataTransmissionProtocol.JSON:
             data = json.loads(response.content.decode('utf-8'))
             # print(f"JSON parsing time = {time.time()-start_time} @ request_url={request_url}")
         elif data_transmission_protocol==DataTransmissionProtocol.PICKLE:
             data = pickle.loads(response.content)
             # print(f"pickle.loads elapse time = {time.time()-start_time} @ request_url={request_url}")
+        elif data_transmission_protocol==DataTransmissionProtocol.TXT:
+            data = response.content.decode('utf-8')
 
     return data
 
 
 def process_request(request_url, is_post, body=None,
                     username=None, password=None,
                     data_transmission_protocol='JSON',
                     max_retry=0, retry_interval=60):
     data = None
     n_try = 0
-    while data is None and n_try<=max_retry:
-        if n_try!=0:
-            logger.warn(f'Sleeping for {retry_interval} seconds before {n_try} retry ...')
-            time.sleep(retry_interval)
-
+    while data is None:
         try:
             data = _process_request(request_url=request_url, is_post=is_post, body=body,
                                     username=username, password=password,
                                     data_transmission_protocol=data_transmission_protocol)
         except:
             traceback.print_exc()
 
         n_try += 1
+        if n_try>max_retry:
+            break
+
+        logger.warn(f'Sleeping for {retry_interval} seconds before {n_try} retry ...')
+        time.sleep(retry_interval)
 
     if data is None and max_retry>0:
         logger.error(f'Failed to get data after {max_retry} retries !')
 
     return data
```

### Comparing `qtc-0.0.1/qtc/utils/file_system_utils.py` & `qtc-0.0.2/qtc/utils/file_system_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from qtc.ext.logging import set_logger
 logger = set_logger()
 
 
 def extract_datetime_from_path(path, dt_index=None, filename_sep='.', timezone=None):
     """
     >>> import qtc.utils.file_system_utils as fsu
-    >>> fsu.extract_datetime_from_path(path='/mnt/rsk/Risk/Earnings/2021/202110/20211004/earnings.20211004.csv')
+    >>> fsu.extract_datetime_from_path(path='$HOME/earnings.20211004.csv')
     datetime.datetime(2021, 10, 4, 0, 0)
     """
     dt = None
     try:
         components = os.path.basename(path).split(filename_sep)
         if dt_index is None:
             for component in components:
@@ -31,18 +31,18 @@
 
     return dt
 
 
 def is_earlier(path, target_dt=None, dt_index=None, filename_sep='.', timezone=None):
     """
     >>> import qtc.utils.file_system_utils as fsu
-    >>> fsu.is_earlier(path='/bam/aws/devel/quant_risk/market_data/2020/202009/20200901/market_data_snapshot_quantum/market_data_snapshot_quantum.20200901-210228.csv',
+    >>> fsu.is_earlier(path='${HOME}/market_data.20200901-210228.csv',
                        target_dt='20200901-210245')
     True
-    >>> fsu.is_earlier(path='/bam/aws/devel/quant_risk/market_data/2020/202009/20200901/market_data_snapshot_quantum/market_data_snapshot_quantum.20200901-210228.csv',
+    >>> fsu.is_earlier(path='${HOME}/market_data_.20200901-210228.csv',
                        target_dt='20200901-210100')
     False
     """
 
     target_dt = dtu.normalize_dt(dt=target_dt, timezone=timezone)
     if target_dt is None:
         raise Exception(f'target_dt={target_dt} cannot be recognized as a valid datetime !')
@@ -58,24 +58,17 @@
                              ret_abs_path=True, ascending=True, dt_no_later_than=None,
                              timezone=None):
     """
     >>> from qtc.ext.path import sysequity_dir
     >>> folder = sysequity_dir('Reports', 'Archive')
     >>> import qtc.utils.file_system_utils as fsu
     >>> fsu.list_datetime_subfolders(folder=folder)[:5]
-    ['/bam/aws/devel/quant_risk/EPA_Hist/Archive/20160104',
-     '/bam/aws/devel/quant_risk/EPA_Hist/Archive/20160105',
-     '/bam/aws/devel/quant_risk/EPA_Hist/Archive/20160106',
-     '/bam/aws/devel/quant_risk/EPA_Hist/Archive/20160107',
-     '/bam/aws/devel/quant_risk/EPA_Hist/Archive/20160108']
     >>> fsu.list_datetime_subfolders(folder=folder, ret_abs_path=False)[:5]
     ['20160104', '20160105', '20160106', '20160107', '20160108']
     >>> fsu.list_datetime_subfolders(folder=folder, dt_no_later_than=20160105)
-    ['/bam/aws/devel/quant_risk/EPA_Hist/Archive/20160104',
-     '/bam/aws/devel/quant_risk/EPA_Hist/Archive/20160105']
     >>> fsu.list_datetime_subfolders(folder=folder, ret_abs_path=False, ascending=False)[-5:]
     ['20160108', '20160107', '20160106', '20160105', '20160104']
     """
     def is_valid_datetime_folder(path, dt_no_later_than=None):
         if not os.path.isdir(path):
             return False
 
@@ -107,36 +100,35 @@
            for subfolder in os.listdir(folder) if is_valid_datetime_folder(os.path.join(folder, subfolder),
                                                                            dt_no_later_than=dt_no_later_than)]
     ret.sort(reverse=not ascending)
 
     return ret
 
 
-def search_files_by_pattern(file_patten, folder=None):
+def search_files_by_pattern(file_patten, folder=None, exclude_str=None):
     """
     >>> from qtc.ext.path import sysequity_dir
     >>> folder = quant_risk_dir('EPA_Hist', 'Archive', '20160104')
     >>> import qtc.utils.file_system_utils as fsu
     >>> fsu.search_files_by_pattern(file_patten='summary.*.*.pickle.gz', folder=folder)
-    ['/bam/aws/devel/quant_risk/EPA_Hist/Archive/20160104/summary.Archive.20160104.pickle.gz']
     """
     if folder is not None:
         file_patten = os.path.join(folder, file_patten)
 
     files = glob.glob(file_patten)
-    return files
+
+    return files if exclude_str is None else [file for file in files if exclude_str not in file]
 
 
 def search_single_file_by_pattern(file_patten, folder=None, log_error=True):
     """
     >>> from qtc.ext.path import sysequity_dir
     >>> folder = sysequity_dir('EPA_Hist', 'Archive', '20160104')
     >>> import qtc.utils.file_system_utils as fsu
     >>> fsu.search_single_file_by_pattern(file_patten='summary_GICS_IndustrySector.*.*.pickle.gz', folder=folder)
-    '/bam/aws/devel/quant_risk/EPA_Hist/Archive/20160104/summary_GICS_IndustrySector.Archive.20160104.pickle.gz'
     >>> fsu.search_single_file_by_pattern(file_patten='test.*.*.pickle.gz', folder=folder)
 
     """
     files = search_files_by_pattern(file_patten=file_patten, folder=folder)
     if len(files) != 1:
         if log_error:
             logger.error(f"Expecting exactly ONE file with pattern: {file_patten} in folder={folder}, "
```

### Comparing `qtc-0.0.1/qtc/utils/html_utils.py` & `qtc-0.0.2/qtc/utils/html_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.1/qtc/utils/misc_utils.py` & `qtc-0.0.2/qtc/utils/misc_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,16 +118,16 @@
 
     if not inplace:
         df = df.copy()
 
     if isinstance(decimal_unit, str):
         decimal_unit = DecimalUnit.retrieve(value=decimal_unit)
 
-    for col in cols:
-        if col in iterable_to_tuple(cols, raw_type='str'):
+    for col in iterable_to_tuple(cols, raw_type='str'):
+        if col in df.columns:
             if decimal_unit == DecimalUnit.PERCENTAGE:
                 df[col] *= 1e+2
             elif decimal_unit == DecimalUnit.BPS:
                 df[col] *= 1e+4
             elif decimal_unit != DecimalUnit.DECIMAL:
                 raise Exception(f'decimal_unit={decimal_unit} is not supported in [DECIMAL | PERCENTAGE | BPS] !')
```

### Comparing `qtc-0.0.1/qtc/utils/notebook_utils.py` & `qtc-0.0.2/qtc/utils/notebook_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 This module contains some tools to create cleaner report-like output in python notebooks
 """
 
 import base64, io
 import matplotlib.pyplot as plt
 import nbformat
-import nbparameterise
 from IPython.core.display import HTML, Markdown, display, Javascript
 from bs4 import BeautifulSoup
 from jinja2 import Template
 from matplotlib.axes._subplots import SubplotBase
 from nbconvert import HTMLExporter, PDFExporter
 from nbconvert.preprocessors import ExecutePreprocessor, TagRemovePreprocessor
 from qtc.utils.misc_utils import get_zero_centered_min_max
@@ -104,14 +103,16 @@
     for inp in soup.find_all('div', {'class': 'output_html rendered_html output_subarea output_execute_result'}):
         inp['style'] = 'overflow-x: visible;'
 
     return str(soup)
 
 
 def export_notebook_to_html(nb, notebook_filename_out, clean_notebook=True, template=None):
+    if isinstance(nb, str):
+        nb = _read_in_notebook(notebook_fp=nb)
     html_exporter = HTMLExporter(template_file=template) if template else HTMLExporter()
     body, resources = html_exporter.from_notebook_node(nb)
     out_fp = notebook_filename_out.replace(".ipynb", ".html")
     html_final = clean_html(body) if clean_notebook else body
     with open(out_fp, "w", encoding="utf8") as f:
         f.write(html_final)
 
@@ -126,60 +127,50 @@
 
 def _read_in_notebook(notebook_fp):
     with open(notebook_fp) as f:
         nb = nbformat.read(f, as_version=4)
     return nb
 
 
-def _set_parameters(nb, params_dict):
-    orig_parameters = nbparameterise.extract_parameters(nb)
-    params = nbparameterise.parameter_values(orig_parameters, **params_dict)
-    new_nb = nbparameterise.replace_definitions(nb, params, execute=False)
-    _add_notebook_title(new_nb)
-    for name, value in params_dict.items():
-        if name == 'notebook_title':
-            new_nb.metadata['title'] = value
-
-    return new_nb
-
-
-def _add_notebook_title(nb):
-    parameters = nbparameterise.extract_parameters(nb)
-    for p in parameters:
-        if p.name == 'notebook_title':
-            nb.metadata.title = p.value
-            return
-    # default
-    nb.metadata.title = 'NoteBook'
-
-
-def execute_notebook(notebook_path,
-                     notebook_path_out,
-                     params_dict,
-                     run_path='',
-                     timeout=600,
-                     export_html=True,
-                     remove_cell_tags=['remove_cell'],
-                     template=None):
-    nb = _read_in_notebook(notebook_path)
-    new_nb = _set_parameters(nb, params_dict)
-    ep = ExecutePreprocessor(timeout=timeout, kernel_name='python3')
-    tr = TagRemovePreprocessor()
-    tr.remove_cell_tags = remove_cell_tags
-
-    ep.preprocess(new_nb, {'metadata': {'path': run_path}})
-    new_nb, r = tr.preprocess(new_nb, {})
-    with open(notebook_path_out, mode='wt') as f:
-        nbformat.write(new_nb, f)
-    if export_html:
-        export_notebook_to_html(new_nb,
-                                notebook_path_out,
-                                clean_notebook=True,
-                                template=template)
-    return new_nb
+# def _add_notebook_title(nb):
+#     parameters = nbparameterise.extract_parameters(nb)
+#     for p in parameters:
+#         if p.name == 'notebook_title':
+#             nb.metadata.title = p.value
+#             return
+#     # default
+#     nb.metadata.title = 'NoteBook'
+# #
+
+
+# def execute_notebook(notebook_path,
+#                      notebook_path_out,
+#                      params_dict,
+#                      run_path='',
+#                      timeout=600,
+#                      export_html=True,
+#                      remove_cell_tags=['remove_cell'],
+#                      template=None):
+#     nb = _read_in_notebook(notebook_path)
+#     new_nb = _set_parameters(nb, params_dict)
+#     ep = ExecutePreprocessor(timeout=timeout, kernel_name='python3')
+#     tr = TagRemovePreprocessor()
+#     tr.remove_cell_tags = remove_cell_tags
+#
+#     ep.preprocess(new_nb, {'metadata': {'path': run_path}})
+#     new_nb, r = tr.preprocess(new_nb, {})
+#     with open(notebook_path_out, mode='wt') as f:
+#         nbformat.write(new_nb, f)
+#     if export_html:
+#         export_notebook_to_html(new_nb,
+#                                 notebook_path_out,
+#                                 clean_notebook=True,
+#                                 template=template)
+#     return new_nb
+# #
 
 
 def hide_toggle(for_next=False):
     import random
 
     this_cell = """$('div.cell.code_cell.rendered.selected')"""
     next_cell = this_cell + '.next()'
```

### Comparing `qtc-0.0.1/setup.py` & `qtc-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,22 +17,18 @@
     zip_safe=False,
     include_package_data=True,
     platforms='any',
     install_requires=[
         'pandas>=1.3.4',
         'joblib',
         'sqlalchemy',
-        'python-gssapi',
-        'PyMySQL',
         'psycopg2',
         'pyarrow',
         'datatable',
         'pytest-html',
         'pyyaml',
         'requests-kerberos',
-        'krb5',
-        'nbparameterise'
     ],
     tests_require=[
         'pytest'
     ],
 )
```

### Comparing `qtc-0.0.1/tests/ext/test_enum.py` & `qtc-0.0.2/tests/ext/test_enum.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
         self.assertEqual(RiskRegionEnum.retrieve_by_name('AP'), RiskRegionEnum.AP)
         self.assertEqual(RiskRegionEnum.retrieve_by_name('EU'), RiskRegionEnum.EU)
         self.assertEqual(RiskRegionEnum.retrieve_by_name('US'), RiskRegionEnum.US)
 
     def test_retrieve(self):
         class Symbology(Enum):
-            BAM_ID = 'SecurityId'
+            BARRA_ID = 'BarraId'
             AXIOMA_ID = 'AxiomaId'
-            ARIES_ID = 'AriesId'
+            FACTSET_ID = 'FactsetId'
 
-        self.assertEqual(Symbology.retrieve('SecurityId'), Symbology.BAM_ID)
+        self.assertEqual(Symbology.retrieve('BarraId'), Symbology.BARRA_ID)
         self.assertEqual(Symbology.retrieve('AXIOMA_ID'), Symbology.AXIOMA_ID)
-        self.assertEqual(Symbology.retrieve('AriesId'), Symbology.ARIES_ID)
+        self.assertEqual(Symbology.retrieve('FactsetId'), Symbology.FACTSET_ID)
 
 
 if __name__ == '__main__':
-    ut.main()
+    ut.main()
```

### Comparing `qtc-0.0.1/tests/ext/test_inspect.py` & `qtc-0.0.2/tests/ext/test_inspect.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.1/tests/file/test_file_cache.py` & `qtc-0.0.2/tests/file/test_file_cache.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.1/tests/file/test_file_manager.py` & `qtc-0.0.2/tests/file/test_file_manager.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.1/tests/file/test_file_serialization.py` & `qtc-0.0.2/tests/file/test_file_serialization.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.1/tests/utils/test_datetime_utils.py` & `qtc-0.0.2/tests/utils/test_datetime_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         self.assertEqual(dtu.is_weekday(20200511), True)
         self.assertEqual(dtu.is_weekday(20201128), False)
 
     def test_get_biz_dates(self):
         self.assertEqual(dtu.get_biz_dateids(start_date=20201120, end_date=20201129), [20201120, 20201123, 20201124, 20201125, 20201126, 20201127])
 
     def test_next_biz_date(self):
-        self.assertEqual(dtu.next_biz_dateid(date=20201125), 20201126)
-        self.assertEqual(dtu.next_biz_dateid(date=20201127), 20201130)
+        self.assertEqual(dtu.next_biz_dateid(dateid=20201125), 20201126)
+        self.assertEqual(dtu.next_biz_dateid(dateid=20201127), 20201130)
 
     def test_parse_datetime(self):
         self.assertEqual(dtu.parse_datetime(20200210), datetime(2020, 2, 10, 0, 0))
         self.assertEqual(dtu.parse_datetime('2020-11-25', ret_as_timestamp=True), pd.Timestamp('2020-11-25 00:00:00'))
 
         target = dtu.parse_datetime('20200210-164523', timezone='America/New_York')
         benchmark = datetime(2020, 2, 10, 16, 45, 23, tzinfo=pytz.timezone('America/New_York'))
```

### Comparing `qtc-0.0.1/tests/utils/test_db_utils.py` & `qtc-0.0.2/tests/utils/test_db_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.1/tests/utils/test_misc_utils.py` & `qtc-0.0.2/tests/utils/test_misc_utils.py`

 * *Files identical despite different names*

