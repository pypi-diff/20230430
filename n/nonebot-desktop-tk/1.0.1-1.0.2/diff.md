# Comparing `tmp/nonebot-desktop-tk-1.0.1.tar.gz` & `tmp/nonebot-desktop-tk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-desktop-tk-1.0.1.tar", last modified: Sun Apr 30 12:28:10 2023, max compression
+gzip compressed data, was "nonebot-desktop-tk-1.0.2.tar", last modified: Sun Apr 30 12:46:38 2023, max compression
```

## Comparing `nonebot-desktop-tk-1.0.1.tar` & `nonebot-desktop-tk-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:28:10.273184 nonebot-desktop-tk-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-30 12:27:57.000000 nonebot-desktop-tk-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-30 12:28:10.273184 nonebot-desktop-tk-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-30 12:27:57.000000 nonebot-desktop-tk-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-30 12:27:57.000000 nonebot-desktop-tk-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 12:28:10.273184 nonebot-desktop-tk-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:28:10.269184 nonebot-desktop-tk-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:28:10.269184 nonebot-desktop-tk-1.0.1/src/nonebot_desktop_tk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 12:27:57.000000 nonebot-desktop-tk-1.0.1/src/nonebot_desktop_tk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-30 12:27:57.000000 nonebot-desktop-tk-1.0.1/src/nonebot_desktop_tk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51797 2023-04-30 12:27:57.000000 nonebot-desktop-tk-1.0.1/src/nonebot_desktop_tk/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:28:10.273184 nonebot-desktop-tk-1.0.1/src/nonebot_desktop_tk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-30 12:28:10.000000 nonebot-desktop-tk-1.0.1/src/nonebot_desktop_tk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-30 12:28:10.000000 nonebot-desktop-tk-1.0.1/src/nonebot_desktop_tk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:28:10.000000 nonebot-desktop-tk-1.0.1/src/nonebot_desktop_tk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-30 12:28:10.000000 nonebot-desktop-tk-1.0.1/src/nonebot_desktop_tk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 12:28:10.000000 nonebot-desktop-tk-1.0.1/src/nonebot_desktop_tk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:46:37.995325 nonebot-desktop-tk-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-30 12:46:27.000000 nonebot-desktop-tk-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-30 12:46:37.995325 nonebot-desktop-tk-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-30 12:46:27.000000 nonebot-desktop-tk-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-30 12:46:27.000000 nonebot-desktop-tk-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 12:46:37.995325 nonebot-desktop-tk-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:46:37.995325 nonebot-desktop-tk-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:46:37.995325 nonebot-desktop-tk-1.0.2/src/nonebot_desktop_tk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 12:46:27.000000 nonebot-desktop-tk-1.0.2/src/nonebot_desktop_tk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-30 12:46:27.000000 nonebot-desktop-tk-1.0.2/src/nonebot_desktop_tk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51797 2023-04-30 12:46:27.000000 nonebot-desktop-tk-1.0.2/src/nonebot_desktop_tk/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:46:37.995325 nonebot-desktop-tk-1.0.2/src/nonebot_desktop_tk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-30 12:46:37.000000 nonebot-desktop-tk-1.0.2/src/nonebot_desktop_tk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-30 12:46:37.000000 nonebot-desktop-tk-1.0.2/src/nonebot_desktop_tk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:46:37.000000 nonebot-desktop-tk-1.0.2/src/nonebot_desktop_tk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-30 12:46:37.000000 nonebot-desktop-tk-1.0.2/src/nonebot_desktop_tk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 12:46:37.000000 nonebot-desktop-tk-1.0.2/src/nonebot_desktop_tk.egg-info/top_level.txt
```

### Comparing `nonebot-desktop-tk-1.0.1/LICENSE` & `nonebot-desktop-tk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-tk-1.0.1/PKG-INFO` & `nonebot-desktop-tk-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-desktop-tk
-Version: 1.0.1
+Version: 1.0.2
 Summary: NoneBot2 GUI manager written with tkinter.
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonedesktop/nonebot-desktop-tk
 Project-URL: Repository, https://github.com/nonedesktop/nonebot-desktop-tk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nonebot-desktop-tk-1.0.1/README.md` & `nonebot-desktop-tk-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-tk-1.0.1/pyproject.toml` & `nonebot-desktop-tk-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "nonebot-desktop-tk"
-version = "1.0.1"
+version = "1.0.2"
 description = "NoneBot2 GUI manager written with tkinter."
 authors = [
     {name = "HivertMoZara", email = "worldmozara@163.com"},
 ]
 license = {text = "MIT"}
-dependencies = ["tkreform>=0.3.4", "nonebot-desktop-wing>=0.2.3"]
+dependencies = ["tkreform>=0.3.4", "nonebot-desktop-wing>=0.2.4"]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.urls]
 Homepage = "https://github.com/nonedesktop/nonebot-desktop-tk"
 Repository = "https://github.com/nonedesktop/nonebot-desktop-tk"
```

### Comparing `nonebot-desktop-tk-1.0.1/src/nonebot_desktop_tk/gui.py` & `nonebot-desktop-tk-1.0.2/src/nonebot_desktop_tk/gui.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-tk-1.0.1/src/nonebot_desktop_tk.egg-info/PKG-INFO` & `nonebot-desktop-tk-1.0.2/src/nonebot_desktop_tk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-desktop-tk
-Version: 1.0.1
+Version: 1.0.2
 Summary: NoneBot2 GUI manager written with tkinter.
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonedesktop/nonebot-desktop-tk
 Project-URL: Repository, https://github.com/nonedesktop/nonebot-desktop-tk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

