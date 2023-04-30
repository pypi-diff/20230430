# Comparing `tmp/dragonfile-1.0.4.tar.gz` & `tmp/dragonfile-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragonfile-1.0.4.tar", last modified: Sun Apr 30 02:57:51 2023, max compression
+gzip compressed data, was "dragonfile-1.0.5.tar", last modified: Sun Apr 30 04:16:22 2023, max compression
```

## Comparing `dragonfile-1.0.4.tar` & `dragonfile-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 02:57:51.550401 dragonfile-1.0.4/
--rw-rw-rw-   0        0        0     1086 2023-04-20 21:04:35.000000 dragonfile-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      771 2023-04-30 02:57:51.542405 dragonfile-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2091 2023-04-22 02:49:35.000000 dragonfile-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 02:57:51.426476 dragonfile-1.0.4/dragonfile/
--rw-rw-rw-   0        0        0     5439 2023-04-30 02:54:53.000000 dragonfile-1.0.4/dragonfile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 02:57:51.525414 dragonfile-1.0.4/dragonfile.egg-info/
--rw-rw-rw-   0        0        0      771 2023-04-30 02:57:50.000000 dragonfile-1.0.4/dragonfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-04-30 02:57:51.000000 dragonfile-1.0.4/dragonfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 02:57:50.000000 dragonfile-1.0.4/dragonfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-30 02:57:50.000000 dragonfile-1.0.4/dragonfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 02:57:51.551399 dragonfile-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      864 2023-04-30 02:57:21.000000 dragonfile-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 02:57:51.537409 dragonfile-1.0.4/tests/
--rw-rw-rw-   0        0        0        8 2023-04-22 04:26:27.000000 dragonfile-1.0.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 04:16:22.090764 dragonfile-1.0.5/
+-rw-rw-rw-   0        0        0     1086 2023-04-20 21:04:35.000000 dragonfile-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      771 2023-04-30 04:16:22.086768 dragonfile-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2091 2023-04-22 02:49:35.000000 dragonfile-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 04:16:21.985828 dragonfile-1.0.5/dragonfile/
+-rw-rw-rw-   0        0        0     1212 2023-04-30 04:16:01.000000 dragonfile-1.0.5/dragonfile/__init__.py
+-rw-rw-rw-   0        0        0      253 2023-04-30 04:02:17.000000 dragonfile-1.0.5/dragonfile/fileToCsv.py
+-rw-rw-rw-   0        0        0      231 2023-04-30 04:02:39.000000 dragonfile-1.0.5/dragonfile/lenColumns.py
+-rw-rw-rw-   0        0        0      601 2023-04-30 03:59:33.000000 dragonfile-1.0.5/dragonfile/readFile.py
+-rw-rw-rw-   0        0        0     1186 2023-04-30 04:01:23.000000 dragonfile-1.0.5/dragonfile/readFileRename.py
+-rw-rw-rw-   0        0        0     1879 2023-04-30 04:01:00.000000 dragonfile-1.0.5/dragonfile/readFileSetPeriod.py
+-rw-rw-rw-   0        0        0      778 2023-04-30 04:01:53.000000 dragonfile-1.0.5/dragonfile/readValues.py
+drwxrwxrwx   0        0        0        0 2023-04-30 04:16:22.067780 dragonfile-1.0.5/dragonfile.egg-info/
+-rw-rw-rw-   0        0        0      771 2023-04-30 04:16:21.000000 dragonfile-1.0.5/dragonfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-04-30 04:16:21.000000 dragonfile-1.0.5/dragonfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 04:16:21.000000 dragonfile-1.0.5/dragonfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-30 04:16:21.000000 dragonfile-1.0.5/dragonfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 04:16:22.091765 dragonfile-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      864 2023-04-30 04:16:10.000000 dragonfile-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 04:16:22.080771 dragonfile-1.0.5/tests/
+-rw-rw-rw-   0        0        0        8 2023-04-22 04:26:27.000000 dragonfile-1.0.5/tests/__init__.py
```

### Comparing `dragonfile-1.0.4/LICENSE` & `dragonfile-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dragonfile-1.0.4/PKG-INFO` & `dragonfile-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfile
-Version: 1.0.4
+Version: 1.0.5
 Summary: Read CSV - Version Test
 Author: Gabriel Arantd Felipe
 Author-email: grantd.ctt@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dragonfile-1.0.4/README.md` & `dragonfile-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dragonfile-1.0.4/dragonfile.egg-info/PKG-INFO` & `dragonfile-1.0.5/dragonfile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfile
-Version: 1.0.4
+Version: 1.0.5
 Summary: Read CSV - Version Test
 Author: Gabriel Arantd Felipe
 Author-email: grantd.ctt@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dragonfile-1.0.4/setup.py` & `dragonfile-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dragonfile',
-    version='1.0.4',
+    version='1.0.5',
     description='Read CSV - Version Test',
     author='Gabriel Arantd Felipe',
     author_email='grantd.ctt@gmail.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

