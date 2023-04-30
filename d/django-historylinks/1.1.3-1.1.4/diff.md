# Comparing `tmp/django-historylinks-1.1.3.tar.gz` & `tmp/django-historylinks-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-historylinks-1.1.3.tar", last modified: Sat Jan  7 14:38:23 2023, max compression
+gzip compressed data, was "django-historylinks-1.1.4.tar", last modified: Sun Apr 30 11:32:28 2023, max compression
```

## Comparing `django-historylinks-1.1.3.tar` & `django-historylinks-1.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 14:38:23.843236 django-historylinks-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-01-07 14:38:13.000000 django-historylinks-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-07 14:38:13.000000 django-historylinks-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-01-07 14:38:23.843236 django-historylinks-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-01-07 14:38:13.000000 django-historylinks-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-07 14:38:23.843236 django-historylinks-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-01-07 14:38:13.000000 django-historylinks-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 14:38:23.839235 django-historylinks-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 14:38:23.843236 django-historylinks-1.1.3/src/django_historylinks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-01-07 14:38:23.000000 django-historylinks-1.1.3/src/django_historylinks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-01-07 14:38:23.000000 django-historylinks-1.1.3/src/django_historylinks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-07 14:38:23.000000 django-historylinks-1.1.3/src/django_historylinks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-07 14:38:23.000000 django-historylinks-1.1.3/src/django_historylinks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-07 14:38:23.000000 django-historylinks-1.1.3/src/django_historylinks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-07 14:38:23.000000 django-historylinks-1.1.3/src/django_historylinks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 14:38:23.843236 django-historylinks-1.1.3/src/historylinks/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-07 14:38:13.000000 django-historylinks-1.1.3/src/historylinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-07 14:38:13.000000 django-historylinks-1.1.3/src/historylinks/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 14:38:23.843236 django-historylinks-1.1.3/src/historylinks/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-07 14:38:13.000000 django-historylinks-1.1.3/src/historylinks/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 14:38:23.843236 django-historylinks-1.1.3/src/historylinks/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-07 14:38:13.000000 django-historylinks-1.1.3/src/historylinks/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-01-07 14:38:13.000000 django-historylinks-1.1.3/src/historylinks/management/commands/buildhistorylinks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-01-07 14:38:13.000000 django-historylinks-1.1.3/src/historylinks/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 14:38:23.843236 django-historylinks-1.1.3/src/historylinks/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-01-07 14:38:13.000000 django-historylinks-1.1.3/src/historylinks/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-07 14:38:13.000000 django-historylinks-1.1.3/src/historylinks/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-01-07 14:38:13.000000 django-historylinks-1.1.3/src/historylinks/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-01-07 14:38:13.000000 django-historylinks-1.1.3/src/historylinks/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-01-07 14:38:13.000000 django-historylinks-1.1.3/src/historylinks/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:32:28.837736 django-historylinks-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-30 11:32:18.000000 django-historylinks-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-30 11:32:18.000000 django-historylinks-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-30 11:32:28.837736 django-historylinks-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-30 11:32:18.000000 django-historylinks-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 11:32:28.837736 django-historylinks-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-30 11:32:18.000000 django-historylinks-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:32:28.837736 django-historylinks-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:32:28.837736 django-historylinks-1.1.4/src/django_historylinks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-30 11:32:28.000000 django-historylinks-1.1.4/src/django_historylinks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-30 11:32:28.000000 django-historylinks-1.1.4/src/django_historylinks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 11:32:28.000000 django-historylinks-1.1.4/src/django_historylinks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 11:32:28.000000 django-historylinks-1.1.4/src/django_historylinks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-30 11:32:28.000000 django-historylinks-1.1.4/src/django_historylinks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-30 11:32:28.000000 django-historylinks-1.1.4/src/django_historylinks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:32:28.837736 django-historylinks-1.1.4/src/historylinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-30 11:32:18.000000 django-historylinks-1.1.4/src/historylinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-30 11:32:18.000000 django-historylinks-1.1.4/src/historylinks/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:32:28.837736 django-historylinks-1.1.4/src/historylinks/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 11:32:18.000000 django-historylinks-1.1.4/src/historylinks/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:32:28.837736 django-historylinks-1.1.4/src/historylinks/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 11:32:18.000000 django-historylinks-1.1.4/src/historylinks/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-30 11:32:18.000000 django-historylinks-1.1.4/src/historylinks/management/commands/buildhistorylinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-30 11:32:18.000000 django-historylinks-1.1.4/src/historylinks/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:32:28.837736 django-historylinks-1.1.4/src/historylinks/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-30 11:32:18.000000 django-historylinks-1.1.4/src/historylinks/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 11:32:18.000000 django-historylinks-1.1.4/src/historylinks/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-30 11:32:18.000000 django-historylinks-1.1.4/src/historylinks/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-04-30 11:32:18.000000 django-historylinks-1.1.4/src/historylinks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-30 11:32:18.000000 django-historylinks-1.1.4/src/historylinks/shortcuts.py
```

### Comparing `django-historylinks-1.1.3/LICENSE` & `django-historylinks-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-historylinks-1.1.3/PKG-INFO` & `django-historylinks-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-historylinks
-Version: 1.1.3
+Version: 1.1.4
 Summary: Automatic SEO-friendly HTTP 301 redirects if the URL of a Django model changes.
 Home-page: http://github.com/etianen/django-historylinks
 Author: Dave Hall
 Author-email: dave@etianen.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `django-historylinks-1.1.3/README.md` & `django-historylinks-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `django-historylinks-1.1.3/setup.py` & `django-historylinks-1.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 
 setup(
     name = "django-historylinks",
-    version = "1.1.3",
+    version = "1.1.4",
     description = "Automatic SEO-friendly HTTP 301 redirects if the URL of a Django model changes.",
     long_description = open("README.md").read(),
     author = "Dave Hall",
     author_email = "dave@etianen.com",
     url = "http://github.com/etianen/django-historylinks",
     zip_safe = False,
     packages = [
```

### Comparing `django-historylinks-1.1.3/src/django_historylinks.egg-info/PKG-INFO` & `django-historylinks-1.1.4/src/django_historylinks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-historylinks
-Version: 1.1.3
+Version: 1.1.4
 Summary: Automatic SEO-friendly HTTP 301 redirects if the URL of a Django model changes.
 Home-page: http://github.com/etianen/django-historylinks
 Author: Dave Hall
 Author-email: dave@etianen.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `django-historylinks-1.1.3/src/django_historylinks.egg-info/SOURCES.txt` & `django-historylinks-1.1.4/src/django_historylinks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-historylinks-1.1.3/src/historylinks/management/commands/buildhistorylinks.py` & `django-historylinks-1.1.4/src/historylinks/management/commands/buildhistorylinks.py`

 * *Files identical despite different names*

### Comparing `django-historylinks-1.1.3/src/historylinks/middleware.py` & `django-historylinks-1.1.4/src/historylinks/middleware.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,31 +3,30 @@
 
 from django.shortcuts import redirect
 from django.utils.cache import add_never_cache_headers
 from django.utils.deprecation import MiddlewareMixin
 
 from historylinks.registration import history_link_context_manager, default_history_link_manager
 
-
-HISTORYLINK_MIDDLEWARE_FLAG = "historylinks.history_link_fallback_middleware_active"
+HISTORYLINK_MIDDLEWARE_FLAG = "_history_link_fallback_middleware_active"
 
 
 class HistoryLinkFallbackMiddleware(MiddlewareMixin):
 
     """Middleware that attempts to rescue 404 responses with a redirect to it's new location."""
 
     def process_request(self, request):
         """Starts a new history link context."""
-        request.META[(HISTORYLINK_MIDDLEWARE_FLAG, self)] = True
+        setattr(request, HISTORYLINK_MIDDLEWARE_FLAG, True)
         history_link_context_manager.start()
 
     def _close_history_link_context(self, request):
         """Closes the history link context."""
-        if request.META.get((HISTORYLINK_MIDDLEWARE_FLAG, self), False):
-            del request.META[(HISTORYLINK_MIDDLEWARE_FLAG, self)]
+        if getattr(request, HISTORYLINK_MIDDLEWARE_FLAG, False):
+            setattr(request, HISTORYLINK_MIDDLEWARE_FLAG, False)
             history_link_context_manager.end()
 
     def process_response(self, request, response):
         """Attempts to rescue 404 responses and closes the history link context."""
         # Close the history link context.
         self._close_history_link_context(request)
         # Attempt to rescue a 404 error.
```

### Comparing `django-historylinks-1.1.3/src/historylinks/migrations/0001_initial.py` & `django-historylinks-1.1.4/src/historylinks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-historylinks-1.1.3/src/historylinks/models.py` & `django-historylinks-1.1.4/src/historylinks/models.py`

 * *Files identical despite different names*

### Comparing `django-historylinks-1.1.3/src/historylinks/registration.py` & `django-historylinks-1.1.4/src/historylinks/registration.py`

 * *Files identical despite different names*

### Comparing `django-historylinks-1.1.3/src/historylinks/shortcuts.py` & `django-historylinks-1.1.4/src/historylinks/shortcuts.py`

 * *Files identical despite different names*

