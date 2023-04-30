# Comparing `tmp/python-runit-0.0.9.tar.gz` & `tmp/python-runit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-runit-0.0.9.tar", last modified: Mon Dec 12 00:13:20 2022, max compression
+gzip compressed data, was "python-runit-0.1.0.tar", last modified: Sun Apr 30 20:37:12 2023, max compression
```

## Comparing `python-runit-0.0.9.tar` & `python-runit-0.1.0.tar`

### file list

```diff
@@ -1,68 +1,71 @@
-drwxrwxrwx   0        0        0        0 2022-12-12 00:13:20.402922 python-runit-0.0.9/
--rw-rw-rw-   0        0        0       89 2022-12-02 15:17:26.000000 python-runit-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     4639 2022-12-12 00:13:20.399917 python-runit-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3779 2022-11-18 15:19:03.000000 python-runit-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2022-12-12 00:13:17.999918 python-runit-0.0.9/python_runit.egg-info/
--rw-rw-rw-   0        0        0     4639 2022-12-12 00:13:17.000000 python-runit-0.0.9/python_runit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1587 2022-12-12 00:13:17.000000 python-runit-0.0.9/python_runit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-12 00:13:17.000000 python-runit-0.0.9/python_runit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2022-12-12 00:13:17.000000 python-runit-0.0.9/python_runit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2022-12-12 00:13:17.000000 python-runit-0.0.9/python_runit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-12-12 00:13:17.000000 python-runit-0.0.9/python_runit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-12-12 00:13:18.363920 python-runit-0.0.9/runit/
--rw-rw-rw-   0        0        0      730 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/Request.py
--rw-rw-rw-   0        0        0      376 2022-12-10 20:04:06.000000 python-runit-0.0.9/runit/__init__.py
--rw-rw-rw-   0        0        0    12091 2022-12-11 23:40:45.000000 python-runit-0.0.9/runit/cli.py
--rw-rw-rw-   0        0        0     1024 2022-12-11 20:00:13.000000 python-runit-0.0.9/runit/constants.py
-drwxrwxrwx   0        0        0        0 2022-12-12 00:13:18.654935 python-runit-0.0.9/runit/languages/
--rw-rw-rw-   0        0        0      820 2022-12-07 17:56:59.000000 python-runit-0.0.9/runit/languages/__init__.py
--rw-rw-rw-   0        0        0      503 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/languages/javascript.py
--rw-rw-rw-   0        0        0      487 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/languages/php.py
--rw-rw-rw-   0        0        0      485 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/languages/python.py
--rw-rw-rw-   0        0        0     2514 2022-12-07 18:06:28.000000 python-runit-0.0.9/runit/languages/runtime.py
-drwxrwxrwx   0        0        0        0 2022-12-12 00:13:18.709922 python-runit-0.0.9/runit/modules/
--rw-rw-rw-   0        0        0       30 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/modules/__init__.py
--rw-rw-rw-   0        0        0     8940 2022-12-11 23:59:39.000000 python-runit-0.0.9/runit/modules/account.py
--rw-rw-rw-   0        0        0     9559 2022-12-10 20:19:43.000000 python-runit-0.0.9/runit/runit.py
-drwxrwxrwx   0        0        0        0 2022-12-12 00:13:18.774924 python-runit-0.0.9/runit/templates/
--rw-rw-rw-   0        0        0     1157 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/404.html
-drwxrwxrwx   0        0        0        0 2022-12-12 00:13:19.285928 python-runit-0.0.9/runit/templates/javascript/
--rw-rw-rw-   0        0        0       13 2022-09-03 23:35:52.000000 python-runit-0.0.9/runit/templates/javascript/.env
--rw-rw-rw-   0        0        0     1157 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/javascript/404.html
--rw-rw-rw-   0        0        0      259 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/javascript/main.js
--rw-rw-rw-   0        0        0      299 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/javascript/package.json
--rw-rw-rw-   0        0        0      250 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/javascript/runit.json
-drwxrwxrwx   0        0        0        0 2022-12-12 00:13:19.740926 python-runit-0.0.9/runit/templates/php/
--rw-rw-rw-   0        0        0       12 2022-09-03 23:35:52.000000 python-runit-0.0.9/runit/templates/php/.env
--rw-rw-rw-   0        0        0     1122 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/php/404.html
--rw-rw-rw-   0        0        0      276 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/php/composer.json
--rw-rw-rw-   0        0        0      227 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/php/index.php
--rw-rw-rw-   0        0        0      392 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/php/request.php
--rw-rw-rw-   0        0        0      242 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/php/runit.json
--rw-rw-rw-   0        0        0       27 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/php/test.php
-drwxrwxrwx   0        0        0        0 2022-12-12 00:13:19.889923 python-runit-0.0.9/runit/templates/python/
--rw-rw-rw-   0        0        0       18 2022-09-03 23:35:52.000000 python-runit-0.0.9/runit/templates/python/.env
--rw-rw-rw-   0        0        0     1157 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/python/404.html
--rw-rw-rw-   0        0        0     1182 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/python/application.py
-drwxrwxrwx   0        0        0        0 2022-12-12 00:13:19.967924 python-runit-0.0.9/runit/templates/python/packages/
--rw-rw-rw-   0        0        0      807 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/python/packages/Request.py
--rw-rw-rw-   0        0        0       59 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/python/packages/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-12 00:13:20.076916 python-runit-0.0.9/runit/templates/python/packages/__pycache__/
--rw-rw-rw-   0        0        0     1070 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/python/packages/__pycache__/Request.cpython-310.pyc
--rw-rw-rw-   0        0        0      216 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/python/packages/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      213 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/python/packages/__pycache__/modules.cpython-310.pyc
--rw-rw-rw-   0        0        0      363 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/python/requirements.txt
--rw-rw-rw-   0        0        0      255 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/templates/python/runit.json
--rw-rw-rw-   0        0        0      404 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/test.py
-drwxrwxrwx   0        0        0        0 2022-12-12 00:13:17.846922 python-runit-0.0.9/runit/tools/
-drwxrwxrwx   0        0        0        0 2022-12-12 00:13:20.190929 python-runit-0.0.9/runit/tools/javascript/
--rw-rw-rw-   0        0        0      250 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/tools/javascript/loader.js
--rw-rw-rw-   0        0        0      493 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/tools/javascript/runner.js
-drwxrwxrwx   0        0        0        0 2022-12-12 00:13:20.330921 python-runit-0.0.9/runit/tools/php/
--rw-rw-rw-   0        0        0      362 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/tools/php/loader.php
--rw-rw-rw-   0        0        0      630 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/tools/php/runner.php
-drwxrwxrwx   0        0        0        0 2022-12-12 00:13:20.393916 python-runit-0.0.9/runit/tools/python/
--rw-rw-rw-   0        0        0      380 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/tools/python/loader.py
--rw-rw-rw-   0        0        0      639 2022-11-16 16:12:51.000000 python-runit-0.0.9/runit/tools/python/runner.py
--rw-rw-rw-   0        0        0       42 2022-12-12 00:13:20.403923 python-runit-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1433 2022-12-11 20:00:37.000000 python-runit-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.655633 python-runit-0.1.0/
+-rw-rw-rw-   0        0        0     1090 2023-04-30 20:35:32.000000 python-runit-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0       89 2022-12-02 15:17:26.000000 python-runit-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4662 2023-04-30 20:37:12.653631 python-runit-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3779 2022-11-18 15:19:03.000000 python-runit-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.091405 python-runit-0.1.0/python_runit.egg-info/
+-rw-rw-rw-   0        0        0     4662 2023-04-30 20:37:11.000000 python-runit-0.1.0/python_runit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1561 2023-04-30 20:37:11.000000 python-runit-0.1.0/python_runit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 20:37:11.000000 python-runit-0.1.0/python_runit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-30 20:37:11.000000 python-runit-0.1.0/python_runit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-04-30 20:37:11.000000 python-runit-0.1.0/python_runit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-30 20:37:11.000000 python-runit-0.1.0/python_runit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.159412 python-runit-0.1.0/runit/
+-rw-rw-rw-   0        0        0      767 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/Request.py
+-rw-rw-rw-   0        0        0      376 2022-12-10 20:04:06.000000 python-runit-0.1.0/runit/__init__.py
+-rw-rw-rw-   0        0        0    12358 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/cli.py
+-rw-rw-rw-   0        0        0     2064 2023-04-30 20:35:32.000000 python-runit-0.1.0/runit/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.251402 python-runit-0.1.0/runit/languages/
+-rw-rw-rw-   0        0        0     1004 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/languages/__init__.py
+-rw-rw-rw-   0        0        0      503 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/languages/javascript.py
+-rw-rw-rw-   0        0        0     3704 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/languages/multi.py
+-rw-rw-rw-   0        0        0      487 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/languages/php.py
+-rw-rw-rw-   0        0        0      485 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/languages/python.py
+-rw-rw-rw-   0        0        0     2425 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/languages/runtime.py
+drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.285884 python-runit-0.1.0/runit/modules/
+-rw-rw-rw-   0        0        0       30 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/modules/__init__.py
+-rw-rw-rw-   0        0        0     8941 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/modules/account.py
+-rw-rw-rw-   0        0        0    13182 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/runit.py
+drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.323636 python-runit-0.1.0/runit/templates/
+-rw-rw-rw-   0        0        0       67 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/.runitignore
+-rw-rw-rw-   0        0        0     1157 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/templates/404.html
+drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.342624 python-runit-0.1.0/runit/templates/javascript/
+-rw-rw-rw-   0        0        0       13 2022-09-03 23:35:52.000000 python-runit-0.1.0/runit/templates/javascript/.env
+-rw-rw-rw-   0        0        0      259 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/templates/javascript/main.js
+-rw-rw-rw-   0        0        0      299 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/templates/javascript/package.json
+-rw-rw-rw-   0        0        0      270 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/javascript/runit.json
+drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.550056 python-runit-0.1.0/runit/templates/multi/
+-rw-rw-rw-   0        0        0     1182 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/multi/application.py
+-rw-rw-rw-   0        0        0      277 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/multi/composer.json
+-rw-rw-rw-   0        0        0      227 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/multi/index.php
+-rw-rw-rw-   0        0        0      259 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/multi/main.js
+-rw-rw-rw-   0        0        0      299 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/multi/package.json
+-rw-rw-rw-   0        0        0      392 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/multi/request.php
+-rw-rw-rw-   0        0        0        0 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/multi/requirements.txt
+-rw-rw-rw-   0        0        0       27 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/multi/test.php
+drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.579630 python-runit-0.1.0/runit/templates/php/
+-rw-rw-rw-   0        0        0       12 2022-09-03 23:35:52.000000 python-runit-0.1.0/runit/templates/php/.env
+-rw-rw-rw-   0        0        0      277 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/php/composer.json
+-rw-rw-rw-   0        0        0      227 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/templates/php/index.php
+-rw-rw-rw-   0        0        0      392 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/templates/php/request.php
+-rw-rw-rw-   0        0        0      262 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/php/runit.json
+-rw-rw-rw-   0        0        0       27 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/templates/php/test.php
+drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.622630 python-runit-0.1.0/runit/templates/python/
+-rw-rw-rw-   0        0        0       18 2022-09-03 23:35:52.000000 python-runit-0.1.0/runit/templates/python/.env
+-rw-rw-rw-   0        0        0     1182 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/templates/python/application.py
+-rw-rw-rw-   0        0        0      363 2023-04-30 20:35:32.000000 python-runit-0.1.0/runit/templates/python/requirements.txt
+-rw-rw-rw-   0        0        0      275 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/python/runit.json
+-rw-rw-rw-   0        0        0      266 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/runit.json
+-rw-rw-rw-   0        0        0      404 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/test.py
+drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.020402 python-runit-0.1.0/runit/tools/
+drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.630628 python-runit-0.1.0/runit/tools/javascript/
+-rw-rw-rw-   0        0        0      250 2023-04-30 18:54:45.000000 python-runit-0.1.0/runit/tools/javascript/loader.js
+-rw-rw-rw-   0        0        0      490 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/tools/javascript/runner.js
+drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.640631 python-runit-0.1.0/runit/tools/php/
+-rw-rw-rw-   0        0        0      362 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/tools/php/loader.php
+-rw-rw-rw-   0        0        0      630 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/tools/php/runner.php
+drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.648627 python-runit-0.1.0/runit/tools/python/
+-rw-rw-rw-   0        0        0      380 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/tools/python/loader.py
+-rw-rw-rw-   0        0        0      639 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/tools/python/runner.py
+-rw-rw-rw-   0        0        0       42 2023-04-30 20:37:12.656627 python-runit-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1433 2023-04-30 20:35:32.000000 python-runit-0.1.0/setup.py
```

### Comparing `python-runit-0.0.9/PKG-INFO` & `python-runit-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-runit
-Version: 0.0.9
+Version: 0.1.0
 Summary: Develop serverless applications
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/runit/
 Project-URL: Tracker, https://github.com/theonlyamos/runit/issues
 Keywords: python3 runit developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
 
 # Runit CLI ![Python](https://img.shields.io/badge/builthwith-python-brightgreen) 
 The Runit Command Line Interface (CLI) Tools can be used to test, manage, and deploy your Runit project from the command line.
 - Create new runit project
 - Run a local web server for your runit project
 - publish code and assets to your runit-server domain
 - Interact with data in your runit-server database
