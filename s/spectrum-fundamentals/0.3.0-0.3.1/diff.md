# Comparing `tmp/spectrum_fundamentals-0.3.0.tar.gz` & `tmp/spectrum_fundamentals-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_fundamentals-0.3.0.tar", max compression
+gzip compressed data, was "spectrum_fundamentals-0.3.1.tar", max compression
```

## Comparing `spectrum_fundamentals-0.3.0.tar` & `spectrum_fundamentals-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1073 2023-03-09 10:30:45.972993 spectrum_fundamentals-0.3.0/LICENSE
--rw-r--r--   0        0        0     2611 2023-03-09 10:30:45.972993 spectrum_fundamentals-0.3.0/README.rst
--rw-r--r--   0        0        0     2367 2023-03-09 10:30:45.976993 spectrum_fundamentals-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      940 2023-03-09 10:30:45.976993 spectrum_fundamentals-0.3.0/spectrum_fundamentals/__init__.py
--rw-r--r--   0        0        0      381 2023-03-09 10:30:45.976993 spectrum_fundamentals-0.3.0/spectrum_fundamentals/__main__.py
--rw-r--r--   0        0        0       29 2023-03-09 10:30:45.976993 spectrum_fundamentals-0.3.0/spectrum_fundamentals/annotation/__init__.py
--rw-r--r--   0        0        0     8433 2023-03-09 10:30:45.976993 spectrum_fundamentals-0.3.0/spectrum_fundamentals/annotation/annotation.py
--rw-r--r--   0        0        0     1302 2023-03-09 10:30:45.976993 spectrum_fundamentals-0.3.0/spectrum_fundamentals/charge.py
--rw-r--r--   0        0        0     7819 2023-03-09 10:30:45.976993 spectrum_fundamentals-0.3.0/spectrum_fundamentals/constants.py
--rw-r--r--   0        0        0    11854 2023-03-09 10:30:45.976993 spectrum_fundamentals-0.3.0/spectrum_fundamentals/fragments.py
--rw-r--r--   0        0        0       26 2023-03-09 10:30:45.976993 spectrum_fundamentals-0.3.0/spectrum_fundamentals/metrics/__init__.py
--rw-r--r--   0        0        0    14554 2023-03-09 10:30:45.976993 spectrum_fundamentals-0.3.0/spectrum_fundamentals/metrics/fragments_ratio.py
--rw-r--r--   0        0        0     1435 2023-03-09 10:30:45.976993 spectrum_fundamentals-0.3.0/spectrum_fundamentals/metrics/metric.py
--rw-r--r--   0        0        0    21481 2023-03-09 10:30:45.976993 spectrum_fundamentals-0.3.0/spectrum_fundamentals/metrics/percolator.py
--rw-r--r--   0        0        0    23581 2023-03-09 10:30:45.976993 spectrum_fundamentals-0.3.0/spectrum_fundamentals/metrics/similarity.py
--rw-r--r--   0        0        0     9166 2023-03-09 10:30:45.976993 spectrum_fundamentals-0.3.0/spectrum_fundamentals/mod_string.py
--rw-r--r--   0        0        0        0 2023-03-09 10:30:45.976993 spectrum_fundamentals-0.3.0/spectrum_fundamentals/py.typed
--rw-r--r--   0        0        0     3856 1970-01-01 00:00:00.000000 spectrum_fundamentals-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-30 18:37:48.694880 spectrum_fundamentals-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2611 2023-04-30 18:37:48.694880 spectrum_fundamentals-0.3.1/README.rst
+-rw-r--r--   0        0        0     2367 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      940 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/__init__.py
+-rw-r--r--   0        0        0      381 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/__main__.py
+-rw-r--r--   0        0        0       29 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/annotation/__init__.py
+-rw-r--r--   0        0        0    11153 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/annotation/annotation.py
+-rw-r--r--   0        0        0     1372 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/charge.py
+-rw-r--r--   0        0        0     7819 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/constants.py
+-rw-r--r--   0        0        0    12452 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/fragments.py
+-rw-r--r--   0        0        0       26 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/__init__.py
+-rw-r--r--   0        0        0    14554 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/fragments_ratio.py
+-rw-r--r--   0        0        0     1435 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/metric.py
+-rw-r--r--   0        0        0    22213 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/percolator.py
+-rw-r--r--   0        0        0    22378 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/similarity.py
+-rw-r--r--   0        0        0     9443 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/mod_string.py
+-rw-r--r--   0        0        0        0 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/py.typed
+-rw-r--r--   0        0        0     3856 1970-01-01 00:00:00.000000 spectrum_fundamentals-0.3.1/PKG-INFO
```

### Comparing `spectrum_fundamentals-0.3.0/LICENSE` & `spectrum_fundamentals-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.0/README.rst` & `spectrum_fundamentals-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.0/pyproject.toml` & `spectrum_fundamentals-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectrum_fundamentals"
-version = "0.3.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.3.1"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "Fundamentals public repo"
 authors = ["WassimG <wassim.gabriel@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/wilhelm-lab/spectrum_fundamentals"
 repository = "https://github.com/wilhelm-lab/spectrum_fundamentals"
 documentation = "https://spectrum_fundamentals.readthedocs.io"
```

### Comparing `spectrum_fundamentals-0.3.0/spectrum_fundamentals/__init__.py` & `spectrum_fundamentals-0.3.1/spectrum_fundamentals/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Initialize fundamentals."""
 __author__ = "Victor Giurcoiu"
 __email__ = "victor.giurcoiu@tum.de"
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 import logging
 import logging.handlers
 import sys
 import time
 
 CONSOLE_LOG_LEVEL = logging.INFO
```

### Comparing `spectrum_fundamentals-0.3.0/spectrum_fundamentals/charge.py` & `spectrum_fundamentals-0.3.1/spectrum_fundamentals/charge.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,34 +3,33 @@
 import numpy as np
 
 
 def indices_to_one_hot(labels: Union[int, List[int], np.ndarray], classes: Optional[int] = None) -> np.ndarray:
     """
     Convert a single or a list of labels to one-hot encoding.
 
-    :param labels: The labels to be one-hot encoding. Must be zero-based.
+    :param labels: The labels to be one-hot encoding. Must be one-based.
     :param classes: The number of classes, i.e. the length of the encoding. If omitted, set to the max label + 1.
-
     :raises TypeError: If the type of labels is not understood
     :raises ValueError: If the highest label in labels is larger or equal to the number of classes.
-
     :return: np.ndarray with the one-hot encoded labels.
     """
     if isinstance(labels, int):
         labels = np.array([labels])
     elif isinstance(labels, (list, np.ndarray)):
         labels = np.array(labels)
     else:
         raise TypeError(
             f"Type of labels not understood. Only int, List[int] and np.ndarray are supported. Given: {type(labels)}."
         )
 
     max_label = labels.max()
     if classes is None:
-        classes = max_label + 1
-    if max_label >= classes:
-        raise ValueError("All labels must be smaller to the number of classes.")
+        classes = max_label
+    if max_label > classes:
+        raise ValueError(
+            f"All labels must be smaller or equal to the number of classes. max_label: {max_label}, classes: {classes}"
+        )
 
     one_hot = np.zeros((labels.size, classes), dtype=int)
-    one_hot[np.arange(labels.size), labels] = 1
-
+    one_hot[np.arange(labels.size), labels - 1] = 1
     return one_hot
```

### Comparing `spectrum_fundamentals-0.3.0/spectrum_fundamentals/constants.py` & `spectrum_fundamentals-0.3.1/spectrum_fundamentals/constants.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.0/spectrum_fundamentals/fragments.py` & `spectrum_fundamentals-0.3.1/spectrum_fundamentals/fragments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
-from operator import itemgetter
 from typing import Dict, List, Optional, Tuple
 
 import numpy as np
+import pandas as pd
 
 from . import constants as constants
 
 logger = logging.getLogger(__name__)
 
 
 def _get_modifications(peptide_sequence: str) -> Optional[Tuple[Dict[int, float], int, str]]:
@@ -102,15 +102,15 @@
     for i in range(0, peptide_length):  # generate substrings
         forward_sum += constants.AA_MASSES[peptide_sequence[i]]  # sum left to right
         if i in modification_deltas:  # add mass of modification if present
             forward_sum += modification_deltas[i]
     return forward_sum + ion_type_offsets[0] + ion_type_offsets[1]
 
 
-def initialize_peaks(sequence: str, mass_analyzer: str, charge: int) -> Tuple[List[Dict[str, object]], int, str, float]:
+def initialize_peaks(sequence: str, mass_analyzer: str, charge: int) -> Tuple[pd.DataFrame, int, str, float]:
     """
     Generate theoretical peaks for a modified peptide sequence.
 
     :param sequence: Modified peptide sequence
     :param mass_analyzer: Type of mass analyzer used eg. FTMS, ITMS
     :param charge: Precursor charge
     :raises AssertionError:  if peptide sequence contained an unknown modification. TODO do this within the get_mod func.
@@ -119,17 +119,21 @@
     peptide_sequence = sequence
     modifications = _get_modifications(peptide_sequence)
     if modifications is None:
         raise AssertionError("Modification not found.")
     else:
         modification_deltas, tmt_n_term, peptide_sequence = modifications
 
+    col_dtypes = {"ion_type": str, "no": int, "charge": float, "mass": float, "min_mass": float, "max_mass": float}
     peptide_length = len(peptide_sequence)
+
     if peptide_length > 30:
-        return [], -1, "", 0.0
+        df_out = pd.DataFrame(columns=col_dtypes.keys())
+        df_out = df_out.astype(col_dtypes)
+        return df_out, -1, "", 0.0
 
     # initialize constants
     if int(round(charge)) <= 3:
         max_charge = int(round(charge))
     else:
         max_charge = 3
 
@@ -173,38 +177,48 @@
             # positive charge is introduced by protons (or H - ELECTRON_MASS)
             charge_delta = charge * constants.PARTICLE_MASSES["PROTON"]
             for ion_type in range(0, number_of_ion_types):  # generate all ion types
                 # Check for neutral loss here
                 mass = (ion_type_masses[ion_type] + charge_delta) / charge
                 min_mass, max_mass = get_min_max_mass(mass_analyzer, mass)
                 fragments_meta_data.append(
-                    {
-                        "ion_type": ion_types[ion_type],
-                        "no": i + 1,
-                        "charge": charge,
-                        "mass": mass,
-                        "min_mass": min_mass,
-                        "max_mass": max_mass,
-                    }
+                    [
+                        ion_types[ion_type],  # ion type
+                        i + 1,  # no
+                        charge,  # charge
+                        mass,  # mass
+                        min_mass,  # min mass
+                        max_mass,  # max mass
+                    ]
                 )
-        fragments_meta_data = sorted(fragments_meta_data, key=itemgetter("mass"))
-    return fragments_meta_data, tmt_n_term, peptide_sequence, (forward_sum + ion_type_offsets[0] + ion_type_offsets[1])
+    df_out = pd.DataFrame(data=fragments_meta_data, columns=col_dtypes.keys())
+    df_out.sort_values(by="mass", inplace=True)
+    return df_out, tmt_n_term, peptide_sequence, (forward_sum + ion_type_offsets[0] + ion_type_offsets[1])
 
 
 def get_min_max_mass(mass_analyzer: str, mass: float) -> Tuple[float, float]:
-    """Helper function to get min and max mass based on mass analyzer."""
+    """Helper function to get min and max mass based on mass analyzer.
+
+    :param mass_analyzer: the type of mass analyzer used to determine the tolerance.
+    :param mass: the theoretical fragment mass
+    :raises ValueError: if mass_analyzer is other than one of FTMS, TOF, ITMS
+
+    :return: a tuple (min, max) denoting the mass tolerance range.
+    """
     if mass_analyzer == "FTMS":
         min_mass = (mass * -20 / 1000000) + mass
         max_mass = (mass * 20 / 1000000) + mass
     elif mass_analyzer == "TOF":
         min_mass = (mass * -40 / 1000000) + mass
         max_mass = (mass * 40 / 1000000) + mass
-    else:  # use ITMS otherwise
+    elif mass_analyzer == "ITMS":
         min_mass = mass - 0.35
         max_mass = mass + 0.35
+    else:
+        raise ValueError(f"Unsupported mass_analyzer: {mass_analyzer}")
     return (min_mass, max_mass)
 
 
 def compute_ion_masses(seq_int: List[int], charge_onehot: List[int], tmt: str = "") -> Optional[np.ndarray]:
     """
     Collects an integer sequence e.g. [1,2,3] with charge 2 and returns array with 174 positions for ion masses.
```

### Comparing `spectrum_fundamentals-0.3.0/spectrum_fundamentals/metrics/fragments_ratio.py` & `spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/fragments_ratio.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.0/spectrum_fundamentals/metrics/metric.py` & `spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.0/spectrum_fundamentals/metrics/percolator.py` & `spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/percolator.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         self,
         metadata: pd.DataFrame,
         input_type: str,
         pred_intensities: Optional[Union[np.ndarray, scipy.sparse.csr_matrix]] = None,
         true_intensities: Optional[Union[np.ndarray, scipy.sparse.csr_matrix]] = None,
         mz: Optional[Union[np.ndarray, scipy.sparse.csr_matrix]] = None,
         all_features_flag: bool = False,
-        regression_method: str = lowess,
+        regression_method: str = "lowess",
         fdr_cutoff: float = 0.01,
     ):
         """Initialize a Percolator obj."""
         self.metadata = metadata
         self.input_type = input_type
         self.all_features_flag = all_features_flag
         self.regression_method = regression_method
@@ -96,70 +96,68 @@
         return retention_time_df.reset_index(level=0, drop=True).index
 
     @staticmethod
     def get_aligned_predicted_retention_times(
         observed_retention_times_fdr_filtered: Union[np.ndarray, pd.Series],
         predicted_retention_times_fdr_filtered: Union[np.ndarray, pd.Series],
         predicted_retention_times_all: Union[np.ndarray, pd.Series],
-        curve_fitting_method: Optional[str] = "lowess",
+        curve_fitting_method: str = "lowess",
     ) -> np.ndarray:
         """
         Apply regression to find a mapping from predicted iRT values to experimental retention times.
 
         :param observed_retention_times_fdr_filtered: observed retention times after FDR filter
         :param predicted_retention_times_fdr_filtered: predicted retention times after FDR filter
         :param predicted_retention_times_all: all predicted retention times
-        :param curve_fitting_method: method for curve fitting (lowess, spline, or logistic regression)
+        :param curve_fitting_method: method for curve fitting (lowess, spline, or logistic)
         :return: aligned predicted retention times
         """
         observed_rts = np.array(observed_retention_times_fdr_filtered, dtype=np.float64)
         predicted_rts = np.array(predicted_retention_times_fdr_filtered, dtype=np.float64)
 
-        # TODO: use Akaike information criterion to choose a good value for frac
-        frac = 0.5  # Between 0 and 1. The fraction of the data used when estimating each y-value.
         it = 0  # The number of residual-based reweightings to perform. Don't use the iterative reweighting (it > 1),
         # this result in NaNs
+
+        # TODO: use Akaike information criterion to choose a good value for frac
+        frac = 0.5  # Between 0 and 1. The fraction of the data used when estimating each y-value.
+
+        fit_func = get_fitting_func(curve_fitting_method)
         discard_percentage = 0.1  # in percents, so 0.1 = 0.1% (not 10%!)
+        median_abs_error = 1.0
+
+        while discard_percentage < 50.0 and median_abs_error > 0.02:
+            params = fit_func(predicted_rts, observed_rts)
+            aligned_rts_predicted = params[0]
 
-        if curve_fitting_method == "lowess":
-            lowess_model = lowess.Lowess()
-        elif curve_fitting_method == "spline":
-            # spline works only with unique values
-            predicted_rts, indices = np.unique(predicted_rts, return_index=True)
-            observed_rts = observed_rts[indices]
-
-        if curve_fitting_method == "logistic":
-            (a_, b_, c_, d_), _ = opt.curve_fit(f, predicted_rts, observed_rts, method="lm")
-            return f(predicted_retention_times_all, a_, b_, c_, d_)
-        while discard_percentage < 50.0:
-            if curve_fitting_method == "spline":
-                aligned_rts_predicted, t, c, k = spline(2, predicted_rts, observed_rts, predicted_rts)
-            else:
-                lowess_model.fit(predicted_rts, observed_rts, frac=frac, robust_iters=it)
-                aligned_rts_predicted = lowess_model.predict(predicted_rts)
             abs_errors = np.abs(aligned_rts_predicted - observed_rts)
             cut_off = np.percentile(abs_errors, 100 - discard_percentage)
             median_abs_error = np.median(np.abs(abs_errors))
+
             logger.debug(f"Median absolute error aligned rts: {median_abs_error}")
 
             if median_abs_error > 0.02:
                 keep_idxs = np.nonzero(abs_errors < cut_off)
                 observed_rts = observed_rts[keep_idxs[0]]
                 predicted_rts = predicted_rts[keep_idxs[0]]
-            else:
-                break
-            discard_percentage *= 1.5
+
+                discard_percentage *= 1.5
 
         logger.debug(f"Observed RT anchor points:\n{observed_retention_times_fdr_filtered}")
         logger.debug(f"Predicted RT anchor points:\n{predicted_retention_times_fdr_filtered}")
 
         if curve_fitting_method == "spline":
-            aligned_rts_predicted = interpolate.BSpline(t, c, k)(predicted_retention_times_all)
-        else:
+            aligned_rts_predicted = interpolate.BSpline(*params[1:])(predicted_retention_times_all)
+        elif curve_fitting_method == "lowess":
+            lowess_model = lowess.Lowess()
+            lowess_model.fit(predicted_rts, observed_rts, frac=frac, robust_iters=it)
             aligned_rts_predicted = lowess_model.predict(np.array(predicted_retention_times_all))
+        else:  # logistic
+            aligned_rts_predicted = logistic(
+                predicted_retention_times_all, *opt.curve_fit(logistic, predicted_rts, observed_rts, method="lm")[0]
+            )
 
         return aligned_rts_predicted
 
     @staticmethod
     def get_scannr(metadata_subset: Union[pd.Series, Tuple[str, int]]) -> int:
         """
         Creates a hash of the raw_file and scan number to use as a unique scan number in percolator.
@@ -424,17 +422,18 @@
             if lda_failed:
                 sampled_idxs = Percolator.sample_balanced_over_bins(self.metadata[["RETENTION_TIME", "PREDICTED_IRT"]])
             else:
                 sampled_idxs = Percolator.sample_balanced_over_bins(
                     self.metadata[["RETENTION_TIME", "PREDICTED_IRT"]].iloc[idxs_below_lda_fdr, :]
                 )
 
+            file_sample = self.metadata.iloc[sampled_idxs].sort_values("PREDICTED_IRT")
             aligned_predicted_rts = Percolator.get_aligned_predicted_retention_times(
-                self.metadata["RETENTION_TIME"][sampled_idxs],
-                self.metadata["PREDICTED_IRT"][sampled_idxs],
+                file_sample["RETENTION_TIME"],
+                file_sample["PREDICTED_IRT"],
                 self.metadata["PREDICTED_IRT"],
                 self.regression_method,
             )
 
             self.metrics_val["RT"] = self.metadata["RETENTION_TIME"]
             self.metrics_val["pred_RT"] = self.metadata["PREDICTED_IRT"]
             self.metrics_val["iRT"] = aligned_predicted_rts
@@ -459,19 +458,39 @@
             self.metrics_val["andromeda_delta_score"] = Percolator.get_delta_score(
                 self.metrics_val[["ScanNr", "andromeda"]], "andromeda"
             )
 
         self._reorder_columns_for_percolator()
 
 
-def spline(knots: int, x: np.ndarray, y: np.ndarray, x_full: np.ndarray):
+def get_fitting_func(curve_fitting_method: str):
+    """
+    Retrieve the correct function given a curve fitting method.
+
+    :param curve_fitting_method: method for curve fitting (lowess, spline, or logistic)
+    :raises ValueError: if an invalid curve_fitting_method is supplied
+    :return: Callable that accepts x and y, i.e. fit_func(x,y) where x are the data points and y
+        are the corresponding measures for which the fit should be done.
+    """
+    if curve_fitting_method == "logistic":
+        return lambda x, y: (logistic(x, *opt.curve_fit(logistic, x, y, method="lm")[0]),)
+    elif curve_fitting_method == "lowess":
+        return lambda x, y: (lowess.lowess_fit_and_predict(x, y, frac=0.5),)
+    elif curve_fitting_method == "spline":
+        return lambda x, y: spline(2, x, y)
+    else:
+        raise ValueError("curve_fitting_method should be one of the following strings: lowess, spline, logistic.")
+
+
+def spline(knots: int, x: np.ndarray, y: np.ndarray):
     """Calculates spline fitting."""
     x_new = np.linspace(0, 1, knots + 2)[1:-1]
     q_knots = np.quantile(x, x_new)
     t, c, k = interpolate.splrep(x, y, t=q_knots, s=2)
-    yfit = interpolate.BSpline(t, c, k)(x_full)
+    yfit = interpolate.BSpline(t, c, k)(x)
     return yfit, t, c, k
 
 
-def f(x: Union[pd.Series, np.ndarray], a: float, b: float, c: float, d: float):
+def logistic(x: Union[pd.Series, np.ndarray], a: float, b: float, c: float, d: float):
     """Calculates logistic regression function."""
-    return a / (1.0 + np.exp(-c * (x - d))) + b
+    exponent = np.clip(-c * (x - d), -700, 700)  # make this stable, i.e. avoid 0.0 or inf
+    return a / (1.0 + np.exp(exponent)) + b
```

### Comparing `spectrum_fundamentals-0.3.0/spectrum_fundamentals/metrics/similarity.py` & `spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/similarity.py`

 * *Files 6% similar despite different names*

```diff
@@ -328,17 +328,15 @@
             if np.isnan(diff):
                 diff = 0
             diff_values.append(diff)
 
         return diff_values
 
     @staticmethod
-    def calculate_quantiles(
-        observed: scipy.sparse.csr_matrix, predicted: scipy.sparse.csr_matrix, quantile: str
-    ) -> float:
+    def calculate_quantiles(observed: np.ndarray, predicted: np.ndarray, quantile: str) -> float:
         """
         Helper function to calculcate quantiles.
 
         :param observed: observed intensities
         :param predicted: predicted intensities
         :param quantile: quantile method
         :return: calculated quantile
@@ -361,15 +359,16 @@
         Calculate modified cosine similarity as defined in Chris D. McGann et al. (Real-time spectral library \
         matching for sample multiplexed quantitative proteomics).
 
         :param observed_intensities: observed intensities, constants.EPSILON intensity indicates zero intensity peaks, \
                                      0 intensity indicates invalid peaks (charge state > peptide charge state or \
                                      position >= peptide length), array of length 174
         :param predicted_intensities: predicted intensities, see observed_intensities for details, array of length 174
-        :param mz: observed mz values
+        :param observed_mz: observed mz values
+        :param theoretical_mz: theoretical mz values
         :return: calculates cosine values
         """
         epsilon = 1e-7
         observed_normalized = SimilarityMetrics.unit_normalization(observed_intensities)
         predicted_normalized = SimilarityMetrics.unit_normalization(predicted_intensities)
 
         if isinstance(observed_normalized, scipy.sparse.csr_matrix):
@@ -421,44 +420,36 @@
         self.metrics_val["modified_cosine"] = SimilarityMetrics.modified_cosine(
             self.true_intensities, self.pred_intensities, self.mz, self.mz
         )
         if all_features:
             self.metrics_val["spectral_entropy_similarity"] = SimilarityMetrics.spectral_entropy_similarity(
                 self.true_intensities, self.pred_intensities
             )
-            self.metrics_val["spectral_angle_single_charge"] = SimilarityMetrics.spectral_angle(
-                self.true_intensities, self.pred_intensities, 1
-            )
-            self.metrics_val["spectral_angle_double_charge"] = SimilarityMetrics.spectral_angle(
-                self.true_intensities, self.pred_intensities, 2
-            )
-            self.metrics_val["spectral_angle_triple_charge"] = SimilarityMetrics.spectral_angle(
-                self.true_intensities, self.pred_intensities, 3
-            )
-            self.metrics_val["spectral_angle_b_ions"] = SimilarityMetrics.spectral_angle(
-                self.true_intensities, self.pred_intensities, 4
-            )
-            self.metrics_val["spectral_angle_y_ions"] = SimilarityMetrics.spectral_angle(
-                self.true_intensities, self.pred_intensities, 5
-            )
-            self.metrics_val["pearson_corr_single_charge"] = SimilarityMetrics.correlation(
-                self.true_intensities, self.pred_intensities, 1, "pearson"
-            )
-            self.metrics_val["pearson_corr_double_charge"] = SimilarityMetrics.correlation(
-                self.true_intensities, self.pred_intensities, 2, "pearson"
-            )
-            self.metrics_val["pearson_corr_triple_charge"] = SimilarityMetrics.correlation(
-                self.true_intensities, self.pred_intensities, 3, "pearson"
-            )
-            self.metrics_val["pearson_corr_b_ions"] = SimilarityMetrics.correlation(
-                self.true_intensities, self.pred_intensities, 4, "pearson"
-            )
-            self.metrics_val["pearson_corr_y_ions"] = SimilarityMetrics.correlation(
-                self.true_intensities, self.pred_intensities, 5, "pearson"
-            )
+
+            col_names_spectral_angle = [
+                f"spectral_angle_{amount}_charge" for amount in ["single", "double", "triple"]
+            ] + ["spectral_angle_b_ions", "spectral_angle_y_ions"]
+            col_names_pearson_corr = [f"pearson_corr_{amount}_charge" for amount in ["single", "double", "triple"]] + [
+                "pearson_corr_b_ions",
+                "pearson_corr_y_ions",
+            ]
+            col_names_spearman_corr = [
+                f"spearman_corr_{amount}_charge" for amount in ["single", "double", "triple"]
+            ] + ["spearman_corr_b_ions", "spearman_corr_y_ions"]
+
+            for i, col_name_spectral_angle in enumerate(col_names_spectral_angle):
+                self.metrics_val[col_name_spectral_angle] = SimilarityMetrics.spectral_angle(
+                    self.true_intensities, self.pred_intensities, i + 1
+                )
+
+            for i, col_name_pearson_corr in enumerate(col_names_pearson_corr):
+                self.metrics_val[col_name_pearson_corr] = SimilarityMetrics.correlation(
+                    self.true_intensities, self.pred_intensities, i + 1, "pearson"
+                )
+
             self.metrics_val["cos"] = SimilarityMetrics.cos(self.true_intensities, self.pred_intensities)
             self.metrics_val["mean_abs_diff"] = SimilarityMetrics.abs_diff(
                 self.true_intensities, self.pred_intensities, "mean"
             )
             self.metrics_val["std_abs_diff"] = SimilarityMetrics.abs_diff(
                 self.true_intensities, self.pred_intensities, "std"
             )
@@ -477,22 +468,12 @@
             self.metrics_val["max_abs_diff"] = SimilarityMetrics.abs_diff(
                 self.true_intensities, self.pred_intensities, "max"
             )
             self.metrics_val["mse"] = SimilarityMetrics.abs_diff(self.true_intensities, self.pred_intensities, "mse")
             self.metrics_val["spearman_corr"] = SimilarityMetrics.correlation(
                 self.true_intensities, self.pred_intensities, 0, "spearman"
             )
-            self.metrics_val["spearman_corr_single_charge"] = SimilarityMetrics.correlation(
-                self.true_intensities, self.pred_intensities, 1, "spearman"
-            )
-            self.metrics_val["spearman_corr_double_charge"] = SimilarityMetrics.correlation(
-                self.true_intensities, self.pred_intensities, 2, "spearman"
-            )
-            self.metrics_val["spearman_corr_triple_charge"] = SimilarityMetrics.correlation(
-                self.true_intensities, self.pred_intensities, 3, "spearman"
-            )
-            self.metrics_val["spearman_corr_b_ions"] = SimilarityMetrics.correlation(
-                self.true_intensities, self.pred_intensities, 4, "spearman"
-            )
-            self.metrics_val["spearman_corr_y_ions"] = SimilarityMetrics.correlation(
-                self.true_intensities, self.pred_intensities, 5, "spearman"
-            )
+
+            for i, col_name_spearman_corr in enumerate(col_names_spearman_corr):
+                self.metrics_val[col_name_spearman_corr] = SimilarityMetrics.correlation(
+                    self.true_intensities, self.pred_intensities, i + 1, "spearman"
+                )
```

### Comparing `spectrum_fundamentals-0.3.0/spectrum_fundamentals/mod_string.py` & `spectrum_fundamentals-0.3.1/spectrum_fundamentals/mod_string.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,31 +4,34 @@
 from typing import Dict, List, Optional, Tuple
 
 from .constants import MAXQUANT_VAR_MODS, MOD_MASSES, MOD_NAMES, SPECTRONAUT_MODS
 
 
 def internal_to_spectronaut(sequences: List[str]) -> List[str]:
     """
-    Function to translate a modstring from the interal format to the spectronaut format.
+    Function to translate a modstring from the internal format to the spectronaut format.
 
     :param sequences: List[str] of sequences
     :return: List[str] of modified sequences
     """
     regex = re.compile("(%s)" % "|".join(map(re.escape, SPECTRONAUT_MODS.keys())))
     return [regex.sub(lambda mo: SPECTRONAUT_MODS[mo.string[mo.start() : mo.end()]], seq) for seq in sequences]
 
 
 def maxquant_to_internal(sequences: List[str], fixed_mods: Optional[Dict[str, str]] = None) -> List[str]:
     """
     Function to translate a MaxQuant modstring to the Prosit format.
 
     :param sequences: List[str] of sequences
-    :param fixed_mods: Optional dictionary of modifications with key aa and value mod, e.g. 'M': 'M(UNIMOD:35)'. Fixed \
-    modifications must be included in the variable modificatons dictionary throws Assertion error otherwise
-    :return: List[str] of modified sequences
+    :param fixed_mods: Optional dictionary of modifications with key aa and value mod, e.g. 'M': 'M(UNIMOD:35)'.
+        Fixed modifications must be included in the variable modificatons dictionary.
+        By default, i.e. if nothing is supplied to fixed_mods, carbamidomethylation on cystein will be included
+        in the fixed modifications. If you want to have no fixed modifictions at all, supply fixed_mods={}
+    :raises AssertionError: if illegal modification was provided in the fixed_mods dictionary.
+    :return: a list of modified sequences
     """
     if fixed_mods is None:
         fixed_mods = {"C": "C[UNIMOD:4]"}
     err_msg = f"Provided illegal fixed mod, supported modifications are {set(MAXQUANT_VAR_MODS.values())}."
     assert all(x in MAXQUANT_VAR_MODS.values() for x in fixed_mods.values()), err_msg
 
     replacements = {**MAXQUANT_VAR_MODS, **fixed_mods}
@@ -151,15 +154,15 @@
         # Ugly and fast fix for reading modifications as is from maxquant we should reconsider how to fix it.
         # sequence = sequence.replace('M(ox)','M(U:35)')
         # sequence = sequence.replace('C','C(U:4)')
         split_seq = r_pattern.findall(sequence)
         if "".join(split_seq) == sequence:
             if translate:
                 return [alphabet[aa] for aa in split_seq]
-            elif not translate:
+            else:
                 return split_seq
         elif filter:
             return [0]
         else:
             not_parsable_elements = "".join(
                 [li[2] for li in difflib.ndiff(sequence, "".join(split_seq)) if li[0] == "-"]
             )
@@ -170,15 +173,15 @@
     pattern = sorted(alphabet, key=len, reverse=True)
 
     pattern = [re.escape(i) for i in pattern]
     regex_pattern = re.compile("|".join(pattern))
     return map(split_modstring, sequences, repeat(regex_pattern))
 
 
-def proteomicsdb_to_internal(sequence: str, mods_variable: str, mods_fixed: str) -> str:
+def proteomicsdb_to_internal(sequence: str, mods_variable: str = "", mods_fixed: str = "") -> str:
     """
     Function to create a sequence with UNIMOD modifications from given sequence and it's varaible and fixed modifications.
 
     :param sequence: The sequence to modify
     :param mods_variable: the variable modifacations (e.g. "Oxidation@M45")
     :param mods_fixed: the fixed modifacations (e.g. "Carbamidomethyl@C")
     :return: sequence with unimods (e.g."AAC[UNIMOD:4]GHK")
@@ -199,18 +202,19 @@
     # Tag all the modified AAs to replace them with UNIMOD later
     for count in range(len(mods_list)):
         mod_and_position = mods_list[count]
         amino_acid = mod_and_position[1][0]
 
         if len(mod_and_position[1]) > 1:
             position = int(mod_and_position[1][1:])
-            if not position == 0 and not position > len(sequence):
-                sequence = sequence[: position - 1] + mods_dict[amino_acid] + sequence[position:]
-            elif position == 0:
+            if position == 0:
                 mod_at_start = True
+            else:
+                if position <= len(sequence):
+                    sequence = sequence[: position - 1] + mods_dict[amino_acid] + sequence[position:]
 
         elif len(mod_and_position[1]) == 1:
             sequence = sequence.replace(amino_acid, mods_dict[amino_acid])
 
     sequence = sequence.replace("m", "M[UNIMOD:35]")
     sequence = sequence.replace("c", "C[UNIMOD:4]")
     sequence = sequence.replace("k", "K[UNIMOD:737]")
```

### Comparing `spectrum_fundamentals-0.3.0/PKG-INFO` & `spectrum_fundamentals-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum-fundamentals
-Version: 0.3.0
+Version: 0.3.1
 Summary: Fundamentals public repo
 Home-page: https://github.com/wilhelm-lab/spectrum_fundamentals
 License: MIT
 Author: WassimG
 Author-email: wassim.gabriel@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

