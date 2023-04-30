# Comparing `tmp/jellyash-0.3.3.tar.gz` & `tmp/jellyash-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jellyash-0.3.3.tar", last modified: Thu Feb  9 10:03:16 2023, max compression
+gzip compressed data, was "jellyash-0.3.4.tar", last modified: Sun Apr 30 08:37:35 2023, max compression
```

## Comparing `jellyash-0.3.3.tar` & `jellyash-0.3.4.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-02-09 10:03:16.242639 jellyash-0.3.3/
--rw-rw-r--   0 steven    (1000) steven    (1000)     1080 2023-01-31 23:22:28.000000 jellyash-0.3.3/LICENSE
--rw-rw-r--   0 steven    (1000) steven    (1000)     1970 2023-02-09 10:03:16.242639 jellyash-0.3.3/PKG-INFO
--rw-rw-r--   0 steven    (1000) steven    (1000)      693 2023-02-06 00:46:32.000000 jellyash-0.3.3/README.md
-drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-02-09 10:03:16.242639 jellyash-0.3.3/jellyash/
--rw-rw-r--   0 steven    (1000) steven    (1000)       22 2023-02-08 23:20:27.000000 jellyash-0.3.3/jellyash/__init__.py
--rw-rw-r--   0 steven    (1000) steven    (1000)     2235 2023-02-06 00:46:32.000000 jellyash-0.3.3/jellyash/client.py
--rw-rw-r--   0 steven    (1000) steven    (1000)      806 2023-02-06 00:46:32.000000 jellyash-0.3.3/jellyash/duration.py
--rw-rw-r--   0 steven    (1000) steven    (1000)      511 2023-02-06 00:47:28.000000 jellyash-0.3.3/jellyash/nextup.py
--rw-rw-r--   0 steven    (1000) steven    (1000)      455 2023-02-02 01:14:36.000000 jellyash-0.3.3/jellyash/series.py
--rw-rw-r--   0 steven    (1000) steven    (1000)      875 2023-02-08 23:16:45.000000 jellyash-0.3.3/jellyash/token.py
--rw-rw-r--   0 steven    (1000) steven    (1000)     1239 2023-02-06 00:46:32.000000 jellyash-0.3.3/jellyash/unwatched.py
-drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-02-09 10:03:16.242639 jellyash-0.3.3/jellyash.egg-info/
--rw-rw-r--   0 steven    (1000) steven    (1000)     1970 2023-02-09 10:03:16.000000 jellyash-0.3.3/jellyash.egg-info/PKG-INFO
--rw-rw-r--   0 steven    (1000) steven    (1000)      365 2023-02-09 10:03:16.000000 jellyash-0.3.3/jellyash.egg-info/SOURCES.txt
--rw-rw-r--   0 steven    (1000) steven    (1000)        1 2023-02-09 10:03:16.000000 jellyash-0.3.3/jellyash.egg-info/dependency_links.txt
--rw-rw-r--   0 steven    (1000) steven    (1000)      206 2023-02-09 10:03:16.000000 jellyash-0.3.3/jellyash.egg-info/entry_points.txt
--rw-rw-r--   0 steven    (1000) steven    (1000)       26 2023-02-09 10:03:16.000000 jellyash-0.3.3/jellyash.egg-info/requires.txt
--rw-rw-r--   0 steven    (1000) steven    (1000)        9 2023-02-09 10:03:16.000000 jellyash-0.3.3/jellyash.egg-info/top_level.txt
--rw-rw-r--   0 steven    (1000) steven    (1000)      515 2023-02-06 00:46:32.000000 jellyash-0.3.3/pyproject.toml
--rw-rw-r--   0 steven    (1000) steven    (1000)       38 2023-02-09 10:03:16.242639 jellyash-0.3.3/setup.cfg
+drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-04-30 08:37:35.303136 jellyash-0.3.4/
+-rw-rw-r--   0 steven    (1000) steven    (1000)     1080 2023-01-31 23:22:28.000000 jellyash-0.3.4/LICENSE
+-rw-rw-r--   0 steven    (1000) steven    (1000)     1970 2023-04-30 08:37:35.303136 jellyash-0.3.4/PKG-INFO
+-rw-rw-r--   0 steven    (1000) steven    (1000)      693 2023-02-06 00:46:32.000000 jellyash-0.3.4/README.md
+drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-04-30 08:37:35.303136 jellyash-0.3.4/jellyash/
+-rw-rw-r--   0 steven    (1000) steven    (1000)       22 2023-04-30 08:26:35.000000 jellyash-0.3.4/jellyash/__init__.py
+-rw-rw-r--   0 steven    (1000) steven    (1000)     1264 2023-04-30 07:51:28.000000 jellyash-0.3.4/jellyash/bundle.py
+-rw-rw-r--   0 steven    (1000) steven    (1000)     1451 2023-04-30 08:22:47.000000 jellyash-0.3.4/jellyash/client.py
+-rw-rw-r--   0 steven    (1000) steven    (1000)      813 2023-04-30 08:22:47.000000 jellyash-0.3.4/jellyash/duration.py
+-rw-rw-r--   0 steven    (1000) steven    (1000)      556 2023-04-30 08:30:37.000000 jellyash-0.3.4/jellyash/nextup.py
+-rw-rw-r--   0 steven    (1000) steven    (1000)      494 2023-04-30 08:26:35.000000 jellyash-0.3.4/jellyash/series.py
+-rw-rw-r--   0 steven    (1000) steven    (1000)      906 2023-04-30 08:22:47.000000 jellyash-0.3.4/jellyash/token.py
+-rw-rw-r--   0 steven    (1000) steven    (1000)     1281 2023-04-30 08:22:47.000000 jellyash-0.3.4/jellyash/unwatched.py
+drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-04-30 08:37:35.303136 jellyash-0.3.4/jellyash.egg-info/
+-rw-rw-r--   0 steven    (1000) steven    (1000)     1970 2023-04-30 08:37:35.000000 jellyash-0.3.4/jellyash.egg-info/PKG-INFO
+-rw-rw-r--   0 steven    (1000) steven    (1000)      426 2023-04-30 08:37:35.000000 jellyash-0.3.4/jellyash.egg-info/SOURCES.txt
+-rw-rw-r--   0 steven    (1000) steven    (1000)        1 2023-04-30 08:37:35.000000 jellyash-0.3.4/jellyash.egg-info/dependency_links.txt
+-rw-rw-r--   0 steven    (1000) steven    (1000)      206 2023-04-30 08:37:35.000000 jellyash-0.3.4/jellyash.egg-info/entry_points.txt
+-rw-rw-r--   0 steven    (1000) steven    (1000)       72 2023-04-30 08:37:35.000000 jellyash-0.3.4/jellyash.egg-info/requires.txt
+-rw-rw-r--   0 steven    (1000) steven    (1000)        9 2023-04-30 08:37:35.000000 jellyash-0.3.4/jellyash.egg-info/top_level.txt
+-rw-rw-r--   0 steven    (1000) steven    (1000)      593 2023-04-30 08:22:47.000000 jellyash-0.3.4/pyproject.toml
+-rw-rw-r--   0 steven    (1000) steven    (1000)       38 2023-04-30 08:37:35.303136 jellyash-0.3.4/setup.cfg
+drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-04-30 08:37:35.303136 jellyash-0.3.4/tests/
+-rw-rw-r--   0 steven    (1000) steven    (1000)      666 2023-04-30 07:50:08.000000 jellyash-0.3.4/tests/test_bundle.py
+-rw-rw-r--   0 steven    (1000) steven    (1000)     2463 2023-04-30 07:52:18.000000 jellyash-0.3.4/tests/test_client.py
```

### Comparing `jellyash-0.3.3/LICENSE` & `jellyash-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jellyash-0.3.3/PKG-INFO` & `jellyash-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jellyash
-Version: 0.3.3
+Version: 0.3.4
 License: Copyright 2023 Steve Kowalik <steven@wedontsleep.org>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `jellyash-0.3.3/README.md` & `jellyash-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `jellyash-0.3.3/jellyash/client.py` & `jellyash-0.3.4/jellyash/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,89 +1,53 @@
