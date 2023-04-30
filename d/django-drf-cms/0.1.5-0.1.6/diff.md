# Comparing `tmp/django-drf-cms-0.1.5.tar.gz` & `tmp/django-drf-cms-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-drf-cms-0.1.5.tar", last modified: Sun Apr 30 10:32:12 2023, max compression
+gzip compressed data, was "django-drf-cms-0.1.6.tar", last modified: Sun Apr 30 10:37:42 2023, max compression
```

## Comparing `django-drf-cms-0.1.5.tar` & `django-drf-cms-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-30 10:32:12.437902 django-drf-cms-0.1.5/
--rw-r--r--   0 luis       (501) staff       (20)    10936 2023-04-28 16:21:49.000000 django-drf-cms-0.1.5/LICENSE
--rw-r--r--   0 luis       (501) staff       (20)       59 2023-04-28 16:22:53.000000 django-drf-cms-0.1.5/MANIFEST.in
--rw-r--r--   0 luis       (501) staff       (20)     1426 2023-04-30 10:32:12.438022 django-drf-cms-0.1.5/PKG-INFO
--rw-r--r--   0 luis       (501) staff       (20)      525 2023-04-28 18:09:25.000000 django-drf-cms-0.1.5/README.rst
-drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-30 10:32:12.432027 django-drf-cms-0.1.5/django_drf_cms.egg-info/
--rw-r--r--   0 luis       (501) staff       (20)     1426 2023-04-30 10:32:12.000000 django-drf-cms-0.1.5/django_drf_cms.egg-info/PKG-INFO
--rw-r--r--   0 luis       (501) staff       (20)      722 2023-04-30 10:32:12.000000 django-drf-cms-0.1.5/django_drf_cms.egg-info/SOURCES.txt
--rw-r--r--   0 luis       (501) staff       (20)        1 2023-04-30 10:32:12.000000 django-drf-cms-0.1.5/django_drf_cms.egg-info/dependency_links.txt
--rw-r--r--   0 luis       (501) staff       (20)      117 2023-04-30 10:32:12.000000 django-drf-cms-0.1.5/django_drf_cms.egg-info/requires.txt
--rw-r--r--   0 luis       (501) staff       (20)        8 2023-04-30 10:32:12.000000 django-drf-cms-0.1.5/django_drf_cms.egg-info/top_level.txt
-drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-30 10:32:12.436549 django-drf-cms-0.1.5/drf_cms/
--rw-r--r--   0 luis       (501) staff       (20)        0 2023-04-25 16:49:24.000000 django-drf-cms-0.1.5/drf_cms/__init__.py
--rw-r--r--   0 luis       (501) staff       (20)      811 2023-04-30 09:30:04.000000 django-drf-cms-0.1.5/drf_cms/admin.py
--rw-r--r--   0 luis       (501) staff       (20)      146 2023-04-28 08:58:59.000000 django-drf-cms-0.1.5/drf_cms/apps.py
--rw-r--r--   0 luis       (501) staff       (20)      401 2023-04-30 09:30:40.000000 django-drf-cms-0.1.5/drf_cms/forms.py
-drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-30 10:32:12.437739 django-drf-cms-0.1.5/drf_cms/migrations/
--rw-r--r--   0 luis       (501) staff       (20)     1589 2023-04-28 08:59:14.000000 django-drf-cms-0.1.5/drf_cms/migrations/0001_initial.py
--rw-r--r--   0 luis       (501) staff       (20)      434 2023-04-28 08:59:28.000000 django-drf-cms-0.1.5/drf_cms/migrations/0002_alter_text_unique_together_remove_text_site.py
--rw-r--r--   0 luis       (501) staff       (20)     1302 2023-04-28 08:59:32.000000 django-drf-cms-0.1.5/drf_cms/migrations/0003_page_description_en_page_description_es_and_more.py
--rw-r--r--   0 luis       (501) staff       (20)        0 2023-04-25 16:49:24.000000 django-drf-cms-0.1.5/drf_cms/migrations/__init__.py
--rw-r--r--   0 luis       (501) staff       (20)     1506 2023-04-30 09:53:58.000000 django-drf-cms-0.1.5/drf_cms/models.py
--rw-r--r--   0 luis       (501) staff       (20)      657 2023-04-28 17:17:06.000000 django-drf-cms-0.1.5/drf_cms/permissions.py
--rw-r--r--   0 luis       (501) staff       (20)     1582 2023-04-30 09:35:59.000000 django-drf-cms-0.1.5/drf_cms/serializers.py
--rw-r--r--   0 luis       (501) staff       (20)      155 2023-04-28 17:14:19.000000 django-drf-cms-0.1.5/drf_cms/shortcuts.py
--rw-r--r--   0 luis       (501) staff       (20)     1448 2023-04-30 09:28:08.000000 django-drf-cms-0.1.5/drf_cms/storage_backends.py
--rw-r--r--   0 luis       (501) staff       (20)       60 2023-04-25 16:49:24.000000 django-drf-cms-0.1.5/drf_cms/tests.py
--rw-r--r--   0 luis       (501) staff       (20)      302 2023-04-27 09:47:04.000000 django-drf-cms-0.1.5/drf_cms/translation.py
--rw-r--r--   0 luis       (501) staff       (20)      574 2023-04-30 09:34:39.000000 django-drf-cms-0.1.5/drf_cms/urls.py
--rw-r--r--   0 luis       (501) staff       (20)     3600 2023-04-30 09:35:36.000000 django-drf-cms-0.1.5/drf_cms/views.py
--rw-r--r--   0 luis       (501) staff       (20)      108 2023-04-28 09:01:41.000000 django-drf-cms-0.1.5/pyproject.toml
--rw-r--r--   0 luis       (501) staff       (20)     1020 2023-04-30 10:32:12.438497 django-drf-cms-0.1.5/setup.cfg
--rw-r--r--   0 luis       (501) staff       (20)       37 2023-04-28 09:16:43.000000 django-drf-cms-0.1.5/setup.py
+drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-30 10:37:42.021761 django-drf-cms-0.1.6/
+-rw-r--r--   0 luis       (501) staff       (20)    10936 2023-04-28 16:21:49.000000 django-drf-cms-0.1.6/LICENSE
+-rw-r--r--   0 luis       (501) staff       (20)       59 2023-04-28 16:22:53.000000 django-drf-cms-0.1.6/MANIFEST.in
+-rw-r--r--   0 luis       (501) staff       (20)     1426 2023-04-30 10:37:42.021901 django-drf-cms-0.1.6/PKG-INFO
+-rw-r--r--   0 luis       (501) staff       (20)      525 2023-04-28 18:09:25.000000 django-drf-cms-0.1.6/README.rst
+drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-30 10:37:42.016413 django-drf-cms-0.1.6/django_drf_cms.egg-info/
+-rw-r--r--   0 luis       (501) staff       (20)     1426 2023-04-30 10:37:41.000000 django-drf-cms-0.1.6/django_drf_cms.egg-info/PKG-INFO
+-rw-r--r--   0 luis       (501) staff       (20)      722 2023-04-30 10:37:41.000000 django-drf-cms-0.1.6/django_drf_cms.egg-info/SOURCES.txt
+-rw-r--r--   0 luis       (501) staff       (20)        1 2023-04-30 10:37:41.000000 django-drf-cms-0.1.6/django_drf_cms.egg-info/dependency_links.txt
+-rw-r--r--   0 luis       (501) staff       (20)      117 2023-04-30 10:37:41.000000 django-drf-cms-0.1.6/django_drf_cms.egg-info/requires.txt
+-rw-r--r--   0 luis       (501) staff       (20)        8 2023-04-30 10:37:41.000000 django-drf-cms-0.1.6/django_drf_cms.egg-info/top_level.txt
+drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-30 10:37:42.020350 django-drf-cms-0.1.6/drf_cms/
+-rw-r--r--   0 luis       (501) staff       (20)        0 2023-04-25 16:49:24.000000 django-drf-cms-0.1.6/drf_cms/__init__.py
+-rw-r--r--   0 luis       (501) staff       (20)      811 2023-04-30 09:30:04.000000 django-drf-cms-0.1.6/drf_cms/admin.py
+-rw-r--r--   0 luis       (501) staff       (20)      146 2023-04-28 08:58:59.000000 django-drf-cms-0.1.6/drf_cms/apps.py
+-rw-r--r--   0 luis       (501) staff       (20)      401 2023-04-30 09:30:40.000000 django-drf-cms-0.1.6/drf_cms/forms.py
+drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-30 10:37:42.021572 django-drf-cms-0.1.6/drf_cms/migrations/
+-rw-r--r--   0 luis       (501) staff       (20)     1589 2023-04-28 08:59:14.000000 django-drf-cms-0.1.6/drf_cms/migrations/0001_initial.py
+-rw-r--r--   0 luis       (501) staff       (20)      434 2023-04-28 08:59:28.000000 django-drf-cms-0.1.6/drf_cms/migrations/0002_alter_text_unique_together_remove_text_site.py
+-rw-r--r--   0 luis       (501) staff       (20)     1302 2023-04-28 08:59:32.000000 django-drf-cms-0.1.6/drf_cms/migrations/0003_page_description_en_page_description_es_and_more.py
+-rw-r--r--   0 luis       (501) staff       (20)        0 2023-04-25 16:49:24.000000 django-drf-cms-0.1.6/drf_cms/migrations/__init__.py
+-rw-r--r--   0 luis       (501) staff       (20)     1506 2023-04-30 10:37:11.000000 django-drf-cms-0.1.6/drf_cms/models.py
+-rw-r--r--   0 luis       (501) staff       (20)      657 2023-04-28 17:17:06.000000 django-drf-cms-0.1.6/drf_cms/permissions.py
+-rw-r--r--   0 luis       (501) staff       (20)     1582 2023-04-30 09:35:59.000000 django-drf-cms-0.1.6/drf_cms/serializers.py
+-rw-r--r--   0 luis       (501) staff       (20)      155 2023-04-28 17:14:19.000000 django-drf-cms-0.1.6/drf_cms/shortcuts.py
+-rw-r--r--   0 luis       (501) staff       (20)     1448 2023-04-30 09:28:08.000000 django-drf-cms-0.1.6/drf_cms/storage_backends.py
+-rw-r--r--   0 luis       (501) staff       (20)       60 2023-04-25 16:49:24.000000 django-drf-cms-0.1.6/drf_cms/tests.py
+-rw-r--r--   0 luis       (501) staff       (20)      302 2023-04-27 09:47:04.000000 django-drf-cms-0.1.6/drf_cms/translation.py
+-rw-r--r--   0 luis       (501) staff       (20)      574 2023-04-30 09:34:39.000000 django-drf-cms-0.1.6/drf_cms/urls.py
+-rw-r--r--   0 luis       (501) staff       (20)     3600 2023-04-30 09:35:36.000000 django-drf-cms-0.1.6/drf_cms/views.py
+-rw-r--r--   0 luis       (501) staff       (20)      108 2023-04-28 09:01:41.000000 django-drf-cms-0.1.6/pyproject.toml
+-rw-r--r--   0 luis       (501) staff       (20)     1020 2023-04-30 10:37:42.022434 django-drf-cms-0.1.6/setup.cfg
+-rw-r--r--   0 luis       (501) staff       (20)       37 2023-04-28 09:16:43.000000 django-drf-cms-0.1.6/setup.py
```

### Comparing `django-drf-cms-0.1.5/LICENSE` & `django-drf-cms-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.5/PKG-INFO` & `django-drf-cms-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-drf-cms
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Django app to build a simple cms restful server.
 Home-page: https://www.spartanbits.com
 Author: Spartanbits, SLU
 Author-email: info@spartanbits.com
 License: Apache-2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-drf-cms-0.1.5/README.rst` & `django-drf-cms-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.5/django_drf_cms.egg-info/PKG-INFO` & `django-drf-cms-0.1.6/django_drf_cms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-drf-cms
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Django app to build a simple cms restful server.
 Home-page: https://www.spartanbits.com
 Author: Spartanbits, SLU
 Author-email: info@spartanbits.com
 License: Apache-2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-drf-cms-0.1.5/django_drf_cms.egg-info/SOURCES.txt` & `django-drf-cms-0.1.6/django_drf_cms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.5/drf_cms/admin.py` & `django-drf-cms-0.1.6/drf_cms/admin.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.5/drf_cms/migrations/0001_initial.py` & `django-drf-cms-0.1.6/drf_cms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.5/drf_cms/migrations/0003_page_description_en_page_description_es_and_more.py` & `django-drf-cms-0.1.6/drf_cms/migrations/0003_page_description_en_page_description_es_and_more.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.5/drf_cms/models.py` & `django-drf-cms-0.1.6/drf_cms/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 from django.db import models
 from django_bleach.models import BleachField
 from django.contrib.sites.models import Site
 
 
