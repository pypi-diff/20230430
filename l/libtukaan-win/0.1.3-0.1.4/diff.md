# Comparing `tmp/libtukaan-win-0.1.3.tar.gz` & `tmp/libtukaan-win-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libtukaan-win-0.1.3.tar", last modified: Thu Apr  6 13:11:39 2023, max compression
+gzip compressed data, was "libtukaan-win-0.1.4.tar", last modified: Sun Apr 30 17:57:15 2023, max compression
```

## Comparing `libtukaan-win-0.1.3.tar` & `libtukaan-win-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 13:11:39.567260 libtukaan-win-0.1.3/
--rw-rw-rw-   0        0        0      439 2023-04-06 13:11:39.567260 libtukaan-win-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-06 13:11:39.567260 libtukaan-win-0.1.3/libtukaan/
--rw-rw-rw-   0        0        0       26 2023-04-06 13:11:08.000000 libtukaan-win-0.1.3/libtukaan/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-04-06 13:11:08.000000 libtukaan-win-0.1.3/libtukaan/serif.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:11:39.567260 libtukaan-win-0.1.3/libtukaan/win/
--rw-rw-rw-   0        0        0    11776 2023-04-06 13:11:08.000000 libtukaan-win-0.1.3/libtukaan/win/libserif_x64.dll
-drwxrwxrwx   0        0        0        0 2023-04-06 13:11:39.567260 libtukaan-win-0.1.3/libtukaan_win.egg-info/
--rw-rw-rw-   0        0        0      439 2023-04-06 13:11:39.000000 libtukaan-win-0.1.3/libtukaan_win.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-04-06 13:11:39.000000 libtukaan-win-0.1.3/libtukaan_win.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 13:11:39.000000 libtukaan-win-0.1.3/libtukaan_win.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-06 13:11:39.000000 libtukaan-win-0.1.3/libtukaan_win.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 13:11:39.567260 libtukaan-win-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      682 2023-04-06 13:11:08.000000 libtukaan-win-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 17:57:15.758241 libtukaan-win-0.1.4/
+-rw-rw-rw-   0        0        0      439 2023-04-30 17:57:15.758241 libtukaan-win-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-30 17:57:15.758241 libtukaan-win-0.1.4/libtukaan/
+-rw-rw-rw-   0        0        0       56 2023-04-30 17:56:36.000000 libtukaan-win-0.1.4/libtukaan/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-04-30 17:56:36.000000 libtukaan-win-0.1.4/libtukaan/serif.py
+drwxrwxrwx   0        0        0        0 2023-04-30 17:57:15.758241 libtukaan-win-0.1.4/libtukaan/win/
+-rw-rw-rw-   0        0        0    11776 2023-04-30 17:56:36.000000 libtukaan-win-0.1.4/libtukaan/win/libserif_x64.dll
+-rw-rw-rw-   0        0        0     1544 2023-04-30 17:56:36.000000 libtukaan-win-0.1.4/libtukaan/xcursor.py
+drwxrwxrwx   0        0        0        0 2023-04-30 17:57:15.758241 libtukaan-win-0.1.4/libtukaan_win.egg-info/
+-rw-rw-rw-   0        0        0      439 2023-04-30 17:57:15.000000 libtukaan-win-0.1.4/libtukaan_win.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-30 17:57:15.000000 libtukaan-win-0.1.4/libtukaan_win.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 17:57:15.000000 libtukaan-win-0.1.4/libtukaan_win.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-30 17:57:15.000000 libtukaan-win-0.1.4/libtukaan_win.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 17:57:15.758241 libtukaan-win-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      682 2023-04-30 17:56:36.000000 libtukaan-win-0.1.4/setup.py
```

### Comparing `libtukaan-win-0.1.3/libtukaan/serif.py` & `libtukaan-win-0.1.4/libtukaan/serif.py`

 * *Files identical despite different names*

### Comparing `libtukaan-win-0.1.3/libtukaan/win/libserif_x64.dll` & `libtukaan-win-0.1.4/libtukaan/win/libserif_x64.dll`

 * *Files identical despite different names*

### Comparing `libtukaan-win-0.1.3/setup.py` & `libtukaan-win-0.1.4/setup.py`

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

