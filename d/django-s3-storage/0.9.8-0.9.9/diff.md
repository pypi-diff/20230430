# Comparing `tmp/django-s3-storage-0.9.8.tar.gz` & `tmp/django-s3-storage-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-s3-storage-0.9.8.tar", last modified: Thu Dec 17 16:31:26 2015, max compression
+gzip compressed data, was "dist/django-s3-storage-0.9.9.tar", last modified: Fri Jun 24 13:11:39 2016, max compression
```

## Comparing `django-s3-storage-0.9.8.tar` & `django-s3-storage-0.9.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2015-12-17 16:31:26.000000 django-s3-storage-0.9.8/
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2015-12-17 16:31:26.000000 django-s3-storage-0.9.8/django_s3_storage/
--rw-r--r--   0 dave       (501) staff       (20)       65 2015-12-17 16:31:09.000000 django-s3-storage-0.9.8/django_s3_storage/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)     2973 2015-12-17 15:39:49.000000 django-s3-storage-0.9.8/django_s3_storage/conf.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2015-12-17 16:31:26.000000 django-s3-storage-0.9.8/django_s3_storage/management/
--rw-r--r--   0 dave       (501) staff       (20)        0 2015-09-04 13:14:55.000000 django-s3-storage-0.9.8/django_s3_storage/management/__init__.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2015-12-17 16:31:26.000000 django-s3-storage-0.9.8/django_s3_storage/management/commands/
--rw-r--r--   0 dave       (501) staff       (20)        0 2015-09-04 13:14:55.000000 django-s3-storage-0.9.8/django_s3_storage/management/commands/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)      914 2015-09-04 13:14:55.000000 django-s3-storage-0.9.8/django_s3_storage/management/commands/s3_sync_meta.py
--rw-r--r--   0 dave       (501) staff       (20)    16055 2015-12-17 16:10:54.000000 django-s3-storage-0.9.8/django_s3_storage/storage.py
--rw-r--r--   0 dave       (501) staff       (20)    12745 2015-12-17 16:19:38.000000 django-s3-storage-0.9.8/django_s3_storage/tests.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2015-12-17 16:31:26.000000 django-s3-storage-0.9.8/django_s3_storage.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)        1 2015-12-17 16:31:26.000000 django-s3-storage-0.9.8/django_s3_storage.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)      711 2015-12-17 16:31:26.000000 django-s3-storage-0.9.8/django_s3_storage.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)       49 2015-12-17 16:31:26.000000 django-s3-storage-0.9.8/django_s3_storage.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)      500 2015-12-17 16:31:26.000000 django-s3-storage-0.9.8/django_s3_storage.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)       18 2015-12-17 16:31:26.000000 django-s3-storage-0.9.8/django_s3_storage.egg-info/top_level.txt
--rw-r--r--   0 dave       (501) staff       (20)     1524 2015-01-15 15:23:03.000000 django-s3-storage-0.9.8/LICENSE
--rw-r--r--   0 dave       (501) staff       (20)       35 2015-01-15 15:23:03.000000 django-s3-storage-0.9.8/MANIFEST.in
--rw-r--r--   0 dave       (501) staff       (20)      711 2015-12-17 16:31:26.000000 django-s3-storage-0.9.8/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)     7257 2015-12-17 16:22:19.000000 django-s3-storage-0.9.8/README.rst
--rw-r--r--   0 dave       (501) staff       (20)       59 2015-12-17 16:31:26.000000 django-s3-storage-0.9.8/setup.cfg
--rw-r--r--   0 dave       (501) staff       (20)     1093 2015-08-28 15:43:33.000000 django-s3-storage-0.9.8/setup.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2016-06-24 13:11:39.000000 django-s3-storage-0.9.9/
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2016-06-24 13:11:39.000000 django-s3-storage-0.9.9/django_s3_storage/
+-rw-r--r--   0 dave       (501) staff       (20)       65 2016-06-24 09:14:40.000000 django-s3-storage-0.9.9/django_s3_storage/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)     3168 2016-06-24 09:04:17.000000 django-s3-storage-0.9.9/django_s3_storage/conf.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2016-06-24 13:11:39.000000 django-s3-storage-0.9.9/django_s3_storage/management/
+-rw-r--r--   0 dave       (501) staff       (20)        0 2015-09-04 13:14:55.000000 django-s3-storage-0.9.9/django_s3_storage/management/__init__.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2016-06-24 13:11:39.000000 django-s3-storage-0.9.9/django_s3_storage/management/commands/
+-rw-r--r--   0 dave       (501) staff       (20)        0 2015-09-04 13:14:55.000000 django-s3-storage-0.9.9/django_s3_storage/management/commands/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)      914 2015-09-04 13:14:55.000000 django-s3-storage-0.9.9/django_s3_storage/management/commands/s3_sync_meta.py
+-rw-r--r--   0 dave       (501) staff       (20)    16670 2016-06-24 09:04:17.000000 django-s3-storage-0.9.9/django_s3_storage/storage.py
+-rw-r--r--   0 dave       (501) staff       (20)    13424 2016-06-24 09:04:17.000000 django-s3-storage-0.9.9/django_s3_storage/tests.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2016-06-24 13:11:39.000000 django-s3-storage-0.9.9/django_s3_storage.egg-info/
+-rw-r--r--   0 dave       (501) staff       (20)        1 2016-06-24 13:11:39.000000 django-s3-storage-0.9.9/django_s3_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 dave       (501) staff       (20)      711 2016-06-24 13:11:39.000000 django-s3-storage-0.9.9/django_s3_storage.egg-info/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)       49 2016-06-24 13:11:39.000000 django-s3-storage-0.9.9/django_s3_storage.egg-info/requires.txt
+-rw-r--r--   0 dave       (501) staff       (20)      500 2016-06-24 13:11:39.000000 django-s3-storage-0.9.9/django_s3_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 dave       (501) staff       (20)       18 2016-06-24 13:11:39.000000 django-s3-storage-0.9.9/django_s3_storage.egg-info/top_level.txt
+-rw-r--r--   0 dave       (501) staff       (20)     1524 2015-01-15 15:23:03.000000 django-s3-storage-0.9.9/LICENSE
+-rw-r--r--   0 dave       (501) staff       (20)       35 2015-01-15 15:23:03.000000 django-s3-storage-0.9.9/MANIFEST.in
+-rw-r--r--   0 dave       (501) staff       (20)      711 2016-06-24 13:11:39.000000 django-s3-storage-0.9.9/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)     7432 2016-06-24 09:04:17.000000 django-s3-storage-0.9.9/README.rst
+-rw-r--r--   0 dave       (501) staff       (20)       59 2016-06-24 13:11:39.000000 django-s3-storage-0.9.9/setup.cfg
+-rw-r--r--   0 dave       (501) staff       (20)     1093 2015-08-28 15:43:33.000000 django-s3-storage-0.9.9/setup.py
```

### Comparing `django-s3-storage-0.9.8/django_s3_storage/conf.py` & `django-s3-storage-0.9.9/django_s3_storage/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,14 +86,19 @@
     )
 
     AWS_S3_METADATA = LazySetting(
         name = "AWS_S3_METADATA",
         default = {},
     )
 
