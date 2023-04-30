# Comparing `tmp/python-materialsdb-0.0.1.tar.gz` & `tmp/python-materialsdb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-materialsdb-0.0.1.tar", last modified: Sat Jun 19 13:39:49 2021, max compression
+gzip compressed data, was "python-materialsdb-0.0.2.tar", last modified: Sun Apr 30 12:09:38 2023, max compression
```

## Comparing `python-materialsdb-0.0.1.tar` & `python-materialsdb-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 cyril     (1000) cyril     (1000)        0 2021-06-19 13:39:49.087431 python-materialsdb-0.0.1/
--rw-r--r--   0 cyril     (1000) cyril     (1000)    34916 2020-10-21 16:46:35.000000 python-materialsdb-0.0.1/LICENSE.md
--rw-r--r--   0 cyril     (1000) cyril     (1000)     2500 2021-06-19 13:39:49.087431 python-materialsdb-0.0.1/PKG-INFO
--rw-r--r--   0 cyril     (1000) cyril     (1000)     1632 2021-06-19 13:37:08.000000 python-materialsdb-0.0.1/README.md
--rw-r--r--   0 cyril     (1000) cyril     (1000)      159 2021-06-06 19:44:30.000000 python-materialsdb-0.0.1/pyproject.toml
--rw-r--r--   0 cyril     (1000) cyril     (1000)     1062 2021-06-19 13:39:49.087431 python-materialsdb-0.0.1/setup.cfg
-drwxr-xr-x   0 cyril     (1000) cyril     (1000)        0 2021-06-19 13:39:49.084097 python-materialsdb-0.0.1/src/
-drwxr-xr-x   0 cyril     (1000) cyril     (1000)        0 2021-06-19 13:39:49.087431 python-materialsdb-0.0.1/src/materialsdb/
--rw-r--r--   0 cyril     (1000) cyril     (1000)       63 2021-06-06 19:00:01.000000 python-materialsdb-0.0.1/src/materialsdb/__init__.py
--rw-r--r--   0 cyril     (1000) cyril     (1000)     2577 2021-06-09 22:19:56.000000 python-materialsdb-0.0.1/src/materialsdb/cache.py
--rw-r--r--   0 cyril     (1000) cyril     (1000)    21194 2021-06-19 08:20:23.000000 python-materialsdb-0.0.1/src/materialsdb/classes.py
--rw-r--r--   0 cyril     (1000) cyril     (1000)     1331 2021-06-05 20:42:43.000000 python-materialsdb-0.0.1/src/materialsdb/config.py
-drwxr-xr-x   0 cyril     (1000) cyril     (1000)        0 2021-06-19 13:39:49.087431 python-materialsdb-0.0.1/src/materialsdb/ifc/
--rw-r--r--   0 cyril     (1000) cyril     (1000)        0 2021-06-06 17:23:03.000000 python-materialsdb-0.0.1/src/materialsdb/ifc/__init__.py
--rw-r--r--   0 cyril     (1000) cyril     (1000)    13782 2021-06-19 09:22:39.000000 python-materialsdb-0.0.1/src/materialsdb/ifc/project_library.py
--rw-r--r--   0 cyril     (1000) cyril     (1000)     5860 2021-06-09 21:54:57.000000 python-materialsdb-0.0.1/src/materialsdb/serialiser.py
--rw-r--r--   0 cyril     (1000) cyril     (1000)      703 2021-06-10 09:26:52.000000 python-materialsdb-0.0.1/src/materialsdb/utils.py
-drwxr-xr-x   0 cyril     (1000) cyril     (1000)        0 2021-06-19 13:39:49.087431 python-materialsdb-0.0.1/src/python_materialsdb.egg-info/
--rw-r--r--   0 cyril     (1000) cyril     (1000)     2500 2021-06-19 13:39:49.000000 python-materialsdb-0.0.1/src/python_materialsdb.egg-info/PKG-INFO
--rw-r--r--   0 cyril     (1000) cyril     (1000)      506 2021-06-19 13:39:49.000000 python-materialsdb-0.0.1/src/python_materialsdb.egg-info/SOURCES.txt
--rw-r--r--   0 cyril     (1000) cyril     (1000)        1 2021-06-19 13:39:49.000000 python-materialsdb-0.0.1/src/python_materialsdb.egg-info/dependency_links.txt
--rw-r--r--   0 cyril     (1000) cyril     (1000)       25 2021-06-19 13:39:49.000000 python-materialsdb-0.0.1/src/python_materialsdb.egg-info/requires.txt
--rw-r--r--   0 cyril     (1000) cyril     (1000)       12 2021-06-19 13:39:49.000000 python-materialsdb-0.0.1/src/python_materialsdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:09:38.819990 python-materialsdb-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-04-30 12:09:27.000000 python-materialsdb-0.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-30 12:09:38.819990 python-materialsdb-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-30 12:09:27.000000 python-materialsdb-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 12:09:27.000000 python-materialsdb-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-30 12:09:38.819990 python-materialsdb-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:09:38.815990 python-materialsdb-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:09:38.819990 python-materialsdb-0.0.2/src/materialsdb/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-30 12:09:27.000000 python-materialsdb-0.0.2/src/materialsdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-30 12:09:27.000000 python-materialsdb-0.0.2/src/materialsdb/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21194 2023-04-30 12:09:27.000000 python-materialsdb-0.0.2/src/materialsdb/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-30 12:09:27.000000 python-materialsdb-0.0.2/src/materialsdb/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:09:38.819990 python-materialsdb-0.0.2/src/materialsdb/ifc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 12:09:27.000000 python-materialsdb-0.0.2/src/materialsdb/ifc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-04-30 12:09:27.000000 python-materialsdb-0.0.2/src/materialsdb/ifc/material_psets.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-04-30 12:09:27.000000 python-materialsdb-0.0.2/src/materialsdb/ifc/project_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-04-30 12:09:27.000000 python-materialsdb-0.0.2/src/materialsdb/serialiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-30 12:09:27.000000 python-materialsdb-0.0.2/src/materialsdb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:09:38.819990 python-materialsdb-0.0.2/src/python_materialsdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-30 12:09:38.000000 python-materialsdb-0.0.2/src/python_materialsdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-30 12:09:38.000000 python-materialsdb-0.0.2/src/python_materialsdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:09:38.000000 python-materialsdb-0.0.2/src/python_materialsdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-30 12:09:38.000000 python-materialsdb-0.0.2/src/python_materialsdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-30 12:09:38.000000 python-materialsdb-0.0.2/src/python_materialsdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:09:38.819990 python-materialsdb-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-30 12:09:27.000000 python-materialsdb-0.0.2/tests/test_project_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-30 12:09:27.000000 python-materialsdb-0.0.2/tests/test_serialiser.py
```

### Comparing `python-materialsdb-0.0.1/LICENSE.md` & `python-materialsdb-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python-materialsdb-0.0.1/PKG-INFO` & `python-materialsdb-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: python-materialsdb
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library to work with materialsdb.org open standard for building materials.
 Home-page: https://github.com/CyrilWaechter/python-materialsdb
 Author: Cyril Waechter
 Author-email: cyrwae@hotmail.com
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/CyrilWaechter/python-materialsdb/issues
 Project-URL: Community, https://community.osarch.org/
 Keywords: materials,BIM,ifcopenshell,IFC
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 Provides-Extra: ifc
@@ -61,8 +60,7 @@
 
 # Third parties :
 * [materialsdb.org][1] (GPL) : materials schema
 
 [1]: http://www.materialsdb.org
 [2]: https://lxml.de
 [3]: ifcopenshell.org
