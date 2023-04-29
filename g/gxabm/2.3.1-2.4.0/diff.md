# Comparing `tmp/gxabm-2.3.1.tar.gz` & `tmp/gxabm-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gxabm-2.3.1.tar", last modified: Fri Apr 28 19:36:39 2023, max compression
+gzip compressed data, was "gxabm-2.4.0.tar", last modified: Sat Apr 29 23:25:16 2023, max compression
```

## Comparing `gxabm-2.3.1.tar` & `gxabm-2.4.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-28 19:36:39.724062 gxabm-2.3.1/
--rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.3.1/MANIFEST.in
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-04-28 19:36:39.723883 gxabm-2.3.1/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.3.1/README.md
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-28 19:36:39.715787 gxabm-2.3.1/abm/
--rw-r--r--   0 suderman   (502) staff       (20)        6 2023-04-28 19:36:16.000000 gxabm-2.3.1/abm/VERSION
--rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.3.1/abm/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)     8362 2023-04-24 20:24:38.000000 gxabm-2.3.1/abm/__main__.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-28 19:36:39.720768 gxabm-2.3.1/abm/lib/
--rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.3.1/abm/lib/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)    18434 2023-04-27 20:18:52.000000 gxabm-2.3.1/abm/lib/benchmark.py
--rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.3.1/abm/lib/cloudlaunch.py
--rw-r--r--   0 suderman   (502) staff       (20)     5458 2023-04-27 20:18:52.000000 gxabm-2.3.1/abm/lib/common.py
--rw-r--r--   0 suderman   (502) staff       (20)     5433 2022-10-19 17:36:24.000000 gxabm-2.3.1/abm/lib/config.py
--rw-r--r--   0 suderman   (502) staff       (20)     6483 2023-04-27 20:18:52.000000 gxabm-2.3.1/abm/lib/dataset.py
--rw-r--r--   0 suderman   (502) staff       (20)     7661 2023-04-28 19:35:54.000000 gxabm-2.3.1/abm/lib/experiment.py
--rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.3.1/abm/lib/folder.py
--rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.3.1/abm/lib/helm.py
--rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.3.1/abm/lib/histories.yml
--rw-r--r--   0 suderman   (502) staff       (20)     9582 2023-04-27 20:14:45.000000 gxabm-2.3.1/abm/lib/history.py
--rw-r--r--   0 suderman   (502) staff       (20)     3382 2023-04-27 20:18:52.000000 gxabm-2.3.1/abm/lib/job.py
--rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.3.1/abm/lib/kubectl.py
--rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.3.1/abm/lib/library.py
--rw-r--r--   0 suderman   (502) staff       (20)    11186 2023-04-27 20:18:52.000000 gxabm-2.3.1/abm/lib/menu.yml
--rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.3.1/abm/lib/users.py
--rw-r--r--   0 suderman   (502) staff       (20)     6930 2023-04-27 20:18:52.000000 gxabm-2.3.1/abm/lib/workflow.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-28 19:36:39.721573 gxabm-2.3.1/gxabm.egg-info/
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-04-28 19:36:39.000000 gxabm-2.3.1/gxabm.egg-info/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)      669 2023-04-28 19:36:39.000000 gxabm-2.3.1/gxabm.egg-info/SOURCES.txt
--rw-r--r--   0 suderman   (502) staff       (20)        1 2023-04-28 19:36:39.000000 gxabm-2.3.1/gxabm.egg-info/dependency_links.txt
--rw-r--r--   0 suderman   (502) staff       (20)       49 2023-04-28 19:36:39.000000 gxabm-2.3.1/gxabm.egg-info/entry_points.txt
--rw-r--r--   0 suderman   (502) staff       (20)       48 2023-04-28 19:36:39.000000 gxabm-2.3.1/gxabm.egg-info/requires.txt
--rw-r--r--   0 suderman   (502) staff       (20)        9 2023-04-28 19:36:39.000000 gxabm-2.3.1/gxabm.egg-info/top_level.txt
--rw-r--r--   0 suderman   (502) staff       (20)       38 2023-04-28 19:36:39.724110 gxabm-2.3.1/setup.cfg
--rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.3.1/setup.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-28 19:36:39.723139 gxabm-2.3.1/test/
--rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.3.1/test/__init__.py
--rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.3.1/test/check_tools.py
--rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.3.1/test/metrics.py
--rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.3.1/test/test_environments.py
--rw-r--r--   0 suderman   (502) staff       (20)      272 2023-03-14 21:04:32.000000 gxabm-2.3.1/test/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-29 23:25:16.546042 gxabm-2.4.0/
+-rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.4.0/MANIFEST.in
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-04-29 23:25:16.545859 gxabm-2.4.0/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.4.0/README.md
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-29 23:25:16.537356 gxabm-2.4.0/abm/
+-rw-r--r--   0 suderman   (502) staff       (20)        6 2023-04-29 23:24:17.000000 gxabm-2.4.0/abm/VERSION
+-rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.4.0/abm/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)     8362 2023-04-24 20:24:38.000000 gxabm-2.4.0/abm/__main__.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-29 23:25:16.542893 gxabm-2.4.0/abm/lib/
+-rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.4.0/abm/lib/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)    18434 2023-04-27 20:18:52.000000 gxabm-2.4.0/abm/lib/benchmark.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.4.0/abm/lib/cloudlaunch.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7556 2023-04-29 23:23:52.000000 gxabm-2.4.0/abm/lib/common.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5433 2022-10-19 17:36:24.000000 gxabm-2.4.0/abm/lib/config.py
+-rw-r--r--   0 suderman   (502) staff       (20)     6483 2023-04-27 20:18:52.000000 gxabm-2.4.0/abm/lib/dataset.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7661 2023-04-29 03:35:40.000000 gxabm-2.4.0/abm/lib/experiment.py
+-rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.4.0/abm/lib/folder.py
+-rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.4.0/abm/lib/helm.py
+-rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.4.0/abm/lib/histories.yml
+-rw-r--r--   0 suderman   (502) staff       (20)    10348 2023-04-29 23:23:52.000000 gxabm-2.4.0/abm/lib/history.py
+-rw-r--r--   0 suderman   (502) staff       (20)     3610 2023-04-29 23:23:52.000000 gxabm-2.4.0/abm/lib/job.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.4.0/abm/lib/kubectl.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.4.0/abm/lib/library.py
+-rw-r--r--   0 suderman   (502) staff       (20)    11618 2023-04-29 23:23:52.000000 gxabm-2.4.0/abm/lib/menu.yml
+-rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.4.0/abm/lib/users.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7524 2023-04-29 23:23:52.000000 gxabm-2.4.0/abm/lib/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-29 23:25:16.543797 gxabm-2.4.0/gxabm.egg-info/
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-04-29 23:25:16.000000 gxabm-2.4.0/gxabm.egg-info/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)      669 2023-04-29 23:25:16.000000 gxabm-2.4.0/gxabm.egg-info/SOURCES.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        1 2023-04-29 23:25:16.000000 gxabm-2.4.0/gxabm.egg-info/dependency_links.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       49 2023-04-29 23:25:16.000000 gxabm-2.4.0/gxabm.egg-info/entry_points.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       48 2023-04-29 23:25:16.000000 gxabm-2.4.0/gxabm.egg-info/requires.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        9 2023-04-29 23:25:16.000000 gxabm-2.4.0/gxabm.egg-info/top_level.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       38 2023-04-29 23:25:16.546102 gxabm-2.4.0/setup.cfg
+-rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.4.0/setup.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-29 23:25:16.545476 gxabm-2.4.0/test/
+-rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.4.0/test/__init__.py
+-rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.4.0/test/check_tools.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.4.0/test/metrics.py
+-rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.4.0/test/test_environments.py
+-rw-r--r--   0 suderman   (502) staff       (20)      272 2023-03-14 21:04:32.000000 gxabm-2.4.0/test/workflow.py
```

### Comparing `gxabm-2.3.1/PKG-INFO` & `gxabm-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.3.1
+Version: 2.4.0
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.3.1/README.md` & `gxabm-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.1/abm/__main__.py` & `gxabm-2.4.0/abm/__main__.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.1/abm/lib/benchmark.py` & `gxabm-2.4.0/abm/lib/benchmark.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.1/abm/lib/cloudlaunch.py` & `gxabm-2.4.0/abm/lib/cloudlaunch.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.1/abm/lib/config.py` & `gxabm-2.4.0/abm/lib/config.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.1/abm/lib/dataset.py` & `gxabm-2.4.0/abm/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.1/abm/lib/experiment.py` & `gxabm-2.4.0/abm/lib/experiment.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.1/abm/lib/folder.py` & `gxabm-2.4.0/abm/lib/folder.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.1/abm/lib/helm.py` & `gxabm-2.4.0/abm/lib/helm.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.1/abm/lib/history.py` & `gxabm-2.4.0/abm/lib/history.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 import sys
 import yaml
 
