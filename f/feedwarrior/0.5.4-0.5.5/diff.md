# Comparing `tmp/feedwarrior-0.5.4.tar.gz` & `tmp/feedwarrior-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedwarrior-0.5.4.tar", last modified: Sun Apr 30 07:25:27 2023, max compression
+gzip compressed data, was "feedwarrior-0.5.5.tar", last modified: Sun Apr 30 20:16:31 2023, max compression
```

## Comparing `feedwarrior-0.5.4.tar` & `feedwarrior-0.5.5.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 07:25:27.774288 feedwarrior-0.5.4/
--rw-r--r--   0 lash      (1000) lash      (1000)    35149 2020-09-17 16:47:49.000000 feedwarrior-0.5.4/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       26 2022-01-24 00:15:19.000000 feedwarrior-0.5.4/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      603 2023-04-30 07:25:27.774288 feedwarrior-0.5.4/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)       45 2020-09-17 16:47:49.000000 feedwarrior-0.5.4/README
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 07:25:27.770954 feedwarrior-0.5.4/feedwarrior/
--rw-r--r--   0 lash      (1000) lash      (1000)      140 2020-09-17 16:47:49.000000 feedwarrior-0.5.4/feedwarrior/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 07:25:27.774288 feedwarrior-0.5.4/feedwarrior/adapters/
--rw-r--r--   0 lash      (1000) lash      (1000)       37 2020-09-17 16:47:49.000000 feedwarrior-0.5.4/feedwarrior/adapters/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      906 2020-09-17 16:47:49.000000 feedwarrior-0.5.4/feedwarrior/adapters/couchdbadapter.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2831 2022-12-29 12:22:34.000000 feedwarrior-0.5.4/feedwarrior/adapters/fileadapter.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 07:25:27.774288 feedwarrior-0.5.4/feedwarrior/cmd/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-12-29 07:52:30.000000 feedwarrior-0.5.4/feedwarrior/cmd/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2874 2020-09-17 16:47:49.000000 feedwarrior-0.5.4/feedwarrior/cmd/add.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1826 2022-12-29 12:06:53.000000 feedwarrior-0.5.4/feedwarrior/cmd/attach.py
--rw-r--r--   0 lash      (1000) lash      (1000)      790 2020-09-17 16:47:49.000000 feedwarrior-0.5.4/feedwarrior/cmd/create.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1609 2020-09-17 16:47:49.000000 feedwarrior-0.5.4/feedwarrior/cmd/entry.py
--rw-r--r--   0 lash      (1000) lash      (1000)      369 2020-09-17 16:47:49.000000 feedwarrior-0.5.4/feedwarrior/cmd/ls.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1787 2020-09-17 16:58:52.000000 feedwarrior-0.5.4/feedwarrior/cmd/show.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1112 2020-09-17 16:47:49.000000 feedwarrior-0.5.4/feedwarrior/common.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1647 2022-01-12 21:12:45.000000 feedwarrior-0.5.4/feedwarrior/config.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3569 2020-09-17 16:47:49.000000 feedwarrior-0.5.4/feedwarrior/entry.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3510 2020-09-17 17:04:04.000000 feedwarrior-0.5.4/feedwarrior/feed.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 07:25:27.774288 feedwarrior-0.5.4/feedwarrior/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     4197 2022-12-29 08:41:46.000000 feedwarrior-0.5.4/feedwarrior/runnable/main.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 07:25:27.774288 feedwarrior-0.5.4/feedwarrior.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      603 2023-04-30 07:25:27.000000 feedwarrior-0.5.4/feedwarrior.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      753 2023-04-30 07:25:27.000000 feedwarrior-0.5.4/feedwarrior.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-30 07:25:27.000000 feedwarrior-0.5.4/feedwarrior.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       63 2023-04-30 07:25:27.000000 feedwarrior-0.5.4/feedwarrior.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       68 2023-04-30 07:25:27.000000 feedwarrior-0.5.4/feedwarrior.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       12 2023-04-30 07:25:27.000000 feedwarrior-0.5.4/feedwarrior.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       68 2022-12-29 09:12:30.000000 feedwarrior-0.5.4/requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 07:25:27.774288 feedwarrior-0.5.4/scripts/
--rw-r--r--   0 lash      (1000) lash      (1000)     3782 2020-09-17 16:47:49.000000 feedwarrior-0.5.4/scripts/feedwarrior
--rw-r--r--   0 lash      (1000) lash      (1000)      583 2023-04-30 07:25:27.774288 feedwarrior-0.5.4/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      544 2023-04-30 07:14:40.000000 feedwarrior-0.5.4/setup.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 07:25:27.774288 feedwarrior-0.5.4/test/
--rw-r--r--   0 lash      (1000) lash      (1000)     1466 2020-09-17 16:47:49.000000 feedwarrior-0.5.4/test/test_couchdb.py
--rw-r--r--   0 lash      (1000) lash      (1000)      984 2020-09-17 16:47:49.000000 feedwarrior-0.5.4/test/test_file.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/
+-rw-r--r--   0 lash      (1000) lash      (1000)    35149 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       33 2023-04-30 14:34:36.000000 feedwarrior-0.5.5/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      603 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)       45 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/README
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/feedwarrior/
+-rw-r--r--   0 lash      (1000) lash      (1000)      140 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/feedwarrior/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/feedwarrior/adapters/
+-rw-r--r--   0 lash      (1000) lash      (1000)       37 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/feedwarrior/adapters/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      906 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/feedwarrior/adapters/couchdbadapter.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2831 2022-12-29 12:22:34.000000 feedwarrior-0.5.5/feedwarrior/adapters/fileadapter.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/feedwarrior/cmd/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-12-29 07:52:30.000000 feedwarrior-0.5.5/feedwarrior/cmd/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2901 2023-04-30 19:56:14.000000 feedwarrior-0.5.5/feedwarrior/cmd/add.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1826 2022-12-29 12:06:53.000000 feedwarrior-0.5.5/feedwarrior/cmd/attach.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      790 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/feedwarrior/cmd/create.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1636 2023-04-30 19:56:27.000000 feedwarrior-0.5.5/feedwarrior/cmd/entry.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      369 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/feedwarrior/cmd/ls.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1787 2020-09-17 16:58:52.000000 feedwarrior-0.5.5/feedwarrior/cmd/show.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1112 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/feedwarrior/common.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1647 2022-01-12 21:12:45.000000 feedwarrior-0.5.5/feedwarrior/config.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3569 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/feedwarrior/entry.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3510 2020-09-17 17:04:04.000000 feedwarrior-0.5.5/feedwarrior/feed.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/feedwarrior/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     4236 2023-04-30 19:54:13.000000 feedwarrior-0.5.5/feedwarrior/runnable/main.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/feedwarrior.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      603 2023-04-30 20:16:31.000000 feedwarrior-0.5.5/feedwarrior.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      776 2023-04-30 20:16:31.000000 feedwarrior-0.5.5/feedwarrior.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-30 20:16:31.000000 feedwarrior-0.5.5/feedwarrior.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       63 2023-04-30 20:16:31.000000 feedwarrior-0.5.5/feedwarrior.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       68 2023-04-30 20:16:31.000000 feedwarrior-0.5.5/feedwarrior.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       12 2023-04-30 20:16:31.000000 feedwarrior-0.5.5/feedwarrior.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/man/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/man/man1/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3259 2023-04-30 20:09:25.000000 feedwarrior-0.5.5/man/man1/feedwarrior.1
+-rw-r--r--   0 lash      (1000) lash      (1000)       68 2022-12-29 09:12:30.000000 feedwarrior-0.5.5/requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/scripts/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3782 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/scripts/feedwarrior
+-rw-r--r--   0 lash      (1000) lash      (1000)      583 2023-04-30 20:16:31.840170 feedwarrior-0.5.5/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      604 2023-04-30 14:34:25.000000 feedwarrior-0.5.5/setup.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-30 20:16:31.836837 feedwarrior-0.5.5/test/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1466 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/test/test_couchdb.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      984 2020-09-17 16:47:49.000000 feedwarrior-0.5.5/test/test_file.py
```

### Comparing `feedwarrior-0.5.4/LICENSE` & `feedwarrior-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.4/PKG-INFO` & `feedwarrior-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedwarrior
-Version: 0.5.4
+Version: 0.5.5
 Summary: Feeds, warrior style
 Home-page: https://holbrook.no/src/feedwarrior/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPLv3+
 Keywords: feed,log,worklog
 Classifier: Programming Language :: Python :: 3
