# Comparing `tmp/proovl-sms-0.1.1.tar.gz` & `tmp/proovl-sms-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proovl-sms-0.1.1.tar", last modified: Sun Apr 30 16:15:37 2023, max compression
+gzip compressed data, was "proovl-sms-0.1.2.tar", last modified: Sun Apr 30 16:21:40 2023, max compression
```

## Comparing `proovl-sms-0.1.1.tar` & `proovl-sms-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 16:15:37.754902 proovl-sms-0.1.1/
--rwxrwxrwx   0 paulhome   (501) staff       (20)     1065 2023-04-30 15:28:44.000000 proovl-sms-0.1.1/LICENSE.txt
--rw-r--r--   0 paulhome   (501) staff       (20)     2499 2023-04-30 16:15:37.754720 proovl-sms-0.1.1/PKG-INFO
--rwxrwxrwx   0 paulhome   (501) staff       (20)     1738 2023-04-30 16:15:00.000000 proovl-sms-0.1.1/README.md
-drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 16:15:37.753589 proovl-sms-0.1.1/proovl-sms/
--rwxrwxrwx   0 paulhome   (501) staff       (20)       26 2023-04-30 15:23:03.000000 proovl-sms-0.1.1/proovl-sms/__init__.py
--rwxrwxrwx   0 paulhome   (501) staff       (20)     1884 2023-04-30 15:04:46.000000 proovl-sms-0.1.1/proovl-sms/proovl_sms.py
-drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 16:15:37.754484 proovl-sms-0.1.1/proovl_sms.egg-info/
--rw-r--r--   0 paulhome   (501) staff       (20)     2499 2023-04-30 16:15:37.000000 proovl-sms-0.1.1/proovl_sms.egg-info/PKG-INFO
--rw-r--r--   0 paulhome   (501) staff       (20)      247 2023-04-30 16:15:37.000000 proovl-sms-0.1.1/proovl_sms.egg-info/SOURCES.txt
--rw-r--r--   0 paulhome   (501) staff       (20)        1 2023-04-30 16:15:37.000000 proovl-sms-0.1.1/proovl_sms.egg-info/dependency_links.txt
--rw-r--r--   0 paulhome   (501) staff       (20)        9 2023-04-30 16:15:37.000000 proovl-sms-0.1.1/proovl_sms.egg-info/requires.txt
--rw-r--r--   0 paulhome   (501) staff       (20)       11 2023-04-30 16:15:37.000000 proovl-sms-0.1.1/proovl_sms.egg-info/top_level.txt
--rw-r--r--   0 paulhome   (501) staff       (20)       38 2023-04-30 16:15:37.754956 proovl-sms-0.1.1/setup.cfg
--rwxrwxrwx   0 paulhome   (501) staff       (20)      953 2023-04-30 16:15:21.000000 proovl-sms-0.1.1/setup.py
+drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 16:21:40.489804 proovl-sms-0.1.2/
+-rwxrwxrwx   0 paulhome   (501) staff       (20)     1065 2023-04-30 15:28:44.000000 proovl-sms-0.1.2/LICENSE.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)     2498 2023-04-30 16:21:40.489618 proovl-sms-0.1.2/PKG-INFO
+-rwxrwxrwx   0 paulhome   (501) staff       (20)     1737 2023-04-30 16:20:35.000000 proovl-sms-0.1.2/README.md
+drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 16:21:40.488483 proovl-sms-0.1.2/proovl-sms/
+-rwxrwxrwx   0 paulhome   (501) staff       (20)       26 2023-04-30 15:23:03.000000 proovl-sms-0.1.2/proovl-sms/__init__.py
+-rwxrwxrwx   0 paulhome   (501) staff       (20)     1884 2023-04-30 15:04:46.000000 proovl-sms-0.1.2/proovl-sms/proovl_sms.py
+drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 16:21:40.489357 proovl-sms-0.1.2/proovl_sms.egg-info/
+-rw-r--r--   0 paulhome   (501) staff       (20)     2498 2023-04-30 16:21:40.000000 proovl-sms-0.1.2/proovl_sms.egg-info/PKG-INFO
+-rw-r--r--   0 paulhome   (501) staff       (20)      247 2023-04-30 16:21:40.000000 proovl-sms-0.1.2/proovl_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)        1 2023-04-30 16:21:40.000000 proovl-sms-0.1.2/proovl_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)        9 2023-04-30 16:21:40.000000 proovl-sms-0.1.2/proovl_sms.egg-info/requires.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)       11 2023-04-30 16:21:40.000000 proovl-sms-0.1.2/proovl_sms.egg-info/top_level.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)       38 2023-04-30 16:21:40.489861 proovl-sms-0.1.2/setup.cfg
+-rwxrwxrwx   0 paulhome   (501) staff       (20)      953 2023-04-30 16:21:03.000000 proovl-sms-0.1.2/setup.py
```

### Comparing `proovl-sms-0.1.1/LICENSE.txt` & `proovl-sms-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `proovl-sms-0.1.1/PKG-INFO` & `proovl-sms-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proovl-sms
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for sending SMS messages using Proovl API
 Home-page: https://www.proovl.com
 Author: Tomas
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,15 @@
 </p>
 
 
 <h2>Installation</h2>
 
 Install using pip:
 
-<python>pip install proovl-sms<python>
+<code>pip install proovl-sms</code>
 
 
 <h2>Parameters</h2>
 <p>The following parameters are required to send an SMS message:</p>
 
 <ul>
   <li><code>user</code>: Your Proovl API user ID. You can obtain this from your <a href="https://www.proovl.com">Proovl account</a>.</li>
@@ -49,25 +49,25 @@
 
 # Initialize Proovl with your Proovl user, token, and from number
 proovl = Proovl(user='your_proovl_user', token='your_proovl_token', from_num='your_from_number')
 
 # Send a single SMS message
 response = proovl.send_sms(destination='destination_number', message='Hello, world!')
 print(response)
-<code>
+</code>
 
 <h2>Bulk SMS:</h2>
 
 <code>
 from proovl_sms import Proovl
 
 # Initialize Proovl with your Proovl user, token, and from numbers
 proovl = Proovl(user='your_proovl_user', token='your_proovl_token', from_num='your_from_number')
 
 # Send a bulk SMS message
 results = proovl.send_bulk_sms(destinations='destination1;destination2;destination3;destination4;destination5', message='Hello, world!')
 for result in results:
     print(result['number'], result['response'])
-<code>
+</code>
 
 <h2>Credits</h2>
 <p>The proovl-sms package was developed by Tomas. You can obtain your own Proovl account and API credentials from <a href="https://www.proovl.com">proovl.com</a>.</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proovl-sms Version: 0.1.1 Summary: A Python library
+Metadata-Version: 2.1 Name: proovl-sms Version: 0.1.2 Summary: A Python library
 for sending SMS messages using Proovl API Home-page: https://www.proovl.com
 Author: Tomas Author-email: Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Topic :: Communications ::
```

