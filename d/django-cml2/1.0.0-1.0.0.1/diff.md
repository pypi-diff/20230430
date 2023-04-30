# Comparing `tmp/django-cml2-1.0.0.tar.gz` & `tmp/django-cml2-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cml2-1.0.0.tar", last modified: Sat Apr 29 15:10:42 2023, max compression
+gzip compressed data, was "django-cml2-1.0.0.1.tar", last modified: Sun Apr 30 11:09:21 2023, max compression
```

## Comparing `django-cml2-1.0.0.tar` & `django-cml2-1.0.0.1.tar`

### file list

```diff
@@ -1,36 +1,24 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-29 15:10:42.041273 django-cml2-1.0.0/
--rw-r--r--   0 admin      (501) staff       (20)     1515 2023-04-27 07:07:40.000000 django-cml2-1.0.0/LICENSE
--rw-r--r--   0 admin      (501) staff       (20)      163 2023-04-28 21:29:48.000000 django-cml2-1.0.0/MANIFEST.in
--rw-r--r--   0 admin      (501) staff       (20)     2050 2023-04-29 15:10:42.041529 django-cml2-1.0.0/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     1131 2023-04-29 14:15:17.000000 django-cml2-1.0.0/README.rst
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-29 15:10:42.030199 django-cml2-1.0.0/cml/
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-04-27 07:07:40.000000 django-cml2-1.0.0/cml/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     2440 2023-04-26 14:35:21.000000 django-cml2-1.0.0/cml/admin.py
--rw-r--r--   0 admin      (501) staff       (20)     4159 2023-04-16 17:19:40.000000 django-cml2-1.0.0/cml/auth.py
--rw-r--r--   0 admin      (501) staff       (20)      266 2023-04-27 14:41:27.000000 django-cml2-1.0.0/cml/conf.py
--rw-r--r--   0 admin      (501) staff       (20)    30983 2023-04-26 14:02:15.000000 django-cml2-1.0.0/cml/items.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-29 15:10:42.030984 django-cml2-1.0.0/cml/management/
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-04-27 07:07:40.000000 django-cml2-1.0.0/cml/management/__init__.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-29 15:10:42.031779 django-cml2-1.0.0/cml/management/commands/
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-04-27 07:07:40.000000 django-cml2-1.0.0/cml/management/commands/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      943 2023-04-28 13:31:47.000000 django-cml2-1.0.0/cml/management/commands/cml_init.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-29 15:10:42.034643 django-cml2-1.0.0/cml/migrations/
--rw-r--r--   0 admin      (501) staff       (20)      905 2023-04-27 07:56:03.000000 django-cml2-1.0.0/cml/migrations/0001_initial.py
--rw-r--r--   0 admin      (501) staff       (20)     5205 2023-04-27 14:28:07.000000 django-cml2-1.0.0/cml/migrations/0002_reorganize_fields.py
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-04-27 07:07:40.000000 django-cml2-1.0.0/cml/migrations/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1559 2023-04-27 12:50:50.000000 django-cml2-1.0.0/cml/models.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-29 15:10:42.020318 django-cml2-1.0.0/cml/templates/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-29 15:10:42.035859 django-cml2-1.0.0/cml/templates/cml/
--rw-r--r--   0 admin      (501) staff       (20)     1890 2023-04-28 13:22:39.000000 django-cml2-1.0.0/cml/templates/cml/cml_delegate.py
--rw-r--r--   0 admin      (501) staff       (20)      248 2023-04-27 08:50:19.000000 django-cml2-1.0.0/cml/urls.py
--rw-r--r--   0 admin      (501) staff       (20)     2515 2023-04-27 14:44:16.000000 django-cml2-1.0.0/cml/utils.py
--rw-r--r--   0 admin      (501) staff       (20)    12865 2023-04-26 13:17:05.000000 django-cml2-1.0.0/cml/views.py
--rw-r--r--   0 admin      (501) staff       (20)     7583 2023-04-22 18:39:52.000000 django-cml2-1.0.0/cml/xml.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-29 15:10:42.040820 django-cml2-1.0.0/django_cml2.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     2050 2023-04-29 15:10:41.000000 django-cml2-1.0.0/django_cml2.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      584 2023-04-29 15:10:41.000000 django-cml2-1.0.0/django_cml2.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-29 15:10:41.000000 django-cml2-1.0.0/django_cml2.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       34 2023-04-29 15:10:41.000000 django-cml2-1.0.0/django_cml2.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        4 2023-04-29 15:10:41.000000 django-cml2-1.0.0/django_cml2.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       53 2023-04-29 15:10:42.042413 django-cml2-1.0.0/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1295 2023-04-29 14:29:26.000000 django-cml2-1.0.0/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-30 11:09:21.873880 django-cml2-1.0.0.1/
+-rw-r--r--   0 admin      (501) staff       (20)     1515 2023-04-27 07:07:40.000000 django-cml2-1.0.0.1/LICENSE
+-rw-r--r--   0 admin      (501) staff       (20)      163 2023-04-28 21:29:48.000000 django-cml2-1.0.0.1/MANIFEST.in
+-rw-r--r--   0 admin      (501) staff       (20)     2052 2023-04-30 11:09:21.874096 django-cml2-1.0.0.1/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     1131 2023-04-29 14:15:17.000000 django-cml2-1.0.0.1/README.rst
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-30 11:09:21.871268 django-cml2-1.0.0.1/cml2/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-04-27 07:07:40.000000 django-cml2-1.0.0.1/cml2/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2440 2023-04-26 14:35:21.000000 django-cml2-1.0.0.1/cml2/admin.py
+-rw-r--r--   0 admin      (501) staff       (20)     4159 2023-04-16 17:19:40.000000 django-cml2-1.0.0.1/cml2/auth.py
+-rw-r--r--   0 admin      (501) staff       (20)      266 2023-04-27 14:41:27.000000 django-cml2-1.0.0.1/cml2/conf.py
+-rw-r--r--   0 admin      (501) staff       (20)    30983 2023-04-26 14:02:15.000000 django-cml2-1.0.0.1/cml2/items.py
+-rw-r--r--   0 admin      (501) staff       (20)     1559 2023-04-27 12:50:50.000000 django-cml2-1.0.0.1/cml2/models.py
+-rw-r--r--   0 admin      (501) staff       (20)      248 2023-04-27 08:50:19.000000 django-cml2-1.0.0.1/cml2/urls.py
+-rw-r--r--   0 admin      (501) staff       (20)     2515 2023-04-27 14:44:16.000000 django-cml2-1.0.0.1/cml2/utils.py
+-rw-r--r--   0 admin      (501) staff       (20)    12912 2023-04-30 11:03:31.000000 django-cml2-1.0.0.1/cml2/views.py
+-rw-r--r--   0 admin      (501) staff       (20)     7583 2023-04-22 18:39:52.000000 django-cml2-1.0.0.1/cml2/xml.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-30 11:09:21.873503 django-cml2-1.0.0.1/django_cml2.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     2052 2023-04-30 11:09:21.000000 django-cml2-1.0.0.1/django_cml2.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      362 2023-04-30 11:09:21.000000 django-cml2-1.0.0.1/django_cml2.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-30 11:09:21.000000 django-cml2-1.0.0.1/django_cml2.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       34 2023-04-30 11:09:21.000000 django-cml2-1.0.0.1/django_cml2.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)        5 2023-04-30 11:09:21.000000 django-cml2-1.0.0.1/django_cml2.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       53 2023-04-30 11:09:21.874825 django-cml2-1.0.0.1/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1298 2023-04-30 11:08:57.000000 django-cml2-1.0.0.1/setup.py
```

### Comparing `django-cml2-1.0.0/LICENSE` & `django-cml2-1.0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cml2-1.0.0/PKG-INFO` & `django-cml2-1.0.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cml2
-Version: 1.0.0
+Version: 1.0.0.1
 Summary: Application for data exchange in CommerceML 2 standard. This is a new version with new architecture
 Home-page: https://github.com/sergey-gru/django-cml2
 Author: Sergey Grunenko
 Author-email: grunenko.serg@gmail.com
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-cml2-1.0.0/README.rst` & `django-cml2-1.0.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-cml2-1.0.0/cml/admin.py` & `django-cml2-1.0.0.1/cml2/admin.py`

 * *Files identical despite different names*

### Comparing `django-cml2-1.0.0/cml/auth.py` & `django-cml2-1.0.0.1/cml2/auth.py`

 * *Files identical despite different names*

### Comparing `django-cml2-1.0.0/cml/items.py` & `django-cml2-1.0.0.1/cml2/items.py`

 * *Files identical despite different names*

### Comparing `django-cml2-1.0.0/cml/models.py` & `django-cml2-1.0.0.1/cml2/models.py`

 * *Files identical despite different names*

### Comparing `django-cml2-1.0.0/cml/utils.py` & `django-cml2-1.0.0.1/cml2/utils.py`

 * *Files identical despite different names*

### Comparing `django-cml2-1.0.0/cml/views.py` & `django-cml2-1.0.0.1/cml2/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,39 +18,43 @@
 
 logger = logging.getLogger(__name__)
 
 
 # Test configuration of delegate. If delegate was not configured,
 utils.AbstractUserDelegate.get_child_class()
 
