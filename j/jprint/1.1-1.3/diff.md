# Comparing `tmp/jprint-1.1.tar.gz` & `tmp/jprint-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "jprint-1.3.tar", max compression
```

## Comparing `jprint-1.1.tar` & `jprint-1.3.tar`

### file list

```diff
@@ -1,13 +1,5 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 jprint-1.1/.DS_Store
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jprint-1.1/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jprint-1.1/.vscode/settings.json
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 jprint-1.1/images/.DS_Store
--rw-r--r--   0        0        0    27802 2020-02-02 00:00:00.000000 jprint-1.1/images/json_img.png
--rw-r--r--   0        0        0    12413 2020-02-02 00:00:00.000000 jprint-1.1/images/python_img.png
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jprint-1.1/jprint/__init__.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 jprint-1.1/jprint/jprint.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 jprint-1.1/tests/test_jprint.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 jprint-1.1/.gitignore
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 jprint-1.1/README.md
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 jprint-1.1/pyproject.toml
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 jprint-1.1/PKG-INFO
+-rw-r--r--   0        0        0     1449 2023-04-15 14:20:06.268592 jprint-1.3/README.md
+-rw-r--r--   0        0        0       67 2023-04-15 13:54:50.797872 jprint-1.3/jprint/__init__.py
+-rw-r--r--   0        0        0     1012 2023-04-30 11:37:34.068427 jprint-1.3/jprint/jprint.py
+-rw-r--r--   0        0        0      694 2023-04-30 11:40:53.972767 jprint-1.3/pyproject.toml
+-rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 jprint-1.3/PKG-INFO
```

### Comparing `jprint-1.1/jprint/jprint.py` & `jprint-1.3/jprint/jprint.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,23 +14,22 @@
     """
     kwargs["indent"] = kwargs.get("indent", 4)
     kwargs["default"] = kwargs.get("default", str)
     kwargs["sort_keys"] = kwargs.get("sort_keys", True)
     return json.dumps(obj, **kwargs)
 
 
-def jprint(obj: Union[dict, str], **kwargs):
+def jprint(obj: Union[dict, list, str], **kwargs):
     """
-    Pretty print Python dictionaries and JSON strings.
+    Pretty print Python dictionaries, lists, and JSON strings.
     If str is not valid json it will be printed as is.
     """
-    if isinstance(obj, dict):
+    if isinstance(obj, (dict, list)):
         json_str = format(obj, **kwargs)
     else:
         try:
             json_str = format(json.loads(obj), **kwargs)
         except json.JSONDecodeError:
             json_str = format(obj, **kwargs)
-            # raise ValueError("Input str is not a valid JSON string")
 
     colorized_json = highlight(json_str, JsonLexer(), TerminalFormatter())
     print(colorized_json)
```

### Comparing `jprint-1.1/README.md` & `jprint-1.3/README.md`

 * *Files identical despite different names*

### Comparing `jprint-1.1/PKG-INFO` & `jprint-1.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 Metadata-Version: 2.1
 Name: jprint
-Version: 1.1
+Version: 1.3
 Summary: A simple JSON and python dictionary pretty printer
-Project-URL: Homepage, https://github.com/gnulnx/jprint
-Author-email: John Furr <gnulnx@gmail.com>
+License: MIT
+Author: John Furr
+Author-email: gnulnx@gmail.com
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: Pygments (==2.15.0)
+Project-URL: Homepage, https://github.com/gnulnx/jprint
 Description-Content-Type: text/markdown
 
 # jprint
 A simple tool for pretty priting json strings and python dictionaries to the console.
 
 
 ## Python Dictionary Example
@@ -66,8 +75,8 @@
 ```
 
 ![Json Image](https://raw.githubusercontent.com/gnulnx/jprint/main/images/json_img.png?token=GHSAT0AAAAAAB6XJL5ITD2PDRN26LXXB7MSZB2YCFQ)
 
 ## Under The Covers
 
 jprint makes use of the pygmyents library for colored output and json.dumps() for other formatting. 
-You can pass jprint any of the parameters that you would pass to json.dumps
+You can pass jprint any of the parameters that you would pass to json.dumps
```

