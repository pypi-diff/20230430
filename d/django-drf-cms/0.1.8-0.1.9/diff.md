# Comparing `tmp/django-drf-cms-0.1.8.tar.gz` & `tmp/django-drf-cms-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-drf-cms-0.1.8.tar", last modified: Sun Apr 30 10:46:28 2023, max compression
+gzip compressed data, was "django-drf-cms-0.1.9.tar", last modified: Sun Apr 30 10:48:54 2023, max compression
```

## Comparing `django-drf-cms-0.1.8.tar` & `django-drf-cms-0.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-30 10:46:28.454087 django-drf-cms-0.1.8/
--rw-r--r--   0 luis       (501) staff       (20)    10936 2023-04-28 16:21:49.000000 django-drf-cms-0.1.8/LICENSE
--rw-r--r--   0 luis       (501) staff       (20)       59 2023-04-28 16:22:53.000000 django-drf-cms-0.1.8/MANIFEST.in
--rw-r--r--   0 luis       (501) staff       (20)     1426 2023-04-30 10:46:28.454210 django-drf-cms-0.1.8/PKG-INFO
--rw-r--r--   0 luis       (501) staff       (20)      525 2023-04-28 18:09:25.000000 django-drf-cms-0.1.8/README.rst
-drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-30 10:46:28.441552 django-drf-cms-0.1.8/django_drf_cms.egg-info/
--rw-r--r--   0 luis       (501) staff       (20)     1426 2023-04-30 10:46:28.000000 django-drf-cms-0.1.8/django_drf_cms.egg-info/PKG-INFO
--rw-r--r--   0 luis       (501) staff       (20)      722 2023-04-30 10:46:28.000000 django-drf-cms-0.1.8/django_drf_cms.egg-info/SOURCES.txt
--rw-r--r--   0 luis       (501) staff       (20)        1 2023-04-30 10:46:28.000000 django-drf-cms-0.1.8/django_drf_cms.egg-info/dependency_links.txt
--rw-r--r--   0 luis       (501) staff       (20)      117 2023-04-30 10:46:28.000000 django-drf-cms-0.1.8/django_drf_cms.egg-info/requires.txt
--rw-r--r--   0 luis       (501) staff       (20)        8 2023-04-30 10:46:28.000000 django-drf-cms-0.1.8/django_drf_cms.egg-info/top_level.txt
-drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-30 10:46:28.451270 django-drf-cms-0.1.8/drf_cms/
--rw-r--r--   0 luis       (501) staff       (20)        0 2023-04-25 16:49:24.000000 django-drf-cms-0.1.8/drf_cms/__init__.py
--rw-r--r--   0 luis       (501) staff       (20)      811 2023-04-30 09:30:04.000000 django-drf-cms-0.1.8/drf_cms/admin.py
--rw-r--r--   0 luis       (501) staff       (20)      146 2023-04-28 08:58:59.000000 django-drf-cms-0.1.8/drf_cms/apps.py
--rw-r--r--   0 luis       (501) staff       (20)      424 2023-04-30 10:44:35.000000 django-drf-cms-0.1.8/drf_cms/forms.py
-drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-30 10:46:28.453890 django-drf-cms-0.1.8/drf_cms/migrations/
--rw-r--r--   0 luis       (501) staff       (20)     1589 2023-04-28 08:59:14.000000 django-drf-cms-0.1.8/drf_cms/migrations/0001_initial.py
--rw-r--r--   0 luis       (501) staff       (20)      434 2023-04-28 08:59:28.000000 django-drf-cms-0.1.8/drf_cms/migrations/0002_alter_text_unique_together_remove_text_site.py
--rw-r--r--   0 luis       (501) staff       (20)     1302 2023-04-28 08:59:32.000000 django-drf-cms-0.1.8/drf_cms/migrations/0003_page_description_en_page_description_es_and_more.py
--rw-r--r--   0 luis       (501) staff       (20)        0 2023-04-25 16:49:24.000000 django-drf-cms-0.1.8/drf_cms/migrations/__init__.py
--rw-r--r--   0 luis       (501) staff       (20)     1558 2023-04-30 10:41:01.000000 django-drf-cms-0.1.8/drf_cms/models.py
--rw-r--r--   0 luis       (501) staff       (20)      657 2023-04-28 17:17:06.000000 django-drf-cms-0.1.8/drf_cms/permissions.py
--rw-r--r--   0 luis       (501) staff       (20)     1615 2023-04-30 10:45:05.000000 django-drf-cms-0.1.8/drf_cms/serializers.py
--rw-r--r--   0 luis       (501) staff       (20)      155 2023-04-28 17:14:19.000000 django-drf-cms-0.1.8/drf_cms/shortcuts.py
--rw-r--r--   0 luis       (501) staff       (20)     1448 2023-04-30 09:28:08.000000 django-drf-cms-0.1.8/drf_cms/storage_backends.py
--rw-r--r--   0 luis       (501) staff       (20)       60 2023-04-25 16:49:24.000000 django-drf-cms-0.1.8/drf_cms/tests.py
--rw-r--r--   0 luis       (501) staff       (20)      302 2023-04-27 09:47:04.000000 django-drf-cms-0.1.8/drf_cms/translation.py
--rw-r--r--   0 luis       (501) staff       (20)      574 2023-04-30 09:34:39.000000 django-drf-cms-0.1.8/drf_cms/urls.py
--rw-r--r--   0 luis       (501) staff       (20)     3628 2023-04-30 10:45:59.000000 django-drf-cms-0.1.8/drf_cms/views.py
--rw-r--r--   0 luis       (501) staff       (20)      108 2023-04-28 09:01:41.000000 django-drf-cms-0.1.8/pyproject.toml
--rw-r--r--   0 luis       (501) staff       (20)     1020 2023-04-30 10:46:28.454778 django-drf-cms-0.1.8/setup.cfg
--rw-r--r--   0 luis       (501) staff       (20)       37 2023-04-28 09:16:43.000000 django-drf-cms-0.1.8/setup.py
+drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-30 10:48:54.665316 django-drf-cms-0.1.9/
+-rw-r--r--   0 luis       (501) staff       (20)    10936 2023-04-28 16:21:49.000000 django-drf-cms-0.1.9/LICENSE
+-rw-r--r--   0 luis       (501) staff       (20)       59 2023-04-28 16:22:53.000000 django-drf-cms-0.1.9/MANIFEST.in
+-rw-r--r--   0 luis       (501) staff       (20)     1426 2023-04-30 10:48:54.665446 django-drf-cms-0.1.9/PKG-INFO
+-rw-r--r--   0 luis       (501) staff       (20)      525 2023-04-28 18:09:25.000000 django-drf-cms-0.1.9/README.rst
+drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-30 10:48:54.655594 django-drf-cms-0.1.9/django_drf_cms.egg-info/
+-rw-r--r--   0 luis       (501) staff       (20)     1426 2023-04-30 10:48:54.000000 django-drf-cms-0.1.9/django_drf_cms.egg-info/PKG-INFO
+-rw-r--r--   0 luis       (501) staff       (20)      722 2023-04-30 10:48:54.000000 django-drf-cms-0.1.9/django_drf_cms.egg-info/SOURCES.txt
+-rw-r--r--   0 luis       (501) staff       (20)        1 2023-04-30 10:48:54.000000 django-drf-cms-0.1.9/django_drf_cms.egg-info/dependency_links.txt
+-rw-r--r--   0 luis       (501) staff       (20)      133 2023-04-30 10:48:54.000000 django-drf-cms-0.1.9/django_drf_cms.egg-info/requires.txt
+-rw-r--r--   0 luis       (501) staff       (20)        8 2023-04-30 10:48:54.000000 django-drf-cms-0.1.9/django_drf_cms.egg-info/top_level.txt
+drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-30 10:48:54.662723 django-drf-cms-0.1.9/drf_cms/
+-rw-r--r--   0 luis       (501) staff       (20)        0 2023-04-25 16:49:24.000000 django-drf-cms-0.1.9/drf_cms/__init__.py
+-rw-r--r--   0 luis       (501) staff       (20)      811 2023-04-30 09:30:04.000000 django-drf-cms-0.1.9/drf_cms/admin.py
+-rw-r--r--   0 luis       (501) staff       (20)      146 2023-04-28 08:58:59.000000 django-drf-cms-0.1.9/drf_cms/apps.py
+-rw-r--r--   0 luis       (501) staff       (20)      424 2023-04-30 10:44:35.000000 django-drf-cms-0.1.9/drf_cms/forms.py
+drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-30 10:48:54.665079 django-drf-cms-0.1.9/drf_cms/migrations/
+-rw-r--r--   0 luis       (501) staff       (20)     1589 2023-04-28 08:59:14.000000 django-drf-cms-0.1.9/drf_cms/migrations/0001_initial.py
+-rw-r--r--   0 luis       (501) staff       (20)      434 2023-04-28 08:59:28.000000 django-drf-cms-0.1.9/drf_cms/migrations/0002_alter_text_unique_together_remove_text_site.py
+-rw-r--r--   0 luis       (501) staff       (20)     1302 2023-04-28 08:59:32.000000 django-drf-cms-0.1.9/drf_cms/migrations/0003_page_description_en_page_description_es_and_more.py
+-rw-r--r--   0 luis       (501) staff       (20)        0 2023-04-25 16:49:24.000000 django-drf-cms-0.1.9/drf_cms/migrations/__init__.py
+-rw-r--r--   0 luis       (501) staff       (20)     1558 2023-04-30 10:41:01.000000 django-drf-cms-0.1.9/drf_cms/models.py
+-rw-r--r--   0 luis       (501) staff       (20)      657 2023-04-28 17:17:06.000000 django-drf-cms-0.1.9/drf_cms/permissions.py
+-rw-r--r--   0 luis       (501) staff       (20)     1615 2023-04-30 10:45:05.000000 django-drf-cms-0.1.9/drf_cms/serializers.py
+-rw-r--r--   0 luis       (501) staff       (20)      155 2023-04-28 17:14:19.000000 django-drf-cms-0.1.9/drf_cms/shortcuts.py
+-rw-r--r--   0 luis       (501) staff       (20)     1448 2023-04-30 09:28:08.000000 django-drf-cms-0.1.9/drf_cms/storage_backends.py
+-rw-r--r--   0 luis       (501) staff       (20)       60 2023-04-25 16:49:24.000000 django-drf-cms-0.1.9/drf_cms/tests.py
+-rw-r--r--   0 luis       (501) staff       (20)      302 2023-04-27 09:47:04.000000 django-drf-cms-0.1.9/drf_cms/translation.py
+-rw-r--r--   0 luis       (501) staff       (20)      574 2023-04-30 09:34:39.000000 django-drf-cms-0.1.9/drf_cms/urls.py
+-rw-r--r--   0 luis       (501) staff       (20)     3628 2023-04-30 10:45:59.000000 django-drf-cms-0.1.9/drf_cms/views.py
+-rw-r--r--   0 luis       (501) staff       (20)      108 2023-04-28 09:01:41.000000 django-drf-cms-0.1.9/pyproject.toml
+-rw-r--r--   0 luis       (501) staff       (20)     1037 2023-04-30 10:48:54.665987 django-drf-cms-0.1.9/setup.cfg
+-rw-r--r--   0 luis       (501) staff       (20)       37 2023-04-28 09:16:43.000000 django-drf-cms-0.1.9/setup.py
```

### Comparing `django-drf-cms-0.1.8/LICENSE` & `django-drf-cms-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.8/PKG-INFO` & `django-drf-cms-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-drf-cms
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Django app to build a simple cms restful server.
 Home-page: https://www.spartanbits.com
 Author: Spartanbits, SLU
 Author-email: info@spartanbits.com
 License: Apache-2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-drf-cms-0.1.8/README.rst` & `django-drf-cms-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.8/django_drf_cms.egg-info/PKG-INFO` & `django-drf-cms-0.1.9/django_drf_cms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-drf-cms
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Django app to build a simple cms restful server.
 Home-page: https://www.spartanbits.com
 Author: Spartanbits, SLU
 Author-email: info@spartanbits.com
 License: Apache-2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-drf-cms-0.1.8/django_drf_cms.egg-info/SOURCES.txt` & `django-drf-cms-0.1.9/django_drf_cms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.8/drf_cms/admin.py` & `django-drf-cms-0.1.9/drf_cms/admin.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.8/drf_cms/migrations/0001_initial.py` & `django-drf-cms-0.1.9/drf_cms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.8/drf_cms/migrations/0003_page_description_en_page_description_es_and_more.py` & `django-drf-cms-0.1.9/drf_cms/migrations/0003_page_description_en_page_description_es_and_more.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.8/drf_cms/models.py` & `django-drf-cms-0.1.9/drf_cms/models.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.8/drf_cms/permissions.py` & `django-drf-cms-0.1.9/drf_cms/permissions.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.8/drf_cms/serializers.py` & `django-drf-cms-0.1.9/drf_cms/serializers.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.8/drf_cms/storage_backends.py` & `django-drf-cms-0.1.9/drf_cms/storage_backends.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.8/drf_cms/urls.py` & `django-drf-cms-0.1.9/drf_cms/urls.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.8/drf_cms/views.py` & `django-drf-cms-0.1.9/drf_cms/views.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.8/setup.cfg` & `django-drf-cms-0.1.9/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-drf-cms
-version = 0.1.8
+version = 0.1.9
 description = A Django app to build a simple cms restful server.
 long_description = file: README.rst
 url = https://www.spartanbits.com
 author = Spartanbits, SLU
 author_email = info@spartanbits.com
 license = Apache-2.0
 classifiers = 
@@ -28,12 +28,13 @@
 python_requires = >=3.8
 install_requires = 
 	Django >= 4.2
 	django_bleach>=3.0.1
 	djangorestframework>=3.14.0
 	django-modeltranslation>=0.18.9
 	django-storages>=1.13.2
+	boto3>=1.26.123
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

