# Comparing `tmp/spotinst-agent-beta-2.2.274.tar.gz` & `tmp/spotinst-agent-beta-2.2.275.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-agent-beta-2.2.274.tar", last modified: Sun Apr 30 07:43:56 2023, max compression
+gzip compressed data, was "spotinst-agent-beta-2.2.275.tar", last modified: Sun Apr 30 07:57:54 2023, max compression
```

## Comparing `spotinst-agent-beta-2.2.274.tar` & `spotinst-agent-beta-2.2.275.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:43:56.087159 spotinst-agent-beta-2.2.274/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.274/LICENSE
--rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.274/MANIFEST.in
--rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 07:43:56.086982 spotinst-agent-beta-2.2.274/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.274/README.rst
--rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-30 07:43:56.087211 spotinst-agent-beta-2.2.274/setup.cfg
--rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-30 07:43:53.000000 spotinst-agent-beta-2.2.274/setup.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:43:56.084102 spotinst-agent-beta-2.2.274/spotinst_agent/
--rw-r--r--   0 ayeletc    (502) staff       (20)    13080 2023-04-27 12:18:46.000000 spotinst-agent-beta-2.2.274/spotinst_agent/__init__.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.274/spotinst_agent/agent.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.274/spotinst_agent/agentinit.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.274/spotinst_agent/basemodule.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:43:56.081014 spotinst-agent-beta-2.2.274/spotinst_agent/data/
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:43:56.084625 spotinst-agent-beta-2.2.274/spotinst_agent/data/configuration/
--rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.274/spotinst_agent/data/configuration/basemodule.yml
--rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.274/spotinst_agent/data/configuration/spotinst-agent.yml
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:43:56.084891 spotinst-agent-beta-2.2.274/spotinst_agent/data/installation/
--rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.274/spotinst_agent/data/installation/agent-init.sh
--rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.274/spotinst_agent/scheduler.py
--rw-r--r--   0 ayeletc    (502) staff       (20)    10935 2023-04-30 07:43:53.000000 spotinst-agent-beta-2.2.274/spotinst_agent/taskmanager.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.274/spotinst_agent/utils.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:43:56.086701 spotinst-agent-beta-2.2.274/spotinst_agent_beta.egg-info/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 07:43:56.000000 spotinst-agent-beta-2.2.274/spotinst_agent_beta.egg-info/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-30 07:43:56.000000 spotinst-agent-beta-2.2.274/spotinst_agent_beta.egg-info/SOURCES.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-30 07:43:56.000000 spotinst-agent-beta-2.2.274/spotinst_agent_beta.egg-info/dependency_links.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       55 2023-04-30 07:43:56.000000 spotinst-agent-beta-2.2.274/spotinst_agent_beta.egg-info/entry_points.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-30 07:43:56.000000 spotinst-agent-beta-2.2.274/spotinst_agent_beta.egg-info/requires.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-30 07:43:56.000000 spotinst-agent-beta-2.2.274/spotinst_agent_beta.egg-info/top_level.txt
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:57:54.621906 spotinst-agent-beta-2.2.275/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.275/LICENSE
+-rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.275/MANIFEST.in
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 07:57:54.621702 spotinst-agent-beta-2.2.275/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.275/README.rst
+-rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-30 07:57:54.621978 spotinst-agent-beta-2.2.275/setup.cfg
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-30 07:57:51.000000 spotinst-agent-beta-2.2.275/setup.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:57:54.618862 spotinst-agent-beta-2.2.275/spotinst_agent/
+-rw-r--r--   0 ayeletc    (502) staff       (20)    13097 2023-04-30 07:57:51.000000 spotinst-agent-beta-2.2.275/spotinst_agent/__init__.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.275/spotinst_agent/agent.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.275/spotinst_agent/agentinit.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.275/spotinst_agent/basemodule.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:57:54.613752 spotinst-agent-beta-2.2.275/spotinst_agent/data/
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:57:54.619571 spotinst-agent-beta-2.2.275/spotinst_agent/data/configuration/
+-rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.275/spotinst_agent/data/configuration/basemodule.yml
+-rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.275/spotinst_agent/data/configuration/spotinst-agent.yml
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:57:54.619787 spotinst-agent-beta-2.2.275/spotinst_agent/data/installation/
+-rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.275/spotinst_agent/data/installation/agent-init.sh
+-rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.275/spotinst_agent/scheduler.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)    10902 2023-04-30 07:54:06.000000 spotinst-agent-beta-2.2.275/spotinst_agent/taskmanager.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.275/spotinst_agent/utils.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 07:57:54.621383 spotinst-agent-beta-2.2.275/spotinst_agent_beta.egg-info/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 07:57:54.000000 spotinst-agent-beta-2.2.275/spotinst_agent_beta.egg-info/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-30 07:57:54.000000 spotinst-agent-beta-2.2.275/spotinst_agent_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-30 07:57:54.000000 spotinst-agent-beta-2.2.275/spotinst_agent_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       55 2023-04-30 07:57:54.000000 spotinst-agent-beta-2.2.275/spotinst_agent_beta.egg-info/entry_points.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-30 07:57:54.000000 spotinst-agent-beta-2.2.275/spotinst_agent_beta.egg-info/requires.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-30 07:57:54.000000 spotinst-agent-beta-2.2.275/spotinst_agent_beta.egg-info/top_level.txt
```

### Comparing `spotinst-agent-beta-2.2.274/LICENSE` & `spotinst-agent-beta-2.2.275/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.274/PKG-INFO` & `spotinst-agent-beta-2.2.275/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.274
+Version: 2.2.275
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spotinst-agent-beta-2.2.274/README.rst` & `spotinst-agent-beta-2.2.275/README.rst`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.274/setup.py` & `spotinst-agent-beta-2.2.275/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='spotinst-agent-beta',
 
-    version="2.2.274",
+    version="2.2.275",
 
     description='Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.',
 
     long_description=description,
 
     # The project's main homepage.
     url='https://github.com/spotinst/spotinst-spectrum-agent',
```