```

### Comparing `python-runit-0.0.9/README.md` & `python-runit-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `python-runit-0.0.9/python_runit.egg-info/PKG-INFO` & `python-runit-0.1.0/python_runit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-runit
-Version: 0.0.9
+Version: 0.1.0
 Summary: Develop serverless applications
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/runit/
 Project-URL: Tracker, https://github.com/theonlyamos/runit/issues
 Keywords: python3 runit developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
 
 # Runit CLI ![Python](https://img.shields.io/badge/builthwith-python-brightgreen) 
 The Runit Command Line Interface (CLI) Tools can be used to test, manage, and deploy your Runit project from the command line.
 - Create new runit project
 - Run a local web server for your runit project
 - publish code and assets to your runit-server domain
 - Interact with data in your runit-server database
```

### Comparing `python-runit-0.0.9/runit/Request.py` & `python-runit-0.1.0/runit/Request.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import requests
+import os
 
 class Request:
     def __init__(self):
-        req = requests.get('http://localhost:9000/get_app_requests/', headers={'Accept': 'application/json'})
+        req = requests.get(os.getenv('RUNIT_SERVERNAME', 'localhost:9000')+'get_app_requests/', headers={'Accept': 'application/json'})
         self.parameters = req.json()
 
     def args(self):
         return self.parameters
     
     def get(self, name=None):
         if name == None:
