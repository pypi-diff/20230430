# Comparing `tmp/sxlogic-0.4.2.tar.gz` & `tmp/sxlogic-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sxlogic-0.4.2.tar", last modified: Wed Feb 22 00:53:28 2023, max compression
+gzip compressed data, was "dist\sxlogic-0.4.3.tar", last modified: Sun Apr 30 18:33:39 2023, max compression
```

## Comparing `sxlogic-0.4.2.tar` & `sxlogic-0.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-22 00:53:28.000000 sxlogic-0.4.2/
--rw-rw-rw-   0        0        0      455 2023-02-22 00:53:28.000000 sxlogic-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0       34 2021-09-03 11:55:16.000000 sxlogic-0.4.2/README.md
--rw-rw-rw-   0        0        0       42 2023-02-22 00:53:28.000000 sxlogic-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0      894 2023-02-22 00:53:23.000000 sxlogic-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-22 00:53:28.000000 sxlogic-0.4.2/sxlogic/
--rw-rw-rw-   0        0        0    13835 2022-09-25 15:58:08.000000 sxlogic-0.4.2/sxlogic/fpgacap.py
--rw-rw-rw-   0        0        0     1134 2021-09-03 12:09:18.000000 sxlogic-0.4.2/sxlogic/iconvert.py
--rw-rw-rw-   0        0        0     4692 2023-02-22 00:52:02.000000 sxlogic-0.4.2/sxlogic/monocle.py
--rw-rw-rw-   0        0        0     2536 2022-09-25 15:40:43.000000 sxlogic-0.4.2/sxlogic/sxlogic.py
--rw-rw-rw-   0        0        0       80 2021-09-03 12:10:03.000000 sxlogic-0.4.2/sxlogic/__init__.py
--rw-rw-rw-   0        0        0       75 2021-02-12 01:25:50.000000 sxlogic-0.4.2/sxlogic/__main__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 00:53:28.000000 sxlogic-0.4.2/sxlogic.egg-info/
--rw-rw-rw-   0        0        0        1 2023-02-22 00:53:28.000000 sxlogic-0.4.2/sxlogic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2023-02-22 00:53:28.000000 sxlogic-0.4.2/sxlogic.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      455 2023-02-22 00:53:28.000000 sxlogic-0.4.2/sxlogic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-02-22 00:53:28.000000 sxlogic-0.4.2/sxlogic.egg-info/requires.txt
--rw-rw-rw-   0        0        0      323 2023-02-22 00:53:28.000000 sxlogic-0.4.2/sxlogic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-02-22 00:53:28.000000 sxlogic-0.4.2/sxlogic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 18:33:39.000000 sxlogic-0.4.3/
+-rw-rw-rw-   0        0        0      455 2023-04-30 18:33:39.000000 sxlogic-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0       34 2021-09-03 11:55:16.000000 sxlogic-0.4.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 18:33:39.000000 sxlogic-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      894 2023-04-30 18:32:53.000000 sxlogic-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 18:33:38.000000 sxlogic-0.4.3/sxlogic/
+-rw-rw-rw-   0        0        0    13835 2022-09-25 15:58:08.000000 sxlogic-0.4.3/sxlogic/fpgacap.py
+-rw-rw-rw-   0        0        0     1134 2021-09-03 12:09:18.000000 sxlogic-0.4.3/sxlogic/iconvert.py
+-rw-rw-rw-   0        0        0     4946 2023-04-30 14:09:30.000000 sxlogic-0.4.3/sxlogic/monocle.py
+-rw-rw-rw-   0        0        0     2536 2022-09-25 15:40:43.000000 sxlogic-0.4.3/sxlogic/sxlogic.py
+-rw-rw-rw-   0        0        0       80 2021-09-03 12:10:03.000000 sxlogic-0.4.3/sxlogic/__init__.py
+-rw-rw-rw-   0        0        0       75 2021-02-12 01:25:50.000000 sxlogic-0.4.3/sxlogic/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 18:33:39.000000 sxlogic-0.4.3/sxlogic.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-30 18:33:33.000000 sxlogic-0.4.3/sxlogic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2023-04-30 18:33:33.000000 sxlogic-0.4.3/sxlogic.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      455 2023-04-30 18:33:33.000000 sxlogic-0.4.3/sxlogic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-04-30 18:33:33.000000 sxlogic-0.4.3/sxlogic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      323 2023-04-30 18:33:34.000000 sxlogic-0.4.3/sxlogic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-04-30 18:33:33.000000 sxlogic-0.4.3/sxlogic.egg-info/top_level.txt
```

### Comparing `sxlogic-0.4.2/setup.py` & `sxlogic-0.4.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sxlogic",
-    version="0.4.2",
+    version="0.4.3",
     author="StreamLogic, LLC",
     description="StreamLogic Python utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `sxlogic-0.4.2/sxlogic/fpgacap.py` & `sxlogic-0.4.3/sxlogic/fpgacap.py`

 * *Files identical despite different names*

### Comparing `sxlogic-0.4.2/sxlogic/iconvert.py` & `sxlogic-0.4.3/sxlogic/iconvert.py`

 * *Files identical despite different names*

### Comparing `sxlogic-0.4.2/sxlogic/monocle.py` & `sxlogic-0.4.3/sxlogic/monocle.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
 def gw_sh_path(ide_path):
     loc = os.path.dirname(ide_path)
     sh = os.path.join(loc, 'gw_sh.exe')
     return sh
 
 def find_gowin():
+    loc = shutil.which('gw_sh')
+    if loc:
+        return loc
     if sys.platform == 'win32':
         import winreg
         registry = winreg.ConnectRegistry(None,winreg.HKEY_LOCAL_MACHINE)
         key = winreg.OpenKey(registry, r"SOFTWARE\Microsoft\Windows\CurrentVersion\App Paths")
         try:
             return gw_sh_path(winreg.QueryValue(key, "gw_ide.exe"))
         except:
@@ -116,18 +119,22 @@
         print('See build log %s for errors.' % os.path.normpath(outname))
         sys.exit(1)
 
     bitstream = find_fs(build_dir)
     if not bitstream:
         print('ERROR: Output bitstream not found')
 
+    print('SUCCESS! (log in %s)' % os.path.normpath(outname))
+
+    target = os.path.join(build_dir, os.path.join('hw', os.path.basename(bitstream)))
+    shutil.copyfile(bitstream, target)
+    
+    bitstream = os.path.splitext(bitstream)[0]+'.bin'
     target = os.path.join(build_dir, os.path.join('hw', os.path.basename(bitstream)))
     shutil.copyfile(bitstream, target)
-
-    print('SUCCESS! (log in %s)' % os.path.normpath(outname))
 
     print('BUILT', os.path.normpath(target))
 
 def moncole():
     parser = argparse.ArgumentParser(description='monocle')
     parser.add_argument('--gowin', help='Gowin tools directory (saved for future runs)')
     subparsers = parser.add_subparsers(dest='cmd')
```

### Comparing `sxlogic-0.4.2/sxlogic/sxlogic.py` & `sxlogic-0.4.3/sxlogic/sxlogic.py`

 * *Files identical despite different names*

