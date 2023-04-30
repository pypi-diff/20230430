# Comparing `tmp/easypipinstall-0.2.0.tar.gz` & `tmp/easypipinstall-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easypipinstall-0.2.0.tar", last modified: Sun Apr 30 08:21:32 2023, max compression
+gzip compressed data, was "easypipinstall-0.2.1.tar", last modified: Sun Apr 30 08:49:04 2023, max compression
```

## Comparing `easypipinstall-0.2.0.tar` & `easypipinstall-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-30 08:21:32.673605 easypipinstall-0.2.0/
--rw-r--r--   0 nicolasdao   (501) staff       (20)     1541 2023-02-14 06:31:54.000000 easypipinstall-0.2.0/LICENSE
--rw-r--r--   0 nicolasdao   (501) staff       (20)    11843 2023-04-30 08:21:32.673671 easypipinstall-0.2.0/PKG-INFO
--rw-r--r--   0 nicolasdao   (501) staff       (20)    11174 2023-04-30 08:16:27.000000 easypipinstall-0.2.0/README.md
--rw-r--r--   0 nicolasdao   (501) staff       (20)      179 2023-02-14 06:47:32.000000 easypipinstall-0.2.0/pyproject.toml
--rw-r--r--   0 nicolasdao   (501) staff       (20)     1091 2023-04-30 08:21:32.674047 easypipinstall-0.2.0/setup.cfg
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-30 08:21:32.671592 easypipinstall-0.2.0/src/
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-30 08:21:32.672723 easypipinstall-0.2.0/src/easypipinstall/
--rw-r--r--   0 nicolasdao   (501) staff       (20)       85 2023-04-29 07:55:46.000000 easypipinstall-0.2.0/src/easypipinstall/__init__.py
--rw-r--r--   0 nicolasdao   (501) staff       (20)    10532 2023-04-29 15:37:21.000000 easypipinstall-0.2.0/src/easypipinstall/install.py
--rw-r--r--   0 nicolasdao   (501) staff       (20)    14295 2023-04-30 08:18:41.000000 easypipinstall-0.2.0/src/easypipinstall/version.py
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-30 08:21:32.673500 easypipinstall-0.2.0/src/easypipinstall.egg-info/
--rw-r--r--   0 nicolasdao   (501) staff       (20)    11843 2023-04-30 08:21:32.000000 easypipinstall-0.2.0/src/easypipinstall.egg-info/PKG-INFO
--rw-r--r--   0 nicolasdao   (501) staff       (20)      387 2023-04-30 08:21:32.000000 easypipinstall-0.2.0/src/easypipinstall.egg-info/SOURCES.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)        1 2023-04-30 08:21:32.000000 easypipinstall-0.2.0/src/easypipinstall.egg-info/dependency_links.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)       82 2023-04-30 08:21:32.000000 easypipinstall-0.2.0/src/easypipinstall.egg-info/entry_points.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)       32 2023-04-30 08:21:32.000000 easypipinstall-0.2.0/src/easypipinstall.egg-info/requires.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)       15 2023-04-30 08:21:32.000000 easypipinstall-0.2.0/src/easypipinstall.egg-info/top_level.txt
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-30 08:49:04.942735 easypipinstall-0.2.1/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     1541 2023-02-14 06:31:54.000000 easypipinstall-0.2.1/LICENSE
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    11843 2023-04-30 08:49:04.942811 easypipinstall-0.2.1/PKG-INFO
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    11174 2023-04-30 08:16:27.000000 easypipinstall-0.2.1/README.md
+-rw-r--r--   0 nicolasdao   (501) staff       (20)      179 2023-02-14 06:47:32.000000 easypipinstall-0.2.1/pyproject.toml
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     1123 2023-04-30 08:49:04.943224 easypipinstall-0.2.1/setup.cfg
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-30 08:49:04.940123 easypipinstall-0.2.1/src/
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-30 08:49:04.941717 easypipinstall-0.2.1/src/easypipinstall/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)       85 2023-04-29 07:55:46.000000 easypipinstall-0.2.1/src/easypipinstall/__init__.py
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    10532 2023-04-29 15:37:21.000000 easypipinstall-0.2.1/src/easypipinstall/install.py
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    14295 2023-04-30 08:18:41.000000 easypipinstall-0.2.1/src/easypipinstall/version.py
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-30 08:49:04.942605 easypipinstall-0.2.1/src/easypipinstall.egg-info/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    11843 2023-04-30 08:49:04.000000 easypipinstall-0.2.1/src/easypipinstall.egg-info/PKG-INFO
+-rw-r--r--   0 nicolasdao   (501) staff       (20)      387 2023-04-30 08:49:04.000000 easypipinstall-0.2.1/src/easypipinstall.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)        1 2023-04-30 08:49:04.000000 easypipinstall-0.2.1/src/easypipinstall.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)      113 2023-04-30 08:49:04.000000 easypipinstall-0.2.1/src/easypipinstall.egg-info/entry_points.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)       32 2023-04-30 08:49:04.000000 easypipinstall-0.2.1/src/easypipinstall.egg-info/requires.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)       15 2023-04-30 08:49:04.000000 easypipinstall-0.2.1/src/easypipinstall.egg-info/top_level.txt
```

### Comparing `easypipinstall-0.2.0/LICENSE` & `easypipinstall-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easypipinstall-0.2.0/PKG-INFO` & `easypipinstall-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypipinstall
-Version: 0.2.0
+Version: 0.2.1
 Summary: easypipinstall installs Python packages similarly to NPM in NodeJS. It automatically maintains the `requirements.txt`, `prod-requirements.txt` and `setup.cfg` files. It also easily uninstalls all the dependencies from those files.
 Home-page: https://github.com/nicolasdao/easypipinstall
 Author: Nicolas Dao
 Author-email: nicolas.dao@gmail.com
 License: BSD-3-Clause
 Keywords: pip,install,uninstall
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easypipinstall-0.2.0/README.md` & `easypipinstall-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `easypipinstall-0.2.0/setup.cfg` & `easypipinstall-0.2.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easypipinstall
-version = 0.2.0
+version = 0.2.1
 author = Nicolas Dao
 author_email = nicolas.dao@gmail.com
 description = easypipinstall installs Python packages similarly to NPM in NodeJS. It automatically maintains the `requirements.txt`, `prod-requirements.txt` and `setup.cfg` files. It also easily uninstalls all the dependencies from those files.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nicolasdao/easypipinstall
 readme = README.md
@@ -30,14 +30,15 @@
 	flake8
 	twine
 
 [options.entry_points]
 console_scripts = 
 	easyi = easypipinstall:install
 	easyu = easypipinstall:uninstall
+	easyv = easypipinstall:version
 
 [flake8]
 extend-ignore = W191,E501,E302,E231,W291,E305,W391,E722
 exclude = .git,__pycache__,.venv,build,dist,test.py
 
 [egg_info]
 tag_build =
```

### Comparing `easypipinstall-0.2.0/src/easypipinstall/install.py` & `easypipinstall-0.2.1/src/easypipinstall/install.py`

 * *Files identical despite different names*

### Comparing `easypipinstall-0.2.0/src/easypipinstall/version.py` & `easypipinstall-0.2.1/src/easypipinstall/version.py`

 * *Files identical despite different names*

### Comparing `easypipinstall-0.2.0/src/easypipinstall.egg-info/PKG-INFO` & `easypipinstall-0.2.1/src/easypipinstall.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypipinstall
-Version: 0.2.0
+Version: 0.2.1
 Summary: easypipinstall installs Python packages similarly to NPM in NodeJS. It automatically maintains the `requirements.txt`, `prod-requirements.txt` and `setup.cfg` files. It also easily uninstalls all the dependencies from those files.
 Home-page: https://github.com/nicolasdao/easypipinstall
 Author: Nicolas Dao
 Author-email: nicolas.dao@gmail.com
 License: BSD-3-Clause
 Keywords: pip,install,uninstall
 Classifier: Programming Language :: Python :: 3
```