+class Page(models.Model):
+	site = models.ForeignKey(Site, null=False, on_delete=models.CASCADE)
+	key = models.CharField(null=False, max_length=64)
+	title = models.CharField(null=False, max_length=128)
+	description = models.CharField(blank=True, max_length=256)
+
+	class Meta:
+		unique_together = ('site', 'key')
+
+	def __str__(self):
+		return '{} - {}'.format(self.key, self.site.domain)
+
+
 class ContentMixin(models.Model):
 	page = models.ForeignKey(Page, null=False, on_delete=models.CASCADE)
 	key = models.CharField(null=False, max_length=64)
 
 	class Meta:
 		unique_together = ('page', 'key')
 
@@ -28,27 +41,14 @@
 	width = models.PositiveIntegerField(default=0)
 
 
 class FileData(MetadataMixin):
 	file = models.FileField()
 
 
-class Page(models.Model):
-	site = models.ForeignKey(Site, null=False, on_delete=models.CASCADE)
-	key = models.CharField(null=False, max_length=64)
-	title = models.CharField(null=False, max_length=128)
-	description = models.CharField(blank=True, max_length=256)
-
-	class Meta:
-		unique_together = ('site', 'key')
-
-	def __str__(self):
-		return '{} - {}'.format(self.key, self.site.domain)
-
-
 class Text(ContentMixin):
 	content = BleachField(null=False, allowed_tags=['a', 'p', 'i', 'b', 'u'], allowed_attributes=['href'])
 
 
 class Image(ContentMixin):
 	content = models.ForeignKey(ImageData, null=False)
```

### Comparing `django-drf-cms-0.1.5/drf_cms/permissions.py` & `django-drf-cms-0.1.6/drf_cms/permissions.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.5/drf_cms/serializers.py` & `django-drf-cms-0.1.6/drf_cms/serializers.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.5/drf_cms/storage_backends.py` & `django-drf-cms-0.1.6/drf_cms/storage_backends.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.5/drf_cms/urls.py` & `django-drf-cms-0.1.6/drf_cms/urls.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.5/drf_cms/views.py` & `django-drf-cms-0.1.6/drf_cms/views.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.5/setup.cfg` & `django-drf-cms-0.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-drf-cms
-version = 0.1.5
+version = 0.1.6
 description = A Django app to build a simple cms restful server.
 long_description = file: README.rst
 url = https://www.spartanbits.com
 author = Spartanbits, SLU
 author_email = info@spartanbits.com
 license = Apache-2.0
 classifiers =
```

