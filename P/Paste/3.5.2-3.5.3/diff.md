# Comparing `tmp/Paste-3.5.2.tar.gz` & `tmp/Paste-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Paste-3.5.2.tar", last modified: Thu Aug 18 20:37:49 2022, max compression
+gzip compressed data, was "Paste-3.5.3.tar", last modified: Sun Apr 30 11:41:24 2023, max compression
```

## Comparing `Paste-3.5.2.tar` & `Paste-3.5.3.tar`

### file list

```diff
@@ -1,274 +1,274 @@
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.158675 Paste-3.5.2/
--rw-r--r--   0 cdent      (503) staff       (20)      323 2020-01-26 15:30:37.000000 Paste-3.5.2/MANIFEST.in
--rw-r--r--   0 cdent      (503) staff       (20)     4368 2022-08-18 20:37:49.158880 Paste-3.5.2/PKG-INFO
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:48.990765 Paste-3.5.2/Paste.egg-info/
--rw-r--r--   0 cdent      (503) staff       (20)     4368 2022-08-18 20:37:48.000000 Paste-3.5.2/Paste.egg-info/PKG-INFO
--rw-r--r--   0 cdent      (503) staff       (20)     6439 2022-08-18 20:37:48.000000 Paste-3.5.2/Paste.egg-info/SOURCES.txt
--rw-r--r--   0 cdent      (503) staff       (20)        1 2022-08-18 20:37:48.000000 Paste-3.5.2/Paste.egg-info/dependency_links.txt
--rw-r--r--   0 cdent      (503) staff       (20)     1900 2022-08-18 20:37:48.000000 Paste-3.5.2/Paste.egg-info/entry_points.txt
--rw-r--r--   0 cdent      (503) staff       (20)        6 2022-08-18 20:37:48.000000 Paste-3.5.2/Paste.egg-info/namespace_packages.txt
--rw-r--r--   0 cdent      (503) staff       (20)        1 2020-01-26 15:31:09.000000 Paste-3.5.2/Paste.egg-info/not-zip-safe
--rw-r--r--   0 cdent      (503) staff       (20)       93 2022-08-18 20:37:48.000000 Paste-3.5.2/Paste.egg-info/requires.txt
--rw-r--r--   0 cdent      (503) staff       (20)        6 2022-08-18 20:37:48.000000 Paste-3.5.2/Paste.egg-info/top_level.txt
--rw-r--r--   0 cdent      (503) staff       (20)     3299 2020-06-04 11:56:09.000000 Paste-3.5.2/README.rst
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.007334 Paste-3.5.2/docs/
--rw-r--r--   0 cdent      (503) staff       (20)     4608 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/DeveloperGuidelines.txt
--rw-r--r--   0 cdent      (503) staff       (20)     3170 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/StyleGuide.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.008706 Paste-3.5.2/docs/_static/
--rw-r--r--   0 cdent      (503) staff       (20)     5988 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/_static/default.css
--rw-r--r--   0 cdent      (503) staff       (20)      194 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/_static/paste.css
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.010849 Paste-3.5.2/docs/community/
--rw-r--r--   0 cdent      (503) staff       (20)      571 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/community/index.txt
--rw-r--r--   0 cdent      (503) staff       (20)      759 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/community/mailing-list.txt
--rw-r--r--   0 cdent      (503) staff       (20)      141 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/community/repository.txt
--rw-r--r--   0 cdent      (503) staff       (20)     4078 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/conf.py
--rw-r--r--   0 cdent      (503) staff       (20)     4500 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/developer-features.txt
--rw-r--r--   0 cdent      (503) staff       (20)    19254 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/do-it-yourself-framework.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.011401 Paste-3.5.2/docs/download/
--rw-r--r--   0 cdent      (503) staff       (20)     1383 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/download/index.txt
--rw-r--r--   0 cdent      (503) staff       (20)     3184 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/future.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.012386 Paste-3.5.2/docs/include/
--rw-r--r--   0 cdent      (503) staff       (20)      338 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/include/contact.txt
--rw-r--r--   0 cdent      (503) staff       (20)       66 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/include/reference_header.txt
--rw-r--r--   0 cdent      (503) staff       (20)     1985 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/index.txt
--rw-r--r--   0 cdent      (503) staff       (20)     1077 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/license.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.036044 Paste-3.5.2/docs/modules/
--rw-r--r--   0 cdent      (503) staff       (20)      312 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/auth.auth_tkt.txt
--rw-r--r--   0 cdent      (503) staff       (20)      273 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/auth.basic.txt
--rw-r--r--   0 cdent      (503) staff       (20)      186 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/auth.cas.txt
--rw-r--r--   0 cdent      (503) staff       (20)      314 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/auth.cookie.txt
--rw-r--r--   0 cdent      (503) staff       (20)      297 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/auth.digest.txt
--rw-r--r--   0 cdent      (503) staff       (20)      242 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/auth.form.txt
--rw-r--r--   0 cdent      (503) staff       (20)      272 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/auth.grantip.txt
--rw-r--r--   0 cdent      (503) staff       (20)      238 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/auth.multi.txt
--rw-r--r--   0 cdent      (503) staff       (20)      273 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/cascade.txt
--rw-r--r--   0 cdent      (503) staff       (20)      281 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/cgiapp.txt
--rw-r--r--   0 cdent      (503) staff       (20)      260 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/cgitb_catcher.txt
--rw-r--r--   0 cdent      (503) staff       (20)      280 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/debug.debugapp.txt
--rw-r--r--   0 cdent      (503) staff       (20)      354 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/debug.fsdiff.txt
--rw-r--r--   0 cdent      (503) staff       (20)      207 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/debug.prints.txt
--rw-r--r--   0 cdent      (503) staff       (20)      312 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/debug.profile.txt
--rw-r--r--   0 cdent      (503) staff       (20)      325 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/debug.watchthreads.txt
--rw-r--r--   0 cdent      (503) staff       (20)      243 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/debug.wdg_validate.txt
--rw-r--r--   0 cdent      (503) staff       (20)      288 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/errordocument.txt
--rw-r--r--   0 cdent      (503) staff       (20)      226 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/evalexception.txt
--rw-r--r--   0 cdent      (503) staff       (20)     1259 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/exceptions.txt
--rw-r--r--   0 cdent      (503) staff       (20)      248 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/fileapp.txt
--rw-r--r--   0 cdent      (503) staff       (20)      633 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/fixture.txt
--rw-r--r--   0 cdent      (503) staff       (20)      226 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/gzipper.txt
--rw-r--r--   0 cdent      (503) staff       (20)     1604 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/httpexceptions.txt
--rw-r--r--   0 cdent      (503) staff       (20)      216 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/httpheaders.txt
--rw-r--r--   0 cdent      (503) staff       (20)      202 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/httpserver.txt
--rw-r--r--   0 cdent      (503) staff       (20)      272 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/lint.txt
--rw-r--r--   0 cdent      (503) staff       (20)      232 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/pony.txt
--rw-r--r--   0 cdent      (503) staff       (20)      246 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/progress.txt
--rw-r--r--   0 cdent      (503) staff       (20)      306 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/proxy.txt
--rw-r--r--   0 cdent      (503) staff       (20)      232 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/recursive.txt
--rw-r--r--   0 cdent      (503) staff       (20)      372 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/registry.txt
--rw-r--r--   0 cdent      (503) staff       (20)      293 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/reloader.txt
--rw-r--r--   0 cdent      (503) staff       (20)      501 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/request.txt
--rw-r--r--   0 cdent      (503) staff       (20)      353 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/response.txt
--rw-r--r--   0 cdent      (503) staff       (20)      243 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/session.txt
--rw-r--r--   0 cdent      (503) staff       (20)      284 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/transaction.txt
--rw-r--r--   0 cdent      (503) staff       (20)      208 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/translogger.txt
--rw-r--r--   0 cdent      (503) staff       (20)      185 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/url.txt
--rw-r--r--   0 cdent      (503) staff       (20)      224 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/urlmap.txt
--rw-r--r--   0 cdent      (503) staff       (20)      392 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/urlparser.txt
--rw-r--r--   0 cdent      (503) staff       (20)      332 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/util.import_string.txt
--rw-r--r--   0 cdent      (503) staff       (20)      260 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/util.multidict.txt
--rw-r--r--   0 cdent      (503) staff       (20)      520 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/wsgilib.txt
--rw-r--r--   0 cdent      (503) staff       (20)      279 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/modules/wsgiwrappers.txt
--rw-r--r--   0 cdent      (503) staff       (20)    40916 2022-08-18 20:34:45.000000 Paste-3.5.2/docs/news.txt
--rw-r--r--   0 cdent      (503) staff       (20)     6405 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/paste-httpserver-threadpool.txt
--rw-r--r--   0 cdent      (503) staff       (20)      933 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/test_server.ini
--rw-r--r--   0 cdent      (503) staff       (20)     5073 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/testing-applications.txt
--rw-r--r--   0 cdent      (503) staff       (20)    12875 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/url-parsing-with-wsgi.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.037608 Paste-3.5.2/docs/web/
--rw-r--r--   0 cdent      (503) staff       (20)     5756 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/web/default-site.css
--rw-r--r--   0 cdent      (503) staff       (20)     1653 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/web/site.js
--rw-r--r--   0 cdent      (503) staff       (20)     1241 2020-01-26 15:30:37.000000 Paste-3.5.2/docs/web/style.css
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.053761 Paste-3.5.2/paste/
--rw-r--r--   0 cdent      (503) staff       (20)      551 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/__init__.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.059201 Paste-3.5.2/paste/auth/
--rw-r--r--   0 cdent      (503) staff       (20)      444 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/auth/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)    16601 2020-07-22 15:14:09.000000 Paste-3.5.2/paste/auth/auth_tkt.py
--rw-r--r--   0 cdent      (503) staff       (20)     4136 2020-10-12 12:27:11.000000 Paste-3.5.2/paste/auth/basic.py
--rw-r--r--   0 cdent      (503) staff       (20)     4006 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/auth/cas.py
--rw-r--r--   0 cdent      (503) staff       (20)    16588 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/auth/cookie.py
--rw-r--r--   0 cdent      (503) staff       (20)     9304 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/auth/digest.py
--rw-r--r--   0 cdent      (503) staff       (20)     5444 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/auth/form.py
--rw-r--r--   0 cdent      (503) staff       (20)     4021 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/auth/grantip.py
--rw-r--r--   0 cdent      (503) staff       (20)     3042 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/auth/multi.py
--rw-r--r--   0 cdent      (503) staff       (20)    16276 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/auth/open_id.py
--rw-r--r--   0 cdent      (503) staff       (20)     4475 2020-01-28 15:54:01.000000 Paste-3.5.2/paste/cascade.py
--rw-r--r--   0 cdent      (503) staff       (20)     9742 2020-10-12 12:27:11.000000 Paste-3.5.2/paste/cgiapp.py
--rw-r--r--   0 cdent      (503) staff       (20)     3903 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/cgitb_catcher.py
--rw-r--r--   0 cdent      (503) staff       (20)     4312 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/config.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.076876 Paste-3.5.2/paste/cowbell/
--rw-r--r--   0 cdent      (503) staff       (20)     3727 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/cowbell/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)   132993 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/cowbell/bell-ascending.png
--rw-r--r--   0 cdent      (503) staff       (20)   124917 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/cowbell/bell-descending.png
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.082841 Paste-3.5.2/paste/debug/
--rw-r--r--   0 cdent      (503) staff       (20)      221 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/debug/__init__.py
--rwxr-xr-x   0 cdent      (503) staff       (20)     2855 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/debug/debugapp.py
--rwxr-xr-x   0 cdent      (503) staff       (20)    14923 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/debug/doctest_webapp.py
--rw-r--r--   0 cdent      (503) staff       (20)    12902 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/debug/fsdiff.py
--rw-r--r--   0 cdent      (503) staff       (20)     5574 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/debug/prints.py
--rw-r--r--   0 cdent      (503) staff       (20)     7607 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/debug/profile.py
--rwxr-xr-x   0 cdent      (503) staff       (20)     3396 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/debug/testserver.py
--rw-r--r--   0 cdent      (503) staff       (20)    10839 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/debug/watchthreads.py
--rw-r--r--   0 cdent      (503) staff       (20)     4268 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/debug/wdg_validate.py
--rw-r--r--   0 cdent      (503) staff       (20)    13904 2020-10-12 12:27:11.000000 Paste-3.5.2/paste/errordocument.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.084380 Paste-3.5.2/paste/evalexception/
--rw-r--r--   0 cdent      (503) staff       (20)      282 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/evalexception/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     2155 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/evalexception/evalcontext.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.087472 Paste-3.5.2/paste/evalexception/media/
--rw-r--r--   0 cdent      (503) staff       (20)   202262 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/evalexception/media/MochiKit.packed.js
--rw-r--r--   0 cdent      (503) staff       (20)     4257 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/evalexception/media/debug.js
--rw-r--r--   0 cdent      (503) staff       (20)      359 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/evalexception/media/minus.jpg
--rw-r--r--   0 cdent      (503) staff       (20)      361 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/evalexception/media/plus.jpg
--rw-r--r--   0 cdent      (503) staff       (20)    22254 2020-10-12 12:27:11.000000 Paste-3.5.2/paste/evalexception/middleware.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.090538 Paste-3.5.2/paste/exceptions/
--rw-r--r--   0 cdent      (503) staff       (20)      252 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/exceptions/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)    19681 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/exceptions/collector.py
--rw-r--r--   0 cdent      (503) staff       (20)    17045 2020-10-12 12:27:11.000000 Paste-3.5.2/paste/exceptions/errormiddleware.py
--rw-r--r--   0 cdent      (503) staff       (20)    19504 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/exceptions/formatter.py
--rw-r--r--   0 cdent      (503) staff       (20)     4576 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/exceptions/reporter.py
--rw-r--r--   0 cdent      (503) staff       (20)     4127 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/exceptions/serial_number_generator.py
--rw-r--r--   0 cdent      (503) staff       (20)    13698 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/fileapp.py
--rw-r--r--   0 cdent      (503) staff       (20)    59616 2020-09-24 15:58:29.000000 Paste-3.5.2/paste/fixture.py
--rw-r--r--   0 cdent      (503) staff       (20)     3923 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/flup_session.py
--rw-r--r--   0 cdent      (503) staff       (20)     3819 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/gzipper.py
--rw-r--r--   0 cdent      (503) staff       (20)    24522 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/httpexceptions.py
--rw-r--r--   0 cdent      (503) staff       (20)    43615 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/httpheaders.py
--rwxr-xr-x   0 cdent      (503) staff       (20)    57237 2022-06-22 10:14:29.000000 Paste-3.5.2/paste/httpserver.py
--rw-r--r--   0 cdent      (503) staff       (20)    14988 2020-10-12 12:27:11.000000 Paste-3.5.2/paste/lint.py
--rw-r--r--   0 cdent      (503) staff       (20)     7830 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/modpython.py
--rw-r--r--   0 cdent      (503) staff       (20)     2279 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/pony.py
--rwxr-xr-x   0 cdent      (503) staff       (20)     8162 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/progress.py
--rw-r--r--   0 cdent      (503) staff       (20)    10192 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/proxy.py
--rw-r--r--   0 cdent      (503) staff       (20)    14708 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/recursive.py
--rw-r--r--   0 cdent      (503) staff       (20)    22275 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/registry.py
--rw-r--r--   0 cdent      (503) staff       (20)     6038 2022-06-22 10:14:29.000000 Paste-3.5.2/paste/reloader.py
--rw-r--r--   0 cdent      (503) staff       (20)    14214 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/request.py
--rw-r--r--   0 cdent      (503) staff       (20)     7659 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/response.py
--rw-r--r--   0 cdent      (503) staff       (20)    11554 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/session.py
--rw-r--r--   0 cdent      (503) staff       (20)     4363 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/transaction.py
--rw-r--r--   0 cdent      (503) staff       (20)     4887 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/translogger.py
--rw-r--r--   0 cdent      (503) staff       (20)    14738 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/url.py
--rw-r--r--   0 cdent      (503) staff       (20)     9369 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/urlmap.py
--rw-r--r--   0 cdent      (503) staff       (20)    26440 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/urlparser.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.101786 Paste-3.5.2/paste/util/
--rw-r--r--   0 cdent      (503) staff       (20)    83623 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/PySourceColor.py
--rw-r--r--   0 cdent      (503) staff       (20)       86 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     1849 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/classinit.py
--rw-r--r--   0 cdent      (503) staff       (20)     1361 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/classinstance.py
--rw-r--r--   0 cdent      (503) staff       (20)      913 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/converters.py
--rw-r--r--   0 cdent      (503) staff       (20)     2412 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/dateinterval.py
--rw-r--r--   0 cdent      (503) staff       (20)    10796 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/datetimeutil.py
--rw-r--r--   0 cdent      (503) staff       (20)     1427 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/filemixin.py
--rw-r--r--   0 cdent      (503) staff       (20)     3815 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/finddata.py
--rw-r--r--   0 cdent      (503) staff       (20)      782 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/findpackage.py
--rw-r--r--   0 cdent      (503) staff       (20)      802 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/html.py
--rw-r--r--   0 cdent      (503) staff       (20)     3114 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/import_string.py
--rw-r--r--   0 cdent      (503) staff       (20)    19262 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/intset.py
--rw-r--r--   0 cdent      (503) staff       (20)     9320 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/ip4.py
--rw-r--r--   0 cdent      (503) staff       (20)     1227 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/killthread.py
--rw-r--r--   0 cdent      (503) staff       (20)     4036 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/looper.py
--rw-r--r--   0 cdent      (503) staff       (20)     6604 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/mimeparse.py
--rw-r--r--   0 cdent      (503) staff       (20)    12682 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/multidict.py
--rw-r--r--   0 cdent      (503) staff       (20)     2351 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/quoting.py
--rw-r--r--   0 cdent      (503) staff       (20)     5612 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/scgiserver.py
--rw-r--r--   0 cdent      (503) staff       (20)    24403 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/template.py
--rw-r--r--   0 cdent      (503) staff       (20)     8175 2022-06-22 10:14:29.000000 Paste-3.5.2/paste/util/threadedprint.py
--rw-r--r--   0 cdent      (503) staff       (20)     1484 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/util/threadinglocal.py
--rw-r--r--   0 cdent      (503) staff       (20)    20470 2022-08-18 20:32:03.000000 Paste-3.5.2/paste/wsgilib.py
--rw-r--r--   0 cdent      (503) staff       (20)    22299 2020-01-26 15:30:37.000000 Paste-3.5.2/paste/wsgiwrappers.py
--rwxr-xr-x   0 cdent      (503) staff       (20)      234 2020-01-26 15:30:37.000000 Paste-3.5.2/regen-docs
--rw-r--r--   0 cdent      (503) staff       (20)      191 2022-08-18 20:37:49.159904 Paste-3.5.2/setup.cfg
--rw-r--r--   0 cdent      (503) staff       (20)     4507 2022-08-18 20:33:28.000000 Paste-3.5.2/setup.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.115719 Paste-3.5.2/tests/
--rw-r--r--   0 cdent      (503) staff       (20)      138 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/__init__.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.117715 Paste-3.5.2/tests/cgiapp_data/
--rwxr-xr-x   0 cdent      (503) staff       (20)       41 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/cgiapp_data/error.cgi
--rwxr-xr-x   0 cdent      (503) staff       (20)     1816 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/cgiapp_data/form.cgi
--rwxr-xr-x   0 cdent      (503) staff       (20)      132 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/cgiapp_data/ok.cgi
--rwxr-xr-x   0 cdent      (503) staff       (20)      223 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/cgiapp_data/stderr.cgi
--rw-r--r--   0 cdent      (503) staff       (20)     4132 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/template.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.119737 Paste-3.5.2/tests/test_auth/
--rw-r--r--   0 cdent      (503) staff       (20)        0 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_auth/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     1527 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_auth/test_auth_cookie.py
--rw-r--r--   0 cdent      (503) staff       (20)     3077 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_auth/test_auth_digest.py
--rw-r--r--   0 cdent      (503) staff       (20)     3832 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_auth/test_auth_tkt.py
--rw-r--r--   0 cdent      (503) staff       (20)     2053 2020-10-12 12:27:11.000000 Paste-3.5.2/tests/test_cgiapp.py
--rw-r--r--   0 cdent      (503) staff       (20)     2249 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_cgitb_catcher.py
--rw-r--r--   0 cdent      (503) staff       (20)     2901 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_config.py
--rw-r--r--   0 cdent      (503) staff       (20)     1533 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_doctests.py
--rw-r--r--   0 cdent      (503) staff       (20)     3461 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_errordocument.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.143334 Paste-3.5.2/tests/test_exceptions/
--rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_exceptions/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     3389 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_exceptions/test_error_middleware.py
--rw-r--r--   0 cdent      (503) staff       (20)     4985 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_exceptions/test_formatter.py
--rw-r--r--   0 cdent      (503) staff       (20)     4055 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_exceptions/test_httpexceptions.py
--rw-r--r--   0 cdent      (503) staff       (20)     1280 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_exceptions/test_reporter.py
--rw-r--r--   0 cdent      (503) staff       (20)     9766 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_fileapp.py
--rw-r--r--   0 cdent      (503) staff       (20)     2489 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_fixture.py
--rw-r--r--   0 cdent      (503) staff       (20)     1272 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_grantip.py
--rw-r--r--   0 cdent      (503) staff       (20)      888 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_gzipper.py
--rw-r--r--   0 cdent      (503) staff       (20)     6505 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_httpheaders.py
--rw-r--r--   0 cdent      (503) staff       (20)     3447 2020-02-12 10:40:19.000000 Paste-3.5.2/tests/test_httpserver.py
--rw-r--r--   0 cdent      (503) staff       (20)      477 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_import_string.py
--rw-r--r--   0 cdent      (503) staff       (20)     5255 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_multidict.py
--rw-r--r--   0 cdent      (503) staff       (20)      721 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_profilemiddleware.py
--rw-r--r--   0 cdent      (503) staff       (20)      418 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_proxy.py
--rw-r--r--   0 cdent      (503) staff       (20)     4178 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_recursive.py
--rw-r--r--   0 cdent      (503) staff       (20)    11149 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_registry.py
--rw-r--r--   0 cdent      (503) staff       (20)     2354 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_request.py
--rw-r--r--   0 cdent      (503) staff       (20)     1183 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_request_form.py
--rw-r--r--   0 cdent      (503) staff       (20)      369 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_response.py
--rw-r--r--   0 cdent      (503) staff       (20)     1587 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_session.py
--rw-r--r--   0 cdent      (503) staff       (20)     1810 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_urlmap.py
--rw-r--r--   0 cdent      (503) staff       (20)     6944 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_urlparser.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.145956 Paste-3.5.2/tests/test_util/
--rw-r--r--   0 cdent      (503) staff       (20)        0 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_util/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     6026 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_util/test_datetimeutil.py
--rw-r--r--   0 cdent      (503) staff       (20)    11873 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_util/test_mimeparse.py
--rw-r--r--   0 cdent      (503) staff       (20)     1171 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_util/test_quoting.py
--rw-r--r--   0 cdent      (503) staff       (20)      842 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_wsgilib.py
--rw-r--r--   0 cdent      (503) staff       (20)     6441 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/test_wsgiwrappers.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.147216 Paste-3.5.2/tests/urlparser_data/
--rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/__init__.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.147866 Paste-3.5.2/tests/urlparser_data/deep/
--rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/deep/index.html
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.148419 Paste-3.5.2/tests/urlparser_data/deep/sub/
--rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/deep/sub/Main.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.149932 Paste-3.5.2/tests/urlparser_data/find_file/
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.150372 Paste-3.5.2/tests/urlparser_data/find_file/dir with spaces/
--rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/find_file/dir with spaces/test 4.html
--rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/find_file/index.txt
--rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/find_file/test 3.html
--rw-r--r--   0 cdent      (503) staff       (20)        6 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/find_file/test2.html
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.151709 Paste-3.5.2/tests/urlparser_data/hook/
--rw-r--r--   0 cdent      (503) staff       (20)      289 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/hook/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)      231 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/hook/app.py
--rw-r--r--   0 cdent      (503) staff       (20)      232 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/hook/index.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.152158 Paste-3.5.2/tests/urlparser_data/not_found/
--rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/not_found/__init__.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.153042 Paste-3.5.2/tests/urlparser_data/not_found/recur/
--rw-r--r--   0 cdent      (503) staff       (20)      374 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/not_found/recur/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)        9 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/not_found/recur/isfound.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.153896 Paste-3.5.2/tests/urlparser_data/not_found/simple/
--rw-r--r--   0 cdent      (503) staff       (20)      134 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/not_found/simple/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)        9 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/not_found/simple/found.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.154923 Paste-3.5.2/tests/urlparser_data/not_found/user/
--rw-r--r--   0 cdent      (503) staff       (20)      411 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/not_found/user/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)      235 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/not_found/user/list.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.156826 Paste-3.5.2/tests/urlparser_data/python/
--rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/python/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)      183 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/python/simpleapp.py
--rw-r--r--   0 cdent      (503) staff       (20)      208 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/python/stream.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-08-18 20:37:49.158151 Paste-3.5.2/tests/urlparser_data/python/sub/
--rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/python/sub/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)      186 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/python/sub/simpleapp.py
--rw-r--r--   0 cdent      (503) staff       (20)        8 2020-01-26 15:30:37.000000 Paste-3.5.2/tests/urlparser_data/secured.txt
--rw-r--r--   0 cdent      (503) staff       (20)      362 2022-06-22 10:16:25.000000 Paste-3.5.2/tox.ini
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.440560 Paste-3.5.3/
+-rw-r--r--   0 cdent      (503) staff       (20)      323 2020-01-26 15:30:37.000000 Paste-3.5.3/MANIFEST.in
+-rw-r--r--   0 cdent      (503) staff       (20)     4547 2023-04-30 11:41:24.440674 Paste-3.5.3/PKG-INFO
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.354262 Paste-3.5.3/Paste.egg-info/
+-rw-r--r--   0 cdent      (503) staff       (20)     4547 2023-04-30 11:41:24.000000 Paste-3.5.3/Paste.egg-info/PKG-INFO
+-rw-r--r--   0 cdent      (503) staff       (20)     6439 2023-04-30 11:41:24.000000 Paste-3.5.3/Paste.egg-info/SOURCES.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        1 2023-04-30 11:41:24.000000 Paste-3.5.3/Paste.egg-info/dependency_links.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     1900 2023-04-30 11:41:24.000000 Paste-3.5.3/Paste.egg-info/entry_points.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        6 2023-04-30 11:41:24.000000 Paste-3.5.3/Paste.egg-info/namespace_packages.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        1 2020-01-26 15:31:09.000000 Paste-3.5.3/Paste.egg-info/not-zip-safe
+-rw-r--r--   0 cdent      (503) staff       (20)       93 2023-04-30 11:41:24.000000 Paste-3.5.3/Paste.egg-info/requires.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        6 2023-04-30 11:41:24.000000 Paste-3.5.3/Paste.egg-info/top_level.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     3299 2020-06-04 11:56:09.000000 Paste-3.5.3/README.rst
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.364586 Paste-3.5.3/docs/
+-rw-r--r--   0 cdent      (503) staff       (20)     4608 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/DeveloperGuidelines.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     3170 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/StyleGuide.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.365956 Paste-3.5.3/docs/_static/
+-rw-r--r--   0 cdent      (503) staff       (20)     5988 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/_static/default.css
+-rw-r--r--   0 cdent      (503) staff       (20)      194 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/_static/paste.css
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.367625 Paste-3.5.3/docs/community/
+-rw-r--r--   0 cdent      (503) staff       (20)      571 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/community/index.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      759 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/community/mailing-list.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      141 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/community/repository.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     4078 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/conf.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4500 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/developer-features.txt
+-rw-r--r--   0 cdent      (503) staff       (20)    19254 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/do-it-yourself-framework.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.368181 Paste-3.5.3/docs/download/
+-rw-r--r--   0 cdent      (503) staff       (20)     1383 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/download/index.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     3184 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/future.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.369192 Paste-3.5.3/docs/include/
+-rw-r--r--   0 cdent      (503) staff       (20)      338 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/include/contact.txt
+-rw-r--r--   0 cdent      (503) staff       (20)       66 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/include/reference_header.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     1985 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/index.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     1077 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/license.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.385463 Paste-3.5.3/docs/modules/
+-rw-r--r--   0 cdent      (503) staff       (20)      312 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/auth.auth_tkt.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      273 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/auth.basic.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      186 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/auth.cas.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      314 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/auth.cookie.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      297 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/auth.digest.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      242 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/auth.form.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      272 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/auth.grantip.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      238 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/auth.multi.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      273 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/cascade.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      281 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/cgiapp.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      260 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/cgitb_catcher.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      280 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/debug.debugapp.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      354 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/debug.fsdiff.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      207 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/debug.prints.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      312 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/debug.profile.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      325 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/debug.watchthreads.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      243 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/debug.wdg_validate.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      288 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/errordocument.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      226 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/evalexception.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     1259 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/exceptions.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      248 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/fileapp.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      633 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/fixture.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      226 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/gzipper.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     1604 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/httpexceptions.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      216 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/httpheaders.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      202 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/httpserver.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      272 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/lint.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      232 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/pony.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      246 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/progress.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      306 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/proxy.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      232 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/recursive.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      372 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/registry.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      293 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/reloader.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      501 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/request.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      353 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/response.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      243 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/session.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      284 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/transaction.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      208 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/translogger.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      185 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/url.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      224 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/urlmap.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      392 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/urlparser.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      332 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/util.import_string.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      260 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/util.multidict.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      520 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/wsgilib.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      279 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/modules/wsgiwrappers.txt
+-rw-r--r--   0 cdent      (503) staff       (20)    40977 2023-04-30 11:36:33.000000 Paste-3.5.3/docs/news.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     6405 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/paste-httpserver-threadpool.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      933 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/test_server.ini
+-rw-r--r--   0 cdent      (503) staff       (20)     5073 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/testing-applications.txt
+-rw-r--r--   0 cdent      (503) staff       (20)    12875 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/url-parsing-with-wsgi.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.386355 Paste-3.5.3/docs/web/
+-rw-r--r--   0 cdent      (503) staff       (20)     5756 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/web/default-site.css
+-rw-r--r--   0 cdent      (503) staff       (20)     1653 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/web/site.js
+-rw-r--r--   0 cdent      (503) staff       (20)     1241 2020-01-26 15:30:37.000000 Paste-3.5.3/docs/web/style.css
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.396771 Paste-3.5.3/paste/
+-rw-r--r--   0 cdent      (503) staff       (20)      551 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/__init__.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.399680 Paste-3.5.3/paste/auth/
+-rw-r--r--   0 cdent      (503) staff       (20)      444 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/auth/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)    16601 2020-07-22 15:14:09.000000 Paste-3.5.3/paste/auth/auth_tkt.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4136 2020-10-12 12:27:11.000000 Paste-3.5.3/paste/auth/basic.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4006 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/auth/cas.py
+-rw-r--r--   0 cdent      (503) staff       (20)    16588 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/auth/cookie.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9304 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/auth/digest.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5444 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/auth/form.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4021 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/auth/grantip.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3042 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/auth/multi.py
+-rw-r--r--   0 cdent      (503) staff       (20)    16276 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/auth/open_id.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4475 2020-01-28 15:54:01.000000 Paste-3.5.3/paste/cascade.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9742 2020-10-12 12:27:11.000000 Paste-3.5.3/paste/cgiapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3903 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/cgitb_catcher.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4312 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/config.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.401880 Paste-3.5.3/paste/cowbell/
+-rw-r--r--   0 cdent      (503) staff       (20)     3727 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/cowbell/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)   132993 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/cowbell/bell-ascending.png
+-rw-r--r--   0 cdent      (503) staff       (20)   124917 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/cowbell/bell-descending.png
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.404505 Paste-3.5.3/paste/debug/
+-rw-r--r--   0 cdent      (503) staff       (20)      221 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/debug/__init__.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)     2855 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/debug/debugapp.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)    14923 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/debug/doctest_webapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)    12902 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/debug/fsdiff.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5574 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/debug/prints.py
+-rw-r--r--   0 cdent      (503) staff       (20)     7607 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/debug/profile.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)     3396 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/debug/testserver.py
+-rw-r--r--   0 cdent      (503) staff       (20)    10839 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/debug/watchthreads.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4268 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/debug/wdg_validate.py
+-rw-r--r--   0 cdent      (503) staff       (20)    13904 2020-10-12 12:27:11.000000 Paste-3.5.3/paste/errordocument.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.405237 Paste-3.5.3/paste/evalexception/
+-rw-r--r--   0 cdent      (503) staff       (20)      282 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/evalexception/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2155 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/evalexception/evalcontext.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.406802 Paste-3.5.3/paste/evalexception/media/
+-rw-r--r--   0 cdent      (503) staff       (20)   202262 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/evalexception/media/MochiKit.packed.js
+-rw-r--r--   0 cdent      (503) staff       (20)     4257 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/evalexception/media/debug.js
+-rw-r--r--   0 cdent      (503) staff       (20)      359 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/evalexception/media/minus.jpg
+-rw-r--r--   0 cdent      (503) staff       (20)      361 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/evalexception/media/plus.jpg
+-rw-r--r--   0 cdent      (503) staff       (20)    22254 2020-10-12 12:27:11.000000 Paste-3.5.3/paste/evalexception/middleware.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.408619 Paste-3.5.3/paste/exceptions/
+-rw-r--r--   0 cdent      (503) staff       (20)      252 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/exceptions/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)    19681 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/exceptions/collector.py
+-rw-r--r--   0 cdent      (503) staff       (20)    17045 2020-10-12 12:27:11.000000 Paste-3.5.3/paste/exceptions/errormiddleware.py
+-rw-r--r--   0 cdent      (503) staff       (20)    19504 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/exceptions/formatter.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4576 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/exceptions/reporter.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4127 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/exceptions/serial_number_generator.py
+-rw-r--r--   0 cdent      (503) staff       (20)    13698 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/fileapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)    59616 2020-09-24 15:58:29.000000 Paste-3.5.3/paste/fixture.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3923 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/flup_session.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3819 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/gzipper.py
+-rw-r--r--   0 cdent      (503) staff       (20)    24522 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/httpexceptions.py
+-rw-r--r--   0 cdent      (503) staff       (20)    43615 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/httpheaders.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)    57237 2022-06-22 10:14:29.000000 Paste-3.5.3/paste/httpserver.py
+-rw-r--r--   0 cdent      (503) staff       (20)    14988 2020-10-12 12:27:11.000000 Paste-3.5.3/paste/lint.py
+-rw-r--r--   0 cdent      (503) staff       (20)     7830 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/modpython.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2279 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/pony.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)     8162 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/progress.py
+-rw-r--r--   0 cdent      (503) staff       (20)    10192 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/proxy.py
+-rw-r--r--   0 cdent      (503) staff       (20)    14708 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/recursive.py
+-rw-r--r--   0 cdent      (503) staff       (20)    22275 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/registry.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6038 2022-06-22 10:14:29.000000 Paste-3.5.3/paste/reloader.py
+-rw-r--r--   0 cdent      (503) staff       (20)    14214 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/request.py
+-rw-r--r--   0 cdent      (503) staff       (20)     7659 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/response.py
+-rw-r--r--   0 cdent      (503) staff       (20)    11554 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/session.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4363 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/transaction.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4887 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/translogger.py
+-rw-r--r--   0 cdent      (503) staff       (20)    14738 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/url.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9369 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/urlmap.py
+-rw-r--r--   0 cdent      (503) staff       (20)    26865 2023-04-30 11:31:00.000000 Paste-3.5.3/paste/urlparser.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.415639 Paste-3.5.3/paste/util/
+-rw-r--r--   0 cdent      (503) staff       (20)    83623 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/PySourceColor.py
+-rw-r--r--   0 cdent      (503) staff       (20)       86 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1849 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/classinit.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1361 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/classinstance.py
+-rw-r--r--   0 cdent      (503) staff       (20)      913 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/converters.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2412 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/dateinterval.py
+-rw-r--r--   0 cdent      (503) staff       (20)    10796 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/datetimeutil.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1427 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/filemixin.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3815 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/finddata.py
+-rw-r--r--   0 cdent      (503) staff       (20)      782 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/findpackage.py
+-rw-r--r--   0 cdent      (503) staff       (20)      802 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/html.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3114 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/import_string.py
+-rw-r--r--   0 cdent      (503) staff       (20)    19262 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/intset.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9320 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/ip4.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1227 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/killthread.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4036 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/looper.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6604 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/mimeparse.py
+-rw-r--r--   0 cdent      (503) staff       (20)    12682 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/multidict.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2351 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/quoting.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5612 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/scgiserver.py
+-rw-r--r--   0 cdent      (503) staff       (20)    24403 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/template.py
+-rw-r--r--   0 cdent      (503) staff       (20)     8175 2022-06-22 10:14:29.000000 Paste-3.5.3/paste/util/threadedprint.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1484 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/util/threadinglocal.py
+-rw-r--r--   0 cdent      (503) staff       (20)    20470 2022-08-18 20:32:03.000000 Paste-3.5.3/paste/wsgilib.py
+-rw-r--r--   0 cdent      (503) staff       (20)    22299 2020-01-26 15:30:37.000000 Paste-3.5.3/paste/wsgiwrappers.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)      234 2020-01-26 15:30:37.000000 Paste-3.5.3/regen-docs
+-rw-r--r--   0 cdent      (503) staff       (20)      191 2023-04-30 11:41:24.441071 Paste-3.5.3/setup.cfg
+-rw-r--r--   0 cdent      (503) staff       (20)     4715 2023-04-30 11:37:30.000000 Paste-3.5.3/setup.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.427981 Paste-3.5.3/tests/
+-rw-r--r--   0 cdent      (503) staff       (20)      138 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/__init__.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.429365 Paste-3.5.3/tests/cgiapp_data/
+-rwxr-xr-x   0 cdent      (503) staff       (20)       41 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/cgiapp_data/error.cgi
+-rwxr-xr-x   0 cdent      (503) staff       (20)     2039 2023-04-30 11:31:00.000000 Paste-3.5.3/tests/cgiapp_data/form.cgi
+-rwxr-xr-x   0 cdent      (503) staff       (20)      132 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/cgiapp_data/ok.cgi
+-rwxr-xr-x   0 cdent      (503) staff       (20)      223 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/cgiapp_data/stderr.cgi
+-rw-r--r--   0 cdent      (503) staff       (20)     4132 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/template.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.430689 Paste-3.5.3/tests/test_auth/
+-rw-r--r--   0 cdent      (503) staff       (20)        0 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_auth/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1527 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_auth/test_auth_cookie.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3077 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_auth/test_auth_digest.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3832 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_auth/test_auth_tkt.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2053 2020-10-12 12:27:11.000000 Paste-3.5.3/tests/test_cgiapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2249 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_cgitb_catcher.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2901 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_config.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1533 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_doctests.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3461 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_errordocument.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.432237 Paste-3.5.3/tests/test_exceptions/
+-rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_exceptions/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3389 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_exceptions/test_error_middleware.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4985 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_exceptions/test_formatter.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4055 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_exceptions/test_httpexceptions.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1280 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_exceptions/test_reporter.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9766 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_fileapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2489 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_fixture.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1264 2023-04-30 11:31:00.000000 Paste-3.5.3/tests/test_grantip.py
+-rw-r--r--   0 cdent      (503) staff       (20)      888 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_gzipper.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6505 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_httpheaders.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3447 2020-02-12 10:40:19.000000 Paste-3.5.3/tests/test_httpserver.py
+-rw-r--r--   0 cdent      (503) staff       (20)      477 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_import_string.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5255 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_multidict.py
+-rw-r--r--   0 cdent      (503) staff       (20)      721 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_profilemiddleware.py
+-rw-r--r--   0 cdent      (503) staff       (20)      624 2023-04-30 11:31:00.000000 Paste-3.5.3/tests/test_proxy.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4178 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_recursive.py
+-rw-r--r--   0 cdent      (503) staff       (20)    11149 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_registry.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2354 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_request.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1183 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_request_form.py
+-rw-r--r--   0 cdent      (503) staff       (20)      369 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_response.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1587 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_session.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1810 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_urlmap.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6944 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_urlparser.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.433448 Paste-3.5.3/tests/test_util/
+-rw-r--r--   0 cdent      (503) staff       (20)        0 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_util/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6026 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_util/test_datetimeutil.py
+-rw-r--r--   0 cdent      (503) staff       (20)    11873 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_util/test_mimeparse.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1171 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_util/test_quoting.py
+-rw-r--r--   0 cdent      (503) staff       (20)      842 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_wsgilib.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6441 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/test_wsgiwrappers.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.434120 Paste-3.5.3/tests/urlparser_data/
+-rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/__init__.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.434425 Paste-3.5.3/tests/urlparser_data/deep/
+-rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/deep/index.html
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.434721 Paste-3.5.3/tests/urlparser_data/deep/sub/
+-rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/deep/sub/Main.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.435675 Paste-3.5.3/tests/urlparser_data/find_file/
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.435992 Paste-3.5.3/tests/urlparser_data/find_file/dir with spaces/
+-rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/find_file/dir with spaces/test 4.html
+-rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/find_file/index.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/find_file/test 3.html
+-rw-r--r--   0 cdent      (503) staff       (20)        6 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/find_file/test2.html
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.436845 Paste-3.5.3/tests/urlparser_data/hook/
+-rw-r--r--   0 cdent      (503) staff       (20)      289 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/hook/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)      231 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/hook/app.py
+-rw-r--r--   0 cdent      (503) staff       (20)      232 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/hook/index.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.437134 Paste-3.5.3/tests/urlparser_data/not_found/
+-rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/not_found/__init__.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.437761 Paste-3.5.3/tests/urlparser_data/not_found/recur/
+-rw-r--r--   0 cdent      (503) staff       (20)      374 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/not_found/recur/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)        9 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/not_found/recur/isfound.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.438437 Paste-3.5.3/tests/urlparser_data/not_found/simple/
+-rw-r--r--   0 cdent      (503) staff       (20)      134 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/not_found/simple/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)        9 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/not_found/simple/found.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.438957 Paste-3.5.3/tests/urlparser_data/not_found/user/
+-rw-r--r--   0 cdent      (503) staff       (20)      411 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/not_found/user/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)      235 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/not_found/user/list.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.439794 Paste-3.5.3/tests/urlparser_data/python/
+-rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/python/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)      183 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/python/simpleapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)      208 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/python/stream.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-04-30 11:41:24.440325 Paste-3.5.3/tests/urlparser_data/python/sub/
+-rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/python/sub/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)      186 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/python/sub/simpleapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)        8 2020-01-26 15:30:37.000000 Paste-3.5.3/tests/urlparser_data/secured.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      362 2022-06-22 10:16:25.000000 Paste-3.5.3/tox.ini
```

### Comparing `Paste-3.5.2/PKG-INFO` & `Paste-3.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: Paste
-Version: 3.5.2
+Version: 3.5.3
 Summary: Tools for using a Web Server Gateway Interface stack
 Home-page: https://pythonpaste.readthedocs.io/
 Author: Chris Dent
 Author-email: chris.dent@gmail.com
 License: MIT
