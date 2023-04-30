# Comparing `tmp/duckduckgo_search-2.9.0.tar.gz` & `tmp/duckduckgo_search-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-2.9.0.tar", last modified: Sun Apr 30 10:57:21 2023, max compression
+gzip compressed data, was "duckduckgo_search-2.9.1.tar", last modified: Sun Apr 30 18:42:53 2023, max compression
```

## Comparing `duckduckgo_search-2.9.0.tar` & `duckduckgo_search-2.9.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:57:21.693529 duckduckgo_search-2.9.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-04-30 10:57:21.693529 duckduckgo_search-2.9.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    34567 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:57:21.689529 duckduckgo_search-2.9.0/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:57:21.689529 duckduckgo_search-2.9.0/duckduckgo_search/cli/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10405 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/cli/ddgs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6014 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/ddg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2750 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/ddg_answers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6246 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/ddg_images.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7090 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/ddg_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3644 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/ddg_news.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1005 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/ddg_suggestions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1580 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/ddg_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3765 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/ddg_videos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3619 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:57:21.689529 duckduckgo_search-2.9.0/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-04-30 10:57:21.000000 duckduckgo_search-2.9.0/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-30 10:57:21.000000 duckduckgo_search-2.9.0/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 10:57:21.000000 duckduckgo_search-2.9.0/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-30 10:57:21.000000 duckduckgo_search-2.9.0/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-30 10:57:21.000000 duckduckgo_search-2.9.0/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-30 10:57:21.000000 duckduckgo_search-2.9.0/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 10:57:21.693529 duckduckgo_search-2.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:57:21.689529 duckduckgo_search-2.9.0/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1619 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/tests/test_ddg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/tests/test_ddg_answers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2510 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/tests/test_ddg_images.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/tests/test_ddg_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/tests/test_ddg_news.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/tests/test_ddg_suggestions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/tests/test_ddg_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-04-30 10:57:04.000000 duckduckgo_search-2.9.0/tests/test_ddg_videos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:42:53.156472 duckduckgo_search-2.9.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-04-30 18:42:53.156472 duckduckgo_search-2.9.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34567 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:42:53.152472 duckduckgo_search-2.9.1/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/duckduckgo_search/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:42:53.156472 duckduckgo_search-2.9.1/duckduckgo_search/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/duckduckgo_search/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10405 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/duckduckgo_search/cli/ddgs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6014 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/duckduckgo_search/ddg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2750 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/duckduckgo_search/ddg_answers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6246 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/duckduckgo_search/ddg_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7090 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/duckduckgo_search/ddg_maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3644 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/duckduckgo_search/ddg_news.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1005 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/duckduckgo_search/ddg_suggestions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1580 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/duckduckgo_search/ddg_translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3765 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/duckduckgo_search/ddg_videos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3813 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/duckduckgo_search/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:42:53.152472 duckduckgo_search-2.9.1/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-04-30 18:42:53.000000 duckduckgo_search-2.9.1/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-30 18:42:53.000000 duckduckgo_search-2.9.1/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:42:53.000000 duckduckgo_search-2.9.1/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-30 18:42:53.000000 duckduckgo_search-2.9.1/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-30 18:42:53.000000 duckduckgo_search-2.9.1/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-30 18:42:53.000000 duckduckgo_search-2.9.1/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 18:42:53.156472 duckduckgo_search-2.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:42:53.156472 duckduckgo_search-2.9.1/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1619 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/tests/test_ddg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/tests/test_ddg_answers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2510 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/tests/test_ddg_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/tests/test_ddg_maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/tests/test_ddg_news.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/tests/test_ddg_suggestions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/tests/test_ddg_translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-04-30 18:42:31.000000 duckduckgo_search-2.9.1/tests/test_ddg_videos.py
```

### Comparing `duckduckgo_search-2.9.0/LICENSE.md` & `duckduckgo_search-2.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/PKG-INFO` & `duckduckgo_search-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 2.9.0
+Version: 2.9.1
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-2.9.0/README.md` & `duckduckgo_search-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/duckduckgo_search/__init__.py` & `duckduckgo_search-2.9.1/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/duckduckgo_search/cli/ddgs.py` & `duckduckgo_search-2.9.1/duckduckgo_search/cli/ddgs.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/duckduckgo_search/ddg.py` & `duckduckgo_search-2.9.1/duckduckgo_search/ddg.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/duckduckgo_search/ddg_answers.py` & `duckduckgo_search-2.9.1/duckduckgo_search/ddg_answers.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/duckduckgo_search/ddg_images.py` & `duckduckgo_search-2.9.1/duckduckgo_search/ddg_images.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/duckduckgo_search/ddg_maps.py` & `duckduckgo_search-2.9.1/duckduckgo_search/ddg_maps.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/duckduckgo_search/ddg_news.py` & `duckduckgo_search-2.9.1/duckduckgo_search/ddg_news.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/duckduckgo_search/ddg_suggestions.py` & `duckduckgo_search-2.9.1/duckduckgo_search/ddg_suggestions.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/duckduckgo_search/ddg_translate.py` & `duckduckgo_search-2.9.1/duckduckgo_search/ddg_translate.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/duckduckgo_search/ddg_videos.py` & `duckduckgo_search-2.9.1/duckduckgo_search/ddg_videos.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/duckduckgo_search/utils.py` & `duckduckgo_search-2.9.1/duckduckgo_search/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,26 +19,33 @@
 }
 HEADERS_FILE_DOWNLOAD = {
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:102.0) Gecko/20100101 Firefox/102.0"
 }
 SESSION = requests.Session()
 SESSION.headers = HEADERS
 RE_STRIP_TAGS = re.compile("<.*?>")
