# Comparing `tmp/pycryptokms-0.0.3.tar.gz` & `tmp/pycryptokms-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycryptokms-0.0.3.tar", last modified: Sun Apr 30 17:03:24 2023, max compression
+gzip compressed data, was "pycryptokms-0.0.5.tar", last modified: Sun Apr 30 18:28:24 2023, max compression
```

## Comparing `pycryptokms-0.0.3.tar` & `pycryptokms-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 kapkiai   (1000) kapkiai   (1000)        0 2023-04-30 17:03:24.753834 pycryptokms-0.0.3/
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      584 2023-04-30 13:31:01.000000 pycryptokms-0.0.3/LICENCE
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      256 2023-04-30 14:26:51.000000 pycryptokms-0.0.3/MANIFEST.in
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)       44 2023-04-30 14:29:58.000000 pycryptokms-0.0.3/NOTICE
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)     1928 2023-04-30 17:03:24.753834 pycryptokms-0.0.3/PKG-INFO
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      692 2023-04-30 17:00:53.000000 pycryptokms-0.0.3/README.rst
-drwxrwxr-x   0 kapkiai   (1000) kapkiai   (1000)        0 2023-04-30 17:03:24.753834 pycryptokms-0.0.3/docs/
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)     6769 2023-04-30 14:03:07.000000 pycryptokms-0.0.3/docs/Makefile
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      133 2023-04-30 13:57:17.000000 pycryptokms-0.0.3/docs/authors.rst
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)     8802 2023-04-30 15:01:13.000000 pycryptokms-0.0.3/docs/conf.py
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)     3505 2023-04-30 16:00:39.000000 pycryptokms-0.0.3/docs/contributing.rst
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      100 2023-04-30 14:49:36.000000 pycryptokms-0.0.3/docs/devnotes.rst
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)       92 2023-04-30 14:22:19.000000 pycryptokms-0.0.3/docs/history.rst
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      540 2023-04-30 14:46:02.000000 pycryptokms-0.0.3/docs/index.rst
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)     1121 2023-04-30 13:53:55.000000 pycryptokms-0.0.3/docs/installation.rst
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      800 2023-04-30 14:07:49.000000 pycryptokms-0.0.3/docs/make.bat
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)       64 2023-04-30 14:49:37.000000 pycryptokms-0.0.3/docs/modules.rst
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      356 2023-04-30 14:45:14.000000 pycryptokms-0.0.3/docs/py_crypto.crypto.rst
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      329 2023-04-30 14:45:14.000000 pycryptokms-0.0.3/docs/py_crypto.kms.rst
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      407 2023-04-30 14:45:14.000000 pycryptokms-0.0.3/docs/py_crypto.rst
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)       26 2023-04-30 13:54:19.000000 pycryptokms-0.0.3/docs/readme.rst
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      134 2023-04-30 16:08:47.000000 pycryptokms-0.0.3/docs/todo.rst
-drwxrwxr-x   0 kapkiai   (1000) kapkiai   (1000)        0 2023-04-30 17:03:24.753834 pycryptokms-0.0.3/py_crypto/
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)        0 2023-04-30 12:06:24.000000 pycryptokms-0.0.3/py_crypto/__init__.py
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      253 2023-04-30 12:12:43.000000 pycryptokms-0.0.3/py_crypto/config.py
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)     3031 2023-04-30 15:35:11.000000 pycryptokms-0.0.3/py_crypto/crypto.py
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)     2495 2023-04-30 16:58:51.000000 pycryptokms-0.0.3/py_crypto/kms.py
-drwxrwxr-x   0 kapkiai   (1000) kapkiai   (1000)        0 2023-04-30 17:03:24.753834 pycryptokms-0.0.3/pycryptokms.egg-info/
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)     1928 2023-04-30 17:03:24.000000 pycryptokms-0.0.3/pycryptokms.egg-info/PKG-INFO
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      627 2023-04-30 17:03:24.000000 pycryptokms-0.0.3/pycryptokms.egg-info/SOURCES.txt
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)        1 2023-04-30 17:03:24.000000 pycryptokms-0.0.3/pycryptokms.egg-info/dependency_links.txt
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)        1 2023-04-30 17:03:24.000000 pycryptokms-0.0.3/pycryptokms.egg-info/not-zip-safe
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)       46 2023-04-30 17:03:24.000000 pycryptokms-0.0.3/pycryptokms.egg-info/requires.txt
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)       10 2023-04-30 17:03:24.000000 pycryptokms-0.0.3/pycryptokms.egg-info/top_level.txt
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)       74 2023-04-30 16:51:53.000000 pycryptokms-0.0.3/requirements.txt
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      420 2023-04-30 17:03:24.757834 pycryptokms-0.0.3/setup.cfg
--rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)     1829 2023-04-30 17:01:04.000000 pycryptokms-0.0.3/setup.py
+drwxrwxr-x   0 kapkiai   (1000) kapkiai   (1000)        0 2023-04-30 18:28:24.792295 pycryptokms-0.0.5/
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      584 2023-04-30 13:31:01.000000 pycryptokms-0.0.5/LICENCE
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      256 2023-04-30 14:26:51.000000 pycryptokms-0.0.5/MANIFEST.in
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)       44 2023-04-30 14:29:58.000000 pycryptokms-0.0.5/NOTICE
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)     2136 2023-04-30 18:28:24.792295 pycryptokms-0.0.5/PKG-INFO
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      692 2023-04-30 17:00:53.000000 pycryptokms-0.0.5/README.rst
+drwxrwxr-x   0 kapkiai   (1000) kapkiai   (1000)        0 2023-04-30 18:28:24.792295 pycryptokms-0.0.5/docs/
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)     6769 2023-04-30 14:03:07.000000 pycryptokms-0.0.5/docs/Makefile
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      133 2023-04-30 13:57:17.000000 pycryptokms-0.0.5/docs/authors.rst
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)     8802 2023-04-30 15:01:13.000000 pycryptokms-0.0.5/docs/conf.py
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)     3505 2023-04-30 16:00:39.000000 pycryptokms-0.0.5/docs/contributing.rst
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      100 2023-04-30 14:49:36.000000 pycryptokms-0.0.5/docs/devnotes.rst
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      300 2023-04-30 18:08:21.000000 pycryptokms-0.0.5/docs/history.rst
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      540 2023-04-30 14:46:02.000000 pycryptokms-0.0.5/docs/index.rst
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)     1121 2023-04-30 13:53:55.000000 pycryptokms-0.0.5/docs/installation.rst
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      800 2023-04-30 14:07:49.000000 pycryptokms-0.0.5/docs/make.bat
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)       64 2023-04-30 14:49:37.000000 pycryptokms-0.0.5/docs/modules.rst
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      356 2023-04-30 14:45:14.000000 pycryptokms-0.0.5/docs/py_crypto.crypto.rst
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      329 2023-04-30 14:45:14.000000 pycryptokms-0.0.5/docs/py_crypto.kms.rst
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      407 2023-04-30 14:45:14.000000 pycryptokms-0.0.5/docs/py_crypto.rst
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)       26 2023-04-30 13:54:19.000000 pycryptokms-0.0.5/docs/readme.rst
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      134 2023-04-30 16:08:47.000000 pycryptokms-0.0.5/docs/todo.rst
+drwxrwxr-x   0 kapkiai   (1000) kapkiai   (1000)        0 2023-04-30 18:28:24.792295 pycryptokms-0.0.5/py_crypto/
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)        0 2023-04-30 12:06:24.000000 pycryptokms-0.0.5/py_crypto/__init__.py
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      253 2023-04-30 12:12:43.000000 pycryptokms-0.0.5/py_crypto/config.py
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)     3031 2023-04-30 15:35:11.000000 pycryptokms-0.0.5/py_crypto/crypto.py
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)     2575 2023-04-30 18:25:24.000000 pycryptokms-0.0.5/py_crypto/kms.py
+drwxrwxr-x   0 kapkiai   (1000) kapkiai   (1000)        0 2023-04-30 18:28:24.792295 pycryptokms-0.0.5/pycryptokms.egg-info/
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)     2136 2023-04-30 18:28:24.000000 pycryptokms-0.0.5/pycryptokms.egg-info/PKG-INFO
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      627 2023-04-30 18:28:24.000000 pycryptokms-0.0.5/pycryptokms.egg-info/SOURCES.txt
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)        1 2023-04-30 18:28:24.000000 pycryptokms-0.0.5/pycryptokms.egg-info/dependency_links.txt
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)        1 2023-04-30 18:28:24.000000 pycryptokms-0.0.5/pycryptokms.egg-info/not-zip-safe
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)       46 2023-04-30 18:28:24.000000 pycryptokms-0.0.5/pycryptokms.egg-info/requires.txt
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)       10 2023-04-30 18:28:24.000000 pycryptokms-0.0.5/pycryptokms.egg-info/top_level.txt
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)       74 2023-04-30 18:01:21.000000 pycryptokms-0.0.5/requirements.txt
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)      420 2023-04-30 18:28:24.796293 pycryptokms-0.0.5/setup.cfg
+-rw-rw-r--   0 kapkiai   (1000) kapkiai   (1000)     1829 2023-04-30 18:28:23.000000 pycryptokms-0.0.5/setup.py
```

### Comparing `pycryptokms-0.0.3/LICENCE` & `pycryptokms-0.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `pycryptokms-0.0.3/PKG-INFO` & `pycryptokms-0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pycryptokms
-Version: 0.0.3
+Version: 0.0.5
 Summary: PyCrypto: A convenient Python wrapper for the KMS and various cryptographic algorithms
 Home-page: https://github.com/kapkiai/pycrypto
 Author: Mathew Kiprop
 Author-email: mathewkiprop17@gmail.com
 License: Apache Software License 2.0
-Download-URL: https://github.com/kapkiai/pycrypto/archive/0.0.3.tar.gz
+Download-URL: https://github.com/kapkiai/pycrypto/archive/0.0.5.tar.gz
 Keywords: cryptography,kms,wrapper
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
@@ -57,12 +57,24 @@
 
 
 
 =======
 History
 =======
 
-0.0.1 (2023-04-30)
+0.0.4 (2023-04-30)
+------------------
+
+* Bumped down requests library version to 2.25.0.
+
+0.0.3 (2023-04-30)
+------------------
+
+* StepKMSProvider implementation
+* Initial work in file and ranger providers
+
+0.0.2 (2023-04-30)
 ------------------
 
 * First release on PyCrypto.
 
+
```

