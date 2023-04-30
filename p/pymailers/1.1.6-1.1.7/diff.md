# Comparing `tmp/pymailers-1.1.6.tar.gz` & `tmp/pymailers-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymailers-1.1.6.tar", last modified: Sat Apr 29 14:38:40 2023, max compression
+gzip compressed data, was "pymailers-1.1.7.tar", last modified: Sun Apr 30 08:09:47 2023, max compression
```

## Comparing `pymailers-1.1.6.tar` & `pymailers-1.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 root         (0) permagrp2  (9997)        0 2023-04-29 14:38:40.760001 pymailers-1.1.6/
--rw-rw----   0 root         (0) permagrp2  (9997)     2211 2023-04-29 14:38:40.744001 pymailers-1.1.6/PKG-INFO
--rw-rw----   0 root         (0) permagrp2  (9997)     1089 2023-04-29 14:35:59.000000 pymailers-1.1.6/README.md
-drwxrwx---   0 root         (0) permagrp2  (9997)        0 2023-04-29 14:38:40.600000 pymailers-1.1.6/pymailers/
--rw-rw----   0 root         (0) permagrp2  (9997)     1749 2023-04-29 14:06:03.000000 pymailers-1.1.6/pymailers/PyMailer.py
--rw-rw----   0 root         (0) permagrp2  (9997)        0 2023-04-29 13:19:31.000000 pymailers-1.1.6/pymailers/__init__.py
-drwxrwx---   0 root         (0) permagrp2  (9997)        0 2023-04-29 14:38:40.720001 pymailers-1.1.6/pymailers.egg-info/
--rw-rw----   0 root         (0) permagrp2  (9997)     2211 2023-04-29 14:38:39.000000 pymailers-1.1.6/pymailers.egg-info/PKG-INFO
--rw-rw----   0 root         (0) permagrp2  (9997)      194 2023-04-29 14:38:40.000000 pymailers-1.1.6/pymailers.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) permagrp2  (9997)        1 2023-04-29 14:38:39.000000 pymailers-1.1.6/pymailers.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) permagrp2  (9997)       10 2023-04-29 14:38:39.000000 pymailers-1.1.6/pymailers.egg-info/top_level.txt
--rw-rw----   0 root         (0) permagrp2  (9997)       38 2023-04-29 14:38:40.760001 pymailers-1.1.6/setup.cfg
--rw-rw----   0 root         (0) permagrp2  (9997)     1034 2023-04-29 14:37:08.000000 pymailers-1.1.6/setup.py
+drwxrwx---   0 root         (0) permagrp2  (9997)        0 2023-04-30 08:09:47.274786 pymailers-1.1.7/
+-rw-rw----   0 root         (0) permagrp2  (9997)     2211 2023-04-30 08:09:47.262786 pymailers-1.1.7/PKG-INFO
+-rw-rw----   0 root         (0) permagrp2  (9997)     1089 2023-04-30 08:07:19.000000 pymailers-1.1.7/README.md
+drwxrwx---   0 root         (0) permagrp2  (9997)        0 2023-04-30 08:09:47.114786 pymailers-1.1.7/pymailers/
+-rw-rw----   0 root         (0) permagrp2  (9997)     1720 2023-04-30 08:07:58.000000 pymailers-1.1.7/pymailers/PyMailer.py
+-rw-rw----   0 root         (0) permagrp2  (9997)        0 2023-04-30 08:07:19.000000 pymailers-1.1.7/pymailers/__init__.py
+drwxrwx---   0 root         (0) permagrp2  (9997)        0 2023-04-30 08:09:47.230786 pymailers-1.1.7/pymailers.egg-info/
+-rw-rw----   0 root         (0) permagrp2  (9997)     2211 2023-04-30 08:09:45.000000 pymailers-1.1.7/pymailers.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) permagrp2  (9997)      194 2023-04-30 08:09:46.000000 pymailers-1.1.7/pymailers.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) permagrp2  (9997)        1 2023-04-30 08:09:46.000000 pymailers-1.1.7/pymailers.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) permagrp2  (9997)       10 2023-04-30 08:09:46.000000 pymailers-1.1.7/pymailers.egg-info/top_level.txt
+-rw-rw----   0 root         (0) permagrp2  (9997)       38 2023-04-30 08:09:47.278786 pymailers-1.1.7/setup.cfg
+-rw-rw----   0 root         (0) permagrp2  (9997)     1034 2023-04-30 08:08:12.000000 pymailers-1.1.7/setup.py
```

### Comparing `pymailers-1.1.6/PKG-INFO` & `pymailers-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymailers
-Version: 1.1.6
+Version: 1.1.7
 Summary: The classic email sending library for Python.
 Home-page: https://github.com/rioagungpurnomo/pymailers
 Author: Rio Agung Purnomo
 Author-email: rioagungpurnomo.ak@gmail.com
 License: UNKNOWN
 Description: # PyMailers
         The classic email sending library for Python.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymailers Version: 1.1.6 Summary: The classic email
