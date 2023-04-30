# Comparing `tmp/mmif-python-0.4.8.tar.gz` & `tmp/mmif-python-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmif-python-0.4.8.tar", last modified: Fri Feb 10 01:26:36 2023, max compression
+gzip compressed data, was "mmif-python-0.5.0.tar", last modified: Sun Apr 30 04:04:27 2023, max compression
```

## Comparing `mmif-python-0.4.8.tar` & `mmif-python-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 01:26:36.497193 mmif-python-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-02-10 01:26:00.000000 mmif-python-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-10 01:26:00.000000 mmif-python-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-02-10 01:26:36.497193 mmif-python-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-02-10 01:26:00.000000 mmif-python-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-10 01:26:28.000000 mmif-python-0.4.8/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 01:26:36.497193 mmif-python-0.4.8/mmif/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-02-10 01:26:01.000000 mmif-python-0.4.8/mmif/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 01:26:36.497193 mmif-python-0.4.8/mmif/res/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 01:26:36.000000 mmif-python-0.4.8/mmif/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-02-10 01:26:36.000000 mmif-python-0.4.8/mmif/res/clams.vocabulary.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-10 01:26:36.000000 mmif-python-0.4.8/mmif/res/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-02-10 01:26:36.000000 mmif-python-0.4.8/mmif/res/mmif.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 01:26:36.497193 mmif-python-0.4.8/mmif/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-10 01:26:01.000000 mmif-python-0.4.8/mmif/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-02-10 01:26:01.000000 mmif-python-0.4.8/mmif/serialize/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19125 2023-02-10 01:26:01.000000 mmif-python-0.4.8/mmif/serialize/mmif.py
--rw-r--r--   0 runner    (1001) docker     (123)    18396 2023-02-10 01:26:01.000000 mmif-python-0.4.8/mmif/serialize/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15448 2023-02-10 01:26:01.000000 mmif-python-0.4.8/mmif/serialize/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 01:26:36.497193 mmif-python-0.4.8/mmif/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-10 01:26:36.000000 mmif-python-0.4.8/mmif/ver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-10 01:26:36.000000 mmif-python-0.4.8/mmif/ver/do-not-edit.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 01:26:36.497193 mmif-python-0.4.8/mmif/vocabulary/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-10 01:26:36.000000 mmif-python-0.4.8/mmif/vocabulary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-02-10 01:26:36.000000 mmif-python-0.4.8/mmif/vocabulary/annotation_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-02-10 01:26:36.000000 mmif-python-0.4.8/mmif/vocabulary/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-10 01:26:36.000000 mmif-python-0.4.8/mmif/vocabulary/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-02-10 01:26:36.000000 mmif-python-0.4.8/mmif/vocabulary/document_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 01:26:36.497193 mmif-python-0.4.8/mmif_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-02-10 01:26:36.000000 mmif-python-0.4.8/mmif_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-02-10 01:26:36.000000 mmif-python-0.4.8/mmif_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 01:26:36.000000 mmif-python-0.4.8/mmif_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-10 01:26:36.000000 mmif-python-0.4.8/mmif_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-10 01:26:36.000000 mmif-python-0.4.8/mmif_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-10 01:26:01.000000 mmif-python-0.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-10 01:26:36.497193 mmif-python-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-02-10 01:26:01.000000 mmif-python-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:04:27.509018 mmif-python-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-04-30 04:03:52.000000 mmif-python-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-30 04:03:52.000000 mmif-python-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-30 04:04:27.509018 mmif-python-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-30 04:03:52.000000 mmif-python-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 04:03:53.000000 mmif-python-0.5.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:04:27.505018 mmif-python-0.5.0/mmif/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-30 04:03:52.000000 mmif-python-0.5.0/mmif/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:04:27.505018 mmif-python-0.5.0/mmif/res/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/res/clams.vocabulary.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/res/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/res/mmif.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:04:27.509018 mmif-python-0.5.0/mmif/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-30 04:03:52.000000 mmif-python-0.5.0/mmif/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-04-30 04:03:52.000000 mmif-python-0.5.0/mmif/serialize/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19125 2023-04-30 04:03:52.000000 mmif-python-0.5.0/mmif/serialize/mmif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18396 2023-04-30 04:03:52.000000 mmif-python-0.5.0/mmif/serialize/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-04-30 04:03:52.000000 mmif-python-0.5.0/mmif/serialize/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:04:27.509018 mmif-python-0.5.0/mmif/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/ver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/ver/do-not-edit.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:04:27.509018 mmif-python-0.5.0/mmif/vocabulary/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/vocabulary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/vocabulary/annotation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/vocabulary/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/vocabulary/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/vocabulary/document_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:04:27.509018 mmif-python-0.5.0/mmif_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 04:03:52.000000 mmif-python-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 04:04:27.509018 mmif-python-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-30 04:03:52.000000 mmif-python-0.5.0/setup.py
```

### Comparing `mmif-python-0.4.8/LICENSE` & `mmif-python-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mmif-python-0.4.8/PKG-INFO` & `mmif-python-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 0.4.8
+Version: 0.5.0
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: # MMIF for python
```

### Comparing `mmif-python-0.4.8/README.md` & `mmif-python-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mmif-python-0.4.8/mmif/res/clams.vocabulary.yaml` & `mmif-python-0.5.0/mmif/res/clams.vocabulary.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Changes in this file will automatically increase versions of changed object.
+# The versions of types included in a particular MMIF (more specifically CLAMS vocab)
+# is recorded under `docs/x.y.z/vocabulary/ATTYPE_VERSIONS_JSONFILENAME`
+# Note that individuated type versioning is introduced after 0.4.2, 
+# so `docs/x.y.z` sub-directories of <= 0.4.2 won't have that JSON files.
 
 name: Thing
 parent: null
 
 description: >-
   Abstract top type.
