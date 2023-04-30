# Comparing `tmp/flask_encrypted_cookies_session-0.2.3.tar.gz` & `tmp/flask_encrypted_cookies_session-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_encrypted_cookies_session-0.2.3.tar", max compression
+gzip compressed data, was "flask_encrypted_cookies_session-0.2.4.tar", max compression
```

## Comparing `flask_encrypted_cookies_session-0.2.3.tar` & `flask_encrypted_cookies_session-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    21396 2023-04-30 16:30:45.937257 flask_encrypted_cookies_session-0.2.3/LICENSE
--rw-r--r--   0        0        0     2792 2023-04-30 18:14:55.257658 flask_encrypted_cookies_session-0.2.3/README.md
--rw-r--r--   0        0        0      194 2023-04-30 18:15:40.101879 flask_encrypted_cookies_session-0.2.3/flask_encrypted_cookies_session/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 16:30:45.937257 flask_encrypted_cookies_session-0.2.3/flask_encrypted_cookies_session/py.typed
--rw-r--r--   0        0        0     3738 2023-04-30 17:11:42.741374 flask_encrypted_cookies_session-0.2.3/flask_encrypted_cookies_session/session.py
--rw-r--r--   0        0        0     2012 2023-04-30 18:15:40.101879 flask_encrypted_cookies_session-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 flask_encrypted_cookies_session-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    21396 2023-04-30 16:30:45.937257 flask_encrypted_cookies_session-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2792 2023-04-30 18:14:55.257658 flask_encrypted_cookies_session-0.2.4/README.md
+-rw-r--r--   0        0        0      194 2023-04-30 18:28:38.767272 flask_encrypted_cookies_session-0.2.4/flask_encrypted_cookies_session/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 16:30:45.937257 flask_encrypted_cookies_session-0.2.4/flask_encrypted_cookies_session/py.typed
+-rw-r--r--   0        0        0     3702 2023-04-30 18:28:14.451434 flask_encrypted_cookies_session-0.2.4/flask_encrypted_cookies_session/session.py
+-rw-r--r--   0        0        0     2012 2023-04-30 18:28:38.767272 flask_encrypted_cookies_session-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 flask_encrypted_cookies_session-0.2.4/PKG-INFO
```

### Comparing `flask_encrypted_cookies_session-0.2.3/LICENSE` & `flask_encrypted_cookies_session-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_encrypted_cookies_session-0.2.3/README.md` & `flask_encrypted_cookies_session-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `flask_encrypted_cookies_session-0.2.3/flask_encrypted_cookies_session/session.py` & `flask_encrypted_cookies_session-0.2.4/flask_encrypted_cookies_session/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 class FernetJSONSerializer(SerializerInterface):
     """
     A simple JSON backed serializer that rely on Fernet authenticated encryption
     """
 
     def __init__(self, encryption_key: FernetType) -> None:
         self._encryption_key = encryption_key
-        print(type(encryption_key))
 
     def dumps(self, obj: Any) -> Union[str, bytes]:
         data = json.dumps(obj).encode("utf-8")
         return self._encryption_key.encrypt(data)
 
     def loads(
         self, s: Union[str, bytes], **kwargs: Any  # pylint: disable=invalid-name
```

### Comparing `flask_encrypted_cookies_session-0.2.3/pyproject.toml` & `flask_encrypted_cookies_session-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask_encrypted_cookies_session"
-version = "0.2.3" # Managed by poetry-dynamic-versioning
+version = "0.2.4" # Managed by poetry-dynamic-versioning
 description = "An encrypted cookie based session implementation for flask"
 authors = ["Rémi Ferrand <riton.github@gmail.com>"]
 readme = ["README.md"]
 license = "CECILL-B"
 homepage = "https://github.com/riton/flask-encrypted-cookies-session"
 keywords = ["flask", "session", "cookies", "fernet"]
```

### Comparing `flask_encrypted_cookies_session-0.2.3/PKG-INFO` & `flask_encrypted_cookies_session-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-encrypted-cookies-session
-Version: 0.2.3
+Version: 0.2.4
 Summary: An encrypted cookie based session implementation for flask
 Home-page: https://github.com/riton/flask-encrypted-cookies-session
 License: CECILL-B
 Keywords: flask,session,cookies,fernet
 Author: Rémi Ferrand
 Author-email: riton.github@gmail.com
 Requires-Python: >=3.9,<4.0
```

