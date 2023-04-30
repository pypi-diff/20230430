# Comparing `tmp/nonebot-desktop-wing-0.2.6.tar.gz` & `tmp/nonebot-desktop-wing-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-desktop-wing-0.2.6.tar", last modified: Sun Apr 30 14:41:18 2023, max compression
+gzip compressed data, was "nonebot-desktop-wing-0.2.7.tar", last modified: Sun Apr 30 16:04:06 2023, max compression
```

## Comparing `nonebot-desktop-wing-0.2.6.tar` & `nonebot-desktop-wing-0.2.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:41:18.621738 nonebot-desktop-wing-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-30 14:41:07.000000 nonebot-desktop-wing-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-30 14:41:18.621738 nonebot-desktop-wing-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-30 14:41:07.000000 nonebot-desktop-wing-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:41:18.621738 nonebot-desktop-wing-0.2.6/nonebot_desktop_wing/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-30 14:41:07.000000 nonebot-desktop-wing-0.2.6/nonebot_desktop_wing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-30 14:41:07.000000 nonebot-desktop-wing-0.2.6/nonebot_desktop_wing/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-30 14:41:07.000000 nonebot-desktop-wing-0.2.6/nonebot_desktop_wing/hindsight.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-30 14:41:07.000000 nonebot-desktop-wing-0.2.6/nonebot_desktop_wing/lazylib.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-30 14:41:07.000000 nonebot-desktop-wing-0.2.6/nonebot_desktop_wing/lazylib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-04-30 14:41:07.000000 nonebot-desktop-wing-0.2.6/nonebot_desktop_wing/molecules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-30 14:41:07.000000 nonebot-desktop-wing-0.2.6/nonebot_desktop_wing/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-30 14:41:07.000000 nonebot-desktop-wing-0.2.6/nonebot_desktop_wing/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:41:18.621738 nonebot-desktop-wing-0.2.6/nonebot_desktop_wing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-30 14:41:18.000000 nonebot-desktop-wing-0.2.6/nonebot_desktop_wing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-30 14:41:18.000000 nonebot-desktop-wing-0.2.6/nonebot_desktop_wing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 14:41:18.000000 nonebot-desktop-wing-0.2.6/nonebot_desktop_wing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-30 14:41:18.000000 nonebot-desktop-wing-0.2.6/nonebot_desktop_wing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-30 14:41:18.000000 nonebot-desktop-wing-0.2.6/nonebot_desktop_wing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-30 14:41:07.000000 nonebot-desktop-wing-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 14:41:18.621738 nonebot-desktop-wing-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:04:06.284386 nonebot-desktop-wing-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-30 16:03:55.000000 nonebot-desktop-wing-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-30 16:04:06.284386 nonebot-desktop-wing-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-30 16:03:55.000000 nonebot-desktop-wing-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:04:06.284386 nonebot-desktop-wing-0.2.7/nonebot_desktop_wing/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-30 16:03:55.000000 nonebot-desktop-wing-0.2.7/nonebot_desktop_wing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-30 16:03:55.000000 nonebot-desktop-wing-0.2.7/nonebot_desktop_wing/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-30 16:03:55.000000 nonebot-desktop-wing-0.2.7/nonebot_desktop_wing/hindsight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-30 16:03:55.000000 nonebot-desktop-wing-0.2.7/nonebot_desktop_wing/lazylib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-30 16:03:55.000000 nonebot-desktop-wing-0.2.7/nonebot_desktop_wing/lazylib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-04-30 16:03:55.000000 nonebot-desktop-wing-0.2.7/nonebot_desktop_wing/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-30 16:03:55.000000 nonebot-desktop-wing-0.2.7/nonebot_desktop_wing/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-30 16:03:55.000000 nonebot-desktop-wing-0.2.7/nonebot_desktop_wing/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:04:06.284386 nonebot-desktop-wing-0.2.7/nonebot_desktop_wing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-30 16:04:06.000000 nonebot-desktop-wing-0.2.7/nonebot_desktop_wing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-30 16:04:06.000000 nonebot-desktop-wing-0.2.7/nonebot_desktop_wing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 16:04:06.000000 nonebot-desktop-wing-0.2.7/nonebot_desktop_wing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-30 16:04:06.000000 nonebot-desktop-wing-0.2.7/nonebot_desktop_wing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-30 16:04:06.000000 nonebot-desktop-wing-0.2.7/nonebot_desktop_wing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-30 16:03:55.000000 nonebot-desktop-wing-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 16:04:06.284386 nonebot-desktop-wing-0.2.7/setup.cfg
```

### Comparing `nonebot-desktop-wing-0.2.6/LICENSE` & `nonebot-desktop-wing-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.6/PKG-INFO` & `nonebot-desktop-wing-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-desktop-wing
-Version: 0.2.6
+Version: 0.2.7
 Summary: Wings for NoneBot desktop applications.
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonedesktop/nonebot-desktop-wing
 Project-URL: Repository, https://github.com/nonedesktop/nonebot-desktop-wing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nonebot-desktop-wing-0.2.6/README.md` & `nonebot-desktop-wing-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.6/nonebot_desktop_wing/__init__.py` & `nonebot-desktop-wing-0.2.7/nonebot_desktop_wing/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.6/nonebot_desktop_wing/constants.py` & `nonebot-desktop-wing-0.2.7/nonebot_desktop_wing/constants.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.6/nonebot_desktop_wing/hindsight.py` & `nonebot-desktop-wing-0.2.7/nonebot_desktop_wing/hindsight.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.6/nonebot_desktop_wing/lazylib.py` & `nonebot-desktop-wing-0.2.7/nonebot_desktop_wing/lazylib.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.6/nonebot_desktop_wing/lazylib.pyi` & `nonebot-desktop-wing-0.2.7/nonebot_desktop_wing/lazylib.pyi`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.6/nonebot_desktop_wing/molecules.py` & `nonebot-desktop-wing-0.2.7/nonebot_desktop_wing/molecules.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from __future__ import annotations
 import os
 from pathlib import Path
