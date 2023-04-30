# Comparing `tmp/toolbox-1.8.1.tar.gz` & `tmp/toolbox-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolbox-1.8.1.tar", last modified: Wed Jan  5 05:26:02 2022, max compression
+gzip compressed data, was "toolbox-1.9.0.tar", last modified: Wed May 25 00:38:07 2022, max compression
```

## Comparing `toolbox-1.8.1.tar` & `toolbox-1.9.0.tar`

### file list

```diff
@@ -1,84 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.437577 toolbox-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-01-05 05:25:50.000000 toolbox-1.8.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.429576 toolbox-1.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.433577 toolbox-1.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-01-05 05:25:50.000000 toolbox-1.8.1/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-01-05 05:25:50.000000 toolbox-1.8.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-01-05 05:25:50.000000 toolbox-1.8.1/.github/workflows/pytest-cover-run.yml
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-01-05 05:26:02.000000 toolbox-1.8.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-01-05 05:26:02.000000 toolbox-1.8.1/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-01-05 05:25:50.000000 toolbox-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    12944 2022-01-05 05:26:02.437577 toolbox-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11983 2022-01-05 05:25:50.000000 toolbox-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.433577 toolbox-1.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-01-05 05:25:50.000000 toolbox-1.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-01-05 05:25:50.000000 toolbox-1.8.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-01-05 05:25:50.000000 toolbox-1.8.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.433577 toolbox-1.8.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.433577 toolbox-1.8.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-05 05:25:50.000000 toolbox-1.8.1/docs/source/_static/.folder
--rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-01-05 05:25:50.000000 toolbox-1.8.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-01-05 05:25:50.000000 toolbox-1.8.1/docs/source/contents.rst
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-01-05 05:25:50.000000 toolbox-1.8.1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.433577 toolbox-1.8.1/docs/source/module/
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-01-05 05:25:50.000000 toolbox-1.8.1/docs/source/module/asyncio.rst
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-01-05 05:25:50.000000 toolbox-1.8.1/docs/source/module/builtins.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4463 2022-01-05 05:25:50.000000 toolbox-1.8.1/docs/source/module/collections.rst
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-01-05 05:25:50.000000 toolbox-1.8.1/docs/source/module/config.rst
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-01-05 05:25:50.000000 toolbox-1.8.1/docs/source/module/experimental.rst
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-01-05 05:25:50.000000 toolbox-1.8.1/docs/source/module/functools.rst
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-01-05 05:25:50.000000 toolbox-1.8.1/docs/source/module/pkgutil.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-01-05 05:25:50.000000 toolbox-1.8.1/docs/source/module/string.rst
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-01-05 05:25:50.000000 toolbox-1.8.1/docs/source/module/textwrap.rst
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-01-05 05:26:02.437577 toolbox-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-01-05 05:25:50.000000 toolbox-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.433577 toolbox-1.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-05 05:25:50.000000 toolbox-1.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-01-05 05:25:50.000000 toolbox-1.8.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3564 2022-01-05 05:25:50.000000 toolbox-1.8.1/tests/test_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-01-05 05:25:50.000000 toolbox-1.8.1/tests/test_buildins.py
--rw-r--r--   0 runner    (1001) docker     (121)     8508 2022-01-05 05:25:50.000000 toolbox-1.8.1/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-01-05 05:25:50.000000 toolbox-1.8.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-01-05 05:25:50.000000 toolbox-1.8.1/tests/test_functools.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-01-05 05:25:50.000000 toolbox-1.8.1/tests/test_pkgutil.py
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-01-05 05:25:50.000000 toolbox-1.8.1/tests/test_string.py
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-01-05 05:25:50.000000 toolbox-1.8.1/tests/test_textwrap.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.433577 toolbox-1.8.1/toolbox/
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.437577 toolbox-1.8.1/toolbox/asyncio/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6457 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/asyncio/pattern.py
--rw-r--r--   0 runner    (1001) docker     (121)     2734 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/asyncio/streams.py
--rw-r--r--   0 runner    (1001) docker     (121)     2530 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/asyncio/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.437577 toolbox-1.8.1/toolbox/builtins/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/builtins/property.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.437577 toolbox-1.8.1/toolbox/collections/
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5568 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/collections/item.py
--rw-r--r--   0 runner    (1001) docker     (121)     6351 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/collections/mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/collections/namedtuple.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.437577 toolbox-1.8.1/toolbox/config/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/config/globalconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.437577 toolbox-1.8.1/toolbox/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2950 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/experimental/asyncdispatch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.437577 toolbox-1.8.1/toolbox/functools/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/functools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2440 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/functools/timeout.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.437577 toolbox-1.8.1/toolbox/pkgutil/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/pkgutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2388 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/pkgutil/package.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.437577 toolbox-1.8.1/toolbox/string/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6286 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/string/color.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.437577 toolbox-1.8.1/toolbox/textwrap/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/textwrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-01-05 05:25:50.000000 toolbox-1.8.1/toolbox/textwrap/text.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 05:26:02.433577 toolbox-1.8.1/toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12944 2022-01-05 05:26:02.000000 toolbox-1.8.1/toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-01-05 05:26:02.000000 toolbox-1.8.1/toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-05 05:26:02.000000 toolbox-1.8.1/toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-05 05:26:01.000000 toolbox-1.8.1/toolbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-01-05 05:26:02.000000 toolbox-1.8.1/toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.269176 toolbox-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-05-25 00:37:45.000000 toolbox-1.9.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.257176 toolbox-1.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.257176 toolbox-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-05-25 00:37:45.000000 toolbox-1.9.0/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-05-25 00:37:45.000000 toolbox-1.9.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      908 2022-05-25 00:37:45.000000 toolbox-1.9.0/.github/workflows/pytest-cover-run.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-05-25 00:38:07.000000 toolbox-1.9.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-05-25 00:38:07.000000 toolbox-1.9.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-05-25 00:37:45.000000 toolbox-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    12667 2022-05-25 00:38:07.269176 toolbox-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    11706 2022-05-25 00:37:45.000000 toolbox-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.261175 toolbox-1.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      731 2022-05-25 00:37:45.000000 toolbox-1.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      799 2022-05-25 00:37:45.000000 toolbox-1.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-05-25 00:37:45.000000 toolbox-1.9.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.261175 toolbox-1.9.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.261175 toolbox-1.9.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-25 00:37:45.000000 toolbox-1.9.0/docs/source/_static/.folder
+-rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-05-25 00:37:45.000000 toolbox-1.9.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-05-25 00:37:45.000000 toolbox-1.9.0/docs/source/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-05-25 00:37:45.000000 toolbox-1.9.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.261175 toolbox-1.9.0/docs/source/module/
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2022-05-25 00:37:45.000000 toolbox-1.9.0/docs/source/module/asyncio.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2022-05-25 00:37:45.000000 toolbox-1.9.0/docs/source/module/builtins.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4463 2022-05-25 00:37:45.000000 toolbox-1.9.0/docs/source/module/collections.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2022-05-25 00:37:45.000000 toolbox-1.9.0/docs/source/module/config.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      518 2022-05-25 00:37:45.000000 toolbox-1.9.0/docs/source/module/experimental.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2022-05-25 00:37:45.000000 toolbox-1.9.0/docs/source/module/functools.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-05-25 00:37:45.000000 toolbox-1.9.0/docs/source/module/pkgutil.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-05-25 00:37:45.000000 toolbox-1.9.0/docs/source/module/sockets.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-05-25 00:37:45.000000 toolbox-1.9.0/docs/source/module/string.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-05-25 00:37:45.000000 toolbox-1.9.0/docs/source/module/textwrap.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      915 2022-05-25 00:38:07.269176 toolbox-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-05-25 00:37:45.000000 toolbox-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.265175 toolbox-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-25 00:37:45.000000 toolbox-1.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-05-25 00:37:45.000000 toolbox-1.9.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3564 2022-05-25 00:37:45.000000 toolbox-1.9.0/tests/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-05-25 00:37:45.000000 toolbox-1.9.0/tests/test_buildins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8508 2022-05-25 00:37:45.000000 toolbox-1.9.0/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2022-05-25 00:37:45.000000 toolbox-1.9.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-05-25 00:37:45.000000 toolbox-1.9.0/tests/test_functools.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-05-25 00:37:45.000000 toolbox-1.9.0/tests/test_pkgutil.py
+-rw-r--r--   0 runner    (1001) docker     (121)      305 2022-05-25 00:37:45.000000 toolbox-1.9.0/tests/test_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-05-25 00:37:45.000000 toolbox-1.9.0/tests/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-05-25 00:37:45.000000 toolbox-1.9.0/tests/test_textwrap.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.265175 toolbox-1.9.0/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.265175 toolbox-1.9.0/toolbox/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5871 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/asyncio/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2734 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/asyncio/streams.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2530 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/asyncio/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.265175 toolbox-1.9.0/toolbox/builtins/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      690 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/builtins/property.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.265175 toolbox-1.9.0/toolbox/collections/
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5568 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/collections/item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6351 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/collections/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/collections/namedtuple.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.265175 toolbox-1.9.0/toolbox/config/
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/config/globalconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.265175 toolbox-1.9.0/toolbox/functools/
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/functools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2664 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/functools/timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.265175 toolbox-1.9.0/toolbox/pkgutil/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/pkgutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2388 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/pkgutil/package.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.265175 toolbox-1.9.0/toolbox/sockets/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/sockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      339 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/sockets/ip.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.265175 toolbox-1.9.0/toolbox/string/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6286 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/string/color.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.265175 toolbox-1.9.0/toolbox/textwrap/
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/textwrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      952 2022-05-25 00:37:45.000000 toolbox-1.9.0/toolbox/textwrap/text.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 00:38:07.265175 toolbox-1.9.0/toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    12667 2022-05-25 00:38:07.000000 toolbox-1.9.0/toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1705 2022-05-25 00:38:07.000000 toolbox-1.9.0/toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-25 00:38:07.000000 toolbox-1.9.0/toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-25 00:38:03.000000 toolbox-1.9.0/toolbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-05-25 00:38:07.000000 toolbox-1.9.0/toolbox.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-05-25 00:38:07.000000 toolbox-1.9.0/toolbox.egg-info/top_level.txt
```

### Comparing `toolbox-1.8.1/.github/workflows/docs-publish.yml` & `toolbox-1.9.0/.github/workflows/docs-publish.yml`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/.github/workflows/pypi-publish.yml` & `toolbox-1.9.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/.github/workflows/pytest-cover-run.yml` & `toolbox-1.9.0/.github/workflows/pytest-cover-run.yml`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/LICENSE` & `toolbox-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/PKG-INFO` & `toolbox-1.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolbox
-Version: 1.8.1
+Version: 1.9.0
 Summary: Extends Python with useful features.
 Home-page: https://github.com/synchronizing/toolbox
 Author: Felipe Faria
 Author-email: felipefaria@hey.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/synchronizing/toolbox/issues
 Project-URL: Documentation, https://synchronizing.github.io/toolbox/
