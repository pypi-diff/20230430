# Comparing `tmp/yeonghun123-0.0.2-py3-none-any.whl.zip` & `tmp/yeonghun123-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1607 bytes, number of entries: 5
--rw-r--r--  2.0 unx      531 b- defN 23-Apr-30 08:15 mydata/data.py
--rw-r--r--  2.0 unx      351 b- defN 23-Apr-30 08:26 yeonghun123-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-30 08:26 yeonghun123-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-30 08:26 yeonghun123-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      382 b- defN 23-Apr-30 08:26 yeonghun123-0.0.2.dist-info/RECORD
-5 files, 1363 bytes uncompressed, 889 bytes compressed:  34.8%
+Zip file size: 1564 bytes, number of entries: 5
+-rw-r--r--  2.0 unx      478 b- defN 23-Apr-30 08:37 mydata/data.py
+-rw-r--r--  2.0 unx      351 b- defN 23-Apr-30 08:37 yeonghun123-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-30 08:37 yeonghun123-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-30 08:37 yeonghun123-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      382 b- defN 23-Apr-30 08:37 yeonghun123-0.0.3.dist-info/RECORD
+5 files, 1310 bytes uncompressed, 846 bytes compressed:  35.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: mydata/data.py
 Comment: 
 
-Filename: yeonghun123-0.0.2.dist-info/METADATA
+Filename: yeonghun123-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: yeonghun123-0.0.2.dist-info/WHEEL
+Filename: yeonghun123-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: yeonghun123-0.0.2.dist-info/top_level.txt
+Filename: yeonghun123-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: yeonghun123-0.0.2.dist-info/RECORD
+Filename: yeonghun123-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mydata/data.py

```diff
@@ -1,12 +1,14 @@
 # data.py
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
-data=pd.read_csv("C:\\Users\\jyh11\\Desktop\\JYH11224\\workspace\\B_JUN_python\\busan_dust.csv")
+
+file = f"{input()}"
+data=pd.read_csv(file)
 m=np.arange(1,13,1)
 
 def print_data():
     print(data)
 
 def print_visual_data():
     result=[]
```

