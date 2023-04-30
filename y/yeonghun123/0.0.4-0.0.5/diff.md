# Comparing `tmp/yeonghun123-0.0.4-py3-none-any.whl.zip` & `tmp/yeonghun123-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1624 bytes, number of entries: 5
--rw-r--r--  2.0 unx      516 b- defN 23-Apr-30 09:01 mydata/data.py
--rw-r--r--  2.0 unx      351 b- defN 23-Apr-30 09:01 yeonghun123-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-30 09:01 yeonghun123-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-30 09:01 yeonghun123-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      382 b- defN 23-Apr-30 09:01 yeonghun123-0.0.4.dist-info/RECORD
-5 files, 1348 bytes uncompressed, 906 bytes compressed:  32.8%
+Zip file size: 1627 bytes, number of entries: 5
+-rw-r--r--  2.0 unx      664 b- defN 23-Apr-30 09:06 mydata/data.py
+-rw-r--r--  2.0 unx      351 b- defN 23-Apr-30 09:06 yeonghun123-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-30 09:06 yeonghun123-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-30 09:06 yeonghun123-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      382 b- defN 23-Apr-30 09:06 yeonghun123-0.0.5.dist-info/RECORD
+5 files, 1496 bytes uncompressed, 909 bytes compressed:  39.2%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: mydata/data.py
 Comment: 
 
-Filename: yeonghun123-0.0.4.dist-info/METADATA
+Filename: yeonghun123-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: yeonghun123-0.0.4.dist-info/WHEEL
+Filename: yeonghun123-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: yeonghun123-0.0.4.dist-info/top_level.txt
+Filename: yeonghun123-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: yeonghun123-0.0.4.dist-info/RECORD
+Filename: yeonghun123-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mydata/data.py

```diff
@@ -1,21 +1,24 @@
 # data.py
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 
-print("파일명을 입력해주세요: ", end = ' ')
-file = f"{input()}"
-data=pd.read_csv(file)
-m=np.arange(1,13,1)
-
 def print_data():
+    print("파일명을 입력해주세요: ", end = ' ')
+    file = f"{input()}"
+    data=pd.read_csv(file)
+    m=np.arange(1,13,1)
     print(data)
 
 def print_visual_data():
+    print("파일명을 입력해주세요: ", end = ' ')
+    file = f"{input()}"
+    data=pd.read_csv(file)
+    m=np.arange(1,13,1)
     result=[]
     for x in m:
         rest=data[str(x)].sum()
 
         result.append(rest)
     plt.xticks(m)
     plt.xlabel('month')
```

