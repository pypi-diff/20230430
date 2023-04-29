# Comparing `tmp/openmapflow-0.2.3rc2.tar.gz` & `tmp/openmapflow-0.2.3rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmapflow-0.2.3rc2.tar", last modified: Tue Mar  7 12:51:33 2023, max compression
+gzip compressed data, was "openmapflow-0.2.3rc3.tar", last modified: Thu Mar 23 20:56:35 2023, max compression
```

## Comparing `openmapflow-0.2.3rc2.tar` & `openmapflow-0.2.3rc3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-07 12:51:33.122643 openmapflow-0.2.3rc2/
--rw-r--r--   0 runner    (1001) docker     (116)    11314 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)    11535 2023-03-07 12:51:33.122643 openmapflow-0.2.3rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    11023 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-07 12:51:33.106642 openmapflow-0.2.3rc2/openmapflow/
--rw-r--r--   0 runner    (1001) docker     (116)      909 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1932 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/bands.py
--rw-r--r--   0 runner    (1001) docker     (116)     3249 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/bbox.py
--rw-r--r--   0 runner    (1001) docker     (116)     3584 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     1730 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)     1060 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/datasets.py
--rw-r--r--   0 runner    (1001) docker     (116)     4982 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/ee_boundingbox.py
--rw-r--r--   0 runner    (1001) docker     (116)    12124 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/ee_exporter.py
--rw-r--r--   0 runner    (1001) docker     (116)     6125 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/engineer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-07 12:51:33.110643 openmapflow-0.2.3rc2/openmapflow/eo/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/eo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1833 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/eo/era5.py
--rw-r--r--   0 runner    (1001) docker     (116)     2766 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/eo/sentinel1.py
--rw-r--r--   0 runner    (1001) docker     (116)     6278 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/eo/sentinel2.py
--rw-r--r--   0 runner    (1001) docker     (116)      386 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/eo/srtm.py
--rw-r--r--   0 runner    (1001) docker     (116)     8066 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/generate.py
--rw-r--r--   0 runner    (1001) docker     (116)     3153 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/inference.py
--rw-r--r--   0 runner    (1001) docker     (116)     7534 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/inference_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    13719 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/inference_widgets.py
--rw-r--r--   0 runner    (1001) docker     (116)     2305 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/label_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    23030 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/labeled_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-07 12:51:33.110643 openmapflow-0.2.3rc2/openmapflow/notebooks/
--rw-r--r--   0 runner    (1001) docker     (116)     4703 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/notebooks/compare_ceo_labels.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)    14669 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/notebooks/create_map.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)     9416 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/notebooks/generate_project.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)     9907 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/notebooks/new_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)     5802 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/notebooks/train.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)    21070 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/notebooks/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)      608 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/pytorch_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-07 12:51:33.110643 openmapflow-0.2.3rc2/openmapflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (116)     3931 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/scripts/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (116)     2310 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/scripts/merging.sh
--rw-r--r--   0 runner    (1001) docker     (116)     2730 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/scripts/openmapflow
--rw-r--r--   0 runner    (1001) docker     (116)      295 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/scripts/torchserve_start.sh
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-07 12:51:33.114642 openmapflow-0.2.3rc2/openmapflow/templates/
--rw-r--r--   0 runner    (1001) docker     (116)      685 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/templates/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     1615 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/templates/datasets.py
--rw-r--r--   0 runner    (1001) docker     (116)     3198 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/templates/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (116)      903 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/templates/github-deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1240 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/templates/github-test.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     6632 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/templates/integration_test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (116)     2687 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/templates/integration_test_project.py
--rw-r--r--   0 runner    (1001) docker     (116)     2914 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/templates/integration_test_train_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (116)      389 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/templates/openmapflow-default.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       32 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/templates/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)     6631 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/templates/train.py
--rw-r--r--   0 runner    (1001) docker     (116)     5221 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/torchserve_handler.py
--rw-r--r--   0 runner    (1001) docker     (116)     2695 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/train_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-07 12:51:33.118643 openmapflow-0.2.3rc2/openmapflow/trigger_inference_function/
--rw-r--r--   0 runner    (1001) docker     (116)     1177 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/trigger_inference_function/main.py
--rw-r--r--   0 runner    (1001) docker     (116)        8 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/trigger_inference_function/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2652 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/openmapflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-07 12:51:33.106642 openmapflow-0.2.3rc2/openmapflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    11535 2023-03-07 12:51:33.000000 openmapflow-0.2.3rc2/openmapflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2223 2023-03-07 12:51:33.000000 openmapflow-0.2.3rc2/openmapflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-07 12:51:33.000000 openmapflow-0.2.3rc2/openmapflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      265 2023-03-07 12:51:33.000000 openmapflow-0.2.3rc2/openmapflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2023-03-07 12:51:33.000000 openmapflow-0.2.3rc2/openmapflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       30 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-07 12:51:33.122643 openmapflow-0.2.3rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1973 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-07 12:51:33.122643 openmapflow-0.2.3rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     3155 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/tests/test_CLI.py
--rw-r--r--   0 runner    (1001) docker     (116)     2386 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/tests/test_bbox.py
--rw-r--r--   0 runner    (1001) docker     (116)     2589 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (116)     6408 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/tests/test_ee_exporter.py
--rw-r--r--   0 runner    (1001) docker     (116)     3611 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/tests/test_engineer.py
--rw-r--r--   0 runner    (1001) docker     (116)    10037 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (116)     1353 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (116)    12788 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/tests/test_inference_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      780 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/tests/test_inference_widgets.py
--rw-r--r--   0 runner    (1001) docker     (116)     6989 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/tests/test_labeled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (116)      858 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/tests/test_raw_labels.py
--rw-r--r--   0 runner    (1001) docker     (116)      679 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/tests/test_torch_scriptability.py
--rw-r--r--   0 runner    (1001) docker     (116)     5276 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/tests/test_torchserve_handler.py
--rw-r--r--   0 runner    (1001) docker     (116)     2365 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/tests/test_train_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     1258 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/tests/test_trigger_inference_function.py
--rw-r--r--   0 runner    (1001) docker     (116)      513 2023-03-07 12:51:20.000000 openmapflow-0.2.3rc2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-23 20:56:35.016164 openmapflow-0.2.3rc3/
+-rw-r--r--   0 runner    (1001) docker     (116)    11314 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)    11535 2023-03-23 20:56:35.016164 openmapflow-0.2.3rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    11023 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-23 20:56:35.004164 openmapflow-0.2.3rc3/openmapflow/
+-rw-r--r--   0 runner    (1001) docker     (116)      909 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1932 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/bands.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3249 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3584 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1730 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/constants.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1060 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4982 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/ee_boundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12124 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/ee_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6125 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/engineer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-23 20:56:35.008164 openmapflow-0.2.3rc3/openmapflow/eo/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/eo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1833 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/eo/era5.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2766 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/eo/sentinel1.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6278 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/eo/sentinel2.py
+-rw-r--r--   0 runner    (1001) docker     (116)      386 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/eo/srtm.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8066 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/generate.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3153 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/inference.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7534 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/inference_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13719 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/inference_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2305 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/label_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    23211 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/labeled_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-23 20:56:35.008164 openmapflow-0.2.3rc3/openmapflow/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (116)     4703 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/notebooks/compare_ceo_labels.ipynb
+-rw-r--r--   0 runner    (1001) docker     (116)    15751 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/notebooks/create_map.ipynb
+-rw-r--r--   0 runner    (1001) docker     (116)     9416 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/notebooks/generate_project.ipynb
+-rw-r--r--   0 runner    (1001) docker     (116)     9907 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/notebooks/new_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (116)     5802 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/notebooks/train.ipynb
+-rw-r--r--   0 runner    (1001) docker     (116)    21519 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/notebooks/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (116)      608 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/pytorch_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-23 20:56:35.008164 openmapflow-0.2.3rc3/openmapflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (116)     3931 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/scripts/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (116)     2310 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/scripts/merging.sh
+-rw-r--r--   0 runner    (1001) docker     (116)     2730 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/scripts/openmapflow
+-rw-r--r--   0 runner    (1001) docker     (116)      295 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/scripts/torchserve_start.sh
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-23 20:56:35.012164 openmapflow-0.2.3rc3/openmapflow/templates/
+-rw-r--r--   0 runner    (1001) docker     (116)      685 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1615 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/templates/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3198 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/templates/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (116)      903 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/templates/github-deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     1240 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/templates/github-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     6632 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/templates/integration_test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2687 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/templates/integration_test_project.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2914 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/templates/integration_test_train_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (116)      389 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/templates/openmapflow-default.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)       32 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/templates/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     6631 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/templates/train.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5221 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/torchserve_handler.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2695 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/train_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-23 20:56:35.012164 openmapflow-0.2.3rc3/openmapflow/trigger_inference_function/
+-rw-r--r--   0 runner    (1001) docker     (116)     1177 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/trigger_inference_function/main.py
+-rw-r--r--   0 runner    (1001) docker     (116)        8 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/trigger_inference_function/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     2652 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/openmapflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-23 20:56:35.004164 openmapflow-0.2.3rc3/openmapflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    11535 2023-03-23 20:56:34.000000 openmapflow-0.2.3rc3/openmapflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2223 2023-03-23 20:56:34.000000 openmapflow-0.2.3rc3/openmapflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-23 20:56:34.000000 openmapflow-0.2.3rc3/openmapflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      265 2023-03-23 20:56:34.000000 openmapflow-0.2.3rc3/openmapflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       12 2023-03-23 20:56:34.000000 openmapflow-0.2.3rc3/openmapflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       30 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-23 20:56:35.016164 openmapflow-0.2.3rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1973 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-23 20:56:35.016164 openmapflow-0.2.3rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)     3155 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/tests/test_CLI.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2386 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/tests/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2589 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6408 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/tests/test_ee_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3611 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/tests/test_engineer.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10037 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1353 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12788 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/tests/test_inference_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      780 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/tests/test_inference_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6989 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/tests/test_labeled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (116)      858 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/tests/test_raw_labels.py
+-rw-r--r--   0 runner    (1001) docker     (116)      679 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/tests/test_torch_scriptability.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5276 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/tests/test_torchserve_handler.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2365 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/tests/test_train_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1258 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/tests/test_trigger_inference_function.py
+-rw-r--r--   0 runner    (1001) docker     (116)      513 2023-03-23 20:56:26.000000 openmapflow-0.2.3rc3/tests/test_utils.py
```

### Comparing `openmapflow-0.2.3rc2/LICENSE` & `openmapflow-0.2.3rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/PKG-INFO` & `openmapflow-0.2.3rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmapflow
-Version: 0.2.3rc2
+Version: 0.2.3rc3
 Summary: Creating maps with machine learning models and earth observation data.
 Home-page: https://github.com/nasaharvest/openmapflow
 Author: Ivan Zvonkov
 Author-email: izvonkov@umd.edu
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `openmapflow-0.2.3rc2/README.md` & `openmapflow-0.2.3rc3/README.md`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/Dockerfile` & `openmapflow-0.2.3rc3/openmapflow/Dockerfile`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/bands.py` & `openmapflow-0.2.3rc3/openmapflow/bands.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/bbox.py` & `openmapflow-0.2.3rc3/openmapflow/bbox.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/config.py` & `openmapflow-0.2.3rc3/openmapflow/config.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/constants.py` & `openmapflow-0.2.3rc3/openmapflow/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 TEMPLATE_DATASETS = TEMPLATES_DIR / "datasets.py"
 TEMPLATE_TRAIN = TEMPLATES_DIR / "train.py"
 TEMPLATE_EVALUATE = TEMPLATES_DIR / "evaluate.py"
 TEMPLATE_REQUIREMENTS = TEMPLATES_DIR / "requirements.txt"
 TEMPLATE_README = TEMPLATES_DIR / "README.md"
 TEMPLATE_DEPLOY_YML = TEMPLATES_DIR / "github-deploy.yaml"
 TEMPLATE_TEST_YML = TEMPLATES_DIR / "github-test.yaml"
-VERSION = "0.2.3rc2"
+VERSION = "0.2.3rc3"
 
 # -------------- Dataframe column names --------------------------------------
 SOURCE = "source"
 CLASS_PROB = "class_probability"
 START = "start_date"
 END = "end_date"
 LON = "lon"
```

