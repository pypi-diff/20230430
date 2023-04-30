# Comparing `tmp/aiogram-ext-0.2.1.tar.gz` & `tmp/aiogram-ext-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-ext-0.2.1.tar", last modified: Sun Apr 30 07:13:50 2023, max compression
+gzip compressed data, was "aiogram-ext-0.3.0.tar", last modified: Sun Apr 30 07:31:09 2023, max compression
```

## Comparing `aiogram-ext-0.2.1.tar` & `aiogram-ext-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1506 2023-04-28 11:48:42.660234 aiogram-ext-0.2.1/botty/__init__.py
--rw-r--r--   0        0        0      794 2023-04-28 06:49:53.068602 aiogram-ext-0.2.1/botty/bot.py
--rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.2.1/botty/buttons.py
--rw-r--r--   0        0        0      294 2023-04-24 02:27:10.096409 aiogram-ext-0.2.1/botty/config.py
--rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.2.1/botty/context.py
--rw-r--r--   0        0        0     1727 2023-04-28 11:48:42.664740 aiogram-ext-0.2.1/botty/deps.py
--rw-r--r--   0        0        0     6312 2023-04-28 10:41:21.032710 aiogram-ext-0.2.1/botty/dispatcher.py
--rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.2.1/botty/env.py
--rw-r--r--   0        0        0      338 2023-04-28 10:47:37.416009 aiogram-ext-0.2.1/botty/errors.py
--rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.2.1/botty/filters.py
--rw-r--r--   0        0        0     1439 2023-04-30 07:10:43.177855 aiogram-ext-0.2.1/botty/helpers.py
--rw-r--r--   0        0        0      129 2023-04-28 11:17:12.416217 aiogram-ext-0.2.1/botty/html.py
--rw-r--r--   0        0        0      784 2023-04-28 11:05:50.359926 aiogram-ext-0.2.1/botty/keyboards.py
--rw-r--r--   0        0        0      739 2023-04-28 06:52:22.537117 aiogram-ext-0.2.1/botty/loader.py
--rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.2.1/botty/middlewares/__init__.py
--rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.2.1/botty/middlewares/_conversation.py
--rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.2.1/botty/middlewares/_membership.py
--rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.2.1/botty/middlewares/misc.py
--rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.2.1/botty/middlewares/throttling.py
--rw-r--r--   0        0        0      472 2023-04-30 07:10:43.133852 aiogram-ext-0.2.1/botty/r.py
--rw-r--r--   0        0        0      455 2023-04-30 07:13:45.066585 aiogram-ext-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.2.1/README.md
--rw-r--r--   0        0        0      315 2023-04-28 05:22:40.926562 aiogram-ext-0.2.1/tests/__main__.py
--rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1599 2023-04-30 07:30:16.997181 aiogram-ext-0.3.0/botty/__init__.py
+-rw-r--r--   0        0        0      794 2023-04-28 06:49:53.068602 aiogram-ext-0.3.0/botty/bot.py
+-rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.3.0/botty/buttons.py
+-rw-r--r--   0        0        0      294 2023-04-24 02:27:10.096409 aiogram-ext-0.3.0/botty/config.py
+-rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.3.0/botty/context.py
+-rw-r--r--   0        0        0     1727 2023-04-28 11:48:42.664740 aiogram-ext-0.3.0/botty/deps.py
+-rw-r--r--   0        0        0     6312 2023-04-28 10:41:21.032710 aiogram-ext-0.3.0/botty/dispatcher.py
+-rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.3.0/botty/env.py
+-rw-r--r--   0        0        0      338 2023-04-28 10:47:37.416009 aiogram-ext-0.3.0/botty/errors.py
+-rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.3.0/botty/filters.py
+-rw-r--r--   0        0        0     1631 2023-04-30 07:30:17.108202 aiogram-ext-0.3.0/botty/helpers.py
+-rw-r--r--   0        0        0      129 2023-04-28 11:17:12.416217 aiogram-ext-0.3.0/botty/html.py
+-rw-r--r--   0        0        0      784 2023-04-28 11:05:50.359926 aiogram-ext-0.3.0/botty/keyboards.py
+-rw-r--r--   0        0        0      739 2023-04-28 06:52:22.537117 aiogram-ext-0.3.0/botty/loader.py
+-rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.3.0/botty/middlewares/__init__.py
+-rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.3.0/botty/middlewares/_conversation.py
+-rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.3.0/botty/middlewares/_membership.py
+-rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.3.0/botty/middlewares/misc.py
+-rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.3.0/botty/middlewares/throttling.py
+-rw-r--r--   0        0        0      472 2023-04-30 07:10:43.133852 aiogram-ext-0.3.0/botty/r.py
+-rw-r--r--   0        0        0      455 2023-04-30 07:31:04.549895 aiogram-ext-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.3.0/README.md
+-rw-r--r--   0        0        0      315 2023-04-28 05:22:40.926562 aiogram-ext-0.3.0/tests/__main__.py
+-rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.3.0/PKG-INFO
```

### Comparing `aiogram-ext-0.2.1/botty/__init__.py` & `aiogram-ext-0.3.0/botty/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,24 @@
     Update,
     BadRequest,
     RetryAfter,
 )
 from .dispatcher import Dispatcher
 from .env import env
 from .errors import NoSendTextRights, NoSendPhotoRights
