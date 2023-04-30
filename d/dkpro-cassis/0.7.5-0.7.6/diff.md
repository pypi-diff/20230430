# Comparing `tmp/dkpro-cassis-0.7.5.tar.gz` & `tmp/dkpro-cassis-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkpro-cassis-0.7.5.tar", last modified: Thu Feb  9 10:30:13 2023, max compression
+gzip compressed data, was "dkpro-cassis-0.7.6.tar", last modified: Sun Apr 30 19:58:59 2023, max compression
```

## Comparing `dkpro-cassis-0.7.5.tar` & `dkpro-cassis-0.7.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:30:13.989233 dkpro-cassis-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15773 2023-02-09 10:30:13.989233 dkpro-cassis-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14473 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:30:13.985233 dkpro-cassis-0.7.5/cassis/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/cassis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/cassis/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27448 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/cassis/cas.py
--rw-r--r--   0 runner    (1001) docker     (123)    19686 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/cassis/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:30:13.985233 dkpro-cassis-0.7.5/cassis/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/cassis/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   116666 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/cassis/resources/dkpro-core-types.xml
--rw-r--r--   0 runner    (1001) docker     (123)    59683 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/cassis/typesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/cassis/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    32305 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/cassis/xmi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:30:13.989233 dkpro-cassis-0.7.5/dkpro_cassis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15773 2023-02-09 10:30:13.000000 dkpro-cassis-0.7.5/dkpro_cassis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-09 10:30:13.000000 dkpro-cassis-0.7.5/dkpro_cassis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 10:30:13.000000 dkpro-cassis-0.7.5/dkpro_cassis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-02-09 10:30:13.000000 dkpro-cassis-0.7.5/dkpro_cassis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-09 10:30:13.000000 dkpro-cassis-0.7.5/dkpro_cassis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 10:30:13.989233 dkpro-cassis-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:30:13.989233 dkpro-cassis-0.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/tests/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)    16966 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/tests/test_cas.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/tests/test_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    36005 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/tests/test_typesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17205 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/tests/test_xmi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-02-09 10:29:50.000000 dkpro-cassis-0.7.5/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:58:59.070533 dkpro-cassis-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15773 2023-04-30 19:58:59.070533 dkpro-cassis-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14473 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:58:59.070533 dkpro-cassis-0.7.6/cassis/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/cassis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/cassis/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27448 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/cassis/cas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22723 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/cassis/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:58:59.070533 dkpro-cassis-0.7.6/cassis/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/cassis/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116666 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/cassis/resources/dkpro-core-types.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    61200 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/cassis/typesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/cassis/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32305 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/cassis/xmi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:58:59.070533 dkpro-cassis-0.7.6/dkpro_cassis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15773 2023-04-30 19:58:58.000000 dkpro-cassis-0.7.6/dkpro_cassis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-30 19:58:59.000000 dkpro-cassis-0.7.6/dkpro_cassis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 19:58:58.000000 dkpro-cassis-0.7.6/dkpro_cassis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-30 19:58:58.000000 dkpro-cassis-0.7.6/dkpro_cassis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-30 19:58:58.000000 dkpro-cassis-0.7.6/dkpro_cassis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 19:58:59.070533 dkpro-cassis-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:58:59.070533 dkpro-cassis-0.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/tests/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16966 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/tests/test_cas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/tests/test_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36005 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/tests/test_typesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17205 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/tests/test_xmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-30 19:58:29.000000 dkpro-cassis-0.7.6/tests/util.py
```

### Comparing `dkpro-cassis-0.7.5/LICENSE` & `dkpro-cassis-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dkpro-cassis-0.7.5/PKG-INFO` & `dkpro-cassis-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkpro-cassis
-Version: 0.7.5
+Version: 0.7.6
 Summary: UIMA CAS processing library in Python
 Home-page: https://dkpro.github.io
 Author: The DKPro cassis team
 Author-email: dkpro-core-user@googlegroups.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/dkpro/dkpro-cassis/issues
 Project-URL: Documentation, https://cassis.readthedocs.org/