```

### Comparing `python-runit-0.0.9/runit/cli.py` & `python-runit-0.1.0/runit/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 from flask import Flask, request
 from dotenv import load_dotenv, set_key, find_dotenv, dotenv_values
 
 from .languages import LanguageParser
 from .modules import Account
 from .runit import RunIt
 
-from .constants import VERSION, CURRENT_PROJECT, CURRENT_PROJECT_DIR, EXT_TO_RUNTIME
+from .constants import VERSION, CURRENT_PROJECT, CURRENT_PROJECT_DIR, EXT_TO_RUNTIME, \
+                        LANGUAGE_TO_RUNTIME
 
 load_dotenv()
 
 def StartWebserver(project: Type[RunIt], host: str = '127.0.0.1', port: int = 5000):
     app = Flask(__name__)
     app.secret = "fdakfjlfdsaflfkjbasdoiefanckdareafasdfkowadbfakidfadfkj"
     try:
         app.add_url_rule('/', view_func=project.serve)
         app.add_url_rule('/<func>', view_func=project.serve)
         app.add_url_rule('/<func>/', view_func=project.serve)
-        app.run(host, port, True)
+        app.run(host, port, False)
     except KeyboardInterrupt:
         sys.exit(1)
     except Exception as e:
         print(e)
 
 def create_new_project(args):
     global CONFIG_FILE
