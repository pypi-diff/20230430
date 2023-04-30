# Comparing `tmp/fmldk-1.1.9.tar.gz` & `tmp/fmldk-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmldk-1.1.9.tar", last modified: Wed Apr 26 08:01:25 2023, max compression
+gzip compressed data, was "fmldk-1.2.0.tar", last modified: Sun Apr 30 08:07:00 2023, max compression
```

## Comparing `fmldk-1.1.9.tar` & `fmldk-1.2.0.tar`

### file list

```diff
@@ -1,78 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:25.819284 fmldk-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)    28116 2023-04-26 08:01:25.819284 fmldk-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27938 2023-04-26 08:01:12.000000 fmldk-1.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:25.807284 fmldk-1.1.9/ctfr/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55520 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfr/ctfr_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfr/ctfr_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfr/ctfr_losses_bkp.py
--rw-r--r--   0 runner    (1001) docker     (123)   113137 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfr/ctfr_models.py
--rw-r--r--   0 runner    (1001) docker     (123)   105725 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfr/ctfr_models_v0.1.29.py
--rw-r--r--   0 runner    (1001) docker     (123)   111862 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfr/ctfr_models_v0.1.31.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:25.807284 fmldk-1.1.9/ctfrv2/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfrv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55580 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfrv2/ctfrv2_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    42022 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfrv2/ctfrv2_global_scaled_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfrv2/ctfrv2_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    86435 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfrv2/ctfrv2_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:25.807284 fmldk-1.1.9/eda/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-26 08:01:12.000000 fmldk-1.1.9/eda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38969 2023-04-26 08:01:12.000000 fmldk-1.1.9/eda/eda_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-04-26 08:01:12.000000 fmldk-1.1.9/eda/eda_lib_v0.1.18.py
--rw-r--r--   0 runner    (1001) docker     (123)    22984 2023-04-26 08:01:12.000000 fmldk-1.1.9/eda/eda_lib_v0.1.19.py
--rw-r--r--   0 runner    (1001) docker     (123)    34650 2023-04-26 08:01:12.000000 fmldk-1.1.9/eda/eda_lib_v0.1.37.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:25.807284 fmldk-1.1.9/fmldk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28116 2023-04-26 08:01:25.000000 fmldk-1.1.9/fmldk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-26 08:01:25.000000 fmldk-1.1.9/fmldk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:01:25.000000 fmldk-1.1.9/fmldk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 08:01:25.000000 fmldk-1.1.9/fmldk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-26 08:01:25.000000 fmldk-1.1.9/fmldk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:25.811284 fmldk-1.1.9/sage/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-26 08:01:12.000000 fmldk-1.1.9/sage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46583 2023-04-26 08:01:12.000000 fmldk-1.1.9/sage/sage_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    42404 2023-04-26 08:01:12.000000 fmldk-1.1.9/sage/sage_data_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    42020 2023-04-26 08:01:12.000000 fmldk-1.1.9/sage/sage_global_scaled_data_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-04-26 08:01:12.000000 fmldk-1.1.9/sage/sage_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-04-26 08:01:12.000000 fmldk-1.1.9/sage/sage_losses_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    86777 2023-04-26 08:01:12.000000 fmldk-1.1.9/sage/sage_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    83909 2023-04-26 08:01:12.000000 fmldk-1.1.9/sage/sage_model_old.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:01:25.819284 fmldk-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-26 08:01:12.000000 fmldk-1.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:25.811284 fmldk-1.1.9/stctn/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-26 08:01:12.000000 fmldk-1.1.9/stctn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55190 2023-04-26 08:01:12.000000 fmldk-1.1.9/stctn/stctn_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-04-26 08:01:12.000000 fmldk-1.1.9/stctn/stctn_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-04-26 08:01:12.000000 fmldk-1.1.9/stctn/stctn_losses_bkp.py
--rw-r--r--   0 runner    (1001) docker     (123)    53648 2023-04-26 08:01:12.000000 fmldk-1.1.9/stctn/stctn_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:25.815284 fmldk-1.1.9/tfr/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55577 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_data_v0.1.11.py
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_data_v0.1.12.py
--rw-r--r--   0 runner    (1001) docker     (123)    37924 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_data_v0.1.14.py
--rw-r--r--   0 runner    (1001) docker     (123)    40021 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_data_v0.1.15.py
--rw-r--r--   0 runner    (1001) docker     (123)    46425 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_data_v0.1.16.py
--rw-r--r--   0 runner    (1001) docker     (123)    54017 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_data_v0.1.18.py
--rw-r--r--   0 runner    (1001) docker     (123)    55773 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_data_v0.1.21.py
--rw-r--r--   0 runner    (1001) docker     (123)   107319 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_local_block_sparse_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    93067 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_local_block_sparse_attention_v0.1.10.py
--rw-r--r--   0 runner    (1001) docker     (123)    97067 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_local_block_sparse_attention_v0.1.12.py
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_losses_bkp.py
--rw-r--r--   0 runner    (1001) docker     (123)   113988 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    96299 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_models_v0.1.10.py
--rw-r--r--   0 runner    (1001) docker     (123)   100101 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_models_v0.1.11.py
--rw-r--r--   0 runner    (1001) docker     (123)   109483 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_models_v0.1.23.py
--rw-r--r--   0 runner    (1001) docker     (123)   114250 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_models_v0.1.31.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:25.819284 fmldk-1.1.9/tft/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46581 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    42403 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_data_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    55578 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_data_v1.1.3.py
--rw-r--r--   0 runner    (1001) docker     (123)    62667 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_data_v1.1.7.py
--rw-r--r--   0 runner    (1001) docker     (123)    42019 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_global_scaled_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    84122 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    64043 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_model_v0.1.26.py
--rw-r--r--   0 runner    (1001) docker     (123)    65090 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_model_v0.1.31.py
--rw-r--r--   0 runner    (1001) docker     (123)    73433 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_model_v1.1.3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:07:00.589748 fmldk-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-04-30 08:07:00.589748 fmldk-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30262 2023-04-30 08:06:49.000000 fmldk-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:07:00.577748 fmldk-1.2.0/ctfr/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-30 08:06:49.000000 fmldk-1.2.0/ctfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55520 2023-04-30 08:06:49.000000 fmldk-1.2.0/ctfr/ctfr_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-04-30 08:06:49.000000 fmldk-1.2.0/ctfr/ctfr_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-04-30 08:06:49.000000 fmldk-1.2.0/ctfr/ctfr_losses_bkp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113137 2023-04-30 08:06:49.000000 fmldk-1.2.0/ctfr/ctfr_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105725 2023-04-30 08:06:49.000000 fmldk-1.2.0/ctfr/ctfr_models_v0.1.29.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111862 2023-04-30 08:06:49.000000 fmldk-1.2.0/ctfr/ctfr_models_v0.1.31.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:07:00.581748 fmldk-1.2.0/ctfrv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-30 08:06:49.000000 fmldk-1.2.0/ctfrv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55580 2023-04-30 08:06:49.000000 fmldk-1.2.0/ctfrv2/ctfrv2_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42022 2023-04-30 08:06:49.000000 fmldk-1.2.0/ctfrv2/ctfrv2_global_scaled_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-04-30 08:06:49.000000 fmldk-1.2.0/ctfrv2/ctfrv2_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86435 2023-04-30 08:06:49.000000 fmldk-1.2.0/ctfrv2/ctfrv2_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:07:00.581748 fmldk-1.2.0/ctfrv2_gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-30 08:06:49.000000 fmldk-1.2.0/ctfrv2_gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36385 2023-04-30 08:06:49.000000 fmldk-1.2.0/ctfrv2_gpu/ctfrv2_data_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-04-30 08:06:49.000000 fmldk-1.2.0/ctfrv2_gpu/ctfrv2_losses_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78757 2023-04-30 08:06:49.000000 fmldk-1.2.0/ctfrv2_gpu/ctfrv2_model_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:07:00.581748 fmldk-1.2.0/eda/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-30 08:06:49.000000 fmldk-1.2.0/eda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38969 2023-04-30 08:06:49.000000 fmldk-1.2.0/eda/eda_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-04-30 08:06:49.000000 fmldk-1.2.0/eda/eda_lib_v0.1.18.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22984 2023-04-30 08:06:49.000000 fmldk-1.2.0/eda/eda_lib_v0.1.19.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34650 2023-04-30 08:06:49.000000 fmldk-1.2.0/eda/eda_lib_v0.1.37.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:07:00.581748 fmldk-1.2.0/fmldk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-04-30 08:07:00.000000 fmldk-1.2.0/fmldk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-30 08:07:00.000000 fmldk-1.2.0/fmldk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 08:07:00.000000 fmldk-1.2.0/fmldk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-30 08:07:00.000000 fmldk-1.2.0/fmldk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-30 08:07:00.000000 fmldk-1.2.0/fmldk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:07:00.581748 fmldk-1.2.0/sage/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-30 08:06:49.000000 fmldk-1.2.0/sage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46583 2023-04-30 08:06:49.000000 fmldk-1.2.0/sage/sage_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42404 2023-04-30 08:06:49.000000 fmldk-1.2.0/sage/sage_data_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42020 2023-04-30 08:06:49.000000 fmldk-1.2.0/sage/sage_global_scaled_data_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-04-30 08:06:49.000000 fmldk-1.2.0/sage/sage_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-04-30 08:06:49.000000 fmldk-1.2.0/sage/sage_losses_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86777 2023-04-30 08:06:49.000000 fmldk-1.2.0/sage/sage_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83909 2023-04-30 08:06:49.000000 fmldk-1.2.0/sage/sage_model_old.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:07:00.585748 fmldk-1.2.0/sage_gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-30 08:06:49.000000 fmldk-1.2.0/sage_gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36366 2023-04-30 08:06:49.000000 fmldk-1.2.0/sage_gpu/sage_data_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-04-30 08:06:49.000000 fmldk-1.2.0/sage_gpu/sage_losses_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87798 2023-04-30 08:06:49.000000 fmldk-1.2.0/sage_gpu/sage_model_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 08:07:00.589748 fmldk-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-30 08:06:49.000000 fmldk-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:07:00.585748 fmldk-1.2.0/stctn/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-30 08:06:49.000000 fmldk-1.2.0/stctn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55190 2023-04-30 08:06:49.000000 fmldk-1.2.0/stctn/stctn_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-04-30 08:06:49.000000 fmldk-1.2.0/stctn/stctn_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-04-30 08:06:49.000000 fmldk-1.2.0/stctn/stctn_losses_bkp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53648 2023-04-30 08:06:49.000000 fmldk-1.2.0/stctn/stctn_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:07:00.589748 fmldk-1.2.0/tfr/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55577 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/tfr_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/tfr_data_v0.1.11.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/tfr_data_v0.1.12.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37924 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/tfr_data_v0.1.14.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40021 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/tfr_data_v0.1.15.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46425 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/tfr_data_v0.1.16.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54017 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/tfr_data_v0.1.18.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55773 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/tfr_data_v0.1.21.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107319 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/tfr_local_block_sparse_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93067 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/tfr_local_block_sparse_attention_v0.1.10.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97067 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/tfr_local_block_sparse_attention_v0.1.12.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/tfr_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/tfr_losses_bkp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113988 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/tfr_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96299 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/tfr_models_v0.1.10.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100101 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/tfr_models_v0.1.11.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109483 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/tfr_models_v0.1.23.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114250 2023-04-30 08:06:49.000000 fmldk-1.2.0/tfr/tfr_models_v0.1.31.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:07:00.589748 fmldk-1.2.0/tft/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-30 08:06:49.000000 fmldk-1.2.0/tft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46581 2023-04-30 08:06:49.000000 fmldk-1.2.0/tft/tft_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42403 2023-04-30 08:06:49.000000 fmldk-1.2.0/tft/tft_data_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55578 2023-04-30 08:06:49.000000 fmldk-1.2.0/tft/tft_data_v1.1.3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62667 2023-04-30 08:06:49.000000 fmldk-1.2.0/tft/tft_data_v1.1.7.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42019 2023-04-30 08:06:49.000000 fmldk-1.2.0/tft/tft_global_scaled_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-04-30 08:06:49.000000 fmldk-1.2.0/tft/tft_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84122 2023-04-30 08:06:49.000000 fmldk-1.2.0/tft/tft_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64043 2023-04-30 08:06:49.000000 fmldk-1.2.0/tft/tft_model_v0.1.26.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65090 2023-04-30 08:06:49.000000 fmldk-1.2.0/tft/tft_model_v0.1.31.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73433 2023-04-30 08:06:49.000000 fmldk-1.2.0/tft/tft_model_v1.1.3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:07:00.589748 fmldk-1.2.0/tft_gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-30 08:06:49.000000 fmldk-1.2.0/tft_gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36382 2023-04-30 08:06:49.000000 fmldk-1.2.0/tft_gpu/tft_data_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-04-30 08:06:49.000000 fmldk-1.2.0/tft_gpu/tft_losses_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78604 2023-04-30 08:06:49.000000 fmldk-1.2.0/tft_gpu/tft_model_gpu.py
```

### Comparing `fmldk-1.1.9/PKG-INFO` & `fmldk-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmldk
-Version: 1.1.9
+Version: 1.2.0
 Summary: Forecast ML library
 Author: Rahul Sinha
 Author-email: rahul.sinha@unilever.com
 Description-Content-Type: text/markdown
 
 ### A library to easily build & train Transformer models for forecasting.
 
