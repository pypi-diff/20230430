# Comparing `tmp/pyproject-generator-0.1.1.tar.gz` & `tmp/pyproject-generator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-generator-0.1.1.tar", last modified: Sun Apr 30 12:15:28 2023, max compression
+gzip compressed data, was "pyproject-generator-0.1.2.tar", last modified: Sun Apr 30 14:32:21 2023, max compression
```

## Comparing `pyproject-generator-0.1.1.tar` & `pyproject-generator-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 12:15:28.328447 pyproject-generator-0.1.1/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2082 2023-04-30 12:15:28.328731 pyproject-generator-0.1.1/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1563 2023-04-30 01:14:26.000000 pyproject-generator-0.1.1/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-19 15:24:26.000000 pyproject-generator-0.1.1/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-04-30 12:15:28.330014 pyproject-generator-0.1.1/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 12:15:28.302919 pyproject-generator-0.1.1/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 12:15:28.308261 pyproject-generator-0.1.1/src/pyproject/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-19 15:24:27.000000 pyproject-generator-0.1.1/src/pyproject/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-30 12:15:16.000000 pyproject-generator-0.1.1/src/pyproject/__version__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3059 2023-04-30 11:31:44.000000 pyproject-generator-0.1.1/src/pyproject/cli.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 12:15:28.311009 pyproject-generator-0.1.1/src/pyproject/config/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.1.1/src/pyproject/config/config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)      259 2023-04-30 01:22:22.000000 pyproject-generator-0.1.1/src/pyproject/config/default_config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)     8884 2023-04-30 12:15:08.000000 pyproject-generator-0.1.1/src/pyproject/project_builder.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 12:15:28.321192 pyproject-generator-0.1.1/src/pyproject/templates/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.1.1/src/pyproject/templates/gitignore.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.1.1/src/pyproject/templates/license_apache.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.1.1/src/pyproject/templates/license_mit.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.1.1/src/pyproject/templates/pyproject.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.1.1/src/pyproject/templates/readme.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      578 2023-04-14 17:03:04.000000 pyproject-generator-0.1.1/src/pyproject/templates/setup.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.1.1/src/pyproject/templates/tests.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.1.1/src/pyproject/templates/tox.template
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 12:15:28.327124 pyproject-generator-0.1.1/src/pyproject_generator.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2082 2023-04-30 12:15:28.000000 pyproject-generator-0.1.1/src/pyproject_generator.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)      859 2023-04-30 12:15:28.000000 pyproject-generator-0.1.1/src/pyproject_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-30 12:15:28.000000 pyproject-generator-0.1.1/src/pyproject_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-30 12:15:28.000000 pyproject-generator-0.1.1/src/pyproject_generator.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-04-30 12:15:28.000000 pyproject-generator-0.1.1/src/pyproject_generator.egg-info/requires.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-30 12:15:28.000000 pyproject-generator-0.1.1/src/pyproject_generator.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 12:15:28.327920 pyproject-generator-0.1.1/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.1.1/tests/test_pyproject.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 14:32:21.337211 pyproject-generator-0.1.2/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2082 2023-04-30 14:32:21.337476 pyproject-generator-0.1.2/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1563 2023-04-30 01:14:26.000000 pyproject-generator-0.1.2/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-19 15:24:26.000000 pyproject-generator-0.1.2/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-04-30 14:32:21.338793 pyproject-generator-0.1.2/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 14:32:21.312819 pyproject-generator-0.1.2/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 14:32:21.317484 pyproject-generator-0.1.2/src/pyproject/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-19 15:24:27.000000 pyproject-generator-0.1.2/src/pyproject/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-30 14:32:10.000000 pyproject-generator-0.1.2/src/pyproject/__version__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2835 2023-04-30 14:29:20.000000 pyproject-generator-0.1.2/src/pyproject/cli.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 14:32:21.320397 pyproject-generator-0.1.2/src/pyproject/config/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.1.2/src/pyproject/config/config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      259 2023-04-30 01:22:22.000000 pyproject-generator-0.1.2/src/pyproject/config/default_config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     8822 2023-04-30 14:29:09.000000 pyproject-generator-0.1.2/src/pyproject/project_builder.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 14:32:21.330227 pyproject-generator-0.1.2/src/pyproject/templates/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.1.2/src/pyproject/templates/gitignore.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.1.2/src/pyproject/templates/license_apache.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.1.2/src/pyproject/templates/license_mit.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.1.2/src/pyproject/templates/pyproject.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.1.2/src/pyproject/templates/readme.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      578 2023-04-14 17:03:04.000000 pyproject-generator-0.1.2/src/pyproject/templates/setup.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.1.2/src/pyproject/templates/tests.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.1.2/src/pyproject/templates/tox.template
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 14:32:21.335765 pyproject-generator-0.1.2/src/pyproject_generator.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2082 2023-04-30 14:32:21.000000 pyproject-generator-0.1.2/src/pyproject_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      859 2023-04-30 14:32:21.000000 pyproject-generator-0.1.2/src/pyproject_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-30 14:32:21.000000 pyproject-generator-0.1.2/src/pyproject_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-30 14:32:21.000000 pyproject-generator-0.1.2/src/pyproject_generator.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-04-30 14:32:21.000000 pyproject-generator-0.1.2/src/pyproject_generator.egg-info/requires.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-30 14:32:21.000000 pyproject-generator-0.1.2/src/pyproject_generator.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 14:32:21.336610 pyproject-generator-0.1.2/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.1.2/tests/test_pyproject.py
```

### Comparing `pyproject-generator-0.1.1/PKG-INFO` & `pyproject-generator-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.1.1
+Version: 0.1.2
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.1.1/README.md` & `pyproject-generator-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.1/setup.cfg` & `pyproject-generator-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.1/src/pyproject/cli.py` & `pyproject-generator-0.1.2/src/pyproject/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,20 +45,14 @@
         "--remove_dependencies",
         type=str,
         help="Remove dependencies to always download. Pass in a comma delimited string",
     )
     parser.add_argument(
         "--show", required=False, action="store_true", help="Show the current config"
     )
