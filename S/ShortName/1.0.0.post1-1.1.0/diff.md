# Comparing `tmp/ShortName-1.0.0.post1.tar.gz` & `tmp/ShortName-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShortName-1.0.0.post1.tar", last modified: Sun Apr 30 00:15:00 2023, max compression
+gzip compressed data, was "ShortName-1.1.0.tar", last modified: Sun Apr 30 01:56:40 2023, max compression
```

## Comparing `ShortName-1.0.0.post1.tar` & `ShortName-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 00:15:00.169758 ShortName-1.0.0.post1/
--rw-rw-rw-   0        0        0      859 2023-04-29 22:36:24.000000 ShortName-1.0.0.post1/LICENSE
--rw-rw-rw-   0        0        0     5315 2023-04-30 00:15:00.168758 ShortName-1.0.0.post1/PKG-INFO
--rw-rw-rw-   0        0        0     4579 2023-04-30 00:10:30.000000 ShortName-1.0.0.post1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 00:15:00.168758 ShortName-1.0.0.post1/ShortName.egg-info/
--rw-rw-rw-   0        0        0     5315 2023-04-30 00:15:00.000000 ShortName-1.0.0.post1/ShortName.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-04-30 00:15:00.000000 ShortName-1.0.0.post1/ShortName.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 00:15:00.000000 ShortName-1.0.0.post1/ShortName.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-30 00:15:00.000000 ShortName-1.0.0.post1/ShortName.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2023-04-30 00:15:00.000000 ShortName-1.0.0.post1/ShortName.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-30 00:14:59.000000 ShortName-1.0.0.post1/ShortName.egg-info/zip-safe
--rw-rw-rw-   0        0        0     4409 2023-04-29 22:26:30.000000 ShortName-1.0.0.post1/ShortName.py
--rw-rw-rw-   0        0        0      964 2023-04-30 00:14:34.000000 ShortName-1.0.0.post1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 00:15:00.169758 ShortName-1.0.0.post1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 01:56:40.289893 ShortName-1.1.0/
+-rw-rw-rw-   0        0        0      859 2023-04-29 22:36:24.000000 ShortName-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5309 2023-04-30 01:56:40.288893 ShortName-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4579 2023-04-30 00:10:30.000000 ShortName-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 01:56:40.288893 ShortName-1.1.0/ShortName.egg-info/
+-rw-rw-rw-   0        0        0     5309 2023-04-30 01:56:40.000000 ShortName-1.1.0/ShortName.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-04-30 01:56:40.000000 ShortName-1.1.0/ShortName.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 01:56:40.000000 ShortName-1.1.0/ShortName.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-30 01:56:40.000000 ShortName-1.1.0/ShortName.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2023-04-30 01:56:40.000000 ShortName-1.1.0/ShortName.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-30 01:56:39.000000 ShortName-1.1.0/ShortName.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     4724 2023-04-30 01:52:52.000000 ShortName-1.1.0/ShortName.py
+-rw-rw-rw-   0        0        0      958 2023-04-30 01:52:52.000000 ShortName-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 01:56:40.289893 ShortName-1.1.0/setup.cfg
```

### Comparing `ShortName-1.0.0.post1/LICENSE` & `ShortName-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ShortName-1.0.0.post1/PKG-INFO` & `ShortName-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShortName
-Version: 1.0.0.post1
+Version: 1.1.0
 Summary: Command-line utility to view and modify 8.3-style short file names on Windows
 Author: Eta
 License: zlib/libpng License
 Project-URL: Homepage, https://github.com/Eta0/ShortName
 Keywords: windows,cli
 Platform: Win32 (MS Windows)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ShortName-1.0.0.post1/README.md` & `ShortName-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ShortName-1.0.0.post1/ShortName.egg-info/PKG-INFO` & `ShortName-1.1.0/ShortName.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShortName
-Version: 1.0.0.post1
+Version: 1.1.0
 Summary: Command-line utility to view and modify 8.3-style short file names on Windows
 Author: Eta
 License: zlib/libpng License
 Project-URL: Homepage, https://github.com/Eta0/ShortName
 Keywords: windows,cli
 Platform: Win32 (MS Windows)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ShortName-1.0.0.post1/ShortName.py` & `ShortName-1.1.0/ShortName.py`

 * *Files 11% similar despite different names*

```diff
@@ -55,32 +55,38 @@
             print(WinFile.get_short_name(lpszLongPath=args.file))
         except OSError:
             error(f"Could not retrieve shortname for file: {args.file}", 2)
 
 
 class WinFile:
     # Win32 constants
-    GENERIC_ALL = 1 << 28
+    DELETE = 0x00010000
     FILE_SHARE_DELETE, FILE_SHARE_WRITE, FILE_SHARE_READ = 0x4, 0x2, 0x1
     NULL = 0
     OPEN_EXISTING = 3
-    FILE_ATTRIBUTE_NORMAL = 0x80
+    FILE_FLAG_BACKUP_SEMANTICS = 0x02000000
     INVALID_HANDLE = -1
     MAX_PATH = 260
 
     def __init__(
         self,
         lpFileName: str,
-        dwDesiredAccess=GENERIC_ALL,  # GENERIC_ALL is required for SetFileShortName
+        dwDesiredAccess=DELETE,
         dwShareMode=FILE_SHARE_DELETE | FILE_SHARE_WRITE | FILE_SHARE_READ,
         lpSecurityAttributes=NULL,
         dwCreationDisposition=OPEN_EXISTING,
-        dwFlagsAndAttributes=FILE_ATTRIBUTE_NORMAL,
+        dwFlagsAndAttributes=FILE_FLAG_BACKUP_SEMANTICS,
         hTemplateFile=NULL,
     ):
+        # To change the short name of a file later, it must be opened with either:
+        # 1. dwDesiredAccess=GENERIC_ALL, or
+        # 2. dwDesiredAccess=DELETE and dwFlagsAndAttributes=FILE_FLAG_BACKUP_SEMANTICS
+        # FILE_FLAG_BACKUP_SEMANTICS is necessary for opening directories anyway,
+        # so this defaults to the latter option.
+
         # https://learn.microsoft.com/en-us/windows/win32/api/fileapi/nf-fileapi-createfilew
         self.handle = ctypes.windll.kernel32.CreateFileW(
             self.get_long_path(lpFileName),
             dwDesiredAccess,
             dwShareMode,
             lpSecurityAttributes,
             dwCreationDisposition,
```

### Comparing `ShortName-1.0.0.post1/pyproject.toml` & `ShortName-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ShortName"
-version = "1.0.0.post1"
+version = "1.1.0"
 license = { text = "zlib/libpng License" }
 keywords = ["windows", "cli"]
 authors = [
   { name="Eta" }
 ]
 description = "Command-line utility to view and modify 8.3-style short file names on Windows"
 readme = "README.md"
```

