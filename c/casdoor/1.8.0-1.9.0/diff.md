# Comparing `tmp/casdoor-1.8.0.tar.gz` & `tmp/casdoor-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casdoor-1.8.0.tar", last modified: Fri Feb 10 01:08:18 2023, max compression
+gzip compressed data, was "casdoor-1.9.0.tar", last modified: Sat Apr 15 17:37:13 2023, max compression
```

## Comparing `casdoor-1.8.0.tar` & `casdoor-1.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 01:08:18.478085 casdoor-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-10 01:07:43.000000 casdoor-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-02-10 01:08:18.478085 casdoor-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-02-10 01:07:43.000000 casdoor-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-10 01:07:43.000000 casdoor-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-02-10 01:08:18.482085 casdoor-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-10 01:07:43.000000 casdoor-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 01:08:18.478085 casdoor-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 01:08:18.478085 casdoor-1.8.0/src/casdoor/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-10 01:07:43.000000 casdoor-1.8.0/src/casdoor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-02-10 01:07:43.000000 casdoor-1.8.0/src/casdoor/async_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-02-10 01:07:43.000000 casdoor-1.8.0/src/casdoor/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-02-10 01:07:43.000000 casdoor-1.8.0/src/casdoor/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 01:08:18.478085 casdoor-1.8.0/src/casdoor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-02-10 01:08:18.000000 casdoor-1.8.0/src/casdoor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-02-10 01:08:18.000000 casdoor-1.8.0/src/casdoor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 01:08:18.000000 casdoor-1.8.0/src/casdoor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-10 01:08:18.000000 casdoor-1.8.0/src/casdoor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-10 01:08:18.000000 casdoor-1.8.0/src/casdoor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:37:13.124573 casdoor-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-15 17:36:40.000000 casdoor-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-04-15 17:37:13.128573 casdoor-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-04-15 17:36:40.000000 casdoor-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-15 17:36:40.000000 casdoor-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-15 17:37:13.128573 casdoor-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-15 17:36:40.000000 casdoor-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:37:13.124573 casdoor-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:37:13.124573 casdoor-1.9.0/src/casdoor/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-15 17:36:40.000000 casdoor-1.9.0/src/casdoor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-04-15 17:36:40.000000 casdoor-1.9.0/src/casdoor/async_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-04-15 17:36:40.000000 casdoor-1.9.0/src/casdoor/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-15 17:36:40.000000 casdoor-1.9.0/src/casdoor/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:37:13.124573 casdoor-1.9.0/src/casdoor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-04-15 17:37:13.000000 casdoor-1.9.0/src/casdoor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-15 17:37:13.000000 casdoor-1.9.0/src/casdoor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 17:37:13.000000 casdoor-1.9.0/src/casdoor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-15 17:37:13.000000 casdoor-1.9.0/src/casdoor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 17:37:13.000000 casdoor-1.9.0/src/casdoor.egg-info/top_level.txt
```

### Comparing `casdoor-1.8.0/LICENSE` & `casdoor-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casdoor-1.8.0/PKG-INFO` & `casdoor-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casdoor
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python SDK built for Casdoor
 Home-page: https://github.com/casdoor/casdoor-python-sdk
 Author: ffyuanda
 Author-email: shaoxuan.yuan02@gmail.com
 License: Apache 2.0
 Keywords: Casdoor
 Platform: any
@@ -132,15 +132,15 @@
 casdoor-python-sdk support basic user operations, like:
 
 - `get_user(user_id: str)`, get one user by user name.
 - `get_users()`, get all users.
 - `modify_user(method: str, user: User)/add_user(user: User)/update_user(user: User)/delete_user(user: User)`, write user to database.
 - `refresh_token_request(refresh_token: str, scope: str)`, refresh access token
 - `enforce(self, permission_model_name: str, sub: str, obj: str, act: str)`, check permission from model
-
+- `get_user_count(is_online: bool = None)`, get user count.
 
 ## Resource Owner Password Credentials Grant
 
 If your application doesn't have a frontend that redirects users to Casdoor and you have Password Credentials Grant enabled, then you may get access token like this:
 
 ```python
 access_token = sdk.get_oauth_token(username=username, password=password)
```

### Comparing `casdoor-1.8.0/README.md` & `casdoor-1.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 casdoor-python-sdk support basic user operations, like:
 
 - `get_user(user_id: str)`, get one user by user name.
 - `get_users()`, get all users.
 - `modify_user(method: str, user: User)/add_user(user: User)/update_user(user: User)/delete_user(user: User)`, write user to database.
 - `refresh_token_request(refresh_token: str, scope: str)`, refresh access token
 - `enforce(self, permission_model_name: str, sub: str, obj: str, act: str)`, check permission from model
