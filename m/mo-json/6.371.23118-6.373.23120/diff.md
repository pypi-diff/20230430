# Comparing `tmp/mo_json-6.371.23118-py2.py3-none-any.whl.zip` & `tmp/mo_json-6.373.23120-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 30545 bytes, number of entries: 11
+Zip file size: 30499 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat    13208 b- defN 23-Apr-14 10:26 mo_json/__init__.py
 -rw-rw-rw-  2.0 fat      313 b- defN 23-Apr-14 10:26 mo_json/decoder.py
 -rw-rw-rw-  2.0 fat    15429 b- defN 23-Apr-14 10:26 mo_json/encoder.py
 -rw-rw-rw-  2.0 fat    16185 b- defN 23-Apr-14 10:26 mo_json/stream.py
--rw-rw-rw-  2.0 fat    17916 b- defN 23-Apr-14 10:26 mo_json/typed_encoder.py
--rw-rw-rw-  2.0 fat     9865 b- defN 23-Apr-14 10:26 mo_json/types.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-Apr-28 21:34 mo_json-6.371.23118.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    11641 b- defN 23-Apr-28 21:34 mo_json-6.371.23118.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-28 21:34 mo_json-6.371.23118.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-28 21:34 mo_json-6.371.23118.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      875 b- defN 23-Apr-28 21:34 mo_json-6.371.23118.dist-info/RECORD
-11 files, 102275 bytes uncompressed, 29085 bytes compressed:  71.6%
+-rw-rw-rw-  2.0 fat    17726 b- defN 23-Apr-30 12:14 mo_json/typed_encoder.py
+-rw-rw-rw-  2.0 fat    10240 b- defN 23-Apr-30 12:14 mo_json/types.py
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-Apr-30 12:15 mo_json-6.373.23120.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    11595 b- defN 23-Apr-30 12:15 mo_json-6.373.23120.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-30 12:15 mo_json-6.373.23120.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-30 12:15 mo_json-6.373.23120.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      876 b- defN 23-Apr-30 12:15 mo_json-6.373.23120.dist-info/RECORD
+11 files, 102415 bytes uncompressed, 29039 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: mo_json/typed_encoder.py
 Comment: 
 
 Filename: mo_json/types.py
 Comment: 
 
-Filename: mo_json-6.371.23118.dist-info/LICENSE
+Filename: mo_json-6.373.23120.dist-info/LICENSE
 Comment: 
 
-Filename: mo_json-6.371.23118.dist-info/METADATA
+Filename: mo_json-6.373.23120.dist-info/METADATA
 Comment: 
 
-Filename: mo_json-6.371.23118.dist-info/WHEEL
+Filename: mo_json-6.373.23120.dist-info/WHEEL
 Comment: 
 
-Filename: mo_json-6.371.23118.dist-info/top_level.txt
+Filename: mo_json-6.373.23120.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_json-6.371.23118.dist-info/RECORD
+Filename: mo_json-6.373.23120.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_json/typed_encoder.py