@@ -559,8 +559,59 @@
             opt=None,                  # provide own optimizer object (default is Adam/Nadam)             
             clipnorm=0.1,              # max global norm applied. Used for stable training. Default is 'None'.
             min_delta=0.0001,          # Min decrease in validation loss to consider an epoch as improvement
             shuffle=True)              # shuffle train dataset after each epoch
 
 # Inference Steps are similar to TFT or CTFRV2 models
 
+
+````
+### Static Dataset & Options for Reproducibility
+
+### Packages ctfrv2_gpu, tft_gpu, sage_gpu contain dataset api for GPU based, reproducible model training.
+
+#### sample usage 
+````
+data_obj = [tft_gpu | sage_gpu | ctfrv2_gpu].[tft | sage | ctfrv2]_dataset(col_dict=model_columns_dict, 
+                               window_len=int(120), 
+                               fh=int(28), 
+                               batch=32, 
+                               min_nz=1,
+                               max_per_key_train_samples=110,
+                               max_per_key_test_samples=20,
+                               scaling_method='mean_scaling',
+                               interleave=1,
+                               PARALLEL_DATA_JOBS=6, 
+                               PARALLEL_DATA_JOBS_BATCHSIZE=128)
+
+where,
+ batch: no. of unique ids to process at a time
+ max_per_key_train_samples, max_per_key_test_samples: Max samples to extract from a single time series (default: -1, will extract all possible samples. For e.g. if the timeseries has 100 data points & a window_len of 50 is used, 100 - 50 = 50 samples will be extracted by default)
+ scaling_method: mean, standard & no (external) scaling supported
+
+````
+### Models take additional args -- seed & deterministic_ops - for deterministic behaviour with some performance penalty
+
+#### sample usage with sage (also available in tft, tft_gpu, ctfrv2_gpu packages)
+````
+model = sage_gpu.SageModel(col_index_dict = col_index_dict,
+                       vocab_dict = vocab,
+                       num_layers = 1,
+                       num_heads = 4,
+                       kernel_sizes = [1],
+                       d_model = 64,
+                       forecast_horizon = int(24),
+                       max_inp_len = int(168),
+                       loss_type = 'Quantile',
+                       num_quantiles = 1,                
+                       dropout_rate = 0.1,
+                       seed = <int>,
+                       deterministic_ops = [True | False])
+````
+### Tweedie loss fn. & a revised Poisson loss fn. available
+
+#### sample usage
+````
+Poisson: ['loss_type: Poisson', 'Usage: Poisson_Loss(log_scale=False, sample_weights=False)']
+Tweedie: ['loss_type: Tweedie', 'Usage: Tweedie_Loss(p=1.5, log_scale=False, sample_weights=False)']
+
 ````
