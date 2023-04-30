# Comparing `tmp/kk-plugins-0.0.4.tar.gz` & `tmp/kk-plugins-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kk-plugins-0.0.4.tar", last modified: Wed Apr 26 16:17:42 2023, max compression
+gzip compressed data, was "kk-plugins-0.1.0.tar", last modified: Sun Apr 30 03:03:20 2023, max compression
```

## Comparing `kk-plugins-0.0.4.tar` & `kk-plugins-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:42.639626 kk-plugins-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-26 16:17:42.639626 kk-plugins-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 16:17:42.639626 kk-plugins-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:42.635626 kk-plugins-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:42.635626 kk-plugins-0.0.4/src/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/src/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/src/cmd/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:42.635626 kk-plugins-0.0.4/src/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/src/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/src/filter/bloomfilter_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/src/filter/cuckoofilter_redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:42.639626 kk-plugins-0.0.4/src/github/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/src/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/src/github/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:42.639626 kk-plugins-0.0.4/src/kk_plugins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-26 16:17:42.000000 kk-plugins-0.0.4/src/kk_plugins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-26 16:17:42.000000 kk-plugins-0.0.4/src/kk_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:17:42.000000 kk-plugins-0.0.4/src/kk_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-26 16:17:42.000000 kk-plugins-0.0.4/src/kk_plugins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 16:17:42.000000 kk-plugins-0.0.4/src/kk_plugins.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:42.639626 kk-plugins-0.0.4/src/scrapy_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/src/scrapy_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:03:20.810913 kk-plugins-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-30 03:03:20.810913 kk-plugins-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-30 03:03:07.000000 kk-plugins-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 03:03:20.810913 kk-plugins-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-30 03:03:07.000000 kk-plugins-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:03:20.806913 kk-plugins-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:03:20.810913 kk-plugins-0.1.0/src/kk_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-30 03:03:07.000000 kk-plugins-0.1.0/src/kk_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-30 03:03:07.000000 kk-plugins-0.1.0/src/kk_plugins/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:03:20.810913 kk-plugins-0.1.0/src/kk_plugins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-30 03:03:20.000000 kk-plugins-0.1.0/src/kk_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-30 03:03:20.000000 kk-plugins-0.1.0/src/kk_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 03:03:20.000000 kk-plugins-0.1.0/src/kk_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-30 03:03:20.000000 kk-plugins-0.1.0/src/kk_plugins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 03:03:20.000000 kk-plugins-0.1.0/src/kk_plugins.egg-info/top_level.txt
```

### Comparing `kk-plugins-0.0.4/PKG-INFO` & `kk-plugins-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kk-plugins
-Version: 0.0.4
+Version: 0.1.0
 Summary: kk plugins
 Home-page: https://github.com/kk-plugins
 License: MIT
 Keywords: kk-plugins
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kk-plugins-0.0.4/setup.py` & `kk-plugins-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `kk-plugins-0.0.4/src/github/setup.py` & `kk-plugins-0.1.0/src/kk_plugins/project.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 import requests
-from jinja2 import Environment, FileSystemLoader
+from jinja2 import Template
 
 
-class SetUp:
+class StartProject:
     def __init__(self):
         self.__dir = os.getcwd()
         self.__create_github_dir()
         self.__create_workflows_dir()
         self.__create_gitignore()
         self.__create_license()
         self.__create_readme()
@@ -53,24 +53,25 @@
         if not os.path.exists(file_path):
             res = requests.get(
                 'https://gist.githubusercontent.com/wgnpj2cg/bc4ffb641cebfc76eb90dfdef2929427/raw/fa69f61dac913c932676049d00807e55f45c29d1/pre-commit').text
             with open(file_path, 'a+', encoding='utf-8') as f:
                 f.write(res)
 
     def create_python(self):
-        env = Environment(loader=FileSystemLoader(searchpath='templates'))
-        tmpl = env.get_template('python_docker_build_publish.tpl')
-        with open(os.path.join(self.__dir, '.github', 'workflows', 'python_docker_build_publish.yaml'), 'a+') as f:
-            f.write(tmpl.render())
+        # github workflows
+        tmpl = Template(requests.get(
+            'https://gist.githubusercontent.com/wgnpj2cg/479177b348504da61547df1d3925bb9e/raw/2bce40d40ead26585ac4bd473b3289e581b0699d/python_docker_build_publish.tpl').text).render()
 
+        with open(os.path.join(self.__dir, '.github', 'workflows', 'python_docker_build_publish.yaml'), 'a+') as f:
+            f.write(tmpl)
 
-# if __name__ == '__main__':
-#     su = SetUp()
-#     type = {
-#         '1': 'python',
-#         '2': 'java',
-#     }
-#     for k, v in type.items():
-#         print(k, v)
-#     t = input('please input type:')
-#     if t == '1':
-#         su.create_python()
+        # dockerfile
+        with open(os.path.join(self.__dir, "Dockerfile"), "w+") as fn:
+            fn.write(requests.get(
+                'https://gist.githubusercontent.com/wgnpj2cg/479177b348504da61547df1d3925bb9e/raw/436b447c418e586677f9fa9515631b65db4643ab/python_docker').text)
+
+        # start.py
+        start_file = os.path.join(self.__dir, 'src', 'start.py')
+        if not os.path.exists(start_file):
+            with open(start_file, 'a+', encoding='utf-8') as f:
+                f.write(requests.get(
+                    'https://gist.githubusercontent.com/wgnpj2cg/479177b348504da61547df1d3925bb9e/raw/006ce2db2b8ed4df407863afd5fbb391cb59431b/start.py').text)
```

### Comparing `kk-plugins-0.0.4/src/kk_plugins.egg-info/PKG-INFO` & `kk-plugins-0.1.0/src/kk_plugins.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kk-plugins
-Version: 0.0.4
+Version: 0.1.0
 Summary: kk plugins
 Home-page: https://github.com/kk-plugins
 License: MIT
 Keywords: kk-plugins
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

