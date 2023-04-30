# Comparing `tmp/libtukaan-unix-0.1.3.tar.gz` & `tmp/libtukaan-unix-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libtukaan-unix-0.1.3.tar", last modified: Thu Apr  6 13:08:42 2023, max compression
+gzip compressed data, was "libtukaan-unix-0.1.4.tar", last modified: Sun Apr 30 17:56:28 2023, max compression
```

## Comparing `libtukaan-unix-0.1.3.tar` & `libtukaan-unix-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:08:42.455684 libtukaan-unix-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-06 13:08:42.455684 libtukaan-unix-0.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:08:42.455684 libtukaan-unix-0.1.3/libtukaan/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-06 13:08:33.000000 libtukaan-unix-0.1.3/libtukaan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-06 13:08:33.000000 libtukaan-unix-0.1.3/libtukaan/serif.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:08:42.455684 libtukaan-unix-0.1.3/libtukaan/unix/
--rwxr-xr-x   0 runner    (1001) docker     (123)    16920 2023-04-06 13:08:33.000000 libtukaan-unix-0.1.3/libtukaan/unix/libserif_x64.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:08:42.455684 libtukaan-unix-0.1.3/libtukaan_unix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-06 13:08:42.000000 libtukaan-unix-0.1.3/libtukaan_unix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-06 13:08:42.000000 libtukaan-unix-0.1.3/libtukaan_unix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 13:08:42.000000 libtukaan-unix-0.1.3/libtukaan_unix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-06 13:08:42.000000 libtukaan-unix-0.1.3/libtukaan_unix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 13:08:42.455684 libtukaan-unix-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-06 13:08:33.000000 libtukaan-unix-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:56:28.638704 libtukaan-unix-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-30 17:56:28.638704 libtukaan-unix-0.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:56:28.638704 libtukaan-unix-0.1.4/libtukaan/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-30 17:56:18.000000 libtukaan-unix-0.1.4/libtukaan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-30 17:56:18.000000 libtukaan-unix-0.1.4/libtukaan/serif.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:56:28.638704 libtukaan-unix-0.1.4/libtukaan/unix/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16920 2023-04-30 17:56:18.000000 libtukaan-unix-0.1.4/libtukaan/unix/libserif_x64.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16624 2023-04-30 17:56:18.000000 libtukaan-unix-0.1.4/libtukaan/unix/libtkxcursor_x64.so
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-30 17:56:18.000000 libtukaan-unix-0.1.4/libtukaan/xcursor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:56:28.638704 libtukaan-unix-0.1.4/libtukaan_unix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-30 17:56:28.000000 libtukaan-unix-0.1.4/libtukaan_unix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-30 17:56:28.000000 libtukaan-unix-0.1.4/libtukaan_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 17:56:28.000000 libtukaan-unix-0.1.4/libtukaan_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-30 17:56:28.000000 libtukaan-unix-0.1.4/libtukaan_unix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 17:56:28.638704 libtukaan-unix-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-30 17:56:18.000000 libtukaan-unix-0.1.4/setup.py
```

### Comparing `libtukaan-unix-0.1.3/libtukaan/serif.py` & `libtukaan-unix-0.1.4/libtukaan/serif.py`

 * *Files identical despite different names*

### Comparing `libtukaan-unix-0.1.3/libtukaan/unix/libserif_x64.so` & `libtukaan-unix-0.1.4/libtukaan/unix/libserif_x64.so`

 * *Files identical despite different names*

### Comparing `libtukaan-unix-0.1.3/setup.py` & `libtukaan-unix-0.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from setuptools import setup
 
 platform = {"darwin": "mac", "win32": "win"}.get(sys.platform, "unix")
 
 
 setup(
     name=f"libtukaan-{platform}",
-    version="0.1.3",
+    version="0.1.4",
     license="MIT",
     author="rdbende",
-    author_email="rdbende@gmail.com",
+    author_email="rdbende@proton.me",
     description="Binary extensions for Tukaan",
     url="https://tukaan.github.io",
     project_urls={
-        "Documentation": "https://tukaan.github.io/docs",
         "Source": "https://github.com/tukaan/libtukaan",
+        "Documentation": "https://tukaan.github.io/docs",
         "Tracker": "https://github.com/tukaan/libtukaan/issues",
     },
     python_requires=">=3.7",
     packages=["libtukaan"],
     package_data={"libtukaan": [f"{platform}/*.*"]},
 )
```