+Project-URL: Source, https://github.com/cdent/paste
+Project-URL: Bug Tracker, https://github.com/cdent/paste/issues
+Project-URL: Documentation, https://pythonpaste.readthedocs.io
 Keywords: web application server wsgi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
```

### Comparing `Paste-3.5.2/Paste.egg-info/PKG-INFO` & `Paste-3.5.3/Paste.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: Paste
-Version: 3.5.2
+Version: 3.5.3
 Summary: Tools for using a Web Server Gateway Interface stack
 Home-page: https://pythonpaste.readthedocs.io/
 Author: Chris Dent
 Author-email: chris.dent@gmail.com
 License: MIT
+Project-URL: Source, https://github.com/cdent/paste
+Project-URL: Bug Tracker, https://github.com/cdent/paste/issues
+Project-URL: Documentation, https://pythonpaste.readthedocs.io
 Keywords: web application server wsgi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
```

### Comparing `Paste-3.5.2/Paste.egg-info/SOURCES.txt` & `Paste-3.5.3/Paste.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/Paste.egg-info/entry_points.txt` & `Paste-3.5.3/Paste.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/README.rst` & `Paste-3.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/DeveloperGuidelines.txt` & `Paste-3.5.3/docs/DeveloperGuidelines.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/StyleGuide.txt` & `Paste-3.5.3/docs/StyleGuide.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/_static/default.css` & `Paste-3.5.3/docs/_static/default.css`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/community/index.txt` & `Paste-3.5.3/docs/community/index.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/community/mailing-list.txt` & `Paste-3.5.3/docs/community/mailing-list.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/conf.py` & `Paste-3.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/developer-features.txt` & `Paste-3.5.3/docs/developer-features.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/do-it-yourself-framework.txt` & `Paste-3.5.3/docs/do-it-yourself-framework.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/download/index.txt` & `Paste-3.5.3/docs/download/index.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/future.txt` & `Paste-3.5.3/docs/future.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/index.txt` & `Paste-3.5.3/docs/index.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/license.txt` & `Paste-3.5.3/docs/license.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/modules/exceptions.txt` & `Paste-3.5.3/docs/modules/exceptions.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/modules/fixture.txt` & `Paste-3.5.3/docs/modules/fixture.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/modules/httpexceptions.txt` & `Paste-3.5.3/docs/modules/httpexceptions.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/modules/wsgilib.txt` & `Paste-3.5.3/docs/modules/wsgilib.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/news.txt` & `Paste-3.5.3/docs/news.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 News
 ====
 
 .. contents::
 
+3.5.3
+-----
+
+* Use importlib instead of imp with Python 3.
+
+
 3.5.2
 -----
 
 * Additional fixes to next in iterators.
 
 Thanks to cjwatson.
```

