# Comparing `tmp/shipper-shippy-1.9.0a4.tar.gz` & `tmp/shipper-shippy-1.9.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipper-shippy-1.9.0a4.tar", last modified: Sun Jan  8 03:31:43 2023, max compression
+gzip compressed data, was "shipper-shippy-1.9.0a5.tar", last modified: Sun Jan  8 03:46:02 2023, max compression
```

## Comparing `shipper-shippy-1.9.0a4.tar` & `shipper-shippy-1.9.0a5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 03:31:43.763034 shipper-shippy-1.9.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-08 03:31:33.000000 shipper-shippy-1.9.0a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-01-08 03:31:43.763034 shipper-shippy-1.9.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-01-08 03:31:33.000000 shipper-shippy-1.9.0a4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-08 03:31:33.000000 shipper-shippy-1.9.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-08 03:31:43.763034 shipper-shippy-1.9.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-01-08 03:31:33.000000 shipper-shippy-1.9.0a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 03:31:43.763034 shipper-shippy-1.9.0a4/shipper_shippy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-01-08 03:31:43.000000 shipper-shippy-1.9.0a4/shipper_shippy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-01-08 03:31:43.000000 shipper-shippy-1.9.0a4/shipper_shippy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-08 03:31:43.000000 shipper-shippy-1.9.0a4/shipper_shippy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-08 03:31:43.000000 shipper-shippy-1.9.0a4/shipper_shippy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-08 03:31:43.000000 shipper-shippy-1.9.0a4/shipper_shippy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-08 03:31:43.000000 shipper-shippy-1.9.0a4/shipper_shippy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 03:31:43.763034 shipper-shippy-1.9.0a4/shippy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 03:31:33.000000 shipper-shippy-1.9.0a4/shippy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-01-08 03:31:33.000000 shipper-shippy-1.9.0a4/shippy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-01-08 03:31:33.000000 shipper-shippy-1.9.0a4/shippy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-08 03:31:33.000000 shipper-shippy-1.9.0a4/shippy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-01-08 03:31:33.000000 shipper-shippy-1.9.0a4/shippy/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-08 03:31:33.000000 shipper-shippy-1.9.0a4/shippy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-01-08 03:31:33.000000 shipper-shippy-1.9.0a4/shippy/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-08 03:31:33.000000 shipper-shippy-1.9.0a4/shippy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 03:46:02.171043 shipper-shippy-1.9.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-01-08 03:46:02.171043 shipper-shippy-1.9.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-08 03:46:02.171043 shipper-shippy-1.9.0a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 03:46:02.171043 shipper-shippy-1.9.0a5/shipper_shippy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-01-08 03:46:01.000000 shipper-shippy-1.9.0a5/shipper_shippy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-01-08 03:46:01.000000 shipper-shippy-1.9.0a5/shipper_shippy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-08 03:46:01.000000 shipper-shippy-1.9.0a5/shipper_shippy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-08 03:46:01.000000 shipper-shippy-1.9.0a5/shipper_shippy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-08 03:46:01.000000 shipper-shippy-1.9.0a5/shipper_shippy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-08 03:46:01.000000 shipper-shippy-1.9.0a5/shipper_shippy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 03:46:02.171043 shipper-shippy-1.9.0a5/shippy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/shippy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/shippy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/shippy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/shippy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/shippy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/shippy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/shippy/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-08 03:45:51.000000 shipper-shippy-1.9.0a5/shippy/version.py
```

### Comparing `shipper-shippy-1.9.0a4/LICENSE` & `shipper-shippy-1.9.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `shipper-shippy-1.9.0a4/PKG-INFO` & `shipper-shippy-1.9.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 1.9.0a4
+Version: 1.9.0a5
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shipper-shippy-1.9.0a4/README.md` & `shipper-shippy-1.9.0a5/README.md`

 * *Files identical despite different names*

### Comparing `shipper-shippy-1.9.0a4/setup.py` & `shipper-shippy-1.9.0a5/setup.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-1.9.0a4/shipper_shippy.egg-info/PKG-INFO` & `shipper-shippy-1.9.0a5/shipper_shippy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 1.9.0a4
+Version: 1.9.0a5
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shipper-shippy-1.9.0a4/shippy/__main__.py` & `shipper-shippy-1.9.0a5/shippy/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,71 +239,68 @@
                 builds.append(file)
 
         return builds
 
 
 def check_build(filename):
     """Makes sure the build is valid"""
