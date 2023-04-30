# Comparing `tmp/HILO-MPC-1.0.2.tar.gz` & `tmp/HILO-MPC-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HILO-MPC-1.0.2.tar", last modified: Wed Sep 14 12:09:16 2022, max compression
+gzip compressed data, was "HILO-MPC-1.0.3.tar", last modified: Sun Apr 30 07:38:07 2023, max compression
```

## Comparing `HILO-MPC-1.0.2.tar` & `HILO-MPC-1.0.3.tar`

### file list

```diff
@@ -1,95 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.507128 HILO-MPC-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.495128 HILO-MPC-1.0.2/HILO_MPC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7187 2022-09-14 12:09:16.000000 HILO-MPC-1.0.2/HILO_MPC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2398 2022-09-14 12:09:16.000000 HILO-MPC-1.0.2/HILO_MPC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 12:09:16.000000 HILO-MPC-1.0.2/HILO_MPC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-09-14 12:09:16.000000 HILO-MPC-1.0.2/HILO_MPC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-14 12:09:16.000000 HILO-MPC-1.0.2/HILO_MPC.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7187 2022-09-14 12:09:16.507128 HILO-MPC-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5626 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.495128 HILO-MPC-1.0.2/hilo_mpc/
--rw-r--r--   0 runner    (1001) docker     (121)     4787 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.495128 HILO-MPC-1.0.2/hilo_mpc/library/
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8057 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/library/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.499127 HILO-MPC-1.0.2/hilo_mpc/modules/
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   139256 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    17859 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/control_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.499127 HILO-MPC-1.0.2/hilo_mpc/modules/controller/
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/controller/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     9894 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/controller/lqr.py
--rw-r--r--   0 runner    (1001) docker     (121)   101856 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/controller/mpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/controller/ocp.py
--rw-r--r--   0 runner    (1001) docker     (121)    11848 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/controller/pid.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.499127 HILO-MPC-1.0.2/hilo_mpc/modules/dynamic_model/
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/dynamic_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   164442 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/dynamic_model/dynamic_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.499127 HILO-MPC-1.0.2/hilo_mpc/modules/embedded/
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/embedded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6104 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/embedded/muaompc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.499127 HILO-MPC-1.0.2/hilo_mpc/modules/estimator/
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/estimator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11191 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/estimator/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    22167 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/estimator/kf.py
--rw-r--r--   0 runner    (1001) docker     (121)    54149 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/estimator/mhe.py
--rw-r--r--   0 runner    (1001) docker     (121)    15962 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/estimator/pf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.499127 HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4182 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.503128 HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/gp/
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    38432 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/gp/gp.py
--rw-r--r--   0 runner    (1001) docker     (121)     7155 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/gp/inference.py
--rw-r--r--   0 runner    (1001) docker     (121)    57048 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/gp/kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/gp/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)    23756 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/gp/mean.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.503128 HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/nn/
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12250 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/nn/layer.py
--rw-r--r--   0 runner    (1001) docker     (121)    17685 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/nn/nn.py
--rw-r--r--   0 runner    (1001) docker     (121)     2442 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/object.py
--rw-r--r--   0 runner    (1001) docker     (121)    61761 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/modules/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.503128 HILO-MPC-1.0.2/hilo_mpc/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.503128 HILO-MPC-1.0.2/hilo_mpc/plugins/bokeh/
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/plugins/bokeh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    39555 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/plugins/bokeh/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.503128 HILO-MPC-1.0.2/hilo_mpc/plugins/latex/
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/plugins/latex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/plugins/latex/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.503128 HILO-MPC-1.0.2/hilo_mpc/plugins/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (121)     1592 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/plugins/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34733 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/plugins/matplotlib/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     7249 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/plugins/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.503128 HILO-MPC-1.0.2/hilo_mpc/plugins/pytorch/
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/plugins/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22649 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/plugins/pytorch/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.503128 HILO-MPC-1.0.2/hilo_mpc/plugins/sklearn/
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/plugins/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/plugins/sklearn/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.503128 HILO-MPC-1.0.2/hilo_mpc/plugins/tensorboard/
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/plugins/tensorboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5970 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/plugins/tensorboard/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.507128 HILO-MPC-1.0.2/hilo_mpc/plugins/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/plugins/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15443 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/plugins/tensorflow/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:09:16.507128 HILO-MPC-1.0.2/hilo_mpc/util/
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    47044 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/util/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/util/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    16572 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/util/machine_learning.py
--rw-r--r--   0 runner    (1001) docker     (121)    44264 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/util/modeling.py
--rw-r--r--   0 runner    (1001) docker     (121)     9075 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/util/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)    18846 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/util/parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/util/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     9131 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/util/probability.py
--rw-r--r--   0 runner    (1001) docker     (121)     1936 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/util/session.py
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/util/unix.py
--rw-r--r--   0 runner    (1001) docker     (121)    20945 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/util/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     4514 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/hilo_mpc/util/windows.py
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-09-14 12:09:16.507128 HILO-MPC-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2143 2022-09-14 12:08:58.000000 HILO-MPC-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.576445 HILO-MPC-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.556443 HILO-MPC-1.0.3/HILO_MPC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-30 07:38:07.000000 HILO-MPC-1.0.3/HILO_MPC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-30 07:38:07.000000 HILO-MPC-1.0.3/HILO_MPC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 07:38:07.000000 HILO-MPC-1.0.3/HILO_MPC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-30 07:38:07.000000 HILO-MPC-1.0.3/HILO_MPC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-30 07:38:07.000000 HILO-MPC-1.0.3/HILO_MPC.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-30 07:38:07.576445 HILO-MPC-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.556443 HILO-MPC-1.0.3/hilo_mpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.556443 HILO-MPC-1.0.3/hilo_mpc/library/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/library/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.556443 HILO-MPC-1.0.3/hilo_mpc/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139256 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/control_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.560444 HILO-MPC-1.0.3/hilo_mpc/modules/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/controller/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/controller/lqr.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101976 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/controller/mpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/controller/ocp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/controller/pid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.560444 HILO-MPC-1.0.3/hilo_mpc/modules/dynamic_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/dynamic_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   164442 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/dynamic_model/dynamic_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.560444 HILO-MPC-1.0.3/hilo_mpc/modules/embedded/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/embedded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/embedded/muaompc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.560444 HILO-MPC-1.0.3/hilo_mpc/modules/estimator/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/estimator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/estimator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22167 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/estimator/kf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54149 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/estimator/mhe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15962 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/estimator/pf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.560444 HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.564444 HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/gp/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/gp/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57048 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/gp/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/gp/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23756 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/gp/mean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.564444 HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/nn/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17685 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/nn/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61761 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/modules/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.564444 HILO-MPC-1.0.3/hilo_mpc/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.564444 HILO-MPC-1.0.3/hilo_mpc/plugins/bokeh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/plugins/bokeh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39555 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/plugins/bokeh/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.568444 HILO-MPC-1.0.3/hilo_mpc/plugins/latex/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/plugins/latex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/plugins/latex/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.568444 HILO-MPC-1.0.3/hilo_mpc/plugins/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/plugins/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34733 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/plugins/matplotlib/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/plugins/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.568444 HILO-MPC-1.0.3/hilo_mpc/plugins/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/plugins/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22649 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/plugins/pytorch/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.568444 HILO-MPC-1.0.3/hilo_mpc/plugins/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/plugins/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/plugins/sklearn/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.568444 HILO-MPC-1.0.3/hilo_mpc/plugins/tensorboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/plugins/tensorboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/plugins/tensorboard/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.568444 HILO-MPC-1.0.3/hilo_mpc/plugins/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/plugins/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15443 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/plugins/tensorflow/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.572445 HILO-MPC-1.0.3/hilo_mpc/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47044 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/util/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16572 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/util/machine_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44264 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/util/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/util/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18846 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/util/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/util/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/util/probability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/util/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/util/unix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21484 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/hilo_mpc/util/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-30 07:38:07.576445 HILO-MPC-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:38:07.576445 HILO-MPC-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    41940 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/tests/test_GPs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24530 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/tests/test_KFs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/tests/test_LMPC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/tests/test_LQR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25709 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/tests/test_MHE.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97577 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/tests/test_NMPC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/tests/test_OCP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/tests/test_PFs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/tests/test_PID.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24611 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/tests/test_linear_systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/tests/test_linearization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-30 07:37:53.000000 HILO-MPC-1.0.3/tests/test_util_core.py
```

### Comparing `HILO-MPC-1.0.2/HILO_MPC.egg-info/PKG-INFO` & `HILO-MPC-1.0.3/HILO_MPC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HILO-MPC
-Version: 1.0.2
+Version: 1.0.3
 Summary: HILO-MPC is a toolbox for easy, flexible and fast development of machine-learning-supported optimal control and estimation problems
 Home-page: https://www.ccps.tu-darmstadt.de/research_ccps/hilo_mpc/
 Download-URL: https://github.com/hilo-mpc/hilo-mpc/releases
 Author: 
 Author-email: 
 Maintainer: HILO-MPC Developers
 Maintainer-email:
```

### Comparing `HILO-MPC-1.0.2/LICENSE` & `HILO-MPC-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/PKG-INFO` & `HILO-MPC-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HILO-MPC
-Version: 1.0.2
+Version: 1.0.3
 Summary: HILO-MPC is a toolbox for easy, flexible and fast development of machine-learning-supported optimal control and estimation problems
 Home-page: https://www.ccps.tu-darmstadt.de/research_ccps/hilo_mpc/
 Download-URL: https://github.com/hilo-mpc/hilo-mpc/releases
 Author: 
 Author-email: 
 Maintainer: HILO-MPC Developers
 Maintainer-email:
```

### Comparing `HILO-MPC-1.0.2/README.md` & `HILO-MPC-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/library/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/library/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/library/models.py` & `HILO-MPC-1.0.3/hilo_mpc/library/models.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/base.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/base.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/control_loop.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/control_loop.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/controller/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/controller/base.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/controller/base.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/controller/lqr.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/controller/lqr.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/controller/mpc.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/controller/mpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import casadi.tools as catools
 import numpy as np
 
 from .base import Controller
 from ..optimizer import DynamicOptimization
 from ...util.modeling import GenericCost, QuadraticCost, GenericConstraint, continuous2discrete
 from ...util.optimizer import IpoptDebugger
