# Comparing `tmp/NiaAML-1.1.7.tar.gz` & `tmp/NiaAML-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NiaAML-1.1.7.tar", max compression
+gzip compressed data, was "NiaAML-1.1.9.tar", max compression
```

## Comparing `NiaAML-1.1.7.tar` & `NiaAML-1.1.9.tar`

### file list

```diff
@@ -1,92 +1,68 @@
--rw-r--r--   0        0        0    12021 2022-02-21 19:07:43.770881 NiaAML-1.1.7/CHANGELOG.md
--rw-r--r--   0        0        0      395 2021-06-27 13:20:39.526154 NiaAML-1.1.7/CITATION.md
--rw-r--r--   0        0        0     1069 2021-06-27 13:20:39.529269 NiaAML-1.1.7/LICENSE
--rw-r--r--   0        0        0      819 2022-02-21 19:07:43.779951 NiaAML-1.1.7/niaaml/__init__.py
--rw-r--r--   0        0        0     1119 2021-06-27 13:20:39.559713 NiaAML-1.1.7/niaaml/classifiers/__init__.py
--rw-r--r--   0        0        0     3039 2021-06-27 13:20:39.560213 NiaAML-1.1.7/niaaml/classifiers/ada_boost.py
--rw-r--r--   0        0        0     3124 2021-06-27 13:20:39.560856 NiaAML-1.1.7/niaaml/classifiers/bagging.py
--rw-r--r--   0        0        0      894 2021-06-27 13:20:39.561008 NiaAML-1.1.7/niaaml/classifiers/classifier.py
--rw-r--r--   0        0        0     3169 2021-06-27 13:20:39.561750 NiaAML-1.1.7/niaaml/classifiers/decision_tree.py
--rw-r--r--   0        0        0     3165 2021-06-27 13:20:39.562204 NiaAML-1.1.7/niaaml/classifiers/extremely_randomized_trees.py
--rw-r--r--   0        0        0     2819 2021-06-27 13:20:39.562702 NiaAML-1.1.7/niaaml/classifiers/gaussian_naive_bayes.py
--rw-r--r--   0        0        0     3294 2021-06-27 13:20:39.563039 NiaAML-1.1.7/niaaml/classifiers/gaussian_process.py
--rw-r--r--   0        0        0     3124 2021-06-27 13:20:39.563039 NiaAML-1.1.7/niaaml/classifiers/k_neighbors.py
--rw-r--r--   0        0        0     3116 2021-06-27 13:20:39.563805 NiaAML-1.1.7/niaaml/classifiers/linear_svc.py
--rw-r--r--   0        0        0     3317 2021-06-27 13:20:39.564304 NiaAML-1.1.7/niaaml/classifiers/multi_layer_perceptron.py
--rw-r--r--   0        0        0     3024 2021-06-27 13:20:39.564304 NiaAML-1.1.7/niaaml/classifiers/quadratic_driscriminant_analysis.py
--rw-r--r--   0        0        0     3112 2021-06-27 13:20:39.564805 NiaAML-1.1.7/niaaml/classifiers/random_forest.py
--rw-r--r--   0        0        0     1761 2021-06-27 13:20:39.565805 NiaAML-1.1.7/niaaml/classifiers/utility.py
--rw-r--r--   0        0        0      221 2021-06-27 13:20:39.566308 NiaAML-1.1.7/niaaml/data/__init__.py
--rw-r--r--   0        0        0      743 2021-06-27 13:20:39.566806 NiaAML-1.1.7/niaaml/data/basic_data_reader.py
--rw-r--r--   0        0        0     1460 2021-06-27 13:20:39.567360 NiaAML-1.1.7/niaaml/data/csv_data_reader.py
--rw-r--r--   0        0        0     1391 2021-06-27 13:20:39.567855 NiaAML-1.1.7/niaaml/data/data_reader.py
--rw-r--r--   0        0        0      406 2021-06-27 13:20:39.568387 NiaAML-1.1.7/niaaml/fitness/__init__.py
--rw-r--r--   0        0        0      977 2021-06-27 13:20:39.568889 NiaAML-1.1.7/niaaml/fitness/accuracy.py
--rw-r--r--   0        0        0     1000 2021-06-27 13:20:39.569492 NiaAML-1.1.7/niaaml/fitness/cohen_kappa.py
--rw-r--r--   0        0        0      966 2021-06-27 13:20:39.569492 NiaAML-1.1.7/niaaml/fitness/f1.py
--rw-r--r--   0        0        0      952 2021-06-27 13:20:39.570028 NiaAML-1.1.7/niaaml/fitness/fitness_function.py
--rw-r--r--   0        0        0     1004 2021-06-27 13:20:39.570527 NiaAML-1.1.7/niaaml/fitness/precision.py
--rw-r--r--   0        0        0      762 2021-06-27 13:20:39.570527 NiaAML-1.1.7/niaaml/fitness/utility.py
--rw-r--r--   0        0        0     1451 2021-06-27 13:20:39.570527 NiaAML-1.1.7/niaaml/logger.py
--rw-r--r--   0        0        0    21985 2022-02-21 07:18:40.715112 NiaAML-1.1.7/niaaml/pipeline.py
--rw-r--r--   0        0        0     1903 2021-06-27 13:20:39.572575 NiaAML-1.1.7/niaaml/pipeline_component.py
--rw-r--r--   0        0        0    21156 2021-06-27 13:20:39.572938 NiaAML-1.1.7/niaaml/pipeline_optimizer.py
--rw-r--r--   0        0        0      397 2021-06-27 13:20:39.572938 NiaAML-1.1.7/niaaml/preprocessing/__init__.py
--rw-r--r--   0        0        0      403 2021-06-27 13:20:39.574141 NiaAML-1.1.7/niaaml/preprocessing/encoding/__init__.py
--rw-r--r--   0        0        0     1097 2021-06-27 13:20:39.574332 NiaAML-1.1.7/niaaml/preprocessing/encoding/feature_encoder.py
--rw-r--r--   0        0        0     1745 2021-06-27 13:20:39.574888 NiaAML-1.1.7/niaaml/preprocessing/encoding/one_hot_encoder.py
--rw-r--r--   0        0        0     1667 2021-06-27 13:20:39.575017 NiaAML-1.1.7/niaaml/preprocessing/encoding/utility.py
--rw-r--r--   0        0        0     1369 2021-06-27 13:20:39.575521 NiaAML-1.1.7/niaaml/preprocessing/feature_selection/__init__.py
--rw-r--r--   0        0        0     2022 2021-06-27 13:20:39.576108 NiaAML-1.1.7/niaaml/preprocessing/feature_selection/_feature_selection_threshold_problem.py
--rw-r--r--   0        0        0     3345 2021-06-27 13:20:39.576108 NiaAML-1.1.7/niaaml/preprocessing/feature_selection/bat_algorithm.py
--rw-r--r--   0        0        0     3229 2021-06-27 13:20:39.577149 NiaAML-1.1.7/niaaml/preprocessing/feature_selection/differential_evolution.py
--rw-r--r--   0        0        0      805 2021-06-27 13:20:39.577149 NiaAML-1.1.7/niaaml/preprocessing/feature_selection/feature_selection_algorithm.py
--rw-r--r--   0        0        0     2787 2021-06-27 13:20:39.578070 NiaAML-1.1.7/niaaml/preprocessing/feature_selection/grey_wolf_optimizer.py
--rw-r--r--   0        0        0     2963 2021-06-27 13:20:39.578282 NiaAML-1.1.7/niaaml/preprocessing/feature_selection/jDEFSTH.py
--rw-r--r--   0        0        0     3219 2021-06-27 13:20:39.578798 NiaAML-1.1.7/niaaml/preprocessing/feature_selection/particle_swarm_optimization.py
--rw-r--r--   0        0        0     2608 2022-02-21 07:18:40.715650 NiaAML-1.1.7/niaaml/preprocessing/feature_selection/select_k_best.py
--rw-r--r--   0        0        0     2216 2021-06-27 13:20:39.580085 NiaAML-1.1.7/niaaml/preprocessing/feature_selection/select_percentile.py
--rw-r--r--   0        0        0     1639 2021-06-27 13:20:39.580550 NiaAML-1.1.7/niaaml/preprocessing/feature_selection/utility.py
--rw-r--r--   0        0        0     1994 2022-02-21 07:18:40.717025 NiaAML-1.1.7/niaaml/preprocessing/feature_selection/variance_threshold.py
--rw-r--r--   0        0        0      823 2021-06-27 13:20:39.581581 NiaAML-1.1.7/niaaml/preprocessing/feature_transform/__init__.py
--rw-r--r--   0        0        0      930 2021-06-27 13:20:39.581845 NiaAML-1.1.7/niaaml/preprocessing/feature_transform/feature_transform_algorithm.py
--rw-r--r--   0        0        0     1762 2021-06-27 13:20:39.582845 NiaAML-1.1.7/niaaml/preprocessing/feature_transform/max_abs_scaler.py
--rw-r--r--   0        0        0     1944 2021-06-27 13:20:39.583213 NiaAML-1.1.7/niaaml/preprocessing/feature_transform/normalizer.py
--rw-r--r--   0        0        0     1916 2021-06-27 13:20:39.583706 NiaAML-1.1.7/niaaml/preprocessing/feature_transform/quantile_transformer.py
--rw-r--r--   0        0        0     1885 2021-06-27 13:20:39.584206 NiaAML-1.1.7/niaaml/preprocessing/feature_transform/robust_scaler.py
--rw-r--r--   0        0        0     1716 2021-06-27 13:20:39.584270 NiaAML-1.1.7/niaaml/preprocessing/feature_transform/standard_scaler.py
--rw-r--r--   0        0        0     1117 2021-06-27 13:20:39.584763 NiaAML-1.1.7/niaaml/preprocessing/feature_transform/utility.py
--rw-r--r--   0        0        0      345 2021-06-27 13:20:39.584763 NiaAML-1.1.7/niaaml/preprocessing/imputation/__init__.py
--rw-r--r--   0        0        0     1023 2021-06-27 13:20:39.585788 NiaAML-1.1.7/niaaml/preprocessing/imputation/imputer.py
--rw-r--r--   0        0        0     1788 2021-06-27 13:20:39.586041 NiaAML-1.1.7/niaaml/preprocessing/imputation/simple_imputer.py
--rw-r--r--   0        0        0     1342 2021-06-27 13:20:39.586539 NiaAML-1.1.7/niaaml/preprocessing/imputation/utility.py
--rw-r--r--   0        0        0      372 2021-06-27 13:20:39.586684 NiaAML-1.1.7/niaaml/preprocessing/preprocessing_algorithm.py
--rw-r--r--   0        0        0        0 2021-06-27 13:20:39.587099 NiaAML-1.1.7/niaaml/tests/__init__.py
--rw-r--r--   0        0        0      146 2021-06-27 13:20:39.587305 NiaAML-1.1.7/niaaml/tests/conftest.py
--rw-r--r--   0        0        0      919 2021-06-27 13:20:39.587805 NiaAML-1.1.7/niaaml/tests/test_basic_data_reader.py
--rw-r--r--   0        0        0      843 2021-06-27 13:20:39.587960 NiaAML-1.1.7/niaaml/tests/test_classifier_factory.py
--rw-r--r--   0        0        0     3197 2021-06-27 13:20:39.588573 NiaAML-1.1.7/niaaml/tests/test_classifiers.py
--rw-r--r--   0        0        0     1816 2021-06-27 13:20:39.588710 NiaAML-1.1.7/niaaml/tests/test_csv_data_reader.py
--rw-r--r--   0        0        0      853 2021-06-27 13:20:39.589182 NiaAML-1.1.7/niaaml/tests/test_encoder_factory.py
--rw-r--r--   0        0        0     1622 2021-06-27 13:20:39.589330 NiaAML-1.1.7/niaaml/tests/test_feature_encoder.py
--rw-r--r--   0        0        0     2656 2021-06-27 13:20:39.589794 NiaAML-1.1.7/niaaml/tests/test_feature_selection.py
--rw-r--r--   0        0        0      951 2021-06-27 13:20:39.589952 NiaAML-1.1.7/niaaml/tests/test_feature_selection_algorithm_factory.py
--rw-r--r--   0        0        0     1607 2021-06-27 13:20:39.590419 NiaAML-1.1.7/niaaml/tests/test_feature_transform.py
--rw-r--r--   0        0        0      951 2021-06-27 13:20:39.590574 NiaAML-1.1.7/niaaml/tests/test_feature_transform_algorithm_factory.py
--rw-r--r--   0        0        0     2014 2021-06-27 13:20:39.591032 NiaAML-1.1.7/niaaml/tests/test_fitness.py
--rw-r--r--   0        0        0      840 2021-06-27 13:20:39.591179 NiaAML-1.1.7/niaaml/tests/test_fitness_factory.py
--rw-r--r--   0        0        0     1627 2021-06-27 13:20:39.591628 NiaAML-1.1.7/niaaml/tests/test_imputer.py
--rw-r--r--   0        0        0      841 2021-06-27 13:20:39.591793 NiaAML-1.1.7/niaaml/tests/test_imputer_factory.py
--rw-r--r--   0        0        0     6532 2021-06-27 13:20:39.592243 NiaAML-1.1.7/niaaml/tests/test_pipeline.py
--rw-r--r--   0        0        0     5394 2021-06-27 13:20:39.592413 NiaAML-1.1.7/niaaml/tests/test_pipeline_optimizer.py
--rw-r--r--   0        0        0     2722 2021-06-27 13:20:39.593082 NiaAML-1.1.7/niaaml/tests/test_utilities.py
--rw-r--r--   0        0        0     7949 2021-06-27 13:20:39.593082 NiaAML-1.1.7/niaaml/tests/tests_files/dataset_header_classes.csv
--rw-r--r--   0        0        0     8082 2021-06-27 13:20:39.593082 NiaAML-1.1.7/niaaml/tests/tests_files/dataset_header_classes_cat_miss.csv
--rw-r--r--   0        0        0     7146 2021-06-27 13:20:39.594127 NiaAML-1.1.7/niaaml/tests/tests_files/dataset_header_no_classes.csv
--rw-r--r--   0        0        0    11862 2021-06-27 13:20:39.594127 NiaAML-1.1.7/niaaml/tests/tests_files/dataset_no_header_classes.csv
--rw-r--r--   0        0        0     7128 2021-06-27 13:20:39.594127 NiaAML-1.1.7/niaaml/tests/tests_files/dataset_no_header_no_classes.csv
--rw-r--r--   0        0        0     4808 2022-02-21 07:18:40.717852 NiaAML-1.1.7/niaaml/utilities.py
--rw-r--r--   0        0        0      972 2022-02-21 19:07:43.782316 NiaAML-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     5255 2021-11-07 19:07:01.488134 NiaAML-1.1.7/README.rst
--rw-r--r--   0        0        0     6450 2022-02-21 19:08:14.650379 NiaAML-1.1.7/setup.py
--rw-r--r--   0        0        0     6126 2022-02-21 19:08:14.651398 NiaAML-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0    13648 2022-06-08 20:04:11.698646 NiaAML-1.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0      395 2021-06-27 13:20:39.526154 NiaAML-1.1.9/CITATION.md
+-rw-r--r--   0        0        0     1069 2021-06-27 13:20:39.529269 NiaAML-1.1.9/LICENSE
+-rw-r--r--   0        0        0      819 2022-06-08 20:04:11.705752 NiaAML-1.1.9/niaaml/__init__.py
+-rw-r--r--   0        0        0     1119 2021-06-27 13:20:39.559713 NiaAML-1.1.9/niaaml/classifiers/__init__.py
+-rw-r--r--   0        0        0     2829 2022-06-08 20:04:11.706665 NiaAML-1.1.9/niaaml/classifiers/ada_boost.py
+-rw-r--r--   0        0        0     2914 2022-06-08 20:04:11.707548 NiaAML-1.1.9/niaaml/classifiers/bagging.py
+-rw-r--r--   0        0        0      894 2021-06-27 13:20:39.561008 NiaAML-1.1.9/niaaml/classifiers/classifier.py
+-rw-r--r--   0        0        0     2959 2022-06-08 20:04:11.707855 NiaAML-1.1.9/niaaml/classifiers/decision_tree.py
+-rw-r--r--   0        0        0     2955 2022-06-08 20:04:11.707855 NiaAML-1.1.9/niaaml/classifiers/extremely_randomized_trees.py
+-rw-r--r--   0        0        0     2609 2022-06-08 20:04:11.707855 NiaAML-1.1.9/niaaml/classifiers/gaussian_naive_bayes.py
+-rw-r--r--   0        0        0     3084 2022-06-08 20:04:11.707855 NiaAML-1.1.9/niaaml/classifiers/gaussian_process.py
+-rw-r--r--   0        0        0     2914 2022-06-08 20:04:11.707855 NiaAML-1.1.9/niaaml/classifiers/k_neighbors.py
+-rw-r--r--   0        0        0     2906 2022-06-08 20:04:11.707855 NiaAML-1.1.9/niaaml/classifiers/linear_svc.py
+-rw-r--r--   0        0        0     3107 2022-06-08 20:04:11.707855 NiaAML-1.1.9/niaaml/classifiers/multi_layer_perceptron.py
+-rw-r--r--   0        0        0     2814 2022-06-08 20:04:11.707855 NiaAML-1.1.9/niaaml/classifiers/quadratic_driscriminant_analysis.py
+-rw-r--r--   0        0        0     2902 2022-06-08 20:04:11.707855 NiaAML-1.1.9/niaaml/classifiers/random_forest.py
+-rw-r--r--   0        0        0     1761 2021-06-27 13:20:39.565805 NiaAML-1.1.9/niaaml/classifiers/utility.py
+-rw-r--r--   0        0        0      221 2021-06-27 13:20:39.566308 NiaAML-1.1.9/niaaml/data/__init__.py
+-rw-r--r--   0        0        0      743 2021-06-27 13:20:39.566806 NiaAML-1.1.9/niaaml/data/basic_data_reader.py
+-rw-r--r--   0        0        0     1460 2021-06-27 13:20:39.567360 NiaAML-1.1.9/niaaml/data/csv_data_reader.py
+-rw-r--r--   0        0        0     1391 2021-06-27 13:20:39.567855 NiaAML-1.1.9/niaaml/data/data_reader.py
+-rw-r--r--   0        0        0      406 2021-06-27 13:20:39.568387 NiaAML-1.1.9/niaaml/fitness/__init__.py
+-rw-r--r--   0        0        0      977 2021-06-27 13:20:39.568889 NiaAML-1.1.9/niaaml/fitness/accuracy.py
+-rw-r--r--   0        0        0     1000 2021-06-27 13:20:39.569492 NiaAML-1.1.9/niaaml/fitness/cohen_kappa.py
+-rw-r--r--   0        0        0      966 2021-06-27 13:20:39.569492 NiaAML-1.1.9/niaaml/fitness/f1.py
+-rw-r--r--   0        0        0      952 2021-06-27 13:20:39.570028 NiaAML-1.1.9/niaaml/fitness/fitness_function.py
+-rw-r--r--   0        0        0     1004 2021-06-27 13:20:39.570527 NiaAML-1.1.9/niaaml/fitness/precision.py
+-rw-r--r--   0        0        0      762 2021-06-27 13:20:39.570527 NiaAML-1.1.9/niaaml/fitness/utility.py
+-rw-r--r--   0        0        0     1451 2021-06-27 13:20:39.570527 NiaAML-1.1.9/niaaml/logger.py
+-rw-r--r--   0        0        0    21985 2022-02-21 07:18:40.715112 NiaAML-1.1.9/niaaml/pipeline.py
+-rw-r--r--   0        0        0     1903 2021-06-27 13:20:39.572575 NiaAML-1.1.9/niaaml/pipeline_component.py
+-rw-r--r--   0        0        0    21156 2021-06-27 13:20:39.572938 NiaAML-1.1.9/niaaml/pipeline_optimizer.py
+-rw-r--r--   0        0        0      397 2021-06-27 13:20:39.572938 NiaAML-1.1.9/niaaml/preprocessing/__init__.py
+-rw-r--r--   0        0        0      403 2021-06-27 13:20:39.574141 NiaAML-1.1.9/niaaml/preprocessing/encoding/__init__.py
+-rw-r--r--   0        0        0     1097 2021-06-27 13:20:39.574332 NiaAML-1.1.9/niaaml/preprocessing/encoding/feature_encoder.py
+-rw-r--r--   0        0        0     1745 2021-06-27 13:20:39.574888 NiaAML-1.1.9/niaaml/preprocessing/encoding/one_hot_encoder.py
+-rw-r--r--   0        0        0     1667 2021-06-27 13:20:39.575017 NiaAML-1.1.9/niaaml/preprocessing/encoding/utility.py
+-rw-r--r--   0        0        0     1369 2021-06-27 13:20:39.575521 NiaAML-1.1.9/niaaml/preprocessing/feature_selection/__init__.py
+-rw-r--r--   0        0        0     2022 2021-06-27 13:20:39.576108 NiaAML-1.1.9/niaaml/preprocessing/feature_selection/_feature_selection_threshold_problem.py
+-rw-r--r--   0        0        0     3345 2021-06-27 13:20:39.576108 NiaAML-1.1.9/niaaml/preprocessing/feature_selection/bat_algorithm.py
+-rw-r--r--   0        0        0     3229 2021-06-27 13:20:39.577149 NiaAML-1.1.9/niaaml/preprocessing/feature_selection/differential_evolution.py
+-rw-r--r--   0        0        0      805 2021-06-27 13:20:39.577149 NiaAML-1.1.9/niaaml/preprocessing/feature_selection/feature_selection_algorithm.py
+-rw-r--r--   0        0        0     2787 2021-06-27 13:20:39.578070 NiaAML-1.1.9/niaaml/preprocessing/feature_selection/grey_wolf_optimizer.py
+-rw-r--r--   0        0        0     2963 2021-06-27 13:20:39.578282 NiaAML-1.1.9/niaaml/preprocessing/feature_selection/jDEFSTH.py
+-rw-r--r--   0        0        0     3219 2021-06-27 13:20:39.578798 NiaAML-1.1.9/niaaml/preprocessing/feature_selection/particle_swarm_optimization.py
+-rw-r--r--   0        0        0     2608 2022-02-21 07:18:40.715650 NiaAML-1.1.9/niaaml/preprocessing/feature_selection/select_k_best.py
+-rw-r--r--   0        0        0     2216 2021-06-27 13:20:39.580085 NiaAML-1.1.9/niaaml/preprocessing/feature_selection/select_percentile.py
+-rw-r--r--   0        0        0     1639 2021-06-27 13:20:39.580550 NiaAML-1.1.9/niaaml/preprocessing/feature_selection/utility.py
+-rw-r--r--   0        0        0     1994 2022-02-21 07:18:40.717025 NiaAML-1.1.9/niaaml/preprocessing/feature_selection/variance_threshold.py
+-rw-r--r--   0        0        0      823 2021-06-27 13:20:39.581581 NiaAML-1.1.9/niaaml/preprocessing/feature_transform/__init__.py
+-rw-r--r--   0        0        0      930 2021-06-27 13:20:39.581845 NiaAML-1.1.9/niaaml/preprocessing/feature_transform/feature_transform_algorithm.py
+-rw-r--r--   0        0        0     1762 2021-06-27 13:20:39.582845 NiaAML-1.1.9/niaaml/preprocessing/feature_transform/max_abs_scaler.py
+-rw-r--r--   0        0        0     1944 2021-06-27 13:20:39.583213 NiaAML-1.1.9/niaaml/preprocessing/feature_transform/normalizer.py
+-rw-r--r--   0        0        0     1916 2021-06-27 13:20:39.583706 NiaAML-1.1.9/niaaml/preprocessing/feature_transform/quantile_transformer.py
+-rw-r--r--   0        0        0     1885 2021-06-27 13:20:39.584206 NiaAML-1.1.9/niaaml/preprocessing/feature_transform/robust_scaler.py
+-rw-r--r--   0        0        0     1716 2021-06-27 13:20:39.584270 NiaAML-1.1.9/niaaml/preprocessing/feature_transform/standard_scaler.py
+-rw-r--r--   0        0        0     1117 2021-06-27 13:20:39.584763 NiaAML-1.1.9/niaaml/preprocessing/feature_transform/utility.py
+-rw-r--r--   0        0        0      345 2021-06-27 13:20:39.584763 NiaAML-1.1.9/niaaml/preprocessing/imputation/__init__.py
+-rw-r--r--   0        0        0     1023 2021-06-27 13:20:39.585788 NiaAML-1.1.9/niaaml/preprocessing/imputation/imputer.py
+-rw-r--r--   0        0        0     1788 2021-06-27 13:20:39.586041 NiaAML-1.1.9/niaaml/preprocessing/imputation/simple_imputer.py
+-rw-r--r--   0        0        0     1342 2021-06-27 13:20:39.586539 NiaAML-1.1.9/niaaml/preprocessing/imputation/utility.py
+-rw-r--r--   0        0        0      372 2021-06-27 13:20:39.586684 NiaAML-1.1.9/niaaml/preprocessing/preprocessing_algorithm.py
+-rw-r--r--   0        0        0     4808 2022-02-21 07:18:40.717852 NiaAML-1.1.9/niaaml/utilities.py
+-rw-r--r--   0        0        0      972 2022-06-08 20:04:11.707855 NiaAML-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5268 2022-06-08 20:04:11.699491 NiaAML-1.1.9/README.rst
+-rw-r--r--   0        0        0     6411 2022-06-08 20:04:23.698436 NiaAML-1.1.9/setup.py
+-rw-r--r--   0        0        0     6139 2022-06-08 20:04:23.698436 NiaAML-1.1.9/PKG-INFO
```

### Comparing `NiaAML-1.1.7/CHANGELOG.md` & `NiaAML-1.1.9/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,38 @@
 # Changelog
 
