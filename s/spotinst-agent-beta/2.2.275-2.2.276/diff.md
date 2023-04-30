# Comparing `tmp/spotinst-agent-beta-2.2.275.tar.gz` & `tmp/spotinst-agent-beta-2.2.276.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-agent-beta-2.2.275.tar", last modified: Sun Apr 30 07:57:54 2023, max compression
+gzip compressed data, was "spotinst-agent-beta-2.2.276.tar", last modified: Sun Apr 30 10:58:50 2023, max compression
```

## Comparing `spotinst-agent-beta-2.2.275.tar` & `spotinst-agent-beta-2.2.276.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:57:54.621906 spotinst-agent-beta-2.2.275/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.275/LICENSE
--rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.275/MANIFEST.in
--rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 07:57:54.621702 spotinst-agent-beta-2.2.275/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.275/README.rst
--rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-30 07:57:54.621978 spotinst-agent-beta-2.2.275/setup.cfg
--rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-30 07:57:51.000000 spotinst-agent-beta-2.2.275/setup.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:57:54.618862 spotinst-agent-beta-2.2.275/spotinst_agent/
--rw-r--r--   0 ayeletc    (502) staff       (20)    13097 2023-04-30 07:57:51.000000 spotinst-agent-beta-2.2.275/spotinst_agent/__init__.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.275/spotinst_agent/agent.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.275/spotinst_agent/agentinit.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.275/spotinst_agent/basemodule.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:57:54.613752 spotinst-agent-beta-2.2.275/spotinst_agent/data/
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:57:54.619571 spotinst-agent-beta-2.2.275/spotinst_agent/data/configuration/
--rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.275/spotinst_agent/data/configuration/basemodule.yml
--rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.275/spotinst_agent/data/configuration/spotinst-agent.yml
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:57:54.619787 spotinst-agent-beta-2.2.275/spotinst_agent/data/installation/
--rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.275/spotinst_agent/data/installation/agent-init.sh
--rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.275/spotinst_agent/scheduler.py
--rw-r--r--   0 ayeletc    (502) staff       (20)    10902 2023-04-30 07:54:06.000000 spotinst-agent-beta-2.2.275/spotinst_agent/taskmanager.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.275/spotinst_agent/utils.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:57:54.621383 spotinst-agent-beta-2.2.275/spotinst_agent_beta.egg-info/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 07:57:54.000000 spotinst-agent-beta-2.2.275/spotinst_agent_beta.egg-info/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-30 07:57:54.000000 spotinst-agent-beta-2.2.275/spotinst_agent_beta.egg-info/SOURCES.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-30 07:57:54.000000 spotinst-agent-beta-2.2.275/spotinst_agent_beta.egg-info/dependency_links.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       55 2023-04-30 07:57:54.000000 spotinst-agent-beta-2.2.275/spotinst_agent_beta.egg-info/entry_points.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-30 07:57:54.000000 spotinst-agent-beta-2.2.275/spotinst_agent_beta.egg-info/requires.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-30 07:57:54.000000 spotinst-agent-beta-2.2.275/spotinst_agent_beta.egg-info/top_level.txt
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 10:58:50.882691 spotinst-agent-beta-2.2.276/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.276/LICENSE
+-rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.276/MANIFEST.in
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 10:58:50.882486 spotinst-agent-beta-2.2.276/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.276/README.rst
+-rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-30 10:58:50.882738 spotinst-agent-beta-2.2.276/setup.cfg
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-30 10:58:49.000000 spotinst-agent-beta-2.2.276/setup.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 10:58:50.878900 spotinst-agent-beta-2.2.276/spotinst_agent/
+-rw-r--r--   0 ayeletc    (502) staff       (20)    13173 2023-04-30 10:58:32.000000 spotinst-agent-beta-2.2.276/spotinst_agent/__init__.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.276/spotinst_agent/agent.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.276/spotinst_agent/agentinit.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.276/spotinst_agent/basemodule.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 10:58:50.861323 spotinst-agent-beta-2.2.276/spotinst_agent/data/
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 10:58:50.879464 spotinst-agent-beta-2.2.276/spotinst_agent/data/configuration/
+-rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.276/spotinst_agent/data/configuration/basemodule.yml
+-rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.276/spotinst_agent/data/configuration/spotinst-agent.yml
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 10:58:50.879803 spotinst-agent-beta-2.2.276/spotinst_agent/data/installation/
+-rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.276/spotinst_agent/data/installation/agent-init.sh
+-rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.276/spotinst_agent/scheduler.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)    11040 2023-04-30 10:01:09.000000 spotinst-agent-beta-2.2.276/spotinst_agent/taskmanager.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.276/spotinst_agent/utils.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 10:58:50.882166 spotinst-agent-beta-2.2.276/spotinst_agent_beta.egg-info/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 10:58:50.000000 spotinst-agent-beta-2.2.276/spotinst_agent_beta.egg-info/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-30 10:58:50.000000 spotinst-agent-beta-2.2.276/spotinst_agent_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-30 10:58:50.000000 spotinst-agent-beta-2.2.276/spotinst_agent_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       55 2023-04-30 10:58:50.000000 spotinst-agent-beta-2.2.276/spotinst_agent_beta.egg-info/entry_points.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-30 10:58:50.000000 spotinst-agent-beta-2.2.276/spotinst_agent_beta.egg-info/requires.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-30 10:58:50.000000 spotinst-agent-beta-2.2.276/spotinst_agent_beta.egg-info/top_level.txt
```

### Comparing `spotinst-agent-beta-2.2.275/LICENSE` & `spotinst-agent-beta-2.2.276/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.275/PKG-INFO` & `spotinst-agent-beta-2.2.276/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.275
+Version: 2.2.276
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spotinst-agent-beta-2.2.275/README.rst` & `spotinst-agent-beta-2.2.276/README.rst`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.275/setup.py` & `spotinst-agent-beta-2.2.276/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='spotinst-agent-beta',
 
-    version="2.2.275",
+    version="2.2.276",
 
     description='Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.',
 
     long_description=description,
 
     # The project's main homepage.
     url='https://github.com/spotinst/spotinst-spectrum-agent',
```

