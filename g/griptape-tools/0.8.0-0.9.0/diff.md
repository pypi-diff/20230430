# Comparing `tmp/griptape_tools-0.8.0.tar.gz` & `tmp/griptape_tools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_tools-0.8.0.tar", max compression
+gzip compressed data, was "griptape_tools-0.9.0.tar", max compression
```

## Comparing `griptape_tools-0.8.0.tar` & `griptape_tools-0.9.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.8.0/LICENSE
--rw-r--r--   0        0        0     1284 2023-04-21 17:41:39.072846 griptape_tools-0.8.0/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.8.0/griptape/__init__.py
--rw-r--r--   0        0        0      352 2023-04-13 16:07:18.435628 griptape_tools-0.8.0/griptape/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.8.0/griptape/tools/aws_cli/__init__.py
--rw-r--r--   0        0        0      159 2023-04-13 16:14:30.544316 griptape_tools-0.8.0/griptape/tools/aws_cli/manifest.yml
--rw-r--r--   0        0        0       71 2023-04-23 21:38:29.292854 griptape_tools-0.8.0/griptape/tools/aws_cli/requirements.txt
--rw-r--r--   0        0        0     1467 2023-04-24 19:00:12.784453 griptape_tools-0.8.0/griptape/tools/aws_cli/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.8.0/griptape/tools/calculator/__init__.py
--rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.8.0/griptape/tools/calculator/manifest.yml
--rw-r--r--   0        0        0       14 2023-04-23 21:38:29.291686 griptape_tools-0.8.0/griptape/tools/calculator/requirements.txt
--rw-r--r--   0        0        0      676 2023-04-24 19:00:12.782272 griptape_tools-0.8.0/griptape/tools/calculator/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.8.0/griptape/tools/email_client/__init__.py
--rw-r--r--   0        0        0      153 2023-04-12 21:25:06.766972 griptape_tools-0.8.0/griptape/tools/email_client/manifest.yml
--rw-r--r--   0        0        0       14 2023-04-23 21:38:29.288512 griptape_tools-0.8.0/griptape/tools/email_client/requirements.txt
--rw-r--r--   0        0        0     5893 2023-04-24 19:00:12.786990 griptape_tools-0.8.0/griptape/tools/email_client/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.8.0/griptape/tools/sql_client/__init__.py
--rw-r--r--   0        0        0      154 2023-04-12 19:53:04.579660 griptape_tools-0.8.0/griptape/tools/sql_client/manifest.yml
--rw-r--r--   0        0        0       26 2023-04-23 21:38:29.287003 griptape_tools-0.8.0/griptape/tools/sql_client/requirements.txt
--rw-r--r--   0        0        0     1259 2023-04-24 19:00:12.780590 griptape_tools-0.8.0/griptape/tools/sql_client/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.8.0/griptape/tools/web_scraper/__init__.py
--rw-r--r--   0        0        0      195 2023-04-11 21:24:23.634297 griptape_tools-0.8.0/griptape/tools/web_scraper/manifest.yml
--rw-r--r--   0        0        0       46 2023-04-23 21:38:29.290644 griptape_tools-0.8.0/griptape/tools/web_scraper/requirements.txt
--rw-r--r--   0        0        0     4437 2023-04-24 19:00:12.789352 griptape_tools-0.8.0/griptape/tools/web_scraper/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.8.0/griptape/tools/web_search/__init__.py
--rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.8.0/griptape/tools/web_search/manifest.yml
--rw-r--r--   0        0        0       22 2023-04-23 21:38:29.289637 griptape_tools-0.8.0/griptape/tools/web_search/requirements.txt
--rw-r--r--   0        0        0     2263 2023-04-24 19:00:12.778362 griptape_tools-0.8.0/griptape/tools/web_search/tool.py
--rw-r--r--   0        0        0      541 2023-04-24 19:31:33.753195 griptape_tools-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1971 1970-01-01 00:00:00.000000 griptape_tools-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1151 2023-04-24 20:05:55.932841 griptape_tools-0.9.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.9.0/griptape/__init__.py
+-rw-r--r--   0        0        0      352 2023-04-13 16:07:18.435628 griptape_tools-0.9.0/griptape/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.9.0/griptape/tools/aws_cli/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-13 16:14:30.544316 griptape_tools-0.9.0/griptape/tools/aws_cli/manifest.yml
+-rw-r--r--   0        0        0       73 2023-04-30 21:00:51.923653 griptape_tools-0.9.0/griptape/tools/aws_cli/requirements.txt
+-rw-r--r--   0        0        0     1745 2023-04-30 21:02:58.677825 griptape_tools-0.9.0/griptape/tools/aws_cli/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.9.0/griptape/tools/calculator/__init__.py
+-rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.9.0/griptape/tools/calculator/manifest.yml
+-rw-r--r--   0        0        0       16 2023-04-30 21:00:51.922811 griptape_tools-0.9.0/griptape/tools/calculator/requirements.txt
+-rw-r--r--   0        0        0      816 2023-04-30 19:49:57.299564 griptape_tools-0.9.0/griptape/tools/calculator/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.9.0/griptape/tools/email_client/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-12 21:25:06.766972 griptape_tools-0.9.0/griptape/tools/email_client/manifest.yml
+-rw-r--r--   0        0        0       16 2023-04-30 21:00:51.918672 griptape_tools-0.9.0/griptape/tools/email_client/requirements.txt
+-rw-r--r--   0        0        0     6041 2023-04-30 19:49:57.293290 griptape_tools-0.9.0/griptape/tools/email_client/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.9.0/griptape/tools/sql_client/__init__.py
+-rw-r--r--   0        0        0      154 2023-04-12 19:53:04.579660 griptape_tools-0.9.0/griptape/tools/sql_client/manifest.yml
+-rw-r--r--   0        0        0       28 2023-04-30 21:00:51.919938 griptape_tools-0.9.0/griptape/tools/sql_client/requirements.txt
+-rw-r--r--   0        0        0     1413 2023-04-30 19:49:57.297074 griptape_tools-0.9.0/griptape/tools/sql_client/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.9.0/griptape/tools/web_scraper/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-11 21:24:23.634297 griptape_tools-0.9.0/griptape/tools/web_scraper/manifest.yml
+-rw-r--r--   0        0        0       28 2023-04-30 21:00:51.920950 griptape_tools-0.9.0/griptape/tools/web_scraper/requirements.txt
+-rw-r--r--   0        0        0     2890 2023-04-30 19:49:57.304804 griptape_tools-0.9.0/griptape/tools/web_scraper/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.9.0/griptape/tools/web_search/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.9.0/griptape/tools/web_search/manifest.yml
+-rw-r--r--   0        0        0       24 2023-04-30 21:00:51.921786 griptape_tools-0.9.0/griptape/tools/web_search/requirements.txt
+-rw-r--r--   0        0        0     2323 2023-04-30 19:49:57.307290 griptape_tools-0.9.0/griptape/tools/web_search/tool.py
+-rw-r--r--   0        0        0      520 2023-04-30 21:07:32.928296 griptape_tools-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 griptape_tools-0.9.0/PKG-INFO
```

### Comparing `griptape_tools-0.8.0/LICENSE` & `griptape_tools-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.8.0/README.md` & `griptape_tools-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # griptape-tools
 
