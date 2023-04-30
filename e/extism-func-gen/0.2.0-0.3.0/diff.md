# Comparing `tmp/extism_func_gen-0.2.0.tar.gz` & `tmp/extism_func_gen-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extism_func_gen-0.2.0.tar", max compression
+gzip compressed data, was "extism_func_gen-0.3.0.tar", max compression
```

## Comparing `extism_func_gen-0.2.0.tar` & `extism_func_gen-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      731 2023-04-28 20:12:31.368439 extism_func_gen-0.2.0/README.md
--rw-r--r--   0        0        0     3086 2023-04-28 20:22:00.982673 extism_func_gen-0.2.0/func_gen/__init__.py
--rw-r--r--   0        0        0   958069 2023-04-27 16:34:39.047735 extism_func_gen-0.2.0/func_gen/eval.wasm
--rw-r--r--   0        0        0      437 2023-04-28 20:22:05.718481 extism_func_gen-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 extism_func_gen-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      741 2023-04-28 22:36:50.998017 extism_func_gen-0.3.0/README.md
+-rw-r--r--   0        0        0     4079 2023-04-30 20:58:00.513758 extism_func_gen-0.3.0/func_gen/__init__.py
+-rw-r--r--   0        0        0   958069 2023-04-27 16:34:39.047735 extism_func_gen-0.3.0/func_gen/eval.wasm
+-rw-r--r--   0        0        0      437 2023-04-30 20:59:31.487403 extism_func_gen-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 extism_func_gen-0.3.0/PKG-INFO
```

### Comparing `extism_func_gen-0.2.0/README.md` & `extism_func_gen-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 It uses [langchain](https://python.langchain.com/en/latest/index.html) to create javascript functions
 to process text, and it uses [Extism](https://extism.org/) and the [JavaScript PDK](https://extism.org/docs/write-a-plugin/js-pdk)
 to safely execute the code in a Wasm sandbox.
 
 ## Install
 
 ```
-pip install extism-func-gen
+pip install --upgrade extism-func-gen
 ```
 
 ## Run
 
 ```bash
 # Need to set the OpenAI API key
 export OPENAI_API_KEY="sk-<paste-key-here>"
```

### Comparing `extism_func_gen-0.2.0/func_gen/__init__.py` & `extism_func_gen-0.3.0/func_gen/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,33 +7,50 @@
 from extism import Context
 from langchain.chat_models import ChatOpenAI
 from langchain.schema import (
     HumanMessage,
     SystemMessage
 )
 
-MARKDOWN_RE = re.compile("\\`\\`\\`javascript([^\\`]*)\\`\\`\\`")
+MARKDOWN_RE = re.compile("\\`\\`\\`(javascript|js)([^\\`]*)\\`\\`\\`")
 HOME_DIR = pathlib.Path.home() / ".func-gen"
 
 
 def generate_code(description):
     chat = ChatOpenAI(temperature=0, client=None)
 
     messages = [
         SystemMessage(content="Your goal is to write a Javascript function."),
-        SystemMessage(content="You must export the function as the default export, using the CommonJS module syntax"),
+        SystemMessage(content="You must export the function as the default export, using the CommonJS module syntax."),
+        SystemMessage(content="You should not import or require any code."),
+        SystemMessage(content="""
+This JavaScript environment has a global object for making http request called "Http". On that object is a function
+"request" which is a synchronous, blocking funciton and has the following jsdoc:
+
+@param {Object} request - The HTTP request object
+@param {string} request.url - The url for the request
+@param {string} request.method - The HTTP method for the request
+@param {Object} request.headers - Key-Value pairs to be assigned to the headers of the response
+@param {string} body - The request HTTP body. This parameter is required. Use null if the body is not needed.
+@return {HttpResponse} - the HTTP response
+
+It returns an HttpResponse which has two properties, a "body" containing the HTTP response body as a string
+and "status_code" which contains the integer Http status code.
+
+You are to use this function to make http requests
+                      """.strip()),
         SystemMessage(content="You must not include any comments, explanations, or markdown. The response should be JavaScript only."),
         HumanMessage(content=description),
     ]
 
     response = chat(messages)
     code = response.content
     match = MARKDOWN_RE.match(code)
-    if match and match.group(1):
-        code = match.group(1)
+    if match and match.group(2):
+        code = match.group(2)
     return code
 
 
 def execute_code(code, input):
     wasm_file_path = pathlib.Path(__file__).parent / "eval.wasm"
     wasm = wasm_file_path.read_bytes()
     hash = hashlib.sha256(wasm).hexdigest()
```

### Comparing `extism_func_gen-0.2.0/func_gen/eval.wasm` & `extism_func_gen-0.3.0/func_gen/eval.wasm`

 * *Files identical despite different names*

### Comparing `extism_func_gen-0.2.0/PKG-INFO` & `extism_func_gen-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extism-func-gen
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 License: MIT
 Author: The Extism Authors
 Author-email: oss@extism.org
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 It uses [langchain](https://python.langchain.com/en/latest/index.html) to create javascript functions
 to process text, and it uses [Extism](https://extism.org/) and the [JavaScript PDK](https://extism.org/docs/write-a-plugin/js-pdk)
 to safely execute the code in a Wasm sandbox.
 
 ## Install
 
 ```
-pip install extism-func-gen
+pip install --upgrade extism-func-gen
 ```
 
 ## Run
 
 ```bash
 # Need to set the OpenAI API key
 export OPENAI_API_KEY="sk-<paste-key-here>"
```

