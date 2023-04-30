# Comparing `tmp/spotinst-agent-beta-2.2.272.tar.gz` & `tmp/spotinst-agent-beta-2.2.273.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-agent-beta-2.2.272.tar", last modified: Sun Apr 30 07:32:36 2023, max compression
+gzip compressed data, was "spotinst-agent-beta-2.2.273.tar", last modified: Sun Apr 30 07:37:12 2023, max compression
```

## Comparing `spotinst-agent-beta-2.2.272.tar` & `spotinst-agent-beta-2.2.273.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:32:36.926605 spotinst-agent-beta-2.2.272/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.272/LICENSE
--rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.272/MANIFEST.in
--rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 07:32:36.925472 spotinst-agent-beta-2.2.272/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.272/README.rst
--rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-30 07:32:36.926683 spotinst-agent-beta-2.2.272/setup.cfg
--rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-30 07:32:32.000000 spotinst-agent-beta-2.2.272/setup.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:32:36.914621 spotinst-agent-beta-2.2.272/spotinst_agent/
--rw-r--r--   0 ayeletc    (502) staff       (20)    13080 2023-04-27 12:18:46.000000 spotinst-agent-beta-2.2.272/spotinst_agent/__init__.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.272/spotinst_agent/agent.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.272/spotinst_agent/agentinit.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.272/spotinst_agent/basemodule.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:32:36.904018 spotinst-agent-beta-2.2.272/spotinst_agent/data/
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:32:36.918036 spotinst-agent-beta-2.2.272/spotinst_agent/data/configuration/
--rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.272/spotinst_agent/data/configuration/basemodule.yml
--rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.272/spotinst_agent/data/configuration/spotinst-agent.yml
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:32:36.919097 spotinst-agent-beta-2.2.272/spotinst_agent/data/installation/
--rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.272/spotinst_agent/data/installation/agent-init.sh
--rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.272/spotinst_agent/scheduler.py
--rw-r--r--   0 ayeletc    (502) staff       (20)    11269 2023-04-29 20:22:20.000000 spotinst-agent-beta-2.2.272/spotinst_agent/taskmanager.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.272/spotinst_agent/utils.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:32:36.924689 spotinst-agent-beta-2.2.272/spotinst_agent_beta.egg-info/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 07:32:36.000000 spotinst-agent-beta-2.2.272/spotinst_agent_beta.egg-info/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-30 07:32:36.000000 spotinst-agent-beta-2.2.272/spotinst_agent_beta.egg-info/SOURCES.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-30 07:32:36.000000 spotinst-agent-beta-2.2.272/spotinst_agent_beta.egg-info/dependency_links.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       55 2023-04-30 07:32:36.000000 spotinst-agent-beta-2.2.272/spotinst_agent_beta.egg-info/entry_points.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-30 07:32:36.000000 spotinst-agent-beta-2.2.272/spotinst_agent_beta.egg-info/requires.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-30 07:32:36.000000 spotinst-agent-beta-2.2.272/spotinst_agent_beta.egg-info/top_level.txt
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:37:12.668150 spotinst-agent-beta-2.2.273/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.273/LICENSE
+-rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.273/MANIFEST.in
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 07:37:12.667982 spotinst-agent-beta-2.2.273/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.273/README.rst
+-rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-30 07:37:12.668201 spotinst-agent-beta-2.2.273/setup.cfg
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-30 07:37:10.000000 spotinst-agent-beta-2.2.273/setup.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:37:12.665593 spotinst-agent-beta-2.2.273/spotinst_agent/
+-rw-r--r--   0 ayeletc    (502) staff       (20)    13080 2023-04-27 12:18:46.000000 spotinst-agent-beta-2.2.273/spotinst_agent/__init__.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.273/spotinst_agent/agent.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.273/spotinst_agent/agentinit.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.273/spotinst_agent/basemodule.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:37:12.656206 spotinst-agent-beta-2.2.273/spotinst_agent/data/
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:37:12.666090 spotinst-agent-beta-2.2.273/spotinst_agent/data/configuration/
+-rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.273/spotinst_agent/data/configuration/basemodule.yml
+-rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.273/spotinst_agent/data/configuration/spotinst-agent.yml
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:37:12.666327 spotinst-agent-beta-2.2.273/spotinst_agent/data/installation/
+-rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.273/spotinst_agent/data/installation/agent-init.sh
+-rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.273/spotinst_agent/scheduler.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)    11244 2023-04-30 07:35:53.000000 spotinst-agent-beta-2.2.273/spotinst_agent/taskmanager.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.273/spotinst_agent/utils.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:37:12.667709 spotinst-agent-beta-2.2.273/spotinst_agent_beta.egg-info/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 07:37:12.000000 spotinst-agent-beta-2.2.273/spotinst_agent_beta.egg-info/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-30 07:37:12.000000 spotinst-agent-beta-2.2.273/spotinst_agent_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-30 07:37:12.000000 spotinst-agent-beta-2.2.273/spotinst_agent_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       55 2023-04-30 07:37:12.000000 spotinst-agent-beta-2.2.273/spotinst_agent_beta.egg-info/entry_points.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-30 07:37:12.000000 spotinst-agent-beta-2.2.273/spotinst_agent_beta.egg-info/requires.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-30 07:37:12.000000 spotinst-agent-beta-2.2.273/spotinst_agent_beta.egg-info/top_level.txt
```

### Comparing `spotinst-agent-beta-2.2.272/LICENSE` & `spotinst-agent-beta-2.2.273/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.272/PKG-INFO` & `spotinst-agent-beta-2.2.273/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.272
+Version: 2.2.273
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spotinst-agent-beta-2.2.272/README.rst` & `spotinst-agent-beta-2.2.273/README.rst`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.272/setup.py` & `spotinst-agent-beta-2.2.273/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='spotinst-agent-beta',
 
-    version="2.2.272",
+    version="2.2.273",
 
     description='Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.',
 
     long_description=description,
 
     # The project's main homepage.
     url='https://github.com/spotinst/spotinst-spectrum-agent',
```