-[![Tests](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml/badge.svg)](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/griptape-tools.svg)](https://pypi.python.org/pypi/griptape-tools)
-[![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io/en/latest/griptape_tools/)
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/gitbucket/gitbucket/blob/master/LICENSE)
+[![Tests](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml/badge.svg)](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml)
+[![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io/en/latest/griptape-tools/)
 [![Griptape Discord](https://dcbadge.vercel.app/api/server/gnWRz88eym?compact=true&style=flat)](https://discord.gg/gnWRz88eym)
 
 This repo is a collection of official Griptape tools for the [Griptape Framework](https://github.com/griptape-ai/griptape). You can run Griptape tools in [griptape-flow](https://github.com/griptape-ai/griptape-flow), [LangChain](https://github.com/hwchase17/langchain), or as [ChatGPT Plugins](https://openai.com/blog/chatgpt-plugins).
 
 ## Documentation
 
 Please refer to [Griptape Docs](https://griptape.readthedocs.io) for:
```

### Comparing `griptape_tools-0.8.0/griptape/tools/calculator/tool.py` & `griptape_tools-0.9.0/griptape/tools/calculator/tool.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from griptape.core import BaseTool, action
+from griptape.artifacts import BaseArtifact, TextArtifact, ErrorArtifact
+from griptape.core import BaseTool
+from griptape.core.decorators import activity
 import griptape.utils as utils
 from schema import Schema
 
 
 class Calculator(BaseTool):
-    @action(config={
+    @activity(config={
         "name": "calculate",
         "description": "Can be used for making simple calculations in Python",
         "schema": Schema(
             str,
             description="Arithmetic expression parsable in pure Python. Single line only. Don't use any "
                         "imports or external libraries"
         )
     })
-    def calculate(self, value: bytes) -> str:
+    def calculate(self, value: str) -> BaseArtifact:
         try:
-            return utils.PythonRunner().run(value.decode())
+            return TextArtifact(utils.PythonRunner().run(value))
         except Exception as e:
-            return f"error calculating: {e}"
+            return ErrorArtifact(f"error calculating: {e}")
```

### Comparing `griptape_tools-0.8.0/griptape/tools/email_client/tool.py` & `griptape_tools-0.9.0/griptape/tools/email_client/tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-import ast
+import imaplib
 import logging
 import smtplib
-import imaplib
 from email.mime.text import MIMEText
 from typing import Optional
+import schema
 from attr import define, field
-from griptape.core import BaseTool, action
+from griptape.artifacts import BaseArtifact, TextArtifact, ErrorArtifact
+from griptape.core import BaseTool
+from griptape.core.decorators import activity
 from schema import Schema, Literal
 
 
 @define
 class EmailClient(BaseTool):
     # if you set imap|smtp creds explicitly these fields will be overridden
     username: Optional[str] = field(default=None, kw_only=True, metadata={"env": "EMAIL_USERNAME"})
@@ -28,15 +30,15 @@
     # if you set imap user/password fields they will override
     imap_user: Optional[str] = field(default=None, kw_only=True, metadata={"env": "IMAP_USER"})
     imap_password: Optional[str] = field(default=None, kw_only=True, metadata={"env": "IMAP_PASSWORD"})
 
     # be careful of allowing too many records to be returned as it could impact token usage
     email_max_retrieve_count: int = field(default=10, kw_only=True, metadata={"env": "EMAIL_MAX_RETRIEVE_COUNT"})
 
-    @action(config={
+    @activity(config={
         "name": "retrieve",
         "description": "Can be used to retrieve emails",
         "schema": Schema({
             Literal(
                 "label",
                 description="Label to retrieve emails from such as 'INBOX' or 'SENT'"
             ): str,
@@ -44,63 +46,62 @@
                 "key",
                 description="Key for filtering such as 'FROM' or 'SUBJECT'"
             ): str,
             Literal(
                 "search_criteria",
                 description="Search criteria to filter emails"
             ): str,
-            Literal(
-                "retrieve_count",
-                description="Optional param to override the default max retrieve count"
+            schema.Optional(
+                Literal(
+                    "retrieve_count",
+                    description="Optional param to override the default max retrieve count"
+                )
             ): int
         })
     })
-
-    def retrieve(self, value: bytes) -> list[str]:
-        params = ast.literal_eval(value.decode())
-
+    def retrieve(self, value: dict) -> BaseArtifact:
         imap_url = self.env_value("IMAP_URL")
 
         # email username can be overridden by setting the imap user explicitly
         imap_user = self.env_value("IMAP_USER")
         if imap_user is None:
             imap_user = self.env_value("EMAIL_USERNAME")
 
         # email password can be overridden by setting the imap password explicitly
         imap_password = self.env_value("IMAP_PASSWORD")
         if imap_password is None:
             imap_password = self.env_value("EMAIL_PASSWORD")
 
         max_retrieve_count = self.env_value("EMAIL_MAX_RETRIEVE_COUNT")
 
-        label = params["label"]
-        key = params["key"]
-        retrieve_count = int(params["retrieve_count"]) if "retrieve_count" in params else max_retrieve_count
-        search_criteria = params["search_criteria"]
+        label = value["label"]
+        key = value["key"]
+        retrieve_count = int(value["retrieve_count"]) if "retrieve_count" in value else max_retrieve_count
+        search_criteria = value["search_criteria"]
 
         try:
             con = imaplib.IMAP4_SSL(imap_url)
             con.login(imap_user, imap_password)
             con.select(label)
 
-            result, data = con.search(None, key, search_criteria)
+            result, data = con.search(None, key, f'"{search_criteria}"')
             retrieve_list = data[0].split()
             messages = []
             for num in retrieve_list[0:min(int(max_retrieve_count), int(retrieve_count))]:
-                typ, data = con.fetch(num, '(RFC822)')
+                typ, data = con.fetch(num, "(RFC822)")
                 messages.append(data)
             con.close()
 
-            return messages
+            return TextArtifact(str(messages))
         except Exception as e:
             logging.error(e)
-            return "error retrieving email {e}"
 
+            return ErrorArtifact(f"error retrieving email {e}")
 
-    @action(config={
+    @activity(config={
         "name": "send",
         "description": "Can be used to send emails",
         "schema": Schema({
             Literal(
                 "to",
                 description="Recipient's email address"
             ): str,
@@ -110,51 +111,50 @@
             ): str,
             Literal(
                 "body",
                 description="Email body"
             ): str
         })
     })
-    def send(self, value: bytes) -> str:
+    def send(self, value: dict) -> BaseArtifact:
         server: Optional[smtplib.SMTP] = None
-        params = ast.literal_eval(value.decode())
 
         # email username can be overridden by setting the smtp user explicitly
         smtp_user = self.env_value("SMTP_USER")
         if smtp_user is None:
             smtp_user = self.env_value("EMAIL_USERNAME")
 
         # email password can be overridden by setting the smtp password explicitly
         smtp_password = self.env_value("SMTP_PASSWORD")
         if smtp_password is None:
             smtp_password = self.env_value("EMAIL_PASSWORD")
 
         smtp_host = self.env_value("SMTP_HOST")
         smtp_port = int(self.env_value("SMTP_PORT"))
 
-        to_email = params["to"]
-        subject = params["subject"]
-        msg = MIMEText(params["body"])
+        to_email = value["to"]
+        subject = value["subject"]
+        msg = MIMEText(value["body"])
 
         try:
             if self.env_value("SMTP_USE_SSL"):
                 server = smtplib.SMTP_SSL(smtp_host, smtp_port)
             else:
                 server = smtplib.SMTP(smtp_host, smtp_port)
 
             msg["Subject"] = subject
             msg["From"] = smtp_user
             msg["To"] = to_email
 
             server.login(smtp_user, smtp_password)
             server.sendmail(smtp_user, [to_email], msg.as_string())
 
-            return "email was successfully sent"
+            return TextArtifact("email was successfully sent")
         except Exception as e:
             logging.error(e)
 
-            return f"error sending email: {e}"
+            return ErrorArtifact(f"error sending email: {e}")
         finally:
             try:
                 server.quit()
             except:
                 pass
```

### Comparing `griptape_tools-0.8.0/griptape/tools/sql_client/tool.py` & `griptape_tools-0.9.0/griptape/tools/sql_client/tool.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 from typing import Optional
 from attr import define, field
-from griptape.core import BaseTool, action
+from griptape.artifacts import BaseArtifact, TextArtifact, ErrorArtifact
+from griptape.core import BaseTool
+from griptape.core.decorators import activity
 from schema import Schema
 
 
 @define
 class SqlClient(BaseTool):
     engine_url: Optional[str] = field(default=None, kw_only=True, metadata={"env": "ENGINE_URL"})
     engine_name: str = field(kw_only=True)
 
     @property
     def schema_template_args(self) -> dict:
         return {
             "engine": self.engine_name
         }
 
-    @action(config={
+    @activity(config={
         "name": "query",
         "description": "Can be used to execute SQL queries in {{ engine }}",
         "schema": Schema(
             str,
             description="SQL query to execute. For example, SELECT, CREATE, INSERT, DROP, DELETE, etc."
         )
     })
-    def query(self, value: bytes) -> str:
+    def query(self, value: str) -> BaseArtifact:
         from sqlalchemy import create_engine, text
 
         engine = create_engine(self.env_value("ENGINE_URL"))
 
         try:
             with engine.connect() as con:
-                results = con.execute(text(value.decode()))
+                results = con.execute(text(value))
 
                 if results.returns_rows:
-                    return str([row for row in results]).strip('[]')
+                    return TextArtifact(str([row for row in results]).strip('[]'))
                 else:
-                    return "query successfully executed"
+                    return TextArtifact("query successfully executed")
 
         except Exception as e:
-            return f"error executing SQL: {e}"
+            return ErrorArtifact(f"error executing SQL: {e}")
```

### Comparing `griptape_tools-0.8.0/griptape/tools/web_search/tool.py` & `griptape_tools-0.9.0/griptape/tools/web_search/tool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 from typing import Optional
 from attr import define, field
+from griptape.artifacts import BaseArtifact, TextArtifact, ErrorArtifact
 from schema import Schema
-from griptape.core import BaseTool, action
+from griptape.core import BaseTool
+from griptape.core.decorators import activity
 
 
 @define
 class WebSearch(BaseTool):
     results_count: int = field(default=5, kw_only=True, metadata={"env": "SEARCH_RESULTS_COUNT"})
     google_api_lang: str = field(default="lang_en", kw_only=True, metadata={"env": "GOOGLE_API_LANG"})
     google_api_key: Optional[str] = field(default=None, kw_only=True, metadata={"env": "GOOGLE_API_KEY"})
     google_api_search_id: Optional[str] = field(default=None, kw_only=True, metadata={"env": "GOOGLE_API_SEARCH_ID"})
     google_api_country: str = field(default="us", kw_only=True, metadata={"env": "GOOGLE_API_COUNTRY"})
 
-    @action(config={
+    @activity(config={
         "name": "search",
         "description": "Can be used for searching the web",
         "schema": Schema(
             str,
             description="Search engine request that returns a list of pages with titles, descriptions, and URLs"
         )
     })
-    def search(self, value: bytes) -> dict:
+    def search(self, value: str) -> BaseArtifact:
         try:
-            return {
-                "results": self._search_google(value.decode())
-            }
+            return TextArtifact(str(self._search_google(value)))
         except Exception as e:
-            return {
-                "error": f"error searching Google: {e}"
-            }
+            return ErrorArtifact(f"error searching Google: {e}")
 
     def _search_google(self, query: str) -> list[dict]:
         import requests
 
         url = f"https://www.googleapis.com/customsearch/v1?" \
               f"key={self.env_value('GOOGLE_API_KEY')}&" \
               f"cx={self.env_value('GOOGLE_API_SEARCH_ID')}&" \
```

### Comparing `griptape_tools-0.8.0/pyproject.toml` & `griptape_tools-0.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "griptape-tools"
-version = "0.8.0"
+version = "0.9.0"
 description = "Tools for the griptape-core package."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-tools"
 
 packages = [
     {include = "griptape"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-griptape = ">=0.6"
-llama_index = ">= 0.5"
+griptape = ">=0.7.1"
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-mock = "*"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `griptape_tools-0.8.0/PKG-INFO` & `griptape_tools-0.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: griptape-tools
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tools for the griptape-core package.
 Home-page: https://github.com/griptape-ai/griptape-tools
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: griptape (>=0.6)
-Requires-Dist: llama_index (>=0.5)
+Requires-Dist: griptape (>=0.7.1)
 Project-URL: Repository, https://github.com/griptape-ai/griptape-tools
 Description-Content-Type: text/markdown
 
 # griptape-tools
 
-[![Tests](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml/badge.svg)](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/griptape-tools.svg)](https://pypi.python.org/pypi/griptape-tools)
-[![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io/en/latest/griptape_tools/)
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/gitbucket/gitbucket/blob/master/LICENSE)
+[![Tests](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml/badge.svg)](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml)
+[![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io/en/latest/griptape-tools/)
 [![Griptape Discord](https://dcbadge.vercel.app/api/server/gnWRz88eym?compact=true&style=flat)](https://discord.gg/gnWRz88eym)
 
 This repo is a collection of official Griptape tools for the [Griptape Framework](https://github.com/griptape-ai/griptape). You can run Griptape tools in [griptape-flow](https://github.com/griptape-ai/griptape-flow), [LangChain](https://github.com/hwchase17/langchain), or as [ChatGPT Plugins](https://openai.com/blog/chatgpt-plugins).
 
 ## Documentation
 
 Please refer to [Griptape Docs](https://griptape.readthedocs.io) for:
```

