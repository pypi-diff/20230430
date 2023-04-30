# Comparing `tmp/java_bytecode_disassembler-1.0.2.tar.gz` & `tmp/java_bytecode_disassembler-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "java_bytecode_disassembler-1.0.2.tar", last modified: Sun Apr 30 21:17:10 2023, max compression
+gzip compressed data, was "java_bytecode_disassembler-1.0.3.tar", last modified: Sun Apr 30 21:23:02 2023, max compression
```

## Comparing `java_bytecode_disassembler-1.0.2.tar` & `java_bytecode_disassembler-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 21:17:10.233088 java_bytecode_disassembler-1.0.2/
--rw-rw-rw-   0        0        0    26526 2023-04-27 00:53:09.000000 java_bytecode_disassembler-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      824 2023-04-30 21:17:10.217462 java_bytecode_disassembler-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       98 2023-04-27 00:53:09.000000 java_bytecode_disassembler-1.0.2/README.md
--rw-rw-rw-   0        0        0      783 2023-04-30 21:16:05.000000 java_bytecode_disassembler-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 21:17:10.233088 java_bytecode_disassembler-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-30 21:17:10.154955 java_bytecode_disassembler-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 21:17:10.186207 java_bytecode_disassembler-1.0.2/src/disassembler/
--rw-rw-rw-   0        0        0       52 2023-04-30 21:15:58.000000 java_bytecode_disassembler-1.0.2/src/disassembler/__init__.py
--rw-rw-rw-   0        0        0    95221 2023-04-30 21:00:41.000000 java_bytecode_disassembler-1.0.2/src/disassembler/java_bytecode_disassembler.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:17:10.201833 java_bytecode_disassembler-1.0.2/src/java_bytecode_disassembler.egg-info/
--rw-rw-rw-   0        0        0      824 2023-04-30 21:17:10.000000 java_bytecode_disassembler-1.0.2/src/java_bytecode_disassembler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-04-30 21:17:10.000000 java_bytecode_disassembler-1.0.2/src/java_bytecode_disassembler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 21:17:10.000000 java_bytecode_disassembler-1.0.2/src/java_bytecode_disassembler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-30 21:17:10.000000 java_bytecode_disassembler-1.0.2/src/java_bytecode_disassembler.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-30 21:17:10.217462 java_bytecode_disassembler-1.0.2/tests/
--rw-rw-rw-   0        0        0      218 2023-04-30 21:03:13.000000 java_bytecode_disassembler-1.0.2/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:23:02.414571 java_bytecode_disassembler-1.0.3/
+-rw-rw-rw-   0        0        0    26526 2023-04-27 00:53:09.000000 java_bytecode_disassembler-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      824 2023-04-30 21:23:02.414571 java_bytecode_disassembler-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       98 2023-04-27 00:53:09.000000 java_bytecode_disassembler-1.0.3/README.md
+-rw-rw-rw-   0        0        0      783 2023-04-30 21:22:16.000000 java_bytecode_disassembler-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 21:23:02.414571 java_bytecode_disassembler-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 21:23:02.320751 java_bytecode_disassembler-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 21:23:02.383256 java_bytecode_disassembler-1.0.3/src/java_bytecode_disassembler/
+-rw-rw-rw-   0        0        0       52 2023-04-30 21:15:58.000000 java_bytecode_disassembler-1.0.3/src/java_bytecode_disassembler/__init__.py
+-rw-rw-rw-   0        0        0    95221 2023-04-30 21:00:41.000000 java_bytecode_disassembler-1.0.3/src/java_bytecode_disassembler/java_bytecode_disassembler.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:23:02.414571 java_bytecode_disassembler-1.0.3/src/java_bytecode_disassembler.egg-info/
+-rw-rw-rw-   0        0        0      824 2023-04-30 21:23:02.000000 java_bytecode_disassembler-1.0.3/src/java_bytecode_disassembler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-04-30 21:23:02.000000 java_bytecode_disassembler-1.0.3/src/java_bytecode_disassembler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 21:23:02.000000 java_bytecode_disassembler-1.0.3/src/java_bytecode_disassembler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-30 21:23:02.000000 java_bytecode_disassembler-1.0.3/src/java_bytecode_disassembler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 21:23:02.414571 java_bytecode_disassembler-1.0.3/tests/
+-rw-rw-rw-   0        0        0      218 2023-04-30 21:03:13.000000 java_bytecode_disassembler-1.0.3/tests/test.py
```

### Comparing `java_bytecode_disassembler-1.0.2/LICENSE` & `java_bytecode_disassembler-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `java_bytecode_disassembler-1.0.2/PKG-INFO` & `java_bytecode_disassembler-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: java_bytecode_disassembler
-Version: 1.0.2
+Version: 1.0.3
 Summary: Disassembler for java bytecode
 Author-email: Spartanlasergun <bns360@live.com>
 Project-URL: Homepage, https://github.com/Spartanlasergun/java_bytecode_disassembler
 Project-URL: Bug Tracker, https://github.com/Spartanlasergun/java_bytecode_disassembler/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `java_bytecode_disassembler-1.0.2/pyproject.toml` & `java_bytecode_disassembler-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "java_bytecode_disassembler"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Spartanlasergun", email="bns360@live.com" },
 ]
 description = "Disassembler for java bytecode"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `java_bytecode_disassembler-1.0.2/src/disassembler/java_bytecode_disassembler.py` & `java_bytecode_disassembler-1.0.3/src/java_bytecode_disassembler/java_bytecode_disassembler.py`

 * *Files identical despite different names*

### Comparing `java_bytecode_disassembler-1.0.2/src/java_bytecode_disassembler.egg-info/PKG-INFO` & `java_bytecode_disassembler-1.0.3/src/java_bytecode_disassembler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: java-bytecode-disassembler
-Version: 1.0.2
+Version: 1.0.3
 Summary: Disassembler for java bytecode
 Author-email: Spartanlasergun <bns360@live.com>
 Project-URL: Homepage, https://github.com/Spartanlasergun/java_bytecode_disassembler
 Project-URL: Bug Tracker, https://github.com/Spartanlasergun/java_bytecode_disassembler/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

