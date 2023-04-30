# Comparing `tmp/envoy.base.utils-0.4.5.tar.gz` & `tmp/envoy.base.utils-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envoy.base.utils-0.4.5.tar", last modified: Sun Apr 30 09:41:15 2023, max compression
+gzip compressed data, was "envoy.base.utils-0.4.6.tar", last modified: Sun Apr 30 12:13:24 2023, max compression
```

## Comparing `envoy.base.utils-0.4.5.tar` & `envoy.base.utils-0.4.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:41:15.873685 envoy.base.utils-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-30 09:41:15.873685 envoy.base.utils-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:41:15.869685 envoy.base.utils-0.4.5/envoy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:41:15.869685 envoy.base.utils-0.4.5/envoy/base/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:41:15.873685 envoy.base.utils-0.4.5/envoy/base/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:41:15.873685 envoy.base.utils-0.4.5/envoy/base/utils/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/abstract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:41:15.873685 envoy.base.utils-0.4.5/envoy/base/utils/abstract/project/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/abstract/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/abstract/project/changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/abstract/project/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/abstract/project/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/abstract/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/data_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/data_env_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/jinja_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/jinja_env_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/parallel_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/parallel_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/project_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/project_data_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/project_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:41:15.869685 envoy.base.utils-0.4.5/envoy.base.utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy.base.utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy.base.utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy.base.utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy.base.utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy.base.utils.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy.base.utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy.base.utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 09:41:15.873685 envoy.base.utils-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:13:24.296950 envoy.base.utils-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-30 12:13:24.296950 envoy.base.utils-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:13:24.292950 envoy.base.utils-0.4.6/envoy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:13:24.292950 envoy.base.utils-0.4.6/envoy/base/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:13:24.296950 envoy.base.utils-0.4.6/envoy/base/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:13:24.296950 envoy.base.utils-0.4.6/envoy/base/utils/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/abstract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:13:24.296950 envoy.base.utils-0.4.6/envoy/base/utils/abstract/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/abstract/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/abstract/project/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/abstract/project/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/abstract/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/abstract/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/data_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/data_env_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/jinja_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/jinja_env_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/parallel_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/parallel_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/project_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/project_data_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/project_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:13:24.296950 envoy.base.utils-0.4.6/envoy.base.utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy.base.utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy.base.utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy.base.utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy.base.utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy.base.utils.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy.base.utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy.base.utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 12:13:24.296950 envoy.base.utils-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/setup.py
```

### Comparing `envoy.base.utils-0.4.5/backend_shim.py` & `envoy.base.utils-0.4.6/backend_shim.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.5/envoy/base/utils/__init__.py` & `envoy.base.utils-0.4.6/envoy/base/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 from .exceptions import TypeCastingError
 from .tar import (
     extract,
     ExtractError,
     is_tarlike,
     pack,
+    repack,
     TAR_EXTS,
     tar_mode,
     untar)
 from .utils import (
     async_list,
     cd_and_return,
     dt_to_utc_isoformat,
@@ -18,15 +19,17 @@
     increment_version,
     coverage_with_data_file,
     minor_version_for,
     typed,
     to_yaml,
     to_bytes,
     is_sha,
-    last_n_bytes_of)
+    last_n_bytes_of,
+    tuple_pair,
+    TuplePairError)
 from . import interface, typing
 from .parallel_cmd import parallel_cmd
 from .parallel_runner import ParallelRunner
 from .project import Changelog, ChangelogEntry, Changelogs, Project
 from .project_cmd import project_cmd
 from .project_data_cmd import project_data_cmd
 from .project_runner import ProjectDataRunner, ProjectRunner
@@ -69,15 +72,18 @@
     "Project",
     "ProjectDataRunner",
     "ProjectRunner",
     "project_cmd",
     "project_data_cmd",
     "ProtobufSet",
     "ProtobufValidator",
+    "repack",
     "typed",
     "untar",
     "TAR_EXTS",
     "tar_mode",
     "to_bytes",
     "to_yaml",
