# Comparing `tmp/DeltaKG-0.0.2.tar.gz` & `tmp/DeltaKG-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeltaKG-0.0.2.tar", last modified: Sun Apr 30 05:56:32 2023, max compression
+gzip compressed data, was "DeltaKG-0.0.3.tar", last modified: Sun Apr 30 06:03:28 2023, max compression
```

## Comparing `DeltaKG-0.0.2.tar` & `DeltaKG-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 05:56:32.283145 DeltaKG-0.0.2/
-drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 05:56:32.279145 DeltaKG-0.0.2/DeltaKG/
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-29 09:47:59.000000 DeltaKG-0.0.2/DeltaKG/__init__.py
-drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 05:56:32.279145 DeltaKG-0.0.2/DeltaKG/src/
--rwxr-xr-x   0 tbozhong  (1025) tbozhong  (1025)       41 2023-04-18 07:05:24.000000 DeltaKG-0.0.2/DeltaKG/src/__init__.py
-drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 05:56:32.279145 DeltaKG-0.0.2/DeltaKG/src/data/
--rwxr-xr-x   0 tbozhong  (1025) tbozhong  (1025)       79 2023-04-18 07:05:24.000000 DeltaKG-0.0.2/DeltaKG/src/data/__init__.py
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    15070 2023-04-18 07:05:24.000000 DeltaKG-0.0.2/DeltaKG/src/data/data_module.py
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    26588 2023-04-18 07:05:24.000000 DeltaKG-0.0.2/DeltaKG/src/data/processor.py
-drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 05:56:32.279145 DeltaKG-0.0.2/DeltaKG/src/models/
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)       73 2023-04-18 07:05:24.000000 DeltaKG-0.0.2/DeltaKG/src/models/__init__.py
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    71121 2023-04-18 07:05:24.000000 DeltaKG-0.0.2/DeltaKG/src/models/modeling_bert.py
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    36589 2023-04-18 07:05:24.000000 DeltaKG-0.0.2/DeltaKG/src/models/models.py
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     8635 2023-04-18 07:05:24.000000 DeltaKG-0.0.2/DeltaKG/src/models/optimization.py
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)   170056 2023-04-18 07:05:24.000000 DeltaKG-0.0.2/DeltaKG/src/models/trainer.py
-drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 05:56:32.279145 DeltaKG-0.0.2/DeltaKG.egg-info/
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)      488 2023-04-30 05:56:32.000000 DeltaKG-0.0.2/DeltaKG.egg-info/PKG-INFO
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)      450 2023-04-30 05:56:32.000000 DeltaKG-0.0.2/DeltaKG.egg-info/SOURCES.txt
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)        1 2023-04-30 05:56:32.000000 DeltaKG-0.0.2/DeltaKG.egg-info/dependency_links.txt
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)        8 2023-04-30 05:56:32.000000 DeltaKG-0.0.2/DeltaKG.egg-info/top_level.txt
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     1076 2023-04-18 07:08:58.000000 DeltaKG-0.0.2/LICENSE.txt
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)      488 2023-04-30 05:56:32.283145 DeltaKG-0.0.2/PKG-INFO
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     8835 2023-04-30 05:53:09.000000 DeltaKG-0.0.2/README.md
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)       38 2023-04-30 05:56:32.283145 DeltaKG-0.0.2/setup.cfg
--rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     1091 2023-04-30 05:54:20.000000 DeltaKG-0.0.2/setup.py
+drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 06:03:28.934781 DeltaKG-0.0.3/
+drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 06:03:28.930781 DeltaKG-0.0.3/DeltaKG/
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-29 09:47:59.000000 DeltaKG-0.0.3/DeltaKG/__init__.py
+drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 06:03:28.934781 DeltaKG-0.0.3/DeltaKG/src/
+-rwxr-xr-x   0 tbozhong  (1025) tbozhong  (1025)       41 2023-04-18 07:05:24.000000 DeltaKG-0.0.3/DeltaKG/src/__init__.py
+drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 06:03:28.934781 DeltaKG-0.0.3/DeltaKG/src/data/
+-rwxr-xr-x   0 tbozhong  (1025) tbozhong  (1025)       79 2023-04-18 07:05:24.000000 DeltaKG-0.0.3/DeltaKG/src/data/__init__.py
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    15070 2023-04-18 07:05:24.000000 DeltaKG-0.0.3/DeltaKG/src/data/data_module.py
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    26588 2023-04-18 07:05:24.000000 DeltaKG-0.0.3/DeltaKG/src/data/processor.py
+drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 06:03:28.934781 DeltaKG-0.0.3/DeltaKG/src/models/
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)       73 2023-04-18 07:05:24.000000 DeltaKG-0.0.3/DeltaKG/src/models/__init__.py
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    71121 2023-04-18 07:05:24.000000 DeltaKG-0.0.3/DeltaKG/src/models/modeling_bert.py
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)    36589 2023-04-18 07:05:24.000000 DeltaKG-0.0.3/DeltaKG/src/models/models.py
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     8635 2023-04-18 07:05:24.000000 DeltaKG-0.0.3/DeltaKG/src/models/optimization.py
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)   170056 2023-04-18 07:05:24.000000 DeltaKG-0.0.3/DeltaKG/src/models/trainer.py
+drwxrwxr-x   0 tbozhong  (1025) tbozhong  (1025)        0 2023-04-30 06:03:28.934781 DeltaKG-0.0.3/DeltaKG.egg-info/
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)      488 2023-04-30 06:03:28.000000 DeltaKG-0.0.3/DeltaKG.egg-info/PKG-INFO
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)      450 2023-04-30 06:03:28.000000 DeltaKG-0.0.3/DeltaKG.egg-info/SOURCES.txt
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)        1 2023-04-30 06:03:28.000000 DeltaKG-0.0.3/DeltaKG.egg-info/dependency_links.txt
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)        8 2023-04-30 06:03:28.000000 DeltaKG-0.0.3/DeltaKG.egg-info/top_level.txt
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     1076 2023-04-18 07:08:58.000000 DeltaKG-0.0.3/LICENSE.txt
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)      488 2023-04-30 06:03:28.934781 DeltaKG-0.0.3/PKG-INFO
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     8829 2023-04-30 06:02:31.000000 DeltaKG-0.0.3/README.md
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)       38 2023-04-30 06:03:28.934781 DeltaKG-0.0.3/setup.cfg
+-rw-rw-r--   0 tbozhong  (1025) tbozhong  (1025)     1091 2023-04-30 06:02:43.000000 DeltaKG-0.0.3/setup.py
```

### Comparing `DeltaKG-0.0.2/DeltaKG/src/data/data_module.py` & `DeltaKG-0.0.3/DeltaKG/src/data/data_module.py`

 * *Files identical despite different names*

### Comparing `DeltaKG-0.0.2/DeltaKG/src/data/processor.py` & `DeltaKG-0.0.3/DeltaKG/src/data/processor.py`

 * *Files identical despite different names*

### Comparing `DeltaKG-0.0.2/DeltaKG/src/models/modeling_bert.py` & `DeltaKG-0.0.3/DeltaKG/src/models/modeling_bert.py`

 * *Files identical despite different names*

### Comparing `DeltaKG-0.0.2/DeltaKG/src/models/models.py` & `DeltaKG-0.0.3/DeltaKG/src/models/models.py`

 * *Files identical despite different names*

### Comparing `DeltaKG-0.0.2/DeltaKG/src/models/optimization.py` & `DeltaKG-0.0.3/DeltaKG/src/models/optimization.py`

 * *Files identical despite different names*

### Comparing `DeltaKG-0.0.2/DeltaKG/src/models/trainer.py` & `DeltaKG-0.0.3/DeltaKG/src/models/trainer.py`

 * *Files identical despite different names*

### Comparing `DeltaKG-0.0.2/LICENSE.txt` & `DeltaKG-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DeltaKG-0.0.2/README.md` & `DeltaKG-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-<div align="center">
-    <img src="https://github.com/zjunlp/PromptKG/blob/main/resources/deltakg_logo.png" width="550px">
-    <p> <b>
-        A Library for Dynamically Editing PLMs-Based Knowledge Graph Embeddings.</b>
-    </p>
+<p align="center">
+<img src="https://github.com/zjunlp/PromptKG/blob/main/resources/deltakg_logo.png" width="550px">
+</p>
+<p align="center"> <b>
+    A Library for Dynamically Editing PLMs-Based Knowledge Graph Embeddings.</b>
+</p>
     
 ------
 
 <p align="center">
   <a href="#overview">Overview</a> •
   <a href="#installation">Installation</a> •
   <a href="#how-to-run">How To Run</a> •
   <a href="https://arxiv.org/pdf/2301.10405">Paper</a> •
   <a href="https://medium.com/@jack16900/deltakg-a-library-for-dynamically-editing-plm-based-kg-embeddings-243d59a8f168">Medium</a> •
   <a href="#how-to-cite">Citation</a> •
   <a href="#other-kg-representation-open-source-projects">Others</a> 
 </p>
