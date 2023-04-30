# Comparing `tmp/Bigsansar-1.2.3.tar.gz` & `tmp/Bigsansar-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bigsansar-1.2.3.tar", last modified: Sun Apr 30 13:08:33 2023, max compression
+gzip compressed data, was "Bigsansar-1.2.4.tar", last modified: Sun Apr 30 13:23:17 2023, max compression
```

## Comparing `Bigsansar-1.2.3.tar` & `Bigsansar-1.2.4.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:08:33.348975 Bigsansar-1.2.3/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:08:33.308975 Bigsansar-1.2.3/Bigsansar.egg-info/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3121 2023-04-30 13:08:33.000000 Bigsansar-1.2.3/Bigsansar.egg-info/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2116 2023-04-30 13:08:33.000000 Bigsansar-1.2.3/Bigsansar.egg-info/SOURCES.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-04-30 13:08:33.000000 Bigsansar-1.2.3/Bigsansar.egg-info/dependency_links.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-04-30 13:08:33.000000 Bigsansar-1.2.3/Bigsansar.egg-info/entry_points.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       75 2023-04-30 13:08:33.000000 Bigsansar-1.2.3/Bigsansar.egg-info/requires.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-04-30 13:08:33.000000 Bigsansar-1.2.3/Bigsansar.egg-info/top_level.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/LICENSE
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3121 2023-04-30 13:08:33.348975 Bigsansar-1.2.3/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2508 2023-04-29 15:26:29.000000 Bigsansar-1.2.3/README.md
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:08:33.308975 Bigsansar-1.2.3/bigsansar/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:08:33.308975 Bigsansar-1.2.3/bigsansar/contrib/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:08:33.318975 Bigsansar-1.2.3/bigsansar/contrib/account/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/account/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/account/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/account/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/account/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:08:33.318975 Bigsansar-1.2.3/bigsansar/contrib/account/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/account/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/account/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/account/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/account/signals.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:08:33.318975 Bigsansar-1.2.3/bigsansar/contrib/account/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/account/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/account/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/account/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/account/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:08:33.328975 Bigsansar-1.2.3/bigsansar/contrib/sites/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/sites/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1393 2023-04-30 07:03:51.000000 Bigsansar-1.2.3/bigsansar/contrib/sites/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/sites/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      721 2023-04-30 07:01:55.000000 Bigsansar-1.2.3/bigsansar/contrib/sites/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:08:33.328975 Bigsansar-1.2.3/bigsansar/contrib/sites/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1816 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/sites/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      387 2023-04-29 15:42:28.000000 Bigsansar-1.2.3/bigsansar/contrib/sites/migrations/0002_domains_description.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      422 2023-04-30 05:58:24.000000 Bigsansar-1.2.3/bigsansar/contrib/sites/migrations/0003_alter_pages_body.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/sites/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1954 2023-04-30 05:57:56.000000 Bigsansar-1.2.3/bigsansar/contrib/sites/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:08:33.348975 Bigsansar-1.2.3/bigsansar/contrib/sites/templatetags/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/sites/templatetags/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/sites/templatetags/pages.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/sites/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/contrib/sites/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:08:33.348975 Bigsansar-1.2.3/bigsansar/core/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/core/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/core/host.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9177 2023-04-30 08:01:38.000000 Bigsansar-1.2.3/bigsansar/core/init.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/main.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:08:33.348975 Bigsansar-1.2.3/bigsansar/management/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/management/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:08:33.348975 Bigsansar-1.2.3/bigsansar/management/commands/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/management/commands/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.2.3/bigsansar/management/commands/createuser.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:08:33.348975 Bigsansar-1.2.3/bigsansar/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:08:33.348975 Bigsansar-1.2.3/bigsansar/static/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/static/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/static/logo.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/static/style.css
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:08:33.348975 Bigsansar-1.2.3/bigsansar/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/templates/404.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/templates/acc_active_email.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1134 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/templates/base.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/templates/default.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/templates/defaultpage.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2171 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/templates/nav.html
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:08:33.348975 Bigsansar-1.2.3/bigsansar/templates/page/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       14 2023-04-30 07:35:31.000000 Bigsansar-1.2.3/bigsansar/templates/page/default.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/templates/parking.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.3/bigsansar/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1046 2023-04-30 07:26:30.000000 Bigsansar-1.2.3/bigsansar/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1887 2023-04-30 13:08:04.000000 Bigsansar-1.2.3/bigsansar/views.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-04-30 13:08:33.348975 Bigsansar-1.2.3/setup.cfg
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1304 2023-04-30 13:08:17.000000 Bigsansar-1.2.3/setup.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:23:17.668971 Bigsansar-1.2.4/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:23:17.628971 Bigsansar-1.2.4/Bigsansar.egg-info/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3121 2023-04-30 13:23:17.000000 Bigsansar-1.2.4/Bigsansar.egg-info/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2116 2023-04-30 13:23:17.000000 Bigsansar-1.2.4/Bigsansar.egg-info/SOURCES.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-04-30 13:23:17.000000 Bigsansar-1.2.4/Bigsansar.egg-info/dependency_links.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-04-30 13:23:17.000000 Bigsansar-1.2.4/Bigsansar.egg-info/entry_points.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       75 2023-04-30 13:23:17.000000 Bigsansar-1.2.4/Bigsansar.egg-info/requires.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-04-30 13:23:17.000000 Bigsansar-1.2.4/Bigsansar.egg-info/top_level.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/LICENSE
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3121 2023-04-30 13:23:17.668971 Bigsansar-1.2.4/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2508 2023-04-29 15:26:29.000000 Bigsansar-1.2.4/README.md
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:23:17.628971 Bigsansar-1.2.4/bigsansar/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:23:17.628971 Bigsansar-1.2.4/bigsansar/contrib/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:23:17.638971 Bigsansar-1.2.4/bigsansar/contrib/account/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/account/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/account/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/account/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/account/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:23:17.648971 Bigsansar-1.2.4/bigsansar/contrib/account/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/account/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/account/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/account/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/account/signals.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:23:17.648971 Bigsansar-1.2.4/bigsansar/contrib/account/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/account/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/account/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/account/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/account/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:23:17.648971 Bigsansar-1.2.4/bigsansar/contrib/sites/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/sites/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1393 2023-04-30 07:03:51.000000 Bigsansar-1.2.4/bigsansar/contrib/sites/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/sites/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      721 2023-04-30 07:01:55.000000 Bigsansar-1.2.4/bigsansar/contrib/sites/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:23:17.648971 Bigsansar-1.2.4/bigsansar/contrib/sites/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1816 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/sites/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      387 2023-04-29 15:42:28.000000 Bigsansar-1.2.4/bigsansar/contrib/sites/migrations/0002_domains_description.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      422 2023-04-30 05:58:24.000000 Bigsansar-1.2.4/bigsansar/contrib/sites/migrations/0003_alter_pages_body.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/sites/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1954 2023-04-30 05:57:56.000000 Bigsansar-1.2.4/bigsansar/contrib/sites/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:23:17.648971 Bigsansar-1.2.4/bigsansar/contrib/sites/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/sites/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/sites/templatetags/pages.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/sites/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/contrib/sites/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:23:17.648971 Bigsansar-1.2.4/bigsansar/core/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/core/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/core/host.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9177 2023-04-30 08:01:38.000000 Bigsansar-1.2.4/bigsansar/core/init.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/main.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:23:17.648971 Bigsansar-1.2.4/bigsansar/management/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/management/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:23:17.648971 Bigsansar-1.2.4/bigsansar/management/commands/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/management/commands/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.2.4/bigsansar/management/commands/createuser.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:23:17.648971 Bigsansar-1.2.4/bigsansar/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:23:17.658971 Bigsansar-1.2.4/bigsansar/static/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/static/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/static/logo.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/static/style.css
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:23:17.668971 Bigsansar-1.2.4/bigsansar/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/templates/404.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/templates/acc_active_email.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1134 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/templates/base.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/templates/default.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/templates/defaultpage.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2171 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/templates/nav.html
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-30 13:23:17.668971 Bigsansar-1.2.4/bigsansar/templates/page/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       14 2023-04-30 07:35:31.000000 Bigsansar-1.2.4/bigsansar/templates/page/default.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/templates/parking.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.4/bigsansar/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1046 2023-04-30 07:26:30.000000 Bigsansar-1.2.4/bigsansar/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1849 2023-04-30 13:22:53.000000 Bigsansar-1.2.4/bigsansar/views.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-04-30 13:23:17.668971 Bigsansar-1.2.4/setup.cfg
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1304 2023-04-30 13:23:01.000000 Bigsansar-1.2.4/setup.py
```

### Comparing `Bigsansar-1.2.3/Bigsansar.egg-info/PKG-INFO` & `Bigsansar-1.2.4/Bigsansar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.2.3
+Version: 1.2.4
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
```

### Comparing `Bigsansar-1.2.3/Bigsansar.egg-info/SOURCES.txt` & `Bigsansar-1.2.4/Bigsansar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/LICENSE` & `Bigsansar-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/PKG-INFO` & `Bigsansar-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.2.3
+Version: 1.2.4
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
```

### Comparing `Bigsansar-1.2.3/README.md` & `Bigsansar-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/contrib/account/forms.py` & `Bigsansar-1.2.4/bigsansar/contrib/account/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/contrib/account/migrations/0001_initial.py` & `Bigsansar-1.2.4/bigsansar/contrib/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/contrib/account/models.py` & `Bigsansar-1.2.4/bigsansar/contrib/account/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/contrib/sites/admin.py` & `Bigsansar-1.2.4/bigsansar/contrib/sites/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/contrib/sites/forms.py` & `Bigsansar-1.2.4/bigsansar/contrib/sites/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/contrib/sites/migrations/0001_initial.py` & `Bigsansar-1.2.4/bigsansar/contrib/sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/contrib/sites/models.py` & `Bigsansar-1.2.4/bigsansar/contrib/sites/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/core/__init__.py` & `Bigsansar-1.2.4/bigsansar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/core/init.py` & `Bigsansar-1.2.4/bigsansar/core/init.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/management/commands/createuser.py` & `Bigsansar-1.2.4/bigsansar/management/commands/createuser.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/static/logo.png` & `Bigsansar-1.2.4/bigsansar/static/logo.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/static/style.css` & `Bigsansar-1.2.4/bigsansar/static/style.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/templates/404.html` & `Bigsansar-1.2.4/bigsansar/templates/404.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/templates/base.html` & `Bigsansar-1.2.4/bigsansar/templates/base.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/templates/default.html` & `Bigsansar-1.2.4/bigsansar/templates/default.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/templates/defaultpage.html` & `Bigsansar-1.2.4/bigsansar/templates/defaultpage.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/templates/nav.html` & `Bigsansar-1.2.4/bigsansar/templates/nav.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/templates/parking.html` & `Bigsansar-1.2.4/bigsansar/templates/parking.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/urls.py` & `Bigsansar-1.2.4/bigsansar/urls.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.3/bigsansar/views.py` & `Bigsansar-1.2.4/bigsansar/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,22 +21,24 @@
 
     except:
         current_site = get_current_site(request)
         time = datetime.datetime.now()
         return render(request, 'parking.html', {'domain': current_site, 'time': time})
 
     else:
+        try:
+            pages.objects.get(domain=db, slug='index')
         
-        if pages.objects.get(domain=db, slug='index'):
-            template = loader.get_template('page/default.html')
+        except:
+            return render(request, 'default.html')
         
         else:
-            template = loader.get_template('default.html')
+            return render(request, 'page/default.html')
         
-        return HttpResponse(template.render({}, request))
+    
 def pathviews(request, url):
     default_page = 'defaultpage.html'
 
     try:
         current_site = get_current_site(request)
         db = domains.objects.get(domain=current_site)
         get_pagename = url.strip('/')
```

### Comparing `Bigsansar-1.2.3/setup.py` & `Bigsansar-1.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Bigsansar",
-    version="1.2.3",
+    version="1.2.4",
     author="Bikash Pokhrel",
     author_email="bigsansaroffice@gmail.com",
     description="Build one in minutes with bigsansar - a visual site building tool!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bigsansar.com",
     project_urls={
```

