# Comparing `tmp/chat_completion_utils-1.2.2.tar.gz` & `tmp/chat_completion_utils-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_completion_utils-1.2.2.tar", max compression
+gzip compressed data, was "chat_completion_utils-1.2.3.tar", max compression
```

## Comparing `chat_completion_utils-1.2.2.tar` & `chat_completion_utils-1.2.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3798 2023-04-12 17:43:11.699264 chat_completion_utils-1.2.2/README.md
--rw-r--r--   0        0        0       26 2023-04-30 06:44:13.145330 chat_completion_utils-1.2.2/chat_completion_utils/__init__.py
--rw-r--r--   0        0        0     5323 2023-04-30 06:53:21.079583 chat_completion_utils-1.2.2/chat_completion_utils/chat_utils.py
--rw-r--r--   0        0        0      367 2023-04-30 06:53:26.100407 chat_completion_utils-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     4279 1970-01-01 00:00:00.000000 chat_completion_utils-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     3798 2023-04-12 17:43:11.699264 chat_completion_utils-1.2.3/README.md
+-rw-r--r--   0        0        0       26 2023-04-30 06:44:13.145330 chat_completion_utils-1.2.3/chat_completion_utils/__init__.py
+-rw-r--r--   0        0        0     5337 2023-04-30 06:54:38.062548 chat_completion_utils-1.2.3/chat_completion_utils/chat_utils.py
+-rw-r--r--   0        0        0      367 2023-04-30 06:54:41.758642 chat_completion_utils-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4279 1970-01-01 00:00:00.000000 chat_completion_utils-1.2.3/PKG-INFO
```

### Comparing `chat_completion_utils-1.2.2/README.md` & `chat_completion_utils-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `chat_completion_utils-1.2.2/chat_completion_utils/chat_utils.py` & `chat_completion_utils-1.2.3/chat_completion_utils/chat_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 from typing import List
 
 openai.api_key=os.environ.get("OPENAI_API_KEY")
 
 MODELS = {
     'models': ['gpt-3.5-turbo', 'gpt-4', 'gpt-4-32k'],
     'gpt-3.5-turbo': {
-        model: 'gpt-3.5-turbo',
-        max_tokens: 4096,
+        'model': 'gpt-3.5-turbo',
+        'max_tokens': 4096,
     },
     'gpt-4': { 
-        model: 'gpt-4',
-        max_tokens: 8192,
+        'model': 'gpt-4',
+        'max_tokensi': 8192,
     },
     'gpt-4-32k': {
-        model: 'gpt-4-32k',
-        max_tokens: 32768,
+        'modeli': 'gpt-4-32k',
+        'max_tokens': 32768,
     },
 }
 
 DEFAULT_MODEL=MODELS['gpt-4'].model
 
 def set_default_model(model_family: str='gpt-4') -> None:
     DEFAULT_MODEL=model_family
```

### Comparing `chat_completion_utils-1.2.2/PKG-INFO` & `chat_completion_utils-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-completion-utils
-Version: 1.2.2
+Version: 1.2.3
 Summary: 
 Author: estill01
 Author-email: ehs.stillman@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

