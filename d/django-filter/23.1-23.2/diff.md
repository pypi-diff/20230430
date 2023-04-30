# Comparing `tmp/django-filter-23.1.tar.gz` & `tmp/django-filter-23.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-filter-23.1.tar", last modified: Sun Mar 26 09:46:12 2023, max compression
+gzip compressed data, was "django-filter-23.2.tar", last modified: Sun Apr 30 09:11:57 2023, max compression
```

## Comparing `django-filter-23.1.tar` & `django-filter-23.2.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.358661 django-filter-23.1/
--rw-r--r--   0 carlton    (501) staff       (20)      329 2021-11-10 09:12:06.000000 django-filter-23.1/AUTHORS
--rw-r--r--   0 carlton    (501) staff       (20)    14031 2023-03-26 09:40:57.000000 django-filter-23.1/CHANGES.rst
--rw-r--r--   0 carlton    (501) staff       (20)     1487 2021-11-10 09:12:06.000000 django-filter-23.1/LICENSE
--rw-r--r--   0 carlton    (501) staff       (20)      356 2021-11-10 09:12:06.000000 django-filter-23.1/MANIFEST.in
--rw-r--r--   0 carlton    (501) staff       (20)     5099 2023-03-26 09:46:12.358746 django-filter-23.1/PKG-INFO
--rw-r--r--   0 carlton    (501) staff       (20)     3588 2021-11-10 09:12:06.000000 django-filter-23.1/README.rst
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.342915 django-filter-23.1/django_filter.egg-info/
--rw-r--r--   0 carlton    (501) staff       (20)     5099 2023-03-26 09:46:12.000000 django-filter-23.1/django_filter.egg-info/PKG-INFO
--rw-r--r--   0 carlton    (501) staff       (20)     3843 2023-03-26 09:46:12.000000 django-filter-23.1/django_filter.egg-info/SOURCES.txt
--rw-r--r--   0 carlton    (501) staff       (20)        1 2023-03-26 09:46:12.000000 django-filter-23.1/django_filter.egg-info/dependency_links.txt
--rw-r--r--   0 carlton    (501) staff       (20)        1 2021-12-16 14:01:17.000000 django-filter-23.1/django_filter.egg-info/not-zip-safe
--rw-r--r--   0 carlton    (501) staff       (20)       12 2023-03-26 09:46:12.000000 django-filter-23.1/django_filter.egg-info/requires.txt
--rw-r--r--   0 carlton    (501) staff       (20)       15 2023-03-26 09:46:12.000000 django-filter-23.1/django_filter.egg-info/top_level.txt
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.344379 django-filter-23.1/django_filters/
--rw-r--r--   0 carlton    (501) staff       (20)      644 2023-03-26 09:41:18.000000 django-filter-23.1/django_filters/__init__.py
--rw-r--r--   0 carlton    (501) staff       (20)      545 2022-06-17 14:23:37.000000 django-filter-23.1/django_filters/compat.py
--rw-r--r--   0 carlton    (501) staff       (20)     3049 2022-06-17 14:23:37.000000 django-filter-23.1/django_filters/conf.py
--rw-r--r--   0 carlton    (501) staff       (20)       63 2022-06-17 14:23:37.000000 django-filter-23.1/django_filters/constants.py
--rw-r--r--   0 carlton    (501) staff       (20)      253 2022-06-17 14:23:37.000000 django-filter-23.1/django_filters/exceptions.py
--rw-r--r--   0 carlton    (501) staff       (20)     9784 2022-06-17 14:33:37.000000 django-filter-23.1/django_filters/fields.py
--rw-r--r--   0 carlton    (501) staff       (20)    24935 2023-03-26 09:14:56.000000 django-filter-23.1/django_filters/filters.py
--rw-r--r--   0 carlton    (501) staff       (20)    15928 2022-06-17 14:33:37.000000 django-filter-23.1/django_filters/filterset.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.338656 django-filter-23.1/django_filters/locale/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.335881 django-filter-23.1/django_filters/locale/ar/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.344696 django-filter-23.1/django_filters/locale/ar/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     2568 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 carlton    (501) staff       (20)     3625 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.336015 django-filter-23.1/django_filters/locale/be/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.344982 django-filter-23.1/django_filters/locale/be/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     2819 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/locale/be/LC_MESSAGES/django.mo
--rw-r--r--   0 carlton    (501) staff       (20)     3696 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/be/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.336149 django-filter-23.1/django_filters/locale/bg/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.345332 django-filter-23.1/django_filters/locale/bg/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     2711 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 carlton    (501) staff       (20)     3740 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.336284 django-filter-23.1/django_filters/locale/cs/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.345665 django-filter-23.1/django_filters/locale/cs/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     2368 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 carlton    (501) staff       (20)     3242 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.336413 django-filter-23.1/django_filters/locale/da/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.346000 django-filter-23.1/django_filters/locale/da/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     2166 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0 carlton    (501) staff       (20)     3173 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.336561 django-filter-23.1/django_filters/locale/de/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.346282 django-filter-23.1/django_filters/locale/de/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     2277 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 carlton    (501) staff       (20)     3338 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.336689 django-filter-23.1/django_filters/locale/el/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.346547 django-filter-23.1/django_filters/locale/el/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     2836 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 carlton    (501) staff       (20)     3909 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.336813 django-filter-23.1/django_filters/locale/es/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.346828 django-filter-23.1/django_filters/locale/es/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     2279 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 carlton    (501) staff       (20)     3426 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.336932 django-filter-23.1/django_filters/locale/es_AR/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.347119 django-filter-23.1/django_filters/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)      703 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0 carlton    (501) staff       (20)     3035 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.337046 django-filter-23.1/django_filters/locale/fa/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.347413 django-filter-23.1/django_filters/locale/fa/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     2624 2023-03-26 09:14:56.000000 django-filter-23.1/django_filters/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 carlton    (501) staff       (20)     3623 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.337169 django-filter-23.1/django_filters/locale/fi/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.347568 django-filter-23.1/django_filters/locale/fi/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     3433 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.337287 django-filter-23.1/django_filters/locale/fr/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.348001 django-filter-23.1/django_filters/locale/fr/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     2360 2023-03-26 09:14:56.000000 django-filter-23.1/django_filters/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 carlton    (501) staff       (20)     3429 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.337426 django-filter-23.1/django_filters/locale/it/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.348377 django-filter-23.1/django_filters/locale/it/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     2268 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 carlton    (501) staff       (20)     3290 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.337556 django-filter-23.1/django_filters/locale/nl/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.348558 django-filter-23.1/django_filters/locale/nl/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     2794 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.337701 django-filter-23.1/django_filters/locale/pl/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.348969 django-filter-23.1/django_filters/locale/pl/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     1859 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 carlton    (501) staff       (20)     3551 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.337930 django-filter-23.1/django_filters/locale/pt_BR/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.349600 django-filter-23.1/django_filters/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     2263 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 carlton    (501) staff       (20)     3298 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.338162 django-filter-23.1/django_filters/locale/ro/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.349820 django-filter-23.1/django_filters/locale/ro/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     3478 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.338286 django-filter-23.1/django_filters/locale/ru/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.350185 django-filter-23.1/django_filters/locale/ru/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     2796 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 carlton    (501) staff       (20)     3863 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.338404 django-filter-23.1/django_filters/locale/sk/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.350555 django-filter-23.1/django_filters/locale/sk/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     2394 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 carlton    (501) staff       (20)     3467 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.338530 django-filter-23.1/django_filters/locale/uk/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.350983 django-filter-23.1/django_filters/locale/uk/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)     2912 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 carlton    (501) staff       (20)     3792 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.338731 django-filter-23.1/django_filters/locale/zh_CN/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.351320 django-filter-23.1/django_filters/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 carlton    (501) staff       (20)      852 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 carlton    (501) staff       (20)     3123 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.351896 django-filter-23.1/django_filters/rest_framework/
--rw-r--r--   0 carlton    (501) staff       (20)      113 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/rest_framework/__init__.py
--rw-r--r--   0 carlton    (501) staff       (20)     5284 2022-06-17 14:23:37.000000 django-filter-23.1/django_filters/rest_framework/backends.py
--rw-r--r--   0 carlton    (501) staff       (20)      312 2022-06-17 14:23:37.000000 django-filter-23.1/django_filters/rest_framework/filters.py
--rw-r--r--   0 carlton    (501) staff       (20)     1174 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/rest_framework/filterset.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.339021 django-filter-23.1/django_filters/templates/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.339199 django-filter-23.1/django_filters/templates/django_filters/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.352192 django-filter-23.1/django_filters/templates/django_filters/rest_framework/
--rw-r--r--   0 carlton    (501) staff       (20)      108 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/templates/django_filters/rest_framework/crispy_form.html
--rw-r--r--   0 carlton    (501) staff       (20)      211 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/templates/django_filters/rest_framework/form.html
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.352345 django-filter-23.1/django_filters/templates/django_filters/widgets/
--rw-r--r--   0 carlton    (501) staff       (20)      118 2021-11-10 09:12:06.000000 django-filter-23.1/django_filters/templates/django_filters/widgets/multiwidget.html
--rw-r--r--   0 carlton    (501) staff       (20)    10789 2023-03-26 09:29:15.000000 django-filter-23.1/django_filters/utils.py
--rw-r--r--   0 carlton    (501) staff       (20)     4034 2022-06-17 14:33:36.000000 django-filter-23.1/django_filters/views.py
--rw-r--r--   0 carlton    (501) staff       (20)     9021 2023-03-26 09:30:42.000000 django-filter-23.1/django_filters/widgets.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.353116 django-filter-23.1/docs/
--rw-r--r--   0 carlton    (501) staff       (20)     5662 2021-11-10 09:12:06.000000 django-filter-23.1/docs/Makefile
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.353304 django-filter-23.1/docs/assets/
--rw-r--r--   0 carlton    (501) staff       (20)    13678 2021-11-10 09:12:06.000000 django-filter-23.1/docs/assets/form.png
--rw-r--r--   0 carlton    (501) staff       (20)     8481 2022-06-17 14:33:27.000000 django-filter-23.1/docs/conf.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.353465 django-filter-23.1/docs/dev/
--rw-r--r--   0 carlton    (501) staff       (20)     1943 2021-11-10 09:12:06.000000 django-filter-23.1/docs/dev/tests.txt
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.354125 django-filter-23.1/docs/guide/
--rw-r--r--   0 carlton    (501) staff       (20)      622 2021-11-10 09:12:06.000000 django-filter-23.1/docs/guide/install.txt
--rw-r--r--   0 carlton    (501) staff       (20)    11203 2021-11-10 09:12:06.000000 django-filter-23.1/docs/guide/migration.txt
--rw-r--r--   0 carlton    (501) staff       (20)     7864 2021-11-10 09:12:06.000000 django-filter-23.1/docs/guide/rest_framework.txt
--rw-r--r--   0 carlton    (501) staff       (20)    10169 2021-11-10 09:12:06.000000 django-filter-23.1/docs/guide/tips.txt
--rw-r--r--   0 carlton    (501) staff       (20)    11261 2023-03-26 09:29:15.000000 django-filter-23.1/docs/guide/usage.txt
--rw-r--r--   0 carlton    (501) staff       (20)      668 2021-11-10 09:12:06.000000 django-filter-23.1/docs/index.txt
--rw-r--r--   0 carlton    (501) staff       (20)     5110 2021-11-10 09:12:06.000000 django-filter-23.1/docs/make.bat
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.354761 django-filter-23.1/docs/ref/
--rw-r--r--   0 carlton    (501) staff       (20)      850 2021-11-10 09:12:06.000000 django-filter-23.1/docs/ref/fields.txt
--rw-r--r--   0 carlton    (501) staff       (20)    27495 2022-06-16 15:11:02.000000 django-filter-23.1/docs/ref/filters.txt
--rw-r--r--   0 carlton    (501) staff       (20)     6583 2021-11-10 09:12:06.000000 django-filter-23.1/docs/ref/filterset.txt
--rw-r--r--   0 carlton    (501) staff       (20)     2711 2021-11-10 09:12:06.000000 django-filter-23.1/docs/ref/settings.txt
--rw-r--r--   0 carlton    (501) staff       (20)     2435 2023-03-26 09:29:15.000000 django-filter-23.1/docs/ref/widgets.txt
--rw-r--r--   0 carlton    (501) staff       (20)       90 2021-11-10 09:12:06.000000 django-filter-23.1/pyproject.toml
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.355174 django-filter-23.1/requirements/
--rw-r--r--   0 carlton    (501) staff       (20)       18 2021-11-10 09:12:06.000000 django-filter-23.1/requirements/maintainer.txt
--rw-r--r--   0 carlton    (501) staff       (20)       75 2021-11-10 09:12:06.000000 django-filter-23.1/requirements/test-ci.txt
--rw-r--r--   0 carlton    (501) staff       (20)       42 2021-11-10 09:12:06.000000 django-filter-23.1/requirements/test.txt
--rwxr-xr-x   0 carlton    (501) staff       (20)      390 2022-06-17 14:33:27.000000 django-filter-23.1/runshell.py
--rwxr-xr-x   0 carlton    (501) staff       (20)      323 2022-06-17 14:33:27.000000 django-filter-23.1/runtests.py
--rw-r--r--   0 carlton    (501) staff       (20)      244 2023-03-26 09:46:12.359138 django-filter-23.1/setup.cfg
--rw-r--r--   0 carlton    (501) staff       (20)     2636 2023-03-26 09:41:10.000000 django-filter-23.1/setup.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.357265 django-filter-23.1/tests/
--rw-r--r--   0 carlton    (501) staff       (20)        0 2021-11-10 09:12:06.000000 django-filter-23.1/tests/__init__.py
--rw-r--r--   0 carlton    (501) staff       (20)     5347 2022-06-17 14:23:37.000000 django-filter-23.1/tests/models.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.358148 django-filter-23.1/tests/rest_framework/
--rw-r--r--   0 carlton    (501) staff       (20)       73 2022-06-17 14:23:37.000000 django-filter-23.1/tests/rest_framework/__init__.py
--rw-r--r--   0 carlton    (501) staff       (20)      184 2022-06-17 14:23:37.000000 django-filter-23.1/tests/rest_framework/apps.py
--rw-r--r--   0 carlton    (501) staff       (20)      809 2022-06-17 14:23:37.000000 django-filter-23.1/tests/rest_framework/models.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.358315 django-filter-23.1/tests/rest_framework/templates/
--rw-r--r--   0 carlton    (501) staff       (20)        5 2021-11-10 09:12:06.000000 django-filter-23.1/tests/rest_framework/templates/filter_template.html
--rw-r--r--   0 carlton    (501) staff       (20)    14423 2022-06-17 14:33:37.000000 django-filter-23.1/tests/rest_framework/test_backends.py
--rw-r--r--   0 carlton    (501) staff       (20)     1080 2022-06-17 14:23:37.000000 django-filter-23.1/tests/rest_framework/test_filters.py
--rw-r--r--   0 carlton    (501) staff       (20)     1867 2023-02-10 10:37:27.000000 django-filter-23.1/tests/rest_framework/test_filterset.py
--rw-r--r--   0 carlton    (501) staff       (20)    15593 2022-06-17 14:33:37.000000 django-filter-23.1/tests/rest_framework/test_integration.py
--rw-r--r--   0 carlton    (501) staff       (20)      889 2022-06-17 14:23:37.000000 django-filter-23.1/tests/settings.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.340248 django-filter-23.1/tests/templates/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-03-26 09:46:12.358528 django-filter-23.1/tests/templates/tests/
--rw-r--r--   0 carlton    (501) staff       (20)       75 2021-11-10 09:12:06.000000 django-filter-23.1/tests/templates/tests/book_filter.html
--rw-r--r--   0 carlton    (501) staff       (20)     3429 2022-06-17 14:23:37.000000 django-filter-23.1/tests/test_conf.py
--rw-r--r--   0 carlton    (501) staff       (20)    10525 2023-03-26 09:29:15.000000 django-filter-23.1/tests/test_fields.py
--rw-r--r--   0 carlton    (501) staff       (20)    72621 2023-03-26 09:36:20.000000 django-filter-23.1/tests/test_filtering.py
--rw-r--r--   0 carlton    (501) staff       (20)    56378 2023-03-26 09:14:56.000000 django-filter-23.1/tests/test_filters.py
--rw-r--r--   0 carlton    (501) staff       (20)    32240 2023-03-26 09:14:56.000000 django-filter-23.1/tests/test_filterset.py
--rw-r--r--   0 carlton    (501) staff       (20)     8459 2022-06-17 14:23:37.000000 django-filter-23.1/tests/test_forms.py
--rw-r--r--   0 carlton    (501) staff       (20)    20489 2023-03-26 09:29:15.000000 django-filter-23.1/tests/test_utils.py
--rw-r--r--   0 carlton    (501) staff       (20)     5484 2022-06-17 14:23:37.000000 django-filter-23.1/tests/test_views.py
--rw-r--r--   0 carlton    (501) staff       (20)    17436 2022-06-17 14:33:37.000000 django-filter-23.1/tests/test_widgets.py
--rw-r--r--   0 carlton    (501) staff       (20)      354 2022-06-17 14:23:37.000000 django-filter-23.1/tests/urls.py
--rw-r--r--   0 carlton    (501) staff       (20)      381 2022-06-17 14:23:37.000000 django-filter-23.1/tests/utils.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.379596 django-filter-23.2/
+-rw-r--r--   0 carlton    (501) staff       (20)      329 2021-11-10 09:12:06.000000 django-filter-23.2/AUTHORS
+-rw-r--r--   0 carlton    (501) staff       (20)    14706 2023-04-30 09:10:39.000000 django-filter-23.2/CHANGES.rst
+-rw-r--r--   0 carlton    (501) staff       (20)     1487 2021-11-10 09:12:06.000000 django-filter-23.2/LICENSE
+-rw-r--r--   0 carlton    (501) staff       (20)      356 2021-11-10 09:12:06.000000 django-filter-23.2/MANIFEST.in
+-rw-r--r--   0 carlton    (501) staff       (20)     5099 2023-04-30 09:11:57.379682 django-filter-23.2/PKG-INFO
+-rw-r--r--   0 carlton    (501) staff       (20)     3588 2021-11-10 09:12:06.000000 django-filter-23.2/README.rst
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.358437 django-filter-23.2/django_filter.egg-info/
+-rw-r--r--   0 carlton    (501) staff       (20)     5099 2023-04-30 09:11:57.000000 django-filter-23.2/django_filter.egg-info/PKG-INFO
+-rw-r--r--   0 carlton    (501) staff       (20)     3843 2023-04-30 09:11:57.000000 django-filter-23.2/django_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 carlton    (501) staff       (20)        1 2023-04-30 09:11:57.000000 django-filter-23.2/django_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 carlton    (501) staff       (20)        1 2023-04-30 09:11:57.000000 django-filter-23.2/django_filter.egg-info/not-zip-safe
+-rw-r--r--   0 carlton    (501) staff       (20)       12 2023-04-30 09:11:57.000000 django-filter-23.2/django_filter.egg-info/requires.txt
+-rw-r--r--   0 carlton    (501) staff       (20)       15 2023-04-30 09:11:57.000000 django-filter-23.2/django_filter.egg-info/top_level.txt
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.361030 django-filter-23.2/django_filters/
+-rw-r--r--   0 carlton    (501) staff       (20)      766 2023-04-30 09:10:39.000000 django-filter-23.2/django_filters/__init__.py
+-rw-r--r--   0 carlton    (501) staff       (20)      711 2023-04-30 09:10:30.000000 django-filter-23.2/django_filters/compat.py
+-rw-r--r--   0 carlton    (501) staff       (20)     3049 2022-06-17 14:23:37.000000 django-filter-23.2/django_filters/conf.py
+-rw-r--r--   0 carlton    (501) staff       (20)       63 2022-06-17 14:23:37.000000 django-filter-23.2/django_filters/constants.py
+-rw-r--r--   0 carlton    (501) staff       (20)      253 2022-06-17 14:23:37.000000 django-filter-23.2/django_filters/exceptions.py
+-rw-r--r--   0 carlton    (501) staff       (20)     9784 2022-06-17 14:33:37.000000 django-filter-23.2/django_filters/fields.py
+-rw-r--r--   0 carlton    (501) staff       (20)    24935 2023-03-26 09:14:56.000000 django-filter-23.2/django_filters/filters.py
+-rw-r--r--   0 carlton    (501) staff       (20)    15928 2022-06-17 14:33:37.000000 django-filter-23.2/django_filters/filterset.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.354855 django-filter-23.2/django_filters/locale/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.352434 django-filter-23.2/django_filters/locale/ar/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.361530 django-filter-23.2/django_filters/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     2568 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 carlton    (501) staff       (20)     3625 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.352556 django-filter-23.2/django_filters/locale/be/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.362033 django-filter-23.2/django_filters/locale/be/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     2819 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/locale/be/LC_MESSAGES/django.mo
+-rw-r--r--   0 carlton    (501) staff       (20)     3696 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/be/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.352681 django-filter-23.2/django_filters/locale/bg/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.362484 django-filter-23.2/django_filters/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     2711 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 carlton    (501) staff       (20)     3740 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.352797 django-filter-23.2/django_filters/locale/cs/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.363013 django-filter-23.2/django_filters/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     2368 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 carlton    (501) staff       (20)     3242 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.352910 django-filter-23.2/django_filters/locale/da/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.363510 django-filter-23.2/django_filters/locale/da/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     2166 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0 carlton    (501) staff       (20)     3173 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.353020 django-filter-23.2/django_filters/locale/de/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.364007 django-filter-23.2/django_filters/locale/de/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     2277 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 carlton    (501) staff       (20)     3338 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.353134 django-filter-23.2/django_filters/locale/el/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.364406 django-filter-23.2/django_filters/locale/el/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     2836 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 carlton    (501) staff       (20)     3909 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.353249 django-filter-23.2/django_filters/locale/es/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.364787 django-filter-23.2/django_filters/locale/es/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     2279 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 carlton    (501) staff       (20)     3426 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.353369 django-filter-23.2/django_filters/locale/es_AR/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.365196 django-filter-23.2/django_filters/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)      703 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 carlton    (501) staff       (20)     3035 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.353479 django-filter-23.2/django_filters/locale/fa/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.365576 django-filter-23.2/django_filters/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     2624 2023-03-26 09:14:56.000000 django-filter-23.2/django_filters/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 carlton    (501) staff       (20)     3623 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.353593 django-filter-23.2/django_filters/locale/fi/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.365866 django-filter-23.2/django_filters/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     3433 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.353709 django-filter-23.2/django_filters/locale/fr/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.366276 django-filter-23.2/django_filters/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     2360 2023-03-26 09:14:56.000000 django-filter-23.2/django_filters/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 carlton    (501) staff       (20)     3429 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.353837 django-filter-23.2/django_filters/locale/it/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.366686 django-filter-23.2/django_filters/locale/it/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     2268 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 carlton    (501) staff       (20)     3290 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.353968 django-filter-23.2/django_filters/locale/nl/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.366844 django-filter-23.2/django_filters/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     2794 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.354122 django-filter-23.2/django_filters/locale/pl/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.367281 django-filter-23.2/django_filters/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     1859 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 carlton    (501) staff       (20)     3720 2023-04-30 09:10:30.000000 django-filter-23.2/django_filters/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.354292 django-filter-23.2/django_filters/locale/pt_BR/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.367563 django-filter-23.2/django_filters/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     2263 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 carlton    (501) staff       (20)     3298 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.354426 django-filter-23.2/django_filters/locale/ro/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.367720 django-filter-23.2/django_filters/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     3478 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.354542 django-filter-23.2/django_filters/locale/ru/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.368015 django-filter-23.2/django_filters/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     2796 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 carlton    (501) staff       (20)     3863 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.354661 django-filter-23.2/django_filters/locale/sk/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.368312 django-filter-23.2/django_filters/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     2394 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 carlton    (501) staff       (20)     3467 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.354781 django-filter-23.2/django_filters/locale/uk/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.368636 django-filter-23.2/django_filters/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)     2912 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 carlton    (501) staff       (20)     3792 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.354902 django-filter-23.2/django_filters/locale/zh_CN/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.368928 django-filter-23.2/django_filters/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 carlton    (501) staff       (20)      852 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 carlton    (501) staff       (20)     3123 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.369655 django-filter-23.2/django_filters/rest_framework/
+-rw-r--r--   0 carlton    (501) staff       (20)      113 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/rest_framework/__init__.py
+-rw-r--r--   0 carlton    (501) staff       (20)     5744 2023-04-30 09:10:30.000000 django-filter-23.2/django_filters/rest_framework/backends.py
+-rw-r--r--   0 carlton    (501) staff       (20)      312 2022-06-17 14:23:37.000000 django-filter-23.2/django_filters/rest_framework/filters.py
+-rw-r--r--   0 carlton    (501) staff       (20)     1174 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/rest_framework/filterset.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.355128 django-filter-23.2/django_filters/templates/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.355273 django-filter-23.2/django_filters/templates/django_filters/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.370025 django-filter-23.2/django_filters/templates/django_filters/rest_framework/
+-rw-r--r--   0 carlton    (501) staff       (20)      108 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/templates/django_filters/rest_framework/crispy_form.html
+-rw-r--r--   0 carlton    (501) staff       (20)      211 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/templates/django_filters/rest_framework/form.html
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.370228 django-filter-23.2/django_filters/templates/django_filters/widgets/
+-rw-r--r--   0 carlton    (501) staff       (20)      118 2021-11-10 09:12:06.000000 django-filter-23.2/django_filters/templates/django_filters/widgets/multiwidget.html
+-rw-r--r--   0 carlton    (501) staff       (20)    10789 2023-03-26 09:29:15.000000 django-filter-23.2/django_filters/utils.py
+-rw-r--r--   0 carlton    (501) staff       (20)     4034 2022-06-17 14:33:36.000000 django-filter-23.2/django_filters/views.py
+-rw-r--r--   0 carlton    (501) staff       (20)     9021 2023-03-26 09:30:42.000000 django-filter-23.2/django_filters/widgets.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.371032 django-filter-23.2/docs/
+-rw-r--r--   0 carlton    (501) staff       (20)     5662 2021-11-10 09:12:06.000000 django-filter-23.2/docs/Makefile
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.371210 django-filter-23.2/docs/assets/
+-rw-r--r--   0 carlton    (501) staff       (20)    13678 2021-11-10 09:12:06.000000 django-filter-23.2/docs/assets/form.png
+-rw-r--r--   0 carlton    (501) staff       (20)     8481 2022-06-17 14:33:27.000000 django-filter-23.2/docs/conf.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.371404 django-filter-23.2/docs/dev/
+-rw-r--r--   0 carlton    (501) staff       (20)     1943 2021-11-10 09:12:06.000000 django-filter-23.2/docs/dev/tests.txt
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.372309 django-filter-23.2/docs/guide/
+-rw-r--r--   0 carlton    (501) staff       (20)      622 2021-11-10 09:12:06.000000 django-filter-23.2/docs/guide/install.txt
+-rw-r--r--   0 carlton    (501) staff       (20)    11203 2021-11-10 09:12:06.000000 django-filter-23.2/docs/guide/migration.txt
+-rw-r--r--   0 carlton    (501) staff       (20)     7864 2021-11-10 09:12:06.000000 django-filter-23.2/docs/guide/rest_framework.txt
+-rw-r--r--   0 carlton    (501) staff       (20)    10169 2021-11-10 09:12:06.000000 django-filter-23.2/docs/guide/tips.txt
+-rw-r--r--   0 carlton    (501) staff       (20)    11261 2023-03-26 09:29:15.000000 django-filter-23.2/docs/guide/usage.txt
+-rw-r--r--   0 carlton    (501) staff       (20)      668 2021-11-10 09:12:06.000000 django-filter-23.2/docs/index.txt
+-rw-r--r--   0 carlton    (501) staff       (20)     5110 2021-11-10 09:12:06.000000 django-filter-23.2/docs/make.bat
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.373509 django-filter-23.2/docs/ref/
+-rw-r--r--   0 carlton    (501) staff       (20)      850 2021-11-10 09:12:06.000000 django-filter-23.2/docs/ref/fields.txt
+-rw-r--r--   0 carlton    (501) staff       (20)    27495 2022-06-16 15:11:02.000000 django-filter-23.2/docs/ref/filters.txt
+-rw-r--r--   0 carlton    (501) staff       (20)     6583 2021-11-10 09:12:06.000000 django-filter-23.2/docs/ref/filterset.txt
+-rw-r--r--   0 carlton    (501) staff       (20)     2711 2021-11-10 09:12:06.000000 django-filter-23.2/docs/ref/settings.txt
+-rw-r--r--   0 carlton    (501) staff       (20)     2435 2023-03-26 09:29:15.000000 django-filter-23.2/docs/ref/widgets.txt
+-rw-r--r--   0 carlton    (501) staff       (20)       90 2021-11-10 09:12:06.000000 django-filter-23.2/pyproject.toml
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.373918 django-filter-23.2/requirements/
+-rw-r--r--   0 carlton    (501) staff       (20)       18 2021-11-10 09:12:06.000000 django-filter-23.2/requirements/maintainer.txt
+-rw-r--r--   0 carlton    (501) staff       (20)       67 2023-04-30 09:10:30.000000 django-filter-23.2/requirements/test-ci.txt
+-rw-r--r--   0 carlton    (501) staff       (20)       42 2021-11-10 09:12:06.000000 django-filter-23.2/requirements/test.txt
+-rwxr-xr-x   0 carlton    (501) staff       (20)      390 2022-06-17 14:33:27.000000 django-filter-23.2/runshell.py
+-rwxr-xr-x   0 carlton    (501) staff       (20)      323 2022-06-17 14:33:27.000000 django-filter-23.2/runtests.py
+-rw-r--r--   0 carlton    (501) staff       (20)      244 2023-04-30 09:11:57.380054 django-filter-23.2/setup.cfg
+-rw-r--r--   0 carlton    (501) staff       (20)     2636 2023-04-30 09:10:39.000000 django-filter-23.2/setup.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.377339 django-filter-23.2/tests/
+-rw-r--r--   0 carlton    (501) staff       (20)        0 2021-11-10 09:12:06.000000 django-filter-23.2/tests/__init__.py
+-rw-r--r--   0 carlton    (501) staff       (20)     5347 2022-06-17 14:23:37.000000 django-filter-23.2/tests/models.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.378927 django-filter-23.2/tests/rest_framework/
+-rw-r--r--   0 carlton    (501) staff       (20)       73 2022-06-17 14:23:37.000000 django-filter-23.2/tests/rest_framework/__init__.py
+-rw-r--r--   0 carlton    (501) staff       (20)      184 2022-06-17 14:23:37.000000 django-filter-23.2/tests/rest_framework/apps.py
+-rw-r--r--   0 carlton    (501) staff       (20)      809 2022-06-17 14:23:37.000000 django-filter-23.2/tests/rest_framework/models.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.379207 django-filter-23.2/tests/rest_framework/templates/
+-rw-r--r--   0 carlton    (501) staff       (20)        5 2021-11-10 09:12:06.000000 django-filter-23.2/tests/rest_framework/templates/filter_template.html
+-rw-r--r--   0 carlton    (501) staff       (20)    14969 2023-04-30 09:10:30.000000 django-filter-23.2/tests/rest_framework/test_backends.py
+-rw-r--r--   0 carlton    (501) staff       (20)     1080 2022-06-17 14:23:37.000000 django-filter-23.2/tests/rest_framework/test_filters.py
+-rw-r--r--   0 carlton    (501) staff       (20)     1867 2023-02-10 10:37:27.000000 django-filter-23.2/tests/rest_framework/test_filterset.py
+-rw-r--r--   0 carlton    (501) staff       (20)    15593 2022-06-17 14:33:37.000000 django-filter-23.2/tests/rest_framework/test_integration.py
+-rw-r--r--   0 carlton    (501) staff       (20)      889 2022-06-17 14:23:37.000000 django-filter-23.2/tests/settings.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.356083 django-filter-23.2/tests/templates/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2023-04-30 09:11:57.379403 django-filter-23.2/tests/templates/tests/
+-rw-r--r--   0 carlton    (501) staff       (20)       75 2021-11-10 09:12:06.000000 django-filter-23.2/tests/templates/tests/book_filter.html
+-rw-r--r--   0 carlton    (501) staff       (20)     3429 2022-06-17 14:23:37.000000 django-filter-23.2/tests/test_conf.py
+-rw-r--r--   0 carlton    (501) staff       (20)    10525 2023-03-26 09:29:15.000000 django-filter-23.2/tests/test_fields.py
+-rw-r--r--   0 carlton    (501) staff       (20)    72654 2023-04-30 09:10:30.000000 django-filter-23.2/tests/test_filtering.py
+-rw-r--r--   0 carlton    (501) staff       (20)    56378 2023-03-26 09:14:56.000000 django-filter-23.2/tests/test_filters.py
+-rw-r--r--   0 carlton    (501) staff       (20)    32240 2023-03-26 09:14:56.000000 django-filter-23.2/tests/test_filterset.py
+-rw-r--r--   0 carlton    (501) staff       (20)     8459 2022-06-17 14:23:37.000000 django-filter-23.2/tests/test_forms.py
+-rw-r--r--   0 carlton    (501) staff       (20)    20489 2023-03-26 09:29:15.000000 django-filter-23.2/tests/test_utils.py
+-rw-r--r--   0 carlton    (501) staff       (20)     5484 2022-06-17 14:23:37.000000 django-filter-23.2/tests/test_views.py
+-rw-r--r--   0 carlton    (501) staff       (20)    17436 2022-06-17 14:33:37.000000 django-filter-23.2/tests/test_widgets.py
+-rw-r--r--   0 carlton    (501) staff       (20)      354 2022-06-17 14:23:37.000000 django-filter-23.2/tests/urls.py
+-rw-r--r--   0 carlton    (501) staff       (20)      381 2022-06-17 14:23:37.000000 django-filter-23.2/tests/utils.py
```

### Comparing `django-filter-23.1/CHANGES.rst` & `django-filter-23.2/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Version 23.2 (2023-4-30)
+------------------------
+
+* Deprecated the schema generation methods of the DRF related ``DjangoFilterBackend``.
+  These will be removed in version 25.1.
+
+  You should use `drf-spectacular <https://drf-spectacular.readthedocs.io/en/latest/>`_
+  for generating OpenAPI schemas with DRF.
+
+* In addition, stopped testing against the (very old now) ``coreapi`` schema generation.
+  These methods should continue to work if you're using them until v25.1, but
+  ``coreapi`` is no longer maintained, and is raising warnings against the current
+  versions of Python. To workaround this is not worth the effort at this point.
+
+* Updated Polish translations.
+
 Version 23.1 (2023-3-26)
 ------------------------
 
 * Declared support for Django 4.2.
 
 * Various updated and new translations. Thanks to all who contributed, and
   Weblate for hosting.
