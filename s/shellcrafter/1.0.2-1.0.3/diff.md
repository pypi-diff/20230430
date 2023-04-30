# Comparing `tmp/shellcrafter-1.0.2.tar.gz` & `tmp/shellcrafter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellcrafter-1.0.2.tar", last modified: Sun Apr 30 02:34:39 2023, max compression
+gzip compressed data, was "shellcrafter-1.0.3.tar", last modified: Sun Apr 30 12:07:35 2023, max compression
```

## Comparing `shellcrafter-1.0.2.tar` & `shellcrafter-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:34:39.019671 shellcrafter-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-30 02:34:39.019671 shellcrafter-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-30 02:34:08.000000 shellcrafter-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-30 02:34:08.000000 shellcrafter-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 02:34:39.019671 shellcrafter-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-30 02:34:08.000000 shellcrafter-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:34:39.015671 shellcrafter-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:34:39.019671 shellcrafter-1.0.2/src/shellcrafter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 02:34:08.000000 shellcrafter-1.0.2/src/shellcrafter/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1100 2023-04-30 02:34:08.000000 shellcrafter-1.0.2/src/shellcrafter/ascii_hex_stack_push_converter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11958 2023-04-30 02:34:08.000000 shellcrafter-1.0.2/src/shellcrafter/find_gadgets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-04-30 02:34:08.000000 shellcrafter-1.0.2/src/shellcrafter/keyst_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1082 2023-04-30 02:34:08.000000 shellcrafter-1.0.2/src/shellcrafter/ror_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:34:39.019671 shellcrafter-1.0.2/src/shellcrafter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-30 02:34:39.000000 shellcrafter-1.0.2/src/shellcrafter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-30 02:34:39.000000 shellcrafter-1.0.2/src/shellcrafter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 02:34:39.000000 shellcrafter-1.0.2/src/shellcrafter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-30 02:34:39.000000 shellcrafter-1.0.2/src/shellcrafter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-30 02:34:39.000000 shellcrafter-1.0.2/src/shellcrafter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-30 02:34:39.000000 shellcrafter-1.0.2/src/shellcrafter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:07:35.443284 shellcrafter-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-30 12:07:35.443284 shellcrafter-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-30 12:07:14.000000 shellcrafter-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-30 12:07:14.000000 shellcrafter-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 12:07:35.443284 shellcrafter-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-30 12:07:14.000000 shellcrafter-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:07:35.443284 shellcrafter-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:07:35.443284 shellcrafter-1.0.3/src/shellcrafter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 12:07:14.000000 shellcrafter-1.0.3/src/shellcrafter/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1121 2023-04-30 12:07:14.000000 shellcrafter-1.0.3/src/shellcrafter/ascii_hex_stack_push_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11958 2023-04-30 12:07:14.000000 shellcrafter-1.0.3/src/shellcrafter/find_gadgets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-04-30 12:07:14.000000 shellcrafter-1.0.3/src/shellcrafter/keyst_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1082 2023-04-30 12:07:14.000000 shellcrafter-1.0.3/src/shellcrafter/ror_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:07:35.443284 shellcrafter-1.0.3/src/shellcrafter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-30 12:07:35.000000 shellcrafter-1.0.3/src/shellcrafter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-30 12:07:35.000000 shellcrafter-1.0.3/src/shellcrafter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:07:35.000000 shellcrafter-1.0.3/src/shellcrafter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-30 12:07:35.000000 shellcrafter-1.0.3/src/shellcrafter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-30 12:07:35.000000 shellcrafter-1.0.3/src/shellcrafter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-30 12:07:35.000000 shellcrafter-1.0.3/src/shellcrafter.egg-info/top_level.txt
```

### Comparing `shellcrafter-1.0.2/PKG-INFO` & `shellcrafter-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellcrafter
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package containing scripts for developing and generating shellcode
 Author: totekuh
 Author-email: totekuh@protonmail.com
 
 # Shellcrafter
 
 Shellcrafter is a package containing scripts for developing and generating shellcode.
```

### Comparing `shellcrafter-1.0.2/README.md` & `shellcrafter-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.2/setup.py` & `shellcrafter-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-version = "1.0.2"
+version = "1.0.3"
 
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
```

### Comparing `shellcrafter-1.0.2/src/shellcrafter/ascii_hex_stack_push_converter.py` & `shellcrafter-1.0.3/src/shellcrafter/ascii_hex_stack_push_converter.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 def str_to_hex_little_endian_push(s):
     hex_str = binascii.hexlify(s.encode('utf-8')).decode('utf-8')
     hex_str = ''.join(reversed([hex_str[i:i+2] for i in range(0, len(hex_str), 2)]))
     if len(hex_str) % 8 != 0:
         hex_str = '0' * (8 - len(hex_str) % 8) + hex_str
     result = os.linesep.join([hex_str[i:i + 8] for i in range(0, len(hex_str), 8)])
     result = [f"push 0x{h}" for h in result.split(os.linesep)]
+    result.reverse()
     for h in result:
         print(h)
 
 def main():
     options = get_arguments()
     string = options.input
     str_to_hex_little_endian_push(s=string)
```

### Comparing `shellcrafter-1.0.2/src/shellcrafter/find_gadgets.py` & `shellcrafter-1.0.3/src/shellcrafter/find_gadgets.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.2/src/shellcrafter/keyst_api.py` & `shellcrafter-1.0.3/src/shellcrafter/keyst_api.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.2/src/shellcrafter/ror_hash.py` & `shellcrafter-1.0.3/src/shellcrafter/ror_hash.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.2/src/shellcrafter.egg-info/PKG-INFO` & `shellcrafter-1.0.3/src/shellcrafter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellcrafter
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package containing scripts for developing and generating shellcode
 Author: totekuh
 Author-email: totekuh@protonmail.com
 
 # Shellcrafter
 
 Shellcrafter is a package containing scripts for developing and generating shellcode.
```

