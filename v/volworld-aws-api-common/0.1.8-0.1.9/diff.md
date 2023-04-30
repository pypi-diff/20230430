# Comparing `tmp/volworld_aws_api_common-0.1.8.tar.gz` & `tmp/volworld_aws_api_common-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volworld_aws_api_common-0.1.8.tar", last modified: Thu Feb  2 06:15:46 2023, max compression
+gzip compressed data, was "volworld_aws_api_common-0.1.9.tar", last modified: Thu Feb  2 06:18:11 2023, max compression
```

## Comparing `volworld_aws_api_common-0.1.8.tar` & `volworld_aws_api_common-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:15:46.609555 volworld_aws_api_common-0.1.8/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1070 2023-01-31 04:59:04.000000 volworld_aws_api_common-0.1.8/LICENSE.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      250 2023-02-02 06:15:46.609555 volworld_aws_api_common-0.1.8/PKG-INFO
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       31 2023-01-31 04:59:04.000000 volworld_aws_api_common-0.1.8/README.rst
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       38 2023-02-02 06:15:46.609555 volworld_aws_api_common-0.1.8/setup.cfg
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      386 2023-02-02 06:15:42.000000 volworld_aws_api_common-0.1.8/setup.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:15:46.605555 volworld_aws_api_common-0.1.8/src/
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:15:46.605555 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 00:23:33.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:15:46.605555 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/api/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      225 2023-02-02 02:33:23.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/api/AA.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       76 2023-02-01 01:40:45.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/api/Aws.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 00:23:59.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/api/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:15:46.605555 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/api/enum/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      859 2023-02-02 01:14:00.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/api/enum/HttpStatus.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 01:05:27.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/api/enum/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:15:46.605555 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/api/url/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 00:32:05.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/api/url/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      429 2023-02-02 06:15:34.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/api/url/authUrl.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:15:46.605555 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 00:24:05.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:15:46.605555 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/aws/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      146 2023-01-31 08:23:17.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/aws/ATestRequest.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 00:25:50.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/aws/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:15:46.609555 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/aws/act/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 02:25:47.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/aws/act/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      750 2023-02-02 02:31:42.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/aws/act/act__signup.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      759 2023-02-02 02:31:35.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/aws/act/act__signup_login.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:15:46.609555 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/aws/request/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 00:30:46.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/aws/request/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      708 2023-02-02 01:36:03.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/aws/request/get__current_user.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      939 2023-02-02 01:39:09.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/aws/request/post__login.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      901 2023-02-02 01:35:45.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/aws/request/post__signup.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      481 2023-02-01 01:33:41.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/aws/url.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     4243 2023-02-02 01:36:03.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/request.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:15:46.605555 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common.egg-info/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      250 2023-02-02 06:15:46.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common.egg-info/PKG-INFO
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1291 2023-02-02 06:15:46.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common.egg-info/SOURCES.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        1 2023-02-02 06:15:46.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common.egg-info/dependency_links.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       22 2023-02-02 06:15:46.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common.egg-info/requires.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       24 2023-02-02 06:15:46.000000 volworld_aws_api_common-0.1.8/src/volworld_aws_api_common.egg-info/top_level.txt
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1070 2023-01-31 04:59:04.000000 volworld_aws_api_common-0.1.9/LICENSE.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      250 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/PKG-INFO
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       31 2023-01-31 04:59:04.000000 volworld_aws_api_common-0.1.9/README.rst
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       38 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/setup.cfg
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      386 2023-02-02 06:18:08.000000 volworld_aws_api_common-0.1.9/setup.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 00:23:33.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      225 2023-02-02 02:33:23.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/AA.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       76 2023-02-01 01:40:45.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/Aws.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 00:23:59.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/enum/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      859 2023-02-02 01:14:00.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/enum/HttpStatus.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 01:05:27.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/enum/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/url/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 00:32:05.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/url/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      429 2023-02-02 06:15:34.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/url/authUrl.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 00:24:05.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      146 2023-01-31 08:23:17.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/ATestRequest.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 00:25:50.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/act/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 02:25:47.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/act/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      750 2023-02-02 02:31:42.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/act/act__signup.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      759 2023-02-02 02:31:35.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/act/act__signup_login.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/request/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 00:30:46.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/request/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      708 2023-02-02 01:36:03.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/request/get__current_user.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      939 2023-02-02 01:39:09.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/request/post__login.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      901 2023-02-02 01:35:45.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/request/post__signup.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      482 2023-02-02 06:17:48.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/url.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     4243 2023-02-02 01:36:03.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/request.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common.egg-info/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      250 2023-02-02 06:18:11.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common.egg-info/PKG-INFO
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1291 2023-02-02 06:18:11.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        1 2023-02-02 06:18:11.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       22 2023-02-02 06:18:11.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common.egg-info/requires.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       24 2023-02-02 06:18:11.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common.egg-info/top_level.txt
```

### Comparing `volworld_aws_api_common-0.1.8/LICENSE.txt` & `volworld_aws_api_common-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/api/enum/HttpStatus.py` & `volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/enum/HttpStatus.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/aws/act/act__signup.py` & `volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/act/act__signup.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/aws/act/act__signup_login.py` & `volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/act/act__signup_login.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/aws/request/get__current_user.py` & `volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/request/get__current_user.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/aws/request/post__login.py` & `volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/request/post__login.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/aws/request/post__signup.py` & `volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/request/post__signup.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.8/src/volworld_aws_api_common/test/request.py` & `volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/request.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.8/src/volworld_aws_api_common.egg-info/SOURCES.txt` & `volworld_aws_api_common-0.1.9/src/volworld_aws_api_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

