# Comparing `tmp/python_frank_energie-4.0.0.tar.gz` & `tmp/python_frank_energie-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_frank_energie-4.0.0.tar", max compression
+gzip compressed data, was "python_frank_energie-4.0.1.tar", max compression
```

## Comparing `python_frank_energie-4.0.0.tar` & `python_frank_energie-4.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11346 2023-04-23 13:11:10.815568 python_frank_energie-4.0.0/LICENSE
--rw-r--r--   0        0        0      325 2023-04-23 13:11:10.815568 python_frank_energie-4.0.0/README.md
--rw-r--r--   0        0        0     2353 2023-04-23 13:11:39.727562 python_frank_energie-4.0.0/pyproject.toml
--rw-r--r--   0        0        0      175 2023-04-23 13:11:10.815568 python_frank_energie-4.0.0/python_frank_energie/__init__.py
--rw-r--r--   0        0        0      378 2023-04-23 13:11:10.815568 python_frank_energie-4.0.0/python_frank_energie/exceptions.py
--rw-r--r--   0        0        0     7195 2023-04-23 13:11:10.815568 python_frank_energie-4.0.0/python_frank_energie/frank_energie.py
--rw-r--r--   0        0        0     9879 2023-04-23 13:11:10.815568 python_frank_energie-4.0.0/python_frank_energie/models.py
--rw-r--r--   0        0        0     1217 1970-01-01 00:00:00.000000 python_frank_energie-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-04-30 08:35:22.681678 python_frank_energie-4.0.1/LICENSE
+-rw-r--r--   0        0        0      325 2023-04-30 08:35:22.681678 python_frank_energie-4.0.1/README.md
+-rw-r--r--   0        0        0     2353 2023-04-30 08:35:46.114092 python_frank_energie-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-04-30 08:35:22.681678 python_frank_energie-4.0.1/python_frank_energie/__init__.py
+-rw-r--r--   0        0        0      378 2023-04-30 08:35:22.681678 python_frank_energie-4.0.1/python_frank_energie/exceptions.py
+-rw-r--r--   0        0        0     7195 2023-04-30 08:35:22.681678 python_frank_energie-4.0.1/python_frank_energie/frank_energie.py
+-rw-r--r--   0        0        0    10023 2023-04-30 08:35:22.681678 python_frank_energie-4.0.1/python_frank_energie/models.py
+-rw-r--r--   0        0        0     1217 1970-01-01 00:00:00.000000 python_frank_energie-4.0.1/PKG-INFO
```

### Comparing `python_frank_energie-4.0.0/LICENSE` & `python_frank_energie-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_frank_energie-4.0.0/pyproject.toml` & `python_frank_energie-4.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-frank-energie"
-version = "4.0.0"
+version = "4.0.1"
 description = "Asynchronous Python client for the Frank Energie"
 authors = ["DCSBL"]
 maintainers = ["DCSBL"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://github.com/dcsbl/python-frank-energie"
 repository = "https://github.com/dcsbl/python-frank-energie"
```

### Comparing `python_frank_energie-4.0.0/python_frank_energie/frank_energie.py` & `python_frank_energie-4.0.1/python_frank_energie/frank_energie.py`

 * *Files identical despite different names*

### Comparing `python_frank_energie-4.0.0/python_frank_energie/models.py` & `python_frank_energie-4.0.1/python_frank_energie/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,17 +288,20 @@
     electricity: PriceData
     gas: PriceData
 
     @staticmethod
     def from_dict(data: dict[str, str]) -> MarketPrices:
         """Parse the response from the marketPrices query."""
         if errors := data.get("errors"):
+            if errors[0]["message"].startswith("No marketprices found for segment"):
+                return MarketPrices(PriceData(), PriceData())
+
             raise RequestException(errors[0]["message"])
 
-        payload = data.get("data", {})
+        payload = data.get("data")
         if not payload:
             raise RequestException("Unexpected response")
 
         return MarketPrices(
             electricity=PriceData(payload.get("marketPricesElectricity")),
             gas=PriceData(payload.get("marketPricesGas")),
         )
```

### Comparing `python_frank_energie-4.0.0/PKG-INFO` & `python_frank_energie-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-frank-energie
-Version: 4.0.0
+Version: 4.0.1
 Summary: Asynchronous Python client for the Frank Energie
 Home-page: https://github.com/dcsbl/python-frank-energie
 License: Apache-2.0
 Author: DCSBL
 Maintainer: DCSBL
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

