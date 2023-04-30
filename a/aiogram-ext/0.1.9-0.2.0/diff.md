# Comparing `tmp/aiogram-ext-0.1.9.tar.gz` & `tmp/aiogram-ext-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-ext-0.1.9.tar", last modified: Mon Apr 24 03:51:49 2023, max compression
+gzip compressed data, was "aiogram-ext-0.2.0.tar", last modified: Sun Apr 30 07:11:34 2023, max compression
```

## Comparing `aiogram-ext-0.1.9.tar` & `aiogram-ext-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
--rw-r--r--   0        0        0     1059 2023-04-24 03:32:27.312633 aiogram-ext-0.1.9/botty/__init__.py
--rw-r--r--   0        0        0      251 2023-04-14 12:15:49.770806 aiogram-ext-0.1.9/botty/bot.py
--rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.1.9/botty/buttons.py
--rw-r--r--   0        0        0      294 2023-04-24 02:27:10.096409 aiogram-ext-0.1.9/botty/config.py
--rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.1.9/botty/context.py
--rw-r--r--   0        0        0     1665 2023-04-16 22:10:48.295151 aiogram-ext-0.1.9/botty/deps.py
--rw-r--r--   0        0        0     5999 2023-04-20 17:26:03.233411 aiogram-ext-0.1.9/botty/dispatcher.py
--rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.1.9/botty/env.py
--rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.1.9/botty/filters.py
--rw-r--r--   0        0        0      993 2023-04-24 03:51:46.752347 aiogram-ext-0.1.9/botty/helpers.py
--rw-r--r--   0        0        0      722 2023-04-12 14:37:01.113297 aiogram-ext-0.1.9/botty/keyboards.py
--rw-r--r--   0        0        0      669 2023-04-24 03:10:12.100277 aiogram-ext-0.1.9/botty/loader.py
--rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.1.9/botty/middlewares/__init__.py
--rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.1.9/botty/middlewares/_conversation.py
--rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.1.9/botty/middlewares/_membership.py
--rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.1.9/botty/middlewares/misc.py
--rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.1.9/botty/middlewares/throttling.py
--rw-r--r--   0        0        0      455 2023-04-24 03:51:46.760862 aiogram-ext-0.1.9/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.1.9/README.md
--rw-r--r--   0        0        0      239 2023-04-16 23:01:01.500707 aiogram-ext-0.1.9/tests/__main__.py
--rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1506 2023-04-28 11:48:42.660234 aiogram-ext-0.2.0/botty/__init__.py
+-rw-r--r--   0        0        0      794 2023-04-28 06:49:53.068602 aiogram-ext-0.2.0/botty/bot.py
+-rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.2.0/botty/buttons.py
+-rw-r--r--   0        0        0      294 2023-04-24 02:27:10.096409 aiogram-ext-0.2.0/botty/config.py
+-rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.2.0/botty/context.py
+-rw-r--r--   0        0        0     1727 2023-04-28 11:48:42.664740 aiogram-ext-0.2.0/botty/deps.py
+-rw-r--r--   0        0        0     6312 2023-04-28 10:41:21.032710 aiogram-ext-0.2.0/botty/dispatcher.py
+-rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.2.0/botty/env.py
+-rw-r--r--   0        0        0      338 2023-04-28 10:47:37.416009 aiogram-ext-0.2.0/botty/errors.py
+-rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.2.0/botty/filters.py
+-rw-r--r--   0        0        0     1439 2023-04-30 07:10:43.177855 aiogram-ext-0.2.0/botty/helpers.py
+-rw-r--r--   0        0        0      129 2023-04-28 11:17:12.416217 aiogram-ext-0.2.0/botty/html.py
+-rw-r--r--   0        0        0      784 2023-04-28 11:05:50.359926 aiogram-ext-0.2.0/botty/keyboards.py
+-rw-r--r--   0        0        0      739 2023-04-28 06:52:22.537117 aiogram-ext-0.2.0/botty/loader.py
+-rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.2.0/botty/middlewares/__init__.py
+-rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.2.0/botty/middlewares/_conversation.py
+-rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.2.0/botty/middlewares/_membership.py
+-rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.2.0/botty/middlewares/misc.py
+-rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.2.0/botty/middlewares/throttling.py
+-rw-r--r--   0        0        0      472 2023-04-30 07:10:43.133852 aiogram-ext-0.2.0/botty/r.py
+-rw-r--r--   0        0        0      455 2023-04-30 07:11:29.022398 aiogram-ext-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.2.0/README.md
+-rw-r--r--   0        0        0      315 2023-04-28 05:22:40.926562 aiogram-ext-0.2.0/tests/__main__.py
+-rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.2.0/PKG-INFO
```

### Comparing `aiogram-ext-0.1.9/botty/__init__.py` & `aiogram-ext-0.2.0/botty/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,26 +4,34 @@
     InlineQueryButton,
     ContactRequestButton,
     InlineButton,
 )
 from .deps import (
     Message,
     Query,
+    Chat,
+    User,
     FSMContext,
     State,
     StatesGroup,
     SkipHandler,
     CancelHandler,
     TelegramAPIError,
+    Update,
+    BadRequest,
+    RetryAfter,
 )
 from .dispatcher import Dispatcher
 from .env import env
