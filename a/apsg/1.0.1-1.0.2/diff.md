# Comparing `tmp/apsg-1.0.1.tar.gz` & `tmp/apsg-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apsg-1.0.1.tar", last modified: Tue Nov 22 08:32:18 2022, max compression
+gzip compressed data, was "apsg-1.0.2.tar", last modified: Sun Apr 30 10:38:29 2023, max compression
```

## Comparing `apsg-1.0.1.tar` & `apsg-1.0.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 08:32:18.601110 apsg-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)      130 2022-11-22 08:32:02.000000 apsg-1.0.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (122)     2976 2022-11-22 08:32:02.000000 apsg-1.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     8847 2022-11-22 08:32:02.000000 apsg-1.0.1/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2022-11-22 08:32:02.000000 apsg-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      240 2022-11-22 08:32:02.000000 apsg-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    14296 2022-11-22 08:32:18.601110 apsg-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4543 2022-11-22 08:32:02.000000 apsg-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 08:32:18.589109 apsg-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     6754 2022-11-22 08:32:02.000000 apsg-1.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     2990 2022-11-22 08:32:02.000000 apsg-1.0.1/docs/apsg.database.rst
--rw-r--r--   0 runner    (1001) docker     (122)      248 2022-11-22 08:32:02.000000 apsg-1.0.1/docs/apsg.feature.rst
--rw-r--r--   0 runner    (1001) docker     (122)      113 2022-11-22 08:32:02.000000 apsg-1.0.1/docs/apsg.helpers.rst
--rw-r--r--   0 runner    (1001) docker     (122)      199 2022-11-22 08:32:02.000000 apsg-1.0.1/docs/apsg.math.rst
--rw-r--r--   0 runner    (1001) docker     (122)      256 2022-11-22 08:32:02.000000 apsg-1.0.1/docs/apsg.plotting.rst
--rw-r--r--   0 runner    (1001) docker     (122)      167 2022-11-22 08:32:02.000000 apsg-1.0.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      192 2022-11-22 08:32:02.000000 apsg-1.0.1/docs/automodules.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8666 2022-11-22 08:32:02.000000 apsg-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     2954 2022-11-22 08:32:02.000000 apsg-1.0.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3982 2022-11-22 08:32:02.000000 apsg-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2022-11-22 08:32:02.000000 apsg-1.0.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6455 2022-11-22 08:32:02.000000 apsg-1.0.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)      222 2022-11-22 08:32:02.000000 apsg-1.0.1/docs/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (122)      110 2022-11-22 08:32:02.000000 apsg-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      255 2022-11-22 08:32:18.601110 apsg-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1622 2022-11-22 08:32:02.000000 apsg-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 08:32:18.581109 apsg-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 08:32:18.589109 apsg-1.0.1/src/apsg/
--rw-r--r--   0 runner    (1001) docker     (122)     1963 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4609 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 08:32:18.593109 apsg-1.0.1/src/apsg/database/
--rw-r--r--   0 runner    (1001) docker     (122)      143 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14871 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/database/_alchemy.py
--rw-r--r--   0 runner    (1001) docker     (122)    10868 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/database/_sdbread.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 08:32:18.593109 apsg-1.0.1/src/apsg/decorator/
--rw-r--r--   0 runner    (1001) docker     (122)      160 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1160 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/decorator/_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 08:32:18.593109 apsg-1.0.1/src/apsg/feature/
--rw-r--r--   0 runner    (1001) docker     (122)     1640 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    56674 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/feature/_container.py
--rw-r--r--   0 runner    (1001) docker     (122)    21489 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/feature/_geodata.py
--rw-r--r--   0 runner    (1001) docker     (122)    14921 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/feature/_paleomag.py
--rw-r--r--   0 runner    (1001) docker     (122)    13916 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/feature/_statistics.py
--rw-r--r--   0 runner    (1001) docker     (122)    12450 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/feature/_tensor2.py
--rw-r--r--   0 runner    (1001) docker     (122)    25051 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/feature/_tensor3.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 08:32:18.597109 apsg-1.0.1/src/apsg/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)      532 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/helpers/_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)      862 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/helpers/_math.py
--rw-r--r--   0 runner    (1001) docker     (122)     2486 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/helpers/_notation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 08:32:18.597109 apsg-1.0.1/src/apsg/math/
--rw-r--r--   0 runner    (1001) docker     (122)      211 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10382 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/math/_matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    16409 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/math/_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 08:32:18.601110 apsg-1.0.1/src/apsg/plotting/
--rw-r--r--   0 runner    (1001) docker     (122)      627 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16514 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/plotting/_fabricplot.py
--rw-r--r--   0 runner    (1001) docker     (122)     2325 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/plotting/_paleomagplots.py
--rw-r--r--   0 runner    (1001) docker     (122)    20299 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/plotting/_plot_artists.py
--rw-r--r--   0 runner    (1001) docker     (122)    11473 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/plotting/_projection.py
--rw-r--r--   0 runner    (1001) docker     (122)    10937 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/plotting/_roseplot.py
--rw-r--r--   0 runner    (1001) docker     (122)    12037 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/plotting/_stereogrid.py
--rw-r--r--   0 runner    (1001) docker     (122)    27954 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/plotting/_stereonet.py
--rw-r--r--   0 runner    (1001) docker     (122)      718 2022-11-22 08:32:02.000000 apsg-1.0.1/src/apsg/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 08:32:18.593109 apsg-1.0.1/src/apsg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14296 2022-11-22 08:32:18.000000 apsg-1.0.1/src/apsg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1511 2022-11-22 08:32:18.000000 apsg-1.0.1/src/apsg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-22 08:32:18.000000 apsg-1.0.1/src/apsg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2022-11-22 08:32:18.000000 apsg-1.0.1/src/apsg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-22 08:32:18.000000 apsg-1.0.1/src/apsg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2022-11-22 08:32:18.000000 apsg-1.0.1/src/apsg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 08:32:18.601110 apsg-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 08:32:02.000000 apsg-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2022-11-22 08:32:02.000000 apsg-1.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    16080 2022-11-22 08:32:02.000000 apsg-1.0.1/tests/test_apsg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2504 2022-11-22 08:32:02.000000 apsg-1.0.1/tests/test_tensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.220525 apsg-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-30 10:38:13.000000 apsg-1.0.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-30 10:38:13.000000 apsg-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-30 10:38:13.000000 apsg-1.0.2/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-30 10:38:13.000000 apsg-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-30 10:38:13.000000 apsg-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-04-30 10:38:29.220525 apsg-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-30 10:38:13.000000 apsg-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.216525 apsg-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/apsg.database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/apsg.feature.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/apsg.helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/apsg.math.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/apsg.plotting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/automodules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-30 10:38:13.000000 apsg-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-30 10:38:29.220525 apsg-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-30 10:38:13.000000 apsg-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.212525 apsg-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.216525 apsg-1.0.2/src/apsg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.216525 apsg-1.0.2/src/apsg/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/database/_alchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/database/_sdbread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.216525 apsg-1.0.2/src/apsg/decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/decorator/_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.220525 apsg-1.0.2/src/apsg/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56754 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/feature/_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21489 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/feature/_geodata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/feature/_paleomag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13916 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/feature/_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/feature/_tensor2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25724 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/feature/_tensor3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.220525 apsg-1.0.2/src/apsg/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/helpers/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/helpers/_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/helpers/_notation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.220525 apsg-1.0.2/src/apsg/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/math/_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16409 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/math/_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.220525 apsg-1.0.2/src/apsg/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/plotting/_fabricplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/plotting/_paleomagplots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20299 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/plotting/_plot_artists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/plotting/_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/plotting/_roseplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/plotting/_stereogrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28705 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/plotting/_stereonet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.216525 apsg-1.0.2/src/apsg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-04-30 10:38:29.000000 apsg-1.0.2/src/apsg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-30 10:38:29.000000 apsg-1.0.2/src/apsg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 10:38:29.000000 apsg-1.0.2/src/apsg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-30 10:38:29.000000 apsg-1.0.2/src/apsg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-30 10:38:29.000000 apsg-1.0.2/src/apsg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 10:38:29.000000 apsg-1.0.2/src/apsg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.220525 apsg-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:13.000000 apsg-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-30 10:38:13.000000 apsg-1.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-04-30 10:38:13.000000 apsg-1.0.2/tests/test_apsg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-30 10:38:13.000000 apsg-1.0.2/tests/test_tensors.py
```

### Comparing `apsg-1.0.1/CONTRIBUTING.md` & `apsg-1.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/HISTORY.md` & `apsg-1.0.2/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changes
 
