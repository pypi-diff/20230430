# Comparing `tmp/noteyXMLParser-0.2.7.tar.gz` & `tmp/noteyXMLParser-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/noteyXMLParser-0.2.7.tar", last modified: Wed Apr 12 21:51:36 2023, max compression
+gzip compressed data, was "dist/noteyXMLParser-0.2.8.tar", last modified: Sat Apr 29 22:38:39 2023, max compression
```

## Comparing `noteyXMLParser-0.2.7.tar` & `noteyXMLParser-0.2.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxr-xr-x   0 aminmahjoub   (501) staff       (20)        0 2023-04-12 21:51:36.627603 noteyXMLParser-0.2.7/
--rw-r--r--   0 aminmahjoub   (501) staff       (20)      904 2023-04-12 21:51:36.627336 noteyXMLParser-0.2.7/PKG-INFO
--rw-r--r--   0 aminmahjoub   (501) staff       (20)      359 2023-04-11 06:22:11.000000 noteyXMLParser-0.2.7/README.md
--rw-r--r--   0 aminmahjoub   (501) staff       (20)       38 2023-04-12 21:51:36.627743 noteyXMLParser-0.2.7/setup.cfg
--rw-r--r--   0 aminmahjoub   (501) staff       (20)      689 2023-04-12 21:51:14.000000 noteyXMLParser-0.2.7/setup.py
+drwxr-xr-x   0 aminmahjoub   (501) staff       (20)        0 2023-04-29 22:38:39.397964 noteyXMLParser-0.2.8/
+-rw-r--r--   0 aminmahjoub   (501) staff       (20)      904 2023-04-29 22:38:39.397456 noteyXMLParser-0.2.8/PKG-INFO
+-rw-r--r--   0 aminmahjoub   (501) staff       (20)      359 2023-04-11 06:22:11.000000 noteyXMLParser-0.2.8/README.md
+-rw-r--r--   0 aminmahjoub   (501) staff       (20)       38 2023-04-29 22:38:39.398169 noteyXMLParser-0.2.8/setup.cfg
+-rw-r--r--   0 aminmahjoub   (501) staff       (20)      689 2023-04-29 22:38:32.000000 noteyXMLParser-0.2.8/setup.py
```

### Comparing `noteyXMLParser-0.2.7/PKG-INFO` & `noteyXMLParser-0.2.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noteyXMLParser
-Version: 0.2.7
+Version: 0.2.8
 Summary: Music XML Parser
 Home-page: https://github.com/mmahjoub5/NoteyXMLParser
 Author: Amin Mahjoub
 Author-email: mahjoub@usc.edu
 License: UNKNOWN
 Description: my parser
```

### Comparing `noteyXMLParser-0.2.7/setup.py` & `noteyXMLParser-0.2.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
      name='noteyXMLParser',  
-     version='0.2.7',
+     version='0.2.8',
      author="Amin Mahjoub",
      author_email="mahjoub@usc.edu",
      description="Music XML Parser",
      long_description=long_description,
      package_dir={"":"/Users/aminmahjoub/NoteyXMLParser/xmlParser/src"},
      url="https://github.com/mmahjoub5/NoteyXMLParser",
    long_description_content_type="text/markdown",
```