### Comparing `openmapflow-0.2.3rc2/openmapflow/datasets.py` & `openmapflow-0.2.3rc3/openmapflow/datasets.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/ee_boundingbox.py` & `openmapflow-0.2.3rc3/openmapflow/ee_boundingbox.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/ee_exporter.py` & `openmapflow-0.2.3rc3/openmapflow/ee_exporter.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/engineer.py` & `openmapflow-0.2.3rc3/openmapflow/engineer.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/eo/era5.py` & `openmapflow-0.2.3rc3/openmapflow/eo/era5.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/eo/sentinel1.py` & `openmapflow-0.2.3rc3/openmapflow/eo/sentinel1.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/eo/sentinel2.py` & `openmapflow-0.2.3rc3/openmapflow/eo/sentinel2.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/generate.py` & `openmapflow-0.2.3rc3/openmapflow/generate.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/inference.py` & `openmapflow-0.2.3rc3/openmapflow/inference.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/inference_utils.py` & `openmapflow-0.2.3rc3/openmapflow/inference_utils.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/inference_widgets.py` & `openmapflow-0.2.3rc3/openmapflow/inference_widgets.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/label_utils.py` & `openmapflow-0.2.3rc3/openmapflow/label_utils.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/labeled_dataset.py` & `openmapflow-0.2.3rc3/openmapflow/labeled_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -383,28 +383,36 @@
             duplicates_index = clean_df.index[duplicates]
             df.loc[duplicates_index, EO_STATUS] = EO_STATUS_DUPLICATE
             df.loc[duplicates_index, EO_LAT] = None
             df.loc[duplicates_index, EO_LON] = None
             df.loc[duplicates_index, EO_FILE] = None
         return df
 
