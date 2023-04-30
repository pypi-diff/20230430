# Comparing `tmp/bulk-mv-0.1.4.tar.gz` & `tmp/bulk-mv-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulk-mv-0.1.4.tar", last modified: Sun Apr 30 01:50:47 2023, max compression
+gzip compressed data, was "bulk-mv-0.1.5.tar", last modified: Sun Apr 30 02:40:01 2023, max compression
```

## Comparing `bulk-mv-0.1.4.tar` & `bulk-mv-0.1.5.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.279064 bulk-mv-0.1.4/
--rw-r--r--   0 garcia     (501) staff       (20)      503 2023-04-30 01:44:40.000000 bulk-mv-0.1.4/.bumpversion.cfg
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 20:25:34.000000 bulk-mv-0.1.4/.nojekyll
--rw-r--r--   0 garcia     (501) staff       (20)     1030 2023-04-07 16:09:06.000000 bulk-mv-0.1.4/CONTRIBUTING.md
--rw-r--r--   0 garcia     (501) staff       (20)    11357 2023-03-20 19:12:19.000000 bulk-mv-0.1.4/LICENSE
--rw-r--r--   0 garcia     (501) staff       (20)      553 2023-04-04 20:27:21.000000 bulk-mv-0.1.4/MANIFEST.in
--rw-r--r--   0 garcia     (501) staff       (20)     2521 2023-04-04 20:32:28.000000 bulk-mv-0.1.4/Makefile
--rw-r--r--   0 garcia     (501) staff       (20)    19287 2023-04-30 01:50:47.278253 bulk-mv-0.1.4/PKG-INFO
--rw-r--r--   0 garcia     (501) staff       (20)     5454 2023-04-17 18:36:32.000000 bulk-mv-0.1.4/README.md
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.251062 bulk-mv-0.1.4/branding/
--rw-r--r--   0 garcia     (501) staff       (20)   246902 2023-04-03 14:39:52.000000 bulk-mv-0.1.4/branding/logo.png
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.255861 bulk-mv-0.1.4/bulk_mv/
--rw-r--r--   0 garcia     (501) staff       (20)      316 2023-04-30 01:44:40.000000 bulk-mv-0.1.4/bulk_mv/__init__.py
--rw-r--r--   0 garcia     (501) staff       (20)      144 2023-04-03 01:23:55.000000 bulk-mv-0.1.4/bulk_mv/__main__.py
--rw-r--r--   0 garcia     (501) staff       (20)      670 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/bulk_mv/bmv.lark
--rw-r--r--   0 garcia     (501) staff       (20)      865 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/bulk_mv/bmv_generator.py
--rw-r--r--   0 garcia     (501) staff       (20)    11035 2023-04-30 01:42:58.000000 bulk-mv-0.1.4/bulk_mv/bmv_parser.py
--rw-r--r--   0 garcia     (501) staff       (20)     1008 2023-04-30 01:42:58.000000 bulk-mv-0.1.4/bulk_mv/cli.py
--rw-r--r--   0 garcia     (501) staff       (20)     3378 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/bulk_mv/file_tree.py
--rw-r--r--   0 garcia     (501) staff       (20)      968 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/bulk_mv/file_tree_builder.py
--rw-r--r--   0 garcia     (501) staff       (20)      559 2023-04-03 14:39:52.000000 bulk-mv-0.1.4/bulk_mv/helpers.py
--rw-r--r--   0 garcia     (501) staff       (20)     1819 2023-04-30 01:42:58.000000 bulk-mv-0.1.4/bulk_mv/operations.py
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.263760 bulk-mv-0.1.4/bulk_mv/tests/
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.265336 bulk-mv-0.1.4/bulk_mv/tests/dummy_bmv_files/
--rw-r--r--   0 garcia     (501) staff       (20)      288 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_bmv_files/sample1.bmv
--rw-r--r--   0 garcia     (501) staff       (20)      246 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_bmv_files/sample3.bmv
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.244682 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.265905 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.266678 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/admin/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:36:22.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/admin/index.html
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:36:18.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/admin/nichoal.html
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/index.html
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.267807 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/users/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:35:17.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/users/angel.html
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.268197 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/users/blocked/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/users/blocked/blocked_user_1.html
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:35:38.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/users/index.html
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:35:59.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample1/users/josh.html
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.269724 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:37:58.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/a.txt
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:01.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/b.txt
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:05.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/c.txt
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.270108 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/data/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:37.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/data/report.csv
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:49.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/readme.md
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.271280 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/web/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:15.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/web/index.html
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:21.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/web/main.css
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:19.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample2/web/main.js
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.245830 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.271652 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/delete/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-30 01:37:16.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/delete/no_more.html
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.272398 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/markdown/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 01:41:20.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/markdown/1.md
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-30 01:37:16.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/markdown/2.md
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.272934 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/photos/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 01:41:20.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/photos/test.jpg
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.273689 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/text/
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-23 01:36:28.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/text/1.txt
--rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 02:57:45.000000 bulk-mv-0.1.4/bulk_mv/tests/dummy_directories/sample3/text/2.txt
--rw-r--r--   0 garcia     (501) staff       (20)      935 2023-04-30 01:42:58.000000 bulk-mv-0.1.4/bulk_mv/tests/test_bmv_generator.py
--rw-r--r--   0 garcia     (501) staff       (20)     1160 2023-04-30 01:42:58.000000 bulk-mv-0.1.4/bulk_mv/tests/test_bmv_parser.py
--rw-r--r--   0 garcia     (501) staff       (20)     4243 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/bulk_mv/tests/test_file_tree.py
--rw-r--r--   0 garcia     (501) staff       (20)     1116 2023-03-23 02:03:19.000000 bulk-mv-0.1.4/bulk_mv/tests/test_file_tree_builder.py
--rw-r--r--   0 garcia     (501) staff       (20)      676 2023-04-04 01:50:14.000000 bulk-mv-0.1.4/bulk_mv/tests/test_helpers.py
--rw-r--r--   0 garcia     (501) staff       (20)     1996 2023-04-30 01:42:58.000000 bulk-mv-0.1.4/bulk_mv/tests/test_operations.py
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.259005 bulk-mv-0.1.4/bulk_mv.egg-info/
--rw-r--r--   0 garcia     (501) staff       (20)    19287 2023-04-30 01:50:47.000000 bulk-mv-0.1.4/bulk_mv.egg-info/PKG-INFO
--rw-r--r--   0 garcia     (501) staff       (20)     2046 2023-04-30 01:50:47.000000 bulk-mv-0.1.4/bulk_mv.egg-info/SOURCES.txt
--rw-r--r--   0 garcia     (501) staff       (20)        1 2023-04-30 01:50:47.000000 bulk-mv-0.1.4/bulk_mv.egg-info/dependency_links.txt
--rw-r--r--   0 garcia     (501) staff       (20)       46 2023-04-30 01:50:47.000000 bulk-mv-0.1.4/bulk_mv.egg-info/entry_points.txt
--rw-r--r--   0 garcia     (501) staff       (20)      161 2023-04-30 01:50:47.000000 bulk-mv-0.1.4/bulk_mv.egg-info/requires.txt
--rw-r--r--   0 garcia     (501) staff       (20)        8 2023-04-30 01:50:47.000000 bulk-mv-0.1.4/bulk_mv.egg-info/top_level.txt
--rw-r--r--   0 garcia     (501) staff       (20)      115 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/codecov.yml
-drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 01:50:47.277016 bulk-mv-0.1.4/doc/
--rw-r--r--   0 garcia     (501) staff       (20)      634 2023-04-03 14:39:52.000000 bulk-mv-0.1.4/doc/Makefile
--rw-r--r--   0 garcia     (501) staff       (20)     1191 2023-04-04 02:58:22.000000 bulk-mv-0.1.4/doc/bulk_mv.rst
--rw-r--r--   0 garcia     (501) staff       (20)     1109 2023-04-30 01:44:40.000000 bulk-mv-0.1.4/doc/conf.py
--rw-r--r--   0 garcia     (501) staff       (20)      448 2023-04-03 14:39:52.000000 bulk-mv-0.1.4/doc/index.rst
--rw-r--r--   0 garcia     (501) staff       (20)      765 2023-04-03 14:39:52.000000 bulk-mv-0.1.4/doc/make.bat
--rw-r--r--   0 garcia     (501) staff       (20)       58 2023-04-03 14:39:52.000000 bulk-mv-0.1.4/doc/modules.rst
--rw-r--r--   0 garcia     (501) staff       (20)     2240 2023-04-30 01:44:40.000000 bulk-mv-0.1.4/pyproject.toml
--rw-r--r--   0 garcia     (501) staff       (20)       38 2023-04-30 01:50:47.279338 bulk-mv-0.1.4/setup.cfg
--rw-r--r--   0 garcia     (501) staff       (20)      521 2023-04-30 01:44:40.000000 bulk-mv-0.1.4/setup.py
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.454944 bulk-mv-0.1.5/
+-rw-r--r--   0 garcia     (501) staff       (20)      503 2023-04-30 02:38:58.000000 bulk-mv-0.1.5/.bumpversion.cfg
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 20:25:34.000000 bulk-mv-0.1.5/.nojekyll
+-rw-r--r--   0 garcia     (501) staff       (20)     1030 2023-04-07 16:09:06.000000 bulk-mv-0.1.5/CONTRIBUTING.md
+-rw-r--r--   0 garcia     (501) staff       (20)    11357 2023-03-20 19:12:19.000000 bulk-mv-0.1.5/LICENSE
+-rw-r--r--   0 garcia     (501) staff       (20)      553 2023-04-04 20:27:21.000000 bulk-mv-0.1.5/MANIFEST.in
+-rw-r--r--   0 garcia     (501) staff       (20)     2521 2023-04-04 20:32:28.000000 bulk-mv-0.1.5/Makefile
+-rw-r--r--   0 garcia     (501) staff       (20)    19471 2023-04-30 02:40:01.454311 bulk-mv-0.1.5/PKG-INFO
+-rw-r--r--   0 garcia     (501) staff       (20)     5638 2023-04-30 02:31:24.000000 bulk-mv-0.1.5/README.md
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.397461 bulk-mv-0.1.5/branding/
+-rw-r--r--   0 garcia     (501) staff       (20)   246902 2023-04-03 14:39:52.000000 bulk-mv-0.1.5/branding/logo.png
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.408292 bulk-mv-0.1.5/bulk_mv/
+-rw-r--r--   0 garcia     (501) staff       (20)      316 2023-04-30 02:38:58.000000 bulk-mv-0.1.5/bulk_mv/__init__.py
+-rw-r--r--   0 garcia     (501) staff       (20)      144 2023-04-03 01:23:55.000000 bulk-mv-0.1.5/bulk_mv/__main__.py
+-rw-r--r--   0 garcia     (501) staff       (20)      670 2023-04-04 02:58:22.000000 bulk-mv-0.1.5/bulk_mv/bmv.lark
+-rw-r--r--   0 garcia     (501) staff       (20)      865 2023-04-04 02:58:22.000000 bulk-mv-0.1.5/bulk_mv/bmv_generator.py
+-rw-r--r--   0 garcia     (501) staff       (20)    11418 2023-04-30 02:31:24.000000 bulk-mv-0.1.5/bulk_mv/bmv_parser.py
+-rw-r--r--   0 garcia     (501) staff       (20)     1040 2023-04-30 02:31:24.000000 bulk-mv-0.1.5/bulk_mv/cli.py
+-rw-r--r--   0 garcia     (501) staff       (20)     3378 2023-04-04 02:58:22.000000 bulk-mv-0.1.5/bulk_mv/file_tree.py
+-rw-r--r--   0 garcia     (501) staff       (20)      968 2023-04-04 02:58:22.000000 bulk-mv-0.1.5/bulk_mv/file_tree_builder.py
+-rw-r--r--   0 garcia     (501) staff       (20)      559 2023-04-03 14:39:52.000000 bulk-mv-0.1.5/bulk_mv/helpers.py
+-rw-r--r--   0 garcia     (501) staff       (20)     1785 2023-04-30 02:31:24.000000 bulk-mv-0.1.5/bulk_mv/operations.py
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.417040 bulk-mv-0.1.5/bulk_mv/tests/
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.418160 bulk-mv-0.1.5/bulk_mv/tests/dummy_bmv_files/
+-rw-r--r--   0 garcia     (501) staff       (20)      288 2023-04-04 02:58:22.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_bmv_files/sample1.bmv
+-rw-r--r--   0 garcia     (501) staff       (20)      246 2023-04-04 02:58:22.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_bmv_files/sample3.bmv
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.366082 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.418762 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample1/
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.439457 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample1/admin/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:36:22.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample1/admin/index.html
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:36:18.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample1/admin/nichoal.html
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 02:58:22.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample1/index.html
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.440862 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample1/users/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:35:17.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample1/users/angel.html
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.441370 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample1/users/blocked/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 02:58:22.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample1/users/blocked/blocked_user_1.html
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:35:38.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample1/users/index.html
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:35:59.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample1/users/josh.html
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.443192 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample2/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:37:58.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample2/a.txt
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:01.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample2/b.txt
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:05.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample2/c.txt
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.443672 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample2/data/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:37.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample2/data/report.csv
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:49.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample2/readme.md
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.445084 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample2/web/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:15.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample2/web/index.html
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:21.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample2/web/main.css
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 01:38:19.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample2/web/main.js
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.367233 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample3/
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.445711 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample3/delete/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-30 01:37:16.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample3/delete/no_more.html
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.446701 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample3/markdown/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 01:41:20.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample3/markdown/1.md
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-30 01:37:16.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample3/markdown/2.md
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.447175 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample3/photos/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-04-04 01:41:20.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample3/photos/test.jpg
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.448114 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample3/text/
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-23 01:36:28.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample3/text/1.txt
+-rw-r--r--   0 garcia     (501) staff       (20)        0 2023-03-21 02:57:45.000000 bulk-mv-0.1.5/bulk_mv/tests/dummy_directories/sample3/text/2.txt
+-rw-r--r--   0 garcia     (501) staff       (20)      924 2023-04-30 02:31:24.000000 bulk-mv-0.1.5/bulk_mv/tests/test_bmv_generator.py
+-rw-r--r--   0 garcia     (501) staff       (20)     1192 2023-04-30 02:31:24.000000 bulk-mv-0.1.5/bulk_mv/tests/test_bmv_parser.py
+-rw-r--r--   0 garcia     (501) staff       (20)     4243 2023-04-04 02:58:22.000000 bulk-mv-0.1.5/bulk_mv/tests/test_file_tree.py
+-rw-r--r--   0 garcia     (501) staff       (20)     1116 2023-03-23 02:03:19.000000 bulk-mv-0.1.5/bulk_mv/tests/test_file_tree_builder.py
+-rw-r--r--   0 garcia     (501) staff       (20)      676 2023-04-04 01:50:14.000000 bulk-mv-0.1.5/bulk_mv/tests/test_helpers.py
+-rw-r--r--   0 garcia     (501) staff       (20)     2032 2023-04-30 02:31:24.000000 bulk-mv-0.1.5/bulk_mv/tests/test_operations.py
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.413245 bulk-mv-0.1.5/bulk_mv.egg-info/
+-rw-r--r--   0 garcia     (501) staff       (20)    19471 2023-04-30 02:40:01.000000 bulk-mv-0.1.5/bulk_mv.egg-info/PKG-INFO
+-rw-r--r--   0 garcia     (501) staff       (20)     2046 2023-04-30 02:40:01.000000 bulk-mv-0.1.5/bulk_mv.egg-info/SOURCES.txt
+-rw-r--r--   0 garcia     (501) staff       (20)        1 2023-04-30 02:40:01.000000 bulk-mv-0.1.5/bulk_mv.egg-info/dependency_links.txt
+-rw-r--r--   0 garcia     (501) staff       (20)       46 2023-04-30 02:40:01.000000 bulk-mv-0.1.5/bulk_mv.egg-info/entry_points.txt
+-rw-r--r--   0 garcia     (501) staff       (20)      161 2023-04-30 02:40:01.000000 bulk-mv-0.1.5/bulk_mv.egg-info/requires.txt
+-rw-r--r--   0 garcia     (501) staff       (20)        8 2023-04-30 02:40:01.000000 bulk-mv-0.1.5/bulk_mv.egg-info/top_level.txt
+-rw-r--r--   0 garcia     (501) staff       (20)      115 2023-04-04 02:58:22.000000 bulk-mv-0.1.5/codecov.yml
+drwxr-xr-x   0 garcia     (501) staff       (20)        0 2023-04-30 02:40:01.453046 bulk-mv-0.1.5/doc/
+-rw-r--r--   0 garcia     (501) staff       (20)      634 2023-04-03 14:39:52.000000 bulk-mv-0.1.5/doc/Makefile
+-rw-r--r--   0 garcia     (501) staff       (20)     1191 2023-04-04 02:58:22.000000 bulk-mv-0.1.5/doc/bulk_mv.rst
+-rw-r--r--   0 garcia     (501) staff       (20)     1109 2023-04-30 02:38:58.000000 bulk-mv-0.1.5/doc/conf.py
+-rw-r--r--   0 garcia     (501) staff       (20)      448 2023-04-03 14:39:52.000000 bulk-mv-0.1.5/doc/index.rst
+-rw-r--r--   0 garcia     (501) staff       (20)      765 2023-04-03 14:39:52.000000 bulk-mv-0.1.5/doc/make.bat
+-rw-r--r--   0 garcia     (501) staff       (20)       58 2023-04-03 14:39:52.000000 bulk-mv-0.1.5/doc/modules.rst
+-rw-r--r--   0 garcia     (501) staff       (20)     2240 2023-04-30 02:38:58.000000 bulk-mv-0.1.5/pyproject.toml
+-rw-r--r--   0 garcia     (501) staff       (20)       38 2023-04-30 02:40:01.455143 bulk-mv-0.1.5/setup.cfg
+-rw-r--r--   0 garcia     (501) staff       (20)      521 2023-04-30 02:38:58.000000 bulk-mv-0.1.5/setup.py
```

### Comparing `bulk-mv-0.1.4/CONTRIBUTING.md` & `bulk-mv-0.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.4/LICENSE` & `bulk-mv-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.4/MANIFEST.in` & `bulk-mv-0.1.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.4/Makefile` & `bulk-mv-0.1.5/Makefile`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.4/PKG-INFO` & `bulk-mv-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulk-mv
-Version: 0.1.4
+Version: 0.1.5
 Summary: An example python project
 Home-page: https://github.com/angarc/bulk-mv
 Author: Angel Garcia
 Author-email: Angel Garcia <angarc37@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -222,20 +222,20 @@
 Provides-Extra: develop
 License-File: LICENSE
 
 ![cover_photo](./branding/logo.png)
 
 # Overview
 
-[![License](https://img.shields.io/github/license/angarc/bulk-mv)]()
-[![Issues](https://img.shields.io/github/issues/angarc/bulk-mv)]()
-[![codecov](https://img.shields.io/codecov/c/github/angarc/bulk-mv)]()
-[![build](https://img.shields.io/github/actions/workflow/status/angarc/bulk-mv/build.yml)]()
+[![License](https://img.shields.io/github/license/angarc/bulk-mv)](https://github.com/angarc/bulk-mv/blob/main/LICENSE)
+[![Issues](https://img.shields.io/github/issues/angarc/bulk-mv)](https://github.com/angarc/bulk-mv/issues)
+[![codecov](https://img.shields.io/codecov/c/github/angarc/bulk-mv)](https://app.codecov.io/gh/angarc/bulk-mv)
+[![build](https://img.shields.io/github/actions/workflow/status/angarc/bulk-mv/build.yml)](https://github.com/angarc/bulk-mv/actions/workflows/build.yml)
 [![PyPI](https://img.shields.io/pypi/v/bulk-mv)](https://pypi.org/project/bulk-mv/)
-[![Docs](https://img.shields.io/readthedocs/bulk-mv)](https://bulk-mv.readthedocs.io/en/latest/)
+[![Docs](https://img.shields.io/readthedocs/bulk-mv)](https://angarc.github.io/bulk-mv/)
 
 bulk-mv is an interactive tool that does what the `mv` command does, but for mulitiple files, with the ability to do more like adding and deleting files as well.
 
 # Installation
 
 ```
 pip install bulk-mv
