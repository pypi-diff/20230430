# Comparing `tmp/pyascore-0.7.0b0.tar.gz` & `tmp/pyascore-1.0.0b1-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pyAscore/pyAscore/dist/tmp8rvu25bz/pyascore-0.7.0b0.tar", last modified: Sun Apr 24 20:56:11 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