-from ...util.util import check_and_wrap_to_list, check_and_wrap_to_DM, scale_vector
+from ...util.util import check_and_wrap_to_list, check_and_wrap_to_DM, scale_vector, clip
 
 
 class NMPC(Controller, DynamicOptimization):
     """Class for Nonlinear Model Predictive Control"""
     def __init__(self, model, id=None, name=None, plot_backend=None, use_sx=True, stats=False):
         """Constructor method"""
         # TODO: when discrete_u or discrete_x is given to the opts structure, but NMPC is used, raise an error saying
@@ -713,21 +713,22 @@
                 self._v0 = sol['x']
         else:
             pert_factor = kwargs.get('pert_factor', 0.1)
             f_r_better = np.inf
             v00 = v0
             for r in range(runs):
                 sol = self._solver(x0=v00, lbx=self._v_lb, ubx=self._v_ub, lbg=self._g_lb, ubg=self._g_ub, p=param)
-                if sol['f'] < f_r_better:
+                self._solver_status_wrapper()
+                if self._solver_status_code in [1,2] and sol['f'] < f_r_better:
                     f_r_better = sol['f']
                     self._nlp_solution = sol
                     u_opt = sol['x'][self._u_ind[0]]
                     if self._nlp_options['warm_start']:
                         self._v0 = sol['x']