```

### Comparing `fmldk-1.1.9/README.md` & `fmldk-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -551,8 +551,59 @@
             opt=None,                  # provide own optimizer object (default is Adam/Nadam)             
             clipnorm=0.1,              # max global norm applied. Used for stable training. Default is 'None'.
             min_delta=0.0001,          # Min decrease in validation loss to consider an epoch as improvement
             shuffle=True)              # shuffle train dataset after each epoch
 
 # Inference Steps are similar to TFT or CTFRV2 models
 
+
+````
+### Static Dataset & Options for Reproducibility
+
+### Packages ctfrv2_gpu, tft_gpu, sage_gpu contain dataset api for GPU based, reproducible model training.
+
+#### sample usage 
+````
+data_obj = [tft_gpu | sage_gpu | ctfrv2_gpu].[tft | sage | ctfrv2]_dataset(col_dict=model_columns_dict, 
+                               window_len=int(120), 
+                               fh=int(28), 
+                               batch=32, 
+                               min_nz=1,
+                               max_per_key_train_samples=110,
+                               max_per_key_test_samples=20,
+                               scaling_method='mean_scaling',
+                               interleave=1,
+                               PARALLEL_DATA_JOBS=6, 
+                               PARALLEL_DATA_JOBS_BATCHSIZE=128)
+
+where,
+ batch: no. of unique ids to process at a time
+ max_per_key_train_samples, max_per_key_test_samples: Max samples to extract from a single time series (default: -1, will extract all possible samples. For e.g. if the timeseries has 100 data points & a window_len of 50 is used, 100 - 50 = 50 samples will be extracted by default)
+ scaling_method: mean, standard & no (external) scaling supported
+
+````
+### Models take additional args -- seed & deterministic_ops - for deterministic behaviour with some performance penalty
+
+#### sample usage with sage (also available in tft, tft_gpu, ctfrv2_gpu packages)
+````
+model = sage_gpu.SageModel(col_index_dict = col_index_dict,
+                       vocab_dict = vocab,
+                       num_layers = 1,
+                       num_heads = 4,
+                       kernel_sizes = [1],
+                       d_model = 64,
+                       forecast_horizon = int(24),
+                       max_inp_len = int(168),
+                       loss_type = 'Quantile',
+                       num_quantiles = 1,                
+                       dropout_rate = 0.1,
+                       seed = <int>,
+                       deterministic_ops = [True | False])
+````
+### Tweedie loss fn. & a revised Poisson loss fn. available
+
+#### sample usage
+````
+Poisson: ['loss_type: Poisson', 'Usage: Poisson_Loss(log_scale=False, sample_weights=False)']
+Tweedie: ['loss_type: Tweedie', 'Usage: Tweedie_Loss(p=1.5, log_scale=False, sample_weights=False)']
+
 ````
