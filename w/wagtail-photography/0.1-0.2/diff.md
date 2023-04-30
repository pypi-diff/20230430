# Comparing `tmp/wagtail-photography-0.1.tar.gz` & `tmp/wagtail-photography-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-photography-0.1.tar", last modified: Sat Apr 29 01:53:43 2023, max compression
+gzip compressed data, was "wagtail-photography-0.2.tar", last modified: Sun Apr 30 05:37:56 2023, max compression
```

## Comparing `wagtail-photography-0.1.tar` & `wagtail-photography-0.2.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-04-29 01:53:43.114184 wagtail-photography-0.1/
--rw-rw-r--   0 ave       (1000) ave       (1000)    11356 2023-04-24 20:19:57.000000 wagtail-photography-0.1/LICENSE
--rw-rw-r--   0 ave       (1000) ave       (1000)      156 2023-04-24 20:32:56.000000 wagtail-photography-0.1/MANIFEST.in
--rw-rw-r--   0 ave       (1000) ave       (1000)     1744 2023-04-29 01:53:43.114184 wagtail-photography-0.1/PKG-INFO
--rw-rw-r--   0 ave       (1000) ave       (1000)      855 2023-04-29 01:52:45.000000 wagtail-photography-0.1/README.md
--rw-rw-r--   0 ave       (1000) ave       (1000)       88 2023-04-24 20:20:58.000000 wagtail-photography-0.1/pyproject.toml
--rw-rw-r--   0 ave       (1000) ave       (1000)      940 2023-04-29 01:53:43.114184 wagtail-photography-0.1/setup.cfg
--rw-rw-r--   0 ave       (1000) ave       (1000)       38 2023-04-26 01:55:13.000000 wagtail-photography-0.1/setup.py
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-04-29 01:53:43.114184 wagtail-photography-0.1/wagtail_photography/
--rw-rw-r--   0 ave       (1000) ave       (1000)        0 2023-04-24 19:22:23.000000 wagtail-photography-0.1/wagtail_photography/__init__.py
--rw-rw-r--   0 ave       (1000) ave       (1000)      169 2023-04-24 19:22:23.000000 wagtail-photography-0.1/wagtail_photography/apps.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     1372 2023-04-29 01:28:30.000000 wagtail-photography-0.1/wagtail_photography/blocks.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     1276 2023-04-24 19:22:23.000000 wagtail-photography-0.1/wagtail_photography/forms.py
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-04-29 01:53:43.114184 wagtail-photography-0.1/wagtail_photography/migrations/
--rw-rw-r--   0 ave       (1000) ave       (1000)     2623 2023-04-29 01:28:30.000000 wagtail-photography-0.1/wagtail_photography/migrations/0001_initial.py
--rw-rw-r--   0 ave       (1000) ave       (1000)        0 2023-04-24 19:22:23.000000 wagtail-photography-0.1/wagtail_photography/migrations/__init__.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     4678 2023-04-29 01:28:30.000000 wagtail-photography-0.1/wagtail_photography/models.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     1044 2023-04-29 01:28:30.000000 wagtail-photography-0.1/wagtail_photography/signals.py
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-04-29 01:53:43.114184 wagtail-photography-0.1/wagtail_photography/static/
--rw-rw-r--   0 ave       (1000) ave       (1000)     1234 2023-04-26 02:00:09.000000 wagtail-photography-0.1/wagtail_photography/static/app.js
--rw-rw-r--   0 ave       (1000) ave       (1000)      384 2023-04-26 02:00:09.000000 wagtail-photography-0.1/wagtail_photography/static/photo_gallery.css
--rw-rw-r--   0 ave       (1000) ave       (1000)     3119 2023-04-26 02:01:14.000000 wagtail-photography-0.1/wagtail_photography/static/photo_gallery_admin.css
--rw-rw-r--   0 ave       (1000) ave       (1000)    11256 2023-04-26 02:01:14.000000 wagtail-photography-0.1/wagtail_photography/static/photo_gallery_admin.js
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-04-29 01:53:43.114184 wagtail-photography-0.1/wagtail_photography/templates/
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-04-29 01:53:43.114184 wagtail-photography-0.1/wagtail_photography/templates/blocks/
--rw-rw-r--   0 ave       (1000) ave       (1000)      980 2023-04-29 01:28:30.000000 wagtail-photography-0.1/wagtail_photography/templates/blocks/photo_gallery.html
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-04-29 01:53:43.114184 wagtail-photography-0.1/wagtail_photography/templates/includes/
--rw-rw-r--   0 ave       (1000) ave       (1000)     2526 2023-04-29 01:28:30.000000 wagtail-photography-0.1/wagtail_photography/templates/includes/photo_swipe.html
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-04-29 01:53:43.114184 wagtail-photography-0.1/wagtail_photography/templates/wagtail_photography/
--rw-rw-r--   0 ave       (1000) ave       (1000)     1620 2023-04-29 01:28:30.000000 wagtail-photography-0.1/wagtail_photography/templates/wagtail_photography/album_detail.html
--rw-rw-r--   0 ave       (1000) ave       (1000)      541 2023-04-29 01:28:30.000000 wagtail-photography-0.1/wagtail_photography/templates/wagtail_photography/extra_css.html
--rw-rw-r--   0 ave       (1000) ave       (1000)     1090 2023-04-29 01:28:30.000000 wagtail-photography-0.1/wagtail_photography/templates/wagtail_photography/extra_js.html
--rw-rw-r--   0 ave       (1000) ave       (1000)       60 2023-04-24 19:22:23.000000 wagtail-photography-0.1/wagtail_photography/tests.py
--rw-rw-r--   0 ave       (1000) ave       (1000)      373 2023-04-29 01:28:30.000000 wagtail-photography-0.1/wagtail_photography/views.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     1221 2023-04-29 01:28:30.000000 wagtail-photography-0.1/wagtail_photography/wagtail_hooks.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     1030 2023-04-29 01:28:30.000000 wagtail-photography-0.1/wagtail_photography/widgets.py
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-04-29 01:53:43.114184 wagtail-photography-0.1/wagtail_photography.egg-info/
--rw-rw-r--   0 ave       (1000) ave       (1000)     1744 2023-04-29 01:53:43.000000 wagtail-photography-0.1/wagtail_photography.egg-info/PKG-INFO
--rw-rw-r--   0 ave       (1000) ave       (1000)     1162 2023-04-29 01:53:43.000000 wagtail-photography-0.1/wagtail_photography.egg-info/SOURCES.txt
--rw-rw-r--   0 ave       (1000) ave       (1000)        1 2023-04-29 01:53:43.000000 wagtail-photography-0.1/wagtail_photography.egg-info/dependency_links.txt
--rw-rw-r--   0 ave       (1000) ave       (1000)       39 2023-04-29 01:53:43.000000 wagtail-photography-0.1/wagtail_photography.egg-info/requires.txt
--rw-rw-r--   0 ave       (1000) ave       (1000)       20 2023-04-29 01:53:43.000000 wagtail-photography-0.1/wagtail_photography.egg-info/top_level.txt
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-04-30 05:37:56.554024 wagtail-photography-0.2/
+-rw-rw-r--   0 ave       (1000) ave       (1000)    11356 2023-04-24 20:19:57.000000 wagtail-photography-0.2/LICENSE
+-rw-rw-r--   0 ave       (1000) ave       (1000)      156 2023-04-24 20:32:56.000000 wagtail-photography-0.2/MANIFEST.in
+-rw-rw-r--   0 ave       (1000) ave       (1000)     2236 2023-04-30 05:37:56.554024 wagtail-photography-0.2/PKG-INFO
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1347 2023-04-30 05:36:56.000000 wagtail-photography-0.2/README.md
+-rw-rw-r--   0 ave       (1000) ave       (1000)       88 2023-04-24 20:20:58.000000 wagtail-photography-0.2/pyproject.toml
+-rw-rw-r--   0 ave       (1000) ave       (1000)      940 2023-04-30 05:37:56.554024 wagtail-photography-0.2/setup.cfg
+-rw-rw-r--   0 ave       (1000) ave       (1000)       38 2023-04-26 01:55:13.000000 wagtail-photography-0.2/setup.py
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-04-30 05:37:56.550024 wagtail-photography-0.2/wagtail_photography/
+-rw-rw-r--   0 ave       (1000) ave       (1000)        0 2023-04-24 19:22:23.000000 wagtail-photography-0.2/wagtail_photography/__init__.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)      169 2023-04-24 19:22:23.000000 wagtail-photography-0.2/wagtail_photography/apps.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1372 2023-04-29 01:28:30.000000 wagtail-photography-0.2/wagtail_photography/blocks.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1276 2023-04-24 19:22:23.000000 wagtail-photography-0.2/wagtail_photography/forms.py
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-04-30 05:37:56.550024 wagtail-photography-0.2/wagtail_photography/migrations/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     2623 2023-04-29 01:28:30.000000 wagtail-photography-0.2/wagtail_photography/migrations/0001_initial.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)        0 2023-04-24 19:22:23.000000 wagtail-photography-0.2/wagtail_photography/migrations/__init__.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     5147 2023-04-30 05:36:56.000000 wagtail-photography-0.2/wagtail_photography/models.py
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-04-30 05:37:56.554024 wagtail-photography-0.2/wagtail_photography/static/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1234 2023-04-26 02:00:09.000000 wagtail-photography-0.2/wagtail_photography/static/app.js
+-rw-rw-r--   0 ave       (1000) ave       (1000)      384 2023-04-26 02:00:09.000000 wagtail-photography-0.2/wagtail_photography/static/photo_gallery.css
+-rw-rw-r--   0 ave       (1000) ave       (1000)     3119 2023-04-26 02:01:14.000000 wagtail-photography-0.2/wagtail_photography/static/photo_gallery_admin.css
+-rw-rw-r--   0 ave       (1000) ave       (1000)    11256 2023-04-26 02:01:14.000000 wagtail-photography-0.2/wagtail_photography/static/photo_gallery_admin.js
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-04-30 05:37:56.550024 wagtail-photography-0.2/wagtail_photography/templates/
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-04-30 05:37:56.554024 wagtail-photography-0.2/wagtail_photography/templates/blocks/
+-rw-rw-r--   0 ave       (1000) ave       (1000)      980 2023-04-29 01:28:30.000000 wagtail-photography-0.2/wagtail_photography/templates/blocks/photo_gallery.html
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-04-30 05:37:56.554024 wagtail-photography-0.2/wagtail_photography/templates/includes/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     2526 2023-04-29 01:28:30.000000 wagtail-photography-0.2/wagtail_photography/templates/includes/photo_swipe.html
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-04-30 05:37:56.554024 wagtail-photography-0.2/wagtail_photography/templates/wagtail_photography/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1378 2023-04-30 05:36:56.000000 wagtail-photography-0.2/wagtail_photography/templates/wagtail_photography/album_detail.html
+-rw-rw-r--   0 ave       (1000) ave       (1000)      541 2023-04-29 01:28:30.000000 wagtail-photography-0.2/wagtail_photography/templates/wagtail_photography/extra_css.html
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1106 2023-04-30 05:36:56.000000 wagtail-photography-0.2/wagtail_photography/templates/wagtail_photography/extra_js.html
+-rw-rw-r--   0 ave       (1000) ave       (1000)       60 2023-04-24 19:22:23.000000 wagtail-photography-0.2/wagtail_photography/tests.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)      373 2023-04-29 01:28:30.000000 wagtail-photography-0.2/wagtail_photography/views.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1221 2023-04-29 01:28:30.000000 wagtail-photography-0.2/wagtail_photography/wagtail_hooks.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1030 2023-04-29 01:28:30.000000 wagtail-photography-0.2/wagtail_photography/widgets.py
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-04-30 05:37:56.550024 wagtail-photography-0.2/wagtail_photography.egg-info/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     2236 2023-04-30 05:37:56.000000 wagtail-photography-0.2/wagtail_photography.egg-info/PKG-INFO
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1131 2023-04-30 05:37:56.000000 wagtail-photography-0.2/wagtail_photography.egg-info/SOURCES.txt
+-rw-rw-r--   0 ave       (1000) ave       (1000)        1 2023-04-30 05:37:56.000000 wagtail-photography-0.2/wagtail_photography.egg-info/dependency_links.txt
+-rw-rw-r--   0 ave       (1000) ave       (1000)       39 2023-04-30 05:37:56.000000 wagtail-photography-0.2/wagtail_photography.egg-info/requires.txt
+-rw-rw-r--   0 ave       (1000) ave       (1000)       20 2023-04-30 05:37:56.000000 wagtail-photography-0.2/wagtail_photography.egg-info/top_level.txt
```

### Comparing `wagtail-photography-0.1/LICENSE` & `wagtail-photography-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.1/PKG-INFO` & `wagtail-photography-0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-photography
-Version: 0.1
+Version: 0.2
 Summary: A Wagtail app to display photographs
 Home-page: https://averyuslaner.com/
 Author: Avery Uslaner
 Author-email: uslaner.avery@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Wagtail
