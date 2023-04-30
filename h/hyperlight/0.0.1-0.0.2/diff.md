# Comparing `tmp/hyperlight-0.0.1.tar.gz` & `tmp/hyperlight-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperlight-0.0.1.tar", max compression
+gzip compressed data, was "hyperlight-0.0.2.tar", max compression
```

## Comparing `hyperlight-0.0.1.tar` & `hyperlight-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2023-02-13 22:58:53.681101 hyperlight-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2023-02-13 22:58:53.681196 hyperlight-0.0.1/README.md
--rw-r--r--   0        0        0     2340 2023-02-13 22:58:53.681469 hyperlight-0.0.1/hyperlight/convert.py
--rw-r--r--   0        0        0      185 2023-02-13 22:58:53.681821 hyperlight-0.0.1/hyperlight/hyper/__init__.py
--rw-r--r--   0        0        0     4534 2023-02-13 22:58:53.682062 hyperlight-0.0.1/hyperlight/hyper/base.py
--rw-r--r--   0        0        0     1938 2023-02-13 22:58:53.682257 hyperlight-0.0.1/hyperlight/hyper/delta.py
--rw-r--r--   0        0        0     1092 2023-02-13 22:58:53.682525 hyperlight-0.0.1/hyperlight/hyper/encoder.py
--rw-r--r--   0        0        0     1065 2023-02-13 22:58:53.682721 hyperlight-0.0.1/hyperlight/hyper/hypermodule.py
--rw-r--r--   0        0        0      237 2023-02-13 22:58:53.682985 hyperlight-0.0.1/hyperlight/nn/__init__.py
--rw-r--r--   0        0        0     2328 2023-02-13 22:58:53.683172 hyperlight-0.0.1/hyperlight/nn/conv.py
--rw-r--r--   0        0        0      977 2023-02-13 22:58:53.683353 hyperlight-0.0.1/hyperlight/nn/linear.py
--rw-r--r--   0        0        0     3830 2023-02-13 22:58:53.683563 hyperlight-0.0.1/hyperlight/nn/voidmodule.py
--rw-r--r--   0        0        0     1139 2023-02-13 22:58:53.683743 hyperlight-0.0.1/hyperlight/nn/xparam.py
--rw-r--r--   0        0        0     1748 2023-02-13 23:02:05.543034 hyperlight-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 hyperlight-0.0.1/setup.py
--rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 hyperlight-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-04-30 17:07:30.205256 hyperlight-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3789 2023-04-30 17:51:10.782753 hyperlight-0.0.2/README.md
+-rw-r--r--   0        0        0      180 2023-04-30 18:14:38.420816 hyperlight-0.0.2/hyperlight/__init__.py
+-rw-r--r--   0        0        0     6320 2023-04-30 17:16:14.247970 hyperlight-0.0.2/hyperlight/convert.py
+-rw-r--r--   0        0        0     4117 2023-04-30 17:16:00.075788 hyperlight-0.0.2/hyperlight/find.py
+-rw-r--r--   0        0        0       43 2023-04-30 17:07:30.229256 hyperlight-0.0.2/hyperlight/hypernet/__init__.py
+-rw-r--r--   0        0        0     1475 2023-04-30 17:07:30.233256 hyperlight-0.0.2/hyperlight/hypernet/encoding.py
+-rw-r--r--   0        0        0     3624 2023-04-30 17:07:30.237256 hyperlight-0.0.2/hyperlight/hypernet/initialization.py
+-rw-r--r--   0        0        0    12406 2023-04-30 17:20:04.258919 hyperlight-0.0.2/hyperlight/hypernet/model.py
+-rw-r--r--   0        0        0      141 2023-04-30 17:07:30.241256 hyperlight-0.0.2/hyperlight/nn/__init__.py
+-rw-r--r--   0        0        0      566 2023-04-30 17:07:30.245257 hyperlight-0.0.2/hyperlight/nn/container.py
+-rw-r--r--   0        0        0     3888 2023-04-30 17:07:30.245257 hyperlight-0.0.2/hyperlight/nn/layers.py
+-rw-r--r--   0        0        0     9388 2023-04-30 17:07:30.249256 hyperlight-0.0.2/hyperlight/nn/module.py
+-rw-r--r--   0        0        0     4446 2023-04-30 17:07:30.253257 hyperlight-0.0.2/hyperlight/nn/xparam.py
+-rw-r--r--   0        0        0     1420 2023-04-30 18:44:03.807500 hyperlight-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4841 1970-01-01 00:00:00.000000 hyperlight-0.0.2/PKG-INFO
```

