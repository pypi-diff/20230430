# Comparing `tmp/gptagent-0.0.8.tar.gz` & `tmp/gptagent-0.0.9.tar.gz`

## Comparing `gptagent-0.0.8.tar` & `gptagent-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gptagent-0.0.8/examples/chat_key.json
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 gptagent-0.0.8/examples/gptagent_example.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 gptagent-0.0.8/src/GPTAgent/GPTAgent.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 gptagent-0.0.8/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 gptagent-0.0.8/LICENSE
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 gptagent-0.0.8/README.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 gptagent-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 gptagent-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 gptagent-0.0.9/src/GPTAgent/GPTAgent.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gptagent-0.0.9/tests/chat_key.json
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 gptagent-0.0.9/tests/gptagent_example.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 gptagent-0.0.9/tests/testa_agente.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 gptagent-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 gptagent-0.0.9/LICENSE
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 gptagent-0.0.9/README.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 gptagent-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 gptagent-0.0.9/PKG-INFO
```

### Comparing `gptagent-0.0.8/src/GPTAgent/GPTAgent.py` & `gptagent-0.0.9/src/GPTAgent/GPTAgent.py`

 * *Files identical despite different names*

### Comparing `gptagent-0.0.8/LICENSE` & `gptagent-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gptagent-0.0.8/pyproject.toml` & `gptagent-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "openai"]
 build-backend = "hatchling.build"
 
 [project]
 name = "GPTAgent"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Hobbert Evergreen", email="inteligenciamilgrau@gmail.com" },
 ]
 description = "A small and simple way to generate a ChatGPT agent"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `gptagent-0.0.8/PKG-INFO` & `gptagent-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPTAgent
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small and simple way to generate a ChatGPT agent
 Project-URL: Homepage, https://github.com/inteligenciamilgrau/ChatGPT/tree/main/GPTAgent
 Author-email: Hobbert Evergreen <inteligenciamilgrau@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