```

### Comparing `bulk-mv-0.1.4/README.md` & `bulk-mv-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ![cover_photo](./branding/logo.png)
 
 # Overview
 
-[![License](https://img.shields.io/github/license/angarc/bulk-mv)]()
-[![Issues](https://img.shields.io/github/issues/angarc/bulk-mv)]()
-[![codecov](https://img.shields.io/codecov/c/github/angarc/bulk-mv)]()
-[![build](https://img.shields.io/github/actions/workflow/status/angarc/bulk-mv/build.yml)]()
+[![License](https://img.shields.io/github/license/angarc/bulk-mv)](https://github.com/angarc/bulk-mv/blob/main/LICENSE)
+[![Issues](https://img.shields.io/github/issues/angarc/bulk-mv)](https://github.com/angarc/bulk-mv/issues)
+[![codecov](https://img.shields.io/codecov/c/github/angarc/bulk-mv)](https://app.codecov.io/gh/angarc/bulk-mv)
+[![build](https://img.shields.io/github/actions/workflow/status/angarc/bulk-mv/build.yml)](https://github.com/angarc/bulk-mv/actions/workflows/build.yml)
 [![PyPI](https://img.shields.io/pypi/v/bulk-mv)](https://pypi.org/project/bulk-mv/)
-[![Docs](https://img.shields.io/readthedocs/bulk-mv)](https://bulk-mv.readthedocs.io/en/latest/)
+[![Docs](https://img.shields.io/readthedocs/bulk-mv)](https://angarc.github.io/bulk-mv/)
 
 bulk-mv is an interactive tool that does what the `mv` command does, but for mulitiple files, with the ability to do more like adding and deleting files as well.
 
 # Installation
 
 ```
 pip install bulk-mv
```

### Comparing `bulk-mv-0.1.4/branding/logo.png` & `bulk-mv-0.1.5/branding/logo.png`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.4/bulk_mv/bmv.lark` & `bulk-mv-0.1.5/bulk_mv/bmv.lark`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.4/bulk_mv/bmv_generator.py` & `bulk-mv-0.1.5/bulk_mv/bmv_generator.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.4/bulk_mv/bmv_parser.py` & `bulk-mv-0.1.5/bulk_mv/bmv_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -255,89 +255,93 @@
     def lbrack(self, _):
         return "["
 
     def rbrack(self, _):
         return "]"
 
 
-def get_operations(tree, ops, current_path):
-    """Extracts operation instructions from BMV Parse tree
-
-    Args:
-        tree (dict): BMV Parse tree
-        ops (dict): Dictionary to store operations
-        current_path (str): Current path of the directory
-
-    Returns:
-        dict: Dictionary of operations
-    """
-    for op in tree['unary']:
-        if 'add' in op:
-            if 'file' in op['add']:
-                final_path = current_path + '/' + op['add']['file']
-                ops['add'].append(final_path.replace("//", "/"))
-            elif 'dir' in op['add']:
-                final_path = current_path + '/' + op['add']['dir']['dirname']
-                ops['add'].append((final_path + '/').replace("//", "/"))
-
-                for file in op['add']['dir']['files']:
-                    ops['add'].append((final_path + '/' + file).replace("//", "/"))
-
-                get_operations(op['add']['dir'], ops, final_path.replace("//", "/"))
-
-        elif 'delete' in op:
-            if 'file' in op['delete']:
-                final_path = current_path + '/' + op['delete']['file']
-                ops['delete'].append(final_path.replace("//", "/"))
-            elif 'dir' in op['delete']:
-                final_path = current_path + '/' + op['delete']['dir']['dirname']
-                ops['delete'].append((final_path + '/').replace("//", "/"))
-
-    for op in tree['file_op']:
-        if "rename_file_op" in op:
-            old_path = current_path + '/' + op['rename_file_op']['old_name']
-            new_path = current_path + '/' + op['rename_file_op']['new_name']
-            ops['rename_files'].append({'old_path': old_path, 'new_path': new_path})
-        if "move_file_op" in op:
-            old_path = current_path + '/' + op['move_file_op']['current_name']
-            new_path = op['move_file_op']['new_path']
-            ops['move_files'].append({'current_path': old_path, 'new_path': new_path})
-
-    for op in tree['dir_op']:
-        if 'rename' in op:
-            if current_path != op['rename']['old_name']:
+class BmvParser:
+    def __init__(self):
+        self.tree = None
+
+    def parse(self, data):
+        """Parses a BMV string and returns a dictionary of operations
+
+        Args:
+            data (str): BMV string
+
+        Returns:
+            dict: Dictionary of operations
+        """
+        parser = Lark.open("bmv.lark", rel_to=__file__, parser='lalr')
+        tree = parser.parse(data)
+        res = TreeToOperations().transform(tree)
+        self.tree = res['dir']
+
+        ops = {'add': [], 'delete': [], 'rename_files': [], 'rename_dirs': [], 'move_files': [], 'move_dirs': []}
+        self.get_operations(self.tree, ops, res['dir']['dirname'])
+        ops['rename_dirs'] = ops['rename_dirs'][::-1]
+
+        return ops
+
+    def get_operations(self, tree, ops, current_path):
+        """Extracts operation instructions from BMV Parse tree
+
+        Args:
+            tree (dict): BMV Parse tree
+            ops (dict): Dictionary to store operations
+            current_path (str): Current path of the directory
+
+        Returns:
+            dict: Dictionary of operations
+        """
+        for op in tree['unary']:
+            if 'add' in op:
+                if 'file' in op['add']:
+                    final_path = current_path + '/' + op['add']['file']
+                    ops['add'].append(final_path.replace("//", "/"))
+                elif 'dir' in op['add']:
+                    final_path = current_path + '/' + op['add']['dir']['dirname']
+                    ops['add'].append((final_path + '/').replace("//", "/"))
+
+                    for file in op['add']['dir']['files']:
+                        ops['add'].append((final_path + '/' + file).replace("//", "/"))
+
+                    self.get_operations(op['add']['dir'], ops, final_path.replace("//", "/"))
+
+            elif 'delete' in op:
+                if 'file' in op['delete']:
+                    final_path = current_path + '/' + op['delete']['file']
+                    ops['delete'].append(final_path.replace("//", "/"))
+                elif 'dir' in op['delete']:
+                    final_path = current_path + '/' + op['delete']['dir']['dirname']
+                    ops['delete'].append((final_path + '/').replace("//", "/"))
+
+        for op in tree['file_op']:
+            if "rename_file_op" in op:
+                old_path = current_path + '/' + op['rename_file_op']['old_name']
+                new_path = current_path + '/' + op['rename_file_op']['new_name']
+                ops['rename_files'].append({'old_path': old_path, 'new_path': new_path})
+            if "move_file_op" in op:
+                old_path = current_path + '/' + op['move_file_op']['current_name']
+                new_path = op['move_file_op']['new_path']
+                ops['move_files'].append({'current_path': old_path, 'new_path': new_path})
+
+        for op in tree['dir_op']:
+            if 'rename' in op:
+                if current_path != op['rename']['old_name']:
+                    old_path = current_path + '/'
+
+                    last_slash_index = get_last_index_of_substring(current_path, "/")
+                    new_path = current_path[:last_slash_index] + '/' + op['rename']['new_name']
+                    ops['rename_dirs'].append({'old_path': old_path, 'new_path': new_path})
+                else:
+                    ops['rename_dirs'].append(op['rename'])
+            if 'move' in op:
                 old_path = current_path + '/'
+                new_path = op['move']['new_path']
 
-                last_slash_index = get_last_index_of_substring(current_path, "/")
-                new_path = current_path[:last_slash_index] + '/' + op['rename']['new_name']
-                ops['rename_dirs'].append({'old_path': old_path, 'new_path': new_path})
-            else:
-                ops['rename_dirs'].append(op['rename'])
-        if 'move' in op:
-            old_path = current_path + '/'
-            new_path = op['move']['new_path']
-
-            ops['move_dirs'].append({'current_path': old_path, 'new_path': new_path})
-
-    for dir in tree['dirs']:
-        final_path = current_path + '/' + dir['dirname']
-        get_operations(dir, ops, final_path.replace('//', '/'))
-
-
-def parse_bmv(data):
-    """Parses a BMV string and returns a dictionary of operations
-
-    Args:
-        data (str): BMV string
-
-    Returns:
-        dict: Dictionary of operations
-    """
-    parser = Lark.open("bmv.lark", rel_to=__file__, parser='lalr')
-    tree = parser.parse(data)
-    res = TreeToOperations().transform(tree)
-
-    ops = {'add': [], 'delete': [], 'rename_files': [], 'rename_dirs': [], 'move_files': [], 'move_dirs': []}
-    get_operations(res['dir'], ops, res['dir']['dirname'])
-    ops['rename_dirs'] = ops['rename_dirs'][::-1]
+                ops['move_dirs'].append({'current_path': old_path, 'new_path': new_path})
 
-    return ops
+        for dir in tree['dirs']:
+            final_path = current_path + '/' + dir['dirname']
+            self.get_operations(dir, ops, final_path.replace('//', '/'))
```

### Comparing `bulk-mv-0.1.4/bulk_mv/cli.py` & `bulk-mv-0.1.5/bulk_mv/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .file_tree_builder import build_from_directory
-from .bmv_parser import parse_bmv
+from .bmv_parser import BmvParser
 from .bmv_generator import BmvGenerator
 from os import system
 from .operations import perform_adds, perform_deletes, perform_renames, perform_moves
 
 
 def run(start_path):
     """Runs the full pipeline for bmv.
@@ -20,15 +20,16 @@
 
     with open("file_tree.bmv", "w") as file:
         file.write(bmv_content)
 
     system("vim file_tree.bmv")
 
     with open("file_tree.bmv", "r") as file:
-        output = parse_bmv(file.read().strip())
+        parser = BmvParser()
+        output = parser.parse(file.read().strip())
 
     perform_adds(output["add"])
     perform_deletes(output["delete"])
     perform_renames(output["rename_files"])
     perform_renames(output["rename_dirs"])
     perform_moves(output["move_files"])
     perform_moves(output["move_dirs"])
```

### Comparing `bulk-mv-0.1.4/bulk_mv/file_tree.py` & `bulk-mv-0.1.5/bulk_mv/file_tree.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.4/bulk_mv/file_tree_builder.py` & `bulk-mv-0.1.5/bulk_mv/file_tree_builder.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.4/bulk_mv/helpers.py` & `bulk-mv-0.1.5/bulk_mv/helpers.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.4/bulk_mv/operations.py` & `bulk-mv-0.1.5/bulk_mv/operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     Args:
         renamings (dict): dict containing old_path and new_path as keys
 
     """
     for renaming in renamings:
         old_name = renaming["old_path"]
         new_name = renaming["new_path"]
-        print(old_name, new_name)
         rename(old_name, new_name)
 
 
 def perform_moves(movements):
     """Moves old file/dir names to new paths as
     specified by movements
```

### Comparing `bulk-mv-0.1.4/bulk_mv/tests/test_bmv_generator.py` & `bulk-mv-0.1.5/bulk_mv/tests/test_bmv_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from bulk_mv import build_from_directory, parse_bmv, BmvGenerator
+from bulk_mv import build_from_directory, BmvGenerator
 from pathlib import Path
 
 
 class TestBmvGenerator(unittest.TestCase):
     def test_generator(self):
         self.maxDiff = 10000
         file_tree = build_from_directory(f"{Path(__file__).parent}/dummy_directories/sample1/")
```

### Comparing `bulk-mv-0.1.4/bulk_mv/tests/test_bmv_parser.py` & `bulk-mv-0.1.5/bulk_mv/tests/test_bmv_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import unittest
-from bulk_mv import build_from_directory, FileTree, parse_bmv
+from bulk_mv import build_from_directory, FileTree, BmvParser
 from pathlib import Path
 
 
 class TestBmvParser(unittest.TestCase):
     def sample1_file_contents(self):
         with open(f"{Path(__file__).parent}/dummy_bmv_files/sample1.bmv") as file:
             return file.read().strip()
 
     def test_file_tree_visitor(self):
         sample1 = self.sample1_file_contents()
-        output = parse_bmv(sample1)
+        parser = BmvParser()
+        output = parser.parse(sample1)
 
         expected_output = {
             "add": ["web/assets/", "web/pages/images/", "web/pages/images/profile_photos/"],
             "delete": ["web/pages/images/delete_me.jpg"],
             "rename_files": [
                 {"old_path": "web/static/main.css", "new_path": "web/static/script.css"},
                 {"old_path": "web/static/main.js", "new_path": "web/static/script.js"},
```

### Comparing `bulk-mv-0.1.4/bulk_mv/tests/test_file_tree.py` & `bulk-mv-0.1.5/bulk_mv/tests/test_file_tree.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.4/bulk_mv/tests/test_file_tree_builder.py` & `bulk-mv-0.1.5/bulk_mv/tests/test_file_tree_builder.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.4/bulk_mv/tests/test_helpers.py` & `bulk-mv-0.1.5/bulk_mv/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.4/bulk_mv/tests/test_operations.py` & `bulk-mv-0.1.5/bulk_mv/tests/test_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import unittest
 from bulk_mv import (
     build_from_directory,
-    parse_bmv,
+    BmvParser,
     perform_adds,
     perform_deletes,
     perform_renames,
     perform_moves,
 )
 from os import path, remove, rename
 from shutil import rmtree, move
 import pathlib
 
 
 class TestOperations(unittest.TestCase):
     def setUp(self):
         with open("bulk_mv/tests/dummy_bmv_files/sample3.bmv", "r") as file:
-            self.output = parse_bmv(file.read().strip())
+            parser = BmvParser()
+            self.output = parser.parse(file.read().strip())
 
     def test_perform_adds(self):
         perform_adds(self.output["add"])
 
         self.assertTrue(path.exists("./bulk_mv/tests/dummy_directories/sample3/new_file.txt"))
 
         remove("./bulk_mv/tests/dummy_directories/sample3/new_file.txt")
```

### Comparing `bulk-mv-0.1.4/bulk_mv.egg-info/PKG-INFO` & `bulk-mv-0.1.5/bulk_mv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulk-mv
-Version: 0.1.4
+Version: 0.1.5
 Summary: An example python project
 Home-page: https://github.com/angarc/bulk-mv
 Author: Angel Garcia
 Author-email: Angel Garcia <angarc37@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -222,20 +222,20 @@
 Provides-Extra: develop
 License-File: LICENSE
 
 ![cover_photo](./branding/logo.png)
 
 # Overview
 
-[![License](https://img.shields.io/github/license/angarc/bulk-mv)]()
-[![Issues](https://img.shields.io/github/issues/angarc/bulk-mv)]()
-[![codecov](https://img.shields.io/codecov/c/github/angarc/bulk-mv)]()
-[![build](https://img.shields.io/github/actions/workflow/status/angarc/bulk-mv/build.yml)]()
+[![License](https://img.shields.io/github/license/angarc/bulk-mv)](https://github.com/angarc/bulk-mv/blob/main/LICENSE)
+[![Issues](https://img.shields.io/github/issues/angarc/bulk-mv)](https://github.com/angarc/bulk-mv/issues)
+[![codecov](https://img.shields.io/codecov/c/github/angarc/bulk-mv)](https://app.codecov.io/gh/angarc/bulk-mv)
+[![build](https://img.shields.io/github/actions/workflow/status/angarc/bulk-mv/build.yml)](https://github.com/angarc/bulk-mv/actions/workflows/build.yml)
 [![PyPI](https://img.shields.io/pypi/v/bulk-mv)](https://pypi.org/project/bulk-mv/)
-[![Docs](https://img.shields.io/readthedocs/bulk-mv)](https://bulk-mv.readthedocs.io/en/latest/)
+[![Docs](https://img.shields.io/readthedocs/bulk-mv)](https://angarc.github.io/bulk-mv/)
 
 bulk-mv is an interactive tool that does what the `mv` command does, but for mulitiple files, with the ability to do more like adding and deleting files as well.
 
 # Installation
 
 ```
 pip install bulk-mv
```

### Comparing `bulk-mv-0.1.4/bulk_mv.egg-info/SOURCES.txt` & `bulk-mv-0.1.5/bulk_mv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.4/doc/Makefile` & `bulk-mv-0.1.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.4/doc/bulk_mv.rst` & `bulk-mv-0.1.5/doc/bulk_mv.rst`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.4/doc/conf.py` & `bulk-mv-0.1.5/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.napoleon']
 
 templates_path = ['_templates']
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
-version = "0.1.4"
+version = "0.1.5"
 release = version
 
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'sphinx_rtd_theme'
```

### Comparing `bulk-mv-0.1.4/doc/make.bat` & `bulk-mv-0.1.5/doc/make.bat`

 * *Files identical despite different names*

### Comparing `bulk-mv-0.1.4/pyproject.toml` & `bulk-mv-0.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "bulk-mv"
 authors = [{name = "Angel Garcia", email = "angarc37@gmail.com"}]
 description="An example python project"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 requires-python = ">=3.7"
 
 dependencies = [
   "lark"
 ]
 
 classifiers = [
```

### Comparing `bulk-mv-0.1.4/setup.py` & `bulk-mv-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name='bulk-mv',
-    version="0.1.4",
+    version="0.1.5",
     description='Move, rename, delete, and add files as fast as you can use Vim.',
     author='Angel Garcia',
     author_email='angarc37@gmail.com',
     url='https://github.com/angarc/bulk-mv',
     py_modules=[
         'bulk_mv.__main__',
     ],
```

