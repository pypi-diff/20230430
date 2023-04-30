# Comparing `tmp/hugchat-0.0.2.tar.gz` & `tmp/hugchat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat-0.0.2.tar", last modified: Thu Apr 27 06:11:52 2023, max compression
+gzip compressed data, was "hugchat-0.0.3.tar", last modified: Sun Apr 30 03:06:28 2023, max compression
```

## Comparing `hugchat-0.0.2.tar` & `hugchat-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 06:11:52.032969 hugchat-0.0.2/
--rw-rw-rw-   0        0        0    35184 2023-04-27 05:43:02.000000 hugchat-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1359 2023-04-27 06:11:52.031969 hugchat-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-04-27 05:40:54.000000 hugchat-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-27 06:11:52.032969 hugchat-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1442 2023-04-27 06:11:48.000000 hugchat-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 06:11:52.002969 hugchat-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 06:11:52.010972 hugchat-0.0.2/src/hugchat/
--rw-rw-rw-   0        0        0     2830 2023-04-27 06:11:23.000000 hugchat-0.0.2/src/hugchat/hugchat.py
-drwxrwxrwx   0        0        0        0 2023-04-27 06:11:52.029969 hugchat-0.0.2/src/hugchat.egg-info/
--rw-rw-rw-   0        0        0     1359 2023-04-27 06:11:51.000000 hugchat-0.0.2/src/hugchat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-27 06:11:51.000000 hugchat-0.0.2/src/hugchat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 06:11:51.000000 hugchat-0.0.2/src/hugchat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-27 06:11:51.000000 hugchat-0.0.2/src/hugchat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-27 06:11:51.000000 hugchat-0.0.2/src/hugchat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 03:06:28.707101 hugchat-0.0.3/
+-rw-rw-rw-   0        0        0    35184 2023-04-27 05:43:02.000000 hugchat-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1705 2023-04-30 03:06:28.706102 hugchat-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      663 2023-04-30 03:05:54.000000 hugchat-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 03:06:28.707101 hugchat-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1442 2023-04-30 03:06:08.000000 hugchat-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 03:06:28.661101 hugchat-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 03:06:28.676103 hugchat-0.0.3/src/hugchat/
+-rw-rw-rw-   0        0        0     3966 2023-04-30 03:04:55.000000 hugchat-0.0.3/src/hugchat/hugchat.py
+drwxrwxrwx   0        0        0        0 2023-04-30 03:06:28.703101 hugchat-0.0.3/src/hugchat.egg-info/
+-rw-rw-rw-   0        0        0     1705 2023-04-30 03:06:28.000000 hugchat-0.0.3/src/hugchat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-30 03:06:28.000000 hugchat-0.0.3/src/hugchat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 03:06:28.000000 hugchat-0.0.3/src/hugchat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 03:06:28.000000 hugchat-0.0.3/src/hugchat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-30 03:06:28.000000 hugchat-0.0.3/src/hugchat.egg-info/top_level.txt
```

### Comparing `hugchat-0.0.2/LICENSE` & `hugchat-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat-0.0.2/PKG-INFO` & `hugchat-0.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.2
+Version: 0.0.3
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -21,19 +21,29 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hugging-chat-api
 HuggingChat Python API
 
