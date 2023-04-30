# Comparing `tmp/shellcrafter-1.0.1.tar.gz` & `tmp/shellcrafter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellcrafter-1.0.1.tar", last modified: Sun Apr 30 02:14:31 2023, max compression
+gzip compressed data, was "shellcrafter-1.0.2.tar", last modified: Sun Apr 30 02:34:39 2023, max compression
```

## Comparing `shellcrafter-1.0.1.tar` & `shellcrafter-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:14:31.742332 shellcrafter-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-30 02:14:31.738332 shellcrafter-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-30 02:14:05.000000 shellcrafter-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-30 02:14:05.000000 shellcrafter-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 02:14:31.742332 shellcrafter-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-30 02:14:05.000000 shellcrafter-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:14:31.738332 shellcrafter-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:14:31.738332 shellcrafter-1.0.1/src/shellcrafter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 02:14:05.000000 shellcrafter-1.0.1/src/shellcrafter/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1100 2023-04-30 02:14:05.000000 shellcrafter-1.0.1/src/shellcrafter/ascii_hex_stack_push_converter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11958 2023-04-30 02:14:05.000000 shellcrafter-1.0.1/src/shellcrafter/find_gadgets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-04-30 02:14:05.000000 shellcrafter-1.0.1/src/shellcrafter/keyst_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1082 2023-04-30 02:14:05.000000 shellcrafter-1.0.1/src/shellcrafter/ror_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:14:31.738332 shellcrafter-1.0.1/src/shellcrafter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-30 02:14:31.000000 shellcrafter-1.0.1/src/shellcrafter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-30 02:14:31.000000 shellcrafter-1.0.1/src/shellcrafter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 02:14:31.000000 shellcrafter-1.0.1/src/shellcrafter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-30 02:14:31.000000 shellcrafter-1.0.1/src/shellcrafter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-30 02:14:31.000000 shellcrafter-1.0.1/src/shellcrafter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-30 02:14:31.000000 shellcrafter-1.0.1/src/shellcrafter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:34:39.019671 shellcrafter-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-30 02:34:39.019671 shellcrafter-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-30 02:34:08.000000 shellcrafter-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-30 02:34:08.000000 shellcrafter-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 02:34:39.019671 shellcrafter-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-30 02:34:08.000000 shellcrafter-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:34:39.015671 shellcrafter-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:34:39.019671 shellcrafter-1.0.2/src/shellcrafter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 02:34:08.000000 shellcrafter-1.0.2/src/shellcrafter/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1100 2023-04-30 02:34:08.000000 shellcrafter-1.0.2/src/shellcrafter/ascii_hex_stack_push_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11958 2023-04-30 02:34:08.000000 shellcrafter-1.0.2/src/shellcrafter/find_gadgets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-04-30 02:34:08.000000 shellcrafter-1.0.2/src/shellcrafter/keyst_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1082 2023-04-30 02:34:08.000000 shellcrafter-1.0.2/src/shellcrafter/ror_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:34:39.019671 shellcrafter-1.0.2/src/shellcrafter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-30 02:34:39.000000 shellcrafter-1.0.2/src/shellcrafter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-30 02:34:39.000000 shellcrafter-1.0.2/src/shellcrafter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 02:34:39.000000 shellcrafter-1.0.2/src/shellcrafter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-30 02:34:39.000000 shellcrafter-1.0.2/src/shellcrafter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-30 02:34:39.000000 shellcrafter-1.0.2/src/shellcrafter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-30 02:34:39.000000 shellcrafter-1.0.2/src/shellcrafter.egg-info/top_level.txt
```

### Comparing `shellcrafter-1.0.1/PKG-INFO` & `shellcrafter-1.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,12 @@
-Metadata-Version: 2.1
-Name: shellcrafter
-Version: 1.0.1
-Summary: A package containing scripts for developing and generating shellcode
-Author: totekuh
-Author-email: totekuh@protonmail.com
-
 # Shellcrafter
 
 Shellcrafter is a package containing scripts for developing and generating shellcode. 
 
-It provides a collection of utilities for working with shellcode in various ways, such as generating shellcode from assembly instructions, computing hashes from function names, and converting ASCII text to hex stack push instructions.
+It provides a collection of utilities for working with shellcode in various ways, such as generating shellcode from assembly instructions, computing hashes from function names, converting ASCII text to hex stack push instructions, and finding ROP gadgets.
 
 ## Installation
 
 To install Shellcrafter, use pip:
 
 ```bash
 pip3 install shellcrafter
@@ -29,15 +22,17 @@
 ## Usage
 
 Shellcrafter provides the following command-line utilities:
 
 - `keyst-api`: A shellcode generator using the Keystone Engine to assemble assembly instructions into shellcode.
 - `compute-hashes-from-function-name`: Computes the hash for a given function name using the ROR operation.
 - `ascii-to-push`: Converts an ASCII string to a series of x86 PUSH instructions that represent the given string as hexadecimal values.
+- `find-gadgets`: Searches for clean, categorized gadgets from a given list of files.
 
 To get help on how to use each utility, run the corresponding command with the `-h` or `--help` flag:
 
 ```bash
 keyst-api --help
 compute-hashes-from-function-name --help
 ascii-to-push --help
