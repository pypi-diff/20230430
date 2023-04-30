# Comparing `tmp/chemotools-0.0.8.tar.gz` & `tmp/chemotools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemotools-0.0.8.tar", last modified: Mon Apr 10 15:18:14 2023, max compression
+gzip compressed data, was "chemotools-0.0.9.tar", last modified: Mon Apr 10 20:03:27 2023, max compression
```

## Comparing `chemotools-0.0.8.tar` & `chemotools-0.0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.922122 chemotools-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-10 15:17:51.000000 chemotools-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-10 15:18:14.922122 chemotools-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-10 15:17:51.000000 chemotools-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.914122 chemotools-0.0.8/chemotools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.918122 chemotools-0.0.8/chemotools/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/baseline/air_pls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/baseline/cubic_spline_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/baseline/linear_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/baseline/non_negative.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/baseline/polynomial_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.918122 chemotools-0.0.8/chemotools/derivative/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/derivative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/derivative/norris_william.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/derivative/savitzky_golay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.918122 chemotools-0.0.8/chemotools/normalize/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/normalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/normalize/l_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/normalize/min_max_normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.918122 chemotools-0.0.8/chemotools/scattering/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/scattering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/scattering/extended_multiplicative_scatter_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/scattering/multiplicative_scatter_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/scattering/standard_normal_variate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.918122 chemotools-0.0.8/chemotools/smoothing/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/smoothing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/smoothing/mean_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/smoothing/median_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/smoothing/savitzky_golay_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/smoothing/whittaker_smooth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.918122 chemotools-0.0.8/chemotools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/utils/check_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.922122 chemotools-0.0.8/chemotools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-10 15:18:14.000000 chemotools-0.0.8/chemotools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-10 15:18:14.000000 chemotools-0.0.8/chemotools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:18:14.000000 chemotools-0.0.8/chemotools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 15:18:14.000000 chemotools-0.0.8/chemotools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-10 15:18:14.000000 chemotools-0.0.8/chemotools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 15:17:51.000000 chemotools-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:18:14.922122 chemotools-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-10 15:17:51.000000 chemotools-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.922122 chemotools-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:17:51.000000 chemotools-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-10 15:17:51.000000 chemotools-0.0.8/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-04-10 15:17:51.000000 chemotools-0.0.8/tests/test_functionality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-10 15:17:51.000000 chemotools-0.0.8/tests/test_sklearn_compliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:03:27.263652 chemotools-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-10 20:03:15.000000 chemotools-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18484 2023-04-10 20:03:27.259652 chemotools-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17937 2023-04-10 20:03:15.000000 chemotools-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:03:27.259652 chemotools-0.0.9/chemotools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:03:27.259652 chemotools-0.0.9/chemotools/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/baseline/air_pls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/baseline/cubic_spline_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/baseline/linear_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/baseline/non_negative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/baseline/polynomial_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:03:27.259652 chemotools-0.0.9/chemotools/derivative/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/derivative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/derivative/norris_william.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/derivative/savitzky_golay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:03:27.259652 chemotools-0.0.9/chemotools/scale/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/scale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/scale/l_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/scale/min_max_normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:03:27.259652 chemotools-0.0.9/chemotools/scatter/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/scatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/scatter/extended_multiplicative_scatter_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/scatter/multiplicative_scatter_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/scatter/standard_normal_variate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:03:27.259652 chemotools-0.0.9/chemotools/smooth/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/smooth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/smooth/mean_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/smooth/median_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/smooth/savitzky_golay_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/smooth/whittaker_smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:03:27.259652 chemotools-0.0.9/chemotools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-10 20:03:15.000000 chemotools-0.0.9/chemotools/utils/check_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:03:27.259652 chemotools-0.0.9/chemotools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18484 2023-04-10 20:03:27.000000 chemotools-0.0.9/chemotools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-10 20:03:27.000000 chemotools-0.0.9/chemotools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:03:27.000000 chemotools-0.0.9/chemotools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 20:03:27.000000 chemotools-0.0.9/chemotools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-10 20:03:27.000000 chemotools-0.0.9/chemotools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 20:03:15.000000 chemotools-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 20:03:27.263652 chemotools-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-10 20:03:15.000000 chemotools-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:03:27.259652 chemotools-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:03:15.000000 chemotools-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-10 20:03:15.000000 chemotools-0.0.9/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-10 20:03:15.000000 chemotools-0.0.9/tests/test_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-10 20:03:15.000000 chemotools-0.0.9/tests/test_sklearn_compliance.py
```

### Comparing `chemotools-0.0.8/LICENSE` & `chemotools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/chemotools/baseline/air_pls.py` & `chemotools-0.0.9/chemotools/baseline/air_pls.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/chemotools/baseline/cubic_spline_correction.py` & `chemotools-0.0.9/chemotools/baseline/cubic_spline_correction.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/chemotools/baseline/linear_correction.py` & `chemotools-0.0.9/chemotools/baseline/linear_correction.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/chemotools/baseline/non_negative.py` & `chemotools-0.0.9/chemotools/baseline/non_negative.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/chemotools/baseline/polynomial_correction.py` & `chemotools-0.0.9/chemotools/baseline/polynomial_correction.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/chemotools/derivative/norris_william.py` & `chemotools-0.0.9/chemotools/derivative/norris_william.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/chemotools/derivative/savitzky_golay.py` & `chemotools-0.0.9/chemotools/derivative/savitzky_golay.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/chemotools/normalize/l_normalize.py` & `chemotools-0.0.9/chemotools/scale/l_normalize.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/chemotools/normalize/min_max_normalize.py` & `chemotools-0.0.9/chemotools/scale/min_max_normalize.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import numpy as np
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_is_fitted
 
 from chemotools.utils.check_inputs import check_input
 
 
