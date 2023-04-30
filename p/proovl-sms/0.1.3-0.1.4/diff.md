# Comparing `tmp/proovl-sms-0.1.3.tar.gz` & `tmp/proovl-sms-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proovl-sms-0.1.3.tar", last modified: Sun Apr 30 16:38:59 2023, max compression
+gzip compressed data, was "proovl-sms-0.1.4.tar", last modified: Sun Apr 30 16:42:04 2023, max compression
```

## Comparing `proovl-sms-0.1.3.tar` & `proovl-sms-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 16:38:59.204518 proovl-sms-0.1.3/
--rwxrwxrwx   0 paulhome   (501) staff       (20)     1065 2023-04-30 15:28:44.000000 proovl-sms-0.1.3/LICENSE.txt
--rw-r--r--   0 paulhome   (501) staff       (20)     2511 2023-04-30 16:38:59.204330 proovl-sms-0.1.3/PKG-INFO
--rwxrwxrwx   0 paulhome   (501) staff       (20)     1750 2023-04-30 16:36:37.000000 proovl-sms-0.1.3/README.md
-drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 16:38:59.203033 proovl-sms-0.1.3/proovl-sms/
--rwxrwxrwx   0 paulhome   (501) staff       (20)       26 2023-04-30 15:23:03.000000 proovl-sms-0.1.3/proovl-sms/__init__.py
--rwxrwxrwx   0 paulhome   (501) staff       (20)     1884 2023-04-30 15:04:46.000000 proovl-sms-0.1.3/proovl-sms/proovl_sms.py
-drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 16:38:59.204049 proovl-sms-0.1.3/proovl_sms.egg-info/
--rw-r--r--   0 paulhome   (501) staff       (20)     2511 2023-04-30 16:38:59.000000 proovl-sms-0.1.3/proovl_sms.egg-info/PKG-INFO
--rw-r--r--   0 paulhome   (501) staff       (20)      247 2023-04-30 16:38:59.000000 proovl-sms-0.1.3/proovl_sms.egg-info/SOURCES.txt
--rw-r--r--   0 paulhome   (501) staff       (20)        1 2023-04-30 16:38:59.000000 proovl-sms-0.1.3/proovl_sms.egg-info/dependency_links.txt
--rw-r--r--   0 paulhome   (501) staff       (20)        9 2023-04-30 16:38:59.000000 proovl-sms-0.1.3/proovl_sms.egg-info/requires.txt
--rw-r--r--   0 paulhome   (501) staff       (20)       11 2023-04-30 16:38:59.000000 proovl-sms-0.1.3/proovl_sms.egg-info/top_level.txt
--rw-r--r--   0 paulhome   (501) staff       (20)       38 2023-04-30 16:38:59.204578 proovl-sms-0.1.3/setup.cfg
--rwxrwxrwx   0 paulhome   (501) staff       (20)      953 2023-04-30 16:38:50.000000 proovl-sms-0.1.3/setup.py
+drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 16:42:04.754598 proovl-sms-0.1.4/
+-rwxrwxrwx   0 paulhome   (501) staff       (20)     1065 2023-04-30 15:28:44.000000 proovl-sms-0.1.4/LICENSE.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)     2486 2023-04-30 16:42:04.754414 proovl-sms-0.1.4/PKG-INFO
+-rwxrwxrwx   0 paulhome   (501) staff       (20)     1725 2023-04-30 16:41:46.000000 proovl-sms-0.1.4/README.md
+drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 16:42:04.753271 proovl-sms-0.1.4/proovl-sms/
+-rwxrwxrwx   0 paulhome   (501) staff       (20)       26 2023-04-30 15:23:03.000000 proovl-sms-0.1.4/proovl-sms/__init__.py
+-rwxrwxrwx   0 paulhome   (501) staff       (20)     1884 2023-04-30 15:04:46.000000 proovl-sms-0.1.4/proovl-sms/proovl_sms.py
+drwxr-xr-x   0 paulhome   (501) staff       (20)        0 2023-04-30 16:42:04.754165 proovl-sms-0.1.4/proovl_sms.egg-info/
+-rw-r--r--   0 paulhome   (501) staff       (20)     2486 2023-04-30 16:42:04.000000 proovl-sms-0.1.4/proovl_sms.egg-info/PKG-INFO
+-rw-r--r--   0 paulhome   (501) staff       (20)      247 2023-04-30 16:42:04.000000 proovl-sms-0.1.4/proovl_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)        1 2023-04-30 16:42:04.000000 proovl-sms-0.1.4/proovl_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)        9 2023-04-30 16:42:04.000000 proovl-sms-0.1.4/proovl_sms.egg-info/requires.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)       11 2023-04-30 16:42:04.000000 proovl-sms-0.1.4/proovl_sms.egg-info/top_level.txt
+-rw-r--r--   0 paulhome   (501) staff       (20)       38 2023-04-30 16:42:04.754650 proovl-sms-0.1.4/setup.cfg
+-rwxrwxrwx   0 paulhome   (501) staff       (20)      953 2023-04-30 16:41:17.000000 proovl-sms-0.1.4/setup.py
```

### Comparing `proovl-sms-0.1.3/LICENSE.txt` & `proovl-sms-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `proovl-sms-0.1.3/PKG-INFO` & `proovl-sms-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proovl-sms
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python library for sending SMS messages using Proovl API
 Home-page: https://www.proovl.com
 Author: Tomas
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -40,38 +40,35 @@
   <li><code>token</code>: Your Proovl API authentication token. You can obtain this from your Proovl account.</li>
   <li><code>from_num</code>: The sender's name or phone number. This must be registered with Proovl. Leave this blank if you want to use the default sender name.</li>
 </ul>
 
 
 <h2>Usage:</h2>
 
-<pre>
+
 ```python
 from proovl_sms import Proovl
 
 # Initialize Proovl with your Proovl user, token, and from number
 proovl = Proovl(user='your_proovl_user', token='your_proovl_token', from_num='your_from_number')
 
 # Send a single SMS message
 response = proovl.send_sms(destination='destination_number', message='Hello, world!')
 print(response)
 ```
-</pre>
 
 <h2>Bulk SMS:</h2>
 
-<pre>
 ```python
 from proovl_sms import Proovl
 
 # Initialize Proovl with your Proovl user, token, and from numbers
 proovl = Proovl(user='your_proovl_user', token='your_proovl_token', from_num='your_from_number')
 
 # Send a bulk SMS message
 results = proovl.send_bulk_sms(destinations='destination1;destination2;destination3;destination4;destination5', message='Hello, world!')
 for result in results:
     print(result['number'], result['response'])
 ```
-</pre>
 
 <h2>Credits</h2>
 <p>The proovl-sms package was developed by Tomas. You can obtain your own Proovl account and API credentials from <a href="https://www.proovl.com">proovl.com</a>.</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proovl-sms Version: 0.1.3 Summary: A Python library
+Metadata-Version: 2.1 Name: proovl-sms Version: 0.1.4 Summary: A Python library
 for sending SMS messages using Proovl API Home-page: https://www.proovl.com
 Author: Tomas Author-email: Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Topic :: Communications ::
@@ -17,37 +17,23 @@
     * user: Your Proovl API user ID. You can obtain this from your Proovl
       account.
     * token: Your Proovl API authentication token. You can obtain this from
       your Proovl account.
     * from_num: The sender's name or phone number. This must be registered with
       Proovl. Leave this blank if you want to use the default sender name.
 ***** Usage: *****
-```python
-from proovl_sms import Proovl
-
-# Initialize Proovl with your Proovl user, token, and from number
-proovl = Proovl(user='your_proovl_user', token='your_proovl_token',
-from_num='your_from_number')
-
-# Send a single SMS message
-response = proovl.send_sms(destination='destination_number', message='Hello,
-world!')
-print(response)
-```
+```python from proovl_sms import Proovl # Initialize Proovl with your Proovl
+user, token, and from number proovl = Proovl(user='your_proovl_user',
+token='your_proovl_token', from_num='your_from_number') # Send a single SMS
+message response = proovl.send_sms(destination='destination_number',
+message='Hello, world!') print(response) ```
 ***** Bulk SMS: *****
-```python
-from proovl_sms import Proovl
-
-# Initialize Proovl with your Proovl user, token, and from numbers
-proovl = Proovl(user='your_proovl_user', token='your_proovl_token',
-from_num='your_from_number')
-
-# Send a bulk SMS message
-results = proovl.send_bulk_sms
+```python from proovl_sms import Proovl # Initialize Proovl with your Proovl
+user, token, and from numbers proovl = Proovl(user='your_proovl_user',
+token='your_proovl_token', from_num='your_from_number') # Send a bulk SMS
+message results = proovl.send_bulk_sms
 (destinations='destination1;destination2;destination3;destination4;destination5',
-message='Hello, world!')
-for result in results:
-    print(result['number'], result['response'])
-```
+message='Hello, world!') for result in results: print(result['number'], result
+['response']) ```
 ***** Credits *****
 The proovl-sms package was developed by Tomas. You can obtain your own Proovl
 account and API credentials from proovl.com.
```

