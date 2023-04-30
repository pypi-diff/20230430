# Comparing `tmp/Flask-Session-0.4.0.tar.gz` & `tmp/Flask-Session-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-Session-0.4.0.tar", last modified: Thu Jun 24 10:02:41 2021, max compression
+gzip compressed data, was "Flask-Session-0.4.1.tar", last modified: Sun Apr 30 05:18:57 2023, max compression
```

## Comparing `Flask-Session-0.4.0.tar` & `Flask-Session-0.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 fsp        (501) staff       (20)        0 2021-06-24 10:02:41.135783 Flask-Session-0.4.0/
--rw-r--r--   0 fsp        (501) staff       (20)     1146 2021-06-24 09:48:27.000000 Flask-Session-0.4.0/CHANGES
-drwxr-xr-x   0 fsp        (501) staff       (20)        0 2021-06-24 10:02:41.127590 Flask-Session-0.4.0/Flask_Session.egg-info/
--rw-r--r--   0 fsp        (501) staff       (20)      986 2021-06-24 10:02:40.000000 Flask-Session-0.4.0/Flask_Session.egg-info/PKG-INFO
--rw-r--r--   0 fsp        (501) staff       (20)      431 2021-06-24 10:02:40.000000 Flask-Session-0.4.0/Flask_Session.egg-info/SOURCES.txt
--rw-r--r--   0 fsp        (501) staff       (20)        1 2021-06-24 10:02:40.000000 Flask-Session-0.4.0/Flask_Session.egg-info/dependency_links.txt
--rw-r--r--   0 fsp        (501) staff       (20)        1 2015-03-19 12:14:02.000000 Flask-Session-0.4.0/Flask_Session.egg-info/not-zip-safe
--rw-r--r--   0 fsp        (501) staff       (20)       20 2021-06-24 10:02:40.000000 Flask-Session-0.4.0/Flask_Session.egg-info/requires.txt
--rw-r--r--   0 fsp        (501) staff       (20)       14 2021-06-24 10:02:40.000000 Flask-Session-0.4.0/Flask_Session.egg-info/top_level.txt
--rw-r--r--   0 fsp        (501) staff       (20)     1455 2015-03-19 07:23:57.000000 Flask-Session-0.4.0/LICENSE
--rw-r--r--   0 fsp        (501) staff       (20)      154 2015-03-19 07:23:57.000000 Flask-Session-0.4.0/MANIFEST.in
--rw-r--r--   0 fsp        (501) staff       (20)      986 2021-06-24 10:02:41.136089 Flask-Session-0.4.0/PKG-INFO
--rw-r--r--   0 fsp        (501) staff       (20)      132 2015-03-19 07:23:57.000000 Flask-Session-0.4.0/README.md
-drwxr-xr-x   0 fsp        (501) staff       (20)        0 2021-06-24 10:02:41.131434 Flask-Session-0.4.0/docs/
--rw-r--r--   0 fsp        (501) staff       (20)     6790 2015-03-19 07:23:57.000000 Flask-Session-0.4.0/docs/Makefile
-drwxr-xr-x   0 fsp        (501) staff       (20)        0 2021-06-24 10:02:41.132684 Flask-Session-0.4.0/docs/_static/
--rw-r--r--   0 fsp        (501) staff       (20)     4987 2015-03-19 07:23:57.000000 Flask-Session-0.4.0/docs/_static/flask-session.png
--rw-r--r--   0 fsp        (501) staff       (20)     8934 2020-05-14 06:55:28.000000 Flask-Session-0.4.0/docs/conf.py
--rw-r--r--   0 fsp        (501) staff       (20)     9517 2020-05-14 07:30:30.000000 Flask-Session-0.4.0/docs/index.rst
--rw-r--r--   0 fsp        (501) staff       (20)     6715 2015-03-19 07:23:57.000000 Flask-Session-0.4.0/docs/make.bat
-drwxr-xr-x   0 fsp        (501) staff       (20)        0 2021-06-24 10:02:41.134535 Flask-Session-0.4.0/flask_session/
--rw-r--r--   0 fsp        (501) staff       (20)     4223 2021-06-24 09:47:15.000000 Flask-Session-0.4.0/flask_session/__init__.py
--rw-r--r--   0 fsp        (501) staff       (20)    22431 2021-06-24 09:43:09.000000 Flask-Session-0.4.0/flask_session/sessions.py
--rw-r--r--   0 fsp        (501) staff       (20)       61 2021-06-24 10:02:41.137304 Flask-Session-0.4.0/setup.cfg
--rw-r--r--   0 fsp        (501) staff       (20)     1171 2021-06-24 09:47:33.000000 Flask-Session-0.4.0/setup.py
--rw-r--r--   0 fsp        (501) staff       (20)     6365 2017-02-09 05:39:08.000000 Flask-Session-0.4.0/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 05:18:57.243419 Flask-Session-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/CHANGES
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 05:18:57.243419 Flask-Session-0.4.1/Flask_Session.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-30 05:18:57.000000 Flask-Session-0.4.1/Flask_Session.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-30 05:18:57.000000 Flask-Session-0.4.1/Flask_Session.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 05:18:57.000000 Flask-Session-0.4.1/Flask_Session.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 05:18:57.000000 Flask-Session-0.4.1/Flask_Session.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-30 05:18:57.000000 Flask-Session-0.4.1/Flask_Session.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-30 05:18:57.000000 Flask-Session-0.4.1/Flask_Session.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-30 05:18:57.243419 Flask-Session-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 05:18:57.243419 Flask-Session-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 05:18:57.243419 Flask-Session-0.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/docs/_static/flask-session.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 05:18:57.243419 Flask-Session-0.4.1/flask_session/
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/flask_session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22431 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/flask_session/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-30 05:18:57.243419 Flask-Session-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/test_session.py
```

### Comparing `Flask-Session-0.4.0/CHANGES` & `Flask-Session-0.4.1/CHANGES`

 * *Files identical despite different names*

### Comparing `Flask-Session-0.4.0/Flask_Session.egg-info/PKG-INFO` & `Flask-Session-0.4.1/Flask_Session.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: Flask-Session
-Version: 0.4.0
+Version: 0.4.1
 Summary: Adds server-side session support to your Flask application
 Home-page: https://github.com/fengsp/flask-session
 Author: Shipeng Feng
 Author-email: fsp261@gmail.com
 License: BSD