-class MinMaxNormalize(BaseEstimator, TransformerMixin):
+class MinMaxScaler(BaseEstimator, TransformerMixin):
     def __init__(self, norm: str = 'max'):
         self.norm = norm
 
 
-    def fit(self, X: np.ndarray, y=None) -> "MinMaxNormalize":
+    def fit(self, X: np.ndarray, y=None) -> "MinMaxScaler":
         # Check that X is a 2D array and has only finite values
         X = check_input(X)
 
         # Set the number of features
         self.n_features_in_ = X.shape[1]
 
         # Set the fitted attribute to True
```

### Comparing `chemotools-0.0.8/chemotools/scattering/extended_multiplicative_scatter_correction.py` & `chemotools-0.0.9/chemotools/scatter/extended_multiplicative_scatter_correction.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/chemotools/scattering/multiplicative_scatter_correction.py` & `chemotools-0.0.9/chemotools/scatter/multiplicative_scatter_correction.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/chemotools/scattering/standard_normal_variate.py` & `chemotools-0.0.9/chemotools/scatter/standard_normal_variate.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/chemotools/smoothing/mean_filter.py` & `chemotools-0.0.9/chemotools/smooth/mean_filter.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/chemotools/smoothing/median_filter.py` & `chemotools-0.0.9/chemotools/smooth/median_filter.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/chemotools/smoothing/savitzky_golay_filter.py` & `chemotools-0.0.9/chemotools/smooth/savitzky_golay_filter.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/chemotools/smoothing/whittaker_smooth.py` & `chemotools-0.0.9/chemotools/smooth/whittaker_smooth.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/chemotools/utils/check_inputs.py` & `chemotools-0.0.9/chemotools/utils/check_inputs.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/chemotools.egg-info/SOURCES.txt` & `chemotools-0.0.9/chemotools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 ./chemotools/baseline/cubic_spline_correction.py
 ./chemotools/baseline/linear_correction.py
 ./chemotools/baseline/non_negative.py
 ./chemotools/baseline/polynomial_correction.py
 ./chemotools/derivative/__init__.py
 ./chemotools/derivative/norris_william.py
 ./chemotools/derivative/savitzky_golay.py
-./chemotools/normalize/__init__.py
-./chemotools/normalize/l_normalize.py
-./chemotools/normalize/min_max_normalize.py
-./chemotools/scattering/__init__.py
-./chemotools/scattering/extended_multiplicative_scatter_correction.py
-./chemotools/scattering/multiplicative_scatter_correction.py
-./chemotools/scattering/standard_normal_variate.py
-./chemotools/smoothing/__init__.py
-./chemotools/smoothing/mean_filter.py
-./chemotools/smoothing/median_filter.py
-./chemotools/smoothing/savitzky_golay_filter.py
-./chemotools/smoothing/whittaker_smooth.py
+./chemotools/scale/__init__.py
+./chemotools/scale/l_normalize.py
+./chemotools/scale/min_max_normalize.py
+./chemotools/scatter/__init__.py
+./chemotools/scatter/extended_multiplicative_scatter_correction.py
+./chemotools/scatter/multiplicative_scatter_correction.py
+./chemotools/scatter/standard_normal_variate.py
+./chemotools/smooth/__init__.py
+./chemotools/smooth/mean_filter.py
+./chemotools/smooth/median_filter.py
+./chemotools/smooth/savitzky_golay_filter.py
+./chemotools/smooth/whittaker_smooth.py
 ./chemotools/utils/__init__.py
 ./chemotools/utils/check_inputs.py
 ./tests/__init__.py
 ./tests/fixtures.py
 ./tests/test_functionality.py
 ./tests/test_sklearn_compliance.py
 chemotools.egg-info/PKG-INFO
