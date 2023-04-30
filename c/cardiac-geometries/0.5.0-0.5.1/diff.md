# Comparing `tmp/cardiac_geometries-0.5.0.tar.gz` & `tmp/cardiac_geometries-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardiac_geometries-0.5.0.tar", last modified: Fri Apr 28 11:20:48 2023, max compression
+gzip compressed data, was "cardiac_geometries-0.5.1.tar", last modified: Sun Apr 30 15:36:18 2023, max compression
```

## Comparing `cardiac_geometries-0.5.0.tar` & `cardiac_geometries-0.5.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:20:48.743077 cardiac_geometries-0.5.0/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1082 2023-04-28 11:20:48.743077 cardiac_geometries-0.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      384 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1599 2023-04-28 11:20:48.743077 cardiac_geometries-0.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:20:48.731077 cardiac_geometries-0.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:20:48.735077 cardiac_geometries-0.5.0/src/cardiac_geometries/
--rw-r--r--   0 root         (0) root         (0)     1512 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:20:48.739076 cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/
--rw-r--r--   0 root         (0) root         (0)      602 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10271 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     9594 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     2357 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/_slab.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/utils.py
--rw-r--r--   0 root         (0) root         (0)      778 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_import_checks.py
--rw-r--r--   0 root         (0) root         (0)    21055 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_mesh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:20:48.739076 cardiac_geometries-0.5.0/src/cardiac_geometries/_mshr/
--rw-r--r--   0 root         (0) root         (0)      260 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_mshr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5721 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_mshr/_biv.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_mshr/_lv.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/_mshr/_utils.py
--rw-r--r--   0 root         (0) root         (0)     4165 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/calculus.py
--rw-r--r--   0 root         (0) root         (0)    19505 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/cli.py
--rw-r--r--   0 root         (0) root         (0)     4615 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/dolfin_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:20:48.739076 cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/
--rw-r--r--   0 root         (0) root         (0)      133 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1248 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/_biv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     5490 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/_lv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     4187 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/_slab.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/_utils.py
--rw-r--r--   0 root         (0) root         (0)    14224 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/geometry.py
--rw-r--r--   0 root         (0) root         (0)      254 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/utils.py
--rw-r--r--   0 root         (0) root         (0)     9972 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/src/cardiac_geometries/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:20:48.735077 cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1082 2023-04-28 11:20:48.000000 cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1361 2023-04-28 11:20:48.000000 cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 11:20:48.000000 cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-04-28 11:20:48.000000 cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 11:20:36.000000 cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      236 2023-04-28 11:20:48.000000 cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-28 11:20:48.000000 cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:20:48.743077 cardiac_geometries-0.5.0/tests/
--rw-r--r--   0 root         (0) root         (0)     1970 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     4372 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/tests/test_geometry.py
--rw-r--r--   0 root         (0) root         (0)     1702 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/tests/test_gmsh.py
--rw-r--r--   0 root         (0) root         (0)      438 2023-04-28 11:20:35.000000 cardiac_geometries-0.5.0/tests/test_mshr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 15:36:18.078199 cardiac_geometries-0.5.1/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-04-30 15:36:18.078199 cardiac_geometries-0.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      384 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-04-30 15:36:18.078199 cardiac_geometries-0.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 15:36:18.070199 cardiac_geometries-0.5.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 15:36:18.074199 cardiac_geometries-0.5.1/src/cardiac_geometries/
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 15:36:18.074199 cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/
+-rw-r--r--   0 root         (0) root         (0)      602 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12783 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     9594 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     2357 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/_slab.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/utils.py
+-rw-r--r--   0 root         (0) root         (0)      778 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_import_checks.py
+-rw-r--r--   0 root         (0) root         (0)    21343 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_mesh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 15:36:18.078199 cardiac_geometries-0.5.1/src/cardiac_geometries/_mshr/
+-rw-r--r--   0 root         (0) root         (0)      260 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_mshr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5721 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_mshr/_biv.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_mshr/_lv.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_mshr/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/calculus.py
+-rw-r--r--   0 root         (0) root         (0)    19764 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/cli.py
+-rw-r--r--   0 root         (0) root         (0)     4615 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/dolfin_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 15:36:18.078199 cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/_biv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     5490 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/_lv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     4187 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/_slab.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/_utils.py
+-rw-r--r--   0 root         (0) root         (0)    14224 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/geometry.py
+-rw-r--r--   0 root         (0) root         (0)      254 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9972 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 15:36:18.074199 cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-04-30 15:36:18.000000 cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-04-30 15:36:18.000000 cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 15:36:18.000000 cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-04-30 15:36:18.000000 cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 15:36:05.000000 cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      236 2023-04-30 15:36:18.000000 cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-30 15:36:18.000000 cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 15:36:18.078199 cardiac_geometries-0.5.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     4372 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/tests/test_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/tests/test_gmsh.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/tests/test_mshr.py
```

### Comparing `cardiac_geometries-0.5.0/LICENSE` & `cardiac_geometries-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/PKG-INFO` & `cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cardiac_geometries
-Version: 0.5.0
+Name: cardiac-geometries
+Version: 0.5.1
 Summary: A python library for cardiac geometries
 Home-page: https://github.com/ComputationalPhysiology/cardiac_geometries
 Author: Henrik Finsberg
 Author-email: henriknf@simula.no
 License: MIT
 Keywords: cardiac,geometry,mesh,gmsh
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cardiac_geometries-0.5.0/setup.cfg` & `cardiac_geometries-0.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cardiac_geometries
-version = 0.5.0
+version = 0.5.1
 description = A python library for cardiac geometries
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ComputationalPhysiology/cardiac_geometries
 author = Henrik Finsberg
 author_email = henriknf@simula.no
 license = MIT
