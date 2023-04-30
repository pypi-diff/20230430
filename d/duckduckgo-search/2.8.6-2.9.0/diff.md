# Comparing `tmp/duckduckgo_search-2.8.6.tar.gz` & `tmp/duckduckgo_search-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-2.8.6.tar", last modified: Sat Apr 15 09:07:48 2023, max compression
+gzip compressed data, was "duckduckgo_search-2.9.0.tar", last modified: Sun Apr 30 10:57:21 2023, max compression
```

## Comparing `duckduckgo_search-2.8.6.tar` & `duckduckgo_search-2.9.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:07:48.312422 duckduckgo_search-2.8.6/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-04-15 09:07:48.312422 duckduckgo_search-2.8.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    34567 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:07:48.312422 duckduckgo_search-2.8.6/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:07:48.312422 duckduckgo_search-2.8.6/duckduckgo_search/cli/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10405 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/cli/ddgs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6014 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/ddg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2750 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/ddg_answers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6246 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/ddg_images.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7090 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/ddg_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3644 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/ddg_news.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1005 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/ddg_suggestions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1548 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/ddg_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3765 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/ddg_videos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3570 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:07:48.312422 duckduckgo_search-2.8.6/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-04-15 09:07:48.000000 duckduckgo_search-2.8.6/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-15 09:07:48.000000 duckduckgo_search-2.8.6/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 09:07:48.000000 duckduckgo_search-2.8.6/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-15 09:07:48.000000 duckduckgo_search-2.8.6/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-15 09:07:48.000000 duckduckgo_search-2.8.6/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-15 09:07:48.000000 duckduckgo_search-2.8.6/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 09:07:48.312422 duckduckgo_search-2.8.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:07:48.312422 duckduckgo_search-2.8.6/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1619 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/tests/test_ddg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/tests/test_ddg_answers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2510 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/tests/test_ddg_images.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/tests/test_ddg_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/tests/test_ddg_news.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/tests/test_ddg_suggestions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/tests/test_ddg_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/tests/test_ddg_videos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:57:21.693529 duckduckgo_search-2.9.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-04-30 10:57:21.693529 duckduckgo_search-2.9.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34567 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:57:21.689529 duckduckgo_search-2.9.0/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:57:21.689529 duckduckgo_search-2.9.0/duckduckgo_search/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10405 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/cli/ddgs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6014 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/ddg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2750 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/ddg_answers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6246 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/ddg_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7090 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/ddg_maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3644 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/ddg_news.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1005 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/ddg_suggestions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1580 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/ddg_translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3765 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/ddg_videos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3619 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:57:21.689529 duckduckgo_search-2.9.0/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-04-30 10:57:21.000000 duckduckgo_search-2.9.0/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-30 10:57:21.000000 duckduckgo_search-2.9.0/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 10:57:21.000000 duckduckgo_search-2.9.0/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-30 10:57:21.000000 duckduckgo_search-2.9.0/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-30 10:57:21.000000 duckduckgo_search-2.9.0/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-30 10:57:21.000000 duckduckgo_search-2.9.0/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 10:57:21.693529 duckduckgo_search-2.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:57:21.689529 duckduckgo_search-2.9.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1619 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/tests/test_ddg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/tests/test_ddg_answers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2510 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/tests/test_ddg_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/tests/test_ddg_maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/tests/test_ddg_news.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/tests/test_ddg_suggestions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/tests/test_ddg_translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/tests/test_ddg_videos.py
```

### Comparing `duckduckgo_search-2.8.6/LICENSE.md` & `duckduckgo_search-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.6/PKG-INFO` & `duckduckgo_search-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 2.8.6
+Version: 2.9.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-2.8.6/README.md` & `duckduckgo_search-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.6/duckduckgo_search/__init__.py` & `duckduckgo_search-2.9.0/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.6/duckduckgo_search/cli/ddgs.py` & `duckduckgo_search-2.9.0/duckduckgo_search/cli/ddgs.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.6/duckduckgo_search/ddg.py` & `duckduckgo_search-2.9.0/duckduckgo_search/ddg.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.6/duckduckgo_search/ddg_answers.py` & `duckduckgo_search-2.9.0/duckduckgo_search/ddg_answers.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.6/duckduckgo_search/ddg_images.py` & `duckduckgo_search-2.9.0/duckduckgo_search/ddg_images.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.6/duckduckgo_search/ddg_maps.py` & `duckduckgo_search-2.9.0/duckduckgo_search/ddg_maps.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.6/duckduckgo_search/ddg_news.py` & `duckduckgo_search-2.9.0/duckduckgo_search/ddg_news.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.6/duckduckgo_search/ddg_suggestions.py` & `duckduckgo_search-2.9.0/duckduckgo_search/ddg_suggestions.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.6/duckduckgo_search/ddg_translate.py` & `duckduckgo_search-2.9.0/duckduckgo_search/ddg_translate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from .utils import SESSION, VQD_DICT, _do_output, _get_vqd
+from .utils import SESSION, VQD_CACHE, _do_output, _get_vqd
 
 logger = logging.getLogger(__name__)
 
 
 def ddg_translate(
     keywords,
     from_=None,
@@ -51,14 +51,15 @@
                 data=data.encode("utf-8"),
             )
             resp.raise_for_status()
             result = resp.json()
             result["original"] = data
             results.append(result)
         except Exception:
-            VQD_DICT.pop("translate", None)
+            VQD_CACHE.pop("translate", None)
+            VQD_CACHE.close()
             logger.exception("")
 
     if output:
         keywords = keywords[0]
         _do_output("ddg_translate", keywords, output, results)
     return results
