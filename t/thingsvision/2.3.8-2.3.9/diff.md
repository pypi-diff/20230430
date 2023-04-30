# Comparing `tmp/thingsvision-2.3.8.tar.gz` & `tmp/thingsvision-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thingsvision-2.3.8.tar", last modified: Sun Mar  5 10:17:48 2023, max compression
+gzip compressed data, was "thingsvision-2.3.9.tar", last modified: Mon Mar  6 10:23:53 2023, max compression
```

## Comparing `thingsvision-2.3.8.tar` & `thingsvision-2.3.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-05 10:17:48.502551 thingsvision-2.3.8/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.3.8/LICENSE
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15999 2023-03-05 10:17:48.502219 thingsvision-2.3.8/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    13419 2023-03-02 12:32:50.000000 thingsvision-2.3.8/README.md
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2023-03-05 10:17:48.502630 thingsvision-2.3.8/setup.cfg
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1820 2023-03-05 10:17:07.000000 thingsvision-2.3.8/setup.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-05 10:17:48.468634 thingsvision-2.3.8/tests/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.3.8/tests/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-05 10:17:48.469850 thingsvision-2.3.8/tests/extractor/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.3.8/tests/extractor/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-05 10:17:48.472440 thingsvision-2.3.8/tests/extractor/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.3.8/tests/extractor/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2023-01-17 18:07:55.000000 thingsvision-2.3.8/tests/extractor/extraction/test_custom_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2023-02-24 09:48:38.000000 thingsvision-2.3.8/tests/extractor/extraction/test_model_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1656 2023-01-18 14:03:54.000000 thingsvision-2.3.8/tests/extractor/extraction/test_pretrained_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2359 2023-01-17 18:07:38.000000 thingsvision-2.3.8/tests/extractor/extraction/test_torch_vs_tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2022-10-26 15:18:20.000000 thingsvision-2.3.8/tests/extractor/test_load_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.3.8/tests/extractor/test_transformations.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8661 2023-03-02 18:14:59.000000 thingsvision-2.3.8/tests/helper.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2023-02-22 09:56:38.000000 thingsvision-2.3.8/tests/test_features.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3719 2022-08-31 09:02:04.000000 thingsvision-2.3.8/tests/test_rest.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-05 10:17:48.473811 thingsvision-2.3.8/thingsvision/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.3.8/thingsvision/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2023-03-05 10:17:17.000000 thingsvision-2.3.8/thingsvision/_version.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-05 10:17:48.475896 thingsvision-2.3.8/thingsvision/core/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.3.8/thingsvision/core/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-05 10:17:48.476631 thingsvision-2.3.8/thingsvision/core/cka/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       21 2022-08-22 09:49:44.000000 thingsvision-2.3.8/thingsvision/core/cka/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1974 2022-08-22 09:49:44.000000 thingsvision-2.3.8/thingsvision/core/cka/base.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-05 10:17:48.480030 thingsvision-2.3.8/thingsvision/core/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      193 2023-02-15 09:26:37.000000 thingsvision-2.3.8/thingsvision/core/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8269 2023-02-17 14:03:21.000000 thingsvision-2.3.8/thingsvision/core/extraction/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    13241 2023-02-22 09:56:38.000000 thingsvision-2.3.8/thingsvision/core/extraction/extractors.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7934 2023-03-02 12:32:50.000000 thingsvision-2.3.8/thingsvision/core/extraction/helpers.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2750 2023-02-24 09:48:38.000000 thingsvision-2.3.8/thingsvision/core/extraction/tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5199 2023-02-24 09:48:38.000000 thingsvision-2.3.8/thingsvision/core/extraction/torch.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-05 10:17:48.481397 thingsvision-2.3.8/thingsvision/core/rsa/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.3.8/thingsvision/core/rsa/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.3.8/thingsvision/core/rsa/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.3.8/thingsvision/core/rsa/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-05 10:17:48.496012 thingsvision-2.3.8/thingsvision/custom_models/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      327 2023-03-02 18:14:59.000000 thingsvision-2.3.8/thingsvision/custom_models/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      619 2022-09-22 09:46:01.000000 thingsvision-2.3.8/thingsvision/custom_models/alexnet_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      624 2022-12-20 12:41:31.000000 thingsvision-2.3.8/thingsvision/custom_models/alexnet_salobjsub.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-05 10:17:48.498306 thingsvision-2.3.8/thingsvision/custom_models/cornet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.3.8/thingsvision/custom_models/cornet/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.3.8/thingsvision/custom_models/cornet/cornet_r.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.3.8/thingsvision/custom_models/cornet/cornet_rt.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.3.8/thingsvision/custom_models/cornet/cornet_s.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.3.8/thingsvision/custom_models/cornet/cornet_z.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.3.8/thingsvision/custom_models/custom.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1301 2023-03-02 18:14:59.000000 thingsvision-2.3.8/thingsvision/custom_models/harmonization.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      628 2022-09-22 09:46:01.000000 thingsvision-2.3.8/thingsvision/custom_models/inception_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      511 2022-10-26 15:18:20.000000 thingsvision-2.3.8/thingsvision/custom_models/official_clip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      982 2022-10-26 15:18:20.000000 thingsvision-2.3.8/thingsvision/custom_models/openclip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      622 2022-09-22 09:46:01.000000 thingsvision-2.3.8/thingsvision/custom_models/resnet50_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      615 2023-02-24 09:48:36.000000 thingsvision-2.3.8/thingsvision/custom_models/vgg16_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-01-18 10:11:35.000000 thingsvision-2.3.8/thingsvision/custom_models/vgg16bn_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5812 2022-12-13 13:51:38.000000 thingsvision-2.3.8/thingsvision/thingsvision.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-05 10:17:48.498618 thingsvision-2.3.8/thingsvision/utils/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.3.8/thingsvision/utils/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-05 10:17:48.500089 thingsvision-2.3.8/thingsvision/utils/data/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.3.8/thingsvision/utils/data/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.3.8/thingsvision/utils/data/data_loader.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.3.8/thingsvision/utils/data/dataset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.3.8/thingsvision/utils/data/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-05 10:17:48.500660 thingsvision-2.3.8/thingsvision/utils/imagenet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.3.8/thingsvision/utils/imagenet/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-05 10:17:48.501427 thingsvision-2.3.8/thingsvision/utils/storing/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.3.8/thingsvision/utils/storing/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2023-02-22 09:56:38.000000 thingsvision-2.3.8/thingsvision/utils/storing/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-05 10:17:48.475662 thingsvision-2.3.8/thingsvision.egg-info/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15999 2023-03-05 10:17:48.000000 thingsvision-2.3.8/thingsvision.egg-info/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2185 2023-03-05 10:17:48.000000 thingsvision-2.3.8/thingsvision.egg-info/SOURCES.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       90 2023-03-05 10:17:48.000000 thingsvision-2.3.8/thingsvision.egg-info/dependency_links.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       65 2023-03-05 10:17:48.000000 thingsvision-2.3.8/thingsvision.egg-info/entry_points.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      394 2023-03-05 10:17:48.000000 thingsvision-2.3.8/thingsvision.egg-info/requires.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2023-03-05 10:17:48.000000 thingsvision-2.3.8/thingsvision.egg-info/top_level.txt
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.808122 thingsvision-2.3.9/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.3.9/LICENSE
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    14022 2023-03-06 10:23:53.807833 thingsvision-2.3.9/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    13419 2023-03-02 12:32:50.000000 thingsvision-2.3.9/README.md
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2023-03-06 10:23:53.808197 thingsvision-2.3.9/setup.cfg
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1824 2023-03-06 10:23:19.000000 thingsvision-2.3.9/setup.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.784160 thingsvision-2.3.9/tests/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.3.9/tests/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.786024 thingsvision-2.3.9/tests/extractor/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.3.9/tests/extractor/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.788524 thingsvision-2.3.9/tests/extractor/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.3.9/tests/extractor/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2023-01-17 18:07:55.000000 thingsvision-2.3.9/tests/extractor/extraction/test_custom_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2023-02-24 09:48:38.000000 thingsvision-2.3.9/tests/extractor/extraction/test_model_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1656 2023-01-18 14:03:54.000000 thingsvision-2.3.9/tests/extractor/extraction/test_pretrained_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2359 2023-01-17 18:07:38.000000 thingsvision-2.3.9/tests/extractor/extraction/test_torch_vs_tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2022-10-26 15:18:20.000000 thingsvision-2.3.9/tests/extractor/test_load_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.3.9/tests/extractor/test_transformations.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8661 2023-03-02 18:14:59.000000 thingsvision-2.3.9/tests/helper.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2023-02-22 09:56:38.000000 thingsvision-2.3.9/tests/test_features.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3719 2022-08-31 09:02:04.000000 thingsvision-2.3.9/tests/test_rest.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.790125 thingsvision-2.3.9/thingsvision/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.3.9/thingsvision/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2023-03-06 10:23:28.000000 thingsvision-2.3.9/thingsvision/_version.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.792168 thingsvision-2.3.9/thingsvision/core/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.3.9/thingsvision/core/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.793126 thingsvision-2.3.9/thingsvision/core/cka/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       21 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/core/cka/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1974 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/core/cka/base.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.795974 thingsvision-2.3.9/thingsvision/core/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      193 2023-02-15 09:26:37.000000 thingsvision-2.3.9/thingsvision/core/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8269 2023-02-17 14:03:21.000000 thingsvision-2.3.9/thingsvision/core/extraction/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    13241 2023-02-22 09:56:38.000000 thingsvision-2.3.9/thingsvision/core/extraction/extractors.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7934 2023-03-02 12:32:50.000000 thingsvision-2.3.9/thingsvision/core/extraction/helpers.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2750 2023-02-24 09:48:38.000000 thingsvision-2.3.9/thingsvision/core/extraction/tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5199 2023-02-24 09:48:38.000000 thingsvision-2.3.9/thingsvision/core/extraction/torch.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.797214 thingsvision-2.3.9/thingsvision/core/rsa/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/core/rsa/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.3.9/thingsvision/core/rsa/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.3.9/thingsvision/core/rsa/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.802365 thingsvision-2.3.9/thingsvision/custom_models/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      327 2023-03-02 18:14:59.000000 thingsvision-2.3.9/thingsvision/custom_models/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      619 2022-09-22 09:46:01.000000 thingsvision-2.3.9/thingsvision/custom_models/alexnet_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      624 2022-12-20 12:41:31.000000 thingsvision-2.3.9/thingsvision/custom_models/alexnet_salobjsub.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.804288 thingsvision-2.3.9/thingsvision/custom_models/cornet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/custom_models/cornet/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/custom_models/cornet/cornet_r.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/custom_models/cornet/cornet_rt.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/custom_models/cornet/cornet_s.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/custom_models/cornet/cornet_z.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.3.9/thingsvision/custom_models/custom.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1301 2023-03-02 18:14:59.000000 thingsvision-2.3.9/thingsvision/custom_models/harmonization.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      628 2022-09-22 09:46:01.000000 thingsvision-2.3.9/thingsvision/custom_models/inception_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      511 2022-10-26 15:18:20.000000 thingsvision-2.3.9/thingsvision/custom_models/official_clip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      982 2022-10-26 15:18:20.000000 thingsvision-2.3.9/thingsvision/custom_models/openclip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      622 2022-09-22 09:46:01.000000 thingsvision-2.3.9/thingsvision/custom_models/resnet50_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      615 2023-02-24 09:48:36.000000 thingsvision-2.3.9/thingsvision/custom_models/vgg16_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-01-18 10:11:35.000000 thingsvision-2.3.9/thingsvision/custom_models/vgg16bn_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5812 2022-12-13 13:51:38.000000 thingsvision-2.3.9/thingsvision/thingsvision.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.804632 thingsvision-2.3.9/thingsvision/utils/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.3.9/thingsvision/utils/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.805995 thingsvision-2.3.9/thingsvision/utils/data/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.3.9/thingsvision/utils/data/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.3.9/thingsvision/utils/data/data_loader.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.3.9/thingsvision/utils/data/dataset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.3.9/thingsvision/utils/data/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.806432 thingsvision-2.3.9/thingsvision/utils/imagenet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/utils/imagenet/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.807254 thingsvision-2.3.9/thingsvision/utils/storing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/utils/storing/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2023-02-22 09:56:38.000000 thingsvision-2.3.9/thingsvision/utils/storing/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.791922 thingsvision-2.3.9/thingsvision.egg-info/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    14022 2023-03-06 10:23:53.000000 thingsvision-2.3.9/thingsvision.egg-info/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2185 2023-03-06 10:23:53.000000 thingsvision-2.3.9/thingsvision.egg-info/SOURCES.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2023-03-06 10:23:53.000000 thingsvision-2.3.9/thingsvision.egg-info/dependency_links.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2023-03-06 10:23:53.000000 thingsvision-2.3.9/thingsvision.egg-info/entry_points.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      380 2023-03-06 10:23:53.000000 thingsvision-2.3.9/thingsvision.egg-info/requires.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2023-03-06 10:23:53.000000 thingsvision-2.3.9/thingsvision.egg-info/top_level.txt
```

### Comparing `thingsvision-2.3.8/LICENSE` & `thingsvision-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/PKG-INFO` & `thingsvision-2.3.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,263 +1,263 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.3.8
+Version: 2.3.9
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
-Description: <a name="readme-top"></a>
-        <div align="center">
-            <a href="https://github.com/ViCCo-Group/thingsvision/actions/workflows/tests.yml" rel="nofollow">
-                <img src="https://github.com/ViCCo-Group/thingsvision/actions/workflows/tests.yml/badge.svg" alt="Tests" />
-            </a>
-            <a href="https://github.com/ViCCo-Group/thingsvision/actions/workflows/coverage.yml" rel="nofollow">
-                <img src="https://codecov.io/gh/ViCCo-Group/thingsvision/branch/master/graph/badge.svg" alt="Code Coverage" />
-            </a>
-            <a href="https://gist.github.com/cheerfulstoic/d107229326a01ff0f333a1d3476e068d" rel="nofollow">
-                <img src="https://img.shields.io/badge/maintenance-yes-brightgreen.svg" alt="Maintenance" />
-            </a>
-            <a href="https://pypi.org/project/thingsvision/" rel="nofollow">
-                <img src="https://img.shields.io/pypi/v/thingsvision" alt="PyPI" />
-            </a>
-            <a href="https://pepy.tech/project/thingsvision">
-                <img alt="Pepy" src="https://pepy.tech/badge/thingsvision">
-            </a>
-            <a href="https://www.python.org/" rel="nofollow">
-                <img src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg" alt="Python version" />
-            </a>
-            <a href="https://github.com/ViCCo-Group/thingsvision/blob/master/LICENSE" rel="nofollow">
-                <img src="https://img.shields.io/pypi/l/thingsvision" alt="License" />
-            </a>
-            <a href="https://github.com/psf/black" rel="nofollow">
-                <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black" />
-            </a>
-            <a href="https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/pytorch.ipynb" rel="nofollow">
-                <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" />
-            </a>
-        </div>
-        <br />
-        
-        <!-- Table of Contents -->
-        # :notebook_with_decorative_cover: Table of Contents
-        
-        - [About the Project](#star2-about-the-project)
-          * [Functionality](#mechanical_arm-functionality)
-          * [Model collection](#file_cabinet-model-collection)
-        - [Getting Started](#running-getting-started)
-          * [Setting up your environment](#computer-setting-up-your-environment)
-          * [Basic usage](#mag-basic-usage)
-        - [Contributing](#wave-how-to-contribute)
-        - [License](#warning-license)
-        - [Citation](#page_with_curl-citation)
-        - [Contributions](#gem-contributions)
-        
-        
-        <!-- About the Project -->
-        ## :star2: About the Project
-        `thingsvision` is a Python package that let's you easily extract image representations from many state-of-the-art neural networks for computer vision. In a nutshell, you feed `thingsvision` with a directory of images and tell it which neural network you are interested in. `thingsvision` will then give you the  representation of the indicated neural network for each image so that you will end up with one feature vector per image. You can use these feature vectors for further analyses. We use the word `features` for short when we mean "image representation".
-        
-        :rotating_light: Note: some function calls mentioned in the [paper](https://www.frontiersin.org/articles/10.3389/fninf.2021.679838/full) have been deprecated. To use this package successfully, exclusively follow this `README` and the [documentation](https://vicco-group.github.io/thingsvision/). :rotating_light:
-        
-        <p align="right">(<a href="#readme-top">back to top</a>)</p>
-        
-        <!-- Functionality -->
-        ### :mechanical_arm: Functionality
-        With `thingsvision`, you can:
-        - extract features for any imageset from many popular networks.
-        - extract features for any imageset from your custom networks.
-        - extract features for >26,000 images from the [THINGS image database](https://osf.io/jum2f/).
-        - optionally turn off the standard center cropping performed by many networks before extracting features.
-        - extract features from HDF5 datasets directly (e.g. NSD stimuli)
-        - conduct basic Representational Similarity Analysis (RSA) after feature extraction.
-        - perform Centered Kernel Alignment (CKA) to compare image features across model-module combinations.
-        <p align="right">(<a href="#readme-top">back to top</a>)</p>
-        
-        
-        <!-- Model collection -->
-        ### :file_cabinet: Model collection
-        Neural networks come from different sources. With `thingsvision`, you can extract image representations of all models from:
-        - [torchvision](https://pytorch.org/vision/0.8/models.html)
-        - [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications)
-        - [timm](https://github.com/rwightman/pytorch-image-models)
-        - `ssl` (Self-Supervised Learning Models)
-          - `simclr-rn50`, `mocov2-rn50`, `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `pirl-rn50` (retrieved from [vissl](https://github.com/facebookresearch/vissl))
-          - `barlowtwins-rn50`, `vicreg-rn50`, `dino-vit{s/b}{8/16}`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-rn50` (retrieved from [torch.hub](https://pytorch.org/hub/))
-        - [OpenCLIP](https://github.com/mlfoundations/open_clip)
-        - both original [CLIP](https://github.com/openai/CLIP) variants (`ViT-B/32` and `RN50`)
-        - a few custom models (Alexnet, VGG-16, Resnet50, and Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/pnas.2011417118) rather than ImageNet  and one Alexnet pretrained on ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/sos.html)
-        - each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions
-        - [Harmonization](https://arxiv.org/abs/2211.04533) models from the [official repo](https://github.com/serre-lab/harmonization). The default variant is `ViT_B16`. However, the following encoders are additionally available: `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, `LeViT_small`<br> 
-        
-        <p align="right">(<a href="#readme-top">back to top</a>)</p>
-        
-        
-        <!-- Getting Started -->
-        ## :running: Getting Started
-        
-        <!-- Setting up your environment -->
-        ### :computer: Setting up your environment
-        #### Working locally.
-        First, create a new `conda environment` with Python version 3.8, 3.9, or 3.10 e.g. by using `conda`:
-        
-        ```bash
-        $ conda create -n thingsvision python=3.9
-        $ conda activate thingsvision
-        ```
-        
-        Then, activate the environment and simply install `thingsvision` via running the following `pip` command in your terminal.
-        
-        ```bash
-        $ pip install --upgrade thingsvision
-        $ pip install git+https://github.com/openai/CLIP.git
-        $ pip install git+https://github.com/serre-lab/Harmonization.git
-        ```
-        
-        #### Google Colab.
-        Alternatively, you can use Google Colab to play around with `thingsvision` by uploading your image data to Google Drive (via directory mounting).
-        You can find the jupyter notebook using `PyTorch` [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/tensorflow.ipynb).
-        <p align="right">(<a href="#readme-top">back to top</a>)</p>
-        
-        
-        <!-- Basic usage -->
-        ### :mag: Basic usage
-        
-        #### Command Line Interface (CLI)
-        
-        `thingsvision` was designed to simplify feature extraction. If you have some folder of images (e.g., `./images`) and want to extract features for each of these images without opening a Jupyter Notebook instance or writing a Python script, it's probably easiest to use our CLI. The interface includes two options,
-        
-        - `thingsvision show-model`
-        - `thingsvision extract-features`
-        
-        Example calls might look as follows:
-        
-        ```bash
-        thingsvision show-model --model-name "alexnet" --source "torchvision"
-        thingsvision extract_features --image-root "./data" --model-name "alexnet" --module-name "features.10" --batch-size 32 --device "cuda" --source "torchvision" --file-format "npy" --out-path "./features"
-        ```
-        
-        See `thingsvision show-model -h` and `thingsvision extract-features -h` for a list of all possible arguments. Note that the CLI provides just the basic extraction functionalities but is probably enough for most users that don't want to dive too deep into various models and modules. If you need more fine-grained control over the extraction itself, we recommend to use the python package directly and write your own Python script.
-        
-        #### Python commands
-        
-        To do this start by importing all the necessary components and instantiating a `thingsvision` extractor. Here we're using `AlexNet` from the `torchvision` library as the model to extract features from and also load the model to GPU for faster inference,
-        
-        ```python
-        import torch
-        from thingsvision import get_extractor
-        from thingsvision.utils.storing import save_features
-        from thingsvision.utils.data import ImageDataset, DataLoader
-        
-        model_name = 'alexnet'
-        source = 'torchvision'
-        device = 'cuda' if torch.cuda.is_available() else 'cpu'
-        
-        extractor = get_extractor(
-            model_name=model_name,
-            source=source,
-            device=device,
-            pretrained=True
-        )
-        ```
-        
-        As a next step, create both dataset and dataloader for your images. We assume that all of your images are in a single `root` directory which can contain subfolders (e.g., for individual classes). Therefore, we leverage the `ImageDataset` class. 
-        
-        ```python
-        root='path/to/root/img/directory' # (e.g., './images/)
-        batch_size = 32
-        
-        dataset = ImageDataset(
-            root=root,
-            out_path='path/to/features',
-            backend=extractor.get_backend(), # backend framework of model
-            transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set input dimensionality to whatever is required for your pretrained model
-        )
-        
-        batches = DataLoader(
-            dataset=dataset,
-            batch_size=batch_size,
-            backend=extractor.get_backend() # backend framework of model
-        )
-        ```
-        
-        Now all that is left is to extract the image features and store them to disk! Here we're extracting features from the last convolutional layer of AlexNet (`features.10`), but if you don't know which modules are available for a given model, just call `extractor.show_model()` to print all modules.
-        
-        ```python
-        module_name = 'features.10'
-        
-        features = extractor.extract_features(
-            batches=batches,
-            module_name=module_name,
-            flatten_acts=True, # flatten 2D feature maps from convolutional layer
-            output_type="ndarray", # or "tensor" (only applicable to PyTorch models)
-        )
-        
-        save_features(features, out_path='path/to/features', file_format='npy')
-        ```
-        
-        _For more examples on the many models available in `thingsvision` and explanations of additional functionality like how to optionally turn off center cropping, how to use HDF5 datasets (e.g. NSD stimuli), how to perform RSA or CKA, or how to easily extract features for the [THINGS image database](https://osf.io/jum2f/), please refer to the [Documentation](https://vicco-group.github.io/thingsvision/)._
-        <p align="right">(<a href="#readme-top">back to top</a>)</p>
-        
-        
-        <!-- Contributing -->
-        ## :wave: How to contribute
-        If you come across problems or have suggestions please submit an issue!
-        <p align="right">(<a href="#readme-top">back to top</a>)</p>
-        
-        
-        <!-- License -->
-        ## :warning: License
-        This GitHub repository is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
-        <p align="right">(<a href="#readme-top">back to top</a>)</p>
-        
-        
-        <!-- Citation -->
-        ## :page_with_curl: Citation
-        If you use this GitHub repository (or any modules associated with it), please cite our [paper](https://www.frontiersin.org/articles/10.3389/fninf.2021.679838/full) for the initial version of `thingsvision` as follows:
-        
-        ```latex
-        @article{Muttenthaler_2021,
-        	author = {Muttenthaler, Lukas and Hebart, Martin N.},
-        	title = {THINGSvision: A Python Toolbox for Streamlining the Extraction of Activations From Deep Neural Networks},
-        	journal ={Frontiers in Neuroinformatics},
-        	volume = {15},
-        	pages = {45},
-        	year = {2021},
-        	url = {https://www.frontiersin.org/article/10.3389/fninf.2021.679838},
-        	doi = {10.3389/fninf.2021.679838},
-        	issn = {1662-5196},
-        }
-        ```
-        <p align="right">(<a href="#readme-top">back to top</a>)</p>
-        
-        
-        <!-- Contributions -->
-        ## :gem: Contributions
-        This library is based on the groundwork laid by [Lukas Muttenthaler](https://lukasmut.github.io/) and [Martin N. Hebart](http://martin-hebart.de/), who are both still actively involved, but has been extended and refined into its current form with the help of our many contributors,
-        
-        - [Alex Murphy](https://github.com/Alxmrphi) (software dev.)
-        - [Florian Mahner](https://www.cbs.mpg.de/person/mahner/1483114) (software dev.)
-        - [Hannes Hansen](https://github.com/hahahannes) (software dev.)
-        - [Johannes Roth](https://jroth.space/) (software dev., design, docs)
-        - [Jonas Dippel](https://github.com/jonasd4) (software dev.)
-        - [Lukas Muttenthaler](https://lukasmut.github.io/) (software dev., design, docs, general responsibility)
-        - [Martin N. Hebart](http://martin-hebart.de/) (design)
-        - [Oliver Contier](https://olivercontier.com/) (docs)
-        - [Philipp Kaniuth](https://www.cbs.mpg.de/person/kaniuth/1483114) (design, docs)
-        - [Roman Leipe](https://github.com/RLeipe) (sofware dev., docs),
-        
-        sorted alphabetically. 
-        
-        This is a joint open-source project between the Max Planck Institute for Human Cognitive and Brain Sciences, Leipzig, and the Machine Learning Group at Technische Universtität Berlin. Correspondence and requests for contributing should be adressed to [Lukas Muttenthaler](https://lukasmut.github.io/). Feel free to contact us if you want to become a contributor or have any suggestions/feedback. For the latter, you could also just post an issue or engange in discussions. We'll try to respond as fast as we can.
-        
-        <p align="right">(<a href="#readme-top">back to top</a>)</p>
-        
-        
 Keywords: feature extraction
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<a name="readme-top"></a>
+<div align="center">
+    <a href="https://github.com/ViCCo-Group/thingsvision/actions/workflows/tests.yml" rel="nofollow">
+        <img src="https://github.com/ViCCo-Group/thingsvision/actions/workflows/tests.yml/badge.svg" alt="Tests" />
+    </a>
+    <a href="https://github.com/ViCCo-Group/thingsvision/actions/workflows/coverage.yml" rel="nofollow">
+        <img src="https://codecov.io/gh/ViCCo-Group/thingsvision/branch/master/graph/badge.svg" alt="Code Coverage" />
+    </a>
+    <a href="https://gist.github.com/cheerfulstoic/d107229326a01ff0f333a1d3476e068d" rel="nofollow">
+        <img src="https://img.shields.io/badge/maintenance-yes-brightgreen.svg" alt="Maintenance" />
+    </a>
+    <a href="https://pypi.org/project/thingsvision/" rel="nofollow">
+        <img src="https://img.shields.io/pypi/v/thingsvision" alt="PyPI" />
+    </a>
+    <a href="https://pepy.tech/project/thingsvision">
+        <img alt="Pepy" src="https://pepy.tech/badge/thingsvision">
+    </a>
+    <a href="https://www.python.org/" rel="nofollow">
+        <img src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg" alt="Python version" />
+    </a>
+    <a href="https://github.com/ViCCo-Group/thingsvision/blob/master/LICENSE" rel="nofollow">
+        <img src="https://img.shields.io/pypi/l/thingsvision" alt="License" />
+    </a>
+    <a href="https://github.com/psf/black" rel="nofollow">
+        <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black" />
+    </a>
+    <a href="https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/pytorch.ipynb" rel="nofollow">
+        <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" />
+    </a>
+</div>
+<br />
+
+<!-- Table of Contents -->
+# :notebook_with_decorative_cover: Table of Contents
+
+- [About the Project](#star2-about-the-project)
+  * [Functionality](#mechanical_arm-functionality)
+  * [Model collection](#file_cabinet-model-collection)
+- [Getting Started](#running-getting-started)
+  * [Setting up your environment](#computer-setting-up-your-environment)
+  * [Basic usage](#mag-basic-usage)
+- [Contributing](#wave-how-to-contribute)
+- [License](#warning-license)
+- [Citation](#page_with_curl-citation)
+- [Contributions](#gem-contributions)
+
+
+<!-- About the Project -->
+## :star2: About the Project
+`thingsvision` is a Python package that let's you easily extract image representations from many state-of-the-art neural networks for computer vision. In a nutshell, you feed `thingsvision` with a directory of images and tell it which neural network you are interested in. `thingsvision` will then give you the  representation of the indicated neural network for each image so that you will end up with one feature vector per image. You can use these feature vectors for further analyses. We use the word `features` for short when we mean "image representation".
+
+:rotating_light: Note: some function calls mentioned in the [paper](https://www.frontiersin.org/articles/10.3389/fninf.2021.679838/full) have been deprecated. To use this package successfully, exclusively follow this `README` and the [documentation](https://vicco-group.github.io/thingsvision/). :rotating_light:
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+<!-- Functionality -->
+### :mechanical_arm: Functionality
+With `thingsvision`, you can:
+- extract features for any imageset from many popular networks.
+- extract features for any imageset from your custom networks.
+- extract features for >26,000 images from the [THINGS image database](https://osf.io/jum2f/).
+- optionally turn off the standard center cropping performed by many networks before extracting features.
+- extract features from HDF5 datasets directly (e.g. NSD stimuli)
+- conduct basic Representational Similarity Analysis (RSA) after feature extraction.
+- perform Centered Kernel Alignment (CKA) to compare image features across model-module combinations.
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- Model collection -->
+### :file_cabinet: Model collection
+Neural networks come from different sources. With `thingsvision`, you can extract image representations of all models from:
+- [torchvision](https://pytorch.org/vision/0.8/models.html)
+- [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications)
+- [timm](https://github.com/rwightman/pytorch-image-models)
+- `ssl` (Self-Supervised Learning Models)
+  - `simclr-rn50`, `mocov2-rn50`, `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `pirl-rn50` (retrieved from [vissl](https://github.com/facebookresearch/vissl))
+  - `barlowtwins-rn50`, `vicreg-rn50`, `dino-vit{s/b}{8/16}`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-rn50` (retrieved from [torch.hub](https://pytorch.org/hub/))
+- [OpenCLIP](https://github.com/mlfoundations/open_clip)
+- both original [CLIP](https://github.com/openai/CLIP) variants (`ViT-B/32` and `RN50`)
+- a few custom models (Alexnet, VGG-16, Resnet50, and Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/pnas.2011417118) rather than ImageNet  and one Alexnet pretrained on ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/sos.html)
+- each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions
+- [Harmonization](https://arxiv.org/abs/2211.04533) models from the [official repo](https://github.com/serre-lab/harmonization). The default variant is `ViT_B16`. However, the following encoders are additionally available: `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, `LeViT_small`<br> 
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- Getting Started -->
+## :running: Getting Started
+
+<!-- Setting up your environment -->
+### :computer: Setting up your environment
+#### Working locally.
+First, create a new `conda environment` with Python version 3.8, 3.9, or 3.10 e.g. by using `conda`:
+
+```bash
+$ conda create -n thingsvision python=3.9
+$ conda activate thingsvision
+```
+
+Then, activate the environment and simply install `thingsvision` via running the following `pip` command in your terminal.
+
+```bash
+$ pip install --upgrade thingsvision
+$ pip install git+https://github.com/openai/CLIP.git
+$ pip install git+https://github.com/serre-lab/Harmonization.git
+```
+
+#### Google Colab.
+Alternatively, you can use Google Colab to play around with `thingsvision` by uploading your image data to Google Drive (via directory mounting).
+You can find the jupyter notebook using `PyTorch` [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/tensorflow.ipynb).
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- Basic usage -->
+### :mag: Basic usage
+
+#### Command Line Interface (CLI)
+
+`thingsvision` was designed to simplify feature extraction. If you have some folder of images (e.g., `./images`) and want to extract features for each of these images without opening a Jupyter Notebook instance or writing a Python script, it's probably easiest to use our CLI. The interface includes two options,
+
+- `thingsvision show-model`
+- `thingsvision extract-features`
+
+Example calls might look as follows:
+
+```bash
+thingsvision show-model --model-name "alexnet" --source "torchvision"
+thingsvision extract_features --image-root "./data" --model-name "alexnet" --module-name "features.10" --batch-size 32 --device "cuda" --source "torchvision" --file-format "npy" --out-path "./features"
+```
+
+See `thingsvision show-model -h` and `thingsvision extract-features -h` for a list of all possible arguments. Note that the CLI provides just the basic extraction functionalities but is probably enough for most users that don't want to dive too deep into various models and modules. If you need more fine-grained control over the extraction itself, we recommend to use the python package directly and write your own Python script.
+
+#### Python commands
+
+To do this start by importing all the necessary components and instantiating a `thingsvision` extractor. Here we're using `AlexNet` from the `torchvision` library as the model to extract features from and also load the model to GPU for faster inference,
+
+```python
+import torch
+from thingsvision import get_extractor
+from thingsvision.utils.storing import save_features
+from thingsvision.utils.data import ImageDataset, DataLoader
+
+model_name = 'alexnet'
+source = 'torchvision'
+device = 'cuda' if torch.cuda.is_available() else 'cpu'
+
+extractor = get_extractor(
+    model_name=model_name,
+    source=source,
+    device=device,
+    pretrained=True
+)
+```
+
+As a next step, create both dataset and dataloader for your images. We assume that all of your images are in a single `root` directory which can contain subfolders (e.g., for individual classes). Therefore, we leverage the `ImageDataset` class. 
+
+```python
+root='path/to/root/img/directory' # (e.g., './images/)
+batch_size = 32
+
+dataset = ImageDataset(
+    root=root,
+    out_path='path/to/features',
+    backend=extractor.get_backend(), # backend framework of model
+    transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set input dimensionality to whatever is required for your pretrained model
+)
+
+batches = DataLoader(
+    dataset=dataset,
+    batch_size=batch_size,
+    backend=extractor.get_backend() # backend framework of model
+)
+```
+
+Now all that is left is to extract the image features and store them to disk! Here we're extracting features from the last convolutional layer of AlexNet (`features.10`), but if you don't know which modules are available for a given model, just call `extractor.show_model()` to print all modules.
+
+```python
+module_name = 'features.10'
+
+features = extractor.extract_features(
+    batches=batches,
+    module_name=module_name,
+    flatten_acts=True, # flatten 2D feature maps from convolutional layer
+    output_type="ndarray", # or "tensor" (only applicable to PyTorch models)
+)
+
+save_features(features, out_path='path/to/features', file_format='npy')
+```
+
+_For more examples on the many models available in `thingsvision` and explanations of additional functionality like how to optionally turn off center cropping, how to use HDF5 datasets (e.g. NSD stimuli), how to perform RSA or CKA, or how to easily extract features for the [THINGS image database](https://osf.io/jum2f/), please refer to the [Documentation](https://vicco-group.github.io/thingsvision/)._
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- Contributing -->
+## :wave: How to contribute
+If you come across problems or have suggestions please submit an issue!
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- License -->
+## :warning: License
+This GitHub repository is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- Citation -->
+## :page_with_curl: Citation
+If you use this GitHub repository (or any modules associated with it), please cite our [paper](https://www.frontiersin.org/articles/10.3389/fninf.2021.679838/full) for the initial version of `thingsvision` as follows:
+
+```latex
+@article{Muttenthaler_2021,
+	author = {Muttenthaler, Lukas and Hebart, Martin N.},
+	title = {THINGSvision: A Python Toolbox for Streamlining the Extraction of Activations From Deep Neural Networks},
+	journal ={Frontiers in Neuroinformatics},
+	volume = {15},
+	pages = {45},
+	year = {2021},
+	url = {https://www.frontiersin.org/article/10.3389/fninf.2021.679838},
+	doi = {10.3389/fninf.2021.679838},
+	issn = {1662-5196},
+}
+```
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- Contributions -->
+## :gem: Contributions
+This library is based on the groundwork laid by [Lukas Muttenthaler](https://lukasmut.github.io/) and [Martin N. Hebart](http://martin-hebart.de/), who are both still actively involved, but has been extended and refined into its current form with the help of our many contributors,
+
+- [Alex Murphy](https://github.com/Alxmrphi) (software dev.)
+- [Florian Mahner](https://www.cbs.mpg.de/person/mahner/1483114) (software dev.)
+- [Hannes Hansen](https://github.com/hahahannes) (software dev.)
+- [Johannes Roth](https://jroth.space/) (software dev., design, docs)
+- [Jonas Dippel](https://github.com/jonasd4) (software dev.)
+- [Lukas Muttenthaler](https://lukasmut.github.io/) (software dev., design, docs, general responsibility)
+- [Martin N. Hebart](http://martin-hebart.de/) (design)
+- [Oliver Contier](https://olivercontier.com/) (docs)
+- [Philipp Kaniuth](https://www.cbs.mpg.de/person/kaniuth/1483114) (design, docs)
+- [Roman Leipe](https://github.com/RLeipe) (sofware dev., docs),
+
+sorted alphabetically. 
+
+This is a joint open-source project between the Max Planck Institute for Human Cognitive and Brain Sciences, Leipzig, and the Machine Learning Group at Technische Universtität Berlin. Correspondence and requests for contributing should be adressed to [Lukas Muttenthaler](https://lukasmut.github.io/). Feel free to contact us if you want to become a contributor or have any suggestions/feedback. For the latter, you could also just post an issue or engange in discussions. We'll try to respond as fast as we can.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
```

#### html2text {}

```diff
@@ -1,12 +1,15 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.3.8 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.3.9 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
-Description:
+Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
+Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
+MIT License Classifier: Operating System :: OS Independent Requires-Python:
+>=3.8 Description-Content-Type: text/markdown License-File: LICENSE
 [Tests] [Code_Coverage] [Maintenance] [PyPI] [Pepy] [Python_version] [License]
                       [Code_style:_black] [Open_In_Colab]
 
  # :notebook_with_decorative_cover: Table of Contents - [About the Project]
 (#star2-about-the-project) * [Functionality](#mechanical_arm-functionality) *
 [Model collection](#file_cabinet-model-collection) - [Getting Started]
 (#running-getting-started) * [Setting up your environment](#computer-setting-
@@ -157,11 +160,7 @@
 Sciences, Leipzig, and the Machine Learning Group at Technische UniverstitÃ¤t
 Berlin. Correspondence and requests for contributing should be adressed to
 [Lukas Muttenthaler](https://lukasmut.github.io/). Feel free to contact us if
 you want to become a contributor or have any suggestions/feedback. For the
 latter, you could also just post an issue or engange in discussions. We'll try
 to respond as fast as we can.
                                                                   (back_to_top)
-Keywords: feature extraction Platform: UNKNOWN Classifier: Programming Language
-:: Python :: 3.8 Classifier: Natural Language :: English Classifier: License ::
-OSI Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8 Description-Content-Type: text/markdown
```

### Comparing `thingsvision-2.3.8/README.md` & `thingsvision-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/setup.py` & `thingsvision-2.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "tensorflow-macos==2.9.* ; sys_platform == 'darwin' and platform_machine == 'arm64'",
     "timm==0.6.*",
     "torch>=1.13.1",
     "torchvision==0.14.*",
     "torchtyping",
     "tqdm",
     "CLIP",
-    "Harmonization",
+    # "Harmonization",
     # 'CLIP @ git+ssh://git@github.com/openai/CLIP@v1.0#egg=CLIP'
 ]
 
 setuptools.setup(
     name="thingsvision",
     version=__version__,
     author="Lukas Muttenthaler",
@@ -50,10 +50,10 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={"console_scripts": ["thingsvision = thingsvision.thingsvision:main"]},
     python_requires=">=3.8",
     dependency_links=[
         "git+https://github.com/openai/CLIP.git",
-        "git+https://github.com/serre-lab/Harmonization.git",
+        # "git+https://github.com/serre-lab/Harmonization.git",
     ],
 )
```

### Comparing `thingsvision-2.3.8/tests/extractor/extraction/test_custom_model.py` & `thingsvision-2.3.9/tests/extractor/extraction/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/tests/extractor/extraction/test_model_extractor.py` & `thingsvision-2.3.9/tests/extractor/extraction/test_model_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/tests/extractor/extraction/test_pretrained_model.py` & `thingsvision-2.3.9/tests/extractor/extraction/test_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/tests/extractor/extraction/test_torch_vs_tensorflow.py` & `thingsvision-2.3.9/tests/extractor/extraction/test_torch_vs_tensorflow.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/tests/extractor/test_load_extractor.py` & `thingsvision-2.3.9/tests/extractor/test_load_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/tests/extractor/test_transformations.py` & `thingsvision-2.3.9/tests/extractor/test_transformations.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/tests/helper.py` & `thingsvision-2.3.9/tests/helper.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/tests/test_features.py` & `thingsvision-2.3.9/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/tests/test_rest.py` & `thingsvision-2.3.9/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/core/cka/base.py` & `thingsvision-2.3.9/thingsvision/core/cka/base.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/core/extraction/base.py` & `thingsvision-2.3.9/thingsvision/core/extraction/base.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/core/extraction/extractors.py` & `thingsvision-2.3.9/thingsvision/core/extraction/extractors.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/core/extraction/helpers.py` & `thingsvision-2.3.9/thingsvision/core/extraction/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/core/extraction/tensorflow.py` & `thingsvision-2.3.9/thingsvision/core/extraction/tensorflow.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/core/extraction/torch.py` & `thingsvision-2.3.9/thingsvision/core/extraction/torch.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/core/rsa/helpers.py` & `thingsvision-2.3.9/thingsvision/core/rsa/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/custom_models/alexnet_ecoset.py` & `thingsvision-2.3.9/thingsvision/custom_models/alexnet_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/custom_models/alexnet_salobjsub.py` & `thingsvision-2.3.9/thingsvision/custom_models/alexnet_salobjsub.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/custom_models/cornet/__init__.py` & `thingsvision-2.3.9/thingsvision/custom_models/cornet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/custom_models/cornet/cornet_r.py` & `thingsvision-2.3.9/thingsvision/custom_models/cornet/cornet_r.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/custom_models/cornet/cornet_rt.py` & `thingsvision-2.3.9/thingsvision/custom_models/cornet/cornet_rt.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/custom_models/cornet/cornet_s.py` & `thingsvision-2.3.9/thingsvision/custom_models/cornet/cornet_s.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/custom_models/cornet/cornet_z.py` & `thingsvision-2.3.9/thingsvision/custom_models/cornet/cornet_z.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/custom_models/harmonization.py` & `thingsvision-2.3.9/thingsvision/custom_models/harmonization.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/custom_models/inception_ecoset.py` & `thingsvision-2.3.9/thingsvision/custom_models/inception_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/custom_models/openclip.py` & `thingsvision-2.3.9/thingsvision/custom_models/openclip.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/custom_models/resnet50_ecoset.py` & `thingsvision-2.3.9/thingsvision/custom_models/resnet50_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/custom_models/vgg16_ecoset.py` & `thingsvision-2.3.9/thingsvision/custom_models/vgg16_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/custom_models/vgg16bn_ecoset.py` & `thingsvision-2.3.9/thingsvision/custom_models/vgg16bn_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/thingsvision.py` & `thingsvision-2.3.9/thingsvision/thingsvision.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/utils/data/__init__.py` & `thingsvision-2.3.9/thingsvision/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/utils/data/data_loader.py` & `thingsvision-2.3.9/thingsvision/utils/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/utils/data/dataset.py` & `thingsvision-2.3.9/thingsvision/utils/data/dataset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/utils/data/helpers.py` & `thingsvision-2.3.9/thingsvision/utils/data/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/utils/imagenet/__init__.py` & `thingsvision-2.3.9/thingsvision/utils/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision/utils/storing/helpers.py` & `thingsvision-2.3.9/thingsvision/utils/storing/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.8/thingsvision.egg-info/PKG-INFO` & `thingsvision-2.3.9/thingsvision.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,263 +1,263 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.3.8
+Version: 2.3.9
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
-Description: <a name="readme-top"></a>
-        <div align="center">
-            <a href="https://github.com/ViCCo-Group/thingsvision/actions/workflows/tests.yml" rel="nofollow">
-                <img src="https://github.com/ViCCo-Group/thingsvision/actions/workflows/tests.yml/badge.svg" alt="Tests" />
-            </a>
-            <a href="https://github.com/ViCCo-Group/thingsvision/actions/workflows/coverage.yml" rel="nofollow">
-                <img src="https://codecov.io/gh/ViCCo-Group/thingsvision/branch/master/graph/badge.svg" alt="Code Coverage" />
-            </a>
-            <a href="https://gist.github.com/cheerfulstoic/d107229326a01ff0f333a1d3476e068d" rel="nofollow">
-                <img src="https://img.shields.io/badge/maintenance-yes-brightgreen.svg" alt="Maintenance" />
-            </a>
-            <a href="https://pypi.org/project/thingsvision/" rel="nofollow">
-                <img src="https://img.shields.io/pypi/v/thingsvision" alt="PyPI" />
-            </a>
-            <a href="https://pepy.tech/project/thingsvision">
-                <img alt="Pepy" src="https://pepy.tech/badge/thingsvision">
-            </a>
-            <a href="https://www.python.org/" rel="nofollow">
-                <img src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg" alt="Python version" />
-            </a>
-            <a href="https://github.com/ViCCo-Group/thingsvision/blob/master/LICENSE" rel="nofollow">
-                <img src="https://img.shields.io/pypi/l/thingsvision" alt="License" />
-            </a>
-            <a href="https://github.com/psf/black" rel="nofollow">
-                <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black" />
-            </a>
-            <a href="https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/pytorch.ipynb" rel="nofollow">
-                <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" />
-            </a>
-        </div>
-        <br />
-        
-        <!-- Table of Contents -->
-        # :notebook_with_decorative_cover: Table of Contents
-        
-        - [About the Project](#star2-about-the-project)
-          * [Functionality](#mechanical_arm-functionality)
-          * [Model collection](#file_cabinet-model-collection)
-        - [Getting Started](#running-getting-started)
-          * [Setting up your environment](#computer-setting-up-your-environment)
-          * [Basic usage](#mag-basic-usage)
-        - [Contributing](#wave-how-to-contribute)
-        - [License](#warning-license)
-        - [Citation](#page_with_curl-citation)
-        - [Contributions](#gem-contributions)
-        
-        
-        <!-- About the Project -->
-        ## :star2: About the Project
-        `thingsvision` is a Python package that let's you easily extract image representations from many state-of-the-art neural networks for computer vision. In a nutshell, you feed `thingsvision` with a directory of images and tell it which neural network you are interested in. `thingsvision` will then give you the  representation of the indicated neural network for each image so that you will end up with one feature vector per image. You can use these feature vectors for further analyses. We use the word `features` for short when we mean "image representation".
-        
-        :rotating_light: Note: some function calls mentioned in the [paper](https://www.frontiersin.org/articles/10.3389/fninf.2021.679838/full) have been deprecated. To use this package successfully, exclusively follow this `README` and the [documentation](https://vicco-group.github.io/thingsvision/). :rotating_light:
-        
-        <p align="right">(<a href="#readme-top">back to top</a>)</p>
-        
-        <!-- Functionality -->
-        ### :mechanical_arm: Functionality
-        With `thingsvision`, you can:
-        - extract features for any imageset from many popular networks.
-        - extract features for any imageset from your custom networks.
-        - extract features for >26,000 images from the [THINGS image database](https://osf.io/jum2f/).
-        - optionally turn off the standard center cropping performed by many networks before extracting features.
-        - extract features from HDF5 datasets directly (e.g. NSD stimuli)
-        - conduct basic Representational Similarity Analysis (RSA) after feature extraction.
-        - perform Centered Kernel Alignment (CKA) to compare image features across model-module combinations.
-        <p align="right">(<a href="#readme-top">back to top</a>)</p>
-        
-        
-        <!-- Model collection -->
-        ### :file_cabinet: Model collection
-        Neural networks come from different sources. With `thingsvision`, you can extract image representations of all models from:
-        - [torchvision](https://pytorch.org/vision/0.8/models.html)
-        - [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications)
-        - [timm](https://github.com/rwightman/pytorch-image-models)
-        - `ssl` (Self-Supervised Learning Models)
-          - `simclr-rn50`, `mocov2-rn50`, `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `pirl-rn50` (retrieved from [vissl](https://github.com/facebookresearch/vissl))
-          - `barlowtwins-rn50`, `vicreg-rn50`, `dino-vit{s/b}{8/16}`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-rn50` (retrieved from [torch.hub](https://pytorch.org/hub/))
-        - [OpenCLIP](https://github.com/mlfoundations/open_clip)
-        - both original [CLIP](https://github.com/openai/CLIP) variants (`ViT-B/32` and `RN50`)
-        - a few custom models (Alexnet, VGG-16, Resnet50, and Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/pnas.2011417118) rather than ImageNet  and one Alexnet pretrained on ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/sos.html)
-        - each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions
-        - [Harmonization](https://arxiv.org/abs/2211.04533) models from the [official repo](https://github.com/serre-lab/harmonization). The default variant is `ViT_B16`. However, the following encoders are additionally available: `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, `LeViT_small`<br> 
-        
-        <p align="right">(<a href="#readme-top">back to top</a>)</p>
-        
-        
-        <!-- Getting Started -->
-        ## :running: Getting Started
-        
-        <!-- Setting up your environment -->
-        ### :computer: Setting up your environment
-        #### Working locally.
-        First, create a new `conda environment` with Python version 3.8, 3.9, or 3.10 e.g. by using `conda`:
-        
-        ```bash
-        $ conda create -n thingsvision python=3.9
-        $ conda activate thingsvision
-        ```
-        
-        Then, activate the environment and simply install `thingsvision` via running the following `pip` command in your terminal.
-        
-        ```bash
-        $ pip install --upgrade thingsvision
-        $ pip install git+https://github.com/openai/CLIP.git
-        $ pip install git+https://github.com/serre-lab/Harmonization.git
-        ```
-        
-        #### Google Colab.
-        Alternatively, you can use Google Colab to play around with `thingsvision` by uploading your image data to Google Drive (via directory mounting).
-        You can find the jupyter notebook using `PyTorch` [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/tensorflow.ipynb).
-        <p align="right">(<a href="#readme-top">back to top</a>)</p>
-        
-        
-        <!-- Basic usage -->
-        ### :mag: Basic usage
-        
-        #### Command Line Interface (CLI)
-        
-        `thingsvision` was designed to simplify feature extraction. If you have some folder of images (e.g., `./images`) and want to extract features for each of these images without opening a Jupyter Notebook instance or writing a Python script, it's probably easiest to use our CLI. The interface includes two options,
-        
-        - `thingsvision show-model`
-        - `thingsvision extract-features`
-        
-        Example calls might look as follows:
-        
-        ```bash
-        thingsvision show-model --model-name "alexnet" --source "torchvision"
-        thingsvision extract_features --image-root "./data" --model-name "alexnet" --module-name "features.10" --batch-size 32 --device "cuda" --source "torchvision" --file-format "npy" --out-path "./features"
-        ```
-        
-        See `thingsvision show-model -h` and `thingsvision extract-features -h` for a list of all possible arguments. Note that the CLI provides just the basic extraction functionalities but is probably enough for most users that don't want to dive too deep into various models and modules. If you need more fine-grained control over the extraction itself, we recommend to use the python package directly and write your own Python script.
-        
-        #### Python commands
-        
-        To do this start by importing all the necessary components and instantiating a `thingsvision` extractor. Here we're using `AlexNet` from the `torchvision` library as the model to extract features from and also load the model to GPU for faster inference,
-        
-        ```python
-        import torch
-        from thingsvision import get_extractor
-        from thingsvision.utils.storing import save_features
-        from thingsvision.utils.data import ImageDataset, DataLoader
-        
-        model_name = 'alexnet'
-        source = 'torchvision'
-        device = 'cuda' if torch.cuda.is_available() else 'cpu'
-        
-        extractor = get_extractor(
-            model_name=model_name,
-            source=source,
-            device=device,
-            pretrained=True
-        )
-        ```
-        
-        As a next step, create both dataset and dataloader for your images. We assume that all of your images are in a single `root` directory which can contain subfolders (e.g., for individual classes). Therefore, we leverage the `ImageDataset` class. 
-        
-        ```python
-        root='path/to/root/img/directory' # (e.g., './images/)
-        batch_size = 32
-        
-        dataset = ImageDataset(
-            root=root,
-            out_path='path/to/features',
-            backend=extractor.get_backend(), # backend framework of model
-            transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set input dimensionality to whatever is required for your pretrained model
-        )
-        
-        batches = DataLoader(
-            dataset=dataset,
-            batch_size=batch_size,
-            backend=extractor.get_backend() # backend framework of model
-        )
-        ```
-        
-        Now all that is left is to extract the image features and store them to disk! Here we're extracting features from the last convolutional layer of AlexNet (`features.10`), but if you don't know which modules are available for a given model, just call `extractor.show_model()` to print all modules.
-        
-        ```python
-        module_name = 'features.10'
-        
-        features = extractor.extract_features(
-            batches=batches,
-            module_name=module_name,
-            flatten_acts=True, # flatten 2D feature maps from convolutional layer
-            output_type="ndarray", # or "tensor" (only applicable to PyTorch models)
-        )
-        
-        save_features(features, out_path='path/to/features', file_format='npy')
-        ```
-        
-        _For more examples on the many models available in `thingsvision` and explanations of additional functionality like how to optionally turn off center cropping, how to use HDF5 datasets (e.g. NSD stimuli), how to perform RSA or CKA, or how to easily extract features for the [THINGS image database](https://osf.io/jum2f/), please refer to the [Documentation](https://vicco-group.github.io/thingsvision/)._
-        <p align="right">(<a href="#readme-top">back to top</a>)</p>
-        
-        
-        <!-- Contributing -->
-        ## :wave: How to contribute
-        If you come across problems or have suggestions please submit an issue!
-        <p align="right">(<a href="#readme-top">back to top</a>)</p>
-        
-        
-        <!-- License -->
-        ## :warning: License
-        This GitHub repository is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
-        <p align="right">(<a href="#readme-top">back to top</a>)</p>
-        
-        
-        <!-- Citation -->
-        ## :page_with_curl: Citation
-        If you use this GitHub repository (or any modules associated with it), please cite our [paper](https://www.frontiersin.org/articles/10.3389/fninf.2021.679838/full) for the initial version of `thingsvision` as follows:
-        
-        ```latex
-        @article{Muttenthaler_2021,
-        	author = {Muttenthaler, Lukas and Hebart, Martin N.},
-        	title = {THINGSvision: A Python Toolbox for Streamlining the Extraction of Activations From Deep Neural Networks},
-        	journal ={Frontiers in Neuroinformatics},
-        	volume = {15},
-        	pages = {45},
-        	year = {2021},
-        	url = {https://www.frontiersin.org/article/10.3389/fninf.2021.679838},
-        	doi = {10.3389/fninf.2021.679838},
-        	issn = {1662-5196},
-        }
-        ```
-        <p align="right">(<a href="#readme-top">back to top</a>)</p>
-        
-        
-        <!-- Contributions -->
-        ## :gem: Contributions
-        This library is based on the groundwork laid by [Lukas Muttenthaler](https://lukasmut.github.io/) and [Martin N. Hebart](http://martin-hebart.de/), who are both still actively involved, but has been extended and refined into its current form with the help of our many contributors,
-        
-        - [Alex Murphy](https://github.com/Alxmrphi) (software dev.)
-        - [Florian Mahner](https://www.cbs.mpg.de/person/mahner/1483114) (software dev.)
-        - [Hannes Hansen](https://github.com/hahahannes) (software dev.)
-        - [Johannes Roth](https://jroth.space/) (software dev., design, docs)
-        - [Jonas Dippel](https://github.com/jonasd4) (software dev.)
-        - [Lukas Muttenthaler](https://lukasmut.github.io/) (software dev., design, docs, general responsibility)
-        - [Martin N. Hebart](http://martin-hebart.de/) (design)
-        - [Oliver Contier](https://olivercontier.com/) (docs)
-        - [Philipp Kaniuth](https://www.cbs.mpg.de/person/kaniuth/1483114) (design, docs)
-        - [Roman Leipe](https://github.com/RLeipe) (sofware dev., docs),
-        
-        sorted alphabetically. 
-        
-        This is a joint open-source project between the Max Planck Institute for Human Cognitive and Brain Sciences, Leipzig, and the Machine Learning Group at Technische Universtität Berlin. Correspondence and requests for contributing should be adressed to [Lukas Muttenthaler](https://lukasmut.github.io/). Feel free to contact us if you want to become a contributor or have any suggestions/feedback. For the latter, you could also just post an issue or engange in discussions. We'll try to respond as fast as we can.
-        
-        <p align="right">(<a href="#readme-top">back to top</a>)</p>
-        
-        
 Keywords: feature extraction
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<a name="readme-top"></a>
+<div align="center">
+    <a href="https://github.com/ViCCo-Group/thingsvision/actions/workflows/tests.yml" rel="nofollow">
+        <img src="https://github.com/ViCCo-Group/thingsvision/actions/workflows/tests.yml/badge.svg" alt="Tests" />
+    </a>
+    <a href="https://github.com/ViCCo-Group/thingsvision/actions/workflows/coverage.yml" rel="nofollow">
+        <img src="https://codecov.io/gh/ViCCo-Group/thingsvision/branch/master/graph/badge.svg" alt="Code Coverage" />
+    </a>
+    <a href="https://gist.github.com/cheerfulstoic/d107229326a01ff0f333a1d3476e068d" rel="nofollow">
+        <img src="https://img.shields.io/badge/maintenance-yes-brightgreen.svg" alt="Maintenance" />
+    </a>
+    <a href="https://pypi.org/project/thingsvision/" rel="nofollow">
+        <img src="https://img.shields.io/pypi/v/thingsvision" alt="PyPI" />
+    </a>
+    <a href="https://pepy.tech/project/thingsvision">
+        <img alt="Pepy" src="https://pepy.tech/badge/thingsvision">
+    </a>
+    <a href="https://www.python.org/" rel="nofollow">
+        <img src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg" alt="Python version" />
+    </a>
+    <a href="https://github.com/ViCCo-Group/thingsvision/blob/master/LICENSE" rel="nofollow">
+        <img src="https://img.shields.io/pypi/l/thingsvision" alt="License" />
+    </a>
+    <a href="https://github.com/psf/black" rel="nofollow">
+        <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black" />
+    </a>
+    <a href="https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/pytorch.ipynb" rel="nofollow">
+        <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" />
+    </a>
+</div>
+<br />
+
+<!-- Table of Contents -->
+# :notebook_with_decorative_cover: Table of Contents
+
+- [About the Project](#star2-about-the-project)
+  * [Functionality](#mechanical_arm-functionality)
+  * [Model collection](#file_cabinet-model-collection)
+- [Getting Started](#running-getting-started)
+  * [Setting up your environment](#computer-setting-up-your-environment)
+  * [Basic usage](#mag-basic-usage)
+- [Contributing](#wave-how-to-contribute)
+- [License](#warning-license)
+- [Citation](#page_with_curl-citation)
+- [Contributions](#gem-contributions)
+
+
+<!-- About the Project -->
+## :star2: About the Project
+`thingsvision` is a Python package that let's you easily extract image representations from many state-of-the-art neural networks for computer vision. In a nutshell, you feed `thingsvision` with a directory of images and tell it which neural network you are interested in. `thingsvision` will then give you the  representation of the indicated neural network for each image so that you will end up with one feature vector per image. You can use these feature vectors for further analyses. We use the word `features` for short when we mean "image representation".
+
+:rotating_light: Note: some function calls mentioned in the [paper](https://www.frontiersin.org/articles/10.3389/fninf.2021.679838/full) have been deprecated. To use this package successfully, exclusively follow this `README` and the [documentation](https://vicco-group.github.io/thingsvision/). :rotating_light:
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+<!-- Functionality -->
+### :mechanical_arm: Functionality
+With `thingsvision`, you can:
+- extract features for any imageset from many popular networks.
+- extract features for any imageset from your custom networks.
+- extract features for >26,000 images from the [THINGS image database](https://osf.io/jum2f/).
+- optionally turn off the standard center cropping performed by many networks before extracting features.
+- extract features from HDF5 datasets directly (e.g. NSD stimuli)
+- conduct basic Representational Similarity Analysis (RSA) after feature extraction.
+- perform Centered Kernel Alignment (CKA) to compare image features across model-module combinations.
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- Model collection -->
+### :file_cabinet: Model collection
+Neural networks come from different sources. With `thingsvision`, you can extract image representations of all models from:
+- [torchvision](https://pytorch.org/vision/0.8/models.html)
+- [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications)
+- [timm](https://github.com/rwightman/pytorch-image-models)
+- `ssl` (Self-Supervised Learning Models)
+  - `simclr-rn50`, `mocov2-rn50`, `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `pirl-rn50` (retrieved from [vissl](https://github.com/facebookresearch/vissl))
+  - `barlowtwins-rn50`, `vicreg-rn50`, `dino-vit{s/b}{8/16}`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-rn50` (retrieved from [torch.hub](https://pytorch.org/hub/))
+- [OpenCLIP](https://github.com/mlfoundations/open_clip)
+- both original [CLIP](https://github.com/openai/CLIP) variants (`ViT-B/32` and `RN50`)
+- a few custom models (Alexnet, VGG-16, Resnet50, and Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/pnas.2011417118) rather than ImageNet  and one Alexnet pretrained on ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/sos.html)
+- each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions
+- [Harmonization](https://arxiv.org/abs/2211.04533) models from the [official repo](https://github.com/serre-lab/harmonization). The default variant is `ViT_B16`. However, the following encoders are additionally available: `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, `LeViT_small`<br> 
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- Getting Started -->
+## :running: Getting Started
+
+<!-- Setting up your environment -->
+### :computer: Setting up your environment
+#### Working locally.
+First, create a new `conda environment` with Python version 3.8, 3.9, or 3.10 e.g. by using `conda`:
+
+```bash
+$ conda create -n thingsvision python=3.9
+$ conda activate thingsvision
+```
+
+Then, activate the environment and simply install `thingsvision` via running the following `pip` command in your terminal.
+
+```bash
+$ pip install --upgrade thingsvision
+$ pip install git+https://github.com/openai/CLIP.git
+$ pip install git+https://github.com/serre-lab/Harmonization.git
+```
+
+#### Google Colab.
+Alternatively, you can use Google Colab to play around with `thingsvision` by uploading your image data to Google Drive (via directory mounting).
+You can find the jupyter notebook using `PyTorch` [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/tensorflow.ipynb).
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- Basic usage -->
+### :mag: Basic usage
+
+#### Command Line Interface (CLI)
+
+`thingsvision` was designed to simplify feature extraction. If you have some folder of images (e.g., `./images`) and want to extract features for each of these images without opening a Jupyter Notebook instance or writing a Python script, it's probably easiest to use our CLI. The interface includes two options,
+
+- `thingsvision show-model`
+- `thingsvision extract-features`
+
+Example calls might look as follows:
+
+```bash
+thingsvision show-model --model-name "alexnet" --source "torchvision"
+thingsvision extract_features --image-root "./data" --model-name "alexnet" --module-name "features.10" --batch-size 32 --device "cuda" --source "torchvision" --file-format "npy" --out-path "./features"
+```
+
+See `thingsvision show-model -h` and `thingsvision extract-features -h` for a list of all possible arguments. Note that the CLI provides just the basic extraction functionalities but is probably enough for most users that don't want to dive too deep into various models and modules. If you need more fine-grained control over the extraction itself, we recommend to use the python package directly and write your own Python script.
+
+#### Python commands
+
+To do this start by importing all the necessary components and instantiating a `thingsvision` extractor. Here we're using `AlexNet` from the `torchvision` library as the model to extract features from and also load the model to GPU for faster inference,
+
+```python
+import torch
+from thingsvision import get_extractor
+from thingsvision.utils.storing import save_features
+from thingsvision.utils.data import ImageDataset, DataLoader
+
+model_name = 'alexnet'
+source = 'torchvision'
+device = 'cuda' if torch.cuda.is_available() else 'cpu'
+
+extractor = get_extractor(
+    model_name=model_name,
+    source=source,
+    device=device,
+    pretrained=True
+)
+```
+
+As a next step, create both dataset and dataloader for your images. We assume that all of your images are in a single `root` directory which can contain subfolders (e.g., for individual classes). Therefore, we leverage the `ImageDataset` class. 
+
+```python
+root='path/to/root/img/directory' # (e.g., './images/)
+batch_size = 32
+
+dataset = ImageDataset(
+    root=root,
+    out_path='path/to/features',
+    backend=extractor.get_backend(), # backend framework of model
+    transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set input dimensionality to whatever is required for your pretrained model
+)
+
+batches = DataLoader(
+    dataset=dataset,
+    batch_size=batch_size,
+    backend=extractor.get_backend() # backend framework of model
+)
+```
+
+Now all that is left is to extract the image features and store them to disk! Here we're extracting features from the last convolutional layer of AlexNet (`features.10`), but if you don't know which modules are available for a given model, just call `extractor.show_model()` to print all modules.
+
+```python
+module_name = 'features.10'
+
+features = extractor.extract_features(
+    batches=batches,
+    module_name=module_name,
+    flatten_acts=True, # flatten 2D feature maps from convolutional layer
+    output_type="ndarray", # or "tensor" (only applicable to PyTorch models)
+)
+
+save_features(features, out_path='path/to/features', file_format='npy')
+```
+
+_For more examples on the many models available in `thingsvision` and explanations of additional functionality like how to optionally turn off center cropping, how to use HDF5 datasets (e.g. NSD stimuli), how to perform RSA or CKA, or how to easily extract features for the [THINGS image database](https://osf.io/jum2f/), please refer to the [Documentation](https://vicco-group.github.io/thingsvision/)._
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- Contributing -->
+## :wave: How to contribute
+If you come across problems or have suggestions please submit an issue!
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- License -->
+## :warning: License
+This GitHub repository is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- Citation -->
+## :page_with_curl: Citation
+If you use this GitHub repository (or any modules associated with it), please cite our [paper](https://www.frontiersin.org/articles/10.3389/fninf.2021.679838/full) for the initial version of `thingsvision` as follows:
+
+```latex
+@article{Muttenthaler_2021,
+	author = {Muttenthaler, Lukas and Hebart, Martin N.},
+	title = {THINGSvision: A Python Toolbox for Streamlining the Extraction of Activations From Deep Neural Networks},
+	journal ={Frontiers in Neuroinformatics},
+	volume = {15},
+	pages = {45},
+	year = {2021},
+	url = {https://www.frontiersin.org/article/10.3389/fninf.2021.679838},
+	doi = {10.3389/fninf.2021.679838},
+	issn = {1662-5196},
+}
+```
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- Contributions -->
+## :gem: Contributions
+This library is based on the groundwork laid by [Lukas Muttenthaler](https://lukasmut.github.io/) and [Martin N. Hebart](http://martin-hebart.de/), who are both still actively involved, but has been extended and refined into its current form with the help of our many contributors,
+
+- [Alex Murphy](https://github.com/Alxmrphi) (software dev.)
+- [Florian Mahner](https://www.cbs.mpg.de/person/mahner/1483114) (software dev.)
+- [Hannes Hansen](https://github.com/hahahannes) (software dev.)
+- [Johannes Roth](https://jroth.space/) (software dev., design, docs)
+- [Jonas Dippel](https://github.com/jonasd4) (software dev.)
+- [Lukas Muttenthaler](https://lukasmut.github.io/) (software dev., design, docs, general responsibility)
+- [Martin N. Hebart](http://martin-hebart.de/) (design)
+- [Oliver Contier](https://olivercontier.com/) (docs)
+- [Philipp Kaniuth](https://www.cbs.mpg.de/person/kaniuth/1483114) (design, docs)
+- [Roman Leipe](https://github.com/RLeipe) (sofware dev., docs),
+
+sorted alphabetically. 
+
+This is a joint open-source project between the Max Planck Institute for Human Cognitive and Brain Sciences, Leipzig, and the Machine Learning Group at Technische Universtität Berlin. Correspondence and requests for contributing should be adressed to [Lukas Muttenthaler](https://lukasmut.github.io/). Feel free to contact us if you want to become a contributor or have any suggestions/feedback. For the latter, you could also just post an issue or engange in discussions. We'll try to respond as fast as we can.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
```

#### html2text {}

```diff
@@ -1,12 +1,15 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.3.8 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.3.9 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
-Description:
+Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
+Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
+MIT License Classifier: Operating System :: OS Independent Requires-Python:
+>=3.8 Description-Content-Type: text/markdown License-File: LICENSE
 [Tests] [Code_Coverage] [Maintenance] [PyPI] [Pepy] [Python_version] [License]
                       [Code_style:_black] [Open_In_Colab]
 
  # :notebook_with_decorative_cover: Table of Contents - [About the Project]
 (#star2-about-the-project) * [Functionality](#mechanical_arm-functionality) *
 [Model collection](#file_cabinet-model-collection) - [Getting Started]
 (#running-getting-started) * [Setting up your environment](#computer-setting-
@@ -157,11 +160,7 @@
 Sciences, Leipzig, and the Machine Learning Group at Technische UniverstitÃ¤t
 Berlin. Correspondence and requests for contributing should be adressed to
 [Lukas Muttenthaler](https://lukasmut.github.io/). Feel free to contact us if
 you want to become a contributor or have any suggestions/feedback. For the
 latter, you could also just post an issue or engange in discussions. We'll try
 to respond as fast as we can.
                                                                   (back_to_top)
-Keywords: feature extraction Platform: UNKNOWN Classifier: Programming Language
-:: Python :: 3.8 Classifier: Natural Language :: English Classifier: License ::
-OSI Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8 Description-Content-Type: text/markdown
```

### Comparing `thingsvision-2.3.8/thingsvision.egg-info/SOURCES.txt` & `thingsvision-2.3.9/thingsvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

