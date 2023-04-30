# Comparing `tmp/schoolware_api-1.0.7.tar.gz` & `tmp/schoolware_api-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schoolware_api-1.0.7.tar", last modified: Fri Apr 28 11:03:35 2023, max compression
+gzip compressed data, was "schoolware_api-1.0.8.tar", last modified: Fri Apr 28 11:10:22 2023, max compression
```

## Comparing `schoolware_api-1.0.7.tar` & `schoolware_api-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:03:35.913947 schoolware_api-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-28 11:03:35.913947 schoolware_api-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-28 11:03:22.000000 schoolware_api-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-28 11:03:22.000000 schoolware_api-1.0.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:03:35.913947 schoolware_api-1.0.7/schoolware_api/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 11:03:22.000000 schoolware_api-1.0.7/schoolware_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-04-28 11:03:22.000000 schoolware_api-1.0.7/schoolware_api/schoolware_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:03:35.913947 schoolware_api-1.0.7/schoolware_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-28 11:03:35.000000 schoolware_api-1.0.7/schoolware_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-28 11:03:35.000000 schoolware_api-1.0.7/schoolware_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:03:35.000000 schoolware_api-1.0.7/schoolware_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-28 11:03:35.000000 schoolware_api-1.0.7/schoolware_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 11:03:35.000000 schoolware_api-1.0.7/schoolware_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 11:03:35.913947 schoolware_api-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-28 11:03:22.000000 schoolware_api-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:10:22.009314 schoolware_api-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-28 11:10:22.009314 schoolware_api-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-28 11:10:06.000000 schoolware_api-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-28 11:10:06.000000 schoolware_api-1.0.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:10:22.005313 schoolware_api-1.0.8/schoolware_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 11:10:06.000000 schoolware_api-1.0.8/schoolware_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-04-28 11:10:06.000000 schoolware_api-1.0.8/schoolware_api/schoolware_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:10:22.009314 schoolware_api-1.0.8/schoolware_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-28 11:10:22.000000 schoolware_api-1.0.8/schoolware_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-28 11:10:22.000000 schoolware_api-1.0.8/schoolware_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:10:22.000000 schoolware_api-1.0.8/schoolware_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-28 11:10:22.000000 schoolware_api-1.0.8/schoolware_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 11:10:22.000000 schoolware_api-1.0.8/schoolware_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 11:10:22.009314 schoolware_api-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-28 11:10:06.000000 schoolware_api-1.0.8/setup.py
```

### Comparing `schoolware_api-1.0.7/PKG-INFO` & `schoolware_api-1.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware_api
-Version: 1.0.7
+Version: 1.0.8
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
@@ -33,36 +33,36 @@
 | password | school microsoft password
 | bg | background procces to keep token valid
 | bot_token | telegram bot token to enable telegram bot
 | chat_id | id to send messages to
 | verbose | show a lot more info
 
 ## Install
-* `pip3 install schoolware_api termcolor --upgrade `
+* `pip3 install schoolware_api --upgrade `
 * `playwright install &&  playwright install-deps`
 
 ## optional
 * `pip3 install python-telegram-bot`
 
 ## Simple example
 
 ```python
-from schoolware_api import schoolware_api
+from schoolware_api import schoolware
 
 config = {"domain":"", "user":"", "password":""} #example domain: kov.schoolware.be user: name.lastname@leerling.kov.be password: password 
 
-schoolware = schoolware_api.schoolware(config)
+Schoolware = schoolware(config)
 
-print(schoolware.todo())  # Returns all todo items
-print(schoolware.punten()) # Returns all scores this schoolyear
-print(schoolware.agenda()) # Returns agenda points today
-print(schoolware.agenda(datum="2023-03-06 00:00:00")) # Returns agenda points for 2023-03-06
+print(Schoolware.todo())  # Returns all todo items
+print(Schoolware.punten()) # Returns all scores this schoolyear
+print(Schoolware.agenda()) # Returns agenda points today
+print(Schoolware.agenda(datum="2023-03-06 00:00:00")) # Returns agenda points for 2023-03-06
 ```
 ## Complete example
 ```python
-from schoolware_api import schoolware_api
+from schoolware_api import schoolware
 config = {"domain":"","password":"","user":"","verbose": false, "bg": true, "bot_token": "", "chat_id": ""}
 
-schoolware = schoolware_api.schoolware(config)
+Schoolware = schoolware(config)
 
 # same as other
 ```
```

### Comparing `schoolware_api-1.0.7/README.md` & `schoolware_api-1.0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,36 +18,36 @@
 | password | school microsoft password
 | bg | background procces to keep token valid
 | bot_token | telegram bot token to enable telegram bot
 | chat_id | id to send messages to
 | verbose | show a lot more info
 
 ## Install
