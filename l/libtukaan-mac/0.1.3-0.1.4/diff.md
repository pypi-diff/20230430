# Comparing `tmp/libtukaan-mac-0.1.3.tar.gz` & `tmp/libtukaan-mac-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libtukaan-mac-0.1.3.tar", last modified: Thu Apr  6 13:08:53 2023, max compression
+gzip compressed data, was "libtukaan-mac-0.1.4.tar", last modified: Sun Apr 30 17:57:09 2023, max compression
```

## Comparing `libtukaan-mac-0.1.3.tar` & `libtukaan-mac-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-06 13:08:53.953196 libtukaan-mac-0.1.3/
--rw-r--r--   0 runner     (501) staff       (20)      423 2023-04-06 13:08:53.952806 libtukaan-mac-0.1.3/PKG-INFO
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-06 13:08:53.949673 libtukaan-mac-0.1.3/libtukaan/
--rw-r--r--   0 runner     (501) staff       (20)       25 2023-04-06 13:08:42.000000 libtukaan-mac-0.1.3/libtukaan/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-06 13:08:53.950126 libtukaan-mac-0.1.3/libtukaan/mac/
--rw-r--r--   0 runner     (501) staff       (20)    49992 2023-04-06 13:08:42.000000 libtukaan-mac-0.1.3/libtukaan/mac/libserif_x64.dylib
--rw-r--r--   0 runner     (501) staff       (20)     1612 2023-04-06 13:08:42.000000 libtukaan-mac-0.1.3/libtukaan/serif.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-06 13:08:53.952223 libtukaan-mac-0.1.3/libtukaan_mac.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)      423 2023-04-06 13:08:53.000000 libtukaan-mac-0.1.3/libtukaan_mac.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      230 2023-04-06 13:08:53.000000 libtukaan-mac-0.1.3/libtukaan_mac.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-06 13:08:53.000000 libtukaan-mac-0.1.3/libtukaan_mac.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       10 2023-04-06 13:08:53.000000 libtukaan-mac-0.1.3/libtukaan_mac.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-06 13:08:53.953314 libtukaan-mac-0.1.3/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      658 2023-04-06 13:08:42.000000 libtukaan-mac-0.1.3/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 17:57:09.662782 libtukaan-mac-0.1.4/
+-rw-r--r--   0 runner     (501) staff       (20)      423 2023-04-30 17:57:09.662347 libtukaan-mac-0.1.4/PKG-INFO
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 17:57:09.659061 libtukaan-mac-0.1.4/libtukaan/
+-rw-r--r--   0 runner     (501) staff       (20)       54 2023-04-30 17:56:57.000000 libtukaan-mac-0.1.4/libtukaan/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 17:57:09.659678 libtukaan-mac-0.1.4/libtukaan/mac/
+-rw-r--r--   0 runner     (501) staff       (20)    49992 2023-04-30 17:56:57.000000 libtukaan-mac-0.1.4/libtukaan/mac/libserif_x64.dylib
+-rw-r--r--   0 runner     (501) staff       (20)     1612 2023-04-30 17:56:57.000000 libtukaan-mac-0.1.4/libtukaan/serif.py
+-rw-r--r--   0 runner     (501) staff       (20)     1495 2023-04-30 17:56:57.000000 libtukaan-mac-0.1.4/libtukaan/xcursor.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 17:57:09.661681 libtukaan-mac-0.1.4/libtukaan_mac.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)      423 2023-04-30 17:57:09.000000 libtukaan-mac-0.1.4/libtukaan_mac.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      251 2023-04-30 17:57:09.000000 libtukaan-mac-0.1.4/libtukaan_mac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-30 17:57:09.000000 libtukaan-mac-0.1.4/libtukaan_mac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       10 2023-04-30 17:57:09.000000 libtukaan-mac-0.1.4/libtukaan_mac.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-30 17:57:09.662922 libtukaan-mac-0.1.4/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      658 2023-04-30 17:56:57.000000 libtukaan-mac-0.1.4/setup.py
```

### Comparing `libtukaan-mac-0.1.3/libtukaan/mac/libserif_x64.dylib` & `libtukaan-mac-0.1.4/libtukaan/mac/libserif_x64.dylib`

 * *Files identical despite different names*

### Comparing `libtukaan-mac-0.1.3/libtukaan/serif.py` & `libtukaan-mac-0.1.4/libtukaan/serif.py`

 * *Files identical despite different names*

### Comparing `libtukaan-mac-0.1.3/setup.py` & `libtukaan-mac-0.1.4/setup.py`

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

