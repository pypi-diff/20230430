# Comparing `tmp/rm545_xd-0.6.2.tar.gz` & `tmp/rm545_xd-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rm545_xd-0.6.2.tar", last modified: Fri Apr 28 16:40:31 2023, max compression
+gzip compressed data, was "rm545_xd-0.7.2.tar", last modified: Sun Apr 30 00:53:18 2023, max compression
```

## Comparing `rm545_xd-0.6.2.tar` & `rm545_xd-0.7.2.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 xuantingdong   (501) staff       (20)        0 2023-04-28 16:40:31.717032 rm545_xd-0.6.2/
--rw-r--r--   0 xuantingdong   (501) staff       (20)      331 2023-04-28 16:40:31.716863 rm545_xd-0.6.2/PKG-INFO
--rw-r--r--   0 xuantingdong   (501) staff       (20)        0 2023-04-28 16:37:40.000000 rm545_xd-0.6.2/README.md
--rw-r--r--   0 xuantingdong   (501) staff       (20)      464 2023-04-28 16:40:25.000000 rm545_xd-0.6.2/pyproject.toml
--rw-r--r--   0 xuantingdong   (501) staff       (20)       38 2023-04-28 16:40:31.717089 rm545_xd-0.6.2/setup.cfg
-drwxr-xr-x   0 xuantingdong   (501) staff       (20)        0 2023-04-28 16:40:31.713986 rm545_xd-0.6.2/src/
-drwxr-xr-x   0 xuantingdong   (501) staff       (20)        0 2023-04-28 16:40:31.715796 rm545_xd-0.6.2/src/rm545_xd/
--rw-rw-r--   0 xuantingdong   (501) staff       (20)     7085 2023-04-28 16:29:22.000000 rm545_xd-0.6.2/src/rm545_xd/VaR.py
--rw-r--r--   0 xuantingdong   (501) staff       (20)        0 2023-04-28 16:28:59.000000 rm545_xd-0.6.2/src/rm545_xd/__init__.py
--rw-rw-r--   0 xuantingdong   (501) staff       (20)     1864 2023-04-28 16:29:22.000000 rm545_xd-0.6.2/src/rm545_xd/calculation.py
--rw-rw-r--   0 xuantingdong   (501) staff       (20)     6713 2023-04-28 16:29:22.000000 rm545_xd-0.6.2/src/rm545_xd/cov_matrix.py
--rw-rw-r--   0 xuantingdong   (501) staff       (20)      683 2023-04-28 16:29:22.000000 rm545_xd-0.6.2/src/rm545_xd/linear_regression.py
--rw-rw-r--   0 xuantingdong   (501) staff       (20)     3311 2023-04-28 16:29:22.000000 rm545_xd-0.6.2/src/rm545_xd/simulation.py
-drwxr-xr-x   0 xuantingdong   (501) staff       (20)        0 2023-04-28 16:40:31.716637 rm545_xd-0.6.2/src/rm545_xd.egg-info/
--rw-r--r--   0 xuantingdong   (501) staff       (20)      331 2023-04-28 16:40:31.000000 rm545_xd-0.6.2/src/rm545_xd.egg-info/PKG-INFO
--rw-r--r--   0 xuantingdong   (501) staff       (20)      329 2023-04-28 16:40:31.000000 rm545_xd-0.6.2/src/rm545_xd.egg-info/SOURCES.txt
--rw-r--r--   0 xuantingdong   (501) staff       (20)        1 2023-04-28 16:40:31.000000 rm545_xd-0.6.2/src/rm545_xd.egg-info/dependency_links.txt
--rw-r--r--   0 xuantingdong   (501) staff       (20)        9 2023-04-28 16:40:31.000000 rm545_xd-0.6.2/src/rm545_xd.egg-info/top_level.txt
+drwxr-xr-x   0 xuantingdong   (501) staff       (20)        0 2023-04-30 00:53:18.468195 rm545_xd-0.7.2/
+-rw-r--r--   0 xuantingdong   (501) staff       (20)      331 2023-04-30 00:53:18.468018 rm545_xd-0.7.2/PKG-INFO
+-rw-r--r--   0 xuantingdong   (501) staff       (20)        0 2023-04-30 00:51:44.000000 rm545_xd-0.7.2/README.md
+-rw-r--r--   0 xuantingdong   (501) staff       (20)      464 2023-04-30 00:52:43.000000 rm545_xd-0.7.2/pyproject.toml
+-rw-r--r--   0 xuantingdong   (501) staff       (20)       38 2023-04-30 00:53:18.468244 rm545_xd-0.7.2/setup.cfg
+drwxr-xr-x   0 xuantingdong   (501) staff       (20)        0 2023-04-30 00:53:18.464112 rm545_xd-0.7.2/src/
+drwxr-xr-x   0 xuantingdong   (501) staff       (20)        0 2023-04-30 00:53:18.467090 rm545_xd-0.7.2/src/qrm545_xd/
+-rw-rw-r--   0 xuantingdong   (501) staff       (20)    16468 2023-04-30 00:49:56.000000 rm545_xd-0.7.2/src/qrm545_xd/Option.py
+-rw-rw-r--   0 xuantingdong   (501) staff       (20)      317 2023-04-30 00:49:56.000000 rm545_xd-0.7.2/src/qrm545_xd/VaR.py
+-rw-r--r--   0 xuantingdong   (501) staff       (20)        0 2023-04-30 00:49:35.000000 rm545_xd-0.7.2/src/qrm545_xd/__init__.py
+-rw-rw-r--   0 xuantingdong   (501) staff       (20)     1865 2023-04-30 00:49:56.000000 rm545_xd-0.7.2/src/qrm545_xd/calculation.py
+-rw-rw-r--   0 xuantingdong   (501) staff       (20)     7874 2023-04-30 00:49:56.000000 rm545_xd-0.7.2/src/qrm545_xd/cov_matrix.py
+-rw-rw-r--   0 xuantingdong   (501) staff       (20)     1534 2023-04-30 00:49:56.000000 rm545_xd-0.7.2/src/qrm545_xd/linear_regression.py
+-rw-rw-r--   0 xuantingdong   (501) staff       (20)     1648 2023-04-30 00:49:56.000000 rm545_xd-0.7.2/src/qrm545_xd/optimal_portfolio.py
+-rw-rw-r--   0 xuantingdong   (501) staff       (20)     5605 2023-04-30 00:49:56.000000 rm545_xd-0.7.2/src/qrm545_xd/risk_attribution.py
+-rw-rw-r--   0 xuantingdong   (501) staff       (20)     2641 2023-04-30 00:49:56.000000 rm545_xd-0.7.2/src/qrm545_xd/risk_parity.py
+-rw-rw-r--   0 xuantingdong   (501) staff       (20)     5280 2023-04-30 00:49:56.000000 rm545_xd-0.7.2/src/qrm545_xd/simulation.py
+drwxr-xr-x   0 xuantingdong   (501) staff       (20)        0 2023-04-30 00:53:18.467809 rm545_xd-0.7.2/src/rm545_xd.egg-info/
+-rw-r--r--   0 xuantingdong   (501) staff       (20)      331 2023-04-30 00:53:18.000000 rm545_xd-0.7.2/src/rm545_xd.egg-info/PKG-INFO
+-rw-r--r--   0 xuantingdong   (501) staff       (20)      457 2023-04-30 00:53:18.000000 rm545_xd-0.7.2/src/rm545_xd.egg-info/SOURCES.txt
+-rw-r--r--   0 xuantingdong   (501) staff       (20)        1 2023-04-30 00:53:18.000000 rm545_xd-0.7.2/src/rm545_xd.egg-info/dependency_links.txt
+-rw-r--r--   0 xuantingdong   (501) staff       (20)       10 2023-04-30 00:53:18.000000 rm545_xd-0.7.2/src/rm545_xd.egg-info/top_level.txt
```

### Comparing `rm545_xd-0.6.2/src/rm545_xd/calculation.py` & `rm545_xd-0.7.2/src/qrm545_xd/calculation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import pandas as pd
 