```

### Comparing `dkpro-cassis-0.7.5/README.rst` & `dkpro-cassis-0.7.6/README.rst`

 * *Files identical despite different names*

### Comparing `dkpro-cassis-0.7.5/cassis/__init__.py` & `dkpro-cassis-0.7.6/cassis/__init__.py`

 * *Files identical despite different names*

### Comparing `dkpro-cassis-0.7.5/cassis/cas.py` & `dkpro-cassis-0.7.6/cassis/cas.py`

 * *Files identical despite different names*

### Comparing `dkpro-cassis-0.7.5/cassis/json.py` & `dkpro-cassis-0.7.6/cassis/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,25 +70,27 @@
         else:
             data = json.load(source)
 
         self._max_xmi_id = 0
         self._max_sofa_num = 0
         self._post_processors = []
 
-        embedded_typesystem = TypeSystem()
         json_typesystem = data.get(TYPES_FIELD)
+        embedded_typesystem = TypeSystem(
+            add_document_annotation_type=not (json_typesystem.get(FLAG_DOCUMENT_ANNOTATION))
+        )
 
         # First, build a dependency graph to support cases where a child type is defined before its super type
         type_dependencies = defaultdict(set)
         for type_name, json_type in json_typesystem.items():
             type_dependencies[type_name].add(json_type[SUPER_TYPE_FIELD])
 
         # Second, load all the types but no features since features of a type X might be of a later loaded type Y
         for type_name in toposort_flatten(type_dependencies):
-            if is_predefined(type_name):
+            if is_predefined(type_name) or embedded_typesystem.contains_type(type_name):
                 continue
 
             self._parse_type(embedded_typesystem, type_name, json_typesystem[type_name])
 
         # Now we are sure we know all the types, we can create the features
         for type_name, json_type in json_typesystem.items():
             self._parse_features(embedded_typesystem, type_name, json_type)
@@ -96,32 +98,56 @@
         typesystem = merge_typesystems(typesystem, embedded_typesystem)
 
         cas = Cas(typesystem=typesystem)
 
         feature_structures = {}
         json_feature_structures = data.get(FEATURE_STRUCTURES_FIELD)
         if isinstance(json_feature_structures, list):
+            def parse_and_add(json_fs_):
+                parsed = self._parse_feature_structure(typesystem, json_fs_.get(ID_FIELD), json_fs_, feature_structures)
+                feature_structures[parsed.xmiID] = parsed
+
+            # According to the JSON CAS 0.4.0 spec, we should be able to do this in a single loop as SofaFSes
+            # should normally appear before any FSes referring to them. However, the Java implementation currently
+            # does not do this, so we do two passes to be able to read its data.
             for json_fs in json_feature_structures:
                 if json_fs.get(TYPE_FIELD) == TYPE_NAME_SOFA:
+                    # In case the Sofa references a byte array that has not been parsed yet, we need to fetch it
+                    sofa_byte_array_ref = json_fs.get(REF_FEATURE_PREFIX + FEATURE_BASE_NAME_SOFAARRAY)
+                    if sofa_byte_array_ref and not feature_structures.get(sofa_byte_array_ref):
+                        for json_fs_2 in json_feature_structures:
+                            if json_fs_2.get(ID_FIELD) == sofa_byte_array_ref:
+                                parse_and_add(json_fs_2)
                     fs_id = json_fs.get(ID_FIELD)
                     fs = self._parse_sofa(cas, fs_id, json_fs, feature_structures)
-                else:
-                    fs_id = json_fs.get(ID_FIELD)
-                    fs = self._parse_feature_structure(typesystem, fs_id, json_fs, feature_structures)
-                feature_structures[fs.xmiID] = fs
+                    feature_structures[fs.xmiID] = fs
+            for json_fs in json_feature_structures:
+                if json_fs.get(TYPE_FIELD) != TYPE_NAME_SOFA:
+                    parse_and_add(json_fs)
 
         if isinstance(json_feature_structures, dict):
