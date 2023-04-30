# Comparing `tmp/llama-server-0.2.0.tar.gz` & `tmp/llama-server-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama-server-0.2.0.tar", last modified: Sun Apr 30 04:57:20 2023, max compression
+gzip compressed data, was "llama-server-0.2.1.tar", last modified: Sun Apr 30 17:13:17 2023, max compression
```

## Comparing `llama-server-0.2.0.tar` & `llama-server-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:57:20.546722 llama-server-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-30 04:57:10.000000 llama-server-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-30 04:57:20.546722 llama-server-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-30 04:57:10.000000 llama-server-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:57:20.542722 llama-server-0.2.0/llama_server/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 04:57:10.000000 llama-server-0.2.0/llama_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:57:20.546722 llama-server-0.2.0/llama_server/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-30 04:57:10.000000 llama-server-0.2.0/llama_server/prompts/alpaca.txt
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-30 04:57:10.000000 llama-server-0.2.0/llama_server/prompts/chat-with-bob.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-30 04:57:10.000000 llama-server-0.2.0/llama_server/prompts/dan.txt
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-30 04:57:10.000000 llama-server-0.2.0/llama_server/prompts/reason-act.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-30 04:57:10.000000 llama-server-0.2.0/llama_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:57:20.542722 llama-server-0.2.0/llama_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-30 04:57:20.000000 llama-server-0.2.0/llama_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-30 04:57:20.000000 llama-server-0.2.0/llama_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 04:57:20.000000 llama-server-0.2.0/llama_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-30 04:57:20.000000 llama-server-0.2.0/llama_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-30 04:57:20.000000 llama-server-0.2.0/llama_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-30 04:57:20.000000 llama-server-0.2.0/llama_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-30 04:57:20.546722 llama-server-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-30 04:57:10.000000 llama-server-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:13:17.934796 llama-server-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-30 17:13:06.000000 llama-server-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-30 17:13:17.934796 llama-server-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-30 17:13:06.000000 llama-server-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:13:17.934796 llama-server-0.2.1/llama_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 17:13:06.000000 llama-server-0.2.1/llama_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:13:17.934796 llama-server-0.2.1/llama_server/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-30 17:13:06.000000 llama-server-0.2.1/llama_server/prompts/alpaca.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-30 17:13:06.000000 llama-server-0.2.1/llama_server/prompts/chat-with-bob.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-30 17:13:06.000000 llama-server-0.2.1/llama_server/prompts/dan.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-30 17:13:06.000000 llama-server-0.2.1/llama_server/prompts/reason-act.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-04-30 17:13:06.000000 llama-server-0.2.1/llama_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:13:17.934796 llama-server-0.2.1/llama_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-30 17:13:17.000000 llama-server-0.2.1/llama_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-30 17:13:17.000000 llama-server-0.2.1/llama_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 17:13:17.000000 llama-server-0.2.1/llama_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-30 17:13:17.000000 llama-server-0.2.1/llama_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-30 17:13:17.000000 llama-server-0.2.1/llama_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-30 17:13:17.000000 llama-server-0.2.1/llama_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-30 17:13:17.934796 llama-server-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-30 17:13:06.000000 llama-server-0.2.1/setup.py
```

### Comparing `llama-server-0.2.0/LICENSE` & `llama-server-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llama-server-0.2.0/PKG-INFO` & `llama-server-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-server
-Version: 0.2.0
+Version: 0.2.1
 Summary: LLaMA Server combines the power of LLaMA C++ with the beauty of Chatbot UI.
 Home-page: https://github.com/nuance1979/llama-server
 Author: Yi Su
 Author-email: nuance@gmail.com
 License: MIT
 Keywords: llama llama.cpp chatbot-ui chatbot
 Classifier: Development Status :: 4 - Beta
```

### Comparing `llama-server-0.2.0/README.md` & `llama-server-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `llama-server-0.2.0/llama_server/prompts/dan.txt` & `llama-server-0.2.1/llama_server/prompts/dan.txt`

 * *Files identical despite different names*

### Comparing `llama-server-0.2.0/llama_server/prompts/reason-act.txt` & `llama-server-0.2.1/llama_server/prompts/reason-act.txt`

 * *Files identical despite different names*

### Comparing `llama-server-0.2.0/llama_server/server.py` & `llama-server-0.2.1/llama_server/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     temperature: float
     stream: bool
 
 
 class Choice(BaseModel):
     message: Optional[Message] = None
     delta: Optional[Message] = None
+    finish_reason: Optional[str] = None
 
 
 class Completion(BaseModel):
     choices: List[Choice]
 
 
 class ModelInfo(BaseModel):
@@ -63,44 +64,52 @@
 logger = None
 model_id = None
 model = None
 
 app = FastAPI()
 
 
-def _chat(user_utt: str) -> Generator[str, None, None]:
-    return model.generate(user_utt, n_predict=256, repeat_penalty=1.0, n_threads=8)
+def _chat(user_utt: str, temperature: float) -> Generator[str, None, None]:
+    return model.generate(
+        user_utt, n_predict=256, repeat_penalty=1.0, n_threads=8, temp=temperature
+    )
 
 
-def chat_stream(user_utt: str) -> Generator[Dict[str, Any], None, None]:
-    for text in _chat(user_utt):
+def chat_stream(
+    user_utt: str, temperature: float
+) -> Generator[Dict[str, Any], None, None]:
+    for text in _chat(user_utt, temperature):
         logger.debug("text: %s", text)
         payload = Completion(
             choices=[Choice(delta=Message(role="assistant", content=text))]
         )
         yield {"event": "event", "data": payload.json()}
-    yield {"event": "event", "data": "[DONE]"}
+    payload = Completion(choices=[Choice(finish_reason="stop")])
+    yield {"event": "event", "data": payload.json()}
 
 
-def chat_nonstream(user_utt: str) -> Completion:
-    assistant_utt = "".join(_chat(user_utt))
+def chat_nonstream(user_utt: str, temperature: float) -> Completion:
+    assistant_utt = "".join(_chat(user_utt, temperature))
     logger.info("assistant: %s", assistant_utt)
     return Completion(
         choices=[Choice(message=Message(role="assistant", content=assistant_utt))]
     )
 
 
 @app.post("/v1/chat/completions")
 def chat(conv: Conversation):
     user_utt = conv.messages[-1].content
-    logger.info("user: %s", user_utt)
+    temperature = conv.temperature
+    logger.info("user: %s temperature: %f", user_utt, temperature)
     if not conv.stream:
-        return chat_nonstream(user_utt)
+        return chat_nonstream(user_utt, temperature)
     else:
-        return EventSourceResponse(chat_stream(user_utt), ping_message_factory=None)
+        return EventSourceResponse(
+            chat_stream(user_utt, temperature), ping_message_factory=None
+        )
 
 
 @app.get("/v1/models")
 def models():
     return ModelList(data=[ModelInfo(id=model_id)])
```

### Comparing `llama-server-0.2.0/llama_server.egg-info/PKG-INFO` & `llama-server-0.2.1/llama_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-server
-Version: 0.2.0
+Version: 0.2.1
 Summary: LLaMA Server combines the power of LLaMA C++ with the beauty of Chatbot UI.
 Home-page: https://github.com/nuance1979/llama-server
 Author: Yi Su
 Author-email: nuance@gmail.com
 License: MIT
 Keywords: llama llama.cpp chatbot-ui chatbot
 Classifier: Development Status :: 4 - Beta
```

### Comparing `llama-server-0.2.0/setup.py` & `llama-server-0.2.1/setup.py`

 * *Files identical despite different names*

