# Comparing `tmp/yeonghun123-0.0.2-py3-none-any.whl.zip` & `tmp/yeonghun123-0.0.4-py3-none-any.whl.zip`

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
+Zip file size: 1624 bytes, number of entries: 5
+-rw-r--r--  2.0 unx      516 b- defN 23-Apr-30 09:01 mydata/data.py
+-rw-r--r--  2.0 unx      351 b- defN 23-Apr-30 09:01 yeonghun123-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-30 09:01 yeonghun123-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-30 09:01 yeonghun123-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      382 b- defN 23-Apr-30 09:01 yeonghun123-0.0.4.dist-info/RECORD
+5 files, 1348 bytes uncompressed, 906 bytes compressed:  32.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: mydata/data.py
 Comment: 
 
-Filename: yeonghun123-0.0.2.dist-info/METADATA
+Filename: yeonghun123-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: yeonghun123-0.0.2.dist-info/WHEEL
+Filename: yeonghun123-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: yeonghun123-0.0.2.dist-info/top_level.txt
+Filename: yeonghun123-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: yeonghun123-0.0.2.dist-info/RECORD
+Filename: yeonghun123-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mydata/data.py

```diff
@@ -1,24 +1,26 @@
 # data.py
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
-data=pd.read_csv("C:\\Users\\jyh11\\Desktop\\JYH11224\\workspace\\B_JUN_python\\busan_dust.csv")
+
+print("파일명을 입력해주세요: ", end = ' ')
+file = f"{input()}"
+data=pd.read_csv(file)
 m=np.arange(1,13,1)
 
 def print_data():
     print(data)
 
 def print_visual_data():
     result=[]
     for x in m:
         rest=data[str(x)].sum()
 
         result.append(rest)
-    print(data)
     plt.xticks(m)
     plt.xlabel('month')
     plt.ylabel('year')
     plt.title('Number of dust storm days per month in Busan')
     plt.bar(m,result)
 
     plt.show()
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

