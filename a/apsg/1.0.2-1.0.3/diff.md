# Comparing `tmp/apsg-1.0.2.tar.gz` & `tmp/apsg-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apsg-1.0.2.tar", last modified: Sun Apr 30 10:38:29 2023, max compression
+gzip compressed data, was "apsg-1.0.3.tar", last modified: Sun Apr 30 12:23:47 2023, max compression
```

## Comparing `apsg-1.0.2.tar` & `apsg-1.0.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.220525 apsg-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-30 10:38:13.000000 apsg-1.0.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-30 10:38:13.000000 apsg-1.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-30 10:38:13.000000 apsg-1.0.2/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-30 10:38:13.000000 apsg-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-30 10:38:13.000000 apsg-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-04-30 10:38:29.220525 apsg-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-30 10:38:13.000000 apsg-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.216525 apsg-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/apsg.database.rst
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/apsg.feature.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/apsg.helpers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/apsg.math.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/apsg.plotting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/automodules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-30 10:38:13.000000 apsg-1.0.2/docs/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-30 10:38:13.000000 apsg-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-30 10:38:29.220525 apsg-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-30 10:38:13.000000 apsg-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.212525 apsg-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.216525 apsg-1.0.2/src/apsg/
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.216525 apsg-1.0.2/src/apsg/database/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/database/_alchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/database/_sdbread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.216525 apsg-1.0.2/src/apsg/decorator/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/decorator/_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.220525 apsg-1.0.2/src/apsg/feature/
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56754 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/feature/_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    21489 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/feature/_geodata.py
--rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/feature/_paleomag.py
--rw-r--r--   0 runner    (1001) docker     (123)    13916 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/feature/_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/feature/_tensor2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25724 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/feature/_tensor3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.220525 apsg-1.0.2/src/apsg/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/helpers/_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/helpers/_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/helpers/_notation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.220525 apsg-1.0.2/src/apsg/math/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/math/_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    16409 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/math/_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.220525 apsg-1.0.2/src/apsg/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/plotting/_fabricplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/plotting/_paleomagplots.py
--rw-r--r--   0 runner    (1001) docker     (123)    20299 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/plotting/_plot_artists.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/plotting/_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/plotting/_roseplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/plotting/_stereogrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    28705 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/plotting/_stereonet.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-30 10:38:13.000000 apsg-1.0.2/src/apsg/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.216525 apsg-1.0.2/src/apsg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-04-30 10:38:29.000000 apsg-1.0.2/src/apsg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-30 10:38:29.000000 apsg-1.0.2/src/apsg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 10:38:29.000000 apsg-1.0.2/src/apsg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-30 10:38:29.000000 apsg-1.0.2/src/apsg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-30 10:38:29.000000 apsg-1.0.2/src/apsg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 10:38:29.000000 apsg-1.0.2/src/apsg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:29.220525 apsg-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:38:13.000000 apsg-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-30 10:38:13.000000 apsg-1.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-04-30 10:38:13.000000 apsg-1.0.2/tests/test_apsg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-30 10:38:13.000000 apsg-1.0.2/tests/test_tensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:23:47.855253 apsg-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-30 12:23:34.000000 apsg-1.0.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-30 12:23:34.000000 apsg-1.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-30 12:23:34.000000 apsg-1.0.3/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-30 12:23:34.000000 apsg-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-30 12:23:34.000000 apsg-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-04-30 12:23:47.855253 apsg-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-30 12:23:34.000000 apsg-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:23:47.847253 apsg-1.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-04-30 12:23:34.000000 apsg-1.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-30 12:23:34.000000 apsg-1.0.3/docs/apsg.database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 12:23:34.000000 apsg-1.0.3/docs/apsg.feature.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-30 12:23:34.000000 apsg-1.0.3/docs/apsg.helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-30 12:23:34.000000 apsg-1.0.3/docs/apsg.math.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-30 12:23:34.000000 apsg-1.0.3/docs/apsg.plotting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-30 12:23:34.000000 apsg-1.0.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-30 12:23:34.000000 apsg-1.0.3/docs/automodules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-04-30 12:23:34.000000 apsg-1.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-30 12:23:34.000000 apsg-1.0.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-30 12:23:34.000000 apsg-1.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-30 12:23:34.000000 apsg-1.0.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-04-30 12:23:34.000000 apsg-1.0.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-30 12:23:34.000000 apsg-1.0.3/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-30 12:23:34.000000 apsg-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-30 12:23:47.855253 apsg-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-30 12:23:34.000000 apsg-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:23:47.847253 apsg-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:23:47.847253 apsg-1.0.3/src/apsg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:23:47.851253 apsg-1.0.3/src/apsg/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/database/_alchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/database/_sdbread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:23:47.851253 apsg-1.0.3/src/apsg/decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/decorator/_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:23:47.851253 apsg-1.0.3/src/apsg/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56754 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/feature/_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21489 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/feature/_geodata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/feature/_paleomag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13916 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/feature/_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/feature/_tensor2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25724 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/feature/_tensor3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:23:47.851253 apsg-1.0.3/src/apsg/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/helpers/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/helpers/_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/helpers/_notation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:23:47.851253 apsg-1.0.3/src/apsg/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/math/_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16409 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/math/_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:23:47.851253 apsg-1.0.3/src/apsg/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/plotting/_fabricplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/plotting/_paleomagplots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20299 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/plotting/_plot_artists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/plotting/_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/plotting/_roseplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/plotting/_stereogrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28705 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/plotting/_stereonet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-30 12:23:34.000000 apsg-1.0.3/src/apsg/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:23:47.851253 apsg-1.0.3/src/apsg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-04-30 12:23:47.000000 apsg-1.0.3/src/apsg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-30 12:23:47.000000 apsg-1.0.3/src/apsg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:23:47.000000 apsg-1.0.3/src/apsg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-30 12:23:47.000000 apsg-1.0.3/src/apsg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-30 12:23:47.000000 apsg-1.0.3/src/apsg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 12:23:47.000000 apsg-1.0.3/src/apsg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:23:47.851253 apsg-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 12:23:34.000000 apsg-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-30 12:23:34.000000 apsg-1.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-04-30 12:23:34.000000 apsg-1.0.3/tests/test_apsg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-30 12:23:34.000000 apsg-1.0.3/tests/test_tensors.py
```

### Comparing `apsg-1.0.2/CONTRIBUTING.md` & `apsg-1.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/HISTORY.md` & `apsg-1.0.3/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Changes
 