-VQD_CACHE = Cache(
-    "vqd_cache", size_limit=104_857_600, eviction_policy="least-frequently-used"
-)
+try:
+    VQD_CACHE = Cache(
+        f"{os.path.dirname(__file__)}/vqd_cache",
+        size_limit=104_857_600,
+        eviction_policy="least-frequently-used",
+    )
+except OSError:
+    VQD_CACHE = Cache(
+        "vqd_cache", size_limit=104_857_600, eviction_policy="least-frequently-used"
+    )
 
 
 def _get_vqd(keywords):
     global SESSION
 
     vqd_bytes = VQD_CACHE.get(keywords, None)
     VQD_CACHE.close()
     if vqd_bytes:
-        logger.info("keywords=%s. Got vqd from cache", keywords)
+        logger.debug("keywords=%s. Got vqd from cache", keywords)
         return vqd_bytes.decode()
 
     payload = {"q": keywords}
     for _ in range(2):
         try:
             resp = SESSION.post("https://duckduckgo.com", data=payload, timeout=10)
             resp.raise_for_status()
```

### Comparing `duckduckgo_search-2.9.0/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-2.9.1/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo-search
-Version: 2.9.0
+Version: 2.9.1
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-2.9.0/duckduckgo_search.egg-info/SOURCES.txt` & `duckduckgo_search-2.9.1/duckduckgo_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/pyproject.toml` & `duckduckgo_search-2.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/tests/test_ddg.py` & `duckduckgo_search-2.9.1/tests/test_ddg.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/tests/test_ddg_answers.py` & `duckduckgo_search-2.9.1/tests/test_ddg_answers.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/tests/test_ddg_images.py` & `duckduckgo_search-2.9.1/tests/test_ddg_images.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/tests/test_ddg_news.py` & `duckduckgo_search-2.9.1/tests/test_ddg_news.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/tests/test_ddg_suggestions.py` & `duckduckgo_search-2.9.1/tests/test_ddg_suggestions.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/tests/test_ddg_translate.py` & `duckduckgo_search-2.9.1/tests/test_ddg_translate.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.0/tests/test_ddg_videos.py` & `duckduckgo_search-2.9.1/tests/test_ddg_videos.py`

 * *Files identical despite different names*

