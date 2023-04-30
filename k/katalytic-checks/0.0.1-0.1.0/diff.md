# Comparing `tmp/katalytic-checks-0.0.1.tar.gz` & `tmp/katalytic-checks-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-checks-0.0.1.tar", last modified: Thu Apr 27 05:26:09 2023, max compression
+gzip compressed data, was "katalytic-checks-0.1.0.tar", last modified: Sun Apr 30 05:55:13 2023, max compression
```

## Comparing `katalytic-checks-0.0.1.tar` & `katalytic-checks-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-checks-0.0.1/.coveragerc
--rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-checks-0.0.1/.gitignore
--rw-r--r--   0        0        0     3109 2023-04-16 15:20:55.636719 katalytic-checks-0.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0     6569 2023-04-27 05:23:14.397929 katalytic-checks-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-checks-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1990 2023-04-27 05:10:58.838831 katalytic-checks-0.0.1/README.md
--rw-r--r--   0        0        0     1525 2023-04-27 05:23:14.397929 katalytic-checks-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5722 2023-04-25 05:47:11.165924 katalytic-checks-0.0.1/src/katalytic/checks.py
--rw-r--r--   0        0        0    16327 2023-04-24 05:49:34.858602 katalytic-checks-0.0.1/tests/test_checks.py
--rw-r--r--   0        0        0     3041 1970-01-01 00:00:00.000000 katalytic-checks-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-checks-0.1.0/.coveragerc
+-rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-checks-0.1.0/.gitignore
+-rw-r--r--   0        0        0     3062 2023-04-30 05:48:57.335564 katalytic-checks-0.1.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      598 2023-04-30 05:54:56.055866 katalytic-checks-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-checks-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1990 2023-04-27 05:10:58.838831 katalytic-checks-0.1.0/README.md
+-rw-r--r--   0        0        0     1257 2023-04-30 05:54:56.055866 katalytic-checks-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6052 2023-04-30 05:32:34.812039 katalytic-checks-0.1.0/src/katalytic/checks.py
+-rw-r--r--   0        0        0    16322 2023-04-30 05:18:35.946848 katalytic-checks-0.1.0/tests/test_checks.py
+-rw-r--r--   0        0        0     3095 1970-01-01 00:00:00.000000 katalytic-checks-0.1.0/PKG-INFO
```

### Comparing `katalytic-checks-0.0.1/.gitignore` & `katalytic-checks-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-checks-0.0.1/.gitlab-ci.yml` & `katalytic-checks-0.1.0/.gitlab-ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,15 @@
   PIP_NO_CACHE_DIR: "off"
 
 test_cov:
   image: python:3.6
   stage: coverage
   script:
     - pip install --upgrade pip
-    - pip install pytest pytest-cov pytest-randomly
-    - pip install -e .
+    - pip install -e .[dev]
     - python -m pytest --cov-fail-under=100 --cov=src --cov-report term-missing || { echo "Tests failed. Exiting ..." && exit 1; }
   rules:
     - if: '$CI_COMMIT_MESSAGE =~ /(feat|fix|refactor|perf|test|chore|style)/i'
       when: always
     - when: never
   allow_failure: false
```

### Comparing `katalytic-checks-0.0.1/LICENSE.txt` & `katalytic-checks-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-checks-0.0.1/README.md` & `katalytic-checks-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-checks-0.0.1/src/katalytic/checks.py` & `katalytic-checks-0.1.0/src/katalytic/checks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import collections
 import inspect
+from decimal import Decimal
+from fractions import Fraction
 
 
 def contains_all_of(haystack, needles):
     if not is_iterable(haystack):
         raise TypeError(f'<haystack> expects an iterable. Got {type(haystack).__name__}: {haystack!r}')
     elif not is_iterable(needles):
         raise TypeError(f'<needles> expects an iterable. Got {type(needles).__name__}: {needles!r}')
@@ -113,43 +115,53 @@
     if is_singleton(a) or is_singleton(b):
         return a is b
     else:
         return a == b
 
 
 def is_generator(x):
-    return inspect.isgenerator(x)
+    return inspect.isgenerator(x) or inspect.isgeneratorfunction(x)
 
 
 def is_iterable(x):
