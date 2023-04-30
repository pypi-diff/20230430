# Comparing `tmp/feedwarrior-0.5.5.tar.gz` & `tmp/feedwarrior-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedwarrior-0.5.5.tar", last modified: Sun Apr 30 20:16:31 2023, max compression
+gzip compressed data, was "feedwarrior-0.5.6.tar", last modified: Sun Apr 30 20:42:42 2023, max compression
```

## Comparing `feedwarrior-0.5.5.tar` & `feedwarrior-0.5.6.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/
--rw-r--r--   0 lash      (1000) lash      (1000)    35149 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       33 2023-04-30 14:34:36.000000 feedwarrior-0.5.5/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      603 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)       45 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/README
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/feedwarrior/
--rw-r--r--   0 lash      (1000) lash      (1000)      140 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/feedwarrior/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/feedwarrior/adapters/
--rw-r--r--   0 lash      (1000) lash      (1000)       37 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/feedwarrior/adapters/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      906 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/feedwarrior/adapters/couchdbadapter.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2831 2022-12-29 12:22:34.000000 feedwarrior-0.5.5/feedwarrior/adapters/fileadapter.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/feedwarrior/cmd/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-12-29 07:52:30.000000 feedwarrior-0.5.5/feedwarrior/cmd/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2901 2023-04-30 19:56:14.000000 feedwarrior-0.5.5/feedwarrior/cmd/add.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1826 2022-12-29 12:06:53.000000 feedwarrior-0.5.5/feedwarrior/cmd/attach.py
--rw-r--r--   0 lash      (1000) lash      (1000)      790 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/feedwarrior/cmd/create.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1636 2023-04-30 19:56:27.000000 feedwarrior-0.5.5/feedwarrior/cmd/entry.py
--rw-r--r--   0 lash      (1000) lash      (1000)      369 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/feedwarrior/cmd/ls.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1787 2020-09-17 16:58:52.000000 feedwarrior-0.5.5/feedwarrior/cmd/show.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1112 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/feedwarrior/common.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1647 2022-01-12 21:12:45.000000 feedwarrior-0.5.5/feedwarrior/config.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3569 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/feedwarrior/entry.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3510 2020-09-17 17:04:04.000000 feedwarrior-0.5.5/feedwarrior/feed.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/feedwarrior/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     4236 2023-04-30 19:54:13.000000 feedwarrior-0.5.5/feedwarrior/runnable/main.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/feedwarrior.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      603 2023-04-30 20:16:31.000000 feedwarrior-0.5.5/feedwarrior.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      776 2023-04-30 20:16:31.000000 feedwarrior-0.5.5/feedwarrior.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-30 20:16:31.000000 feedwarrior-0.5.5/feedwarrior.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       63 2023-04-30 20:16:31.000000 feedwarrior-0.5.5/feedwarrior.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       68 2023-04-30 20:16:31.000000 feedwarrior-0.5.5/feedwarrior.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       12 2023-04-30 20:16:31.000000 feedwarrior-0.5.5/feedwarrior.egg-info/top_level.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/man/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/man/man1/
--rw-r--r--   0 lash      (1000) lash      (1000)     3259 2023-04-30 20:09:25.000000 feedwarrior-0.5.5/man/man1/feedwarrior.1
--rw-r--r--   0 lash      (1000) lash      (1000)       68 2022-12-29 09:12:30.000000 feedwarrior-0.5.5/requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/scripts/
--rw-r--r--   0 lash      (1000) lash      (1000)     3782 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/scripts/feedwarrior
--rw-r--r--   0 lash      (1000) lash      (1000)      583 2023-04-30 20:16:31.840170 feedwarrior-0.5.5/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      604 2023-04-30 14:34:25.000000 feedwarrior-0.5.5/setup.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/test/
--rw-r--r--   0 lash      (1000) lash      (1000)     1466 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/test/test_couchdb.py
--rw-r--r--   0 lash      (1000) lash      (1000)      984 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/test/test_file.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:42:42.199133 feedwarrior-0.5.6/
+-rw-r--r--   0 lash      (1000) lash      (1000)    35149 2020-09-17 16:47:49.000000 feedwarrior-0.5.6/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       41 2023-04-30 20:39:46.000000 feedwarrior-0.5.6/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)     4001 2023-04-30 20:42:42.199133 feedwarrior-0.5.6/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     3947 2023-04-30 20:23:41.000000 feedwarrior-0.5.6/README
+-rw-r--r--   0 lash      (1000) lash      (1000)     3357 2023-04-30 20:23:47.000000 feedwarrior-0.5.6/README.md
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:42:42.195799 feedwarrior-0.5.6/feedwarrior/
+-rw-r--r--   0 lash      (1000) lash      (1000)      140 2020-09-17 16:47:49.000000 feedwarrior-0.5.6/feedwarrior/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:42:42.195799 feedwarrior-0.5.6/feedwarrior/adapters/
+-rw-r--r--   0 lash      (1000) lash      (1000)       37 2020-09-17 16:47:49.000000 feedwarrior-0.5.6/feedwarrior/adapters/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      906 2020-09-17 16:47:49.000000 feedwarrior-0.5.6/feedwarrior/adapters/couchdbadapter.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2831 2022-12-29 12:22:34.000000 feedwarrior-0.5.6/feedwarrior/adapters/fileadapter.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:42:42.195799 feedwarrior-0.5.6/feedwarrior/cmd/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-12-29 07:52:30.000000 feedwarrior-0.5.6/feedwarrior/cmd/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2901 2023-04-30 19:56:14.000000 feedwarrior-0.5.6/feedwarrior/cmd/add.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1826 2022-12-29 12:06:53.000000 feedwarrior-0.5.6/feedwarrior/cmd/attach.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      790 2020-09-17 16:47:49.000000 feedwarrior-0.5.6/feedwarrior/cmd/create.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1636 2023-04-30 19:56:27.000000 feedwarrior-0.5.6/feedwarrior/cmd/entry.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      369 2020-09-17 16:47:49.000000 feedwarrior-0.5.6/feedwarrior/cmd/ls.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1787 2020-09-17 16:58:52.000000 feedwarrior-0.5.6/feedwarrior/cmd/show.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1112 2020-09-17 16:47:49.000000 feedwarrior-0.5.6/feedwarrior/common.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1647 2022-01-12 21:12:45.000000 feedwarrior-0.5.6/feedwarrior/config.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3569 2020-09-17 16:47:49.000000 feedwarrior-0.5.6/feedwarrior/entry.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3510 2020-09-17 17:04:04.000000 feedwarrior-0.5.6/feedwarrior/feed.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:42:42.195799 feedwarrior-0.5.6/feedwarrior/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     4236 2023-04-30 19:54:13.000000 feedwarrior-0.5.6/feedwarrior/runnable/main.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:42:42.195799 feedwarrior-0.5.6/feedwarrior.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)     4001 2023-04-30 20:42:42.000000 feedwarrior-0.5.6/feedwarrior.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      786 2023-04-30 20:42:42.000000 feedwarrior-0.5.6/feedwarrior.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-30 20:42:42.000000 feedwarrior-0.5.6/feedwarrior.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       63 2023-04-30 20:42:42.000000 feedwarrior-0.5.6/feedwarrior.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       68 2023-04-30 20:42:42.000000 feedwarrior-0.5.6/feedwarrior.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       12 2023-04-30 20:42:42.000000 feedwarrior-0.5.6/feedwarrior.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:42:42.195799 feedwarrior-0.5.6/man/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:42:42.195799 feedwarrior-0.5.6/man/man1/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3259 2023-04-30 20:09:25.000000 feedwarrior-0.5.6/man/man1/feedwarrior.1
+-rw-r--r--   0 lash      (1000) lash      (1000)       68 2022-12-29 09:12:30.000000 feedwarrior-0.5.6/requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:42:42.195799 feedwarrior-0.5.6/scripts/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3782 2020-09-17 16:47:49.000000 feedwarrior-0.5.6/scripts/feedwarrior
+-rw-r--r--   0 lash      (1000) lash      (1000)      583 2023-04-30 20:42:42.199133 feedwarrior-0.5.6/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      749 2023-04-30 20:39:28.000000 feedwarrior-0.5.6/setup.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:42:42.199133 feedwarrior-0.5.6/test/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1466 2020-09-17 16:47:49.000000 feedwarrior-0.5.6/test/test_couchdb.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      984 2020-09-17 16:47:49.000000 feedwarrior-0.5.6/test/test_file.py
```

### Comparing `feedwarrior-0.5.5/LICENSE` & `feedwarrior-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.5/feedwarrior/adapters/couchdbadapter.py` & `feedwarrior-0.5.6/feedwarrior/adapters/couchdbadapter.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.5/feedwarrior/adapters/fileadapter.py` & `feedwarrior-0.5.6/feedwarrior/adapters/fileadapter.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.5/feedwarrior/cmd/add.py` & `feedwarrior-0.5.6/feedwarrior/cmd/add.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.5/feedwarrior/cmd/attach.py` & `feedwarrior-0.5.6/feedwarrior/cmd/attach.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.5/feedwarrior/cmd/create.py` & `feedwarrior-0.5.6/feedwarrior/cmd/create.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.5/feedwarrior/cmd/entry.py` & `feedwarrior-0.5.6/feedwarrior/cmd/entry.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.5/feedwarrior/cmd/show.py` & `feedwarrior-0.5.6/feedwarrior/cmd/show.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.5/feedwarrior/common.py` & `feedwarrior-0.5.6/feedwarrior/common.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.5/feedwarrior/config.py` & `feedwarrior-0.5.6/feedwarrior/config.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.5/feedwarrior/entry.py` & `feedwarrior-0.5.6/feedwarrior/entry.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.5/feedwarrior/feed.py` & `feedwarrior-0.5.6/feedwarrior/feed.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.5/feedwarrior/runnable/main.py` & `feedwarrior-0.5.6/feedwarrior/runnable/main.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.5/feedwarrior.egg-info/SOURCES.txt` & `feedwarrior-0.5.6/feedwarrior.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README
+README.md
 requirements.txt
 setup.cfg
 setup.py
 feedwarrior/__init__.py
 feedwarrior/common.py
 feedwarrior/config.py
 feedwarrior/entry.py
