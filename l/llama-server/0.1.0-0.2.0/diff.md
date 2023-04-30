# Comparing `tmp/llama-server-0.1.0.tar.gz` & `tmp/llama-server-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama-server-0.1.0.tar", last modified: Wed Apr 12 04:39:21 2023, max compression
+gzip compressed data, was "llama-server-0.2.0.tar", last modified: Sun Apr 30 04:57:20 2023, max compression
```

## Comparing `llama-server-0.1.0.tar` & `llama-server-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:39:21.288362 llama-server-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-12 04:39:09.000000 llama-server-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-12 04:39:21.288362 llama-server-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-12 04:39:09.000000 llama-server-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:39:21.288362 llama-server-0.1.0/llama_server/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 04:39:09.000000 llama-server-0.1.0/llama_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:39:21.288362 llama-server-0.1.0/llama_server/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 04:39:09.000000 llama-server-0.1.0/llama_server/prompts/alpaca.txt
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-12 04:39:09.000000 llama-server-0.1.0/llama_server/prompts/chat-with-bob.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-12 04:39:09.000000 llama-server-0.1.0/llama_server/prompts/dan.txt
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-12 04:39:09.000000 llama-server-0.1.0/llama_server/prompts/reason-act.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-04-12 04:39:09.000000 llama-server-0.1.0/llama_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:39:21.288362 llama-server-0.1.0/llama_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-12 04:39:21.000000 llama-server-0.1.0/llama_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-12 04:39:21.000000 llama-server-0.1.0/llama_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 04:39:21.000000 llama-server-0.1.0/llama_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-12 04:39:21.000000 llama-server-0.1.0/llama_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 04:39:21.000000 llama-server-0.1.0/llama_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-12 04:39:21.000000 llama-server-0.1.0/llama_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-12 04:39:21.288362 llama-server-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-12 04:39:09.000000 llama-server-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:57:20.546722 llama-server-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-30 04:57:10.000000 llama-server-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-30 04:57:20.546722 llama-server-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-30 04:57:10.000000 llama-server-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:57:20.542722 llama-server-0.2.0/llama_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 04:57:10.000000 llama-server-0.2.0/llama_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:57:20.546722 llama-server-0.2.0/llama_server/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-30 04:57:10.000000 llama-server-0.2.0/llama_server/prompts/alpaca.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-30 04:57:10.000000 llama-server-0.2.0/llama_server/prompts/chat-with-bob.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-30 04:57:10.000000 llama-server-0.2.0/llama_server/prompts/dan.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-30 04:57:10.000000 llama-server-0.2.0/llama_server/prompts/reason-act.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-30 04:57:10.000000 llama-server-0.2.0/llama_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:57:20.542722 llama-server-0.2.0/llama_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-30 04:57:20.000000 llama-server-0.2.0/llama_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-30 04:57:20.000000 llama-server-0.2.0/llama_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 04:57:20.000000 llama-server-0.2.0/llama_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-30 04:57:20.000000 llama-server-0.2.0/llama_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-30 04:57:20.000000 llama-server-0.2.0/llama_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-30 04:57:20.000000 llama-server-0.2.0/llama_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-30 04:57:20.546722 llama-server-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-30 04:57:10.000000 llama-server-0.2.0/setup.py
```

### Comparing `llama-server-0.1.0/LICENSE` & `llama-server-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llama-server-0.1.0/PKG-INFO` & `llama-server-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-server
-Version: 0.1.0
+Version: 0.2.0
 Summary: LLaMA Server combines the power of LLaMA C++ with the beauty of Chatbot UI.
 Home-page: https://github.com/nuance1979/llama-server
 Author: Yi Su
 Author-email: nuance@gmail.com
 License: MIT
 Keywords: llama llama.cpp chatbot-ui chatbot
 Classifier: Development Status :: 4 - Beta
@@ -18,25 +18,31 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # LLaMA Server
 