-from lib.common import connect, parse_profile, Context
+from lib.common import connect, parse_profile, Context, summarize_metrics
 from pprint import pprint
 from pathlib import Path
 
 #
 # History related functions
 #
 
@@ -301,8 +301,28 @@
 
     gi = connect(context)
     hid = args.pop(0)
     if not replace:
         history = gi.histories.show_history(hid, contents=False)
         args += history['tags']
     gi.histories.update_history(hid, tags=args)
-    print(f"Set history tags to: {', '.join(args)}")
+    print(f"Set history tags to: {', '.join(args)}")
+
+def summarize(context: Context, args: list):
+    if len(args) == 0:
+        print("ERROR: Provide one or more history ID values.")
+        return
+    gi = connect(context)
+    hid = args[0]
+    all_jobs = []
+    invocations = gi.invocations.get_invocations(history_id=hid)
+    for invocation in invocations:
+        id = invocation['id']
+        jobs = gi.jobs.get_jobs(history_id=hid, invocation_id=id)
+        for job in jobs:
+            job['invocation_id'] = id
+            job['history_id'] = hid
+            if 'workflow_id' in invocation:
+                job['workflow_id'] = invocation['workflow_id']
+            all_jobs.append(job)
+    # summarize_metrics(gi, gi.jobs.get_jobs(history_id=args[0]))
+    summarize_metrics(gi, all_jobs)
```

### Comparing `gxabm-2.3.1/abm/lib/job.py` & `gxabm-2.4.0/abm/lib/job.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from .common import connect, Context
+from .common import connect, Context, print_json
 from pprint import pprint
 import logging
 
 log = logging.getLogger('abm')
 
 
 def list(context: Context, args: list):