@@ -35,21 +35,43 @@
 
 Detailed documentation is in the "docs" directory.
 
 Quick start
 -----------
 
 1. Install requirements
-    
-    ```pip install wagtail-generic-chooser```
+
+   ```pip install wagtail-generic-chooser```
+
+
 2. Add "wagtail_photography" and wagtail-generic-chooser to your INSTALLED_APPS setting like this:
 
-    INSTALLED_APPS = [
-         ...,
-         "generic_chooser"
-         "wagtail_photography",
-    ]
+   ```python
+   INSTALLED_APPS = [
+      ...
+      "generic_chooser"
+      "wagtail_photography",
+   ]
+   ```
+
+
+3. [Setup Wagtail to dynamically serve image urls](https://docs.wagtail.org/en/stable/advanced_topics/images/image_serve_view.html#setup):
+
+```python
+from wagtail.images.views.serve import ServeView
+
+urlpatterns = [
+    ...
+
+    re_path(r'^images/([^/]*)/(\d*)/([^/]*)/[^/]*$', ServeView.as_view(), name='wagtailimages_serve'),
+
+    ...
+
+    # Ensure that the wagtailimages_serve line appears above the default Wagtail page serving route
+    re_path(r'', include(wagtail_urls)),
+]
+```
 
 3. Run ``python manage.py migrate`` to create the wagtail_photography models.
 
 4. Start the development server and visit http://127.0.0.1:8000/admin/
    to create an album.
```

### Comparing `wagtail-photography-0.1/README.md` & `wagtail-photography-0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -11,21 +11,43 @@
 
 Detailed documentation is in the "docs" directory.
 
 Quick start
 -----------
 
 1. Install requirements
-    
-    ```pip install wagtail-generic-chooser```
+
+   ```pip install wagtail-generic-chooser```
+
+
 2. Add "wagtail_photography" and wagtail-generic-chooser to your INSTALLED_APPS setting like this:
 
-    INSTALLED_APPS = [
-         ...,
-         "generic_chooser"
-         "wagtail_photography",
-    ]
+   ```python
+   INSTALLED_APPS = [
+      ...
+      "generic_chooser"
+      "wagtail_photography",
+   ]
+   ```
+
+
+3. [Setup Wagtail to dynamically serve image urls](https://docs.wagtail.org/en/stable/advanced_topics/images/image_serve_view.html#setup):
+
+```python
+from wagtail.images.views.serve import ServeView
+
+urlpatterns = [
+    ...
+
+    re_path(r'^images/([^/]*)/(\d*)/([^/]*)/[^/]*$', ServeView.as_view(), name='wagtailimages_serve'),
+
+    ...
+
+    # Ensure that the wagtailimages_serve line appears above the default Wagtail page serving route
+    re_path(r'', include(wagtail_urls)),
+]
+```
 
 3. Run ``python manage.py migrate`` to create the wagtail_photography models.
 
 4. Start the development server and visit http://127.0.0.1:8000/admin/
    to create an album.
```

### Comparing `wagtail-photography-0.1/setup.cfg` & `wagtail-photography-0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-photography
-version = 0.1
+version = 0.2
 description = A Wagtail app to display photographs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://averyuslaner.com/
 author = Avery Uslaner
 author_email = uslaner.avery@gmail.com
 license = Apache License 2.0
```

### Comparing `wagtail-photography-0.1/wagtail_photography/blocks.py` & `wagtail-photography-0.2/wagtail_photography/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.1/wagtail_photography/forms.py` & `wagtail-photography-0.2/wagtail_photography/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.1/wagtail_photography/migrations/0001_initial.py` & `wagtail-photography-0.2/wagtail_photography/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.1/wagtail_photography/models.py` & `wagtail-photography-0.2/wagtail_photography/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import copy
 import itertools
+import json
 import uuid
 
 from django import forms
 from django.db import models
 from django.http import Http404
 from django.shortcuts import render
 from modelcluster.fields import ParentalKey
 from modelcluster.models import ClusterableModel
 from wagtail.admin.panels import FieldPanel, MultiFieldPanel, HelpPanel, TabbedInterface, ObjectList, InlinePanel
 from wagtail.contrib.routable_page.models import RoutablePageMixin, route
 from wagtail.coreutils import resolve_model_string
 from wagtail.fields import StreamField
 from wagtail.images import get_image_model_string
+from wagtail.images.views.serve import generate_image_url
 from wagtail.models import Orderable
 
 from .blocks import GalleryBlock
 from .forms import AlbumForm
 
 
 class Album(ClusterableModel):
@@ -82,16 +84,14 @@
 
 
 class AlbumImage(Orderable):
     name = models.CharField(max_length=255, default=None, null=True)
     image = models.ForeignKey('wagtailimages.Image', on_delete=models.SET_NULL, null=True)
     album = ParentalKey('Album', on_delete=models.CASCADE, related_name='images')
     created = models.DateTimeField(auto_now_add=True)
-    width = models.IntegerField(default=0)
-    height = models.IntegerField(default=0)
     slug = models.SlugField(max_length=70, default=uuid.uuid4, editable=False)
 
     panels = [
         FieldPanel('image'),
     ]
 
     def __init__(self, *args, **kwargs):
@@ -127,14 +127,23 @@
         for gallery in self._gallery_blocks:
             try:
                 album = gallery.block.filter_albums(gallery.value).get(slug=slug)
 
             except Album.DoesNotExist:
                 continue
 
+            image_data = []
+            for album_image in album.images.all():
+                image = album_image.image
+                image_data.append({'image': image,
+                                   'jpeg_image_url': generate_image_url(image, 'fill-300x300|format-jpeg'),
+                                   'webp_image_url': generate_image_url(image, 'fill-300x300|format-webp'),
+                                   'album_image': album_image,
+                                   })
+
             return render(
                 request,
                 'wagtail_photography/album_detail.html',
-                {'page': self, 'album': album, 'images': album.images.all()}
+                {'page': self, 'album': album, 'image_data': image_data}
             )
 
         raise Http404
```

### Comparing `wagtail-photography-0.1/wagtail_photography/static/app.js` & `wagtail-photography-0.2/wagtail_photography/static/app.js`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.1/wagtail_photography/static/photo_gallery_admin.css` & `wagtail-photography-0.2/wagtail_photography/static/photo_gallery_admin.css`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.1/wagtail_photography/static/photo_gallery_admin.js` & `wagtail-photography-0.2/wagtail_photography/static/photo_gallery_admin.js`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.1/wagtail_photography/templates/blocks/photo_gallery.html` & `wagtail-photography-0.2/wagtail_photography/templates/blocks/photo_gallery.html`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.1/wagtail_photography/templates/includes/photo_swipe.html` & `wagtail-photography-0.2/wagtail_photography/templates/includes/photo_swipe.html`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.1/wagtail_photography/templates/wagtail_photography/album_detail.html` & `wagtail-photography-0.2/wagtail_photography/templates/wagtail_photography/album_detail.html`

 * *Files 27% similar despite different names*

```diff
@@ -11,24 +11,22 @@
             <header>
                 <h1>{{ album.title }}</h1>
             </header>
             <section>
                 <p>{{ album.description }}</p>
 
                 <div class="photo-gallery-container">
-                    {% for item in images %}
+                    {% for image_item in image_data %}
                         <a href="javascript:pswpInit({{ forloop.counter0 }});">
                             <picture>
-                                {% image item.image fill-300x300 format-webp as image_webp %}
-                                <source srcset="{{ image_webp.url }}" type="image/webp">
+                                <source srcset="{{ image_item.webp_image_url }}" type="image/webp">
 
-                                {% image item.image fill-300x300 format-jpeg as image_jpeg %}
-                                <source srcset="{{ image_jpeg.url }}" type="image/jpeg">
+                                <source srcset="{{ image_item.jpeg_image_url }}" type="image/jpeg">
 
-                                {% image item.image fill-300x300 %}
+                                {% image image_item.image fill-300x300 %}
                             </picture>
                         </a>
                     {% endfor %}
                 </div>
 
             </section>
         </article>
@@ -40,14 +38,9 @@
     {% endif %}
 
     <a href="{{ page.url }}">Go back</a>
 
 {% endblock %}
 
 {% block extra_js %}
-    <script>
-    {% for item in images %}
-console.log({{item}});
-{% endfor %}
-    </script>
     {% include 'wagtail_photography/extra_js.html' with images=images %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,14 +1,12 @@
 {% extends "base.html" %} {% load wagtailimages_tags %} {% block extra_css %}
 {% include 'wagtail_photography/extra_css.html' %} {% endblock %} {% block
 content %} {% if album.is_visible %}
 ****** {{ album.title }} ******
 
 {{ album.description }}
-{% for item in images %} _{%_image_item.image_fill-300x300_format-webp_as
-image_webp_%}__{%_image_item.image_fill-300x300_format-jpeg_as_image_jpeg_%}__
-{%_image_item.image_fill-300x300_%}_ {% endfor %}
+{% for image_item in image_data %} ___{%_image_image_item.image_fill-300x300_%}
+{% endfor %}
   {% include 'includes/photo_swipe.html' %} {% else %}
 **** This album is temporarily unavailable. ****
-{% endif %} Go_back {% endblock %} {% block extra_js %}
- {% include 'wagtail_photography/extra_js.html' with images=images %} {%
-endblock %}
+{% endif %} Go_back {% endblock %} {% block extra_js %} {% include
+'wagtail_photography/extra_js.html' with images=images %} {% endblock %}
```

### Comparing `wagtail-photography-0.1/wagtail_photography/templates/wagtail_photography/extra_css.html` & `wagtail-photography-0.2/wagtail_photography/templates/wagtail_photography/extra_css.html`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.1/wagtail_photography/templates/wagtail_photography/extra_js.html` & `wagtail-photography-0.2/wagtail_photography/templates/wagtail_photography/extra_js.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 {% load static %}
+{% load wagtailimages_tags %}
 
 <script
         src="https://code.jquery.com/jquery-3.5.1.slim.min.js"
         integrity="sha256-4+XzXVhsDmqanXGHaHvgh1gMQKX40OUvDEBTu8JcmNs="
         crossorigin="anonymous"></script>
 
 <script src="{% static 'app.js' %}"></script>
 <script>
-{% for item in images %}
-console.log({{item}});
-{% endfor %}
-</script>
-<script>
     // build the json album images collection
     window.djangoAlbumImages = [
-        {% for item in images %}
+        {% for image_item in image_data %}
+            {% image image_item.image original as photo %}
             {
-                src: '{{ item.image.url }}',
-                w:  {{ item.width }},
-                h:  {{ item.height }}
+                src: '{{ photo.url }}',
+                w:  {{ photo.width }},
+                h:  {{ photo.height }}
             },
         {% endfor %}
     ];
 </script>
 
 <script src="https://cdn.jsdelivr.net/npm/photoswipe@4.1.3/dist/photoswipe.min.js"
         integrity="sha384-jkeJ/ETDRD/P4Y3I3CQi1QIwrEJjR9GdAZV2/aqDwwgA5ldCNiExYJeBwKyQC/+q"
```

#### html2text {}

```diff
@@ -1,2 +1,2 @@
-{% load static %}
+{% load static %} {% load wagtailimages_tags %}
```

### Comparing `wagtail-photography-0.1/wagtail_photography/wagtail_hooks.py` & `wagtail-photography-0.2/wagtail_photography/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.1/wagtail_photography/widgets.py` & `wagtail-photography-0.2/wagtail_photography/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.1/wagtail_photography.egg-info/PKG-INFO` & `wagtail-photography-0.2/wagtail_photography.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-photography
-Version: 0.1
+Version: 0.2
 Summary: A Wagtail app to display photographs
 Home-page: https://averyuslaner.com/
 Author: Avery Uslaner
 Author-email: uslaner.avery@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Wagtail
@@ -35,21 +35,43 @@
 
 Detailed documentation is in the "docs" directory.
 
 Quick start
 -----------
 
 1. Install requirements
-    
-    ```pip install wagtail-generic-chooser```
+
+   ```pip install wagtail-generic-chooser```
+
+
 2. Add "wagtail_photography" and wagtail-generic-chooser to your INSTALLED_APPS setting like this:
 
-    INSTALLED_APPS = [
-         ...,
-         "generic_chooser"
-         "wagtail_photography",
-    ]
+   ```python
+   INSTALLED_APPS = [
+      ...
+      "generic_chooser"
+      "wagtail_photography",
+   ]
+   ```
+
+
+3. [Setup Wagtail to dynamically serve image urls](https://docs.wagtail.org/en/stable/advanced_topics/images/image_serve_view.html#setup):
+
+```python
+from wagtail.images.views.serve import ServeView
+
+urlpatterns = [
+    ...
+
+    re_path(r'^images/([^/]*)/(\d*)/([^/]*)/[^/]*$', ServeView.as_view(), name='wagtailimages_serve'),
+
+    ...
+
+    # Ensure that the wagtailimages_serve line appears above the default Wagtail page serving route
+    re_path(r'', include(wagtail_urls)),
+]
+```
 
 3. Run ``python manage.py migrate`` to create the wagtail_photography models.
 
 4. Start the development server and visit http://127.0.0.1:8000/admin/
    to create an album.
```

### Comparing `wagtail-photography-0.1/wagtail_photography.egg-info/SOURCES.txt` & `wagtail-photography-0.2/wagtail_photography.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 setup.cfg
 setup.py
 wagtail_photography/__init__.py
 wagtail_photography/apps.py
 wagtail_photography/blocks.py
 wagtail_photography/forms.py
 wagtail_photography/models.py
-wagtail_photography/signals.py
 wagtail_photography/tests.py
 wagtail_photography/views.py
 wagtail_photography/wagtail_hooks.py
 wagtail_photography/widgets.py
 wagtail_photography.egg-info/PKG-INFO
 wagtail_photography.egg-info/SOURCES.txt
 wagtail_photography.egg-info/dependency_links.txt
```

