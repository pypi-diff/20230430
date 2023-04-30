# Comparing `tmp/tootstagram-0.0.2.tar.gz` & `tmp/tootstagram-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tootstagram-0.0.2.tar", last modified: Thu Apr 27 11:30:19 2023, max compression
+gzip compressed data, was "tootstagram-0.0.3.tar", last modified: Sun Apr 30 17:55:11 2023, max compression
```

## Comparing `tootstagram-0.0.2.tar` & `tootstagram-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-04-27 11:30:19.755646 tootstagram-0.0.2/
--rw-rw-r--   0 gmc       (1000) gmc       (1000)    21387 2023-04-26 13:26:59.000000 tootstagram-0.0.2/LICENSE.md
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     1705 2023-04-27 11:30:19.755646 tootstagram-0.0.2/PKG-INFO
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     1134 2023-04-27 06:55:29.000000 tootstagram-0.0.2/README.md
--rw-rw-r--   0 gmc       (1000) gmc       (1000)      697 2023-04-27 11:29:54.000000 tootstagram-0.0.2/pyproject.toml
--rw-rw-r--   0 gmc       (1000) gmc       (1000)       38 2023-04-27 11:30:19.755646 tootstagram-0.0.2/setup.cfg
-drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-04-27 11:30:19.755646 tootstagram-0.0.2/tootstagram/
--rw-rw-r--   0 gmc       (1000) gmc       (1000)      243 2023-04-27 06:40:20.000000 tootstagram-0.0.2/tootstagram/__init__.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     1454 2023-04-27 06:40:20.000000 tootstagram-0.0.2/tootstagram/database.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     1119 2023-04-27 11:27:52.000000 tootstagram-0.0.2/tootstagram/instagram.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     1778 2023-04-27 11:28:09.000000 tootstagram-0.0.2/tootstagram/main.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     2219 2023-04-27 11:25:42.000000 tootstagram-0.0.2/tootstagram/mastodon.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)      459 2023-04-27 06:40:20.000000 tootstagram-0.0.2/tootstagram/utils.py
-drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-04-27 11:30:19.755646 tootstagram-0.0.2/tootstagram.egg-info/
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     1705 2023-04-27 11:30:19.000000 tootstagram-0.0.2/tootstagram.egg-info/PKG-INFO
--rw-rw-r--   0 gmc       (1000) gmc       (1000)      385 2023-04-27 11:30:19.000000 tootstagram-0.0.2/tootstagram.egg-info/SOURCES.txt
--rw-rw-r--   0 gmc       (1000) gmc       (1000)        1 2023-04-27 11:30:19.000000 tootstagram-0.0.2/tootstagram.egg-info/dependency_links.txt
--rw-rw-r--   0 gmc       (1000) gmc       (1000)       54 2023-04-27 11:30:19.000000 tootstagram-0.0.2/tootstagram.egg-info/entry_points.txt
--rw-rw-r--   0 gmc       (1000) gmc       (1000)       41 2023-04-27 11:30:19.000000 tootstagram-0.0.2/tootstagram.egg-info/requires.txt
--rw-rw-r--   0 gmc       (1000) gmc       (1000)       12 2023-04-27 11:30:19.000000 tootstagram-0.0.2/tootstagram.egg-info/top_level.txt
+drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-04-30 17:55:11.543398 tootstagram-0.0.3/
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)    21387 2023-04-29 17:31:28.000000 tootstagram-0.0.3/LICENSE.md
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2084 2023-04-30 17:55:11.543398 tootstagram-0.0.3/PKG-INFO
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     1513 2023-04-30 17:52:39.000000 tootstagram-0.0.3/README.md
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)      697 2023-04-30 17:54:57.000000 tootstagram-0.0.3/pyproject.toml
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)       38 2023-04-30 17:55:11.543398 tootstagram-0.0.3/setup.cfg
+drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-04-30 17:55:11.539398 tootstagram-0.0.3/tootstagram/
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)      243 2023-04-29 17:31:28.000000 tootstagram-0.0.3/tootstagram/__init__.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     1297 2023-04-30 17:30:14.000000 tootstagram-0.0.3/tootstagram/database.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2339 2023-04-30 17:42:14.000000 tootstagram-0.0.3/tootstagram/instagram.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2080 2023-04-30 17:48:18.000000 tootstagram-0.0.3/tootstagram/main.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2219 2023-04-29 17:31:28.000000 tootstagram-0.0.3/tootstagram/mastodon.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)      459 2023-04-29 17:31:28.000000 tootstagram-0.0.3/tootstagram/utils.py
+drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-04-30 17:55:11.543398 tootstagram-0.0.3/tootstagram.egg-info/
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2084 2023-04-30 17:55:11.000000 tootstagram-0.0.3/tootstagram.egg-info/PKG-INFO
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)      385 2023-04-30 17:55:11.000000 tootstagram-0.0.3/tootstagram.egg-info/SOURCES.txt
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)        1 2023-04-30 17:55:11.000000 tootstagram-0.0.3/tootstagram.egg-info/dependency_links.txt
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)       54 2023-04-30 17:55:11.000000 tootstagram-0.0.3/tootstagram.egg-info/entry_points.txt
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)       41 2023-04-30 17:55:11.000000 tootstagram-0.0.3/tootstagram.egg-info/requires.txt
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)       12 2023-04-30 17:55:11.000000 tootstagram-0.0.3/tootstagram.egg-info/top_level.txt
```

### Comparing `tootstagram-0.0.2/LICENSE.md` & `tootstagram-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tootstagram-0.0.2/PKG-INFO` & `tootstagram-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: tootstagram
-Version: 0.0.2
-Summary: Duplicate posted images from Mastodon to Instagram
-Author-email: Koen Martens <kmartens@sonologic.se>
-Project-URL: Homepage, https://cvs.sonologic.net/gmc/tootstagram
-Project-URL: Bug Tracker, https://cvs.sonologic.net/gmc/tootstagram/-/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # Tootstagram
 
 https://cvs.sonologic.net/gmc/tootstagram
 
 ## Installation
 
 ```
@@ -40,17 +25,30 @@
 ```
 tootstagram
 ```
 
 This will fetch the feed from the Mastodon account and post any
 images that were not already posted to the Instagram account.
 
+## Security
+
+Make sure you keep the configuration file as well as the `.tootstagram`
+directory in your home or user dir private. The configuration file 
+contains your instagram username and password, and the `.tootstagram`
+directory contains a file `session.json` which should be treated as
+equivalent to your username and password.
+
 ## Limitations
 
 * Only posts toots with images, not videos (I don't do videos myself)
 * Any html tags in the toot are crudely removed by a simple regexp
 * If a toot has multiple images, but not all have alt text, none of the
   instagram posts will have alt text (because it is impossible to derive
   from the feed which alt text belongs to which image)
 * Editing a toot will not alter on or repost to instagram
 * Only posts listed toots, as those are the only ones available from the
   feed
+
+## Planned features
+
+* Hashtag translation
+
```

