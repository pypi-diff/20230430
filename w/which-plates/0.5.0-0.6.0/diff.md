# Comparing `tmp/which_plates-0.5.0.tar.gz` & `tmp/which_plates-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "which_plates-0.5.0.tar", max compression
+gzip compressed data, was "which_plates-0.6.0.tar", max compression
```

## Comparing `which_plates-0.5.0.tar` & `which_plates-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    18047 2023-04-29 00:38:45.246151 which_plates-0.5.0/LICENSE
--rw-r--r--   0        0        0     1112 2023-04-29 00:38:45.246151 which_plates-0.5.0/README.md
--rw-r--r--   0        0        0     2087 2023-04-29 00:38:45.246151 which_plates-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      174 2023-04-29 00:38:45.246151 which_plates-0.5.0/src/which_plates/__init__.py
--rw-r--r--   0        0        0     1274 2023-04-29 00:38:45.246151 which_plates-0.5.0/src/which_plates/functions.py
--rw-r--r--   0        0        0     1759 2023-04-29 00:38:45.246151 which_plates-0.5.0/src/which_plates/main.py
--rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 which_plates-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    18047 2023-04-30 19:02:06.394543 which_plates-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1112 2023-04-30 19:02:06.394543 which_plates-0.6.0/README.md
+-rw-r--r--   0        0        0     2087 2023-04-30 19:02:06.394543 which_plates-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-04-30 19:02:06.394543 which_plates-0.6.0/src/which_plates/__init__.py
+-rw-r--r--   0        0        0     1314 2023-04-30 19:02:06.394543 which_plates-0.6.0/src/which_plates/functions.py
+-rw-r--r--   0        0        0     1759 2023-04-30 19:02:06.394543 which_plates-0.6.0/src/which_plates/main.py
+-rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 which_plates-0.6.0/PKG-INFO
```

### Comparing `which_plates-0.5.0/LICENSE` & `which_plates-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `which_plates-0.5.0/README.md` & `which_plates-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `which_plates-0.5.0/pyproject.toml` & `which_plates-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "which_plates"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = ["Ian Day <ian@ianday.me>"]
 readme = "README.md"
 #packages = [{include = "which_plates"}]
 homepage = "https://github.com/iandday/whichPlates"
 repository = "https://github.com/iandday/whichPlates"
 license = "GNUv2"
```

### Comparing `which_plates-0.5.0/src/which_plates/functions.py` & `which_plates-0.6.0/src/which_plates/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,12 +31,13 @@
         weight (int): desired weight
         available_plates (list): available plates
     Returns:
         dict: number of plates per weight to reach supplied weight
     """
     plates = {}
     remaining_weight = Decimal(round_num(weight))
+    available_plates.sort(reverse=True)
     for plate in available_plates:
         if remaining_weight / Decimal(plate) >= Decimal(2):
             plates[plate] = int(Decimal(remaining_weight) // Decimal(plate))
             remaining_weight -= Decimal(plate) * Decimal(plates[plate])
     return plates
```

### Comparing `which_plates-0.5.0/src/which_plates/main.py` & `which_plates-0.6.0/src/which_plates/main.py`

 * *Files identical despite different names*

### Comparing `which_plates-0.5.0/PKG-INFO` & `which_plates-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: which-plates
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Home-page: https://github.com/iandday/whichPlates
 License: GNUv2
 Author: Ian Day
 Author-email: ian@ianday.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

