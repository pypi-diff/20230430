# Comparing `tmp/facefinder-0.1.2.tar.gz` & `tmp/facefinder-0.1.3.tar.gz`

## Comparing `facefinder-0.1.2.tar` & `facefinder-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 facefinder-0.1.2/Cargo.toml
--rw-r--r--   0        0        0     2795 2023-04-10 04:37:28.000000 facefinder-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0        0        0      697 2023-04-20 14:44:25.000000 facefinder-0.1.2/.gitignore
--rw-r--r--   0        0        0      541 2023-04-20 07:56:10.000000 facefinder-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      198 2023-04-24 13:40:08.000000 facefinder-0.1.2/src/python/facefinder/__init__.py
--rw-r--r--   0        0        0     6651 2023-04-20 14:34:18.000000 facefinder-0.1.2/src/python/facefinder/interact.py
--rw-r--r--   0        0        0     3871 2023-04-20 09:22:54.000000 facefinder-0.1.2/src/python/facefinder/metadata.py
--rw-r--r--   0        0        0    16960 2023-04-25 14:34:07.000000 facefinder-0.1.2/src/python/facefinder/metrics.py
--rw-r--r--   0        0        0     4892 2023-03-14 01:32:39.000000 facefinder-0.1.2/src/python/facefinder/prompting.py
--rw-r--r--   0        0        0      349 2023-04-20 07:54:19.000000 facefinder-0.1.2/src/rust/lib.rs
--rw-r--r--   0        0        0     7654 2023-04-25 14:35:01.000000 facefinder-0.1.2/Cargo.lock
--rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 facefinder-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 facefinder-0.1.3/Cargo.toml
+-rw-r--r--   0        0        0     2795 2023-04-10 04:37:28.000000 facefinder-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      697 2023-04-20 14:44:25.000000 facefinder-0.1.3/.gitignore
+-rw-r--r--   0        0        0      541 2023-04-20 07:56:10.000000 facefinder-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      202 2023-04-30 10:00:01.000000 facefinder-0.1.3/src/python/facefinder/__init__.py
+-rw-r--r--   0        0        0     6651 2023-04-20 14:34:18.000000 facefinder-0.1.3/src/python/facefinder/interact.py
+-rw-r--r--   0        0        0     3871 2023-04-20 09:22:54.000000 facefinder-0.1.3/src/python/facefinder/metadata.py
+-rw-r--r--   0        0        0    19845 2023-04-30 10:25:34.000000 facefinder-0.1.3/src/python/facefinder/metrics.py
+-rw-r--r--   0        0        0     4892 2023-03-14 01:32:39.000000 facefinder-0.1.3/src/python/facefinder/prompting.py
+-rw-r--r--   0        0        0      349 2023-04-20 07:54:19.000000 facefinder-0.1.3/src/rust/lib.rs
+-rw-r--r--   0        0        0     7654 2023-04-30 10:54:28.000000 facefinder-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 facefinder-0.1.3/PKG-INFO
```

### Comparing `facefinder-0.1.2/.github/workflows/CI.yml` & `facefinder-0.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.2/.gitignore` & `facefinder-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.2/pyproject.toml` & `facefinder-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.2/src/python/facefinder/interact.py` & `facefinder-0.1.3/src/python/facefinder/interact.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.2/src/python/facefinder/metadata.py` & `facefinder-0.1.3/src/python/facefinder/metadata.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.2/src/python/facefinder/prompting.py` & `facefinder-0.1.3/src/python/facefinder/prompting.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.2/Cargo.lock` & `facefinder-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "facefinder"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
```

