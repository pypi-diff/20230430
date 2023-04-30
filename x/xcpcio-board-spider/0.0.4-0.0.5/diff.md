# Comparing `tmp/xcpcio_board_spider-0.0.4.tar.gz` & `tmp/xcpcio_board_spider-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcpcio_board_spider-0.0.4.tar", max compression
+gzip compressed data, was "xcpcio_board_spider-0.0.5.tar", max compression
```

## Comparing `xcpcio_board_spider-0.0.4.tar` & `xcpcio_board_spider-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,10 @@
--rw-r--r--   0        0        0     1063 2023-04-29 17:21:52.609006 xcpcio_board_spider-0.0.4/LICENSE
--rw-r--r--   0        0        0      538 2023-04-29 17:21:52.609006 xcpcio_board_spider-0.0.4/README.md
--rw-r--r--   0        0        0      977 2023-04-29 17:21:52.613006 xcpcio_board_spider-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-29 17:21:52.613006 xcpcio_board_spider-0.0.4/xcpcio_board_spider/__init__.py
--rw-r--r--   0        0        0     1851 2023-04-29 17:21:52.613006 xcpcio_board_spider-0.0.4/xcpcio_board_spider/utils.py
--rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 xcpcio_board_spider-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-30 15:29:30.966794 xcpcio_board_spider-0.0.5/LICENSE
+-rw-r--r--   0        0        0      538 2023-04-30 15:29:30.966794 xcpcio_board_spider-0.0.5/README.md
+-rw-r--r--   0        0        0      977 2023-04-30 15:29:30.966794 xcpcio_board_spider-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-30 15:29:30.966794 xcpcio_board_spider-0.0.5/xcpcio_board_spider/__init__.py
+-rw-r--r--   0        0        0     2160 2023-04-30 15:29:30.966794 xcpcio_board_spider-0.0.5/xcpcio_board_spider/config.py
+-rw-r--r--   0        0        0      303 2023-04-30 15:29:30.966794 xcpcio_board_spider-0.0.5/xcpcio_board_spider/constants.py
+-rw-r--r--   0        0        0      377 2023-04-30 15:29:30.966794 xcpcio_board_spider-0.0.5/xcpcio_board_spider/logger.py
+-rw-r--r--   0        0        0     1074 2023-04-30 15:29:30.970794 xcpcio_board_spider-0.0.5/xcpcio_board_spider/logo.py
+-rw-r--r--   0        0        0     2885 2023-04-30 15:29:30.970794 xcpcio_board_spider-0.0.5/xcpcio_board_spider/utils.py
+-rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 xcpcio_board_spider-0.0.5/PKG-INFO
```

### Comparing `xcpcio_board_spider-0.0.4/LICENSE` & `xcpcio_board_spider-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.4/README.md` & `xcpcio_board_spider-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.4/pyproject.toml` & `xcpcio_board_spider-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcpcio-board-spider"
-version = "0.0.4"
+version = "0.0.5"
 description = "XCPCIO Board Spider"
 authors = ["Dup4 <lyuzhi.pan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `xcpcio_board_spider-0.0.4/PKG-INFO` & `xcpcio_board_spider-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcpcio-board-spider
-Version: 0.0.4
+Version: 0.0.5
 Summary: XCPCIO Board Spider
 License: MIT
 Author: Dup4
 Author-email: lyuzhi.pan@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

