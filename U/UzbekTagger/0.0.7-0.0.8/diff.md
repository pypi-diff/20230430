# Comparing `tmp/UzbekTagger-0.0.7.tar.gz` & `tmp/UzbekTagger-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UzbekTagger-0.0.7.tar", last modified: Sun Apr 30 09:45:57 2023, max compression
+gzip compressed data, was "UzbekTagger-0.0.8.tar", last modified: Sun Apr 30 09:52:54 2023, max compression
```

## Comparing `UzbekTagger-0.0.7.tar` & `UzbekTagger-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 09:45:57.931465 UzbekTagger-0.0.7/
--rw-rw-rw-   0        0        0    11558 2022-12-22 05:23:51.000000 UzbekTagger-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      716 2023-04-30 09:45:57.931465 UzbekTagger-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-03-02 11:43:55.000000 UzbekTagger-0.0.7/README.md
--rw-rw-rw-   0        0        0      502 2023-04-30 09:44:57.000000 UzbekTagger-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 09:45:57.931465 UzbekTagger-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1213 2023-04-30 09:44:57.000000 UzbekTagger-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 09:45:57.905199 UzbekTagger-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 09:45:57.931465 UzbekTagger-0.0.7/src/UzbekTagger/
--rw-rw-rw-   0        0        0     6217 2023-04-30 09:44:21.000000 UzbekTagger-0.0.7/src/UzbekTagger/UzbekTagger.py
--rw-rw-rw-   0        0        0        0 2023-04-30 03:55:06.000000 UzbekTagger-0.0.7/src/UzbekTagger/__init__.py
--rw-rw-rw-   0        0        0  4038555 2023-04-30 03:38:16.000000 UzbekTagger-0.0.7/src/UzbekTagger/word.xml
-drwxrwxrwx   0        0        0        0 2023-04-30 09:45:57.931465 UzbekTagger-0.0.7/src/UzbekTagger.egg-info/
--rw-rw-rw-   0        0        0      716 2023-04-30 09:45:57.000000 UzbekTagger-0.0.7/src/UzbekTagger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-04-30 09:45:57.000000 UzbekTagger-0.0.7/src/UzbekTagger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 09:45:57.000000 UzbekTagger-0.0.7/src/UzbekTagger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-30 09:45:57.000000 UzbekTagger-0.0.7/src/UzbekTagger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 09:52:54.581205 UzbekTagger-0.0.8/
+-rw-rw-rw-   0        0        0    11558 2022-12-22 05:23:51.000000 UzbekTagger-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      716 2023-04-30 09:52:54.581205 UzbekTagger-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-03-02 11:43:55.000000 UzbekTagger-0.0.8/README.md
+-rw-rw-rw-   0        0        0      502 2023-04-30 09:52:39.000000 UzbekTagger-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 09:52:54.581205 UzbekTagger-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1213 2023-04-30 09:52:39.000000 UzbekTagger-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 09:52:54.565505 UzbekTagger-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 09:52:54.565505 UzbekTagger-0.0.8/src/UzbekTagger/
+-rw-rw-rw-   0        0        0     6218 2023-04-30 09:52:22.000000 UzbekTagger-0.0.8/src/UzbekTagger/UzbekTagger.py
+-rw-rw-rw-   0        0        0        0 2023-04-30 03:55:06.000000 UzbekTagger-0.0.8/src/UzbekTagger/__init__.py
+-rw-rw-rw-   0        0        0  4038555 2023-04-30 03:38:16.000000 UzbekTagger-0.0.8/src/UzbekTagger/word.xml
+drwxrwxrwx   0        0        0        0 2023-04-30 09:52:54.581205 UzbekTagger-0.0.8/src/UzbekTagger.egg-info/
+-rw-rw-rw-   0        0        0      716 2023-04-30 09:52:54.000000 UzbekTagger-0.0.8/src/UzbekTagger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-04-30 09:52:54.000000 UzbekTagger-0.0.8/src/UzbekTagger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 09:52:54.000000 UzbekTagger-0.0.8/src/UzbekTagger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-30 09:52:54.000000 UzbekTagger-0.0.8/src/UzbekTagger.egg-info/top_level.txt
```

### Comparing `UzbekTagger-0.0.7/LICENSE` & `UzbekTagger-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `UzbekTagger-0.0.7/PKG-INFO` & `UzbekTagger-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UzbekTagger
-Version: 0.0.7
+Version: 0.0.8
 Summary: Part of Speech Tagger for Uzbek Language.
 Home-page: https://https://github.com/MaksudSharipov/UzbekTokenizer
 Author: Maksud Sharipov, Ollabergan Yuldashov
 Author-email: "Sharipov Maksud,Yuldashov Ollabergan" <maqsbek72@gmail.com>
 Project-URL: Homepage, https://https://github.com/MaksudSharipov/UzbekTokenizer
 Keywords: python,UzbekTagger,uzbek texts,Tagger,POS,Part of Speech
 Classifier: Programming Language :: Python :: 3
```

### Comparing `UzbekTagger-0.0.7/setup.py` & `UzbekTagger-0.0.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="UzbekTagger",
-    version="0.0.7",
+    version="0.0.8",
     author="Maksud Sharipov, Ollabergan Yuldashov",
     author_email="maqsbek72@gmail.com, ollaberganyuldashov@gmail.com",
     description="Part of Speech Tagger for Uzbek Language.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://https://github.com/MaksudSharipov/UzbekTokenizer",
     project_urls={
```

### Comparing `UzbekTagger-0.0.7/src/UzbekTagger/UzbekTagger.py` & `UzbekTagger-0.0.8/src/UzbekTagger/UzbekTagger.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,8 +172,8 @@
             for i in range(len(tagged_list)):
                 tagged_sent=tagged_sent+' '+tagged_list[i]['word']+'/'+tagged_list[i]['pos']
             tagged_sent=tagged_sent+' '+punk+'/PUNCT\n'
             tagged_text=tagged_text+tagged_sent
             #print(tagged_sent)
         return tagged_text
 
-print(pos.tagger("Men bugun uyga bordim"))
+#print(pos.tagger("Men bugun uyga bordim"))
```

### Comparing `UzbekTagger-0.0.7/src/UzbekTagger/word.xml` & `UzbekTagger-0.0.8/src/UzbekTagger/word.xml`

 * *Files identical despite different names*

### Comparing `UzbekTagger-0.0.7/src/UzbekTagger.egg-info/PKG-INFO` & `UzbekTagger-0.0.8/src/UzbekTagger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UzbekTagger
-Version: 0.0.7
+Version: 0.0.8
 Summary: Part of Speech Tagger for Uzbek Language.
 Home-page: https://https://github.com/MaksudSharipov/UzbekTokenizer
 Author: Maksud Sharipov, Ollabergan Yuldashov
 Author-email: "Sharipov Maksud,Yuldashov Ollabergan" <maqsbek72@gmail.com>
 Project-URL: Homepage, https://https://github.com/MaksudSharipov/UzbekTokenizer
 Keywords: python,UzbekTagger,uzbek texts,Tagger,POS,Part of Speech
 Classifier: Programming Language :: Python :: 3
```

