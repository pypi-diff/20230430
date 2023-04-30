# Comparing `tmp/DeltaKG-0.0.1.tar.gz` & `tmp/DeltaKG-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeltaKG-0.0.1.tar", last modified: Sat Apr 29 09:39:14 2023, max compression
+gzip compressed data, was "DeltaKG-0.0.2.tar", last modified: Sun Apr 30 05:56:32 2023, max compression
```

## Comparing `DeltaKG-0.0.1.tar` & `DeltaKG-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,25 @@
-drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-29 09:39:14.449031 DeltaKG-0.0.1/
-drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-29 09:39:14.449031 DeltaKG-0.0.1/DeltaKG.egg-info/
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)      474 2023-04-29 09:39:14.000000 DeltaKG-0.0.1/DeltaKG.egg-info/PKG-INFO
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)      154 2023-04-29 09:39:14.000000 DeltaKG-0.0.1/DeltaKG.egg-info/SOURCES.txt
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)        1 2023-04-29 09:39:14.000000 DeltaKG-0.0.1/DeltaKG.egg-info/dependency_links.txt
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)        1 2023-04-29 09:39:14.000000 DeltaKG-0.0.1/DeltaKG.egg-info/top_level.txt
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     1076 2023-04-18 07:08:58.000000 DeltaKG-0.0.1/LICENSE.txt
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)      474 2023-04-29 09:39:14.449031 DeltaKG-0.0.1/PKG-INFO
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     8787 2023-04-29 09:34:59.000000 DeltaKG-0.0.1/README.md
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)       38 2023-04-29 09:39:14.449031 DeltaKG-0.0.1/setup.cfg
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     1077 2023-04-18 07:25:25.000000 DeltaKG-0.0.1/setup.py
+drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 05:56:32.283145 DeltaKG-0.0.2/
+drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 05:56:32.279145 DeltaKG-0.0.2/DeltaKG/
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-29 09:47:59.000000 DeltaKG-0.0.2/DeltaKG/__init__.py
+drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 05:56:32.279145 DeltaKG-0.0.2/DeltaKG/src/
+-rwxr-xr-x   0 tbozhong  (1025) tbozhong  (1025)       41 2023-04-18 07:05:24.000000 DeltaKG-0.0.2/DeltaKG/src/__init__.py
+drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 05:56:32.279145 DeltaKG-0.0.2/DeltaKG/src/data/
+-rwxr-xr-x   0 tbozhong  (1025) tbozhong  (1025)       79 2023-04-18 07:05:24.000000 DeltaKG-0.0.2/DeltaKG/src/data/__init__.py
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    15070 2023-04-18 07:05:24.000000 DeltaKG-0.0.2/DeltaKG/src/data/data_module.py
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    26588 2023-04-18 07:05:24.000000 DeltaKG-0.0.2/DeltaKG/src/data/processor.py
+drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 05:56:32.279145 DeltaKG-0.0.2/DeltaKG/src/models/
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)       73 2023-04-18 07:05:24.000000 DeltaKG-0.0.2/DeltaKG/src/models/__init__.py
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    71121 2023-04-18 07:05:24.000000 DeltaKG-0.0.2/DeltaKG/src/models/modeling_bert.py
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    36589 2023-04-18 07:05:24.000000 DeltaKG-0.0.2/DeltaKG/src/models/models.py
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     8635 2023-04-18 07:05:24.000000 DeltaKG-0.0.2/DeltaKG/src/models/optimization.py
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)   170056 2023-04-18 07:05:24.000000 DeltaKG-0.0.2/DeltaKG/src/models/trainer.py
+drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 05:56:32.279145 DeltaKG-0.0.2/DeltaKG.egg-info/
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)      488 2023-04-30 05:56:32.000000 DeltaKG-0.0.2/DeltaKG.egg-info/PKG-INFO
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)      450 2023-04-30 05:56:32.000000 DeltaKG-0.0.2/DeltaKG.egg-info/SOURCES.txt
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)        1 2023-04-30 05:56:32.000000 DeltaKG-0.0.2/DeltaKG.egg-info/dependency_links.txt
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)        8 2023-04-30 05:56:32.000000 DeltaKG-0.0.2/DeltaKG.egg-info/top_level.txt
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     1076 2023-04-18 07:08:58.000000 DeltaKG-0.0.2/LICENSE.txt
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)      488 2023-04-30 05:56:32.283145 DeltaKG-0.0.2/PKG-INFO
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     8835 2023-04-30 05:53:09.000000 DeltaKG-0.0.2/README.md
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)       38 2023-04-30 05:56:32.283145 DeltaKG-0.0.2/setup.cfg
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     1091 2023-04-30 05:54:20.000000 DeltaKG-0.0.2/setup.py
```

### Comparing `DeltaKG-0.0.1/LICENSE.txt` & `DeltaKG-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DeltaKG-0.0.1/README.md` & `DeltaKG-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 <div align="center">
-    <!-- <img src="https://github.com/zjunlp/PromptKG/blob/main/resources/lambda_logo.png" width="550px"> -->
-    <h1> DeltaKG </h1>
+    <img src="https://github.com/zjunlp/PromptKG/blob/main/resources/deltakg_logo.png" width="550px">
     <p> <b>
