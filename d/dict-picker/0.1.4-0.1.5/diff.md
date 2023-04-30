# Comparing `tmp/dict_picker-0.1.4-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.whl.zip` & `tmp/dict_picker-0.1.5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1077616 bytes, number of entries: 6
--rw-r--r--  4.6 unx     5448 b- defN 23-Apr-16 11:14 dict_picker-0.1.4.dist-info/METADATA
--rw-r--r--  4.6 unx      128 b- defN 23-Apr-16 11:14 dict_picker-0.1.4.dist-info/WHEEL
--rw-r--r--  4.6 unx     1066 b- defN 23-Apr-16 11:14 dict_picker-0.1.4.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      127 b- defN 23-Apr-16 11:14 dict_picker/__init__.py
--rwxr-xr-x  4.6 unx  4022748 b- defN 23-Apr-16 11:14 dict_picker/dict_picker.pypy39-pp73-x86-linux-gnu.so
--rw-r--r--  4.6 unx      516 b- defN 23-Apr-16 11:14 dict_picker-0.1.4.dist-info/RECORD
-6 files, 4030033 bytes uncompressed, 1076684 bytes compressed:  73.3%
+Zip file size: 115112 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     5622 b- defN 23-Apr-30 18:48 dict_picker-0.1.5.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Apr-30 18:48 dict_picker-0.1.5.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1087 b- defN 23-Apr-30 18:48 dict_picker-0.1.5.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      127 b- defN 23-Apr-30 18:48 dict_picker/__init__.py
+-rwxr-xr-x  4.6 unx   247808 b- defN 23-Apr-30 18:48 dict_picker/dict_picker.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      504 b- defN 23-Apr-30 18:48 dict_picker-0.1.5.dist-info/RECORD
+6 files, 255244 bytes uncompressed, 114200 bytes compressed:  55.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: dict_picker-0.1.4.dist-info/METADATA
+Filename: dict_picker-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: dict_picker-0.1.4.dist-info/WHEEL
+Filename: dict_picker-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: dict_picker-0.1.4.dist-info/license_files/LICENSE
+Filename: dict_picker-0.1.5.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: dict_picker/__init__.py
 Comment: 
 
-Filename: dict_picker/dict_picker.pypy39-pp73-x86-linux-gnu.so
+Filename: dict_picker/dict_picker.cp39-win_amd64.pyd
 Comment: 
 
