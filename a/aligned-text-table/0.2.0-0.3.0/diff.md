# Comparing `tmp/aligned_text_table-0.2.0.tar.gz` & `tmp/aligned_text_table-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligned_text_table-0.2.0.tar", max compression
+gzip compressed data, was "aligned_text_table-0.3.0.tar", max compression
```

## Comparing `aligned_text_table-0.2.0.tar` & `aligned_text_table-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      654 2023-04-28 23:55:20.419467 aligned_text_table-0.2.0/README.md
--rw-r--r--   0        0        0       21 2023-04-28 22:29:05.027773 aligned_text_table-0.2.0/aligned_text_table/__init__.py
--rw-r--r--   0        0        0     2057 2023-04-29 00:38:42.566669 aligned_text_table-0.2.0/aligned_text_table/parser.py
--rw-r--r--   0        0        0      464 2023-04-29 00:39:26.491256 aligned_text_table-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 aligned_text_table-0.2.0/setup.py
--rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 aligned_text_table-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      654 2023-04-28 23:55:20.419467 aligned_text_table-0.3.0/README.md
+-rw-r--r--   0        0        0       36 2023-04-30 07:03:08.744674 aligned_text_table-0.3.0/aligned_text_table/__init__.py
+-rw-r--r--   0        0        0     1855 2023-04-30 07:03:32.001582 aligned_text_table-0.3.0/aligned_text_table/parser.py
+-rw-r--r--   0        0        0      464 2023-04-29 07:35:38.543534 aligned_text_table-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 aligned_text_table-0.3.0/setup.py
+-rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 aligned_text_table-0.3.0/PKG-INFO
```

### Comparing `aligned_text_table-0.2.0/README.md` & `aligned_text_table-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aligned_text_table-0.2.0/aligned_text_table/parser.py` & `aligned_text_table-0.3.0/aligned_text_table/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 import re
 
 
-def parse_row(
-    lines: list, keys: list
-) -> dict:
+class LineLengthError(Exception):
+    pass
+
+
+def parse_row(lines: list) -> list:
     """
     This will parse a single multi-line row of a space-aligned table into a
-    Python dictionary containing the data mapped to the provided `keys`.
+    list containing the text for each column.
 
     ```
     >>> parse_row(
     ...     lines=[
     ...         "This is     Column two   This one ",
     ...         "column one               is column",
     ...         "                         three    "
-    ...     ],
-    ...     keys=["One", "Two", "Three"]
+    ...     ]
     ... )
-    
-    {
-        "One": "This is column one",
-        "Two": "Column two",
-        "Three": "This one is column three"
-    }
+
+    [
+        "This is column one",
+        "Column two",
+        "This one is column three"
+    ]
     ```
     """
 
     first_line = lines[0]
-    column_data = {}
     gutter_regex = "\s\s\s+"
 
-    # Find column locations
+    # Find column ranges
+    # ===
     column_ranges = []
     start_position = 0
     gutter_match = re.search(gutter_regex, first_line)
 
-    while(gutter_match):
+    while gutter_match:
         new_position = start_position + gutter_match.end()
-        column_ranges.append( (start_position, new_position) )
+        column_ranges.append((start_position, new_position))
         gutter_match = re.search(gutter_regex, first_line[new_position:])
         start_position = new_position
 
     # Add the final column if it wasn't already added
     if start_position < len(first_line):
-        column_ranges.append( (start_position, len(first_line)) )
-
-    if len(column_ranges) != len(keys):
-        raise ValueError(
-            "The number of keys provided doesn't match the number of columns"
-        )
-
-    # Check lines
-    for index, line in enumerate(lines):
-        # Add spaces to start of short lines
-        if len(line) < len(first_line):
-            difference = len(first_line) - len(line)
-            lines[index] = difference * " " + line
+        column_ranges.append((start_position, len(first_line)))
 
-    # Split into columns
-    for index, key in enumerate(keys):
+    # Check line length
+    # ===
+    first_line_length = len(lines[0])
+    for line in lines:
+        if len(line) != first_line_length:
+            raise LineLengthError(
+                f"Found lines of differing lengths: {first_line_length} vs {len(line)}"
+            )
+
+    # Split line text into columns
+    # ===
+    columns = []
+    for column_range in column_ranges:
         column_lines = []
 
         for line in lines:
             # Split line into columns
-            start = column_ranges[index][0]
-            end = column_ranges[index][1]
+            start = column_range[0]
+            end = column_range[1]
             column_lines.append(line[start:end].strip())
 
-        column_data[key] = " ".join(column_lines).strip()
+        columns.append(" ".join(column_lines).strip())
 
-    return column_data
+    return columns
```

### Comparing `aligned_text_table-0.2.0/setup.py` & `aligned_text_table-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['aligned_text_table']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'aligned-text-table',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Parser for space-aligned tables in plain text',
     'long_description': '# Aligned text table\n\nA parser for tables in plain text that are aligned with spaces, e.g.:\n\n```\nThis is     Column two   This one\ncolumn one               is column\n                         three\n```\n\n## Usage\n\n```\n>>> from aligned_text_table import parse_row\n\n>>> parse_row(\n...     lines=[\n...         "This is     Column two   This one ",\n...         "column one               is column",\n...         "three    "\n...     ],\n...     keys=["one", "two", "three"]\n... )\n\n{\n    "one": "This is column one",\n    "two": "Column two",\n    "three": "This one is column three"\n}\n```\n\n## Tests\n\nTo run tests, install and run Tox:\n\n```\npip3 install tox\ntox\n```\n',
     'author': 'Robin Winslow',
     'author_email': 'robin@robinwinslow.co.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/nottrobin/aligned-text-table',
```

### Comparing `aligned_text_table-0.2.0/PKG-INFO` & `aligned_text_table-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligned-text-table
-Version: 0.2.0
+Version: 0.3.0
 Summary: Parser for space-aligned tables in plain text
 Home-page: https://github.com/nottrobin/aligned-text-table
 License: Public domain
 Author: Robin Winslow
 Author-email: robin@robinwinslow.co.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

