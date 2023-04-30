# Comparing `tmp/pyhrp-0.0.8.tar.gz` & `tmp/pyhrp-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyhrp-0.0.8.tar", last modified: Fri May 29 18:56:05 2020, max compression
+gzip compressed data, was "pyhrp-0.4.0.tar", max compression
```

## Comparing `pyhrp-0.0.8.tar` & `pyhrp-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,9 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-29 18:56:05.000000 pyhrp-0.0.8/
--rwxr-xr-x   0 root         (0) root         (0)     1083 2020-05-29 18:50:49.000000 pyhrp-0.0.8/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       58 2020-05-29 18:50:49.000000 pyhrp-0.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2028 2020-05-29 18:56:05.000000 pyhrp-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1332 2020-05-29 18:50:49.000000 pyhrp-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-29 18:56:05.000000 pyhrp-0.0.8/pyhrp/
--rwxr-xr-x   0 root         (0) root         (0)      126 2020-05-29 18:50:49.000000 pyhrp-0.0.8/pyhrp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2473 2020-05-29 18:50:49.000000 pyhrp-0.0.8/pyhrp/cluster.py
--rw-r--r--   0 root         (0) root         (0)      237 2020-05-29 18:50:49.000000 pyhrp-0.0.8/pyhrp/graph.py
--rw-r--r--   0 root         (0) root         (0)     2473 2020-05-29 18:50:49.000000 pyhrp-0.0.8/pyhrp/hrp.py
--rw-r--r--   0 root         (0) root         (0)     1997 2020-05-29 18:50:49.000000 pyhrp-0.0.8/pyhrp/marcos.py
--rw-r--r--   0 root         (0) root         (0)     2532 2020-05-29 18:50:49.000000 pyhrp-0.0.8/pyhrp/obsolete.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-29 18:56:05.000000 pyhrp-0.0.8/pyhrp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2028 2020-05-29 18:56:05.000000 pyhrp-0.0.8/pyhrp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      373 2020-05-29 18:56:05.000000 pyhrp-0.0.8/pyhrp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-05-29 18:56:05.000000 pyhrp-0.0.8/pyhrp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2020-05-29 18:56:05.000000 pyhrp-0.0.8/pyhrp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2020-05-29 18:56:05.000000 pyhrp-0.0.8/pyhrp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      107 2020-05-29 18:56:05.000000 pyhrp-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      721 2020-05-29 18:50:49.000000 pyhrp-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-29 18:56:05.000000 pyhrp-0.0.8/test/
--rw-r--r--   0 root         (0) root         (0)     2151 2020-05-29 18:50:49.000000 pyhrp-0.0.8/test/test_cluster.py
--rw-r--r--   0 root         (0) root         (0)     3166 2020-05-29 18:50:49.000000 pyhrp-0.0.8/test/test_hrp.py
--rw-r--r--   0 root         (0) root         (0)      519 2020-05-29 18:50:49.000000 pyhrp-0.0.8/test/test_marcos.py
--rw-r--r--   0 root         (0) root         (0)      461 2020-05-29 18:50:49.000000 pyhrp-0.0.8/test/test_obsolete.py
+-rwxr-xr-x   0        0        0     1083 2023-04-30 01:16:50.010663 pyhrp-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     1515 2023-04-30 01:16:50.010663 pyhrp-0.4.0/README.md
+-rwxr-xr-x   0        0        0        0 2023-04-30 01:16:50.010663 pyhrp-0.4.0/pyhrp/__init__.py
+-rw-r--r--   0        0        0     3047 2023-04-30 01:16:50.010663 pyhrp-0.4.0/pyhrp/cluster.py
+-rw-r--r--   0        0        0      309 2023-04-30 01:16:50.010663 pyhrp-0.4.0/pyhrp/graph.py
+-rw-r--r--   0        0        0     2559 2023-04-30 01:16:50.010663 pyhrp-0.4.0/pyhrp/hrp.py
+-rw-r--r--   0        0        0     2250 2023-04-30 01:16:50.010663 pyhrp-0.4.0/pyhrp/marcos.py
+-rw-r--r--   0        0        0      479 2023-04-30 01:17:11.884564 pyhrp-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 pyhrp-0.4.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyhrp-0.0.8/LICENSE.txt` & `pyhrp-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyhrp-0.0.8/README.md` & `pyhrp-0.4.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # pyhrp
 