-
+- `get_user_count(is_online: bool = None)`, get user count.
 
 ## Resource Owner Password Credentials Grant
 
 If your application doesn't have a frontend that redirects users to Casdoor and you have Password Credentials Grant enabled, then you may get access token like this:
 
 ```python
 access_token = sdk.get_oauth_token(username=username, password=password)
```

### Comparing `casdoor-1.8.0/setup.cfg` & `casdoor-1.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = casdoor
-version = 1.8.0
+version = 1.9.0
 author = ffyuanda
 author_email = shaoxuan.yuan02@gmail.com
 url = https://github.com/casdoor/casdoor-python-sdk
 description = Python SDK built for Casdoor
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache 2.0
```

### Comparing `casdoor-1.8.0/src/casdoor/async_main.py` & `casdoor-1.9.0/src/casdoor/async_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,14 +328,37 @@
             "clientId": self.client_id,
             "clientSecret": self.client_secret,
         }
         async with self._session.get(url, params=params) as request:
             user = await request.json()
             return user
 
+    async def get_user_count(self, is_online: bool = None) -> int:
+        """
+        Get the count of filtered users for an organization
+        :param is_online: True for online users, False for offline users,
+                          None for all users
+        :return: the count of filtered users for an organization
+        """
+        url = self.endpoint + "/api/get-user-count"
+        params = {
+            "owner": self.org_name,
+            "clientId": self.client_id,
+            "clientSecret": self.client_secret,
+        }
+
+        if is_online is None:
+            params["isOnline"] = ""
+        else:
+            params["isOnline"] = "1" if is_online else "0"
+
+        async with self._session.get(url, params=params) as request:
+            count = await request.json()
+            return count
+
     async def modify_user(self, method: str, user: User) -> dict:
         url = self.endpoint + f"/api/{method}"
         user.owner = self.org_name
         params = {
             "id": f"{user.owner}/{user.name}",
             "clientId": self.client_id,
             "clientSecret": self.client_secret,
```

### Comparing `casdoor-1.8.0/src/casdoor/main.py` & `casdoor-1.9.0/src/casdoor/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -312,14 +312,37 @@
             "clientId": self.client_id,
             "clientSecret": self.client_secret,
         }
         r = requests.get(url, params)
         user = r.json()
         return user
 
+    def get_user_count(self, is_online: bool = None) -> int:
+        """
+        Get the count of filtered users for an organization
+        :param is_online: True for online users, False for offline users,
+                          None for all users
+        :return: the count of filtered users for an organization
+        """
+        url = self.endpoint + "/api/get-user-count"
+        params = {
+            "owner": self.org_name,
+            "clientId": self.client_id,
+            "clientSecret": self.client_secret,
+        }
+
+        if is_online is None:
+            params["isOnline"] = ""
+        else:
+            params["isOnline"] = "1" if is_online else "0"
+
+        r = requests.get(url, params)
+        count = r.json()
+        return count
+
     def modify_user(self, method: str, user: User) -> dict:
         url = self.endpoint + f"/api/{method}"
         user.owner = self.org_name
         params = {
             "id": f"{user.owner}/{user.name}",
             "clientId": self.client_id,
             "clientSecret": self.client_secret,
```

### Comparing `casdoor-1.8.0/src/casdoor/user.py` & `casdoor-1.9.0/src/casdoor/user.py`

 * *Files identical despite different names*

### Comparing `casdoor-1.8.0/src/casdoor.egg-info/PKG-INFO` & `casdoor-1.9.0/src/casdoor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casdoor
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python SDK built for Casdoor
 Home-page: https://github.com/casdoor/casdoor-python-sdk
 Author: ffyuanda
 Author-email: shaoxuan.yuan02@gmail.com
 License: Apache 2.0
 Keywords: Casdoor
 Platform: any
@@ -132,15 +132,15 @@
 casdoor-python-sdk support basic user operations, like:
 
 - `get_user(user_id: str)`, get one user by user name.
 - `get_users()`, get all users.
 - `modify_user(method: str, user: User)/add_user(user: User)/update_user(user: User)/delete_user(user: User)`, write user to database.
 - `refresh_token_request(refresh_token: str, scope: str)`, refresh access token
 - `enforce(self, permission_model_name: str, sub: str, obj: str, act: str)`, check permission from model
-
+- `get_user_count(is_online: bool = None)`, get user count.
 
 ## Resource Owner Password Credentials Grant
 
 If your application doesn't have a frontend that redirects users to Casdoor and you have Password Credentials Grant enabled, then you may get access token like this:
 
 ```python
 access_token = sdk.get_oauth_token(username=username, password=password)
```

