# Comparing `tmp/py-randomprime-1.9.5.tar.gz` & `tmp/py-randomprime-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/runner/work/py-randomprime/py-randomprime/dist/tmpo2sgv66c/py-randomprime-1.9.5.tar", last modified: Tue Jul 26 20:32:51 2022, max compression
+gzip compressed data, was "/Users/runner/work/py-randomprime/py-randomprime/dist/tmp026ztx87/py-randomprime-1.9.6.tar", last modified: Fri Jul 29 22:44:29 2022, max compression
```

## Comparing `py-randomprime-1.9.5.tar` & `py-randomprime-1.9.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-26 20:32:51.000000 py-randomprime-1.9.5/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-26 20:32:51.000000 py-randomprime-1.9.5/.github/
--rw-r--r--   0 runner     (501) staff       (20)      801 2022-07-26 20:24:08.000000 py-randomprime-1.9.5/.github/dependabot.yml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-26 20:32:51.000000 py-randomprime-1.9.5/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     4721 2022-07-26 20:24:08.000000 py-randomprime-1.9.5/.github/workflows/python.yml
--rw-r--r--   0 runner     (501) staff       (20)     1825 2022-07-26 20:24:08.000000 py-randomprime-1.9.5/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)      118 2022-07-26 20:24:08.000000 py-randomprime-1.9.5/.gitmodules
--rw-r--r--   0 runner     (501) staff       (20)    28108 2022-07-26 20:24:08.000000 py-randomprime-1.9.5/Cargo.lock
--rw-r--r--   0 runner     (501) staff       (20)      638 2022-07-26 20:24:08.000000 py-randomprime-1.9.5/Cargo.toml
--rw-r--r--   0 runner     (501) staff       (20)     1087 2022-07-26 20:24:08.000000 py-randomprime-1.9.5/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      699 2022-07-26 20:32:51.000000 py-randomprime-1.9.5/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      104 2022-07-26 20:24:08.000000 py-randomprime-1.9.5/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-26 20:32:51.000000 py-randomprime-1.9.5/py_randomprime/
--rw-r--r--   0 runner     (501) staff       (20)     2038 2022-07-26 20:24:08.000000 py-randomprime-1.9.5/py_randomprime/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      452 2022-07-26 20:24:08.000000 py-randomprime-1.9.5/py_randomprime/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)      176 2022-07-26 20:32:50.000000 py-randomprime-1.9.5/py_randomprime/version.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-26 20:32:51.000000 py-randomprime-1.9.5/py_randomprime.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)      699 2022-07-26 20:32:50.000000 py-randomprime-1.9.5/py_randomprime.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      449 2022-07-26 20:32:51.000000 py-randomprime-1.9.5/py_randomprime.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-07-26 20:32:50.000000 py-randomprime-1.9.5/py_randomprime.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-07-26 20:25:27.000000 py-randomprime-1.9.5/py_randomprime.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)       15 2022-07-26 20:32:50.000000 py-randomprime-1.9.5/py_randomprime.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)      246 2022-07-26 20:24:08.000000 py-randomprime-1.9.5/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)      699 2022-07-26 20:32:51.000000 py-randomprime-1.9.5/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      254 2022-07-26 20:24:08.000000 py-randomprime-1.9.5/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-26 20:32:51.000000 py-randomprime-1.9.5/src/
--rw-r--r--   0 runner     (501) staff       (20)     6405 2022-07-26 20:24:08.000000 py-randomprime-1.9.5/src/lib.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-26 20:32:51.000000 py-randomprime-1.9.5/test/
--rw-r--r--   0 runner     (501) staff       (20)      372 2022-07-26 20:24:08.000000 py-randomprime-1.9.5/test/test_library.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-29 22:44:29.000000 py-randomprime-1.9.6/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-29 22:44:29.000000 py-randomprime-1.9.6/.github/
+-rw-r--r--   0 runner     (501) staff       (20)      801 2022-07-29 22:38:13.000000 py-randomprime-1.9.6/.github/dependabot.yml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-29 22:44:29.000000 py-randomprime-1.9.6/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     4721 2022-07-29 22:38:13.000000 py-randomprime-1.9.6/.github/workflows/python.yml
+-rw-r--r--   0 runner     (501) staff       (20)     1825 2022-07-29 22:38:13.000000 py-randomprime-1.9.6/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)      118 2022-07-29 22:38:13.000000 py-randomprime-1.9.6/.gitmodules
+-rw-r--r--   0 runner     (501) staff       (20)    28108 2022-07-29 22:38:13.000000 py-randomprime-1.9.6/Cargo.lock
+-rw-r--r--   0 runner     (501) staff       (20)      638 2022-07-29 22:38:13.000000 py-randomprime-1.9.6/Cargo.toml
+-rw-r--r--   0 runner     (501) staff       (20)     1087 2022-07-29 22:38:13.000000 py-randomprime-1.9.6/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      699 2022-07-29 22:44:29.000000 py-randomprime-1.9.6/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      104 2022-07-29 22:38:13.000000 py-randomprime-1.9.6/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-29 22:44:29.000000 py-randomprime-1.9.6/py_randomprime/
+-rw-r--r--   0 runner     (501) staff       (20)     2038 2022-07-29 22:38:13.000000 py-randomprime-1.9.6/py_randomprime/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      452 2022-07-29 22:38:13.000000 py-randomprime-1.9.6/py_randomprime/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)      176 2022-07-29 22:44:29.000000 py-randomprime-1.9.6/py_randomprime/version.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-29 22:44:29.000000 py-randomprime-1.9.6/py_randomprime.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)      699 2022-07-29 22:44:29.000000 py-randomprime-1.9.6/py_randomprime.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      449 2022-07-29 22:44:29.000000 py-randomprime-1.9.6/py_randomprime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2022-07-29 22:44:29.000000 py-randomprime-1.9.6/py_randomprime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2022-07-29 22:39:19.000000 py-randomprime-1.9.6/py_randomprime.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)       15 2022-07-29 22:44:29.000000 py-randomprime-1.9.6/py_randomprime.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)      246 2022-07-29 22:38:13.000000 py-randomprime-1.9.6/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)      699 2022-07-29 22:44:29.000000 py-randomprime-1.9.6/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      254 2022-07-29 22:38:13.000000 py-randomprime-1.9.6/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-29 22:44:29.000000 py-randomprime-1.9.6/src/
+-rw-r--r--   0 runner     (501) staff       (20)     6405 2022-07-29 22:38:13.000000 py-randomprime-1.9.6/src/lib.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-29 22:44:29.000000 py-randomprime-1.9.6/test/
+-rw-r--r--   0 runner     (501) staff       (20)      372 2022-07-29 22:38:13.000000 py-randomprime-1.9.6/test/test_library.py
```

### Comparing `py-randomprime-1.9.5/.github/dependabot.yml` & `py-randomprime-1.9.6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `py-randomprime-1.9.5/.github/workflows/python.yml` & `py-randomprime-1.9.6/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `py-randomprime-1.9.5/.gitignore` & `py-randomprime-1.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `py-randomprime-1.9.5/Cargo.lock` & `py-randomprime-1.9.6/Cargo.lock`

 * *Files identical despite different names*

### Comparing `py-randomprime-1.9.5/Cargo.toml` & `py-randomprime-1.9.6/Cargo.toml`

 * *Files identical despite different names*

### Comparing `py-randomprime-1.9.5/LICENSE` & `py-randomprime-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py-randomprime-1.9.5/PKG-INFO` & `py-randomprime-1.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-randomprime
-Version: 1.9.5
+Version: 1.9.6
 Summary: A Metroid Prime 1 patcher, for randomizers and plandomizers.
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `py-randomprime-1.9.5/py_randomprime/__init__.py` & `py-randomprime-1.9.6/py_randomprime/__init__.py`

 * *Files identical despite different names*

### Comparing `py-randomprime-1.9.5/py_randomprime.egg-info/PKG-INFO` & `py-randomprime-1.9.6/py_randomprime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-randomprime
-Version: 1.9.5
+Version: 1.9.6
 Summary: A Metroid Prime 1 patcher, for randomizers and plandomizers.
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `py-randomprime-1.9.5/setup.cfg` & `py-randomprime-1.9.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `py-randomprime-1.9.5/src/lib.rs` & `py-randomprime-1.9.6/src/lib.rs`

 * *Files identical despite different names*

