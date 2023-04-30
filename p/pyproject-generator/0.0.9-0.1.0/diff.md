# Comparing `tmp/pyproject-generator-0.0.9.tar.gz` & `tmp/pyproject-generator-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-generator-0.0.9.tar", last modified: Sun Apr 30 11:34:34 2023, max compression
+gzip compressed data, was "pyproject-generator-0.1.0.tar", last modified: Sun Apr 30 11:41:20 2023, max compression
```

## Comparing `pyproject-generator-0.0.9.tar` & `pyproject-generator-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:34:34.242709 pyproject-generator-0.0.9/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2082 2023-04-30 11:34:34.242889 pyproject-generator-0.0.9/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1563 2023-04-30 01:14:26.000000 pyproject-generator-0.0.9/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-19 15:24:26.000000 pyproject-generator-0.0.9/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-04-30 11:34:34.243928 pyproject-generator-0.0.9/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:34:34.218305 pyproject-generator-0.0.9/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:34:34.223891 pyproject-generator-0.0.9/src/pyproject/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-19 15:24:27.000000 pyproject-generator-0.0.9/src/pyproject/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-30 11:34:19.000000 pyproject-generator-0.0.9/src/pyproject/__version__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3059 2023-04-30 11:31:44.000000 pyproject-generator-0.0.9/src/pyproject/cli.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:34:34.226912 pyproject-generator-0.0.9/src/pyproject/config/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.0.9/src/pyproject/config/config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)      259 2023-04-30 01:22:22.000000 pyproject-generator-0.0.9/src/pyproject/config/default_config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)     9026 2023-04-30 11:23:07.000000 pyproject-generator-0.0.9/src/pyproject/project_builder.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:34:34.235875 pyproject-generator-0.0.9/src/pyproject/templates/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.0.9/src/pyproject/templates/gitignore.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.0.9/src/pyproject/templates/license_apache.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.0.9/src/pyproject/templates/license_mit.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.0.9/src/pyproject/templates/pyproject.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.0.9/src/pyproject/templates/readme.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      578 2023-04-14 17:03:04.000000 pyproject-generator-0.0.9/src/pyproject/templates/setup.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.0.9/src/pyproject/templates/tests.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.0.9/src/pyproject/templates/tox.template
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:34:34.241601 pyproject-generator-0.0.9/src/pyproject_generator.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2082 2023-04-30 11:34:34.000000 pyproject-generator-0.0.9/src/pyproject_generator.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)      859 2023-04-30 11:34:34.000000 pyproject-generator-0.0.9/src/pyproject_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-30 11:34:34.000000 pyproject-generator-0.0.9/src/pyproject_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-30 11:34:34.000000 pyproject-generator-0.0.9/src/pyproject_generator.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-04-30 11:34:34.000000 pyproject-generator-0.0.9/src/pyproject_generator.egg-info/requires.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-30 11:34:34.000000 pyproject-generator-0.0.9/src/pyproject_generator.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:34:34.242230 pyproject-generator-0.0.9/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.0.9/tests/test_pyproject.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:41:20.770048 pyproject-generator-0.1.0/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2082 2023-04-30 11:41:20.770209 pyproject-generator-0.1.0/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1563 2023-04-30 01:14:26.000000 pyproject-generator-0.1.0/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-19 15:24:26.000000 pyproject-generator-0.1.0/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-04-30 11:41:20.771521 pyproject-generator-0.1.0/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:41:20.745757 pyproject-generator-0.1.0/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:41:20.751091 pyproject-generator-0.1.0/src/pyproject/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-19 15:24:27.000000 pyproject-generator-0.1.0/src/pyproject/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-30 11:41:10.000000 pyproject-generator-0.1.0/src/pyproject/__version__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3059 2023-04-30 11:31:44.000000 pyproject-generator-0.1.0/src/pyproject/cli.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:41:20.752968 pyproject-generator-0.1.0/src/pyproject/config/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.1.0/src/pyproject/config/config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      259 2023-04-30 01:22:22.000000 pyproject-generator-0.1.0/src/pyproject/config/default_config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     9039 2023-04-30 11:40:21.000000 pyproject-generator-0.1.0/src/pyproject/project_builder.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:41:20.762934 pyproject-generator-0.1.0/src/pyproject/templates/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.1.0/src/pyproject/templates/gitignore.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.1.0/src/pyproject/templates/license_apache.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.1.0/src/pyproject/templates/license_mit.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.1.0/src/pyproject/templates/pyproject.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.1.0/src/pyproject/templates/readme.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      578 2023-04-14 17:03:04.000000 pyproject-generator-0.1.0/src/pyproject/templates/setup.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.1.0/src/pyproject/templates/tests.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.1.0/src/pyproject/templates/tox.template
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:41:20.768653 pyproject-generator-0.1.0/src/pyproject_generator.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2082 2023-04-30 11:41:20.000000 pyproject-generator-0.1.0/src/pyproject_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      859 2023-04-30 11:41:20.000000 pyproject-generator-0.1.0/src/pyproject_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-30 11:41:20.000000 pyproject-generator-0.1.0/src/pyproject_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-30 11:41:20.000000 pyproject-generator-0.1.0/src/pyproject_generator.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-04-30 11:41:20.000000 pyproject-generator-0.1.0/src/pyproject_generator.egg-info/requires.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-30 11:41:20.000000 pyproject-generator-0.1.0/src/pyproject_generator.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:41:20.769705 pyproject-generator-0.1.0/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.1.0/tests/test_pyproject.py
```

### Comparing `pyproject-generator-0.0.9/PKG-INFO` & `pyproject-generator-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.0.9
+Version: 0.1.0
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.0.9/README.md` & `pyproject-generator-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.9/setup.cfg` & `pyproject-generator-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.9/src/pyproject/cli.py` & `pyproject-generator-0.1.0/src/pyproject/cli.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.9/src/pyproject/project_builder.py` & `pyproject-generator-0.1.0/src/pyproject/project_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,24 +239,24 @@
         return merged_config
 
     def _write_config_file(self, config: dict):
         config["dependencies"] = list(config["dependencies"])
         with open(self._user_config_dir / "config.json", "w") as f:
             json.dump(config, f, indent=4)
 
