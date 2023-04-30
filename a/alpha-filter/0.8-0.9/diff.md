# Comparing `tmp/alpha-filter-0.8.tar.gz` & `tmp/alpha-filter-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpha-filter-0.8.tar", last modified: Sat Apr 29 23:38:15 2023, max compression
+gzip compressed data, was "alpha-filter-0.9.tar", last modified: Sun Apr 30 11:19:15 2023, max compression
```

## Comparing `alpha-filter-0.8.tar` & `alpha-filter-0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 23:38:15.974504 alpha-filter-0.8/
--rw-rw-rw-   0        0        0       87 2023-04-29 23:38:15.973550 alpha-filter-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1458 2023-04-29 23:04:47.000000 alpha-filter-0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 23:38:15.972504 alpha-filter-0.8/alpha_filter.egg-info/
--rw-rw-rw-   0        0        0       87 2023-04-29 23:38:15.000000 alpha-filter-0.8/alpha_filter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-04-29 23:38:15.000000 alpha-filter-0.8/alpha_filter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 23:38:15.000000 alpha-filter-0.8/alpha_filter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 23:38:15.000000 alpha-filter-0.8/alpha_filter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4683 2023-04-29 23:05:36.000000 alpha-filter-0.8/alphafilter.py
--rw-rw-rw-   0        0        0       42 2023-04-29 23:38:15.974504 alpha-filter-0.8/setup.cfg
--rw-rw-rw-   0        0        0      190 2023-04-29 23:38:10.000000 alpha-filter-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 11:19:15.605029 alpha-filter-0.9/
+-rw-rw-rw-   0        0        0     1607 2023-04-30 11:19:15.604031 alpha-filter-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1453 2023-04-29 23:39:58.000000 alpha-filter-0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 11:19:15.603030 alpha-filter-0.9/alpha_filter.egg-info/
+-rw-rw-rw-   0        0        0     1607 2023-04-30 11:19:15.000000 alpha-filter-0.9/alpha_filter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-04-30 11:19:15.000000 alpha-filter-0.9/alpha_filter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 11:19:15.000000 alpha-filter-0.9/alpha_filter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-30 11:19:15.000000 alpha-filter-0.9/alpha_filter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4683 2023-04-29 23:05:36.000000 alpha-filter-0.9/alphafilter.py
+-rw-rw-rw-   0        0        0       42 2023-04-30 11:19:15.605029 alpha-filter-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      353 2023-04-30 11:18:54.000000 alpha-filter-0.9/setup.py
```

### Comparing `alpha-filter-0.8/README.md` & `alpha-filter-0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 ```sh
 pip install alpha-filter
 ```
 
 ### Usage
 
 ```python
-from alpha-filter import filter_urls
+from alphafilter import filter_ads
 
 first_parsing_urls = ["https://www.example.com/1", "https://www.example.com/2"]
-new, old = filter_urls(first_parsing_urls)
+new, old = filter_ads(first_parsing_urls)
 new = ["https://www.example.com/1", "https://www.example.com/2"]
 old = []
 
 second_parsing_urls = first_parsing_urls # second parsing same with first
 
-new, old = filter_urls(second_parsing_urls)
+new, old = filter_ads(second_parsing_urls)
 new = []
 old = []
 
 third_parsing_urls = ["https://www.example.com/2", "https://www.example.com/3"]
 
-new, old = filter_urls(third_parsing_urls)
+new, old = filter_ads(third_parsing_urls)
 new = ["https://www.example.com/3"]
 old = ["https://www.example.com/2"]
 ```
 It uses a fast sqlite database to store urls. The database file ('ads.db') will be created in the root directory
 
 __Warning!!! this package has no protection against sql injection, do not use it for the external interface__
```

### Comparing `alpha-filter-0.8/alphafilter.py` & `alpha-filter-0.9/alphafilter.py`

 * *Files identical despite different names*