### Comparing `proovl-sms-0.1.1/README.md` & `proovl-sms-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 </p>
 
 
 <h2>Installation</h2>
 
 Install using pip:
 
-<python>pip install proovl-sms<python>
+<code>pip install proovl-sms</code>
 
 
 <h2>Parameters</h2>
 <p>The following parameters are required to send an SMS message:</p>
 
 <ul>
   <li><code>user</code>: Your Proovl API user ID. You can obtain this from your <a href="https://www.proovl.com">Proovl account</a>.</li>
@@ -29,25 +29,25 @@
 
 # Initialize Proovl with your Proovl user, token, and from number
 proovl = Proovl(user='your_proovl_user', token='your_proovl_token', from_num='your_from_number')
 
 # Send a single SMS message
 response = proovl.send_sms(destination='destination_number', message='Hello, world!')
 print(response)
-<code>
+</code>
 
 <h2>Bulk SMS:</h2>
 
 <code>
 from proovl_sms import Proovl
 
 # Initialize Proovl with your Proovl user, token, and from numbers
 proovl = Proovl(user='your_proovl_user', token='your_proovl_token', from_num='your_from_number')
 
 # Send a bulk SMS message
 results = proovl.send_bulk_sms(destinations='destination1;destination2;destination3;destination4;destination5', message='Hello, world!')
 for result in results:
     print(result['number'], result['response'])
-<code>
+</code>
 
 <h2>Credits</h2>
 <p>The proovl-sms package was developed by Tomas. You can obtain your own Proovl account and API credentials from <a href="https://www.proovl.com">proovl.com</a>.</p>
```

### Comparing `proovl-sms-0.1.1/proovl-sms/proovl_sms.py` & `proovl-sms-0.1.2/proovl-sms/proovl_sms.py`

 * *Files identical despite different names*

### Comparing `proovl-sms-0.1.1/proovl_sms.egg-info/PKG-INFO` & `proovl-sms-0.1.2/proovl_sms.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proovl-sms
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for sending SMS messages using Proovl API
 Home-page: https://www.proovl.com
 Author: Tomas
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,15 @@
 </p>
 
 
 <h2>Installation</h2>
 
 Install using pip:
 
-<python>pip install proovl-sms<python>
+<code>pip install proovl-sms</code>
 
 
 <h2>Parameters</h2>
 <p>The following parameters are required to send an SMS message:</p>
 
 <ul>
   <li><code>user</code>: Your Proovl API user ID. You can obtain this from your <a href="https://www.proovl.com">Proovl account</a>.</li>
@@ -49,25 +49,25 @@
 
 # Initialize Proovl with your Proovl user, token, and from number
 proovl = Proovl(user='your_proovl_user', token='your_proovl_token', from_num='your_from_number')
 
 # Send a single SMS message
 response = proovl.send_sms(destination='destination_number', message='Hello, world!')
 print(response)
-<code>
+</code>
 
 <h2>Bulk SMS:</h2>
 
 <code>
 from proovl_sms import Proovl
 
 # Initialize Proovl with your Proovl user, token, and from numbers
 proovl = Proovl(user='your_proovl_user', token='your_proovl_token', from_num='your_from_number')
 
 # Send a bulk SMS message
 results = proovl.send_bulk_sms(destinations='destination1;destination2;destination3;destination4;destination5', message='Hello, world!')
 for result in results:
     print(result['number'], result['response'])
-<code>
+</code>
 
 <h2>Credits</h2>
 <p>The proovl-sms package was developed by Tomas. You can obtain your own Proovl account and API credentials from <a href="https://www.proovl.com">proovl.com</a>.</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proovl-sms Version: 0.1.1 Summary: A Python library
+Metadata-Version: 2.1 Name: proovl-sms Version: 0.1.2 Summary: A Python library
 for sending SMS messages using Proovl API Home-page: https://www.proovl.com
 Author: Tomas Author-email: Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Topic :: Communications ::
```

### Comparing `proovl-sms-0.1.1/setup.py` & `proovl-sms-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='proovl-sms',
-    version='0.1.1',
+    version='0.1.2',
     author='Tomas',
     author_email='',
     description='A Python library for sending SMS messages using Proovl API',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://www.proovl.com',
     packages=find_packages(),
```

