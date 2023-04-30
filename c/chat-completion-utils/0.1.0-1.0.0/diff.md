# Comparing `tmp/chat_completion_utils-0.1.0.tar.gz` & `tmp/chat_completion_utils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_completion_utils-0.1.0.tar", max compression
+gzip compressed data, was "chat_completion_utils-1.0.0.tar", max compression
```

## Comparing `chat_completion_utils-0.1.0.tar` & `chat_completion_utils-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3798 2023-04-12 17:43:11.699264 chat_completion_utils-0.1.0/README.md
--rw-r--r--   0        0        0       19 2023-04-30 05:31:20.562503 chat_completion_utils-0.1.0/chat_completion_utils/__init__.py
--rw-r--r--   0        0        0     5316 2023-04-30 05:31:12.899379 chat_completion_utils-0.1.0/chat_completion_utils/main.py
--rw-r--r--   0        0        0      367 2023-04-12 17:40:30.904955 chat_completion_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4279 1970-01-01 00:00:00.000000 chat_completion_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3798 2023-04-12 17:43:11.699264 chat_completion_utils-1.0.0/README.md
+-rw-r--r--   0        0        0       36 2023-04-30 06:33:02.330135 chat_completion_utils-1.0.0/chat_completion_utils/__init__.py
+-rw-r--r--   0        0        0     5316 2023-04-30 05:47:53.378321 chat_completion_utils-1.0.0/chat_completion_utils/chat_completion_utils.py
+-rw-r--r--   0        0        0      367 2023-04-30 06:34:40.326696 chat_completion_utils-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4279 1970-01-01 00:00:00.000000 chat_completion_utils-1.0.0/PKG-INFO
```

### Comparing `chat_completion_utils-0.1.0/README.md` & `chat_completion_utils-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `chat_completion_utils-0.1.0/chat_completion_utils/main.py` & `chat_completion_utils-1.0.0/chat_completion_utils/chat_completion_utils.py`

 * *Files identical despite different names*

### Comparing `chat_completion_utils-0.1.0/PKG-INFO` & `chat_completion_utils-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-completion-utils
-Version: 0.1.0
+Version: 1.0.0
 Summary: 
 Author: estill01
 Author-email: ehs.stillman@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

