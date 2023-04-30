# Comparing `tmp/pyproject-generator-0.0.8.tar.gz` & `tmp/pyproject-generator-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-generator-0.0.8.tar", last modified: Sat Apr 29 21:03:23 2023, max compression
+gzip compressed data, was "pyproject-generator-0.0.9.tar", last modified: Sun Apr 30 11:34:34 2023, max compression
```

## Comparing `pyproject-generator-0.0.8.tar` & `pyproject-generator-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 21:03:23.894517 pyproject-generator-0.0.8/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-29 21:03:23.894679 pyproject-generator-0.0.8/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1439 2023-04-19 15:24:26.000000 pyproject-generator-0.0.8/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-19 15:24:26.000000 pyproject-generator-0.0.8/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-04-29 21:03:23.895766 pyproject-generator-0.0.8/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 21:03:23.869879 pyproject-generator-0.0.8/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 21:03:23.875511 pyproject-generator-0.0.8/src/pyproject/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-19 15:24:27.000000 pyproject-generator-0.0.8/src/pyproject/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-29 21:03:04.000000 pyproject-generator-0.0.8/src/pyproject/__version__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2714 2023-04-29 20:40:26.000000 pyproject-generator-0.0.8/src/pyproject/cli.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 21:03:23.877802 pyproject-generator-0.0.8/src/pyproject/config/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.0.8/src/pyproject/config/config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:07.000000 pyproject-generator-0.0.8/src/pyproject/config/default_config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)     8205 2023-04-29 21:01:17.000000 pyproject-generator-0.0.8/src/pyproject/project_builder.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 21:03:23.885381 pyproject-generator-0.0.8/src/pyproject/templates/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.0.8/src/pyproject/templates/gitignore.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.0.8/src/pyproject/templates/pyproject.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.0.8/src/pyproject/templates/readme.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      578 2023-04-14 17:03:04.000000 pyproject-generator-0.0.8/src/pyproject/templates/setup.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.0.8/src/pyproject/templates/tests.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.0.8/src/pyproject/templates/tox.template
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 21:03:23.893024 pyproject-generator-0.0.8/src/pyproject_generator.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-29 21:03:23.000000 pyproject-generator-0.0.8/src/pyproject_generator.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)      766 2023-04-29 21:03:23.000000 pyproject-generator-0.0.8/src/pyproject_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-29 21:03:23.000000 pyproject-generator-0.0.8/src/pyproject_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-29 21:03:23.000000 pyproject-generator-0.0.8/src/pyproject_generator.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-04-29 21:03:23.000000 pyproject-generator-0.0.8/src/pyproject_generator.egg-info/requires.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-29 21:03:23.000000 pyproject-generator-0.0.8/src/pyproject_generator.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 21:03:23.894188 pyproject-generator-0.0.8/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.0.8/tests/test_pyproject.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:34:34.242709 pyproject-generator-0.0.9/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2082 2023-04-30 11:34:34.242889 pyproject-generator-0.0.9/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1563 2023-04-30 01:14:26.000000 pyproject-generator-0.0.9/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-19 15:24:26.000000 pyproject-generator-0.0.9/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-04-30 11:34:34.243928 pyproject-generator-0.0.9/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:34:34.218305 pyproject-generator-0.0.9/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:34:34.223891 pyproject-generator-0.0.9/src/pyproject/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-19 15:24:27.000000 pyproject-generator-0.0.9/src/pyproject/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-30 11:34:19.000000 pyproject-generator-0.0.9/src/pyproject/__version__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3059 2023-04-30 11:31:44.000000 pyproject-generator-0.0.9/src/pyproject/cli.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:34:34.226912 pyproject-generator-0.0.9/src/pyproject/config/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.0.9/src/pyproject/config/config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      259 2023-04-30 01:22:22.000000 pyproject-generator-0.0.9/src/pyproject/config/default_config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     9026 2023-04-30 11:23:07.000000 pyproject-generator-0.0.9/src/pyproject/project_builder.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:34:34.235875 pyproject-generator-0.0.9/src/pyproject/templates/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.0.9/src/pyproject/templates/gitignore.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.0.9/src/pyproject/templates/license_apache.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.0.9/src/pyproject/templates/license_mit.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.0.9/src/pyproject/templates/pyproject.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.0.9/src/pyproject/templates/readme.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      578 2023-04-14 17:03:04.000000 pyproject-generator-0.0.9/src/pyproject/templates/setup.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.0.9/src/pyproject/templates/tests.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.0.9/src/pyproject/templates/tox.template
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:34:34.241601 pyproject-generator-0.0.9/src/pyproject_generator.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2082 2023-04-30 11:34:34.000000 pyproject-generator-0.0.9/src/pyproject_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      859 2023-04-30 11:34:34.000000 pyproject-generator-0.0.9/src/pyproject_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-30 11:34:34.000000 pyproject-generator-0.0.9/src/pyproject_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-30 11:34:34.000000 pyproject-generator-0.0.9/src/pyproject_generator.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-04-30 11:34:34.000000 pyproject-generator-0.0.9/src/pyproject_generator.egg-info/requires.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-30 11:34:34.000000 pyproject-generator-0.0.9/src/pyproject_generator.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 11:34:34.242230 pyproject-generator-0.0.9/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.0.9/tests/test_pyproject.py
```

### Comparing `pyproject-generator-0.0.8/PKG-INFO` & `pyproject-generator-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pyproject-generator
-Version: 0.0.8
-Summary: A command line tool to setup Python packages
-Home-page: https://github.com/CangyuanLi/pyproject
-Author: Cangyuan Li
-Author-email: everest229@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # pyproject: 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyproject)
 
 ## What is it?
 
 **pyproject** is a command line utility to setup and distribute Python packages.
 
