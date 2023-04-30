# Comparing `tmp/antgo-0.1.4.tar.gz` & `tmp/antgo-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antgo-0.1.4.tar", last modified: Sat Apr 29 06:56:00 2023, max compression
+gzip compressed data, was "antgo-0.1.5.tar", last modified: Sun Apr 30 00:02:05 2023, max compression
```

## Comparing `antgo-0.1.4.tar` & `antgo-0.1.5.tar`

### file list

```diff
@@ -1,944 +1,944 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.982218 antgo-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/LICENSE.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-04-29 06:53:15.000000 antgo-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-29 06:56:00.978217 antgo-0.1.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     4480 2023-04-29 06:53:15.000000 antgo-0.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.638213 antgo-0.1.4/antgo/
--rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.646213 antgo-0.1.4/antgo/ant/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25864 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/activelearning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/activelearning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/activelearning_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9805 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/batch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14101 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/browser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28324 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)    34652 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    22044 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/environment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4162 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/flags.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44521 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/watch.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1711 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/config.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)     8645 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.654213 antgo-0.1.4/antgo/crowdsource/
--rwxr-xr-x   0 runner    (1001) docker     (123)      206 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/activelearning_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/base_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    12973 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/batch_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43022 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/browser_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6412 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/crowdsource_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    27245 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/demo_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    15578 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/ensemble_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    33823 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/label_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8055 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/watch_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.654213 antgo-0.1.4/antgo/cutils/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8249 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/cutils/maskApi.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2176 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/cutils/maskApi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.654213 antgo-0.1.4/antgo/dataflow/
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5412 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/basic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22875 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14235 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.670213 antgo-0.1.4/antgo/dataflow/dataset/
--rwxr-xr-x   0 runner    (1001) docker     (123)      783 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/ade20k.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14996 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/celeba.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5425 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/cityscape.py
--rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/clsdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    25177 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/coco2017.py
--rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/cusdomcls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29220 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/empty_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/fashionai_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/fashionai_landmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/flic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3139 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/horse2zebra.py
--rw-r--r--   0 runner    (1001) docker     (123)    35327 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16512 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/interhand26M.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3083 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/iphone2dslr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8328 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/lfw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/lip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/lsp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/mpii.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3725 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/omniglot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/parallel_read.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13131 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/pascal_voc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/proxy_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/queue_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/random_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14554 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4465 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/simpleimages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/simplevideos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/spider_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3559 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/vggface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/visalso.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/datasetio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.670213 antgo-0.1.4/antgo/dataflow/datasynth/
--rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/datasynth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.674214 antgo-0.1.4/antgo/dataflow/imgaug/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1037 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65619 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/autoaugment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    46247 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/batch_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/colorspace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3274 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    25279 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/gridmask_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16268 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/op_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)   110228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/operators_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    17718 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/photometric.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10813 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/regular.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21369 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.678213 antgo-0.1.4/antgo/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.682214 antgo-0.1.4/antgo/framework/helper/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/activelearning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.682214 antgo-0.1.4/antgo/framework/helper/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/apis/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/base_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.682214 antgo-0.1.4/antgo/framework/helper/cnn/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/alexnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.686214 antgo-0.1.4/antgo/framework/helper/cnn/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/backbone/ddr_lcnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/backbone/ddr_mobilenet_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.694214 antgo-0.1.4/antgo/framework/helper/cnn/bricks/
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/context_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/conv2d_adaptive_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/conv_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/depthwise_separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/generalized_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/hsigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/hswish.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/non_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/swish.py
--rw-r--r--   0 runner    (1001) docker     (123)    37224 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/waterfall.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.698214 antgo-0.1.4/antgo/framework/helper/cnn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/utils/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/utils/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)    26005 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/utils/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.698214 antgo-0.1.4/antgo/framework/helper/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.698214 antgo-0.1.4/antgo/framework/helper/configs/activelearning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/activelearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/activelearning/ac_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.698214 antgo-0.1.4/antgo/framework/helper/configs/adda/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/adda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/adda/adda_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.698214 antgo-0.1.4/antgo/framework/helper/configs/distillation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/distillation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/distillation/reviewkd_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.702214 antgo-0.1.4/antgo/framework/helper/configs/semi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/semi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/semi/dense_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/semi/detmpl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/semi/mpl_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.702214 antgo-0.1.4/antgo/framework/helper/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/dataset_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/dataset_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/kvdataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.706214 antgo-0.1.4/antgo/framework/helper/dataset/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37456 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/pipelines/auto_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/pipelines/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/pipelines/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    29127 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/pipelines/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.710214 antgo-0.1.4/antgo/framework/helper/dataset/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/samplers/class_aware_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/samplers/distributed_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/samplers/group_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/samplers/infinite_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/samplers/kv_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/tfdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.710214 antgo-0.1.4/antgo/framework/helper/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36707 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.714214 antgo-0.1.4/antgo/framework/helper/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.714214 antgo-0.1.4/antgo/framework/helper/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/metrics/kp2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/metrics/seg2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.718214 antgo-0.1.4/antgo/framework/helper/models/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.718214 antgo-0.1.4/antgo/framework/helper/models/activelearning/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/activelearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/activelearning/acnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.718214 antgo-0.1.4/antgo/framework/helper/models/adda/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/adda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/adda/adda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.718214 antgo-0.1.4/antgo/framework/helper/models/classification/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.718214 antgo-0.1.4/antgo/framework/helper/models/classification/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23127 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/backbones/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/backbones/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    23751 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/backbones/resnext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.722214 antgo-0.1.4/antgo/framework/helper/models/classification/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/heads/cls_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/heads/stacked_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.722214 antgo-0.1.4/antgo/framework/helper/models/classification/losses/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.722214 antgo-0.1.4/antgo/framework/helper/models/classification/model/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/model/classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.722214 antgo-0.1.4/antgo/framework/helper/models/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.726214 antgo-0.1.4/antgo/framework/helper/models/detectors/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.726214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.726214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/anchor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/point_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.726214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.734214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/approx_max_iou_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/assign_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/atss_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/base_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/center_region_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/grid_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/hungarian_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/max_iou_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/point_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/region_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/sim_ota_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/uniform_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.734214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/base_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/bucketing_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/delta_xywh_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/distance_point_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/legacy_delta_xywh_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/pseudo_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/tblr_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/yolo_bbox_coder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.738214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/iou2d_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.738214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/match_costs/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/match_costs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/match_costs/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/match_costs/match_cost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.742214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/combined_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/instance_balanced_pos_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/iou_balanced_neg_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/ohem_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/pseudo_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/sampling_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/score_hlr_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.742214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/mask/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/mask/mask_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    40231 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/mask/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/mask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.742214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/utils/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.746214 antgo-0.1.4/antgo/framework/helper/models/detectors/head/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/head/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/head/base_dense_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    19071 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/head/fcos_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    24258 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/head/fcos_head_ml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.750214 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/ae_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/balanced_l1_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/gaussian_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/gfocal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/ghm_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15521 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/iou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/kd_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/mse_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/pisa_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    10116 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/seesaw_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/smooth_l1_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/varifocal_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.750214 antgo-0.1.4/antgo/framework/helper/models/detectors/model/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/model/ttfnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.750214 antgo-0.1.4/antgo/framework/helper/models/detectors/neck/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/neck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/neck/fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/single_stage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.754214 antgo-0.1.4/antgo/framework/helper/models/detectors/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/utils/gaussian_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/utils/util_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/utils/util_random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.754214 antgo-0.1.4/antgo/framework/helper/models/distillation/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/distillation_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.762215 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/ab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/afd.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/at.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/bss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/cc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/crd.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/dml.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/fitnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/fsp.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/ft.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/hcl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/irg.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/logits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/lwm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/mgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/nst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/ofd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/pkt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/rkd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/sobolev.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/sp.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/st.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/vid.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/dummy_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/ema_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.762215 antgo-0.1.4/antgo/framework/helper/models/nas/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.762215 antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.762215 antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29450 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/model_zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.766215 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.766215 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/baseline/fastdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/baseline/mobilenet_v3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.766215 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/networks/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/networks/ofa_fastdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16116 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/networks/ofa_mbv3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.766215 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/training/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/training/epoch_based_sampling_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/training/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.766215 antgo-0.1.4/antgo/framework/helper/models/nas/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/search/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.770215 antgo-0.1.4/antgo/framework/helper/models/nas/search/accuracy_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/search/accuracy_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/search/accuracy_predictor/arch_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.770215 antgo-0.1.4/antgo/framework/helper/models/nas/search/efficiency_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/search/efficiency_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/search/efficiency_predictor/latency_lookup_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.770215 antgo-0.1.4/antgo/framework/helper/models/nas/search/search_algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/search/search_algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/search/search_algorithm/evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.770215 antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/accuracy_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/evolution_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15018 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/flops_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/imagenet_eval_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/latency_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.774215 antgo-0.1.4/antgo/framework/helper/models/nas/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/utils/common_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    24233 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/utils/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/utils/my_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/utils/pytorch_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/utils/pytorch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.774215 antgo-0.1.4/antgo/framework/helper/models/pose3d/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.774215 antgo-0.1.4/antgo/framework/helper/models/pose3d/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/backbone/QNetLite0_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/backbone/QNetLite0_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/backbone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.778215 antgo-0.1.4/antgo/framework/helper/models/pose3d/head/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/head/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/head/handpose_qnet_lite0_pose_heatmap2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/head/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/head/twohand_3dpose_latent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.778215 antgo-0.1.4/antgo/framework/helper/models/pose3d/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/losses/gaussian_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.778215 antgo-0.1.4/antgo/framework/helper/models/pose3d/model/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/model/ddr_twohand_pose3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/model/keynet_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.778215 antgo-0.1.4/antgo/framework/helper/models/pose3d/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/proxy_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.778215 antgo-0.1.4/antgo/framework/helper/models/segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.782215 antgo-0.1.4/antgo/framework/helper/models/segmentation/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/segmentation/backbone/DDRQNetLite0.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/segmentation/backbone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.782215 antgo-0.1.4/antgo/framework/helper/models/segmentation/head/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/segmentation/head/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/segmentation/head/aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/segmentation/head/simple_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.782215 antgo-0.1.4/antgo/framework/helper/models/segmentation/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/segmentation/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.782215 antgo-0.1.4/antgo/framework/helper/models/segmentation/model/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/segmentation/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/segmentation/model/encoder_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.782215 antgo-0.1.4/antgo/framework/helper/models/semi/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/semi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/semi/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/semi/detmpl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.782215 antgo-0.1.4/antgo/framework/helper/models/semi/hook/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/semi/hook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/semi/hook/mean_teacher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.786215 antgo-0.1.4/antgo/framework/helper/models/semi/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/semi/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/semi/losses/quality_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/semi/mpl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.790215 antgo-0.1.4/antgo/framework/helper/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10458 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/brick_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/ckpt_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/conv_upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/csp_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/gaussian_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/normed_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/panoptic_gt_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/res_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/structure_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    40231 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/multi_stream_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.794215 antgo-0.1.4/antgo/framework/helper/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/parallel/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/parallel/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/parallel/data_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/parallel/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/parallel/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/parallel/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/parallel/scatter_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/parallel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.798215 antgo-0.1.4/antgo/framework/helper/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19868 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    27545 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/epoch_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/fp16_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.806215 antgo-0.1.4/antgo/framework/helper/runner/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/closure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)    23377 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/iter_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.806215 antgo-0.1.4/antgo/framework/helper/runner/hooks/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/logger/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/logger/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/logger/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    28452 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/lr_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    24618 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/momentum_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/sampler_seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.806215 antgo-0.1.4/antgo/framework/helper/runner/hooks/samplingmethods/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/samplingmethods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/samplingmethods/kcenter_greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/samplingmethods/sampling_def.py
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/submodules_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/sync_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/weight_adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/iter_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/log_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.810215 antgo-0.1.4/antgo/framework/helper/runner/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/task_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.810215 antgo-0.1.4/antgo/framework/helper/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/tools/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/tools/exp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/tools/export_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/tools/schedule_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/tools/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    27342 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.818215 antgo-0.1.4/antgo/framework/helper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/compat_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    27018 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/device_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/ext_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    19158 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/math_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/parrots_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/util_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/version_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.818215 antgo-0.1.4/antgo/framework/paddle2torch/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.822215 antgo-0.1.4/antgo/framework/paddle2torch/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/mapper/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/mapper/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/mapper/nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/mapper/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/mapper/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.822215 antgo-0.1.4/antgo/framework/paddle2torch/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.822215 antgo-0.1.4/antgo/framework/paddle2torch/vision/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.822215 antgo-0.1.4/antgo/framework/torch2paddle/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.830216 antgo-0.1.4/antgo/framework/torch2paddle/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.830216 antgo-0.1.4/antgo/framework/torch2paddle/mapper/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/cuda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/cuda/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/nn_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/nn_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/nn_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/parambase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.830216 antgo-0.1.4/antgo/framework/torch2paddle/mapper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/varbase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.830216 antgo-0.1.4/antgo/framework/torch2paddle/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28762 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/tools/ast_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/tools/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/tools/dependency_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.834215 antgo-0.1.4/antgo/framework/torch2paddle/vision/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/vision/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/vision/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/vision/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24880 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    15294 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/interactcontext.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29822 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20912 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/main_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.846216 antgo-0.1.4/antgo/measures/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2528 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/ali_fashion_attribute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/ali_fashion_landmark_ne.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5903 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/average_precision.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4744 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/binary_c.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1554 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/binomial_deviance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2060 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/confusion_matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21500 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/crowdsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9002 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/deep_analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6339 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/face_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1985 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/kdd_average_precision.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3456 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/matting_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/moving_statistic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4826 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/multi_c.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4348 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/multic_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/multil_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/normalized_error.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    45355 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/objdect_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2826 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/pck.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/person_search_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6784 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/precision_recall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8696 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/quadratic_weighted_kappa.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2438 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/regression_metric.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2765 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/regression_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13252 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/repeat_statistic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      192 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/retrieval_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5448 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/segmentation_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3467 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/significance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7540 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/statistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/topk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/track_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4010 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/yesno_crowdsource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.846216 antgo-0.1.4/antgo/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.850216 antgo-0.1.4/antgo/pipeline/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.850216 antgo-0.1.4/antgo/pipeline/engine/execution/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/engine/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/engine/execution/base_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/engine/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/engine/operator_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/engine/operator_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/engine/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.850216 antgo-0.1.4/antgo/pipeline/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.850216 antgo-0.1.4/antgo/pipeline/functional/common/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/common/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17173 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/data_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/entity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.854216 antgo-0.1.4/antgo/pipeline/functional/image/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/image/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/image/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/image/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.862216 antgo-0.1.4/antgo/pipeline/functional/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/computer_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/option.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/storages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.862216 antgo-0.1.4/antgo/pipeline/hparam/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hparam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hparam/hyperparameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.862216 antgo-0.1.4/antgo/pipeline/hub/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.862216 antgo-0.1.4/antgo/pipeline/hub/builtin/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.862216 antgo-0.1.4/antgo/pipeline/hub/builtin/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/builtin/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/builtin/operators/inference_model_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/builtin/operators/inference_onnx_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/builtin/operators/runas_op.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.866216 antgo-0.1.4/antgo/pipeline/hub/external/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.870216 antgo-0.1.4/antgo/pipeline/hub/external/mm/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/external/mm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/external/mm/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/external/mm/inpainting.py
--rw-r--r--   0 runner    (1001) docker     (123)    18069 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/external/mm/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/external/mm/pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/external/mm/restoration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/external/mm/segmentor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.870216 antgo-0.1.4/antgo/pipeline/models/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.630213 antgo-0.1.4/antgo/pipeline/models/cfg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.870216 antgo-0.1.4/antgo/pipeline/models/cfg/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/cfg/dataset/coco.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.870216 antgo-0.1.4/antgo/pipeline/models/cfg/detector/
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/cfg/detector/yolov7-e6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/cfg/detector/yolov7-w6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/cfg/detector/yolov7.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/cfg/detector/yolov7x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.870216 antgo-0.1.4/antgo/pipeline/models/detector/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/detector/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.874216 antgo-0.1.4/antgo/pipeline/models/detector/yolov7/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/detector/yolov7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/detector/yolov7/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/detector/yolov7/yolov7.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.874216 antgo-0.1.4/antgo/pipeline/models/pose/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/pose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.874216 antgo-0.1.4/antgo/pipeline/models/segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.878216 antgo-0.1.4/antgo/pipeline/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86819 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/utils/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.878216 antgo-0.1.4/antgo/pipeline/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/operators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/operators/nop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.878216 antgo-0.1.4/antgo/pipeline/serve/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.878216 antgo-0.1.4/antgo/pipeline/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/utils/repo_normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.878216 antgo-0.1.4/antgo/resource/
--rwxr-xr-x   0 runner    (1001) docker     (123)      200 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.882216 antgo-0.1.4/antgo/resource/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.882216 antgo-0.1.4/antgo/resource/app/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/css/359.32c5c11e.css
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/css/385.1759eef9.css
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/css/854.9e012a59.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/css/app.48eb9280.css
--rw-r--r--   0 runner    (1001) docker     (123)   219463 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/css/chunk-vendors.1944359c.css
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.898216 antgo-0.1.4/antgo/resource/app/js/
--rw-r--r--   0 runner    (1001) docker     (123)   182502 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/359.afb86915.js
--rw-r--r--   0 runner    (1001) docker     (123)   828443 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/359.afb86915.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/385.90ba0f66.js
--rw-r--r--   0 runner    (1001) docker     (123)    31358 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/385.90ba0f66.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/532.f949def3.js
--rw-r--r--   0 runner    (1001) docker     (123)    24678 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/532.f949def3.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/651.c5601578.js
--rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/651.c5601578.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/769.b7247054.js
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/769.b7247054.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/854.d3c0e54f.js
--rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/854.d3c0e54f.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/880.cba02e88.js
--rw-r--r--   0 runner    (1001) docker     (123)    19810 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/880.cba02e88.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/app.f01f9b7a.js
--rw-r--r--   0 runner    (1001) docker     (123)    33636 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/app.f01f9b7a.js.map
--rw-r--r--   0 runner    (1001) docker     (123)  1289477 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/chunk-vendors.18913786.js
--rw-r--r--   0 runner    (1001) docker     (123)  3750898 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/chunk-vendors.18913786.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.918217 antgo-0.1.4/antgo/resource/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/3dpw.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/ade20k.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/cityscapes.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/coco.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/flic.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/h36m.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/lfw.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15596 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/lip.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/lsp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/mpii.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/vgg-face2-data.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/vgg-face2-meta.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/voc.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    23363 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/html.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.926217 antgo-0.1.4/antgo/resource/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/antgo.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     9662 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/antgo.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/antgo.js
--rw-r--r--   0 runner    (1001) docker     (123)   236514 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/apply.png
--rw-r--r--   0 runner    (1001) docker     (123)   292973 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/banner.png
--rw-r--r--   0 runner    (1001) docker     (123)    32806 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/card.png
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/crowdsource.js
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/error.json
--rw-r--r--   0 runner    (1001) docker     (123)    85624 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/filetree.png
--rw-r--r--   0 runner    (1001) docker     (123)    32294 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/holder.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   106186 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/register.png
--rw-r--r--   0 runner    (1001) docker     (123)   244247 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/start-experiment.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.938217 antgo-0.1.4/antgo/resource/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/activelearning.html
--rwxr-xr-x   0 runner    (1001) docker     (123)    16328 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/crowdsource.html
--rw-r--r--   0 runner    (1001) docker     (123)    22287 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/demo.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.942217 antgo-0.1.4/antgo/resource/templates/mvp/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.946217 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.946217 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/configs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    19161 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.950217 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/models/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/models/wideres.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/coco_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/install.sh
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/launch.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/lsp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/pascal_voc_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/visalso_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/project.json
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/sample_gt.json
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/sample_meta.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    61982 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/statistic-report.html
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/task.template
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/task_main_file.template
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/task_main_param.template
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/task_shell.template
--rw-r--r--   0 runner    (1001) docker     (123)    30333 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/trainmaster.html
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/trainworker.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     1867 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/yesno_crowdsource.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.950217 antgo-0.1.4/antgo/sandbox/
--rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/sandbox/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2542 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/sandbox/sandbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.958217 antgo-0.1.4/antgo/script/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/create_dataset_share.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/custom_submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/data_convert_cifar10_tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/data_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/local_submit.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/ssh-launch.sh
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/ssh-submit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/ssh-submit.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/ssh_submit.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/submit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/test.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.958217 antgo-0.1.4/antgo/task/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/task/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12291 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/task/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.962217 antgo-0.1.4/antgo/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/tools/browser_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/tools/download_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/tools/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/tools/filter_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25713 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/tools/label_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/tools/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/tools/share_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.974218 antgo-0.1.4/antgo/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      402 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1756 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/_bbox.pyx
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/_encode_png.pyx
--rwxr-xr-x   0 runner    (1001) docker     (123)    11418 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/_mask.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/args.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1150 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/argscope.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/colormap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8104 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/concurrency.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1887 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/cpu.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1242 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/encode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3819 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/fs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2915 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/gpu.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4076 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4553 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/mask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9588 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/netvis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10128 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/parallel_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/pickledb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/processbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/sample_gt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1372 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.978217 antgo-0.1.4/antgo/utils/shared_queue/
--rwxr-xr-x   0 runner    (1001) docker     (123)      992 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/shared_queue/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3163 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/shared_queue/queue.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17513 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/shared_queue/sharedmemory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/timer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3959 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.638213 antgo-0.1.4/antgo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-29 06:56:00.000000 antgo-0.1.4/antgo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36262 2023-04-29 06:56:00.000000 antgo-0.1.4/antgo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 06:56:00.000000 antgo-0.1.4/antgo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-29 06:56:00.000000 antgo-0.1.4/antgo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 06:56:00.000000 antgo-0.1.4/antgo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 06:56:00.000000 antgo-0.1.4/antgo.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-04-29 06:53:15.000000 antgo-0.1.4/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-04-29 06:53:15.000000 antgo-0.1.4/roadmap.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 06:56:00.982218 antgo-0.1.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2183 2023-04-29 06:53:15.000000 antgo-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.978217 antgo-0.1.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-29 06:53:15.000000 antgo-0.1.4/test/test_antgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-29 06:53:15.000000 antgo-0.1.4/test/test_paddle_c.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-29 06:53:15.000000 antgo-0.1.4/test/test_torch_c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:05.049716 antgo-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/LICENSE.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-04-29 23:59:18.000000 antgo-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-30 00:02:05.049716 antgo-0.1.5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4480 2023-04-29 23:59:18.000000 antgo-0.1.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.709707 antgo-0.1.5/antgo/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.717707 antgo-0.1.5/antgo/ant/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25864 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/activelearning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/activelearning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/activelearning_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9805 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/batch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14101 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/browser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28324 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34652 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22044 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/environment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4162 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/flags.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44521 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/ant/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1711 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      228 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/config.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8645 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.721708 antgo-0.1.5/antgo/crowdsource/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      206 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/crowdsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/crowdsource/activelearning_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/crowdsource/base_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12973 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/crowdsource/batch_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43022 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/crowdsource/browser_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6412 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/crowdsource/crowdsource_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27245 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/crowdsource/demo_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15578 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/crowdsource/ensemble_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33823 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/crowdsource/label_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/crowdsource/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8055 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/crowdsource/watch_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.725708 antgo-0.1.5/antgo/cutils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8249 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/cutils/maskApi.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2176 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/cutils/maskApi.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.725708 antgo-0.1.5/antgo/dataflow/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5412 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/basic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22875 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14235 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.741708 antgo-0.1.5/antgo/dataflow/dataset/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      783 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/ade20k.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14996 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/celeba.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5425 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/cityscape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/clsdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25177 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/coco2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/cusdomcls.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29220 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/empty_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/fashionai_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/fashionai_landmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/flic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3139 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/horse2zebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35327 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16512 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/interhand26M.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3083 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/iphone2dslr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8328 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/lfw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/lip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/lsp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/mpii.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3725 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/omniglot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/parallel_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13131 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/pascal_voc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/proxy_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/queue_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/random_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14554 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4465 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/simpleimages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/simplevideos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/spider_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3559 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/vggface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/dataset/visalso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/datasetio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.741708 antgo-0.1.5/antgo/dataflow/datasynth/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/datasynth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.749708 antgo-0.1.5/antgo/dataflow/imgaug/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1037 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/imgaug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65619 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/imgaug/autoaugment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46247 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/imgaug/batch_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/imgaug/colorspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3274 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/imgaug/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25279 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/imgaug/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/imgaug/gridmask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16268 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/imgaug/op_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110228 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/imgaug/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/imgaug/operators_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17718 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/imgaug/photometric.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10813 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/imgaug/regular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/imgaug/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21369 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/dataflow/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.749708 antgo-0.1.5/antgo/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.753708 antgo-0.1.5/antgo/framework/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/activelearning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.757709 antgo-0.1.5/antgo/framework/helper/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/apis/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/base_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.757709 antgo-0.1.5/antgo/framework/helper/cnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/alexnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.757709 antgo-0.1.5/antgo/framework/helper/cnn/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/backbone/ddr_lcnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/backbone/ddr_mobilenet_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.773709 antgo-0.1.5/antgo/framework/helper/cnn/bricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/context_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/conv2d_adaptive_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/conv_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/depthwise_separable_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/generalized_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/hsigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/hswish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/non_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/swish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37224 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/bricks/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.773709 antgo-0.1.5/antgo/framework/helper/cnn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/utils/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/utils/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26005 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/utils/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/cnn/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.773709 antgo-0.1.5/antgo/framework/helper/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.773709 antgo-0.1.5/antgo/framework/helper/configs/activelearning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/configs/activelearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/configs/activelearning/ac_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.777709 antgo-0.1.5/antgo/framework/helper/configs/adda/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/configs/adda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/configs/adda/adda_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.777709 antgo-0.1.5/antgo/framework/helper/configs/distillation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/configs/distillation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/configs/distillation/reviewkd_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.777709 antgo-0.1.5/antgo/framework/helper/configs/semi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/configs/semi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/configs/semi/dense_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/configs/semi/detmpl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/configs/semi/mpl_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.781709 antgo-0.1.5/antgo/framework/helper/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/dataset/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/dataset/dataset_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/dataset/dataset_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/dataset/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/dataset/kvdataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.781709 antgo-0.1.5/antgo/framework/helper/dataset/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/dataset/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37456 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/dataset/pipelines/auto_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/dataset/pipelines/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/dataset/pipelines/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29127 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/dataset/pipelines/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.785709 antgo-0.1.5/antgo/framework/helper/dataset/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/dataset/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/dataset/samplers/class_aware_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/dataset/samplers/distributed_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/dataset/samplers/group_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/dataset/samplers/infinite_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/dataset/samplers/kv_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/dataset/tfdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.789709 antgo-0.1.5/antgo/framework/helper/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36707 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.789709 antgo-0.1.5/antgo/framework/helper/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.793709 antgo-0.1.5/antgo/framework/helper/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/metrics/kp2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/metrics/seg2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.793709 antgo-0.1.5/antgo/framework/helper/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.793709 antgo-0.1.5/antgo/framework/helper/models/activelearning/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/activelearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/activelearning/acnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.797710 antgo-0.1.5/antgo/framework/helper/models/adda/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/adda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/adda/adda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.797710 antgo-0.1.5/antgo/framework/helper/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.801710 antgo-0.1.5/antgo/framework/helper/models/classification/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/classification/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23127 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/classification/backbones/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/classification/backbones/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23751 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/classification/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/classification/backbones/resnext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.801710 antgo-0.1.5/antgo/framework/helper/models/classification/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/classification/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/classification/heads/cls_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/classification/heads/stacked_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.805710 antgo-0.1.5/antgo/framework/helper/models/classification/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/classification/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/classification/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/classification/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/classification/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.805710 antgo-0.1.5/antgo/framework/helper/models/classification/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/classification/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/classification/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/classification/model/classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.809710 antgo-0.1.5/antgo/framework/helper/models/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.809710 antgo-0.1.5/antgo/framework/helper/models/detectors/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.809710 antgo-0.1.5/antgo/framework/helper/models/detectors/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.809710 antgo-0.1.5/antgo/framework/helper/models/detectors/core/anchor/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/anchor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/anchor/anchor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/anchor/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/anchor/point_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/anchor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.813710 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.821710 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/approx_max_iou_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/assign_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/atss_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/base_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/center_region_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/grid_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/hungarian_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/max_iou_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/point_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/region_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/sim_ota_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/uniform_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.825710 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/coder/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/coder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/coder/base_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/coder/bucketing_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/coder/delta_xywh_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/coder/distance_point_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/coder/legacy_delta_xywh_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/coder/pseudo_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/coder/tblr_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/coder/yolo_bbox_coder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.825710 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/iou2d_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.829710 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/match_costs/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/match_costs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/match_costs/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/match_costs/match_cost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.833711 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/combined_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/instance_balanced_pos_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/iou_balanced_neg_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/ohem_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/pseudo_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/sampling_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/score_hlr_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.833711 antgo-0.1.5/antgo/framework/helper/models/detectors/core/mask/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/mask/mask_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40231 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/mask/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/mask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.837710 antgo-0.1.5/antgo/framework/helper/models/detectors/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/utils/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.837710 antgo-0.1.5/antgo/framework/helper/models/detectors/head/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/head/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/head/base_dense_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19071 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/head/fcos_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24258 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/head/fcos_head_ml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.845711 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/ae_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/balanced_l1_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/gaussian_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/gfocal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/ghm_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15521 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/iou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/kd_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/mse_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/pisa_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10116 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/seesaw_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/smooth_l1_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/losses/varifocal_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.849711 antgo-0.1.5/antgo/framework/helper/models/detectors/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/model/ttfnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.849711 antgo-0.1.5/antgo/framework/helper/models/detectors/neck/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/neck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/neck/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/single_stage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.849711 antgo-0.1.5/antgo/framework/helper/models/detectors/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/utils/gaussian_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/utils/util_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/detectors/utils/util_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.849711 antgo-0.1.5/antgo/framework/helper/models/distillation/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/distillation_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.861711 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/ab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/afd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/bss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/cc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/crd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/dml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/fitnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/fsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/ft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/hcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/irg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/logits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/lwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/mgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/nst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/ofd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/pkt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/rkd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/sobolev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/sp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/st.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/distillation/loss/vid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/dummy_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/ema_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.861711 antgo-0.1.5/antgo/framework/helper/models/nas/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.861711 antgo-0.1.5/antgo/framework/helper/models/nas/elastic_nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/elastic_nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.861711 antgo-0.1.5/antgo/framework/helper/models/nas/elastic_nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/elastic_nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29450 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/elastic_nn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/model_zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.865711 antgo-0.1.5/antgo/framework/helper/models/nas/ofa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/ofa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.865711 antgo-0.1.5/antgo/framework/helper/models/nas/ofa/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/ofa/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/ofa/baseline/fastdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/ofa/baseline/mobilenet_v3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.865711 antgo-0.1.5/antgo/framework/helper/models/nas/ofa/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/ofa/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/ofa/networks/ofa_fastdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16116 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/ofa/networks/ofa_mbv3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.865711 antgo-0.1.5/antgo/framework/helper/models/nas/ofa/training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/ofa/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/ofa/training/epoch_based_sampling_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/ofa/training/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/ofa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.869711 antgo-0.1.5/antgo/framework/helper/models/nas/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/search/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.869711 antgo-0.1.5/antgo/framework/helper/models/nas/search/accuracy_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/search/accuracy_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/search/accuracy_predictor/arch_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.869711 antgo-0.1.5/antgo/framework/helper/models/nas/search/efficiency_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/search/efficiency_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/search/efficiency_predictor/latency_lookup_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.869711 antgo-0.1.5/antgo/framework/helper/models/nas/search/search_algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/search/search_algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/search/search_algorithm/evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.873711 antgo-0.1.5/antgo/framework/helper/models/nas/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/tutorial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/tutorial/accuracy_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/tutorial/evolution_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15018 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/tutorial/flops_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/tutorial/imagenet_eval_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/tutorial/latency_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.877712 antgo-0.1.5/antgo/framework/helper/models/nas/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/utils/common_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24233 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/utils/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/utils/my_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/utils/pytorch_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/nas/utils/pytorch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.877712 antgo-0.1.5/antgo/framework/helper/models/pose3d/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/pose3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.877712 antgo-0.1.5/antgo/framework/helper/models/pose3d/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/pose3d/backbone/QNetLite0_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/pose3d/backbone/QNetLite0_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/pose3d/backbone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.877712 antgo-0.1.5/antgo/framework/helper/models/pose3d/head/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/pose3d/head/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/pose3d/head/handpose_qnet_lite0_pose_heatmap2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/pose3d/head/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/pose3d/head/twohand_3dpose_latent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.881712 antgo-0.1.5/antgo/framework/helper/models/pose3d/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/pose3d/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/pose3d/losses/gaussian_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/pose3d/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/pose3d/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.881712 antgo-0.1.5/antgo/framework/helper/models/pose3d/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/pose3d/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/pose3d/model/ddr_twohand_pose3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/pose3d/model/keynet_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.881712 antgo-0.1.5/antgo/framework/helper/models/pose3d/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/pose3d/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/proxy_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.881712 antgo-0.1.5/antgo/framework/helper/models/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.881712 antgo-0.1.5/antgo/framework/helper/models/segmentation/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/segmentation/backbone/DDRQNetLite0.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/segmentation/backbone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.881712 antgo-0.1.5/antgo/framework/helper/models/segmentation/head/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/segmentation/head/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/segmentation/head/aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/segmentation/head/simple_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.881712 antgo-0.1.5/antgo/framework/helper/models/segmentation/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/segmentation/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.885712 antgo-0.1.5/antgo/framework/helper/models/segmentation/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/segmentation/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/segmentation/model/encoder_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.885712 antgo-0.1.5/antgo/framework/helper/models/semi/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/semi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/semi/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/semi/detmpl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.885712 antgo-0.1.5/antgo/framework/helper/models/semi/hook/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/semi/hook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/semi/hook/mean_teacher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.885712 antgo-0.1.5/antgo/framework/helper/models/semi/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/semi/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/semi/losses/quality_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/semi/mpl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.893712 antgo-0.1.5/antgo/framework/helper/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10458 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/utils/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/utils/brick_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/utils/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/utils/ckpt_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/utils/conv_upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/utils/csp_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/utils/gaussian_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/utils/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/utils/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/utils/normed_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/utils/panoptic_gt_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/utils/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/utils/res_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/utils/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/utils/structure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40231 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/models/utils/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/multi_stream_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.897712 antgo-0.1.5/antgo/framework/helper/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/parallel/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/parallel/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/parallel/data_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/parallel/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/parallel/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/parallel/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/parallel/scatter_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/parallel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.901712 antgo-0.1.5/antgo/framework/helper/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19868 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27545 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/epoch_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/fp16_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.905712 antgo-0.1.5/antgo/framework/helper/runner/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/closure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23377 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/iter_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.909712 antgo-0.1.5/antgo/framework/helper/runner/hooks/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/logger/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/logger/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/logger/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28452 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/lr_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24618 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/momentum_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/sampler_seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.909712 antgo-0.1.5/antgo/framework/helper/runner/hooks/samplingmethods/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/samplingmethods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/samplingmethods/kcenter_greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/samplingmethods/sampling_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/submodules_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/sync_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/hooks/weight_adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/iter_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/log_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.909712 antgo-0.1.5/antgo/framework/helper/runner/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/runner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/task_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.913712 antgo-0.1.5/antgo/framework/helper/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/tools/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/tools/exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/tools/export_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/tools/schedule_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/tools/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27342 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.921713 antgo-0.1.5/antgo/framework/helper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/compat_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27018 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/device_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/ext_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19158 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/math_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/parrots_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/util_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/helper/utils/version_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.921713 antgo-0.1.5/antgo/framework/paddle2torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/paddle2torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.921713 antgo-0.1.5/antgo/framework/paddle2torch/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/paddle2torch/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/paddle2torch/mapper/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/paddle2torch/mapper/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/paddle2torch/mapper/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/paddle2torch/mapper/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/paddle2torch/mapper/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.921713 antgo-0.1.5/antgo/framework/paddle2torch/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/paddle2torch/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/paddle2torch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.921713 antgo-0.1.5/antgo/framework/paddle2torch/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/paddle2torch/vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.921713 antgo-0.1.5/antgo/framework/torch2paddle/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.929713 antgo-0.1.5/antgo/framework/torch2paddle/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.929713 antgo-0.1.5/antgo/framework/torch2paddle/mapper/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/cuda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/cuda/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/nn_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/nn_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/nn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/parambase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.929713 antgo-0.1.5/antgo/framework/torch2paddle/mapper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/mapper/varbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.933713 antgo-0.1.5/antgo/framework/torch2paddle/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28762 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/tools/ast_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/tools/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/tools/dependency_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.933713 antgo-0.1.5/antgo/framework/torch2paddle/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/vision/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/vision/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/framework/torch2paddle/vision/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24880 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15294 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/interactcontext.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29822 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20912 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/main_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.945713 antgo-0.1.5/antgo/measures/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2528 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/ali_fashion_attribute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/ali_fashion_landmark_ne.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5903 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/average_precision.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4744 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/binary_c.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1554 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/binomial_deviance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2060 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/confusion_matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21500 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/crowdsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9002 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/deep_analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6339 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/face_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1985 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/kdd_average_precision.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3456 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/matting_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/moving_statistic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4826 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/multi_c.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4348 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/multic_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/multil_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/normalized_error.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45355 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/objdect_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2826 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/pck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/person_search_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6784 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/precision_recall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8696 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/quadratic_weighted_kappa.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2438 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/regression_metric.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2765 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/regression_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13252 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/repeat_statistic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      192 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/retrieval_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5448 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/segmentation_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3467 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/significance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7540 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/track_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4010 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/measures/yesno_crowdsource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.945713 antgo-0.1.5/antgo/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.949713 antgo-0.1.5/antgo/pipeline/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.949713 antgo-0.1.5/antgo/pipeline/engine/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/engine/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/engine/execution/base_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/engine/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/engine/operator_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/engine/operator_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/engine/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.953714 antgo-0.1.5/antgo/pipeline/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.953714 antgo-0.1.5/antgo/pipeline/functional/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/common/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17173 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/data_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/entity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.953714 antgo-0.1.5/antgo/pipeline/functional/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/image/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/image/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/image/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.961714 antgo-0.1.5/antgo/pipeline/functional/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/mixins/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/mixins/computer_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/mixins/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/mixins/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/mixins/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/mixins/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/mixins/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/mixins/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/mixins/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/mixins/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/mixins/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/mixins/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/mixins/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/functional/storages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.961714 antgo-0.1.5/antgo/pipeline/hparam/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/hparam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/hparam/hyperparameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.961714 antgo-0.1.5/antgo/pipeline/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.961714 antgo-0.1.5/antgo/pipeline/hub/builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/hub/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.961714 antgo-0.1.5/antgo/pipeline/hub/builtin/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/hub/builtin/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/hub/builtin/operators/inference_model_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/hub/builtin/operators/inference_onnx_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/hub/builtin/operators/runas_op.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.961714 antgo-0.1.5/antgo/pipeline/hub/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/hub/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.965714 antgo-0.1.5/antgo/pipeline/hub/external/mm/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/hub/external/mm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/hub/external/mm/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/hub/external/mm/inpainting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18069 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/hub/external/mm/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/hub/external/mm/pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/hub/external/mm/restoration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/hub/external/mm/segmentor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.965714 antgo-0.1.5/antgo/pipeline/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.701707 antgo-0.1.5/antgo/pipeline/models/cfg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.965714 antgo-0.1.5/antgo/pipeline/models/cfg/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/models/cfg/dataset/coco.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.969714 antgo-0.1.5/antgo/pipeline/models/cfg/detector/
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/models/cfg/detector/yolov7-e6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/models/cfg/detector/yolov7-w6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/models/cfg/detector/yolov7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/models/cfg/detector/yolov7x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.969714 antgo-0.1.5/antgo/pipeline/models/detector/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/models/detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/models/detector/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.969714 antgo-0.1.5/antgo/pipeline/models/detector/yolov7/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/models/detector/yolov7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/models/detector/yolov7/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/models/detector/yolov7/yolov7.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.969714 antgo-0.1.5/antgo/pipeline/models/pose/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/models/pose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.969714 antgo-0.1.5/antgo/pipeline/models/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/models/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.973714 antgo-0.1.5/antgo/pipeline/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86819 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/models/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/models/utils/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/models/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.973714 antgo-0.1.5/antgo/pipeline/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/operators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/operators/nop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.973714 antgo-0.1.5/antgo/pipeline/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.973714 antgo-0.1.5/antgo/pipeline/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/pipeline/utils/repo_normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.977714 antgo-0.1.5/antgo/resource/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      200 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.977714 antgo-0.1.5/antgo/resource/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.977714 antgo-0.1.5/antgo/resource/app/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/css/359.32c5c11e.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/css/385.1759eef9.css
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/css/854.9e012a59.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/css/app.48eb9280.css
+-rw-r--r--   0 runner    (1001) docker     (123)   219463 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/css/chunk-vendors.1944359c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.993714 antgo-0.1.5/antgo/resource/app/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   182502 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/js/359.afb86915.js
+-rw-r--r--   0 runner    (1001) docker     (123)   828443 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/js/359.afb86915.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/js/385.90ba0f66.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31358 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/js/385.90ba0f66.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/js/532.f949def3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24678 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/js/532.f949def3.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/js/651.c5601578.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/js/651.c5601578.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/js/769.b7247054.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/js/769.b7247054.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/js/854.d3c0e54f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/js/854.d3c0e54f.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/js/880.cba02e88.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19810 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/js/880.cba02e88.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/js/app.f01f9b7a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33636 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/js/app.f01f9b7a.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)  1289477 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/js/chunk-vendors.18913786.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3750898 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/app/js/chunk-vendors.18913786.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:05.009715 antgo-0.1.5/antgo/resource/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/dataset/3dpw.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/dataset/ade20k.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/dataset/cityscapes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/dataset/coco.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/dataset/flic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/dataset/h36m.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/dataset/lfw.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15596 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/dataset/lip.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/dataset/lsp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/dataset/mpii.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/dataset/vgg-face2-data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/dataset/vgg-face2-meta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/dataset/voc.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23363 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:05.017715 antgo-0.1.5/antgo/resource/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/static/antgo.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9662 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/static/antgo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/static/antgo.js
+-rw-r--r--   0 runner    (1001) docker     (123)   236514 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/static/apply.png
+-rw-r--r--   0 runner    (1001) docker     (123)   292973 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/static/banner.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32806 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/static/card.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/static/crowdsource.js
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/static/error.json
+-rw-r--r--   0 runner    (1001) docker     (123)    85624 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/static/filetree.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32294 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/static/holder.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   106186 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/static/register.png
+-rw-r--r--   0 runner    (1001) docker     (123)   244247 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/static/start-experiment.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:05.025715 antgo-0.1.5/antgo/resource/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/activelearning.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16328 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/crowdsource.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22287 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/demo.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:05.029715 antgo-0.1.5/antgo/resource/templates/mvp/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:05.029715 antgo-0.1.5/antgo/resource/templates/mvp/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:05.029715 antgo-0.1.5/antgo/resource/templates/mvp/cifar10/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/cifar10/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/cifar10/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/cifar10/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19161 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/cifar10/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/cifar10/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:05.029715 antgo-0.1.5/antgo/resource/templates/mvp/cifar10/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/cifar10/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/cifar10/models/wideres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/coco_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/install.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/launch.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/lsp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/pascal_voc_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/mvp/visalso_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/project.json
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/sample_gt.json
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/sample_meta.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    61982 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/statistic-report.html
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/task.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/task_main_file.template
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/task_main_param.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/task_shell.template
+-rw-r--r--   0 runner    (1001) docker     (123)    30333 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/trainmaster.html
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/trainworker.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1867 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/resource/templates/yesno_crowdsource.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:05.033715 antgo-0.1.5/antgo/sandbox/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/sandbox/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2542 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/sandbox/sandbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:05.033715 antgo-0.1.5/antgo/script/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/script/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/script/create_dataset_share.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/script/custom_submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/script/data_convert_cifar10_tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/script/data_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/script/local_submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/script/ssh-launch.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/script/ssh-submit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/script/ssh-submit.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/script/ssh_submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/script/submit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/script/test.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:05.037716 antgo-0.1.5/antgo/task/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/task/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12291 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/task/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:05.037716 antgo-0.1.5/antgo/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/tools/browser_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/tools/download_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/tools/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/tools/filter_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25713 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/tools/label_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/tools/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/tools/share_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:05.045716 antgo-0.1.5/antgo/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      402 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1756 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/_bbox.pyx
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/_encode_png.pyx
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11418 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/_mask.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/args.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1150 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/argscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/colormap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8104 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/concurrency.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1887 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/cpu.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1242 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/encode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3819 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/fs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2915 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/gpu.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4076 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4553 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/mask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9588 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/netvis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10128 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/parallel_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/pickledb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/processbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/sample_gt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1372 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:05.049716 antgo-0.1.5/antgo/utils/shared_queue/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      992 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/shared_queue/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3163 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/shared_queue/queue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17513 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/shared_queue/sharedmemory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3959 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-04-29 23:59:18.000000 antgo-0.1.5/antgo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:04.709707 antgo-0.1.5/antgo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-30 00:02:04.000000 antgo-0.1.5/antgo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36262 2023-04-30 00:02:04.000000 antgo-0.1.5/antgo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 00:02:04.000000 antgo-0.1.5/antgo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-30 00:02:04.000000 antgo-0.1.5/antgo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 00:02:04.000000 antgo-0.1.5/antgo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 00:02:04.000000 antgo-0.1.5/antgo.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-04-29 23:59:18.000000 antgo-0.1.5/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-04-29 23:59:18.000000 antgo-0.1.5/roadmap.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 00:02:05.049716 antgo-0.1.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2183 2023-04-29 23:59:18.000000 antgo-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:02:05.049716 antgo-0.1.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-29 23:59:18.000000 antgo-0.1.5/test/test_antgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-29 23:59:18.000000 antgo-0.1.5/test/test_paddle_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-29 23:59:18.000000 antgo-0.1.5/test/test_torch_c.py
```

### Comparing `antgo-0.1.4/PKG-INFO` & `antgo-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antgo
-Version: 0.1.4
+Version: 0.1.5
 Summary: machine learning experiment platform
 Home-page: https://github.com/jianzfb/antgo
 Author: jian
 Author-email: jian@mltalker.com
 License-File: LICENSE.md
 
 ======================
