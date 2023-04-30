# Comparing `tmp/xpypact-0.3.0.tar.gz` & `tmp/xpypact-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpypact-0.3.0.tar", max compression
+gzip compressed data, was "xpypact-0.4.0.tar", max compression
```

## Comparing `xpypact-0.3.0.tar` & `xpypact-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1063 2023-04-11 10:08:01.831799 xpypact-0.3.0/LICENSE
--rw-r--r--   0        0        0     3296 2023-04-11 10:08:01.831799 xpypact-0.3.0/README.rst
--rw-r--r--   0        0        0    17326 2023-04-11 10:08:14.379796 xpypact-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1199 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/__init__.py
--rw-r--r--   0        0        0      174 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/dao/__init__.py
--rw-r--r--   0        0        0     2241 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/dao/api.py
--rw-r--r--   0        0        0      168 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/dao/duckdb/__init__.py
--rw-r--r--   0        0        0     2870 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/dao/duckdb/create_schema.sql
--rw-r--r--   0        0        0     7790 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/dao/duckdb/implementation.py
--rw-r--r--   0        0        0    14156 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/data_arrays.py
--rw-r--r--   0        0        0     5307 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/data_frames.py
--rw-r--r--   0        0        0    12337 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/fluxes.py
--rw-r--r--   0        0        0     5862 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/inventory.py
--rw-r--r--   0        0        0     1965 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/nuclide.py
--rw-r--r--   0        0        0        0 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/py.typed
--rw-r--r--   0        0        0      515 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/run_data.py
--rw-r--r--   0        0        0     4924 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/time_step.py
--rw-r--r--   0        0        0       29 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/utils/__init__.py
--rw-r--r--   0        0        0      809 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/utils/io.py
--rw-r--r--   0        0        0        0 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/utils/py.typed
--rw-r--r--   0        0        0      768 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/utils/resource.py
--rw-r--r--   0        0        0      270 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/utils/types.py
--rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 xpypact-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-30 12:22:42.233936 xpypact-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3296 2023-04-30 12:22:42.233936 xpypact-0.4.0/README.rst
+-rw-r--r--   0        0        0    17341 2023-04-30 12:23:06.746078 xpypact-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1199 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/__init__.py
+-rw-r--r--   0        0        0      174 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/dao/__init__.py
+-rw-r--r--   0        0        0     2241 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/dao/api.py
+-rw-r--r--   0        0        0      168 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/dao/duckdb/__init__.py
+-rw-r--r--   0        0        0     2870 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/dao/duckdb/create_schema.sql
+-rw-r--r--   0        0        0     7971 2023-04-30 12:23:06.746078 xpypact-0.4.0/src/xpypact/dao/duckdb/implementation.py
+-rw-r--r--   0        0        0    14156 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/data_arrays.py
+-rw-r--r--   0        0        0     5307 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/data_frames.py
+-rw-r--r--   0        0        0    12337 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/fluxes.py
+-rw-r--r--   0        0        0     5862 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/inventory.py
+-rw-r--r--   0        0        0     1965 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/nuclide.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/py.typed
+-rw-r--r--   0        0        0      515 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/run_data.py
+-rw-r--r--   0        0        0     4924 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/time_step.py
+-rw-r--r--   0        0        0       29 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/utils/__init__.py
+-rw-r--r--   0        0        0      809 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/utils/io.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/utils/py.typed
+-rw-r--r--   0        0        0      768 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/utils/resource.py
+-rw-r--r--   0        0        0      270 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/utils/types.py
+-rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 xpypact-0.4.0/PKG-INFO
```

### Comparing `xpypact-0.3.0/LICENSE` & `xpypact-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xpypact-0.3.0/README.rst` & `xpypact-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `xpypact-0.3.0/pyproject.toml` & `xpypact-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xpypact"
-version = "0.3.0"
+version = "0.4.0"
 description = "\"Python tools to work with elements and isotopes\""
 authors = ["dvp <dmitri_portnov@yahoo.com>"]
 license = "MIT"
 homepage = "https://github.com/MC-kit/xpypact"
 repository = "https://github.com/MC-kit/xpypact"
 documentation = "https://xpypact.readthedocs.io"
 keywords = [
@@ -237,15 +237,15 @@
 xfail_strict = true
 filterwarnings = [
     "error",
     'ignore:Implementing implicit namespace packages \(as specified in PEP 420\) is preferred to `pkg_resources.declare_namespace`',
     "ignore:.*not typechecking multipledispatch.dispatcher.*UserWarning",
     'ignore:.*io.FileIO \[closed\]',
     'ignore:.*Deprecated call to `pkg_resources.declare_namespace',