```

### Comparing `fmldk-1.1.9/ctfr/ctfr_data.py` & `fmldk-1.2.0/ctfr/ctfr_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/ctfr/ctfr_losses.py` & `fmldk-1.2.0/ctfr/ctfr_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/ctfr/ctfr_losses_bkp.py` & `fmldk-1.2.0/ctfr/ctfr_losses_bkp.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/ctfr/ctfr_models.py` & `fmldk-1.2.0/ctfr/ctfr_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/ctfr/ctfr_models_v0.1.29.py` & `fmldk-1.2.0/ctfr/ctfr_models_v0.1.29.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/ctfr/ctfr_models_v0.1.31.py` & `fmldk-1.2.0/ctfr/ctfr_models_v0.1.31.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/ctfrv2/ctfrv2_data.py` & `fmldk-1.2.0/ctfrv2/ctfrv2_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/ctfrv2/ctfrv2_global_scaled_data.py` & `fmldk-1.2.0/ctfrv2/ctfrv2_global_scaled_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/ctfrv2/ctfrv2_losses.py` & `fmldk-1.2.0/ctfrv2/ctfrv2_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/ctfrv2/ctfrv2_models.py` & `fmldk-1.2.0/ctfrv2/ctfrv2_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/eda/eda_lib.py` & `fmldk-1.2.0/eda/eda_lib.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/eda/eda_lib_v0.1.18.py` & `fmldk-1.2.0/eda/eda_lib_v0.1.18.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/eda/eda_lib_v0.1.19.py` & `fmldk-1.2.0/eda/eda_lib_v0.1.19.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/eda/eda_lib_v0.1.37.py` & `fmldk-1.2.0/eda/eda_lib_v0.1.37.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/fmldk.egg-info/PKG-INFO` & `fmldk-1.2.0/fmldk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmldk
-Version: 1.1.9
+Version: 1.2.0
 Summary: Forecast ML library
 Author: Rahul Sinha
 Author-email: rahul.sinha@unilever.com
 Description-Content-Type: text/markdown
 
 ### A library to easily build & train Transformer models for forecasting.
 
