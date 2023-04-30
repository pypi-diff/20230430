# Comparing `tmp/pyfirebird-0.0.6.tar.gz` & `tmp/pyfirebird-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfirebird-0.0.6.tar", last modified: Sun Apr 30 08:21:38 2023, max compression
+gzip compressed data, was "pyfirebird-0.0.7.tar", last modified: Sun Apr 30 08:34:02 2023, max compression
```

## Comparing `pyfirebird-0.0.6.tar` & `pyfirebird-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 08:21:38.793124 pyfirebird-0.0.6/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      367 2023-04-30 08:21:38.793124 pyfirebird-0.0.6/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        8 2023-04-30 05:34:25.000000 pyfirebird-0.0.6/README.md
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-04-30 08:21:38.793124 pyfirebird-0.0.6/setup.cfg
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1051 2023-04-30 08:21:36.000000 pyfirebird-0.0.6/setup.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 08:21:38.789124 pyfirebird-0.0.6/src/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 08:21:38.789124 pyfirebird-0.0.6/src/firebird/
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)      169 2023-04-30 06:39:02.000000 pyfirebird-0.0.6/src/firebird/__init__.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)    10042 2023-04-30 05:32:50.000000 pyfirebird-0.0.6/src/firebird/base.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 08:21:38.793124 pyfirebird-0.0.6/src/firebird/cmd_tools/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 05:45:15.000000 pyfirebird-0.0.6/src/firebird/cmd_tools/__init__.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     7298 2023-04-30 08:21:26.000000 pyfirebird-0.0.6/src/firebird/cmd_tools/executor.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2980 2023-04-30 07:22:18.000000 pyfirebird-0.0.6/src/firebird/cmd_tools/pipeline.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2946 2023-04-30 06:57:56.000000 pyfirebird-0.0.6/src/firebird/cmd_tools/pipeline_impl.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2972 2023-04-30 05:32:50.000000 pyfirebird-0.0.6/src/firebird/rabbitmq.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     5714 2023-04-30 07:37:36.000000 pyfirebird-0.0.6/src/firebird/zkdb.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 08:21:38.793124 pyfirebird-0.0.6/src/pyfirebird.egg-info/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      367 2023-04-30 08:21:38.000000 pyfirebird-0.0.6/src/pyfirebird.egg-info/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      485 2023-04-30 08:21:38.000000 pyfirebird-0.0.6/src/pyfirebird.egg-info/SOURCES.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-04-30 08:21:38.000000 pyfirebird-0.0.6/src/pyfirebird.egg-info/dependency_links.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      106 2023-04-30 08:21:38.000000 pyfirebird-0.0.6/src/pyfirebird.egg-info/entry_points.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       27 2023-04-30 08:21:38.000000 pyfirebird-0.0.6/src/pyfirebird.egg-info/requires.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        9 2023-04-30 08:21:38.000000 pyfirebird-0.0.6/src/pyfirebird.egg-info/top_level.txt
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 08:34:02.265881 pyfirebird-0.0.7/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      367 2023-04-30 08:34:02.265881 pyfirebird-0.0.7/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        8 2023-04-30 05:34:25.000000 pyfirebird-0.0.7/README.md
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-04-30 08:34:02.265881 pyfirebird-0.0.7/setup.cfg
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1051 2023-04-30 08:33:57.000000 pyfirebird-0.0.7/setup.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 08:34:02.261881 pyfirebird-0.0.7/src/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 08:34:02.261881 pyfirebird-0.0.7/src/firebird/
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)      169 2023-04-30 06:39:02.000000 pyfirebird-0.0.7/src/firebird/__init__.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)    10042 2023-04-30 05:32:50.000000 pyfirebird-0.0.7/src/firebird/base.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 08:34:02.261881 pyfirebird-0.0.7/src/firebird/cmd_tools/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 05:45:15.000000 pyfirebird-0.0.7/src/firebird/cmd_tools/__init__.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     7298 2023-04-30 08:21:26.000000 pyfirebird-0.0.7/src/firebird/cmd_tools/executor.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2980 2023-04-30 07:22:18.000000 pyfirebird-0.0.7/src/firebird/cmd_tools/pipeline.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     3090 2023-04-30 08:33:02.000000 pyfirebird-0.0.7/src/firebird/cmd_tools/pipeline_impl.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2972 2023-04-30 05:32:50.000000 pyfirebird-0.0.7/src/firebird/rabbitmq.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     5714 2023-04-30 07:37:36.000000 pyfirebird-0.0.7/src/firebird/zkdb.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 08:34:02.265881 pyfirebird-0.0.7/src/pyfirebird.egg-info/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      367 2023-04-30 08:34:02.000000 pyfirebird-0.0.7/src/pyfirebird.egg-info/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      485 2023-04-30 08:34:02.000000 pyfirebird-0.0.7/src/pyfirebird.egg-info/SOURCES.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-04-30 08:34:02.000000 pyfirebird-0.0.7/src/pyfirebird.egg-info/dependency_links.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      106 2023-04-30 08:34:02.000000 pyfirebird-0.0.7/src/pyfirebird.egg-info/entry_points.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       27 2023-04-30 08:34:02.000000 pyfirebird-0.0.7/src/pyfirebird.egg-info/requires.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        9 2023-04-30 08:34:02.000000 pyfirebird-0.0.7/src/pyfirebird.egg-info/top_level.txt
```

### Comparing `pyfirebird-0.0.6/setup.py` & `pyfirebird-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), "r") as f:
     README = f.read()
 
 # This call to setup() does all the work
 setup(
     name="pyfirebird",
-    version="0.0.6",
+    version="0.0.7",
     description="Streaming Data Processing Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/stonezhong/firebird",
     author="Stone Zhong",
     author_email="stonezhong@hotmail.com",
     license="MIT",
```

### Comparing `pyfirebird-0.0.6/src/firebird/base.py` & `pyfirebird-0.0.7/src/firebird/base.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.6/src/firebird/cmd_tools/executor.py` & `pyfirebird-0.0.7/src/firebird/cmd_tools/executor.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.6/src/firebird/cmd_tools/pipeline.py` & `pyfirebird-0.0.7/src/firebird/cmd_tools/pipeline.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.6/src/firebird/cmd_tools/pipeline_impl.py` & `pyfirebird-0.0.7/src/firebird/cmd_tools/pipeline_impl.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,27 +53,28 @@
     docker_client = docker.DockerClient(base_url=f"ssh://{docker_host_name}:22", use_ssh_client=True)
     try:
         r = docker_client.containers.run(
             "pulse-streaming", 
             name=docker_container_name, 
             hostname=docker_container_name, 
             environment={
-                "ENV_HOME": "/mnt/DATA_DISK/mordor"
+                "ENV_HOME": "/mnt/DATA_DISK/mordor",
+                "PYTHONPATH": "/mnt/DATA_DISK/mordor/apps/pulse-streaming/current",
             }, 
             volumes = {
                 "/mnt/DATA_DISK": {
                     "bind": "/mnt/DATA_DISK",
                     "mode": "rw"
                 },
             },
             network = "sfnet",
             detach = True,
             command=[
                 "python", "-u",
-                "executor.py",
+                "/usr/local/lib/python3.11/site-packages/firebird/cmd_tools/executor.py",
                 "-pid", pipeline_id,
                 "-dhn", docker_host_name,
                 "-dcn", docker_container_name
             ]
         )
     finally:
         docker_client.close()
```

### Comparing `pyfirebird-0.0.6/src/firebird/rabbitmq.py` & `pyfirebird-0.0.7/src/firebird/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.6/src/firebird/zkdb.py` & `pyfirebird-0.0.7/src/firebird/zkdb.py`

 * *Files identical despite different names*