### Comparing `tootstagram-0.0.2/pyproject.toml` & `tootstagram-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tootstagram"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Koen Martens", email="kmartens@sonologic.se" },
 ]
 description = "Duplicate posted images from Mastodon to Instagram"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tootstagram-0.0.2/tootstagram/database.py` & `tootstagram-0.0.3/tootstagram/database.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,18 +9,16 @@
 """
 import os
 import sqlite3
 from pathlib import Path
 
 
 class Database:
-    def __init__(self) -> None:
-        if not os.path.isdir(os.path.join(Path.home(), '.tootstagram')):
-            os.mkdir(os.path.join(Path.home(), '.tootstagram'))
-        self._database_path = os.path.join(Path.home(), '.tootstagram', 'toots.db')
+    def __init__(self, database_path: str) -> None:
+        self._database_path = database_path
         self._connection = sqlite3.connect(self._database_path)
         self._create_table_if_needed()
 
     def _create_table_if_needed(self) -> None:
         cursor = self._connection.cursor()
         result = cursor.execute("SELECT name FROM sqlite_master WHERE name='processed'")
         if not result.fetchone():
```

### Comparing `tootstagram-0.0.2/tootstagram/instagram.py` & `tootstagram-0.0.3/tootstagram/instagram.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,22 +7,51 @@
 https://firstdonoharm.dev/version/3/0/bds-cl-eco-extr-ffd-media-my-soc-sv-tal-xuar.md
 
 """
 import os
 from tempfile import TemporaryDirectory
 
 import instagrapi
+from instagrapi.exceptions import LoginRequired
 
 from tootstagram.utils import download_file
 
 
 class InstagramClient:
-    def __init__(self, username: str, password: str) -> None:
+    def __init__(self, username: str, password: str, session_file_path: str) -> None:
         self._client = instagrapi.Client()
