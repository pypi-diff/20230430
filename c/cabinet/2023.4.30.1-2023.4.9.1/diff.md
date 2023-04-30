# Comparing `tmp/cabinet-2023.4.30.1.tar.gz` & `tmp/cabinet-2023.4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2023.4.30.1.tar", last modified: Sun Apr 30 05:32:56 2023, max compression
+gzip compressed data, was "cabinet-2023.4.9.1.tar", last modified: Mon Apr 10 04:09:49 2023, max compression
```

## Comparing `cabinet-2023.4.30.1.tar` & `cabinet-2023.4.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-30 05:32:56.980301 cabinet-2023.4.30.1/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.4.30.1/LICENSE
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6494 2023-04-30 05:32:56.980301 cabinet-2023.4.30.1/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6142 2023-04-16 16:59:23.000000 cabinet-2023.4.30.1/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.4.30.1/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-04-30 05:32:56.980301 cabinet-2023.4.30.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-30 05:32:56.980301 cabinet-2023.4.30.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-30 05:32:56.980301 cabinet-2023.4.30.1/src/cabinet/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    25639 2023-04-30 05:31:21.000000 cabinet-2023.4.30.1/src/cabinet/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-03-25 22:04:50.000000 cabinet-2023.4.30.1/src/cabinet/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3687 2023-04-16 16:59:23.000000 cabinet-2023.4.30.1/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-30 05:32:56.980301 cabinet-2023.4.30.1/src/cabinet.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6494 2023-04-30 05:32:56.000000 cabinet-2023.4.30.1/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      288 2023-04-30 05:32:56.000000 cabinet-2023.4.30.1/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-04-30 05:32:56.000000 cabinet-2023.4.30.1/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-04-30 05:32:56.000000 cabinet-2023.4.30.1/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-04-30 05:32:56.000000 cabinet-2023.4.30.1/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.4.9.1/LICENSE
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4365 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4014 2023-03-25 22:04:50.000000 cabinet-2023.4.9.1/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.4.9.1/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/src/cabinet/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    20802 2023-03-25 22:04:50.000000 cabinet-2023.4.9.1/src/cabinet/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-03-25 22:04:50.000000 cabinet-2023.4.9.1/src/cabinet/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2737 2023-03-25 22:04:50.000000 cabinet-2023.4.9.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/src/cabinet.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4365 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      288 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/top_level.txt
```

### Comparing `cabinet-2023.4.30.1/LICENSE` & `cabinet-2023.4.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cabinet-2023.4.30.1/PKG-INFO` & `cabinet-2023.4.9.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.4.30.1
+Version: 2023.4.9.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cabinet
 A Python library to easily store data across multiple projects in one or more JSON files.
 
-Supports a cli, email, and event logging.
+Supports email and event logging.
 
 ## Features
 
 - Read and write data in the JSON files of your choice
 - Log to a file/directory of your choice without having to configure `logger` each time
 - Send/receive mail using `cabinet.Cabinet().mail()`
 
@@ -28,210 +28,131 @@
   - this can be changed on a per-log basis
 
 ## Installation and Setup
 
 ```bash
   python3 -m pip install cabinet
 
-  cabinet --config
-```
-
-## CLI usage
-```
-Usage: cabinet [OPTIONS]
-
-Options:
-  -h, --help              Show this help message and exit
-  --configure, -config    Configure
-  --edit, -e              Edit the settings.json file
-  --edit-file, -ef        Edit a specific file
-  --no-create             (for -ef) Do not create file if it does not exist
-  --get, -g [GET ...]     Get a property from settings.json
-  --put PUT [PUT ...]     Put a property into settings.json
-  --get-file GET_FILE     Get file
-  --strip                 (for --get-file) Whether to strip file content whitespace
-  --log, -l               Log a message to the default location
-  --level LOG_LEVEL       (for -l) Log level [debug, info, warn, error, critical]
-  -v, --version           show version number and exit
-
-Mail:
-  --mail                Sends an email
-  --subject SUBJECT, -s SUBJECT
-                        Email subject
-  --body BODY, -b BODY  Email body
-  --to TO_ADDR, -t TO_ADDR
+  cabinet config
 ```
 
 ## Configuration
 
-- Upon first launch, will prompt you to choose a location for `settings.json`. You can change this at any time with `cabinet --config`.
+- Upon first launch, will prompt you to choose a location for `settings.json`. You can change this at any time with `cabinet config`.
 
-### edit_file() shortcuts
-- see example below to enable something like
-  - `cabinet -ef shopping` from the terminal
-    - rather than `cabinet -ef "/home/{username}/path/to/shopping_list.md"`
-  - or `cabinet.Cabinet().edit("shopping")`
-    - rather than `cabinet.Cabinet().edit("/home/{username}/path/to/whatever.md")`
+### edit() shortcuts
+- see example below to enable something like `cabinet edit shopping` from the terminal
+  - or `cabinet.Cabinet().edit("shopping")`, rather than `cabinet.Cabinet().edit("/home/{username}/path/to/shopping.md")`
 
-file:
 ```
 # example only; these commands will be unique to your setup
 
 {
   "path": {
     "edit": {
       "shopping": {
-        "value": "/home/{username}/path/to/whatever.md",
+        "value": "/home/{username}/path/to/shopping.md",
       },
       "todo": {
-        "value": "/home/{username}/path/to/whatever.md",
+        "value": "/home/{username}/path/to/todo.md",
       }
     }
   }
 }
 ```
 
