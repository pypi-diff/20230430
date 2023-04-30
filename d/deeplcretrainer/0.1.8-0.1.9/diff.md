# Comparing `tmp/deeplcretrainer-0.1.8.tar.gz` & `tmp/deeplcretrainer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplcretrainer-0.1.8.tar", last modified: Sat Feb  4 10:00:13 2023, max compression
+gzip compressed data, was "deeplcretrainer-0.1.9.tar", last modified: Sat Feb  4 10:09:56 2023, max compression
```

## Comparing `deeplcretrainer-0.1.8.tar` & `deeplcretrainer-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1928 2022-11-01 11:50:52.599911 deeplcretrainer-0.1.8/.gitignore
--rw-r--r--   0        0        0    11558 2022-11-01 11:50:52.599911 deeplcretrainer-0.1.8/LICENSE
--rw-r--r--   0        0        0       17 2022-11-01 11:50:52.599911 deeplcretrainer-0.1.8/README.md
--rw-r--r--   0        0        0       46 2023-02-04 09:59:32.692046 deeplcretrainer-0.1.8/deeplcretrainer/__init__.py
--rw-r--r--   0        0        0    35431 2022-10-09 11:22:15.564382 deeplcretrainer-0.1.8/deeplcretrainer/cnn_functions.py
--rw-r--r--   0        0        0    13944 2023-02-04 09:59:27.447549 deeplcretrainer-0.1.8/deeplcretrainer/deeplcretrainer.py
--rw-r--r--   0        0        0      581 2022-12-07 14:04:28.618661 deeplcretrainer-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 deeplcretrainer-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1928 2022-11-01 11:50:52.599911 deeplcretrainer-0.1.9/.gitignore
+-rw-r--r--   0        0        0    11558 2022-11-01 11:50:52.599911 deeplcretrainer-0.1.9/LICENSE
+-rw-r--r--   0        0        0       17 2022-11-01 11:50:52.599911 deeplcretrainer-0.1.9/README.md
+-rw-r--r--   0        0        0       46 2023-02-04 10:09:29.347116 deeplcretrainer-0.1.9/deeplcretrainer/__init__.py
+-rw-r--r--   0        0        0    35431 2022-10-09 11:22:15.564382 deeplcretrainer-0.1.9/deeplcretrainer/cnn_functions.py
+-rw-r--r--   0        0        0    14082 2023-02-04 10:09:03.490447 deeplcretrainer-0.1.9/deeplcretrainer/deeplcretrainer.py
+-rw-r--r--   0        0        0      581 2022-12-07 14:04:28.618661 deeplcretrainer-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 deeplcretrainer-0.1.9/PKG-INFO
```

### Comparing `deeplcretrainer-0.1.8/.gitignore` & `deeplcretrainer-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `deeplcretrainer-0.1.8/LICENSE` & `deeplcretrainer-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplcretrainer-0.1.8/deeplcretrainer/cnn_functions.py` & `deeplcretrainer-0.1.9/deeplcretrainer/cnn_functions.py`

 * *Files identical despite different names*

### Comparing `deeplcretrainer-0.1.8/deeplcretrainer/deeplcretrainer.py` & `deeplcretrainer-0.1.9/deeplcretrainer/deeplcretrainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,20 @@
 from tensorflow.keras.layers import ReLU
 import importlib
 
 try:
     from gooey import Gooey, local_resource_path
     from gooey import GooeyParser
 except ImportError:
-    pass
+    def Gooey(
+        program_name="DeepLC re-tR-ainer",
+        default_size=(720, 790),
+        monospace_display=True
+    ):
+        pass
 
 try:
     from deeplcretrainer import cnn_functions
 except ImportError:
     import cnn_functions
 
 import itertools
```

### Comparing `deeplcretrainer-0.1.8/pyproject.toml` & `deeplcretrainer-0.1.9/pyproject.toml`

 * *Files identical despite different names*

