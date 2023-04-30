# Comparing `tmp/ManimPango-1.0.0a1.tar.gz` & `tmp/ManimPango-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ManimPango-1.0.0a1.tar", last modified: Sat Apr 29 17:38:49 2023, max compression
+gzip compressed data, was "ManimPango-1.0.0a2.tar", last modified: Sun Apr 30 17:51:55 2023, max compression
```

## Comparing `ManimPango-1.0.0a1.tar` & `ManimPango-1.0.0a2.tar`

### file list

```diff
@@ -1,97 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.567579 ManimPango-1.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.543579 ManimPango-1.0.0a1/ManimPango.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-04-29 17:38:49.000000 ManimPango-1.0.0a1/ManimPango.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-29 17:38:49.000000 ManimPango-1.0.0a1/ManimPango.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:38:49.000000 ManimPango-1.0.0a1/ManimPango.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:38:49.000000 ManimPango-1.0.0a1/ManimPango.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 17:38:49.000000 ManimPango-1.0.0a1/ManimPango.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-04-29 17:38:49.567579 ManimPango-1.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.547579 ManimPango-1.0.0a1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/RELEASE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.547579 ManimPango-1.0.0a1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.539579 ManimPango-1.0.0a1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.547579 ManimPango-1.0.0a1/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/building.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/integration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/news.rst
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.547579 ManimPango-1.0.0a1/manimpango/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/_distributor_init.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.547579 ManimPango-1.0.0a1/manimpango/attributes/
--rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/attributes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/cmanimpango.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/cmanimpango.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/enums.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.551579 ManimPango-1.0.0a1/manimpango/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/fonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/fonts/_font_desc.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/fonts/_font_desc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/fonts/_font_desc.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/fonts/enums.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/fonts/enums.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.551579 ManimPango-1.0.0a1/manimpango/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/include/cairo.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/include/glib.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/include/pango.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/include/pango_attributes.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.551579 ManimPango-1.0.0a1/manimpango/layout/
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/layout/_layout.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/register_font.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/register_font.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.551579 ManimPango-1.0.0a1/manimpango/renderer/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/renderer/image_renderer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/renderer/image_renderer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/renderer/image_renderer.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/renderer/svg_renderer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/renderer/svg_renderer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/renderer/svg_renderer.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.555579 ManimPango-1.0.0a1/manimpango/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/utils/_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/utils/utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-29 17:38:49.567579 ManimPango-1.0.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.555579 ManimPango-1.0.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/tests/_manim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.559579 ManimPango-1.0.0a1/tests/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   183752 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/tests/fonts/AdobeVFPrototype.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    75348 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/tests/fonts/BungeeColor-Regular_colr_Windows.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   235924 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/tests/fonts/BungeeOutline-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/tests/fonts/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  5856032 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/fonts/MaShanZheng-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/svg_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_font_desc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_fonts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_list_fonts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_valid_svg.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:51:55.444089 ManimPango-1.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:51:55.432088 ManimPango-1.0.0a2/ManimPango.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-04-30 17:51:55.000000 ManimPango-1.0.0a2/ManimPango.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-30 17:51:55.000000 ManimPango-1.0.0a2/ManimPango.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 17:51:55.000000 ManimPango-1.0.0a2/ManimPango.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 17:51:55.000000 ManimPango-1.0.0a2/ManimPango.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 17:51:55.000000 ManimPango-1.0.0a2/ManimPango.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-04-30 17:51:55.444089 ManimPango-1.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:51:55.432088 ManimPango-1.0.0a2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/docs/RELEASE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:51:55.432088 ManimPango-1.0.0a2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:51:55.432088 ManimPango-1.0.0a2/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:51:55.432088 ManimPango-1.0.0a2/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/docs/building.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/docs/integration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/docs/news.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/docs/reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:51:55.436089 ManimPango-1.0.0a2/manimpango/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/_distributor_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:51:55.436089 ManimPango-1.0.0a2/manimpango/attributes/
+-rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/attributes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/attributes/attributes.pxi
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/buffer.pxi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/cmanimpango.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/cmanimpango.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/enums.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:51:55.436089 ManimPango-1.0.0a2/manimpango/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/fonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/fonts/_font_desc.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/fonts/_font_desc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/fonts/_font_desc.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/fonts/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/fonts/enums.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:51:55.436089 ManimPango-1.0.0a2/manimpango/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/include/cairo.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/include/glib.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/include/pango.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/include/pango_attributes.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:51:55.436089 ManimPango-1.0.0a2/manimpango/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/layout/_layout.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/layout/layout.pxi
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/register_font.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/register_font.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:51:55.436089 ManimPango-1.0.0a2/manimpango/renderer/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/renderer/cairo_utils.pxi
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/renderer/image_renderer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/renderer/image_renderer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/renderer/image_renderer.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/renderer/svg_renderer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/renderer/svg_renderer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/renderer/svg_renderer.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:51:55.436089 ManimPango-1.0.0a2/manimpango/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/utils/_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/manimpango/utils/utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-30 17:51:55.444089 ManimPango-1.0.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:51:55.440089 ManimPango-1.0.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/tests/_manim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:51:55.440089 ManimPango-1.0.0a2/tests/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   183752 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/tests/fonts/AdobeVFPrototype.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    75348 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/tests/fonts/BungeeColor-Regular_colr_Windows.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   235924 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/tests/fonts/BungeeOutline-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-30 17:51:41.000000 ManimPango-1.0.0a2/tests/fonts/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  5856032 2023-04-30 17:51:42.000000 ManimPango-1.0.0a2/tests/fonts/MaShanZheng-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-04-30 17:51:42.000000 ManimPango-1.0.0a2/tests/svg_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-30 17:51:42.000000 ManimPango-1.0.0a2/tests/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-30 17:51:42.000000 ManimPango-1.0.0a2/tests/test_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-30 17:51:42.000000 ManimPango-1.0.0a2/tests/test_font_desc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-30 17:51:42.000000 ManimPango-1.0.0a2/tests/test_fonts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-30 17:51:42.000000 ManimPango-1.0.0a2/tests/test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-30 17:51:42.000000 ManimPango-1.0.0a2/tests/test_list_fonts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-30 17:51:42.000000 ManimPango-1.0.0a2/tests/test_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-30 17:51:42.000000 ManimPango-1.0.0a2/tests/test_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-30 17:51:42.000000 ManimPango-1.0.0a2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-30 17:51:42.000000 ManimPango-1.0.0a2/tests/test_valid_svg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-30 17:51:42.000000 ManimPango-1.0.0a2/tests/test_version.py
```

### Comparing `ManimPango-1.0.0a1/LICENSE` & `ManimPango-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/ManimPango.egg-info/PKG-INFO` & `ManimPango-1.0.0a2/ManimPango.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ManimPango
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Bindings for Pango for using with Manim.
 Home-page: https://manimpango.manim.community/
 Author: Naveen M K
 Author-email: naveen@manim.community
 Maintainer: The Manim Community Developers
 License: MIT
 Project-URL: Documentation, https://manimpango.manim.community/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ManimPango Version: 1.0.0a1 Summary: Bindings for
