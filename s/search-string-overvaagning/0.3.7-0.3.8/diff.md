# Comparing `tmp/search_string_overvaagning-0.3.7-py3-none-any.whl.zip` & `tmp/search_string_overvaagning-0.3.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 16383 bytes, number of entries: 11
--rw-r--r--  2.0 unx      239 b- defN 23-Apr-15 05:59 search_string/__init__.py
--rw-r--r--  2.0 unx      385 b- defN 23-Apr-15 05:59 search_string/constants.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-15 05:59 search_string/py.typed
--rw-r--r--  2.0 unx    21840 b- defN 23-Apr-15 05:59 search_string/search_string.py
--rw-r--r--  2.0 unx    12295 b- defN 23-Apr-15 05:59 search_string/search_string_collection.py
--rw-r--r--  2.0 unx       58 b- defN 23-Apr-15 05:59 search_string/version.py
--rw-r--r--  2.0 unx     4074 b- defN 23-Apr-15 06:00 search_string_overvaagning-0.3.7.dist-info/LICENSE
--rw-r--r--  2.0 unx    10296 b- defN 23-Apr-15 06:00 search_string_overvaagning-0.3.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 06:00 search_string_overvaagning-0.3.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-15 06:00 search_string_overvaagning-0.3.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      987 b- defN 23-Apr-15 06:00 search_string_overvaagning-0.3.7.dist-info/RECORD
-11 files, 50280 bytes uncompressed, 14681 bytes compressed:  70.8%
+Zip file size: 16463 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      239 b- defN 23-Apr-30 20:28 search_string/__init__.py
+-rw-r--r--  2.0 unx      385 b- defN 23-Apr-30 20:28 search_string/constants.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-30 20:28 search_string/py.typed
+-rw-r--r--  2.0 unx    21840 b- defN 23-Apr-30 20:28 search_string/search_string.py
+-rw-r--r--  2.0 unx    12295 b- defN 23-Apr-30 20:28 search_string/search_string_collection.py
+-rw-r--r--  2.0 unx       58 b- defN 23-Apr-30 20:28 search_string/version.py
+-rw-r--r--  2.0 unx     4074 b- defN 23-Apr-30 20:28 search_string_overvaagning-0.3.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10450 b- defN 23-Apr-30 20:28 search_string_overvaagning-0.3.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-30 20:28 search_string_overvaagning-0.3.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-30 20:28 search_string_overvaagning-0.3.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      987 b- defN 23-Apr-30 20:28 search_string_overvaagning-0.3.8.dist-info/RECORD
+11 files, 50434 bytes uncompressed, 14761 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: search_string/search_string_collection.py
 Comment: 
 
 Filename: search_string/version.py
 Comment: 
 
-Filename: search_string_overvaagning-0.3.7.dist-info/LICENSE
+Filename: search_string_overvaagning-0.3.8.dist-info/LICENSE
 Comment: 
 
-Filename: search_string_overvaagning-0.3.7.dist-info/METADATA
+Filename: search_string_overvaagning-0.3.8.dist-info/METADATA
 Comment: 
 
-Filename: search_string_overvaagning-0.3.7.dist-info/WHEEL
+Filename: search_string_overvaagning-0.3.8.dist-info/WHEEL
 Comment: 
 
-Filename: search_string_overvaagning-0.3.7.dist-info/top_level.txt
+Filename: search_string_overvaagning-0.3.8.dist-info/top_level.txt
 Comment: 
 
-Filename: search_string_overvaagning-0.3.7.dist-info/RECORD
+Filename: search_string_overvaagning-0.3.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## search_string/version.py

```diff
@@ -1,3 +1,3 @@
 from __future__ import annotations
 
-__version__ = '0.3.7'
+__version__ = '0.3.8'
```

