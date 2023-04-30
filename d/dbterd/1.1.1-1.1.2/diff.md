# Comparing `tmp/dbterd-1.1.1.tar.gz` & `tmp/dbterd-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbterd-1.1.1.tar", max compression
+gzip compressed data, was "dbterd-1.1.2.tar", max compression
```

## Comparing `dbterd-1.1.1.tar` & `dbterd-1.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1067 2023-04-27 16:08:23.050140 dbterd-1.1.1/LICENSE
--rw-r--r--   0        0        0     4504 2023-04-27 16:08:23.050140 dbterd-1.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/__init__.py
--rw-r--r--   0        0        0       37 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/__main__.py
--rw-r--r--   0        0        0        0 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/algos/__init__.py
--rw-r--r--   0        0        0     4465 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/algos/base.py
--rw-r--r--   0        0        0     3157 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/algos/filter.py
--rw-r--r--   0        0        0      545 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/algos/meta.py
--rw-r--r--   0        0        0     2505 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/algos/test_relationship.py
--rw-r--r--   0        0        0     2561 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/base.py
--rw-r--r--   0        0        0      560 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/factory.py
--rw-r--r--   0        0        0        0 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/targets/__init__.py
--rw-r--r--   0        0        0      132 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/targets/constants.py
--rw-r--r--   0        0        0      304 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/targets/dbml/__init__.py
--rw-r--r--   0        0        0     1373 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/targets/dbml/dbml_test_relationship.py
--rw-r--r--   0        0        0      168 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/targets/default.py
--rw-r--r--   0        0        0      316 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/targets/mermaid/__init__.py
--rw-r--r--   0        0        0     1597 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py
--rw-r--r--   0        0        0      222 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/worker.py
--rw-r--r--   0        0        0        0 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/cli/__init__.py
--rw-r--r--   0        0        0     2026 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/cli/main.py
--rw-r--r--   0        0        0     1928 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/cli/params.py
--rw-r--r--   0        0        0      284 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/default.py
--rw-r--r--   0        0        0        0 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/helpers/__init__.py
--rw-r--r--   0        0        0      721 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/helpers/cli_messaging.py
--rw-r--r--   0        0        0      877 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/helpers/dict.py
--rw-r--r--   0        0        0     4494 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/helpers/file.py
--rw-r--r--   0        0        0     1022 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/helpers/jsonify.py
--rw-r--r--   0        0        0      976 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/helpers/log.py
--rw-r--r--   0        0        0     1605 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/helpers/yaml.py
--rw-r--r--   0        0        0       94 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/main.py
--rw-r--r--   0        0        0     2111 2023-04-27 16:08:46.922338 dbterd-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     5551 1970-01-01 00:00:00.000000 dbterd-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      203 2023-04-30 10:54:44.787016 dbterd-1.1.2/LICENSE
+-rw-r--r--   0        0        0     4491 2023-04-30 10:54:44.787016 dbterd-1.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/__init__.py
+-rw-r--r--   0        0        0       37 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/algos/__init__.py
+-rw-r--r--   0        0        0     4465 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/algos/base.py
+-rw-r--r--   0        0        0     3157 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/algos/filter.py
+-rw-r--r--   0        0        0      545 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/algos/meta.py
+-rw-r--r--   0        0        0     2505 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/algos/test_relationship.py
+-rw-r--r--   0        0        0     2561 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/base.py
+-rw-r--r--   0        0        0      560 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/factory.py
+-rw-r--r--   0        0        0        0 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/targets/__init__.py
+-rw-r--r--   0        0        0      132 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/targets/constants.py
+-rw-r--r--   0        0        0      304 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/targets/dbml/__init__.py
+-rw-r--r--   0        0        0     1373 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/targets/dbml/dbml_test_relationship.py
+-rw-r--r--   0        0        0      168 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/targets/default.py
+-rw-r--r--   0        0        0      316 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/targets/mermaid/__init__.py
+-rw-r--r--   0        0        0     1597 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py
+-rw-r--r--   0        0        0      222 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/worker.py
+-rw-r--r--   0        0        0        0 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/cli/__init__.py
+-rw-r--r--   0        0        0     2026 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/cli/main.py
+-rw-r--r--   0        0        0     1928 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/cli/params.py
+-rw-r--r--   0        0        0      284 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/default.py
+-rw-r--r--   0        0        0        0 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/helpers/__init__.py
+-rw-r--r--   0        0        0      721 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/helpers/cli_messaging.py
+-rw-r--r--   0        0        0      877 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/helpers/dict.py
+-rw-r--r--   0        0        0     4494 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/helpers/file.py
+-rw-r--r--   0        0        0     1022 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/helpers/jsonify.py
+-rw-r--r--   0        0        0      976 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/helpers/log.py
+-rw-r--r--   0        0        0     1605 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/helpers/yaml.py
+-rw-r--r--   0        0        0       94 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/main.py
+-rw-r--r--   0        0        0     2095 2023-04-30 10:54:57.123205 dbterd-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5538 1970-01-01 00:00:00.000000 dbterd-1.1.2/PKG-INFO
```

### Comparing `dbterd-1.1.1/README.md` & `dbterd-1.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # dbterd
 CLI to generate Diagram-as-a-code file ([DBML](https://dbdiagram.io/d), [Mermaid](https://mermaid-js.github.io/mermaid-live-editor/)) from dbt artifact files (required: `manifest.json`, `catalog.json`)
-> Version 0.1: only required `manifest.json`
 
 [![PyPI version](https://badge.fury.io/py/dbterd.svg)](https://pypi.org/project/dbterd/)
 ![python-cli](https://img.shields.io/badge/CLI-Python-FFCE3E?labelColor=14354C&logo=python&logoColor=white)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![python](https://img.shields.io/badge/Python-3.9|3.10|3.11-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 [![codecov](https://codecov.io/gh/datnguye/dbterd/branch/main/graph/badge.svg?token=N7DMQBLH4P)](https://codecov.io/gh/datnguye/dbterd)
 
@@ -13,32 +12,14 @@
 ```
 
 Verify installed version:
 ```
 dbterd --version
 ```
 
-
-```bash
-dbterd -h
-Usage: dbterd [OPTIONS] COMMAND [ARGS]...
-
-  Tools for producing diagram-as-code
-
-Options:
-  --version   Show the version and exit.
-  -h, --help  Show this message and exit.
-
-Commands:
-  debug  Inspect the hidden magics
-  run    Run the convert
-
-  Specify one of these sub-commands and you can find more help from there.
-```
-
 ## Quick examine with existing samples
 ```bash
 # select all models in dbt_resto
 dbterd run -ad "samples/dbtresto" -o "target"
 # select all models in dbt_resto, Select multiple dbt resources
 dbterd run -ad "samples/dbtresto" -o "target" -rt "model" -rt "source"
 # select only models in dbt_resto excluding staging
@@ -119,7 +100,16 @@
 ![screencapture-dbdocs-io-datnguye-poc-2023-02-25-10_29_32.png](https://raw.githubusercontent.com/datnguye/dbterd/main/assets/images/screencapture-dbdocs-io-datnguye-poc-2023-02-25-10_29_32.png)
 
 
 ## Contributing ✨
 If you've ever wanted to contribute to this tool, and a great cause, now is your chance!
 
 See the contributing docs [CONTRIBUTING.md](https://github.com/datnguye/dbterd/blob/main/CONTRIBUTING.md) for more information
+
+
+## Contributors
+
+Thanks for all the great resources! Can't see your avatar? Check the [contribution guide](https://dbterd.datnguyen.de/latest/nav/development/contributing-guide.html) on how you can submit your resources to the community!
+
+<a href="https://github.com/datnguye/dbterd/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=datnguye/dbterd" />
+</a>
```

### Comparing `dbterd-1.1.1/dbterd/adapters/algos/base.py` & `dbterd-1.1.2/dbterd/adapters/algos/base.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.1/dbterd/adapters/algos/filter.py` & `dbterd-1.1.2/dbterd/adapters/algos/filter.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.1/dbterd/adapters/algos/meta.py` & `dbterd-1.1.2/dbterd/adapters/algos/meta.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.1/dbterd/adapters/algos/test_relationship.py` & `dbterd-1.1.2/dbterd/adapters/algos/test_relationship.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.1/dbterd/adapters/base.py` & `dbterd-1.1.2/dbterd/adapters/base.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.1/dbterd/adapters/factory.py` & `dbterd-1.1.2/dbterd/adapters/factory.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.1/dbterd/adapters/targets/dbml/dbml_test_relationship.py` & `dbterd-1.1.2/dbterd/adapters/targets/dbml/dbml_test_relationship.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.1/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py` & `dbterd-1.1.2/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.1/dbterd/cli/main.py` & `dbterd-1.1.2/dbterd/cli/main.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.1/dbterd/cli/params.py` & `dbterd-1.1.2/dbterd/cli/params.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.1/dbterd/helpers/cli_messaging.py` & `dbterd-1.1.2/dbterd/helpers/cli_messaging.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.1/dbterd/helpers/dict.py` & `dbterd-1.1.2/dbterd/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.1/dbterd/helpers/file.py` & `dbterd-1.1.2/dbterd/helpers/file.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.1/dbterd/helpers/jsonify.py` & `dbterd-1.1.2/dbterd/helpers/jsonify.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.1/dbterd/helpers/log.py` & `dbterd-1.1.2/dbterd/helpers/log.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.1/dbterd/helpers/yaml.py` & `dbterd-1.1.2/dbterd/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.1/pyproject.toml` & `dbterd-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbterd"
-version = "1.1.1"
+version = "1.1.2"
 description = "dbterd is a Command Line Interface (CLI) to convert dbt manifest.json file to diagram file"
 authors = ["Dat Nguyen <datnguyen.it09@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/datnguye/dbterd"
 repository = "https://github.com/datnguye/dbterd"
 keywords = ["flake8", "markdown", "lint"]
@@ -27,29 +27,28 @@
 dbterd = "dbterd.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.3"
 dbt-artifacts-parser = "^0.2.3"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^6.2.5"
 pytest-sugar = "^0.9.6"
 black = "^22.10.0"
 coverage = {version = "^6.5.0", extras = ["toml"]}
 poethepoet = "^0.16.4"
 pre-commit = "^2.20.0"
-
-[tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 autoflake = "^2.0.1"
 mkdocs = "^1.4.2"
 mkdocs-minify-plugin = "^0.6.4"
 mkdocs-material = "^9.1.5"
+mike = "^1.1.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 multi_line_output = 3
```

### Comparing `dbterd-1.1.1/PKG-INFO` & `dbterd-1.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbterd
-Version: 1.1.1
+Version: 1.1.2
 Summary: dbterd is a Command Line Interface (CLI) to convert dbt manifest.json file to diagram file
 Home-page: https://github.com/datnguye/dbterd
 License: MIT
 Keywords: flake8,markdown,lint
 Author: Dat Nguyen
 Author-email: datnguyen.it09@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -21,15 +21,14 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dbt-artifacts-parser (>=0.2.3,<0.3.0)
 Project-URL: Repository, https://github.com/datnguye/dbterd
 Description-Content-Type: text/markdown
 
 # dbterd
 CLI to generate Diagram-as-a-code file ([DBML](https://dbdiagram.io/d), [Mermaid](https://mermaid-js.github.io/mermaid-live-editor/)) from dbt artifact files (required: `manifest.json`, `catalog.json`)
-> Version 0.1: only required `manifest.json`
 
 [![PyPI version](https://badge.fury.io/py/dbterd.svg)](https://pypi.org/project/dbterd/)
 ![python-cli](https://img.shields.io/badge/CLI-Python-FFCE3E?labelColor=14354C&logo=python&logoColor=white)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![python](https://img.shields.io/badge/Python-3.9|3.10|3.11-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 [![codecov](https://codecov.io/gh/datnguye/dbterd/branch/main/graph/badge.svg?token=N7DMQBLH4P)](https://codecov.io/gh/datnguye/dbterd)
 
@@ -38,32 +37,14 @@
 ```
 
 Verify installed version:
 ```
 dbterd --version
 ```
 
-
-```bash
-dbterd -h
-Usage: dbterd [OPTIONS] COMMAND [ARGS]...
-
-  Tools for producing diagram-as-code
-
-Options:
-  --version   Show the version and exit.
-  -h, --help  Show this message and exit.
-
-Commands:
-  debug  Inspect the hidden magics
-  run    Run the convert
-
-  Specify one of these sub-commands and you can find more help from there.
-```
-
 ## Quick examine with existing samples
 ```bash
 # select all models in dbt_resto
 dbterd run -ad "samples/dbtresto" -o "target"
 # select all models in dbt_resto, Select multiple dbt resources
 dbterd run -ad "samples/dbtresto" -o "target" -rt "model" -rt "source"
 # select only models in dbt_resto excluding staging
@@ -145,7 +126,16 @@
 
 
 ## Contributing ✨
 If you've ever wanted to contribute to this tool, and a great cause, now is your chance!
 
 See the contributing docs [CONTRIBUTING.md](https://github.com/datnguye/dbterd/blob/main/CONTRIBUTING.md) for more information
 
+
+## Contributors
+
+Thanks for all the great resources! Can't see your avatar? Check the [contribution guide](https://dbterd.datnguyen.de/latest/nav/development/contributing-guide.html) on how you can submit your resources to the community!
+
+<a href="https://github.com/datnguye/dbterd/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=datnguye/dbterd" />
+</a>
+
```