@@ -37,14 +22,17 @@
 ## Running
 
 Simply run 
 ```sh
 pyproject init {project_name}
 ```
 
+to create your project folder. It will automatically setup a package structure, virtual
+environment, and install packages.
+
 **pyproject** also allows you to configure your author name, email, Github url,
 PyPI username and password, and a list of default dependencies that you want to install. 
 Please note that your credentials are simply stored locally as plaintext. 
 If you do not wish to store them, you can simply pass them in manually
 via the --pypi_username and --pypi_password flags. To configure, run
 
 ```sh
```

### Comparing `pyproject-generator-0.0.8/setup.cfg` & `pyproject-generator-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.8/src/pyproject/cli.py` & `pyproject-generator-0.0.9/src/pyproject/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 import argparse
 import typing
 
 from .project_builder import Action, ProjectBuilder
 from .__version__ import __version__
 
 ACTIONS = list(typing.get_args(Action))
+LICENSES = ("apache", "mit")
 
 
 def get_parser():
     parser = argparse.ArgumentParser(description="Generate python project")
 
     parser.add_argument("action", type=str, choices=ACTIONS, help="Action")
     parser.add_argument(
         "project_name", type=str, nargs="?", default=None, help="Name of the project"
     )
 
     parser.add_argument(
         "--reset_config",
         required=False,
         action="store_true",
-        help="Reset configuration to default settings",
+        help="Reset configuration to default settings.",
     )
     parser.add_argument("--pypi_username", type=str, help="Set PyPI username")
     parser.add_argument("--pypi_password", type=str, help="Set PyPI password")
     parser.add_argument("--github_url", type=str, help="Set Github URL")
     parser.add_argument("--author", type=str, help="Set author name")
     parser.add_argument("--email", type=str, help="Set author email")
+    parser.add_argument("--license", type=str, choices=LICENSES, help="Set license")
     parser.add_argument(
         "--set_dependencies",
         type=str,
         help=(
             "Set dependencies to always download. Overwrites saved config. Pass in a"
-            " comma delimited string."
+            " comma delimited string"
         ),
     )
     parser.add_argument(
         "--add_dependencies",
         type=str,
-        help="Add dependencies to always download. Pass in a comma delimited string.",
+        help="Add dependencies to always download. Pass in a comma delimited string",
     )
     parser.add_argument(
         "--remove_dependencies",
         type=str,
-        help=(
-            "Remove dependencies to always download. Pass in a comma delimited string."
-        ),
+        help="Remove dependencies to always download. Pass in a comma delimited string",
     )
     parser.add_argument(
         "--show", required=False, action="store_true", help="Show the current config"
     )
