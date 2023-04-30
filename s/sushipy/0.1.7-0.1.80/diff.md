# Comparing `tmp/sushipy-0.1.7.tar.gz` & `tmp/sushipy-0.1.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sushipy-0.1.7.tar", last modified: Sat Apr 15 16:00:19 2023, max compression
+gzip compressed data, was "sushipy-0.1.80.tar", last modified: Sun Apr 30 15:55:44 2023, max compression
```

## Comparing `sushipy-0.1.7.tar` & `sushipy-0.1.80.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 16:00:19.743575 sushipy-0.1.7/
--rw-rw-rw-   0        0        0     1087 2023-03-24 14:21:03.000000 sushipy-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     1936 2023-04-15 16:00:19.743575 sushipy-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1604 2023-03-29 18:16:15.000000 sushipy-0.1.7/README.md
--rw-rw-rw-   0        0        0      108 2023-04-05 19:52:34.000000 sushipy-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       36 2023-04-15 15:59:54.000000 sushipy-0.1.7/requirements.txt
--rw-rw-rw-   0        0        0      531 2023-04-15 16:00:19.745574 sushipy-0.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 16:00:19.652576 sushipy-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 16:00:19.693576 sushipy-0.1.7/src/sushipy/
--rw-rw-rw-   0        0        0        0 2023-02-04 16:09:33.000000 sushipy-0.1.7/src/sushipy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 16:00:19.720575 sushipy-0.1.7/src/sushipy/cache/
--rw-rw-rw-   0        0        0        0 2023-01-29 15:04:23.000000 sushipy-0.1.7/src/sushipy/cache/__init__.py
--rw-rw-rw-   0        0        0      206 2023-04-15 15:59:54.000000 sushipy-0.1.7/src/sushipy/cache/cache_template.py
--rw-rw-rw-   0        0        0     1215 2023-03-30 14:52:20.000000 sushipy-0.1.7/src/sushipy/cache/main.py
-drwxrwxrwx   0        0        0        0 2023-04-15 16:00:19.731075 sushipy-0.1.7/src/sushipy/config/
--rw-rw-rw-   0        0        0        0 2023-02-04 17:47:51.000000 sushipy-0.1.7/src/sushipy/config/__init__.py
--rw-rw-rw-   0        0        0     2203 2023-04-15 15:59:54.000000 sushipy-0.1.7/src/sushipy/config/auto_detect.py
--rw-rw-rw-   0        0        0     3584 2023-04-05 20:02:07.000000 sushipy-0.1.7/src/sushipy/config/extends.py
--rw-rw-rw-   0        0        0     4877 2023-04-13 16:25:20.000000 sushipy-0.1.7/src/sushipy/execute.py
--rw-rw-rw-   0        0        0     2822 2023-04-14 13:41:03.000000 sushipy-0.1.7/src/sushipy/git.py
--rw-rw-rw-   0        0        0     4243 2023-04-15 15:59:54.000000 sushipy-0.1.7/src/sushipy/index.py
--rw-rw-rw-   0        0        0     1752 2023-04-15 15:59:54.000000 sushipy-0.1.7/src/sushipy/main.py
--rw-rw-rw-   0        0        0     2050 2023-04-14 13:39:24.000000 sushipy-0.1.7/src/sushipy/one_compile.py
-drwxrwxrwx   0        0        0        0 2023-04-15 16:00:19.734575 sushipy-0.1.7/src/sushipy/scripts/
--rw-rw-rw-   0        0        0      406 2023-04-01 11:57:52.000000 sushipy-0.1.7/src/sushipy/scripts/git_init.ps1
--rw-rw-rw-   0        0        0      330 2023-04-01 11:57:52.000000 sushipy-0.1.7/src/sushipy/scripts/git_init.sh
--rw-rw-rw-   0        0        0      453 2023-03-30 14:53:23.000000 sushipy-0.1.7/src/sushipy/stores.py
-drwxrwxrwx   0        0        0        0 2023-04-15 16:00:19.739075 sushipy-0.1.7/src/sushipy/utils/
--rw-rw-rw-   0        0        0        0 2023-02-10 16:59:00.000000 sushipy-0.1.7/src/sushipy/utils/__init__.py
--rw-rw-rw-   0        0        0      236 2023-02-10 16:59:00.000000 sushipy-0.1.7/src/sushipy/utils/find_dict.py
--rw-rw-rw-   0        0        0      685 2023-03-29 18:15:30.000000 sushipy-0.1.7/src/sushipy/utils/verbose_print.py
-drwxrwxrwx   0        0        0        0 2023-04-15 16:00:19.711075 sushipy-0.1.7/src/sushipy.egg-info/
--rw-rw-rw-   0        0        0     1936 2023-04-15 16:00:19.000000 sushipy-0.1.7/src/sushipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-04-15 16:00:19.000000 sushipy-0.1.7/src/sushipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 16:00:19.000000 sushipy-0.1.7/src/sushipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-15 16:00:19.000000 sushipy-0.1.7/src/sushipy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 16:00:19.742076 sushipy-0.1.7/tests/
--rw-rw-rw-   0        0        0     1665 2023-04-15 15:59:54.000000 sushipy-0.1.7/tests/test_execute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:55:44.158192 sushipy-0.1.80/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-30 15:55:26.000000 sushipy-0.1.80/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 15:55:44.158192 sushipy-0.1.80/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-30 15:55:26.000000 sushipy-0.1.80/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-30 15:55:44.158192 sushipy-0.1.80/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:55:44.150191 sushipy-0.1.80/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:55:44.154192 sushipy-0.1.80/src/sushipy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:55:44.154192 sushipy-0.1.80/src/sushipy/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/cache/cache_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/cache/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:55:44.154192 sushipy-0.1.80/src/sushipy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/config/auto_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/config/extends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/one_compile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:55:44.158192 sushipy-0.1.80/src/sushipy/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/scripts/git_init.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/scripts/git_init.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/stores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:55:44.158192 sushipy-0.1.80/src/sushipy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/utils/find_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/utils/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-30 15:55:26.000000 sushipy-0.1.80/src/sushipy/utils/verbose_print.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:55:44.154192 sushipy-0.1.80/src/sushipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 15:55:44.000000 sushipy-0.1.80/src/sushipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-30 15:55:44.000000 sushipy-0.1.80/src/sushipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 15:55:44.000000 sushipy-0.1.80/src/sushipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 15:55:44.000000 sushipy-0.1.80/src/sushipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:55:44.158192 sushipy-0.1.80/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-30 15:55:26.000000 sushipy-0.1.80/tests/test_execute.py
```

### Comparing `sushipy-0.1.7/LICENSE` & `sushipy-0.1.80/LICENSE`

 * *Files identical despite different names*

### Comparing `sushipy-0.1.7/src/sushipy/cache/main.py` & `sushipy-0.1.80/src/sushipy/cache/main.py`

 * *Files identical despite different names*

### Comparing `sushipy-0.1.7/src/sushipy/config/extends.py` & `sushipy-0.1.80/src/sushipy/config/extends.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from git import Repo
 from rich import print as rich_print
 
 # pylint: disable=import-error, too-few-public-methods
 from ..cache.main import Cache
 
