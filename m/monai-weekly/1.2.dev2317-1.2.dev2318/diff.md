# Comparing `tmp/monai-weekly-1.2.dev2317.tar.gz` & `tmp/monai-weekly-1.2.dev2318.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monai-weekly-1.2.dev2317.tar", last modified: Sun Apr 23 02:24:34 2023, max compression
+gzip compressed data, was "monai-weekly-1.2.dev2318.tar", last modified: Sun Apr 30 02:19:55 2023, max compression
```

## Comparing `monai-weekly-1.2.dev2317.tar` & `monai-weekly-1.2.dev2318.tar`

### file list

```diff
@@ -1,1133 +1,1134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.931623 monai-weekly-1.2.dev2317/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-23 02:24:34.931623 monai-weekly-1.2.dev2317/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.935623 monai-weekly-1.2.dev2317/monai/
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-23 02:22:48.000000 monai-weekly-1.2.dev2317/monai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.475618 monai-weekly-1.2.dev2317/monai/_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.475618 monai-weekly-1.2.dev2317/monai/_extensions/gmm/
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm.h
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm_cuda_linalg.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/_extensions/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-23 02:24:34.935623 monai-weekly-1.2.dev2317/monai/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.479619 monai-weekly-1.2.dev2317/monai/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.483619 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37105 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/auto_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    26014 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/bundle_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/data_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    23351 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/ensemble_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17523 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/hpo_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34568 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.487619 monai-weekly-1.2.dev2317/monai/apps/deepedit/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/deepedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/deepedit/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    37435 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/deepedit/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.487619 monai-weekly-1.2.dev2317/monai/apps/deepgrow/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/deepgrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/deepgrow/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/deepgrow/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    42011 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/deepgrow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.487619 monai-weekly-1.2.dev2317/monai/apps/detection/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.491619 monai-weekly-1.2.dev2317/monai/apps/detection/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26617 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/metrics/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/metrics/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.491619 monai-weekly-1.2.dev2317/monai/apps/detection/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53221 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/networks/retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    18850 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/networks/retinanet_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.495619 monai-weekly-1.2.dev2317/monai/apps/detection/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24519 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    17916 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/transforms/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    68979 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.499619 monai-weekly-1.2.dev2317/monai/apps/detection/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/utils/ATSS_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18681 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/utils/anchor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/utils/box_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/utils/box_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/utils/detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/utils/hard_negative_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/utils/predict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.499619 monai-weekly-1.2.dev2317/monai/apps/mmars/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/mmars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/mmars/mmars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/mmars/model_desc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.503619 monai-weekly-1.2.dev2317/monai/apps/nnunet/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/nnunet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/nnunet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38587 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/nnunet/nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/nnunet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.503619 monai-weekly-1.2.dev2317/monai/apps/nuclick/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/nuclick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/nuclick/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.503619 monai-weekly-1.2.dev2317/monai/apps/pathology/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.503619 monai-weekly-1.2.dev2317/monai/apps/pathology/engines/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/engines/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.507619 monai-weekly-1.2.dev2317/monai/apps/pathology/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/handlers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.507619 monai-weekly-1.2.dev2317/monai/apps/pathology/inferers/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/inferers/inferer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.507619 monai-weekly-1.2.dev2317/monai/apps/pathology/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/losses/hovernet_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.507619 monai-weekly-1.2.dev2317/monai/apps/pathology/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/metrics/lesion_froc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.507619 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.511619 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37322 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.511619 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/stain/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/stain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/stain/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/stain/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.511619 monai-weekly-1.2.dev2317/monai/apps/reconstruction/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/mri_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.511619 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.515619 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/blocks/varnetblock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.515619 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/complex_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/varnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.515619 monai-weekly-1.2.dev2317/monai/apps/reconstruction/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    15844 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.519619 monai-weekly-1.2.dev2317/monai/apps/tcia/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/tcia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/tcia/label_desc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/tcia/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.519619 monai-weekly-1.2.dev2317/monai/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/auto3dseg/algo_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    41223 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/auto3dseg/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/auto3dseg/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/auto3dseg/seg_summarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12193 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/auto3dseg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.523619 monai-weekly-1.2.dev2317/monai/bundle/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/bundle/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16035 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/bundle/config_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/bundle/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/bundle/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/bundle/reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    63940 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/bundle/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/bundle/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/bundle/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.527619 monai-weekly-1.2.dev2317/monai/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/config/deviceconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/config/type_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.539619 monai-weekly-1.2.dev2317/monai/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50102 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    68927 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    60619 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    39872 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/image_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/meta_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    27321 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/test_time_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    64795 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/video_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/wsi_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    49442 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/wsi_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.543619 monai-weekly-1.2.dev2317/monai/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24568 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/engines/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/engines/multi_gpu_supervised_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21347 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/engines/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/engines/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/engines/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.543619 monai-weekly-1.2.dev2317/monai/fl/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/fl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.543619 monai-weekly-1.2.dev2317/monai/fl/client/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/fl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/fl/client/client_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    33232 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/fl/client/monai_algo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.547619 monai-weekly-1.2.dev2317/monai/fl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/fl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/fl/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/fl/utils/exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/fl/utils/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.555619 monai-weekly-1.2.dev2317/monai/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/clearml_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/earlystop_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/ignite_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/logfile_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/lr_schedule_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/metrics_reloaded_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/nvtx_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/probability_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/smartcache_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/stats_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    23325 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/tensorboard_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/validation_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.559620 monai-weekly-1.2.dev2317/monai/inferers/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/inferers/inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/inferers/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/inferers/splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20017 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/inferers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.563619 monai-weekly-1.2.dev2317/monai/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/deform.py
--rw-r--r--   0 runner    (1001) docker     (123)    46326 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/image_dissimilarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/spatial_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/tversky.py
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/unified_focal_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.571620 monai-weekly-1.2.dev2317/monai/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/active_learning_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/f_beta_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/meandice.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/meaniou.py
--rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/rocauc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.571620 monai-weekly-1.2.dev2317/monai/networks/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.583620 monai-weekly-1.2.dev2317/monai/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/acti_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/backbone_fpn_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/crf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/denseblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/dints_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/feature_pyramid_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/fft_utils_t.py
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/selfattention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/squeeze_and_excitation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/text_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.587620 monai-weekly-1.2.dev2317/monai/networks/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/convutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/simplelayers.py
--rw-r--r--   0 runner    (1001) docker     (123)    25576 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/spatial_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.603620 monai-weekly-1.2.dev2317/monai/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21533 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/ahnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/dints.py
--rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/dynunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    40643 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/highresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/milmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/netadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17189 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/regunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/segresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/senet.py
--rw-r--r--   0 runner    (1001) docker     (123)    42000 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/torchvision_fc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/transchex.py
--rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/vnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    46938 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.603620 monai-weekly-1.2.dev2317/monai/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/optimizers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/optimizers/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/optimizers/novograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/optimizers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.611620 monai-weekly-1.2.dev2317/monai/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/adaptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    40812 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/compose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.615620 monai-weekly-1.2.dev2317/monai/transforms/croppad/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/croppad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68231 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/croppad/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/croppad/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    54071 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/croppad/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/croppad/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.619620 monai-weekly-1.2.dev2317/monai/transforms/intensity/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/intensity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    98613 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/intensity/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    76501 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/intensity/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/inverse_batch_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.619620 monai-weekly-1.2.dev2317/monai/transforms/io/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25430 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/io/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/io/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.623620 monai-weekly-1.2.dev2317/monai/transforms/lazy/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/lazy/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/lazy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.623620 monai-weekly-1.2.dev2317/monai/transforms/meta_utility/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/meta_utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/meta_utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/nvtx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.623620 monai-weekly-1.2.dev2317/monai/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    39905 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.627620 monai-weekly-1.2.dev2317/monai/transforms/signal/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16378 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/signal/array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.627620 monai-weekly-1.2.dev2317/monai/transforms/smooth_field/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/smooth_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/smooth_field/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/smooth_field/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.631620 monai-weekly-1.2.dev2317/monai/transforms/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   168618 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/spatial/array.py
--rw-r--r--   0 runner    (1001) docker     (123)   107151 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/spatial/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    31494 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/spatial/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.635620 monai-weekly-1.2.dev2317/monai/transforms/utility/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70839 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/utility/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    76330 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    72516 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31081 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/utils_create_transform_ims.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/utils_pytorch_numpy_unification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.639620 monai-weekly-1.2.dev2317/monai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/deprecate_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    16807 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/jupyter_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    27512 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/nvtx.py
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/type_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.643620 monai-weekly-1.2.dev2317/monai/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/visualize/class_activation_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/visualize/gradient_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/visualize/img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/visualize/occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/visualize/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/visualize/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.647620 monai-weekly-1.2.dev2317/monai_weekly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-23 02:24:34.000000 monai-weekly-1.2.dev2317/monai_weekly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33869 2023-04-23 02:24:34.000000 monai-weekly-1.2.dev2317/monai_weekly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 02:24:34.000000 monai-weekly-1.2.dev2317/monai_weekly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 02:24:34.000000 monai-weekly-1.2.dev2317/monai_weekly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-23 02:24:34.000000 monai-weekly-1.2.dev2317/monai_weekly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 02:24:34.000000 monai-weekly-1.2.dev2317/monai_weekly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-23 02:24:34.931623 monai-weekly-1.2.dev2317/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.931623 monai-weekly-1.2.dev2317/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_acn_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_activationsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_adaptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_add_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_add_coordinate_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_add_coordinate_channelsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_add_extreme_points_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_add_extreme_points_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_adn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_affine_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_affined.py
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ahnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_anchor_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_apply_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_arraydataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_as_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_as_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_as_channel_last.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_as_channel_lastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_as_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_as_discreted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_atss_box_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_auto3dseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_auto3dseg_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_auto3dseg_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_avg_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bending_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bilateral_approx_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bilateral_approx_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bilateral_precise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_blend_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_border_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_border_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bounding_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bounding_rectd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_box_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_box_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_ckpt_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_init_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_onnx_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_trt_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_verify_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_verify_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cachedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cachedataset_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cachedataset_persistent_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cachentransdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_call_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cast_to_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cast_to_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_center_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_center_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_center_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_center_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_channel_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_check_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_check_missing_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_classes_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_component_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compose_get_number_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_f_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_ho_ver_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_ho_ver_maps_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_meandice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_meaniou.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_variance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_concat_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_config_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_contrastive_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_convert_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_convert_to_multi_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_convert_to_multi_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_convert_to_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_convert_to_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_convert_to_trt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_copy_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_copy_model_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_correct_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_create_cross_validation_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_create_grid_and_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_crf_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_crf_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_crop_foreground.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_crop_foregroundd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_csv_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cumulative.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cumulative_average_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cv2_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_data_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_data_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dataset_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_decathlondataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_decollate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_deepedit_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_deepedit_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_deepgrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_deepgrow_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_deepgrow_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_delete_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_denseblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_detect_envelope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_detection_coco_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_detector_boxselector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dev_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dice_ce_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dints_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dints_mixop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dints_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_divisible_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_divisible_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_download_and_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_downsample_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_drop_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dvf2ddf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dynunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ensemble_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ensure_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ensure_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ensure_tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ensure_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ensure_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_enum_bound_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_eval_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_evenly_divisible_all_gather_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_factorized_increase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_factorized_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fg_bg_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fg_bg_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_file_basename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fill_holes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fill_holesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fl_exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fl_monai_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fl_monai_algo_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fl_monai_algo_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_flatten_sub_keysd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_foreground_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_foreground_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fpn_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_from_engine_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_gaussian_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generalized_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generalized_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generalized_wasserstein_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_distance_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_distance_mapd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_instance_border.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_instance_borderd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_instance_centroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_instance_centroidd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_instance_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_instance_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_instance_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_label_classes_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_param_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_pos_neg_label_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_spatial_bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_succinct_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_succinct_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_watershed_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_watershed_markersd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_watershed_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_watershed_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_get_equivalent_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_get_extreme_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_get_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_get_package_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_get_unique_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_global_mutual_information_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_globalnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_grid_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_grid_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_grid_splitd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_classification_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_clearml_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_clearml_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_confusion_matrix_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_early_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_logfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_metrics_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_nvtx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_prob_map_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_regression_metrics_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_rocauc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_rocauc_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_smartcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_tb_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_tb_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hardnegsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_header_correct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_highresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hilbert_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_histogram_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_histogram_normalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hovernet_instance_map_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hovernet_instance_map_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hovernet_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hovernet_nuclear_type_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hovernet_nuclear_type_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_identityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_image_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_image_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_init_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_autorunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_bundle_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_classification_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_fast_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_gpu_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_lazy_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_segmentation_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_sliding_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_stn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_unet_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_workflows_gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_intensity_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_intensity_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    18873 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_inverse_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_inverse_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_invert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_invertd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_is_supported_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_itk_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_keep_largest_connected_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_keep_largest_connected_componentd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_kspace_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_label_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_label_filterd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_label_quality_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_label_to_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_label_to_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_label_to_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_label_to_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_lesion_froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_list_data_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_list_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_lltm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_lmdbdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_lmdbdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_load_decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_load_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_load_imaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_load_spacing_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_loader_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_local_normalized_cross_correlation_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_localnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_look_up_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_make_nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_map_binary_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_map_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_map_label_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_map_label_valued.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_map_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_mask_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_mask_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_masked_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_masked_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_masked_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_matshow3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_mean_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_mean_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_median_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_median_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_median_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_mednistdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_meta_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    23490 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_metatensor_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_milmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_mmar_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_module_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_monai_env_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_monai_utils_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_mri_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_net_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_network_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_nifti_endianness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_nifti_header_revise.py
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_nifti_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_normalize_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_npzdictitemdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_nrrd_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_nuclick_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_numpy_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_nvtx_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_nvtx_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_one_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_optim_novograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_optional_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ori_ras_lps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_orientationd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_p3d_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_pad_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_pad_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_parallel_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_parallel_execution_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_partition_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_partition_dataset_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_patch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_patch_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_pathology_he_stain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_pathology_he_stain_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_pathology_prob_nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_persistentdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_persistentdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_phl_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_phl_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_pil_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_plot_2d_or_3d_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_png_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_polyval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_prepare_batch_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_prepare_batch_default_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_prepare_batch_extra_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_prepare_batch_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_preset_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_print_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_print_transform_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_probnms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_probnmsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_pytorch_version_after.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_query_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_affined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_axis_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_axis_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_bias_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_bias_fieldd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_coarse_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_coarse_dropoutd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_coarse_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_coarse_shuffled.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_crop_by_label_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_crop_by_label_classesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_crop_by_pos_neg_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_crop_by_pos_neg_labeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_deform_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_elastic_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_elastic_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_elasticd_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_elasticd_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_gaussian_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_histogram_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_histogram_shiftd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_rician_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_rician_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_spatial_crop_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_spatial_crop_samplesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_weighted_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_weighted_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_randidentity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_random_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_randomizable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_randomizable_transform_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_randtorchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rankfilter_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_recon_net_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_reference_based_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_reference_based_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_reg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_regunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_remove_repeated_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_remove_repeated_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_remove_small_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_repeat_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_repeat_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_replace_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_require_pkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resample_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resample_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resample_to_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resample_to_matchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resize_with_pad_or_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resize_with_pad_or_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resized.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_retinanet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_retinanet_predict_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_safe_dtype_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_saliency_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_sample_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_save_classificationd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_save_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_save_imaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_save_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_savitzky_golay_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_savitzky_golay_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_savitzky_golay_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_scale_intensity_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_scale_intensity_range_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_scale_intensity_range_percentilesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_scale_intensity_ranged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_se_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_se_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_seg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_segresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_select_cross_validation_folds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_select_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_selfattention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_senet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_separable_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_set_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_set_visible_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_shuffle_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_continuouswavelet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_fillempty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_rand_add_gaussiannoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_rand_add_sine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_rand_add_sine_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_rand_add_squarepulse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_rand_add_squarepulse_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_rand_drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_rand_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_rand_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_remove_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_simple_aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_simulatedelay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_simulatedelayd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_skip_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_slice_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_sliding_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_sliding_window_hovernet_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_sliding_window_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_sliding_window_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_smartcachedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_smooth_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_sobel_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_sobel_gradientd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_some_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_spacingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_spatial_combine_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_spatial_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_spatial_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_spatial_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_spatial_resampled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_split_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_split_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_splitdim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_splitdimd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_squeezedim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_squeezedimd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ssim_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_str2bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_str2list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_subpixel_upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_tciadataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_testtimeaugmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_text_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_threadcontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_threshold_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_threshold_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_timedcall_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_contiguous.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_cupy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_cupyd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_deviced.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_from_meta_tensord.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_numpyd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_onehot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_pild.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_tensord.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_torchvision_fc_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_torchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_traceable_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_train_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_trainable_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_trainable_joint_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_transchex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_transposed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_tversky_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_unified_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_upsample_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_utils_pytorch_numpy_unification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_varnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_version_leq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_video_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_vis_cam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_vis_gradbased.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_vis_gradcam.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_vnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_vote_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_vote_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_warp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_watershed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_watershedd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_weighted_random_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_with_allow_missing_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_write_metrics_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    25914 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_wsireader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_zipdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_zoom_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)    81097 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.741173 monai-weekly-1.2.dev2318/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-30 02:19:55.741173 monai-weekly-1.2.dev2318/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.741173 monai-weekly-1.2.dev2318/monai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-30 02:17:39.000000 monai-weekly-1.2.dev2318/monai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.001177 monai-weekly-1.2.dev2318/monai/_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.001177 monai-weekly-1.2.dev2318/monai/_extensions/gmm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/_extensions/gmm/gmm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/_extensions/gmm/gmm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/_extensions/gmm/gmm_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/_extensions/gmm/gmm_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/_extensions/gmm/gmm_cuda_linalg.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/_extensions/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-30 02:19:55.741173 monai-weekly-1.2.dev2318/monai/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.005177 monai-weekly-1.2.dev2318/monai/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.013177 monai-weekly-1.2.dev2318/monai/apps/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/auto3dseg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37011 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/auto3dseg/auto_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26063 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/auto3dseg/bundle_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/auto3dseg/data_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24588 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/auto3dseg/ensemble_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/auto3dseg/hpo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/auto3dseg/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/auto3dseg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34568 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.013177 monai-weekly-1.2.dev2318/monai/apps/deepedit/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/deepedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/deepedit/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37435 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/deepedit/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.017177 monai-weekly-1.2.dev2318/monai/apps/deepgrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/deepgrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/deepgrow/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/deepgrow/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42011 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/deepgrow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.017177 monai-weekly-1.2.dev2318/monai/apps/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.021177 monai-weekly-1.2.dev2318/monai/apps/detection/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26617 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/metrics/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/metrics/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.021177 monai-weekly-1.2.dev2318/monai/apps/detection/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53221 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/networks/retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18850 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/networks/retinanet_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.025177 monai-weekly-1.2.dev2318/monai/apps/detection/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24519 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17916 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/transforms/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68979 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.033177 monai-weekly-1.2.dev2318/monai/apps/detection/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/utils/ATSS_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18681 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/utils/anchor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/utils/box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/utils/box_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/utils/detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/utils/hard_negative_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/detection/utils/predict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.033177 monai-weekly-1.2.dev2318/monai/apps/mmars/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/mmars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/mmars/mmars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/mmars/model_desc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.037176 monai-weekly-1.2.dev2318/monai/apps/nnunet/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/nnunet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/nnunet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38587 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/nnunet/nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/nnunet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.037176 monai-weekly-1.2.dev2318/monai/apps/nuclick/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/nuclick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/nuclick/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.041177 monai-weekly-1.2.dev2318/monai/apps/pathology/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.041177 monai-weekly-1.2.dev2318/monai/apps/pathology/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/engines/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.045177 monai-weekly-1.2.dev2318/monai/apps/pathology/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/handlers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.045177 monai-weekly-1.2.dev2318/monai/apps/pathology/inferers/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/inferers/inferer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.049177 monai-weekly-1.2.dev2318/monai/apps/pathology/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/losses/hovernet_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.049177 monai-weekly-1.2.dev2318/monai/apps/pathology/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/metrics/lesion_froc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.049177 monai-weekly-1.2.dev2318/monai/apps/pathology/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.053176 monai-weekly-1.2.dev2318/monai/apps/pathology/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37322 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.057176 monai-weekly-1.2.dev2318/monai/apps/pathology/transforms/stain/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/transforms/stain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/transforms/stain/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/transforms/stain/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/pathology/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.061176 monai-weekly-1.2.dev2318/monai/apps/reconstruction/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/reconstruction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/reconstruction/complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/reconstruction/fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/reconstruction/mri_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.061176 monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.061176 monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/blocks/varnetblock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.069177 monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/nets/complex_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/nets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/nets/varnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.069177 monai-weekly-1.2.dev2318/monai/apps/reconstruction/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/reconstruction/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/reconstruction/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15844 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/reconstruction/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.073176 monai-weekly-1.2.dev2318/monai/apps/tcia/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/tcia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/tcia/label_desc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/tcia/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.077176 monai-weekly-1.2.dev2318/monai/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/auto3dseg/algo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41223 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/auto3dseg/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/auto3dseg/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/auto3dseg/seg_summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/auto3dseg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.085176 monai-weekly-1.2.dev2318/monai/bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/bundle/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16035 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/bundle/config_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/bundle/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/bundle/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/bundle/reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64234 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/bundle/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/bundle/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19001 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/bundle/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.085176 monai-weekly-1.2.dev2318/monai/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/config/deviceconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/config/type_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.109176 monai-weekly-1.2.dev2318/monai/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50102 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68927 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60619 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39872 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/image_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/meta_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27321 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/test_time_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64795 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/video_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/wsi_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49442 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/data/wsi_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.117176 monai-weekly-1.2.dev2318/monai/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24568 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/engines/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/engines/multi_gpu_supervised_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21347 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/engines/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/engines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/engines/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.117176 monai-weekly-1.2.dev2318/monai/fl/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/fl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.121176 monai-weekly-1.2.dev2318/monai/fl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/fl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/fl/client/client_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33232 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/fl/client/monai_algo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.125176 monai-weekly-1.2.dev2318/monai/fl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/fl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/fl/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/fl/utils/exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/fl/utils/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.141176 monai-weekly-1.2.dev2318/monai/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/clearml_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/earlystop_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/ignite_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/logfile_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/lr_schedule_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/metrics_reloaded_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/nvtx_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/probability_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/smartcache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/stats_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23325 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/tensorboard_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/handlers/validation_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.145176 monai-weekly-1.2.dev2318/monai/inferers/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32256 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/inferers/inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/inferers/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/inferers/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20017 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/inferers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.153176 monai-weekly-1.2.dev2318/monai/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/losses/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/losses/deform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46326 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/losses/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/losses/ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/losses/giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/losses/image_dissimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/losses/multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/losses/spatial_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/losses/ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/losses/tversky.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/losses/unified_focal_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.169176 monai-weekly-1.2.dev2318/monai/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/active_learning_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/f_beta_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/meandice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/metrics/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.173176 monai-weekly-1.2.dev2318/monai/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.189176 monai-weekly-1.2.dev2318/monai/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/acti_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/backbone_fpn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/crf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/dints_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/feature_pyramid_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/fft_utils_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/squeeze_and_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/text_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/blocks/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.193176 monai-weekly-1.2.dev2318/monai/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/layers/convutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/layers/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/layers/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/layers/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/layers/gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/layers/simplelayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25576 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/layers/spatial_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/layers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/layers/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.217176 monai-weekly-1.2.dev2318/monai/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21533 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/dints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40643 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/netadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17189 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/regunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42000 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/torchvision_fc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/transchex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/nets/vnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46938 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/networks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.221176 monai-weekly-1.2.dev2318/monai/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/optimizers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/optimizers/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/optimizers/novograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/optimizers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.229176 monai-weekly-1.2.dev2318/monai/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40812 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/compose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.237176 monai-weekly-1.2.dev2318/monai/transforms/croppad/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/croppad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68231 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/croppad/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/croppad/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54071 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/croppad/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/croppad/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.237176 monai-weekly-1.2.dev2318/monai/transforms/intensity/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/intensity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98613 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/intensity/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76501 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/intensity/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18604 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/inverse_batch_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.241176 monai-weekly-1.2.dev2318/monai/transforms/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25430 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/io/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/io/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.241176 monai-weekly-1.2.dev2318/monai/transforms/lazy/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/lazy/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/lazy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.245175 monai-weekly-1.2.dev2318/monai/transforms/meta_utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/meta_utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/meta_utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/nvtx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.245175 monai-weekly-1.2.dev2318/monai/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39905 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.245175 monai-weekly-1.2.dev2318/monai/transforms/signal/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16378 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/signal/array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.249175 monai-weekly-1.2.dev2318/monai/transforms/smooth_field/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/smooth_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/smooth_field/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/smooth_field/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.253176 monai-weekly-1.2.dev2318/monai/transforms/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   166745 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/spatial/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107151 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/spatial/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31773 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/spatial/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.257176 monai-weekly-1.2.dev2318/monai/transforms/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70839 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/utility/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76330 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77669 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31081 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/utils_create_transform_ims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/transforms/utils_pytorch_numpy_unification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.265175 monai-weekly-1.2.dev2318/monai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/utils/deprecate_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16807 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/utils/jupyter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28185 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/utils/nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/utils/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/utils/state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/utils/type_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.269175 monai-weekly-1.2.dev2318/monai/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/visualize/class_activation_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/visualize/gradient_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/visualize/img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/visualize/occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/visualize/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/monai/visualize/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.269175 monai-weekly-1.2.dev2318/monai_weekly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-30 02:19:54.000000 monai-weekly-1.2.dev2318/monai_weekly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33903 2023-04-30 02:19:54.000000 monai-weekly-1.2.dev2318/monai_weekly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 02:19:54.000000 monai-weekly-1.2.dev2318/monai_weekly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 02:19:54.000000 monai-weekly-1.2.dev2318/monai_weekly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-30 02:19:54.000000 monai-weekly-1.2.dev2318/monai_weekly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 02:19:54.000000 monai-weekly-1.2.dev2318/monai_weekly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-30 02:19:55.741173 monai-weekly-1.2.dev2318/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:19:55.741173 monai-weekly-1.2.dev2318/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_acn_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_activationsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_add_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_add_coordinate_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_add_coordinate_channelsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_add_extreme_points_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_add_extreme_points_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_adn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_affine_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_affined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_anchor_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_apply_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_arraydataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_as_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_as_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_as_channel_last.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_as_channel_lastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_as_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_as_discreted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_atss_box_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_auto3dseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_auto3dseg_bundlegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_auto3dseg_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_auto3dseg_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_avg_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_bending_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_bilateral_approx_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_bilateral_approx_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_bilateral_precise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_blend_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_border_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_border_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_bounding_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_bounding_rectd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_box_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_bundle_ckpt_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_bundle_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_bundle_get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_bundle_init_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_bundle_onnx_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_bundle_trt_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_bundle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_bundle_verify_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_bundle_verify_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_bundle_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_cachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_cachedataset_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_cachedataset_persistent_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_cachentransdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_call_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_cast_to_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_cast_to_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_center_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_center_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_center_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_center_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_channel_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_check_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_check_missing_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_classes_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_component_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_compose_get_number_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_compute_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_compute_f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_compute_froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_compute_generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_compute_ho_ver_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_compute_ho_ver_maps_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_compute_meandice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_compute_meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_compute_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_compute_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_compute_roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_compute_variance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_concat_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_config_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_contrastive_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_convert_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_convert_to_multi_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_convert_to_multi_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_convert_to_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_convert_to_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_convert_to_trt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_copy_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_copy_model_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_correct_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_create_cross_validation_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_create_grid_and_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_crf_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_crf_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_crop_foreground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_crop_foregroundd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_csv_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_cumulative_average_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_cv2_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_data_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_data_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_dataset_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_decathlondataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_decollate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_deepedit_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_deepedit_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_deepgrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_deepgrow_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_deepgrow_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_delete_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_detect_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_detection_coco_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_detector_boxselector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_dev_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_dice_ce_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_dints_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_dints_mixop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_dints_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_divisible_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_divisible_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_download_and_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_downsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_dvf2ddf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_ensemble_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_ensure_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_ensure_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_ensure_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_ensure_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_ensure_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_enum_bound_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_eval_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_evenly_divisible_all_gather_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_factorized_increase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_factorized_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_fg_bg_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_fg_bg_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_file_basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_fill_holes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_fill_holesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_fl_exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_fl_monai_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_fl_monai_algo_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_fl_monai_algo_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_flatten_sub_keysd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_foreground_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_foreground_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_fpn_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_from_engine_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_gaussian_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generalized_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generalized_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generalized_wasserstein_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_distance_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_distance_mapd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_instance_border.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_instance_borderd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_instance_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_instance_centroidd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_instance_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_instance_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_instance_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_label_classes_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_param_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_pos_neg_label_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_spatial_bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_succinct_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_succinct_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_watershed_markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_watershed_markersd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_watershed_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generate_watershed_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_get_equivalent_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_get_extreme_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_get_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_get_package_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_get_unique_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_global_mutual_information_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_globalnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_grid_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_grid_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_grid_splitd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_classification_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_clearml_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_clearml_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_confusion_matrix_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_early_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_logfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_metrics_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_prob_map_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_regression_metrics_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_rocauc_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_smartcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_tb_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_tb_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_handler_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_hardnegsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_header_correct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_hilbert_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_histogram_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_histogram_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_hovernet_instance_map_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_hovernet_instance_map_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_hovernet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_hovernet_nuclear_type_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_hovernet_nuclear_type_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_identityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_image_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_image_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_init_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_integration_autorunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_integration_bundle_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_integration_classification_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_integration_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_integration_fast_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_integration_gpu_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_integration_lazy_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_integration_nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_integration_segmentation_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_integration_sliding_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_integration_stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_integration_unet_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_integration_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_integration_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_integration_workflows_gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_intensity_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_intensity_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18873 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_inverse_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_inverse_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_invert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_invertd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_is_supported_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_itk_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_keep_largest_connected_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_keep_largest_connected_componentd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_kspace_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_label_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_label_filterd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_label_quality_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_label_to_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_label_to_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_label_to_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_label_to_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_lesion_froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_list_data_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_list_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_lltm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_lmdbdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_lmdbdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_load_decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_load_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_load_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_load_spacing_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_loader_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_local_normalized_cross_correlation_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_localnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_look_up_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_make_nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_map_binary_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_map_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_map_label_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_map_label_valued.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_map_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_mask_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_mask_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_masked_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_masked_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_masked_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_matshow3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_mean_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_mean_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_median_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_median_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_median_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_mednistdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_meta_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23490 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_metatensor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_mmar_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_monai_env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_monai_utils_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_mri_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_net_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_network_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_nifti_endianness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_nifti_header_revise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_nifti_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_normalize_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_npzdictitemdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_nrrd_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_nuclick_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_numpy_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_nvtx_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_nvtx_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_optim_novograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_optional_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_ori_ras_lps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_orientationd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_p3d_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_pad_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_pad_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_parallel_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_parallel_execution_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_partition_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_partition_dataset_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_patch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_patch_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_pathology_he_stain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_pathology_he_stain_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_pathology_prob_nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_persistentdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_persistentdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_phl_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_phl_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_pil_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_plot_2d_or_3d_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_png_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_polyval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_prepare_batch_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_prepare_batch_default_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_prepare_batch_extra_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_prepare_batch_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_preset_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_print_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_print_transform_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_probnms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_probnmsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_pytorch_version_after.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_query_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_affined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_axis_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_axis_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_bias_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_bias_fieldd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_coarse_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_coarse_dropoutd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_coarse_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_coarse_shuffled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_crop_by_label_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_crop_by_label_classesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_crop_by_pos_neg_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_crop_by_pos_neg_labeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_deform_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_elastic_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_elastic_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_elasticd_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_elasticd_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_gaussian_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_histogram_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_histogram_shiftd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_rician_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_rician_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_spatial_crop_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_spatial_crop_samplesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_weighted_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_weighted_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rand_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_randidentity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_random_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_randomizable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_randomizable_transform_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_randtorchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rankfilter_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_recon_net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_reference_based_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_reference_based_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_reg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_regunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_remove_repeated_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_remove_repeated_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_remove_small_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_repeat_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_repeat_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_replace_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_require_pkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_resample_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_resample_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_resample_to_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_resample_to_matchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_resize_with_pad_or_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_resize_with_pad_or_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_resized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_retinanet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_retinanet_predict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_safe_dtype_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_saliency_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_sample_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_save_classificationd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_save_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_save_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_save_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_savitzky_golay_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_savitzky_golay_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_savitzky_golay_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_scale_intensity_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_scale_intensity_range_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_scale_intensity_range_percentilesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_scale_intensity_ranged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_se_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_se_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_seg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_select_cross_validation_folds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_select_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_separable_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_set_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_set_visible_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_shuffle_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_signal_continuouswavelet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_signal_fillempty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_signal_rand_add_gaussiannoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_signal_rand_add_sine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_signal_rand_add_sine_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_signal_rand_add_squarepulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_signal_rand_add_squarepulse_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_signal_rand_drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_signal_rand_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_signal_rand_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_signal_remove_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_simple_aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_simulatedelay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_simulatedelayd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_skip_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_slice_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_sliding_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_sliding_window_hovernet_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_sliding_window_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_sliding_window_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_smartcachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_smooth_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_sobel_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_sobel_gradientd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_some_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_spacingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_spatial_combine_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_spatial_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_spatial_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_spatial_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_spatial_resampled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_split_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_split_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_splitdim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_splitdimd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_squeezedim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_squeezedimd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_ssim_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_str2bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_str2list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_subpixel_upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_tciadataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_testtimeaugmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_text_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_threadcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_threshold_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_threshold_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_timedcall_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_to_contiguous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_to_cupy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_to_cupyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_to_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_to_deviced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_to_from_meta_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_to_numpyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_to_onehot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_to_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_to_pild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_to_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_to_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_torchvision_fc_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_torchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_traceable_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_train_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_trainable_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_trainable_joint_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_transchex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_transposed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_tversky_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_unified_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_upsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_utils_pytorch_numpy_unification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_varnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_version_leq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_video_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_vis_cam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_vis_gradbased.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_vis_gradcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_vnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_vote_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_vote_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_warp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_watershed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_watershedd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_weighted_random_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_with_allow_missing_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_write_metrics_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25914 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_wsireader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_zipdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_zoom_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/tests/test_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81097 2023-04-30 02:17:33.000000 monai-weekly-1.2.dev2318/versioneer.py
```

### Comparing `monai-weekly-1.2.dev2317/LICENSE` & `monai-weekly-1.2.dev2318/LICENSE`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/PKG-INFO` & `monai-weekly-1.2.dev2318/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.2.dev2317
+Version: 1.2.dev2318
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
```

