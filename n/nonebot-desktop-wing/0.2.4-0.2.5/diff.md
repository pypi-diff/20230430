# Comparing `tmp/nonebot-desktop-wing-0.2.4.tar.gz` & `tmp/nonebot-desktop-wing-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-desktop-wing-0.2.4.tar", last modified: Sun Apr 30 12:41:57 2023, max compression
+gzip compressed data, was "nonebot-desktop-wing-0.2.5.tar", last modified: Sun Apr 30 12:54:36 2023, max compression
```

## Comparing `nonebot-desktop-wing-0.2.4.tar` & `nonebot-desktop-wing-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:41:57.911306 nonebot-desktop-wing-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-30 12:41:47.000000 nonebot-desktop-wing-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-30 12:41:57.911306 nonebot-desktop-wing-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-30 12:41:47.000000 nonebot-desktop-wing-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:41:57.907306 nonebot-desktop-wing-0.2.4/nonebot_desktop_wing/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-30 12:41:47.000000 nonebot-desktop-wing-0.2.4/nonebot_desktop_wing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-30 12:41:47.000000 nonebot-desktop-wing-0.2.4/nonebot_desktop_wing/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-30 12:41:47.000000 nonebot-desktop-wing-0.2.4/nonebot_desktop_wing/hindsight.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-30 12:41:47.000000 nonebot-desktop-wing-0.2.4/nonebot_desktop_wing/lazylib.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-30 12:41:47.000000 nonebot-desktop-wing-0.2.4/nonebot_desktop_wing/lazylib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-04-30 12:41:47.000000 nonebot-desktop-wing-0.2.4/nonebot_desktop_wing/molecules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-04-30 12:41:47.000000 nonebot-desktop-wing-0.2.4/nonebot_desktop_wing/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-30 12:41:47.000000 nonebot-desktop-wing-0.2.4/nonebot_desktop_wing/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:41:57.911306 nonebot-desktop-wing-0.2.4/nonebot_desktop_wing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-30 12:41:57.000000 nonebot-desktop-wing-0.2.4/nonebot_desktop_wing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-30 12:41:57.000000 nonebot-desktop-wing-0.2.4/nonebot_desktop_wing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:41:57.000000 nonebot-desktop-wing-0.2.4/nonebot_desktop_wing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-30 12:41:57.000000 nonebot-desktop-wing-0.2.4/nonebot_desktop_wing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-30 12:41:57.000000 nonebot-desktop-wing-0.2.4/nonebot_desktop_wing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-30 12:41:47.000000 nonebot-desktop-wing-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 12:41:57.911306 nonebot-desktop-wing-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:54:36.892450 nonebot-desktop-wing-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-30 12:54:22.000000 nonebot-desktop-wing-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-30 12:54:36.892450 nonebot-desktop-wing-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-30 12:54:22.000000 nonebot-desktop-wing-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:54:36.892450 nonebot-desktop-wing-0.2.5/nonebot_desktop_wing/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-30 12:54:22.000000 nonebot-desktop-wing-0.2.5/nonebot_desktop_wing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-30 12:54:22.000000 nonebot-desktop-wing-0.2.5/nonebot_desktop_wing/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-30 12:54:22.000000 nonebot-desktop-wing-0.2.5/nonebot_desktop_wing/hindsight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-30 12:54:22.000000 nonebot-desktop-wing-0.2.5/nonebot_desktop_wing/lazylib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-30 12:54:22.000000 nonebot-desktop-wing-0.2.5/nonebot_desktop_wing/lazylib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-04-30 12:54:22.000000 nonebot-desktop-wing-0.2.5/nonebot_desktop_wing/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-04-30 12:54:22.000000 nonebot-desktop-wing-0.2.5/nonebot_desktop_wing/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-30 12:54:22.000000 nonebot-desktop-wing-0.2.5/nonebot_desktop_wing/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:54:36.892450 nonebot-desktop-wing-0.2.5/nonebot_desktop_wing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-30 12:54:36.000000 nonebot-desktop-wing-0.2.5/nonebot_desktop_wing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-30 12:54:36.000000 nonebot-desktop-wing-0.2.5/nonebot_desktop_wing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:54:36.000000 nonebot-desktop-wing-0.2.5/nonebot_desktop_wing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-30 12:54:36.000000 nonebot-desktop-wing-0.2.5/nonebot_desktop_wing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-30 12:54:36.000000 nonebot-desktop-wing-0.2.5/nonebot_desktop_wing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-30 12:54:22.000000 nonebot-desktop-wing-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 12:54:36.892450 nonebot-desktop-wing-0.2.5/setup.cfg
```

### Comparing `nonebot-desktop-wing-0.2.4/LICENSE` & `nonebot-desktop-wing-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.4/PKG-INFO` & `nonebot-desktop-wing-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-desktop-wing
-Version: 0.2.4
+Version: 0.2.5
 Summary: Wings for NoneBot desktop applications.
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonedesktop/nonebot-desktop-wing
 Project-URL: Repository, https://github.com/nonedesktop/nonebot-desktop-wing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nonebot-desktop-wing-0.2.4/README.md` & `nonebot-desktop-wing-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.4/nonebot_desktop_wing/__init__.py` & `nonebot-desktop-wing-0.2.5/nonebot_desktop_wing/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.4/nonebot_desktop_wing/constants.py` & `nonebot-desktop-wing-0.2.5/nonebot_desktop_wing/constants.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.4/nonebot_desktop_wing/hindsight.py` & `nonebot-desktop-wing-0.2.5/nonebot_desktop_wing/hindsight.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.4/nonebot_desktop_wing/lazylib.py` & `nonebot-desktop-wing-0.2.5/nonebot_desktop_wing/lazylib.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.4/nonebot_desktop_wing/lazylib.pyi` & `nonebot-desktop-wing-0.2.5/nonebot_desktop_wing/lazylib.pyi`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.4/nonebot_desktop_wing/molecules.py` & `nonebot-desktop-wing-0.2.5/nonebot_desktop_wing/molecules.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.4/nonebot_desktop_wing/project.py` & `nonebot-desktop-wing-0.2.5/nonebot_desktop_wing/project.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.4/nonebot_desktop_wing/resources.py` & `nonebot-desktop-wing-0.2.5/nonebot_desktop_wing/resources.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from functools import cache