+    AWS_S3_GZIP = LazySetting(
+        name = "AWS_S3_GZIP",
+        default = True
+    )
+
     # Static storage config.
 
     AWS_S3_BUCKET_NAME_STATIC = LazySetting(
         name = "AWS_S3_BUCKET_NAME_STATIC",
     )
 
     AWS_S3_CALLING_FORMAT_STATIC = LazySetting(
@@ -128,10 +133,14 @@
     )
 
     AWS_S3_METADATA_STATIC = LazySetting(
         name = "AWS_S3_METADATA_STATIC",
         default = {},
     )
 
+    AWS_S3_GZIP_STATIC = LazySetting(
+        name = "AWS_S3_GZIP_STATIC",
+        default = True
+    )
 
 
 settings = LazySettings(settings)
```

### Comparing `django-s3-storage-0.9.8/django_s3_storage/management/commands/s3_sync_meta.py` & `django-s3-storage-0.9.9/django_s3_storage/management/commands/s3_sync_meta.py`

 * *Files identical despite different names*

### Comparing `django-s3-storage-0.9.8/django_s3_storage/storage.py` & `django-s3-storage-0.9.9/django_s3_storage/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import unicode_literals
 
-import posixpath, datetime, mimetypes, gzip
+import posixpath, datetime, mimetypes, gzip, os
 from io import TextIOBase
 from email.utils import parsedate_tz
 from contextlib import closing, contextmanager
 from tempfile import SpooledTemporaryFile
 
 from boto import s3
 from boto.s3.connection import S3ResponseError