-
```

### Comparing `python-materialsdb-0.0.1/README.md` & `python-materialsdb-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `python-materialsdb-0.0.1/setup.cfg` & `python-materialsdb-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-materialsdb
-version = 0.0.1
+version = 0.0.2
 author = Cyril Waechter
 author_email = cyrwae@hotmail.com
 description = A library to work with materialsdb.org open standard for building materials.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GPLv3+
 keywords = materials, BIM, ifcopenshell, IFC
```

### Comparing `python-materialsdb-0.0.1/src/materialsdb/cache.py` & `python-materialsdb-0.0.2/src/materialsdb/cache.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import os
 import pathlib
 import urllib.request
+from collections import namedtuple
 from typing import Optional
 from lxml import etree
 
-MATERIALSDBINDEXURL = "http://www.materialsdb.org/download/ProducerIndex.xml"
+MATERIALSDBINDEXURLLIST = [
+    "http://www.materialsdb.org/download/ProducerIndex.xml",
+    "http://www.materialsdb.org/download/generic/GenericIndex.xml",
+]
 
 
 def get_cache_folder():
     cache_dir = pathlib.Path(
         os.environ.get("APPDATA")
         or os.environ.get("XDG_CACHE_HOME")
         or pathlib.Path.home() / ".cache"
     ).joinpath(
         "materialsdb",
     )
     pathlib.Path(cache_dir).mkdir(parents=True, exist_ok=True)
     return cache_dir
 
 