-    def load_df(self, check_eo_data: bool = True, to_np: bool = False) -> pd.DataFrame:
+    def load_df(
+        self,
+        check_eo_data: bool = True,
+        to_np: bool = False,
+        disable_tqdm: bool = False,
+    ) -> pd.DataFrame:
         """Load dataset (labels + earth observation data) as a DataFrame"""
         if not self.df_path.exists():
             print(self.create_dataset())
         df = pd.read_csv(self.df_path)
         df = df[clean_df_condition(df)].copy()
         if check_eo_data and df[EO_DATA].isnull().any():
             raise ValueError(
                 f"{self.name} has missing earth observation data, "
                 + "run openmapflow create-datasets"
             )
         if to_np:
-            tqdm.pandas(desc=self.name)
-            df[EO_DATA] = df[EO_DATA].progress_apply(str_to_np)
+            if disable_tqdm:
+                df[EO_DATA] = df[EO_DATA].apply(str_to_np)
+            else:
+                tqdm.pandas(desc=self.name)
+                df[EO_DATA] = df[EO_DATA].progress_apply(str_to_np)
         return df
 
     def _verify_and_standardize_df(self, df: pd.DataFrame) -> pd.DataFrame:
         print(f"Verifying labels: {self.name}")
         if not verify_df(df):
             raise ValueError("DataFrame is not valid, check the output above.")
