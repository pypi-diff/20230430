# Comparing `tmp/xia_scw_template-0.0.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_template-0.0.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 101041 bytes, number of entries: 11
--rw-r--r--  2.0 unx      107 b- defN 23-Apr-30 19:46 xia_scw_template/__init__.py
--rw-r--r--  2.0 unx   236032 b- defN 23-Apr-30 19:53 xia_scw_template/template.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      103 b- defN 23-Apr-30 19:50 xia_scw_template/templates/Template/backend.tf
--rw-rw-rw-  2.0 unx      414 b- defN 23-Apr-30 19:50 xia_scw_template/templates/Template/main.tf
--rw-rw-rw-  2.0 unx       88 b- defN 23-Apr-30 19:50 xia_scw_template/templates/Template/output.tf
--rw-rw-rw-  2.0 unx      136 b- defN 23-Apr-30 19:50 xia_scw_template/templates/Template/variables.tf
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-30 19:53 xia_scw_template-0.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      672 b- defN 23-Apr-30 19:53 xia_scw_template-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-30 19:53 xia_scw_template-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-30 19:53 xia_scw_template-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1025 b- defN 23-Apr-30 19:53 xia_scw_template-0.0.1.dist-info/RECORD
-11 files, 238845 bytes uncompressed, 99259 bytes compressed:  58.4%
+Zip file size: 101069 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      107 b- defN 23-Apr-30 20:24 xia_scw_template/__init__.py
+-rw-r--r--  2.0 unx   236032 b- defN 23-Apr-30 20:26 xia_scw_template/template.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      103 b- defN 23-Apr-30 20:24 xia_scw_template/templates/ScwTemplate/backend.tf
+-rw-rw-rw-  2.0 unx      414 b- defN 23-Apr-30 20:24 xia_scw_template/templates/ScwTemplate/main.tf
+-rw-rw-rw-  2.0 unx       88 b- defN 23-Apr-30 20:24 xia_scw_template/templates/ScwTemplate/output.tf
+-rw-rw-rw-  2.0 unx      136 b- defN 23-Apr-30 20:24 xia_scw_template/templates/ScwTemplate/variables.tf
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-30 20:26 xia_scw_template-0.0.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      672 b- defN 23-Apr-30 20:26 xia_scw_template-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-30 20:26 xia_scw_template-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-30 20:26 xia_scw_template-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1037 b- defN 23-Apr-30 20:26 xia_scw_template-0.0.2.dist-info/RECORD
+11 files, 238857 bytes uncompressed, 99263 bytes compressed:  58.4%
```

## zipnote {}

```diff
@@ -1,34 +1,34 @@
 Filename: xia_scw_template/__init__.py
 Comment: 
 
 Filename: xia_scw_template/template.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_scw_template/templates/Template/backend.tf
+Filename: xia_scw_template/templates/ScwTemplate/backend.tf
 Comment: 
 
-Filename: xia_scw_template/templates/Template/main.tf
+Filename: xia_scw_template/templates/ScwTemplate/main.tf
 Comment: 
 
-Filename: xia_scw_template/templates/Template/output.tf
+Filename: xia_scw_template/templates/ScwTemplate/output.tf
 Comment: 
 
-Filename: xia_scw_template/templates/Template/variables.tf
+Filename: xia_scw_template/templates/ScwTemplate/variables.tf
 Comment: 
 
-Filename: xia_scw_template-0.0.1.dist-info/LICENSE.txt
+Filename: xia_scw_template-0.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_template-0.0.1.dist-info/METADATA
+Filename: xia_scw_template-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_template-0.0.1.dist-info/WHEEL
+Filename: xia_scw_template-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_template-0.0.1.dist-info/top_level.txt
+Filename: xia_scw_template-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_template-0.0.1.dist-info/RECORD
+Filename: xia_scw_template-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_template/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_scw_template.template import ScwTemplate
 
 
 __all__ = [
     "ScwTemplate"
 ]
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