@@ -46,15 +47,16 @@
             print(f'{name} project already Exists')
             sys.exit(1)
         
         CONFIG_FILE = 'runit.json'
         config = {}
         config['name'] = args.name
         config['language'] = args.language
-        config['runtime'] = args.runtime
+        config['runtime'] = args.runtime if args.runtime else LANGUAGE_TO_RUNTIME[args.language]
+        config['private'] = args.private
         config['author'] = {}
         config['author']['name'] = getpass.getuser()
         config['author']['email'] = "name@example.com"
         
         user = Account.user()
         os.chdir(CURRENT_PROJECT_DIR)
         if user is not None:
@@ -144,22 +146,20 @@
     
     print('[#] Files Uploaded!!!')
     if 'project_id' in result.keys():
         project._id = result['project_id']
         project.homepage = result['homepage']
         project.update_config()
         print('[*] Project config updated')
-        if find_dotenv():
-            print(find_dotenv())
-            set_key(find_dotenv(), 'RUNIT_PROJECT_ID', result['project_id'])
+        # if find_dotenv():
+        #     set_key(find_dotenv(), 'RUNIT_PROJECT_ID', result['project_id'])
 
     print('[*] Project published successfully')
     print('[!] Access your functions with the urls below:')
 
-    print(f"[-] {result['homepage']}")
     for func_url in result['functions']:
         print(f"[-] {func_url}")
 
 def setup_runit(args):
     '''
     Setup Runit server side api
     
@@ -213,18 +213,20 @@
     global parser
     global VERSION
     
     subparsers = parser.add_subparsers()
     new_parser = subparsers.add_parser('new', help='Create new project or function')
     new_parser.add_argument("name", type=str, nargs="?", 
                         help="Name of the new project")          
-    new_parser.add_argument('-l', '--language', type=str, choices=['python', 'php', 'javascript'],
-                        help="Language of the new project")
+    new_parser.add_argument('-l', '--language', type=str, choices=['multi' 'python', 'php', 'javascript'],
+                        help="Language of the new project", default="multi")
     new_parser.add_argument('-r','--runtime', type=str,
-                        help="Runtime of the project language. E.g: python3.10, node")
+                        help="Runtime of the project language. E.g: python3.11, node, php8")
+    new_parser.add_argument('--private', action='store_true', 
+                        help="Make project publicly accessible or not. Default is public.")
     new_parser.set_defaults(func=create_new_project)
     
     # run_parser = subparsers.add_parser('run', help='Run current|specified project|function')
     # run_parser.add_argument('function', default='index', type=str, nargs='?', help='Name of function to run')
     # run_parser.add_argument('--file', type=str, nargs='?', help='Name of file to run')
     # run_parser.add_argument('--shell', action='store_true', help='Run function only in shell')
     # run_parser.add_argument('-x', '--arguments', action='append', default=[], help='Comma separated function arguments')
@@ -303,8 +305,8 @@
 
     except FileNotFoundError:
         print('No runit project or file to run\n')
         parser.print_help()
         sys.exit(1)
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `python-runit-0.0.9/runit/languages/__init__.py` & `python-runit-0.1.0/runit/languages/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from typing import Type
-from .python import Python
 from .php import PHP
+from .multi import Multi
+from .python import Python
 from .javascript import Javascript
 
 import os
 from typing import Union
 
 class LanguageParser(object):
     '''
     Class for parsing script language.
     Determines which language paackage
     to use
     '''
 
-    EXT_TO_LANG = {'.py': Python, '.php': PHP, '.js': Javascript}
+    EXT_TO_LANG = {'.py': Python, '.php': PHP, '.js': Javascript,
+                   '.jsx': Javascript, '.ts': Javascript, '.tsx': Javascript}
 
     def __init__(self):
         pass
     
     @staticmethod
     def detect_language(filename: str, runtime: str)-> Union[Python, PHP, Javascript]:
+        if runtime == 'multi':
+            return Multi(filename, runtime)
         return LanguageParser.EXT_TO_LANG[os.path.splitext(filename)[1].lower()](filename, runtime)
 
     @staticmethod
     def run_file(filename, runtime):
         lang_parser = LanguageParser.detect_language(filename, runtime)
         lang_parser.is_file = True
-        lang_parser.anon_function()
+        lang_parser.anon_function()
```

### Comparing `python-runit-0.0.9/runit/languages/runtime.py` & `python-runit-0.1.0/runit/languages/runtime.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,57 @@
-from datetime import datetime, timedelta
-from dotenv import load_dotenv
 import os
-
+from datetime import datetime, timedelta
 from subprocess import check_output
-from typing import Any
+
+from dotenv import load_dotenv
+from ..constants import EXT_TO_RUNTIME
 
 load_dotenv()
 
 class Runtime(object):
     '''
     Class for parsing and running
     functions from file
     '''
     LOADER = ""
     RUNNER = ""
     
     def __init__(self, filename="", runtime="", is_file = False):
+        extension = os.path.splitext(filename)[1].lower()
         self.filename = filename
         self.runtime = runtime
         self.is_file = is_file
         self.module = os.path.realpath(os.path.join(os.curdir, self.filename))
         self.functions = []
-        self.load_functions_from_file()
+        self.load_functions_from_supported_files()
     
-    def load_functions_from_file(self):
+    def load_functions_from_supported_files(self):
         '''
