# Comparing `tmp/rrcf-0.4.3.tar.gz` & `tmp/rrcf-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rrcf-0.4.3.tar", last modified: Wed Jun 10 01:53:47 2020, max compression
+gzip compressed data, was "rrcf-0.4.4.tar", last modified: Sun Apr 30 02:24:35 2023, max compression
```

## Comparing `rrcf-0.4.3.tar` & `rrcf-0.4.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 mdbartos   (501) staff       (20)        0 2020-06-10 01:53:47.000000 rrcf-0.4.3/
--rw-r--r--   0 mdbartos   (501) staff       (20)      349 2020-06-10 01:53:47.000000 rrcf-0.4.3/PKG-INFO
-drwxr-xr-x   0 mdbartos   (501) staff       (20)        0 2020-06-10 01:53:47.000000 rrcf-0.4.3/test/
--rw-r--r--   0 mdbartos   (501) staff       (20)     5556 2020-06-10 01:53:37.000000 rrcf-0.4.3/test/test_rrcf.py
-drwxr-xr-x   0 mdbartos   (501) staff       (20)        0 2020-06-10 01:53:47.000000 rrcf-0.4.3/rrcf.egg-info/
--rw-r--r--   0 mdbartos   (501) staff       (20)      349 2020-06-10 01:53:46.000000 rrcf-0.4.3/rrcf.egg-info/PKG-INFO
--rw-r--r--   0 mdbartos   (501) staff       (20)      221 2020-06-10 01:53:46.000000 rrcf-0.4.3/rrcf.egg-info/SOURCES.txt
--rw-r--r--   0 mdbartos   (501) staff       (20)        6 2020-06-10 01:53:46.000000 rrcf-0.4.3/rrcf.egg-info/requires.txt
--rw-r--r--   0 mdbartos   (501) staff       (20)        5 2020-06-10 01:53:46.000000 rrcf-0.4.3/rrcf.egg-info/top_level.txt
--rw-r--r--   0 mdbartos   (501) staff       (20)        1 2020-06-10 01:53:46.000000 rrcf-0.4.3/rrcf.egg-info/dependency_links.txt
--rw-r--r--   0 mdbartos   (501) staff       (20)     8870 2020-06-10 01:53:37.000000 rrcf-0.4.3/README.md
--rw-r--r--   0 mdbartos   (501) staff       (20)      445 2020-06-10 01:53:37.000000 rrcf-0.4.3/setup.py
--rw-r--r--   0 mdbartos   (501) staff       (20)       38 2020-06-10 01:53:47.000000 rrcf-0.4.3/setup.cfg
-drwxr-xr-x   0 mdbartos   (501) staff       (20)        0 2020-06-10 01:53:47.000000 rrcf-0.4.3/rrcf/
--rw-r--r--   0 mdbartos   (501) staff       (20)      634 2020-06-10 01:53:37.000000 rrcf-0.4.3/rrcf/shingle.py
--rw-r--r--   0 mdbartos   (501) staff       (20)      140 2020-06-10 01:53:37.000000 rrcf-0.4.3/rrcf/__init__.py
--rw-r--r--   0 mdbartos   (501) staff       (20)    35066 2020-06-10 01:53:37.000000 rrcf-0.4.3/rrcf/rrcf.py
+drwxr-xr-x   0 mdbartos   (501) staff       (20)        0 2023-04-30 02:24:35.805955 rrcf-0.4.4/
+-rw-r--r--   0 mdbartos   (501) staff       (20)     1063 2023-04-30 02:24:02.000000 rrcf-0.4.4/LICENSE
+-rw-r--r--   0 mdbartos   (501) staff       (20)      326 2023-04-30 02:24:35.805832 rrcf-0.4.4/PKG-INFO
+-rw-r--r--   0 mdbartos   (501) staff       (20)     8870 2023-04-30 02:24:02.000000 rrcf-0.4.4/README.md
+drwxr-xr-x   0 mdbartos   (501) staff       (20)        0 2023-04-30 02:24:35.805083 rrcf-0.4.4/rrcf/
+-rw-r--r--   0 mdbartos   (501) staff       (20)      140 2023-04-30 02:24:02.000000 rrcf-0.4.4/rrcf/__init__.py
+-rw-r--r--   0 mdbartos   (501) staff       (20)    35042 2023-04-30 02:24:02.000000 rrcf-0.4.4/rrcf/rrcf.py
+-rw-r--r--   0 mdbartos   (501) staff       (20)      634 2023-04-30 02:24:02.000000 rrcf-0.4.4/rrcf/shingle.py
+drwxr-xr-x   0 mdbartos   (501) staff       (20)        0 2023-04-30 02:24:35.805588 rrcf-0.4.4/rrcf.egg-info/
+-rw-r--r--   0 mdbartos   (501) staff       (20)      326 2023-04-30 02:24:35.000000 rrcf-0.4.4/rrcf.egg-info/PKG-INFO
+-rw-r--r--   0 mdbartos   (501) staff       (20)      229 2023-04-30 02:24:35.000000 rrcf-0.4.4/rrcf.egg-info/SOURCES.txt
+-rw-r--r--   0 mdbartos   (501) staff       (20)        1 2023-04-30 02:24:35.000000 rrcf-0.4.4/rrcf.egg-info/dependency_links.txt
+-rw-r--r--   0 mdbartos   (501) staff       (20)        6 2023-04-30 02:24:35.000000 rrcf-0.4.4/rrcf.egg-info/requires.txt
+-rw-r--r--   0 mdbartos   (501) staff       (20)        5 2023-04-30 02:24:35.000000 rrcf-0.4.4/rrcf.egg-info/top_level.txt
+-rw-r--r--   0 mdbartos   (501) staff       (20)       38 2023-04-30 02:24:35.805997 rrcf-0.4.4/setup.cfg
+-rw-r--r--   0 mdbartos   (501) staff       (20)      445 2023-04-30 02:24:02.000000 rrcf-0.4.4/setup.py
+drwxr-xr-x   0 mdbartos   (501) staff       (20)        0 2023-04-30 02:24:35.805684 rrcf-0.4.4/test/
+-rw-r--r--   0 mdbartos   (501) staff       (20)     5556 2023-04-30 02:24:02.000000 rrcf-0.4.4/test/test_rrcf.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rrcf-0.4.3/test/test_rrcf.py` & `rrcf-0.4.4/test/test_rrcf.py`

 * *Files identical despite different names*

### Comparing `rrcf-0.4.3/README.md` & `rrcf-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `rrcf-0.4.3/rrcf/shingle.py` & `rrcf-0.4.4/rrcf/shingle.py`

 * *Files identical despite different names*