### Comparing `proovl-sms-0.1.3/README.md` & `proovl-sms-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,38 +20,35 @@
   <li><code>token</code>: Your Proovl API authentication token. You can obtain this from your Proovl account.</li>
   <li><code>from_num</code>: The sender's name or phone number. This must be registered with Proovl. Leave this blank if you want to use the default sender name.</li>
 </ul>
 
 
 <h2>Usage:</h2>
 
-<pre>
+
 ```python
 from proovl_sms import Proovl
 
 # Initialize Proovl with your Proovl user, token, and from number
 proovl = Proovl(user='your_proovl_user', token='your_proovl_token', from_num='your_from_number')
 
 # Send a single SMS message
 response = proovl.send_sms(destination='destination_number', message='Hello, world!')
 print(response)
 ```
-</pre>
 
 <h2>Bulk SMS:</h2>
 
-<pre>
 ```python
 from proovl_sms import Proovl
 
 # Initialize Proovl with your Proovl user, token, and from numbers
 proovl = Proovl(user='your_proovl_user', token='your_proovl_token', from_num='your_from_number')
 
 # Send a bulk SMS message
 results = proovl.send_bulk_sms(destinations='destination1;destination2;destination3;destination4;destination5', message='Hello, world!')
 for result in results:
     print(result['number'], result['response'])
 ```