-import json
 import inspect
-from pathlib import Path
+import json
+import pathlib
 import platform
-from uuid import uuid4
 import sys
+from typing import Optional
+from uuid import uuid4
 
-from jellyfin_apiclient_python.api import API
 from jellyfin_apiclient_python.client import JellyfinClient
 
 from . import __version__
+from .bundle import WrappedAPI
 
-
-CREDENTIALS_FILE = Path.home() / ".jellyfin_creds"
-
-
-class WrappedAPI(API):
-    def _get(self, handler, params=None):
-        return ApiResponse(super()._get(handler, params=params))
+CREDENTIALS_FILE = pathlib.Path.home() / ".jellyfin_creds"
 
 
-def create_client(app_name=None):
+def create_client(app_name: Optional[str] = None):
     client = JellyfinClient()
     if not app_name:
         app_name = determine_app_name()
     client.config.app(app_name, __version__, platform.node(), str(uuid4()))
     client.config.data["auth.ssl"] = True
     client.jellyfin = WrappedAPI(client.http)
     return client
 
 
-def auth_with_password(client, address, user, password):
+def auth_with_password(client, address: str, user: str, password: str):
     client.auth.connect_to_address(address)
     return client.auth.login(address, user, password)
 
 
-def auth_with_token(client):
-    with open(CREDENTIALS_FILE, 'r') as f:
+def auth_with_token(client) -> None:
+    if not CREDENTIALS_FILE.is_file():
+        raise ValueError(f"{sys.argv[0]}: Requires credential file.")
+    with open(CREDENTIALS_FILE, "r") as f:
         credentials = json.load(f)
     client.authenticate({"Servers": [credentials]}, discover=False)
 
 
 def authed_client():
