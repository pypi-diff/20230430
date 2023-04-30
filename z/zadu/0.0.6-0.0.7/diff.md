# Comparing `tmp/zadu-0.0.6.tar.gz` & `tmp/zadu-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zadu-0.0.6.tar", last modified: Sun Apr 30 14:55:41 2023, max compression
+gzip compressed data, was "dist/zadu-0.0.7.tar", last modified: Sun Apr 30 16:44:23 2023, max compression
```

## Comparing `zadu-0.0.6.tar` & `zadu-0.0.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:55:41.144671 zadu-0.0.6/
--rw-rw-r--   0 hj        (1010) hj        (1010)     5658 2023-04-30 14:55:41.144671 zadu-0.0.6/PKG-INFO
--rw-rw-r--   0 hj        (1010) hj        (1010)     4235 2023-04-30 13:42:58.000000 zadu-0.0.6/README.md
--rw-rw-r--   0 hj        (1010) hj        (1010)       38 2023-04-30 14:55:41.144671 zadu-0.0.6/setup.cfg
--rw-rw-r--   0 hj        (1010) hj        (1010)      841 2023-04-30 14:55:35.000000 zadu-0.0.6/setup.py
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:55:41.140671 zadu-0.0.6/src/
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:55:41.144671 zadu-0.0.6/src/zadu/
--rw-rw-r--   0 hj        (1010) hj        (1010)        0 2023-04-30 14:50:34.000000 zadu-0.0.6/src/zadu/__init__.py
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:55:41.144671 zadu-0.0.6/src/zadu/measures/
--rw-rw-r--   0 hj        (1010) hj        (1010)      495 2023-04-30 14:16:48.000000 zadu-0.0.6/src/zadu/measures/__init__.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     2685 2023-04-13 09:45:13.000000 zadu-0.0.6/src/zadu/measures/class_aware_trustworthiness_continuity.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1438 2023-04-13 09:45:25.000000 zadu-0.0.6/src/zadu/measures/clustering_and_external_validation_measure.py
--rw-rw-r--   0 hj        (1010) hj        (1010)      920 2023-04-13 09:45:30.000000 zadu-0.0.6/src/zadu/measures/distance_consistency.py
--rw-rw-r--   0 hj        (1010) hj        (1010)      867 2023-04-13 09:45:35.000000 zadu-0.0.6/src/zadu/measures/distance_to_measure.py
--rw-rw-r--   0 hj        (1010) hj        (1010)      715 2023-04-13 09:45:42.000000 zadu-0.0.6/src/zadu/measures/internal_validation_measure.py
--rw-rw-r--   0 hj        (1010) hj        (1010)      909 2023-04-13 09:45:48.000000 zadu-0.0.6/src/zadu/measures/kl_divergence.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1211 2023-04-13 09:45:53.000000 zadu-0.0.6/src/zadu/measures/local_continuity_meta_criteria.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     2203 2023-04-13 09:45:59.000000 zadu-0.0.6/src/zadu/measures/mean_relative_rank_error.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1107 2023-04-13 09:46:04.000000 zadu-0.0.6/src/zadu/measures/neighbor_dissimilarity.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1025 2023-04-13 09:46:10.000000 zadu-0.0.6/src/zadu/measures/neighborhood_hit.py
--rw-rw-r--   0 hj        (1010) hj        (1010)      775 2023-04-13 09:46:15.000000 zadu-0.0.6/src/zadu/measures/pearson_r.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1127 2023-04-30 14:11:34.000000 zadu-0.0.6/src/zadu/measures/procrustes.py
--rw-rw-r--   0 hj        (1010) hj        (1010)      795 2023-04-13 09:46:20.000000 zadu-0.0.6/src/zadu/measures/spearman_rho.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1590 2023-04-24 10:19:02.000000 zadu-0.0.6/src/zadu/measures/steadiness_cohesiveness.py
--rw-rw-r--   0 hj        (1010) hj        (1010)      808 2023-04-14 20:28:49.000000 zadu-0.0.6/src/zadu/measures/stress.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1581 2023-04-30 13:46:46.000000 zadu-0.0.6/src/zadu/measures/topographic_product.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     2154 2023-04-14 20:05:24.000000 zadu-0.0.6/src/zadu/measures/trustworthiness_continuity.py
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:55:41.144671 zadu-0.0.6/src/zadu/measures/utils/
--rw-rw-r--   0 hj        (1010) hj        (1010)        0 2023-04-06 03:59:50.000000 zadu-0.0.6/src/zadu/measures/utils/__init__.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     3200 2023-04-15 02:30:27.000000 zadu-0.0.6/src/zadu/measures/utils/knn.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1166 2023-04-06 15:35:44.000000 zadu-0.0.6/src/zadu/measures/utils/pairwise_dist.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     6738 2023-04-30 14:16:39.000000 zadu-0.0.6/src/zadu/zadu.py
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:55:41.144671 zadu-0.0.6/src/zadu.egg-info/
--rw-rw-r--   0 hj        (1010) hj        (1010)     5658 2023-04-30 14:55:41.000000 zadu-0.0.6/src/zadu.egg-info/PKG-INFO
--rw-rw-r--   0 hj        (1010) hj        (1010)     1154 2023-04-30 14:55:41.000000 zadu-0.0.6/src/zadu.egg-info/SOURCES.txt
--rw-rw-r--   0 hj        (1010) hj        (1010)        1 2023-04-30 14:55:41.000000 zadu-0.0.6/src/zadu.egg-info/dependency_links.txt
--rw-rw-r--   0 hj        (1010) hj        (1010)       40 2023-04-30 14:55:41.000000 zadu-0.0.6/src/zadu.egg-info/requires.txt
--rw-rw-r--   0 hj        (1010) hj        (1010)       13 2023-04-30 14:55:41.000000 zadu-0.0.6/src/zadu.egg-info/top_level.txt
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 14:55:41.144671 zadu-0.0.6/src/zaduvis/
--rw-rw-r--   0 hj        (1010) hj        (1010)        0 2023-04-30 14:50:47.000000 zadu-0.0.6/src/zaduvis/__init__.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1629 2023-04-08 07:45:55.000000 zadu-0.0.6/src/zaduvis/colormap.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1798 2023-04-09 02:48:07.000000 zadu-0.0.6/src/zaduvis/zaduvis.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 16:44:23.079130 zadu-0.0.7/
+-rw-rw-r--   0 hj        (1010) hj        (1010)     5658 2023-04-30 16:44:23.079130 zadu-0.0.7/PKG-INFO
+-rw-rw-r--   0 hj        (1010) hj        (1010)     4235 2023-04-30 13:42:58.000000 zadu-0.0.7/README.md
+-rw-rw-r--   0 hj        (1010) hj        (1010)       38 2023-04-30 16:44:23.079130 zadu-0.0.7/setup.cfg
+-rw-rw-r--   0 hj        (1010) hj        (1010)      856 2023-04-30 16:43:46.000000 zadu-0.0.7/setup.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 16:44:23.079130 zadu-0.0.7/src/
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 16:44:23.079130 zadu-0.0.7/src/zadu/
+-rw-rw-r--   0 hj        (1010) hj        (1010)        0 2023-04-30 14:50:34.000000 zadu-0.0.7/src/zadu/__init__.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 16:44:23.079130 zadu-0.0.7/src/zadu/measures/
+-rw-rw-r--   0 hj        (1010) hj        (1010)      495 2023-04-30 14:16:48.000000 zadu-0.0.7/src/zadu/measures/__init__.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     2685 2023-04-13 09:45:13.000000 zadu-0.0.7/src/zadu/measures/class_aware_trustworthiness_continuity.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1438 2023-04-13 09:45:25.000000 zadu-0.0.7/src/zadu/measures/clustering_and_external_validation_measure.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)      920 2023-04-13 09:45:30.000000 zadu-0.0.7/src/zadu/measures/distance_consistency.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)      867 2023-04-13 09:45:35.000000 zadu-0.0.7/src/zadu/measures/distance_to_measure.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)      715 2023-04-13 09:45:42.000000 zadu-0.0.7/src/zadu/measures/internal_validation_measure.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)      909 2023-04-13 09:45:48.000000 zadu-0.0.7/src/zadu/measures/kl_divergence.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1211 2023-04-13 09:45:53.000000 zadu-0.0.7/src/zadu/measures/local_continuity_meta_criteria.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     2203 2023-04-13 09:45:59.000000 zadu-0.0.7/src/zadu/measures/mean_relative_rank_error.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1107 2023-04-13 09:46:04.000000 zadu-0.0.7/src/zadu/measures/neighbor_dissimilarity.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1025 2023-04-13 09:46:10.000000 zadu-0.0.7/src/zadu/measures/neighborhood_hit.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)      775 2023-04-13 09:46:15.000000 zadu-0.0.7/src/zadu/measures/pearson_r.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1127 2023-04-30 14:11:34.000000 zadu-0.0.7/src/zadu/measures/procrustes.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)      795 2023-04-13 09:46:20.000000 zadu-0.0.7/src/zadu/measures/spearman_rho.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1590 2023-04-24 10:19:02.000000 zadu-0.0.7/src/zadu/measures/steadiness_cohesiveness.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)      808 2023-04-14 20:28:49.000000 zadu-0.0.7/src/zadu/measures/stress.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1581 2023-04-30 13:46:46.000000 zadu-0.0.7/src/zadu/measures/topographic_product.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     2154 2023-04-14 20:05:24.000000 zadu-0.0.7/src/zadu/measures/trustworthiness_continuity.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 16:44:23.079130 zadu-0.0.7/src/zadu/measures/utils/
+-rw-rw-r--   0 hj        (1010) hj        (1010)        0 2023-04-06 03:59:50.000000 zadu-0.0.7/src/zadu/measures/utils/__init__.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     3200 2023-04-15 02:30:27.000000 zadu-0.0.7/src/zadu/measures/utils/knn.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1166 2023-04-06 15:35:44.000000 zadu-0.0.7/src/zadu/measures/utils/pairwise_dist.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     6738 2023-04-30 14:16:39.000000 zadu-0.0.7/src/zadu/zadu.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 16:44:23.079130 zadu-0.0.7/src/zadu.egg-info/
+-rw-rw-r--   0 hj        (1010) hj        (1010)     5658 2023-04-30 16:44:22.000000 zadu-0.0.7/src/zadu.egg-info/PKG-INFO
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1154 2023-04-30 16:44:22.000000 zadu-0.0.7/src/zadu.egg-info/SOURCES.txt
+-rw-rw-r--   0 hj        (1010) hj        (1010)        1 2023-04-30 16:44:22.000000 zadu-0.0.7/src/zadu.egg-info/dependency_links.txt
+-rw-rw-r--   0 hj        (1010) hj        (1010)       50 2023-04-30 16:44:22.000000 zadu-0.0.7/src/zadu.egg-info/requires.txt
+-rw-rw-r--   0 hj        (1010) hj        (1010)       13 2023-04-30 16:44:22.000000 zadu-0.0.7/src/zadu.egg-info/top_level.txt
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-30 16:44:23.079130 zadu-0.0.7/src/zaduvis/
+-rw-rw-r--   0 hj        (1010) hj        (1010)        0 2023-04-30 14:50:47.000000 zadu-0.0.7/src/zaduvis/__init__.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1629 2023-04-08 07:45:55.000000 zadu-0.0.7/src/zaduvis/colormap.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1798 2023-04-09 02:48:07.000000 zadu-0.0.7/src/zaduvis/zaduvis.py
```

### Comparing `zadu-0.0.6/PKG-INFO` & `zadu-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zadu
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings
 Home-page: https://github.com/hj-n/zadu
 Author: Hyeon Jeon
 Author-email: hj@hcil.snu.ac.kr
 License: UNKNOWN
 Description: # ZADU: A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings
```

### Comparing `zadu-0.0.6/README.md` & `zadu-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/setup.py` & `zadu-0.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
 	long_description = fh.read()
 
 print(setuptools.find_packages(where="src"))
 
 setuptools.setup(
 	name="zadu",
-	version="0.0.6",
+	version="0.0.7",
 	author="Hyeon Jeon",
 	author_email="hj@hcil.snu.ac.kr",
 	description="A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/hj-n/zadu",
 	classifiers=[
@@ -20,13 +20,14 @@
 			"Operating System :: OS Independent",
 	],
 	install_requires=[
 		"numpy",
 		"scikit-learn",
 		"scipy",
 		"snc",
-		"matplotlib"
+		"matplotlib",
+		"faiss-cpu"
 	],
 	package_dir={"": "src"},
 	packages=["zadu", "zaduvis", "zadu.measures", "zadu.measures.utils"],
 	python_requires=">=3.9.0",
 )
```

### Comparing `zadu-0.0.6/src/zadu/measures/class_aware_trustworthiness_continuity.py` & `zadu-0.0.7/src/zadu/measures/class_aware_trustworthiness_continuity.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/measures/clustering_and_external_validation_measure.py` & `zadu-0.0.7/src/zadu/measures/clustering_and_external_validation_measure.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/measures/distance_consistency.py` & `zadu-0.0.7/src/zadu/measures/distance_consistency.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/measures/distance_to_measure.py` & `zadu-0.0.7/src/zadu/measures/distance_to_measure.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/measures/internal_validation_measure.py` & `zadu-0.0.7/src/zadu/measures/internal_validation_measure.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/measures/kl_divergence.py` & `zadu-0.0.7/src/zadu/measures/kl_divergence.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/measures/local_continuity_meta_criteria.py` & `zadu-0.0.7/src/zadu/measures/local_continuity_meta_criteria.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/measures/mean_relative_rank_error.py` & `zadu-0.0.7/src/zadu/measures/mean_relative_rank_error.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/measures/neighbor_dissimilarity.py` & `zadu-0.0.7/src/zadu/measures/neighbor_dissimilarity.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/measures/neighborhood_hit.py` & `zadu-0.0.7/src/zadu/measures/neighborhood_hit.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/measures/pearson_r.py` & `zadu-0.0.7/src/zadu/measures/pearson_r.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/measures/procrustes.py` & `zadu-0.0.7/src/zadu/measures/procrustes.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/measures/spearman_rho.py` & `zadu-0.0.7/src/zadu/measures/spearman_rho.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/measures/steadiness_cohesiveness.py` & `zadu-0.0.7/src/zadu/measures/steadiness_cohesiveness.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/measures/stress.py` & `zadu-0.0.7/src/zadu/measures/stress.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/measures/topographic_product.py` & `zadu-0.0.7/src/zadu/measures/topographic_product.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/measures/trustworthiness_continuity.py` & `zadu-0.0.7/src/zadu/measures/trustworthiness_continuity.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/measures/utils/knn.py` & `zadu-0.0.7/src/zadu/measures/utils/knn.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/measures/utils/pairwise_dist.py` & `zadu-0.0.7/src/zadu/measures/utils/pairwise_dist.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu/zadu.py` & `zadu-0.0.7/src/zadu/zadu.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zadu.egg-info/PKG-INFO` & `zadu-0.0.7/src/zadu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zadu
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings
 Home-page: https://github.com/hj-n/zadu
 Author: Hyeon Jeon
 Author-email: hj@hcil.snu.ac.kr
 License: UNKNOWN
 Description: # ZADU: A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings
```

### Comparing `zadu-0.0.6/src/zadu.egg-info/SOURCES.txt` & `zadu-0.0.7/src/zadu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zaduvis/colormap.py` & `zadu-0.0.7/src/zaduvis/colormap.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.6/src/zaduvis/zaduvis.py` & `zadu-0.0.7/src/zaduvis/zaduvis.py`

 * *Files identical despite different names*

