# Comparing `tmp/envoy.gpg.sign-0.1.1.tar.gz` & `tmp/envoy.gpg.sign-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envoy.gpg.sign-0.1.1.tar", last modified: Mon Jan 30 12:54:23 2023, max compression
+gzip compressed data, was "envoy.gpg.sign-0.2.0.tar", last modified: Sun Apr 30 18:23:05 2023, max compression
```

## Comparing `envoy.gpg.sign-0.1.1.tar` & `envoy.gpg.sign-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 12:54:23.517803 envoy.gpg.sign-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-30 12:54:23.000000 envoy.gpg.sign-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-01-30 12:54:23.517803 envoy.gpg.sign-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-01-30 12:54:23.000000 envoy.gpg.sign-0.1.1/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 12:54:23.513803 envoy.gpg.sign-0.1.1/envoy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 12:54:23.513803 envoy.gpg.sign-0.1.1/envoy/gpg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 12:54:23.517803 envoy.gpg.sign-0.1.1/envoy/gpg/sign/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-01-30 12:54:23.000000 envoy.gpg.sign-0.1.1/envoy/gpg/sign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-01-30 12:54:23.000000 envoy.gpg.sign-0.1.1/envoy/gpg/sign/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-01-30 12:54:23.000000 envoy.gpg.sign-0.1.1/envoy/gpg/sign/deb.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-30 12:54:23.000000 envoy.gpg.sign-0.1.1/envoy/gpg/sign/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 12:54:23.000000 envoy.gpg.sign-0.1.1/envoy/gpg/sign/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-01-30 12:54:23.000000 envoy.gpg.sign-0.1.1/envoy/gpg/sign/rpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-01-30 12:54:23.000000 envoy.gpg.sign-0.1.1/envoy/gpg/sign/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-01-30 12:54:23.000000 envoy.gpg.sign-0.1.1/envoy/gpg/sign/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 12:54:23.517803 envoy.gpg.sign-0.1.1/envoy.gpg.sign.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-01-30 12:54:23.000000 envoy.gpg.sign-0.1.1/envoy.gpg.sign.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-01-30 12:54:23.000000 envoy.gpg.sign-0.1.1/envoy.gpg.sign.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 12:54:23.000000 envoy.gpg.sign-0.1.1/envoy.gpg.sign.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-30 12:54:23.000000 envoy.gpg.sign-0.1.1/envoy.gpg.sign.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 12:54:23.000000 envoy.gpg.sign-0.1.1/envoy.gpg.sign.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-30 12:54:23.000000 envoy.gpg.sign-0.1.1/envoy.gpg.sign.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-30 12:54:23.000000 envoy.gpg.sign-0.1.1/envoy.gpg.sign.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 12:54:23.517803 envoy.gpg.sign-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-01-30 12:54:23.000000 envoy.gpg.sign-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:23:05.452021 envoy.gpg.sign-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-30 18:23:05.448021 envoy.gpg.sign-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:23:05.448021 envoy.gpg.sign-0.2.0/envoy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:23:05.448021 envoy.gpg.sign-0.2.0/envoy/gpg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:23:05.448021 envoy.gpg.sign-0.2.0/envoy/gpg/sign/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/envoy/gpg/sign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/envoy/gpg/sign/bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/envoy/gpg/sign/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/envoy/gpg/sign/deb.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/envoy/gpg/sign/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/envoy/gpg/sign/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/envoy/gpg/sign/rpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/envoy/gpg/sign/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/envoy/gpg/sign/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:23:05.448021 envoy.gpg.sign-0.2.0/envoy.gpg.sign.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/envoy.gpg.sign.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/envoy.gpg.sign.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/envoy.gpg.sign.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/envoy.gpg.sign.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/envoy.gpg.sign.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/envoy.gpg.sign.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/envoy.gpg.sign.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 18:23:05.452021 envoy.gpg.sign-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-30 18:23:05.000000 envoy.gpg.sign-0.2.0/setup.py
```

### Comparing `envoy.gpg.sign-0.1.1/backend_shim.py` & `envoy.gpg.sign-0.2.0/backend_shim.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 
 # DO NOT EDIT THIS FILE -- AUTOGENERATED BY PANTS
 
+import os
 import setuptools.build_meta
 
 backend = setuptools.build_meta.__legacy__
 
 dist_dir = "dist"
 build_wheel = True
 build_sdist = True
 wheel_config_settings = {
 }
 sdist_config_settings = {
 }
 
+os.makedirs(dist_dir, exist_ok=True)
 wheel_path = backend.build_wheel(dist_dir, wheel_config_settings) if build_wheel else None
 sdist_path = backend.build_sdist(dist_dir, sdist_config_settings) if build_sdist else None
 
 if wheel_path:
     print("wheel: {wheel_path}".format(wheel_path=wheel_path))
 if sdist_path:
     print("sdist: {sdist_path}".format(sdist_path=sdist_path))
