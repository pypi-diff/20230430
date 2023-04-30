# Comparing `tmp/pygti-0.9.3.tar.gz` & `tmp/pygti-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygti-0.9.3.tar", last modified: Wed Jul 13 20:56:32 2022, max compression
+gzip compressed data, was "pygti-0.9.4.tar", last modified: Sun Apr 30 10:18:10 2023, max compression
```

## Comparing `pygti-0.9.3.tar` & `pygti-0.9.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2022-07-13 20:56:32.595716 pygti-0.9.3/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2022-07-13 20:56:32.593626 pygti-0.9.3/.devcontainer/
--rw-r--r--   0 tom        (501) staff       (20)      975 2022-07-13 20:43:54.000000 pygti-0.9.3/.devcontainer/Dockerfile
--rw-r--r--   0 tom        (501) staff       (20)     2470 2022-07-13 20:43:54.000000 pygti-0.9.3/.devcontainer/base.Dockerfile
--rw-r--r--   0 tom        (501) staff       (20)     1644 2022-07-13 20:43:54.000000 pygti-0.9.3/.devcontainer/devcontainer.json
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2022-07-13 20:56:32.594158 pygti-0.9.3/.devcontainer/library-scripts/
--rw-r--r--   0 tom        (501) staff       (20)      483 2022-07-13 20:43:54.000000 pygti-0.9.3/.devcontainer/library-scripts/README.md
--rw-r--r--   0 tom        (501) staff       (20)     6470 2022-07-13 20:43:54.000000 pygti-0.9.3/.devcontainer/library-scripts/common-debian.sh
--rw-r--r--   0 tom        (501) staff       (20)     3470 2022-07-13 20:43:54.000000 pygti-0.9.3/.devcontainer/library-scripts/node-debian.sh
--rw-r--r--   0 tom        (501) staff       (20)     4499 2022-07-13 20:43:54.000000 pygti-0.9.3/.devcontainer/library-scripts/python-debian.sh
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2022-07-13 20:56:32.594278 pygti-0.9.3/.github/
--rw-r--r--   0 tom        (501) staff       (20)      759 2022-07-13 20:43:54.000000 pygti-0.9.3/.github/release-drafter.yml
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2022-07-13 20:56:32.594410 pygti-0.9.3/.github/workflows/
--rw-r--r--   0 tom        (501) staff       (20)      395 2022-07-13 20:43:54.000000 pygti-0.9.3/.github/workflows/release-drafter.yml
--rw-r--r--   0 tom        (501) staff       (20)     1696 2022-07-13 20:43:54.000000 pygti-0.9.3/.gitignore
--rw-r--r--   0 tom        (501) staff       (20)      332 2022-07-13 20:43:54.000000 pygti-0.9.3/.pre-commit-config.yaml
--rw-r--r--   0 tom        (501) staff       (20)     1767 2022-07-13 20:43:54.000000 pygti-0.9.3/CONTRIBUTING.md
--rw-r--r--   0 tom        (501) staff       (20)    11347 2022-07-13 20:43:54.000000 pygti-0.9.3/LICENSE.md
--rw-r--r--   0 tom        (501) staff       (20)     4999 2022-07-13 20:56:32.595795 pygti-0.9.3/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     4324 2022-07-13 20:43:54.000000 pygti-0.9.3/README.md
--rw-r--r--   0 tom        (501) staff       (20)      853 2022-07-13 20:43:54.000000 pygti-0.9.3/azure-pipelines.yml
--rw-r--r--   0 tom        (501) staff       (20)    10906 2022-07-13 20:43:54.000000 pygti-0.9.3/examples.py
--rw-r--r--   0 tom        (501) staff       (20)     1662 2022-07-13 20:43:54.000000 pygti-0.9.3/notes.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2022-07-13 20:56:32.594978 pygti-0.9.3/pygti/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-07-13 20:43:54.000000 pygti-0.9.3/pygti/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     2435 2022-07-13 20:55:32.000000 pygti-0.9.3/pygti/auth.py
--rw-r--r--   0 tom        (501) staff       (20)     1014 2022-07-13 20:43:54.000000 pygti-0.9.3/pygti/const.py
--rw-r--r--   0 tom        (501) staff       (20)      778 2022-07-13 20:43:54.000000 pygti-0.9.3/pygti/exceptions.py
--rw-r--r--   0 tom        (501) staff       (20)     4391 2022-07-13 20:43:54.000000 pygti-0.9.3/pygti/gti.py
--rw-r--r--   0 tom        (501) staff       (20)    81527 2022-07-13 20:43:54.000000 pygti-0.9.3/pygti/schemas.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2022-07-13 20:56:32.595514 pygti-0.9.3/pygti.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     4999 2022-07-13 20:56:32.000000 pygti-0.9.3/pygti.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      785 2022-07-13 20:56:32.000000 pygti-0.9.3/pygti.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2022-07-13 20:56:32.000000 pygti-0.9.3/pygti.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)       24 2022-07-13 20:56:32.000000 pygti-0.9.3/pygti.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)        6 2022-07-13 20:56:32.000000 pygti-0.9.3/pygti.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       94 2022-07-13 20:43:54.000000 pygti-0.9.3/pytest.ini
--rw-r--r--   0 tom        (501) staff       (20)       18 2022-07-13 20:43:54.000000 pygti-0.9.3/requirements_dev.txt
--rw-r--r--   0 tom        (501) staff       (20)       27 2022-07-13 20:43:54.000000 pygti-0.9.3/requirements_test.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2022-07-13 20:56:32.595626 pygti-0.9.3/script/
--rw-r--r--   0 tom        (501) staff       (20)      544 2022-07-13 20:43:54.000000 pygti-0.9.3/script/generate.py
--rw-r--r--   0 tom        (501) staff       (20)      142 2022-07-13 20:56:32.596002 pygti-0.9.3/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)     3666 2022-07-13 20:43:54.000000 pygti-0.9.3/setup.py
--rw-r--r--   0 tom        (501) staff       (20)      193 2022-07-13 20:43:54.000000 pygti-0.9.3/tox.ini
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-30 10:18:10.848680 pygti-0.9.4/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-30 10:18:10.846241 pygti-0.9.4/.devcontainer/
+-rw-r--r--   0 tom        (501) staff       (20)      975 2022-07-13 20:43:54.000000 pygti-0.9.4/.devcontainer/Dockerfile
+-rw-r--r--   0 tom        (501) staff       (20)     2470 2022-07-13 20:43:54.000000 pygti-0.9.4/.devcontainer/base.Dockerfile
+-rw-r--r--   0 tom        (501) staff       (20)     1644 2022-07-13 20:43:54.000000 pygti-0.9.4/.devcontainer/devcontainer.json
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-30 10:18:10.846756 pygti-0.9.4/.devcontainer/library-scripts/
+-rw-r--r--   0 tom        (501) staff       (20)      483 2022-07-13 20:43:54.000000 pygti-0.9.4/.devcontainer/library-scripts/README.md
+-rw-r--r--   0 tom        (501) staff       (20)     6470 2022-07-13 20:43:54.000000 pygti-0.9.4/.devcontainer/library-scripts/common-debian.sh
+-rw-r--r--   0 tom        (501) staff       (20)     3470 2022-07-13 20:43:54.000000 pygti-0.9.4/.devcontainer/library-scripts/node-debian.sh
+-rw-r--r--   0 tom        (501) staff       (20)     4499 2022-07-13 20:43:54.000000 pygti-0.9.4/.devcontainer/library-scripts/python-debian.sh
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-30 10:18:10.846880 pygti-0.9.4/.github/
+-rw-r--r--   0 tom        (501) staff       (20)      759 2022-07-13 20:43:54.000000 pygti-0.9.4/.github/release-drafter.yml
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-30 10:18:10.847011 pygti-0.9.4/.github/workflows/
+-rw-r--r--   0 tom        (501) staff       (20)      395 2022-07-13 20:43:54.000000 pygti-0.9.4/.github/workflows/release-drafter.yml
+-rw-r--r--   0 tom        (501) staff       (20)     1696 2022-07-13 20:43:54.000000 pygti-0.9.4/.gitignore
+-rw-r--r--   0 tom        (501) staff       (20)      332 2022-07-13 20:43:54.000000 pygti-0.9.4/.pre-commit-config.yaml
+-rw-r--r--   0 tom        (501) staff       (20)     1767 2022-07-13 20:43:54.000000 pygti-0.9.4/CONTRIBUTING.md
+-rw-r--r--   0 tom        (501) staff       (20)    11347 2022-07-13 20:43:54.000000 pygti-0.9.4/LICENSE.md
+-rw-r--r--   0 tom        (501) staff       (20)     4999 2023-04-30 10:18:10.848758 pygti-0.9.4/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     4324 2022-07-13 20:43:54.000000 pygti-0.9.4/README.md
+-rw-r--r--   0 tom        (501) staff       (20)      853 2022-07-13 20:43:54.000000 pygti-0.9.4/azure-pipelines.yml
+-rw-r--r--   0 tom        (501) staff       (20)    10906 2023-04-30 10:17:58.000000 pygti-0.9.4/examples.py
+-rw-r--r--   0 tom        (501) staff       (20)     1662 2022-07-13 20:43:54.000000 pygti-0.9.4/notes.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-30 10:18:10.847745 pygti-0.9.4/pygti/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-07-13 20:43:54.000000 pygti-0.9.4/pygti/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     2435 2023-04-30 10:10:28.000000 pygti-0.9.4/pygti/auth.py
+-rw-r--r--   0 tom        (501) staff       (20)     1014 2022-07-13 20:43:54.000000 pygti-0.9.4/pygti/const.py
+-rw-r--r--   0 tom        (501) staff       (20)      778 2022-07-13 20:43:54.000000 pygti-0.9.4/pygti/exceptions.py
+-rw-r--r--   0 tom        (501) staff       (20)     4391 2022-07-13 20:43:54.000000 pygti-0.9.4/pygti/gti.py
+-rw-r--r--   0 tom        (501) staff       (20)    81527 2022-07-13 20:43:54.000000 pygti-0.9.4/pygti/schemas.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-30 10:18:10.848445 pygti-0.9.4/pygti.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)     4999 2023-04-30 10:18:10.000000 pygti-0.9.4/pygti.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      785 2023-04-30 10:18:10.000000 pygti-0.9.4/pygti.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-04-30 10:18:10.000000 pygti-0.9.4/pygti.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)       24 2023-04-30 10:18:10.000000 pygti-0.9.4/pygti.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)        6 2023-04-30 10:18:10.000000 pygti-0.9.4/pygti.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       94 2022-07-13 20:43:54.000000 pygti-0.9.4/pytest.ini
+-rw-r--r--   0 tom        (501) staff       (20)       18 2022-07-13 20:43:54.000000 pygti-0.9.4/requirements_dev.txt
+-rw-r--r--   0 tom        (501) staff       (20)       27 2022-07-13 20:43:54.000000 pygti-0.9.4/requirements_test.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-30 10:18:10.848568 pygti-0.9.4/script/
+-rw-r--r--   0 tom        (501) staff       (20)      544 2022-07-13 20:43:54.000000 pygti-0.9.4/script/generate.py
+-rw-r--r--   0 tom        (501) staff       (20)      142 2023-04-30 10:18:10.848994 pygti-0.9.4/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)     3666 2022-07-13 20:43:54.000000 pygti-0.9.4/setup.py
+-rw-r--r--   0 tom        (501) staff       (20)      193 2022-07-13 20:43:54.000000 pygti-0.9.4/tox.ini
```

### Comparing `pygti-0.9.3/.devcontainer/Dockerfile` & `pygti-0.9.4/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/.devcontainer/base.Dockerfile` & `pygti-0.9.4/.devcontainer/base.Dockerfile`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/.devcontainer/devcontainer.json` & `pygti-0.9.4/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/.devcontainer/library-scripts/common-debian.sh` & `pygti-0.9.4/.devcontainer/library-scripts/common-debian.sh`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/.devcontainer/library-scripts/node-debian.sh` & `pygti-0.9.4/.devcontainer/library-scripts/node-debian.sh`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/.devcontainer/library-scripts/python-debian.sh` & `pygti-0.9.4/.devcontainer/library-scripts/python-debian.sh`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/.github/release-drafter.yml` & `pygti-0.9.4/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/.gitignore` & `pygti-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/CONTRIBUTING.md` & `pygti-0.9.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/LICENSE.md` & `pygti-0.9.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/PKG-INFO` & `pygti-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygti
-Version: 0.9.3
+Version: 0.9.4
 Summary: access public transport information in hamburg, germany.
 Home-page: https://github.com/vigonotion/pygti
 Author: Tom Schneider
 Author-email: mail@vigonotion.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygti Version: 0.9.3 Summary: access public