### Comparing `monai-weekly-1.2.dev2317/README.md` & `monai-weekly-1.2.dev2318/README.md`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/__init__.py` & `monai-weekly-1.2.dev2318/monai/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,8 +74,8 @@
     "metrics",
     "networks",
     "optimizers",
     "transforms",
     "utils",
     "visualize",
 ]
-__commit_id__ = "43902e3330da8d879222511131e60f40b38d692e"
+__commit_id__ = "d29914d50dd66fbc35e0474da4782fb45a6b47b5"
```

### Comparing `monai-weekly-1.2.dev2317/monai/_extensions/__init__.py` & `monai-weekly-1.2.dev2318/monai/_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm.cpp` & `monai-weekly-1.2.dev2318/monai/_extensions/gmm/gmm.cpp`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm.h` & `monai-weekly-1.2.dev2318/monai/_extensions/gmm/gmm.h`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm_cpu.cpp` & `monai-weekly-1.2.dev2318/monai/_extensions/gmm/gmm_cpu.cpp`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm_cuda.cu` & `monai-weekly-1.2.dev2318/monai/_extensions/gmm/gmm_cuda.cu`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm_cuda_linalg.cuh` & `monai-weekly-1.2.dev2318/monai/_extensions/gmm/gmm_cuda_linalg.cuh`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/_extensions/loader.py` & `monai-weekly-1.2.dev2318/monai/_extensions/loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/auto3dseg/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/auto3dseg/__main__.py` & `monai-weekly-1.2.dev2318/monai/apps/auto3dseg/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/auto3dseg/auto_runner.py` & `monai-weekly-1.2.dev2318/monai/apps/auto3dseg/auto_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 from monai.apps.auto3dseg.data_analyzer import DataAnalyzer
 from monai.apps.auto3dseg.ensemble_builder import EnsembleRunner
 from monai.apps.auto3dseg.hpo_gen import NNIGen
 from monai.apps.auto3dseg.utils import export_bundle_algo_history, import_bundle_algo_history
 from monai.apps.utils import get_logger
 from monai.auto3dseg.utils import algo_to_pickle
 from monai.bundle import ConfigParser
+from monai.transforms import SaveImage
 from monai.utils import AlgoKeys, has_option, look_up_option, optional_import
+from monai.utils.misc import check_kwargs_exist_in_class_init
 
 logger = get_logger(module_name=__name__)
 
 nni, has_nni = optional_import("nni")
 
 
 class AutoRunner:
@@ -101,90 +103,81 @@
             python -m monai.apps.auto3dseg AutoRunner run --input=./input.yaml
 
         - User can specify work_dir and data source config input and run AutoRunner:
 
         .. code-block:: python
 
             work_dir = "./work_dir"
-            input = "path_to_yaml_data_cfg"
+            input = "path/to/input_yaml"
             runner = AutoRunner(work_dir=work_dir, input=input)
             runner.run()
 
         - User can specify a subset of algorithms to use and run AutoRunner:
 
         .. code-block:: python
 
             work_dir = "./work_dir"
-            input = "path_to_yaml_data_cfg"
+            input = "path/to/input_yaml"
             algos = ["segresnet", "dints"]
             runner = AutoRunner(work_dir=work_dir, input=input, algos=algos)
             runner.run()
 
         - User can specify a a local folder with algorithms templates and run AutoRunner:
 
         .. code-block:: python
 
             work_dir = "./work_dir"
-            input = "path_to_yaml_data_cfg"
+            input = "path/to/input_yaml"
             algos = "segresnet"
             templates_path_or_url = "./local_path_to/algorithm_templates"
             runner = AutoRunner(work_dir=work_dir, input=input, algos=algos, templates_path_or_url=templates_path_or_url)
             runner.run()
 
         - User can specify training parameters by:
 
         .. code-block:: python
 
-            input = "path_to_yaml_data_cfg"
+            input = "path/to/input_yaml"
             runner = AutoRunner(input=input)
             train_param = {
-                "CUDA_VISIBLE_DEVICES": [0],
-                "num_iterations": 8,
-                "num_iterations_per_validation": 4,
+                "num_epochs_per_validation": 1,
                 "num_images_per_batch": 2,
                 "num_epochs": 2,
             }
             runner.set_training_params(params=train_param)  # 2 epochs
             runner.run()
 
         - User can specify the fold number of cross validation
 
         .. code-block:: python
 
-            input = "path_to_yaml_data_cfg"
+            input = "path/to/input_yaml"
             runner = AutoRunner(input=input)
             runner.set_num_fold(n_fold = 2)
             runner.run()
 
         - User can specify the prediction parameters during algo ensemble inference:
 
         .. code-block:: python
 
-            input = "path_to_yaml_data_cfg"
+            input = "path/to/input_yaml"
             pred_params = {
                 'files_slices': slice(0,2),
                 'mode': "vote",
                 'sigmoid': True,
             }
             runner = AutoRunner(input=input)
             runner.set_prediction_params(params=pred_params)
             runner.run()
 
         - User can define a grid search space and use the HPO during training.
 
         .. code-block:: python
 
-            input = "path_to_yaml_data_cfg"
-            pred_param = {
-                "CUDA_VISIBLE_DEVICES": [0],
-                "num_iterations": 8,
-                "num_iterations_per_validation": 4,
-                "num_images_per_batch": 2,
-                "num_epochs": 2,
-            }
+            input = "path/to/input_yaml"
             runner = AutoRunner(input=input, hpo=True)
             runner.set_nni_search_space({"learning_rate": {"_type": "choice", "_value": [0.0001, 0.001, 0.01, 0.1]}})
             runner.run()
 
     Notes:
         Expected results in the work_dir as below::
 
@@ -465,15 +458,15 @@
 
         Args:
             params: a dict that defines the overriding key-value pairs during training. The overriding method
                 is defined by the algo class.
 
         Examples:
             For BundleAlgo objects, the training parameter to shorten the training time to a few epochs can be
-                {"num_iterations": 8, "num_iterations_per_validation": 4}
+                {"num_epochs": 2, "num_epochs_per_validation": 1}
 
         """
         self.train_params = deepcopy(params) if params is not None else {}
         if "CUDA_VISIBLE_DEVICES" in self.train_params:
             warnings.warn(
                 "CUDA_VISIBLE_DEVICES is deprecated from 'set_training_params'. Use 'set_device_info' intead.",
                 DeprecationWarning,
@@ -557,15 +550,22 @@
 
         Args:
             kwargs: image writing parameters for the ensemble inference. The kwargs format follows SaveImage
                 transform. For more information, check https://docs.monai.io/en/stable/transforms.html#saveimage.
 
         """
 
-        self.kwargs.update(kwargs)
+        are_all_args_present, extra_args = check_kwargs_exist_in_class_init(SaveImage, kwargs)
+        if are_all_args_present:
+            self.kwargs.update(kwargs)
+        else:
+            raise ValueError(
+                f"{extra_args} are not supported in monai.transforms.SaveImage,"
+                "Check https://docs.monai.io/en/stable/transforms.html#saveimage for more information."
+            )
 
     def set_prediction_params(self, params: dict[str, Any] | None = None) -> None:
         """
         Set the prediction params for all algos.
 
         Args:
             params: a dict that defines the overriding key-value pairs during prediction. The overriding method
@@ -583,18 +583,14 @@
         """
         Set the data analysis extra params.
 
         Args:
             params: a dict that defines the overriding key-value pairs during training. The overriding method
                 is defined by the algo class.
 
-        Examples:
-            For BundleAlgo objects, the training parameter to shorten the training time to a few epochs can be
-                {"num_iterations": 8, "num_iterations_per_validation": 4}
-
         """
         if params is None:
             self.analyze_params = {"do_ccp": False, "device": "cuda"}
         else:
             self.analyze_params = deepcopy(params)
 
     def set_hpo_params(self, params: dict[str, Any] | None = None) -> None:
```

### Comparing `monai-weekly-1.2.dev2317/monai/apps/auto3dseg/bundle_gen.py` & `monai-weekly-1.2.dev2318/monai/apps/auto3dseg/bundle_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import torch
 
 from monai.apps import download_and_extract
 from monai.apps.utils import get_logger
 from monai.auto3dseg.algo_gen import Algo, AlgoGen
 from monai.auto3dseg.utils import algo_to_pickle
 from monai.bundle.config_parser import ConfigParser
+from monai.config import PathLike
 from monai.utils import ensure_tuple
 from monai.utils.enums import AlgoKeys
 
 logger = get_logger(module_name=__name__)
 ALGO_HASH = os.environ.get("MONAI_ALGO_HASH", "23ea143")
 
 __all__ = ["BundleAlgo", "BundleGen"]
@@ -59,15 +60,15 @@
 
     This class creates MONAI bundles from a directory of 'bundle template'. Different from the regular MONAI bundle
     format, the bundle template may contain placeholders that must be filled using ``fill_template_config`` during
     ``export_to_disk``. Then created bundle keeps the same file structure as the template.
 
     """
 
-    def __init__(self, template_path: str):
+    def __init__(self, template_path: PathLike):
         """
         Create an Algo instance based on the predefined Algo template.
 
         Args:
             template_path: path to the root of the algo template.
 
         """
@@ -149,17 +150,17 @@
 
         """
         if kwargs.pop("copy_dirs", True):
             self.output_path = os.path.join(output_path, algo_name)
             os.makedirs(self.output_path, exist_ok=True)
             if os.path.isdir(self.output_path):
                 shutil.rmtree(self.output_path)
-            shutil.copytree(self.template_path, self.output_path)
+            shutil.copytree(str(self.template_path), self.output_path)
         else:
-            self.output_path = self.template_path
+            self.output_path = str(self.template_path)
         if kwargs.pop("fill_template", True):
             self.fill_records = self.fill_template_config(self.data_stats_files, self.output_path, **kwargs)
         logger.info(f"Generated:{self.output_path}")
 
     def _create_cmd(self, train_params: None | dict = None) -> tuple[str, str]:
         """
         Create the command to execute training.
```

### Comparing `monai-weekly-1.2.dev2317/monai/apps/auto3dseg/data_analyzer.py` & `monai-weekly-1.2.dev2318/monai/apps/auto3dseg/data_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,14 @@
             hist_bins=self.hist_bins,
             hist_range=self.hist_range,
             histogram_only=self.histogram_only,
         )
         n_cases = len(result_bycase[DataStatsKeys.BY_CASE])
         result[DataStatsKeys.SUMMARY] = summarizer.summarize(cast(list, result_bycase[DataStatsKeys.BY_CASE]))
         result[DataStatsKeys.SUMMARY]["n_cases"] = n_cases
-        result[DataStatsKeys.BY_CASE] = [None] * n_cases
         result_bycase[DataStatsKeys.SUMMARY] = result[DataStatsKeys.SUMMARY]
         if not self._check_data_uniformity([ImageStatsKeys.SPACING], result):
             logger.info("Data spacing is not completely uniform. MONAI transforms may provide unexpected result")
         if self.output_path:
             ConfigParser.export_config_file(
                 result, self.output_path, fmt=self.fmt, default_flow_style=None, sort_keys=False
             )
```

### Comparing `monai-weekly-1.2.dev2317/monai/apps/auto3dseg/ensemble_builder.py` & `monai-weekly-1.2.dev2318/monai/apps/auto3dseg/ensemble_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,17 +26,18 @@
 from monai.apps.auto3dseg.bundle_gen import BundleAlgo
 from monai.apps.auto3dseg.utils import import_bundle_algo_history
 from monai.apps.utils import get_logger
 from monai.auto3dseg import concat_val_to_np
 from monai.auto3dseg.utils import datafold_read
 from monai.bundle import ConfigParser
 from monai.data import partition_dataset
-from monai.transforms import MeanEnsemble, VoteEnsemble
+from monai.transforms import MeanEnsemble, SaveImage, VoteEnsemble
+from monai.utils import RankFilter
 from monai.utils.enums import AlgoKeys
-from monai.utils.misc import prob2class
+from monai.utils.misc import check_kwargs_exist_in_class_init, prob2class
 from monai.utils.module import look_up_option, optional_import
 
 tqdm, has_tqdm = optional_import("tqdm", name="tqdm")
 
 logger = get_logger(module_name=__name__)
 
 
@@ -391,15 +392,15 @@
         **kwargs: Any,
     ) -> None:
         self.data_src_cfg_name = data_src_cfg_name
         self.work_dir = work_dir
         self.num_fold = num_fold
         self.ensemble_method_name = ensemble_method_name
         self.mgpu = mgpu
-        self.kwargs = kwargs
+        self.kwargs = deepcopy(kwargs)
         self.rank = 0
         self.world_size = 1
         self.device_setting: dict[str, int | str] = {
             "CUDA_VISIBLE_DEVICES": ",".join([str(x) for x in range(torch.cuda.device_count())]),
             "n_devices": torch.cuda.device_count(),
             "NUM_NODES": int(os.environ.get("NUM_NODES", 1)),
             "MN_START_METHOD": os.environ.get("MN_START_METHOD", "bcprun"),
@@ -424,52 +425,74 @@
             n_best = kwargs.pop("n_best", False) or 2
             self.ensemble_method = AlgoEnsembleBestN(n_best=n_best)
         elif self.ensemble_method_name == "AlgoEnsembleBestByFold":
             self.ensemble_method = AlgoEnsembleBestByFold(n_fold=self.num_fold)  # type: ignore
         else:
             raise NotImplementedError(f"Ensemble method {self.ensemble_method_name} is not implemented.")
 
-    def set_image_save_transform(self, **kwargs):
+    def _pop_kwargs_to_get_image_save_transform(self, **kwargs):
         """
-        Set the ensemble output transform.
+        Pop the kwargs used to define ImageSave class for the ensemble output.
 
         Args:
             kwargs: image writing parameters for the ensemble inference. The kwargs format follows SaveImage
                 transform. For more information, check https://docs.monai.io/en/stable/transforms.html#saveimage .
 
+        Returns:
+            save_image: a dictionary that can be used to instantiate a SaveImage class in ConfigParser.
         """
 
-        if "output_dir" in kwargs:
-            output_dir = kwargs.pop("output_dir")
-        else:
+        output_dir = kwargs.pop("output_dir", None)
+
+        if output_dir is None:
             output_dir = os.path.join(self.work_dir, "ensemble_output")
-            if self.rank == 0:
-                logger.info(f"The output_dir is not specified. {output_dir} will be used to save ensemble predictions")
+            logger.info(f"The output_dir is not specified. {output_dir} will be used to save ensemble predictions.")
 
         if not os.path.isdir(output_dir):
-            os.makedirs(output_dir)
-            if self.rank == 0:
-                logger.info(f"Directory {output_dir} is created to save ensemble predictions")
-
-        self.output_dir = output_dir
-        output_postfix = kwargs.pop("output_postfix", "ensemble")
-        output_dtype = kwargs.pop("output_dtype", "$np.uint8")
-        resample = kwargs.pop("resample", False)
+            os.makedirs(output_dir, exist_ok=True)
+            logger.info(f"Directory {output_dir} is created to save ensemble predictions")
 
-        self.save_image = {
+        save_image = {
             "_target_": "SaveImage",
             "output_dir": output_dir,
-            "output_postfix": output_postfix,
-            "output_dtype": output_dtype,
-            "resample": resample,
+            "output_postfix": kwargs.pop("output_postfix", "ensemble"),
+            "output_dtype": kwargs.pop("output_dtype", "$np.uint8"),
+            "resample": kwargs.pop("resample", False),
             "print_log": False,
             "savepath_in_metadict": True,
         }
-        if kwargs:
-            self.save_image.update(kwargs)
+
+        are_all_args_save_image, extra_args = check_kwargs_exist_in_class_init(SaveImage, kwargs)
+        if are_all_args_save_image:
+            save_image.update(kwargs)
+        else:
+            # kwargs has extra values for other purposes, for example, pred_params
+            for args in list(kwargs):
+                if args not in extra_args:
+                    save_image.update({args: kwargs.pop(args)})
+
+        return save_image
+
+    def set_image_save_transform(self, **kwargs: Any) -> None:
+        """
+        Set the ensemble output transform.
+
+        Args:
+            kwargs: image writing parameters for the ensemble inference. The kwargs format follows SaveImage
+                transform. For more information, check https://docs.monai.io/en/stable/transforms.html#saveimage .
+
+        """
+        are_all_args_present, extra_args = check_kwargs_exist_in_class_init(SaveImage, kwargs)
+        if are_all_args_present:
+            self.kwargs.update(kwargs)
+        else:
+            raise ValueError(
+                f"{extra_args} are not supported in monai.transforms.SaveImage,"
+                "Check https://docs.monai.io/en/stable/transforms.html#saveimage for more information."
+            )
 
     def set_num_fold(self, num_fold: int = 5) -> None:
         """
         Set the number of cross validation folds for all algos.
 
         Args:
             num_fold: a positive integer to define the number of folds.
@@ -481,27 +504,28 @@
 
     def ensemble(self):
         if self.mgpu:  # torch.cuda.device_count() is not used because env is not set by autorruner
             # init multiprocessing and update infer_files
             dist.init_process_group(backend="nccl", init_method="env://")
             self.world_size = dist.get_world_size()
             self.rank = dist.get_rank()
+            logger.addFilter(RankFilter())
         # set params after init_process_group to know the rank
         self.set_num_fold(num_fold=self.num_fold)
-        self.set_image_save_transform(**self.kwargs)
         self.set_ensemble_method(self.ensemble_method_name, **self.kwargs)
+        # self.kwargs needs to pop out args for set_image_save_transform
+        save_image = self._pop_kwargs_to_get_image_save_transform(**self.kwargs)
 
         history = import_bundle_algo_history(self.work_dir, only_trained=False)
         history_untrained = [h for h in history if not h[AlgoKeys.IS_TRAINED]]
         if history_untrained:
-            if self.rank == 0:
-                warn(
-                    f"Ensembling step will skip {[h[AlgoKeys.ID] for h in history_untrained]} untrained algos."
-                    "Generally it means these algos did not complete training."
-                )
+            logger.warning(
+                f"Ensembling step will skip {[h[AlgoKeys.ID] for h in history_untrained]} untrained algos."
+                "Generally it means these algos did not complete training."
+            )
             history = [h for h in history if h[AlgoKeys.IS_TRAINED]]
         if len(history) == 0:
             raise ValueError(
                 f"Could not find the trained results in {self.work_dir}. "
                 "Possibly the required training step was not completed."
             )
 
@@ -510,23 +534,22 @@
         self.ensembler = builder.get_ensemble()
         infer_files = self.ensembler.infer_files
         infer_files = partition_dataset(
             data=infer_files, shuffle=False, num_partitions=self.world_size, even_divisible=True
         )[self.rank]
         # TO DO: Add some function in ensembler for infer_files update?
         self.ensembler.infer_files = infer_files
-        # self.kwargs has poped out args for set_image_save_transform
         # add rank to pred_params
         self.kwargs["rank"] = self.rank
-        self.kwargs["image_save_func"] = self.save_image
-        if self.rank == 0:
-            logger.info("Auto3Dseg picked the following networks to ensemble:")
-            for algo in self.ensembler.get_algo_ensemble():
-                logger.info(algo[AlgoKeys.ID])
-            logger.info(f"Auto3Dseg ensemble prediction outputs will be saved in {self.output_dir}.")
+        self.kwargs["image_save_func"] = save_image
+        logger.info("Auto3Dseg picked the following networks to ensemble:")
+        for algo in self.ensembler.get_algo_ensemble():
+            logger.info(algo[AlgoKeys.ID])
+        output_dir = save_image["output_dir"]
+        logger.info(f"Auto3Dseg ensemble prediction outputs will be saved in {output_dir}.")
         self.ensembler(pred_param=self.kwargs)
 
         if self.mgpu:
             dist.destroy_process_group()
 
     def run(self, device_setting: dict | None = None) -> None:
         """
```

### Comparing `monai-weekly-1.2.dev2317/monai/apps/auto3dseg/hpo_gen.py` & `monai-weekly-1.2.dev2318/monai/apps/auto3dseg/hpo_gen.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,19 +125,15 @@
                     output_folder = os.path.dirname(algo.get_output_path())
 
                     params.update({"fill_with_datastats": False})  # just copy, not using datastats to fill
                     self.algo.export_to_disk(output_folder, name, **params)
             else:
                 self.algo = algo
 
-            if isinstance(self.algo, BundleAlgo):
-                self.obj_filename = algo_to_pickle(self.algo, template_path=self.algo.template_path)
-            else:
-                self.obj_filename = algo_to_pickle(self.algo)
-                # nni instruction unknown
+            self.obj_filename = algo_to_pickle(self.algo, template_path=self.algo.template_path)
 
     def get_obj_filename(self):
         """Return the filename of the dumped pickle algo object."""
         return self.obj_filename
 
     def print_bundle_algo_instruction(self):
         """