### Comparing `Paste-3.5.2/docs/paste-httpserver-threadpool.txt` & `Paste-3.5.3/docs/paste-httpserver-threadpool.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/test_server.ini` & `Paste-3.5.3/docs/test_server.ini`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/testing-applications.txt` & `Paste-3.5.3/docs/testing-applications.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/url-parsing-with-wsgi.txt` & `Paste-3.5.3/docs/url-parsing-with-wsgi.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/web/default-site.css` & `Paste-3.5.3/docs/web/default-site.css`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/web/site.js` & `Paste-3.5.3/docs/web/site.js`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/docs/web/style.css` & `Paste-3.5.3/docs/web/style.css`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/__init__.py` & `Paste-3.5.3/paste/__init__.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/auth/auth_tkt.py` & `Paste-3.5.3/paste/auth/auth_tkt.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/auth/basic.py` & `Paste-3.5.3/paste/auth/basic.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/auth/cas.py` & `Paste-3.5.3/paste/auth/cas.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/auth/cookie.py` & `Paste-3.5.3/paste/auth/cookie.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/auth/digest.py` & `Paste-3.5.3/paste/auth/digest.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/auth/form.py` & `Paste-3.5.3/paste/auth/form.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/auth/grantip.py` & `Paste-3.5.3/paste/auth/grantip.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/auth/multi.py` & `Paste-3.5.3/paste/auth/multi.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/auth/open_id.py` & `Paste-3.5.3/paste/auth/open_id.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/cascade.py` & `Paste-3.5.3/paste/cascade.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/cgiapp.py` & `Paste-3.5.3/paste/cgiapp.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/cgitb_catcher.py` & `Paste-3.5.3/paste/cgitb_catcher.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/config.py` & `Paste-3.5.3/paste/config.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/cowbell/__init__.py` & `Paste-3.5.3/paste/cowbell/__init__.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/cowbell/bell-ascending.png` & `Paste-3.5.3/paste/cowbell/bell-ascending.png`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/cowbell/bell-descending.png` & `Paste-3.5.3/paste/cowbell/bell-descending.png`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/debug/debugapp.py` & `Paste-3.5.3/paste/debug/debugapp.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/debug/doctest_webapp.py` & `Paste-3.5.3/paste/debug/doctest_webapp.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/debug/fsdiff.py` & `Paste-3.5.3/paste/debug/fsdiff.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/debug/prints.py` & `Paste-3.5.3/paste/debug/prints.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/debug/profile.py` & `Paste-3.5.3/paste/debug/profile.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/debug/testserver.py` & `Paste-3.5.3/paste/debug/testserver.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/debug/watchthreads.py` & `Paste-3.5.3/paste/debug/watchthreads.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/debug/wdg_validate.py` & `Paste-3.5.3/paste/debug/wdg_validate.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/errordocument.py` & `Paste-3.5.3/paste/errordocument.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/evalexception/evalcontext.py` & `Paste-3.5.3/paste/evalexception/evalcontext.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/evalexception/media/MochiKit.packed.js` & `Paste-3.5.3/paste/evalexception/media/MochiKit.packed.js`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/evalexception/media/debug.js` & `Paste-3.5.3/paste/evalexception/media/debug.js`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/evalexception/middleware.py` & `Paste-3.5.3/paste/evalexception/middleware.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/exceptions/collector.py` & `Paste-3.5.3/paste/exceptions/collector.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/exceptions/errormiddleware.py` & `Paste-3.5.3/paste/exceptions/errormiddleware.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/exceptions/formatter.py` & `Paste-3.5.3/paste/exceptions/formatter.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/exceptions/reporter.py` & `Paste-3.5.3/paste/exceptions/reporter.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/exceptions/serial_number_generator.py` & `Paste-3.5.3/paste/exceptions/serial_number_generator.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/fileapp.py` & `Paste-3.5.3/paste/fileapp.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/fixture.py` & `Paste-3.5.3/paste/fixture.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/flup_session.py` & `Paste-3.5.3/paste/flup_session.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/gzipper.py` & `Paste-3.5.3/paste/gzipper.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/httpexceptions.py` & `Paste-3.5.3/paste/httpexceptions.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/httpheaders.py` & `Paste-3.5.3/paste/httpheaders.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/httpserver.py` & `Paste-3.5.3/paste/httpserver.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/lint.py` & `Paste-3.5.3/paste/lint.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/modpython.py` & `Paste-3.5.3/paste/modpython.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/pony.py` & `Paste-3.5.3/paste/pony.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/progress.py` & `Paste-3.5.3/paste/progress.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/proxy.py` & `Paste-3.5.3/paste/proxy.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/recursive.py` & `Paste-3.5.3/paste/recursive.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/registry.py` & `Paste-3.5.3/paste/registry.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/reloader.py` & `Paste-3.5.3/paste/reloader.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/request.py` & `Paste-3.5.3/paste/request.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/response.py` & `Paste-3.5.3/paste/response.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/session.py` & `Paste-3.5.3/paste/session.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/transaction.py` & `Paste-3.5.3/paste/transaction.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/translogger.py` & `Paste-3.5.3/paste/translogger.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/url.py` & `Paste-3.5.3/paste/url.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/urlmap.py` & `Paste-3.5.3/paste/urlmap.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/urlparser.py` & `Paste-3.5.3/paste/urlparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 """
 WSGI applications that parse the URL and dispatch to on-disk resources
 """
 
 import os
 import six
 import sys
-import imp
+
+if six.PY2:
+    import imp
+else:
+    import importlib.util as imputil
+
 import mimetypes
 try:
     import pkg_resources
 except ImportError:
     pkg_resources = None
 from paste import request
 from paste import fileapp
@@ -372,32 +377,42 @@
         except (OSError, IOError) as e:
             errors.write(
                 'Cannot write __init__.py file into directory %s (%s)\n'
                 % (os.path.dirname(filename), e))
             return None
         f.write('#\n')
         f.close()
-    fp = None
     if module_name in sys.modules:
         return sys.modules[module_name]
     if '.' in module_name:
         parent_name = '.'.join(module_name.split('.')[:-1])
         base_name = module_name.split('.')[-1]
         parent = load_module_from_name(environ, os.path.dirname(filename),
                                        parent_name, errors)
     else:
         base_name = module_name
-    fp = None
-    try:
-        fp, pathname, stuff = imp.find_module(
-            base_name, [os.path.dirname(filename)])
-        module = imp.load_module(module_name, fp, pathname, stuff)
-    finally:
-        if fp is not None:
-            fp.close()
+    module = None
+
+    if six.PY2:
+        fp = None
+        try:
+            fp, pathname, stuff = imp.find_module(
+                base_name, [os.path.dirname(filename)])
+            module = imp.load_module(module_name, fp, pathname, stuff)
+        finally:
+            if fp is not None:
+                fp.close()
+    else:
+        # imp is deprecated and will be removed in Python 3.12
+        spec = imputil.spec_from_file_location(base_name, filename)
+        if spec is not None:
+            module = imputil.module_from_spec(spec)
+            sys.modules[base_name] = module
+            spec.loader.exec_module(module)
+
     return module
 
 def make_py(parser, environ, filename):
     module = load_module(environ, filename)
     if not module:
         return None
     if hasattr(module, 'application') and module.application:
```

### Comparing `Paste-3.5.2/paste/util/PySourceColor.py` & `Paste-3.5.3/paste/util/PySourceColor.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/classinit.py` & `Paste-3.5.3/paste/util/classinit.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/classinstance.py` & `Paste-3.5.3/paste/util/classinstance.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/converters.py` & `Paste-3.5.3/paste/util/converters.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/dateinterval.py` & `Paste-3.5.3/paste/util/dateinterval.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/datetimeutil.py` & `Paste-3.5.3/paste/util/datetimeutil.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/filemixin.py` & `Paste-3.5.3/paste/util/filemixin.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/finddata.py` & `Paste-3.5.3/paste/util/finddata.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/findpackage.py` & `Paste-3.5.3/paste/util/findpackage.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/html.py` & `Paste-3.5.3/paste/util/html.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/import_string.py` & `Paste-3.5.3/paste/util/import_string.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/intset.py` & `Paste-3.5.3/paste/util/intset.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/ip4.py` & `Paste-3.5.3/paste/util/ip4.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/killthread.py` & `Paste-3.5.3/paste/util/killthread.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/looper.py` & `Paste-3.5.3/paste/util/looper.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/mimeparse.py` & `Paste-3.5.3/paste/util/mimeparse.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/multidict.py` & `Paste-3.5.3/paste/util/multidict.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/quoting.py` & `Paste-3.5.3/paste/util/quoting.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/scgiserver.py` & `Paste-3.5.3/paste/util/scgiserver.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/template.py` & `Paste-3.5.3/paste/util/template.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/threadedprint.py` & `Paste-3.5.3/paste/util/threadedprint.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/util/threadinglocal.py` & `Paste-3.5.3/paste/util/threadinglocal.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/wsgilib.py` & `Paste-3.5.3/paste/wsgilib.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/paste/wsgiwrappers.py` & `Paste-3.5.3/paste/wsgiwrappers.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/setup.py` & `Paste-3.5.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # - update changelog: docs/news.txt
 #
 # - git commit
 # - git tag -s VERSION
 # - git push
 # - python setup.py sdist bdist_wheel upload --sign
 
-__version__ = '3.5.2'
+__version__ = '3.5.3'
 
 from setuptools import setup, find_packages
 import sys, os
 sys.path.append(os.path.join(os.path.dirname(__file__),
                                 'paste', 'util'))
 import finddata
 
@@ -42,14 +42,19 @@
         "Topic :: Internet :: WWW/HTTP :: WSGI :: Server",
         "Framework :: Paste",
         ],
       keywords='web application server wsgi',
       author="Chris Dent",
       author_email="chris.dent@gmail.com",
       url="https://pythonpaste.readthedocs.io/",
+      project_urls={
+        "Source": "https://github.com/cdent/paste",
+        "Bug Tracker": "https://github.com/cdent/paste/issues",
+        "Documentation": "https://pythonpaste.readthedocs.io"
+      },
       license="MIT",
       packages=find_packages(exclude=['ez_setup', 'examples', 'packages', 'tests*']),
       package_data=finddata.find_package_data(
           exclude_directories=finddata.standard_exclude_directories + ('tests',)),
       namespace_packages=['paste'],
       zip_safe=False,
       install_requires=[
```

### Comparing `Paste-3.5.2/tests/cgiapp_data/form.cgi` & `Paste-3.5.3/tests/cgiapp_data/form.cgi`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 #!/usr/bin/env python
 
 from __future__ import print_function
 
+import sys
+
+# Quiet warnings in this CGI so that it does not upset tests.
+if not sys.warnoptions:
+    import warnings
+    warnings.simplefilter("ignore")
+
+# TODO: cgi is deprecated and will go away in Python 3.13.
 import cgi
-import six
 
 print('Content-type: text/plain')
 print('')
 
-if six.PY3:
+if sys.version_info.major >= 3:
     # Python 3: cgi.FieldStorage keeps some field names as unicode and some as
     # the repr() of byte strings, duh.
 
     class FieldStorage(cgi.FieldStorage):
 
         def _key_candidates(self, key):
             yield key
```

### Comparing `Paste-3.5.2/tests/template.txt` & `Paste-3.5.3/tests/template.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_auth/test_auth_cookie.py` & `Paste-3.5.3/tests/test_auth/test_auth_cookie.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_auth/test_auth_digest.py` & `Paste-3.5.3/tests/test_auth/test_auth_digest.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_auth/test_auth_tkt.py` & `Paste-3.5.3/tests/test_auth/test_auth_tkt.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_cgiapp.py` & `Paste-3.5.3/tests/test_cgiapp.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_cgitb_catcher.py` & `Paste-3.5.3/tests/test_cgitb_catcher.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_config.py` & `Paste-3.5.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_doctests.py` & `Paste-3.5.3/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_errordocument.py` & `Paste-3.5.3/tests/test_errordocument.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_exceptions/test_error_middleware.py` & `Paste-3.5.3/tests/test_exceptions/test_error_middleware.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_exceptions/test_formatter.py` & `Paste-3.5.3/tests/test_exceptions/test_formatter.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_exceptions/test_httpexceptions.py` & `Paste-3.5.3/tests/test_exceptions/test_httpexceptions.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_exceptions/test_reporter.py` & `Paste-3.5.3/tests/test_exceptions/test_reporter.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_fileapp.py` & `Paste-3.5.3/tests/test_fileapp.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_fixture.py` & `Paste-3.5.3/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_grantip.py` & `Paste-3.5.3/tests/test_grantip.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from paste.auth import grantip
 from paste.fixture import *
 
-def test_make_app():
+def _make_app():
     def application(environ, start_response):
         start_response('200 OK', [('content-type', 'text/plain')])
         lines = [
             str(environ.get('REMOTE_USER')),
             ':',
             str(environ.get('REMOTE_USER_TOKENS')),
             ]
@@ -19,15 +19,15 @@
         '192.168.0.8': ('__remove__', '-worker'),
         }
     app = grantip.GrantIPMiddleware(application, ip_map)
     app = TestApp(app)
     return app
 
 def test_req():
-    app = test_make_app()
+    app = _make_app()
     def doit(remote_addr):
         res = app.get('/', extra_environ={'REMOTE_ADDR': remote_addr})
         return res.body
     assert doit('127.0.0.1') == b'None:system'
     assert doit('192.168.15.12') == b'None:worker'
     assert doit('192.168.0.4') == b'None:worker'
     result = doit('192.168.0.5')
```

### Comparing `Paste-3.5.2/tests/test_gzipper.py` & `Paste-3.5.3/tests/test_gzipper.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_httpheaders.py` & `Paste-3.5.3/tests/test_httpheaders.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_httpserver.py` & `Paste-3.5.3/tests/test_httpserver.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_multidict.py` & `Paste-3.5.3/tests/test_multidict.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_profilemiddleware.py` & `Paste-3.5.3/tests/test_profilemiddleware.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_recursive.py` & `Paste-3.5.3/tests/test_recursive.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_registry.py` & `Paste-3.5.3/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_request.py` & `Paste-3.5.3/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_request_form.py` & `Paste-3.5.3/tests/test_request_form.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_session.py` & `Paste-3.5.3/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_urlmap.py` & `Paste-3.5.3/tests/test_urlmap.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_urlparser.py` & `Paste-3.5.3/tests/test_urlparser.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_util/test_datetimeutil.py` & `Paste-3.5.3/tests/test_util/test_datetimeutil.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_util/test_mimeparse.py` & `Paste-3.5.3/tests/test_util/test_mimeparse.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_util/test_quoting.py` & `Paste-3.5.3/tests/test_util/test_quoting.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_wsgilib.py` & `Paste-3.5.3/tests/test_wsgilib.py`

 * *Files identical despite different names*

### Comparing `Paste-3.5.2/tests/test_wsgiwrappers.py` & `Paste-3.5.3/tests/test_wsgiwrappers.py`

 * *Files identical despite different names*