-Description: 
-        Flask-Session
-        -------------
-        
-        Flask-Session is an extension for Flask that adds support for
-        Server-side Session to your application.
-        
-        Links
-        `````
-        
-        * `development version
-          <https://github.com/fengsp/flask-session/zipball/master#egg=Flask-dev>`_
-        
-        
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+
+
+Flask-Session
+-------------
+
+Flask-Session is an extension for Flask that adds support for
+Server-side Session to your application.
+
+Links
+`````
+
+* `development version
+  <https://github.com/fengsp/flask-session/zipball/master#egg=Flask-dev>`_
+
```

### Comparing `Flask-Session-0.4.0/LICENSE` & `Flask-Session-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Session-0.4.0/PKG-INFO` & `Flask-Session-0.4.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: Flask-Session
-Version: 0.4.0
+Version: 0.4.1
 Summary: Adds server-side session support to your Flask application
 Home-page: https://github.com/fengsp/flask-session
 Author: Shipeng Feng
 Author-email: fsp261@gmail.com
 License: BSD
-Description: 
-        Flask-Session
-        -------------
-        
-        Flask-Session is an extension for Flask that adds support for
-        Server-side Session to your application.
-        
-        Links
-        `````
-        
-        * `development version
-          <https://github.com/fengsp/flask-session/zipball/master#egg=Flask-dev>`_
-        
-        
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+
+
+Flask-Session
+-------------
+
+Flask-Session is an extension for Flask that adds support for
+Server-side Session to your application.
+
+Links
+`````
+
+* `development version
+  <https://github.com/fengsp/flask-session/zipball/master#egg=Flask-dev>`_
+
```

### Comparing `Flask-Session-0.4.0/docs/Makefile` & `Flask-Session-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-Session-0.4.0/docs/_static/flask-session.png` & `Flask-Session-0.4.1/docs/_static/flask-session.png`

 * *Files identical despite different names*

### Comparing `Flask-Session-0.4.0/docs/conf.py` & `Flask-Session-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-Session-0.4.0/docs/index.rst` & `Flask-Session-0.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Flask-Session-0.4.0/docs/make.bat` & `Flask-Session-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-Session-0.4.0/flask_session/__init__.py` & `Flask-Session-0.4.1/flask_session/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
     Adds server session support to your application.
 
     :copyright: (c) 2014 by Shipeng Feng.
     :license: BSD, see LICENSE for more details.
 """
 
-__version__ = '0.4.0'
+__version__ = '0.4.1'
 
 import os
 
 from .sessions import NullSessionInterface, RedisSessionInterface, \
     MemcachedSessionInterface, FileSystemSessionInterface, \
     MongoDBSessionInterface, SqlAlchemySessionInterface
```

### Comparing `Flask-Session-0.4.0/flask_session/sessions.py` & `Flask-Session-0.4.1/flask_session/sessions.py`

 * *Files identical despite different names*

### Comparing `Flask-Session-0.4.0/setup.py` & `Flask-Session-0.4.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,32 +8,38 @@
 Links
 `````
 
 * `development version
   <https://github.com/fengsp/flask-session/zipball/master#egg=Flask-dev>`_
 
 """
+import re, io
 from setuptools import setup
 
+# setup.py shall not import main package
+__version__ = re.search(
+    r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]',  # It excludes inline comment too
+    io.open('flask_session/__init__.py', encoding='utf_8_sig').read()
+    ).group(1)
 
 setup(
     name='Flask-Session',
-    version='0.4.0',
+    version=__version__,
     url='https://github.com/fengsp/flask-session',
     license='BSD',
     author='Shipeng Feng',
     author_email='fsp261@gmail.com',
     description='Adds server-side session support to your Flask application',
     long_description=__doc__,
     packages=['flask_session'],
     zip_safe=False,
     include_package_data=True,
     platforms='any',
     install_requires=[
-        'Flask>=0.8',
+        'Flask>=0.8,<2.3',  # Flask 2.3 removed app.session_cookie_name
         'cachelib'
     ],
     test_suite='test_session',
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
```

### Comparing `Flask-Session-0.4.0/test_session.py` & `Flask-Session-0.4.1/test_session.py`

 * *Files identical despite different names*