-## [1.1.7](https://github.com/lukapecnik/niaaml/tree/1.1.7) (2022-02-21)
+## [1.1.9](https://github.com/lukapecnik/NiaAML/tree/1.1.9) (2022-05-25)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/1.1.6...1.1.7)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/1.1.8...1.1.9)
+
+**Closed issues:**
+
+- Test with python-scikit-learn 1.1.0 is not passing [\#71](https://github.com/lukapecnik/NiaAML/issues/71)
+
+**Merged pull requests:**
+
+- Bump version [\#75](https://github.com/lukapecnik/NiaAML/pull/75) ([firefly-cpp](https://github.com/firefly-cpp))
+- Do not package the tests [\#74](https://github.com/lukapecnik/NiaAML/pull/74) ([firefly-cpp](https://github.com/firefly-cpp))
+
+## [1.1.8](https://github.com/lukapecnik/NiaAML/tree/1.1.8) (2022-05-24)
+
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/1.1.7...1.1.8)
+
+**Merged pull requests:**
+
+- Removed deprecated sklearn warnings [\#72](https://github.com/lukapecnik/NiaAML/pull/72) ([zStupan](https://github.com/zStupan))
+- Update README.md [\#70](https://github.com/lukapecnik/NiaAML/pull/70) ([firefly-cpp](https://github.com/firefly-cpp))
+- Run tests with github action [\#68](https://github.com/lukapecnik/NiaAML/pull/68) ([lukapecnik](https://github.com/lukapecnik))
+- docs: add lukapecnik as a contributor for infra [\#67](https://github.com/lukapecnik/NiaAML/pull/67) ([allcontributors[bot]](https://github.com/apps/allcontributors))
+- docs: add musicinmybrain as a contributor for code, infra [\#66](https://github.com/lukapecnik/NiaAML/pull/66) ([allcontributors[bot]](https://github.com/apps/allcontributors))
+- docs: add zStupan as a contributor for code [\#65](https://github.com/lukapecnik/NiaAML/pull/65) ([allcontributors[bot]](https://github.com/apps/allcontributors))
+
+## [1.1.7](https://github.com/lukapecnik/NiaAML/tree/1.1.7) (2022-02-21)
+
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/1.1.6...1.1.7)
 
 **Closed issues:**
 
 - Update to the latest niapy stable release [\#62](https://github.com/lukapecnik/NiaAML/issues/62)
 - Example file pipeline.ppln is out of date [\#60](https://github.com/lukapecnik/NiaAML/issues/60)
 - np.int is a deprecated alias [\#56](https://github.com/lukapecnik/NiaAML/issues/56)
 - Remove setup.py file [\#54](https://github.com/lukapecnik/NiaAML/issues/54)
@@ -18,177 +44,177 @@
 - Eschew deprecated numpy aliases for builtins [\#61](https://github.com/lukapecnik/NiaAML/pull/61) ([musicinmybrain](https://github.com/musicinmybrain))
 - Corrected dependencies in CONTRIBUTING [\#59](https://github.com/lukapecnik/NiaAML/pull/59) ([firefly-cpp](https://github.com/firefly-cpp))
 - Do not install text files in site-packages/ [\#58](https://github.com/lukapecnik/NiaAML/pull/58) ([musicinmybrain](https://github.com/musicinmybrain))
 - Use the latest upstream's release for niapy [\#57](https://github.com/lukapecnik/NiaAML/pull/57) ([firefly-cpp](https://github.com/firefly-cpp))
 - Add reference links [\#55](https://github.com/lukapecnik/NiaAML/pull/55) ([firefly-cpp](https://github.com/firefly-cpp))
 - Add link to the API [\#53](https://github.com/lukapecnik/NiaAML/pull/53) ([firefly-cpp](https://github.com/firefly-cpp))
 
-## [1.1.6](https://github.com/lukapecnik/niaaml/tree/1.1.6) (2021-06-27)
+## [1.1.6](https://github.com/lukapecnik/NiaAML/tree/1.1.6) (2021-06-27)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/1.1.5...1.1.6)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/1.1.5...1.1.6)
 
 **Closed issues:**
 
 - Upgrade to the latest niapy release [\#51](https://github.com/lukapecnik/NiaAML/issues/51)
 
 **Merged pull requests:**
 
 - Update to the latest niapy version and fix docs build warnings [\#52](https://github.com/lukapecnik/NiaAML/pull/52) ([zStupan](https://github.com/zStupan))
 
-## [1.1.5](https://github.com/lukapecnik/niaaml/tree/1.1.5) (2021-06-01)
+## [1.1.5](https://github.com/lukapecnik/NiaAML/tree/1.1.5) (2021-06-01)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/1.1.4...1.1.5)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/1.1.4...1.1.5)
 
 **Merged pull requests:**
 
 - Citation details [\#50](https://github.com/lukapecnik/NiaAML/pull/50) ([firefly-cpp](https://github.com/firefly-cpp))
 
-## [1.1.4](https://github.com/lukapecnik/niaaml/tree/1.1.4) (2021-05-24)
+## [1.1.4](https://github.com/lukapecnik/NiaAML/tree/1.1.4) (2021-05-24)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/1.1.3...1.1.4)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/1.1.3...1.1.4)
 
 **Closed issues:**
 
 - Unable to install with conda [\#47](https://github.com/lukapecnik/NiaAML/issues/47)
 
-## [1.1.3](https://github.com/lukapecnik/niaaml/tree/1.1.3) (2021-05-23)
+## [1.1.3](https://github.com/lukapecnik/NiaAML/tree/1.1.3) (2021-05-23)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/1.1.2...1.1.3)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/1.1.2...1.1.3)
 
-## [1.1.2](https://github.com/lukapecnik/niaaml/tree/1.1.2) (2021-05-19)
+## [1.1.2](https://github.com/lukapecnik/NiaAML/tree/1.1.2) (2021-05-19)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/1.1.1...1.1.2)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/1.1.1...1.1.2)
 
 **Merged pull requests:**
 
 - Update niapy dependency [\#49](https://github.com/lukapecnik/NiaAML/pull/49) ([lukapecnik](https://github.com/lukapecnik))
 
-## [1.1.1](https://github.com/lukapecnik/niaaml/tree/1.1.1) (2021-03-09)
+## [1.1.1](https://github.com/lukapecnik/NiaAML/tree/1.1.1) (2021-03-09)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/1.1.1rc2...1.1.1)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/1.1.1rc2...1.1.1)
 
 **Merged pull requests:**
 
 - logo \[ci skip\] [\#48](https://github.com/lukapecnik/NiaAML/pull/48) ([lukapecnik](https://github.com/lukapecnik))
 - Fedora package pushed to stable [\#46](https://github.com/lukapecnik/NiaAML/pull/46) ([firefly-cpp](https://github.com/firefly-cpp))
 - Restructuring of paper and editorial changes [\#45](https://github.com/lukapecnik/NiaAML/pull/45) ([adi3](https://github.com/adi3))
 - Corrections of paper [\#44](https://github.com/lukapecnik/NiaAML/pull/44) ([firefly-cpp](https://github.com/firefly-cpp))
 
-## [1.1.1rc2](https://github.com/lukapecnik/niaaml/tree/1.1.1rc2) (2020-12-22)
+## [1.1.1rc2](https://github.com/lukapecnik/NiaAML/tree/1.1.1rc2) (2020-12-22)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/1.1.1rc1...1.1.1rc2)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/1.1.1rc1...1.1.1rc2)
 
-## [1.1.1rc1](https://github.com/lukapecnik/niaaml/tree/1.1.1rc1) (2020-12-22)
+## [1.1.1rc1](https://github.com/lukapecnik/NiaAML/tree/1.1.1rc1) (2020-12-22)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/1.1.0...1.1.1rc1)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/1.1.0...1.1.1rc1)
 
 **Merged pull requests:**
 
 - Original NiaAML method support \[ci skip\] [\#43](https://github.com/lukapecnik/NiaAML/pull/43) ([lukapecnik](https://github.com/lukapecnik))
 
-## [1.1.0](https://github.com/lukapecnik/niaaml/tree/1.1.0) (2020-12-16)
+## [1.1.0](https://github.com/lukapecnik/NiaAML/tree/1.1.0) (2020-12-16)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/1.0.0rc7...1.1.0)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/1.0.0rc7...1.1.0)
 
-## [1.0.0rc7](https://github.com/lukapecnik/niaaml/tree/1.0.0rc7) (2020-12-14)
+## [1.0.0rc7](https://github.com/lukapecnik/NiaAML/tree/1.0.0rc7) (2020-12-14)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/1.0.0rc6...1.0.0rc7)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/1.0.0rc6...1.0.0rc7)
 
 **Closed issues:**
 
 - References [\#40](https://github.com/lukapecnik/NiaAML/issues/40)
 
 **Merged pull requests:**
 
 - Paper update [\#42](https://github.com/lukapecnik/NiaAML/pull/42) ([firefly-cpp](https://github.com/firefly-cpp))
 - minor corrections in examples [\#39](https://github.com/lukapecnik/NiaAML/pull/39) ([firefly-cpp](https://github.com/firefly-cpp))
 
-## [1.0.0rc6](https://github.com/lukapecnik/niaaml/tree/1.0.0rc6) (2020-12-12)
+## [1.0.0rc6](https://github.com/lukapecnik/NiaAML/tree/1.0.0rc6) (2020-12-12)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/1.0.0rc5...1.0.0rc6)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/1.0.0rc5...1.0.0rc6)
 
 **Closed issues:**
 
 - Conda package [\#34](https://github.com/lukapecnik/NiaAML/issues/34)
 
 **Merged pull requests:**
 
 - Additional features [\#38](https://github.com/lukapecnik/NiaAML/pull/38) ([lukapecnik](https://github.com/lukapecnik))
 - Conda fix \[ci skip\] [\#37](https://github.com/lukapecnik/NiaAML/pull/37) ([lukapecnik](https://github.com/lukapecnik))
 - Orcid identifiers added [\#36](https://github.com/lukapecnik/NiaAML/pull/36) ([firefly-cpp](https://github.com/firefly-cpp))
 
-## [1.0.0rc5](https://github.com/lukapecnik/niaaml/tree/1.0.0rc5) (2020-12-11)
+## [1.0.0rc5](https://github.com/lukapecnik/NiaAML/tree/1.0.0rc5) (2020-12-11)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/1.0.0rc4...1.0.0rc5)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/1.0.0rc4...1.0.0rc5)
 
 **Closed issues:**
 
 - Installation problems [\#31](https://github.com/lukapecnik/NiaAML/issues/31)
 
 **Merged pull requests:**
 
 - Conda support [\#35](https://github.com/lukapecnik/NiaAML/pull/35) ([lukapecnik](https://github.com/lukapecnik))
 
-## [1.0.0rc4](https://github.com/lukapecnik/niaaml/tree/1.0.0rc4) (2020-12-10)
+## [1.0.0rc4](https://github.com/lukapecnik/NiaAML/tree/1.0.0rc4) (2020-12-10)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/1.0.0rc3...1.0.0rc4)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/1.0.0rc3...1.0.0rc4)
 
 **Merged pull requests:**
 
 - Python 3.6 support [\#33](https://github.com/lukapecnik/NiaAML/pull/33) ([lukapecnik](https://github.com/lukapecnik))
 - First version of paper [\#32](https://github.com/lukapecnik/NiaAML/pull/32) ([firefly-cpp](https://github.com/firefly-cpp))
 
-## [1.0.0rc3](https://github.com/lukapecnik/niaaml/tree/1.0.0rc3) (2020-12-10)
+## [1.0.0rc3](https://github.com/lukapecnik/NiaAML/tree/1.0.0rc3) (2020-12-10)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/1.0.0rc2...1.0.0rc3)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/1.0.0rc2...1.0.0rc3)
 
-## [1.0.0rc2](https://github.com/lukapecnik/niaaml/tree/1.0.0rc2) (2020-12-08)
+## [1.0.0rc2](https://github.com/lukapecnik/NiaAML/tree/1.0.0rc2) (2020-12-08)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/1.0.0rc1...1.0.0rc2)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/1.0.0rc1...1.0.0rc2)
 
 **Merged pull requests:**
 
 - feature missing values imputation [\#30](https://github.com/lukapecnik/NiaAML/pull/30) ([lukapecnik](https://github.com/lukapecnik))
 - README updated [\#29](https://github.com/lukapecnik/NiaAML/pull/29) ([firefly-cpp](https://github.com/firefly-cpp))
 - Readme update, encoder check for type int64 [\#28](https://github.com/lukapecnik/NiaAML/pull/28) ([lukapecnik](https://github.com/lukapecnik))
 - Markdown and docs [\#27](https://github.com/lukapecnik/NiaAML/pull/27) ([lukapecnik](https://github.com/lukapecnik))
 
-## [1.0.0rc1](https://github.com/lukapecnik/niaaml/tree/1.0.0rc1) (2020-12-06)
+## [1.0.0rc1](https://github.com/lukapecnik/NiaAML/tree/1.0.0rc1) (2020-12-06)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/0.1.4...1.0.0rc1)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/0.1.4...1.0.0rc1)
 
 **Merged pull requests:**
 
 - Added support for categorical features [\#26](https://github.com/lukapecnik/NiaAML/pull/26) ([lukapecnik](https://github.com/lukapecnik))
 
-## [0.1.4](https://github.com/lukapecnik/niaaml/tree/0.1.4) (2020-12-05)
+## [0.1.4](https://github.com/lukapecnik/NiaAML/tree/0.1.4) (2020-12-05)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/0.1.3...0.1.4)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/0.1.3...0.1.4)
 
 **Merged pull requests:**
 
 - remove 10-fold cross validation from benchmark, critical bug fix [\#25](https://github.com/lukapecnik/NiaAML/pull/25) ([lukapecnik](https://github.com/lukapecnik))
 - run all experiments at once [\#24](https://github.com/lukapecnik/NiaAML/pull/24) ([firefly-cpp](https://github.com/firefly-cpp))
 
-## [0.1.3](https://github.com/lukapecnik/niaaml/tree/0.1.3) (2020-12-04)
+## [0.1.3](https://github.com/lukapecnik/NiaAML/tree/0.1.3) (2020-12-04)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/0.1.3a1...0.1.3)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/0.1.3a1...0.1.3)
 
-## [0.1.3a1](https://github.com/lukapecnik/niaaml/tree/0.1.3a1) (2020-12-01)
+## [0.1.3a1](https://github.com/lukapecnik/NiaAML/tree/0.1.3a1) (2020-12-01)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/0.1.2...0.1.3a1)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/0.1.2...0.1.3a1)
 
 **Merged pull requests:**
 
 - 0.1.3a1 pre-release python 3.7 compatibility [\#23](https://github.com/lukapecnik/NiaAML/pull/23) ([lukapecnik](https://github.com/lukapecnik))
 - Fixes and additions [\#22](https://github.com/lukapecnik/NiaAML/pull/22) ([lukapecnik](https://github.com/lukapecnik))
 
-## [0.1.2](https://github.com/lukapecnik/niaaml/tree/0.1.2) (2020-11-30)
+## [0.1.2](https://github.com/lukapecnik/NiaAML/tree/0.1.2) (2020-11-30)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/0.1.2a1...0.1.2)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/0.1.2a1...0.1.2)
 
 **Implemented enhancements:**
 
 - On the use of unittest [\#2](https://github.com/lukapecnik/NiaAML/issues/2)
 
 **Closed issues:**
 
@@ -196,43 +222,43 @@
 
 **Merged pull requests:**
 
 - readme.rst fix, pipeline fix [\#21](https://github.com/lukapecnik/NiaAML/pull/21) ([lukapecnik](https://github.com/lukapecnik))
 - Travis ci integration [\#20](https://github.com/lukapecnik/NiaAML/pull/20) ([lukapecnik](https://github.com/lukapecnik))
 - badges and readme update [\#19](https://github.com/lukapecnik/NiaAML/pull/19) ([lukapecnik](https://github.com/lukapecnik))
 
-## [0.1.2a1](https://github.com/lukapecnik/niaaml/tree/0.1.2a1) (2020-11-29)
+## [0.1.2a1](https://github.com/lukapecnik/NiaAML/tree/0.1.2a1) (2020-11-29)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/0.1.1...0.1.2a1)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/0.1.1...0.1.2a1)
 
 **Closed issues:**
 
 - Information about hyperparameter tuning [\#15](https://github.com/lukapecnik/NiaAML/issues/15)
 - CHANGELOG [\#14](https://github.com/lukapecnik/NiaAML/issues/14)
 - Examples [\#13](https://github.com/lukapecnik/NiaAML/issues/13)
 
 **Merged pull requests:**
 
 - Unittests, examples' description, references added to docs [\#17](https://github.com/lukapecnik/NiaAML/pull/17) ([lukapecnik](https://github.com/lukapecnik))
 
-## [0.1.1](https://github.com/lukapecnik/niaaml/tree/0.1.1) (2020-11-28)
+## [0.1.1](https://github.com/lukapecnik/NiaAML/tree/0.1.1) (2020-11-28)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/0.1.0...0.1.1)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/0.1.0...0.1.1)
 
 **Closed issues:**
 
 - Installation instructions [\#11](https://github.com/lukapecnik/NiaAML/issues/11)
 
 **Merged pull requests:**
 
 - Contributors table added [\#12](https://github.com/lukapecnik/NiaAML/pull/12) ([lukapecnik](https://github.com/lukapecnik))
 
-## [0.1.0](https://github.com/lukapecnik/niaaml/tree/0.1.0) (2020-11-27)
+## [0.1.0](https://github.com/lukapecnik/NiaAML/tree/0.1.0) (2020-11-27)
 
-[Full Changelog](https://github.com/lukapecnik/niaaml/compare/fbf47d71adb6ba72aa9210e4ead316b318253862...0.1.0)
+[Full Changelog](https://github.com/lukapecnik/NiaAML/compare/fbf47d71adb6ba72aa9210e4ead316b318253862...0.1.0)
 
 **Implemented enhancements:**
 
 - CSV Data Reader class [\#3](https://github.com/lukapecnik/NiaAML/issues/3)
 
 **Closed issues:**
```

### Comparing `NiaAML-1.1.7/LICENSE` & `NiaAML-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/__init__.py` & `NiaAML-1.1.9/niaaml/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
     "PipelineOptimizer",
     "Pipeline",
     "PipelineComponent",
     "Logger",
 ]
 
 __project__ = "niaaml"
-__version__ = "1.1.7"
+__version__ = "1.1.9"
```

### Comparing `NiaAML-1.1.7/niaaml/classifiers/__init__.py` & `NiaAML-1.1.9/niaaml/classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/classifiers/ada_boost.py` & `NiaAML-1.1.9/niaaml/classifiers/ada_boost.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 from niaaml.utilities import MinMax
 from niaaml.utilities import ParameterDefinition
 from sklearn.ensemble import AdaBoostClassifier
 import numpy as np
 
 import warnings
 from sklearn.exceptions import (
-    ChangedBehaviorWarning,
     ConvergenceWarning,
     DataConversionWarning,
     DataDimensionalityWarning,
     EfficiencyWarning,
     FitFailedWarning,
-    NonBLASDotWarning,
     UndefinedMetricWarning,
 )
 
 __all__ = ["AdaBoost"]
 
 
 class AdaBoost(Classifier):
@@ -40,21 +38,19 @@
     See Also:
         * :class:`niaaml.classifiers.Classifier`
     """
     Name = "AdaBoost"
 
     def __init__(self, **kwargs):
         r"""Initialize AdaBoost instance."""
-        warnings.filterwarnings(action="ignore", category=ChangedBehaviorWarning)
         warnings.filterwarnings(action="ignore", category=ConvergenceWarning)
         warnings.filterwarnings(action="ignore", category=DataConversionWarning)
         warnings.filterwarnings(action="ignore", category=DataDimensionalityWarning)
         warnings.filterwarnings(action="ignore", category=EfficiencyWarning)
         warnings.filterwarnings(action="ignore", category=FitFailedWarning)
-        warnings.filterwarnings(action="ignore", category=NonBLASDotWarning)
         warnings.filterwarnings(action="ignore", category=UndefinedMetricWarning)
 
         self._params = dict(
             n_estimators=ParameterDefinition(MinMax(min=10, max=111), np.uint),
             algorithm=ParameterDefinition(["SAMME", "SAMME.R"]),
         )
         self.__ada_boost = AdaBoostClassifier()
```

### Comparing `NiaAML-1.1.7/niaaml/classifiers/bagging.py` & `NiaAML-1.1.9/niaaml/classifiers/bagging.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 from niaaml.utilities import MinMax
 from niaaml.utilities import ParameterDefinition
 from sklearn.ensemble import BaggingClassifier
 import numpy as np
 
 import warnings
 from sklearn.exceptions import (
-    ChangedBehaviorWarning,
     ConvergenceWarning,
     DataConversionWarning,
     DataDimensionalityWarning,
     EfficiencyWarning,
     FitFailedWarning,
-    NonBLASDotWarning,
     UndefinedMetricWarning,
 )
 
 __all__ = ["Bagging"]
 
 
 class Bagging(Classifier):
@@ -40,21 +38,19 @@
     See Also:
         * :class:`niaaml.classifiers.Classifier`
     """
     Name = "Bagging"
 
     def __init__(self, **kwargs):
         r"""Initialize Bagging instance."""
-        warnings.filterwarnings(action="ignore", category=ChangedBehaviorWarning)
         warnings.filterwarnings(action="ignore", category=ConvergenceWarning)
         warnings.filterwarnings(action="ignore", category=DataConversionWarning)
         warnings.filterwarnings(action="ignore", category=DataDimensionalityWarning)
         warnings.filterwarnings(action="ignore", category=EfficiencyWarning)
         warnings.filterwarnings(action="ignore", category=FitFailedWarning)
-        warnings.filterwarnings(action="ignore", category=NonBLASDotWarning)
         warnings.filterwarnings(action="ignore", category=UndefinedMetricWarning)
 
         self._params = dict(
             n_estimators=ParameterDefinition(MinMax(min=10, max=111), np.uint),
             bootstrap=ParameterDefinition([True, False]),
             bootstrap_features=ParameterDefinition([True, False]),
         )
```

### Comparing `NiaAML-1.1.7/niaaml/classifiers/classifier.py` & `NiaAML-1.1.9/niaaml/classifiers/classifier.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/classifiers/decision_tree.py` & `NiaAML-1.1.9/niaaml/classifiers/decision_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from niaaml.classifiers.classifier import Classifier
 from niaaml.utilities import ParameterDefinition
 from sklearn.tree import DecisionTreeClassifier as DTC
 
 import warnings
 from sklearn.exceptions import (
-    ChangedBehaviorWarning,
     ConvergenceWarning,
     DataConversionWarning,
     DataDimensionalityWarning,
     EfficiencyWarning,
     FitFailedWarning,
-    NonBLASDotWarning,
     UndefinedMetricWarning,
 )
 
 __all__ = ["DecisionTree"]
 
 
 class DecisionTree(Classifier):
@@ -38,21 +36,19 @@
     See Also:
         * :class:`niaaml.classifiers.Classifier`
     """
     Name = "Decision Tree Classifier"
 
     def __init__(self, **kwargs):
         r"""Initialize DecisionTree instance."""
-        warnings.filterwarnings(action="ignore", category=ChangedBehaviorWarning)
         warnings.filterwarnings(action="ignore", category=ConvergenceWarning)
         warnings.filterwarnings(action="ignore", category=DataConversionWarning)
         warnings.filterwarnings(action="ignore", category=DataDimensionalityWarning)
         warnings.filterwarnings(action="ignore", category=EfficiencyWarning)
         warnings.filterwarnings(action="ignore", category=FitFailedWarning)
-        warnings.filterwarnings(action="ignore", category=NonBLASDotWarning)
         warnings.filterwarnings(action="ignore", category=UndefinedMetricWarning)
 
         self._params = dict(
             criterion=ParameterDefinition(["gini", "entropy"]),
             splitter=ParameterDefinition(["best", "random"]),
         )
         self.__decision_tree_classifier = DTC()
```

### Comparing `NiaAML-1.1.7/niaaml/classifiers/extremely_randomized_trees.py` & `NiaAML-1.1.9/niaaml/classifiers/extremely_randomized_trees.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 from niaaml.utilities import MinMax
 from niaaml.utilities import ParameterDefinition
 from sklearn.ensemble import ExtraTreesClassifier
 import numpy as np
 
 import warnings
 from sklearn.exceptions import (
-    ChangedBehaviorWarning,
     ConvergenceWarning,
     DataConversionWarning,
     DataDimensionalityWarning,
     EfficiencyWarning,
     FitFailedWarning,
-    NonBLASDotWarning,
     UndefinedMetricWarning,
 )
 
 __all__ = ["ExtremelyRandomizedTrees"]
 
 
 class ExtremelyRandomizedTrees(Classifier):
@@ -40,21 +38,19 @@
     See Also:
         * :class:`niaaml.classifiers.Classifier`
     """
     Name = "Extremely Randomized Trees"
 
     def __init__(self, **kwargs):
         r"""Initialize ExtremelyRandomizedTrees instance."""
-        warnings.filterwarnings(action="ignore", category=ChangedBehaviorWarning)
         warnings.filterwarnings(action="ignore", category=ConvergenceWarning)
         warnings.filterwarnings(action="ignore", category=DataConversionWarning)
         warnings.filterwarnings(action="ignore", category=DataDimensionalityWarning)
         warnings.filterwarnings(action="ignore", category=EfficiencyWarning)
         warnings.filterwarnings(action="ignore", category=FitFailedWarning)
-        warnings.filterwarnings(action="ignore", category=NonBLASDotWarning)
         warnings.filterwarnings(action="ignore", category=UndefinedMetricWarning)
 
         self._params = dict(
             n_estimators=ParameterDefinition(MinMax(min=10, max=111), np.uint)
         )
         self.__extra_trees_classifier = ExtraTreesClassifier()
```

### Comparing `NiaAML-1.1.7/niaaml/classifiers/gaussian_naive_bayes.py` & `NiaAML-1.1.9/niaaml/classifiers/gaussian_process.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,92 +1,95 @@
 from niaaml.classifiers.classifier import Classifier
-from sklearn.naive_bayes import GaussianNB as GNB
+from niaaml.utilities import MinMax
+from niaaml.utilities import ParameterDefinition
+from sklearn.gaussian_process import GaussianProcessClassifier as GPC
+import numpy as np
 
 import warnings
 from sklearn.exceptions import (
-    ChangedBehaviorWarning,
     ConvergenceWarning,
     DataConversionWarning,
     DataDimensionalityWarning,
     EfficiencyWarning,
     FitFailedWarning,
-    NonBLASDotWarning,
     UndefinedMetricWarning,
 )
 
-__all__ = ["GaussianNB"]
+__all__ = ["GaussianProcess"]
 
 
-class GaussianNB(Classifier):
-    r"""Implementation of gaussian Naive Bayes classifier.
+class GaussianProcess(Classifier):
+    r"""Implementation of gaussian process classifier.
 
     Date:
         2020
 
     Author:
         Luka Pečnik
 
     License:
         MIT
 
     Reference:
-        Murphy, Kevin P. "Naive bayes classifiers." University of British Columbia 18 (2006): 60.
+        Rasmussen, Carl Edward, and Hannes Nickisch. "Gaussian processes for machine learning (GPML) toolbox." The Journal of Machine Learning Research 11 (2010): 3011-3015.
 
     Documentation:
-        https://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.GaussianNB.html
+        https://scikit-learn.org/stable/modules/generated/sklearn.gaussian_process.GaussianProcessClassifier.html
 
     See Also:
         * :class:`niaaml.classifiers.Classifier`
     """
-    Name = "Gaussian Naive Bayes"
+    Name = "Gaussian Process Classifier"
 
     def __init__(self, **kwargs):
-        r"""Initialize GaussianNB instance."""
-        warnings.filterwarnings(action="ignore", category=ChangedBehaviorWarning)
+        r"""Initialize GaussianProcess instance."""
         warnings.filterwarnings(action="ignore", category=ConvergenceWarning)
         warnings.filterwarnings(action="ignore", category=DataConversionWarning)
         warnings.filterwarnings(action="ignore", category=DataDimensionalityWarning)
         warnings.filterwarnings(action="ignore", category=EfficiencyWarning)
         warnings.filterwarnings(action="ignore", category=FitFailedWarning)
-        warnings.filterwarnings(action="ignore", category=NonBLASDotWarning)
         warnings.filterwarnings(action="ignore", category=UndefinedMetricWarning)
 
-        self.__gaussian_nb = GNB()
-        super(GaussianNB, self).__init__()
+        self._params = dict(
+            max_iter_predict=ParameterDefinition(MinMax(50, 200), np.uint),
+            warm_start=ParameterDefinition([True, False]),
+            multi_class=ParameterDefinition(["one_vs_rest", "one_vs_one"]),
+        )
+        self.__gaussian_process = GPC()
 
     def set_parameters(self, **kwargs):
         r"""Set the parameters/arguments of the algorithm."""
-        self.__gaussian_nb.set_params(**kwargs)
+        self.__gaussian_process.set_params(**kwargs)
 
     def fit(self, x, y, **kwargs):
-        r"""Fit GaussianNB.
+        r"""Fit GaussianProcess.
 
         Arguments:
             x (pandas.core.frame.DataFrame): n samples to classify.
             y (pandas.core.series.Series): n classes of the samples in the x array.
 
         Returns:
             None
         """
-        self.__gaussian_nb.fit(x, y)
+        self.__gaussian_process.fit(x, y)
 
     def predict(self, x, **kwargs):
         r"""Predict class for each sample (row) in x.
 
         Arguments:
             x (pandas.core.frame.DataFrame): n samples to classify.
 
         Returns:
             pandas.core.series.Series: n predicted classes.
         """
-        return self.__gaussian_nb.predict(x)
+        return self.__gaussian_process.predict(x)
 
     def to_string(self):
         r"""User friendly representation of the object.
 
         Returns:
             str: User friendly representation of the object.
         """
         return Classifier.to_string(self).format(
             name=self.Name,
-            args=self._parameters_to_string(self.__gaussian_nb.get_params()),
+            args=self._parameters_to_string(self.__gaussian_process.get_params()),
         )
```

### Comparing `NiaAML-1.1.7/niaaml/classifiers/gaussian_process.py` & `NiaAML-1.1.9/niaaml/classifiers/k_neighbors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,92 @@
 from niaaml.classifiers.classifier import Classifier
-from niaaml.utilities import MinMax
 from niaaml.utilities import ParameterDefinition
-from sklearn.gaussian_process import GaussianProcessClassifier as GPC
-import numpy as np
+from sklearn.neighbors import KNeighborsClassifier as KNC
 
 import warnings
 from sklearn.exceptions import (
-    ChangedBehaviorWarning,
     ConvergenceWarning,
     DataConversionWarning,
     DataDimensionalityWarning,
     EfficiencyWarning,
     FitFailedWarning,
-    NonBLASDotWarning,
     UndefinedMetricWarning,
 )
 
-__all__ = ["GaussianProcess"]
+__all__ = ["KNeighbors"]
 
 
-class GaussianProcess(Classifier):
-    r"""Implementation of gaussian process classifier.
+class KNeighbors(Classifier):
+    r"""Implementation of k neighbors classifier.
 
     Date:
         2020
 
     Author:
         Luka Pečnik
 
     License:
         MIT
 
     Reference:
-        Rasmussen, Carl Edward, and Hannes Nickisch. "Gaussian processes for machine learning (GPML) toolbox." The Journal of Machine Learning Research 11 (2010): 3011-3015.
+        “Neighbourhood Components Analysis”, J. Goldberger, S. Roweis, G. Hinton, R. Salakhutdinov, Advances in Neural Information Processing Systems, Vol. 17, May 2005, pp. 513-520.
 
     Documentation:
-        https://scikit-learn.org/stable/modules/generated/sklearn.gaussian_process.GaussianProcessClassifier.html
+        https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html
 
     See Also:
         * :class:`niaaml.classifiers.Classifier`
     """
-    Name = "Gaussian Process Classifier"
+    Name = "K Neighbors Classifier"
 
     def __init__(self, **kwargs):
-        r"""Initialize GaussianProcess instance."""
-        warnings.filterwarnings(action="ignore", category=ChangedBehaviorWarning)
+        r"""Initialize KNeighbors instance."""
         warnings.filterwarnings(action="ignore", category=ConvergenceWarning)
         warnings.filterwarnings(action="ignore", category=DataConversionWarning)
         warnings.filterwarnings(action="ignore", category=DataDimensionalityWarning)
         warnings.filterwarnings(action="ignore", category=EfficiencyWarning)
         warnings.filterwarnings(action="ignore", category=FitFailedWarning)
-        warnings.filterwarnings(action="ignore", category=NonBLASDotWarning)
         warnings.filterwarnings(action="ignore", category=UndefinedMetricWarning)
 
         self._params = dict(
-            max_iter_predict=ParameterDefinition(MinMax(50, 200), np.uint),
-            warm_start=ParameterDefinition([True, False]),
-            multi_class=ParameterDefinition(["one_vs_rest", "one_vs_one"]),
+            weights=ParameterDefinition(["uniform", "distance"]),
+            algorithm=ParameterDefinition(["auto", "ball_tree", "kd_tree", "brute"]),
         )
-        self.__gaussian_process = GPC()
+        self.__kn_classifier = KNC()
 
     def set_parameters(self, **kwargs):
         r"""Set the parameters/arguments of the algorithm."""
-        self.__gaussian_process.set_params(**kwargs)
+        self.__kn_classifier.set_params(**kwargs)
 
     def fit(self, x, y, **kwargs):
-        r"""Fit GaussianProcess.
+        r"""Fit KNeighbors.
 
         Arguments:
             x (pandas.core.frame.DataFrame): n samples to classify.
             y (pandas.core.series.Series): n classes of the samples in the x array.
 
         Returns:
             None
         """
-        self.__gaussian_process.fit(x, y)
+        self.__kn_classifier.fit(x, y)
 
     def predict(self, x, **kwargs):
         r"""Predict class for each sample (row) in x.
 
         Arguments:
             x (pandas.core.frame.DataFrame): n samples to classify.
 
         Returns:
             pandas.core.series.Series: n predicted classes.
         """
-        return self.__gaussian_process.predict(x)
+        return self.__kn_classifier.predict(x)
 
     def to_string(self):
         r"""User friendly representation of the object.
 
         Returns:
             str: User friendly representation of the object.
         """
         return Classifier.to_string(self).format(
             name=self.Name,
-            args=self._parameters_to_string(self.__gaussian_process.get_params()),
+            args=self._parameters_to_string(self.__kn_classifier.get_params()),
         )
```

### Comparing `NiaAML-1.1.7/niaaml/classifiers/k_neighbors.py` & `NiaAML-1.1.9/niaaml/classifiers/gaussian_naive_bayes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,96 +1,88 @@
 from niaaml.classifiers.classifier import Classifier
-from niaaml.utilities import ParameterDefinition
-from sklearn.neighbors import KNeighborsClassifier as KNC
+from sklearn.naive_bayes import GaussianNB as GNB
 
 import warnings
 from sklearn.exceptions import (
-    ChangedBehaviorWarning,
     ConvergenceWarning,
     DataConversionWarning,
     DataDimensionalityWarning,
     EfficiencyWarning,
     FitFailedWarning,
-    NonBLASDotWarning,
     UndefinedMetricWarning,
 )
 
-__all__ = ["KNeighbors"]
+__all__ = ["GaussianNB"]
 
 
-class KNeighbors(Classifier):
-    r"""Implementation of k neighbors classifier.
+class GaussianNB(Classifier):
+    r"""Implementation of gaussian Naive Bayes classifier.
 
     Date:
         2020
 
     Author:
         Luka Pečnik
 
     License:
         MIT
 
     Reference:
-        “Neighbourhood Components Analysis”, J. Goldberger, S. Roweis, G. Hinton, R. Salakhutdinov, Advances in Neural Information Processing Systems, Vol. 17, May 2005, pp. 513-520.
+        Murphy, Kevin P. "Naive bayes classifiers." University of British Columbia 18 (2006): 60.
 
     Documentation:
-        https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html
+        https://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.GaussianNB.html
 
     See Also:
         * :class:`niaaml.classifiers.Classifier`
     """
-    Name = "K Neighbors Classifier"
+    Name = "Gaussian Naive Bayes"
 
     def __init__(self, **kwargs):
-        r"""Initialize KNeighbors instance."""
-        warnings.filterwarnings(action="ignore", category=ChangedBehaviorWarning)
+        r"""Initialize GaussianNB instance."""
         warnings.filterwarnings(action="ignore", category=ConvergenceWarning)
         warnings.filterwarnings(action="ignore", category=DataConversionWarning)
         warnings.filterwarnings(action="ignore", category=DataDimensionalityWarning)
         warnings.filterwarnings(action="ignore", category=EfficiencyWarning)
         warnings.filterwarnings(action="ignore", category=FitFailedWarning)
-        warnings.filterwarnings(action="ignore", category=NonBLASDotWarning)
         warnings.filterwarnings(action="ignore", category=UndefinedMetricWarning)
 
-        self._params = dict(
-            weights=ParameterDefinition(["uniform", "distance"]),
-            algorithm=ParameterDefinition(["auto", "ball_tree", "kd_tree", "brute"]),
-        )
-        self.__kn_classifier = KNC()
+        self.__gaussian_nb = GNB()
+        super(GaussianNB, self).__init__()
 
     def set_parameters(self, **kwargs):
         r"""Set the parameters/arguments of the algorithm."""
-        self.__kn_classifier.set_params(**kwargs)
+        self.__gaussian_nb.set_params(**kwargs)
 
     def fit(self, x, y, **kwargs):
-        r"""Fit KNeighbors.
+        r"""Fit GaussianNB.
 
         Arguments:
             x (pandas.core.frame.DataFrame): n samples to classify.
             y (pandas.core.series.Series): n classes of the samples in the x array.
 
         Returns:
             None
         """
-        self.__kn_classifier.fit(x, y)
+        self.__gaussian_nb.fit(x, y)
 
     def predict(self, x, **kwargs):
         r"""Predict class for each sample (row) in x.
 
         Arguments:
             x (pandas.core.frame.DataFrame): n samples to classify.
 
         Returns:
             pandas.core.series.Series: n predicted classes.
         """
-        return self.__kn_classifier.predict(x)
+        return self.__gaussian_nb.predict(x)
 
     def to_string(self):
         r"""User friendly representation of the object.
 
         Returns:
             str: User friendly representation of the object.
         """
         return Classifier.to_string(self).format(
             name=self.Name,
-            args=self._parameters_to_string(self.__kn_classifier.get_params()),
+            args=self._parameters_to_string(self.__gaussian_nb.get_params()),
         )
```

### Comparing `NiaAML-1.1.7/niaaml/classifiers/linear_svc.py` & `NiaAML-1.1.9/niaaml/classifiers/linear_svc.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 from niaaml.utilities import MinMax
 from niaaml.utilities import ParameterDefinition
 from sklearn.svm import LinearSVC as LSVC
 import numpy as np
 
 import warnings
 from sklearn.exceptions import (
-    ChangedBehaviorWarning,
     ConvergenceWarning,
     DataConversionWarning,
     DataDimensionalityWarning,
     EfficiencyWarning,
     FitFailedWarning,
-    NonBLASDotWarning,
     UndefinedMetricWarning,
 )
 
 __all__ = ["LinearSVC"]
 
 
 class LinearSVC(Classifier):
@@ -40,21 +38,19 @@
     See Also:
         * :class:`niaaml.classifiers.Classifier`
     """
     Name = "Linear Support Vector Classification"
 
     def __init__(self, **kwargs):
         r"""Initialize LinearSVCClassifier instance."""
-        warnings.filterwarnings(action="ignore", category=ChangedBehaviorWarning)
         warnings.filterwarnings(action="ignore", category=ConvergenceWarning)
         warnings.filterwarnings(action="ignore", category=DataConversionWarning)
         warnings.filterwarnings(action="ignore", category=DataDimensionalityWarning)
         warnings.filterwarnings(action="ignore", category=EfficiencyWarning)
         warnings.filterwarnings(action="ignore", category=FitFailedWarning)
-        warnings.filterwarnings(action="ignore", category=NonBLASDotWarning)
         warnings.filterwarnings(action="ignore", category=UndefinedMetricWarning)
 
         self._params = dict(
             penalty=ParameterDefinition(["l1", "l2"]),
             max_iter=ParameterDefinition(MinMax(min=300, max=2000), np.uint),
         )
         self.__linear_SVC = LSVC()
```

### Comparing `NiaAML-1.1.7/niaaml/classifiers/multi_layer_perceptron.py` & `NiaAML-1.1.9/niaaml/classifiers/multi_layer_perceptron.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from niaaml.classifiers.classifier import Classifier
 from niaaml.utilities import ParameterDefinition
 from sklearn.neural_network import MLPClassifier
 
 import warnings
 from sklearn.exceptions import (
-    ChangedBehaviorWarning,
     ConvergenceWarning,
     DataConversionWarning,
     DataDimensionalityWarning,
     EfficiencyWarning,
     FitFailedWarning,
-    NonBLASDotWarning,
     UndefinedMetricWarning,
 )
 
 __all__ = ["MultiLayerPerceptron"]
 
 
 class MultiLayerPerceptron(Classifier):
@@ -38,21 +36,19 @@
     See Also:
         * :class:`niaaml.classifiers.Classifier`
     """
     Name = "Multi Layer Perceptron"
 
     def __init__(self, **kwargs):
         r"""Initialize MultiLayerPerceptron instance."""
-        warnings.filterwarnings(action="ignore", category=ChangedBehaviorWarning)
         warnings.filterwarnings(action="ignore", category=ConvergenceWarning)
         warnings.filterwarnings(action="ignore", category=DataConversionWarning)
         warnings.filterwarnings(action="ignore", category=DataDimensionalityWarning)
         warnings.filterwarnings(action="ignore", category=EfficiencyWarning)
         warnings.filterwarnings(action="ignore", category=FitFailedWarning)
-        warnings.filterwarnings(action="ignore", category=NonBLASDotWarning)
         warnings.filterwarnings(action="ignore", category=UndefinedMetricWarning)
 
         self._params = dict(
             activation=ParameterDefinition(["identity", "logistic", "tanh", "relu"]),
             solver=ParameterDefinition(["lbfgs", "sgd", "adam"]),
             learning_rate=ParameterDefinition(["constant", "invscaling", "adaptive"]),
         )
```

### Comparing `NiaAML-1.1.7/niaaml/classifiers/quadratic_driscriminant_analysis.py` & `NiaAML-1.1.9/niaaml/classifiers/quadratic_driscriminant_analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from niaaml.classifiers.classifier import Classifier
 from sklearn.discriminant_analysis import QuadraticDiscriminantAnalysis as QDA
 
 import warnings
 from sklearn.exceptions import (
-    ChangedBehaviorWarning,
     ConvergenceWarning,
     DataConversionWarning,
     DataDimensionalityWarning,
     EfficiencyWarning,
     FitFailedWarning,
-    NonBLASDotWarning,
     UndefinedMetricWarning,
 )
 
 __all__ = ["QuadraticDiscriminantAnalysis"]
 
 
 class QuadraticDiscriminantAnalysis(Classifier):
@@ -37,21 +35,19 @@
     See Also:
         * :class:`niaaml.classifiers.Classifier`
     """
     Name = "Quadratic Discriminant Analysis"
 
     def __init__(self, **kwargs):
         r"""Initialize QuadraticDiscriminantAnalysis instance."""
-        warnings.filterwarnings(action="ignore", category=ChangedBehaviorWarning)
         warnings.filterwarnings(action="ignore", category=ConvergenceWarning)
         warnings.filterwarnings(action="ignore", category=DataConversionWarning)
         warnings.filterwarnings(action="ignore", category=DataDimensionalityWarning)
         warnings.filterwarnings(action="ignore", category=EfficiencyWarning)
         warnings.filterwarnings(action="ignore", category=FitFailedWarning)
-        warnings.filterwarnings(action="ignore", category=NonBLASDotWarning)
         warnings.filterwarnings(action="ignore", category=UndefinedMetricWarning)
 
         self.__qda = QDA()
         super(QuadraticDiscriminantAnalysis, self).__init__()
 
     def set_parameters(self, **kwargs):
         r"""Set the parameters/arguments of the algorithm."""
```

### Comparing `NiaAML-1.1.7/niaaml/classifiers/random_forest.py` & `NiaAML-1.1.9/niaaml/classifiers/random_forest.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 from niaaml.utilities import MinMax
 from niaaml.utilities import ParameterDefinition
 from sklearn.ensemble import RandomForestClassifier as RF
 import numpy as np
 
 import warnings
 from sklearn.exceptions import (
-    ChangedBehaviorWarning,
     ConvergenceWarning,
     DataConversionWarning,
     DataDimensionalityWarning,
     EfficiencyWarning,
     FitFailedWarning,
-    NonBLASDotWarning,
     UndefinedMetricWarning,
 )
 
 __all__ = ["RandomForest"]
 
 
 class RandomForest(Classifier):
@@ -40,21 +38,19 @@
     See Also:
         * :class:`niaaml.classifiers.Classifier`
     """
     Name = "Random Forest Classifier"
 
     def __init__(self, **kwargs):
         r"""Initialize RandomForestClassifier instance."""
-        warnings.filterwarnings(action="ignore", category=ChangedBehaviorWarning)
         warnings.filterwarnings(action="ignore", category=ConvergenceWarning)
         warnings.filterwarnings(action="ignore", category=DataConversionWarning)
         warnings.filterwarnings(action="ignore", category=DataDimensionalityWarning)
         warnings.filterwarnings(action="ignore", category=EfficiencyWarning)
         warnings.filterwarnings(action="ignore", category=FitFailedWarning)
-        warnings.filterwarnings(action="ignore", category=NonBLASDotWarning)
         warnings.filterwarnings(action="ignore", category=UndefinedMetricWarning)
 
         self._params = dict(
             n_estimators=ParameterDefinition(MinMax(min=10, max=111), np.uint)
         )
         self.__random_forest_classifier = RF()
```

### Comparing `NiaAML-1.1.7/niaaml/classifiers/utility.py` & `NiaAML-1.1.9/niaaml/classifiers/utility.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/data/basic_data_reader.py` & `NiaAML-1.1.9/niaaml/data/basic_data_reader.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/data/csv_data_reader.py` & `NiaAML-1.1.9/niaaml/data/csv_data_reader.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/data/data_reader.py` & `NiaAML-1.1.9/niaaml/data/data_reader.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/fitness/accuracy.py` & `NiaAML-1.1.9/niaaml/fitness/accuracy.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/fitness/cohen_kappa.py` & `NiaAML-1.1.9/niaaml/fitness/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/fitness/f1.py` & `NiaAML-1.1.9/niaaml/fitness/f1.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/fitness/fitness_function.py` & `NiaAML-1.1.9/niaaml/fitness/fitness_function.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/fitness/precision.py` & `NiaAML-1.1.9/niaaml/fitness/precision.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/fitness/utility.py` & `NiaAML-1.1.9/niaaml/fitness/utility.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/logger.py` & `NiaAML-1.1.9/niaaml/logger.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/pipeline.py` & `NiaAML-1.1.9/niaaml/pipeline.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/pipeline_component.py` & `NiaAML-1.1.9/niaaml/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/pipeline_optimizer.py` & `NiaAML-1.1.9/niaaml/pipeline_optimizer.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/encoding/feature_encoder.py` & `NiaAML-1.1.9/niaaml/preprocessing/encoding/feature_encoder.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/encoding/one_hot_encoder.py` & `NiaAML-1.1.9/niaaml/preprocessing/encoding/one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/encoding/utility.py` & `NiaAML-1.1.9/niaaml/preprocessing/encoding/utility.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_selection/__init__.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_selection/_feature_selection_threshold_problem.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_selection/_feature_selection_threshold_problem.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_selection/bat_algorithm.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_selection/bat_algorithm.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_selection/differential_evolution.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_selection/differential_evolution.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_selection/feature_selection_algorithm.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_selection/feature_selection_algorithm.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_selection/grey_wolf_optimizer.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_selection/grey_wolf_optimizer.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_selection/jDEFSTH.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_selection/jDEFSTH.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_selection/particle_swarm_optimization.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_selection/particle_swarm_optimization.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_selection/select_k_best.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_selection/select_k_best.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_selection/select_percentile.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_selection/select_percentile.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_selection/utility.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_selection/utility.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_selection/variance_threshold.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_selection/variance_threshold.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_transform/__init__.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_transform/__init__.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_transform/feature_transform_algorithm.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_transform/feature_transform_algorithm.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_transform/max_abs_scaler.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_transform/max_abs_scaler.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_transform/normalizer.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_transform/normalizer.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_transform/quantile_transformer.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_transform/quantile_transformer.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_transform/robust_scaler.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_transform/robust_scaler.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_transform/standard_scaler.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_transform/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/feature_transform/utility.py` & `NiaAML-1.1.9/niaaml/preprocessing/feature_transform/utility.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/imputation/imputer.py` & `NiaAML-1.1.9/niaaml/preprocessing/imputation/imputer.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/imputation/simple_imputer.py` & `NiaAML-1.1.9/niaaml/preprocessing/imputation/simple_imputer.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/preprocessing/imputation/utility.py` & `NiaAML-1.1.9/niaaml/preprocessing/imputation/utility.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/niaaml/utilities.py` & `NiaAML-1.1.9/niaaml/utilities.py`

 * *Files identical despite different names*

### Comparing `NiaAML-1.1.7/pyproject.toml` & `NiaAML-1.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "NiaAML"
-version = "1.1.7"
+version = "1.1.9"
 description = "Python automated machine learning framework."
 license = "MIT"
 authors = ["Luka Pečnik <lukapecnik96@gmail.com>", "Iztok Fister Jr. <iztok.fister1@um.si>"]
 keywords = ['classification', 'NiaPy', 'scikit-learn', 'nature-inspired algorithms', 'feature selection', 'preprocessing']
 homepage = "https://github.com/lukapecnik/NiaAML"
 repository = "https://github.com/lukapecnik/NiaAML"
 readme = "README.rst"
```

### Comparing `NiaAML-1.1.7/README.rst` & `NiaAML-1.1.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 NiaAML
 ======
 
-.. image:: https://travis-ci.com/lukapecnik/NiaAML.svg?branch=master
-    :target: https://travis-ci.com/lukapecnik/NiaAML
+.. image:: https://github.com/lukapecnik/niaaml/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/lukapecnik/niaaml
 
 .. image:: https://coveralls.io/repos/github/lukapecnik/NiaAML/badge.svg?branch=travisCI_integration
     :target: https://coveralls.io/github/lukapecnik/NiaAML?branch=travisCI_integration
 
 .. image:: https://img.shields.io/pypi/v/niaaml.svg
     :target: https://pypi.python.org/pypi/niaaml
```

### Comparing `NiaAML-1.1.7/setup.py` & `NiaAML-1.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,31 +6,30 @@
  'niaaml.classifiers',
  'niaaml.data',
  'niaaml.fitness',
  'niaaml.preprocessing',
  'niaaml.preprocessing.encoding',
  'niaaml.preprocessing.feature_selection',
  'niaaml.preprocessing.feature_transform',
- 'niaaml.preprocessing.imputation',
- 'niaaml.tests']
+ 'niaaml.preprocessing.imputation']
 
 package_data = \
-{'': ['*'], 'niaaml.tests': ['tests_files/*']}
+{'': ['*']}
 
 install_requires = \
 ['niapy>=2.0.0,<3.0.0',
  'numpy>=1.19.1,<2.0.0',
  'pandas>=1.1.4,<2.0.0',
  'scikit-learn>=0.23.2,<0.24.0']
 
 setup_kwargs = {
     'name': 'niaaml',
-    'version': '1.1.7',
+    'version': '1.1.9',
     'description': 'Python automated machine learning framework.',
-    'long_description': "NiaAML\n======\n\n.. image:: https://travis-ci.com/lukapecnik/NiaAML.svg?branch=master\n    :target: https://travis-ci.com/lukapecnik/NiaAML\n\n.. image:: https://coveralls.io/repos/github/lukapecnik/NiaAML/badge.svg?branch=travisCI_integration\n    :target: https://coveralls.io/github/lukapecnik/NiaAML?branch=travisCI_integration\n\n.. image:: https://img.shields.io/pypi/v/niaaml.svg\n    :target: https://pypi.python.org/pypi/niaaml\n\n.. image:: https://img.shields.io/pypi/pyversions/niaaml.svg\n    :target: https://pypi.org/project/NiaPy/\n\n.. image:: https://img.shields.io/github/license/lukapecnik/niaaml.svg\n    :target: https://github.com/lukapecnik/niaaml/blob/master/LICENSE\n\n.. image:: https://zenodo.org/badge/289322337.svg\n   :target: https://zenodo.org/badge/latestdoi/289322337\n\n.. image:: https://joss.theoj.org/papers/10.21105/joss.02949/status.svg\n   :target: https://doi.org/10.21105/joss.02949\n\nNiaAML is an automated machine learning Python framework based on\nnature-inspired algorithms for optimization. The name comes from the\nautomated machine learning method of the same name [1]. Its\ngoal is to efficiently compose the best possible classification pipeline\nfor the given task using components on the input. The components are\ndivided into three groups: feature seletion algorithms, feature\ntransformation algorithms and classifiers. The framework uses\nnature-inspired algorithms for optimization to choose the best set of\ncomponents for the classification pipeline on the output and optimize\ntheir parameters. We use `NiaPy framework <https://github.com/NiaOrg/NiaPy>`_ for the optimization process\nwhich is a popular Python collection of nature-inspired algorithms. The\nNiaAML framework is easy to use and customize or expand to suit your\nneeds.\n\nThe NiaAML framework allows you not only to run full pipeline optimization, but also separate implemented components such as classifiers, feature selection algorithms, etc. **It supports numerical and categorical features as well as missing values in datasets.**\n\n- **Documentation:** https://niaaml.readthedocs.io/en/latest/,\n- **Tested OS:** Windows, Ubuntu, Fedora, Linux Mint and CentOS. **However, that does not mean it does not work on others.**\n\nInstallation\n------------\n\npip\n~~~\n\nInstall NiaAML with pip3:\n\n.. code:: sh\n\n    pip3 install niaaml\n\nIn case you would like to try out the latest pre-release version of the framework, install it using:\n\n.. code:: sh\n\n    pip3 install niaaml --pre\n\nGraphical User Interface\n------------------------\n\nYou can find a simple graphical user interface for NiaAML package `here <https://github.com/lukapecnik/NiaAML-GUI>`_.\n\nUsage\n-----\n\nSee the project's `repository <https://github.com/lukapecnik/NiaAML>`_ for usage examples.\n\nComponents\n----------\n\nIn the following sections you can see a list of currently implemented \ncomponents divided into groups: classifiers, feature selection \nalgorithms and feature transformation algorithms. At the end you can \nalso see a list of currently implemented fitness functions for the optimization process, \ncategorical features' encoders, and missing values' imputers.\n\nClassifiers\n~~~~~~~~~~~\n\n-  Adaptive Boosting (AdaBoost),\n-  Bagging (Bagging),\n-  Extremely Randomized Trees (ExtremelyRandomizedTrees),\n-  Linear SVC (LinearSVC),\n-  Multi Layer Perceptron (MultiLayerPerceptron),\n-  Random Forest Classifier (RandomForest),\n-  Decision Tree Classifier (DecisionTree),\n-  K-Neighbors Classifier (KNeighbors),\n-  Gaussian Process Classifier (GaussianProcess),\n-  Gaussian Naive Bayes (GaussianNB),\n-  Quadratic Discriminant Analysis (QuadraticDiscriminantAnalysis).\n\nFeature Selection Algorithms\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n-  Select K Best (SelectKBest),\n-  Select Percentile (SelectPercentile),\n-  Variance Threshold (VarianceThreshold).\n\nNature-Inspired\n^^^^^^^^^^^^^^^\n\n-  Bat Algorithm (BatAlgorithm),\n-  Differential Evolution (DifferentialEvolution),\n-  Self-Adaptive Differential Evolution (jDEFSTH),\n-  Grey Wolf Optimizer (GreyWolfOptimizer),\n-  Particle Swarm Optimization (ParticleSwarmOptimization).\n\nFeature Transformation Algorithms\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n-  Normalizer (Normalizer),\n-  Standard Scaler (StandardScaler),\n-  Maximum Absolute Scaler (MaxAbsScaler),\n-  Quantile Transformer (QuantileTransformer),\n-  Robust Scaler (RobustScaler).\n\nFitness Functions based on\n~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n-  Accuracy (Accuracy),\n-  Cohen's kappa (CohenKappa),\n-  F1-Score (F1),\n-  Precision (Precision).\n\nCategorical Feature Encoders\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n- One-Hot Encoder (OneHotEncoder).\n\nFeature Imputers\n~~~~~~~~~~~~~~~~\n\n- Simple Imputer (SimpleImputer).\n\nLicence\n-------\n\nThis package is distributed under the MIT License. This license can be\nfound online at http://www.opensource.org/licenses/MIT.\n\nDisclaimer\n----------\n\nThis framework is provided as-is, and there are no guarantees that it\nfits your purposes or that it is bug-free. Use it at your own risk!\n\nReferences\n----------\n\n[1] Iztok Fister Jr., Milan Zorman, Dušan Fister, Iztok Fister.\nContinuous optimizers for automatic design and evaluation of\nclassification pipelines. In: Frontier applications of nature inspired\ncomputation. Springer tracts in nature-inspired computing, pp.281-301,\n2020.\n",
+    'long_description': "NiaAML\n======\n\n.. image:: https://github.com/lukapecnik/niaaml/actions/workflows/test.yml/badge.svg\n    :target: https://github.com/lukapecnik/niaaml\n\n.. image:: https://coveralls.io/repos/github/lukapecnik/NiaAML/badge.svg?branch=travisCI_integration\n    :target: https://coveralls.io/github/lukapecnik/NiaAML?branch=travisCI_integration\n\n.. image:: https://img.shields.io/pypi/v/niaaml.svg\n    :target: https://pypi.python.org/pypi/niaaml\n\n.. image:: https://img.shields.io/pypi/pyversions/niaaml.svg\n    :target: https://pypi.org/project/NiaPy/\n\n.. image:: https://img.shields.io/github/license/lukapecnik/niaaml.svg\n    :target: https://github.com/lukapecnik/niaaml/blob/master/LICENSE\n\n.. image:: https://zenodo.org/badge/289322337.svg\n   :target: https://zenodo.org/badge/latestdoi/289322337\n\n.. image:: https://joss.theoj.org/papers/10.21105/joss.02949/status.svg\n   :target: https://doi.org/10.21105/joss.02949\n\nNiaAML is an automated machine learning Python framework based on\nnature-inspired algorithms for optimization. The name comes from the\nautomated machine learning method of the same name [1]. Its\ngoal is to efficiently compose the best possible classification pipeline\nfor the given task using components on the input. The components are\ndivided into three groups: feature seletion algorithms, feature\ntransformation algorithms and classifiers. The framework uses\nnature-inspired algorithms for optimization to choose the best set of\ncomponents for the classification pipeline on the output and optimize\ntheir parameters. We use `NiaPy framework <https://github.com/NiaOrg/NiaPy>`_ for the optimization process\nwhich is a popular Python collection of nature-inspired algorithms. The\nNiaAML framework is easy to use and customize or expand to suit your\nneeds.\n\nThe NiaAML framework allows you not only to run full pipeline optimization, but also separate implemented components such as classifiers, feature selection algorithms, etc. **It supports numerical and categorical features as well as missing values in datasets.**\n\n- **Documentation:** https://niaaml.readthedocs.io/en/latest/,\n- **Tested OS:** Windows, Ubuntu, Fedora, Linux Mint and CentOS. **However, that does not mean it does not work on others.**\n\nInstallation\n------------\n\npip\n~~~\n\nInstall NiaAML with pip3:\n\n.. code:: sh\n\n    pip3 install niaaml\n\nIn case you would like to try out the latest pre-release version of the framework, install it using:\n\n.. code:: sh\n\n    pip3 install niaaml --pre\n\nGraphical User Interface\n------------------------\n\nYou can find a simple graphical user interface for NiaAML package `here <https://github.com/lukapecnik/NiaAML-GUI>`_.\n\nUsage\n-----\n\nSee the project's `repository <https://github.com/lukapecnik/NiaAML>`_ for usage examples.\n\nComponents\n----------\n\nIn the following sections you can see a list of currently implemented \ncomponents divided into groups: classifiers, feature selection \nalgorithms and feature transformation algorithms. At the end you can \nalso see a list of currently implemented fitness functions for the optimization process, \ncategorical features' encoders, and missing values' imputers.\n\nClassifiers\n~~~~~~~~~~~\n\n-  Adaptive Boosting (AdaBoost),\n-  Bagging (Bagging),\n-  Extremely Randomized Trees (ExtremelyRandomizedTrees),\n-  Linear SVC (LinearSVC),\n-  Multi Layer Perceptron (MultiLayerPerceptron),\n-  Random Forest Classifier (RandomForest),\n-  Decision Tree Classifier (DecisionTree),\n-  K-Neighbors Classifier (KNeighbors),\n-  Gaussian Process Classifier (GaussianProcess),\n-  Gaussian Naive Bayes (GaussianNB),\n-  Quadratic Discriminant Analysis (QuadraticDiscriminantAnalysis).\n\nFeature Selection Algorithms\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n-  Select K Best (SelectKBest),\n-  Select Percentile (SelectPercentile),\n-  Variance Threshold (VarianceThreshold).\n\nNature-Inspired\n^^^^^^^^^^^^^^^\n\n-  Bat Algorithm (BatAlgorithm),\n-  Differential Evolution (DifferentialEvolution),\n-  Self-Adaptive Differential Evolution (jDEFSTH),\n-  Grey Wolf Optimizer (GreyWolfOptimizer),\n-  Particle Swarm Optimization (ParticleSwarmOptimization).\n\nFeature Transformation Algorithms\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n-  Normalizer (Normalizer),\n-  Standard Scaler (StandardScaler),\n-  Maximum Absolute Scaler (MaxAbsScaler),\n-  Quantile Transformer (QuantileTransformer),\n-  Robust Scaler (RobustScaler).\n\nFitness Functions based on\n~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n-  Accuracy (Accuracy),\n-  Cohen's kappa (CohenKappa),\n-  F1-Score (F1),\n-  Precision (Precision).\n\nCategorical Feature Encoders\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n- One-Hot Encoder (OneHotEncoder).\n\nFeature Imputers\n~~~~~~~~~~~~~~~~\n\n- Simple Imputer (SimpleImputer).\n\nLicence\n-------\n\nThis package is distributed under the MIT License. This license can be\nfound online at http://www.opensource.org/licenses/MIT.\n\nDisclaimer\n----------\n\nThis framework is provided as-is, and there are no guarantees that it\nfits your purposes or that it is bug-free. Use it at your own risk!\n\nReferences\n----------\n\n[1] Iztok Fister Jr., Milan Zorman, Dušan Fister, Iztok Fister.\nContinuous optimizers for automatic design and evaluation of\nclassification pipelines. In: Frontier applications of nature inspired\ncomputation. Springer tracts in nature-inspired computing, pp.281-301,\n2020.\n",
     'author': 'Luka Pečnik',
     'author_email': 'lukapecnik96@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/lukapecnik/NiaAML',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `NiaAML-1.1.7/PKG-INFO` & `NiaAML-1.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niaaml
-Version: 1.1.7
+Version: 1.1.9
 Summary: Python automated machine learning framework.
 Home-page: https://github.com/lukapecnik/NiaAML
 License: MIT
 Keywords: classification,NiaPy,scikit-learn,nature-inspired algorithms,feature selection,preprocessing
 Author: Luka Pečnik
 Author-email: lukapecnik96@gmail.com
 Requires-Python: >=3.6.2,<4.0.0
@@ -19,16 +19,16 @@
 Requires-Dist: scikit-learn (>=0.23.2,<0.24.0)
 Project-URL: Repository, https://github.com/lukapecnik/NiaAML
 Description-Content-Type: text/x-rst
 
 NiaAML
 ======
 
-.. image:: https://travis-ci.com/lukapecnik/NiaAML.svg?branch=master
-    :target: https://travis-ci.com/lukapecnik/NiaAML
+.. image:: https://github.com/lukapecnik/niaaml/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/lukapecnik/niaaml
 
 .. image:: https://coveralls.io/repos/github/lukapecnik/NiaAML/badge.svg?branch=travisCI_integration
     :target: https://coveralls.io/github/lukapecnik/NiaAML?branch=travisCI_integration
 
 .. image:: https://img.shields.io/pypi/v/niaaml.svg
     :target: https://pypi.python.org/pypi/niaaml
```

