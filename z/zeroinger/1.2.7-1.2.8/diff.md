# Comparing `tmp/zeroinger-1.2.7.tar.gz` & `tmp/zeroinger-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroinger-1.2.7.tar", last modified: Tue Apr 19 07:44:08 2022, max compression
+gzip compressed data, was "zeroinger-1.2.8.tar", last modified: Sun Apr 30 09:35:17 2023, max compression
```

## Comparing `zeroinger-1.2.7.tar` & `zeroinger-1.2.8.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2022-04-19 07:44:08.078429 zeroinger-1.2.7/
--rw-r--r--   0 liangjz    (502) staff       (20)     1060 2022-04-19 07:26:25.000000 zeroinger-1.2.7/LICENSE
--rw-r--r--   0 liangjz    (502) staff       (20)      166 2022-04-19 07:26:25.000000 zeroinger-1.2.7/MANIFEST.in
--rw-r--r--   0 liangjz    (502) staff       (20)     2452 2022-04-19 07:44:08.078039 zeroinger-1.2.7/PKG-INFO
--rw-r--r--   0 liangjz    (502) staff       (20)     1793 2022-04-19 07:26:25.000000 zeroinger-1.2.7/README.md
--rw-r--r--   0 liangjz    (502) staff       (20)       38 2022-04-19 07:44:08.078525 zeroinger-1.2.7/setup.cfg
--rw-r--r--   0 liangjz    (502) staff       (20)     3880 2022-04-19 07:43:47.000000 zeroinger-1.2.7/setup.py
-drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2022-04-19 07:44:08.027585 zeroinger-1.2.7/test/
-drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2022-04-19 07:44:08.031480 zeroinger-1.2.7/test/excel/
--rw-r--r--   0 liangjz    (502) staff       (20)        0 2022-04-19 07:26:25.000000 zeroinger-1.2.7/test/excel/__init__.py
--rw-r--r--   0 liangjz    (502) staff       (20)     1358 2022-04-19 07:26:25.000000 zeroinger-1.2.7/test/excel/test_XLSX.py
-drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2022-04-19 07:44:08.032204 zeroinger-1.2.7/test/pca/
--rw-r--r--   0 liangjz    (502) staff       (20)        0 2022-04-19 07:26:25.000000 zeroinger-1.2.7/test/pca/__init__.py
--rw-r--r--   0 liangjz    (502) staff       (20)     1576 2022-04-19 07:26:25.000000 zeroinger-1.2.7/test/pca/test_matcher.py
-drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2022-04-19 07:44:08.033754 zeroinger-1.2.7/test/time/
--rw-r--r--   0 liangjz    (502) staff       (20)        0 2022-04-19 07:26:25.000000 zeroinger-1.2.7/test/time/__init__.py
--rw-r--r--   0 liangjz    (502) staff       (20)      377 2022-04-19 07:26:25.000000 zeroinger-1.2.7/test/time/test_counter.py
--rw-r--r--   0 liangjz    (502) staff       (20)     2066 2022-04-19 07:26:25.000000 zeroinger-1.2.7/test/time/test_dateUtils.py
--rw-r--r--   0 liangjz    (502) staff       (20)      609 2022-04-19 07:26:25.000000 zeroinger-1.2.7/test/time/test_stopwatch.py
-drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2022-04-19 07:44:08.034573 zeroinger-1.2.7/zeroinger/
--rw-r--r--   0 liangjz    (502) staff       (20)      529 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/__init__.py
--rw-r--r--   0 liangjz    (502) staff       (20)      352 2022-04-19 07:43:58.000000 zeroinger-1.2.7/zeroinger/__version__.py
-drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2022-04-19 07:44:08.037513 zeroinger-1.2.7/zeroinger/compression/
--rw-r--r--   0 liangjz    (502) staff       (20)        0 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/compression/__init__.py
--rw-r--r--   0 liangjz    (502) staff       (20)      995 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/compression/abs_cfu.py
--rw-r--r--   0 liangjz    (502) staff       (20)     1231 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/compression/cfu_7z.py
-drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2022-04-19 07:44:08.038609 zeroinger-1.2.7/zeroinger/config/
--rw-r--r--   0 liangjz    (502) staff       (20)       81 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/config/__init__.py
--rw-r--r--   0 liangjz    (502) staff       (20)      995 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/config/config_parser_util.py
-drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2022-04-19 07:44:08.039843 zeroinger-1.2.7/zeroinger/excel/
--rw-r--r--   0 liangjz    (502) staff       (20)       67 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/excel/__init__.py
--rw-r--r--   0 liangjz    (502) staff       (20)     5814 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/excel/csv.py
--rw-r--r--   0 liangjz    (502) staff       (20)     1845 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/excel/xlsx.py
-drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2022-04-19 07:44:08.040686 zeroinger-1.2.7/zeroinger/file/
--rw-r--r--   0 liangjz    (502) staff       (20)       70 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/file/__init__.py
--rw-r--r--   0 liangjz    (502) staff       (20)      704 2022-04-19 07:33:42.000000 zeroinger-1.2.7/zeroinger/file/path_util.py
-drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2022-04-19 07:44:08.042176 zeroinger-1.2.7/zeroinger/msg/
--rw-r--r--   0 liangjz    (502) staff       (20)      103 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/msg/__init__.py
--rw-r--r--   0 liangjz    (502) staff       (20)     1016 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/msg/ding.py
--rw-r--r--   0 liangjz    (502) staff       (20)     5314 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/msg/feishu.py
-drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2022-04-19 07:44:08.073030 zeroinger-1.2.7/zeroinger/pca/
--rw-r--r--   0 liangjz    (502) staff       (20)      123 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/pca/__init__.py
--rw-r--r--   0 liangjz    (502) staff       (20)    83223 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/pca/adcode.tsv
--rw-r--r--   0 liangjz    (502) staff       (20)     4872 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/pca/adcode_loader.py
--rw-r--r--   0 liangjz    (502) staff       (20)     3564 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/pca/alias_builder.py
--rw-r--r--   0 liangjz    (502) staff       (20)     2373 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/pca/area.py
--rw-r--r--   0 liangjz    (502) staff       (20)  9972187 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/pca/area2street_village.json
--rw-r--r--   0 liangjz    (502) staff       (20)     9794 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/pca/matcher.py
--rw-r--r--   0 liangjz    (502) staff       (20)      909 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/pca/nations.txt
--rw-r--r--   0 liangjz    (502) staff       (20)     2286 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/pca/script_gen_area2street_village.py
-drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2022-04-19 07:44:08.074880 zeroinger-1.2.7/zeroinger/text/
--rw-r--r--   0 liangjz    (502) staff       (20)      103 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/text/__init__.py
--rw-r--r--   0 liangjz    (502) staff       (20)      323 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/text/string.py
--rw-r--r--   0 liangjz    (502) staff       (20)     2083 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/text/text_file.py
-drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2022-04-19 07:44:08.077360 zeroinger-1.2.7/zeroinger/time/
--rw-r--r--   0 liangjz    (502) staff       (20)      138 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/time/__init__.py
--rw-r--r--   0 liangjz    (502) staff       (20)      882 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/time/counter.py
--rw-r--r--   0 liangjz    (502) staff       (20)     3985 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/time/dateutils.py
--rw-r--r--   0 liangjz    (502) staff       (20)     1260 2022-04-19 07:26:25.000000 zeroinger-1.2.7/zeroinger/time/stopwatch.py
-drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2022-04-19 07:44:08.036297 zeroinger-1.2.7/zeroinger.egg-info/
--rw-r--r--   0 liangjz    (502) staff       (20)     2452 2022-04-19 07:44:07.000000 zeroinger-1.2.7/zeroinger.egg-info/PKG-INFO
--rw-r--r--   0 liangjz    (502) staff       (20)     1277 2022-04-19 07:44:08.000000 zeroinger-1.2.7/zeroinger.egg-info/SOURCES.txt
--rw-r--r--   0 liangjz    (502) staff       (20)        1 2022-04-19 07:44:07.000000 zeroinger-1.2.7/zeroinger.egg-info/dependency_links.txt
--rw-r--r--   0 liangjz    (502) staff       (20)      101 2022-04-19 07:44:07.000000 zeroinger-1.2.7/zeroinger.egg-info/requires.txt
--rw-r--r--   0 liangjz    (502) staff       (20)       15 2022-04-19 07:44:07.000000 zeroinger-1.2.7/zeroinger.egg-info/top_level.txt
+drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2023-04-30 09:35:17.830120 zeroinger-1.2.8/
+-rw-r--r--   0 liangjz    (502) staff       (20)     1060 2022-04-19 07:26:25.000000 zeroinger-1.2.8/LICENSE
+-rw-r--r--   0 liangjz    (502) staff       (20)      166 2022-04-19 07:26:25.000000 zeroinger-1.2.8/MANIFEST.in
+-rw-r--r--   0 liangjz    (502) staff       (20)     2452 2023-04-30 09:35:17.829406 zeroinger-1.2.8/PKG-INFO
+-rw-r--r--   0 liangjz    (502) staff       (20)     1793 2022-04-19 07:26:25.000000 zeroinger-1.2.8/README.md
+-rw-r--r--   0 liangjz    (502) staff       (20)       38 2023-04-30 09:35:17.830304 zeroinger-1.2.8/setup.cfg
+-rw-r--r--   0 liangjz    (502) staff       (20)     3932 2023-04-30 09:31:51.000000 zeroinger-1.2.8/setup.py
+drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2023-04-30 09:35:17.754460 zeroinger-1.2.8/test/
+drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2023-04-30 09:35:17.762766 zeroinger-1.2.8/test/excel/
+-rw-r--r--   0 liangjz    (502) staff       (20)        0 2022-04-19 07:26:25.000000 zeroinger-1.2.8/test/excel/__init__.py
+-rw-r--r--   0 liangjz    (502) staff       (20)     1358 2022-04-19 07:26:25.000000 zeroinger-1.2.8/test/excel/test_XLSX.py
+drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2023-04-30 09:35:17.764665 zeroinger-1.2.8/test/pca/
+-rw-r--r--   0 liangjz    (502) staff       (20)        0 2022-04-19 07:26:25.000000 zeroinger-1.2.8/test/pca/__init__.py
+-rw-r--r--   0 liangjz    (502) staff       (20)     1576 2022-04-19 07:26:25.000000 zeroinger-1.2.8/test/pca/test_matcher.py
+drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2023-04-30 09:35:17.769207 zeroinger-1.2.8/test/time/
+-rw-r--r--   0 liangjz    (502) staff       (20)        0 2022-04-19 07:26:25.000000 zeroinger-1.2.8/test/time/__init__.py
+-rw-r--r--   0 liangjz    (502) staff       (20)      377 2022-04-19 07:26:25.000000 zeroinger-1.2.8/test/time/test_counter.py
+-rw-r--r--   0 liangjz    (502) staff       (20)     2066 2022-04-19 07:26:25.000000 zeroinger-1.2.8/test/time/test_dateUtils.py
+-rw-r--r--   0 liangjz    (502) staff       (20)      609 2022-04-19 07:26:25.000000 zeroinger-1.2.8/test/time/test_stopwatch.py
+drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2023-04-30 09:35:17.771218 zeroinger-1.2.8/zeroinger/
+-rw-r--r--   0 liangjz    (502) staff       (20)      529 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/__init__.py
+-rw-r--r--   0 liangjz    (502) staff       (20)      352 2023-04-30 09:32:54.000000 zeroinger-1.2.8/zeroinger/__version__.py
+drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2023-04-30 09:35:17.776784 zeroinger-1.2.8/zeroinger/compression/
+-rw-r--r--   0 liangjz    (502) staff       (20)        0 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/compression/__init__.py
+-rw-r--r--   0 liangjz    (502) staff       (20)      995 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/compression/abs_cfu.py
+-rw-r--r--   0 liangjz    (502) staff       (20)     1231 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/compression/cfu_7z.py
+drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2023-04-30 09:35:17.779363 zeroinger-1.2.8/zeroinger/config/
+-rw-r--r--   0 liangjz    (502) staff       (20)       81 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/config/__init__.py
+-rw-r--r--   0 liangjz    (502) staff       (20)      995 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/config/config_parser_util.py
+drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2023-04-30 09:35:17.782634 zeroinger-1.2.8/zeroinger/excel/
+-rw-r--r--   0 liangjz    (502) staff       (20)       67 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/excel/__init__.py
+-rw-r--r--   0 liangjz    (502) staff       (20)     5814 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/excel/csv.py
+-rw-r--r--   0 liangjz    (502) staff       (20)     1845 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/excel/xlsx.py
+drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2023-04-30 09:35:17.785498 zeroinger-1.2.8/zeroinger/file/
+-rw-r--r--   0 liangjz    (502) staff       (20)       70 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/file/__init__.py
+-rw-r--r--   0 liangjz    (502) staff       (20)      704 2022-04-19 07:33:42.000000 zeroinger-1.2.8/zeroinger/file/path_util.py
+drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2023-04-30 09:35:17.789116 zeroinger-1.2.8/zeroinger/msg/
+-rw-r--r--   0 liangjz    (502) staff       (20)      103 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/msg/__init__.py
+-rw-r--r--   0 liangjz    (502) staff       (20)     1016 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/msg/ding.py
+-rw-r--r--   0 liangjz    (502) staff       (20)     5314 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/msg/feishu.py
+drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2023-04-30 09:35:17.822379 zeroinger-1.2.8/zeroinger/pca/
+-rw-r--r--   0 liangjz    (502) staff       (20)      123 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/pca/__init__.py
+-rw-r--r--   0 liangjz    (502) staff       (20)    83223 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/pca/adcode.tsv
+-rw-r--r--   0 liangjz    (502) staff       (20)     4872 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/pca/adcode_loader.py
+-rw-r--r--   0 liangjz    (502) staff       (20)     3564 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/pca/alias_builder.py
+-rw-r--r--   0 liangjz    (502) staff       (20)     2373 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/pca/area.py
+-rw-r--r--   0 liangjz    (502) staff       (20)  9972187 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/pca/area2street_village.json
+-rw-r--r--   0 liangjz    (502) staff       (20)     9794 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/pca/matcher.py
+-rw-r--r--   0 liangjz    (502) staff       (20)      909 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/pca/nations.txt
+-rw-r--r--   0 liangjz    (502) staff       (20)     2286 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/pca/script_gen_area2street_village.py
+drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2023-04-30 09:35:17.824886 zeroinger-1.2.8/zeroinger/text/
+-rw-r--r--   0 liangjz    (502) staff       (20)      103 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/text/__init__.py
+-rw-r--r--   0 liangjz    (502) staff       (20)      323 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/text/string.py
+-rw-r--r--   0 liangjz    (502) staff       (20)     2083 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/text/text_file.py
+drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2023-04-30 09:35:17.828170 zeroinger-1.2.8/zeroinger/time/
+-rw-r--r--   0 liangjz    (502) staff       (20)      138 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/time/__init__.py
+-rw-r--r--   0 liangjz    (502) staff       (20)      882 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/time/counter.py
+-rw-r--r--   0 liangjz    (502) staff       (20)     3985 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/time/dateutils.py
+-rw-r--r--   0 liangjz    (502) staff       (20)     1260 2022-04-19 07:26:25.000000 zeroinger-1.2.8/zeroinger/time/stopwatch.py
+drwxr-xr-x   0 liangjz    (502) staff       (20)        0 2023-04-30 09:35:17.774298 zeroinger-1.2.8/zeroinger.egg-info/
+-rw-r--r--   0 liangjz    (502) staff       (20)     2452 2023-04-30 09:35:17.000000 zeroinger-1.2.8/zeroinger.egg-info/PKG-INFO
+-rw-r--r--   0 liangjz    (502) staff       (20)     1277 2023-04-30 09:35:17.000000 zeroinger-1.2.8/zeroinger.egg-info/SOURCES.txt
+-rw-r--r--   0 liangjz    (502) staff       (20)        1 2023-04-30 09:35:17.000000 zeroinger-1.2.8/zeroinger.egg-info/dependency_links.txt
+-rw-r--r--   0 liangjz    (502) staff       (20)      113 2023-04-30 09:35:17.000000 zeroinger-1.2.8/zeroinger.egg-info/requires.txt
+-rw-r--r--   0 liangjz    (502) staff       (20)       15 2023-04-30 09:35:17.000000 zeroinger-1.2.8/zeroinger.egg-info/top_level.txt
```

### Comparing `zeroinger-1.2.7/LICENSE` & `zeroinger-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/PKG-INFO` & `zeroinger-1.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroinger
-Version: 1.2.7
+Version: 1.2.8
 Summary: group of tools for data process
 Home-page: https://github.com/liangjz92/zeroinger-utils
 Author: liangjz
 Author-email: liangjianzeng@qq.com   
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zeroinger-1.2.7/README.md` & `zeroinger-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/setup.py` & `zeroinger-1.2.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,25 @@
 AUTHOR = 'liangjz'
 REQUIRES_PYTHON = '>=3.6.0'
 VERSION = None
 include_package_data = True
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    'requests', 'logzero', 'arrow', 'configparser', 'requests', 'pyexcel', 'pyahocorasick', 'arrow',
-    'dataclasses','python-dateutil'
+    'requests',
+    'logzero',
+    'arrow',
+    'configparser',
+    'requests',
+    'pyexcel',
+    'pyahocorasick',
+    'arrow',
+    'dataclasses',
+    'python-dateutil',
+    'xlrd<=1.2.0'
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

