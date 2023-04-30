# Comparing `tmp/simulated_bifurcation-1.0.1.tar.gz` & `tmp/simulated_bifurcation-1.0.2.tar.gz`

## Comparing `simulated_bifurcation-1.0.1.tar` & `simulated_bifurcation-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/CITATION.cff
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/requirements.txt
--rw-r--r--   0        0        0    24832 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/src/simulated_bifurcation/__init__.py
--rw-r--r--   0        0        0    13826 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/src/simulated_bifurcation/interface.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/src/simulated_bifurcation/markowitz.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/src/simulated_bifurcation/partitioning.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/src/simulated_bifurcation/qubo.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/.gitignore
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/LICENSE
--rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/README.md
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     9425 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/CITATION.cff
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/requirements.txt
+-rw-r--r--   0        0        0    24832 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/src/simulated_bifurcation/__init__.py
+-rw-r--r--   0        0        0    13826 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/src/simulated_bifurcation/interface.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/src/simulated_bifurcation/markowitz.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/src/simulated_bifurcation/partitioning.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/src/simulated_bifurcation/qubo.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/LICENSE
+-rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/README.md
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     9425 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/PKG-INFO
```

### Comparing `simulated_bifurcation-1.0.1/src/simulated_bifurcation/__init__.py` & `simulated_bifurcation-1.0.2/src/simulated_bifurcation/__init__.py`

 * *Files identical despite different names*

### Comparing `simulated_bifurcation-1.0.1/src/simulated_bifurcation/interface.py` & `simulated_bifurcation-1.0.2/src/simulated_bifurcation/interface.py`

 * *Files identical despite different names*

### Comparing `simulated_bifurcation-1.0.1/src/simulated_bifurcation/markowitz.py` & `simulated_bifurcation-1.0.2/src/simulated_bifurcation/markowitz.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,16 @@
         risk_coefficient: float = 1, 
         number_of_bits: int = 1,
         dtype: torch.dtype=torch.float32,
         device: str = 'cpu'
     ) -> None:
 
         # Data
-        self.covariance       = covariance.to(dtype, device)
-        self.expected_return  = expected_return.to(dtype, device)
+        self.covariance       = covariance.to(dtype=dtype, device=device)
+        self.expected_return  = expected_return.to(dtype=dtype, device=device)
         self.risk_coefficient = risk_coefficient
         super().__init__(- risk_coefficient * covariance, 
                         - expected_return, number_of_bits,
                         dtype, device)
 
     @property
     def portfolio(self) -> torch.Tensor: return self.solution
```

### Comparing `simulated_bifurcation-1.0.1/src/simulated_bifurcation/partitioning.py` & `simulated_bifurcation-1.0.2/src/simulated_bifurcation/partitioning.py`

 * *Files identical despite different names*

### Comparing `simulated_bifurcation-1.0.1/src/simulated_bifurcation/qubo.py` & `simulated_bifurcation-1.0.2/src/simulated_bifurcation/qubo.py`

 * *Files identical despite different names*

### Comparing `simulated_bifurcation-1.0.1/.gitignore` & `simulated_bifurcation-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `simulated_bifurcation-1.0.1/LICENSE` & `simulated_bifurcation-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simulated_bifurcation-1.0.1/README.md` & `simulated_bifurcation-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -159,11 +159,11 @@
 If you are using this code for your own projects please cite our work:
 
 ```bibtex
 @software{Ageron_Simulated_Bifurcation_SB_2022,
     author = {Ageron, Romain and Bouquet, Thomas and Pugliese, Lorenzo},
     month = {4},
     title = {{Simulated Bifurcation (SB) algorithm for Python}},
-    version = {1.0.0},
+    version = {1.0.2},
     year = {2023}
 }
 ```
```

### Comparing `simulated_bifurcation-1.0.1/pyproject.toml` & `simulated_bifurcation-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simulated_bifurcation"
-version = "1.0.1"
+version = "1.0.2"
 description = "An efficient implementation of the quantum physics-inspired Simulated Bifurcation (SB) algorithm to solve Ising-like problems."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `simulated_bifurcation-1.0.1/PKG-INFO` & `simulated_bifurcation-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulated_bifurcation
-Version: 1.0.1
+Version: 1.0.2
 Summary: An efficient implementation of the quantum physics-inspired Simulated Bifurcation (SB) algorithm to solve Ising-like problems.
 Project-URL: Homepage, https://github.com/bqth29/simulated-bifurcation-algorithm
 Project-URL: Bug Tracker, https://github.com/bqth29/simulated-bifurcation-algorithm/issues
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -172,11 +172,11 @@
 If you are using this code for your own projects please cite our work:
 
 ```bibtex
 @software{Ageron_Simulated_Bifurcation_SB_2022,
     author = {Ageron, Romain and Bouquet, Thomas and Pugliese, Lorenzo},
     month = {4},
     title = {{Simulated Bifurcation (SB) algorithm for Python}},
-    version = {1.0.0},
+    version = {1.0.2},
     year = {2023}
 }
 ```
```

