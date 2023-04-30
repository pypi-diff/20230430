# Comparing `tmp/xia_scw_instance-0.0.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_instance-0.0.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 114820 bytes, number of entries: 12
--rw-r--r--  2.0 unx      133 b- defN 23-Apr-22 10:42 xia_scw_instance/__init__.py
--rw-r--r--  2.0 unx   266752 b- defN 23-Apr-22 12:40 xia_scw_instance/instance.cp39-win_amd64.pyd
+Zip file size: 114821 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      133 b- defN 23-Apr-22 16:35 xia_scw_instance/__init__.py
+-rw-r--r--  2.0 unx   266752 b- defN 23-Apr-22 16:44 xia_scw_instance/instance.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 unx       69 b- defN 23-Apr-21 11:31 xia_scw_instance/templates/ScwInstance/backend.tf
 -rw-rw-rw-  2.0 unx     3026 b- defN 23-Apr-22 12:29 xia_scw_instance/templates/ScwInstance/main.tf
--rw-rw-rw-  2.0 unx      766 b- defN 23-Apr-22 10:42 xia_scw_instance/templates/ScwInstance/output.tf
+-rw-rw-rw-  2.0 unx      766 b- defN 23-Apr-22 16:35 xia_scw_instance/templates/ScwInstance/output.tf
 -rw-rw-rw-  2.0 unx      343 b- defN 23-Apr-21 11:31 xia_scw_instance/templates/ScwInstance/provider.tf
 -rw-rw-rw-  2.0 unx     4173 b- defN 23-Apr-22 10:42 xia_scw_instance/templates/ScwInstance/variables.tf
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-22 12:40 xia_scw_instance-0.0.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      699 b- defN 23-Apr-22 12:40 xia_scw_instance-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-22 12:40 xia_scw_instance-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-22 12:40 xia_scw_instance-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1145 b- defN 23-Apr-22 12:40 xia_scw_instance-0.0.8.dist-info/RECORD
-12 files, 277374 bytes uncompressed, 112838 bytes compressed:  59.3%
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-22 16:44 xia_scw_instance-0.0.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      699 b- defN 23-Apr-22 16:44 xia_scw_instance-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-22 16:44 xia_scw_instance-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-22 16:44 xia_scw_instance-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1145 b- defN 23-Apr-22 16:44 xia_scw_instance-0.0.9.dist-info/RECORD
+12 files, 277374 bytes uncompressed, 112839 bytes compressed:  59.3%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: xia_scw_instance/templates/ScwInstance/provider.tf
 Comment: 
 
 Filename: xia_scw_instance/templates/ScwInstance/variables.tf
 Comment: 
 
-Filename: xia_scw_instance-0.0.8.dist-info/LICENSE.txt
+Filename: xia_scw_instance-0.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_instance-0.0.8.dist-info/METADATA
+Filename: xia_scw_instance-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_instance-0.0.8.dist-info/WHEEL
+Filename: xia_scw_instance-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_instance-0.0.8.dist-info/top_level.txt
+Filename: xia_scw_instance-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_instance-0.0.8.dist-info/RECORD
+Filename: xia_scw_instance-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_instance/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_scw_instance.instance import ScwInstance, ScwForward
 
 
 __all__ = [
     "ScwInstance", "ScwForward"
 ]
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

## xia_scw_instance/templates/ScwInstance/output.tf

```diff
@@ -27,15 +27,15 @@
 }
 
 output "wan_ip" {
   value = var.wan_ip
 }
 
 output "lan_ip" {
-  value = var.wan_ip
+  value = var.lan_ip
 }
 
 output "lan_name" {
   value = var.lan_name
 }
 
 output "ssh_hosts" {
```

## Comparing `xia_scw_instance-0.0.8.dist-info/METADATA` & `xia_scw_instance-0.0.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-scw-instance
-Version: 0.0.8
+Version: 0.0.9
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-scw-instance/0.0.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-scw-instance/0.0.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_scw_instance-0.0.8.dist-info/RECORD` & `xia_scw_instance-0.0.9.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-xia_scw_instance/__init__.py,sha256=xE9u2A2lBfr7FX2xDzAx2VAtHRy8_vMNeDY7TqCRv-k,133
-xia_scw_instance/instance.cp39-win_amd64.pyd,sha256=lbyRefOCQz165AL7Re3UUj_vBySd7cwfi7XlCh1BWiU,266752
+xia_scw_instance/__init__.py,sha256=hvJ-V6hddQOpaA5D8-F3ZKJ01tu3dEUuoZYn3FFJy1E,133
+xia_scw_instance/instance.cp39-win_amd64.pyd,sha256=K4FJllWXj0Xyh5b6iQ-moOHgRQqNjZh2cFj9DzX1Ufs,266752
 xia_scw_instance/templates/ScwInstance/backend.tf,sha256=E6fgAX-nMcTt9oErRKvK67uJPdB-O77YJpzAvf06zgs,69
 xia_scw_instance/templates/ScwInstance/main.tf,sha256=4AT2qTq0fYZBzJBJXvWxktIvoqWY6Qlgs-6Wf1PXeQE,3026
-xia_scw_instance/templates/ScwInstance/output.tf,sha256=3xDrNiAsa1jY_YqxmeTH2aJDtGPboK-5MnJwtIH4Yi8,766
+xia_scw_instance/templates/ScwInstance/output.tf,sha256=Z-bfCjy9nrVOd98T2JSHiDAv5cP7kI_Qs5h49elb6H0,766
 xia_scw_instance/templates/ScwInstance/provider.tf,sha256=h_zFGas7QtYJPGvufLGuPHtgDhoZa28Qa5t--1dpheI,343
 xia_scw_instance/templates/ScwInstance/variables.tf,sha256=qkzRe_c7wVjYF89AqoJQcYPu0kyxRgo1Q0QrlUuxgsQ,4173
-xia_scw_instance-0.0.8.dist-info/LICENSE.txt,sha256=CgeJ1rTURAK7GLPD_GW3lyXH8ZFFrBDM0ekl9JHZR2s,152
-xia_scw_instance-0.0.8.dist-info/METADATA,sha256=LtehzFZFORd1xJrN582GGhqDMd3dlgjGotzxIVGxCd0,699
-xia_scw_instance-0.0.8.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_scw_instance-0.0.8.dist-info/top_level.txt,sha256=ffd5mxc0r47bbdzdm8uAtew5JL-56N5Dvcrqvp9tri0,17
-xia_scw_instance-0.0.8.dist-info/RECORD,,
+xia_scw_instance-0.0.9.dist-info/LICENSE.txt,sha256=CgeJ1rTURAK7GLPD_GW3lyXH8ZFFrBDM0ekl9JHZR2s,152
+xia_scw_instance-0.0.9.dist-info/METADATA,sha256=rnTGHV4EhHlRK8USD2W1hocPT1qPdv3pGtGFNr67bsY,699
+xia_scw_instance-0.0.9.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_scw_instance-0.0.9.dist-info/top_level.txt,sha256=ffd5mxc0r47bbdzdm8uAtew5JL-56N5Dvcrqvp9tri0,17
+xia_scw_instance-0.0.9.dist-info/RECORD,,
```

