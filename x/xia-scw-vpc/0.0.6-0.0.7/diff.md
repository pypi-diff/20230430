# Comparing `tmp/xia_scw_vpc-0.0.6-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_vpc-0.0.7-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 110231 bytes, number of entries: 12
--rw-r--r--  2.0 unx       87 b- defN 23-Apr-21 16:00 xia_scw_vpc/__init__.py
--rw-r--r--  2.0 unx   257024 b- defN 23-Apr-21 16:06 xia_scw_vpc/vpc.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx       69 b- defN 23-Apr-21 13:39 xia_scw_vpc/templates/ScwVpc/backend.tf
--rw-rw-rw-  2.0 unx      991 b- defN 23-Apr-21 16:00 xia_scw_vpc/templates/ScwVpc/main.tf
--rw-rw-rw-  2.0 unx      651 b- defN 23-Apr-21 16:00 xia_scw_vpc/templates/ScwVpc/output.tf
--rw-rw-rw-  2.0 unx      343 b- defN 23-Apr-21 13:39 xia_scw_vpc/templates/ScwVpc/provider.tf
--rw-rw-rw-  2.0 unx     1953 b- defN 23-Apr-21 16:00 xia_scw_vpc/templates/ScwVpc/variables.tf
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-21 16:06 xia_scw_vpc-0.0.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      652 b- defN 23-Apr-21 16:06 xia_scw_vpc-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-21 16:06 xia_scw_vpc-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-21 16:06 xia_scw_vpc-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1053 b- defN 23-Apr-21 16:06 xia_scw_vpc-0.0.6.dist-info/RECORD
-12 files, 263086 bytes uncompressed, 108429 bytes compressed:  58.8%
+Zip file size: 87766 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       87 b- defN 23-Apr-30 07:59 xia_scw_vpc/__init__.py
+-rw-r--r--  2.0 unx   235400 b- defN 23-Apr-30 07:59 xia_scw_vpc/vpc.cpython-310-darwin.so
+-rw-r--r--  2.0 unx       69 b- defN 23-Apr-21 16:02 xia_scw_vpc/templates/ScwVpc/backend.tf
+-rw-r--r--  2.0 unx      991 b- defN 23-Apr-21 16:02 xia_scw_vpc/templates/ScwVpc/main.tf
+-rw-r--r--  2.0 unx      651 b- defN 23-Apr-21 16:02 xia_scw_vpc/templates/ScwVpc/output.tf
+-rw-r--r--  2.0 unx      343 b- defN 23-Apr-21 16:02 xia_scw_vpc/templates/ScwVpc/provider.tf
+-rw-r--r--  2.0 unx     1953 b- defN 23-Apr-21 16:02 xia_scw_vpc/templates/ScwVpc/variables.tf
+-rw-r--r--  2.0 unx      152 b- defN 23-Apr-30 07:59 xia_scw_vpc-0.0.7.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      615 b- defN 23-Apr-30 07:59 xia_scw_vpc-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Apr-30 07:59 xia_scw_vpc-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-30 07:59 xia_scw_vpc-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1057 b- defN 23-Apr-30 07:59 xia_scw_vpc-0.0.7.dist-info/RECORD
+12 files, 241438 bytes uncompressed, 85958 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
 Filename: xia_scw_vpc/__init__.py
 Comment: 
 
-Filename: xia_scw_vpc/vpc.cp39-win_amd64.pyd
+Filename: xia_scw_vpc/vpc.cpython-310-darwin.so
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/backend.tf
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/main.tf
 Comment: 
@@ -15,23 +15,23 @@
 
 Filename: xia_scw_vpc/templates/ScwVpc/provider.tf
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/variables.tf
 Comment: 
 
-Filename: xia_scw_vpc-0.0.6.dist-info/LICENSE.txt
+Filename: xia_scw_vpc-0.0.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_vpc-0.0.6.dist-info/METADATA
+Filename: xia_scw_vpc-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_vpc-0.0.6.dist-info/WHEEL
+Filename: xia_scw_vpc-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_vpc-0.0.6.dist-info/top_level.txt
+Filename: xia_scw_vpc-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_vpc-0.0.6.dist-info/RECORD
+Filename: xia_scw_vpc-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_vpc/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_scw_vpc.vpc import ScwVpc
 
 
 __all__ = [
     "ScwVpc"
 ]
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
```

## Comparing `xia_scw_vpc-0.0.6.dist-info/METADATA` & `xia_scw_vpc-0.0.7.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xia-scw-vpc
-Version: 0.0.6
+Version: 0.0.7
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-scw-vpc/0.0.6/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-scw-vpc/0.0.7/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: xia-engine-terraform
 
 .. image:: https://img.shields.io/pypi/v/xia-scw-vpc.svg?color=blue
    :alt: PyPI-Server
@@ -26,9 +24,7 @@
 =============================
 
 Install the package::
 
     pip install
 
 
-
-
```