-</div>
+
 
 ## Overview
 Knowledge graph embedding (KGE) is a method for representing symbolic facts in low-dimensional vector spaces, with the goal of projecting relations and entities into a continuous vector space. This approach enhances knowledge reasoning capabilities and facilitates application to downstream tasks.
 
 We introduce DeltaKG (MIT License), a dynamic, PLM-based library for KGEs that equips with numerous baseline models, such as K-Adapter, CaliNet, KnowledgeEditor, MEND, and KGEditor, and supports a variety of datasets, including E-FB15k237, A-FB15k237, E-WN18RR, and A-WN18RR.
 
 **DeltaKG** is now publicly open-sourced, with [a demo](https://huggingface.co/spaces/zjunlp/KGEditor), [a leaderboard](https://zjunlp.github.io/project/KGE_Editing/) and long-term maintenance.
 <!-- - ❗NOTE: We provide some KGE baselines at [OpenBG-IMG](https://github.com/OpenBGBenchmark/OpenBG-IMG). -->
 
 ## Model Architecture
 
-<div align=center>
+<p align="center">
 <img src="resource/model.png" width="75%" height="75%" />
-</div>
+</p>
 
  Illustration of KGEditor for a) The external model-based editor, b) The additional parameter-based editor and c) KGEditor.
 
 ## Installation
 
 **Step1** Download the basic code
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
    [https://github.com/zjunlp/PromptKG/blob/main/resources/deltakg_logo.png]
    A Library for Dynamically Editing PLMs-Based Knowledge Graph Embeddings.
-                                    ------
+------
 Overview â¢ Installation â¢ How_To_Run â¢ Paper â¢ Medium â¢ Citation â¢
                                     Others
 ## Overview Knowledge graph embedding (KGE) is a method for representing
 symbolic facts in low-dimensional vector spaces, with the goal of projecting
 relations and entities into a continuous vector space. This approach enhances
 knowledge reasoning capabilities and facilitates application to downstream
 tasks. We introduce DeltaKG (MIT License), a dynamic, PLM-based library for
```

### Comparing `DeltaKG-0.0.2/setup.py` & `DeltaKG-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     import pypandoc
     long_description = pypandoc.convert('README.md', 'rst')
 except:
     long_description = ""
 
 setuptools.setup(
     name='DeltaKG',
-    version='0.0.2',
+    version='0.0.3',
     description='A Library for Dynamically Editing PLMs-Based Knowledge Graph Embeddings.',
     author='Bozhong Tian',
     author_email='tbozhong@zju.edu.cn',
     url='https://github.com/zjunlp/PromptKG/tree/main/deltaKG',
     install_requires=[],
     # install_requires=['dataclasses==0.8', 'transformers==4.26.1', 'activations==0.1.0', 'flax==0.3.4',
     #                   'utils==1.0.1', 'pytorch_lightning==1.3.1', 'jsonlines', 'higher', 'allennlp', 'file_utils==0.0.1'],
```

