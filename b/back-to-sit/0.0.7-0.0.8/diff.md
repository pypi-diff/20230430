# Comparing `tmp/back_to_sit-0.0.7.tar.gz` & `tmp/back_to_sit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "back_to_sit-0.0.7.tar", last modified: Sun Apr 30 15:57:27 2023, max compression
+gzip compressed data, was "back_to_sit-0.0.8.tar", last modified: Sun Apr 30 16:06:18 2023, max compression
```

## Comparing `back_to_sit-0.0.7.tar` & `back_to_sit-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 15:57:27.937192 back_to_sit-0.0.7/
--rw-r--r--   0 diegulio   (501) staff       (20)     1065 2023-03-16 05:01:50.000000 back_to_sit-0.0.7/LICENSE
--rw-r--r--   0 diegulio   (501) staff       (20)      281 2023-04-30 15:57:27.937047 back_to_sit-0.0.7/PKG-INFO
--rw-r--r--   0 diegulio   (501) staff       (20)       84 2023-03-16 05:01:50.000000 back_to_sit-0.0.7/README.md
-drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 15:57:27.935977 back_to_sit-0.0.7/back_to_sit/
--rw-r--r--   0 diegulio   (501) staff       (20)       59 2023-03-18 22:50:18.000000 back_to_sit-0.0.7/back_to_sit/__init__.py
--rw-r--r--   0 diegulio   (501) staff       (20)     1598 2023-04-30 15:54:53.000000 back_to_sit-0.0.7/back_to_sit/back_to_sit.py
-drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 15:57:27.936855 back_to_sit-0.0.7/back_to_sit.egg-info/
--rw-r--r--   0 diegulio   (501) staff       (20)      281 2023-04-30 15:57:27.000000 back_to_sit-0.0.7/back_to_sit.egg-info/PKG-INFO
--rw-r--r--   0 diegulio   (501) staff       (20)      266 2023-04-30 15:57:27.000000 back_to_sit-0.0.7/back_to_sit.egg-info/SOURCES.txt
--rw-r--r--   0 diegulio   (501) staff       (20)        1 2023-04-30 15:57:27.000000 back_to_sit-0.0.7/back_to_sit.egg-info/dependency_links.txt
--rw-r--r--   0 diegulio   (501) staff       (20)        9 2023-04-30 15:57:27.000000 back_to_sit-0.0.7/back_to_sit.egg-info/requires.txt
--rw-r--r--   0 diegulio   (501) staff       (20)       12 2023-04-30 15:57:27.000000 back_to_sit-0.0.7/back_to_sit.egg-info/top_level.txt
--rw-r--r--   0 diegulio   (501) staff       (20)      355 2023-04-30 15:57:20.000000 back_to_sit-0.0.7/pyproject.toml
--rw-r--r--   0 diegulio   (501) staff       (20)       38 2023-04-30 15:57:27.937241 back_to_sit-0.0.7/setup.cfg
--rw-r--r--   0 diegulio   (501) staff       (20)      732 2023-04-30 15:57:21.000000 back_to_sit-0.0.7/setup.py
+drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 16:06:18.155442 back_to_sit-0.0.8/
+-rw-r--r--   0 diegulio   (501) staff       (20)     1065 2023-03-16 05:01:50.000000 back_to_sit-0.0.8/LICENSE
+-rw-r--r--   0 diegulio   (501) staff       (20)      281 2023-04-30 16:06:18.155294 back_to_sit-0.0.8/PKG-INFO
+-rw-r--r--   0 diegulio   (501) staff       (20)       84 2023-03-16 05:01:50.000000 back_to_sit-0.0.8/README.md
+drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 16:06:18.154352 back_to_sit-0.0.8/back_to_sit/
+-rw-r--r--   0 diegulio   (501) staff       (20)       59 2023-03-18 22:50:18.000000 back_to_sit-0.0.8/back_to_sit/__init__.py
+-rw-r--r--   0 diegulio   (501) staff       (20)     1593 2023-04-30 16:06:05.000000 back_to_sit-0.0.8/back_to_sit/back_to_sit.py
+drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 16:06:18.155106 back_to_sit-0.0.8/back_to_sit.egg-info/
+-rw-r--r--   0 diegulio   (501) staff       (20)      281 2023-04-30 16:06:18.000000 back_to_sit-0.0.8/back_to_sit.egg-info/PKG-INFO
+-rw-r--r--   0 diegulio   (501) staff       (20)      266 2023-04-30 16:06:18.000000 back_to_sit-0.0.8/back_to_sit.egg-info/SOURCES.txt
+-rw-r--r--   0 diegulio   (501) staff       (20)        1 2023-04-30 16:06:18.000000 back_to_sit-0.0.8/back_to_sit.egg-info/dependency_links.txt
+-rw-r--r--   0 diegulio   (501) staff       (20)        9 2023-04-30 16:06:18.000000 back_to_sit-0.0.8/back_to_sit.egg-info/requires.txt
+-rw-r--r--   0 diegulio   (501) staff       (20)       12 2023-04-30 16:06:18.000000 back_to_sit-0.0.8/back_to_sit.egg-info/top_level.txt
+-rw-r--r--   0 diegulio   (501) staff       (20)      355 2023-04-30 16:06:14.000000 back_to_sit-0.0.8/pyproject.toml
+-rw-r--r--   0 diegulio   (501) staff       (20)       38 2023-04-30 16:06:18.155494 back_to_sit-0.0.8/setup.cfg
+-rw-r--r--   0 diegulio   (501) staff       (20)      732 2023-04-30 16:06:12.000000 back_to_sit-0.0.8/setup.py
```

### Comparing `back_to_sit-0.0.7/LICENSE` & `back_to_sit-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `back_to_sit-0.0.7/back_to_sit/back_to_sit.py` & `back_to_sit-0.0.8/back_to_sit/back_to_sit.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,31 +18,29 @@
     # Create an event loop
     if start_time is not None:
         message = message + f"\n Time taken to execute: {(end_time - start_time)/60:.6f} minutes"
 
     if notebook:
         loop = asyncio.get_event_loop()
         loop.create_task(__send_telegram_message(message, chat_id, token))
-        loop.stop()
-        loop.close()
     else:
         loop = asyncio.new_event_loop()
         # Run the coroutine in the event loop
         loop.run_until_complete(__send_telegram_message(message, chat_id, token))
         loop.stop()
         loop.close()
 
-def back_to_sit_decorator(base_message, chat_id, token):
+def back_to_sit_decorator(base_message, chat_id, token, notebook = True):
     """
     Decorator that send a message when the function is done
     and report the time taken to execute the function
     """
     def decorator(func):
         def wrapper(*args, **kwargs):
             start_time = time.time()
             result = func(*args, **kwargs)
             end_time = time.time()
             NEW_MESSAGE = base_message + f"\n Time taken to execute {func.__name__}: {(end_time - start_time)/60:.6f} minutes"
-            back_to_sit(message=NEW_MESSAGE, chat_id=chat_id, token=token)
+            back_to_sit(message=NEW_MESSAGE, chat_id=chat_id, token=token, notebook=notebook)
             return result
         return wrapper
     return decorator
```

### Comparing `back_to_sit-0.0.7/setup.py` & `back_to_sit-0.0.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7' 
+VERSION = '0.0.8' 
 DESCRIPTION = 'Back to sit when the your code is ready'
 LONG_DESCRIPTION = 'A package that send a message to your telegram when your code is ready'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="back_to_sit",
```

