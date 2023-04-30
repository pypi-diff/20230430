# Comparing `tmp/lino-avanti-23.3.0.tar.gz` & `tmp/lino-avanti-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino-avanti-23.3.0.tar", last modified: Wed Mar  1 21:18:47 2023, max compression
+gzip compressed data, was "lino-avanti-23.4.0.tar", last modified: Sun Apr 30 03:12:01 2023, max compression
```

## Comparing `lino-avanti-23.3.0.tar` & `lino-avanti-23.4.0.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.590892 lino-avanti-23.3.0/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:55:33.000000 lino-avanti-23.3.0/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)       64 2018-08-13 17:13:49.000000 lino-avanti-23.3.0/MANIFEST.in
--rw-rw-r--   0 luc       (1000) www-data    (33)     2107 2023-03-01 21:18:47.590892 lino-avanti-23.3.0/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1178 2021-04-07 13:16:37.000000 lino-avanti-23.3.0/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.586892 lino-avanti-23.3.0/lino_avanti/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      467 2021-04-25 11:15:49.000000 lino-avanti-23.3.0/lino_avanti/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.586892 lino-avanti-23.3.0/lino_avanti/lib/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      269 2021-04-07 10:22:53.000000 lino-avanti-23.3.0/lino_avanti/lib/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.586892 lino-avanti-23.3.0/lino_avanti/lib/avanti/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1369 2021-04-07 10:22:54.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1663 2021-04-07 10:22:54.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/choicelists.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.578890 lino-avanti-23.3.0/lino_avanti/lib/avanti/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.578890 lino-avanti-23.3.0/lino_avanti/lib/avanti/config/avanti/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.586892 lino-avanti-23.3.0/lino_avanti/lib/avanti/config/avanti/Client/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2597 2020-07-07 02:26:11.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/config/avanti/Client/final_report.weasy.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.586892 lino-avanti-23.3.0/lino_avanti/lib/avanti/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-01-21 04:33:31.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7085 2021-04-07 10:22:55.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      950 2021-04-07 10:22:55.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1082 2021-04-07 10:22:55.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4610 2023-02-15 05:14:30.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/help_texts.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     1492 2022-09-30 11:46:08.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/layouts.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.578890 lino-avanti-23.3.0/lino_avanti/lib/avanti/locale/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.578890 lino-avanti-23.3.0/lino_avanti/lib/avanti/locale/de/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.586892 lino-avanti-23.3.0/lino_avanti/lib/avanti/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6679 2020-04-20 16:09:38.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    19981 2021-02-11 19:04:16.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/locale/de/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.578890 lino-avanti-23.3.0/lino_avanti/lib/avanti/locale/fr/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.586892 lino-avanti-23.3.0/lino_avanti/lib/avanti/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    38461 2016-11-20 18:48:07.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    96464 2021-02-11 19:04:17.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/locale/fr/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.582891 lino-avanti-23.3.0/lino_avanti/lib/avanti/locale/nl/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.586892 lino-avanti-23.3.0/lino_avanti/lib/avanti/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      409 2015-09-19 03:53:53.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    93297 2021-02-11 17:36:49.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/locale/nl/LC_MESSAGES/django.po
--rw-rw-rw-   0 luc       (1000) www-data    (33)      683 2021-04-07 10:22:54.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/migrate.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    21966 2022-09-05 23:22:01.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      704 2021-04-07 10:22:54.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/roles.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5894 2022-07-02 16:53:08.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/settings.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3499 2021-11-12 10:16:18.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/user_types.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1780 2021-04-07 10:22:54.000000 lino-avanti-23.3.0/lino_avanti/lib/avanti/workflows.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.586892 lino-avanti-23.3.0/lino_avanti/lib/cal/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      667 2021-04-07 10:22:54.000000 lino-avanti-23.3.0/lino_avanti/lib/cal/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.586892 lino-avanti-23.3.0/lino_avanti/lib/cal/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:36:34.000000 lino-avanti-23.3.0/lino_avanti/lib/cal/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       45 2016-02-22 08:52:24.000000 lino-avanti-23.3.0/lino_avanti/lib/cal/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      370 2018-10-07 07:17:23.000000 lino-avanti-23.3.0/lino_avanti/lib/cal/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1513 2021-04-07 10:22:54.000000 lino-avanti-23.3.0/lino_avanti/lib/cal/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.586892 lino-avanti-23.3.0/lino_avanti/lib/contacts/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      425 2021-04-07 10:22:54.000000 lino-avanti-23.3.0/lino_avanti/lib/contacts/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.586892 lino-avanti-23.3.0/lino_avanti/lib/contacts/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:36:35.000000 lino-avanti-23.3.0/lino_avanti/lib/contacts/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       55 2016-07-06 14:59:00.000000 lino-avanti-23.3.0/lino_avanti/lib/contacts/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       54 2016-07-06 14:59:00.000000 lino-avanti-23.3.0/lino_avanti/lib/contacts/fixtures/std.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.586892 lino-avanti-23.3.0/lino_avanti/lib/contacts/management/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:36:35.000000 lino-avanti-23.3.0/lino_avanti/lib/contacts/management/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.586892 lino-avanti-23.3.0/lino_avanti/lib/contacts/management/commands/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:36:35.000000 lino-avanti-23.3.0/lino_avanti/lib/contacts/management/commands/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       71 2016-07-06 14:58:59.000000 lino-avanti-23.3.0/lino_avanti/lib/contacts/management/commands/garble_persons.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3095 2022-09-05 23:22:02.000000 lino-avanti-23.3.0/lino_avanti/lib/contacts/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.586892 lino-avanti-23.3.0/lino_avanti/lib/courses/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      959 2021-04-07 10:22:54.000000 lino-avanti-23.3.0/lino_avanti/lib/courses/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      719 2021-04-07 10:22:54.000000 lino-avanti-23.3.0/lino_avanti/lib/courses/choicelists.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.582891 lino-avanti-23.3.0/lino_avanti/lib/courses/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.582891 lino-avanti-23.3.0/lino_avanti/lib/courses/config/courses/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.586892 lino-avanti-23.3.0/lino_avanti/lib/courses/config/courses/Enrolment/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    49781 2017-10-04 00:59:51.000000 lino-avanti-23.3.0/lino_avanti/lib/courses/config/courses/Enrolment/Default.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.590892 lino-avanti-23.3.0/lino_avanti/lib/courses/config/courses/Reminder/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    40323 2018-01-15 02:55:31.000000 lino-avanti-23.3.0/lino_avanti/lib/courses/config/courses/Reminder/Default.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-10-04 00:40:35.000000 lino-avanti-23.3.0/lino_avanti/lib/courses/config/courses/Reminder/body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3009 2018-01-17 21:32:39.000000 lino-avanti-23.3.0/lino_avanti/lib/courses/config/courses/Reminder/reminder.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)    11056 2022-11-08 12:29:27.000000 lino-avanti-23.3.0/lino_avanti/lib/courses/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     5900 2022-11-08 12:30:48.000000 lino-avanti-23.3.0/lino_avanti/lib/courses/ui.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      415 2020-11-04 09:18:05.000000 lino-avanti-23.3.0/lino_avanti/lib/courses/workflows.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.590892 lino-avanti-23.3.0/lino_avanti/lib/cv/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      316 2021-04-07 10:22:54.000000 lino-avanti-23.3.0/lino_avanti/lib/cv/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.590892 lino-avanti-23.3.0/lino_avanti/lib/cv/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:36:34.000000 lino-avanti-23.3.0/lino_avanti/lib/cv/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2019-09-21 18:31:41.000000 lino-avanti-23.3.0/lino_avanti/lib/cv/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1437 2021-04-07 10:22:54.000000 lino-avanti-23.3.0/lino_avanti/lib/cv/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.590892 lino-avanti-23.3.0/lino_avanti/lib/households/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      295 2021-04-07 10:22:54.000000 lino-avanti-23.3.0/lino_avanti/lib/households/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.590892 lino-avanti-23.3.0/lino_avanti/lib/households/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:45.000000 lino-avanti-23.3.0/lino_avanti/lib/households/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       51 2016-02-22 08:57:42.000000 lino-avanti-23.3.0/lino_avanti/lib/households/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       50 2016-02-22 08:57:42.000000 lino-avanti-23.3.0/lino_avanti/lib/households/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      871 2021-04-07 10:22:54.000000 lino-avanti-23.3.0/lino_avanti/lib/households/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.590892 lino-avanti-23.3.0/lino_avanti/lib/tickets/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      329 2021-04-07 10:22:54.000000 lino-avanti-23.3.0/lino_avanti/lib/tickets/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1324 2021-04-07 10:22:54.000000 lino-avanti-23.3.0/lino_avanti/lib/tickets/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.590892 lino-avanti-23.3.0/lino_avanti/lib/users/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      385 2022-11-08 14:56:08.000000 lino-avanti-23.3.0/lino_avanti/lib/users/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.590892 lino-avanti-23.3.0/lino_avanti/lib/users/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:53.000000 lino-avanti-23.3.0/lino_avanti/lib/users/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-06-13 23:56:47.000000 lino-avanti-23.3.0/lino_avanti/lib/users/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2017-06-13 23:56:47.000000 lino-avanti-23.3.0/lino_avanti/lib/users/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2017-06-13 23:56:48.000000 lino-avanti-23.3.0/lino_avanti/lib/users/fixtures/demo_users.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      238 2022-11-08 12:29:27.000000 lino-avanti-23.3.0/lino_avanti/lib/users/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1154 2022-11-08 12:30:48.000000 lino-avanti-23.3.0/lino_avanti/lib/users/ui.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3529 2023-03-01 21:17:57.000000 lino-avanti-23.3.0/lino_avanti/setup_info.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.586892 lino-avanti-23.3.0/lino_avanti.egg-info/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2107 2023-03-01 21:18:47.000000 lino-avanti-23.3.0/lino_avanti.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2936 2023-03-01 21:18:47.000000 lino-avanti-23.3.0/lino_avanti.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-03-01 21:18:47.000000 lino-avanti-23.3.0/lino_avanti.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       17 2023-03-01 21:18:47.000000 lino-avanti-23.3.0/lino_avanti.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       12 2023-03-01 21:18:47.000000 lino-avanti-23.3.0/lino_avanti.egg-info/top_level.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      136 2021-05-05 05:16:56.000000 lino-avanti-23.3.0/requirements.stable.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      122 2021-05-05 05:16:56.000000 lino-avanti-23.3.0/requirements.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-03-01 21:18:47.590892 lino-avanti-23.3.0/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      182 2020-07-10 08:02:46.000000 lino-avanti-23.3.0/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      252 2018-04-29 04:12:02.000000 lino-avanti-23.3.0/tasks.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-01 21:18:47.590892 lino-avanti-23.3.0/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      797 2022-10-18 03:28:38.000000 lino-avanti-23.3.0/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      189 2020-04-20 16:10:32.000000 lino-avanti-23.3.0/tests/test_docs.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.984109 lino-avanti-23.4.0/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:55:33.000000 lino-avanti-23.4.0/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       64 2018-08-13 17:13:49.000000 lino-avanti-23.4.0/MANIFEST.in
+-rw-rw-r--   0 luc       (1000) www-data    (33)     2107 2023-04-30 03:12:01.984109 lino-avanti-23.4.0/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1178 2023-03-17 19:56:26.000000 lino-avanti-23.4.0/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.976109 lino-avanti-23.4.0/lino_avanti/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      467 2021-04-25 11:15:49.000000 lino-avanti-23.4.0/lino_avanti/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti/lib/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      269 2021-04-07 10:22:53.000000 lino-avanti-23.4.0/lino_avanti/lib/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti/lib/avanti/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1369 2021-04-07 10:22:54.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1663 2021-04-07 10:22:54.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/choicelists.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.976109 lino-avanti-23.4.0/lino_avanti/lib/avanti/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.976109 lino-avanti-23.4.0/lino_avanti/lib/avanti/config/avanti/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti/lib/avanti/config/avanti/Client/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2597 2020-07-07 02:26:11.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/config/avanti/Client/final_report.weasy.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti/lib/avanti/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-01-21 04:33:31.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     7085 2021-04-07 10:22:55.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/fixtures/demo.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      967 2023-04-05 09:41:20.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1082 2021-04-07 10:22:55.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4610 2023-04-28 19:21:03.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/help_texts.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1492 2022-09-30 11:46:08.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/layouts.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.976109 lino-avanti-23.4.0/lino_avanti/lib/avanti/locale/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.976109 lino-avanti-23.4.0/lino_avanti/lib/avanti/locale/de/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti/lib/avanti/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6679 2020-04-20 16:09:38.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    19981 2021-02-11 19:04:16.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/locale/de/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.976109 lino-avanti-23.4.0/lino_avanti/lib/avanti/locale/fr/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti/lib/avanti/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    38461 2016-11-20 18:48:07.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    96464 2021-02-11 19:04:17.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/locale/fr/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.976109 lino-avanti-23.4.0/lino_avanti/lib/avanti/locale/nl/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti/lib/avanti/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      409 2015-09-19 03:53:53.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    93297 2021-02-11 17:36:49.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/locale/nl/LC_MESSAGES/django.po
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      683 2021-04-07 10:22:54.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/migrate.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    21966 2022-09-05 23:22:01.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      704 2021-04-07 10:22:54.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/roles.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     5885 2023-04-01 07:25:11.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/settings.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3499 2021-11-12 10:16:18.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/user_types.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1780 2021-04-07 10:22:54.000000 lino-avanti-23.4.0/lino_avanti/lib/avanti/workflows.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti/lib/cal/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      667 2021-04-07 10:22:54.000000 lino-avanti-23.4.0/lino_avanti/lib/cal/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti/lib/cal/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:36:34.000000 lino-avanti-23.4.0/lino_avanti/lib/cal/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       45 2016-02-22 08:52:24.000000 lino-avanti-23.4.0/lino_avanti/lib/cal/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      370 2018-10-07 07:17:23.000000 lino-avanti-23.4.0/lino_avanti/lib/cal/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1513 2021-04-07 10:22:54.000000 lino-avanti-23.4.0/lino_avanti/lib/cal/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti/lib/contacts/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      425 2021-04-07 10:22:54.000000 lino-avanti-23.4.0/lino_avanti/lib/contacts/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti/lib/contacts/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:36:35.000000 lino-avanti-23.4.0/lino_avanti/lib/contacts/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       55 2016-07-06 14:59:00.000000 lino-avanti-23.4.0/lino_avanti/lib/contacts/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       54 2016-07-06 14:59:00.000000 lino-avanti-23.4.0/lino_avanti/lib/contacts/fixtures/std.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti/lib/contacts/management/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:36:35.000000 lino-avanti-23.4.0/lino_avanti/lib/contacts/management/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti/lib/contacts/management/commands/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:36:35.000000 lino-avanti-23.4.0/lino_avanti/lib/contacts/management/commands/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       71 2016-07-06 14:58:59.000000 lino-avanti-23.4.0/lino_avanti/lib/contacts/management/commands/garble_persons.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3095 2022-09-05 23:22:02.000000 lino-avanti-23.4.0/lino_avanti/lib/contacts/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti/lib/courses/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      959 2021-04-07 10:22:54.000000 lino-avanti-23.4.0/lino_avanti/lib/courses/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      719 2021-04-07 10:22:54.000000 lino-avanti-23.4.0/lino_avanti/lib/courses/choicelists.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.976109 lino-avanti-23.4.0/lino_avanti/lib/courses/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.976109 lino-avanti-23.4.0/lino_avanti/lib/courses/config/courses/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti/lib/courses/config/courses/Enrolment/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    49781 2017-10-04 00:59:51.000000 lino-avanti-23.4.0/lino_avanti/lib/courses/config/courses/Enrolment/Default.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti/lib/courses/config/courses/Reminder/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    40323 2018-01-15 02:55:31.000000 lino-avanti-23.4.0/lino_avanti/lib/courses/config/courses/Reminder/Default.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-10-04 00:40:35.000000 lino-avanti-23.4.0/lino_avanti/lib/courses/config/courses/Reminder/body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3009 2018-01-17 21:32:39.000000 lino-avanti-23.4.0/lino_avanti/lib/courses/config/courses/Reminder/reminder.body.html
+-rw-rw-r--   0 luc       (1000) www-data    (33)    11058 2023-04-05 09:41:20.000000 lino-avanti-23.4.0/lino_avanti/lib/courses/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     5900 2022-11-08 12:30:48.000000 lino-avanti-23.4.0/lino_avanti/lib/courses/ui.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      415 2020-11-04 09:18:05.000000 lino-avanti-23.4.0/lino_avanti/lib/courses/workflows.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti/lib/cv/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      316 2021-04-07 10:22:54.000000 lino-avanti-23.4.0/lino_avanti/lib/cv/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti/lib/cv/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:36:34.000000 lino-avanti-23.4.0/lino_avanti/lib/cv/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2019-09-21 18:31:41.000000 lino-avanti-23.4.0/lino_avanti/lib/cv/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1437 2021-04-07 10:22:54.000000 lino-avanti-23.4.0/lino_avanti/lib/cv/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.984109 lino-avanti-23.4.0/lino_avanti/lib/households/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      295 2021-04-07 10:22:54.000000 lino-avanti-23.4.0/lino_avanti/lib/households/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.984109 lino-avanti-23.4.0/lino_avanti/lib/households/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:45.000000 lino-avanti-23.4.0/lino_avanti/lib/households/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       51 2016-02-22 08:57:42.000000 lino-avanti-23.4.0/lino_avanti/lib/households/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       50 2016-02-22 08:57:42.000000 lino-avanti-23.4.0/lino_avanti/lib/households/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      871 2021-04-07 10:22:54.000000 lino-avanti-23.4.0/lino_avanti/lib/households/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.984109 lino-avanti-23.4.0/lino_avanti/lib/tickets/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      329 2021-04-07 10:22:54.000000 lino-avanti-23.4.0/lino_avanti/lib/tickets/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1324 2021-04-07 10:22:54.000000 lino-avanti-23.4.0/lino_avanti/lib/tickets/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.984109 lino-avanti-23.4.0/lino_avanti/lib/users/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      385 2022-11-08 14:56:08.000000 lino-avanti-23.4.0/lino_avanti/lib/users/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.984109 lino-avanti-23.4.0/lino_avanti/lib/users/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:53.000000 lino-avanti-23.4.0/lino_avanti/lib/users/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-06-13 23:56:47.000000 lino-avanti-23.4.0/lino_avanti/lib/users/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2017-06-13 23:56:47.000000 lino-avanti-23.4.0/lino_avanti/lib/users/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2017-06-13 23:56:48.000000 lino-avanti-23.4.0/lino_avanti/lib/users/fixtures/demo_users.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      238 2022-11-08 12:29:27.000000 lino-avanti-23.4.0/lino_avanti/lib/users/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1142 2023-04-15 09:46:50.000000 lino-avanti-23.4.0/lino_avanti/lib/users/ui.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3529 2023-04-30 03:11:17.000000 lino-avanti-23.4.0/lino_avanti/setup_info.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.980109 lino-avanti-23.4.0/lino_avanti.egg-info/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2107 2023-04-30 03:12:01.000000 lino-avanti-23.4.0/lino_avanti.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2936 2023-04-30 03:12:01.000000 lino-avanti-23.4.0/lino_avanti.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-04-30 03:12:01.000000 lino-avanti-23.4.0/lino_avanti.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       17 2023-04-30 03:12:01.000000 lino-avanti-23.4.0/lino_avanti.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       12 2023-04-30 03:12:01.000000 lino-avanti-23.4.0/lino_avanti.egg-info/top_level.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      136 2021-05-05 05:16:56.000000 lino-avanti-23.4.0/requirements.stable.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      122 2021-05-05 05:16:56.000000 lino-avanti-23.4.0/requirements.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-04-30 03:12:01.984109 lino-avanti-23.4.0/setup.cfg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      182 2020-07-10 08:02:46.000000 lino-avanti-23.4.0/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      252 2018-04-29 04:12:02.000000 lino-avanti-23.4.0/tasks.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-30 03:12:01.984109 lino-avanti-23.4.0/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      797 2022-10-18 03:28:38.000000 lino-avanti-23.4.0/tests/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      189 2020-04-20 16:10:32.000000 lino-avanti-23.4.0/tests/test_docs.py
```

### Comparing `lino-avanti-23.3.0/COPYING` & `lino-avanti-23.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/PKG-INFO` & `lino-avanti-23.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-avanti
-Version: 23.3.0
+Version: 23.4.0
 Summary: Manage the integration course of immigrants in East Belgium
 Home-page: https://gitlab.com/lino-framework/avanti
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `lino-avanti-23.3.0/README.rst` & `lino-avanti-23.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/__init__.py` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/choicelists.py` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/config/avanti/Client/final_report.weasy.html` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/config/avanti/Client/final_report.weasy.html`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/fixtures/demo.py` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/fixtures/demo2.py` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/fixtures/demo2.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,8 +24,8 @@
     # removed 20190727 because it causes failure under mysql
     # # obj = rt.models.courses.Enrolment.objects.order_by('id')[1]
     # obj = rt.models.courses.Enrolment.objects.get(pk=2)
     # yield rt.models.courses.Reminder(
     #     enrolment=obj, user=obj.pupil.user,
     #     date_issued=settings.SITE.demo_date(-10))
 
-    rt.models.courses.update_missing_rates()
+    rt.models.courses.update_missing_rates(rt.login('robin'))
```

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/fixtures/std.py` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/help_texts.py` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/help_texts.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/layouts.py` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/layouts.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/locale/de/LC_MESSAGES/django.mo` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/locale/de/LC_MESSAGES/django.po` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/locale/fr/LC_MESSAGES/django.mo` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/locale/fr/LC_MESSAGES/django.po` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/locale/nl/LC_MESSAGES/django.po` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/migrate.py` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/migrate.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/models.py` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/models.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/roles.py` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/roles.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/settings.py` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     # textfield_format = 'html'
     # use_silk_icons = False
     default_build_method = "appypdf"
 
     webdav_protocol = 'webdav'
     # beid_protocol = 'beid'
 
