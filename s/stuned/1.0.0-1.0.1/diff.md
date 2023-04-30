# Comparing `tmp/stuned-1.0.0.tar.gz` & `tmp/stuned-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stuned-1.0.0.tar", last modified: Sun Apr 30 20:34:36 2023, max compression
+gzip compressed data, was "stuned-1.0.1.tar", last modified: Sun Apr 30 21:19:13 2023, max compression
```

## Comparing `stuned-1.0.0.tar` & `stuned-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 arubinstein17  (4499) oh        (4049)        0 2023-04-30 20:34:36.000000 stuned-1.0.0/
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)     1077 2023-04-04 14:16:55.000000 stuned-1.0.0/LICENSE
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)      719 2023-04-30 20:34:36.000000 stuned-1.0.0/PKG-INFO
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)       79 2023-04-04 14:16:55.000000 stuned-1.0.0/README.md
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)       85 2023-04-30 20:19:26.000000 stuned-1.0.0/pyproject.toml
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)     4667 2023-04-30 20:34:36.000000 stuned-1.0.0/setup.cfg
-drwxr-xr-x   0 arubinstein17  (4499) oh        (4049)        0 2023-04-30 20:34:36.000000 stuned-1.0.0/src/
-drwxr-xr-x   0 arubinstein17  (4499) oh        (4049)        0 2023-04-30 20:34:36.000000 stuned-1.0.0/src/stuned/
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)        0 2023-04-04 15:11:41.000000 stuned-1.0.0/src/stuned/__init__.py
-drwxr-xr-x   0 arubinstein17  (4499) oh        (4049)        0 2023-04-30 20:34:36.000000 stuned-1.0.0/src/stuned/datasets/
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)        0 2023-04-04 15:25:23.000000 stuned-1.0.0/src/stuned/datasets/__init__.py
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)     3900 2023-04-04 14:23:11.000000 stuned-1.0.0/src/stuned/datasets/base.py
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)     3600 2023-04-04 16:43:10.000000 stuned-1.0.0/src/stuned/datasets/common.py
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)    17514 2023-04-04 16:46:04.000000 stuned-1.0.0/src/stuned/datasets/dsprites.py
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)    17533 2023-04-04 15:21:56.000000 stuned-1.0.0/src/stuned/datasets/features_labeller.py
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)    10719 2023-04-04 15:25:05.000000 stuned-1.0.0/src/stuned/datasets/tiny_imagenet.py
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)    11870 2023-04-04 16:49:01.000000 stuned-1.0.0/src/stuned/datasets/utils.py
-drwxr-xr-x   0 arubinstein17  (4499) oh        (4049)        0 2023-04-30 20:34:36.000000 stuned-1.0.0/src/stuned/utility/
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)        0 2023-04-04 14:24:27.000000 stuned-1.0.0/src/stuned/utility/__init__.py
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)     5652 2023-04-30 19:32:18.000000 stuned-1.0.0/src/stuned/utility/helpers_for_main.py
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)     4146 2023-04-30 19:38:59.000000 stuned-1.0.0/src/stuned/utility/helpers_for_tests.py
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)    44049 2023-04-30 19:13:03.000000 stuned-1.0.0/src/stuned/utility/logger.py
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)    44800 2023-04-30 19:43:38.000000 stuned-1.0.0/src/stuned/utility/utils.py
-drwxr-xr-x   0 arubinstein17  (4499) oh        (4049)        0 2023-04-30 20:34:36.000000 stuned-1.0.0/src/stuned.egg-info/
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)      719 2023-04-30 20:34:36.000000 stuned-1.0.0/src/stuned.egg-info/PKG-INFO
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)      630 2023-04-30 20:34:36.000000 stuned-1.0.0/src/stuned.egg-info/SOURCES.txt
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)        1 2023-04-30 20:34:36.000000 stuned-1.0.0/src/stuned.egg-info/dependency_links.txt
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)     3681 2023-04-30 20:34:36.000000 stuned-1.0.0/src/stuned.egg-info/requires.txt
--rw-r--r--   0 arubinstein17  (4499) oh        (4049)        7 2023-04-30 20:34:36.000000 stuned-1.0.0/src/stuned.egg-info/top_level.txt
+drwxr-xr-x   0 arubinstein17  (4499) oh        (4049)        0 2023-04-30 21:19:13.000000 stuned-1.0.1/
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)     1077 2023-04-04 14:16:55.000000 stuned-1.0.1/LICENSE
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)      719 2023-04-30 21:19:13.000000 stuned-1.0.1/PKG-INFO
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)       79 2023-04-04 14:16:55.000000 stuned-1.0.1/README.md
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)       85 2023-04-30 20:19:26.000000 stuned-1.0.1/pyproject.toml
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)     4667 2023-04-30 21:19:13.000000 stuned-1.0.1/setup.cfg
+drwxr-xr-x   0 arubinstein17  (4499) oh        (4049)        0 2023-04-30 21:19:13.000000 stuned-1.0.1/src/
+drwxr-xr-x   0 arubinstein17  (4499) oh        (4049)        0 2023-04-30 21:19:13.000000 stuned-1.0.1/src/stuned/
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)        0 2023-04-04 15:11:41.000000 stuned-1.0.1/src/stuned/__init__.py
+drwxr-xr-x   0 arubinstein17  (4499) oh        (4049)        0 2023-04-30 21:19:13.000000 stuned-1.0.1/src/stuned/datasets/
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)        0 2023-04-04 15:25:23.000000 stuned-1.0.1/src/stuned/datasets/__init__.py
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)     3900 2023-04-04 14:23:11.000000 stuned-1.0.1/src/stuned/datasets/base.py
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)     3600 2023-04-04 16:43:10.000000 stuned-1.0.1/src/stuned/datasets/common.py
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)    17514 2023-04-04 16:46:04.000000 stuned-1.0.1/src/stuned/datasets/dsprites.py
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)    17533 2023-04-04 15:21:56.000000 stuned-1.0.1/src/stuned/datasets/features_labeller.py
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)    10719 2023-04-04 15:25:05.000000 stuned-1.0.1/src/stuned/datasets/tiny_imagenet.py
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)    11870 2023-04-04 16:49:01.000000 stuned-1.0.1/src/stuned/datasets/utils.py
+drwxr-xr-x   0 arubinstein17  (4499) oh        (4049)        0 2023-04-30 21:19:13.000000 stuned-1.0.1/src/stuned/run_from_csv/
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)        0 2023-04-30 21:04:11.000000 stuned-1.0.1/src/stuned/run_from_csv/__init__.py
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)    13601 2023-04-30 21:09:58.000000 stuned-1.0.1/src/stuned/run_from_csv/__main__.py
+drwxr-xr-x   0 arubinstein17  (4499) oh        (4049)        0 2023-04-30 21:19:13.000000 stuned-1.0.1/src/stuned/utility/
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)        0 2023-04-04 14:24:27.000000 stuned-1.0.1/src/stuned/utility/__init__.py
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)     5953 2023-04-30 21:08:55.000000 stuned-1.0.1/src/stuned/utility/helpers_for_main.py
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)     4146 2023-04-30 19:38:59.000000 stuned-1.0.1/src/stuned/utility/helpers_for_tests.py
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)    44049 2023-04-30 19:13:03.000000 stuned-1.0.1/src/stuned/utility/logger.py
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)    44800 2023-04-30 19:43:38.000000 stuned-1.0.1/src/stuned/utility/utils.py
+drwxr-xr-x   0 arubinstein17  (4499) oh        (4049)        0 2023-04-30 21:19:13.000000 stuned-1.0.1/src/stuned.egg-info/
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)      719 2023-04-30 21:19:13.000000 stuned-1.0.1/src/stuned.egg-info/PKG-INFO
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)      702 2023-04-30 21:19:13.000000 stuned-1.0.1/src/stuned.egg-info/SOURCES.txt
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)        1 2023-04-30 21:19:13.000000 stuned-1.0.1/src/stuned.egg-info/dependency_links.txt
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)     3681 2023-04-30 21:19:13.000000 stuned-1.0.1/src/stuned.egg-info/requires.txt
+-rw-r--r--   0 arubinstein17  (4499) oh        (4049)        7 2023-04-30 21:19:13.000000 stuned-1.0.1/src/stuned.egg-info/top_level.txt
```

### Comparing `stuned-1.0.0/LICENSE` & `stuned-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stuned-1.0.0/PKG-INFO` & `stuned-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stuned
-Version: 1.0.0
+Version: 1.0.1
 Summary: Utility code from STAI (https://scalabletrustworthyai.github.io/)
 Home-page: https://github.com/AlexanderRubinstein/STAI-tuned
 Author: Alexander Rubinstein
 Author-email: rubalex14@gmail.com
 Project-URL: Bug Tracker, https://github.com/AlexanderRubinstein/STAI-tuned/issues
 Project-URL: repository, https://github.com/AlexanderRubinstein/STAI-tuned
 Classifier: Programming Language :: Python :: 3
```

### Comparing `stuned-1.0.0/setup.cfg` & `stuned-1.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = stuned
-version = 1.0.0
+version = 1.0.1
 author = Alexander Rubinstein
 author_email = rubalex14@gmail.com
 description = Utility code from STAI (https://scalabletrustworthyai.github.io/)
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/AlexanderRubinstein/STAI-tuned
 project_urls =
```

### Comparing `stuned-1.0.0/src/stuned/datasets/base.py` & `stuned-1.0.1/src/stuned/datasets/base.py`

 * *Files identical despite different names*

### Comparing `stuned-1.0.0/src/stuned/datasets/common.py` & `stuned-1.0.1/src/stuned/datasets/common.py`

 * *Files identical despite different names*

### Comparing `stuned-1.0.0/src/stuned/datasets/dsprites.py` & `stuned-1.0.1/src/stuned/datasets/dsprites.py`

 * *Files identical despite different names*

### Comparing `stuned-1.0.0/src/stuned/datasets/features_labeller.py` & `stuned-1.0.1/src/stuned/datasets/features_labeller.py`

 * *Files identical despite different names*

### Comparing `stuned-1.0.0/src/stuned/datasets/tiny_imagenet.py` & `stuned-1.0.1/src/stuned/datasets/tiny_imagenet.py`

 * *Files identical despite different names*

### Comparing `stuned-1.0.0/src/stuned/datasets/utils.py` & `stuned-1.0.1/src/stuned/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `stuned-1.0.0/src/stuned/utility/helpers_for_main.py` & `stuned-1.0.1/src/stuned/utility/helpers_for_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     make_logger_with_tmp_output_folder,
     handle_exception,
     redneck_logger_context,
     make_logger
 )
 
 
+AUTOGEN_PREFIX = "autogenerated"
 EXP_NAME_CONFIG_KEY = "experiment_name"
 RUN_PATH_CONFIG_KEY = "current_run_folder"
 START_TIME_CONFIG_KEY = "start_time"
 TYPE_KEY = "type"
 OUTPUT_CSV_KEY = "output_csv"
 DEFAULT_WANDB_CONFIG = \
     {
@@ -200,7 +201,21 @@
 def normalize_paths(config, nested_keys, separator='/'):
     for key in nested_keys:
         apply_func_to_dict_by_nested_key(
             config,
             key.split(separator),
             normalize_path
         )
+
+
+def make_csv_config(
+    csv_path,
+    csv_row_number,
+    spreadsheet_url,
+    worksheet_name
+):
+    return {
+        "path": csv_path,
+        "row_number": csv_row_number,
+        "spreadsheet_url": spreadsheet_url,
+        "worksheet_name": worksheet_name
+    }
```

### Comparing `stuned-1.0.0/src/stuned/utility/helpers_for_tests.py` & `stuned-1.0.1/src/stuned/utility/helpers_for_tests.py`

 * *Files identical despite different names*

### Comparing `stuned-1.0.0/src/stuned/utility/logger.py` & `stuned-1.0.1/src/stuned/utility/logger.py`

 * *Files identical despite different names*

### Comparing `stuned-1.0.0/src/stuned/utility/utils.py` & `stuned-1.0.1/src/stuned/utility/utils.py`

 * *Files identical despite different names*

### Comparing `stuned-1.0.0/src/stuned.egg-info/PKG-INFO` & `stuned-1.0.1/src/stuned.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stuned
-Version: 1.0.0
+Version: 1.0.1
 Summary: Utility code from STAI (https://scalabletrustworthyai.github.io/)
 Home-page: https://github.com/AlexanderRubinstein/STAI-tuned
 Author: Alexander Rubinstein
 Author-email: rubalex14@gmail.com
 Project-URL: Bug Tracker, https://github.com/AlexanderRubinstein/STAI-tuned/issues
 Project-URL: repository, https://github.com/AlexanderRubinstein/STAI-tuned
 Classifier: Programming Language :: Python :: 3
```

### Comparing `stuned-1.0.0/src/stuned.egg-info/SOURCES.txt` & `stuned-1.0.1/src/stuned.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,12 +11,14 @@
 src/stuned/datasets/__init__.py
 src/stuned/datasets/base.py
 src/stuned/datasets/common.py
 src/stuned/datasets/dsprites.py
 src/stuned/datasets/features_labeller.py
 src/stuned/datasets/tiny_imagenet.py
 src/stuned/datasets/utils.py
+src/stuned/run_from_csv/__init__.py
+src/stuned/run_from_csv/__main__.py
 src/stuned/utility/__init__.py
 src/stuned/utility/helpers_for_main.py
 src/stuned/utility/helpers_for_tests.py
 src/stuned/utility/logger.py
 src/stuned/utility/utils.py
```

### Comparing `stuned-1.0.0/src/stuned.egg-info/requires.txt` & `stuned-1.0.1/src/stuned.egg-info/requires.txt`

 * *Files identical despite different names*

