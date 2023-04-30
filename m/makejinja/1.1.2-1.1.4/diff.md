# Comparing `tmp/makejinja-1.1.2.tar.gz` & `tmp/makejinja-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makejinja-1.1.2.tar", max compression
+gzip compressed data, was "makejinja-1.1.4.tar", max compression
```

## Comparing `makejinja-1.1.2.tar` & `makejinja-1.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-02-14 12:36:13.521906 makejinja-1.1.2/LICENSE
--rw-r--r--   0        0        0    16660 2023-02-14 12:36:13.521906 makejinja-1.1.2/README.md
--rw-r--r--   0        0        0      101 2023-02-14 12:36:13.521906 makejinja-1.1.2/makejinja/__init__.py
--rw-r--r--   0        0        0       48 2023-02-14 12:36:13.521906 makejinja-1.1.2/makejinja/__main__.py
--rw-r--r--   0        0        0     6304 2023-02-14 12:36:13.521906 makejinja-1.1.2/makejinja/app.py
--rw-r--r--   0        0        0      544 2023-02-14 12:36:13.521906 makejinja-1.1.2/makejinja/cli.py
--rw-r--r--   0        0        0    12184 2023-02-14 12:36:13.521906 makejinja-1.1.2/makejinja/config.py
--rw-r--r--   0        0        0     1060 2023-02-14 12:36:13.521906 makejinja-1.1.2/makejinja/loader.py
--rw-r--r--   0        0        0        0 2023-02-14 12:36:13.521906 makejinja-1.1.2/makejinja/py.typed
--rw-r--r--   0        0        0      843 2023-02-14 12:36:44.290370 makejinja-1.1.2/pyproject.toml
--rw-r--r--   0        0        0    17871 1970-01-01 00:00:00.000000 makejinja-1.1.2/setup.py
--rw-r--r--   0        0        0    17574 1970-01-01 00:00:00.000000 makejinja-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-30 13:14:01.745901 makejinja-1.1.4/LICENSE
+-rw-r--r--   0        0        0    16660 2023-04-30 13:14:01.745901 makejinja-1.1.4/README.md
+-rw-r--r--   0        0        0      101 2023-04-30 13:14:01.745901 makejinja-1.1.4/makejinja/__init__.py
+-rw-r--r--   0        0        0       48 2023-04-30 13:14:01.745901 makejinja-1.1.4/makejinja/__main__.py
+-rw-r--r--   0        0        0     5805 2023-04-30 13:14:01.745901 makejinja-1.1.4/makejinja/app.py
+-rw-r--r--   0        0        0     1291 2023-04-30 13:14:01.745901 makejinja-1.1.4/makejinja/cli.py
+-rw-r--r--   0        0        0    12184 2023-04-30 13:14:01.745901 makejinja-1.1.4/makejinja/config.py
+-rw-r--r--   0        0        0     1060 2023-04-30 13:14:01.745901 makejinja-1.1.4/makejinja/loader.py
+-rw-r--r--   0        0        0        0 2023-04-30 13:14:01.745901 makejinja-1.1.4/makejinja/py.typed
+-rw-r--r--   0        0        0      811 2023-04-30 13:15:24.797858 makejinja-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0    17867 1970-01-01 00:00:00.000000 makejinja-1.1.4/setup.py
+-rw-r--r--   0        0        0    17520 1970-01-01 00:00:00.000000 makejinja-1.1.4/PKG-INFO
```

### Comparing `makejinja-1.1.2/LICENSE` & `makejinja-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `makejinja-1.1.2/README.md` & `makejinja-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `makejinja-1.1.2/makejinja/app.py` & `makejinja-1.1.4/makejinja/app.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,21 +19,15 @@
 
 from makejinja.config import Config
 
 __all__ = ["makejinja"]
 
 
 def makejinja(config: Config):
-    """makejinja can be used to automatically generate files from [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/templates/).
-
-    Instead of passing CLI options, you can also write them to a file called `.makejinja.toml` in your working directory.
-    **Note**: In this file, options may be named differently.
-    Please refer to the file [`makejinja/config.py`](https://github.com/mirkolenz/makejinja/blob/main/makejinja/config.py) to see their actual names.
-    You will also find an example here: [`makejinja/tests/data/.makejinja.toml`](https://github.com/mirkolenz/makejinja/blob/main/tests/data/.makejinja.toml).
-    """
+    """makejinja can be used to automatically generate files from [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/templates/)."""
 
     for path in config.import_paths:
         sys.path.append(str(path.resolve()))
 
     data = load_data(config)
     env = init_jinja_env(config)
