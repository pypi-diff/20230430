# Comparing `tmp/ipymock-1.0.3.tar.gz` & `tmp/ipymock-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipymock-1.0.3.tar", last modified: Sat Apr 29 09:27:02 2023, max compression
+gzip compressed data, was "ipymock-1.0.4.tar", last modified: Sun Apr 30 09:41:14 2023, max compression
```

## Comparing `ipymock-1.0.3.tar` & `ipymock-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-29 09:27:02.326377 ipymock-1.0.3/
--rw-rw-r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-1.0.3/LICENSE
--rw-rw-r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-1.0.3/MANIFEST.in
--rw-r--r--   0 saintway   (501) staff       (20)    10620 2023-04-29 09:27:02.325906 ipymock-1.0.3/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)     9877 2023-04-29 09:26:04.000000 ipymock-1.0.3/README.md
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-29 09:27:02.322131 ipymock-1.0.3/ipymock/
--rw-rw-r--   0 saintway   (501) staff       (20)     1605 2023-04-29 09:25:44.000000 ipymock-1.0.3/ipymock/__init__.py
--rw-rw-r--   0 saintway   (501) staff       (20)     2454 2023-04-29 09:25:44.000000 ipymock-1.0.3/ipymock/_nbdev.py
--rw-rw-r--   0 saintway   (501) staff       (20)    18079 2023-04-29 09:25:44.000000 ipymock-1.0.3/ipymock/agi.py
--rw-rw-r--   0 saintway   (501) staff       (20)    15390 2023-04-29 09:25:44.000000 ipymock-1.0.3/ipymock/browser.py
--rw-rw-r--   0 saintway   (501) staff       (20)      995 2023-04-29 09:25:44.000000 ipymock-1.0.3/ipymock/llm.py
--rw-rw-r--   0 saintway   (501) staff       (20)     2974 2023-04-29 09:25:44.000000 ipymock-1.0.3/ipymock/reader.py
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-29 09:27:02.324315 ipymock-1.0.3/ipymock.egg-info/
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-29 09:27:02.325183 ipymock-1.0.3/ipymock.egg-info/.ipynb_checkpoints/
--rw-rw-r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-1.0.3/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-1.0.3/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-rw-r--   0 saintway   (501) staff       (20)    10620 2023-04-29 09:27:02.000000 ipymock-1.0.3/ipymock.egg-info/PKG-INFO
--rw-rw-r--   0 saintway   (501) staff       (20)      460 2023-04-29 09:27:02.000000 ipymock-1.0.3/ipymock.egg-info/SOURCES.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-04-29 09:27:02.000000 ipymock-1.0.3/ipymock.egg-info/dependency_links.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-1.0.3/ipymock.egg-info/not-zip-safe
--rw-rw-r--   0 saintway   (501) staff       (20)      129 2023-04-29 09:27:02.000000 ipymock-1.0.3/ipymock.egg-info/requires.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-04-29 09:27:02.000000 ipymock-1.0.3/ipymock.egg-info/top_level.txt
--rw-rw-r--   0 saintway   (501) staff       (20)     2610 2023-04-29 09:06:43.000000 ipymock-1.0.3/settings.ini
--rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-29 09:27:02.326479 ipymock-1.0.3/setup.cfg
--rw-rw-r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-1.0.3/setup.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-30 09:41:14.765576 ipymock-1.0.4/
+-rw-rw-r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-1.0.4/LICENSE
+-rw-rw-r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-1.0.4/MANIFEST.in
+-rw-r--r--   0 saintway   (501) staff       (20)    10620 2023-04-30 09:41:14.765125 ipymock-1.0.4/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)     9877 2023-04-30 09:39:51.000000 ipymock-1.0.4/README.md
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-30 09:41:14.761087 ipymock-1.0.4/ipymock/
+-rw-rw-r--   0 saintway   (501) staff       (20)     1605 2023-04-30 09:39:30.000000 ipymock-1.0.4/ipymock/__init__.py
+-rw-rw-r--   0 saintway   (501) staff       (20)     2454 2023-04-30 09:39:30.000000 ipymock-1.0.4/ipymock/_nbdev.py
+-rw-rw-r--   0 saintway   (501) staff       (20)    18079 2023-04-30 09:39:30.000000 ipymock-1.0.4/ipymock/agi.py
+-rw-rw-r--   0 saintway   (501) staff       (20)    16107 2023-04-30 09:39:30.000000 ipymock-1.0.4/ipymock/browser.py
+-rw-rw-r--   0 saintway   (501) staff       (20)      995 2023-04-30 09:39:30.000000 ipymock-1.0.4/ipymock/llm.py
+-rw-rw-r--   0 saintway   (501) staff       (20)     2974 2023-04-30 09:39:30.000000 ipymock-1.0.4/ipymock/reader.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-30 09:41:14.763519 ipymock-1.0.4/ipymock.egg-info/
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-30 09:41:14.764442 ipymock-1.0.4/ipymock.egg-info/.ipynb_checkpoints/
+-rw-rw-r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-1.0.4/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-1.0.4/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)    10620 2023-04-30 09:41:14.000000 ipymock-1.0.4/ipymock.egg-info/PKG-INFO
+-rw-rw-r--   0 saintway   (501) staff       (20)      460 2023-04-30 09:41:14.000000 ipymock-1.0.4/ipymock.egg-info/SOURCES.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-04-30 09:41:14.000000 ipymock-1.0.4/ipymock.egg-info/dependency_links.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-1.0.4/ipymock.egg-info/not-zip-safe
+-rw-rw-r--   0 saintway   (501) staff       (20)      129 2023-04-30 09:41:14.000000 ipymock-1.0.4/ipymock.egg-info/requires.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-04-30 09:41:14.000000 ipymock-1.0.4/ipymock.egg-info/top_level.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)     2610 2023-04-30 08:37:11.000000 ipymock-1.0.4/settings.ini
+-rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-30 09:41:14.765661 ipymock-1.0.4/setup.cfg
+-rw-rw-r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-1.0.4/setup.py
```

### Comparing `ipymock-1.0.3/LICENSE` & `ipymock-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.3/PKG-INFO` & `ipymock-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Tool that Allows You Run PyTest within Jupyter Notebook Cells
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipymock-1.0.3/README.md` & `ipymock-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.3/ipymock/__init__.py` & `ipymock-1.0.4/ipymock/__init__.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.3/ipymock/_nbdev.py` & `ipymock-1.0.4/ipymock/_nbdev.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.3/ipymock/agi.py` & `ipymock-1.0.4/ipymock/agi.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.3/ipymock/browser.py` & `ipymock-1.0.4/ipymock/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 # Internal Cell
 from queue import Queue
 
 class Common:
     chat_gpt_base_url = 'http://127.0.0.1:8080'
     access_token = None
 
