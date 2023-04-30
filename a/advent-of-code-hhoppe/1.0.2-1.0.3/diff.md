# Comparing `tmp/advent-of-code-hhoppe-1.0.2.tar.gz` & `tmp/advent-of-code-hhoppe-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advent-of-code-hhoppe-1.0.2.tar", last modified: Fri Apr  7 23:19:39 2023, max compression
+gzip compressed data, was "advent-of-code-hhoppe-1.0.3.tar", last modified: Sun Apr 30 04:13:24 2023, max compression
```

## Comparing `advent-of-code-hhoppe-1.0.2.tar` & `advent-of-code-hhoppe-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-04-07 23:19:31.652335 advent-of-code-hhoppe-1.0.2/LICENSE
--rw-r--r--   0        0        0     2367 2023-04-07 23:19:31.652335 advent-of-code-hhoppe-1.0.2/README.md
--rw-r--r--   0        0        0     7737 2023-04-07 23:19:31.652335 advent-of-code-hhoppe-1.0.2/advent_of_code_hhoppe/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 23:19:31.652335 advent-of-code-hhoppe-1.0.2/advent_of_code_hhoppe/py.typed
--rw-r--r--   0        0        0      907 2023-04-07 23:19:31.652335 advent-of-code-hhoppe-1.0.2/advent_of_code_hhoppe/setup.cfg
--rw-r--r--   0        0        0     2017 2023-04-07 23:19:31.652335 advent-of-code-hhoppe-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 advent-of-code-hhoppe-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-30 04:13:14.972766 advent-of-code-hhoppe-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2367 2023-04-30 04:13:14.972766 advent-of-code-hhoppe-1.0.3/README.md
+-rw-r--r--   0        0        0     7733 2023-04-30 04:13:14.972766 advent-of-code-hhoppe-1.0.3/advent_of_code_hhoppe/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 04:13:14.972766 advent-of-code-hhoppe-1.0.3/advent_of_code_hhoppe/py.typed
+-rw-r--r--   0        0        0      907 2023-04-30 04:13:14.972766 advent-of-code-hhoppe-1.0.3/advent_of_code_hhoppe/setup.cfg
+-rw-r--r--   0        0        0     1993 2023-04-30 04:13:14.972766 advent-of-code-hhoppe-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 advent-of-code-hhoppe-1.0.3/PKG-INFO
```

### Comparing `advent-of-code-hhoppe-1.0.2/LICENSE` & `advent-of-code-hhoppe-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `advent-of-code-hhoppe-1.0.2/README.md` & `advent-of-code-hhoppe-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `advent-of-code-hhoppe-1.0.2/advent_of_code_hhoppe/__init__.py` & `advent-of-code-hhoppe-1.0.3/advent_of_code_hhoppe/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 """Library for Advent of Code -- Hugues Hoppe."""
 
 from __future__ import annotations
 
 __docformat__ = 'google'
-__version__ = '1.0.2'
+__version__ = '1.0.3'
 __version_info__ = tuple(int(num) for num in __version__.split('.'))
 
 from collections.abc import Callable
 import contextlib
 import dataclasses
 import numbers
 import pathlib
@@ -25,16 +25,15 @@
 
 
 def _read_contents(path_or_url: str, /) -> bytes:
   if path_or_url.startswith(('http://', 'https://')):
     with urllib.request.urlopen(path_or_url) as response:
       data: bytes = response.read()
     return data
-  with open(path_or_url, 'rb') as f:
-    return f.read()
+  return pathlib.Path(path_or_url).read_bytes()
 
 
 @dataclasses.dataclass
 class PuzzlePart:
   """Part (1 or 2) of a daily puzzle."""
 
   advent: Advent = dataclasses.field(repr=False)
@@ -57,15 +56,15 @@
         answer: str = puz.answer_a
         return answer
     elif self.part == 2:
       if puz.answered_b:
         answer = puz.answer_b
         return answer
     else:
-      raise AssertionError()
+      raise ValueError(self.part)
     return None
 
   def compute(self, input_: str, /, *, silent: bool = False, repeat: int = 1) -> None:
     """Run the stored function on the selected input."""
     assert self.func
     elapsed_times = []
     for _ in range(repeat):
```

### Comparing `advent-of-code-hhoppe-1.0.2/advent_of_code_hhoppe/setup.cfg` & `advent-of-code-hhoppe-1.0.3/advent_of_code_hhoppe/setup.cfg`

 * *Files identical despite different names*

### Comparing `advent-of-code-hhoppe-1.0.2/pyproject.toml` & `advent-of-code-hhoppe-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 pyink-indentation = 2
 line-length = 100  # Default is 88.
 pyink-use-majority-quotes = true
 extend-exclude = "\\.ipynb"
 
 [tool.pylint.main]
 disable = [
-    "unspecified-encoding", "fixme", "redefined-builtin", "cell-var-from-loop",
+    "fixme", "redefined-builtin", "cell-var-from-loop",
     "using-constant-test", "simplifiable-condition", "import-outside-toplevel", "line-too-long",
     "too-many-lines", "too-few-public-methods", "too-many-arguments", "too-many-locals", "use-dict-literal",
 ]
 reports = false
 score = false
 recursive = true
 ignore-paths = [".*\\.ipynb_checkpoints"]
```

### Comparing `advent-of-code-hhoppe-1.0.2/PKG-INFO` & `advent-of-code-hhoppe-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advent-of-code-hhoppe
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for Advent of Code -- Hugues Hoppe.
 Keywords: 
 Author-email: Hugues Hoppe <hhoppe@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

