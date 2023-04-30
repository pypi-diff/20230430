# Comparing `tmp/BingImageCreator-0.1.3.tar.gz` & `tmp/BingImageCreator-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BingImageCreator-0.1.3.tar", last modified: Fri Apr 21 10:17:24 2023, max compression
+gzip compressed data, was "BingImageCreator-0.1.4.tar", last modified: Sun Apr 30 03:29:37 2023, max compression
```

## Comparing `BingImageCreator-0.1.3.tar` & `BingImageCreator-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:17:24.157638 BingImageCreator-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-21 10:17:02.000000 BingImageCreator-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-21 10:17:24.157638 BingImageCreator-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-21 10:17:02.000000 BingImageCreator-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-21 10:17:24.157638 BingImageCreator-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-21 10:17:02.000000 BingImageCreator-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:17:24.153638 BingImageCreator-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:17:24.157638 BingImageCreator-0.1.3/src/BingImageCreator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-21 10:17:24.000000 BingImageCreator-0.1.3/src/BingImageCreator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-21 10:17:24.000000 BingImageCreator-0.1.3/src/BingImageCreator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:17:24.000000 BingImageCreator-0.1.3/src/BingImageCreator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 10:17:24.000000 BingImageCreator-0.1.3/src/BingImageCreator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 10:17:24.000000 BingImageCreator-0.1.3/src/BingImageCreator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-04-21 10:17:02.000000 BingImageCreator-0.1.3/src/BingImageCreator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:29:37.427073 BingImageCreator-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-30 03:29:14.000000 BingImageCreator-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-30 03:29:37.427073 BingImageCreator-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-30 03:29:14.000000 BingImageCreator-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-30 03:29:37.427073 BingImageCreator-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-30 03:29:14.000000 BingImageCreator-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:29:37.423073 BingImageCreator-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:29:37.427073 BingImageCreator-0.1.4/src/BingImageCreator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-30 03:29:37.000000 BingImageCreator-0.1.4/src/BingImageCreator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-30 03:29:37.000000 BingImageCreator-0.1.4/src/BingImageCreator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 03:29:37.000000 BingImageCreator-0.1.4/src/BingImageCreator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-30 03:29:37.000000 BingImageCreator-0.1.4/src/BingImageCreator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 03:29:37.000000 BingImageCreator-0.1.4/src/BingImageCreator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14144 2023-04-30 03:29:14.000000 BingImageCreator-0.1.4/src/BingImageCreator.py
```

### Comparing `BingImageCreator-0.1.3/LICENSE` & `BingImageCreator-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.1.3/PKG-INFO` & `BingImageCreator-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.1.3
+Version: 0.1.4
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.1.3/README.md` & `BingImageCreator-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.1.3/setup.py` & `BingImageCreator-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="BingImageCreator",
-    version="0.1.3",
+    version="0.1.4",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="High quality image generation by Microsoft. Reverse engineered API.",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/BingImageCreator",
```

### Comparing `BingImageCreator-0.1.3/src/BingImageCreator.egg-info/PKG-INFO` & `BingImageCreator-0.1.4/src/BingImageCreator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.1.3
+Version: 0.1.4
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.1.3/src/BingImageCreator.py` & `BingImageCreator-0.1.4/src/BingImageCreator.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 import sys
 import time
 import aiohttp
 import pkg_resources
 import regex
 import requests
 from typing import Union
-if(os.environ.get('BING_URL') == None):
+
+if os.environ.get("BING_URL") == None:
     BING_URL = "https://www.bing.com"
 else:
-    BING_URL = os.environ.get('BING_URL')
+    BING_URL = os.environ.get("BING_URL")
 # Generate random IP between range 13.104.0.0/14
 FORWARDED_IP = (
     f"13.{random.randint(104, 107)}.{random.randint(0, 255)}.{random.randint(0, 255)}"
 )
 HEADERS = {
     "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
     "accept-language": "en-US,en;q=0.9",
@@ -141,21 +142,22 @@
         # Use regex to search for src=""
         image_links = regex.findall(r'src="([^"]+)"', response.text)
         # Remove size limit
         normal_image_links = [link.split("?w=")[0] for link in image_links]
         # Remove duplicates
         normal_image_links = list(set(normal_image_links))
 
-        # bad_images = [
-        #     "https://r.bing.com/rp/in-2zU3AJUdkgFe7ZKv19yPBHVs.png",
-        #     "https://r.bing.com/rp/TX9QuO3WzcCJz1uaaSwQAz39Kb0.jpg",
-        # ]
-        # for img in normal_image_links:
-        #     if img in bad_images:
-        #         raise Exception("Bad images")
+        # Bad images
+        bad_images = [
+            "https://r.bing.com/rp/in-2zU3AJUdkgFe7ZKv19yPBHVs.png",
+            "https://r.bing.com/rp/TX9QuO3WzcCJz1uaaSwQAz39Kb0.jpg",
+        ]
+        for img in normal_image_links:
+            if img in bad_images:
+                raise Exception("Bad images")
         # No images
         if not normal_image_links:
             raise Exception(error_no_images)
         return normal_image_links
 
     def save_images(self, links: list, output_dir: str) -> None:
         """
@@ -231,15 +233,15 @@
                 )
                 async with self.session.post(
                     url,
                     allow_redirects=False,
                     timeout=200,
                 ) as response3:
                     if response3.status != 302:
-                        print(f"ERROR: {response3.text}")
+                        print(f"ERROR: {await response3.text()}")
                         raise Exception("Redirect failed")
                     response = response3
         # Get redirect URL
         redirect_url = response.headers["Location"].replace("&nfy=1", "")
         request_id = redirect_url.split("id=")[-1]
         await self.session.get(f"{BING_URL}{redirect_url}")
         # https://www.bing.com/images/create/async/results/{ID}?q={PROMPT}
```

