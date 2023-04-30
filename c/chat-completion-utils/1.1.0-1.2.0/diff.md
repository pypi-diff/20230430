# Comparing `tmp/chat_completion_utils-1.1.0.tar.gz` & `tmp/chat_completion_utils-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_completion_utils-1.1.0.tar", max compression
+gzip compressed data, was "chat_completion_utils-1.2.0.tar", max compression
```

## Comparing `chat_completion_utils-1.1.0.tar` & `chat_completion_utils-1.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3798 2023-04-12 17:43:11.699264 chat_completion_utils-1.1.0/README.md
--rw-r--r--   0        0        0       26 2023-04-30 06:44:13.145330 chat_completion_utils-1.1.0/chat_completion_utils/__init__.py
--rw-r--r--   0        0        0     5316 2023-04-30 05:47:53.378321 chat_completion_utils-1.1.0/chat_completion_utils/chat_utils.py
--rw-r--r--   0        0        0      367 2023-04-30 06:46:17.883371 chat_completion_utils-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4279 1970-01-01 00:00:00.000000 chat_completion_utils-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3798 2023-04-12 17:43:11.699264 chat_completion_utils-1.2.0/README.md
+-rw-r--r--   0        0        0       26 2023-04-30 06:44:13.145330 chat_completion_utils-1.2.0/chat_completion_utils/__init__.py
+-rw-r--r--   0        0        0     5318 2023-04-30 06:50:03.230237 chat_completion_utils-1.2.0/chat_completion_utils/chat_utils.py
+-rw-r--r--   0        0        0      367 2023-04-30 06:50:13.703487 chat_completion_utils-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4279 1970-01-01 00:00:00.000000 chat_completion_utils-1.2.0/PKG-INFO
```

### Comparing `chat_completion_utils-1.1.0/README.md` & `chat_completion_utils-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `chat_completion_utils-1.1.0/chat_completion_utils/chat_utils.py` & `chat_completion_utils-1.2.0/chat_completion_utils/chat_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 import os
 import tiktoken
 from typing import List
 
 openai.api_key=os.environ.get("OPENAI_API_KEY")
 
 MODELS = {
-    'models': ['gpt-3.5-turbo', 'gpt-4', 'gpt-4-32k']
+    'models': ['gpt-3.5-turbo', 'gpt-4', 'gpt-4-32k'],
     'gpt-3.5-turbo': {
         model: 'gpt-3.5-turbo',
         max_tokens: 4096,
     },
     'gpt-4': { 
         model: 'gpt-4',
         max_tokens: 8192,
     },
     'gpt-4-32k': {
         model: 'gpt-4-32k',
         max_tokens: 32768,
-    }
+    },
 }
 
 DEFAULT_MODEL=MODELS['gpt-4'].model
 
 def set_default_model(model_family: str='gpt-4') -> None:
     DEFAULT_MODEL=model_family
```

### Comparing `chat_completion_utils-1.1.0/PKG-INFO` & `chat_completion_utils-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-completion-utils
-Version: 1.1.0
+Version: 1.2.0
 Summary: 
 Author: estill01
 Author-email: ehs.stillman@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