```

### Comparing `django-filter-23.1/LICENSE` & `django-filter-23.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/PKG-INFO` & `django-filter-23.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filter
-Version: 23.1
+Version: 23.2
 Summary: Django-filter is a reusable Django application for allowing users to filter querysets dynamically.
 Home-page: https://github.com/carltongibson/django-filter/tree/main
 Author: Alex Gaynor
 Author-email: alex.gaynor@gmail.com
 Maintainer: Carlton Gibson
 Maintainer-email: carlton.gibson@noumenal.es
 License: BSD
```

### Comparing `django-filter-23.1/README.rst` & `django-filter-23.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filter.egg-info/PKG-INFO` & `django-filter-23.2/django_filter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filter
-Version: 23.1
+Version: 23.2
 Summary: Django-filter is a reusable Django application for allowing users to filter querysets dynamically.
 Home-page: https://github.com/carltongibson/django-filter/tree/main
 Author: Alex Gaynor
 Author-email: alex.gaynor@gmail.com
 Maintainer: Carlton Gibson
 Maintainer-email: carlton.gibson@noumenal.es
 License: BSD
```

### Comparing `django-filter-23.1/django_filter.egg-info/SOURCES.txt` & `django-filter-23.2/django_filter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/conf.py` & `django-filter-23.2/django_filters/conf.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/fields.py` & `django-filter-23.2/django_filters/fields.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/filters.py` & `django-filter-23.2/django_filters/filters.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/filterset.py` & `django-filter-23.2/django_filters/filterset.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/ar/LC_MESSAGES/django.mo` & `django-filter-23.2/django_filters/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/ar/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/be/LC_MESSAGES/django.mo` & `django-filter-23.2/django_filters/locale/be/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/be/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/be/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/bg/LC_MESSAGES/django.mo` & `django-filter-23.2/django_filters/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/bg/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/cs/LC_MESSAGES/django.mo` & `django-filter-23.2/django_filters/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/cs/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/da/LC_MESSAGES/django.mo` & `django-filter-23.2/django_filters/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/da/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/de/LC_MESSAGES/django.mo` & `django-filter-23.2/django_filters/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/de/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/el/LC_MESSAGES/django.mo` & `django-filter-23.2/django_filters/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/el/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/es/LC_MESSAGES/django.mo` & `django-filter-23.2/django_filters/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/es/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/es_AR/LC_MESSAGES/django.mo` & `django-filter-23.2/django_filters/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/es_AR/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/es_AR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/fa/LC_MESSAGES/django.mo` & `django-filter-23.2/django_filters/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/fa/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/fi/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/fr/LC_MESSAGES/django.mo` & `django-filter-23.2/django_filters/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/fr/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/it/LC_MESSAGES/django.mo` & `django-filter-23.2/django_filters/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/it/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/nl/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/pl/LC_MESSAGES/django.mo` & `django-filter-23.2/django_filters/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/pl/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/pl/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: django_filters 0.0.1\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-02-10 11:07+0000\n"
-"PO-Revision-Date: 2023-02-12 14:36+0000\n"
+"PO-Revision-Date: 2023-04-10 20:47+0000\n"
 "Last-Translator: Quadric <quadmachine@wp.pl>\n"
 "Language-Team: Polish <https://hosted.weblate.org/projects/django-filter/"
 "django-filter/pl/>\n"
 "Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && ("
 "n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
 "n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 #: conf.py:16
 msgid "date"
 msgstr "data"
 
 #: conf.py:17
 msgid "year"