-    with console.status(f"Validating build {filename}..."):
-        # Validate that there is a matching checksum file
-        has_checksum_file_type, has_sum_postfix = find_checksum_file(filename=filename)
-
-        if has_checksum_file_type is None:
-            print_warning(
-                "This build does not have a matching checksum file. ", newline=False
+    print(f"Validating build {filename}...")
+    # Validate that there is a matching checksum file
+    has_checksum_file_type, has_sum_postfix = find_checksum_file(filename=filename)
+
+    if has_checksum_file_type is None:
+        print_warning(
+            "This build does not have a matching checksum file. ", newline=False
+        )
+        return False
+
+    # Validate checksum
+    with console.status(f"Checking {has_checksum_file_type.upper()} hash..."):
+        hash_val = get_hash_of_file(
+            filename=filename, checksum_type=has_checksum_file_type
+        )
+        if not has_sum_postfix:
+            actual_hash_val = get_hash_from_checksum_file(
+                f"{filename}.{has_checksum_file_type}"
             )
-            return False
-
-        # Validate checksum
-        with console.status(
-            f"Checking {has_checksum_file_type.upper()} hash of {filename}... this may "
-            "take a couple of seconds. "
-        ):
-            hash_val = get_hash_of_file(
-                filename=filename, checksum_type=has_checksum_file_type
-            )
-            if not has_sum_postfix:
-                actual_hash_val = get_hash_from_checksum_file(
-                    f"{filename}.{has_checksum_file_type}"
-                )
-            else:
-                actual_hash_val = get_hash_from_checksum_file(
-                    f"{filename}.{has_checksum_file_type}sum"
-                )
-            if hash_val != actual_hash_val:
-                print_error(
-                    msg="This build's checksum is invalid. ",
-                    newline=False,
-                    exit_after=False,
-                )
-                return False
-            print_success(f"{has_checksum_file_type.upper()} matched!")
-
-        build_slug, _ = os.path.splitext(filename)
-        _, _, _, build_type, build_variant, _ = build_slug.split("-")
-
-        # Check build type
-        if build_type != "OFFICIAL":
-            print_error(
-                msg="This build is not official. ", newline=False, exit_after=False
+        else:
+            actual_hash_val = get_hash_from_checksum_file(
+                f"{filename}.{has_checksum_file_type}sum"
             )
-            return False
-
-        # Check build variant
-        valid_variants = ["gapps", "vanilla", "foss", "goapps"]
-        if build_variant not in valid_variants:
+        if hash_val != actual_hash_val:
             print_error(
-                msg="This build has an unknown variant. ",
+                msg="This build's checksum is invalid. ",
                 newline=False,
                 exit_after=False,
             )
             return False
+        print_success(f"Success!")
+
+    build_slug, _ = os.path.splitext(filename)
+    _, _, _, build_type, build_variant, _ = build_slug.split("-")
+
+    # Check build type
+    if build_type != "OFFICIAL":
+        print_error(
+            msg="This build is not official. ", newline=False, exit_after=False
+        )
+        return False
+
+    # Check build variant
+    valid_variants = ["gapps", "vanilla", "foss", "goapps"]
+    if build_variant not in valid_variants:
+        print_error(
+            msg="This build has an unknown variant. ",
+            newline=False,
+            exit_after=False,
+        )
+        return False
 
-        print_success(f"Validation of build {filename} complete. No problems found.")
-        return True
+    print_success(f"Validation of build {filename} complete. No problems found.")
+    return True
 
 
 def get_server_url():
     try:
         while True:
             server_url = input("Enter the server URL: ")
             if not check_server_url_schema(server_url):
```

### Comparing `shipper-shippy-1.9.0a4/shippy/client.py` & `shipper-shippy-1.9.0a5/shippy/client.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-1.9.0a4/shippy/config.py` & `shipper-shippy-1.9.0a5/shippy/config.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-1.9.0a4/shippy/constants.py` & `shipper-shippy-1.9.0a5/shippy/constants.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-1.9.0a4/shippy/helper.py` & `shipper-shippy-1.9.0a5/shippy/helper.py`

 * *Files identical despite different names*