-from .helpers import reply, is_group, is_private, is_channel, ask, get_photo_url, edit
+from .helpers import (
+    reply,
+    is_group,
+    is_private,
+    is_channel,
+    ask,
+    get_photo_url,
+    edit,
+    obtain_invite_link,
+)
 from .html import bold, link
 from .keyboards import ReplyKeyboard, InlineKeyboard, ReplyMarkup
 from .loader import bot, dp, logger, app, run, loop
 from .r import r, Answer, e
 
 __all__ = [
     "Dispatcher",
@@ -69,8 +78,9 @@
     "ReplyMarkup",
     "r",
     "Answer",
     "bold",
     "link",
     "e",
     "RetryAfter",
+    "obtain_invite_link",
 ]
```

### Comparing `aiogram-ext-0.2.1/botty/bot.py` & `aiogram-ext-0.3.0/botty/bot.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.2.1/botty/buttons.py` & `aiogram-ext-0.3.0/botty/buttons.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.2.1/botty/context.py` & `aiogram-ext-0.3.0/botty/context.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.2.1/botty/deps.py` & `aiogram-ext-0.3.0/botty/deps.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.2.1/botty/dispatcher.py` & `aiogram-ext-0.3.0/botty/dispatcher.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.2.1/botty/env.py` & `aiogram-ext-0.3.0/botty/env.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.2.1/botty/filters.py` & `aiogram-ext-0.3.0/botty/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.2.1/botty/helpers.py` & `aiogram-ext-0.3.0/botty/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 from aiogram.types import ChatType
+from .loader import bot
 
 from .deps import (
     ReplyKeyboardRemove,
     Message,
     ReplyMarkup,
     Query,
     Chat,
     State,
     InlineKeyboardMarkup,
 )
 
 
 async def reply(
-        event: Message | Query,
-        text: str,
-        markup: ReplyMarkup | bool = None,
-        *,
-        quote: bool = False,
+    event: Message | Query,
+    text: str,
+    markup: ReplyMarkup | bool = None,
+    *,
+    quote: bool = False,
 ) -> Message:
     if isinstance(event, Query):
         await event.answer()
         event = event.message
     if markup is False:
         markup = ReplyKeyboardRemove()
     return await event.answer(text, reply_markup=markup, reply=quote)
 
 
 async def ask(
-        state: State,
-        msg: Message,
-        text: str,
-        markup: ReplyMarkup | bool = False,
+    state: State,
+    msg: Message,
+    text: str,
+    markup: ReplyMarkup | bool = False,
 ):
     await state.set()
     await reply(msg, text, markup)
 
 
 async def edit(
-        event: Message | Query,
-        text: str,
-        markup: InlineKeyboardMarkup = None,
+    event: Message | Query,
+    text: str,
+    markup: InlineKeyboardMarkup = None,
 ) -> Message:
     if isinstance(event, Query):
         await event.answer()
         event = event.message
     return await event.edit_text(text, reply_markup=markup)
 
 
@@ -57,7 +58,14 @@
 
 def is_private(chat: Chat) -> bool:
     return chat.type in [ChatType.PRIVATE]
 
 
 async def get_photo_url(msg: Message) -> str:
     return await msg.photo[-1].get_url()
+
+
+async def obtain_invite_link(chat_id: int) -> str:
+    chat = await bot.get_chat(chat_id)
+    if not chat.invite_link:
+        chat.invite_link = await chat.create_invite_link()
+    return chat.invite_link
```

### Comparing `aiogram-ext-0.2.1/botty/keyboards.py` & `aiogram-ext-0.3.0/botty/keyboards.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.2.1/botty/loader.py` & `aiogram-ext-0.3.0/botty/loader.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.2.1/botty/middlewares/_conversation.py` & `aiogram-ext-0.3.0/botty/middlewares/_conversation.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.2.1/botty/middlewares/_membership.py` & `aiogram-ext-0.3.0/botty/middlewares/_membership.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.2.1/botty/middlewares/misc.py` & `aiogram-ext-0.3.0/botty/middlewares/misc.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.2.1/botty/middlewares/throttling.py` & `aiogram-ext-0.3.0/botty/middlewares/throttling.py`

 * *Files identical despite different names*

