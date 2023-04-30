# Comparing `tmp/pyhrp-0.0.7.tar.gz` & `tmp/pyhrp-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyhrp-0.0.7.tar", last modified: Thu Apr 30 19:20:10 2020, max compression
+gzip compressed data, was "dist/pyhrp-0.0.8.tar", last modified: Fri May 29 18:56:05 2020, max compression
```

## Comparing `pyhrp-0.0.7.tar` & `pyhrp-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 tschm     (1000) tschm     (1002)        0 2020-04-30 19:20:10.000000 pyhrp-0.0.7/
--rwxrwxr-x   0 tschm     (1000) tschm     (1002)     1083 2020-04-22 20:14:34.000000 pyhrp-0.0.7/LICENSE.txt
-drwxrwxr-x   0 tschm     (1000) tschm     (1002)        0 2020-04-30 19:20:10.000000 pyhrp-0.0.7/test/
--rw-rw-r--   0 tschm     (1000) tschm     (1002)      553 2020-04-30 07:17:46.000000 pyhrp-0.0.7/test/test_marcos.py
--rw-rw-r--   0 tschm     (1000) tschm     (1002)     2524 2020-04-29 08:41:32.000000 pyhrp-0.0.7/test/test_cluster.py
--rw-rw-r--   0 tschm     (1000) tschm     (1002)     3166 2020-04-30 07:19:52.000000 pyhrp-0.0.7/test/test_hrp.py
--rw-rw-r--   0 tschm     (1000) tschm     (1002)      461 2020-04-30 07:46:57.000000 pyhrp-0.0.7/test/test_obsolete.py
--rw-rw-r--   0 tschm     (1000) tschm     (1002)     1332 2020-04-30 07:41:05.000000 pyhrp-0.0.7/README.md
-drwxrwxr-x   0 tschm     (1000) tschm     (1002)        0 2020-04-30 19:20:10.000000 pyhrp-0.0.7/pyhrp.egg-info/
--rw-rw-r--   0 tschm     (1000) tschm     (1002)       38 2020-04-30 19:20:09.000000 pyhrp-0.0.7/pyhrp.egg-info/requires.txt
--rw-rw-r--   0 tschm     (1000) tschm     (1002)      373 2020-04-30 19:20:09.000000 pyhrp-0.0.7/pyhrp.egg-info/SOURCES.txt
--rw-rw-r--   0 tschm     (1000) tschm     (1002)     2028 2020-04-30 19:20:09.000000 pyhrp-0.0.7/pyhrp.egg-info/PKG-INFO
--rw-rw-r--   0 tschm     (1000) tschm     (1002)        6 2020-04-30 19:20:09.000000 pyhrp-0.0.7/pyhrp.egg-info/top_level.txt
--rw-rw-r--   0 tschm     (1000) tschm     (1002)        1 2020-04-30 19:20:09.000000 pyhrp-0.0.7/pyhrp.egg-info/dependency_links.txt
--rw-rw-r--   0 tschm     (1000) tschm     (1002)      107 2020-04-30 19:20:10.000000 pyhrp-0.0.7/setup.cfg
--rw-rw-r--   0 tschm     (1000) tschm     (1002)     2028 2020-04-30 19:20:10.000000 pyhrp-0.0.7/PKG-INFO
-drwxrwxr-x   0 tschm     (1000) tschm     (1002)        0 2020-04-30 19:20:10.000000 pyhrp-0.0.7/pyhrp/
--rw-rw-r--   0 tschm     (1000) tschm     (1002)     2490 2020-04-29 11:16:26.000000 pyhrp-0.0.7/pyhrp/cluster.py
--rw-rw-r--   0 tschm     (1000) tschm     (1002)      237 2020-04-27 13:52:57.000000 pyhrp-0.0.7/pyhrp/graph.py
--rwxrwxr-x   0 tschm     (1000) tschm     (1002)      126 2020-04-30 18:34:50.000000 pyhrp-0.0.7/pyhrp/__init__.py
--rw-rw-r--   0 tschm     (1000) tschm     (1002)     2532 2020-04-30 07:53:05.000000 pyhrp-0.0.7/pyhrp/obsolete.py
--rw-rw-r--   0 tschm     (1000) tschm     (1002)     2447 2020-04-30 07:55:52.000000 pyhrp-0.0.7/pyhrp/hrp.py
--rw-rw-r--   0 tschm     (1000) tschm     (1002)     1699 2020-04-30 07:41:05.000000 pyhrp-0.0.7/pyhrp/marcos.py
--rw-rw-r--   0 tschm     (1000) tschm     (1002)      721 2020-04-28 14:07:19.000000 pyhrp-0.0.7/setup.py
--rw-rw-r--   0 tschm     (1000) tschm     (1002)       58 2020-04-22 20:16:51.000000 pyhrp-0.0.7/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-29 18:56:05.000000 pyhrp-0.0.8/
+-rwxr-xr-x   0 root         (0) root         (0)     1083 2020-05-29 18:50:49.000000 pyhrp-0.0.8/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2020-05-29 18:50:49.000000 pyhrp-0.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2028 2020-05-29 18:56:05.000000 pyhrp-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1332 2020-05-29 18:50:49.000000 pyhrp-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-29 18:56:05.000000 pyhrp-0.0.8/pyhrp/
+-rwxr-xr-x   0 root         (0) root         (0)      126 2020-05-29 18:50:49.000000 pyhrp-0.0.8/pyhrp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2473 2020-05-29 18:50:49.000000 pyhrp-0.0.8/pyhrp/cluster.py
+-rw-r--r--   0 root         (0) root         (0)      237 2020-05-29 18:50:49.000000 pyhrp-0.0.8/pyhrp/graph.py
+-rw-r--r--   0 root         (0) root         (0)     2473 2020-05-29 18:50:49.000000 pyhrp-0.0.8/pyhrp/hrp.py
+-rw-r--r--   0 root         (0) root         (0)     1997 2020-05-29 18:50:49.000000 pyhrp-0.0.8/pyhrp/marcos.py
+-rw-r--r--   0 root         (0) root         (0)     2532 2020-05-29 18:50:49.000000 pyhrp-0.0.8/pyhrp/obsolete.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-29 18:56:05.000000 pyhrp-0.0.8/pyhrp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2028 2020-05-29 18:56:05.000000 pyhrp-0.0.8/pyhrp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      373 2020-05-29 18:56:05.000000 pyhrp-0.0.8/pyhrp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-05-29 18:56:05.000000 pyhrp-0.0.8/pyhrp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2020-05-29 18:56:05.000000 pyhrp-0.0.8/pyhrp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2020-05-29 18:56:05.000000 pyhrp-0.0.8/pyhrp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2020-05-29 18:56:05.000000 pyhrp-0.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      721 2020-05-29 18:50:49.000000 pyhrp-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-29 18:56:05.000000 pyhrp-0.0.8/test/
+-rw-r--r--   0 root         (0) root         (0)     2151 2020-05-29 18:50:49.000000 pyhrp-0.0.8/test/test_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     3166 2020-05-29 18:50:49.000000 pyhrp-0.0.8/test/test_hrp.py
+-rw-r--r--   0 root         (0) root         (0)      519 2020-05-29 18:50:49.000000 pyhrp-0.0.8/test/test_marcos.py
+-rw-r--r--   0 root         (0) root         (0)      461 2020-05-29 18:50:49.000000 pyhrp-0.0.8/test/test_obsolete.py
```

### Comparing `pyhrp-0.0.7/LICENSE.txt` & `pyhrp-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyhrp-0.0.7/test/test_marcos.py` & `pyhrp-0.0.8/test/test_marcos.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 
 def test_marcos():
     prices = get_data()
 
     root = marcos(prices=prices)
 
     # uncomment this line if you want generating a new file