```

### Comparing `feedwarrior-0.5.5/man/man1/feedwarrior.1` & `feedwarrior-0.5.6/man/man1/feedwarrior.1`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.5/scripts/feedwarrior` & `feedwarrior-0.5.6/scripts/feedwarrior`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.5/setup.cfg` & `feedwarrior-0.5.6/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = feedwarrior
-version = 0.5.5
+version = 0.5.6
 description = Feeds, warrior style
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://holbrook.no/src/feedwarrior/log.html
 keywords = 
 	feed
 	log
```

### Comparing `feedwarrior-0.5.5/setup.py` & `feedwarrior-0.5.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 while True:
     l = f.readline()
     if l == '':
         break
     requirements.append(l.rstrip())
 f.close()
 
+f = open('README.md', 'r')
+description = f.read()
+f.close()
 
 setup(
     packages=[
         'feedwarrior',
         'feedwarrior.cmd',
         'feedwarrior.adapters',
         'feedwarrior.runnable',
@@ -23,8 +26,10 @@
         ],
     entry_points = {
         'console_scripts': [
             'feedwarrior = feedwarrior.runnable.main:main',
             ],
         },
     data_files=[("man/man1", ["man/man1/feedwarrior.1"],)],
+    long_description=description,
+    long_description_content_type='text/markdown',
 )
```

### Comparing `feedwarrior-0.5.5/test/test_couchdb.py` & `feedwarrior-0.5.6/test/test_couchdb.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.5/test/test_file.py` & `feedwarrior-0.5.6/test/test_file.py`

 * *Files identical despite different names*

