# Comparing `tmp/ShortName-1.0.0.tar.gz` & `tmp/ShortName-1.0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShortName-1.0.0.tar", last modified: Sun Apr 30 00:01:55 2023, max compression
+gzip compressed data, was "ShortName-1.0.0.post1.tar", last modified: Sun Apr 30 00:15:00 2023, max compression
```

## Comparing `ShortName-1.0.0.tar` & `ShortName-1.0.0.post1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 00:01:55.142918 ShortName-1.0.0/
--rw-rw-rw-   0        0        0      859 2023-04-29 22:36:24.000000 ShortName-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4893 2023-04-30 00:01:55.141919 ShortName-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4163 2023-04-29 23:51:56.000000 ShortName-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 00:01:55.141919 ShortName-1.0.0/ShortName.egg-info/
--rw-rw-rw-   0        0        0     4893 2023-04-30 00:01:55.000000 ShortName-1.0.0/ShortName.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-04-30 00:01:55.000000 ShortName-1.0.0/ShortName.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 00:01:55.000000 ShortName-1.0.0/ShortName.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-30 00:01:55.000000 ShortName-1.0.0/ShortName.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2023-04-30 00:01:55.000000 ShortName-1.0.0/ShortName.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-30 00:01:54.000000 ShortName-1.0.0/ShortName.egg-info/zip-safe
--rw-rw-rw-   0        0        0     4409 2023-04-29 22:26:30.000000 ShortName-1.0.0/ShortName.py
--rw-rw-rw-   0        0        0      958 2023-04-29 23:41:39.000000 ShortName-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 00:01:55.142918 ShortName-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 00:15:00.169758 ShortName-1.0.0.post1/
+-rw-rw-rw-   0        0        0      859 2023-04-29 22:36:24.000000 ShortName-1.0.0.post1/LICENSE
+-rw-rw-rw-   0        0        0     5315 2023-04-30 00:15:00.168758 ShortName-1.0.0.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     4579 2023-04-30 00:10:30.000000 ShortName-1.0.0.post1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 00:15:00.168758 ShortName-1.0.0.post1/ShortName.egg-info/
+-rw-rw-rw-   0        0        0     5315 2023-04-30 00:15:00.000000 ShortName-1.0.0.post1/ShortName.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-04-30 00:15:00.000000 ShortName-1.0.0.post1/ShortName.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 00:15:00.000000 ShortName-1.0.0.post1/ShortName.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-30 00:15:00.000000 ShortName-1.0.0.post1/ShortName.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2023-04-30 00:15:00.000000 ShortName-1.0.0.post1/ShortName.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-30 00:14:59.000000 ShortName-1.0.0.post1/ShortName.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     4409 2023-04-29 22:26:30.000000 ShortName-1.0.0.post1/ShortName.py
+-rw-rw-rw-   0        0        0      964 2023-04-30 00:14:34.000000 ShortName-1.0.0.post1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 00:15:00.169758 ShortName-1.0.0.post1/setup.cfg
```

### Comparing `ShortName-1.0.0/LICENSE` & `ShortName-1.0.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `ShortName-1.0.0/PKG-INFO` & `ShortName-1.0.0.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShortName
-Version: 1.0.0
+Version: 1.0.0.post1
 Summary: Command-line utility to view and modify 8.3-style short file names on Windows
 Author: Eta
 License: zlib/libpng License
 Project-URL: Homepage, https://github.com/Eta0/ShortName
 Keywords: windows,cli
 Platform: Win32 (MS Windows)
 Classifier: Programming Language :: Python :: 3
@@ -24,14 +24,15 @@
 [8.3-style short file names](https://learn.microsoft.com/en-us/windows/win32/fileio/naming-a-file#short-vs-long-names)
 on Windows, with no dependencies.
 
 ## Table of Contents
 
 - [What Is This?](#what-is-this)
 - [Setup](#setup)
+  - [As a Script](#as-a-script)
   - [Optional Installation](#optional-installation)
 - [Usage](#usage)
   - [View the Short Name of a File](#view-the-short-name-of-a-file)
   - [Set the Short Name of a File](#set-the-short-name-of-a-file)
 - [License](#license)
 
 ## What Is This?
@@ -53,35 +54,48 @@
 
 If the full path to `some_long_file_name.txt` is `C:\Files\some_long_file_name.txt`,
 you can now refer to it almost everywhere as `C:\Files\short.txt` as well;
 `notepad C:\Files\short.txt` will open the same file as `notepad C:\Files\some_long_file_name.txt`.
 
 ## Setup
 
-1. Install [Python 3](https://www.python.org/downloads/), if you don't have it
-2. [Download `ShortName.py`](https://raw.githubusercontent.com/Eta0/ShortName/main/ShortName.py)
+You can run ShortName either as a single-file script `ShortName.py`,
+or install it to run it more easily from anywhere.
 
-Installing ShortName itself is not necessary, as it has no dependencies.
-You can use it immediately as a script, e.g.:
+Regardless of the method, you first need to [install Python 3](https://www.python.org/downloads/) if you don't have it.
+
+### As a Script
+
+- [Download `ShortName.py`](https://raw.githubusercontent.com/Eta0/ShortName/main/ShortName.py)
+
+No further installation is required, as it has no dependencies. You can use it immediately as a script, e.g.:
 
 ```cmd
 python ShortName.py get .\some_long_file_name.txt
 ```
 
 ### Optional Installation
 
-If you wish to install ShortName anyway—for example, to invoke it from anywhere—you can:
+If you wish to install ShortName—for example, to invoke it from anywhere—you can run:
+
+```cmd
+python -m pip install ShortName
+```
+To install [ShortName via PyPI](https://pypi.org/project/ShortName/1.0.0).
+
+Alternatively, you can:
 
 1. [Download the ShortName repository](https://github.com/Eta0/ShortName/archive/refs/heads/main.zip)
 2. Unzip it
 3. Run `python -m pip install <path to unzipped directory>`
 
-Then you should be able to invoke `ShortName` from anywhere, in either of the following two ways:
+Regardless of which of installation method you choose, you should then be able to invoke `ShortName` from anywhere,
+in either of the following two ways:
 
-1. `python -m ShortName get .\some_long_file_name.txt`
+1. `python -m ShortName get .\some_long_file_name.txt`, or
 2. `ShortName get .\some_long_file_name.txt`
 
 To uninstall it, run:
 
 ```cmd
 python -m pip uninstall ShortName
 ```
```