-</pre>
 
 <h2>Credits</h2>
 <p>The proovl-sms package was developed by Tomas. You can obtain your own Proovl account and API credentials from <a href="https://www.proovl.com">proovl.com</a>.</p>
```

#### html2text {}

```diff
@@ -7,37 +7,23 @@
     * user: Your Proovl API user ID. You can obtain this from your Proovl
       account.
     * token: Your Proovl API authentication token. You can obtain this from
       your Proovl account.
     * from_num: The sender's name or phone number. This must be registered with
       Proovl. Leave this blank if you want to use the default sender name.
 ***** Usage: *****
-```python
-from proovl_sms import Proovl
-
-# Initialize Proovl with your Proovl user, token, and from number
-proovl = Proovl(user='your_proovl_user', token='your_proovl_token',
-from_num='your_from_number')
-
-# Send a single SMS message
-response = proovl.send_sms(destination='destination_number', message='Hello,
-world!')
-print(response)
-```
+```python from proovl_sms import Proovl # Initialize Proovl with your Proovl
+user, token, and from number proovl = Proovl(user='your_proovl_user',
+token='your_proovl_token', from_num='your_from_number') # Send a single SMS
+message response = proovl.send_sms(destination='destination_number',
+message='Hello, world!') print(response) ```
 ***** Bulk SMS: *****
-```python
-from proovl_sms import Proovl
-
-# Initialize Proovl with your Proovl user, token, and from numbers
-proovl = Proovl(user='your_proovl_user', token='your_proovl_token',
-from_num='your_from_number')
-
-# Send a bulk SMS message
-results = proovl.send_bulk_sms
+```python from proovl_sms import Proovl # Initialize Proovl with your Proovl
+user, token, and from numbers proovl = Proovl(user='your_proovl_user',
+token='your_proovl_token', from_num='your_from_number') # Send a bulk SMS
+message results = proovl.send_bulk_sms
 (destinations='destination1;destination2;destination3;destination4;destination5',
-message='Hello, world!')
-for result in results:
-    print(result['number'], result['response'])
-```
+message='Hello, world!') for result in results: print(result['number'], result
+['response']) ```
 ***** Credits *****
 The proovl-sms package was developed by Tomas. You can obtain your own Proovl
 account and API credentials from proovl.com.
