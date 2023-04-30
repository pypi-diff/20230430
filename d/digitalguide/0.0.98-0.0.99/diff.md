# Comparing `tmp/digitalguide-0.0.98.tar.gz` & `tmp/digitalguide-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalguide-0.0.98.tar", last modified: Thu Nov 18 21:38:31 2021, max compression
+gzip compressed data, was "digitalguide-0.0.99.tar", last modified: Thu Nov 18 21:41:55 2021, max compression
```

## Comparing `digitalguide-0.0.98.tar` & `digitalguide-0.0.99.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 21:38:31.360648 digitalguide-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2021-11-18 21:38:04.000000 digitalguide-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      223 2021-11-18 21:38:31.360648 digitalguide-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-11-18 21:38:04.000000 digitalguide-0.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 21:38:31.360648 digitalguide-0.0.98/digitalguide/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      662 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/contextActions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/conversationActions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/db_objects.py
--rw-r--r--   0 runner    (1001) docker     (121)      472 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/errorHandler.py
--rw-r--r--   0 runner    (1001) docker     (121)    13651 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/generateActions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3853 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/generateStates.py
--rw-r--r--   0 runner    (1001) docker     (121)     4073 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/gsheet2actions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1570 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/imageActions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1365 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/listenfrageActions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7984 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/mongo_persistence.py
--rw-r--r--   0 runner    (1001) docker     (121)     3828 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/pattern.py
--rw-r--r--   0 runner    (1001) docker     (121)      942 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/rasa_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2028 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/schaetzfragenActions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 21:38:31.360648 digitalguide-0.0.98/digitalguide/standardinteraktion/
--rw-r--r--   0 runner    (1001) docker     (121)     3406 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/standardinteraktion/Action.py
--rw-r--r--   0 runner    (1001) docker     (121)    13246 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/standardinteraktion/Interaktion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/standardinteraktion/Trigger.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/standardinteraktion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      338 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/uhrzeit_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2818 2021-11-18 21:38:04.000000 digitalguide-0.0.98/digitalguide/writeActions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 21:38:31.360648 digitalguide-0.0.98/digitalguide.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      223 2021-11-18 21:38:31.000000 digitalguide-0.0.98/digitalguide.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      921 2021-11-18 21:38:31.000000 digitalguide-0.0.98/digitalguide.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-18 21:38:31.000000 digitalguide-0.0.98/digitalguide.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      149 2021-11-18 21:38:31.000000 digitalguide-0.0.98/digitalguide.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-11-18 21:38:31.000000 digitalguide-0.0.98/digitalguide.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-18 21:38:31.360648 digitalguide-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      791 2021-11-18 21:38:04.000000 digitalguide-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 21:38:31.360648 digitalguide-0.0.98/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 21:38:04.000000 digitalguide-0.0.98/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2021-11-18 21:38:04.000000 digitalguide-0.0.98/tests/test_uhrzeit_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 21:41:55.036814 digitalguide-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (121)     1091 2021-11-18 21:41:23.000000 digitalguide-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2021-11-18 21:41:55.036814 digitalguide-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-11-18 21:41:23.000000 digitalguide-0.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 21:41:55.032814 digitalguide-0.0.99/digitalguide/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/contextActions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/conversationActions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1466 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/db_objects.py
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/errorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13651 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/generateActions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3853 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/generateStates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4100 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/gsheet2actions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1570 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/imageActions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1365 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/listenfrageActions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7984 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/mongo_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3828 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (121)      942 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/rasa_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2028 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/schaetzfragenActions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 21:41:55.036814 digitalguide-0.0.99/digitalguide/standardinteraktion/
+-rw-r--r--   0 runner    (1001) docker     (121)     3406 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/standardinteraktion/Action.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13246 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/standardinteraktion/Interaktion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1909 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/standardinteraktion/Trigger.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/standardinteraktion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      338 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/uhrzeit_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2818 2021-11-18 21:41:23.000000 digitalguide-0.0.99/digitalguide/writeActions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 21:41:55.036814 digitalguide-0.0.99/digitalguide.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2021-11-18 21:41:55.000000 digitalguide-0.0.99/digitalguide.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      921 2021-11-18 21:41:55.000000 digitalguide-0.0.99/digitalguide.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-18 21:41:55.000000 digitalguide-0.0.99/digitalguide.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2021-11-18 21:41:55.000000 digitalguide-0.0.99/digitalguide.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2021-11-18 21:41:55.000000 digitalguide-0.0.99/digitalguide.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-18 21:41:55.036814 digitalguide-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      791 2021-11-18 21:41:23.000000 digitalguide-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 21:41:55.036814 digitalguide-0.0.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 21:41:23.000000 digitalguide-0.0.99/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1204 2021-11-18 21:41:23.000000 digitalguide-0.0.99/tests/test_uhrzeit_filter.py
```

### Comparing `digitalguide-0.0.98/LICENSE` & `digitalguide-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `digitalguide-0.0.98/digitalguide/contextActions.py` & `digitalguide-0.0.99/digitalguide/contextActions.py`

 * *Files identical despite different names*

