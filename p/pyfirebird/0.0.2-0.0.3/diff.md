# Comparing `tmp/pyfirebird-0.0.2.tar.gz` & `tmp/pyfirebird-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfirebird-0.0.2.tar", last modified: Sun Apr 30 07:17:36 2023, max compression
+gzip compressed data, was "pyfirebird-0.0.3.tar", last modified: Sun Apr 30 07:22:32 2023, max compression
```

## Comparing `pyfirebird-0.0.2.tar` & `pyfirebird-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 07:17:36.299412 pyfirebird-0.0.2/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      367 2023-04-30 07:17:36.295412 pyfirebird-0.0.2/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        8 2023-04-30 05:34:25.000000 pyfirebird-0.0.2/README.md
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-04-30 07:17:36.299412 pyfirebird-0.0.2/setup.cfg
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1051 2023-04-30 07:16:38.000000 pyfirebird-0.0.2/setup.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 07:17:36.295412 pyfirebird-0.0.2/src/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 07:17:36.295412 pyfirebird-0.0.2/src/firebird/
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)      169 2023-04-30 06:39:02.000000 pyfirebird-0.0.2/src/firebird/__init__.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)    10042 2023-04-30 05:32:50.000000 pyfirebird-0.0.2/src/firebird/base.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 07:17:36.295412 pyfirebird-0.0.2/src/firebird/cmd_tools/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 05:45:15.000000 pyfirebird-0.0.2/src/firebird/cmd_tools/__init__.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     7301 2023-04-30 07:15:12.000000 pyfirebird-0.0.2/src/firebird/cmd_tools/executor.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     3115 2023-04-30 06:50:01.000000 pyfirebird-0.0.2/src/firebird/cmd_tools/pipeline.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2946 2023-04-30 06:57:56.000000 pyfirebird-0.0.2/src/firebird/cmd_tools/pipeline_impl.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2972 2023-04-30 05:32:50.000000 pyfirebird-0.0.2/src/firebird/rabbitmq.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     5696 2023-04-30 07:12:11.000000 pyfirebird-0.0.2/src/firebird/zkdb.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 07:17:36.295412 pyfirebird-0.0.2/src/pyfirebird.egg-info/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      367 2023-04-30 07:17:36.000000 pyfirebird-0.0.2/src/pyfirebird.egg-info/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      485 2023-04-30 07:17:36.000000 pyfirebird-0.0.2/src/pyfirebird.egg-info/SOURCES.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-04-30 07:17:36.000000 pyfirebird-0.0.2/src/pyfirebird.egg-info/dependency_links.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      106 2023-04-30 07:17:36.000000 pyfirebird-0.0.2/src/pyfirebird.egg-info/entry_points.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       27 2023-04-30 07:17:36.000000 pyfirebird-0.0.2/src/pyfirebird.egg-info/requires.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        9 2023-04-30 07:17:36.000000 pyfirebird-0.0.2/src/pyfirebird.egg-info/top_level.txt
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 07:22:32.460733 pyfirebird-0.0.3/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      367 2023-04-30 07:22:32.460733 pyfirebird-0.0.3/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        8 2023-04-30 05:34:25.000000 pyfirebird-0.0.3/README.md
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-04-30 07:22:32.460733 pyfirebird-0.0.3/setup.cfg
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1051 2023-04-30 07:22:28.000000 pyfirebird-0.0.3/setup.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 07:22:32.460733 pyfirebird-0.0.3/src/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 07:22:32.460733 pyfirebird-0.0.3/src/firebird/
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)      169 2023-04-30 06:39:02.000000 pyfirebird-0.0.3/src/firebird/__init__.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)    10042 2023-04-30 05:32:50.000000 pyfirebird-0.0.3/src/firebird/base.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 07:22:32.460733 pyfirebird-0.0.3/src/firebird/cmd_tools/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 05:45:15.000000 pyfirebird-0.0.3/src/firebird/cmd_tools/__init__.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     7301 2023-04-30 07:15:12.000000 pyfirebird-0.0.3/src/firebird/cmd_tools/executor.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2980 2023-04-30 07:22:18.000000 pyfirebird-0.0.3/src/firebird/cmd_tools/pipeline.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2946 2023-04-30 06:57:56.000000 pyfirebird-0.0.3/src/firebird/cmd_tools/pipeline_impl.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2972 2023-04-30 05:32:50.000000 pyfirebird-0.0.3/src/firebird/rabbitmq.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     5696 2023-04-30 07:12:11.000000 pyfirebird-0.0.3/src/firebird/zkdb.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 07:22:32.460733 pyfirebird-0.0.3/src/pyfirebird.egg-info/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      367 2023-04-30 07:22:32.000000 pyfirebird-0.0.3/src/pyfirebird.egg-info/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      485 2023-04-30 07:22:32.000000 pyfirebird-0.0.3/src/pyfirebird.egg-info/SOURCES.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-04-30 07:22:32.000000 pyfirebird-0.0.3/src/pyfirebird.egg-info/dependency_links.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      106 2023-04-30 07:22:32.000000 pyfirebird-0.0.3/src/pyfirebird.egg-info/entry_points.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       27 2023-04-30 07:22:32.000000 pyfirebird-0.0.3/src/pyfirebird.egg-info/requires.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        9 2023-04-30 07:22:32.000000 pyfirebird-0.0.3/src/pyfirebird.egg-info/top_level.txt
```

### Comparing `pyfirebird-0.0.2/setup.py` & `pyfirebird-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), "r") as f:
     README = f.read()
 
 # This call to setup() does all the work
 setup(
     name="pyfirebird",
-    version="0.0.2",
+    version="0.0.3",
     description="Streaming Data Processing Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/stonezhong/firebird",
     author="Stone Zhong",
     author_email="stonezhong@hotmail.com",
     license="MIT",
```

### Comparing `pyfirebird-0.0.2/src/firebird/base.py` & `pyfirebird-0.0.3/src/firebird/base.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.2/src/firebird/cmd_tools/executor.py` & `pyfirebird-0.0.3/src/firebird/cmd_tools/executor.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.2/src/firebird/cmd_tools/pipeline.py` & `pyfirebird-0.0.3/src/firebird/cmd_tools/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,18 +51,14 @@
         help="Configuration directory"
     )
     parser.add_argument(
         "-pmn", "--pipeline-module-name", type=str, required=False,
         help="Pipeline module name"
     )
     parser.add_argument(
-        "-pmn", "--pipeline-module-name", type=str, required=False,
-        help="Pipeline module name"
-    )
-    parser.add_argument(
         "-pid", "--pipeline-id", type=str, required=False, help="pipeline ID"
     )
     parser.add_argument(
         "-wc", "--worker-count", type=int, default=1, required=False,
         help="Worker count"
     )
     parser.add_argument(
```

### Comparing `pyfirebird-0.0.2/src/firebird/cmd_tools/pipeline_impl.py` & `pyfirebird-0.0.3/src/firebird/cmd_tools/pipeline_impl.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.2/src/firebird/rabbitmq.py` & `pyfirebird-0.0.3/src/firebird/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.2/src/firebird/zkdb.py` & `pyfirebird-0.0.3/src/firebird/zkdb.py`

 * *Files identical despite different names*

