# Comparing `tmp/spotinst-agent-beta-2.2.276.tar.gz` & `tmp/spotinst-agent-beta-2.2.277.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-agent-beta-2.2.276.tar", last modified: Sun Apr 30 10:58:50 2023, max compression
+gzip compressed data, was "spotinst-agent-beta-2.2.277.tar", last modified: Sun Apr 30 11:23:52 2023, max compression
```

## Comparing `spotinst-agent-beta-2.2.276.tar` & `spotinst-agent-beta-2.2.277.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 10:58:50.882691 spotinst-agent-beta-2.2.276/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.276/LICENSE
--rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.276/MANIFEST.in
--rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 10:58:50.882486 spotinst-agent-beta-2.2.276/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.276/README.rst
--rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-30 10:58:50.882738 spotinst-agent-beta-2.2.276/setup.cfg
--rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-30 10:58:49.000000 spotinst-agent-beta-2.2.276/setup.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 10:58:50.878900 spotinst-agent-beta-2.2.276/spotinst_agent/
--rw-r--r--   0 ayeletc    (502) staff       (20)    13173 2023-04-30 10:58:32.000000 spotinst-agent-beta-2.2.276/spotinst_agent/__init__.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.276/spotinst_agent/agent.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.276/spotinst_agent/agentinit.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.276/spotinst_agent/basemodule.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 10:58:50.861323 spotinst-agent-beta-2.2.276/spotinst_agent/data/
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 10:58:50.879464 spotinst-agent-beta-2.2.276/spotinst_agent/data/configuration/
--rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.276/spotinst_agent/data/configuration/basemodule.yml
--rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.276/spotinst_agent/data/configuration/spotinst-agent.yml
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 10:58:50.879803 spotinst-agent-beta-2.2.276/spotinst_agent/data/installation/
--rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.276/spotinst_agent/data/installation/agent-init.sh
--rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.276/spotinst_agent/scheduler.py
--rw-r--r--   0 ayeletc    (502) staff       (20)    11040 2023-04-30 10:01:09.000000 spotinst-agent-beta-2.2.276/spotinst_agent/taskmanager.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.276/spotinst_agent/utils.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 10:58:50.882166 spotinst-agent-beta-2.2.276/spotinst_agent_beta.egg-info/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 10:58:50.000000 spotinst-agent-beta-2.2.276/spotinst_agent_beta.egg-info/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-30 10:58:50.000000 spotinst-agent-beta-2.2.276/spotinst_agent_beta.egg-info/SOURCES.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-30 10:58:50.000000 spotinst-agent-beta-2.2.276/spotinst_agent_beta.egg-info/dependency_links.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       55 2023-04-30 10:58:50.000000 spotinst-agent-beta-2.2.276/spotinst_agent_beta.egg-info/entry_points.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-30 10:58:50.000000 spotinst-agent-beta-2.2.276/spotinst_agent_beta.egg-info/requires.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-30 10:58:50.000000 spotinst-agent-beta-2.2.276/spotinst_agent_beta.egg-info/top_level.txt
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 11:23:52.410245 spotinst-agent-beta-2.2.277/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.277/LICENSE
+-rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.277/MANIFEST.in
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 11:23:52.410060 spotinst-agent-beta-2.2.277/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.277/README.rst
+-rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-30 11:23:52.410298 spotinst-agent-beta-2.2.277/setup.cfg
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-30 11:23:50.000000 spotinst-agent-beta-2.2.277/setup.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 11:23:52.407503 spotinst-agent-beta-2.2.277/spotinst_agent/
+-rw-r--r--   0 ayeletc    (502) staff       (20)    13173 2023-04-30 10:58:32.000000 spotinst-agent-beta-2.2.277/spotinst_agent/__init__.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.277/spotinst_agent/agent.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.277/spotinst_agent/agentinit.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.277/spotinst_agent/basemodule.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 11:23:52.398925 spotinst-agent-beta-2.2.277/spotinst_agent/data/
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 11:23:52.408078 spotinst-agent-beta-2.2.277/spotinst_agent/data/configuration/
+-rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.277/spotinst_agent/data/configuration/basemodule.yml
+-rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.277/spotinst_agent/data/configuration/spotinst-agent.yml
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 11:23:52.408493 spotinst-agent-beta-2.2.277/spotinst_agent/data/installation/
+-rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.277/spotinst_agent/data/installation/agent-init.sh
+-rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.277/spotinst_agent/scheduler.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)    10899 2023-04-30 11:23:50.000000 spotinst-agent-beta-2.2.277/spotinst_agent/taskmanager.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.277/spotinst_agent/utils.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 11:23:52.409798 spotinst-agent-beta-2.2.277/spotinst_agent_beta.egg-info/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 11:23:52.000000 spotinst-agent-beta-2.2.277/spotinst_agent_beta.egg-info/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-30 11:23:52.000000 spotinst-agent-beta-2.2.277/spotinst_agent_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-30 11:23:52.000000 spotinst-agent-beta-2.2.277/spotinst_agent_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       55 2023-04-30 11:23:52.000000 spotinst-agent-beta-2.2.277/spotinst_agent_beta.egg-info/entry_points.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-30 11:23:52.000000 spotinst-agent-beta-2.2.277/spotinst_agent_beta.egg-info/requires.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-30 11:23:52.000000 spotinst-agent-beta-2.2.277/spotinst_agent_beta.egg-info/top_level.txt
```

### Comparing `spotinst-agent-beta-2.2.276/LICENSE` & `spotinst-agent-beta-2.2.277/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.276/PKG-INFO` & `spotinst-agent-beta-2.2.277/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.276
+Version: 2.2.277
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spotinst-agent-beta-2.2.276/README.rst` & `spotinst-agent-beta-2.2.277/README.rst`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.276/setup.py` & `spotinst-agent-beta-2.2.277/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='spotinst-agent-beta',
 
-    version="2.2.276",
+    version="2.2.277",
 
     description='Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.',
 
     long_description=description,
 
     # The project's main homepage.
     url='https://github.com/spotinst/spotinst-spectrum-agent',
```

