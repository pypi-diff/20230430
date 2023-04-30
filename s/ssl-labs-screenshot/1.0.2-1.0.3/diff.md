# Comparing `tmp/ssl-labs-screenshot-1.0.2.tar.gz` & `tmp/ssl-labs-screenshot-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssl-labs-screenshot-1.0.2.tar", last modified: Sun Apr 30 20:13:28 2023, max compression
+gzip compressed data, was "ssl-labs-screenshot-1.0.3.tar", last modified: Sun Apr 30 21:25:34 2023, max compression
```

## Comparing `ssl-labs-screenshot-1.0.2.tar` & `ssl-labs-screenshot-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 20:13:28.421608 ssl-labs-screenshot-1.0.2/
--rw-r--r--   0 mark       (501) staff       (20)     1068 2023-04-30 18:51:38.000000 ssl-labs-screenshot-1.0.2/LICENSE.txt
--rw-r--r--   0 mark       (501) staff       (20)       24 2023-04-30 20:06:51.000000 ssl-labs-screenshot-1.0.2/MANIFEST.in
--rw-r--r--   0 mark       (501) staff       (20)     2445 2023-04-30 20:13:28.421470 ssl-labs-screenshot-1.0.2/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     1721 2023-04-30 18:50:26.000000 ssl-labs-screenshot-1.0.2/README.md
--rw-r--r--   0 mark       (501) staff       (20)       56 2023-04-30 20:02:02.000000 ssl-labs-screenshot-1.0.2/pyproject.toml
--rw-r--r--   0 mark       (501) staff       (20)       31 2023-04-30 18:30:24.000000 ssl-labs-screenshot-1.0.2/requirements.txt
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-30 20:13:28.421644 ssl-labs-screenshot-1.0.2/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1270 2023-04-30 20:12:00.000000 ssl-labs-screenshot-1.0.2/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 20:13:28.413117 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot/
--rw-r--r--   0 mark       (501) staff       (20)        0 2023-04-30 18:53:22.000000 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot/__init__.py
--rwxr-xr-x   0 mark       (501) staff       (20)     4104 2023-04-29 01:32:27.000000 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot/__main__.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 20:13:28.421296 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)     2445 2023-04-30 20:13:28.000000 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      398 2023-04-30 20:13:28.000000 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-30 20:13:28.000000 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)       74 2023-04-30 20:13:28.000000 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot.egg-info/entry_points.txt
--rw-r--r--   0 mark       (501) staff       (20)       32 2023-04-30 20:13:28.000000 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)       20 2023-04-30 20:13:28.000000 ssl-labs-screenshot-1.0.2/ssl_labs_screenshot.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 21:25:34.076173 ssl-labs-screenshot-1.0.3/
+-rw-r--r--   0 mark       (501) staff       (20)     1068 2023-04-30 18:51:38.000000 ssl-labs-screenshot-1.0.3/LICENSE.txt
+-rw-r--r--   0 mark       (501) staff       (20)       24 2023-04-30 20:06:51.000000 ssl-labs-screenshot-1.0.3/MANIFEST.in
+-rw-r--r--   0 mark       (501) staff       (20)     2067 2023-04-30 21:25:34.076031 ssl-labs-screenshot-1.0.3/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     1343 2023-04-30 21:24:07.000000 ssl-labs-screenshot-1.0.3/README.md
+-rw-r--r--   0 mark       (501) staff       (20)       56 2023-04-30 20:02:02.000000 ssl-labs-screenshot-1.0.3/pyproject.toml
+-rw-r--r--   0 mark       (501) staff       (20)       31 2023-04-30 18:30:24.000000 ssl-labs-screenshot-1.0.3/requirements.txt
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-30 21:25:34.076211 ssl-labs-screenshot-1.0.3/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1270 2023-04-30 21:25:25.000000 ssl-labs-screenshot-1.0.3/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 21:25:34.069847 ssl-labs-screenshot-1.0.3/ssl_labs_screenshot/
+-rw-r--r--   0 mark       (501) staff       (20)        0 2023-04-30 18:53:22.000000 ssl-labs-screenshot-1.0.3/ssl_labs_screenshot/__init__.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     4104 2023-04-29 01:32:27.000000 ssl-labs-screenshot-1.0.3/ssl_labs_screenshot/__main__.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 21:25:34.075847 ssl-labs-screenshot-1.0.3/ssl_labs_screenshot.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)     2067 2023-04-30 21:25:34.000000 ssl-labs-screenshot-1.0.3/ssl_labs_screenshot.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      398 2023-04-30 21:25:34.000000 ssl-labs-screenshot-1.0.3/ssl_labs_screenshot.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-30 21:25:34.000000 ssl-labs-screenshot-1.0.3/ssl_labs_screenshot.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)       74 2023-04-30 21:25:34.000000 ssl-labs-screenshot-1.0.3/ssl_labs_screenshot.egg-info/entry_points.txt
+-rw-r--r--   0 mark       (501) staff       (20)       32 2023-04-30 21:25:34.000000 ssl-labs-screenshot-1.0.3/ssl_labs_screenshot.egg-info/requires.txt
+-rw-r--r--   0 mark       (501) staff       (20)       20 2023-04-30 21:25:34.000000 ssl-labs-screenshot-1.0.3/ssl_labs_screenshot.egg-info/top_level.txt
```

### Comparing `ssl-labs-screenshot-1.0.2/LICENSE.txt` & `ssl-labs-screenshot-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssl-labs-screenshot-1.0.2/PKG-INFO` & `ssl-labs-screenshot-1.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssl-labs-screenshot
-Version: 1.0.2
+Version: 1.0.3
 Summary: A script to capture SSL Labs server test report screenshots
 Home-page: https://github.com/marksowell/ssl-labs-screenshot
 Author: Mark Sowell
 Author-email: mark@marksowell.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,37 +13,33 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# SSL Labs Screenshot