-### 1.0.2 (Apr 30 2023)
+### 1.0.3 (Apr 30 2023)
  * lambda properties of tensors renamed to S
  * cursor coordinates in stereonet show lin and fol
 
 ### 1.0.1 (Nov 22 2022)
  * density_lookup method implemented for StereoNet.grid
  * Stress tensor sigma* properties using inverted order of eigenvalues
  * render2fig method of StereoNet implemented
```

### Comparing `apsg-1.0.2/LICENSE` & `apsg-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/PKG-INFO` & `apsg-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apsg
-Version: 1.0.2
+Version: 1.0.3
 Summary: APSG - The package for structural geologists
 Home-page: https://github.com/ondrolexa/apsg
 Author: Ondrej Lexa
 Author-email: lexa.ondrej@gmail.com
 License: MIT
 Project-URL: Documentation, https://apsg.readthedocs.io/
 Project-URL: Source Code, https://github.com/ondrolexa/apsg/
@@ -127,15 +127,15 @@
 ## License
 
 APSG is free software: you can redistribute it and/or modify it under the terms of the MIT License. A copy of this license is provided in ``LICENSE`` file.
 
 
 # Changes
 
-### 1.0.2 (Apr 30 2023)
+### 1.0.3 (Apr 30 2023)
  * lambda properties of tensors renamed to S
  * cursor coordinates in stereonet show lin and fol
 
 ### 1.0.1 (Nov 22 2022)
  * density_lookup method implemented for StereoNet.grid
  * Stress tensor sigma* properties using inverted order of eigenvalues
  * render2fig method of StereoNet implemented
```

### Comparing `apsg-1.0.2/README.md` & `apsg-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/docs/Makefile` & `apsg-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/docs/apsg.database.rst` & `apsg-1.0.3/docs/apsg.database.rst`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/docs/conf.py` & `apsg-1.0.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,24 +57,24 @@
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = u"APSG"
-copyright = u"2022, Ondrej Lexa"
+copyright = u"2023, Ondrej Lexa"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 version = "1.0"
 # The full version, including alpha/beta/rc tags.
-release = "1.0.2"
+release = "1.0.3"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to
 # some non-false value, then it is used:
```

