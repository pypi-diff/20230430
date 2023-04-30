# Comparing `tmp/gpt4free-0.1.2.tar.gz` & `tmp/gpt4free-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\Progamming Project\gpt4free python package\dist\.tmp-t73nbx1n\gpt4free-0.1.2.tar", last modified: Mon May  1 01:05:46 2023, max compression
+gzip compressed data, was "F:\Progamming Project\gpt4free python package\dist\.tmp-spsifcfe\gpt4free-0.1.3.tar", last modified: Mon May  1 02:38:30 2023, max compression
```

## Comparing `gpt4free-0.1.2.tar` & `gpt4free-0.1.3.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 01:05:46.183970 gpt4free-0.1.2/
--rw-rw-rw-   0        0        0      171 2023-04-27 05:47:31.000000 gpt4free-0.1.2/AUTHORS.md
--rw-rw-rw-   0        0        0     3654 2023-04-27 05:47:31.000000 gpt4free-0.1.2/CONTRIBUTING.md
--rw-rw-rw-   0        0        0        0 2023-04-27 08:27:03.000000 gpt4free-0.1.2/HISTORY.md
--rw-rw-rw-   0        0        0     1739 2023-04-27 05:47:31.000000 gpt4free-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      209 2023-04-27 07:44:37.000000 gpt4free-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1440 2023-05-01 01:05:46.183970 gpt4free-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-04-27 08:34:50.000000 gpt4free-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 01:05:46.161823 gpt4free-0.1.2/gpt4free/
--rw-rw-rw-   0        0        0      136 2023-05-01 01:05:38.000000 gpt4free-0.1.2/gpt4free/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 01:05:46.171960 gpt4free-0.1.2/gpt4free/forefront/
--rw-rw-rw-   0        0        0     5330 2023-04-27 08:09:30.000000 gpt4free-0.1.2/gpt4free/forefront/__init__.py
--rw-rw-rw-   0        0        0     2147 2023-04-27 05:59:26.000000 gpt4free-0.1.2/gpt4free/forefront/mail.py
--rw-rw-rw-   0        0        0     1795 2023-04-27 05:59:26.000000 gpt4free-0.1.2/gpt4free/forefront/typing.py
-drwxrwxrwx   0        0        0        0 2023-05-01 01:05:46.174964 gpt4free-0.1.2/gpt4free/gui/
--rw-rw-rw-   0        0        0        0 2023-04-27 08:22:19.000000 gpt4free-0.1.2/gpt4free/gui/__init__.py
--rw-rw-rw-   0        0        0     1535 2023-04-27 05:59:26.000000 gpt4free-0.1.2/gpt4free/gui/streamlit_app.py
-drwxrwxrwx   0        0        0        0 2023-05-01 01:05:46.179966 gpt4free-0.1.2/gpt4free/quora/
--rw-rw-rw-   0        0        0    22029 2023-04-27 08:09:31.000000 gpt4free-0.1.2/gpt4free/quora/__init__.py
--rw-rw-rw-   0        0        0    19819 2023-04-27 05:59:26.000000 gpt4free-0.1.2/gpt4free/quora/api.py
-drwxrwxrwx   0        0        0        0 2023-05-01 01:05:46.180963 gpt4free-0.1.2/gpt4free/quora/graphql/
--rw-rw-rw-   0        0        0        0 2023-04-27 05:59:26.000000 gpt4free-0.1.2/gpt4free/quora/graphql/__init__.py
--rw-rw-rw-   0        0        0     2391 2023-04-27 05:59:26.000000 gpt4free-0.1.2/gpt4free/quora/mail.py
-drwxrwxrwx   0        0        0        0 2023-05-01 01:05:46.181963 gpt4free-0.1.2/gpt4free/theb/
--rw-rw-rw-   0        0        0     1699 2023-04-27 05:59:26.000000 gpt4free-0.1.2/gpt4free/theb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 01:05:46.182964 gpt4free-0.1.2/gpt4free/you/
--rw-rw-rw-   0        0        0     3716 2023-04-27 05:59:26.000000 gpt4free-0.1.2/gpt4free/you/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 01:05:46.168817 gpt4free-0.1.2/gpt4free.egg-info/
--rw-rw-rw-   0        0        0     1440 2023-05-01 01:05:46.000000 gpt4free-0.1.2/gpt4free.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-05-01 01:05:46.000000 gpt4free-0.1.2/gpt4free.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 01:05:46.000000 gpt4free-0.1.2/gpt4free.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-01 01:05:45.000000 gpt4free-0.1.2/gpt4free.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      124 2023-05-01 01:05:46.000000 gpt4free-0.1.2/gpt4free.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-01 01:05:46.000000 gpt4free-0.1.2/gpt4free.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      451 2023-05-01 01:05:46.184983 gpt4free-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2116 2023-05-01 01:05:36.000000 gpt4free-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.378336 gpt4free-0.1.3/
+-rw-rw-rw-   0        0        0      171 2023-04-27 05:47:31.000000 gpt4free-0.1.3/AUTHORS.md
+-rw-rw-rw-   0        0        0     3654 2023-04-27 05:47:31.000000 gpt4free-0.1.3/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0        0 2023-04-27 08:27:03.000000 gpt4free-0.1.3/HISTORY.md
+-rw-rw-rw-   0        0        0     1739 2023-04-27 05:47:31.000000 gpt4free-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      209 2023-04-27 07:44:37.000000 gpt4free-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1440 2023-05-01 02:38:30.378336 gpt4free-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-04-27 08:34:50.000000 gpt4free-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.353337 gpt4free-0.1.3/gpt4free/
+-rw-rw-rw-   0        0        0     2659 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.363329 gpt4free-0.1.3/gpt4free/cocalc/
+-rw-rw-rw-   0        0        0     2461 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/cocalc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.366330 gpt4free-0.1.3/gpt4free/forefront/
+-rw-rw-rw-   0        0        0     6503 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/forefront/__init__.py
+-rw-rw-rw-   0        0        0      437 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/forefront/typing.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.370332 gpt4free-0.1.3/gpt4free/quora/
+-rw-rw-rw-   0        0        0    21139 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/quora/__init__.py
+-rw-rw-rw-   0        0        0    19700 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/quora/api.py
+-rw-rw-rw-   0        0        0     1464 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/quora/backup-mail.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.372333 gpt4free-0.1.3/gpt4free/quora/graphql/
+-rw-rw-rw-   0        0        0        0 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/quora/graphql/__init__.py
+-rw-rw-rw-   0        0        0     2359 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/quora/mail.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.375333 gpt4free-0.1.3/gpt4free/theb/
+-rw-rw-rw-   0        0        0     1887 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/theb/__init__.py
+-rw-rw-rw-   0        0        0      106 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/theb/theb_test.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.376333 gpt4free-0.1.3/gpt4free/usesless/
+-rw-rw-rw-   0        0        0     1744 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/usesless/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.377335 gpt4free-0.1.3/gpt4free/you/
+-rw-rw-rw-   0        0        0     4037 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/you/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.362341 gpt4free-0.1.3/gpt4free.egg-info/
+-rw-rw-rw-   0        0        0     1440 2023-05-01 02:38:30.000000 gpt4free-0.1.3/gpt4free.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2023-05-01 02:38:30.000000 gpt4free-0.1.3/gpt4free.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 02:38:30.000000 gpt4free-0.1.3/gpt4free.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-01 02:38:29.000000 gpt4free-0.1.3/gpt4free.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      142 2023-05-01 02:38:30.000000 gpt4free-0.1.3/gpt4free.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-01 02:38:30.000000 gpt4free-0.1.3/gpt4free.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      451 2023-05-01 02:38:30.379330 gpt4free-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2147 2023-05-01 02:37:59.000000 gpt4free-0.1.3/setup.py
```

### Comparing `gpt4free-0.1.2/CONTRIBUTING.md` & `gpt4free-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.2/LICENSE` & `gpt4free-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.2/PKG-INFO` & `gpt4free-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4free
-Version: 0.1.2
+Version: 0.1.3
 Summary: decentralising the Ai Industry, free gpt-4/3.5 scripts through several reverse engineered api's
 Home-page: https://github.com/rzashakeri/gpt4free
 Author: Reza Shakeri
 Author-email: rzashakeri@gmail.com
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/rzashakeri/gpt4free
 Project-URL: Issue tracker, https://github.com/rzashakeri/gpt4free/issues