-This is a Python script that captures a trimmed screenshot of the SSL Labs report for a given domain, using the Selenium WebDriver and the Pillow image library.
-
-<p align="center"><img src="images/www.ssllabs.com_report.png" width="300px" />
+SSL Labs Screenshot is a Python script that captures a trimmed screenshot of the SSL Labs report for a given domain.
 
 ## Requirements
 - Python 3.x
 - Chrome browser (version 89 or later)
 - ChromeDriver
 
 ## Installation
-1. Clone this repository:   
-```git clone https://github.com/marksowell/SSL-Labs-Screenshot.git```
-2. Install the required libraries by running the following command:  
-```pip install -r requirements.txt```
+1. Install SSL Labs Screenshot using pip:   
+```
+pip install ssl-labs-screenshot
+```
 3. Download the latest version of ChromeDriver from the following link: https://sites.google.com/chromium.org/driver/downloads
 4. Extract the contents of the downloaded ZIP file to a directory on your system.
 5. Either move the ChromeDriver executable to a directory already in your system's `PATH` environment variable or add the path to the directory where you extracted the ChromeDriver executable to the `PATH` variable.
 
 ## Usage
 Run the script with the following command:  
-```python ssl-labs-screenshot.py domain.com```  
+```
+ssl-labs-screenshot.py domain.com
+```  
 
 Replace domain.com with the domain you want to test. The script will open a headless Chrome browser and load the SSL Labs report for the domain. It will capture a temporary screenshot of the report and save it as a PNG file in the same directory as the script, with the name domain_report_tmp.png. The script will delete the temporary screenshot after the trimmed image is created with the name domain_report.png
 
 ## Limitations
 The script only captures the first server's report for domains with multiple servers.
-
-## License
-The scripts and documentation in this project are released under the [MIT License](LICENSE)
```

### Comparing `ssl-labs-screenshot-1.0.2/README.md` & `ssl-labs-screenshot-1.0.3/ssl_labs_screenshot.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,45 @@
-# SSL Labs Screenshot
-This is a Python script that captures a trimmed screenshot of the SSL Labs report for a given domain, using the Selenium WebDriver and the Pillow image library.
+Metadata-Version: 2.1
+Name: ssl-labs-screenshot
+Version: 1.0.3
+Summary: A script to capture SSL Labs server test report screenshots
+Home-page: https://github.com/marksowell/ssl-labs-screenshot
+Author: Mark Sowell
+Author-email: mark@marksowell.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
-<p align="center"><img src="images/www.ssllabs.com_report.png" width="300px" />
+SSL Labs Screenshot is a Python script that captures a trimmed screenshot of the SSL Labs report for a given domain.
 
 ## Requirements
 - Python 3.x
 - Chrome browser (version 89 or later)
 - ChromeDriver
 
 ## Installation
-1. Clone this repository:   
-```git clone https://github.com/marksowell/SSL-Labs-Screenshot.git```
-2. Install the required libraries by running the following command:  
-```pip install -r requirements.txt```
+1. Install SSL Labs Screenshot using pip:   
+```
+pip install ssl-labs-screenshot
+```
 3. Download the latest version of ChromeDriver from the following link: https://sites.google.com/chromium.org/driver/downloads
 4. Extract the contents of the downloaded ZIP file to a directory on your system.
 5. Either move the ChromeDriver executable to a directory already in your system's `PATH` environment variable or add the path to the directory where you extracted the ChromeDriver executable to the `PATH` variable.
 
 ## Usage
 Run the script with the following command:  
-```python ssl-labs-screenshot.py domain.com```  
+```
+ssl-labs-screenshot.py domain.com
+```  
 
 Replace domain.com with the domain you want to test. The script will open a headless Chrome browser and load the SSL Labs report for the domain. It will capture a temporary screenshot of the report and save it as a PNG file in the same directory as the script, with the name domain_report_tmp.png. The script will delete the temporary screenshot after the trimmed image is created with the name domain_report.png
 
 ## Limitations
 The script only captures the first server's report for domains with multiple servers.
-
-## License
-The scripts and documentation in this project are released under the [MIT License](LICENSE)
```

### Comparing `ssl-labs-screenshot-1.0.2/setup.py` & `ssl-labs-screenshot-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, "requirements.txt"), "r") as fh:
     requirements = fh.read().splitlines()
 
 setup(
     name="ssl-labs-screenshot",
-    version="1.0.2",
+    version="1.0.3",
     author="Mark Sowell",
     author_email="mark@marksowell.com",
     description="A script to capture SSL Labs server test report screenshots",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/marksowell/ssl-labs-screenshot",
     packages=find_packages(),
```

### Comparing `ssl-labs-screenshot-1.0.2/ssl_labs_screenshot/__main__.py` & `ssl-labs-screenshot-1.0.3/ssl_labs_screenshot/__main__.py`

 * *Files identical despite different names*