-    def update_config(self, config):
+    def update_config(self, config: dict):
         default = self._parse_config_file("default_config.json")
         merged_config = {}
         for k, v in default.items():
             if k not in config:
                 merged_config[k] = v
             else:
                 merged_config[k] = config[k]
 
-        self._write_config_file(config)
+        self._write_config_file(merged_config)
 
     def config(self):
         self._write_config_file(self._config)
 
     def upload(self):
         username = self._config["pypi_username"]
         password = self._config["pypi_password"]
```

### Comparing `pyproject-generator-0.0.9/src/pyproject/templates/gitignore.template` & `pyproject-generator-0.1.0/src/pyproject/templates/gitignore.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.9/src/pyproject/templates/license_apache.template` & `pyproject-generator-0.1.0/src/pyproject/templates/license_apache.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.9/src/pyproject/templates/license_mit.template` & `pyproject-generator-0.1.0/src/pyproject/templates/license_mit.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.9/src/pyproject/templates/setup.template` & `pyproject-generator-0.1.0/src/pyproject/templates/setup.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.9/src/pyproject/templates/tests.template` & `pyproject-generator-0.1.0/src/pyproject/templates/tests.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.9/src/pyproject_generator.egg-info/PKG-INFO` & `pyproject-generator-0.1.0/src/pyproject_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.0.9
+Version: 0.1.0
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.0.9/src/pyproject_generator.egg-info/SOURCES.txt` & `pyproject-generator-0.1.0/src/pyproject_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

