# Comparing `tmp/katalytic-data-0.7.0.tar.gz` & `tmp/katalytic-data-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-data-0.7.0.tar", last modified: Sun Apr 30 04:53:53 2023, max compression
+gzip compressed data, was "katalytic-data-0.7.1.tar", last modified: Sun Apr 30 05:44:06 2023, max compression
```

## Comparing `katalytic-data-0.7.0.tar` & `katalytic-data-0.7.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.7.0/.coveragerc
--rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.7.0/.gitignore
--rw-r--r--   0        0        0     3109 2023-04-27 17:15:54.916636 katalytic-data-0.7.0/.gitlab-ci.yml
--rw-r--r--   0        0        0    12386 2023-04-30 04:53:50.237236 katalytic-data-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     2083 2023-04-16 12:25:23.268033 katalytic-data-0.7.0/README.md
--rw-r--r--   0        0        0     1245 2023-04-30 04:53:50.237236 katalytic-data-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    20968 2023-04-30 04:48:19.340092 katalytic-data-0.7.0/src/katalytic/data.py
--rw-r--r--   0        0        0    41125 2023-04-30 04:47:50.159666 katalytic-data-0.7.0/tests/test_data.py
--rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 katalytic-data-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.7.1/.coveragerc
+-rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.7.1/.gitignore
+-rw-r--r--   0        0        0     3109 2023-04-27 17:15:54.916636 katalytic-data-0.7.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0    12580 2023-04-30 05:44:02.196844 katalytic-data-0.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0     2083 2023-04-16 12:25:23.268033 katalytic-data-0.7.1/README.md
+-rw-r--r--   0        0        0     1245 2023-04-30 05:44:02.192844 katalytic-data-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    21404 2023-04-30 05:34:31.790368 katalytic-data-0.7.1/src/katalytic/data.py
+-rw-r--r--   0        0        0    41638 2023-04-30 05:38:20.462596 katalytic-data-0.7.1/tests/test_data.py
+-rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 katalytic-data-0.7.1/PKG-INFO
```

### Comparing `katalytic-data-0.7.0/.gitignore` & `katalytic-data-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.7.0/.gitlab-ci.yml` & `katalytic-data-0.7.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.7.0/CHANGELOG.md` & `katalytic-data-0.7.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.7.1 (2023-04-30)
+### fix
+- [[`5a06ff8`](https://gitlab.com/katalytic/katalytic-data/commit/5a06ff8ee54e58e502c18fee5723bad8c4bf702a)] add missing categories of types and extend the tests
+
+
 ## 0.7.0 (2023-04-30)
 ### feat
 - [[`46caaef`](https://gitlab.com/katalytic/katalytic-data/commit/46caaeff90e1c3bff58e0db81bc082632c0f52a3)] allow passing a str to all_types() and all_types_besides()
 
 
 ## 0.6.0 (2023-04-29)
 ### feat
```

### Comparing `katalytic-data-0.7.0/LICENSE.txt` & `katalytic-data-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.7.0/README.md` & `katalytic-data-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.7.0/pyproject.toml` & `katalytic-data-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-data"
-version = "0.7.0"
+version = "0.7.1"
 description = "This plugin adds utilities for working with data to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-data-0.7.0/src/katalytic/data.py` & `katalytic-data-0.7.1/src/katalytic/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from decimal import Decimal
 from fractions import Fraction
 from pathlib import Path
 
 from katalytic.checks import (
-    is_any_of, is_iterable, is_iterator, is_none_of, is_primitive, is_dict_of_sequences_uniform, is_sequence_of_sequences_uniform,
+    is_any_of, is_generator, is_iterable, is_iterator, is_none_of, is_primitive, is_dict_of_sequences_uniform, is_sequence_of_sequences_uniform,
     is_sequence_of_dicts_uniform
 )
 
 from katalytic.pkg import get_version
 
 __version__, __version_info__ = get_version(__name__)
 
@@ -39,14 +39,15 @@
 _singletons = [None, True, False]
 _primitives = [*_singletons, 0, 0.0, '', b'', bytearray(b'')]
 _callables = [_generator, _function, _lambda, _C_obj, _C]
 _numbers = [0, 0.0, 0j, Decimal('0'), Fraction(0, 1)]
 _objects = [_obj, _C_obj]
 _generators = [_generator, _generator_expr]
 _functions = [_generator, _function, _lambda]
+_strings = ['', b'', bytearray(b'')]
 
 _types = {
     'bool': False,
     'bytearray': bytearray(b''),
     'bytes': b'',
     'callables': _callables,
     'callable object': _C_obj,
@@ -73,14 +74,15 @@
     'objects': _objects,
     'path': Path(''),
     'primitives': _primitives,
     'sequences': _sequences,
     'set': set(),
     'singletons': _singletons,
     'str': '',
+    'strings': _strings,
     'tuple': (),
 }
 
 
 def all_types(whitelist=None):
     if whitelist is None:
         return flatten(_types.values())
@@ -89,30 +91,30 @@
     elif not is_iterable(whitelist):
         raise TypeError(f'<whitelist> must be iterable. Got {type(whitelist).__name__}')
 
     unexpected = set(whitelist) - set(_types.keys())
     if unexpected:
         raise ValueError(f'Unexpected types in <whitelist>: {unexpected}')
 
-    return flatten(_types[t] for t in whitelist)
+    return _flatten(_types[t] for t in whitelist)
 
 
 def all_types_besides(blacklist):
     if isinstance(blacklist, str):
         blacklist = [blacklist]
     if not is_iterable(blacklist):
         raise TypeError(f'<blacklist> must be iterable. Got {type(blacklist).__name__}')
 
     blacklist = set(blacklist)
     unexpected = blacklist - set(_types.keys())
     if unexpected:
         raise ValueError(f'Unexpected types in <blacklist>: {unexpected}')
 
-    to_remove = flatten(_types[t] for t in blacklist)
-    all_types = flatten(_types.values())
+    to_remove = _flatten(_types[t] for t in blacklist)
+    all_types = _flatten(_types.values())
     kept = []
     for t in all_types:
         if t in to_remove:
             continue
 
         # remove duplicates too
         # I have to do it this way because python considers
@@ -121,14 +123,30 @@
             continue
 
         kept.append(t)
 
     return kept
 
 
+def _flatten(iterable):
+    if not is_iterable(iterable):
+        raise TypeError(f'<iterable> expects an iterable. Got {type(iterable).__name__}')
+
+    flat = []
+    for x in iterable:
+        if is_generator(x):
+            flat.append(x)
+        elif is_iterable(x):
+            flat.extend(x)
+        else:
+            flat.append(x)
+
+    return flat
+
+
 def as_dict_of_lists(data):
     """This format is useful when you need to perform operations on each column
     of a table.
 
     It's as compact as the sequence_of_sequences format, but less intuitive"""
     if is_sequence_of_dicts_uniform(data):
         return {k: [d[k] for d in data] for k in data[0]}
```

### Comparing `katalytic-data-0.7.0/tests/test_data.py` & `katalytic-data-0.7.1/tests/test_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from fractions import Fraction
 from pathlib import Path, PosixPath
 
 import pytest
 
 from katalytic.checks import is_iterator, dicts_share_key_order, dicts_share_value_order, is_equal
 from katalytic.data import (
-    _C, _C_obj, _function, _iterables, _lambda, _numbers, _obj, _objects, _types, all_types, all_types_besides, as_list_of_dicts, as_list_of_lists, first, first_with_idx, flatten, flatten_recursive, last, last_with_idx, map_dict_keys, map_dict_values,
+    _C, _C_obj, _callables, _collections, _dict_views, _function, _functions, _generators, _iterables, _iterators, _lambda, _numbers, _obj, _objects, _primitives, _sequences, _singletons, _strings, _types, all_types, all_types_besides, as_list_of_dicts, as_list_of_lists, first, first_with_idx, flatten, flatten_recursive, last, last_with_idx, map_dict_keys, map_dict_values,
     map_recursive, one, pick_all, pick_all_besides, pick_any, sort_dict_by_keys, sort_dict_by_keys_recursive, sort_dict_by_values, sort_dict_by_values_recursive,
     as_dict_of_lists, sort_recursive, xor, xor_with_idx, detect_fronts, detect_fronts_positive, detect_fronts_negative
 )
 
 
 def _is_list(x):
     return isinstance(x, list)
@@ -42,18 +42,29 @@
         ['iterable', 'func', 'strong']
     ])
     def test_unexpected(self, unexpected):
         with pytest.raises(ValueError):
             all_types(unexpected)
 
     @pytest.mark.parametrize('whitelist, expected', [
+        ('callables', _callables),
+        ('collections', _collections),
+        ('dict_views', _dict_views),
+        ('functions', _functions),
+        ('generators', _generators),
+        ('iterators', _iterators),
+        ('numbers', _numbers),
+        ('objects', _objects),
+        ('primitives', _primitives),
+        ('sequences', _sequences),
+        ('singletons', _singletons),
+        ('strings', _strings),
         (None, flatten(_types.values())),
-        (['iterables'], _iterables),
         (['iterables', 'objects', 'path'], [*_iterables, *_objects, Path('')]),
-        ('numbers', _numbers),
+        (['iterables'], _iterables),
     ])
     def test_all_types(self, whitelist, expected):
         assert all_types(whitelist) == expected
 
 
 class Test_all_types_besides:
     @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, None, object()])
```

### Comparing `katalytic-data-0.7.0/PKG-INFO` & `katalytic-data-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-data
-Version: 0.7.0
+Version: 0.7.1
 Summary: This plugin adds utilities for working with data to the katalytic namespace
 Keywords: high-level,data conversion
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

