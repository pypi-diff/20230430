# Comparing `tmp/odoo-env-0.9.8.tar.gz` & `tmp/odoo-env-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odoo-env-0.9.8.tar", last modified: Thu Sep 26 01:28:45 2019, max compression
+gzip compressed data, was "dist/odoo-env-0.9.9.tar", last modified: Thu Sep 26 02:14:47 2019, max compression
```

## Comparing `odoo-env-0.9.8.tar` & `odoo-env-0.9.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 jobiols   (1000) jobiols   (1000)        0 2019-09-26 01:28:45.000000 odoo-env-0.9.8/
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)       80 2019-09-26 01:28:45.000000 odoo-env-0.9.8/setup.cfg
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)     8943 2019-09-26 00:41:51.000000 odoo-env-0.9.8/README.md
-drwxrwxr-x   0 jobiols   (1000) jobiols   (1000)        0 2019-09-26 01:28:45.000000 odoo-env-0.9.8/odoo_env/
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)     7904 2019-07-28 22:24:41.000000 odoo-env-0.9.8/odoo_env/client.py
-drwxrwxr-x   0 jobiols   (1000) jobiols   (1000)        0 2019-09-26 01:28:45.000000 odoo-env-0.9.8/odoo_env/data/
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)      676 2019-09-26 00:20:23.000000 odoo-env-0.9.8/odoo_env/data/odoo.conf
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)     1568 2019-06-22 13:49:31.000000 odoo-env-0.9.8/odoo_env/data/nginx.conf
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)     1172 2019-07-08 18:55:13.000000 odoo-env-0.9.8/odoo_env/options.py
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)      596 2019-07-08 18:19:59.000000 odoo-env-0.9.8/odoo_env/images.py
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)     4747 2019-09-26 00:11:46.000000 odoo-env-0.9.8/odoo_env/command.py
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)       46 2019-09-26 01:27:53.000000 odoo-env-0.9.8/odoo_env/__init__.py
--rwxrwxr-x   0 jobiols   (1000) jobiols   (1000)     2531 2019-05-19 05:13:33.000000 odoo-env-0.9.8/odoo_env/sd.py
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)    30373 2019-09-26 01:26:14.000000 odoo-env-0.9.8/odoo_env/odooenv.py
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)     1122 2019-07-08 18:18:52.000000 odoo-env-0.9.8/odoo_env/repos.py
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)      852 2019-05-19 03:38:44.000000 odoo-env-0.9.8/odoo_env/messages.py
--rwxrwxr-x   0 jobiols   (1000) jobiols   (1000)     7662 2019-07-14 20:09:54.000000 odoo-env-0.9.8/odoo_env/oe.py
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)      371 2018-11-17 17:34:47.000000 odoo-env-0.9.8/odoo_env/constants.py
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)    14798 2019-09-25 22:47:15.000000 odoo-env-0.9.8/odoo_env/test_oe.py
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)     1409 2019-09-25 22:04:52.000000 odoo-env-0.9.8/setup.py
-drwxrwxr-x   0 jobiols   (1000) jobiols   (1000)        0 2019-09-26 01:28:45.000000 odoo-env-0.9.8/odoo_env.egg-info/
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)        1 2019-09-26 01:28:44.000000 odoo-env-0.9.8/odoo_env.egg-info/dependency_links.txt
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)      501 2019-09-26 01:28:44.000000 odoo-env-0.9.8/odoo_env.egg-info/SOURCES.txt
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)        7 2019-09-26 01:28:44.000000 odoo-env-0.9.8/odoo_env.egg-info/requires.txt
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)    11174 2019-09-26 01:28:44.000000 odoo-env-0.9.8/odoo_env.egg-info/PKG-INFO
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)        9 2019-09-26 01:28:44.000000 odoo-env-0.9.8/odoo_env.egg-info/top_level.txt
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)       63 2019-09-26 01:28:44.000000 odoo-env-0.9.8/odoo_env.egg-info/entry_points.txt
--rw-rw-r--   0 jobiols   (1000) jobiols   (1000)    11174 2019-09-26 01:28:45.000000 odoo-env-0.9.8/PKG-INFO
+drwxrwxr-x   0 jobiols   (1000) jobiols   (1000)        0 2019-09-26 02:14:47.000000 odoo-env-0.9.9/
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)       80 2019-09-26 02:14:47.000000 odoo-env-0.9.9/setup.cfg
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)     8943 2019-09-26 00:41:51.000000 odoo-env-0.9.9/README.md
+drwxrwxr-x   0 jobiols   (1000) jobiols   (1000)        0 2019-09-26 02:14:47.000000 odoo-env-0.9.9/odoo_env/
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)     7904 2019-07-28 22:24:41.000000 odoo-env-0.9.9/odoo_env/client.py
+drwxrwxr-x   0 jobiols   (1000) jobiols   (1000)        0 2019-09-26 02:14:47.000000 odoo-env-0.9.9/odoo_env/data/
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)      638 2019-09-26 02:14:03.000000 odoo-env-0.9.9/odoo_env/data/odoo.conf
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)     1568 2019-06-22 13:49:31.000000 odoo-env-0.9.9/odoo_env/data/nginx.conf
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)     1172 2019-07-08 18:55:13.000000 odoo-env-0.9.9/odoo_env/options.py
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)      596 2019-07-08 18:19:59.000000 odoo-env-0.9.9/odoo_env/images.py
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)     4747 2019-09-26 00:11:46.000000 odoo-env-0.9.9/odoo_env/command.py
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)       46 2019-09-26 02:12:07.000000 odoo-env-0.9.9/odoo_env/__init__.py
+-rwxrwxr-x   0 jobiols   (1000) jobiols   (1000)     2531 2019-05-19 05:13:33.000000 odoo-env-0.9.9/odoo_env/sd.py
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)    30373 2019-09-26 01:26:14.000000 odoo-env-0.9.9/odoo_env/odooenv.py
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)     1122 2019-07-08 18:18:52.000000 odoo-env-0.9.9/odoo_env/repos.py
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)      852 2019-05-19 03:38:44.000000 odoo-env-0.9.9/odoo_env/messages.py
+-rwxrwxr-x   0 jobiols   (1000) jobiols   (1000)     7662 2019-07-14 20:09:54.000000 odoo-env-0.9.9/odoo_env/oe.py
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)      371 2018-11-17 17:34:47.000000 odoo-env-0.9.9/odoo_env/constants.py
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)    14798 2019-09-25 22:47:15.000000 odoo-env-0.9.9/odoo_env/test_oe.py
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)     1409 2019-09-25 22:04:52.000000 odoo-env-0.9.9/setup.py
+drwxrwxr-x   0 jobiols   (1000) jobiols   (1000)        0 2019-09-26 02:14:47.000000 odoo-env-0.9.9/odoo_env.egg-info/
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)        1 2019-09-26 02:14:47.000000 odoo-env-0.9.9/odoo_env.egg-info/dependency_links.txt
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)      501 2019-09-26 02:14:47.000000 odoo-env-0.9.9/odoo_env.egg-info/SOURCES.txt
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)        7 2019-09-26 02:14:47.000000 odoo-env-0.9.9/odoo_env.egg-info/requires.txt
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)    11174 2019-09-26 02:14:47.000000 odoo-env-0.9.9/odoo_env.egg-info/PKG-INFO
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)        9 2019-09-26 02:14:47.000000 odoo-env-0.9.9/odoo_env.egg-info/top_level.txt
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)       63 2019-09-26 02:14:47.000000 odoo-env-0.9.9/odoo_env.egg-info/entry_points.txt
+-rw-rw-r--   0 jobiols   (1000) jobiols   (1000)    11174 2019-09-26 02:14:47.000000 odoo-env-0.9.9/PKG-INFO
```

### Comparing `odoo-env-0.9.8/README.md` & `odoo-env-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `odoo-env-0.9.8/odoo_env/client.py` & `odoo-env-0.9.9/odoo_env/client.py`

 * *Files identical despite different names*