```

### Comparing `proovl-sms-0.1.3/proovl-sms/proovl_sms.py` & `proovl-sms-0.1.4/proovl-sms/proovl_sms.py`

 * *Files identical despite different names*

### Comparing `proovl-sms-0.1.3/proovl_sms.egg-info/PKG-INFO` & `proovl-sms-0.1.4/proovl_sms.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proovl-sms
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python library for sending SMS messages using Proovl API
 Home-page: https://www.proovl.com
 Author: Tomas
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -40,38 +40,35 @@
   <li><code>token</code>: Your Proovl API authentication token. You can obtain this from your Proovl account.</li>
   <li><code>from_num</code>: The sender's name or phone number. This must be registered with Proovl. Leave this blank if you want to use the default sender name.</li>
 </ul>
 
 
 <h2>Usage:</h2>
 
-<pre>
+
 ```python
 from proovl_sms import Proovl
 
 # Initialize Proovl with your Proovl user, token, and from number
 proovl = Proovl(user='your_proovl_user', token='your_proovl_token', from_num='your_from_number')
 
 # Send a single SMS message
 response = proovl.send_sms(destination='destination_number', message='Hello, world!')
 print(response)
 ```
-</pre>
 
 <h2>Bulk SMS:</h2>
 
-<pre>
 ```python
 from proovl_sms import Proovl
 
 # Initialize Proovl with your Proovl user, token, and from numbers
 proovl = Proovl(user='your_proovl_user', token='your_proovl_token', from_num='your_from_number')
 
 # Send a bulk SMS message
 results = proovl.send_bulk_sms(destinations='destination1;destination2;destination3;destination4;destination5', message='Hello, world!')
 for result in results:
     print(result['number'], result['response'])
 ```
-</pre>
 
 <h2>Credits</h2>
 <p>The proovl-sms package was developed by Tomas. You can obtain your own Proovl account and API credentials from <a href="https://www.proovl.com">proovl.com</a>.</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proovl-sms Version: 0.1.3 Summary: A Python library
+Metadata-Version: 2.1 Name: proovl-sms Version: 0.1.4 Summary: A Python library
 for sending SMS messages using Proovl API Home-page: https://www.proovl.com
 Author: Tomas Author-email: Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Topic :: Communications ::
@@ -17,37 +17,23 @@
     * user: Your Proovl API user ID. You can obtain this from your Proovl
       account.
     * token: Your Proovl API authentication token. You can obtain this from
       your Proovl account.
     * from_num: The sender's name or phone number. This must be registered with
       Proovl. Leave this blank if you want to use the default sender name.
 ***** Usage: *****
-```python
-from proovl_sms import Proovl
-
-# Initialize Proovl with your Proovl user, token, and from number
-proovl = Proovl(user='your_proovl_user', token='your_proovl_token',
-from_num='your_from_number')
-
-# Send a single SMS message
-response = proovl.send_sms(destination='destination_number', message='Hello,
-world!')
-print(response)
-```
+```python from proovl_sms import Proovl # Initialize Proovl with your Proovl
+user, token, and from number proovl = Proovl(user='your_proovl_user',
+token='your_proovl_token', from_num='your_from_number') # Send a single SMS
+message response = proovl.send_sms(destination='destination_number',
+message='Hello, world!') print(response) ```
 ***** Bulk SMS: *****
-```python
-from proovl_sms import Proovl
-
-# Initialize Proovl with your Proovl user, token, and from numbers
-proovl = Proovl(user='your_proovl_user', token='your_proovl_token',
-from_num='your_from_number')
-
-# Send a bulk SMS message
-results = proovl.send_bulk_sms
+```python from proovl_sms import Proovl # Initialize Proovl with your Proovl
+user, token, and from numbers proovl = Proovl(user='your_proovl_user',
+token='your_proovl_token', from_num='your_from_number') # Send a bulk SMS
+message results = proovl.send_bulk_sms
 (destinations='destination1;destination2;destination3;destination4;destination5',
-message='Hello, world!')
-for result in results:
-    print(result['number'], result['response'])
-```
+message='Hello, world!') for result in results: print(result['number'], result
+['response']) ```
 ***** Credits *****
 The proovl-sms package was developed by Tomas. You can obtain your own Proovl
 account and API credentials from proovl.com.
```

### Comparing `proovl-sms-0.1.3/setup.py` & `proovl-sms-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='proovl-sms',
-    version='0.1.3',
+    version='0.1.4',
     author='Tomas',
     author_email='',
     description='A Python library for sending SMS messages using Proovl API',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://www.proovl.com',
     packages=find_packages(),
```