```

### Comparing `makejinja-1.1.2/makejinja/cli.py` & `makejinja-1.1.4/makejinja/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from pathlib import Path
+from typing import Type, cast
 
 import rich_click as click
 import typed_settings as ts
+from typed_settings.types import AttrsInstance
 
 from makejinja.config import OPTION_GROUPS, Config
 
 from .app import makejinja
 
 __all__ = ["makejinja_cli"]
 
@@ -14,14 +16,22 @@
 
 _loader = ts.default_loaders(
     appname="makejinja", config_files=(Path(".makejinja.toml"),)
 )
 
 
 @click.command("makejinja")
-@ts.click_options(Config, _loader)
+@ts.click_options(cast(Type[AttrsInstance], Config), _loader)
 def makejinja_cli(config: Config):
+    """makejinja can be used to automatically generate files from [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/templates/).
+
+    Instead of passing CLI options, you can also write them to a file called `.makejinja.toml` in your working directory.
+    **Note**: In this file, options may be named differently.
+    Please refer to the file [`makejinja/config.py`](https://github.com/mirkolenz/makejinja/blob/main/makejinja/config.py) to see their actual names.
+    You will also find an example here: [`makejinja/tests/data/.makejinja.toml`](https://github.com/mirkolenz/makejinja/blob/main/tests/data/.makejinja.toml).
+    """
+
     makejinja(config)
 
 
 if __name__ == "__main__":
     makejinja_cli()