### Comparing `zeroinger-1.2.7/test/excel/test_XLSX.py` & `zeroinger-1.2.8/test/excel/test_XLSX.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/test/pca/test_matcher.py` & `zeroinger-1.2.8/test/pca/test_matcher.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/test/time/test_dateUtils.py` & `zeroinger-1.2.8/test/time/test_dateUtils.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/test/time/test_stopwatch.py` & `zeroinger-1.2.8/test/time/test_stopwatch.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/__init__.py` & `zeroinger-1.2.8/zeroinger/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/compression/abs_cfu.py` & `zeroinger-1.2.8/zeroinger/compression/abs_cfu.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/compression/cfu_7z.py` & `zeroinger-1.2.8/zeroinger/compression/cfu_7z.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/config/config_parser_util.py` & `zeroinger-1.2.8/zeroinger/config/config_parser_util.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/excel/csv.py` & `zeroinger-1.2.8/zeroinger/excel/csv.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/excel/xlsx.py` & `zeroinger-1.2.8/zeroinger/excel/xlsx.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/file/path_util.py` & `zeroinger-1.2.8/zeroinger/file/path_util.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/msg/ding.py` & `zeroinger-1.2.8/zeroinger/msg/ding.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/msg/feishu.py` & `zeroinger-1.2.8/zeroinger/msg/feishu.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/pca/adcode.tsv` & `zeroinger-1.2.8/zeroinger/pca/adcode.tsv`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/pca/adcode_loader.py` & `zeroinger-1.2.8/zeroinger/pca/adcode_loader.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/pca/alias_builder.py` & `zeroinger-1.2.8/zeroinger/pca/alias_builder.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/pca/area.py` & `zeroinger-1.2.8/zeroinger/pca/area.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/pca/area2street_village.json` & `zeroinger-1.2.8/zeroinger/pca/area2street_village.json`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/pca/matcher.py` & `zeroinger-1.2.8/zeroinger/pca/matcher.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/pca/nations.txt` & `zeroinger-1.2.8/zeroinger/pca/nations.txt`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/pca/script_gen_area2street_village.py` & `zeroinger-1.2.8/zeroinger/pca/script_gen_area2street_village.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/text/text_file.py` & `zeroinger-1.2.8/zeroinger/text/text_file.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/time/counter.py` & `zeroinger-1.2.8/zeroinger/time/counter.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/time/dateutils.py` & `zeroinger-1.2.8/zeroinger/time/dateutils.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger/time/stopwatch.py` & `zeroinger-1.2.8/zeroinger/time/stopwatch.py`

 * *Files identical despite different names*

### Comparing `zeroinger-1.2.7/zeroinger.egg-info/PKG-INFO` & `zeroinger-1.2.8/zeroinger.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroinger
-Version: 1.2.7
+Version: 1.2.8
 Summary: group of tools for data process
 Home-page: https://github.com/liangjz92/zeroinger-utils
 Author: liangjz
 Author-email: liangjianzeng@qq.com   
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zeroinger-1.2.7/zeroinger.egg-info/SOURCES.txt` & `zeroinger-1.2.8/zeroinger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

