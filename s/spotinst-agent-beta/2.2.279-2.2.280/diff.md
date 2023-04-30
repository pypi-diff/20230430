# Comparing `tmp/spotinst-agent-beta-2.2.279.tar.gz` & `tmp/spotinst-agent-beta-2.2.280.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-agent-beta-2.2.279.tar", last modified: Sun Apr 30 12:32:26 2023, max compression
+gzip compressed data, was "spotinst-agent-beta-2.2.280.tar", last modified: Sun Apr 30 12:49:34 2023, max compression
```

## Comparing `spotinst-agent-beta-2.2.279.tar` & `spotinst-agent-beta-2.2.280.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 12:32:26.249028 spotinst-agent-beta-2.2.279/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.279/LICENSE
--rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.279/MANIFEST.in
--rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 12:32:26.248830 spotinst-agent-beta-2.2.279/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.279/README.rst
--rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-30 12:32:26.249081 spotinst-agent-beta-2.2.279/setup.cfg
--rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-30 12:32:24.000000 spotinst-agent-beta-2.2.279/setup.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 12:32:26.241528 spotinst-agent-beta-2.2.279/spotinst_agent/
--rw-r--r--   0 ayeletc    (502) staff       (20)    13234 2023-04-30 11:50:35.000000 spotinst-agent-beta-2.2.279/spotinst_agent/__init__.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.279/spotinst_agent/agent.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.279/spotinst_agent/agentinit.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.279/spotinst_agent/basemodule.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 12:32:26.231019 spotinst-agent-beta-2.2.279/spotinst_agent/data/
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 12:32:26.244291 spotinst-agent-beta-2.2.279/spotinst_agent/data/configuration/
--rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.279/spotinst_agent/data/configuration/basemodule.yml
--rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.279/spotinst_agent/data/configuration/spotinst-agent.yml
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 12:32:26.244624 spotinst-agent-beta-2.2.279/spotinst_agent/data/installation/
--rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.279/spotinst_agent/data/installation/agent-init.sh
--rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.279/spotinst_agent/scheduler.py
--rw-r--r--   0 ayeletc    (502) staff       (20)    10922 2023-04-30 12:32:07.000000 spotinst-agent-beta-2.2.279/spotinst_agent/taskmanager.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.279/spotinst_agent/utils.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 12:32:26.248555 spotinst-agent-beta-2.2.279/spotinst_agent_beta.egg-info/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 12:32:26.000000 spotinst-agent-beta-2.2.279/spotinst_agent_beta.egg-info/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-30 12:32:26.000000 spotinst-agent-beta-2.2.279/spotinst_agent_beta.egg-info/SOURCES.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-30 12:32:26.000000 spotinst-agent-beta-2.2.279/spotinst_agent_beta.egg-info/dependency_links.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       55 2023-04-30 12:32:26.000000 spotinst-agent-beta-2.2.279/spotinst_agent_beta.egg-info/entry_points.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-30 12:32:26.000000 spotinst-agent-beta-2.2.279/spotinst_agent_beta.egg-info/requires.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-30 12:32:26.000000 spotinst-agent-beta-2.2.279/spotinst_agent_beta.egg-info/top_level.txt
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 12:49:34.962934 spotinst-agent-beta-2.2.280/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.280/LICENSE
+-rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.280/MANIFEST.in
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 12:49:34.962757 spotinst-agent-beta-2.2.280/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.280/README.rst
+-rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-30 12:49:34.962982 spotinst-agent-beta-2.2.280/setup.cfg
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-30 12:49:32.000000 spotinst-agent-beta-2.2.280/setup.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 12:49:34.960402 spotinst-agent-beta-2.2.280/spotinst_agent/
+-rw-r--r--   0 ayeletc    (502) staff       (20)    13234 2023-04-30 12:48:55.000000 spotinst-agent-beta-2.2.280/spotinst_agent/__init__.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.280/spotinst_agent/agent.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.280/spotinst_agent/agentinit.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.280/spotinst_agent/basemodule.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 12:49:34.957165 spotinst-agent-beta-2.2.280/spotinst_agent/data/
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 12:49:34.960903 spotinst-agent-beta-2.2.280/spotinst_agent/data/configuration/
+-rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.280/spotinst_agent/data/configuration/basemodule.yml
+-rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.280/spotinst_agent/data/configuration/spotinst-agent.yml
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 12:49:34.961154 spotinst-agent-beta-2.2.280/spotinst_agent/data/installation/
+-rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.280/spotinst_agent/data/installation/agent-init.sh
+-rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.280/spotinst_agent/scheduler.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)    10922 2023-04-30 12:49:32.000000 spotinst-agent-beta-2.2.280/spotinst_agent/taskmanager.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.280/spotinst_agent/utils.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 12:49:34.962486 spotinst-agent-beta-2.2.280/spotinst_agent_beta.egg-info/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 12:49:34.000000 spotinst-agent-beta-2.2.280/spotinst_agent_beta.egg-info/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-30 12:49:34.000000 spotinst-agent-beta-2.2.280/spotinst_agent_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-30 12:49:34.000000 spotinst-agent-beta-2.2.280/spotinst_agent_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       55 2023-04-30 12:49:34.000000 spotinst-agent-beta-2.2.280/spotinst_agent_beta.egg-info/entry_points.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-30 12:49:34.000000 spotinst-agent-beta-2.2.280/spotinst_agent_beta.egg-info/requires.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-30 12:49:34.000000 spotinst-agent-beta-2.2.280/spotinst_agent_beta.egg-info/top_level.txt
```

### Comparing `spotinst-agent-beta-2.2.279/LICENSE` & `spotinst-agent-beta-2.2.280/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.279/PKG-INFO` & `spotinst-agent-beta-2.2.280/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.279
+Version: 2.2.280
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spotinst-agent-beta-2.2.279/README.rst` & `spotinst-agent-beta-2.2.280/README.rst`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.279/setup.py` & `spotinst-agent-beta-2.2.280/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='spotinst-agent-beta',
 
-    version="2.2.279",
+    version="2.2.280",
 
     description='Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.',
 
     long_description=description,
 
     # The project's main homepage.
     url='https://github.com/spotinst/spotinst-spectrum-agent',
```

