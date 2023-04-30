# Comparing `tmp/django_stats_middleware-0.2.tar.gz` & `tmp/django_stats_middleware-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_stats_middleware-0.2.tar", last modified: Wed Mar  2 04:11:52 2022, max compression
+gzip compressed data, was "django_stats_middleware-0.3.tar", last modified: Sun Apr 30 02:09:12 2023, max compression
```

## Comparing `django_stats_middleware-0.2.tar` & `django_stats_middleware-0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2022-03-02 04:11:52.325319 django_stats_middleware-0.2/
--rw-rw-r--   0 bernd     (1000) bernd     (1000)    15891 2021-10-14 11:18:17.000000 django_stats_middleware-0.2/LICENSE.md
--rw-rw-r--   0 bernd     (1000) bernd     (1000)     2206 2022-03-02 04:11:52.325319 django_stats_middleware-0.2/PKG-INFO
--rw-rw-r--   0 bernd     (1000) bernd     (1000)     1369 2022-02-12 10:50:49.000000 django_stats_middleware-0.2/README.md
--rw-rw-r--   0 bernd     (1000) bernd     (1000)      104 2021-10-14 10:42:04.000000 django_stats_middleware-0.2/pyproject.toml
--rw-rw-r--   0 bernd     (1000) bernd     (1000)      878 2022-03-02 04:11:52.325319 django_stats_middleware-0.2/setup.cfg
-drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2022-03-02 04:11:52.301319 django_stats_middleware-0.2/src/
-drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2022-03-02 04:11:52.325319 django_stats_middleware-0.2/src/django_stats_middleware/
--rw-r--r--   0 bernd     (1000) bernd     (1000)     3688 2022-02-12 11:27:45.000000 django_stats_middleware-0.2/src/django_stats_middleware/__init__.py
-drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2022-03-02 04:11:52.325319 django_stats_middleware-0.2/src/django_stats_middleware.egg-info/
--rw-rw-r--   0 bernd     (1000) bernd     (1000)     2206 2022-03-02 04:11:52.000000 django_stats_middleware-0.2/src/django_stats_middleware.egg-info/PKG-INFO
--rw-rw-r--   0 bernd     (1000) bernd     (1000)      289 2022-03-02 04:11:52.000000 django_stats_middleware-0.2/src/django_stats_middleware.egg-info/SOURCES.txt
--rw-rw-r--   0 bernd     (1000) bernd     (1000)        1 2022-03-02 04:11:52.000000 django_stats_middleware-0.2/src/django_stats_middleware.egg-info/dependency_links.txt
--rw-rw-r--   0 bernd     (1000) bernd     (1000)       24 2022-03-02 04:11:52.000000 django_stats_middleware-0.2/src/django_stats_middleware.egg-info/top_level.txt
+drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-30 02:09:12.221535 django_stats_middleware-0.3/
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)    15891 2021-10-14 11:18:17.000000 django_stats_middleware-0.3/LICENSE.md
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)     2566 2023-04-30 02:09:12.221535 django_stats_middleware-0.3/PKG-INFO
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)     1766 2023-04-30 02:08:18.000000 django_stats_middleware-0.3/README.md
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)      104 2021-10-14 10:42:04.000000 django_stats_middleware-0.3/pyproject.toml
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)      878 2023-04-30 02:09:12.221535 django_stats_middleware-0.3/setup.cfg
+drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-30 02:09:12.169535 django_stats_middleware-0.3/src/
+drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-30 02:09:12.217535 django_stats_middleware-0.3/src/django_stats_middleware/
+-rw-r--r--   0 bernd     (1000) bernd     (1000)     4212 2023-04-30 02:04:53.000000 django_stats_middleware-0.3/src/django_stats_middleware/__init__.py
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)      163 2023-04-30 01:55:15.000000 django_stats_middleware-0.3/src/django_stats_middleware/apps.py
+drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-30 02:09:12.221535 django_stats_middleware-0.3/src/django_stats_middleware.egg-info/
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)     2566 2023-04-30 02:09:12.000000 django_stats_middleware-0.3/src/django_stats_middleware.egg-info/PKG-INFO
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)      325 2023-04-30 02:09:12.000000 django_stats_middleware-0.3/src/django_stats_middleware.egg-info/SOURCES.txt
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)        1 2023-04-30 02:09:12.000000 django_stats_middleware-0.3/src/django_stats_middleware.egg-info/dependency_links.txt
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)       24 2023-04-30 02:09:12.000000 django_stats_middleware-0.3/src/django_stats_middleware.egg-info/top_level.txt
```

### Comparing `django_stats_middleware-0.2/LICENSE.md` & `django_stats_middleware-0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_stats_middleware-0.2/PKG-INFO` & `django_stats_middleware-0.3/src/django_stats_middleware.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
-Name: django_stats_middleware
-Version: 0.2
+Name: django-stats-middleware
+Version: 0.3
 Summary: Django Middleware for reporting very simple lightweight timing stats at end of ever page.
 Home-page: https://github.com/bernd-wechner/django-stats-middleware
 Author: Bernd Wechner
 Author-email: bwechner@yahoo.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/bernd-wechner/django-stats-middleware/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Django Stats Middleware
 
 [Django](https://www.djangoproject.com/) is one of the most popular Python web frameworks today.
 
-When a Django site seems slow, it's nice to put some real number to to that. The [Django Debug Toolbar](https://django-debug-toolbar.readthedocs.io/en/latest/) is the go-to middleware solution for diagnosing Django performance among other things, but it is rather large, and slow itself, adding significantly to the load time of your pages. So it's in a bit of catch 22 bind for simple performance overviews.
+When a Django site seems slow, it's nice to put some real number to to that. The [Django Debug Toolbar](https://django-debug-toolbar.readthedocs.io/en/latest/) is the go-to middleware solution for diagnosing Django performance among other things, but it is rather large, and slow itself, adding significantly to the load time of your pages. So it's in a bit of catch-22 bind for simple performance overviews.
 
 For that reason I wrote this tiny little lightweight piece of middleware that reports at the bottom of every page a single line reporting some basic timing stats. 
 
 - **Total Time**: The time from the request arriving to the response being delivered.
 - **Python Time**: Time spent running Python code
 - **DB Time**: Time spent waiting on database queries
 - **Number of Queries**: The number of database queries run
@@ -46,8 +44,24 @@
 MIDDLEWARE = (
     'django_stats_middleware.StatsMiddleware',
 	...
 ```
 
 That way Total Time will include the time spent in all other middleware as well as your site code.
 
+It includes some minimal CSS and to include that in your site include it as an app (so Django knows to collect static files from it):
+
+```python
+    INSTALLED_APPS += (
+        'django_stats_middleware',
+    )
+```
+
+and in your template load the CSS:
+
+```html
+    {% load static %}
+    <link rel="stylesheet" type="text/css" href="{% static 'django-stats-middleware/css/default.css' %}" />
+```
+
+
```

### Comparing `django_stats_middleware-0.2/README.md` & `django_stats_middleware-0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Django Stats Middleware
 
 [Django](https://www.djangoproject.com/) is one of the most popular Python web frameworks today.
 
-When a Django site seems slow, it's nice to put some real number to to that. The [Django Debug Toolbar](https://django-debug-toolbar.readthedocs.io/en/latest/) is the go-to middleware solution for diagnosing Django performance among other things, but it is rather large, and slow itself, adding significantly to the load time of your pages. So it's in a bit of catch 22 bind for simple performance overviews.
+When a Django site seems slow, it's nice to put some real number to to that. The [Django Debug Toolbar](https://django-debug-toolbar.readthedocs.io/en/latest/) is the go-to middleware solution for diagnosing Django performance among other things, but it is rather large, and slow itself, adding significantly to the load time of your pages. So it's in a bit of catch-22 bind for simple performance overviews.
 
 For that reason I wrote this tiny little lightweight piece of middleware that reports at the bottom of every page a single line reporting some basic timing stats. 
 
 - **Total Time**: The time from the request arriving to the response being delivered.
 - **Python Time**: Time spent running Python code
 - **DB Time**: Time spent waiting on database queries
 - **Number of Queries**: The number of database queries run
@@ -24,7 +24,25 @@
 ```python
 MIDDLEWARE = (
     'django_stats_middleware.StatsMiddleware',
 	...
 ```
 
 That way Total Time will include the time spent in all other middleware as well as your site code.
+
+It includes some minimal CSS and to include that in your site include it as an app (so Django knows to collect static files from it):
+
+```python
+    INSTALLED_APPS += (
+        'django_stats_middleware',
+    )
+```
+
+and in your template load the CSS:
+
+```html
+    {% load static %}
+    <link rel="stylesheet" type="text/css" href="{% static 'django-stats-middleware/css/default.css' %}" />
+```
+
+
+
```

### Comparing `django_stats_middleware-0.2/setup.cfg` & `django_stats_middleware-0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [metadata]
 name = django_stats_middleware
-version = 0.2
+version = 0.3
 author = Bernd Wechner
 author_email = bwechner@yahoo.com
 description = Django Middleware for reporting very simple lightweight timing stats at end of ever page.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/bernd-wechner/django-stats-middleware
 project_urls = 
 	Bug Tracker = https://github.com/bernd-wechner/django-stats-middleware/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Freely Distributable
 	Operating System :: OS Independent
 	Development Status :: 4 - Beta
-	Framework :: Django :: 3.2
+	Framework :: Django :: 4.0
 	Intended Audience :: System Administrators
 	Topic :: Internet :: WWW/HTTP :: HTTP Servers
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.7
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django_stats_middleware-0.2/src/django_stats_middleware/__init__.py` & `django_stats_middleware-0.3/src/django_stats_middleware/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,26 +4,37 @@
 Django Stats Middleware
 
 @author: Bernd Wechner, based on an old snippet here: https://code.djangoproject.com/wiki/PageStatsMiddleware
 @status: Beta - works and is in use on a dedicated project.
 
 Inserts some basic performance stats just prior to the </body> tag in the response of every page served.
 
-To use, add it to the MIDDLEWARE list in settings.py as follows:
+To use, add it to the MIDDLEWARE list in settings.py as follows (put it first to catch all times):
 
-MIDDLEWARE = (
-    'django_stats_middleware.StatsMiddleware',
-    'django.contrib.sessions.middleware.SessionMiddleware',
-    'django.middleware.common.CommonMiddleware',
-    'django.middleware.csrf.CsrfViewMiddleware',
-    'django.contrib.auth.middleware.AuthenticationMiddleware',
-    'django.contrib.messages.middleware.MessageMiddleware',
-    'django.middleware.clickjacking.XFrameOptionsMiddleware',
-    'django.middleware.security.SecurityMiddleware'
-)
+    MIDDLEWARE = (
+        'django_stats_middleware.StatsMiddleware',
+        'django.contrib.sessions.middleware.SessionMiddleware',
+        'django.middleware.common.CommonMiddleware',
+        'django.middleware.csrf.CsrfViewMiddleware',
+        'django.contrib.auth.middleware.AuthenticationMiddleware',
+        'django.contrib.messages.middleware.MessageMiddleware',
+        'django.middleware.clickjacking.XFrameOptionsMiddleware',
+        'django.middleware.security.SecurityMiddleware'
+    )
+
+It provided minimal default css also and for this it be incorporated in your site, add it as an app:
+
+    INSTALLED_APPS += (
+        'django_stats_middleware',
+    )
+
+and include the CSS with:
+
+    {% load static %}
+    <link rel="stylesheet" type="text/css" href="{% static 'django-stats-middleware/css/default.css' %}" />
 
 Can be easily tweaked below to deliver whatever stats you like.
 
 This information cannot be delivered to pages through the template context because timing information isn't
 collected until the whole template is already rendered. To wit, it is patched into the content just above
 the </body> tag. If your page has no such tag, stats won't appear on it of course.
 
@@ -70,21 +81,26 @@
                                    for q in connection.queries[n:]])
         else:
             db_time = 0.0
 
         # and backout python time
         python_time = total_time - db_time
 
-        stats = br''.join((br'<div id="stats" style="margin-top:1ex"><table><tr>'
-                           br'<td><b>STATS:</b></td>',
-                           br'<td style="padding-left: 5ch;">Total Time:</td><td>', "{:.1f} ms".format(total_time * 1000).encode(), br'</td>',
-                           br'<td style="padding-left: 5ch;">Python Time:</td><td>', "{:.1f} ms".format(python_time).encode(), br'</td>',
-                           br'<td style="padding-left: 5ch;">DB Time:</td><td>', "{:.1f} ms".format(db_time).encode(), br'</td>',
-                           br'<td style="padding-left: 5ch;">Number of Queries:</td><td>', "{:,}".format(db_queries).encode(), br'</td>',
-                           br'</tr></table></div>\1'))
+        div_class = "django_stats"
+        h1_class = "django_stats_heading1"
+        h2_class = "django_stats_heading2"
+        val_class = "django_stats_value"
+
+        stats = r''.join((fr'<div id="django_stats" class="{div_class}"><table><tr>'
+                          fr'<td class="{h1_class}"><b>STATS:</b></td>',
+                          fr'<td class="{h2_class}">Total Time:</td><td class="{val_class}">{total_time * 1000:.1f} ms</td>',
+                          fr'<td class="{h2_class}">Python Time:</td><td class="{val_class}">{python_time:.1f} ms</td>',
+                          fr'<td class="{h2_class}">DB Time:</td><td class="{val_class}">{db_time:.1f} ms</td>',
+                          fr'<td class="{h2_class}">Number of Queries:</td><td class="{val_class}">{db_queries:,}</td>',
+                          fr'</tr></table></div>\1'))
 
         # Insert the stats just prior to the body close tag (we need to update the Content-Length header or browser won't render it all.
         if response and getattr(response, 'content', False):
-            response.content = re.sub(br"(</body>)", stats, response.content, flags=re.RegexFlag.IGNORECASE)
+            response.content = re.sub(br"(</body>)", stats.encode(), response.content, flags=re.RegexFlag.IGNORECASE)
             response['Content-Length'] = str(len(response.content))
 
         return response
```

### Comparing `django_stats_middleware-0.2/src/django_stats_middleware.egg-info/PKG-INFO` & `django_stats_middleware-0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
-Name: django-stats-middleware
-Version: 0.2
+Name: django_stats_middleware
+Version: 0.3
 Summary: Django Middleware for reporting very simple lightweight timing stats at end of ever page.
 Home-page: https://github.com/bernd-wechner/django-stats-middleware
 Author: Bernd Wechner
 Author-email: bwechner@yahoo.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/bernd-wechner/django-stats-middleware/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Django Stats Middleware
 
 [Django](https://www.djangoproject.com/) is one of the most popular Python web frameworks today.
 
-When a Django site seems slow, it's nice to put some real number to to that. The [Django Debug Toolbar](https://django-debug-toolbar.readthedocs.io/en/latest/) is the go-to middleware solution for diagnosing Django performance among other things, but it is rather large, and slow itself, adding significantly to the load time of your pages. So it's in a bit of catch 22 bind for simple performance overviews.
+When a Django site seems slow, it's nice to put some real number to to that. The [Django Debug Toolbar](https://django-debug-toolbar.readthedocs.io/en/latest/) is the go-to middleware solution for diagnosing Django performance among other things, but it is rather large, and slow itself, adding significantly to the load time of your pages. So it's in a bit of catch-22 bind for simple performance overviews.
 
 For that reason I wrote this tiny little lightweight piece of middleware that reports at the bottom of every page a single line reporting some basic timing stats. 
 
 - **Total Time**: The time from the request arriving to the response being delivered.
 - **Python Time**: Time spent running Python code
 - **DB Time**: Time spent waiting on database queries
 - **Number of Queries**: The number of database queries run
@@ -46,8 +44,24 @@
 MIDDLEWARE = (
     'django_stats_middleware.StatsMiddleware',
 	...
 ```
 
 That way Total Time will include the time spent in all other middleware as well as your site code.
 
+It includes some minimal CSS and to include that in your site include it as an app (so Django knows to collect static files from it):
+
+```python
+    INSTALLED_APPS += (
+        'django_stats_middleware',
+    )
+```
+
+and in your template load the CSS:
+
+```html
+    {% load static %}
+    <link rel="stylesheet" type="text/css" href="{% static 'django-stats-middleware/css/default.css' %}" />
+```
+
+
```

