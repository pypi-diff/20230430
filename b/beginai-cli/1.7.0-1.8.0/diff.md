# Comparing `tmp/beginai-cli-1.7.0.tar.gz` & `tmp/beginai-cli-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beginai-cli-1.7.0.tar", last modified: Wed Apr 26 22:08:45 2023, max compression
+gzip compressed data, was "beginai-cli-1.8.0.tar", last modified: Sun Apr 30 00:58:37 2023, max compression
```

## Comparing `beginai-cli-1.7.0.tar` & `beginai-cli-1.8.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:45.485932 beginai-cli-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-26 22:08:45.485932 beginai-cli-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-26 22:08:32.000000 beginai-cli-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:45.481932 beginai-cli-1.7.0/beginai_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:32.000000 beginai-cli-1.7.0/beginai_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-04-26 22:08:32.000000 beginai-cli-1.7.0/beginai_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:45.481932 beginai-cli-1.7.0/beginai_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-26 22:08:45.000000 beginai-cli-1.7.0/beginai_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-26 22:08:45.000000 beginai-cli-1.7.0/beginai_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 22:08:45.000000 beginai-cli-1.7.0/beginai_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-26 22:08:45.000000 beginai-cli-1.7.0/beginai_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-26 22:08:45.000000 beginai-cli-1.7.0/beginai_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 22:08:45.000000 beginai-cli-1.7.0/beginai_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-26 22:08:45.485932 beginai-cli-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-26 22:08:43.000000 beginai-cli-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:37.467450 beginai-cli-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-30 00:58:37.467450 beginai-cli-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-30 00:58:24.000000 beginai-cli-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:37.467450 beginai-cli-1.8.0/beginai_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:24.000000 beginai-cli-1.8.0/beginai_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-04-30 00:58:24.000000 beginai-cli-1.8.0/beginai_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:37.467450 beginai-cli-1.8.0/beginai_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-30 00:58:37.000000 beginai-cli-1.8.0/beginai_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-30 00:58:37.000000 beginai-cli-1.8.0/beginai_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 00:58:37.000000 beginai-cli-1.8.0/beginai_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-30 00:58:37.000000 beginai-cli-1.8.0/beginai_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-30 00:58:37.000000 beginai-cli-1.8.0/beginai_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-30 00:58:37.000000 beginai-cli-1.8.0/beginai_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 00:58:37.467450 beginai-cli-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-30 00:58:36.000000 beginai-cli-1.8.0/setup.py
```

### Comparing `beginai-cli-1.7.0/PKG-INFO` & `beginai-cli-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beginai-cli
-Version: 1.7.0
+Version: 1.8.0
 Summary: A CLI part of Begin AI ecosystesm that enables batch processing with minimum code.
 Home-page: https://docs.begin.ai
 Author: Begin AI Research & Engineering
 Author-email: engineering@begin.ai
 License: Proprietary
 Description: 
                 This is Begin AI CLI for both batch processing.
```

### Comparing `beginai-cli-1.7.0/README.md` & `beginai-cli-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `beginai-cli-1.7.0/beginai_cli/main.py` & `beginai-cli-1.8.0/beginai_cli/main.py`

 * *Files identical despite different names*

### Comparing `beginai-cli-1.7.0/beginai_cli.egg-info/PKG-INFO` & `beginai-cli-1.8.0/beginai_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beginai-cli
-Version: 1.7.0
+Version: 1.8.0
 Summary: A CLI part of Begin AI ecosystesm that enables batch processing with minimum code.
 Home-page: https://docs.begin.ai
 Author: Begin AI Research & Engineering
 Author-email: engineering@begin.ai
 License: Proprietary
 Description: 
                 This is Begin AI CLI for both batch processing.
```

### Comparing `beginai-cli-1.7.0/setup.py` & `beginai-cli-1.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 REQ_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "pip-dep")
 core_reqs, core_dependency_links = get_requirements(os.path.join(REQ_DIR, "requirements.txt"))
 
 
 if __name__ == "__main__":
     setup(
         name="beginai-cli",
-        version="1.7.0",
+        version="1.8.0",
         author="Begin AI Research & Engineering",
         author_email="engineering@begin.ai",
         description="A CLI part of Begin AI ecosystesm that enables batch processing with minimum code.",
         long_description="""
         This is Begin AI CLI for both batch processing.
         It can be used to process historical data and generate signatures that are sent over to Begin AI servers
```

