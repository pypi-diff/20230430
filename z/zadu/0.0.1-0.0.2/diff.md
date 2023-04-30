# Comparing `tmp/zadu-0.0.1.tar.gz` & `tmp/zadu-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zadu-0.0.1.tar", last modified: Sun Apr 30 14:19:15 2023, max compression
+gzip compressed data, was "dist/zadu-0.0.2.tar", last modified: Sun Apr 30 14:30:59 2023, max compression
```

## Comparing `zadu-0.0.1.tar` & `zadu-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:19:15.523885 zadu-0.0.1/
--rw-rw-r--   0 hj        (1010) hj        (1010)     5658 2023-04-30 14:19:15.523885 zadu-0.0.1/PKG-INFO
--rw-rw-r--   0 hj        (1010) hj        (1010)     4235 2023-04-30 13:42:58.000000 zadu-0.0.1/README.md
--rw-rw-r--   0 hj        (1010) hj        (1010)       38 2023-04-30 14:19:15.523885 zadu-0.0.1/setup.cfg
--rw-rw-r--   0 hj        (1010) hj        (1010)      773 2023-04-30 14:18:27.000000 zadu-0.0.1/setup.py
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:19:15.523885 zadu-0.0.1/src/
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:19:15.523885 zadu-0.0.1/src/zadu.egg-info/
--rw-rw-r--   0 hj        (1010) hj        (1010)     5658 2023-04-30 14:19:15.000000 zadu-0.0.1/src/zadu.egg-info/PKG-INFO
--rw-rw-r--   0 hj        (1010) hj        (1010)      177 2023-04-30 14:19:15.000000 zadu-0.0.1/src/zadu.egg-info/SOURCES.txt
--rw-rw-r--   0 hj        (1010) hj        (1010)        1 2023-04-30 14:19:15.000000 zadu-0.0.1/src/zadu.egg-info/dependency_links.txt
--rw-rw-r--   0 hj        (1010) hj        (1010)       40 2023-04-30 14:19:15.000000 zadu-0.0.1/src/zadu.egg-info/requires.txt
--rw-rw-r--   0 hj        (1010) hj        (1010)        1 2023-04-30 14:19:15.000000 zadu-0.0.1/src/zadu.egg-info/top_level.txt
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:30:59.173587 zadu-0.0.2/
+-rw-rw-r--   0 hj        (1010) hj        (1010)     5658 2023-04-30 14:30:59.173587 zadu-0.0.2/PKG-INFO
+-rw-rw-r--   0 hj        (1010) hj        (1010)     4235 2023-04-30 13:42:58.000000 zadu-0.0.2/README.md
+-rw-rw-r--   0 hj        (1010) hj        (1010)       38 2023-04-30 14:30:59.173587 zadu-0.0.2/setup.cfg
+-rw-rw-r--   0 hj        (1010) hj        (1010)      773 2023-04-30 14:30:31.000000 zadu-0.0.2/setup.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:30:59.173587 zadu-0.0.2/src/
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:30:59.173587 zadu-0.0.2/src/zadu.egg-info/
+-rw-rw-r--   0 hj        (1010) hj        (1010)     5658 2023-04-30 14:30:59.000000 zadu-0.0.2/src/zadu.egg-info/PKG-INFO
+-rw-rw-r--   0 hj        (1010) hj        (1010)      177 2023-04-30 14:30:59.000000 zadu-0.0.2/src/zadu.egg-info/SOURCES.txt
+-rw-rw-r--   0 hj        (1010) hj        (1010)        1 2023-04-30 14:30:59.000000 zadu-0.0.2/src/zadu.egg-info/dependency_links.txt
+-rw-rw-r--   0 hj        (1010) hj        (1010)       40 2023-04-30 14:30:59.000000 zadu-0.0.2/src/zadu.egg-info/requires.txt
+-rw-rw-r--   0 hj        (1010) hj        (1010)        1 2023-04-30 14:30:59.000000 zadu-0.0.2/src/zadu.egg-info/top_level.txt
```

### Comparing `zadu-0.0.1/PKG-INFO` & `zadu-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zadu
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings
 Home-page: https://github.com/hj-n/zadu
 Author: Hyeon Jeon
 Author-email: hj@hcil.snu.ac.kr
 License: UNKNOWN
 Description: # ZADU: A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings
```

### Comparing `zadu-0.0.1/README.md` & `zadu-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `zadu-0.0.1/setup.py` & `zadu-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="zadu",
-	version="0.0.1",
+	version="0.0.2",
 	author="Hyeon Jeon",
 	author_email="hj@hcil.snu.ac.kr",
 	description="A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/hj-n/zadu",
 	classifiers=[
```

### Comparing `zadu-0.0.1/src/zadu.egg-info/PKG-INFO` & `zadu-0.0.2/src/zadu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zadu
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings
 Home-page: https://github.com/hj-n/zadu
 Author: Hyeon Jeon
 Author-email: hj@hcil.snu.ac.kr
 License: UNKNOWN
 Description: # ZADU: A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings
```

