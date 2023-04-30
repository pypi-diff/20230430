# Comparing `tmp/envoy.base.utils-0.4.6.tar.gz` & `tmp/envoy.base.utils-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envoy.base.utils-0.4.6.tar", last modified: Sun Apr 30 12:13:24 2023, max compression
+gzip compressed data, was "envoy.base.utils-0.4.7.tar", last modified: Sun Apr 30 17:55:05 2023, max compression
```

## Comparing `envoy.base.utils-0.4.6.tar` & `envoy.base.utils-0.4.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:13:24.296950 envoy.base.utils-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-30 12:13:24.296950 envoy.base.utils-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:13:24.292950 envoy.base.utils-0.4.6/envoy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:13:24.292950 envoy.base.utils-0.4.6/envoy/base/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:13:24.296950 envoy.base.utils-0.4.6/envoy/base/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:13:24.296950 envoy.base.utils-0.4.6/envoy/base/utils/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/abstract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:13:24.296950 envoy.base.utils-0.4.6/envoy/base/utils/abstract/project/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/abstract/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/abstract/project/changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/abstract/project/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/abstract/project/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/abstract/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/data_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/data_env_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/jinja_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/jinja_env_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/parallel_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/parallel_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/project_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/project_data_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/project_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy/base/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:13:24.296950 envoy.base.utils-0.4.6/envoy.base.utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy.base.utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy.base.utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy.base.utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy.base.utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy.base.utils.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy.base.utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/envoy.base.utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 12:13:24.296950 envoy.base.utils-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-30 12:13:24.000000 envoy.base.utils-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:55:05.319741 envoy.base.utils-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-30 17:55:05.319741 envoy.base.utils-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:55:05.315741 envoy.base.utils-0.4.7/envoy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:55:05.315741 envoy.base.utils-0.4.7/envoy/base/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:55:05.319741 envoy.base.utils-0.4.7/envoy/base/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:55:05.319741 envoy.base.utils-0.4.7/envoy/base/utils/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/abstract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:55:05.319741 envoy.base.utils-0.4.7/envoy/base/utils/abstract/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/abstract/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/abstract/project/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/abstract/project/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/abstract/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/abstract/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/data_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/data_env_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/jinja_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/jinja_env_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/parallel_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/parallel_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/project_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/project_data_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/project_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy/base/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:55:05.315741 envoy.base.utils-0.4.7/envoy.base.utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy.base.utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy.base.utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy.base.utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy.base.utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy.base.utils.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy.base.utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/envoy.base.utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 17:55:05.319741 envoy.base.utils-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-30 17:55:05.000000 envoy.base.utils-0.4.7/setup.py
```

### Comparing `envoy.base.utils-0.4.6/backend_shim.py` & `envoy.base.utils-0.4.7/backend_shim.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.6/envoy/base/utils/__init__.py` & `envoy.base.utils-0.4.7/envoy/base/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.6/envoy/base/utils/abstract/project/changelog.py` & `envoy.base.utils-0.4.7/envoy/base/utils/abstract/project/changelog.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.6/envoy/base/utils/abstract/project/inventory.py` & `envoy.base.utils-0.4.7/envoy/base/utils/abstract/project/inventory.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.6/envoy/base/utils/abstract/project/project.py` & `envoy.base.utils-0.4.7/envoy/base/utils/abstract/project/project.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.6/envoy/base/utils/abstract/protobuf.py` & `envoy.base.utils-0.4.7/envoy/base/utils/abstract/protobuf.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.6/envoy/base/utils/data_env.py` & `envoy.base.utils-0.4.7/envoy/base/utils/data_env.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.6/envoy/base/utils/interface.py` & `envoy.base.utils-0.4.7/envoy/base/utils/interface.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.6/envoy/base/utils/jinja_env.py` & `envoy.base.utils-0.4.7/envoy/base/utils/jinja_env.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.6/envoy/base/utils/parallel_runner.py` & `envoy.base.utils-0.4.7/envoy/base/utils/parallel_runner.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.6/envoy/base/utils/project.py` & `envoy.base.utils-0.4.7/envoy/base/utils/project.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.6/envoy/base/utils/project_runner.py` & `envoy.base.utils-0.4.7/envoy/base/utils/project_runner.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.6/envoy/base/utils/tar.py` & `envoy.base.utils-0.4.7/envoy/base/utils/tar.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 import tarfile
 import tempfile
 from typing import (
     ContextManager, Iterator, Optional, Pattern, Set)
 
 import zstandard
 
-from aio.core import functional
-
 
 # See here for a list of known tar file extensions:
 #   https://en.wikipedia.org/wiki/Tar_(computing)#Suffixes_for_compressed_files
 # not all are listed here, and some extensions may require additional software
 # to handle. This list can be updated as required
 TAR_EXTS: Set[str] = {"tar", "tar.gz", "tar.xz", "tar.bz2", "tar.zst"}
 COMPRESSION_EXTS: Set[str] = {"gz", "bz2", "xz"}
@@ -53,35 +51,33 @@
 
 # Extraction
 
 def extract(
         path: pathlib.Path | str,
         *tarballs: pathlib.Path | str,
         matching: Optional[Pattern[str]] = None,
-        mappings: Optional[dict[str, str]] = None) -> pathlib.Path:
+        mappings: Optional[dict[str, str]] = None,
+        inmem: bool = True) -> pathlib.Path:
     if not tarballs:
         raise ExtractError(f"No tarballs specified for extraction to {path}")