@@ -559,8 +559,59 @@
             opt=None,                  # provide own optimizer object (default is Adam/Nadam)             
             clipnorm=0.1,              # max global norm applied. Used for stable training. Default is 'None'.
             min_delta=0.0001,          # Min decrease in validation loss to consider an epoch as improvement
             shuffle=True)              # shuffle train dataset after each epoch
 
 # Inference Steps are similar to TFT or CTFRV2 models
 
+
+````
+### Static Dataset & Options for Reproducibility
+
+### Packages ctfrv2_gpu, tft_gpu, sage_gpu contain dataset api for GPU based, reproducible model training.
+
+#### sample usage 
+````
+data_obj = [tft_gpu | sage_gpu | ctfrv2_gpu].[tft | sage | ctfrv2]_dataset(col_dict=model_columns_dict, 
+                               window_len=int(120), 
+                               fh=int(28), 
+                               batch=32, 
+                               min_nz=1,
+                               max_per_key_train_samples=110,
+                               max_per_key_test_samples=20,
+                               scaling_method='mean_scaling',
+                               interleave=1,
+                               PARALLEL_DATA_JOBS=6, 
+                               PARALLEL_DATA_JOBS_BATCHSIZE=128)
+
+where,
+ batch: no. of unique ids to process at a time
+ max_per_key_train_samples, max_per_key_test_samples: Max samples to extract from a single time series (default: -1, will extract all possible samples. For e.g. if the timeseries has 100 data points & a window_len of 50 is used, 100 - 50 = 50 samples will be extracted by default)
+ scaling_method: mean, standard & no (external) scaling supported
+
+````
+### Models take additional args -- seed & deterministic_ops - for deterministic behaviour with some performance penalty
+
+#### sample usage with sage (also available in tft, tft_gpu, ctfrv2_gpu packages)
+````
+model = sage_gpu.SageModel(col_index_dict = col_index_dict,
+                       vocab_dict = vocab,
+                       num_layers = 1,
+                       num_heads = 4,
+                       kernel_sizes = [1],
+                       d_model = 64,
+                       forecast_horizon = int(24),
+                       max_inp_len = int(168),
+                       loss_type = 'Quantile',
+                       num_quantiles = 1,                
+                       dropout_rate = 0.1,
+                       seed = <int>,
+                       deterministic_ops = [True | False])
+````
+### Tweedie loss fn. & a revised Poisson loss fn. available
+
+#### sample usage
+````
+Poisson: ['loss_type: Poisson', 'Usage: Poisson_Loss(log_scale=False, sample_weights=False)']
+Tweedie: ['loss_type: Tweedie', 'Usage: Tweedie_Loss(p=1.5, log_scale=False, sample_weights=False)']
+
 ````