### Comparing `pycryptokms-0.0.3/README.rst` & `pycryptokms-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `pycryptokms-0.0.3/docs/Makefile` & `pycryptokms-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pycryptokms-0.0.3/docs/conf.py` & `pycryptokms-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pycryptokms-0.0.3/docs/contributing.rst` & `pycryptokms-0.0.5/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `pycryptokms-0.0.3/docs/index.rst` & `pycryptokms-0.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pycryptokms-0.0.3/docs/installation.rst` & `pycryptokms-0.0.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pycryptokms-0.0.3/docs/make.bat` & `pycryptokms-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pycryptokms-0.0.3/py_crypto/crypto.py` & `pycryptokms-0.0.5/py_crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `pycryptokms-0.0.3/py_crypto/kms.py` & `pycryptokms-0.0.5/py_crypto/kms.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 
     @lru_cache(maxsize=10)
     def get_encryption_key(self, key_identifier: str) -> str:
         try:
             session = requests.Session()
             # TODO: Look for a way to disable this
             session.verify = False
-            response = session.get(url=self.key_url, params={'id': key_identifier, 'username': 'hive'}, timeout=300)
+            response = session.get(url=self.key_url, auth=(self.kms_username, self.kms_password),
+                                   params={'id': key_identifier, 'username': 'hive'}, timeout=300)
             kms_res = response.json()
             return kms_res['key']
         except Exception as e:
             self.log.error('Could not retrieve key from kms due to %s', e)
             raise e