@@ -30,27 +30,28 @@
     """
     An implementation of Django file storage over S3.
 
     It would be nice to use django-storages for this, but it doesn't support
     Python 3, which is kinda lame.
     """
 
-    def __init__(self, aws_region=None, aws_access_key_id=None, aws_secret_access_key=None, aws_s3_bucket_name=None, aws_s3_calling_format=None, aws_s3_key_prefix=None, aws_s3_bucket_auth=None, aws_s3_max_age_seconds=None, aws_s3_public_url=None, aws_s3_reduced_redundancy=False, aws_s3_host=None, aws_s3_metadata=None):
+    def __init__(self, aws_region=None, aws_access_key_id=None, aws_secret_access_key=None, aws_s3_bucket_name=None, aws_s3_calling_format=None, aws_s3_key_prefix=None, aws_s3_bucket_auth=None, aws_s3_max_age_seconds=None, aws_s3_public_url=None, aws_s3_reduced_redundancy=False, aws_s3_host=None, aws_s3_metadata=None, aws_s3_gzip=None):
         self.aws_region = settings.AWS_REGION if aws_region is None else aws_region
         self.aws_access_key_id = settings.AWS_ACCESS_KEY_ID if aws_access_key_id is None else aws_access_key_id
         self.aws_secret_access_key = settings.AWS_SECRET_ACCESS_KEY if aws_secret_access_key is None else aws_secret_access_key
         self.aws_s3_bucket_name = settings.AWS_S3_BUCKET_NAME if aws_s3_bucket_name is None else aws_s3_bucket_name
         self.aws_s3_calling_format = settings.AWS_S3_CALLING_FORMAT if aws_s3_calling_format is None else aws_s3_calling_format
         self.aws_s3_key_prefix = settings.AWS_S3_KEY_PREFIX if aws_s3_key_prefix is None else aws_s3_key_prefix
         self.aws_s3_bucket_auth = settings.AWS_S3_BUCKET_AUTH if aws_s3_bucket_auth is None else aws_s3_bucket_auth
         self.aws_s3_max_age_seconds = settings.AWS_S3_MAX_AGE_SECONDS if aws_s3_max_age_seconds is None else aws_s3_max_age_seconds
         self.aws_s3_public_url = settings.AWS_S3_PUBLIC_URL if aws_s3_public_url is None else aws_s3_public_url
         self.aws_s3_reduced_redundancy = settings.AWS_S3_REDUCED_REDUNDANCY if aws_s3_reduced_redundancy is None else aws_s3_reduced_redundancy
         self.aws_s3_host = settings.AWS_S3_HOST if aws_s3_host is None else aws_s3_host
         self.aws_s3_metadata = settings.AWS_S3_METADATA if aws_s3_metadata is None else aws_s3_metadata
+        self.aws_s3_gzip = settings.AWS_S3_GZIP if aws_s3_gzip is None else aws_s3_gzip
         # Validate args.
         if self.aws_s3_public_url and self.aws_s3_bucket_auth:
             raise ImproperlyConfigured("Cannot use AWS_S3_BUCKET_AUTH with AWS_S3_PUBLIC_URL.")
         # Connect to S3.
         connection_kwargs = {
             "calling_format": self.aws_s3_calling_format,
         }
