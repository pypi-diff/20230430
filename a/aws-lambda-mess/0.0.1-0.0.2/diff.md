# Comparing `tmp/aws_lambda_mess-0.0.1.tar.gz` & `tmp/aws_lambda_mess-0.0.2.tar.gz`

## Comparing `aws_lambda_mess-0.0.1.tar` & `aws_lambda_mess-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.1/aws_lambda_mess/__about__.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.1/aws_lambda_mess/cli.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.1/aws_lambda_mess/framework/Route.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.1/aws_lambda_mess/framework/failures.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.1/aws_lambda_mess/framework/lambda_dispatcher.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.1/aws_lambda_mess/framework/server.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.1/aws_lambda_mess/framework/success.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.1/aws_lambda_mess/init_files/.aws_lambda_mess
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.1/aws_lambda_mess/init_files/.gitignore
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.1/aws_lambda_mess/init_files/app.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.1/aws_lambda_mess/init_files/requirements.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.1/README.md
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/__about__.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/cli.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/framework/Route.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/framework/failures.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/framework/lambda_dispatcher.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/framework/server.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/framework/success.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/init_files/.aws_lambda_mess.json
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/init_files/.gitignore
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/init_files/app.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/init_files/requirements.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/.gitignore
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/README.md
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/PKG-INFO
```

### Comparing `aws_lambda_mess-0.0.1/aws_lambda_mess/cli.py` & `aws_lambda_mess-0.0.2/aws_lambda_mess/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import shutil
-from configparser import ConfigParser
+import json
 from pip._internal.cli.main import main as pipmain
 
-CONFIG_FILE = ".aws_lambda_mess"
+CONFIG_FILE = ".aws_lambda_mess.json"
 REQUIREMENTS_FILE = "requirements.txt"
 GITIGNORE_FILE = ".gitignore"
 APP_FILE = "app.py"
 
 def new(dirname):
     print('Running new', dirname)
 
@@ -44,23 +44,23 @@
         exit(1)
 
     if not os.path.isdir("./build"):
         os.mkdir("./build")
     if not os.path.isdir("./build/aws_lambda_mess"):
         os.mkdir("./build/aws_lambda_mess")
 
-    cfg = ConfigParser()
-    cfg.read(CONFIG_FILE)
-    cfg_source = cfg.get('main', 'source')
-    cfg_package = cfg.get('main', 'package')
-
-    shutil.copytree(cfg_source, "./build/aws_lambda_mess", dirs_exist_ok=True)
+    with open(CONFIG_FILE,"r") as file:
+        cfg = json.load(file)
+    cfg_packages = cfg.get('main', 'packages')
 
+    shutil.copytree(cfg["source"], "./build/aws_lambda_mess", dirs_exist_ok=True)
     shutil.make_archive("./dist/package", "zip", "./build/aws_lambda_mess")
-    pipmain(['install',"--upgrade","--target=./build/aws_lambda_mess/package","pymysql"])
+
+    for package in cfg["packages"]:
+        pipmain(['install', "--upgrade", "--target=./build/aws_lambda_mess/package", package])
 
 
 def run():
     import argparse
 
     parser = argparse.ArgumentParser(description="aws lambda mess")
     subparsers = parser.add_subparsers(dest='subparser')
```

### Comparing `aws_lambda_mess-0.0.1/aws_lambda_mess/framework/Route.py` & `aws_lambda_mess-0.0.2/aws_lambda_mess/framework/Route.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.1/aws_lambda_mess/framework/server.py` & `aws_lambda_mess-0.0.2/aws_lambda_mess/framework/server.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.1/aws_lambda_mess/init_files/app.py` & `aws_lambda_mess-0.0.2/aws_lambda_mess/init_files/app.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.1/pyproject.toml` & `aws_lambda_mess-0.0.2/pyproject.toml`

 * *Files identical despite different names*

