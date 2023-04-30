# Comparing `tmp/qrmfinal_xd-0.1.6.tar.gz` & `tmp/qrmfinal_xd-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrmfinal_xd-0.1.6.tar", max compression
+gzip compressed data, was "qrmfinal_xd-0.2.0.tar", max compression
```

## Comparing `qrmfinal_xd-0.1.6.tar` & `qrmfinal_xd-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      599 2023-04-30 18:20:25.232184 qrmfinal_xd-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      379 2023-04-30 17:57:11.864517 qrmfinal_xd-0.1.6/src/qrmfinal_xd/VaR.py
--rw-r--r--   0        0        0      182 2023-04-30 18:13:29.150658 qrmfinal_xd-0.1.6/src/qrmfinal_xd/__init__.py
--rw-r--r--   0        0        0     1854 2023-04-30 17:38:39.851104 qrmfinal_xd-0.1.6/src/qrmfinal_xd/cal.py
--rw-r--r--   0        0        0     7874 2023-04-30 17:35:06.989884 qrmfinal_xd-0.1.6/src/qrmfinal_xd/matrix.py
--rw-r--r--   0        0        0    16461 2023-04-30 17:55:12.456855 qrmfinal_xd-0.1.6/src/qrmfinal_xd/option_cal.py
--rw-r--r--   0        0        0     1641 2023-04-30 17:50:29.692771 qrmfinal_xd-0.1.6/src/qrmfinal_xd/portfolio_cal.py
--rw-r--r--   0        0        0     1530 2023-04-30 17:57:57.248116 qrmfinal_xd-0.1.6/src/qrmfinal_xd/regression.py
--rw-r--r--   0        0        0     8210 2023-04-30 17:58:26.309748 qrmfinal_xd-0.1.6/src/qrmfinal_xd/risk_cal.py
--rw-r--r--   0        0        0     5272 2023-04-30 18:00:25.758611 qrmfinal_xd-0.1.6/src/qrmfinal_xd/simulation.py
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 qrmfinal_xd-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      599 2023-04-30 18:32:58.898197 qrmfinal_xd-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      379 2023-04-30 17:57:11.864517 qrmfinal_xd-0.2.0/src/qrmfinal_xd/VaR.py
+-rw-r--r--   0        0        0      182 2023-04-30 18:31:30.024047 qrmfinal_xd-0.2.0/src/qrmfinal_xd/__init__.py
+-rw-r--r--   0        0        0     1854 2023-04-30 17:38:39.851104 qrmfinal_xd-0.2.0/src/qrmfinal_xd/cal.py
+-rw-r--r--   0        0        0     7874 2023-04-30 17:35:06.989884 qrmfinal_xd-0.2.0/src/qrmfinal_xd/matrix.py
+-rw-r--r--   0        0        0    16461 2023-04-30 17:55:12.456855 qrmfinal_xd-0.2.0/src/qrmfinal_xd/option_cal.py
+-rw-r--r--   0        0        0     1641 2023-04-30 17:50:29.692771 qrmfinal_xd-0.2.0/src/qrmfinal_xd/portfolio_cal.py
+-rw-r--r--   0        0        0     1530 2023-04-30 17:57:57.248116 qrmfinal_xd-0.2.0/src/qrmfinal_xd/regression.py
+-rw-r--r--   0        0        0     8210 2023-04-30 17:58:26.309748 qrmfinal_xd-0.2.0/src/qrmfinal_xd/risk_cal.py
+-rw-r--r--   0        0        0     6587 2023-04-30 18:32:40.334794 qrmfinal_xd-0.2.0/src/qrmfinal_xd/sim_copula.py
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 qrmfinal_xd-0.2.0/PKG-INFO
```

### Comparing `qrmfinal_xd-0.1.6/pyproject.toml` & `qrmfinal_xd-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=58.1.0", "wheel>=0.37.0", "hatchling"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qrmfinal_xd"
-version = "0.1.6"
+version = "0.2.0"
 authors = [
   { name = "Xuanting Dong", email = "xd67@duke.edu" },
 ]
 description = "use for Quant545"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -16,10 +16,10 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 
 [tool.poetry]
 name = "qrmfinal_xd"