-    auto_configure_logger_names = 'schedule atelier django lino lino_xl lino_avanti'
+    auto_configure_logger_names = 'atelier django lino lino_xl lino_avanti'
 
     def get_installed_apps(self):
         """Implements :meth:`lino.core.site.Site.get_installed_apps`.
 
         """
         yield super(Site, self).get_installed_apps()
         yield 'lino.modlib.help'
```

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/user_types.py` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/user_types.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/avanti/workflows.py` & `lino-avanti-23.4.0/lino_avanti/lib/avanti/workflows.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/cal/__init__.py` & `lino-avanti-23.4.0/lino_avanti/lib/cal/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/cal/models.py` & `lino-avanti-23.4.0/lino_avanti/lib/cal/models.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/contacts/models.py` & `lino-avanti-23.4.0/lino_avanti/lib/contacts/models.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/courses/__init__.py` & `lino-avanti-23.4.0/lino_avanti/lib/courses/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/courses/choicelists.py` & `lino-avanti-23.4.0/lino_avanti/lib/courses/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/courses/config/courses/Enrolment/Default.odt` & `lino-avanti-23.4.0/lino_avanti/lib/courses/config/courses/Enrolment/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/courses/config/courses/Reminder/Default.odt` & `lino-avanti-23.4.0/lino_avanti/lib/courses/config/courses/Reminder/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/courses/config/courses/Reminder/reminder.body.html` & `lino-avanti-23.4.0/lino_avanti/lib/courses/config/courses/Reminder/reminder.body.html`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/courses/models.py` & `lino-avanti-23.4.0/lino_avanti/lib/courses/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,13 +306,13 @@
 #         if obj.pupil and obj.pupil.user:
 #             return obj.pupil.user
 #         return super(EnrolmentChecker, self).get_responsible_user(obj)
 
 # EnrolmentChecker.activate()
 
 @dd.schedule_daily()
-def update_missing_rates():
+def update_missing_rates(ar):
     for obj in rt.models.courses.Enrolment.objects.all():
         obj.update_missing_rate()
 
 
 from .ui import *
```

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/courses/ui.py` & `lino-avanti-23.4.0/lino_avanti/lib/courses/ui.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/cv/models.py` & `lino-avanti-23.4.0/lino_avanti/lib/cv/models.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/households/models.py` & `lino-avanti-23.4.0/lino_avanti/lib/households/models.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/tickets/models.py` & `lino-avanti-23.4.0/lino_avanti/lib/tickets/models.py`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/lino_avanti/lib/users/ui.py` & `lino-avanti-23.4.0/lino_avanti/lib/users/ui.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     """
 
     calendar = dd.Panel("""
     cal_left:30 cal.TasksByUser:60
     """, label=dd.plugins.cal.verbose_name, required_roles=dd.login_required(OfficeUser))
 
     cal_left = """
-    event_type access_class
+    event_type 
     cal.SubscriptionsByUser
     # cal.MembershipsByUser
     """
 
     coaching = dd.Panel("""
     coaching_type coaching_supervisor
     coachings.CoachingsByUser:40
```