-def get_cached_index_path() -> pathlib.Path:
-    return get_cache_folder() / "ProducerIndex.xml"
+def get_cached_index_path(index) -> pathlib.Path:
+    return get_cache_folder() / pathlib.Path(index).name
 
 
-def parse_cached_index() -> etree._ElementTree:
-    path = get_cached_index_path()
+def parse_cached_index(index) -> etree._ElementTree:
+    path = get_cached_index_path(index)
     if path.exists():
         return etree.parse(str(path))
     root = etree.Element("root")
     return etree.ElementTree(root)
 
 
 def get_by_id(root: etree._Element, id: str) -> Optional[etree._Element]:
@@ -49,35 +53,55 @@
 
 def get_producers_dir() -> pathlib.Path:
     producer_path = get_cache_folder().joinpath("Producers")
     pathlib.Path(producer_path).mkdir(parents=True, exist_ok=True)
     return producer_path
 
 
-def update_producers_data():
-    cached_index = parse_cached_index()
+Report = namedtuple("Report", ["existing", "updated", "deleted"])
+
+
+def update_producers_data(url_list=MATERIALSDBINDEXURLLIST):
+    existing = []
+    updated = []
+    deleted = []
+    for index in url_list:
+        report = update_producers_from_index(index)
+        existing.extend(report.existing)
+        updated.extend(report.updated)
+        deleted.extend(report.deleted)
+    return Report(existing, updated, deleted)
+
+
+def update_producers_from_index(index):
+    cached_index = parse_cached_index(index)
     cached_root = cached_index.getroot()
-    new_index = etree.parse(MATERIALSDBINDEXURL)
+    new_index = etree.parse(index)
     new_root = new_index.getroot()
     producers_dir = get_producers_dir()
     has_index_update = False
+    existing = []
+    updated = []
+    deleted = []
     for company in new_root:
-        cached_company = get_by_id(cached_root, company.get("id"))
-        if (
-            not require_update(cached_company, company)
-            and (producers_dir / pathlib.Path(company.get("href")).name).exists()
-        ):
+        cached_producer = get_by_id(cached_root, company.get("id"))
+        producer_path = producers_dir / pathlib.Path(company.get("href")).name
+        if not require_update(cached_producer, company) and producer_path.exists():
+            existing.append(producer_path)
             continue
-        if cached_company:
-            (producers_dir / pathlib.Path(cached_company.get("href")).name).unlink(True)
+        if cached_producer:
+            cached_path = producers_dir / pathlib.Path(cached_producer.get("href")).name
+            deleted.append(cached_path)
+            cached_path.unlink(True)
         has_index_update = True
-        producer_path = producers_dir / pathlib.Path(company.get("href")).name
         urllib.request.urlretrieve(company.get("href"), producer_path)
+        updated.append(producer_path)
     if has_index_update:
-        new_index.write(str(get_cached_index_path()))
+        new_index.write(str(get_cached_index_path(index)))
+    return Report(existing, updated, deleted)
 
 
 def producers():
     for producer in get_producers_dir().iterdir():
         if producer.suffix.lower() == ".xml":
             yield producer
