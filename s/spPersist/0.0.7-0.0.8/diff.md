# Comparing `tmp/sppersist-0.0.7.tar.gz` & `tmp/sppersist-0.0.8.tar.gz`

## Comparing `sppersist-0.0.7.tar` & `sppersist-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.0.7/src/spPersist/__init__.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 sppersist-0.0.7/src/spPersist/read.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.0.7/LICENSE
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sppersist-0.0.7/README.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sppersist-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 sppersist-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.0.8/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 sppersist-0.0.8/src/spPersist/read.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.0.8/LICENSE
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sppersist-0.0.8/README.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sppersist-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 sppersist-0.0.8/PKG-INFO
```

### Comparing `sppersist-0.0.7/src/spPersist/read.py` & `sppersist-0.0.8/src/spPersist/read.py`

 * *Files identical despite different names*

### Comparing `sppersist-0.0.7/LICENSE` & `sppersist-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-0.0.7/pyproject.toml` & `sppersist-0.0.8/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial analysis package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sppersist-0.0.7/PKG-INFO` & `sppersist-0.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.0.7
+Version: 0.0.8
 Summary: Spatial analysis package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