### Comparing `spotinst-agent-beta-2.2.272/spotinst_agent/__init__.py` & `spotinst-agent-beta-2.2.273/spotinst_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.272/spotinst_agent/agent.py` & `spotinst-agent-beta-2.2.273/spotinst_agent/agent.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.272/spotinst_agent/agentinit.py` & `spotinst-agent-beta-2.2.273/spotinst_agent/agentinit.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.272/spotinst_agent/basemodule.py` & `spotinst-agent-beta-2.2.273/spotinst_agent/basemodule.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.272/spotinst_agent/data/configuration/spotinst-agent.yml` & `spotinst-agent-beta-2.2.273/spotinst_agent/data/configuration/spotinst-agent.yml`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.272/spotinst_agent/data/installation/agent-init.sh` & `spotinst-agent-beta-2.2.273/spotinst_agent/data/installation/agent-init.sh`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.272/spotinst_agent/scheduler.py` & `spotinst-agent-beta-2.2.273/spotinst_agent/scheduler.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.272/spotinst_agent/taskmanager.py` & `spotinst-agent-beta-2.2.273/spotinst_agent/taskmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
                     self.log.error("Failed to import module: %s. %s" % (modname, traceback.format_exc()))
                     continue
 
                 # Find all classes defined in the module
                 self.log.info("Finding classes defined in module " + str(modname))
 
                 try :
-                    self.log.info("Modname is" + mod + "string is " + str(mod) + "and his size is " + len(dir(mod)))
+                    self.log.info("Modname is" + mod +  "and his size is " + len(dir(mod)))
                 except Exception as e:
                     # Log error
                     self.log.error("Failed to log: %s. %s" % (modname, traceback.format_exc()))
                     continue
                 for attrname in dir(mod):
                     attr = getattr(mod, attrname)
                     # Only attempt to load classes that are infact classes but not the base Module class
```

### Comparing `spotinst-agent-beta-2.2.272/spotinst_agent/utils.py` & `spotinst-agent-beta-2.2.273/spotinst_agent/utils.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.272/spotinst_agent_beta.egg-info/PKG-INFO` & `spotinst-agent-beta-2.2.273/spotinst_agent_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.272
+Version: 2.2.273
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spotinst-agent-beta-2.2.272/spotinst_agent_beta.egg-info/SOURCES.txt` & `spotinst-agent-beta-2.2.273/spotinst_agent_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