### Comparing `odoo-env-0.9.8/odoo_env/data/odoo.conf` & `odoo-env-0.9.9/odoo_env/data/odoo.conf`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 max_cron_threads = $max_cron_threads$
 db_user = odoo
 db_password = odoo
 db_host = db
 db_template = template1
 data_dir = /opt/odoo/data
 proxy_mode = True
-server_wide_modules = web,web_kanban,server_mode,database_tools
+server_wide_modules = web
 dbfilter = .*
 
 # other performance parameters
 db_maxconn = 32
 limit_memory_hard = $limit_memory_hard$
 limit_memory_soft = $limit_memory_soft$
 limit_request = $limit_request$
```

### Comparing `odoo-env-0.9.8/odoo_env/data/nginx.conf` & `odoo-env-0.9.9/odoo_env/data/nginx.conf`

 * *Files identical despite different names*

### Comparing `odoo-env-0.9.8/odoo_env/options.py` & `odoo-env-0.9.9/odoo_env/options.py`

 * *Files identical despite different names*

### Comparing `odoo-env-0.9.8/odoo_env/images.py` & `odoo-env-0.9.9/odoo_env/images.py`

 * *Files identical despite different names*

### Comparing `odoo-env-0.9.8/odoo_env/command.py` & `odoo-env-0.9.9/odoo_env/command.py`

 * *Files identical despite different names*

### Comparing `odoo-env-0.9.8/odoo_env/sd.py` & `odoo-env-0.9.9/odoo_env/sd.py`

 * *Files identical despite different names*

### Comparing `odoo-env-0.9.8/odoo_env/odooenv.py` & `odoo-env-0.9.9/odoo_env/odooenv.py`

 * *Files identical despite different names*

### Comparing `odoo-env-0.9.8/odoo_env/repos.py` & `odoo-env-0.9.9/odoo_env/repos.py`

 * *Files identical despite different names*

### Comparing `odoo-env-0.9.8/odoo_env/messages.py` & `odoo-env-0.9.9/odoo_env/messages.py`

 * *Files identical despite different names*

### Comparing `odoo-env-0.9.8/odoo_env/oe.py` & `odoo-env-0.9.9/odoo_env/oe.py`

 * *Files identical despite different names*

### Comparing `odoo-env-0.9.8/odoo_env/test_oe.py` & `odoo-env-0.9.9/odoo_env/test_oe.py`

 * *Files identical despite different names*

### Comparing `odoo-env-0.9.8/setup.py` & `odoo-env-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `odoo-env-0.9.8/odoo_env.egg-info/PKG-INFO` & `odoo-env-0.9.9/odoo_env.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-env
-Version: 0.9.8
+Version: 0.9.9
 Summary: An environment to manage Docker for Odoo
 Home-page: https://github.com/jobiols/odoo-env
 Author: Jorge E. Obiols
 Author-email: jorge.obiols@gmail.com
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/jobiols/odoo-env.svg?branch=master)](https://travis-ci.org/jobiols/odoo-env)
         [![codecov](https://codecov.io/gh/jobiols/odoo-env/branch/master/graph/badge.svg)](https://codecov.io/gh/jobiols/odoo-env)
```

### Comparing `odoo-env-0.9.8/PKG-INFO` & `odoo-env-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-env
-Version: 0.9.8
+Version: 0.9.9
 Summary: An environment to manage Docker for Odoo
 Home-page: https://github.com/jobiols/odoo-env
 Author: Jorge E. Obiols
 Author-email: jorge.obiols@gmail.com
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/jobiols/odoo-env.svg?branch=master)](https://travis-ci.org/jobiols/odoo-env)
         [![codecov](https://codecov.io/gh/jobiols/odoo-env/branch/master/graph/badge.svg)](https://codecov.io/gh/jobiols/odoo-env)
```