@@ -87,15 +87,15 @@
 
 #: conf.py:38
 msgid "is in range"
 msgstr "zawiera się w zakresie"
 
 #: conf.py:39
 msgid "is null"
-msgstr ""
+msgstr "jest wartością null"
 
 #: conf.py:40 conf.py:41
 msgid "matches regex"
 msgstr "pasuje do wyrażenia regularnego"
 
 #: conf.py:42 conf.py:49
 msgid "search"
@@ -103,35 +103,35 @@
 
 #: conf.py:44
 msgid "is contained by"
 msgstr "zawiera się w"
 
 #: conf.py:45
 msgid "overlaps"
-msgstr ""
+msgstr "nakłada się"
 
 #: conf.py:46
 msgid "has key"
-msgstr ""
+msgstr "posiada klucz"
 
 #: conf.py:47
 msgid "has keys"
-msgstr ""
+msgstr "posiada klucze"
 
 #: conf.py:48
 msgid "has any keys"
-msgstr ""
+msgstr "posiada jakiekolwiek klucze"
 
 #: fields.py:94
 msgid "Select a lookup."
-msgstr ""
+msgstr "Wybierz wyszukiwanie."
 
 #: fields.py:198
 msgid "Range query expects two values."
-msgstr ""
+msgstr "Zapytanie o zakres oczekuje dwóch wartości."
 
 #: filters.py:437
 msgid "Today"
 msgstr "Dziś"
 
 #: filters.py:438
 msgid "Yesterday"
