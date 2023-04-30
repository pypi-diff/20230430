# Comparing `tmp/instld-0.0.5.tar.gz` & `tmp/instld-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instld-0.0.5.tar", last modified: Sun Apr 30 11:55:42 2023, max compression
+gzip compressed data, was "instld-0.0.6.tar", last modified: Sun Apr 30 12:01:48 2023, max compression
```

## Comparing `instld-0.0.5.tar` & `instld-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 11:55:42.715731 instld-0.0.5/
--rw-r--r--   0 pomponchik   (501) staff       (20)     1067 2023-04-02 20:16:05.000000 instld-0.0.5/LICENSE
--rw-r--r--   0 pomponchik   (501) staff       (20)     2029 2023-04-30 11:55:42.715466 instld-0.0.5/PKG-INFO
--rw-r--r--   0 pomponchik   (501) staff       (20)     1445 2023-04-09 18:09:35.000000 instld-0.0.5/README.md
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 11:55:42.713474 instld-0.0.5/installed/
--rw-r--r--   0 pomponchik   (501) staff       (20)      107 2023-04-29 15:51:00.000000 instld-0.0.5/installed/__init__.py
--rw-r--r--   0 pomponchik   (501) staff       (20)     1326 2023-04-29 21:56:56.000000 instld-0.0.5/installed/context_manager.py
--rw-r--r--   0 pomponchik   (501) staff       (20)      239 2023-04-30 11:52:44.000000 instld-0.0.5/installed/empty_logger.py
--rw-r--r--   0 pomponchik   (501) staff       (20)       50 2023-04-29 15:42:44.000000 instld-0.0.5/installed/errors.py
--rw-r--r--   0 pomponchik   (501) staff       (20)      415 2023-04-29 21:55:47.000000 instld-0.0.5/installed/proxy_module.py
--rw-r--r--   0 pomponchik   (501) staff       (20)      737 2023-04-30 11:53:49.000000 instld-0.0.5/installed/runner.py
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 11:55:42.714400 instld-0.0.5/instld.egg-info/
--rw-r--r--   0 pomponchik   (501) staff       (20)     2029 2023-04-30 11:55:42.000000 instld-0.0.5/instld.egg-info/PKG-INFO
--rw-r--r--   0 pomponchik   (501) staff       (20)      340 2023-04-30 11:55:42.000000 instld-0.0.5/instld.egg-info/SOURCES.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)        1 2023-04-30 11:55:42.000000 instld-0.0.5/instld.egg-info/dependency_links.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)       16 2023-04-30 11:55:42.000000 instld-0.0.5/instld.egg-info/top_level.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)       38 2023-04-30 11:55:42.715806 instld-0.0.5/setup.cfg
--rw-r--r--   0 pomponchik   (501) staff       (20)      865 2023-04-29 15:41:33.000000 instld-0.0.5/setup.py
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 11:55:42.710887 instld-0.0.5/tests/
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 11:55:42.714836 instld-0.0.5/tests/units/
--rw-r--r--   0 pomponchik   (501) staff       (20)        0 2023-04-29 15:45:14.000000 instld-0.0.5/tests/units/__init__.py
--rw-r--r--   0 pomponchik   (501) staff       (20)       52 2023-04-29 15:52:00.000000 instld-0.0.5/tests/units/test_errors.py
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 12:01:48.033189 instld-0.0.6/
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1067 2023-04-02 20:16:05.000000 instld-0.0.6/LICENSE
+-rw-r--r--   0 pomponchik   (501) staff       (20)     2029 2023-04-30 12:01:48.032925 instld-0.0.6/PKG-INFO
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1445 2023-04-09 18:09:35.000000 instld-0.0.6/README.md
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 12:01:48.031282 instld-0.0.6/installed/
+-rw-r--r--   0 pomponchik   (501) staff       (20)      107 2023-04-29 15:51:00.000000 instld-0.0.6/installed/__init__.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1326 2023-04-29 21:56:56.000000 instld-0.0.6/installed/context_manager.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)      239 2023-04-30 11:52:44.000000 instld-0.0.6/installed/empty_logger.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)       50 2023-04-29 15:42:44.000000 instld-0.0.6/installed/errors.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)      415 2023-04-29 21:55:47.000000 instld-0.0.6/installed/proxy_module.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)      726 2023-04-30 11:58:19.000000 instld-0.0.6/installed/runner.py
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 12:01:48.032106 instld-0.0.6/instld.egg-info/
+-rw-r--r--   0 pomponchik   (501) staff       (20)     2029 2023-04-30 12:01:47.000000 instld-0.0.6/instld.egg-info/PKG-INFO
+-rw-r--r--   0 pomponchik   (501) staff       (20)      340 2023-04-30 12:01:47.000000 instld-0.0.6/instld.egg-info/SOURCES.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)        1 2023-04-30 12:01:47.000000 instld-0.0.6/instld.egg-info/dependency_links.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)       16 2023-04-30 12:01:47.000000 instld-0.0.6/instld.egg-info/top_level.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)       38 2023-04-30 12:01:48.033266 instld-0.0.6/setup.cfg
+-rw-r--r--   0 pomponchik   (501) staff       (20)      865 2023-04-30 11:59:06.000000 instld-0.0.6/setup.py
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 12:01:48.028558 instld-0.0.6/tests/
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 12:01:48.032539 instld-0.0.6/tests/units/
+-rw-r--r--   0 pomponchik   (501) staff       (20)        0 2023-04-29 15:45:14.000000 instld-0.0.6/tests/units/__init__.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)       52 2023-04-29 15:52:00.000000 instld-0.0.6/tests/units/test_errors.py
```

### Comparing `instld-0.0.5/LICENSE` & `instld-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `instld-0.0.5/PKG-INFO` & `instld-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instld
-Version: 0.0.5
+Version: 0.0.6
 Summary: The simplest package management from the source code
 Home-page: https://github.com/pomponchik/installed
 Author: Evgeniy Blinov
 Author-email: zheni-b@yandex.ru
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `instld-0.0.5/README.md` & `instld-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `instld-0.0.5/installed/context_manager.py` & `instld-0.0.6/installed/context_manager.py`

 * *Files identical despite different names*

### Comparing `instld-0.0.5/installed/runner.py` & `instld-0.0.6/installed/runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import subprocess
 
 
-def run_python(args: list[str], logger):
+def run_python(args, logger):
     all_args = [sys.executable, *args]
     args_string_representation = " ".join(all_args)
 
     try:
         logger.info(f'The beginning of the execution of the command "{args_string_representation}".')
         subprocess.check_call(all_args, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         logger.info(f'The command "{args_string_representation}" has been executed.')
```

### Comparing `instld-0.0.5/instld.egg-info/PKG-INFO` & `instld-0.0.6/instld.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instld
-Version: 0.0.5
+Version: 0.0.6
 Summary: The simplest package management from the source code
 Home-page: https://github.com/pomponchik/installed
 Author: Evgeniy Blinov
 Author-email: zheni-b@yandex.ru
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `instld-0.0.5/setup.py` & `instld-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = []
 
 setup(
     name="instld",
-    version="0.0.5",
+    version="0.0.6",
     author="Evgeniy Blinov",
     author_email="zheni-b@yandex.ru",
     description="The simplest package management from the source code",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/pomponchik/installed",
     packages=find_packages(exclude=["tests"]),
```