@@ -131,15 +132,15 @@
         Attempts to compress the given file.
 
         If the file is larger when compressed, returns the original
         file.
 
         Returns a tuple of (content_encoding, content).
         """
-        if content_encoding == CONTENT_ENCODING_GZIP:
+        if self.aws_s3_gzip and content_encoding == CONTENT_ENCODING_GZIP:
             # Ideally, we would do some sort of incremental compression here,
             # but boto doesn't support uploading a key from an iterator.
             with self._temporary_file() as temp_file:
                 with closing(gzip.GzipFile(name, "wb", 9, temp_file)) as zipfile:
                     for chunk in content.chunks():
                         zipfile.write(chunk)
                 # Check if the zipped version is actually smaller!
@@ -169,15 +170,21 @@
         with self._conditional_convert_content_to_bytes(name, content) as content:
             # Attempt content compression.
             with self._conditional_compress_file(name, content, content_encoding) as (content, content_encoding):
                 # Return the calculated headers and file.
                 yield content, content_type, content_encoding,
 
     def _get_key_name(self, name):
-        return posixpath.join(self.aws_s3_key_prefix, name)
+        """
+        Builds the key name we use to fetch this file form s3
+
+        Normalises the path at the end as name can be a relative url
+        """
+        name = posixpath.join(self.aws_s3_key_prefix, name.replace(os.sep, "/"))
+        return posixpath.normpath(name)
 
     def _generate_url(self, name):
         """
         Generates a URL to the given file.
 
         Authenticated storage will return a signed URL. Non-authenticated
         storage will return an unsigned URL, which aids in browser caching.
@@ -255,15 +262,19 @@
         self._get_key(name).delete()
 
     def exists(self, name):
         """
         Returns True if a file referenced by the given name already exists in the
         storage system, or False if the name is available for a new file.
         """
-        return self._get_key(name).exists()
+        # We also need to check for directory existence, so we'll list matching
+        # keys and return success if any match.
+        for _ in self.bucket.list(prefix=self._get_key_name(name)):
+            return True
+        return False
 
     def listdir(self, path):
         """
         Lists the contents of the specified path, returning a 2-tuple of lists;
         the first item being directories, the second item being files.
         """
         path = self._get_key_name(path)
@@ -384,13 +395,14 @@
         kwargs.setdefault("aws_s3_key_prefix", settings.AWS_S3_KEY_PREFIX_STATIC)
         kwargs.setdefault("aws_s3_bucket_auth", settings.AWS_S3_BUCKET_AUTH_STATIC)
         kwargs.setdefault("aws_s3_max_age_seconds", settings.AWS_S3_MAX_AGE_SECONDS_STATIC)
         kwargs.setdefault("aws_s3_public_url", settings.AWS_S3_PUBLIC_URL_STATIC)
         kwargs.setdefault("aws_s3_reduced_redundancy", settings.AWS_S3_REDUCED_REDUNDANCY_STATIC)
         kwargs.setdefault("aws_s3_host", settings.AWS_S3_HOST_STATIC)
         kwargs.setdefault("aws_s3_metadata", settings.AWS_S3_METADATA_STATIC)
+        kwargs.setdefault("aws_s3_gzip", settings.AWS_S3_GZIP_STATIC)
         super(StaticS3Storage, self).__init__(**kwargs)
 
 
 class ManifestStaticS3Storage(ManifestFilesMixin, StaticS3Storage):
 
     pass
```

### Comparing `django-s3-storage-0.9.8/django_s3_storage/tests.py` & `django-s3-storage-0.9.9/django_s3_storage/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,17 @@
         finally:
             self.storage.delete(upload_path)
 
     def testExists(self):
         self.assertTrue(self.storage.exists(self.upload_path))
         self.assertFalse(self.storage.exists(self.generateUploadPath()))
 
+    def testDirExists(self):
+        self.assertTrue(self.storage.exists(""))
+
     def testDelete(self):
         # Make a new file to delete.
         upload_path = self.generateUploadPath()
         self.saveTestFile(upload_path)
         self.assertTrue(self.storage.exists(upload_path))
         # Delete the file.
         self.storage.delete(upload_path)