@@ -170,23 +170,23 @@
 #: templates/django_filters/rest_framework/crispy_form.html:4
 #: templates/django_filters/rest_framework/form.html:2
 msgid "Field filters"
 msgstr "Filtry pola"
 
 #: utils.py:308
 msgid "exclude"
-msgstr ""
+msgstr "wyklucz"
 
 #: widgets.py:58
 msgid "All"
 msgstr "Wszystko"
 
 #: widgets.py:162
 msgid "Unknown"
-msgstr ""
+msgstr "Nieznane"
 
 #: widgets.py:162
 msgid "Yes"
 msgstr "Tak"
 
 #: widgets.py:162
 msgid "No"
```

### Comparing `django-filter-23.1/django_filters/locale/pt_BR/LC_MESSAGES/django.mo` & `django-filter-23.2/django_filters/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/pt_BR/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/ro/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/ru/LC_MESSAGES/django.mo` & `django-filter-23.2/django_filters/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/ru/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/sk/LC_MESSAGES/django.mo` & `django-filter-23.2/django_filters/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/sk/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/uk/LC_MESSAGES/django.mo` & `django-filter-23.2/django_filters/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/uk/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/zh_CN/LC_MESSAGES/django.mo` & `django-filter-23.2/django_filters/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/locale/zh_CN/LC_MESSAGES/django.po` & `django-filter-23.2/django_filters/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/rest_framework/backends.py` & `django-filter-23.2/django_filters/rest_framework/backends.py`

 * *Files 16% similar despite different names*

```diff
@@ -89,14 +89,19 @@
             field_cls = compat.coreschema.String
         return field_cls(description=str(field.extra.get("help_text", "")))
 
     def get_schema_fields(self, view):
         # This is not compatible with widgets where the query param differs from the
         # filter's attribute name. Notably, this includes `MultiWidget`, where query
         # params will be of the format `<name>_0`, `<name>_1`, etc...
+        from django_filters import RemovedInDjangoFilter25Warning
+        warnings.warn(
+            "Built-in schema generation is deprecated. Use drf-spectacular.",
+            category=RemovedInDjangoFilter25Warning,
+        )
         assert (
             compat.coreapi is not None
         ), "coreapi must be installed to use `get_schema_fields()`"
         assert (
             compat.coreschema is not None
         ), "coreschema must be installed to use `get_schema_fields()`"
 
@@ -121,14 +126,19 @@
                     schema=self.get_coreschema_field(field),
                 )
                 for field_name, field in filterset_class.base_filters.items()
             ]
         )
 
     def get_schema_operation_parameters(self, view):
+        from django_filters import RemovedInDjangoFilter25Warning
+        warnings.warn(
+            "Built-in schema generation is deprecated. Use drf-spectacular.",
+            category=RemovedInDjangoFilter25Warning,
+        )
         try:
             queryset = view.get_queryset()
         except Exception:
             queryset = None
             warnings.warn(
                 "{} is not compatible with schema generation".format(view.__class__)
             )
```

### Comparing `django-filter-23.1/django_filters/rest_framework/filterset.py` & `django-filter-23.2/django_filters/rest_framework/filterset.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/utils.py` & `django-filter-23.2/django_filters/utils.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/views.py` & `django-filter-23.2/django_filters/views.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/django_filters/widgets.py` & `django-filter-23.2/django_filters/widgets.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/docs/Makefile` & `django-filter-23.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/docs/assets/form.png` & `django-filter-23.2/docs/assets/form.png`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/docs/conf.py` & `django-filter-23.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/docs/dev/tests.txt` & `django-filter-23.2/docs/dev/tests.txt`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/docs/guide/install.txt` & `django-filter-23.2/docs/guide/install.txt`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/docs/guide/migration.txt` & `django-filter-23.2/docs/guide/migration.txt`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/docs/guide/rest_framework.txt` & `django-filter-23.2/docs/guide/rest_framework.txt`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/docs/guide/tips.txt` & `django-filter-23.2/docs/guide/tips.txt`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/docs/guide/usage.txt` & `django-filter-23.2/docs/guide/usage.txt`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/docs/index.txt` & `django-filter-23.2/docs/index.txt`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/docs/make.bat` & `django-filter-23.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/docs/ref/fields.txt` & `django-filter-23.2/docs/ref/fields.txt`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/docs/ref/filters.txt` & `django-filter-23.2/docs/ref/filters.txt`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/docs/ref/filterset.txt` & `django-filter-23.2/docs/ref/filterset.txt`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/docs/ref/settings.txt` & `django-filter-23.2/docs/ref/settings.txt`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/docs/ref/widgets.txt` & `django-filter-23.2/docs/ref/widgets.txt`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/setup.py` & `django-filter-23.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 
 from setuptools import find_packages, setup
 
 # FIXME: Main module requires django to be present, so cannot run setup.py in
 # clean environment.
 # from django_filters import __version__
-__version__ = "23.1"
+__version__ = "23.2"
 
 f = open("README.rst")
 readme = f.read()
 f.close()
 
 if sys.argv[-1] == "publish":
     if os.system("pip freeze | grep wheel"):
```

### Comparing `django-filter-23.1/tests/models.py` & `django-filter-23.2/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/tests/rest_framework/models.py` & `django-filter-23.2/tests/rest_framework/models.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/tests/rest_framework/test_backends.py` & `django-filter-23.2/tests/rest_framework/test_backends.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import warnings
 from unittest import mock, skipIf
 
 from django.db.models import BooleanField
 from django.test import TestCase
-from django.test.utils import override_settings
+from django.test.utils import ignore_warnings, override_settings
 from rest_framework import generics, serializers
 from rest_framework.test import APIRequestFactory
 
-from django_filters import compat, filters
+from django_filters import RemovedInDjangoFilter25Warning, compat, filters
 from django_filters.rest_framework import DjangoFilterBackend, FilterSet, backends
 
 from ..models import Article
 from .models import CategoryItem, FilterableItem
 
 factory = APIRequestFactory()
 
@@ -241,21 +241,23 @@
         fields = backend.get_schema_fields(view)
         fields = [f.name for f in fields]
 
         self.assertEqual(fields, ["text", "decimal", "date", "f"])
 
 
 class GetSchemaOperationParametersTests(TestCase):