-* `pip3 install schoolware_api termcolor --upgrade `
+* `pip3 install schoolware_api --upgrade `
 * `playwright install &&  playwright install-deps`
 
 ## optional
 * `pip3 install python-telegram-bot`
 
 ## Simple example
 
 ```python
-from schoolware_api import schoolware_api
+from schoolware_api import schoolware
 
 config = {"domain":"", "user":"", "password":""} #example domain: kov.schoolware.be user: name.lastname@leerling.kov.be password: password 
 
-schoolware = schoolware_api.schoolware(config)
+Schoolware = schoolware(config)
 
-print(schoolware.todo())  # Returns all todo items
-print(schoolware.punten()) # Returns all scores this schoolyear
-print(schoolware.agenda()) # Returns agenda points today
-print(schoolware.agenda(datum="2023-03-06 00:00:00")) # Returns agenda points for 2023-03-06
+print(Schoolware.todo())  # Returns all todo items
+print(Schoolware.punten()) # Returns all scores this schoolyear
+print(Schoolware.agenda()) # Returns agenda points today
+print(Schoolware.agenda(datum="2023-03-06 00:00:00")) # Returns agenda points for 2023-03-06
 ```
 ## Complete example
 ```python
-from schoolware_api import schoolware_api
+from schoolware_api import schoolware
 config = {"domain":"","password":"","user":"","verbose": false, "bg": true, "bot_token": "", "chat_id": ""}
 
-schoolware = schoolware_api.schoolware(config)
+Schoolware = schoolware(config)
 
 # same as other
 ```
```

### Comparing `schoolware_api-1.0.7/pyproject.toml` & `schoolware_api-1.0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schoolware_api"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="MB", email="schoolware_api@mb-server.com" },
 ]
 description = "A api for schoolware written in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `schoolware_api-1.0.7/schoolware_api/schoolware_api.py` & `schoolware_api-1.0.8/schoolware_api/schoolware_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,25 @@
 from playwright.sync_api import sync_playwright
 import time
 from termcolor import colored
 import threading
 class schoolware:
 
     def __init__(self, config) -> None:
-        """Pass config file to init class
-
+        """Pass config dict to init class
         Args:
-            config (dict): The config file docs at https://github.com/Maarten-buelens/schoolware_api
+        | Key | Description |
+        | --- | --- |
+        | domain | domain name of schoolware
+        | user | school microsoft email
+        | password | school microsoft password
+        | bg | background procces to keep token valid
+        | bot_token | telegram bot token to enable telegram bot
+        | chat_id | id to send messages to
+        | verbose | show a lot more info
         """
         self.config = config
         if("debug" in config):
             self.verbose = config["debug"]
         else:
             self.verbose = False
         if("verbose" in config):
```

### Comparing `schoolware_api-1.0.7/schoolware_api.egg-info/PKG-INFO` & `schoolware_api-1.0.8/schoolware_api.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware-api
-Version: 1.0.7
+Version: 1.0.8
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
@@ -33,36 +33,36 @@
 | password | school microsoft password
 | bg | background procces to keep token valid
 | bot_token | telegram bot token to enable telegram bot
 | chat_id | id to send messages to
 | verbose | show a lot more info
 
 ## Install
-* `pip3 install schoolware_api termcolor --upgrade `
+* `pip3 install schoolware_api --upgrade `
 * `playwright install &&  playwright install-deps`
 
 ## optional
 * `pip3 install python-telegram-bot`
 
 ## Simple example
 
 ```python
-from schoolware_api import schoolware_api
+from schoolware_api import schoolware
 
 config = {"domain":"", "user":"", "password":""} #example domain: kov.schoolware.be user: name.lastname@leerling.kov.be password: password 
 
-schoolware = schoolware_api.schoolware(config)
+Schoolware = schoolware(config)
 
-print(schoolware.todo())  # Returns all todo items
-print(schoolware.punten()) # Returns all scores this schoolyear
-print(schoolware.agenda()) # Returns agenda points today
-print(schoolware.agenda(datum="2023-03-06 00:00:00")) # Returns agenda points for 2023-03-06
+print(Schoolware.todo())  # Returns all todo items
+print(Schoolware.punten()) # Returns all scores this schoolyear
+print(Schoolware.agenda()) # Returns agenda points today
+print(Schoolware.agenda(datum="2023-03-06 00:00:00")) # Returns agenda points for 2023-03-06
 ```
 ## Complete example
 ```python
-from schoolware_api import schoolware_api
+from schoolware_api import schoolware
 config = {"domain":"","password":"","user":"","verbose": false, "bg": true, "bot_token": "", "chat_id": ""}
 
-schoolware = schoolware_api.schoolware(config)
+Schoolware = schoolware(config)
 
 # same as other
 ```
```

