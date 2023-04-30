# Comparing `tmp/sigma_cli-0.7.2.tar.gz` & `tmp/sigma_cli-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigma_cli-0.7.2.tar", max compression
+gzip compressed data, was "sigma_cli-0.7.3.tar", max compression
```

## Comparing `sigma_cli-0.7.2.tar` & `sigma_cli-0.7.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3440 2023-03-03 22:22:02.427126 sigma_cli-0.7.2/README.md
--rw-r--r--   0        0        0     1017 2023-03-03 22:22:02.427126 sigma_cli-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     5593 2023-03-03 22:22:02.427126 sigma_cli-0.7.2/sigma/cli/check.py
--rw-r--r--   0        0        0     9156 2023-03-03 22:22:02.427126 sigma_cli-0.7.2/sigma/cli/convert.py
--rw-r--r--   0        0        0     2938 2023-03-03 22:22:02.427126 sigma_cli-0.7.2/sigma/cli/list.py
--rw-r--r--   0        0        0      361 2023-03-03 22:22:02.427126 sigma_cli-0.7.2/sigma/cli/main.py
--rw-r--r--   0        0        0     3729 2023-03-03 22:22:02.427126 sigma_cli-0.7.2/sigma/cli/plugin.py
--rw-r--r--   0        0        0      473 2023-03-03 22:22:02.427126 sigma_cli-0.7.2/sigma/cli/rules.py
--rw-r--r--   0        0        0     4422 1970-01-01 00:00:00.000000 sigma_cli-0.7.2/setup.py
--rw-r--r--   0        0        0     4648 1970-01-01 00:00:00.000000 sigma_cli-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     3440 2023-04-30 10:12:10.273470 sigma_cli-0.7.3/README.md
+-rw-r--r--   0        0        0     1017 2023-04-30 10:12:10.273470 sigma_cli-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     5629 2023-04-30 10:12:10.273470 sigma_cli-0.7.3/sigma/cli/check.py
+-rw-r--r--   0        0        0     9173 2023-04-30 10:12:10.273470 sigma_cli-0.7.3/sigma/cli/convert.py
+-rw-r--r--   0        0        0     5047 2023-04-30 10:12:10.273470 sigma_cli-0.7.3/sigma/cli/list.py
+-rw-r--r--   0        0        0      361 2023-04-30 10:12:10.273470 sigma_cli-0.7.3/sigma/cli/main.py
+-rw-r--r--   0        0        0     3729 2023-04-30 10:12:10.277470 sigma_cli-0.7.3/sigma/cli/plugin.py
+-rw-r--r--   0        0        0      714 2023-04-30 10:12:10.277470 sigma_cli-0.7.3/sigma/cli/rules.py
+-rw-r--r--   0        0        0     4422 1970-01-01 00:00:00.000000 sigma_cli-0.7.3/setup.py
+-rw-r--r--   0        0        0     4648 1970-01-01 00:00:00.000000 sigma_cli-0.7.3/PKG-INFO
```

### Comparing `sigma_cli-0.7.2/README.md` & `sigma_cli-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `sigma_cli-0.7.2/pyproject.toml` & `sigma_cli-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sigma-cli"
-version = "0.7.2"
+version = "0.7.3"
 description = "Sigma Command Line Interface (conversion, check etc.) based on pySigma"
 authors = ["Thomas Patzke <thomas@patzke.org>"]
 license = "LGPL-2.1-or-later"
 readme = "README.md"
 repository = "https://github.com/SigmaHQ/sigma-cli"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `sigma_cli-0.7.2/sigma/cli/check.py` & `sigma_cli-0.7.3/sigma/cli/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     default=False,
     show_default=True,
     help="Fail on Sigma rule validation issues.",
 )
 @click.argument(
     "input",
     nargs=-1,
-    type=click.Path(exists=True, path_type=pathlib.Path),
+    required=True,
+    type=click.Path(exists=True, allow_dash=True, path_type=pathlib.Path),
 )
 def check(input, validation_config, file_pattern, fail_on_error, fail_on_issues):
     """Check Sigma rules for validity and best practices (not yet implemented)."""
     if validation_config is None:   # no validation config provided, use basic config with all validators
         rule_validator = SigmaValidator(validators.values())
     else:
         rule_validator = SigmaValidator.from_yaml(validation_config.read(), validators)
```

### Comparing `sigma_cli-0.7.2/sigma/cli/convert.py` & `sigma_cli-0.7.3/sigma/cli/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     multiple=True,
     help="Backend-specific options provided as key=value pair.",
 )
 @click.argument(
     "input",
     nargs=-1,
     required=True,
-    type=click.Path(exists=True, path_type=pathlib.Path),
+    type=click.Path(exists=True, allow_dash=True, path_type=pathlib.Path),
 )
 def convert(target, pipeline, without_pipeline, pipeline_check, format, skip_unsupported, output, encoding, json_indent, backend_option, input, file_pattern):
     """
     Convert Sigma rules into queries. INPUT can be multiple files or directories. This command automatically recurses
     into directories and converts all files matching the pattern in --file-pattern.
     """
     # Check if pipeline is required
