# Comparing `tmp/envoy.base.utils-0.4.4.tar.gz` & `tmp/envoy.base.utils-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envoy.base.utils-0.4.4.tar", last modified: Sat Apr 29 13:59:38 2023, max compression
+gzip compressed data, was "envoy.base.utils-0.4.5.tar", last modified: Sun Apr 30 09:41:15 2023, max compression
```

## Comparing `envoy.base.utils-0.4.4.tar` & `envoy.base.utils-0.4.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:38.758401 envoy.base.utils-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-29 13:59:38.758401 envoy.base.utils-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:38.750400 envoy.base.utils-0.4.4/envoy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:38.750400 envoy.base.utils-0.4.4/envoy/base/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:38.758401 envoy.base.utils-0.4.4/envoy/base/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:38.758401 envoy.base.utils-0.4.4/envoy/base/utils/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/abstract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:38.758401 envoy.base.utils-0.4.4/envoy/base/utils/abstract/project/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/abstract/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/abstract/project/changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/abstract/project/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/abstract/project/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/abstract/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/data_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/data_env_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/jinja_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/jinja_env_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/parallel_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/parallel_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/project_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/project_data_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/project_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:38.754401 envoy.base.utils-0.4.4/envoy.base.utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy.base.utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy.base.utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy.base.utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy.base.utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy.base.utils.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy.base.utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy.base.utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 13:59:38.758401 envoy.base.utils-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:41:15.873685 envoy.base.utils-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-30 09:41:15.873685 envoy.base.utils-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:41:15.869685 envoy.base.utils-0.4.5/envoy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:41:15.869685 envoy.base.utils-0.4.5/envoy/base/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:41:15.873685 envoy.base.utils-0.4.5/envoy/base/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:41:15.873685 envoy.base.utils-0.4.5/envoy/base/utils/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/abstract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:41:15.873685 envoy.base.utils-0.4.5/envoy/base/utils/abstract/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/abstract/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/abstract/project/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/abstract/project/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/abstract/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/abstract/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/data_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/data_env_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/jinja_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/jinja_env_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/parallel_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/parallel_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/project_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/project_data_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/project_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy/base/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:41:15.869685 envoy.base.utils-0.4.5/envoy.base.utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy.base.utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy.base.utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy.base.utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy.base.utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy.base.utils.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy.base.utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/envoy.base.utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 09:41:15.873685 envoy.base.utils-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-30 09:41:15.000000 envoy.base.utils-0.4.5/setup.py
```

### Comparing `envoy.base.utils-0.4.4/backend_shim.py` & `envoy.base.utils-0.4.5/backend_shim.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.4/envoy/base/utils/__init__.py` & `envoy.base.utils-0.4.5/envoy/base/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 from .exceptions import TypeCastingError
 from .tar import (
     extract,
     ExtractError,
     is_tarlike,
+    pack,
     TAR_EXTS,
     tar_mode,
     untar)
 from .utils import (
     async_list,
     cd_and_return,
     dt_to_utc_isoformat,
@@ -57,14 +58,15 @@
     "is_sha",
     "is_tarlike",
     "JinjaEnvironment",
     "jinja_env_cmd",
     "last_n_bytes_of",
     "coverage_with_data_file",
     "minor_version_for",
+    "pack",
     "Parallel",
     "ParallelRunner",
     "parallel_cmd",
     "Project",
     "ProjectDataRunner",
     "ProjectRunner",
     "project_cmd",
```

### Comparing `envoy.base.utils-0.4.4/envoy/base/utils/abstract/project/changelog.py` & `envoy.base.utils-0.4.5/envoy/base/utils/abstract/project/changelog.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.4/envoy/base/utils/abstract/project/inventory.py` & `envoy.base.utils-0.4.5/envoy/base/utils/abstract/project/inventory.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.4/envoy/base/utils/abstract/project/project.py` & `envoy.base.utils-0.4.5/envoy/base/utils/abstract/project/project.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.4/envoy/base/utils/abstract/protobuf.py` & `envoy.base.utils-0.4.5/envoy/base/utils/abstract/protobuf.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.4/envoy/base/utils/data_env.py` & `envoy.base.utils-0.4.5/envoy/base/utils/data_env.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.4/envoy/base/utils/interface.py` & `envoy.base.utils-0.4.5/envoy/base/utils/interface.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.4/envoy/base/utils/jinja_env.py` & `envoy.base.utils-0.4.5/envoy/base/utils/jinja_env.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.4/envoy/base/utils/parallel_runner.py` & `envoy.base.utils-0.4.5/envoy/base/utils/parallel_runner.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.4/envoy/base/utils/project.py` & `envoy.base.utils-0.4.5/envoy/base/utils/project.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.4/envoy/base/utils/project_runner.py` & `envoy.base.utils-0.4.5/envoy/base/utils/project_runner.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.4/envoy/base/utils/tar.py` & `envoy.base.utils-0.4.5/envoy/base/utils/tar.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 #
 # Provides tar utils:
 #   multi-path extraction, zst support, filtering
 #
 
+# TODO:
+# - improve the inconsistent api here
+# - use asyncio and move to aio.core
+# - remove zst when https://bugs.python.org/issue37095 is resolved
+
 import contextlib
 import io
 import pathlib
 import shutil
 import tarfile
 import tempfile
 from typing import (
@@ -18,14 +23,15 @@
 
 
 # See here for a list of known tar file extensions:
 #   https://en.wikipedia.org/wiki/Tar_(computing)#Suffixes_for_compressed_files
 # not all are listed here, and some extensions may require additional software
 # to handle. This list can be updated as required
 TAR_EXTS: Set[str] = {"tar", "tar.gz", "tar.xz", "tar.bz2", "tar.zst"}
+COMPRESSION_EXTS: Set[str] = {"gz", "bz2", "xz"}
 
 
 class ExtractError(Exception):
     pass
 
 
 def is_tarlike(path: Union[pathlib.Path, str]) -> bool:
@@ -35,16 +41,15 @@
     This allows for a provided path to save to, to dynamically be either
     considered a directory (to create) or a tar file (to create).
     """
     return any(str(path).endswith(ext) for ext in TAR_EXTS)
 
 
 def tar_mode(path: Union[pathlib.Path, str], mode="r") -> str:
-    suffixes = ["gz", "bz2", "xz"]
-    for suffix in suffixes:
+    for suffix in COMPRESSION_EXTS:
         if str(path).endswith(f".{suffix}"):
             return f"{mode}:{suffix}"
     return mode
 
 
 # Extraction
 
@@ -173,7 +178,36 @@
 def _should_extract(
         member: tarfile.TarInfo,
         matching: Optional[Pattern[str]] = None,
         mappings: Optional[dict[str, str]] = None) -> bool:
     return bool(
         (matching and matching.match(member.name))
         or (member.name in (mappings or {})))
+
+
+# Packing
+
+def pack(
+        path: str | pathlib.Path,
+        out: str | pathlib.Path) -> None:
+    (_pack_zst(path, out)
+     if str(out).endswith(".zst")
+     else _pack(path, out))
+
+
+def _pack(
+        path: str | pathlib.Path,
+        out: str | pathlib.Path) -> None:
+    with tarfile.open(out, mode=tar_mode(out, mode="w")) as tar:
+        tar.add(path, arcname=".")
+
+
+def _pack_zst(
+        path: str | pathlib.Path,
+        out: str | pathlib.Path) -> None:
+    tarout = io.BytesIO()
+    cctx = zstandard.ZstdCompressor(threads=-1)
+    with tarfile.open(fileobj=tarout, mode="w") as tar:
+        tar.add(path, arcname=".")
+        tarout.seek(0)
+        with open(out, "wb") as writeout:
+            cctx.copy_stream(tarout, writeout)
```

### Comparing `envoy.base.utils-0.4.4/envoy/base/utils/typing.py` & `envoy.base.utils-0.4.5/envoy/base/utils/typing.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.4/envoy/base/utils/utils.py` & `envoy.base.utils-0.4.5/envoy/base/utils/utils.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.4/envoy/base/utils/yaml.py` & `envoy.base.utils-0.4.5/envoy/base/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.4/envoy.base.utils.egg-info/SOURCES.txt` & `envoy.base.utils-0.4.5/envoy.base.utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.4/setup.py` & `envoy.base.utils-0.4.5/setup.py`

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
-    'version': '0.4.4',
+    'version': '0.4.5',
 })
```