-[![PyPI version](https://img.shields.io/pypi/v/llama-server)](https://pypi.org/project/llama-server/)[![Unit test](https://github.com/nuance1979/llama-server/actions/workflows/test.yml/badge.svg?branch=main&&event=push)](https://github.com/nuance1979/llama-server/actions)[![GitHub stars](https://img.shields.io/github/stars/nuance1979/llama-server)](https://star-history.com/#nuance1979/llama-server&Date)[![GitHub license](https://img.shields.io/github/license/nuance1979/llama-server)](https://github.com/nuance1979/llama-server/blob/master/LICENSE)
+[![PyPI version](https://img.shields.io/pypi/v/llama-server)](https://pypi.org/project/llama-server/) [![Unit test](https://github.com/nuance1979/llama-server/actions/workflows/test.yml/badge.svg?branch=main&&event=push)](https://github.com/nuance1979/llama-server/actions) [![GitHub stars](https://img.shields.io/github/stars/nuance1979/llama-server)](https://star-history.com/#nuance1979/llama-server&Date) [![GitHub license](https://img.shields.io/github/license/nuance1979/llama-server)](https://github.com/nuance1979/llama-server/blob/master/LICENSE)
 
-LLaMA Server combines the power of [LLaMA C++](https://github.com/ggerganov/llama.cpp) (via [PyLLaMACpp](https://github.com/nomic-ai/pyllamacpp)) with the beauty of [Chatbot UI](https://github.com/mckaywrigley/chatbot-ui).
+LLaMA Server combines the power of [LLaMA C++](https://github.com/ggerganov/llama.cpp) (via [PyLLaMACpp](https://github.com/abdeladim-s/pyllamacpp)) with the beauty of [Chatbot UI](https://github.com/mckaywrigley/chatbot-ui).
 
 🦙LLaMA C++ (via 🐍PyLLaMACpp) ➕ 🤖Chatbot UI ➕ 🔗LLaMA Server 🟰 😊
 
-**UPDATE**: Now supports better streaming through [PyLLaMACpp](https://github.com/nomic-ai/pyllamacpp)!
+**UPDATE**: Greatly simplified implementation thanks to the [awesome Pythonic APIs](https://github.com/abdeladim-s/pyllamacpp#different-persona) of PyLLaMACpp 2.0.0!
+
+**UPDATE**: Now supports better streaming through [PyLLaMACpp](https://github.com/abdeladim-s/pyllamacpp)!
 
 **UPDATE**: Now supports streaming!
 
 ## Demo
+- Better Streaming
+
+https://user-images.githubusercontent.com/10931178/231539194-052f7c5f-c7a3-42b7-9f8b-142422e42a67.mov
+
 - Streaming
 
 https://user-images.githubusercontent.com/10931178/229980159-61546fa6-2985-4cdc-8230-5dcb6a69c559.mov
 
 - Non-streaming
 
 https://user-images.githubusercontent.com/10931178/229408428-5b6ef72d-28d0-427f-ae83-e23972e2dcff.mov
@@ -71,19 +77,14 @@
   python -m pip install llama-server
   ```
   - Or from source:
   ```bash
   python -m pip install git+https://github.com/nuance1979/llama-server.git
   ```
 
-- Install a patched version of PyLLaMACpp: (*Note:* this step will not be needed **after** PyLLaMACpp makes a new release.)
-```bash
-python -m pip install git+https://github.com/nuance1979/pyllamacpp.git@dev --upgrade
-```
-
 - Start LLaMA Server with your `models.yml` file:
 ```bash
 llama-server --models-yml models.yml --model-id llama-7b
 ```
 
 - Check out [my fork](https://github.com/nuance1979/chatbot-ui) of Chatbot UI and start the app;
 ```bash
@@ -107,19 +108,14 @@
 - Try a larger model if you have it:
 ```bash
 llama-server --models-yml models.yml --model-id llama-13b  # or any `model_id` defined in `models.yml`
 ```
 
 - Try non-streaming mode by restarting Chatbot UI:
 ```bash
-export LLAMA_STREAM_MODE=1  # 0 to disable streaming
+export LLAMA_STREAM_MODE=0  # 1 to enable streaming
 npm run dev
 ```
 
-## Limitations
-
-- "Regenerate response" is currently not working;
-- IMHO, the prompt/reverse-prompt machanism of LLaMA C++'s interactive mode needs an overhaul. I tried very hard to dance around it but the whole thing is still a hack.
-
 ## Fun facts
 
 I am not fluent in JavaScript at all but I was able to make the changes in Chatbot UI by chatting with [ChatGPT](https://chat.openai.com); no more StackOverflow.
```

### Comparing `llama-server-0.1.0/README.md` & `llama-server-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # LLaMA Server
 
-[![PyPI version](https://img.shields.io/pypi/v/llama-server)](https://pypi.org/project/llama-server/)[![Unit test](https://github.com/nuance1979/llama-server/actions/workflows/test.yml/badge.svg?branch=main&&event=push)](https://github.com/nuance1979/llama-server/actions)[![GitHub stars](https://img.shields.io/github/stars/nuance1979/llama-server)](https://star-history.com/#nuance1979/llama-server&Date)[![GitHub license](https://img.shields.io/github/license/nuance1979/llama-server)](https://github.com/nuance1979/llama-server/blob/master/LICENSE)
+[![PyPI version](https://img.shields.io/pypi/v/llama-server)](https://pypi.org/project/llama-server/) [![Unit test](https://github.com/nuance1979/llama-server/actions/workflows/test.yml/badge.svg?branch=main&&event=push)](https://github.com/nuance1979/llama-server/actions) [![GitHub stars](https://img.shields.io/github/stars/nuance1979/llama-server)](https://star-history.com/#nuance1979/llama-server&Date) [![GitHub license](https://img.shields.io/github/license/nuance1979/llama-server)](https://github.com/nuance1979/llama-server/blob/master/LICENSE)
 
-LLaMA Server combines the power of [LLaMA C++](https://github.com/ggerganov/llama.cpp) (via [PyLLaMACpp](https://github.com/nomic-ai/pyllamacpp)) with the beauty of [Chatbot UI](https://github.com/mckaywrigley/chatbot-ui).
+LLaMA Server combines the power of [LLaMA C++](https://github.com/ggerganov/llama.cpp) (via [PyLLaMACpp](https://github.com/abdeladim-s/pyllamacpp)) with the beauty of [Chatbot UI](https://github.com/mckaywrigley/chatbot-ui).
 
 🦙LLaMA C++ (via 🐍PyLLaMACpp) ➕ 🤖Chatbot UI ➕ 🔗LLaMA Server 🟰 😊
 
-**UPDATE**: Now supports better streaming through [PyLLaMACpp](https://github.com/nomic-ai/pyllamacpp)!
+**UPDATE**: Greatly simplified implementation thanks to the [awesome Pythonic APIs](https://github.com/abdeladim-s/pyllamacpp#different-persona) of PyLLaMACpp 2.0.0!
+
+**UPDATE**: Now supports better streaming through [PyLLaMACpp](https://github.com/abdeladim-s/pyllamacpp)!
 
 **UPDATE**: Now supports streaming!
 
 ## Demo
+- Better Streaming
+
+https://user-images.githubusercontent.com/10931178/231539194-052f7c5f-c7a3-42b7-9f8b-142422e42a67.mov
+
 - Streaming
 
 https://user-images.githubusercontent.com/10931178/229980159-61546fa6-2985-4cdc-8230-5dcb6a69c559.mov
 
 - Non-streaming
 
 https://user-images.githubusercontent.com/10931178/229408428-5b6ef72d-28d0-427f-ae83-e23972e2dcff.mov
@@ -49,19 +55,14 @@
   python -m pip install llama-server
   ```
   - Or from source:
   ```bash
   python -m pip install git+https://github.com/nuance1979/llama-server.git
   ```
 
-- Install a patched version of PyLLaMACpp: (*Note:* this step will not be needed **after** PyLLaMACpp makes a new release.)
-```bash
-python -m pip install git+https://github.com/nuance1979/pyllamacpp.git@dev --upgrade
-```
-
 - Start LLaMA Server with your `models.yml` file:
 ```bash
 llama-server --models-yml models.yml --model-id llama-7b
 ```
 
 - Check out [my fork](https://github.com/nuance1979/chatbot-ui) of Chatbot UI and start the app;
 ```bash
@@ -85,19 +86,14 @@
 - Try a larger model if you have it:
 ```bash
 llama-server --models-yml models.yml --model-id llama-13b  # or any `model_id` defined in `models.yml`
 ```
 
 - Try non-streaming mode by restarting Chatbot UI:
 ```bash
-export LLAMA_STREAM_MODE=1  # 0 to disable streaming
+export LLAMA_STREAM_MODE=0  # 1 to enable streaming
 npm run dev
 ```
 
-## Limitations
-
-- "Regenerate response" is currently not working;
-- IMHO, the prompt/reverse-prompt machanism of LLaMA C++'s interactive mode needs an overhaul. I tried very hard to dance around it but the whole thing is still a hack.
-
 ## Fun facts
 
 I am not fluent in JavaScript at all but I was able to make the changes in Chatbot UI by chatting with [ChatGPT](https://chat.openai.com); no more StackOverflow.
```

### Comparing `llama-server-0.1.0/llama_server/prompts/dan.txt` & `llama-server-0.2.0/llama_server/prompts/dan.txt`

 * *Files identical despite different names*

### Comparing `llama-server-0.1.0/llama_server/prompts/reason-act.txt` & `llama-server-0.2.0/llama_server/prompts/reason-act.txt`

 * *Files identical despite different names*

### Comparing `llama-server-0.1.0/llama_server.egg-info/PKG-INFO` & `llama-server-0.2.0/llama_server.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-server
-Version: 0.1.0
+Version: 0.2.0
 Summary: LLaMA Server combines the power of LLaMA C++ with the beauty of Chatbot UI.
 Home-page: https://github.com/nuance1979/llama-server
 Author: Yi Su
 Author-email: nuance@gmail.com
 License: MIT
 Keywords: llama llama.cpp chatbot-ui chatbot
 Classifier: Development Status :: 4 - Beta
@@ -18,25 +18,31 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # LLaMA Server
 
-[![PyPI version](https://img.shields.io/pypi/v/llama-server)](https://pypi.org/project/llama-server/)[![Unit test](https://github.com/nuance1979/llama-server/actions/workflows/test.yml/badge.svg?branch=main&&event=push)](https://github.com/nuance1979/llama-server/actions)[![GitHub stars](https://img.shields.io/github/stars/nuance1979/llama-server)](https://star-history.com/#nuance1979/llama-server&Date)[![GitHub license](https://img.shields.io/github/license/nuance1979/llama-server)](https://github.com/nuance1979/llama-server/blob/master/LICENSE)
+[![PyPI version](https://img.shields.io/pypi/v/llama-server)](https://pypi.org/project/llama-server/) [![Unit test](https://github.com/nuance1979/llama-server/actions/workflows/test.yml/badge.svg?branch=main&&event=push)](https://github.com/nuance1979/llama-server/actions) [![GitHub stars](https://img.shields.io/github/stars/nuance1979/llama-server)](https://star-history.com/#nuance1979/llama-server&Date) [![GitHub license](https://img.shields.io/github/license/nuance1979/llama-server)](https://github.com/nuance1979/llama-server/blob/master/LICENSE)
 
-LLaMA Server combines the power of [LLaMA C++](https://github.com/ggerganov/llama.cpp) (via [PyLLaMACpp](https://github.com/nomic-ai/pyllamacpp)) with the beauty of [Chatbot UI](https://github.com/mckaywrigley/chatbot-ui).
+LLaMA Server combines the power of [LLaMA C++](https://github.com/ggerganov/llama.cpp) (via [PyLLaMACpp](https://github.com/abdeladim-s/pyllamacpp)) with the beauty of [Chatbot UI](https://github.com/mckaywrigley/chatbot-ui).
 
 🦙LLaMA C++ (via 🐍PyLLaMACpp) ➕ 🤖Chatbot UI ➕ 🔗LLaMA Server 🟰 😊
 
-**UPDATE**: Now supports better streaming through [PyLLaMACpp](https://github.com/nomic-ai/pyllamacpp)!
+**UPDATE**: Greatly simplified implementation thanks to the [awesome Pythonic APIs](https://github.com/abdeladim-s/pyllamacpp#different-persona) of PyLLaMACpp 2.0.0!
+
+**UPDATE**: Now supports better streaming through [PyLLaMACpp](https://github.com/abdeladim-s/pyllamacpp)!
 
 **UPDATE**: Now supports streaming!
 
 ## Demo
+- Better Streaming
+
+https://user-images.githubusercontent.com/10931178/231539194-052f7c5f-c7a3-42b7-9f8b-142422e42a67.mov
+
 - Streaming
 
 https://user-images.githubusercontent.com/10931178/229980159-61546fa6-2985-4cdc-8230-5dcb6a69c559.mov
 
 - Non-streaming
 
 https://user-images.githubusercontent.com/10931178/229408428-5b6ef72d-28d0-427f-ae83-e23972e2dcff.mov
@@ -71,19 +77,14 @@
   python -m pip install llama-server
   ```
   - Or from source:
   ```bash
   python -m pip install git+https://github.com/nuance1979/llama-server.git
   ```
 
-- Install a patched version of PyLLaMACpp: (*Note:* this step will not be needed **after** PyLLaMACpp makes a new release.)
-```bash
-python -m pip install git+https://github.com/nuance1979/pyllamacpp.git@dev --upgrade
-```
-
 - Start LLaMA Server with your `models.yml` file:
 ```bash
 llama-server --models-yml models.yml --model-id llama-7b
 ```
 
 - Check out [my fork](https://github.com/nuance1979/chatbot-ui) of Chatbot UI and start the app;
 ```bash
@@ -107,19 +108,14 @@
 - Try a larger model if you have it:
 ```bash
 llama-server --models-yml models.yml --model-id llama-13b  # or any `model_id` defined in `models.yml`
 ```
 
 - Try non-streaming mode by restarting Chatbot UI:
 ```bash
-export LLAMA_STREAM_MODE=1  # 0 to disable streaming
+export LLAMA_STREAM_MODE=0  # 1 to enable streaming
 npm run dev
 ```
 
-## Limitations
-
-- "Regenerate response" is currently not working;
-- IMHO, the prompt/reverse-prompt machanism of LLaMA C++'s interactive mode needs an overhaul. I tried very hard to dance around it but the whole thing is still a hack.
-
 ## Fun facts
 
 I am not fluent in JavaScript at all but I was able to make the changes in Chatbot UI by chatting with [ChatGPT](https://chat.openai.com); no more StackOverflow.
```

### Comparing `llama-server-0.1.0/setup.py` & `llama-server-0.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         "click",
     ]
 
 
 def get_extras_require() -> str:
     req = {
         "dev": [
+            "httpx",
             "pre-commit",
             "pytest",
             "pytest-cov",
             "pytest-xdist",
         ],
     }
     return req
```

