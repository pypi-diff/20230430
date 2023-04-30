# Comparing `tmp/stepmix-1.0.0.tar.gz` & `tmp/stepmix-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepmix-1.0.0.tar", last modified: Thu Apr  6 20:42:12 2023, max compression
+gzip compressed data, was "stepmix-1.0.1.tar", last modified: Sun Apr 30 21:21:57 2023, max compression
```

## Comparing `stepmix-1.0.0.tar` & `stepmix-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      954 2023-01-11 22:01:14.079040 stepmix-1.0.0/.github/workflows/pytest.yaml
--rw-r--r--   0        0        0       54 2023-01-11 22:01:14.079040 stepmix-1.0.0/.gitignore
--rw-r--r--   0        0        0      309 2023-01-11 22:01:14.079040 stepmix-1.0.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1068 2023-01-11 22:01:14.079040 stepmix-1.0.0/LICENSE
--rw-r--r--   0        0        0     2428 2023-04-06 20:40:02.587187 stepmix-1.0.0/README-dev.md
--rw-r--r--   0        0        0     4831 2023-03-31 15:18:45.991430 stepmix-1.0.0/README.md
--rw-r--r--   0        0        0      638 2023-01-11 22:01:14.079040 stepmix-1.0.0/docs/Makefile
--rw-r--r--   0        0        0      764 2023-01-11 22:01:14.079040 stepmix-1.0.0/docs/make.bat
--rw-r--r--   0        0        0      929 2023-01-11 22:01:14.079040 stepmix-1.0.0/docs/source/api.rst
--rw-r--r--   0        0        0     1016 2023-04-06 20:41:49.179379 stepmix-1.0.0/docs/source/conf.py
--rw-r--r--   0        0        0      955 2023-01-11 22:01:14.083040 stepmix-1.0.0/docs/source/index.rst
--rw-r--r--   0        0        0      283 2023-03-31 15:25:56.504322 stepmix-1.0.0/docs/source/installation.rst
--rw-r--r--   0        0        0     2814 2023-01-11 22:01:14.083040 stepmix-1.0.0/docs/source/tutorials.rst
--rw-r--r--   0        0        0     1872 2023-04-06 20:41:49.179379 stepmix-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      579 2023-04-03 16:48:45.082884 stepmix-1.0.0/scripts/README.md
--rwxr-xr-x   0        0        0     5603 2023-03-09 18:24:49.769774 stepmix-1.0.0/scripts/run_bakk_simulation.py
--rwxr-xr-x   0        0        0     4996 2023-03-09 22:19:26.676204 stepmix-1.0.0/scripts/run_bakk_simulation_complete.py
--rw-r--r--   0        0        0      174 2023-04-06 20:41:49.179379 stepmix-1.0.0/stepmix/__init__.py
--rw-r--r--   0        0        0     8113 2023-01-11 22:01:14.083040 stepmix-1.0.0/stepmix/bootstrap.py
--rw-r--r--   0        0        0     2033 2023-01-11 22:01:14.083040 stepmix-1.0.0/stepmix/corrections.py
--rw-r--r--   0        0        0    11630 2023-03-09 22:19:26.676204 stepmix-1.0.0/stepmix/datasets.py
--rw-r--r--   0        0        0        0 2023-01-11 22:01:14.083040 stepmix-1.0.0/stepmix/emission/__init__.py
--rw-r--r--   0        0        0     1660 2023-01-11 22:01:14.083040 stepmix-1.0.0/stepmix/emission/build_emission.py
--rw-r--r--   0        0        0     6283 2023-03-09 22:19:26.676204 stepmix-1.0.0/stepmix/emission/categorical.py
--rw-r--r--   0        0        0     4831 2023-03-09 21:04:30.147441 stepmix-1.0.0/stepmix/emission/covariate.py
--rw-r--r--   0        0        0     6031 2023-01-11 22:01:14.083040 stepmix-1.0.0/stepmix/emission/emission.py
--rw-r--r--   0        0        0    15489 2023-01-12 20:57:50.331048 stepmix-1.0.0/stepmix/emission/gaussian.py
--rw-r--r--   0        0        0     4681 2023-03-09 22:19:26.676204 stepmix-1.0.0/stepmix/emission/nested.py
--rw-r--r--   0        0        0    52639 2023-03-09 18:24:49.769774 stepmix-1.0.0/stepmix/stepmix.py
--rw-r--r--   0        0        0    17894 2023-03-09 22:19:26.676204 stepmix-1.0.0/stepmix/utils.py
--rw-r--r--   0        0        0     4074 2023-03-09 22:19:26.676204 stepmix-1.0.0/test/conftest.py
--rw-r--r--   0        0        0     3608 2023-03-09 22:19:26.676204 stepmix-1.0.0/test/test_benchmarks.py
--rw-r--r--   0        0        0     4499 2023-01-11 22:01:14.083040 stepmix-1.0.0/test/test_bootstrap.py
--rw-r--r--   0        0        0     8163 2023-03-09 22:19:26.676204 stepmix-1.0.0/test/test_emission.py
--rw-r--r--   0        0        0     1479 2023-01-11 22:01:14.083040 stepmix-1.0.0/test/test_fiml.py
--rw-r--r--   0        0        0     1001 2023-01-11 22:01:14.083040 stepmix-1.0.0/test/test_inputs.py
--rw-r--r--   0        0        0     4284 2023-03-09 18:24:49.769774 stepmix-1.0.0/test/test_random_state.py
--rw-r--r--   0        0        0      795 2023-01-11 22:01:14.083040 stepmix-1.0.0/test/test_sklearn.py
--rw-r--r--   0        0        0     4570 2023-01-11 22:01:14.083040 stepmix-1.0.0/test/test_steps.py
--rw-r--r--   0        0        0     6095 1970-01-01 00:00:00.000000 stepmix-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      954 2023-01-11 22:01:14.079040 stepmix-1.0.1/.github/workflows/pytest.yaml
+-rw-r--r--   0        0        0       54 2023-01-11 22:01:14.079040 stepmix-1.0.1/.gitignore
+-rw-r--r--   0        0        0      309 2023-01-11 22:01:14.079040 stepmix-1.0.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1068 2023-01-11 22:01:14.079040 stepmix-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2428 2023-04-25 21:29:34.007800 stepmix-1.0.1/README-dev.md
+-rw-r--r--   0        0        0     5261 2023-04-30 21:21:22.007846 stepmix-1.0.1/README.md
+-rw-r--r--   0        0        0      638 2023-01-11 22:01:14.079040 stepmix-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0      764 2023-01-11 22:01:14.079040 stepmix-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0      929 2023-01-11 22:01:14.079040 stepmix-1.0.1/docs/source/api.rst
+-rw-r--r--   0        0        0     1016 2023-04-30 21:21:22.007846 stepmix-1.0.1/docs/source/conf.py
+-rw-r--r--   0        0        0      955 2023-01-11 22:01:14.083040 stepmix-1.0.1/docs/source/index.rst
+-rw-r--r--   0        0        0      283 2023-04-25 21:29:34.007800 stepmix-1.0.1/docs/source/installation.rst
+-rw-r--r--   0        0        0     2814 2023-01-11 22:01:14.083040 stepmix-1.0.1/docs/source/tutorials.rst
+-rw-r--r--   0        0        0     1872 2023-04-30 21:21:22.007846 stepmix-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      579 2023-04-25 21:29:34.007800 stepmix-1.0.1/scripts/README.md
+-rwxr-xr-x   0        0        0     5603 2023-03-09 18:24:49.769774 stepmix-1.0.1/scripts/run_bakk_simulation.py
+-rwxr-xr-x   0        0        0     4996 2023-03-09 22:19:26.676204 stepmix-1.0.1/scripts/run_bakk_simulation_complete.py
+-rw-r--r--   0        0        0      174 2023-04-30 21:21:22.007846 stepmix-1.0.1/stepmix/__init__.py
+-rw-r--r--   0        0        0     8113 2023-01-11 22:01:14.083040 stepmix-1.0.1/stepmix/bootstrap.py
+-rw-r--r--   0        0        0     2033 2023-01-11 22:01:14.083040 stepmix-1.0.1/stepmix/corrections.py
+-rw-r--r--   0        0        0    11630 2023-03-09 22:19:26.676204 stepmix-1.0.1/stepmix/datasets.py
+-rw-r--r--   0        0        0        0 2023-01-11 22:01:14.083040 stepmix-1.0.1/stepmix/emission/__init__.py
+-rw-r--r--   0        0        0     1660 2023-01-11 22:01:14.083040 stepmix-1.0.1/stepmix/emission/build_emission.py
+-rw-r--r--   0        0        0     6283 2023-03-09 22:19:26.676204 stepmix-1.0.1/stepmix/emission/categorical.py
+-rw-r--r--   0        0        0     4831 2023-03-09 21:04:30.147441 stepmix-1.0.1/stepmix/emission/covariate.py
+-rw-r--r--   0        0        0     6031 2023-01-11 22:01:14.083040 stepmix-1.0.1/stepmix/emission/emission.py
+-rw-r--r--   0        0        0    15489 2023-01-12 20:57:50.331048 stepmix-1.0.1/stepmix/emission/gaussian.py
+-rw-r--r--   0        0        0     4681 2023-03-09 22:19:26.676204 stepmix-1.0.1/stepmix/emission/nested.py
+-rw-r--r--   0        0        0    52639 2023-03-09 18:24:49.769774 stepmix-1.0.1/stepmix/stepmix.py
+-rw-r--r--   0        0        0    18189 2023-04-30 21:21:22.007846 stepmix-1.0.1/stepmix/utils.py
+-rw-r--r--   0        0        0     4074 2023-03-09 22:19:26.676204 stepmix-1.0.1/test/conftest.py
+-rw-r--r--   0        0        0     3608 2023-03-09 22:19:26.676204 stepmix-1.0.1/test/test_benchmarks.py
+-rw-r--r--   0        0        0     4499 2023-01-11 22:01:14.083040 stepmix-1.0.1/test/test_bootstrap.py
+-rw-r--r--   0        0        0     8818 2023-04-30 21:21:22.007846 stepmix-1.0.1/test/test_emission.py
+-rw-r--r--   0        0        0     1479 2023-01-11 22:01:14.083040 stepmix-1.0.1/test/test_fiml.py
+-rw-r--r--   0        0        0     1781 2023-04-30 21:21:22.007846 stepmix-1.0.1/test/test_inputs.py
+-rw-r--r--   0        0        0     4284 2023-03-09 18:24:49.769774 stepmix-1.0.1/test/test_random_state.py
+-rw-r--r--   0        0        0      795 2023-01-11 22:01:14.083040 stepmix-1.0.1/test/test_sklearn.py
+-rw-r--r--   0        0        0     4570 2023-01-11 22:01:14.083040 stepmix-1.0.1/test/test_steps.py
+-rw-r--r--   0        0        0     6525 1970-01-01 00:00:00.000000 stepmix-1.0.1/PKG-INFO
```

### Comparing `stepmix-1.0.0/.github/workflows/pytest.yaml` & `stepmix-1.0.1/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/LICENSE` & `stepmix-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/README-dev.md` & `stepmix-1.0.1/README-dev.md`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/README.md` & `stepmix-1.0.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -2,83 +2,101 @@
 ==============================
 <a href="https://pypi.org/project/stepmix/"><img src="https://badge.fury.io/py/stepmix.svg" alt="PyPI version"></a>
 [![Build](https://github.com/Labo-Lacourse/stepmix/actions/workflows/pytest.yaml/badge.svg)](https://github.com/Labo-Lacourse/stepmix/actions/workflows/pytest.yaml)
 [![Documentation Status](https://readthedocs.org/projects/stepmix/badge/?version=latest)](https://stepmix.readthedocs.io/en/latest/index.html)
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 [![Downloads](https://static.pepy.tech/badge/stepmix)](https://pepy.tech/project/stepmix)
 [![Downloads](https://static.pepy.tech/badge/stepmix/month)](https://pepy.tech/project/stepmix)
+[![arXiv](https://img.shields.io/badge/arXiv-2304.03853-b31b1b.svg)](https://arxiv.org/abs/2304.03853)
 
 *For StepMixR, please refer to <a href="https://github.com/Labo-Lacourse/stepmixr">this repository.</a>*
 
 A Python package following the scikit-learn API for model-based clustering and generalized mixture modeling (latent class/profile analysis) of continuous and categorical data. 
 StepMix handles missing values through Full Information Maximum Likelihood (FIML) and provides multiple stepwise Expectation-Maximization (EM) estimation methods based on pseudolikelihood theory. 
 Additional features include support for covariates and distal outcomes, various simulation utilities, and non-parametric bootstrapping, which allows inference
 in semi-supervised and unsupervised settings.
 
+# Reference
+If you find StepMix useful, please consider citing our [arXiv preprint](https://arxiv.org/abs/2304.03853):
+```
+@article{morin2023stepmix,
+  title={StepMix: A Python Package for Pseudo-Likelihood Estimation of Generalized Mixture Models with External Variables},
+  author={Morin, Sacha and Legault, Robin and Bakk, Zsuzsa and Gigu{\`e}re, Charles-{\'E}douard and de la Sablonni{\`e}re, Roxane and Lacourse, {\'E}ric},
+  journal={arXiv preprint arXiv:2304.03853},
+  year={2023}
+}
+```
+
 
 # Install
-You can install StepMix with pip, preferably in a virtual environment : 
+You can install StepMix with pip, preferably in a virtual environment: 
 ```
 pip install stepmix
 ``` 
+# Quickstart
+A simple StepMix mixture using the continuous variables of the Iris Dataset:
+
+```python
+import pandas as pd
+from sklearn.datasets import load_iris
+from sklearn.metrics import rand_score
+
+from stepmix.stepmix import StepMix
+
+# Load dataset in a Dataframe
+data_continuous, target = load_iris(return_X_y=True, as_frame=True)
+
+# Continuous StepMix Model with 3 latent classes
+model = StepMix(n_components=3, measurement="continuous", verbose=0, random_state=123)
+
+# Fit model and predict clusters
+model.fit(data_continuous)
+pred_continuous = model.predict(data_continuous)
+
+# A Rand score close to 1 indicates good alignment between clusters and flower types
+print(rand_score(pred_continuous, target))
+```
+StepMix also provides support for categorical mixtures:
+
+```python
+# Create categorical data based on the Iris Dataset quantiles
+data_categorical = data_continuous.copy()
+for col in data_categorical:
+   data_categorical[col] = pd.qcut(data_continuous[col], q=3).cat.codes
+
+# Categorical StepMix Model with 3 latent classes
+model = StepMix(n_components=3, measurement="categorical", verbose=0, random_state=123)
+
+# Fit model and predict clusters
+model.fit(data_categorical)
+pred_categorical = model.predict(data_categorical)
+
+# A Rand score close to 1 indicates good alignment between clusters and flower types
+print(rand_score(pred_categorical, target))
+```
+Please refer to the StepMix tutorials to learn how to handle missing values and combine continuous and categorical data in the same model.
 # Tutorials
-Detailed tutorials are available in notebooks : 
-1. [Generalized Mixture Models with StepMix](https://colab.research.google.com/drive/1KAxcvxjL_vB2lAG9e47we7hrf_2fR1eK?usp=sharing) : 
+Detailed tutorials are available in notebooks: 
+1. [Generalized Mixture Models with StepMix](https://colab.research.google.com/drive/1KAxcvxjL_vB2lAG9e47we7hrf_2fR1eK?usp=sharing): 
 an in-depth look at how latent class models can be defined with StepMix. The tutorial uses the Iris Dataset as an example
-and covers :
+and covers:
    1. Continuous LCA models (latent profile analysis/gaussian mixture model);
    2. Binary LCA models;
    3. Categorical LCA models;
    3. Mixed variables mixture models (continuous and categorical data);
    5. Missing Values through Full-Information Maximum Likelihood.
-2. [Stepwise Estimation with StepMix](https://colab.research.google.com/drive/1T_UObkN5Y-iFTKiun0zOkKk7LjtMeV25?usp=sharing) :
+2. [Stepwise Estimation with StepMix](https://colab.research.google.com/drive/1T_UObkN5Y-iFTKiun0zOkKk7LjtMeV25?usp=sharing):
     a tutorial demonstrating how to define measurement and structural models. The tutorial discusses:
    1. LCA models with distal outcomes;
    2. LCA models with covariates; 
    3. 1-step, 2-step and 3-step estimation;
    4. Corrections (BCH or ML) and other options for 3-step estimation.
-3. [Model Selection](https://colab.research.google.com/drive/1iyFTD-D2wn88_vd-qxXkovIuWHRtU7V8?usp=sharing) :
+3. [Model Selection](https://colab.research.google.com/drive/1iyFTD-D2wn88_vd-qxXkovIuWHRtU7V8?usp=sharing):
    a short tutorial discussing:
     1. Selecting the number of components in a mixture model (```n_components```);
     2. Comparing models with fit indices: AIC and BIC.
-4. [Parameters, Bootstrapping and CI](https://colab.research.google.com/drive/14Ir08HXQ3svydbVV4jlvi1HjGnfc4fc0?usp=sharing) :
+4. [Parameters, Bootstrapping and CI](https://colab.research.google.com/drive/14Ir08HXQ3svydbVV4jlvi1HjGnfc4fc0?usp=sharing):
    a tutorial discussing how to:
    1. Access StepMix parameters;
    2. Bootstrap StepMix estimators;
    2. Quickly plot confidence intervals.
 
-# Quickstart
-A simple example for 3-step estimation on simulated data :
-
-```python
-from stepmix.datasets import data_bakk_response
-from stepmix.stepmix import StepMix
-
-# Soft 3-step 
-X, Y, _ = data_bakk_response(n_samples=1000, sep_level=.9, random_state=42)
-model = StepMix(n_components=3, n_steps=3, measurement='bernoulli', structural='gaussian_unit', assignment='soft',
-            random_state=42)
-model.fit(X, Y)
-print(model.score(X, Y))  # Average log-likelihood
-
-# Equivalently, each step can be performed individually. See the code of the fit method for details.
-model = StepMix(n_components=3, measurement='bernoulli', structural='gaussian_unit', random_state=42)
-model.em(X)  # Step 1
-probs = model.predict_proba(X)  # Step 2
-model.m_step_structural(probs, Y)  # Step 3
-print(model.score(X, Y))
-```
-1-step and 2-step estimation are simply a matter of changing of the `n_steps` argument. Additionally, some bias correction
-methods are available for 3-step estimation.
-
-# References
-- Bolck, A., Croon, M., and Hagenaars, J. Estimating latent structure models with categorical variables: One-step
-versus three-step estimators. Political analysis, 12(1): 3–27, 2004.
-
-- Vermunt, J. K. Latent class modeling with covariates: Two improved three-step approaches. Political analysis,
-18 (4):450–469, 2010.
-
-- Bakk, Z., Tekle, F. B., and Vermunt, J. K. Estimating the association between latent class membership and external
-variables using bias-adjusted three-step approaches. Sociological Methodology, 43(1):272–311, 2013.
-
-- Bakk, Z. and Kuha, J. Two-step estimation of models between latent classes and external variables. Psychometrika,
-83(4):871–892, 2018
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,60 +1,66 @@
 StepMix ============================== [PyPI_version] [![Build](https://
 github.com/Labo-Lacourse/stepmix/actions/workflows/pytest.yaml/badge.svg)]
 (https://github.com/Labo-Lacourse/stepmix/actions/workflows/pytest.yaml) [!
 [Documentation Status](https://readthedocs.org/projects/stepmix/badge/
 ?version=latest)](https://stepmix.readthedocs.io/en/latest/index.html) [Code
 style:_black] [![Downloads](https://static.pepy.tech/badge/stepmix)](https://
 pepy.tech/project/stepmix) [![Downloads](https://static.pepy.tech/badge/
-stepmix/month)](https://pepy.tech/project/stepmix) *For StepMixR, please refer
-to this_repository.* A Python package following the scikit-learn API for model-
-based clustering and generalized mixture modeling (latent class/profile
-analysis) of continuous and categorical data. StepMix handles missing values
-through Full Information Maximum Likelihood (FIML) and provides multiple
-stepwise Expectation-Maximization (EM) estimation methods based on
-pseudolikelihood theory. Additional features include support for covariates and
-distal outcomes, various simulation utilities, and non-parametric
-bootstrapping, which allows inference in semi-supervised and unsupervised
-settings. # Install You can install StepMix with pip, preferably in a virtual
-environment : ``` pip install stepmix ``` # Tutorials Detailed tutorials are
-available in notebooks : 1. [Generalized Mixture Models with StepMix](https://
-colab.research.google.com/drive/1KAxcvxjL_vB2lAG9e47we7hrf_2fR1eK?usp=sharing)
-: an in-depth look at how latent class models can be defined with StepMix. The
-tutorial uses the Iris Dataset as an example and covers : 1. Continuous LCA
-models (latent profile analysis/gaussian mixture model); 2. Binary LCA models;
-3. Categorical LCA models; 3. Mixed variables mixture models (continuous and
-categorical data); 5. Missing Values through Full-Information Maximum
-Likelihood. 2. [Stepwise Estimation with StepMix](https://
-colab.research.google.com/drive/1T_UObkN5Y-iFTKiun0zOkKk7LjtMeV25?usp=sharing)
-: a tutorial demonstrating how to define measurement and structural models. The
-tutorial discusses: 1. LCA models with distal outcomes; 2. LCA models with
-covariates; 3. 1-step, 2-step and 3-step estimation; 4. Corrections (BCH or ML)
-and other options for 3-step estimation. 3. [Model Selection](https://
-colab.research.google.com/drive/1iyFTD-D2wn88_vd-qxXkovIuWHRtU7V8?usp=sharing)
-: a short tutorial discussing: 1. Selecting the number of components in a
-mixture model (```n_components```); 2. Comparing models with fit indices: AIC
-and BIC. 4. [Parameters, Bootstrapping and CI](https://
-colab.research.google.com/drive/14Ir08HXQ3svydbVV4jlvi1HjGnfc4fc0?usp=sharing)
-: a tutorial discussing how to: 1. Access StepMix parameters; 2. Bootstrap
-StepMix estimators; 2. Quickly plot confidence intervals. # Quickstart A simple
-example for 3-step estimation on simulated data : ```python from
-stepmix.datasets import data_bakk_response from stepmix.stepmix import StepMix
-# Soft 3-step X, Y, _ = data_bakk_response(n_samples=1000, sep_level=.9,
-random_state=42) model = StepMix(n_components=3, n_steps=3,
-measurement='bernoulli', structural='gaussian_unit', assignment='soft',
-random_state=42) model.fit(X, Y) print(model.score(X, Y)) # Average log-
-likelihood # Equivalently, each step can be performed individually. See the
-code of the fit method for details. model = StepMix(n_components=3,
-measurement='bernoulli', structural='gaussian_unit', random_state=42) model.em
-(X) # Step 1 probs = model.predict_proba(X) # Step 2 model.m_step_structural
-(probs, Y) # Step 3 print(model.score(X, Y)) ``` 1-step and 2-step estimation
-are simply a matter of changing of the `n_steps` argument. Additionally, some
-bias correction methods are available for 3-step estimation. # References -
-Bolck, A., Croon, M., and Hagenaars, J. Estimating latent structure models with
-categorical variables: One-step versus three-step estimators. Political
-analysis, 12(1): 3â27, 2004. - Vermunt, J. K. Latent class modeling with
-covariates: Two improved three-step approaches. Political analysis, 18 (4):
-450â469, 2010. - Bakk, Z., Tekle, F. B., and Vermunt, J. K. Estimating the
-association between latent class membership and external variables using bias-
-adjusted three-step approaches. Sociological Methodology, 43(1):272â311,
-2013. - Bakk, Z. and Kuha, J. Two-step estimation of models between latent
-classes and external variables. Psychometrika, 83(4):871â892, 2018
+stepmix/month)](https://pepy.tech/project/stepmix) [![arXiv](https://
+img.shields.io/badge/arXiv-2304.03853-b31b1b.svg)](https://arxiv.org/abs/
+2304.03853) *For StepMixR, please refer to this_repository.* A Python package
+following the scikit-learn API for model-based clustering and generalized
+mixture modeling (latent class/profile analysis) of continuous and categorical
+data. StepMix handles missing values through Full Information Maximum
+Likelihood (FIML) and provides multiple stepwise Expectation-Maximization (EM)
+estimation methods based on pseudolikelihood theory. Additional features
+include support for covariates and distal outcomes, various simulation
+utilities, and non-parametric bootstrapping, which allows inference in semi-
+supervised and unsupervised settings. # Reference If you find StepMix useful,
+please consider citing our [arXiv preprint](https://arxiv.org/abs/2304.03853):
+``` @article{morin2023stepmix, title={StepMix: A Python Package for Pseudo-
+Likelihood Estimation of Generalized Mixture Models with External Variables},
+author={Morin, Sacha and Legault, Robin and Bakk, Zsuzsa and Gigu{\`e}re,
+Charles-{\'E}douard and de la Sablonni{\`e}re, Roxane and Lacourse, {\'E}ric},
+journal={arXiv preprint arXiv:2304.03853}, year={2023} } ``` # Install You can
+install StepMix with pip, preferably in a virtual environment: ``` pip install
+stepmix ``` # Quickstart A simple StepMix mixture using the continuous
+variables of the Iris Dataset: ```python import pandas as pd from
+sklearn.datasets import load_iris from sklearn.metrics import rand_score from
+stepmix.stepmix import StepMix # Load dataset in a Dataframe data_continuous,
+target = load_iris(return_X_y=True, as_frame=True) # Continuous StepMix Model
+with 3 latent classes model = StepMix(n_components=3, measurement="continuous",
+verbose=0, random_state=123) # Fit model and predict clusters model.fit
+(data_continuous) pred_continuous = model.predict(data_continuous) # A Rand
+score close to 1 indicates good alignment between clusters and flower types
+print(rand_score(pred_continuous, target)) ``` StepMix also provides support
+for categorical mixtures: ```python # Create categorical data based on the Iris
+Dataset quantiles data_categorical = data_continuous.copy() for col in
+data_categorical: data_categorical[col] = pd.qcut(data_continuous[col],
+q=3).cat.codes # Categorical StepMix Model with 3 latent classes model =
+StepMix(n_components=3, measurement="categorical", verbose=0, random_state=123)
+# Fit model and predict clusters model.fit(data_categorical) pred_categorical =
+model.predict(data_categorical) # A Rand score close to 1 indicates good
+alignment between clusters and flower types print(rand_score(pred_categorical,
+target)) ``` Please refer to the StepMix tutorials to learn how to handle
+missing values and combine continuous and categorical data in the same model. #
+Tutorials Detailed tutorials are available in notebooks: 1. [Generalized
+Mixture Models with StepMix](https://colab.research.google.com/drive/
+1KAxcvxjL_vB2lAG9e47we7hrf_2fR1eK?usp=sharing): an in-depth look at how latent
+class models can be defined with StepMix. The tutorial uses the Iris Dataset as
+an example and covers: 1. Continuous LCA models (latent profile analysis/
+gaussian mixture model); 2. Binary LCA models; 3. Categorical LCA models; 3.
+Mixed variables mixture models (continuous and categorical data); 5. Missing
+Values through Full-Information Maximum Likelihood. 2. [Stepwise Estimation
+with StepMix](https://colab.research.google.com/drive/1T_UObkN5Y-
+iFTKiun0zOkKk7LjtMeV25?usp=sharing): a tutorial demonstrating how to define
+measurement and structural models. The tutorial discusses: 1. LCA models with
+distal outcomes; 2. LCA models with covariates; 3. 1-step, 2-step and 3-step
+estimation; 4. Corrections (BCH or ML) and other options for 3-step estimation.
+3. [Model Selection](https://colab.research.google.com/drive/1iyFTD-D2wn88_vd-
+qxXkovIuWHRtU7V8?usp=sharing): a short tutorial discussing: 1. Selecting the
+number of components in a mixture model (```n_components```); 2. Comparing
+models with fit indices: AIC and BIC. 4. [Parameters, Bootstrapping and CI]
+(https://colab.research.google.com/drive/
+14Ir08HXQ3svydbVV4jlvi1HjGnfc4fc0?usp=sharing): a tutorial discussing how to:
+1. Access StepMix parameters; 2. Bootstrap StepMix estimators; 2. Quickly plot
+confidence intervals.
```

### Comparing `stepmix-1.0.0/docs/Makefile` & `stepmix-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/docs/make.bat` & `stepmix-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/docs/source/api.rst` & `stepmix-1.0.1/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/docs/source/conf.py` & `stepmix-1.0.1/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 sys.path.insert(0, os.path.abspath("../.."))
 
 project = "StepMix"
 copyright = "2022, Labo-Lacourse"
 author = "Sacha Morin, Robin Legault"
 
 release = "0.0"
-version = "1.0.0"
+version = "1.0.1"
 
 
 # -- General configuration
 
 extensions = [
     "sphinx.ext.napoleon",
     # 'numpydoc',
```

### Comparing `stepmix-1.0.0/docs/source/index.rst` & `stepmix-1.0.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/docs/source/tutorials.rst` & `stepmix-1.0.1/docs/source/tutorials.rst`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/pyproject.toml` & `stepmix-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "flit", "pytest", "sphinx", "sphinx-rtd-theme"]
 
 [project.urls]
 Homepage = "https://stepmix.readthedocs.io/en/latest/"
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.0.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `stepmix-1.0.0/scripts/README.md` & `stepmix-1.0.1/scripts/README.md`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/scripts/run_bakk_simulation.py` & `stepmix-1.0.1/scripts/run_bakk_simulation.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/scripts/run_bakk_simulation_complete.py` & `stepmix-1.0.1/scripts/run_bakk_simulation_complete.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/stepmix/bootstrap.py` & `stepmix-1.0.1/stepmix/bootstrap.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/stepmix/corrections.py` & `stepmix-1.0.1/stepmix/corrections.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/stepmix/datasets.py` & `stepmix-1.0.1/stepmix/datasets.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/stepmix/emission/build_emission.py` & `stepmix-1.0.1/stepmix/emission/build_emission.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/stepmix/emission/categorical.py` & `stepmix-1.0.1/stepmix/emission/categorical.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/stepmix/emission/covariate.py` & `stepmix-1.0.1/stepmix/emission/covariate.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/stepmix/emission/emission.py` & `stepmix-1.0.1/stepmix/emission/emission.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/stepmix/emission/gaussian.py` & `stepmix-1.0.1/stepmix/emission/gaussian.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/stepmix/emission/nested.py` & `stepmix-1.0.1/stepmix/emission/nested.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/stepmix/stepmix.py` & `stepmix-1.0.1/stepmix/stepmix.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/stepmix/utils.py` & `stepmix-1.0.1/stepmix/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -452,14 +452,16 @@
     """Multiple categorical one-hot encoding.
 
     Takes an n_samples x n_features array of integer-encoded categorical features and returns an
     n_samples x (n_features x max_n_outcomes) array where max_n_outcomes is the number of outcomes in the
     categorical feature with the most categories. Categories are one-hot encoded and categories with
     fewer than max_n_outcomes simply have unused extra columns.
 
+    Handles missing values.
+
     Examples
     --------
     .. code-block:: python
         arr = np.array(
             [
                 [0, 3],
                 [1, 0],
@@ -494,21 +496,27 @@
 
     """
     n_samples = array.shape[0]
     n_features = array.shape[1]
 
     # Get maximal number of outcomes
     if max_n_outcomes is None:
-        max_n_outcomes = int(array.max() + 1)
+        max_n_outcomes = int(np.nanmax(array) + 1)
 
     # Create one-hot encoding
     one_hot = np.zeros((n_samples, array.shape[1] * max_n_outcomes))
 
     for c in range(n_features):
-        one_hot[np.arange(n_samples), array[:, c].astype(int) + c * max_n_outcomes] = 1
+        integer_codes = array[:, c]
+        not_observed = np.isnan(integer_codes)
+        integer_codes = np.nan_to_num(integer_codes, nan=0).astype(int)
+        one_hot[np.arange(n_samples), integer_codes + c * max_n_outcomes] = 1.0
+
+        # Now reapply NaNs
+        one_hot[not_observed, c * max_n_outcomes : (c + 1) * max_n_outcomes] = np.nan
 
     return one_hot, max_n_outcomes
 
 
 def get_mixed_descriptor(dataframe, **kwargs):
     """Simpler API to build the mixed model descriptor from a dataframe.
```

### Comparing `stepmix-1.0.0/test/conftest.py` & `stepmix-1.0.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/test/test_benchmarks.py` & `stepmix-1.0.1/test/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/test/test_bootstrap.py` & `stepmix-1.0.1/test/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/test/test_emission.py` & `stepmix-1.0.1/test/test_emission.py`

 * *Files 10% similar despite different names*

```diff
@@ -216,14 +216,40 @@
 
     onehot, max_n_outcomes = max_one_hot(a)
 
     assert max_n_outcomes == 4
     assert np.all(onehot == target)
 
 
+def test_max_one_hot_nan(data, kwargs):
+    """Test the max_one_hot method in utils with NaNs"""
+    a = np.array(
+        [
+            [0, 3],
+            [1, np.nan],
+            [np.nan, 1],
+            [2, 2],
+        ]
+    )
+
+    target = np.array(
+        [
+            [1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0],
+            [0.0, 1.0, 0.0, 0.0, np.nan, np.nan, np.nan, np.nan],
+            [np.nan, np.nan, np.nan, np.nan, 0.0, 1.0, 0.0, 0.0],
+            [0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 1.0, 0.0],
+        ]
+    )
+
+    onehot, max_n_outcomes = max_one_hot(a)
+
+    assert max_n_outcomes == 4
+    assert np.allclose(onehot, target, equal_nan=True)
+
+
 def test_categorical_encoding(kwargs):
     # Ignore base measurement and structural for this step
     kwargs.pop("measurement")
     kwargs.pop("structural")
 
     # Declare data
     data_int = np.array(
```

### Comparing `stepmix-1.0.0/test/test_fiml.py` & `stepmix-1.0.1/test/test_fiml.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/test/test_inputs.py` & `stepmix-1.0.1/test/test_inputs.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 import pandas as pd
 import numpy as np
 
 from stepmix.stepmix import StepMix
+from stepmix.emission.build_emission import EMISSION_DICT
 
 
 def test_dataframe(data, kwargs):
     X, Y = data
     X_df, Y_df = pd.DataFrame(X), pd.DataFrame(Y)
 
     # Test on numpy arrays
@@ -18,24 +19,46 @@
     model_2 = StepMix(n_steps=1, **kwargs)
     model_2.fit(X_df, Y_df)
     ll_2 = model_1.score(X_df, Y_df)  # Average log-likelihood
 
     assert ll_1 == ll_2
 
 
-def test_nan(data, kwargs):
+@pytest.mark.filterwarnings(
+    "ignore::RuntimeWarning"
+)  # Ignore most numerical errors since we do not run the emission models on appropriate data
+@pytest.mark.filterwarnings(
+    "ignore::sklearn.exceptions.ConvergenceWarning"
+)  # Ignore convergence warnings for same reason
+@pytest.mark.parametrize("model", EMISSION_DICT.keys())
+def test_nan(data, kwargs, model):
     X, Y = data
+    kwargs["measurement"] = model
+    kwargs["structural"] = model
 
     # Test on numpy arrays
     model_1 = StepMix(n_steps=1, **kwargs)
 
+    supports_nan = model.endswith("_nan")
+
     # Make sure vanilla models raise an Error if a missing value is found in the input
     X = X.astype(float)
     X_nan = X.copy()
     X_nan[0, 0] = np.nan
-    with pytest.raises(ValueError) as e_info:
+
+    if supports_nan:
+        # Should fit without error
         model_1.fit(X_nan, Y)
+    else:
+        # Should raise error
+        with pytest.raises(ValueError) as e_info:
+            model_1.fit(X_nan, Y)
 
     Y_nan = Y.copy()
     Y_nan[0, 0] = np.nan
-    with pytest.raises(ValueError) as e_info:
-        model_1.fit(X, Y_nan)
+    if supports_nan:
+        # Should fit without error
+        model_1.fit(X_nan, Y)
+    else:
+        # Should raise error
+        with pytest.raises(ValueError) as e_info:
+            model_1.fit(X, Y_nan)
```

### Comparing `stepmix-1.0.0/test/test_random_state.py` & `stepmix-1.0.1/test/test_random_state.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/test/test_sklearn.py` & `stepmix-1.0.1/test/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/test/test_steps.py` & `stepmix-1.0.1/test/test_steps.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.0/PKG-INFO` & `stepmix-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepmix
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for stepwise estimation of latent class models with measurement and structural components. The package can also be used to fit mixture models with various observed random variables.
 Keywords: clustering,mixtures,lca,em,latent-class-analysis,expectation–maximization
 Author-email: Sacha Morin <sacha.morin@mila.quebec>, Robin Legault <robin.legault@umontreal.ca>, Charles-Édouard Giguère <ce.giguere@gmail.com>, Éric Lacourse <eric.lacourse@umontreal.ca>, Roxane de la Sablonnière <roxane.de.la.sablonniere@umontreal.ca>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -27,84 +27,102 @@
 ==============================
 <a href="https://pypi.org/project/stepmix/"><img src="https://badge.fury.io/py/stepmix.svg" alt="PyPI version"></a>
 [![Build](https://github.com/Labo-Lacourse/stepmix/actions/workflows/pytest.yaml/badge.svg)](https://github.com/Labo-Lacourse/stepmix/actions/workflows/pytest.yaml)
 [![Documentation Status](https://readthedocs.org/projects/stepmix/badge/?version=latest)](https://stepmix.readthedocs.io/en/latest/index.html)
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 [![Downloads](https://static.pepy.tech/badge/stepmix)](https://pepy.tech/project/stepmix)
 [![Downloads](https://static.pepy.tech/badge/stepmix/month)](https://pepy.tech/project/stepmix)
+[![arXiv](https://img.shields.io/badge/arXiv-2304.03853-b31b1b.svg)](https://arxiv.org/abs/2304.03853)
 
 *For StepMixR, please refer to <a href="https://github.com/Labo-Lacourse/stepmixr">this repository.</a>*
 
 A Python package following the scikit-learn API for model-based clustering and generalized mixture modeling (latent class/profile analysis) of continuous and categorical data. 
 StepMix handles missing values through Full Information Maximum Likelihood (FIML) and provides multiple stepwise Expectation-Maximization (EM) estimation methods based on pseudolikelihood theory. 
 Additional features include support for covariates and distal outcomes, various simulation utilities, and non-parametric bootstrapping, which allows inference
 in semi-supervised and unsupervised settings.
 
+# Reference
+If you find StepMix useful, please consider citing our [arXiv preprint](https://arxiv.org/abs/2304.03853):
+```
+@article{morin2023stepmix,
+  title={StepMix: A Python Package for Pseudo-Likelihood Estimation of Generalized Mixture Models with External Variables},
+  author={Morin, Sacha and Legault, Robin and Bakk, Zsuzsa and Gigu{\`e}re, Charles-{\'E}douard and de la Sablonni{\`e}re, Roxane and Lacourse, {\'E}ric},
+  journal={arXiv preprint arXiv:2304.03853},
+  year={2023}
+}
+```
+
 
 # Install
-You can install StepMix with pip, preferably in a virtual environment : 
+You can install StepMix with pip, preferably in a virtual environment: 
 ```
 pip install stepmix
 ``` 
+# Quickstart
+A simple StepMix mixture using the continuous variables of the Iris Dataset:
+
+```python
+import pandas as pd
+from sklearn.datasets import load_iris
+from sklearn.metrics import rand_score
+
+from stepmix.stepmix import StepMix
+
+# Load dataset in a Dataframe
+data_continuous, target = load_iris(return_X_y=True, as_frame=True)
+
+# Continuous StepMix Model with 3 latent classes
+model = StepMix(n_components=3, measurement="continuous", verbose=0, random_state=123)
+
+# Fit model and predict clusters
+model.fit(data_continuous)
+pred_continuous = model.predict(data_continuous)
+
+# A Rand score close to 1 indicates good alignment between clusters and flower types
+print(rand_score(pred_continuous, target))
+```
+StepMix also provides support for categorical mixtures:
+
+```python
+# Create categorical data based on the Iris Dataset quantiles
+data_categorical = data_continuous.copy()
+for col in data_categorical:
+   data_categorical[col] = pd.qcut(data_continuous[col], q=3).cat.codes
+
+# Categorical StepMix Model with 3 latent classes
+model = StepMix(n_components=3, measurement="categorical", verbose=0, random_state=123)
+
+# Fit model and predict clusters
+model.fit(data_categorical)
+pred_categorical = model.predict(data_categorical)
+
+# A Rand score close to 1 indicates good alignment between clusters and flower types
+print(rand_score(pred_categorical, target))
+```
+Please refer to the StepMix tutorials to learn how to handle missing values and combine continuous and categorical data in the same model.
 # Tutorials
-Detailed tutorials are available in notebooks : 
-1. [Generalized Mixture Models with StepMix](https://colab.research.google.com/drive/1KAxcvxjL_vB2lAG9e47we7hrf_2fR1eK?usp=sharing) : 
+Detailed tutorials are available in notebooks: 
+1. [Generalized Mixture Models with StepMix](https://colab.research.google.com/drive/1KAxcvxjL_vB2lAG9e47we7hrf_2fR1eK?usp=sharing): 
 an in-depth look at how latent class models can be defined with StepMix. The tutorial uses the Iris Dataset as an example
-and covers :
+and covers:
    1. Continuous LCA models (latent profile analysis/gaussian mixture model);
    2. Binary LCA models;
    3. Categorical LCA models;
    3. Mixed variables mixture models (continuous and categorical data);
    5. Missing Values through Full-Information Maximum Likelihood.
-2. [Stepwise Estimation with StepMix](https://colab.research.google.com/drive/1T_UObkN5Y-iFTKiun0zOkKk7LjtMeV25?usp=sharing) :
+2. [Stepwise Estimation with StepMix](https://colab.research.google.com/drive/1T_UObkN5Y-iFTKiun0zOkKk7LjtMeV25?usp=sharing):
     a tutorial demonstrating how to define measurement and structural models. The tutorial discusses:
    1. LCA models with distal outcomes;
    2. LCA models with covariates; 
    3. 1-step, 2-step and 3-step estimation;
    4. Corrections (BCH or ML) and other options for 3-step estimation.
-3. [Model Selection](https://colab.research.google.com/drive/1iyFTD-D2wn88_vd-qxXkovIuWHRtU7V8?usp=sharing) :
+3. [Model Selection](https://colab.research.google.com/drive/1iyFTD-D2wn88_vd-qxXkovIuWHRtU7V8?usp=sharing):
    a short tutorial discussing:
     1. Selecting the number of components in a mixture model (```n_components```);
     2. Comparing models with fit indices: AIC and BIC.
-4. [Parameters, Bootstrapping and CI](https://colab.research.google.com/drive/14Ir08HXQ3svydbVV4jlvi1HjGnfc4fc0?usp=sharing) :
+4. [Parameters, Bootstrapping and CI](https://colab.research.google.com/drive/14Ir08HXQ3svydbVV4jlvi1HjGnfc4fc0?usp=sharing):
    a tutorial discussing how to:
    1. Access StepMix parameters;
    2. Bootstrap StepMix estimators;
    2. Quickly plot confidence intervals.
 
-# Quickstart
-A simple example for 3-step estimation on simulated data :
-
-```python
-from stepmix.datasets import data_bakk_response
-from stepmix.stepmix import StepMix
-
-# Soft 3-step 
-X, Y, _ = data_bakk_response(n_samples=1000, sep_level=.9, random_state=42)
-model = StepMix(n_components=3, n_steps=3, measurement='bernoulli', structural='gaussian_unit', assignment='soft',
-            random_state=42)
-model.fit(X, Y)
-print(model.score(X, Y))  # Average log-likelihood
-
-# Equivalently, each step can be performed individually. See the code of the fit method for details.
-model = StepMix(n_components=3, measurement='bernoulli', structural='gaussian_unit', random_state=42)
-model.em(X)  # Step 1
-probs = model.predict_proba(X)  # Step 2
-model.m_step_structural(probs, Y)  # Step 3
-print(model.score(X, Y))
-```
-1-step and 2-step estimation are simply a matter of changing of the `n_steps` argument. Additionally, some bias correction
-methods are available for 3-step estimation.
-
-# References
-- Bolck, A., Croon, M., and Hagenaars, J. Estimating latent structure models with categorical variables: One-step
-versus three-step estimators. Political analysis, 12(1): 3–27, 2004.
-
-- Vermunt, J. K. Latent class modeling with covariates: Two improved three-step approaches. Political analysis,
-18 (4):450–469, 2010.
-
-- Bakk, Z., Tekle, F. B., and Vermunt, J. K. Estimating the association between latent class membership and external
-variables using bias-adjusted three-step approaches. Sociological Methodology, 43(1):272–311, 2013.
-
-- Bakk, Z. and Kuha, J. Two-step estimation of models between latent classes and external variables. Psychometrika,
-83(4):871–892, 2018
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stepmix Version: 1.0.0 Summary: A Python package
+Metadata-Version: 2.1 Name: stepmix Version: 1.0.1 Summary: A Python package
 for stepwise estimation of latent class models with measurement and structural
 components. The package can also be used to fit mixture models with various
 observed random variables. Keywords: clustering,mixtures,lca,em,latent-class-
 analysis,expectationâmaximization Author-email: Sacha Morin
 morin@mila.quebec>, Robin Legault
 legault@umontreal.ca>, Charles-Ãdouard GiguÃ¨re
 giguere@gmail.com>, Ãric Lacourse
@@ -19,60 +19,66 @@
 Extra: dev StepMix ============================== [PyPI_version] [![Build]
 (https://github.com/Labo-Lacourse/stepmix/actions/workflows/pytest.yaml/
 badge.svg)](https://github.com/Labo-Lacourse/stepmix/actions/workflows/
 pytest.yaml) [![Documentation Status](https://readthedocs.org/projects/stepmix/
 badge/?version=latest)](https://stepmix.readthedocs.io/en/latest/index.html)
 [Code_style:_black] [![Downloads](https://static.pepy.tech/badge/stepmix)]
 (https://pepy.tech/project/stepmix) [![Downloads](https://static.pepy.tech/
-badge/stepmix/month)](https://pepy.tech/project/stepmix) *For StepMixR, please
-refer to this_repository.* A Python package following the scikit-learn API for
-model-based clustering and generalized mixture modeling (latent class/profile
-analysis) of continuous and categorical data. StepMix handles missing values
-through Full Information Maximum Likelihood (FIML) and provides multiple
-stepwise Expectation-Maximization (EM) estimation methods based on
-pseudolikelihood theory. Additional features include support for covariates and
-distal outcomes, various simulation utilities, and non-parametric
-bootstrapping, which allows inference in semi-supervised and unsupervised
-settings. # Install You can install StepMix with pip, preferably in a virtual
-environment : ``` pip install stepmix ``` # Tutorials Detailed tutorials are
-available in notebooks : 1. [Generalized Mixture Models with StepMix](https://
-colab.research.google.com/drive/1KAxcvxjL_vB2lAG9e47we7hrf_2fR1eK?usp=sharing)
-: an in-depth look at how latent class models can be defined with StepMix. The
-tutorial uses the Iris Dataset as an example and covers : 1. Continuous LCA
-models (latent profile analysis/gaussian mixture model); 2. Binary LCA models;
-3. Categorical LCA models; 3. Mixed variables mixture models (continuous and
-categorical data); 5. Missing Values through Full-Information Maximum
-Likelihood. 2. [Stepwise Estimation with StepMix](https://
-colab.research.google.com/drive/1T_UObkN5Y-iFTKiun0zOkKk7LjtMeV25?usp=sharing)
-: a tutorial demonstrating how to define measurement and structural models. The
-tutorial discusses: 1. LCA models with distal outcomes; 2. LCA models with
-covariates; 3. 1-step, 2-step and 3-step estimation; 4. Corrections (BCH or ML)
-and other options for 3-step estimation. 3. [Model Selection](https://
-colab.research.google.com/drive/1iyFTD-D2wn88_vd-qxXkovIuWHRtU7V8?usp=sharing)
-: a short tutorial discussing: 1. Selecting the number of components in a
-mixture model (```n_components```); 2. Comparing models with fit indices: AIC
-and BIC. 4. [Parameters, Bootstrapping and CI](https://
-colab.research.google.com/drive/14Ir08HXQ3svydbVV4jlvi1HjGnfc4fc0?usp=sharing)
-: a tutorial discussing how to: 1. Access StepMix parameters; 2. Bootstrap
-StepMix estimators; 2. Quickly plot confidence intervals. # Quickstart A simple
-example for 3-step estimation on simulated data : ```python from
-stepmix.datasets import data_bakk_response from stepmix.stepmix import StepMix
-# Soft 3-step X, Y, _ = data_bakk_response(n_samples=1000, sep_level=.9,
-random_state=42) model = StepMix(n_components=3, n_steps=3,
-measurement='bernoulli', structural='gaussian_unit', assignment='soft',
-random_state=42) model.fit(X, Y) print(model.score(X, Y)) # Average log-
-likelihood # Equivalently, each step can be performed individually. See the
-code of the fit method for details. model = StepMix(n_components=3,
-measurement='bernoulli', structural='gaussian_unit', random_state=42) model.em
-(X) # Step 1 probs = model.predict_proba(X) # Step 2 model.m_step_structural
-(probs, Y) # Step 3 print(model.score(X, Y)) ``` 1-step and 2-step estimation
-are simply a matter of changing of the `n_steps` argument. Additionally, some
-bias correction methods are available for 3-step estimation. # References -
-Bolck, A., Croon, M., and Hagenaars, J. Estimating latent structure models with
-categorical variables: One-step versus three-step estimators. Political
-analysis, 12(1): 3â27, 2004. - Vermunt, J. K. Latent class modeling with
-covariates: Two improved three-step approaches. Political analysis, 18 (4):
-450â469, 2010. - Bakk, Z., Tekle, F. B., and Vermunt, J. K. Estimating the
-association between latent class membership and external variables using bias-
-adjusted three-step approaches. Sociological Methodology, 43(1):272â311,
-2013. - Bakk, Z. and Kuha, J. Two-step estimation of models between latent
-classes and external variables. Psychometrika, 83(4):871â892, 2018
+badge/stepmix/month)](https://pepy.tech/project/stepmix) [![arXiv](https://
+img.shields.io/badge/arXiv-2304.03853-b31b1b.svg)](https://arxiv.org/abs/
+2304.03853) *For StepMixR, please refer to this_repository.* A Python package
+following the scikit-learn API for model-based clustering and generalized
+mixture modeling (latent class/profile analysis) of continuous and categorical
+data. StepMix handles missing values through Full Information Maximum
+Likelihood (FIML) and provides multiple stepwise Expectation-Maximization (EM)
+estimation methods based on pseudolikelihood theory. Additional features
+include support for covariates and distal outcomes, various simulation
+utilities, and non-parametric bootstrapping, which allows inference in semi-
+supervised and unsupervised settings. # Reference If you find StepMix useful,
+please consider citing our [arXiv preprint](https://arxiv.org/abs/2304.03853):
+``` @article{morin2023stepmix, title={StepMix: A Python Package for Pseudo-
+Likelihood Estimation of Generalized Mixture Models with External Variables},
+author={Morin, Sacha and Legault, Robin and Bakk, Zsuzsa and Gigu{\`e}re,
+Charles-{\'E}douard and de la Sablonni{\`e}re, Roxane and Lacourse, {\'E}ric},
+journal={arXiv preprint arXiv:2304.03853}, year={2023} } ``` # Install You can
+install StepMix with pip, preferably in a virtual environment: ``` pip install
+stepmix ``` # Quickstart A simple StepMix mixture using the continuous
+variables of the Iris Dataset: ```python import pandas as pd from
+sklearn.datasets import load_iris from sklearn.metrics import rand_score from
+stepmix.stepmix import StepMix # Load dataset in a Dataframe data_continuous,
+target = load_iris(return_X_y=True, as_frame=True) # Continuous StepMix Model
+with 3 latent classes model = StepMix(n_components=3, measurement="continuous",
+verbose=0, random_state=123) # Fit model and predict clusters model.fit
+(data_continuous) pred_continuous = model.predict(data_continuous) # A Rand
+score close to 1 indicates good alignment between clusters and flower types
+print(rand_score(pred_continuous, target)) ``` StepMix also provides support
+for categorical mixtures: ```python # Create categorical data based on the Iris
+Dataset quantiles data_categorical = data_continuous.copy() for col in
+data_categorical: data_categorical[col] = pd.qcut(data_continuous[col],
+q=3).cat.codes # Categorical StepMix Model with 3 latent classes model =
+StepMix(n_components=3, measurement="categorical", verbose=0, random_state=123)
+# Fit model and predict clusters model.fit(data_categorical) pred_categorical =
+model.predict(data_categorical) # A Rand score close to 1 indicates good
+alignment between clusters and flower types print(rand_score(pred_categorical,
+target)) ``` Please refer to the StepMix tutorials to learn how to handle
+missing values and combine continuous and categorical data in the same model. #
+Tutorials Detailed tutorials are available in notebooks: 1. [Generalized
+Mixture Models with StepMix](https://colab.research.google.com/drive/
+1KAxcvxjL_vB2lAG9e47we7hrf_2fR1eK?usp=sharing): an in-depth look at how latent
+class models can be defined with StepMix. The tutorial uses the Iris Dataset as
+an example and covers: 1. Continuous LCA models (latent profile analysis/
+gaussian mixture model); 2. Binary LCA models; 3. Categorical LCA models; 3.
+Mixed variables mixture models (continuous and categorical data); 5. Missing
+Values through Full-Information Maximum Likelihood. 2. [Stepwise Estimation
+with StepMix](https://colab.research.google.com/drive/1T_UObkN5Y-
+iFTKiun0zOkKk7LjtMeV25?usp=sharing): a tutorial demonstrating how to define
+measurement and structural models. The tutorial discusses: 1. LCA models with
+distal outcomes; 2. LCA models with covariates; 3. 1-step, 2-step and 3-step
+estimation; 4. Corrections (BCH or ML) and other options for 3-step estimation.
+3. [Model Selection](https://colab.research.google.com/drive/1iyFTD-D2wn88_vd-
+qxXkovIuWHRtU7V8?usp=sharing): a short tutorial discussing: 1. Selecting the
+number of components in a mixture model (```n_components```); 2. Comparing
+models with fit indices: AIC and BIC. 4. [Parameters, Bootstrapping and CI]
+(https://colab.research.google.com/drive/
+14Ir08HXQ3svydbVV4jlvi1HjGnfc4fc0?usp=sharing): a tutorial discussing how to:
+1. Access StepMix parameters; 2. Bootstrap StepMix estimators; 2. Quickly plot
+confidence intervals.
```