+            def parse_and_add(fs_id_, json_fs_):
+                parsed = self._parse_feature_structure(typesystem, int(fs_id_), json_fs_, feature_structures)
+                feature_structures[parsed.xmiID] = parsed
+
+            # According to the JSON CAS 0.4.0 spec, we should be able to do this in a single loop as SofaFSes
+            # should normally appear before any FSes referring to them. However, the Java implementation currently
+            # does not do this, so we do two passes to be able to read its data.
             for fs_id, json_fs in json_feature_structures.items():
                 if json_fs.get(TYPE_FIELD) == TYPE_NAME_SOFA:
+                    # In case the Sofa references a byte array that has not been parsed yet, we need to fetch it
+                    sofa_byte_array_ref = json_fs.get(REF_FEATURE_PREFIX + FEATURE_BASE_NAME_SOFAARRAY)
+                    if sofa_byte_array_ref and not feature_structures.get(sofa_byte_array_ref):
+                        parse_and_add(sofa_byte_array_ref, json_feature_structures.get(sofa_byte_array_ref))
                     fs_id = int(fs_id)
                     fs = self._parse_sofa(cas, fs_id, json_fs, feature_structures)
-                else:
-                    fs_id = int(fs_id)
-                    fs = self._parse_feature_structure(typesystem, fs_id, json_fs, feature_structures)
-                feature_structures[fs.xmiID] = fs
+                    feature_structures[fs.xmiID] = fs
+            for fs_id, json_fs in json_feature_structures.items():
+                if json_fs.get(TYPE_FIELD) != TYPE_NAME_SOFA:
+                    parse_and_add(fs_id, json_fs)
 
         for post_processor in self._post_processors:
             post_processor()
 
         cas._xmi_id_generator = IdGenerator(self._max_xmi_id + 1)
         cas._sofa_num_generator = IdGenerator(self._max_sofa_num + 1)
 
@@ -140,20 +166,26 @@
         typesystem.create_type(type_name, super_type_name, description=description)
 
     def _parse_features(self, typesystem: TypeSystem, type_name: str, json_type: Dict[str, any]):
         new_type = typesystem.get_type(type_name)
         for key, json_feature in json_type.items():
             if key.startswith(RESERVED_FIELD_PREFIX):
                 continue
+
+            range_type = json_feature[RANGE_FIELD]
+            element_type = json_feature.get(ELEMENT_TYPE_FIELD)
+            if range_type.endswith('[]'):
+                element_type = range_type[:-2]
+                range_type = array_type_name_for_type(element_type)
             typesystem.create_feature(
                 new_type,
                 name=key,
-                rangeType=json_feature[RANGE_FIELD],
+                rangeType=range_type,
+                elementType=element_type,
                 description=json_feature.get(DESCRIPTION_FIELD),
-                elementType=json_feature.get(ELEMENT_TYPE_FIELD),
                 multipleReferencesAllowed=json_feature.get(MULTIPLE_REFERENCES_ALLOWED_FIELD),
             )
 
     def _get_or_create_view(
         self, cas: Cas, view_name: str, fs_id: Optional[int] = None, sofa_num: Optional[int] = None
     ) -> Cas:
         if view_name == NAME_DEFAULT_SOFA:
@@ -184,15 +216,18 @@
         view.sofa_array = feature_structures.get(json_fs.get(REF_FEATURE_PREFIX + FEATURE_BASE_NAME_SOFAARRAY))
 
         return view.get_sofa()
 
     def _parse_feature_structure(
         self, typesystem: TypeSystem, fs_id: int, json_fs: Dict[str, any], feature_structures: Dict[int, any]
     ):
-        AnnotationType = typesystem.get_type(json_fs.get(TYPE_FIELD))
+        type_name = json_fs.get(TYPE_FIELD)
+        if type_name.endswith('[]'):
+            type_name = array_type_name_for_type(type_name)
+        AnnotationType = typesystem.get_type(type_name)
 
         attributes = dict(json_fs)
 
         # Map the JSON FS ID to xmiID
         attributes["xmiID"] = fs_id
 
         # Remap features that use a reserved Python name
@@ -383,26 +418,37 @@
     def _serialize_feature(self, json_type, feature: Feature):
         # If the feature name is a reserved name like `self`, then we added an
         # underscore to it before so Python can handle it. We now need to remove it.
         feature_name = feature.name
         if feature._has_reserved_name:
             feature_name = feature_name[:-1]
 
