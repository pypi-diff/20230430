# Comparing `tmp/search_hound_ai-0.1.6.tar.gz` & `tmp/search_hound_ai-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "search_hound_ai-0.1.6.tar", max compression
+gzip compressed data, was "search_hound_ai-0.1.8.tar", max compression
```

## Comparing `search_hound_ai-0.1.6.tar` & `search_hound_ai-0.1.8.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-04-22 04:54:54.011720 search_hound_ai-0.1.6/LICENSE
--rw-r--r--   0        0        0      960 2023-04-22 04:54:54.011720 search_hound_ai-0.1.6/README.md
--rw-r--r--   0        0        0      673 2023-04-22 04:54:54.011720 search_hound_ai-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      504 2023-04-22 04:54:54.011720 search_hound_ai-0.1.6/search_hound_ai/__init__.py
--rwxr-xr-x   0        0        0      385 2023-04-22 04:54:54.011720 search_hound_ai-0.1.6/search_hound_ai/app.py
--rw-r--r--   0        0        0      369 2023-04-22 04:54:54.011720 search_hound_ai-0.1.6/search_hound_ai/app_test.py
--rw-r--r--   0        0        0      643 2023-04-22 04:54:54.011720 search_hound_ai-0.1.6/search_hound_ai/hound_client_commands.py
--rw-r--r--   0        0        0     1146 2023-04-22 04:54:54.011720 search_hound_ai-0.1.6/search_hound_ai/openai_lib.py
--rw-r--r--   0        0        0      773 2023-04-22 04:54:54.011720 search_hound_ai-0.1.6/search_hound_ai/search_hound_lib.py
--rw-r--r--   0        0        0      681 2023-04-22 04:54:54.011720 search_hound_ai-0.1.6/search_hound_ai/validate_env.py
--rw-r--r--   0        0        0     1590 1970-01-01 00:00:00.000000 search_hound_ai-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-24 05:26:18.013833 search_hound_ai-0.1.8/LICENSE
+-rw-r--r--   0        0        0      967 2023-04-24 05:26:18.013833 search_hound_ai-0.1.8/README.md
+-rw-r--r--   0        0        0      673 2023-04-24 05:26:18.013833 search_hound_ai-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      504 2023-04-24 05:26:18.013833 search_hound_ai-0.1.8/search_hound_ai/__init__.py
+-rwxr-xr-x   0        0        0      385 2023-04-24 05:26:18.013833 search_hound_ai-0.1.8/search_hound_ai/app.py
+-rw-r--r--   0        0        0      643 2023-04-24 05:26:18.013833 search_hound_ai-0.1.8/search_hound_ai/hound_client_commands.py
+-rw-r--r--   0        0        0     1146 2023-04-24 05:26:18.013833 search_hound_ai-0.1.8/search_hound_ai/openai_lib.py
+-rw-r--r--   0        0        0      868 2023-04-24 05:26:18.013833 search_hound_ai-0.1.8/search_hound_ai/search_hound_lib.py
+-rw-r--r--   0        0        0      778 2023-04-24 05:26:18.013833 search_hound_ai-0.1.8/search_hound_ai/validate_env.py
+-rw-r--r--   0        0        0     1597 1970-01-01 00:00:00.000000 search_hound_ai-0.1.8/PKG-INFO
```

### Comparing `search_hound_ai-0.1.6/LICENSE` & `search_hound_ai-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `search_hound_ai-0.1.6/README.md` & `search_hound_ai-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SearchHoundAI
+# SearchHoundAI  🐕 
 
 A CLI for GPT with a focus on simplicity and ease of use. For developer just wanting to use gpt in there command line.
 
 PIP Package: [Search Hound AI](https://pypi.org/project/search-hound-ai/)
 
 ## Installation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `search_hound_ai-0.1.6/pyproject.toml` & `search_hound_ai-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "search-hound-ai"
-version = "0.1.6"
+version = "0.1.8"
 description = "A CLI for GPT with a focus on simplicity and ease of use. For developer just wanting to use gpt in there command line."
 authors = ["Martin Patino <martin@sibipro.com>"]
 readme = "README.md"
 packages = [{include = "search_hound_ai"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `search_hound_ai-0.1.6/search_hound_ai/hound_client_commands.py` & `search_hound_ai-0.1.8/search_hound_ai/hound_client_commands.py`

 * *Files identical despite different names*

### Comparing `search_hound_ai-0.1.6/search_hound_ai/openai_lib.py` & `search_hound_ai-0.1.8/search_hound_ai/openai_lib.py`

 * *Files identical despite different names*

### Comparing `search_hound_ai-0.1.6/search_hound_ai/search_hound_lib.py` & `search_hound_ai-0.1.8/search_hound_ai/search_hound_lib.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import typer
+import pkg_resources
 
 from search_hound_ai.openai_lib import OpenAISearch
 
 
 class SearchHoundLib:
     """"Provides a simple interface to openai.
 
@@ -15,12 +16,13 @@
     def searchHound(search_string: str) -> str:
         response: str = OpenAISearch(search_string)
         return response
     def storeOpenAIConfig(config: str):
         if config is None or config == "":
             return "OPENAI_API_KEY config provided"
         
-        text_file = open(".env", "w")
+        filename = pkg_resources.resource_filename(__name__, "../.env")
+        text_file = open(filename, "w")
         text_file.write('OPENAI_API_KEY=' + config)
         text_file.close()
 
         return "OPENAI_API_KEY ENV saved"
```

### Comparing `search_hound_ai-0.1.6/search_hound_ai/validate_env.py` & `search_hound_ai-0.1.8/search_hound_ai/validate_env.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import logging
 import os
 
+import pkg_resources
+
 def ValidateEnv():
     OPENAI_API_KEY = os.getenv('OPENAI_API_KEY')
     print("OPENAI_API_KEY", OPENAI_API_KEY)
     if OPENAI_API_KEY == None or OPENAI_API_KEY == '':
         open_ai_key_value = input("Enter your OPENAI_API_KEY: ")
 
         if open_ai_key_value == None or open_ai_key_value == '':
             logging.error("OPENAI_API_KEY is required.")
             exit(1)
 
         if open_ai_key_value != None and open_ai_key_value != '':
-            text_file = open(".env", "w")
+            filename = pkg_resources.resource_filename(__name__, ".env")
+            text_file = open(filename, "w")
             text_file.write('OPENAI_API_KEY=' + open_ai_key_value)
             text_file.close()
             logging.info("OPENAI_API_KEY ENV saved")
             exit(1)
```

### Comparing `search_hound_ai-0.1.6/PKG-INFO` & `search_hound_ai-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: search-hound-ai
-Version: 0.1.6
+Version: 0.1.8
 Summary: A CLI for GPT with a focus on simplicity and ease of use. For developer just wanting to use gpt in there command line.
 Author: Martin Patino
 Author-email: martin@sibipro.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: langchain (>=0.0.146,<0.0.147)
 Requires-Dist: load-dotenv (>=0.1.0,<0.2.0)
 Requires-Dist: logging (>=0.4.9.6,<0.5.0.0)
 Requires-Dist: openai (>=0.27.4,<0.28.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
-# SearchHoundAI
+# SearchHoundAI  🐕 
 
 A CLI for GPT with a focus on simplicity and ease of use. For developer just wanting to use gpt in there command line.
 
 PIP Package: [Search Hound AI](https://pypi.org/project/search-hound-ai/)
 
 ## Installation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