```

### Comparing `fmldk-1.1.9/fmldk.egg-info/SOURCES.txt` & `fmldk-1.2.0/fmldk.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 ctfr/ctfr_models_v0.1.29.py
 ctfr/ctfr_models_v0.1.31.py
 ctfrv2/__init__.py
 ctfrv2/ctfrv2_data.py
 ctfrv2/ctfrv2_global_scaled_data.py
 ctfrv2/ctfrv2_losses.py
 ctfrv2/ctfrv2_models.py
+ctfrv2_gpu/__init__.py
+ctfrv2_gpu/ctfrv2_data_gpu.py
+ctfrv2_gpu/ctfrv2_losses_gpu.py
+ctfrv2_gpu/ctfrv2_model_gpu.py
 eda/__init__.py
 eda/eda_lib.py
 eda/eda_lib_v0.1.18.py
 eda/eda_lib_v0.1.19.py
 eda/eda_lib_v0.1.37.py
 fmldk.egg-info/PKG-INFO
 fmldk.egg-info/SOURCES.txt
@@ -26,14 +30,18 @@
 sage/sage_data.py
 sage/sage_data_old.py
 sage/sage_global_scaled_data_old.py
 sage/sage_losses.py
 sage/sage_losses_old.py
 sage/sage_model.py
 sage/sage_model_old.py
