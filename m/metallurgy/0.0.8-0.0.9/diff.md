# Comparing `tmp/metallurgy-0.0.8.tar.gz` & `tmp/metallurgy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metallurgy-0.0.8.tar", last modified: Thu Sep 22 16:19:45 2022, max compression
+gzip compressed data, was "metallurgy-0.0.9.tar", last modified: Fri Sep 23 09:06:22 2022, max compression
```

## Comparing `metallurgy-0.0.8.tar` & `metallurgy-0.0.9.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-22 16:19:45.202012 metallurgy-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-22 16:19:45.198012 metallurgy-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-22 16:19:45.198012 metallurgy-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1155 2022-09-22 16:19:35.000000 metallurgy-0.0.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (116)      605 2022-09-22 16:19:35.000000 metallurgy-0.0.8/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (116)      981 2022-09-22 16:19:35.000000 metallurgy-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      402 2022-09-22 16:19:35.000000 metallurgy-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      179 2022-09-22 16:19:35.000000 metallurgy-0.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1522 2022-09-22 16:19:35.000000 metallurgy-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      904 2022-09-22 16:19:45.202012 metallurgy-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      252 2022-09-22 16:19:35.000000 metallurgy-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-22 16:19:45.198012 metallurgy-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (116)      638 2022-09-22 16:19:35.000000 metallurgy-0.0.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)      804 2022-09-22 16:19:35.000000 metallurgy-0.0.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)       22 2022-09-22 16:19:35.000000 metallurgy-0.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-22 16:19:45.198012 metallurgy-0.0.8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (116)     2308 2022-09-22 16:19:35.000000 metallurgy-0.0.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      569 2022-09-22 16:19:35.000000 metallurgy-0.0.8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      127 2022-09-22 16:19:35.000000 metallurgy-0.0.8/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-22 16:19:45.202012 metallurgy-0.0.8/metallurgy/
--rw-r--r--   0 runner    (1001) docker     (116)      960 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      176 2022-09-22 16:19:45.000000 metallurgy-0.0.8/metallurgy/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)    41142 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/alloy.py
--rw-r--r--   0 runner    (1001) docker     (116)      778 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/analyse.py
--rw-r--r--   0 runner    (1001) docker     (116)     1254 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/calculate.py
--rw-r--r--   0 runner    (1001) docker     (116)      102 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)      901 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/density.py
--rw-r--r--   0 runner    (1001) docker     (116)     2117 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/deviation.py
--rw-r--r--   0 runner    (1001) docker     (116)     8765 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/enthalpy.py
--rw-r--r--   0 runner    (1001) docker     (116)     3567 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/entropy.py
--rw-r--r--   0 runner    (1001) docker     (116)     1016 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/features.py
--rw-r--r--   0 runner    (1001) docker     (116)     8599 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/generate.py
--rw-r--r--   0 runner    (1001) docker     (116)      764 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/linear_mixture.py
--rw-r--r--   0 runner    (1001) docker     (116)     6446 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/plots.py
--rw-r--r--   0 runner    (1001) docker     (116)      859 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/price.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/py.typed
--rw-r--r--   0 runner    (1001) docker     (116)     2139 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/radii.py
--rw-r--r--   0 runner    (1001) docker     (116)     1177 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/ratios.py
--rw-r--r--   0 runner    (1001) docker     (116)      647 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/rdf.py
--rw-r--r--   0 runner    (1001) docker     (116)     1466 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/valence.py
--rw-r--r--   0 runner    (1001) docker     (116)     2205 2022-09-22 16:19:35.000000 metallurgy-0.0.8/metallurgy/viscosity.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-22 16:19:45.202012 metallurgy-0.0.8/metallurgy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      904 2022-09-22 16:19:45.000000 metallurgy-0.0.8/metallurgy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1093 2022-09-22 16:19:45.000000 metallurgy-0.0.8/metallurgy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-09-22 16:19:45.000000 metallurgy-0.0.8/metallurgy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       84 2022-09-22 16:19:45.000000 metallurgy-0.0.8/metallurgy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       11 2022-09-22 16:19:45.000000 metallurgy-0.0.8/metallurgy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      683 2022-09-22 16:19:35.000000 metallurgy-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       44 2022-09-22 16:19:35.000000 metallurgy-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      899 2022-09-22 16:19:45.202012 metallurgy-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       69 2022-09-22 16:19:35.000000 metallurgy-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-22 16:19:45.202012 metallurgy-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (116)      336 2022-09-22 16:19:35.000000 metallurgy-0.0.8/tests/test_alloy.py
--rw-r--r--   0 runner    (1001) docker     (116)      209 2022-09-22 16:19:35.000000 metallurgy-0.0.8/tests/test_deviation.py
--rw-r--r--   0 runner    (1001) docker     (116)     1769 2022-09-22 16:19:35.000000 metallurgy-0.0.8/tests/test_enthalpy.py
--rw-r--r--   0 runner    (1001) docker     (116)     1538 2022-09-22 16:19:35.000000 metallurgy-0.0.8/tests/test_entropy.py
--rw-r--r--   0 runner    (1001) docker     (116)     3646 2022-09-22 16:19:35.000000 metallurgy-0.0.8/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (116)      323 2022-09-22 16:19:35.000000 metallurgy-0.0.8/tests/test_linear_mixture.py
--rw-r--r--   0 runner    (1001) docker     (116)      513 2022-09-22 16:19:35.000000 metallurgy-0.0.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-23 09:06:22.795392 metallurgy-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-23 09:06:22.791392 metallurgy-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-23 09:06:22.791392 metallurgy-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     1155 2022-09-23 09:06:13.000000 metallurgy-0.0.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      605 2022-09-23 09:06:13.000000 metallurgy-0.0.9/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      981 2022-09-23 09:06:13.000000 metallurgy-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      402 2022-09-23 09:06:13.000000 metallurgy-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      179 2022-09-23 09:06:13.000000 metallurgy-0.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     1522 2022-09-23 09:06:13.000000 metallurgy-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      904 2022-09-23 09:06:22.795392 metallurgy-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      252 2022-09-23 09:06:13.000000 metallurgy-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-23 09:06:22.791392 metallurgy-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)      638 2022-09-23 09:06:13.000000 metallurgy-0.0.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)      804 2022-09-23 09:06:13.000000 metallurgy-0.0.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2022-09-23 09:06:13.000000 metallurgy-0.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-23 09:06:22.791392 metallurgy-0.0.9/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (116)     2308 2022-09-23 09:06:13.000000 metallurgy-0.0.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)      569 2022-09-23 09:06:13.000000 metallurgy-0.0.9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      127 2022-09-23 09:06:13.000000 metallurgy-0.0.9/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-23 09:06:22.795392 metallurgy-0.0.9/metallurgy/
+-rw-r--r--   0 runner    (1001) docker     (116)      960 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      176 2022-09-23 09:06:22.000000 metallurgy-0.0.9/metallurgy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)    41142 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/alloy.py
+-rw-r--r--   0 runner    (1001) docker     (116)      778 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1254 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (116)      102 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (116)      901 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/density.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2117 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/deviation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8765 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/enthalpy.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3567 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1016 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/features.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8689 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/generate.py
+-rw-r--r--   0 runner    (1001) docker     (116)      764 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/linear_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6446 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/plots.py
+-rw-r--r--   0 runner    (1001) docker     (116)      859 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/price.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (116)     2139 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/radii.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1177 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/ratios.py
+-rw-r--r--   0 runner    (1001) docker     (116)      647 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1466 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/valence.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2205 2022-09-23 09:06:13.000000 metallurgy-0.0.9/metallurgy/viscosity.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-23 09:06:22.795392 metallurgy-0.0.9/metallurgy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      904 2022-09-23 09:06:22.000000 metallurgy-0.0.9/metallurgy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1076 2022-09-23 09:06:22.000000 metallurgy-0.0.9/metallurgy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-09-23 09:06:22.000000 metallurgy-0.0.9/metallurgy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      128 2022-09-23 09:06:22.000000 metallurgy-0.0.9/metallurgy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       11 2022-09-23 09:06:22.000000 metallurgy-0.0.9/metallurgy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      683 2022-09-23 09:06:13.000000 metallurgy-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)      947 2022-09-23 09:06:22.795392 metallurgy-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)       69 2022-09-23 09:06:13.000000 metallurgy-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-23 09:06:22.795392 metallurgy-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)      336 2022-09-23 09:06:13.000000 metallurgy-0.0.9/tests/test_alloy.py
+-rw-r--r--   0 runner    (1001) docker     (116)      209 2022-09-23 09:06:13.000000 metallurgy-0.0.9/tests/test_deviation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1769 2022-09-23 09:06:13.000000 metallurgy-0.0.9/tests/test_enthalpy.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1538 2022-09-23 09:06:13.000000 metallurgy-0.0.9/tests/test_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3646 2022-09-23 09:06:13.000000 metallurgy-0.0.9/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (116)      323 2022-09-23 09:06:13.000000 metallurgy-0.0.9/tests/test_linear_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (116)      475 2022-09-23 09:06:13.000000 metallurgy-0.0.9/tox.ini
```

### Comparing `metallurgy-0.0.8/.github/workflows/publish-to-pypi.yml` & `metallurgy-0.0.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/.github/workflows/tests.yml` & `metallurgy-0.0.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/.gitignore` & `metallurgy-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/LICENSE` & `metallurgy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/PKG-INFO` & `metallurgy-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metallurgy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Calculates approximate properties of alloy compositions.
 Home-page: https://github.com/Robert-Forrest/metallurgy
 Author: Robert Forrest
 Author-email: robertforrest@live.com
 License: BSD 3-Clause License
 Platform: unix
 Platform: linux
