# Comparing `tmp/ssl-labs-screenshot-1.0.4.tar.gz` & `tmp/ssl-labs-screenshot-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssl-labs-screenshot-1.0.4.tar", last modified: Sun Apr 30 21:30:20 2023, max compression
+gzip compressed data, was "ssl-labs-screenshot-1.0.5.tar", last modified: Sun Apr 30 21:33:51 2023, max compression
```

## Comparing `ssl-labs-screenshot-1.0.4.tar` & `ssl-labs-screenshot-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 21:30:20.634317 ssl-labs-screenshot-1.0.4/
--rw-r--r--   0 mark       (501) staff       (20)     1068 2023-04-30 18:51:38.000000 ssl-labs-screenshot-1.0.4/LICENSE.txt
--rw-r--r--   0 mark       (501) staff       (20)       24 2023-04-30 20:06:51.000000 ssl-labs-screenshot-1.0.4/MANIFEST.in
--rw-r--r--   0 mark       (501) staff       (20)     2056 2023-04-30 21:30:20.634203 ssl-labs-screenshot-1.0.4/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     1331 2023-04-30 21:30:06.000000 ssl-labs-screenshot-1.0.4/README.md
--rw-r--r--   0 mark       (501) staff       (20)       56 2023-04-30 20:02:02.000000 ssl-labs-screenshot-1.0.4/pyproject.toml
--rw-r--r--   0 mark       (501) staff       (20)       31 2023-04-30 18:30:24.000000 ssl-labs-screenshot-1.0.4/requirements.txt
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-30 21:30:20.634358 ssl-labs-screenshot-1.0.4/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1270 2023-04-30 21:29:45.000000 ssl-labs-screenshot-1.0.4/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 21:30:20.633320 ssl-labs-screenshot-1.0.4/ssl_labs_screenshot/
--rw-r--r--   0 mark       (501) staff       (20)        0 2023-04-30 18:53:22.000000 ssl-labs-screenshot-1.0.4/ssl_labs_screenshot/__init__.py
--rwxr-xr-x   0 mark       (501) staff       (20)     4104 2023-04-29 01:32:27.000000 ssl-labs-screenshot-1.0.4/ssl_labs_screenshot/__main__.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 21:30:20.634056 ssl-labs-screenshot-1.0.4/ssl_labs_screenshot.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)     2056 2023-04-30 21:30:20.000000 ssl-labs-screenshot-1.0.4/ssl_labs_screenshot.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      398 2023-04-30 21:30:20.000000 ssl-labs-screenshot-1.0.4/ssl_labs_screenshot.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-30 21:30:20.000000 ssl-labs-screenshot-1.0.4/ssl_labs_screenshot.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)       74 2023-04-30 21:30:20.000000 ssl-labs-screenshot-1.0.4/ssl_labs_screenshot.egg-info/entry_points.txt
--rw-r--r--   0 mark       (501) staff       (20)       32 2023-04-30 21:30:20.000000 ssl-labs-screenshot-1.0.4/ssl_labs_screenshot.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)       20 2023-04-30 21:30:20.000000 ssl-labs-screenshot-1.0.4/ssl_labs_screenshot.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 21:33:51.736444 ssl-labs-screenshot-1.0.5/
+-rw-r--r--   0 mark       (501) staff       (20)     1068 2023-04-30 18:51:38.000000 ssl-labs-screenshot-1.0.5/LICENSE.txt
+-rw-r--r--   0 mark       (501) staff       (20)       24 2023-04-30 20:06:51.000000 ssl-labs-screenshot-1.0.5/MANIFEST.in
+-rw-r--r--   0 mark       (501) staff       (20)     2065 2023-04-30 21:33:51.736302 ssl-labs-screenshot-1.0.5/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     1340 2023-04-30 21:33:41.000000 ssl-labs-screenshot-1.0.5/README.md
+-rw-r--r--   0 mark       (501) staff       (20)       56 2023-04-30 20:02:02.000000 ssl-labs-screenshot-1.0.5/pyproject.toml
+-rw-r--r--   0 mark       (501) staff       (20)       31 2023-04-30 18:30:24.000000 ssl-labs-screenshot-1.0.5/requirements.txt
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-30 21:33:51.736481 ssl-labs-screenshot-1.0.5/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1270 2023-04-30 21:33:24.000000 ssl-labs-screenshot-1.0.5/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 21:33:51.731411 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot/
+-rw-r--r--   0 mark       (501) staff       (20)        0 2023-04-30 18:53:22.000000 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot/__init__.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     4104 2023-04-29 01:32:27.000000 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot/__main__.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 21:33:51.736131 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)     2065 2023-04-30 21:33:51.000000 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      398 2023-04-30 21:33:51.000000 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-30 21:33:51.000000 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)       74 2023-04-30 21:33:51.000000 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot.egg-info/entry_points.txt
+-rw-r--r--   0 mark       (501) staff       (20)       32 2023-04-30 21:33:51.000000 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot.egg-info/requires.txt
+-rw-r--r--   0 mark       (501) staff       (20)       20 2023-04-30 21:33:51.000000 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot.egg-info/top_level.txt
```

### Comparing `ssl-labs-screenshot-1.0.4/LICENSE.txt` & `ssl-labs-screenshot-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssl-labs-screenshot-1.0.4/PKG-INFO` & `ssl-labs-screenshot-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssl-labs-screenshot
-Version: 1.0.4
+Version: 1.0.5
 Summary: A script to capture SSL Labs server test report screenshots
 Home-page: https://github.com/marksowell/ssl-labs-screenshot
 Author: Mark Sowell
 Author-email: mark@marksowell.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -22,17 +22,17 @@
 ## Requirements
 - Python 3.x
 - Chrome browser (version 89 or later)
 - ChromeDriver
 
 ## Installation
 1. Install SSL Labs Screenshot using pip:
-```
-pip install ssl-labs-screenshot
-```
+   ```
+   pip install ssl-labs-screenshot
+   ```
 3. Download the latest version of ChromeDriver from the following link: https://sites.google.com/chromium.org/driver/downloads
 4. Extract the contents of the downloaded ZIP file to a directory on your system.
 5. Either move the ChromeDriver executable to a directory already in your system's `PATH` environment variable or add the path to the directory where you extracted the ChromeDriver executable to the `PATH` variable.
 
 ## Usage
 Run the script with the following command:
 ```
```

### Comparing `ssl-labs-screenshot-1.0.4/README.md` & `ssl-labs-screenshot-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 ## Requirements
 - Python 3.x
 - Chrome browser (version 89 or later)
 - ChromeDriver
 
 ## Installation
 1. Install SSL Labs Screenshot using pip:
-```
-pip install ssl-labs-screenshot
-```
+   ```
+   pip install ssl-labs-screenshot
+   ```
 3. Download the latest version of ChromeDriver from the following link: https://sites.google.com/chromium.org/driver/downloads
 4. Extract the contents of the downloaded ZIP file to a directory on your system.
 5. Either move the ChromeDriver executable to a directory already in your system's `PATH` environment variable or add the path to the directory where you extracted the ChromeDriver executable to the `PATH` variable.
 
 ## Usage
 Run the script with the following command:
 ```
```

### Comparing `ssl-labs-screenshot-1.0.4/setup.py` & `ssl-labs-screenshot-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, "requirements.txt"), "r") as fh:
     requirements = fh.read().splitlines()
 
 setup(
     name="ssl-labs-screenshot",
-    version="1.0.4",
+    version="1.0.5",
     author="Mark Sowell",
     author_email="mark@marksowell.com",
     description="A script to capture SSL Labs server test report screenshots",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/marksowell/ssl-labs-screenshot",
     packages=find_packages(),
```

### Comparing `ssl-labs-screenshot-1.0.4/ssl_labs_screenshot/__main__.py` & `ssl-labs-screenshot-1.0.5/ssl_labs_screenshot/__main__.py`

 * *Files identical despite different names*

### Comparing `ssl-labs-screenshot-1.0.4/ssl_labs_screenshot.egg-info/PKG-INFO` & `ssl-labs-screenshot-1.0.5/ssl_labs_screenshot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssl-labs-screenshot
-Version: 1.0.4
+Version: 1.0.5
 Summary: A script to capture SSL Labs server test report screenshots
 Home-page: https://github.com/marksowell/ssl-labs-screenshot
 Author: Mark Sowell
 Author-email: mark@marksowell.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -22,17 +22,17 @@
 ## Requirements
 - Python 3.x
 - Chrome browser (version 89 or later)
 - ChromeDriver
 
 ## Installation
 1. Install SSL Labs Screenshot using pip:
-```
-pip install ssl-labs-screenshot
-```
+   ```
+   pip install ssl-labs-screenshot
+   ```
 3. Download the latest version of ChromeDriver from the following link: https://sites.google.com/chromium.org/driver/downloads
 4. Extract the contents of the downloaded ZIP file to a directory on your system.
 5. Either move the ChromeDriver executable to a directory already in your system's `PATH` environment variable or add the path to the directory where you extracted the ChromeDriver executable to the `PATH` variable.
 
 ## Usage
 Run the script with the following command:
 ```
```