-set from terminal:
-```
-cabinet -p edit shopping value "/home/{username}/path/to/whatever.md"
-cabinet -p edit todo value "/home/{username}/path/to/whatever.md"
-```
-
 ### mail
 
 - It is NEVER a good idea to store your password in plaintext; for this reason, I strongly recommend a "throwaway" account that is only used for sending emails
 - Gmail (as of May 2022) and most other mainstream email providers won't work with this; for support, search for sending mail from your email provider with `smtplib`.
 - In `settings.json`, add the `email` object to make your settings file look like this example:
 
-file:
 ```
 {
     "email": {
         "from": "throwaway@example.com",
         "from_pw": "example",
         "from_name": "Raspberry Pi",
         "to": "destination@protonmail.com",
         "smtp_server": "example.com",
         "imap_server": "example.com",
         "port": 123
     }
 }
 ```
 
-set from terminal:
-```
-cabinet -p email from throwaway@example.com
-cabinet -p email from_pw example
-...
-```
-
 ## Examples
 
-### `put`
+### `set`
 
-python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
 
-cab.put("employee", "Tyler", "salary", 7.25)
-```
-
-or terminal:
-```
-# warning - from the terminal, numeric values in cabinet are stored as strings
-cabinet -p employer Tyler salary 7.25
+cab.set("employee", "Tyler", "salary", 7.25)
 ```
 
 results in this structure in settings.json:
+
 ```
 {
     "employee": {
         "Tyler": {
-            "salary": 7.25 # or "7.25" if done from terminal
+            "salary": 7.25
         }
     }
 }
 ```
 
 ### `get`
 
-python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
 
 print(cab.get("employee", "Tyler", "salary"))
 ```
 
-or terminal:
 ```
-cabinet -g employee Tyler salary
+> python3 test.py
+> 7.25
 ```
 
-results in:
-```
-7.25
-```
-
-### `edit_file`
+### `edit`
 
-python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
 
-# if put("path", "edit", "shopping", "/path/to/shopping.md") has been called, this will edit the file assigned to that shortcut.
+# if set("path", "edit", "shopping", "/path/to/shopping.md") has been called, this will edit the file assigned to that shortcut.
 
 # opens file in Vim, saves upon exit
 cab.edit("shopping")
 
 # or you can edit a file directly...
 cab.edit("/path/to/shopping.md")
 ```
 
-terminal:
-```
-# assumes path -> edit -> shopping -> path/to/shopping.md has been set
-cabinet -ef shoppping
-
-or 
-
-cabinet -ef "/path/to/shopping.md"
-```
-
 ### `mail`
 
-python:
 ```
 
-from cabinet import Mail
-
-mail = Mail()
+from cabinet import mail
 
 mail.send('Test Subject', 'Test Body')
 
 ```
 
-terminal:
-```
-cabinet --mail --subject "Test Subject" --body "Test Body"
-
-# or
-
-cabinet --mail -s "Test Subject" -b "Test Body"
-```
-
 ### `log`
 
-python:
 ```
+
 from cabinet import Cabinet
 
 cab = Cabinet()
 
 # writes to a file named LOG_DAILY_YYYY-MM-DD in the default log folder (or cab.get('path', 'log')) inside a YYYY-MM-DD folder
 
 cab.log("Connection timed out") # defaults to 'info' if no level is set
@@ -248,34 +169,26 @@
 cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
-terminal:
-```
-# defaults to 'info' if no level is set
-cab -l "Connection timed out" 
-
-# -l and --log are interchangeable
-cab --log "Connection timed out"
-
-# change levels with --level
-cab --log "Server is on fire" --level "critical"
-```
-
 ## Dependencies
 
 - Python >= 3.6
 - smtplib
 
 ## Disclaimers
 
 - Although I've done quite a bit of testing, I can't guarantee everything that works on my machine will work on yours. Always back up your data to multiple places to avoid data loss.
 - If you find any issues, please contact me... or get your hands dirty and raise a PR!
 