-    openers = functional.nested(
-        *tuple(_open(tarball) for tarball in tarballs))
     path = pathlib.Path(path)
-
-    with openers as tarfiles:
-        for prefix, tar in tarfiles:
+    for tarball in tarballs:
+        with _open(tarball, inmem) as (prefix, tar):
             _extract(path, prefix, tar, matching, mappings)
-
     _mv_paths(path, mappings)
     _rm_paths(path, matching)
     return path
 
 
 @contextlib.contextmanager
 def untar(
         *tarballs: pathlib.Path | str,
         matching: Optional[Pattern[str]] = None,
-        mappings: Optional[dict[str, str]] = None) -> Iterator[pathlib.Path]:
+        mappings: Optional[dict[str, str]] = None,
+        inmem: bool = True) -> Iterator[pathlib.Path]:
     """Untar a tarball into a temporary directory.
 
     for example to list the contents of a tarball:
 
     ```
     import os
 
@@ -96,15 +92,16 @@
     the created temp directory will be cleaned up on
     exiting the contextmanager
     """
     with tempfile.TemporaryDirectory() as tmpdir:
         yield extract(
             tmpdir, *tarballs,
             matching=matching,
-            mappings=mappings)
+            mappings=mappings,
+            inmem=inmem)
 
 
 def _extract(
         path: pathlib.Path,
         prefix: str,
         tar: tarfile.TarFile,
         matching: Optional[Pattern[str]],
@@ -112,63 +109,71 @@
     if not matching:
         tar.extractall(path=path.joinpath(prefix))
         return
     for member in tar.getmembers():
         if _should_extract(member, matching, mappings):
             tar.extract(
                 member,
-                path=path.joinpath(prefix).joinpath(member.name))
+                path=path.joinpath(prefix))
 
 
 def _mv_paths(path: pathlib.Path, mappings: Optional[dict[str, str]]) -> None:
     for src, dest in (mappings or {}).items():
         src_path = path.joinpath(src)
         dest_path = path.joinpath(dest)
         dest_path.parent.mkdir(exist_ok=True, parents=True)
         shutil.move(src_path, dest_path)
 
 
 def _open(
-        path: pathlib.Path | str) -> (
+        path: pathlib.Path | str,
+        inmem: bool = True) -> (
             ContextManager[tuple[str, tarfile.TarFile]]):
     """For a given tarball path if it contains `:` split prefix, path,
     otherwise prefix is empty.
 
     If the tarfile is `tar.zst` use zstd to decompress.
 
     Return prefix, and opened tarfile for path.
     """
     _path = str(path)
     prefix, _path = (
         _path.split(":")
         if ":" in _path
         else ("", _path))
     return (
-        _opener(_open_zst(_path), prefix)
+        _opener(_open_zst(_path, inmem), prefix)
         if _path.endswith(".zst")
         else _opener(tarfile.open(_path), prefix))
 
 
-def _open_zst(path: pathlib.Path | str) -> tarfile.TarFile:
+def _open_zst(
+        path: pathlib.Path | str,
+        inmem: bool = True) -> tarfile.TarFile:
     """extract .zst file."""
     archive = pathlib.Path(path).expanduser()
     dctx = zstandard.ZstdDecompressor()
-    outfile = io.BytesIO()
+    outfile = (
+        io.BytesIO()
+        if inmem
+        else tempfile.TemporaryFile(suffix=".tar"))
     with archive.open("rb") as infile:
         dctx.copy_stream(infile, outfile)
     outfile.seek(0)
     return tarfile.open(fileobj=outfile)
 
 
 @contextlib.contextmanager
 def _opener(
         tarball: tarfile.TarFile,
         prefix: str = "") -> Iterator[tuple[str, tarfile.TarFile]]:
     with tarball as t:
         yield prefix, t
+        if "fileobj" in t.__dict__:
+            t.__dict__["fileobj"].close()
 
 
 def _rm_paths(path: pathlib.Path, matching: Optional[Pattern[str]]):
     if not matching:
         return
     for sub in path.glob("*"):
         if not matching.match(sub.name):
@@ -234,11 +239,14 @@
 
 @contextlib.contextmanager
 def repack(
         out: str | pathlib.Path,
         *paths: str | pathlib.Path,
         matching: Optional[Pattern[str]] = None,
         mappings: Optional[dict[str, str]] = None,
-        include: Optional[Pattern[str]] = None) -> Iterator[pathlib.Path]:
-    with untar(*paths, matching=matching, mappings=mappings) as tardir:
+        include: Optional[Pattern[str]] = None,
+        inmem: bool = True) -> Iterator[pathlib.Path]:
+    extracted = untar(
+        *paths, matching=matching, mappings=mappings, inmem=inmem)
+    with extracted as tardir:
         yield tardir
         pack(tardir, out, include=include)
```

### Comparing `envoy.base.utils-0.4.6/envoy/base/utils/typing.py` & `envoy.base.utils-0.4.7/envoy/base/utils/typing.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.6/envoy/base/utils/utils.py` & `envoy.base.utils-0.4.7/envoy/base/utils/utils.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.6/envoy/base/utils/yaml.py` & `envoy.base.utils-0.4.7/envoy/base/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.6/envoy.base.utils.egg-info/SOURCES.txt` & `envoy.base.utils-0.4.7/envoy.base.utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.6/setup.py` & `envoy.base.utils-0.4.7/setup.py`

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
-    'version': '0.4.6',
+    'version': '0.4.7',
 })
```