### Comparing `apsg-1.0.2/docs/contributing.rst` & `apsg-1.0.3/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/docs/index.rst` & `apsg-1.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/docs/installation.rst` & `apsg-1.0.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/docs/make.bat` & `apsg-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/setup.py` & `apsg-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open(path.join(CURRENT_PATH, "HISTORY.md")) as file:
     history = file.read()
 
 setup(
     name="apsg",
-    version="1.0.2",
+    version="1.0.3",
     description="APSG - The package for structural geologists",
     long_description=readme + "\n\n" + history,
     long_description_content_type="text/markdown",
     author="Ondrej Lexa",
     author_email="lexa.ondrej@gmail.com",
     url="https://github.com/ondrolexa/apsg",
     license="MIT",
```

### Comparing `apsg-1.0.2/src/apsg/__init__.py` & `apsg-1.0.3/src/apsg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,10 +94,10 @@
     "VollmerPlot",
     "RamsayPlot",
     "FlinnPlot",
     "HsuPlot",
     "quicknet",
 )
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 __author__ = "Ondrej Lexa"
 __email__ = "lexa.ondrej@gmail.com"
```

### Comparing `apsg-1.0.2/src/apsg/config.py` & `apsg-1.0.3/src/apsg/config.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/database/_alchemy.py` & `apsg-1.0.3/src/apsg/database/_alchemy.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/database/_sdbread.py` & `apsg-1.0.3/src/apsg/database/_sdbread.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/decorator/_decorator.py` & `apsg-1.0.3/src/apsg/decorator/_decorator.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/feature/__init__.py` & `apsg-1.0.3/src/apsg/feature/__init__.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/feature/_container.py` & `apsg-1.0.3/src/apsg/feature/_container.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/feature/_geodata.py` & `apsg-1.0.3/src/apsg/feature/_geodata.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/feature/_paleomag.py` & `apsg-1.0.3/src/apsg/feature/_paleomag.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/feature/_statistics.py` & `apsg-1.0.3/src/apsg/feature/_statistics.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/feature/_tensor2.py` & `apsg-1.0.3/src/apsg/feature/_tensor2.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/feature/_tensor3.py` & `apsg-1.0.3/src/apsg/feature/_tensor3.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/helpers/__init__.py` & `apsg-1.0.3/src/apsg/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/helpers/_math.py` & `apsg-1.0.3/src/apsg/helpers/_math.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/helpers/_notation.py` & `apsg-1.0.3/src/apsg/helpers/_notation.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/math/_matrix.py` & `apsg-1.0.3/src/apsg/math/_matrix.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/math/_vector.py` & `apsg-1.0.3/src/apsg/math/_vector.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/plotting/__init__.py` & `apsg-1.0.3/src/apsg/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/plotting/_fabricplot.py` & `apsg-1.0.3/src/apsg/plotting/_fabricplot.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/plotting/_paleomagplots.py` & `apsg-1.0.3/src/apsg/plotting/_paleomagplots.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/plotting/_plot_artists.py` & `apsg-1.0.3/src/apsg/plotting/_plot_artists.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/plotting/_projection.py` & `apsg-1.0.3/src/apsg/plotting/_projection.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/plotting/_roseplot.py` & `apsg-1.0.3/src/apsg/plotting/_roseplot.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/plotting/_stereogrid.py` & `apsg-1.0.3/src/apsg/plotting/_stereogrid.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/plotting/_stereonet.py` & `apsg-1.0.3/src/apsg/plotting/_stereonet.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg/shell.py` & `apsg-1.0.3/src/apsg/shell.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/src/apsg.egg-info/PKG-INFO` & `apsg-1.0.3/src/apsg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apsg
-Version: 1.0.2
+Version: 1.0.3
 Summary: APSG - The package for structural geologists
 Home-page: https://github.com/ondrolexa/apsg
 Author: Ondrej Lexa
 Author-email: lexa.ondrej@gmail.com
 License: MIT
 Project-URL: Documentation, https://apsg.readthedocs.io/
 Project-URL: Source Code, https://github.com/ondrolexa/apsg/
@@ -127,15 +127,15 @@
 ## License
 
 APSG is free software: you can redistribute it and/or modify it under the terms of the MIT License. A copy of this license is provided in ``LICENSE`` file.
 
 
 # Changes
 
-### 1.0.2 (Apr 30 2023)
+### 1.0.3 (Apr 30 2023)
  * lambda properties of tensors renamed to S
  * cursor coordinates in stereonet show lin and fol
 
 ### 1.0.1 (Nov 22 2022)
  * density_lookup method implemented for StereoNet.grid
  * Stress tensor sigma* properties using inverted order of eigenvalues
  * render2fig method of StereoNet implemented
```

### Comparing `apsg-1.0.2/src/apsg.egg-info/SOURCES.txt` & `apsg-1.0.3/src/apsg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/tests/conftest.py` & `apsg-1.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/tests/test_apsg.py` & `apsg-1.0.3/tests/test_apsg.py`

 * *Files identical despite different names*

### Comparing `apsg-1.0.2/tests/test_tensors.py` & `apsg-1.0.3/tests/test_tensors.py`

 * *Files identical despite different names*