-        Class method for retrieving exported
+        Class method for loading exported
         function names in .js file
 
         @param None
         @return None
         '''
         
         try:
-            command = check_output(f'{self.runtime} {self.LOADER} {self.module}', shell=True)
-            result = str(command)
-            result = result.lstrip("b'").lstrip('"').replace('\\n', '\n').replace('\\r', '\r').rstrip("'").rstrip('"').strip()
-            
+            result = check_output(f'{self.runtime} {self.LOADER} {self.module}', shell=True, encoding='utf-8')
+            result = result.strip()
             if self.runtime == 'php':
                 self.functions = result.split(',')
             else:
                 self.functions = eval(result)
 
             for key in self.functions:
                 self.__setattr__(key, self.anon_function)
                 
         except Exception as e:
             print(str(e))
             return str(e)
-
+        
     def list_functions(self):
         '''
         List Class methods
 
         @param None
         @retun None
         '''
@@ -61,18 +60,17 @@
     def anon_function(self, *args):
         args = ', '.join(args)
         try:
             if len(args):
                 if self.is_file:
                     return os.system(f'{self.runtime} {self.filename} "{args}"')
                 else:
-                    command = check_output(f'{self.runtime} {self.RUNNER} {self.module} {self.current_func} "{args}"', shell=True)
+                    result = check_output(f'{self.runtime} {self.RUNNER} {self.module} {self.current_func} "{args}"', shell=True, encoding='utf-8')
             else:
                 if self.is_file:
                     return os.system(f'{self.runtime} {self.filename}')
                 else:
-                    command = check_output(f'{self.runtime} {self.RUNNER} {self.module} {self.current_func}', shell=True)
+                    result = check_output(f'{self.runtime} {self.RUNNER} {self.module} {self.current_func}', shell=True, encoding='utf-8')
 
-            result = str(command)
-            return result.lstrip("b'").replace('\\n', '\n').replace('\\r', '\r').rstrip("'").strip()
+            return result.strip()
         except Exception as e:
             return str(e)
```

### Comparing `python-runit-0.0.9/runit/modules/account.py` & `python-runit-0.1.0/runit/modules/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             request = requests.get(url, headers=BASE_HEADERS)
             result = request.json()
             if 'msg' in result.keys():
                 raise Exception(result['msg'])
             return result
 
         except Exception as e:
-            print(str(e))
+            #print(str(e))
             return None
   
     @staticmethod
     def info(args):
         '''
         Retrieve account details
