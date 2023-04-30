# Comparing `tmp/gsbg-0.1.tar.gz` & `tmp/gsbg-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsbg-0.1.tar", last modified: Sat Apr 29 07:26:03 2023, max compression
+gzip compressed data, was "gsbg-0.1.1.tar", last modified: Sun Apr 30 15:17:50 2023, max compression
```

## Comparing `gsbg-0.1.tar` & `gsbg-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 07:26:03.979861 gsbg-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-29 07:25:54.000000 gsbg-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-29 07:25:54.000000 gsbg-0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-29 07:26:03.979861 gsbg-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-29 07:25:54.000000 gsbg-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 07:26:03.975861 gsbg-0.1/gsbg/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-29 07:25:54.000000 gsbg-0.1/gsbg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10646 2023-04-29 07:25:54.000000 gsbg-0.1/gsbg/google_scholar_badge_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 07:26:03.979861 gsbg-0.1/gsbg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-29 07:26:03.000000 gsbg-0.1/gsbg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-29 07:26:03.000000 gsbg-0.1/gsbg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 07:26:03.000000 gsbg-0.1/gsbg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-29 07:26:03.000000 gsbg-0.1/gsbg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 07:26:03.000000 gsbg-0.1/gsbg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 07:26:03.979861 gsbg-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-29 07:25:54.000000 gsbg-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:17:50.763956 gsbg-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-30 15:17:40.000000 gsbg-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 15:17:40.000000 gsbg-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-30 15:17:50.763956 gsbg-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-30 15:17:40.000000 gsbg-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:17:50.763956 gsbg-0.1.1/gsbg/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-30 15:17:40.000000 gsbg-0.1.1/gsbg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-04-30 15:17:40.000000 gsbg-0.1.1/gsbg/google_scholar_badge_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:17:50.763956 gsbg-0.1.1/gsbg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-30 15:17:50.000000 gsbg-0.1.1/gsbg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-30 15:17:50.000000 gsbg-0.1.1/gsbg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 15:17:50.000000 gsbg-0.1.1/gsbg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 15:17:50.000000 gsbg-0.1.1/gsbg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 15:17:50.000000 gsbg-0.1.1/gsbg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 15:17:50.763956 gsbg-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-30 15:17:40.000000 gsbg-0.1.1/setup.py
```

### Comparing `gsbg-0.1/LICENSE` & `gsbg-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gsbg-0.1/gsbg/google_scholar_badge_generator.py` & `gsbg-0.1.1/gsbg/google_scholar_badge_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from bs4 import BeautifulSoup, element
 
 MIRROR_SITES = {
     "scholar.lanfanshu.cn": "True",  # 'True' means this mirror site is in Chinese
 }
 
 ARTICLE_CITATION_SELECTOR = (
-    "#gsc_oci_table > div:nth-child(6) > div.gsc_oci_value > div:nth-child(1) > a"
+    "#gsc_oci_table > div > div.gsc_oci_value > div > a"
 )
 PROFILE_CITATION_SELECTOR = "#gsc_rsb_st > tbody > tr:nth-child(1) > td:nth-child(2)"
 
 USER_AGENTS = [
     "Mozilla/4.0 (compatible; MSIE 6.0; Windows NT 5.1; SV1; AcooBrowser; .NET CLR 1.1.4322; .NET CLR 2.0.50727)",
     "Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 6.0; Acoo Browser; SLCC1; .NET CLR 2.0.50727; Media Center PC 5.0; .NET CLR 3.0.04506)",
     "Mozilla/4.0 (compatible; MSIE 7.0; AOL 9.5; AOLBuild 4337.35; Windows NT 5.1; .NET CLR 1.1.4322; .NET CLR 2.0.50727)",
```

### Comparing `gsbg-0.1/setup.py` & `gsbg-0.1.1/setup.py`

 * *Files identical despite different names*

