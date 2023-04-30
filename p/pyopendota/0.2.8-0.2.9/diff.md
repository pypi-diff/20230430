# Comparing `tmp/pyopendota-0.2.8.tar.gz` & `tmp/pyopendota-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopendota-0.2.8.tar", last modified: Mon Aug 22 10:42:03 2022, max compression
+gzip compressed data, was "pyopendota-0.2.9.tar", last modified: Sun Apr 30 06:04:54 2023, max compression
```

## Comparing `pyopendota-0.2.8.tar` & `pyopendota-0.2.9.tar`

### file list

```diff
@@ -1,38 +1,44 @@
-drwxrwxr-x   0 hrishirt  (1000) hrishirt  (1000)        0 2022-08-22 10:42:03.547455 pyopendota-0.2.8/
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      172 2022-08-04 16:47:39.000000 pyopendota-0.2.8/AUTHORS.rst
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)     3562 2022-08-04 16:47:39.000000 pyopendota-0.2.8/CONTRIBUTING.rst
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      245 2022-08-04 16:47:39.000000 pyopendota-0.2.8/HISTORY.rst
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)     1079 2022-08-04 16:47:39.000000 pyopendota-0.2.8/LICENSE
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      262 2022-08-04 16:47:39.000000 pyopendota-0.2.8/MANIFEST.in
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)     4732 2022-08-22 10:42:03.547455 pyopendota-0.2.8/PKG-INFO
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)     3541 2022-08-04 16:47:39.000000 pyopendota-0.2.8/README.rst
-drwxrwxr-x   0 hrishirt  (1000) hrishirt  (1000)        0 2022-08-22 10:42:03.547455 pyopendota-0.2.8/docs/
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      611 2022-08-04 16:47:39.000000 pyopendota-0.2.8/docs/Makefile
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       28 2022-08-04 16:47:39.000000 pyopendota-0.2.8/docs/authors.rst
--rwxrwxr-x   0 hrishirt  (1000) hrishirt  (1000)     5228 2022-08-04 16:47:39.000000 pyopendota-0.2.8/docs/conf.py
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       33 2022-08-04 16:47:39.000000 pyopendota-0.2.8/docs/contributing.rst
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       28 2022-08-04 16:47:39.000000 pyopendota-0.2.8/docs/history.rst
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)     2288 2022-08-04 16:47:39.000000 pyopendota-0.2.8/docs/index.rst
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)     1169 2022-08-04 16:47:39.000000 pyopendota-0.2.8/docs/installation.rst
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      770 2022-08-04 16:47:39.000000 pyopendota-0.2.8/docs/make.bat
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       61 2022-08-04 16:47:39.000000 pyopendota-0.2.8/docs/modules.rst
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      435 2022-08-04 16:47:39.000000 pyopendota-0.2.8/docs/opendota.rst
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       27 2022-08-04 16:47:39.000000 pyopendota-0.2.8/docs/readme.rst
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       26 2022-08-04 16:47:39.000000 pyopendota-0.2.8/docs/usage.rst
-drwxrwxr-x   0 hrishirt  (1000) hrishirt  (1000)        0 2022-08-22 10:42:03.547455 pyopendota-0.2.8/opendota/
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      246 2022-08-22 10:41:57.000000 pyopendota-0.2.8/opendota/__init__.py
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      551 2022-08-04 16:47:39.000000 pyopendota-0.2.8/opendota/cli.py
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)    26146 2022-08-22 10:37:08.000000 pyopendota-0.2.8/opendota/opendota.py
-drwxrwxr-x   0 hrishirt  (1000) hrishirt  (1000)        0 2022-08-22 10:42:03.547455 pyopendota-0.2.8/pyopendota.egg-info/
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)     4732 2022-08-22 10:42:02.000000 pyopendota-0.2.8/pyopendota.egg-info/PKG-INFO
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      628 2022-08-22 10:42:03.000000 pyopendota-0.2.8/pyopendota.egg-info/SOURCES.txt
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)        1 2022-08-22 10:42:02.000000 pyopendota-0.2.8/pyopendota.egg-info/dependency_links.txt
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       47 2022-08-22 10:42:02.000000 pyopendota-0.2.8/pyopendota.egg-info/entry_points.txt
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)        1 2022-08-22 10:42:02.000000 pyopendota-0.2.8/pyopendota.egg-info/not-zip-safe
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       14 2022-08-22 10:42:03.000000 pyopendota-0.2.8/pyopendota.egg-info/requires.txt
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)        9 2022-08-22 10:42:03.000000 pyopendota-0.2.8/pyopendota.egg-info/top_level.txt
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      425 2022-08-22 10:42:03.547455 pyopendota-0.2.8/setup.cfg
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)     1610 2022-08-22 10:41:57.000000 pyopendota-0.2.8/setup.py
-drwxrwxr-x   0 hrishirt  (1000) hrishirt  (1000)        0 2022-08-22 10:42:03.547455 pyopendota-0.2.8/tests/
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       40 2022-08-04 16:47:39.000000 pyopendota-0.2.8/tests/__init__.py
--rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      556 2022-08-04 16:47:39.000000 pyopendota-0.2.8/tests/test_opendota.py
+drwxrwxr-x   0 hrishirt  (1000) hrishirt  (1000)        0 2023-04-30 06:04:54.433691 pyopendota-0.2.9/
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      172 2021-07-20 06:43:05.000000 pyopendota-0.2.9/AUTHORS.rst
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)     3562 2021-07-20 09:34:27.000000 pyopendota-0.2.9/CONTRIBUTING.rst
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      245 2022-03-04 08:54:59.000000 pyopendota-0.2.9/HISTORY.rst
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)     1079 2021-07-20 06:43:05.000000 pyopendota-0.2.9/LICENSE
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      262 2021-07-20 06:43:05.000000 pyopendota-0.2.9/MANIFEST.in
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)     4712 2023-04-30 06:04:54.433691 pyopendota-0.2.9/PKG-INFO
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)     3541 2022-03-04 09:13:15.000000 pyopendota-0.2.9/README.rst
+drwxrwxr-x   0 hrishirt  (1000) hrishirt  (1000)        0 2023-04-30 06:04:53.961686 pyopendota-0.2.9/docs/
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      611 2021-07-20 09:29:16.000000 pyopendota-0.2.9/docs/Makefile
+drwxrwxr-x   0 hrishirt  (1000) hrishirt  (1000)        0 2023-04-30 06:04:52.569672 pyopendota-0.2.9/docs/_build/
+drwxrwxr-x   0 hrishirt  (1000) hrishirt  (1000)        0 2023-04-30 06:04:52.569672 pyopendota-0.2.9/docs/_build/html/
+drwxrwxr-x   0 hrishirt  (1000) hrishirt  (1000)        0 2023-04-30 06:04:53.981686 pyopendota-0.2.9/docs/_build/html/_static/
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      286 2021-01-01 06:53:29.000000 pyopendota-0.2.9/docs/_build/html/_static/file.png
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       90 2021-01-01 06:53:29.000000 pyopendota-0.2.9/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       90 2021-01-01 06:53:29.000000 pyopendota-0.2.9/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       28 2021-07-20 09:29:16.000000 pyopendota-0.2.9/docs/authors.rst
+-rwxrwxr-x   0 hrishirt  (1000) hrishirt  (1000)     5228 2022-03-04 08:52:09.000000 pyopendota-0.2.9/docs/conf.py
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       33 2021-07-20 09:29:16.000000 pyopendota-0.2.9/docs/contributing.rst
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       28 2021-07-20 09:29:16.000000 pyopendota-0.2.9/docs/history.rst
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)     2288 2022-03-04 09:12:46.000000 pyopendota-0.2.9/docs/index.rst
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)     1169 2021-07-20 09:29:16.000000 pyopendota-0.2.9/docs/installation.rst
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      770 2021-07-20 09:29:16.000000 pyopendota-0.2.9/docs/make.bat
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       61 2022-03-04 09:17:26.000000 pyopendota-0.2.9/docs/modules.rst
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      435 2022-03-04 09:17:26.000000 pyopendota-0.2.9/docs/opendota.rst
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       27 2021-07-20 09:29:16.000000 pyopendota-0.2.9/docs/readme.rst
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       26 2022-03-04 08:52:38.000000 pyopendota-0.2.9/docs/usage.rst
+drwxrwxr-x   0 hrishirt  (1000) hrishirt  (1000)        0 2023-04-30 06:04:54.229689 pyopendota-0.2.9/opendota/
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      246 2023-04-30 06:03:45.000000 pyopendota-0.2.9/opendota/__init__.py
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      551 2021-09-07 18:28:56.000000 pyopendota-0.2.9/opendota/cli.py
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)    26361 2023-04-29 16:27:53.000000 pyopendota-0.2.9/opendota/opendota.py
+drwxrwxr-x   0 hrishirt  (1000) hrishirt  (1000)        0 2023-04-30 06:04:54.233689 pyopendota-0.2.9/pyopendota.egg-info/
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)     4712 2023-04-30 06:04:30.000000 pyopendota-0.2.9/pyopendota.egg-info/PKG-INFO
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      731 2023-04-30 06:04:32.000000 pyopendota-0.2.9/pyopendota.egg-info/SOURCES.txt
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)        1 2023-04-30 06:04:30.000000 pyopendota-0.2.9/pyopendota.egg-info/dependency_links.txt
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       47 2023-04-30 06:04:30.000000 pyopendota-0.2.9/pyopendota.egg-info/entry_points.txt
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)        1 2023-04-30 06:04:30.000000 pyopendota-0.2.9/pyopendota.egg-info/not-zip-safe
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       14 2023-04-30 06:04:30.000000 pyopendota-0.2.9/pyopendota.egg-info/requires.txt
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)        9 2023-04-30 06:04:30.000000 pyopendota-0.2.9/pyopendota.egg-info/top_level.txt
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      425 2023-04-30 06:04:54.433691 pyopendota-0.2.9/setup.cfg
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)     1610 2023-04-30 06:03:45.000000 pyopendota-0.2.9/setup.py
+drwxrwxr-x   0 hrishirt  (1000) hrishirt  (1000)        0 2023-04-30 06:04:54.329690 pyopendota-0.2.9/tests/
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)       40 2021-07-20 09:30:26.000000 pyopendota-0.2.9/tests/__init__.py
+-rw-rw-r--   0 hrishirt  (1000) hrishirt  (1000)      556 2021-07-20 06:43:05.000000 pyopendota-0.2.9/tests/test_opendota.py
```

### Comparing `pyopendota-0.2.8/CONTRIBUTING.rst` & `pyopendota-0.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyopendota-0.2.8/LICENSE` & `pyopendota-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopendota-0.2.8/PKG-INFO` & `pyopendota-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyopendota
-Version: 0.2.8
+Version: 0.2.9
 Summary: A python interface for <OPENDOTA/> API
 Home-page: https://github.com/hrishikeshrt/pyopendota
 Author: Hrishikesh Terdalkar
 Author-email: hrishikeshrt@linuxmail.org
 License: MIT license
 Keywords: opendota
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -181,9 +180,7 @@
 * Fantasy score calculation
 * Bugfixes
 
 0.1.0 (2021-07-20)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `pyopendota-0.2.8/README.rst` & `pyopendota-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyopendota-0.2.8/docs/Makefile` & `pyopendota-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyopendota-0.2.8/docs/conf.py` & `pyopendota-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyopendota-0.2.8/docs/index.rst` & `pyopendota-0.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyopendota-0.2.8/docs/installation.rst` & `pyopendota-0.2.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyopendota-0.2.8/docs/make.bat` & `pyopendota-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyopendota-0.2.8/opendota/cli.py` & `pyopendota-0.2.9/opendota/cli.py`

 * *Files identical despite different names*

