# Comparing `tmp/sppersist-0.0.1.tar.gz` & `tmp/sppersist-0.0.2.tar.gz`

## Comparing `sppersist-0.0.1.tar` & `sppersist-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.0.1/src/spPersist/__init__.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 sppersist-0.0.1/src/spPersist/accession_to_h5.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 sppersist-0.0.1/src/spPersist/visium.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.0.1/LICENSE
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sppersist-0.0.1/README.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 sppersist-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 sppersist-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.0.2/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 sppersist-0.0.2/src/spPersist/accession_to_h5.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 sppersist-0.0.2/src/spPersist/visium.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.0.2/LICENSE
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sppersist-0.0.2/README.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 sppersist-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 sppersist-0.0.2/PKG-INFO
```

### Comparing `sppersist-0.0.1/src/spPersist/accession_to_h5.py` & `sppersist-0.0.2/src/spPersist/accession_to_h5.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,22 +28,22 @@
               os.unlink(file_path)
           elif os.path.isdir(file_path):
               shutil.rmtree(file_path)
       except Exception as e:
           print('Failed to delete %s. Reason: %s' % (file_path, e))
 
 
-  if 'visium' not in os.listdir():
-    !mkdir visium
-  if 'h5' not in os.listdir():
-    !mkdir h5
-
   visium_path = './visium/'
   h5_path = './h5/'
 
+  if 'visium' not in os.listdir():
+    os.mkdir(visium_path)
+  if 'h5' not in os.listdir():
+    os.mkdir(h5_path)
+
   emptydir(h5_path)
 
   for sampleid in sampleids:
     emptydir(visium_path)
     
     # extract files for a given sample id to the visium foler
     tar.extractall(path=visium_path,
@@ -57,8 +57,8 @@
     
     adata = visium(gex, pos)
 
     savefilename = sampleid + '.h5'
     adata.write_h5ad(h5_path+savefilename)
   
   # zip h5 files
-  !zip -r ./h5.zip ./h5
+  shutil.make_archive('h5.zip', 'zip', h5_path)
```

### Comparing `sppersist-0.0.1/src/spPersist/visium.py` & `sppersist-0.0.2/src/spPersist/visium.py`

 * *Files identical despite different names*

### Comparing `sppersist-0.0.1/LICENSE` & `sppersist-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-0.0.1/pyproject.toml` & `sppersist-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial analysis with Persistent Homology"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sppersist-0.0.1/PKG-INFO` & `sppersist-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.0.1
+Version: 0.0.2
 Summary: Spatial analysis with Persistent Homology
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

