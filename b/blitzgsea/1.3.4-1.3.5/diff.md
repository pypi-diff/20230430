# Comparing `tmp/blitzgsea-1.3.4.tar.gz` & `tmp/blitzgsea-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blitzgsea-1.3.4.tar", last modified: Sun Apr 30 01:06:55 2023, max compression
+gzip compressed data, was "blitzgsea-1.3.5.tar", last modified: Sun Apr 30 01:10:30 2023, max compression
```

## Comparing `blitzgsea-1.3.4.tar` & `blitzgsea-1.3.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-04-30 01:06:55.149342 blitzgsea-1.3.4/
--rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-07-24 15:38:47.000000 blitzgsea-1.3.4/LICENSE
--rw-r--r--   0 maayanlab   (501) staff       (20)    11988 2023-04-30 01:06:55.149126 blitzgsea-1.3.4/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)    11430 2023-04-30 01:04:00.000000 blitzgsea-1.3.4/README.md
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-04-30 01:06:55.148006 blitzgsea-1.3.4/blitzgsea/
--rw-r--r--   0 maayanlab   (501) staff       (20)    15508 2023-04-29 01:49:21.000000 blitzgsea-1.3.4/blitzgsea/__init__.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     2768 2023-04-28 02:23:48.000000 blitzgsea-1.3.4/blitzgsea/enrichr.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     7316 2022-07-24 15:38:47.000000 blitzgsea-1.3.4/blitzgsea/plot.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     2594 2022-07-24 15:38:47.000000 blitzgsea-1.3.4/blitzgsea/shuffle.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-04-30 01:06:55.148881 blitzgsea-1.3.4/blitzgsea.egg-info/
--rw-r--r--   0 maayanlab   (501) staff       (20)    11988 2023-04-30 01:06:55.000000 blitzgsea-1.3.4/blitzgsea.egg-info/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)      272 2023-04-30 01:06:55.000000 blitzgsea-1.3.4/blitzgsea.egg-info/SOURCES.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-04-30 01:06:55.000000 blitzgsea-1.3.4/blitzgsea.egg-info/dependency_links.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)      128 2023-04-30 01:06:55.000000 blitzgsea-1.3.4/blitzgsea.egg-info/requires.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)       10 2023-04-30 01:06:55.000000 blitzgsea-1.3.4/blitzgsea.egg-info/top_level.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-04-30 01:06:55.149398 blitzgsea-1.3.4/setup.cfg
--rw-r--r--   0 maayanlab   (501) staff       (20)     1083 2023-04-30 00:23:09.000000 blitzgsea-1.3.4/setup.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-04-30 01:10:30.274576 blitzgsea-1.3.5/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-07-24 15:38:47.000000 blitzgsea-1.3.5/LICENSE
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11987 2023-04-30 01:10:30.273890 blitzgsea-1.3.5/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11429 2023-04-30 01:10:11.000000 blitzgsea-1.3.5/README.md
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-04-30 01:10:30.272509 blitzgsea-1.3.5/blitzgsea/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    15508 2023-04-29 01:49:21.000000 blitzgsea-1.3.5/blitzgsea/__init__.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2768 2023-04-28 02:23:48.000000 blitzgsea-1.3.5/blitzgsea/enrichr.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     7316 2022-07-24 15:38:47.000000 blitzgsea-1.3.5/blitzgsea/plot.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2594 2022-07-24 15:38:47.000000 blitzgsea-1.3.5/blitzgsea/shuffle.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-04-30 01:10:30.273630 blitzgsea-1.3.5/blitzgsea.egg-info/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11987 2023-04-30 01:10:30.000000 blitzgsea-1.3.5/blitzgsea.egg-info/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)      272 2023-04-30 01:10:30.000000 blitzgsea-1.3.5/blitzgsea.egg-info/SOURCES.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-04-30 01:10:30.000000 blitzgsea-1.3.5/blitzgsea.egg-info/dependency_links.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)      128 2023-04-30 01:10:30.000000 blitzgsea-1.3.5/blitzgsea.egg-info/requires.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)       10 2023-04-30 01:10:30.000000 blitzgsea-1.3.5/blitzgsea.egg-info/top_level.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-04-30 01:10:30.274642 blitzgsea-1.3.5/setup.cfg
+-rw-r--r--   0 maayanlab   (501) staff       (20)     1083 2023-04-30 01:09:57.000000 blitzgsea-1.3.5/setup.py
```

### Comparing `blitzgsea-1.3.4/LICENSE` & `blitzgsea-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `blitzgsea-1.3.4/PKG-INFO` & `blitzgsea-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: blitzgsea
-Version: 1.3.4
+Version: 1.3.5
 Summary: Package for fast calculation of GSEA similar to prerank using gamma distribution approximation.
 Home-page: https://github.com/maayanlab/blitzgsea
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img title="a title" alt="blitzGSEA" src="https://github.com/MaayanLab/blitzgsea/blob/main/icon/bgsea_small.png" width=200>
+<img title="a title" alt="blitzGSEA" src="https://github.com/MaayanLab/blitzgsea/raw/main/icon/bgsea_small.png" width=200>
 
 [Installation](#installation) | [Example](#python-example) | [Optional Parameters](#optional-parameters) | [Speed-up](#speeding-up-enrichment-calculations) | [Plotting](#plotting-enrichment-results) | [Attribution](#attribution) | [References](#references)
 
 # blitzGSEA Introduction
 
 This Python package provides a computationally performant <b>G</b>ene <b>S</b>et <b>E</b>nrichment <b>A</b>nalysis (GSEA) implementation of the pre-rank algorithm [1]. GSEApy was used as the reference for the running sum and enrichment score calculation [2]. The algorithm estimates the enrichment score (ES) distribution of the null model by fitting data to gamma distibutions instead of calculating permutations for each gene set. blitzGSEA calculates p-values with much higher accuracy than other reference implementations available in Python.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blitzgsea Version: 1.3.4 Summary: Package for fast
+Metadata-Version: 2.1 Name: blitzgsea Version: 1.3.5 Summary: Package for fast
 calculation of GSEA similar to prerank using gamma distribution approximation.
 Home-page: https://github.com/maayanlab/blitzgsea Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu License: UNKNOWN Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE [blitzGSEA] [Installation](#installation) | [Example]
```

