# Comparing `tmp/aiogram-ext-0.5.0.tar.gz` & `tmp/aiogram-ext-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-ext-0.5.0.tar", last modified: Sun Apr 30 16:06:26 2023, max compression
+gzip compressed data, was "aiogram-ext-0.5.1.tar", last modified: Sun Apr 30 16:19:09 2023, max compression
```

## Comparing `aiogram-ext-0.5.0.tar` & `aiogram-ext-0.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1705 2023-04-30 08:48:21.984741 aiogram-ext-0.5.0/botty/__init__.py
--rw-r--r--   0        0        0      794 2023-04-28 06:49:53.068602 aiogram-ext-0.5.0/botty/bot.py
--rw-r--r--   0        0        0     1752 2023-04-30 07:58:02.593722 aiogram-ext-0.5.0/botty/broadcast.py
--rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.5.0/botty/buttons.py
--rw-r--r--   0        0        0      294 2023-04-24 02:27:10.096409 aiogram-ext-0.5.0/botty/config.py
--rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.5.0/botty/context.py
--rw-r--r--   0        0        0     1763 2023-04-30 08:48:22.035344 aiogram-ext-0.5.0/botty/deps.py
--rw-r--r--   0        0        0     6569 2023-04-30 16:06:22.798732 aiogram-ext-0.5.0/botty/dispatcher.py
--rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.5.0/botty/env.py
--rw-r--r--   0        0        0      338 2023-04-28 10:47:37.416009 aiogram-ext-0.5.0/botty/errors.py
--rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.5.0/botty/filters.py
--rw-r--r--   0        0        0     1631 2023-04-30 07:30:17.108202 aiogram-ext-0.5.0/botty/helpers.py
--rw-r--r--   0        0        0      129 2023-04-28 11:17:12.416217 aiogram-ext-0.5.0/botty/html.py
--rw-r--r--   0        0        0      784 2023-04-28 11:05:50.359926 aiogram-ext-0.5.0/botty/keyboards.py
--rw-r--r--   0        0        0      592 2023-04-30 16:02:33.058131 aiogram-ext-0.5.0/botty/loader.py
--rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.5.0/botty/middlewares/__init__.py
--rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.5.0/botty/middlewares/_conversation.py
--rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.5.0/botty/middlewares/_membership.py
--rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.5.0/botty/middlewares/misc.py
--rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.5.0/botty/middlewares/throttling.py
--rw-r--r--   0        0        0      472 2023-04-30 07:10:43.133852 aiogram-ext-0.5.0/botty/r.py
--rw-r--r--   0        0        0      455 2023-04-30 16:06:22.816151 aiogram-ext-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.5.0/README.md
--rw-r--r--   0        0        0      315 2023-04-28 05:22:40.926562 aiogram-ext-0.5.0/tests/__main__.py
--rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1705 2023-04-30 08:48:21.984741 aiogram-ext-0.5.1/botty/__init__.py
+-rw-r--r--   0        0        0      794 2023-04-28 06:49:53.068602 aiogram-ext-0.5.1/botty/bot.py
+-rw-r--r--   0        0        0     1752 2023-04-30 07:58:02.593722 aiogram-ext-0.5.1/botty/broadcast.py
+-rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.5.1/botty/buttons.py
+-rw-r--r--   0        0        0      294 2023-04-24 02:27:10.096409 aiogram-ext-0.5.1/botty/config.py
+-rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.5.1/botty/context.py
+-rw-r--r--   0        0        0     1763 2023-04-30 08:48:22.035344 aiogram-ext-0.5.1/botty/deps.py
+-rw-r--r--   0        0        0     6505 2023-04-30 16:18:41.547471 aiogram-ext-0.5.1/botty/dispatcher.py
+-rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.5.1/botty/env.py
+-rw-r--r--   0        0        0      240 2023-04-30 16:18:41.592946 aiogram-ext-0.5.1/botty/errors.py
+-rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.5.1/botty/filters.py
+-rw-r--r--   0        0        0     1631 2023-04-30 07:30:17.108202 aiogram-ext-0.5.1/botty/helpers.py
+-rw-r--r--   0        0        0      129 2023-04-28 11:17:12.416217 aiogram-ext-0.5.1/botty/html.py
+-rw-r--r--   0        0        0      784 2023-04-28 11:05:50.359926 aiogram-ext-0.5.1/botty/keyboards.py
+-rw-r--r--   0        0        0      592 2023-04-30 16:02:33.058131 aiogram-ext-0.5.1/botty/loader.py
+-rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.5.1/botty/middlewares/__init__.py
+-rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.5.1/botty/middlewares/_conversation.py
+-rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.5.1/botty/middlewares/_membership.py
+-rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.5.1/botty/middlewares/misc.py
+-rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.5.1/botty/middlewares/throttling.py
+-rw-r--r--   0        0        0      472 2023-04-30 07:10:43.133852 aiogram-ext-0.5.1/botty/r.py
+-rw-r--r--   0        0        0      455 2023-04-30 16:19:03.620706 aiogram-ext-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.5.1/README.md
+-rw-r--r--   0        0        0      315 2023-04-28 05:22:40.926562 aiogram-ext-0.5.1/tests/__main__.py
+-rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.5.1/PKG-INFO
```

### Comparing `aiogram-ext-0.5.0/botty/__init__.py` & `aiogram-ext-0.5.1/botty/__init__.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.5.0/botty/bot.py` & `aiogram-ext-0.5.1/botty/bot.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.5.0/botty/broadcast.py` & `aiogram-ext-0.5.1/botty/broadcast.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.5.0/botty/buttons.py` & `aiogram-ext-0.5.1/botty/buttons.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.5.0/botty/context.py` & `aiogram-ext-0.5.1/botty/context.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.5.0/botty/deps.py` & `aiogram-ext-0.5.1/botty/deps.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.5.0/botty/dispatcher.py` & `aiogram-ext-0.5.1/botty/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 from typing import TypeVar, Awaitable
 
 import aiogram
 from aiogram.utils.executor import start_polling, Executor
 from aiohttp.web import Application