```

### Comparing `sigma_cli-0.7.2/sigma/cli/plugin.py` & `sigma_cli-0.7.3/sigma/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `sigma_cli-0.7.2/setup.py` & `sigma_cli-0.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'pysigma>=0.9.5,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['sigma = sigma.cli.main:main']}
 
 setup_kwargs = {
     'name': 'sigma-cli',
-    'version': '0.7.2',
+    'version': '0.7.3',
     'description': 'Sigma Command Line Interface (conversion, check etc.) based on pySigma',
     'long_description': '# Sigma Command Line Interface\n\n![Tests](https://github.com/SigmaHQ/sigma-cli/actions/workflows/test.yml/badge.svg)\n![Coverage Badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/thomaspatzke/0c868df261d4a5d5a1dafe71b1557d69/raw/SigmaHQ-sigma-cli.json)\n![Status](https://img.shields.io/badge/Status-pre--release-orange)\n\nThis is the Sigma command line interface using the [pySigma](https://github.com/SigmaHQ/pySigma) library to manage, list\nand convert Sigma rules into query languages.\n\n## Getting Started\n\n### Installation\n\nThe easiest way to install the Sigma CLI is via *pipx* or *pip*. For this purpose run one of the following:\n\n```\npython -m pipx install sigma-cli\npython -m pip install sigma-cli\n```\non macOS use\n```\npython3 -m pip install sigma-cli\n```\n\nAnother way is to run this from source in a virtual environment managed by [Poetry](https://python-poetry.org/docs/basic-usage/):\n\n```\ngit clone https://github.com/SigmaHQ/sigma-cli.git\ncd sigma-cli\npoetry install\npoetry shell\n```\n\n### Usage\n\nThe CLI is available as *sigma* command. A typical invocation is:\n\n```\nsigma convert -t <backend> -p <processing pipeline 1> -p <processing pipeline 2> [...] <directory or file>\n```\n\nE.g. to convert process creation Sigma rules from a directory into Splunk queries for Sysmon logs run:\n\n```\nsigma convert -t splunk -p sysmon sigma/rules/windows/process_creation\n```\n\nAvailable conversion backends and processing pipelines can be listed with `sigma list`. \nUse `-O` or `--backend-option` for passing options to the backend as key=value pairs (`-O testparam=123`) .\nThis backend option parameter can be used multiple times (`-O first=123 -O second=456`).\n\nBackends can support different output formats, e.g. plain queries and a file that can be imported into the target\nsystem. These formats can be listed with `sigma list formats <backend>` and specified for conversion with the `-f`\noption.\n\nIn addition, an output file can be specified with `-o`.\n\nExample for output formats and files:\n\n```\nsigma convert -t splunk -f savedsearches -p sysmon -o savedsearches.conf sigma/rules/windows/process_creation\n```\n\nOutputs a Splunk savedsearches.conf containing the converted searches.\n\n### Integration of Backends and Pipelines\n\nBackends and pipelines can be integrated by adding the corresponding packages as dependency with:\n\n```\npoetry add <package name>\n```\n\nA backend has to be added to the `backends` dict in `sigma/cli/backends.py` by creation of a `Backend` named tuple with\nthe following parameters:\n\n* The backend class.\n* A display name shown to the user in the targets list (`sigma list targets`).\n* A dict that maps output format names (used in `-f` parameter) to descriptions of the formats that are shown in the\n  format list (`sigma list formats <backend>`). The formats must be supported by the backend!\n\nThe dict key is the name used in the `-t` parameter.\n\nA processing pipeline is defined in the `pipelines` variable dict in `sigma/cli/pipelines.py`. The variable contains a\n`ProcessingPipelineResolver` that is instantiated with a dict that maps identifiers that can\nbe used in the `-p` parameter to functions that return `ProcessingPipeline` objects. The descriptive text shown in the pipeline list (`sigma list pipelines`) is provided from\nthe `name` attribute of the `ProcessingPipeline` object.\n\n## Maintainers\n\nThe project is currently maintained by:\n\n- Thomas Patzke <thomas@patzke.org>\n',
     'author': 'Thomas Patzke',
     'author_email': 'thomas@patzke.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/SigmaHQ/sigma-cli',
```

### Comparing `sigma_cli-0.7.2/PKG-INFO` & `sigma_cli-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigma-cli
-Version: 0.7.2
+Version: 0.7.3
 Summary: Sigma Command Line Interface (conversion, check etc.) based on pySigma
 Home-page: https://github.com/SigmaHQ/sigma-cli
 License: LGPL-2.1-or-later
 Author: Thomas Patzke
 Author-email: thomas@patzke.org
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