### Comparing `lino-avanti-23.3.0/lino_avanti/setup_info.py` & `lino-avanti-23.4.0/lino_avanti/setup_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2017-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 # test it with: $ python setup.py test -s tests.PackagesTests
 SETUP_INFO = dict(
     name='lino-avanti',
-    version='23.3.0',
+    version='23.4.0',
     install_requires=['lino-xl', 'metafone'],
     description=("Manage the integration course of immigrants in East Belgium"),
     author='Rumma & Ko Ltd',
     author_email='info@lino-framework.org',
     url="https://gitlab.com/lino-framework/avanti",
     license_files=['COPYING'],
     test_suite='tests')
```

### Comparing `lino-avanti-23.3.0/lino_avanti.egg-info/PKG-INFO` & `lino-avanti-23.4.0/lino_avanti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-avanti
-Version: 23.3.0
+Version: 23.4.0
 Summary: Manage the integration course of immigrants in East Belgium
 Home-page: https://gitlab.com/lino-framework/avanti
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `lino-avanti-23.3.0/lino_avanti.egg-info/SOURCES.txt` & `lino-avanti-23.4.0/lino_avanti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lino-avanti-23.3.0/tests/__init__.py` & `lino-avanti-23.4.0/tests/__init__.py`

 * *Files identical despite different names*