## Comparing `xia_scw_template-0.0.1.dist-info/METADATA` & `xia_scw_template-0.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-scw-template
-Version: 0.0.1
+Version: 0.0.2
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-scw-template/0.0.1/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-scw-template/0.0.2/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_scw_template-0.0.1.dist-info/RECORD` & `xia_scw_template-0.0.2.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-xia_scw_template/__init__.py,sha256=cNymPmXPORIASGtvQklS_LZd70gAWalRueTKLyv8v5s,107
-xia_scw_template/template.cp39-win_amd64.pyd,sha256=F6bRKT99gmXWEJT-OATGnar0lnRig5bCV6fRpqJrdWA,236032
-xia_scw_template/templates/Template/backend.tf,sha256=bbBhWpPkAyaZDrgmjRWClB3kEffcP-qaiC2vlXXlAKY,103
-xia_scw_template/templates/Template/main.tf,sha256=USKe9YPVicChcPSxUbZP_-f-kcFqLY4Ssi3zkPkHS8Q,414
-xia_scw_template/templates/Template/output.tf,sha256=1KMXhU7r9bqIjg7VEHcajCLA-ZSvh12mqYzXsK2Jaqs,88
-xia_scw_template/templates/Template/variables.tf,sha256=aR-VP5gMS05TmxMvdMAIuKoGmfNULd0cBGUqelhyCv8,136
-xia_scw_template-0.0.1.dist-info/LICENSE.txt,sha256=t7dcmwWYpCopxtSO2xM5htr8WC8xUXgTax2q0dOA-Ak,152
-xia_scw_template-0.0.1.dist-info/METADATA,sha256=WL0Y0x5s5GwBvRJZj6rjekTzie-L5I9NnhG9M3gKM-U,672
-xia_scw_template-0.0.1.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_scw_template-0.0.1.dist-info/top_level.txt,sha256=PnzNPYJvb9BCFS0nMLHk3DDKw5vJjkdhUg0gD_vL_cU,17
-xia_scw_template-0.0.1.dist-info/RECORD,,
+xia_scw_template/__init__.py,sha256=O03FiJ1FnOSSupNBZMHPHBQbbbhPMCFBnUaUwwJHJRY,107
+xia_scw_template/template.cp39-win_amd64.pyd,sha256=o0NVWdnhQ0z8R9nG7hCJoh3HlBOmdSam4ggTaTwjRUE,236032
+xia_scw_template/templates/ScwTemplate/backend.tf,sha256=bbBhWpPkAyaZDrgmjRWClB3kEffcP-qaiC2vlXXlAKY,103
+xia_scw_template/templates/ScwTemplate/main.tf,sha256=USKe9YPVicChcPSxUbZP_-f-kcFqLY4Ssi3zkPkHS8Q,414
+xia_scw_template/templates/ScwTemplate/output.tf,sha256=1KMXhU7r9bqIjg7VEHcajCLA-ZSvh12mqYzXsK2Jaqs,88
+xia_scw_template/templates/ScwTemplate/variables.tf,sha256=aR-VP5gMS05TmxMvdMAIuKoGmfNULd0cBGUqelhyCv8,136
+xia_scw_template-0.0.2.dist-info/LICENSE.txt,sha256=t7dcmwWYpCopxtSO2xM5htr8WC8xUXgTax2q0dOA-Ak,152
+xia_scw_template-0.0.2.dist-info/METADATA,sha256=0xLOk5QO_uxqnsGLqurZ8NEK59_ikM2WXpF5IG8n7Yo,672
+xia_scw_template-0.0.2.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_scw_template-0.0.2.dist-info/top_level.txt,sha256=PnzNPYJvb9BCFS0nMLHk3DDKw5vJjkdhUg0gD_vL_cU,17
+xia_scw_template-0.0.2.dist-info/RECORD,,
```