### Comparing `spotinst-agent-beta-2.2.274/spotinst_agent/__init__.py` & `spotinst-agent-beta-2.2.275/spotinst_agent/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import os
 import subprocess
 import urllib2
 import utils
 import sys
 from shutil import copyfile
-from .agent import run_agent
+from agent import run_agent
 from time import sleep
 
 
 def main():
     s3_base_link = 'https://s3.amazonaws.com/spotinst-public/services/spotinst-agent'
     s3_base_workers_link = s3_base_link + "/workers"
     s3_base_collectors_link = s3_base_link + "/collectors"
@@ -18,15 +18,15 @@
     initiator_modules_path = '/etc/spotinst/agent/initiators/modules'
     instance_details_path = '/etc/spotinst'
 
     results = parse_arguments()
     action = results.action
     argument = results.argument
     second_argument = results.second_argument
-    third_argument = results.third_argument
+    third_argument  = results.third_argument
     cloud_provider = results.cloud_provider
     args = vars(results)
     verbose = False
     debug = False
 
     if args['verbose']:
         verbose = True
@@ -34,47 +34,47 @@
     if args['debug']:
         debug = True
 
     if action == "add-worker":
         if argument is not None:
             install_worker(modules_path, s3_base_workers_link, argument)
         else:
-            print("Please enter the name of the worker which you want to add.")
+            print ("Please enter the name of the worker which you want to add.")
 
     elif action == "add-collector":
         if argument is not None:
             install_collector(argument, modules_path, s3_base_collectors_link)
         else:
-            print("Please enter the name of the collector which you want to add.")
+            print ("Please enter the name of the collector which you want to add.")
 
     elif action == "add-initiator":
         if argument is not None:
             install_initiator(argument, initiator_modules_path, s3_base_initiator_link)
         else:
             print("Please enter the name of the initiator which you want to add.")
 
     elif action == "run":
         run_agent(debug, verbose, cloud_provider)
 
     elif action == "configure":
         if argument is not None:
-            print("configuring " + argument)
+            print ("configuring " + argument)
         else:
-            print("Spotinst agent configuration")
+            print ("Spotinst agent configuration")
 
     elif action == "init":
 
         try_num = 1
         install_succeed = False
         while (not install_succeed) and (try_num <= 3):
             if try_num > 1:
                 sleep(20)
                 print("trying to Initializing agent again (retry %s/3)" % (format(try_num)))
             try_num += 1