```diff
@@ -3,15 +3,14 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-import re
 from datetime import date, datetime, timedelta
 from decimal import Decimal
 
 from mo_dots import (
     CLASS,
     Data,
     DataObject,
@@ -20,14 +19,18 @@
     SLOT,
     _get,
     is_data,
     join_field,
     split_field,
     concat_field,
 )
+from mo_logs import Log
+from mo_logs.strings import quote
+from mo_times import Date, Duration
+
 from mo_future import (
     binary_type,
     generator_types,
     integer_types,
     is_binary,
     is_text,
     sort_using_key,
@@ -50,17 +53,15 @@
 from mo_json.encoder import (
     COLON,
     COMMA,
     UnicodeBuilder,
     json_encoder,
     problem_serializing,
 )
-from mo_logs import Log
-from mo_logs.strings import quote
-from mo_times import Date, Duration
+from mo_json.types import BOOLEAN_KEY, NUMBER_KEY, INTEGER_KEY, STRING_KEY, ARRAY_KEY, EXISTS_KEY, IS_TYPE_KEY
 
 
 def encode_property(name):
     return name.replace(",", "\\,").replace(".", ",")
 
 
 def decode_property(encoded):
@@ -100,37 +101,30 @@
 def get_nested_path(typed_path):
     # CONSTRUCT THE nested_path FROM THE typed_path
     path = split_field(typed_path)
     parent = "."
     nested_path = (parent,)
     for i, p in enumerate(path[:-1]):
         if p == ARRAY_KEY:
-            step = concat_field(parent, join_field(path[0 : i + 1]))
+            step = concat_field(parent, join_field(path[0: i + 1]))
             nested_path = (step,) + nested_path
     return nested_path
 
 
 def untyped(value):
     return _untype_value(value)
 
 
 def _untype_list(value):
     if any(is_data(v) for v in value):
         # MAY BE MORE TYPED OBJECTS IN THIS LIST
-        output = [_untype_value(v) for v in value]
+        return [_untype_value(v) for v in value]
     else:
         # LIST OF PRIMITIVE VALUES
-        output = value
-
-    if len(output) == 0:
-        return None
-    elif len(output) == 1:
-        return output[0]
-    else:
-        return output
+        return value
 
 
 def _untype_dict(value):
     output = {}
 
     for k, v in value.items():
         if IS_TYPE_KEY.match(k):
@@ -187,15 +181,15 @@
         if sub_schema.__class__.__name__ == "Column":
             value_json_type = python_type_to_jx_type[value.__class__]
             column_json_type = es_type_to_json_type[sub_schema.es_type]
 
             if value_json_type == column_json_type:
                 pass  # ok
             elif value_json_type == ARRAY and all(
-                python_type_to_jx_type[v.__class__] == column_json_type for v in value if v != None
+                    python_type_to_jx_type[v.__class__] == column_json_type for v in value if v != None
             ):
                 pass  # empty arrays can be anything
             else:
                 from mo_logs import Log
 
                 Log.error(
                     "Can not store {{value}} in {{column|quote}}", value=value, column=sub_schema.name,
@@ -490,22 +484,14 @@
         append(buffer, "1}")
     else:
         append(buffer, "{")
         append(buffer, QUOTED_EXISTS_KEY)
         append(buffer, "1}")
 
 
-IS_TYPE_KEY = re.compile(r"^~[bintdsaje]~$")
-BOOLEAN_KEY = "~b~"
-NUMBER_KEY = "~n~"
-INTEGER_KEY = "~i~"
-STRING_KEY = "~s~"
-ARRAY_KEY = "~N~"
-EXISTS_KEY = "~e~"
-
 append = UnicodeBuilder.append
 
 QUOTED_BOOLEAN_KEY = quote(BOOLEAN_KEY) + COLON
 QUOTED_NUMBER_KEY = quote(NUMBER_KEY) + COLON
 QUOTED_INTEGER_KEY = quote(INTEGER_KEY) + COLON
 QUOTED_STRING_KEY = quote(STRING_KEY) + COLON
 QUOTED_ARRAY_KEY = quote(ARRAY_KEY) + COLON
```

## mo_json/types.py

