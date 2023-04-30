# Comparing `tmp/arcangelai-2.0.2.tar.gz` & `tmp/arcangelai-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcangelai-2.0.2.tar", last modified: Sat Apr 29 23:08:10 2023, max compression
+gzip compressed data, was "arcangelai-2.0.3.tar", last modified: Sun Apr 30 00:40:06 2023, max compression
```

## Comparing `arcangelai-2.0.2.tar` & `arcangelai-2.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 william    (506) staff       (20)        0 2023-04-29 23:08:10.585640 arcangelai-2.0.2/
--rw-r--r--   0 william    (506) staff       (20)       77 2023-04-29 21:40:13.000000 arcangelai-2.0.2/CHANGELOG.txt
--rw-r--r--   0 william    (506) staff       (20)     1067 2023-04-29 21:25:13.000000 arcangelai-2.0.2/LICENSE
--rw-r--r--   0 william    (506) staff       (20)       25 2023-04-29 21:53:13.000000 arcangelai-2.0.2/MANIFEST.in
--rw-r--r--   0 william    (506) staff       (20)      554 2023-04-29 23:08:10.585116 arcangelai-2.0.2/PKG-INFO
--rw-r--r--   0 william    (506) staff       (20)       36 2023-04-29 22:47:34.000000 arcangelai-2.0.2/README.md
-drwxr-xr-x   0 william    (506) staff       (20)        0 2023-04-29 23:08:10.580990 arcangelai-2.0.2/arcangelai/
--rw-r--r--   0 william    (506) staff       (20)      881 2023-04-29 23:07:52.000000 arcangelai-2.0.2/arcangelai/__init__.py
-drwxr-xr-x   0 william    (506) staff       (20)        0 2023-04-29 23:08:10.584610 arcangelai-2.0.2/arcangelai.egg-info/
--rw-r--r--   0 william    (506) staff       (20)      554 2023-04-29 23:08:10.000000 arcangelai-2.0.2/arcangelai.egg-info/PKG-INFO
--rw-r--r--   0 william    (506) staff       (20)      211 2023-04-29 23:08:10.000000 arcangelai-2.0.2/arcangelai.egg-info/SOURCES.txt
--rw-r--r--   0 william    (506) staff       (20)        1 2023-04-29 23:08:10.000000 arcangelai-2.0.2/arcangelai.egg-info/dependency_links.txt
--rw-r--r--   0 william    (506) staff       (20)       11 2023-04-29 23:08:10.000000 arcangelai-2.0.2/arcangelai.egg-info/top_level.txt
--rw-r--r--   0 william    (506) staff       (20)       38 2023-04-29 23:08:10.585753 arcangelai-2.0.2/setup.cfg
--rw-r--r--   0 william    (506) staff       (20)      646 2023-04-29 23:08:04.000000 arcangelai-2.0.2/setup.py
+drwxr-xr-x   0 william    (506) staff       (20)        0 2023-04-30 00:40:06.582791 arcangelai-2.0.3/
+-rw-r--r--   0 william    (506) staff       (20)       77 2023-04-29 21:40:13.000000 arcangelai-2.0.3/CHANGELOG.txt
+-rw-r--r--   0 william    (506) staff       (20)     1067 2023-04-29 21:25:13.000000 arcangelai-2.0.3/LICENSE
+-rw-r--r--   0 william    (506) staff       (20)       25 2023-04-29 21:53:13.000000 arcangelai-2.0.3/MANIFEST.in
+-rw-r--r--   0 william    (506) staff       (20)      554 2023-04-30 00:40:06.582232 arcangelai-2.0.3/PKG-INFO
+-rw-r--r--   0 william    (506) staff       (20)       36 2023-04-29 22:47:34.000000 arcangelai-2.0.3/README.md
+drwxr-xr-x   0 william    (506) staff       (20)        0 2023-04-30 00:40:06.578772 arcangelai-2.0.3/arcangelai/
+-rw-r--r--   0 william    (506) staff       (20)      795 2023-04-30 00:38:42.000000 arcangelai-2.0.3/arcangelai/__init__.py
+drwxr-xr-x   0 william    (506) staff       (20)        0 2023-04-30 00:40:06.581723 arcangelai-2.0.3/arcangelai.egg-info/
+-rw-r--r--   0 william    (506) staff       (20)      554 2023-04-30 00:40:06.000000 arcangelai-2.0.3/arcangelai.egg-info/PKG-INFO
+-rw-r--r--   0 william    (506) staff       (20)      211 2023-04-30 00:40:06.000000 arcangelai-2.0.3/arcangelai.egg-info/SOURCES.txt
+-rw-r--r--   0 william    (506) staff       (20)        1 2023-04-30 00:40:06.000000 arcangelai-2.0.3/arcangelai.egg-info/dependency_links.txt
+-rw-r--r--   0 william    (506) staff       (20)       11 2023-04-30 00:40:06.000000 arcangelai-2.0.3/arcangelai.egg-info/top_level.txt
+-rw-r--r--   0 william    (506) staff       (20)       38 2023-04-30 00:40:06.582916 arcangelai-2.0.3/setup.cfg
+-rw-r--r--   0 william    (506) staff       (20)      646 2023-04-30 00:39:10.000000 arcangelai-2.0.3/setup.py
```

### Comparing `arcangelai-2.0.2/LICENSE` & `arcangelai-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arcangelai-2.0.2/PKG-INFO` & `arcangelai-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcangelai
-Version: 2.0.2
+Version: 2.0.3
 Summary: Autonomous AI
 Home-page: 
 Author: Arc Angel Ai
 Author-email: arcangelgpt@gmail.com
 License: MIT
 Keywords: autonomous
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arcangelai-2.0.2/arcangelai/__init__.py` & `arcangelai-2.0.3/arcangelai/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,8 +21,8 @@
         # Check if the API call was successful
         if response.status_code == 200:
             # Get the JSON response
             json_response = response.json()
             return json_response
         else:
             # Handle the error
-            return {"response": str(response.status_code), "message": "Error: API call failed with status code "}
+            return response
```

### Comparing `arcangelai-2.0.2/arcangelai.egg-info/PKG-INFO` & `arcangelai-2.0.3/arcangelai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcangelai
-Version: 2.0.2
+Version: 2.0.3
 Summary: Autonomous AI
 Home-page: 
 Author: Arc Angel Ai
 Author-email: arcangelgpt@gmail.com
 License: MIT
 Keywords: autonomous
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arcangelai-2.0.2/setup.py` & `arcangelai-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   'Intended Audience :: Education',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='arcangelai',
-  version='2.0.2',
+  version='2.0.3',
   description='Autonomous AI',
   long_description_content_type='text/x-rst',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Arc Angel Ai',
   author_email='arcangelgpt@gmail.com',
   license='MIT',
```