```

### Comparing `chemotools-0.0.8/setup.py` & `chemotools-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/tests/fixtures.py` & `chemotools-0.0.9/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.8/tests/test_functionality.py` & `chemotools-0.0.9/tests/test_functionality.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 
 from chemotools.baseline import AirPls, LinearCorrection, NonNegative
 from chemotools.derivative import NorrisWilliams, SavitzkyGolay
-from chemotools.normalize import LNormalize, MinMaxNormalize
-from chemotools.scattering import MultiplicativeScatterCorrection, StandardNormalVariate
-from chemotools.smoothing import MeanFilter, MedianFilter, WhittakerSmooth
+from chemotools.scale import LNormalize, MinMaxScaler
+from chemotools.scatter import MultiplicativeScatterCorrection, StandardNormalVariate
+from chemotools.smooth import MeanFilter, MedianFilter, WhittakerSmooth
 from tests.fixtures import (
     spectrum,
     reference_airpls,
     reference_msc_mean,
     reference_msc_median,
     reference_sg_15_2,
     reference_snv,
@@ -63,15 +63,15 @@
     # Assert
     assert spectrum_corrected[0][0] == 0
     assert spectrum_corrected[-1][0] == 0
 
 
 def test_max_norm(spectrum):
     # Arrange
-    max_norm = MinMaxNormalize(norm="max")
+    max_norm = MinMaxScaler(norm="max")
 
     # Act
     spectrum_corrected = max_norm.fit_transform(spectrum)
 
     # Assert
     assert np.allclose(
         spectrum_corrected[0], spectrum[0] / np.max(spectrum[0]), atol=1e-8
@@ -100,15 +100,15 @@
 
     # Assert
     assert np.allclose(array_corrected[0], [1, 2.0, 4.0, 5.0, 5.0], atol=1e-8)
 
 
 def test_min_norm(spectrum):
     # Arrange
-    min_norm = MinMaxNormalize(norm="min")
+    min_norm = MinMaxScaler(norm="min")
 
     # Act
     spectrum_corrected = min_norm.fit_transform(spectrum)
 
     # Assert
     assert np.allclose(
         spectrum_corrected[0], spectrum[0] / np.min(spectrum[0]), atol=1e-8
```

### Comparing `chemotools-0.0.8/tests/test_sklearn_compliance.py` & `chemotools-0.0.9/tests/test_sklearn_compliance.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from sklearn.utils.estimator_checks import check_estimator
 
 from chemotools.baseline import AirPls, CubicSplineCorrection, LinearCorrection, NonNegative, PolynomialCorrection
 from chemotools.derivative import NorrisWilliams, SavitzkyGolay
-from chemotools.normalize import MinMaxNormalize, LNormalize
-from chemotools.scattering import MultiplicativeScatterCorrection, StandardNormalVariate
-from chemotools.smoothing import MeanFilter, MedianFilter, SavitzkyGolayFilter, WhittakerSmooth
+from chemotools.scale import MinMaxScaler, LNormalize
+from chemotools.scatter import MultiplicativeScatterCorrection, StandardNormalVariate
+from chemotools.smooth import MeanFilter, MedianFilter, SavitzkyGolayFilter, WhittakerSmooth
 
 
 # AirPls
 def test_compliance_air_pls():
     # Arrange
     transformer = AirPls()
     # Act & Assert
@@ -48,15 +48,15 @@
     transformer = MedianFilter()
     # Act & Assert
     check_estimator(transformer)
 
 # MinMaxNormalize
 def test_compliance_min_max_norm():
     # Arrange
-    transformer = MinMaxNormalize()
+    transformer = MinMaxScaler()
     # Act & Assert
     check_estimator(transformer)
 
 # MultiplicativeScatterCorrection
 def test_compliance_multiplicative_scatter_correction():
     # Arrange
     transformer = MultiplicativeScatterCorrection()
```

