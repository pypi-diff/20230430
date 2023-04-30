# Comparing `tmp/tflite_runtime_nightly-2.13.0.dev20230427-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/tflite_runtime_nightly-2.13.0.dev20230428-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 2385864 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       80 b- defN 23-Apr-28 04:56 tflite_runtime/__init__.py
--rwxrwxr-x  2.0 unx  6781128 b- defN 23-Apr-28 04:58 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
--rw-rw-r--  2.0 unx    38775 b- defN 23-Apr-28 04:55 tflite_runtime/interpreter.py
--rw-rw-r--  2.0 unx     1542 b- defN 23-Apr-28 04:55 tflite_runtime/metrics_interface.py
--rw-rw-r--  2.0 unx     2048 b- defN 23-Apr-28 04:55 tflite_runtime/metrics_portable.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-Apr-28 04:58 tflite_runtime_nightly-2.13.0.dev20230427.dist-info/METADATA
--rw-rw-r--  2.0 unx      111 b- defN 23-Apr-28 04:58 tflite_runtime_nightly-2.13.0.dev20230427.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-28 04:58 tflite_runtime_nightly-2.13.0.dev20230427.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      878 b- defN 23-Apr-28 04:58 tflite_runtime_nightly-2.13.0.dev20230427.dist-info/RECORD
-9 files, 6826017 bytes uncompressed, 2384318 bytes compressed:  65.1%
+Zip file size: 2385861 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       80 b- defN 23-Apr-29 04:52 tflite_runtime/__init__.py
+-rwxrwxr-x  2.0 unx  6781128 b- defN 23-Apr-29 04:54 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
+-rw-rw-r--  2.0 unx    38775 b- defN 23-Apr-29 04:52 tflite_runtime/interpreter.py
+-rw-rw-r--  2.0 unx     1542 b- defN 23-Apr-29 04:52 tflite_runtime/metrics_interface.py
+-rw-rw-r--  2.0 unx     2048 b- defN 23-Apr-29 04:52 tflite_runtime/metrics_portable.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Apr-29 04:54 tflite_runtime_nightly-2.13.0.dev20230428.dist-info/METADATA
+-rw-rw-r--  2.0 unx      111 b- defN 23-Apr-29 04:54 tflite_runtime_nightly-2.13.0.dev20230428.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-29 04:54 tflite_runtime_nightly-2.13.0.dev20230428.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 23-Apr-29 04:54 tflite_runtime_nightly-2.13.0.dev20230428.dist-info/RECORD
+9 files, 6826017 bytes uncompressed, 2384315 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tflite_runtime/metrics_interface.py
 Comment: 
 
 Filename: tflite_runtime/metrics_portable.py
 Comment: 
 
-Filename: tflite_runtime_nightly-2.13.0.dev20230427.dist-info/METADATA
+Filename: tflite_runtime_nightly-2.13.0.dev20230428.dist-info/METADATA
 Comment: 
 
-Filename: tflite_runtime_nightly-2.13.0.dev20230427.dist-info/WHEEL
+Filename: tflite_runtime_nightly-2.13.0.dev20230428.dist-info/WHEEL
 Comment: 
 
-Filename: tflite_runtime_nightly-2.13.0.dev20230427.dist-info/top_level.txt
+Filename: tflite_runtime_nightly-2.13.0.dev20230428.dist-info/top_level.txt
 Comment: 
 
-Filename: tflite_runtime_nightly-2.13.0.dev20230427.dist-info/RECORD
+Filename: tflite_runtime_nightly-2.13.0.dev20230428.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tflite_runtime/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '2.13.0dev20230427'
-__git_version__ = '0.6.0-147137-g24558c4400c'
+__version__ = '2.13.0dev20230428'
+__git_version__ = '0.6.0-147191-g426c4e9ef22'
```

## Comparing `tflite_runtime_nightly-2.13.0.dev20230427.dist-info/METADATA` & `tflite_runtime_nightly-2.13.0.dev20230428.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tflite-runtime-nightly
-Version: 2.13.0.dev20230427
+Version: 2.13.0.dev20230428
 Summary: TensorFlow Lite is for mobile and embedded devices.
 Home-page: https://www.tensorflow.org/lite/
 Author: Google, LLC
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Keywords: tflite tensorflow tensor machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

