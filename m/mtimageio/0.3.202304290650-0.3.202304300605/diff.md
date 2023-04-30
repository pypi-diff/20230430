# Comparing `tmp/mtimageio-0.3.202304290650-py3-none-any.whl.zip` & `tmp/mtimageio-0.3.202304300605-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 8979 bytes, number of entries: 12
+Zip file size: 9023 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      162 b- defN 23-Feb-21 07:08 mt/iio/__init__.py
 -rw-r--r--  2.0 unx      194 b- defN 22-Dec-30 06:14 mt/imageio/__init__.py
 -rw-r--r--  2.0 unx     3600 b- defN 23-Feb-21 07:08 mt/imageio/immview.py
 -rw-r--r--  2.0 unx    10139 b- defN 23-Apr-29 06:50 mt/imageio/imread.py
--rw-r--r--  2.0 unx     7561 b- defN 23-Apr-29 06:40 mt/imageio/imwrite.py
--rw-r--r--  2.0 unx      396 b- defN 23-Apr-29 06:50 mt/imageio/version.py
--rwxr-xr-x  2.0 unx     1003 b- defN 23-Apr-29 06:51 mtimageio-0.3.202304290650.data/scripts/immview
--rw-r--r--  2.0 unx     1500 b- defN 23-Apr-29 06:51 mtimageio-0.3.202304290650.dist-info/LICENSE
--rw-r--r--  2.0 unx      290 b- defN 23-Apr-29 06:51 mtimageio-0.3.202304290650.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-29 06:51 mtimageio-0.3.202304290650.dist-info/WHEEL
--rw-r--r--  2.0 unx        3 b- defN 23-Apr-29 06:51 mtimageio-0.3.202304290650.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1016 b- defN 23-Apr-29 06:51 mtimageio-0.3.202304290650.dist-info/RECORD
-12 files, 25956 bytes uncompressed, 7257 bytes compressed:  72.0%
+-rw-r--r--  2.0 unx     7734 b- defN 23-Apr-30 06:05 mt/imageio/imwrite.py
+-rw-r--r--  2.0 unx      396 b- defN 23-Apr-30 06:05 mt/imageio/version.py
+-rwxr-xr-x  2.0 unx     1003 b- defN 23-Apr-30 06:06 mtimageio-0.3.202304300605.data/scripts/immview
+-rw-r--r--  2.0 unx     1500 b- defN 23-Apr-30 06:06 mtimageio-0.3.202304300605.dist-info/LICENSE
+-rw-r--r--  2.0 unx      290 b- defN 23-Apr-30 06:06 mtimageio-0.3.202304300605.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-30 06:06 mtimageio-0.3.202304300605.dist-info/WHEEL
+-rw-r--r--  2.0 unx        3 b- defN 23-Apr-30 06:06 mtimageio-0.3.202304300605.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1016 b- defN 23-Apr-30 06:06 mtimageio-0.3.202304300605.dist-info/RECORD
+12 files, 26129 bytes uncompressed, 7301 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: mt/imageio/imwrite.py
 Comment: 
 
 Filename: mt/imageio/version.py
 Comment: 
 
-Filename: mtimageio-0.3.202304290650.data/scripts/immview
+Filename: mtimageio-0.3.202304300605.data/scripts/immview
 Comment: 
 
-Filename: mtimageio-0.3.202304290650.dist-info/LICENSE
+Filename: mtimageio-0.3.202304300605.dist-info/LICENSE
 Comment: 
 
-Filename: mtimageio-0.3.202304290650.dist-info/METADATA
+Filename: mtimageio-0.3.202304300605.dist-info/METADATA
 Comment: 
 
-Filename: mtimageio-0.3.202304290650.dist-info/WHEEL
+Filename: mtimageio-0.3.202304300605.dist-info/WHEEL
 Comment: 
 
-Filename: mtimageio-0.3.202304290650.dist-info/top_level.txt
+Filename: mtimageio-0.3.202304300605.dist-info/top_level.txt
 Comment: 
 
-Filename: mtimageio-0.3.202304290650.dist-info/RECORD
+Filename: mtimageio-0.3.202304300605.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mt/imageio/imwrite.py