### Comparing `digitalguide-0.0.98/digitalguide/conversationActions.py` & `digitalguide-0.0.99/digitalguide/conversationActions.py`

 * *Files identical despite different names*

### Comparing `digitalguide-0.0.98/digitalguide/db_objects.py` & `digitalguide-0.0.99/digitalguide/db_objects.py`

 * *Files identical despite different names*

### Comparing `digitalguide-0.0.98/digitalguide/generateActions.py` & `digitalguide-0.0.99/digitalguide/generateActions.py`

 * *Files identical despite different names*

### Comparing `digitalguide-0.0.98/digitalguide/generateStates.py` & `digitalguide-0.0.99/digitalguide/generateStates.py`

 * *Files identical despite different names*

### Comparing `digitalguide-0.0.98/digitalguide/gsheet2actions.py` & `digitalguide-0.0.99/digitalguide/gsheet2actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,11 +117,11 @@
 
         states = {**states, **interaktion.states}
         actions = {**actions, **interaktion.actions}
         action_requirements += interaktion.action_requirements
     
     for action_requirement in action_requirements:
         if not action_requirement in actions.keys():
-            print("ERROR: Die erforderliche Aktion {} ist nicht definiert.")
+            print("ERROR: Die erforderliche Aktion {} ist nicht definiert.".format(action_requirement))
 
     states["NONE"]=[]
     return states, actions
```

### Comparing `digitalguide-0.0.98/digitalguide/imageActions.py` & `digitalguide-0.0.99/digitalguide/imageActions.py`

 * *Files identical despite different names*

### Comparing `digitalguide-0.0.98/digitalguide/listenfrageActions.py` & `digitalguide-0.0.99/digitalguide/listenfrageActions.py`

 * *Files identical despite different names*

### Comparing `digitalguide-0.0.98/digitalguide/mongo_persistence.py` & `digitalguide-0.0.99/digitalguide/mongo_persistence.py`

 * *Files identical despite different names*

### Comparing `digitalguide-0.0.98/digitalguide/pattern.py` & `digitalguide-0.0.99/digitalguide/pattern.py`

 * *Files identical despite different names*

### Comparing `digitalguide-0.0.98/digitalguide/rasa_filter.py` & `digitalguide-0.0.99/digitalguide/rasa_filter.py`

 * *Files identical despite different names*

### Comparing `digitalguide-0.0.98/digitalguide/schaetzfragenActions.py` & `digitalguide-0.0.99/digitalguide/schaetzfragenActions.py`

 * *Files identical despite different names*

### Comparing `digitalguide-0.0.98/digitalguide/standardinteraktion/Action.py` & `digitalguide-0.0.99/digitalguide/standardinteraktion/Action.py`

 * *Files identical despite different names*

### Comparing `digitalguide-0.0.98/digitalguide/standardinteraktion/Interaktion.py` & `digitalguide-0.0.99/digitalguide/standardinteraktion/Interaktion.py`

 * *Files identical despite different names*

### Comparing `digitalguide-0.0.98/digitalguide/standardinteraktion/Trigger.py` & `digitalguide-0.0.99/digitalguide/standardinteraktion/Trigger.py`

 * *Files identical despite different names*

### Comparing `digitalguide-0.0.98/digitalguide/writeActions.py` & `digitalguide-0.0.99/digitalguide/writeActions.py`

 * *Files identical despite different names*

### Comparing `digitalguide-0.0.98/digitalguide.egg-info/SOURCES.txt` & `digitalguide-0.0.99/digitalguide.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalguide-0.0.98/setup.py` & `digitalguide-0.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name='digitalguide',
     packages=find_packages(),
-    version='0.0.98',
+    version='0.0.99',
     description='A Python Library to write digital guides for telegram',
     author='Soeren Etler',
     license='MIT',
     install_requires=["python-telegram-bot",
                       "ctparse",
                       "boto3",
                       "pymongo[srv]",
```

### Comparing `digitalguide-0.0.98/tests/test_uhrzeit_filter.py` & `digitalguide-0.0.99/tests/test_uhrzeit_filter.py`

 * *Files identical despite different names*

