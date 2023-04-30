# Comparing `tmp/DeltaKG-0.0.4.tar.gz` & `tmp/DeltaKG-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/DeltaKG-0.0.4.tar", last modified: Sun Apr 30 06:13:57 2023, max compression
+gzip compressed data, was "DeltaKG-0.0.5.tar", last modified: Sun Apr 30 06:29:07 2023, max compression
```

## Comparing `DeltaKG-0.0.4.tar` & `DeltaKG-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 06:13:57.001113 DeltaKG-0.0.4/
-drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 06:13:57.001113 DeltaKG-0.0.4/DeltaKG/
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-29 09:47:59.000000 DeltaKG-0.0.4/DeltaKG/__init__.py
-drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 06:13:57.001113 DeltaKG-0.0.4/DeltaKG/src/
--rwxr-xr-x   0 tbozhong  (1025) tbozhong  (1025)       41 2023-04-18 07:05:24.000000 DeltaKG-0.0.4/DeltaKG/src/__init__.py
-drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 06:13:57.001113 DeltaKG-0.0.4/DeltaKG/src/data/
--rwxr-xr-x   0 tbozhong  (1025) tbozhong  (1025)       79 2023-04-18 07:05:24.000000 DeltaKG-0.0.4/DeltaKG/src/data/__init__.py
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    15070 2023-04-18 07:05:24.000000 DeltaKG-0.0.4/DeltaKG/src/data/data_module.py
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    26588 2023-04-18 07:05:24.000000 DeltaKG-0.0.4/DeltaKG/src/data/processor.py
-drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 06:13:57.001113 DeltaKG-0.0.4/DeltaKG/src/models/
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)       73 2023-04-18 07:05:24.000000 DeltaKG-0.0.4/DeltaKG/src/models/__init__.py
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    71121 2023-04-18 07:05:24.000000 DeltaKG-0.0.4/DeltaKG/src/models/modeling_bert.py
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    36589 2023-04-18 07:05:24.000000 DeltaKG-0.0.4/DeltaKG/src/models/models.py
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     8635 2023-04-18 07:05:24.000000 DeltaKG-0.0.4/DeltaKG/src/models/optimization.py
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)   170056 2023-04-18 07:05:24.000000 DeltaKG-0.0.4/DeltaKG/src/models/trainer.py
-drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 06:13:57.001113 DeltaKG-0.0.4/DeltaKG.egg-info/
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)      488 2023-04-30 06:13:56.000000 DeltaKG-0.0.4/DeltaKG.egg-info/PKG-INFO
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)      450 2023-04-30 06:13:56.000000 DeltaKG-0.0.4/DeltaKG.egg-info/SOURCES.txt
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)        1 2023-04-30 06:13:56.000000 DeltaKG-0.0.4/DeltaKG.egg-info/dependency_links.txt
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)        8 2023-04-30 06:13:56.000000 DeltaKG-0.0.4/DeltaKG.egg-info/top_level.txt
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     1076 2023-04-18 07:08:58.000000 DeltaKG-0.0.4/LICENSE.txt
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)      488 2023-04-30 06:13:57.001113 DeltaKG-0.0.4/PKG-INFO
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)      842 2023-04-30 06:12:14.000000 DeltaKG-0.0.4/README.md
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)       38 2023-04-30 06:13:57.001113 DeltaKG-0.0.4/setup.cfg
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     1091 2023-04-30 06:13:51.000000 DeltaKG-0.0.4/setup.py
+drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 06:29:07.956257 DeltaKG-0.0.5/
+drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 06:29:07.952257 DeltaKG-0.0.5/DeltaKG/
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-29 09:47:59.000000 DeltaKG-0.0.5/DeltaKG/__init__.py
+drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 06:29:07.952257 DeltaKG-0.0.5/DeltaKG/src/
+-rwxr-xr-x   0 tbozhong  (1025) tbozhong  (1025)       41 2023-04-18 07:05:24.000000 DeltaKG-0.0.5/DeltaKG/src/__init__.py
+drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 06:29:07.952257 DeltaKG-0.0.5/DeltaKG/src/data/
+-rwxr-xr-x   0 tbozhong  (1025) tbozhong  (1025)       79 2023-04-18 07:05:24.000000 DeltaKG-0.0.5/DeltaKG/src/data/__init__.py
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    15070 2023-04-18 07:05:24.000000 DeltaKG-0.0.5/DeltaKG/src/data/data_module.py
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    26588 2023-04-18 07:05:24.000000 DeltaKG-0.0.5/DeltaKG/src/data/processor.py
+drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 06:29:07.952257 DeltaKG-0.0.5/DeltaKG/src/models/
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)       73 2023-04-18 07:05:24.000000 DeltaKG-0.0.5/DeltaKG/src/models/__init__.py
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    71121 2023-04-18 07:05:24.000000 DeltaKG-0.0.5/DeltaKG/src/models/modeling_bert.py
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    36589 2023-04-18 07:05:24.000000 DeltaKG-0.0.5/DeltaKG/src/models/models.py
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     8635 2023-04-18 07:05:24.000000 DeltaKG-0.0.5/DeltaKG/src/models/optimization.py
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)   170056 2023-04-18 07:05:24.000000 DeltaKG-0.0.5/DeltaKG/src/models/trainer.py
+drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 06:29:07.952257 DeltaKG-0.0.5/DeltaKG.egg-info/
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     1402 2023-04-30 06:29:07.000000 DeltaKG-0.0.5/DeltaKG.egg-info/PKG-INFO
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)      450 2023-04-30 06:29:07.000000 DeltaKG-0.0.5/DeltaKG.egg-info/SOURCES.txt
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)        1 2023-04-30 06:29:07.000000 DeltaKG-0.0.5/DeltaKG.egg-info/dependency_links.txt
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)        8 2023-04-30 06:29:07.000000 DeltaKG-0.0.5/DeltaKG.egg-info/top_level.txt
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     1076 2023-04-18 07:08:58.000000 DeltaKG-0.0.5/LICENSE.txt
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     1402 2023-04-30 06:29:07.956257 DeltaKG-0.0.5/PKG-INFO
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)      842 2023-04-30 06:12:14.000000 DeltaKG-0.0.5/README.md
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)       38 2023-04-30 06:29:07.956257 DeltaKG-0.0.5/setup.cfg
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     1177 2023-04-30 06:26:20.000000 DeltaKG-0.0.5/setup.py
```

### Comparing `DeltaKG-0.0.4/DeltaKG/src/data/data_module.py` & `DeltaKG-0.0.5/DeltaKG/src/data/data_module.py`

 * *Files identical despite different names*

### Comparing `DeltaKG-0.0.4/DeltaKG/src/data/processor.py` & `DeltaKG-0.0.5/DeltaKG/src/data/processor.py`

 * *Files identical despite different names*

### Comparing `DeltaKG-0.0.4/DeltaKG/src/models/modeling_bert.py` & `DeltaKG-0.0.5/DeltaKG/src/models/modeling_bert.py`

 * *Files identical despite different names*

### Comparing `DeltaKG-0.0.4/DeltaKG/src/models/models.py` & `DeltaKG-0.0.5/DeltaKG/src/models/models.py`

 * *Files identical despite different names*

### Comparing `DeltaKG-0.0.4/DeltaKG/src/models/optimization.py` & `DeltaKG-0.0.5/DeltaKG/src/models/optimization.py`

 * *Files identical despite different names*

### Comparing `DeltaKG-0.0.4/DeltaKG/src/models/trainer.py` & `DeltaKG-0.0.5/DeltaKG/src/models/trainer.py`

 * *Files identical despite different names*

### Comparing `DeltaKG-0.0.4/LICENSE.txt` & `DeltaKG-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DeltaKG-0.0.4/README.md` & `DeltaKG-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `DeltaKG-0.0.4/setup.py` & `DeltaKG-0.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # coding: utf-8
 import setuptools
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 
-try:
-    import pypandoc
-    long_description = pypandoc.convert('README.md', 'rst')
-except:
-    long_description = ""
-
+# try:
+#     import pypandoc
+#     long_description = pypandoc.convert('README.md', 'rst')
+# except:
+#     long_description = ""
+import pypandoc
+long_description = pypandoc.convert_file('README.md', 'rst')
 setuptools.setup(
     name='DeltaKG',
-    version='0.0.4',
+    version='0.0.5',
     description='A Library for Dynamically Editing PLMs-Based Knowledge Graph Embeddings.',
     author='Bozhong Tian',
     author_email='tbozhong@zju.edu.cn',
     url='https://github.com/zjunlp/PromptKG/tree/main/deltaKG',
     install_requires=[],
     # install_requires=['dataclasses==0.8', 'transformers==4.26.1', 'activations==0.1.0', 'flax==0.3.4',
     #                   'utils==1.0.1', 'pytorch_lightning==1.3.1', 'jsonlines', 'higher', 'allennlp', 'file_utils==0.0.1'],
```