-    if not CREDENTIALS_FILE.is_file():
-        print(f"{sys.argv[0]}: Requires credential file.")
-        sys.exit(1)
     client = create_client(None)
-    auth_with_token(client)
+    try:
+        auth_with_token(client)
+    except (PermissionError, ValueError, json.decoder.JSONDecodeError) as e:
+        print(e)
+        sys.exit(1)
     return client
 
 
-def determine_app_name():
+def determine_app_name() -> str:
     frame = inspect.stack()[-2]
     return f"jellyfin_{inspect.getmodulename(frame.filename)}"
 
-
-class ApiResponse:
-    def __init__(self, value):
-        self.value = value
-
-    def __str__(self):
-        return f"<ApiResponse object containing {len(self)} items>"
-
-    def __iter__(self):
-        yield from [Item(i) for i in self.value["Items"]]
-
-    def __getitem__(self, key):
-        return Item(self.value["Items"][key])
-
-    def __len__(self):
-        return self.value["TotalRecordCount"] + self.value["StartIndex"]
-
-
-class Item:
-    def __init__(self, item):
-        self.item = item
-
-    def _raw_item(self):
-        return self.item
-
-    def __getattr__(self, attr):
-        try:
-            value = self.item[attr]
-            if isinstance(value, dict):
-                value = Item(value)
-            return value
-        except KeyError:
-            raise AttributeError(f"Item has no attribute '{attr}'")
-
```

### Comparing `jellyash-0.3.3/jellyash/duration.py` & `jellyash-0.3.4/jellyash/duration.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import argparse
 from decimal import Decimal
 
 from .client import authed_client
 from .series import search_single_show
 
 
-def average_duration():
+def average_duration() -> None:
     parser = argparse.ArgumentParser()
-    parser.add_argument('show', nargs='+')
+    parser.add_argument("show", nargs="+")
     args = parser.parse_args()
     client = authed_client()
     try:
         show = search_single_show(client, " ".join(args.show))
     except ValueError as e:
         print(str(e))
         return
     count = 0
     duration = 0
     for season in client.jellyfin.get_seasons(show.Id):
         count += season.ChildCount
         episodes = client.jellyfin.get_season(show.Id, season.Id)
         duration += sum([e.RunTimeTicks for e in episodes])
-    average = (duration / count) / int(Decimal('6E+008'))
+    average = (duration / count) / int(Decimal("6E+008"))
     print(f"Average duration over {count} episodes: {average:.1f} minutes")
-
```

### Comparing `jellyash-0.3.3/jellyash/token.py` & `jellyash-0.3.4/jellyash/token.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import argparse
 import json
