# Comparing `tmp/overloaded-iterables-0.5.47.tar.gz` & `tmp/overloaded-iterables-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overloaded-iterables-0.5.47.tar", last modified: Sun Apr 30 15:43:06 2023, max compression
+gzip compressed data, was "overloaded-iterables-0.6.tar", last modified: Sun Apr 30 21:06:36 2023, max compression
```

## Comparing `overloaded-iterables-0.5.47.tar` & `overloaded-iterables-0.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 15:43:06.056347 overloaded-iterables-0.5.47/
--rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.5.47/LICENSE
--rw-rw-rw-   0        0        0      613 2023-04-30 15:43:06.056347 overloaded-iterables-0.5.47/PKG-INFO
--rw-rw-rw-   0        0        0     3348 2023-04-30 15:28:30.000000 overloaded-iterables-0.5.47/README.md
--rw-rw-rw-   0        0        0      111 2023-04-30 15:43:06.062347 overloaded-iterables-0.5.47/setup.cfg
--rw-rw-rw-   0        0        0      958 2023-04-30 15:42:19.000000 overloaded-iterables-0.5.47/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 15:43:06.035347 overloaded-iterables-0.5.47/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 15:43:06.041346 overloaded-iterables-0.5.47/src/overloaded_iterables/
--rw-rw-rw-   0        0        0        0 2023-04-29 23:52:39.000000 overloaded-iterables-0.5.47/src/overloaded_iterables/__init__.py
--rw-rw-rw-   0        0        0     2483 2023-04-30 15:28:16.000000 overloaded-iterables-0.5.47/src/overloaded_iterables/classes.py
-drwxrwxrwx   0        0        0        0 2023-04-30 15:43:06.055346 overloaded-iterables-0.5.47/src/overloaded_iterables.egg-info/
--rw-rw-rw-   0        0        0      613 2023-04-30 15:43:05.000000 overloaded-iterables-0.5.47/src/overloaded_iterables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-04-30 15:43:05.000000 overloaded-iterables-0.5.47/src/overloaded_iterables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 15:43:05.000000 overloaded-iterables-0.5.47/src/overloaded_iterables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-30 15:43:05.000000 overloaded-iterables-0.5.47/src/overloaded_iterables.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 21:06:36.108930 overloaded-iterables-0.6/
+-rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.6/LICENSE
+-rw-rw-rw-   0        0        0     7861 2023-04-30 21:06:36.109930 overloaded-iterables-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7150 2023-04-30 20:48:12.000000 overloaded-iterables-0.6/README.md
+-rw-rw-rw-   0        0        0      111 2023-04-30 21:06:36.110935 overloaded-iterables-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1475 2023-04-30 21:06:19.000000 overloaded-iterables-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:06:36.095933 overloaded-iterables-0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 21:06:36.100930 overloaded-iterables-0.6/src/overloaded_iterables/
+-rw-rw-rw-   0        0        0        0 2023-04-29 23:52:39.000000 overloaded-iterables-0.6/src/overloaded_iterables/__init__.py
+-rw-rw-rw-   0        0        0    13051 2023-04-30 20:19:49.000000 overloaded-iterables-0.6/src/overloaded_iterables/classes.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:06:36.108930 overloaded-iterables-0.6/src/overloaded_iterables.egg-info/
+-rw-rw-rw-   0        0        0     7861 2023-04-30 21:06:36.000000 overloaded-iterables-0.6/src/overloaded_iterables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-04-30 21:06:36.000000 overloaded-iterables-0.6/src/overloaded_iterables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 21:06:36.000000 overloaded-iterables-0.6/src/overloaded_iterables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-30 21:06:36.000000 overloaded-iterables-0.6/src/overloaded_iterables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-30 21:06:36.000000 overloaded-iterables-0.6/src/overloaded_iterables.egg-info/top_level.txt
```

### Comparing `overloaded-iterables-0.5.47/LICENSE` & `overloaded-iterables-0.6/LICENSE`

 * *Files identical despite different names*

