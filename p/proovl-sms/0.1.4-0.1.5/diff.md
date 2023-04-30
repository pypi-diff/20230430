# Comparing `tmp/proovl-sms-0.1.4.tar.gz` & `tmp/proovl-sms-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proovl-sms-0.1.4.tar", last modified: Sun Apr 30 16:42:04 2023, max compression
+gzip compressed data, was "proovl-sms-0.1.5.tar", last modified: Sun Apr 30 17:09:45 2023, max compression
```

## Comparing `proovl-sms-0.1.4.tar` & `proovl-sms-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 16:42:04.754598 proovl-sms-0.1.4/
--rwxrwxrwx   0 paulhome   (501) staff       (20)     1065 2023-04-30 15:28:44.000000 proovl-sms-0.1.4/LICENSE.txt
--rw-r--r--   0 paulhome   (501) staff       (20)     2486 2023-04-30 16:42:04.754414 proovl-sms-0.1.4/PKG-INFO
--rwxrwxrwx   0 paulhome   (501) staff       (20)     1725 2023-04-30 16:41:46.000000 proovl-sms-0.1.4/README.md
-drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 16:42:04.753271 proovl-sms-0.1.4/proovl-sms/
--rwxrwxrwx   0 paulhome   (501) staff       (20)       26 2023-04-30 15:23:03.000000 proovl-sms-0.1.4/proovl-sms/__init__.py
--rwxrwxrwx   0 paulhome   (501) staff       (20)     1884 2023-04-30 15:04:46.000000 proovl-sms-0.1.4/proovl-sms/proovl_sms.py
-drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 16:42:04.754165 proovl-sms-0.1.4/proovl_sms.egg-info/
--rw-r--r--   0 paulhome   (501) staff       (20)     2486 2023-04-30 16:42:04.000000 proovl-sms-0.1.4/proovl_sms.egg-info/PKG-INFO
--rw-r--r--   0 paulhome   (501) staff       (20)      247 2023-04-30 16:42:04.000000 proovl-sms-0.1.4/proovl_sms.egg-info/SOURCES.txt
--rw-r--r--   0 paulhome   (501) staff       (20)        1 2023-04-30 16:42:04.000000 proovl-sms-0.1.4/proovl_sms.egg-info/dependency_links.txt
--rw-r--r--   0 paulhome   (501) staff       (20)        9 2023-04-30 16:42:04.000000 proovl-sms-0.1.4/proovl_sms.egg-info/requires.txt
--rw-r--r--   0 paulhome   (501) staff       (20)       11 2023-04-30 16:42:04.000000 proovl-sms-0.1.4/proovl_sms.egg-info/top_level.txt
--rw-r--r--   0 paulhome   (501) staff       (20)       38 2023-04-30 16:42:04.754650 proovl-sms-0.1.4/setup.cfg
--rwxrwxrwx   0 paulhome   (501) staff       (20)      953 2023-04-30 16:41:17.000000 proovl-sms-0.1.4/setup.py
+drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 17:09:45.273104 proovl-sms-0.1.5/
+-rwxrwxrwx   0 paulhome   (501) staff       (20)     1065 2023-04-30 15:28:44.000000 proovl-sms-0.1.5/LICENSE.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)     2486 2023-04-30 17:09:45.272913 proovl-sms-0.1.5/PKG-INFO
+-rwxrwxrwx   0 paulhome   (501) staff       (20)     1725 2023-04-30 16:41:46.000000 proovl-sms-0.1.5/README.md
+drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 17:09:45.271701 proovl-sms-0.1.5/proovl-sms/
+-rwxrwxrwx   0 paulhome   (501) staff       (20)       29 2023-04-30 17:08:58.000000 proovl-sms-0.1.5/proovl-sms/__init__.py
+-rwxrwxrwx   0 paulhome   (501) staff       (20)     1884 2023-04-30 15:04:46.000000 proovl-sms-0.1.5/proovl-sms/proovl_sms.py
+drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 17:09:45.272658 proovl-sms-0.1.5/proovl_sms.egg-info/
+-rw-r--r--   0 paulhome   (501) staff       (20)     2486 2023-04-30 17:09:45.000000 proovl-sms-0.1.5/proovl_sms.egg-info/PKG-INFO
+-rw-r--r--   0 paulhome   (501) staff       (20)      247 2023-04-30 17:09:45.000000 proovl-sms-0.1.5/proovl_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)        1 2023-04-30 17:09:45.000000 proovl-sms-0.1.5/proovl_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)        9 2023-04-30 17:09:45.000000 proovl-sms-0.1.5/proovl_sms.egg-info/requires.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)       11 2023-04-30 17:09:45.000000 proovl-sms-0.1.5/proovl_sms.egg-info/top_level.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)       38 2023-04-30 17:09:45.273171 proovl-sms-0.1.5/setup.cfg
+-rwxrwxrwx   0 paulhome   (501) staff       (20)      953 2023-04-30 17:09:06.000000 proovl-sms-0.1.5/setup.py
```

### Comparing `proovl-sms-0.1.4/LICENSE.txt` & `proovl-sms-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `proovl-sms-0.1.4/PKG-INFO` & `proovl-sms-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proovl-sms
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python library for sending SMS messages using Proovl API
 Home-page: https://www.proovl.com
 Author: Tomas
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proovl-sms Version: 0.1.4 Summary: A Python library
+Metadata-Version: 2.1 Name: proovl-sms Version: 0.1.5 Summary: A Python library
 for sending SMS messages using Proovl API Home-page: https://www.proovl.com
 Author: Tomas Author-email: Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Topic :: Communications ::
```

### Comparing `proovl-sms-0.1.4/README.md` & `proovl-sms-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `proovl-sms-0.1.4/proovl-sms/proovl_sms.py` & `proovl-sms-0.1.5/proovl-sms/proovl_sms.py`

 * *Files identical despite different names*

### Comparing `proovl-sms-0.1.4/proovl_sms.egg-info/PKG-INFO` & `proovl-sms-0.1.5/proovl_sms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proovl-sms
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python library for sending SMS messages using Proovl API
 Home-page: https://www.proovl.com
 Author: Tomas
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proovl-sms Version: 0.1.4 Summary: A Python library
+Metadata-Version: 2.1 Name: proovl-sms Version: 0.1.5 Summary: A Python library
 for sending SMS messages using Proovl API Home-page: https://www.proovl.com
 Author: Tomas Author-email: Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Topic :: Communications ::
```

### Comparing `proovl-sms-0.1.4/setup.py` & `proovl-sms-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='proovl-sms',
-    version='0.1.4',
+    version='0.1.5',
     author='Tomas',
     author_email='',
     description='A Python library for sending SMS messages using Proovl API',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://www.proovl.com',
     packages=find_packages(),
```

