# Comparing `tmp/voxx-cli-1.0.3.tar.gz` & `tmp/voxx-cli-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxx-cli-1.0.3.tar", last modified: Sun Apr 30 08:11:18 2023, max compression
+gzip compressed data, was "voxx-cli-1.0.4.tar", last modified: Sun Apr 30 08:21:11 2023, max compression
```

## Comparing `voxx-cli-1.0.3.tar` & `voxx-cli-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 08:11:18.107745 voxx-cli-1.0.3/
--rw-rw-rw-   0        0        0     2693 2023-04-30 08:11:18.107245 voxx-cli-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1451 2023-04-30 08:10:08.000000 voxx-cli-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-30 08:11:18.108003 voxx-cli-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1499 2023-04-30 04:35:11.000000 voxx-cli-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:11:18.096919 voxx-cli-1.0.3/voxx/
--rw-rw-rw-   0        0        0      140 2023-04-30 07:53:09.000000 voxx-cli-1.0.3/voxx/__init__.py
--rw-rw-rw-   0        0        0     3330 2023-04-30 08:05:30.000000 voxx-cli-1.0.3/voxx/__main__.py
--rw-rw-rw-   0        0        0     3718 2023-04-29 05:54:49.000000 voxx-cli-1.0.3/voxx/connection.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:11:18.098226 voxx-cli-1.0.3/voxx/css/
--rw-rw-rw-   0        0        0      900 2023-04-28 23:07:53.000000 voxx-cli-1.0.3/voxx/css/tui.css
--rw-rw-rw-   0        0        0     2333 2023-04-30 00:51:11.000000 voxx-cli-1.0.3/voxx/model.py
--rw-rw-rw-   0        0        0     5188 2023-04-30 00:51:11.000000 voxx-cli-1.0.3/voxx/tui.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:11:18.105738 voxx-cli-1.0.3/voxx_cli.egg-info/
--rw-rw-rw-   0        0        0     2693 2023-04-30 08:11:18.000000 voxx-cli-1.0.3/voxx_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-04-30 08:11:18.000000 voxx-cli-1.0.3/voxx_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       29 2023-04-30 08:11:18.000000 voxx-cli-1.0.3/voxx_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-30 08:11:18.000000 voxx-cli-1.0.3/voxx_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-04-30 08:11:18.000000 voxx-cli-1.0.3/voxx_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-30 08:11:18.000000 voxx-cli-1.0.3/voxx_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 08:21:11.064964 voxx-cli-1.0.4/
+-rw-rw-rw-   0        0        0     1084 2023-04-30 08:21:11.064964 voxx-cli-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2023-04-30 08:19:16.000000 voxx-cli-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 08:21:11.065464 voxx-cli-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2023-04-30 04:35:11.000000 voxx-cli-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:21:11.054953 voxx-cli-1.0.4/voxx/
+-rw-rw-rw-   0        0        0      140 2023-04-30 08:20:06.000000 voxx-cli-1.0.4/voxx/__init__.py
+-rw-rw-rw-   0        0        0     3330 2023-04-30 08:05:30.000000 voxx-cli-1.0.4/voxx/__main__.py
+-rw-rw-rw-   0        0        0     3718 2023-04-29 05:54:49.000000 voxx-cli-1.0.4/voxx/connection.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:21:11.055953 voxx-cli-1.0.4/voxx/css/
+-rw-rw-rw-   0        0        0      900 2023-04-28 23:07:53.000000 voxx-cli-1.0.4/voxx/css/tui.css
+-rw-rw-rw-   0        0        0     2333 2023-04-30 00:51:11.000000 voxx-cli-1.0.4/voxx/model.py
+-rw-rw-rw-   0        0        0     5188 2023-04-30 00:51:11.000000 voxx-cli-1.0.4/voxx/tui.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:21:11.063460 voxx-cli-1.0.4/voxx_cli.egg-info/
+-rw-rw-rw-   0        0        0     1084 2023-04-30 08:21:10.000000 voxx-cli-1.0.4/voxx_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-04-30 08:21:11.000000 voxx-cli-1.0.4/voxx_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       29 2023-04-30 08:21:10.000000 voxx-cli-1.0.4/voxx_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-30 08:21:10.000000 voxx-cli-1.0.4/voxx_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-04-30 08:21:10.000000 voxx-cli-1.0.4/voxx_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-30 08:21:10.000000 voxx-cli-1.0.4/voxx_cli.egg-info/top_level.txt
```

### Comparing `voxx-cli-1.0.3/setup.py` & `voxx-cli-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `voxx-cli-1.0.3/voxx/__main__.py` & `voxx-cli-1.0.4/voxx/__main__.py`

 * *Files identical despite different names*

### Comparing `voxx-cli-1.0.3/voxx/connection.py` & `voxx-cli-1.0.4/voxx/connection.py`

 * *Files identical despite different names*

### Comparing `voxx-cli-1.0.3/voxx/css/tui.css` & `voxx-cli-1.0.4/voxx/css/tui.css`

 * *Files identical despite different names*

### Comparing `voxx-cli-1.0.3/voxx/model.py` & `voxx-cli-1.0.4/voxx/model.py`

 * *Files identical despite different names*

### Comparing `voxx-cli-1.0.3/voxx/tui.py` & `voxx-cli-1.0.4/voxx/tui.py`

 * *Files identical despite different names*