```

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries/__init__.py` & `cardiac_geometries-0.5.1/src/cardiac_geometries/__init__.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/__init__.py` & `cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/__init__.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py` & `cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py`

 * *Files 18% similar despite different names*

```diff
@@ -148,14 +148,15 @@
     gmsh.finalize()
 
     return path
 
 
 def biv_ellipsoid_torso(
     mesh_name: str = "",
+    heart_as_surface: bool = False,
     torso_length: float = 20.0,
     torso_width: float = 20.0,
     torso_height: float = 20.0,
     rotation_angle: float = math.pi / 6,
     center_lv=(0.0, 0.0, 0.0),
     radius_lv=1.0,
     radius_lv_endo=1.0,
@@ -250,20 +251,36 @@
         3,
     )
 
     # Rotate torso around this point to align with realistic heart in torso
     gmsh.model.occ.rotate([(3, torso_tag)], 0, 0, 0, 0, 0, 1, -rotation_angle)
     gmsh.model.occ.rotate([(3, torso_tag)], 0, 0, 0, 0, 1, 0, rotation_angle)
 
-    # Now we mark the different surfaces
+    if heart_as_surface:
+        mark_heart_as_surface(ov2, torso_tag)
+    else:
+        mark_heart_as_volume(ov2, torso_tag)
+
+    # gmsh.option.setNumber("Mesh.SaveAll", 1)
+    gmsh.option.setNumber("Mesh.CharacteristicLengthMin", char_length)
+    gmsh.option.setNumber("Mesh.CharacteristicLengthMax", char_length)
+
+    gmsh.model.mesh.generate(3)
+    gmsh.model.mesh.optimize("Netgen")
+
+    gmsh.write(path.as_posix())
+    gmsh.finalize()
+
+    return path
+
+
+def mark_heart_as_surface(ov2, torso_tag):
     surfaces = gmsh.model.occ.getEntities(dim=2)
     volumes = gmsh.model.occ.getEntities(dim=3)
 
-    gmsh.model.occ.synchronize()
-
     gmsh.model.occ.cut(
         [(3, torso_tag)],
         ov2,
     )
 
     gmsh.model.occ.synchronize()
 
@@ -275,14 +292,16 @@
     side1_marker = 5
     side2_marker = 6
     side3_marker = 7
     side4_marker = 8
     side5_marker = 9
     side6_marker = 10
 
+    tissue_marker = 11
+
     gmsh.model.addPhysicalGroup(
         dim=surfaces[0][0],
         tags=[surfaces[0][1]],
         tag=side1_marker,
         name="TOP",
     )
     gmsh.model.addPhysicalGroup(
@@ -337,19 +356,112 @@
     gmsh.model.addPhysicalGroup(
         dim=surfaces[12][0],
         tags=[surfaces[12][1], surfaces[13][1]],
         tag=endo_lv_marker,
         name="ENDO_LV",
     )
 
-    gmsh.model.add_physical_group(dim=3, tags=[volumes[0][1]], tag=50, name="TISSUE")
-    # gmsh.option.setNumber("Mesh.SaveAll", 0)
-    gmsh.option.setNumber("Mesh.CharacteristicLengthMin", char_length)
-    gmsh.option.setNumber("Mesh.CharacteristicLengthMax", char_length)
+    gmsh.model.add_physical_group(
+        dim=3,
+        tags=[volumes[0][1]],
+        tag=tissue_marker,
+        name="TISSUE",
+    )
 
-    gmsh.model.mesh.generate(3)
-    gmsh.model.mesh.optimize("Netgen")
 
-    gmsh.write(path.as_posix())
-    gmsh.finalize()
+def mark_heart_as_volume(ov2, torso_tag):
+    surfaces = gmsh.model.occ.getEntities(dim=2)
 
-    return path
+    gmsh.model.occ.fuse([(3, torso_tag)], ov2, removeTool=False)
+
+    volumes = gmsh.model.occ.getEntities(dim=3)
+
+    gmsh.model.occ.synchronize()
+
+    base_marker = 1
+    endo_lv_marker = 2
+    endo_rv_marker = 3
+    epi_marker = 4
+
+    side1_marker = 5
+    side2_marker = 6
+    side3_marker = 7
+    side4_marker = 8
+    side5_marker = 9
+    side6_marker = 10
+
+    tissue_marker = 11
+    heart_marker = 12
+
+    gmsh.model.addPhysicalGroup(
+        dim=surfaces[8][0],
+        tags=[surfaces[8][1]],
+        tag=side1_marker,
+        name="TOP",
+    )
+    gmsh.model.addPhysicalGroup(
+        dim=surfaces[9][0],
+        tags=[surfaces[9][1]],
+        tag=side2_marker,
+        name="LEFT",
+    )
+    gmsh.model.addPhysicalGroup(
+        dim=surfaces[10][0],
+        tags=[surfaces[10][1]],
+        tag=side3_marker,
+        name="FRONT",
+    )
+    gmsh.model.addPhysicalGroup(
+        dim=surfaces[11][0],
+        tags=[surfaces[11][1]],
+        tag=side4_marker,
+        name="RIGHT",
+    )
+    gmsh.model.addPhysicalGroup(
+        dim=surfaces[12][0],
+        tags=[surfaces[12][1]],
+        tag=side5_marker,
+        name="BACK",
+    )
+    gmsh.model.addPhysicalGroup(
+        dim=surfaces[13][0],
+        tags=[surfaces[13][1]],
+        tag=side6_marker,
+        name="BOTTOM",
+    )
+
+    gmsh.model.addPhysicalGroup(
+        dim=surfaces[0][0],
+        tags=[surfaces[0][1], surfaces[2][1]],
+        tag=epi_marker,
+        name="EPI",
+    )
+    gmsh.model.addPhysicalGroup(
+        dim=surfaces[1][0],
+        tags=[surfaces[1][1]],
+        tag=base_marker,
+        name="BASE",
+    )
+    gmsh.model.addPhysicalGroup(
+        dim=surfaces[3][0],
+        tags=[surfaces[3][1], surfaces[4][1], surfaces[5][1]],
+        tag=endo_rv_marker,
+        name="ENDO_RV",
+    )
+    gmsh.model.addPhysicalGroup(
+        dim=surfaces[7][0],
+        tags=[surfaces[6][1], surfaces[7][1]],
+        tag=endo_lv_marker,
+        name="ENDO_LV",
+    )
+    gmsh.model.add_physical_group(
+        dim=3,
+        tags=[volumes[1][1]],
+        tag=tissue_marker,
+        name="TISSUE",
+    )
+    gmsh.model.add_physical_group(
+        dim=3,
+        tags=[volumes[0][1]],
+        tag=heart_marker,
+        name="HEART",
+    )
```

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py` & `cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries/_gmsh/_slab.py` & `cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/_slab.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries/_import_checks.py` & `cardiac_geometries-0.5.1/src/cardiac_geometries/_import_checks.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries/_mesh.py` & `cardiac_geometries-0.5.1/src/cardiac_geometries/_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,15 @@
 
     return geo
 
 
 def create_biv_ellipsoid_torso(
     outdir: Union[str, Path, None] = None,
     char_length: float = 0.5,
+    heart_as_surface: bool = True,
     torso_length: float = 20.0,
     torso_width: float = 20.0,
     torso_height: float = 20.0,
     rotation_angle: float = math.pi / 6,
     center_lv_y: float = 0.0,
     a_endo_lv: float = 2.5,
     b_endo_lv: float = 1.0,
@@ -223,14 +224,17 @@
     Parameters
     ----------
     outdir : Union[str, Path, None], optional
         Directory where to save the results. If not provided a temporary
         directory will be created, by default None, by default None
     char_length : float, optional
         Characteristic length of mesh, by default 0.5
+    heart_as_surface: bool
+        If true, create the heart as a a surface inside the torso,
+        otherwise let the heart be a volume, by default True.
     torso_length : float, optional
         Length of torso in the x-direction, by default 20.0
     torso_width : float, optional
         Length of torso in the y-direction, by default 20.0
     torso_height : float, optional
         Length of torso in the z-direction, by default 20.0
     rotation_angle: float, optional
@@ -297,14 +301,15 @@
     outdir = Path(outdir)
     outdir.mkdir(exist_ok=True, parents=True)
 
     with open(outdir / "info.json", "w") as f:
         json.dump(
             {
                 "char_length": char_length,
+                "heart_as_surface": heart_as_surface,
                 "torso_length": torso_length,
                 "torso_width": torso_width,
                 "torso_height": torso_height,
                 "rotation_angle": rotation_angle,
                 "center_lv": (0.0, center_lv_y, 0.0),
                 "a_endo_lv": a_endo_lv,
                 "b_endo_lv": b_endo_lv,
@@ -333,14 +338,15 @@
         )
 
     mesh_name = outdir / "biv_ellipsoid_torso.msh"
 
     biv_ellipsoid_torso(
         mesh_name=mesh_name.as_posix(),
         char_length=char_length,
+        heart_as_surface=heart_as_surface,
         torso_length=torso_length,
         torso_height=torso_height,
         torso_width=torso_width,
         rotation_angle=rotation_angle,
         center_lv=(0.0, center_lv_y, 0.0),
         a_endo_lv=a_endo_lv,
         b_endo_lv=b_endo_lv,
```

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries/_mshr/_biv.py` & `cardiac_geometries-0.5.1/src/cardiac_geometries/_mshr/_biv.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries/_mshr/_lv.py` & `cardiac_geometries-0.5.1/src/cardiac_geometries/_mshr/_lv.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries/calculus.py` & `cardiac_geometries-0.5.1/src/cardiac_geometries/calculus.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries/cli.py` & `cardiac_geometries-0.5.1/src/cardiac_geometries/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,14 +385,20 @@
     "--char-length",
     default=0.5,
     type=float,
     help="Characteristic length of mesh",
     show_default=True,
 )
 @click.option(
+    "--heart-as-surface/--heart-as-volume",
+    default=True,
+    help="Whether the heart should be a surface of a volume inside the torso",
+    show_default=True,
+)
+@click.option(
     "--torso-length",
     default=20,
     type=float,
     help="Length of torso in the x-direction",
     show_default=True,
 )
 @click.option(
@@ -545,14 +551,15 @@
     type=str,
     help="Function space for fibers of the form family_degree",
     show_default=True,
 )
 def create_biv_ellipsoid_torso(
     outdir: Path,
     char_length: float = 0.5,
+    heart_as_surface: bool = True,
     torso_length: float = 20.0,
     torso_width: float = 20.0,
     torso_height: float = 20.0,
     rotation_angle: float = math.pi / 6,
     center_lv_y: float = 0.0,
     a_endo_lv: float = 2.5,
     b_endo_lv: float = 1.0,
@@ -576,14 +583,15 @@
     outdir.mkdir(exist_ok=True)
 
     from ._mesh import create_biv_ellipsoid_torso
 
     geo = create_biv_ellipsoid_torso(
         outdir=outdir,
         char_length=char_length,
+        heart_as_surface=heart_as_surface,
         torso_length=torso_length,
         torso_height=torso_height,
         torso_width=torso_width,
         rotation_angle=rotation_angle,
         center_lv_y=center_lv_y,
         a_endo_lv=a_endo_lv,
         b_endo_lv=b_endo_lv,
```

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries/dolfin_utils.py` & `cardiac_geometries-0.5.1/src/cardiac_geometries/dolfin_utils.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/_biv_ellipsoid.py` & `cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/_biv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/_lv_ellipsoid.py` & `cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/_lv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/_slab.py` & `cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/_slab.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries/fibers/_utils.py` & `cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/_utils.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries/geometry.py` & `cardiac_geometries-0.5.1/src/cardiac_geometries/geometry.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries/viz.py` & `cardiac_geometries-0.5.1/src/cardiac_geometries/viz.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/PKG-INFO` & `cardiac_geometries-0.5.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cardiac-geometries
-Version: 0.5.0
+Name: cardiac_geometries
+Version: 0.5.1
 Summary: A python library for cardiac geometries
 Home-page: https://github.com/ComputationalPhysiology/cardiac_geometries
 Author: Henrik Finsberg
 Author-email: henriknf@simula.no
 License: MIT
 Keywords: cardiac,geometry,mesh,gmsh
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cardiac_geometries-0.5.0/src/cardiac_geometries.egg-info/SOURCES.txt` & `cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/tests/test_cli.py` & `cardiac_geometries-0.5.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/tests/test_geometry.py` & `cardiac_geometries-0.5.1/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.0/tests/test_gmsh.py` & `cardiac_geometries-0.5.1/tests/test_gmsh.py`

 * *Files identical despite different names*