+```
+
+```
+
 ## Author
 
 - Tyler Woodfin
   - [GitHub](https://www.github.com/tylerjwoodfin)
   - [Website](http://tyler.cloud)
```

### Comparing `cabinet-2023.4.30.1/README.md` & `cabinet-2023.4.9.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,23 @@
+Metadata-Version: 2.1
+Name: cabinet
+Version: 2023.4.9.1
+Summary: Easily manage data storage and logging across repos
+Home-page: https://github.com/tylerjwoodfin/cabinet
+Author: Tyler Woodfin
+Author-email: feedback@tyler.cloud
+License: : OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # cabinet
 A Python library to easily store data across multiple projects in one or more JSON files.
 
-Supports a cli, email, and event logging.
+Supports email and event logging.
 
 ## Features
 
 - Read and write data in the JSON files of your choice
 - Log to a file/directory of your choice without having to configure `logger` each time
 - Send/receive mail using `cabinet.Cabinet().mail()`
 
@@ -16,210 +28,131 @@
   - this can be changed on a per-log basis
 
 ## Installation and Setup
 
 ```bash
   python3 -m pip install cabinet
 
-  cabinet --config
-```
-
-## CLI usage
-```
-Usage: cabinet [OPTIONS]
-
-Options:
-  -h, --help              Show this help message and exit
-  --configure, -config    Configure
-  --edit, -e              Edit the settings.json file
-  --edit-file, -ef        Edit a specific file
-  --no-create             (for -ef) Do not create file if it does not exist
-  --get, -g [GET ...]     Get a property from settings.json
-  --put PUT [PUT ...]     Put a property into settings.json
-  --get-file GET_FILE     Get file
-  --strip                 (for --get-file) Whether to strip file content whitespace
-  --log, -l               Log a message to the default location
-  --level LOG_LEVEL       (for -l) Log level [debug, info, warn, error, critical]
-  -v, --version           show version number and exit
-
-Mail:
-  --mail                Sends an email
-  --subject SUBJECT, -s SUBJECT
-                        Email subject
-  --body BODY, -b BODY  Email body
-  --to TO_ADDR, -t TO_ADDR
+  cabinet config
 ```
 
 ## Configuration
 
-- Upon first launch, will prompt you to choose a location for `settings.json`. You can change this at any time with `cabinet --config`.
+- Upon first launch, will prompt you to choose a location for `settings.json`. You can change this at any time with `cabinet config`.
 
-### edit_file() shortcuts
-- see example below to enable something like
-  - `cabinet -ef shopping` from the terminal
-    - rather than `cabinet -ef "/home/{username}/path/to/shopping_list.md"`
-  - or `cabinet.Cabinet().edit("shopping")`
-    - rather than `cabinet.Cabinet().edit("/home/{username}/path/to/whatever.md")`
+### edit() shortcuts
+- see example below to enable something like `cabinet edit shopping` from the terminal
+  - or `cabinet.Cabinet().edit("shopping")`, rather than `cabinet.Cabinet().edit("/home/{username}/path/to/shopping.md")`
 
-file:
 ```
 # example only; these commands will be unique to your setup
 
 {
   "path": {
     "edit": {
       "shopping": {
-        "value": "/home/{username}/path/to/whatever.md",
+        "value": "/home/{username}/path/to/shopping.md",
       },
       "todo": {
-        "value": "/home/{username}/path/to/whatever.md",
+        "value": "/home/{username}/path/to/todo.md",
       }
     }
   }
 }
 ```
 
-set from terminal:
-```
-cabinet -p edit shopping value "/home/{username}/path/to/whatever.md"
-cabinet -p edit todo value "/home/{username}/path/to/whatever.md"
-```
-
 ### mail
 
 - It is NEVER a good idea to store your password in plaintext; for this reason, I strongly recommend a "throwaway" account that is only used for sending emails
 - Gmail (as of May 2022) and most other mainstream email providers won't work with this; for support, search for sending mail from your email provider with `smtplib`.
 - In `settings.json`, add the `email` object to make your settings file look like this example:
 
-file:
 ```
 {
     "email": {
         "from": "throwaway@example.com",
         "from_pw": "example",
         "from_name": "Raspberry Pi",
         "to": "destination@protonmail.com",
         "smtp_server": "example.com",
         "imap_server": "example.com",
         "port": 123
     }
 }
 ```
 
-set from terminal:
-```
-cabinet -p email from throwaway@example.com
-cabinet -p email from_pw example
-...
-```
-
 ## Examples
 
-### `put`
+### `set`
 
-python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
 
-cab.put("employee", "Tyler", "salary", 7.25)
-```
-
-or terminal:
-```
-# warning - from the terminal, numeric values in cabinet are stored as strings
-cabinet -p employer Tyler salary 7.25
+cab.set("employee", "Tyler", "salary", 7.25)
 ```
 
 results in this structure in settings.json:
+
 ```
 {
     "employee": {
         "Tyler": {
-            "salary": 7.25 # or "7.25" if done from terminal
+            "salary": 7.25
         }
     }
 }
 ```
 
 ### `get`
 
-python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
 
 print(cab.get("employee", "Tyler", "salary"))
 ```
 
-or terminal:
 ```
-cabinet -g employee Tyler salary
+> python3 test.py
+> 7.25
 ```
 
-results in:
-```
-7.25
-```
-
-### `edit_file`
+### `edit`
 
-python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
 
-# if put("path", "edit", "shopping", "/path/to/shopping.md") has been called, this will edit the file assigned to that shortcut.
+# if set("path", "edit", "shopping", "/path/to/shopping.md") has been called, this will edit the file assigned to that shortcut.
 
 # opens file in Vim, saves upon exit
 cab.edit("shopping")
 
 # or you can edit a file directly...
 cab.edit("/path/to/shopping.md")
 ```
 
-terminal:
-```
-# assumes path -> edit -> shopping -> path/to/shopping.md has been set
-cabinet -ef shoppping
-
-or 
-
-cabinet -ef "/path/to/shopping.md"
-```
-
 ### `mail`
 
-python:
 ```
 
-from cabinet import Mail
-
-mail = Mail()
+from cabinet import mail
 
 mail.send('Test Subject', 'Test Body')
 
 ```
 
-terminal:
-```
-cabinet --mail --subject "Test Subject" --body "Test Body"
-
-# or
-
-cabinet --mail -s "Test Subject" -b "Test Body"
-```
-
 ### `log`
 
-python:
 ```
+
 from cabinet import Cabinet
 
 cab = Cabinet()
 
 # writes to a file named LOG_DAILY_YYYY-MM-DD in the default log folder (or cab.get('path', 'log')) inside a YYYY-MM-DD folder
 
 cab.log("Connection timed out") # defaults to 'info' if no level is set
@@ -236,34 +169,26 @@
 cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
-terminal:
-```
-# defaults to 'info' if no level is set
-cab -l "Connection timed out" 
-
-# -l and --log are interchangeable
-cab --log "Connection timed out"
-
-# change levels with --level
-cab --log "Server is on fire" --level "critical"
-```
-
 ## Dependencies
 
 - Python >= 3.6
 - smtplib
 
 ## Disclaimers
 
 - Although I've done quite a bit of testing, I can't guarantee everything that works on my machine will work on yours. Always back up your data to multiple places to avoid data loss.
 - If you find any issues, please contact me... or get your hands dirty and raise a PR!
 
+```
+
+```
+
 ## Author
 
 - Tyler Woodfin
   - [GitHub](https://www.github.com/tylerjwoodfin)
   - [Website](http://tyler.cloud)
```

### Comparing `cabinet-2023.4.30.1/setup.cfg` & `cabinet-2023.4.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cabinet
-version = 2023.04.30.1
+version = 2023.04.09.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls =
```

### Comparing `cabinet-2023.4.30.1/src/cabinet/__init__.py` & `cabinet-2023.4.9.1/src/cabinet/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Cabinet provides a simple interface for storing and retrieving data in a centralized location.
+Cabinet provides a simple interface for storing and retrieving data in a centralized location. 
 
 It includes a variety of utility methods for managing files, logging, and managing configurations.
 
 Usage:
     ```
     from cabinet import Cabinet
 
@@ -12,41 +12,28 @@
 """
 
 import os
 import json
 import pathlib
 import logging
 import sys
-import argparse
 from datetime import date
 from typing import Optional
-import importlib.metadata
-from .mail import Mail
 
 
 class Cabinet:
     """
     The main class for Cabinet
     """
 
     path_cabinet: str = None
     path_config_file: str = None
     path_settings_file: str = None
     path_log: str = None
     settings_json = None
-    new_setup: bool = False
-
-    NEW_SETUP_MSG = (
-        "Welcome to Cabinet!\n\n"
-        "Enter the directory to store the default settings.json.\n"
-        "This should be an absolute path in a public place, like "
-        f"{pathlib.Path.home().resolve()}/cabinet.\n\n"
-        "Don't worry, this won't overwrite anything in this folder.\n"
-        "By continuing, a new configuration file will be created in your site-packages folder.\n\n"
-    )
 
     def __init__(self, path_cabinet: str = None):
         """
         The main module for file management
 
         Args:
             - path_cabinet (str, optional): the directory of a settings.json file to be used
@@ -62,56 +49,52 @@
             ```
         """
 
         # config file, stored within the package
         self.path_config_file = pathlib.Path(
             __file__).resolve().parent / "config.json"
 
-        # determines where settings.json is stored; by default, this is ~/cabinet
+        # Determines where settings.json is stored; by default, this is ~/cabinet
         self.path_cabinet = os.path.expanduser(
             self._get_config('path_cabinet'))
 
         path_cabinet = path_cabinet or self.path_cabinet
 
-        # new setup
         if path_cabinet is None:
-            self.new_setup = True
-            path_cabinet = input(self.NEW_SETUP_MSG)
+            path_cabinet = input(
+                "Enter the directory to store settings.json: ")
             if not path_cabinet:
                 path_cabinet = str(pathlib.Path.home() / "cabinet")
 
         self.path_settings_file = pathlib.Path(path_cabinet) / "settings.json"
 
         try:
             with open(f'{path_cabinet}/settings.json', 'r+', encoding="utf8") as file:
                 file.seek(0, os.SEEK_END)
-        except FileNotFoundError:
+        except FileNotFoundError as error:
             # initialize settings file if it doesn't exist
             if not os.path.exists(path_cabinet):
                 os.makedirs(path_cabinet)
             with open(f'{path_cabinet}/settings.json', 'x+', encoding="utf8") as file:
-                new_file_msg = ("\n\nWarning: settings.json not found; "
-                                f"created a blank one in {path_cabinet}")
-                self._ifprint(new_file_msg,
-                              self.new_setup is False)
-                self._ifprint("You can change this location by calling 'cabinet config'.\n\n",
-                              self.new_setup is False)
+                print(f"\n\nWarning: settings.json not found; \
+                    created a blank one in {path_cabinet} ({error})")
+                print("You can change this location by calling 'cabinet config'.\n\n")
                 file.write('{}')
 
         try:
             self.settings_json = json.load(
                 open(f'{path_cabinet}/settings.json', encoding="utf8"))
 
         except json.decoder.JSONDecodeError as error:
             print(f"{error}\n")
 
-            response = input(f"The settings file ({path_cabinet}/settings.json) is not valid JSON. "
-                             "Do you want to replace it with an empty JSON file? "
-                             f"(The existing file will be backed up in {path_cabinet}) (y/n)\n")
-
+            response = input(
+                f"The settings file ({path_cabinet}/settings.json) is not valid JSON. \
+                    Do you want to replace it with an empty JSON file? \
+                        (The existing file will be backed up in {path_cabinet}) (y/n)\n")
             if response.lower().startswith("y"):
                 print("Backing up...")
 
                 # for some reason, this only works when you call touch; TODO fix this
                 os.system(
                     f"touch {path_cabinet}/settings-backup.json \
                         && cp {path_cabinet}/settings.json {path_cabinet}/settings-backup.json")
@@ -126,65 +109,65 @@
             sys.exit(-1)
 
         path_log = self.get('path', 'log')
 
         if path_log is None:
             path_log = self.put(
                 'path', 'log', f"{path_cabinet}/log", file_name='settings.json')
-            print(
-                f"\nCalling cabinet.log in Python (or 'cabinet --log' in the terminal) "
-                f"will write to {path_cabinet}/log by default.\n"
-                f"You can change this in {path_cabinet}/settings.json.\n\n"
-            )
+            print(f"""
+                \n\nCalling cabinet.log in Python will now write to {path_cabinet}/log by default.
+                """)
+            print(f"You can change this in {path_cabinet}/settings.json.\n\n")
         if not os.path.exists(path_log):
             os.makedirs(path_log)
         if not path_log[-1] == '/':
             path_log += '/'
 
         self.path_log = path_log
-        self.new_setup = False
 
     def _get_config(self, key=None):
         """
         Gets a property from the internal configuration file.
 
         Args:
         - key (str): The key to search for in the JSON file.
 
         Returns:
         - The value of the key in the JSON file.
 
-        If the JSON file does not exist or is not valid JSON,
+        If the JSON file does not exist or is not valid JSON, 
             the function provides default behavior:
         - If `key` is `path_cabinet`, the function prompts
             the user to enter a directory to store settings.json.
         - If `key` is not found, the function returns an empty string.
         - If the file is not valid JSON, the function prompts
             the user to replace the file with an empty JSON file.
         """
 
         try:
             with open(self.path_config_file, 'r+', encoding="utf8") as file:
                 return json.load(file)[key]
         except FileNotFoundError:
             if key == 'path_cabinet':
-                # setup
-                self.new_setup = True
-                path_cabinet = input(self.NEW_SETUP_MSG)
+                # set default settings.json and log path to ~/cabinet
+                path_cabinet_msg = """Enter the directory to store settings.json.\n"""\
+                    f"""This should be a public place, """\
+                    f"""such as {pathlib.Path.home().resolve()}/cabinet.\n\n"""
+
+                path_cabinet = input(path_cabinet_msg)
 
                 self._put_config(key, path_cabinet)
                 return path_cabinet
         except KeyError:
             print(f"Warning: Key error for key: {key}")
             return ""
         except json.decoder.JSONDecodeError:
             response = input(
-                f"The config file ({self.path_config_file}) is not valid JSON.\n"
-                "Do you want to replace it with an empty JSON file? "
-                "(you will lose existing data) (y/n)\n")
+                f"The config file ({self.path_config_file}) is not valid JSON. Do you want to \
+                    replace it with an empty JSON file?  (you will lose existing data) (y/n)\n")
             if response.lower().startswith("y"):
                 with open(self.path_config_file, 'w+', encoding="utf8") as file:
                     file.write('{}')
                 print("Done. Please try your last command again.")
             else:
                 print(f"OK. Please fix {self.path_config_file} and try again.")
 
@@ -214,45 +197,37 @@
             if key == 'path_cabinet' and value[0] != '/' and value[0] != '~':
                 value = f"/{value}"
             if key == 'path_cabinet' and value[-1] == '/':
                 value = f"{value[:-1]}"
 
             # warn about potential problems
             if not os.path.exists(os.path.expanduser(value)):
-                print(f"Warning: {value} doesn't exist.")
-                create_dir = input(
-                    "Do you want to create the directory? (y/n): ")
-                if create_dir.lower().startswith("y"):
-                    os.makedirs(os.path.expanduser(value))
-                    print("Done.")
-                else:
-                    print("OK, but if you run into problems, "
-                          "run 'cabinet --config' to change to an existing directory.")
+                print(f"Warning: {value} is not a valid path.")
             if value[0] == '~':
-                print("Warning: using tilde expansions may cause problems ",
-                      "if using cabinet for multiple users. It is recommended to use full paths.""")
+                print("""
+Warning: using tilde expansions may cause problems
+if using cabinet for multiple users. It is recommended to use full paths.""")
 
         try:
             with open(self.path_config_file, 'r+', encoding="utf8") as file:
                 config = json.load(file)
         except FileNotFoundError:
             with open(self.path_config_file, 'x+', encoding="utf8") as file:
-                self._ifprint(
-                    "Note: Could not find an existing config file; creating a new one.",
-                    self.new_setup is False)
+                print(
+                    "Note: Could not find an existing config file; creating a new one.")
                 file.write('{}')
                 config = {}
 
         config[key] = value
 
         with open(self.path_config_file, 'w+', encoding="utf8") as file:
             json.dump(config, file, indent=4)
 
         print(f"\n\nUpdated configuration file ({self.path_config_file}).")
-        self._ifprint(f"{key} is now {value}\n", self.new_setup is False)
+        print(f"{key} is now {value}\n")
 
         return value
 
     def _get_logger(self, log_name: str = None, level: int = logging.INFO,
                     file_path: str = None, is_quiet: bool = False) -> logging.Logger:
         """
         A helper function for log()
@@ -270,21 +245,21 @@
         Returns:
         - logger (Logger): the configured logger object
         """
 
         today = str(date.today())
 
         if file_path is None:
-            file_path = f"{self.path_log or self.path_cabinet + '/log/'}{today}"
+            file_path = f"{self.path_log}{today}"
         if log_name is None:
             log_name = f"LOG_DAILY_{today}"
 
         # create path if necessary
         if not os.path.exists(file_path):
-            self._ifprint(f"Creating {file_path}", self.new_setup is True)
+            print(f"Creating {file_path}")
             os.makedirs(file_path)
 
         logger = logging.getLogger(log_name)
 
         logger.setLevel(level)
 
         if logger.handlers:
@@ -301,44 +276,31 @@
         file_handler = logging.FileHandler(
             f"{file_path}/{log_name}.log", mode='a')
         file_handler.setFormatter(log_format)
 
         logger.addHandler(file_handler)
         return logger
 
-    def _ifprint(self, message: str, is_print: bool):
-        """
-        Prints a string if `print` is true.
-        """
-        if is_print:
-            print(message)
-
     def configure(self):
         """
         Configures the Cabinet instance based on command line arguments or user input.
         """
 
         message = f"""
-Enter the full path of the directory where you want to store
+Enter the full path of the directory where you want to store 
 all data (currently {self.path_cabinet}):\n"""
 
         self._put_config('path_cabinet', input(message))
 
-    def edit(self):
-        """
-        Edits and saves the settings file.
-        """
-        self.edit_file(self.path_settings_file)
-
     def edit_file(self, file_path: str = None, create_if_not_exist: bool = True) -> None:
         """
-        Edit and save a file in Vim.
+        Edit and save a file using Vim.
 
         Args:
-            - file_path (str, optional): The path to the file to edit.
+            - file_path (str, optional): The path to the file to edit. 
                 Allows for shortcuts by setting paths in settings.json -> path -> edit
                 If unset, edit settings.json
 
             - create_if_not_exist (bool, optional): Whether to create the file if it does not exist.
                 Defaults to False.
 
         Raises:
@@ -348,18 +310,17 @@
 
         Returns:
             None
         """
 
         # edit settings.json if no file_path
         if file_path is None:
-            message = (
-                "Enter the path of the file you want to edit "
-                f"(default: {self.path_cabinet}/settings.json):\n"
-            )
+            message = f"""
+Enter the path of the file you want to edit
+(default: {self.path_cabinet}/settings.json):\n"""
 
             path = self.path_settings_file or input(
                 message) or f"{self.path_cabinet}/settings.json"
             self.edit_file(path)
             return
 
         # allows for shortcuts by setting paths in settings.json -> path -> edit
@@ -387,15 +348,15 @@
 
         with open(file_path, "r", encoding="utf-8") as file:
             new_contents = file.readlines()
 
         if original_contents == new_contents:
             print("No changes.")
 
-    def get(self, *attributes, warn_missing=False, is_print=False):
+    def get(self, *attributes, warn_missing=False):
         """
         Returns a property in a JSON file based on the input attributes.
 
         Args:
             - attributes (str): the attributes to traverse in the JSON file
             - warn_missing (bool, optional): whether to warn if an attribute is missing
 
@@ -403,36 +364,32 @@
             - The value of the attribute if it exists in the JSON file, otherwise default.
 
         Usage:
             - get('person', 'tyler', 'salary') returns person -> tyler -> salary from self.settings
         """
 
         if self.settings_json is None:
-            self._ifprint("None", is_print)
             return None
 
         settings = self.settings_json
 
         for index, item in enumerate(attributes):
             if item in settings:
                 settings = settings[item]
             elif warn_missing and (len(attributes) < 2 or attributes[1] != "edit"):
-                is_print(
+                print(
                     f"Warning: {item} not found in \
                         {settings if index > 0 else f'{self.path_cabinet}/settings.json'}")
-                self._ifprint("None", is_print)
                 return None
             else:
-                self._ifprint("None", is_print)
                 return None
 
-        self._ifprint(settings, is_print)
         return settings
 
-    def put(self, *attribute, value=None, file_name='settings.json', is_print=False):
+    def put(self, *attribute, value=None, file_name='settings.json'):
         """
         Adds or replaces a property in a JSON file (default name: settings.json).
 
         Args:
             *attribute (str): A series of keys in the JSON object
                 to identify the location of the property.
             value (optional): The value to put into the property.
@@ -450,42 +407,33 @@
 
         _settings = self.settings_json if file_name == 'settings.json' else json.load(
             open(path_full, encoding="utf8"))
 
         # iterate through entire JSON object and replace 2nd to last attribute with value
 
         partition = _settings
-
         for index, item in enumerate(attribute[:-1]):
             if item not in partition:
-                try:
-                    partition[item] = value if index == len(
-                        attribute) - 2 else {}
-                    partition = partition[item]
-                    self.log(
-                        f"Adding new key '{item}' to {partition if index > 0 else path_full}",
-                        is_quiet=self.new_setup)
-                except TypeError as error:
-                    self.log(f"{error}\n\n{attribute[index-1]} is currently a string, so it cannot \
-be treated as an object with multiple properties.", level="error")
+                partition[item] = value if index == len(attribute) - 2 else {}
+                partition = partition[item]
+                print(
+                    f"Warning: Adding new key '{item}' to {partition if index > 0 else path_full}")
             else:
                 if index == len(attribute) - 2:
                     partition[item] = value
                 else:
                     partition = partition[item]
 
         with open(path_full, 'w+', encoding="utf8") as file:
             json.dump(_settings, file, indent=4)
 
-        self._ifprint(
-            f"{' -> '.join(attribute[:-1])} set to {value}", is_print)
         return value
 
     def get_file_as_array(self, item: str, file_path=None, strip: bool = True,
-                          ignore_not_found: bool = False):
+                          ignore_not_found: bool = False) -> list[str]:
         """
         Reads a file and returns its contents as a list of lines.
         The file is assumed to be encoded in UTF-8.
 
         Args:
             - item (str): The filename to read.
             - file_path (str, optional): The path to the directory containing the file.
@@ -552,41 +500,38 @@
             if not is_quiet:
                 print(f"Wrote to '{file_path}/{file_name}'")
             return True
         except (OSError, IOError) as error:
             self.log(f"write_file: {error}", level="error")
             return False
 
-    def log(self, message: str = '', log_name: str = None, level: str = None,
+    def log(self, message: str = '', log_name: str = None, level: str = 'info',
             file_path: str = None, is_quiet: bool = False) -> None:
         """
         Logs a message using the specified log level
         and writes it to a file if a file path is provided.
 
         Args:
             message (str, optional): The message to log. Defaults to ''.
             log_name (str, optional): The name of the logger to use. Defaults to None.
-            level (str, optional): The log level to use.
+            level (str, optional): The log level to use. 
                 Must be one of 'debug', 'info', 'warning', 'error', or 'critical'.
                 Defaults to 'info'.
-            file_path (str, optional): The path to the log file.
+            file_path (str, optional): The path to the log file. 
                 If not provided, logs will be saved to settings.json -> path -> log.
                 Defaults to None.
             is_quiet (bool, optional): If True, logging output will be silenced. Defaults to False.
 
         Raises:
             ValueError: If an invalid log level is provided.
 
         Returns:
             None
         """
 
-        if level is None:
-            level = 'info'
-
         # validate log level
         valid_levels = {'debug', 'info', 'warn',
                         'warning', 'error', 'critical'}
         if level.lower() not in valid_levels:
             raise ValueError(
                 f"Invalid log level: {level}. Must be one of {', '.join(valid_levels)}.")
 
@@ -611,77 +556,21 @@
 
     Usage:
         (from the terminal)
         cabinet config
         cabinet edit <file path/name, optional; default: settings.json>
     """
 
-    cab = Cabinet()
-    package_name = sys.modules[__name__].__package__.split('.')[0]
-    version = importlib.metadata.version(package_name)
-
-    parser = argparse.ArgumentParser(
-        description=f"Cabinet ({version})")
-
-    parser.add_argument('--configure', '-config', dest='configure',
-                        action='store_true', help='Configure')
-    parser.add_argument('--edit', '-e', dest='edit', action='store_true',
-                        help='Edit the settings.json file')
-    parser.add_argument('--edit-file', '-ef', type=str, dest='edit_file',
-                        help='Edit a specific file')
-    parser.add_argument('--no-create', dest='create',
-                        action='store_false',
-                        help='(for -ef) Do not create file if it does not exist')
-    parser.add_argument('--get', '-g', dest='get', nargs='+',
-                        help='Get a property from settings.json')
-    parser.add_argument('--put', '-p', dest='put', nargs='+',
-                        help='Put a property into settings.json')
-    parser.add_argument('--get-file', dest='get_file',
-                        type=str, help='Get file')
-    parser.add_argument('--strip', dest='strip', action='store_false',
-                        help='(for --get-file) Whether to strip file content whitespace')
-    parser.add_argument('--log', '-l', type=str,
-                        dest='log', help='Log a message to the default location')
-    parser.add_argument('--level', type=str, dest='log_level',
-                        help='(for -l) Log level [debug, info, warn, error, critical]')
-
-    mail_group = parser.add_argument_group('Mail')
-    mail_group.add_argument(
-        '--mail', dest='mail', action='store_true', help='Sends an email')
-    mail_group.add_argument(
-        '--subject', '-s', dest='subject', required='--mail' in sys.argv, help='Email subject')
-    mail_group.add_argument(
-        '--body', '-b', dest='body', required='--mail' in sys.argv, help='Email body')
-    mail_group.add_argument('--to', '-t', dest='to_addr',
-                            help='The "to" email address')
-
-    parser.add_argument('-v', '--version',
-                        action='version', help='Show version number and exit', version=version)
-
-    args = parser.parse_args()
-
-    if args.configure:
-        cab.configure()
-    elif args.edit:
-        cab.edit()
-    elif args.edit_file:
-        cab.edit_file(file_path=args.edit_file,
-                      create_if_not_exist=args.create)
-    elif args.get:
-        cab.get(is_print=True, *args.get)
-    elif args.put:
-        attribute_values = args.put
-        cab.put(*attribute_values, is_print=True)
-    elif args.get_file:
-        cab.get_file_as_array(item=args.get_file,
-                              file_path=None, strip=args.strip)
-    elif args.log:
-        cab.log(message=args.log, level=args.log_level)
-    elif args.mail:
-        to_addr = None
-        if args.to_addr:
-            to_addr = ''.join(args.to_addr).split(',')
-        Mail().send(args.subject, args.body, to_addr=to_addr)
+    if len(sys.argv) < 2:
+        print("Cabinet is not intended to be directly run. See README.md.")
+        sys.exit(0)
+
+    if "cabinet" in sys.argv[0] and len(sys.argv) > 1:
+        if "config" == sys.argv[1]:
+            Cabinet().configure()
+        elif "edit" == sys.argv[1]:
+            path = None if len(sys.argv) < 3 else sys.argv[2]
+            Cabinet().edit_file(path)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cabinet-2023.4.30.1/src/cabinet/mail.py` & `cabinet-2023.4.9.1/src/cabinet/mail.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,97 +11,78 @@
 from typing import List
 from urllib.parse import unquote
 import sys
 import pwd
 import os
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
-import cabinet
+from cabinet import Cabinet
 
-class Mail:
+cab = Cabinet()
+
+userDir = pwd.getpwuid(os.getuid())[0]
+
+# parameters
+port = cab.get("email", "port")
+smtp_server = cab.get("email", "smtp_server")
+imap_server = cab.get("email", "imap_server")
+username = cab.get("email", "from")
+password = cab.get("email", "from_pw")
+
+
+def send(subject: str, body: str, signature: str = '', to_addr: List[str] = None,
+         from_name: str = None, logging_enabled: bool = True, is_quiet: bool = False) -> None:
     """
-    Provides functionality for sending email using SMTP and MIMEText.
-    Does not support Gmail.
-    A throwaway email is highly recommended.
+    Sends an email with the given subject and body to the specified recipients.
+
+    Args:
+    - subject (str): The subject of the email.
+    - body (str): The body of the email.
+    - signature (str): The signature to include at the end of the email.
+    - to_addr (List): A list of email addresses to send the email to.
+    - from_name (str, optional): The name to appear in the "From" field of the email.
+        Reads from settings.json -> email -> from_name if unset.
+        If this is unset, defaults to `Raspberry Pi`
+    - logging_enabled (bool, optional): Whether to log the email send event.
+        Defaults to True.
+    - is_quiet: Whether to suppress log output.
+        Defaults to False.
+
+    Gmail will almost certainly not work.
     """
 
-    def __init__(self):
-        self.user_dir = pwd.getpwuid(os.getuid())[0]
-        self.cab = cabinet.Cabinet()
-
-        # parameters
-        self.port = self.cab.get("email", "port")
-        self.smtp_server = self.cab.get("email", "smtp_server")
-        self.imap_server = self.cab.get("email", "imap_server")
-        self.username = self.cab.get("email", "from")
-        self.password = self.cab.get("email", "from_pw")
-
-    def send(self, subject: str, body: str, signature: str = '', to_addr: List[str] = None,
-             from_name: str = None, logging_enabled: bool = True, is_quiet: bool = False) -> None:
-        """
-        Sends an email with the given subject and body to the specified recipients.
-
-        Args:
-        - subject (str): The subject of the email.
-        - body (str): The body of the email.
-        - signature (str): The signature to include at the end of the email.
-        - to_addr (List): A list of email addresses to send the email to.
-        - from_name (str, optional): The name to appear in the "From" field of the email.
-            Reads from settings.json -> email -> from_name if unset.
-            If this is unset, defaults to `Raspberry Pi`
-        - logging_enabled (bool, optional): Whether to log the email send event.
-            Defaults to True.
-        - is_quiet: Whether to suppress log output.
-            Defaults to False.
-
-        Raises:
-        - smtplib.SMTPAuthenticationError: If the SMTP server rejects the login credentials.
-
-        Gmail will almost certainly not work.
-        """
-
-        # Set default `from_name` if unset.
-        if from_name is None:
-            from_name = (self.cab.get("email", "from_name")
-                         or "Raspberry Pi") + f" <{self.username}>"
+    from_name = (cab.get("email", "from_name") or "Raspberry Pi") + f" <{username}>"
+    signature = signature or f"<br><br>Thanks,<br>{from_name}"
 
-        # Set default `to_addr` if unset.
-        if to_addr is None:
-            to_addr = self.cab.get("email", "to")
+    if to_addr is None:
+        to_addr = cab.get("email", "to")
 
-            if to_addr is None:
-                self.cab.log("cabinet -> email -> to is unset", level="error")
-                return
-
-        # Append `signature` to the `body` of the email.
-        signature = signature or f"<br><br>Thanks,<br>{from_name}"
-        body += unquote(signature)
-
-        # Create the message object.
-        message = MIMEMultipart()
-        message["Subject"] = unquote(subject)
-        message["From"] = from_name
-        message["To"] = (', ').join(to_addr)
-        message.attach(MIMEText(unquote(body), "html"))
-
-        # Send the email.
-        server = smtplib.SMTP_SSL(self.smtp_server, self.port)
-
-        try:
-            server.login(self.username, self.password)
-
-            server.send_message(message)
-
-            if logging_enabled:
-                self.cab.log(
-                    f"Sent Email to {message['To']} as {message['From']}: {subject}",
-                    is_quiet=is_quiet)
-
-        except smtplib.SMTPAuthenticationError as err:
-            self.cab.log(
-                f"Could not log into {self.username}; set this with Cabinet.\n\n{err}",
-                level="error")
+        if to_addr is None:
+            cab.log("cabinet -> email -> to is unset", level="error")
+            return
 
+    # Parse
+    body += unquote(signature)
+    message = MIMEMultipart()
+    message["Subject"] = unquote(subject)
+    message["From"] = from_name
+    message["To"] = (', ').join(to_addr)
+    message.attach(MIMEText(unquote(body), "html"))
+
+    # Send Email
+    server = smtplib.SMTP_SSL(smtp_server, port)
+
+    try:
+        server.login(username, password)
+        server.send_message(message)
+
+        if logging_enabled:
+            cab.log(
+                f"Sent Email to {message['To']} as {message['From']}: {subject}", is_quiet=is_quiet)
+
+    except smtplib.SMTPAuthenticationError as err:
+        cab.log(
+            f"Could not log into {username}; set this with Cabinet.\n\n{err}", level="error")
 
 if __name__ == "__main__":
     if len(sys.argv) == 1:
-        print("Usage: cabinet --mail -s <subject> -b <body> --to <to, optional>")
+        print("sys.argv usage: send <subject>, <body>")
```