```

### Comparing `metallurgy-0.0.8/docs/Makefile` & `metallurgy-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/docs/make.bat` & `metallurgy-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/docs/source/conf.py` & `metallurgy-0.0.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/docs/source/index.rst` & `metallurgy-0.0.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/metallurgy/__init__.py` & `metallurgy-0.0.9/metallurgy/__init__.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/metallurgy/alloy.py` & `metallurgy-0.0.9/metallurgy/alloy.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/metallurgy/analyse.py` & `metallurgy-0.0.9/metallurgy/analyse.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/metallurgy/calculate.py` & `metallurgy-0.0.9/metallurgy/calculate.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/metallurgy/density.py` & `metallurgy-0.0.9/metallurgy/density.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/metallurgy/deviation.py` & `metallurgy-0.0.9/metallurgy/deviation.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/metallurgy/enthalpy.py` & `metallurgy-0.0.9/metallurgy/enthalpy.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/metallurgy/entropy.py` & `metallurgy-0.0.9/metallurgy/entropy.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/metallurgy/features.py` & `metallurgy-0.0.9/metallurgy/features.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/metallurgy/generate.py` & `metallurgy-0.0.9/metallurgy/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,21 @@
     num_extra_elements -= len(percentage_constraints)
 
     if num_extra_elements > 0:
         other_elements = allowed_elements[:]
         for element in percentage_constraints:
             if element in other_elements:
                 other_elements.remove(element)
