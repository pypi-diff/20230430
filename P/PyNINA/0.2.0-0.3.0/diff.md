# Comparing `tmp/PyNINA-0.2.0.tar.gz` & `tmp/PyNINA-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNINA-0.2.0.tar", last modified: Thu Dec  8 20:28:03 2022, max compression
+gzip compressed data, was "PyNINA-0.3.0.tar", last modified: Sun Apr 30 11:38:04 2023, max compression
```

## Comparing `PyNINA-0.2.0.tar` & `PyNINA-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-12-08 20:28:03.888248 PyNINA-0.2.0/
--rw-rw-rw-   0        0        0     1087 2021-08-31 18:45:53.000000 PyNINA-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     2120 2022-12-08 20:28:03.887226 PyNINA-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-12-08 20:28:03.876496 PyNINA-0.2.0/PyNINA.egg-info/
--rw-rw-rw-   0        0        0     2120 2022-12-08 20:28:03.000000 PyNINA-0.2.0/PyNINA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2022-12-08 20:28:03.000000 PyNINA-0.2.0/PyNINA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-08 20:28:03.000000 PyNINA-0.2.0/PyNINA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2022-12-08 20:28:03.000000 PyNINA-0.2.0/PyNINA.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-12-08 20:28:03.000000 PyNINA-0.2.0/PyNINA.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      552 2021-09-11 21:30:24.000000 PyNINA-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2022-12-08 20:28:03.885631 PyNINA-0.2.0/pynina/
--rw-rw-rw-   0        0        0      138 2022-12-08 20:26:58.000000 PyNINA-0.2.0/pynina/__init__.py
--rw-rw-rw-   0        0        0     1342 2022-02-07 18:49:23.000000 PyNINA-0.2.0/pynina/baseApi.py
--rw-rw-rw-   0        0        0    15135 2022-12-08 20:25:43.000000 PyNINA-0.2.0/pynina/const.py
--rw-rw-rw-   0        0        0      696 2022-12-08 20:25:43.000000 PyNINA-0.2.0/pynina/label_matcher.py
--rw-rw-rw-   0        0        0     2143 2022-12-08 20:25:43.000000 PyNINA-0.2.0/pynina/nina.py
--rw-rw-rw-   0        0        0     2434 2022-12-08 20:25:43.000000 PyNINA-0.2.0/pynina/warning.py
--rw-rw-rw-   0        0        0       42 2022-12-08 20:28:03.888294 PyNINA-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      585 2022-12-08 20:26:58.000000 PyNINA-0.2.0/setup.py
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-04-30 11:38:04.448151 PyNINA-0.3.0/
+-rwxrwxrwx   0 user      (1000) user      (1000)     1087 2021-08-31 18:45:53.000000 PyNINA-0.3.0/LICENSE
+-rwxrwxrwx   0 user      (1000) user      (1000)     2061 2023-04-30 11:38:04.444534 PyNINA-0.3.0/PKG-INFO
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-04-30 11:38:04.253357 PyNINA-0.3.0/PyNINA.egg-info/
+-rwxrwxrwx   0 user      (1000) user      (1000)     2061 2023-04-30 11:38:03.000000 PyNINA-0.3.0/PyNINA.egg-info/PKG-INFO
+-rwxrwxrwx   0 user      (1000) user      (1000)      285 2023-04-30 11:38:04.000000 PyNINA-0.3.0/PyNINA.egg-info/SOURCES.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        1 2023-04-30 11:38:03.000000 PyNINA-0.3.0/PyNINA.egg-info/dependency_links.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)       15 2023-04-30 11:38:03.000000 PyNINA-0.3.0/PyNINA.egg-info/requires.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        7 2023-04-30 11:38:03.000000 PyNINA-0.3.0/PyNINA.egg-info/top_level.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)      552 2021-09-11 21:30:24.000000 PyNINA-0.3.0/README.md
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-04-30 11:38:04.413967 PyNINA-0.3.0/pynina/
+-rwxrwxrwx   0 user      (1000) user      (1000)      138 2023-04-30 11:36:00.000000 PyNINA-0.3.0/pynina/__init__.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1431 2023-04-30 11:34:43.000000 PyNINA-0.3.0/pynina/baseApi.py
+-rwxrwxrwx   0 user      (1000) user      (1000)    15135 2023-04-30 11:32:16.000000 PyNINA-0.3.0/pynina/const.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      696 2022-12-08 20:25:43.000000 PyNINA-0.3.0/pynina/label_matcher.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     2143 2022-12-08 20:25:43.000000 PyNINA-0.3.0/pynina/nina.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     2434 2022-12-08 20:25:43.000000 PyNINA-0.3.0/pynina/warning.py
+-rwxrwxrwx   0 user      (1000) user      (1000)       38 2023-04-30 11:38:04.449874 PyNINA-0.3.0/setup.cfg
+-rwxrwxrwx   0 user      (1000) user      (1000)      585 2023-04-30 11:35:19.000000 PyNINA-0.3.0/setup.py
```

### Comparing `PyNINA-0.2.0/LICENSE` & `PyNINA-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNINA-0.2.0/README.md` & `PyNINA-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `PyNINA-0.2.0/pynina/baseApi.py` & `PyNINA-0.3.0/pynina/baseApi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import asyncio
 from typing import Any, Dict
 
-from aiohttp import ClientSession, ClientConnectionError
+from aiohttp import ClientSession, ClientConnectionError, ClientTimeout
 
 
 class BaseAPI:
     """Class to perform CMI API requests"""
 
     def __init__(self, session: ClientSession = None):
         """Constructor for BaseAPI."""
@@ -14,28 +15,28 @@
         """Retrieve data from API."""
         internalSession: bool = False
         if self.session is None:
             internalSession = True
             self.session = ClientSession()
 
         try:
-            async with self.session.get(url) as res:
+            async with self.session.get(url, timeout=ClientTimeout(total=9)) as res:
                 if res.status != 200:
                     raise ApiError(f"Invalid response: {res.status}")
 
                 json: Dict[str, Any] = await res.json()
                 if internalSession:
                     await self.session.close()
                     self.session = None
                 return json
-        except ClientConnectionError:
+        except (ClientConnectionError, asyncio.TimeoutError):
             if internalSession:
                 await self.session.close()
                 self.session = None
-            raise ApiError(f"Could not connect to Api")
+            raise ApiError(f"Could not connect to {url}")
 
 
 class ApiError(Exception):
     """Raised when API request ended in error."""
 
     def __init__(self, status: str):
         """Initialize."""
```

### Comparing `PyNINA-0.2.0/pynina/const.py` & `PyNINA-0.3.0/pynina/const.py`

 * *Files identical despite different names*

### Comparing `PyNINA-0.2.0/pynina/label_matcher.py` & `PyNINA-0.3.0/pynina/label_matcher.py`

 * *Files identical despite different names*

### Comparing `PyNINA-0.2.0/pynina/nina.py` & `PyNINA-0.3.0/pynina/nina.py`

 * *Files identical despite different names*

### Comparing `PyNINA-0.2.0/pynina/warning.py` & `PyNINA-0.3.0/pynina/warning.py`

 * *Files identical despite different names*

### Comparing `PyNINA-0.2.0/setup.py` & `PyNINA-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = f.read()
 
 with open("LICENSE", "r") as f:
     license = f.read()
 
 setup(
     name="PyNINA",
-    version="0.2.0",
+    version="0.3.0",
     description="A Python API wrapper to retrieve warnings from the german NINA app.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/DeerMaximum/pynina",
     author="DeerMaximum",
     author_email="git983456@parabelmail.de",
     license=license,
```

