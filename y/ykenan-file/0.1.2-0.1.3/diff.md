# Comparing `tmp/ykenan_file-0.1.2.tar.gz` & `tmp/ykenan_file-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_file-0.1.2.tar", last modified: Fri Apr 28 06:35:32 2023, max compression
+gzip compressed data, was "ykenan_file-0.1.3.tar", last modified: Sat Apr 29 22:30:10 2023, max compression
```

## Comparing `ykenan_file-0.1.2.tar` & `ykenan_file-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 06:35:32.440379 ykenan_file-0.1.2/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      829 2023-04-28 06:35:32.439379 ykenan_file-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-04-21 09:34:27.000000 ykenan_file-0.1.2/README.md
--rw-rw-rw-   0        0        0      676 2023-04-28 06:33:51.000000 ykenan_file-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       32 2023-03-22 07:40:08.000000 ykenan_file-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 06:35:32.440379 ykenan_file-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 06:35:32.415381 ykenan_file-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 06:35:32.428381 ykenan_file-0.1.2/src/ykenan_file/
--rw-rw-rw-   0        0        0    23401 2023-04-28 06:33:22.000000 ykenan_file-0.1.2/src/ykenan_file/__init__.py
--rw-rw-rw-   0        0        0      157 2023-04-06 01:49:10.000000 ykenan_file-0.1.2/src/ykenan_file/util.py
-drwxrwxrwx   0        0        0        0 2023-04-28 06:35:32.437379 ykenan_file-0.1.2/src/ykenan_file.egg-info/
--rw-rw-rw-   0        0        0      829 2023-04-28 06:35:32.000000 ykenan_file-0.1.2/src/ykenan_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-28 06:35:32.000000 ykenan_file-0.1.2/src/ykenan_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 06:35:32.000000 ykenan_file-0.1.2/src/ykenan_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-28 06:35:32.000000 ykenan_file-0.1.2/src/ykenan_file.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-28 06:35:32.000000 ykenan_file-0.1.2/src/ykenan_file.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 22:30:10.357571 ykenan_file-0.1.3/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      829 2023-04-29 22:30:10.357571 ykenan_file-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-04-21 09:34:27.000000 ykenan_file-0.1.3/README.md
+-rw-rw-rw-   0        0        0      676 2023-04-29 22:28:52.000000 ykenan_file-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       32 2023-03-22 07:40:08.000000 ykenan_file-0.1.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 22:30:10.357571 ykenan_file-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 22:30:10.333574 ykenan_file-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-29 22:30:10.345573 ykenan_file-0.1.3/src/ykenan_file/
+-rw-rw-rw-   0        0        0    23397 2023-04-29 22:28:52.000000 ykenan_file-0.1.3/src/ykenan_file/__init__.py
+-rw-rw-rw-   0        0        0      157 2023-04-06 01:49:10.000000 ykenan_file-0.1.3/src/ykenan_file/util.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:30:10.355572 ykenan_file-0.1.3/src/ykenan_file.egg-info/
+-rw-rw-rw-   0        0        0      829 2023-04-29 22:30:10.000000 ykenan_file-0.1.3/src/ykenan_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-29 22:30:10.000000 ykenan_file-0.1.3/src/ykenan_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 22:30:10.000000 ykenan_file-0.1.3/src/ykenan_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-29 22:30:10.000000 ykenan_file-0.1.3/src/ykenan_file.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 22:30:10.000000 ykenan_file-0.1.3/src/ykenan_file.egg-info/top_level.txt
```

### Comparing `ykenan_file-0.1.2/LICENSE` & `ykenan_file-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_file-0.1.2/PKG-INFO` & `ykenan_file-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_file
-Version: 0.1.2
+Version: 0.1.3
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_file-0.1.2/pyproject.toml` & `ykenan_file-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_file"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "file", "read", "write"]
 description = "File read and write operations"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `ykenan_file-0.1.2/src/ykenan_file/__init__.py` & `ykenan_file-0.1.3/src/ykenan_file/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -554,15 +554,15 @@
         dirs: list = []
         contents: list = []
         dict_: dict = {}
         with os.scandir(path) as it:
             for entry in it:
                 entry: os.DirEntry
                 # 判断是否满足情况
-                if suffix is None or entry.name.endswith(entry.name):
+                if suffix is None or entry.name.endswith(suffix):
                     if type_ == 0:
                         dict_ = dict(itertools.chain(dict_.items(), {
                             entry.name: entry.path
                         }.items()))
                         contents.append(entry.name)
                     elif type_ == 1:
                         # 此处判断不能和 type_ == 1 连写，因为需要进行提示 ValueError("type input error, type is 0 or 1 or 2.")
```

### Comparing `ykenan_file-0.1.2/src/ykenan_file.egg-info/PKG-INFO` & `ykenan_file-0.1.3/src/ykenan_file.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-file
-Version: 0.1.2
+Version: 0.1.3
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

