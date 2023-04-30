# Comparing `tmp/djangocms-simple-admin-style-0.1.0.tar.gz` & `tmp/djangocms-simple-admin-style-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-simple-admin-style-0.1.0.tar", last modified: Sun Apr 30 16:49:40 2023, max compression
+gzip compressed data, was "djangocms-simple-admin-style-0.1.1.tar", last modified: Sun Apr 30 17:13:17 2023, max compression
```

## Comparing `djangocms-simple-admin-style-0.1.0.tar` & `djangocms-simple-admin-style-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 fsbraun    (501) staff       (20)        0 2023-04-30 16:49:40.258438 djangocms-simple-admin-style-0.1.0/
--rw-r--r--   0 fsbraun    (501) staff       (20)     1479 2023-04-30 16:44:00.000000 djangocms-simple-admin-style-0.1.0/LICENSE
--rw-r--r--   0 fsbraun    (501) staff       (20)      218 2023-04-30 14:54:14.000000 djangocms-simple-admin-style-0.1.0/MANIFEST.in
--rw-r--r--   0 fsbraun    (501) staff       (20)     4045 2023-04-30 16:49:40.258505 djangocms-simple-admin-style-0.1.0/PKG-INFO
--rw-r--r--   0 fsbraun    (501) staff       (20)     2155 2023-04-30 16:38:49.000000 djangocms-simple-admin-style-0.1.0/README.rst
-drwxr-xr-x   0 fsbraun    (501) staff       (20)        0 2023-04-30 16:49:40.256591 djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style/
--rw-r--r--   0 fsbraun    (501) staff       (20)       22 2023-04-30 14:56:33.000000 djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style/__init__.py
-drwxr-xr-x   0 fsbraun    (501) staff       (20)        0 2023-04-30 16:49:40.255718 djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style/static/
-drwxr-xr-x   0 fsbraun    (501) staff       (20)        0 2023-04-30 16:49:40.255766 djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style/static/djangocms_simple_admin_style/
-drwxr-xr-x   0 fsbraun    (501) staff       (20)        0 2023-04-30 16:49:40.257905 djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/
--rw-r--r--   0 fsbraun    (501) staff       (20)     4582 2023-04-30 16:14:29.000000 djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/djangocms-simple-admin.css
-drwxr-xr-x   0 fsbraun    (501) staff       (20)        0 2023-04-30 16:49:40.255881 djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style/templates/
-drwxr-xr-x   0 fsbraun    (501) staff       (20)        0 2023-04-30 16:49:40.258195 djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style/templates/admin/
--rw-r--r--   0 fsbraun    (501) staff       (20)      528 2023-04-30 14:49:14.000000 djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style/templates/admin/base_site.html
-drwxr-xr-x   0 fsbraun    (501) staff       (20)        0 2023-04-30 16:49:40.257728 djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style.egg-info/
--rw-r--r--   0 fsbraun    (501) staff       (20)     4045 2023-04-30 16:49:40.000000 djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style.egg-info/PKG-INFO
--rw-r--r--   0 fsbraun    (501) staff       (20)      556 2023-04-30 16:49:40.000000 djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style.egg-info/SOURCES.txt
--rw-r--r--   0 fsbraun    (501) staff       (20)        1 2023-04-30 16:49:40.000000 djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style.egg-info/dependency_links.txt
--rw-r--r--   0 fsbraun    (501) staff       (20)        1 2023-04-30 14:56:39.000000 djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style.egg-info/not-zip-safe
--rw-r--r--   0 fsbraun    (501) staff       (20)       11 2023-04-30 16:49:40.000000 djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style.egg-info/requires.txt
--rw-r--r--   0 fsbraun    (501) staff       (20)       29 2023-04-30 16:49:40.000000 djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style.egg-info/top_level.txt
--rw-r--r--   0 fsbraun    (501) staff       (20)      559 2023-04-30 16:49:40.258717 djangocms-simple-admin-style-0.1.0/setup.cfg
--rw-r--r--   0 fsbraun    (501) staff       (20)     2309 2023-04-30 16:49:33.000000 djangocms-simple-admin-style-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:13:16.999463 djangocms-simple-admin-style-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-30 17:13:08.000000 djangocms-simple-admin-style-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-30 17:13:08.000000 djangocms-simple-admin-style-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-04-30 17:13:16.999463 djangocms-simple-admin-style-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-30 17:13:08.000000 djangocms-simple-admin-style-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:13:16.999463 djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 17:13:08.000000 djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:13:16.999463 djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:13:16.999463 djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style/static/djangocms_simple_admin_style/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:13:16.999463 djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-30 17:13:08.000000 djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/djangocms-simple-admin.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:13:16.999463 djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:13:16.999463 djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-30 17:13:08.000000 djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style/templates/admin/base_site.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:13:16.999463 djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-04-30 17:13:16.000000 djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-30 17:13:16.000000 djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 17:13:16.000000 djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 17:13:16.000000 djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 17:13:16.000000 djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-30 17:13:16.000000 djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-30 17:13:16.999463 djangocms-simple-admin-style-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-30 17:13:08.000000 djangocms-simple-admin-style-0.1.1/setup.py
```

### Comparing `djangocms-simple-admin-style-0.1.0/LICENSE` & `djangocms-simple-admin-style-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.1.0/PKG-INFO` & `djangocms-simple-admin-style-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-simple-admin-style
-Version: 0.1.0
+Version: 0.1.1
 Summary: Adds pretty CSS styles for the django CMS admin interface.
 Home-page: https://github.com/fsbraun/djangocms-simple-admin-style
 Author: Fabian Braun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `djangocms-simple-admin-style-0.1.0/README.rst` & `djangocms-simple-admin-style-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/djangocms-simple-admin.css` & `djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/djangocms-simple-admin.css`

 * *Files 3% similar despite different names*

```diff
@@ -186,7 +186,15 @@
     border: 1px solid var(--dca-gray-lighter, #ddd);
 }
 
 a.btn {
     color: var(--body-fg);
     border: 1px solid var(--dca-gray-lighter, #ddd);
 }
+
+body.cms-admin-sideframe #header {
+    display: none;
+}
+
+body.cms-admin-sideframe .breadcrumbs {
+    margin-top: 46px;
+}
```

### Comparing `djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style/templates/admin/base_site.html` & `djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style.egg-info/PKG-INFO` & `djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-simple-admin-style
-Version: 0.1.0
+Version: 0.1.1
 Summary: Adds pretty CSS styles for the django CMS admin interface.
 Home-page: https://github.com/fsbraun/djangocms-simple-admin-style
 Author: Fabian Braun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `djangocms-simple-admin-style-0.1.0/djangocms_simple_admin_style.egg-info/SOURCES.txt` & `djangocms-simple-admin-style-0.1.1/djangocms_simple_admin_style.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.1.0/setup.cfg` & `djangocms-simple-admin-style-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.1.0/setup.py` & `djangocms-simple-admin-style-0.1.1/setup.py`

 * *Files identical despite different names*