+[![DeepSource](https://deepsource.io/gh/tschm/hrp.svg/?label=active+issues&show_trend=true&token=qjT_aLQgo_1Xbe2Z9ZNdH3Cx)](https://deepsource.io/gh/tschm/hrp/?ref=repository-badge)
+
 A recursive implementation of the Hierarchical Risk Parity (hrp) approach by Marcos Lopez de Prado.
 We take heavily advantage of the scipy.cluster.hierarchy package. 
 
 Here's a simple example
 
 ```python
 import pandas as pd
```

### Comparing `pyhrp-0.0.8/pyhrp/cluster.py` & `pyhrp-0.4.0/pyhrp/cluster.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,97 @@
+"""risk parity for clusters"""
+from dataclasses import dataclass
+from typing import Dict
+
 import numpy as np
 import pandas as pd
 
 
-def risk_parity(cluster_left, cluster_right, cov, node=None):
+def risk_parity(cluster_left, cluster_right, cov):
+    """
+    Given two clusters compute in a bottom-up approach their parent.
+
+    :param cluster_left: left cluster
+    :param cluster_right: right cluster
+    :param cov: (global) covariance matrix. Will pick the correct sub-matrix
+
+    """
+
     # combine two clusters
 
-    def rp(v_left, v_right):
+    def parity(v_left, v_right):
         """
         Compute the weights for a risk parity portfolio of two assets
         :param v_left: Variance of the "left" portfolio
         :param v_right: Variance of the "right" portfolio
-        :return: w, 1-w the weights for the left and the right portfolio. It is w*v_left == (1-w)*v_right and hence w = v_right / (v_right + v_left)
+        :return: w, 1-w the weights for the left and the right portfolio.
+                 It is w*v_left == (1-w)*v_right hence w = v_right / (v_right + v_left)
         """
         return v_right / (v_left + v_right), v_left / (v_left + v_right)
 
-    assert set(cluster_left.assets).isdisjoint(set(cluster_right.assets))
-
-    # the split is such that v_left * alpha_left == v_right * alpha_right and alpha + beta = 1
-    alpha_left, alpha_right = rp(cluster_left.variance, cluster_right.variance)
-
-    # assets in the cluster are the assets of the left and right cluster further downstream
-    assets = {**(alpha_left * cluster_left.weights).to_dict(), **(alpha_right * cluster_right.weights).to_dict()}
-
-    w = np.array(list(assets.values()))
-    c = cov[assets.keys()].loc[assets.keys()]
-
-    var = np.linalg.multi_dot((w, c, w))
-
-    return Cluster(assets=assets, variance=var, left=cluster_left, right=cluster_right, node=node)
-
-
-class Cluster(object):
-    def __init__(self, assets, variance, left=None, right=None, node=None):
-        assert variance >= 0
+    if not set(cluster_left.assets).isdisjoint(set(cluster_right.assets)):
+        raise AssertionError
 
-        self.__node = node
-        self.__assets = assets
-        self.__variance = variance
-        self.__left = left
-        self.__right = right
-        self.__node = node
+    # split is s.t. v_left * alpha_left == v_right * alpha_right and alpha + beta = 1
+    alpha_left, alpha_right = parity(cluster_left.variance, cluster_right.variance)
 
-        if left is None:
+    # assets in the cluster are the assets of the left and right cluster
+    # further downstream
+    assets = {
+        **(alpha_left * cluster_left.weights).to_dict(),
+        **(alpha_right * cluster_right.weights).to_dict(),
+    }
+
+    weights = np.array(list(assets.values()))
+    covariance = cov[assets.keys()].loc[assets.keys()]
+
+    var = np.linalg.multi_dot((weights, covariance, weights))
+
+    return Cluster(
+        assets=assets,
+        variance=var,
+        left=cluster_left,
+        right=cluster_right,  # , node=node
+    )
+
+
+@dataclass(frozen=True)
+class Cluster:
+    """
+    Clusters are the nodes of the graphs we build.
+    Each cluster is aware of the left and the right cluster
+    it is connecting to.
+    """
+
+    assets: Dict[str, float]
+    variance: float
+    left: object = None
+    right: object = None
+
+    def __post_init__(self):
+        """check input"""
+
+        if self.variance <= 0:
+            raise AssertionError
+        if self.left is None:
             # if there is no left, there can't be a right
-            assert right is None
+            if self.right is not None:
+                raise AssertionError
         else:
             # left is not None, hence both left and right have to be clusters
-            assert isinstance(left, Cluster)
-            assert isinstance(right, Cluster)
-            assert set(left.assets.keys()).isdisjoint(set(right.assets.keys()))
-
-    @property
-    def variance(self):
-        return self.__variance
-
-    @property
-    def assets(self):
-        return self.__assets
-
-    @property
-    def left(self):
-        return self.__left
-
-    @property
-    def right(self):
-        return self.__right
+            if not isinstance(self.left, Cluster):
+                raise AssertionError
+            if not isinstance(self.right, Cluster):
+                raise AssertionError
+            if not set(self.left.assets.keys()).isdisjoint(
+                set(self.right.assets.keys())
+            ):
+                raise AssertionError
 
     def is_leaf(self):
+        """true if this cluster is a leaf, e.g. no clusters follow downstream"""
         return self.left is None and self.right is None
 
     @property
     def weights(self):
+        """weight series"""
         return pd.Series(self.assets, name="Weights").sort_index()
-
-    @property
-    def node(self):
-        return self.__node
```

### Comparing `pyhrp-0.0.8/pyhrp/hrp.py` & `pyhrp-0.4.0/pyhrp/hrp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,72 @@
+"""the hrp algorithm"""
 import numpy as np
 import scipy.cluster.hierarchy as sch
+import scipy.spatial.distance as ssd
 
 from pyhrp.cluster import Cluster, risk_parity
 
-import scipy.spatial.distance as ssd
-
 
 def dist(cor):
     """
-    Compute the correlation based distance matrix d, compare with page 239 of the first book by Marcos
+    Compute the correlation based distance matrix d,
+    compare with page 239 of the first book by Marcos
     :param cor: the n x n correlation matrix
-    :return: The matrix d indicating the distance between column i and i. Note that all the diagonal entries are zero.
+    :return: The matrix d indicating the distance between column i and i.
+             Note that all the diagonal entries are zero.
 
     """
     # https://stackoverflow.com/questions/18952587/
-    matrix = np.sqrt(np.clip((1.0 - cor) / 2., a_min=0.0, a_max=1.0))
+    matrix = np.sqrt(np.clip((1.0 - cor) / 2.0, a_min=0.0, a_max=1.0))
     np.fill_diagonal(matrix, val=0.0)
     return ssd.squareform(matrix)
 
 
-def linkage(dist, method="ward", **kwargs):
+def linkage(dist_vec, method="ward", **kwargs):
     """
     Based on distance matrix compute the underlying links
-    :param dist: The distance vector based on the correlation matrix
+    :param dist_vec: The distance vector based on the correlation matrix
     :param method: "single", "ward", etc.
-    :return: links  The links describing the graph (useful to draw the dendrogram) and basis for constructing the tree object
+    :return: links  The links describing the graph (useful to draw the dendrogram)
+                    and basis for constructing the tree object
     """
     # compute the root node of the dendrogram
-    return sch.linkage(dist, method=method, **kwargs)
+    return sch.linkage(dist_vec, method=method, **kwargs)
 
 
-def tree(linkage):
+def tree(links):
     """
     Compute the root ClusterNode.
-    # see https://docs.scipy.org/doc/scipy/reference/generated/scipy.cluster.hierarchy.ClusterNode.html
     :param links: The Linkage matrix compiled by the linkage function above
     :return: The root node. From there it's possible to reach the entire graph
     """
-    return sch.to_tree(linkage, rd=False)
+    return sch.to_tree(links, rd=False)
 
 
-def _hrp(node, cov):
+def build_cluster(node, cov):
+    """compute a cluster"""
     if node.is_leaf():
-        # a node is a leaf if has no further relatives downstream. No leaves, no branches...
+        # a node is a leaf if has no further relatives downstream.
+        # no leaves, no branches, ...
         asset = cov.keys().to_list()[node.id]
-        return Cluster(assets={asset: 1.0}, variance=cov[asset][asset], node=node)
-    else:
-        cluster_left = _hrp(node.left, cov)
-        cluster_right = _hrp(node.right, cov)
-        return risk_parity(cluster_left, cluster_right, cov=cov, node=node)
+        return Cluster(assets={asset: 1.0}, variance=cov[asset][asset])
+
+    # drill down on the left
+    cluster_left = build_cluster(node.left, cov)
+    # drill down on the right
+    cluster_right = build_cluster(node.right, cov)
+    # combine left and right into a new cluster
+    return risk_parity(cluster_left, cluster_right, cov=cov)
 
 
 def hrp(prices, node=None, method="single"):
     """
     Computes the root node for the hierarchical risk parity portfolio
     :param cov: This is the covariance matrix that shall be used
     :param node: Optional. This is the rootnode of the graph describing the dendrogram
     :return: the root cluster of the risk parity portfolio
     """
     returns = prices.pct_change().dropna(axis=0, how="all")
     cov, cor = returns.cov(), returns.corr()
-    links = linkage(dist(cor.values), method=method)
-    node = node or tree(links)
-
-    return _hrp(node, cov)
+    node = node or tree(linkage(dist(cor.values), method=method))
 
+    return build_cluster(node, cov)
```

### Comparing `pyhrp-0.0.8/pyhrp/marcos.py` & `pyhrp-0.4.0/pyhrp/marcos.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,55 @@
-# the original implementation by Marcos Lopez de Prado is using recursive bisection on a ranked list of columns of the covariance matrix
-# To get to this list Lopez de Prado is using what he calls the matrix quasi-diagonlization but it's induced by the order (from left to right) of the dendrogram
-# Based on that we build a tree reflecting the recursive bisection.
-# With that tree and the covariance matrix we go back to the hrp algorithm.
+"""Replicate the implementation of HRP by Marcos Lopez de Prado using this package
+
+The original implementation by Marcos Lopez de Prado is using recursive bisection
+on a ranked list of columns of the covariance matrix
+To get to this list Lopez de Prado is using a matrix quasi-diagonalization
+induced by the order (from left to right) of the dendrogram.
+Based on that we build a tree reflecting the recursive bisection.
+With that tree and the covariance matrix we go back to the hrp algorithm"""
+
 import pandas as pd
-import numpy.random as nr
 import scipy.cluster.hierarchy as sch
 
-from pyhrp.hrp import tree, linkage, _hrp, dist
+from pyhrp.hrp import build_cluster, dist, linkage, tree
 
 
 def bisection(ids):
     """
     Compute the graph underlying the recursive bisection of Marcos Lopez de Prado
 
     :param ids: A (ranked) set of indixes
     :return: The root ClusterNode of this tree
     """
 
     def split(ids):
-        # split the vector ids in two parts, split in the middle
-        assert len(ids) >= 2
-        n = len(ids)
-        return ids[:n // 2], ids[n // 2:]
-
-    assert len(ids) >= 1
-    assert len(ids) == len(set(ids))
+        """split the vector ids in two parts, split in the middle"""
+        if len(ids) < 2:
+            raise AssertionError
+        num = len(ids)
+        return ids[: num // 2], ids[num // 2 :]
+
+    if len(ids) < 1:
+        raise AssertionError
+    if len(ids) != len(set(ids)):
+        raise AssertionError
 
     if len(ids) == 1:
         return sch.ClusterNode(id=ids[0])
 
     left, right = split(ids)
     return sch.ClusterNode(id=0, left=bisection(ids=left), right=bisection(ids=right))
 
 
 def marcos(prices, node=None, method=None):
+    """The algorithm as implemented in the book by Marcos Lopez de Prado"""
+
     # make sure the prices are a DataFrame
-    assert isinstance(prices, pd.DataFrame)
+    if not isinstance(prices, pd.DataFrame):
+        raise AssertionError
 
     # convert into returns
     returns = prices.pct_change().dropna(axis=0, how="all")
 
     # compute covariance matrix and correlation matrices (both as DataFrames)
     cov, cor = returns.cov(), returns.corr()
 
@@ -48,9 +58,10 @@
     node = node or tree(linkage(dist(cor.values), method=method))
 
     # this is an interesting step
     ids = node.pre_order()
     # apply bisection, root is now a ClusterNode of the graph
     root = bisection(ids=ids)
 
-    # It's not clear to me why Marcos is going down this route. Rather than sticking with the graph computed above.
-    return _hrp(node=root, cov=cov)
+    # It's not clear to me why Marcos is going down this route.
+    # Rather than sticking with the graph computed above.
+    return build_cluster(node=root, cov=cov)
```