```

### Comparing `pycryptokms-0.0.3/pycryptokms.egg-info/PKG-INFO` & `pycryptokms-0.0.5/pycryptokms.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pycryptokms
-Version: 0.0.3
+Version: 0.0.5
 Summary: PyCrypto: A convenient Python wrapper for the KMS and various cryptographic algorithms
 Home-page: https://github.com/kapkiai/pycrypto
 Author: Mathew Kiprop
 Author-email: mathewkiprop17@gmail.com
 License: Apache Software License 2.0
-Download-URL: https://github.com/kapkiai/pycrypto/archive/0.0.3.tar.gz
+Download-URL: https://github.com/kapkiai/pycrypto/archive/0.0.5.tar.gz
 Keywords: cryptography,kms,wrapper
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
@@ -57,12 +57,24 @@
 
 
 
 =======
 History
 =======
 
-0.0.1 (2023-04-30)
+0.0.4 (2023-04-30)
+------------------
+
+* Bumped down requests library version to 2.25.0.
+
+0.0.3 (2023-04-30)
+------------------
+
+* StepKMSProvider implementation
+* Initial work in file and ranger providers
+
+0.0.2 (2023-04-30)
 ------------------
 
 * First release on PyCrypto.
 
+
```

### Comparing `pycryptokms-0.0.3/pycryptokms.egg-info/SOURCES.txt` & `pycryptokms-0.0.5/pycryptokms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycryptokms-0.0.3/setup.py` & `pycryptokms-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('docs/history.rst') as history_file:
     history = history_file.read()
 
-proj_version = '0.0.3'
+proj_version = '0.0.5'
 
 with open('requirements.txt') as reqs_file:
     requirements = reqs_file.read().splitlines()
 
 setup(
     name='pycryptokms',
     version=proj_version,
```