+        range_type_name = self._to_external_type_name(feature.rangeType.name)
+        skip_element_type = False
+        if is_array(feature.rangeType):
+            skip_element_type = True
+            if is_primitive_array(feature.rangeType):
+                range_type_name = element_type_name_for_array_type(feature.rangeType) + "[]"
+            elif feature.elementType:
+                range_type_name = self._to_external_type_name(feature.elementType.name) + "[]"
+            else:
+                range_type_name = TYPE_NAME_TOP + "[]"
+
         json_feature = {
             NAME_FIELD: feature_name,
-            RANGE_FIELD: self._to_external_type_name(feature.rangeType.name),
+            RANGE_FIELD: range_type_name,
         }
 
         if feature.description:
             json_feature[DESCRIPTION_FIELD] = feature.description
 
         if feature.multipleReferencesAllowed is not None:
             json_feature[MULTIPLE_REFERENCES_ALLOWED_FIELD] = feature.multipleReferencesAllowed
 
-        if feature.elementType is not None:
+        if not skip_element_type and feature.elementType is not None:
             json_feature[ELEMENT_TYPE_FIELD] = self._to_external_type_name(feature.elementType.name)
 
         return json_feature
 
     def _serialize_feature_structure(self, fs) -> dict:
         type_name = fs.type.name
```

### Comparing `dkpro-cassis-0.7.5/cassis/resources/dkpro-core-types.xml` & `dkpro-cassis-0.7.6/cassis/resources/dkpro-core-types.xml`

 * *Files identical despite different names*

### Comparing `dkpro-cassis-0.7.5/cassis/typesystem.py` & `dkpro-cassis-0.7.6/cassis/typesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,54 @@
 class TypeSystemMode(Enum):
     """How much type system information to include."""
 
     FULL = auto()
     MINIMAL = auto()
     NONE = auto()
 
+def array_type_name_for_type(type_: Union[str, "Type"]) -> str:
+    type_name = type_ if isinstance(type_, str) else type_.name
+    if type_name == TYPE_NAME_BYTE:
+        return TYPE_NAME_BYTE_ARRAY
+    if type_name == TYPE_NAME_FLOAT:
+        return TYPE_NAME_FLOAT_ARRAY
+    if type_name == TYPE_NAME_DOUBLE:
+        return TYPE_NAME_DOUBLE_ARRAY
+    if type_name == TYPE_NAME_BOOLEAN:
+        return TYPE_NAME_BOOLEAN_ARRAY
+    if type_name == TYPE_NAME_INTEGER:
+        return TYPE_NAME_INTEGER_ARRAY
+    if type_name == TYPE_NAME_SHORT:
+        return TYPE_NAME_SHORT_ARRAY
+    if type_name == TYPE_NAME_LONG:
+        return TYPE_NAME_LONG_ARRAY
+    if type_name == TYPE_NAME_STRING:
+        return TYPE_NAME_STRING_ARRAY
+    return TYPE_NAME_FS_ARRAY
+
 