+    "tuple_pair",
+    "TuplePairError",
     "TypeCastingError",
     "typing")
```

### Comparing `envoy.base.utils-0.4.5/envoy/base/utils/abstract/project/changelog.py` & `envoy.base.utils-0.4.6/envoy/base/utils/abstract/project/changelog.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.5/envoy/base/utils/abstract/project/inventory.py` & `envoy.base.utils-0.4.6/envoy/base/utils/abstract/project/inventory.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.5/envoy/base/utils/abstract/project/project.py` & `envoy.base.utils-0.4.6/envoy/base/utils/abstract/project/project.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.5/envoy/base/utils/abstract/protobuf.py` & `envoy.base.utils-0.4.6/envoy/base/utils/abstract/protobuf.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.5/envoy/base/utils/data_env.py` & `envoy.base.utils-0.4.6/envoy/base/utils/data_env.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.5/envoy/base/utils/interface.py` & `envoy.base.utils-0.4.6/envoy/base/utils/interface.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.5/envoy/base/utils/jinja_env.py` & `envoy.base.utils-0.4.6/envoy/base/utils/jinja_env.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.5/envoy/base/utils/parallel_runner.py` & `envoy.base.utils-0.4.6/envoy/base/utils/parallel_runner.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.5/envoy/base/utils/project.py` & `envoy.base.utils-0.4.6/envoy/base/utils/project.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.5/envoy/base/utils/project_runner.py` & `envoy.base.utils-0.4.6/envoy/base/utils/project_runner.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.5/envoy/base/utils/tar.py` & `envoy.base.utils-0.4.6/envoy/base/utils/tar.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import contextlib
 import io
 import pathlib
 import shutil
 import tarfile
 import tempfile
 from typing import (
-    ContextManager, Iterator, Optional, Pattern, Set, Union)
+    ContextManager, Iterator, Optional, Pattern, Set)
 
 import zstandard
 
 from aio.core import functional
 
 
 # See here for a list of known tar file extensions:
@@ -30,36 +30,36 @@
 COMPRESSION_EXTS: Set[str] = {"gz", "bz2", "xz"}
 
 
 class ExtractError(Exception):
     pass
 
 
-def is_tarlike(path: Union[pathlib.Path, str]) -> bool:
+def is_tarlike(path: pathlib.Path | str) -> bool:
     """Returns a bool based on whether a file looks like a tar file depending
     on its file extension.
 
     This allows for a provided path to save to, to dynamically be either
     considered a directory (to create) or a tar file (to create).
     """
     return any(str(path).endswith(ext) for ext in TAR_EXTS)
 
 
-def tar_mode(path: Union[pathlib.Path, str], mode="r") -> str:
+def tar_mode(path: pathlib.Path | str, mode="r") -> str:
     for suffix in COMPRESSION_EXTS:
         if str(path).endswith(f".{suffix}"):
             return f"{mode}:{suffix}"
     return mode
 
 
 # Extraction
 
 def extract(
-        path: Union[pathlib.Path, str],
-        *tarballs: Union[pathlib.Path, str],
+        path: pathlib.Path | str,
+        *tarballs: pathlib.Path | str,
         matching: Optional[Pattern[str]] = None,
         mappings: Optional[dict[str, str]] = None) -> pathlib.Path:
     if not tarballs:
         raise ExtractError(f"No tarballs specified for extraction to {path}")
     openers = functional.nested(
         *tuple(_open(tarball) for tarball in tarballs))
     path = pathlib.Path(path)