-# from utils.verbose_print import verbose_print TODO
+from ..utils.verbose_print import verbose_print
 
 if isfile("sushicache.py"):
     import sushicache
 # pylint: enable=import-error
 
 
 config = configparser.ConfigParser()
@@ -53,28 +53,28 @@
     def _review_config(self, filename: str):
         rich_print("[bold red]sushi[/bold red]   review configuration!")
 
         with open(f"{tempdir}/sushi/{filename}", "r", encoding="UTF-8") as f:
             content = f.read()
         pydoc.pager(content)
 
-        # rich_print(
-        #     "[bold red]sushi[/bold red]   Press C to cancel, otherwise press any other key."
-        # )
+        rich_print(
+            "[bold red]sushi[/bold red]   Press C to cancel, otherwise press any other key."
+        )
 
         out = input()
 
         if out.upper() == "C":
             rmtree(f"{tempdir}/sushi/")
             sys.exit(0)
 
     def _get_repo(self, data: str, filename: str):
         repourl = f"https://github.com/{data.get('user')}/{data.get('name')}"
 
-        # verbose_print(f"[bold green]sushi[/bold green]   cloning repository {repourl}")
+        verbose_print(f"[bold green]sushi[/bold green]   cloning repository {repourl}")
 
         # clone repository
         repo = Repo.clone_from(repourl, f"{tempdir}/sushi/")
         repo.git.checkout("main")
 
         # show what command will be executed from extended config
         temp_config = configparser.ConfigParser()
@@ -86,17 +86,17 @@
         # add new config to cache
         with open(f"{tempdir}/sushi/{filename}", "r", encoding="UTF-8") as f:
             Cache.update(
                 Cache, "EXTENDS_CONFIG = None", f'EXTENDS_CONFIG = """{f.read()}"""'
             )
 
         rmtree(f"{tempdir}/sushi/")