-        A dynamic, PLM-based library for Knowledge Graph Embeddings.</b>
+        A Library for Dynamically Editing PLMs-Based Knowledge Graph Embeddings.</b>
     </p>
     
 ------
 
 <p align="center">
   <a href="#overview">Overview</a> •
   <a href="#installation">Installation</a> •
   <a href="#how-to-run">How To Run</a> •
   <a href="https://arxiv.org/pdf/2301.10405">Paper</a> •
-  <a href="https://medium.com/@tbozhong/a935ba8769a7">Medium</a> •
+  <a href="https://medium.com/@jack16900/deltakg-a-library-for-dynamically-editing-plm-based-kg-embeddings-243d59a8f168">Medium</a> •
   <a href="#how-to-cite">Citation</a> •
   <a href="#other-kg-representation-open-source-projects">Others</a> 
 </p>
 </div>
 
 ## Overview
 Knowledge graph embedding (KGE) is a method for representing symbolic facts in low-dimensional vector spaces, with the goal of projecting relations and entities into a continuous vector space. This approach enhances knowledge reasoning capabilities and facilitates application to downstream tasks.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-                             ****** DeltaKG ******
-         A dynamic, PLM-based library for Knowledge Graph Embeddings.
+   [https://github.com/zjunlp/PromptKG/blob/main/resources/deltakg_logo.png]
+   A Library for Dynamically Editing PLMs-Based Knowledge Graph Embeddings.
                                     ------
 Overview â¢ Installation â¢ How_To_Run â¢ Paper â¢ Medium â¢ Citation â¢
                                     Others
 ## Overview Knowledge graph embedding (KGE) is a method for representing
 symbolic facts in low-dimensional vector spaces, with the goal of projecting
 relations and entities into a continuous vector space. This approach enhances
 knowledge reasoning capabilities and facilitates application to downstream
```

### Comparing `DeltaKG-0.0.1/setup.py` & `DeltaKG-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     import pypandoc
     long_description = pypandoc.convert('README.md', 'rst')
 except:
     long_description = ""
 
 setuptools.setup(
     name='DeltaKG',
-    version='0.0.1',
-    description='A library for dynamically editing PLM-based KG embeddings.',
+    version='0.0.2',
+    description='A Library for Dynamically Editing PLMs-Based Knowledge Graph Embeddings.',
     author='Bozhong Tian',
     author_email='tbozhong@zju.edu.cn',
     url='https://github.com/zjunlp/PromptKG/tree/main/deltaKG',
     install_requires=[],
     # install_requires=['dataclasses==0.8', 'transformers==4.26.1', 'activations==0.1.0', 'flax==0.3.4',
     #                   'utils==1.0.1', 'pytorch_lightning==1.3.1', 'jsonlines', 'higher', 'allennlp', 'file_utils==0.0.1'],
     keywords='knowledge graph embedding edit',
```