```diff
@@ -111,15 +111,23 @@
     )
     return data
 
 
 def immencode_webp(imm: cv.Image) -> bytes:
     xmp = json.dumps(imm.meta)
     data = iio.imwrite(
-        "<bytes>", imm.image, plugin="pillow", extension=".webp", lossless=True, xmp=xmp
+        "<bytes>",
+        imm.image,
+        plugin="pillow",
+        extension=".webp",
+        lossless=True,
+        exact=True,  # pillow default is False
+        quality=90,  # pillow default is 80
+        method=5,  # pillow default is 4
+        xmp=xmp,
     )
     return data
 
 
 def immencode(imm: cv.Image, encoding_format: str = "png") -> bytes:
     """Encodes a :class:`mt.cv.opencv.Image` instance as a PNG or WEBP image with metadata.
```

## mt/imageio/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('04')
-VERSION_DAY = int('29')
+VERSION_DAY = int('30')
 VERSION_HOUR = int('06')
-VERSION_MINUTE = int('50')
+VERSION_MINUTE = int('05')
 MAJOR_VERSION = 0
 MINOR_VERSION = 3
-PATCH_VERSION = 202304290650
-version_date = '2023/04/29 06:50'
+PATCH_VERSION = 202304300605
+version_date = '2023/04/30 06:05'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mtimageio-0.3.202304290650.data/scripts/immview` & `mtimageio-0.3.202304300605.data/scripts/immview`

 * *Files identical despite different names*

## Comparing `mtimageio-0.3.202304290650.dist-info/LICENSE` & `mtimageio-0.3.202304300605.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mtimageio-0.3.202304290650.dist-info/RECORD` & `mtimageio-0.3.202304300605.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 mt/iio/__init__.py,sha256=EqGagZkVypSdxXpARpz7jco0R_-IH9YOmbEBPmJl5vk,162
 mt/imageio/__init__.py,sha256=lUXEdtMwN2YBWCoNu82YeTe_YHUL9ZsvW-Qd_F06iQ8,194
 mt/imageio/immview.py,sha256=PO7HjMIk1lybhp0a51ZbdIIER_cp7KWuBU4D2KpmJV8,3600
 mt/imageio/imread.py,sha256=q4kobqEFSi5uge0d0Flo5daf7_PwmXbK_LKgfvzD-rA,10139
-mt/imageio/imwrite.py,sha256=HhzA-iEaN5LcKVDwgwxdjRLdVaUJESaM39V8D9agwjg,7561
-mt/imageio/version.py,sha256=p-PR3aYnN1aE2vJo5YydR45sekEtPW-e4oX-79qLQ34,396
-mtimageio-0.3.202304290650.data/scripts/immview,sha256=5N4zFtr2NtR2p23VWEWCRq2s3asG50R4FxHM3dfoP2o,1003
-mtimageio-0.3.202304290650.dist-info/LICENSE,sha256=k16lM0fLB6Uu6qiyvogvT22QGfqaJSE7PmVWdXm452A,1500
-mtimageio-0.3.202304290650.dist-info/METADATA,sha256=pp-HOloXEe-e03q1bBV43NMT6Nd1vbhUJAT2Jm2mxIg,290
-mtimageio-0.3.202304290650.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mtimageio-0.3.202304290650.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
-mtimageio-0.3.202304290650.dist-info/RECORD,,
+mt/imageio/imwrite.py,sha256=qlz4YYnPEl7kw_u5bYyDwacbaVClL2qg2VU5vISVyVE,7734
+mt/imageio/version.py,sha256=Q8uBRVc09vCe9JXortZY4_i4RUxEeBkpnL2M1WA6wGc,396
+mtimageio-0.3.202304300605.data/scripts/immview,sha256=5N4zFtr2NtR2p23VWEWCRq2s3asG50R4FxHM3dfoP2o,1003
+mtimageio-0.3.202304300605.dist-info/LICENSE,sha256=k16lM0fLB6Uu6qiyvogvT22QGfqaJSE7PmVWdXm452A,1500
+mtimageio-0.3.202304300605.dist-info/METADATA,sha256=BBiUFrkIc8x42IbHcOFDj1DhMvmQF9-Wpu_9szxvdvA,290
+mtimageio-0.3.202304300605.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+mtimageio-0.3.202304300605.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
+mtimageio-0.3.202304300605.dist-info/RECORD,,
```