-    'ignore:.*DeprecationWarning.*Implicit None on return values'
+    'ignore:.*Implicit None on return values:DeprecationWarning'
 ]
 log_format = "%(asctime)s %(levelname)s %(message)s"
 log_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.xdoctest]
 quiet = true
 options = ""
@@ -575,15 +575,15 @@
 "src/xpypact/fluxes.py" = ["F811"]
 "benchmarks/*" = ["S101"]
 "noxfile.py" = ["ANN"]
 "tests/*" = ["ANN", "D100", "D101", "D102", "D103", "D104",  "PLR2004", "S101"]
 "src/xpypact/inventory.py" = ["F811"]
 "src/xpypact/data_arrays.py" = ["ANN401", "PD011"]
 "src/xpypact/utils/resource.py" = ["ANN202"]
-"tools/*" = ["T201", "INP001"]
+"tools/*" = ["T201", "INP001", "S603", "S607"]
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.ruff.flake8-type-checking]
 strict = true
```

### Comparing `xpypact-0.3.0/src/xpypact/__init__.py` & `xpypact-0.4.0/src/xpypact/__init__.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.3.0/src/xpypact/dao/api.py` & `xpypact-0.4.0/src/xpypact/dao/api.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.3.0/src/xpypact/dao/duckdb/create_schema.sql` & `xpypact-0.4.0/src/xpypact/dao/duckdb/create_schema.sql`

 * *Files identical despite different names*

### Comparing `xpypact-0.3.0/src/xpypact/dao/duckdb/implementation.py` & `xpypact-0.4.0/src/xpypact/dao/duckdb/implementation.py`

 * *Files 8% similar despite different names*

```diff
@@ -200,20 +200,24 @@
             path: Path = target_dir / k
             path.mkdir(parents=True, exist_ok=True)
             frame = _add_material_and_case_columns(  # noqa: F841 - used in query
                 v,
                 material_id,
                 case_id,
             )
+            time_step_partition = "time_step_number, " if "time_step_number" in v.columns else ""
             sql = f"""
                 copy
                 (select * from frame)
-                to
-                '{path}'
-                (format parquet, partition_by (material_id, case_id), allow_overwrite 1)
+                to '{path}'
+                (
+                    format parquet,
+                    partition_by ({time_step_partition}material_id, case_id),
+                    allow_overwrite 1
+                )
                 """  # noqa: S608 - sql injection
             con.execute(sql)
     finally:
         con.close()
 
 
 def _add_material_and_case_columns(
```

### Comparing `xpypact-0.3.0/src/xpypact/data_arrays.py` & `xpypact-0.4.0/src/xpypact/data_arrays.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.3.0/src/xpypact/data_frames.py` & `xpypact-0.4.0/src/xpypact/data_frames.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.3.0/src/xpypact/fluxes.py` & `xpypact-0.4.0/src/xpypact/fluxes.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.3.0/src/xpypact/inventory.py` & `xpypact-0.4.0/src/xpypact/inventory.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.3.0/src/xpypact/nuclide.py` & `xpypact-0.4.0/src/xpypact/nuclide.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.3.0/src/xpypact/run_data.py` & `xpypact-0.4.0/src/xpypact/run_data.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.3.0/src/xpypact/time_step.py` & `xpypact-0.4.0/src/xpypact/time_step.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.3.0/src/xpypact/utils/io.py` & `xpypact-0.4.0/src/xpypact/utils/io.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.3.0/src/xpypact/utils/resource.py` & `xpypact-0.4.0/src/xpypact/utils/resource.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.3.0/PKG-INFO` & `xpypact-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpypact
-Version: 0.3.0
+Version: 0.4.0
 Summary: "Python tools to work with elements and isotopes"
 Home-page: https://github.com/MC-kit/xpypact
 License: MIT
 Keywords: element,nuclide,isotope,abundance,FISPACT,activation,duckdb,parquet
 Author: dvp
 Author-email: dmitri_portnov@yahoo.com
 Requires-Python: >=3.8.1,<4.0
```