### Comparing `ShortName-1.0.0/README.md` & `ShortName-1.0.0.post1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 [8.3-style short file names](https://learn.microsoft.com/en-us/windows/win32/fileio/naming-a-file#short-vs-long-names)
 on Windows, with no dependencies.
 
 ## Table of Contents
 
 - [What Is This?](#what-is-this)
 - [Setup](#setup)
+  - [As a Script](#as-a-script)
   - [Optional Installation](#optional-installation)
 - [Usage](#usage)
   - [View the Short Name of a File](#view-the-short-name-of-a-file)
   - [Set the Short Name of a File](#set-the-short-name-of-a-file)
 - [License](#license)
 
 ## What Is This?
@@ -33,35 +34,48 @@
 
 If the full path to `some_long_file_name.txt` is `C:\Files\some_long_file_name.txt`,
 you can now refer to it almost everywhere as `C:\Files\short.txt` as well;
 `notepad C:\Files\short.txt` will open the same file as `notepad C:\Files\some_long_file_name.txt`.
 
 ## Setup
 
-1. Install [Python 3](https://www.python.org/downloads/), if you don't have it
-2. [Download `ShortName.py`](https://raw.githubusercontent.com/Eta0/ShortName/main/ShortName.py)
+You can run ShortName either as a single-file script `ShortName.py`,
+or install it to run it more easily from anywhere.
 
-Installing ShortName itself is not necessary, as it has no dependencies.
-You can use it immediately as a script, e.g.:
+Regardless of the method, you first need to [install Python 3](https://www.python.org/downloads/) if you don't have it.
+
+### As a Script
+
+- [Download `ShortName.py`](https://raw.githubusercontent.com/Eta0/ShortName/main/ShortName.py)
+
+No further installation is required, as it has no dependencies. You can use it immediately as a script, e.g.:
 
 ```cmd
 python ShortName.py get .\some_long_file_name.txt
 ```
 
 ### Optional Installation
 
-If you wish to install ShortName anyway—for example, to invoke it from anywhere—you can:
+If you wish to install ShortName—for example, to invoke it from anywhere—you can run:
+
+```cmd
+python -m pip install ShortName
+```
+To install [ShortName via PyPI](https://pypi.org/project/ShortName/1.0.0).
+
+Alternatively, you can:
 
 1. [Download the ShortName repository](https://github.com/Eta0/ShortName/archive/refs/heads/main.zip)
 2. Unzip it
 3. Run `python -m pip install <path to unzipped directory>`
 
-Then you should be able to invoke `ShortName` from anywhere, in either of the following two ways:
+Regardless of which of installation method you choose, you should then be able to invoke `ShortName` from anywhere,
+in either of the following two ways:
 
-1. `python -m ShortName get .\some_long_file_name.txt`
+1. `python -m ShortName get .\some_long_file_name.txt`, or
 2. `ShortName get .\some_long_file_name.txt`
 
 To uninstall it, run:
 
 ```cmd
 python -m pip uninstall ShortName
 ```
```

### Comparing `ShortName-1.0.0/ShortName.egg-info/PKG-INFO` & `ShortName-1.0.0.post1/ShortName.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShortName
-Version: 1.0.0
+Version: 1.0.0.post1
 Summary: Command-line utility to view and modify 8.3-style short file names on Windows
 Author: Eta
 License: zlib/libpng License
 Project-URL: Homepage, https://github.com/Eta0/ShortName
 Keywords: windows,cli
 Platform: Win32 (MS Windows)
 Classifier: Programming Language :: Python :: 3
@@ -24,14 +24,15 @@
 [8.3-style short file names](https://learn.microsoft.com/en-us/windows/win32/fileio/naming-a-file#short-vs-long-names)
 on Windows, with no dependencies.
 
 ## Table of Contents
 
 - [What Is This?](#what-is-this)
 - [Setup](#setup)
+  - [As a Script](#as-a-script)
   - [Optional Installation](#optional-installation)
 - [Usage](#usage)
   - [View the Short Name of a File](#view-the-short-name-of-a-file)
   - [Set the Short Name of a File](#set-the-short-name-of-a-file)
 - [License](#license)
 
 ## What Is This?
@@ -53,35 +54,48 @@
 
 If the full path to `some_long_file_name.txt` is `C:\Files\some_long_file_name.txt`,
 you can now refer to it almost everywhere as `C:\Files\short.txt` as well;
 `notepad C:\Files\short.txt` will open the same file as `notepad C:\Files\some_long_file_name.txt`.
 
 ## Setup
 
-1. Install [Python 3](https://www.python.org/downloads/), if you don't have it
-2. [Download `ShortName.py`](https://raw.githubusercontent.com/Eta0/ShortName/main/ShortName.py)
+You can run ShortName either as a single-file script `ShortName.py`,
+or install it to run it more easily from anywhere.
 
-Installing ShortName itself is not necessary, as it has no dependencies.
-You can use it immediately as a script, e.g.:
+Regardless of the method, you first need to [install Python 3](https://www.python.org/downloads/) if you don't have it.
+
+### As a Script
+
+- [Download `ShortName.py`](https://raw.githubusercontent.com/Eta0/ShortName/main/ShortName.py)
+
+No further installation is required, as it has no dependencies. You can use it immediately as a script, e.g.:
 
 ```cmd
 python ShortName.py get .\some_long_file_name.txt
 ```
 
 ### Optional Installation
 
-If you wish to install ShortName anyway—for example, to invoke it from anywhere—you can:
+If you wish to install ShortName—for example, to invoke it from anywhere—you can run:
+
+```cmd
+python -m pip install ShortName
+```
+To install [ShortName via PyPI](https://pypi.org/project/ShortName/1.0.0).
+
+Alternatively, you can:
 
 1. [Download the ShortName repository](https://github.com/Eta0/ShortName/archive/refs/heads/main.zip)
 2. Unzip it
 3. Run `python -m pip install <path to unzipped directory>`
 
-Then you should be able to invoke `ShortName` from anywhere, in either of the following two ways:
+Regardless of which of installation method you choose, you should then be able to invoke `ShortName` from anywhere,
+in either of the following two ways:
 
-1. `python -m ShortName get .\some_long_file_name.txt`
+1. `python -m ShortName get .\some_long_file_name.txt`, or
 2. `ShortName get .\some_long_file_name.txt`
 
 To uninstall it, run:
 
 ```cmd
 python -m pip uninstall ShortName
 ```
```

### Comparing `ShortName-1.0.0/ShortName.py` & `ShortName-1.0.0.post1/ShortName.py`

 * *Files identical despite different names*

### Comparing `ShortName-1.0.0/pyproject.toml` & `ShortName-1.0.0.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ShortName"
-version = "1.0.0"
+version = "1.0.0.post1"
 license = { text = "zlib/libpng License" }
 keywords = ["windows", "cli"]
 authors = [
   { name="Eta" }
 ]
 description = "Command-line utility to view and modify 8.3-style short file names on Windows"
 readme = "README.md"
```