-from getpass import getpass as getpassword, getuser
+from getpass import getpass as getpassword
+from getpass import getuser
 
-from .client import create_client, auth_with_password, CREDENTIALS_FILE
+from .client import CREDENTIALS_FILE, auth_with_password, create_client
 
 
-def create_jellyfin_token():
-    client = create_client('create_jellyfin_token')
+def create_jellyfin_token() -> None:
+    client = create_client("create_jellyfin_token")
     parser = argparse.ArgumentParser()
-    parser.add_argument('-u', '--user', dest='user', default=getuser())
+    parser.add_argument("-u", "--user", dest="user", default=getuser())
     parser.add_argument(
-        'server', nargs='?', default="https://jellyfin.wedontsleep.org/")
+        "server", nargs="?", default="https://jellyfin.wedontsleep.org/"
+    )
     args = parser.parse_args()
     password = getpassword()
     result = auth_with_password(client, args.server, args.user, password)
     if "AccessToken" in result:
         credentials = client.auth.credentials.get_credentials()
         server = credentials["Servers"][0]
         server["username"] = args.user
-        with open(CREDENTIALS_FILE, 'w') as f:
+        with open(CREDENTIALS_FILE, "w") as f:
             json.dump(server, f)
         print("Credentials saved.")
-
```

### Comparing `jellyash-0.3.3/jellyash/unwatched.py` & `jellyash-0.3.4/jellyash/unwatched.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import argparse
 from operator import attrgetter
 
 from .client import authed_client
 from .series import search_single_show
 
 
-def unwatched():
+def unwatched() -> None:
     client = authed_client()
     parser = argparse.ArgumentParser()
-    parser.add_argument('show', nargs='*')
+    parser.add_argument("show", nargs="*")
     args = parser.parse_args()
     if not args.show:
         all_unwatched(client)
     else:
         specific_unwatched(client, " ".join(args.show))
 
 
-def all_unwatched(client):
-    r = client.jellyfin.search_media_items(term="", media="Series", limit=300)
+def all_unwatched(client) -> None:
+    r = client.jellyfin.search_media_items(
+        term="", media="Series", limit=300
+    )
     total = 0
     for series in sorted(r, key=attrgetter("Name")):
         if (count := series.UserData.UnplayedItemCount) > 0:
-            ending = "s" if count != 1 else ''
+            ending = "s" if count != 1 else ""
             print(f"{series.Name}: {count} unwatched episode{ending}")
             total += count
     print(f"Total: {total} unwatched episodes")
 
 
-def specific_unwatched(client, term):
+def specific_unwatched(client, term: str) -> None:
     try:
         show = search_single_show(client, term)
     except ValueError as e:
         print(str(e))
         return
     unwatched = show.UserData.UnplayedItemCount
     total = sum(s.ChildCount for s in client.jellyfin.get_seasons(show.Id))
     print(f"{show.Name}: {total - unwatched} watched episodes")
     print(f"{show.Name}: {unwatched} unwatched episodes")
-
```

### Comparing `jellyash-0.3.3/jellyash.egg-info/PKG-INFO` & `jellyash-0.3.4/jellyash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jellyash
-Version: 0.3.3
+Version: 0.3.4
 License: Copyright 2023 Steve Kowalik <steven@wedontsleep.org>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `jellyash-0.3.3/pyproject.toml` & `jellyash-0.3.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -4,18 +4,22 @@
 
 [project]
 name = "jellyash"
 dynamic = ["version"]
 license = {file = "LICENSE"}
 readme = "README.md"
 dependencies = [
-	"jellyfin_apiclient_python",
+    "jellyfin_apiclient_python",
+    "typing_extensions;python_version<'3.11'",
 ]
 
 [project.scripts]
 average_duration = "jellyash.duration:average_duration"
 create_jellyfin_token = "jellyash.token:create_jellyfin_token"
 nextup = "jellyash.nextup:nextup"
 unwatched = "jellyash.unwatched:unwatched"
 
 [tool.setuptools.dynamic]
 version = {attr = "jellyash.__version__"}
+
+[tool.ruff]
+line-length=77
```