```

### Comparing `openmapflow-0.2.3rc2/openmapflow/notebooks/compare_ceo_labels.ipynb` & `openmapflow-0.2.3rc3/openmapflow/notebooks/compare_ceo_labels.ipynb`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/notebooks/create_map.ipynb` & `openmapflow-0.2.3rc3/openmapflow/notebooks/create_map.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9905041152263374%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, '!pip install openmapflow[data]==0.2.3rc2 -q\\n')], "*

 * *            "delete: [1]}}, 5: {'source': {insert: [(24, 'print(PROJECT)\\n'), (25, "*

 * *            '\'os.environ["GCLOUD_PROJECT"] = GCLOUD_PROJECT_ID\')], delete: [24]}}, insert: [(2, '*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count', None), ('metadata', "*

 * *            "OrderedDict()), ('outputs', []), ('source', ['# Downgrade gdal \\n', '%%shell\\n', "*

 * *            "'yes | add-apt-repository pp […]*

```diff
@@ -17,22 +17,40 @@
             "execution_count": null,
             "metadata": {
                 "id": "fxgxmfAKpg6U"
             },
             "outputs": [],
             "source": [
                 "!pip install \"ipywidgets>=7,<8\" -q # https://github.com/googlecolab/colabtools/issues/3020\n",
-                "!pip install openmapflow[data]==0.2.1 -q\n",
+                "!pip install openmapflow[data]==0.2.3rc2 -q\n",
                 "!pip install cmocean ipyleaflet==0.16.0 pyyaml==5.4.1 -q # Colab likes this version\n",
                 "%env USE_AUTH_EPHEM=0"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Downgrade gdal \n",
+                "%%shell\n",
+                "yes | add-apt-repository ppa:ubuntugis/ppa\n",
+                "apt-get update\n",
+                "apt-get install python3-gdal=3.0.4+dfsg-1build3\n",
+                "apt-get install gdal-bin=3.0.4+dfsg-1build3\n",
+                "apt-get install libgdal-dev=3.0.4+dfsg-1build3\n",
+                "C_INCLUDE_PATH=/usr/include/gdal \n",
+                "CPLUS_INCLUDE_PATH=/usr/include/gdal \n",
+                "python -m pip install GDAL==3.0.4"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {
                 "id": "R9nTgKE1qU1a"
             },
             "outputs": [],
             "source": [
                 "import ipywidgets as widgets\n",
                 "config_yml_input = widgets.Textarea(placeholder=\"Your openmapflow.yaml\", layout=widgets.Layout(height=\"10em\", width=\"50%\"))\n",
@@ -79,15 +97,16 @@
                 "    find_missing_predictions, \n",
                 "    make_new_predictions, \n",
                 "    build_vrt,\n",
                 "    get_available_bboxes,\n",
                 "    get_available_models\n",
                 ")\n",
                 "warnings.simplefilter(action='ignore', category=FutureWarning)\n",
-                "print(PROJECT)"
+                "print(PROJECT)\n",
+                "os.environ[\"GCLOUD_PROJECT\"] = GCLOUD_PROJECT_ID"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "Ag1WM1J_Ch-w"
             },
@@ -312,14 +331,29 @@
             "source": [
                 "build_vrt(prefix)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Upgrade gdal to 3.3.2\n",
+                "%%shell\n",
+                "apt-get install gdal-bin\n",
+                "apt-get install libgdal-dev\n",
+                "C_INCLUDE_PATH=/usr/include/gdal \n",
+                "CPLUS_INCLUDE_PATH=/usr/include/gdal \n",
+                "python -m pip install GDAL==3.3.2"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {
                 "id": "alItdeCvrn4Y"
             },
             "outputs": [],
             "source": [
                 "# Translate vrt for all predictions into a tif file\n",
                 "!gdal_translate -a_srs EPSG:4326 -of GTiff {prefix}_final.vrt {prefix}_final.tif"
```

### Comparing `openmapflow-0.2.3rc2/openmapflow/notebooks/generate_project.ipynb` & `openmapflow-0.2.3rc3/openmapflow/notebooks/generate_project.ipynb`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/notebooks/new_data.ipynb` & `openmapflow-0.2.3rc3/openmapflow/notebooks/new_data.ipynb`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/notebooks/train.ipynb` & `openmapflow-0.2.3rc3/openmapflow/notebooks/train.ipynb`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/notebooks/tutorial.ipynb` & `openmapflow-0.2.3rc3/openmapflow/notebooks/tutorial.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9889504716981132%*

 * *Differences: {"'cells'": "{10: {'metadata': {replace: OrderedDict([('id', 'FhzRYzMNOiNV')])}}, 36: {'source': "*

 * *            "{insert: [(3, 'preds_dir.mkdir(exist_ok=True)')], delete: [11, 10, 9, 8, 7, 6, 5, 4, "*

 * *            "3]}}, 39: {'source': ['!gdalbuildvrt {tifs_dir}.vrt {tifs_dir}/*.tif\\n', "*

 * *            "'!gdal_translate -a_srs EPSG:4326 -of GTiff {tifs_dir}.vrt {tifs_dir}.tif']}, 40: "*

 * *            '{\'source\': {insert: [(6, \'eo_data = rio.open(f"{tifs_dir}.tif")\\n\')], delete: '*

 * *            "[6]}}, 42: {'sou […]*

```diff
@@ -123,14 +123,28 @@
                 "!pip install dvc[gs] cmocean pyyaml==5.4.1 -q"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
+                "id": "NGv4CE0zXLxj"
+            },
+            "outputs": [],
+            "source": [
+                "# Installing gdal\n",
+                "%%shell\n",
+                "yes | add-apt-repository ppa:ubuntugis/ppa && apt-get update -qq\n",
+                "apt-get install python3-gdal gdal-bin -y -q"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
                 "id": "ckKKdRZW-06Q"
             },
             "outputs": [],
             "source": [
                 "# CLI\n",
                 "!openmapflow"
             ]
@@ -145,15 +159,17 @@
                 "\n",
                 "<img src=\"https://storage.googleapis.com/harvest-public-assets/openmapflow/step1.png\" width=\"70%\"/>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "id": "FhzRYzMNOiNV"
+            },
             "outputs": [],
             "source": [
                 "# A Google Cloud Account is required to access the data\n",
                 "!gcloud auth application-default login"
             ]
         },
         {
@@ -504,23 +520,15 @@
                 "id": "TOSsu9Q3tiBX"
             },
             "outputs": [],
             "source": [
                 "tifs_dir = Path(f\"/content/tifs\")\n",
                 "preds_dir = Path(f\"/content/preds\")\n",
                 "tifs_dir.mkdir(exist_ok=True)\n",
-                "preds_dir.mkdir(exist_ok=True)\n",
-                "\n",
-                "def merge_tifs(full_prefix):\n",
-                "  vrt_in_file = f\"{full_prefix}*\"\n",
-                "  vrt_out_file = f\"{full_prefix}.vrt\"\n",
-                "  merged_file = f\"{full_prefix}.tif\"\n",
-                "  !gdalbuildvrt {vrt_out_file} {vrt_in_file}\n",
-                "  !gdal_translate -a_srs EPSG:4326 -of GTiff {vrt_out_file} {merged_file}\n",
-                "  return merged_file"
+                "preds_dir.mkdir(exist_ok=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "pd9Xtn_7xFUz"
             },
