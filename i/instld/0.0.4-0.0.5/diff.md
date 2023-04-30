# Comparing `tmp/instld-0.0.4.tar.gz` & `tmp/instld-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instld-0.0.4.tar", last modified: Sat Apr  8 08:57:34 2023, max compression
+gzip compressed data, was "instld-0.0.5.tar", last modified: Sun Apr 30 11:55:42 2023, max compression
```

## Comparing `instld-0.0.4.tar` & `instld-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,22 @@
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-08 08:57:34.992448 instld-0.0.4/
--rw-r--r--   0 pomponchik   (501) staff       (20)     1067 2023-04-02 20:16:05.000000 instld-0.0.4/LICENSE
--rw-r--r--   0 pomponchik   (501) staff       (20)     2069 2023-04-08 08:57:34.992323 instld-0.0.4/PKG-INFO
--rw-r--r--   0 pomponchik   (501) staff       (20)     1448 2023-04-08 08:54:23.000000 instld-0.0.4/README.md
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-08 08:57:34.991410 instld-0.0.4/installed/
--rw-r--r--   0 pomponchik   (501) staff       (20)     1624 2023-04-08 08:51:06.000000 instld-0.0.4/installed/__init__.py
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-08 08:57:34.992128 instld-0.0.4/instld.egg-info/
--rw-r--r--   0 pomponchik   (501) staff       (20)     2069 2023-04-08 08:57:34.000000 instld-0.0.4/instld.egg-info/PKG-INFO
--rw-r--r--   0 pomponchik   (501) staff       (20)      168 2023-04-08 08:57:34.000000 instld-0.0.4/instld.egg-info/SOURCES.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)        1 2023-04-08 08:57:34.000000 instld-0.0.4/instld.egg-info/dependency_links.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)       10 2023-04-08 08:57:34.000000 instld-0.0.4/instld.egg-info/top_level.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)       38 2023-04-08 08:57:34.992499 instld-0.0.4/setup.cfg
--rw-r--r--   0 pomponchik   (501) staff       (20)      865 2023-04-08 08:52:43.000000 instld-0.0.4/setup.py
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 11:55:42.715731 instld-0.0.5/
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1067 2023-04-02 20:16:05.000000 instld-0.0.5/LICENSE
+-rw-r--r--   0 pomponchik   (501) staff       (20)     2029 2023-04-30 11:55:42.715466 instld-0.0.5/PKG-INFO
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1445 2023-04-09 18:09:35.000000 instld-0.0.5/README.md
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 11:55:42.713474 instld-0.0.5/installed/
+-rw-r--r--   0 pomponchik   (501) staff       (20)      107 2023-04-29 15:51:00.000000 instld-0.0.5/installed/__init__.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1326 2023-04-29 21:56:56.000000 instld-0.0.5/installed/context_manager.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)      239 2023-04-30 11:52:44.000000 instld-0.0.5/installed/empty_logger.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)       50 2023-04-29 15:42:44.000000 instld-0.0.5/installed/errors.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)      415 2023-04-29 21:55:47.000000 instld-0.0.5/installed/proxy_module.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)      737 2023-04-30 11:53:49.000000 instld-0.0.5/installed/runner.py
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 11:55:42.714400 instld-0.0.5/instld.egg-info/
+-rw-r--r--   0 pomponchik   (501) staff       (20)     2029 2023-04-30 11:55:42.000000 instld-0.0.5/instld.egg-info/PKG-INFO
+-rw-r--r--   0 pomponchik   (501) staff       (20)      340 2023-04-30 11:55:42.000000 instld-0.0.5/instld.egg-info/SOURCES.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)        1 2023-04-30 11:55:42.000000 instld-0.0.5/instld.egg-info/dependency_links.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)       16 2023-04-30 11:55:42.000000 instld-0.0.5/instld.egg-info/top_level.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)       38 2023-04-30 11:55:42.715806 instld-0.0.5/setup.cfg
+-rw-r--r--   0 pomponchik   (501) staff       (20)      865 2023-04-29 15:41:33.000000 instld-0.0.5/setup.py
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 11:55:42.710887 instld-0.0.5/tests/
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 11:55:42.714836 instld-0.0.5/tests/units/
+-rw-r--r--   0 pomponchik   (501) staff       (20)        0 2023-04-29 15:45:14.000000 instld-0.0.5/tests/units/__init__.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)       52 2023-04-29 15:52:00.000000 instld-0.0.5/tests/units/test_errors.py
```

### Comparing `instld-0.0.4/LICENSE` & `instld-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `instld-0.0.4/PKG-INFO` & `instld-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: instld
-Version: 0.0.4
+Version: 0.0.5
 Summary: The simplest package management from the source code
 Home-page: https://github.com/pomponchik/installed
 Author: Evgeniy Blinov
 Author-email: zheni-b@yandex.ru
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # INSTALLED: the simplest package management from the source code
 
 [![Downloads](https://pepy.tech/badge/instld/month)](https://pepy.tech/project/instld)
-[![Downloads](https://pepy.tech/badge/instld)](https://pepy.tech/project/installed)
+[![Downloads](https://pepy.tech/badge/instld)](https://pepy.tech/project/instld)
 [![codecov](https://codecov.io/gh/pomponchik/installed/branch/main/graph/badge.svg)](https://codecov.io/gh/pomponchik/installed)
 [![Test-Package](https://github.com/pomponchik/installed/actions/workflows/coverage.yml/badge.svg)](https://github.com/pomponchik/installed/actions/workflows/coverage.yml)
 [![Python versions](https://img.shields.io/pypi/pyversions/instld.svg)](https://pypi.python.org/pypi/instld)
 [![PyPI version](https://badge.fury.io/py/instld.svg)](https://badge.fury.io/py/instld)
 
 Thanks to this package, it is very easy to manage the lifecycle of packages directly from the code.
 
@@ -44,9 +42,7 @@
 
   config.add_handlers(file_writer())
 
   log('some message!')
 ```
 
 This code installs the [polog](https://github.com/pomponchik/polog) package, imports the necessary objects from there and displays a message. At the end of the program, there will be no excess garbage left in the system. This way you can easily try different packages without bothering with their installation and subsequent removal.
-
-
```

### Comparing `instld-0.0.4/README.md` & `instld-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # INSTALLED: the simplest package management from the source code
 
 [![Downloads](https://pepy.tech/badge/instld/month)](https://pepy.tech/project/instld)
-[![Downloads](https://pepy.tech/badge/instld)](https://pepy.tech/project/installed)
+[![Downloads](https://pepy.tech/badge/instld)](https://pepy.tech/project/instld)
 [![codecov](https://codecov.io/gh/pomponchik/installed/branch/main/graph/badge.svg)](https://codecov.io/gh/pomponchik/installed)
 [![Test-Package](https://github.com/pomponchik/installed/actions/workflows/coverage.yml/badge.svg)](https://github.com/pomponchik/installed/actions/workflows/coverage.yml)
 [![Python versions](https://img.shields.io/pypi/pyversions/instld.svg)](https://pypi.python.org/pypi/instld)
 [![PyPI version](https://badge.fury.io/py/instld.svg)](https://badge.fury.io/py/instld)
 
 Thanks to this package, it is very easy to manage the lifecycle of packages directly from the code.
```

### Comparing `instld-0.0.4/installed/__init__.py` & `instld-0.0.5/installed/context_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 import os
 import sys
 import tempfile
-import subprocess
+
 from threading import Lock
 from io import StringIO
 from contextlib import contextmanager
 
-
-class InstallingPackageError(Exception):
-    pass
+from installed.errors import InstallingPackageError
 
 
 lock = Lock()
 
-
 @contextmanager
-def search_path(base_dir):
+def search_path(base_dir, logger, runner):
     path_to_venv = os.path.join(base_dir, 'venv')
     sys_path = os.path.join(path_to_venv, 'lib')
 
-    subprocess.check_call([sys.executable, '-m', 'venv', path_to_venv], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    runner(['-m', 'venv', path_to_venv], logger)
 
     for maybe_directory in os.listdir(path=sys_path):
         maybe_directory_full = os.path.join(sys_path, maybe_directory)
         if maybe_directory.startswith('python') and os.path.isdir(maybe_directory_full):
             sys_path = os.path.join(sys_path, maybe_directory, 'site-packages')
             break
 
@@ -32,24 +29,17 @@
 
     yield sys_path
 
     with lock:
         del sys.path[sys.path.index(sys_path)]
 
 @contextmanager
-def pip_context(*packages_names):
+def pip_context(packages_names, logger, runner):
     with tempfile.TemporaryDirectory() as directory:
-        with search_path(directory) as where:
+        with search_path(directory, logger, runner) as where:
             try:
                 for package_name in packages_names:
-                    subprocess.check_call([sys.executable, '-m', 'pip', 'install', f'--target={where}', package_name], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+                    runner(['-m', 'pip', 'install', f'--target={where}', package_name], logger)
             except subprocess.CalledProcessError as e:
                 raise InstallingPackageError from e
 
             yield
-
-
-class ProxyModule(sys.modules[__name__].__class__):
-    def __call__(self, *packages_names):
-        return pip_context(*packages_names)
-
-sys.modules[__name__].__class__ = ProxyModule
```

### Comparing `instld-0.0.4/instld.egg-info/PKG-INFO` & `instld-0.0.5/instld.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: instld
-Version: 0.0.4
+Version: 0.0.5
 Summary: The simplest package management from the source code
 Home-page: https://github.com/pomponchik/installed
 Author: Evgeniy Blinov
 Author-email: zheni-b@yandex.ru
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # INSTALLED: the simplest package management from the source code
 
 [![Downloads](https://pepy.tech/badge/instld/month)](https://pepy.tech/project/instld)
-[![Downloads](https://pepy.tech/badge/instld)](https://pepy.tech/project/installed)
+[![Downloads](https://pepy.tech/badge/instld)](https://pepy.tech/project/instld)
 [![codecov](https://codecov.io/gh/pomponchik/installed/branch/main/graph/badge.svg)](https://codecov.io/gh/pomponchik/installed)
 [![Test-Package](https://github.com/pomponchik/installed/actions/workflows/coverage.yml/badge.svg)](https://github.com/pomponchik/installed/actions/workflows/coverage.yml)
 [![Python versions](https://img.shields.io/pypi/pyversions/instld.svg)](https://pypi.python.org/pypi/instld)
 [![PyPI version](https://badge.fury.io/py/instld.svg)](https://badge.fury.io/py/instld)
 
 Thanks to this package, it is very easy to manage the lifecycle of packages directly from the code.
 
@@ -44,9 +42,7 @@
 
   config.add_handlers(file_writer())
 
   log('some message!')
 ```
 
 This code installs the [polog](https://github.com/pomponchik/polog) package, imports the necessary objects from there and displays a message. At the end of the program, there will be no excess garbage left in the system. This way you can easily try different packages without bothering with their installation and subsequent removal.
-
-
```

### Comparing `instld-0.0.4/setup.py` & `instld-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = []
 
 setup(
     name="instld",
-    version="0.0.4",
+    version="0.0.5",
     author="Evgeniy Blinov",
     author_email="zheni-b@yandex.ru",
     description="The simplest package management from the source code",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/pomponchik/installed",
     packages=find_packages(exclude=["tests"]),
```