```

### Comparing `feedwarrior-0.5.4/feedwarrior/adapters/couchdbadapter.py` & `feedwarrior-0.5.5/feedwarrior/adapters/couchdbadapter.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.4/feedwarrior/adapters/fileadapter.py` & `feedwarrior-0.5.5/feedwarrior/adapters/fileadapter.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.4/feedwarrior/cmd/add.py` & `feedwarrior-0.5.5/feedwarrior/cmd/add.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,7 +88,8 @@
     uu = str(entry.uuid)
     logg.debug('adding entry {}'.format(uu))
     
     fa = fileadapter(config.data_dir, feed.uuid)
     fa.put(entry.uuid, entry, compress=args.z)
    
     feed.add(entry)
+    return str(entry.uuid)
```

### Comparing `feedwarrior-0.5.4/feedwarrior/cmd/attach.py` & `feedwarrior-0.5.5/feedwarrior/cmd/attach.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.4/feedwarrior/cmd/create.py` & `feedwarrior-0.5.5/feedwarrior/cmd/create.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.4/feedwarrior/cmd/entry.py` & `feedwarrior-0.5.5/feedwarrior/cmd/entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,7 +44,8 @@
     uu = str(entry.uuid)
     logg.debug('adding entry {}'.format(uu))
     
     fa = fileadapter(config.data_dir, feed.uuid)
     fa.put(entry.uuid, entry, compress=args.z)
    
     feed.add(entry)
