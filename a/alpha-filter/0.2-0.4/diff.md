# Comparing `tmp/alpha-filter-0.2.tar.gz` & `tmp/alpha-filter-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpha-filter-0.2.tar", last modified: Sat Apr 29 21:04:35 2023, max compression
+gzip compressed data, was "alpha-filter-0.4.tar", last modified: Sat Apr 29 23:07:51 2023, max compression
```

## Comparing `alpha-filter-0.2.tar` & `alpha-filter-0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 21:04:35.607802 alpha-filter-0.2/
--rw-rw-rw-   0        0        0       90 2023-04-29 21:04:35.606801 alpha-filter-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-02-28 18:59:23.000000 alpha-filter-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 21:04:35.606801 alpha-filter-0.2/alpha_filter.egg-info/
--rw-rw-rw-   0        0        0       90 2023-04-29 21:04:35.000000 alpha-filter-0.2/alpha_filter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-04-29 21:04:35.000000 alpha-filter-0.2/alpha_filter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 21:04:35.000000 alpha-filter-0.2/alpha_filter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-29 21:04:35.000000 alpha-filter-0.2/alpha_filter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4165 2023-04-29 21:03:02.000000 alpha-filter-0.2/filter.py
--rw-rw-rw-   0        0        0       42 2023-04-29 21:04:35.607802 alpha-filter-0.2/setup.cfg
--rw-rw-rw-   0        0        0      158 2023-04-29 21:04:22.000000 alpha-filter-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 23:07:51.260834 alpha-filter-0.4/
+-rw-rw-rw-   0        0        0      111 2023-04-29 23:07:51.259833 alpha-filter-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1458 2023-04-29 23:04:47.000000 alpha-filter-0.4/README.md
+-rw-rw-rw-   0        0        0     4683 2023-04-29 23:05:36.000000 alpha-filter-0.4/alpha-filter.py
+drwxrwxrwx   0        0        0        0 2023-04-29 23:07:51.258832 alpha-filter-0.4/alpha_filter.egg-info/
+-rw-rw-rw-   0        0        0      111 2023-04-29 23:07:51.000000 alpha-filter-0.4/alpha_filter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-04-29 23:07:51.000000 alpha-filter-0.4/alpha_filter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 23:07:51.000000 alpha-filter-0.4/alpha_filter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-29 23:07:51.000000 alpha-filter-0.4/alpha_filter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 23:07:51.260834 alpha-filter-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      190 2023-04-29 23:07:32.000000 alpha-filter-0.4/setup.py
```

