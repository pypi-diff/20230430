# Comparing `tmp/sppersist-0.0.2.tar.gz` & `tmp/sppersist-0.0.3.tar.gz`

## Comparing `sppersist-0.0.2.tar` & `sppersist-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.0.2/src/spPersist/__init__.py
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 sppersist-0.0.2/src/spPersist/accession_to_h5.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 sppersist-0.0.2/src/spPersist/visium.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.0.2/LICENSE
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sppersist-0.0.2/README.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 sppersist-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 sppersist-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.0.3/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 sppersist-0.0.3/src/spPersist/accession_to_h5-1.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 sppersist-0.0.3/src/spPersist/visium.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.0.3/LICENSE
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sppersist-0.0.3/README.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 sppersist-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 sppersist-0.0.3/PKG-INFO
```

### Comparing `sppersist-0.0.2/src/spPersist/accession_to_h5.py` & `sppersist-0.0.3/src/spPersist/accession_to_h5-1.py`

 * *Files identical despite different names*

### Comparing `sppersist-0.0.2/src/spPersist/visium.py` & `sppersist-0.0.3/src/spPersist/visium.py`

 * *Files identical despite different names*

### Comparing `sppersist-0.0.2/LICENSE` & `sppersist-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-0.0.2/pyproject.toml` & `sppersist-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial analysis with Persistent Homology"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sppersist-0.0.2/PKG-INFO` & `sppersist-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.0.2
+Version: 0.0.3
 Summary: Spatial analysis with Persistent Homology
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