```

### Comparing `gpt4free-0.1.2/gpt4free/quora/__init__.py` & `gpt4free-0.1.3/gpt4free/quora/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,495 +1,477 @@
-import json
-from datetime import datetime
-from hashlib import md5
-from json import dumps
-from pathlib import Path
-from random import choice, choices, randint
-from re import search, findall
-from string import ascii_letters, digits
-from typing import Optional, Union
-from urllib.parse import unquote
-
-import selenium.webdriver.support.expected_conditions as EC
-from fake_useragent import UserAgent
-from pypasser import reCaptchaV3
-from requests import Session
-from selenium.webdriver import Firefox, Chrome, FirefoxOptions, ChromeOptions
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support.wait import WebDriverWait
-from tls_client import Session as TLS
-
-from gpt4free.quora.api import Client as PoeClient
-from gpt4free.quora.mail import Emailnator
-
-SELENIUM_WEB_DRIVER_ERROR_MSG = b'''The error message you are receiving is due to the `geckodriver` executable not
-being found in your system\'s PATH. To resolve this issue, you need to download the geckodriver and add its location
-to your system\'s PATH.\n\nHere are the steps to resolve the issue:\n\n1. Download the geckodriver for your platform
-(Windows, macOS, or Linux) from the following link: https://github.com/mozilla/geckodriver/releases\n\n2. Extract the
-downloaded archive and locate the geckodriver executable.\n\n3. Add the geckodriver executable to your system\'s
-PATH.\n\nFor macOS and Linux:\n\n- Open a terminal window.\n- Move the geckodriver executable to a directory that is
-already in your PATH, or create a new directory and add it to your PATH:\n\n```bash\n# Example: Move geckodriver to
-/usr/local/bin\nmv /path/to/your/geckodriver /usr/local/bin\n```\n\n- If you created a new directory, add it to your
-PATH:\n\n```bash\n# Example: Add a new directory to PATH\nexport PATH=$PATH:/path/to/your/directory\n```\n\nFor
-Windows:\n\n- Right-click on "My Computer" or "This PC" and select "Properties".\n- Click on "Advanced system
-settings".\n- Click on the "Environment Variables" button.\n- In the "System variables" section, find the "Path"
-variable, select it, and click "Edit".\n- Click "New" and add the path to the directory containing the geckodriver
-executable.\n\nAfter adding the geckodriver to your PATH, restart your terminal or command prompt and try running
-your script again. The error should be resolved.'''
-
-# from twocaptcha import TwoCaptcha
-# solver = TwoCaptcha('72747bf24a9d89b4dcc1b24875efd358')
-
-MODELS = {
-    'Sage': 'capybara',
-    'GPT-4': 'beaver',
-    'Claude+': 'a2_2',
-    'Claude-instant': 'a2',
-    'ChatGPT': 'chinchilla',
-    'Dragonfly': 'nutria',
-    'NeevaAI': 'hutia',
-}
-
-
-def extract_formkey(html):
-    script_regex = r'<script>if\(.+\)throw new Error;(.+)</script>'
-    script_text = search(script_regex, html).group(1)
-    key_regex = r'var .="([0-9a-f]+)",'
-    key_text = search(key_regex, script_text).group(1)
-    cipher_regex = r'.\[(\d+)\]=.\[(\d+)\]'
-    cipher_pairs = findall(cipher_regex, script_text)
-
-    formkey_list = [''] * len(cipher_pairs)
-    for pair in cipher_pairs:
-        formkey_index, key_index = map(int, pair)
-        formkey_list[formkey_index] = key_text[key_index]
-    formkey = ''.join(formkey_list)
-
-    return formkey
-
-
-class PoeResponse:
-    class Completion:
-        class Choices:
-            def __init__(self, choice: dict) -> None:
-                self.text = choice['text']
-                self.content = self.text.encode()
-                self.index = choice['index']
-                self.logprobs = choice['logprobs']
-                self.finish_reason = choice['finish_reason']
-
-            def __repr__(self) -> str:
-                return f'''<__main__.APIResponse.Completion.Choices(\n    text           = {self.text.encode()},\n    index          = {self.index},\n    logprobs       = {self.logprobs},\n    finish_reason  = {self.finish_reason})object at 0x1337>'''
-
-        def __init__(self, choices: dict) -> None:
-            self.choices = [self.Choices(choice) for choice in choices]
-
-    class Usage:
-        def __init__(self, usage_dict: dict) -> None:
-            self.prompt_tokens = usage_dict['prompt_tokens']
-            self.completion_tokens = usage_dict['completion_tokens']
-            self.total_tokens = usage_dict['total_tokens']
-
-        def __repr__(self):
-            return f'''<__main__.APIResponse.Usage(\n    prompt_tokens      = {self.prompt_tokens},\n    completion_tokens  = {self.completion_tokens},\n    total_tokens       = {self.total_tokens})object at 0x1337>'''
-
-    def __init__(self, response_dict: dict) -> None:
-        self.response_dict = response_dict
-        self.id = response_dict['id']
-        self.object = response_dict['object']
-        self.created = response_dict['created']
-        self.model = response_dict['model']
-        self.completion = self.Completion(response_dict['choices'])
-        self.usage = self.Usage(response_dict['usage'])
-
-    def json(self) -> dict:
-        return self.response_dict
-
-
-class ModelResponse:
-    def __init__(self, json_response: dict) -> None:
-        self.id = json_response['data']['poeBotCreate']['bot']['id']
-        self.name = json_response['data']['poeBotCreate']['bot']['displayName']
-        self.limit = json_response['data']['poeBotCreate']['bot']['messageLimit']['dailyLimit']
-        self.deleted = json_response['data']['poeBotCreate']['bot']['deletionState']
-
-
-class Model:
-    @staticmethod
-    def create(
-            token: str,
-            model: str = 'gpt-3.5-turbo',  # claude-instant
-            system_prompt: str = 'You are ChatGPT a large language model developed by Openai. Answer as consisely as possible',
-            description: str = 'gpt-3.5 language model from openai, skidded by poe.com',
-            handle: str = None,
-    ) -> ModelResponse:
-        models = {
-            'gpt-3.5-turbo': 'chinchilla',
-            'claude-instant-v1.0': 'a2',
-            'gpt-4': 'beaver',
-        }
-
-        if not handle:
-            handle = f'gptx{randint(1111111, 9999999)}'
-
-        client = Session()
-        client.cookies['p-b'] = token
-
-        formkey = extract_formkey(client.get('https://poe.com').text)
-        settings = client.get('https://poe.com/api/settings').json()
-
-        client.headers = {
-            'host': 'poe.com',
-            'origin': 'https://poe.com',
-            'referer': 'https://poe.com/',
-            'poe-formkey': formkey,
-            'poe-tchannel': settings['tchannelData']['channel'],
-            'user-agent': UserAgent().random,
-            'connection': 'keep-alive',
-            'sec-ch-ua': '"Chromium";v="112", "Google Chrome";v="112", "Not:A-Brand";v="99"',
-            'sec-ch-ua-mobile': '?0',
-            'sec-ch-ua-platform': '"macOS"',
-            'content-type': 'application/json',
-            'sec-fetch-site': 'same-origin',
-            'sec-fetch-mode': 'cors',
-            'sec-fetch-dest': 'empty',
-            'accept': '*/*',
-            'accept-encoding': 'gzip, deflate, br',
-            'accept-language': 'en-GB,en-US;q=0.9,en;q=0.8',
-        }
-
-        payload = dumps(
-            separators=(',', ':'),
-            obj={
-                'queryName': 'CreateBotMain_poeBotCreate_Mutation',
-                'variables': {
-                    'model': models[model],
-                    'handle': handle,
-                    'prompt': system_prompt,
-                    'isPromptPublic': True,
-                    'introduction': '',
-                    'description': description,
-                    'profilePictureUrl': 'https://qph.fs.quoracdn.net/main-qimg-24e0b480dcd946e1cc6728802c5128b6',
-                    'apiUrl': None,
-                    'apiKey': ''.join(choices(ascii_letters + digits, k=32)),
-                    'isApiBot': False,
-                    'hasLinkification': False,
-                    'hasMarkdownRendering': False,
-                    'hasSuggestedReplies': False,
-                    'isPrivateBot': False,
-                },
-                'query': 'mutation CreateBotMain_poeBotCreate_Mutation(\n  $model: String!\n  $handle: String!\n  $prompt: String!\n  $isPromptPublic: Boolean!\n  $introduction: String!\n  $description: String!\n  $profilePictureUrl: String\n  $apiUrl: String\n  $apiKey: String\n  $isApiBot: Boolean\n  $hasLinkification: Boolean\n  $hasMarkdownRendering: Boolean\n  $hasSuggestedReplies: Boolean\n  $isPrivateBot: Boolean\n) {\n  poeBotCreate(model: $model, handle: $handle, promptPlaintext: $prompt, isPromptPublic: $isPromptPublic, introduction: $introduction, description: $description, profilePicture: $profilePictureUrl, apiUrl: $apiUrl, apiKey: $apiKey, isApiBot: $isApiBot, hasLinkification: $hasLinkification, hasMarkdownRendering: $hasMarkdownRendering, hasSuggestedReplies: $hasSuggestedReplies, isPrivateBot: $isPrivateBot) {\n    status\n    bot {\n      id\n      ...BotHeader_bot\n    }\n  }\n}\n\nfragment BotHeader_bot on Bot {\n  displayName\n  messageLimit {\n    dailyLimit\n  }\n  ...BotImage_bot\n  ...BotLink_bot\n  ...IdAnnotation_node\n  ...botHelpers_useViewerCanAccessPrivateBot\n  ...botHelpers_useDeletion_bot\n}\n\nfragment BotImage_bot on Bot {\n  displayName\n  ...botHelpers_useDeletion_bot\n  ...BotImage_useProfileImage_bot\n}\n\nfragment BotImage_useProfileImage_bot on Bot {\n  image {\n    __typename\n    ... on LocalBotImage {\n      localName\n    }\n    ... on UrlBotImage {\n      url\n    }\n  }\n  ...botHelpers_useDeletion_bot\n}\n\nfragment BotLink_bot on Bot {\n  displayName\n}\n\nfragment IdAnnotation_node on Node {\n  __isNode: __typename\n  id\n}\n\nfragment botHelpers_useDeletion_bot on Bot {\n  deletionState\n}\n\nfragment botHelpers_useViewerCanAccessPrivateBot on Bot {\n  isPrivateBot\n  viewerIsCreator\n}\n',
-            },
-        )
-
-        base_string = payload + client.headers['poe-formkey'] + 'WpuLMiXEKKE98j56k'
-        client.headers['poe-tag-id'] = md5(base_string.encode()).hexdigest()
-
-        response = client.post('https://poe.com/api/gql_POST', data=payload)
-
-        if 'success' not in response.text:
-            raise Exception(
-                '''
-                Bot creation Failed
-                !! Important !!
-                Bot creation was not enabled on this account
-                please use: quora.Account.create with enable_bot_creation set to True
-            '''
-            )
-
-        return ModelResponse(response.json())
-
-
-class Account:
-    @staticmethod
-    def create(
-            proxy: Optional[str] = None,
-            logging: bool = False,
-            enable_bot_creation: bool = False,
-    ):
-        client = TLS(client_identifier='chrome110')
-        client.proxies = {'http': f'http://{proxy}', 'https': f'http://{proxy}'} if proxy else None
-
-        mail_client = Emailnator()
-        mail_address = mail_client.get_mail()
-
-        if logging:
-            print('email', mail_address)
-
-        client.headers = {
-            'authority': 'poe.com',
-            'accept': '*/*',
-            'accept-language': 'en,fr-FR;q=0.9,fr;q=0.8,es-ES;q=0.7,es;q=0.6,en-US;q=0.5,am;q=0.4,de;q=0.3',
-            'content-type': 'application/json',
-            'origin': 'https://poe.com',
-            'poe-tag-id': 'null',
-            'referer': 'https://poe.com/login',
-            'sec-ch-ua': '"Chromium";v="112", "Google Chrome";v="112", "Not:A-Brand";v="99"',
-            'sec-ch-ua-mobile': '?0',
-            'sec-ch-ua-platform': '"macOS"',
-            'sec-fetch-dest': 'empty',
-            'sec-fetch-mode': 'cors',
-            'sec-fetch-site': 'same-origin',
-            'user-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
-            'poe-formkey': extract_formkey(client.get('https://poe.com/login').text),
-            'poe-tchannel': client.get('https://poe.com/api/settings').json()['tchannelData']['channel'],
-        }
-
-        token = reCaptchaV3(
-            'https://www.recaptcha.net/recaptcha/enterprise/anchor?ar=1&k=6LflhEElAAAAAI_ewVwRWI9hsyV4mbZnYAslSvlG&co=aHR0cHM6Ly9wb2UuY29tOjQ0Mw..&hl=en&v=4PnKmGB9wRHh1i04o7YUICeI&size=invisible&cb=bi6ivxoskyal'
-        )
-        # token = solver.recaptcha(sitekey='6LflhEElAAAAAI_ewVwRWI9hsyV4mbZnYAslSvlG',
-        #     url        = 'https://poe.com/login?redirect_url=%2F',
-        #     version    = 'v3',
-        #     enterprise = 1,
-        #     invisible  = 1,
-        #     action     = 'login',)['code']
-
-        payload = dumps(
-            separators=(',', ':'),
-            obj={
-                'queryName': 'MainSignupLoginSection_sendVerificationCodeMutation_Mutation',
-                'variables': {
-                    'emailAddress': mail_address,
-                    'phoneNumber': None,
-                    'recaptchaToken': token,
-                },
-                'query': 'mutation MainSignupLoginSection_sendVerificationCodeMutation_Mutation(\n  $emailAddress: String\n  $phoneNumber: String\n  $recaptchaToken: String\n) {\n  sendVerificationCode(verificationReason: login, emailAddress: $emailAddress, phoneNumber: $phoneNumber, recaptchaToken: $recaptchaToken) {\n    status\n    errorMessage\n  }\n}\n',
-            },
-        )
-
-        base_string = payload + client.headers['poe-formkey'] + 'WpuLMiXEKKE98j56k'
-        client.headers['poe-tag-id'] = md5(base_string.encode()).hexdigest()
-
-        print(dumps(client.headers, indent=4))
-
-        response = client.post('https://poe.com/api/gql_POST', data=payload)
-
-        if 'automated_request_detected' in response.text:
-            print('please try using a proxy / wait for fix')
-
-        if 'Bad Request' in response.text:
-            if logging:
-                print('bad request, retrying...', response.json())
-            quit()
-
-        if logging:
-            print('send_code', response.json())
-
-        mail_content = mail_client.get_message()
-        mail_token = findall(r';">(\d{6,7})</div>', mail_content)[0]
-
-        if logging:
-            print('code', mail_token)
-
-        payload = dumps(
-            separators=(',', ':'),
-            obj={
-                'queryName': 'SignupOrLoginWithCodeSection_signupWithVerificationCodeMutation_Mutation',
-                'variables': {
-                    'verificationCode': str(mail_token),
-                    'emailAddress': mail_address,
-                    'phoneNumber': None,
-                },
-                'query': 'mutation SignupOrLoginWithCodeSection_signupWithVerificationCodeMutation_Mutation(\n  $verificationCode: String!\n  $emailAddress: String\n  $phoneNumber: String\n) {\n  signupWithVerificationCode(verificationCode: $verificationCode, emailAddress: $emailAddress, phoneNumber: $phoneNumber) {\n    status\n    errorMessage\n  }\n}\n',
-            },
-        )
-
-        base_string = payload + client.headers['poe-formkey'] + 'WpuLMiXEKKE98j56k'
-        client.headers['poe-tag-id'] = md5(base_string.encode()).hexdigest()
-
-        response = client.post('https://poe.com/api/gql_POST', data=payload)
-        if logging:
-            print('verify_code', response.json())
-
-    def get(self):
-        cookies = open(Path(__file__).resolve().parent / 'cookies.txt', 'r').read().splitlines()
-        return choice(cookies)
-
-
-class StreamingCompletion:
-    @staticmethod
-    def create(
-            model: str = 'gpt-4',
-            custom_model: bool = None,
-            prompt: str = 'hello world',
-            token: str = '',
-    ):
-        _model = MODELS[model] if not custom_model else custom_model
-
-        client = PoeClient(token)
-
-        for chunk in client.send_message(_model, prompt):
-            yield PoeResponse(
-                {
-                    'id': chunk['messageId'],
-                    'object': 'text_completion',
-                    'created': chunk['creationTime'],
-                    'model': _model,
-                    'choices': [
-                        {
-                            'text': chunk['text_new'],
-                            'index': 0,
-                            'logprobs': None,
-                            'finish_reason': 'stop',
-                        }
-                    ],
-                    'usage': {
-                        'prompt_tokens': len(prompt),
-                        'completion_tokens': len(chunk['text_new']),
-                        'total_tokens': len(prompt) + len(chunk['text_new']),
-                    },
-                }
-            )
-
-
-class Completion:
-    def create(
-            model: str = 'gpt-4',
-            custom_model: str = None,
-            prompt: str = 'hello world',
-            token: str = '',
-    ):
-        models = {
-            'sage': 'capybara',
-            'gpt-4': 'beaver',
-            'claude-v1.2': 'a2_2',
-            'claude-instant-v1.0': 'a2',
-            'gpt-3.5-turbo': 'chinchilla',
-        }
-
-        _model = models[model] if not custom_model else custom_model
-
-        client = PoeClient(token)
-
-        for chunk in client.send_message(_model, prompt):
-            pass
-
-        return PoeResponse(
-            {
-                'id': chunk['messageId'],
-                'object': 'text_completion',
-                'created': chunk['creationTime'],
-                'model': _model,
-                'choices': [
-                    {
-                        'text': chunk['text'],
-                        'index': 0,
-                        'logprobs': None,
-                        'finish_reason': 'stop',
-                    }
-                ],
-                'usage': {
-                    'prompt_tokens': len(prompt),
-                    'completion_tokens': len(chunk['text']),
-                    'total_tokens': len(prompt) + len(chunk['text']),
-                },
-            }
-        )
-
-
-class Poe:
-    def __init__(
-            self,
-            model: str = 'ChatGPT',
-            driver: str = 'firefox',
-            download_driver: bool = False,
-            driver_path: Optional[str] = None,
-            cookie_path: str = './quora/cookie.json',
-    ):
-        # validating the model
-        if model and model not in MODELS:
-            raise RuntimeError('Sorry, the model you provided does not exist. Please check and try again.')
-        self.model = MODELS[model]
-        self.cookie_path = cookie_path
-        self.cookie = self.__load_cookie(driver, download_driver, driver_path=driver_path)
-        self.client = PoeClient(self.cookie)
-
-    def __load_cookie(self, driver: str, download_driver: bool, driver_path: Optional[str] = None) -> str:
-        if (cookie_file := Path(self.cookie_path)).exists():
-            with cookie_file.open() as fp:
-                cookie = json.load(fp)
-                if datetime.fromtimestamp(cookie['expiry']) < datetime.now():
-                    cookie = self.__register_and_get_cookie(driver, driver_path=driver_path)
-                else:
-                    print('Loading the cookie from file')
-        else:
-            cookie = self.__register_and_get_cookie(driver, driver_path=driver_path)
-
-        return unquote(cookie['value'])
-
-    def __register_and_get_cookie(self, driver: str, driver_path: Optional[str] = None) -> dict:
-        mail_client = Emailnator()
-        mail_address = mail_client.get_mail()
-
-        driver = self.__resolve_driver(driver, driver_path=driver_path)
-        driver.get("https://www.poe.com")
-
-        # clicking use email button
-        driver.find_element(By.XPATH, '//button[contains(text(), "Use email")]').click()
-
-        email = WebDriverWait(driver, 30).until(EC.presence_of_element_located((By.XPATH, '//input[@type="email"]')))
-        email.send_keys(mail_address)
-        driver.find_element(By.XPATH, '//button[text()="Go"]').click()
-
-        code = findall(r';">(\d{6,7})</div>', mail_client.get_message())[0]
-        print(code)
-
-        verification_code = WebDriverWait(driver, 30).until(
-            EC.presence_of_element_located((By.XPATH, '//input[@placeholder="Code"]'))
-        )
-        verification_code.send_keys(code)
-        verify_button = EC.presence_of_element_located((By.XPATH, '//button[text()="Verify"]'))
-        login_button = EC.presence_of_element_located((By.XPATH, '//button[text()="Log In"]'))
-
-        WebDriverWait(driver, 30).until(EC.any_of(verify_button, login_button)).click()
-
-        cookie = driver.get_cookie('p-b')
-
-        with open(self.cookie_path, 'w') as fw:
-            json.dump(cookie, fw)
-
-        driver.close()
-        return cookie
-
-    @classmethod
-    def __resolve_driver(cls, driver: str, driver_path: Optional[str] = None) -> Union[Firefox, Chrome]:
-        options = FirefoxOptions() if driver == 'firefox' else ChromeOptions()
-        options.add_argument('-headless')
-
-        if driver_path:
-            options.binary_location = driver_path
-        try:
-            return Firefox(options=options) if driver == 'firefox' else Chrome(options=options)
-        except Exception:
-            raise Exception(SELENIUM_WEB_DRIVER_ERROR_MSG)
-
-    def chat(self, message: str, model: Optional[str] = None) -> str:
-        if model and model not in MODELS:
-            raise RuntimeError('Sorry, the model you provided does not exist. Please check and try again.')
-        model = MODELS[model] if model else self.model
-        response = None
-        for chunk in self.client.send_message(model, message):
-            response = chunk['text']
-        return response
-
-    def create_bot(
-            self,
-            name: str,
-            /,
-            prompt: str = '',
-            base_model: str = 'ChatGPT',
-            description: str = '',
-    ) -> None:
-        if base_model not in MODELS:
-            raise RuntimeError('Sorry, the base_model you provided does not exist. Please check and try again.')
-
-        response = self.client.create_bot(
-            handle=name,
-            prompt=prompt,
-            base_model=MODELS[base_model],
-            description=description,
-        )
-        print(f'Successfully created bot with name: {response["bot"]["displayName"]}')
-
-    def list_bots(self) -> list:
-        return list(self.client.bot_names.values())
+import json
+from datetime import datetime
+from hashlib import md5
+from json import dumps
+from pathlib import Path
+from random import choice, choices, randint
+from re import search, findall
+from string import ascii_letters, digits
+from typing import Optional, Union, List, Any, Generator
+from urllib.parse import unquote
+
+import selenium.webdriver.support.expected_conditions as EC
+from fake_useragent import UserAgent
+from pydantic import BaseModel
+from pypasser import reCaptchaV3
+from requests import Session
+from selenium.webdriver import Firefox, Chrome, FirefoxOptions, ChromeOptions
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support.wait import WebDriverWait
+from tls_client import Session as TLS
+
+from .api import Client as PoeClient
+from .mail import Emailnator
+
+SELENIUM_WEB_DRIVER_ERROR_MSG = b'''The error message you are receiving is due to the `geckodriver` executable not 
+being found in your system\'s PATH. To resolve this issue, you need to download the geckodriver and add its location 
+to your system\'s PATH.\n\nHere are the steps to resolve the issue:\n\n1. Download the geckodriver for your platform 
+(Windows, macOS, or Linux) from the following link: https://github.com/mozilla/geckodriver/releases\n\n2. Extract the 
+downloaded archive and locate the geckodriver executable.\n\n3. Add the geckodriver executable to your system\'s 
+PATH.\n\nFor macOS and Linux:\n\n- Open a terminal window.\n- Move the geckodriver executable to a directory that is 
+already in your PATH, or create a new directory and add it to your PATH:\n\n```bash\n# Example: Move geckodriver to 
+/usr/local/bin\nmv /path/to/your/geckodriver /usr/local/bin\n```\n\n- If you created a new directory, add it to your 
+PATH:\n\n```bash\n# Example: Add a new directory to PATH\nexport PATH=$PATH:/path/to/your/directory\n```\n\nFor 
+Windows:\n\n- Right-click on "My Computer" or "This PC" and select "Properties".\n- Click on "Advanced system 
+settings".\n- Click on the "Environment Variables" button.\n- In the "System variables" section, find the "Path" 
+variable, select it, and click "Edit".\n- Click "New" and add the path to the directory containing the geckodriver 
+executable.\n\nAfter adding the geckodriver to your PATH, restart your terminal or command prompt and try running 
+your script again. The error should be resolved.'''
+
+# from twocaptcha import TwoCaptcha
+# solver = TwoCaptcha('72747bf24a9d89b4dcc1b24875efd358')
+
+MODELS = {
+    'Sage': 'capybara',
+    'GPT-4': 'beaver',
+    'Claude+': 'a2_2',
+    'Claude-instant': 'a2',
+    'ChatGPT': 'chinchilla',
+    'Dragonfly': 'nutria',
+    'NeevaAI': 'hutia',
+}
+
+
+def extract_formkey(html):
+    script_regex = r'<script>if\(.+\)throw new Error;(.+)</script>'
+    script_text = search(script_regex, html).group(1)
+    key_regex = r'var .="([0-9a-f]+)",'
+    key_text = search(key_regex, script_text).group(1)
+    cipher_regex = r'.\[(\d+)\]=.\[(\d+)\]'
+    cipher_pairs = findall(cipher_regex, script_text)
+
+    formkey_list = [''] * len(cipher_pairs)
+    for pair in cipher_pairs:
+        formkey_index, key_index = map(int, pair)
+        formkey_list[formkey_index] = key_text[key_index]
+    formkey = ''.join(formkey_list)
+
+    return formkey
+
+
+class Choice(BaseModel):
+    text: str
+    index: int
+    logprobs: Any
+    finish_reason: str
+
+
+class Usage(BaseModel):
+    prompt_tokens: int
+    completion_tokens: int
+    total_tokens: int
+
+
+class PoeResponse(BaseModel):
+    id: int
+    object: str
+    created: int
+    model: str
+    choices: List[Choice]
+    usage: Usage
+    text: str
+
+
+class ModelResponse:
+    def __init__(self, json_response: dict) -> None:
+        self.id = json_response['data']['poeBotCreate']['bot']['id']
+        self.name = json_response['data']['poeBotCreate']['bot']['displayName']
+        self.limit = json_response['data']['poeBotCreate']['bot']['messageLimit']['dailyLimit']
+        self.deleted = json_response['data']['poeBotCreate']['bot']['deletionState']
+
+
+class Model:
+    @staticmethod
+    def create(
+        token: str,
+        model: str = 'gpt-3.5-turbo',  # claude-instant
+        system_prompt: str = 'You are ChatGPT a large language model developed by Openai. Answer as consisely as possible',
+        description: str = 'gpt-3.5 language model from openai, skidded by poe.com',
+        handle: str = None,
+    ) -> ModelResponse:
+        if not handle:
+            handle = f'gptx{randint(1111111, 9999999)}'
+
+        client = Session()
+        client.cookies['p-b'] = token
+
+        formkey = extract_formkey(client.get('https://poe.com').text)
+        settings = client.get('https://poe.com/api/settings').json()
+
+        client.headers = {
+            'host': 'poe.com',
+            'origin': 'https://poe.com',
+            'referer': 'https://poe.com/',
+            'poe-formkey': formkey,
+            'poe-tchannel': settings['tchannelData']['channel'],
+            'user-agent': UserAgent().random,
+            'connection': 'keep-alive',
+            'sec-ch-ua': '"Chromium";v="112", "Google Chrome";v="112", "Not:A-Brand";v="99"',
+            'sec-ch-ua-mobile': '?0',
+            'sec-ch-ua-platform': '"macOS"',
+            'content-type': 'application/json',
+            'sec-fetch-site': 'same-origin',
+            'sec-fetch-mode': 'cors',
+            'sec-fetch-dest': 'empty',
+            'accept': '*/*',
+            'accept-encoding': 'gzip, deflate, br',
+            'accept-language': 'en-GB,en-US;q=0.9,en;q=0.8',
+        }
+
+        payload = dumps(
+            separators=(',', ':'),
+            obj={
+                'queryName': 'CreateBotMain_poeBotCreate_Mutation',
+                'variables': {
+                    'model': MODELS[model],
+                    'handle': handle,
+                    'prompt': system_prompt,
+                    'isPromptPublic': True,
+                    'introduction': '',
+                    'description': description,
+                    'profilePictureUrl': 'https://qph.fs.quoracdn.net/main-qimg-24e0b480dcd946e1cc6728802c5128b6',
+                    'apiUrl': None,
+                    'apiKey': ''.join(choices(ascii_letters + digits, k=32)),
+                    'isApiBot': False,
+                    'hasLinkification': False,
+                    'hasMarkdownRendering': False,
+                    'hasSuggestedReplies': False,
+                    'isPrivateBot': False,
+                },
+                'query': 'mutation CreateBotMain_poeBotCreate_Mutation(\n  $model: String!\n  $handle: String!\n  $prompt: String!\n  $isPromptPublic: Boolean!\n  $introduction: String!\n  $description: String!\n  $profilePictureUrl: String\n  $apiUrl: String\n  $apiKey: String\n  $isApiBot: Boolean\n  $hasLinkification: Boolean\n  $hasMarkdownRendering: Boolean\n  $hasSuggestedReplies: Boolean\n  $isPrivateBot: Boolean\n) {\n  poeBotCreate(model: $model, handle: $handle, promptPlaintext: $prompt, isPromptPublic: $isPromptPublic, introduction: $introduction, description: $description, profilePicture: $profilePictureUrl, apiUrl: $apiUrl, apiKey: $apiKey, isApiBot: $isApiBot, hasLinkification: $hasLinkification, hasMarkdownRendering: $hasMarkdownRendering, hasSuggestedReplies: $hasSuggestedReplies, isPrivateBot: $isPrivateBot) {\n    status\n    bot {\n      id\n      ...BotHeader_bot\n    }\n  }\n}\n\nfragment BotHeader_bot on Bot {\n  displayName\n  messageLimit {\n    dailyLimit\n  }\n  ...BotImage_bot\n  ...BotLink_bot\n  ...IdAnnotation_node\n  ...botHelpers_useViewerCanAccessPrivateBot\n  ...botHelpers_useDeletion_bot\n}\n\nfragment BotImage_bot on Bot {\n  displayName\n  ...botHelpers_useDeletion_bot\n  ...BotImage_useProfileImage_bot\n}\n\nfragment BotImage_useProfileImage_bot on Bot {\n  image {\n    __typename\n    ... on LocalBotImage {\n      localName\n    }\n    ... on UrlBotImage {\n      url\n    }\n  }\n  ...botHelpers_useDeletion_bot\n}\n\nfragment BotLink_bot on Bot {\n  displayName\n}\n\nfragment IdAnnotation_node on Node {\n  __isNode: __typename\n  id\n}\n\nfragment botHelpers_useDeletion_bot on Bot {\n  deletionState\n}\n\nfragment botHelpers_useViewerCanAccessPrivateBot on Bot {\n  isPrivateBot\n  viewerIsCreator\n}\n',
+            },
+        )
+
+        base_string = payload + client.headers['poe-formkey'] + 'WpuLMiXEKKE98j56k'
+        client.headers['poe-tag-id'] = md5(base_string.encode()).hexdigest()
+
+        response = client.post('https://poe.com/api/gql_POST', data=payload)
+
+        if 'success' not in response.text:
+            raise Exception(
+                '''
+                Bot creation Failed
+                !! Important !!
+                Bot creation was not enabled on this account
+                please use: quora.Account.create with enable_bot_creation set to True
+            '''
+            )
+
+        return ModelResponse(response.json())
+
+
+class Account:
+    @staticmethod
+    def create(
+        proxy: Optional[str] = None,
+        logging: bool = False,
+        enable_bot_creation: bool = False,
+    ):
+        client = TLS(client_identifier='chrome110')
+        client.proxies = {'http': f'http://{proxy}', 'https': f'http://{proxy}'} if proxy else {}
+
+        mail_client = Emailnator()
+        mail_address = mail_client.get_mail()
+
+        if logging:
+            print('email', mail_address)
+
+        client.headers = {
+            'authority': 'poe.com',
+            'accept': '*/*',
+            'accept-language': 'en,fr-FR;q=0.9,fr;q=0.8,es-ES;q=0.7,es;q=0.6,en-US;q=0.5,am;q=0.4,de;q=0.3',
+            'content-type': 'application/json',
+            'origin': 'https://poe.com',
+            'poe-tag-id': 'null',
+            'referer': 'https://poe.com/login',
+            'sec-ch-ua': '"Chromium";v="112", "Google Chrome";v="112", "Not:A-Brand";v="99"',
+            'sec-ch-ua-mobile': '?0',
+            'sec-ch-ua-platform': '"macOS"',
+            'sec-fetch-dest': 'empty',
+            'sec-fetch-mode': 'cors',
+            'sec-fetch-site': 'same-origin',
+            'user-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
+            'poe-formkey': extract_formkey(client.get('https://poe.com/login').text),
+            'poe-tchannel': client.get('https://poe.com/api/settings').json()['tchannelData']['channel'],
+        }
+
+        token = reCaptchaV3(
+            'https://www.recaptcha.net/recaptcha/enterprise/anchor?ar=1&k=6LflhEElAAAAAI_ewVwRWI9hsyV4mbZnYAslSvlG&co=aHR0cHM6Ly9wb2UuY29tOjQ0Mw..&hl=en&v=4PnKmGB9wRHh1i04o7YUICeI&size=invisible&cb=bi6ivxoskyal'
+        )
+        # token = solver.recaptcha(sitekey='6LflhEElAAAAAI_ewVwRWI9hsyV4mbZnYAslSvlG',
+        #     url        = 'https://poe.com/login?redirect_url=%2F',
+        #     version    = 'v3',
+        #     enterprise = 1,
+        #     invisible  = 1,
+        #     action     = 'login',)['code']
+
+        payload = dumps(
+            separators=(',', ':'),
+            obj={
+                'queryName': 'MainSignupLoginSection_sendVerificationCodeMutation_Mutation',
+                'variables': {
+                    'emailAddress': mail_address,
+                    'phoneNumber': None,
+                    'recaptchaToken': token,
+                },
+                'query': 'mutation MainSignupLoginSection_sendVerificationCodeMutation_Mutation(\n  $emailAddress: String\n  $phoneNumber: String\n  $recaptchaToken: String\n) {\n  sendVerificationCode(verificationReason: login, emailAddress: $emailAddress, phoneNumber: $phoneNumber, recaptchaToken: $recaptchaToken) {\n    status\n    errorMessage\n  }\n}\n',
+            },
+        )
+
+        base_string = payload + client.headers['poe-formkey'] + 'WpuLMiXEKKE98j56k'
+        client.headers['poe-tag-id'] = md5(base_string.encode()).hexdigest()
+
+        print(dumps(client.headers, indent=4))
+
+        response = client.post('https://poe.com/api/gql_POST', data=payload)
+
+        if 'automated_request_detected' in response.text:
+            print('please try using a proxy / wait for fix')
+
+        if 'Bad Request' in response.text:
+            if logging:
+                print('bad request, retrying...', response.json())
+            quit()
+
+        if logging:
+            print('send_code', response.json())
+
+        mail_content = mail_client.get_message()
+        mail_token = findall(r';">(\d{6,7})</div>', mail_content)[0]
+
+        if logging:
+            print('code', mail_token)
+
+        payload = dumps(
+            separators=(',', ':'),
+            obj={
+                'queryName': 'SignupOrLoginWithCodeSection_signupWithVerificationCodeMutation_Mutation',
+                'variables': {
+                    'verificationCode': str(mail_token),
+                    'emailAddress': mail_address,
+                    'phoneNumber': None,
+                },
+                'query': 'mutation SignupOrLoginWithCodeSection_signupWithVerificationCodeMutation_Mutation(\n  $verificationCode: String!\n  $emailAddress: String\n  $phoneNumber: String\n) {\n  signupWithVerificationCode(verificationCode: $verificationCode, emailAddress: $emailAddress, phoneNumber: $phoneNumber) {\n    status\n    errorMessage\n  }\n}\n',
+            },
+        )
+
+        base_string = payload + client.headers['poe-formkey'] + 'WpuLMiXEKKE98j56k'
+        client.headers['poe-tag-id'] = md5(base_string.encode()).hexdigest()
+
+        response = client.post('https://poe.com/api/gql_POST', data=payload)
+        if logging:
+            print('verify_code', response.json())
+
+    def get(self):
+        cookies = open(Path(__file__).resolve().parent / 'cookies.txt', 'r').read().splitlines()
+        return choice(cookies)
+
+
+class StreamingCompletion:
+    @staticmethod
+    def create(
+        model: str = 'gpt-4',
+        custom_model: bool = None,
+        prompt: str = 'hello world',
+        token: str = '',
+        proxy: Optional[str] = None
+    ) -> Generator[PoeResponse, None, None]:
+        _model = MODELS[model] if not custom_model else custom_model
+
+        proxies = { 'http': 'http://' + proxy, 'https': 'http://' + proxy } if proxy else False
+        client = PoeClient(token)
+        client.proxy = proxies
+
+        for chunk in client.send_message(_model, prompt):
+            yield PoeResponse(
+                **{
+                    'id': chunk['messageId'],
+                    'object': 'text_completion',
+                    'created': chunk['creationTime'],
+                    'model': _model,
+                    'text': chunk['text_new'],
+                    'choices': [
+                        {
+                            'text': chunk['text_new'],
+                            'index': 0,
+                            'logprobs': None,
+                            'finish_reason': 'stop',
+                        }
+                    ],
+                    'usage': {
+                        'prompt_tokens': len(prompt),
+                        'completion_tokens': len(chunk['text_new']),
+                        'total_tokens': len(prompt) + len(chunk['text_new']),
+                    },
+                }
+            )
+
+
+class Completion:
+    @staticmethod
+    def create(
+        model: str = 'gpt-4',
+        custom_model: str = None,
+        prompt: str = 'hello world',
+        token: str = '',
+        proxy: Optional[str] = None
+    ) -> PoeResponse:
+        _model = MODELS[model] if not custom_model else custom_model
+
+        proxies = {'http': 'http://' + proxy, 'https': 'http://' + proxy} if proxy else False
+        client = PoeClient(token)
+        client.proxy = proxies
+
+        chunk = None
+        for response in client.send_message(_model, prompt):
+            chunk = response
+
+        return PoeResponse(
+            **{
+                'id': chunk['messageId'],
+                'object': 'text_completion',
+                'created': chunk['creationTime'],
+                'model': _model,
+                'text': chunk['text'],
+                'choices': [
+                    {
+                        'text': chunk['text'],
+                        'index': 0,
+                        'logprobs': None,
+                        'finish_reason': 'stop',
+                    }
+                ],
+                'usage': {
+                    'prompt_tokens': len(prompt),
+                    'completion_tokens': len(chunk['text']),
+                    'total_tokens': len(prompt) + len(chunk['text']),
+                },
+            }
+        )
+
+
+class Poe:
+    def __init__(
+        self,
+        model: str = 'ChatGPT',
+        driver: str = 'firefox',
+        download_driver: bool = False,
+        driver_path: Optional[str] = None,
+        cookie_path: str = './quora/cookie.json',
+    ):
+        # validating the model
+        if model and model not in MODELS:
+            raise RuntimeError('Sorry, the model you provided does not exist. Please check and try again.')
+        self.model = MODELS[model]
+        self.cookie_path = cookie_path
+        self.cookie = self.__load_cookie(driver, driver_path=driver_path)
+        self.client = PoeClient(self.cookie)
+
+    def __load_cookie(self, driver: str, driver_path: Optional[str] = None) -> str:
+        if (cookie_file := Path(self.cookie_path)).exists():
+            with cookie_file.open() as fp:
+                cookie = json.load(fp)
+                if datetime.fromtimestamp(cookie['expiry']) < datetime.now():
+                    cookie = self.__register_and_get_cookie(driver, driver_path=driver_path)
+                else:
+                    print('Loading the cookie from file')
+        else:
+            cookie = self.__register_and_get_cookie(driver, driver_path=driver_path)
+
+        return unquote(cookie['value'])
+
+    def __register_and_get_cookie(self, driver: str, driver_path: Optional[str] = None) -> dict:
+        mail_client = Emailnator()
+        mail_address = mail_client.get_mail()
+
+        driver = self.__resolve_driver(driver, driver_path=driver_path)
+        driver.get("https://www.poe.com")
+
+        # clicking use email button
+        driver.find_element(By.XPATH, '//button[contains(text(), "Use email")]').click()
+
+        email = WebDriverWait(driver, 30).until(EC.presence_of_element_located((By.XPATH, '//input[@type="email"]')))
+        email.send_keys(mail_address)
+        driver.find_element(By.XPATH, '//button[text()="Go"]').click()
+
+        code = findall(r';">(\d{6,7})</div>', mail_client.get_message())[0]
+        print(code)
+
+        verification_code = WebDriverWait(driver, 30).until(
+            EC.presence_of_element_located((By.XPATH, '//input[@placeholder="Code"]'))
+        )
+        verification_code.send_keys(code)
+        verify_button = EC.presence_of_element_located((By.XPATH, '//button[text()="Verify"]'))
+        login_button = EC.presence_of_element_located((By.XPATH, '//button[text()="Log In"]'))
+
+        WebDriverWait(driver, 30).until(EC.any_of(verify_button, login_button)).click()
+
+        cookie = driver.get_cookie('p-b')
+
+        with open(self.cookie_path, 'w') as fw:
+            json.dump(cookie, fw)
+
+        driver.close()
+        return cookie
+
+    @staticmethod
+    def __resolve_driver(driver: str, driver_path: Optional[str] = None) -> Union[Firefox, Chrome]:
+        options = FirefoxOptions() if driver == 'firefox' else ChromeOptions()
+        options.add_argument('-headless')
+
+        if driver_path:
+            options.binary_location = driver_path
+        try:
+            return Firefox(options=options) if driver == 'firefox' else Chrome(options=options)
+        except Exception:
+            raise Exception(SELENIUM_WEB_DRIVER_ERROR_MSG)
+
+    def chat(self, message: str, model: Optional[str] = None) -> str:
+        if model and model not in MODELS:
+            raise RuntimeError('Sorry, the model you provided does not exist. Please check and try again.')
+        model = MODELS[model] if model else self.model
+        response = None
+        for chunk in self.client.send_message(model, message):
+            response = chunk['text']
+        return response
+
+    def create_bot(
+        self,
+        name: str,
+        /,
+        prompt: str = '',
+        base_model: str = 'ChatGPT',
+        description: str = '',
+    ) -> None:
+        if base_model not in MODELS:
+            raise RuntimeError('Sorry, the base_model you provided does not exist. Please check and try again.')
+
+        response = self.client.create_bot(
+            handle=name,
+            prompt=prompt,
+            base_model=MODELS[base_model],
+            description=description,
+        )
+        print(f'Successfully created bot with name: {response["bot"]["displayName"]}')
+
+    def list_bots(self) -> list:
+        return list(self.client.bot_names.values())
```

### Comparing `gpt4free-0.1.2/gpt4free/quora/api.py` & `gpt4free-0.1.3/gpt4free/quora/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
                 "poe-tag-id": hashlib.md5(base_string.encode()).hexdigest(),
             }
             headers = {**self.gql_headers, **headers}
 
             r = request_with_retries(self.session.post, self.gql_url, data=payload, headers=headers)
 
             data = r.json()