-        self._client.login(username, password)
+        self._client.delay_range = [1, 3]
+        self._session_file_path = session_file_path
+        self._username = username
+        self._password = password
+        self._authenticate()
+
+    def _authenticate(self) -> None:
+        if os.path.isfile(self._session_file_path):
+            session = self._client.load_settings(self._session_file_path)
+            self._client.set_settings(session)
+            self._client.login(self._username, self._password)
+            if not self._client_logged_in:
+                print("Invalid session, logging in with username and password")
+                old_session = self._client.get_timeline_feed()
+                self._client.set_settings({})
+                self._client.set_uuids(old_session['uuids'])
+        else:
+            self._client.login(self._username, self._password)
+        if not self._client_logged_in:
+            raise RuntimeError("Unable to authenticate with instagram")
+        self._client.dump_settings(self._session_file_path)
+
+    @property
+    def _client_logged_in(self) -> bool:
+        try:
+            self._client.get_timeline_feed()
+        except LoginRequired:
+            return False
+        return True
 
     def post_image(self, image_url: str, description: str, alt_text: str) -> None:
         extra_data = {}
         if alt_text:
             extra_data['custom_accessibility_caption'] = alt_text
 
         extension = os.path.splitext(os.path.basename(image_url))[1][1:]
```

### Comparing `tootstagram-0.0.2/tootstagram/main.py` & `tootstagram-0.0.3/tootstagram/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -28,22 +28,28 @@
     if os.path.isfile(os.path.join(os.getcwd(), CONFIG_FILENAME)):
         return os.path.join(os.getcwd(), CONFIG_FILENAME)
     raise RuntimeError("No configuration file found.")
 
 
 def main() -> None:
     config = toml.load(config_finder())
-    database = Database()
+    if not os.path.isdir(os.path.join(Path.home(), '.tootstagram')):
+        os.mkdir(os.path.join(Path.home(), '.tootstagram'), mode=0o700)
+    database = Database(os.path.join(Path.home(), '.tootstagram', 'toots.db'))
     mastodon_client = MastodonClient(config['mastodon']['account'], database)
     print("Fetching Mastodon feed.")
     to_post = mastodon_client.get_images()
     if to_post:
         print("Log in to Instagram")
-        instagram_client = InstagramClient(config['instagram']['username'], config['instagram']['password'])
+        instagram_client = InstagramClient(
+            config['instagram']['username'],
+            config['instagram']['password'],
+            os.path.join(Path.home(), '.tootstagram', 'session.json')
+        )
         for toot in to_post:
             print(f"Processing toot {toot.id}:")
             for media in toot.media:
                 print(f"- downloading and posting image {media.url} to Instagram")
-                instagram_client.post_image(media.url, toot.description, media.alt_text)
+                # instagram_client.post_image(media.url, toot.description, media.alt_text)
                 database.add_processed(toot.id, media.url)
     else:
-        print("No new posts found.")
+        print("No new posts found.")
```

### Comparing `tootstagram-0.0.2/tootstagram/mastodon.py` & `tootstagram-0.0.3/tootstagram/mastodon.py`

 * *Files identical despite different names*

### Comparing `tootstagram-0.0.2/tootstagram.egg-info/PKG-INFO` & `tootstagram-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tootstagram
-Version: 0.0.2
+Version: 0.0.3
 Summary: Duplicate posted images from Mastodon to Instagram
 Author-email: Koen Martens <kmartens@sonologic.se>
 Project-URL: Homepage, https://cvs.sonologic.net/gmc/tootstagram
 Project-URL: Bug Tracker, https://cvs.sonologic.net/gmc/tootstagram/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
@@ -40,17 +40,30 @@
 ```
 tootstagram
 ```
 
 This will fetch the feed from the Mastodon account and post any
 images that were not already posted to the Instagram account.
 
+## Security
+
+Make sure you keep the configuration file as well as the `.tootstagram`
+directory in your home or user dir private. The configuration file 
+contains your instagram username and password, and the `.tootstagram`
+directory contains a file `session.json` which should be treated as
+equivalent to your username and password.
+
 ## Limitations
 
 * Only posts toots with images, not videos (I don't do videos myself)
 * Any html tags in the toot are crudely removed by a simple regexp
 * If a toot has multiple images, but not all have alt text, none of the
   instagram posts will have alt text (because it is impossible to derive
   from the feed which alt text belongs to which image)
 * Editing a toot will not alter on or repost to instagram
 * Only posts listed toots, as those are the only ones available from the
   feed
+
+## Planned features
+
+* Hashtag translation
+
```

