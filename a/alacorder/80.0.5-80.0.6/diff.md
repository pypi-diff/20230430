# Comparing `tmp/alacorder-80.0.5.tar.gz` & `tmp/alacorder-80.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.0.5.tar", max compression
+gzip compressed data, was "alacorder-80.0.6.tar", max compression
```

## Comparing `alacorder-80.0.5.tar` & `alacorder-80.0.6.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.0.5/LICENSE
--rw-r--r--   0        0        0     6821 2023-04-29 16:14:55.778453 alacorder-80.0.5/README.md
--rw-r--r--   0        0        0      697 2023-04-29 16:03:14.696382 alacorder-80.0.5/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-04-29 15:44:27.166659 alacorder-80.0.5/src/alacorder/.DS_Store
--rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-80.0.5/src/alacorder/__init__.py
--rw-r--r--   0        0        0   198035 2023-04-29 16:02:26.019897 alacorder-80.0.5/src/alacorder/__main__.py
--rw-r--r--   0        0        0   198035 2023-04-29 16:02:31.026154 alacorder-80.0.5/src/alacorder/alac.py
--rw-r--r--   0        0        0     7750 1970-01-01 00:00:00.000000 alacorder-80.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.0.6/LICENSE
+-rw-r--r--   0        0        0     6821 2023-04-29 16:14:55.778453 alacorder-80.0.6/README.md
+-rw-r--r--   0        0        0      697 2023-04-29 16:58:31.189834 alacorder-80.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-80.0.6/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   198007 2023-04-29 16:57:59.791922 alacorder-80.0.6/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   198007 2023-04-29 16:57:53.150392 alacorder-80.0.6/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7750 1970-01-01 00:00:00.000000 alacorder-80.0.6/PKG-INFO
```

### Comparing `alacorder-80.0.5/LICENSE` & `alacorder-80.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.5/README.md` & `alacorder-80.0.6/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.5/pyproject.toml` & `alacorder-80.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.0.5"
+version = "80.0.6"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.0.5/src/alacorder/__init__.py` & `alacorder-80.0.6/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.5/src/alacorder/__main__.py` & `alacorder-80.0.6/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.0.5"
+version = "80.0.6"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2232,15 +2232,14 @@
             pl.col("FinancialHistory")
             .str.extract(r"\s([0-9]{7})\s")
             .alias("TransactionBatch"),
             pl.col("FinancialHistory").str.extract(r"\s([A-Z]{3})$").alias("Operator"),
         ]
     )
     fh = fh.select(
-        "FinancialHistory",
         "TransactionDate",
         "Description",
         "DisbursementAccount",
         "TransactionBatch",
         "ReceiptNumber",
         "Amount",
         "FromParty",
```

### Comparing `alacorder-80.0.5/src/alacorder/alac.py` & `alacorder-80.0.6/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.0.5"
+version = "80.0.6"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2232,15 +2232,14 @@
             pl.col("FinancialHistory")
             .str.extract(r"\s([0-9]{7})\s")
             .alias("TransactionBatch"),
             pl.col("FinancialHistory").str.extract(r"\s([A-Z]{3})$").alias("Operator"),
         ]
     )
     fh = fh.select(
-        "FinancialHistory",
         "TransactionDate",
         "Description",
         "DisbursementAccount",
         "TransactionBatch",
         "ReceiptNumber",
         "Amount",
         "FromParty",
```

### Comparing `alacorder-80.0.5/PKG-INFO` & `alacorder-80.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.0.5
+Version: 80.0.6
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