-    # root.weights_series(index=list(prices.keys())).to_csv(resource("weights_marcos.csv"), header=False)
+    # root.weights.to_csv(resource("weights_marcos.csv"), header=False)
 
     x = pd.read_csv(resource("weights_marcos.csv"), squeeze=True, index_col=0, header=None)
     x.name = "Weights"
     x.index.name = None
 
     pd.testing.assert_series_equal(x, root.weights, check_exact=False)
```

### Comparing `pyhrp-0.0.7/test/test_cluster.py` & `pyhrp-0.0.8/test/test_cluster.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,34 +4,19 @@
 import pytest
 
 
 def test_cluster_simple():
     c = Cluster(assets={"A": 0.2, "B": 0.8}, variance=1)
 
 
-def test_negative_weight():
-    with pytest.raises(AssertionError):
-        Cluster(assets={"A": -0.2, "B": 0.8}, variance=1)
-
-
-def test_double_column():
-    with pytest.raises(AssertionError):
-        Cluster(assets={"A": 0.5, "A": 0.5}, variance=1)
-
-
 def test_negative_variance():
     with pytest.raises(AssertionError):
         Cluster(assets={"A": -0.2, "B": 0.8}, variance=-1)
 
 
-def test_leverage():
-    with pytest.raises(AssertionError):
-        Cluster(assets={"A": 0.5, "B": 0.9}, variance=1)
-
-
 def test_only_left():
     with pytest.raises(AssertionError):
         Cluster(assets={"A": 0.5, "B": 0.5}, variance=1, left=Cluster(assets={"C": 1.0}, variance=1))
 
 
 def test_wrong_type():
     with pytest.raises(AssertionError):