-        # verbose_print(
-        #     f"[bold green]sushi[/bold green]   removing file {tempdir}/sushi/"
-        # )
+        verbose_print(
+            f"[bold green]sushi[/bold green]   removing file {tempdir}/sushi/"
+        )
 
     def install(self):
         """installs custom config"""
 
         repo: str = config["extends"]["repo"]
         filename: str = config["extends"]["file"]
```

### Comparing `sushipy-0.1.7/src/sushipy/execute.py` & `sushipy-0.1.80/src/sushipy/execute.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,22 +81,27 @@
         call_function = inspect.stack()[1].function
         verbose_print(
             f"[bold green]sushi[/bold green]   finding function {call_function}"
         )
 
         self.init_args = re.sub("[()]", "", rf"{args}".replace(",", ""))
         import_syntax = launch_config["import_syntax"]
+        if config["main"]["use_templates"] is True:
+            import_syntax = sushicache.TEMPLATE_IMPORT_SYNTAX
 
         file_name = main_config["lib_path"].split("/")[-1]
         if main_config["lib_path"][-1] == "*":
             # user selected multiple files
             file_name = main_config["lib_path"].replace("*", file)
             file_name = file_name.split("/")[-1]
 
         self.temp_file = config["temp_file"]["temp_file"]
+        if config["main"]["use_templates"] is True:
+            self.temp_file = sushicache.TEMPLATE_TEMP_FILE
+
         if ONE_COMPILE:
             # if () is in temp file remove it
             delimiter = "SUSHI_FUNCTION"
 
             index = self.temp_file.find(delimiter)
             after = self.temp_file[index + len(delimiter) :]
```

### Comparing `sushipy-0.1.7/src/sushipy/index.py` & `sushipy-0.1.80/src/sushipy/index.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,51 +28,67 @@
 try:
     CUSTOM_TEMP_FILE = sushicache.CUSTOM_TEMP_FILE
 except NameError:
     CUSTOM_TEMP_FILE = """"""
 
 
 def _open_find(file):
-    """finds all functions by using regex from sushi.conf"""
-    verbose_print(
-        f"[bold green]sushi[/bold green]   finding functions in {file} from sushi.conf"
-    )
+    """finds all functions"""
+    verbose_print(f"[bold green]sushi[/bold green]   finding functions in {file}")
 
     with open(file=file, mode="r", encoding="UTF-8") as f:
         lines = f.read()
 
         detect = TSDetect(
             "cpp",
             lines,
         )
 
         for x in detect.parse_tree():
-            tree = x.decode("utf-8")
-            function_name = tree.split("(")[0]
+            data_x = x["data"]
+            tree = data_x.decode("utf-8")
 
-            function_args = tree.split("(")[1].replace(")", "")
-            with suppress(IndexError):
-                function_args = function_args.split(" ")[1]
-
-            data = {
-                "name": function_name,
-                "arg": function_args,
-                "file": file,
-            }
-
-            # pylint: disable=unnecessary-dunder-call
-            if ONE_COMPILE:
-                oc_data = OneCompile().setup()
-                for x in oc_data:
-                    if x["name"] == function_name:
-                        data.__setitem__("uuid", x["uuid"])
-            data.__setitem__("uuid", "")
-            # pylint: enable=unnecessary-dunder-call
+            if x["type"] == "function":
+                function_name = tree.split("(")[0]
 
-            DATA.append(data)
+                function_args = tree.split("(")[1].replace(")", "")
+                with suppress(IndexError):
+                    function_args = function_args.split(" ")[1]
+
+                data = {
+                    "name": function_name,
+                    "arg": function_args,
+                    "file": file,
+                    "type": "function",
+                }
+
+                # pylint: disable=unnecessary-dunder-call
+                if ONE_COMPILE and sushicache.INDEXED_FUNCTIONS is not None:
+                    oc_data = OneCompile().setup()
+                    for data_x in oc_data:
+                        if data_x["name"] == function_name:
+                            data.__setitem__("uuid", data_x["uuid"])
+                data.__setitem__("uuid", "")
+                # pylint: enable=unnecessary-dunder-call
+
+                DATA.append(data)
+            else:
+                # extract variable
+                split = tree.split("=")
+                name = split[0]
+                variable_data = split[1]
+
+                DATA.append(
+                    {
+                        "type": "variable",
+                        "name": name,
+                        "variable_data": variable_data,
+                        "file": file,
+                    }
+                )
 
 
 def find():
     """finds functions"""
 
     files = config["main"]["lib_path"]
 
