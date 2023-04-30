# Comparing `tmp/wtt01-0.3.2.tar.gz` & `tmp/wtt01-0.3.3.tar.gz`

## Comparing `wtt01-0.3.2.tar` & `wtt01-0.3.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 wtt01-0.3.2/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtt01-0.3.2/tests/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 wtt01-0.3.2/tests/test_load.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 wtt01-0.3.2/wtt01/__about__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wtt01-0.3.2/wtt01/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 wtt01-0.3.2/wtt01/_env.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wtt01-0.3.2/wtt01/cli.py
--rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 wtt01-0.3.2/wtt01/main.py
--rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 wtt01-0.3.2/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 wtt01-0.3.2/LICENSE.txt
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wtt01-0.3.2/README.md
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 wtt01-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 wtt01-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 wtt01-0.3.3/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtt01-0.3.3/tests/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 wtt01-0.3.3/tests/test_load.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 wtt01-0.3.3/wtt01/__about__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wtt01-0.3.3/wtt01/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 wtt01-0.3.3/wtt01/_env.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wtt01-0.3.3/wtt01/cli.py
+-rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 wtt01-0.3.3/wtt01/main.py
+-rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 wtt01-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 wtt01-0.3.3/LICENSE.txt
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wtt01-0.3.3/README.md
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 wtt01-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 wtt01-0.3.3/PKG-INFO
```

### Comparing `wtt01-0.3.2/tests/test_load.py` & `wtt01-0.3.3/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `wtt01-0.3.2/wtt01/cli.py` & `wtt01-0.3.3/wtt01/cli.py`

 * *Files identical despite different names*

### Comparing `wtt01-0.3.2/wtt01/main.py` & `wtt01-0.3.3/wtt01/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Package for wtt01."""
 
 from pathlib import Path
 from typing import Optional, Union
 import os
 from string import Template
+import shutil
+import gzip
 
 import platform
-import zipfile
 import tempfile
 
 import urllib.request
 
 import duckdb
 
 from wtt01.__about__ import __version__, EXTENSION_NAME
@@ -55,15 +56,14 @@
         return con.execute(file_path.read_text(encoding="utf-8"))
 
 
 def get_connection(
     database: str = ":memory:",
     read_only: bool = False,
     config: Optional[dict] = None,
-    s3_uri: Optional[str] = None,
     file_path: Optional[Path] = None,
 ) -> duckdb.DuckDBPyConnection:
     """Return a connection with wtt01 loaded."""
 
     if "WTT_01_LICENSE" not in os.environ:
         raise WTT01ConfigurationException(
             "WTT_01_LICENSE environment variable not set. "
@@ -88,53 +88,57 @@
             con.install_extension(str(extension_path), force_install=True)
             con.load_extension(EXTENSION_NAME)
 
         elif file_path is not None and file_path.exists():
             con.install_extension(str(file_path.absolute()), force_install=True)
             con.load_extension(EXTENSION_NAME)
 
-        elif s3_uri is not None:
-            # download
-            pass
         else:
+            version = __version__
+            name = "wtt01"
+
             platform_uname = platform.uname()
             operating_system = platform_uname.system
             architecture = platform_uname.machine
-            version = __version__
 
-            from wtt01._env import ENVIRONMENT
+            if operating_system.lower() == "windows":
+                duckdb_arch = "windows_amd64"
+            elif operating_system.lower() == "darwin" and architecture.lower() == "x86_64":
+                duckdb_arch = "osx_amd64"
+            elif operating_system.lower() == "darwin" and architecture.lower() == "arm64":
+                duckdb_arch = "osx_arm64"
+            elif operating_system.lower() == "linux" and architecture.lower() == "x86_64":
+                duckdb_arch = "linux_amd64_gcc4"
+            else:
+                raise WTTException(
+                    f"Unable to find extension for {operating_system} {architecture}"
+                )
 
-            env = os.getenv("WTT01_ENVIRONMENT", ENVIRONMENT)
-
-            name = "wtt01"
-            bucket = f"wtt-01-dist-{env}"
-            filename = f"{name}-{version}-{operating_system}-{architecture}.zip"
-
-            full_s3_path = (
-                f"http://{bucket}.s3.amazonaws.com/extension/{name}/{filename}"
-            )
+            filename = f"{name}.duckdb_extension.gz"
+            url = f"https://dbe.wheretrue.com/{name}/{version}/v0.7.1/{duckdb_arch}/{filename}"
 
             with tempfile.TemporaryDirectory() as temp_dir:
                 temp_dir_path = Path(temp_dir)
                 temp_file_name = temp_dir_path / filename
 
                 try:
-                    urllib.request.urlretrieve(full_s3_path, temp_file_name)
+                    urllib.request.urlretrieve(url, temp_file_name)
                 except Exception as retrieve_exp:
                     raise WTTException(
                         f"Unable to download extension from {full_s3_path}"
                     ) from retrieve_exp
 
-                with zipfile.ZipFile(temp_file_name, "r") as zip_ref:
-                    zip_ref.extract(f"{name}.duckdb_extension", temp_dir)
+                # ungzip the file
+                with gzip.open(temp_file_name, "rb") as f_in:
+                    with open(temp_file_name, "wb") as f_out:
+                        shutil.copyfileobj(f_in, f_out)
 
                 output_file = temp_dir_path / f"{name}.duckdb_extension"
                 if not output_file.exists():
                     raise WTTException(
                         f"Unable to find extension file at {output_file}"
                     ) from exp
 
                 con.install_extension(output_file.as_posix(), force_install=True)
-
                 con.load_extension(EXTENSION_NAME)
 
     return con
```

### Comparing `wtt01-0.3.2/.gitignore` & `wtt01-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `wtt01-0.3.2/LICENSE.txt` & `wtt01-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wtt01-0.3.2/pyproject.toml` & `wtt01-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wtt01-0.3.2/PKG-INFO` & `wtt01-0.3.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtt01
-Version: 0.3.2
+Version: 0.3.3
 Author-email: Trent Hauck <thauck@wheretrue.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

