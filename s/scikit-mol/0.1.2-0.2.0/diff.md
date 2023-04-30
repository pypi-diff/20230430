# Comparing `tmp/scikit_mol-0.1.2.tar.gz` & `tmp/scikit_mol-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit_mol-0.1.2.tar", last modified: Sat Mar  4 10:01:11 2023, max compression
+gzip compressed data, was "scikit_mol-0.2.0.tar", last modified: Sun Apr 30 08:56:11 2023, max compression
```

## Comparing `scikit_mol-0.1.2.tar` & `scikit_mol-0.2.0.tar`

### file list

```diff
@@ -1,73 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 10:01:11.858824 scikit_mol-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-03-04 10:01:11.858824 scikit_mol-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 10:01:11.850824 scikit_mol-0.1.2/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    16046 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/01_basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/01_basic_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)    24353 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/02_descriptor_transformer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/02_descriptor_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 10:01:11.850824 scikit_mol-0.1.2/notebooks/02_descriptor_transformer_files/
--rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/02_descriptor_transformer_files/02_descriptor_transformer_5_0.png
--rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/03_example_pipeline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/03_example_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    29763 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/04_standardizer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/04_standardizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 10:01:11.854824 scikit_mol-0.1.2/notebooks/04_standardizer_files/
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/04_standardizer_files/04_standardizer_3_0.png
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/04_standardizer_files/04_standardizer_3_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/05_smiles_sanitaztion.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/05_smiles_sanitaztion.py
--rw-r--r--   0 runner    (1001) docker     (123)    19128 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/06_hyperparameter_tuning.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/06_hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/07_parallel_transforms.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/07_parallel_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 10:01:11.854824 scikit_mol-0.1.2/notebooks/images/
--rw-r--r--   0 runner    (1001) docker     (123)    66320 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/images/AtomPairFingerprintTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    60999 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/images/AtomPairFingerprintTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)    64259 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/images/Desc2DTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    58977 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/images/Desc2DTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)    66054 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/images/MACCSTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    60534 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/images/MACCSTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)    65268 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/images/MorganTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    59856 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/images/MorganTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)    65110 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/images/RDKitFPTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    60176 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/images/RDKitFPTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)    64025 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/images/SECFingerprintTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    60783 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/images/SECFingerprintTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)    68278 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/images/TopologicalTorsionFingerprintTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    60915 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/images/TopologicalTorsionFingerprintTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/images/Transformer_Widget.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    52959 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/images/max_speedup_vs_throughput.png
--rw-r--r--   0 runner    (1001) docker     (123)    46854 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/images/max_speedup_vs_throughput.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/pair_notebook.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/run_notebooks.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       20 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/notebooks/sync_notebooks.sh
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 10:01:11.858824 scikit_mol-0.1.2/scikit_mol/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/scikit_mol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-04 10:01:11.000000 scikit_mol-0.1.2/scikit_mol/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/scikit_mol/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/scikit_mol/sanitizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/scikit_mol/standardizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19955 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/scikit_mol/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 10:01:11.858824 scikit_mol-0.1.2/scikit_mol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-03-04 10:01:11.000000 scikit_mol-0.1.2/scikit_mol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-03-04 10:01:11.000000 scikit_mol-0.1.2/scikit_mol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 10:01:11.000000 scikit_mol-0.1.2/scikit_mol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-04 10:01:11.000000 scikit_mol-0.1.2/scikit_mol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-04 10:01:11.000000 scikit_mol-0.1.2/scikit_mol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-03-04 10:01:11.858824 scikit_mol-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 10:01:11.858824 scikit_mol-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 10:01:11.858824 scikit_mol-0.1.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    18060 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/tests/data/SLC6A4_active_excapedb_subset.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/tests/test_desctransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/tests/test_fptransformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/tests/test_sanitizer.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/tests/test_scikit_mol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/tests/test_smilestomol.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-03-04 10:01:01.000000 scikit_mol-0.1.2/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:56:11.666782 scikit_mol-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-30 08:56:11.666782 scikit_mol-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:56:11.658783 scikit_mol-0.2.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    15972 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/01_basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/01_basic_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40949 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/02_descriptor_transformer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/02_descriptor_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:56:11.658783 scikit_mol-0.2.0/notebooks/02_descriptor_transformer_files/
+-rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/02_descriptor_transformer_files/02_descriptor_transformer_5_0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/03_example_pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/03_example_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30287 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/04_standardizer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/04_standardizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:56:11.658783 scikit_mol-0.2.0/notebooks/04_standardizer_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/04_standardizer_files/04_standardizer_3_0.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/04_standardizer_files/04_standardizer_3_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/05_smiles_sanitaztion.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/05_smiles_sanitaztion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19466 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/06_hyperparameter_tuning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/06_hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/07_parallel_transforms.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/07_parallel_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/08_external_library_skopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:56:11.662783 scikit_mol-0.2.0/notebooks/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    66320 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/AtomPairFingerprintTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60999 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/AtomPairFingerprintTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    64259 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/Desc2DTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (123)    58977 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/Desc2DTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    66054 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/MACCSTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60534 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/MACCSTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    65268 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/MorganTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (123)    59856 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/MorganTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    65110 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/RDKitFPTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60176 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/RDKitFPTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    64025 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/SECFingerprintTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60783 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/SECFingerprintTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    68278 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/TopologicalTorsionFingerprintTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60915 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/TopologicalTorsionFingerprintTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/Transformer_Widget.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    52959 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/max_speedup_vs_throughput.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46854 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/max_speedup_vs_throughput.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/pair_notebook.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/run_notebooks.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       20 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/sync_notebooks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:56:11.662783 scikit_mol-0.2.0/scikit_mol/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/scikit_mol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-30 08:56:11.000000 scikit_mol-0.2.0/scikit_mol/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/scikit_mol/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/scikit_mol/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21524 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/scikit_mol/fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/scikit_mol/standardizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/scikit_mol/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:56:11.662783 scikit_mol-0.2.0/scikit_mol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-30 08:56:11.000000 scikit_mol-0.2.0/scikit_mol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-30 08:56:11.000000 scikit_mol-0.2.0/scikit_mol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 08:56:11.000000 scikit_mol-0.2.0/scikit_mol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-30 08:56:11.000000 scikit_mol-0.2.0/scikit_mol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 08:56:11.000000 scikit_mol-0.2.0/scikit_mol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-30 08:56:11.666782 scikit_mol-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:56:11.666782 scikit_mol-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:56:11.666782 scikit_mol-0.2.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    18060 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/data/SLC6A4_active_excapedb_subset.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/test_desctransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/test_fptransformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/test_parameter_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/test_sanitizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/test_scikit_mol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/test_smilestomol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/test_transformers.py
```

### Comparing `scikit_mol-0.1.2/LICENSE` & `scikit_mol-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/PKG-INFO` & `scikit_mol-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit_mol
-Version: 0.1.2
+Version: 0.2.0
 Summary: scikit-learn classes for molecule transformation
 Home-page: https://github.com/EBjerrum/scikit-mol
 Download-URL: https://github.com/EBjerrum/scikit-mol
 Author: Esben Jannik Bjerrum
 Author-email: esben@cheminformania.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