+find-gadgets --help
 ```
```

### Comparing `shellcrafter-1.0.1/README.md` & `shellcrafter-1.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,19 @@
+Metadata-Version: 2.1
+Name: shellcrafter
+Version: 1.0.2
+Summary: A package containing scripts for developing and generating shellcode
+Author: totekuh
+Author-email: totekuh@protonmail.com
+
 # Shellcrafter
 
 Shellcrafter is a package containing scripts for developing and generating shellcode. 
 
-It provides a collection of utilities for working with shellcode in various ways, such as generating shellcode from assembly instructions, computing hashes from function names, and converting ASCII text to hex stack push instructions.
+It provides a collection of utilities for working with shellcode in various ways, such as generating shellcode from assembly instructions, computing hashes from function names, converting ASCII text to hex stack push instructions, and finding ROP gadgets.
 
 ## Installation
 
 To install Shellcrafter, use pip:
 
 ```bash
 pip3 install shellcrafter
@@ -22,15 +29,17 @@
 ## Usage
 
 Shellcrafter provides the following command-line utilities:
 
 - `keyst-api`: A shellcode generator using the Keystone Engine to assemble assembly instructions into shellcode.
 - `compute-hashes-from-function-name`: Computes the hash for a given function name using the ROR operation.
 - `ascii-to-push`: Converts an ASCII string to a series of x86 PUSH instructions that represent the given string as hexadecimal values.
+- `find-gadgets`: Searches for clean, categorized gadgets from a given list of files.
 
 To get help on how to use each utility, run the corresponding command with the `-h` or `--help` flag:
 
 ```bash
 keyst-api --help
 compute-hashes-from-function-name --help
 ascii-to-push --help
+find-gadgets --help
 ```
```

### Comparing `shellcrafter-1.0.1/setup.py` & `shellcrafter-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-version = "1.0.1"
+version = "1.0.2"
 
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
```

### Comparing `shellcrafter-1.0.1/src/shellcrafter/ascii_hex_stack_push_converter.py` & `shellcrafter-1.0.2/src/shellcrafter/ascii_hex_stack_push_converter.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.1/src/shellcrafter/find_gadgets.py` & `shellcrafter-1.0.2/src/shellcrafter/find_gadgets.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.1/src/shellcrafter/keyst_api.py` & `shellcrafter-1.0.2/src/shellcrafter/keyst_api.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.1/src/shellcrafter/ror_hash.py` & `shellcrafter-1.0.2/src/shellcrafter/ror_hash.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.1/src/shellcrafter.egg-info/PKG-INFO` & `shellcrafter-1.0.2/src/shellcrafter.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: shellcrafter
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package containing scripts for developing and generating shellcode
 Author: totekuh
 Author-email: totekuh@protonmail.com
 
 # Shellcrafter
 
 Shellcrafter is a package containing scripts for developing and generating shellcode. 
 
-It provides a collection of utilities for working with shellcode in various ways, such as generating shellcode from assembly instructions, computing hashes from function names, and converting ASCII text to hex stack push instructions.
+It provides a collection of utilities for working with shellcode in various ways, such as generating shellcode from assembly instructions, computing hashes from function names, converting ASCII text to hex stack push instructions, and finding ROP gadgets.
 
 ## Installation
 
 To install Shellcrafter, use pip:
 
 ```bash
 pip3 install shellcrafter
@@ -29,15 +29,17 @@
 ## Usage
 
 Shellcrafter provides the following command-line utilities:
 
 - `keyst-api`: A shellcode generator using the Keystone Engine to assemble assembly instructions into shellcode.
 - `compute-hashes-from-function-name`: Computes the hash for a given function name using the ROR operation.
 - `ascii-to-push`: Converts an ASCII string to a series of x86 PUSH instructions that represent the given string as hexadecimal values.
+- `find-gadgets`: Searches for clean, categorized gadgets from a given list of files.
 
 To get help on how to use each utility, run the corresponding command with the `-h` or `--help` flag:
 
 ```bash
 keyst-api --help
 compute-hashes-from-function-name --help
 ascii-to-push --help
+find-gadgets --help
 ```
```