-    chat_gpt_model = 'gpt-3.5-turbo'
+    chat_gpt_model = 'text-davinci-002-render-sha'
+    role_system = 'system'
     role_user = 'user'
     role_assistant = 'assistant'
 
     question_answer_map = {}
     message_channel = Queue()
     exit_for_loop_channel = Queue()
     response_text_channel = Queue()
@@ -39,14 +40,19 @@
 # Cell
 def get_conversations():
     response = requests.get(f'{common.chat_gpt_base_url}/conversations?offset=0&limit=100', headers = {'Authorization': common.access_token})
     return response.json()
 
 def get_conversation(conversation_id):
     response = requests.get(f'{common.chat_gpt_base_url}/conversation/{conversation_id}', headers = {'Authorization': common.access_token})
+
+    if response.status_code >= 400:
+        sys.stderr.write(f'Error Status Code: {response.status_code}\n{response.text}\n')
+    response.raise_for_status()
+
     conversation = response.json()
     current_node = conversation['current_node']
     try:
         handle_conversation_detail(current_node, conversation['mapping'])
     except RecursionError as errr:
         sys.stderr.write(f'Error Recursing: {errr}\n')
     common.exit_for_loop_channel.put(True)
@@ -72,59 +78,63 @@
         except requests.exceptions.ConnectionError as errc:
             sys.stderr.write(f'Error Connecting: {errc}\n')
 
     if common.conversation_id == '' or common.parent_message_id == '':
         common.conversation_id = ''
         common.parent_message_id = str(uuid.uuid4())
 
-    if isinstance(prompt, str):
-        prompt = [{'role': common.role_user, 'parts': [prompt]}]
-    if isinstance(prompt, dict):
-        prompt = [prompt]
     if isinstance(prompt, list):
         raw_prompt = prompt
         prompt = []
         parts = []
         for item in raw_prompt:
-            if isinstance(item, dict):
+            if isinstance(item, dict) and 'parts' in item:
+                if common.conversation_id == '' and 'role' in item and item['role'] == common.role_system:
+                    sys.stderr.write(f'Error Messaging: role system is not allowed in the first prompt. It is changed to role user.\n')
+                    item['role'] = common.role_user
                 prompt.append(item)
             else:
                 parts.append(str(item))
         prompt.append({'role': common.role_user, 'parts': parts})
