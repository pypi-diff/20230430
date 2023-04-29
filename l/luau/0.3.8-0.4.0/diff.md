# Comparing `tmp/luau-0.3.8.tar.gz` & `tmp/luau-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luau-0.3.8.tar", last modified: Tue Apr 18 16:50:22 2023, max compression
+gzip compressed data, was "luau-0.4.0.tar", last modified: Sat Apr 29 22:13:29 2023, max compression
```

## Comparing `luau-0.3.8.tar` & `luau-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 16:50:22.439170 luau-0.3.8/
--rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.3.8/LICENSE
--rw-rw-rw-   0        0        0      405 2023-04-18 16:50:22.438173 luau-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.3.8/README.md
--rw-rw-rw-   0        0        0      512 2023-04-18 16:50:03.000000 luau-0.3.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 16:50:22.439170 luau-0.3.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-18 16:50:22.396287 luau-0.3.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 16:50:22.406261 luau-0.3.8/src/luau/
--rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.3.8/src/luau/__init__.py
--rw-rw-rw-   0        0        0     5709 2023-04-15 01:24:18.000000 luau-0.3.8/src/luau/convert.py
--rw-rw-rw-   0        0        0     2627 2023-04-18 16:26:04.000000 luau-0.3.8/src/luau/path.py
-drwxrwxrwx   0        0        0        0 2023-04-18 16:50:22.437176 luau-0.3.8/src/luau/roblox/
--rw-rw-rw-   0        0        0      937 2023-04-18 01:10:33.000000 luau-0.3.8/src/luau/roblox/__init__.py
--rw-rw-rw-   0        0        0     1821 2023-04-18 16:49:53.000000 luau-0.3.8/src/luau/roblox/rojo.py
--rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.3.8/src/luau/roblox/tool.py
--rw-rw-rw-   0        0        0      863 2023-04-14 22:00:20.000000 luau-0.3.8/src/luau/roblox/util.py
--rw-rw-rw-   0        0        0     2849 2023-04-15 00:38:19.000000 luau-0.3.8/src/luau/roblox/wally.py
-drwxrwxrwx   0        0        0        0 2023-04-18 16:50:22.429219 luau-0.3.8/src/luau.egg-info/
--rw-rw-rw-   0        0        0      405 2023-04-18 16:50:22.000000 luau-0.3.8/src/luau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-04-18 16:50:22.000000 luau-0.3.8/src/luau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 16:50:22.000000 luau-0.3.8/src/luau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-18 16:50:22.000000 luau-0.3.8/src/luau.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-18 16:50:22.000000 luau-0.3.8/src/luau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 22:13:29.156001 luau-0.4.0/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-04-29 22:13:29.155005 luau-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.4.0/README.md
+-rw-rw-rw-   0        0        0      547 2023-04-29 22:13:02.000000 luau-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 22:13:29.156001 luau-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 22:13:29.102157 luau-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-29 22:13:29.117109 luau-0.4.0/src/luau/
+-rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.4.0/src/luau/__init__.py
+-rw-rw-rw-   0        0        0     5709 2023-04-15 01:24:18.000000 luau-0.4.0/src/luau/convert.py
+-rw-rw-rw-   0        0        0     2627 2023-04-18 16:26:04.000000 luau-0.4.0/src/luau/path.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:13:29.152011 luau-0.4.0/src/luau/roblox/
+-rw-rw-rw-   0        0        0      997 2023-04-29 22:08:10.000000 luau-0.4.0/src/luau/roblox/__init__.py
+-rw-rw-rw-   0        0        0   117136 2023-04-29 21:45:18.000000 luau-0.4.0/src/luau/roblox/api.py
+-rw-rw-rw-   0        0        0     1761 2023-04-29 22:08:06.000000 luau-0.4.0/src/luau/roblox/rojo.py
+-rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.4.0/src/luau/roblox/tool.py
+-rw-rw-rw-   0        0        0     1689 2023-04-29 22:08:06.000000 luau-0.4.0/src/luau/roblox/util.py
+-rw-rw-rw-   0        0        0     2734 2023-04-29 22:09:37.000000 luau-0.4.0/src/luau/roblox/wally.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:13:29.141040 luau-0.4.0/src/luau.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-04-29 22:13:29.000000 luau-0.4.0/src/luau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-04-29 22:13:29.000000 luau-0.4.0/src/luau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 22:13:29.000000 luau-0.4.0/src/luau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-29 22:13:29.000000 luau-0.4.0/src/luau.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-29 22:13:29.000000 luau-0.4.0/src/luau.egg-info/top_level.txt
```

### Comparing `luau-0.3.8/LICENSE` & `luau-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `luau-0.3.8/src/luau/__init__.py` & `luau-0.4.0/src/luau/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.8/src/luau/convert.py` & `luau-0.4.0/src/luau/convert.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.8/src/luau/path.py` & `luau-0.4.0/src/luau/path.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.8/src/luau/roblox/__init__.py` & `luau-0.4.0/src/luau/roblox/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
-from .tool import get_tool_name
+from .util import run_bundled_exe
 
 def format(path: str):
-	stylua_tool_name = get_tool_name("JohnnyMorganz/StyLua", "0.15.3")
-	os.system(f"{stylua_tool_name} {path}")
+	# stylua_tool_name = get_tool_name("JohnnyMorganz/StyLua", "0.15.3")
+	# os.system(f"{stylua_tool_name} {path}")
+	run_bundled_exe(exe_name="stylua.exe", args=[path])
 
 def write_script(build_path: str, content: str, write_as_directory: bool=False):
 	dir_name, file_name = os.path.split(build_path)
 	if not os.path.exists(dir_name):
 		os.makedirs(dir_name)
 	elif os.path.exists(build_path):
 		os.remove(build_path)
```

