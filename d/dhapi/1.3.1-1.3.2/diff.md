# Comparing `tmp/dhapi-1.3.1.tar.gz` & `tmp/dhapi-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhapi-1.3.1.tar", last modified: Fri Apr 21 16:18:49 2023, max compression
+gzip compressed data, was "dhapi-1.3.2.tar", last modified: Sun Apr 30 12:25:38 2023, max compression
```

## Comparing `dhapi-1.3.1.tar` & `dhapi-1.3.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-21 16:18:49.127054 dhapi-1.3.1/
--rw-r--r--   0 roeniss    (501) staff       (20)    11356 2023-03-28 15:41:09.000000 dhapi-1.3.1/LICENSE.txt
--rw-r--r--   0 roeniss    (501) staff       (20)     1542 2023-04-21 16:18:49.126858 dhapi-1.3.1/PKG-INFO
--rw-r--r--   0 roeniss    (501) staff       (20)      505 2023-04-21 16:11:39.000000 dhapi-1.3.1/README.md
--rw-r--r--   0 roeniss    (501) staff       (20)       51 2023-04-21 16:11:39.000000 dhapi-1.3.1/pyproject.toml
--rw-r--r--   0 roeniss    (501) staff       (20)       38 2023-04-21 16:18:49.127109 dhapi-1.3.1/setup.cfg
--rw-r--r--   0 roeniss    (501) staff       (20)     1560 2023-04-21 16:12:55.000000 dhapi-1.3.1/setup.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-21 16:18:49.122649 dhapi-1.3.1/src/
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-21 16:18:49.124384 dhapi-1.3.1/src/dhapi/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/__init__.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-21 16:18:49.125381 dhapi-1.3.1/src/dhapi/client/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/client/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     4657 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/client/lottery_client.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-21 16:18:49.125627 dhapi-1.3.1/src/dhapi/domain_object/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/domain_object/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     3393 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/domain_object/lotto645_buy_request.py
--rw-r--r--   0 roeniss    (501) staff       (20)      120 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/main.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-21 16:18:49.125870 dhapi-1.3.1/src/dhapi/purchase/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/purchase/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     2372 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/purchase/lotto645_controller.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-21 16:18:49.126219 dhapi-1.3.1/src/dhapi/router/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/router/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     3919 2023-04-21 16:15:47.000000 dhapi-1.3.1/src/dhapi/router/arg_parser.py
--rw-r--r--   0 roeniss    (501) staff       (20)      463 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/router/router.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-21 16:18:49.126446 dhapi-1.3.1/src/dhapi/user_info/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/user_info/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)      202 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/user_info/user_info_controller.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-21 16:18:49.125129 dhapi-1.3.1/src/dhapi.egg-info/
--rw-r--r--   0 roeniss    (501) staff       (20)     1542 2023-04-21 16:18:49.000000 dhapi-1.3.1/src/dhapi.egg-info/PKG-INFO
--rw-r--r--   0 roeniss    (501) staff       (20)      637 2023-04-21 16:18:49.000000 dhapi-1.3.1/src/dhapi.egg-info/SOURCES.txt
--rw-r--r--   0 roeniss    (501) staff       (20)        1 2023-04-21 16:18:49.000000 dhapi-1.3.1/src/dhapi.egg-info/dependency_links.txt
--rw-r--r--   0 roeniss    (501) staff       (20)       42 2023-04-21 16:18:49.000000 dhapi-1.3.1/src/dhapi.egg-info/entry_points.txt
--rw-r--r--   0 roeniss    (501) staff       (20)        6 2023-04-21 16:18:49.000000 dhapi-1.3.1/src/dhapi.egg-info/top_level.txt
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-30 12:25:38.176642 dhapi-1.3.2/
+-rw-r--r--   0 roeniss    (501) staff       (20)    11356 2023-04-19 16:05:26.000000 dhapi-1.3.2/LICENSE.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)     1160 2023-04-30 12:25:38.176519 dhapi-1.3.2/PKG-INFO
+-rw-r--r--   0 roeniss    (501) staff       (20)      505 2023-04-19 16:05:26.000000 dhapi-1.3.2/README.md
+-rw-r--r--   0 roeniss    (501) staff       (20)       51 2023-04-19 16:05:26.000000 dhapi-1.3.2/pyproject.toml
+-rw-r--r--   0 roeniss    (501) staff       (20)       38 2023-04-30 12:25:38.176673 dhapi-1.3.2/setup.cfg
+-rw-r--r--   0 roeniss    (501) staff       (20)     1271 2023-04-30 12:24:58.000000 dhapi-1.3.2/setup.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-30 12:25:38.173391 dhapi-1.3.2/src/
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-30 12:25:38.174504 dhapi-1.3.2/src/dhapi/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.2/src/dhapi/__init__.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-30 12:25:38.175318 dhapi-1.3.2/src/dhapi/client/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.2/src/dhapi/client/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     4657 2023-04-30 11:41:52.000000 dhapi-1.3.2/src/dhapi/client/lottery_client.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-30 12:25:38.175570 dhapi-1.3.2/src/dhapi/domain_object/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.2/src/dhapi/domain_object/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     3393 2023-04-30 11:41:52.000000 dhapi-1.3.2/src/dhapi/domain_object/lotto645_buy_request.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      120 2023-04-19 16:05:26.000000 dhapi-1.3.2/src/dhapi/main.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-30 12:25:38.175802 dhapi-1.3.2/src/dhapi/purchase/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.2/src/dhapi/purchase/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     2372 2023-04-30 11:41:52.000000 dhapi-1.3.2/src/dhapi/purchase/lotto645_controller.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-30 12:25:38.176129 dhapi-1.3.2/src/dhapi/router/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.2/src/dhapi/router/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     3919 2023-04-30 11:41:52.000000 dhapi-1.3.2/src/dhapi/router/arg_parser.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      463 2023-04-30 11:41:52.000000 dhapi-1.3.2/src/dhapi/router/router.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-30 12:25:38.176353 dhapi-1.3.2/src/dhapi/user_info/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.2/src/dhapi/user_info/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      202 2023-04-19 16:05:26.000000 dhapi-1.3.2/src/dhapi/user_info/user_info_controller.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-30 12:25:38.175114 dhapi-1.3.2/src/dhapi.egg-info/
+-rw-r--r--   0 roeniss    (501) staff       (20)     1160 2023-04-30 12:25:38.000000 dhapi-1.3.2/src/dhapi.egg-info/PKG-INFO
+-rw-r--r--   0 roeniss    (501) staff       (20)      669 2023-04-30 12:25:38.000000 dhapi-1.3.2/src/dhapi.egg-info/SOURCES.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)        1 2023-04-30 12:25:38.000000 dhapi-1.3.2/src/dhapi.egg-info/dependency_links.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)       42 2023-04-30 12:25:38.000000 dhapi-1.3.2/src/dhapi.egg-info/entry_points.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)       54 2023-04-30 12:25:38.000000 dhapi-1.3.2/src/dhapi.egg-info/requires.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)        6 2023-04-30 12:25:38.000000 dhapi-1.3.2/src/dhapi.egg-info/top_level.txt
```

### Comparing `dhapi-1.3.1/LICENSE.txt` & `dhapi-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.1/src/dhapi/client/lottery_client.py` & `dhapi-1.3.2/src/dhapi/client/lottery_client.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.1/src/dhapi/domain_object/lotto645_buy_request.py` & `dhapi-1.3.2/src/dhapi/domain_object/lotto645_buy_request.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.1/src/dhapi/purchase/lotto645_controller.py` & `dhapi-1.3.2/src/dhapi/purchase/lotto645_controller.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.1/src/dhapi/router/arg_parser.py` & `dhapi-1.3.2/src/dhapi/router/arg_parser.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.1/src/dhapi.egg-info/SOURCES.txt` & `dhapi-1.3.2/src/dhapi.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 src/dhapi/__init__.py
 src/dhapi/main.py
 src/dhapi.egg-info/PKG-INFO
 src/dhapi.egg-info/SOURCES.txt
 src/dhapi.egg-info/dependency_links.txt
 src/dhapi.egg-info/entry_points.txt
+src/dhapi.egg-info/requires.txt
 src/dhapi.egg-info/top_level.txt
 src/dhapi/client/__init__.py
 src/dhapi/client/lottery_client.py
 src/dhapi/domain_object/__init__.py
 src/dhapi/domain_object/lotto645_buy_request.py
 src/dhapi/purchase/__init__.py
 src/dhapi/purchase/lotto645_controller.py
```

