# Comparing `tmp/bulk-mv-0.1.3.tar.gz` & `tmp/bulk-mv-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulk-mv-0.1.3.tar", last modified: Tue Apr  4 03:04:27 2023, max compression
+gzip compressed data, was "bulk-mv-0.1.4.tar", last modified: Sun Apr 30 01:50:47 2023, max compression
```

## Comparing `bulk-mv-0.1.3.tar` & `bulk-mv-0.1.4.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:27.000732 bulk-mv-0.1.3/
--rw-r--r--   0 garcia     (501) staff       (20)      503 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/.bumpversion.cfg
--rw-r--r--   0 garcia     (501) staff       (20)     1030 2023-03-23 02:09:51.000000 bulk-mv-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 garcia     (501) staff       (20)    11357 2023-03-20 19:12:19.000000 bulk-mv-0.1.3/LICENSE
--rw-r--r--   0 garcia     (501) staff       (20)      535 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/MANIFEST.in
--rw-r--r--   0 garcia     (501) staff       (20)     2204 2023-03-23 02:47:16.000000 bulk-mv-0.1.3/Makefile
--rw-r--r--   0 garcia     (501) staff       (20)    18864 2023-04-04 03:04:27.000344 bulk-mv-0.1.3/PKG-INFO
--rw-r--r--   0 garcia     (501) staff       (20)     5030 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/README.md
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.967301 bulk-mv-0.1.3/branding/
--rw-r--r--   0 garcia     (501) staff       (20)   246902 2023-04-03 14:39:52.000000 bulk-mv-0.1.3/branding/logo.png
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.974676 bulk-mv-0.1.3/bulk_mv/
--rw-r--r--   0 garcia     (501) staff       (20)      316 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/bulk_mv/__init__.py
--rw-r--r--   0 garcia     (501) staff       (20)      144 2023-04-03 01:23:55.000000 bulk-mv-0.1.3/bulk_mv/__main__.py
--rw-r--r--   0 garcia     (501) staff       (20)      670 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/bulk_mv/bmv.lark
--rw-r--r--   0 garcia     (501) staff       (20)      865 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/bulk_mv/bmv_generator.py
--rw-r--r--   0 garcia     (501) staff       (20)    11035 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/bulk_mv/bmv_parser.py
--rw-r--r--   0 garcia     (501) staff       (20)     1008 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/bulk_mv/cli.py
--rw-r--r--   0 garcia     (501) staff       (20)     3378 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/bulk_mv/file_tree.py
--rw-r--r--   0 garcia     (501) staff       (20)      968 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/bulk_mv/file_tree_builder.py
--rw-r--r--   0 garcia     (501) staff       (20)      559 2023-04-03 14:39:52.000000 bulk-mv-0.1.3/bulk_mv/helpers.py
--rw-r--r--   0 garcia     (501) staff       (20)     1819 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/bulk_mv/operations.py
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.983484 bulk-mv-0.1.3/bulk_mv/tests/
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.985326 bulk-mv-0.1.3/bulk_mv/tests/dummy_bmv_files/
--rw-r--r--   0 garcia     (501) staff       (20)      288 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_bmv_files/sample1.bmv
--rw-r--r--   0 garcia     (501) staff       (20)      246 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_bmv_files/sample3.bmv
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.959834 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.986131 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample1/
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.987221 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample1/admin/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:36:22.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample1/admin/index.html
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:36:18.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample1/admin/nichoal.html
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample1/index.html
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.989135 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample1/users/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:35:17.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample1/users/angel.html
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.989675 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample1/users/blocked/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample1/users/blocked/blocked_user_1.html
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:35:38.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample1/users/index.html
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:35:59.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample1/users/josh.html
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.991651 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample2/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:37:58.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample2/a.txt
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:01.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample2/b.txt
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:05.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample2/c.txt
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.992049 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample2/data/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:37.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample2/data/report.csv
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:49.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample2/readme.md
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.993378 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample2/web/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:15.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample2/web/index.html
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:21.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample2/web/main.css
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:19.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample2/web/main.js
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.960722 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample3/
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.993687 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample3/delete/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample3/delete/no_more.html
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.994543 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample3/markdown/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 01:41:20.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample3/markdown/1.md
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 01:59:35.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample3/markdown/2.md
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.994971 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample3/photos/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 01:41:20.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample3/photos/test.jpg
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.995998 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample3/text/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-23 01:36:28.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample3/text/1.txt
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 02:57:45.000000 bulk-mv-0.1.3/bulk_mv/tests/dummy_directories/sample3/text/2.txt
--rw-r--r--   0 garcia     (501) staff       (20)      935 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/bulk_mv/tests/test_bmv_generator.py
--rw-r--r--   0 garcia     (501) staff       (20)     1160 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/bulk_mv/tests/test_bmv_parser.py
--rw-r--r--   0 garcia     (501) staff       (20)     4243 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/bulk_mv/tests/test_file_tree.py
--rw-r--r--   0 garcia     (501) staff       (20)     1116 2023-03-23 02:03:19.000000 bulk-mv-0.1.3/bulk_mv/tests/test_file_tree_builder.py
--rw-r--r--   0 garcia     (501) staff       (20)      676 2023-04-04 01:50:14.000000 bulk-mv-0.1.3/bulk_mv/tests/test_helpers.py
--rw-r--r--   0 garcia     (501) staff       (20)     1996 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/bulk_mv/tests/test_operations.py
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.979070 bulk-mv-0.1.3/bulk_mv.egg-info/
--rw-r--r--   0 garcia     (501) staff       (20)    18864 2023-04-04 03:04:26.000000 bulk-mv-0.1.3/bulk_mv.egg-info/PKG-INFO
--rw-r--r--   0 garcia     (501) staff       (20)     2036 2023-04-04 03:04:26.000000 bulk-mv-0.1.3/bulk_mv.egg-info/SOURCES.txt
--rw-r--r--   0 garcia     (501) staff       (20)        1 2023-04-04 03:04:26.000000 bulk-mv-0.1.3/bulk_mv.egg-info/dependency_links.txt
--rw-r--r--   0 garcia     (501) staff       (20)       46 2023-04-04 03:04:26.000000 bulk-mv-0.1.3/bulk_mv.egg-info/entry_points.txt
--rw-r--r--   0 garcia     (501) staff       (20)      161 2023-04-04 03:04:26.000000 bulk-mv-0.1.3/bulk_mv.egg-info/requires.txt
--rw-r--r--   0 garcia     (501) staff       (20)        8 2023-04-04 03:04:26.000000 bulk-mv-0.1.3/bulk_mv.egg-info/top_level.txt
--rw-r--r--   0 garcia     (501) staff       (20)      115 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/codecov.yml
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-04 03:04:26.999625 bulk-mv-0.1.3/doc/
--rw-r--r--   0 garcia     (501) staff       (20)      634 2023-04-03 14:39:52.000000 bulk-mv-0.1.3/doc/Makefile
--rw-r--r--   0 garcia     (501) staff       (20)     1191 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/doc/bulk_mv.rst
--rw-r--r--   0 garcia     (501) staff       (20)     1109 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/doc/conf.py
--rw-r--r--   0 garcia     (501) staff       (20)      448 2023-04-03 14:39:52.000000 bulk-mv-0.1.3/doc/index.rst
--rw-r--r--   0 garcia     (501) staff       (20)      765 2023-04-03 14:39:52.000000 bulk-mv-0.1.3/doc/make.bat
--rw-r--r--   0 garcia     (501) staff       (20)       58 2023-04-03 14:39:52.000000 bulk-mv-0.1.3/doc/modules.rst
--rw-r--r--   0 garcia     (501) staff       (20)     2240 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/pyproject.toml
--rw-r--r--   0 garcia     (501) staff       (20)       38 2023-04-04 03:04:27.000862 bulk-mv-0.1.3/setup.cfg
--rw-r--r--   0 garcia     (501) staff       (20)      521 2023-04-04 02:58:22.000000 bulk-mv-0.1.3/setup.py
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.279064 bulk-mv-0.1.4/
+-rw-r--r--   0 garcia     (501) staff       (20)      503 2023-04-30 01:44:40.000000 bulk-mv-0.1.4/.bumpversion.cfg
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 20:25:34.000000 bulk-mv-0.1.4/.nojekyll
+-rw-r--r--   0 garcia     (501) staff       (20)     1030 2023-04-07 16:09:06.000000 bulk-mv-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0 garcia     (501) staff       (20)    11357 2023-03-20 19:12:19.000000 bulk-mv-0.1.4/LICENSE
+-rw-r--r--   0 garcia     (501) staff       (20)      553 2023-04-04 20:27:21.000000 bulk-mv-0.1.4/MANIFEST.in
+-rw-r--r--   0 garcia     (501) staff       (20)     2521 2023-04-04 20:32:28.000000 bulk-mv-0.1.4/Makefile
+-rw-r--r--   0 garcia     (501) staff       (20)    19287 2023-04-30 01:50:47.278253 bulk-mv-0.1.4/PKG-INFO
+-rw-r--r--   0 garcia     (501) staff       (20)     5454 2023-04-17 18:36:32.000000 bulk-mv-0.1.4/README.md
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.251062 bulk-mv-0.1.4/branding/
+-rw-r--r--   0 garcia     (501) staff       (20)   246902 2023-04-03 14:39:52.000000 bulk-mv-0.1.4/branding/logo.png
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.255861 bulk-mv-0.1.4/bulk_mv/
+-rw-r--r--   0 garcia     (501) staff       (20)      316 2023-04-30 01:44:40.000000 bulk-mv-0.1.4/bulk_mv/__init__.py
+-rw-r--r--   0 garcia     (501) staff       (20)      144 2023-04-03 01:23:55.000000 bulk-mv-0.1.4/bulk_mv/__main__.py
+-rw-r--r--   0 garcia     (501) staff       (20)      670 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/bulk_mv/bmv.lark
+-rw-r--r--   0 garcia     (501) staff       (20)      865 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/bulk_mv/bmv_generator.py
+-rw-r--r--   0 garcia     (501) staff       (20)    11035 2023-04-30 01:42:58.000000 bulk-mv-0.1.4/bulk_mv/bmv_parser.py
+-rw-r--r--   0 garcia     (501) staff       (20)     1008 2023-04-30 01:42:58.000000 bulk-mv-0.1.4/bulk_mv/cli.py
+-rw-r--r--   0 garcia     (501) staff       (20)     3378 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/bulk_mv/file_tree.py
+-rw-r--r--   0 garcia     (501) staff       (20)      968 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/bulk_mv/file_tree_builder.py
+-rw-r--r--   0 garcia     (501) staff       (20)      559 2023-04-03 14:39:52.000000 bulk-mv-0.1.4/bulk_mv/helpers.py
+-rw-r--r--   0 garcia     (501) staff       (20)     1819 2023-04-30 01:42:58.000000 bulk-mv-0.1.4/bulk_mv/operations.py
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.263760 bulk-mv-0.1.4/bulk_mv/tests/
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.265336 bulk-mv-0.1.4/bulk_mv/tests/dummy_bmv_files/
+-rw-r--r--   0 garcia     (501) staff       (20)      288 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_bmv_files/sample1.bmv
+-rw-r--r--   0 garcia     (501) staff       (20)      246 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_bmv_files/sample3.bmv
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.244682 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.265905 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.266678 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/admin/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:36:22.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/admin/index.html
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:36:18.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/admin/nichoal.html
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/index.html
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.267807 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/users/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:35:17.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/users/angel.html
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.268197 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/users/blocked/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/users/blocked/blocked_user_1.html
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:35:38.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/users/index.html
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:35:59.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/users/josh.html
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.269724 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:37:58.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/a.txt
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:01.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/b.txt
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:05.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/c.txt
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.270108 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/data/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:37.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/data/report.csv
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:49.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/readme.md
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.271280 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/web/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:15.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/web/index.html
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:21.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/web/main.css
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:19.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/web/main.js
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.245830 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.271652 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/delete/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-30 01:37:16.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/delete/no_more.html
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.272398 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/markdown/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 01:41:20.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/markdown/1.md
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-30 01:37:16.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/markdown/2.md
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.272934 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/photos/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 01:41:20.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/photos/test.jpg
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.273689 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/text/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-23 01:36:28.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/text/1.txt
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 02:57:45.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/text/2.txt
+-rw-r--r--   0 garcia     (501) staff       (20)      935 2023-04-30 01:42:58.000000 bulk-mv-0.1.4/bulk_mv/tests/test_bmv_generator.py
+-rw-r--r--   0 garcia     (501) staff       (20)     1160 2023-04-30 01:42:58.000000 bulk-mv-0.1.4/bulk_mv/tests/test_bmv_parser.py
+-rw-r--r--   0 garcia     (501) staff       (20)     4243 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/bulk_mv/tests/test_file_tree.py
+-rw-r--r--   0 garcia     (501) staff       (20)     1116 2023-03-23 02:03:19.000000 bulk-mv-0.1.4/bulk_mv/tests/test_file_tree_builder.py
+-rw-r--r--   0 garcia     (501) staff       (20)      676 2023-04-04 01:50:14.000000 bulk-mv-0.1.4/bulk_mv/tests/test_helpers.py
+-rw-r--r--   0 garcia     (501) staff       (20)     1996 2023-04-30 01:42:58.000000 bulk-mv-0.1.4/bulk_mv/tests/test_operations.py
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.259005 bulk-mv-0.1.4/bulk_mv.egg-info/
+-rw-r--r--   0 garcia     (501) staff       (20)    19287 2023-04-30 01:50:47.000000 bulk-mv-0.1.4/bulk_mv.egg-info/PKG-INFO
+-rw-r--r--   0 garcia     (501) staff       (20)     2046 2023-04-30 01:50:47.000000 bulk-mv-0.1.4/bulk_mv.egg-info/SOURCES.txt
+-rw-r--r--   0 garcia     (501) staff       (20)        1 2023-04-30 01:50:47.000000 bulk-mv-0.1.4/bulk_mv.egg-info/dependency_links.txt
+-rw-r--r--   0 garcia     (501) staff       (20)       46 2023-04-30 01:50:47.000000 bulk-mv-0.1.4/bulk_mv.egg-info/entry_points.txt
+-rw-r--r--   0 garcia     (501) staff       (20)      161 2023-04-30 01:50:47.000000 bulk-mv-0.1.4/bulk_mv.egg-info/requires.txt
+-rw-r--r--   0 garcia     (501) staff       (20)        8 2023-04-30 01:50:47.000000 bulk-mv-0.1.4/bulk_mv.egg-info/top_level.txt
+-rw-r--r--   0 garcia     (501) staff       (20)      115 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/codecov.yml
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.277016 bulk-mv-0.1.4/doc/
+-rw-r--r--   0 garcia     (501) staff       (20)      634 2023-04-03 14:39:52.000000 bulk-mv-0.1.4/doc/Makefile
+-rw-r--r--   0 garcia     (501) staff       (20)     1191 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/doc/bulk_mv.rst
+-rw-r--r--   0 garcia     (501) staff       (20)     1109 2023-04-30 01:44:40.000000 bulk-mv-0.1.4/doc/conf.py
+-rw-r--r--   0 garcia     (501) staff       (20)      448 2023-04-03 14:39:52.000000 bulk-mv-0.1.4/doc/index.rst
+-rw-r--r--   0 garcia     (501) staff       (20)      765 2023-04-03 14:39:52.000000 bulk-mv-0.1.4/doc/make.bat
+-rw-r--r--   0 garcia     (501) staff       (20)       58 2023-04-03 14:39:52.000000 bulk-mv-0.1.4/doc/modules.rst
+-rw-r--r--   0 garcia     (501) staff       (20)     2240 2023-04-30 01:44:40.000000 bulk-mv-0.1.4/pyproject.toml
+-rw-r--r--   0 garcia     (501) staff       (20)       38 2023-04-30 01:50:47.279338 bulk-mv-0.1.4/setup.cfg
+-rw-r--r--   0 garcia     (501) staff       (20)      521 2023-04-30 01:44:40.000000 bulk-mv-0.1.4/setup.py
```

### Comparing `bulk-mv-0.1.3/CONTRIBUTING.md` & `bulk-mv-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/LICENSE` & `bulk-mv-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/MANIFEST.in` & `bulk-mv-0.1.4/MANIFEST.in`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 include README.md
 include CONTRIBUTING.md
 
 include .bumpversion.cfg
 include pyproject.toml
 include Makefile
 include codecov.yml
+include .nojekyll
 
 include branding/*.png
 recursive-include doc *.bat
 recursive-include doc *.py
 recursive-include doc *.rst
 recursive-include doc Makefile
```