```

### Comparing `python-runit-0.0.9/runit/runit.py` & `python-runit-0.1.0/runit/runit.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,38 +9,40 @@
 
 from flask import request
 from dotenv import load_dotenv
 
 from .languages import LanguageParser
 from .constants import TEMPLATES_FOLDER, STARTER_FILES, NOT_FOUND_FILE, \
         CONFIG_FILE, STARTER_CONFIG_FILE, IS_RUNNING, PROJECTS_DIR, \
-        CURRENT_PROJECT_DIR
+        CURRENT_PROJECT_DIR, DOT_RUNIT_IGNORE
 
 load_dotenv()
 class RunIt:
     def __init__(self, name, _id="", version="0.0.1", description="", homepage="",
-    language="", runtime="", start_file="", author={}, is_file: bool = False):
+    language="", runtime="", start_file="", private=False, author={}, is_file: bool = False):
         global STARTER_FILES
 
         self._id = _id
         self.name = name
         self.version = version
         self.description = description
         self.homepage = homepage
         self.language = language
         self.runtime = runtime
+        self.private = private
         self.author = author
         self.config = {}
         self.start_file = start_file if start_file else STARTER_FILES[self.language]
         self.create_config()
         
         if not RunIt.has_config_file() and not is_file:
             self.create_folder()
             self.dump_config()
             self.create_starter_files()
+            self.language_depending_packaging()
     
     def __repr__(self):
         return json.dumps(self.config, indent=4)
 
     @staticmethod
     def exists(name):
         return os.path.exists(os.path.join(os.curdir, name))
@@ -90,14 +92,25 @@
                 
             while not name:
                 name = str(input('Enter RunIt Name: '))
             return name
         except KeyboardInterrupt:
             sys.exit(1)
 
+    @classmethod
+    def is_private(cls, project_id: str, projects_folder: str = PROJECTS_DIR)-> bool:
+        global NOT_FOUND_FILE
+
+        os.chdir(projects_folder)
+        
+        if not RunIt.has_config_file():
+            return False
+        
+        project = cls(**RunIt.load_config())
+        return project.private
 
     @classmethod
     def start(cls, project_id: str, func='index', projects_folder: str = PROJECTS_DIR):
         global NOT_FOUND_FILE
 
         os.chdir(projects_folder)
         
@@ -146,50 +159,52 @@
     def get_functions(self)->list:
         lang_parser = LanguageParser.detect_language(self.start_file, self.runtime)
         return lang_parser.list_functions()
     
     def serve(self, func: str = 'index', args: Optional[Union[dict,list]]=None, filename: str = ''):
         global NOT_FOUND_FILE
         global request
-
-        lang_parser = LanguageParser.detect_language(self.start_file, self.runtime)
-        lang_parser.current_func = func
         
+        lang_parser = LanguageParser.detect_language(self.start_file, self.runtime)
+        setattr(lang_parser, 'current_func', func)
+
         if not args and request:
             args = dict(request.args)
 
         args_list = args if type(args) == list else []
         
         if type(args) == dict:
             for key, value in args.items():
                 args_list.append(value)
-
+        
         try:
             return getattr(lang_parser, func)(*args_list)
         except AttributeError as e:
             return RunIt.notfound()
             # return f"Function with name '{func}' not defined!"
         except TypeError as e:
             try:
                 return getattr(lang_parser, func)()
             except TypeError as e:
                 return str(e)
