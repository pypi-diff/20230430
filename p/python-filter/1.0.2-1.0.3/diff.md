# Comparing `tmp/python-filter-1.0.2.tar.gz` & `tmp/python-filter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-filter-1.0.2.tar", last modified: Fri Apr 21 01:00:27 2023, max compression
+gzip compressed data, was "python-filter-1.0.3.tar", last modified: Sun Apr 30 14:50:16 2023, max compression
```

## Comparing `python-filter-1.0.2.tar` & `python-filter-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 01:00:27.360016 python-filter-1.0.2/
--rw-rw-rw-   0        0        0      239 2023-04-21 01:00:27.358006 python-filter-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-21 01:00:27.330011 python-filter-1.0.2/pyfilter/
--rw-rw-rw-   0        0        0       67 2023-04-21 01:00:16.000000 python-filter-1.0.2/pyfilter/__init__.py
--rw-rw-rw-   0        0        0     2515 2023-04-21 00:46:51.000000 python-filter-1.0.2/pyfilter/dict_list.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:00:27.356007 python-filter-1.0.2/python_filter.egg-info/
--rw-rw-rw-   0        0        0      239 2023-04-21 01:00:27.000000 python-filter-1.0.2/python_filter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-04-21 01:00:27.000000 python-filter-1.0.2/python_filter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 01:00:27.000000 python-filter-1.0.2/python_filter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 01:00:27.000000 python-filter-1.0.2/python_filter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 01:00:27.000000 python-filter-1.0.2/python_filter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 01:00:27.360016 python-filter-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-04-21 01:00:22.000000 python-filter-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 14:50:16.098490 python-filter-1.0.3/
+-rw-rw-rw-   0        0        0      239 2023-04-30 14:50:16.097494 python-filter-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-30 14:50:16.027489 python-filter-1.0.3/pyfilter/
+-rw-rw-rw-   0        0        0       67 2023-04-21 01:00:16.000000 python-filter-1.0.3/pyfilter/__init__.py
+-rw-rw-rw-   0        0        0     2515 2023-04-21 00:46:51.000000 python-filter-1.0.3/pyfilter/dict_list.py
+-rw-rw-rw-   0        0        0      376 2023-04-30 14:49:44.000000 python-filter-1.0.3/pyfilter/tuple_list.py
+drwxrwxrwx   0        0        0        0 2023-04-30 14:50:16.095491 python-filter-1.0.3/python_filter.egg-info/
+-rw-rw-rw-   0        0        0      239 2023-04-30 14:50:15.000000 python-filter-1.0.3/python_filter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-04-30 14:50:15.000000 python-filter-1.0.3/python_filter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 14:50:15.000000 python-filter-1.0.3/python_filter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 14:50:15.000000 python-filter-1.0.3/python_filter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 14:50:15.000000 python-filter-1.0.3/python_filter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 14:50:16.099494 python-filter-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      456 2023-04-30 14:50:03.000000 python-filter-1.0.3/setup.py
```

### Comparing `python-filter-1.0.2/pyfilter/dict_list.py` & `python-filter-1.0.3/pyfilter/dict_list.py`

 * *Files identical despite different names*

