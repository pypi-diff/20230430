# Comparing `tmp/tinyusdz-0.8.0rc1.tar.gz` & `tmp/tinyusdz-0.8.0rc4-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyusdz-0.8.0rc1.tar", last modified: Wed Apr 19 11:05:02 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