+        except Exception as e:
+            return str(e)
     
     def create_folder(self):
         os.mkdir(os.path.join(os.curdir, self.name))
 
     def dump_config(self):
         global CONFIG_FILE
 
         if isinstance(CONFIG_FILE, str):
             config_file = open(os.path.join(os.curdir, self.name,
             CONFIG_FILE),'wt')
         else:
             config_file = CONFIG_FILE
-
+        
         json.dump(self.config, config_file, indent=4)
         config_file.close()
 
     def update_config(self):
         global CONFIG_FILE
         global STARTER_CONFIG_FILE
 
@@ -201,74 +216,149 @@
         self.config['_id'] = self._id
         self.config['name'] = self.name
         self.config['version'] = self.version
         self.config['description'] = self.description
         self.config['homepage'] = self.homepage
         self.config['language'] = self.language
         self.config['runtime'] = self.runtime
+        self.config['private'] = self.private
         self.config['start_file'] = self.start_file
         self.config['author'] = self.author
         json.dump(self.config, config_file, indent=4)
         config_file.close()
     
     def compress(self):
         os.chdir(CURRENT_PROJECT_DIR)
 
         zipname = f'{self.name}.zip'
+        
         exclude_list = [zipname, 'account.db']
         
+        with open('.runitignore', 'rt') as file:
+            for line in file.readlines():
+                if line:
+                    exclude_list.append(os.path.normpath(line.strip()))
+        
+        del exclude_list[exclude_list.index('.')]
         with ZipFile(zipname, 'w') as zipobj:
             print('[!] Compressing Project Files...')
             for folderName, subfolders, filenames in os.walk(os.curdir):
+                
                 for filename in filenames:
-                    filepath = os.path.join(folderName,  filename)
-                    
-                    if not os.path.basename(filepath) in exclude_list and not '__pycache__' in folderName:
-                        zipobj.write(filepath, filepath)
-                        print(f'[{filepath}] Compressed!')
+                    if not os.path.normpath(os.path.dirname(folderName)).split(os.path.sep)[0] in exclude_list:
+                        filepath = os.path.join(folderName,  filename)
+
+                        if not os.path.basename(filepath) in exclude_list and not '__pycache__' in folderName:
+                            zipobj.write(filepath, filepath)
+                            print(f'[{filepath}] Compressed!')
             print(f'[!] Filename: {zipname}')
         return zipname
 
     def create_config(self):
         self.config['_id'] = self._id
         self.config['name'] = self.name
         self.config['version'] = self.version
         self.config['description'] = self.description
         self.config['homepage'] = 'https://example.com/project_id/'
         self.config['language'] = self.language
         self.config['runtime'] = self.runtime
+        self.config['private'] = self.private
         self.config['start_file'] = self.start_file
         self.config['author'] = self.author
     
     def create_starter_files(self):
+        global DOT_RUNIT_IGNORE
         global TEMPLATES_FOLDER
         global NOT_FOUND_FILE
         
-        with open(os.path.join(os.curdir, TEMPLATES_FOLDER, self.language,
-            self.start_file),'rt') as file:
-            with open(os.path.join(os.curdir, self.name, self.start_file), 'wt') as starter:
-                starter.write(file.read())
+        self.LANGUAGE_TEMPLATE_FOLDER = os.path.realpath(os.path.join(TEMPLATES_FOLDER, self.language))
+        self.LANGUAGE_TEMPLATE_FILES = os.listdir(self.LANGUAGE_TEMPLATE_FOLDER)
         
-        with open(os.path.join(os.curdir, TEMPLATES_FOLDER, NOT_FOUND_FILE),'rt') as file:
+        for template_file in self.LANGUAGE_TEMPLATE_FILES:
+            with open(os.path.join(self.LANGUAGE_TEMPLATE_FOLDER,
+                template_file),'rt') as file:
+                with open(os.path.join(os.curdir, self.name, template_file), 'wt') as starter:
+                    starter.write(file.read())
+            
+        with open(os.path.join(TEMPLATES_FOLDER, NOT_FOUND_FILE),'rt') as file:
             with open(os.path.join(os.curdir, self.name, NOT_FOUND_FILE), 'wt') as error:
                 error.write(file.read())
         