### Comparing `rrcf-0.4.3/rrcf/rrcf.py` & `rrcf-0.4.4/rrcf/rrcf.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,22 +91,22 @@
                                 axis=0)
             # If duplicates exist, take unique elements
             if N.max() > 1:
                 n, d = U.shape
                 X = U
             else:
                 n, d = X.shape
-                N = np.ones(n, dtype=np.int)
+                N = np.ones(n, dtype=int)
                 I = None
             # Store dimension of dataset
             self.ndim = d
             # Set node above to None in case of bottom-up search
             self.u = None
             # Create RRC Tree
-            S = np.ones(n, dtype=np.bool)
+            S = np.ones(n, dtype=bool)
             self._mktree(X, S, N, I, parent=self)
             # Remove parent of root
             self.root.u = None
             # Count all leaves under each branch
             self._count_all_top_down(self.root)
             # Set bboxes of all branches
             self._get_bbox_top_down(self.root)
@@ -173,15 +173,15 @@
         # If S1 does not contain an isolated point...
         if S1.sum() > 1:
             # Recursively construct tree on S1
             self._mktree(X, S1, N, I, parent=branch, side='l', depth=depth)
         # Otherwise...
         else:
             # Create a leaf node from isolated point
-            i = np.asscalar(np.flatnonzero(S1))
+            i = np.flatnonzero(S1).item()
             leaf = Leaf(i=i, d=depth, u=branch, x=X[i, :], n=N[i])
             # Link leaf node to parent
             branch.l = leaf
             # If duplicates exist...
             if I is not None:
                 # Add a key in the leaves dict pointing to leaf for all duplicate indices
                 J = np.flatnonzero(I == i)
@@ -195,15 +195,15 @@
         # If S2 does not contain an isolated point...
         if S2.sum() > 1:
             # Recursively construct tree on S2
             self._mktree(X, S2, N, I, parent=branch, side='r', depth=depth)
         # Otherwise...
         else:
             # Create a leaf node from isolated point
-            i = np.asscalar(np.flatnonzero(S2))
+            i = np.flatnonzero(S2).item()
             leaf = Leaf(i=i, d=depth, u=branch, x=X[i, :], n=N[i])
             # Link leaf node to parent
             branch.r = leaf
             # If duplicates exist...
             if I is not None:
                 # Add a key in the leaves dict pointing to leaf for all duplicate indices
                 J = np.flatnonzero(I == i)
@@ -933,15 +933,15 @@
 
     def _count_leaves(self, node):
         """
         Count leaves underneath a single node.
         """
         num_leaves = np.array(0, dtype=np.int64)
         self.map_leaves(node, op=self._accumulate, accumulator=num_leaves)
-        num_leaves = np.asscalar(num_leaves)
+        num_leaves = num_leaves.item()
         return num_leaves
 
     def _query(self, point, node):
         """
         Recursively search for the nearest leaf to a given point.
         """
         if isinstance(node, Leaf):
```

