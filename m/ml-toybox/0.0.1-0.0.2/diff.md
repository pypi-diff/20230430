# Comparing `tmp/ml-toybox-0.0.1.tar.gz` & `tmp/ml-toybox-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ml-toybox-0.0.1.tar", last modified: Sat Sep 26 00:12:16 2020, max compression
+gzip compressed data, was "ml-toybox-0.0.2.tar", last modified: Sun Apr 30 05:56:41 2023, max compression
```

## Comparing `ml-toybox-0.0.1.tar` & `ml-toybox-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2020-09-26 00:12:16.742644 ml-toybox-0.0.1/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      821 2020-09-26 00:12:16.742644 ml-toybox-0.0.1/PKG-INFO
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      181 2020-09-26 00:09:29.000000 ml-toybox-0.0.1/README.rst
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2020-09-26 00:12:16.742644 ml-toybox-0.0.1/ml_toybox.egg-info/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      821 2020-09-26 00:12:16.000000 ml-toybox-0.0.1/ml_toybox.egg-info/PKG-INFO
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      239 2020-09-26 00:12:16.000000 ml-toybox-0.0.1/ml_toybox.egg-info/SOURCES.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        1 2020-09-26 00:12:16.000000 ml-toybox-0.0.1/ml_toybox.egg-info/dependency_links.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       10 2020-09-26 00:12:16.000000 ml-toybox-0.0.1/ml_toybox.egg-info/top_level.txt
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2020-09-26 00:12:16.742644 ml-toybox-0.0.1/mltoolbox/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2020-09-26 00:08:19.000000 ml-toybox-0.0.1/mltoolbox/__init__.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     4997 2020-09-26 00:08:19.000000 ml-toybox-0.0.1/mltoolbox/perceptron_classifier.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     6318 2020-09-26 00:08:19.000000 ml-toybox-0.0.1/mltoolbox/pocket_classifier.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       38 2020-09-26 00:12:16.742644 ml-toybox-0.0.1/setup.cfg
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1003 2020-09-26 00:10:16.000000 ml-toybox-0.0.1/setup.py
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 05:56:41.081318 ml-toybox-0.0.2/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1067 2023-04-22 22:39:09.000000 ml-toybox-0.0.2/LICENSE
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      781 2023-04-30 05:56:41.081318 ml-toybox-0.0.2/PKG-INFO
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      181 2023-04-22 22:39:09.000000 ml-toybox-0.0.2/README.rst
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 05:56:41.081318 ml-toybox-0.0.2/ml_toybox.egg-info/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      781 2023-04-30 05:56:41.000000 ml-toybox-0.0.2/ml_toybox.egg-info/PKG-INFO
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      289 2023-04-30 05:56:41.000000 ml-toybox-0.0.2/ml_toybox.egg-info/SOURCES.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        1 2023-04-30 05:56:41.000000 ml-toybox-0.0.2/ml_toybox.egg-info/dependency_links.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       57 2023-04-30 05:56:41.000000 ml-toybox-0.0.2/ml_toybox.egg-info/entry_points.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       15 2023-04-30 05:56:41.000000 ml-toybox-0.0.2/ml_toybox.egg-info/top_level.txt
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 05:56:41.081318 ml-toybox-0.0.2/mltoolbox/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-22 22:39:09.000000 ml-toybox-0.0.2/mltoolbox/__init__.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     4998 2023-04-22 22:41:23.000000 ml-toybox-0.0.2/mltoolbox/perceptron_classifier.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     6319 2023-04-22 22:54:07.000000 ml-toybox-0.0.2/mltoolbox/pocket_classifier.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      802 2023-04-30 05:53:45.000000 ml-toybox-0.0.2/pyproject.toml
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       38 2023-04-30 05:56:41.081318 ml-toybox-0.0.2/setup.cfg
```

### Comparing `ml-toybox-0.0.1/PKG-INFO` & `ml-toybox-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: ml-toybox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Machine Learning ToyBox
-Home-page: https://github.com/shunsvineyard/ml-toybox
-Author: Shun Huang
-Author-email: shunsvineyard@protonmail.com
-License: MIT
-Description: ########################
-        Machine Learning ToyBox
-        ########################
-        
-        Machine Learning ToyBox consists of many machine learning algorithm implementation for learning and fun. 
-        
+Author-email: Shun Huang <shun@formosa1544.com>
+License: MIT License
+Project-URL: repository, https://github.com/burpeesDaily/ml-toybox
 Keywords: Machine Learning
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+########################
+Machine Learning ToyBox
+########################
+
+Machine Learning ToyBox consists of many machine learning algorithm implementation for learning and fun.
```

### Comparing `ml-toybox-0.0.1/ml_toybox.egg-info/PKG-INFO` & `ml-toybox-0.0.2/ml_toybox.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: ml-toybox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Machine Learning ToyBox
-Home-page: https://github.com/shunsvineyard/ml-toybox
-Author: Shun Huang
-Author-email: shunsvineyard@protonmail.com
-License: MIT
-Description: ########################
-        Machine Learning ToyBox
-        ########################
-        
-        Machine Learning ToyBox consists of many machine learning algorithm implementation for learning and fun. 
-        
+Author-email: Shun Huang <shun@formosa1544.com>
+License: MIT License
+Project-URL: repository, https://github.com/burpeesDaily/ml-toybox
 Keywords: Machine Learning
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+########################
+Machine Learning ToyBox
+########################
+
+Machine Learning ToyBox consists of many machine learning algorithm implementation for learning and fun.
```

### Comparing `ml-toybox-0.0.1/mltoolbox/perceptron_classifier.py` & `ml-toybox-0.0.2/mltoolbox/perceptron_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     train(samples: [[]], labels: [], max_iterator: int = 10)
         Train the perceptron learning algorithm with samples.
     classify(new_data: [[]]) -> []
         Classify the input data.
     See Also
     --------
     See details at:
-    https://shunsvineyard.info/2017/10/22/machine-learning-basics-and-perceptron-learning-algorithm/
+    https://www.formosa1544.com/2017/10/22/machine-learning-basics-and-perceptron-learning-algorithm/
     Examples
     --------
     Two dimensions list and each sample has four attributes
     >>> import perceptron_classifier
     >>> samples = [[5.1, 3.5, 1.4, 0.2],
                    [4.9, 3.0, 1.4, 0.2],
                    [4.7, 3.2, 1.3, 0.2],
```

### Comparing `ml-toybox-0.0.1/mltoolbox/pocket_classifier.py` & `ml-toybox-0.0.2/mltoolbox/pocket_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     train(samples: [[]], labels: [], max_iterator: int = 10)
         Train the perceptron learning algorithm with samples.
     classify(new_data: [[]]) -> []
         Classify the input data.
     See Also
     --------
     See details at:
-    https://shunsvineyard.info/2018/02/11/machine-learning-basics-pocket-learning-algorithm-and-basic-feature-engineering/
+    https://www.formosa1544.com/2018/02/11/machine-learning-basics-pocket-learning-algorithm-and-basic-feature-engineering/
     Examples
     --------
     Two dimensions list and each sample has four attributes
     >>> import pocket_classifier
     >>> samples = [[5.1, 3.5, 1.4, 0.2],
                    [4.9, 3.0, 1.4, 0.2],
                    [4.7, 3.2, 1.3, 0.2],
```