-        '''
-        with open(os.path.join(os.curdir, 'runit-cli.py'),'rt') as file:
-            with open(os.path.join(os.curdir, self.name, 'runit-cli.py'), 'wt') as client:
-                client.write(file.read())
-        '''
-
-        if self.language.startswith('python'):
-            PACKAGES_FOLDER = 'packages'
-            os.mkdir(os.path.join(os.curdir, self.name, PACKAGES_FOLDER))
-            for filename in os.listdir(os.path.abspath(os.path.join(os.curdir, TEMPLATES_FOLDER, self.language, PACKAGES_FOLDER))):
-                if os.path.isfile(os.path.join(os.curdir, TEMPLATES_FOLDER, self.language,
-                    PACKAGES_FOLDER, filename)):
-                    with open(os.path.join(os.curdir, TEMPLATES_FOLDER, self.language,
-                        PACKAGES_FOLDER, filename),'rt') as file:
-                        with open(os.path.join(os.curdir, self.name, PACKAGES_FOLDER, filename), 'wt') as package:
-                            package.write(file.read())
-
-
-
+        with open(os.path.join(TEMPLATES_FOLDER, DOT_RUNIT_IGNORE),'rt') as file:
+            with open(os.path.join(os.curdir, self.name, DOT_RUNIT_IGNORE), 'wt') as dotrunitignore:
+                dotrunitignore.write(file.read())
+    
+    def language_depending_packaging(self):
+        # os.chdir(os.path.join(os.curdir, self.name))
+        packaging_functions = {}
+        packaging_functions['javascript'] = self.update_and_install_package_json
+        packaging_functions['php'] = self.update_and_install_composer_json
+        packaging_functions['python'] = self.install_python_packages
+        packaging_functions['multi'] = self.install_all_language_packages
+        packaging_functions[self.language]()
+    
+    def install_all_language_packages(self):
+        try:
+            print("[+] Installing all packages...")
+            self.update_and_install_package_json()
+            self.update_and_install_composer_json()
+            self.install_python_packages()
+        except:
+            print("[!] Couldn't install packages")
+            print("[~] Try again manually later.")
+    
+    def update_and_install_package_json(self):
+        print("[-] Creating and updating package.json")
+        package_file = open('package.json', 'rt')
+        package_details = json.load(package_file)
+        package_file.close()
+        
+        package_details['name'] = self.name
+        package_details['author'] = self.author
+        
+        package_file = open('package.json', 'wt')
+        json.dump(package_details, package_file, indent=4)
+        package_file.close()
+        try:
+            print('[-] Installing node modules...')
+            os.system('npm install')
+        except Exception as e:
+            print(str(e))
+            print("[!] Couldn't install modules")
+            print("[~] Try again manually later.")
+        
+
+    def update_and_install_composer_json(self):
+        print("[-] Creating and updating composer.json")
+        package_file = open('composer.json', 'rt')
+        package_details = json.load(package_file)
+        package_file.close()
+        
+        package_details['name'] = f"runit/{self.name.replace('-', '_')}"
+        package_details['author'] = self.author
+        
+        package_file = open('composer.json', 'wt')
+        json.dump(package_details, package_file, indent=4)
+        package_file.close()
+        # try:
+        #     print('[-] Installing php packages...')
+        #     os.system('composer install')
+        # except Exception as e:
+        #     print(str(e))
+        #     print("[!] Couldn't install packages")
+        #     print("[~] Try again manually later.")
+    
+    def install_python_packages(self):
+        print("[-] Creating virtual environment")
+        os.system(f"python -m venv venv")
+        pip_path = os.path.join(os.curdir, 'venv', 'Scripts', 'pip.exe')
+        try:
+            print("[-] Installing python packages")
+            activate_install_instructions = f"""
+            {pip_path} install -r requirements.txt
+            """.strip()
+            os.system(activate_install_instructions)
+        except Exception as e:
+            print(str(e))
+            print("[!] Couldn't install packages")
+            print("[~] Try again manually later.")
```

### Comparing `python-runit-0.0.9/runit/templates/404.html` & `python-runit-0.1.0/runit/templates/404.html`

 * *Files identical despite different names*

### Comparing `python-runit-0.0.9/runit/templates/python/application.py` & `python-runit-0.1.0/runit/templates/multi/application.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.0.9/runit/tools/php/runner.php` & `python-runit-0.1.0/runit/tools/php/runner.php`

 * *Files identical despite different names*

### Comparing `python-runit-0.0.9/runit/tools/python/runner.py` & `python-runit-0.1.0/runit/tools/python/runner.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.0.9/setup.py` & `python-runit-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib.metadata import entry_points
 from setuptools import setup, find_packages
 
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 
 with open('README.md', 'rt') as file:
     LONG_DESCRIPTION = file.read()
 
 setup(
     name='python-runit',
     version=VERSION,
```