### Comparing `spotinst-agent-beta-2.2.275/spotinst_agent/__init__.py` & `spotinst-agent-beta-2.2.276/spotinst_agent/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,14 +254,15 @@
     except Exception as e:
         print ("Could not get collector " + collector_name + " Exception : " + str(e))
 
 
 def install_initiator(initiator_name, initiator_modules_path, s3_base_initiator_link):
     print("adding initiator " + initiator_name)
     try:
+        handle_prerequisites(s3_base_initiator_link, initiator_name)
         get_initiator_files(initiator_name, initiator_modules_path, s3_base_initiator_link)
 
     except Exception as e:
         print("Could not get initiator " + initiator_name + " Exception : " + str(e))
 
 
 def get_worker_files(modules_path, s3_base_workers_link, worker_name):
@@ -280,20 +281,21 @@
         collector.write(response.read())
     with open(modules_path + '/' + collector_name + '.yml', 'wb') as collector_cfg:
         response = urllib2.urlopen(s3_base_collectors_link + '/' + collector_name + '/' + collector_name + '.yml')
         collector_cfg.write(response.read())
 
 
 def get_initiator_files(initiator_name, initiator_modules_path, s3_base_initiator_link):
+    py_response = urllib2.urlopen(s3_base_initiator_link + '/' + initiator_name + '/' + initiator_name + '.py')
+    yml_response = urllib2.urlopen(s3_base_initiator_link + '/' + initiator_name + '/' + initiator_name + '.yml')
+
     with open(initiator_modules_path + '/' + initiator_name + '.py', 'wb') as initiator:
-        response = urllib2.urlopen(s3_base_initiator_link + '/' + initiator_name + '/' + initiator_name + '.py')
-        initiator.write(response.read())
+        initiator.write(py_response.read())
     with open(initiator_modules_path + '/' + initiator_name + '.yml', 'wb') as initiator_cfg:
-        response = urllib2.urlopen(s3_base_initiator_link + '/' + initiator_name + '/' + initiator_name + '.yml')
-        initiator_cfg.write(response.read())
+        initiator_cfg.write(yml_response.read())
 
 
 def handle_prerequisites(s3_base_module_link, module_name):
     try:
         response = urllib2.urlopen(s3_base_module_link + '/' + module_name + '/' + module_name + '.req')
         requirements_file = response.read()
         requirements_names = requirements_file.split("\n")
```

### Comparing `spotinst-agent-beta-2.2.275/spotinst_agent/agent.py` & `spotinst-agent-beta-2.2.276/spotinst_agent/agent.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.275/spotinst_agent/agentinit.py` & `spotinst-agent-beta-2.2.276/spotinst_agent/agentinit.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.275/spotinst_agent/basemodule.py` & `spotinst-agent-beta-2.2.276/spotinst_agent/basemodule.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.275/spotinst_agent/data/configuration/spotinst-agent.yml` & `spotinst-agent-beta-2.2.276/spotinst_agent/data/configuration/spotinst-agent.yml`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.275/spotinst_agent/data/installation/agent-init.sh` & `spotinst-agent-beta-2.2.276/spotinst_agent/data/installation/agent-init.sh`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.275/spotinst_agent/scheduler.py` & `spotinst-agent-beta-2.2.276/spotinst_agent/scheduler.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.275/spotinst_agent/taskmanager.py` & `spotinst-agent-beta-2.2.276/spotinst_agent/taskmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,24 +132,25 @@
                 mod_modification_time_str = str(mod_modification_time)
                 self.log.info("Py file found: %s" % modname)
 
                 modules_list = [x.lower() for x in self.tasks.keys()]
                 if modname in modules_list:
                     if self.tasks[modname]['modification_time'] == mod_modification_time_str:
                         self.log.info("Module '{0}' already loaded".format(modname))
-                #         continue
+                        continue
 
                 if modname == "utils" or modname == "basemodule":
                     continue
 
                 # import module only if it exists for more than 1 second (had enough time to write the entire content)
                 now = time.time()
                 if now - mod_modification_time < 1:
                     self.log.info("Not loading file since it was created too recently: modified at %s, now is %s" % (mod_modification_time, now))
-                #     continue
+                    continue
+
                 try:
                     # Import the module
                     self.log.info("Importing %s" % modname)
                     mod = __import__(modname, globals(), locals(), ['*'])
                 except Exception as e:
                     # Log error
                     self.log.error("Failed to import module: %s. %s" % (modname, traceback.format_exc()))
@@ -159,14 +160,17 @@
                 self.log.info("Finding classes defined in module " + str(modname))
                 for attrname in dir(mod):
                     attr = getattr(mod, attrname)
                     # Only attempt to load classes that are infact classes but not the base Module class
                     self.log.debug("Checking " + str(modname) + " Attribute " + str(attrname))
                     self.log.info("Checking " + str(modname) + " Attribute " + str(attrname))
 
+                    self.log.info("is class: %" % inspect.isclass(attr))
+                    self.log.info("is module: %" % isModule(attr))
+
                     if inspect.isclass(attr) and isModule(attr) and attr != basemodule.Module:
                         # Get class name
                         fqcn = '.'.join([modname, attrname])
                         self.log.info("Module loaded : " + fqcn)
                         try:
                             # Load Module class
                             cls = load_class_from_name(fqcn)
```

### Comparing `spotinst-agent-beta-2.2.275/spotinst_agent/utils.py` & `spotinst-agent-beta-2.2.276/spotinst_agent/utils.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.275/spotinst_agent_beta.egg-info/PKG-INFO` & `spotinst-agent-beta-2.2.276/spotinst_agent_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.275
+Version: 2.2.276
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spotinst-agent-beta-2.2.275/spotinst_agent_beta.egg-info/SOURCES.txt` & `spotinst-agent-beta-2.2.276/spotinst_agent_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