### Comparing `luau-0.3.8/src/luau/roblox/rojo.py` & `luau-0.4.0/src/luau/roblox/rojo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import dpath
 import json
-from .tool import get_tool_name
+from .util import run_bundled_exe
 
 DEFAULT_ROJO_PROJECT_PATH = "default.project.json"
 ROJO_SOURCE = "rojo-rbx/rojo"
 ROJO_VERSION = "7.1.0"
 
 def get_rojo_project_path() -> str:
 	if os.path.exists(DEFAULT_ROJO_PROJECT_PATH):
@@ -14,21 +14,18 @@
 		if os.path.isfile(file_path):
 			base, ext = os.path.splitext(file_path)
 			if ext == ".json":
 				sec_base, sec_ext = os.path.splitext(base)
 				if sec_ext== ".project":
 					return file_path
 
-def get_rojo_name() -> str:
-	return get_tool_name(ROJO_SOURCE, ROJO_VERSION)
-
 def build_sourcemap(project_json_path: str = ""):
 	if project_json_path == "":
 		project_json_path = get_rojo_project_path()
-	os.system(f"{get_rojo_name()} sourcemap {project_json_path} --output sourcemap.json")	
+	run_bundled_exe(exe_name="rojo.exe", args=["sourcemap", project_json_path, "--output", "sourcemap.json"])
 
 def get_roblox_path_from_env_path(env_path: str) -> str:
 	project_path = get_rojo_project_path()
 	rojo_file = open(project_path, "r")
 	rojo_config = json.loads(rojo_file.read())
 	rojo_file.close()
 	tree_config = rojo_config["tree"]
```

### Comparing `luau-0.3.8/src/luau/roblox/tool.py` & `luau-0.4.0/src/luau/roblox/tool.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.8/src/luau/roblox/wally.py` & `luau-0.4.0/src/luau/roblox/wally.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 import os
 import toml
+from .util import run_bundled_exe
 from .tool import get_tool_name
-from .rojo import get_rojo_project_path, get_rojo_name, build_sourcemap
+from .rojo import get_rojo_project_path, build_sourcemap
 
 WALLY_SOURCE = "UpliftGames/wally"
 WALLY_VERSION = "0.3.1"
 WPT_SOURCE = "JohnnyMorganz/wally-package-types"
 WPT_VERSION = "1.2.0"
 
 def get_wally_name():
 	return get_tool_name(WALLY_SOURCE, WALLY_VERSION)
 
-def get_wally_package_types_name():
-	return get_tool_name(WPT_SOURCE, WPT_VERSION)
-
 def update_wally():
 
 	project_path = get_rojo_project_path()
-
 	wally_tool_name = get_wally_name()
-	rojo_tool_name = get_rojo_name()
-	wpt_tool_name = get_wally_package_types_name()
 
 	os.system(f"{wally_tool_name} install")
 	build_sourcemap()
-	os.system(f"{wpt_tool_name} --sourcemap sourcemap.json Packages")
+	run_bundled_exe(exe_name="wally-package-types.exe", args=["--sourcemap", "sourcemap.json", "Packages"])
 
 def get_wally_package_nickname(package_wally_path: str) -> str:
 	wally_config = toml.loads(open("wally.toml", "r").read())
 	generated_nickname = (package_wally_path.split("/")[1].split("@")[0]).title()
 	name_parts = generated_nickname.split("-")
 	for i, name_part in enumerate(name_parts):
 		name_parts[i] = name_part.title()
```