### Comparing `pyopendota-0.2.8/opendota/opendota.py` & `pyopendota-0.2.9/opendota/opendota.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,30 +222,30 @@
 
         url_parts = list(urlsplit(self.api_url))
         url_parts[2] += url
         if not post:
             url_parts[3] = "&".join([f"{k}={v}" for k, v in data.items()])
 
         query_url = urlunsplit(url_parts)
-        LOGGER.info("Query URL:", query_url)
+        LOGGER.info(f"Query URL: {query_url}")
 
         if not post:
             r = self._session.get(query_url)
         else:
             r = self._session.post(query_url, data=data)
 
         content = r.content.decode("utf-8")
         json_data = json.loads(content)
 
         if json_data and "error" in json_data:
             LOGGER.warning(f"Could not fetch '{url}' ({json_data['error']}).")
             return None
 
         if path is not None:
-            with open(path, "w") as f:
+            with open(path, "w", encoding='utf-8') as f:
                 json.dump(json_data, f, ensure_ascii=False)
         return json_data
 
     def get(self, *args, **kwargs):
         """
         Make a GET request to <OPENDOTA/> API.
 
@@ -428,19 +428,23 @@
 
     def get_match(self, match_id: int or str, force: bool = False):
         """Get match data"""
         url = f"/matches/{match_id}"
         filename = f"match_{match_id}.json"
         return self.get(url, filename=filename, force=force)
 
-    def get_pro_matches(self, force: bool = False):
+    def get_pro_matches(self, match_id: int or str = None, force: bool = False):
         """Get a list of pro matches"""
         url = "/proMatches"
         filename = "pro_matches.json"
-        return self.get(url, filename=filename, force=force)
+        data = {}
+        if match_id is not None:
+            data["less_than_match_id"] = match_id
+            filename = f"pro_matches_{match_id}.json"
+        return self.get(url, filename=filename, data=data, force=force)
 
     def get_live(self):
         """Get top currently ongoing live games"""
         url = "/live"
         return self.get(url)
 
     # ----------------------------------------------------------------------- #
```

### Comparing `pyopendota-0.2.8/pyopendota.egg-info/PKG-INFO` & `pyopendota-0.2.9/pyopendota.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyopendota
-Version: 0.2.8
+Version: 0.2.9
 Summary: A python interface for <OPENDOTA/> API
 Home-page: https://github.com/hrishikeshrt/pyopendota
 Author: Hrishikesh Terdalkar
 Author-email: hrishikeshrt@linuxmail.org
 License: MIT license
 Keywords: opendota
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -181,9 +180,7 @@
 * Fantasy score calculation
 * Bugfixes
 
 0.1.0 (2021-07-20)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `pyopendota-0.2.8/pyopendota.egg-info/SOURCES.txt` & `pyopendota-0.2.9/pyopendota.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/modules.rst
 docs/opendota.rst
 docs/readme.rst
 docs/usage.rst
+docs/_build/html/_static/file.png
+docs/_build/html/_static/minus.png
+docs/_build/html/_static/plus.png
 opendota/__init__.py
 opendota/cli.py
 opendota/opendota.py
 pyopendota.egg-info/PKG-INFO
 pyopendota.egg-info/SOURCES.txt
 pyopendota.egg-info/dependency_links.txt
 pyopendota.egg-info/entry_points.txt
```

### Comparing `pyopendota-0.2.8/setup.py` & `pyopendota-0.2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     include_package_data=True,
     keywords='opendota',
     name='pyopendota',
     packages=find_packages(include=['opendota', 'opendota.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/hrishikeshrt/pyopendota',
-    version='0.2.8',
+    version='0.2.9',
     zip_safe=False,
 )
```

### Comparing `pyopendota-0.2.8/tests/test_opendota.py` & `pyopendota-0.2.9/tests/test_opendota.py`

 * *Files identical despite different names*