+def element_type_name_for_array_type(type_: Union[str, "Type"]) -> str:
+    type_name = type_ if isinstance(type_, str) else type_.name
+    if type_name == TYPE_NAME_BYTE_ARRAY:
+        return TYPE_NAME_BYTE
+    if type_name == TYPE_NAME_FLOAT_ARRAY:
+        return TYPE_NAME_FLOAT
+    if type_name == TYPE_NAME_DOUBLE_ARRAY:
+        return TYPE_NAME_DOUBLE
+    if type_name == TYPE_NAME_BOOLEAN_ARRAY:
+        return TYPE_NAME_BOOLEAN
+    if type_name == TYPE_NAME_INTEGER_ARRAY:
+        return TYPE_NAME_INTEGER
+    if type_name == TYPE_NAME_SHORT_ARRAY:
+        return TYPE_NAME_SHORT
+    if type_name == TYPE_NAME_LONG_ARRAY:
+        return TYPE_NAME_LONG
+    if type_name == TYPE_NAME_STRING_ARRAY:
+        return TYPE_NAME_STRING
+    return TYPE_NAME_TOP
 def _string_to_valid_classname(name: str):
     return re.sub("[^a-zA-Z0-9_]", "_", name)
 
 
 def is_predefined(type_: Union[str, "Type"]) -> bool:
     """Checks if the given type  is predefined by UIMA and by default in a new type system.
 
@@ -1098,16 +1137,16 @@
 
         return errors
 
     def _defines_predefined_type(self, type_name):
         self._predefined_types.add(type_name)
 
     def _add_document_annotation_type(self):
-        t = self.create_type(name=_DOCUMENT_ANNOTATION_TYPE, supertypeName="uima.tcas.Annotation")
-        self.create_feature(t, name="language", rangeType="uima.cas.String")
+        t = self.create_type(name=_DOCUMENT_ANNOTATION_TYPE, supertypeName=TYPE_NAME_ANNOTATION)
+        self.create_feature(t, name="language", rangeType=TYPE_NAME_STRING)
 
     def transitive_closure(self, seed_types: Set[Type], built_in: bool = False) -> Set[Type]:
         # Build transitive closure of used types by following parents, features, etc.
         transitively_referenced_types = set()
         openlist = []
         openlist.extend(seed_types)
         while openlist:
```

### Comparing `dkpro-cassis-0.7.5/cassis/util.py` & `dkpro-cassis-0.7.6/cassis/util.py`

 * *Files identical despite different names*

### Comparing `dkpro-cassis-0.7.5/cassis/xmi.py` & `dkpro-cassis-0.7.6/cassis/xmi.py`

 * *Files identical despite different names*

### Comparing `dkpro-cassis-0.7.5/dkpro_cassis.egg-info/PKG-INFO` & `dkpro-cassis-0.7.6/dkpro_cassis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkpro-cassis
-Version: 0.7.5
+Version: 0.7.6
 Summary: UIMA CAS processing library in Python
 Home-page: https://dkpro.github.io
 Author: The DKPro cassis team
 Author-email: dkpro-core-user@googlegroups.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/dkpro/dkpro-cassis/issues
 Project-URL: Documentation, https://cassis.readthedocs.org/
```

### Comparing `dkpro-cassis-0.7.5/dkpro_cassis.egg-info/SOURCES.txt` & `dkpro-cassis-0.7.6/dkpro_cassis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkpro-cassis-0.7.5/setup.py` & `dkpro-cassis-0.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `dkpro-cassis-0.7.5/tests/fixtures.py` & `dkpro-cassis-0.7.6/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `dkpro-cassis-0.7.5/tests/performance.py` & `dkpro-cassis-0.7.6/tests/performance.py`

 * *Files identical despite different names*

### Comparing `dkpro-cassis-0.7.5/tests/test_cas.py` & `dkpro-cassis-0.7.6/tests/test_cas.py`

 * *Files identical despite different names*

### Comparing `dkpro-cassis-0.7.5/tests/test_json.py` & `dkpro-cassis-0.7.6/tests/test_json.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from cassis.typesystem import TYPE_NAME_ANNOTATION, TypeSystemMode
 from tests.fixtures import *
 from tests.test_files.test_cas_generators import MultiFeatureRandomCasGenerator, MultiTypeRandomCasGenerator
 from tests.util import assert_json_equal
 
 FIXTURE_DIR = os.path.join(os.path.dirname(os.path.realpath(__file__)), "test_files", "json")
 SER_REF_DIR = os.path.join(FIXTURE_DIR, "fs_as_array", "ser-ref")
+ONE_WAY_DIR = os.path.join(FIXTURE_DIR, "fs_as_array", "one-way")
 
-FIXTURES = [
+ROUND_TRIP_FIXTURES = [
     (os.path.join(SER_REF_DIR, "casWithSofaDataArray"), []),
     (os.path.join(SER_REF_DIR, "casWithSofaDataURI"), []),
     (os.path.join(SER_REF_DIR, "casWithFloatingPointSpecialValues"), []),
     (os.path.join(SER_REF_DIR, "casWithText"), [["uima.tcas.DocumentAnnotation", 0, 15, "This is a test."]]),
     (
         os.path.join(SER_REF_DIR, "casWithoutTextButWithAnnotations"),
         [
@@ -73,30 +74,57 @@
             ["uima.tcas.Annotation", 0, 1, "這"],
             ["uima.tcas.Annotation", 1, 2, "是"],
             ["uima.tcas.Annotation", 2, 4, "一個"],
             ["uima.tcas.Annotation", 4, 6, "測試"],
             ["uima.tcas.DocumentAnnotation", 0, 6, "這是一個測試"],
         ],
     ),
+    (
+        os.path.join(SER_REF_DIR, "casExtendingDocumentAnnotation"),
+        [["de.tudarmstadt.ukp.dkpro.core.api.metadata.type.DocumentMetaData", 0, 16, "This is a test ."]],
+    ),
 ]
 
+ONE_WAY_FIXTURES = [
+    (
+        os.path.join(ONE_WAY_DIR, "casWithBadSofaFsOrder"),
+        [["de.tudarmstadt.ukp.dkpro.core.api.metadata.type.DocumentMetaData", 0, 16, "This is a test ."]],
+    ),
+    (
+        os.path.join(ONE_WAY_DIR, "tsv3-testSimpleSlotFeature"),
+        [],
+    )
+]
 
-@pytest.mark.parametrize("json_path, annotations", FIXTURES)
+@pytest.mark.parametrize("json_path, annotations", ROUND_TRIP_FIXTURES)
 def test_deserialization_serialization(json_path, annotations):
     with open(os.path.join(json_path, "data.json"), "rb") as f:
         cas = load_cas_from_json(f)
 
     with open(os.path.join(json_path, "data.json"), "rb") as f:
         expected_json = json.load(f)
 
     actual_json = cas.to_json(pretty_print=True)
 
     assert_json_equal(actual_json, expected_json, sort_keys=True)
 
 
+@pytest.mark.parametrize("json_path, annotations", ONE_WAY_FIXTURES)
+def test_deserialization_serialization_one_way(json_path, annotations):
+    with open(os.path.join(json_path, "data.json"), "rb") as f:
+        cas = load_cas_from_json(f)
+
+    with open(os.path.join(json_path, "data-ref.json"), "rb") as f:
+        expected_json = json.load(f)
+
+    actual_json = cas.to_json(pretty_print=True)
+
+    assert_json_equal(actual_json, expected_json, sort_keys=True)
+
+
 def test_multi_type_random_serialization_deserialization():
     generator = MultiTypeRandomCasGenerator()
     for i in range(0, 10):
         generator.size = (i + 1) * 10
         generator.type_count = i + 1
         typesystem = generator.generate_type_system()
         randomized_cas = generator.generate_cas(typesystem)
@@ -120,15 +148,15 @@
 
         loaded_cas = load_cas_from_json(expected_json)
         actual_json = loaded_cas.to_json()
 
         assert_json_equal(actual_json, expected_json)
 
 
-@pytest.mark.parametrize("json_path, annotations", FIXTURES)
+@pytest.mark.parametrize("json_path, annotations", ROUND_TRIP_FIXTURES)
 def test_unicode(json_path, annotations):
     with open(os.path.join(json_path, "data.json"), "rb") as f:
         cas = load_cas_from_json(f)
 
     actual_annotations = [
         [a.type.name, a.begin, a.end, a.get_covered_text()]
         for a in sorted(cas.select(TYPE_NAME_ANNOTATION), key=lambda k: k.type.name)
```

### Comparing `dkpro-cassis-0.7.5/tests/test_typesystem.py` & `dkpro-cassis-0.7.6/tests/test_typesystem.py`

 * *Files identical despite different names*

### Comparing `dkpro-cassis-0.7.5/tests/test_util.py` & `dkpro-cassis-0.7.6/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dkpro-cassis-0.7.5/tests/test_xmi.py` & `dkpro-cassis-0.7.6/tests/test_xmi.py`

 * *Files identical despite different names*

### Comparing `dkpro-cassis-0.7.5/tests/util.py` & `dkpro-cassis-0.7.6/tests/util.py`

 * *Files identical despite different names*

