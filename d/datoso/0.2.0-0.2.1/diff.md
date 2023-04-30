# Comparing `tmp/datoso-0.2.0.tar.gz` & `tmp/datoso-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso-0.2.0.tar", last modified: Mon Apr 17 03:32:34 2023, max compression
+gzip compressed data, was "datoso-0.2.1.tar", last modified: Sun Apr 30 17:58:16 2023, max compression
```

## Comparing `datoso-0.2.0.tar` & `datoso-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:32:34.048972 datoso-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-17 03:32:06.000000 datoso-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-17 03:32:06.000000 datoso-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-17 03:32:34.048972 datoso-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-17 03:32:06.000000 datoso-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-17 03:32:06.000000 datoso-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 03:32:34.048972 datoso-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:32:34.044972 datoso-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:32:34.048972 datoso-0.2.0/src/datoso/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-17 03:32:06.000000 datoso-0.2.0/src/datoso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18062 2023-04-17 03:32:06.000000 datoso-0.2.0/src/datoso/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-17 03:32:06.000000 datoso-0.2.0/src/datoso/datoso.ini
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-17 03:32:06.000000 datoso-0.2.0/src/datoso/seeds.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:32:34.048972 datoso-0.2.0/src/datoso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-17 03:32:33.000000 datoso-0.2.0/src/datoso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-17 03:32:34.000000 datoso-0.2.0/src/datoso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 03:32:33.000000 datoso-0.2.0/src/datoso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-17 03:32:33.000000 datoso-0.2.0/src/datoso.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-17 03:32:33.000000 datoso-0.2.0/src/datoso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 03:32:33.000000 datoso-0.2.0/src/datoso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:58:16.131066 datoso-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-30 17:58:03.000000 datoso-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-30 17:58:03.000000 datoso-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-30 17:58:16.131066 datoso-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-30 17:58:03.000000 datoso-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-30 17:58:03.000000 datoso-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-30 17:58:16.131066 datoso-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:58:16.131066 datoso-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:58:16.131066 datoso-0.2.1/src/datoso/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-30 17:58:03.000000 datoso-0.2.1/src/datoso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-04-30 17:58:03.000000 datoso-0.2.1/src/datoso/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-30 17:58:03.000000 datoso-0.2.1/src/datoso/datoso.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-30 17:58:03.000000 datoso-0.2.1/src/datoso/seeds.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:58:16.131066 datoso-0.2.1/src/datoso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-30 17:58:16.000000 datoso-0.2.1/src/datoso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-30 17:58:16.000000 datoso-0.2.1/src/datoso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 17:58:16.000000 datoso-0.2.1/src/datoso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-30 17:58:16.000000 datoso-0.2.1/src/datoso.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-30 17:58:16.000000 datoso-0.2.1/src/datoso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-30 17:58:16.000000 datoso-0.2.1/src/datoso.egg-info/top_level.txt
```

### Comparing `datoso-0.2.0/LICENSE` & `datoso-0.2.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Lacides Miranda
+Copyright (c) 2023 Lacides Miranda
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `datoso-0.2.0/PKG-INFO` & `datoso-0.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,119 +1,123 @@
-Metadata-Version: 2.1
-Name: datoso
-Version: 0.2.0
-Summary: Python command line tool to download and organize your Rom Dat files.
-Author-email: Lacides Miranda <laromicas@hotmail.com>
-License: MIT License
-Project-URL: Source Code, https://github.com/laromicas/datoso
-Keywords: emulators,roms
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: System :: Emulators
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: selenium
-Provides-Extra: nointro
-Provides-Extra: redump
-Provides-Extra: dev
-License-File: LICENSE
-
-``` bash
-    .___       __
-  __| _/____ _/  |_  ____  __________
- / __ |\__  \\   __\/  _ \/  ___/  _ \
-/ /_/ | / __ \|  | (  <_> )___ (  <_> )
-\____ |(____  /__|  \____/____  >____/
-     \/     \/                \/
-```
+![Datoso](/bearlogo.png)
 
 # Datoso
 
 Datoso is a WIP Python command line tool to download and organize your Dat Roms.
 As today the tool supports dat-omatic, redump, and translated-english dats.
 It merges all the dats in a tree folder structure thought to use with Emulators rather than dats.
 The dat file format must be compatible with [ROMVault](https://www.romvault.com/).
 
 ## Installation
 
-Use pip or download a release and install it (recommended to use a
-virtual environment):
+Datoso requires python 3.10+.
+
+Use pip (recommended to use a virtual environment):
 
 ``` bash
+# Optional (create a virtual environment)
+python3 -m venv venv
+source venv/bin/activate
+
+# Install datoso base (doesn't do much without plugins)
 pip install datoso
+
+# Install datoso with all official plugins
+pip install datoso[all]
+
+# Install datoso with only one of the plugins
+pip install datoso[fbneo]
+pip install datoso[nointro]
+pip install datoso[pleasuredome]
+pip install datoso[redump]
+pip install datoso[translatedenglish]
+
+# Install datoso plugins after installing datoso
+pip install datoso_seed_fbneo
+pip install datoso_seed_nointro
+pip install datoso_seed_pleasuredome
+pip install datoso_seed_redump
+pip install datoso_seed_translatedenglish
+
 ```
 
 ## Usage
 
 ``` bash
 # Show help
 $ datoso --help
 
-# List installed seeds
-$ datoso list
+usage: datoso [-h] [-v] {config,doctor,dat,seed,import,deduper,all} ...
 
-# Doctor the seeds installation
-$ datoso doctor [seed]
+Update dats from different sources.
 
-# List available seeds
-$ datoso seed available
+positional arguments:
+  {config,doctor,dat,seed,import,deduper,base,fbneo,nointro,pleasuredome,private,redump,translatedenglish,all}
+                        sub-command help
+    config              Show configuration
+    doctor              Doctor installed seeds
+    dat                 Changes configuration in current dats
+    seed                Seed admin commands
+    import              Import dats from existing romvault
+    deduper             Deduplicate dats, removes duplicates from input dat existing in parent dat
+    all                 Update seed all
+
+options:
+  -h, --help            show this help message and exit
+  -v, --version         show version
 
-# Seed install
-$ datoso seed install [seed] [--repository REPOSITORY] [--branch BRANCH]
 
-# Seed remove
-$ datoso seed remove [seed]
 
 # Seed commands
-$ datoso [seed] {--fetch|--process} [--filter FILTER]
+$ datoso seed [list,details]
+
+# Seed commands
+$ datoso {<seed> | all} {--fetch | --process} [--filter FILTER]
+#e.g.
+$ datoso redump --fetch                    # Downloads all dats from redump
+$ datoso redump --process --filter IBM     # Process all dats downloaded in the step before that has IBM in its name
+
+# Doctor
+$ datoso doctor [seed]        # Validates if all requirements for all seeds are OK
+
+# Deduper
+$ datoso deduper -input <input_dat> -p <parent_dat> [-o <output_dat>]   # If output dat is not especified, input dat will be overwritten.
 
 optional arguments:
    -h, --help            show the help message and exit, feel free to append to other commands
    -v, --verbose         verbose output
    -q, --quiet           quiet output
 ```
 
-## How to Build
+## Developing a seed
 
-``` bash
-# Install build
-$ pip install build
-
-# Build
-$ python -m build
-```
+Check [datoso_seed_base](https://github.com/laromicas/datoso_seed_base)
 
 ## Posible Issues
 
 Be careful when updating dats from datomatic, sometimes they put a
 captcha, and you may be banned if the captcha fails, captcha support is
 OTW.
 
 ## TODO (without priority)
 
--   Database initialization !!! (priority)
--   Make update rules write to database only when finished
+-   Datoso Initialization
+-   Change logo
+-   Change pydantic to dataclasses
 -   Better rules update process
--   Logging
+    -   Make update rules write to database only when finished
 -   Tests
 -   More dat repositories
 -   Mega.nz download support (<https://pypi.org/project/mega.py/>)
 -   Zippyshare download support (<https://pypi.org/project/zippyshare-downloader/>)
 -   Zippyshare download support (<https://pypi.org/project/pyOneFichierClient/>)
 -   Configurable folder structure (instead of emulator-focused structure use dat-repositories or viceversa)
-    -   Maybe with a builder, to avoid the need to change the code
--   Modular design for repositories (done for seeds, repositores
-    missing)
--   Better structure for the downloaders \*
--   Better command line support
--   Migrate to python modules
--   Manually Deduplicate dats from command line (easy to implement)
+    -   Maybe with a builder, to avoid the need to change the code anytime
+-   Modular design for repositories (done for seeds, repositores missing)
+
 
 *(*) Done but to be improved*
 *(**) Did it Yay!!!*
 
 ## USEFUL DEVELOPMENT COMMANDS
 
 ```bash
@@ -126,23 +130,21 @@
 # Pylint
 $ pylint src --errors-only
 $ pylint src --disable=all --enable=missing-function-docstring
 ```
 
 ## WISHLIST (without priority)
 
--   Modular design for dat seeds (\*\*)
 -   Dat structure for ClrMamePro or another dat manager.
 -   Web interface
 -   Download from central repositories (an S3 or something like that to prevent overload main sites)
     -   Lambda to download dats and upload to S3
     -   Downloading from S3
 -   Auto-Import MIA Lists (for redump)
     -   Add \[MIA\] to dat roms
--   Deduplicate dats (\*\*)
 -   Remove MIA from dats
 -   .cue Generator
 
 *(**) Did it Yay!!!*
 
 ## Contributing
```

### Comparing `datoso-0.2.0/pyproject.toml` & `datoso-0.2.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires      = ["setuptools~=62.6", "wheel~=0.37.1"]
+requires      = ["setuptools~=67.6", "wheel~=0.40.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name        = "datoso"
 description = "Python command line tool to download and organize your Rom Dat files."
 readme      = "README.md"
@@ -22,36 +22,35 @@
     'Topic :: System :: Emulators',
 ]
 dependencies = [
     "tinydb>=4.7.0",
     "pydantic>=1.9.2",
     "python-dateutil>=2.8.0",
     "xmltodict>=0.13.0",
-    "internetarchive>=3.0.0",
     "tabulate>=0.9.0",
-    "orjson>=3.8.10",
 ]
 dynamic = ["version"]
 
 
 [project.optional-dependencies]
-selenium = [
-    "selenium==4.3.0",
+all = [
+    "datoso_seed_fbneo>=0.1.0",
+    "datoso_seed_nointro>=0.1.0",
+    "datoso_seed_pleasuredome>=0.1.0",
+    "datoso_seed_redump>=0.1.0",
+    "datoso_seed_translatedenglish>=0.1.0",
     ]
-
-nointro = [
-    "datoso_nointro>=0.1.0",
-    ]
-
-redump = [
-    "datoso_redump>=0.1.0",
-    ]
-
+fbneo = [ "datoso_seed_fbneo>=0.1.0" ]
+nointro = [ "datoso_seed_nointro>=0.1.0" ]
+pleasuredome = [ "datoso_seed_pleasuredome>=0.1.0" ]
+redump = [ "datoso_seed_redump>=0.1.0" ]
+translatedenglish = [ "datoso_seed_translatedenglish>=0.1.0" ]
 dev = [
     "ruff>=0.0.261",
+    "line_profiler==4.0.3"
     ]
 
 [project.urls]
 "Source Code"       = "https://github.com/laromicas/datoso"
 
 [project.scripts]
 datoso = "datoso.__main__:main"
```

### Comparing `datoso-0.2.0/src/datoso/__main__.py` & `datoso-0.2.1/src/datoso/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 """Main entry point for datoso"""
 import configparser
 import json
 import logging
 import os
 from pathlib import Path
-from pydoc import locate
 import re
 import sys
 import argparse
 from venv import logger
 from tabulate import tabulate
+from datoso.configuration.configuration import get_seed_name
 from datoso.configuration.logger import enable_logging, set_verbosity
 from datoso.database.models.datfile import Dat
 
-from datoso import __version__, ROOT_FOLDER
+from datoso import __version__, __app_name__, ROOT_FOLDER
 from datoso.helpers import Bcolors
 from datoso.configuration import config
 
-from datoso.commands.list import installed_seeds, seed_description
-from datoso.commands.doctor import check_dependencies, check_main_executables, check_seed
-from datoso.commands.seed_manager import seed_available, get_seed_repository, seed_install, seed_remove
+from datoso.helpers.plugins import installed_seeds, seed_description
+from datoso.commands.doctor import check_module, check_seed
 from datoso.commands.seed import Seed
 from datoso.repositories.dedupe import Dedupe
 from datoso.seeds.rules import Rules
 from datoso.seeds.unknown_seed import detect_seed
 
-
 #---------Boilerplate to check python version ----------
 if sys.version_info[0] < 3 or sys.version_info.minor < 9:
     print("This is a Python 3 script. Please run it with Python 3.9 or above")
     sys.exit(1)
 
 
 def parse_args() -> argparse.Namespace:
@@ -42,78 +40,72 @@
     parser = argparse.ArgumentParser(description='Update dats from different sources.')
     subparser = parser.add_subparsers(help='sub-command help')
 
     parser.add_argument('-v', '--version', action='store_true', help='show version')
 
     parser_save = subparser.add_parser('config', help='Show configuration')
     parser_save.add_argument('-s', '--save', action='store_true', help='Save configuration to .datosorc')
+    parser_save.add_argument('-d', '--directory', default='~', choices=['~', '.'], help='Directory to save .datosorc')
     parser_save.set_defaults(func=command_config)
     parser_save.add_argument('-ru', '--rules-update', action='store_true', help='Update system rules from GoogleSheets Url')
 
     group_save = parser_save.add_mutually_exclusive_group()
     group_save.add_argument('--set', nargs=2, metavar=('configuration', 'value'), help='Set Configuration Option separated by point with new value e.g. <GENERAL.Overwrite> <false>')
     group_save.add_argument('--get', metavar=('configuration'), help='Get value of Configuration Option.')
     parser_save.add_argument('-g','--global', action='store_true', help='When set, saves to global config, else to `.datosorc`')
 
-    parser_list = subparser.add_parser('list', help='List installed seeds')
-    parser_list.set_defaults(func=command_list)
-
     parser_doctor = subparser.add_parser('doctor', help='Doctor installed seeds')
-    parser_doctor.add_argument('command', nargs='?', help='Seed to doctor')
+    parser_doctor.add_argument('seed', nargs='?', help='Seed to doctor')
     parser_doctor.set_defaults(func=command_doctor)
     parser_doctor.add_argument('-r', '--repair', action='store_true', help='Try to repair seed(s)')
 
-    parser_dat = subparser.add_parser('dat', help='Make changes in dat config')
+    parser_dat = subparser.add_parser('dat', help='Changes configuration in current dats')
     parser_dat.add_argument('command', nargs='?', help='Command to execute')
-    group_dat= parser_dat.add_mutually_exclusive_group(required=True)
 
+    group_dat= parser_dat.add_mutually_exclusive_group(required=True)
     group_dat.add_argument('-d', '--dat-name', help='Select dat to update/check, must be in format "seed:name"')
     group_dat.add_argument('-f', '--find', help='Select dats based on filter, they are "<field><operator><value>;...", valid operators are: =, !=, and ~=')
+    group_dat.add_argument('-a', '--all', help='Show all dats', action='store_true')
+
     parser_dat.add_argument('-s', '--set', help='Manually set variable, must be in format "variable=value"')
     parser_dat.add_argument('-on', '--only-names', action='store_true', help='Only show names')
 
     parser_dat.set_defaults(func=command_dat)
 
     # Seed admin commands
-    parser_seed = subparser.add_parser('seed', help='Seed scripts')
+    parser_seed = subparser.add_parser('seed', help='Seed admin commands')
     subparser_seed = parser_seed.add_subparsers(help='sub-command help')
 
-    parser_available = subparser_seed.add_parser('available', help='List available seeds')
-    parser_available.set_defaults(func=command_seed_available)
+    parser_available = subparser_seed.add_parser('installed', help='List installed seeds')
+    parser_available.set_defaults(func=command_seed_installed)
 
-    parser_install = subparser_seed.add_parser('install', help='Install seed')
-    parser_install.add_argument('seed', help='Seed to install')
-    parser_install.set_defaults(func=command_seed_install)
-    parser_install.add_argument('-r', '--repository', help='Use repository instead of default')
-    parser_install.add_argument('-b', '--branch', help='Use branch name instead of master')
-    parser_install.add_argument('-d', '--developer', action='store_true', help='Install developer version (with git)')
-    parser_install.add_argument('-id', '--install-dependencies', action='store_true', help='Install all required dependencies')
-
-    parser_remove = subparser_seed.add_parser('remove', help='Remove seed')
-    parser_remove.add_argument('seed', help='Seed to remove')
-    parser_remove.set_defaults(func=command_seed_remove)
+    parser_details = subparser_seed.add_parser('details', help='Show details of seed')
+    parser_details.add_argument('seed', help='Seed to show details of')
+    parser_details.set_defaults(func=command_seed_details)
 
     parser_import = subparser.add_parser('import', help='Import dats from existing romvault')
     parser_import.set_defaults(func=command_import)
 
     parser_deduper = subparser.add_parser('deduper', help='Deduplicate dats, removes duplicates from input dat existing in parent dat')
     parser_deduper.add_argument('-i', '--input', required=True, help='Input dat file e.g. "redump:psx_child" or "/mnt/roms/redump_psx_child.dat"')
     parser_deduper.add_argument('-p', '--parent', default=None, help='Parent dat file e.g. "redump:psx" or "/mnt/roms/redump_psx.dat" if not set, parent is taken from input dat with prescanned dats')
     parser_deduper.add_argument('-o', '--output', default=None, help='If different from input.dat, must be a file path e.g. "/mnt/roms/redump_psx_child_deduped.dat"')
     parser_deduper.add_argument('-dr', '--dry-run', action='store_true', help='Do not write output file, just show actions')
 
     parser_deduper.set_defaults(func=command_deduper)
 
 
     # Seed commands
-    for seed in list(installed_seeds()) + [('all', 'All seeds')]:
-        parser_command = subparser.add_parser(seed[0], help=f'Update seed {seed[0]}')
-        parser_command.set_defaults(func=command_seed, seed=seed[0])
+    for seed, _ in list(installed_seeds().items()) + [('all', 'All seeds')]:
+        seed = get_seed_name(seed)
+        parser_command = subparser.add_parser(seed, help=f'Update seed {seed}')
+        parser_command.set_defaults(func=command_seed, seed=seed)
         parser_command.add_argument('-f', '--fetch', action='store_true', help='Fetch seed')
         parser_command.add_argument('-p', '--process', action='store_true', help='Process dats from seed')
+        parser_command.add_argument('-d', '--details', action='store_true', help='Show details of seed')
         parser_command.add_argument('-fd', '--filter', help='Filter dats to process')
 
     # Common arguments
     subparsers = [subparser, subparser_seed]
     for subpars in subparsers:
         for subpar in subpars.choices.values():
             subpar.add_argument('-v', '--verbose', action='store_true', help='verbose output')
@@ -157,70 +149,82 @@
     merged.dedupe()
     if args.output and not args.dry_run:
         merged.save(args.output)
     elif not args.dry_run:
         merged.save(args.input)
     print(f'{Bcolors.OKBLUE}File saved to {args.output if args.output else args.input}{Bcolors.ENDC}')
 
+
 def command_import(_) -> None:
     """ Make changes in dat config """
     dat_root_path = config['PATHS']['DatPath']
+
+    if not dat_root_path or not Path(dat_root_path).exists():
+        print(f'{Bcolors.FAIL}Dat root path not set or does not exist{Bcolors.ENDC}')
+        sys.exit(1)
+
     rules = Rules().rules
 
     dats = { str(x):None for x in Path(dat_root_path).rglob("*.[dD][aA][tT]") }
+
     if config['IMPORT'].get('IgnoreRegEx'):
         ignore_regex = re.compile(config['IMPORT']['IgnoreRegEx'])
         dats = [ dat for dat in dats if not ignore_regex.match(dat) ]
 
     fromhere = ''
     found = False
     for dat_name in dats:
         if dat_name == fromhere or fromhere == '':
             found = True
         if not found:
             continue
         print(f'{dat_name} - ', end='')
-        seed, class_detected = detect_seed(dat_name, rules)
-        print(f'{seed} - {class_detected}')
-        if class_detected:
-            class_name = locate(class_detected)
-            dat = class_name(file=dat_name)
+        seed, _class = detect_seed(dat_name, rules)
+        print(f'{seed} - {_class.__name__ if _class else None}')
+        if _class:
+            dat = _class(file=dat_name)
             dat.load()
             database = Dat(seed=seed, new_file=dat_name, **dat.dict())
             database.save()
             database.close()
 
 
 def command_dat(args):
     """ Make changes in dat config """
+
+    def print_dats(dats):
+        """ Print dats """
+        output = []
+        for dat in dats:
+            output.append({
+                'seed': dat['seed'],
+                'name': dat['name'],
+                'status': dat['status'] if 'status' in dat else 'enabled',
+            })
+        if getattr(args, 'only_names', False):
+            for dat in output:
+                print(f"{dat['seed']}:{dat['name']}")
+            return
+        print(tabulate(output, headers='keys', tablefmt='psql'))
+
     from datoso.database import DB
     from tinydb import Query
     query = Query()
     table = DB.table('dats')
-    output = []
     if args.dat_name:
         splitted = args.dat_name.split(':')
         if len(splitted) != 2:
             print(f'{Bcolors.WARNING}Invalid dat name, must be in format "seed:name"{Bcolors.ENDC}')
             print(f'Showing results for filter: {Bcolors.OKCYAN}name~={args.dat_name}{Bcolors.ENDC}')
             print('--------------------------------------------------------------')
             name = args.dat_name
             result = table.search(query.name.matches(r'^.*' + name + r'.*', flags=re.IGNORECASE))
-            if getattr(args, 'only_names', False):
-                for dat in result:
-                    print(f"{dat['seed']}:{dat['name']}")
-                sys.exit()
-            for dat in result:
-                output.append({
-                    'seed': dat['seed'],
-                    'name': dat['name'],
-                    'status': dat['status'] if 'status' in dat else 'enabled',
-                })
-            print(tabulate(output, headers='keys', tablefmt='psql'))
-            sys.exit(0)
+
+            print_dats(result)
+
         else:
             seed, name = splitted
             result = table.get((query.name == name) & (query.seed == seed))
             if not result:
                 print(f'{Bcolors.FAIL}Dat not found{Bcolors.ENDC}')
                 sys.exit(1)
             if args.set:
@@ -229,73 +233,70 @@
                     value = int(value)
                 if value.lower() == 'true':
                     value = True
                 table.update({key: value}, doc_ids=[result.doc_id])
                 table.storage.flush()
                 print(f'{Bcolors.OKGREEN}Dat {Bcolors.OKCYAN}{seed}:{name}{Bcolors.OKGREEN} {key} set to {Bcolors.OKBLUE}{value}{Bcolors.ENDC}')
                 sys.exit(0)
-            if result:
-                output.append({
-                    'seed': result['seed'],
-                    'name': result['name'],
-                    'status': result['status'] if 'status' in result else 'enabled',
-                })
-            print(tabulate(output, headers='keys', tablefmt='psql'))
-            sys.exit(0)
-
-
-def command_seed_remove(args) -> None:
-    """ Remove seed """
-    if not check_seed(args.seed):
-        print(f'Module Seed {Bcolors.FAIL}  - {Bcolors.BOLD}{args.seed}{Bcolors.ENDC} not found')
-        sys.exit(1)
-    seed_remove(args.seed)
-    print(f'Seed {Bcolors.OKGREEN}{args.seed}{Bcolors.ENDC} removed successfully')
+            print_dats([result])
+    elif args.all:
+        # Show all dats
+        print_dats(table.all())
+
+    elif args.find:
+        # Find dats TODO: finish
+        print(f'Showing results for filter: {Bcolors.OKCYAN}{args.find}{Bcolors.ENDC}')
+        print('--------------------------------------------------------------')
+        name, value = args.find.split('=')
+        from tinydb import where
+        result = table.search(where(name) == value)
+        print_dats(result)
 
 
-def command_seed_install(args) -> None:
-    """ Install seed """
-    if check_seed(args.seed):
-        print(f'Module Seed {Bcolors.WARNING}{args.seed}{Bcolors.ENDC} already installed')
-        print('Reinstall? [y/n]: ', end='')
-        if input().lower() != 'y':
-            sys.exit(1)
-    repository = get_seed_repository(args.seed) or (args.repository if getattr(args, 'repository', None) else None)
-    if not repository:
-        print(f'{Bcolors.FAIL}Repository for seed {args.seed} not found.{Bcolors.ENDC}')
-        print('Please provide it with --repository parameter.')
-        sys.exit(1)
-    seed_install(args, repository)
-    print(f'Seed {Bcolors.OKGREEN}{args.seed}{Bcolors.ENDC} installed successfully')
-
-
-def command_seed_available(_) -> None:
+def command_seed_installed(_) -> None:
     """ List available seeds """
-    status = {
-        'installed': Bcolors.OKGREEN,
-        'not installed': Bcolors.OKCYAN,
-    }
-    print('Available seeds:')
-    for seed in seed_available():
-        installed = 'installed' if check_seed(seed[0]) else 'not installed'
-        print(f'* {status[installed]}{seed[0]}{Bcolors.ENDC} - {seed[1][0:60] if len(seed[1]) > 60 else seed[1]}...')
+    print('Installed seeds:')
+    for seed, seed_module in installed_seeds().items():
+        description = seed_description(seed_module)
+        description = {description[0:60]+'...' if len(description) > 60 else description}
+        seed_name = seed[12:]
+        print(f'* {Bcolors.OKGREEN}{seed_name}{Bcolors.ENDC} - {description}')
+
+
+def command_seed_details(args) -> None:
+    module = None
+    for seed, seed_module in installed_seeds().items():
+        if seed == f'{__app_name__}_seed_{args.seed}':
+            module = seed_module
+            break
+    if not module:
+        print(f'Seed {Bcolors.FAIL}{args.seed}{Bcolors.ENDC} not installed')
+        sys.exit(1)
+    print(f'Seed {Bcolors.OKGREEN}{args.seed}{Bcolors.ENDC} details:')
+    print(f'  * Name: {module.__name__}')
+    print(f'  * Version: {module.__version__}')
+    print(f'  * Author: {module.__author__}')
+    print(f'  * Description: {module.__description__}')
 
 
 def command_seed(args) -> None:
     """ Commands with the seed (must be installed) """
     if args.seed == 'all':
-        for seed in installed_seeds():
+        for seed, _ in installed_seeds().items():
+            seed = get_seed_name(seed)
             if config['PROCESS'].get('SeedIgnoreRegEx'):
                 ignore_regex = re.compile(config['PROCESS']['SeedIgnoreRegEx'])
-                if ignore_regex.match(seed[0]):
+                if ignore_regex.match(seed):
                     continue
-            args.seed = seed[0]
+            args.seed = seed
             command_seed(args)
         sys.exit(0)
     seed = Seed(name=args.seed)
+    if getattr(args, 'details', False):
+        command_seed_details(args)
     if getattr(args, 'fetch', False):
         print(f'Fetching seed {Bcolors.OKGREEN}{args.seed}{Bcolors.ENDC}')
         if seed.fetch():
             print(f'Errors fetching {Bcolors.FAIL}{args.seed}{Bcolors.ENDC}')
             print('Please enable logs for more information or use -v parameter')
             command_doctor(args)
     if getattr(args, 'process', False):
@@ -304,19 +305,20 @@
         print('=======================')
         if seed.process_dats(fltr=getattr(args, 'filter', None)):
             print(f'Errors processing {Bcolors.FAIL}{args.seed}{Bcolors.ENDC}')
             print('Please enable logs for more information or use -v parameter')
             command_doctor(args)
 
 
-def command_config_save(_) -> None:
+def command_config_save(args) -> None:
     """ Save config to file """
-    with open('.datosorc', 'w', encoding='utf-8') as file:
+    config_file = os.path.expanduser('~/.datosorc') if args.directory == '~' else os.path.join(os.getcwd(), '.datosorc')
+    with open(config_file, 'w', encoding='utf-8') as file:
         config.write(file)
-    print(f'Config saved to {Bcolors.OKGREEN}.datosorc{Bcolors.ENDC}')
+    print(f'Config saved to {Bcolors.OKGREEN}{config_file}{Bcolors.ENDC}')
 
 
 def command_config_set(args) -> None:
     """ Set config value, if global is set, it will be set in datoso.ini file """
     myconfig = args.set[0].split('.')
     if len(myconfig) != 2:
         print(f'{Bcolors.FAIL}Invalid config key, must be in <SECTION>.<Option> format. {Bcolors.ENDC}')
@@ -327,14 +329,16 @@
 
     newconfig = configparser.ConfigParser(comment_prefixes='/', allow_no_value=True)
     newconfig.optionxform = lambda option: option
     if getattr(args, 'global', False):
         file = os.path.join(ROOT_FOLDER, 'datoso.ini')
     else:
         file = os.path.join(os.getcwd(), '.datosorc')
+        if not os.path.isfile(file):
+            file = os.path.expanduser('~/.datosorc')
     newconfig.read(file)
     if not newconfig.has_section(myconfig[0]):
         newconfig.add_section(myconfig[0])
     newconfig[myconfig[0]][myconfig[1]] = args.set[1]
     with open(file, 'w', encoding='utf-8') as file:
         newconfig.write(file)
     if getattr(args, 'global', False):
@@ -383,33 +387,36 @@
     else:
         config_dict = {s:dict(config.items(s)) for s in config.sections()}
         print(json.dumps(config_dict, indent=4))
 
 
 def command_list(_):
     """ List installed seeds """
-    seeds = installed_seeds()
-    for seed in seeds:
-        print(f'* {Bcolors.OKCYAN}{seed[0]}{Bcolors.ENDC} - {seed[1][0:60] if len(seed[1]) > 60 else seed[1]}...')
+    for seed, seed_class in installed_seeds().items():
+        description = seed_class.description()
+        print(f'* {Bcolors.OKCYAN}{seed}{Bcolors.ENDC} - {description[0:60] if len(description) > 60 else description}...')
 
 def command_doctor(args):
     """ Doctor installed seeds """
-    check_main_executables()
     if getattr(args, 'seed', False):
         seed = check_seed(args.seed)
         if not seed:
             print(f'Module Seed {Bcolors.FAIL}  - {Bcolors.BOLD}{args.seed}{Bcolors.ENDC} not found')
             sys.exit(1)
-        seeds = [(args.seed, seed_description(args.seed))]
+        seed = seed if args.seed.startswith('datoso_seed_') else f'datoso_seed_{args.seed}'
+        seeds = {seed: None}
     else:
         seeds = installed_seeds()
-    for seed in seeds:
-        check_dependencies(seed[0], args.repair)
+    for seed, module in seeds.items():
+        print(f'Checking seed {Bcolors.OKCYAN}{seed}{Bcolors.ENDC}')
+        check_module(seed, module, args.repair)
 
 def main():
     """ Main function """
+    from datoso.database.seeds.dat_rules import detect_first_run
+    detect_first_run()
     args = parse_args()
     args.func(args)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `datoso-0.2.0/src/datoso/datoso.ini` & `datoso-0.2.1/src/datoso/datoso.ini`

 * *Files 18% similar despite different names*

```diff
@@ -32,26 +32,22 @@
 Source Code = Other/Source Code
 Video = Other/Video
 Mobile = Mobile
 Manuals = Other/Manuals
 BIOS Images = Other/BIOS Images
 
 [PATHS]
-# THe path for ROMVault (or destination path for the files)
-RomVaultPath = .
+# the relative path to the database and configuration file
+DatosoPath = ~/.datoso
 # The path for the dats inside RomVaultPath
-DatPath = DatRoot
-# where database and temporal files will be stored
-WorkingPath = .
-# the relative path to the database file
-DatabasePath = ~/.datoso
+DatPath = ~/ROMVault/DatRoot
 # the name of the database file
-DatabaseFile = database.json
+DatabaseFile = datoso.json
 # the relative path to the temporary file
-TempPath = tmp
+DownloadPath = ~/.datoso/dats
 
 
 [IMPORT]
 # This ignores the files matching the regex when importing
 IgnoreRegEx =
 
 [PROCESS]
```

### Comparing `datoso-0.2.0/src/datoso.egg-info/PKG-INFO` & `datoso-0.2.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,119 +1,148 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Emulators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Provides-Extra: selenium
+Provides-Extra: all
+Provides-Extra: fbneo
 Provides-Extra: nointro
+Provides-Extra: pleasuredome
 Provides-Extra: redump
+Provides-Extra: translatedenglish
 Provides-Extra: dev
 License-File: LICENSE
 
-``` bash
-    .___       __
-  __| _/____ _/  |_  ____  __________
- / __ |\__  \\   __\/  _ \/  ___/  _ \
-/ /_/ | / __ \|  | (  <_> )___ (  <_> )
-\____ |(____  /__|  \____/____  >____/
-     \/     \/                \/
-```
+![Datoso](/bearlogo.png)
 
 # Datoso
 
 Datoso is a WIP Python command line tool to download and organize your Dat Roms.
 As today the tool supports dat-omatic, redump, and translated-english dats.
 It merges all the dats in a tree folder structure thought to use with Emulators rather than dats.
 The dat file format must be compatible with [ROMVault](https://www.romvault.com/).
 
 ## Installation
 
-Use pip or download a release and install it (recommended to use a
-virtual environment):
+Datoso requires python 3.10+.
+
+Use pip (recommended to use a virtual environment):
 
 ``` bash
+# Optional (create a virtual environment)
+python3 -m venv venv
+source venv/bin/activate
+
+# Install datoso base (doesn't do much without plugins)
 pip install datoso
+
+# Install datoso with all official plugins
+pip install datoso[all]
+
+# Install datoso with only one of the plugins
+pip install datoso[fbneo]
+pip install datoso[nointro]
+pip install datoso[pleasuredome]
+pip install datoso[redump]
+pip install datoso[translatedenglish]
+
+# Install datoso plugins after installing datoso
+pip install datoso_seed_fbneo
+pip install datoso_seed_nointro
+pip install datoso_seed_pleasuredome
+pip install datoso_seed_redump
+pip install datoso_seed_translatedenglish
+
 ```
 
 ## Usage
 
 ``` bash
 # Show help
 $ datoso --help
 
-# List installed seeds
-$ datoso list
+usage: datoso [-h] [-v] {config,doctor,dat,seed,import,deduper,all} ...
 
-# Doctor the seeds installation
-$ datoso doctor [seed]
+Update dats from different sources.
 
-# List available seeds
-$ datoso seed available
+positional arguments:
+  {config,doctor,dat,seed,import,deduper,base,fbneo,nointro,pleasuredome,private,redump,translatedenglish,all}
+                        sub-command help
+    config              Show configuration
+    doctor              Doctor installed seeds
+    dat                 Changes configuration in current dats
+    seed                Seed admin commands
+    import              Import dats from existing romvault
+    deduper             Deduplicate dats, removes duplicates from input dat existing in parent dat
+    all                 Update seed all
+
+options:
+  -h, --help            show this help message and exit
+  -v, --version         show version
 
-# Seed install
-$ datoso seed install [seed] [--repository REPOSITORY] [--branch BRANCH]
 
-# Seed remove
-$ datoso seed remove [seed]
 
 # Seed commands
-$ datoso [seed] {--fetch|--process} [--filter FILTER]
+$ datoso seed [list,details]
+
+# Seed commands
+$ datoso {<seed> | all} {--fetch | --process} [--filter FILTER]
+#e.g.
+$ datoso redump --fetch                    # Downloads all dats from redump
+$ datoso redump --process --filter IBM     # Process all dats downloaded in the step before that has IBM in its name
+
+# Doctor
+$ datoso doctor [seed]        # Validates if all requirements for all seeds are OK
+
+# Deduper
+$ datoso deduper -input <input_dat> -p <parent_dat> [-o <output_dat>]   # If output dat is not especified, input dat will be overwritten.
 
 optional arguments:
    -h, --help            show the help message and exit, feel free to append to other commands
    -v, --verbose         verbose output
    -q, --quiet           quiet output
 ```
 
-## How to Build
+## Developing a seed
 
-``` bash
-# Install build
-$ pip install build
-
-# Build
-$ python -m build
-```
+Check [datoso_seed_base](https://github.com/laromicas/datoso_seed_base)
 
 ## Posible Issues
 
 Be careful when updating dats from datomatic, sometimes they put a
 captcha, and you may be banned if the captcha fails, captcha support is
 OTW.
 
 ## TODO (without priority)
 
--   Database initialization !!! (priority)
--   Make update rules write to database only when finished
+-   Datoso Initialization
+-   Change logo
+-   Change pydantic to dataclasses
 -   Better rules update process
--   Logging
+    -   Make update rules write to database only when finished
 -   Tests
 -   More dat repositories
 -   Mega.nz download support (<https://pypi.org/project/mega.py/>)
 -   Zippyshare download support (<https://pypi.org/project/zippyshare-downloader/>)
 -   Zippyshare download support (<https://pypi.org/project/pyOneFichierClient/>)
 -   Configurable folder structure (instead of emulator-focused structure use dat-repositories or viceversa)
-    -   Maybe with a builder, to avoid the need to change the code
--   Modular design for repositories (done for seeds, repositores
-    missing)
--   Better structure for the downloaders \*
--   Better command line support
--   Migrate to python modules
--   Manually Deduplicate dats from command line (easy to implement)
+    -   Maybe with a builder, to avoid the need to change the code anytime
+-   Modular design for repositories (done for seeds, repositores missing)
+
 
 *(*) Done but to be improved*
 *(**) Did it Yay!!!*
 
 ## USEFUL DEVELOPMENT COMMANDS
 
 ```bash
@@ -126,23 +155,21 @@
 # Pylint
 $ pylint src --errors-only
 $ pylint src --disable=all --enable=missing-function-docstring
 ```
 
 ## WISHLIST (without priority)
 
--   Modular design for dat seeds (\*\*)
 -   Dat structure for ClrMamePro or another dat manager.
 -   Web interface
 -   Download from central repositories (an S3 or something like that to prevent overload main sites)
     -   Lambda to download dats and upload to S3
     -   Downloading from S3
 -   Auto-Import MIA Lists (for redump)
     -   Add \[MIA\] to dat roms
--   Deduplicate dats (\*\*)
 -   Remove MIA from dats
 -   .cue Generator
 
 *(**) Did it Yay!!!*
 
 ## Contributing
```