-# How to Use?
+[![PyPi](https://img.shields.io/pypi/v/hugchat.svg)](https://pypi.python.org/pypi/hugchat)
+[![Support_Platform](https://img.shields.io/pypi/pyversions/hugchat)](https://pypi.python.org/pypi/hugchat)
 
+- ChatGPT 平替！
+- 无需任何账号，中国大陆的朋友无需梯子
+
+# How to Use
+```bash
+pip install hugchat
 ```
-chatbot = ChatBot()
-chatbot.chat("Hello, I am a robot.")
+
+```py
+from hugchat import hugchat
+chatbot = hugchat.ChatBot()
+print(chatbot.chat("HI"))
 
 # New a conversation (ignore error)
 id = chatbot.new_conversation()
 chatbot.change_conversation(id)
 
 # Get conversation list
 conversation_list = chatbot.get_conversation_list()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hugchat-0.0.2/setup.py` & `hugchat-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 setup(
     name="hugchat",
-    version="0.0.2",
+    version="0.0.3",
     description="A huggingchat python api.",
     long_description=open("README.md", "rt", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Soulter/hugging-chat-api",
     project_urls={
         "Bug Report": "https://github.com/Soulter/hugging-chat-api/issues"
     },
```

### Comparing `hugchat-0.0.2/src/hugchat/hugchat.py` & `hugchat-0.0.3/src/hugchat/hugchat.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from requests import Session
 import json
+import uuid
 
 hf_url = "https://huggingface.co/chat"
 
 
 class ChatBot:
     def __init__(self) -> None:
         self.session = self.get_hc_session()
@@ -33,14 +34,17 @@
                 return json.loads(resp.text)['conversationId']
             except BaseException as e:
                 err_count += 1
                 print(f"[Error] Failed to create new conversation. Retrying... ({err_count})")
                 if err_count > 5:
                     raise e
                 continue
+
+    def get_cookies(self) -> dict:
+        return self.session.cookies.get_dict()
         
 
     def chat(self, text: str, temperature=0.9, top_p=0.95, repetition_penalty=1.2, top_k=50, truncate=1024) -> str:
         if self.now_conversation == "":
             self.now_conversation = self.new_conversation()
         req_json = {
             "inputs": text,
@@ -48,31 +52,51 @@
                 "temperature": temperature,
                 "top_p": top_p,
                 "repetition_penalty": repetition_penalty,
                 "top_k": top_k,
                 "truncate": truncate,
                 "watermark": False,
                 "max_new_tokens": 1024,
-                "stop": ["<|endoftext|>"],
+                "stop": ["</s>"],
                 "return_full_text": False,
                 "stream": True,
-                "options": {"use_cache": False},
-            }
+            },
+            "options": {
+                    "use_cache": False,
+                    "is_retry": False,
+                    "id": str(uuid.uuid4()),
+            },
         }
-        resp = self.session.post(hf_url + f"/conversation/{self.now_conversation}", json=req_json, stream=True)
-        
+        # print(req_json)
+        # print(self.session.cookies.get_dict())
+        # print(f"https://huggingface.co/chat/conversation/{self.now_conversation}")
+        headers = {
+            "Origin": "https://huggingface.co",
+            "Referer": f"https://huggingface.co/chat/conversation/{self.now_conversation}",
+            "Sec-Fetch-Dest": "empty",
+            "Sec-Fetch-Mode": "cors",
+            "Sec-Fetch-Site": "same-origin",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36 Edg/112.0.1722.64",
+            "Content-Type": "application/json",
+            "Accept": "*/*",
+        }
+        resp = self.session.post(hf_url + f"/conversation/{self.now_conversation}", json=req_json, stream=True, headers=headers, cookies=self.session.cookies.get_dict())
+        res_text = ""
         if resp.status_code == 200:
             for line in resp.iter_lines():
                 if line:
                     res = line.decode("utf-8")
                     obj = json.loads(res[1:-1])
                     if "generated_text" in obj:
                         self.conversation_list.append(obj["generated_text"])
-                        return obj["generated_text"]
+                        res_text += obj["generated_text"]
                     elif "error" in obj:
                         raise Exception(obj["error"])
+            return res_text
+        else:
+            raise Exception(f"Failed to chat. Status code: {resp.status_code}")
     
 
 if __name__ == "__main__":
     chatbot = ChatBot()
-    res = chatbot.chat("Hello, I am a robot.")
+    res = chatbot.chat("help me to write a python helloworld program")
     print(res)
```

### Comparing `hugchat-0.0.2/src/hugchat.egg-info/PKG-INFO` & `hugchat-0.0.3/src/hugchat.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.2
+Version: 0.0.3
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -21,19 +21,29 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hugging-chat-api
 HuggingChat Python API
 
-# How to Use?
+[![PyPi](https://img.shields.io/pypi/v/hugchat.svg)](https://pypi.python.org/pypi/hugchat)
+[![Support_Platform](https://img.shields.io/pypi/pyversions/hugchat)](https://pypi.python.org/pypi/hugchat)
 
+- ChatGPT 平替！
+- 无需任何账号，中国大陆的朋友无需梯子
+
+# How to Use
+```bash
+pip install hugchat
 ```
-chatbot = ChatBot()
-chatbot.chat("Hello, I am a robot.")
+
+```py
+from hugchat import hugchat
+chatbot = hugchat.ChatBot()
+print(chatbot.chat("HI"))
 
 # New a conversation (ignore error)
 id = chatbot.new_conversation()
 chatbot.change_conversation(id)
 
 # Get conversation list
 conversation_list = chatbot.get_conversation_list()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