### Comparing `blitzgsea-1.3.4/README.md` & `blitzgsea-1.3.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img title="a title" alt="blitzGSEA" src="https://github.com/MaayanLab/blitzgsea/blob/main/icon/bgsea_small.png" width=200>
+<img title="a title" alt="blitzGSEA" src="https://github.com/MaayanLab/blitzgsea/raw/main/icon/bgsea_small.png" width=200>
 
 [Installation](#installation) | [Example](#python-example) | [Optional Parameters](#optional-parameters) | [Speed-up](#speeding-up-enrichment-calculations) | [Plotting](#plotting-enrichment-results) | [Attribution](#attribution) | [References](#references)
 
 # blitzGSEA Introduction
 
 This Python package provides a computationally performant <b>G</b>ene <b>S</b>et <b>E</b>nrichment <b>A</b>nalysis (GSEA) implementation of the pre-rank algorithm [1]. GSEApy was used as the reference for the running sum and enrichment score calculation [2]. The algorithm estimates the enrichment score (ES) distribution of the null model by fitting data to gamma distibutions instead of calculating permutations for each gene set. blitzGSEA calculates p-values with much higher accuracy than other reference implementations available in Python.
```

### Comparing `blitzgsea-1.3.4/blitzgsea/__init__.py` & `blitzgsea-1.3.5/blitzgsea/__init__.py`

 * *Files identical despite different names*

### Comparing `blitzgsea-1.3.4/blitzgsea/enrichr.py` & `blitzgsea-1.3.5/blitzgsea/enrichr.py`

 * *Files identical despite different names*

### Comparing `blitzgsea-1.3.4/blitzgsea/plot.py` & `blitzgsea-1.3.5/blitzgsea/plot.py`

 * *Files identical despite different names*

### Comparing `blitzgsea-1.3.4/blitzgsea/shuffle.py` & `blitzgsea-1.3.5/blitzgsea/shuffle.py`

 * *Files identical despite different names*

### Comparing `blitzgsea-1.3.4/blitzgsea.egg-info/PKG-INFO` & `blitzgsea-1.3.5/blitzgsea.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: blitzgsea
-Version: 1.3.4
+Version: 1.3.5
 Summary: Package for fast calculation of GSEA similar to prerank using gamma distribution approximation.
 Home-page: https://github.com/maayanlab/blitzgsea
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img title="a title" alt="blitzGSEA" src="https://github.com/MaayanLab/blitzgsea/blob/main/icon/bgsea_small.png" width=200>
+<img title="a title" alt="blitzGSEA" src="https://github.com/MaayanLab/blitzgsea/raw/main/icon/bgsea_small.png" width=200>
 
 [Installation](#installation) | [Example](#python-example) | [Optional Parameters](#optional-parameters) | [Speed-up](#speeding-up-enrichment-calculations) | [Plotting](#plotting-enrichment-results) | [Attribution](#attribution) | [References](#references)
 
 # blitzGSEA Introduction
 
 This Python package provides a computationally performant <b>G</b>ene <b>S</b>et <b>E</b>nrichment <b>A</b>nalysis (GSEA) implementation of the pre-rank algorithm [1]. GSEApy was used as the reference for the running sum and enrichment score calculation [2]. The algorithm estimates the enrichment score (ES) distribution of the null model by fitting data to gamma distibutions instead of calculating permutations for each gene set. blitzGSEA calculates p-values with much higher accuracy than other reference implementations available in Python.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blitzgsea Version: 1.3.4 Summary: Package for fast
+Metadata-Version: 2.1 Name: blitzgsea Version: 1.3.5 Summary: Package for fast
 calculation of GSEA similar to prerank using gamma distribution approximation.
 Home-page: https://github.com/maayanlab/blitzgsea Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu License: UNKNOWN Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE [blitzGSEA] [Installation](#installation) | [Example]
```

### Comparing `blitzgsea-1.3.4/setup.py` & `blitzgsea-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="blitzgsea",
-    version="1.3.4",
+    version="1.3.5",
     author="Alexander Lachmann",
     author_email="alexander.lachmann@mssm.edu",
     description="Package for fast calculation of GSEA similar to prerank using gamma distribution approximation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/maayanlab/blitzgsea",
     packages=setuptools.find_packages(),
```