+
 # Calculate the return
 def return_calculate(prices, method="DISCRETE", dateColumn="Date"):
     vars_ = prices.columns
     nVars = len(vars_)
     vars_ = [var for var in vars_ if var != dateColumn]
     if nVars == len(vars_):
         raise ValueError(f"dateColumn: {dateColumn} not in DataFrame: {vars_}")
```

### Comparing `rm545_xd-0.6.2/src/rm545_xd/cov_matrix.py` & `rm545_xd-0.7.2/src/qrm545_xd/cov_matrix.py`

 * *Files 14% similar despite different names*

```diff
@@ -198,8 +198,45 @@
         Yk = np.matmul(np.matmul(invSD, Yk), invSD)
     return Yk
 
 # Check the matrix is PSD or not
 def is_psd(matrix):
     """For a given matrix, check if the matrix is psd or not."""
     eigenvalues = np.linalg.eigh(matrix)[0]
-    return np.all(eigenvalues >= -1e-8)
+    return np.all(eigenvalues >= -1e-8)
+
+
+def missing_cov(x, skipMiss=True, fun=np.corrcoef):
+    n, m = x.shape
+    nMiss = np.sum(np.isnan(x), axis=0)
+
+    # nothing missing, just calculate it.
+    if np.sum(nMiss) == 0:
+        return fun(x)
+
+    idxMissing = [set(np.where(np.isnan(x[:, i]))[0]) for i in range(m)]
+
+    if skipMiss:
+        # Skipping Missing, get all the rows which have values and calculate the covariance
+        rows = set(range(n))
+        for c in range(m):
+            for rm in idxMissing[c]:
+                if rm in rows:
+                    rows.remove(rm)
+        rows = sorted(list(rows))
+        return fun(x[rows,:].T)
+
+    else:
+        # Pairwise, for each cell, calculate the covariance.
+        out = np.empty((m, m))
+        for i in range(m):
+            for j in range(i+1):
+                rows = set(range(n))
+                for c in (i,j):
+                    for rm in idxMissing[c]:
+                        if rm in rows:
+                            rows.remove(rm)
+                rows = sorted(list(rows))
+                out[i,j] = fun(x[rows,:][:,[i,j]].T)[0,1]
+                if i != j:
+                    out[j,i] = out[i,j]
+        return out
```

