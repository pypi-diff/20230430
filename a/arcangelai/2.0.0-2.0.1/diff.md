# Comparing `tmp/arcangelai-2.0.0.tar.gz` & `tmp/arcangelai-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcangelai-2.0.0.tar", last modified: Sat Apr 29 22:01:40 2023, max compression
+gzip compressed data, was "arcangelai-2.0.1.tar", last modified: Sat Apr 29 22:59:12 2023, max compression
```

## Comparing `arcangelai-2.0.0.tar` & `arcangelai-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 william    (506) staff       (20)        0 2023-04-29 22:01:40.175207 arcangelai-2.0.0/
--rw-r--r--   0 william    (506) staff       (20)       77 2023-04-29 21:40:13.000000 arcangelai-2.0.0/CHANGELOG.txt
--rw-r--r--   0 william    (506) staff       (20)     1067 2023-04-29 21:25:13.000000 arcangelai-2.0.0/LICENSE
--rw-r--r--   0 william    (506) staff       (20)       25 2023-04-29 21:53:13.000000 arcangelai-2.0.0/MANIFEST.in
--rw-r--r--   0 william    (506) staff       (20)      495 2023-04-29 22:01:40.174640 arcangelai-2.0.0/PKG-INFO
--rw-r--r--   0 william    (506) staff       (20)       14 2023-04-29 21:18:11.000000 arcangelai-2.0.0/README.md
-drwxr-xr-x   0 william    (506) staff       (20)        0 2023-04-29 22:01:40.171759 arcangelai-2.0.0/arcangelai/
--rw-r--r--   0 william    (506) staff       (20)      165 2023-04-29 21:36:54.000000 arcangelai-2.0.0/arcangelai/__init__.py
-drwxr-xr-x   0 william    (506) staff       (20)        0 2023-04-29 22:01:40.174150 arcangelai-2.0.0/arcangelai.egg-info/
--rw-r--r--   0 william    (506) staff       (20)      495 2023-04-29 22:01:40.000000 arcangelai-2.0.0/arcangelai.egg-info/PKG-INFO
--rw-r--r--   0 william    (506) staff       (20)      211 2023-04-29 22:01:40.000000 arcangelai-2.0.0/arcangelai.egg-info/SOURCES.txt
--rw-r--r--   0 william    (506) staff       (20)        1 2023-04-29 22:01:40.000000 arcangelai-2.0.0/arcangelai.egg-info/dependency_links.txt
--rw-r--r--   0 william    (506) staff       (20)       11 2023-04-29 22:01:40.000000 arcangelai-2.0.0/arcangelai.egg-info/top_level.txt
--rw-r--r--   0 william    (506) staff       (20)       38 2023-04-29 22:01:40.175327 arcangelai-2.0.0/setup.cfg
--rw-r--r--   0 william    (506) staff       (20)      600 2023-04-29 22:00:00.000000 arcangelai-2.0.0/setup.py
+drwxr-xr-x   0 william    (506) staff       (20)        0 2023-04-29 22:59:12.769548 arcangelai-2.0.1/
+-rw-r--r--   0 william    (506) staff       (20)       77 2023-04-29 21:40:13.000000 arcangelai-2.0.1/CHANGELOG.txt
+-rw-r--r--   0 william    (506) staff       (20)     1067 2023-04-29 21:25:13.000000 arcangelai-2.0.1/LICENSE
+-rw-r--r--   0 william    (506) staff       (20)       25 2023-04-29 21:53:13.000000 arcangelai-2.0.1/MANIFEST.in
+-rw-r--r--   0 william    (506) staff       (20)      554 2023-04-29 22:59:12.768980 arcangelai-2.0.1/PKG-INFO
+-rw-r--r--   0 william    (506) staff       (20)       36 2023-04-29 22:47:34.000000 arcangelai-2.0.1/README.md
+drwxr-xr-x   0 william    (506) staff       (20)        0 2023-04-29 22:59:12.765449 arcangelai-2.0.1/arcangelai/
+-rw-r--r--   0 william    (506) staff       (20)      887 2023-04-29 22:44:08.000000 arcangelai-2.0.1/arcangelai/__init__.py
+drwxr-xr-x   0 william    (506) staff       (20)        0 2023-04-29 22:59:12.767789 arcangelai-2.0.1/arcangelai.egg-info/
+-rw-r--r--   0 william    (506) staff       (20)      554 2023-04-29 22:59:12.000000 arcangelai-2.0.1/arcangelai.egg-info/PKG-INFO
+-rw-r--r--   0 william    (506) staff       (20)      211 2023-04-29 22:59:12.000000 arcangelai-2.0.1/arcangelai.egg-info/SOURCES.txt
+-rw-r--r--   0 william    (506) staff       (20)        1 2023-04-29 22:59:12.000000 arcangelai-2.0.1/arcangelai.egg-info/dependency_links.txt
+-rw-r--r--   0 william    (506) staff       (20)       11 2023-04-29 22:59:12.000000 arcangelai-2.0.1/arcangelai.egg-info/top_level.txt
+-rw-r--r--   0 william    (506) staff       (20)       38 2023-04-29 22:59:12.769667 arcangelai-2.0.1/setup.cfg
+-rw-r--r--   0 william    (506) staff       (20)      646 2023-04-29 22:49:30.000000 arcangelai-2.0.1/setup.py
```

### Comparing `arcangelai-2.0.0/LICENSE` & `arcangelai-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arcangelai-2.0.0/setup.py` & `arcangelai-2.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,16 +5,17 @@
   'Intended Audience :: Education',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='arcangelai',
-  version='2.0.0',
+  version='2.0.1',
   description='Autonomous AI',
+  long_description_content_type='text/x-rst',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Arc Angel Ai',
   author_email='arcangelgpt@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='autonomous',
```