-import shlex
 from shutil import which
 import subprocess
 from tempfile import mkstemp
 from threading import Lock
 from types import ModuleType
-from typing import List, Literal, Optional, Tuple, TypeVar, Union, overload
+from typing import (
+    Iterable, List, Literal, Optional, Tuple, TypeVar, Union, overload
+)
 
 from nonebot_desktop_wing.constants import LINUX_TERMINALS, WINDOWS
 
 _import_lock = Lock()
 T = TypeVar("T")
 
 
+def anojoin(args: Iterable[str]) -> str:
+    """Like `shlex.join`, but uses dquote (`"`) instead of squote (`'`)."""
+    dq, cdq = "\"", "\\\""
+    return " ".join([f"\"{s.replace(dq, cdq)}\"" for s in args])
+
+
 def import_with_lock(
     name: str,
     package: Optional[str] = None
 ) -> ModuleType:
     """Like `importlib.import_module(...)`, but using a lock to avoid
     conflicts when importing package.
     """
@@ -116,15 +123,15 @@
                                       stderr.
 
     - return: `(Popen[bytes], str)` - the process running commands and temp
                                       script path.
     """
     sname = gen_run_script(cmd, cwd)
     return subprocess.Popen(
-        shlex.join((*get_terminal_starter(), sname)), shell=True,
+        anojoin((*get_terminal_starter(), sname)), shell=True,
         stdout=subprocess.PIPE if catch_output else None,
         stderr=subprocess.STDOUT if catch_output else None
     ), sname
 
 
 def exec_new_win(
     cmd: str, cwd: Union[str, Path, None] = None
@@ -136,30 +143,30 @@
     - cwd: `Union[str, Path, None]` - the first work directory to be set.
 
     - return: `(Popen[bytes], str)` - the process running commands and temp
                                       script path.
     """
     sname = gen_run_script(cmd, cwd)
     return subprocess.Popen(
-        shlex.join((*get_terminal_starter(), sname)), shell=True,
+        anojoin((*get_terminal_starter(), sname)), shell=True,
     ), sname
 
 
 def open_new_win(
     cwd: Union[str, Path, None] = None
 ) -> subprocess.Popen[bytes]:
     """
     Open a new terminal window.
 
     - cwd: `Union[str, Path, None]` - the first work directory to be set.
 
     - return: `Popen[bytes]`        - the process running new window.
     """
     return subprocess.Popen(
-        shlex.join(get_terminal_starter_pure()), shell=True, cwd=cwd
+        anojoin(get_terminal_starter_pure()), shell=True, cwd=cwd
     )
 
 
 def system_open(
     fp: Union[str, Path], *, catch_output: bool = False
 ) -> subprocess.Popen[bytes]:
     """
@@ -167,15 +174,15 @@
 
     - fp: `Union[str, Path]`    - a file path or URI.
     - catch_output: `bool`      - whether to catch output stdout and stderr.
 
     - return: `Popen[bytes]`    - the process running external applications.
     """
     return subprocess.Popen(
-        shlex.join(("start" if WINDOWS else "xdg-open", str(fp))), shell=True,
+        anojoin(("start" if WINDOWS else "xdg-open", str(fp))), shell=True,
         stdout=subprocess.PIPE if catch_output else None,
         stderr=subprocess.STDOUT if catch_output else None
     )
 
 
 @overload
 def perform_pip_command(
@@ -213,15 +220,15 @@
     cmd = [pyexec, "-m", "pip", command, *args]
     if not new_win:
         return subprocess.Popen(
             cmd,
             stdout=subprocess.PIPE if catch_output else None,
             stderr=subprocess.STDOUT if catch_output else None
         )
-    return exec_new_win(shlex.join(cmd))
+    return exec_new_win(anojoin(cmd))
 
 
 @overload
 def perform_pip_install(
     pyexec: str, *packages: str, update: bool = False, index: str = "",
     new_win: Literal[False] = False, catch_output: bool = False
 ) -> subprocess.Popen[bytes]:
```

### Comparing `nonebot-desktop-wing-0.2.6/nonebot_desktop_wing/project.py` & `nonebot-desktop-wing-0.2.7/nonebot_desktop_wing/project.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.6/nonebot_desktop_wing/resources.py` & `nonebot-desktop-wing-0.2.7/nonebot_desktop_wing/resources.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.6/nonebot_desktop_wing.egg-info/PKG-INFO` & `nonebot-desktop-wing-0.2.7/nonebot_desktop_wing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-desktop-wing
-Version: 0.2.6
+Version: 0.2.7
 Summary: Wings for NoneBot desktop applications.
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonedesktop/nonebot-desktop-wing
 Project-URL: Repository, https://github.com/nonedesktop/nonebot-desktop-wing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nonebot-desktop-wing-0.2.6/nonebot_desktop_wing.egg-info/SOURCES.txt` & `nonebot-desktop-wing-0.2.7/nonebot_desktop_wing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.6/pyproject.toml` & `nonebot-desktop-wing-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-desktop-wing"
-version = "0.2.6"
+version = "0.2.7"
 description = "Wings for NoneBot desktop applications."
 authors = [
     {name = "HivertMoZara", email = "worldmozara@163.com"},
 ]
 license = {text = "MIT"}
 dependencies = ["nb_cli~=1.0.0", "python-dotenv~=1.0.0", "httpx>=0.23", "typing-extensions>=4.5.0"]
 requires-python = ">=3.8"
```