@@ -552,15 +560,16 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "1QNJ3jSRxgHn"
             },
             "outputs": [],
             "source": [
-                "merged_eo_file = merge_tifs(full_prefix=f\"{tifs_dir}/\")"
+                "!gdalbuildvrt {tifs_dir}.vrt {tifs_dir}/*.tif\n",
+                "!gdal_translate -a_srs EPSG:4326 -of GTiff {tifs_dir}.vrt {tifs_dir}.tif"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "4dRU1zyqxeUD"
@@ -569,15 +578,15 @@
             "source": [
                 "def normalize(array):\n",
                 "    array_min, array_max = array.min(), array.max()*0.5\n",
                 "    return ((array - array_min)/(array_max - array_min))\n",
                 "\n",
                 "month = 2\n",
                 "rgb_indexes = [DYNAMIC_BANDS.index(b) for b in [\"B4\", \"B3\", \"B2\"]]\n",
-                "eo_data = rio.open(merged_eo_file)\n",
+                "eo_data = rio.open(f\"{tifs_dir}.tif\")\n",
                 "colors = [eo_data.read(i + month*len(DYNAMIC_BANDS)) for i in rgb_indexes]\n",
                 "normalized_colors = [normalize(c) for c in colors]\n",
                 "rgb = np.dstack(normalized_colors)\n",
                 "plt.figure(figsize=(10,10))\n",
                 "plt.title(\"Earth Observation data for one month\")\n",
                 "plt.axis('off')\n",
                 "plt.imshow(rgb);"
@@ -603,16 +612,15 @@
                 "model = torch.jit.load(model_path_from_name(os.environ[\"MODEL_NAME\"]))\n",
                 "inference = Inference(model=model, normalizing_dict=None)\n",
                 "local_pred_paths = []\n",
                 "tifs = list(Path(tifs_dir).glob(\"*.tif\"))\n",
                 "for local_tif_path in tqdm(tifs, desc=\"Making predictions\"):\n",
                 "  local_pred_path = Path(f\"{preds_dir}/pred_{local_tif_path.stem}.nc\")\n",
                 "  inference.run(\n",
-                "      local_path=local_tif_path, \n",
-                "      start_date=date(2019, 2, 1), \n",
+                "      local_path=local_tif_path,  \n",
                 "      dest_path=local_pred_path\n",
                 "  )\n",
                 "  local_pred_paths.append(local_pred_path)"
             ]
         },
         {
             "cell_type": "markdown",
@@ -625,19 +633,32 @@
                 "<img src=\"https://storage.googleapis.com/harvest-public-assets/openmapflow/merging_predictions.png\" width=\"50%\"/>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "id": "NdPMyyP3MR_o"
+                "id": "XTb8nMmvUh3B"
+            },
+            "outputs": [],
+            "source": [
+                "!apt-get install python3-gdal=3.0.4+dfsg-1build3 gdal-bin=3.0.4+dfsg-1build3 libgdal-dev=3.0.4+dfsg-1build3 -qq\n",
+                "!gdalbuildvrt {preds_dir}.vrt {preds_dir}/*.nc"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "id": "CIEAiDJPVCg7"
             },
             "outputs": [],
             "source": [
-                "merged_pred_file = merge_tifs(full_prefix=f\"{preds_dir}/\")"
+                "!apt-get install python3-gdal gdal-bin libgdal-dev -qq\n",
+                "!gdal_translate -a_srs EPSG:4326 -of GTiff {preds_dir}.vrt {preds_dir}.tif"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "mL7Z3UdCxkSa"
             },