+Metadata-Version: 2.1 Name: pygti Version: 0.9.4 Summary: access public
 transport information in hamburg, germany. Home-page: https://github.com/
 vigonotion/pygti Author: Tom Schneider Author-email: mail@vigonotion.com
 License: Apache-2.0 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
```

### Comparing `pygti-0.9.3/README.md` & `pygti-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/azure-pipelines.yml` & `pygti-0.9.4/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/examples.py` & `pygti-0.9.4/examples.py`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/notes.md` & `pygti-0.9.4/notes.md`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/pygti/auth.py` & `pygti-0.9.4/pygti/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         headers = kwargs.get("headers")
 
         if headers is None:
             headers = {}
         else:
             headers = dict(headers)
 
-        payload.update({"version": 38})
+        payload.update({"version": 54})
 
         data = self.websession.json_serialize(payload).encode("UTF-8")
 
         signature = base64.b64encode(
             hmac.new(self.password.encode("UTF-8"), data, hashlib.sha1).digest()
         ).decode("UTF-8")
```

### Comparing `pygti-0.9.3/pygti/const.py` & `pygti-0.9.4/pygti/const.py`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/pygti/exceptions.py` & `pygti-0.9.4/pygti/exceptions.py`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/pygti/gti.py` & `pygti-0.9.4/pygti/gti.py`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/pygti/schemas.py` & `pygti-0.9.4/pygti/schemas.py`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/pygti.egg-info/PKG-INFO` & `pygti-0.9.4/pygti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygti
-Version: 0.9.3
+Version: 0.9.4
 Summary: access public transport information in hamburg, germany.
 Home-page: https://github.com/vigonotion/pygti
 Author: Tom Schneider
 Author-email: mail@vigonotion.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygti Version: 0.9.3 Summary: access public
+Metadata-Version: 2.1 Name: pygti Version: 0.9.4 Summary: access public
 transport information in hamburg, germany. Home-page: https://github.com/
 vigonotion/pygti Author: Tom Schneider Author-email: mail@vigonotion.com
 License: Apache-2.0 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
```

### Comparing `pygti-0.9.3/pygti.egg-info/SOURCES.txt` & `pygti-0.9.4/pygti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/script/generate.py` & `pygti-0.9.4/script/generate.py`

 * *Files identical despite different names*

### Comparing `pygti-0.9.3/setup.py` & `pygti-0.9.4/setup.py`

 * *Files identical despite different names*