+sage_gpu/__init__.py
+sage_gpu/sage_data_gpu.py
+sage_gpu/sage_losses_gpu.py
+sage_gpu/sage_model_gpu.py
 stctn/__init__.py
 stctn/stctn_data.py
 stctn/stctn_losses.py
 stctn/stctn_losses_bkp.py
 stctn/stctn_models.py
 tfr/__init__.py
 tfr/tfr_data.py
@@ -60,8 +68,12 @@
 tft/tft_data_v1.1.3.py
 tft/tft_data_v1.1.7.py
 tft/tft_global_scaled_data.py
 tft/tft_losses.py
 tft/tft_model.py
 tft/tft_model_v0.1.26.py
 tft/tft_model_v0.1.31.py
-tft/tft_model_v1.1.3.py
+tft/tft_model_v1.1.3.py
+tft_gpu/__init__.py
+tft_gpu/tft_data_gpu.py
+tft_gpu/tft_losses_gpu.py
+tft_gpu/tft_model_gpu.py
```

### Comparing `fmldk-1.1.9/sage/sage_data.py` & `fmldk-1.2.0/sage/sage_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/sage/sage_data_old.py` & `fmldk-1.2.0/sage/sage_data_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/sage/sage_global_scaled_data_old.py` & `fmldk-1.2.0/sage/sage_global_scaled_data_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/sage/sage_losses.py` & `fmldk-1.2.0/sage/sage_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/sage/sage_losses_old.py` & `fmldk-1.2.0/sage/sage_losses_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/sage/sage_model.py` & `fmldk-1.2.0/sage/sage_model.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/sage/sage_model_old.py` & `fmldk-1.2.0/sage/sage_model_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/setup.py` & `fmldk-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 # The directory containing this file
 this_directory = Path(__file__).parent
 long_description  = (this_directory / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="fmldk",
-    version="1.1.9",
+    version="1.2.0",
     description="Forecast ML library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Rahul Sinha",
     author_email="rahul.sinha@unilever.com",
-    packages=["sage","tfr","tft","stctn","ctfr","ctfrv2","eda"],
+    packages=["sage","sage_gpu","tfr","tft","tft_gpu","stctn","ctfr","ctfrv2","ctfrv2_gpu","eda"],
     include_package_data=True,
     install_requires=["tensorflow", "tensorflow_probability", "numpy", "statsmodels", "pandas", "joblib", "pathlib",
                       "bokeh", "holoviews", "hvplot", "ennemi"]
 )
