# Comparing `tmp/requestium-0.2.0.tar.gz` & `tmp/requestium-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requestium-0.2.0.tar", last modified: Wed Mar 15 01:57:42 2023, max compression
+gzip compressed data, was "requestium-0.2.1.tar", last modified: Sun Apr 30 16:37:51 2023, max compression
```

## Comparing `requestium-0.2.0.tar` & `requestium-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jud        (501) staff       (20)        0 2023-03-15 01:57:42.543794 requestium-0.2.0/
--rw-r--r--   0 jud        (501) staff       (20)     1017 2023-03-13 21:41:14.000000 requestium-0.2.0/.travis.yml
--rw-r--r--   0 jud        (501) staff       (20)     1508 2023-03-13 21:41:14.000000 requestium-0.2.0/LICENSE
--rw-r--r--   0 jud        (501) staff       (20)      109 2023-03-14 23:31:33.000000 requestium-0.2.0/MANIFEST.in
--rw-r--r--   0 jud        (501) staff       (20)    14789 2023-03-15 01:57:42.543548 requestium-0.2.0/PKG-INFO
--rw-r--r--   0 jud        (501) staff       (20)    14105 2023-03-14 00:43:31.000000 requestium-0.2.0/README.md
-drwxr-xr-x   0 jud        (501) staff       (20)        0 2023-03-15 01:57:42.542404 requestium-0.2.0/requestium/
--rw-r--r--   0 jud        (501) staff       (20)      225 2023-03-13 21:41:14.000000 requestium-0.2.0/requestium/__init__.py
--rw-r--r--   0 jud        (501) staff       (20)    17955 2023-03-14 23:50:31.000000 requestium-0.2.0/requestium/requestium.py
-drwxr-xr-x   0 jud        (501) staff       (20)        0 2023-03-15 01:57:42.543198 requestium-0.2.0/requestium.egg-info/
--rw-r--r--   0 jud        (501) staff       (20)    14789 2023-03-15 01:57:42.000000 requestium-0.2.0/requestium.egg-info/PKG-INFO
--rw-r--r--   0 jud        (501) staff       (20)      350 2023-03-15 01:57:42.000000 requestium-0.2.0/requestium.egg-info/SOURCES.txt
--rw-r--r--   0 jud        (501) staff       (20)        1 2023-03-15 01:57:42.000000 requestium-0.2.0/requestium.egg-info/dependency_links.txt
--rw-r--r--   0 jud        (501) staff       (20)        1 2023-03-13 21:43:30.000000 requestium-0.2.0/requestium.egg-info/not-zip-safe
--rw-r--r--   0 jud        (501) staff       (20)       72 2023-03-15 01:57:42.000000 requestium-0.2.0/requestium.egg-info/requires.txt
--rw-r--r--   0 jud        (501) staff       (20)       11 2023-03-15 01:57:42.000000 requestium-0.2.0/requestium.egg-info/top_level.txt
--rw-r--r--   0 jud        (501) staff       (20)       84 2023-03-14 23:29:41.000000 requestium-0.2.0/requirements.txt
--rw-r--r--   0 jud        (501) staff       (20)       38 2023-03-15 01:57:42.543846 requestium-0.2.0/setup.cfg
--rw-r--r--   0 jud        (501) staff       (20)     1177 2023-03-14 23:27:38.000000 requestium-0.2.0/setup.py
-drwxr-xr-x   0 jud        (501) staff       (20)        0 2023-03-15 01:57:42.543321 requestium-0.2.0/tests/
--rw-r--r--   0 jud        (501) staff       (20)     1038 2023-03-14 23:26:20.000000 requestium-0.2.0/tests/test_requestium.py
--rw-r--r--   0 jud        (501) staff       (20)      209 2023-03-14 15:44:06.000000 requestium-0.2.0/tox.ini
+drwxr-xr-x   0 jud        (501) staff       (20)        0 2023-04-30 16:37:51.626762 requestium-0.2.1/
+-rw-r--r--   0 jud        (501) staff       (20)     1017 2023-03-13 21:41:14.000000 requestium-0.2.1/.travis.yml
+-rw-r--r--   0 jud        (501) staff       (20)     1508 2023-03-13 21:41:14.000000 requestium-0.2.1/LICENSE
+-rw-r--r--   0 jud        (501) staff       (20)      109 2023-03-14 23:31:33.000000 requestium-0.2.1/MANIFEST.in
+-rw-r--r--   0 jud        (501) staff       (20)    14584 2023-04-30 16:37:51.626570 requestium-0.2.1/PKG-INFO
+-rw-r--r--   0 jud        (501) staff       (20)    13900 2023-03-15 02:02:41.000000 requestium-0.2.1/README.md
+drwxr-xr-x   0 jud        (501) staff       (20)        0 2023-04-30 16:37:51.625103 requestium-0.2.1/requestium/
+-rw-r--r--   0 jud        (501) staff       (20)      225 2023-03-13 21:41:14.000000 requestium-0.2.1/requestium/__init__.py
+-rw-r--r--   0 jud        (501) staff       (20)    17955 2023-03-14 23:50:31.000000 requestium-0.2.1/requestium/requestium.py
+drwxr-xr-x   0 jud        (501) staff       (20)        0 2023-04-30 16:37:51.626161 requestium-0.2.1/requestium.egg-info/
+-rw-r--r--   0 jud        (501) staff       (20)    14584 2023-04-30 16:37:51.000000 requestium-0.2.1/requestium.egg-info/PKG-INFO
+-rw-r--r--   0 jud        (501) staff       (20)      350 2023-04-30 16:37:51.000000 requestium-0.2.1/requestium.egg-info/SOURCES.txt
+-rw-r--r--   0 jud        (501) staff       (20)        1 2023-04-30 16:37:51.000000 requestium-0.2.1/requestium.egg-info/dependency_links.txt
+-rw-r--r--   0 jud        (501) staff       (20)        1 2023-03-13 21:43:30.000000 requestium-0.2.1/requestium.egg-info/not-zip-safe
+-rw-r--r--   0 jud        (501) staff       (20)       65 2023-04-30 16:37:51.000000 requestium-0.2.1/requestium.egg-info/requires.txt
+-rw-r--r--   0 jud        (501) staff       (20)       11 2023-04-30 16:37:51.000000 requestium-0.2.1/requestium.egg-info/top_level.txt
+-rw-r--r--   0 jud        (501) staff       (20)       65 2023-03-18 18:49:49.000000 requestium-0.2.1/requirements.txt
+-rw-r--r--   0 jud        (501) staff       (20)       38 2023-04-30 16:37:51.626798 requestium-0.2.1/setup.cfg
+-rw-r--r--   0 jud        (501) staff       (20)     1172 2023-04-30 16:37:10.000000 requestium-0.2.1/setup.py
+drwxr-xr-x   0 jud        (501) staff       (20)        0 2023-04-30 16:37:51.626267 requestium-0.2.1/tests/
+-rw-r--r--   0 jud        (501) staff       (20)      889 2023-03-18 18:48:54.000000 requestium-0.2.1/tests/test_requestium.py
+-rw-r--r--   0 jud        (501) staff       (20)      209 2023-03-14 15:44:06.000000 requestium-0.2.1/tox.ini
```

### Comparing `requestium-0.2.0/.travis.yml` & `requestium-0.2.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `requestium-0.2.0/LICENSE` & `requestium-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `requestium-0.2.0/PKG-INFO` & `requestium-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requestium
-Version: 0.2.0
+Version: 0.2.1
 Summary: Adds a Selenium webdriver and parsel's parser to a request's Session object, and makes switching between them seamless. Handles cookie, proxy and header transfer.
 Home-page: https://github.com/tryolabs/requestium
 Author: Joaquin Alori
 Author-email: joaquin@tryolabs.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -45,29 +45,24 @@
 You should then download your preferred Selenium webdriver if you plan to use the Selenium part of Requestium, such as [Chromedriver](https://sites.google.com/a/chromium.org/chromedriver/).
 
 ## Usage
 First create a session as you would do on Requests, and optionally add arguments for the web-driver if you plan to use one.
 ```python
 from requestium import Session, Keys
 
-s = Session(webdriver_path='./chromedriver',
-            browser='chrome',
-            default_timeout=15,
-            webdriver_options={'arguments': ['headless']})
+options = {'arguments': ['headless']}
+s = Session(webdriver_path='./chromedriver', default_timeout=15, webdriver_options=options)
 ```
 
-Specifying `chrome-headless` as the browser type configures sensible default webdriver
-argument options when running Chrome in that mode.
+Since headless mode is common, there's a shortcut for it by pecifying `headless=True`.
 
 ```python
 from requestium import Session, Keys
 
-s = Session(webdriver_path='./chromedriver',
-            browser='chrome-headless',
-            default_timeout=15)
+s = Session(webdriver_path='./chromedriver' headless=True)
 ```
 
 You can also create a Selenium webdriver outside Requestium and have it use that instead:
 
 ```python
 from selenium import webdriver
 from requestium import Session, Keys
@@ -79,18 +74,17 @@
 
 You can also specify a 3rd party Chrome webdriver class and use it by specifying the `browser` argument as well. This will allow, for example, to use [Selenium-Wire](https://github.com/wkeeling/selenium-wire) to get XHR requests of a web page:
 
 ```python
 from seleniumwire import webdriver
 from requestium import Session, Keys
 
-s = Session(webdriver_path='./chromedriver',
-            driver_class=webdriver.Chrome,
-            browser='chrome-headless',
-            default_timeout=15)
+seleniumwire_driver = webdriver.Chrome()
+
+s = Session(webdriver_path='./chromedriver', driver=seleniumwire_driver)
 
 ```
 
 You don't need to parse the response, it is done automatically when calling xpath, css or re.
 ```python
 title = s.get('http://samplesite.com').xpath('//title/text()').extract_first(default='Default Title')
 ```
@@ -204,15 +198,15 @@
 ### Using Requestium
 ```python
 from requestium import Session, Keys
 
 # If you want requestium to type your username in the browser for you, write it in here:
 reddit_user_name = ''
 
-s = Session('./chromedriver', browser='chrome', default_timeout=15)
+s = Session('./chromedriver', default_timeout=15)
 s.driver.get('http://reddit.com')
 s.driver.find_element_by_xpath("//a[@href='https://www.reddit.com/login']").click()
 
 print('Waiting for elements to load...')
 s.driver.ensure_element_by_class_name("desktop-onboarding-sign-up__form-toggler",
 				      state='visible').click()
 
@@ -235,14 +229,15 @@
     print("Comment karma: {}".format(cmnt_karma))
     print("Reddit golds given: {}".format(reddit_golds_given))
 else:
     print("Couldn't get user name")
 ```
 
 ### Using Requests + Selenium + lxml
+
 ```python
 import re
 from lxml import etree
 from requests import Session
 from selenium import webdriver
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.common.keys import Keys
```

### Comparing `requestium-0.2.0/README.md` & `requestium-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -28,29 +28,24 @@
 You should then download your preferred Selenium webdriver if you plan to use the Selenium part of Requestium, such as [Chromedriver](https://sites.google.com/a/chromium.org/chromedriver/).
 
 ## Usage
 First create a session as you would do on Requests, and optionally add arguments for the web-driver if you plan to use one.
 ```python
 from requestium import Session, Keys
 
-s = Session(webdriver_path='./chromedriver',
-            browser='chrome',
-            default_timeout=15,
-            webdriver_options={'arguments': ['headless']})
+options = {'arguments': ['headless']}
+s = Session(webdriver_path='./chromedriver', default_timeout=15, webdriver_options=options)
 ```
 
-Specifying `chrome-headless` as the browser type configures sensible default webdriver
-argument options when running Chrome in that mode.
+Since headless mode is common, there's a shortcut for it by pecifying `headless=True`.
 
 ```python
 from requestium import Session, Keys
 
-s = Session(webdriver_path='./chromedriver',
-            browser='chrome-headless',
-            default_timeout=15)
+s = Session(webdriver_path='./chromedriver' headless=True)
 ```
 
 You can also create a Selenium webdriver outside Requestium and have it use that instead:
 
 ```python
 from selenium import webdriver
 from requestium import Session, Keys
@@ -62,18 +57,17 @@
 
 You can also specify a 3rd party Chrome webdriver class and use it by specifying the `browser` argument as well. This will allow, for example, to use [Selenium-Wire](https://github.com/wkeeling/selenium-wire) to get XHR requests of a web page:
 
 ```python
 from seleniumwire import webdriver
 from requestium import Session, Keys
 
-s = Session(webdriver_path='./chromedriver',
-            driver_class=webdriver.Chrome,
-            browser='chrome-headless',
-            default_timeout=15)
+seleniumwire_driver = webdriver.Chrome()
+
+s = Session(webdriver_path='./chromedriver', driver=seleniumwire_driver)
 
 ```
 
 You don't need to parse the response, it is done automatically when calling xpath, css or re.
 ```python
 title = s.get('http://samplesite.com').xpath('//title/text()').extract_first(default='Default Title')
 ```
@@ -187,15 +181,15 @@
 ### Using Requestium
 ```python
 from requestium import Session, Keys
 
 # If you want requestium to type your username in the browser for you, write it in here:
 reddit_user_name = ''
 
-s = Session('./chromedriver', browser='chrome', default_timeout=15)
+s = Session('./chromedriver', default_timeout=15)
 s.driver.get('http://reddit.com')
 s.driver.find_element_by_xpath("//a[@href='https://www.reddit.com/login']").click()
 
 print('Waiting for elements to load...')
 s.driver.ensure_element_by_class_name("desktop-onboarding-sign-up__form-toggler",
 				      state='visible').click()
 
@@ -218,14 +212,15 @@
     print("Comment karma: {}".format(cmnt_karma))
     print("Reddit golds given: {}".format(reddit_golds_given))
 else:
     print("Couldn't get user name")
 ```
 
 ### Using Requests + Selenium + lxml
+
 ```python
 import re
 from lxml import etree
 from requests import Session
 from selenium import webdriver
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.common.keys import Keys
```

### Comparing `requestium-0.2.0/requestium/requestium.py` & `requestium-0.2.1/requestium/requestium.py`

 * *Files identical despite different names*

### Comparing `requestium-0.2.0/requestium.egg-info/PKG-INFO` & `requestium-0.2.1/requestium.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requestium
-Version: 0.2.0
+Version: 0.2.1
 Summary: Adds a Selenium webdriver and parsel's parser to a request's Session object, and makes switching between them seamless. Handles cookie, proxy and header transfer.
 Home-page: https://github.com/tryolabs/requestium
 Author: Joaquin Alori
 Author-email: joaquin@tryolabs.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -45,29 +45,24 @@
 You should then download your preferred Selenium webdriver if you plan to use the Selenium part of Requestium, such as [Chromedriver](https://sites.google.com/a/chromium.org/chromedriver/).
 
 ## Usage
 First create a session as you would do on Requests, and optionally add arguments for the web-driver if you plan to use one.
 ```python
 from requestium import Session, Keys
 
-s = Session(webdriver_path='./chromedriver',
-            browser='chrome',
-            default_timeout=15,
-            webdriver_options={'arguments': ['headless']})
+options = {'arguments': ['headless']}
+s = Session(webdriver_path='./chromedriver', default_timeout=15, webdriver_options=options)
 ```
 
-Specifying `chrome-headless` as the browser type configures sensible default webdriver
-argument options when running Chrome in that mode.
+Since headless mode is common, there's a shortcut for it by pecifying `headless=True`.
 
 ```python
 from requestium import Session, Keys
 
-s = Session(webdriver_path='./chromedriver',
-            browser='chrome-headless',
-            default_timeout=15)
+s = Session(webdriver_path='./chromedriver' headless=True)
 ```
 
 You can also create a Selenium webdriver outside Requestium and have it use that instead:
 
 ```python
 from selenium import webdriver
 from requestium import Session, Keys
@@ -79,18 +74,17 @@
 
 You can also specify a 3rd party Chrome webdriver class and use it by specifying the `browser` argument as well. This will allow, for example, to use [Selenium-Wire](https://github.com/wkeeling/selenium-wire) to get XHR requests of a web page:
 
 ```python
 from seleniumwire import webdriver
 from requestium import Session, Keys
 
-s = Session(webdriver_path='./chromedriver',
-            driver_class=webdriver.Chrome,
-            browser='chrome-headless',
-            default_timeout=15)
+seleniumwire_driver = webdriver.Chrome()
+
+s = Session(webdriver_path='./chromedriver', driver=seleniumwire_driver)
 
 ```
 
 You don't need to parse the response, it is done automatically when calling xpath, css or re.
 ```python
 title = s.get('http://samplesite.com').xpath('//title/text()').extract_first(default='Default Title')
 ```
@@ -204,15 +198,15 @@
 ### Using Requestium
 ```python
 from requestium import Session, Keys
 
 # If you want requestium to type your username in the browser for you, write it in here:
 reddit_user_name = ''
 
-s = Session('./chromedriver', browser='chrome', default_timeout=15)
+s = Session('./chromedriver', default_timeout=15)
 s.driver.get('http://reddit.com')
 s.driver.find_element_by_xpath("//a[@href='https://www.reddit.com/login']").click()
 
 print('Waiting for elements to load...')
 s.driver.ensure_element_by_class_name("desktop-onboarding-sign-up__form-toggler",
 				      state='visible').click()
 
@@ -235,14 +229,15 @@
     print("Comment karma: {}".format(cmnt_karma))
     print("Reddit golds given: {}".format(reddit_golds_given))
 else:
     print("Couldn't get user name")
 ```
 
 ### Using Requests + Selenium + lxml
+
 ```python
 import re
 from lxml import etree
 from requests import Session
 from selenium import webdriver
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.common.keys import Keys
```

### Comparing `requestium-0.2.0/setup.py` & `requestium-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 
 # Get the long description from the README file
 with open('README.md') as file:
     long_description = file.read()
 
 setup(
     name='requestium',
-    version='0.2.0',
+    version='0.2.1',
     description=(
         "Adds a Selenium webdriver and parsel's parser to a request's Session "
         "object, and makes switching between them seamless. Handles cookie, "
         "proxy and header transfer."
     ),
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Joaquin Alori',
     author_email='joaquin@tryolabs.com',
     url='https://github.com/tryolabs/requestium',
     packages=('requestium',),
     install_requires=(
-        'requests>=2.18.1',
-        'selenium>=3.7.0,<4.0.0',
-        'parsel>=1.2.0',
-        'tldextract>=2.1.0'
+        'parsel>=1.7.0',
+        'requests>=2.28.1',
+        'selenium>=4.6.0',
+        'tldextract>=3.4.0',
     ),
     license='MIT',
     zip_safe=False,
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 3',
-    ]
+    ],
 )
```

### Comparing `requestium-0.2.0/tests/test_requestium.py` & `requestium-0.2.1/tests/test_requestium.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,32 @@
-import warnings
-
 import pytest
 import selenium
 
 import requestium
 
 
-warnings.filterwarnings('ignore', category=DeprecationWarning)
-
-
 chrome_webdriver = selenium.webdriver.chrome.webdriver.WebDriver()
 firefox_webdriver = selenium.webdriver.firefox.webdriver.WebDriver()
 
 
 session_parameters = [
     {'webdriver_path': 'chromedriver'},
     {'webdriver_path': 'chromedriver', 'headless': True},
     {'driver': chrome_webdriver},
     {'driver': firefox_webdriver},
 ]
 
 
 @pytest.fixture(params=session_parameters)
 def session(request):
-    warnings.filterwarnings('ignore', category=DeprecationWarning)
     session = requestium.Session(**request.param)
     yield session
     session.driver.close()
 
 
 def test_simple_page_load(session):
     session.driver.get('http://the-internet.herokuapp.com')
-    session.driver.ensure_element_by_id('content')
+    session.driver.ensure_element('id', 'content')
     title = session.driver.title
-    heading = session.driver.find_element_by_xpath('//*[@id="content"]/h1')
+    heading = session.driver.find_element('xpath', '//*[@id="content"]/h1')
     assert title == 'The Internet'
     assert heading.text == 'Welcome to the-internet'
```