+Metadata-Version: 2.1 Name: pymailers Version: 1.1.7 Summary: The classic email
 sending library for Python. Home-page: https://github.com/rioagungpurnomo/
 pymailers Author: Rio Agung Purnomo Author-email: rioagungpurnomo.ak@gmail.com
 License: UNKNOWN Description: # PyMailers The classic email sending library for
 Python. ## Installation Start to do the installation. ```bash pip install
 pymailers ``` ## Example A simple example is just sending an email message with
 PyMailer, in **display** you can replace it with **false** then it will not get
 any logs but if it is made **true** then you will get a log after sending the
```

### Comparing `pymailers-1.1.6/README.md` & `pymailers-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pymailers-1.1.6/pymailers/PyMailer.py` & `pymailers-1.1.7/pymailers/PyMailer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import smtplib
-import ExceptionType
 from sys import exit as logout
 from email.mime.text import MIMEText
 
 class PyMailer:
   def __init__(self, array):
     self.smtp_host = array['smtp_host']
     self.smtp_port = array['smtp_port']
@@ -30,22 +29,22 @@
     msg['From'] = self.email
     msg['To'] = self.to
     msg['Subject'] = self.subject
     
     try:
       with smtplib.SMTP(self.smtp_host, self.smtp_port) as smtp:
         smtp.starttls()
-    except ExceptionType:
+    except Exception:
       logout(print(f"""\n{self.failed} {self.message_smtp}{self.DEFAULT}"""))
     try:
         smtp.login(self.email, self.password)
         smtp.send_message(msg)
         if self.display:
           print(f"""\n{self.WHITE}SMTP Host : {self.smtp_host}
           SMTP Port : {self.smtp_port}
           Email : {self.email}
           To : {self.to}
           Subject : {self.subject}
           Body : {self.body}\n
           {self.success} Email sent successfully.{self.DEFAULT}""")
-    except ExceptionType:
+    except Exception:
       logout(print(f"""\n{self.failed} {self.message}{self.DEFAULT}"""))
```

### Comparing `pymailers-1.1.6/pymailers.egg-info/PKG-INFO` & `pymailers-1.1.7/pymailers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymailers
-Version: 1.1.6
+Version: 1.1.7
 Summary: The classic email sending library for Python.
 Home-page: https://github.com/rioagungpurnomo/pymailers
 Author: Rio Agung Purnomo
 Author-email: rioagungpurnomo.ak@gmail.com
 License: UNKNOWN
 Description: # PyMailers
         The classic email sending library for Python.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymailers Version: 1.1.6 Summary: The classic email
+Metadata-Version: 2.1 Name: pymailers Version: 1.1.7 Summary: The classic email
 sending library for Python. Home-page: https://github.com/rioagungpurnomo/
 pymailers Author: Rio Agung Purnomo Author-email: rioagungpurnomo.ak@gmail.com
 License: UNKNOWN Description: # PyMailers The classic email sending library for
 Python. ## Installation Start to do the installation. ```bash pip install
 pymailers ``` ## Example A simple example is just sending an email message with
 PyMailer, in **display** you can replace it with **false** then it will not get
 any logs but if it is made **true** then you will get a log after sending the
```

### Comparing `pymailers-1.1.6/setup.py` & `pymailers-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pymailers',
-    version='1.1.6',
+    version='1.1.7',
     description='The classic email sending library for Python.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Rio Agung Purnomo',
     author_email='rioagungpurnomo.ak@gmail.com',
     url='https://github.com/rioagungpurnomo/pymailers',
     packages=['pymailers'],
```