### Comparing `spotinst-agent-beta-2.2.276/spotinst_agent/__init__.py` & `spotinst-agent-beta-2.2.277/spotinst_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.276/spotinst_agent/agent.py` & `spotinst-agent-beta-2.2.277/spotinst_agent/agent.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.276/spotinst_agent/agentinit.py` & `spotinst-agent-beta-2.2.277/spotinst_agent/agentinit.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.276/spotinst_agent/basemodule.py` & `spotinst-agent-beta-2.2.277/spotinst_agent/basemodule.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.276/spotinst_agent/data/configuration/spotinst-agent.yml` & `spotinst-agent-beta-2.2.277/spotinst_agent/data/configuration/spotinst-agent.yml`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.276/spotinst_agent/data/installation/agent-init.sh` & `spotinst-agent-beta-2.2.277/spotinst_agent/data/installation/agent-init.sh`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.276/spotinst_agent/scheduler.py` & `spotinst-agent-beta-2.2.277/spotinst_agent/scheduler.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.276/spotinst_agent/taskmanager.py` & `spotinst-agent-beta-2.2.277/spotinst_agent/taskmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,17 +160,14 @@
                 self.log.info("Finding classes defined in module " + str(modname))
                 for attrname in dir(mod):
                     attr = getattr(mod, attrname)
                     # Only attempt to load classes that are infact classes but not the base Module class
                     self.log.debug("Checking " + str(modname) + " Attribute " + str(attrname))
                     self.log.info("Checking " + str(modname) + " Attribute " + str(attrname))
 
-                    self.log.info("is class: %" % inspect.isclass(attr))
-                    self.log.info("is module: %" % isModule(attr))
-
                     if inspect.isclass(attr) and isModule(attr) and attr != basemodule.Module:
                         # Get class name
                         fqcn = '.'.join([modname, attrname])
                         self.log.info("Module loaded : " + fqcn)
                         try:
                             # Load Module class
                             cls = load_class_from_name(fqcn)
```

### Comparing `spotinst-agent-beta-2.2.276/spotinst_agent/utils.py` & `spotinst-agent-beta-2.2.277/spotinst_agent/utils.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.276/spotinst_agent_beta.egg-info/PKG-INFO` & `spotinst-agent-beta-2.2.277/spotinst_agent_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.276
+Version: 2.2.277
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spotinst-agent-beta-2.2.276/spotinst_agent_beta.egg-info/SOURCES.txt` & `spotinst-agent-beta-2.2.277/spotinst_agent_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