@@ -650,15 +671,15 @@
             "execution_count": null,
             "metadata": {
                 "id": "TlC_bZLrMT5y"
             },
             "outputs": [],
             "source": [
                 "# Visualize\n",
-                "predictions_map = rio.open(merged_pred_file)\n",
+                "predictions_map = rio.open(f\"{preds_dir}.tif\")\n",
                 "if \"maize\" in PROJECT:\n",
                 "  cmap = cmocean.cm.solar\n",
                 "elif \"crop\" in PROJECT:\n",
                 "  cmap = cmocean.cm.speed\n",
                 "else:\n",
                 "  cmap = cmocean.cm.thermal\n",
                 "\n",
@@ -727,15 +748,14 @@
                 "\n",
                 "<img src=\"https://storage.googleapis.com/harvest-public-assets/openmapflow/step3.png\" width=\"80%\"/>"
             ]
         }
     ],
     "metadata": {
         "colab": {
-            "collapsed_sections": [],
             "name": "tutorial.ipynb",
             "provenance": []
         },
         "kernelspec": {
             "display_name": "Python 3.9.12 ('venv': venv)",
             "language": "python",
             "name": "python3"
```

### Comparing `openmapflow-0.2.3rc2/openmapflow/pytorch_dataset.py` & `openmapflow-0.2.3rc3/openmapflow/pytorch_dataset.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/scripts/deploy.sh` & `openmapflow-0.2.3rc3/openmapflow/scripts/deploy.sh`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/scripts/merging.sh` & `openmapflow-0.2.3rc3/openmapflow/scripts/merging.sh`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/scripts/openmapflow` & `openmapflow-0.2.3rc3/openmapflow/scripts/openmapflow`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/templates/README.md` & `openmapflow-0.2.3rc3/openmapflow/templates/README.md`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/templates/datasets.py` & `openmapflow-0.2.3rc3/openmapflow/templates/datasets.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/templates/evaluate.py` & `openmapflow-0.2.3rc3/openmapflow/templates/evaluate.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/templates/github-deploy.yaml` & `openmapflow-0.2.3rc3/openmapflow/templates/github-deploy.yaml`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/templates/github-test.yaml` & `openmapflow-0.2.3rc3/openmapflow/templates/github-test.yaml`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/templates/integration_test_datasets.py` & `openmapflow-0.2.3rc3/openmapflow/templates/integration_test_datasets.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/templates/integration_test_project.py` & `openmapflow-0.2.3rc3/openmapflow/templates/integration_test_project.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/templates/integration_test_train_evaluate.py` & `openmapflow-0.2.3rc3/openmapflow/templates/integration_test_train_evaluate.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/templates/train.py` & `openmapflow-0.2.3rc3/openmapflow/templates/train.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/torchserve_handler.py` & `openmapflow-0.2.3rc3/openmapflow/torchserve_handler.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/train_utils.py` & `openmapflow-0.2.3rc3/openmapflow/train_utils.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/trigger_inference_function/main.py` & `openmapflow-0.2.3rc3/openmapflow/trigger_inference_function/main.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow/utils.py` & `openmapflow-0.2.3rc3/openmapflow/utils.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/openmapflow.egg-info/PKG-INFO` & `openmapflow-0.2.3rc3/openmapflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmapflow
-Version: 0.2.3rc2
+Version: 0.2.3rc3
 Summary: Creating maps with machine learning models and earth observation data.
 Home-page: https://github.com/nasaharvest/openmapflow
 Author: Ivan Zvonkov
 Author-email: izvonkov@umd.edu
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `openmapflow-0.2.3rc2/openmapflow.egg-info/SOURCES.txt` & `openmapflow-0.2.3rc3/openmapflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/setup.py` & `openmapflow-0.2.3rc3/setup.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/tests/test_CLI.py` & `openmapflow-0.2.3rc3/tests/test_CLI.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/tests/test_bbox.py` & `openmapflow-0.2.3rc3/tests/test_bbox.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/tests/test_config.py` & `openmapflow-0.2.3rc3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/tests/test_ee_exporter.py` & `openmapflow-0.2.3rc3/tests/test_ee_exporter.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/tests/test_engineer.py` & `openmapflow-0.2.3rc3/tests/test_engineer.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/tests/test_generate.py` & `openmapflow-0.2.3rc3/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/tests/test_inference.py` & `openmapflow-0.2.3rc3/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/tests/test_inference_utils.py` & `openmapflow-0.2.3rc3/tests/test_inference_utils.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/tests/test_inference_widgets.py` & `openmapflow-0.2.3rc3/tests/test_inference_widgets.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/tests/test_labeled_dataset.py` & `openmapflow-0.2.3rc3/tests/test_labeled_dataset.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/tests/test_raw_labels.py` & `openmapflow-0.2.3rc3/tests/test_raw_labels.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/tests/test_torch_scriptability.py` & `openmapflow-0.2.3rc3/tests/test_torch_scriptability.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/tests/test_torchserve_handler.py` & `openmapflow-0.2.3rc3/tests/test_torchserve_handler.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/tests/test_train_utils.py` & `openmapflow-0.2.3rc3/tests/test_train_utils.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/tests/test_trigger_inference_function.py` & `openmapflow-0.2.3rc3/tests/test_trigger_inference_function.py`

 * *Files identical despite different names*

### Comparing `openmapflow-0.2.3rc2/tests/test_utils.py` & `openmapflow-0.2.3rc3/tests/test_utils.py`

 * *Files identical despite different names*