```

### Comparing `antgo-0.1.4/README.rst` & `antgo-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/ant/activelearning.py` & `antgo-0.1.5/antgo/ant/activelearning.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/ant/activelearning_api.py` & `antgo-0.1.5/antgo/ant/activelearning_api.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/ant/activelearning_v2.py` & `antgo-0.1.5/antgo/ant/activelearning_v2.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/ant/base.py` & `antgo-0.1.5/antgo/ant/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/ant/batch.py` & `antgo-0.1.5/antgo/ant/batch.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/ant/browser.py` & `antgo-0.1.5/antgo/ant/browser.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/ant/challenge.py` & `antgo-0.1.5/antgo/ant/challenge.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/ant/client.py` & `antgo-0.1.5/antgo/ant/client.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/ant/debug.py` & `antgo-0.1.5/antgo/ant/debug.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/ant/demo.py` & `antgo-0.1.5/antgo/ant/demo.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/ant/download.py` & `antgo-0.1.5/antgo/ant/download.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/ant/ensemble.py` & `antgo-0.1.5/antgo/ant/ensemble.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/ant/environment.py` & `antgo-0.1.5/antgo/ant/environment.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/ant/flags.py` & `antgo-0.1.5/antgo/ant/flags.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/ant/train.py` & `antgo-0.1.5/antgo/ant/train.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/ant/utils.py` & `antgo-0.1.5/antgo/ant/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/ant/watch.py` & `antgo-0.1.5/antgo/ant/watch.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/config.py` & `antgo-0.1.5/antgo/config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/context.py` & `antgo-0.1.5/antgo/context.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/crowdsource/activelearning_server.py` & `antgo-0.1.5/antgo/crowdsource/activelearning_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/crowdsource/base_server.py` & `antgo-0.1.5/antgo/crowdsource/base_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/crowdsource/batch_server.py` & `antgo-0.1.5/antgo/crowdsource/batch_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/crowdsource/browser_server.py` & `antgo-0.1.5/antgo/crowdsource/browser_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/crowdsource/crowdsource_server.py` & `antgo-0.1.5/antgo/crowdsource/crowdsource_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/crowdsource/demo_server.py` & `antgo-0.1.5/antgo/crowdsource/demo_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/crowdsource/ensemble_server.py` & `antgo-0.1.5/antgo/crowdsource/ensemble_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/crowdsource/label_server.py` & `antgo-0.1.5/antgo/crowdsource/label_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/crowdsource/utils.py` & `antgo-0.1.5/antgo/crowdsource/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/crowdsource/watch_server.py` & `antgo-0.1.5/antgo/crowdsource/watch_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/cutils/maskApi.c` & `antgo-0.1.5/antgo/cutils/maskApi.c`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/cutils/maskApi.h` & `antgo-0.1.5/antgo/cutils/maskApi.h`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/basic.py` & `antgo-0.1.5/antgo/dataflow/basic.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/common.py` & `antgo-0.1.5/antgo/dataflow/common.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/core.py` & `antgo-0.1.5/antgo/dataflow/core.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/__init__.py` & `antgo-0.1.5/antgo/dataflow/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/ade20k.py` & `antgo-0.1.5/antgo/dataflow/dataset/ade20k.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/celeba.py` & `antgo-0.1.5/antgo/dataflow/dataset/celeba.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/cifar.py` & `antgo-0.1.5/antgo/dataflow/dataset/cifar.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/cityscape.py` & `antgo-0.1.5/antgo/dataflow/dataset/cityscape.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/clsdataset.py` & `antgo-0.1.5/antgo/dataflow/dataset/clsdataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/coco2017.py` & `antgo-0.1.5/antgo/dataflow/dataset/coco2017.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/cusdomcls.py` & `antgo-0.1.5/antgo/dataflow/dataset/cusdomcls.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/dataset.py` & `antgo-0.1.5/antgo/dataflow/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/empty_dataset.py` & `antgo-0.1.5/antgo/dataflow/dataset/empty_dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/fashionai_attribute.py` & `antgo-0.1.5/antgo/dataflow/dataset/fashionai_attribute.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/fashionai_landmark.py` & `antgo-0.1.5/antgo/dataflow/dataset/fashionai_landmark.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/flic.py` & `antgo-0.1.5/antgo/dataflow/dataset/flic.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/horse2zebra.py` & `antgo-0.1.5/antgo/dataflow/dataset/horse2zebra.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/imagenet.py` & `antgo-0.1.5/antgo/dataflow/dataset/imagenet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/interhand26M.py` & `antgo-0.1.5/antgo/dataflow/dataset/interhand26M.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/iphone2dslr.py` & `antgo-0.1.5/antgo/dataflow/dataset/iphone2dslr.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/lfw.py` & `antgo-0.1.5/antgo/dataflow/dataset/lfw.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/lip.py` & `antgo-0.1.5/antgo/dataflow/dataset/lip.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/lsp.py` & `antgo-0.1.5/antgo/dataflow/dataset/lsp.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/mnist.py` & `antgo-0.1.5/antgo/dataflow/dataset/mnist.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/mpii.py` & `antgo-0.1.5/antgo/dataflow/dataset/mpii.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/omniglot.py` & `antgo-0.1.5/antgo/dataflow/dataset/omniglot.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/parallel_read.py` & `antgo-0.1.5/antgo/dataflow/dataset/parallel_read.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/pascal_voc.py` & `antgo-0.1.5/antgo/dataflow/dataset/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/proxy_dataset.py` & `antgo-0.1.5/antgo/dataflow/dataset/proxy_dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/queue_dataset.py` & `antgo-0.1.5/antgo/dataflow/dataset/queue_dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/random_dataset.py` & `antgo-0.1.5/antgo/dataflow/dataset/random_dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/reader.py` & `antgo-0.1.5/antgo/dataflow/dataset/reader.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/simpleimages.py` & `antgo-0.1.5/antgo/dataflow/dataset/simpleimages.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/simplevideos.py` & `antgo-0.1.5/antgo/dataflow/dataset/simplevideos.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/spider_dataset.py` & `antgo-0.1.5/antgo/dataflow/dataset/spider_dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/vggface.py` & `antgo-0.1.5/antgo/dataflow/dataset/vggface.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/dataset/visalso.py` & `antgo-0.1.5/antgo/dataflow/dataset/visalso.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/datasetio.py` & `antgo-0.1.5/antgo/dataflow/datasetio.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/imgaug/__init__.py` & `antgo-0.1.5/antgo/dataflow/imgaug/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/imgaug/autoaugment_utils.py` & `antgo-0.1.5/antgo/dataflow/imgaug/autoaugment_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/imgaug/batch_operators.py` & `antgo-0.1.5/antgo/dataflow/imgaug/batch_operators.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/imgaug/colorspace.py` & `antgo-0.1.5/antgo/dataflow/imgaug/colorspace.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/imgaug/functional.py` & `antgo-0.1.5/antgo/dataflow/imgaug/functional.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/imgaug/geometric.py` & `antgo-0.1.5/antgo/dataflow/imgaug/geometric.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/imgaug/gridmask_utils.py` & `antgo-0.1.5/antgo/dataflow/imgaug/gridmask_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/imgaug/op_helper.py` & `antgo-0.1.5/antgo/dataflow/imgaug/op_helper.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/imgaug/operators.py` & `antgo-0.1.5/antgo/dataflow/imgaug/operators.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/imgaug/operators_3d.py` & `antgo-0.1.5/antgo/dataflow/imgaug/operators_3d.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/imgaug/photometric.py` & `antgo-0.1.5/antgo/dataflow/imgaug/photometric.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/imgaug/regular.py` & `antgo-0.1.5/antgo/dataflow/imgaug/regular.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/imgaug/util.py` & `antgo-0.1.5/antgo/dataflow/imgaug/util.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/recorder.py` & `antgo-0.1.5/antgo/dataflow/recorder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/dataflow/vis.py` & `antgo-0.1.5/antgo/dataflow/vis.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/activelearning.py` & `antgo-0.1.5/antgo/framework/helper/activelearning.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/apis/train.py` & `antgo-0.1.5/antgo/framework/helper/apis/train.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/base_module.py` & `antgo-0.1.5/antgo/framework/helper/base_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/base_trainer.py` & `antgo-0.1.5/antgo/framework/helper/base_trainer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/__init__.py` & `antgo-0.1.5/antgo/framework/helper/cnn/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/alexnet.py` & `antgo-0.1.5/antgo/framework/helper/cnn/alexnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/backbone/ddr_lcnet.py` & `antgo-0.1.5/antgo/framework/helper/cnn/backbone/ddr_lcnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/backbone/ddr_mobilenet_v2.py` & `antgo-0.1.5/antgo/framework/helper/cnn/backbone/ddr_mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/__init__.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/activation.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/activation.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/context_block.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/context_block.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/conv.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/conv.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/conv2d_adaptive_padding.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/conv2d_adaptive_padding.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/conv_module.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/conv_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/conv_ws.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/conv_ws.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/depthwise_separable_conv_module.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/drop.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/generalized_attention.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/generalized_attention.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/hsigmoid.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/hsigmoid.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/hswish.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/hswish.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/inverted_residual.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/make_divisible.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/make_divisible.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/non_local.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/non_local.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/norm.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/norm.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/padding.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/padding.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/plugin.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/plugin.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/registry.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/registry.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/scale.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/scale.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/se_layer.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/se_layer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/transformer.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/transformer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/upsample.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/upsample.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/waterfall.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/waterfall.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/bricks/wrappers.py` & `antgo-0.1.5/antgo/framework/helper/cnn/bricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/resnet.py` & `antgo-0.1.5/antgo/framework/helper/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/utils/__init__.py` & `antgo-0.1.5/antgo/framework/helper/cnn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/utils/flops_counter.py` & `antgo-0.1.5/antgo/framework/helper/cnn/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/utils/fuse_conv_bn.py` & `antgo-0.1.5/antgo/framework/helper/cnn/utils/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/utils/sync_bn.py` & `antgo-0.1.5/antgo/framework/helper/cnn/utils/sync_bn.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/utils/weight_init.py` & `antgo-0.1.5/antgo/framework/helper/cnn/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/cnn/vgg.py` & `antgo-0.1.5/antgo/framework/helper/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/configs/activelearning/ac_config.py` & `antgo-0.1.5/antgo/framework/helper/configs/activelearning/ac_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/configs/adda/adda_config.py` & `antgo-0.1.5/antgo/framework/helper/configs/adda/adda_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/configs/distillation/reviewkd_config.py` & `antgo-0.1.5/antgo/framework/helper/configs/distillation/reviewkd_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/configs/semi/dense_config.py` & `antgo-0.1.5/antgo/framework/helper/configs/semi/dense_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/configs/semi/mpl_config.py` & `antgo-0.1.5/antgo/framework/helper/configs/semi/mpl_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/dataset/__init__.py` & `antgo-0.1.5/antgo/framework/helper/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/dataset/builder.py` & `antgo-0.1.5/antgo/framework/helper/dataset/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/dataset/dataset_filter.py` & `antgo-0.1.5/antgo/framework/helper/dataset/dataset_filter.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/dataset/dataset_split.py` & `antgo-0.1.5/antgo/framework/helper/dataset/dataset_split.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/dataset/dataset_wrappers.py` & `antgo-0.1.5/antgo/framework/helper/dataset/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/dataset/kvdataset.py` & `antgo-0.1.5/antgo/framework/helper/dataset/kvdataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/dataset/pipelines/auto_augment.py` & `antgo-0.1.5/antgo/framework/helper/dataset/pipelines/auto_augment.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/dataset/pipelines/builder.py` & `antgo-0.1.5/antgo/framework/helper/dataset/pipelines/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/dataset/pipelines/formatting.py` & `antgo-0.1.5/antgo/framework/helper/dataset/pipelines/formatting.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/dataset/pipelines/transforms.py` & `antgo-0.1.5/antgo/framework/helper/dataset/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/dataset/samplers/__init__.py` & `antgo-0.1.5/antgo/framework/helper/dataset/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/dataset/samplers/class_aware_sampler.py` & `antgo-0.1.5/antgo/framework/helper/dataset/samplers/class_aware_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/dataset/samplers/distributed_sampler.py` & `antgo-0.1.5/antgo/framework/helper/dataset/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/dataset/samplers/group_sampler.py` & `antgo-0.1.5/antgo/framework/helper/dataset/samplers/group_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/dataset/samplers/infinite_sampler.py` & `antgo-0.1.5/antgo/framework/helper/dataset/samplers/infinite_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/dataset/samplers/kv_sampler.py` & `antgo-0.1.5/antgo/framework/helper/dataset/samplers/kv_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/dataset/tfdataset.py` & `antgo-0.1.5/antgo/framework/helper/dataset/tfdataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -497,20 +497,23 @@
             pprint(f'Rank {self.rank} local-index {local_select_index_list_in_world}')
             pprint(f'Rank {self.rank} thread id {worker_info.id} use index {select_index_list} and data path list {data_path_list}')
 
         remain_sample_num = 0
         if worker_info is not None:
             shard = worker_info.id, worker_info.num_workers
             np.random.seed(worker_info.seed % np.iinfo(np.uint32).max)
