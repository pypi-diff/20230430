# Comparing `tmp/tootstagram-0.0.3.tar.gz` & `tmp/tootstagram-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tootstagram-0.0.3.tar", last modified: Sun Apr 30 17:55:11 2023, max compression
+gzip compressed data, was "tootstagram-0.0.4.tar", last modified: Sun Apr 30 18:02:39 2023, max compression
```

## Comparing `tootstagram-0.0.3.tar` & `tootstagram-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-04-30 17:55:11.543398 tootstagram-0.0.3/
--rw-rw-r--   0 gmc       (1000) gmc       (1000)    21387 2023-04-29 17:31:28.000000 tootstagram-0.0.3/LICENSE.md
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     2084 2023-04-30 17:55:11.543398 tootstagram-0.0.3/PKG-INFO
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     1513 2023-04-30 17:52:39.000000 tootstagram-0.0.3/README.md
--rw-rw-r--   0 gmc       (1000) gmc       (1000)      697 2023-04-30 17:54:57.000000 tootstagram-0.0.3/pyproject.toml
--rw-rw-r--   0 gmc       (1000) gmc       (1000)       38 2023-04-30 17:55:11.543398 tootstagram-0.0.3/setup.cfg
-drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-04-30 17:55:11.539398 tootstagram-0.0.3/tootstagram/
--rw-rw-r--   0 gmc       (1000) gmc       (1000)      243 2023-04-29 17:31:28.000000 tootstagram-0.0.3/tootstagram/__init__.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     1297 2023-04-30 17:30:14.000000 tootstagram-0.0.3/tootstagram/database.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     2339 2023-04-30 17:42:14.000000 tootstagram-0.0.3/tootstagram/instagram.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     2080 2023-04-30 17:48:18.000000 tootstagram-0.0.3/tootstagram/main.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     2219 2023-04-29 17:31:28.000000 tootstagram-0.0.3/tootstagram/mastodon.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)      459 2023-04-29 17:31:28.000000 tootstagram-0.0.3/tootstagram/utils.py
-drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-04-30 17:55:11.543398 tootstagram-0.0.3/tootstagram.egg-info/
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     2084 2023-04-30 17:55:11.000000 tootstagram-0.0.3/tootstagram.egg-info/PKG-INFO
--rw-rw-r--   0 gmc       (1000) gmc       (1000)      385 2023-04-30 17:55:11.000000 tootstagram-0.0.3/tootstagram.egg-info/SOURCES.txt
--rw-rw-r--   0 gmc       (1000) gmc       (1000)        1 2023-04-30 17:55:11.000000 tootstagram-0.0.3/tootstagram.egg-info/dependency_links.txt
--rw-rw-r--   0 gmc       (1000) gmc       (1000)       54 2023-04-30 17:55:11.000000 tootstagram-0.0.3/tootstagram.egg-info/entry_points.txt
--rw-rw-r--   0 gmc       (1000) gmc       (1000)       41 2023-04-30 17:55:11.000000 tootstagram-0.0.3/tootstagram.egg-info/requires.txt
--rw-rw-r--   0 gmc       (1000) gmc       (1000)       12 2023-04-30 17:55:11.000000 tootstagram-0.0.3/tootstagram.egg-info/top_level.txt
+drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-04-30 18:02:39.678214 tootstagram-0.0.4/
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)    21387 2023-04-29 17:31:28.000000 tootstagram-0.0.4/LICENSE.md
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2084 2023-04-30 18:02:39.678214 tootstagram-0.0.4/PKG-INFO
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     1513 2023-04-30 17:52:39.000000 tootstagram-0.0.4/README.md
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)      697 2023-04-30 18:02:30.000000 tootstagram-0.0.4/pyproject.toml
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)       38 2023-04-30 18:02:39.678214 tootstagram-0.0.4/setup.cfg
+drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-04-30 18:02:39.678214 tootstagram-0.0.4/tootstagram/
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)      243 2023-04-29 17:31:28.000000 tootstagram-0.0.4/tootstagram/__init__.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     1297 2023-04-30 17:30:14.000000 tootstagram-0.0.4/tootstagram/database.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2339 2023-04-30 17:42:14.000000 tootstagram-0.0.4/tootstagram/instagram.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2078 2023-04-30 18:01:40.000000 tootstagram-0.0.4/tootstagram/main.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2219 2023-04-29 17:31:28.000000 tootstagram-0.0.4/tootstagram/mastodon.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)      459 2023-04-29 17:31:28.000000 tootstagram-0.0.4/tootstagram/utils.py
+drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-04-30 18:02:39.678214 tootstagram-0.0.4/tootstagram.egg-info/
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2084 2023-04-30 18:02:39.000000 tootstagram-0.0.4/tootstagram.egg-info/PKG-INFO
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)      385 2023-04-30 18:02:39.000000 tootstagram-0.0.4/tootstagram.egg-info/SOURCES.txt
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)        1 2023-04-30 18:02:39.000000 tootstagram-0.0.4/tootstagram.egg-info/dependency_links.txt
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)       54 2023-04-30 18:02:39.000000 tootstagram-0.0.4/tootstagram.egg-info/entry_points.txt
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)       41 2023-04-30 18:02:39.000000 tootstagram-0.0.4/tootstagram.egg-info/requires.txt
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)       12 2023-04-30 18:02:39.000000 tootstagram-0.0.4/tootstagram.egg-info/top_level.txt
```

### Comparing `tootstagram-0.0.3/LICENSE.md` & `tootstagram-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tootstagram-0.0.3/PKG-INFO` & `tootstagram-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tootstagram
-Version: 0.0.3
+Version: 0.0.4
 Summary: Duplicate posted images from Mastodon to Instagram
 Author-email: Koen Martens <kmartens@sonologic.se>
 Project-URL: Homepage, https://cvs.sonologic.net/gmc/tootstagram
 Project-URL: Bug Tracker, https://cvs.sonologic.net/gmc/tootstagram/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tootstagram-0.0.3/README.md` & `tootstagram-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tootstagram-0.0.3/pyproject.toml` & `tootstagram-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tootstagram"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Koen Martens", email="kmartens@sonologic.se" },
 ]
 description = "Duplicate posted images from Mastodon to Instagram"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tootstagram-0.0.3/tootstagram/database.py` & `tootstagram-0.0.4/tootstagram/database.py`

 * *Files identical despite different names*

### Comparing `tootstagram-0.0.3/tootstagram/instagram.py` & `tootstagram-0.0.4/tootstagram/instagram.py`

 * *Files identical despite different names*

### Comparing `tootstagram-0.0.3/tootstagram/main.py` & `tootstagram-0.0.4/tootstagram/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,11 +45,11 @@
             config['instagram']['password'],
             os.path.join(Path.home(), '.tootstagram', 'session.json')
         )
         for toot in to_post:
             print(f"Processing toot {toot.id}:")
             for media in toot.media:
                 print(f"- downloading and posting image {media.url} to Instagram")
-                # instagram_client.post_image(media.url, toot.description, media.alt_text)
+                instagram_client.post_image(media.url, toot.description, media.alt_text)
                 database.add_processed(toot.id, media.url)
     else:
         print("No new posts found.")
```

### Comparing `tootstagram-0.0.3/tootstagram/mastodon.py` & `tootstagram-0.0.4/tootstagram/mastodon.py`

 * *Files identical despite different names*

### Comparing `tootstagram-0.0.3/tootstagram.egg-info/PKG-INFO` & `tootstagram-0.0.4/tootstagram.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tootstagram
-Version: 0.0.3
+Version: 0.0.4
 Summary: Duplicate posted images from Mastodon to Instagram
 Author-email: Koen Martens <kmartens@sonologic.se>
 Project-URL: Homepage, https://cvs.sonologic.net/gmc/tootstagram
 Project-URL: Bug Tracker, https://cvs.sonologic.net/gmc/tootstagram/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
```