```

### Comparing `makejinja-1.1.2/makejinja/config.py` & `makejinja-1.1.4/makejinja/config.py`

 * *Files identical despite different names*

### Comparing `makejinja-1.1.2/makejinja/loader.py` & `makejinja-1.1.4/makejinja/loader.py`

 * *Files identical despite different names*

### Comparing `makejinja-1.1.2/pyproject.toml` & `makejinja-1.1.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "makejinja"
-version = "1.1.2"
+version = "1.1.4"
 description = "Automatically generate files based on Jinja templates. Use it to easily generate complex Home Assistant dashboards!"
 authors = ["Mirko Lenz <mirko@mirkolenz.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mirkolenz/makejinja"
 
 [tool.poetry.scripts]
 makejinja = "makejinja.cli:makejinja_cli"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 jinja2 = "^3.1.2"
 pyyaml = "^6.0"
 rich-click = "^1.6.1"
-typed-settings = { extras = ["click"], version = "^2.0.2" }
+typed-settings = "^23.0.0"
 tomli = { version = "^2.0.1", python = "<3.11" }
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.1"
+pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 
 [tool.pytest.ini_options]
 addopts = "--cov makejinja --cov-report term-missing -vv"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `makejinja-1.1.2/setup.py` & `makejinja-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,35 +7,35 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['jinja2>=3.1.2,<4.0.0',
  'pyyaml>=6.0,<7.0',
  'rich-click>=1.6.1,<2.0.0',
- 'typed-settings[click]>=2.0.2,<3.0.0']
+ 'typed-settings>=23.0.0,<24.0.0']
 
 extras_require = \
 {':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['makejinja = makejinja.cli:makejinja_cli']}
 
 setup_kwargs = {
     'name': 'makejinja',
-    'version': '1.1.2',
+    'version': '1.1.4',
     'description': 'Automatically generate files based on Jinja templates. Use it to easily generate complex Home Assistant dashboards!',
     'long_description': '# makejinja\n\nmakejinja can be used to automatically generate files from [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/templates/).\nThis allows you to load variables from external files or create repeating patterns via loops.\nIt is conceptually similar to [gomplate](https://github.com/hairyhenderson/gomplate), but is built on Python and Jinja instead of Go.\nA use case for this tool is generating config files for [Home Assistant](https://www.home-assistant.io/):\nUsing the same language that the built-in templates use, you can greatly simplify your configuration.\n\n## Home Assistant Example\n\n[A concrete example for Home Assistant can be found in the tests directory.](./tests/data)\n\n## Features\n\n- Recursively convert nested directories containing template files. One can even specify a pattern to specify relevant files in a folder.\n- Load data files containing variables to use in your Jinja templates from YAML, TOML, and Python files.\n- Use custom functions in your Jinja templates by loading custom filters and/or globals.\n- Easily load bundled as well as custom Jinja extensions.\n- Tailor the whitespace behavior to your needs.\n- Use custom delimiters for Jinja blocks/comments/variables.\n- Modify _all_ init options for the Jinja environment.\n- Write custom **Python loaders** that implement a subset of our fully typed [abstract loader class](./makejinja/loader.py)\n\n## Installation\n\nmakejinja is available via `pip` and can be installed via\n\n`pip install makejinja`\n\nBeware that depending on other packages installed on your system via pip, there may be incompatibilities.\nThus, we advise leveraging [`pipx`](https://github.com/pypa/pipx) instead:\n\n`pipx install makejinja`\n\nAlternatively, the application can also be used via Docker.\nWe automatically publish an image at `ghcr.io/mirkolenz/makejinja`.\nTo use it, mount a folder to the container and pass the options as the command.\nFor example, to process files in `./data/input` and render them to `./data/output`, you could run:\n\n`docker run --rm -v $(pwd)/data:/data ghcr.io/mirkolenz/makejinja@latest --input /data/input --output /data/output`\n\n## Usage\n\nIn its default configuration, makejinja searches the input folder recursively for files ending in `.jinja`.\nAlso, we copy all contents (except raw template files) of the input folder to the output folder and remove the `.jinja` ending during the render process.\nTo get an overview of the remaining options, we advise you to run `makejinja --help`:\n\n<!-- echo -e "\\n```txt\\n$(COLUMNS=120 poetry run makejinja --help)\\n```" >> README.md -->\n\n```txt\n\n Usage: makejinja [OPTIONS]\n\n makejinja can be used to automatically generate files from Jinja templates.\n Instead of passing CLI options, you can also write them to a file called .makejinja.toml in your working directory.\n Note: In this file, options may be named differently. Please refer to the file makejinja/config.py to see their actual\n names. You will also find an example here: makejinja/tests/data/.makejinja.toml.\n\n╭─ Input/Output ───────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ *  --input                DIRECTORY  Path to a folder containing template files. It is passed to Jinja\'s             │\n│                                      FileSystemLoader when creating the environment.                                 │\n│                                      [required]                                                                      │\n│ *  --output               DIRECTORY  Path to a folder where the rendered templates are stored. makejinja preserves   │\n│                                      the relative paths in the process, meaning that you can even use it on nested   │\n│                                      directories.                                                                    │\n│                                      [required]                                                                      │\n│    --input-pattern        TEXT       Glob pattern to search for files in input_folder. Accepts all pattern supported │\n│                                      by fnmatch. If a file is matched by this pattern and does not end with the      │\n│                                      specified jinja-suffix, it is copied over to the output_folder. Note: Do not    │\n│                                      add a special suffix used by your template files here, instead use the          │\n│                                      jinja-suffix option.                                                            │\n│                                      [default: **/*]                                                                 │\n│    --jinja-suffix         TEXT       File ending of Jinja template files. All files with this suffix in input_folder │\n│                                      matched by pattern are passed to the Jinja renderer. Note: Should be provided   │\n│                                      with the leading dot.                                                           │\n│                                      [default: .jinja]                                                               │\n│    --copy-tree                       If your input_folder containes additional files besides Jinja templates, you    │\n│                                      may want to copy them to output_folder as well. This operation maintains the    │\n│                                      metadata of all files and folders, meaning that tools like rsync will treat     │\n│                                      them exactly like the original ones. Note: Even if set to no-copy-tree, files   │\n│                                      that are matched by your provided pattern within input_folder are still copied  │\n│                                      over. In both cases, a file\'s metadata is untouched. The main difference is     │\n│                                      that with copy-tree, folders keep their metadata while matched files are copied │\n│                                      to newly-created subfolders that differ in their metadata.                      │\n│    --keep-jinja-suffix               Decide whether the specified jinja-suffix is removed from the file after        │\n│                                      rendering.                                                                      │\n│    --keep-empty                      Some Jinja template files may be empty after rendering (e.g., if they only      │\n│                                      contain macros that are imported by other templates). By default, we do not     │\n│                                      copy such empty files. If there is a need to have them available anyway, you    │\n│                                      can adjust that.                                                                │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Jinja Environment ──────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --data           PATH       Load variables from yaml/yml/toml files for use in your Jinja templates. The defintions  │\n│                             are passed to Jinja\'s render function. Can either be a file or a folder containg files.  │\n│                             Note: This option may be passed multiple times to pass a list of values. If multiple     │\n│                             files are supplied, beware that previous declarations will be overwritten by newer ones. │\n│ --loader         TEXT       Use custom Python code to adjust the used Jinja environment to your needs. The specified │\n│                             Python file should export a class containing a subset of the following functions:        │\n│                             filters, globals, data, and extensions. In addition, you may add an __init__ function    │\n│                             that recives two positional arguments: the created Jinja environment and the data parsed │\n│                             from the files supplied to makejinja\'s data option. This allows you to apply aribtrary   │\n│                             logic to makejinja. An import path can be specified either in dotted notation            │\n│                             (your.custom.Loader) or with a colon as object delimiter (your.custom:Loader). Note:     │\n│                             This option may be passed multiple times to pass a list of values.                       │\n│ --import-path    DIRECTORY  In order to load custom loaders or Jinja extensions, the PYTHONPATH variable needs to be │\n│                             patched. By default, makejinja will look for modules in your current directory, but you  │\n│                             may change that.                                                                         │\n│                             [default: .]                                                                             │\n│ --extension      TEXT       List of Jinja extensions to use as strings of import paths. An overview of the built-in  │\n│                             ones can be found on the project website. Note: This option may be passed multiple times │\n│                             to pass a list of values.                                                                │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Jinja Whitespace ───────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --lstrip-blocks/--no-lstrip-blocks          If this is set to True, leading spaces and tabs are stripped from the    │\n│                                             start of a line to a block.                                              │\n│                                             [default: lstrip-blocks]                                                 │\n│ --trim-blocks/--no-trim-blocks              If this is set to True, the first newline after a block is removed       │\n│                                             (block, not variable tag!).                                              │\n│                                             [default: trim-blocks]                                                   │\n│ --keep-trailing-newline                     Preserve the trailing newline when rendering templates. The default is   │\n│                                             False, which causes a single newline, if present, to be stripped from    │\n│                                             the end of the template.                                                 │\n│ --newline-sequence                    TEXT  The sequence that starts a newline. The default is tailored for          │\n│                                             UNIX-like systems (Linux/macOS).                                         │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Jinja Delimiters ───────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --delimiter-block-start       TEXT  The string marking the beginning of a block.                                     │\n│                                     [default: {%]                                                                    │\n│ --delimiter-block-end         TEXT  The string marking the end of a block.                                           │\n│                                     [default: %}]                                                                    │\n│ --delimiter-comment-start     TEXT  The string marking the beginning of a comment.                                   │\n│                                     [default: {#]                                                                    │\n│ --delimiter-comment-end       TEXT  The string marking the end of a comment.                                         │\n│                                     [default: #}]                                                                    │\n│ --delimiter-variable-start    TEXT  The string marking the beginning of a print statement.                           │\n│                                     [default: {{]                                                                    │\n│ --delimiter-variable-end      TEXT  The string marking the end of a print statement.                                 │\n│                                     [default: }}]                                                                    │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Jinja Prefixes ─────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --prefix-line-statement    TEXT  If given and a string, this will be used as prefix for line based statements.       │\n│ --prefix-line-comment      TEXT  If given and a string, this will be used as prefix for line based comments.         │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --help      Show this message and exit.                                                                              │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n```\n',
     'author': 'Mirko Lenz',
     'author_email': 'mirko@mirkolenz.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mirkolenz/makejinja',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `makejinja-1.1.2/PKG-INFO` & `makejinja-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: makejinja
-Version: 1.1.2
+Version: 1.1.4
 Summary: Automatically generate files based on Jinja templates. Use it to easily generate complex Home Assistant dashboards!
 Home-page: https://github.com/mirkolenz/makejinja
 License: MIT
 Author: Mirko Lenz
 Author-email: mirko@mirkolenz.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
-Requires-Dist: typed-settings[click] (>=2.0.2,<3.0.0)
+Requires-Dist: typed-settings (>=23.0.0,<24.0.0)
 Project-URL: Repository, https://github.com/mirkolenz/makejinja
 Description-Content-Type: text/markdown
 
 # makejinja
 
 makejinja can be used to automatically generate files from [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/templates/).
 This allows you to load variables from external files or create repeating patterns via loops.
```

