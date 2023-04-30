# Comparing `tmp/QATLibrary-23.5.2.tar.gz` & `tmp/QATLibrary-23.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QATLibrary-23.5.2.tar", last modified: Sat Apr 29 07:23:24 2023, max compression
+gzip compressed data, was "QATLibrary-23.5.3.tar", last modified: Sun Apr 30 19:33:28 2023, max compression
```

## Comparing `QATLibrary-23.5.2.tar` & `QATLibrary-23.5.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 07:23:24.094325 QATLibrary-23.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-29 07:23:02.000000 QATLibrary-23.5.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-29 07:23:24.094325 QATLibrary-23.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-04-29 07:23:02.000000 QATLibrary-23.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-29 07:23:24.098325 QATLibrary-23.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 07:23:02.000000 QATLibrary-23.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 07:23:24.094325 QATLibrary-23.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 07:23:24.094325 QATLibrary-23.5.2/src/QATLibrary/
--rw-r--r--   0 runner    (1001) docker     (123)    16601 2023-04-29 07:23:02.000000 QATLibrary-23.5.2/src/QATLibrary/QATLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-29 07:23:02.000000 QATLibrary-23.5.2/src/QATLibrary/TLSAdapter.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-29 07:23:02.000000 QATLibrary-23.5.2/src/QATLibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-29 07:23:02.000000 QATLibrary-23.5.2/src/QATLibrary/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-29 07:23:02.000000 QATLibrary-23.5.2/src/QATLibrary/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-29 07:23:02.000000 QATLibrary-23.5.2/src/QATLibrary/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 07:23:24.094325 QATLibrary-23.5.2/src/QATLibrary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-29 07:23:24.000000 QATLibrary-23.5.2/src/QATLibrary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-29 07:23:24.000000 QATLibrary-23.5.2/src/QATLibrary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 07:23:24.000000 QATLibrary-23.5.2/src/QATLibrary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-29 07:23:24.000000 QATLibrary-23.5.2/src/QATLibrary.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 07:23:24.000000 QATLibrary-23.5.2/src/QATLibrary.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-29 07:23:24.000000 QATLibrary-23.5.2/src/QATLibrary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 07:23:24.000000 QATLibrary-23.5.2/src/QATLibrary.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:33:28.566028 QATLibrary-23.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-30 19:33:11.000000 QATLibrary-23.5.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-04-30 19:33:28.566028 QATLibrary-23.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-04-30 19:33:11.000000 QATLibrary-23.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-30 19:33:28.566028 QATLibrary-23.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 19:33:11.000000 QATLibrary-23.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:33:28.566028 QATLibrary-23.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:33:28.566028 QATLibrary-23.5.3/src/QATLibrary/
+-rw-r--r--   0 runner    (1001) docker     (123)    16611 2023-04-30 19:33:11.000000 QATLibrary-23.5.3/src/QATLibrary/QATLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-30 19:33:11.000000 QATLibrary-23.5.3/src/QATLibrary/TLSAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-30 19:33:11.000000 QATLibrary-23.5.3/src/QATLibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-30 19:33:11.000000 QATLibrary-23.5.3/src/QATLibrary/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-30 19:33:11.000000 QATLibrary-23.5.3/src/QATLibrary/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-30 19:33:11.000000 QATLibrary-23.5.3/src/QATLibrary/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:33:28.566028 QATLibrary-23.5.3/src/QATLibrary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-04-30 19:33:28.000000 QATLibrary-23.5.3/src/QATLibrary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-30 19:33:28.000000 QATLibrary-23.5.3/src/QATLibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 19:33:28.000000 QATLibrary-23.5.3/src/QATLibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-30 19:33:28.000000 QATLibrary-23.5.3/src/QATLibrary.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 19:33:28.000000 QATLibrary-23.5.3/src/QATLibrary.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-30 19:33:28.000000 QATLibrary-23.5.3/src/QATLibrary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 19:33:28.000000 QATLibrary-23.5.3/src/QATLibrary.egg-info/top_level.txt
```

### Comparing `QATLibrary-23.5.2/LICENSE.md` & `QATLibrary-23.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `QATLibrary-23.5.2/PKG-INFO` & `QATLibrary-23.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QATLibrary
-Version: 23.5.2
+Version: 23.5.3
 Summary: Data/Configuration Driven REST API Test Automation Library. Can be used as a Robot Framework Library or as standalone CLI tool.
 Home-page: https://github.com/toil-free/QATLibrary.git
 Author: Sharif Rahman
 Author-email: shrif.sbu@gmail.com
 License: MIT
 Project-URL: Docs, https://github.com/toil-free/QATLibrary/README.md
 Project-URL: Issue Tracker, https://github.com/toil-free/QATLibrary/issues
@@ -121,27 +121,28 @@
 1. [Sample CSV Test Data](https://github.com/sharif314/QATLibrary/blob/main/sample/TestCases.csv): Test Cases or Data file. 
 Test cases gets generated based on this file's content using Robot Framework. 
 
 2. [Sample Config YAML](https://github.com/sharif314/QATLibrary/blob/main/sample/config.yaml): This file contains various runtime configurations 
 for tests. Can be utilize to accommodate various CI or Test environments. Please follow the inline comments for more details -  
     ```yaml
     ---
