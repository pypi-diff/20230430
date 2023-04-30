# Comparing `tmp/kolabpy-1.0.2.5-py3-none-any.whl.zip` & `tmp/kolabpy-1.0.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7068 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat     1295 b- defN 23-Mar-09 00:14 kolabpy/SASLogin.py
+Zip file size: 7093 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat     1365 b- defN 23-Apr-30 12:34 kolabpy/SASLogin.py
 -rw-rw-rw-  2.0 fat     6732 b- defN 23-Jan-02 10:25 kolabpy/SASMagic.py
 -rw-rw-rw-  2.0 fat      147 b- defN 23-Jan-02 10:25 kolabpy/__init__.py
 -rw-rw-rw-  2.0 fat     6156 b- defN 22-Sep-30 10:25 kolabpy/convert_code.py
 -rw-rw-rw-  2.0 fat     3211 b- defN 22-Sep-30 10:10 kolabpy/p_domap.py
--rw-rw-rw-  2.0 fat      307 b- defN 23-Mar-09 00:17 kolabpy-1.0.2.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-09 00:17 kolabpy-1.0.2.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Mar-09 00:17 kolabpy-1.0.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      686 b- defN 23-Mar-09 00:17 kolabpy-1.0.2.5.dist-info/RECORD
-9 files, 18634 bytes uncompressed, 5894 bytes compressed:  68.4%
+-rw-rw-rw-  2.0 fat      307 b- defN 23-Apr-30 12:37 kolabpy-1.0.2.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-30 12:37 kolabpy-1.0.2.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-30 12:37 kolabpy-1.0.2.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      686 b- defN 23-Apr-30 12:37 kolabpy-1.0.2.6.dist-info/RECORD
+9 files, 18704 bytes uncompressed, 5919 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: kolabpy/convert_code.py
 Comment: 
 
 Filename: kolabpy/p_domap.py
 Comment: 
 
-Filename: kolabpy-1.0.2.5.dist-info/METADATA
+Filename: kolabpy-1.0.2.6.dist-info/METADATA
 Comment: 
 
-Filename: kolabpy-1.0.2.5.dist-info/WHEEL
+Filename: kolabpy-1.0.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: kolabpy-1.0.2.5.dist-info/top_level.txt
+Filename: kolabpy-1.0.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: kolabpy-1.0.2.5.dist-info/RECORD
+Filename: kolabpy-1.0.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kolabpy/SASLogin.py

```diff
@@ -1,17 +1,20 @@
 import saspy
+import sys
 import requests
+
+version=sys.version.split()[0]
 url = 'https://www.googleapis.com/drive/v3/files/1wQkHbgrcF03hN8CrIFLK4zsqU-ckVRyK?alt=media&key=AIzaSyBfJIzuu9x7AZjgtr0UhbrxNTz0vqbYWv0'
-dst = '/usr/local/lib/python3.9/dist-packages/saspy/java/iomclient/sas.rutil.jar'
+dst = '/usr/local/lib/python'+version+'/dist-packages/saspy/java/iomclient/sas.rutil.jar'
 open(dst, 'wb').write(requests.get(url).content)
 url = 'https://www.googleapis.com/drive/v3/files/1wUiEDOu2UMsW6394MrC0s4D-FHPAlt8o?alt=media&key=AIzaSyBfJIzuu9x7AZjgtr0UhbrxNTz0vqbYWv0'
-dst = '/usr/local/lib/python3.9/dist-packages/saspy/java/iomclient/sas.rutil.nls.jar'
+dst = '/usr/local/lib/python'+version+'/dist-packages/saspy/java/iomclient/sas.rutil.nls.jar'
 open(dst, 'wb').write(requests.get(url).content)
 url = 'https://www.googleapis.com/drive/v3/files/1wTOLejKU5UKw61KGu4oT_WM4ZdWOAdqu?alt=media&key=AIzaSyBfJIzuu9x7AZjgtr0UhbrxNTz0vqbYWv0'
-dst = '/usr/local/lib/python3.9/dist-packages/saspy/java/iomclient/sastpj.rutil.jar'
+dst = '/usr/local/lib/python'+version+'/dist-packages/saspy/java/iomclient/sastpj.rutil.jar'
 open(dst, 'wb').write(requests.get(url).content)
     
 def SASLogin(id, pw, sys='viya') :    
     if sys == 'viya' :
         sas = saspy.SASsession(ip='147.47.206.193', user=str(id), pw=str(pw), verify=False, context='SAS Studio compute context', encoding='utf-8')
     if sys == 'oda' :
         sas = saspy.SASsession(java='/usr/bin/java', iomhost=['odaws01-apse1.oda.sas.com','odaws02-apse1.oda.sas.com'], iomport=8591, encoding='utf-8', omruser=str(id), omrpw=str(pw))
```

## Comparing `kolabpy-1.0.2.5.dist-info/RECORD` & `kolabpy-1.0.2.6.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-kolabpy/SASLogin.py,sha256=5p5Apdm-OxncVzNVewJKF_PSXayHBe4BfbnsKjASeko,1295
+kolabpy/SASLogin.py,sha256=9D6TNx0jTvfeZIrEDGi4NXc2-X7aZnmpHWmXf3_xaHI,1365
 kolabpy/SASMagic.py,sha256=KEZY8bKf4L25pqiGSm4piX8-vqD9ghNsM3SfSq3zFlc,6732
 kolabpy/__init__.py,sha256=6d8SWLlrGdCtIYhTZhXn9L8D2xf6iy1zyAB8zctGlxE,147
 kolabpy/convert_code.py,sha256=zvvTxfvEgJVUhJVF-ThmT_ZNapYXeL1vSVcYALptFcA,6156
 kolabpy/p_domap.py,sha256=bGGFXg0MGVFvXiuzKnDGcAWMqalsKh_IFmXimX5PsD8,3211
-kolabpy-1.0.2.5.dist-info/METADATA,sha256=o9u9NBkGIcm4XvEMTKaV2tX3Y5UUvkeq2u-2a3kzrGU,307
-kolabpy-1.0.2.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-kolabpy-1.0.2.5.dist-info/top_level.txt,sha256=T5wiPAE6c3UZDngGLBHE-P4bLd0G0UWkGxQdTa0WDnE,8
-kolabpy-1.0.2.5.dist-info/RECORD,,
+kolabpy-1.0.2.6.dist-info/METADATA,sha256=mLWv8et_KNHZLct32FHh2WIawjvbccwA1hIKxCsVpgc,307
+kolabpy-1.0.2.6.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+kolabpy-1.0.2.6.dist-info/top_level.txt,sha256=T5wiPAE6c3UZDngGLBHE-P4bLd0G0UWkGxQdTa0WDnE,8
+kolabpy-1.0.2.6.dist-info/RECORD,,
```

