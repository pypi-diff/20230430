# Comparing `tmp/polygone-0.1.0.tar.gz` & `tmp/polygone-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polygone-0.1.0.tar", max compression
+gzip compressed data, was "polygone-0.1.2.tar", max compression
```

## Comparing `polygone-0.1.0.tar` & `polygone-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      359 2023-04-30 00:40:27.947209 polygone-0.1.0/README.md
--rw-r--r--   0        0        0       60 2023-04-30 00:14:11.766982 polygone-0.1.0/polygone/__main__.py
--rw-r--r--   0        0        0     3487 2023-04-30 00:48:50.513538 polygone-0.1.0/polygone/cli.py
--rw-r--r--   0        0        0     1445 2023-04-30 00:16:48.951724 polygone-0.1.0/polygone/log.py
--rw-r--r--   0        0        0     4823 2023-04-30 00:46:01.387841 polygone-0.1.0/polygone/packer.py
--rw-r--r--   0        0        0      417 2023-04-30 00:48:00.987125 polygone-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      902 1970-01-01 00:00:00.000000 polygone-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      359 2023-04-30 00:40:27.947209 polygone-0.1.2/README.md
+-rw-r--r--   0        0        0       60 2023-04-30 00:14:11.766982 polygone-0.1.2/polygone/__main__.py
+-rw-r--r--   0        0        0     3865 2023-04-30 01:53:36.525103 polygone-0.1.2/polygone/cli.py
+-rw-r--r--   0        0        0     1445 2023-04-30 00:16:48.951724 polygone-0.1.2/polygone/log.py
+-rw-r--r--   0        0        0     4823 2023-04-30 00:46:01.387841 polygone-0.1.2/polygone/packer.py
+-rw-r--r--   0        0        0      409 2023-04-30 02:57:27.506872 polygone-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 polygone-0.1.2/PKG-INFO
```

### Comparing `polygone-0.1.0/polygone/cli.py` & `polygone-0.1.2/polygone/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 import sh
 import sys
 import os
 import typer
+import math
 import tempfile
 import zipfile
 from typing import List, Optional
 
 from PIL import Image
 from humanfriendly import format_size
 
@@ -29,14 +30,20 @@
 def pack(
     cover_f: str = typer.Argument(..., help="PNG file to use as cover"),
     content_f: str = typer.Argument(..., help="File containing data to embed"),
     output_file: str = typer.Argument(..., help="Output file"),
     should_zip: bool = typer.Option(
         False, "--zip", "-z", help="Zip the content file before embedding"
     ),
+    zip_level: int = typer.Option(
+        5,
+        "--zip-level",
+        "-l",
+        help="Compression level to use when zipping the content file",
+    ),
 ):
     logger.info(f"checking cover: {cover_f}")
 
     with open(cover_f, "rb") as output_f:
         cover_data = output_f.read()
 
     cover_image = Image.open(cover_f)
@@ -45,15 +52,15 @@
         logger.error("  cover image is not a PNG")
         raise typer.Exit(1)
 
     if should_zip:
         tmp = tempfile.NamedTemporaryFile(suffix=".zip")
         logger.info(f"  zipping content file: {content_f} -> {tmp.name}")
         # compress using zipfile deflate, medium compression
-        with zipfile.ZipFile(tmp.name, "w", zipfile.ZIP_DEFLATED, 5) as zipf:
+        with zipfile.ZipFile(tmp.name, "w", zipfile.ZIP_DEFLATED, zip_level) as zipf:
             zipf.write(content_f, os.path.basename(content_f))
         content_f = tmp.name
 
     # get size of content file on disk
     content_file_size = os.path.getsize(content_f)
 
     # get size of cover image on disk
@@ -61,20 +68,24 @@
 
     # check dimensions, ensure they are large enough to embed the content
     cover_width, cover_height = cover_image.size
     logger.info(f"  cover image size: {cover_width}x{cover_height}")
 
     cover_pixel_count = cover_width * cover_height
 
-    cover_can_fit_content = cover_file_size < cover_pixel_count - content_file_size
+    cover_remaining_budget = cover_pixel_count - cover_file_size
+    cover_can_fit_content = cover_file_size < cover_remaining_budget
 
     if not cover_can_fit_content:
         logger.error("  cover image is too small to embed the content")
         logger.error(
-            f"    failed condition: {cover_file_size} < {cover_pixel_count} - {content_file_size}"
+            f"    failed condition: {cover_file_size} < {cover_remaining_budget} ({cover_pixel_count} - {content_file_size})"
+        )
+        logger.info(
+            f"    hint: try using a larger cover image, or compressing the content file"
         )
         raise typer.Exit(1)
 
     logger.info(f"packing: {cover_f} + {content_f} -> {output_file}")
 
     with open(output_file, "wb") as output_f:
         cover_f = open(cover_f, "rb")
```

### Comparing `polygone-0.1.0/polygone/log.py` & `polygone-0.1.2/polygone/log.py`

 * *Files identical despite different names*

### Comparing `polygone-0.1.0/polygone/packer.py` & `polygone-0.1.2/polygone/packer.py`

 * *Files identical despite different names*

### Comparing `polygone-0.1.0/PKG-INFO` & `polygone-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: polygone
-Version: 0.1.0
+Version: 0.1.2
 Summary: 
-Author: Your Name
-Author-email: you@example.com
+Author: nemo
+Author-email: nemo@alt.icu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: humanfriendly (>=10.0,<11.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
```