-            if data["data"] == None:
+            if data["data"] is None:
                 logger.warn(f'{query_name} returned an error: {data["errors"][0]["message"]} | Retrying ({i + 1}/20)')
                 time.sleep(2)
                 continue
 
             return r.json()
 
         raise RuntimeError(f"{query_name} failed too many times.")
@@ -312,15 +312,15 @@
                 for key, value in copied_dict.items():
                     # add the message to the appropriate queue
                     if value == message["messageId"] and key in self.message_queues:
                         self.message_queues[key].put(message)
                         return
 
                     # indicate that the response id is tied to the human message id
-                    elif key != "pending" and value == None and message["state"] != "complete":
+                    elif key != "pending" and value is None and message["state"] != "complete":
                         self.active_messages[key] = message["messageId"]
                         self.message_queues[key].put(message)
                         return
 
         except Exception:
             logger.error(traceback.format_exc())
             self.disconnect_ws()
@@ -380,15 +380,15 @@
             if message["state"] == "complete":
                 if last_text and message["messageId"] == message_id:
                     break
                 else:
                     continue
 
             # update info about response
-            message["text_new"] = message["text"][len(last_text):]
+            message["text_new"] = message["text"][len(last_text) :]
             last_text = message["text"]
             message_id = message["messageId"]
 
             yield message
 
         del self.active_messages[human_message_id]
         del self.message_queues[human_message_id]
