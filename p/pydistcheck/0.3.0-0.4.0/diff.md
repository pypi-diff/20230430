# Comparing `tmp/pydistcheck-0.3.0.tar.gz` & `tmp/pydistcheck-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydistcheck-0.3.0.tar", last modified: Thu Feb 16 04:43:18 2023, max compression
+gzip compressed data, was "pydistcheck-0.4.0.tar", last modified: Sun Apr 30 02:48:36 2023, max compression
```

## Comparing `pydistcheck-0.3.0.tar` & `pydistcheck-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 04:43:18.105512 pydistcheck-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-02-16 04:43:18.105512 pydistcheck-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-02-16 04:43:18.105512 pydistcheck-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 04:43:18.101512 pydistcheck-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 04:43:18.101512 pydistcheck-0.3.0/src/pydistcheck/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/src/pydistcheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/src/pydistcheck/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/src/pydistcheck/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/src/pydistcheck/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/src/pydistcheck/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/src/pydistcheck/distribution_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/src/pydistcheck/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/src/pydistcheck/shared_lib_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/src/pydistcheck/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 04:43:18.101512 pydistcheck-0.3.0/src/pydistcheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-02-16 04:43:18.000000 pydistcheck-0.3.0/src/pydistcheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-02-16 04:43:18.000000 pydistcheck-0.3.0/src/pydistcheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 04:43:18.000000 pydistcheck-0.3.0/src/pydistcheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-16 04:43:18.000000 pydistcheck-0.3.0/src/pydistcheck.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-16 04:43:18.000000 pydistcheck-0.3.0/src/pydistcheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-16 04:43:18.000000 pydistcheck-0.3.0/src/pydistcheck.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 04:43:18.105512 pydistcheck-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17873 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/tests/test_distribution_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-02-16 04:43:08.000000 pydistcheck-0.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:48:36.468651 pydistcheck-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:48:36.464651 pydistcheck-0.4.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/LICENSES/DELOCATE_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-30 02:48:36.468651 pydistcheck-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-30 02:48:36.468651 pydistcheck-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:48:36.464651 pydistcheck-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:48:36.464651 pydistcheck-0.4.0/src/pydistcheck/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/src/pydistcheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/src/pydistcheck/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/src/pydistcheck/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/src/pydistcheck/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/src/pydistcheck/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/src/pydistcheck/distribution_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/src/pydistcheck/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/src/pydistcheck/shared_lib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/src/pydistcheck/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:48:36.464651 pydistcheck-0.4.0/src/pydistcheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-30 02:48:36.000000 pydistcheck-0.4.0/src/pydistcheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-30 02:48:36.000000 pydistcheck-0.4.0/src/pydistcheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 02:48:36.000000 pydistcheck-0.4.0/src/pydistcheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-30 02:48:36.000000 pydistcheck-0.4.0/src/pydistcheck.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-30 02:48:36.000000 pydistcheck-0.4.0/src/pydistcheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-30 02:48:36.000000 pydistcheck-0.4.0/src/pydistcheck.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:48:36.468651 pydistcheck-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18439 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/tests/test_distribution_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/tests/test_utils.py
```

### Comparing `pydistcheck-0.3.0/LICENSE` & `pydistcheck-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.3.0/PKG-INFO` & `pydistcheck-0.4.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: pydistcheck
-Version: 0.3.0
-Summary: Inspect Python package distributions and raise warnings on common problems.
-Home-page: https://github.com/jameslamb/pydistcheck
-Download-URL: https://github.com/jameslamb/pydistcheck
-Author: James Lamb
-Author-email: jaylamb20@gmail.com
-Maintainer: James Lamb
-Maintainer-email: jaylamb20@gmail.com
-License: BSD-3-Clause
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-License-File: LICENSE
-
 # pydistcheck
 
 [![conda-forge version](https://img.shields.io/conda/vn/conda-forge/pydistcheck.svg)](https://anaconda.org/conda-forge/pydistcheck)
 [![conda-forge downloads](https://img.shields.io/conda/dn/conda-forge/pydistcheck.svg)](https://anaconda.org/conda-forge/pydistcheck)
 [![PyPI Version](https://img.shields.io/pypi/v/pydistcheck.svg?logo=pypi&logoColor=white)](https://pypi.org/project/pydistcheck)
 [![PyPI downloads](https://static.pepy.tech/badge/pydistcheck)](https://pypi.org/project/pydistcheck)
 [![Documentation Status](https://readthedocs.org/projects/pydistcheck/badge/?version=latest)](https://pydistcheck.readthedocs.io/)
@@ -55,35 +25,57 @@
 
 ```shell
 pipx install pydistcheck
 ```
 
 ## Quickstart
 
-Try it out on the test data in this project!
+Try it out on the test data in this project ...
 
 ```shell
 pydistcheck tests/data/problematic-package-*
 ```
 
-Yields something like the following.
+... to see the types of issues it checks for.
+
+```text
+------------ check results -----------
+1. [files-only-differ-by-case] Found files which differ only by case. Files: problematic-package-0.1.0/problematic_package/Question.py,problematic-package-0.1.0/problematic_package/question.PY,problematic-package-0.1.0/problematic_package/question.py
+2. [mixed-file-extensions] Found a mix of file extensions for the same file type: .NDJSON (1), .jsonl (1), .ndjson (1)
+3. [mixed-file-extensions] Found a mix of file extensions for the same file type: .yaml (2), .yml (1)
+4. [path-contains-non-ascii-characters] Found file path containing non-ASCII characters: 'problematic-package-0.1.0/problematic_package/?veryone-loves-python.py'
+5. [path-contains-spaces] Found path with spaces: 'problematic-package-0.1.0/beep boop.ini'
+6. [path-contains-spaces] Found path with spaces: 'problematic-package-0.1.0/problematic_package/bad code/'
+7. [path-contains-spaces] Found path with spaces: 'problematic-package-0.1.0/problematic_package/bad code/__init__.py'
+8. [path-contains-spaces] Found path with spaces: 'problematic-package-0.1.0/problematic_package/bad code/ship-it.py'
+9. [unexpected-files] Found unexpected directory 'problematic-package-0.1.0/.git/'.
+10. [unexpected-files] Found unexpected file 'problematic-package-0.1.0/.gitignore'.
+11. [unexpected-files] Found unexpected file 'problematic-package-0.1.0/.hadolint.yaml'.
+12. [unexpected-files] Found unexpected file 'problematic-package-0.1.0/problematic_package/.gitignore'.
+errors found while checking: 12
+```
+
+And on a built distribution containing compiled objects ...
+
+```shell
+pydistcheck tests/data/debug-baseballmmetrics*.whl
+```
+
+... `pydistcheck` can detect the inclusion of debug symbols (which increase distribution size).
 
 ```text
+checking 'tests/data/debug-baseballmetrics-0.1.0-py3-none-macosx_10_15_x86_64.macosx_11_6_x86_64.macosx_12_5_x86_64.whl'
+------------ check results -----------
+1. [compiled-objects-have-debug-symbols] Found compiled object containing debug symbols. For details, extract the distribution contents and run 'dsymutil -s "lib/lib_baseballmetrics.dylib"'.
+errors found while checking: 1
+
+checking 'tests/data/debug-baseballmetrics-py3-none-manylinux_2_28_x86_64.manylinux_2_5_x86_64.manylinux1_x86_64.whl'
 ------------ check results -----------
-1. [files-only-differ-by-case] Found files which differ only by case. Such files are not portable, since some filesystems are case-insensitive. Files: problematic-package-0.1.0/problematic_package/Question.py,problematic-package-0.1.0/problematic_package/question.PY,problematic-package-0.1.0/problematic_package/question.py
-2. [path-contains-spaces] File paths with spaces are not portable. Found path with spaces: 'problematic-package-0.1.0/beep boop.ini'
-3. [path-contains-spaces] File paths with spaces are not portable. Found path with spaces: 'problematic-package-0.1.0/problematic_package/bad code'
-4. [path-contains-spaces] File paths with spaces are not portable. Found path with spaces: 'problematic-package-0.1.0/problematic_package/bad code/__init__.py'
-5. [path-contains-spaces] File paths with spaces are not portable. Found path with spaces: 'problematic-package-0.1.0/problematic_package/bad code/ship-it.py'
-6. [path-contains-non-ascii-characters] Found file path containing non-ASCII characters: 'problematic-package-0.1.0/problematic_package/?veryone-loves-python.py'
-7. [unexpected-files] Found unexpected directory 'problematic-package-0.1.0/.git/'.
-8. [unexpected-files] Found unexpected file 'problematic-package-0.1.0/.gitignore'.
-9. [unexpected-files] Found unexpected file 'problematic-package-0.1.0/.hadolint.yaml'.
-10. [unexpected-files] Found unexpected file 'problematic-package-0.1.0/problematic_package/.gitignore'.
-errors found while checking: 10
+1. [compiled-objects-have-debug-symbols] Found compiled object containing debug symbols. For details, extract the distribution contents and run 'objdump --all-headers "lib/lib_baseballmetrics.so"'.
+errors found while checking: 1
 ```
 
 See https://pydistcheck.readthedocs.io/en/latest/ to learn more.
 
 ## Related Projects
 
 * https://pypi.org/project/inspect4py/
```

### Comparing `pydistcheck-0.3.0/src/pydistcheck/checks.py` & `pydistcheck-0.4.0/src/pydistcheck/checks.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # relies on unit tests to ensure that it's updated as the list of checks changes.
 ALL_CHECKS = {
     "compiled-objects-have-debug-symbols",
     "distro-too-large-compressed",
     "distro-too-large-uncompressed",
     "too-many-files",
     "files-only-differ-by-case",
+    "mixed-file-extensions",
     "path-contains-non-ascii-characters",
     "path-contains-spaces",
     "unexpected-files",
 }
 
 
 class _CheckProtocol(Protocol):
@@ -122,15 +123,14 @@
             if len(filepaths) > 1:
                 duplicates_list += filepaths
 
         if duplicates_list:
             duplicates_str = ",".join(sorted(duplicates_list))
             msg = (
                 f"[{self.check_name}] Found files which differ only by case. "
-                "Such files are not portable, since some filesystems are case-insensitive. "
                 f"Files: {duplicates_str}"
             )
             out.append(msg)
         return out
 
 
 class _NonAsciiCharacterCheck(_CheckProtocol):
@@ -145,25 +145,52 @@
                     f"[{self.check_name}] Found file path containing non-ASCII characters: "
                     f"'{ascii_converted_str}'"
                 )
                 out.append(msg)
         return out
 
 
+class _MixedFileExtensionCheck(_CheckProtocol):
+    check_name = "mixed-file-extensions"
+
+    file_ext_groups = [
+        {".cc", ".CC", ".cpp", ".CPP"},
+        {".htm", ".HTM", ".html", ".HTML"},
+        {".jpg", ".JPG", ".jpeg", ".JPEG"},
+        {".jsonl", ".JSONL", ".ndjson", ".NDJSON"},
+        {".txt", ".TXT", ".text", ".TEXT"},
+        {".yaml", ".YAML", ".yml", ".YML"},
+    ]
+
+    def __call__(self, distro_summary: _DistributionSummary) -> List[str]:
+        out: List[str] = []
+        file_extensions_in_distro = set(distro_summary.files_by_extension.keys())
+        for file_ext_group in self.file_ext_groups:
+            extensions_found = file_ext_group.intersection(file_extensions_in_distro)
+            if len(extensions_found) >= 2:
+                count_str = ", ".join(
+                    f"{ext} ({distro_summary.count_by_file_extension[ext]})"
+                    for ext in sorted(extensions_found)
+                )
+                msg = (
+                    f"[{self.check_name}] Found a mix of file extensions for "
+                    f"the same file type: {count_str}"
+                )
+                out.append(msg)
+        return out
+
+
 class _SpacesInPathCheck(_CheckProtocol):
     check_name = "path-contains-spaces"
 
     def __call__(self, distro_summary: _DistributionSummary) -> List[str]:
         out: List[str] = []
         for file_path in distro_summary.all_paths:
             if file_path != file_path.replace(" ", ""):
-                msg = (
-                    f"[{self.check_name}] File paths with spaces are not portable. "
-                    f"Found path with spaces: '{file_path}'"
-                )
+                msg = f"[{self.check_name}] Found path with spaces: '{file_path}'"
                 out.append(msg)
         return out
 
 
 class _UnexpectedFilesCheck(_CheckProtocol):
     check_name = "unexpected-files"
```

### Comparing `pydistcheck-0.3.0/src/pydistcheck/cli.py` & `pydistcheck-0.4.0/src/pydistcheck/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from pydistcheck.checks import (
     ALL_CHECKS,
     _CompiledObjectsDebugSymbolCheck,
     _DistroTooLargeCompressedCheck,
     _DistroTooLargeUnCompressedCheck,
     _FileCountCheck,
     _FilesOnlyDifferByCaseCheck,
+    _MixedFileExtensionCheck,
     _NonAsciiCharacterCheck,
     _SpacesInPathCheck,
     _UnexpectedFilesCheck,
 )
 from pydistcheck.config import _Config
 from pydistcheck.distribution_summary import _DistributionSummary
 from pydistcheck.inspect import inspect_distribution
@@ -155,14 +156,15 @@
         _DistroTooLargeUnCompressedCheck(
             max_allowed_size_bytes=_FileSize.from_string(
                 size_str=config.max_allowed_size_uncompressed
             ).total_size_bytes
         ),
         _FileCountCheck(max_allowed_files=config.max_allowed_files),
         _FilesOnlyDifferByCaseCheck(),
+        _MixedFileExtensionCheck(),
         _SpacesInPathCheck(),
         _UnexpectedFilesCheck(
             unexpected_directory_patterns=unexpected_directory_patterns.split(","),
             unexpected_file_patterns=unexpected_file_patterns.split(","),
         ),
         _NonAsciiCharacterCheck(),
     ]
```

### Comparing `pydistcheck-0.3.0/src/pydistcheck/config.py` & `pydistcheck-0.4.0/src/pydistcheck/config.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.3.0/src/pydistcheck/distribution_summary.py` & `pydistcheck-0.4.0/src/pydistcheck/distribution_summary.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 import os
 import pathlib
 import tarfile
 import zipfile
 from collections import OrderedDict, defaultdict
 from dataclasses import dataclass
-from typing import List, Tuple, Union
+from functools import cached_property
+from typing import Dict, List, Tuple, Union
 
 
 @dataclass
 class _DirectoryInfo:
     name: str
 
 
@@ -169,18 +170,32 @@
     def all_paths(self) -> List[str]:
         return self.file_paths + self.directory_paths
 
     @property
     def compiled_objects(self) -> List[_FileInfo]:
         return [f for f in self.files if f.is_compiled is True]
 
+    @cached_property
+    def count_by_file_extension(self) -> Dict[str, int]:
+        return {
+            file_extension: len(file_list)
+            for file_extension, file_list in self.files_by_extension.items()
+        }
+
     @property
     def directory_paths(self) -> List[str]:
         return [d.name for d in self.directories]
 
+    @cached_property
+    def files_by_extension(self) -> Dict[str, List[_FileInfo]]:
+        out: Dict[str, List[_FileInfo]] = defaultdict(list)
+        for f in self.files:
+            out[f.file_extension].append(f)
+        return out
+
     @property
     def file_paths(self) -> List[str]:
         return [f.name for f in self.files]
 
     @property
     def num_directories(self) -> int:
         return len(self.directories)
@@ -198,16 +213,17 @@
         """
         Aggregate file sizes in a distribution by extension.
 
         :return: An OrderedDict where keys are file extensions and values are the total size in
                  bytes occupied by such files in the distribution. Sorted in descending
                  order by size.
         """
-        summary_dict: defaultdict = defaultdict(int)
-        for f in self.files:
-            summary_dict[f.file_extension] += f.uncompressed_size_bytes
+        summary_dict = {
+            file_extension: sum(f.uncompressed_size_bytes for f in files)
+            for file_extension, files in self.files_by_extension.items()
+        }
         sorted_sizes = list(summary_dict.items())
         sorted_sizes.sort(key=lambda x: x[1], reverse=True)
         out = OrderedDict()
         for file_extension, size_in_bytes in sorted_sizes:
             out[file_extension] = size_in_bytes
         return out
```

### Comparing `pydistcheck-0.3.0/src/pydistcheck/inspect.py` & `pydistcheck-0.4.0/src/pydistcheck/inspect.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.3.0/src/pydistcheck/shared_lib_utils.py` & `pydistcheck-0.4.0/src/pydistcheck/shared_lib_utils.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.3.0/src/pydistcheck/utils.py` & `pydistcheck-0.4.0/src/pydistcheck/utils.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.3.0/tests/test_checks.py` & `pydistcheck-0.4.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.3.0/tests/test_cli.py` & `pydistcheck-0.4.0/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -326,112 +326,124 @@
             r"larger than the allowed size \(0\.1K\)\.$"
         ),
     )
     _assert_log_matches_pattern(result, "errors found while checking\\: 1")
 
 
 @pytest.mark.parametrize("distro_file", PROBLEMATIC_PACKAGES)
-def test_cli_raises_exactly_the_expected_number_of_errors_for_the_problematic_package(distro_file):
-    runner = CliRunner()
-    result = runner.invoke(
-        check,
-        [os.path.join(TEST_DATA_DIR, distro_file)],
-    )
-    assert result.exit_code == 1
-    _assert_log_matches_pattern(result=result, pattern=r"errors found while checking\: 10$")
-
-
-@pytest.mark.parametrize("distro_file", PROBLEMATIC_PACKAGES)
 def test_files_only_differ_by_case_works(distro_file):
     runner = CliRunner()
     result = runner.invoke(
         check,
         [os.path.join(TEST_DATA_DIR, distro_file)],
     )
     assert result.exit_code == 1
 
     _assert_log_matches_pattern(
         result=result,
         pattern=(
             r"^1\. \[files\-only\-differ\-by\-case\] Found files which differ only by case\. "
-            r"Such files are not portable, since some filesystems are case-insensitive\. "
             r"Files\: problematic\-package\-0\.1\.0/problematic_package/Question\.py"
             r",problematic\-package\-0\.1\.0/problematic_package/question\.PY"
             r",problematic\-package\-0\.1\.0/problematic_package/question\.py"
         ),
     )
     _assert_log_matches_pattern(result=result, pattern=r"errors found while checking\: [0-9]{1}")
 
 
 @pytest.mark.parametrize("distro_file", PROBLEMATIC_PACKAGES)
-def test_path_contains_spaces_works(distro_file):
+def test_mixed_file_extension_use_works(distro_file):
     runner = CliRunner()
     result = runner.invoke(
         check,
         [os.path.join(TEST_DATA_DIR, distro_file)],
     )
     assert result.exit_code == 1
 
-    # should report a file with spaces in a directory without spaces
     _assert_log_matches_pattern(
         result=result,
         pattern=(
-            r"^3\. \[path\-contains\-spaces\] File paths with spaces are not portable\. "
-            r"Found path with spaces\: 'problematic\-package\-0\.1\.0/beep boop\.ini"
+            r"^2\. \[mixed\-file\-extensions\] Found a mix of file extensions for the "
+            r"same file type\: \.NDJSON \(1\), \.jsonl \(1\), \.ndjson \(1\)"
         ),
     )
-
-    # should report a directory with spaces
     _assert_log_matches_pattern(
         result=result,
         pattern=(
-            r"^4\. \[path\-contains\-spaces\] File paths with spaces are not portable\. "
-            r"Found path with spaces\: "
-            r"'problematic\-package\-0\.1\.0/problematic_package/bad code[/]*"
+            r"^3\. \[mixed\-file\-extensions\] Found a mix of file extensions for the "
+            r"same file type\: \.yaml \(2\), \.yml \(1\)"
         ),
     )
 
-    # should report a file without spaces inside a directory with spaces
-    _assert_log_matches_pattern(
-        result=result,
-        pattern=(
-            r"^5\. \[path\-contains\-spaces\] File paths with spaces are not portable\. "
-            r"Found path with spaces\: "
-            r"'problematic\-package\-0\.1\.0/problematic_package/bad code/__init__\.py"
-        ),
+    _assert_log_matches_pattern(result=result, pattern=r"errors found while checking\: [0-9]{1}")
+
+
+@pytest.mark.parametrize("distro_file", PROBLEMATIC_PACKAGES)
+def test_path_contains_non_ascii_characters_works(distro_file):
+    runner = CliRunner()
+    result = runner.invoke(
+        check,
+        [os.path.join(TEST_DATA_DIR, distro_file)],
     )
+    assert result.exit_code == 1
+
+    # NOTE: matching a variable number of '?' because zip and tar (and even different
+    #       implementations of those) encode non-ASCII characters in paths differently
     _assert_log_matches_pattern(
         result=result,
         pattern=(
-            r"^6\. \[path\-contains\-spaces\] File paths with spaces are not portable\. "
-            r"Found path with spaces\: "
-            r"'problematic\-package\-0\.1\.0/problematic_package/bad code/ship\-it\.py"
+            r"^4\. \[path\-contains\-non\-ascii\-characters\] Found file path containing non-ASCII "
+            r"characters\: "
+            r"'problematic\-package\-0\.1\.0/problematic_package/\?+veryone-loves-python\.py'"
         ),
     )
 
     _assert_log_matches_pattern(result=result, pattern=r"errors found while checking\: [0-9]{1}")
 
 
 @pytest.mark.parametrize("distro_file", PROBLEMATIC_PACKAGES)
-def test_path_contains_non_ascii_characters_works(distro_file):
+def test_path_contains_spaces_works(distro_file):
     runner = CliRunner()
     result = runner.invoke(
         check,
         [os.path.join(TEST_DATA_DIR, distro_file)],
     )
     assert result.exit_code == 1
 
-    # NOTE: matching a variable number of '?' because zip and tar (and even different
-    #       implementations of those) encode non-ASCII characters in paths differently
+    # should report a file with spaces in a directory without spaces
     _assert_log_matches_pattern(
         result=result,
         pattern=(
-            r"^2\. \[path\-contains\-non\-ascii\-characters\] Found file path containing non-ASCII "
-            r"characters\: "
-            r"'problematic\-package\-0\.1\.0/problematic_package/\?+veryone-loves-python\.py'"
+            r"^5\. \[path\-contains\-spaces\] "
+            r"Found path with spaces\: 'problematic\-package\-0\.1\.0/beep boop\.ini"
+        ),
+    )
+
+    # should report a directory with spaces
+    _assert_log_matches_pattern(
+        result=result,
+        pattern=(
+            r"^6\. \[path\-contains\-spaces\] Found path with spaces\: "
+            r"'problematic\-package\-0\.1\.0/problematic_package/bad code[/]*"
+        ),
+    )
+
+    # should report a file without spaces inside a directory with spaces
+    _assert_log_matches_pattern(
+        result=result,
+        pattern=(
+            r"^7\. \[path\-contains\-spaces\] Found path with spaces\: "
+            r"'problematic\-package\-0\.1\.0/problematic_package/bad code/__init__\.py"
+        ),
+    )
+    _assert_log_matches_pattern(
+        result=result,
+        pattern=(
+            r"^8\. \[path\-contains\-spaces\] Found path with spaces\: "
+            r"'problematic\-package\-0\.1\.0/problematic_package/bad code/ship\-it\.py"
         ),
     )
 
     _assert_log_matches_pattern(result=result, pattern=r"errors found while checking\: [0-9]{1}")
 
 
 @pytest.mark.parametrize("distro_file", PROBLEMATIC_PACKAGES)
@@ -443,47 +455,58 @@
     )
     assert result.exit_code == 1
 
     # directory
     _assert_log_matches_pattern(
         result=result,
         pattern=(
-            r"^7\. \[unexpected\-files\] Found unexpected directory "
+            r"^9\. \[unexpected\-files\] Found unexpected directory "
             r"'problematic\-package\-0\.1\.0/\.git[/]{0,1}'\."
         ),
     )
 
     # root-level files
     _assert_log_matches_pattern(
         result=result,
         pattern=(
-            r"^8\. \[unexpected\-files\] Found unexpected file "
+            r"^10\. \[unexpected\-files\] Found unexpected file "
             r"'problematic\-package\-0\.1\.0/\.gitignore'\."
         ),
     )
     _assert_log_matches_pattern(
         result=result,
         pattern=(
-            r"^9\. \[unexpected\-files\] Found unexpected file "
+            r"^11\. \[unexpected\-files\] Found unexpected file "
             r"'problematic\-package\-0\.1\.0/\.hadolint\.yaml'\."
         ),
     )
 
     # nested files
     _assert_log_matches_pattern(
         result=result,
         pattern=(
-            r"^10\. \[unexpected\-files\] Found unexpected file "
+            r"^12\. \[unexpected\-files\] Found unexpected file "
             r"'problematic\-package\-0\.1\.0/problematic_package/\.gitignore'\."
         ),
     )
 
     _assert_log_matches_pattern(result=result, pattern=r"errors found while checking\: [0-9]{1}")
 
 
+@pytest.mark.parametrize("distro_file", PROBLEMATIC_PACKAGES)
+def test_cli_raises_exactly_the_expected_number_of_errors_for_the_problematic_package(distro_file):
+    runner = CliRunner()
+    result = runner.invoke(
+        check,
+        [os.path.join(TEST_DATA_DIR, distro_file)],
+    )
+    assert result.exit_code == 1
+    _assert_log_matches_pattern(result=result, pattern=r"errors found while checking\: 12$")
+
+
 @pytest.mark.parametrize("distro_file", WHEELS_WITH_DEBUG_SYMBOLS)
 def test_debug_symbols_check_works(distro_file):
     runner = CliRunner()
     result = runner.invoke(
         check,
         [os.path.join(TEST_DATA_DIR, distro_file)],
     )
```

### Comparing `pydistcheck-0.3.0/tests/test_config.py` & `pydistcheck-0.4.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.3.0/tests/test_distribution_summary.py` & `pydistcheck-0.4.0/tests/test_distribution_summary.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,14 +73,18 @@
         ".cfg": 258,
         ".md": 15,
         "no-extension": 382,
         ".py": 70,
         ".txt": 11603,
     }
 
+    # files_by_extension makes sense
+    assert ds.files_by_extension.keys() == ds.size_by_file_extension.keys()
+    assert sum(len(file_list) for file_list in ds.files_by_extension.values()) == ds.num_files
+
     # size_by_file_extension should return results sorted from largest to smallest by file size
     last_size_seen = float("inf")
     for _, size_in_bytes in ds.size_by_file_extension.items():
         assert size_in_bytes < last_size_seen
         last_size_seen = size_in_bytes
 
 
@@ -142,23 +146,27 @@
     assert lib_file_info.is_compiled is True
 
     assert sorted(ds.directory_paths) == sorted(expected_dir_paths)
     assert sorted(ds.file_paths) == sorted(expected_file_paths)
 
     # total archive sizes should make sense
     assert ds.compressed_size_bytes > 0
-    assert ds.compressed_size_bytes < 6e3
     assert ds.uncompressed_size_bytes > 0
-    assert ds.uncompressed_size_bytes > ds.compressed_size_bytes
+    if "macosx" in distro_file:
+        assert ds.compressed_size_bytes < 25e3
+        assert ds.uncompressed_size_bytes != ds.compressed_size_bytes
+    else:
+        assert ds.compressed_size_bytes < 6e3
+        assert ds.uncompressed_size_bytes > ds.compressed_size_bytes
 
     # size_by_file_extension should work as expected
     if "macosx" in distro_file:
         assert ds.size_by_file_extension == {
             ".dylib": 16504,
-            "no-extension": 824,
+            "no-extension": 837,
             ".py": 536,
             ".txt": 0,
         }
     else:
         assert ds.size_by_file_extension == {
             ".so": 15616,
             "no-extension": 902,
```

### Comparing `pydistcheck-0.3.0/tests/test_docs.py` & `pydistcheck-0.4.0/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.3.0/tests/test_utils.py` & `pydistcheck-0.4.0/tests/test_utils.py`

 * *Files identical despite different names*

