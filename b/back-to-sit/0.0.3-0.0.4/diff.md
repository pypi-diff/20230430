# Comparing `tmp/back_to_sit-0.0.3.tar.gz` & `tmp/back_to_sit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "back_to_sit-0.0.3.tar", last modified: Sat Mar 18 23:08:20 2023, max compression
+gzip compressed data, was "back_to_sit-0.0.4.tar", last modified: Sun Apr 30 15:02:59 2023, max compression
```

## Comparing `back_to_sit-0.0.3.tar` & `back_to_sit-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-03-18 23:08:20.554801 back_to_sit-0.0.3/
--rw-r--r--   0 diegulio   (501) staff       (20)     1065 2023-03-16 05:01:50.000000 back_to_sit-0.0.3/LICENSE
--rw-r--r--   0 diegulio   (501) staff       (20)      281 2023-03-18 23:08:20.554665 back_to_sit-0.0.3/PKG-INFO
--rw-r--r--   0 diegulio   (501) staff       (20)       84 2023-03-16 05:01:50.000000 back_to_sit-0.0.3/README.md
-drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-03-18 23:08:20.553682 back_to_sit-0.0.3/back_to_sit/
--rw-r--r--   0 diegulio   (501) staff       (20)       59 2023-03-18 22:50:18.000000 back_to_sit-0.0.3/back_to_sit/__init__.py
--rw-r--r--   0 diegulio   (501) staff       (20)     1194 2023-03-18 23:05:04.000000 back_to_sit-0.0.3/back_to_sit/back_to_sit.py
-drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-03-18 23:08:20.554476 back_to_sit-0.0.3/back_to_sit.egg-info/
--rw-r--r--   0 diegulio   (501) staff       (20)      281 2023-03-18 23:08:20.000000 back_to_sit-0.0.3/back_to_sit.egg-info/PKG-INFO
--rw-r--r--   0 diegulio   (501) staff       (20)      266 2023-03-18 23:08:20.000000 back_to_sit-0.0.3/back_to_sit.egg-info/SOURCES.txt
--rw-r--r--   0 diegulio   (501) staff       (20)        1 2023-03-18 23:08:20.000000 back_to_sit-0.0.3/back_to_sit.egg-info/dependency_links.txt
--rw-r--r--   0 diegulio   (501) staff       (20)        9 2023-03-18 23:08:20.000000 back_to_sit-0.0.3/back_to_sit.egg-info/requires.txt
--rw-r--r--   0 diegulio   (501) staff       (20)       12 2023-03-18 23:08:20.000000 back_to_sit-0.0.3/back_to_sit.egg-info/top_level.txt
--rw-r--r--   0 diegulio   (501) staff       (20)      355 2023-03-18 23:07:29.000000 back_to_sit-0.0.3/pyproject.toml
--rw-r--r--   0 diegulio   (501) staff       (20)       38 2023-03-18 23:08:20.554857 back_to_sit-0.0.3/setup.cfg
--rw-r--r--   0 diegulio   (501) staff       (20)      732 2023-03-18 23:07:27.000000 back_to_sit-0.0.3/setup.py
+drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 15:02:59.545193 back_to_sit-0.0.4/
+-rw-r--r--   0 diegulio   (501) staff       (20)     1065 2023-03-16 05:01:50.000000 back_to_sit-0.0.4/LICENSE
+-rw-r--r--   0 diegulio   (501) staff       (20)      281 2023-04-30 15:02:59.545031 back_to_sit-0.0.4/PKG-INFO
+-rw-r--r--   0 diegulio   (501) staff       (20)       84 2023-03-16 05:01:50.000000 back_to_sit-0.0.4/README.md
+drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 15:02:59.544029 back_to_sit-0.0.4/back_to_sit/
+-rw-r--r--   0 diegulio   (501) staff       (20)       59 2023-03-18 22:50:18.000000 back_to_sit-0.0.4/back_to_sit/__init__.py
+-rw-r--r--   0 diegulio   (501) staff       (20)     1344 2023-03-20 23:06:53.000000 back_to_sit-0.0.4/back_to_sit/back_to_sit.py
+drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 15:02:59.544824 back_to_sit-0.0.4/back_to_sit.egg-info/
+-rw-r--r--   0 diegulio   (501) staff       (20)      281 2023-04-30 15:02:59.000000 back_to_sit-0.0.4/back_to_sit.egg-info/PKG-INFO
+-rw-r--r--   0 diegulio   (501) staff       (20)      266 2023-04-30 15:02:59.000000 back_to_sit-0.0.4/back_to_sit.egg-info/SOURCES.txt
+-rw-r--r--   0 diegulio   (501) staff       (20)        1 2023-04-30 15:02:59.000000 back_to_sit-0.0.4/back_to_sit.egg-info/dependency_links.txt
+-rw-r--r--   0 diegulio   (501) staff       (20)        9 2023-04-30 15:02:59.000000 back_to_sit-0.0.4/back_to_sit.egg-info/requires.txt
+-rw-r--r--   0 diegulio   (501) staff       (20)       12 2023-04-30 15:02:59.000000 back_to_sit-0.0.4/back_to_sit.egg-info/top_level.txt
+-rw-r--r--   0 diegulio   (501) staff       (20)      354 2023-04-30 15:02:36.000000 back_to_sit-0.0.4/pyproject.toml
+-rw-r--r--   0 diegulio   (501) staff       (20)       38 2023-04-30 15:02:59.545248 back_to_sit-0.0.4/setup.cfg
+-rw-r--r--   0 diegulio   (501) staff       (20)      732 2023-04-30 15:02:42.000000 back_to_sit-0.0.4/setup.py
```

### Comparing `back_to_sit-0.0.3/LICENSE` & `back_to_sit-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `back_to_sit-0.0.3/back_to_sit/back_to_sit.py` & `back_to_sit-0.0.4/back_to_sit/back_to_sit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import telegram
 import asyncio
 import time 
-import functools
-import wrapt
 
 async def __send_telegram_message(message, chat_id, token):
     # Set up the bot
     bot = telegram.Bot(token=token)
 
     # Send a message
     await bot.send_message(chat_id=chat_id, text=message)
 
 
-def back_to_sit(message, chat_id, token):
+def back_to_sit(message, chat_id, token, start_time = None):
     """
     Function that send message when is called
     """
+    end_time = time.time()
     # Create an event loop
+    if start_time is not None:
+        message = message + f"\n Time taken to execute: {(end_time - start_time)/60:.6f} minutes"
     loop = asyncio.new_event_loop()
     # Run the coroutine in the event loop
     loop.run_until_complete(__send_telegram_message(message, chat_id, token))
 
 def back_to_sit_decorator(base_message, chat_id, token):
     """
     Decorator that send a message when the function is done
     and report the time taken to execute the function
     """
     def decorator(func):
         def wrapper(*args, **kwargs):
             start_time = time.time()
             result = func(*args, **kwargs)
             end_time = time.time()
-            NEW_MESSAGE = base_message + f"\n Time taken to execute {func.__name__}: {end_time - start_time:.6f} seconds"
+            NEW_MESSAGE = base_message + f"\n Time taken to execute {func.__name__}: {(end_time - start_time)/60:.6f} minutes"
             back_to_sit(message=NEW_MESSAGE, chat_id=chat_id, token=token)
             return result
         return wrapper
     return decorator
```

### Comparing `back_to_sit-0.0.3/setup.py` & `back_to_sit-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3' 
+VERSION = '0.0.4' 
 DESCRIPTION = 'Back to sit when the your code is ready'
 LONG_DESCRIPTION = 'A package that send a message to your telegram when your code is ready'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="back_to_sit",
```