+RESPONSE_SUCCESS = 'success'
+RESPONSE_PROGRESS = 'progress'
+RESPONSE_ERROR = 'error'
+
 
 @csrf_exempt
 @auth.has_perm_or_basicauth("cml.add_exchange")
 @auth.logged_in_or_basicauth()
 def front_view(request):
     return ProtocolView().dispatch(request)
 
 
 class ResponseException(Exception):
     def __init__(self, response: HttpResponse):
         self.res = response
 
 
 def response_success(msg='') -> HttpResponse:
-    res = "{}\n{}".format(settings.CML_RESPONSE_SUCCESS, msg)
+    res = "{}\n{}".format(RESPONSE_SUCCESS, msg)
     return HttpResponse(res)
 
 
 def response_progress(msg='') -> HttpResponse:
-    res = "{}\n{}".format(settings.CML_RESPONSE_PROGRESS, msg)
+    res = "{}\n{}".format(RESPONSE_PROGRESS, msg)
     return HttpResponse(res)
 
 
 def response_error(msg='') -> HttpResponse:
-    res = "{}\n{}".format(settings.CML_RESPONSE_ERROR, msg)
+    res = "{}\n{}".format(RESPONSE_ERROR, msg)
     return HttpResponse(res)
 
 
 msg_err_srv = 'An internal error occurred. We already know about it. We will try to fix it soon.'
 
 
 # Protocol description:
```

### Comparing `django-cml2-1.0.0/cml/xml.py` & `django-cml2-1.0.0.1/cml2/xml.py`

 * *Files identical despite different names*

### Comparing `django-cml2-1.0.0/django_cml2.egg-info/PKG-INFO` & `django-cml2-1.0.0.1/django_cml2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cml2
-Version: 1.0.0
+Version: 1.0.0.1
 Summary: Application for data exchange in CommerceML 2 standard. This is a new version with new architecture
 Home-page: https://github.com/sergey-gru/django-cml2
 Author: Sergey Grunenko
 Author-email: grunenko.serg@gmail.com
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-cml2-1.0.0/setup.py` & `django-cml2-1.0.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-cml2',
-    version='1.0.0',
+    version='1.0.0.1',
     description='Application for data exchange in CommerceML 2 standard. This is a new version with new architecture',
     long_description=README,
     author='Sergey Grunenko',
     author_email='grunenko.serg@gmail.com',
 
     url='https://github.com/sergey-gru/django-cml2',
     license='BSD License',
 
-    packages=['cml'],
+    packages=['cml2'],
     include_package_data=True,
 
     python_requires='>3.3.0',
     install_requires=['Django>=3.2', 'django-appconf>=1.0.1'],
 
     classifiers=[
         'Environment :: Web Environment',
```

