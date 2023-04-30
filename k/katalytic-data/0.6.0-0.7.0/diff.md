# Comparing `tmp/katalytic-data-0.6.0.tar.gz` & `tmp/katalytic-data-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-data-0.6.0.tar", last modified: Sat Apr 29 20:11:18 2023, max compression
+gzip compressed data, was "katalytic-data-0.7.0.tar", last modified: Sun Apr 30 04:53:53 2023, max compression
```

## Comparing `katalytic-data-0.6.0.tar` & `katalytic-data-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.6.0/.coveragerc
--rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.6.0/.gitignore
--rw-r--r--   0        0        0     3109 2023-04-27 17:15:54.916636 katalytic-data-0.6.0/.gitlab-ci.yml
--rw-r--r--   0        0        0    12185 2023-04-29 20:11:15.675044 katalytic-data-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     2083 2023-04-16 12:25:23.268033 katalytic-data-0.6.0/README.md
--rw-r--r--   0        0        0     1245 2023-04-29 20:11:15.675044 katalytic-data-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    20832 2023-04-29 20:04:37.808201 katalytic-data-0.6.0/src/katalytic/data.py
--rw-r--r--   0        0        0    40893 2023-04-29 20:05:14.136232 katalytic-data-0.6.0/tests/test_data.py
--rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 katalytic-data-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.7.0/.coveragerc
+-rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.7.0/.gitignore
+-rw-r--r--   0        0        0     3109 2023-04-27 17:15:54.916636 katalytic-data-0.7.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0    12386 2023-04-30 04:53:50.237236 katalytic-data-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     2083 2023-04-16 12:25:23.268033 katalytic-data-0.7.0/README.md
+-rw-r--r--   0        0        0     1245 2023-04-30 04:53:50.237236 katalytic-data-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    20968 2023-04-30 04:48:19.340092 katalytic-data-0.7.0/src/katalytic/data.py
+-rw-r--r--   0        0        0    41125 2023-04-30 04:47:50.159666 katalytic-data-0.7.0/tests/test_data.py
+-rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 katalytic-data-0.7.0/PKG-INFO
```

### Comparing `katalytic-data-0.6.0/.gitignore` & `katalytic-data-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.6.0/.gitlab-ci.yml` & `katalytic-data-0.7.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.6.0/CHANGELOG.md` & `katalytic-data-0.7.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.7.0 (2023-04-30)
+### feat
+- [[`46caaef`](https://gitlab.com/katalytic/katalytic-data/commit/46caaeff90e1c3bff58e0db81bc082632c0f52a3)] allow passing a str to all_types() and all_types_besides()
+
+
 ## 0.6.0 (2023-04-29)
 ### feat
 - [[`52b8faf`](https://gitlab.com/katalytic/katalytic-data/commit/52b8faf9d53af06a791c4fab8c7b8a70001c1490)] **all_types_besides:** add "numbers" category
 - [[`c7c80ad`](https://gitlab.com/katalytic/katalytic-data/commit/c7c80ade75dfa858022855df849c6be6ccb3c4fc)] add all_types
 
 
 ## 0.5.1 (2023-04-29)
```

### Comparing `katalytic-data-0.6.0/LICENSE.txt` & `katalytic-data-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.6.0/README.md` & `katalytic-data-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.6.0/pyproject.toml` & `katalytic-data-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-data"
-version = "0.6.0"
+version = "0.7.0"
 description = "This plugin adds utilities for working with data to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-data-0.6.0/src/katalytic/data.py` & `katalytic-data-0.7.0/src/katalytic/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,25 +80,29 @@
     'tuple': (),
 }
 
 
 def all_types(whitelist=None):
     if whitelist is None:
         return flatten(_types.values())
+    elif isinstance(whitelist, str):
+        whitelist = [whitelist]
     elif not is_iterable(whitelist):
         raise TypeError(f'<whitelist> must be iterable. Got {type(whitelist).__name__}')
 
     unexpected = set(whitelist) - set(_types.keys())
     if unexpected:
         raise ValueError(f'Unexpected types in <whitelist>: {unexpected}')
 
     return flatten(_types[t] for t in whitelist)
 
 
 def all_types_besides(blacklist):
+    if isinstance(blacklist, str):
+        blacklist = [blacklist]
     if not is_iterable(blacklist):
         raise TypeError(f'<blacklist> must be iterable. Got {type(blacklist).__name__}')
 
     blacklist = set(blacklist)
     unexpected = blacklist - set(_types.keys())
     if unexpected:
         raise ValueError(f'Unexpected types in <blacklist>: {unexpected}')
```

### Comparing `katalytic-data-0.6.0/tests/test_data.py` & `katalytic-data-0.7.0/tests/test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from fractions import Fraction
 from pathlib import Path, PosixPath
 
 import pytest
 
 from katalytic.checks import is_iterator, dicts_share_key_order, dicts_share_value_order, is_equal
 from katalytic.data import (
-    _C, _C_obj, _function, _iterables, _lambda, _obj, _objects, _types, all_types, all_types_besides, as_list_of_dicts, as_list_of_lists, first, first_with_idx, flatten, flatten_recursive, last, last_with_idx, map_dict_keys, map_dict_values,
+    _C, _C_obj, _function, _iterables, _lambda, _numbers, _obj, _objects, _types, all_types, all_types_besides, as_list_of_dicts, as_list_of_lists, first, first_with_idx, flatten, flatten_recursive, last, last_with_idx, map_dict_keys, map_dict_values,
     map_recursive, one, pick_all, pick_all_besides, pick_any, sort_dict_by_keys, sort_dict_by_keys_recursive, sort_dict_by_values, sort_dict_by_values_recursive,
     as_dict_of_lists, sort_recursive, xor, xor_with_idx, detect_fronts, detect_fronts_positive, detect_fronts_negative
 )
 
 
 def _is_list(x):
     return isinstance(x, list)
@@ -29,15 +29,15 @@
 
 
 def _is_str(x):
     return isinstance(x, str)
 
 
 class Test_all_types:
-    @pytest.mark.parametrize('wrong_type', ['', 1, 1.0, True, False, object()])
+    @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, object()])
     def test_wrong_type(self, wrong_type):
         with pytest.raises(TypeError):
             all_types(wrong_type)
 
     @pytest.mark.parametrize('unexpected', [
         ['iterable', 'func', 'strong']
     ])
@@ -45,21 +45,22 @@
         with pytest.raises(ValueError):
             all_types(unexpected)
 
     @pytest.mark.parametrize('whitelist, expected', [
         (None, flatten(_types.values())),
         (['iterables'], _iterables),
         (['iterables', 'objects', 'path'], [*_iterables, *_objects, Path('')]),
+        ('numbers', _numbers),
     ])
     def test_all_types(self, whitelist, expected):
         assert all_types(whitelist) == expected
 
 
 class Test_all_types_besides:
-    @pytest.mark.parametrize('wrong_type', ['', 1, 1.0, True, False, None, object()])
+    @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, None, object()])
     def test_wrong_type(self, wrong_type):
         with pytest.raises(TypeError):
             all_types_besides(wrong_type)
 
     @pytest.mark.parametrize('unexpected', [
         ['iterable', 'func', 'strong']
     ])
@@ -69,14 +70,18 @@
 
     @pytest.mark.parametrize('blacklist, expected', [
         (
             ['iterables'],
             [False, bytearray(b''), b'', _function, _lambda, _C_obj, _C, 0j, Decimal('0'), 0.0, Fraction(0, 1), 0, None, _obj, PosixPath('.'), True, '']
         ),
         (
+            'iterables',
+            [False, bytearray(b''), b'', _function, _lambda, _C_obj, _C, 0j, Decimal('0'), 0.0, Fraction(0, 1), 0, None, _obj, PosixPath('.'), True, '']
+        ),
+        (
             ['iterables', 'generators', 'functions', 'objects', 'path'],
             [False, bytearray(b''), b'', _C, 0j, Decimal('0'), 0.0, Fraction(0, 1), 0, None, True, '']
         ),
     ])
     def test_all_types_besides(self, blacklist, expected):
         assert all_types_besides(blacklist) == expected
```

### Comparing `katalytic-data-0.6.0/PKG-INFO` & `katalytic-data-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-data
-Version: 0.6.0
+Version: 0.7.0
 Summary: This plugin adds utilities for working with data to the katalytic namespace
 Keywords: high-level,data conversion
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