+Metadata-Version: 2.1 Name: ManimPango Version: 1.0.0a2 Summary: Bindings for
 Pango for using with Manim. Home-page: https://manimpango.manim.community/
 Author: Naveen M K Author-email: naveen@manim.community Maintainer: The Manim
 Community Developers License: MIT Project-URL: Documentation, https://
 manimpango.manim.community/ Project-URL: Source, https://github.com/
 ManimCommunity/manimpango Project-URL: Release notes, https://github.com/
 ManimCommunity/ManimPango/releases/ Description: # ManimPango
 [PyPI_Latest_Release] [PyPI_-_Wheel] [PyPI_-_Downloads] [PyPI_-_License] [PyPI
```

### Comparing `ManimPango-1.0.0a1/ManimPango.egg-info/SOURCES.txt` & `ManimPango-1.0.0a2/ManimPango.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -25,34 +25,38 @@
 docs/_static/favicon.ico
 docs/_static/logo.png
 docs/_templates/autosummary/class.rst
 docs/_templates/autosummary/module.rst
 manimpango/__init__.py
 manimpango/_distributor_init.py
 manimpango/_version.py
+manimpango/buffer.pxi
 manimpango/cmanimpango.pxd
 manimpango/cmanimpango.pyx
 manimpango/enums.pyx
 manimpango/exceptions.py
 manimpango/register_font.pxd
 manimpango/register_font.pyx
 manimpango/attributes/__init__.py
+manimpango/attributes/attributes.pxi
 manimpango/fonts/__init__.py
 manimpango/fonts/_font_desc.pxd
 manimpango/fonts/_font_desc.pyi
 manimpango/fonts/_font_desc.pyx
 manimpango/fonts/enums.pyi
 manimpango/fonts/enums.pyx
 manimpango/include/cairo.pxd
 manimpango/include/glib.pxd
 manimpango/include/pango.pxd
 manimpango/include/pango_attributes.pxd
 manimpango/layout/__init__.py
 manimpango/layout/_layout.pyx
+manimpango/layout/layout.pxi
 manimpango/renderer/__init__.py
+manimpango/renderer/cairo_utils.pxi
 manimpango/renderer/image_renderer.pxd
 manimpango/renderer/image_renderer.pyi
 manimpango/renderer/image_renderer.pyx
 manimpango/renderer/svg_renderer.pxd
 manimpango/renderer/svg_renderer.pyi
 manimpango/renderer/svg_renderer.pyx
 manimpango/utils/__init__.py
```

### Comparing `ManimPango-1.0.0a1/PKG-INFO` & `ManimPango-1.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ManimPango
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Bindings for Pango for using with Manim.
 Home-page: https://manimpango.manim.community/
 Author: Naveen M K
 Author-email: naveen@manim.community
 Maintainer: The Manim Community Developers
 License: MIT
 Project-URL: Documentation, https://manimpango.manim.community/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ManimPango Version: 1.0.0a1 Summary: Bindings for
+Metadata-Version: 2.1 Name: ManimPango Version: 1.0.0a2 Summary: Bindings for
 Pango for using with Manim. Home-page: https://manimpango.manim.community/
 Author: Naveen M K Author-email: naveen@manim.community Maintainer: The Manim
 Community Developers License: MIT Project-URL: Documentation, https://
 manimpango.manim.community/ Project-URL: Source, https://github.com/
 ManimCommunity/manimpango Project-URL: Release notes, https://github.com/
 ManimCommunity/ManimPango/releases/ Description: # ManimPango
 [PyPI_Latest_Release] [PyPI_-_Wheel] [PyPI_-_Downloads] [PyPI_-_License] [PyPI
```

### Comparing `ManimPango-1.0.0a1/README.md` & `ManimPango-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/docs/RELEASE.rst` & `ManimPango-1.0.0a2/docs/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/docs/_static/favicon.ico` & `ManimPango-1.0.0a2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/docs/_static/logo.png` & `ManimPango-1.0.0a2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/docs/_templates/autosummary/module.rst` & `ManimPango-1.0.0a2/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/docs/building.rst` & `ManimPango-1.0.0a2/docs/building.rst`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/docs/conf.py` & `ManimPango-1.0.0a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/docs/examples.rst` & `ManimPango-1.0.0a2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/docs/index.rst` & `ManimPango-1.0.0a2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/docs/integration.rst` & `ManimPango-1.0.0a2/docs/integration.rst`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/docs/make.bat` & `ManimPango-1.0.0a2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/docs/reference.rst` & `ManimPango-1.0.0a2/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/__init__.py` & `ManimPango-1.0.0a2/manimpango/__init__.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/_distributor_init.py` & `ManimPango-1.0.0a2/manimpango/_distributor_init.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/attributes/__init__.py` & `ManimPango-1.0.0a2/manimpango/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/cmanimpango.pyx` & `ManimPango-1.0.0a2/manimpango/cmanimpango.pyx`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/enums.pyx` & `ManimPango-1.0.0a2/manimpango/enums.pyx`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/fonts/__init__.py` & `ManimPango-1.0.0a2/manimpango/fonts/__init__.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/fonts/_font_desc.pyi` & `ManimPango-1.0.0a2/manimpango/fonts/_font_desc.pyi`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/fonts/_font_desc.pyx` & `ManimPango-1.0.0a2/manimpango/fonts/_font_desc.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -75,16 +75,19 @@
     def variant(self, variant):
         pango_font_description_set_variant(
             self.pango_font_desc, variant.value)
 
     @classmethod
     def from_string(cls, string: str):
         _t = _FontDescription()
+        cdef PangoFontDescription* font_desc = NULL
         _t.pango_font_desc = \
             pango_font_description_from_string(string.encode())
+        if _t.pango_font_desc is NULL:
+            raise ValueError("pango_font_description_from_string() returned NULL")
         return _t
 
     def __repr__(self):
         cdef char* desc = \
             pango_font_description_to_string(self.pango_font_desc)
         p_desc = <bytes>desc
         g_free(desc)
```

### Comparing `ManimPango-1.0.0a1/manimpango/fonts/enums.pyx` & `ManimPango-1.0.0a2/manimpango/fonts/enums.pyx`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/include/cairo.pxd` & `ManimPango-1.0.0a2/manimpango/include/cairo.pxd`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/include/glib.pxd` & `ManimPango-1.0.0a2/manimpango/include/glib.pxd`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/include/pango.pxd` & `ManimPango-1.0.0a2/manimpango/include/pango.pxd`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/include/pango_attributes.pxd` & `ManimPango-1.0.0a2/manimpango/include/pango_attributes.pxd`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/layout/__init__.py` & `ManimPango-1.0.0a2/manimpango/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/layout/_layout.pyx` & `ManimPango-1.0.0a2/manimpango/layout/_layout.pyx`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/register_font.pxd` & `ManimPango-1.0.0a2/manimpango/register_font.pxd`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/register_font.pyx` & `ManimPango-1.0.0a2/manimpango/register_font.pyx`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/renderer/image_renderer.pxd` & `ManimPango-1.0.0a2/manimpango/renderer/image_renderer.pxd`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/renderer/image_renderer.pyx` & `ManimPango-1.0.0a2/manimpango/renderer/image_renderer.pyx`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/renderer/svg_renderer.pxd` & `ManimPango-1.0.0a2/manimpango/renderer/svg_renderer.pxd`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/renderer/svg_renderer.pyx` & `ManimPango-1.0.0a2/manimpango/renderer/svg_renderer.pyx`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/utils/utils.py` & `ManimPango-1.0.0a2/manimpango/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/manimpango/utils/utils.pyx` & `ManimPango-1.0.0a2/manimpango/utils/utils.pyx`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/setup.py` & `ManimPango-1.0.0a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,10 +318,10 @@
     project_urls={
         "Documentation": "https://manimpango.manim.community/",
         "Source": "https://github.com/ManimCommunity/manimpango",
         "Release notes": "https://github.com/ManimCommunity/ManimPango/releases/",
     },
     ext_modules=ext_modules,
     package_data={
-        "manimpango": ["*.pxd", "*.pyx", "*.pyi"],
+        "manimpango": ["*.pxd", "*.pyx", "*.pyi", "*.pxi"],
     },
 )
```

### Comparing `ManimPango-1.0.0a1/tests/__init__.py` & `ManimPango-1.0.0a2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/tests/_manim.py` & `ManimPango-1.0.0a2/tests/_manim.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/tests/conftest.py` & `ManimPango-1.0.0a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/tests/fonts/AdobeVFPrototype.ttf` & `ManimPango-1.0.0a2/tests/fonts/AdobeVFPrototype.ttf`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/tests/fonts/BungeeColor-Regular_colr_Windows.ttf` & `ManimPango-1.0.0a2/tests/fonts/BungeeColor-Regular_colr_Windows.ttf`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/tests/fonts/BungeeOutline-Regular.ttf` & `ManimPango-1.0.0a2/tests/fonts/BungeeOutline-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/tests/fonts/LICENSE.txt` & `ManimPango-1.0.0a2/tests/fonts/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/tests/fonts/MaShanZheng-Regular.ttf` & `ManimPango-1.0.0a2/tests/fonts/MaShanZheng-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/tests/svg_tester.py` & `ManimPango-1.0.0a2/tests/svg_tester.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/tests/test_attributes.py` & `ManimPango-1.0.0a2/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/tests/test_colors.py` & `ManimPango-1.0.0a2/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/tests/test_font_desc.py` & `ManimPango-1.0.0a2/tests/test_font_desc.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/tests/test_fonts.py` & `ManimPango-1.0.0a2/tests/test_fonts.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/tests/test_layout.py` & `ManimPango-1.0.0a2/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/tests/test_list_fonts.py` & `ManimPango-1.0.0a2/tests/test_list_fonts.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/tests/test_markup.py` & `ManimPango-1.0.0a2/tests/test_markup.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/tests/test_renderer.py` & `ManimPango-1.0.0a2/tests/test_renderer.py`

 * *Files identical despite different names*

### Comparing `ManimPango-1.0.0a1/tests/test_utils.py` & `ManimPango-1.0.0a2/tests/test_utils.py`

 * *Files identical despite different names*