```

### Comparing `envoy.gpg.sign-0.1.1/envoy/gpg/sign/deb.py` & `envoy.gpg.sign-0.2.0/envoy/gpg/sign/deb.py`

 * *Files identical despite different names*

### Comparing `envoy.gpg.sign-0.1.1/envoy/gpg/sign/rpm.py` & `envoy.gpg.sign-0.2.0/envoy/gpg/sign/rpm.py`

 * *Files identical despite different names*

### Comparing `envoy.gpg.sign-0.1.1/envoy/gpg/sign/runner.py` & `envoy.gpg.sign-0.2.0/envoy/gpg/sign/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import argparse
 import pathlib
-import tarfile
+import re
 import tempfile
 from functools import cached_property
-from typing import Optional, Type, Union
+from typing import Optional, Type
 
 from aio.run import runner
 
 from envoy.base import utils
 from envoy.gpg import identity
 
 from .exceptions import SigningError
@@ -29,32 +29,33 @@
             cls,
             name: str,
             util: Type[DirectorySigningUtil]) -> None:
         """Register util for signing a package type."""
         cls._signing_utils = getattr(cls, "_signing_utils") + ((name, util),)
 
     @property
-    def extract(self) -> bool:
-        return self.args.extract
-
-    @property
     def gen_key(self) -> bool:
         return self.args.gen_key
 
     @property
     def gnupg_home(self) -> Optional[pathlib.Path]:
         return (
             pathlib.Path(self.gnupg_tempdir.name)
             if self.gen_key
             else None)
 
     @cached_property
     def gnupg_tempdir(self) -> tempfile.TemporaryDirectory:
         return tempfile.TemporaryDirectory()
 
+    @property
+    def infiles(self) -> str:
+        """Path to the packages directory."""
+        return self.args.infiles
+
     @cached_property
     def maintainer(self) -> identity.GPGIdentity:
         """A representation of the maintainer with GPG capabilities."""
         return self.maintainer_class(
             self.maintainer_name,
             self.maintainer_email,
             self.log,
@@ -72,50 +73,57 @@
 
     @property
     def maintainer_name(self) -> str:
         """Name of the maintainer if set."""
         return self.args.maintainer_name
 
     @property
+    def mappings(self) -> dict[str, str]:
+        return dict(
+            utils.tuple_pair(m)
+            for m
+            in (self.args.mapping or []))
+
+    @property
+    def outfile(self) -> str:
+        return self.args.out
+
+    @property
     def package_type(self) -> str:
         """Package type - eg deb/rpm"""
         return self.args.package_type
 
     @property
-    def path(self) -> pathlib.Path:
-        """Path to the packages directory."""
-        return pathlib.Path(self.args.path)
+    def repack(self):
+        return utils.repack(
+            self.outfile,
+            *self.infiles,
+            mappings=self.mappings,
+            matching=re.compile("^(?!^(dbg|utils)).*"),
+            include=re.compile(
+                f"{self.signing_key_path}"
+                f"|{'|'.join(self.signing_utils)}"))
 
     @property
     def signing_key_path(self) -> str:
         return SIGNING_KEY_PATH
 
     @cached_property
     def signing_utils(self) -> dict:
         """Configured signing utils - eg `DebSigningUtil`, `RPMSigningUtil`"""
         return dict(getattr(self, "_signing_utils"))
 
-    @property
-    def tar(self) -> str:
-        return self.args.tar
-
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         super().add_arguments(parser)
         parser.add_argument(
-            "path",
-            default="",
-            help="Path to the directory containing packages to sign")
+            "infiles",
+            nargs="+",
+            help="Paths to the tarballs containing packages to sign")
         parser.add_argument(
-            "--extract",
-            action="store_true",
-            help=(
-                "If set, treat the path as a tarball containing directories "
-                "according to package_type"))
-        parser.add_argument(
-            "--tar",
+            "--out",
             help="Path to save the signed packages as tar file")
         parser.add_argument(
             "--type",
             default="",
             choices=[c for c in self.signing_utils] + [""],
             help="Package type to sign")
         parser.add_argument(
@@ -132,59 +140,41 @@
                 "to match with"))
         parser.add_argument(
             "--gen-key",
             action="store_true",
             help=(
                 "If set, create the signing key (requires "
                 "`--maintainer-name` and `--maintainer-email`) "))
+        parser.add_argument(
+            "-m", "--mapping",
+            action="append")
 