```diff
@@ -43,17 +43,17 @@
 
         dirty = False
         for k, ov in od.items():
             sv = sd.get(k)
             if sv is ov:
                 continue
             if sv is None:
-                if k in JX_NUMBER_TYPES.__dict__ and sd.get(_N):
+                if k in JX_NUMBER_TYPES.__dict__ and sd.get(NUMBER_KEY):
                     continue
-                elif k is _N and any(sd.get(kk) for kk in JX_NUMBER_TYPES.__dict__.keys()):
+                elif k is NUMBER_KEY and any(sd.get(kk) for kk in JX_NUMBER_TYPES.__dict__.keys()):
                     for kk in JX_NUMBER_TYPES.__dict__.keys():
                         try:
                             del sd[kk]
                         except Exception as cause:
                             pass
                     sd[k] = JX_NUMBER.__dict__[k]
                     dirty = True
@@ -111,15 +111,15 @@
 
     def __ne__(self, other):
         if self is JX_ANY and other is ARRAY:
             return False
         return not self == other
 
     def __eq__(self, other):
-        if other is ARRAY and hasattr(self, _A):
+        if other is ARRAY and hasattr(self, ARRAY_KEY):
             # SHALLOW CHECK IF THIS IS AN ARRAY
             return True
 
         if not isinstance(other, JxType):
             return False
 
         if self is JX_INTEGER or self is JX_NUMBER:
@@ -168,23 +168,23 @@
         return str(self.__data__())
 
     def __repr__(self):
         return "JxType(**" + str(self.__data__()) + ")"
 
 
 def array_of(type_):
-    return JxType(**{_A: type_})
+    return JxType(**{ARRAY_KEY: type_})
 
 
 def member_type(type_):
     """
     RETURN THE MEMBER TYPE, IF AN ARRAY
     """
     if type_ == ARRAY:
-        return getattr(type_, _A)
+        return getattr(type_, ARRAY_KEY)
     else:
         return type_
 
 
 def base_type(type_):
     """
     TYPES OFTEN COME WITH SIMPLE NAMES THAT GET IN THE WAY OF THE "BASE TYPE"
@@ -215,15 +215,15 @@
 
     for t in types:
         output |= t
     return output
 
 
 def array_type(item_type):
-    return _primitive(_A, item_type)
+    return _primitive(ARRAY_KEY, item_type)
 
 
 _new = object.__new__
 
 
 def _primitive(name, value):
     output = _new(JxType)
@@ -257,27 +257,27 @@
 }
 JSON_TYPES = (BOOLEAN, INTEGER, NUMBER, STRING, OBJECT)
 NUMBER_TYPES = (INTEGER, NUMBER, TIME, INTERVAL)
 PRIMITIVE = (EXISTS, BOOLEAN, INTEGER, NUMBER, TIME, INTERVAL, STRING)
 INTERNAL = (EXISTS, OBJECT, ARRAY)
 STRUCT = (OBJECT, ARRAY)
 
-_B, _I, _N, _T, _D, _S, _A, _J = "~b~", "~i~", "~n~", "~t~", "~d~", "~s~", "~a~", "~j~"
-ARRAY_KEY = _A
+BOOLEAN_KEY, INTEGER_KEY, NUMBER_KEY, TIME_KEY, DURATION_KEY, STRING_KEY, ARRAY_KEY, EXISTS_KEY, JSON_KEY = "~b~", "~i~", "~n~", "~t~", "~d~", "~s~", "~a~", "~e~", "~j~"
 IS_PRIMITIVE_KEY = re.compile(r"^~[bintds]~$")
+IS_TYPE_KEY = re.compile(r"^~[bintdsaje]~$")
 
 JX_IS_NULL = _new(JxType)
-JX_BOOLEAN = _primitive(_B, BOOLEAN)
-JX_INTEGER = _primitive(_I, INTEGER)
-JX_NUMBER = _primitive(_N, NUMBER)
-JX_TIME = _primitive(_T, TIME)
-JX_INTERVAL = _primitive(_D, INTERVAL)  # d FOR DELTA
-JX_TEXT = _primitive(_S, STRING)
-JX_ARRAY = _primitive(_A, ARRAY)
-JX_ANY = _primitive(_J, JSON)
+JX_BOOLEAN = _primitive(BOOLEAN_KEY, BOOLEAN)
+JX_INTEGER = _primitive(INTEGER_KEY, INTEGER)
+JX_NUMBER = _primitive(NUMBER_KEY, NUMBER)
+JX_TIME = _primitive(TIME_KEY, TIME)
+JX_INTERVAL = _primitive(DURATION_KEY, INTERVAL)  # d FOR DELTA
+JX_TEXT = _primitive(STRING_KEY, STRING)
+JX_ARRAY = _primitive(ARRAY_KEY, ARRAY)
+JX_ANY = _primitive(JSON_KEY, JSON)
 
 JX_PRIMITIVE = _new(JxType)
 JX_PRIMITIVE.__dict__ = [
     (x, x.update(d))[0]
     for x in [{}]
     for d in [
         JX_BOOLEAN.__dict__,
@@ -325,15 +325,15 @@
     elif is_sequence(v):
         return ARRAY
     return None
 
 
 def value_to_jx_type(value):
     if is_many(value):
-        return _primitive(_A, union_type(*(value_to_json_type(v) for v in value)))
+        return _primitive(ARRAY_KEY, union_type(*(value_to_json_type(v) for v in value)))
     elif is_data(value):
         return JxType(**{k: value_to_json_type(v) for k, v in value.items()})
     else:
         return _python_type_to_jx_type[value.__class__]
 
 
 def python_type_to_jx_type(type):
@@ -370,31 +370,31 @@
     date: JX_TIME,
 }
 
 for k, v in items(_python_type_to_jx_type):
     _python_type_to_jx_type[k.__name__] = v
 
 jx_type_to_key = {
-    JX_IS_NULL: _J,
-    JX_BOOLEAN: _B,
-    JX_INTEGER: _I,
-    JX_NUMBER: _N,
-    JX_TIME: _T,
-    JX_INTERVAL: _D,
-    JX_TEXT: _S,
-    JX_ARRAY: _A,
+    JX_IS_NULL: JSON_KEY,
+    JX_BOOLEAN: BOOLEAN_KEY,
+    JX_INTEGER: INTEGER_KEY,
+    JX_NUMBER: NUMBER_KEY,
+    JX_TIME: TIME_KEY,
+    JX_INTERVAL: DURATION_KEY,
+    JX_TEXT: STRING_KEY,
+    JX_ARRAY: ARRAY_KEY,
 }
 
 python_type_to_jx_type_key = {
-    bool: _B,
-    int: _I,
-    float: _N,
-    Decimal: _N,
-    Date: _T,
-    datetime: _T,
-    date: _T,
-    text: _S,
-    NullType: _J,
-    none_type: _J,
-    list: _A,
-    set: _A,
+    bool: BOOLEAN_KEY,
+    int: INTEGER_KEY,
+    float: NUMBER_KEY,
+    Decimal: NUMBER_KEY,
+    Date: TIME_KEY,
+    datetime: TIME_KEY,
+    date: TIME_KEY,
+    text: STRING_KEY,
+    NullType: JSON_KEY,
+    none_type: JSON_KEY,
+    list: ARRAY_KEY,
+    set: ARRAY_KEY,
 }
```