-            remain_sample_num = int(self.num_samples - real_num_samples)
             if worker_info.num_workers != 1:
-                if worker_info.id != worker_info.num_workers - 1:
-                    remain_sample_num = remain_sample_num // worker_info.num_workers
-                else:
-                    remain_sample_num = (remain_sample_num // worker_info.num_workers) + (remain_sample_num - remain_sample_num // worker_info.num_workers * worker_info.num_workers)
+                expect_target_num = \
+                    self.num_samples * (worker_info.id+1) // worker_info.num_workers - \
+                    self.num_samples * (worker_info.id) // worker_info.num_workers
+
+                real_target_num = real_num_samples * (worker_info.id+1) // worker_info.num_workers - \
+                    real_num_samples * (worker_info.id) // worker_info.num_workers
+
+                remain_sample_num = expect_target_num - real_target_num
 
             # debug
             pprint(f'Rank {self.rank} thread {worker_info.id} face remain sample_num {remain_sample_num}')
         else:
             shard = None
 
         if not self.sample_num_equalizer:
```

### Comparing `antgo-0.1.4/antgo/framework/helper/exporter.py` & `antgo-0.1.5/antgo/framework/helper/exporter.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/fileio/__init__.py` & `antgo-0.1.5/antgo/framework/helper/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/fileio/file_client.py` & `antgo-0.1.5/antgo/framework/helper/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/fileio/handlers/base.py` & `antgo-0.1.5/antgo/framework/helper/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/fileio/handlers/json_handler.py` & `antgo-0.1.5/antgo/framework/helper/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/fileio/handlers/pickle_handler.py` & `antgo-0.1.5/antgo/framework/helper/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/fileio/handlers/yaml_handler.py` & `antgo-0.1.5/antgo/framework/helper/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/fileio/io.py` & `antgo-0.1.5/antgo/framework/helper/fileio/io.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/fileio/parse.py` & `antgo-0.1.5/antgo/framework/helper/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/metrics/kp2d.py` & `antgo-0.1.5/antgo/framework/helper/metrics/kp2d.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/metrics/metrics.py` & `antgo-0.1.5/antgo/framework/helper/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/metrics/seg2d.py` & `antgo-0.1.5/antgo/framework/helper/metrics/seg2d.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/activelearning/acnet.py` & `antgo-0.1.5/antgo/framework/helper/models/activelearning/acnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/adda/adda.py` & `antgo-0.1.5/antgo/framework/helper/models/adda/adda.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/builder.py` & `antgo-0.1.5/antgo/framework/helper/models/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/classification/backbones/hrnet.py` & `antgo-0.1.5/antgo/framework/helper/models/classification/backbones/hrnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/classification/backbones/mobilenet_v2.py` & `antgo-0.1.5/antgo/framework/helper/models/classification/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/classification/backbones/resnet.py` & `antgo-0.1.5/antgo/framework/helper/models/classification/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/classification/backbones/resnext.py` & `antgo-0.1.5/antgo/framework/helper/models/classification/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/classification/heads/cls_head.py` & `antgo-0.1.5/antgo/framework/helper/models/classification/heads/cls_head.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/classification/heads/stacked_head.py` & `antgo-0.1.5/antgo/framework/helper/models/classification/heads/stacked_head.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/classification/losses/accuracy.py` & `antgo-0.1.5/antgo/framework/helper/models/classification/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/classification/losses/cross_entropy_loss.py` & `antgo-0.1.5/antgo/framework/helper/models/classification/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/classification/losses/utils.py` & `antgo-0.1.5/antgo/framework/helper/models/classification/losses/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/classification/model/base.py` & `antgo-0.1.5/antgo/framework/helper/models/classification/model/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/classification/model/classifier.py` & `antgo-0.1.5/antgo/framework/helper/models/classification/model/classifier.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/base.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/__init__.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/anchor/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/anchor_generator.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/anchor/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/builder.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/anchor/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/point_generator.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/anchor/point_generator.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/utils.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/anchor/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/__init__.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/__init__.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/approx_max_iou_assigner.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/approx_max_iou_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/assign_result.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/assign_result.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/atss_assigner.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/atss_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/center_region_assigner.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/center_region_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/grid_assigner.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/grid_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/hungarian_assigner.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/hungarian_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/max_iou_assigner.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/max_iou_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/point_assigner.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/point_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/region_assigner.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/region_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/sim_ota_assigner.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/sim_ota_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/uniform_assigner.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/assigners/uniform_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/builder.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/__init__.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/coder/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/bucketing_bbox_coder.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/coder/bucketing_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/delta_xywh_bbox_coder.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/coder/delta_xywh_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/distance_point_bbox_coder.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/coder/distance_point_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/legacy_delta_xywh_bbox_coder.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/coder/legacy_delta_xywh_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/pseudo_bbox_coder.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/coder/pseudo_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/tblr_bbox_coder.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/coder/tblr_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/yolo_bbox_coder.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/coder/yolo_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/iou2d_calculator.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/iou2d_calculator.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/match_costs/match_cost.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/match_costs/match_cost.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/__init__.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/base_sampler.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/base_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/combined_sampler.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/combined_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/instance_balanced_pos_sampler.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/instance_balanced_pos_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/iou_balanced_neg_sampler.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/iou_balanced_neg_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/ohem_sampler.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/ohem_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/pseudo_sampler.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/pseudo_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/random_sampler.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/sampling_result.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/sampling_result.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/score_hlr_sampler.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/samplers/score_hlr_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/transforms.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/bbox/transforms.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/mask/mask_target.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/mask/mask_target.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/mask/structures.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/mask/structures.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/mask/utils.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/mask/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/utils/__init__.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/utils/dist_utils.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/utils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/core/utils/misc.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/core/utils/misc.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/head/base_dense_head.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/head/base_dense_head.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/head/fcos_head.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/head/fcos_head.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/head/fcos_head_ml.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/head/fcos_head_ml.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/__init__.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/accuracy.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/ae_loss.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/losses/ae_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/balanced_l1_loss.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/losses/balanced_l1_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/cross_entropy_loss.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/dice_loss.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/losses/dice_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/focal_loss.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/gaussian_focal_loss.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/losses/gaussian_focal_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/gfocal_loss.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/losses/gfocal_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/ghm_loss.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/losses/ghm_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/iou_loss.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/losses/iou_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/kd_loss.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/losses/kd_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/mse_loss.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/losses/mse_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/pisa_loss.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/losses/pisa_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/seesaw_loss.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/losses/seesaw_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/smooth_l1_loss.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/losses/smooth_l1_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/utils.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/losses/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/varifocal_loss.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/losses/varifocal_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/model/ttfnet.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/model/ttfnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/neck/fpn.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/neck/fpn.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/single_stage.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/single_stage.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/utils/gaussian_target.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/utils/gaussian_target.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/utils/util_mixins.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/utils/util_mixins.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/detectors/utils/util_random.py` & `antgo-0.1.5/antgo/framework/helper/models/detectors/utils/util_random.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/distillation_model.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/distillation_model.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/ab.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/ab.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/afd.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/afd.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/at.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/at.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/bss.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/bss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/cc.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/cc.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/crd.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/crd.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/dml.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/dml.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/fsp.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/fsp.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/ft.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/ft.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/hcl.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/hcl.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/irg.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/irg.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/logits.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/logits.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/lwm.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/lwm.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/mgd.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/mgd.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/nst.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/nst.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/ofd.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/ofd.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/pkt.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/pkt.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/rkd.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/rkd.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/sobolev.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/sobolev.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/sp.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/sp.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/st.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/st.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/vid.py` & `antgo-0.1.5/antgo/framework/helper/models/distillation/loss/vid.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/dummy_module.py` & `antgo-0.1.5/antgo/framework/helper/models/dummy_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/ema_module.py` & `antgo-0.1.5/antgo/framework/helper/models/ema_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_layers.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_layers.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_op.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_op.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/utils.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/elastic_nn/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/model_zoo.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/model_zoo.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/ofa/baseline/mobilenet_v3.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/ofa/baseline/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/ofa/networks/ofa_mbv3.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/ofa/networks/ofa_mbv3.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/ofa/training/epoch_based_sampling_runner.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/ofa/training/epoch_based_sampling_runner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/ofa/training/evaluation.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/ofa/training/evaluation.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/ofa/utils.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/ofa/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_dataset.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_predictor.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_predictor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/search/accuracy_predictor/arch_encoder.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/search/accuracy_predictor/arch_encoder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/search/efficiency_predictor/__init__.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/search/efficiency_predictor/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/search/efficiency_predictor/latency_lookup_table.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/search/efficiency_predictor/latency_lookup_table.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/search/search_algorithm/evolution.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/search/search_algorithm/evolution.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/test.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/test.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/accuracy_predictor.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/tutorial/accuracy_predictor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/evolution_finder.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/tutorial/evolution_finder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/flops_table.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/tutorial/flops_table.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/imagenet_eval_helper.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/tutorial/imagenet_eval_helper.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/latency_table.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/tutorial/latency_table.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/utils/common_tools.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/utils/common_tools.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/utils/flops_counter.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/utils/layers.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/utils/layers.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/utils/my_modules.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/utils/my_modules.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/utils/pytorch_modules.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/utils/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/nas/utils/pytorch_utils.py` & `antgo-0.1.5/antgo/framework/helper/models/nas/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/pose3d/backbone/QNetLite0_alpha.py` & `antgo-0.1.5/antgo/framework/helper/models/pose3d/backbone/QNetLite0_alpha.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/pose3d/backbone/QNetLite0_beta.py` & `antgo-0.1.5/antgo/framework/helper/models/pose3d/backbone/QNetLite0_beta.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/pose3d/head/handpose_qnet_lite0_pose_heatmap2d.py` & `antgo-0.1.5/antgo/framework/helper/models/pose3d/head/handpose_qnet_lite0_pose_heatmap2d.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/pose3d/head/layer.py` & `antgo-0.1.5/antgo/framework/helper/models/pose3d/head/layer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/pose3d/head/twohand_3dpose_latent.py` & `antgo-0.1.5/antgo/framework/helper/models/pose3d/head/twohand_3dpose_latent.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/pose3d/losses/gaussian_focal_loss.py` & `antgo-0.1.5/antgo/framework/helper/models/pose3d/losses/gaussian_focal_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/pose3d/losses/loss.py` & `antgo-0.1.5/antgo/framework/helper/models/pose3d/losses/loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/pose3d/losses/utils.py` & `antgo-0.1.5/antgo/framework/helper/models/pose3d/losses/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/pose3d/model/ddr_twohand_pose3d.py` & `antgo-0.1.5/antgo/framework/helper/models/pose3d/model/ddr_twohand_pose3d.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/pose3d/model/keynet_model.py` & `antgo-0.1.5/antgo/framework/helper/models/pose3d/model/keynet_model.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/proxy_module.py` & `antgo-0.1.5/antgo/framework/helper/models/proxy_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/segmentation/backbone/DDRQNetLite0.py` & `antgo-0.1.5/antgo/framework/helper/models/segmentation/backbone/DDRQNetLite0.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/segmentation/head/aspp_head.py` & `antgo-0.1.5/antgo/framework/helper/models/segmentation/head/aspp_head.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/segmentation/head/simple_head.py` & `antgo-0.1.5/antgo/framework/helper/models/segmentation/head/simple_head.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/segmentation/model/encoder_decoder.py` & `antgo-0.1.5/antgo/framework/helper/models/segmentation/model/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/semi/dense.py` & `antgo-0.1.5/antgo/framework/helper/models/semi/dense.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/semi/detmpl.py` & `antgo-0.1.5/antgo/framework/helper/models/semi/detmpl.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/semi/hook/mean_teacher.py` & `antgo-0.1.5/antgo/framework/helper/models/semi/hook/mean_teacher.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/semi/losses/quality_focal_loss.py` & `antgo-0.1.5/antgo/framework/helper/models/semi/losses/quality_focal_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/semi/mpl.py` & `antgo-0.1.5/antgo/framework/helper/models/semi/mpl.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/utils/__init__.py` & `antgo-0.1.5/antgo/framework/helper/models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/utils/box_utils.py` & `antgo-0.1.5/antgo/framework/helper/models/utils/box_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/utils/brick_wrappers.py` & `antgo-0.1.5/antgo/framework/helper/models/utils/brick_wrappers.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/utils/builder.py` & `antgo-0.1.5/antgo/framework/helper/models/utils/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/utils/ckpt_convert.py` & `antgo-0.1.5/antgo/framework/helper/models/utils/ckpt_convert.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/utils/conv_upsample.py` & `antgo-0.1.5/antgo/framework/helper/models/utils/conv_upsample.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/utils/csp_layer.py` & `antgo-0.1.5/antgo/framework/helper/models/utils/csp_layer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/utils/gaussian_target.py` & `antgo-0.1.5/antgo/framework/helper/models/utils/gaussian_target.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/utils/inverted_residual.py` & `antgo-0.1.5/antgo/framework/helper/models/utils/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/utils/make_divisible.py` & `antgo-0.1.5/antgo/framework/helper/models/utils/make_divisible.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/utils/misc.py` & `antgo-0.1.5/antgo/framework/helper/models/utils/misc.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/utils/normed_predictor.py` & `antgo-0.1.5/antgo/framework/helper/models/utils/normed_predictor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/utils/panoptic_gt_processing.py` & `antgo-0.1.5/antgo/framework/helper/models/utils/panoptic_gt_processing.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/utils/positional_encoding.py` & `antgo-0.1.5/antgo/framework/helper/models/utils/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/utils/res_layer.py` & `antgo-0.1.5/antgo/framework/helper/models/utils/res_layer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/utils/se_layer.py` & `antgo-0.1.5/antgo/framework/helper/models/utils/se_layer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/utils/structure_utils.py` & `antgo-0.1.5/antgo/framework/helper/models/utils/structure_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/models/utils/structures.py` & `antgo-0.1.5/antgo/framework/helper/models/utils/structures.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/multi_stream_module.py` & `antgo-0.1.5/antgo/framework/helper/multi_stream_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/parallel/_functions.py` & `antgo-0.1.5/antgo/framework/helper/parallel/_functions.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/parallel/collate.py` & `antgo-0.1.5/antgo/framework/helper/parallel/collate.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/parallel/data_container.py` & `antgo-0.1.5/antgo/framework/helper/parallel/data_container.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/parallel/data_parallel.py` & `antgo-0.1.5/antgo/framework/helper/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/parallel/distributed.py` & `antgo-0.1.5/antgo/framework/helper/parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/parallel/scatter_gather.py` & `antgo-0.1.5/antgo/framework/helper/parallel/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/parallel/utils.py` & `antgo-0.1.5/antgo/framework/helper/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/reader.py` & `antgo-0.1.5/antgo/framework/helper/reader.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/__init__.py` & `antgo-0.1.5/antgo/framework/helper/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/base_runner.py` & `antgo-0.1.5/antgo/framework/helper/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/builder.py` & `antgo-0.1.5/antgo/framework/helper/runner/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/checkpoint.py` & `antgo-0.1.5/antgo/framework/helper/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/default_constructor.py` & `antgo-0.1.5/antgo/framework/helper/runner/default_constructor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/dist_utils.py` & `antgo-0.1.5/antgo/framework/helper/runner/dist_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/epoch_based_runner.py` & `antgo-0.1.5/antgo/framework/helper/runner/epoch_based_runner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/fp16_utils.py` & `antgo-0.1.5/antgo/framework/helper/runner/fp16_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/__init__.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/checkpoint.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/ema.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/ema.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/evaluation.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/evaluation.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/hook.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/logger/base.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/logger/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/logger/neptune.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/logger/neptune.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/logger/text.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/logger/text.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/lr_updater.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/lr_updater.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/memory.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/memory.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/momentum_updater.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/momentum_updater.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/optimizer.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/optimizer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/profiler.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/profiler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/sampler_seed.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/sampler_seed.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/samplingmethods/kcenter_greedy.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/samplingmethods/kcenter_greedy.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/samplingmethods/sampling_def.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/samplingmethods/sampling_def.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/submodules_evaluation.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/submodules_evaluation.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/sync_buffer.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/sync_buffer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/hooks/weight_adjust.py` & `antgo-0.1.5/antgo/framework/helper/runner/hooks/weight_adjust.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/iter_based_runner.py` & `antgo-0.1.5/antgo/framework/helper/runner/iter_based_runner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/log_buffer.py` & `antgo-0.1.5/antgo/framework/helper/runner/log_buffer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/optimizer/builder.py` & `antgo-0.1.5/antgo/framework/helper/runner/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/optimizer/default_constructor.py` & `antgo-0.1.5/antgo/framework/helper/runner/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/priority.py` & `antgo-0.1.5/antgo/framework/helper/runner/priority.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/test.py` & `antgo-0.1.5/antgo/framework/helper/runner/test.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/runner/utils.py` & `antgo-0.1.5/antgo/framework/helper/runner/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/task_flag.py` & `antgo-0.1.5/antgo/framework/helper/task_flag.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/tester.py` & `antgo-0.1.5/antgo/framework/helper/tester.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/tools/evaluate.py` & `antgo-0.1.5/antgo/framework/helper/tools/evaluate.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/tools/exp.py` & `antgo-0.1.5/antgo/framework/helper/tools/exp.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/tools/export_onnx.py` & `antgo-0.1.5/antgo/framework/helper/tools/export_onnx.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/tools/train.py` & `antgo-0.1.5/antgo/framework/helper/tools/train.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/tools/util.py` & `antgo-0.1.5/antgo/framework/helper/tools/util.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/trainer.py` & `antgo-0.1.5/antgo/framework/helper/trainer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/__init__.py` & `antgo-0.1.5/antgo/framework/helper/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/compat_config.py` & `antgo-0.1.5/antgo/framework/helper/utils/compat_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/config.py` & `antgo-0.1.5/antgo/framework/helper/utils/config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/dist_utils.py` & `antgo-0.1.5/antgo/framework/helper/utils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/env.py` & `antgo-0.1.5/antgo/framework/helper/utils/env.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/ext_loader.py` & `antgo-0.1.5/antgo/framework/helper/utils/ext_loader.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/hub.py` & `antgo-0.1.5/antgo/framework/helper/utils/hub.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/logging.py` & `antgo-0.1.5/antgo/framework/helper/utils/logging.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/math_3d.py` & `antgo-0.1.5/antgo/framework/helper/utils/math_3d.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/misc.py` & `antgo-0.1.5/antgo/framework/helper/utils/misc.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/parrots_jit.py` & `antgo-0.1.5/antgo/framework/helper/utils/parrots_jit.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/parrots_wrapper.py` & `antgo-0.1.5/antgo/framework/helper/utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/path.py` & `antgo-0.1.5/antgo/framework/helper/utils/path.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/progressbar.py` & `antgo-0.1.5/antgo/framework/helper/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/registry.py` & `antgo-0.1.5/antgo/framework/helper/utils/registry.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/seed.py` & `antgo-0.1.5/antgo/framework/helper/utils/seed.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/setup_env.py` & `antgo-0.1.5/antgo/framework/helper/utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/testing.py` & `antgo-0.1.5/antgo/framework/helper/utils/testing.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/timer.py` & `antgo-0.1.5/antgo/framework/helper/utils/timer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/trace.py` & `antgo-0.1.5/antgo/framework/helper/utils/trace.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/util_distribution.py` & `antgo-0.1.5/antgo/framework/helper/utils/util_distribution.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/helper/utils/version_utils.py` & `antgo-0.1.5/antgo/framework/helper/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/paddle2torch/mapper/io.py` & `antgo-0.1.5/antgo/framework/paddle2torch/mapper/io.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/paddle2torch/mapper/nn.py` & `antgo-0.1.5/antgo/framework/paddle2torch/mapper/nn.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/paddle2torch/mapper/ops.py` & `antgo-0.1.5/antgo/framework/paddle2torch/mapper/ops.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/paddle2torch/mapper/optimizer.py` & `antgo-0.1.5/antgo/framework/paddle2torch/mapper/optimizer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/paddle2torch/utils.py` & `antgo-0.1.5/antgo/framework/paddle2torch/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/mapper/__init__.py` & `antgo-0.1.5/antgo/framework/torch2paddle/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/mapper/device.py` & `antgo-0.1.5/antgo/framework/torch2paddle/mapper/device.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/mapper/distributed.py` & `antgo-0.1.5/antgo/framework/torch2paddle/mapper/distributed.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/mapper/io.py` & `antgo-0.1.5/antgo/framework/torch2paddle/mapper/io.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/mapper/layer.py` & `antgo-0.1.5/antgo/framework/torch2paddle/mapper/layer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/mapper/nn.py` & `antgo-0.1.5/antgo/framework/torch2paddle/mapper/nn.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/mapper/nn_functional.py` & `antgo-0.1.5/antgo/framework/torch2paddle/mapper/nn_functional.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/mapper/nn_init.py` & `antgo-0.1.5/antgo/framework/torch2paddle/mapper/nn_init.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/mapper/nn_utils.py` & `antgo-0.1.5/antgo/framework/torch2paddle/mapper/nn_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/mapper/ops.py` & `antgo-0.1.5/antgo/framework/torch2paddle/mapper/ops.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/mapper/optimizer.py` & `antgo-0.1.5/antgo/framework/torch2paddle/mapper/optimizer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/mapper/parambase.py` & `antgo-0.1.5/antgo/framework/torch2paddle/mapper/parambase.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/mapper/tensor.py` & `antgo-0.1.5/antgo/framework/torch2paddle/mapper/tensor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/mapper/varbase.py` & `antgo-0.1.5/antgo/framework/torch2paddle/mapper/varbase.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/tools/ast_update.py` & `antgo-0.1.5/antgo/framework/torch2paddle/tools/ast_update.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/tools/convert.py` & `antgo-0.1.5/antgo/framework/torch2paddle/tools/convert.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/tools/dependency_analyzer.py` & `antgo-0.1.5/antgo/framework/torch2paddle/tools/dependency_analyzer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/tools/utils.py` & `antgo-0.1.5/antgo/framework/torch2paddle/tools/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/utils.py` & `antgo-0.1.5/antgo/framework/torch2paddle/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/vision/datasets.py` & `antgo-0.1.5/antgo/framework/torch2paddle/vision/datasets.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/vision/transforms.py` & `antgo-0.1.5/antgo/framework/torch2paddle/vision/transforms.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/framework/torch2paddle/vision/utils.py` & `antgo-0.1.5/antgo/framework/torch2paddle/vision/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/help.py` & `antgo-0.1.5/antgo/help.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/interactcontext.py` & `antgo-0.1.5/antgo/interactcontext.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/main.py` & `antgo-0.1.5/antgo/main.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/main_backup.py` & `antgo-0.1.5/antgo/main_backup.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/__init__.py` & `antgo-0.1.5/antgo/measures/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/ali_fashion_attribute_error.py` & `antgo-0.1.5/antgo/measures/ali_fashion_attribute_error.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/ali_fashion_landmark_ne.py` & `antgo-0.1.5/antgo/measures/ali_fashion_landmark_ne.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/average_precision.py` & `antgo-0.1.5/antgo/measures/average_precision.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/base.py` & `antgo-0.1.5/antgo/measures/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/binary_c.py` & `antgo-0.1.5/antgo/measures/binary_c.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/binomial_deviance.py` & `antgo-0.1.5/antgo/measures/binomial_deviance.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/confusion_matrix.py` & `antgo-0.1.5/antgo/measures/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/crowdsource.py` & `antgo-0.1.5/antgo/measures/crowdsource.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/deep_analysis.py` & `antgo-0.1.5/antgo/measures/deep_analysis.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/error.py` & `antgo-0.1.5/antgo/measures/error.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/face_task.py` & `antgo-0.1.5/antgo/measures/face_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/kdd_average_precision.py` & `antgo-0.1.5/antgo/measures/kdd_average_precision.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/matting_task.py` & `antgo-0.1.5/antgo/measures/matting_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/moving_statistic.py` & `antgo-0.1.5/antgo/measures/moving_statistic.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/multi_c.py` & `antgo-0.1.5/antgo/measures/multi_c.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/multic_task.py` & `antgo-0.1.5/antgo/measures/multic_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/multil_task.py` & `antgo-0.1.5/antgo/measures/multil_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/objdect_task.py` & `antgo-0.1.5/antgo/measures/objdect_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/pck.py` & `antgo-0.1.5/antgo/measures/pck.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/person_search_task.py` & `antgo-0.1.5/antgo/measures/person_search_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/precision_recall.py` & `antgo-0.1.5/antgo/measures/precision_recall.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/quadratic_weighted_kappa.py` & `antgo-0.1.5/antgo/measures/quadratic_weighted_kappa.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/regression_metric.py` & `antgo-0.1.5/antgo/measures/regression_metric.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/regression_task.py` & `antgo-0.1.5/antgo/measures/regression_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/repeat_statistic.py` & `antgo-0.1.5/antgo/measures/repeat_statistic.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/roc_auc.py` & `antgo-0.1.5/antgo/measures/roc_auc.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/segmentation_task.py` & `antgo-0.1.5/antgo/measures/segmentation_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/significance.py` & `antgo-0.1.5/antgo/measures/significance.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/statistic.py` & `antgo-0.1.5/antgo/measures/statistic.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/topk.py` & `antgo-0.1.5/antgo/measures/topk.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/track_task.py` & `antgo-0.1.5/antgo/measures/track_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/measures/yesno_crowdsource.py` & `antgo-0.1.5/antgo/measures/yesno_crowdsource.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/engine/__init__.py` & `antgo-0.1.5/antgo/pipeline/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/engine/execution/base_execution.py` & `antgo-0.1.5/antgo/pipeline/engine/execution/base_execution.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/engine/factory.py` & `antgo-0.1.5/antgo/pipeline/engine/factory.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/engine/operator_loader.py` & `antgo-0.1.5/antgo/pipeline/engine/operator_loader.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/engine/operator_registry.py` & `antgo-0.1.5/antgo/pipeline/engine/operator_registry.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/engine/uri.py` & `antgo-0.1.5/antgo/pipeline/engine/uri.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/__init__.py` & `antgo-0.1.5/antgo/pipeline/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/common/util.py` & `antgo-0.1.5/antgo/pipeline/functional/common/util.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/data_collection.py` & `antgo-0.1.5/antgo/pipeline/functional/data_collection.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/entity.py` & `antgo-0.1.5/antgo/pipeline/functional/entity.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/image/__init__.py` & `antgo-0.1.5/antgo/pipeline/functional/image/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/image/io.py` & `antgo-0.1.5/antgo/pipeline/functional/image/io.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/image/plot.py` & `antgo-0.1.5/antgo/pipeline/functional/image/plot.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/image/process.py` & `antgo-0.1.5/antgo/pipeline/functional/image/process.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/mixins/__init__.py` & `antgo-0.1.5/antgo/pipeline/functional/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/mixins/column.py` & `antgo-0.1.5/antgo/pipeline/functional/mixins/column.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/mixins/computer_vision.py` & `antgo-0.1.5/antgo/pipeline/functional/mixins/computer_vision.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/mixins/config.py` & `antgo-0.1.5/antgo/pipeline/functional/mixins/config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/mixins/dag.py` & `antgo-0.1.5/antgo/pipeline/functional/mixins/dag.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/mixins/data_processing.py` & `antgo-0.1.5/antgo/pipeline/functional/mixins/data_processing.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/mixins/dataframe.py` & `antgo-0.1.5/antgo/pipeline/functional/mixins/dataframe.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/mixins/dataset.py` & `antgo-0.1.5/antgo/pipeline/functional/mixins/dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/mixins/demo.py` & `antgo-0.1.5/antgo/pipeline/functional/mixins/demo.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/mixins/dispatcher.py` & `antgo-0.1.5/antgo/pipeline/functional/mixins/dispatcher.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/mixins/list.py` & `antgo-0.1.5/antgo/pipeline/functional/mixins/list.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/mixins/serve.py` & `antgo-0.1.5/antgo/pipeline/functional/mixins/serve.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/mixins/show.py` & `antgo-0.1.5/antgo/pipeline/functional/mixins/show.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/mixins/stream.py` & `antgo-0.1.5/antgo/pipeline/functional/mixins/stream.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/option.py` & `antgo-0.1.5/antgo/pipeline/functional/option.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/functional/storages.py` & `antgo-0.1.5/antgo/pipeline/functional/storages.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/hparam/__init__.py` & `antgo-0.1.5/antgo/pipeline/hparam/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/hparam/hyperparameter.py` & `antgo-0.1.5/antgo/pipeline/hparam/hyperparameter.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/hub/builtin/operators/inference_model_op.py` & `antgo-0.1.5/antgo/pipeline/hub/builtin/operators/inference_model_op.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/hub/builtin/operators/inference_onnx_op.py` & `antgo-0.1.5/antgo/pipeline/hub/builtin/operators/inference_onnx_op.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/hub/builtin/operators/runas_op.py` & `antgo-0.1.5/antgo/pipeline/hub/builtin/operators/runas_op.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/hub/external/mm/detector.py` & `antgo-0.1.5/antgo/pipeline/hub/external/mm/detector.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/hub/external/mm/inpainting.py` & `antgo-0.1.5/antgo/pipeline/hub/external/mm/inpainting.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/hub/external/mm/ocr.py` & `antgo-0.1.5/antgo/pipeline/hub/external/mm/ocr.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/hub/external/mm/pose.py` & `antgo-0.1.5/antgo/pipeline/hub/external/mm/pose.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/hub/external/mm/restoration.py` & `antgo-0.1.5/antgo/pipeline/hub/external/mm/restoration.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/hub/external/mm/segmentor.py` & `antgo-0.1.5/antgo/pipeline/hub/external/mm/segmentor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/models/cfg/dataset/coco.yaml` & `antgo-0.1.5/antgo/pipeline/models/cfg/dataset/coco.yaml`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/models/cfg/detector/yolov7-e6.yaml` & `antgo-0.1.5/antgo/pipeline/models/cfg/detector/yolov7-e6.yaml`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/models/cfg/detector/yolov7-w6.yaml` & `antgo-0.1.5/antgo/pipeline/models/cfg/detector/yolov7-w6.yaml`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/models/cfg/detector/yolov7.yaml` & `antgo-0.1.5/antgo/pipeline/models/cfg/detector/yolov7.yaml`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/models/cfg/detector/yolov7x.yaml` & `antgo-0.1.5/antgo/pipeline/models/cfg/detector/yolov7x.yaml`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/models/detector/util.py` & `antgo-0.1.5/antgo/pipeline/models/detector/util.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/models/detector/yolov7/util.py` & `antgo-0.1.5/antgo/pipeline/models/detector/yolov7/util.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/models/detector/yolov7/yolov7.py` & `antgo-0.1.5/antgo/pipeline/models/detector/yolov7/yolov7.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/models/utils/common.py` & `antgo-0.1.5/antgo/pipeline/models/utils/common.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/models/utils/preprocess.py` & `antgo-0.1.5/antgo/pipeline/models/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/models/utils/utils.py` & `antgo-0.1.5/antgo/pipeline/models/utils/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/operators/base.py` & `antgo-0.1.5/antgo/pipeline/operators/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/operators/nop.py` & `antgo-0.1.5/antgo/pipeline/operators/nop.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/pipeline/utils/repo_normalize.py` & `antgo-0.1.5/antgo/pipeline/utils/repo_normalize.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/css/359.32c5c11e.css` & `antgo-0.1.5/antgo/resource/app/css/359.32c5c11e.css`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/css/385.1759eef9.css` & `antgo-0.1.5/antgo/resource/app/css/385.1759eef9.css`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/css/chunk-vendors.1944359c.css` & `antgo-0.1.5/antgo/resource/app/css/chunk-vendors.1944359c.css`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/favicon.ico` & `antgo-0.1.5/antgo/resource/app/favicon.ico`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/index.html` & `antgo-0.1.5/antgo/resource/app/index.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/js/359.afb86915.js` & `antgo-0.1.5/antgo/resource/app/js/359.afb86915.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/js/359.afb86915.js.map` & `antgo-0.1.5/antgo/resource/app/js/359.afb86915.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/js/385.90ba0f66.js` & `antgo-0.1.5/antgo/resource/app/js/385.90ba0f66.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/js/385.90ba0f66.js.map` & `antgo-0.1.5/antgo/resource/app/js/385.90ba0f66.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/js/532.f949def3.js` & `antgo-0.1.5/antgo/resource/app/js/532.f949def3.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/js/532.f949def3.js.map` & `antgo-0.1.5/antgo/resource/app/js/532.f949def3.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/js/651.c5601578.js` & `antgo-0.1.5/antgo/resource/app/js/651.c5601578.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/js/651.c5601578.js.map` & `antgo-0.1.5/antgo/resource/app/js/651.c5601578.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/js/769.b7247054.js` & `antgo-0.1.5/antgo/resource/app/js/769.b7247054.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/js/769.b7247054.js.map` & `antgo-0.1.5/antgo/resource/app/js/769.b7247054.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/js/854.d3c0e54f.js` & `antgo-0.1.5/antgo/resource/app/js/854.d3c0e54f.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/js/854.d3c0e54f.js.map` & `antgo-0.1.5/antgo/resource/app/js/854.d3c0e54f.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/js/880.cba02e88.js` & `antgo-0.1.5/antgo/resource/app/js/880.cba02e88.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/js/880.cba02e88.js.map` & `antgo-0.1.5/antgo/resource/app/js/880.cba02e88.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/js/app.f01f9b7a.js` & `antgo-0.1.5/antgo/resource/app/js/app.f01f9b7a.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/js/app.f01f9b7a.js.map` & `antgo-0.1.5/antgo/resource/app/js/app.f01f9b7a.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/js/chunk-vendors.18913786.js` & `antgo-0.1.5/antgo/resource/app/js/chunk-vendors.18913786.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/app/js/chunk-vendors.18913786.js.map` & `antgo-0.1.5/antgo/resource/app/js/chunk-vendors.18913786.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/dataset/3dpw.txt` & `antgo-0.1.5/antgo/resource/dataset/3dpw.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/dataset/ade20k.txt` & `antgo-0.1.5/antgo/resource/dataset/ade20k.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/dataset/cityscapes.txt` & `antgo-0.1.5/antgo/resource/dataset/cityscapes.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/dataset/coco.txt` & `antgo-0.1.5/antgo/resource/dataset/coco.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/dataset/flic.txt` & `antgo-0.1.5/antgo/resource/dataset/flic.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/dataset/h36m.txt` & `antgo-0.1.5/antgo/resource/dataset/h36m.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/dataset/lfw.txt` & `antgo-0.1.5/antgo/resource/dataset/lfw.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/dataset/lip.txt` & `antgo-0.1.5/antgo/resource/dataset/lip.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/dataset/lsp.txt` & `antgo-0.1.5/antgo/resource/dataset/lsp.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/dataset/mpii.txt` & `antgo-0.1.5/antgo/resource/dataset/mpii.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/dataset/vgg-face2-data.txt` & `antgo-0.1.5/antgo/resource/dataset/vgg-face2-data.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/dataset/vgg-face2-meta.txt` & `antgo-0.1.5/antgo/resource/dataset/vgg-face2-meta.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/dataset/voc.txt` & `antgo-0.1.5/antgo/resource/dataset/voc.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/html.py` & `antgo-0.1.5/antgo/resource/html.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/static/antgo.ico` & `antgo-0.1.5/antgo/resource/static/antgo.ico`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/static/antgo.js` & `antgo-0.1.5/antgo/resource/static/antgo.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/static/apply.png` & `antgo-0.1.5/antgo/resource/static/apply.png`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/static/banner.png` & `antgo-0.1.5/antgo/resource/static/banner.png`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/static/card.png` & `antgo-0.1.5/antgo/resource/static/card.png`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/static/filetree.png` & `antgo-0.1.5/antgo/resource/static/filetree.png`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/static/holder.min.js` & `antgo-0.1.5/antgo/resource/static/holder.min.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/static/register.png` & `antgo-0.1.5/antgo/resource/static/register.png`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/static/start-experiment.png` & `antgo-0.1.5/antgo/resource/static/start-experiment.png`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/activelearning.html` & `antgo-0.1.5/antgo/resource/templates/activelearning.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/crowdsource.html` & `antgo-0.1.5/antgo/resource/templates/crowdsource.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/demo.html` & `antgo-0.1.5/antgo/resource/templates/demo.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/mvp/README.md` & `antgo-0.1.5/antgo/resource/templates/mvp/README.md`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/mvp/cifar10/configs/config.py` & `antgo-0.1.5/antgo/resource/templates/mvp/cifar10/configs/config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/mvp/cifar10/dataset.py` & `antgo-0.1.5/antgo/resource/templates/mvp/cifar10/dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/mvp/cifar10/hooks.py` & `antgo-0.1.5/antgo/resource/templates/mvp/cifar10/hooks.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/mvp/cifar10/main.py` & `antgo-0.1.5/antgo/resource/templates/mvp/cifar10/main.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/mvp/cifar10/metrics.py` & `antgo-0.1.5/antgo/resource/templates/mvp/cifar10/metrics.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/mvp/cifar10/models/wideres.py` & `antgo-0.1.5/antgo/resource/templates/mvp/cifar10/models/wideres.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/mvp/coco_config.py` & `antgo-0.1.5/antgo/resource/templates/mvp/coco_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/mvp/config.py` & `antgo-0.1.5/antgo/resource/templates/mvp/config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/mvp/lsp_config.py` & `antgo-0.1.5/antgo/resource/templates/mvp/lsp_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/mvp/pascal_voc_config.py` & `antgo-0.1.5/antgo/resource/templates/mvp/pascal_voc_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/mvp/system.py` & `antgo-0.1.5/antgo/resource/templates/mvp/system.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/mvp/visalso_config.py` & `antgo-0.1.5/antgo/resource/templates/mvp/visalso_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/project.json` & `antgo-0.1.5/antgo/resource/templates/project.json`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/sample_gt.json` & `antgo-0.1.5/antgo/resource/templates/sample_gt.json`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/statistic-report.html` & `antgo-0.1.5/antgo/resource/templates/statistic-report.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/task_main_file.template` & `antgo-0.1.5/antgo/resource/templates/task_main_file.template`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/task_main_param.template` & `antgo-0.1.5/antgo/resource/templates/task_main_param.template`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/task_shell.template` & `antgo-0.1.5/antgo/resource/templates/task_shell.template`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/trainmaster.html` & `antgo-0.1.5/antgo/resource/templates/trainmaster.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/resource/templates/yesno_crowdsource.html` & `antgo-0.1.5/antgo/resource/templates/yesno_crowdsource.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/sandbox/sandbox.py` & `antgo-0.1.5/antgo/sandbox/sandbox.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/script/base.py` & `antgo-0.1.5/antgo/script/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/script/create_dataset_share.py` & `antgo-0.1.5/antgo/script/create_dataset_share.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/script/custom_submit.py` & `antgo-0.1.5/antgo/script/custom_submit.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/script/data_convert_cifar10_tfrecord.py` & `antgo-0.1.5/antgo/script/data_convert_cifar10_tfrecord.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/script/data_prepare.py` & `antgo-0.1.5/antgo/script/data_prepare.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/script/local_submit.py` & `antgo-0.1.5/antgo/script/local_submit.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/script/ssh-submit.sh` & `antgo-0.1.5/antgo/script/ssh-submit.sh`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/script/ssh_submit.py` & `antgo-0.1.5/antgo/script/ssh_submit.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/task/task.py` & `antgo-0.1.5/antgo/task/task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/tools/__init__.py` & `antgo-0.1.5/antgo/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/tools/browser_funcs.py` & `antgo-0.1.5/antgo/tools/browser_funcs.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/tools/download_funcs.py` & `antgo-0.1.5/antgo/tools/download_funcs.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/tools/extract.py` & `antgo-0.1.5/antgo/tools/extract.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/tools/filter_funcs.py` & `antgo-0.1.5/antgo/tools/filter_funcs.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/tools/label_funcs.py` & `antgo-0.1.5/antgo/tools/label_funcs.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/tools/package.py` & `antgo-0.1.5/antgo/tools/package.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/tools/share_funcs.py` & `antgo-0.1.5/antgo/tools/share_funcs.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/_bbox.pyx` & `antgo-0.1.5/antgo/utils/_bbox.pyx`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/_encode_png.pyx` & `antgo-0.1.5/antgo/utils/_encode_png.pyx`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/_mask.pyx` & `antgo-0.1.5/antgo/utils/_mask.pyx`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/args.py` & `antgo-0.1.5/antgo/utils/args.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/argscope.py` & `antgo-0.1.5/antgo/utils/argscope.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/colormap.py` & `antgo-0.1.5/antgo/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/concurrency.py` & `antgo-0.1.5/antgo/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/cpu.py` & `antgo-0.1.5/antgo/utils/cpu.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/encode.py` & `antgo-0.1.5/antgo/utils/encode.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/fs.py` & `antgo-0.1.5/antgo/utils/fs.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/gpu.py` & `antgo-0.1.5/antgo/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/logger.py` & `antgo-0.1.5/antgo/utils/logger.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/mask.py` & `antgo-0.1.5/antgo/utils/mask.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/netvis.py` & `antgo-0.1.5/antgo/utils/netvis.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/parallel_map.py` & `antgo-0.1.5/antgo/utils/parallel_map.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/pickledb.py` & `antgo-0.1.5/antgo/utils/pickledb.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/processbar.py` & `antgo-0.1.5/antgo/utils/processbar.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/sample_gt.py` & `antgo-0.1.5/antgo/utils/sample_gt.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/serialize.py` & `antgo-0.1.5/antgo/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/shared_queue/__init__.py` & `antgo-0.1.5/antgo/utils/shared_queue/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/shared_queue/queue.py` & `antgo-0.1.5/antgo/utils/shared_queue/queue.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/shared_queue/sharedmemory.py` & `antgo-0.1.5/antgo/utils/shared_queue/sharedmemory.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/timer.py` & `antgo-0.1.5/antgo/utils/timer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo/utils/utils.py` & `antgo-0.1.5/antgo/utils/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/antgo.egg-info/PKG-INFO` & `antgo-0.1.5/antgo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antgo
-Version: 0.1.4
+Version: 0.1.5
 Summary: machine learning experiment platform
 Home-page: https://github.com/jianzfb/antgo
 Author: jian
 Author-email: jian@mltalker.com
 License-File: LICENSE.md
 
 ======================
```

### Comparing `antgo-0.1.4/antgo.egg-info/SOURCES.txt` & `antgo-0.1.5/antgo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/setup.py` & `antgo-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 def read_requirements(filename):
     return [line.strip() for line in read_file(filename).splitlines()
             if not line.startswith('#')]
 
 
 setup(name='antgo',
-      version='0.1.4',
+      version='0.1.5',
       description='machine learning experiment platform',
       __short_description__='machine learning experiment platform',
       url='https://github.com/jianzfb/antgo',
       author='jian',
       author_email='jian@mltalker.com',
       setup_requires=[
         # Setuptools 18.0 properly handles Cython extensions.
```

### Comparing `antgo-0.1.4/test/test_antgo.py` & `antgo-0.1.5/test/test_antgo.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/test/test_paddle_c.py` & `antgo-0.1.5/test/test_paddle_c.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.4/test/test_torch_c.py` & `antgo-0.1.5/test/test_torch_c.py`

 * *Files identical despite different names*