@@ -241,16 +244,29 @@
             response = self.assertUrlAccessible(url)
             self.assertEqual(response.headers["content-disposition"], "attachment;filename={}".format(posixpath.basename(upload_path)))
             self.assertEqual(response.headers["content-language"], "fr")
         finally:
             # Clean up the test file.
             self.storage.delete(upload_path)
 
-    # Syncing meta information.
+    def testUploadWithRelativePath(self):
+        upload_path = self.generateUploadBasename()
+        relative_upload_path = './%s' % upload_path
+        self.saveTestFile(upload_path=relative_upload_path)
+        try:
+            self.assertTrue(self.storage.exists(relative_upload_path))
+            url = self.storage.url(relative_upload_path)
+            # Ensure that the URL is accessible.
+            self.assertNotIn(relative_upload_path, url)
+            self.assertIn(upload_path, url)
+            self.assertUrlAccessible(url)
+        finally:
+            self.storage.delete(upload_path)
 
+    # Syncing meta information.
     def testSyncMetaPrivateToPublic(self):
         url = self.insecure_storage.url(self.upload_path)
         self.assertUrlInaccessible(url)
         # Sync the meta to insecure storage.
         self.insecure_storage.sync_meta()
         time.sleep(0.2)  # Give it a chance to propagate over S3.
         # URL is now accessible and well-cached.
```

### Comparing `django-s3-storage-0.9.8/django_s3_storage.egg-info/PKG-INFO` & `django-s3-storage-0.9.9/django_s3_storage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-s3-storage
-Version: 0.9.8
+Version: 0.9.9
 Summary: Django Amazon S3 file storage.
 Home-page: https://github.com/etianen/django-s3-storage
 Author: Dave Hall
 Author-email: dave@etianen.com
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-s3-storage-0.9.8/LICENSE` & `django-s3-storage-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-s3-storage-0.9.8/PKG-INFO` & `django-s3-storage-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-s3-storage
-Version: 0.9.8
+Version: 0.9.9
 Summary: Django Amazon S3 file storage.
 Home-page: https://github.com/etianen/django-s3-storage
 Author: Dave Hall
 Author-email: dave@etianen.com
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-s3-storage-0.9.8/README.rst` & `django-s3-storage-0.9.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,17 @@
     # Whether to set the storage class of uploaded files to REDUCED_REDUNDANCY.
     AWS_S3_REDUCED_REDUNDANCY = False
 
     # A dictionary of additional metadata to set on the uploaded files.
     # If the value is a callable, it will be called with the path of the file on S3.
     AWS_S3_METADATA = {}
 
+    # Whether to enable gzip compression for uploaded files.
+    AWS_S3_GZIP = True
+
     # The S3 bucket used to store static files.
     AWS_S3_BUCKET_NAME_STATIC = ""
 
     # The S3 calling format to use to connect to the static bucket.
     AWS_S3_CALLING_FORMAT_STATIC = "boto.s3.connection.OrdinaryCallingFormat"
 
     # The host to connect to for static files (only needed if you are using a non-AWS host)
@@ -88,14 +91,17 @@
     # Whether to set the storage class of static files to REDUCED_REDUNDANCY.
     AWS_S3_REDUCED_REDUNDANCY_STATIC = False
 
     # A dictionary of additional metadata to set on the static files.
     # If the value is a callable, it will be called with the path of the file on S3.
     AWS_S3_METADATA_STATIC = {}
 
+    # Whether to enable gzip compression for static files.
+    AWS_S3_GZIP_STATIC = True
+
 
 **Important:** If you change any of the ``AWS_S3_BUCKET_AUTH`` or ``AWS_S3_MAX_AGE_SECONDS`` settings, you will need
 to run ``./manage.py s3_sync_meta path.to.your.storage`` before the changes will be applied to existing media files.
 
 
 How it works
 ------------
```

### Comparing `django-s3-storage-0.9.8/setup.py` & `django-s3-storage-0.9.9/setup.py`

 * *Files identical despite different names*

