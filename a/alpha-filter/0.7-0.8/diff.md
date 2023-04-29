# Comparing `tmp/alpha-filter-0.7.tar.gz` & `tmp/alpha-filter-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpha-filter-0.7.tar", last modified: Sat Apr 29 23:35:37 2023, max compression
+gzip compressed data, was "alpha-filter-0.8.tar", last modified: Sat Apr 29 23:38:15 2023, max compression
```

## Comparing `alpha-filter-0.7.tar` & `alpha-filter-0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 23:35:37.709935 alpha-filter-0.7/
--rw-rw-rw-   0        0        0       87 2023-04-29 23:35:37.705935 alpha-filter-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1458 2023-04-29 23:04:47.000000 alpha-filter-0.7/README.md
--rw-rw-rw-   0        0        0     4683 2023-04-29 23:05:36.000000 alpha-filter-0.7/alpha-ads-filter.py
-drwxrwxrwx   0        0        0        0 2023-04-29 23:35:37.705935 alpha-filter-0.7/alpha_filter.egg-info/
--rw-rw-rw-   0        0        0       87 2023-04-29 23:35:37.000000 alpha-filter-0.7/alpha_filter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-29 23:35:37.000000 alpha-filter-0.7/alpha_filter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 23:35:37.000000 alpha-filter-0.7/alpha_filter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-29 23:35:37.000000 alpha-filter-0.7/alpha_filter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 23:35:37.709935 alpha-filter-0.7/setup.cfg
--rw-rw-rw-   0        0        0      195 2023-04-29 23:34:58.000000 alpha-filter-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 23:38:15.974504 alpha-filter-0.8/
+-rw-rw-rw-   0        0        0       87 2023-04-29 23:38:15.973550 alpha-filter-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1458 2023-04-29 23:04:47.000000 alpha-filter-0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 23:38:15.972504 alpha-filter-0.8/alpha_filter.egg-info/
+-rw-rw-rw-   0        0        0       87 2023-04-29 23:38:15.000000 alpha-filter-0.8/alpha_filter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-04-29 23:38:15.000000 alpha-filter-0.8/alpha_filter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 23:38:15.000000 alpha-filter-0.8/alpha_filter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 23:38:15.000000 alpha-filter-0.8/alpha_filter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4683 2023-04-29 23:05:36.000000 alpha-filter-0.8/alphafilter.py
+-rw-rw-rw-   0        0        0       42 2023-04-29 23:38:15.974504 alpha-filter-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      190 2023-04-29 23:38:10.000000 alpha-filter-0.8/setup.py
```

### Comparing `alpha-filter-0.7/README.md` & `alpha-filter-0.8/README.md`

 * *Files identical despite different names*

### Comparing `alpha-filter-0.7/alpha-ads-filter.py` & `alpha-filter-0.8/alphafilter.py`

 * *Files identical despite different names*