-            print("Initializing agent")
+            print ("Initializing agent")
             install_succeed = handle_cloud_provider(cloud_provider, instance_details_path) and install_and_init_agent(
                 argument, second_argument, third_argument, modules_path, initiator_modules_path)
 
         if not install_succeed:
             print("init failed")
             exit(1)
         else:
@@ -94,15 +94,15 @@
         create_agent_local_folders()
         handle_base_modules(dirname, modules_path, initiator_modules_path)
         handle_yml_file(dirname)
         handle_credentials(account_id, script_full_path, spotinst_agent_path, token, custom_host)
         handle_agent_path(spotinst_agent_path)
         runscript = subprocess.Popen(script_full_path)
         runscript.wait()
-        print('result : ' + str(runscript.communicate()))
+        print ('result : ' + str(runscript.communicate()))
     except:
         if runscript is not None:
             runscript.kill()
         return False
     return True
 
 
@@ -114,15 +114,15 @@
         full_path = instance_details_path + "/cloud_provider.txt"
         cloud_provider_file = open(full_path, 'w')
         cloud_provider_file.write(cloud_provider)
         cloud_provider_file.close()
         os.chmod(full_path, 0o644)
         return True
     except IOError:
-        print("Unable to create /etc/spotinst/cloud_provider.txt")
+        print ("Unable to create /etc/spotinst/cloud_provider.txt")
         if cloud_provider_file is not None:
             cloud_provider_file.close()
         return False
 
 
 def create_agent_local_folders():
     if not os.path.exists('/etc/spotinst'):
@@ -157,18 +157,18 @@
     default_yml_destination = '/etc/spotinst/agent/config/spotinst-agent.yml'
     if not os.path.exists('/etc/spotinst/agent/config/spotinst-agent.yml'):
         copyfile(default_agent_yml, default_yml_destination)
 
 
 def handle_credentials(account_id, script_full_path, spotinst_agent_path, token, host):
     if token is not None:
-        print("Creating Spotinst credentials directory")
+        print ("Creating Spotinst credentials directory")
 
         if host is None:
-            # if the customer didn't supply custom host set the default
+            #if the customer didn't supply custom host set the default
             host = 'api.spotinst.io'
         creds_file, creds_path = create_creds_file()
         write_creds_path(account_id, creds_file, token, host)
         os.chmod(creds_path, 0o777)
 
     else:
         # Credentials already exist - retrieve from file
@@ -198,15 +198,15 @@
     return creds_file, creds_path
 
 
 def handle_agent_path(spotinst_agent_path):
     try:
         os.symlink(spotinst_agent_path, '/usr/local/bin/spotinst-agent-service')
     except OSError:
-        print('Symlink exists. Skipping symlink creation.')
+        print ('Symlink exists. Skipping symlink creation.')
     os.chmod(spotinst_agent_path, 0o777)
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(description='Spotinst Agent')
     parser.add_argument('action',
                         action="store",
@@ -232,31 +232,31 @@
                         default='AWS',
                         help='The cloud provider, supports: \'AWS\'(default), \'Azure\', \'Azure_Spot\', \'GCP\'')
     results = parser.parse_args()
     return results
 
 
 def install_worker(modules_path, s3_base_workers_link, worker_name):
-    print("adding worker " + worker_name)
+    print ("adding worker " + worker_name)
     try:
         handle_prerequisites(s3_base_workers_link, worker_name)
         get_worker_files(modules_path, s3_base_workers_link, worker_name)
 
     except Exception as e:
-        print("Could not get worker " + str(worker_name) + " Exception : " + str(e))
+        print ("Could not get worker " + str(worker_name) + " Exception : " + str(e))
 
 
 def install_collector(collector_name, modules_path, s3_base_collectors_link):
-    print("adding collector " + collector_name)
+    print ("adding collector " + collector_name)
     try:
         handle_prerequisites(s3_base_collectors_link, collector_name)
         get_collector_files(collector_name, modules_path, s3_base_collectors_link)
 
     except Exception as e:
