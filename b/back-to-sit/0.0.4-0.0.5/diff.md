# Comparing `tmp/back_to_sit-0.0.4.tar.gz` & `tmp/back_to_sit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "back_to_sit-0.0.4.tar", last modified: Sun Apr 30 15:02:59 2023, max compression
+gzip compressed data, was "back_to_sit-0.0.5.tar", last modified: Sun Apr 30 15:29:38 2023, max compression
```

## Comparing `back_to_sit-0.0.4.tar` & `back_to_sit-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 15:02:59.545193 back_to_sit-0.0.4/
--rw-r--r--   0 diegulio   (501) staff       (20)     1065 2023-03-16 05:01:50.000000 back_to_sit-0.0.4/LICENSE
--rw-r--r--   0 diegulio   (501) staff       (20)      281 2023-04-30 15:02:59.545031 back_to_sit-0.0.4/PKG-INFO
--rw-r--r--   0 diegulio   (501) staff       (20)       84 2023-03-16 05:01:50.000000 back_to_sit-0.0.4/README.md
-drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 15:02:59.544029 back_to_sit-0.0.4/back_to_sit/
--rw-r--r--   0 diegulio   (501) staff       (20)       59 2023-03-18 22:50:18.000000 back_to_sit-0.0.4/back_to_sit/__init__.py
--rw-r--r--   0 diegulio   (501) staff       (20)     1344 2023-03-20 23:06:53.000000 back_to_sit-0.0.4/back_to_sit/back_to_sit.py
-drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 15:02:59.544824 back_to_sit-0.0.4/back_to_sit.egg-info/
--rw-r--r--   0 diegulio   (501) staff       (20)      281 2023-04-30 15:02:59.000000 back_to_sit-0.0.4/back_to_sit.egg-info/PKG-INFO
--rw-r--r--   0 diegulio   (501) staff       (20)      266 2023-04-30 15:02:59.000000 back_to_sit-0.0.4/back_to_sit.egg-info/SOURCES.txt
--rw-r--r--   0 diegulio   (501) staff       (20)        1 2023-04-30 15:02:59.000000 back_to_sit-0.0.4/back_to_sit.egg-info/dependency_links.txt
--rw-r--r--   0 diegulio   (501) staff       (20)        9 2023-04-30 15:02:59.000000 back_to_sit-0.0.4/back_to_sit.egg-info/requires.txt
--rw-r--r--   0 diegulio   (501) staff       (20)       12 2023-04-30 15:02:59.000000 back_to_sit-0.0.4/back_to_sit.egg-info/top_level.txt
--rw-r--r--   0 diegulio   (501) staff       (20)      354 2023-04-30 15:02:36.000000 back_to_sit-0.0.4/pyproject.toml
--rw-r--r--   0 diegulio   (501) staff       (20)       38 2023-04-30 15:02:59.545248 back_to_sit-0.0.4/setup.cfg
--rw-r--r--   0 diegulio   (501) staff       (20)      732 2023-04-30 15:02:42.000000 back_to_sit-0.0.4/setup.py
+drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 15:29:38.725558 back_to_sit-0.0.5/
+-rw-r--r--   0 diegulio   (501) staff       (20)     1065 2023-03-16 05:01:50.000000 back_to_sit-0.0.5/LICENSE
+-rw-r--r--   0 diegulio   (501) staff       (20)      281 2023-04-30 15:29:38.725385 back_to_sit-0.0.5/PKG-INFO
+-rw-r--r--   0 diegulio   (501) staff       (20)       84 2023-03-16 05:01:50.000000 back_to_sit-0.0.5/README.md
+drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 15:29:38.724180 back_to_sit-0.0.5/back_to_sit/
+-rw-r--r--   0 diegulio   (501) staff       (20)       59 2023-03-18 22:50:18.000000 back_to_sit-0.0.5/back_to_sit/__init__.py
+-rw-r--r--   0 diegulio   (501) staff       (20)     1377 2023-04-30 15:23:05.000000 back_to_sit-0.0.5/back_to_sit/back_to_sit.py
+drwxr-xr-x   0 diegulio   (501) staff       (20)        0 2023-04-30 15:29:38.725168 back_to_sit-0.0.5/back_to_sit.egg-info/
+-rw-r--r--   0 diegulio   (501) staff       (20)      281 2023-04-30 15:29:38.000000 back_to_sit-0.0.5/back_to_sit.egg-info/PKG-INFO
+-rw-r--r--   0 diegulio   (501) staff       (20)      266 2023-04-30 15:29:38.000000 back_to_sit-0.0.5/back_to_sit.egg-info/SOURCES.txt
+-rw-r--r--   0 diegulio   (501) staff       (20)        1 2023-04-30 15:29:38.000000 back_to_sit-0.0.5/back_to_sit.egg-info/dependency_links.txt
+-rw-r--r--   0 diegulio   (501) staff       (20)        9 2023-04-30 15:29:38.000000 back_to_sit-0.0.5/back_to_sit.egg-info/requires.txt
+-rw-r--r--   0 diegulio   (501) staff       (20)       12 2023-04-30 15:29:38.000000 back_to_sit-0.0.5/back_to_sit.egg-info/top_level.txt
+-rw-r--r--   0 diegulio   (501) staff       (20)      354 2023-04-30 15:21:22.000000 back_to_sit-0.0.5/pyproject.toml
+-rw-r--r--   0 diegulio   (501) staff       (20)       38 2023-04-30 15:29:38.725621 back_to_sit-0.0.5/setup.cfg
+-rw-r--r--   0 diegulio   (501) staff       (20)      732 2023-04-30 15:21:38.000000 back_to_sit-0.0.5/setup.py
```

### Comparing `back_to_sit-0.0.4/LICENSE` & `back_to_sit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `back_to_sit-0.0.4/back_to_sit/back_to_sit.py` & `back_to_sit-0.0.5/back_to_sit/back_to_sit.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     end_time = time.time()
     # Create an event loop
     if start_time is not None:
         message = message + f"\n Time taken to execute: {(end_time - start_time)/60:.6f} minutes"
     loop = asyncio.new_event_loop()
     # Run the coroutine in the event loop
     loop.run_until_complete(__send_telegram_message(message, chat_id, token))
+    loop.stop()
+    loop.close()
 
 def back_to_sit_decorator(base_message, chat_id, token):
     """
     Decorator that send a message when the function is done
     and report the time taken to execute the function
     """
     def decorator(func):
```

### Comparing `back_to_sit-0.0.4/setup.py` & `back_to_sit-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4' 
+VERSION = '0.0.5' 
 DESCRIPTION = 'Back to sit when the your code is ready'
 LONG_DESCRIPTION = 'A package that send a message to your telegram when your code is ready'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="back_to_sit",
```

