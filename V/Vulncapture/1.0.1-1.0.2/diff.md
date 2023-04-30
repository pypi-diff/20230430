# Comparing `tmp/Vulncapture-1.0.1.tar.gz` & `tmp/Vulncapture-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Vulncapture-1.0.1.tar", last modified: Sun Apr 30 04:05:41 2023, max compression
+gzip compressed data, was "Vulncapture-1.0.2.tar", last modified: Sun Apr 30 04:14:05 2023, max compression
```

## Comparing `Vulncapture-1.0.1.tar` & `Vulncapture-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 04:05:41.301985 Vulncapture-1.0.1/
--rw-rw-rw-   0        0        0     1091 2023-04-26 08:28:29.000000 Vulncapture-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1323 2023-04-30 04:05:41.300977 Vulncapture-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      776 2023-04-30 04:05:25.000000 Vulncapture-1.0.1/README.md
--rw-rw-rw-   0        0        0      631 2023-04-30 04:04:29.000000 Vulncapture-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 04:05:41.301985 Vulncapture-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      189 2023-04-29 17:26:11.000000 Vulncapture-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 04:05:41.280537 Vulncapture-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 04:05:41.299968 Vulncapture-1.0.1/src/Vulncapture.egg-info/
--rw-rw-rw-   0        0        0     1323 2023-04-30 04:05:41.000000 Vulncapture-1.0.1/src/Vulncapture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-04-30 04:05:41.000000 Vulncapture-1.0.1/src/Vulncapture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 04:05:41.000000 Vulncapture-1.0.1/src/Vulncapture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 04:05:41.000000 Vulncapture-1.0.1/src/Vulncapture.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 04:14:05.709710 Vulncapture-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-26 08:28:29.000000 Vulncapture-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1340 2023-04-30 04:14:05.708708 Vulncapture-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      793 2023-04-30 04:13:36.000000 Vulncapture-1.0.2/README.md
+-rw-rw-rw-   0        0        0      631 2023-04-30 04:11:46.000000 Vulncapture-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 04:14:05.709710 Vulncapture-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      189 2023-04-30 04:13:17.000000 Vulncapture-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 04:14:05.660021 Vulncapture-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 04:14:05.689561 Vulncapture-1.0.2/src/Vulncapture/
+-rw-rw-rw-   0        0        0    17839 2023-04-30 04:02:19.000000 Vulncapture-1.0.2/src/Vulncapture/Vulncapture.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:29:13.000000 Vulncapture-1.0.2/src/Vulncapture/__init__.py
+-rw-rw-rw-   0        0        0     1559 2022-11-09 05:08:38.000000 Vulncapture-1.0.2/src/Vulncapture/dialogui.png
+-rw-rw-rw-   0        0        0 15044440 2022-11-09 06:03:08.000000 Vulncapture-1.0.2/src/Vulncapture/mshei.ttf
+-rw-rw-rw-   0        0        0       28 2023-04-30 04:00:12.000000 Vulncapture-1.0.2/src/Vulncapture/requirements.txt
+-rw-rw-rw-   0        0        0     7710 2022-11-09 05:30:26.000000 Vulncapture-1.0.2/src/Vulncapture/titlegui.png
+drwxrwxrwx   0        0        0        0 2023-04-30 04:14:05.706715 Vulncapture-1.0.2/src/Vulncapture.egg-info/
+-rw-rw-rw-   0        0        0     1340 2023-04-30 04:14:05.000000 Vulncapture-1.0.2/src/Vulncapture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-04-30 04:14:05.000000 Vulncapture-1.0.2/src/Vulncapture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 04:14:05.000000 Vulncapture-1.0.2/src/Vulncapture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-30 04:14:05.000000 Vulncapture-1.0.2/src/Vulncapture.egg-info/top_level.txt
```

### Comparing `Vulncapture-1.0.1/LICENSE` & `Vulncapture-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Vulncapture-1.0.1/PKG-INFO` & `Vulncapture-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Vulncapture
-Version: 1.0.1
+Version: 1.0.2
 Summary: A capture moudle return base64 image
 Author-email: jiangyangcreate <jiangyangcreate@gamil.com>
 Project-URL: Homepage, https://github.com/jiangmiemie/Vulncapture
 Project-URL: Bug Tracker, https://github.com/jiangmiemie/Vulncapture/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 # Install
 
 pip install Vulncapture
 
 # Use
 
 ```
-import Vulncapture
+from Vulncapture import Vulncapture
 import base64
 image=Vulncapture.run_snapshot(url='http://www.baidu.com',keyword='换一换')
 '''
 run_snapshot() parmers
 url : aim url
 keyword : str
 headers : dict
```

### Comparing `Vulncapture-1.0.1/README.md` & `Vulncapture-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Install
 
 pip install Vulncapture
 
 # Use
 
 ```
-import Vulncapture
+from Vulncapture import Vulncapture
 import base64
 image=Vulncapture.run_snapshot(url='http://www.baidu.com',keyword='换一换')
 '''
 run_snapshot() parmers
 url : aim url
 keyword : str
 headers : dict
```

### Comparing `Vulncapture-1.0.1/pyproject.toml` & `Vulncapture-1.0.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Vulncapture"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="jiangyangcreate", email="jiangyangcreate@gamil.com" },
 ]
 description = "A capture moudle return base64 image"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `Vulncapture-1.0.1/src/Vulncapture.egg-info/PKG-INFO` & `Vulncapture-1.0.2/src/Vulncapture.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Vulncapture
-Version: 1.0.1
+Version: 1.0.2
 Summary: A capture moudle return base64 image
 Author-email: jiangyangcreate <jiangyangcreate@gamil.com>
 Project-URL: Homepage, https://github.com/jiangmiemie/Vulncapture
 Project-URL: Bug Tracker, https://github.com/jiangmiemie/Vulncapture/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 # Install
 
 pip install Vulncapture
 
 # Use
 
 ```
-import Vulncapture
+from Vulncapture import Vulncapture
 import base64
 image=Vulncapture.run_snapshot(url='http://www.baidu.com',keyword='换一换')
 '''
 run_snapshot() parmers
 url : aim url
 keyword : str
 headers : dict
```

