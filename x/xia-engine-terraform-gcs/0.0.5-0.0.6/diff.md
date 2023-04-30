# Comparing `tmp/xia_engine_terraform_gcs-0.0.5-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_terraform_gcs-0.0.6-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 124570 bytes, number of entries: 7
--rw-r--r--  2.0 unx      378 b- defN 23-Apr-21 09:20 xia_engine_terraform_gcs/__init__.py
--rw-r--r--  2.0 unx   295424 b- defN 23-Apr-21 09:23 xia_engine_terraform_gcs/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-21 09:23 xia_engine_terraform_gcs-0.0.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      726 b- defN 23-Apr-21 09:23 xia_engine_terraform_gcs-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-21 09:23 xia_engine_terraform_gcs-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 23-Apr-21 09:23 xia_engine_terraform_gcs-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      674 b- defN 23-Apr-21 09:23 xia_engine_terraform_gcs-0.0.5.dist-info/RECORD
-7 files, 297478 bytes uncompressed, 123348 bytes compressed:  58.5%
+Zip file size: 101980 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      378 b- defN 23-Apr-30 16:39 xia_engine_terraform_gcs/__init__.py
+-rw-r--r--  2.0 unx   270752 b- defN 23-Apr-30 16:39 xia_engine_terraform_gcs/engine.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      152 b- defN 23-Apr-30 16:39 xia_engine_terraform_gcs-0.0.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      689 b- defN 23-Apr-30 16:39 xia_engine_terraform_gcs-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Apr-30 16:39 xia_engine_terraform_gcs-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 23-Apr-30 16:39 xia_engine_terraform_gcs-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      678 b- defN 23-Apr-30 16:39 xia_engine_terraform_gcs-0.0.6.dist-info/RECORD
+7 files, 272782 bytes uncompressed, 100752 bytes compressed:  63.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_terraform_gcs/__init__.py
 Comment: 
 
-Filename: xia_engine_terraform_gcs/engine.cp39-win_amd64.pyd
+Filename: xia_engine_terraform_gcs/engine.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.0.5.dist-info/LICENSE.txt
+Filename: xia_engine_terraform_gcs-0.0.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.0.5.dist-info/METADATA
+Filename: xia_engine_terraform_gcs-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.0.5.dist-info/WHEEL
+Filename: xia_engine_terraform_gcs-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.0.5.dist-info/top_level.txt
+Filename: xia_engine_terraform_gcs-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.0.5.dist-info/RECORD
+Filename: xia_engine_terraform_gcs-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_terraform_gcs/__init__.py

```diff
@@ -3,8 +3,8 @@
 
 
 __all__ = [
     "TerraformGcsEngine", "TerraformGcsConnectParam", "TerraformGcsClient",
     "ScwTerraformGcsEngine", "ScwTerraformGcsConnectParam"
 ]
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
```

## Comparing `xia_engine_terraform_gcs-0.0.5.dist-info/METADATA` & `xia_engine_terraform_gcs-0.0.6.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xia-engine-terraform-gcs
-Version: 0.0.5
+Version: 0.0.6
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform-gcs/0.0.5/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform-gcs/0.0.6/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: jinja2
 Requires-Dist: xia-engine-terraform
 
 .. image:: https://img.shields.io/pypi/v/xia-engine-terraform-gcs.svg?color=blue
@@ -27,9 +25,7 @@
 =============================
 
 Install the package::
 
     pip install
 
 
-
-
```