+### 1.0.2 (Apr 30 2023)
+ * lambda properties of tensors renamed to S
+ * cursor coordinates in stereonet show lin and fol
+
 ### 1.0.1 (Nov 22 2022)
  * density_lookup method implemented for StereoNet.grid
  * Stress tensor sigma* properties using inverted order of eigenvalues
  * render2fig method of StereoNet implemented
  * vector-like objects are not iterable, so properly render in pandas 
 
 ## 1.0.0 (Oct 7 2022)
```

### Comparing `apsg-1.0.1/LICENSE` & `apsg-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/PKG-INFO` & `apsg-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apsg
-Version: 1.0.1
+Version: 1.0.2
 Summary: APSG - The package for structural geologists
 Home-page: https://github.com/ondrolexa/apsg
 Author: Ondrej Lexa
 Author-email: lexa.ondrej@gmail.com
 License: MIT
 Project-URL: Documentation, https://apsg.readthedocs.io/
 Project-URL: Source Code, https://github.com/ondrolexa/apsg/
@@ -127,14 +127,18 @@
 ## License
 
 APSG is free software: you can redistribute it and/or modify it under the terms of the MIT License. A copy of this license is provided in ``LICENSE`` file.
 
 
 # Changes
 
+### 1.0.2 (Apr 30 2023)
+ * lambda properties of tensors renamed to S
+ * cursor coordinates in stereonet show lin and fol
+
 ### 1.0.1 (Nov 22 2022)
  * density_lookup method implemented for StereoNet.grid
  * Stress tensor sigma* properties using inverted order of eigenvalues
  * render2fig method of StereoNet implemented
  * vector-like objects are not iterable, so properly render in pandas 
 
 ## 1.0.0 (Oct 7 2022)
```

### Comparing `apsg-1.0.1/README.md` & `apsg-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/docs/Makefile` & `apsg-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/docs/apsg.database.rst` & `apsg-1.0.2/docs/apsg.database.rst`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/docs/conf.py` & `apsg-1.0.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 version = "1.0"
 # The full version, including alpha/beta/rc tags.
-release = "1.0.1"
+release = "1.0.2"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to
 # some non-false value, then it is used:
```

### Comparing `apsg-1.0.1/docs/contributing.rst` & `apsg-1.0.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/docs/index.rst` & `apsg-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/docs/installation.rst` & `apsg-1.0.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/docs/make.bat` & `apsg-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/setup.py` & `apsg-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open(path.join(CURRENT_PATH, "HISTORY.md")) as file:
     history = file.read()
 
 setup(
     name="apsg",
-    version="1.0.1",
+    version="1.0.2",
     description="APSG - The package for structural geologists",
     long_description=readme + "\n\n" + history,
     long_description_content_type="text/markdown",
     author="Ondrej Lexa",
     author_email="lexa.ondrej@gmail.com",
     url="https://github.com/ondrolexa/apsg",
     license="MIT",
```

### Comparing `apsg-1.0.1/src/apsg/__init__.py` & `apsg-1.0.2/src/apsg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,10 +94,10 @@
     "VollmerPlot",
     "RamsayPlot",
     "FlinnPlot",
     "HsuPlot",
     "quicknet",
 )
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __author__ = "Ondrej Lexa"
 __email__ = "lexa.ondrej@gmail.com"
```

### Comparing `apsg-1.0.1/src/apsg/config.py` & `apsg-1.0.2/src/apsg/config.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/src/apsg/database/_alchemy.py` & `apsg-1.0.2/src/apsg/database/_alchemy.py`

 * *Files 18% similar despite different names*

```diff
@@ -140,25 +140,25 @@
 
     sites = relationship("Site", back_populates="unit")
 
     def __repr__(self):
         return "Unit:{}".format(self.name)
 
 
