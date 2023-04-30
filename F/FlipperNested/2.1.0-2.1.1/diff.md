# Comparing `tmp/FlipperNested-2.1.0.tar.gz` & `tmp/FlipperNested-2.1.1-cp311-cp311-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlipperNested-2.1.0.tar", last modified: Thu Apr 27 23:47:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