```

### Comparing `duckduckgo_search-2.8.6/duckduckgo_search/ddg_videos.py` & `duckduckgo_search-2.9.0/duckduckgo_search/ddg_videos.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.6/duckduckgo_search/utils.py` & `duckduckgo_search-2.9.0/duckduckgo_search/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,65 +5,70 @@
 import re
 from datetime import datetime
 from html import unescape
 from shutil import copyfileobj
 from time import sleep
 
 import requests
+from diskcache import Cache
 
 logger = logging.getLogger(__name__)
 
 HEADERS = {
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:102.0) Gecko/20100101 Firefox/102.0",
     "Referer": "https://duckduckgo.com/",
 }
+HEADERS_FILE_DOWNLOAD = {
+    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:102.0) Gecko/20100101 Firefox/102.0"
+}
 SESSION = requests.Session()
 SESSION.headers = HEADERS
-VQD_DICT = dict()
 RE_STRIP_TAGS = re.compile("<.*?>")
+VQD_CACHE = Cache(
+    "vqd_cache", size_limit=104_857_600, eviction_policy="least-frequently-used"
+)
 
 
 def _get_vqd(keywords):
     global SESSION
 
-    vqd_bytes = VQD_DICT.get(keywords, None)
+    vqd_bytes = VQD_CACHE.get(keywords, None)
+    VQD_CACHE.close()
     if vqd_bytes:
-        # move_to_end (LRU cache)
-        VQD_DICT[keywords] = VQD_DICT.pop(keywords)
+        logger.info("keywords=%s. Got vqd from cache", keywords)
         return vqd_bytes.decode()
 
     payload = {"q": keywords}
     for _ in range(2):
         try:
             resp = SESSION.post("https://duckduckgo.com", data=payload, timeout=10)
             resp.raise_for_status()
             vqd_index_start = resp.content.index(b"vqd='") + 5
             vqd_index_end = resp.content.index(b"'", vqd_index_start)
             vqd_bytes = resp.content[vqd_index_start:vqd_index_end]
 
             if vqd_bytes:
-                # delete the first key to reduce memory consumption
-                if len(VQD_DICT) > 32768:
-                    VQD_DICT.pop(next(iter(VQD_DICT)))
-                VQD_DICT[keywords] = vqd_bytes
+                VQD_CACHE[keywords] = vqd_bytes
+                VQD_CACHE.close()
                 return vqd_bytes.decode()
 
         except Exception:
             logger.exception("")
 
         # refresh SESSION if not vqd
         prev_proxies = SESSION.proxies
         SESSION.close()
         SESSION = requests.Session()
         SESSION.headers = HEADERS
         SESSION.proxies = prev_proxies
         logger.warning(
             "keywords=%s. _get_vqd() is None. Refresh SESSION and retry...", keywords
         )
-        VQD_DICT.pop(keywords, None)
+        VQD_CACHE.pop(keywords, None)
+        VQD_CACHE.close()
         sleep(0.25)
 
     # sleep to prevent blocking
     sleep(0.25)
 
 
 def _save_json(jsonfile, data):
@@ -77,19 +82,18 @@
             headers = data[0].keys()
             writer = csv.DictWriter(file, fieldnames=headers, quoting=csv.QUOTE_MINIMAL)
             writer.writeheader()
             writer.writerows(data)
 
 
 def _download_file(url, dir_path, filename):
-    headers = {
-        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:102.0) Gecko/20100101 Firefox/102.0"
-    }
     try:
-        with requests.get(url, headers=headers, stream=True, timeout=10) as resp:
+        with requests.get(
+            url, headers=HEADERS_FILE_DOWNLOAD, stream=True, timeout=10
+        ) as resp:
             resp.raise_for_status()
             resp.raw.decode_content = True
             with open(os.path.join(dir_path, filename), "wb") as file:
                 copyfileobj(resp.raw, file)
             logger.info(f"File downloaded {url}")
     except Exception:
         logger.exception("")
```

### Comparing `duckduckgo_search-2.8.6/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-2.9.0/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo-search
-Version: 2.8.6
+Version: 2.9.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-2.8.6/duckduckgo_search.egg-info/SOURCES.txt` & `duckduckgo_search-2.9.0/duckduckgo_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.6/pyproject.toml` & `duckduckgo_search-2.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,17 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-    "requests>=2.28.2",
     "click>=8.1.3",
+    "diskcache>=5.6.1",
+    "requests>=2.29.0",
 ]
 dynamic = ["version"]
 
 [project.urls]  # Optional
 "Homepage" = "https://github.com/deedy5/duckduckgo_search"
 
 [project.scripts]
```

### Comparing `duckduckgo_search-2.8.6/tests/test_ddg.py` & `duckduckgo_search-2.9.0/tests/test_ddg.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.6/tests/test_ddg_answers.py` & `duckduckgo_search-2.9.0/tests/test_ddg_answers.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.6/tests/test_ddg_images.py` & `duckduckgo_search-2.9.0/tests/test_ddg_images.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.6/tests/test_ddg_news.py` & `duckduckgo_search-2.9.0/tests/test_ddg_news.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.6/tests/test_ddg_suggestions.py` & `duckduckgo_search-2.9.0/tests/test_ddg_suggestions.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.6/tests/test_ddg_translate.py` & `duckduckgo_search-2.9.0/tests/test_ddg_translate.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.6/tests/test_ddg_videos.py` & `duckduckgo_search-2.9.0/tests/test_ddg_videos.py`

 * *Files identical despite different names*

