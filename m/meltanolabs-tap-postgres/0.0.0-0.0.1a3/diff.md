# Comparing `tmp/meltanolabs_tap_postgres-0.0.0.tar.gz` & `tmp/meltanolabs_tap_postgres-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltanolabs_tap_postgres-0.0.0.tar", max compression
+gzip compressed data, was "meltanolabs_tap_postgres-0.0.1a3.tar", max compression
```

## Comparing `meltanolabs_tap_postgres-0.0.0.tar` & `meltanolabs_tap_postgres-0.0.1a3.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     4268 2023-04-27 15:39:36.235767 meltanolabs_tap_postgres-0.0.0/README.md
--rw-r--r--   0        0        0     1852 2023-04-30 19:57:50.971606 meltanolabs_tap_postgres-0.0.0/pyproject.toml
--rw-r--r--   0        0        0       61 2023-02-10 16:16:20.889085 meltanolabs_tap_postgres-0.0.0/tap_postgres/__init__.py
--rw-r--r--   0        0        0     6162 2023-04-30 19:49:51.268046 meltanolabs_tap_postgres-0.0.0/tap_postgres/client.py
--rw-r--r--   0        0        0     7262 2023-04-27 15:39:36.235767 meltanolabs_tap_postgres-0.0.0/tap_postgres/tap.py
--rw-r--r--   0        0        0     5347 1970-01-01 00:00:00.000000 meltanolabs_tap_postgres-0.0.0/setup.py
--rw-r--r--   0        0        0     5591 1970-01-01 00:00:00.000000 meltanolabs_tap_postgres-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4268 2023-04-30 21:45:34.786831 meltanolabs_tap_postgres-0.0.1a3/README.md
+-rw-r--r--   0        0        0     1894 2023-04-30 21:45:54.438543 meltanolabs_tap_postgres-0.0.1a3/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-04-30 21:45:34.790831 meltanolabs_tap_postgres-0.0.1a3/tap_postgres/__init__.py
+-rw-r--r--   0        0        0     6162 2023-04-30 21:45:34.790831 meltanolabs_tap_postgres-0.0.1a3/tap_postgres/client.py
+-rw-r--r--   0        0        0     7262 2023-04-30 21:45:34.790831 meltanolabs_tap_postgres-0.0.1a3/tap_postgres/tap.py
+-rw-r--r--   0        0        0     5661 1970-01-01 00:00:00.000000 meltanolabs_tap_postgres-0.0.1a3/PKG-INFO
```

### Comparing `meltanolabs_tap_postgres-0.0.0/README.md` & `meltanolabs_tap_postgres-0.0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `meltanolabs_tap_postgres-0.0.0/pyproject.toml` & `meltanolabs_tap_postgres-0.0.1a3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "meltanolabs-tap-postgres"
-version = "0.0.0"
+version = "0.0.1a3"
 description = "`tap-postgres` is a Singer tap for Postgres, built with the Meltano SDK for Singer Targets."
-authors = ["Meltano Team and Contributors"]
-maintainers = ["Meltano Team and Contributors"]
+authors = ["Meltano Team and Contributors <hello@meltano.com>"]
+maintainers = ["Meltano Team and Contributors <hello@meltano.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://meltano.com"
 repository = "https://github.com/meltanolabs/tap-postgres"
 keywords = [
     "Postgres",
     "Singer",
```

