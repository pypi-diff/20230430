# Comparing `tmp/ssl-labs-screenshot-1.0.1.tar.gz` & `tmp/ssl-labs-screenshot-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssl-labs-screenshot-1.0.1.tar", last modified: Sun Apr 30 18:59:06 2023, max compression
+gzip compressed data, was "ssl-labs-screenshot-1.0.2.tar", last modified: Sun Apr 30 20:13:28 2023, max compression
```

## Comparing `ssl-labs-screenshot-1.0.1.tar` & `ssl-labs-screenshot-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 18:59:06.398779 ssl-labs-screenshot-1.0.1/
--rw-r--r--   0 mark       (501) staff       (20)     1068 2023-04-30 18:51:38.000000 ssl-labs-screenshot-1.0.1/LICENSE.txt
--rw-r--r--   0 mark       (501) staff       (20)     2445 2023-04-30 18:59:06.398640 ssl-labs-screenshot-1.0.1/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     1721 2023-04-30 18:50:26.000000 ssl-labs-screenshot-1.0.1/README.md
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-30 18:59:06.398821 ssl-labs-screenshot-1.0.1/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1190 2023-04-30 18:54:34.000000 ssl-labs-screenshot-1.0.1/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 18:59:06.397658 ssl-labs-screenshot-1.0.1/ssl_labs_screenshot/
--rw-r--r--   0 mark       (501) staff       (20)        0 2023-04-30 18:53:22.000000 ssl-labs-screenshot-1.0.1/ssl_labs_screenshot/__init__.py
--rwxr-xr-x   0 mark       (501) staff       (20)     4104 2023-04-29 01:32:27.000000 ssl-labs-screenshot-1.0.1/ssl_labs_screenshot/__main__.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 18:59:06.398456 ssl-labs-screenshot-1.0.1/ssl_labs_screenshot.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)     2445 2023-04-30 18:59:06.000000 ssl-labs-screenshot-1.0.1/ssl_labs_screenshot.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      354 2023-04-30 18:59:06.000000 ssl-labs-screenshot-1.0.1/ssl_labs_screenshot.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-30 18:59:06.000000 ssl-labs-screenshot-1.0.1/ssl_labs_screenshot.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)       74 2023-04-30 18:59:06.000000 ssl-labs-screenshot-1.0.1/ssl_labs_screenshot.egg-info/entry_points.txt
--rw-r--r--   0 mark       (501) staff       (20)       32 2023-04-30 18:59:06.000000 ssl-labs-screenshot-1.0.1/ssl_labs_screenshot.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)       20 2023-04-30 18:59:06.000000 ssl-labs-screenshot-1.0.1/ssl_labs_screenshot.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 20:13:28.421608 ssl-labs-screenshot-1.0.2/
+-rw-r--r--   0 mark       (501) staff       (20)     1068 2023-04-30 18:51:38.000000 ssl-labs-screenshot-1.0.2/LICENSE.txt
+-rw-r--r--   0 mark       (501) staff       (20)       24 2023-04-30 20:06:51.000000 ssl-labs-screenshot-1.0.2/MANIFEST.in
+-rw-r--r--   0 mark       (501) staff       (20)     2445 2023-04-30 20:13:28.421470 ssl-labs-screenshot-1.0.2/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     1721 2023-04-30 18:50:26.000000 ssl-labs-screenshot-1.0.2/README.md
+-rw-r--r--   0 mark       (501) staff       (20)       56 2023-04-30 20:02:02.000000 ssl-labs-screenshot-1.0.2/pyproject.toml
+-rw-r--r--   0 mark       (501) staff       (20)       31 2023-04-30 18:30:24.000000 ssl-labs-screenshot-1.0.2/requirements.txt
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-30 20:13:28.421644 ssl-labs-screenshot-1.0.2/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1270 2023-04-30 20:12:00.000000 ssl-labs-screenshot-1.0.2/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 20:13:28.413117 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot/
+-rw-r--r--   0 mark       (501) staff       (20)        0 2023-04-30 18:53:22.000000 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot/__init__.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     4104 2023-04-29 01:32:27.000000 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot/__main__.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 20:13:28.421296 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)     2445 2023-04-30 20:13:28.000000 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      398 2023-04-30 20:13:28.000000 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-30 20:13:28.000000 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)       74 2023-04-30 20:13:28.000000 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot.egg-info/entry_points.txt
+-rw-r--r--   0 mark       (501) staff       (20)       32 2023-04-30 20:13:28.000000 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot.egg-info/requires.txt
+-rw-r--r--   0 mark       (501) staff       (20)       20 2023-04-30 20:13:28.000000 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot.egg-info/top_level.txt
```

### Comparing `ssl-labs-screenshot-1.0.1/LICENSE.txt` & `ssl-labs-screenshot-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssl-labs-screenshot-1.0.1/PKG-INFO` & `ssl-labs-screenshot-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssl-labs-screenshot
-Version: 1.0.1
+Version: 1.0.2
 Summary: A script to capture SSL Labs server test report screenshots
 Home-page: https://github.com/marksowell/ssl-labs-screenshot
 Author: Mark Sowell
 Author-email: mark@marksowell.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssl-labs-screenshot-1.0.1/README.md` & `ssl-labs-screenshot-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ssl-labs-screenshot-1.0.1/setup.py` & `ssl-labs-screenshot-1.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from setuptools import setup, find_packages
+import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-with open("requirements.txt", "r") as fh:
+here = os.path.abspath(os.path.dirname(__file__))
+with open(os.path.join(here, "requirements.txt"), "r") as fh:
     requirements = fh.read().splitlines()
 
 setup(
     name="ssl-labs-screenshot",
-    version="1.0.1",
+    version="1.0.2",
     author="Mark Sowell",
     author_email="mark@marksowell.com",
     description="A script to capture SSL Labs server test report screenshots",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/marksowell/ssl-labs-screenshot",
     packages=find_packages(),
```

### Comparing `ssl-labs-screenshot-1.0.1/ssl_labs_screenshot/__main__.py` & `ssl-labs-screenshot-1.0.2/ssl_labs_screenshot/__main__.py`

 * *Files identical despite different names*

### Comparing `ssl-labs-screenshot-1.0.1/ssl_labs_screenshot.egg-info/PKG-INFO` & `ssl-labs-screenshot-1.0.2/ssl_labs_screenshot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssl-labs-screenshot
-Version: 1.0.1
+Version: 1.0.2
 Summary: A script to capture SSL Labs server test report screenshots
 Home-page: https://github.com/marksowell/ssl-labs-screenshot
 Author: Mark Sowell
 Author-email: mark@marksowell.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

