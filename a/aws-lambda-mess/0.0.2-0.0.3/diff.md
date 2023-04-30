# Comparing `tmp/aws_lambda_mess-0.0.2.tar.gz` & `tmp/aws_lambda_mess-0.0.3.tar.gz`

## Comparing `aws_lambda_mess-0.0.2.tar` & `aws_lambda_mess-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/__about__.py
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/cli.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/framework/Route.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/framework/failures.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/framework/lambda_dispatcher.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/framework/server.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/framework/success.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/init_files/.aws_lambda_mess.json
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/init_files/.gitignore
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/init_files/app.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/aws_lambda_mess/init_files/requirements.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/.gitignore
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/README.md
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/__about__.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/cli.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/framework/Route.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/framework/failures.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/framework/lambda_dispatcher.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/framework/server.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/framework/success.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/init_files/.aws_lambda_mess.json
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/init_files/.gitignore
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/init_files/app.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/aws_lambda_mess/init_files/requirements.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/.gitignore
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/README.md
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.3/PKG-INFO
```

### Comparing `aws_lambda_mess-0.0.2/aws_lambda_mess/cli.py` & `aws_lambda_mess-0.0.3/aws_lambda_mess/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,28 +19,21 @@
     os.chdir(dirname)
     try:
         shutil.copyfile(os.path.join(os.path.dirname(__file__), 'init_files', CONFIG_FILE), CONFIG_FILE)
         shutil.copyfile(os.path.join(os.path.dirname(__file__), 'init_files', REQUIREMENTS_FILE), REQUIREMENTS_FILE)
         shutil.copyfile(os.path.join(os.path.dirname(__file__), 'init_files', GITIGNORE_FILE), GITIGNORE_FILE)
         os.mkdir("src")
         shutil.copyfile(os.path.join(os.path.dirname(__file__), 'init_files', APP_FILE), os.path.join("src", APP_FILE))
-        os.mkdir("package")
         os.mkdir("dist")
         os.mkdir("tests")
     except Exception as e:
         print(e)
         os.chdir("..")
         exit(1)
 
-
-    #framework_dir = os.path.join(os.path.dirname(__file__), "framework")
-    #files = [file_name for file_name in os.listdir(framework_dir) if file_name not in ["__pycache__"]]
-    #for file in files:
-    #    print(f"{os.path.join(framework_dir,file)}")
-
 def build():
     print('Running build', __file__ )
     if not os.path.isfile(CONFIG_FILE):
         print("Project not initialised. Please run init")
         exit(1)
 
     if not os.path.isdir("./build"):
```

### Comparing `aws_lambda_mess-0.0.2/aws_lambda_mess/framework/Route.py` & `aws_lambda_mess-0.0.3/aws_lambda_mess/framework/Route.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.2/aws_lambda_mess/framework/server.py` & `aws_lambda_mess-0.0.3/aws_lambda_mess/framework/server.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.2/pyproject.toml` & `aws_lambda_mess-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.2/PKG-INFO` & `aws_lambda_mess-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_lambda_mess
-Version: 0.0.2
+Version: 0.0.3
 Project-URL: Documentation, https://github.com/johanjordaan/aws_lambda_mess#readme
 Project-URL: Issues, https://github.com/johanjordaan/aws_lambda_mess/issues
 Project-URL: Source, https://github.com/johanjordaan/aws_lambda_mess
 Author-email: johan jordaan <djjordaan@gmail.com>
 License-Expression: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

