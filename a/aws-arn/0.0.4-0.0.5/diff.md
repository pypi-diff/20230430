# Comparing `tmp/aws-arn-0.0.4.tar.gz` & `tmp/aws-arn-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-arn-0.0.4.tar", last modified: Sun Apr 30 13:28:46 2023, max compression
+gzip compressed data, was "aws-arn-0.0.5.tar", last modified: Sun Apr 30 13:30:51 2023, max compression
```

## Comparing `aws-arn-0.0.4.tar` & `aws-arn-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-04-30 13:28:46.049208 aws-arn-0.0.4/
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)      455 2023-04-30 13:28:46.049090 aws-arn-0.0.4/PKG-INFO
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)    48465 2023-04-30 13:20:23.000000 aws-arn-0.0.4/README.md
-drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-04-30 13:28:46.048409 aws-arn-0.0.4/aws_arn/
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)     2898 2023-04-30 12:56:06.000000 aws-arn-0.0.4/aws_arn/__init__.py
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)   157803 2023-04-30 11:54:55.000000 aws-arn-0.0.4/aws_arn/arn.py
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)     2913 2023-04-30 13:03:37.000000 aws-arn-0.0.4/aws_arn/get_parser.py
--rwxr-xr-x   0 gabrielsoltz   (501) staff       (20)     1179 2023-04-30 13:28:30.000000 aws-arn-0.0.4/aws_arn/main.py
-drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-04-30 13:28:46.048944 aws-arn-0.0.4/aws_arn.egg-info/
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)      455 2023-04-30 13:28:46.000000 aws-arn-0.0.4/aws_arn.egg-info/PKG-INFO
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)      249 2023-04-30 13:28:46.000000 aws-arn-0.0.4/aws_arn.egg-info/SOURCES.txt
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)        1 2023-04-30 13:28:46.000000 aws-arn-0.0.4/aws_arn.egg-info/dependency_links.txt
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)       33 2023-04-30 13:28:46.000000 aws-arn-0.0.4/aws_arn.egg-info/entry_points.txt
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)        8 2023-04-30 13:28:46.000000 aws-arn-0.0.4/aws_arn.egg-info/top_level.txt
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)       38 2023-04-30 13:28:46.049241 aws-arn-0.0.4/setup.cfg
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)      704 2023-04-30 13:28:39.000000 aws-arn-0.0.4/setup.py
+drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-04-30 13:30:51.479533 aws-arn-0.0.5/
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)      455 2023-04-30 13:30:51.479418 aws-arn-0.0.5/PKG-INFO
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)    48465 2023-04-30 13:20:23.000000 aws-arn-0.0.5/README.md
+drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-04-30 13:30:51.478722 aws-arn-0.0.5/aws_arn/
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)     2898 2023-04-30 12:56:06.000000 aws-arn-0.0.5/aws_arn/__init__.py
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)   157803 2023-04-30 11:54:55.000000 aws-arn-0.0.5/aws_arn/arn.py
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)     2913 2023-04-30 13:03:37.000000 aws-arn-0.0.5/aws_arn/get_parser.py
+-rwxr-xr-x   0 gabrielsoltz   (501) staff       (20)     1179 2023-04-30 13:28:30.000000 aws-arn-0.0.5/aws_arn/main.py
+drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-04-30 13:30:51.479273 aws-arn-0.0.5/aws_arn.egg-info/
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)      455 2023-04-30 13:30:51.000000 aws-arn-0.0.5/aws_arn.egg-info/PKG-INFO
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)      249 2023-04-30 13:30:51.000000 aws-arn-0.0.5/aws_arn.egg-info/SOURCES.txt
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)        1 2023-04-30 13:30:51.000000 aws-arn-0.0.5/aws_arn.egg-info/dependency_links.txt
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)       41 2023-04-30 13:30:51.000000 aws-arn-0.0.5/aws_arn.egg-info/entry_points.txt
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)        8 2023-04-30 13:30:51.000000 aws-arn-0.0.5/aws_arn.egg-info/top_level.txt
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)       38 2023-04-30 13:30:51.479564 aws-arn-0.0.5/setup.cfg
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)      712 2023-04-30 13:30:48.000000 aws-arn-0.0.5/setup.py
```

### Comparing `aws-arn-0.0.4/README.md` & `aws-arn-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aws-arn-0.0.4/aws_arn/__init__.py` & `aws-arn-0.0.5/aws_arn/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-arn-0.0.4/aws_arn/arn.py` & `aws-arn-0.0.5/aws_arn/arn.py`

 * *Files identical despite different names*

### Comparing `aws-arn-0.0.4/aws_arn/get_parser.py` & `aws-arn-0.0.5/aws_arn/get_parser.py`

 * *Files identical despite different names*

### Comparing `aws-arn-0.0.4/aws_arn/main.py` & `aws-arn-0.0.5/aws_arn/main.py`

 * *Files identical despite different names*

### Comparing `aws-arn-0.0.4/setup.py` & `aws-arn-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
     name='aws-arn',
-    version='0.0.4',
+    version='0.0.5',
     description='A library to work with AWS ARNs',
     packages=["aws_arn"],
     install_requires=[
     ],
     entry_points={
         'console_scripts': [
-            'aws-arn = main',
+            'aws-arn = aws_arn:main',
         ],
     },
     author="Gabriel Alejandro Soltz",
     author_email="gabriel@3ops.com",
     project_urls={
         "Source code": "https://github.com/gabrielsoltz/aws-arn",
     },
```