@@ -100,8 +100,17 @@
 
 
 def problems(context: Context, args: list):
     if len(args) == 0:
         print('ERROR: no job ID provided.')
         return
     gi = connect(context)
-    pprint(gi.jobs.get_common_problems(args[0]))
+    print_json(gi.jobs.get_common_problems(args[0]))
+
+
+def rerun(context: Context, args: list):
+    if len(args) == 0:
+        print("ERROR: no job ID provided")
+        return
+    gi = connect(context)
+    result = gi.jobs.rerun_job(args[0])
+    print_json(result)
```

### Comparing `gxabm-2.3.1/abm/lib/kubectl.py` & `gxabm-2.4.0/abm/lib/kubectl.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.1/abm/lib/library.py` & `gxabm-2.4.0/abm/lib/library.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.1/abm/lib/menu.yml` & `gxabm-2.4.0/abm/lib/menu.yml`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,18 @@
       handler: workflow.invocation
       params: "--workflow WORKFLOW_ID --invocation INVOCATION_ID"
       help: show details about a specific workflow invocation
     - name: ['inputs']
       help: list inputs required by a workflow
       params: WORKFLOW_ID
       handler: workflow.inputs
+    - name: [summary, summarize]
+      handler: workflow.summarize
+      help: generate a CSV with job metrics for all workflow runs
+      params: ID [ID ...]
     - name: ['test']
       handler: workflow.test
       help: run some test code
 - name:
     - dataset
     - ds
   help: manage datasets
@@ -144,14 +148,18 @@
       handler: history.tag
       help: add or replace history tags
       params: ID [-r|--repace] tag1 [tag2...]
     - name: [show]
       handler: history.show
       params: "ID [-c|--contents]"
       help: show detailed information about a history
+    - name: [summarize, summary, table]
+      handler: history.summarize
+      params: "ID [ID...]"
+      help: Generate a CSV table with runtime metrics for all jobs in the history.
     - name: [publish, pub]
       handler: history.publish
       help: publish the given history
       params: ID
     - name: [rename, ren]
       handler: history.rename
       help: rename a history
@@ -172,15 +180,15 @@
       handler: history.purge
 - name: [ jobs, job ]
   help: manage jobs on the server
   menu:
     - name: [ list, ls ]
       help: list all jobs, or jobs in a particular state. Can filter by a history.
       handler: job.list
-      params: "[-s|--state ok|running|error|waiting] [-h|--history_id historyID]"
+      params: "[-s|--state ok|running|error|waiting] [-h|--history historyID]"
     - name: [ show ]
       help: show detailed information about a job
       handler: job.show
       params: ID
     - name: [problems, problem, prob]
       help: list common problems that may have caused a job to fail
       handler: job.problems
@@ -189,14 +197,18 @@
       help: kills a job
       handler: job.cancel
       params: ID
     - name: [ metrics, stats ]
       help: display runtime metrics for the job, or a list of jobs contained in a history
       handler: job.metrics
       params: "[ID | -h|--history historyID]"
+    - name: [ rerun ]
+      handler: job.rerun
+      params: JOB_ID
+      help: re-run a job
 - name: [users, user]
   help: manage users on the Galaxy instance
   menu:
     - name: [list, ls]
       help: list all users on the Galaxy instance
       handler: users.list
     - name: [api_key, apikey, key]
```