@@ -222,32 +218,26 @@
                 ``{algorithm_templates_dir}/{network}/scripts/algo.py``
         """
         if not os.path.isfile(obj_filename):
             raise ValueError(f"{obj_filename} is not found")
 
         self.algo, algo_meta_data = algo_from_pickle(obj_filename, template_path=template_path)
 
-        if isinstance(self.algo, BundleAlgo):  # algo's template path needs override
-            self.algo.template_path = algo_meta_data["template_path"]
-
         # step 1 sample hyperparams
         params = self.get_hyperparameters()
         # step 2 set the update params for the algo to run in the next trial
         self.update_params(params)
         # step 3 generate the folder to save checkpoints and train
         self.generate(output_folder)
         self.algo.train(self.params)
         # step 4 report validation acc to controller
         acc = self.algo.get_score()
         algo_meta_data = {str(AlgoKeys.SCORE): acc}
 
-        if isinstance(self.algo, BundleAlgo):
-            algo_to_pickle(self.algo, template_path=self.algo.template_path, **algo_meta_data)
-        else:
-            algo_to_pickle(self.algo, **algo_meta_data)
+        algo_to_pickle(self.algo, template_path=self.algo.template_path, **algo_meta_data)
         self.set_score(acc)
 
 
 class OptunaGen(HPOGen):
     """
     Generate algorithms for the Optuna to automate hyperparameter tuning. Please refer to NNI and Optuna
     (https://optuna.readthedocs.io/en/stable/) for more information. Optuna has different running scheme
@@ -300,19 +290,15 @@
                     output_folder = os.path.dirname(algo.get_output_path())
 
                     params.update({"fill_with_datastats": False})  # just copy, not using datastats to fill
                     self.algo.export_to_disk(output_folder, name, **params)
             else:
                 self.algo = algo
 
-            if isinstance(self.algo, BundleAlgo):
-                self.obj_filename = algo_to_pickle(self.algo, template_path=self.algo.template_path)
-            else:
-                self.obj_filename = algo_to_pickle(self.algo)
-                # nni instruction unknown
+            self.obj_filename = algo_to_pickle(self.algo, template_path=self.algo.template_path)
 
     def get_obj_filename(self):
         """Return the dumped pickle object of algo."""
         return self.obj_filename
 
     def get_hyperparameters(self):
         """
@@ -395,25 +381,19 @@
                 ``{algorithm_templates_dir}/{network}/scripts/algo.py``
         """
         if not os.path.isfile(obj_filename):
             raise ValueError(f"{obj_filename} is not found")
 
         self.algo, algo_meta_data = algo_from_pickle(obj_filename, template_path=template_path)
 
-        if isinstance(self.algo, BundleAlgo):  # algo's template path needs override
-            self.algo.template_path = algo_meta_data["template_path"]
-
         # step 1 sample hyperparams
         params = self.get_hyperparameters()
         # step 2 set the update params for the algo to run in the next trial
         self.update_params(params)
         # step 3 generate the folder to save checkpoints and train
         self.generate(output_folder)
         self.algo.train(self.params)
         # step 4 report validation acc to controller
         acc = self.algo.get_score()
         algo_meta_data = {str(AlgoKeys.SCORE): acc}
-        if isinstance(self.algo, BundleAlgo):
-            algo_to_pickle(self.algo, template_path=self.algo.template_path, **algo_meta_data)
-        else:
-            algo_to_pickle(self.algo, **algo_meta_data)
+        algo_to_pickle(self.algo, template_path=self.algo.template_path, **algo_meta_data)
         self.set_score(acc)
```

### Comparing `monai-weekly-1.2.dev2317/monai/apps/auto3dseg/transforms.py` & `monai-weekly-1.2.dev2318/monai/apps/auto3dseg/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/auto3dseg/utils.py` & `monai-weekly-1.2.dev2318/monai/apps/auto3dseg/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,17 +42,14 @@
 
         obj_filename = os.path.join(write_path, "algo_object.pkl")
         if not os.path.isfile(obj_filename):  # saved mode pkl
             continue
 
         algo, algo_meta_data = algo_from_pickle(obj_filename, template_path=template_path)
 
-        if isinstance(algo, BundleAlgo):  # algo's template path needs override
-            algo.template_path = algo_meta_data["template_path"]
-
         best_metric = algo_meta_data.get(AlgoKeys.SCORE, None)
         if best_metric is None:
             try:
                 best_metric = algo.get_score()
             except BaseException:
                 pass
```

### Comparing `monai-weekly-1.2.dev2317/monai/apps/datasets.py` & `monai-weekly-1.2.dev2318/monai/apps/datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/deepedit/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/deepedit/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/deepedit/interaction.py` & `monai-weekly-1.2.dev2318/monai/apps/deepedit/interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/deepedit/transforms.py` & `monai-weekly-1.2.dev2318/monai/apps/deepedit/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/deepgrow/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/deepgrow/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/deepgrow/dataset.py` & `monai-weekly-1.2.dev2318/monai/apps/deepgrow/dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/deepgrow/interaction.py` & `monai-weekly-1.2.dev2318/monai/apps/deepgrow/interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/deepgrow/transforms.py` & `monai-weekly-1.2.dev2318/monai/apps/deepgrow/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/metrics/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/metrics/coco.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/metrics/coco.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/metrics/matching.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/metrics/matching.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/networks/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/networks/retinanet_detector.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/networks/retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/networks/retinanet_network.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/networks/retinanet_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/transforms/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/transforms/array.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/transforms/box_ops.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/transforms/box_ops.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/transforms/dictionary.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/utils/ATSS_matcher.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/utils/ATSS_matcher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/utils/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/utils/anchor_utils.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/utils/anchor_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/utils/box_coder.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/utils/box_coder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/utils/box_selector.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/utils/box_selector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/utils/detector_utils.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/utils/detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/utils/hard_negative_sampler.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/utils/hard_negative_sampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/detection/utils/predict_utils.py` & `monai-weekly-1.2.dev2318/monai/apps/detection/utils/predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/mmars/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/mmars/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/mmars/mmars.py` & `monai-weekly-1.2.dev2318/monai/apps/mmars/mmars.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/mmars/model_desc.py` & `monai-weekly-1.2.dev2318/monai/apps/mmars/model_desc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/nnunet/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/nnunet/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/nnunet/__main__.py` & `monai-weekly-1.2.dev2318/monai/apps/nnunet/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/nnunet/nnunetv2_runner.py` & `monai-weekly-1.2.dev2318/monai/apps/nnunet/nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/nnunet/utils.py` & `monai-weekly-1.2.dev2318/monai/apps/nnunet/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/nuclick/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/nuclick/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/nuclick/transforms.py` & `monai-weekly-1.2.dev2318/monai/apps/nuclick/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/engines/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/engines/utils.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/handlers/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/handlers/utils.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/inferers/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/inferers/inferer.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/losses/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/losses/hovernet_loss.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/losses/hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/metrics/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/metrics/lesion_froc.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/metrics/lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/post/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/post/array.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/post/dictionary.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/stain/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/transforms/stain/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/stain/array.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/transforms/stain/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/stain/dictionary.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/transforms/stain/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/pathology/utils.py` & `monai-weekly-1.2.dev2318/monai/apps/pathology/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/reconstruction/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/reconstruction/complex_utils.py` & `monai-weekly-1.2.dev2318/monai/apps/reconstruction/complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/reconstruction/fastmri_reader.py` & `monai-weekly-1.2.dev2318/monai/apps/reconstruction/fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/reconstruction/mri_utils.py` & `monai-weekly-1.2.dev2318/monai/apps/reconstruction/mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/blocks/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/blocks/varnetblock.py` & `monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/blocks/varnetblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py` & `monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/complex_unet.py` & `monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/nets/complex_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/utils.py` & `monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/nets/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/varnet.py` & `monai-weekly-1.2.dev2318/monai/apps/reconstruction/networks/nets/varnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/reconstruction/transforms/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/reconstruction/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/reconstruction/transforms/array.py` & `monai-weekly-1.2.dev2318/monai/apps/reconstruction/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/reconstruction/transforms/dictionary.py` & `monai-weekly-1.2.dev2318/monai/apps/reconstruction/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/tcia/__init__.py` & `monai-weekly-1.2.dev2318/monai/apps/tcia/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/tcia/label_desc.py` & `monai-weekly-1.2.dev2318/monai/apps/tcia/label_desc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/tcia/utils.py` & `monai-weekly-1.2.dev2318/monai/apps/tcia/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/apps/utils.py` & `monai-weekly-1.2.dev2318/monai/apps/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/auto3dseg/__init__.py` & `monai-weekly-1.2.dev2318/monai/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/auto3dseg/algo_gen.py` & `monai-weekly-1.2.dev2318/monai/auto3dseg/algo_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from monai.config import PathLike
 from monai.transforms import Randomizable
 
 
 class Algo:
     """
     An algorithm in this context is loosely defined as a data processing pipeline consisting of multiple components
     such as image preprocessing, followed by deep learning model training and evaluation.
     """
 
+    template_path: PathLike | None = None
+
     def set_data_stats(self, *args, **kwargs):
         """Provide dataset (and summaries) so that the model creation can depend on the input datasets."""
         pass
 
     def train(self, *args, **kwargs):
         """Read training/validation data and output a model."""
         pass
```

### Comparing `monai-weekly-1.2.dev2317/monai/auto3dseg/analyzer.py` & `monai-weekly-1.2.dev2318/monai/auto3dseg/analyzer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/auto3dseg/operations.py` & `monai-weekly-1.2.dev2318/monai/auto3dseg/operations.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/auto3dseg/seg_summarizer.py` & `monai-weekly-1.2.dev2318/monai/auto3dseg/seg_summarizer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/auto3dseg/utils.py` & `monai-weekly-1.2.dev2318/monai/auto3dseg/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+import logging
 import os
 import pickle
 import sys
-import warnings
 from copy import deepcopy
 from numbers import Number
 from typing import Any, cast
 
 import numpy as np
 import torch
 
 from monai.auto3dseg import Algo
 from monai.bundle.config_parser import ConfigParser
 from monai.bundle.utils import ID_SEP_KEY
+from monai.config import PathLike
 from monai.data.meta_tensor import MetaTensor
 from monai.transforms import CropForeground, ToCupy
 from monai.utils import min_version, optional_import
 
 __all__ = [
     "get_foreground_image",
     "get_foreground_label",
@@ -268,86 +269,106 @@
                 return verify_report_format(v[0], v_fmt[0])
             else:
                 return False
 
     return True
 
 
-def algo_to_pickle(algo: Algo, **algo_meta_data: Any) -> str:
+def algo_to_pickle(algo: Algo, template_path: PathLike | None = None, **algo_meta_data: Any) -> str:
     """
-    Export the Algo object to pickle file
+    Export the Algo object to pickle file.
 
     Args:
-        algo: Algo-like object
-        algo_meta_data: additional keyword to save into the dictionary. It may include template_path
-            which is used to instantiate the class. It may also include model training info
+        algo: Algo-like object.
+        template_path: a str path that is needed to be added to the sys.path to instantiate the class.
+        algo_meta_data: additional keyword to save into the dictionary, for example, model training info
             such as acc/best_metrics
 
     Returns:
         filename of the pickled Algo object
     """
-    data = {"algo_bytes": pickle.dumps(algo)}
+    data = {"algo_bytes": pickle.dumps(algo), "template_path": str(template_path)}
     pkl_filename = os.path.join(algo.get_output_path(), "algo_object.pkl")
     for k, v in algo_meta_data.items():
         data.update({k: v})
     data_bytes = pickle.dumps(data)
     with open(pkl_filename, "wb") as f_pi:
         f_pi.write(data_bytes)
     return pkl_filename
 
 
-def algo_from_pickle(pkl_filename: str, **kwargs: Any) -> Any:
+def algo_from_pickle(pkl_filename: str, template_path: PathLike | None = None, **kwargs: Any) -> Any:
     """
-    Import the Algo object from a pickle file
+    Import the Algo object from a pickle file.
 
     Args:
-        pkl_filename: name of the pickle file
-        algo_templates_dir: the algorithm script folder which is needed to instantiate the object.
-            If it is None, the function will use the internal ``'algo_templates_dir`` in the object
-            dict.
+        pkl_filename: the name of the pickle file.
+        template_path: a folder containing files to instantiate the Algo. Besides the `template_path`,
+        this function will also attempt to use the `template_path` saved in the pickle file and a directory
+        named `algorithm_templates` in the parent folder of the folder containing the pickle file.
 
     Returns:
-        algo: Algo-like object
+        algo: the Algo object saved in the pickle file.
+        algo_meta_data: additional keyword saved in the pickle file, for example, acc/best_metrics.
 
     Raises:
-        ValueError if the pkl_filename does not contain a dict, or the dict does not contain
-            ``template_path`` or ``algo_bytes``
+        ValueError if the pkl_filename does not contain a dict, or the dict does not contain `algo_bytes`.
+        ModuleNotFoundError if it is unable to instiante the Algo class.
+
     """
     with open(pkl_filename, "rb") as f_pi:
         data_bytes = f_pi.read()
     data = pickle.loads(data_bytes)
 
     if not isinstance(data, dict):
         raise ValueError(f"the data object is {data.__class__}. Dict is expected.")
 
     if "algo_bytes" not in data:
         raise ValueError(f"key [algo_bytes] not found in {data}. Unable to instantiate.")
 
     algo_bytes = data.pop("algo_bytes")
-    algo_meta_data = {}
+    algo_template_path = data.pop("template_path", None)
+
+    template_paths_candidates: list[str] = []
 
-    if "template_path" in kwargs:  # add template_path to sys.path
-        template_path = kwargs["template_path"]
-        if template_path is None:  # then load template_path from pickled data
-            if "template_path" not in data:
-                raise ValueError(f"key [template_path] not found in {data}")
-            template_path = data.pop("template_path")
-
-        if not os.path.isdir(template_path):
-            raise ValueError(f"Algorithm templates {template_path} is not a directory")
-        # Example of template path: "algorithm_templates/dints".
-        sys.path.insert(0, os.path.abspath(os.path.join(template_path, "..")))
-        algo_meta_data.update({"template_path": template_path})
+    if os.path.isdir(str(template_path)):
+        template_paths_candidates.append(os.path.abspath(str(template_path)))
+        template_paths_candidates.append(os.path.abspath(os.path.join(str(template_path), "..")))
+
+    if os.path.isdir(str(algo_template_path)):
+        template_paths_candidates.append(os.path.abspath(algo_template_path))
+        template_paths_candidates.append(os.path.abspath(os.path.join(algo_template_path, "..")))
 
-    algo = pickle.loads(algo_bytes)
     pkl_dir = os.path.dirname(pkl_filename)
-    if pkl_dir != algo.get_output_path():
-        warnings.warn(
-            f"{algo.get_output_path()} does not contain {pkl_filename}."
-            f"Now override the Algo output_path with: {pkl_dir}"
-        )
+    algo_template_path_fuzzy = os.path.join(pkl_dir, "..", "algorithm_templates")
+
+    if os.path.isdir(algo_template_path_fuzzy):
+        template_paths_candidates.append(os.path.abspath(algo_template_path_fuzzy))
+
+    if len(template_paths_candidates) == 0:
+        # no template_path provided or needed
+        algo = pickle.loads(algo_bytes)
+        algo.template_path = None
+    else:
+        for i, p in enumerate(template_paths_candidates):
+            try:
+                sys.path.append(p)
+                algo = pickle.loads(algo_bytes)
+                break
+            except ModuleNotFoundError as not_found_err:
+                logging.debug(f"Folder {p} doesn't contain the Algo templates for Algo instantiation.")
+                sys.path.pop()
+                if i == len(template_paths_candidates) - 1:
+                    raise ValueError(
+                        f"Failed to instantiate {pkl_filename} with {template_paths_candidates}"
+                    ) from not_found_err
+        algo.template_path = p
+
+    if os.path.abspath(pkl_dir) != os.path.abspath(algo.get_output_path()):
+        logging.debug(f"{algo.get_output_path()} is changed. Now override the Algo output_path with: {pkl_dir}.")
         algo.output_path = pkl_dir
 
+    algo_meta_data = {}
     for k, v in data.items():
         algo_meta_data.update({k: v})
 
     return algo, algo_meta_data
```

### Comparing `monai-weekly-1.2.dev2317/monai/bundle/__init__.py` & `monai-weekly-1.2.dev2318/monai/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/bundle/__main__.py` & `monai-weekly-1.2.dev2318/monai/bundle/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/bundle/config_item.py` & `monai-weekly-1.2.dev2318/monai/bundle/config_item.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/bundle/config_parser.py` & `monai-weekly-1.2.dev2318/monai/bundle/config_parser.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/bundle/properties.py` & `monai-weekly-1.2.dev2318/monai/bundle/properties.py`

 * *Files 6% similar despite different names*

```diff
@@ -155,14 +155,29 @@
         BundlePropertyConfig.ID: "bundle_root",
     },
     "device": {
         BundleProperty.DESC: "target device to execute the bundle workflow.",
         BundleProperty.REQUIRED: True,
         BundlePropertyConfig.ID: "device",
     },
+    "dataset_dir": {
+        BundleProperty.DESC: "directory path of the dataset.",
+        BundleProperty.REQUIRED: True,
+        BundlePropertyConfig.ID: "dataset_dir",
+    },
+    "dataset": {
+        BundleProperty.DESC: "PyTorch dataset object for the inference / evaluation logic.",
+        BundleProperty.REQUIRED: True,
+        BundlePropertyConfig.ID: "dataset",
+    },
+    "dataset_data": {
+        BundleProperty.DESC: "data source for the inference / evaluation dataset.",
+        BundleProperty.REQUIRED: True,
+        BundlePropertyConfig.ID: f"dataset{ID_SEP_KEY}data",
+    },
     "evaluator": {
         BundleProperty.DESC: "inference / evaluation workflow engine.",
         BundleProperty.REQUIRED: True,
         BundlePropertyConfig.ID: "evaluator",
     },
     "network_def": {
         BundleProperty.DESC: "network module for the inference.",
@@ -170,14 +185,20 @@
         BundlePropertyConfig.ID: "network_def",
     },
     "inferer": {
         BundleProperty.DESC: "MONAI Inferer object to execute the model computation in inference.",
         BundleProperty.REQUIRED: True,
         BundlePropertyConfig.ID: "inferer",
     },
+    "handlers": {
+        BundleProperty.DESC: "event-handlers for the inference / evaluation logic.",
+        BundleProperty.REQUIRED: False,
+        BundlePropertyConfig.ID: "handlers",
+        BundlePropertyConfig.REF_ID: f"evaluator{ID_SEP_KEY}val_handlers",
+    },
     "preprocessing": {
         BundleProperty.DESC: "preprocessing for the input data.",
         BundleProperty.REQUIRED: False,
         BundlePropertyConfig.ID: "preprocessing",
         BundlePropertyConfig.REF_ID: f"dataset{ID_SEP_KEY}transform",
     },
     "postprocessing": {
```

### Comparing `monai-weekly-1.2.dev2317/monai/bundle/reference_resolver.py` & `monai-weekly-1.2.dev2318/monai/bundle/reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/bundle/scripts.py` & `monai-weekly-1.2.dev2318/monai/bundle/scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -604,24 +604,30 @@
     Specify `config_file` to run monai bundle components and workflows.
 
     Typical usage examples:
 
     .. code-block:: bash
 
         # Execute this module as a CLI entry:
+        python -m monai.bundle run --meta_file <meta path> --config_file <config path>
+
+        # Execute with specified `run_id=training`:
         python -m monai.bundle run training --meta_file <meta path> --config_file <config path>
 
+        # Execute with all specified `run_id=runtest`, `init_id=inittest`, `final_id=finaltest`:
+        python -m monai.bundle run --run_id runtest --init_id inittest --final_id finaltest ...
+
         # Override config values at runtime by specifying the component id and its new value:
-        python -m monai.bundle run training --net#input_chns 1 ...
+        python -m monai.bundle run --net#input_chns 1 ...
 
         # Override config values with another config file `/path/to/another.json`:
-        python -m monai.bundle run evaluating --net %/path/to/another.json ...
+        python -m monai.bundle run --net %/path/to/another.json ...
 
         # Override config values with part content of another config file:
-        python -m monai.bundle run training --net %/data/other.json#net_arg ...
+        python -m monai.bundle run --net %/data/other.json#net_arg ...
 
         # Set default args of `run` in a JSON / YAML file, help to record and simplify the command line.
         # Other args still can override the default args at runtime:
         python -m monai.bundle run --args_file "/workspace/data/args.json" --config_file <config path>
 
     Args:
         run_id: ID name of the expected config expression to run, default to "run".
@@ -1458,15 +1464,15 @@
     with open(str(docs_dir / "README.md"), "w") as o:
         readme = """
         # Your Model Name
 
         Describe your model here and how to run it, for example using `inference.json`:
 
         ```
-        python -m monai.bundle run evaluating \
+        python -m monai.bundle run \
             --meta_file /path/to/bundle/configs/metadata.json \
             --config_file /path/to/bundle/configs/inference.json \
             --dataset_dir ./input \
             --bundle_root /path/to/bundle
         ```
         """
```

### Comparing `monai-weekly-1.2.dev2317/monai/bundle/utils.py` & `monai-weekly-1.2.dev2318/monai/bundle/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/bundle/workflows.py` & `monai-weekly-1.2.dev2318/monai/bundle/workflows.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from __future__ import annotations
 
 import os
 import time
 import warnings
 from abc import ABC, abstractmethod
+from copy import copy
 from logging.config import fileConfig
 from pathlib import Path
 from typing import Any, Sequence
 
 from monai.apps.utils import get_logger
 from monai.bundle.config_parser import ConfigParser
 from monai.bundle.properties import InferProperties, TrainProperties
@@ -49,18 +50,18 @@
 
     def __init__(self, workflow: str | None = None):
         if workflow is None:
             self.properties = None
             self.workflow = None
             return
         if workflow.lower() in self.supported_train_type:
-            self.properties = TrainProperties
+            self.properties = copy(TrainProperties)
             self.workflow = "train"
         elif workflow.lower() in self.supported_infer_type:
-            self.properties = InferProperties
+            self.properties = copy(InferProperties)
             self.workflow = "infer"
         else:
             raise ValueError(f"Unsupported workflow type: '{workflow}'.")
 
     @abstractmethod
     def initialize(self, *args: Any, **kwargs: Any) -> Any:
         """
@@ -125,14 +126,32 @@
     def get_workflow_type(self):
         """
         Get the workflow type, it can be `None`, "train", or "infer".
 
         """
         return self.workflow
 
+    def add_property(self, name: str, required: str, desc: str | None = None) -> None:
+        """
+        Besides the default predefined properties, some 3rd party aplications may need the bundle
+        definition to provide additonal properties for the specific use cases, if the bundlle can't
+        provide the property, means it can't work with the application.
+        This utility adds the property for the application requirements check and access.
+
+        Args:
+            name: the name of target property.
+            required: whether the property is "must-have".
+            desc: descriptions for the property.
+        """
+        if self.properties is None:
+            self.properties = {}
+        if name in self.properties:
+            warnings.warn(f"property '{name}' already exists in the properties list, overriding it.")
+        self.properties[name] = {BundleProperty.DESC: desc, BundleProperty.REQUIRED: required}
+
     def check_properties(self) -> list[str] | None:
         """
         Check whether the required properties are existing in the bundle workflow.
         If no workflow type specified, return None, otherwise, return a list of required but missing properties.
 
         """
         if self.properties is None:
@@ -312,14 +331,33 @@
         prop_id = self._get_prop_id(name, property)
         if prop_id is not None:
             self.parser[prop_id] = value
             # must parse the config again after changing the content
             self._is_initialized = False
             self.parser.ref_resolver.reset()
 
+    def add_property(  # type: ignore[override]
+        self, name: str, required: str, config_id: str, desc: str | None = None
+    ) -> None:
+        """
+        Besides the default predefined properties, some 3rd party aplications may need the bundle
+        definition to provide additonal properties for the specific use cases, if the bundlle can't
+        provide the property, means it can't work with the application.
+        This utility adds the property for the application requirements check and access.
+
+        Args:
+            name: the name of target property.
+            required: whether the property is "must-have".
+            config_id: the config ID of target property in the bundle definition.
+            desc: descriptions for the property.
+
+        """
+        super().add_property(name=name, required=required, desc=desc)
+        self.properties[name][BundlePropertyConfig.ID] = config_id  # type: ignore[index]
+
     def _check_optional_id(self, name: str, property: dict) -> bool:
         """
         If an optional property has reference in the config, check whether the property is existing.
         If `ValidationHandler` is defined for a training workflow, will check whether the optional properties
         "evaluator" and "val_interval" are existing.
 
         Args:
```

### Comparing `monai-weekly-1.2.dev2317/monai/config/__init__.py` & `monai-weekly-1.2.dev2318/monai/config/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/config/deviceconfig.py` & `monai-weekly-1.2.dev2318/monai/config/deviceconfig.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/config/type_definitions.py` & `monai-weekly-1.2.dev2318/monai/config/type_definitions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/__init__.py` & `monai-weekly-1.2.dev2318/monai/data/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/box_utils.py` & `monai-weekly-1.2.dev2318/monai/data/box_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/csv_saver.py` & `monai-weekly-1.2.dev2318/monai/data/csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/dataloader.py` & `monai-weekly-1.2.dev2318/monai/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/dataset.py` & `monai-weekly-1.2.dev2318/monai/data/dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/dataset_summary.py` & `monai-weekly-1.2.dev2318/monai/data/dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/decathlon_datalist.py` & `monai-weekly-1.2.dev2318/monai/data/decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/fft_utils.py` & `monai-weekly-1.2.dev2318/monai/data/fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/folder_layout.py` & `monai-weekly-1.2.dev2318/monai/data/folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/grid_dataset.py` & `monai-weekly-1.2.dev2318/monai/data/grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/image_dataset.py` & `monai-weekly-1.2.dev2318/monai/data/image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/image_reader.py` & `monai-weekly-1.2.dev2318/monai/data/image_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/image_writer.py` & `monai-weekly-1.2.dev2318/monai/data/image_writer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/iterable_dataset.py` & `monai-weekly-1.2.dev2318/monai/data/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/itk_torch_bridge.py` & `monai-weekly-1.2.dev2318/monai/data/itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/meta_obj.py` & `monai-weekly-1.2.dev2318/monai/data/meta_obj.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/meta_tensor.py` & `monai-weekly-1.2.dev2318/monai/data/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/samplers.py` & `monai-weekly-1.2.dev2318/monai/data/samplers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/synthetic.py` & `monai-weekly-1.2.dev2318/monai/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/test_time_augmentation.py` & `monai-weekly-1.2.dev2318/monai/data/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/thread_buffer.py` & `monai-weekly-1.2.dev2318/monai/data/thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/torchscript_utils.py` & `monai-weekly-1.2.dev2318/monai/data/torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/utils.py` & `monai-weekly-1.2.dev2318/monai/data/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/video_dataset.py` & `monai-weekly-1.2.dev2318/monai/data/video_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/wsi_datasets.py` & `monai-weekly-1.2.dev2318/monai/data/wsi_datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/data/wsi_reader.py` & `monai-weekly-1.2.dev2318/monai/data/wsi_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/engines/__init__.py` & `monai-weekly-1.2.dev2318/monai/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/engines/evaluator.py` & `monai-weekly-1.2.dev2318/monai/engines/evaluator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/engines/multi_gpu_supervised_trainer.py` & `monai-weekly-1.2.dev2318/monai/engines/multi_gpu_supervised_trainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/engines/trainer.py` & `monai-weekly-1.2.dev2318/monai/engines/trainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/engines/utils.py` & `monai-weekly-1.2.dev2318/monai/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/engines/workflow.py` & `monai-weekly-1.2.dev2318/monai/engines/workflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/fl/__init__.py` & `monai-weekly-1.2.dev2318/monai/fl/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/fl/client/__init__.py` & `monai-weekly-1.2.dev2318/monai/fl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/fl/client/client_algo.py` & `monai-weekly-1.2.dev2318/monai/fl/client/client_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/fl/client/monai_algo.py` & `monai-weekly-1.2.dev2318/monai/fl/client/monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/fl/utils/__init__.py` & `monai-weekly-1.2.dev2318/monai/fl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/fl/utils/constants.py` & `monai-weekly-1.2.dev2318/monai/fl/utils/constants.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/fl/utils/exchange_object.py` & `monai-weekly-1.2.dev2318/monai/fl/utils/exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/fl/utils/filters.py` & `monai-weekly-1.2.dev2318/monai/fl/utils/filters.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/__init__.py` & `monai-weekly-1.2.dev2318/monai/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/checkpoint_loader.py` & `monai-weekly-1.2.dev2318/monai/handlers/checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/checkpoint_saver.py` & `monai-weekly-1.2.dev2318/monai/handlers/checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/classification_saver.py` & `monai-weekly-1.2.dev2318/monai/handlers/classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/clearml_handlers.py` & `monai-weekly-1.2.dev2318/monai/handlers/clearml_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/confusion_matrix.py` & `monai-weekly-1.2.dev2318/monai/handlers/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/decollate_batch.py` & `monai-weekly-1.2.dev2318/monai/handlers/decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/earlystop_handler.py` & `monai-weekly-1.2.dev2318/monai/handlers/earlystop_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/garbage_collector.py` & `monai-weekly-1.2.dev2318/monai/handlers/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/hausdorff_distance.py` & `monai-weekly-1.2.dev2318/monai/handlers/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/ignite_metric.py` & `monai-weekly-1.2.dev2318/monai/handlers/ignite_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/logfile_handler.py` & `monai-weekly-1.2.dev2318/monai/handlers/logfile_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/lr_schedule_handler.py` & `monai-weekly-1.2.dev2318/monai/handlers/lr_schedule_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/mean_dice.py` & `monai-weekly-1.2.dev2318/monai/handlers/mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/mean_iou.py` & `monai-weekly-1.2.dev2318/monai/handlers/mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/metric_logger.py` & `monai-weekly-1.2.dev2318/monai/handlers/metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/metrics_reloaded_handler.py` & `monai-weekly-1.2.dev2318/monai/handlers/metrics_reloaded_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/metrics_saver.py` & `monai-weekly-1.2.dev2318/monai/handlers/metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/mlflow_handler.py` & `monai-weekly-1.2.dev2318/monai/handlers/mlflow_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,18 @@
 
 import torch
 
 from monai.config import IgniteInfo
 from monai.utils import ensure_tuple, min_version, optional_import
 
 Events, _ = optional_import("ignite.engine", IgniteInfo.OPT_IMPORT_VERSION, min_version, "Events")
-mlflow, _ = optional_import("mlflow")
-mlflow.entities, _ = optional_import("mlflow.entities")
+mlflow, _ = optional_import("mlflow", descriptor="Please install mlflow before using MLFlowHandler.")
+mlflow.entities, _ = optional_import(
+    "mlflow.entities", descriptor="Please install mlflow.entities before using MLFlowHandler."
+)
 
 if TYPE_CHECKING:
     from ignite.engine import Engine
 else:
     Engine, _ = optional_import(
         "ignite.engine", IgniteInfo.OPT_IMPORT_VERSION, min_version, "Engine", as_type="decorator"
     )
@@ -72,29 +74,31 @@
             Must accept parameter "engine", use default logger if None.
         output_transform: a callable that is used to transform the
             ``ignite.engine.state.output`` into a scalar to track, or a dictionary of {key: scalar}.
             By default this value logging happens when every iteration completed.
             The default behavior is to track loss from output[0] as output is a decollated list
             and we replicated loss value for every item of the decollated list.
             `engine.state` and `output_transform` inherit from the ignite concept:
-            https://pytorch.org/ignite/concepts.html#state, explanation and usage example are in the tutorial:
+            https://pytorch-ignite.ai/concepts/03-state/, explanation and usage example are in the tutorial:
             https://github.com/Project-MONAI/tutorials/blob/master/modules/batch_output_transform.ipynb.
         global_epoch_transform: a callable that is used to customize global epoch number.
             For example, in evaluation, the evaluator engine might want to track synced epoch number
             with the trainer engine.
         state_attributes: expected attributes from `engine.state`, if provided, will extract them
             when epoch completed.
         tag_name: when iteration output is a scalar, `tag_name` is used to track, defaults to `'Loss'`.
-        experiment_name: name for an experiment, defaults to `default_experiment`.
-        run_name: name for run in an experiment.
-        experiment_param: a dict recording parameters which will not change through whole experiment,
+        experiment_name: the experiment name of MLflow, default to `'monai_experiment'`. An experiment can be
+            used to record several runs.
+        run_name: the run name in an experiment. A run can be used to record information about a workflow,
+            like the loss, metrics and so on.
+        experiment_param: a dict recording parameters which will not change through the whole workflow,
             like torch version, cuda version and so on.
-        artifacts: paths to images that need to be recorded after a whole run.
-        optimizer_param_names: parameters' name in optimizer that need to be record during running,
-            defaults to "lr".
+        artifacts: paths to images that need to be recorded after running the workflow.
+        optimizer_param_names: parameter names in the optimizer that need to be recorded during running the
+            workflow, default to `'lr'`.
         close_on_complete: whether to close the mlflow run in `complete` phase in workflow, default to False.
 
     For more details of MLFlow usage, please refer to: https://mlflow.org/docs/latest/index.html.
 
     """
 
     # parameters that are logged at the start of training
@@ -128,14 +132,15 @@
         self.tag_name = tag_name
         self.experiment_name = experiment_name
         self.run_name = run_name
         self.experiment_param = experiment_param
         self.artifacts = ensure_tuple(artifacts)
         self.optimizer_param_names = ensure_tuple(optimizer_param_names)
         self.client = mlflow.MlflowClient(tracking_uri=tracking_uri if tracking_uri else None)
+        self.run_finish_status = mlflow.entities.RunStatus.to_string(mlflow.entities.RunStatus.FINISHED)
         self.close_on_complete = close_on_complete
         self.experiment = None
         self.cur_run = None
 
     def _delete_exist_param_in_dict(self, param_dict: dict) -> None:
         """
         Delete parameters in given dict, if they are already logged by current mlflow run.
@@ -187,14 +192,16 @@
         if not self.experiment:
             raise ValueError(f"Failed to set experiment '{self.experiment_name}' as the active experiment")
 
         if not self.cur_run:
             run_name = f"run_{time.strftime('%Y%m%d_%H%M%S')}" if self.run_name is None else self.run_name
             runs = self.client.search_runs(self.experiment.experiment_id)
             runs = [r for r in runs if r.info.run_name == run_name or not self.run_name]
+            # runs marked as finish should not record info any more
+            runs = [r for r in runs if r.info.status != self.run_finish_status]
             if runs:
                 self.cur_run = self.client.get_run(runs[-1].info.run_id)  # pick latest active run
             else:
                 self.cur_run = self.client.create_run(experiment_id=self.experiment.experiment_id, run_name=run_name)
 
         if self.experiment_param:
             self._log_params(self.experiment_param)
@@ -260,16 +267,15 @@
 
     def close(self) -> None:
         """
         Stop current running logger of MLFlow.
 
         """
         if self.cur_run:
-            status = mlflow.entities.RunStatus.to_string(mlflow.entities.RunStatus.FINISHED)
-            self.client.set_terminated(self.cur_run.info.run_id, status)
+            self.client.set_terminated(self.cur_run.info.run_id, self.run_finish_status)
             self.cur_run = None
 
     def epoch_completed(self, engine: Engine) -> None:
         """
         Handler for train or validation/evaluation epoch completed Event.
         Track epoch level log, default values are from Ignite `engine.state.metrics` dict.
```

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/nvtx_handlers.py` & `monai-weekly-1.2.dev2318/monai/handlers/nvtx_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/panoptic_quality.py` & `monai-weekly-1.2.dev2318/monai/handlers/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/parameter_scheduler.py` & `monai-weekly-1.2.dev2318/monai/handlers/parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/postprocessing.py` & `monai-weekly-1.2.dev2318/monai/handlers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/probability_maps.py` & `monai-weekly-1.2.dev2318/monai/handlers/probability_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/regression_metrics.py` & `monai-weekly-1.2.dev2318/monai/handlers/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/roc_auc.py` & `monai-weekly-1.2.dev2318/monai/handlers/roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/smartcache_handler.py` & `monai-weekly-1.2.dev2318/monai/handlers/smartcache_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/stats_handler.py` & `monai-weekly-1.2.dev2318/monai/handlers/stats_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/surface_distance.py` & `monai-weekly-1.2.dev2318/monai/handlers/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/tensorboard_handlers.py` & `monai-weekly-1.2.dev2318/monai/handlers/tensorboard_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/utils.py` & `monai-weekly-1.2.dev2318/monai/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/handlers/validation_handler.py` & `monai-weekly-1.2.dev2318/monai/handlers/validation_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/inferers/__init__.py` & `monai-weekly-1.2.dev2318/monai/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/inferers/inferer.py` & `monai-weekly-1.2.dev2318/monai/inferers/inferer.py`

 * *Files 0% similar despite different names*

```diff
@@ -457,14 +457,15 @@
             args: optional args to be passed to ``network``.
             kwargs: optional keyword args to be passed to ``network``.
 
         """
 
         device = kwargs.pop("device", self.device)
         buffer_steps = kwargs.pop("buffer_steps", self.buffer_steps)
+        buffer_dim = kwargs.pop("buffer_dim", self.buffer_dim)
 
         if device is None and self.cpu_thresh is not None and inputs.shape[2:].numel() > self.cpu_thresh:
             device = "cpu"  # stitch in cpu memory if image is too large
 
         return sliding_window_inference(
             inputs,
             self.roi_size,
@@ -477,15 +478,15 @@
             self.cval,
             self.sw_device,
             device,
             self.progress,
             self.roi_weight_map,
             None,
             buffer_steps,
-            self.buffer_dim,
+            buffer_dim,
             *args,
             **kwargs,
         )
 
 
 class SlidingWindowInfererAdapt(SlidingWindowInferer):
     """
@@ -520,22 +521,29 @@
             return super().__call__(inputs, network, *args, **kwargs)
 
         skip_buffer = self.buffer_steps is not None and self.buffer_steps <= 0
         cpu_cond = self.cpu_thresh is not None and inputs.shape[2:].numel() > self.cpu_thresh
         gpu_stitching = inputs.is_cuda and not cpu_cond
         buffered_stitching = inputs.is_cuda and cpu_cond and not skip_buffer
         buffer_steps = max(1, self.buffer_steps) if self.buffer_steps is not None else 1
+        buffer_dim = -1
+
+        sh = list(inputs.shape[2:])
+        max_dim = sh.index(max(sh))
+        if inputs.shape[max_dim + 2] / inputs.shape[-1] >= 2:
+            buffer_dim = max_dim
 
         for _ in range(10):  # at most 10 trials
             try:
                 return super().__call__(
                     inputs,
                     network,
                     device=inputs.device if gpu_stitching else torch.device("cpu"),
                     buffer_steps=buffer_steps if buffered_stitching else None,
+                    buffer_dim=buffer_dim,
                     *args,
                     **kwargs,
                 )
             except RuntimeError as e:
                 if not gpu_stitching and not buffered_stitching or "OutOfMemoryError" not in str(type(e).__name__):
                     raise e
 
@@ -543,32 +551,31 @@
 
                 if gpu_stitching:  # if failed on gpu
                     gpu_stitching = False
                     self.cpu_thresh = inputs.shape[2:].numel() - 1  # update thresh
 
                     if skip_buffer:
                         buffered_stitching = False
-                        logger.warning(f"GPU stitching failed, attempting on CPU, image dim {inputs.shape}..")
+                        logger.warning(f"GPU stitching failed, attempting on CPU, image dim {inputs.shape}.")
 
                     else:
                         buffered_stitching = True
                         self.buffer_steps = buffer_steps
                         logger.warning(
-                            f"GPU stitching failed, attempting with buffer {buffer_steps}, image dim {inputs.shape}.."
+                            f"GPU stitching failed, buffer {buffer_steps} dim {buffer_dim}, image dim {inputs.shape}."
                         )
                 elif buffer_steps > 1:
                     buffer_steps = max(1, buffer_steps // 2)
                     self.buffer_steps = buffer_steps
                     logger.warning(
-                        f"GPU buffered stitching failed, image dim {inputs.shape} reducing buffer to {buffer_steps}"
+                        f"GPU buffered stitching failed, image dim {inputs.shape} reducing buffer to {buffer_steps}."
                     )
                 else:
                     buffered_stitching = False
-                    self.buffer_steps = 0  # disable future buffer attempts
-                    logger.warning(f"GPU buffered stitching failed, attempting on CPU, image dim {inputs.shape}")
+                    logger.warning(f"GPU buffered stitching failed, attempting on CPU, image dim {inputs.shape}.")
         raise RuntimeError(  # not possible to finish after the trials
             f"SlidingWindowInfererAdapt {skip_buffer} {cpu_cond} {gpu_stitching} {buffered_stitching} {buffer_steps}"
         )
 
 
 class SaliencyInferer(Inferer):
     """
```

### Comparing `monai-weekly-1.2.dev2317/monai/inferers/merger.py` & `monai-weekly-1.2.dev2318/monai/inferers/merger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/inferers/splitter.py` & `monai-weekly-1.2.dev2318/monai/inferers/splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/inferers/utils.py` & `monai-weekly-1.2.dev2318/monai/inferers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/losses/__init__.py` & `monai-weekly-1.2.dev2318/monai/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/losses/contrastive.py` & `monai-weekly-1.2.dev2318/monai/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/losses/deform.py` & `monai-weekly-1.2.dev2318/monai/losses/deform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/losses/dice.py` & `monai-weekly-1.2.dev2318/monai/losses/dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/losses/ds_loss.py` & `monai-weekly-1.2.dev2318/monai/losses/ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/losses/focal_loss.py` & `monai-weekly-1.2.dev2318/monai/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/losses/giou_loss.py` & `monai-weekly-1.2.dev2318/monai/losses/giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/losses/image_dissimilarity.py` & `monai-weekly-1.2.dev2318/monai/losses/image_dissimilarity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/losses/multi_scale.py` & `monai-weekly-1.2.dev2318/monai/losses/multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/losses/spatial_mask.py` & `monai-weekly-1.2.dev2318/monai/losses/spatial_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/losses/ssim_loss.py` & `monai-weekly-1.2.dev2318/monai/losses/ssim_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/losses/tversky.py` & `monai-weekly-1.2.dev2318/monai/losses/tversky.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/losses/unified_focal_loss.py` & `monai-weekly-1.2.dev2318/monai/losses/unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/__init__.py` & `monai-weekly-1.2.dev2318/monai/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/active_learning_metrics.py` & `monai-weekly-1.2.dev2318/monai/metrics/active_learning_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/confusion_matrix.py` & `monai-weekly-1.2.dev2318/monai/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/cumulative_average.py` & `monai-weekly-1.2.dev2318/monai/metrics/cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/f_beta_score.py` & `monai-weekly-1.2.dev2318/monai/metrics/f_beta_score.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/froc.py` & `monai-weekly-1.2.dev2318/monai/metrics/froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/generalized_dice.py` & `monai-weekly-1.2.dev2318/monai/metrics/generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/hausdorff_distance.py` & `monai-weekly-1.2.dev2318/monai/metrics/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/loss_metric.py` & `monai-weekly-1.2.dev2318/monai/metrics/loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/meandice.py` & `monai-weekly-1.2.dev2318/monai/metrics/meandice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/meaniou.py` & `monai-weekly-1.2.dev2318/monai/metrics/meaniou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/metric.py` & `monai-weekly-1.2.dev2318/monai/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/panoptic_quality.py` & `monai-weekly-1.2.dev2318/monai/metrics/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/regression.py` & `monai-weekly-1.2.dev2318/monai/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/rocauc.py` & `monai-weekly-1.2.dev2318/monai/metrics/rocauc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/surface_dice.py` & `monai-weekly-1.2.dev2318/monai/metrics/surface_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/surface_distance.py` & `monai-weekly-1.2.dev2318/monai/metrics/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/utils.py` & `monai-weekly-1.2.dev2318/monai/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/metrics/wrapper.py` & `monai-weekly-1.2.dev2318/monai/metrics/wrapper.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/__init__.py` & `monai-weekly-1.2.dev2318/monai/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/__init__.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/acti_norm.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/acti_norm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/activation.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/activation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/aspp.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/aspp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/backbone_fpn_utils.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/backbone_fpn_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/convolutions.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/convolutions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/crf.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/crf.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/denseblock.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/denseblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/dints_block.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/dints_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/downsample.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/downsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/dynunet_block.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/encoder.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/encoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/fcn.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/fcn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/feature_pyramid_network.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/feature_pyramid_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/fft_utils_t.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/fft_utils_t.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/localnet_block.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/mlp.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/mlp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/patchembedding.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/regunet_block.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/segresnet_block.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/selfattention.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/selfattention.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/squeeze_and_excitation.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/text_embedding.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/text_embedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/transformerblock.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/unetr_block.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/upsample.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/upsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/blocks/warp.py` & `monai-weekly-1.2.dev2318/monai/networks/blocks/warp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/layers/__init__.py` & `monai-weekly-1.2.dev2318/monai/networks/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/layers/convutils.py` & `monai-weekly-1.2.dev2318/monai/networks/layers/convutils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/layers/drop_path.py` & `monai-weekly-1.2.dev2318/monai/networks/layers/drop_path.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/layers/factories.py` & `monai-weekly-1.2.dev2318/monai/networks/layers/factories.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/layers/filtering.py` & `monai-weekly-1.2.dev2318/monai/networks/layers/filtering.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/layers/gmm.py` & `monai-weekly-1.2.dev2318/monai/networks/layers/gmm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/layers/simplelayers.py` & `monai-weekly-1.2.dev2318/monai/networks/layers/simplelayers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/layers/spatial_transforms.py` & `monai-weekly-1.2.dev2318/monai/networks/layers/spatial_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/layers/utils.py` & `monai-weekly-1.2.dev2318/monai/networks/layers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/layers/weight_init.py` & `monai-weekly-1.2.dev2318/monai/networks/layers/weight_init.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/__init__.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/ahnet.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/ahnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/attentionunet.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/autoencoder.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/basic_unet.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/basic_unetplusplus.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/classifier.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/classifier.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/densenet.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/densenet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/dints.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/dints.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/dynunet.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/dynunet.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,18 +265,19 @@
         else:
             self.filters = filters[: len(self.strides)]
 
     def forward(self, x):
         out = self.skip_layers(x)
         out = self.output_block(out)
         if self.training and self.deep_supervision:
-            out_all = [out]
-            for feature_map in self.heads:
-                out_all.append(interpolate(feature_map, out.shape[2:]))
-            return torch.stack(out_all, dim=1)
+            out_all = torch.zeros(out.shape[0], len(self.heads) + 1, *out.shape[1:], device=out.device, dtype=out.dtype)
+            out_all[:, 0] = out
+            for idx, feature_map in enumerate(self.heads):
+                out_all[:, idx + 1] = interpolate(feature_map, out.shape[2:])
+            return out_all
         return out
 
     def get_input_block(self):
         return self.conv_block(
             self.spatial_dims,
             self.in_channels,
             self.filters[0],
```

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/efficientnet.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/flexible_unet.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/fullyconnectednet.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/generator.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/generator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/highresnet.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/highresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/hovernet.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/milmodel.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/milmodel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/netadapter.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/netadapter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/regressor.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/regressor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/regunet.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/regunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/resnet.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/resnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/segresnet.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/segresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/segresnet_ds.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/senet.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/senet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/swin_unetr.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/torchvision_fc.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/torchvision_fc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/transchex.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/transchex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/unet.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/unetr.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/varautoencoder.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/vit.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/vit.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/vitautoenc.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/vitautoenc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/nets/vnet.py` & `monai-weekly-1.2.dev2318/monai/networks/nets/vnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/networks/utils.py` & `monai-weekly-1.2.dev2318/monai/networks/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/optimizers/__init__.py` & `monai-weekly-1.2.dev2318/monai/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/optimizers/lr_finder.py` & `monai-weekly-1.2.dev2318/monai/optimizers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/optimizers/lr_scheduler.py` & `monai-weekly-1.2.dev2318/monai/optimizers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/optimizers/novograd.py` & `monai-weekly-1.2.dev2318/monai/optimizers/novograd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/optimizers/utils.py` & `monai-weekly-1.2.dev2318/monai/optimizers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/__init__.py` & `monai-weekly-1.2.dev2318/monai/transforms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -656,14 +656,15 @@
     rand_choice,
     remove_small_objects,
     rescale_array,
     rescale_array_int_max,
     rescale_instance_array,
     reset_ops_id,
     resize_center,
+    resolves_modes,
     sync_meta_info,
     weighted_patch_samples,
     zero_margins,
 )
 from .utils_pytorch_numpy_unification import (
     allclose,
     any_np_pt,
```

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/adaptors.py` & `monai-weekly-1.2.dev2318/monai/transforms/adaptors.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/compose.py` & `monai-weekly-1.2.dev2318/monai/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/croppad/__init__.py` & `monai-weekly-1.2.dev2318/monai/transforms/croppad/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/croppad/array.py` & `monai-weekly-1.2.dev2318/monai/transforms/croppad/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/croppad/batch.py` & `monai-weekly-1.2.dev2318/monai/transforms/croppad/batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/croppad/dictionary.py` & `monai-weekly-1.2.dev2318/monai/transforms/croppad/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/croppad/functional.py` & `monai-weekly-1.2.dev2318/monai/transforms/croppad/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/intensity/__init__.py` & `monai-weekly-1.2.dev2318/monai/transforms/intensity/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/intensity/array.py` & `monai-weekly-1.2.dev2318/monai/transforms/intensity/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/intensity/dictionary.py` & `monai-weekly-1.2.dev2318/monai/transforms/intensity/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/inverse.py` & `monai-weekly-1.2.dev2318/monai/transforms/inverse.py`

 * *Files 4% similar despite different names*

```diff
@@ -222,20 +222,26 @@
             else:
                 info[LazyAttr.AFFINE] = affine
             info[LazyAttr.AFFINE] = convert_to_tensor(info[LazyAttr.AFFINE], device=torch.device("cpu"))
             out_obj.push_pending_operation(info)
         else:
             if out_obj.pending_operations:
                 transform_name = info.get(TraceKeys.CLASS_NAME, "") if isinstance(info, dict) else ""
-                warnings.warn(
+                msg = (
                     f"Applying transform {transform_name} to a MetaTensor with pending operations "
                     "is not supported (as this eventually changes the ordering of applied_operations when the pending "
                     f"operations are executed). Please clear the pending operations before transform {transform_name}."
                     f"\nPending operations: {[x.get(TraceKeys.CLASS_NAME) for x in out_obj.pending_operations]}."
                 )
+                pend = out_obj.pending_operations[-1]
+                if not isinstance(pend.get(TraceKeys.EXTRA_INFO), dict):
+                    pend[TraceKeys.EXTRA_INFO] = dict(pend.get(TraceKeys.EXTRA_INFO, {}))
+                if not isinstance(info.get(TraceKeys.EXTRA_INFO), dict):
+                    info[TraceKeys.EXTRA_INFO] = dict(info.get(TraceKeys.EXTRA_INFO, {}))
+                info[TraceKeys.EXTRA_INFO]["warn"] = pend[TraceKeys.EXTRA_INFO]["warn"] = msg
             out_obj.push_applied_operation(info)
         if isinstance(data, Mapping):
             if not isinstance(data, dict):
                 data = dict(data)
             if isinstance(data_t, MetaTensor):
                 data[key] = data_t.copy_meta_from(out_obj)
             else:
@@ -251,14 +257,17 @@
         xform_id = transform.get(TraceKeys.ID, "")
         if xform_id == id(self):
             return
         # TraceKeys.NONE to skip the id check
         if xform_id == TraceKeys.NONE:
             return
         xform_name = transform.get(TraceKeys.CLASS_NAME, "")
+        warning_msg = transform.get(TraceKeys.EXTRA_INFO, {}).get("warn")
+        if warning_msg:
+            warnings.warn(warning_msg)
         # basic check if multiprocessing uses 'spawn' (objects get recreated so don't have same ID)
         if torch.multiprocessing.get_start_method() in ("spawn", None) and xform_name == self.__class__.__name__:
             return
         raise RuntimeError(
             f"Error {self.__class__.__name__} getting the most recently "
             f"applied invertible transform {xform_name} {xform_id} != {id(self)}."
         )
```

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/inverse_batch_transform.py` & `monai-weekly-1.2.dev2318/monai/transforms/inverse_batch_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/io/__init__.py` & `monai-weekly-1.2.dev2318/monai/transforms/io/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/io/array.py` & `monai-weekly-1.2.dev2318/monai/transforms/io/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/io/dictionary.py` & `monai-weekly-1.2.dev2318/monai/transforms/io/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/lazy/__init__.py` & `monai-weekly-1.2.dev2318/monai/transforms/lazy/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/lazy/functional.py` & `monai-weekly-1.2.dev2318/monai/transforms/lazy/functional.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from __future__ import annotations
 
 from typing import Any
 
 import torch
 
 from monai.data.meta_tensor import MetaTensor
+from monai.data.utils import to_affine_nd
 from monai.transforms.lazy.utils import (
     affine_from_pending,
     combine_transforms,
     is_compatible_apply_kwargs,
     kwargs_from_pending,
     resample,
 )
@@ -74,14 +75,17 @@
         data.clear_pending_operations()
     pending = [] if pending is None else pending
 
     if not pending:
         return data, []
 
     cumulative_xform = affine_from_pending(pending[0])
+    if cumulative_xform.shape[0] == 3:
+        cumulative_xform = to_affine_nd(3, cumulative_xform)
+
     cur_kwargs = kwargs_from_pending(pending[0])
     override_kwargs: dict[str, Any] = {}
     if "mode" in overrides:
         override_kwargs[LazyAttr.INTERP_MODE] = overrides["mode"]
     if "padding_mode" in overrides:
         override_kwargs[LazyAttr.PADDING_MODE] = overrides["padding_mode"]
     if "align_corners" in overrides:
@@ -96,14 +100,16 @@
         new_kwargs = kwargs_from_pending(p)
         if not is_compatible_apply_kwargs(cur_kwargs, new_kwargs):
             # carry out an intermediate resample here due to incompatibility between arguments
             _cur_kwargs = cur_kwargs.copy()
             _cur_kwargs.update(override_kwargs)
             data = resample(data.to(device), cumulative_xform, _cur_kwargs)
         next_matrix = affine_from_pending(p)
+        if next_matrix.shape[0] == 3:
+            next_matrix = to_affine_nd(3, next_matrix)
         cumulative_xform = combine_transforms(cumulative_xform, next_matrix)
         cur_kwargs.update(new_kwargs)
     cur_kwargs.update(override_kwargs)
     data = resample(data.to(device), cumulative_xform, cur_kwargs)
     if isinstance(data, MetaTensor):
         for p in pending:
             data.push_applied_operation(p)
```

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/lazy/utils.py` & `monai-weekly-1.2.dev2318/monai/transforms/lazy/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/meta_utility/__init__.py` & `monai-weekly-1.2.dev2318/monai/transforms/meta_utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/meta_utility/dictionary.py` & `monai-weekly-1.2.dev2318/monai/transforms/meta_utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/nvtx.py` & `monai-weekly-1.2.dev2318/monai/transforms/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/post/__init__.py` & `monai-weekly-1.2.dev2318/monai/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/post/array.py` & `monai-weekly-1.2.dev2318/monai/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/post/dictionary.py` & `monai-weekly-1.2.dev2318/monai/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/signal/__init__.py` & `monai-weekly-1.2.dev2318/monai/transforms/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/signal/array.py` & `monai-weekly-1.2.dev2318/monai/transforms/signal/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/smooth_field/__init__.py` & `monai-weekly-1.2.dev2318/monai/transforms/smooth_field/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/smooth_field/array.py` & `monai-weekly-1.2.dev2318/monai/transforms/smooth_field/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/smooth_field/dictionary.py` & `monai-weekly-1.2.dev2318/monai/transforms/smooth_field/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/spatial/__init__.py` & `monai-weekly-1.2.dev2318/monai/transforms/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/spatial/array.py` & `monai-weekly-1.2.dev2318/monai/transforms/spatial/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 A collection of "vanilla" transforms for spatial operations
 https://github.com/Project-MONAI/MONAI/wiki/MONAI_Design
 """
 
 from __future__ import annotations
 
-import functools
 import warnings
 from collections.abc import Callable
 from copy import deepcopy
 from itertools import zip_longest
 from typing import Any, Optional, Sequence, Tuple, Union, cast
 
 import numpy as np
@@ -50,24 +49,23 @@
     create_control_grid,
     create_grid,
     create_rotate,
     create_scale,
     create_shear,
     create_translate,
     map_spatial_axes,
+    resolves_modes,
     scale_affine,
 )
 from monai.transforms.utils_pytorch_numpy_unification import argsort, argwhere, linalg_inv, moveaxis
 from monai.utils import (
     GridSampleMode,
     GridSamplePadMode,
     InterpolateMode,
-    NdimageMode,
     NumpyPadMode,
-    SplineMode,
     convert_to_cupy,
     convert_to_dst_type,
     convert_to_numpy,
     convert_to_tensor,
     ensure_tuple,
     ensure_tuple_rep,
     ensure_tuple_size,
@@ -691,15 +689,15 @@
         align_corners: bool | None = None,
         anti_aliasing: bool = False,
         anti_aliasing_sigma: Sequence[float] | float | None = None,
         dtype: DtypeLike | torch.dtype = torch.float32,
     ) -> None:
         self.size_mode = look_up_option(size_mode, ["all", "longest"])
         self.spatial_size = spatial_size
-        self.mode: InterpolateMode = look_up_option(mode, InterpolateMode)
+        self.mode = mode
         self.align_corners = align_corners
         self.anti_aliasing = anti_aliasing
         self.anti_aliasing_sigma = anti_aliasing_sigma
         self.dtype = dtype
 
     def __call__(
         self,
@@ -755,15 +753,15 @@
         else:  # for the "longest" mode
             img_size = img.peek_pending_shape() if isinstance(img, MetaTensor) else img.shape[1:]
             if not isinstance(self.spatial_size, int):
                 raise ValueError("spatial_size must be an int number if size_mode is 'longest'.")
             scale = self.spatial_size / max(img_size)
             sp_size = tuple(int(round(s * scale)) for s in img_size)
 
-        _mode = look_up_option(self.mode if mode is None else mode, InterpolateMode)
+        _mode = self.mode if mode is None else mode
         _align_corners = self.align_corners if align_corners is None else align_corners
         _dtype = get_equivalent_dtype(dtype or self.dtype or img.dtype, torch.Tensor)
         return resize(  # type: ignore
             img,
             sp_size,
             _mode,
             _align_corners,
@@ -827,16 +825,16 @@
         mode: str = GridSampleMode.BILINEAR,
         padding_mode: str = GridSamplePadMode.BORDER,
         align_corners: bool = False,
         dtype: DtypeLike | torch.dtype = torch.float32,
     ) -> None:
         self.angle = angle
         self.keep_size = keep_size
-        self.mode: str = look_up_option(mode, GridSampleMode)
-        self.padding_mode: str = look_up_option(padding_mode, GridSamplePadMode)
+        self.mode: str = mode
+        self.padding_mode: str = padding_mode
         self.align_corners = align_corners
         self.dtype = dtype
 
     def __call__(
         self,
         img: torch.Tensor,
         mode: str | None = None,
@@ -863,16 +861,16 @@
 
         Raises:
             ValueError: When ``img`` spatially is not one of [2D, 3D].
 
         """
         img = convert_to_tensor(img, track_meta=get_track_meta())
         _dtype = get_equivalent_dtype(dtype or self.dtype or img.dtype, torch.Tensor)
-        _mode = look_up_option(mode or self.mode, GridSampleMode)
-        _padding_mode = look_up_option(padding_mode or self.padding_mode, GridSamplePadMode)
+        _mode = mode or self.mode
+        _padding_mode = padding_mode or self.padding_mode
         _align_corners = self.align_corners if align_corners is None else align_corners
         im_shape = img.peek_pending_shape() if isinstance(img, MetaTensor) else img.shape[1:]
         output_shape = im_shape if self.keep_size else None
         return rotate(  # type: ignore
             img, self.angle, output_shape, _mode, _padding_mode, _align_corners, _dtype, self.get_transform_info()
         )
 
@@ -884,18 +882,19 @@
         fwd_rot_mat = transform[TraceKeys.EXTRA_INFO]["rot_mat"]
         mode = transform[TraceKeys.EXTRA_INFO]["mode"]
         padding_mode = transform[TraceKeys.EXTRA_INFO]["padding_mode"]
         align_corners = transform[TraceKeys.EXTRA_INFO]["align_corners"]
         dtype = transform[TraceKeys.EXTRA_INFO]["dtype"]
         inv_rot_mat = linalg_inv(convert_to_numpy(fwd_rot_mat))
 
+        _, _m, _p, _ = resolves_modes(mode, padding_mode)
         xform = AffineTransform(
             normalized=False,
-            mode=mode,
-            padding_mode=padding_mode,
+            mode=_m,
+            padding_mode=_p,
             align_corners=False if align_corners == TraceKeys.NONE else align_corners,
             reverse_indexing=True,
         )
         img_t: torch.Tensor = convert_data_type(data, MetaTensor, dtype=dtype)[0]
         transform_t, *_ = convert_to_dst_type(inv_rot_mat, img_t)
         sp_size = transform[TraceKeys.ORIG_SIZE]
         out: torch.Tensor = xform(img_t.unsqueeze(0), transform_t, spatial_size=sp_size).float().squeeze(0)
@@ -949,15 +948,15 @@
         padding_mode: str = NumpyPadMode.EDGE,
         align_corners: bool | None = None,
         dtype: DtypeLike | torch.dtype = torch.float32,
         keep_size: bool = True,
         **kwargs,
     ) -> None:
         self.zoom = zoom
-        self.mode: InterpolateMode = InterpolateMode(mode)
+        self.mode = mode
         self.padding_mode = padding_mode
         self.align_corners = align_corners
         self.dtype = dtype
         self.keep_size = keep_size
         self.kwargs = kwargs
 
     def __call__(
@@ -987,15 +986,15 @@
                 See also: https://pytorch.org/docs/stable/generated/torch.nn.functional.interpolate.html
             dtype: data type for resampling computation. Defaults to ``self.dtype``.
                 If None, use the data type of input data.
 
         """
         img = convert_to_tensor(img, track_meta=get_track_meta())
         _zoom = ensure_tuple_rep(self.zoom, img.ndim - 1)  # match the spatial image dim
-        _mode = look_up_option(self.mode if mode is None else mode, InterpolateMode).value
+        _mode = self.mode if mode is None else mode
         _padding_mode = padding_mode or self.padding_mode
         _align_corners = self.align_corners if align_corners is None else align_corners
         _dtype = get_equivalent_dtype(dtype or self.dtype or img.dtype, torch.Tensor)
         return zoom(  # type: ignore
             img, _zoom, self.keep_size, _mode, _padding_mode, _align_corners, _dtype, self.get_transform_info()
         )
 
@@ -1177,16 +1176,16 @@
         if len(self.range_y) == 1:
             self.range_y = tuple(sorted([-self.range_y[0], self.range_y[0]]))
         self.range_z = ensure_tuple(range_z)
         if len(self.range_z) == 1:
             self.range_z = tuple(sorted([-self.range_z[0], self.range_z[0]]))
 
         self.keep_size = keep_size
-        self.mode: str = look_up_option(mode, GridSampleMode)
-        self.padding_mode: str = look_up_option(padding_mode, GridSamplePadMode)
+        self.mode: str = mode
+        self.padding_mode: str = padding_mode
         self.align_corners = align_corners
         self.dtype = dtype
 
         self.x = 0.0
         self.y = 0.0
         self.z = 0.0
 
@@ -1227,16 +1226,16 @@
             self.randomize()
 
         if self._do_transform:
             ndim = len(img.peek_pending_shape() if isinstance(img, MetaTensor) else img.shape[1:])
             rotator = Rotate(
                 angle=self.x if ndim == 2 else (self.x, self.y, self.z),
                 keep_size=self.keep_size,
-                mode=look_up_option(mode or self.mode, GridSampleMode),
-                padding_mode=look_up_option(padding_mode or self.padding_mode, GridSamplePadMode),
+                mode=mode or self.mode,
+                padding_mode=padding_mode or self.padding_mode,
                 align_corners=self.align_corners if align_corners is None else align_corners,
                 dtype=dtype or self.dtype or img.dtype,
             )
             rotator.lazy_evaluation = self.lazy_evaluation
             out = rotator(img)
         else:
             out = convert_to_tensor(img, track_meta=get_track_meta(), dtype=torch.float32)
@@ -1402,15 +1401,15 @@
         RandomizableTransform.__init__(self, prob)
         self.min_zoom = ensure_tuple(min_zoom)
         self.max_zoom = ensure_tuple(max_zoom)
         if len(self.min_zoom) != len(self.max_zoom):
             raise ValueError(
                 f"min_zoom and max_zoom must have same length, got {len(self.min_zoom)} and {len(self.max_zoom)}."
             )
-        self.mode: InterpolateMode = look_up_option(mode, InterpolateMode)
+        self.mode = mode
         self.padding_mode = padding_mode
         self.align_corners = align_corners
         self.dtype = dtype
         self.keep_size = keep_size
         self.kwargs = kwargs
 
         self._zoom: Sequence[float] = [1.0]
@@ -1463,15 +1462,15 @@
 
         if not self._do_transform:
             out = convert_to_tensor(img, track_meta=get_track_meta(), dtype=torch.float32)
         else:
             xform = Zoom(
                 self._zoom,
                 keep_size=self.keep_size,
-                mode=look_up_option(mode or self.mode, InterpolateMode),
+                mode=mode or self.mode,
                 padding_mode=padding_mode or self.padding_mode,
                 align_corners=self.align_corners if align_corners is None else align_corners,
                 dtype=dtype or self.dtype,
                 **self.kwargs,
             )
             xform.lazy_evaluation = self.lazy_evaluation
             out = xform(img)
@@ -1811,43 +1810,14 @@
         self.mode = mode
         self.padding_mode = padding_mode
         self.norm_coords = norm_coords
         self.device = device
         self.align_corners = align_corners
         self.dtype = dtype
 
-    @staticmethod
-    @functools.lru_cache(None)
-    def resolve_modes(interp_mode, padding_mode):
-        """compute the backend and the corresponding mode for the given interpolation mode and padding mode."""
-        _interp_mode = None
-        _padding_mode = None
-        if look_up_option(str(interp_mode), SplineMode, default=None) is not None:
-            backend = TransformBackends.NUMPY
-        else:
-            backend = TransformBackends.TORCH
-
-        if (not USE_COMPILED) and (backend == TransformBackends.TORCH):
-            if str(interp_mode).lower().endswith("linear"):
-                _interp_mode = GridSampleMode("bilinear")
-            _interp_mode = GridSampleMode(interp_mode)
-            _padding_mode = GridSamplePadMode(padding_mode)
-        elif USE_COMPILED and backend == TransformBackends.TORCH:  # compiled is using torch backend param name
-            _padding_mode = 1 if padding_mode == "reflection" else padding_mode  # type: ignore
-            if interp_mode == "bicubic":
-                _interp_mode = 3  # type: ignore
-            elif interp_mode == "bilinear":
-                _interp_mode = 1  # type: ignore
-            else:
-                _interp_mode = GridSampleMode(interp_mode)
-        else:  # TransformBackends.NUMPY
-            _interp_mode = int(interp_mode)  # type: ignore
-            _padding_mode = look_up_option(padding_mode, NdimageMode)
-        return backend, _interp_mode, _padding_mode
-
     def __call__(
         self,
         img: torch.Tensor,
         grid: torch.Tensor | None = None,
         mode: str | int | None = None,
         padding_mode: str | None = None,
         dtype: DtypeLike = None,
@@ -1890,16 +1860,19 @@
             return img
 
         _device = img.device if isinstance(img, torch.Tensor) else self.device
         _dtype = dtype or self.dtype or img.dtype
         _align_corners = self.align_corners if align_corners is None else align_corners
         img_t, *_ = convert_data_type(img, torch.Tensor, dtype=_dtype, device=_device)
         sr = min(len(img_t.peek_pending_shape() if isinstance(img_t, MetaTensor) else img_t.shape[1:]), 3)
-        backend, _interp_mode, _padding_mode = Resample.resolve_modes(
-            self.mode if mode is None else mode, self.padding_mode if padding_mode is None else padding_mode
+        backend, _interp_mode, _padding_mode, _ = resolves_modes(
+            self.mode if mode is None else mode,
+            self.padding_mode if padding_mode is None else padding_mode,
+            backend=None,
+            use_compiled=USE_COMPILED,
         )
 
         if USE_COMPILED or backend == TransformBackends.NUMPY:
             grid_t, *_ = convert_to_dst_type(grid[:sr], img_t, dtype=grid.dtype, wrap_sequence=True)
             if isinstance(grid, torch.Tensor) and grid_t.data_ptr() == grid.data_ptr():
                 grid_t = grid_t.clone(memory_format=torch.contiguous_format)
             for i, dim in enumerate(img_t.shape[1 : 1 + sr]):
```

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/spatial/dictionary.py` & `monai-weekly-1.2.dev2318/monai/transforms/spatial/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/spatial/functional.py` & `monai-weekly-1.2.dev2318/monai/transforms/spatial/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from monai.data.meta_obj import get_track_meta
 from monai.data.meta_tensor import MetaTensor
 from monai.data.utils import AFFINE_TOL, compute_shape_offset, to_affine_nd
 from monai.networks.layers import AffineTransform
 from monai.transforms.croppad.array import ResizeWithPadOrCrop
 from monai.transforms.intensity.array import GaussianSmooth
 from monai.transforms.inverse import TraceableTransform
-from monai.transforms.utils import create_rotate, create_translate, scale_affine
+from monai.transforms.utils import create_rotate, create_translate, resolves_modes, scale_affine
 from monai.transforms.utils_pytorch_numpy_unification import allclose
 from monai.utils import (
     LazyAttr,
     TraceKeys,
     convert_to_dst_type,
     convert_to_numpy,
     convert_to_tensor,
@@ -168,16 +168,17 @@
             image_only=True,
             dtype=dtype_pt,
             align_corners=align_corners,
         )
         with affine_xform.trace_transform(False):
             img = affine_xform(img, mode=mode, padding_mode=padding_mode)
     else:
+        _, _m, _p, _ = resolves_modes(mode, padding_mode)
         affine_xform = AffineTransform(  # type: ignore
-            normalized=False, mode=mode, padding_mode=padding_mode, align_corners=align_corners, reverse_indexing=True
+            normalized=False, mode=_m, padding_mode=_p, align_corners=align_corners, reverse_indexing=True
         )
         img = affine_xform(img.unsqueeze(0), theta=xform.to(img), spatial_size=spatial_size).squeeze(0)  # type: ignore
     if additional_dims:
         full_shape = (chns, *spatial_size, *additional_dims)
         img = img.reshape(full_shape)
     out = _maybe_new_metatensor(img, dtype=torch.float32)
     return out.copy_meta_from(meta_info) if isinstance(out, MetaTensor) else out  # type: ignore
@@ -327,16 +328,17 @@
         else:
             # if sigma is given, use the given value for downsampling axis
             anti_aliasing_sigma = list(ensure_tuple_rep(anti_aliasing_sigma, len(out_size)))
             for axis in range(len(out_size)):
                 anti_aliasing_sigma[axis] = anti_aliasing_sigma[axis] * int(factors[axis] > 1)
         anti_aliasing_filter = GaussianSmooth(sigma=anti_aliasing_sigma)
         img_ = convert_to_tensor(anti_aliasing_filter(img_), track_meta=False)
+    _, _m, _, _ = resolves_modes(mode, torch_interpolate_spatial_nd=len(img_.shape) - 1)
     resized = torch.nn.functional.interpolate(
-        input=img_.unsqueeze(0), size=out_size, mode=mode, align_corners=align_corners
+        input=img_.unsqueeze(0), size=out_size, mode=_m, align_corners=align_corners
     )
     out, *_ = convert_to_dst_type(resized.squeeze(0), out, dtype=torch.float32)
     return out.copy_meta_from(meta_info) if isinstance(out, MetaTensor) else out
 
 
 def rotate(img, angle, output_shape, mode, padding_mode, align_corners, dtype, transform_info):
     """
@@ -392,16 +394,17 @@
         orig_size=im_shape,
         transform_info=transform_info,
         lazy_evaluation=transform_info.get(TraceKeys.LAZY_EVALUATION, False),
     )
     out = _maybe_new_metatensor(img)
     if transform_info.get(TraceKeys.LAZY_EVALUATION, False):
         return out.copy_meta_from(meta_info) if isinstance(out, MetaTensor) else meta_info
+    _, _m, _p, _ = resolves_modes(mode, padding_mode)
     xform = AffineTransform(
-        normalized=False, mode=mode, padding_mode=padding_mode, align_corners=align_corners, reverse_indexing=True
+        normalized=False, mode=_m, padding_mode=_p, align_corners=align_corners, reverse_indexing=True
     )
     img_t = out.to(dtype)
     transform_t, *_ = convert_to_dst_type(transform, img_t)
     output: torch.Tensor = xform(img_t.unsqueeze(0), transform_t, spatial_size=tuple(int(i) for i in output_shape))
     output = output.float().squeeze(0)
     out, *_ = convert_to_dst_type(output, dst=out, dtype=torch.float32)
     return out.copy_meta_from(meta_info) if isinstance(out, MetaTensor) else out
@@ -464,19 +467,20 @@
         transform_info=transform_info,
         lazy_evaluation=transform_info.get(TraceKeys.LAZY_EVALUATION, False),
     )
     out = _maybe_new_metatensor(img)
     if transform_info.get(TraceKeys.LAZY_EVALUATION, False):
         return out.copy_meta_from(meta_info) if isinstance(out, MetaTensor) else meta_info
     img_t = out.to(dtype)
+    _, _m, _, _ = resolves_modes(mode, torch_interpolate_spatial_nd=len(img_t.shape) - 1)
     zoomed: NdarrayOrTensor = torch.nn.functional.interpolate(
         recompute_scale_factor=True,
         input=img_t.unsqueeze(0),
         scale_factor=list(scale_factor),
-        mode=mode,
+        mode=_m,
         align_corners=align_corners,
     ).squeeze(0)
     out, *_ = convert_to_dst_type(zoomed, dst=out, dtype=torch.float32)
     if isinstance(out, MetaTensor):
         out = out.copy_meta_from(meta_info)
     do_pad_crop = not np.allclose(output_size, zoomed.shape[1:])
     if do_pad_crop:
```

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/traits.py` & `monai-weekly-1.2.dev2318/monai/transforms/traits.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/transform.py` & `monai-weekly-1.2.dev2318/monai/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/utility/__init__.py` & `monai-weekly-1.2.dev2318/monai/transforms/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/utility/array.py` & `monai-weekly-1.2.dev2318/monai/transforms/utility/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/utility/dictionary.py` & `monai-weekly-1.2.dev2318/monai/transforms/utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/utils.py` & `monai-weekly-1.2.dev2318/monai/transforms/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from __future__ import annotations
 
 import itertools
 import random
 import warnings
 from collections.abc import Callable, Hashable, Iterable, Mapping, Sequence
 from contextlib import contextmanager
-from functools import wraps
+from functools import lru_cache, wraps
 from inspect import getmembers, isclass
 from typing import Any
 
 import numpy as np
 import torch
 
 import monai
@@ -40,28 +40,32 @@
     searchsorted,
     unique,
     unravel_index,
     where,
 )
 from monai.utils import (
     GridSampleMode,
+    GridSamplePadMode,
     InterpolateMode,
+    NdimageMode,
     NumpyPadMode,
     PostFix,
     PytorchPadMode,
+    SplineMode,
     TraceKeys,
     ensure_tuple,
     ensure_tuple_rep,
     ensure_tuple_size,
     fall_back_tuple,
     get_equivalent_dtype,
     issequenceiterable,
     look_up_option,
     min_version,
     optional_import,
+    pytorch_after,
 )
 from monai.utils.enums import TransformBackends
 from monai.utils.type_conversion import convert_data_type, convert_to_cupy, convert_to_dst_type, convert_to_tensor
 
 measure, has_measure = optional_import("skimage.measure", "0.14.2", min_version)
 morphology, has_morphology = optional_import("skimage.morphology")
 ndimage, _ = optional_import("scipy.ndimage")
@@ -112,14 +116,15 @@
     "convert_pad_mode",
     "convert_to_contiguous",
     "get_unique_labels",
     "scale_affine",
     "attach_hook",
     "sync_meta_info",
     "reset_ops_id",
+    "resolves_modes",
 ]
 
 
 def rand_choice(prob: float = 0.5) -> bool:
     """
     Returns True if a randomly chosen number is less than or equal to `prob`, by default this is a 50/50 chance.
     """
@@ -1839,9 +1844,128 @@
     mask2 = (~mask1) & (tmod < w * 2 * torch.pi)
     y[mask2] = 1
     mask3 = (~mask1) & (~mask2)
     y[mask3] = -1
     return y
 
 
+def _to_numpy_resample_interp_mode(interp_mode):
+    ret = look_up_option(str(interp_mode), SplineMode, default=None)
+    if ret is not None:
+        return int(ret)
+    _mapping = {
+        InterpolateMode.NEAREST: SplineMode.ZERO,
+        InterpolateMode.NEAREST_EXACT: SplineMode.ZERO,
+        InterpolateMode.LINEAR: SplineMode.ONE,
+        InterpolateMode.BILINEAR: SplineMode.ONE,
+        InterpolateMode.TRILINEAR: SplineMode.ONE,
+        InterpolateMode.BICUBIC: SplineMode.THREE,
+        InterpolateMode.AREA: SplineMode.ZERO,
+    }
+    ret = look_up_option(str(interp_mode), _mapping, default=None)
+    if ret is not None:
+        return ret
+    return look_up_option(str(interp_mode), list(_mapping) + list(SplineMode))  # for better error msg
+
+
+def _to_torch_resample_interp_mode(interp_mode):
+    ret = look_up_option(str(interp_mode), InterpolateMode, default=None)
+    if ret is not None:
+        return ret
+    _mapping = {
+        SplineMode.ZERO: InterpolateMode.NEAREST_EXACT if pytorch_after(1, 11) else InterpolateMode.NEAREST,
+        SplineMode.ONE: InterpolateMode.LINEAR,
+        SplineMode.THREE: InterpolateMode.BICUBIC,
+    }
+    ret = look_up_option(str(interp_mode), _mapping, default=None)
+    if ret is not None:
+        return ret
+    return look_up_option(str(interp_mode), list(_mapping) + list(InterpolateMode))
+
+
+def _to_numpy_resample_padding_mode(m):
+    ret = look_up_option(str(m), NdimageMode, default=None)
+    if ret is not None:
+        return ret
+    _mapping = {
+        GridSamplePadMode.ZEROS: NdimageMode.CONSTANT,
+        GridSamplePadMode.BORDER: NdimageMode.NEAREST,
+        GridSamplePadMode.REFLECTION: NdimageMode.REFLECT,
+    }
+    ret = look_up_option(str(m), _mapping, default=None)
+    if ret is not None:
+        return ret
+    return look_up_option(str(m), list(_mapping) + list(NdimageMode))
+
+
+def _to_torch_resample_padding_mode(m):
+    ret = look_up_option(str(m), GridSamplePadMode, default=None)
+    if ret is not None:
+        return ret
+    _mapping = {
+        NdimageMode.CONSTANT: GridSamplePadMode.ZEROS,
+        NdimageMode.GRID_CONSTANT: GridSamplePadMode.ZEROS,
+        NdimageMode.NEAREST: GridSamplePadMode.BORDER,
+        NdimageMode.REFLECT: GridSamplePadMode.REFLECTION,
+        NdimageMode.WRAP: GridSamplePadMode.REFLECTION,
+        NdimageMode.GRID_WRAP: GridSamplePadMode.REFLECTION,
+        NdimageMode.GRID_MIRROR: GridSamplePadMode.REFLECTION,
+    }
+    ret = look_up_option(str(m), _mapping, default=None)
+    if ret is not None:
+        return ret
+    return look_up_option(str(m), list(_mapping) + list(GridSamplePadMode))
+
+
+@lru_cache(None)
+def resolves_modes(
+    interp_mode: str | None = "constant", padding_mode="zeros", backend=TransformBackends.TORCH, **kwargs
+):
+    """
+    Automatically adjust the resampling interpolation mode and padding mode,
+    so that they are compatible with the corresponding API of the `backend`.
+    Depending on the availability of the backends, when there's no exact
+    equivalent, a similar mode is returned.
+
+    Args:
+        interp_mode: interpolation mode.
+        padding_mdoe: padding mode.
+        backend: optional backend of `TransformBackends`. If None, the backend will be decided from `interp_mode`.
+        kwargs: additional keyword arguments. currently support ``torch_interpolate_spatial_nd``, to provide
+            additional information to determine ``linear``, ``bilinear`` and ``trilinear``;
+            ``use_compiled`` to use MONAI's precompiled backend (pytorch c++ extensions), default to ``False``.
+    """
+    _interp_mode, _padding_mode, _kwargs = None, None, (kwargs or {}).copy()
+    if backend is None:  # infer backend
+        backend = (
+            TransformBackends.NUMPY
+            if look_up_option(str(interp_mode), SplineMode, default=None) is not None
+            else TransformBackends.TORCH
+        )
+    if backend == TransformBackends.NUMPY:
+        _interp_mode = _to_numpy_resample_interp_mode(interp_mode)
+        _padding_mode = _to_numpy_resample_padding_mode(padding_mode)
+        return backend, _interp_mode, _padding_mode, _kwargs
+    _interp_mode = _to_torch_resample_interp_mode(interp_mode)
+    _padding_mode = _to_torch_resample_padding_mode(padding_mode)
+    if str(_interp_mode).endswith("linear"):
+        nd = _kwargs.pop("torch_interpolate_spatial_nd", 2)
+        if nd == 1:
+            _interp_mode = InterpolateMode.LINEAR
+        elif nd == 3:
+            _interp_mode = InterpolateMode.TRILINEAR
+        else:
+            _interp_mode = InterpolateMode.BILINEAR  # torch grid_sample bilinear is trilinear in 3D
+    if not _kwargs.pop("use_compiled", False):
+        return backend, _interp_mode, _padding_mode, _kwargs
+    _padding_mode = 1 if _padding_mode == "reflection" else _padding_mode
+    if _interp_mode == "bicubic":
+        _interp_mode = 3
+    elif str(_interp_mode).endswith("linear"):
+        _interp_mode = 1
+    else:
+        _interp_mode = GridSampleMode(_interp_mode)
+    return backend, _interp_mode, _padding_mode, _kwargs
+
+
 if __name__ == "__main__":
     print_transform_backends()
```

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/utils_create_transform_ims.py` & `monai-weekly-1.2.dev2318/monai/transforms/utils_create_transform_ims.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/transforms/utils_pytorch_numpy_unification.py` & `monai-weekly-1.2.dev2318/monai/transforms/utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/utils/__init__.py` & `monai-weekly-1.2.dev2318/monai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/utils/aliases.py` & `monai-weekly-1.2.dev2318/monai/utils/aliases.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/utils/decorators.py` & `monai-weekly-1.2.dev2318/monai/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/utils/deprecate_utils.py` & `monai-weekly-1.2.dev2318/monai/utils/deprecate_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/utils/dist.py` & `monai-weekly-1.2.dev2318/monai/utils/dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/utils/enums.py` & `monai-weekly-1.2.dev2318/monai/utils/enums.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/utils/jupyter_utils.py` & `monai-weekly-1.2.dev2318/monai/utils/jupyter_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/utils/misc.py` & `monai-weekly-1.2.dev2318/monai/utils/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     "save_obj",
     "label_union",
     "path_to_uri",
     "pprint_edges",
     "check_key_duplicates",
     "CheckKeyDuplicatesYamlLoader",
     "ConvertUnits",
+    "check_kwargs_exist_in_class_init",
 ]
 
 _seed = None
 _flag_deterministic = torch.backends.cudnn.deterministic
 _flag_cudnn_benchmark = torch.backends.cudnn.benchmark
 NP_MAX = np.iinfo(np.uint32).max
 MAX_SEED = NP_MAX + 1  # 2**32, the actual seed should be in [0, MAX_SEED - 1] for uint32
@@ -796,7 +797,27 @@
             return 1.0
         input_power = self._get_unit_power(self.input_unit)
         target_power = self._get_unit_power(self.target_unit)
         self.conversion_factor = 10 ** (input_power - target_power)
 
     def __call__(self, value: int | float) -> Any:
         return float(value) * self.conversion_factor
+
+
+def check_kwargs_exist_in_class_init(cls, kwargs):
+    """
+    Check if the all keys in kwargs exist in the __init__ method of the class.
+
+    Args:
+        cls: the class to check.
+        kwargs: kwargs to examine.
+
+    Returns:
+        a boolean inidicating if all keys exist.
+        a set of extra keys that are not used in the __init__.
+    """
+    init_signature = inspect.signature(cls.__init__)
+    init_params = set(init_signature.parameters) - {"self"}  # Exclude 'self' from the parameter list
+    input_kwargs = set(kwargs)
+    extra_kwargs = input_kwargs - init_params
+
+    return extra_kwargs == set(), extra_kwargs
```

### Comparing `monai-weekly-1.2.dev2317/monai/utils/module.py` & `monai-weekly-1.2.dev2318/monai/utils/module.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/utils/nvtx.py` & `monai-weekly-1.2.dev2318/monai/utils/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/utils/profiling.py` & `monai-weekly-1.2.dev2318/monai/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/utils/state_cacher.py` & `monai-weekly-1.2.dev2318/monai/utils/state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/utils/type_conversion.py` & `monai-weekly-1.2.dev2318/monai/utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/visualize/__init__.py` & `monai-weekly-1.2.dev2318/monai/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/visualize/class_activation_maps.py` & `monai-weekly-1.2.dev2318/monai/visualize/class_activation_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/visualize/gradient_based.py` & `monai-weekly-1.2.dev2318/monai/visualize/gradient_based.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/visualize/img2tensorboard.py` & `monai-weekly-1.2.dev2318/monai/visualize/img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/visualize/occlusion_sensitivity.py` & `monai-weekly-1.2.dev2318/monai/visualize/occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/visualize/utils.py` & `monai-weekly-1.2.dev2318/monai/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai/visualize/visualizer.py` & `monai-weekly-1.2.dev2318/monai/visualize/visualizer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/monai_weekly.egg-info/PKG-INFO` & `monai-weekly-1.2.dev2318/monai_weekly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.2.dev2317
+Version: 1.2.dev2318
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
```

### Comparing `monai-weekly-1.2.dev2317/monai_weekly.egg-info/SOURCES.txt` & `monai-weekly-1.2.dev2318/monai_weekly.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -398,14 +398,15 @@
 tests/test_as_channel_last.py
 tests/test_as_channel_lastd.py
 tests/test_as_discrete.py
 tests/test_as_discreted.py
 tests/test_atss_box_matcher.py
 tests/test_attentionunet.py
 tests/test_auto3dseg.py
+tests/test_auto3dseg_bundlegen.py
 tests/test_auto3dseg_ensemble.py
 tests/test_auto3dseg_hpo.py
 tests/test_autoencoder.py
 tests/test_avg_merger.py
 tests/test_basic_unet.py
 tests/test_basic_unetplusplus.py
 tests/test_bending_energy.py
```

### Comparing `monai-weekly-1.2.dev2317/monai_weekly.egg-info/requires.txt` & `monai-weekly-1.2.dev2318/monai_weekly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/pyproject.toml` & `monai-weekly-1.2.dev2318/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/setup.cfg` & `monai-weekly-1.2.dev2318/setup.cfg`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/setup.py` & `monai-weekly-1.2.dev2318/setup.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_acn_block.py` & `monai-weekly-1.2.dev2318/tests/test_acn_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_activations.py` & `monai-weekly-1.2.dev2318/tests/test_activations.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_activationsd.py` & `monai-weekly-1.2.dev2318/tests/test_activationsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_adaptors.py` & `monai-weekly-1.2.dev2318/tests/test_adaptors.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_add_channeld.py` & `monai-weekly-1.2.dev2318/tests/test_add_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_add_coordinate_channels.py` & `monai-weekly-1.2.dev2318/tests/test_add_coordinate_channels.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_add_coordinate_channelsd.py` & `monai-weekly-1.2.dev2318/tests/test_add_coordinate_channelsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_add_extreme_points_channel.py` & `monai-weekly-1.2.dev2318/tests/test_add_extreme_points_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_add_extreme_points_channeld.py` & `monai-weekly-1.2.dev2318/tests/test_add_extreme_points_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_adjust_contrast.py` & `monai-weekly-1.2.dev2318/tests/test_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_adjust_contrastd.py` & `monai-weekly-1.2.dev2318/tests/test_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_adn.py` & `monai-weekly-1.2.dev2318/tests/test_adn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_affine.py` & `monai-weekly-1.2.dev2318/tests/test_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_affine_grid.py` & `monai-weekly-1.2.dev2318/tests/test_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_affine_transform.py` & `monai-weekly-1.2.dev2318/tests/test_affine_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_affined.py` & `monai-weekly-1.2.dev2318/tests/test_affined.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_ahnet.py` & `monai-weekly-1.2.dev2318/tests/test_ahnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_alias.py` & `monai-weekly-1.2.dev2318/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_anchor_box.py` & `monai-weekly-1.2.dev2318/tests/test_anchor_box.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_apply.py` & `monai-weekly-1.2.dev2318/tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_apply_filter.py` & `monai-weekly-1.2.dev2318/tests/test_apply_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_arraydataset.py` & `monai-weekly-1.2.dev2318/tests/test_arraydataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_as_channel_first.py` & `monai-weekly-1.2.dev2318/tests/test_as_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_as_channel_firstd.py` & `monai-weekly-1.2.dev2318/tests/test_as_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_as_channel_last.py` & `monai-weekly-1.2.dev2318/tests/test_as_channel_last.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_as_channel_lastd.py` & `monai-weekly-1.2.dev2318/tests/test_as_channel_lastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_as_discrete.py` & `monai-weekly-1.2.dev2318/tests/test_as_discrete.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_as_discreted.py` & `monai-weekly-1.2.dev2318/tests/test_as_discreted.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_atss_box_matcher.py` & `monai-weekly-1.2.dev2318/tests/test_atss_box_matcher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_attentionunet.py` & `monai-weekly-1.2.dev2318/tests/test_attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_auto3dseg.py` & `monai-weekly-1.2.dev2318/tests/test_auto3dseg.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_auto3dseg_ensemble.py` & `monai-weekly-1.2.dev2318/tests/test_auto3dseg_ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,18 +176,18 @@
         self.assertTrue(runner.ensemble_method.n_fold == 3)  # type: ignore
 
         runner.set_ensemble_method(ensemble_method_name="AlgoEnsembleBestN", n_best=3)
         self.assertIsInstance(runner.ensemble_method, AlgoEnsembleBestN)
         self.assertTrue(runner.ensemble_method.n_best == 3)
 
         save_output = os.path.join(self.test_dir.name, "workdir")
-        runner.set_image_save_transform(
+        save_image = runner._pop_kwargs_to_get_image_save_transform(
             output_dir=save_output, output_postfix="test_ensemble", output_dtype=float, resample=True
         )
-        self.assertIsInstance(ConfigParser(runner.save_image).get_parsed_content(), SaveImage)
+        self.assertIsInstance(ConfigParser(save_image).get_parsed_content(), SaveImage)
 
     def tearDown(self) -> None:
         set_determinism(None)
         self.test_dir.cleanup()
 
 
 if __name__ == "__main__":
```

### Comparing `monai-weekly-1.2.dev2317/tests/test_auto3dseg_hpo.py` & `monai-weekly-1.2.dev2318/tests/test_auto3dseg_hpo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_autoencoder.py` & `monai-weekly-1.2.dev2318/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_avg_merger.py` & `monai-weekly-1.2.dev2318/tests/test_avg_merger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_basic_unet.py` & `monai-weekly-1.2.dev2318/tests/test_basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_basic_unetplusplus.py` & `monai-weekly-1.2.dev2318/tests/test_basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_bending_energy.py` & `monai-weekly-1.2.dev2318/tests/test_bending_energy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_bilateral_approx_cpu.py` & `monai-weekly-1.2.dev2318/tests/test_bilateral_approx_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_bilateral_approx_cuda.py` & `monai-weekly-1.2.dev2318/tests/test_bilateral_approx_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_bilateral_precise.py` & `monai-weekly-1.2.dev2318/tests/test_bilateral_precise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_blend_images.py` & `monai-weekly-1.2.dev2318/tests/test_blend_images.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_border_pad.py` & `monai-weekly-1.2.dev2318/tests/test_border_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_border_padd.py` & `monai-weekly-1.2.dev2318/tests/test_border_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_bounding_rect.py` & `monai-weekly-1.2.dev2318/tests/test_bounding_rect.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_bounding_rectd.py` & `monai-weekly-1.2.dev2318/tests/test_bounding_rectd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_box_coder.py` & `monai-weekly-1.2.dev2318/tests/test_box_coder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_box_transform.py` & `monai-weekly-1.2.dev2318/tests/test_box_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_box_utils.py` & `monai-weekly-1.2.dev2318/tests/test_box_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_bundle_ckpt_export.py` & `monai-weekly-1.2.dev2318/tests/test_bundle_ckpt_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_bundle_download.py` & `monai-weekly-1.2.dev2318/tests/test_bundle_download.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_bundle_get_data.py` & `monai-weekly-1.2.dev2318/tests/test_bundle_get_data.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_bundle_init_bundle.py` & `monai-weekly-1.2.dev2318/tests/test_bundle_init_bundle.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_bundle_onnx_export.py` & `monai-weekly-1.2.dev2318/tests/test_bundle_onnx_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_bundle_trt_export.py` & `monai-weekly-1.2.dev2318/tests/test_bundle_trt_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_bundle_utils.py` & `monai-weekly-1.2.dev2318/tests/test_bundle_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_bundle_verify_metadata.py` & `monai-weekly-1.2.dev2318/tests/test_bundle_verify_metadata.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_bundle_verify_net.py` & `monai-weekly-1.2.dev2318/tests/test_bundle_verify_net.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_bundle_workflow.py` & `monai-weekly-1.2.dev2318/tests/test_bundle_workflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_cachedataset.py` & `monai-weekly-1.2.dev2318/tests/test_cachedataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_cachedataset_parallel.py` & `monai-weekly-1.2.dev2318/tests/test_cachedataset_parallel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_cachedataset_persistent_workers.py` & `monai-weekly-1.2.dev2318/tests/test_cachedataset_persistent_workers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_cachentransdataset.py` & `monai-weekly-1.2.dev2318/tests/test_cachentransdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_call_dist.py` & `monai-weekly-1.2.dev2318/tests/test_call_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_cast_to_type.py` & `monai-weekly-1.2.dev2318/tests/test_cast_to_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_cast_to_typed.py` & `monai-weekly-1.2.dev2318/tests/test_cast_to_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_center_scale_crop.py` & `monai-weekly-1.2.dev2318/tests/test_center_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_center_scale_cropd.py` & `monai-weekly-1.2.dev2318/tests/test_center_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_center_spatial_crop.py` & `monai-weekly-1.2.dev2318/tests/test_center_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_center_spatial_cropd.py` & `monai-weekly-1.2.dev2318/tests/test_center_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_channel_pad.py` & `monai-weekly-1.2.dev2318/tests/test_channel_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_check_hash.py` & `monai-weekly-1.2.dev2318/tests/test_check_hash.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_check_missing_files.py` & `monai-weekly-1.2.dev2318/tests/test_check_missing_files.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_classes_to_indices.py` & `monai-weekly-1.2.dev2318/tests/test_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_classes_to_indicesd.py` & `monai-weekly-1.2.dev2318/tests/test_classes_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_complex_utils.py` & `monai-weekly-1.2.dev2318/tests/test_complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_component_locator.py` & `monai-weekly-1.2.dev2318/tests/test_component_locator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_compose.py` & `monai-weekly-1.2.dev2318/tests/test_compose.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,9 +334,20 @@
             if isinstance(actual, dict):
                 for k in actual.keys():
                     self.assertTrue(expected[k], actual[k])
             else:
                 self.assertTrue(expected, actual)
 
 
+TEST_LAZY_COMPOSE_PIPELINE_FIX_CASES = [[(Flip(0), Flip(1), Rotate90(1), Zoom(0.8), NormalizeIntensity())]]
+
+
+class TestLazyComposePipelineFixes(unittest.TestCase):
+    @parameterized.expand(TEST_LAZY_COMPOSE_PIPELINE_FIX_CASES)
+    def test_lazy_compose_pipeline_fixes(self, pipeline):
+        data = torch.unsqueeze(torch.tensor(np.arange(12 * 16).reshape(12, 16)), dim=0)
+        c = Compose(deepcopy(pipeline), lazy_evaluation=True)
+        _ = c(data)
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2317/tests/test_compose_get_number_conversions.py` & `monai-weekly-1.2.dev2318/tests/test_compose_get_number_conversions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_compute_confusion_matrix.py` & `monai-weekly-1.2.dev2318/tests/test_compute_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_compute_f_beta.py` & `monai-weekly-1.2.dev2318/tests/test_compute_f_beta.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_compute_froc.py` & `monai-weekly-1.2.dev2318/tests/test_compute_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_compute_generalized_dice.py` & `monai-weekly-1.2.dev2318/tests/test_compute_generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_compute_ho_ver_maps.py` & `monai-weekly-1.2.dev2318/tests/test_compute_ho_ver_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_compute_ho_ver_maps_d.py` & `monai-weekly-1.2.dev2318/tests/test_compute_ho_ver_maps_d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_compute_meandice.py` & `monai-weekly-1.2.dev2318/tests/test_compute_meandice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_compute_meaniou.py` & `monai-weekly-1.2.dev2318/tests/test_compute_meaniou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_compute_panoptic_quality.py` & `monai-weekly-1.2.dev2318/tests/test_compute_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_compute_regression_metrics.py` & `monai-weekly-1.2.dev2318/tests/test_compute_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_compute_roc_auc.py` & `monai-weekly-1.2.dev2318/tests/test_compute_roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_compute_variance.py` & `monai-weekly-1.2.dev2318/tests/test_compute_variance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_concat_itemsd.py` & `monai-weekly-1.2.dev2318/tests/test_concat_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_config_item.py` & `monai-weekly-1.2.dev2318/tests/test_config_item.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_config_parser.py` & `monai-weekly-1.2.dev2318/tests/test_config_parser.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_contrastive_loss.py` & `monai-weekly-1.2.dev2318/tests/test_contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_convert_data_type.py` & `monai-weekly-1.2.dev2318/tests/test_convert_data_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_convert_to_multi_channel.py` & `monai-weekly-1.2.dev2318/tests/test_convert_to_multi_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_convert_to_multi_channeld.py` & `monai-weekly-1.2.dev2318/tests/test_convert_to_multi_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_convert_to_onnx.py` & `monai-weekly-1.2.dev2318/tests/test_convert_to_onnx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_convert_to_torchscript.py` & `monai-weekly-1.2.dev2318/tests/test_convert_to_torchscript.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_convert_to_trt.py` & `monai-weekly-1.2.dev2318/tests/test_convert_to_trt.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_convolutions.py` & `monai-weekly-1.2.dev2318/tests/test_convolutions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_copy_itemsd.py` & `monai-weekly-1.2.dev2318/tests/test_copy_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_copy_model_state.py` & `monai-weekly-1.2.dev2318/tests/test_copy_model_state.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_correct_crop_centers.py` & `monai-weekly-1.2.dev2318/tests/test_correct_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_create_cross_validation_datalist.py` & `monai-weekly-1.2.dev2318/tests/test_create_cross_validation_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_create_grid_and_affine.py` & `monai-weekly-1.2.dev2318/tests/test_create_grid_and_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_crf_cpu.py` & `monai-weekly-1.2.dev2318/tests/test_crf_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_crf_cuda.py` & `monai-weekly-1.2.dev2318/tests/test_crf_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_crop_foreground.py` & `monai-weekly-1.2.dev2318/tests/test_crop_foreground.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_crop_foregroundd.py` & `monai-weekly-1.2.dev2318/tests/test_crop_foregroundd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_cross_validation.py` & `monai-weekly-1.2.dev2318/tests/test_cross_validation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_csv_dataset.py` & `monai-weekly-1.2.dev2318/tests/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_csv_iterable_dataset.py` & `monai-weekly-1.2.dev2318/tests/test_csv_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_csv_saver.py` & `monai-weekly-1.2.dev2318/tests/test_csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_cucim_dict_transform.py` & `monai-weekly-1.2.dev2318/tests/test_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_cucim_transform.py` & `monai-weekly-1.2.dev2318/tests/test_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_cumulative.py` & `monai-weekly-1.2.dev2318/tests/test_cumulative.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_cumulative_average.py` & `monai-weekly-1.2.dev2318/tests/test_cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_cumulative_average_dist.py` & `monai-weekly-1.2.dev2318/tests/test_cumulative_average_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_cv2_dist.py` & `monai-weekly-1.2.dev2318/tests/test_cv2_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_data_stats.py` & `monai-weekly-1.2.dev2318/tests/test_data_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_data_statsd.py` & `monai-weekly-1.2.dev2318/tests/test_data_statsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_dataloader.py` & `monai-weekly-1.2.dev2318/tests/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_dataset.py` & `monai-weekly-1.2.dev2318/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_dataset_func.py` & `monai-weekly-1.2.dev2318/tests/test_dataset_func.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_dataset_summary.py` & `monai-weekly-1.2.dev2318/tests/test_dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_decathlondataset.py` & `monai-weekly-1.2.dev2318/tests/test_decathlondataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_decollate.py` & `monai-weekly-1.2.dev2318/tests/test_decollate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_deepedit_interaction.py` & `monai-weekly-1.2.dev2318/tests/test_deepedit_interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_deepedit_transforms.py` & `monai-weekly-1.2.dev2318/tests/test_deepedit_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_deepgrow_dataset.py` & `monai-weekly-1.2.dev2318/tests/test_deepgrow_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_deepgrow_interaction.py` & `monai-weekly-1.2.dev2318/tests/test_deepgrow_interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_deepgrow_transforms.py` & `monai-weekly-1.2.dev2318/tests/test_deepgrow_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_delete_itemsd.py` & `monai-weekly-1.2.dev2318/tests/test_delete_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_denseblock.py` & `monai-weekly-1.2.dev2318/tests/test_denseblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_densenet.py` & `monai-weekly-1.2.dev2318/tests/test_densenet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_deprecated.py` & `monai-weekly-1.2.dev2318/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_detect_envelope.py` & `monai-weekly-1.2.dev2318/tests/test_detect_envelope.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_detection_coco_metrics.py` & `monai-weekly-1.2.dev2318/tests/test_detection_coco_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_detector_boxselector.py` & `monai-weekly-1.2.dev2318/tests/test_detector_boxselector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_detector_utils.py` & `monai-weekly-1.2.dev2318/tests/test_detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_dev_collate.py` & `monai-weekly-1.2.dev2318/tests/test_dev_collate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_dice_ce_loss.py` & `monai-weekly-1.2.dev2318/tests/test_dice_ce_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_dice_focal_loss.py` & `monai-weekly-1.2.dev2318/tests/test_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_dice_loss.py` & `monai-weekly-1.2.dev2318/tests/test_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_dints_cell.py` & `monai-weekly-1.2.dev2318/tests/test_dints_cell.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_dints_mixop.py` & `monai-weekly-1.2.dev2318/tests/test_dints_mixop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_dints_network.py` & `monai-weekly-1.2.dev2318/tests/test_dints_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_discriminator.py` & `monai-weekly-1.2.dev2318/tests/test_discriminator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_divisible_pad.py` & `monai-weekly-1.2.dev2318/tests/test_divisible_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_divisible_padd.py` & `monai-weekly-1.2.dev2318/tests/test_divisible_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_download_and_extract.py` & `monai-weekly-1.2.dev2318/tests/test_download_and_extract.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_downsample_block.py` & `monai-weekly-1.2.dev2318/tests/test_downsample_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_drop_path.py` & `monai-weekly-1.2.dev2318/tests/test_drop_path.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_ds_loss.py` & `monai-weekly-1.2.dev2318/tests/test_ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_dvf2ddf.py` & `monai-weekly-1.2.dev2318/tests/test_dvf2ddf.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_dynunet.py` & `monai-weekly-1.2.dev2318/tests/test_dynunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_dynunet_block.py` & `monai-weekly-1.2.dev2318/tests/test_dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_efficientnet.py` & `monai-weekly-1.2.dev2318/tests/test_efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_ensemble_evaluator.py` & `monai-weekly-1.2.dev2318/tests/test_ensemble_evaluator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_ensure_channel_first.py` & `monai-weekly-1.2.dev2318/tests/test_ensure_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_ensure_channel_firstd.py` & `monai-weekly-1.2.dev2318/tests/test_ensure_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_ensure_tuple.py` & `monai-weekly-1.2.dev2318/tests/test_ensure_tuple.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_ensure_type.py` & `monai-weekly-1.2.dev2318/tests/test_ensure_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_ensure_typed.py` & `monai-weekly-1.2.dev2318/tests/test_ensure_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_enum_bound_interp.py` & `monai-weekly-1.2.dev2318/tests/test_enum_bound_interp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_eval_mode.py` & `monai-weekly-1.2.dev2318/tests/test_eval_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_evenly_divisible_all_gather_dist.py` & `monai-weekly-1.2.dev2318/tests/test_evenly_divisible_all_gather_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_factorized_increase.py` & `monai-weekly-1.2.dev2318/tests/test_factorized_increase.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_factorized_reduce.py` & `monai-weekly-1.2.dev2318/tests/test_factorized_reduce.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_fastmri_reader.py` & `monai-weekly-1.2.dev2318/tests/test_fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_fft_utils.py` & `monai-weekly-1.2.dev2318/tests/test_fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_fg_bg_to_indices.py` & `monai-weekly-1.2.dev2318/tests/test_fg_bg_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_fg_bg_to_indicesd.py` & `monai-weekly-1.2.dev2318/tests/test_fg_bg_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_file_basename.py` & `monai-weekly-1.2.dev2318/tests/test_file_basename.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_fill_holes.py` & `monai-weekly-1.2.dev2318/tests/test_fill_holes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_fill_holesd.py` & `monai-weekly-1.2.dev2318/tests/test_fill_holesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_fl_exchange_object.py` & `monai-weekly-1.2.dev2318/tests/test_fl_exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_fl_monai_algo.py` & `monai-weekly-1.2.dev2318/tests/test_fl_monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_fl_monai_algo_dist.py` & `monai-weekly-1.2.dev2318/tests/test_fl_monai_algo_dist.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,18 @@
     def test_train(self):
         train_configs = [pathjoin(_data_dir, "config_fl_train.json"), pathjoin(_data_dir, "multi_gpu_train.json")]
         eval_configs = [
             pathjoin(_data_dir, "config_fl_train.json"),
             pathjoin(_data_dir, "config_fl_evaluate.json"),
             pathjoin(_data_dir, "multi_gpu_evaluate.json"),
         ]
+        train_workflow = ConfigWorkflow(config_file=train_configs, workflow="train", logging_file=_logging_file)
+        # simulate the case that this application has specific requirements for a bundle workflow
+        train_workflow.add_property(name="loader", required=True, config_id="train#training_transforms#0", desc="NA")
+
         # initialize algo
         algo = MonaiAlgo(
             bundle_root=_data_dir,
             train_workflow=ConfigWorkflow(config_file=train_configs, workflow="train", logging_file=_logging_file),
             eval_workflow=ConfigWorkflow(config_file=eval_configs, workflow="train", logging_file=_logging_file),
             config_filters_filename=pathjoin(_root_dir, "testing_data", "config_fl_filters.json"),
         )
```

### Comparing `monai-weekly-1.2.dev2317/tests/test_fl_monai_algo_stats.py` & `monai-weekly-1.2.dev2318/tests/test_fl_monai_algo_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_flatten_sub_keysd.py` & `monai-weekly-1.2.dev2318/tests/test_flatten_sub_keysd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_flexible_unet.py` & `monai-weekly-1.2.dev2318/tests/test_flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_flip.py` & `monai-weekly-1.2.dev2318/tests/test_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_flipd.py` & `monai-weekly-1.2.dev2318/tests/test_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_focal_loss.py` & `monai-weekly-1.2.dev2318/tests/test_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_folder_layout.py` & `monai-weekly-1.2.dev2318/tests/test_folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_foreground_mask.py` & `monai-weekly-1.2.dev2318/tests/test_foreground_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_foreground_maskd.py` & `monai-weekly-1.2.dev2318/tests/test_foreground_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_fourier.py` & `monai-weekly-1.2.dev2318/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_fpn_block.py` & `monai-weekly-1.2.dev2318/tests/test_fpn_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_from_engine_hovernet.py` & `monai-weekly-1.2.dev2318/tests/test_from_engine_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_fullyconnectednet.py` & `monai-weekly-1.2.dev2318/tests/test_fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_gaussian.py` & `monai-weekly-1.2.dev2318/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_gaussian_filter.py` & `monai-weekly-1.2.dev2318/tests/test_gaussian_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_gaussian_sharpen.py` & `monai-weekly-1.2.dev2318/tests/test_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_gaussian_sharpend.py` & `monai-weekly-1.2.dev2318/tests/test_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_gaussian_smooth.py` & `monai-weekly-1.2.dev2318/tests/test_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_gaussian_smoothd.py` & `monai-weekly-1.2.dev2318/tests/test_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generalized_dice_focal_loss.py` & `monai-weekly-1.2.dev2318/tests/test_generalized_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generalized_dice_loss.py` & `monai-weekly-1.2.dev2318/tests/test_generalized_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generalized_wasserstein_dice_loss.py` & `monai-weekly-1.2.dev2318/tests/test_generalized_wasserstein_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_distance_map.py` & `monai-weekly-1.2.dev2318/tests/test_generate_distance_map.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_distance_mapd.py` & `monai-weekly-1.2.dev2318/tests/test_generate_distance_mapd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_instance_border.py` & `monai-weekly-1.2.dev2318/tests/test_generate_instance_border.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_instance_borderd.py` & `monai-weekly-1.2.dev2318/tests/test_generate_instance_borderd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_instance_centroid.py` & `monai-weekly-1.2.dev2318/tests/test_generate_instance_centroid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_instance_centroidd.py` & `monai-weekly-1.2.dev2318/tests/test_generate_instance_centroidd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_instance_contour.py` & `monai-weekly-1.2.dev2318/tests/test_generate_instance_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_instance_contourd.py` & `monai-weekly-1.2.dev2318/tests/test_generate_instance_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_instance_type.py` & `monai-weekly-1.2.dev2318/tests/test_generate_instance_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_instance_typed.py` & `monai-weekly-1.2.dev2318/tests/test_generate_instance_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_label_classes_crop_centers.py` & `monai-weekly-1.2.dev2318/tests/test_generate_label_classes_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_param_groups.py` & `monai-weekly-1.2.dev2318/tests/test_generate_param_groups.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_pos_neg_label_crop_centers.py` & `monai-weekly-1.2.dev2318/tests/test_generate_pos_neg_label_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_spatial_bounding_box.py` & `monai-weekly-1.2.dev2318/tests/test_generate_spatial_bounding_box.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_succinct_contour.py` & `monai-weekly-1.2.dev2318/tests/test_generate_succinct_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_succinct_contourd.py` & `monai-weekly-1.2.dev2318/tests/test_generate_succinct_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_watershed_markers.py` & `monai-weekly-1.2.dev2318/tests/test_generate_watershed_markers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_watershed_markersd.py` & `monai-weekly-1.2.dev2318/tests/test_generate_watershed_markersd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_watershed_mask.py` & `monai-weekly-1.2.dev2318/tests/test_generate_watershed_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generate_watershed_maskd.py` & `monai-weekly-1.2.dev2318/tests/test_generate_watershed_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_generator.py` & `monai-weekly-1.2.dev2318/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_get_equivalent_dtype.py` & `monai-weekly-1.2.dev2318/tests/test_get_equivalent_dtype.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_get_extreme_points.py` & `monai-weekly-1.2.dev2318/tests/test_get_extreme_points.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_get_layers.py` & `monai-weekly-1.2.dev2318/tests/test_get_layers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_get_package_version.py` & `monai-weekly-1.2.dev2318/tests/test_get_package_version.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_get_unique_labels.py` & `monai-weekly-1.2.dev2318/tests/test_get_unique_labels.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_gibbs_noise.py` & `monai-weekly-1.2.dev2318/tests/test_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_gibbs_noised.py` & `monai-weekly-1.2.dev2318/tests/test_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_giou_loss.py` & `monai-weekly-1.2.dev2318/tests/test_giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_global_mutual_information_loss.py` & `monai-weekly-1.2.dev2318/tests/test_global_mutual_information_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_globalnet.py` & `monai-weekly-1.2.dev2318/tests/test_globalnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_gmm.py` & `monai-weekly-1.2.dev2318/tests/test_gmm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_grid_dataset.py` & `monai-weekly-1.2.dev2318/tests/test_grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_grid_distortion.py` & `monai-weekly-1.2.dev2318/tests/test_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_grid_distortiond.py` & `monai-weekly-1.2.dev2318/tests/test_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_grid_patch.py` & `monai-weekly-1.2.dev2318/tests/test_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_grid_patchd.py` & `monai-weekly-1.2.dev2318/tests/test_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_grid_pull.py` & `monai-weekly-1.2.dev2318/tests/test_grid_pull.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_grid_split.py` & `monai-weekly-1.2.dev2318/tests/test_grid_split.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_grid_splitd.py` & `monai-weekly-1.2.dev2318/tests/test_grid_splitd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_checkpoint_loader.py` & `monai-weekly-1.2.dev2318/tests/test_handler_checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_checkpoint_saver.py` & `monai-weekly-1.2.dev2318/tests/test_handler_checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_classification_saver.py` & `monai-weekly-1.2.dev2318/tests/test_handler_classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_classification_saver_dist.py` & `monai-weekly-1.2.dev2318/tests/test_handler_classification_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_clearml_image.py` & `monai-weekly-1.2.dev2318/tests/test_handler_clearml_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_clearml_stats.py` & `monai-weekly-1.2.dev2318/tests/test_handler_clearml_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_confusion_matrix.py` & `monai-weekly-1.2.dev2318/tests/test_handler_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_confusion_matrix_dist.py` & `monai-weekly-1.2.dev2318/tests/test_handler_confusion_matrix_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_decollate_batch.py` & `monai-weekly-1.2.dev2318/tests/test_handler_decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_early_stop.py` & `monai-weekly-1.2.dev2318/tests/test_handler_early_stop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_garbage_collector.py` & `monai-weekly-1.2.dev2318/tests/test_handler_garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_hausdorff_distance.py` & `monai-weekly-1.2.dev2318/tests/test_handler_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_logfile.py` & `monai-weekly-1.2.dev2318/tests/test_handler_logfile.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_lr_scheduler.py` & `monai-weekly-1.2.dev2318/tests/test_handler_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_mean_dice.py` & `monai-weekly-1.2.dev2318/tests/test_handler_mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_mean_iou.py` & `monai-weekly-1.2.dev2318/tests/test_handler_mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_metric_logger.py` & `monai-weekly-1.2.dev2318/tests/test_handler_metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_metrics_reloaded.py` & `monai-weekly-1.2.dev2318/tests/test_handler_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_metrics_saver.py` & `monai-weekly-1.2.dev2318/tests/test_handler_metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_metrics_saver_dist.py` & `monai-weekly-1.2.dev2318/tests/test_handler_metrics_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_mlflow.py` & `monai-weekly-1.2.dev2318/tests/test_handler_mlflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,14 +64,47 @@
         self.tmpdir_list = []
 
     def tearDown(self):
         for tmpdir in self.tmpdir_list:
             if tmpdir and os.path.exists(tmpdir):
                 shutil.rmtree(tmpdir)
 
+    def test_multi_run(self):
+        with tempfile.TemporaryDirectory() as tempdir:
+            # set up the train function for engine
+            def _train_func(engine, batch):
+                return [batch + 1.0]
+
+            # create and run an engine several times to get several runs
+            create_engine_times = 3
+            for _ in range(create_engine_times):
+                engine = Engine(_train_func)
+
+                @engine.on(Events.EPOCH_COMPLETED)
+                def _update_metric(engine):
+                    current_metric = engine.state.metrics.get("acc", 0.1)
+                    engine.state.metrics["acc"] = current_metric + 0.1
+                    engine.state.test = current_metric
+
+                # set up testing handler
+                test_path = os.path.join(tempdir, "mlflow_test")
+                handler = MLFlowHandler(
+                    iteration_log=False,
+                    epoch_log=True,
+                    tracking_uri=path_to_uri(test_path),
+                    state_attributes=["test"],
+                    close_on_complete=True,
+                )
+                handler.attach(engine)
+                engine.run(range(3), max_epochs=2)
+                run_cnt = len(handler.client.search_runs(handler.experiment.experiment_id))
+                handler.close()
+            # the run count should equal to the times of creating engine
+            self.assertEqual(create_engine_times, run_cnt)
+
     def test_metrics_track(self):
         experiment_param = {"backbone": "efficientnet_b0"}
         with tempfile.TemporaryDirectory() as tempdir:
             # set up engine
             def _train_func(engine, batch):
                 return [batch + 1.0]
```

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_nvtx.py` & `monai-weekly-1.2.dev2318/tests/test_handler_nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_panoptic_quality.py` & `monai-weekly-1.2.dev2318/tests/test_handler_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_parameter_scheduler.py` & `monai-weekly-1.2.dev2318/tests/test_handler_parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_post_processing.py` & `monai-weekly-1.2.dev2318/tests/test_handler_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_prob_map_producer.py` & `monai-weekly-1.2.dev2318/tests/test_handler_prob_map_producer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_regression_metrics.py` & `monai-weekly-1.2.dev2318/tests/test_handler_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_regression_metrics_dist.py` & `monai-weekly-1.2.dev2318/tests/test_handler_regression_metrics_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_rocauc.py` & `monai-weekly-1.2.dev2318/tests/test_handler_rocauc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_rocauc_dist.py` & `monai-weekly-1.2.dev2318/tests/test_handler_rocauc_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_smartcache.py` & `monai-weekly-1.2.dev2318/tests/test_handler_smartcache.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_stats.py` & `monai-weekly-1.2.dev2318/tests/test_handler_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_surface_distance.py` & `monai-weekly-1.2.dev2318/tests/test_handler_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_tb_image.py` & `monai-weekly-1.2.dev2318/tests/test_handler_tb_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_tb_stats.py` & `monai-weekly-1.2.dev2318/tests/test_handler_tb_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_handler_validation.py` & `monai-weekly-1.2.dev2318/tests/test_handler_validation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_hardnegsampler.py` & `monai-weekly-1.2.dev2318/tests/test_hardnegsampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_hashing.py` & `monai-weekly-1.2.dev2318/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_hausdorff_distance.py` & `monai-weekly-1.2.dev2318/tests/test_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_header_correct.py` & `monai-weekly-1.2.dev2318/tests/test_header_correct.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_highresnet.py` & `monai-weekly-1.2.dev2318/tests/test_highresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_hilbert_transform.py` & `monai-weekly-1.2.dev2318/tests/test_hilbert_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_histogram_normalize.py` & `monai-weekly-1.2.dev2318/tests/test_histogram_normalize.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_histogram_normalized.py` & `monai-weekly-1.2.dev2318/tests/test_histogram_normalized.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_hovernet.py` & `monai-weekly-1.2.dev2318/tests/test_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_hovernet_instance_map_post_processing.py` & `monai-weekly-1.2.dev2318/tests/test_hovernet_instance_map_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_hovernet_instance_map_post_processingd.py` & `monai-weekly-1.2.dev2318/tests/test_hovernet_instance_map_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_hovernet_loss.py` & `monai-weekly-1.2.dev2318/tests/test_hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_hovernet_nuclear_type_post_processing.py` & `monai-weekly-1.2.dev2318/tests/test_hovernet_nuclear_type_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_hovernet_nuclear_type_post_processingd.py` & `monai-weekly-1.2.dev2318/tests/test_hovernet_nuclear_type_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_identity.py` & `monai-weekly-1.2.dev2318/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_identityd.py` & `monai-weekly-1.2.dev2318/tests/test_identityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_image_dataset.py` & `monai-weekly-1.2.dev2318/tests/test_image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_image_filter.py` & `monai-weekly-1.2.dev2318/tests/test_image_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_image_rw.py` & `monai-weekly-1.2.dev2318/tests/test_image_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_img2tensorboard.py` & `monai-weekly-1.2.dev2318/tests/test_img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_init_reader.py` & `monai-weekly-1.2.dev2318/tests/test_init_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_integration_autorunner.py` & `monai-weekly-1.2.dev2318/tests/test_integration_autorunner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_integration_bundle_run.py` & `monai-weekly-1.2.dev2318/tests/test_integration_bundle_run.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_integration_classification_2d.py` & `monai-weekly-1.2.dev2318/tests/test_integration_classification_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_integration_determinism.py` & `monai-weekly-1.2.dev2318/tests/test_integration_determinism.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_integration_fast_train.py` & `monai-weekly-1.2.dev2318/tests/test_integration_fast_train.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_integration_gpu_customization.py` & `monai-weekly-1.2.dev2318/tests/test_integration_gpu_customization.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_integration_lazy_samples.py` & `monai-weekly-1.2.dev2318/tests/test_integration_lazy_samples.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_integration_nnunetv2_runner.py` & `monai-weekly-1.2.dev2318/tests/test_integration_nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_integration_segmentation_3d.py` & `monai-weekly-1.2.dev2318/tests/test_integration_segmentation_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_integration_sliding_window.py` & `monai-weekly-1.2.dev2318/tests/test_integration_sliding_window.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_integration_stn.py` & `monai-weekly-1.2.dev2318/tests/test_integration_stn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_integration_unet_2d.py` & `monai-weekly-1.2.dev2318/tests/test_integration_unet_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_integration_workers.py` & `monai-weekly-1.2.dev2318/tests/test_integration_workers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_integration_workflows.py` & `monai-weekly-1.2.dev2318/tests/test_integration_workflows.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_integration_workflows_gan.py` & `monai-weekly-1.2.dev2318/tests/test_integration_workflows_gan.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_intensity_stats.py` & `monai-weekly-1.2.dev2318/tests/test_intensity_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_intensity_statsd.py` & `monai-weekly-1.2.dev2318/tests/test_intensity_statsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_inverse.py` & `monai-weekly-1.2.dev2318/tests/test_inverse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_inverse_array.py` & `monai-weekly-1.2.dev2318/tests/test_inverse_array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_inverse_collation.py` & `monai-weekly-1.2.dev2318/tests/test_inverse_collation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_invertd.py` & `monai-weekly-1.2.dev2318/tests/test_invertd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_is_supported_format.py` & `monai-weekly-1.2.dev2318/tests/test_is_supported_format.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_iterable_dataset.py` & `monai-weekly-1.2.dev2318/tests/test_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_itk_torch_bridge.py` & `monai-weekly-1.2.dev2318/tests/test_itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_itk_writer.py` & `monai-weekly-1.2.dev2318/tests/test_itk_writer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_k_space_spike_noise.py` & `monai-weekly-1.2.dev2318/tests/test_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_k_space_spike_noised.py` & `monai-weekly-1.2.dev2318/tests/test_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_keep_largest_connected_component.py` & `monai-weekly-1.2.dev2318/tests/test_keep_largest_connected_component.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_keep_largest_connected_componentd.py` & `monai-weekly-1.2.dev2318/tests/test_keep_largest_connected_componentd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_kspace_mask.py` & `monai-weekly-1.2.dev2318/tests/test_kspace_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_label_filter.py` & `monai-weekly-1.2.dev2318/tests/test_label_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_label_filterd.py` & `monai-weekly-1.2.dev2318/tests/test_label_filterd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_label_quality_score.py` & `monai-weekly-1.2.dev2318/tests/test_label_quality_score.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_label_to_contour.py` & `monai-weekly-1.2.dev2318/tests/test_label_to_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_label_to_contourd.py` & `monai-weekly-1.2.dev2318/tests/test_label_to_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_label_to_mask.py` & `monai-weekly-1.2.dev2318/tests/test_label_to_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_label_to_maskd.py` & `monai-weekly-1.2.dev2318/tests/test_label_to_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_lambda.py` & `monai-weekly-1.2.dev2318/tests/test_lambda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_lambdad.py` & `monai-weekly-1.2.dev2318/tests/test_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_lesion_froc.py` & `monai-weekly-1.2.dev2318/tests/test_lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_list_data_collate.py` & `monai-weekly-1.2.dev2318/tests/test_list_data_collate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_list_to_dict.py` & `monai-weekly-1.2.dev2318/tests/test_list_to_dict.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_lltm.py` & `monai-weekly-1.2.dev2318/tests/test_lltm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_lmdbdataset.py` & `monai-weekly-1.2.dev2318/tests/test_lmdbdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_lmdbdataset_dist.py` & `monai-weekly-1.2.dev2318/tests/test_lmdbdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_load_decathlon_datalist.py` & `monai-weekly-1.2.dev2318/tests/test_load_decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_load_image.py` & `monai-weekly-1.2.dev2318/tests/test_load_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_load_imaged.py` & `monai-weekly-1.2.dev2318/tests/test_load_imaged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_load_spacing_orientation.py` & `monai-weekly-1.2.dev2318/tests/test_load_spacing_orientation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_loader_semaphore.py` & `monai-weekly-1.2.dev2318/tests/test_loader_semaphore.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_local_normalized_cross_correlation_loss.py` & `monai-weekly-1.2.dev2318/tests/test_local_normalized_cross_correlation_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_localnet.py` & `monai-weekly-1.2.dev2318/tests/test_localnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_localnet_block.py` & `monai-weekly-1.2.dev2318/tests/test_localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_look_up_option.py` & `monai-weekly-1.2.dev2318/tests/test_look_up_option.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_loss_metric.py` & `monai-weekly-1.2.dev2318/tests/test_loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_lr_finder.py` & `monai-weekly-1.2.dev2318/tests/test_lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_lr_scheduler.py` & `monai-weekly-1.2.dev2318/tests/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_make_nifti.py` & `monai-weekly-1.2.dev2318/tests/test_make_nifti.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_map_binary_to_indices.py` & `monai-weekly-1.2.dev2318/tests/test_map_binary_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_map_classes_to_indices.py` & `monai-weekly-1.2.dev2318/tests/test_map_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_map_label_value.py` & `monai-weekly-1.2.dev2318/tests/test_map_label_value.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_map_label_valued.py` & `monai-weekly-1.2.dev2318/tests/test_map_label_valued.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_map_transform.py` & `monai-weekly-1.2.dev2318/tests/test_map_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_mask_intensity.py` & `monai-weekly-1.2.dev2318/tests/test_mask_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_mask_intensityd.py` & `monai-weekly-1.2.dev2318/tests/test_mask_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_masked_dice_loss.py` & `monai-weekly-1.2.dev2318/tests/test_masked_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_masked_loss.py` & `monai-weekly-1.2.dev2318/tests/test_masked_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_masked_patch_wsi_dataset.py` & `monai-weekly-1.2.dev2318/tests/test_masked_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_matshow3d.py` & `monai-weekly-1.2.dev2318/tests/test_matshow3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_mean_ensemble.py` & `monai-weekly-1.2.dev2318/tests/test_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_mean_ensembled.py` & `monai-weekly-1.2.dev2318/tests/test_mean_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_median_filter.py` & `monai-weekly-1.2.dev2318/tests/test_median_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_median_smooth.py` & `monai-weekly-1.2.dev2318/tests/test_median_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_median_smoothd.py` & `monai-weekly-1.2.dev2318/tests/test_median_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_mednistdataset.py` & `monai-weekly-1.2.dev2318/tests/test_mednistdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_meta_affine.py` & `monai-weekly-1.2.dev2318/tests/test_meta_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_meta_tensor.py` & `monai-weekly-1.2.dev2318/tests/test_meta_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_metatensor_integration.py` & `monai-weekly-1.2.dev2318/tests/test_metatensor_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_metrics_reloaded.py` & `monai-weekly-1.2.dev2318/tests/test_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_milmodel.py` & `monai-weekly-1.2.dev2318/tests/test_milmodel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_mlp.py` & `monai-weekly-1.2.dev2318/tests/test_mlp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_mmar_download.py` & `monai-weekly-1.2.dev2318/tests/test_mmar_download.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_module_list.py` & `monai-weekly-1.2.dev2318/tests/test_module_list.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_monai_env_vars.py` & `monai-weekly-1.2.dev2318/tests/test_monai_env_vars.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_mri_utils.py` & `monai-weekly-1.2.dev2318/tests/test_mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_multi_scale.py` & `monai-weekly-1.2.dev2318/tests/test_multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_net_adapter.py` & `monai-weekly-1.2.dev2318/tests/test_net_adapter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_network_consistency.py` & `monai-weekly-1.2.dev2318/tests/test_network_consistency.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_nifti_endianness.py` & `monai-weekly-1.2.dev2318/tests/test_nifti_endianness.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_nifti_header_revise.py` & `monai-weekly-1.2.dev2318/tests/test_nifti_header_revise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_nifti_rw.py` & `monai-weekly-1.2.dev2318/tests/test_nifti_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_normalize_intensity.py` & `monai-weekly-1.2.dev2318/tests/test_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_normalize_intensityd.py` & `monai-weekly-1.2.dev2318/tests/test_normalize_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_npzdictitemdataset.py` & `monai-weekly-1.2.dev2318/tests/test_npzdictitemdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_nrrd_reader.py` & `monai-weekly-1.2.dev2318/tests/test_nrrd_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_nuclick_transforms.py` & `monai-weekly-1.2.dev2318/tests/test_nuclick_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_numpy_reader.py` & `monai-weekly-1.2.dev2318/tests/test_numpy_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_nvtx_decorator.py` & `monai-weekly-1.2.dev2318/tests/test_nvtx_decorator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_nvtx_transform.py` & `monai-weekly-1.2.dev2318/tests/test_nvtx_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_occlusion_sensitivity.py` & `monai-weekly-1.2.dev2318/tests/test_occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_one_of.py` & `monai-weekly-1.2.dev2318/tests/test_one_of.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_optim_novograd.py` & `monai-weekly-1.2.dev2318/tests/test_optim_novograd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_optional_import.py` & `monai-weekly-1.2.dev2318/tests/test_optional_import.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_ori_ras_lps.py` & `monai-weekly-1.2.dev2318/tests/test_ori_ras_lps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_orientation.py` & `monai-weekly-1.2.dev2318/tests/test_orientation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_orientationd.py` & `monai-weekly-1.2.dev2318/tests/test_orientationd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_p3d_block.py` & `monai-weekly-1.2.dev2318/tests/test_p3d_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_pad_collation.py` & `monai-weekly-1.2.dev2318/tests/test_pad_collation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_pad_mode.py` & `monai-weekly-1.2.dev2318/tests/test_pad_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_parallel_execution.py` & `monai-weekly-1.2.dev2318/tests/test_parallel_execution.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_parallel_execution_dist.py` & `monai-weekly-1.2.dev2318/tests/test_parallel_execution_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_partition_dataset.py` & `monai-weekly-1.2.dev2318/tests/test_partition_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_partition_dataset_classes.py` & `monai-weekly-1.2.dev2318/tests/test_partition_dataset_classes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_patch_dataset.py` & `monai-weekly-1.2.dev2318/tests/test_patch_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_patch_inferer.py` & `monai-weekly-1.2.dev2318/tests/test_patch_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_patch_wsi_dataset.py` & `monai-weekly-1.2.dev2318/tests/test_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_patchembedding.py` & `monai-weekly-1.2.dev2318/tests/test_patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_pathology_he_stain.py` & `monai-weekly-1.2.dev2318/tests/test_pathology_he_stain.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_pathology_he_stain_dict.py` & `monai-weekly-1.2.dev2318/tests/test_pathology_he_stain_dict.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_pathology_prob_nms.py` & `monai-weekly-1.2.dev2318/tests/test_pathology_prob_nms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_persistentdataset.py` & `monai-weekly-1.2.dev2318/tests/test_persistentdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_persistentdataset_dist.py` & `monai-weekly-1.2.dev2318/tests/test_persistentdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_phl_cpu.py` & `monai-weekly-1.2.dev2318/tests/test_phl_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_phl_cuda.py` & `monai-weekly-1.2.dev2318/tests/test_phl_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_pil_reader.py` & `monai-weekly-1.2.dev2318/tests/test_pil_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_plot_2d_or_3d_image.py` & `monai-weekly-1.2.dev2318/tests/test_plot_2d_or_3d_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_png_rw.py` & `monai-weekly-1.2.dev2318/tests/test_png_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_polyval.py` & `monai-weekly-1.2.dev2318/tests/test_polyval.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_prepare_batch_default.py` & `monai-weekly-1.2.dev2318/tests/test_prepare_batch_default.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_prepare_batch_default_dist.py` & `monai-weekly-1.2.dev2318/tests/test_prepare_batch_default_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_prepare_batch_extra_input.py` & `monai-weekly-1.2.dev2318/tests/test_prepare_batch_extra_input.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_prepare_batch_hovernet.py` & `monai-weekly-1.2.dev2318/tests/test_prepare_batch_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_preset_filters.py` & `monai-weekly-1.2.dev2318/tests/test_preset_filters.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_print_info.py` & `monai-weekly-1.2.dev2318/tests/test_print_info.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_print_transform_backends.py` & `monai-weekly-1.2.dev2318/tests/test_print_transform_backends.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_probnms.py` & `monai-weekly-1.2.dev2318/tests/test_probnms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_probnmsd.py` & `monai-weekly-1.2.dev2318/tests/test_probnmsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_profiling.py` & `monai-weekly-1.2.dev2318/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_pytorch_version_after.py` & `monai-weekly-1.2.dev2318/tests/test_pytorch_version_after.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_query_memory.py` & `monai-weekly-1.2.dev2318/tests/test_query_memory.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_adjust_contrast.py` & `monai-weekly-1.2.dev2318/tests/test_rand_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_adjust_contrastd.py` & `monai-weekly-1.2.dev2318/tests/test_rand_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_affine.py` & `monai-weekly-1.2.dev2318/tests/test_rand_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_affine_grid.py` & `monai-weekly-1.2.dev2318/tests/test_rand_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_affined.py` & `monai-weekly-1.2.dev2318/tests/test_rand_affined.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_axis_flip.py` & `monai-weekly-1.2.dev2318/tests/test_rand_axis_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_axis_flipd.py` & `monai-weekly-1.2.dev2318/tests/test_rand_axis_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_bias_field.py` & `monai-weekly-1.2.dev2318/tests/test_rand_bias_field.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_bias_fieldd.py` & `monai-weekly-1.2.dev2318/tests/test_rand_bias_fieldd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_coarse_dropout.py` & `monai-weekly-1.2.dev2318/tests/test_rand_coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_coarse_dropoutd.py` & `monai-weekly-1.2.dev2318/tests/test_rand_coarse_dropoutd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_coarse_shuffle.py` & `monai-weekly-1.2.dev2318/tests/test_rand_coarse_shuffle.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_coarse_shuffled.py` & `monai-weekly-1.2.dev2318/tests/test_rand_coarse_shuffled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_crop_by_label_classes.py` & `monai-weekly-1.2.dev2318/tests/test_rand_crop_by_label_classes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_crop_by_label_classesd.py` & `monai-weekly-1.2.dev2318/tests/test_rand_crop_by_label_classesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_crop_by_pos_neg_label.py` & `monai-weekly-1.2.dev2318/tests/test_rand_crop_by_pos_neg_label.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_crop_by_pos_neg_labeld.py` & `monai-weekly-1.2.dev2318/tests/test_rand_crop_by_pos_neg_labeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_cucim_dict_transform.py` & `monai-weekly-1.2.dev2318/tests/test_rand_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_cucim_transform.py` & `monai-weekly-1.2.dev2318/tests/test_rand_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_deform_grid.py` & `monai-weekly-1.2.dev2318/tests/test_rand_deform_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_elastic_2d.py` & `monai-weekly-1.2.dev2318/tests/test_rand_elastic_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_elastic_3d.py` & `monai-weekly-1.2.dev2318/tests/test_rand_elastic_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_elasticd_2d.py` & `monai-weekly-1.2.dev2318/tests/test_rand_elasticd_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_elasticd_3d.py` & `monai-weekly-1.2.dev2318/tests/test_rand_elasticd_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_flip.py` & `monai-weekly-1.2.dev2318/tests/test_rand_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_flipd.py` & `monai-weekly-1.2.dev2318/tests/test_rand_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_gaussian_noise.py` & `monai-weekly-1.2.dev2318/tests/test_rand_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_gaussian_noised.py` & `monai-weekly-1.2.dev2318/tests/test_rand_gaussian_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_gaussian_sharpen.py` & `monai-weekly-1.2.dev2318/tests/test_rand_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_gaussian_sharpend.py` & `monai-weekly-1.2.dev2318/tests/test_rand_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_gaussian_smooth.py` & `monai-weekly-1.2.dev2318/tests/test_rand_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_gaussian_smoothd.py` & `monai-weekly-1.2.dev2318/tests/test_rand_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_gibbs_noise.py` & `monai-weekly-1.2.dev2318/tests/test_rand_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_gibbs_noised.py` & `monai-weekly-1.2.dev2318/tests/test_rand_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_grid_distortion.py` & `monai-weekly-1.2.dev2318/tests/test_rand_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_grid_distortiond.py` & `monai-weekly-1.2.dev2318/tests/test_rand_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_grid_patch.py` & `monai-weekly-1.2.dev2318/tests/test_rand_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_grid_patchd.py` & `monai-weekly-1.2.dev2318/tests/test_rand_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_histogram_shift.py` & `monai-weekly-1.2.dev2318/tests/test_rand_histogram_shift.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_histogram_shiftd.py` & `monai-weekly-1.2.dev2318/tests/test_rand_histogram_shiftd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_k_space_spike_noise.py` & `monai-weekly-1.2.dev2318/tests/test_rand_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_k_space_spike_noised.py` & `monai-weekly-1.2.dev2318/tests/test_rand_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_lambda.py` & `monai-weekly-1.2.dev2318/tests/test_rand_lambda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_lambdad.py` & `monai-weekly-1.2.dev2318/tests/test_rand_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_rician_noise.py` & `monai-weekly-1.2.dev2318/tests/test_rand_rician_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_rician_noised.py` & `monai-weekly-1.2.dev2318/tests/test_rand_rician_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_rotate.py` & `monai-weekly-1.2.dev2318/tests/test_rand_rotate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_rotate90.py` & `monai-weekly-1.2.dev2318/tests/test_rand_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_rotate90d.py` & `monai-weekly-1.2.dev2318/tests/test_rand_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_rotated.py` & `monai-weekly-1.2.dev2318/tests/test_rand_rotated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_scale_crop.py` & `monai-weekly-1.2.dev2318/tests/test_rand_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_scale_cropd.py` & `monai-weekly-1.2.dev2318/tests/test_rand_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_scale_intensity.py` & `monai-weekly-1.2.dev2318/tests/test_rand_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_scale_intensityd.py` & `monai-weekly-1.2.dev2318/tests/test_rand_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_shift_intensity.py` & `monai-weekly-1.2.dev2318/tests/test_rand_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_shift_intensityd.py` & `monai-weekly-1.2.dev2318/tests/test_rand_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_spatial_crop.py` & `monai-weekly-1.2.dev2318/tests/test_rand_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_spatial_crop_samples.py` & `monai-weekly-1.2.dev2318/tests/test_rand_spatial_crop_samples.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_spatial_crop_samplesd.py` & `monai-weekly-1.2.dev2318/tests/test_rand_spatial_crop_samplesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_spatial_cropd.py` & `monai-weekly-1.2.dev2318/tests/test_rand_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_std_shift_intensity.py` & `monai-weekly-1.2.dev2318/tests/test_rand_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_std_shift_intensityd.py` & `monai-weekly-1.2.dev2318/tests/test_rand_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_weighted_crop.py` & `monai-weekly-1.2.dev2318/tests/test_rand_weighted_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_weighted_cropd.py` & `monai-weekly-1.2.dev2318/tests/test_rand_weighted_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_zoom.py` & `monai-weekly-1.2.dev2318/tests/test_rand_zoom.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rand_zoomd.py` & `monai-weekly-1.2.dev2318/tests/test_rand_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_randidentity.py` & `monai-weekly-1.2.dev2318/tests/test_randidentity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_random_order.py` & `monai-weekly-1.2.dev2318/tests/test_random_order.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_randomizable.py` & `monai-weekly-1.2.dev2318/tests/test_randomizable.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_randomizable_transform_type.py` & `monai-weekly-1.2.dev2318/tests/test_randomizable_transform_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_randtorchvisiond.py` & `monai-weekly-1.2.dev2318/tests/test_randtorchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rankfilter_dist.py` & `monai-weekly-1.2.dev2318/tests/test_rankfilter_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_recon_net_utils.py` & `monai-weekly-1.2.dev2318/tests/test_recon_net_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_reference_based_normalize_intensity.py` & `monai-weekly-1.2.dev2318/tests/test_reference_based_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_reference_based_spatial_cropd.py` & `monai-weekly-1.2.dev2318/tests/test_reference_based_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_reference_resolver.py` & `monai-weekly-1.2.dev2318/tests/test_reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_reg_loss_integration.py` & `monai-weekly-1.2.dev2318/tests/test_reg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_regunet.py` & `monai-weekly-1.2.dev2318/tests/test_regunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_regunet_block.py` & `monai-weekly-1.2.dev2318/tests/test_regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_remove_repeated_channel.py` & `monai-weekly-1.2.dev2318/tests/test_remove_repeated_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_remove_repeated_channeld.py` & `monai-weekly-1.2.dev2318/tests/test_remove_repeated_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_remove_small_objects.py` & `monai-weekly-1.2.dev2318/tests/test_remove_small_objects.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_repeat_channel.py` & `monai-weekly-1.2.dev2318/tests/test_repeat_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_repeat_channeld.py` & `monai-weekly-1.2.dev2318/tests/test_repeat_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_replace_module.py` & `monai-weekly-1.2.dev2318/tests/test_replace_module.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_require_pkg.py` & `monai-weekly-1.2.dev2318/tests/test_require_pkg.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_resample.py` & `monai-weekly-1.2.dev2318/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_resample_backends.py` & `monai-weekly-1.2.dev2318/tests/test_resample_backends.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_resample_datalist.py` & `monai-weekly-1.2.dev2318/tests/test_resample_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_resample_to_match.py` & `monai-weekly-1.2.dev2318/tests/test_resample_to_match.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_resample_to_matchd.py` & `monai-weekly-1.2.dev2318/tests/test_resample_to_matchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_resampler.py` & `monai-weekly-1.2.dev2318/tests/test_resampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_resize.py` & `monai-weekly-1.2.dev2318/tests/test_resize.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 TEST_CASE_0 = [{"spatial_size": 15}, (6, 10, 15)]
 
 TEST_CASE_1 = [{"spatial_size": 15, "mode": "area"}, (6, 10, 15)]
 
 TEST_CASE_2 = [{"spatial_size": 6, "mode": "trilinear", "align_corners": True}, (2, 4, 6)]
 
+TEST_CASE_2_1 = [{"spatial_size": 6, "mode": 1, "align_corners": True}, (2, 4, 6)]
+
 TEST_CASE_3 = [{"spatial_size": 15, "anti_aliasing": True}, (6, 10, 15)]
 
 TEST_CASE_4 = [{"spatial_size": 6, "anti_aliasing": True, "anti_aliasing_sigma": 2.0}, (2, 4, 6)]
 
 diff_t = 0.3 if is_tf32_env() else 0.2
 
 
@@ -104,15 +106,15 @@
             if isinstance(out, torch.Tensor):
                 out = out.cpu().detach().numpy()
             good = np.sum(np.isclose(expected, out, atol=0.9))
             self.assertLessEqual(
                 np.abs(good - expected.size) / float(expected.size), diff_t, f"at most {diff_t} percent mismatch "
             )
 
-    @parameterized.expand([TEST_CASE_0, TEST_CASE_1, TEST_CASE_2, TEST_CASE_3, TEST_CASE_4])
+    @parameterized.expand([TEST_CASE_0, TEST_CASE_1, TEST_CASE_2, TEST_CASE_2_1, TEST_CASE_3, TEST_CASE_4])
     def test_longest_shape(self, input_param, expected_shape):
         input_data = np.random.randint(0, 2, size=[3, 4, 7, 10])
         input_param["size_mode"] = "longest"
         result = Resize(**input_param)(input_data)
         np.testing.assert_allclose(result.shape[1:], expected_shape)
 
         set_track_meta(False)
```

### Comparing `monai-weekly-1.2.dev2317/tests/test_resize_with_pad_or_crop.py` & `monai-weekly-1.2.dev2318/tests/test_resize_with_pad_or_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_resize_with_pad_or_cropd.py` & `monai-weekly-1.2.dev2318/tests/test_resize_with_pad_or_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_resized.py` & `monai-weekly-1.2.dev2318/tests/test_resized.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_resnet.py` & `monai-weekly-1.2.dev2318/tests/test_resnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_retinanet.py` & `monai-weekly-1.2.dev2318/tests/test_retinanet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_retinanet_detector.py` & `monai-weekly-1.2.dev2318/tests/test_retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_retinanet_predict_utils.py` & `monai-weekly-1.2.dev2318/tests/test_retinanet_predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rotate.py` & `monai-weekly-1.2.dev2318/tests/test_rotate.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,31 +18,35 @@
 import torch
 from parameterized import parameterized
 
 from monai.config import USE_COMPILED
 from monai.data import MetaTensor, set_track_meta
 from monai.transforms import Rotate
 from tests.lazy_transforms_utils import test_resampler_lazy
-from tests.utils import TEST_NDARRAYS_ALL, NumpyImageTestCase2D, NumpyImageTestCase3D, test_local_inversion
+from tests.utils import HAS_CUPY, TEST_NDARRAYS_ALL, NumpyImageTestCase2D, NumpyImageTestCase3D, test_local_inversion
 
 TEST_CASES_2D: list[tuple] = []
 for p in TEST_NDARRAYS_ALL:
     TEST_CASES_2D.append((p, np.pi / 6, False, "bilinear", "border", False))
     TEST_CASES_2D.append((p, np.pi / 4, True, "bilinear", "border", False))
     TEST_CASES_2D.append((p, -np.pi / 4.5, True, "nearest", "border" if USE_COMPILED else "reflection", False))
     TEST_CASES_2D.append((p, np.pi, False, "nearest", "zeros", False))
     TEST_CASES_2D.append((p, -np.pi / 2, False, "bilinear", "zeros", True))
+    if HAS_CUPY:  # 1 and cuda image requires cupy
+        TEST_CASES_2D.append((p, -np.pi / 2, False, 1, "constant", True))
 
 TEST_CASES_3D: list[tuple] = []
 for p in TEST_NDARRAYS_ALL:
     TEST_CASES_3D.append((p, -np.pi / 2, True, "nearest", "border", False))
     TEST_CASES_3D.append((p, np.pi / 4, True, "bilinear", "border", False))
     TEST_CASES_3D.append((p, -np.pi / 4.5, True, "nearest", "border" if USE_COMPILED else "reflection", False))
     TEST_CASES_3D.append((p, np.pi, False, "nearest", "zeros", False))
     TEST_CASES_3D.append((p, -np.pi / 2, False, "bilinear", "zeros", False))
+    if HAS_CUPY:
+        TEST_CASES_3D.append((p, -np.pi / 2, False, 1, "zeros", False))
 
 TEST_CASES_SHAPE_3D: list[tuple] = []
 for p in TEST_NDARRAYS_ALL:
     TEST_CASES_SHAPE_3D.append((p, [-np.pi / 2, 1.0, 2.0], "nearest", "border", False))
     TEST_CASES_SHAPE_3D.append((p, [np.pi / 4, 0, 0], "bilinear", "border", False))
     TEST_CASES_SHAPE_3D.append((p, [-np.pi / 4.5, -20, 20], "nearest", "reflection", False))
 
@@ -139,12 +143,12 @@
         for p in TEST_NDARRAYS_ALL:
             rotate_fn = Rotate(10, True)
             with self.assertRaises(ValueError):  # wrong shape
                 rotate_fn(p(self.imt))
 
             rotate_fn = Rotate(10, keep_size=False)
             with self.assertRaises(ValueError):  # wrong mode
-                rotate_fn(p(self.imt[0]), mode="trilinear")
+                rotate_fn(p(self.imt[0]), mode="trilinear_spell_error")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2317/tests/test_rotate90.py` & `monai-weekly-1.2.dev2318/tests/test_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rotate90d.py` & `monai-weekly-1.2.dev2318/tests/test_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_rotated.py` & `monai-weekly-1.2.dev2318/tests/test_rotated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_safe_dtype_range.py` & `monai-weekly-1.2.dev2318/tests/test_safe_dtype_range.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_saliency_inferer.py` & `monai-weekly-1.2.dev2318/tests/test_saliency_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_sample_slices.py` & `monai-weekly-1.2.dev2318/tests/test_sample_slices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_sampler_dist.py` & `monai-weekly-1.2.dev2318/tests/test_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_save_classificationd.py` & `monai-weekly-1.2.dev2318/tests/test_save_classificationd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_save_image.py` & `monai-weekly-1.2.dev2318/tests/test_save_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_save_imaged.py` & `monai-weekly-1.2.dev2318/tests/test_save_imaged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_save_state.py` & `monai-weekly-1.2.dev2318/tests/test_save_state.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_savitzky_golay_filter.py` & `monai-weekly-1.2.dev2318/tests/test_savitzky_golay_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_savitzky_golay_smooth.py` & `monai-weekly-1.2.dev2318/tests/test_savitzky_golay_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_savitzky_golay_smoothd.py` & `monai-weekly-1.2.dev2318/tests/test_savitzky_golay_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_scale_intensity.py` & `monai-weekly-1.2.dev2318/tests/test_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_scale_intensity_range.py` & `monai-weekly-1.2.dev2318/tests/test_scale_intensity_range.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_scale_intensity_range_percentiles.py` & `monai-weekly-1.2.dev2318/tests/test_scale_intensity_range_percentiles.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_scale_intensity_range_percentilesd.py` & `monai-weekly-1.2.dev2318/tests/test_scale_intensity_range_percentilesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_scale_intensity_ranged.py` & `monai-weekly-1.2.dev2318/tests/test_scale_intensity_ranged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_scale_intensityd.py` & `monai-weekly-1.2.dev2318/tests/test_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_se_block.py` & `monai-weekly-1.2.dev2318/tests/test_se_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_se_blocks.py` & `monai-weekly-1.2.dev2318/tests/test_se_blocks.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_seg_loss_integration.py` & `monai-weekly-1.2.dev2318/tests/test_seg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_segresnet.py` & `monai-weekly-1.2.dev2318/tests/test_segresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_segresnet_block.py` & `monai-weekly-1.2.dev2318/tests/test_segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_segresnet_ds.py` & `monai-weekly-1.2.dev2318/tests/test_segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_select_cross_validation_folds.py` & `monai-weekly-1.2.dev2318/tests/test_select_cross_validation_folds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_select_itemsd.py` & `monai-weekly-1.2.dev2318/tests/test_select_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_selfattention.py` & `monai-weekly-1.2.dev2318/tests/test_selfattention.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_senet.py` & `monai-weekly-1.2.dev2318/tests/test_senet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_separable_filter.py` & `monai-weekly-1.2.dev2318/tests/test_separable_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_set_determinism.py` & `monai-weekly-1.2.dev2318/tests/test_set_determinism.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_set_visible_devices.py` & `monai-weekly-1.2.dev2318/tests/test_set_visible_devices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_shift_intensity.py` & `monai-weekly-1.2.dev2318/tests/test_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_shift_intensityd.py` & `monai-weekly-1.2.dev2318/tests/test_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_shuffle_buffer.py` & `monai-weekly-1.2.dev2318/tests/test_shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_signal_continuouswavelet.py` & `monai-weekly-1.2.dev2318/tests/test_signal_continuouswavelet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_signal_fillempty.py` & `monai-weekly-1.2.dev2318/tests/test_signal_fillempty.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_signal_rand_add_gaussiannoise.py` & `monai-weekly-1.2.dev2318/tests/test_signal_rand_add_gaussiannoise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_signal_rand_add_sine.py` & `monai-weekly-1.2.dev2318/tests/test_signal_rand_add_sine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_signal_rand_add_sine_partial.py` & `monai-weekly-1.2.dev2318/tests/test_signal_rand_add_sine_partial.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_signal_rand_add_squarepulse.py` & `monai-weekly-1.2.dev2318/tests/test_signal_rand_add_squarepulse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_signal_rand_add_squarepulse_partial.py` & `monai-weekly-1.2.dev2318/tests/test_signal_rand_add_squarepulse_partial.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_signal_rand_drop.py` & `monai-weekly-1.2.dev2318/tests/test_signal_rand_drop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_signal_rand_scale.py` & `monai-weekly-1.2.dev2318/tests/test_signal_rand_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_signal_rand_shift.py` & `monai-weekly-1.2.dev2318/tests/test_signal_rand_shift.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_signal_remove_frequency.py` & `monai-weekly-1.2.dev2318/tests/test_signal_remove_frequency.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_simple_aspp.py` & `monai-weekly-1.2.dev2318/tests/test_simple_aspp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_simulatedelay.py` & `monai-weekly-1.2.dev2318/tests/test_simulatedelay.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_simulatedelayd.py` & `monai-weekly-1.2.dev2318/tests/test_simulatedelayd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_skip_connection.py` & `monai-weekly-1.2.dev2318/tests/test_skip_connection.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_slice_inferer.py` & `monai-weekly-1.2.dev2318/tests/test_slice_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_sliding_patch_wsi_dataset.py` & `monai-weekly-1.2.dev2318/tests/test_sliding_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_sliding_window_hovernet_inference.py` & `monai-weekly-1.2.dev2318/tests/test_sliding_window_hovernet_inference.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_sliding_window_inference.py` & `monai-weekly-1.2.dev2318/tests/test_sliding_window_inference.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_sliding_window_splitter.py` & `monai-weekly-1.2.dev2318/tests/test_sliding_window_splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_smartcachedataset.py` & `monai-weekly-1.2.dev2318/tests/test_smartcachedataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_smooth_field.py` & `monai-weekly-1.2.dev2318/tests/test_smooth_field.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_sobel_gradient.py` & `monai-weekly-1.2.dev2318/tests/test_sobel_gradient.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_sobel_gradientd.py` & `monai-weekly-1.2.dev2318/tests/test_sobel_gradientd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_some_of.py` & `monai-weekly-1.2.dev2318/tests/test_some_of.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_spacing.py` & `monai-weekly-1.2.dev2318/tests/test_spacing.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
             {},
             torch.ones((1, 2, 2, 3, 1)),
             *device,
         ]
     )
     TESTS.append(  # 5D input
         [
-            {"pixdim": 0.5, "padding_mode": "zeros", "mode": "nearest", "scale_extent": True},
+            {"pixdim": 0.5, "padding_mode": "constant", "mode": "nearest", "scale_extent": True},
             torch.ones((1, 368, 336, 368)),  # data
             torch.tensor(
                 [
                     [0.41, 0.005, 0.008, -79.7],
                     [-0.0049, 0.592, 0.0664, -57.4],
                     [-0.0073, -0.0972, 0.404, -32.1],
                     [0.0, 0.0, 0.0, 1.0],
```

### Comparing `monai-weekly-1.2.dev2317/tests/test_spacingd.py` & `monai-weekly-1.2.dev2318/tests/test_spacingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_spatial_combine_transforms.py` & `monai-weekly-1.2.dev2318/tests/test_spatial_combine_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_spatial_crop.py` & `monai-weekly-1.2.dev2318/tests/test_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_spatial_cropd.py` & `monai-weekly-1.2.dev2318/tests/test_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_spatial_pad.py` & `monai-weekly-1.2.dev2318/tests/test_spatial_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_spatial_padd.py` & `monai-weekly-1.2.dev2318/tests/test_spatial_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_spatial_resample.py` & `monai-weekly-1.2.dev2318/tests/test_spatial_resample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_spatial_resampled.py` & `monai-weekly-1.2.dev2318/tests/test_spatial_resampled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_split_channel.py` & `monai-weekly-1.2.dev2318/tests/test_split_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_split_channeld.py` & `monai-weekly-1.2.dev2318/tests/test_split_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_splitdim.py` & `monai-weekly-1.2.dev2318/tests/test_splitdim.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_splitdimd.py` & `monai-weekly-1.2.dev2318/tests/test_splitdimd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_squeezedim.py` & `monai-weekly-1.2.dev2318/tests/test_squeezedim.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_squeezedimd.py` & `monai-weekly-1.2.dev2318/tests/test_squeezedimd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_ssim_loss.py` & `monai-weekly-1.2.dev2318/tests/test_ssim_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_ssim_metric.py` & `monai-weekly-1.2.dev2318/tests/test_ssim_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_state_cacher.py` & `monai-weekly-1.2.dev2318/tests/test_state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_std_shift_intensity.py` & `monai-weekly-1.2.dev2318/tests/test_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_std_shift_intensityd.py` & `monai-weekly-1.2.dev2318/tests/test_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_str2bool.py` & `monai-weekly-1.2.dev2318/tests/test_str2bool.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_str2list.py` & `monai-weekly-1.2.dev2318/tests/test_str2list.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_subpixel_upsample.py` & `monai-weekly-1.2.dev2318/tests/test_subpixel_upsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_surface_dice.py` & `monai-weekly-1.2.dev2318/tests/test_surface_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_surface_distance.py` & `monai-weekly-1.2.dev2318/tests/test_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_swin_unetr.py` & `monai-weekly-1.2.dev2318/tests/test_swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_synthetic.py` & `monai-weekly-1.2.dev2318/tests/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_tciadataset.py` & `monai-weekly-1.2.dev2318/tests/test_tciadataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_testtimeaugmentation.py` & `monai-weekly-1.2.dev2318/tests/test_testtimeaugmentation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_text_encoding.py` & `monai-weekly-1.2.dev2318/tests/test_text_encoding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_thread_buffer.py` & `monai-weekly-1.2.dev2318/tests/test_thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_threadcontainer.py` & `monai-weekly-1.2.dev2318/tests/test_threadcontainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_threshold_intensity.py` & `monai-weekly-1.2.dev2318/tests/test_threshold_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_threshold_intensityd.py` & `monai-weekly-1.2.dev2318/tests/test_threshold_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_timedcall_dist.py` & `monai-weekly-1.2.dev2318/tests/test_timedcall_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_to_contiguous.py` & `monai-weekly-1.2.dev2318/tests/test_to_contiguous.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_to_cupy.py` & `monai-weekly-1.2.dev2318/tests/test_to_cupy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_to_cupyd.py` & `monai-weekly-1.2.dev2318/tests/test_to_cupyd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_to_device.py` & `monai-weekly-1.2.dev2318/tests/test_to_device.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_to_deviced.py` & `monai-weekly-1.2.dev2318/tests/test_to_deviced.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_to_from_meta_tensord.py` & `monai-weekly-1.2.dev2318/tests/test_to_from_meta_tensord.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_to_numpy.py` & `monai-weekly-1.2.dev2318/tests/test_to_numpy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_to_numpyd.py` & `monai-weekly-1.2.dev2318/tests/test_to_numpyd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_to_onehot.py` & `monai-weekly-1.2.dev2318/tests/test_to_onehot.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_to_pil.py` & `monai-weekly-1.2.dev2318/tests/test_to_pil.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_to_pild.py` & `monai-weekly-1.2.dev2318/tests/test_to_pild.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_to_tensor.py` & `monai-weekly-1.2.dev2318/tests/test_to_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_to_tensord.py` & `monai-weekly-1.2.dev2318/tests/test_to_tensord.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_torchscript_utils.py` & `monai-weekly-1.2.dev2318/tests/test_torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_torchvision.py` & `monai-weekly-1.2.dev2318/tests/test_torchvision.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_torchvision_fc_model.py` & `monai-weekly-1.2.dev2318/tests/test_torchvision_fc_model.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_torchvisiond.py` & `monai-weekly-1.2.dev2318/tests/test_torchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_traceable_transform.py` & `monai-weekly-1.2.dev2318/tests/test_traceable_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_train_mode.py` & `monai-weekly-1.2.dev2318/tests/test_train_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_trainable_bilateral.py` & `monai-weekly-1.2.dev2318/tests/test_trainable_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_trainable_joint_bilateral.py` & `monai-weekly-1.2.dev2318/tests/test_trainable_joint_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_transchex.py` & `monai-weekly-1.2.dev2318/tests/test_transchex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_transform.py` & `monai-weekly-1.2.dev2318/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_transformerblock.py` & `monai-weekly-1.2.dev2318/tests/test_transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_transpose.py` & `monai-weekly-1.2.dev2318/tests/test_transpose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_transposed.py` & `monai-weekly-1.2.dev2318/tests/test_transposed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_tversky_loss.py` & `monai-weekly-1.2.dev2318/tests/test_tversky_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_unet.py` & `monai-weekly-1.2.dev2318/tests/test_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_unetr.py` & `monai-weekly-1.2.dev2318/tests/test_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_unetr_block.py` & `monai-weekly-1.2.dev2318/tests/test_unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_unified_focal_loss.py` & `monai-weekly-1.2.dev2318/tests/test_unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_upsample_block.py` & `monai-weekly-1.2.dev2318/tests/test_upsample_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_utils_pytorch_numpy_unification.py` & `monai-weekly-1.2.dev2318/tests/test_utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_varautoencoder.py` & `monai-weekly-1.2.dev2318/tests/test_varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_varnet.py` & `monai-weekly-1.2.dev2318/tests/test_varnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_version_leq.py` & `monai-weekly-1.2.dev2318/tests/test_version_leq.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_video_datasets.py` & `monai-weekly-1.2.dev2318/tests/test_video_datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_vis_cam.py` & `monai-weekly-1.2.dev2318/tests/test_vis_cam.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_vis_gradbased.py` & `monai-weekly-1.2.dev2318/tests/test_vis_gradbased.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_vis_gradcam.py` & `monai-weekly-1.2.dev2318/tests/test_vis_gradcam.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_vit.py` & `monai-weekly-1.2.dev2318/tests/test_vit.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_vitautoenc.py` & `monai-weekly-1.2.dev2318/tests/test_vitautoenc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_vnet.py` & `monai-weekly-1.2.dev2318/tests/test_vnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_vote_ensemble.py` & `monai-weekly-1.2.dev2318/tests/test_vote_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_vote_ensembled.py` & `monai-weekly-1.2.dev2318/tests/test_vote_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_warp.py` & `monai-weekly-1.2.dev2318/tests/test_warp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_watershed.py` & `monai-weekly-1.2.dev2318/tests/test_watershed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_watershedd.py` & `monai-weekly-1.2.dev2318/tests/test_watershedd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_weight_init.py` & `monai-weekly-1.2.dev2318/tests/test_weight_init.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_weighted_random_sampler_dist.py` & `monai-weekly-1.2.dev2318/tests/test_weighted_random_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_with_allow_missing_keys.py` & `monai-weekly-1.2.dev2318/tests/test_with_allow_missing_keys.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_write_metrics_reports.py` & `monai-weekly-1.2.dev2318/tests/test_write_metrics_reports.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_wsireader.py` & `monai-weekly-1.2.dev2318/tests/test_wsireader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_zipdataset.py` & `monai-weekly-1.2.dev2318/tests/test_zipdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_zoom.py` & `monai-weekly-1.2.dev2318/tests/test_zoom.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     test_local_inversion,
 )
 
 VALID_CASES = [
     (1.5, "nearest", True),
     (1.5, "nearest", False),
     (0.8, "bilinear"),
+    (0.8, 1),
     (0.8, "area"),
     (1.5, "nearest", False, True),
     (0.8, "area", False, True),
 ]
 
 INVALID_CASES = [((None, None), "bilinear", TypeError), ((0.9, 0.9), "s", ValueError)]
 
@@ -66,15 +67,15 @@
     def test_correct_results(self, zoom, mode, *_):
         for p in TEST_NDARRAYS_ALL:
             zoom_fn = Zoom(zoom=zoom, mode=mode, keep_size=False)
             im = p(self.imt[0])
             zoomed = zoom_fn(im)
             test_local_inversion(zoom_fn, zoomed, im)
             _order = 0
-            if mode.endswith("linear"):
+            if mode == 1 or mode.endswith("linear"):
                 _order = 1
             expected = []
             for channel in self.imt[0]:
                 expected.append(zoom_scipy(channel, zoom=zoom, mode="nearest", order=_order, prefilter=False))
             expected = np.stack(expected).astype(np.float32)
             assert_allclose(zoomed, p(expected), atol=1.0, type_test=False)
```

### Comparing `monai-weekly-1.2.dev2317/tests/test_zoom_affine.py` & `monai-weekly-1.2.dev2318/tests/test_zoom_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/tests/test_zoomd.py` & `monai-weekly-1.2.dev2318/tests/test_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2317/versioneer.py` & `monai-weekly-1.2.dev2318/versioneer.py`

 * *Files identical despite different names*