```

### Comparing `fmldk-1.1.9/stctn/stctn_data.py` & `fmldk-1.2.0/stctn/stctn_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/stctn/stctn_losses.py` & `fmldk-1.2.0/stctn/stctn_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/stctn/stctn_losses_bkp.py` & `fmldk-1.2.0/stctn/stctn_losses_bkp.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/stctn/stctn_models.py` & `fmldk-1.2.0/stctn/stctn_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tfr/tfr_data.py` & `fmldk-1.2.0/tfr/tfr_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tfr/tfr_data_v0.1.11.py` & `fmldk-1.2.0/tfr/tfr_data_v0.1.11.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tfr/tfr_data_v0.1.12.py` & `fmldk-1.2.0/tfr/tfr_data_v0.1.12.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tfr/tfr_data_v0.1.14.py` & `fmldk-1.2.0/tfr/tfr_data_v0.1.14.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tfr/tfr_data_v0.1.15.py` & `fmldk-1.2.0/tfr/tfr_data_v0.1.15.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tfr/tfr_data_v0.1.16.py` & `fmldk-1.2.0/tfr/tfr_data_v0.1.16.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tfr/tfr_data_v0.1.18.py` & `fmldk-1.2.0/tfr/tfr_data_v0.1.18.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tfr/tfr_data_v0.1.21.py` & `fmldk-1.2.0/tfr/tfr_data_v0.1.21.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tfr/tfr_local_block_sparse_attention.py` & `fmldk-1.2.0/tfr/tfr_local_block_sparse_attention.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tfr/tfr_local_block_sparse_attention_v0.1.10.py` & `fmldk-1.2.0/tfr/tfr_local_block_sparse_attention_v0.1.10.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tfr/tfr_local_block_sparse_attention_v0.1.12.py` & `fmldk-1.2.0/tfr/tfr_local_block_sparse_attention_v0.1.12.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tfr/tfr_losses.py` & `fmldk-1.2.0/tfr/tfr_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tfr/tfr_losses_bkp.py` & `fmldk-1.2.0/tfr/tfr_losses_bkp.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tfr/tfr_models.py` & `fmldk-1.2.0/tfr/tfr_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tfr/tfr_models_v0.1.10.py` & `fmldk-1.2.0/tfr/tfr_models_v0.1.10.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tfr/tfr_models_v0.1.11.py` & `fmldk-1.2.0/tfr/tfr_models_v0.1.11.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tfr/tfr_models_v0.1.23.py` & `fmldk-1.2.0/tfr/tfr_models_v0.1.23.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tfr/tfr_models_v0.1.31.py` & `fmldk-1.2.0/tfr/tfr_models_v0.1.31.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tft/tft_data.py` & `fmldk-1.2.0/tft/tft_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tft/tft_data_old.py` & `fmldk-1.2.0/tft/tft_data_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tft/tft_data_v1.1.3.py` & `fmldk-1.2.0/tft/tft_data_v1.1.3.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tft/tft_data_v1.1.7.py` & `fmldk-1.2.0/tft/tft_data_v1.1.7.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tft/tft_global_scaled_data.py` & `fmldk-1.2.0/tft/tft_global_scaled_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tft/tft_losses.py` & `fmldk-1.2.0/tft/tft_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tft/tft_model.py` & `fmldk-1.2.0/tft/tft_model.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tft/tft_model_v0.1.26.py` & `fmldk-1.2.0/tft/tft_model_v0.1.26.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tft/tft_model_v0.1.31.py` & `fmldk-1.2.0/tft/tft_model_v0.1.31.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.9/tft/tft_model_v1.1.3.py` & `fmldk-1.2.0/tft/tft_model_v1.1.3.py`

 * *Files identical despite different names*