@@ -118,32 +134,43 @@
     print_space = " " * 100
 
     with open(file=f"out/{file_data}.py", mode="w", encoding="UTF-8") as f:
         # TODO: cleanup
         try:
             if config.getboolean("index", "dev"):
                 f.write("from src.sushipy.execute import Execute\n")
+                f.write("from src.sushipy.utils.variables import SushiVariable\n")
             else:
                 f.write("from sushipy.execute import Execute\n")
+                f.write("from sushipy.utils.variables import SushiVariable\n")
 
         except configparser.NoOptionError:
             f.write("from sushipy.execute import Execute\n")
+            f.write("from sushipy.utils.variables import SushiVariable\n")
 
         # Write each function to our created file
         # pylint: disable=line-too-long
         for x in DATA:
             rich_print(
                 f"[bold yellow]sushi[/bold yellow]   saving indexed function '{x['name']}' ({x['file']}){print_space}"
             )
             # pylint: enable=line-too-long
 
             fname = x["name"]
 
-            f.write(
-                f"def {fname}({x['arg']}):\tExecute('{file_data_old}', '{x['uuid']}', {x['arg']})\n"
-            )
+            if x["type"] == "function":
+                f.write(
+                    f"def {fname}({x['arg']}):\tExecute('{file_data_old}', \
+                        '{x['uuid']}', {x['arg']})\n"
+                )
+            else:
+                variable_name = x["name"].replace(" ", "")
+                variable_data = x["variable_data"]
 
+                f.write(
+                    f"{variable_name} = SushiVariable('{variable_name}', {variable_data})\n"
+                )
         f.close()
 
         rich_print(
             f"[bold green]sushi[/bold green]   saved indexed functions to out/{file_data}.py{print_space}"
         )