## Comparing `search_string_overvaagning-0.3.7.dist-info/LICENSE` & `search_string_overvaagning-0.3.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `search_string_overvaagning-0.3.7.dist-info/METADATA` & `search_string_overvaagning-0.3.8.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: search-string-overvaagning
-Version: 0.3.7
+Version: 0.3.8
 Summary: SearchString is a custom implementation for searching strings for overvaagning.app.
 Home-page: https://github.com/kaas-mulvad/search-string
 Author: Søren Mulvad
 Author-email: Soeren Mulvad <post@kaasogmulvad.dk>
 License: End-User License Agreement (EULA) of SearchString
         
         This End-User License Agreement ("EULA") is a legal agreement between you and Kaas & Mulvad. Our EULA was created by EULA Template for SearchString.
@@ -75,19 +75,19 @@
 
 You can install `search-string` from [PyPI][pypi]:
 
 ```bash
 $ pip install search-string-overvaagning
 ```
 
-The package is supported on Python 3.10+.
+The package is supported on Python 3.8+. However, the package is only compiled using `mypyc` starting from Python 3.10 which makes it about twice as fast. As such, it is strongly advised to run it on Python 3.10+.
 
 ## About
 
-This package implements the search string object that is used across [overvaagning.app](https://overvaagning.app/) for different types of surveillance.
+This package implements the search string object that is used across [km24.dk](https://km24.dk/) for different types of surveillance.
 
 It is used for searching a text. For something to be deemed a match, the text must match the `first_str` and if the `second_str` is not empty, the text must also match the `second_str`. If the `not_str` is not empty, the text must *not* match the `not_str`. A logical AND is used between the three conditions. The three strings can each be a collection of strings separated by semicolons wherein a match is deemed by logical OR. You can use '~' to make a word boundary. Finally, you can use `!global` at the end of a string to signal that that part should check globally.
 
 Quick examples:
 
 ```python
 >>> ss = SearchString('example;hello', 'text', 'elephant', data=None)
```

## Comparing `search_string_overvaagning-0.3.7.dist-info/RECORD` & `search_string_overvaagning-0.3.8.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 search_string/__init__.py,sha256=L1sA0kHPqU2plluuMF75eGANNBM6JKbMm_V3Bkuujbw,239
 search_string/constants.py,sha256=sZ740e8ExWt4a3Ks7qvGqJKGy66m9IOZ_nLz3tDJaGw,385
 search_string/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 search_string/search_string.py,sha256=cOLEC73xAa3M6ntFva4qrIydgQ5Re-d6tKshG004fuY,21840
 search_string/search_string_collection.py,sha256=jDdQ2YlCcHc2ymNHaMcU76BwHWQGTkzVy4D_aGxgs-g,12295
-search_string/version.py,sha256=7-zCaSnzACwjBXDt0IGL8tZZj3V6LxMuza7JeZ2uEG8,58
-search_string_overvaagning-0.3.7.dist-info/LICENSE,sha256=xYX49IgOmQdnmBwaNYTW43N4YAiyfzwNr367kxWn2-s,4074
-search_string_overvaagning-0.3.7.dist-info/METADATA,sha256=DvSKnDwyICYzMRGiSTct8WTfBRUHTLWGLIeLKvCh0eo,10296
-search_string_overvaagning-0.3.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-search_string_overvaagning-0.3.7.dist-info/top_level.txt,sha256=66CcfMgUUyQ2MQT4Se3Eit8Zr5agt6PT-YqoodkXGgA,14
-search_string_overvaagning-0.3.7.dist-info/RECORD,,
+search_string/version.py,sha256=rHEQNhQDgCeoNzn4SjapIiGFB1oKCaxcIWX1inBzq4Y,58
+search_string_overvaagning-0.3.8.dist-info/LICENSE,sha256=xYX49IgOmQdnmBwaNYTW43N4YAiyfzwNr367kxWn2-s,4074
+search_string_overvaagning-0.3.8.dist-info/METADATA,sha256=izvOyfc5jP4go_bsNaSODu7SKS9uOlWI0HO5bbX9I7c,10450
+search_string_overvaagning-0.3.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+search_string_overvaagning-0.3.8.dist-info/top_level.txt,sha256=66CcfMgUUyQ2MQT4Se3Eit8Zr5agt6PT-YqoodkXGgA,14
+search_string_overvaagning-0.3.8.dist-info/RECORD,,
```

