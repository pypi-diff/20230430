# Comparing `tmp/polars-streaming-0.1.2.tar.gz` & `tmp/polars-streaming-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/alchemist/Desktop/OpenSource/polars-streaming/dist/.tmp-5d56fhz7/polars-streaming-0.1.2.tar", last modified: Thu Apr 27 13:27:18 2023, max compression
+gzip compressed data, was "/home/alchemist/Desktop/OpenSource/polars-streaming/dist/.tmp-_lveyz49/polars-streaming-0.2.0.tar", last modified: Sun Apr 30 14:08:08 2023, max compression
```

## Comparing `polars-streaming-0.1.2.tar` & `polars-streaming-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 13:27:18.000000 polars-streaming-0.1.2/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    11357 2023-04-19 18:26:51.000000 polars-streaming-0.1.2/LICENSE
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    13953 2023-04-27 13:27:18.000000 polars-streaming-0.1.2/PKG-INFO
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      406 2023-04-26 18:01:15.000000 polars-streaming-0.1.2/README.md
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 13:27:18.000000 polars-streaming-0.1.2/polars_streaming/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      200 2023-04-27 13:27:02.000000 polars-streaming-0.1.2/polars_streaming/__init__.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1039 2023-04-27 13:18:39.000000 polars-streaming-0.1.2/polars_streaming/core.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      436 2023-04-26 17:25:44.000000 polars-streaming-0.1.2/polars_streaming/exceptions.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     2137 2023-04-27 13:21:11.000000 polars-streaming-0.1.2/polars_streaming/fileProcessor.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     2822 2023-04-27 13:20:48.000000 polars-streaming-0.1.2/polars_streaming/kafkaProcessor.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1715 2023-04-26 13:32:40.000000 polars-streaming-0.1.2/polars_streaming/readwriter.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      918 2023-04-27 13:20:59.000000 polars-streaming-0.1.2/polars_streaming/utils.py
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 13:27:18.000000 polars-streaming-0.1.2/polars_streaming.egg-info/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    13953 2023-04-27 13:27:18.000000 polars-streaming-0.1.2/polars_streaming.egg-info/PKG-INFO
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      442 2023-04-27 13:27:18.000000 polars-streaming-0.1.2/polars_streaming.egg-info/SOURCES.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        1 2023-04-27 13:27:18.000000 polars-streaming-0.1.2/polars_streaming.egg-info/dependency_links.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      128 2023-04-27 13:27:18.000000 polars-streaming-0.1.2/polars_streaming.egg-info/requires.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       17 2023-04-27 13:27:18.000000 polars-streaming-0.1.2/polars_streaming.egg-info/top_level.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1228 2023-04-27 13:27:02.000000 polars-streaming-0.1.2/pyproject.toml
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       38 2023-04-27 13:27:18.000000 polars-streaming-0.1.2/setup.cfg
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    11357 2023-04-19 18:26:51.000000 polars-streaming-0.2.0/LICENSE
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    14448 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/PKG-INFO
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      901 2023-04-30 14:07:46.000000 polars-streaming-0.2.0/README.md
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/polars_streaming/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      210 2023-04-30 13:56:54.000000 polars-streaming-0.2.0/polars_streaming/__init__.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1240 2023-04-30 12:55:14.000000 polars-streaming-0.2.0/polars_streaming/core.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      436 2023-04-26 17:25:44.000000 polars-streaming-0.2.0/polars_streaming/exceptions.py
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/polars_streaming/processors/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        0 2023-04-30 12:45:56.000000 polars-streaming-0.2.0/polars_streaming/processors/__init__.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     2138 2023-04-30 12:41:43.000000 polars-streaming-0.2.0/polars_streaming/processors/fileProcessor.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     2823 2023-04-30 12:41:36.000000 polars-streaming-0.2.0/polars_streaming/processors/kafkaProcessor.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1790 2023-04-30 13:55:05.000000 polars-streaming-0.2.0/polars_streaming/processors/socketProcessor.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      919 2023-04-30 12:41:23.000000 polars-streaming-0.2.0/polars_streaming/processors/utils.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1715 2023-04-26 13:32:40.000000 polars-streaming-0.2.0/polars_streaming/readwriter.py
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/polars_streaming/sinks/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        0 2023-04-30 11:14:10.000000 polars-streaming-0.2.0/polars_streaming/sinks/__init__.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1015 2023-04-29 07:01:54.000000 polars-streaming-0.2.0/polars_streaming/sinks/esWriter.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      586 2023-04-29 06:50:31.000000 polars-streaming-0.2.0/polars_streaming/sinks/mongoWriter.py
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/polars_streaming.egg-info/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    14448 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/polars_streaming.egg-info/PKG-INFO
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      670 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/polars_streaming.egg-info/SOURCES.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        1 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/polars_streaming.egg-info/dependency_links.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      128 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/polars_streaming.egg-info/requires.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       17 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/polars_streaming.egg-info/top_level.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1228 2023-04-30 13:56:54.000000 polars-streaming-0.2.0/pyproject.toml
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       38 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/setup.cfg
```

### Comparing `polars-streaming-0.1.2/LICENSE` & `polars-streaming-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polars-streaming-0.1.2/PKG-INFO` & `polars-streaming-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars-streaming
-Version: 0.1.2
+Version: 0.2.0
 Summary: Stream Processing Library using Polars
 Author-email: Vinish M <vinishuchiha@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -231,7 +231,25 @@
 **Install from sources**
 
 Alternatively, you can also clone the latest version from the [repository](https://github.com/VinishUchiha/polars-streaming) and install it directly from the source code:
 
 ```bash
 pip install -e .
 ```
+
+## Quick tour
+```python
+>>> from polars_streaming import StreamProcessor
+
+>>> s = StreamProcessor()
+>>> s.readStream.format('socket').options({'host':'localhost','port':12345}).load()
+
+>>> def transformation(df):
+>>>     # Add your transformation code here
+>>>     df = df.sum() # For example purpose, I am calculating the sum.
+>>>     return df # Return the transformed dataframe
+
+>>> s.add_transform(transformation)
+>>> s.writeStream.format('console').trigger('3 seconds')
+
+>>> s.start()
+```
```

### Comparing `polars-streaming-0.1.2/polars_streaming/fileProcessor.py` & `polars-streaming-0.2.0/polars_streaming/processors/fileProcessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from watchdog.events import PatternMatchingEventHandler
 from watchdog.observers import Observer
-from .exceptions import FileSourcePathMissingException, FileExtensionNotSupportedException
+from ..exceptions import FileSourcePathMissingException, FileExtensionNotSupportedException
 import polars as pl
 import time
 from pathlib import Path
 from .utils import _writer, READERS, SUPPORTED_FILE_WRITERS
 
 class FileHandler(PatternMatchingEventHandler):
     def __init__(self, reader, transform, writer) -> None:
```

### Comparing `polars-streaming-0.1.2/polars_streaming/kafkaProcessor.py` & `polars-streaming-0.2.0/polars_streaming/processors/kafkaProcessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import polars as pl
 import schedule
 from .utils import _writer, SUPPORTED_FILE_WRITERS, trigger_time_extracter
-from .exceptions import ModuleNotFoundException
+from ..exceptions import ModuleNotFoundException
 
 options_mapper = {'kafka.bootstrap.servers':'bootstrap.servers',
                 #'subscribe': 'subscribe',
                 #'includeHeaders': 'includeHeaders',
                 'startingOffsets': 'auto.offset.reset',
                 #'endingOffsets': 'endingOffsets',
                 #'subscribePattern': 'subscribePattern',
```

### Comparing `polars-streaming-0.1.2/polars_streaming/readwriter.py` & `polars-streaming-0.2.0/polars_streaming/readwriter.py`

 * *Files identical despite different names*

### Comparing `polars-streaming-0.1.2/polars_streaming/utils.py` & `polars-streaming-0.2.0/polars_streaming/processors/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .exceptions import FileExtensionNotSupportedException
+from ..exceptions import FileExtensionNotSupportedException
 import polars as pl
 
 READERS = {'csv': pl.read_csv, 'parquet': pl.read_parquet, 'json': pl.read_json, 'avro': pl.read_avro}
 SUPPORTED_FILE_WRITERS = ['csv','parquet','json','avro']
 
 def _writer(df, path, extension):
     if extension == 'csv':
```

### Comparing `polars-streaming-0.1.2/polars_streaming.egg-info/PKG-INFO` & `polars-streaming-0.2.0/polars_streaming.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars-streaming
-Version: 0.1.2
+Version: 0.2.0
 Summary: Stream Processing Library using Polars
 Author-email: Vinish M <vinishuchiha@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -231,7 +231,25 @@
 **Install from sources**
 
 Alternatively, you can also clone the latest version from the [repository](https://github.com/VinishUchiha/polars-streaming) and install it directly from the source code:
 
 ```bash
 pip install -e .
 ```
+
+## Quick tour
+```python
+>>> from polars_streaming import StreamProcessor
+
+>>> s = StreamProcessor()
+>>> s.readStream.format('socket').options({'host':'localhost','port':12345}).load()
+
+>>> def transformation(df):
+>>>     # Add your transformation code here
+>>>     df = df.sum() # For example purpose, I am calculating the sum.
+>>>     return df # Return the transformed dataframe
+
+>>> s.add_transform(transformation)
+>>> s.writeStream.format('console').trigger('3 seconds')
+
+>>> s.start()
+```
```

### Comparing `polars-streaming-0.1.2/pyproject.toml` & `polars-streaming-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "polars-streaming"
-version = "0.1.2"
+version = "0.2.0"
 description = "Stream Processing Library using Polars"
 readme = "README.md"
 authors = [{ name = "Vinish M", email = "vinishuchiha@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
@@ -27,15 +27,15 @@
 kafka = ["confluent-kafka"]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/VinishUchiha/polars-streaming"
 
 [tool.bumpver]
-current_version = "0.1.2"
+current_version = "0.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