### Comparing `spotinst-agent-beta-2.2.279/spotinst_agent/__init__.py` & `spotinst-agent-beta-2.2.280/spotinst_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.279/spotinst_agent/agent.py` & `spotinst-agent-beta-2.2.280/spotinst_agent/agent.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.279/spotinst_agent/agentinit.py` & `spotinst-agent-beta-2.2.280/spotinst_agent/agentinit.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.279/spotinst_agent/basemodule.py` & `spotinst-agent-beta-2.2.280/spotinst_agent/basemodule.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.279/spotinst_agent/data/configuration/spotinst-agent.yml` & `spotinst-agent-beta-2.2.280/spotinst_agent/data/configuration/spotinst-agent.yml`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.279/spotinst_agent/data/installation/agent-init.sh` & `spotinst-agent-beta-2.2.280/spotinst_agent/data/installation/agent-init.sh`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.279/spotinst_agent/scheduler.py` & `spotinst-agent-beta-2.2.280/spotinst_agent/scheduler.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.279/spotinst_agent/taskmanager.py` & `spotinst-agent-beta-2.2.280/spotinst_agent/taskmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.reload_interval = reload_interval
         self.scheduler = ThreadedScheduler()
         self.running = True
         self.tasks = {}
         self.instance_details = instance_details
 
     def start(self):
-        time.sleep(20)
+        time.sleep(30)
         initiators_folder = '/etc/spotinst/agent/initiators/modules'
         self.log.debug("service is %s" % self.enable)
 
         # Search for initiators in folder
         initiators = self.load_modules(initiators_folder)
 
         # Setup Modules
```

### Comparing `spotinst-agent-beta-2.2.279/spotinst_agent/utils.py` & `spotinst-agent-beta-2.2.280/spotinst_agent/utils.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.279/spotinst_agent_beta.egg-info/PKG-INFO` & `spotinst-agent-beta-2.2.280/spotinst_agent_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.279
+Version: 2.2.280
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spotinst-agent-beta-2.2.279/spotinst_agent_beta.egg-info/SOURCES.txt` & `spotinst-agent-beta-2.2.280/spotinst_agent_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