+from functools import lru_cache
 from typing import Any, Dict, List, Literal
 
 
-@cache
+@lru_cache
 def load_module_data_raw(
     module_name: Literal["adapters", "plugins", "drivers"]
 ) -> List[Dict[str, Any]]:
     """Get raw module data."""
     from concurrent.futures import ThreadPoolExecutor, as_completed
     import httpx
     exceptions: List[Exception] = []
```

### Comparing `nonebot-desktop-wing-0.2.4/nonebot_desktop_wing.egg-info/PKG-INFO` & `nonebot-desktop-wing-0.2.5/nonebot_desktop_wing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-desktop-wing
-Version: 0.2.4
+Version: 0.2.5
 Summary: Wings for NoneBot desktop applications.
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonedesktop/nonebot-desktop-wing
 Project-URL: Repository, https://github.com/nonedesktop/nonebot-desktop-wing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nonebot-desktop-wing-0.2.4/nonebot_desktop_wing.egg-info/SOURCES.txt` & `nonebot-desktop-wing-0.2.5/nonebot_desktop_wing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.4/pyproject.toml` & `nonebot-desktop-wing-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-desktop-wing"
-version = "0.2.4"
+version = "0.2.5"
 description = "Wings for NoneBot desktop applications."
 authors = [
     {name = "HivertMoZara", email = "worldmozara@163.com"},
 ]
 license = {text = "MIT"}
 dependencies = ["nb_cli~=1.0.0", "python-dotenv~=1.0.0", "httpx>=0.23", "typing-extensions>=4.5.0"]
 requires-python = ">=3.8"
```

