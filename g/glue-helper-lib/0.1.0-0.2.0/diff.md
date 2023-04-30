# Comparing `tmp/glue_helper_lib-0.1.0.tar.gz` & `tmp/glue_helper_lib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_helper_lib-0.1.0.tar", max compression
+gzip compressed data, was "glue_helper_lib-0.2.0.tar", max compression
```

## Comparing `glue_helper_lib-0.1.0.tar` & `glue_helper_lib-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-03-25 11:21:46.068544 glue_helper_lib-0.1.0/LICENSE
--rw-r--r--   0        0        0       61 2023-04-09 13:34:10.902381 glue_helper_lib-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-03-25 11:33:42.478539 glue_helper_lib-0.1.0/glue_helper_lib/__init__.py
--rw-r--r--   0        0        0     1714 2023-04-09 13:08:52.592360 glue_helper_lib-0.1.0/glue_helper_lib/arguments.py
--rw-r--r--   0        0        0     1156 2023-04-09 13:09:10.252360 glue_helper_lib-0.1.0/glue_helper_lib/logging.py
--rw-r--r--   0        0        0      711 2023-04-09 13:36:22.212382 glue_helper_lib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 glue_helper_lib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-25 11:21:46.068544 glue_helper_lib-0.2.0/LICENSE
+-rw-r--r--   0        0        0       61 2023-04-09 13:42:48.332388 glue_helper_lib-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-25 11:33:42.478539 glue_helper_lib-0.2.0/glue_helper_lib/__init__.py
+-rw-r--r--   0        0        0     1714 2023-04-09 13:08:52.592360 glue_helper_lib-0.2.0/glue_helper_lib/arguments.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:40:12.399875 glue_helper_lib-0.2.0/glue_helper_lib/hudi/__init__.py
+-rw-r--r--   0        0        0     8811 2023-04-30 14:55:32.831653 glue_helper_lib-0.2.0/glue_helper_lib/hudi/config.py
+-rw-r--r--   0        0        0     1074 2023-04-29 15:41:29.309874 glue_helper_lib-0.2.0/glue_helper_lib/hudi/session.py
+-rw-r--r--   0        0        0     1899 2023-04-30 14:55:09.631653 glue_helper_lib-0.2.0/glue_helper_lib/hudi/table.py
+-rw-r--r--   0        0        0     1163 2023-04-09 13:56:20.652399 glue_helper_lib-0.2.0/glue_helper_lib/logging.py
+-rw-r--r--   0        0        0      741 2023-04-30 08:05:37.205594 glue_helper_lib-0.2.0/glue_helper_lib/table.py
+-rw-r--r--   0        0        0      711 2023-04-30 14:56:20.031652 glue_helper_lib-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 glue_helper_lib-0.2.0/PKG-INFO
```

### Comparing `glue_helper_lib-0.1.0/LICENSE` & `glue_helper_lib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.1.0/glue_helper_lib/arguments.py` & `glue_helper_lib-0.2.0/glue_helper_lib/arguments.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.1.0/glue_helper_lib/logging.py` & `glue_helper_lib-0.2.0/glue_helper_lib/logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             <time - name - [level] - message>
     """
 
     def __init__(
         self,
         name: str,
         level: LogLevel,
-        formatter: typing.Optional[logging.Formatter],
+        formatter: typing.Optional[logging.Formatter] = None,
     ) -> None:
         super().__init__(name, level.value)
         self._configure(formatter)
 
     def _configure(self, formatter: typing.Optional[logging.Formatter]):
         handler = logging.StreamHandler(sys.stdout)
         if not formatter:
```

### Comparing `glue_helper_lib-0.1.0/pyproject.toml` & `glue_helper_lib-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glue-helper-lib"
-version = "0.1.0"
+version = "0.2.0"
 description = "A library containing multiple helper and utility functionalities for AWS Glue"
 authors = ["Martijn Sturm <martijn.sturm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "glue_helper_lib" }]
 
 [tool.poetry.dependencies]
```

### Comparing `glue_helper_lib-0.1.0/PKG-INFO` & `glue_helper_lib-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-helper-lib
-Version: 0.1.0
+Version: 0.2.0
 Summary: A library containing multiple helper and utility functionalities for AWS Glue
 License: MIT
 Author: Martijn Sturm
 Author-email: martijn.sturm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

