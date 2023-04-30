# Comparing `tmp/zadu-0.0.2.tar.gz` & `tmp/zadu-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zadu-0.0.2.tar", last modified: Sun Apr 30 14:30:59 2023, max compression
+gzip compressed data, was "dist/zadu-0.0.4.tar", last modified: Sun Apr 30 14:42:01 2023, max compression
```

## Comparing `zadu-0.0.2.tar` & `zadu-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:30:59.173587 zadu-0.0.2/
--rw-rw-r--   0 hj        (1010) hj        (1010)     5658 2023-04-30 14:30:59.173587 zadu-0.0.2/PKG-INFO
--rw-rw-r--   0 hj        (1010) hj        (1010)     4235 2023-04-30 13:42:58.000000 zadu-0.0.2/README.md
--rw-rw-r--   0 hj        (1010) hj        (1010)       38 2023-04-30 14:30:59.173587 zadu-0.0.2/setup.cfg
--rw-rw-r--   0 hj        (1010) hj        (1010)      773 2023-04-30 14:30:31.000000 zadu-0.0.2/setup.py
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:30:59.173587 zadu-0.0.2/src/
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:30:59.173587 zadu-0.0.2/src/zadu.egg-info/
--rw-rw-r--   0 hj        (1010) hj        (1010)     5658 2023-04-30 14:30:59.000000 zadu-0.0.2/src/zadu.egg-info/PKG-INFO
--rw-rw-r--   0 hj        (1010) hj        (1010)      177 2023-04-30 14:30:59.000000 zadu-0.0.2/src/zadu.egg-info/SOURCES.txt
--rw-rw-r--   0 hj        (1010) hj        (1010)        1 2023-04-30 14:30:59.000000 zadu-0.0.2/src/zadu.egg-info/dependency_links.txt
--rw-rw-r--   0 hj        (1010) hj        (1010)       40 2023-04-30 14:30:59.000000 zadu-0.0.2/src/zadu.egg-info/requires.txt
--rw-rw-r--   0 hj        (1010) hj        (1010)        1 2023-04-30 14:30:59.000000 zadu-0.0.2/src/zadu.egg-info/top_level.txt
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:42:01.175642 zadu-0.0.4/
+-rw-rw-r--   0 hj        (1010) hj        (1010)     5658 2023-04-30 14:42:01.175642 zadu-0.0.4/PKG-INFO
+-rw-rw-r--   0 hj        (1010) hj        (1010)     4235 2023-04-30 13:42:58.000000 zadu-0.0.4/README.md
+-rw-rw-r--   0 hj        (1010) hj        (1010)       38 2023-04-30 14:42:01.175642 zadu-0.0.4/setup.cfg
+-rw-rw-r--   0 hj        (1010) hj        (1010)      801 2023-04-30 14:41:51.000000 zadu-0.0.4/setup.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:42:01.175642 zadu-0.0.4/src/
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:42:01.175642 zadu-0.0.4/src/zadu/
+-rw-rw-r--   0 hj        (1010) hj        (1010)     6738 2023-04-30 14:16:39.000000 zadu-0.0.4/src/zadu/zadu.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:42:01.175642 zadu-0.0.4/src/zadu.egg-info/
+-rw-rw-r--   0 hj        (1010) hj        (1010)     5658 2023-04-30 14:42:01.000000 zadu-0.0.4/src/zadu.egg-info/PKG-INFO
+-rw-rw-r--   0 hj        (1010) hj        (1010)      241 2023-04-30 14:42:01.000000 zadu-0.0.4/src/zadu.egg-info/SOURCES.txt
+-rw-rw-r--   0 hj        (1010) hj        (1010)        1 2023-04-30 14:42:01.000000 zadu-0.0.4/src/zadu.egg-info/dependency_links.txt
+-rw-rw-r--   0 hj        (1010) hj        (1010)       40 2023-04-30 14:42:01.000000 zadu-0.0.4/src/zadu.egg-info/requires.txt
+-rw-rw-r--   0 hj        (1010) hj        (1010)       13 2023-04-30 14:42:01.000000 zadu-0.0.4/src/zadu.egg-info/top_level.txt
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:42:01.175642 zadu-0.0.4/src/zaduvis/
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1629 2023-04-08 07:45:55.000000 zadu-0.0.4/src/zaduvis/colormap.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1798 2023-04-09 02:48:07.000000 zadu-0.0.4/src/zaduvis/zaduvis.py
```

### Comparing `zadu-0.0.2/PKG-INFO` & `zadu-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zadu
-Version: 0.0.2
+Version: 0.0.4
 Summary: A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings
 Home-page: https://github.com/hj-n/zadu
 Author: Hyeon Jeon
 Author-email: hj@hcil.snu.ac.kr
 License: UNKNOWN
 Description: # ZADU: A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings
```

### Comparing `zadu-0.0.2/README.md` & `zadu-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `zadu-0.0.2/setup.py` & `zadu-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
 	long_description = fh.read()
 
+print(setuptools.find_packages(where="src"))
+
 setuptools.setup(
 	name="zadu",
-	version="0.0.2",
+	version="0.0.4",
 	author="Hyeon Jeon",
 	author_email="hj@hcil.snu.ac.kr",
 	description="A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/hj-n/zadu",
 	classifiers=[
@@ -21,10 +23,10 @@
 		"numpy",
 		"scikit-learn",
 		"scipy",
 		"snc",
 		"matplotlib"
 	],
 	package_dir={"": "src"},
-	packages=setuptools.find_packages(where="src"),
+	packages=["zadu", "zaduvis"],
 	python_requires=">=3.9.0",
 )
```

### Comparing `zadu-0.0.2/src/zadu.egg-info/PKG-INFO` & `zadu-0.0.4/src/zadu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zadu
-Version: 0.0.2
+Version: 0.0.4
 Summary: A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings
 Home-page: https://github.com/hj-n/zadu
 Author: Hyeon Jeon
 Author-email: hj@hcil.snu.ac.kr
 License: UNKNOWN
 Description: # ZADU: A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings
```