-from .helpers import reply, is_group, is_private, is_channel, ask, get_photo_url
-from .keyboards import ReplyKeyboard, InlineKeyboard
-from .loader import bot, dp, logger, app, run
+from .errors import NoSendTextRights, NoSendPhotoRights
+from .helpers import reply, is_group, is_private, is_channel, ask, get_photo_url, edit
+from .html import bold, link
+from .keyboards import ReplyKeyboard, InlineKeyboard, ReplyMarkup
+from .loader import bot, dp, logger, app, run, loop
+from .r import r, Answer, e
 
 __all__ = [
     "Dispatcher",
     "ReplyKeyboard",
     "InlineKeyboard",
     "InlineButton",
     "CallbackButton",
@@ -46,8 +54,23 @@
     "is_private",
     "is_group",
     "is_channel",
     "app",
     "run",
     "ask",
     "get_photo_url",
+    "edit",
+    "Chat",
+    "User",
+    "loop",
+    "Update",
+    "BadRequest",
+    "NoSendTextRights",
+    "NoSendPhotoRights",
+    "ReplyMarkup",
+    "r",
+    "Answer",
+    "bold",
+    "link",
+    "e",
+    "RetryAfter",
 ]
```

### Comparing `aiogram-ext-0.1.9/botty/buttons.py` & `aiogram-ext-0.2.0/botty/buttons.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.9/botty/context.py` & `aiogram-ext-0.2.0/botty/context.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.9/botty/deps.py` & `aiogram-ext-0.2.0/botty/deps.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Poll,
     PollAnswer,
     ChatMemberUpdated,
     ReplyKeyboardRemove,
 )
 from aiogram.utils import executor
 from aiogram.utils.mixins import ContextInstanceMixin
-from aiogram.utils.exceptions import TelegramAPIError
+from aiogram.utils.exceptions import TelegramAPIError, BadRequest, RetryAfter
 
 __all__ = [
     "ReplyKeyboardMarkup",
     "InlineKeyboardMarkup",
     "InlineKeyboardButton",
     "KeyboardButton",
     "Bot",
@@ -61,10 +61,12 @@
     "environ",
     "MongoStorage",
     "SkipHandler",
     "CancelHandler",
     "StatesGroup",
     "ReplyMarkup",
     "TelegramAPIError",
+    "BadRequest",
+    "RetryAfter",
 ]
 
 ReplyMarkup = ReplyKeyboardMarkup | InlineKeyboardMarkup | ReplyKeyboardRemove