+    elif isinstance(prompt, dict) and 'parts' in prompt:
+        prompt = [prompt]
+    else:
+        prompt = [{'role': common.role_user, 'parts': [str(prompt)]}]
 
     post_data = {
         'action': 'next',
+        'history_and_training_disabled': False,
         'messages': [{
             'id': str(uuid.uuid4()),
             'author': {
-                'role': msg['role'],
+                'role': msg.get('role', common.role_user),
             },
-            'role': msg['role'],
+            'role': msg.get('role', common.role_user),
             'content': {
                 'content_type': 'text',
                 'parts': msg['parts'],
             },
         } for msg in prompt],
         'model': common.chat_gpt_model,
-        'continue_text': '',
+        'timezone_offset_min': -540,
     }
     if common.conversation_id != '':
         post_data['conversation_id'] = common.conversation_id
     if common.parent_message_id != '':
         post_data['parent_message_id'] = common.parent_message_id
 
     response = requests.post(
         f'{common.chat_gpt_base_url}/conversation',
         headers = {
-            'Authorization': common.access_token,
             'Content-Type': 'application/json',
-            'Accept': 'text/event-stream'
+            'Accept': 'text/event-stream',
+            'Authorization': f'Bearer {common.access_token}',
         },
         data = json.dumps(post_data),
-        stream=True
+        stream=True,
     )
 
     temp_conversation_id = ''
     for line in response.iter_lines():
         if not line.startswith(b'data: '):
             continue
 
@@ -136,21 +146,21 @@
             make_conversation_response = json.loads(line.decode('utf-8')[len('data: '):])
         except json.decoder.JSONDecodeError as err:
             sys.stderr.write(f'Error JSON Decoding: line = {line}\n')
             continue
         if make_conversation_response is None:
             continue
         try:
-            parts = make_conversation_response['message']['content']['parts']
+            parts = ''.join(make_conversation_response['message']['content']['parts']).strip()
         except TypeError as err:
             sys.stderr.write(f'TypeError: {err}\nline = {line}\n')
             continue
-        if len(parts) > 0:
-            common.response_text_channel.put(parts[0])
-            yield parts[0]
+        if parts != '':
+            common.response_text_channel.put(parts)
+            yield parts
         if common.conversation_id == '':
             temp_conversation_id = make_conversation_response['conversation_id']
         common.parent_message_id = make_conversation_response['message']['id']
         if make_conversation_response['message']['end_turn'] == True:
             common.conversation_done_channel.put(True)
             continue
 
@@ -238,17 +248,18 @@
         return [attributize(item) for item in obj]
     return obj
 
 def delta(prompt):
     id = ''.join(
         random.choices(string.ascii_letters + string.digits, k = 29)
     )
-    res = ''
     wait_second = 1
     while True:
+        res = ''
+        response = ''
         try:
             for response in start_conversation(prompt):
                 yield attributize({
                     'choices': [
                         {
                             'index': 0,
                             'logprobs': None,
@@ -349,17 +360,18 @@
         },
     })
 
 def chat_delta(prompt):
     id = ''.join(
         random.choices(string.ascii_letters + string.digits, k = 29)
     )
-    res = ''
     wait_second = 1
     while True:
+        res = ''
+        response = ''
         try:
             for response in start_conversation(prompt):
                 yield attributize({
                     'choices': [
                         {
                             'index': 0,
                             'delta': {
@@ -394,17 +406,18 @@
             )
             time.sleep(wait_second)
             wait_second *= 2
             continue
         break
 
 def mock_chat_create(*args, **kwargs):
-    summarized_prompt = []
+    summarized_prompt = ''
     for message in kwargs['messages']:
-        summarized_prompt.append({'role': message['role'], 'parts': [message['content']]})
+        summarized_prompt += f"{message['role']}:\n\n{message['content']}\n\n\n"
+    summarized_prompt.strip()
 
     if kwargs.get('stream', False):
         return chat_delta(summarized_prompt)
 
     response = ''
     wait_second = 1
     while True:
```

### Comparing `ipymock-1.0.3/ipymock/llm.py` & `ipymock-1.0.4/ipymock/llm.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.3/ipymock/reader.py` & `ipymock-1.0.4/ipymock/reader.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.3/ipymock.egg-info/PKG-INFO` & `ipymock-1.0.4/ipymock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Tool that Allows You Run PyTest within Jupyter Notebook Cells
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipymock-1.0.3/settings.ini` & `ipymock-1.0.4/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 user = seii-saintway
 description = A Tool that Allows You Run PyTest within Jupyter Notebook Cells
 keywords = pytest interactive jupyter
 author = andrew
 author_email = andrew.saintway@gmail.com
 copyright = 2023 onwards, Neuro Spirit, DAO.
 branch = main
-version = 1.0.3
+version = 1.0.4
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `ipymock-1.0.3/setup.py` & `ipymock-1.0.4/setup.py`

 * *Files identical despite different names*

