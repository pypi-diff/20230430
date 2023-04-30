# Comparing `tmp/flask_encrypted_cookies_session-0.2.0.tar.gz` & `tmp/flask_encrypted_cookies_session-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_encrypted_cookies_session-0.2.0.tar", max compression
+gzip compressed data, was "flask_encrypted_cookies_session-0.2.1.tar", max compression
```

## Comparing `flask_encrypted_cookies_session-0.2.0.tar` & `flask_encrypted_cookies_session-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    21396 2023-04-30 16:30:45.937257 flask_encrypted_cookies_session-0.2.0/LICENSE
--rw-r--r--   0        0        0      194 2023-04-30 17:33:07.982407 flask_encrypted_cookies_session-0.2.0/flask_encrypted_cookies_session/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 16:30:45.937257 flask_encrypted_cookies_session-0.2.0/flask_encrypted_cookies_session/py.typed
--rw-r--r--   0        0        0     3738 2023-04-30 17:11:42.741374 flask_encrypted_cookies_session-0.2.0/flask_encrypted_cookies_session/session.py
--rw-r--r--   0        0        0     1946 2023-04-30 17:33:07.982407 flask_encrypted_cookies_session-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 flask_encrypted_cookies_session-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    21396 2023-04-30 16:30:45.937257 flask_encrypted_cookies_session-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3031 2023-04-30 16:30:45.937257 flask_encrypted_cookies_session-0.2.1/README.md
+-rw-r--r--   0        0        0      194 2023-04-30 17:56:49.768941 flask_encrypted_cookies_session-0.2.1/flask_encrypted_cookies_session/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 16:30:45.937257 flask_encrypted_cookies_session-0.2.1/flask_encrypted_cookies_session/py.typed
+-rw-r--r--   0        0        0     3738 2023-04-30 17:11:42.741374 flask_encrypted_cookies_session-0.2.1/flask_encrypted_cookies_session/session.py
+-rw-r--r--   0        0        0     2022 2023-04-30 17:56:49.768941 flask_encrypted_cookies_session-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3798 1970-01-01 00:00:00.000000 flask_encrypted_cookies_session-0.2.1/PKG-INFO
```

### Comparing `flask_encrypted_cookies_session-0.2.0/LICENSE` & `flask_encrypted_cookies_session-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_encrypted_cookies_session-0.2.0/flask_encrypted_cookies_session/session.py` & `flask_encrypted_cookies_session-0.2.1/flask_encrypted_cookies_session/session.py`

 * *Files identical despite different names*

### Comparing `flask_encrypted_cookies_session-0.2.0/pyproject.toml` & `flask_encrypted_cookies_session-0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [tool.poetry]
 name = "flask_encrypted_cookies_session"
-version = "0.2.0" # Managed by poetry-dynamic-versioning
+version = "0.2.1" # Managed by poetry-dynamic-versioning
 description = "An encrypted cookie based session implementation for flask"
 authors = ["Rémi Ferrand <remi.ferrand@cc.in2p3.fr>"]
+readme = ["README.md"]
 license = "CECILL-B"
 homepage = "https://gitlab.in2p3.fr/rferrand/flask-encrypted-cookies-session"
+keywords = ["flask", "session", "cookies", "frenet"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 cryptography = "^40.0.2"
 flask = "^2.3.1"
 
 [tool.poetry.group.dev.dependencies]
```