@@ -398,15 +398,15 @@
         result = self.send_query("AddMessageBreakMutation", {"chatId": self.bots[chatbot]["chatId"]})
         return result["data"]["messageBreakCreate"]["message"]
 
     def get_message_history(self, chatbot, count=25, cursor=None):
         logger.info(f"Downloading {count} messages from {chatbot}")
 
         messages = []
-        if cursor == None:
+        if cursor is None:
             chat_data = self.get_bot(self.bot_names[chatbot])
             if not chat_data["messagesConnection"]["edges"]:
                 return []
             messages = chat_data["messagesConnection"]["edges"][:count]
             cursor = chat_data["messagesConnection"]["pageInfo"]["startCursor"]
             count -= len(messages)
 
@@ -452,29 +452,29 @@
 
             if count == 0:
                 return
             last_messages = self.get_message_history(chatbot, count=50)[::-1]
         logger.info(f"No more messages left to delete.")
 
     def create_bot(
-            self,
-            handle,
-            prompt="",
-            base_model="chinchilla",
-            description="",
-            intro_message="",
-            api_key=None,
-            api_bot=False,
-            api_url=None,
-            prompt_public=True,
-            pfp_url=None,
-            linkification=False,
-            markdown_rendering=True,
-            suggested_replies=False,
-            private=False,
+        self,
+        handle,
+        prompt="",
+        base_model="chinchilla",
+        description="",
+        intro_message="",
+        api_key=None,
+        api_bot=False,
+        api_url=None,
+        prompt_public=True,
+        pfp_url=None,
+        linkification=False,
+        markdown_rendering=True,
+        suggested_replies=False,
+        private=False,
     ):
         result = self.send_query(
             "PoeBotCreateMutation",
             {
                 "model": base_model,
                 "handle": handle,
                 "prompt": prompt,
@@ -495,29 +495,29 @@
         data = result["data"]["poeBotCreate"]
         if data["status"] != "success":
             raise RuntimeError(f"Poe returned an error while trying to create a bot: {data['status']}")
         self.get_bots()
         return data
 
     def edit_bot(
-            self,
-            bot_id,
-            handle,
-            prompt="",
-            base_model="chinchilla",
-            description="",
-            intro_message="",
-            api_key=None,
-            api_url=None,
-            private=False,
-            prompt_public=True,
-            pfp_url=None,
-            linkification=False,
-            markdown_rendering=True,
-            suggested_replies=False,
+        self,
+        bot_id,
+        handle,
+        prompt="",
+        base_model="chinchilla",
+        description="",
+        intro_message="",
+        api_key=None,
+        api_url=None,
+        private=False,
+        prompt_public=True,
+        pfp_url=None,
+        linkification=False,
+        markdown_rendering=True,
+        suggested_replies=False,
     ):
         result = self.send_query(
             "PoeBotEditMutation",
             {
                 "baseBot": base_model,
                 "botId": bot_id,
                 "handle": handle,
```

### Comparing `gpt4free-0.1.2/gpt4free/quora/mail.py` & `gpt4free-0.1.3/gpt4free/quora/mail.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,17 +38,15 @@
         return self.email
 
     def get_message(self):
         print("Waiting for message...")
 
         while True:
             sleep(2)
-            mail_token = self.client.post(
-                "https://www.emailnator.com/message-list", json={"email": self.email}
-            )
+            mail_token = self.client.post("https://www.emailnator.com/message-list", json={"email": self.email})
 
             mail_token = loads(mail_token.text)["messageData"]
 
             if len(mail_token) == 2:
                 print("Message received!")
                 print(mail_token[1]["messageID"])
                 break
```

### Comparing `gpt4free-0.1.2/gpt4free/you/__init__.py` & `gpt4free-0.1.3/gpt4free/you/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,49 @@
+import json
 import re
-from json import loads
+from typing import Optional, List, Dict, Any
 from uuid import uuid4
 
 from fake_useragent import UserAgent
+from pydantic import BaseModel
 from tls_client import Session
 
 
+class PoeResponse(BaseModel):
+    text: Optional[str] = None
+    links: List[str] = []
+    extra: Dict[str, Any] = {}
+
+
 class Completion:
     @staticmethod
     def create(
-            prompt: str,
-            page: int = 1,
-            count: int = 10,
-            safe_search: str = 'Moderate',
-            on_shopping_page: bool = False,
-            mkt: str = '',
-            response_filter: str = 'WebPages,Translations,TimeZone,Computation,RelatedSearches',
-            domain: str = 'youchat',
-            query_trace_id: str = None,
-            chat: list = None,
-            include_links: bool = False,
-            detailed: bool = False,
-            debug: bool = False,
-    ) -> dict:
+        prompt: str,
+        page: int = 1,
+        count: int = 10,
+        safe_search: str = 'Moderate',
+        on_shopping_page: bool = False,
+        mkt: str = '',
+        response_filter: str = 'WebPages,Translations,TimeZone,Computation,RelatedSearches',
+        domain: str = 'youchat',
+        query_trace_id: str = None,
+        chat: list = None,
+        include_links: bool = False,
+        detailed: bool = False,
+        debug: bool = False,
+        proxy: Optional[str] = None
+    ) -> PoeResponse:
         if chat is None:
             chat = []
 
+        proxies = { 'http': 'http://' + proxy, 'https': 'http://' + proxy } if proxy else {}
+
         client = Session(client_identifier='chrome_108')
         client.headers = Completion.__get_headers()
+        client.proxies = proxies
 
         response = client.get(
             f'https://you.com/api/streamingSearch',
             params={
                 'q': prompt,
                 'page': page,
                 'count': count,
@@ -53,34 +65,36 @@
         if 'youChatToken' not in response.text:
             return Completion.__get_failure_response()
 
         you_chat_serp_results = re.search(
             r'(?<=event: youChatSerpResults\ndata:)(.*\n)*?(?=event: )', response.text
         ).group()
         third_party_search_results = re.search(
-            r'(?<=event: thirdPartySearchResults\ndata:)(.*\n)*?(?=event: )', response.text).group()
+            r'(?<=event: thirdPartySearchResults\ndata:)(.*\n)*?(?=event: )', response.text
+        ).group()
         # slots                   = findall(r"slots\ndata: (.*)\n\nevent", response.text)[0]
 
         text = ''.join(re.findall(r'{\"youChatToken\": \"(.*?)\"}', response.text))
 
         extra = {
-            'youChatSerpResults': loads(you_chat_serp_results),
+            'youChatSerpResults': json.loads(you_chat_serp_results),
             # 'slots'                   : loads(slots)
         }
 
-        return {
-            'response': text.replace('\\n', '\n').replace('\\\\', '\\').replace('\\"', '"'),
-            'links': loads(third_party_search_results)['search']['third_party_search_results']
-            if include_links
-            else None,
-            'extra': extra if detailed else None,
-        }
+        response = PoeResponse(text=text.replace('\\n', '\n').replace('\\\\', '\\').replace('\\"', '"'))
+        if include_links:
+            response.links = json.loads(third_party_search_results)['search']['third_party_search_results']
+
+        if detailed:
+            response.extra = extra
+
+        return response
 
-    @classmethod
-    def __get_headers(cls) -> dict:
+    @staticmethod
+    def __get_headers() -> dict:
         return {
             'authority': 'you.com',
             'accept': 'text/event-stream',
             'accept-language': 'en,fr-FR;q=0.9,fr;q=0.8,es-ES;q=0.7,es;q=0.6,en-US;q=0.5,am;q=0.4,de;q=0.3',
             'cache-control': 'no-cache',
             'referer': 'https://you.com/search?q=who+are+you&tbm=youchat',
             'sec-ch-ua': '"Not_A Brand";v="99", "Google Chrome";v="109", "Chromium";v="109"',
@@ -89,10 +103,10 @@
             'sec-fetch-dest': 'empty',
             'sec-fetch-mode': 'cors',
             'sec-fetch-site': 'same-origin',
             'cookie': f'safesearch_guest=Moderate; uuid_guest={str(uuid4())}',
             'user-agent': UserAgent().random,
         }
 
-    @classmethod
-    def __get_failure_response(cls) -> dict:
-        return dict(response='Unable to fetch the response, Please try again.', links=[], extra={})
+    @staticmethod
+    def __get_failure_response() -> PoeResponse:
+        return PoeResponse(text='Unable to fetch the response, Please try again.')
```

### Comparing `gpt4free-0.1.2/gpt4free.egg-info/PKG-INFO` & `gpt4free-0.1.3/gpt4free.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4free
-Version: 0.1.2
+Version: 0.1.3
 Summary: decentralising the Ai Industry, free gpt-4/3.5 scripts through several reverse engineered api's
 Home-page: https://github.com/rzashakeri/gpt4free
 Author: Reza Shakeri
 Author-email: rzashakeri@gmail.com
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/rzashakeri/gpt4free
 Project-URL: Issue tracker, https://github.com/rzashakeri/gpt4free/issues
```

### Comparing `gpt4free-0.1.2/setup.py` & `gpt4free-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     "names",
     "colorama",
     "curl_cffi",
     "streamlit==1.21.0",
     "selenium",
     "fake-useragent",
     "twocaptcha",
+    "pydantic",
+    "pymailtm"
 ]
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Reza Shakeri",
     author_email='rzashakeri@gmail.com',
@@ -54,15 +56,15 @@
         "Ai"
     ],
     name='gpt4free',
     packages=find_packages(include=['gpt4free', 'gpt4free.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/rzashakeri/gpt4free',
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
     project_urls={
         "Homepage": "https://github.com/rzashakeri/gpt4free",
         "Issue tracker": "https://github.com/rzashakeri/gpt4free/issues",
         "Release notes": "https://github.com/rzashakeri/gpt4free/releases",
         "Source": "https://github.com/rzashakeri/gpt4free",
         "Discussions": "https://github.com/rzashakeri/gpt4free/discussions",
```

