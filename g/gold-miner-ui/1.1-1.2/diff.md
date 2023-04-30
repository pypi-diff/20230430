# Comparing `tmp/gold-miner-ui-1.1.tar.gz` & `tmp/gold-miner-ui-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gold-miner-ui-1.1.tar", last modified: Fri Apr 28 08:58:09 2023, max compression
+gzip compressed data, was "gold-miner-ui-1.2.tar", last modified: Sun Apr 30 13:01:55 2023, max compression
```

## Comparing `gold-miner-ui-1.1.tar` & `gold-miner-ui-1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:58:09.018945 gold-miner-ui-1.1/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1069 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/LICENSE
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      705 2023-04-28 08:58:09.018945 gold-miner-ui-1.1/PKG-INFO
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      287 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/README.md
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:58:09.015945 gold-miner-ui-1.1/apropos/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/__init__.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:58:09.015945 gold-miner-ui-1.1/apropos/goldminer/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/__init__.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:58:09.016945 gold-miner-ui-1.1/apropos/goldminer/output/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/output/__init__.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     4331 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/output/goldQt.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:58:09.017945 gold-miner-ui-1.1/apropos/goldminer/reports/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/__init__.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1832 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/cancel.svg
--rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)     1808 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/check.svg
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     8410 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/hardhat.svg
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       63 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/header.html
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      796 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/navbar-summary.html
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1118 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/navbar.html
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      567 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/report.css
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      639 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/summary-template.md
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3020 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/template.html
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3356 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/template.md
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:58:09.017945 gold-miner-ui-1.1/apropos/goldminer/tools/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/tools/__init__.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     7479 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/tools/auditor.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     9310 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/tools/fingerprinter.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)    37608 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/tools/tande.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:58:09.017945 gold-miner-ui-1.1/gold_miner_ui.egg-info/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      705 2023-04-28 08:58:08.000000 gold-miner-ui-1.1/gold_miner_ui.egg-info/PKG-INFO
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      949 2023-04-28 08:58:08.000000 gold-miner-ui-1.1/gold_miner_ui.egg-info/SOURCES.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)        1 2023-04-28 08:58:08.000000 gold-miner-ui-1.1/gold_miner_ui.egg-info/dependency_links.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      198 2023-04-28 08:58:08.000000 gold-miner-ui-1.1/gold_miner_ui.egg-info/entry_points.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       75 2023-04-28 08:58:08.000000 gold-miner-ui-1.1/gold_miner_ui.egg-info/requires.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)        8 2023-04-28 08:58:08.000000 gold-miner-ui-1.1/gold_miner_ui.egg-info/top_level.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-04-28 08:58:09.018945 gold-miner-ui-1.1/setup.cfg
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1539 2023-04-28 08:57:56.000000 gold-miner-ui-1.1/setup.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-30 13:01:55.132677 gold-miner-ui-1.2/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1069 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/LICENSE
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      705 2023-04-30 13:01:55.132677 gold-miner-ui-1.2/PKG-INFO
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      287 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/README.md
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-30 13:01:55.129677 gold-miner-ui-1.2/apropos/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/__init__.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-30 13:01:55.129677 gold-miner-ui-1.2/apropos/goldminer/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/goldminer/__init__.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-30 13:01:55.129677 gold-miner-ui-1.2/apropos/goldminer/output/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/goldminer/output/__init__.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     4331 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/goldminer/output/goldQt.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-30 13:01:55.130677 gold-miner-ui-1.2/apropos/goldminer/reports/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/goldminer/reports/__init__.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1832 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/goldminer/reports/cancel.svg
+-rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)     1808 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/goldminer/reports/check.svg
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     8410 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/goldminer/reports/hardhat.svg
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       63 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/goldminer/reports/header.html
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      796 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/goldminer/reports/navbar-summary.html
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1118 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/goldminer/reports/navbar.html
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      567 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/goldminer/reports/report.css
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      639 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/goldminer/reports/summary-template.md
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3020 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/goldminer/reports/template.html
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3356 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/goldminer/reports/template.md
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-30 13:01:55.131677 gold-miner-ui-1.2/apropos/goldminer/tools/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/goldminer/tools/__init__.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     7479 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/goldminer/tools/auditor.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     9310 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/goldminer/tools/fingerprinter.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)    37608 2023-04-28 08:40:21.000000 gold-miner-ui-1.2/apropos/goldminer/tools/tande.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-30 13:01:55.132677 gold-miner-ui-1.2/gold_miner_ui.egg-info/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      705 2023-04-30 13:01:55.000000 gold-miner-ui-1.2/gold_miner_ui.egg-info/PKG-INFO
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      949 2023-04-30 13:01:55.000000 gold-miner-ui-1.2/gold_miner_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)        1 2023-04-30 13:01:55.000000 gold-miner-ui-1.2/gold_miner_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      198 2023-04-30 13:01:55.000000 gold-miner-ui-1.2/gold_miner_ui.egg-info/entry_points.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       75 2023-04-30 13:01:55.000000 gold-miner-ui-1.2/gold_miner_ui.egg-info/requires.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)        8 2023-04-30 13:01:55.000000 gold-miner-ui-1.2/gold_miner_ui.egg-info/top_level.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-04-30 13:01:55.132677 gold-miner-ui-1.2/setup.cfg
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1539 2023-04-30 13:00:01.000000 gold-miner-ui-1.2/setup.py
```

### Comparing `gold-miner-ui-1.1/LICENSE` & `gold-miner-ui-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.1/PKG-INFO` & `gold-miner-ui-1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gold-miner-ui
-Version: 1.1
+Version: 1.2
 Summary: A UI plugin that adds graphical extensions to gold-miner
 Home-page: https://gitlab.com/isi-apropos/gold-miner-ui
 Author: Wes Hardaker
 Author-email: opensource@hardakers.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `gold-miner-ui-1.1/apropos/goldminer/output/goldQt.py` & `gold-miner-ui-1.2/apropos/goldminer/output/goldQt.py`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.1/apropos/goldminer/reports/cancel.svg` & `gold-miner-ui-1.2/apropos/goldminer/reports/cancel.svg`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.1/apropos/goldminer/reports/check.svg` & `gold-miner-ui-1.2/apropos/goldminer/reports/check.svg`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.1/apropos/goldminer/reports/hardhat.svg` & `gold-miner-ui-1.2/apropos/goldminer/reports/hardhat.svg`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.1/apropos/goldminer/reports/navbar-summary.html` & `gold-miner-ui-1.2/apropos/goldminer/reports/navbar-summary.html`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.1/apropos/goldminer/reports/navbar.html` & `gold-miner-ui-1.2/apropos/goldminer/reports/navbar.html`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.1/apropos/goldminer/reports/report.css` & `gold-miner-ui-1.2/apropos/goldminer/reports/report.css`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.1/apropos/goldminer/reports/summary-template.md` & `gold-miner-ui-1.2/apropos/goldminer/reports/summary-template.md`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.1/apropos/goldminer/reports/template.html` & `gold-miner-ui-1.2/apropos/goldminer/reports/template.html`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.1/apropos/goldminer/reports/template.md` & `gold-miner-ui-1.2/apropos/goldminer/reports/template.md`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.1/apropos/goldminer/tools/auditor.py` & `gold-miner-ui-1.2/apropos/goldminer/tools/auditor.py`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.1/apropos/goldminer/tools/fingerprinter.py` & `gold-miner-ui-1.2/apropos/goldminer/tools/fingerprinter.py`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.1/apropos/goldminer/tools/tande.py` & `gold-miner-ui-1.2/apropos/goldminer/tools/tande.py`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.1/gold_miner_ui.egg-info/PKG-INFO` & `gold-miner-ui-1.2/gold_miner_ui.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gold-miner-ui
-Version: 1.1
+Version: 1.2
 Summary: A UI plugin that adds graphical extensions to gold-miner
 Home-page: https://gitlab.com/isi-apropos/gold-miner-ui
 Author: Wes Hardaker
 Author-email: opensource@hardakers.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `gold-miner-ui-1.1/gold_miner_ui.egg-info/SOURCES.txt` & `gold-miner-ui-1.2/gold_miner_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.1/setup.py` & `gold-miner-ui-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gold-miner-ui",
-    version="1.1",
+    version="1.2",
     author="Wes Hardaker",
     author_email="opensource@hardakers.net",
     description="A UI plugin that adds graphical extensions to gold-miner",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/isi-apropos/gold-miner-ui",
     packages=setuptools.find_packages(),
```