+    if is_generator(x):
+        return True
+
     try:
         # The only reliable way to determine whether an object is iterable is to call iter(obj).
         iter(x)
         # str, bytes, bytearray are theoretically a iterables,
         # but in practice we use them as primitives
         return not isinstance(x, (str, bytes, bytearray))
     except TypeError:
         return False
 
 
 def is_iterable_or_str(x):
-    return isinstance(x, collections.abc.Iterable)
+    return is_generator(x) or isinstance(x, collections.abc.Iterable)
 
 
 def is_iterator(x):
-    return isinstance(x, collections.abc.Iterator)
+    return is_generator(x) or isinstance(x, collections.abc.Iterator)
 
 
 def is_none_of(needle, haystack):
     return not is_any_of(needle, haystack)
 
 
+def is_number(x):
+    if isinstance(x, bool):
+        return None
+
+    return isinstance(x, (int, float, complex, Decimal, Fraction))
+
+
 def is_primitive(x):
     """str is theoretically a collection, but in practice we use it as a primitive"""
-    return isinstance(x, (str, int, float, bool, type(None)))
+    return isinstance(x, (str, int, float, bool, type(None), bytes, bytearray))
 
 
 def is_sequence(x):
     """str is theoretically an sequence, but in practice we use it as a primitive"""
     return isinstance(x, collections.abc.Sequence) and not isinstance(x, (str, bytes, bytearray))
```

### Comparing `katalytic-checks-0.0.1/tests/test_checks.py` & `katalytic-checks-0.1.0/tests/test_checks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import pytest
+
 from katalytic.checks import (
-    contains_all_of, contains_any_of, contains_none_of, is_any_of, is_dict_of_sequences, is_generator, is_iterable, is_iterable_or_str, is_iterator, is_none_of, is_primitive,
+    contains_all_of, contains_any_of, contains_none_of, is_any_of, is_dict_of_sequences, is_generator, is_iterable, is_iterable_or_str, is_iterator, is_none_of, is_number, is_primitive,
     is_sequence, is_sequence_of_dicts, is_sequence_of_sequences, is_sequence_or_str, is_sequence_of_dicts_uniform,
     is_dict_of_sequences_uniform, is_sequence_of_sequences_uniform, dicts_share_key_order, dicts_share_value_order, is_singleton, is_equal
 )
 
-import pytest
+from katalytic.data import all_types, all_types_besides
 
 
 def _generator():
     yield 1
 
 
 class Test_contains_all_of:
@@ -239,23 +241,30 @@
 
     @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, None, object(), {}, iter([]), map(lambda x: x, []), [()], ([], ), {'a': {}}])
     def test_False(self, wrong_type):
         assert not is_dict_of_sequences(wrong_type)
 
 
 class Test_is_dict_of_sequences_uniform:
-    def test_True(self):
-        assert is_dict_of_sequences_uniform({'a': (), 'b': ()})
-        assert is_dict_of_sequences_uniform({'a': [1], 'b': [1]})
-        assert is_dict_of_sequences_uniform({'a': (1, 2, 3), 'b': [10, 20, 30]})
-
-    def test_False(self):
-        assert not is_dict_of_sequences_uniform({'a': [1], 'b': [1, 2]})
-        assert not is_dict_of_sequences_uniform({'a': [1], 'b': []})
-        assert not is_dict_of_sequences_uniform({'a': [1], 'b': [1], 'c': [1, 2]})
+    @pytest.mark.parametrize('data', [
+        {'a': (), 'b': ()},
+        {'a': [1], 'b': [1]},
+        {'a': (1, 2, 3), 'b': [10, 20, 30]},
+    ])
+    def test_True(self, data):
+        assert is_dict_of_sequences_uniform(data)
+
+    @pytest.mark.parametrize('data', [
+        {'a': [1], 'b': []},
+        {'a': [1], 'b': [1, 2]},
+        {'a': [1], 'b': [1], 'c': [1, 2]},
+        []
+    ])
+    def test_False(self, data):
+        assert not is_dict_of_sequences_uniform(data)
 
 
 class Test_is_equal:
     @pytest.mark.parametrize('a, b', [
         (0, False),
         (0, None),
         (False, None),
@@ -274,49 +283,49 @@
         (None, None),
     ])
     def test_True(self, a, b):
         assert is_equal(a, b)
 
 
 class Test_is_generator:
-    @pytest.mark.parametrize('correct_type', [_generator()])
+    @pytest.mark.parametrize('correct_type', all_types('generators'))
     def test_True(self, correct_type):
         assert is_generator(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', [iter([]), map(bool, []), 1, 1.0, True, False, None, 'string', object(), range(1)])
+    @pytest.mark.parametrize('wrong_type', all_types_besides('generators'))
     def test_False(self, wrong_type):
         assert not is_generator(wrong_type)
 
 
 class Test_is_iterable:
-    @pytest.mark.parametrize('correct_type', [[], set(), (), {}, {}.keys(), {}.values(), {}.items(), range(1), iter([]), map(lambda x: x, [])])
+    @pytest.mark.parametrize('correct_type', all_types('iterables'))
     def test_True(self, correct_type):
         assert is_iterable(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, None, '', bytes('', 'utf-8'), bytearray('', 'utf-8'), object()])
+    @pytest.mark.parametrize('wrong_type', all_types_besides('iterables'))
     def test_False(self, wrong_type):
         assert not is_iterable(wrong_type)
 
 
 class Test_is_iterable_or_str:
-    @pytest.mark.parametrize('correct_type', ['', bytes('', 'utf-8'), bytearray('', 'utf-8'), [], set(), (), {}, range(1), iter([]), map(lambda x: x, [])])
+    @pytest.mark.parametrize('correct_type', all_types(['iterables', 'strings']))
     def test_True(self, correct_type):
         assert is_iterable_or_str(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, None, object()])
+    @pytest.mark.parametrize('wrong_type', all_types_besides(['iterables', 'strings']))
     def test_False(self, wrong_type):
         assert not is_iterable_or_str(wrong_type)
 
 
 class Test_is_iterator:
-    @pytest.mark.parametrize('correct_type', [iter([]), map(bool, []), _generator()])
+    @pytest.mark.parametrize('correct_type', all_types('iterators'))
     def test_True(self, correct_type):
         assert is_iterator(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, None, 'string', object(), range(1)])
+    @pytest.mark.parametrize('wrong_type', all_types_besides('iterators'))
     def test_False(self, wrong_type):
         assert not is_iterator(wrong_type)
 
 
 class Test_is_none_of:
     @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
     def test_not_iterable(self, wrong_type):
@@ -349,29 +358,29 @@
         (False, [0, 1]),
     ])
     def test_bools_are_not_ints(self, x, iterable):
         assert is_none_of(x, iterable)
 
 
 class Test_is_primitive:
-    @pytest.mark.parametrize('correct_type', [1, 1.0, True, False, 'string', None])
+    @pytest.mark.parametrize('correct_type', all_types('primitives'))
     def test_True(self, correct_type):
         assert is_primitive(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, object()])
+    @pytest.mark.parametrize('wrong_type', all_types_besides('primitives'))
     def test_False(self, wrong_type):
         assert not is_primitive(wrong_type)
 
 
 class Test_is_sequence:
-    @pytest.mark.parametrize('correct_type', [[], (), range(1)])
+    @pytest.mark.parametrize('correct_type', all_types('sequences'))
     def test_True(self, correct_type):
         assert is_sequence(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, None, '', bytes('', 'utf-8'), bytearray('', 'utf-8'), object(), {}, iter([]), map(lambda x: x, [])])
+    @pytest.mark.parametrize('wrong_type', all_types_besides('sequences'))
     def test_False(self, wrong_type):
         assert not is_sequence(wrong_type)
 
 
 class Test_is_sequence_of_dicts:
     @pytest.mark.parametrize('correct_type', [[{}], ({}, )])
     def test_True(self, correct_type):
@@ -379,60 +388,84 @@
 
     @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, None, object(), {}, iter([]), map(lambda x: x, []), [()], ([], ), {'a': []}])
     def test_False(self, wrong_type):
         assert not is_sequence_of_dicts(wrong_type)
 
 
 class Test_is_sequence_of_dicts_uniform:
-    def test_True(self):
-        assert is_sequence_of_dicts_uniform([{}, {}])
-        assert is_sequence_of_dicts_uniform([{'a': 1}, {'a': 2}])
-        assert is_sequence_of_dicts_uniform([{'b': 1, 'a': 1}, {'a': 2, 'b': 2}])
-
-    def test_False(self):
-        assert not is_sequence_of_dicts_uniform([{'a': 1}, {'b': 2}])
-        assert not is_sequence_of_dicts_uniform([{'a': 1, 'b': 1}, {'b': 2}])
+    @pytest.mark.parametrize('data', [
+        [{}, {}],
+        [{'a': 1}, {'a': 2}],
+        [{'b': 1, 'a': 1}, {'a': 2, 'b': 2}],
+    ])
+    def test_True(self, data):
+        assert is_sequence_of_dicts_uniform(data)
+
+    @pytest.mark.parametrize('data', [
+        [{'a': 1}, {'b': 2}],
+        [{'a': 1, 'b': 1}, {'b': 2}],
+        {},
+    ])
+    def test_False(self, data):
+        assert not is_sequence_of_dicts_uniform(data)
 
 
 class Test_is_sequence_of_sequences:
     @pytest.mark.parametrize('correct_type', [[[]], [()], ([], ), ((), )])
     def test_True(self, correct_type):
         assert is_sequence_of_sequences(correct_type)
 
     @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, None, object(), {}, iter([]), map(lambda x: x, []), [{}], {'a': []}])
     def test_False(self, wrong_type):
         assert not is_sequence_of_sequences(wrong_type)
 
 
 class Test_is_sequence_of_sequences_uniform:
-    def test_True(self):
-        assert is_sequence_of_sequences_uniform([[], []])
-        assert is_sequence_of_sequences_uniform([
+    @pytest.mark.parametrize('data', [
+        [[], []],
+        [
             ['a', 'b', 'c'],
             ['x', 'y', 'z'],
             [1, 2, 3],
             [True, False, None]
-        ])
+        ],
+    ])
+    def test_True(self, data):
+        assert is_sequence_of_sequences_uniform(data)
 
-    def test_False(self):
-        assert not is_sequence_of_sequences_uniform([[], [1]])
-        assert not is_sequence_of_sequences_uniform([['a', 'b', 'c'], ['x', 'y']])
+    @pytest.mark.parametrize('data', [
+        [[], [1]],
+        [['a', 'b', 'c'], ['x', 'y']],
+        {},
+    ])
+    def test_False(self, data):
+        assert not is_sequence_of_sequences_uniform(data)
 
 
 class Test_is_sequence_or_str:
-    @pytest.mark.parametrize('correct_type', [[], (), range(1), '', bytes('', 'utf-8'), bytearray('', 'utf-8')])
+    @pytest.mark.parametrize('correct_type', all_types(['sequences', 'strings']))
     def test_True(self, correct_type):
         assert is_sequence_or_str(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, None, object(), {}, iter([]), map(lambda x: x, [])])
+    @pytest.mark.parametrize('wrong_type', all_types_besides(['sequences', 'strings']))
     def test_False(self, wrong_type):
         assert not is_sequence_or_str(wrong_type)
 
 
 class Test_is_singleton:
-    @pytest.mark.parametrize('correct_type', [True, False, None])
+    @pytest.mark.parametrize('correct_type', all_types('singletons'))
     def test_True(self, correct_type):
         assert is_singleton(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', ['string', 1, 1.0, [], set(), (), {}, object(), _generator, range(1)])
+    @pytest.mark.parametrize('wrong_type', all_types_besides('singletons'))
     def test_False(self, wrong_type):
         assert not is_singleton(wrong_type)
+
+
+class Test_is_number:
+    @pytest.mark.parametrize('correct_type', all_types('numbers'))
+    def test_True(self, correct_type):
+        assert is_number(correct_type)
+
+    @pytest.mark.parametrize('wrong_type', all_types_besides('numbers'))
+    def test_False(self, wrong_type):
+        assert not is_number(wrong_type)
```

### Comparing `katalytic-checks-0.0.1/PKG-INFO` & `katalytic-checks-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-checks
-Version: 0.0.1
+Version: 0.1.0
 Summary: This plugin adds utilities for working with data to the katalytic namespace
 Keywords: high-level,data conversion
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Dist: katalytic-pkg>=0.2.6
+Requires-Dist: katalytic-data>=0.7.1 ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest-randomly ; extra == "dev"
 Project-URL: homepage, https://gitlab.com/katalytic/katalytic-checks.git
 Project-URL: repository, https://gitlab.com/katalytic/katalytic-checks.git
 Provides-Extra: dev
```