+    @ignore_warnings(category=RemovedInDjangoFilter25Warning)
     def test_get_operation_parameters_with_filterset_fields_list(self):
         backend = DjangoFilterBackend()
         fields = backend.get_schema_operation_parameters(FilterFieldsRootView())
         fields = [f["name"] for f in fields]
 
         self.assertEqual(fields, ["decimal", "date"])
 
+    @ignore_warnings(category=RemovedInDjangoFilter25Warning)
     def test_get_operation_parameters_with_filterset_fields_list_with_choices(self):
         backend = DjangoFilterBackend()
         fields = backend.get_schema_operation_parameters(CategoryItemView())
 
         self.assertEqual(
             fields,
             [
@@ -265,14 +267,20 @@
                     "in": "query",
                     "description": "category",
                     "schema": {"type": "string", "enum": ["home", "office"]},
                 }
             ],
         )
 
+    def test_deprecation_warning(self):
+        backend = DjangoFilterBackend()
+        msg = "Built-in schema generation is deprecated. Use drf-spectacular."
+        with self.assertWarnsMessage(RemovedInDjangoFilter25Warning, msg):
+            backend.get_schema_operation_parameters(FilterFieldsRootView())
+
 
 class TemplateTests(TestCase):
     def test_backend_output(self):
         """
         Ensure backend renders default if template path does not exist
         """
         view = FilterFieldsRootView()
@@ -403,14 +411,15 @@
         qs = self.backend.filter_queryset(mock.Mock(), prev_qs, mock.Mock())
         self.assertIs(qs, prev_qs)
 
     def test_to_html_none_filter_class(self):
         html = self.backend.to_html(mock.Mock(), mock.Mock(), mock.Mock())
         self.assertIsNone(html)
 
+    @ignore_warnings(category=RemovedInDjangoFilter25Warning)
     def test_get_schema_operation_parameters_userwarning(self):
         with self.assertWarns(UserWarning):
             view = mock.Mock()
             view.__class__.return_value = "Test"
             view.get_queryset.side_effect = Exception
             self.backend.get_schema_operation_parameters(view)
```

### Comparing `django-filter-23.1/tests/rest_framework/test_filters.py` & `django-filter-23.2/tests/rest_framework/test_filters.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/tests/rest_framework/test_filterset.py` & `django-filter-23.2/tests/rest_framework/test_filterset.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/tests/rest_framework/test_integration.py` & `django-filter-23.2/tests/rest_framework/test_integration.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/tests/settings.py` & `django-filter-23.2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/tests/test_conf.py` & `django-filter-23.2/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/tests/test_fields.py` & `django-filter-23.2/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/tests/test_filtering.py` & `django-filter-23.2/tests/test_filtering.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 import unittest
 from operator import attrgetter
 from unittest import mock
 
 import django
 from django import forms
 from django.http import QueryDict
-from django.test import TestCase, override_settings
+from django.test import override_settings
 from django.utils import timezone
 from django.utils.timezone import make_aware, now
 