-def initial_meta():
-    return [
-        Meta(name="version", value="3.0.4"),
-        Meta(name="crs", value="EPSG:4326"),
-        Meta(name="created", value=datetime.now().strftime("%d.%m.%Y %H:%M")),
-        Meta(name="updated", value=datetime.now().strftime("%d.%m.%Y %H:%M")),
-        Meta(name="accessed", value=datetime.now().strftime("%d.%m.%Y %H:%M")),
-    ]
+def default_meta():
+    return dict(
+        version="3.1.0",
+        crs="EPSG:4326",
+        created=datetime.now().strftime("%d.%m.%Y %H:%M"),
+        updated=datetime.now().strftime("%d.%m.%Y %H:%M"),
+        accessed=datetime.now().strftime("%d.%m.%Y %H:%M"),
+    )
 
 
-def initial_values():
+def default_initial_values():
     return [
         Structype(
             pos=1,
             structure="S",
             description="Default planar feature",
             structcode=35,
             groupcode=13,
@@ -180,15 +180,16 @@
     u = session.query(Meta).filter_by(name="updated").first()
     u.value = datetime.now().strftime("%d.%m.%Y %H:%M")
 
 
 def before_insert_pos_update(mapper, connection, target):
     if target.pos is None:
         t = str(mapper.persist_selectable)
-        maxpos = connection.execute("SELECT max({}.pos) FROM {}".format(t, t)).scalar()
+        query = "SELECT max({}.pos) FROM {}".format(t, t)
+        maxpos = connection.scalar(text(query))
         if maxpos is None:
             maxpos = 1
         else:
             maxpos += 1
         target.pos = maxpos
 
 
@@ -198,14 +199,15 @@
 
     Args:
         sdbfile (str): filename of PySDB database
 
     Keyword Args:
         create (bool): if True existing sdbfile will be deleted
             and new database will be created
+        autocommit(bool): if True, each operation is autocommitted
 
     Example:
         >>> db = SDBSession('database.sdb', create=True)
 
     """
 
     def __init__(self, sdb_file, **kwargs):
@@ -214,154 +216,271 @@
                 os.remove(sdb_file)
         self.sdb_engine = create_engine("sqlite:///{}".format(sdb_file))
         if kwargs.get("create", False):
             metadata.create_all(self.sdb_engine)
         sdb_Session = sessionmaker(bind=self.sdb_engine)
         self.session = sdb_Session()
         if kwargs.get("create", False):
-            self.session.add_all(initial_values())
-            self.session.add_all(initial_meta())
+            meta = default_meta()
+            meta.update(kwargs.get("meta", {}))
+            self.session.add_all(default_initial_values())
+            self.session.add_all([Meta(name=n, value=v) for n, v in meta.items()])
             self.session.commit()
+        self.autocommit = kwargs.get("autocommit", False)
         # add listeners
         event.listen(self.session, "before_commit", before_commit_meta_update)
         event.listen(Unit, "before_insert", before_insert_pos_update)
         event.listen(Structype, "before_insert", before_insert_pos_update)
         event.listen(Tag, "before_insert", before_insert_pos_update)
 
+    def __repr__(self):
+        return self.info()
+
+    def info(self, data=False):
+        lines = []
+        lines.append(f"PySDB database version: {self.meta('version').value}")
+        lines.append(f"PySDB database CRS: {self.meta('crs').value}")
+        lines.append(f"PySDB database created: {self.meta('created').value}")
+        lines.append(f"PySDB database updated: {self.meta('created').value}")
+        lines.append(f"Number of sites: {self.session.query(Site).count()}")
+        lines.append(f"Number of units: {self.session.query(Unit).count()}")
+        lines.append(f"Number of structures: {self.session.query(Structype).count()}")
+        lines.append(
+            f"Number of measurements: {self.session.query(Structdata).count()}"
+        )
+        if data:
+            for s in self.structypes():
+                n = self.session.query(Structdata).filter_by(structype=s).count()
+                if n > 0:
+                    lines.append(f"Number of {s.structure} measurements: {n}")
+        return "\n".join(lines)
+
     def close(self):
+        """
+        Close session
+
+        """
         self.session.close()
 
     def commit(self):
+        """
+        commit session
+
+        """
         self.session.commit()
 
-    def site(self, **kwargs):
+    def rollback(self):
         """
-        Insert or retrieve Site
+        rollback session
+
         """
-        assert "name" in kwargs, "name must be provided for site"
-        site = self.session.query(Site).filter_by(name=kwargs["name"]).first()
-        if site is None:
-            assert "unit" in kwargs, "unit must be provided to create site"
-            site = Site(**kwargs)
-            self.session.add(site)
-            self.commit()
+        self.session.rollback()
+
+    def meta(self, name, **kwargs):
+        """
+        Insert, update or retrieve (when kwargs empty) Meta
+
+        Args:
+            name (str): meta name
+
+        Keyword Args:
+            value (str): meta value
+
+        Returns:
+            Meta
+        """
+        meta = self.session.query(Meta).filter_by(name=name).first()
+        if kwargs:
+            if meta is None:
+                meta = Meta(name=name, **kwargs)
+                self.session.add(meta)
+            else:
+                self.session.query(Meta).filter_by(name=name).update(kwargs)
+            if self.autocommit:
+                self.commit()
+        return meta
+
+    def site(self, name, **kwargs):
+        """
+        Insert, update or retrieve (when kwargs empty) Site
+
+        Args:
+            name (str): site name
+
+        Keyword Args:
+            x_coord (float): x coord or longitude
+            y_coord (float): y coord or latitude
+            description (str): site description
+            unit (Unit): unit instance (mus be provided)
+
+        Returns:
+            Site
+        """
+        site = self.session.query(Site).filter_by(name=name).first()
+        if kwargs:
+            if site is None:
+                site = Site(name=name, **kwargs)
+                self.session.add(site)
+            else:
+                self.session.query(Site).filter_by(name=name).update(kwargs)
+            if self.autocommit:
+                self.commit()
         return site
 
-    def unit(self, **kwargs):
+    def unit(self, name, **kwargs):
         """
-        Insert or retrieve Unit
+        Insert, update or retrieve (when kwargs empty) Unit
+
+        Args:
+            name (str): unit name
+
+        Keyword Args:
+            description (str): unit description
+
+        Returns:
+            Unit
         """
-        assert "name" in kwargs, "name must be provided for unit"
-        unit = self.session.query(Unit).filter_by(name=kwargs["name"]).first()
-        if unit is None:
-            unit = Unit(**kwargs)
-            self.session.add(unit)
-            self.commit()
+        unit = self.session.query(Unit).filter_by(name=name).first()
+        if kwargs:
+            if unit is None:
+                unit = Unit(name=name, **kwargs)
+                self.session.add(unit)
+            else:
+                self.session.query(Unit).filter_by(name=name).update(kwargs)
+            if self.autocommit:
+                self.commit()
         return unit
 
-    def tag(self, **kwargs):
+    def tag(self, name, **kwargs):
         """
-        Insert or retrieve Tag
+        Insert, update or retrieve (when kwargs empty) Tag
+
+        Args:
+            name (str): tag name
+
+        Keyword Args:
+            description (str): tag description
+
+        Returns:
+            Tag
         """
-        assert "name" in kwargs, "name must be provided for tag"
-        tag = self.session.query(Tag).filter_by(name=kwargs["name"]).first()
-        if tag is None:
-            tag = Tag(**kwargs)
-            self.session.add(tag)
-            self.commit()
+        tag = self.session.query(Tag).filter_by(name=name).first()
+        if kwargs:
+            if tag is None:
+                tag = Tag(name=name, **kwargs)
+                self.session.add(tag)
+            else:
+                self.session.query(Tag).filter_by(name=name).update(kwargs)
+            if self.autocommit:
+                self.commit()
         return tag
 
-    def structype(self, **kwargs):
+    def structype(self, structure, **kwargs):
         """
-        Insert or retrieve Structype
+        Insert, update or retrieve (when kwargs empty) Structype
+
+        Args:
+            structure (str): label for structure
+
+        Keyword Args:
+            description (str): structype description
+            planar (int): 1 for planar 0 for linear
+            structcode (int): structcode (optional)
+            groupcode (int): groupcode (optional)
+
+        Returns:
+            Structype
         """
-        assert "structure" in kwargs, "structure must be provided for structype"
-        structype = (
-            self.session.query(Structype)
-            .filter_by(structure=kwargs["structure"])
-            .first()
-        )
-        if structype is None:
-            structype = Structype(**kwargs)
-            self.session.add(structype)
-            self.commit()
+        structype = self.session.query(Structype).filter_by(structure=structure).first()
+        if kwargs:
+            if structype is None:
+                structype = Structype(structure=structure, **kwargs)
+                self.session.add(structype)
+            else:
+                self.session.query(Structype).filter_by(structure=structure).update(
+                    kwargs
+                )
+            if self.autocommit:
+                self.commit()
         return structype
 
-    def add_structdata(self, **kwargs):
+    def add_structdata(self, site, structype, azimuth, inclination, **kwargs):
         """
-        Add measurement to site
+        Add structdata to site
+
+        Args:
+            site (Site): site instance
+            structype (Structype): structype instance
+            azimuth (float): dip direction or plunge direction
+            inclination (float): dip or plunge
 
         Keyword Args:
-            site(Site): site instance
-            structype(Structype): structype instance
-            azimuth(float): dip direction or plunge direction
-            inclination(float): dip or plunge
+            description (str): structdata description
 
         Returns:
             Structdata
 
         """
-        assert "site" in kwargs, "site must be provided for structdata"
-        assert "structype" in kwargs, "structype must be provided for structdata"
-        data = Structdata(**kwargs)
+        data = Structdata(
+            site=site,
+            structype=structype,
+            azimuth=azimuth,
+            inclination=inclination,
+            **kwargs,
+        )
         self.session.add(data)
-        self.commit()
+        if self.autocommit:
+            self.commit()
         return data
 
-    def add_fol(self, fol, **kwargs):
+    def add_fol(self, site, structype, fol, **kwargs):
         """
         Add Foliation to site
 
         Args:
+            site (Site): site instance
+            structype (Structype): structype instance
             fol (Foliation): foliation instance
 
         Keyword Args:
-            site(Site): site instance
-            structype(Structype): structype instance
+            description (str): structdata description
 
         Returns:
             Structdata
 
         """
         assert isinstance(
             fol, Foliation
         ), "fol argument must be instance of Foliation class"
-        assert "site" in kwargs, "site must be provided for structdata"
-        assert "structype" in kwargs, "structype must be provided for structdata"
-        assert kwargs["structype"].planar, "structype must be planar"
-        azi, inc = fol.geo
-        kwargs["azimuth"] = azi
-        kwargs["inclination"] = inc
-        return self.add_structdata(**kwargs)
+        assert structype.planar, "structype must be planar"
+        azimuth, inclination = fol.geo
+        return self.add_structdata(site, structype, azimuth, inclination, **kwargs)
 
-    def add_lin(self, lin, **kwargs):
+    def add_lin(self, site, structype, lin, **kwargs):
         """
         Add Lineation to site
 
         Args:
+            site (Site): site instance
+            structype (Structype): structype instance
             lin (Lineation): lineation instance
 
         Keyword Args:
-            site(Site): site instance
-            structype(Structype): structype instance
+            description (str): structdata description
 
         Returns:
             Structdata
 
         """
         assert isinstance(
             lin, Lineation
         ), "lin argument must be instance of Lineation class"
-        assert "site" in kwargs, "site must be provided for structdata"
-        assert "structype" in kwargs, "structype must be provided for structdata"
-        assert not kwargs["structype"].planar, "structype must be linear"
-        azi, inc = lin.geo
-        kwargs["azimuth"] = azi
-        kwargs["inclination"] = inc
-        return self.add_structdata(**kwargs)
+        assert not structype.planar, "structype must be linear"
+        azimuth, inclination = lin.geo
+        return self.add_structdata(site, structype, azimuth, inclination, **kwargs)
 
     def attach(self, fol, lin):
         """
         Add Lineation to site
 
         Args:
             fol (Foliation): foliation instance
@@ -369,15 +488,16 @@
 
         Returns:
             Attached
 
         """
         pair = Attached(planar=fol, linear=lin)
         self.session.add(pair)
-        self.commit()
+        if self.autocommit:
+            self.commit()
         return pair
 
     def add_pair(self, pair, foltype, lintype, **kwargs):
         """
         Add attached foliation and lineation to database
 
         Args:
```

### Comparing `apsg-1.0.1/src/apsg/database/_sdbread.py` & `apsg-1.0.2/src/apsg/database/_sdbread.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/src/apsg/decorator/_decorator.py` & `apsg-1.0.2/src/apsg/decorator/_decorator.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         def wrapper(self, *args, **kwargs):
             nargs = list(args)
             ok = []
             for ix, cls in enumerate(datatypes):
                 try:
                     nargs[ix] = cls(nargs[ix])
                     ok.append(True)
-                except:
+                except Exception:
                     ok.append(False)
             if all(ok):
                 return method(self, *nargs, **kwargs)
             else:
                 raise TypeError(
                     f'Unsupported arguments for {method.__name__}. Must be {" or ".join([dt.__name__ for dt in datatypes])}'
                 )
```

### Comparing `apsg-1.0.1/src/apsg/feature/__init__.py` & `apsg-1.0.2/src/apsg/feature/__init__.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/src/apsg/feature/_container.py` & `apsg-1.0.2/src/apsg/feature/_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from apsg.config import apsg_conf
 from apsg.helpers._math import sind, cosd, atan2d
 from apsg.math._vector import Vector2, Vector3
 from apsg.helpers._math import acosd
 from apsg.feature._geodata import Lineation, Foliation, Pair, Fault, Cone
 from apsg.feature._tensor3 import OrientationTensor3, Ellipsoid
+from apsg.feature._tensor2 import OrientationTensor2, Ellipse
 from apsg.feature._statistics import KentDistribution, vonMisesFisher
 
 
 class FeatureSet:
     """
     Base class for containers
     """
@@ -264,25 +265,23 @@
     def ortensor(self):
         """Return orientation tensor ``Ortensor`` of ``Group``."""
 
         return self._ortensor
 
     @property
     def _ortensor(self):
-        # if "ortensor" not in self._cache:
-        #     self._cache["ortensor"] = OrientationTensor2.from_features(self)
-        # return self._cache["ortensor"]
-        return NotImplemented
+        if "ortensor" not in self._cache:
+            self._cache["ortensor"] = OrientationTensor2.from_features(self)
+        return self._cache["ortensor"]
 
     @property
     def _svd(self):
-        # if "svd" not in self._cache:
-        #     self._cache["svd"] = np.linalg.svd(self._ortensor)
-        # return self._cache["svd"]
-        return NotImplemented
+        if "svd" not in self._cache:
+            self._cache["svd"] = np.linalg.svd(self._ortensor)
+        return self._cache["svd"]
 
     def centered(self, max_vertical=False):
         """Rotate ``FeatureSet`` object to position that eigenvectors are parallel
         to axes of coordinate system: E1||X (north-south), E2||X(east-west),
         E3||X(vertical)
 
         Args:
@@ -1275,26 +1274,26 @@
     """
     Class to store set of ``Ellipse`` features
     """
 
     __feature_type__ = "Ellipse"
 
     @property
-    def lambda1(self) -> np.ndarray:
+    def S1(self) -> np.ndarray:
         """
-        Return the array of square root of maximum eigenvalues.
+        Return the array of maximum principal stretches.
         """
-        return np.array([e.lambda1 for e in self])
+        return np.array([e.S1 for e in self])
 
     @property
-    def lambda2(self) -> np.ndarray:
+    def S2(self) -> np.ndarray:
         """
-        Return the array of square root of minimum eigenvalues.
+        Return the array of minimum principal stretches.
         """
-        return np.array([e.lambda2 for e in self])
+        return np.array([e.S2 for e in self])
 
     @property
     def e1(self) -> np.ndarray:
         """
         Return the maximum natural principal strains.
         """
         return np.array([e.e1 for e in self])
@@ -1354,33 +1353,33 @@
     def shape(self) -> np.ndarray:
         """
         Return the array of the Woodcock shape.
         """
         return np.array([e.shape for e in self])
 
     @property
-    def lambda1(self) -> np.ndarray:
+    def S1(self) -> np.ndarray:
         """
-        Return the array of the square root of maximum eigenvalue.
+        Return the array of maximum principal stretches.
         """
-        return np.array([e.lambda1 for e in self])
+        return np.array([e.S1 for e in self])
 
     @property
-    def lambda2(self) -> np.ndarray:
+    def S2(self) -> np.ndarray:
         """
-        Return the array of the square root of middle eigenvalue.
+        Return the array of middle principal stretches.
         """
-        return np.array([e.lambda2 for e in self])
+        return np.array([e.S2 for e in self])
 
     @property
-    def lambda3(self) -> np.ndarray:
+    def S3(self) -> np.ndarray:
         """
-        Return the array of the square root of minimum eigenvalue.
+        Return the array of minimum principal stretches.
         """
-        return np.array([e.lambda3 for e in self])
+        return np.array([e.S3 for e in self])
 
     @property
     def e1(self) -> np.ndarray:
         """
         Return the array of the maximum natural principal strain.
         """
         return np.array([e.e1 for e in self])
@@ -1718,13 +1717,17 @@
             return FaultSet(lst, name=name)
         elif dtype_cls is Cone:
             return ConeSet(lst, name=name)
         elif dtype_cls is Ellipsoid:
             return EllipsoidSet(lst, name=name)
         elif dtype_cls is OrientationTensor3:
             return OrientationTensor3Set(lst, name=name)
+        elif dtype_cls is Ellipse:
+            return EllipseSet(lst, name=name)
+        elif dtype_cls is OrientationTensor2:
+            return OrientationTensor2Set(lst, name=name)
         else:
             raise TypeError("Wrong datatype to create FeatureSet")
 
 
 def angle_metric(u, v):
     return np.degrees(np.arccos(np.abs(np.dot(u, v))))
```

### Comparing `apsg-1.0.1/src/apsg/feature/_geodata.py` & `apsg-1.0.2/src/apsg/feature/_geodata.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/src/apsg/feature/_paleomag.py` & `apsg-1.0.2/src/apsg/feature/_paleomag.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/src/apsg/feature/_statistics.py` & `apsg-1.0.2/src/apsg/feature/_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         """
         Returns the normalization constant of the Kent distribution.
         The proportional error may be expected not to be greater than
         1E-11.
         """
 
         (k, b) = (self.kappa, self.beta)
-        if not (k, b) in cache:
+        if (k, b) not in cache:
             G = gamma_fun
             Imb2 = modified_bessel_2ndkind
             result = 0.0
             j = 0
             if b == 0.0:
                 result = (0.5 * k) ** (-2 * j - 0.5) * Imb2(2 * j + 0.5, k)
                 result /= G(j + 1)
@@ -299,15 +299,15 @@
     def normalize_prime(self, cache=dict(), return_num_iterations=False):
         """
         Returns the derivative of the normalization factor with respect
         to kappa and beta.
         """
 
         (k, b) = (self.kappa, self.beta)
-        if not (k, b) in cache:
+        if (k, b) not in cache:
             G = gamma_fun
             Imb2 = modified_bessel_2ndkind
             (dcdk, dcdb) = (0.0, 0.0)
             j = 0
             if b == 0:
                 dcdk = (
                     G(j + 0.5)
```

### Comparing `apsg-1.0.1/src/apsg/feature/_tensor2.py` & `apsg-1.0.2/src/apsg/feature/_tensor2.py`

 * *Files 7% similar despite different names*

```diff
@@ -375,15 +375,15 @@
 
     Example:
       >>> E = ellipse([[8, 0], [0, 2]])
       >>> E
       Ellipse
       [[8. 0.]
        [0. 2.]]
-      (ar:2, ori:90)
+      (ar:2, ori:0)
 
     """
 
     def __repr__(self) -> str:
         return (
             f"{Matrix2.__repr__(self)}\n(ar:{self.ar:.3g}, ori:{self.orientation:.3g})"
         )
@@ -411,47 +411,47 @@
     def from_stretch(cls, x=1, y=1, **kwargs) -> "Ellipse":
         """
         Return diagonal tensor defined by magnitudes of principal stretches.
         """
         return cls([[x * x, 0], [0, y * y]], **kwargs)
 
     @property
-    def lambda1(self) -> float:
+    def S1(self) -> float:
         """
-        Return the square root of maximum eigenvalue.
+        Return the maximum  principal stretch.
         """
         return math.sqrt(self.E1)
 
     @property
-    def lambda2(self) -> float:
+    def S2(self) -> float:
         """
-        Return the square root of minimum eigenvalue.
+        Return the minimum principal stretch.
         """
         return math.sqrt(self.E2)
 
     @property
     def e1(self) -> float:
         """
         Return the maximum natural principal strain.
         """
-        return math.log(self.lambda1)
+        return math.log(self.S1)
 
     @property
     def e2(self) -> float:
         """
         Return the minimum natural principal strain.
         """
-        return math.log(self.lambda2)
+        return math.log(self.S2)
 
     @property
     def ar(self) -> float:
         """
-        Return the lambda1/lambda2 ratio.
+        Return the ellipse axial ratio.
         """
-        return self.lambda1 / self.lambda2
+        return self.S1 / self.S2
 
     @property
     def orientation(self):
         """
         Return the orientation of the maximum eigenvector.
         """
         return self.eigenvectors()[np.argmax(self.eigenvalues())].direction % 180
@@ -476,35 +476,37 @@
              2x2 2D matrix. This includes lists, tuples and ndarrays.
              Array could be also ``Group`` (for backward compatibility)
 
     Returns:
       ``OrientationTensor2`` object
 
     Example:
-      >>> ot = ortensor2([[8, 0], [0, 2]])
+      >>> v = vec2set.random(n=1000)
+      >>> ot = v.ortensor()
       >>> ot
       OrientationTensor2
-      [[8. 0.]
-       [0. 2.]]
-      (ar:2, ori:90)
+      [[ 0.502 -0.011]
+       [-0.011  0.498]]
+      (ar:1.02, ori:140)
 
     """
 
     @classmethod
     def from_features(cls, g) -> "OrientationTensor2":
         """
         Return ``Ortensor`` of data in ``Group``
 
         Args:
             g: ``Group`` of ``Vector2``, ``Lin`` or ``Foliation``
 
         Example:
           >>> v = vec2set.random_vonmises(position=120)
-          >>> ortensor2.from_features(v)
+          >>> ot = v.ortensor()
+          >>> ot
           OrientationTensor2
-          [[ 0.684 -0.253]
-           [-0.253  0.316]]
-          (ar:2.09, ori:117)
+          [[ 0.377 -0.282]
+           [-0.282  0.623]]
+          (ar:2.05, ori:123)
 
         """
 
         return cls(np.dot(np.array(g).T, np.array(g)) / len(g))
```

### Comparing `apsg-1.0.1/src/apsg/feature/_tensor3.py` & `apsg-1.0.2/src/apsg/feature/_tensor3.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,14 +159,17 @@
 
         Lineation in pair define x axis and normal to foliation in pair define z axis
 
         Args:
             p1 (``Pair``): from
             p2 (``Pair``): to
 
+        Keyword Args:
+          symmetry (bool): If True, returns minimum angle rotation of axial pairs
+
         Returns:
             ``Defgrad3`` rotational matrix
 
         Example:
             >>> p1 = pair(58, 36, 81, 34)
             >>> p2 = pair(217,42, 162, 27)
             >>> R = defgrad.from_two_pairs(p1, p2)
@@ -220,15 +223,15 @@
         if abs(axis.z) > 1e-8:
             sina = (R[1][0] + (cosa - 1.0) * axis.x * axis.y) / axis.z
         elif abs(axis.y) > 1e-8:
             sina = (R[0][2] + (cosa - 1.0) * axis.x * axis.z) / axis.y
         else:
             sina = (R[2][1] + (cosa - 1.0) * axis.y * axis.z) / axis.x
         angle = np.rad2deg(np.arctan2(sina, cosa))
-        return axis, angle
+        return axis, float(angle)
 
     def velgrad(self, time=1):
         """
         Return ``VelocityGradient3`` calculated as matrix logarithm divided by given time.
 
         Keyword Args:
             time (float): total time. Default 1
@@ -584,23 +587,23 @@
     Returns:
       ``Ellipsoid`` object
 
     Example:
       >>> E = ellipsoid([[8, 0, 0], [0, 2, 0], [0, 0, 1]])
       >>> E
       Ellipsoid
-      [[8. 0. 0.]
-       [0. 2. 0.]
-       [0. 0. 1.]]
-      (λ1:2.83, λ2:1.41, λ3:1)
+      [[8 0 0]
+       [0 2 0]
+       [0 0 1]]
+      (S1:2.83, S2:1.41, S3:1)
 
     """
 
     def __repr__(self) -> str:
-        return f"{Matrix3.__repr__(self)}\n(λ1:{self.lambda1:.3g}, λ2:{self.lambda2:.3g}, λ3:{self.lambda3:.3g})"
+        return f"{Matrix3.__repr__(self)}\n(S1:{self.S1:.3g}, S2:{self.S2:.3g}, S3:{self.S3:.3g})"
 
     @classmethod
     def from_defgrad(cls, F, form="left", **kwargs) -> "Ellipsoid":
         """
         Return deformation tensor from ``Defgrad3``.
 
         Kwargs:
@@ -655,68 +658,68 @@
     def shape(self) -> float:
         """
         return the Woodcock shape.
         """
         return self.K
 
     @property
-    def lambda1(self) -> float:
+    def S1(self) -> float:
         """
-        Return the square root of maximum eigenvalue.
+        Return the maximum principal stretch.
         """
         return math.sqrt(self.E1)
 
     @property
-    def lambda2(self) -> float:
+    def S2(self) -> float:
         """
-        Return the square root of middle eigenvalue.
+        Return the middle principal stretch.
         """
         return math.sqrt(self.E2)
 
     @property
-    def lambda3(self) -> float:
+    def S3(self) -> float:
         """
-        Return the square root of minimum eigenvalue.
+        Return the minimum principal stretch.
         """
         return math.sqrt(self.E3)
 
     @property
     def e1(self) -> float:
         """
         Return the maximum natural principal strain.
         """
-        return math.log(self.lambda1)
+        return math.log(self.S1)
 
     @property
     def e2(self) -> float:
         """
         Return the middle natural principal strain.
         """
-        return math.log(self.lambda2)
+        return math.log(self.S2)
 
     @property
     def e3(self) -> float:
         """
         Return the minimum natural principal strain.
         """
-        return math.log(self.lambda3)
+        return math.log(self.S3)
 
     @property
     def Rxy(self) -> float:
         """
         Return the Rxy ratio.
         """
-        return self.lambda1 / self.lambda2 if self.lambda2 != 0 else np.inf
+        return self.S1 / self.S2 if self.S2 != 0 else float("inf")
 
     @property
     def Ryz(self) -> float:
         """
         Return the Ryz ratio.
         """
-        return self.lambda2 / self.lambda3 if self.lambda3 != 0 else np.inf
+        return self.S2 / self.S3 if self.S3 != 0 else float("inf")
 
     @property
     def e12(self) -> float:
         """
         Return the e1 - e2.
         """
         return self.e1 - self.e2
@@ -736,29 +739,29 @@
         return self.e2 - self.e3
 
     @property
     def k(self) -> float:
         """
         Return the strain symmetry.
         """
-        return (self.Rxy - 1) / (self.Ryz - 1) if self.Ryz > 1 else np.inf
+        return (self.Rxy - 1) / (self.Ryz - 1) if self.Ryz > 1 else float("inf")
 
     @property
     def d(self) -> float:
         """
         Return the strain intensity.
         """
         return math.sqrt((self.Rxy - 1) ** 2 + (self.Ryz - 1) ** 2)
 
     @property
     def K(self) -> float:
         """
         Return the strain symmetry (Ramsay, 1983).
         """
-        return self.e12 / self.e23 if self.e23 > 0 else np.inf
+        return self.e12 / self.e23 if self.e23 > 0 else float("inf")
 
     @property
     def D(self) -> float:
         """
         Return the strain intensity.
         """
         return self.e12**2 + self.e23**2
@@ -829,31 +832,31 @@
 
     @property
     def Intensity(self) -> float:
         """
         Intensity index (Lisle, 1985).
         """
 
-        return 7.5 * np.sum((np.array(self.eigenvalues()) - 1 / 3) ** 2)
+        return 7.5 * float(np.sum((np.array(self.eigenvalues()) - 1 / 3) ** 2))
 
     @property
     def aMAD_l(self) -> float:
         """
         Return approximate angular deviation from the major axis along E1.
         """
 
-        return atand(np.sqrt((1 - self.E1) / self.E1))
+        return float(atand(np.sqrt((1 - self.E1) / self.E1)))
 
     @property
     def aMAD_p(self) -> float:
         """
         Return approximate deviation from the plane normal to E3.
         """
 
-        return atand(np.sqrt(self.E3 / (1 - self.E3)))
+        return float(atand(np.sqrt(self.E3 / (1 - self.E3))))
 
     @property
     def aMAD(self) -> float:
         """
         Return approximate deviation according to shape
         """
 
@@ -865,24 +868,24 @@
     @property
     def MAD_l(self) -> float:
         """
         Return maximum angular deviation (MAD) of linearly distributed vectors.
 
         Kirschvink 1980
         """
-        return atand(np.sqrt((self.E2 + self.E3) / self.E1))
+        return float(atand(np.sqrt((self.E2 + self.E3) / self.E1)))
 
     @property
     def MAD_p(self) -> float:
         """
         Return maximum angular deviation (MAD) of planarly distributed vectors.
 
         Kirschvink 1980
         """
-        return atand(np.sqrt(self.E3 / self.E2 + self.E3 / self.E1))
+        return float(atand(np.sqrt(self.E3 / self.E2 + self.E3 / self.E1)))
 
     @property
     def MAD(self) -> float:
         """
         Return maximum angular deviation (MAD)
         """
 
@@ -907,18 +910,18 @@
     Returns:
       ``OrientationTensor3`` object
 
     Example:
       >>> ot = ortensor([[8, 0, 0], [0, 2, 0], [0, 0, 1]])
       >>> ot
       OrientationTensor3
-      [[8. 0. 0.]
-       [0. 2. 0.]
-       [0. 0. 1.]]
-      (λ1:2.83, λ2:1.41, λ3:1)
+      [[8 0 0]
+       [0 2 0]
+       [0 0 1]]
+      (S1:2.83, S2:1.41, S3:1)
 
     """
 
     @classmethod
     def from_features(cls, g) -> "OrientationTensor3":
         """
         Return ``Ortensor`` of data in ``Group``
@@ -927,46 +930,64 @@
             g: ``Group`` of ``Vector3``, ``Lin`` or ``Foliation``
 
         Example:
           >>> g = linset.random_fisher(position=lin(120,50))
           >>> ot = ortensor.from_features(g)
           >>> ot
           OrientationTensor3
-          [[ 0.142 -0.151 -0.212]
-           [-0.151  0.326  0.37 ]
-           [-0.212  0.37   0.532]]
-          (λ1:0.95, λ2:0.241, λ3:0.2)
+          [[ 0.126 -0.149 -0.202]
+           [-0.149  0.308  0.373]
+           [-0.202  0.373  0.566]]
+          (S1:0.955, S2:0.219, S3:0.2)
           >>> ot.eigenlins
-          (L:120/49, L:216/5, L:310/40)
+          (L:119/51, L:341/31, L:237/21)
 
         """
 
         return cls(np.dot(np.array(g).T, np.array(g)) / len(g))
 
     @classmethod
-    def from_pairs(cls, p) -> "OrientationTensor3":
+    def from_pairs(cls, p, shift=True) -> "OrientationTensor3":
         """
         Return Lisle (1989) ``Ortensor`` of orthogonal data in ``PairSet``
 
-        Lisle, R. (1989). The Statistical Analysis of Orthogonal Orientation Data. The Journal of Geology, 97(3), 360-364.
+        Lisle, R. (1989). The Statistical Analysis of Orthogonal Orientation Data.
+            The Journal of Geology, 97(3), 360-364.
+
+        Note: Tensor is by default shifted towards positive eigenvalues, so it
+            could be used as Scheidegger orientation tensor for plotting. When
+            original Lisle tensor is needed, set shift to False.
 
         Args:
             p: ``PairSet``
 
+        Keyword Args:
+            shift (bool): When True the tensor is shifted. Default True
+
         Example:
           >>> p = pairset([pair(109, 82, 21, 10),
                            pair(118, 76, 30, 11),
                            pair(97, 86, 7, 3),
                            pair(109, 75, 23, 14)])
           >>> ot = ortensor.from_pairs(p)
           >>> ot
           OrientationTensor3
-          [[ 0.731  0.575  0.086]
-           [ 0.575 -0.725  0.224]
-           [ 0.086  0.224 -0.005]]
-          (λ1:0.98, λ2:0.978, λ3:0.0688)
+          [[0.577 0.192 0.029]
+           [0.192 0.092 0.075]
+           [0.029 0.075 0.332]]
+          (S1:0.807, S2:0.579, S3:0.114)
 
         """
-        return cls(
-            OrientationTensor3.from_features(p.lvec)
-            - OrientationTensor3.from_features(p.fvec)
-        )
+        if shift:
+            return cls(
+                (
+                    OrientationTensor3.from_features(p.lvec)
+                    - OrientationTensor3.from_features(p.fvec)
+                    + np.eye(3)
+                )
+                / 3
+            )
+        else:
+            return cls(
+                OrientationTensor3.from_features(p.lvec)
+                - OrientationTensor3.from_features(p.fvec)
+            )
```

### Comparing `apsg-1.0.1/src/apsg/helpers/__init__.py` & `apsg-1.0.2/src/apsg/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/src/apsg/helpers/_math.py` & `apsg-1.0.2/src/apsg/helpers/_math.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/src/apsg/helpers/_notation.py` & `apsg-1.0.2/src/apsg/helpers/_notation.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/src/apsg/math/_matrix.py` & `apsg-1.0.2/src/apsg/math/_matrix.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/src/apsg/math/_vector.py` & `apsg-1.0.2/src/apsg/math/_vector.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/src/apsg/plotting/__init__.py` & `apsg-1.0.2/src/apsg/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/src/apsg/plotting/_fabricplot.py` & `apsg-1.0.2/src/apsg/plotting/_fabricplot.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/src/apsg/plotting/_paleomagplots.py` & `apsg-1.0.2/src/apsg/plotting/_paleomagplots.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/src/apsg/plotting/_plot_artists.py` & `apsg-1.0.2/src/apsg/plotting/_plot_artists.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/src/apsg/plotting/_projection.py` & `apsg-1.0.2/src/apsg/plotting/_projection.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/src/apsg/plotting/_roseplot.py` & `apsg-1.0.2/src/apsg/plotting/_roseplot.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/src/apsg/plotting/_stereogrid.py` & `apsg-1.0.2/src/apsg/plotting/_stereogrid.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/src/apsg/plotting/_stereonet.py` & `apsg-1.0.2/src/apsg/plotting/_stereonet.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,19 +222,29 @@
 
         Args:
             fig (Figure): A mtplotlib Figure artist
         """
         self.fig = fig
         self._render()
 
+    def format_coord(self, x, y):
+        """Format stereonet coordinates"""
+        if x is not None and y is not None:
+            if (x**2 + y**2) <= 1:
+                l = Lineation(*self.proj.inverse_data(x, y))
+                f = Foliation(*self.proj.inverse_data(x, y))
+                return f"{l} {f}"
+        return ""
+
     def show(self):
         """Show stereonet"""
         plt.close(0)  # close previously rendered figure
         self.init_figure()
         self._render()
+        self.ax.format_coord = self.format_coord
         plt.show()
 
     def savefig(self, filename="stereonet.png", **kwargs):
         """
         Save stereonet figure to graphics file
 
         Keyword Args:
@@ -477,26 +487,34 @@
                 h.set_clip_path(self.primitive)
         return handles
 
     def _scatter(self, *args, **kwargs):
         legend = kwargs.pop("legend")
         num = kwargs.pop("num")
         x_lower, y_lower = self.proj.project_data(*np.vstack(args).T)
-        mask_lower = ~np.isnan(x_lower)
-        x_upper, y_upper, mask_upper = self.proj.project_data(*(-np.vstack(args).T))
-        mask_upper = ~np.isnan(x_upper)
+        # mask_lower = ~np.isnan(x_lower)
+        x_upper, y_upper = self.proj.project_data(*(-np.vstack(args).T))
+        # mask_upper = ~np.isnan(x_upper)
+        # x_lower, y_lower, x_upper, y_upper = self.proj.project_data_antipodal(
+        #    *np.vstack(args).T
+        # )
         prop = "sizes"
         if kwargs["s"] is not None:
             s = np.atleast_1d(kwargs["s"])
-            kwargs["s"] = np.hstack((s[mask_lower], s[mask_upper]))
+            # kwargs["s"] = np.hstack((s[mask_lower], s[mask_upper]))
+            kwargs["s"] = np.hstack((s, s))
         if kwargs["c"] is not None:
             c = np.atleast_1d(kwargs["c"])
-            kwargs["c"] = np.hstack((c[mask_lower], c[mask_upper]))
+            # kwargs["c"] = np.hstack((c[mask_lower], c[mask_upper]))
+            kwargs["c"] = np.hstack((c, c))
             prop = "colors"
         sc = self.ax.scatter(
+            # np.hstack((x_lower[mask_lower], x_upper[mask_upper])),
+            # np.hstack((y_lower[mask_lower], y_upper[mask_upper])),
+            # **kwargs,
             np.hstack((x_lower, x_upper)),
             np.hstack((y_lower, y_upper)),
             **kwargs,
         )
         if legend:
             self.ax.legend(
                 *sc.legend_elements(prop, num=num),
```

### Comparing `apsg-1.0.1/src/apsg/shell.py` & `apsg-1.0.2/src/apsg/shell.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/src/apsg.egg-info/PKG-INFO` & `apsg-1.0.2/src/apsg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apsg
-Version: 1.0.1
+Version: 1.0.2
 Summary: APSG - The package for structural geologists
 Home-page: https://github.com/ondrolexa/apsg
 Author: Ondrej Lexa
 Author-email: lexa.ondrej@gmail.com
 License: MIT
 Project-URL: Documentation, https://apsg.readthedocs.io/
 Project-URL: Source Code, https://github.com/ondrolexa/apsg/
@@ -127,14 +127,18 @@
 ## License
 
 APSG is free software: you can redistribute it and/or modify it under the terms of the MIT License. A copy of this license is provided in ``LICENSE`` file.
 
 
 # Changes
 
+### 1.0.2 (Apr 30 2023)
+ * lambda properties of tensors renamed to S
+ * cursor coordinates in stereonet show lin and fol
+
 ### 1.0.1 (Nov 22 2022)
  * density_lookup method implemented for StereoNet.grid
  * Stress tensor sigma* properties using inverted order of eigenvalues
  * render2fig method of StereoNet implemented
  * vector-like objects are not iterable, so properly render in pandas 
 
 ## 1.0.0 (Oct 7 2022)
```

### Comparing `apsg-1.0.1/src/apsg.egg-info/SOURCES.txt` & `apsg-1.0.2/src/apsg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/tests/conftest.py` & `apsg-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/tests/test_apsg.py` & `apsg-1.0.2/tests/test_apsg.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.1/tests/test_tensors.py` & `apsg-1.0.2/tests/test_tensors.py`

 * *Files identical despite different names*