-import logging
+
 from .bot import Bot
 from .buttons import CallbackButton
 from .config import APP_PORT
 from .deps import State, MongoStorage, Update
 from .filters import (
     CallbackQueryButton,
     InlineQueryButton,
@@ -28,27 +28,27 @@
         self.TEXT = self.text()
         self.START = self.start()
         self.MESSAGE = self.message()
         self.ERROR = self.error()
 
     @staticmethod
     def _gen_payload(
-        locals_: dict, exclude: list[str] = None, default_exclude=("self", "cls")
+            locals_: dict, exclude: list[str] = None, default_exclude=("self", "cls")
     ):
         kwargs = locals_.pop("kwargs", {})
         locals_.update(kwargs)
 
         if exclude is None:
             exclude = []
         return {
             key: value
             for key, value in locals_.items()
             if key not in exclude + list(default_exclude)
-            and value is not None
-            and not key.startswith("_")
+               and value is not None
+               and not key.startswith("_")
         }
 
     def _setup_filters(self):
         filters_factory = self.filters_factory
         filters_factory.bind(
             StorageDataFilter,
             exclude_event_handlers=[
@@ -105,19 +105,19 @@
             for task in tasks:
                 await task
 
         self.ERROR(on_error)
         start_polling(self, on_startup=on_startup)
 
     def run_server(
-        self,
-        app_url: str,
-        app: Application = None,
-        path: str = "/bot",
-        port: int = APP_PORT,
+            self,
+            app_url: str,
+            app: Application = None,
+            path: str = "/bot",
+            port: int = APP_PORT,
     ):
         executor = Executor(self)
         executor.set_webhook(path, web_app=app)
         self._set_webhook(app_url + path)
         executor.run_app(port=port)
 
     def _set_webhook(self, url: str):
@@ -226,11 +226,9 @@
             chat_id=self._chat_id,
             user_id=self._user_id,
             **self._extra,
         )
         return deco(callback)
 
 
-async def on_error(update: Update, error: Exception):
-    logger = logging.getLogger()
-    logger.exception(f"{error=} on {update=}")
+async def on_error(_update: Update, _error: Exception):
     return True
```

### Comparing `aiogram-ext-0.5.0/botty/env.py` & `aiogram-ext-0.5.1/botty/env.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.5.0/botty/filters.py` & `aiogram-ext-0.5.1/botty/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.5.0/botty/helpers.py` & `aiogram-ext-0.5.1/botty/helpers.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.5.0/botty/keyboards.py` & `aiogram-ext-0.5.1/botty/keyboards.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.5.0/botty/loader.py` & `aiogram-ext-0.5.1/botty/loader.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.5.0/botty/middlewares/_conversation.py` & `aiogram-ext-0.5.1/botty/middlewares/_conversation.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.5.0/botty/middlewares/_membership.py` & `aiogram-ext-0.5.1/botty/middlewares/_membership.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.5.0/botty/middlewares/misc.py` & `aiogram-ext-0.5.1/botty/middlewares/misc.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.5.0/botty/middlewares/throttling.py` & `aiogram-ext-0.5.1/botty/middlewares/throttling.py`

 * *Files identical despite different names*