```

### Comparing `pyhrp-0.0.7/test/test_hrp.py` & `pyhrp-0.0.8/test/test_hrp.py`

 * *Files identical despite different names*

### Comparing `pyhrp-0.0.7/README.md` & `pyhrp-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyhrp-0.0.7/pyhrp.egg-info/PKG-INFO` & `pyhrp-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhrp
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python for Hierarchical Risk Parity
 Home-page: https://github.com/tschm/hrp
 Author: Thomas Schmelzer
 Author-email: thomas.schmelzer@gmail.com
 License: UNKNOWN
 Project-URL: Source Code, https://github.com/tschm/hrp
 Description: # pyhrp
```

### Comparing `pyhrp-0.0.7/PKG-INFO` & `pyhrp-0.0.8/pyhrp.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhrp
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python for Hierarchical Risk Parity
 Home-page: https://github.com/tschm/hrp
 Author: Thomas Schmelzer
 Author-email: thomas.schmelzer@gmail.com
 License: UNKNOWN
 Project-URL: Source Code, https://github.com/tschm/hrp
 Description: # pyhrp
```

### Comparing `pyhrp-0.0.7/pyhrp/cluster.py` & `pyhrp-0.0.8/pyhrp/cluster.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pandas as pd
 
 
-def risk_parity(cluster_left, cluster_right, cov):
+def risk_parity(cluster_left, cluster_right, cov, node=None):
     # combine two clusters
 
     def rp(v_left, v_right):
         """
         Compute the weights for a risk parity portfolio of two assets
         :param v_left: Variance of the "left" portfolio
         :param v_right: Variance of the "right" portfolio
@@ -23,31 +23,27 @@
     assets = {**(alpha_left * cluster_left.weights).to_dict(), **(alpha_right * cluster_right.weights).to_dict()}
 
     w = np.array(list(assets.values()))
     c = cov[assets.keys()].loc[assets.keys()]
 
     var = np.linalg.multi_dot((w, c, w))
 
-    return Cluster(assets=assets, variance=var, left=cluster_left, right=cluster_right)
+    return Cluster(assets=assets, variance=var, left=cluster_left, right=cluster_right, node=node)
 
 
 class Cluster(object):
-    def __init__(self, assets, variance, left=None, right=None):
-        w = np.array(list(assets.values()))
-
-        assert np.all(w > 0)
+    def __init__(self, assets, variance, left=None, right=None, node=None):
         assert variance >= 0
 
-        # test that the weights are close to 1.0
-        assert np.isclose(np.sum(w), 1.0)
-
+        self.__node = node
         self.__assets = assets
         self.__variance = variance
         self.__left = left
         self.__right = right
+        self.__node = node
 
         if left is None:
             # if there is no left, there can't be a right
             assert right is None
         else:
             # left is not None, hence both left and right have to be clusters
             assert isinstance(left, Cluster)
@@ -72,7 +68,11 @@
 
     def is_leaf(self):
         return self.left is None and self.right is None
 
     @property
     def weights(self):
         return pd.Series(self.assets, name="Weights").sort_index()
+
+    @property
+    def node(self):
+        return self.__node
```

### Comparing `pyhrp-0.0.7/pyhrp/obsolete.py` & `pyhrp-0.0.8/pyhrp/obsolete.py`

 * *Files identical despite different names*

### Comparing `pyhrp-0.0.7/pyhrp/hrp.py` & `pyhrp-0.0.8/pyhrp/hrp.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,27 +40,27 @@
     return sch.to_tree(linkage, rd=False)
 
 
 def _hrp(node, cov):
     if node.is_leaf():
         # a node is a leaf if has no further relatives downstream. No leaves, no branches...
         asset = cov.keys().to_list()[node.id]
-        return Cluster(assets={asset: 1.0}, variance=cov[asset][asset])
+        return Cluster(assets={asset: 1.0}, variance=cov[asset][asset], node=node)
     else:
         cluster_left = _hrp(node.left, cov)
         cluster_right = _hrp(node.right, cov)
-        return risk_parity(cluster_left, cluster_right, cov=cov)
+        return risk_parity(cluster_left, cluster_right, cov=cov, node=node)
 
 
 def hrp(prices, node=None, method="single"):
     """
