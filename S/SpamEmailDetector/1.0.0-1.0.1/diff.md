# Comparing `tmp/SpamEmailDetector-1.0.0.tar.gz` & `tmp/SpamEmailDetector-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpamEmailDetector-1.0.0.tar", last modified: Fri Apr 28 15:21:00 2023, max compression
+gzip compressed data, was "SpamEmailDetector-1.0.1.tar", last modified: Sun Apr 30 12:31:38 2023, max compression
```

## Comparing `SpamEmailDetector-1.0.0.tar` & `SpamEmailDetector-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yanyan     (501) staff       (20)        0 2023-04-28 15:21:00.236702 SpamEmailDetector-1.0.0/
-drwxr-xr-x   0 yanyan     (501) staff       (20)        0 2023-04-28 15:21:00.235740 SpamEmailDetector-1.0.0/Globals/
--rw-r--r--   0 yanyan     (501) staff       (20)      616 2023-04-25 01:25:27.000000 SpamEmailDetector-1.0.0/Globals/GlobalFunctions.py
--rw-r--r--   0 yanyan     (501) staff       (20)        0 2023-04-25 14:12:53.000000 SpamEmailDetector-1.0.0/Globals/__init__.py
--rw-r--r--   0 yanyan     (501) staff       (20)     1073 2023-04-27 15:52:01.000000 SpamEmailDetector-1.0.0/LICENSE.txt
--rw-r--r--   0 yanyan     (501) staff       (20)    11655 2023-04-28 15:21:00.236498 SpamEmailDetector-1.0.0/PKG-INFO
--rw-r--r--   0 yanyan     (501) staff       (20)    11051 2023-04-28 14:56:12.000000 SpamEmailDetector-1.0.0/README.md
-drwxr-xr-x   0 yanyan     (501) staff       (20)        0 2023-04-28 15:21:00.236283 SpamEmailDetector-1.0.0/SpamEmailDetector.egg-info/
--rw-r--r--   0 yanyan     (501) staff       (20)    11655 2023-04-28 15:21:00.000000 SpamEmailDetector-1.0.0/SpamEmailDetector.egg-info/PKG-INFO
--rw-r--r--   0 yanyan     (501) staff       (20)      241 2023-04-28 15:21:00.000000 SpamEmailDetector-1.0.0/SpamEmailDetector.egg-info/SOURCES.txt
--rw-r--r--   0 yanyan     (501) staff       (20)        1 2023-04-28 15:21:00.000000 SpamEmailDetector-1.0.0/SpamEmailDetector.egg-info/dependency_links.txt
--rw-r--r--   0 yanyan     (501) staff       (20)        8 2023-04-28 15:21:00.000000 SpamEmailDetector-1.0.0/SpamEmailDetector.egg-info/top_level.txt
--rw-r--r--   0 yanyan     (501) staff       (20)       38 2023-04-28 15:21:00.236747 SpamEmailDetector-1.0.0/setup.cfg
--rw-r--r--   0 yanyan     (501) staff       (20)     1193 2023-04-28 15:12:09.000000 SpamEmailDetector-1.0.0/setup.py
+drwxr-xr-x   0 yanyan     (501) staff       (20)        0 2023-04-30 12:31:38.785397 SpamEmailDetector-1.0.1/
+drwxr-xr-x   0 yanyan     (501) staff       (20)        0 2023-04-30 12:31:38.784476 SpamEmailDetector-1.0.1/Globals/
+-rw-r--r--   0 yanyan     (501) staff       (20)      616 2023-04-25 01:25:27.000000 SpamEmailDetector-1.0.1/Globals/GlobalFunctions.py
+-rw-r--r--   0 yanyan     (501) staff       (20)        0 2023-04-25 14:12:53.000000 SpamEmailDetector-1.0.1/Globals/__init__.py
+-rw-r--r--   0 yanyan     (501) staff       (20)     1073 2023-04-27 15:52:01.000000 SpamEmailDetector-1.0.1/LICENSE.txt
+-rw-r--r--   0 yanyan     (501) staff       (20)    11655 2023-04-30 12:31:38.785206 SpamEmailDetector-1.0.1/PKG-INFO
+-rw-r--r--   0 yanyan     (501) staff       (20)    11051 2023-04-28 14:56:12.000000 SpamEmailDetector-1.0.1/README.md
+drwxr-xr-x   0 yanyan     (501) staff       (20)        0 2023-04-30 12:31:38.785016 SpamEmailDetector-1.0.1/SpamEmailDetector.egg-info/
+-rw-r--r--   0 yanyan     (501) staff       (20)    11655 2023-04-30 12:31:38.000000 SpamEmailDetector-1.0.1/SpamEmailDetector.egg-info/PKG-INFO
+-rw-r--r--   0 yanyan     (501) staff       (20)      241 2023-04-30 12:31:38.000000 SpamEmailDetector-1.0.1/SpamEmailDetector.egg-info/SOURCES.txt
+-rw-r--r--   0 yanyan     (501) staff       (20)        1 2023-04-30 12:31:38.000000 SpamEmailDetector-1.0.1/SpamEmailDetector.egg-info/dependency_links.txt
+-rw-r--r--   0 yanyan     (501) staff       (20)        8 2023-04-30 12:31:38.000000 SpamEmailDetector-1.0.1/SpamEmailDetector.egg-info/top_level.txt
+-rw-r--r--   0 yanyan     (501) staff       (20)       38 2023-04-30 12:31:38.785442 SpamEmailDetector-1.0.1/setup.cfg
+-rw-r--r--   0 yanyan     (501) staff       (20)     1193 2023-04-30 12:23:07.000000 SpamEmailDetector-1.0.1/setup.py
```

### Comparing `SpamEmailDetector-1.0.0/Globals/GlobalFunctions.py` & `SpamEmailDetector-1.0.1/Globals/GlobalFunctions.py`

 * *Files identical despite different names*

### Comparing `SpamEmailDetector-1.0.0/LICENSE.txt` & `SpamEmailDetector-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SpamEmailDetector-1.0.0/PKG-INFO` & `SpamEmailDetector-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpamEmailDetector
-Version: 1.0.0
+Version: 1.0.1
 Summary: This is a package for detecting spam emails and normal emails. Codes included will continuesly listen to the provided email address, and will return message when a new email is received
 Home-page: https://github.com/NathanHuXy/SpamEmailDetector
 Author: Xueyan Hu
 Author-email: xueyanhu1231@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SpamEmailDetector-1.0.0/README.md` & `SpamEmailDetector-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `SpamEmailDetector-1.0.0/SpamEmailDetector.egg-info/PKG-INFO` & `SpamEmailDetector-1.0.1/SpamEmailDetector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpamEmailDetector
-Version: 1.0.0
+Version: 1.0.1
 Summary: This is a package for detecting spam emails and normal emails. Codes included will continuesly listen to the provided email address, and will return message when a new email is received
 Home-page: https://github.com/NathanHuXy/SpamEmailDetector
 Author: Xueyan Hu
 Author-email: xueyanhu1231@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SpamEmailDetector-1.0.0/setup.py` & `SpamEmailDetector-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SpamEmailDetector",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.0.0",  # 包版本号，便于维护版本
+    version="1.0.1",  # 包版本号，便于维护版本
     author="Xueyan Hu",  # 作者，可以写自己的姓名
     author_email="xueyanhu1231@163.com",  # 作者联系方式，可写自己的邮箱地址
     description="This is a package for detecting spam emails and normal emails. Codes included will continuesly listen to the provided email address, and will return message when a new email is received",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/NathanHuXy/SpamEmailDetector",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