-Filename: dict_picker-0.1.4.dist-info/RECORD
+Filename: dict_picker-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `dict_picker-0.1.4.dist-info/METADATA` & `dict_picker-0.1.5.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,187 +1,187 @@
 Metadata-Version: 2.1
 Name: dict-picker
-Version: 0.1.4
+Version: 0.1.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Fast key search in python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Homepage, https://github.com/sarvensis/dict-picker
 
-# Dict picker (dictionary picker)
-
-Retrieve data from Python dictionaries and lists.
-
-## Installation
-
-With **pip**:
-
-```shell
-pip install -U dict-picker
-```
-
-Or with **conda**:
-
-```shell
-conda install "dict-picker" -c conda-forge
-```
-
-## Usage
-
-### `pick_by_path`
-
-The `pick_by_path` function is used to extract values from nested dictionaries using a path-like string to identify the desired value. The function takes three arguments: a dictionary object, a string representing the path to the desired value and optionally a delimiter.
-
-The path string consists of a sequence of keys, separated by the delimiter character (`'/'` by default), where each key represents a level in the nested dictionary. If the key has the value `'*'`, it matches any key on that level, or sets it to check all items in the list.
-
-The function returns the value at the end of the path or a list of values if the path contains a wildcard. If the path is not found, the function returns `None`.
-
-```python
-from dict_picker import pick_by_path
-
-example_dict = {
-    "foo": "bar",
-    "baz": {
-        "qux": "quux",
-        "quuux": "corge"
-    },
-    "fred": {
-        "wilma": "betty",
-        "barney": "pebbles"
-    },
-    "arr": [
-        { 'id': 123 },
-        { 'id': 456 },
-        { 'id': 789 },
-        { 'name': 'bubbles' },
-    ],
-}
-
-assert pick_by_path(example_dict, "foo") == "bar"
-assert pick_by_path(example_dict, "baz/qux") == "quux"
-assert pick_by_path(example_dict, "fred/wilma") == "betty"
-assert pick_by_path(example_dict, "*/qux") == "quux"
-assert pick_by_path(example_dict, "fred/*") == {"wilma": "betty", "barney": "pebbles"}
-assert pick_by_path(example_dict, "*/quux") is None
-assert pick_by_path(example_dict, "arr/*/id") == [123, 456, 789]
-
-# slice syntax
-assert pick_by_path(example_dict, "arr/0") == {'id': 123}
-assert pick_by_path(example_dict, "arr/1/id") == 456
-assert pick_by_path(example_dict, "arr/-1") == {'name': 'bubbles'}
-assert pick_by_path(example_dict, "arr/1:/id") == [456, 789, None]
-assert pick_by_path(example_dict, "arr/::-2/id") == [789, 123]
-```
-
-Parameters:
-
-- `obj` -- A dictionary object to search for the desired value.
-- `path: str` -- A string representing the path to the desired value.
-- `delimiter: str` -- A string used to separate keys in the path string. Default is "/".
-
-Return value:
-
-- Returns the value found at the end of the path string, or a list of values if the path contains a wildcard. If the path is not found, None is returned.
-
-
-### `pick_by_paths`
-
-The `pick_by_paths` function is similar to `pick_by_path`, but can extract values from multiple paths at once. It takes a dictionary object and a list of path strings as arguments, and returns a list of values found at the end of each path string or None if a path is not found. This works faster than running `pick_by_path` in a loop.
-
-```python
-from dict_picker import pick_by_path, pick_by_paths
-
-example_dict = {
-    "foo": "bar",
-    "baz": {
-        "qux": "quux",
-        "quuux": "corge"
-    },
-    "fred": {
-        "wilma": "betty",
-        "barney": "pebbles"
-    },
-    "arr": [
-        { 'id': 123 },
-        { 'id': 456 },
-        { 'id': 789 },
-        { 'name': 'bubbles' },
-    ],
-}
-
-assert pick_by_paths(example_dict, ["fred/*","*/quux", "arr/*/id",]) == [{"wilma": "betty", "barney": "pebbles"}, None, [123, 456, 789]]
-```
-
-## Build from sources
-
-### Cargo
-
-```shell
-curl --proto '=https' --tlsv1.2 -sSf <https://sh.rustup.rs> | sh
-```
-
-For other installation options, see [the official website](https://www.rust-lang.org/tools/install).
-
-### Maturin
-
-To bind python and rust, pyo3 is used. The [Maturin](https://github.com/PyO3/maturin) library is used to make it easy to work with.
-
-```shell
-python -m pip install maturin
-```
-
-### Build
-
-```shell
-python -m maturin build --release
-```
-
-Wheel will be released under the system and python in which it will be built. [Read more about the compilation](https://www.maturin.rs/distribution.html).
-
-The finished wheel can be found in the target/wheels folder.
-
-## Build with docker
-
-```shell
-docker run --rm -v $(pwd):/io ghcr.io/pyo3/maturin build --release  # or other maturin arguments
-```
-
-On macOS, it is better to use docker instead of podman.
-
-## Roadmap
-
-- [ ] Arbitrary levels skip operator `**`;
-- [X] Search inside an array of dictionaries. For example:
-
-    ```python
-    {
-        arr:  [
-            { id: 123 },
-            { id: 456 },
-            { id: 789 },
-        ]
-    }
-    'arr/*/id' -> [123, 456, 789]
-    ```
-
-- [X] Search by tuple of patterns. Returns the result as a list of found values.
-
-- [X] add option to access lists via python slice syntax ([issue #2](https://github.com/sarvensis/dict-picker/issues/2)):
-
-    ```python
-    {
-        arr:  [
-            { id: 123 },
-            { id: 456 },
-            { id: 789 },
-        ]
-    }
-    'arr/1/id' -> 456
-    'arr/1' -> { id: 123 }
-    'arr/:2/id' -> [123, 456]
-    'arr/1:' -> [{ id: 456 },{ id: 789 }]
-    'arr/::2/id' -> [123, 789]
-    ```
+# Dict picker (dictionary picker)
+
+Retrieve data from Python dictionaries and lists.
+
+## Installation
+
+With **pip**:
+
+```shell
+pip install -U dict-picker
+```
+
+Or with **conda**:
+
+```shell
+conda install "dict-picker" -c conda-forge
+```
+
+## Usage
+
+### `pick_by_path`
+
+The `pick_by_path` function is used to extract values from nested dictionaries using a path-like string to identify the desired value. The function takes three arguments: a dictionary object, a string representing the path to the desired value and optionally a delimiter.
+
+The path string consists of a sequence of keys, separated by the delimiter character (`'/'` by default), where each key represents a level in the nested dictionary. If the key has the value `'*'`, it matches any key on that level, or sets it to check all items in the list.
+
+The function returns the value at the end of the path or a list of values if the path contains a wildcard. If the path is not found, the function returns `None`.
+
+```python
+from dict_picker import pick_by_path
+
+example_dict = {
+    "foo": "bar",
+    "baz": {
+        "qux": "quux",
+        "quuux": "corge"
+    },
+    "fred": {
+        "wilma": "betty",
+        "barney": "pebbles"
+    },
+    "arr": [
+        { 'id': 123 },
+        { 'id': 456 },
+        { 'id': 789 },
+        { 'name': 'bubbles' },
+    ],
+}
+
+assert pick_by_path(example_dict, "foo") == "bar"
+assert pick_by_path(example_dict, "baz/qux") == "quux"
+assert pick_by_path(example_dict, "fred/wilma") == "betty"
+assert pick_by_path(example_dict, "*/qux") == "quux"
+assert pick_by_path(example_dict, "fred/*") == {"wilma": "betty", "barney": "pebbles"}
+assert pick_by_path(example_dict, "*/quux") is None
+assert pick_by_path(example_dict, "arr/*/id") == [123, 456, 789]
+
+# slice syntax
+assert pick_by_path(example_dict, "arr/0") == {'id': 123}
+assert pick_by_path(example_dict, "arr/1/id") == 456
+assert pick_by_path(example_dict, "arr/-1") == {'name': 'bubbles'}
+assert pick_by_path(example_dict, "arr/1:/id") == [456, 789, None]
+assert pick_by_path(example_dict, "arr/::-2/id") == [789, 123]
+```
+
+Parameters:
+
+- `obj` -- A dictionary object to search for the desired value.
+- `path: str` -- A string representing the path to the desired value.
+- `delimiter: str` -- A string used to separate keys in the path string. Default is "/".
+
+Return value:
+
+- Returns the value found at the end of the path string, or a list of values if the path contains a wildcard. If the path is not found, None is returned.
+
+
+### `pick_by_paths`
+
+The `pick_by_paths` function is similar to `pick_by_path`, but can extract values from multiple paths at once. It takes a dictionary object and a list of path strings as arguments, and returns a list of values found at the end of each path string or None if a path is not found. This works faster than running `pick_by_path` in a loop.
+
+```python
+from dict_picker import pick_by_path, pick_by_paths
+
+example_dict = {
+    "foo": "bar",
+    "baz": {
+        "qux": "quux",
+        "quuux": "corge"
+    },
+    "fred": {
+        "wilma": "betty",
+        "barney": "pebbles"
+    },
+    "arr": [
+        { 'id': 123 },
+        { 'id': 456 },
+        { 'id': 789 },
+        { 'name': 'bubbles' },
+    ],
+}
+
+assert pick_by_paths(example_dict, ["fred/*","*/quux", "arr/*/id",]) == [{"wilma": "betty", "barney": "pebbles"}, None, [123, 456, 789]]
+```
+
+## Build from sources
+
+### Cargo
+
+```shell
+curl --proto '=https' --tlsv1.2 -sSf <https://sh.rustup.rs> | sh
+```
+
+For other installation options, see [the official website](https://www.rust-lang.org/tools/install).
+
+### Maturin
+
+To bind python and rust, pyo3 is used. The [Maturin](https://github.com/PyO3/maturin) library is used to make it easy to work with.
+
+```shell
+python -m pip install maturin
+```
+
+### Build
+
+```shell
+python -m maturin build --release
+```
+
+Wheel will be released under the system and python in which it will be built. [Read more about the compilation](https://www.maturin.rs/distribution.html).
+
+The finished wheel can be found in the target/wheels folder.
+
+## Build with docker
+
+```shell
+docker run --rm -v $(pwd):/io ghcr.io/pyo3/maturin build --release  # or other maturin arguments
+```
+
+On macOS, it is better to use docker instead of podman.
+
+## Roadmap
+
+- [ ] Arbitrary levels skip operator `**`;
+- [X] Search inside an array of dictionaries. For example:
+
+    ```python
+    {
+        arr:  [
+            { id: 123 },
+            { id: 456 },
+            { id: 789 },
+        ]
+    }
+    'arr/*/id' -> [123, 456, 789]
+    ```
+
+- [X] Search by tuple of patterns. Returns the result as a list of found values.
+
+- [X] add option to access lists via python slice syntax ([issue #2](https://github.com/sarvensis/dict-picker/issues/2)):
+
+    ```python
+    {
+        arr:  [
+            { id: 123 },
+            { id: 456 },
+            { id: 789 },
+        ]
+    }
+    'arr/1/id' -> 456
+    'arr/1' -> { id: 123 }
+    'arr/:2/id' -> [123, 456]
+    'arr/1:' -> [{ id: 456 },{ id: 789 }]
+    'arr/::2/id' -> [123, 789]
+    ```
```

## Comparing `dict_picker-0.1.4.dist-info/license_files/LICENSE` & `dict_picker-0.1.5.dist-info/license_files/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 sarvensis
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 sarvensis
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

