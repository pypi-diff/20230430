# Comparing `tmp/ErCore-1.1.tar.gz` & `tmp/ErCore-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ErCore-1.1.tar", last modified: Thu Apr 27 08:53:07 2023, max compression
+gzip compressed data, was "ErCore-1.2.tar", last modified: Sun Apr 30 06:12:21 2023, max compression
```

## Comparing `ErCore-1.1.tar` & `ErCore-1.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 08:53:07.560261 ErCore-1.1/
-drwxrwxrwx   0        0        0        0 2023-04-27 08:53:07.516245 ErCore-1.1/ErCore/
--rw-rw-rw-   0        0        0     2114 2023-04-27 08:34:53.000000 ErCore-1.1/ErCore/Core.py
--rw-rw-rw-   0        0        0       70 2023-04-26 11:12:02.000000 ErCore-1.1/ErCore/__init__.py
--rw-rw-rw-   0        0        0     3190 2023-04-27 08:26:30.000000 ErCore-1.1/ErCore/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-27 08:53:07.557245 ErCore-1.1/ErCore/std/
--rw-rw-rw-   0        0        0      375 2023-04-25 04:21:27.000000 ErCore-1.1/ErCore/std/Base.py
--rw-rw-rw-   0        0        0       33 2023-04-25 04:21:27.000000 ErCore-1.1/ErCore/std/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 08:53:07.530244 ErCore-1.1/ErCore.egg-info/
--rw-rw-rw-   0        0        0      475 2023-04-27 08:53:07.000000 ErCore-1.1/ErCore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-04-27 08:53:07.000000 ErCore-1.1/ErCore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 08:53:07.000000 ErCore-1.1/ErCore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-04-27 08:53:07.000000 ErCore-1.1/ErCore.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 08:53:07.000000 ErCore-1.1/ErCore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-04-21 12:30:11.000000 ErCore-1.1/LICENSE
--rw-rw-rw-   0        0        0      475 2023-04-27 08:53:07.560261 ErCore-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-04-27 08:27:25.000000 ErCore-1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-27 08:53:07.561244 ErCore-1.1/setup.cfg
--rw-rw-rw-   0        0        0      679 2023-04-27 08:26:47.000000 ErCore-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:12:21.200359 ErCore-1.2/
+drwxrwxrwx   0        0        0        0 2023-04-30 06:12:21.175347 ErCore-1.2/ErCore/
+-rw-rw-rw-   0        0        0     2057 2023-04-30 06:10:30.000000 ErCore-1.2/ErCore/Core.py
+-rw-rw-rw-   0        0        0       58 2023-04-30 06:12:01.000000 ErCore-1.2/ErCore/__init__.py
+-rw-rw-rw-   0        0        0     3170 2023-04-30 06:07:55.000000 ErCore-1.2/ErCore/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:12:21.197357 ErCore-1.2/ErCore/std/
+-rw-rw-rw-   0        0        0      745 2023-04-30 06:06:11.000000 ErCore-1.2/ErCore/std/Base.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:12:21.196346 ErCore-1.2/ErCore.egg-info/
+-rw-rw-rw-   0        0        0      475 2023-04-30 06:12:20.000000 ErCore-1.2/ErCore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-04-30 06:12:20.000000 ErCore-1.2/ErCore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 06:12:20.000000 ErCore-1.2/ErCore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-04-30 06:12:20.000000 ErCore-1.2/ErCore.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-30 06:12:20.000000 ErCore-1.2/ErCore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-04-21 12:30:11.000000 ErCore-1.2/LICENSE
+-rw-rw-rw-   0        0        0      475 2023-04-30 06:12:21.199357 ErCore-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-04-27 08:27:25.000000 ErCore-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 06:12:21.200359 ErCore-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      679 2023-04-30 06:09:42.000000 ErCore-1.2/setup.py
```

### Comparing `ErCore-1.1/ErCore/Core.py` & `ErCore-1.2/ErCore/Core.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import time
 import platform
 
-from std import colors, style
+from std.Base import *
 
 
 class ECore:
     def __init__(self):
-        self.version = 1.1
+        self.version = 1.2
         self.IS_WINDOWS = (platform.system() == 'Windows')
         self.IS_LINUX = (platform.system() == 'Linux')
         self.IS_MAC = (platform.system() == 'Darwin')
 
     def info(self):
         try:
             print(f'Autor: Eragod\nProject: ErCore\nVersion: {self.version}')
         except Exception as error:
-            print(f'{colors["Red"]}Error!\n{error}\nError!{colors["Reset"]}')
+            print(f'{red}Error!\n{error}\nError!{RESET}')
 
     def make_runner(self):
         file = input('file name: ')
         if self.IS_WINDOWS:
             with open(f'run.bat', 'w') as runner:
                 runner.write(f'@echo off\npython {file}.py\npause')
         if self.IS_LINUX:
@@ -32,26 +32,26 @@
     @staticmethod
     def logger(function):
         try:
             if function is not None:
                 second = time.localtime().tm_sec
                 minute = time.localtime().tm_min
                 hour = time.localtime().tm_hour
-                print(f'{style["BOLD"]}{colors["Red"]}{hour}:{minute}:{second}:{colors["Reset"]}',
+                print(f'{bold}{red}{hour}:{minute}:{second}:{RESET}',
                       f'{function.__name__} Start work!')
                 function()
                 second = time.localtime().tm_sec
                 minute = time.localtime().tm_min
                 hour = time.localtime().tm_hour
-                print(f'{style["BOLD"]}{colors["Red"]}{hour}:{minute}:{second}:{colors["Reset"]}',
+                print(f'{bold}{red}{hour}:{minute}:{second}:{RESET}',
                       f'{function.__name__} End work!')
             else:
                 ...
         except Exception as error:
-            print(f'{error}')
+            print(f'{red}Error!\n{error}\nError!{RESET}')
 
 
 def EDecor(iteration: int = 1):
     def EraDeCore(func):
         def wrapper(*args, **kwargs):
             for _ in range(iteration):
                 func(*args, **kwargs)
```

### Comparing `ErCore-1.1/ErCore/cli.py` & `ErCore-1.2/ErCore/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import time
 import platform
 
-from std import colors
+from std.Base import *
 
 
 def make_project():
     try:
         name = str(input('Enter project name: '))
         readme = str(input('Add readme file?[Y/N]: '))
         python = str(input('Add python file?[Y/N]: '))
@@ -39,15 +39,15 @@
                 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
                 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
                 FROM,OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE."""
 
                 with open('LICENSE', 'w') as lt:
                     lt.write(mit_l)
             else:
-                print(f'{colors["Red"]}Error! WORK ONLY MIT LICENSE (try again){colors["Reset"]}')
+                print(f'{red}Error! WORK ONLY MIT LICENSE (try again){RESET}')
         else:
             print('')
     except ValueError as error:
         print('!!!' * 20)
         print(error)
         print('!!!' * 20)
         print('Helper: pls restart command and enter string')
```

### Comparing `ErCore-1.1/LICENSE` & `ErCore-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ErCore-1.1/setup.py` & `ErCore-1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ErCore',
-    version='1.1',
+    version='1.2',
     packages=find_packages(),
     author='Eragod',
     description='Core for projects',
     url="https://github.com/Eragod/ErCore",
     long_description=open('README.md', 'r').read(),
     long_description_content_type="text/markdown",
     entry_points={'console_scripts': ['ErCore-project = ErCore.cli:make_project',
```

