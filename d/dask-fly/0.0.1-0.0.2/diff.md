# Comparing `tmp/dask_fly-0.0.1.tar.gz` & `tmp/dask_fly-0.0.2.tar.gz`

## Comparing `dask_fly-0.0.1.tar` & `dask_fly-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dask_fly-0.0.1/.markdownlint.json
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 dask_fly-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dask_fly-0.0.1/src/dask_fly/__about__.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 dask_fly-0.0.1/src/dask_fly/__init__.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 dask_fly-0.0.1/src/dask_fly/client.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 dask_fly-0.0.1/src/dask_fly/scheduler.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dask_fly-0.0.1/src/dask_fly/utils.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 dask_fly-0.0.1/src/dask_fly/worker.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 dask_fly-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dask_fly-0.0.1/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 dask_fly-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 dask_fly-0.0.1/README.md
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 dask_fly-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 dask_fly-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dask_fly-0.0.2/.markdownlint.json
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 dask_fly-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dask_fly-0.0.2/src/dask_fly/__about__.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 dask_fly-0.0.2/src/dask_fly/__init__.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 dask_fly-0.0.2/src/dask_fly/client.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dask_fly-0.0.2/src/dask_fly/cluster.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 dask_fly-0.0.2/src/dask_fly/scheduler.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dask_fly-0.0.2/src/dask_fly/utils.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 dask_fly-0.0.2/src/dask_fly/worker.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 dask_fly-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dask_fly-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 dask_fly-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 dask_fly-0.0.2/README.md
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 dask_fly-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 dask_fly-0.0.2/PKG-INFO
```

### Comparing `dask_fly-0.0.1/.github/workflows/python-publish.yml` & `dask_fly-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dask_fly-0.0.1/src/dask_fly/__init__.py` & `dask_fly-0.0.2/src/dask_fly/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # SPDX-FileCopyrightText: 2023-present Miles Zimmerman <miles@zim.dev>
 #
 # SPDX-License-Identifier: MIT
 import os
+import dask_fly.client
+import dask_fly.cluster
+import dask_fly.scheduler
+import dask_fly.worker
 
 standard_env_fly_token = os.environ.get("FLY_API_TOKEN")
 standard_env_fly_hostname = os.environ.get("FLY_API_HOSTNAME")
 # Dask Cloudprovider Syntax
 cloudprovider_fly_token = os.environ.get("DASK_CLOUDPROVIDER__FLY__API_TOKEN")
 cloudprovider_fly_hostname = os.environ.get(
     "DASK_CLOUDPROVIDER__FLY__API_HOSTNAME")
```

### Comparing `dask_fly-0.0.1/src/dask_fly/scheduler.py` & `dask_fly-0.0.2/src/dask_fly/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import aiohttp
 from dask_fly import FLY_API_HOSTNAME, HEADERS
 from dask_fly.utils import random_string
 
+
 class FlyDaskScheduler:
     def __init__(self, app_name, region):
         self.app_name = app_name
         self.region = region
         self.name = f"dask-scheduler-{random_string()}"
 
     async def create(self):
```

### Comparing `dask_fly-0.0.1/src/dask_fly/worker.py` & `dask_fly-0.0.2/src/dask_fly/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import aiohttp
 from dask_fly import FLY_API_HOSTNAME, HEADERS, EXTRA_PIP_PACKAGES
 from dask_fly.utils import random_string
 
+
 class FlyDaskWorker:
     def __init__(self, app_name, region, name=None, memory=None, cpu=None):
         self.app_name = app_name
         self.region = region
         self.name = name or f"worker-{region}-{random_string()}"
         self.memory = memory
         self.cpu = cpu
```

### Comparing `dask_fly-0.0.1/LICENSE.txt` & `dask_fly-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask_fly-0.0.1/README.md` & `dask_fly-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dask_fly-0.0.1/pyproject.toml` & `dask_fly-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask_fly-0.0.1/PKG-INFO` & `dask_fly-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-fly
-Version: 0.0.1
+Version: 0.0.2
 Summary: Deploy Dask on Fly.io
 Project-URL: Documentation, https://github.com/mileszim/dask-fly#readme
 Project-URL: Issues, https://github.com/mileszim/dask-fly/issues
 Project-URL: Source, https://github.com/mileszim/dask-fly
 Author-email: Miles Zimmerman <miles@zim.dev>
 License-Expression: MIT
 License-File: LICENSE.txt
```