@@ -96,7 +96,8 @@
 * Esben Jannik Bjerrum [@ebjerrum](https://github.com/ebjerrum), esben@cheminformania.com
 * Carmen Esposito [@cespos](https://github.com/cespos)
 * Son Ha, sonha@uni-mainz.de
 * Oh-hyeon Choung, ohhyeon.choung@gmail.com
 * Andreas Poehlmann, [@ap--](https://github.com/ap--)
 * Ya Chen, [@anya-chen](https://github.com/anya-chen)
 * Rafał Bachorz [@rafalbachorz](https://github.com/rafalbachorz)
+* Adrien Chaton [@adrienchaton](https://github.com/adrienchaton)
```

### Comparing `scikit_mol-0.1.2/README.md` & `scikit_mol-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -67,7 +67,8 @@
 * Esben Jannik Bjerrum [@ebjerrum](https://github.com/ebjerrum), esben@cheminformania.com
 * Carmen Esposito [@cespos](https://github.com/cespos)
 * Son Ha, sonha@uni-mainz.de
 * Oh-hyeon Choung, ohhyeon.choung@gmail.com
 * Andreas Poehlmann, [@ap--](https://github.com/ap--)
 * Ya Chen, [@anya-chen](https://github.com/anya-chen)
 * Rafał Bachorz [@rafalbachorz](https://github.com/rafalbachorz)
+* Adrien Chaton [@adrienchaton](https://github.com/adrienchaton)
```

### Comparing `scikit_mol-0.1.2/notebooks/01_basic_usage.ipynb` & `scikit_mol-0.2.0/notebooks/01_basic_usage.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9521479479949875%*

 * *Differences: {"'cells'": "{0: {'id': '8a3e313c'}, 1: {'id': '7bcbed23'}, 2: {'id': 'f8025236', 'metadata': "*

 * *            "{'execution': {'iopub.execute_input': '2023-03-19T08:54:22.197918Z', "*

 * *            "'iopub.status.busy': '2023-03-19T08:54:22.197263Z', 'iopub.status.idle': "*

 * *            "'2023-03-19T08:54:22.205876Z', 'shell.execute_reply': "*

 * *            "'2023-03-19T08:54:22.205379Z'}}}, 3: {'id': '58a33f4d', 'metadata': {'execution': "*

 * *            "{'iopub.execute_input': '2023-03-19T08:54:22.208372Z', 'iopub.sta […]*

```diff
@@ -1,55 +1,55 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "73523f92",
+            "id": "8a3e313c",
             "metadata": {},
             "source": [
                 "# Scikit-Mol\n",
                 "## scikit-learn compatible RDKit transformers\n",
                 "\n",
                 "Scikit-mol is a collection of scikit-learn compatible transformer classes that integrate into the scikit-learn framework and thus bridge between the molecular information in form of RDKit molecules or SMILES and the machine learning framework from scikit-learn\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a23e85c0",
+            "id": "7bcbed23",
             "metadata": {},
             "source": [
                 "The transformer classes are easy to load, configure and use to process molecular information into vectorized formats using fingerprinters or collections of descriptors. For demonstration purposes, let's load a MorganTransformer, that can convert a list of RDKit molecular objects into a numpy array of morgan fingerprints. First create some molecules from SMILES strings."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
-            "id": "5465b117",
+            "id": "f8025236",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:15.620059Z",
-                    "iopub.status.busy": "2022-12-09T17:05:15.619096Z",
-                    "iopub.status.idle": "2022-12-09T17:05:15.626395Z",
-                    "shell.execute_reply": "2022-12-09T17:05:15.627147Z"
+                    "iopub.execute_input": "2023-03-19T08:54:22.197918Z",
+                    "iopub.status.busy": "2023-03-19T08:54:22.197263Z",
+                    "iopub.status.idle": "2023-03-19T08:54:22.205876Z",
+                    "shell.execute_reply": "2023-03-19T08:54:22.205379Z"
                 }
             },
             "outputs": [],
             "source": [
                 "from IPython.core.display import HTML"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
-            "id": "146e0986",
+            "id": "58a33f4d",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:15.632656Z",
-                    "iopub.status.busy": "2022-12-09T17:05:15.631450Z",
-                    "iopub.status.idle": "2022-12-09T17:05:15.863922Z",
-                    "shell.execute_reply": "2022-12-09T17:05:15.863285Z"
+                    "iopub.execute_input": "2023-03-19T08:54:22.208372Z",
+                    "iopub.status.busy": "2023-03-19T08:54:22.208130Z",
+                    "iopub.status.idle": "2023-03-19T08:54:22.428376Z",
+                    "shell.execute_reply": "2023-03-19T08:54:22.427474Z"
                 }
             },
             "outputs": [],
             "source": [
                 "from rdkit import Chem\n",
                 "\n",
                 "smiles_strings = [\"C12C([C@@H](OC(C=3C=CC(=CC3)F)C=4C=CC(=CC4)F)CC(N1CCCCCC5=CC=CC=C5)CC2)C(=O)OC\", \n",
@@ -60,151 +60,152 @@
                 "\"FC(F)(F)C=1C(CN(C2CCNCC2)CC(CC)CC)=CC=CC1\"]\n",
                 "\n",
                 "mols = [Chem.MolFromSmiles(smiles) for smiles in smiles_strings]"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "6b0f57df",
+            "id": "0228c878",
             "metadata": {},
             "source": [
                 "Next we import the Morgan fingerprint transformer"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
-            "id": "69a1e742",
+            "id": "cdb821a1",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:15.874453Z",
-                    "iopub.status.busy": "2022-12-09T17:05:15.869155Z",
-                    "iopub.status.idle": "2022-12-09T17:05:16.515461Z",
-                    "shell.execute_reply": "2022-12-09T17:05:16.516116Z"
+                    "iopub.execute_input": "2023-03-19T08:54:22.431905Z",
+                    "iopub.status.busy": "2023-03-19T08:54:22.431641Z",
+                    "iopub.status.idle": "2023-03-19T08:54:22.962569Z",
+                    "shell.execute_reply": "2023-03-19T08:54:22.961792Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "MorganTransformer(radius=3)\n"
                     ]
                 }
             ],
             "source": [
-                "from scikit_mol.transformers import MorganTransformer\n",
+                "from scikit_mol.fingerprints import MorganFingerprintTransformer\n",
                 "\n",
-                "transformer = MorganTransformer(radius=3)\n",
+                "transformer = MorganFingerprintTransformer(radius=3)\n",
                 "print(transformer)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "4771be4e",
+            "id": "e8ebae67",
             "metadata": {},
             "source": [
                 "It actually renders as a cute little interactive block in the Jupyter notebook and lists the options that are not the default values. If we print it, it also gives the information on the settings. \n",
                 "\n",
                 "![An image of the interactive transformer widget](images/Transformer_Widget.jpg \"Transformer object rendering in Jupyter\")\n",
                 "\n",
                 "The graphical representation is probably nice when working with complex pipelines. However, the graphical representation doesn't work when previewing the notebook on GitHub and sometimes nbviewer.org, so for the rest of these scikit-mol notebook examples, we'll use the print() output."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
-            "id": "090d8236",
+            "id": "c3a24f4e",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:16.533536Z",
-                    "iopub.status.busy": "2022-12-09T17:05:16.532722Z",
-                    "iopub.status.idle": "2022-12-09T17:05:16.536962Z",
-                    "shell.execute_reply": "2022-12-09T17:05:16.537462Z"
+                    "iopub.execute_input": "2023-03-19T08:54:22.965768Z",
+                    "iopub.status.busy": "2023-03-19T08:54:22.965105Z",
+                    "iopub.status.idle": "2023-03-19T08:54:22.971941Z",
+                    "shell.execute_reply": "2023-03-19T08:54:22.971327Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style>#sk-container-id-1 {color: black;background-color: white;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 div.sk-toggleable {background-color: white;}#sk-container-id-1 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-1 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-1 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-1 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-1 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-1 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-1 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-1 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-1 div.sk-item {position: relative;z-index: 1;}#sk-container-id-1 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-1 div.sk-item::before, #sk-container-id-1 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-1 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-1 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-1 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-1 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-1 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-1 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-1 div.sk-label-container {text-align: center;}#sk-container-id-1 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-1 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-1\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>MorganTransformer(radius=3)</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-1\" type=\"checkbox\" checked><label for=\"sk-estimator-id-1\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">MorganTransformer</label><div class=\"sk-toggleable__content\"><pre>MorganTransformer(radius=3)</pre></div></div></div></div></div>"
                         ],
                         "text/plain": [
                             "MorganTransformer(radius=3)"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "transformer"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "bdacd1be",
+            "id": "c6e5de37",
             "metadata": {},
             "source": [
                 "If we want to get all the settings explicitly, we can use the .get_params() method."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
-            "id": "875bcb5c",
+            "id": "112afff2",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:16.545216Z",
-                    "iopub.status.busy": "2022-12-09T17:05:16.544442Z",
-                    "iopub.status.idle": "2022-12-09T17:05:16.548197Z",
-                    "shell.execute_reply": "2022-12-09T17:05:16.547530Z"
+                    "iopub.execute_input": "2023-03-19T08:54:22.974458Z",
+                    "iopub.status.busy": "2023-03-19T08:54:22.974238Z",
+                    "iopub.status.idle": "2023-03-19T08:54:22.978835Z",
+                    "shell.execute_reply": "2023-03-19T08:54:22.978252Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{'nBits': 2048,\n",
+                            " 'parallel': False,\n",
                             " 'radius': 3,\n",
                             " 'useBondTypes': True,\n",
                             " 'useChirality': False,\n",
                             " 'useCounts': False,\n",
                             " 'useFeatures': False}"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "parameters = transformer.get_params()\n",
                 "parameters"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c40b2e97",
+            "id": "45296da6",
             "metadata": {},
             "source": [
                 "The corresponding .set_params() method can be used to update the settings from options or from a dictionary (via ** unpackaging). The get_params and set_params methods are sometimes used by sklearn, as example hyperparameter search objects."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
-            "id": "7c483432",
+            "id": "4229d3d3",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:16.553806Z",
-                    "iopub.status.busy": "2022-12-09T17:05:16.552955Z",
-                    "iopub.status.idle": "2022-12-09T17:05:16.560010Z",
-                    "shell.execute_reply": "2022-12-09T17:05:16.559494Z"
+                    "iopub.execute_input": "2023-03-19T08:54:22.981502Z",
+                    "iopub.status.busy": "2023-03-19T08:54:22.981247Z",
+                    "iopub.status.idle": "2023-03-19T08:54:22.985186Z",
+                    "shell.execute_reply": "2023-03-19T08:54:22.984526Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -217,141 +218,141 @@
                 "parameters[\"nBits\"] = 256\n",
                 "transformer.set_params(**parameters)\n",
                 "print(transformer)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "f415d9d3",
+            "id": "1d38c224",
             "metadata": {},
             "source": [
                 "Transformation is easy, simply use the .transform() method. For sklearn compatibility the scikit-learn transformers also have a .fit_transform() method, but it is usually not fitting anything."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
-            "id": "c02716d7",
+            "id": "d2276e30",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:16.565481Z",
-                    "iopub.status.busy": "2022-12-09T17:05:16.565012Z",
-                    "iopub.status.idle": "2022-12-09T17:05:16.573625Z",
-                    "shell.execute_reply": "2022-12-09T17:05:16.573134Z"
+                    "iopub.execute_input": "2023-03-19T08:54:22.987984Z",
+                    "iopub.status.busy": "2023-03-19T08:54:22.987693Z",
+                    "iopub.status.idle": "2023-03-19T08:54:22.992008Z",
+                    "shell.execute_reply": "2023-03-19T08:54:22.991412Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "fps is a <class 'numpy.ndarray'> with shape (6, 256) and data type float64\n"
+                        "fps is a <class 'numpy.ndarray'> with shape (6, 256) and data type int8\n"
                     ]
                 }
             ],
             "source": [
                 "fps = transformer.transform(mols)\n",
                 "print(f\"fps is a {type(fps)} with shape {fps.shape} and data type {fps.dtype}\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9b0835ed",
+            "id": "666bf64b",
             "metadata": {},
             "source": [
                 "For sklearn compatibility, the transform function can be given a second parameter, usually representing the targets in the machine learning, but it is simply ignored most of the time"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
-            "id": "f957a045",
+            "id": "d3b01806",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:16.581311Z",
-                    "iopub.status.busy": "2022-12-09T17:05:16.579338Z",
-                    "iopub.status.idle": "2022-12-09T17:05:16.588090Z",
-                    "shell.execute_reply": "2022-12-09T17:05:16.587455Z"
+                    "iopub.execute_input": "2023-03-19T08:54:22.994560Z",
+                    "iopub.status.busy": "2023-03-19T08:54:22.994348Z",
+                    "iopub.status.idle": "2023-03-19T08:54:22.999695Z",
+                    "shell.execute_reply": "2023-03-19T08:54:22.999044Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "array([[0., 1., 0., ..., 0., 0., 0.],\n",
-                            "       [1., 0., 0., ..., 0., 0., 1.],\n",
-                            "       [1., 0., 0., ..., 0., 0., 0.],\n",
-                            "       [0., 0., 0., ..., 0., 0., 1.],\n",
-                            "       [1., 1., 0., ..., 0., 0., 0.],\n",
-                            "       [1., 1., 0., ..., 0., 0., 0.]])"
+                            "array([[0, 1, 0, ..., 0, 0, 0],\n",
+                            "       [1, 0, 0, ..., 0, 0, 1],\n",
+                            "       [1, 0, 0, ..., 0, 0, 0],\n",
+                            "       [0, 0, 0, ..., 0, 0, 1],\n",
+                            "       [1, 1, 0, ..., 0, 0, 0],\n",
+                            "       [1, 1, 0, ..., 0, 0, 0]], dtype=int8)"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "y = range(len(mols))\n",
                 "transformer.transform(mols, y)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0c58cdeb",
+            "id": "1e5c385f",
             "metadata": {},
             "source": [
                 "Sometimes we may want to transform SMILES into molecules, and scikit-mol also has a transformer for that. It simply takes a list of SMILES and produces a list of RDKit molecules, this may come in handy when building pipelines for machine learning models, as we will demo in another notebook."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
-            "id": "b567acfa",
+            "id": "26081bb2",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:16.592991Z",
-                    "iopub.status.busy": "2022-12-09T17:05:16.592379Z",
-                    "iopub.status.idle": "2022-12-09T17:05:16.595717Z",
-                    "shell.execute_reply": "2022-12-09T17:05:16.596135Z"
+                    "iopub.execute_input": "2023-03-19T08:54:23.002288Z",
+                    "iopub.status.busy": "2023-03-19T08:54:23.002005Z",
+                    "iopub.status.idle": "2023-03-19T08:54:23.006182Z",
+                    "shell.execute_reply": "2023-03-19T08:54:23.005653Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "SmilesToMol()\n"
                     ]
                 }
             ],
             "source": [
-                "from scikit_mol.transformers import SmilesToMol\n",
-                "smi2mol = SmilesToMol()\n",
+                "from scikit_mol.conversions import SmilesToMolTransformer\n",
+                "smi2mol = SmilesToMolTransformer()\n",
                 "print(smi2mol)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
-            "id": "0c8093fd",
+            "id": "6b0e5f4a",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:16.605135Z",
-                    "iopub.status.busy": "2022-12-09T17:05:16.604217Z",
-                    "iopub.status.idle": "2022-12-09T17:05:16.607427Z",
-                    "shell.execute_reply": "2022-12-09T17:05:16.607829Z"
+                    "iopub.execute_input": "2023-03-19T08:54:23.009239Z",
+                    "iopub.status.busy": "2023-03-19T08:54:23.008966Z",
+                    "iopub.status.idle": "2023-03-19T08:54:23.014260Z",
+                    "shell.execute_reply": "2023-03-19T08:54:23.013537Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[<rdkit.Chem.rdchem.Mol object at 0x7f773ee10d60>, <rdkit.Chem.rdchem.Mol object at 0x7f773ee10b80>, <rdkit.Chem.rdchem.Mol object at 0x7f773ee10f40>, <rdkit.Chem.rdchem.Mol object at 0x7f773ee10fa0>, <rdkit.Chem.rdchem.Mol object at 0x7f773ee10dc0>, <rdkit.Chem.rdchem.Mol object at 0x7f773eda6040>]\n"
+                        "[<rdkit.Chem.rdchem.Mol object at 0x7fb1ac449af0>, <rdkit.Chem.rdchem.Mol object at 0x7fb1ac449b60>, <rdkit.Chem.rdchem.Mol object at 0x7fb1ac449bd0>, <rdkit.Chem.rdchem.Mol object at 0x7fb1ac449c40>, <rdkit.Chem.rdchem.Mol object at 0x7fb1ac449cb0>, <rdkit.Chem.rdchem.Mol object at 0x7fb1ac449d20>]\n"
                     ]
                 }
             ],
             "source": [
                 "print(smi2mol.transform(smiles_strings))"
             ]
         }
@@ -371,18 +372,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.4"
-        },
-        "vscode": {
-            "interpreter": {
-                "hash": "dc6218d6ccd9a44863300cd5111a59d6c18db4de812eb936d6a68ad5fa5cf18f"
-            }
+            "version": "3.10.9"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `scikit_mol-0.1.2/notebooks/01_basic_usage.py` & `scikit_mol-0.2.0/notebooks/01_basic_usage.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # jupyter:
 #   jupytext:
 #     formats: ipynb,py:percent
 #     text_representation:
 #       extension: .py
 #       format_name: percent
 #       format_version: '1.3'
-#       jupytext_version: 1.14.1
+#       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3.9.4 ('rdkit')
 #     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
@@ -38,17 +38,17 @@
 
 mols = [Chem.MolFromSmiles(smiles) for smiles in smiles_strings]
 
 # %% [markdown]
 # Next we import the Morgan fingerprint transformer
 
 # %%
-from scikit_mol.transformers import MorganTransformer
+from scikit_mol.fingerprints import MorganFingerprintTransformer
 
-transformer = MorganTransformer(radius=3)
+transformer = MorganFingerprintTransformer(radius=3)
 print(transformer)
 
 # %% [markdown]
 # It actually renders as a cute little interactive block in the Jupyter notebook and lists the options that are not the default values. If we print it, it also gives the information on the settings. 
 #
 # ![An image of the interactive transformer widget](images/Transformer_Widget.jpg "Transformer object rendering in Jupyter")
 #
@@ -87,13 +87,13 @@
 y = range(len(mols))
 transformer.transform(mols, y)
 
 # %% [markdown]
 # Sometimes we may want to transform SMILES into molecules, and scikit-mol also has a transformer for that. It simply takes a list of SMILES and produces a list of RDKit molecules, this may come in handy when building pipelines for machine learning models, as we will demo in another notebook.
 
 # %%
-from scikit_mol.transformers import SmilesToMol
-smi2mol = SmilesToMol()
+from scikit_mol.conversions import SmilesToMolTransformer
+smi2mol = SmilesToMolTransformer()
 print(smi2mol)
 
 # %%
 print(smi2mol.transform(smiles_strings))
```

### Comparing `scikit_mol-0.1.2/notebooks/02_descriptor_transformer.py` & `scikit_mol-0.2.0/notebooks/02_descriptor_transformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #   jupytext:
 #     cell_metadata_filter: -all
 #     formats: ipynb,py:percent
 #     text_representation:
 #       extension: .py
 #       format_name: percent
 #       format_version: '1.3'
-#       jupytext_version: 1.14.1
+#       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3.9.4 ('rdkit')
 #     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
@@ -19,20 +19,20 @@
 #
 # The descriptors transformer can convert molecules into a list of RDKit descriptors. It largely follows the API of the other transformers, but has a few extra methods and properties to manage the descriptors.
 
 # %%
 from rdkit import Chem
 import numpy as np
 import matplotlib.pyplot as plt
-from scikit_mol.descriptors import Desc2DTransformer
+from scikit_mol.descriptors import MolecularDescriptorTransformer
 # %% [markdown]
 # After instantiation of the descriptor transformer, we can query which descriptors it found available in the RDKit framework.
 
 # %%
-descriptor = Desc2DTransformer()
+descriptor = MolecularDescriptorTransformer()
 available_descriptors = descriptor.available_descriptors
 print(f"There are {len(available_descriptors)} available descriptors")
 print(f"The first five descriptor names: {available_descriptors[:5]}")
 
 # %% [markdown]
 # We can transform molecules to their descriptor profiles
 
@@ -43,15 +43,15 @@
 features = descriptor.transform(mols)
 _ = plt.plot(np.array(features).T)
 
 # %% [markdown]
 # If we only want some of them, this can be specified at object instantiation.
 
 # %%
-some_descriptors = Desc2DTransformer(desc_list=['HeavyAtomCount', 'FractionCSP3', 'RingCount', 'MolLogP', 'MolWt'])
+some_descriptors = MolecularDescriptorTransformer(desc_list=['HeavyAtomCount', 'FractionCSP3', 'RingCount', 'MolLogP', 'MolWt'])
 print(f"Selected descriptors are {some_descriptors.selected_descriptors}")
 features = some_descriptors.transform(mols)
 
 # %% [markdown]
 # If we want to update the selected descriptors on an already existing object, this can be done via the .set_params() method
 
 # %%
```

### Comparing `scikit_mol-0.1.2/notebooks/02_descriptor_transformer_files/02_descriptor_transformer_5_0.png` & `scikit_mol-0.2.0/notebooks/02_descriptor_transformer_files/02_descriptor_transformer_5_0.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/03_example_pipeline.ipynb` & `scikit_mol-0.2.0/notebooks/03_example_pipeline.ipynb`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8150337076118326%*

 * *Differences: {"'cells'": "{0: {'id': 'f3f842d3'}, 1: {'metadata': {'execution': {'iopub.execute_input': "*

 * *            "'2023-03-19T08:54:27.653561Z', 'iopub.status.busy': '2023-03-19T08:54:27.653105Z', "*

 * *            "'iopub.status.idle': '2023-03-19T08:54:28.385099Z', 'shell.execute_reply': "*

 * *            "'2023-03-19T08:54:28.384146Z'}}, 'id': 'b92c5a96'}, 2: {'metadata': {'execution': "*

 * *            "{'iopub.execute_input': '2023-03-19T08:54:28.388213Z', 'iopub.status.busy': "*

 * *            "'2023-03-19T08:54:28.387874Z', […]*

```diff
@@ -1,29 +1,31 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
+            "id": "f3f842d3",
             "metadata": {},
             "source": [
                 "# Pipelining the scikit-mol transformer\n",
                 "\n",
                 "One of the very usable things with scikit-learn are their pipelines. With pipelines different scikit-learn transformers can be stacked and operated on just as a single model object. In this example we will build a simple model that can predict directly on RDKit molecules and then expand it to one that predicts directly on SMILES strings\n",
                 "\n",
                 "First some needed imports and a dataset"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
+            "id": "b92c5a96",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:22.596037Z",
-                    "iopub.status.busy": "2022-12-09T17:05:22.595197Z",
-                    "iopub.status.idle": "2022-12-09T17:05:23.571104Z",
-                    "shell.execute_reply": "2022-12-09T17:05:23.572385Z"
+                    "iopub.execute_input": "2023-03-19T08:54:27.653561Z",
+                    "iopub.status.busy": "2023-03-19T08:54:27.653105Z",
+                    "iopub.status.idle": "2023-03-19T08:54:28.385099Z",
+                    "shell.execute_reply": "2023-03-19T08:54:28.384146Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "import rdkit\n",
                 "from rdkit import Chem\n",
@@ -33,47 +35,50 @@
                 "from time import time\n",
                 "import numpy as np"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
+            "id": "0d79bc45",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:23.578194Z",
-                    "iopub.status.busy": "2022-12-09T17:05:23.576362Z",
-                    "iopub.status.idle": "2022-12-09T17:05:23.587619Z",
-                    "shell.execute_reply": "2022-12-09T17:05:23.588644Z"
+                    "iopub.execute_input": "2023-03-19T08:54:28.388213Z",
+                    "iopub.status.busy": "2023-03-19T08:54:28.387874Z",
+                    "iopub.status.idle": "2023-03-19T08:54:28.394786Z",
+                    "shell.execute_reply": "2023-03-19T08:54:28.394110Z"
                 },
                 "lines_to_next_cell": 0
             },
             "outputs": [],
             "source": [
                 "csv_file = \"../tests/data/SLC6A4_active_excapedb_subset.csv\" # Hmm, maybe better to download directly\n",
                 "data = pd.read_csv(csv_file)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "3569affd",
             "metadata": {},
             "source": [
                 "The dataset is a subset of the SLC6A4 actives from ExcapeDB. They are hand selected to give test set performance despite the small size, and are provided as example data only and should not be used to build serious QSAR models.\n",
                 "\n",
                 "We add RDKit mol objects to the dataframe with pandastools and check that all conversions went well."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
+            "id": "594f45ba",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:23.594260Z",
-                    "iopub.status.busy": "2022-12-09T17:05:23.592486Z",
-                    "iopub.status.idle": "2022-12-09T17:05:23.665835Z",
-                    "shell.execute_reply": "2022-12-09T17:05:23.666912Z"
+                    "iopub.execute_input": "2023-03-19T08:54:28.397967Z",
+                    "iopub.status.busy": "2023-03-19T08:54:28.397752Z",
+                    "iopub.status.idle": "2023-03-19T08:54:28.436822Z",
+                    "shell.execute_reply": "2023-03-19T08:54:28.436140Z"
                 },
                 "lines_to_next_cell": 0
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -85,104 +90,112 @@
             "source": [
                 "PandasTools.AddMoleculeColumnToFrame(data, smilesCol=\"SMILES\")\n",
                 "print(f\"{data.ROMol.isna().sum()} out of {len(data)} SMILES failed in conversion\")"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "04af16b2",
             "metadata": {},
             "source": [
                 "Then, let's import some tools from scikit-learn and two transformers from scikit-mol"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
+            "id": "ed19f736",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:23.672213Z",
-                    "iopub.status.busy": "2022-12-09T17:05:23.670546Z",
-                    "iopub.status.idle": "2022-12-09T17:05:24.247618Z",
-                    "shell.execute_reply": "2022-12-09T17:05:24.249061Z"
+                    "iopub.execute_input": "2023-03-19T08:54:28.439485Z",
+                    "iopub.status.busy": "2023-03-19T08:54:28.439232Z",
+                    "iopub.status.idle": "2023-03-19T08:54:28.834836Z",
+                    "shell.execute_reply": "2023-03-19T08:54:28.833932Z"
                 },
                 "lines_to_next_cell": 0
             },
             "outputs": [],
             "source": [
                 "from sklearn.pipeline import Pipeline\n",
                 "from sklearn.linear_model import Ridge\n",
                 "from sklearn.model_selection import train_test_split\n",
-                "from scikit_mol.transformers import MorganTransformer, SmilesToMol"
+                "from scikit_mol.fingerprints import MorganFingerprintTransformer\n",
+                "from scikit_mol.conversions import SmilesToMolTransformer"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
+            "id": "c4a255f4",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:24.254941Z",
-                    "iopub.status.busy": "2022-12-09T17:05:24.253181Z",
-                    "iopub.status.idle": "2022-12-09T17:05:24.265332Z",
-                    "shell.execute_reply": "2022-12-09T17:05:24.265976Z"
+                    "iopub.execute_input": "2023-03-19T08:54:28.838155Z",
+                    "iopub.status.busy": "2023-03-19T08:54:28.837767Z",
+                    "iopub.status.idle": "2023-03-19T08:54:28.842399Z",
+                    "shell.execute_reply": "2023-03-19T08:54:28.841851Z"
                 }
             },
             "outputs": [],
             "source": [
                 "mol_list_train, mol_list_test, y_train, y_test = train_test_split(data.ROMol, data.pXC50, random_state=0)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "a088665f",
             "metadata": {},
             "source": [
                 "After a split into train and test, we'll build the first pipeline"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
+            "id": "0ddbf668",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:24.275680Z",
-                    "iopub.status.busy": "2022-12-09T17:05:24.272313Z",
-                    "iopub.status.idle": "2022-12-09T17:05:24.285661Z",
-                    "shell.execute_reply": "2022-12-09T17:05:24.285068Z"
+                    "iopub.execute_input": "2023-03-19T08:54:28.845331Z",
+                    "iopub.status.busy": "2023-03-19T08:54:28.845041Z",
+                    "iopub.status.idle": "2023-03-19T08:54:28.851043Z",
+                    "shell.execute_reply": "2023-03-19T08:54:28.850277Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Pipeline(steps=[('mol_transformer', MorganTransformer()),\n",
                         "                ('Regressor', Ridge())])\n"
                     ]
                 }
             ],
             "source": [
-                "pipe = Pipeline([('mol_transformer', MorganTransformer()), ('Regressor', Ridge())])\n",
+                "pipe = Pipeline([('mol_transformer', MorganFingerprintTransformer()), ('Regressor', Ridge())])\n",
                 "print(pipe)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "004b0d25",
             "metadata": {},
             "source": [
                 "We can do the fit by simply providing the list of RDKit molecule objects"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
+            "id": "231d0534",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:24.292814Z",
-                    "iopub.status.busy": "2022-12-09T17:05:24.291238Z",
-                    "iopub.status.idle": "2022-12-09T17:05:24.465316Z",
-                    "shell.execute_reply": "2022-12-09T17:05:24.465945Z"
+                    "iopub.execute_input": "2023-03-19T08:54:28.853975Z",
+                    "iopub.status.busy": "2023-03-19T08:54:28.853718Z",
+                    "iopub.status.idle": "2023-03-19T08:54:28.944670Z",
+                    "shell.execute_reply": "2023-03-19T08:54:28.943808Z"
                 },
                 "lines_to_next_cell": 0
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -196,62 +209,66 @@
                 "pipe.fit(mol_list_train, y_train)\n",
                 "print(f\"Train score is :{pipe.score(mol_list_train,y_train):0.2F}\")\n",
                 "print(f\"Test score is  :{pipe.score(mol_list_test, y_test):0.2F}\")"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "55915786",
             "metadata": {},
             "source": [
                 "Nevermind the performance, or the exact value of the prediction, this is for demonstration purpures. We can easily predict on lists of molecules"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
+            "id": "5d1e9220",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:24.470874Z",
-                    "iopub.status.busy": "2022-12-09T17:05:24.470149Z",
-                    "iopub.status.idle": "2022-12-09T17:05:24.483910Z",
-                    "shell.execute_reply": "2022-12-09T17:05:24.484664Z"
+                    "iopub.execute_input": "2023-03-19T08:54:28.949968Z",
+                    "iopub.status.busy": "2023-03-19T08:54:28.949504Z",
+                    "iopub.status.idle": "2023-03-19T08:54:28.964037Z",
+                    "shell.execute_reply": "2023-03-19T08:54:28.963010Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([6.00400299])"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "pipe.predict([Chem.MolFromSmiles('c1ccccc1C(=O)[OH]')])"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "07cf53ea",
             "metadata": {},
             "source": [
                 "We can also expand the already fitted pipeline, how about creating a pipeline that can predict directly from SMILES? With scikit-mol that is easy!"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
+            "id": "eb8ce486",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:24.491861Z",
-                    "iopub.status.busy": "2022-12-09T17:05:24.491111Z",
-                    "iopub.status.idle": "2022-12-09T17:05:24.506048Z",
-                    "shell.execute_reply": "2022-12-09T17:05:24.506671Z"
+                    "iopub.execute_input": "2023-03-19T08:54:28.969289Z",
+                    "iopub.status.busy": "2023-03-19T08:54:28.968614Z",
+                    "iopub.status.idle": "2023-03-19T08:54:28.983422Z",
+                    "shell.execute_reply": "2023-03-19T08:54:28.982473Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -259,61 +276,64 @@
                         "                ('pipe',\n",
                         "                 Pipeline(steps=[('mol_transformer', MorganTransformer()),\n",
                         "                                 ('Regressor', Ridge())]))])\n"
                     ]
                 }
             ],
             "source": [
-                "smiles_pipe = Pipeline([('smiles_transformer', SmilesToMol()), ('pipe', pipe)])\n",
+                "smiles_pipe = Pipeline([('smiles_transformer', SmilesToMolTransformer()), ('pipe', pipe)])\n",
                 "print(smiles_pipe)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
+            "id": "1444b605",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:24.514152Z",
-                    "iopub.status.busy": "2022-12-09T17:05:24.513303Z",
-                    "iopub.status.idle": "2022-12-09T17:05:24.522451Z",
-                    "shell.execute_reply": "2022-12-09T17:05:24.523095Z"
+                    "iopub.execute_input": "2023-03-19T08:54:28.988161Z",
+                    "iopub.status.busy": "2023-03-19T08:54:28.987478Z",
+                    "iopub.status.idle": "2023-03-19T08:54:28.995432Z",
+                    "shell.execute_reply": "2023-03-19T08:54:28.994415Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([6.00400299])"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "smiles_pipe.predict(['c1ccccc1C(=O)[OH]'])"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "90d7817b",
             "metadata": {},
             "source": [
                 "From here, the pipelines could be pickled, and later loaded for easy prediction on RDKit molecule objects or SMILES in other scripts. The transformation with the MorganTransformer will be the same as during fitting, so no need to remember if radius 2 or 3 was used for this or that model, as it is already in the pipeline itself. If we need to see the parameters for a particular pipeline of model, we can always get the non default settings via print or all settings with .get_params()."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
+            "id": "1eacda8f",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:24.528383Z",
-                    "iopub.status.busy": "2022-12-09T17:05:24.527563Z",
-                    "iopub.status.idle": "2022-12-09T17:05:24.549223Z",
-                    "shell.execute_reply": "2022-12-09T17:05:24.549973Z"
+                    "iopub.execute_input": "2023-03-19T08:54:29.000764Z",
+                    "iopub.status.busy": "2023-03-19T08:54:29.000309Z",
+                    "iopub.status.idle": "2023-03-19T08:54:29.015001Z",
+                    "shell.execute_reply": "2023-03-19T08:54:29.014049Z"
                 },
                 "lines_to_next_cell": 2
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
@@ -322,38 +342,39 @@
                             "  ('pipe',\n",
                             "   Pipeline(steps=[('mol_transformer', MorganTransformer()),\n",
                             "                   ('Regressor', Ridge())]))],\n",
                             " 'verbose': False,\n",
                             " 'smiles_transformer': SmilesToMol(),\n",
                             " 'pipe': Pipeline(steps=[('mol_transformer', MorganTransformer()),\n",
                             "                 ('Regressor', Ridge())]),\n",
+                            " 'smiles_transformer__parallel': False,\n",
                             " 'pipe__memory': None,\n",
                             " 'pipe__steps': [('mol_transformer', MorganTransformer()),\n",
                             "  ('Regressor', Ridge())],\n",
                             " 'pipe__verbose': False,\n",
                             " 'pipe__mol_transformer': MorganTransformer(),\n",
                             " 'pipe__Regressor': Ridge(),\n",
                             " 'pipe__mol_transformer__nBits': 2048,\n",
+                            " 'pipe__mol_transformer__parallel': False,\n",
                             " 'pipe__mol_transformer__radius': 2,\n",
                             " 'pipe__mol_transformer__useBondTypes': True,\n",
                             " 'pipe__mol_transformer__useChirality': False,\n",
                             " 'pipe__mol_transformer__useCounts': False,\n",
                             " 'pipe__mol_transformer__useFeatures': False,\n",
                             " 'pipe__Regressor__alpha': 1.0,\n",
                             " 'pipe__Regressor__copy_X': True,\n",
                             " 'pipe__Regressor__fit_intercept': True,\n",
                             " 'pipe__Regressor__max_iter': None,\n",
-                            " 'pipe__Regressor__normalize': 'deprecated',\n",
                             " 'pipe__Regressor__positive': False,\n",
                             " 'pipe__Regressor__random_state': None,\n",
                             " 'pipe__Regressor__solver': 'auto',\n",
-                            " 'pipe__Regressor__tol': 0.001}"
+                            " 'pipe__Regressor__tol': 0.0001}"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "smiles_pipe.get_params()"
             ]
@@ -375,18 +396,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.4"
-        },
-        "vscode": {
-            "interpreter": {
-                "hash": "dc6218d6ccd9a44863300cd5111a59d6c18db4de812eb936d6a68ad5fa5cf18f"
-            }
+            "version": "3.10.9"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 5
 }
```

### Comparing `scikit_mol-0.1.2/notebooks/03_example_pipeline.py` & `scikit_mol-0.2.0/notebooks/03_example_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #   jupytext:
 #     cell_metadata_filter: title,-all
 #     formats: ipynb,py:percent
 #     text_representation:
 #       extension: .py
 #       format_name: percent
 #       format_version: '1.3'
-#       jupytext_version: 1.14.1
+#       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3.9.4 ('rdkit')
 #     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
@@ -45,23 +45,24 @@
 # %% [markdown]
 # Then, let's import some tools from scikit-learn and two transformers from scikit-mol
 
 # %%
 from sklearn.pipeline import Pipeline
 from sklearn.linear_model import Ridge
 from sklearn.model_selection import train_test_split
-from scikit_mol.transformers import MorganTransformer, SmilesToMol
+from scikit_mol.fingerprints import MorganFingerprintTransformer
+from scikit_mol.conversions import SmilesToMolTransformer
 # %%
 mol_list_train, mol_list_test, y_train, y_test = train_test_split(data.ROMol, data.pXC50, random_state=0)
 
 # %% [markdown]
 # After a split into train and test, we'll build the first pipeline
 
 # %%
-pipe = Pipeline([('mol_transformer', MorganTransformer()), ('Regressor', Ridge())])
+pipe = Pipeline([('mol_transformer', MorganFingerprintTransformer()), ('Regressor', Ridge())])
 print(pipe)
 
 # %% [markdown]
 # We can do the fit by simply providing the list of RDKit molecule objects
 
 # %%
 pipe.fit(mol_list_train, y_train)
@@ -73,15 +74,15 @@
 # %%
 pipe.predict([Chem.MolFromSmiles('c1ccccc1C(=O)[OH]')])
 
 # %% [markdown]
 # We can also expand the already fitted pipeline, how about creating a pipeline that can predict directly from SMILES? With scikit-mol that is easy!
 
 # %%
-smiles_pipe = Pipeline([('smiles_transformer', SmilesToMol()), ('pipe', pipe)])
+smiles_pipe = Pipeline([('smiles_transformer', SmilesToMolTransformer()), ('pipe', pipe)])
 print(smiles_pipe)
 
 # %%
 smiles_pipe.predict(['c1ccccc1C(=O)[OH]'])
 
 # %% [markdown]
 # From here, the pipelines could be pickled, and later loaded for easy prediction on RDKit molecule objects or SMILES in other scripts. The transformation with the MorganTransformer will be the same as during fitting, so no need to remember if radius 2 or 3 was used for this or that model, as it is already in the pipeline itself. If we need to see the parameters for a particular pipeline of model, we can always get the non default settings via print or all settings with .get_params().
```

### Comparing `scikit_mol-0.1.2/notebooks/04_standardizer.ipynb` & `scikit_mol-0.2.0/notebooks/04_standardizer.ipynb`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8142476851851852%*

 * *Differences: {"'cells'": "{0: {'id': 'be682e9c'}, 1: {'metadata': {'execution': {'iopub.execute_input': "*

 * *            "'2023-03-19T08:54:30.753417Z', 'iopub.status.busy': '2023-03-19T08:54:30.753027Z', "*

 * *            "'iopub.status.idle': '2023-03-19T08:54:31.649909Z', 'shell.execute_reply': "*

 * *            "'2023-03-19T08:54:31.649009Z'}}, 'source': {insert: [(2, 'from "*

 * *            "scikit_mol.fingerprints import MorganFingerprintTransformer\\n'), (3, 'from "*

 * *            "scikit_mol.conversions import SmilesToMolTransfor […]*

```diff
@@ -1,149 +1,158 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
+            "id": "be682e9c",
             "metadata": {},
             "source": [
                 "# Molecule standardization\n",
                 "When building machine learning models of molecules, it is important to standardize the molecules. We often don't want different predictions just because things are drawn in slightly different forms, such as protonated or deprotanted carboxylic acids. Scikit-mol provides a very basic standardize transformer based on the molvs implementation in RDKit"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
+            "id": "2aa91923",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:26.283410Z",
-                    "iopub.status.busy": "2022-12-09T17:05:26.282880Z",
-                    "iopub.status.idle": "2022-12-09T17:05:26.971413Z",
-                    "shell.execute_reply": "2022-12-09T17:05:26.972141Z"
+                    "iopub.execute_input": "2023-03-19T08:54:30.753417Z",
+                    "iopub.status.busy": "2023-03-19T08:54:30.753027Z",
+                    "iopub.status.idle": "2023-03-19T08:54:31.649909Z",
+                    "shell.execute_reply": "2023-03-19T08:54:31.649009Z"
                 }
             },
             "outputs": [],
             "source": [
                 "from rdkit import Chem\n",
                 "from scikit_mol.standardizer import Standardizer\n",
-                "from scikit_mol.transformers import MorganTransformer, SmilesToMol\n",
+                "from scikit_mol.fingerprints import MorganFingerprintTransformer\n",
+                "from scikit_mol.conversions import SmilesToMolTransformer\n",
                 "from sklearn.pipeline import make_pipeline\n",
                 "from sklearn.linear_model import Ridge"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "0fed8d0b",
             "metadata": {},
             "source": [
                 "For demonstration let's create some molecules with different protonation states. The two first molecules are Benzoic acid and Sodium benzoate."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
+            "id": "934c031b",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:26.995515Z",
-                    "iopub.status.busy": "2022-12-09T17:05:26.994760Z",
-                    "iopub.status.idle": "2022-12-09T17:05:27.004591Z",
-                    "shell.execute_reply": "2022-12-09T17:05:27.005011Z"
+                    "iopub.execute_input": "2023-03-19T08:54:31.653346Z",
+                    "iopub.status.busy": "2023-03-19T08:54:31.653052Z",
+                    "iopub.status.idle": "2023-03-19T08:54:31.676827Z",
+                    "shell.execute_reply": "2023-03-19T08:54:31.676081Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAcIAAACWCAIAAADCEh9HAAAABmJLR0QA/wD/AP+gvaeTAAAe0UlEQVR4nO3dd1iV5f8H8DdDQAQZ4QpMUWSIgiiaA2eOBoUrDAeaYmlqICJuxU1qSpiWlplpaV/LkZqlqYUmliEOhmBuxJAVGw7nnPv3x8MPyxCeA+c59xmf1+UfXPrB631x2bv7POO+jRhjIIQQUl/GvAMQQohuoxolhJAGoRolhJAGoRolhJAGoRolhJAGMeUdgBAigfJy5OSgqAg2NnBwgJkZ70D6jFajhOiRigps3gw/P1hbo3VrdOwIR0fY2GDIEOzaBYWCdz79ZETPjRKiJ65eRUAA7tx56oC3Nw4fRps2motkGGg1SoheSEpCv364cwdGRggKwqlTKCgAY8jNxZEjGDIEAK5cQe/eePCAd1Z9Q6tRQnSfTIbu3XH1KkxNsXs33nijhpnVq7F4MQAMHYoff9RwQP1Gq1FCdN833+DqVQCYO7fmDgWwaBFGjgSAEydw7pzmshkAqlFCdN+nnwKAhQXmzq1tbPnyf80TNaEaJUTHVVbiwgUAGDAAdna1TXbqBA8PAIiL00Qwg0E1SoiOu34dZWUA4ONT93DXrgBw+zYKCqRNZUjo8XvOtm7dev/+fd4p1MDX13fUqFG8UxiknJyqL1q2rHu4eiYnBzY2UkUyMFSj3BQVFQ0cODA3N/dOLQ/66Y4ePXps2bLlp59+MjamjziaVVxc9YWlZd3DVlZVXxQVSZXH8FCNcrNy5cqEhAQXF5fVq1cbGRnxjtMglZWVH374YXZ29u7duydOnMg7joGpbkbho33tSkqqvrC2liqP4aEa5ePmzZuxsbHGxsZfffVV9+7decdRA2dn5+Dg4Hnz5o0YMaJp06a84xgSe/uqL7Kz6x5+9OjJ7yINRp+/+AgPD6+oqJg0aZJ+dCiA8ePH9+nTJysr67333uOdxcC4uVXtPCI8Olq7K1cAoHXrOu7pE1XQW0wcnDp1avDgwdbW1mlpaa1ateIdR20SEhJ69OhhamqalJTUoUMH3nEMSa9euHABTZvi4cParpDevYt27aBU4o03sHevBvPpOVqNappcLp89ezaAxYsX61OHAujWrdv48eNlMtn8+fN5ZzEwwcEAUFhYx3P1GzdCqQSASZM0EMpw0GpU02JjY0NDQ9u3b5+cnGxubs47jpplZWW5uroWFhb++OOPQ4cO5R3HYBQXw8MDGRlo2hSnT6Nbtxpmjh1DQAAUCnTvjt9+g47f1dQqtBrVqLy8vBUrVgDYuHGj/nUogBYtWsybNw/A7Nmz5XI57zgGw8oKn30GExMUFmLQIMTEoLDw8Z/m5GDZMowcCYUCTZpg1y7qUPWi1ahGzZgxY+vWrS+88MJPP/3EO4tUZDJZp06dbty4sXXr1unTp/OOo48KC2FtXUMVHjyIceOqHnsyM4ObG+ztkZ2NtLSqDZsdHHDkCHr21HRgfUc1qjkpKSne3t6MscTExM6dO/OOI6EDBw6MGjXK3t4+PT39mWee4R1H7/j7o6AAO3fCxeXJP7p9G0uX4uDBx8+HCuzsMH48lixBs2Yai2k4qEY1Z9iwYSdOnJg1a1ZsbCzvLJIbOnToyZMnQ0NDY2JieGfRLydPYuhQNG2KtLSnvv1ZUYGLF3H/PoqKYGeHNm3QtStM6SFxqVCNasjBgwdHjhxpZ2d348YNQ1igJScnd+nSBUBiYmKnTp14x9EXcjm6dEFyMt5/H+HhvNOQKnSLSRNkMplw42XlypWG0KEAPD09p06dKpfLw8LCeGfRI5s3IzkZLi6YMYN3FPIYrUY1ITo6esGCBR07drxy5YqpwXy2ysvLc3V1zc3NPXLkiL+/P+84ui8vDx06IC8PR4/ilVd4pyGP0WpUcllZWWvXrgWwadMmw+lQAPb29kuWLAEQFhZWUVHBO47uW7gQeXkYPJg6VNtQjUpu/vz5hYWFw4cPF/M4emZm5vnz5zWQqoGOHDkiphlnzJjRqVOnmzdvbt68WQOp9FlyMnbsgKkpRN6yO3MG9NyuxjAipYSEBGNjYzMzs/T0dDHzwcHBRkZGH3zwgdTBGuLtt98G8N5774kZPnnyJABra+vMzEypg+mzAQMYwGbPFjV86RIzMWE+PqyyUuJYhDHGqEYlpFQq/fz8AMyfP1/M/B9//CF07o0bN6TO1hCnTp1SqRmFC6MhISFSB9Nb+/czgNnbs9xcUfP9+zOAzZkjcSxShWpUQnv27AHQokWLgoKCOoeVSmWfPn0ALFy4UAPZGui1114DMHnyZDHDf/75p7m5ubGx8cWLF6UOpofKypizMwPYxx+Lmt+3jwGseXOWny9xMlKFalQqpaWlzz33HICdO3eKmd+1a5f4zuWuuhl/++03MfNz5swB0Lt3b6VSKXU2fbNyJQOYp6eoT+ilpaxtWwaw7dulT0aqUI1KRbhJ3bVrV4VCUedwSUlJ69atAezatUsD2dQiMjISQK9evcQ0Y2FhYcuWLQHs27dPA9n0R0YGs7JiADtxQtR8VBQDWJcuTC6XOBl5jGpUEvfu3bO0tDQyMoqLixMzv2jRIgDdunUT07laorCwUNgv9auvvhIzv337dgBOTk7FxcVSZ9Mf48czgI0eLWo4I4M1acIA9vPPEsci/0I1KonXX38dwLhx48QM37p1y8LCwsjI6OzZs1IHU68dO3aIb0aFQuHr6wsgKipKA9n0QXw8MzJi5uZM5C3HsWMZwAIDJY5FnkQ1qn7nzp0zMjJq3Ljx3bt3xcwLx7tPmDBB6mBqp1AohLOkli1bJmb+119/FX4yd+7ckTia7lMq2fPPM4AtWiRq/vx5ZmTEGjdmt29LG4z8B9WomlWvuVasWCFm/vTp0wAsLS1Fdq62OX/+vNCMt8X91xsYGAhg7NixEufSfZ9/zgDm6MiKiuoeVihYjx4MYEuXSp+MPIlqVM22bdsGoHXr1iUlJXUOy+Vyb29vAKtWrdJANokEBQUBGDNmjJhhVa8aG6iiIvbsswxgX3whan7HjqrOpevOPFCNqlNBQYFwP/rrr78WM//RRx+J71ytdf/+/SZNmgD4WdydjaVLlwLw8fHRoftpmrZgAQNYz55MzPNhhYWsVSsGsC+/lD4ZqQHVqDqFh4cD6NOnj5hngPLz85s1awZg//79GsgmqaioKABdunSRi3jOprS0tE2bNgB27NihgWy65+ZNZmHBjIzYhQui5ufNYwDr1UtU5xIJUI2qzY0bN1R6V0fYiNPPz08PnkivbsZPPvlEzPyXX34JoHnz5n///bfU2XTPiBEMYBMnihq+eZOZmzNjYybuPQgiBapRtXn55ZcBvPXWW2KGU1NTGzVqZGxs/Mcff0gdTDP27t0rvhmVSmXfvn0BREZGaiCbLjl9mgHMyoo9eCBqPiCAAezNNyWORWpDNaoe1fsYPXz4UMz8Sy+9BGDatGlSB9Okfv36AYiIiBAzfOnSJWEflrS0NKmD6Qy5nHl5MYCtXi1q/tQpBjBra0a7Z3FFNaoGlZWVnp6eADZs2CBm/ujRowCaNm36119/SZ1Nky5dumRiYmJmZnb9+nUx82+++SaAgIAAqYPpCsW2bQxgzs6srKzuabmcde7MABYdLX00UhuqUTXYuHEjABcXl/Ly8jqHZTKZm5sbgI0bN2ogm4aFhIQA8Pf3FzP8119/2djYAPjhhx+kDqb98vLyOrVpEz9ggOLbb0V9w+bNDGDt2jER/+qIpKhGGyo3N9fe3h7A0aNHxcxv2LABgLu7u0wmkzqb5mVlZQnNePz4cTHz0dHRADw8PPTyp6GSd999F8DAgQNFTeflMQcHBrCDByXORepGNdpQwlbwgwcPFjOclZVla2sL4Pvvv5c6GC/r1q0T34wVFRWurq4ANm/erIFsWislJaVRo0YmJiZXrlwR9Q0zZzKADRokcS4iCtVogyQlJZmampqamiYlJYmZnzp1KoBXXnlF6mAcVTdjTEyMmPlDhw4BsLOzy87Oljqb1nrxxRcBTJ8+XdR0cjJr1IiZmLCrVyXORUShGm2QIUOGAAgLCxMznJiYaGJi0qhRI5F3YHTXd999p1IzDhs2DMDMmTOlDqadVP1xsWHDGMAM9celhahG62///v0A7O3tc3JyxMz3798fQHh4uNTBtIFKy6vk5GThI+1Vw1teqbp4Z4cOMYDZ2TEDXrxrG6rReiovL3dxcQHw0UcfiZn/+uuvATRr1izfME7IUfVi38yZMwEMMryLfevXr1fpUnJJv34MYLGxGshGRKIaradVq1YB8PT0rBRxQk5paWnbtm0BbNu2TQPZtIRKt57z8vIcHBwAHDp0SOpg2kPVBxvWrVtnZWZ2KjCQTk7WKlSj9ZGRkWFlZQXghLgTclasWCF+5w69Ud2M34p7EHLz5s0A2rVrJ+bxW/1Aj9nqB6rR+pgwYQKAUaNGiRnOyMhQaR85fbJlyxYAzs7OZSJey5HL5Z07dwYQbRiv5dBLX3qDalRl8fHxRkZG5ubmN8SdkDNu3DgAr7/+utTBtJBcLvfy8gKwWtxL4qdOnRK2Jsg0gJfEaQsCvUE1qhqlUvn8888DWCTuhBzhjA0LCwuRZ2zoH+GUFCsrqwfitiwKCAgA8Ka+b1m0b98+2hBLb1CNqubzzz8H0LJly4KCgjqHFQpFjx49ACxZskQD2bTWiBEjAEwUt4HmzZs3hW1bf9PfDTSrbzlu375dzDxtz6rlqEZVUFRU9OyzzwL4QtwJOTt37gTg6Oho4Cez37x5UzhB+oK47dznzZsHoFevXnqwoXWN6LAAPUM1qoKFCxcC6Natm5hDhKo7d8+ePRrIpuUWLFgAoGfPnmKasbCwsFWrVgC+1MfDhVQ9umrZsmV0dJWWoxoV69atW8KS6uzZs2Lm58+fL7449J6qC/kdO3bo60JepYNUqzv3l19+kToYqTeqUbFGjhwJIDg4WMxw9cdYPb7ApyrhsrKjo2ORiIPXqy8rL9Wvg9eFW46NGzcWectxzJgxAIKCgiTORRqEalQUVW83Dx8+HMCkSZOkDqZD6veQg/jG0X6q/r/h119/FX4Cd+7ckTobaQiq0brV7+FH8Z1rOFR95Hbs2LEAAgMDpQ6mGSpdqVAoFL6+vgCioqI0kI00BNVo3bZu3arSqzhC565du1YD2XTO+PHjAYwePVrMsD69AKbqfbNPPvkEgJOTk/5dHdY/VKN1qH4x/JtvvhEz/+GHHwovhovpXAOk6nYEKj0bpM0iIyPFP8VV3bl79+7VQDbSQFSjdQgNDa3HNkUHDhyQOpjuWrlyZT02xxL5pLp2UvWdgoiICAC9e/emxzx0AtVobao3zbx8+bKY+VmzZhnmppkqKSsrc3Z2Fr9Va/V7k7q7VatKb7j++eefQuf+/vvvUgcjakE1WhuVtnBX+VQyA1Z9cEBubq6YeeHggDlz5kgdTCJnzpzx8/MTud+Kv78/gJCQEKlTEXWhGn2qI0eOALC1tRV5Qs6xY8ccHBzEnkpm8AYMGNC+fXuRy3zhGCvxe8rprp9++slw9rjSG0aMMZD/kMlkXl5eaWlpmzZtCgsLE/ld+fn5AOzs7KSMpicyMzOfeeYZc3NzkfNTp0799NNPhwwZItzE03WWlpZOTk5P/KZcLvfx8UlKSlq3bt3cuXO5BCP1QDVas9u3bw8ZMqS8vPz27duNGjXiHYcgKyvL2dnZ0tIyNzeXdxY16Nu379ixY6dNm/bP3/zggw/CwsLat2+fnJws/n8whDtT3gG0lEwmu3v3roWFRV5eXosWLXjHIbh3715FRQVjrH379sbGxrzjNAhj7NKlS2fPnnVxcRk8eLDwm3l5ecIzDJs2baIO1TF8rylos1dffRXAlClTeAchTKlU+vn5AViwYAHvLOoRHR2Nfx8I+s477wB44YUX+AYj9UA1+lT03In22L17N4AWLVqI2S1bJ1QfT79582bGWGZmppmZmampaVJSEu9oRGVUo7Whp6C1QUlJyXPPPQdg586dvLOo06FDhwDY2dkJj4IkJiZu2bKFdyhSH1SjtaF38rTB4sWLAXTt2lX/9i0eNmwYgJkzZ/IOQhqE7tTX4dNPP506daqTk9P169eFbTKIJt2/f9/d3b2srCwuLk64PKpPUlJSunTpolQqExMThcOliS7S7TueGjB58uTu3btnZGSsX7+edxZDFB4eXlpaOm7cOP3rUAAdO3Z8++23FQqF+GeTiRai1Wjdzp8/7+fnZ2FhkZqaKhwuRjTj119/7du3b+PGjVNTU4XLo/onPz/f1dU1Jyfn0KFDwqv3ROfQarRuvXv3DgwMLCsrE85lI5qhVCpDQ0MZYwsWLNDXDgVgZ2cnHFoXHh5eUVHBOw6pD1qNipKRkeHu7l5SUvLLL7/069ePdxyDsG3btmnTprVu3fr69euWlpa840hIoVD4+Phcu3YtOjpaOFya6BZajYri5OQkPPwUFhamVCp5x9F/hYWFwobN77//vn53KAATE5OYmBgAq1evfvjwIe84RGVUo2LNmzevTZs2iYmJO3fu5J1F/0VFRf311199+vQZPXo07yyaMGjQoICAgKKiokWLFvHOQlRGH+pVsHfv3rFjxzZv3jw9Pd3GxoZ3HL31559/enp6yuXy33//vVu3brzjaMitW7c6duxYWVkZHx8vHCBKdAWtRlUQFBTUt2/fR48erVmzhncWfRYaGiqTyUJCQgynQwG0a9dOuGQUFhZGixvdQqtR1SQmJvr6+pqaml67dk14J5qo18mTJ4cOHdq0adO0tLSWLVvyjqNRRUVFbm5uDx8+/PLLL4XDpYlOoNWoanx8fCZNmiSTyWhXXSnI5fLZs2cDWLZsmaF1KABra+tVq1YBiIyMLCkp4R2HiEU1qrK1a9fa2Nh89913P/zwA+8s+iY2NjY5OdnFxWXGjBm8s/AxadKkHj16PHjwYN26dbyzELHoQ319rFu3bt68eR4eHleuXKG98dUlOzvb1dX177//Pnbs2Msvv8w7Djfx8fF9+vSxsLBISUkRDpcmWo5Wo/URFhbm6uqampr68ccf886iP5YsWfL3338PHjzYkDsUQK9evYKCgsrKyuhRfF1Bq9F6Onz48PDhw+3s7NLT0x0cHHjH0XlXrlzp1q2bkZHR5cuXPT09ecfh7MGDB25ubiUlJT///LNwuDTRZrQaraeAgIBhw4bl5+cLL9uQBgoLC1MoFLNmzaIOBeDo6BgZGYn//7HwjkPqQKvR+ktNTfX29lYqlZcuXfLy8uIdR4ft378/MDDQ3t7+xo0b9vb2vONohbKyso4dO965c2f79u1Tp07lHYfUhlaj9efh4TFt2jSFQiE8o0Pqp7y8XFh5rVmzhjq0WuPGjYVj745t2YKCAt5xSG2oRhtk+fLlDg4Op0+fFs7VIfWwYcOGO3fueHp6TpkyhXcW7RIYGBg3efKhtDSsXMk7C6kNfahvqA8//HDWrFnt2rVLTk62sLDgHUfHPHjwwN3dvbi4+MSJE0OGDOEdR/tcvgxfXxgb49o1uLnxTkNqRqvRhpo+fXrnzp1v3bol7HVGVDJ//vzi4uLRo0dTh9asSxe8+SYqKxERwTsKeSpajarB6dOnX3jhBSsrq7S0tGeffZZ3HJ1x4cKF3r17m5ubp6SkODs7846jrR49gqsrCgrw/fd46SXeaUgNaDWqBoMGDRo+fHhxcTFtFikeY0w4IyQiIoI6tDbNm2PxYgAID0dlJe80pAa0GlWPW7dueXp6VlRUXLhwgTaLFGPXrl2TJk1ydHS8fv26lZUV7zjaTSaDlxfS0hATg9BQ3mnIk2g1qh7t2rUT1la0WaQYxcXFCxcuBBAdHU0dWjczM2zYAADLlyMnh3ca8iSqUbVZtGhRq1at4uPjv/rqK95ZtN2aNWsyMzN79uw5btw43ll0hL8/XnwR+flYupR3FPIk+lCvTjt37pw8ebKjo2NaWlqTJk14x9FS1RdA4uPjn3/+ed5xdEdqKry9oVQiIQHe3rzTkMdoNapOEydOFDaLfO+993hn0V4RERHl5eXBwcHUoarx8MA770ChAL01p2VoNapmwmaR5ubmqamptFnkf505c2bQoEH0cFg95efD1RU5Ofj2W4wcyTsNqUKrUTUTNossLy+nzSL/S6FQhIWFAVi4cCF1aH3Y2WH5cgCIiEB5Oe80pAqtRtWPNot8mq1bt86YMcPZ2TklJYVenK0nhQJdu+LqVaxejYULeachAK1GpUCbRdYoPz9/2bJlADZs2EAdWn8mJhBeO167FpmZvNMQgGpUInPnzm3btu3ly5d37NjBO4u2iIqKysnJGThw4Ei6qNdAAwdi5EgUF2PBAt5RCEAf6qXzv//9b8yYMc2aNUtPT7e1teUdhzPa4lrNbt9Gx46oqEB8POiBB95oNSqVwMDA/v37Z2dnCyePG7jw8PDKysq33nqLOlQ9nJ0xezYYQ1gYaCXEG61GJXT58mVfX19jY+Nr1665GfBmkUeOHHnttdfo+D81Ky6GmxsyM/HFF5gwgXcag0arUQl16dJl8uTJlZWVc+bM4Z2FG5lMFhERAWDZsmXUoepkZYU1awBgwQIUF/NOY9CoRqW1atUqW1vbY8eOHT9+nHcWPj744IP09HQPD4933nmHdxa9ExyMHj3w4AHorTmu6EO95N5///2IiAh3d/erV682atRIpe9NTk7Ozs6WKJiq2rZtq+p7WY8ePXJ1dS0oKDh+/PiLL74oTS7DduECeveGuTlSUkDbtvLCiMRkMplwYXTTpk2qfu+IESN4/wN5bPHixarmDwkJAeDv76/qNxIVjB/PADZ6NO8chotWo5pw9OjRV1991dbWNj09vVmzZuK/cenSpXFxcdIFU0lwcPDkyZPFzycmJnbv3t3ExOTq1auGfIdNcg8ewM0NJSU4fx69evFOY4ioRjXk5ZdfPn78+LRp0z766CPeWTSkf//+cXFxERER69ev551F38XGwtwcISEwMeEdxRBRjWrI9evXvby8lEplQkKCtwFsFrlv376goKDmzZunp6fb2NjwjkOIhKhGNWf27NkxMTF+fn5xcXFGRka840iorKzMw8Pj7t27n3zyiXB5lGhUWRl+/x2ZmSgqgo0NnnsOvr747+3NrCzcuwcAXl4wN6/5r5LLkZgIAI6OoE25nobvpVmDkp+fL1wY/eabb3hnkVZUVBQAHx8fuVzOO4uBSUlhr7/OLCwY8K9fVlZsyhR2796/hjdurPrT9PSn/oUPH1bNREVJnV130XOjmmNra7tixQoA4eHhpaWlvONIJSMjQ7gYGhMTY0KX6jRp9254e2P/fpSXw9wcXl4YMACdOsHEBMXF2LEDnp44cYJ3Sj1ENapRU6dO9fb2vnfv3qZNm3hnkUpkZGRJScmYMWP69evHO4shOXwYEyeishJ2dti6Fbm5uHIFZ87g2jU8eoQVK2BujqIi+Pvjt994Z9U3VKMaZWJiIhTomjVr7gmXpfRLfHz8vn37GjduHB0dzTuLIcnLQ0gIGIO9PeLiMH06/nmior09lizBd9/B1BSVlQgORmUlv6x6iGpU0wYOHDhq1KjS0tLFixfzzqJmSqUyNDSUMRYZGUnnUGnUZ59VnV+/fj06dap5ZuhQCHs7pKfj4EHNZTMAVKMcrF+/3sLCYs+ePefOneOdRZ0+//zzixcvOjk5zZ07l3cWA7NnDwA4OGD8+NrGQkNhavp4nqgJ1SgHzs7O4eHhjLGwsDClUsk7jnoUFRUJ6+t169Y1+ecnSiK1oiIkJQHAoEEwM6ttslUrdO0KAOfP0y6lakQ1yseiRYtat26dkJCwR1/WBatWrXr48GGvXr3eeOMN3lkMTHo6hCO/nvZx/p+EbbNzc6suAghyc5GVVfOvf46RpzDlHcBAWVparlq1auLEie++++62bdt4x2kouVyemJhobGwcGxur328WaKO8vKov7O3rHn7mmSe/C6A38RuIapSbCRMm3Lx58/Dhw+fPn+edRQ0CAgL69+/v6+vLO4jhqaio+qL2T/SC6reVysqkymN4qEa5MTIyWr58+ahRo4qKinhnUYMWLVq4uLjwTmGQqrcsKCmpe7j6H5ud3ePf/OMPtGtX8/yjR3B3b0g6Q0A1yhkd8UYaqnnzqi8yMuoevn8fAIyN8c8DXZo2/Ver/lP1Upc8Hd1iIkTHdegAa2sAuHSp7uGEBABwdwc9TaE+VKOE6DhjY/TtCwBnzyIrq7bJixdx+zYADByoiWAGg2qUEN331lsAIJdj9eraxlas+Nc8UROqUUJ0n79/1UNLW7bgs89qnlm6FEePAkBQEOiKvFpRjRKi+0xMsGsXmjWDUokpUzBqFE6cQEEBAOTm4vBhDBqElSsBoEMHbNnCN6z+oTv1hOiFDh1w7hyGD0dqKg4cwIEDNcz4+eHbb596U57UF61GCdEXrq64ehXbtmHAgH8dGWJpiZdewv79iIt7/HQUAGtrODnByamG80WqmZhUzdCBWk9HZzERoo9kMmRno7AQtrZo1qxqYyciDapRQghpEPpQTwghDUI1SgghDUI1SgghDUI1SgghDUI1SgghDfJ/805nGcU1ehIAAAC3elRYdHJka2l0UEtMIHJka2l0IDIwMjIuMDMuNQAAeJx7v2/tPQYg4GWAAEYg5oTiBkY2hwwgzcxMJEMDxGBhY4DQHBCaiUPBAkQzMnEzMGYwMTIlMDFnMDGzJLCwZjCxsimwsWswsXEosDIkiDCyMbCyMDMxipdBXQIGnKGhV/c9dFu2H8QJDf26H8ZevUrrANCVqkji9hA2WL09RM0qOwaGA0sh7FdAsYalEDWqDgj1YDbYTDEAkP8v218XUVIAAADyelRYdE1PTCByZGtpdCAyMDIyLjAzLjUAAHichZLbDoIwDEDf9xX9AZfuwqCPcokxBkgU/Qff/f/YYrAQ42hpso7TrZcZELm2l+cLvuJbYwAw8xERPAIimh5kAXV3Og/QTMd62WnG+zDdgFhRdEsep7Ffdhw0cEAbXUqphIOznghDBWhxFo31QjpL+2QQ0tuUZlL//4Bxc2TmxGKTZQZMDKINs0jE36tLBp2t9sEKRvC2mMnczbTmct3phnYzgc9M6nFodSaRzWvjI1vQ7kYx7aFooZ1iB5L2w7GVWrVnq7Q2xy5pCVEC1omu0xJ/eWS8Nm+CaoPjrV8lQQAAAHN6VFh0U01JTEVTIHJka2l0IDIwMjIuMDMuNQAAeJxVjFEOgCAMQ6/iJyRj2RhOCeHLA3AIrsHhFRNA+9e+tiVfptjKtYu3Zjzup4gAo4+RAiTG7gUI0mBuQkKRQR1hYFU91vYpRv4nHvXt0Ieuv/UxM9tuW2ciHfaelrkAAAAASUVORK5CYII=",
+                        "image/png": "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\n",
                         "text/plain": [
-                            "<rdkit.Chem.rdchem.Mol at 0x7fa7325a8b20>"
+                            "<rdkit.Chem.rdchem.Mol at 0x7f9f74e5bca0>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "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\n",
                         "text/plain": [
-                            "<rdkit.Chem.rdchem.Mol at 0x7fa7325a8c40>"
+                            "<rdkit.Chem.rdchem.Mol at 0x7f9f74e5bd10>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "smiles_strings = ('c1ccccc1C(=O)[OH]','c1ccccc1C(=O)[O-].[Na+]','CC[NH+](C)C','CC[N+](C)(C)C',\n",
                 "       '[O-]CC(C(=O)[O-])C[NH+](C)C','[O-]CC(C(=O)[O-])C[N+](C)(C)C')\n",
                 "\n",
-                "smi2mol = SmilesToMol()\n",
+                "smi2mol = SmilesToMolTransformer()\n",
                 "\n",
                 "mols  = smi2mol.transform(smiles_strings)\n",
                 "for mol in mols[0:2]:\n",
                 "    display(mol)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "e68b0eff",
             "metadata": {},
             "source": [
                 "We can simply use the transformer directly and get a list of standardized molecules"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
+            "id": "c18bbd3e",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:27.023486Z",
-                    "iopub.status.busy": "2022-12-09T17:05:27.022727Z",
-                    "iopub.status.idle": "2022-12-09T17:05:27.026315Z",
-                    "shell.execute_reply": "2022-12-09T17:05:27.026695Z"
+                    "iopub.execute_input": "2023-03-19T08:54:31.679653Z",
+                    "iopub.status.busy": "2023-03-19T08:54:31.679396Z",
+                    "iopub.status.idle": "2023-03-19T08:54:31.695079Z",
+                    "shell.execute_reply": "2023-03-19T08:54:31.694415Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "['O=C(O)c1ccccc1',\n",
                             " 'O=C(O)c1ccccc1',\n",
                             " 'CCN(C)C',\n",
                             " 'CC[N+](C)(C)C',\n",
                             " 'CN(C)CC(CO)C(=O)O',\n",
                             " 'C[N+](C)(C)CC(CO)C(=O)[O-]']"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# You can just run straight up like this. Note that neutralising is optional\n",
                 "standardizer = Standardizer(neutralize=True)\n",
                 "standard_mols = standardizer.transform(mols)\n",
                 "standard_smiles = smi2mol.inverse_transform(standard_mols)\n",
                 "standard_smiles"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "da3fc3e2",
             "metadata": {},
             "source": [
                 "Some of the molecules were desalted and neutralized.\n",
                 "\n",
                 "A typical usecase would be to add the standardizer to a pipeline for prediction"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
+            "id": "d03be7dc",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:27.044133Z",
-                    "iopub.status.busy": "2022-12-09T17:05:27.043311Z",
-                    "iopub.status.idle": "2022-12-09T17:05:27.095856Z",
-                    "shell.execute_reply": "2022-12-09T17:05:27.096335Z"
+                    "iopub.execute_input": "2023-03-19T08:54:31.697750Z",
+                    "iopub.status.busy": "2023-03-19T08:54:31.697437Z",
+                    "iopub.status.idle": "2023-03-19T08:54:31.754193Z",
+                    "shell.execute_reply": "2023-03-19T08:54:31.753035Z"
                 },
                 "lines_to_next_cell": 2
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -153,46 +162,48 @@
                     ]
                 }
             ],
             "source": [
                 "# Typical use case is to use it in an sklearn pipeline, like below \n",
                 "predictor = Ridge()\n",
                 "\n",
-                "std_pipe = make_pipeline(SmilesToMol(), Standardizer(), MorganTransformer(useCounts=True), predictor)\n",
-                "nonstd_pipe = make_pipeline(SmilesToMol(), MorganTransformer(useCounts=True), predictor)\n",
+                "std_pipe = make_pipeline(SmilesToMolTransformer(), Standardizer(), MorganFingerprintTransformer(useCounts=True), predictor)\n",
+                "nonstd_pipe = make_pipeline(SmilesToMolTransformer(), MorganFingerprintTransformer(useCounts=True), predictor)\n",
                 "\n",
                 "fake_y = range(len(smiles_strings))\n",
                 "\n",
                 "std_pipe.fit(smiles_strings, fake_y)\n",
                 "\n",
                 "\n",
                 "print(f'Predictions with no standardization: {std_pipe.predict(smiles_strings)}')\n",
                 "print(f'Predictions with standardization:    {nonstd_pipe.predict(smiles_strings)}')"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "9cfab56c",
             "metadata": {},
             "source": [
                 "As we can see, the predictions with the standardizer and without are different. The two first molecules were benzoic acid and sodium benzoate, which with the standardized pipeline is predicted as the same, but differently with the nonstandardized pipeline. Wheter we want to make the prediction on the parent compound, or predict the exact form, will of course depend on the use-case, but now there is at least a way to handle it easily in pipelined predictors.\n",
                 "\n",
                 "The example also demonstrate another feature. We created the ridge regressor before creating the two pipelines. Fitting one of the pipelines thus also updated the object in the other pipeline. This can be useful for building inference pipelines that takes in SMILES molecules, but rather do the fitting on already converted and standardized molecules. However, be aware that the crossvalidation classes of scikit-learn may clone the estimators internally when doing the search loop, which would break this interdependence, and necessitate the rebuilding of the inference pipeline.\n",
                 "\n",
                 "If we had fitted the non standardizing pipeline, the model would have been different as shown below, as some of the molecules would be perceived different by the Ridge regressor."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
+            "id": "e5f8495f",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:27.103670Z",
-                    "iopub.status.busy": "2022-12-09T17:05:27.103127Z",
-                    "iopub.status.idle": "2022-12-09T17:05:27.127113Z",
-                    "shell.execute_reply": "2022-12-09T17:05:27.126580Z"
+                    "iopub.execute_input": "2023-03-19T08:54:31.760234Z",
+                    "iopub.status.busy": "2023-03-19T08:54:31.759681Z",
+                    "iopub.status.idle": "2023-03-19T08:54:31.800782Z",
+                    "shell.execute_reply": "2023-03-19T08:54:31.799781Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -224,18 +235,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.4"
-        },
-        "vscode": {
-            "interpreter": {
-                "hash": "dc6218d6ccd9a44863300cd5111a59d6c18db4de812eb936d6a68ad5fa5cf18f"
-            }
+            "version": "3.10.9"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 5
 }
```

### Comparing `scikit_mol-0.1.2/notebooks/04_standardizer.py` & `scikit_mol-0.2.0/notebooks/04_standardizer.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,40 +3,41 @@
 #   jupytext:
 #     cell_metadata_filter: -all
 #     formats: ipynb,py:percent
 #     text_representation:
 #       extension: .py
 #       format_name: percent
 #       format_version: '1.3'
-#       jupytext_version: 1.14.1
+#       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3.9.4 ('rdkit')
 #     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
 # # Molecule standardization
 # When building machine learning models of molecules, it is important to standardize the molecules. We often don't want different predictions just because things are drawn in slightly different forms, such as protonated or deprotanted carboxylic acids. Scikit-mol provides a very basic standardize transformer based on the molvs implementation in RDKit
 
 # %%
 from rdkit import Chem
 from scikit_mol.standardizer import Standardizer
-from scikit_mol.transformers import MorganTransformer, SmilesToMol
+from scikit_mol.fingerprints import MorganFingerprintTransformer
+from scikit_mol.conversions import SmilesToMolTransformer
 from sklearn.pipeline import make_pipeline
 from sklearn.linear_model import Ridge
 
 # %% [markdown]
 # For demonstration let's create some molecules with different protonation states. The two first molecules are Benzoic acid and Sodium benzoate.
 
 # %%
 smiles_strings = ('c1ccccc1C(=O)[OH]','c1ccccc1C(=O)[O-].[Na+]','CC[NH+](C)C','CC[N+](C)(C)C',
        '[O-]CC(C(=O)[O-])C[NH+](C)C','[O-]CC(C(=O)[O-])C[N+](C)(C)C')
 
-smi2mol = SmilesToMol()
+smi2mol = SmilesToMolTransformer()
 
 mols  = smi2mol.transform(smiles_strings)
 for mol in mols[0:2]:
     display(mol)
 
 # %% [markdown]
 # We can simply use the transformer directly and get a list of standardized molecules
@@ -53,16 +54,16 @@
 #
 # A typical usecase would be to add the standardizer to a pipeline for prediction
 
 # %%
 # Typical use case is to use it in an sklearn pipeline, like below 
 predictor = Ridge()
 
-std_pipe = make_pipeline(SmilesToMol(), Standardizer(), MorganTransformer(useCounts=True), predictor)
-nonstd_pipe = make_pipeline(SmilesToMol(), MorganTransformer(useCounts=True), predictor)
+std_pipe = make_pipeline(SmilesToMolTransformer(), Standardizer(), MorganFingerprintTransformer(useCounts=True), predictor)
+nonstd_pipe = make_pipeline(SmilesToMolTransformer(), MorganFingerprintTransformer(useCounts=True), predictor)
 
 fake_y = range(len(smiles_strings))
 
 std_pipe.fit(smiles_strings, fake_y)
 
 
 print(f'Predictions with no standardization: {std_pipe.predict(smiles_strings)}')
```

### Comparing `scikit_mol-0.1.2/notebooks/04_standardizer_files/04_standardizer_3_0.png` & `scikit_mol-0.2.0/notebooks/04_standardizer_files/04_standardizer_3_0.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/04_standardizer_files/04_standardizer_3_1.png` & `scikit_mol-0.2.0/notebooks/04_standardizer_files/04_standardizer_3_1.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/05_smiles_sanitaztion.ipynb` & `scikit_mol-0.2.0/notebooks/05_smiles_sanitaztion.ipynb`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8150166095478596%*

 * *Differences: {"'cells'": "{0: {'id': 'b6fe4dbd'}, 1: {'metadata': {'execution': {'iopub.execute_input': "*

 * *            "'2023-03-19T08:54:33.431115Z', 'iopub.status.busy': '2023-03-19T08:54:33.430360Z', "*

 * *            "'iopub.status.idle': '2023-03-19T08:54:33.801123Z', 'shell.execute_reply': "*

 * *            "'2023-03-19T08:54:33.800330Z'}}, 'id': 'c46f479f'}, 2: {'id': '5db46e76'}, 3: "*

 * *            "{'metadata': {'execution': {'iopub.execute_input': '2023-03-19T08:54:33.804206Z', "*

 * *            "'iopub.status.busy': '2023-0 […]*

```diff
@@ -1,70 +1,75 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
+            "id": "b6fe4dbd",
             "metadata": {},
             "source": [
                 "# SMILES sanitation\n",
                 "Sometimes we are faced with datasets which has SMILES that rdkit doesn't want to sanitize. This can be human entry errors, or differences between RDKits more strict sanitazion and other toolkits implementations of the parser. e.g. RDKit will not handle a tetravalent nitrogen when it has no charge, where other toolkits may simply build the graph anyway, disregarding the issues with the valence rules or guessing that the nitrogen should have a charge, where it could also by accident instead have a methyl group too many."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
+            "id": "c46f479f",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:29.189828Z",
-                    "iopub.status.busy": "2022-12-09T17:05:29.189136Z",
-                    "iopub.status.idle": "2022-12-09T17:05:29.523835Z",
-                    "shell.execute_reply": "2022-12-09T17:05:29.523297Z"
+                    "iopub.execute_input": "2023-03-19T08:54:33.431115Z",
+                    "iopub.status.busy": "2023-03-19T08:54:33.430360Z",
+                    "iopub.status.idle": "2023-03-19T08:54:33.801123Z",
+                    "shell.execute_reply": "2023-03-19T08:54:33.800330Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
                 "from rdkit.Chem import PandasTools\n",
                 "\n",
                 "csv_file = \"../tests/data/SLC6A4_active_excapedb_subset.csv\" # Hmm, maybe better to download directly\n",
                 "data = pd.read_csv(csv_file)\n",
                 "\n"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "5db46e76",
             "metadata": {},
             "source": [
                 "Now, this example dataset contain all sanitizable SMILES, so for demonstration purposes, we will corrupt one of them"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
+            "id": "a7bc5ff6",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:29.530812Z",
-                    "iopub.status.busy": "2022-12-09T17:05:29.530234Z",
-                    "iopub.status.idle": "2022-12-09T17:05:29.532348Z",
-                    "shell.execute_reply": "2022-12-09T17:05:29.531954Z"
+                    "iopub.execute_input": "2023-03-19T08:54:33.804206Z",
+                    "iopub.status.busy": "2023-03-19T08:54:33.803981Z",
+                    "iopub.status.idle": "2023-03-19T08:54:33.807721Z",
+                    "shell.execute_reply": "2023-03-19T08:54:33.807162Z"
                 }
             },
             "outputs": [],
             "source": [
                 "data.loc[1,'SMILES'] = 'CN(C)(C)(C)'"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
+            "id": "a792f370",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:29.575406Z",
-                    "iopub.status.busy": "2022-12-09T17:05:29.574704Z",
-                    "iopub.status.idle": "2022-12-09T17:05:29.579466Z",
-                    "shell.execute_reply": "2022-12-09T17:05:29.578643Z"
+                    "iopub.execute_input": "2023-03-19T08:54:33.810589Z",
+                    "iopub.status.busy": "2023-03-19T08:54:33.810336Z",
+                    "iopub.status.idle": "2023-03-19T08:54:33.849855Z",
+                    "shell.execute_reply": "2023-03-19T08:54:33.849118Z"
                 },
                 "lines_to_next_cell": 2
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -72,81 +77,85 @@
                         "Dataset contains 1 unparsable mols\n"
                     ]
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "[18:05:29] Explicit valence for atom # 1 N, 4, is greater than permitted\n"
+                        "[09:54:33] Explicit valence for atom # 1 N, 4, is greater than permitted\n"
                     ]
                 }
             ],
             "source": [
                 "\n",
                 "PandasTools.AddMoleculeColumnToFrame(data, smilesCol=\"SMILES\")\n",
                 "print(f'Dataset contains {data.ROMol.isna().sum()} unparsable mols')"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "54341ece",
             "metadata": {},
             "source": [
                 "If we use these SMILES for the scikit-learn pipeline, we would face an error, so we need to check and clean the dataset first. The CheckSmilesSanitation can help us with that."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
+            "id": "849b643f",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:29.584682Z",
-                    "iopub.status.busy": "2022-12-09T17:05:29.583849Z",
-                    "iopub.status.idle": "2022-12-09T17:05:29.635089Z",
-                    "shell.execute_reply": "2022-12-09T17:05:29.635453Z"
+                    "iopub.execute_input": "2023-03-19T08:54:33.852625Z",
+                    "iopub.status.busy": "2023-03-19T08:54:33.852342Z",
+                    "iopub.status.idle": "2023-03-19T08:54:33.894579Z",
+                    "shell.execute_reply": "2023-03-19T08:54:33.893765Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Error in parsing 1 SMILES. Unparsable SMILES can be found in self.errors\n"
                     ]
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "[18:05:29] Explicit valence for atom # 1 N, 4, is greater than permitted\n"
+                        "[09:54:33] Explicit valence for atom # 1 N, 4, is greater than permitted\n"
                     ]
                 }
             ],
             "source": [
-                "from scikit_mol.sanitizer import CheckSmilesSanitazion\n",
+                "from scikit_mol.utilities import CheckSmilesSanitazion\n",
                 "smileschecker = CheckSmilesSanitazion()\n",
                 "\n",
                 "smiles_list_valid, y_valid, smiles_errors, y_errors = smileschecker.sanitize(list(data.SMILES), list(data.pXC50))"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "5e410e4c",
             "metadata": {},
             "source": [
                 "Now the smiles_list_valid should be all valid and the y_values filtered as well. Errors are returned, but also accesible after the call to .sanitize() in the .errors property"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
+            "id": "2145530c",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:29.644439Z",
-                    "iopub.status.busy": "2022-12-09T17:05:29.643862Z",
-                    "iopub.status.idle": "2022-12-09T17:05:29.695395Z",
-                    "shell.execute_reply": "2022-12-09T17:05:29.694961Z"
+                    "iopub.execute_input": "2023-03-19T08:54:33.897271Z",
+                    "iopub.status.busy": "2023-03-19T08:54:33.896965Z",
+                    "iopub.status.idle": "2023-03-19T08:54:33.910201Z",
+                    "shell.execute_reply": "2023-03-19T08:54:33.909540Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -182,54 +191,56 @@
                             "</div>"
                         ],
                         "text/plain": [
                             "        SMILES        y\n",
                             "0  CN(C)(C)(C)  7.18046"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "smileschecker.errors"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "c9906a45",
             "metadata": {},
             "source": [
                 "The checker can also be used only on X"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
+            "id": "d5fd425e",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:29.739932Z",
-                    "iopub.status.busy": "2022-12-09T17:05:29.735518Z",
-                    "iopub.status.idle": "2022-12-09T17:05:29.745144Z",
-                    "shell.execute_reply": "2022-12-09T17:05:29.745544Z"
+                    "iopub.execute_input": "2023-03-19T08:54:33.913053Z",
+                    "iopub.status.busy": "2023-03-19T08:54:33.912806Z",
+                    "iopub.status.idle": "2023-03-19T08:54:33.956093Z",
+                    "shell.execute_reply": "2023-03-19T08:54:33.955470Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Error in parsing 1 SMILES. Unparsable SMILES can be found in self.errors\n"
                     ]
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "[18:05:29] Explicit valence for atom # 1 N, 4, is greater than permitted\n"
+                        "[09:54:33] Explicit valence for atom # 1 N, 4, is greater than permitted\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -262,15 +273,15 @@
                             "</div>"
                         ],
                         "text/plain": [
                             "        SMILES\n",
                             "0  CN(C)(C)(C)"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "smiles_list_valid, X_errors = smileschecker.sanitize(list(data.SMILES))\n",
                 "smileschecker.errors"
@@ -292,18 +303,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.4"
-        },
-        "vscode": {
-            "interpreter": {
-                "hash": "dc6218d6ccd9a44863300cd5111a59d6c18db4de812eb936d6a68ad5fa5cf18f"
-            }
+            "version": "3.10.9"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 5
 }
```

### Comparing `scikit_mol-0.1.2/notebooks/05_smiles_sanitaztion.py` & `scikit_mol-0.2.0/notebooks/05_smiles_sanitaztion.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # jupyter:
 #   jupytext:
 #     formats: ipynb,py:percent
 #     text_representation:
 #       extension: .py
 #       format_name: percent
 #       format_version: '1.3'
-#       jupytext_version: 1.14.1
+#       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3.9.4 ('rdkit')
 #     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
@@ -38,15 +38,15 @@
 print(f'Dataset contains {data.ROMol.isna().sum()} unparsable mols')
 
 
 # %% [markdown]
 # If we use these SMILES for the scikit-learn pipeline, we would face an error, so we need to check and clean the dataset first. The CheckSmilesSanitation can help us with that.
 
 # %%
-from scikit_mol.sanitizer import CheckSmilesSanitazion
+from scikit_mol.utilities import CheckSmilesSanitazion
 smileschecker = CheckSmilesSanitazion()
 
 smiles_list_valid, y_valid, smiles_errors, y_errors = smileschecker.sanitize(list(data.SMILES), list(data.pXC50))
 
 # %% [markdown]
 # Now the smiles_list_valid should be all valid and the y_values filtered as well. Errors are returned, but also accesible after the call to .sanitize() in the .errors property
```

### Comparing `scikit_mol-0.1.2/notebooks/06_hyperparameter_tuning.ipynb` & `scikit_mol-0.2.0/notebooks/06_hyperparameter_tuning.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.814665660824515%*

 * *Differences: {"'cells'": "{0: {'id': '9d600dd1'}, 1: {'metadata': {'execution': {'iopub.execute_input': "*

 * *            "'2023-03-19T08:54:35.701525Z', 'iopub.status.busy': '2023-03-19T08:54:35.700822Z', "*

 * *            "'iopub.status.idle': '2023-03-19T08:54:37.014139Z', 'shell.execute_reply': "*

 * *            "'2023-03-19T08:54:37.013259Z'}}, 'source': {insert: [(11, 'from "*

 * *            "scikit_mol.fingerprints import MorganFingerprintTransformer\\n'), (12, 'from "*

 * *            "scikit_mol.conversions import SmilesToMolTransf […]*

```diff
@@ -1,27 +1,29 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
+            "id": "9d600dd1",
             "metadata": {},
             "source": [
                 "# Full example: Hyperparameter tuning\n",
                 "\n",
                 "first some imports of the usual suspects: RDKit, pandas, matplotlib, numpy and sklearn. New kid on the block is scikit-mol"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
+            "id": "7df4793c",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:31.106942Z",
-                    "iopub.status.busy": "2022-12-09T17:05:31.106378Z",
-                    "iopub.status.idle": "2022-12-09T17:05:31.975903Z",
-                    "shell.execute_reply": "2022-12-09T17:05:31.975423Z"
+                    "iopub.execute_input": "2023-03-19T08:54:35.701525Z",
+                    "iopub.status.busy": "2023-03-19T08:54:35.700822Z",
+                    "iopub.status.idle": "2023-03-19T08:54:37.014139Z",
+                    "shell.execute_reply": "2023-03-19T08:54:37.013259Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "import rdkit\n",
                 "from rdkit import Chem\n",
@@ -29,33 +31,36 @@
                 "import pandas as pd\n",
                 "import matplotlib.pyplot as plt\n",
                 "from time import time\n",
                 "import numpy as np\n",
                 "from sklearn.pipeline import Pipeline, make_pipeline\n",
                 "from sklearn.linear_model import Ridge\n",
                 "from sklearn.model_selection import train_test_split\n",
-                "from scikit_mol.transformers import MorganTransformer, SmilesToMol"
+                "from scikit_mol.fingerprints import MorganFingerprintTransformer\n",
+                "from scikit_mol.conversions import SmilesToMolTransformer"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "8acee1c3",
             "metadata": {},
             "source": [
                 "We will need some data. There is a dataset with the SLC6A4 active compounds from ExcapeDB on Zenodo. The scikit-mol project uses a subset of this for testing, and the samples there has been specially selected to give good results in testing (it should therefore be used for any production modelling). If full_set is false, the fast subset will be used, and otherwise the full dataset will be downloaded if needed."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
+            "id": "45a8ebf1",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:31.980867Z",
-                    "iopub.status.busy": "2022-12-09T17:05:31.980341Z",
-                    "iopub.status.idle": "2022-12-09T17:05:31.981907Z",
-                    "shell.execute_reply": "2022-12-09T17:05:31.982294Z"
+                    "iopub.execute_input": "2023-03-19T08:54:37.017824Z",
+                    "iopub.status.busy": "2023-03-19T08:54:37.017350Z",
+                    "iopub.status.idle": "2023-03-19T08:54:37.022818Z",
+                    "shell.execute_reply": "2023-03-19T08:54:37.022080Z"
                 }
             },
             "outputs": [],
             "source": [
                 "full_set = False\n",
                 "\n",
                 "if full_set:\n",
@@ -66,28 +71,30 @@
                 "        urllib.request.urlretrieve(url, csv_file)\n",
                 "else:\n",
                 "    csv_file = '../tests/data/SLC6A4_active_excapedb_subset.csv'"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "f3c108d4",
             "metadata": {},
             "source": [
                 "The CSV data is loaded into a Pandas dataframe and the PandasTools utility from RDKit is used to add a column with RDKit molecules"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
+            "id": "08c233a7",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:31.986793Z",
-                    "iopub.status.busy": "2022-12-09T17:05:31.986251Z",
-                    "iopub.status.idle": "2022-12-09T17:05:32.027801Z",
-                    "shell.execute_reply": "2022-12-09T17:05:32.027264Z"
+                    "iopub.execute_input": "2023-03-19T08:54:37.025520Z",
+                    "iopub.status.busy": "2023-03-19T08:54:37.025310Z",
+                    "iopub.status.idle": "2023-03-19T08:54:37.077231Z",
+                    "shell.execute_reply": "2023-03-19T08:54:37.076469Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -101,53 +108,57 @@
                 "\n",
                 "PandasTools.AddMoleculeColumnToFrame(data, smilesCol=\"SMILES\")\n",
                 "print(f\"{data.ROMol.isna().sum()} out of {len(data)} SMILES failed in conversion\")"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "e1828bee",
             "metadata": {},
             "source": [
                 "We use the train_test_split to, well, split the dataframe's molecule columns and pXC50 column into lists for train and testing"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
+            "id": "5363d05a",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:32.033376Z",
-                    "iopub.status.busy": "2022-12-09T17:05:32.032767Z",
-                    "iopub.status.idle": "2022-12-09T17:05:32.035287Z",
-                    "shell.execute_reply": "2022-12-09T17:05:32.034690Z"
+                    "iopub.execute_input": "2023-03-19T08:54:37.080021Z",
+                    "iopub.status.busy": "2023-03-19T08:54:37.079756Z",
+                    "iopub.status.idle": "2023-03-19T08:54:37.084574Z",
+                    "shell.execute_reply": "2023-03-19T08:54:37.084021Z"
                 },
                 "lines_to_next_cell": 2
             },
             "outputs": [],
             "source": [
                 "\n",
                 "mol_list_train, mol_list_test, y_train, y_test = train_test_split(data.ROMol, data.pXC50, random_state=0)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "bf9e8c8d",
             "metadata": {},
             "source": [
                 "We will standardize the molecules before modelling. This is best done before the hyperparameter optimizatiion of the featurization with the scikit-mol transformer and regression modelling, as the standardization is otherwise done for every loop in the hyperparameter optimization, which will make it take longer time."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
+            "id": "885daf12",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:32.039664Z",
-                    "iopub.status.busy": "2022-12-09T17:05:32.039160Z",
-                    "iopub.status.idle": "2022-12-09T17:05:32.440152Z",
-                    "shell.execute_reply": "2022-12-09T17:05:32.440660Z"
+                    "iopub.execute_input": "2023-03-19T08:54:37.087530Z",
+                    "iopub.status.busy": "2023-03-19T08:54:37.087275Z",
+                    "iopub.status.idle": "2023-03-19T08:54:37.454935Z",
+                    "shell.execute_reply": "2023-03-19T08:54:37.454153Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# Probably the recommended way would be to prestandardize the data if there's no changes to the transformer, \n",
                 "# and then add the standardizer in the inference pipeline.\n",
                 "\n",
@@ -155,117 +166,125 @@
                 "\n",
                 "standardizer = Standardizer()\n",
                 "mol_list_std_train = standardizer.transform(mol_list_train)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "a81ae4c4",
             "metadata": {},
             "source": [
                 "A simple pipeline with a MorganTransformer and a Ridge() regression for demonstration."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
+            "id": "8fd14250",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:32.444639Z",
-                    "iopub.status.busy": "2022-12-09T17:05:32.444166Z",
-                    "iopub.status.idle": "2022-12-09T17:05:32.446316Z",
-                    "shell.execute_reply": "2022-12-09T17:05:32.445873Z"
+                    "iopub.execute_input": "2023-03-19T08:54:37.458340Z",
+                    "iopub.status.busy": "2023-03-19T08:54:37.458092Z",
+                    "iopub.status.idle": "2023-03-19T08:54:37.461663Z",
+                    "shell.execute_reply": "2023-03-19T08:54:37.461052Z"
                 }
             },
             "outputs": [],
             "source": [
                 "\n",
-                "moltransformer = MorganTransformer()\n",
+                "moltransformer = MorganFingerprintTransformer()\n",
                 "regressor = Ridge()\n",
                 "\n",
                 "optimization_pipe = make_pipeline(moltransformer, regressor)\n",
                 "\n"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "ad2752d0",
             "metadata": {},
             "source": [
                 "For hyperparameter optimization we import the RandomizedSearchCV class from Scikit-Learn. It will try different random combinations of settings and use internal cross-validation to find the best model. In the end, it will fit the best found parameters on the full set. We also import loguniform, to get a better sampling of some of the parameters."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
+            "id": "fa082078",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:32.449590Z",
-                    "iopub.status.busy": "2022-12-09T17:05:32.449101Z",
-                    "iopub.status.idle": "2022-12-09T17:05:32.451169Z",
-                    "shell.execute_reply": "2022-12-09T17:05:32.450726Z"
+                    "iopub.execute_input": "2023-03-19T08:54:37.464188Z",
+                    "iopub.status.busy": "2023-03-19T08:54:37.463905Z",
+                    "iopub.status.idle": "2023-03-19T08:54:37.467187Z",
+                    "shell.execute_reply": "2023-03-19T08:54:37.466548Z"
                 },
                 "title": "Now hyperparameter tuning"
             },
             "outputs": [],
             "source": [
                 "from sklearn.model_selection import RandomizedSearchCV\n",
                 "from sklearn.utils.fixes import loguniform"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "fa2a316a",
             "metadata": {},
             "source": [
                 "With the pipelines, getting the names of the parameters to tune is a bit more tricky, as they are concatenations of the name of the step and the parameter with double underscores in between. We can get the available parameters from the pipeline with the get_params() method, and select the parameters we want to change from there."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
+            "id": "046e24d3",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:32.456332Z",
-                    "iopub.status.busy": "2022-12-09T17:05:32.455672Z",
-                    "iopub.status.idle": "2022-12-09T17:05:32.458577Z",
-                    "shell.execute_reply": "2022-12-09T17:05:32.458136Z"
+                    "iopub.execute_input": "2023-03-19T08:54:37.470133Z",
+                    "iopub.status.busy": "2023-03-19T08:54:37.469879Z",
+                    "iopub.status.idle": "2023-03-19T08:54:37.476370Z",
+                    "shell.execute_reply": "2023-03-19T08:54:37.475763Z"
                 },
                 "title": "Which keys do we have?"
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "dict_keys(['memory', 'steps', 'verbose', 'morgantransformer', 'ridge', 'morgantransformer__nBits', 'morgantransformer__radius', 'morgantransformer__useBondTypes', 'morgantransformer__useChirality', 'morgantransformer__useCounts', 'morgantransformer__useFeatures', 'ridge__alpha', 'ridge__copy_X', 'ridge__fit_intercept', 'ridge__max_iter', 'ridge__normalize', 'ridge__positive', 'ridge__random_state', 'ridge__solver', 'ridge__tol'])"
+                            "dict_keys(['memory', 'steps', 'verbose', 'morgantransformer', 'ridge', 'morgantransformer__nBits', 'morgantransformer__parallel', 'morgantransformer__radius', 'morgantransformer__useBondTypes', 'morgantransformer__useChirality', 'morgantransformer__useCounts', 'morgantransformer__useFeatures', 'ridge__alpha', 'ridge__copy_X', 'ridge__fit_intercept', 'ridge__max_iter', 'ridge__positive', 'ridge__random_state', 'ridge__solver', 'ridge__tol'])"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "\n",
                 "optimization_pipe.get_params().keys()"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "cd7c2297",
             "metadata": {},
             "source": [
                 "We will tune the regularization strength of the Ridge regressor, and try out different parameters for the Morgan fingerprint, namely the number of bits, the radius of the fingerprint, wheter to use counts or bits and features."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
+            "id": "cf2c45d7",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:32.463967Z",
-                    "iopub.status.busy": "2022-12-09T17:05:32.462972Z",
-                    "iopub.status.idle": "2022-12-09T17:05:32.465028Z",
-                    "shell.execute_reply": "2022-12-09T17:05:32.464632Z"
+                    "iopub.execute_input": "2023-03-19T08:54:37.478959Z",
+                    "iopub.status.busy": "2023-03-19T08:54:37.478683Z",
+                    "iopub.status.idle": "2023-03-19T08:54:37.483305Z",
+                    "shell.execute_reply": "2023-03-19T08:54:37.482688Z"
                 },
                 "lines_to_next_cell": 1
             },
             "outputs": [],
             "source": [
                 "\n",
                 "param_dist = {'ridge__alpha': loguniform(1e-2, 1e3),\n",
@@ -273,28 +292,30 @@
                 "            'morgantransformer__radius':[1,2,3,4],\n",
                 "            'morgantransformer__useCounts': [True,False],\n",
                 "            'morgantransformer__useFeatures':[True,False]}"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "d61fc18c",
             "metadata": {},
             "source": [
                 "The report function was taken from [this example](https://scikit-learn.org/stable/auto_examples/model_selection/plot_randomized_search.html#sphx-glr-auto-examples-model-selection-plot-randomized-search-py) from the scikit learn documentation."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
+            "id": "fbb2cacd",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:32.470321Z",
-                    "iopub.status.busy": "2022-12-09T17:05:32.469658Z",
-                    "iopub.status.idle": "2022-12-09T17:05:32.472516Z",
-                    "shell.execute_reply": "2022-12-09T17:05:32.472910Z"
+                    "iopub.execute_input": "2023-03-19T08:54:37.485906Z",
+                    "iopub.status.busy": "2023-03-19T08:54:37.485645Z",
+                    "iopub.status.idle": "2023-03-19T08:54:37.489973Z",
+                    "shell.execute_reply": "2023-03-19T08:54:37.489382Z"
                 },
                 "title": "From https://scikit-learn.org/stable/auto_examples/model_selection/plot_randomized_search.html#sphx-glr-auto-examples-model-selection-plot-randomized-search-py"
             },
             "outputs": [],
             "source": [
                 "# Utility function to report best scores\n",
                 "def report(results, n_top=3):\n",
@@ -310,36 +331,38 @@
                 "            )\n",
                 "            print(\"Parameters: {0}\".format(results[\"params\"][candidate]))\n",
                 "            print(\"\")"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "ad49376f",
             "metadata": {},
             "source": [
                 "We will do 25 tries of random parameter sets, and see what comes out as the best one. If you are using the small example dataset, this should take some second, but may take some minutes with the full set."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
+            "id": "bc66efa3",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:32.481672Z",
-                    "iopub.status.busy": "2022-12-09T17:05:32.479533Z",
-                    "iopub.status.idle": "2022-12-09T17:05:35.991730Z",
-                    "shell.execute_reply": "2022-12-09T17:05:35.991275Z"
+                    "iopub.execute_input": "2023-03-19T08:54:37.492677Z",
+                    "iopub.status.busy": "2023-03-19T08:54:37.492327Z",
+                    "iopub.status.idle": "2023-03-19T08:54:44.019837Z",
+                    "shell.execute_reply": "2023-03-19T08:54:44.018820Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Runtime: 3.51 for 25 iterations)\n"
+                        "Runtime: 6.52 for 25 iterations)\n"
                     ]
                 }
             ],
             "source": [
                 "n_iter_search = 25\n",
                 "random_search = RandomizedSearchCV(\n",
                 "    optimization_pipe, param_distributions=param_dist, n_iter=n_iter_search, cv=3\n",
@@ -350,150 +373,152 @@
                 "\n",
                 "print(f'Runtime: {t1-t0:0.2F} for {n_iter_search} iterations)')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
+            "id": "b2b3d623",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:35.996322Z",
-                    "iopub.status.busy": "2022-12-09T17:05:35.995574Z",
-                    "iopub.status.idle": "2022-12-09T17:05:35.999486Z",
-                    "shell.execute_reply": "2022-12-09T17:05:35.999098Z"
+                    "iopub.execute_input": "2023-03-19T08:54:44.026632Z",
+                    "iopub.status.busy": "2023-03-19T08:54:44.024799Z",
+                    "iopub.status.idle": "2023-03-19T08:54:44.034480Z",
+                    "shell.execute_reply": "2023-03-19T08:54:44.033518Z"
                 },
                 "lines_to_next_cell": 0
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Model with rank: 1\n",
-                        "Mean validation score: 0.546 (std: 0.061)\n",
-                        "Parameters: {'morgantransformer__nBits': 4096, 'morgantransformer__radius': 3, 'morgantransformer__useCounts': False, 'morgantransformer__useFeatures': False, 'ridge__alpha': 4.312365864763315}\n",
+                        "Mean validation score: 0.492 (std: 0.048)\n",
+                        "Parameters: {'morgantransformer__nBits': 2048, 'morgantransformer__radius': 4, 'morgantransformer__useCounts': False, 'morgantransformer__useFeatures': False, 'ridge__alpha': 18.49687467370123}\n",
                         "\n",
                         "Model with rank: 2\n",
-                        "Mean validation score: 0.508 (std: 0.114)\n",
-                        "Parameters: {'morgantransformer__nBits': 4096, 'morgantransformer__radius': 3, 'morgantransformer__useCounts': True, 'morgantransformer__useFeatures': False, 'ridge__alpha': 7.6093388407142575}\n",
+                        "Mean validation score: 0.446 (std: 0.188)\n",
+                        "Parameters: {'morgantransformer__nBits': 256, 'morgantransformer__radius': 2, 'morgantransformer__useCounts': False, 'morgantransformer__useFeatures': False, 'ridge__alpha': 0.22311472368521185}\n",
                         "\n",
                         "Model with rank: 3\n",
-                        "Mean validation score: 0.508 (std: 0.087)\n",
-                        "Parameters: {'morgantransformer__nBits': 512, 'morgantransformer__radius': 3, 'morgantransformer__useCounts': False, 'morgantransformer__useFeatures': False, 'ridge__alpha': 0.2749324296584268}\n",
+                        "Mean validation score: 0.440 (std: 0.025)\n",
+                        "Parameters: {'morgantransformer__nBits': 4096, 'morgantransformer__radius': 3, 'morgantransformer__useCounts': False, 'morgantransformer__useFeatures': True, 'ridge__alpha': 6.023414585108017}\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
                 "report(random_search.cv_results_)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "219e3e32",
             "metadata": {},
             "source": [
                 "It can be interesting to see what combinations of hyperparameters gave good results for the cross-validation. Usually the number of bits are in the high end and radius is 2 to 4. But this can vary a bit, as we do a small number of tries for this demo. More extended search with more iterations could maybe find even better and more consistent. solutions"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "630772af",
             "metadata": {},
             "source": [
                 "Let's see if standardization had any influence on this dataset. We build an inference pipeline that includes the standardization object and the best estimator, and run the best estimator directly on the list of test molecules"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
+            "id": "cb369a0e",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:36.008894Z",
-                    "iopub.status.busy": "2022-12-09T17:05:36.003125Z",
-                    "iopub.status.idle": "2022-12-09T17:05:36.173289Z",
-                    "shell.execute_reply": "2022-12-09T17:05:36.173697Z"
+                    "iopub.execute_input": "2023-03-19T08:54:44.041562Z",
+                    "iopub.status.busy": "2023-03-19T08:54:44.039729Z",
+                    "iopub.status.idle": "2023-03-19T08:54:44.258048Z",
+                    "shell.execute_reply": "2023-03-19T08:54:44.256978Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "No Standardization 0.5435\n",
-                        "With Standardization 0.5435\n"
+                        "No Standardization 0.5222\n",
+                        "With Standardization 0.5222\n"
                     ]
                 }
             ],
             "source": [
                 "inference_pipe = make_pipeline(standardizer, random_search.best_estimator_)\n",
                 "\n",
                 "print(f'No Standardization {random_search.best_estimator_.score(mol_list_test, y_test):0.4F}')\n",
                 "print(f'With Standardization {inference_pipe.score(mol_list_test, y_test):0.4F}')"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "e00bae88",
             "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2022-12-08T19:52:40.680157Z",
-                    "iopub.status.busy": "2022-12-08T19:52:40.669086Z",
-                    "iopub.status.idle": "2022-12-08T19:52:40.894050Z",
-                    "shell.execute_reply": "2022-12-08T19:52:40.893263Z"
-                },
                 "lines_to_next_cell": 0,
                 "title": "Building an inference pipeline, it appears our test-data was pretty standard"
             },
             "source": [
                 "We see that the dataset already appeared to be in forms that are similar to the ones coming from the standardization. \n",
                 "\n",
                 "Interestingly the test-set performance often seem to be better than the CV performance during the hyperparameter search. This may be due to the model being refit at the end of the search to the whole training dataset, as the refit parameter on the randomized_search object by default is true. The final model is thus fitted on more data than the individual models during training.\n",
                 "\n",
                 "To demonstrate the effect of standartization we can see the difference if we challenge the predictor with different forms of benzoic acid and benzoates."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
+            "id": "f6426b23",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-12-09T17:05:36.198952Z",
-                    "iopub.status.busy": "2022-12-09T17:05:36.196929Z",
-                    "iopub.status.idle": "2022-12-09T17:05:36.202973Z",
-                    "shell.execute_reply": "2022-12-09T17:05:36.203345Z"
+                    "iopub.execute_input": "2023-03-19T08:54:44.264895Z",
+                    "iopub.status.busy": "2023-03-19T08:54:44.264460Z",
+                    "iopub.status.idle": "2023-03-19T08:54:44.295917Z",
+                    "shell.execute_reply": "2023-03-19T08:54:44.294841Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Predictions with no standardization: [6.23241902 6.29654138 6.29654138 6.44934317 6.38440899]\n",
-                        "Predictions with standardization:    [6.23241902 6.23241902 6.23241902 6.23241902 6.23241902]\n"
+                        "Predictions with no standardization: [6.29056823 6.31806374 6.34706809 6.44119607 6.41499794]\n",
+                        "Predictions with standardization:    [6.29056823 6.29056823 6.29056823 6.29056823 6.29056823]\n"
                     ]
                 }
             ],
             "source": [
                 "# Intergrating the Standardizer and challenge it with some different forms and salts of benzoic acid\n",
                 "smiles_list = ['c1ccccc1C(=O)[OH]', 'c1ccccc1C(=O)[O-]', 'c1ccccc1C(=O)[O-].[Na+]', 'c1ccccc1C(=O)[O][Na]', 'c1ccccc1C(=O)[O-].C[N+](C)C']\n",
                 "mols_list = [Chem.MolFromSmiles(smiles) for smiles in smiles_list]\n",
                 "\n",
                 "print(f'Predictions with no standardization: {random_search.best_estimator_.predict(mols_list)}')\n",
                 "print(f'Predictions with standardization:    {inference_pipe.predict(mols_list)}')"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "47345289",
             "metadata": {},
             "source": [
                 "Without standardization we get variation in the predictions, but with the standardization object in place, we get the same results. If you want a model that gives different predictions for the different forms, either the standardization need to be removed or the settings changed.\n",
                 "\n",
                 "From here it should be easy to save the model using pickle, so that it can be loaded and used in other python projects. The pipeline carries both the standardization, the featurization and the prediction in one, easy to reuse object. If you want the model to be able to predict directly from SMILES strings, check out the SmilesToMol class, which is also available in Scikit-Mol :-)\n"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "8e0a8f49",
             "metadata": {},
             "source": []
         }
     ],
     "metadata": {
         "jupytext": {
             "cell_metadata_filter": "title,-all",
@@ -510,18 +535,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.4"
-        },
-        "vscode": {
-            "interpreter": {
-                "hash": "dc6218d6ccd9a44863300cd5111a59d6c18db4de812eb936d6a68ad5fa5cf18f"
-            }
+            "version": "3.10.9"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 5
 }
```

### Comparing `scikit_mol-0.1.2/notebooks/06_hyperparameter_tuning.py` & `scikit_mol-0.2.0/notebooks/06_hyperparameter_tuning.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #   jupytext:
 #     cell_metadata_filter: title,-all
 #     formats: ipynb,py:percent
 #     text_representation:
 #       extension: .py
 #       format_name: percent
 #       format_version: '1.3'
-#       jupytext_version: 1.14.1
+#       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3.9.4 ('rdkit')
 #     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
@@ -27,15 +27,16 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 from time import time
 import numpy as np
 from sklearn.pipeline import Pipeline, make_pipeline
 from sklearn.linear_model import Ridge
 from sklearn.model_selection import train_test_split
-from scikit_mol.transformers import MorganTransformer, SmilesToMol
+from scikit_mol.fingerprints import MorganFingerprintTransformer
+from scikit_mol.conversions import SmilesToMolTransformer
 
 # %% [markdown]
 # We will need some data. There is a dataset with the SLC6A4 active compounds from ExcapeDB on Zenodo. The scikit-mol project uses a subset of this for testing, and the samples there has been specially selected to give good results in testing (it should therefore be used for any production modelling). If full_set is false, the fast subset will be used, and otherwise the full dataset will be downloaded if needed.
 
 # %%
 full_set = False
 
@@ -79,15 +80,15 @@
 mol_list_std_train = standardizer.transform(mol_list_train)
 
 # %% [markdown]
 # A simple pipeline with a MorganTransformer and a Ridge() regression for demonstration.
 
 # %%
 
-moltransformer = MorganTransformer()
+moltransformer = MorganFingerprintTransformer()
 regressor = Ridge()
 
 optimization_pipe = make_pipeline(moltransformer, regressor)
 
 
 
 # %% [markdown]
```

### Comparing `scikit_mol-0.1.2/notebooks/07_parallel_transforms.ipynb` & `scikit_mol-0.2.0/notebooks/07_parallel_transforms.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7940438034188034%*

 * *Differences: {"'cells'": "{0: {'id': '3c3e2734', delete: ['attachments']}, 1: {'metadata': {replace: "*

 * *            "OrderedDict([('execution', OrderedDict([('iopub.execute_input', "*

 * *            "'2023-03-19T08:54:46.001221Z'), ('iopub.status.busy', '2023-03-19T08:54:46.000726Z'), "*

 * *            "('iopub.status.idle', '2023-03-19T08:54:46.882639Z'), ('shell.execute_reply', "*

 * *            "'2023-03-19T08:54:46.881724Z')]))])}, 'source': {insert: [(5, 'from "*

 * *            "scikit_mol.descriptors import MolecularDescriptorTran […]*

```diff
@@ -1,52 +1,69 @@
 {
     "cells": [
         {
-            "attachments": {},
             "cell_type": "markdown",
+            "id": "3c3e2734",
             "metadata": {},
             "source": [
                 "# Parallel calculations of transforms\n",
                 "\n",
                 "Scikit-mol supports parallel calculations of fingerprints and descriptors. This feature can be activated and configured using the `parallel` parameter or the `.parallel` attribute after object instantiation.\n",
                 "\n",
                 "To begin, let's import the necessary libraries: RDKit and pandas. And of course, we'll also need to import scikit-mol, which is the new kid on the block."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
-            "metadata": {},
+            "id": "d34a6f7e",
+            "metadata": {
+                "execution": {
+                    "iopub.execute_input": "2023-03-19T08:54:46.001221Z",
+                    "iopub.status.busy": "2023-03-19T08:54:46.000726Z",
+                    "iopub.status.idle": "2023-03-19T08:54:46.882639Z",
+                    "shell.execute_reply": "2023-03-19T08:54:46.881724Z"
+                }
+            },
             "outputs": [],
             "source": [
                 "from rdkit.Chem import PandasTools\n",
                 "import pandas as pd\n",
                 "import time\n",
                 "\n",
                 "\n",
-                "from scikit_mol.descriptors import Desc2DTransformer\n",
-                "from scikit_mol.transformers import MorganTransformer, SmilesToMol"
+                "from scikit_mol.descriptors import MolecularDescriptorTransformer\n",
+                "from scikit_mol.fingerprints import MorganFingerprintTransformer\n",
+                "from scikit_mol.conversions import SmilesToMolTransformer"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
+            "id": "f73bfd41",
             "metadata": {},
             "source": [
                 "## Obtaining the Data\n",
                 "\n",
                 "We'll need some data to work with, so we'll use a dataset of SLC6A4 active compounds from ExcapeDB that is available on Zenodo. Scikit-mol uses a subset of this dataset for testing purposes, and the samples have been specially selected to provide good results in testing. Note: This dataset should never be used for production modeling.\n",
                 "\n",
                 "In the code below, you can set full_set to True to download the full dataset. Otherwise, the smaller dataset will be used."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
-            "metadata": {},
+            "id": "f59b0883",
+            "metadata": {
+                "execution": {
+                    "iopub.execute_input": "2023-03-19T08:54:46.887587Z",
+                    "iopub.status.busy": "2023-03-19T08:54:46.886796Z",
+                    "iopub.status.idle": "2023-03-19T08:54:46.891008Z",
+                    "shell.execute_reply": "2023-03-19T08:54:46.890486Z"
+                }
+            },
             "outputs": [],
             "source": [
                 "full_set = False\n",
                 "\n",
                 "if full_set:\n",
                 "    csv_file = \"SLC6A4_active_excape_export.csv\"\n",
                 "    if not os.path.exists(csv_file):\n",
@@ -56,15 +73,23 @@
                 "else:\n",
                 "    csv_file = '../tests/data/SLC6A4_active_excapedb_subset.csv'"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
-            "metadata": {},
+            "id": "9cb3cb5c",
+            "metadata": {
+                "execution": {
+                    "iopub.execute_input": "2023-03-19T08:54:46.893737Z",
+                    "iopub.status.busy": "2023-03-19T08:54:46.893457Z",
+                    "iopub.status.idle": "2023-03-19T08:54:46.936836Z",
+                    "shell.execute_reply": "2023-03-19T08:54:46.936183Z"
+                }
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "0 out of 200 SMILES failed in conversion\n"
                     ]
@@ -75,123 +100,153 @@
                 "data = pd.read_csv(csv_file)\n",
                 "\n",
                 "PandasTools.AddMoleculeColumnToFrame(data, smilesCol=\"SMILES\")\n",
                 "print(f\"{data.ROMol.isna().sum()} out of {len(data)} SMILES failed in conversion\")"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
+            "id": "cbdda331",
             "metadata": {},
             "source": [
                 "## Evaluating the Impact of Parallelism on Transformations\n",
                 "\n",
                 "Let's start by creating a baseline for our calculations without using parallelism."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 4,
+            "id": "45c042f0",
             "metadata": {
+                "execution": {
+                    "iopub.execute_input": "2023-03-19T08:54:46.939675Z",
+                    "iopub.status.busy": "2023-03-19T08:54:46.939406Z",
+                    "iopub.status.idle": "2023-03-19T08:54:46.944552Z",
+                    "shell.execute_reply": "2023-03-19T08:54:46.943846Z"
+                },
                 "title": "A demonstration of the speedup that can be had for the descriptor transformer"
             },
             "outputs": [],
             "source": [
-                "transformer = Desc2DTransformer(parallel=False)"
+                "transformer = MolecularDescriptorTransformer(parallel=False)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
-            "metadata": {},
+            "execution_count": 5,
+            "id": "8f158499",
+            "metadata": {
+                "execution": {
+                    "iopub.execute_input": "2023-03-19T08:54:46.947093Z",
+                    "iopub.status.busy": "2023-03-19T08:54:46.946789Z",
+                    "iopub.status.idle": "2023-03-19T08:54:49.121374Z",
+                    "shell.execute_reply": "2023-03-19T08:54:49.120448Z"
+                }
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Calculation time on dataset of size 200  with parallel=False:\t2.06 seconds\n"
+                        "Calculation time on dataset of size 200  with parallel=False:\t2.17 seconds\n"
                     ]
                 }
             ],
             "source": [
                 "def test_transformer(transformer):\n",
                 "    t0 = time.time()\n",
                 "    X = transformer.transform(data.ROMol)\n",
                 "    t = time.time()-t0\n",
                 "    print(f\"Calculation time on dataset of size {len(data)}  with parallel={transformer.parallel}:\\t{t:0.2F} seconds\")\n",
                 "test_transformer(transformer)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
+            "id": "08b2cb6e",
             "metadata": {},
             "source": [
                 "\n",
                 "Let's see if parallelism can help us speed up our transformations."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
-            "metadata": {},
+            "execution_count": 6,
+            "id": "f1b48596",
+            "metadata": {
+                "execution": {
+                    "iopub.execute_input": "2023-03-19T08:54:49.124419Z",
+                    "iopub.status.busy": "2023-03-19T08:54:49.124108Z",
+                    "iopub.status.idle": "2023-03-19T08:54:50.037528Z",
+                    "shell.execute_reply": "2023-03-19T08:54:50.036724Z"
+                }
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Calculation time on dataset of size 200  with parallel=True:\t1.34 seconds\n"
+                        "Calculation time on dataset of size 200  with parallel=True:\t0.91 seconds\n"
                     ]
                 }
             ],
             "source": [
                 "\n",
-                "transformer = Desc2DTransformer(parallel=True)\n",
+                "transformer = MolecularDescriptorTransformer(parallel=True)\n",
                 "test_transformer(transformer)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
+            "id": "267de7b7",
             "metadata": {},
             "source": [
                 "We've seen that parallelism can help speed up our transformations, with the degree of speedup depending on the number of CPU cores available. However, it's worth noting that there may be some overhead associated with the process of splitting the dataset, pickling objects and functions, and passing them to the parallel child processes. As a result, it may not always be worthwhile to use parallelism, particularly for smaller datasets or certain types of fingerprints.\n",
                 "\n",
                 "It's also worth noting that there are different methods for creating the child processes, with the default method on Linux being 'fork', while on Mac and Windows it's 'spawn'. The code we're using has been tested on Linux using the 'fork' method.\n",
                 "\n",
                 "Now, let's see how parallelism impacts another type of transformer."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 7,
+            "id": "f8b61e6c",
             "metadata": {
+                "execution": {
+                    "iopub.execute_input": "2023-03-19T08:54:50.040549Z",
+                    "iopub.status.busy": "2023-03-19T08:54:50.040317Z",
+                    "iopub.status.idle": "2023-03-19T08:54:50.144137Z",
+                    "shell.execute_reply": "2023-03-19T08:54:50.143373Z"
+                },
                 "lines_to_next_cell": 2,
                 "title": "Some of the benchmarking plots"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Calculation time on dataset of size 200  with parallel=False:\t0.04 seconds\n",
-                        "Calculation time on dataset of size 200  with parallel=True:\t0.13 seconds\n"
+                        "Calculation time on dataset of size 200  with parallel=False:\t0.02 seconds\n",
+                        "Calculation time on dataset of size 200  with parallel=True:\t0.08 seconds\n"
                     ]
                 }
             ],
             "source": [
-                "transformer = MorganTransformer(parallel=False)\n",
+                "transformer = MorganFingerprintTransformer(parallel=False)\n",
                 "test_transformer(transformer)\n",
                 "transformer.parallel = True\n",
                 "test_transformer(transformer)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
+            "id": "9c29a58f",
             "metadata": {},
             "source": [
                 "Interestingly, we observed that parallelism actually took longer to calculate the fingerprints in some cases, which is a perfect illustration of the overhead issue associated with parallelism. Generally, the faster the fingerprint calculation in itself, the larger the dataset needs to be for parallelism to be worthwhile. For example, the Descriptor transformer, which is one of the slowest, can benefit even for smaller datasets, while for faster fingerprint types like Morgan, Atompairs, and Topological Torsion fingerprints, the dataset needs to be larger.\n",
                 "\n",
                 "![ Relation ship between throughput and parallel speedup](https://github.com/EBjerrum/scikit-mol/raw/main/notebooks/images/max_speedup_vs_throughput.png \"Not all fingerprints are equally fast and benefit the same from parallelism\")\n",
                 "\n",
                 "We've also included a series of plots below, showing the speedup over serial for different numbers of cores used for different dataset sizes. These timings were taken on a 16 core machine (32 Hyperthreads). Only the largest datasets (>10,000 samples) would make it worthwhile to parallelize Morgan, Atompairs, and Topological Torsions. SECfingerprint, MACCS keys, and RDKitFP are intermediate and would benefit from parallelism when the dataset size is larger, say >500. Descriptors, on the other hand, benefit almost immediately even for the smallest datasets (>100 samples).\n",
@@ -214,16 +269,15 @@
                 "\n"
             ]
         }
     ],
     "metadata": {
         "jupytext": {
             "cell_metadata_filter": "title,-all",
-            "formats": "ipynb,py:percent",
-            "main_language": "python"
+            "formats": "ipynb,py:percent"
         },
         "kernelspec": {
             "display_name": "rdkit2",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
@@ -233,17 +287,12 @@
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.10.9"
-        },
-        "vscode": {
-            "interpreter": {
-                "hash": "e701a5111a346cb2e1e77ca225e26cf8da6f62a90d5df6197f147c55a3018ac3"
-            }
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 5
 }
```

### Comparing `scikit_mol-0.1.2/notebooks/07_parallel_transforms.py` & `scikit_mol-0.2.0/notebooks/07_parallel_transforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #   jupytext:
 #     cell_metadata_filter: title,-all
 #     formats: ipynb,py:percent
 #     text_representation:
 #       extension: .py
 #       format_name: percent
 #       format_version: '1.3'
-#       jupytext_version: 1.14.1
+#       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: rdkit2
 #     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
@@ -23,16 +23,17 @@
 
 # %%
 from rdkit.Chem import PandasTools
 import pandas as pd
 import time
 
 
-from scikit_mol.descriptors import Desc2DTransformer
-from scikit_mol.transformers import MorganTransformer, SmilesToMol
+from scikit_mol.descriptors import MolecularDescriptorTransformer
+from scikit_mol.fingerprints import MorganFingerprintTransformer
+from scikit_mol.conversions import SmilesToMolTransformer
 
 # %% [markdown]
 # ## Obtaining the Data
 #
 # We'll need some data to work with, so we'll use a dataset of SLC6A4 active compounds from ExcapeDB that is available on Zenodo. Scikit-mol uses a subset of this dataset for testing purposes, and the samples have been specially selected to provide good results in testing. Note: This dataset should never be used for production modeling.
 #
 # In the code below, you can set full_set to True to download the full dataset. Otherwise, the smaller dataset will be used.
@@ -58,15 +59,15 @@
 
 # %% [markdown]
 # ## Evaluating the Impact of Parallelism on Transformations
 #
 # Let's start by creating a baseline for our calculations without using parallelism.
 
 # %% A demonstration of the speedup that can be had for the descriptor transformer
-transformer = Desc2DTransformer(parallel=False)
+transformer = MolecularDescriptorTransformer(parallel=False)
 
 
 # %%
 def test_transformer(transformer):
     t0 = time.time()
     X = transformer.transform(data.ROMol)
     t = time.time()-t0
@@ -75,26 +76,26 @@
 
 # %% [markdown]
 #
 # Let's see if parallelism can help us speed up our transformations.
 
 # %%
 
-transformer = Desc2DTransformer(parallel=True)
+transformer = MolecularDescriptorTransformer(parallel=True)
 test_transformer(transformer)
 
 # %% [markdown]
 # We've seen that parallelism can help speed up our transformations, with the degree of speedup depending on the number of CPU cores available. However, it's worth noting that there may be some overhead associated with the process of splitting the dataset, pickling objects and functions, and passing them to the parallel child processes. As a result, it may not always be worthwhile to use parallelism, particularly for smaller datasets or certain types of fingerprints.
 #
 # It's also worth noting that there are different methods for creating the child processes, with the default method on Linux being 'fork', while on Mac and Windows it's 'spawn'. The code we're using has been tested on Linux using the 'fork' method.
 #
 # Now, let's see how parallelism impacts another type of transformer.
 
 # %% Some of the benchmarking plots
-transformer = MorganTransformer(parallel=False)
+transformer = MorganFingerprintTransformer(parallel=False)
 test_transformer(transformer)
 transformer.parallel = True
 test_transformer(transformer)
 
 
 # %% [markdown]
 # Interestingly, we observed that parallelism actually took longer to calculate the fingerprints in some cases, which is a perfect illustration of the overhead issue associated with parallelism. Generally, the faster the fingerprint calculation in itself, the larger the dataset needs to be for parallelism to be worthwhile. For example, the Descriptor transformer, which is one of the slowest, can benefit even for smaller datasets, while for faster fingerprint types like Morgan, Atompairs, and Topological Torsion fingerprints, the dataset needs to be larger.
```

### Comparing `scikit_mol-0.1.2/notebooks/README.md` & `scikit_mol-0.2.0/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/images/AtomPairFingerprintTransformer_par.png` & `scikit_mol-0.2.0/notebooks/images/AtomPairFingerprintTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/images/AtomPairFingerprintTransformer_par.svg` & `scikit_mol-0.2.0/notebooks/images/AtomPairFingerprintTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/images/Desc2DTransformer_par.png` & `scikit_mol-0.2.0/notebooks/images/Desc2DTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/images/Desc2DTransformer_par.svg` & `scikit_mol-0.2.0/notebooks/images/Desc2DTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/images/MACCSTransformer_par.png` & `scikit_mol-0.2.0/notebooks/images/MACCSTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/images/MACCSTransformer_par.svg` & `scikit_mol-0.2.0/notebooks/images/MACCSTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/images/MorganTransformer_par.png` & `scikit_mol-0.2.0/notebooks/images/MorganTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/images/MorganTransformer_par.svg` & `scikit_mol-0.2.0/notebooks/images/MorganTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/images/RDKitFPTransformer_par.png` & `scikit_mol-0.2.0/notebooks/images/RDKitFPTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/images/RDKitFPTransformer_par.svg` & `scikit_mol-0.2.0/notebooks/images/RDKitFPTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/images/SECFingerprintTransformer_par.png` & `scikit_mol-0.2.0/notebooks/images/SECFingerprintTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/images/SECFingerprintTransformer_par.svg` & `scikit_mol-0.2.0/notebooks/images/SECFingerprintTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/images/TopologicalTorsionFingerprintTransformer_par.png` & `scikit_mol-0.2.0/notebooks/images/TopologicalTorsionFingerprintTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/images/TopologicalTorsionFingerprintTransformer_par.svg` & `scikit_mol-0.2.0/notebooks/images/TopologicalTorsionFingerprintTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/images/Transformer_Widget.jpg` & `scikit_mol-0.2.0/notebooks/images/Transformer_Widget.jpg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/images/max_speedup_vs_throughput.png` & `scikit_mol-0.2.0/notebooks/images/max_speedup_vs_throughput.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/notebooks/images/max_speedup_vs_throughput.svg` & `scikit_mol-0.2.0/notebooks/images/max_speedup_vs_throughput.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/scikit_mol/descriptors.py` & `scikit_mol-0.2.0/scikit_mol/descriptors.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from rdkit.Chem import Descriptors
 from rdkit.ML.Descriptors.MoleculeDescriptors import MolecularDescriptorCalculator
 
 from sklearn.base import BaseEstimator, TransformerMixin
 
 
 
-class Desc2DTransformer(BaseEstimator, TransformerMixin):
+class MolecularDescriptorTransformer(BaseEstimator, TransformerMixin):
     """Descriptor calculation transformer
     
     Parameters
     ----------
     desc_list : (List of descriptor names)
         A list of RDKit descriptors to include in the calculation
     parallel : boolean, int
@@ -130,14 +130,14 @@
 
 
 # May be safer to instantiate the transformer object in the child process, and only transfer the parameters
 # There were issues with freezing when using RDKit 2022.3
 def parallel_helper(args):
     """Will get a tuple with Desc2DTransformer parameters and mols to transform. 
     Will then instantiate the transformer and transform the molecules"""
-    from scikit_mol.descriptors import Desc2DTransformer
+    from scikit_mol.descriptors import MolecularDescriptorTransformer
     
     params, mols = args
-    transformer = Desc2DTransformer(**params)
+    transformer = MolecularDescriptorTransformer(**params)
     y = transformer._transform(mols)
     return y
```

### Comparing `scikit_mol-0.1.2/scikit_mol/sanitizer.py` & `scikit_mol-0.2.0/scikit_mol/utilities.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/scikit_mol/standardizer.py` & `scikit_mol-0.2.0/scikit_mol/standardizer.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/scikit_mol/transformers.py` & `scikit_mol-0.2.0/scikit_mol/fingerprints.py`

 * *Files 10% similar despite different names*

```diff
@@ -89,28 +89,38 @@
                 parameters = self.get_params()
                 arrays = pool.map(parallel_helper, [(self.__class__.__name__, parameters, x_chunk) for x_chunk in x_chunks]) 
 
                 arr = np.concatenate(arrays)
             return arr
 
 
-class MACCSTransformer(FpsTransformer):
+class MACCSKeysFingerprintTransformer(FpsTransformer):
     def __init__(self, parallel: Union[bool, int] = False):
         """MACCS keys fingerprinter
         calculates the 167 fixed MACCS keys
         """
         super().__init__(parallel = parallel)
         self.nBits = 167
 
+    @property
+    def nBits(self):
+        return self._nBits
+
+    @nBits.setter
+    def nBits(self, nBits):
+        if nBits != 167:
+            raise ValueError("nBits can only be 167, matching the number of defined MACCS keys!")
+        self._nBits = nBits
+
     def _mol2fp(self, mol):
         return rdMolDescriptors.GetMACCSKeysFingerprint(
             mol
         )
 
-class RDKitFPTransformer(FpsTransformer):
+class RDKitFingerprintTransformer(FpsTransformer):
     def __init__(self, minPath:int = 1, maxPath:int =7, useHs:bool = True, branchedPaths:bool = True,
                  useBondOrder:bool = True, countSimulation:bool = False, countBounds = None,
                  fpSize:int  = 2048, numBitsPerFeature:int = 2, atomInvariantsGenerator = None,
                  parallel: Union[bool, int] = False
                  ):
         """Calculates the RDKit fingerprints
 
@@ -155,20 +165,20 @@
 
     #Scikit-Learn expects to be able to set fpSize directly on object via .set_params(), so this updates nBits used by the abstract class
     @fpSize.setter
     def fpSize(self, fpSize):
         self.nBits = fpSize
 
     def _mol2fp(self, mol):
-        generator = rdFingerprintGenerator.GetRDKitFPGenerator(minPath=self.minPath, maxPath=self.maxPath,
-                                                               useHs=self.useHs, branchedPaths=self.branchedPaths,
-                                                               useBondOrder=self.useBondOrder,
-                                                               countSimulation=self.countSimulation,
-                                                               countBounds=self.countBounds, fpSize=self.fpSize,
-                                                               numBitsPerFeature=self.numBitsPerFeature,
+        generator = rdFingerprintGenerator.GetRDKitFPGenerator(minPath=int(self.minPath), maxPath=int(self.maxPath),
+                                                               useHs=bool(self.useHs), branchedPaths=bool(self.branchedPaths),
+                                                               useBondOrder=bool(self.useBondOrder),
+                                                               countSimulation=bool(self.countSimulation),
+                                                               countBounds=bool(self.countBounds), fpSize=int(self.fpSize),
+                                                               numBitsPerFeature=int(self.numBitsPerFeature),
                                                                atomInvariantsGenerator=self.atomInvariantsGenerator
                                                                )
         return generator.GetFingerprint(mol)
 
 class AtomPairFingerprintTransformer(FpsTransformer): #FIXME, some of the init arguments seems to be molecule specific, and should probably not be setable?
     def __init__(self, minLength:int = 1, maxLength:int = 30, fromAtoms = 0, ignoreAtoms = 0, atomInvariants = 0,
                  nBitsPerEntry:int = 4, includeChirality:bool = False, use2D:bool = True, confId:int = -1, nBits=2048,
@@ -184,35 +194,35 @@
         self.confId = confId
         self.nBits = nBits
         self.nBitsPerEntry = nBitsPerEntry
         self.useCounts = useCounts
 
     def _mol2fp(self, mol):
         if self.useCounts:
-            return rdMolDescriptors.GetHashedAtomPairFingerprint(mol, nBits=self.nBits,
-                                                                 minLength=self.minLength,
-                                                                 maxLength=self.maxLength,
+            return rdMolDescriptors.GetHashedAtomPairFingerprint(mol, nBits=int(self.nBits),
+                                                                 minLength=int(self.minLength),
+                                                                 maxLength=int(self.maxLength),
                                                                  fromAtoms=self.fromAtoms,
                                                                  ignoreAtoms=self.ignoreAtoms,
                                                                  atomInvariants=self.atomInvariants,
-                                                                 includeChirality=self.includeChirality,
-                                                                 use2D=self.use2D,
-                                                                 confId=self.confId
+                                                                 includeChirality=bool(self.includeChirality),
+                                                                 use2D=bool(self.use2D),
+                                                                 confId=int(self.confId)
                                                            )
         else:
-            return rdMolDescriptors.GetHashedAtomPairFingerprintAsBitVect(mol, nBits=self.nBits,
-                                                                          minLength=self.minLength,
-                                                                          maxLength=self.maxLength,
+            return rdMolDescriptors.GetHashedAtomPairFingerprintAsBitVect(mol, nBits=int(self.nBits),
+                                                                          minLength=int(self.minLength),
+                                                                          maxLength=int(self.maxLength),
                                                                           fromAtoms=self.fromAtoms,
                                                                           ignoreAtoms=self.ignoreAtoms,
                                                                           atomInvariants=self.atomInvariants,
-                                                                          nBitsPerEntry=self.nBitsPerEntry,
-                                                                          includeChirality=self.includeChirality,
-                                                                          use2D=self.use2D,
-                                                                          confId=self.confId
+                                                                          nBitsPerEntry=int(self.nBitsPerEntry),
+                                                                          includeChirality=bool(self.includeChirality),
+                                                                          use2D=bool(self.use2D),
+                                                                          confId=int(self.confId)
                                                        )
 
 class TopologicalTorsionFingerprintTransformer(FpsTransformer):
     def __init__(self, targetSize:int = 4, fromAtoms = 0, ignoreAtoms = 0, atomInvariants = 0,
                  includeChirality:bool = False, nBitsPerEntry:int = 4, nBits=2048,
                  useCounts:bool=False, parallel: Union[bool, int] = False):
         super().__init__(parallel = parallel)
@@ -223,31 +233,113 @@
         self.includeChirality = includeChirality
         self.nBitsPerEntry = nBitsPerEntry
         self.nBits = nBits
         self.useCounts = useCounts
 
     def _mol2fp(self, mol):
         if self.useCounts:
-            return rdMolDescriptors.GetHashedTopologicalTorsionFingerprint(mol, nBits=self.nBits,
-                                                                           targetSize=self.targetSize,
+            return rdMolDescriptors.GetHashedTopologicalTorsionFingerprint(mol, nBits=int(self.nBits),
+                                                                           targetSize=int(self.targetSize),
                                                                            fromAtoms=self.fromAtoms,
                                                                            ignoreAtoms=self.ignoreAtoms,
                                                                            atomInvariants=self.atomInvariants,
-                                                                           includeChirality=self.includeChirality,
+                                                                           includeChirality=bool(self.includeChirality),
                                                            )
         else:
-            return rdMolDescriptors.GetHashedTopologicalTorsionFingerprintAsBitVect(mol, nBits=self.nBits,
-                                                                                    targetSize=self.targetSize,
+            return rdMolDescriptors.GetHashedTopologicalTorsionFingerprintAsBitVect(mol, nBits=int(self.nBits),
+                                                                                    targetSize=int(self.targetSize),
                                                                                     fromAtoms=self.fromAtoms,
                                                                                     ignoreAtoms=self.ignoreAtoms,
                                                                                     atomInvariants=self.atomInvariants,
-                                                                                    includeChirality=self.includeChirality,
-                                                                                    nBitsPerEntry=self.nBitsPerEntry
+                                                                                    includeChirality=bool(self.includeChirality),
+                                                                                    nBitsPerEntry=int(self.nBitsPerEntry)
                                                                                     )
 
+class MHFingerprintTransformer(FpsTransformer):
+    # https://jcheminf.biomedcentral.com/articles/10.1186/s13321-018-0321-8
+    def __init__(self, radius:int=3, rings:bool=True, isomeric:bool=False, kekulize:bool=False,
+                 min_radius:int=1, n_permutations:int=2048, seed:int=42, parallel: Union[bool, int] = False,):
+        """Transforms the RDKit mol into the MinHash fingerprint (MHFP)
+
+        Args:
+            radius (int, optional): The MHFP radius. Defaults to 3.
+            rings (bool, optional): Whether or not to include rings in the shingling. Defaults to True.
+            isomeric (bool, optional): Whether the isomeric SMILES to be considered. Defaults to False.
+            kekulize (bool, optional): Whether or not to kekulize the extracted SMILES. Defaults to False.
+            min_radius (int, optional): The minimum radius that is used to extract n-gram. Defaults to 1.
+            n_permutations (int, optional): The number of permutations used for hashing. Defaults to 0, 
+            this is effectively the length of the FP
+            seed (int, optional): The value used to seed numpy.random. Defaults to 0.
+        """
+        super().__init__(parallel = parallel)
+        self.radius = radius
+        self.rings = rings
+        self.isomeric = isomeric
+        self.kekulize = kekulize
+        self.min_radius = min_radius
+        #Set the .n_permutations and .seed without creating the encoder twice
+        self._n_permutations = n_permutations
+        self._seed = seed
+        # create the encoder instance
+        self._recreate_encoder()
+
+    def __getstate__(self):
+        # Get the state of the parent class
+        state = super().__getstate__()
+        # Remove the unpicklable property from the state
+        state.pop("mhfp_encoder", None) # mhfp_encoder is not picklable
+        return state
+
+    def __setstate__(self, state):
+        # Restore the state of the parent class
+        super().__setstate__(state)
+        # Re-create the unpicklable property
+        self._recreate_encoder()
+
+    def _transform(self, X):
+        arr = np.zeros((len(X), self.nBits), dtype=np.int32)
+        for i, mol in enumerate(X):
+            arr[i,:] = self._transform_mol(mol)
+        return arr
+
+    def _mol2fp(self, mol):
+        fp = self.mhfp_encoder.EncodeMol(mol, self.radius, self.rings, self.isomeric, self.kekulize, self.min_radius)
+        return fp
+    
+    def _fp2array(self, fp):
+        return np.array(fp)
+
+    def _recreate_encoder(self):
+        self.mhfp_encoder = rdMHFPFingerprint.MHFPEncoder(self._n_permutations, self._seed)
+
+    @property
+    def seed(self):
+        return self._seed
+
+    @seed.setter
+    def seed(self, seed):
+        self._seed = seed
+        # each time the seed parameter is modified refresh an instance of the encoder
+        self._recreate_encoder()
+
+    @property
+    def n_permutations(self):
+        return self._n_permutations
+
+    @n_permutations.setter
+    def n_permutations(self, n_permutations):
+        self._n_permutations = n_permutations
+        # each time the n_permutations parameter is modified refresh an instance of the encoder
+        self._recreate_encoder()
+
+    @property
+    def nBits(self):
+        # to be compliant with the requirement of the base class
+        return self._n_permutations
+
 class SECFingerprintTransformer(FpsTransformer):
     # https://jcheminf.biomedcentral.com/articles/10.1186/s13321-018-0321-8
     def __init__(self, radius:int=3, rings:bool=True, isomeric:bool=False, kekulize:bool=False,
                  min_radius:int=1, length:int=2048, n_permutations:int=0, seed:int=0, parallel: Union[bool, int] = False,):
         """Transforms the RDKit mol into the SMILES extended connectivity fingerprint (SECFP)
 
         Args:
@@ -263,37 +355,38 @@
         super().__init__(parallel = parallel)
         self.radius = radius
         self.rings = rings
         self.isomeric = isomeric
         self.kekulize = kekulize
         self.min_radius = min_radius
         self.length = length
+        #Set the .n_permutations and seed without creating the encoder twice
         self._n_permutations = n_permutations
         self._seed = seed
         # create the encoder instance
         self._recreate_encoder()
 
     def __getstate__(self):
         # Get the state of the parent class
         state = super().__getstate__()
         # Remove the unpicklable property from the state
-        state.pop("secfp_encoder", None) # secfp_encoder is not picklable
+        state.pop("mhfp_encoder", None) # mhfp_encoder is not picklable
         return state
 
     def __setstate__(self, state):
         # Restore the state of the parent class
         super().__setstate__(state)
         # Re-create the unpicklable property
         self._recreate_encoder()
 
     def _mol2fp(self, mol):
-        return self.secfp_encoder.EncodeSECFPMol(mol, self.radius, self.rings, self.isomeric, self.kekulize, self.min_radius, self.length) 
+        return self.mhfp_encoder.EncodeSECFPMol(mol, self.radius, self.rings, self.isomeric, self.kekulize, self.min_radius, self.length) 
 
     def _recreate_encoder(self):
-        self.secfp_encoder = rdMHFPFingerprint.MHFPEncoder(self._n_permutations, self._seed) #TODO, this seems unpicklable, need to delete property when pickling, and recreate it when unpickling!
+        self.mhfp_encoder = rdMHFPFingerprint.MHFPEncoder(self._n_permutations, self._seed)
 
     @property
     def seed(self):
         return self._seed
 
     @seed.setter
     def seed(self, seed):
@@ -312,15 +405,15 @@
         self._recreate_encoder()
 
     @property
     def nBits(self):
         # to be compliant with the requirement of the base class
         return self.length
 
-class MorganTransformer(FpsTransformer):
+class MorganFingerprintTransformer(FpsTransformer):
     def __init__(self, nBits=2048, radius=2, useChirality=False, useBondTypes=True, useFeatures=False, useCounts=False, parallel: Union[bool, int] = False,):
         """Transform RDKit mols into Count or bit-based hashed MorganFingerprints
 
         Parameters
         ----------
         nBits : int, optional
             Size of the hashed fingerprint, by default 2048
@@ -342,89 +435,28 @@
         self.useBondTypes = useBondTypes
         self.useFeatures = useFeatures
         self.useCounts = useCounts
 
     def _mol2fp(self, mol):
         if self.useCounts:
             return rdMolDescriptors.GetHashedMorganFingerprint(
-                mol,self.radius,nBits=self.nBits, useFeatures=self.useFeatures,
-                useChirality=self.useChirality, useBondTypes=self.useBondTypes
+                mol,int(self.radius),nBits=int(self.nBits), useFeatures=bool(self.useFeatures),
+                useChirality=bool(self.useChirality), useBondTypes=bool(self.useBondTypes)
             )
         else:
             return rdMolDescriptors.GetMorganFingerprintAsBitVect(
-                mol,self.radius,nBits=self.nBits, useFeatures=self.useFeatures,
-                useChirality=self.useChirality, useBondTypes=self.useBondTypes
+                mol,int(self.radius),nBits=int(self.nBits), useFeatures=bool(self.useFeatures),
+                useChirality=bool(self.useChirality), useBondTypes=bool(self.useBondTypes)
             )
         
 
-class SmilesToMol(BaseEstimator, TransformerMixin):
-
-    def __init__(self, parallel: Union[bool, int] = False):
-        self.parallel = parallel
-        self.start_method = None  #TODO implement handling of start_method
-
-    def fit(self, X=None, y=None):
-        """Included for scikit-learn compatibility, does nothing"""
-        return self
-
-    def transform(self, X_smiles_list, y=None):
-        """Converts SMILES into RDKit mols
-
-        Parameters
-        ----------
-        X_smiles_list : list-like
-            A list of RDKit parsable strings
-
-        Returns
-        -------
-        List
-            List of RDKit mol objects
-
-        Raises
-        ------
-        ValueError
-            Raises ValueError if a SMILES string is unparsable by RDKit
-        """
-        
-
-        if not self.parallel:
-            return self._transform(X_smiles_list)
-        elif self.parallel:
-            n_processes = self.parallel if self.parallel > 1 else None # Pool(processes=None) autodetects
-            n_chunks = n_processes*2 if n_processes is not None else multiprocessing.cpu_count()*2 #TODO, tune the number of chunks per child process
-            with get_context(self.start_method).Pool(processes=n_processes) as pool:
-                    x_chunks = np.array_split(X_smiles_list, n_chunks) 
-                    arrays = pool.map(self._transform, x_chunks) #is the helper function a safer way of handling the picklind and child process communication
-
-                    arr = np.concatenate(arrays)
-                    return arr
-
-    def _transform(self, X_smiles_list):
-        X_out = []
-        for smiles in X_smiles_list:
-            mol = Chem.MolFromSmiles(smiles)
-            if mol:
-                X_out.append(mol)
-            else:
-                raise ValueError(f'Issue with parsing SMILES {smiles}\nYou probably should use the scikit-mol.sanitizer.Sanitizer on your dataset first')
-
-        return X_out
-
-    def inverse_transform(self, X_mols_list, y=None): #TODO, maybe the inverse transform should be configurable e.g. isomericSmiles etc.?
-        X_out = []
-
-        for mol in X_mols_list:
-            smiles = Chem.MolToSmiles(mol)
-            X_out.append(smiles)
-
-        return X_out
 
 
 def parallel_helper(args):
     """Parallel_helper takes a tuple with classname, the objects parameters and the mols to process.
     Then instantiates the class with the parameters and processes the mol.
     Intention is to be able to do this in chilcprocesses as some classes can't be pickled"""
     classname, parameters, X_mols = args
-    from scikit_mol import transformers
-    transformer = getattr(transformers, classname)(**parameters)
+    from scikit_mol import fingerprints
+    transformer = getattr(fingerprints, classname)(**parameters)
     return transformer._transform(X_mols)
```

### Comparing `scikit_mol-0.1.2/scikit_mol.egg-info/PKG-INFO` & `scikit_mol-0.2.0/scikit_mol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-mol
-Version: 0.1.2
+Version: 0.2.0
 Summary: scikit-learn classes for molecule transformation
 Home-page: https://github.com/EBjerrum/scikit-mol
 Download-URL: https://github.com/EBjerrum/scikit-mol
 Author: Esben Jannik Bjerrum
 Author-email: esben@cheminformania.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
@@ -96,7 +96,8 @@
 * Esben Jannik Bjerrum [@ebjerrum](https://github.com/ebjerrum), esben@cheminformania.com
 * Carmen Esposito [@cespos](https://github.com/cespos)
 * Son Ha, sonha@uni-mainz.de
 * Oh-hyeon Choung, ohhyeon.choung@gmail.com
 * Andreas Poehlmann, [@ap--](https://github.com/ap--)
 * Ya Chen, [@anya-chen](https://github.com/anya-chen)
 * Rafał Bachorz [@rafalbachorz](https://github.com/rafalbachorz)
+* Adrien Chaton [@adrienchaton](https://github.com/adrienchaton)
```

### Comparing `scikit_mol-0.1.2/scikit_mol.egg-info/SOURCES.txt` & `scikit_mol-0.2.0/scikit_mol.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 notebooks/04_standardizer.py
 notebooks/05_smiles_sanitaztion.ipynb
 notebooks/05_smiles_sanitaztion.py
 notebooks/06_hyperparameter_tuning.ipynb
 notebooks/06_hyperparameter_tuning.py
 notebooks/07_parallel_transforms.ipynb
 notebooks/07_parallel_transforms.py
+notebooks/08_external_library_skopt.py
 notebooks/README.md
 notebooks/pair_notebook.sh
 notebooks/run_notebooks.sh
 notebooks/sync_notebooks.sh
 notebooks/02_descriptor_transformer_files/02_descriptor_transformer_5_0.png
 notebooks/04_standardizer_files/04_standardizer_3_0.png
 notebooks/04_standardizer_files/04_standardizer_3_1.png
@@ -39,25 +40,27 @@
 notebooks/images/TopologicalTorsionFingerprintTransformer_par.png
 notebooks/images/TopologicalTorsionFingerprintTransformer_par.svg
 notebooks/images/Transformer_Widget.jpg
 notebooks/images/max_speedup_vs_throughput.png
 notebooks/images/max_speedup_vs_throughput.svg
 scikit_mol/__init__.py
 scikit_mol/_version.py
+scikit_mol/conversions.py
 scikit_mol/descriptors.py
-scikit_mol/sanitizer.py
+scikit_mol/fingerprints.py
 scikit_mol/standardizer.py
-scikit_mol/transformers.py
+scikit_mol/utilities.py
 scikit_mol.egg-info/PKG-INFO
 scikit_mol.egg-info/SOURCES.txt
 scikit_mol.egg-info/dependency_links.txt
 scikit_mol.egg-info/requires.txt
 scikit_mol.egg-info/top_level.txt
 tests/conftest.py
 tests/fixtures.py
 tests/test_desctransformer.py
 tests/test_fptransformers.py
+tests/test_parameter_types.py
 tests/test_sanitizer.py
 tests/test_scikit_mol.py
 tests/test_smilestomol.py
 tests/test_transformers.py
 tests/data/SLC6A4_active_excapedb_subset.csv
```

### Comparing `scikit_mol-0.1.2/setup.cfg` & `scikit_mol-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/tests/conftest.py` & `scikit_mol-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/tests/data/SLC6A4_active_excapedb_subset.csv` & `scikit_mol-0.2.0/tests/data/SLC6A4_active_excapedb_subset.csv`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/tests/fixtures.py` & `scikit_mol-0.2.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.1.2/tests/test_desctransformer.py` & `scikit_mol-0.2.0/tests/test_desctransformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import time
 import pytest 
 import numpy as np
 import pandas as pd
 from rdkit.Chem import Descriptors
-from scikit_mol.descriptors import Desc2DTransformer
+from scikit_mol.descriptors import MolecularDescriptorTransformer
 from fixtures import mols_list, smiles_list
 from sklearn import clone
 import joblib
 
 
 
 @pytest.fixture
 def default_descriptor_transformer():
-    return Desc2DTransformer()
+    return MolecularDescriptorTransformer()
 
 @pytest.fixture
 def selected_descriptor_transformer():
-    return Desc2DTransformer(desc_list=['HeavyAtomCount', 'FractionCSP3', 'RingCount', 'MolLogP', 'MolWt'])
+    return MolecularDescriptorTransformer(desc_list=['HeavyAtomCount', 'FractionCSP3', 'RingCount', 'MolLogP', 'MolWt'])
 
 def test_descriptor_transformer_clonability( default_descriptor_transformer):
     for t in [ default_descriptor_transformer]:
         params   = t.get_params()
         t2 = clone(t)
         params_2 = t2.get_params()
         #Parameters of cloned transformers should be the same
@@ -53,25 +53,25 @@
     for mols in  [mols_list, np.array(mols_list), pd.Series(mols_list)]:
         features = default_descriptor_transformer.transform(mols)
         assert(len(features) == len(mols))
         assert(len(features[0]) == len(Descriptors._descList))
         
 def test_descriptor_transformer_wrong_descriptors():
     with pytest.raises(AssertionError):
-        Desc2DTransformer(desc_list=['Color', 'Icecream content', 'ChokolateDarkness', 'Content42', 'MolWt'])
+        MolecularDescriptorTransformer(desc_list=['Color', 'Icecream content', 'ChokolateDarkness', 'Content42', 'MolWt'])
 
 
 
 def test_descriptor_transformer_parallel(mols_list, default_descriptor_transformer):
     default_descriptor_transformer.set_params(parallel=True)
     features = default_descriptor_transformer.transform(mols_list)
     assert(len(features) == len(mols_list))
     assert(len(features[0]) == len(Descriptors._descList))
     #Now with Rdkit 2022.3 creating a second transformer and running it, froze the process
-    transformer2 = Desc2DTransformer(**default_descriptor_transformer.get_params())
+    transformer2 = MolecularDescriptorTransformer(**default_descriptor_transformer.get_params())
     features2 = transformer2.transform(mols_list)
     assert(len(features2) == len(mols_list))
     assert(len(features2[0]) == len(Descriptors._descList))
 
 # This test may fail on windows and mac (due to spawn rather than fork?)
 # def test_descriptor_transformer_parallel_speedup(mols_list, default_descriptor_transformer):
 #     n_phys_cpus = joblib.cpu_count(only_physical_cores=True)
```

### Comparing `scikit_mol-0.1.2/tests/test_fptransformers.py` & `scikit_mol-0.2.0/tests/test_fptransformers.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,41 +2,47 @@
 import tempfile
 import pytest
 import numpy as np
 import pandas as pd
 from rdkit import Chem
 from fixtures import mols_list, smiles_list, fingerprint, chiral_smiles_list, chiral_mols_list
 from sklearn import clone
-from scikit_mol.transformers import MorganTransformer, MACCSTransformer, RDKitFPTransformer, AtomPairFingerprintTransformer, TopologicalTorsionFingerprintTransformer, SECFingerprintTransformer
+
+from scikit_mol.fingerprints import MorganFingerprintTransformer, MACCSKeysFingerprintTransformer, RDKitFingerprintTransformer, AtomPairFingerprintTransformer, TopologicalTorsionFingerprintTransformer, SECFingerprintTransformer, MHFingerprintTransformer
+
 
 
 @pytest.fixture
 def morgan_transformer():
-    return MorganTransformer()
+    return MorganFingerprintTransformer()
 
 @pytest.fixture
 def rdkit_transformer():
-    return RDKitFPTransformer()
+    return RDKitFingerprintTransformer()
 
 @pytest.fixture
 def atompair_transformer():
     return AtomPairFingerprintTransformer()
 
 @pytest.fixture
 def topologicaltorsion_transformer():
     return TopologicalTorsionFingerprintTransformer()
 
 @pytest.fixture
 def maccs_transformer():
-    return MACCSTransformer()
+    return MACCSKeysFingerprintTransformer()
 
 @pytest.fixture
 def secfp_transformer():
     return SECFingerprintTransformer()
 
+@pytest.fixture
+def mhfp_transformer():
+    return MHFingerprintTransformer()
+
 
 def test_fpstransformer_fp2array(morgan_transformer, fingerprint):
     fp = morgan_transformer._fp2array(fingerprint)
     #See that fp is the correct type, shape and bit count
     assert(type(fp) == type(np.array([0])))
     assert(fp.shape == (1000,))
     assert(fp.sum() == 25)
@@ -44,25 +50,25 @@
 def test_fpstransformer_transform_mol(morgan_transformer, mols_list):
     fp = morgan_transformer._transform_mol(mols_list[0])
     #See that fp is the correct type, shape and bit count
     assert(type(fp) == type(np.array([0])))
     assert(fp.shape == (2048,))
     assert(fp.sum() == 14)
 
-def test_clonability(maccs_transformer, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, secfp_transformer):
-    for t in [maccs_transformer, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, secfp_transformer]:
+def test_clonability(maccs_transformer, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, secfp_transformer, mhfp_transformer):
+    for t in [maccs_transformer, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, secfp_transformer, mhfp_transformer]:
         params   = t.get_params()
         t2 = clone(t)
         params_2 = t2.get_params()
         #Parameters of cloned transformers should be the same
         assert all([ params[key] == params_2[key] for key in params.keys()])
         #Cloned transformers should not be the same object
         assert t2 != t
 
-def test_set_params(morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, secfp_transformer):
+def test_set_params(morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, secfp_transformer, mhfp_transformer):
     for t in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer]:
         params   = t.get_params()
         #change extracted dictionary
         params['nBits'] = 4242
         #change params in transformer
         t.set_params(nBits = 4242)
         # get parameters as dictionary and assert that it is the same
@@ -79,54 +85,57 @@
     for t in [secfp_transformer]:
         params   = t.get_params()
         params['length'] = 4242
         t.set_params(length = 4242)
         params_2 = t.get_params()
         assert all([ params[key] == params_2[key] for key in params.keys()])
 
-def test_transform(mols_list, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, secfp_transformer):
+    for t in [mhfp_transformer]:
+        params   = t.get_params()
+        params['n_permutations'] = 4242
+        t.set_params(n_permutations = 4242)
+        params_2 = t.get_params()
+        assert all([ params[key] == params_2[key] for key in params.keys()])
+
+def test_transform(mols_list, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, secfp_transformer, mhfp_transformer):
     #Test different types of input
     for mols in [mols_list, np.array(mols_list), pd.Series(mols_list)]:
         #Test the different transformers
-        for t in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, rdkit_transformer, secfp_transformer]:
+        for t in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, rdkit_transformer, secfp_transformer, mhfp_transformer]:
             params   = t.get_params()
             fps = t.transform(mols)
             #Assert that the same length of input and output
             assert len(fps) == len(mols_list)
 
             # assert that the size of the fingerprint is the expected size
-            if type(t) == type(maccs_transformer):
+            if type(t) == type(maccs_transformer) or type(t) == type(secfp_transformer) or type(t) == type(mhfp_transformer):
                 fpsize = t.nBits
             elif type(t) == type(rdkit_transformer):
                 fpsize = params['fpSize']
-            elif type(t) == type(secfp_transformer):
-                fpsize = t.nBits
             else:
                 fpsize = params['nBits']
             
             assert len(fps[0]) == fpsize
 
-def test_transform_parallel(mols_list, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, secfp_transformer):
+def test_transform_parallel(mols_list, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, secfp_transformer, mhfp_transformer):
     #Test different types of input
     for mols in [mols_list, np.array(mols_list), pd.Series(mols_list)]:
         #Test the different transformers
-        for t in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, rdkit_transformer, secfp_transformer]:
+        for t in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, rdkit_transformer, secfp_transformer, mhfp_transformer]:
             t.set_params(parallel=True)
             params   = t.get_params()
             fps = t.transform(mols)
             #Assert that the same length of input and output
             assert len(fps) == len(mols_list)
 
             # assert that the size of the fingerprint is the expected size
-            if type(t) == type(maccs_transformer):
+            if type(t) == type(maccs_transformer) or type(t) == type(secfp_transformer) or type(t) == type(mhfp_transformer):
                 fpsize = t.nBits
             elif type(t) == type(rdkit_transformer):
                 fpsize = params['fpSize']
-            elif type(t) == type(secfp_transformer):
-                fpsize = t.nBits
             else:
                 fpsize = params['nBits']
             
             assert len(fps[0]) == fpsize
 
 
 def test_picklable(morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, secfp_transformer):
@@ -165,15 +174,15 @@
     new_params = {'nBits': 1024,
                 'radius': 1,
                 'useBondTypes': False,# TODO, why doesn't this change the FP?
                 'useChirality': True,
                 'useCounts': True,
                 'useFeatures': True}
     
-    assert_transformer_set_params(MorganTransformer, new_params, chiral_mols_list)
+    assert_transformer_set_params(MorganFingerprintTransformer, new_params, chiral_mols_list)
 
 
 def test_atompairs_set_params(chiral_mols_list):
     new_params = {
         #'atomInvariants': 1,
         #'confId': -1,
         #'fromAtoms': 1,
@@ -209,23 +218,34 @@
                 'fpSize': 1024,
                 'maxPath': 3,
                 'minPath': 2,
                 'numBitsPerFeature': 3,
                 'useBondOrder': False, #TODO, why doesn't this change the FP?
                 #'useHs': False, #TODO, why doesn't this change the FP?
                 }
-    assert_transformer_set_params(RDKitFPTransformer, new_params, chiral_mols_list)
+    assert_transformer_set_params(RDKitFingerprintTransformer, new_params, chiral_mols_list)
 
 
 def test_SECFingerprintTransformer(chiral_mols_list):
     new_params = {'isomeric': True,
                 'kekulize': True,
                 'length': 1048,
                 'min_radius': 2,
                 #'n_permutations': 2, # The SECFp is not using this setting
                 'radius': 2,
                 'rings': False,
                 #'seed': 1 # The SECFp is not using this setting
                 }
     assert_transformer_set_params(SECFingerprintTransformer, new_params, chiral_mols_list)
 
+def test_MHFingerprintTransformer(chiral_mols_list):
+    new_params = {'radius': 2,
+                'rings': False,
+                'isomeric': True,
+                'kekulize': True,
+                'min_radius': 2,
+                'n_permutations': 4096, 
+                'seed': 44
+                }
+    assert_transformer_set_params(MHFingerprintTransformer, new_params, chiral_mols_list)
+
```

### Comparing `scikit_mol-0.1.2/tests/test_sanitizer.py` & `scikit_mol-0.2.0/tests/test_sanitizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import numpy as np
 import pandas as pd
 from rdkit import Chem
 from fixtures import smiles_list, invalid_smiles_list
-from scikit_mol.sanitizer import CheckSmilesSanitazion
+from scikit_mol.utilities import CheckSmilesSanitazion
 
 @pytest.fixture
 def sanitizer():
     return CheckSmilesSanitazion()
 
 @pytest.fixture
 def return_mol_sanitizer():
```

### Comparing `scikit_mol-0.1.2/tests/test_smilestomol.py` & `scikit_mol-0.2.0/tests/test_smilestomol.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pytest
 import numpy as np
 import pandas as pd
 from sklearn import clone
 from rdkit import Chem
-from scikit_mol.transformers import SmilesToMol
+from scikit_mol.conversions import SmilesToMolTransformer
 from fixtures import smiles_list, invalid_smiles_list
 
 
 @pytest.fixture
 def smilestomol_transformer():
-    return SmilesToMol()
+    return SmilesToMolTransformer()
 
 def test_smilestomol(smiles_list, smilestomol_transformer):
     mol_list = smilestomol_transformer.transform(smiles_list)
     assert all([ a == b for a, b in zip(smiles_list, [Chem.MolToSmiles(mol) for mol in mol_list])])
 
 def test_smilestomol_numpy(smiles_list, smilestomol_transformer):
     mol_list = smilestomol_transformer.transform(np.array(smiles_list))
```

### Comparing `scikit_mol-0.1.2/tests/test_transformers.py` & `scikit_mol-0.2.0/tests/test_transformers.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,45 +6,49 @@
 # pytest tests/test_transformers.py --> tests/test_transformers.py::test_transformer PASSED
 
 
 import pytest
 import pandas as pd
 from sklearn.pipeline import Pipeline
 from sklearn.ensemble import RandomForestRegressor
-from scikit_mol.transformers import SmilesToMol
-from scikit_mol.transformers import MACCSTransformer, RDKitFPTransformer, AtomPairFingerprintTransformer, \
-                                    TopologicalTorsionFingerprintTransformer, MorganTransformer
+from scikit_mol.conversions import SmilesToMolTransformer
+from scikit_mol.fingerprints import MACCSKeysFingerprintTransformer, RDKitFingerprintTransformer, AtomPairFingerprintTransformer, \
+                                    TopologicalTorsionFingerprintTransformer, MorganFingerprintTransformer, SECFingerprintTransformer, \
+                                    MHFingerprintTransformer
+
 
 from fixtures import SLC6A4_subset
 
 def test_transformer(SLC6A4_subset):
     # load some toy data for quick testing on a small number of samples
     X_smiles, Y = SLC6A4_subset.SMILES, SLC6A4_subset.pXC50
     X_train, X_test = X_smiles[:128], X_smiles[128:]
     Y_train, Y_test = Y[:128], Y[128:]
 
     # run FP with default parameters except when useCounts can be given as an argument
-    FP_dict = {"MACCSTransformer": [MACCSTransformer, None],
-               "RDKitFPTransformer": [RDKitFPTransformer, None],
+    FP_dict = {"MACCSTransformer": [MACCSKeysFingerprintTransformer, None],
+               "RDKitFPTransformer": [RDKitFingerprintTransformer, None],
                "AtomPairFingerprintTransformer": [AtomPairFingerprintTransformer, False],
                "AtomPairFingerprintTransformer useCounts": [AtomPairFingerprintTransformer, True],
                "TopologicalTorsionFingerprintTransformer": [TopologicalTorsionFingerprintTransformer, False],
                "TopologicalTorsionFingerprintTransformer useCounts": [TopologicalTorsionFingerprintTransformer, True],
-               "MorganTransformer": [MorganTransformer, False],
-               "MorganTransformer useCounts": [MorganTransformer, True]}
+               "MorganTransformer": [MorganFingerprintTransformer, False],
+               "MorganTransformer useCounts": [MorganFingerprintTransformer, True],
+               "SECFingerprintTransformer": [SECFingerprintTransformer, None],
+               "MHFingerprintTransformer": [MHFingerprintTransformer, None]}
 
     # fit on toy data and print train/test score if successful or collect the failed FP
     failed_FP = []
     for FP_name, (FP, useCounts) in FP_dict.items():
         try:
             print(f"\nrunning pipeline fitting and scoring for {FP_name} with useCounts={useCounts}")
             if useCounts is None:
-                pipeline = Pipeline([("s2m", SmilesToMol()), ("FP", FP()), ("RF", RandomForestRegressor())])
+                pipeline = Pipeline([("s2m", SmilesToMolTransformer()), ("FP", FP()), ("RF", RandomForestRegressor())])
             else:
-                pipeline = Pipeline([("s2m", SmilesToMol()), ("FP", FP(useCounts=useCounts)), ("RF", RandomForestRegressor())])
+                pipeline = Pipeline([("s2m", SmilesToMolTransformer()), ("FP", FP(useCounts=useCounts)), ("RF", RandomForestRegressor())])
             pipeline.fit(X_train, Y_train)
             train_score = pipeline.score(X_train, Y_train)
             test_score = pipeline.score(X_test, Y_test)
             print(f"\nfitting and scoring completed train_score={train_score}, test_score={test_score}")
         except:
             print(f"\n!!!! FAILED pipeline fitting and scoring for {FP_name} with useCounts={useCounts}")
             failed_FP.append(FP_name)
```

