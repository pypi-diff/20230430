# Comparing `tmp/proovl-sms-0.1.0.tar.gz` & `tmp/proovl-sms-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proovl-sms-0.1.0.tar", last modified: Sun Apr 30 15:53:18 2023, max compression
+gzip compressed data, was "proovl-sms-0.1.1.tar", last modified: Sun Apr 30 16:15:37 2023, max compression
```

## Comparing `proovl-sms-0.1.0.tar` & `proovl-sms-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 15:53:18.689862 proovl-sms-0.1.0/
--rwxrwxrwx   0 paulhome   (501) staff       (20)     1065 2023-04-30 15:28:44.000000 proovl-sms-0.1.0/LICENSE.txt
--rw-r--r--   0 paulhome   (501) staff       (20)     2551 2023-04-30 15:53:18.689672 proovl-sms-0.1.0/PKG-INFO
--rwxrwxrwx   0 paulhome   (501) staff       (20)     1790 2023-04-30 15:49:22.000000 proovl-sms-0.1.0/README.md
-drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 15:53:18.688375 proovl-sms-0.1.0/proovl-sms/
--rwxrwxrwx   0 paulhome   (501) staff       (20)       26 2023-04-30 15:23:03.000000 proovl-sms-0.1.0/proovl-sms/__init__.py
--rwxrwxrwx   0 paulhome   (501) staff       (20)     1884 2023-04-30 15:04:46.000000 proovl-sms-0.1.0/proovl-sms/proovl_sms.py
-drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 15:53:18.689387 proovl-sms-0.1.0/proovl_sms.egg-info/
--rw-r--r--   0 paulhome   (501) staff       (20)     2551 2023-04-30 15:53:18.000000 proovl-sms-0.1.0/proovl_sms.egg-info/PKG-INFO
--rw-r--r--   0 paulhome   (501) staff       (20)      247 2023-04-30 15:53:18.000000 proovl-sms-0.1.0/proovl_sms.egg-info/SOURCES.txt
--rw-r--r--   0 paulhome   (501) staff       (20)        1 2023-04-30 15:53:18.000000 proovl-sms-0.1.0/proovl_sms.egg-info/dependency_links.txt
--rw-r--r--   0 paulhome   (501) staff       (20)        9 2023-04-30 15:53:18.000000 proovl-sms-0.1.0/proovl_sms.egg-info/requires.txt
--rw-r--r--   0 paulhome   (501) staff       (20)       11 2023-04-30 15:53:18.000000 proovl-sms-0.1.0/proovl_sms.egg-info/top_level.txt
--rw-r--r--   0 paulhome   (501) staff       (20)       38 2023-04-30 15:53:18.689914 proovl-sms-0.1.0/setup.cfg
--rwxrwxrwx   0 paulhome   (501) staff       (20)      953 2023-04-30 15:15:41.000000 proovl-sms-0.1.0/setup.py
+drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 16:15:37.754902 proovl-sms-0.1.1/
+-rwxrwxrwx   0 paulhome   (501) staff       (20)     1065 2023-04-30 15:28:44.000000 proovl-sms-0.1.1/LICENSE.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)     2499 2023-04-30 16:15:37.754720 proovl-sms-0.1.1/PKG-INFO
+-rwxrwxrwx   0 paulhome   (501) staff       (20)     1738 2023-04-30 16:15:00.000000 proovl-sms-0.1.1/README.md
+drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 16:15:37.753589 proovl-sms-0.1.1/proovl-sms/
+-rwxrwxrwx   0 paulhome   (501) staff       (20)       26 2023-04-30 15:23:03.000000 proovl-sms-0.1.1/proovl-sms/__init__.py
+-rwxrwxrwx   0 paulhome   (501) staff       (20)     1884 2023-04-30 15:04:46.000000 proovl-sms-0.1.1/proovl-sms/proovl_sms.py
+drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 16:15:37.754484 proovl-sms-0.1.1/proovl_sms.egg-info/
+-rw-r--r--   0 paulhome   (501) staff       (20)     2499 2023-04-30 16:15:37.000000 proovl-sms-0.1.1/proovl_sms.egg-info/PKG-INFO
+-rw-r--r--   0 paulhome   (501) staff       (20)      247 2023-04-30 16:15:37.000000 proovl-sms-0.1.1/proovl_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)        1 2023-04-30 16:15:37.000000 proovl-sms-0.1.1/proovl_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)        9 2023-04-30 16:15:37.000000 proovl-sms-0.1.1/proovl_sms.egg-info/requires.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)       11 2023-04-30 16:15:37.000000 proovl-sms-0.1.1/proovl_sms.egg-info/top_level.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)       38 2023-04-30 16:15:37.754956 proovl-sms-0.1.1/setup.cfg
+-rwxrwxrwx   0 paulhome   (501) staff       (20)      953 2023-04-30 16:15:21.000000 proovl-sms-0.1.1/setup.py
```

### Comparing `proovl-sms-0.1.0/LICENSE.txt` & `proovl-sms-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `proovl-sms-0.1.0/PKG-INFO` & `proovl-sms-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proovl-sms
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library for sending SMS messages using Proovl API
 Home-page: https://www.proovl.com
 Author: Tomas
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -16,60 +16,58 @@
 Classifier: Topic :: Communications :: Telephony
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <h1 align="center">proovl-sms</h1>
 
-<p align="center">
+<p>
   <strong>A Python library for sending SMS messages using Proovl API</strong>
 </p>
 
 
 <h2>Installation</h2>
 
 Install using pip:
 
-```sh
-<p><python>pip install proovl-sms</python></p>
-
+<python>pip install proovl-sms<python>
 
 
 <h2>Parameters</h2>
 <p>The following parameters are required to send an SMS message:</p>
 
 <ul>
   <li><code>user</code>: Your Proovl API user ID. You can obtain this from your <a href="https://www.proovl.com">Proovl account</a>.</li>
   <li><code>token</code>: Your Proovl API authentication token. You can obtain this from your Proovl account.</li>
   <li><code>from_num</code>: The sender's name or phone number. This must be registered with Proovl. Leave this blank if you want to use the default sender name.</li>
 </ul>
 
 