```

### Comparing `aiogram-ext-0.1.9/botty/dispatcher.py` & `aiogram-ext-0.2.0/botty/dispatcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import asyncio
-from typing import TypeVar
+from typing import TypeVar, Awaitable
 
 import aiogram
-from aiogram.utils.executor import Executor
+from aiogram.utils.executor import start_polling, Executor
 from aiohttp.web import Application
+
 from .bot import Bot
 from .buttons import CallbackButton
+from .config import APP_PORT
 from .deps import State, MongoStorage
 from .filters import (
     CallbackQueryButton,
     InlineQueryButton,
     MessageButton,
     StorageDataFilter,
 )
-from .config import APP_PORT
 
 T = TypeVar("T")
 
 
 class Dispatcher(aiogram.Dispatcher):
-    def __init__(self, bot: Bot, storage: MongoStorage):
-        super().__init__(bot, storage=storage)
+    def __init__(self, bot: Bot, storage: MongoStorage, loop=None):
+        super().__init__(bot, loop, storage)
         self.CONTACT = self.contact()
         self.DOCUMENT = self.document()
         self.PHOTO = self.photo()
         self.TEXT = self.text()
         self.START = self.start()
         self.MESSAGE = self.message()
 
@@ -73,15 +74,15 @@
 
     def command(self, command: str):
         return CommandHandler(self, command)
 
     def start(self, state: str | State | None = "*"):
         return self.command("start").state(state)
 
-    def button(self, button: CallbackButton):
+    def button(self, button: CallbackButton | list[CallbackButton]):
         return ButtonHandler(self, button)
 
     def text(self, text: str = None):
         return TextHandler(self, text)
 
     def contact(self):
         return ContactHandler(self)
@@ -91,16 +92,23 @@
 
     def photo(self):
         return PhotoHandler(self)
 
     def message(self):
         return MessageHandler(self)
 