-    Computes the expected variance and the weights for the hierarchical risk parity portfolio
+    Computes the root node for the hierarchical risk parity portfolio
     :param cov: This is the covariance matrix that shall be used
     :param node: Optional. This is the rootnode of the graph describing the dendrogram
-    :return: variance, weights
+    :return: the root cluster of the risk parity portfolio
     """
     returns = prices.pct_change().dropna(axis=0, how="all")
     cov, cor = returns.cov(), returns.corr()
     links = linkage(dist(cor.values), method=method)
     node = node or tree(links)
 
     return _hrp(node, cov)
```

### Comparing `pyhrp-0.0.7/pyhrp/marcos.py` & `pyhrp-0.0.8/pyhrp/marcos.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # the original implementation by Marcos Lopez de Prado is using recursive bisection on a ranked list of columns of the covariance matrix
 # To get to this list Lopez de Prado is using what he calls the matrix quasi-diagonlization but it's induced by the order (from left to right) of the dendrogram
 # Based on that we build a tree reflecting the recursive bisection.
 # With that tree and the covariance matrix we go back to the hrp algorithm.
+import pandas as pd
 import numpy.random as nr
 import scipy.cluster.hierarchy as sch
 
 from pyhrp.hrp import tree, linkage, _hrp, dist
 
 
 def bisection(ids):
@@ -19,27 +20,36 @@
     def split(ids):
         # split the vector ids in two parts, split in the middle
         assert len(ids) >= 2
         n = len(ids)
         return ids[:n // 2], ids[n // 2:]
 
     assert len(ids) >= 1
+    assert len(ids) == len(set(ids))
 
     if len(ids) == 1:
         return sch.ClusterNode(id=ids[0])
 
     left, right = split(ids)
-    return sch.ClusterNode(id=nr.randint(low=100000, high=200000), left=bisection(ids=left), right=bisection(ids=right))
+    return sch.ClusterNode(id=0, left=bisection(ids=left), right=bisection(ids=right))
 
 
-def marcos(prices, node=None):
+def marcos(prices, node=None, method=None):
+    # make sure the prices are a DataFrame
+    assert isinstance(prices, pd.DataFrame)
+
+    # convert into returns
     returns = prices.pct_change().dropna(axis=0, how="all")
+
+    # compute covariance matrix and correlation matrices (both as DataFrames)
     cov, cor = returns.cov(), returns.corr()
 
-    node = node or tree(linkage(dist(cor.values), method="single"))
+    # Compute the root node of the tree
+    method = method or "ward"
+    node = node or tree(linkage(dist(cor.values), method=method))
 
     # this is an interesting step
     ids = node.pre_order()
     # apply bisection, root is now a ClusterNode of the graph
     root = bisection(ids=ids)
 
     # It's not clear to me why Marcos is going down this route. Rather than sticking with the graph computed above.
```

### Comparing `pyhrp-0.0.7/setup.py` & `pyhrp-0.0.8/setup.py`

 * *Files identical despite different names*