-<h2>Usage</h2>
+<h2>Usage:</h2>
 
-<p><python>
+<code>
 from proovl_sms import Proovl
 
 # Initialize Proovl with your Proovl user, token, and from number
 proovl = Proovl(user='your_proovl_user', token='your_proovl_token', from_num='your_from_number')
 
 # Send a single SMS message
 response = proovl.send_sms(destination='destination_number', message='Hello, world!')
 print(response)
-</python></p>
+<code>
 
-<h2>Bulk SMS</h2>
+<h2>Bulk SMS:</h2>
 
-<p><python>
+<code>
 from proovl_sms import Proovl
 
 # Initialize Proovl with your Proovl user, token, and from numbers
 proovl = Proovl(user='your_proovl_user', token='your_proovl_token', from_num='your_from_number')
 
 # Send a bulk SMS message
 results = proovl.send_bulk_sms(destinations='destination1;destination2;destination3;destination4;destination5', message='Hello, world!')
 for result in results:
     print(result['number'], result['response'])
-</python></p>
+<code>
 
 <h2>Credits</h2>
 <p>The proovl-sms package was developed by Tomas. You can obtain your own Proovl account and API credentials from <a href="https://www.proovl.com">proovl.com</a>.</p>
```

#### html2text {}

```diff
@@ -1,37 +1,36 @@
-Metadata-Version: 2.1 Name: proovl-sms Version: 0.1.0 Summary: A Python library
+Metadata-Version: 2.1 Name: proovl-sms Version: 0.1.1 Summary: A Python library
 for sending SMS messages using Proovl API Home-page: https://www.proovl.com
 Author: Tomas Author-email: Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Topic :: Communications ::
 Telephony Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Description-Content-Type: text/markdown License-File: LICENSE.txt
                            ****** proovl-sms ******
-          A Python library for sending SMS messages using Proovl API
+A Python library for sending SMS messages using Proovl API
 ***** Installation *****
-Install using pip: ```sh
-pip install proovl-sms
+Install using pip: pip install proovl-sms
 ***** Parameters *****
 The following parameters are required to send an SMS message:
     * user: Your Proovl API user ID. You can obtain this from your Proovl
       account.
     * token: Your Proovl API authentication token. You can obtain this from
       your Proovl account.
     * from_num: The sender's name or phone number. This must be registered with
       Proovl. Leave this blank if you want to use the default sender name.
-***** Usage *****
+***** Usage: *****
 from proovl_sms import Proovl # Initialize Proovl with your Proovl user, token,
 and from number proovl = Proovl(user='your_proovl_user',
 token='your_proovl_token', from_num='your_from_number') # Send a single SMS
 message response = proovl.send_sms(destination='destination_number',
 message='Hello, world!') print(response)
-***** Bulk SMS *****
+***** Bulk SMS: *****
 from proovl_sms import Proovl # Initialize Proovl with your Proovl user, token,
 and from numbers proovl = Proovl(user='your_proovl_user',
 token='your_proovl_token', from_num='your_from_number') # Send a bulk SMS
 message results = proovl.send_bulk_sms
 (destinations='destination1;destination2;destination3;destination4;destination5',
 message='Hello, world!') for result in results: print(result['number'], result
 ['response'])
```

