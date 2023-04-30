# Comparing `tmp/django-ffmpeg-0.1.6.tar.gz` & `tmp/django-ffmpeg-0.1.7.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-ffmpeg-0.1.6.tar", last modified: Thu Dec  2 06:46:23 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