+
         elements = list(percentage_constraints.keys()) + list(
-            np.random.choice(other_elements, num_extra_elements, replace=False)
+            np.random.choice(
+                other_elements,
+                min(num_extra_elements, len(other_elements)),
+                replace=False,
+            )
         )
 
     else:
         elements = list(
             np.random.choice(
                 list(percentage_constraints.keys()),
                 num_extra_elements + len(percentage_constraints.keys()),
```

### Comparing `metallurgy-0.0.8/metallurgy/linear_mixture.py` & `metallurgy-0.0.9/metallurgy/linear_mixture.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/metallurgy/plots.py` & `metallurgy-0.0.9/metallurgy/plots.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/metallurgy/price.py` & `metallurgy-0.0.9/metallurgy/price.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/metallurgy/radii.py` & `metallurgy-0.0.9/metallurgy/radii.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/metallurgy/ratios.py` & `metallurgy-0.0.9/metallurgy/ratios.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/metallurgy/rdf.py` & `metallurgy-0.0.9/metallurgy/rdf.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/metallurgy/valence.py` & `metallurgy-0.0.9/metallurgy/valence.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/metallurgy/viscosity.py` & `metallurgy-0.0.9/metallurgy/viscosity.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/metallurgy.egg-info/PKG-INFO` & `metallurgy-0.0.9/metallurgy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metallurgy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Calculates approximate properties of alloy compositions.
 Home-page: https://github.com/Robert-Forrest/metallurgy
 Author: Robert Forrest
 Author-email: robertforrest@live.com
 License: BSD 3-Clause License
 Platform: unix
 Platform: linux
```

### Comparing `metallurgy-0.0.8/metallurgy.egg-info/SOURCES.txt` & `metallurgy-0.0.9/metallurgy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
 LICENSE
 README.md
 pyproject.toml
-requirements.txt
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/publish-to-pypi.yml
 .github/workflows/tests.yml
 docs/Makefile
 docs/make.bat
```

### Comparing `metallurgy-0.0.8/pyproject.toml` & `metallurgy-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/setup.cfg` & `metallurgy-0.0.9/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 	Operating System :: OS Independent
 
 [options]
 packages = metallurgy
 python_requires = >=3.7
 install_requires = 
 	pandas
+	elementy
+	cerebral
+	matplotlib
+	python-ternary
 
 [options.entry_points]
 console_scripts = 
 
 [options.extras_require]
 dev = 
 	pre-commit
```

### Comparing `metallurgy-0.0.8/tests/test_enthalpy.py` & `metallurgy-0.0.9/tests/test_enthalpy.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/tests/test_entropy.py` & `metallurgy-0.0.9/tests/test_entropy.py`

 * *Files identical despite different names*

### Comparing `metallurgy-0.0.8/tests/test_generate.py` & `metallurgy-0.0.9/tests/test_generate.py`

 * *Files identical despite different names*