```

### Comparing `python-materialsdb-0.0.1/src/materialsdb/classes.py` & `python-materialsdb-0.0.2/src/materialsdb/classes.py`

 * *Files identical despite different names*

### Comparing `python-materialsdb-0.0.1/src/materialsdb/config.py` & `python-materialsdb-0.0.2/src/materialsdb/config.py`

 * *Files identical despite different names*

### Comparing `python-materialsdb-0.0.1/src/materialsdb/ifc/project_library.py` & `python-materialsdb-0.0.2/src/materialsdb/ifc/project_library.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,22 +2,18 @@
 import datetime
 import json
 from pathlib import Path
 import ifcopenshell
 import ifcopenshell.api
 
 from materialsdb.serialiser import XmlDeserialiser
-from materialsdb import config
+from materialsdb import config, utils
 from materialsdb.classes import (
     Materials,
     Material,
-    TLocalizedString,
-    Webinfo,
-    ISO639_1,
-    Mimetype,
 )
 
 CATEGORIES = {
     "Others": {"hatch": "", "color": (255, 255, 255)},
     "Water_Proof": {"hatch": "", "color": (255, 255, 255)},
     "Vapour_Proof": {"hatch": "", "color": (0, 0, 0)},
     "Concrete": {"hatch": "", "color": (0, 255, 0)},
@@ -49,41 +45,20 @@
     return new_dict
 
 
 PSETS = json.loads(Path(__file__).with_name("material_psets.json").read_text("utf-8"))
 PSETS = clean_psets(PSETS)
 
 
-def date_from_xml(days: float) -> datetime.datetime:
-    """Convert days since 30.12.1899 which is materialsdb xml convention to datetime"""
-    return datetime.datetime(1899, 12, 30) + datetime.timedelta(days=days)
-
-
-def date_to_xml(date: datetime.datetime) -> float:
-    """Convert datetime to days since 30.12.1899 which is materialsdb xml convention
-    >>> datetime.timedelta(days=1).total_seconds()
-    86400.0"""
-    return (date - datetime.datetime(1899, 12, 30)).total_seconds() / 86400
-
-
-def get_by_country(values, country):
-    for value in values:
-        if value.country == country:
-            return value
-    for value in values:
-        if value.country is None:
-            return value
-
-
 def get_value(layer, definition, country=None):
     value = layer
     for attrib in definition["path"]:
         value = getattr(value, attrib)
         if isinstance(value, list):
-            value = get_by_country(value, country)
+            value = utils.get_by_country(value, country)
             if not value:
                 return None
     return value
 
 
 class ProjectLibrary:
     def __init__(self, schema: str = "IFC4"):
@@ -143,15 +118,15 @@
             person, organisation, Roles=[role]
         )
 
         # https://standards.buildingsmart.org/IFC/RELEASE/IFC4/ADD2_TC1/HTML/link/ifcownerhistory.htm
         owner_history = file.createIfcOwnerHistory(
             OwningUser=person_and_organisation,
             OwningApplication=self.application,
-            CreationDate=int(date_from_xml(source.crd).timestamp()),
+            CreationDate=max(int(utils.date_from_xml(source.crd).timestamp()),-2147483648),
         )
         self.owner_history = owner_history
 
         # https://standards.buildingsmart.org/IFC/RELEASE/IFC4/ADD2_TC1/HTML/link/ifcprojectlibrary.htm
         file.createIfcProjectLibrary(
             GlobalId=ifcopenshell.guid.new(),
             OwnerHistory=owner_history,
@@ -160,18 +135,18 @@
             ObjectType="MaterialLibrary",
             LongName=f"{source.company} version {source.ver}",
         )
 
     def create_materials(self, source: Materials):
         file = self.file
         context = file.createIfcRepresentationContext()
-        for material in source.material:
-            name = get_material_name(material, self.lang)
-            description = get_material_description(material, self.lang)
-            webinfo = get_material_webinfo(material, self.lang)
+        for material in utils.get_materials(source, self.country):
+            name = utils.get_material_name(material, self.lang)
+            description = utils.get_material_description(material, self.lang)
+            webinfo = utils.get_material_webinfo(material, self.lang)
             category = material.information.group
             labels = material.information.labels
             color = material.information.color
             brushstyle = material.information.BrushStyle
             surface_style = self.get_surface_style(color, category)
             styled_item = file.createIfcStyledItem(Styles=[surface_style])
             # TODO: hatch_item = file.createIfcFillAreaStyleHatching()