@@ -53,21 +53,19 @@
 
 ## Documentation
 
 Documentation can be found [**here**](http://synchronizing.github.io/toolbox/).
 
 ## Using
 
-Toolbox follows the same pattern as of the Python Standard Library (PSL) which means that all tools are found inside package names that corresponds to that of the PSL (e.g. `asyncio`, `collections`, etc.) with only one exception (`config`). Check out documentation for function definitions and more details.
-
 ### `asyncio`
 
 #### [`async to_thread`](https://synchronizing.github.io/toolbox/module/asyncio.html#toolbox.asyncio.threads.to_thread)
 
-Runs passed function in a new thread to ensure non-blocking IO during asynchronous programming.
+Runs given function in a new thread during asynchronous IO.
 
 ```python
 from toolbox import to_thread
 import asyncio
 import time
 
 def func():
@@ -115,50 +113,66 @@
     # Communication is now encrypted.
 
 asyncio.run(client())
 ```
 
 #### [`CoroutineClass`](https://synchronizing.github.io/toolbox/module/asyncio.html#toolbox.asyncio.pattern.CoroutineClass)
 
-Useful pattern to add non-blocking start/stop functions and an async context manager to a class.
+Pattern for creating a coroutine-like class that has multiple ways to start it.
 
 ```python
 from toolbox import CoroutineClass
 import asyncio
 
 class Coroutine(CoroutineClass):
     def __init__(self, run: bool = False):
         super().__init__(run=run)
 
+    # Default entry function.
     async def entry(self):
-        # Default entry function.
-        # Some async functionality here.
+        await asyncio.sleep(1)
+        return "Hello world"
 
-async def main():
+# Start coroutine outside Python async context.
+def iomain():
 
-    # Use with __init__ start.
-    process = AsyncClass(start=True)
-    await asyncio.sleep(1)
-    process.stop()
+    # via __init__
+    coro = Coroutine(run=True)
+    print(coro.result)  # Hello world
+
+    # via .run()
+    coro = Coroutine()
+    result = coro.run()
+    print(result)  # Hello world
 
-    # Use with functions to start/stop.
-    process = AsyncClass()
-    process.start()
+# Start coroutine inside Python async context.
+async def aiomain():
+
+    # via __init__
+    coro = Coroutine(run=True)
     await asyncio.sleep(1)
-    process.stop()
+    coro.stop()
+    print(coro.result)  # None - because process was stopped before completion.
 
-    # Use with context manager to start/stop.
-    async with AsyncClass() as process:
-        ...
-
-    # Use it with await.
-    process = AsyncClass()
-    await process
+    # via .run()
+    coro = Coroutine()
+    coro.run()
+    await asyncio.sleep(1)
+    result = coro.stop()  # None - because coroutine was stopped before completion.
+    print(result)  # Hello world
 
-asyncio.run(main())
+    # via await
+    coro = Coroutine()
+    result = await coro  # You can also start, and await later.
+    print(result)  # Hello World
+
+    # via context manager
+    async with Coroutine() as coro:
+        result = await coro
+    print(result)  # Hello World
 ```
 
 ### `builtins`
 
 #### [`classproperty`](https://synchronizing.github.io/toolbox/module/builtins.html#toolbox.builtins.property.classproperty)
 
 Combines a `property` and a `classmethod` into one, creating a class property. Allows access to computed class attributes.
@@ -167,142 +181,142 @@
 from toolbox import classproperty
 
 class Animal:
     @classproperty
     def dog(cls):
         return "whoof!"
 
-print(Animal.dog) # >>> 'whoof!'
+print(Animal.dog) #  'whoof!'
 ```
 
 
 ### `collections`
 
 #### [`Item`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.item.Item)
 
 An interface for type-agnostic operations between different types.
 
 ```python
 from toolbox import Item
 
 item = Item(100)
-print(item == b"100" == "100" == 100) # >>> True
+print(item == b"100" == "100" == 100) #  True
 ```
 
 #### [`BidirectionalDict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.mapping.BidirectionalDict)
 
 Dictionary with two-way capabilities.
 
 ```python
 from toolbox import BidirectionalDict
 
 d = BidirectionalDict({"hello": "world"})
-print(d) # >>> {'hello': 'world', 'world': 'hello'}
+print(d) #  {'hello': 'world', 'world': 'hello'}
 ```
 
 #### [`ObjectDict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.mapping.ObjectDict)
 
 Dictionary that can be accessed as though it was an object.
 
 ```python
 from toolbox import ObjectDict
 
 d = ObjectDict({"hello": "world"})
-print(d.hello) # >>> 'world'
+print(d.hello) #  'world'
 ```
 
 #### [`OverloadedDict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.mapping.OverloadedDict)
 
 Dictionary that can be added or subtracted to.
 
 ```python
 from toolbox import OverloadedDict
 
 d1 = OverloadedDict({"hello": "world"})
 d2 = OverloadedDict({"ola": "mundo"})
 
 d1 += d2
-print(d1) # >>> {'hello': 'world', 'ola': 'mundo'}
+print(d1) #  {'hello': 'world', 'ola': 'mundo'}
 
 d1 -= d2
-print(d1) # >>> {'hello': 'world'}
+print(d1) #  {'hello': 'world'}
 ```
 
 #### [`UnderscoreAccessDict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.mapping.UnderscoreAccessDict)
 
 Dictionary that does not distinct between spaces and underscores.
 
 ```python
 from toolbox import UnderscoreAccessDict
 
 d = UnderscoreAccessDict({"hello world": "ola mundo"})
-d['hello_world'] # >>> 'ola mundo'
+d['hello_world'] #  'ola mundo'
 ```
 
 #### [`FrozenDict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.mapping.FrozenDict)
 
 Dictionary that is frozen.
 
 ```python
 from toolbox import FrozenDict
 
 d = FrozenDict({"hello": "world"})
 d['ola'] = 'mundo'
-# >>> KeyError: 'Cannot set key and value because this is a frozen dictionary.'
+#  KeyError: 'Cannot set key and value because this is a frozen dictionary.'
 ```
 
 #### [`ItemDict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.mapping.ItemDict)
 
 Dictionary that utilizes [`Item`](#Item) for key and values.
 
 ```python
 from toolbox import ItemDict, Item
 
 d = ItemDict({"100": "one hundred"})
-print(d[100])                                          # >>> one hundred
-print(d[100] == d['100'] == d[b'100'] == d[Item(100)]) # >>> True
+print(d[100])                                          #  one hundred
+print(d[100] == d['100'] == d[b'100'] == d[Item(100)]) #  True
 ```
 
 All `*Dict` types above can be combined together (as mixins) to create unique dictionary types. Example:
 
 ```python
 from toolbox import ObjectDict, UnderscoreAccessDict
 
 class Dict(ObjectDict, UnderscoreAccessDict):
     """ New dictionary that allows object access with underscore access. """
 
 d = Dict({"hello world": "ola mundo", "100": "one hundred"})
-print(d.hello_world)    # >>> ola mundo
-print(d._100)           # >>> one hundred
+print(d.hello_world)    #  ola mundo
+print(d._100)           #  one hundred
 ```
 
 #### [`nestednamedtuple`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.namedtuple.nestednamedtuple)
 
 Creates a nested `namedtuple` for easy object access.
 
 ```python
 from toolbox import nestednamedtuple
 
 nt = nestednamedtuple({"hello": {"ola": "mundo"}})
-print(nt)           # >>> namedtupled(hello=namedtupled(ola='mundo'))
-print(nt.hello.ola) # >>> mundo
+print(nt)           #  namedtupled(hello=namedtupled(ola='mundo'))
+print(nt.hello.ola) #  mundo
 ```
 
 #### [`fdict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.namedtuple.fdict)
 
 Forces `nestednamedtuple` to not convert `dict` to `namedtuple`. 
 
 ```python
 from toolbox import nestednamedtuple
 
 d = {"hello": "world"}
 nt = nestednamedtuple({"forced": fdict(d), "notforced": d})
 
-print(nt.notforced) # >>> namedtupled(hello='world')
-print(nt.forced)    # >>> {'hello': 'world'}
+print(nt.notforced) #  namedtupled(hello='world')
+print(nt.forced)    #  {'hello': 'world'}
 ```
 
 ### `config`
 
 #### [`make_config`](https://synchronizing.github.io/toolbox/module/config.html#toolbox.config.globalconfig.make_config)
 
 Creates a global configuration that can be accessed by other portions of the code via `conf` or `config` function calls. Minimizes the need to create `Config` objects and pass them around different modules, classes, functions, etc.
@@ -316,157 +330,157 @@
 #### [`conf`](https://synchronizing.github.io/toolbox/module/config.html#toolbox.config.globalconfig.conf)
 
 Access global configuration as a `nestednamedtuple`.
 
 ```python
 from toolbox import conf
 
-print(conf().hello) # >>> 'world'
+print(conf().hello) #  'world'
 ```
 
 #### [`config`](https://synchronizing.github.io/toolbox/module/config.html#toolbox.config.globalconfig.config)
 
 Access global configuration as a dictionary.
 
 ```python
 from toolbox import config
 
-print(config()['hello']) # >>> 'world'
+print(config()['hello']) #  'world'
 ```
 
 ### `functools`
 
 #### [`timeout`](https://synchronizing.github.io/toolbox/module/functools.html#toolbox.functools.timeout.timeout)
 
 Decorator that adds support for synchronous and asynchronous function timeout. Quits function after an amount of time passes.
 
 ```python
 from toolbox import timeout
+import asyncio
+import time
 
-@timeout(seconds=5)
+@timeout(seconds=1)
 def func():
-    time.wait(15)
+    time.sleep(15)
 
-func()
+@timeout(seconds=1)
+async def func():
+    await asyncio.sleep(15)
 ```
 
 ### `pkgutil`
 
 #### [`search_package`](https://synchronizing.github.io/toolbox/module/pkgutil.html#toolbox.pkgutil.package.search_package)
 
 Searches for packages installed in the system.
 
 ```python
 from toolbox import search_package
 
 print(search_package("toolbox", method="is"))
-# >>> {'toolbox': <module 'toolbox' from '.../toolbox/__init__.py'>}
+#  {'toolbox': <module 'toolbox' from '.../toolbox/__init__.py'>}
 ```
 
-### `experimental`
-
-All tools marked as experimental are not meant to be used in production.
-
-#### [`asyncdispatch`](https://synchronizing.github.io/toolbox/module/experimental.html#toolbox.experimental.asyncdispatch.asyncdispatch)
+### `sockets`
 
-Decorator for adding dispatch functionality between async and sync functions. Allows calling the same function name, one as a normal function and one as an awaitable, yet receive different results.
+#### [`is_ip`](https://synchronizing.github.io/toolbox/module/sockets.html#toolbox.sockets.ip.is_ip)
+ 
+Checks if a string is an IP address.
 
 ```python
-from toolbox import asyncdispatch
-import asyncio
-
-@asyncdispatch
-def func():
-    return "sync"
-
-@func.register
-async def _():
-    return "async"
-
-async def main():
-    print(func())          # >>> sync
-    print(await func())    # >>> async
+from toolbox import is_ip
 
-asyncio.run(main())
+print(is_ip('127.0.0.1')) # True
+print(is_ip('localhost'))  # False
 ```
 
 ### `string`
 
-Comes out of the box with built-in ANSI formats that allows text style modification.
+#### ANSI Formatting
 
 ```python
 from toolbox import bold, red
 
 print(red("This text is red!"))
 print(bold("This text is bolded!"))
 ```
 
 Check documentation [here](https://synchronizing.github.io/toolbox/module/string.html#color) for further information on all built-in formats.
 
-#### [`Format`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.Format)
+##### [`Format`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.Format)
 
-Persistent ANSI format container that allows custom ANSI code.
+Persistent ANSI formatter that takes a custom ANSI code.
 
 ```python
 from toolbox import Format
 
 bold = Format(code=1)
 print(bold("hello world"))
 ```
 
-#### [`Style`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.Style)
+##### [`Style`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.Style)
 
-Persistent ANSI format container that allows multiple ANSI codes.
+Persistent ANSI formatter that allows multiple ANSI codes.
 
 ```python
 from toolbox import Style, red, bold
 
 error = Style(red, bold)
 print(error("This is red & bolded error."))
 ```
 
-#### [`supports_color`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.supports_color)
+##### [`supports_color`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.supports_color)
 
-Returns bool that indicates whether or not the user's terminal supports color.
+Check's whether user's terminal supports color.
 
 ```python
 from toolbox import supports_color
 
 print(supports_color())
 ```
 
-#### [`strip_ansi`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.strip_ansi)
+##### [`strip_ansi`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.strip_ansi)
 
 Removes ANSI codes from string.
 
 ```python
 from toolbox import strip_ansi
 
-print(strip_ansi("\x1b[1mhello world\x1b[0m")) # >>> hello world
+print(strip_ansi("\x1b[1mhello world\x1b[0m")) #  hello world
 ```
 
 ### `textwrap`
 
 #### [`unindent`](https://synchronizing.github.io/toolbox/module/textwrap.html#toolbox.textwrap.text.unindent)
 
-Unident triple quotes and removes any white spaces before or after text.
+Unindent triple quotes and removes any white spaces before or after text.
 
 ```python
-from toolbox import unident
+from toolbox import unindent
+
 
 def test():
-    return unindent(
-        '''
+    text = """
+           hello world
+           this is a test
+           """
+    print(text)
+
+    text = unindent(
+        """
         hello world
         this is a test
-        of this functionality
-        '''
+        """
     )
+    print(text)
+
 
-print(test()) 
-# >>> hello world
-# >>> this is a test
-# >>> of this functionality
+test()
+#           hello world
+#           this is a test
+#
+# hello world
+# this is a test
 ```
```

### Comparing `toolbox-1.8.1/README.md` & `toolbox-1.9.0/toolbox.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: toolbox
+Version: 1.9.0
+Summary: Extends Python with useful features.
+Home-page: https://github.com/synchronizing/toolbox
+Author: Felipe Faria
+Author-email: felipefaria@hey.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/synchronizing/toolbox/issues
+Project-URL: Documentation, https://synchronizing.github.io/toolbox/
+Project-URL: Source Code, https://github.com/synchronizing/toolbox/tree/master
+Keywords: toolbox,asyncio,builtins,collections,config,functools,textwrap
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE
+License-File: AUTHORS
+
 # 🧰 Toolbox
 
 <p align="center">
 
   <a href="https://github.com/synchronizing/toolbox/actions?query=workflow%3ABuild">
     <img src="https://github.com/synchronizing/toolbox/workflows/Build/badge.svg?branch=master&event=push">
   </a>
@@ -29,21 +53,19 @@
 
 ## Documentation
 
 Documentation can be found [**here**](http://synchronizing.github.io/toolbox/).
 
 ## Using
 
-Toolbox follows the same pattern as of the Python Standard Library (PSL) which means that all tools are found inside package names that corresponds to that of the PSL (e.g. `asyncio`, `collections`, etc.) with only one exception (`config`). Check out documentation for function definitions and more details.
-
 ### `asyncio`
 
 #### [`async to_thread`](https://synchronizing.github.io/toolbox/module/asyncio.html#toolbox.asyncio.threads.to_thread)
 
-Runs passed function in a new thread to ensure non-blocking IO during asynchronous programming.
+Runs given function in a new thread during asynchronous IO.
 
 ```python
 from toolbox import to_thread
 import asyncio
 import time
 
 def func():
@@ -91,50 +113,66 @@
     # Communication is now encrypted.
 
 asyncio.run(client())
 ```
 
 #### [`CoroutineClass`](https://synchronizing.github.io/toolbox/module/asyncio.html#toolbox.asyncio.pattern.CoroutineClass)
 
-Useful pattern to add non-blocking start/stop functions and an async context manager to a class.
+Pattern for creating a coroutine-like class that has multiple ways to start it.
 
 ```python
 from toolbox import CoroutineClass
 import asyncio
 
 class Coroutine(CoroutineClass):
     def __init__(self, run: bool = False):
         super().__init__(run=run)
 
+    # Default entry function.
     async def entry(self):
-        # Default entry function.
-        # Some async functionality here.
+        await asyncio.sleep(1)
+        return "Hello world"
 
-async def main():
+# Start coroutine outside Python async context.
+def iomain():
 
-    # Use with __init__ start.
-    process = AsyncClass(start=True)
-    await asyncio.sleep(1)
-    process.stop()
+    # via __init__
+    coro = Coroutine(run=True)
+    print(coro.result)  # Hello world
+
+    # via .run()
+    coro = Coroutine()
+    result = coro.run()
+    print(result)  # Hello world
+
+# Start coroutine inside Python async context.
+async def aiomain():
 
-    # Use with functions to start/stop.
-    process = AsyncClass()
-    process.start()
+    # via __init__
+    coro = Coroutine(run=True)
     await asyncio.sleep(1)
-    process.stop()
+    coro.stop()
+    print(coro.result)  # None - because process was stopped before completion.
 
-    # Use with context manager to start/stop.
-    async with AsyncClass() as process:
-        ...
-
-    # Use it with await.
-    process = AsyncClass()
-    await process
+    # via .run()
+    coro = Coroutine()
+    coro.run()
+    await asyncio.sleep(1)
+    result = coro.stop()  # None - because coroutine was stopped before completion.
+    print(result)  # Hello world
 
-asyncio.run(main())
+    # via await
+    coro = Coroutine()
+    result = await coro  # You can also start, and await later.
+    print(result)  # Hello World
+
+    # via context manager
+    async with Coroutine() as coro:
+        result = await coro
+    print(result)  # Hello World
 ```
 
 ### `builtins`
 
 #### [`classproperty`](https://synchronizing.github.io/toolbox/module/builtins.html#toolbox.builtins.property.classproperty)
 
 Combines a `property` and a `classmethod` into one, creating a class property. Allows access to computed class attributes.
@@ -143,142 +181,142 @@
 from toolbox import classproperty
 
 class Animal:
     @classproperty
     def dog(cls):
         return "whoof!"
 
-print(Animal.dog) # >>> 'whoof!'
+print(Animal.dog) #  'whoof!'
 ```
 
 
 ### `collections`
 
 #### [`Item`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.item.Item)
 
 An interface for type-agnostic operations between different types.
 
 ```python
 from toolbox import Item
 
 item = Item(100)
-print(item == b"100" == "100" == 100) # >>> True
+print(item == b"100" == "100" == 100) #  True
 ```
 
 #### [`BidirectionalDict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.mapping.BidirectionalDict)
 
 Dictionary with two-way capabilities.
 
 ```python
 from toolbox import BidirectionalDict
 
 d = BidirectionalDict({"hello": "world"})
-print(d) # >>> {'hello': 'world', 'world': 'hello'}
+print(d) #  {'hello': 'world', 'world': 'hello'}
 ```
 
 #### [`ObjectDict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.mapping.ObjectDict)
 
 Dictionary that can be accessed as though it was an object.
 
 ```python
 from toolbox import ObjectDict
 
 d = ObjectDict({"hello": "world"})
-print(d.hello) # >>> 'world'
+print(d.hello) #  'world'
 ```
 
 #### [`OverloadedDict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.mapping.OverloadedDict)
 
 Dictionary that can be added or subtracted to.
 
 ```python
 from toolbox import OverloadedDict
 
 d1 = OverloadedDict({"hello": "world"})
 d2 = OverloadedDict({"ola": "mundo"})
 
 d1 += d2
-print(d1) # >>> {'hello': 'world', 'ola': 'mundo'}
+print(d1) #  {'hello': 'world', 'ola': 'mundo'}
 
 d1 -= d2
-print(d1) # >>> {'hello': 'world'}
+print(d1) #  {'hello': 'world'}
 ```
 
 #### [`UnderscoreAccessDict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.mapping.UnderscoreAccessDict)
 
 Dictionary that does not distinct between spaces and underscores.
 
 ```python
 from toolbox import UnderscoreAccessDict
 
 d = UnderscoreAccessDict({"hello world": "ola mundo"})
-d['hello_world'] # >>> 'ola mundo'
+d['hello_world'] #  'ola mundo'
 ```
 
 #### [`FrozenDict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.mapping.FrozenDict)
 
 Dictionary that is frozen.
 
 ```python
 from toolbox import FrozenDict
 
 d = FrozenDict({"hello": "world"})
 d['ola'] = 'mundo'
-# >>> KeyError: 'Cannot set key and value because this is a frozen dictionary.'
+#  KeyError: 'Cannot set key and value because this is a frozen dictionary.'
 ```
 
 #### [`ItemDict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.mapping.ItemDict)
 
 Dictionary that utilizes [`Item`](#Item) for key and values.
 
 ```python
 from toolbox import ItemDict, Item
 
 d = ItemDict({"100": "one hundred"})
-print(d[100])                                          # >>> one hundred
-print(d[100] == d['100'] == d[b'100'] == d[Item(100)]) # >>> True
+print(d[100])                                          #  one hundred
+print(d[100] == d['100'] == d[b'100'] == d[Item(100)]) #  True
 ```
 
 All `*Dict` types above can be combined together (as mixins) to create unique dictionary types. Example:
 
 ```python
 from toolbox import ObjectDict, UnderscoreAccessDict
 
 class Dict(ObjectDict, UnderscoreAccessDict):
     """ New dictionary that allows object access with underscore access. """
 
 d = Dict({"hello world": "ola mundo", "100": "one hundred"})
-print(d.hello_world)    # >>> ola mundo
-print(d._100)           # >>> one hundred
+print(d.hello_world)    #  ola mundo
+print(d._100)           #  one hundred
 ```
 
 #### [`nestednamedtuple`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.namedtuple.nestednamedtuple)
 
 Creates a nested `namedtuple` for easy object access.
 
 ```python
 from toolbox import nestednamedtuple
 
 nt = nestednamedtuple({"hello": {"ola": "mundo"}})
-print(nt)           # >>> namedtupled(hello=namedtupled(ola='mundo'))
-print(nt.hello.ola) # >>> mundo
+print(nt)           #  namedtupled(hello=namedtupled(ola='mundo'))
+print(nt.hello.ola) #  mundo
 ```
 
 #### [`fdict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.namedtuple.fdict)
 
 Forces `nestednamedtuple` to not convert `dict` to `namedtuple`. 
 
 ```python
 from toolbox import nestednamedtuple
 
 d = {"hello": "world"}
 nt = nestednamedtuple({"forced": fdict(d), "notforced": d})
 
-print(nt.notforced) # >>> namedtupled(hello='world')
-print(nt.forced)    # >>> {'hello': 'world'}
+print(nt.notforced) #  namedtupled(hello='world')
+print(nt.forced)    #  {'hello': 'world'}
 ```
 
 ### `config`
 
 #### [`make_config`](https://synchronizing.github.io/toolbox/module/config.html#toolbox.config.globalconfig.make_config)
 
 Creates a global configuration that can be accessed by other portions of the code via `conf` or `config` function calls. Minimizes the need to create `Config` objects and pass them around different modules, classes, functions, etc.
@@ -292,154 +330,157 @@
 #### [`conf`](https://synchronizing.github.io/toolbox/module/config.html#toolbox.config.globalconfig.conf)
 
 Access global configuration as a `nestednamedtuple`.
 
 ```python
 from toolbox import conf
 
-print(conf().hello) # >>> 'world'
+print(conf().hello) #  'world'
 ```
 
 #### [`config`](https://synchronizing.github.io/toolbox/module/config.html#toolbox.config.globalconfig.config)
 
 Access global configuration as a dictionary.
 
 ```python
 from toolbox import config
 
-print(config()['hello']) # >>> 'world'
+print(config()['hello']) #  'world'
 ```
 
 ### `functools`
 
 #### [`timeout`](https://synchronizing.github.io/toolbox/module/functools.html#toolbox.functools.timeout.timeout)
 
 Decorator that adds support for synchronous and asynchronous function timeout. Quits function after an amount of time passes.
 
 ```python
 from toolbox import timeout
+import asyncio
+import time
 
-@timeout(seconds=5)
+@timeout(seconds=1)
 def func():
-    time.wait(15)
+    time.sleep(15)
 
-func()
+@timeout(seconds=1)
+async def func():
+    await asyncio.sleep(15)
 ```
 
 ### `pkgutil`
 
 #### [`search_package`](https://synchronizing.github.io/toolbox/module/pkgutil.html#toolbox.pkgutil.package.search_package)
 
 Searches for packages installed in the system.
 
 ```python
 from toolbox import search_package
 
 print(search_package("toolbox", method="is"))
-# >>> {'toolbox': <module 'toolbox' from '.../toolbox/__init__.py'>}
+#  {'toolbox': <module 'toolbox' from '.../toolbox/__init__.py'>}
 ```
 
-### `experimental`
+### `sockets`
 
-All tools marked as experimental are not meant to be used in production.
-
-#### [`asyncdispatch`](https://synchronizing.github.io/toolbox/module/experimental.html#toolbox.experimental.asyncdispatch.asyncdispatch)
-
-Decorator for adding dispatch functionality between async and sync functions. Allows calling the same function name, one as a normal function and one as an awaitable, yet receive different results.
+#### [`is_ip`](https://synchronizing.github.io/toolbox/module/sockets.html#toolbox.sockets.ip.is_ip)
+ 
+Checks if a string is an IP address.
 
 ```python
-from toolbox import asyncdispatch
-import asyncio
+from toolbox import is_ip
 
-@asyncdispatch
-def func():
-    return "sync"
-
-@func.register
-async def _():
-    return "async"
-
-async def main():
-    print(func())          # >>> sync
-    print(await func())    # >>> async
-
-asyncio.run(main())
+print(is_ip('127.0.0.1')) # True
+print(is_ip('localhost'))  # False
 ```
 
 ### `string`
 
-Comes out of the box with built-in ANSI formats that allows text style modification.
+#### ANSI Formatting
 
 ```python
 from toolbox import bold, red
 
 print(red("This text is red!"))
 print(bold("This text is bolded!"))
 ```
 
 Check documentation [here](https://synchronizing.github.io/toolbox/module/string.html#color) for further information on all built-in formats.
 
-#### [`Format`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.Format)
+##### [`Format`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.Format)
 
-Persistent ANSI format container that allows custom ANSI code.
+Persistent ANSI formatter that takes a custom ANSI code.
 
 ```python
 from toolbox import Format
 
 bold = Format(code=1)
 print(bold("hello world"))
 ```
 
-#### [`Style`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.Style)
+##### [`Style`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.Style)
 
-Persistent ANSI format container that allows multiple ANSI codes.
+Persistent ANSI formatter that allows multiple ANSI codes.
 
 ```python
 from toolbox import Style, red, bold
 
 error = Style(red, bold)
 print(error("This is red & bolded error."))
 ```
 
-#### [`supports_color`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.supports_color)
+##### [`supports_color`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.supports_color)
 
-Returns bool that indicates whether or not the user's terminal supports color.
+Check's whether user's terminal supports color.
 
 ```python
 from toolbox import supports_color
 
 print(supports_color())
 ```
 
-#### [`strip_ansi`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.strip_ansi)
+##### [`strip_ansi`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.strip_ansi)
 
 Removes ANSI codes from string.
 
 ```python
 from toolbox import strip_ansi
 
-print(strip_ansi("\x1b[1mhello world\x1b[0m")) # >>> hello world
+print(strip_ansi("\x1b[1mhello world\x1b[0m")) #  hello world
 ```
 
 ### `textwrap`
 
 #### [`unindent`](https://synchronizing.github.io/toolbox/module/textwrap.html#toolbox.textwrap.text.unindent)
 
-Unident triple quotes and removes any white spaces before or after text.
+Unindent triple quotes and removes any white spaces before or after text.
 
 ```python
-from toolbox import unident
+from toolbox import unindent
+
 
 def test():
-    return unindent(
-        '''
+    text = """
+           hello world
+           this is a test
+           """
+    print(text)
+
+    text = unindent(
+        """
         hello world
         this is a test
-        of this functionality
-        '''
+        """
     )
+    print(text)
+
 
-print(test()) 
-# >>> hello world
-# >>> this is a test
-# >>> of this functionality
+test()
+#           hello world
+#           this is a test
+#
+# hello world
+# this is a test
 ```
+
+
+
```

### Comparing `toolbox-1.8.1/docs/Makefile` & `toolbox-1.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/docs/make.bat` & `toolbox-1.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/docs/source/conf.py` & `toolbox-1.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/docs/source/module/asyncio.rst` & `toolbox-1.9.0/docs/source/module/asyncio.rst`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/docs/source/module/collections.rst` & `toolbox-1.9.0/docs/source/module/collections.rst`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/docs/source/module/experimental.rst` & `toolbox-1.9.0/docs/source/module/experimental.rst`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/docs/source/module/string.rst` & `toolbox-1.9.0/docs/source/module/string.rst`

 * *Files 9% similar despite different names*

```diff
@@ -6,57 +6,57 @@
 color
 *****
 
 .. code-block:: python
 
     from toolbox.string import color
 
-Out-of-the-box this module includes the following :class:`toolbox.string.color.Format` definitions:
+.. autoclass:: toolbox.string.color.Format
 
-.. list-table:: 
-    :header-rows: 1
+    Out-of-the-box this module includes the following :class:`toolbox.string.color.Format` definitions:
 
-    *   - Foreground Color
-        - Background Color
-        - Styles
-    *   - :py:class:`black`
-        - :py:class:`bblack`
-        - :py:class:`reset`
-    *   - :py:class:`red`
-        - :py:class:`bred`
-        - :py:class:`bold`
-    *   - :py:class:`green`
-        - :py:class:`bgreen`
-        - :py:class:`underline`
-    *   - :py:class:`yellow`
-        - :py:class:`byellow`
-        - :py:class:`blink`
-    *   - :py:class:`blue`
-        - :py:class:`bblue`
-        - :py:class:`reverse`
-    *   - :py:class:`magenta`
-        - :py:class:`bmagenta`
-        - :py:class:`conceal`
-    *   - :py:class:`cyan`
-        - :py:class:`bcyan`
-        - 
-    *   - :py:class:`white`
-        - :py:class:`bwhite`
-        - 
+    .. list-table:: 
+        :header-rows: 1
 
+        *   - Foreground Color
+            - Background Color
+            - Styles
+        *   - :py:class:`black`
+            - :py:class:`bblack`
+            - :py:class:`reset`
+        *   - :py:class:`red`
+            - :py:class:`bred`
+            - :py:class:`bold`
+        *   - :py:class:`green`
+            - :py:class:`bgreen`
+            - :py:class:`underline`
+        *   - :py:class:`yellow`
+            - :py:class:`byellow`
+            - :py:class:`blink`
+        *   - :py:class:`blue`
+            - :py:class:`bblue`
+            - :py:class:`reverse`
+        *   - :py:class:`magenta`
+            - :py:class:`bmagenta`
+            - :py:class:`conceal`
+        *   - :py:class:`cyan`
+            - :py:class:`bcyan`
+            - 
+        *   - :py:class:`white`
+            - :py:class:`bwhite`
+            - 
 
-These can be utilized like so:
 
-.. code-block:: python
+    These can be utilized like so:
 
-    from toolbox.string.color import bold
+    .. code-block:: python
 
-    print(bold("Hello world!"))
+        from toolbox.string.color import bold
 
-.. autoclass:: toolbox.string.color.Format
+        print(bold("Hello world!"))
 
 .. autoclass:: toolbox.string.color.Style
 
 .. autofunction:: toolbox.string.color.supports_color
 
 .. autofunction:: toolbox.string.color.strip_ansi
```

### Comparing `toolbox-1.8.1/setup.cfg` & `toolbox-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/tests/test_asyncio.py` & `toolbox-1.9.0/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/tests/test_collections.py` & `toolbox-1.9.0/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/tests/test_functools.py` & `toolbox-1.9.0/tests/test_functools.py`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/tests/test_string.py` & `toolbox-1.9.0/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/toolbox/asyncio/streams.py` & `toolbox-1.9.0/toolbox/asyncio/streams.py`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/toolbox/asyncio/threads.py` & `toolbox-1.9.0/toolbox/asyncio/threads.py`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/toolbox/builtins/property.py` & `toolbox-1.9.0/toolbox/builtins/property.py`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/toolbox/collections/item.py` & `toolbox-1.9.0/toolbox/collections/item.py`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/toolbox/collections/mapping.py` & `toolbox-1.9.0/toolbox/collections/mapping.py`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/toolbox/collections/namedtuple.py` & `toolbox-1.9.0/toolbox/collections/namedtuple.py`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/toolbox/config/globalconfig.py` & `toolbox-1.9.0/toolbox/config/globalconfig.py`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/toolbox/functools/timeout.py` & `toolbox-1.9.0/toolbox/functools/timeout.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,42 +39,50 @@
             func()
     """
 
     td = datetime.timedelta(days=days, hours=hours, minutes=minutes, seconds=seconds)
     total_seconds = int(td.total_seconds())
 
     def wrapper(func: Union[Callable, Awaitable]):
+        """
+        Wraps async or sync function with timeout functionality.
+        """
+
         @functools.wraps(func)
         async def async_wrapper(*args, **kwargs):
+            """
+            Leverages the asyncio.wait_for() function to wait for a given amount of time.
+            """
+
             try:
                 return await asyncio.wait_for(func(*args, **kwargs), total_seconds)
             except asyncio.TimeoutError as err:
                 if error:
                     raise TimeoutError(
                         "Function {} timed out.".format(func.__name__)
                     ) from err
-                else:
-                    return None
 
         @functools.wraps(func)
         def sync_wrapper(*args, **kwargs):
+            """
+            Leverages the signal.alarm() function to wait for a given amount of time.
+            """
+
             def _handle_timeout(signum, frame):
                 raise TimeoutError
 
             signal.signal(signal.SIGALRM, _handle_timeout)
             signal.alarm(total_seconds)
             try:
                 return func(*args, **kwargs)
             except TimeoutError as err:
                 if error:
                     raise TimeoutError(
                         "Function {} timed out.".format(func.__name__)
                     ) from err
-                else:
-                    return None
 
         if inspect.iscoroutinefunction(func):
             return async_wrapper
         else:
             return sync_wrapper
 
     return wrapper
```

### Comparing `toolbox-1.8.1/toolbox/pkgutil/package.py` & `toolbox-1.9.0/toolbox/pkgutil/package.py`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/toolbox/string/color.py` & `toolbox-1.9.0/toolbox/string/color.py`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/toolbox/textwrap/text.py` & `toolbox-1.9.0/toolbox/textwrap/text.py`

 * *Files identical despite different names*

### Comparing `toolbox-1.8.1/toolbox.egg-info/PKG-INFO` & `toolbox-1.9.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: toolbox
-Version: 1.8.1
-Summary: Extends Python with useful features.
-Home-page: https://github.com/synchronizing/toolbox
-Author: Felipe Faria
-Author-email: felipefaria@hey.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/synchronizing/toolbox/issues
-Project-URL: Documentation, https://synchronizing.github.io/toolbox/
-Project-URL: Source Code, https://github.com/synchronizing/toolbox/tree/master
-Keywords: toolbox,asyncio,builtins,collections,config,functools,textwrap
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8
-License-File: LICENSE
-License-File: AUTHORS
-
 # 🧰 Toolbox
 
 <p align="center">
 
   <a href="https://github.com/synchronizing/toolbox/actions?query=workflow%3ABuild">
     <img src="https://github.com/synchronizing/toolbox/workflows/Build/badge.svg?branch=master&event=push">
   </a>
@@ -53,21 +29,19 @@
 
 ## Documentation
 
 Documentation can be found [**here**](http://synchronizing.github.io/toolbox/).
 
 ## Using
 
-Toolbox follows the same pattern as of the Python Standard Library (PSL) which means that all tools are found inside package names that corresponds to that of the PSL (e.g. `asyncio`, `collections`, etc.) with only one exception (`config`). Check out documentation for function definitions and more details.
-
 ### `asyncio`
 
 #### [`async to_thread`](https://synchronizing.github.io/toolbox/module/asyncio.html#toolbox.asyncio.threads.to_thread)
 
-Runs passed function in a new thread to ensure non-blocking IO during asynchronous programming.
+Runs given function in a new thread during asynchronous IO.
 
 ```python
 from toolbox import to_thread
 import asyncio
 import time
 
 def func():
@@ -115,50 +89,66 @@
     # Communication is now encrypted.
 
 asyncio.run(client())
 ```
 
 #### [`CoroutineClass`](https://synchronizing.github.io/toolbox/module/asyncio.html#toolbox.asyncio.pattern.CoroutineClass)
 
-Useful pattern to add non-blocking start/stop functions and an async context manager to a class.
+Pattern for creating a coroutine-like class that has multiple ways to start it.
 
 ```python
 from toolbox import CoroutineClass
 import asyncio
 
 class Coroutine(CoroutineClass):
     def __init__(self, run: bool = False):
         super().__init__(run=run)
 
+    # Default entry function.
     async def entry(self):
-        # Default entry function.
-        # Some async functionality here.
+        await asyncio.sleep(1)
+        return "Hello world"
 
-async def main():
+# Start coroutine outside Python async context.
+def iomain():
 
-    # Use with __init__ start.
-    process = AsyncClass(start=True)
-    await asyncio.sleep(1)
-    process.stop()
+    # via __init__
+    coro = Coroutine(run=True)
+    print(coro.result)  # Hello world
+
+    # via .run()
+    coro = Coroutine()
+    result = coro.run()
+    print(result)  # Hello world
+
+# Start coroutine inside Python async context.
+async def aiomain():
 
-    # Use with functions to start/stop.
-    process = AsyncClass()
-    process.start()
+    # via __init__
+    coro = Coroutine(run=True)
     await asyncio.sleep(1)
-    process.stop()
+    coro.stop()
+    print(coro.result)  # None - because process was stopped before completion.
 
-    # Use with context manager to start/stop.
-    async with AsyncClass() as process:
-        ...
-
-    # Use it with await.
-    process = AsyncClass()
-    await process
+    # via .run()
+    coro = Coroutine()
+    coro.run()
+    await asyncio.sleep(1)
+    result = coro.stop()  # None - because coroutine was stopped before completion.
+    print(result)  # Hello world
 
-asyncio.run(main())
+    # via await
+    coro = Coroutine()
+    result = await coro  # You can also start, and await later.
+    print(result)  # Hello World
+
+    # via context manager
+    async with Coroutine() as coro:
+        result = await coro
+    print(result)  # Hello World
 ```
 
 ### `builtins`
 
 #### [`classproperty`](https://synchronizing.github.io/toolbox/module/builtins.html#toolbox.builtins.property.classproperty)
 
 Combines a `property` and a `classmethod` into one, creating a class property. Allows access to computed class attributes.
@@ -167,142 +157,142 @@
 from toolbox import classproperty
 
 class Animal:
     @classproperty
     def dog(cls):
         return "whoof!"
 
-print(Animal.dog) # >>> 'whoof!'
+print(Animal.dog) #  'whoof!'
 ```
 
 
 ### `collections`
 
 #### [`Item`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.item.Item)
 
 An interface for type-agnostic operations between different types.
 
 ```python
 from toolbox import Item
 
 item = Item(100)
-print(item == b"100" == "100" == 100) # >>> True
+print(item == b"100" == "100" == 100) #  True
 ```
 
 #### [`BidirectionalDict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.mapping.BidirectionalDict)
 
 Dictionary with two-way capabilities.
 
 ```python
 from toolbox import BidirectionalDict
 
 d = BidirectionalDict({"hello": "world"})
-print(d) # >>> {'hello': 'world', 'world': 'hello'}
+print(d) #  {'hello': 'world', 'world': 'hello'}
 ```
 
 #### [`ObjectDict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.mapping.ObjectDict)
 
 Dictionary that can be accessed as though it was an object.
 
 ```python
 from toolbox import ObjectDict
 
 d = ObjectDict({"hello": "world"})
-print(d.hello) # >>> 'world'
+print(d.hello) #  'world'
 ```
 
 #### [`OverloadedDict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.mapping.OverloadedDict)
 
 Dictionary that can be added or subtracted to.
 
 ```python
 from toolbox import OverloadedDict
 
 d1 = OverloadedDict({"hello": "world"})
 d2 = OverloadedDict({"ola": "mundo"})
 
 d1 += d2
-print(d1) # >>> {'hello': 'world', 'ola': 'mundo'}
+print(d1) #  {'hello': 'world', 'ola': 'mundo'}
 
 d1 -= d2
-print(d1) # >>> {'hello': 'world'}
+print(d1) #  {'hello': 'world'}
 ```
 
 #### [`UnderscoreAccessDict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.mapping.UnderscoreAccessDict)
 
 Dictionary that does not distinct between spaces and underscores.
 
 ```python
 from toolbox import UnderscoreAccessDict
 
 d = UnderscoreAccessDict({"hello world": "ola mundo"})
-d['hello_world'] # >>> 'ola mundo'
+d['hello_world'] #  'ola mundo'
 ```
 
 #### [`FrozenDict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.mapping.FrozenDict)
 
 Dictionary that is frozen.
 
 ```python
 from toolbox import FrozenDict
 
 d = FrozenDict({"hello": "world"})
 d['ola'] = 'mundo'
-# >>> KeyError: 'Cannot set key and value because this is a frozen dictionary.'
+#  KeyError: 'Cannot set key and value because this is a frozen dictionary.'
 ```
 
 #### [`ItemDict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.mapping.ItemDict)
 
 Dictionary that utilizes [`Item`](#Item) for key and values.
 
 ```python
 from toolbox import ItemDict, Item
 
 d = ItemDict({"100": "one hundred"})
-print(d[100])                                          # >>> one hundred
-print(d[100] == d['100'] == d[b'100'] == d[Item(100)]) # >>> True
+print(d[100])                                          #  one hundred
+print(d[100] == d['100'] == d[b'100'] == d[Item(100)]) #  True
 ```
 
 All `*Dict` types above can be combined together (as mixins) to create unique dictionary types. Example:
 
 ```python
 from toolbox import ObjectDict, UnderscoreAccessDict
 
 class Dict(ObjectDict, UnderscoreAccessDict):
     """ New dictionary that allows object access with underscore access. """
 
 d = Dict({"hello world": "ola mundo", "100": "one hundred"})
-print(d.hello_world)    # >>> ola mundo
-print(d._100)           # >>> one hundred
+print(d.hello_world)    #  ola mundo
+print(d._100)           #  one hundred
 ```
 
 #### [`nestednamedtuple`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.namedtuple.nestednamedtuple)
 
 Creates a nested `namedtuple` for easy object access.
 
 ```python
 from toolbox import nestednamedtuple
 
 nt = nestednamedtuple({"hello": {"ola": "mundo"}})
-print(nt)           # >>> namedtupled(hello=namedtupled(ola='mundo'))
-print(nt.hello.ola) # >>> mundo
+print(nt)           #  namedtupled(hello=namedtupled(ola='mundo'))
+print(nt.hello.ola) #  mundo
 ```
 
 #### [`fdict`](https://synchronizing.github.io/toolbox/module/collections.html#toolbox.collections.namedtuple.fdict)
 
 Forces `nestednamedtuple` to not convert `dict` to `namedtuple`. 
 
 ```python
 from toolbox import nestednamedtuple
 
 d = {"hello": "world"}
 nt = nestednamedtuple({"forced": fdict(d), "notforced": d})
 
-print(nt.notforced) # >>> namedtupled(hello='world')
-print(nt.forced)    # >>> {'hello': 'world'}
+print(nt.notforced) #  namedtupled(hello='world')
+print(nt.forced)    #  {'hello': 'world'}
 ```
 
 ### `config`
 
 #### [`make_config`](https://synchronizing.github.io/toolbox/module/config.html#toolbox.config.globalconfig.make_config)
 
 Creates a global configuration that can be accessed by other portions of the code via `conf` or `config` function calls. Minimizes the need to create `Config` objects and pass them around different modules, classes, functions, etc.
@@ -316,157 +306,154 @@
 #### [`conf`](https://synchronizing.github.io/toolbox/module/config.html#toolbox.config.globalconfig.conf)
 
 Access global configuration as a `nestednamedtuple`.
 
 ```python
 from toolbox import conf
 
-print(conf().hello) # >>> 'world'
+print(conf().hello) #  'world'
 ```
 
 #### [`config`](https://synchronizing.github.io/toolbox/module/config.html#toolbox.config.globalconfig.config)
 
 Access global configuration as a dictionary.
 
 ```python
 from toolbox import config
 
-print(config()['hello']) # >>> 'world'
+print(config()['hello']) #  'world'
 ```
 
 ### `functools`
 
 #### [`timeout`](https://synchronizing.github.io/toolbox/module/functools.html#toolbox.functools.timeout.timeout)
 
 Decorator that adds support for synchronous and asynchronous function timeout. Quits function after an amount of time passes.
 
 ```python
 from toolbox import timeout
+import asyncio
+import time
 
-@timeout(seconds=5)
+@timeout(seconds=1)
 def func():
-    time.wait(15)
+    time.sleep(15)
 
-func()
+@timeout(seconds=1)
+async def func():
+    await asyncio.sleep(15)
 ```
 
 ### `pkgutil`
 
 #### [`search_package`](https://synchronizing.github.io/toolbox/module/pkgutil.html#toolbox.pkgutil.package.search_package)
 
 Searches for packages installed in the system.
 
 ```python
 from toolbox import search_package
 
 print(search_package("toolbox", method="is"))
-# >>> {'toolbox': <module 'toolbox' from '.../toolbox/__init__.py'>}
+#  {'toolbox': <module 'toolbox' from '.../toolbox/__init__.py'>}
 ```
 
-### `experimental`
+### `sockets`
 
-All tools marked as experimental are not meant to be used in production.
-
-#### [`asyncdispatch`](https://synchronizing.github.io/toolbox/module/experimental.html#toolbox.experimental.asyncdispatch.asyncdispatch)
-
-Decorator for adding dispatch functionality between async and sync functions. Allows calling the same function name, one as a normal function and one as an awaitable, yet receive different results.
+#### [`is_ip`](https://synchronizing.github.io/toolbox/module/sockets.html#toolbox.sockets.ip.is_ip)
+ 
+Checks if a string is an IP address.
 
 ```python
-from toolbox import asyncdispatch
-import asyncio
+from toolbox import is_ip
 
-@asyncdispatch
-def func():
-    return "sync"
-
-@func.register
-async def _():
-    return "async"
-
-async def main():
-    print(func())          # >>> sync
-    print(await func())    # >>> async
-
-asyncio.run(main())
+print(is_ip('127.0.0.1')) # True
+print(is_ip('localhost'))  # False
 ```
 
 ### `string`
 
-Comes out of the box with built-in ANSI formats that allows text style modification.
+#### ANSI Formatting
 
 ```python
 from toolbox import bold, red
 
 print(red("This text is red!"))
 print(bold("This text is bolded!"))
 ```
 
 Check documentation [here](https://synchronizing.github.io/toolbox/module/string.html#color) for further information on all built-in formats.
 
-#### [`Format`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.Format)
+##### [`Format`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.Format)
 
-Persistent ANSI format container that allows custom ANSI code.
+Persistent ANSI formatter that takes a custom ANSI code.
 
 ```python
 from toolbox import Format
 
 bold = Format(code=1)
 print(bold("hello world"))
 ```
 
-#### [`Style`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.Style)
+##### [`Style`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.Style)
 
-Persistent ANSI format container that allows multiple ANSI codes.
+Persistent ANSI formatter that allows multiple ANSI codes.
 
 ```python
 from toolbox import Style, red, bold
 
 error = Style(red, bold)
 print(error("This is red & bolded error."))
 ```
 
-#### [`supports_color`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.supports_color)
+##### [`supports_color`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.supports_color)
 
-Returns bool that indicates whether or not the user's terminal supports color.
+Check's whether user's terminal supports color.
 
 ```python
 from toolbox import supports_color
 
 print(supports_color())
 ```
 
-#### [`strip_ansi`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.strip_ansi)
+##### [`strip_ansi`](https://synchronizing.github.io/toolbox/module/string.html#toolbox.string.color.strip_ansi)
 
 Removes ANSI codes from string.
 
 ```python
 from toolbox import strip_ansi
 
-print(strip_ansi("\x1b[1mhello world\x1b[0m")) # >>> hello world
+print(strip_ansi("\x1b[1mhello world\x1b[0m")) #  hello world
 ```
 
 ### `textwrap`
 
 #### [`unindent`](https://synchronizing.github.io/toolbox/module/textwrap.html#toolbox.textwrap.text.unindent)
 
-Unident triple quotes and removes any white spaces before or after text.
+Unindent triple quotes and removes any white spaces before or after text.
 
 ```python
-from toolbox import unident
+from toolbox import unindent
+
 
 def test():
-    return unindent(
-        '''
+    text = """
+           hello world
+           this is a test
+           """
+    print(text)
+
+    text = unindent(
+        """
         hello world
         this is a test
-        of this functionality
-        '''
+        """
     )
-
-print(test()) 
-# >>> hello world
-# >>> this is a test
-# >>> of this functionality
-```
-
+    print(text)
 
 
+test()
+#           hello world
+#           this is a test
+#
+# hello world
+# this is a test
+```
```

### Comparing `toolbox-1.8.1/toolbox.egg-info/SOURCES.txt` & `toolbox-1.9.0/toolbox.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,47 +18,50 @@
 docs/source/module/asyncio.rst
 docs/source/module/builtins.rst
 docs/source/module/collections.rst
 docs/source/module/config.rst
 docs/source/module/experimental.rst
 docs/source/module/functools.rst
 docs/source/module/pkgutil.rst
+docs/source/module/sockets.rst
 docs/source/module/string.rst
 docs/source/module/textwrap.rst
 tests/__init__.py
 tests/requirements.txt
 tests/test_asyncio.py
 tests/test_buildins.py
 tests/test_collections.py
 tests/test_config.py
 tests/test_functools.py
 tests/test_pkgutil.py
+tests/test_sockets.py
 tests/test_string.py
 tests/test_textwrap.py
 toolbox/__init__.py
 toolbox.egg-info/PKG-INFO
 toolbox.egg-info/SOURCES.txt
 toolbox.egg-info/dependency_links.txt
 toolbox.egg-info/not-zip-safe
+toolbox.egg-info/pbr.json
 toolbox.egg-info/top_level.txt
 toolbox/asyncio/__init__.py
 toolbox/asyncio/pattern.py
 toolbox/asyncio/streams.py
 toolbox/asyncio/threads.py
 toolbox/builtins/__init__.py
 toolbox/builtins/property.py
 toolbox/collections/__init__.py
 toolbox/collections/item.py
 toolbox/collections/mapping.py
 toolbox/collections/namedtuple.py
 toolbox/config/__init__.py
 toolbox/config/globalconfig.py
-toolbox/experimental/__init__.py
-toolbox/experimental/asyncdispatch.py
 toolbox/functools/__init__.py
 toolbox/functools/timeout.py
 toolbox/pkgutil/__init__.py
 toolbox/pkgutil/package.py
+toolbox/sockets/__init__.py
+toolbox/sockets/ip.py
 toolbox/string/__init__.py
 toolbox/string/color.py
 toolbox/textwrap/__init__.py
 toolbox/textwrap/text.py
```

