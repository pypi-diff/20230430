# Comparing `tmp/UzbekTagger-0.0.5.tar.gz` & `tmp/UzbekTagger-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UzbekTagger-0.0.5.tar", last modified: Sun Apr 30 09:21:21 2023, max compression
+gzip compressed data, was "UzbekTagger-0.0.6.tar", last modified: Sun Apr 30 09:32:50 2023, max compression
```

## Comparing `UzbekTagger-0.0.5.tar` & `UzbekTagger-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 09:21:21.255285 UzbekTagger-0.0.5/
--rw-rw-rw-   0        0        0    11558 2022-12-22 05:23:51.000000 UzbekTagger-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      716 2023-04-30 09:21:21.255285 UzbekTagger-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-03-02 11:43:55.000000 UzbekTagger-0.0.5/README.md
--rw-rw-rw-   0        0        0      502 2023-04-30 03:43:09.000000 UzbekTagger-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 09:21:21.255285 UzbekTagger-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1213 2023-04-30 09:18:27.000000 UzbekTagger-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 09:21:21.218707 UzbekTagger-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 09:21:21.223991 UzbekTagger-0.0.5/src/UzbekTagger/
--rw-rw-rw-   0        0        0     4687 2023-04-30 03:43:09.000000 UzbekTagger-0.0.5/src/UzbekTagger/UzbekTagger.py
--rw-rw-rw-   0        0        0        0 2023-04-30 03:55:06.000000 UzbekTagger-0.0.5/src/UzbekTagger/__init__.py
--rw-rw-rw-   0        0        0     1339 2023-03-13 10:27:15.000000 UzbekTagger-0.0.5/src/UzbekTagger/service_to_uzbek_text.py
--rw-rw-rw-   0        0        0  4038555 2023-04-30 03:38:16.000000 UzbekTagger-0.0.5/src/UzbekTagger/word.xml
-drwxrwxrwx   0        0        0        0 2023-04-30 09:21:21.255285 UzbekTagger-0.0.5/src/UzbekTagger.egg-info/
--rw-rw-rw-   0        0        0      716 2023-04-30 09:21:21.000000 UzbekTagger-0.0.5/src/UzbekTagger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-04-30 09:21:21.000000 UzbekTagger-0.0.5/src/UzbekTagger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 09:21:21.000000 UzbekTagger-0.0.5/src/UzbekTagger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-30 09:21:21.000000 UzbekTagger-0.0.5/src/UzbekTagger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 09:32:50.579475 UzbekTagger-0.0.6/
+-rw-rw-rw-   0        0        0    11558 2022-12-22 05:23:51.000000 UzbekTagger-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      716 2023-04-30 09:32:50.570177 UzbekTagger-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-03-02 11:43:55.000000 UzbekTagger-0.0.6/README.md
+-rw-rw-rw-   0        0        0      502 2023-04-30 09:32:19.000000 UzbekTagger-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 09:32:50.579475 UzbekTagger-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1213 2023-04-30 09:32:19.000000 UzbekTagger-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 09:32:50.554661 UzbekTagger-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 09:32:50.570177 UzbekTagger-0.0.6/src/UzbekTagger/
+-rw-rw-rw-   0        0        0     4704 2023-04-30 09:32:19.000000 UzbekTagger-0.0.6/src/UzbekTagger/UzbekTagger.py
+-rw-rw-rw-   0        0        0        0 2023-04-30 03:55:06.000000 UzbekTagger-0.0.6/src/UzbekTagger/__init__.py
+-rw-rw-rw-   0        0        0     1339 2023-03-13 10:27:15.000000 UzbekTagger-0.0.6/src/UzbekTagger/service_to_uzbek_text.py
+-rw-rw-rw-   0        0        0  4038555 2023-04-30 03:38:16.000000 UzbekTagger-0.0.6/src/UzbekTagger/word.xml
+drwxrwxrwx   0        0        0        0 2023-04-30 09:32:50.570177 UzbekTagger-0.0.6/src/UzbekTagger.egg-info/
+-rw-rw-rw-   0        0        0      716 2023-04-30 09:32:50.000000 UzbekTagger-0.0.6/src/UzbekTagger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-04-30 09:32:50.000000 UzbekTagger-0.0.6/src/UzbekTagger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 09:32:50.000000 UzbekTagger-0.0.6/src/UzbekTagger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-30 09:32:50.000000 UzbekTagger-0.0.6/src/UzbekTagger.egg-info/top_level.txt
```

### Comparing `UzbekTagger-0.0.5/LICENSE` & `UzbekTagger-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `UzbekTagger-0.0.5/PKG-INFO` & `UzbekTagger-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UzbekTagger
-Version: 0.0.5
+Version: 0.0.6
 Summary: Part of Speech Tagger for Uzbek Language.
 Home-page: https://https://github.com/MaksudSharipov/UzbekTokenizer
 Author: Maksud Sharipov, Ollabergan Yuldashov
 Author-email: "Sharipov Maksud,Yuldashov Ollabergan" <maqsbek72@gmail.com>
 Project-URL: Homepage, https://https://github.com/MaksudSharipov/UzbekTokenizer
 Keywords: python,UzbekTagger,uzbek texts,Tagger,POS,Part of Speech
 Classifier: Programming Language :: Python :: 3
```

### Comparing `UzbekTagger-0.0.5/setup.py` & `UzbekTagger-0.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="UzbekTagger",
-    version="0.0.5",
+    version="0.0.6",
     author="Maksud Sharipov, Ollabergan Yuldashov",
     author_email="maqsbek72@gmail.com, ollaberganyuldashov@gmail.com",
     description="Part of Speech Tagger for Uzbek Language.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://https://github.com/MaksudSharipov/UzbekTokenizer",
     project_urls={
```

### Comparing `UzbekTagger-0.0.5/src/UzbekTagger/UzbekTagger.py` & `UzbekTagger-0.0.6/src/UzbekTagger/UzbekTagger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import service_to_uzbek_text
+from UzbekTagger import service_to_uzbek_text
 import xml.etree.ElementTree as et
 from pathlib import Path
 from lxml import etree
 
 
 class pos:
     __this_directory = Path(__file__).parent
```

### Comparing `UzbekTagger-0.0.5/src/UzbekTagger/service_to_uzbek_text.py` & `UzbekTagger-0.0.6/src/UzbekTagger/service_to_uzbek_text.py`

 * *Files identical despite different names*

### Comparing `UzbekTagger-0.0.5/src/UzbekTagger/word.xml` & `UzbekTagger-0.0.6/src/UzbekTagger/word.xml`

 * *Files identical despite different names*

### Comparing `UzbekTagger-0.0.5/src/UzbekTagger.egg-info/PKG-INFO` & `UzbekTagger-0.0.6/src/UzbekTagger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UzbekTagger
-Version: 0.0.5
+Version: 0.0.6
 Summary: Part of Speech Tagger for Uzbek Language.
 Home-page: https://https://github.com/MaksudSharipov/UzbekTokenizer
 Author: Maksud Sharipov, Ollabergan Yuldashov
 Author-email: "Sharipov Maksud,Yuldashov Ollabergan" <maqsbek72@gmail.com>
 Project-URL: Homepage, https://https://github.com/MaksudSharipov/UzbekTokenizer
 Keywords: python,UzbekTagger,uzbek texts,Tagger,POS,Part of Speech
 Classifier: Programming Language :: Python :: 3
```