-    # optional args; uncomment as-needed
+    # optional args; uncomment as-needed. 
+    # Any block or k/v not required, recommended to keep commented out for reasonable defaults. 
     base_url: httpbin.org           # base url/server name. Default localhost
     timeout: 10                     # In seconds. Default 5 seconds
     allow_redirects: True           # Allow Redirects. Default True.
     stream: False                   # True/False. Default False.
     
     ## global headers - these are added to every request from your data csv. All headers should be strings.
     headers:
       user-agent: QATLibrary                                  # this is a static header
       Authorization: Basic c29tZXVzZXI6bm90dmVyeXNlY3JldHBhc3M=
-      # dynamic headers can be added with ${} syntax like below -
-      X-correlation-id: ${str(__import__('uuid').uuid4())}         # dynamic headers use python's eval func.
-      random-digit: ${str(__import__('random').randint(0,99))}     # dynamic headers use python's eval func.
+      # dynamic headers can be added with ${{ }} syntax like below -
+      X-correlation-id: ${{str(__import__('uuid').uuid4())}}         # dynamic headers use python's eval func.
+      random-digit: ${{str(__import__('random').randint(0,99))}}     # dynamic headers use python's eval func.
     
     
     ## To enable proxies for http/https, enable the following config.
     #proxies:
     #  http_proxy:                   # HTTP proxy. Default None.
     #  https_proxy:                  # HTTPS proxy. Default None.
     #  no_proxy:                     # Bypass proxy
@@ -165,14 +166,15 @@
     #    grant_type:
     
     ## Enable following block for bearer auth TLS config.
     #  tls:
     #    verify_server_cert: True       # True/False or path to CA Bundle. Default False.
     #    certificate:                  # .pem format certificate. Default None
     #    private_key:                  # .pem format private key (unencrypted). Default None
+
    ```
 
 Once the files are generated, you can rename them according to your test suites or requirements.  
 
 ## Contributing
 This is [Sharif](https://www.linkedin.com/in/sharif-rahman/). I started this project basically to make my life 
 a bit easier around simple REST API tests. This project is ideal for you if want to get some automated tests done
```