### Comparing `gxabm-2.3.1/abm/lib/users.py` & `gxabm-2.4.0/abm/lib/users.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.1/abm/lib/workflow.py` & `gxabm-2.4.0/abm/lib/workflow.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pprint import pprint
 
 import requests
 import yaml
 import planemo
 from planemo.runnable import for_path, for_uri
 from planemo.galaxy.workflows import install_shed_repos
-from common import connect, Context
+from common import connect, Context, summarize_metrics
 from pathlib import Path
 
 log = logging.getLogger('abm')
 
 def list(context: Context, args: list):
     gi = connect(context)
     workflows = gi.workflows.get_workflows(published=True)
@@ -219,8 +219,23 @@
     if len(args) != 2:
         print("USAGE: rename ID 'new workflow name'")
         return
     gi = connect(context)
     result = gi.workflows.update_workflow(args[0], name=args[1])
     print(f"Renamed workflow to {result['name']}")
 
-
+def summarize(context: Context, args: list):
+    if len(args) == 0:
+        print("ERROR: Provide one or more workflow ID values.")
+        return
+    gi = connect(context)
+    wid = args[0]
+    all_jobs = []
+    invocations = gi.invocations.get_invocations(workflow_id=wid)
+    for invocation in invocations:
+        id = invocation['id']
+        jobs = gi.jobs.get_jobs(invocation_id=id, workflow_id=wid)
+        for job in jobs:
+            job['invocation_id'] = id
+            job['workflow_id'] = wid
+            all_jobs.append(job)
+    summarize_metrics(gi, all_jobs)
```

### Comparing `gxabm-2.3.1/gxabm.egg-info/PKG-INFO` & `gxabm-2.4.0/gxabm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.3.1
+Version: 2.4.0
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.3.1/gxabm.egg-info/SOURCES.txt` & `gxabm-2.4.0/gxabm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.1/setup.py` & `gxabm-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.1/test/check_tools.py` & `gxabm-2.4.0/test/check_tools.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.1/test/metrics.py` & `gxabm-2.4.0/test/metrics.py`

 * *Files identical despite different names*

