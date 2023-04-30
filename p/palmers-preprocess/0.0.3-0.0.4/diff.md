# Comparing `tmp/palmers_preprocess-0.0.3.tar.gz` & `tmp/palmers_preprocess-0.0.4.tar.gz`

## Comparing `palmers_preprocess-0.0.3.tar` & `palmers_preprocess-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,31 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/.idea/.gitignore
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/.idea/misc.xml
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/.idea/modules.xml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/.idea/sdatta_packages.iml
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/.idea/workspace.xml
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/src/palmers_preprocess/__init__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/src/palmers_preprocess/example.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/LICENSE
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/README.md
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/__init__.py
+-rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/clearml_data_handler.py
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/config.py
+-rw-r--r--   0        0        0    43603 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/events_handler.py
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/lags_feature_handler.py
+-rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/preprocessor.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/regular_data_handler.py
+-rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/features/__init__.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/features/config.py
+-rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/features/cumulative_features.py
+-rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/features/event_features.py
+-rw-r--r--   0        0        0     8418 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/features/future_features.py
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/features/lags_features.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/features/weather_features.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0   719548 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/tests/config_batch_dict.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/tests/event_feature_test.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/tests/features_test.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/tests/lags_features_test.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/tests/preprocessor_test.py
+-rw-r--r--   0        0        0    50890 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/tests/sanity_checks.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/tests/test_todelete.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/tests/weather_test.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/LICENSE
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/README.md
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/PKG-INFO
```

### Comparing `palmers_preprocess-0.0.3/pyproject.toml` & `palmers_preprocess-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "palmers_preprocess"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Roy ", email="roy@sdatta.ai" },
   { name="Assaf", email="assafm@sdatta.ai" },
   { name="Guy", email="assafm@sdatta.ai" },
   { name="Oran", email="assafm@sdatta.ai" },
   { name="Yotam", email="assafm@sdatta.ai" },
 ]
```

### Comparing `palmers_preprocess-0.0.3/PKG-INFO` & `palmers_preprocess-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palmers_preprocess
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package to preprocess data for Palmer's project
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Roy  <roy@sdatta.ai>, Assaf <assafm@sdatta.ai>, Guy <assafm@sdatta.ai>, Oran <assafm@sdatta.ai>, Yotam <assafm@sdatta.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