## Comparing `mo_json-6.371.23118.dist-info/LICENSE` & `mo_json-6.373.23120.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_json-6.371.23118.dist-info/METADATA` & `mo_json-6.373.23120.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-json
-Version: 6.371.23118
+Version: 6.373.23120
 Summary: More JSON Tools! 
 Home-page: https://github.com/klahnakoski/mo-json
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -18,15 +18,14 @@
 License-File: LICENSE
 Requires-Dist: hjson
 Requires-Dist: mo-dots (==9.368.23092)
 Requires-Dist: mo-future (==7.340.23006)
 Requires-Dist: mo-logs (==7.371.23118)
 Requires-Dist: mo-times (==5.371.23118)
 Provides-Extra: tests
-Requires-Dist: pyLibrary ; extra == 'tests'
 Requires-Dist: mo-testing ; extra == 'tests'
 Requires-Dist: mo-threads ; extra == 'tests'
 
 # More JSON Tools
 
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mo-json.svg)](https://pypi.org/project/mo-json/)
@@ -334,10 +333,10 @@
 
 **Update Mar2016** - *PyPy version 5.x appears to have improved C integration to
 the point that the C library callbacks are no longer a significant overhead:
 This pure Python JSON encoder is no longer faster than a compound C/Python
 solution.*
 
 Fast JSON encoder used in `convert.value2json()` when running in Pypy. Run the
-[speedtest](https://github.com/klahnakoski/pyLibrary/blob/dev/tests/speedtest_json.py)
+[speed test](https://github.com/klahnakoski/mo-json/blob/dev/tests/speedtest_json.py)
 to compare with default implementation and ujson
```

## Comparing `mo_json-6.371.23118.dist-info/RECORD` & `mo_json-6.373.23120.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 mo_json/__init__.py,sha256=u8xZL00hAoeMsFwimj6TjfHuzTaiKjsqW6Vm8fXquV0,13208
 mo_json/decoder.py,sha256=iCE9aa_bwOCD6iDk461ywcHIBMJye-YIicGM6ILMlBk,313
 mo_json/encoder.py,sha256=PH8y_YEz9TSNhm1QJy2eW1PKUSPE2GdZwtHkASb18Js,15429
 mo_json/stream.py,sha256=DRbMb3IwpyW1s2J-Udws1wjCVCbaXGiXAa_7Ao9W4tI,16185
-mo_json/typed_encoder.py,sha256=t2f3u3Qy9dZkybEurPyQw7YI8kliCcUn3FlOP9vJlAQ,17916
-mo_json/types.py,sha256=mywKG-fBpSQ-V1lCgWLdXPhH6FmZzXRQubrJCofr2xE,9865
-mo_json-6.371.23118.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
-mo_json-6.371.23118.dist-info/METADATA,sha256=h5O-6_WWhPMA4bPlOqLMhwoaO9PLIulEnXTIfW1gU_s,11641
-mo_json-6.371.23118.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_json-6.371.23118.dist-info/top_level.txt,sha256=svvpHEXHZaMl3nAq8QPmHxHJjsBFiFLZ2RSfAVPck1g,8
-mo_json-6.371.23118.dist-info/RECORD,,
+mo_json/typed_encoder.py,sha256=AdNgUXz3V6-LHFYa6dgkPA1uIT_ZqB3T8fsZUw5OcLU,17726
+mo_json/types.py,sha256=VSLHgpQ8KF1iTXuqV0XTZILaLO28AGSrab_wdFLgo48,10240
+mo_json-6.373.23120.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
+mo_json-6.373.23120.dist-info/METADATA,sha256=GD_ZOdxib6OL7Yd-QNaxDCM-4n5yLvKRrfkJjJd6EsY,11595
+mo_json-6.373.23120.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_json-6.373.23120.dist-info/top_level.txt,sha256=svvpHEXHZaMl3nAq8QPmHxHJjsBFiFLZ2RSfAVPck1g,8
+mo_json-6.373.23120.dist-info/RECORD,,
```