### Comparing `meltanolabs_tap_postgres-0.0.0/tap_postgres/client.py` & `meltanolabs_tap_postgres-0.0.1a3/tap_postgres/client.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_tap_postgres-0.0.0/tap_postgres/tap.py` & `meltanolabs_tap_postgres-0.0.1a3/tap_postgres/tap.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_tap_postgres-0.0.0/setup.py` & `meltanolabs_tap_postgres-0.0.1a3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,151 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: meltanolabs-tap-postgres
+Version: 0.0.1a3
+Summary: `tap-postgres` is a Singer tap for Postgres, built with the Meltano SDK for Singer Targets.
+Home-page: https://meltano.com
+License: MIT
+Keywords: Postgres,Singer,ELT,Meltano,Meltano SDK
+Author: Meltano Team and Contributors
+Author-email: hello@meltano.com
+Maintainer: Meltano Team and Contributors
+Maintainer-email: hello@meltano.com
+Requires-Python: >=3.8.1,<3.12
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Dist: psycopg2-binary (==2.9.6)
+Requires-Dist: requests (>=2.25.1,<3.0.0)
+Requires-Dist: singer-sdk[testing] (>=0.24.0,<0.25.0)
+Requires-Dist: sshtunnel (==0.4.0)
+Project-URL: Repository, https://github.com/meltanolabs/tap-postgres
+Description-Content-Type: text/markdown
+
+# `tap-postgres`
+
+Singer tap for Postgres.
+
+Built with the [Meltano Singer SDK](https://sdk.meltano.com).
+
+## Capabilities
+
+* `catalog`
+* `state`
+* `discover`
+* `about`
+* `stream-maps`
+* `schema-flattening`
+
+## Settings
+
+| Setting             | Required | Default | Description |
+|:--------------------|:--------:|:-------:|:------------|
+| sqlalchemy_url      | True     | None    | Example postgresql://postgres:postgres@localhost:5432/postgres |
+| ssh_tunnel          | False    | None    | SSH Tunnel Configuration, this is a json object. |
+| ssh_tunnel.enable   | True (if ssh_tunnel set) | False   | Enable an ssh tunnel (also known as bastion host), see the other ssh_tunnel.* properties for more details.
+| ssh_tunnel.host | True (if ssh_tunnel set) | False   | Host of the bastion host, this is the host we'll connect to via ssh
+| ssh_tunnel.username | True (if ssh_tunnel set) | False   |Username to connect to bastion host
+| ssh_tunnel.port | True (if ssh_tunnel set) | 22 | Port to connect to bastion host
+| ssh_tunnel.private_key | True (if ssh_tunnel set) | None | Private Key for authentication to the bastion host
+| ssh_tunnel.private_key_password | False | None | Private Key Password, leave None if no password is set
+| stream_maps         | False    | None    | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |
+| stream_map_config   | False    | None    | User-defined config values to be used within map expressions. |
+| flattening_enabled  | False    | None    | 'True' to enable schema flattening and automatically expand nested properties. |
+| flattening_max_depth| False    | None    | The max depth to flatten schemas. |
+
+A full list of supported settings and capabilities is available by running: `tap-postgres --about`
+
+### Configure using environment variables
+
+This Singer tap will automatically import any environment variables within the working directory's
+`.env` if the `--config=ENV` is provided, such that config values will be considered if a matching
+environment variable is set either in the terminal context or in the `.env` file.
+
+### SSH Tunnels (Bastion Hosts)
+
+This tap supports connecting to a Postgres database via an SSH tunnel (also known as a bastion host). This is useful if you need to connect to a database that is not publicly accessible. This is the same as using `ssh -L` and `ssh -R`, but this is done inside the tap itself.
+
+## Installation
+
+- [ ] `Developer TODO:` Update the below as needed to correctly describe the install procedure. For instance, if you do not have a PyPi repo, or if you want users to directly install from your git repo, you can modify this step as appropriate.
+
+```bash
+pipx install tap-postgres
+```
+
+## Usage
+
+You can easily run `tap-postgres` by itself or in a pipeline using [Meltano](https://meltano.com/).
+
+### Executing the Tap Directly
+
+```bash
+tap-postgres --version
+tap-postgres --help
+tap-postgres --config CONFIG --discover > ./catalog.json
+```
+
+## Developer Resources
+
+### Initialize your Development Environment
+
+```bash
+pipx install poetry
+poetry install
+```
+
+### Create and Run Tests
+
+Create tests within the `tap_postgres/tests` subfolder and
+  then run:
+
+```bash
+poetry run pytest
+```
+
+You can also test the `tap-postgres` CLI interface directly using `poetry run`:
+
+```bash
+poetry run tap-postgres --help
+```
+
+### Testing with [Meltano](https://www.meltano.com)
+
+_**Note:** This tap will work in any Singer environment and does not require Meltano.
+Examples here are for convenience and to streamline end-to-end orchestration scenarios._
+
+Your project comes with a custom `meltano.yml` project file already created.
+
+Next, install Meltano (if you haven't already) and any needed plugins:
+
+```bash
+# Install meltano
+pipx install meltano
+# Initialize meltano within this directory
+cd tap-postgres
+meltano install
+```
+
+Now you can test and orchestrate using Meltano:
+
+```bash
+# Test invocation:
+meltano invoke tap-postgres --version
+# OR run a test `elt` pipeline:
+meltano elt tap-postgres target-jsonl
+```
 
-packages = \
-['tap_postgres']
+### SDK Dev Guide
 
-package_data = \
-{'': ['*']}
+See the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the SDK to
+develop your own taps and targets.
 
-install_requires = \
-['psycopg2-binary==2.9.6',
- 'requests>=2.25.1,<3.0.0',
- 'singer-sdk[testing]>=0.24.0,<0.25.0',
- 'sshtunnel==0.4.0']
-
-entry_points = \
-{'console_scripts': ['tap-postgres = tap_postgres.tap:TapPostgres.cli']}
-
-setup_kwargs = {
-    'name': 'meltanolabs-tap-postgres',
-    'version': '0.0.0',
-    'description': '`tap-postgres` is a Singer tap for Postgres, built with the Meltano SDK for Singer Targets.',
-    'long_description': "# `tap-postgres`\n\nSinger tap for Postgres.\n\nBuilt with the [Meltano Singer SDK](https://sdk.meltano.com).\n\n## Capabilities\n\n* `catalog`\n* `state`\n* `discover`\n* `about`\n* `stream-maps`\n* `schema-flattening`\n\n## Settings\n\n| Setting             | Required | Default | Description |\n|:--------------------|:--------:|:-------:|:------------|\n| sqlalchemy_url      | True     | None    | Example postgresql://postgres:postgres@localhost:5432/postgres |\n| ssh_tunnel          | False    | None    | SSH Tunnel Configuration, this is a json object. |\n| ssh_tunnel.enable   | True (if ssh_tunnel set) | False   | Enable an ssh tunnel (also known as bastion host), see the other ssh_tunnel.* properties for more details.\n| ssh_tunnel.host | True (if ssh_tunnel set) | False   | Host of the bastion host, this is the host we'll connect to via ssh\n| ssh_tunnel.username | True (if ssh_tunnel set) | False   |Username to connect to bastion host\n| ssh_tunnel.port | True (if ssh_tunnel set) | 22 | Port to connect to bastion host\n| ssh_tunnel.private_key | True (if ssh_tunnel set) | None | Private Key for authentication to the bastion host\n| ssh_tunnel.private_key_password | False | None | Private Key Password, leave None if no password is set\n| stream_maps         | False    | None    | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |\n| stream_map_config   | False    | None    | User-defined config values to be used within map expressions. |\n| flattening_enabled  | False    | None    | 'True' to enable schema flattening and automatically expand nested properties. |\n| flattening_max_depth| False    | None    | The max depth to flatten schemas. |\n\nA full list of supported settings and capabilities is available by running: `tap-postgres --about`\n\n### Configure using environment variables\n\nThis Singer tap will automatically import any environment variables within the working directory's\n`.env` if the `--config=ENV` is provided, such that config values will be considered if a matching\nenvironment variable is set either in the terminal context or in the `.env` file.\n\n### SSH Tunnels (Bastion Hosts)\n\nThis tap supports connecting to a Postgres database via an SSH tunnel (also known as a bastion host). This is useful if you need to connect to a database that is not publicly accessible. This is the same as using `ssh -L` and `ssh -R`, but this is done inside the tap itself.\n\n## Installation\n\n- [ ] `Developer TODO:` Update the below as needed to correctly describe the install procedure. For instance, if you do not have a PyPi repo, or if you want users to directly install from your git repo, you can modify this step as appropriate.\n\n```bash\npipx install tap-postgres\n```\n\n## Usage\n\nYou can easily run `tap-postgres` by itself or in a pipeline using [Meltano](https://meltano.com/).\n\n### Executing the Tap Directly\n\n```bash\ntap-postgres --version\ntap-postgres --help\ntap-postgres --config CONFIG --discover > ./catalog.json\n```\n\n## Developer Resources\n\n### Initialize your Development Environment\n\n```bash\npipx install poetry\npoetry install\n```\n\n### Create and Run Tests\n\nCreate tests within the `tap_postgres/tests` subfolder and\n  then run:\n\n```bash\npoetry run pytest\n```\n\nYou can also test the `tap-postgres` CLI interface directly using `poetry run`:\n\n```bash\npoetry run tap-postgres --help\n```\n\n### Testing with [Meltano](https://www.meltano.com)\n\n_**Note:** This tap will work in any Singer environment and does not require Meltano.\nExamples here are for convenience and to streamline end-to-end orchestration scenarios._\n\nYour project comes with a custom `meltano.yml` project file already created.\n\nNext, install Meltano (if you haven't already) and any needed plugins:\n\n```bash\n# Install meltano\npipx install meltano\n# Initialize meltano within this directory\ncd tap-postgres\nmeltano install\n```\n\nNow you can test and orchestrate using Meltano:\n\n```bash\n# Test invocation:\nmeltano invoke tap-postgres --version\n# OR run a test `elt` pipeline:\nmeltano elt tap-postgres target-jsonl\n```\n\n### SDK Dev Guide\n\nSee the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the SDK to\ndevelop your own taps and targets.\n",
-    'author': 'Meltano Team and Contributors',
-    'author_email': 'None',
-    'maintainer': 'Meltano Team and Contributors',
-    'maintainer_email': 'None',
-    'url': 'https://meltano.com',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8.1,<3.12',
-}
-
-
-setup(**setup_kwargs)
```