### Comparing `proovl-sms-0.1.0/README.md` & `proovl-sms-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 <h1 align="center">proovl-sms</h1>
 
-<p align="center">
+<p>
   <strong>A Python library for sending SMS messages using Proovl API</strong>
 </p>
 
 
 <h2>Installation</h2>
 
 Install using pip:
 
-```sh
-<p><python>pip install proovl-sms</python></p>
-
+<python>pip install proovl-sms<python>
 
 
 <h2>Parameters</h2>
 <p>The following parameters are required to send an SMS message:</p>
 
 <ul>
   <li><code>user</code>: Your Proovl API user ID. You can obtain this from your <a href="https://www.proovl.com">Proovl account</a>.</li>
   <li><code>token</code>: Your Proovl API authentication token. You can obtain this from your Proovl account.</li>
   <li><code>from_num</code>: The sender's name or phone number. This must be registered with Proovl. Leave this blank if you want to use the default sender name.</li>
 </ul>
 
 
-<h2>Usage</h2>
+<h2>Usage:</h2>
 
-<p><python>
+<code>
 from proovl_sms import Proovl
 
 # Initialize Proovl with your Proovl user, token, and from number
 proovl = Proovl(user='your_proovl_user', token='your_proovl_token', from_num='your_from_number')
 
 # Send a single SMS message
 response = proovl.send_sms(destination='destination_number', message='Hello, world!')
 print(response)
-</python></p>
+<code>
 
-<h2>Bulk SMS</h2>
+<h2>Bulk SMS:</h2>
 
-<p><python>
+<code>
 from proovl_sms import Proovl
 
 # Initialize Proovl with your Proovl user, token, and from numbers
 proovl = Proovl(user='your_proovl_user', token='your_proovl_token', from_num='your_from_number')
 
 # Send a bulk SMS message
 results = proovl.send_bulk_sms(destinations='destination1;destination2;destination3;destination4;destination5', message='Hello, world!')
 for result in results:
     print(result['number'], result['response'])
-</python></p>
+<code>
 
 <h2>Credits</h2>
 <p>The proovl-sms package was developed by Tomas. You can obtain your own Proovl account and API credentials from <a href="https://www.proovl.com">proovl.com</a>.</p>
```

#### html2text {}

```diff
@@ -1,27 +1,26 @@
                            ****** proovl-sms ******
-          A Python library for sending SMS messages using Proovl API
+A Python library for sending SMS messages using Proovl API
 ***** Installation *****
-Install using pip: ```sh
-pip install proovl-sms
+Install using pip: pip install proovl-sms
 ***** Parameters *****
 The following parameters are required to send an SMS message:
     * user: Your Proovl API user ID. You can obtain this from your Proovl
       account.
     * token: Your Proovl API authentication token. You can obtain this from
       your Proovl account.
     * from_num: The sender's name or phone number. This must be registered with
       Proovl. Leave this blank if you want to use the default sender name.
-***** Usage *****
+***** Usage: *****
 from proovl_sms import Proovl # Initialize Proovl with your Proovl user, token,
 and from number proovl = Proovl(user='your_proovl_user',
 token='your_proovl_token', from_num='your_from_number') # Send a single SMS
 message response = proovl.send_sms(destination='destination_number',
 message='Hello, world!') print(response)
-***** Bulk SMS *****
+***** Bulk SMS: *****
 from proovl_sms import Proovl # Initialize Proovl with your Proovl user, token,
 and from numbers proovl = Proovl(user='your_proovl_user',
 token='your_proovl_token', from_num='your_from_number') # Send a bulk SMS
 message results = proovl.send_bulk_sms
 (destinations='destination1;destination2;destination3;destination4;destination5',
 message='Hello, world!') for result in results: print(result['number'], result
 ['response'])
```

### Comparing `proovl-sms-0.1.0/proovl-sms/proovl_sms.py` & `proovl-sms-0.1.1/proovl-sms/proovl_sms.py`

 * *Files identical despite different names*

### Comparing `proovl-sms-0.1.0/proovl_sms.egg-info/PKG-INFO` & `proovl-sms-0.1.1/proovl_sms.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proovl-sms
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library for sending SMS messages using Proovl API
 Home-page: https://www.proovl.com
 Author: Tomas
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -16,60 +16,58 @@
 Classifier: Topic :: Communications :: Telephony
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <h1 align="center">proovl-sms</h1>
 