@@ -71,15 +71,15 @@
     _mv_paths(path, mappings)
     _rm_paths(path, matching)
     return path
 
 
 @contextlib.contextmanager
 def untar(
-        *tarballs: Union[pathlib.Path, str],
+        *tarballs: pathlib.Path | str,
         matching: Optional[Pattern[str]] = None,
         mappings: Optional[dict[str, str]] = None) -> Iterator[pathlib.Path]:
     """Untar a tarball into a temporary directory.
 
     for example to list the contents of a tarball:
 
     ```
@@ -184,30 +184,61 @@
         or (member.name in (mappings or {})))
 
 
 # Packing
 
 def pack(
         path: str | pathlib.Path,
-        out: str | pathlib.Path) -> None:
-    (_pack_zst(path, out)
+        out: str | pathlib.Path,
+        include: Optional[Pattern[str]] = None) -> None:
+    (_pack_zst(path, out, include=include)
      if str(out).endswith(".zst")
-     else _pack(path, out))
+     else _pack(path, out, include=include))
 
 
 def _pack(
         path: str | pathlib.Path,
-        out: str | pathlib.Path) -> None:
+        out: str | pathlib.Path,
+        include: Optional[Pattern[str]] = None) -> None:
     with tarfile.open(out, mode=tar_mode(out, mode="w")) as tar:
-        tar.add(path, arcname=".")
+        tar.add(_prune(path, include), arcname=".")
 
 
 def _pack_zst(
         path: str | pathlib.Path,
-        out: str | pathlib.Path) -> None:
+        out: str | pathlib.Path,
+        include: Optional[Pattern[str]] = None) -> None:
     tarout = io.BytesIO()
     cctx = zstandard.ZstdCompressor(threads=-1)
     with tarfile.open(fileobj=tarout, mode="w") as tar:
-        tar.add(path, arcname=".")
+        tar.add(_prune(path, include), arcname=".")
         tarout.seek(0)
         with open(out, "wb") as writeout:
             cctx.copy_stream(tarout, writeout)
+
+
+def _prune(
+        path: str | pathlib.Path,
+        include: Optional[Pattern[str]] = None) -> pathlib.Path:
+    path = pathlib.Path(path)
+    if not include:
+        return path
+    for sub in path.glob("*"):
+        if not include.match(sub.name):
+            (shutil.rmtree(sub)
+             if sub.is_dir()
+             else sub.unlink())
+    return path
+
+
+# Repacking
+
+@contextlib.contextmanager
+def repack(
+        out: str | pathlib.Path,
+        *paths: str | pathlib.Path,
+        matching: Optional[Pattern[str]] = None,
+        mappings: Optional[dict[str, str]] = None,
+        include: Optional[Pattern[str]] = None) -> Iterator[pathlib.Path]:
+    with untar(*paths, matching=matching, mappings=mappings) as tardir:
+        yield tardir
+        pack(tardir, out, include=include)
```

### Comparing `envoy.base.utils-0.4.5/envoy/base/utils/typing.py` & `envoy.base.utils-0.4.6/envoy/base/utils/typing.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.5/envoy/base/utils/utils.py` & `envoy.base.utils-0.4.6/envoy/base/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -163,7 +163,20 @@
 def increment_version(
         version: _version.Version,
         patch: bool = False) -> _version.Version:
     return _version.Version(
         f"{version.major}.{version.minor}.{version.micro + 1}"
         if patch
         else f"{version.major}.{version.minor + 1}.{version.micro}")
+
+
+class TuplePairError(Exception):
+    pass
+
+
+def tuple_pair(input: str, separator: str = ":") -> tuple[str, str]:
+    """This allows dict generators to split items and pass type checking."""
+    pair = input.split(separator)
+    if len(pair) != 2:
+        raise TuplePairError(
+            f"Provided string did not split ({separator}) in 2: {input}")
+    return pair[0], pair[1]
```

### Comparing `envoy.base.utils-0.4.5/envoy/base/utils/yaml.py` & `envoy.base.utils-0.4.6/envoy/base/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.5/envoy.base.utils.egg-info/SOURCES.txt` & `envoy.base.utils-0.4.6/envoy.base.utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.5/setup.py` & `envoy.base.utils-0.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,9 +53,9 @@
     'packages': (
         'envoy.base.utils',
         'envoy.base.utils.abstract',
         'envoy.base.utils.abstract.project',
     ),
     'python_requires': '>=3.10.0',
     'url': 'https://github.com/envoyproxy/pytooling/tree/main/envoy.base.utils',
-    'version': '0.4.5',
+    'version': '0.4.6',
 })
```

