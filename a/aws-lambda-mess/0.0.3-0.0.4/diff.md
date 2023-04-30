# Comparing `tmp/aws_lambda_mess-0.0.3.tar.gz` & `tmp/aws_lambda_mess-0.0.4.tar.gz`

## Comparing `aws_lambda_mess-0.0.3.tar` & `aws_lambda_mess-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/__about__.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/cli.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/framework/Route.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/framework/failures.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/framework/lambda_dispatcher.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/framework/server.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/framework/success.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/init_files/.aws_lambda_mess.json
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/init_files/.gitignore
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/init_files/app.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/init_files/requirements.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/.gitignore
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/README.md
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.4/aws_lambda_mess/__about__.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.4/aws_lambda_mess/cli.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.4/aws_lambda_mess/framework/Route.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.4/aws_lambda_mess/framework/failures.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.4/aws_lambda_mess/framework/lambda_dispatcher.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.4/aws_lambda_mess/framework/server.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.4/aws_lambda_mess/framework/success.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.4/aws_lambda_mess/init_files/.aws_lambda_mess.json
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.4/aws_lambda_mess/init_files/.gitignore
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.4/aws_lambda_mess/init_files/app.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.4/aws_lambda_mess/init_files/requirements.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.4/.gitignore
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.4/README.md
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.4/PKG-INFO
```

### Comparing `aws_lambda_mess-0.0.3/aws_lambda_mess/cli.py` & `aws_lambda_mess-0.0.4/aws_lambda_mess/cli.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -42,19 +42,19 @@
         os.mkdir("./build/aws_lambda_mess")
 
     with open(CONFIG_FILE,"r") as file:
         cfg = json.load(file)
     cfg_packages = cfg.get('main', 'packages')
 
     shutil.copytree(cfg["source"], "./build/aws_lambda_mess", dirs_exist_ok=True)
-    shutil.make_archive("./dist/package", "zip", "./build/aws_lambda_mess")
 
     for package in cfg["packages"]:
         pipmain(['install', "--upgrade", "--target=./build/aws_lambda_mess/package", package])
 
+    shutil.make_archive("./dist/package", "zip", "./build/aws_lambda_mess")
 
 def run():
     import argparse
 
     parser = argparse.ArgumentParser(description="aws lambda mess")
     subparsers = parser.add_subparsers(dest='subparser')
```

### Comparing `aws_lambda_mess-0.0.3/aws_lambda_mess/framework/Route.py` & `aws_lambda_mess-0.0.4/aws_lambda_mess/framework/Route.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.3/aws_lambda_mess/framework/server.py` & `aws_lambda_mess-0.0.4/aws_lambda_mess/framework/server.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.3/aws_lambda_mess/init_files/app.py` & `aws_lambda_mess-0.0.4/aws_lambda_mess/init_files/app.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.3/pyproject.toml` & `aws_lambda_mess-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.3/PKG-INFO` & `aws_lambda_mess-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_lambda_mess
-Version: 0.0.3
+Version: 0.0.4
 Project-URL: Documentation, https://github.com/johanjordaan/aws_lambda_mess#readme
 Project-URL: Issues, https://github.com/johanjordaan/aws_lambda_mess/issues
 Project-URL: Source, https://github.com/johanjordaan/aws_lambda_mess
 Author-email: johan jordaan <djjordaan@gmail.com>
 License-Expression: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