@@ -204,17 +179,17 @@
                         continue
                     pset = file.create_entity(
                         "IfcMaterialProperties",
                         Name=pset_name,
                         Properties=properties,
                         Material=ifc_material,
                     )
-                geometry = get_by_country(layer.geometry, self.country)
+                geometry = utils.get_by_country(layer.geometry, self.country)
                 if getattr(geometry, "thick", None):
-                    element_name = name + f" | {geometry.thick}mm"
+                    element_name = f"{name} | {geometry.thick}mm"
                     ifc_layer = file.create_entity(
                         "IfcMaterialLayer",
                         Material=ifc_material,
                         LayerThickness=geometry.thick / 1000,
                         Name=element_name,
                     )
                     assigned_material = file.create_entity(
@@ -302,40 +277,14 @@
         """Color definition in xml is obscur. We assume that it is a decimal color.
         See: https://stackoverflow.com/a/2262152/4098083"""
         return self.file.createIfcColourRgb(
             Blue=color & 255, Green=(color >> 8) & 255, Red=(color >> 16) & 255
         )
 
 
-def get_material_name(material: Material, lang: str) -> TLocalizedString:
-    name = TLocalizedString("")
-    for name in material.information.names.name:
-        if name.lang == lang:
-            return name
-    return name
-
-
-def get_material_description(material: Material, lang: str) -> TLocalizedString:
-    description = TLocalizedString("")
-    explanations = getattr(material.information, "explanations", None)
-    for description in getattr(explanations, "explanation", ()):
-        if description.lang == lang:
-            return description
-    return description
-
-
-def get_material_webinfo(material: Material, lang: str) -> Webinfo:
-    webinfo = Webinfo(Mimetype(""), "", "", lang=ISO639_1(lang))
-    webinfos = getattr(material.information, "webinfos", None)
-    for webinfo in getattr(webinfos, "webinfo", ()):
-        if webinfo.lang == lang:
-            return webinfo
-    return webinfo
-
-
 def create_project_library_from_xml(xml_path):
     library = ProjectLibrary()
     deserialiser = XmlDeserialiser()
     source = deserialiser.from_xml(str(xml_path))
     library.create_project_library(source)
     library.create_materials(source)
     return library.file
```

### Comparing `python-materialsdb-0.0.1/src/materialsdb/serialiser.py` & `python-materialsdb-0.0.2/src/materialsdb/serialiser.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 
 class XmlDeserialiser:
     def __init__(self):
         self.schema = etree.XMLSchema(file=get_xml_schema())
         self.parser = objectify.makeparser(schema=self.schema)
 
-    def from_xml(self, xml_path: str, assert_schema: bool = False):
+    def from_xml(self, xml_path: str, assert_schema: bool = False) -> classes.Materials:
         if assert_schema:
             tree = objectify.parse(xml_path, self.parser)
         else:
             tree = objectify.parse(xml_path)
         return self.from_element(get_valid_root(tree))
 
     def from_element(self, element=None, base_class=None):
```

### Comparing `python-materialsdb-0.0.1/src/python_materialsdb.egg-info/PKG-INFO` & `python-materialsdb-0.0.2/src/python_materialsdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: python-materialsdb
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library to work with materialsdb.org open standard for building materials.
 Home-page: https://github.com/CyrilWaechter/python-materialsdb
 Author: Cyril Waechter
 Author-email: cyrwae@hotmail.com
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/CyrilWaechter/python-materialsdb/issues
 Project-URL: Community, https://community.osarch.org/
 Keywords: materials,BIM,ifcopenshell,IFC
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 Provides-Extra: ifc
@@ -61,8 +60,7 @@
 
 # Third parties :
 * [materialsdb.org][1] (GPL) : materials schema
 
 [1]: http://www.materialsdb.org
 [2]: https://lxml.de
 [3]: ifcopenshell.org
-
```

