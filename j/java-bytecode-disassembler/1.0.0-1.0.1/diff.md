# Comparing `tmp/java_bytecode_disassembler-1.0.0.tar.gz` & `tmp/java_bytecode_disassembler-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "java_bytecode_disassembler-1.0.0.tar", last modified: Sun Apr 30 21:05:54 2023, max compression
+gzip compressed data, was "java_bytecode_disassembler-1.0.1.tar", last modified: Sun Apr 30 21:10:03 2023, max compression
```

## Comparing `java_bytecode_disassembler-1.0.0.tar` & `java_bytecode_disassembler-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 21:05:54.388316 java_bytecode_disassembler-1.0.0/
--rw-rw-rw-   0        0        0    26526 2023-04-27 00:53:09.000000 java_bytecode_disassembler-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      802 2023-04-30 21:05:54.388316 java_bytecode_disassembler-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       98 2023-04-27 00:53:09.000000 java_bytecode_disassembler-1.0.0/README.md
--rw-rw-rw-   0        0        0      761 2023-04-30 21:04:55.000000 java_bytecode_disassembler-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 21:05:54.388316 java_bytecode_disassembler-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-30 21:05:54.294564 java_bytecode_disassembler-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 21:05:54.325812 java_bytecode_disassembler-1.0.0/src/disassembler/
--rw-rw-rw-   0        0        0       66 2023-04-29 14:05:19.000000 java_bytecode_disassembler-1.0.0/src/disassembler/__init__.py
--rw-rw-rw-   0        0        0    95221 2023-04-30 21:00:41.000000 java_bytecode_disassembler-1.0.0/src/disassembler/java_bytecode_disassembler.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:05:54.388316 java_bytecode_disassembler-1.0.0/src/java_bytecode_disassembler.egg-info/
--rw-rw-rw-   0        0        0      802 2023-04-30 21:05:54.000000 java_bytecode_disassembler-1.0.0/src/java_bytecode_disassembler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-04-30 21:05:54.000000 java_bytecode_disassembler-1.0.0/src/java_bytecode_disassembler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 21:05:54.000000 java_bytecode_disassembler-1.0.0/src/java_bytecode_disassembler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-30 21:05:54.000000 java_bytecode_disassembler-1.0.0/src/java_bytecode_disassembler.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-30 21:05:54.388316 java_bytecode_disassembler-1.0.0/tests/
--rw-rw-rw-   0        0        0      218 2023-04-30 21:03:13.000000 java_bytecode_disassembler-1.0.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:10:03.699427 java_bytecode_disassembler-1.0.1/
+-rw-rw-rw-   0        0        0    26526 2023-04-27 00:53:09.000000 java_bytecode_disassembler-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      824 2023-04-30 21:10:03.683801 java_bytecode_disassembler-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       98 2023-04-27 00:53:09.000000 java_bytecode_disassembler-1.0.1/README.md
+-rw-rw-rw-   0        0        0      783 2023-04-30 21:09:32.000000 java_bytecode_disassembler-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 21:10:03.699427 java_bytecode_disassembler-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 21:10:03.621299 java_bytecode_disassembler-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 21:10:03.652548 java_bytecode_disassembler-1.0.1/src/disassembler/
+-rw-rw-rw-   0        0        0       66 2023-04-29 14:05:19.000000 java_bytecode_disassembler-1.0.1/src/disassembler/__init__.py
+-rw-rw-rw-   0        0        0    95221 2023-04-30 21:00:41.000000 java_bytecode_disassembler-1.0.1/src/disassembler/java_bytecode_disassembler.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:10:03.668174 java_bytecode_disassembler-1.0.1/src/java_bytecode_disassembler.egg-info/
+-rw-rw-rw-   0        0        0      824 2023-04-30 21:10:03.000000 java_bytecode_disassembler-1.0.1/src/java_bytecode_disassembler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-04-30 21:10:03.000000 java_bytecode_disassembler-1.0.1/src/java_bytecode_disassembler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 21:10:03.000000 java_bytecode_disassembler-1.0.1/src/java_bytecode_disassembler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-30 21:10:03.000000 java_bytecode_disassembler-1.0.1/src/java_bytecode_disassembler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 21:10:03.683801 java_bytecode_disassembler-1.0.1/tests/
+-rw-rw-rw-   0        0        0      218 2023-04-30 21:03:13.000000 java_bytecode_disassembler-1.0.1/tests/test.py
```

### Comparing `java_bytecode_disassembler-1.0.0/LICENSE` & `java_bytecode_disassembler-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `java_bytecode_disassembler-1.0.0/PKG-INFO` & `java_bytecode_disassembler-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: java_bytecode_disassembler
-Version: 1.0.0
+Version: 1.0.1
 Summary: Disassembler for java bytecode
 Author-email: Spartanlasergun <bns360@live.com>
-Project-URL: Homepage, https://github.com/Spartanlasergun/calendar_widget
-Project-URL: Bug Tracker, https://github.com/Spartanlasergun/calendar_widget/issues
+Project-URL: Homepage, https://github.com/Spartanlasergun/java_bytecode_disassembler
+Project-URL: Bug Tracker, https://github.com/Spartanlasergun/java_bytecode_disassembler/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `java_bytecode_disassembler-1.0.0/pyproject.toml` & `java_bytecode_disassembler-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "java_bytecode_disassembler"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Spartanlasergun", email="bns360@live.com" },
 ]
 description = "Disassembler for java bytecode"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -16,9 +16,9 @@
   "Intended Audience :: Developers",
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
   "Operating System :: Microsoft :: Windows",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/Spartanlasergun/calendar_widget"
-"Bug Tracker" = "https://github.com/Spartanlasergun/calendar_widget/issues"
+"Homepage" = "https://github.com/Spartanlasergun/java_bytecode_disassembler"
+"Bug Tracker" = "https://github.com/Spartanlasergun/java_bytecode_disassembler/issues"
```

### Comparing `java_bytecode_disassembler-1.0.0/src/disassembler/java_bytecode_disassembler.py` & `java_bytecode_disassembler-1.0.1/src/disassembler/java_bytecode_disassembler.py`

 * *Files identical despite different names*

### Comparing `java_bytecode_disassembler-1.0.0/src/java_bytecode_disassembler.egg-info/PKG-INFO` & `java_bytecode_disassembler-1.0.1/src/java_bytecode_disassembler.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: java-bytecode-disassembler
-Version: 1.0.0
+Version: 1.0.1
 Summary: Disassembler for java bytecode
 Author-email: Spartanlasergun <bns360@live.com>
-Project-URL: Homepage, https://github.com/Spartanlasergun/calendar_widget
-Project-URL: Bug Tracker, https://github.com/Spartanlasergun/calendar_widget/issues
+Project-URL: Homepage, https://github.com/Spartanlasergun/java_bytecode_disassembler
+Project-URL: Bug Tracker, https://github.com/Spartanlasergun/java_bytecode_disassembler/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