+    parser.add_argument(
+        "--update",
+        required=False,
+        action="store_true",
+        help="If there are new keys in the default config, add them to the user config",
+    )
 
     parser.add_argument(
         "-v",
         "--version",
         action="version",
         version="%(prog)s {version}".format(version=__version__),
         help="Displays package version",
@@ -70,19 +76,21 @@
 
     config: dict[str, str] = {
         "pypi_username": args.pypi_username,
         "pypi_password": args.pypi_password,
         "github_url": args.github_url,
         "author": args.author,
         "email": args.email,
+        "license": args.license,
         "set_dependencies": args.set_dependencies,
         "add_dependencies": args.add_dependencies,
         "remove_dependencies": args.remove_dependencies,
         "reset_config": args.reset_config,
         "show": args.show,
+        "update": args.update,
     }
 
     builder = ProjectBuilder(config=config)
     builder.dispatch(action=args.action, project_name=args.project_name)
 
 
 if __name__ == "__main__":
```

### Comparing `pyproject-generator-0.0.8/src/pyproject/project_builder.py` & `pyproject-generator-0.0.9/src/pyproject/project_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Imports
 
+import datetime
 import os
 import json
 from pathlib import Path
 import pprint
 import re
 import shutil
 import subprocess
@@ -103,14 +104,15 @@
         d = {
             "PACKAGE": project_name,
             "PYPI_USERNAME": config["pypi_username"],
             "PYPI_PASSWORD": config["pypi_password"],
             "GITHUB_URL": config["github_url"],
             "AUTHOR": config["author"],
             "EMAIL": config["email"],
+            "YEAR": datetime.datetime.now().year,
         }
 
         filled_in_templates = {}
         for file in self._template_path.glob("*.template"):
             with open(file, "r") as f:
                 src = string.Template(f.read())
                 result = src.substitute(d)
@@ -156,14 +158,17 @@
         # misc setup
         (proj_path / "tox.ini").write_text(templates["tox"])
         (proj_path / "pyproject.toml").write_text(templates["pyproject"])
         (proj_path / "setup.cfg").write_text(templates["setup"])
         (proj_path / ".gitignore").write_text(templates["gitignore"])
         (proj_path / "README.md").write_text(templates["readme"])
 
+        license = self._config["license"]
+        (proj_path / "LICENSE").write_text(templates[f"license_{license}"])
+
         # Setup the virtual environment
 
         venv_builder = Env(with_pip=True)
         venv_builder.venv_create(proj_path / "venv")
         venv_builder.run_bin(["python", "-m", "pip", "install", "-U", "pip"])
 
         # Install developer dependencies
@@ -173,16 +178,18 @@
         # Create requirements_dev file
         reqs = venv_builder.run_bin(["pip", "freeze"], capture_output=True)
         (proj_path / "requirements_dev.txt").write_bytes(reqs.stdout)
 
     def _parse_config_file(self, filename: PathLike) -> dict:
         if filename == "default_config.json":
             path = BASE_PATH / "config/default_config.json"
-        else:
+        elif filename == "config.json":
             path = self._user_config_dir / filename
+        else:
+            raise ValueError("Name wrong.")
 
         with open(path) as f:
             config: dict = json.load(f)
 
         return config
 
     @staticmethod
@@ -212,30 +219,48 @@
 
         config["dependencies"] = (
             config["dependencies"] | config["add_dependencies"]
         ) - config["remove_dependencies"]
 
         merged_config = {}
         for k, v in saved_config.items():
-            if config[k] is None:
+            if k not in config:
+                merged_config[k] = v
+            elif config[k] is None:
                 merged_config[k] = v
             else:
                 merged_config[k] = config[k]
 
         if config["show"]:
             pprint.pprint(merged_config)
 
+        if config["update"]:
+            self.update_config(merged_config)
+
         return merged_config
 
-    def config(self):
-        config = self._config
+    def _write_config_file(self, config: dict):
         config["dependencies"] = list(config["dependencies"])
         with open(self._user_config_dir / "config.json", "w") as f:
             json.dump(config, f, indent=4)
 
+    def update_config(self, config):
+        default = self._parse_config_file("default_config.json")
+        merged_config = {}
+        for k, v in default.items():
+            if k not in config:
+                merged_config[k] = v
+            else:
+                merged_config[k] = config[k]
+
+        self._write_config_file(config)
+
+    def config(self):
+        self._write_config_file(self._config)
+
     def upload(self):
         username = self._config["pypi_username"]
         password = self._config["pypi_password"]
 
         env = Env()
 
         shutil.rmtree(self.proj_path / "dist", ignore_errors=True)
```

### Comparing `pyproject-generator-0.0.8/src/pyproject/templates/gitignore.template` & `pyproject-generator-0.0.9/src/pyproject/templates/gitignore.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.8/src/pyproject/templates/setup.template` & `pyproject-generator-0.0.9/src/pyproject/templates/setup.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.8/src/pyproject/templates/tests.template` & `pyproject-generator-0.0.9/src/pyproject/templates/tests.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.8/src/pyproject_generator.egg-info/PKG-INFO` & `pyproject-generator-0.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.0.8
+Version: 0.0.9
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
@@ -37,14 +37,17 @@
 ## Running
 
 Simply run 
 ```sh
 pyproject init {project_name}
 ```
 
+to create your project folder. It will automatically setup a package structure, virtual
+environment, and install packages.
+
 **pyproject** also allows you to configure your author name, email, Github url,
 PyPI username and password, and a list of default dependencies that you want to install. 
 Please note that your credentials are simply stored locally as plaintext. 
 If you do not wish to store them, you can simply pass them in manually
 via the --pypi_username and --pypi_password flags. To configure, run
 
 ```sh
```

### Comparing `pyproject-generator-0.0.8/src/pyproject_generator.egg-info/SOURCES.txt` & `pyproject-generator-0.0.9/src/pyproject_generator.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 src/pyproject/__init__.py
 src/pyproject/__version__.py
 src/pyproject/cli.py
 src/pyproject/project_builder.py
 src/pyproject/config/config.json
 src/pyproject/config/default_config.json
 src/pyproject/templates/gitignore.template
+src/pyproject/templates/license_apache.template
+src/pyproject/templates/license_mit.template
 src/pyproject/templates/pyproject.template
 src/pyproject/templates/readme.template
 src/pyproject/templates/setup.template
 src/pyproject/templates/tests.template
 src/pyproject/templates/tox.template
 src/pyproject_generator.egg-info/PKG-INFO
 src/pyproject_generator.egg-info/SOURCES.txt
```