+    return str(entry.uuid)
```

### Comparing `feedwarrior-0.5.4/feedwarrior/cmd/show.py` & `feedwarrior-0.5.5/feedwarrior/cmd/show.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.4/feedwarrior/common.py` & `feedwarrior-0.5.5/feedwarrior/common.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.4/feedwarrior/config.py` & `feedwarrior-0.5.5/feedwarrior/config.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.4/feedwarrior/entry.py` & `feedwarrior-0.5.5/feedwarrior/entry.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.4/feedwarrior/feed.py` & `feedwarrior-0.5.5/feedwarrior/feed.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.4/feedwarrior/runnable/main.py` & `feedwarrior-0.5.5/feedwarrior/runnable/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,12 +113,14 @@
         os.makedirs(config.feeds_dir, mode=0o777, exist_ok=False)
         os.makedirs(os.path.join(config.feeds_dir, 'names'), mode=0o777, exist_ok=False)
         logg.debug('creating datadir {}'.format(config.data_dir))
     except FileExistsError as e:
         logg.debug('found existing datadir {}'.format(config.data_dir))
 
     cmd_mod.check_args(args)
-    cmd_mod.execute(config, feed_current, args)
+    r = cmd_mod.execute(config, feed_current, args)
+    if r != None:
+        print(r)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `feedwarrior-0.5.4/feedwarrior.egg-info/PKG-INFO` & `feedwarrior-0.5.5/feedwarrior.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedwarrior
-Version: 0.5.4
+Version: 0.5.5
 Summary: Feeds, warrior style
 Home-page: https://holbrook.no/src/feedwarrior/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPLv3+
 Keywords: feed,log,worklog
 Classifier: Programming Language :: Python :: 3
```

### Comparing `feedwarrior-0.5.4/feedwarrior.egg-info/SOURCES.txt` & `feedwarrior-0.5.5/feedwarrior.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -22,10 +22,11 @@
 feedwarrior/cmd/add.py
 feedwarrior/cmd/attach.py
 feedwarrior/cmd/create.py
 feedwarrior/cmd/entry.py
 feedwarrior/cmd/ls.py
 feedwarrior/cmd/show.py
 feedwarrior/runnable/main.py
+man/man1/feedwarrior.1
 scripts/feedwarrior
 test/test_couchdb.py
 test/test_file.py
```

### Comparing `feedwarrior-0.5.4/scripts/feedwarrior` & `feedwarrior-0.5.5/scripts/feedwarrior`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.4/test/test_couchdb.py` & `feedwarrior-0.5.5/test/test_couchdb.py`

 * *Files identical despite different names*

### Comparing `feedwarrior-0.5.4/test/test_file.py` & `feedwarrior-0.5.5/test/test_file.py`

 * *Files identical despite different names*