-<p align="center">
+<p>
   <strong>A Python library for sending SMS messages using Proovl API</strong>
 </p>
 
 
 <h2>Installation</h2>
 
 Install using pip:
 
-```sh
-<p><python>pip install proovl-sms</python></p>
-
+<python>pip install proovl-sms<python>
 
 
 <h2>Parameters</h2>
 <p>The following parameters are required to send an SMS message:</p>
 
 <ul>
   <li><code>user</code>: Your Proovl API user ID. You can obtain this from your <a href="https://www.proovl.com">Proovl account</a>.</li>
   <li><code>token</code>: Your Proovl API authentication token. You can obtain this from your Proovl account.</li>
   <li><code>from_num</code>: The sender's name or phone number. This must be registered with Proovl. Leave this blank if you want to use the default sender name.</li>
 </ul>
 
 
-<h2>Usage</h2>
+<h2>Usage:</h2>
 
-<p><python>
+<code>
 from proovl_sms import Proovl
 
 # Initialize Proovl with your Proovl user, token, and from number
 proovl = Proovl(user='your_proovl_user', token='your_proovl_token', from_num='your_from_number')
 
 # Send a single SMS message
 response = proovl.send_sms(destination='destination_number', message='Hello, world!')
 print(response)
-</python></p>
+<code>
 
-<h2>Bulk SMS</h2>
+<h2>Bulk SMS:</h2>
 
-<p><python>
+<code>
 from proovl_sms import Proovl
 
 # Initialize Proovl with your Proovl user, token, and from numbers
 proovl = Proovl(user='your_proovl_user', token='your_proovl_token', from_num='your_from_number')
 
 # Send a bulk SMS message
 results = proovl.send_bulk_sms(destinations='destination1;destination2;destination3;destination4;destination5', message='Hello, world!')
 for result in results:
     print(result['number'], result['response'])
-</python></p>
+<code>
 
 <h2>Credits</h2>
 <p>The proovl-sms package was developed by Tomas. You can obtain your own Proovl account and API credentials from <a href="https://www.proovl.com">proovl.com</a>.</p>
```

#### html2text {}

```diff
@@ -1,37 +1,36 @@
-Metadata-Version: 2.1 Name: proovl-sms Version: 0.1.0 Summary: A Python library
+Metadata-Version: 2.1 Name: proovl-sms Version: 0.1.1 Summary: A Python library
 for sending SMS messages using Proovl API Home-page: https://www.proovl.com
 Author: Tomas Author-email: Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Topic :: Communications ::
 Telephony Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Description-Content-Type: text/markdown License-File: LICENSE.txt
                            ****** proovl-sms ******
-          A Python library for sending SMS messages using Proovl API
+A Python library for sending SMS messages using Proovl API
 ***** Installation *****
-Install using pip: ```sh
-pip install proovl-sms
+Install using pip: pip install proovl-sms
 ***** Parameters *****
 The following parameters are required to send an SMS message:
     * user: Your Proovl API user ID. You can obtain this from your Proovl
       account.
     * token: Your Proovl API authentication token. You can obtain this from
       your Proovl account.
     * from_num: The sender's name or phone number. This must be registered with
       Proovl. Leave this blank if you want to use the default sender name.
-***** Usage *****
+***** Usage: *****
 from proovl_sms import Proovl # Initialize Proovl with your Proovl user, token,
 and from number proovl = Proovl(user='your_proovl_user',
 token='your_proovl_token', from_num='your_from_number') # Send a single SMS
 message response = proovl.send_sms(destination='destination_number',
 message='Hello, world!') print(response)
-***** Bulk SMS *****
+***** Bulk SMS: *****
 from proovl_sms import Proovl # Initialize Proovl with your Proovl user, token,
 and from numbers proovl = Proovl(user='your_proovl_user',
 token='your_proovl_token', from_num='your_from_number') # Send a bulk SMS
 message results = proovl.send_bulk_sms
 (destinations='destination1;destination2;destination3;destination4;destination5',
 message='Hello, world!') for result in results: print(result['number'], result
 ['response'])
```

### Comparing `proovl-sms-0.1.0/setup.py` & `proovl-sms-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='proovl-sms',
-    version='0.1.0',
+    version='0.1.1',
     author='Tomas',
     author_email='',
     description='A Python library for sending SMS messages using Proovl API',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://www.proovl.com',
     packages=find_packages(),
```