-version = "0.1.6"
+version = "0.2.0"
 description = "use for Quant545"
 authors = ["Xuanting Dong <xd67@duke.edu>"]
```

### Comparing `qrmfinal_xd-0.1.6/src/qrmfinal_xd/cal.py` & `qrmfinal_xd-0.2.0/src/qrmfinal_xd/cal.py`

 * *Files identical despite different names*

### Comparing `qrmfinal_xd-0.1.6/src/qrmfinal_xd/matrix.py` & `qrmfinal_xd-0.2.0/src/qrmfinal_xd/matrix.py`

 * *Files identical despite different names*

### Comparing `qrmfinal_xd-0.1.6/src/qrmfinal_xd/option_cal.py` & `qrmfinal_xd-0.2.0/src/qrmfinal_xd/option_cal.py`

 * *Files identical despite different names*

### Comparing `qrmfinal_xd-0.1.6/src/qrmfinal_xd/portfolio_cal.py` & `qrmfinal_xd-0.2.0/src/qrmfinal_xd/portfolio_cal.py`

 * *Files identical despite different names*

### Comparing `qrmfinal_xd-0.1.6/src/qrmfinal_xd/regression.py` & `qrmfinal_xd-0.2.0/src/qrmfinal_xd/regression.py`

 * *Files identical despite different names*

### Comparing `qrmfinal_xd-0.1.6/src/qrmfinal_xd/risk_cal.py` & `qrmfinal_xd-0.2.0/src/qrmfinal_xd/risk_cal.py`

 * *Files identical despite different names*

### Comparing `qrmfinal_xd-0.1.6/src/qrmfinal_xd/simulation.py` & `qrmfinal_xd-0.2.0/src/qrmfinal_xd/sim_copula.py`

 * *Files 18% similar despite different names*

```diff
@@ -118,8 +118,39 @@
     sim_returns = pd.DataFrame()
     for i, stock in enumerate(stocks):
         if fitting_model[i] == 't':       
             sim_returns[stock] = t.ppf(sim_sample_cdf[stock], df=parameters[i][0], loc=parameters[i][1], scale = parameters[i][2])
         elif fitting_model[i] == 'n':
             sim_returns[stock] = norm.ppf(sim_sample_cdf[stock],  loc=parameters[i][0], scale = parameters[i][1])
     
-    return sim_returns, pd.DataFrame(parameters,index=[stocks,fitting_model])
+    return sim_returns, pd.DataFrame(parameters,index=[stocks,fitting_model])
+
+
+def t_copula(returns, seed=1234):
+    stocks = returns.columns.tolist()
+
+    # Fitting generalized T model for each stock
+    parameters = []
+    assets_returns_cdf = pd.DataFrame()
+
+    for stock in stocks:
+        params = simulation.Fitting_t_MLE(returns[stock])
+        parameters.append(params)
+        assets_returns_cdf[stock] = t.cdf(returns[stock],df=params[0], loc=params[1], scale = params[2])
+
+    # Simulate N samples with spearman correlation matrix
+    np.random.seed(seed)
+    spearman_corr_matrix = assets_returns_cdf.corr(method='spearman')
+    sim_sample = simulation.multivariate_normal_simulation(spearman_corr_matrix, 10000, method='pca')
+    sim_sample = pd.DataFrame(sim_sample, columns=stocks)
+
+    # Convert simulation result with cdf of standard normal distribution
+    sim_sample_cdf = pd.DataFrame()
+    for stock in stocks:
+        sim_sample_cdf[stock] = norm.cdf(sim_sample[stock],loc=0,scale=1)
+    
+    # Convert cdf matrix to return matrix with parameters of generalized T model
+    sim_returns = pd.DataFrame()
+    for i, stock in enumerate(stocks):
+        sim_returns[stock] = t.ppf(sim_sample_cdf[stock], df=parameters[i][0], loc=parameters[i][1], scale = parameters[i][2])
+    
+    return sim_returns, pd.DataFrame(parameters, columns=['df', 'loc', 'scale'], index=stocks)
```

### Comparing `qrmfinal_xd-0.1.6/PKG-INFO` & `qrmfinal_xd-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrmfinal-xd
-Version: 0.1.6
+Version: 0.2.0
 Summary: use for Quant545
 Author: Xuanting Dong
 Author-email: xd67@duke.edu
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