-    def add_key(self, path: Union[pathlib.Path, str]) -> None:
-        # todo(phlax): always return pathlib.Path from untar and avoid
-        #    the `utils.typed`
-        utils.typed(pathlib.Path, path).joinpath(
+    def add_key(self, path: pathlib.Path) -> None:
+        path.joinpath(
             self.signing_key_path).write_text(self.maintainer.export_key())
 
-    def archive(self, path: Union[pathlib.Path, str]) -> None:
-        with tarfile.open(self.tar, utils.tar_mode(self.tar, mode="w")) as tar:
-            tar.add(path, arcname=".")
-
     async def cleanup(self):
         if "gnupg_tempdir" in self.__dict__:
             self.gnupg_tempdir.cleanup()
             del self.__dict__["gnupg_tempdir"]
 
     def get_signing_util(self, path: pathlib.Path) -> DirectorySigningUtil:
         return self.signing_utils[path.name](path, self.maintainer, self.log)
 
     @runner.catches((identity.GPGError, SigningError))
     @runner.cleansup
     async def run(self) -> None:
-        if self.extract:
-            self.sign_tarball()
-        else:
-            self.sign_directory()
-        self.log.success("Successfully signed packages")
+        with self.repack as tmpdir:
+            self.sign_all(tmpdir)
+            self.add_key(tmpdir)
+        self.log.success(f"Successfully signed packages: {self.outfile}")
 
     def sign(self, path: pathlib.Path) -> None:
         self.log.notice(
             f"Signing {path.name}s ({self.maintainer}) {str(path)}")
-        self.get_signing_util(path).sign()
+        util = self.get_signing_util(path)
+        util.sign()
 
     def sign_all(self, path: pathlib.Path) -> None:
         for directory in path.glob("*"):
             if directory.name in self.signing_utils:
                 self.sign(directory)
-
-    def sign_directory(self) -> None:
-        self.sign(self.path)
-        if self.tar:
-            self.archive(self.path)
-
-    def sign_tarball(self) -> None:
-        if not self.tar:
-            raise SigningError(
-                "You must set a `--tar` file to save to "
-                "when `--extract` is set")
-        with utils.untar(self.path) as tardir:
-            self.sign_all(tardir)
-            self.add_key(tardir)
-            self.archive(tardir)
```

### Comparing `envoy.gpg.sign-0.1.1/envoy/gpg/sign/util.py` & `envoy.gpg.sign-0.2.0/envoy/gpg/sign/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import pathlib
 import shutil
 import subprocess
 from functools import cached_property
-from typing import Optional, Tuple, Union
+from typing import Iterable, Optional
 
 import verboselogs  # type:ignore
 
 from envoy.gpg import identity
 
 from .exceptions import SigningError
 
@@ -17,15 +17,15 @@
 
     command_name = ""
     _package_type = ""
     ext = ""
 
     def __init__(
             self,
-            path: Union[pathlib.Path, str],
+            path: pathlib.Path | str,
             maintainer: identity.GPGIdentity,
             log: verboselogs.VerboseLogger,
             command: Optional[str] = ""):
         self._path = path
         self.maintainer = maintainer
         self.log = log
         self._command = command
@@ -49,15 +49,15 @@
         return self._package_type or self.ext
 
     @property
     def path(self) -> pathlib.Path:
         return pathlib.Path(self._path)
 
     @property
-    def pkg_files(self) -> Tuple[pathlib.Path, ...]:
+    def pkg_files(self) -> Iterable[pathlib.Path]:
         """Tuple of paths to package files to sign."""
         # TODO?(phlax): check maintainer/packager field matches key id
         return tuple(
             pkg_file
             for pkg_file
             in self.path.glob("*")
             if pkg_file.name.endswith(f".{self.ext}"))
```

### Comparing `envoy.gpg.sign-0.1.1/setup.py` & `envoy.gpg.sign-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,16 @@
     'entry_points': {
         'console_scripts': [
             'envoy.gpg.sign=envoy.gpg.sign:cmd',
         ],
     },
     'install_requires': (
         'aio.run.runner>=0.3.3',
-        'envoy.base.utils>=0.3.9',
-        'envoy.gpg.identity>=0.1.0',
-        'verboselogs',
+        'envoy.base.utils>=0.4.7',
+        'envoy.gpg.identity>=0.1.1',
     ),
     'license': 'Apache Software License 2.0',
     'long_description': """
 envoy.gpg.sign
 ==============
 
 GPG signing util used in Envoy proxy's CI
@@ -35,10 +34,11 @@
         'envoy.gpg.sign': (
             'py.typed',
         ),
     },
     'packages': (
         'envoy.gpg.sign',
     ),
+    'python_requires': '>=3.10.0',
     'url': 'https://github.com/envoyproxy/pytooling/tree/main/envoy.gpg.sign',
-    'version': '0.1.1',
+    'version': '0.2.0',
 })
```