-    parser.add_argument(
-        "--update",
-        required=False,
-        action="store_true",
-        help="If there are new keys in the default config, add them to the user config",
-    )
 
     parser.add_argument(
         "-v",
         "--version",
         action="version",
         version="%(prog)s {version}".format(version=__version__),
         help="Displays package version",
@@ -82,15 +76,14 @@
         "email": args.email,
         "license": args.license,
         "set_dependencies": args.set_dependencies,
         "add_dependencies": args.add_dependencies,
         "remove_dependencies": args.remove_dependencies,
         "reset_config": args.reset_config,
         "show": args.show,
-        "update": args.update,
     }
 
     builder = ProjectBuilder(config=config)
     builder.dispatch(action=args.action, project_name=args.project_name)
 
 
 if __name__ == "__main__":
```

### Comparing `pyproject-generator-0.1.1/src/pyproject/project_builder.py` & `pyproject-generator-0.1.2/src/pyproject/project_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,20 +87,27 @@
             raise ValueError(
                 "A valid project name may only contain ASCII letters, numbers, ., -,"
                 " and/or _, and they must begin and end with a letter or number."
             )
 
     def _create_config_dir(self) -> None:
         self._user_config_dir.mkdir(exist_ok=True)
+
         if not (self._user_config_dir / "config.json").exists():
             shutil.copy(
                 BASE_PATH / "config/default_config.json",
                 self._user_config_dir / "config.json",
             )
 
+        config = self._parse_config_file("config.json")
+        default_config = self._parse_config_file("default_config.json")
+
+        config = default_config | config
+        self._write_config_file(config)
+
         return None
 
     def _fill_in_templates(self, project_name: str) -> dict[str, str]:
         config = self._config
         d = {
             "PACKAGE": project_name,
             "PYPI_USERNAME": config["pypi_username"],
@@ -229,30 +236,21 @@
                 merged_config[k] = v
             else:
                 merged_config[k] = config[k]
 
         if config["show"]:
             pprint.pprint(merged_config)
 
-        if config["update"]:
-            self.update_config(merged_config)
-
         return merged_config
 
     def _write_config_file(self, config: dict):
         config["dependencies"] = list(config["dependencies"])
         with open(self._user_config_dir / "config.json", "w") as f:
             json.dump(config, f, indent=4)
 
-    def update_config(self, config: dict):
-        default = self._parse_config_file("default_config.json")
-        merged_config = default | config
-
-        self._write_config_file(merged_config)
-
     def config(self):
         self._write_config_file(self._config)
 
     def upload(self):
         username = self._config["pypi_username"]
         password = self._config["pypi_password"]
```

### Comparing `pyproject-generator-0.1.1/src/pyproject/templates/gitignore.template` & `pyproject-generator-0.1.2/src/pyproject/templates/gitignore.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.1/src/pyproject/templates/license_apache.template` & `pyproject-generator-0.1.2/src/pyproject/templates/license_apache.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.1/src/pyproject/templates/license_mit.template` & `pyproject-generator-0.1.2/src/pyproject/templates/license_mit.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.1/src/pyproject/templates/setup.template` & `pyproject-generator-0.1.2/src/pyproject/templates/setup.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.1/src/pyproject/templates/tests.template` & `pyproject-generator-0.1.2/src/pyproject/templates/tests.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.1/src/pyproject_generator.egg-info/PKG-INFO` & `pyproject-generator-0.1.2/src/pyproject_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.1.1
+Version: 0.1.2
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.1.1/src/pyproject_generator.egg-info/SOURCES.txt` & `pyproject-generator-0.1.2/src/pyproject_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