```

### Comparing `sushipy-0.1.7/src/sushipy/one_compile.py` & `sushipy-0.1.80/src/sushipy/one_compile.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,83 @@
-"""one compile"""
-
-import configparser
-import uuid
-from contextlib import suppress
-from os.path import isfile
-
-from .cache.main import Cache
-
-config = configparser.ConfigParser()
-config.read("sushi.conf")
-
-# pylint: disable=import-error
-if isfile("sushicache.py"):
-    import sushicache
-
-# pylint: enable=import-error
-
-
-class OneCompile:
-    """one compile"""
-
-    def setup(self) -> None:
-        """setup onecompile"""
-
-        cache_data = sushicache.INDEXED_FUNCTIONS
-
-        # TODO: cleanup
-        if_data = self._extract_if()
-        data = [{"uuid": str(uuid.uuid4()), "name": cache_data[0]["name"]}]
-        out = self._parse_if(if_data["if"], data[0]["uuid"], data[0]["name"])
-
-        if len(cache_data) > 1:
-            for x in range(len(cache_data)):
-                with suppress(IndexError):
-                    out += self._parse_if(
-                        if_data["else"], str(uuid.uuid4()), cache_data[x + 1]["name"]
-                    )
-
-        Cache.update(
-            Cache,
-            f'CUSTOM_TEMP_FILE = """{sushicache.CUSTOM_TEMP_FILE}"""',
-            f'CUSTOM_TEMP_FILE = """{out}"""',
-        )
-
-        return data
-
-    def _extract_if(self):
-        # extracts if statements
-        launch = config["launch"]["if_statement"]
-        else_start = "$SUSHI_ELSE_START"
-
-        split_string = launch.split(else_start)
-
-        return {"if": split_string[0], "else": split_string[1]}
-
-    def _parse_if(self, data, uuid_data, code):
-        translate_date = {
-            "$SUSHI_ARG_NUM": "1",
-            "$SUSHI_SEMICOLON": ";",
-            "$SUSHI_UUID": uuid_data,
-            "$SUSHI_CODE": code,
-        }
-
-        for i, j in translate_date.items():
-            data = data.replace(i, j)
-
-        return data
-
-    def __init__(self) -> None:
-        # TODO: implement other cache system
-        try:
-            if sushicache.ONE_COMPILE_CONFIGURED is False:
-                self.setup()
-        except NameError:
-            return
+"""one compile"""
+
+import configparser
+import uuid
+from contextlib import suppress
+from os.path import isfile
+
+from rich import print as rich_print
+
+from .cache.main import Cache
+
+config = configparser.ConfigParser()
+config.read("sushi.conf")
+
+# pylint: disable=import-error
+if isfile("sushicache.py"):
+    import sushicache
+
+# pylint: enable=import-error
+
+
+class OneCompile:
+    """one compile"""
+
+    def setup(self) -> None:
+        """setup onecompile"""
+
+        cache_data = sushicache.INDEXED_FUNCTIONS
+
+        # TODO: cleanup
+        if_data = self._extract_if()
+        data = [{"uuid": str(uuid.uuid4()), "name": cache_data[0]["name"]}]
+        out = self._parse_if(if_data["if"], data[0]["uuid"], data[0]["name"])
+
+        if len(cache_data) > 1:
+            for x in range(len(cache_data)):
+                with suppress(IndexError):
+                    out += self._parse_if(
+                        if_data["else"], str(uuid.uuid4()), cache_data[x + 1]["name"]
+                    )
+
+        Cache.update(
+            Cache,
+            f'CUSTOM_TEMP_FILE = """{sushicache.CUSTOM_TEMP_FILE}"""',
+            f'CUSTOM_TEMP_FILE = """{out}"""',
+        )
+
+        return data
+
+    def _extract_if(self):
+        # extracts if statements
+
+        launch = config["launch"]["if_statement"]
+        if config.getboolean("main", "use_templates") is True:
+            launch = sushicache.TEMPLATE_IF_STATEMENT
+        else_start = "$SUSHI_ELSE_START"
+
+        split_string = launch.split(else_start)
+
+        return {"if": split_string[0], "else": split_string[1]}
+
+    def _parse_if(self, data, uuid_data, code):
+        translate_data = {
+            "$SUSHI_ARG_NUM": "1",
+            "$SUSHI_SEMICOLON": ";",
+            "$SUSHI_UUID": uuid_data,
+            "$SUSHI_CODE": code,
+        }
+
+        for i, j in translate_data.items():
+            data = data.replace(i, j)
+
+        return data
+
+    def __init__(self) -> None:
+        rich_print("[bold red]sushi[/bold red]   one compile is still experimental")
+
+        # TODO: implement other cache system
+        try:
+            if sushicache.ONE_COMPILE_CONFIGURED is False:
+                self.setup()
+        except NameError:
+            return
```

### Comparing `sushipy-0.1.7/src/sushipy/utils/verbose_print.py` & `sushipy-0.1.80/src/sushipy/utils/verbose_print.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-"""verbose print"""
-
-import configparser
-
-from rich import print as rich_print
-
-# TODO: maybe move to stores.py
-
-config = configparser.ConfigParser()
-config.read("sushi.conf")
-
-verbose_flag = config["launch"].getboolean("verbose", fallback=False)
-
-
-def verbose_print(message: str):
-    """
-    Prints a verbose message using rich library if the 'verbose' flag is set to True.
-
-    Args:
-        message (str): The message to be printed.
-        verbose (bool): A flag to determine if the message should be printed or not.
-
-    Example:
-        verbose_print("This is a verbose message", verbose=True)
-    """
-    if verbose_flag:
-        rich_print(message)
+"""verbose print"""
+
+import configparser
+
+from rich import print as rich_print
+
+# TODO: maybe move to stores.py
+
+config = configparser.ConfigParser()
+config.read("sushi.conf")
+
+verbose_flag = config["launch"].getboolean("verbose", fallback=False)
+
+
+def verbose_print(message: str):
+    """
+    Prints a verbose message using rich library if the 'verbose' flag is set to True.
+
+    Args:
+        message (str): The message to be printed.
+        verbose (bool): A flag to determine if the message should be printed or not.
+
+    Example:
+        verbose_print("This is a verbose message", verbose=True)
+    """
+    if verbose_flag:
+        rich_print(message)
```

### Comparing `sushipy-0.1.7/src/sushipy.egg-info/SOURCES.txt` & `sushipy-0.1.80/src/sushipy.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 LICENSE
-README.md
 pyproject.toml
-readme.md
-requirements.txt
 setup.cfg
 src/sushipy/__init__.py
 src/sushipy/execute.py
 src/sushipy/git.py
 src/sushipy/index.py
 src/sushipy/main.py
 src/sushipy/one_compile.py
@@ -21,9 +18,10 @@
 src/sushipy/config/__init__.py
 src/sushipy/config/auto_detect.py
 src/sushipy/config/extends.py
 src/sushipy/scripts/git_init.ps1
 src/sushipy/scripts/git_init.sh
 src/sushipy/utils/__init__.py
 src/sushipy/utils/find_dict.py
+src/sushipy/utils/variables.py
 src/sushipy/utils/verbose_print.py
 tests/test_execute.py
```

### Comparing `sushipy-0.1.7/tests/test_execute.py` & `sushipy-0.1.80/tests/test_execute.py`

 * *Files identical despite different names*

