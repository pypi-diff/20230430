# Comparing `tmp/gptagent-0.0.6.tar.gz` & `tmp/gptagent-0.0.7.tar.gz`

## Comparing `gptagent-0.0.6.tar` & `gptagent-0.0.7.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gptagent-0.0.6/chat_key.json
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 gptagent-0.0.6/src/GPTAgent/GPTAgent.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gptagent-0.0.6/src/GPTAgent/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 gptagent-0.0.6/tests/testa_agente.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 gptagent-0.0.6/LICENSE
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 gptagent-0.0.6/README.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 gptagent-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 gptagent-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gptagent-0.0.7/chat_key.json
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 gptagent-0.0.7/src/GPTAgent/GPTAgent.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 gptagent-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 gptagent-0.0.7/LICENSE
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 gptagent-0.0.7/README.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 gptagent-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 gptagent-0.0.7/PKG-INFO
```

### Comparing `gptagent-0.0.6/src/GPTAgent/GPTAgent.py` & `gptagent-0.0.7/src/GPTAgent/GPTAgent.py`

 * *Files identical despite different names*

### Comparing `gptagent-0.0.6/LICENSE` & `gptagent-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gptagent-0.0.6/pyproject.toml` & `gptagent-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "openai"]
 build-backend = "hatchling.build"
 
 [project]
 name = "GPTAgent"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Hobbert Evergreen", email="inteligenciamilgrau@gmail.com" },
 ]
 description = "A small and simple way to generate a ChatGPT agent"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `gptagent-0.0.6/PKG-INFO` & `gptagent-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPTAgent
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small and simple way to generate a ChatGPT agent
 Project-URL: Homepage, https://github.com/inteligenciamilgrau/ChatGPT/tree/main/GPTAgent
 Author-email: Hobbert Evergreen <inteligenciamilgrau@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -25,13 +25,13 @@
 ```
 {"api_key": "coloque_aqui_sua_api_key_da_OpenAI"}
 ```
 
 Exemplo:
 
 ```
-from GPTAgent_img import GPTAgent
+from GPTAgent.GPTAgent import GPTAgent
 
-agente = GPTAgent.GPTAgent(name="Bob", estilo="Você é engraçado e positivo.")
+agente = GPTAgent(name="Bob", estilo="Você é engraçado e positivo.")
 
 print(agente.perguntar("Bom dia!"))
 ```
```