-    def run(self):
-        Executor(self).start_polling()
+    def error(self, exc: Exception):
+        return self.errors_handler(exception=exc)
+
+    def run(self, *tasks: Awaitable):
+        async def on_startup(_):
+            for task in tasks:
+                await task
+
+        start_polling(self, on_startup=on_startup)
 
     def run_server(
         self,
         app_url: str,
         app: Application = None,
         path: str = "/bot",
         port: int = APP_PORT,
@@ -127,15 +135,15 @@
         self._state = value
         return self
 
     def chat_id(self, value: int):
         self._chat_id = value
         return self
 
-    def user_id(self, value: int):
+    def user_id(self, value: int | list[int]):
         self._user_id = value
         return self
 
     def extra(self, **kwargs):
         self._extra = kwargs
         return self
 
@@ -201,15 +209,15 @@
 
 class DocumentHandler(MessageHandler):
     def __init__(self, dp: Dispatcher):
         super().__init__(dp, "document")
 
 
 class ButtonHandler(Handler):
-    def __init__(self, dp: Dispatcher, button: CallbackButton):
+    def __init__(self, dp: Dispatcher, button: CallbackButton | list[CallbackButton]):
         super().__init__(dp)
         self._button = button
 
     def __call__(self, callback):
         deco = self._dp.callback_query_handler(
             button=self._button,
             state=self._state,
```

### Comparing `aiogram-ext-0.1.9/botty/env.py` & `aiogram-ext-0.2.0/botty/env.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.9/botty/filters.py` & `aiogram-ext-0.2.0/botty/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.9/botty/helpers.py` & `aiogram-ext-0.2.0/botty/helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,56 @@
-from typing import Awaitable
-
 from aiogram.types import ChatType
 
-from .deps import ReplyKeyboardRemove, Message, ReplyMarkup, Query, Chat, State
-
-
-def reply(
-    msg: Message | Query,
-    text: str,
-    markup: ReplyMarkup | bool = None,
-) -> Awaitable[Message]:
-    if isinstance(msg, Query):
-        msg = msg.message
+from .deps import (
+    ReplyKeyboardRemove,
+    Message,
+    ReplyMarkup,
+    Query,
+    Chat,
+    State,
+    InlineKeyboardMarkup,
+)
+
+
+async def reply(
+        event: Message | Query,
+        text: str,
+        markup: ReplyMarkup | bool = None,
+        *,
+        quote: bool = False,
+) -> Message:
+    if isinstance(event, Query):
+        await event.answer()
+        event = event.message
     if markup is False:
         markup = ReplyKeyboardRemove()
-    return msg.answer(text, reply_markup=markup)
+    return await event.answer(text, reply_markup=markup, reply=quote)
 
 
 async def ask(
-    state: State,
-    msg: Message,
-    text: str,
-    markup: ReplyMarkup | bool = False,
+        state: State,
+        msg: Message,
+        text: str,
+        markup: ReplyMarkup | bool = False,
 ):
     await state.set()
     await reply(msg, text, markup)
 
 
+async def edit(
+        event: Message | Query,
+        text: str,
+        markup: InlineKeyboardMarkup = None,
+) -> Message:
+    if isinstance(event, Query):
+        await event.answer()
+        event = event.message
+    return await event.edit_text(text, reply_markup=markup)
+
+
 def is_channel(chat: Chat) -> bool:
     return chat.type in [ChatType.CHANNEL]
 
 
 def is_group(chat: Chat) -> bool:
     return chat.type in [ChatType.GROUP, ChatType.SUPERGROUP]
```

### Comparing `aiogram-ext-0.1.9/botty/keyboards.py` & `aiogram-ext-0.2.0/botty/keyboards.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,7 +20,10 @@
 class InlineKeyboard(InlineKeyboardMarkup):
     buttons: list[InlineButton] = None
     row_width = 1
 
     def __init__(self, *buttons: InlineButton):
         super().__init__(row_width=self.row_width)
         self.add(*(self.buttons or []), *buttons)
+
+
+ReplyMarkup = ReplyKeyboardMarkup | InlineKeyboardMarkup
```

### Comparing `aiogram-ext-0.1.9/botty/loader.py` & `aiogram-ext-0.2.0/botty/loader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import logging
+from asyncio import new_event_loop
 
 from aiohttp.web import Application
 
 from .bot import Bot
 from .config import BOT_TOKEN, MONGO, APP_URL
 from .deps import MongoStorage, Update
 from .dispatcher import Dispatcher
 
-bot = Bot(BOT_TOKEN)
-
 storage = MongoStorage(
     db_name=MONGO.DB,
     host=MONGO.HOST,
     username=MONGO.USER,
     password=MONGO.PASSWORD,
 )
 
-dp = Dispatcher(bot, storage=storage)
-Dispatcher.set_current(dp)
+loop = new_event_loop()
+bot = Bot(BOT_TOKEN, loop)
+dp = Dispatcher(bot, storage, loop)
 logger = logging.getLogger()
+app = Application(loop=loop)
+
+Dispatcher.set_current(dp)
 
 
 @dp.errors_handler()
 async def _(update: Update, error: Exception):
     logger.exception(f"{error=} on {update=}")
     return True
 
 
-app = Application()
-
-
 def run():
     dp.run_server(APP_URL, app)
```

### Comparing `aiogram-ext-0.1.9/botty/middlewares/_conversation.py` & `aiogram-ext-0.2.0/botty/middlewares/_conversation.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.9/botty/middlewares/_membership.py` & `aiogram-ext-0.2.0/botty/middlewares/_membership.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.9/botty/middlewares/misc.py` & `aiogram-ext-0.2.0/botty/middlewares/misc.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.9/botty/middlewares/throttling.py` & `aiogram-ext-0.2.0/botty/middlewares/throttling.py`

 * *Files identical despite different names*

