# Comparing `tmp/escrutinar_jp-0.0.1.tar.gz` & `tmp/escrutinar_jp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "escrutinar_jp-0.0.1.tar", last modified: Wed Dec 14 16:36:42 2022, max compression
+gzip compressed data, was "escrutinar_jp-0.0.4.tar", last modified: Sun Apr 30 03:28:30 2023, max compression
```

## Comparing `escrutinar_jp-0.0.1.tar` & `escrutinar_jp-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jotta     (1000) jotta     (1000)        0 2022-12-14 16:36:42.211120 escrutinar_jp-0.0.1/
--rw-rw-r--   0 jotta     (1000) jotta     (1000)     4292 2022-12-14 16:36:42.211120 escrutinar_jp-0.0.1/PKG-INFO
--rw-rw-r--   0 jotta     (1000) jotta     (1000)     2890 2022-12-14 14:12:09.000000 escrutinar_jp-0.0.1/README.md
-drwxrwxr-x   0 jotta     (1000) jotta     (1000)        0 2022-12-14 16:36:42.191118 escrutinar_jp-0.0.1/escrutinar_jp/
--rw-rw-r--   0 jotta     (1000) jotta     (1000)        0 2022-12-10 23:10:23.000000 escrutinar_jp-0.0.1/escrutinar_jp/__init__.py
--rw-rw-r--   0 jotta     (1000) jotta     (1000)      538 2022-12-10 23:10:23.000000 escrutinar_jp-0.0.1/escrutinar_jp/escrutinar.py
-drwxrwxr-x   0 jotta     (1000) jotta     (1000)        0 2022-12-14 16:36:42.211120 escrutinar_jp-0.0.1/escrutinar_jp.egg-info/
--rw-rw-r--   0 jotta     (1000) jotta     (1000)     4292 2022-12-14 16:36:41.000000 escrutinar_jp-0.0.1/escrutinar_jp.egg-info/PKG-INFO
--rw-rw-r--   0 jotta     (1000) jotta     (1000)      256 2022-12-14 16:36:41.000000 escrutinar_jp-0.0.1/escrutinar_jp.egg-info/SOURCES.txt
--rw-rw-r--   0 jotta     (1000) jotta     (1000)        1 2022-12-14 16:36:41.000000 escrutinar_jp-0.0.1/escrutinar_jp.egg-info/dependency_links.txt
--rw-rw-r--   0 jotta     (1000) jotta     (1000)        9 2022-12-14 16:36:41.000000 escrutinar_jp-0.0.1/escrutinar_jp.egg-info/requires.txt
--rw-rw-r--   0 jotta     (1000) jotta     (1000)       14 2022-12-14 16:36:41.000000 escrutinar_jp-0.0.1/escrutinar_jp.egg-info/top_level.txt
--rw-rw-r--   0 jotta     (1000) jotta     (1000)       38 2022-12-14 16:36:42.211120 escrutinar_jp-0.0.1/setup.cfg
--rw-rw-r--   0 jotta     (1000) jotta     (1000)      650 2022-12-14 16:36:25.000000 escrutinar_jp-0.0.1/setup.py
+drwxr-xr-x   0 jotta     (1000) jotta     (1001)        0 2023-04-30 03:28:30.589064 escrutinar_jp-0.0.4/
+-rw-r--r--   0 jotta     (1000) jotta     (1001)     3681 2023-04-30 03:28:30.585730 escrutinar_jp-0.0.4/PKG-INFO
+-rw-r--r--   0 jotta     (1000) jotta     (1001)     2535 2023-04-30 02:14:06.000000 escrutinar_jp-0.0.4/README.md
+drwxr-xr-x   0 jotta     (1000) jotta     (1001)        0 2023-04-30 03:28:30.579064 escrutinar_jp-0.0.4/escrutinar_jp/
+-rw-r--r--   0 jotta     (1000) jotta     (1001)        0 2023-04-30 00:40:27.000000 escrutinar_jp-0.0.4/escrutinar_jp/__init__.py
+-rw-r--r--   0 jotta     (1000) jotta     (1001)     1231 2023-04-30 00:48:24.000000 escrutinar_jp-0.0.4/escrutinar_jp/escrutinar.py
+drwxr-xr-x   0 jotta     (1000) jotta     (1001)        0 2023-04-30 03:28:30.582397 escrutinar_jp-0.0.4/escrutinar_jp.egg-info/
+-rw-r--r--   0 jotta     (1000) jotta     (1001)     3681 2023-04-30 03:28:29.000000 escrutinar_jp-0.0.4/escrutinar_jp.egg-info/PKG-INFO
+-rw-r--r--   0 jotta     (1000) jotta     (1001)      256 2023-04-30 03:28:30.000000 escrutinar_jp-0.0.4/escrutinar_jp.egg-info/SOURCES.txt
+-rw-r--r--   0 jotta     (1000) jotta     (1001)        1 2023-04-30 03:28:29.000000 escrutinar_jp-0.0.4/escrutinar_jp.egg-info/dependency_links.txt
+-rw-r--r--   0 jotta     (1000) jotta     (1001)        9 2023-04-30 03:28:29.000000 escrutinar_jp-0.0.4/escrutinar_jp.egg-info/requires.txt
+-rw-r--r--   0 jotta     (1000) jotta     (1001)       14 2023-04-30 03:28:29.000000 escrutinar_jp-0.0.4/escrutinar_jp.egg-info/top_level.txt
+-rw-r--r--   0 jotta     (1000) jotta     (1001)       38 2023-04-30 03:28:30.589064 escrutinar_jp-0.0.4/setup.cfg
+-rw-r--r--   0 jotta     (1000) jotta     (1001)      650 2023-04-30 03:27:24.000000 escrutinar_jp-0.0.4/setup.py
```

### Comparing `escrutinar_jp-0.0.1/setup.py` & `escrutinar_jp-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     page_description = f.read()
 
 #with open("requirements.txt", "r") as f:
 #    requirements = f.read().splitlines()
 
 setup(
     name="escrutinar_jp",
-    version="0.0.1",
+    version="0.0.4",
     author="Jorge Paulo",
     author_email="jorgepsan7@gmail.com",
     description="pegar o IP de um determinado site, coletar dados de um determinado IP.",
     long_description=page_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JP-Linux/projeto_escrutinar",
     packages=find_packages(),
```