### Comparing `bulk-mv-0.1.3/Makefile` & `bulk-mv-0.1.4/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+TMPREPO=/tmp/docs/bulk-mv
+
 #########
 # BUILD #
 #########
 develop:  ## install dependencies and build library
 	python -m pip install -e .[develop]
 
 build:  ## build the python library
@@ -81,14 +83,28 @@
 #########
 deep-clean: ## clean everything from the repository
 	git clean -fdx
 
 clean: ## clean the repository
 	rm -rf .coverage coverage cover htmlcov logs build dist *.egg-info .pytest_cache
 
+docs: 
+	$(MAKE) -C doc/ clean
+	$(MAKE) -C doc/ html
+
+pages: 
+	rm -rf $(TMPREPO)
+	git clone -b gh-pages git@github.com:angarc/bulk-mv.git $(TMPREPO)
+	rm -rf $(TMPREPO)/*
+	cp -r doc/_build/html/* $(TMPREPO)
+	cd $(TMPREPO);\
+	git add -A ;\
+	git commit -a -m 'auto-updating docs' ;\
+	git push
+
 ############################################################################################
 
 # Thanks to Francoise at marmelab.com for this
 .DEFAULT_GOAL := help
 help:
 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
```

### Comparing `bulk-mv-0.1.3/PKG-INFO` & `bulk-mv-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulk-mv
-Version: 0.1.3
+Version: 0.1.4
 Summary: An example python project
 Home-page: https://github.com/angarc/bulk-mv
 Author: Angel Garcia
 Author-email: Angel Garcia <angarc37@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -284,14 +284,28 @@
         main.js
       }
     }
   }
 }
 ```
 
+## Some Use Cases
+
+### Renaming multiple files
+
+https://user-images.githubusercontent.com/18252779/229972782-6a5fcad5-a399-409e-b39a-a94f8f6136f9.mov
+
+### Moving multiple directories
+
+https://user-images.githubusercontent.com/18252779/229972812-952d97f5-55ba-4407-bf0b-9ec14ce10fa2.mov
+
+# BMV Syntax
+
+Here's how to use the only four operators in BMV (`+`, `-`, `>`, `>>`) to add, delete, rename, and move files and/or directories. 
+
 ## Creating new files/directories
 
 You can add files or directories using the `+` operator. 
 
 Here's how to use it to add new files and directories
 
 ```bmv
@@ -386,15 +400,15 @@
         main.js > script.js
       }
     }
   }
 }
 ```
 
-Running this would change rename the `./web/public/photos/` directory to `./web/public/images/`, and it rename `./web/static/javascript/main.js` to `./web/static/javascript/script.js`
+Running this would rename the `./web/public/photos/` directory to `./web/public/images/`, and rename `./web/static/javascript/main.js` to `./web/static/javascript/script.js`
 
 ## Moving files/directories
 
 You can move files or directories using the `>>` operator. Moving files to paths with non-existent directories *will not be created automatically*.
 
 ```bmv
 [./] {
```

### Comparing `bulk-mv-0.1.3/README.md` & `bulk-mv-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,28 @@
         main.js
       }
     }
   }
 }
 ```
 
+## Some Use Cases
+
+### Renaming multiple files
+
+https://user-images.githubusercontent.com/18252779/229972782-6a5fcad5-a399-409e-b39a-a94f8f6136f9.mov
+
+### Moving multiple directories
+
+https://user-images.githubusercontent.com/18252779/229972812-952d97f5-55ba-4407-bf0b-9ec14ce10fa2.mov
+
+# BMV Syntax
+
+Here's how to use the only four operators in BMV (`+`, `-`, `>`, `>>`) to add, delete, rename, and move files and/or directories. 
+
 ## Creating new files/directories
 
 You can add files or directories using the `+` operator. 
 
 Here's how to use it to add new files and directories
 
 ```bmv
@@ -162,15 +176,15 @@
         main.js > script.js
       }
     }
   }
 }
 ```
 
-Running this would change rename the `./web/public/photos/` directory to `./web/public/images/`, and it rename `./web/static/javascript/main.js` to `./web/static/javascript/script.js`
+Running this would rename the `./web/public/photos/` directory to `./web/public/images/`, and rename `./web/static/javascript/main.js` to `./web/static/javascript/script.js`
 
 ## Moving files/directories
 
 You can move files or directories using the `>>` operator. Moving files to paths with non-existent directories *will not be created automatically*.
 
 ```bmv
 [./] {
@@ -210,8 +224,8 @@
 3. rename (files first, then directories)
 4. move (files first, then directories)
 
 ## Caveat
 
 So far, bulk-mv only works on files/directories with [POSIX Portable filenames/dirnames](https://www.ibm.com/docs/en/zos/2.2.0?topic=locales-posix-portable-file-name-character-set).
 
-In the future version, I want bulk-mv to support any type of support filenames on Mac OS, Linux, and Windows.
+In the future version, I want bulk-mv to support any type of support filenames on Mac OS, Linux, and Windows.
```

### Comparing `bulk-mv-0.1.3/branding/logo.png` & `bulk-mv-0.1.4/branding/logo.png`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/bulk_mv/bmv.lark` & `bulk-mv-0.1.4/bulk_mv/bmv.lark`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/bulk_mv/bmv_generator.py` & `bulk-mv-0.1.4/bulk_mv/bmv_generator.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/bulk_mv/bmv_parser.py` & `bulk-mv-0.1.4/bulk_mv/bmv_parser.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/bulk_mv/cli.py` & `bulk-mv-0.1.4/bulk_mv/cli.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/bulk_mv/file_tree.py` & `bulk-mv-0.1.4/bulk_mv/file_tree.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/bulk_mv/file_tree_builder.py` & `bulk-mv-0.1.4/bulk_mv/file_tree_builder.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/bulk_mv/helpers.py` & `bulk-mv-0.1.4/bulk_mv/helpers.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/bulk_mv/operations.py` & `bulk-mv-0.1.4/bulk_mv/operations.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/bulk_mv/tests/test_bmv_generator.py` & `bulk-mv-0.1.4/bulk_mv/tests/test_bmv_generator.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/bulk_mv/tests/test_bmv_parser.py` & `bulk-mv-0.1.4/bulk_mv/tests/test_bmv_parser.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/bulk_mv/tests/test_file_tree.py` & `bulk-mv-0.1.4/bulk_mv/tests/test_file_tree.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/bulk_mv/tests/test_file_tree_builder.py` & `bulk-mv-0.1.4/bulk_mv/tests/test_file_tree_builder.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/bulk_mv/tests/test_helpers.py` & `bulk-mv-0.1.4/bulk_mv/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/bulk_mv/tests/test_operations.py` & `bulk-mv-0.1.4/bulk_mv/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/bulk_mv.egg-info/PKG-INFO` & `bulk-mv-0.1.4/bulk_mv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulk-mv
-Version: 0.1.3
+Version: 0.1.4
 Summary: An example python project
 Home-page: https://github.com/angarc/bulk-mv
 Author: Angel Garcia
 Author-email: Angel Garcia <angarc37@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -284,14 +284,28 @@
         main.js
       }
     }
   }
 }
 ```
 
+## Some Use Cases
+
+### Renaming multiple files
+
+https://user-images.githubusercontent.com/18252779/229972782-6a5fcad5-a399-409e-b39a-a94f8f6136f9.mov
+
+### Moving multiple directories
+
+https://user-images.githubusercontent.com/18252779/229972812-952d97f5-55ba-4407-bf0b-9ec14ce10fa2.mov
+
+# BMV Syntax
+
+Here's how to use the only four operators in BMV (`+`, `-`, `>`, `>>`) to add, delete, rename, and move files and/or directories. 
+
 ## Creating new files/directories
 
 You can add files or directories using the `+` operator. 
 
 Here's how to use it to add new files and directories
 
 ```bmv
@@ -386,15 +400,15 @@
         main.js > script.js
       }
     }
   }
 }
 ```
 
-Running this would change rename the `./web/public/photos/` directory to `./web/public/images/`, and it rename `./web/static/javascript/main.js` to `./web/static/javascript/script.js`
+Running this would rename the `./web/public/photos/` directory to `./web/public/images/`, and rename `./web/static/javascript/main.js` to `./web/static/javascript/script.js`
 
 ## Moving files/directories
 
 You can move files or directories using the `>>` operator. Moving files to paths with non-existent directories *will not be created automatically*.
 
 ```bmv
 [./] {
```

### Comparing `bulk-mv-0.1.3/bulk_mv.egg-info/SOURCES.txt` & `bulk-mv-0.1.4/bulk_mv.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .bumpversion.cfg
+.nojekyll
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 codecov.yml
 pyproject.toml
```

### Comparing `bulk-mv-0.1.3/doc/Makefile` & `bulk-mv-0.1.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/doc/bulk_mv.rst` & `bulk-mv-0.1.4/doc/bulk_mv.rst`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/doc/conf.py` & `bulk-mv-0.1.4/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.napoleon']
 
 templates_path = ['_templates']
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
-version = "0.1.3"
+version = "0.1.4"
 release = version
 
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'sphinx_rtd_theme'
```

### Comparing `bulk-mv-0.1.3/doc/make.bat` & `bulk-mv-0.1.4/doc/make.bat`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.3/pyproject.toml` & `bulk-mv-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "bulk-mv"
 authors = [{name = "Angel Garcia", email = "angarc37@gmail.com"}]
 description="An example python project"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 requires-python = ">=3.7"
 
 dependencies = [
   "lark"
 ]
 
 classifiers = [
```

### Comparing `bulk-mv-0.1.3/setup.py` & `bulk-mv-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name='bulk-mv',
-    version="0.1.3",
+    version="0.1.4",
     description='Move, rename, delete, and add files as fast as you can use Vim.',
     author='Angel Garcia',
     author_email='angarc37@gmail.com',
     url='https://github.com/angarc/bulk-mv',
     py_modules=[
         'bulk_mv.__main__',
     ],
```