+from django_filters.compat import TestCase
 from django_filters.filters import (
     AllValuesFilter,
     AllValuesMultipleFilter,
     BaseInFilter,
     CharFilter,
     ChoiceFilter,
     DateFromToRangeFilter,
@@ -61,19 +62,19 @@
         class F(FilterSet):
             class Meta:
                 model = Book
                 fields = ["title"]
 
         qs = Book.objects.all()
         f = F(queryset=qs)
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, [b1.pk, b2.pk, b3.pk], lambda o: o.pk, ordered=False
         )
         f = F({"title": "Snowcrash"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [b3.pk], lambda o: o.pk)
+        self.assertQuerySetEqual(f.qs, [b3.pk], lambda o: o.pk)
 
 
 class IntegerFilterTest(TestCase):
     def test_filtering(self):
         default_values = {
             "in_good_standing": True,
             "friendly": False,
@@ -85,21 +86,21 @@
         class F(FilterSet):
             class Meta:
                 model = BankAccount
                 fields = ["amount_saved"]
 
         qs = BankAccount.objects.all()
         f = F(queryset=qs)
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, [b1.pk, b2.pk, b3.pk], lambda o: o.pk, ordered=False
         )
         f = F({"amount_saved": "10"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [b3.pk], lambda o: o.pk)
+        self.assertQuerySetEqual(f.qs, [b3.pk], lambda o: o.pk)
         f = F({"amount_saved": "0"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [b1.pk], lambda o: o.pk)
+        self.assertQuerySetEqual(f.qs, [b1.pk], lambda o: o.pk)
 
 
 class BooleanFilterTests(TestCase):
     def test_filtering(self):
         User.objects.create(username="alex", is_active=False)
         User.objects.create(username="jacob", is_active=True)
         User.objects.create(username="aaron", is_active=False)
@@ -109,21 +110,21 @@
                 model = User
                 fields = ["is_active"]
 
         qs = User.objects.all()
 
         # '2' and '3' are how the field expects the data from the browser
         f = F({"is_active": "2"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["jacob"], lambda o: o.username, False)
+        self.assertQuerySetEqual(f.qs, ["jacob"], lambda o: o.username, False)
 
         f = F({"is_active": "3"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["alex", "aaron"], lambda o: o.username, False)
+        self.assertQuerySetEqual(f.qs, ["alex", "aaron"], lambda o: o.username, False)
 
         f = F({"is_active": "1"}, queryset=qs)
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, ["alex", "aaron", "jacob"], lambda o: o.username, False
         )
 
 
 class ChoiceFilterTests(TestCase):
     @classmethod
     def setUpTestData(cls):
@@ -141,25 +142,25 @@
     def test_filtering(self):
         class F(FilterSet):
             class Meta:
                 model = User
                 fields = ["status"]
 
         f = F()
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, ["aaron", "alex", "jacob", "carl"], lambda o: o.username, False
         )
         f = F({"status": "1"})
-        self.assertQuerysetEqual(f.qs, ["alex"], lambda o: o.username, False)
+        self.assertQuerySetEqual(f.qs, ["alex"], lambda o: o.username, False)
 
         f = F({"status": "2"})
-        self.assertQuerysetEqual(f.qs, ["jacob", "aaron"], lambda o: o.username, False)
+        self.assertQuerySetEqual(f.qs, ["jacob", "aaron"], lambda o: o.username, False)
 
         f = F({"status": "0"})
-        self.assertQuerysetEqual(f.qs, ["carl"], lambda o: o.username, False)
+        self.assertQuerySetEqual(f.qs, ["carl"], lambda o: o.username, False)
 
     def test_filtering_on_explicitly_defined_field(self):
         """
         Test for #30.
 
         If you explicitly declare ChoiceFilter fields you **MUST** pass `choices`.
         """
@@ -168,34 +169,34 @@
             status = ChoiceFilter(choices=STATUS_CHOICES)
 
             class Meta:
                 model = User
                 fields = ["status"]
 
         f = F()
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, ["aaron", "alex", "jacob", "carl"], lambda o: o.username, False
         )
         f = F({"status": "1"})
-        self.assertQuerysetEqual(f.qs, ["alex"], lambda o: o.username, False)
+        self.assertQuerySetEqual(f.qs, ["alex"], lambda o: o.username, False)
 
         f = F({"status": "2"})
-        self.assertQuerysetEqual(f.qs, ["jacob", "aaron"], lambda o: o.username, False)
+        self.assertQuerySetEqual(f.qs, ["jacob", "aaron"], lambda o: o.username, False)
 
         f = F({"status": "0"})
-        self.assertQuerysetEqual(f.qs, ["carl"], lambda o: o.username, False)
+        self.assertQuerySetEqual(f.qs, ["carl"], lambda o: o.username, False)
 
     def test_filtering_on_empty_choice(self):
         class F(FilterSet):
             class Meta:
                 model = User
                 fields = ["status"]
 
         f = F({"status": ""})
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, ["aaron", "alex", "jacob", "carl"], lambda o: o.username, False
         )
 
     def test_filtering_on_null_choice(self):
         choices = [(u.pk, str(u)) for u in User.objects.order_by("id")]
 
         class F(FilterSet):
@@ -207,18 +208,18 @@
 
             class Meta:
                 model = Article
                 fields = ["author"]
 
         # sanity check to make sure the filter is setup correctly
         f = F({"author": "1"})
-        self.assertQuerysetEqual(f.qs, ["alex"], lambda o: str(o.author), False)
+        self.assertQuerySetEqual(f.qs, ["alex"], lambda o: str(o.author), False)
 
         f = F({"author": "null"})
-        self.assertQuerysetEqual(f.qs, [None], lambda o: o.author, False)
+        self.assertQuerySetEqual(f.qs, [None], lambda o: o.author, False)
 
 
 class MultipleChoiceFilterTests(TestCase):
     def test_filtering(self):
         User.objects.create(username="alex", status=1)
         User.objects.create(username="jacob", status=2)
         User.objects.create(username="aaron", status=2)
@@ -229,26 +230,26 @@
 
             class Meta:
                 model = User
                 fields = ["status"]
 
         qs = User.objects.all().order_by("username")
         f = F(queryset=qs)
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, ["aaron", "jacob", "alex", "carl"], lambda o: o.username, False
         )
 
         f = F({"status": ["0"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["carl"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["carl"], lambda o: o.username)
 
         f = F({"status": ["0", "1"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["alex", "carl"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["alex", "carl"], lambda o: o.username)
 
         f = F({"status": ["0", "1", "2"]}, queryset=qs)
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, ["aaron", "alex", "carl", "jacob"], lambda o: o.username
         )
 
     def test_filtering_on_null_choice(self):
         User.objects.create(username="alex", status=1)
         User.objects.create(username="jacob", status=2)
         User.objects.create(username="aaron", status=2)
@@ -271,21 +272,21 @@
 
             class Meta:
                 model = Article
                 fields = ["author"]
 
         # sanity check to make sure the filter is setup correctly
         f = F({"author": ["1"]})
-        self.assertQuerysetEqual(f.qs, ["alex"], lambda o: str(o.author), False)
+        self.assertQuerySetEqual(f.qs, ["alex"], lambda o: str(o.author), False)
 
         f = F({"author": ["null"]})
-        self.assertQuerysetEqual(f.qs, [None], lambda o: o.author, False)
+        self.assertQuerySetEqual(f.qs, [None], lambda o: o.author, False)
 
         f = F({"author": ["1", "null"]})
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, ["alex", None], lambda o: o.author and str(o.author), False
         )
 
 
 class TypedMultipleChoiceFilterTests(TestCase):
     def test_filtering(self):
         User.objects.create(username="alex", status=1)
@@ -300,26 +301,26 @@
 
             class Meta:
                 model = User
                 fields = ["status"]
 
         qs = User.objects.all().order_by("username")
         f = F(queryset=qs)
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, ["aa", "ja", "al", "ca"], lambda o: o.username[0:2], False
         )
 
         f = F({"status": ["0"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["ca"], lambda o: o.username[0:2])
+        self.assertQuerySetEqual(f.qs, ["ca"], lambda o: o.username[0:2])
 
         f = F({"status": ["0", "1"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["al", "ca"], lambda o: o.username[0:2])
+        self.assertQuerySetEqual(f.qs, ["al", "ca"], lambda o: o.username[0:2])
 
         f = F({"status": ["0", "1", "2"]}, queryset=qs)
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, ["aa", "al", "ca", "ja"], lambda o: o.username[0:2]
         )
 
 
 class DateFilterTests(TestCase):
     def test_filtering(self):
         today = now().date()
@@ -335,15 +336,15 @@
         class F(FilterSet):
             class Meta:
                 model = Comment
                 fields = ["date"]
 
         f = F({"date": check_date}, queryset=Comment.objects.all())
         self.assertEqual(len(f.qs), 2)
-        self.assertQuerysetEqual(f.qs, [2, 4], lambda o: o.pk, False)
+        self.assertQuerySetEqual(f.qs, [2, 4], lambda o: o.pk, False)
 
 
 class TimeFilterTests(TestCase):
     def test_filtering(self):
         today = now().date()
         now_time = now().time().replace(microsecond=0)
         ten_min_ago = now() - datetime.timedelta(minutes=10)
@@ -358,15 +359,15 @@
         class F(FilterSet):
             class Meta:
                 model = Comment
                 fields = ["time"]
 
         f = F({"time": check_time}, queryset=Comment.objects.all())
         self.assertEqual(len(f.qs), 2)
-        self.assertQuerysetEqual(f.qs, [2, 4], lambda o: o.pk, False)
+        self.assertQuerySetEqual(f.qs, [2, 4], lambda o: o.pk, False)
 
 
 class DateTimeFilterTests(TestCase):
     def test_filtering(self):
         now_dt = now()
         ten_min_ago = now_dt - datetime.timedelta(minutes=10)
         one_day_ago = now_dt - datetime.timedelta(days=1)
@@ -384,22 +385,22 @@
             class Meta:
                 model = Article
                 fields = ["published"]
 
         qs = Article.objects.all()
         f = F({"published": ten_min_ago}, queryset=qs)
         self.assertEqual(len(f.qs), 1)
-        self.assertQuerysetEqual(f.qs, [2], lambda o: o.pk)
+        self.assertQuerySetEqual(f.qs, [2], lambda o: o.pk)
 
         # this is how it would come through a browser
         f = F({"published": check_dt}, queryset=qs)
         self.assertEqual(
             len(f.qs), 1, "%s isn't matching %s when cleaned" % (check_dt, ten_min_ago)
         )
-        self.assertQuerysetEqual(f.qs, [2], lambda o: o.pk)
+        self.assertQuerySetEqual(f.qs, [2], lambda o: o.pk)
 
 
 class DurationFilterTests(TestCase):
     """Duration filter tests.
 
     The preferred format for durations in Django is '%d %H:%M:%S.%f'.
     See django.utils.dateparse.parse_duration
@@ -438,63 +439,63 @@
                 model = SpacewalkRecord
                 fields = ["duration"]
 
         qs = SpacewalkRecord.objects.all()
 
         # Django style: 3 days, 10 hours, 22 minutes.
         f = F({"duration": "3 10:22:00"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [self.r1], lambda x: x)
+        self.assertQuerySetEqual(f.qs, [self.r1], lambda x: x)
 
         # ISO 8601: 3 days, 10 hours, 22 minutes.
         f = F({"duration": "P3DT10H22M"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [self.r1], lambda x: x)
+        self.assertQuerySetEqual(f.qs, [self.r1], lambda x: x)
 
         # Django style: 82 hours, 22 minutes.
         f = F({"duration": "82:22:00"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [self.r1], lambda x: x)
+        self.assertQuerySetEqual(f.qs, [self.r1], lambda x: x)
 
         # ISO 8601: 82 hours, 22 minutes.
         f = F({"duration": "PT82H22M"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [self.r1], lambda x: x)
+        self.assertQuerySetEqual(f.qs, [self.r1], lambda x: x)
 
     def test_filtering_with_single_lookup_expr_dictionary(self):
         class F(FilterSet):
             class Meta:
                 model = SpacewalkRecord
                 fields = {"duration": ["gt", "gte", "lt", "lte"]}
 
         qs = SpacewalkRecord.objects.order_by("-duration")
 
         f = F({"duration__gt": "PT58H30M"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [self.r1, self.r2, self.r3], lambda x: x)
+        self.assertQuerySetEqual(f.qs, [self.r1, self.r2, self.r3], lambda x: x)
 
         f = F({"duration__gte": "PT58H30M"}, queryset=qs)
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, [self.r1, self.r2, self.r3, self.r4], lambda x: x
         )
 
         f = F({"duration__lt": "PT58H30M"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [self.r5], lambda x: x)
+        self.assertQuerySetEqual(f.qs, [self.r5], lambda x: x)
 
         f = F({"duration__lte": "PT58H30M"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [self.r4, self.r5], lambda x: x)
+        self.assertQuerySetEqual(f.qs, [self.r4, self.r5], lambda x: x)
 
     def test_filtering_with_multiple_lookup_exprs(self):
         class F(FilterSet):
             min_duration = DurationFilter(field_name="duration", lookup_expr="gte")
             max_duration = DurationFilter(field_name="duration", lookup_expr="lte")
 
             class Meta:
                 model = SpacewalkRecord
                 fields = "__all__"
 
         qs = SpacewalkRecord.objects.order_by("duration")
 
         f = F({"min_duration": "PT55H", "max_duration": "PT60H"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [self.r4, self.r3], lambda x: x)
+        self.assertQuerySetEqual(f.qs, [self.r4, self.r3], lambda x: x)
 
 
 class ModelChoiceFilterTests(TestCase):
     def test_filtering(self):
         alex = User.objects.create(username="alex")
         jacob = User.objects.create(username="jacob")
         date = now().date()
@@ -506,30 +507,30 @@
         class F(FilterSet):
             class Meta:
                 model = Comment
                 fields = ["author"]
 
         qs = Comment.objects.all()
         f = F({"author": jacob.pk}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [1, 3], lambda o: o.pk, False)
+        self.assertQuerySetEqual(f.qs, [1, 3], lambda o: o.pk, False)
 
     @override_settings(FILTERS_NULL_CHOICE_LABEL="No Author")
     def test_filtering_null(self):
         Article.objects.create(published=now())
         alex = User.objects.create(username="alex")
         Article.objects.create(author=alex, published=now())
 
         class F(FilterSet):
             class Meta:
                 model = Article
                 fields = ["author", "name"]
 
         qs = Article.objects.all()
         f = F({"author": "null"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [None], lambda o: o.author, False)
+        self.assertQuerySetEqual(f.qs, [None], lambda o: o.author, False)
 
     def test_callable_queryset(self):
         # Sanity check for callable queryset arguments.
         # Ensure that nothing is improperly cached
         User.objects.create(username="alex")
         jacob = User.objects.create(username="jacob")
         aaron = User.objects.create(username="aaron")
@@ -545,19 +546,19 @@
                 fields = ["author"]
 
         qs = Comment.objects.all()
         request = mock.Mock()
 
         request.user = jacob
         f = F(queryset=qs, request=request).filters["author"].field
-        self.assertQuerysetEqual(f.queryset, [1], lambda o: o.pk, False)
+        self.assertQuerySetEqual(f.queryset, [1], lambda o: o.pk, False)
 
         request.user = aaron
         f = F(queryset=qs, request=request).filters["author"].field
-        self.assertQuerysetEqual(f.queryset, [1, 2], lambda o: o.pk, False)
+        self.assertQuerySetEqual(f.queryset, [1, 2], lambda o: o.pk, False)
 
 
 class ModelMultipleChoiceFilterTests(TestCase):
     def setUp(self):
         alex = User.objects.create(username="alex")
         User.objects.create(username="jacob")
         aaron = User.objects.create(username="aaron")
@@ -576,55 +577,55 @@
         class F(FilterSet):
             class Meta:
                 model = User
                 fields = ["favorite_books"]
 
         qs = User.objects.all().order_by("username")
         f = F({"favorite_books": ["1"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["aaron", "alex"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["aaron", "alex"], lambda o: o.username)
 
         f = F({"favorite_books": ["1", "3"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["aaron", "alex"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["aaron", "alex"], lambda o: o.username)
 
         f = F({"favorite_books": ["2"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["alex"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["alex"], lambda o: o.username)
 
         f = F({"favorite_books": ["4"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, [], lambda o: o.username)
 
     @override_settings(FILTERS_NULL_CHOICE_LABEL="No Favorites")
     def test_filtering_null(self):
         class F(FilterSet):
             class Meta:
                 model = User
                 fields = ["favorite_books"]
 
         qs = User.objects.all()
         f = F({"favorite_books": ["null"]}, queryset=qs)
 
-        self.assertQuerysetEqual(f.qs, ["jacob"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["jacob"], lambda o: o.username)
 
     def test_filtering_dictionary(self):
         class F(FilterSet):
             class Meta:
                 model = User
                 fields = {"favorite_books": ["exact"]}
 
         qs = User.objects.all().order_by("username")
         f = F({"favorite_books": ["1"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["aaron", "alex"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["aaron", "alex"], lambda o: o.username)
 
         f = F({"favorite_books": ["1", "3"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["aaron", "alex"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["aaron", "alex"], lambda o: o.username)
 
         f = F({"favorite_books": ["2"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["alex"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["alex"], lambda o: o.username)
 
         f = F({"favorite_books": ["4"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, [], lambda o: o.username)
 
     def test_filtering_on_all_of_subset_of_choices(self):
         class F(FilterSet):
             class Meta:
                 model = User
                 fields = ["favorite_books"]
 
@@ -639,15 +640,15 @@
 
         qs = User.objects.all().order_by("username")
 
         # Select all the given choices.
         f = F({"favorite_books": ["1", "2"]}, queryset=qs)
 
         # The results should only include matching users - not Jacob.
-        self.assertQuerysetEqual(f.qs, ["aaron", "alex"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["aaron", "alex"], lambda o: o.username)
 
     def test_filtering_on_non_required_fields(self):
         # See issue #132 - filtering with all options on a non-required
         # field should exclude any results where the field is null.
         class F(FilterSet):
             author = ModelMultipleChoiceFilter(queryset=User.objects.all())
 
@@ -688,15 +689,15 @@
     def test_filtering(self):
         class F(FilterSet):
             class Meta:
                 model = Book
                 fields = ["price"]
 
         f = F({"price": 10}, queryset=Book.objects.all())
-        self.assertQuerysetEqual(f.qs, ["Ender's Game"], lambda o: o.title)
+        self.assertQuerySetEqual(f.qs, ["Ender's Game"], lambda o: o.title)
 
 
 class RangeFilterTests(TestCase):
     def setUp(self):
         Book.objects.create(
             title="Ender's Game", price="10.0", average_rating=4.7999999999999998
         )
@@ -715,39 +716,39 @@
 
             class Meta:
                 model = Book
                 fields = ["price"]
 
         qs = Book.objects.all().order_by("title")
         f = F(queryset=qs)
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs,
             ["Ender's Game", "Free Book", "Rainbow Six", "Refund", "Snowcrash"],
             lambda o: o.title,
         )
         f = F({"price_min": "5", "price_max": "15"}, queryset=qs)
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, ["Ender's Game", "Rainbow Six"], lambda o: o.title
         )
 
         f = F({"price_min": "11"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["Rainbow Six", "Snowcrash"], lambda o: o.title)
+        self.assertQuerySetEqual(f.qs, ["Rainbow Six", "Snowcrash"], lambda o: o.title)
         f = F({"price_max": "19"}, queryset=qs)
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs,
             ["Ender's Game", "Free Book", "Rainbow Six", "Refund"],
             lambda o: o.title,
         )
 
         f = F({"price_min": "0", "price_max": "12"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["Ender's Game", "Free Book"], lambda o: o.title)
+        self.assertQuerySetEqual(f.qs, ["Ender's Game", "Free Book"], lambda o: o.title)
         f = F({"price_min": "-11", "price_max": "0"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["Free Book", "Refund"], lambda o: o.title)
+        self.assertQuerySetEqual(f.qs, ["Free Book", "Refund"], lambda o: o.title)
         f = F({"price_min": "0", "price_max": "0"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["Free Book"], lambda o: o.title)
+        self.assertQuerySetEqual(f.qs, ["Free Book"], lambda o: o.title)
 
 
 class DateRangeFilterTests(TestCase):
     class CommentFilter(FilterSet):
         date = DateRangeFilter()
 
         class Meta:
@@ -775,35 +776,35 @@
         with mock.patch("django_filters.filters.now") as mock_now:
             mock_now.return_value = today
             yield
 
     def test_filtering_for_year(self):
         f = self.CommentFilter({"date": "year"})
         with self.relative_to(datetime.datetime(now().year, 4, 1)):
-            self.assertQuerysetEqual(f.qs, [1, 3, 4, 5, 6], lambda o: o.pk, False)
+            self.assertQuerySetEqual(f.qs, [1, 3, 4, 5, 6], lambda o: o.pk, False)
 
     def test_filtering_for_month(self):
         f = self.CommentFilter({"date": "month"})
         with self.relative_to(datetime.datetime(now().year, 4, 21)):
-            self.assertQuerysetEqual(f.qs, [1, 3, 4, 5], lambda o: o.pk, False)
+            self.assertQuerySetEqual(f.qs, [1, 3, 4, 5], lambda o: o.pk, False)
 
     def test_filtering_for_week(self):
         f = self.CommentFilter({"date": "week"})
         with self.relative_to(datetime.datetime(now().year, 1, 1)):
-            self.assertQuerysetEqual(f.qs, [3, 4, 5], lambda o: o.pk, False)
+            self.assertQuerySetEqual(f.qs, [3, 4, 5], lambda o: o.pk, False)
 
     def test_filtering_for_yesterday(self):
         f = self.CommentFilter({"date": "yesterday"})
         with self.relative_to(datetime.datetime(now().year, 1, 1)):
-            self.assertQuerysetEqual(f.qs, [5], lambda o: o.pk, False)
+            self.assertQuerySetEqual(f.qs, [5], lambda o: o.pk, False)
 
     def test_filtering_for_today(self):
         f = self.CommentFilter({"date": "today"})
         with self.relative_to(datetime.datetime(now().year, 1, 1)):
-            self.assertQuerysetEqual(f.qs, [4], lambda o: o.pk, False)
+            self.assertQuerySetEqual(f.qs, [4], lambda o: o.pk, False)
 
 
 class DateFromToRangeFilterTests(TestCase):
     def test_filtering(self):
         adam = User.objects.create(username="adam")
         kwargs = {"text": "test", "author": adam, "time": "10:00"}
         Comment.objects.create(date=datetime.date(2016, 1, 1), **kwargs)
@@ -1175,56 +1176,56 @@
                 fields = ("account",)
 
         f = F()
         self.assertEqual(f.qs.count(), 4)
 
         f = F({"account": 1})
         self.assertEqual(f.qs.count(), 1)
-        self.assertQuerysetEqual(f.qs, [1], lambda o: o.pk)
+        self.assertQuerySetEqual(f.qs, [1], lambda o: o.pk)
 
     def test_o2o_relation_dictionary(self):
         class F(FilterSet):
             class Meta:
                 model = Profile
                 fields = {
                     "account": ["exact"],
                 }
 
         f = F()
         self.assertEqual(f.qs.count(), 4)
 
         f = F({"account": 1})
         self.assertEqual(f.qs.count(), 1)
-        self.assertQuerysetEqual(f.qs, [1], lambda o: o.pk)
+        self.assertQuerySetEqual(f.qs, [1], lambda o: o.pk)
 
     def test_reverse_o2o_relation(self):
         class F(FilterSet):
             class Meta:
                 model = Account
                 fields = ("profile",)
 
         f = F()
         self.assertEqual(f.qs.count(), 4)
 
         f = F({"profile": 1})
         self.assertEqual(f.qs.count(), 1)
-        self.assertQuerysetEqual(f.qs, [1], lambda o: o.pk)
+        self.assertQuerySetEqual(f.qs, [1], lambda o: o.pk)
 
     def test_o2o_relation_attribute(self):
         class F(FilterSet):
             class Meta:
                 model = Profile
                 fields = ("account__in_good_standing",)
 
         f = F()
         self.assertEqual(f.qs.count(), 4)
 
         f = F({"account__in_good_standing": "2"})
         self.assertEqual(f.qs.count(), 2)
-        self.assertQuerysetEqual(f.qs, [2, 3], lambda o: o.pk, False)
+        self.assertQuerySetEqual(f.qs, [2, 3], lambda o: o.pk, False)
 
     def test_o2o_relation_attribute2(self):
         class F(FilterSet):
             class Meta:
                 model = Profile
                 fields = (
                     "account__in_good_standing",
@@ -1232,41 +1233,41 @@
                 )
 
         f = F()
         self.assertEqual(f.qs.count(), 4)
 
         f = F({"account__in_good_standing": "2", "account__friendly": "2"})
         self.assertEqual(f.qs.count(), 1)
-        self.assertQuerysetEqual(f.qs, [2], lambda o: o.pk)
+        self.assertQuerySetEqual(f.qs, [2], lambda o: o.pk)
 
     def test_reverse_o2o_relation_attribute(self):
         class F(FilterSet):
             class Meta:
                 model = Account
                 fields = ("profile__likes_coffee",)
 
         f = F()
         self.assertEqual(f.qs.count(), 4)
 
         f = F({"profile__likes_coffee": "2"})
         self.assertEqual(f.qs.count(), 2)
-        self.assertQuerysetEqual(f.qs, [1, 3], lambda o: o.pk, False)
+        self.assertQuerySetEqual(f.qs, [1, 3], lambda o: o.pk, False)
 
     def test_reverse_o2o_relation_attribute2(self):
         class F(FilterSet):
             class Meta:
                 model = Account
                 fields = ("profile__likes_coffee", "profile__likes_tea")
 
         f = F()
         self.assertEqual(f.qs.count(), 4)
 
         f = F({"profile__likes_coffee": "2", "profile__likes_tea": "2"})
         self.assertEqual(f.qs.count(), 1)
-        self.assertQuerysetEqual(f.qs, [3], lambda o: o.pk)
+        self.assertQuerySetEqual(f.qs, [3], lambda o: o.pk)
 
 
 class FKRelationshipTests(TestCase):
     def test_fk_relation(self):
         company1 = Company.objects.create(name="company1")
         company2 = Company.objects.create(name="company2")
         Location.objects.create(company=company1, open_days="some", zip_code="90210")
@@ -1279,15 +1280,15 @@
                 fields = ("company",)
 
         f = F()
         self.assertEqual(f.qs.count(), 3)
 
         f = F({"company": 1})
         self.assertEqual(f.qs.count(), 2)
-        self.assertQuerysetEqual(f.qs, [1, 3], lambda o: o.pk, False)
+        self.assertQuerySetEqual(f.qs, [1, 3], lambda o: o.pk, False)
 
     def test_reverse_fk_relation(self):
         alex = User.objects.create(username="alex")
         jacob = User.objects.create(username="jacob")
         date = now().date()
         time = now().time()
         Comment.objects.create(text="comment 1", author=jacob, time=time, date=date)
@@ -1297,25 +1298,25 @@
         class F(FilterSet):
             class Meta:
                 model = User
                 fields = ["comments"]
 
         qs = User.objects.all()
         f = F({"comments": [2]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["alex"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["alex"], lambda o: o.username)
 
         class F(FilterSet):
             comments = AllValuesFilter()
 
             class Meta:
                 model = User
                 fields = ["comments"]
 
         f = F({"comments": 2}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["alex"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["alex"], lambda o: o.username)
 
     def test_fk_relation_attribute(self):
         now_dt = now()
         alex = User.objects.create(username="alex")
         jacob = User.objects.create(username="jacob")
         User.objects.create(username="aaron")
 
@@ -1353,25 +1354,25 @@
         class F(FilterSet):
             class Meta:
                 model = User
                 fields = ["comments__text"]
 
         qs = User.objects.all()
         f = F({"comments__text": "comment 2"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["alex"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["alex"], lambda o: o.username)
 
         class F(FilterSet):
             comments__text = AllValuesFilter()
 
             class Meta:
                 model = User
                 fields = ["comments__text"]
 
         f = F({"comments__text": "comment 2"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["alex"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["alex"], lambda o: o.username)
 
     @unittest.skip("todo - need correct models")
     def test_fk_relation_multiple_attributes(self):
         pass
 
     @unittest.expectedFailure
     def test_reverse_fk_relation_multiple_attributes(self):
@@ -1406,124 +1407,124 @@
         class F(FilterSet):
             class Meta:
                 model = User
                 fields = ["favorite_books"]
 
         qs = User.objects.all().order_by("username")
         f = F({"favorite_books": ["1"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["aaron", "alex"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["aaron", "alex"], lambda o: o.username)
 
         f = F({"favorite_books": ["1", "3"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["aaron", "alex"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["aaron", "alex"], lambda o: o.username)
 
         f = F({"favorite_books": ["2"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["alex"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["alex"], lambda o: o.username)
 
         f = F({"favorite_books": ["4"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, [], lambda o: o.username)
 
     def test_reverse_m2m_relation(self):
         class F(FilterSet):
             class Meta:
                 model = Book
                 fields = ["lovers"]
 
         qs = Book.objects.all().order_by("title")
         f = F({"lovers": [1]}, queryset=qs)
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, ["Ender's Game", "Rainbow Six"], lambda o: o.title
         )
 
         class F(FilterSet):
             lovers = AllValuesFilter()
 
             class Meta:
                 model = Book
                 fields = ["lovers"]
 
         f = F({"lovers": 1}, queryset=qs)
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, ["Ender's Game", "Rainbow Six"], lambda o: o.title
         )
 
     def test_m2m_relation_attribute(self):
         class F(FilterSet):
             class Meta:
                 model = User
                 fields = ["favorite_books__title"]
 
         qs = User.objects.all().order_by("username")
         f = F({"favorite_books__title": "Ender's Game"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["aaron", "alex"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["aaron", "alex"], lambda o: o.username)
 
         f = F({"favorite_books__title": "Rainbow Six"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["alex"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["alex"], lambda o: o.username)
 
         class F(FilterSet):
             favorite_books__title = MultipleChoiceFilter()
 
             class Meta:
                 model = User
                 fields = ["favorite_books__title"]
 
         f = F()
         self.assertEqual(len(f.filters["favorite_books__title"].field.choices), 0)
         # f = F({'favorite_books__title': ['1', '3']},
         #     queryset=qs)
-        # self.assertQuerysetEqual(
+        # self.assertQuerySetEqual(
         #     f.qs, ['aaron', 'alex'], lambda o: o.username)
 
         class F(FilterSet):
             favorite_books__title = AllValuesFilter()
 
             class Meta:
                 model = User
                 fields = ["favorite_books__title"]
 
         f = F({"favorite_books__title": "Snowcrash"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["aaron"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["aaron"], lambda o: o.username)
 
     def test_reverse_m2m_relation_attribute(self):
         class F(FilterSet):
             class Meta:
                 model = Book
                 fields = ["lovers__username"]
 
         qs = Book.objects.all().order_by("title")
         f = F({"lovers__username": "alex"}, queryset=qs)
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, ["Ender's Game", "Rainbow Six"], lambda o: o.title
         )
 
         f = F({"lovers__username": "jacob"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [], lambda o: o.title)
+        self.assertQuerySetEqual(f.qs, [], lambda o: o.title)
 
         class F(FilterSet):
             lovers__username = MultipleChoiceFilter()
 
             class Meta:
                 model = Book
                 fields = ["lovers__username"]
 
         f = F()
         self.assertEqual(len(f.filters["lovers__username"].field.choices), 0)
         # f = F({'lovers__username': ['1', '3']},
         #     queryset=qs)
-        # self.assertQuerysetEqual(
+        # self.assertQuerySetEqual(
         #     f.qs, ["Ender's Game", "Rainbow Six"], lambda o: o.title)
 
         class F(FilterSet):
             lovers__username = AllValuesFilter()
 
             class Meta:
                 model = Book
                 fields = ["lovers__username"]
 
         f = F({"lovers__username": "alex"}, queryset=qs)
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, ["Ender's Game", "Rainbow Six"], lambda o: o.title
         )
 
     @unittest.expectedFailure
     def test_m2m_relation_multiple_attributes(self):
         class F(FilterSet):
             class Meta:
@@ -1531,37 +1532,37 @@
                 fields = ["favorite_books__price", "favorite_books__average_rating"]
 
         qs = User.objects.all().order_by("username")
         f = F(
             {"favorite_books__price": "1.00", "favorite_books__average_rating": 4.0},
             queryset=qs,
         )
-        self.assertQuerysetEqual(f.qs, ["aaron"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["aaron"], lambda o: o.username)
 
         f = F(
             {"favorite_books__price": "3.00", "favorite_books__average_rating": 4.0},
             queryset=qs,
         )
-        self.assertQuerysetEqual(f.qs, [], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, [], lambda o: o.username)
 
     @unittest.expectedFailure
     def test_reverse_m2m_relation_multiple_attributes(self):
         class F(FilterSet):
             class Meta:
                 model = Book
                 fields = ["lovers__status", "lovers__username"]
 
         qs = Book.objects.all().order_by("title")
         f = F({"lovers__status": 1, "lovers__username": "alex"}, queryset=qs)
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, ["Ender's Game", "Rainbow Six"], lambda o: o.title
         )
 
         f = F({"lovers__status": 1, "lovers__username": "jacob"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [], lambda o: o.title)
+        self.assertQuerySetEqual(f.qs, [], lambda o: o.title)
 
     @unittest.skip("todo")
     def test_fk_relation_on_m2m_relation(self):
         pass
 
     @unittest.skip("todo")
     def test_fk_relation_attribute_on_m2m_relation(self):
@@ -1583,15 +1584,15 @@
         class F(FilterSet):
             class Meta:
                 model = Node
                 fields = ["adjacents"]
 
         qs = Node.objects.all().order_by("pk")
         f = F({"adjacents": ["1"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [2, 4], lambda o: o.pk)
+        self.assertQuerySetEqual(f.qs, [2, 4], lambda o: o.pk)
 
 
 class NonSymmetricalSelfReferentialRelationshipTests(TestCase):
     def setUp(self):
         n1 = DirectedNode.objects.create(name="one")
         n2 = DirectedNode.objects.create(name="two")
         n3 = DirectedNode.objects.create(name="three")
@@ -1605,25 +1606,25 @@
         class F(FilterSet):
             class Meta:
                 model = DirectedNode
                 fields = ["outbound_nodes"]
 
         qs = DirectedNode.objects.all().order_by("pk")
         f = F({"outbound_nodes": ["1"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [4], lambda o: o.pk)
+        self.assertQuerySetEqual(f.qs, [4], lambda o: o.pk)
 
     def test_reverse_relation(self):
         class F(FilterSet):
             class Meta:
                 model = DirectedNode
                 fields = ["inbound_nodes"]
 
         qs = DirectedNode.objects.all().order_by("pk")
         f = F({"inbound_nodes": ["1"]}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [2], lambda o: o.pk)
+        self.assertQuerySetEqual(f.qs, [2], lambda o: o.pk)
 
 
 @override_settings(TIME_ZONE="UTC")
 class TransformedQueryExpressionFilterTests(TestCase):
     def test_filtering(self):
         now_dt = now()
         after_5pm = now_dt.replace(hour=18)
@@ -1637,15 +1638,15 @@
             class Meta:
                 model = Article
                 fields = {"published": ["hour__gte"]}
 
         qs = Article.objects.all()
         f = F({"published__hour__gte": 17}, queryset=qs)
         self.assertEqual(len(f.qs), 1)
-        self.assertQuerysetEqual(f.qs, [a.pk], lambda o: o.pk)
+        self.assertQuerySetEqual(f.qs, [a.pk], lambda o: o.pk)
 
 
 class LookupChoiceFilterTests(TestCase):
     class BookFilter(FilterSet):
         price = LookupChoiceFilter(
             lookup_choices=["lt", "gt"], field_class=forms.DecimalField
         )
@@ -1666,28 +1667,28 @@
             title="Snowcrash", price="20.0", average_rating=4.2999999999999998
         )
 
     def test_filtering(self):
         F = self.BookFilter
 
         f = F({"price": "15", "price_lookup": "lt"})
-        self.assertQuerysetEqual(f.qs, ["Ender's Game"], lambda o: o.title)
+        self.assertQuerySetEqual(f.qs, ["Ender's Game"], lambda o: o.title)
         f = F({"price": "15", "price_lookup": "lt"})
-        self.assertQuerysetEqual(f.qs, ["Ender's Game"], lambda o: o.title)
+        self.assertQuerySetEqual(f.qs, ["Ender's Game"], lambda o: o.title)
         f = F({"price": "", "price_lookup": "lt"})
         self.assertTrue(f.is_valid())
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs,
             ["Ender's Game", "Rainbow Six", "Snowcrash"],
             lambda o: o.title,
             ordered=False,
         )
         f = F({"price": "15"})
         self.assertFalse(f.is_valid())
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs,
             ["Ender's Game", "Rainbow Six", "Snowcrash"],
             lambda o: o.title,
             ordered=False,
         )
 
     def test_inner_field_class_validation(self):
@@ -1775,15 +1776,15 @@
             ({"status__in": "0,2"}, [2, 3, 4]),
             ({"status__in": "0,,1"}, [1, 4]),
             ({"status__in": "2"}, [2, 3]),
         ]
 
         for params, expected in cases:
             with self.subTest(params=params, expected=expected):
-                self.assertQuerysetEqual(
+                self.assertQuerySetEqual(
                     F(params, queryset=qs).qs, expected, attrgetter("pk")
                 )
 
     def test_string_filtering(self):
         F = self.user_filter
         qs = User.objects.order_by("pk")
 
@@ -1796,15 +1797,15 @@
             ({"username__in": "alex,aaron"}, [1, 3]),
             ({"username__in": "alex,,aaron"}, [1, 3]),
             ({"username__in": "alex,"}, [1]),
         ]
 
         for params, expected in cases:
             with self.subTest(params=params, expected=expected):
-                self.assertQuerysetEqual(
+                self.assertQuerySetEqual(
                     F(params, queryset=qs).qs, expected, attrgetter("pk")
                 )
 
     def test_datetime_filtering(self):
         F = self.article_filter
         qs = Article.objects.order_by("pk")
 
@@ -1838,15 +1839,15 @@
                 [1, 2, 3, 4],
             ),
             ({"published__in": "%s," % (after,)}, [1, 2]),
         ]
 
         for params, expected in cases:
             with self.subTest(params=params, expected=expected):
-                self.assertQuerysetEqual(
+                self.assertQuerySetEqual(
                     F(params, queryset=qs).qs, expected, attrgetter("pk")
                 )
 
     def test_related_filtering(self):
         F = self.article_filter
         qs = Article.objects.order_by("pk")
 
@@ -1859,15 +1860,15 @@
             ({"author__in": "1,2"}, [1, 2, 3, 4]),
             ({"author__in": "1,,2"}, [1, 2, 3, 4]),
             ({"author__in": "1,"}, [1, 3]),
         ]
 
         for params, expected in cases:
             with self.subTest(params=params, expected=expected):
-                self.assertQuerysetEqual(
+                self.assertQuerySetEqual(
                     F(params, queryset=qs).qs, expected, attrgetter("pk")
                 )
 
 
 @override_settings(TIME_ZONE="UTC")
 class CSVRangeFilterTests(TestCase):
     class ArticleFilter(FilterSet):
@@ -1997,29 +1998,29 @@
         qs.all.return_value.filter.assert_called_with(username__exact="jdoe")
 
     def test_filtering_without_meta(self):
         class F(FilterSet):
             username = CharFilter()
 
         f = F({"username": "alex"}, queryset=User.objects.all())
-        self.assertQuerysetEqual(f.qs, ["alex"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["alex"], lambda o: o.username)
 
     def test_filtering_with_multiple_filters(self):
         class F(FilterSet):
             class Meta:
                 model = User
                 fields = ["status", "username"]
 
         qs = User.objects.all()
 
         f = F({"username": "alex", "status": "1"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["alex"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["alex"], lambda o: o.username)
 
         f = F({"username": "alex", "status": "2"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [], lambda o: o.pk)
+        self.assertQuerySetEqual(f.qs, [], lambda o: o.pk)
 
     def test_filter_with_initial(self):
         # Initial values are a form presentation option - the FilterSet should
         # not use an initial value as a default value to filter by.
         class F(FilterSet):
             status = ChoiceFilter(choices=STATUS_CHOICES, initial=1)
 
@@ -2027,18 +2028,18 @@
                 model = User
                 fields = ["status"]
 
         qs = User.objects.all()
         users = ["alex", "jacob", "aaron", "carl"]
 
         f = F(queryset=qs)
-        self.assertQuerysetEqual(f.qs.order_by("pk"), users, lambda o: o.username)
+        self.assertQuerySetEqual(f.qs.order_by("pk"), users, lambda o: o.username)
 
         f = F({"status": 0}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["carl"], lambda o: o.username)
+        self.assertQuerySetEqual(f.qs, ["carl"], lambda o: o.username)
 
     def test_qs_count(self):
         class F(FilterSet):
             class Meta:
                 model = User
                 fields = ["status"]
 
@@ -2070,24 +2071,24 @@
             class Meta:
                 model = User
                 fields = ["last_name", "username"]
 
         qs = User.objects.all()
 
         f = F({"last_name": ["johnson"]}, queryset=qs)
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, ["alex", "jacob"], lambda o: o.username, ordered=False
         )
 
         f = F({"last_name": ["johnson"], "username": "carl"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, [], lambda o: o.username, ordered=False)
+        self.assertQuerySetEqual(f.qs, [], lambda o: o.username, ordered=False)
 
         f = F({"last_name": ["johnson"], "username": "jacob"}, queryset=qs)
-        self.assertQuerysetEqual(f.qs, ["jacob"], lambda o: o.username, ordered=False)
+        self.assertQuerySetEqual(f.qs, ["jacob"], lambda o: o.username, ordered=False)
 
         f = F(
             {"last_name": ["johnson", "white"], "username": "jacob, carl, aaron"},
             queryset=qs,
         )
-        self.assertQuerysetEqual(
+        self.assertQuerySetEqual(
             f.qs, ["jacob", "aaron"], lambda o: o.username, ordered=False
         )
```

### Comparing `django-filter-23.1/tests/test_filters.py` & `django-filter-23.2/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/tests/test_filterset.py` & `django-filter-23.2/tests/test_filterset.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/tests/test_forms.py` & `django-filter-23.2/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/tests/test_utils.py` & `django-filter-23.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/tests/test_views.py` & `django-filter-23.2/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-filter-23.1/tests/test_widgets.py` & `django-filter-23.2/tests/test_widgets.py`

 * *Files identical despite different names*