```

### Comparing `mmif-python-0.4.8/mmif/res/mmif.json` & `mmif-python-0.5.0/mmif/res/mmif.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9960588727678572%*

 * *Differences: {"'definitions'": "{'mmifMetadata': {'properties': {'mmif': {'minLength': 7}}}, 'viewMetadata': "*

 * *                  "{'properties': {'app': {'minLength': 7}, 'error': {'properties': {'message': "*

 * *                  "{'minLength': 1}}}, 'warnings': {'minLength': 1}}}, 'view': {'properties': "*

 * *                  "{'id': {'minLength': 1}}}, 'annotation': {'properties': {'@type': {'minLength': "*

 * *                  "1}}}, 'annotationProperties': {'properties': {'id': {'minLength': 1}}}}",*

 * * "'properties'": "{'docume […]*

```diff
@@ -2,14 +2,15 @@
     "$schema": "http://json-schema.org/draft-04/schema#",
     "additionalProperties": false,
     "definitions": {
         "annotation": {
             "additionalProperties": false,
             "properties": {
                 "@type": {
+                    "minLength": 1,
                     "type": "string"
                 },
                 "properties": {
                     "$ref": "#/definitions/annotationProperties"
                 }
             },
             "required": [
@@ -17,26 +18,28 @@
                 "properties"
             ],
             "type": "object"
         },
         "annotationProperties": {
             "properties": {
                 "id": {
+                    "minLength": 1,
                     "type": "string"
                 }
             },
             "required": [
                 "id"
             ],
             "type": "object"
         },
         "mmifMetadata": {
             "properties": {
                 "mmif": {
                     "format": "uri",
+                    "minLength": 7,
                     "type": "string"
                 }
             },
             "required": [
                 "mmif"
             ],
             "type": "object"
@@ -70,14 +73,15 @@
                 "annotations": {
                     "items": {
                         "$ref": "#/definitions/annotation"
                     },
                     "type": "array"
                 },
                 "id": {
+                    "minLength": 1,
                     "type": "string"
                 },
                 "metadata": {
                     "$ref": "#/definitions/viewMetadata"
                 }
             },
             "required": [
@@ -107,28 +111,30 @@
                         "error"
                     ]
                 }
             ],
             "properties": {
                 "app": {
                     "format": "uri",
+                    "minLength": 7,
                     "type": "string"
                 },
                 "contains": {
                     "additionalProperties": false,
                     "patternProperties": {
                         "^https?://": {
                             "$ref": "#/definitions/strStrMap"
                         }
                     },
                     "type": "object"
                 },
                 "error": {
                     "properties": {
                         "message": {
+                            "minLength": 1,
                             "type": "string"
                         },
                         "stackTrace": {
                             "type": "string"
                         }
                     },
                     "required": [
@@ -143,26 +149,28 @@
                     "format": "date-time",
                     "type": "string"
                 },
                 "warnings": {
                     "items": {
                         "type": "string"
                     },
+                    "minLength": 1,
                     "type": "array"
                 }
             },
             "type": "object"
         }
     },
     "description": "The JSON-LD objects exchanged by CLAMS services.",
     "properties": {
         "documents": {
             "items": {
                 "$ref": "#/definitions/annotation"
             },
+            "minLength": 1,
             "type": "array"
         },
         "metadata": {
             "$ref": "#/definitions/mmifMetadata"
         },
         "views": {
             "items": {
```

### Comparing `mmif-python-0.4.8/mmif/serialize/annotation.py` & `mmif-python-0.5.0/mmif/serialize/annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             self.properties: AnnotationProperties = AnnotationProperties()
             self._attribute_classes = {'properties': AnnotationProperties}
         self.disallow_additional_properties()
         self._required_attributes = ["_type", "properties"]
         super().__init__(anno_obj)
     
     def _deserialize(self, input_dict: dict) -> None:
-        self.at_type = input_dict.pop('_type')
+        self.at_type = input_dict.pop('_type', '')
         # TODO (krim @ 6/1/21): If annotation IDs must follow a certain string format,
         # (e.g. currently auto-generated IDs will always have "prefix"_"number" format)
         # here is the place to parse formatted IDs and store prefixes in the parent mmif object. 
         # (see https://github.com/clamsproject/mmif/issues/64#issuecomment-849241309 for discussion)
         super()._deserialize(input_dict)
         
     def is_type(self, at_type: Union[str, ThingTypesBase]) -> bool:
@@ -110,15 +110,15 @@
 
     If ``document_obj`` is not provided, an empty Document will be generated.
 
     :param document_obj: the JSON data that defines the document
     """
     def __init__(self, doc_obj: Optional[Union[bytes, str, dict]] = None) -> None:
         self._parent_view_id = ''
-        self._type: Union[str, DocumentTypesBase] = ''
+        self._type: Union[ThingTypesBase, DocumentTypesBase] = ThingTypesBase('')
         self.properties: DocumentProperties = DocumentProperties()
         self.disallow_additional_properties()
         self._attribute_classes = {'properties': DocumentProperties}
         super().__init__(doc_obj)
 
     @property
     def parent(self) -> str:
@@ -286,15 +286,14 @@
 
     def _serialize(self, alt_container: Optional[Dict] = None) -> dict:
         serialized = super()._serialize()
         if "location_" in serialized:
             serialized["location"] = serialized.pop("location_")
         return serialized
 
-
     @property
     def text_language(self) -> str:
         return self.text.lang
 
     @text_language.setter
     def text_language(self, lang_code: str) -> None:
         self.text.lang = lang_code
```

### Comparing `mmif-python-0.4.8/mmif/serialize/mmif.py` & `mmif-python-0.5.0/mmif/serialize/mmif.py`

 * *Files identical despite different names*

### Comparing `mmif-python-0.4.8/mmif/serialize/model.py` & `mmif-python-0.5.0/mmif/serialize/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,15 +349,15 @@
 
     @staticmethod
     def _load_json(json_list: Union[list, str]) -> list:
         if type(json_list) is str:
             json_list = json.loads(json_list)
         return [MmifObject._load_json(obj) for obj in json_list]
     
-    def _deserialize(self, input_list: dict) -> None:
+    def _deserialize(self, input_list: list) -> None:
         raise NotImplementedError()
 
     def get(self, key: str) -> Optional[T]:
         """
         Standard dictionary-style get() method, albeit with no ``default``
         parameter. Relies on the implementation of __getitem__.
```

### Comparing `mmif-python-0.4.8/mmif/serialize/view.py` & `mmif-python-0.5.0/mmif/serialize/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 In MMIF, views are created by apps in a pipeline that are annotating
 data that was previously present in the MMIF file.
 """
 from datetime import datetime
 from typing import Dict, Union, Optional, Generator, List, cast
 
-from mmif.vocabulary import ThingTypesBase
+from mmif.vocabulary import ThingTypesBase, ClamsTypesBase
 from .annotation import Annotation, Document
 from .model import MmifObject, DataList, DataDict
 
 __all__ = ['View', 'ViewMetadata', 'Contain']
 
 from .. import DocumentTypes
 
@@ -321,15 +321,15 @@
         Extends base ``_deserialize`` method to initialize ``items`` as a dict from
         annotation IDs to :class:`mmif.serialize.annotation.Annotation` objects.
 
         :param input_list: the JSON data that defines the list of annotations
         :return: None
         """
         self._items = {item['properties']['id']: Document(item)
-                       if item['_type'].endswith("Document") else Annotation(item)
+                       if ClamsTypesBase.attype_iri_isdocument(item['_type']) else Annotation(item)
                        for item in input_list}
 
     def append(self, value: Union[Annotation, Document], overwrite=False) -> None:
         """
         Appends an annotation to the list.
 
         Fails if there is already an annotation with the same ID
```

### Comparing `mmif-python-0.4.8/mmif/vocabulary/base_types.py` & `mmif-python-0.5.0/mmif/vocabulary/base_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 class TypesBase(object):
     """
     Base class for arbitrary vocabulary type. 
     This class provides bisic initializer, comparators, 
     and (de-)serialization methods. 
     """
     _prefixes = {}
-    base_url: str
+    base_uri: str
     shortname: str
     
     def __init__(self, type_uri: str):
         self.parse_names(type_uri)
         if self.__repr__() not in self.__class__._prefixes:
+            # prepare auto-inferred prefix for Annotations.[].id field
             self.__class__._prefixes[self.__repr__()] \
                 = self.__class__._create_prefix(self.shortname,
-                                               self.__class__._prefixes.values()
-                                               )
+                                                self.__class__._prefixes.values()
+                                                )
     
-    def parse_names(self, type_uri:str):
+    def parse_names(self, type_uri: str):
         if '/' in type_uri:
             self.base_uri, self.shortname = type_uri.rsplit('/', 1)
         else:
             self.base_uri = ""
             self.shortname = type_uri
 
     @classmethod
@@ -51,18 +52,22 @@
                     else:
                         continue
                     break
         else:
             prefix = None
         return prefix
 
+    @staticmethod
+    def attype_iri_isdocument(iri):
+        return 'Document/' in iri or iri.endswith('Document')
+
     @classmethod
     def from_str(cls, string: str):
         if 'mmif.clams.ai' in string:
-            if string.endswith('Document'):
+            if cls.attype_iri_isdocument(string):
                 return DocumentTypesBase(string)
             else:
                 return AnnotationTypesBase(string)
         else:
             return cls(string)
     
     def __hash__(self):
@@ -70,15 +75,15 @@
         
     def __eq__(self, other):
         if isinstance(other, str):
             other = self.from_str(other)
         return isinstance(other, TypesBase) and self.base_uri == other.base_uri and self.shortname == other.shortname
             
     def __repr__(self):
-        if len(self.base_uri) > 0: 
+        if self.base_uri:
             return f'{self.base_uri}/{self.shortname}'
         else:
             return self.shortname
     
     # aliases
     def __str__(self):
         return self.__repr__()
@@ -101,41 +106,60 @@
     This class adds handling of MMIF specification versions 
     in initializer and comparators. 
     """
     version: str
     dev_version: ClassVar[str] = 'develop'
     
     def parse_names(self, type_uri:str):
-        if 'mmif.clams.ai' not in type_uri:
-            raise ValueError(f'{type_uri} is not a CLAMS vocabulary URI')
-        self.base_uri, self.version, _, self.shortname = type_uri.rsplit('/', 3)
+        if not type_uri:
+            self.base_uri, self.shortname, self.version = "", "", ""
+        elif 'mmif.clams.ai' not in type_uri:
+            raise ValueError(f'Cannot process "{type_uri}"!: not a CLAMS vocabulary URI')
+        elif type_uri[-1].isdigit():  # new versioning
+            self.base_uri, _, self.shortname, self.version = type_uri.rsplit('/', 3)
+        else:  # legacy versioning
+            self.base_uri, self.version, _, self.shortname = type_uri.rsplit('/', 3)
+            self._check_legacy_version(self.version)
+
+    def _check_legacy_version(self, legacy_ver):
+        if legacy_ver < '0.4.0':
+            raise ValueError(f'Cannot process "{self}"!: CLAMS annotation types from old MMIF (older than 0.4.0) are no '
+                             f'longer supported with this app.')
+        if legacy_ver > '0.4.2':
+            raise ValueError(f'Cannot process "{self}"!: Invalid CLAMS vocabulary type URI.')
+        return True
 
     def __hash__(self):
         return hash(str(self))
 
     def __eq__(self, other):
         if isinstance(other, str):
             other = ThingTypesBase.from_str(other)
         if isinstance(other, ClamsTypesBase):
-            if '.' in self.version and '.' in other.version:
-                # regular version 
-                s_major, s_minor, s_patch = self.version.split('.')
-                o_major, o_minor, o_patch = other.version.split('.')
-                if s_major != o_major or s_minor != o_minor:
-                    return False
-            else:
-                # dummy version given at development time
-                if ClamsTypesBase.dev_version not in {self.version, other.version}: # dummy version given at development time
-                    return False
-            return self.base_uri == other.base_uri and self.shortname == other.shortname
+            vers = []
+            for o in (self, other):
+                if '.' in o.version and self._check_legacy_version(o.version):
+                    # legacy mapping: see https://github.com/clamsproject/mmif/issues/14#issuecomment-1504439497
+                    if o.version == '0.4.2' and o.shortname == 'Annotation':
+                        vers.append('v2')
+                    elif o.version.startswith('0.4.'):
+                        vers.append('v1')
+                else:
+                    vers.append(o.version)
+            return self.base_uri == other.base_uri \
+                and self.shortname == other.shortname \
+                and vers[0] == vers[1]
         else:
             return False
     
     def __repr__(self):
-        return f'{self.base_uri}/{self.version}/vocabulary/{self.shortname}'
+        if self.version[0] == 'v':
+            return f'{self.base_uri}/vocabulary/{self.shortname}/{self.version}'
+        else:
+            return f'{self.base_uri}/{self.version}/vocabulary/{self.shortname}'
 
 
 class AnnotationTypesBase(ClamsTypesBase):
     """
     Inherit from this class to build your own custom annotation
     vocabularies. 
     """
@@ -149,10 +173,11 @@
     """
     ...
 
 
 class ThingType(ThingTypesBase):
     """
     This class contains the topmost CLAMS thing type 
-    defined in the spec version 0.4.2 as a class variable. 
+    defined in the spec version 0.5.0 as a class variable. 
     """
-    Thing = ClamsTypesBase('http://mmif.clams.ai/0.4.2/vocabulary/Thing')
+    Thing = ClamsTypesBase('http://mmif.clams.ai/vocabulary/Thing/v1')
+    typevers = {'Thing': 'v1'}
```

### Comparing `mmif-python-0.4.8/mmif/vocabulary/document_types.py` & `mmif-python-0.5.0/mmif/vocabulary/document_types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# Spec version 0.4.2
+# Spec version 0.5.0
 # This file is auto-generated by setup.py
 
 from .base_types import DocumentTypesBase
 
 
 class DocumentTypes(DocumentTypesBase):
     """
     This class contains the CLAMS document types 
-    defined in the spec version 0.4.2 as class variables. 
+    defined in the spec version 0.5.0 as class variables. 
     """
-    Document = DocumentTypesBase('http://mmif.clams.ai/0.4.2/vocabulary/Document')
-    VideoDocument = DocumentTypesBase('http://mmif.clams.ai/0.4.2/vocabulary/VideoDocument')
-    AudioDocument = DocumentTypesBase('http://mmif.clams.ai/0.4.2/vocabulary/AudioDocument')
-    ImageDocument = DocumentTypesBase('http://mmif.clams.ai/0.4.2/vocabulary/ImageDocument')
-    TextDocument = DocumentTypesBase('http://mmif.clams.ai/0.4.2/vocabulary/TextDocument')
+    Document = DocumentTypesBase('http://mmif.clams.ai/vocabulary/Document/v1')
+    VideoDocument = DocumentTypesBase('http://mmif.clams.ai/vocabulary/VideoDocument/v1')
+    AudioDocument = DocumentTypesBase('http://mmif.clams.ai/vocabulary/AudioDocument/v1')
+    ImageDocument = DocumentTypesBase('http://mmif.clams.ai/vocabulary/ImageDocument/v1')
+    TextDocument = DocumentTypesBase('http://mmif.clams.ai/vocabulary/TextDocument/v1')
+    typevers = {'Document': 'v1', 'VideoDocument': 'v1', 'AudioDocument': 'v1', 'ImageDocument': 'v1', 'TextDocument': 'v1'}
```

### Comparing `mmif-python-0.4.8/mmif_python.egg-info/PKG-INFO` & `mmif-python-0.5.0/mmif_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 0.4.8
+Version: 0.5.0
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: # MMIF for python
```

### Comparing `mmif-python-0.4.8/mmif_python.egg-info/SOURCES.txt` & `mmif-python-0.5.0/mmif_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmif-python-0.4.8/setup.py` & `mmif-python-0.5.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 #! /usr/bin/env python3
 import io
 import json
 import os
+import re
 import shutil
+import string
+import subprocess
 from os.path import join as pjoin
 from typing import Union
 from urllib import request
 
 import setuptools.command.build_py
 import setuptools.command.develop
 
@@ -25,14 +28,15 @@
 mmif_name = "mmif"
 mmif_res_pkg = 'res'
 mmif_ver_pkg = 'ver'
 mmif_vocabulary_pkg = 'vocabulary'
 mmif_schema_res_oriname = 'schema/mmif.json'
 mmif_schema_res_name = 'mmif.json'
 mmif_vocab_res_oriname = 'vocabulary/clams.vocabulary.yaml'
+mmif_vocab_attypevers_res_oriname = 'docs/{version}/vocabulary/attypeversions.json'
 mmif_vocab_res_name = 'clams.vocabulary.yaml'
 
 
 def do_not_edit_warning(dirname):
     with open(pjoin(dirname, 'do-not-edit.txt'), 'w') as warning:
         warning.write("Contents of this directory is automatically generated and should not be manually edited.\n")
         warning.write("Any manual changes will be wiped at next build time.\n")
@@ -45,31 +49,31 @@
     do_not_edit_warning(subpack_dir)
     init_mod = open(pjoin(subpack_dir, '__init__.py'), 'w')
     init_mod.write(init_contents)
     init_mod.close()
     return subpack_dir
 
 
-def generate_vocab_enum(spec_version, clams_types, mod_name) -> str:
-    vocab_url = 'http://mmif.clams.ai/%s/vocabulary' % spec_version
+def generate_vocab_enum(spec_version, clams_types_vers, mod_name) -> str:
     
     template_file = os.path.join(vocabulary_templates_path, mod_name + '.txt')
     if mod_name.startswith('annotation'):
         base_class_name = 'AnnotationTypesBase'
     elif mod_name.startswith('document'):
         base_class_name = 'DocumentTypesBase'
     else: 
         base_class_name = 'ClamsTypesBase'
 
     file_out = io.StringIO()
     with open(template_file, 'r') as file_in:
-        for line in file_in.readlines():
-            file_out.write(line.replace('<VERSION>', spec_version))
-        for type_name in clams_types:
-            file_out.write(f"    {type_name} = {base_class_name}('{vocab_url}/{type_name}')\n")
+        file_out.write(string.Template(file_in.read()).safe_substitute(VERSION=spec_version))
+    for type_name, type_ver in clams_types_vers:
+        vocab_url = f'http://mmif.clams.ai/vocabulary/{type_name}/{type_ver}'
+        file_out.write(f"    {type_name} = {base_class_name}('{vocab_url}')\n")
+    file_out.write(f"    typevers = {dict(clams_types_vers)}\n")
 
     string_out = file_out.getvalue()
     file_out.close()
     return string_out
 
 
 def update_target_spec(target_vers_csv, specver):
@@ -108,18 +112,18 @@
         if not lines[1].startswith(version):
             lines.insert(1, f'{version},"{specver}"\n')
         for line in lines:
             out_f.write(line)
         shutil.move(out_f.name, in_f.name)
 
 
-def generate_vocabulary(spec_version, clams_types):
+def generate_vocabulary(spec_version, clams_types_vers):
     """
     :param spec_version:
-    :param clams_types: the tree
+    :param clams_types_vers: list of (name, version) tuples of annotation types in CLAMS vocab
     :param template_path: the directory of source txt files
     :return:
     """
     types = {
         'base_types': ['ThingTypesBase', 'ThingType', 'ClamsTypesBase', 'AnnotationTypesBase', 'DocumentTypesBase'],
         'annotation_types': ['AnnotationTypes'],
         'document_types': ['DocumentTypes']
@@ -128,51 +132,53 @@
         mmif_name, mmif_vocabulary_pkg,
         '\n'.join(
             f"from .{mod_name} import {class_name}"
             for mod_name, classes in types.items()
             for class_name in classes
         )+'\n'
     )
+    document_types = []
+    annotation_types = []
+    base_types = []
+    
+    for n, v in clams_types_vers.items():
+        if n == 'Thing':
+            base_types.append((n, v))
+        elif 'Document' in n:
+            document_types.append((n, v))
+        else:
+            annotation_types.append((n, v))
 
     type_lists = {
-        # extract document types (hacky for now, improve later)
-        'document_types': [t for t in clams_types if 'Document' in t],
-
-        # extract annotation types
-        'annotation_types': [t for t in clams_types if 'Document' not in t and t != 'Thing'],
-
-        # extract thing type
-        'base_types': clams_types[:1]
+        'document_types': document_types,
+        'annotation_types': annotation_types,
+        'base_types': base_types
     }
 
-    for mod_name, type_list in type_lists.items():
-        enum_contents = generate_vocab_enum(spec_version, type_list, mod_name)
+    for mod_name, type_ver_list in type_lists.items():
+        enum_contents = generate_vocab_enum(spec_version, type_ver_list, mod_name)
         write_res_file(vocabulary_dir, mod_name+'.py', enum_contents)
 
     return vocabulary_dir
 
 
-def get_matching_gittag(version: str):
-    vmaj, vmin, vpat = version.split('.')[0:3]
+def get_latest_mmif_gittag(version: str):
+    # vmaj, vmin, vpat = version.split('.')[0:3]
     res = request.urlopen('https://api.github.com/repos/clamsproject/mmif/git/refs/tags')
     body = json.loads(res.read())
     tags = [os.path.basename(tag['ref']) for tag in body]
     # sort and return highest version
-    return \
-        sorted([tag for tag in tags if f'{vmaj}.{vmin}.' in tag and 'py-' not in tag],
-               key=lambda x: int(x.split('.')[-1]))[-1]
+    mmif_ver_format = lambda x: re.match(r'\d+\.\d+\.\d$', x)
+    return sorted([tag for tag in tags if mmif_ver_format(tag)])[-1]
 
 
-def get_spec_file_at_tag(tag, filepath: str) -> bytes:
+def get_spec_file_at_gitref(tag, filepath: str) -> bytes:
+    filepath = filepath.format(version=tag)
     if LOCALMMIF is not None:
-        file_path = os.path.join(LOCALMMIF, filepath)
-        spec_file = open(file_path, 'br')
-        contents = spec_file.read()
-        spec_file.close()
-        return contents
+        return subprocess.run(f'git --git-dir {LOCALMMIF}/.git --no-pager show {tag}:{filepath}'.split(), capture_output=True).stdout
     file_url = f"https://raw.githubusercontent.com/clamsproject/mmif/{tag}/{filepath}"
     return request.urlopen(file_url).read()
 
 
 def write_res_file(res_dir: str, res_name: str, res_data: Union[bytes, str]):
     open_ops = 'wb' if type(res_data) == bytes else 'w'
     res_file = open(pjoin(res_dir, res_name), open_ops)
@@ -188,35 +194,54 @@
     raise ValueError(f"Cannot find {version_fname} file. Use `make version` to generate one.")
 
 
 def prep_ext_files(setuptools_cmd):
     ori_run = setuptools_cmd.run
 
     def mod_run(self):
-        # assuming build only happens inside the `mmif` git repository
-        # also, NOTE that when in `make develop`, it will use specification files from upstream "develop" branch of mmif github repository
-        gittag = get_matching_gittag(version) if '.dev' not in version else "develop"
-        spec_version = gittag.split('-')[-1]
+        # will infer the `spec_ver` from the latest git tag available either on GH or local `mmif` repository.
+        # NOTE that when `make develop`, it will use specification files from upstream "develop" branch of `mmif` repo
+        latest_mmif_gittag = get_latest_mmif_gittag(version)
+        spec_file_gitref = latest_mmif_gittag if '.dev' not in version else 'develop'
+        # legacy version tags were formatted as xx-a.b.c (e.g., vocab-0.0.1)
+        spec_version = latest_mmif_gittag.split('-')[-1]
         # making resources into a python package so that `pkg_resources` can access resource files
         res_dir = generate_subpack(mmif_name, mmif_res_pkg)
 
         # the following will generate a new version value based on VERSION file
         generate_subpack(mmif_name, mmif_ver_pkg, f'__version__ = "{version}"\n__specver__ = "{spec_version}"')
         update_target_spec('documentation/target-versions.csv', spec_version)
 
         # and write resource files
-        write_res_file(res_dir, mmif_schema_res_name, get_spec_file_at_tag(gittag, mmif_schema_res_oriname))
-        write_res_file(res_dir, mmif_vocab_res_name, get_spec_file_at_tag(gittag, mmif_vocab_res_oriname))
+        for res_name, res_oriname in [(mmif_schema_res_name, mmif_schema_res_oriname), (mmif_vocab_res_name, mmif_vocab_res_oriname)]:
+            if LOCALMMIF:
+                res_content = open(pjoin(LOCALMMIF, res_oriname)).read()
+            else:
+                res_content = get_spec_file_at_gitref(spec_file_gitref, res_oriname)
+            write_res_file(res_dir, res_name, res_content)
 
         # write vocabulary enum
         import yaml
-        yaml_file = io.BytesIO(get_spec_file_at_tag(gittag, mmif_vocab_res_oriname))
-        clams_types = [t['name'] for t in list(yaml.safe_load_all(yaml_file.read()))]
-        generate_vocabulary(spec_version, clams_types)
-
+        attypevers = json.load(io.BytesIO(get_spec_file_at_gitref(latest_mmif_gittag, mmif_vocab_attypevers_res_oriname)))
+        if '.dev' not in version:
+            vocab_yaml_file = io.BytesIO(get_spec_file_at_gitref(latest_mmif_gittag, mmif_vocab_res_oriname))
+            clams_types_vers = {t['name']: attypevers[t['name']] for t in list(yaml.safe_load_all(vocab_yaml_file.read()))}
+        else:
+            last_clams_types = {t['name']: t for t in yaml.safe_load_all(get_spec_file_at_gitref(latest_mmif_gittag, mmif_vocab_res_oriname))}
+            if LOCALMMIF:
+                new_clams_types = {t['name']: t for t in yaml.safe_load_all(open(pjoin(LOCALMMIF, mmif_vocab_res_oriname)))}
+            else:
+                new_clams_types = {t['name']: t for t in yaml.safe_load_all(get_spec_file_at_gitref(spec_file_gitref, mmif_vocab_res_oriname))}
+            clams_types_vers = {n: attypevers[n] for n, t in last_clams_types.items()}
+            for tname in new_clams_types:
+                if tname not in last_clams_types:
+                    clams_types_vers[tname] = 'v1'
+                elif last_clams_types[tname] != new_clams_types[tname]:
+                    clams_types_vers[tname] = f'v{int(clams_types_vers[tname][1:])+1}'
+        generate_vocabulary(spec_version, clams_types_vers)
         ori_run(self)
 
     setuptools_cmd.run = mod_run
     return setuptools_cmd
 
 
 @prep_ext_files
```

