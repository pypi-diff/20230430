# Comparing `tmp/minivn-0.1.2.tar.gz` & `tmp/minivn-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minivn-0.1.2.tar", max compression
+gzip compressed data, was "minivn-0.1.3.tar", max compression
```

## Comparing `minivn-0.1.2.tar` & `minivn-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1958 2023-04-29 21:15:41.719319 minivn-0.1.2/README.md
--rw-r--r--   0        0        0       47 2023-04-29 21:15:41.723319 minivn-0.1.2/minivn/__init__.py
--rw-r--r--   0        0        0     3373 2023-04-29 21:15:41.723319 minivn-0.1.2/minivn/minivn.py
--rw-r--r--   0        0        0      819 2023-04-29 21:15:41.723319 minivn-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2581 1970-01-01 00:00:00.000000 minivn-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2294 2023-04-30 12:03:47.953445 minivn-0.1.3/README.md
+-rw-r--r--   0        0        0       47 2023-04-30 12:03:47.957445 minivn-0.1.3/minivn/__init__.py
+-rw-r--r--   0        0        0     5312 2023-04-30 12:03:47.957445 minivn-0.1.3/minivn/minivn.py
+-rw-r--r--   0        0        0      876 2023-04-30 12:03:47.961445 minivn-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2918 1970-01-01 00:00:00.000000 minivn-0.1.3/PKG-INFO
```

### Comparing `minivn-0.1.2/README.md` & `minivn-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -27,25 +27,34 @@
 
 # Add embeddings to the index
 embedding1 = np.random.rand(128)
 embedding2 = np.random.rand(128)
 embedding3 = np.random.rand(128)
 
 index.add_items([1, 2, 3], [embedding1, embedding2, embedding3])
+
+# or
 index.add_items([4, 5, 6], np.random.rand(3, 128))
 
 # Delete embeddings from the index
 index.delete_items([3])
 
 # Query the index for the nearest neighbor of a given embedding
 query_embedding = np.random.rand(128)
 result = index.query(query_embedding, k=1)
 
 print(result)  # Returns [(index, similarity)] of the nearest neighbor
+
+# Save and load the index
+index.save(filepath)
+
+new_index = Index(dim=128, metric="dot_product")
+new_index.load(filepath)
 ```
 
 ## Comparison with Approximate Nearest Neighbor Search
-Based on a [quick benchmark](https://github.com/aismlv/minivn/blob/main/benchmark/benchmark.md), you might not require an ANN and go with a simpler approach if:
+Based on a [quick benchmark](https://github.com/aismlv/minivn/blob/main/benchmark/README.md), you might not require an ANN and go with a simpler approach if any of the below apply:
 
-- Your document set isn't in the millions
+- Your document set isn't in the multiple millions and you don't need ultra-high latency requirements (to, for example, accommodate a heavy reranker)
 - You're in the experimentation phase and want to iterate quickly on the index
-- You require the best recall and don't want to spend time [fine-tuning hyperparameters](https://github.com/erikbern/ann-benchmarks)
+- Your application requires the best precision and recall
+- You don't want to fine-tune any hyperparameters (which can affect [latency/accuracy trade-off](https://github.com/erikbern/ann-benchmarks) quite a lot)
```

### Comparing `minivn-0.1.2/pyproject.toml` & `minivn-0.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "minivn"
-version = "0.1.2"
+version = "0.1.3"
 description = "Exact nearest neighbor search library for those times when \"approximate\" just won't cut it (or is simply overkill)"
 authors = ["aismlv <adilzhan.ismailov@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.9,<3.12"
 numpy = "^1.24.2"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
 flake8 = "^6.0.0"
 pre-commit = "^3.2.2"
 pytest-cov = "^4.0.0"
+isort = "^5.12.0"
 
 [tool.poetry.group.benchmark]
 optional = true
 
 [tool.poetry.group.benchmark.dependencies]
 pandas = "^2.0.1"
 altair = "5.0.0rc1"
@@ -28,10 +29,13 @@
 ipykernel = "^6.22.0"
 huggingface-hub = "^0.14.1"
 vl-convert-python = "^0.8.1"
 
 [tool.black]
 line-length = 120
 
+[tool.isort]
+profile = "black"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `minivn-0.1.2/PKG-INFO` & `minivn-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: minivn
-Version: 0.1.2
+Version: 0.1.3
 Summary: Exact nearest neighbor search library for those times when "approximate" just won't cut it (or is simply overkill)
 License: Apache-2.0
 Author: aismlv
 Author-email: adilzhan.ismailov@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Description-Content-Type: text/markdown
@@ -43,26 +43,35 @@
 
 # Add embeddings to the index
 embedding1 = np.random.rand(128)
 embedding2 = np.random.rand(128)
 embedding3 = np.random.rand(128)
 
 index.add_items([1, 2, 3], [embedding1, embedding2, embedding3])
+
+# or
 index.add_items([4, 5, 6], np.random.rand(3, 128))
 
 # Delete embeddings from the index
 index.delete_items([3])
 
 # Query the index for the nearest neighbor of a given embedding
 query_embedding = np.random.rand(128)
 result = index.query(query_embedding, k=1)
 
 print(result)  # Returns [(index, similarity)] of the nearest neighbor
+
+# Save and load the index
+index.save(filepath)
+
+new_index = Index(dim=128, metric="dot_product")
+new_index.load(filepath)
 ```
 
 ## Comparison with Approximate Nearest Neighbor Search
-Based on a [quick benchmark](https://github.com/aismlv/minivn/blob/main/benchmark/benchmark.md), you might not require an ANN and go with a simpler approach if:
+Based on a [quick benchmark](https://github.com/aismlv/minivn/blob/main/benchmark/README.md), you might not require an ANN and go with a simpler approach if any of the below apply:
 
-- Your document set isn't in the millions
+- Your document set isn't in the multiple millions and you don't need ultra-high latency requirements (to, for example, accommodate a heavy reranker)
 - You're in the experimentation phase and want to iterate quickly on the index
-- You require the best recall and don't want to spend time [fine-tuning hyperparameters](https://github.com/erikbern/ann-benchmarks)
+- Your application requires the best precision and recall
+- You don't want to fine-tune any hyperparameters (which can affect [latency/accuracy trade-off](https://github.com/erikbern/ann-benchmarks) quite a lot)
```