-        print("Could not get collector " + collector_name + " Exception : " + str(e))
+        print ("Could not get collector " + collector_name + " Exception : " + str(e))
 
 
 def install_initiator(initiator_name, initiator_modules_path, s3_base_initiator_link):
     print("adding initiator " + initiator_name)
     try:
         get_initiator_files(initiator_name, initiator_modules_path, s3_base_initiator_link)
 
@@ -293,30 +293,30 @@
 
 
 def handle_prerequisites(s3_base_module_link, module_name):
     try:
         response = urllib2.urlopen(s3_base_module_link + '/' + module_name + '/' + module_name + '.req')
         requirements_file = response.read()
         requirements_names = requirements_file.split("\n")
-        print("This module requires the following packages to be installed:")
+        print ("This module requires the following packages to be installed:")
         for requirement in requirements_names:
-            print(requirement)
+            print (requirement)
 
         if len(requirements_names) > 0:
             import pip
             installed_packages = pip.get_installed_distributions()
             flat_installed_packages = [package.project_name for package in installed_packages]
 
             missing_packages = []
             for requirement in requirements_names:
                 if requirement not in flat_installed_packages:
                     missing_packages.append(requirement)
 
             if len(missing_packages) <= 0:
-                print("All prerequisites have been met.")
+                print ("All prerequisites have been met.")
                 pass
             else:
-                print("Some prerequisites for this module have not been met. " \
-                      "Please install the following before proceeding: " + str(missing_packages))
+                print ("Some prerequisites for this module have not been met. " \
+                       "Please install the following before proceeding: " + str(missing_packages))
                 sys.exit(1)
     except Exception:
         pass
```

### Comparing `spotinst-agent-beta-2.2.274/spotinst_agent/agent.py` & `spotinst-agent-beta-2.2.275/spotinst_agent/agent.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.274/spotinst_agent/agentinit.py` & `spotinst-agent-beta-2.2.275/spotinst_agent/agentinit.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.274/spotinst_agent/basemodule.py` & `spotinst-agent-beta-2.2.275/spotinst_agent/basemodule.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.274/spotinst_agent/data/configuration/spotinst-agent.yml` & `spotinst-agent-beta-2.2.275/spotinst_agent/data/configuration/spotinst-agent.yml`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.274/spotinst_agent/data/installation/agent-init.sh` & `spotinst-agent-beta-2.2.275/spotinst_agent/data/installation/agent-init.sh`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.274/spotinst_agent/scheduler.py` & `spotinst-agent-beta-2.2.275/spotinst_agent/scheduler.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.274/spotinst_agent/taskmanager.py` & `spotinst-agent-beta-2.2.275/spotinst_agent/taskmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,28 +142,25 @@
                     continue
 
                 # import module only if it exists for more than 1 second (had enough time to write the entire content)
                 now = time.time()
                 if now - mod_modification_time < 1:
                     self.log.info("Not loading file since it was created too recently: modified at %s, now is %s" % (mod_modification_time, now))
                 #     continue
-                time.sleep(45)
                 try:
                     # Import the module
                     self.log.info("Importing %s" % modname)
                     mod = __import__(modname, globals(), locals(), ['*'])
                 except Exception as e:
                     # Log error
                     self.log.error("Failed to import module: %s. %s" % (modname, traceback.format_exc()))
                     continue
 
                 # Find all classes defined in the module
                 self.log.info("Finding classes defined in module " + str(modname))
-
-
                 for attrname in dir(mod):
                     attr = getattr(mod, attrname)
                     # Only attempt to load classes that are infact classes but not the base Module class
                     self.log.debug("Checking " + str(modname) + " Attribute " + str(attrname))
                     self.log.info("Checking " + str(modname) + " Attribute " + str(attrname))
 
                     if inspect.isclass(attr) and isModule(attr) and attr != basemodule.Module:
```

### Comparing `spotinst-agent-beta-2.2.274/spotinst_agent/utils.py` & `spotinst-agent-beta-2.2.275/spotinst_agent/utils.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.274/spotinst_agent_beta.egg-info/PKG-INFO` & `spotinst-agent-beta-2.2.275/spotinst_agent_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.274
+Version: 2.2.275
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spotinst-agent-beta-2.2.274/spotinst_agent_beta.egg-info/SOURCES.txt` & `spotinst-agent-beta-2.2.275/spotinst_agent_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

