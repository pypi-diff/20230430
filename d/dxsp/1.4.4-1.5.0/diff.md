# Comparing `tmp/dxsp-1.4.4.tar.gz` & `tmp/dxsp-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.4.4.tar", max compression
+gzip compressed data, was "dxsp-1.5.0.tar", max compression
```

## Comparing `dxsp-1.4.4.tar` & `dxsp-1.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-04-30 18:59:27.426097 dxsp-1.4.4/LICENSE
--rw-r--r--   0        0        0     3225 2023-04-30 18:59:27.426097 dxsp-1.4.4/README.md
--rw-r--r--   0        0        0       38 2023-04-30 18:59:27.426097 dxsp-1.4.4/dxsp/.gitignore
--rw-r--r--   0        0        0      169 2023-04-30 18:59:28.206128 dxsp-1.4.4/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-30 18:59:27.426097 dxsp-1.4.4/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-04-30 18:59:27.426097 dxsp-1.4.4/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      392 2023-04-30 18:59:27.426097 dxsp-1.4.4/dxsp/config.py
--rw-r--r--   0        0        0      564 2023-04-30 18:59:27.426097 dxsp-1.4.4/dxsp/default_settings.toml
--rw-r--r--   0        0        0    28465 2023-04-30 18:59:27.426097 dxsp-1.4.4/dxsp/main.py
--rw-r--r--   0        0        0     1015 2023-04-30 18:59:28.206128 dxsp-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 dxsp-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-30 19:15:08.567402 dxsp-1.5.0/LICENSE
+-rw-r--r--   0        0        0     3225 2023-04-30 19:15:08.567402 dxsp-1.5.0/README.md
+-rw-r--r--   0        0        0       38 2023-04-30 19:15:08.567402 dxsp-1.5.0/dxsp/.gitignore
+-rw-r--r--   0        0        0      169 2023-04-30 19:15:09.539409 dxsp-1.5.0/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-30 19:15:08.567402 dxsp-1.5.0/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-04-30 19:15:08.567402 dxsp-1.5.0/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      392 2023-04-30 19:15:08.567402 dxsp-1.5.0/dxsp/config.py
+-rw-r--r--   0        0        0      564 2023-04-30 19:15:08.567402 dxsp-1.5.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    28465 2023-04-30 19:15:08.567402 dxsp-1.5.0/dxsp/main.py
+-rw-r--r--   0        0        0     1015 2023-04-30 19:15:09.539409 dxsp-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 dxsp-1.5.0/PKG-INFO
```

### Comparing `dxsp-1.4.4/LICENSE` & `dxsp-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.4.4/README.md` & `dxsp-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.4.4/dxsp/assets/blockchains.py` & `dxsp-1.5.0/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.4.4/dxsp/default_settings.toml` & `dxsp-1.5.0/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-1.4.4/dxsp/main.py` & `dxsp-1.5.0/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.4.4/pyproject.toml` & `dxsp-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.4.4"
+version = "1.5.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-1.4.4/PKG-INFO` & `dxsp-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.4.4
+Version: 1.5.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