-                v00 = v0 + v0 * (1 - 2 * np.random.rand(self._n_v)) * pert_factor
+                v00 = clip(v0 + v0 * (1 - 2 * np.random.rand(self._n_v)) * pert_factor, self._v_lb, self._v_ub)
 
         return u_opt
 
     def optimize(self, x0, cp=None, tvp=None, v0=None, runs=0, fix_x0=True, **kwargs):
         """
         Solves the MPC problem
```

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/controller/ocp.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/controller/ocp.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/controller/pid.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/controller/pid.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/dynamic_model/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/dynamic_model/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/dynamic_model/dynamic_model.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/dynamic_model/dynamic_model.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/embedded/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/embedded/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/embedded/muaompc.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/embedded/muaompc.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/estimator/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/estimator/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/estimator/base.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/estimator/base.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/estimator/kf.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/estimator/kf.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/estimator/mhe.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/estimator/mhe.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/estimator/pf.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/estimator/pf.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/base.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/base.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/gp/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/gp/gp.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/gp/gp.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/gp/inference.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/gp/inference.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/gp/kernel.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/gp/kernel.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/gp/likelihood.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/gp/likelihood.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/gp/mean.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/gp/mean.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/nn/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/nn/layer.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/nn/layer.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/machine_learning/nn/nn.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/machine_learning/nn/nn.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/object.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/object.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/modules/optimizer.py` & `HILO-MPC-1.0.3/hilo_mpc/modules/optimizer.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/plugins/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/plugins/bokeh/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/plugins/bokeh/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/plugins/bokeh/plot.py` & `HILO-MPC-1.0.3/hilo_mpc/plugins/bokeh/plot.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/plugins/latex/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/plugins/latex/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/plugins/latex/plot.py` & `HILO-MPC-1.0.3/hilo_mpc/plugins/latex/plot.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/plugins/matplotlib/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/plugins/matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/plugins/matplotlib/plot.py` & `HILO-MPC-1.0.3/hilo_mpc/plugins/matplotlib/plot.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/plugins/plugins.py` & `HILO-MPC-1.0.3/hilo_mpc/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/plugins/pytorch/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/plugins/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/plugins/pytorch/wrapper.py` & `HILO-MPC-1.0.3/hilo_mpc/plugins/pytorch/wrapper.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/plugins/sklearn/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/plugins/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/plugins/sklearn/wrapper.py` & `HILO-MPC-1.0.3/hilo_mpc/plugins/sklearn/wrapper.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/plugins/tensorboard/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/plugins/tensorboard/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/plugins/tensorboard/wrapper.py` & `HILO-MPC-1.0.3/hilo_mpc/plugins/tensorboard/wrapper.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/plugins/tensorflow/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/plugins/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/plugins/tensorflow/wrapper.py` & `HILO-MPC-1.0.3/hilo_mpc/plugins/tensorflow/wrapper.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/util/__init__.py` & `HILO-MPC-1.0.3/hilo_mpc/util/__init__.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/util/data.py` & `HILO-MPC-1.0.3/hilo_mpc/util/data.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/util/io.py` & `HILO-MPC-1.0.3/hilo_mpc/util/io.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/util/machine_learning.py` & `HILO-MPC-1.0.3/hilo_mpc/util/machine_learning.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/util/modeling.py` & `HILO-MPC-1.0.3/hilo_mpc/util/modeling.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/util/optimizer.py` & `HILO-MPC-1.0.3/hilo_mpc/util/optimizer.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/util/parsing.py` & `HILO-MPC-1.0.3/hilo_mpc/util/parsing.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/util/plotting.py` & `HILO-MPC-1.0.3/hilo_mpc/util/plotting.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/util/probability.py` & `HILO-MPC-1.0.3/hilo_mpc/util/probability.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/util/session.py` & `HILO-MPC-1.0.3/hilo_mpc/util/session.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/util/unix.py` & `HILO-MPC-1.0.3/hilo_mpc/util/unix.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/hilo_mpc/util/util.py` & `HILO-MPC-1.0.3/hilo_mpc/util/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -712,7 +712,23 @@
 
 def who_am_i() -> str:
     """
 
     :return:
     """
     return sys._getframe(1).f_code.co_name
+
+
+def clip(v,v_lb,v_ub):
+    """
+    Given a vector v, it returns the value of the vector clipped between v_lb <= v <=v_ub
+    :param v: NP array, list or ca.DM vector
+    :param v_lb: NP array, list or ca.DM vector
+    :param v_ub: NP array, list or ca.DM vector
+    :return: clipped vector v (casadi DM)
+    """
+
+    v = check_and_wrap_to_list(v)
+    v_lb = check_and_wrap_to_list(v_lb)
+    v_ub = check_and_wrap_to_list(v_ub)
+
+    return ca.DM([v_lb[i] if v[i] < v_lb[i] else v_ub[i] if v[i] > v_ub[i] else v[i] for i in range(len(v))])
```

### Comparing `HILO-MPC-1.0.2/hilo_mpc/util/windows.py` & `HILO-MPC-1.0.3/hilo_mpc/util/windows.py`

 * *Files identical despite different names*

### Comparing `HILO-MPC-1.0.2/setup.cfg` & `HILO-MPC-1.0.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = HILO-MPC
-version = 1.0.2
+version = 1.0.3
 description = HILO-MPC is a toolbox for easy, flexible and fast development of machine-learning-supported optimal
 	control and estimation problems
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = 
 author_email = 
 maintainer = HILO-MPC Developers
```

### Comparing `HILO-MPC-1.0.2/setup.py` & `HILO-MPC-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     :return:
     """
     return open(os.path.join(os.path.dirname(__file__), file_name)).read()
 
 
 setup(
     name='HILO-MPC',
-    version='1.0.2',
+    version='1.0.3',
     description='HILO-MPC is a toolbox for easy, flexible and fast development of machine-learning-supported optimal '
                 'control and estimation problems',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     author='',
     author_email='',
     maintainer='HILO-MPC Developers',
```