### Comparing `QATLibrary-23.5.2/README.md` & `QATLibrary-23.5.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -94,27 +94,28 @@
 1. [Sample CSV Test Data](https://github.com/sharif314/QATLibrary/blob/main/sample/TestCases.csv): Test Cases or Data file. 
 Test cases gets generated based on this file's content using Robot Framework. 
 
 2. [Sample Config YAML](https://github.com/sharif314/QATLibrary/blob/main/sample/config.yaml): This file contains various runtime configurations 
 for tests. Can be utilize to accommodate various CI or Test environments. Please follow the inline comments for more details -  
     ```yaml
     ---
-    # optional args; uncomment as-needed
+    # optional args; uncomment as-needed. 
+    # Any block or k/v not required, recommended to keep commented out for reasonable defaults. 
     base_url: httpbin.org           # base url/server name. Default localhost
     timeout: 10                     # In seconds. Default 5 seconds
     allow_redirects: True           # Allow Redirects. Default True.
     stream: False                   # True/False. Default False.
     
     ## global headers - these are added to every request from your data csv. All headers should be strings.
     headers:
       user-agent: QATLibrary                                  # this is a static header
       Authorization: Basic c29tZXVzZXI6bm90dmVyeXNlY3JldHBhc3M=
-      # dynamic headers can be added with ${} syntax like below -
-      X-correlation-id: ${str(__import__('uuid').uuid4())}         # dynamic headers use python's eval func.
-      random-digit: ${str(__import__('random').randint(0,99))}     # dynamic headers use python's eval func.
+      # dynamic headers can be added with ${{ }} syntax like below -
+      X-correlation-id: ${{str(__import__('uuid').uuid4())}}         # dynamic headers use python's eval func.
+      random-digit: ${{str(__import__('random').randint(0,99))}}     # dynamic headers use python's eval func.
     
     
     ## To enable proxies for http/https, enable the following config.
     #proxies:
     #  http_proxy:                   # HTTP proxy. Default None.
     #  https_proxy:                  # HTTPS proxy. Default None.
     #  no_proxy:                     # Bypass proxy
@@ -138,14 +139,15 @@
     #    grant_type:
     
     ## Enable following block for bearer auth TLS config.
     #  tls:
     #    verify_server_cert: True       # True/False or path to CA Bundle. Default False.
     #    certificate:                  # .pem format certificate. Default None
     #    private_key:                  # .pem format private key (unencrypted). Default None
+
    ```
 
 Once the files are generated, you can rename them according to your test suites or requirements.  
 
 ## Contributing
 This is [Sharif](https://www.linkedin.com/in/sharif-rahman/). I started this project basically to make my life 
 a bit easier around simple REST API tests. This project is ideal for you if want to get some automated tests done
```

### Comparing `QATLibrary-23.5.2/setup.cfg` & `QATLibrary-23.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `QATLibrary-23.5.2/src/QATLibrary/QATLibrary.py` & `QATLibrary-23.5.3/src/QATLibrary/QATLibrary.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from .TLSAdapter import TLSAdapter
 
 
 class QATLibrary(object):
     ROBOT_LISTENER_API_VERSION = 3
     ROBOT_LIBRARY_SCOPE = 'TEST SUITE'
-    HEADER_VAR_EXP = re.compile(r"\${[^}]*}")
+    HEADER_VAR_EXP = re.compile(r"\$\{\{.*?\}\}")
 
     # init session
     session = Session()
     session.mount('https://', TLSAdapter())
 
     def __init__(self):
         self.ROBOT_LIBRARY_LISTENER = self
@@ -161,15 +161,15 @@
         # add bearer auth if available
         global_headers = self.builtin.get_variable_value('${BEARER_AUTH}', {})
 
         # process global headers
         config_headers = self.builtin.get_variable_value('${headers}', {})
         if config_headers:
             for k, v in config_headers.items():
-                global_headers[k] = eval(re.sub(r'\${(.*?)}', r'\1', v)) if self.HEADER_VAR_EXP.search(v) else v
+                global_headers[k] = eval(re.sub(r'\$\{\{(.*?)\}\}', r'\1', v)) if self.HEADER_VAR_EXP.search(v) else v
 
         # check for user defined headers
         usr_def_headers = self.__get_dict(data['reqHeaders'])
         if usr_def_headers:
             return dict(global_headers.items() | usr_def_headers.items())
         return global_headers
```

### Comparing `QATLibrary-23.5.2/src/QATLibrary/TLSAdapter.py` & `QATLibrary-23.5.3/src/QATLibrary/TLSAdapter.py`

 * *Files identical despite different names*

### Comparing `QATLibrary-23.5.2/src/QATLibrary/cli.py` & `QATLibrary-23.5.3/src/QATLibrary/cli.py`

 * *Files identical despite different names*

### Comparing `QATLibrary-23.5.2/src/QATLibrary.egg-info/PKG-INFO` & `QATLibrary-23.5.3/src/QATLibrary.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QATLibrary
-Version: 23.5.2
+Version: 23.5.3
 Summary: Data/Configuration Driven REST API Test Automation Library. Can be used as a Robot Framework Library or as standalone CLI tool.
 Home-page: https://github.com/toil-free/QATLibrary.git
 Author: Sharif Rahman
 Author-email: shrif.sbu@gmail.com
 License: MIT
 Project-URL: Docs, https://github.com/toil-free/QATLibrary/README.md
 Project-URL: Issue Tracker, https://github.com/toil-free/QATLibrary/issues
@@ -121,27 +121,28 @@
 1. [Sample CSV Test Data](https://github.com/sharif314/QATLibrary/blob/main/sample/TestCases.csv): Test Cases or Data file. 
 Test cases gets generated based on this file's content using Robot Framework. 
 
 2. [Sample Config YAML](https://github.com/sharif314/QATLibrary/blob/main/sample/config.yaml): This file contains various runtime configurations 
 for tests. Can be utilize to accommodate various CI or Test environments. Please follow the inline comments for more details -  
     ```yaml
     ---
-    # optional args; uncomment as-needed
+    # optional args; uncomment as-needed. 
+    # Any block or k/v not required, recommended to keep commented out for reasonable defaults. 
     base_url: httpbin.org           # base url/server name. Default localhost
     timeout: 10                     # In seconds. Default 5 seconds
     allow_redirects: True           # Allow Redirects. Default True.
     stream: False                   # True/False. Default False.
     
     ## global headers - these are added to every request from your data csv. All headers should be strings.
     headers:
       user-agent: QATLibrary                                  # this is a static header
       Authorization: Basic c29tZXVzZXI6bm90dmVyeXNlY3JldHBhc3M=
-      # dynamic headers can be added with ${} syntax like below -
-      X-correlation-id: ${str(__import__('uuid').uuid4())}         # dynamic headers use python's eval func.
-      random-digit: ${str(__import__('random').randint(0,99))}     # dynamic headers use python's eval func.
+      # dynamic headers can be added with ${{ }} syntax like below -
+      X-correlation-id: ${{str(__import__('uuid').uuid4())}}         # dynamic headers use python's eval func.
+      random-digit: ${{str(__import__('random').randint(0,99))}}     # dynamic headers use python's eval func.
     
     
     ## To enable proxies for http/https, enable the following config.
     #proxies:
     #  http_proxy:                   # HTTP proxy. Default None.
     #  https_proxy:                  # HTTPS proxy. Default None.
     #  no_proxy:                     # Bypass proxy
@@ -165,14 +166,15 @@
     #    grant_type:
     
     ## Enable following block for bearer auth TLS config.
     #  tls:
     #    verify_server_cert: True       # True/False or path to CA Bundle. Default False.
     #    certificate:                  # .pem format certificate. Default None
     #    private_key:                  # .pem format private key (unencrypted). Default None
+
    ```
 
 Once the files are generated, you can rename them according to your test suites or requirements.  
 
 ## Contributing
 This is [Sharif](https://www.linkedin.com/in/sharif-rahman/). I started this project basically to make my life 
 a bit easier around simple REST API tests. This project is ideal for you if want to get some automated tests done
```

