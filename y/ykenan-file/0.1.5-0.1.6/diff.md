# Comparing `tmp/ykenan_file-0.1.5.tar.gz` & `tmp/ykenan_file-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_file-0.1.5.tar", last modified: Sun Apr 30 11:40:48 2023, max compression
+gzip compressed data, was "ykenan_file-0.1.6.tar", last modified: Sun Apr 30 11:46:14 2023, max compression
```

## Comparing `ykenan_file-0.1.5.tar` & `ykenan_file-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 11:40:48.572468 ykenan_file-0.1.5/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      829 2023-04-30 11:40:48.571468 ykenan_file-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-04-21 09:34:27.000000 ykenan_file-0.1.5/README.md
--rw-rw-rw-   0        0        0      676 2023-04-30 11:39:51.000000 ykenan_file-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       32 2023-03-22 07:40:08.000000 ykenan_file-0.1.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 11:40:48.572468 ykenan_file-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-30 11:40:48.548468 ykenan_file-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 11:40:48.560469 ykenan_file-0.1.5/src/ykenan_file/
--rw-rw-rw-   0        0        0    23829 2023-04-30 11:39:51.000000 ykenan_file-0.1.5/src/ykenan_file/__init__.py
--rw-rw-rw-   0        0        0      157 2023-04-06 01:49:10.000000 ykenan_file-0.1.5/src/ykenan_file/util.py
-drwxrwxrwx   0        0        0        0 2023-04-30 11:40:48.569468 ykenan_file-0.1.5/src/ykenan_file.egg-info/
--rw-rw-rw-   0        0        0      829 2023-04-30 11:40:48.000000 ykenan_file-0.1.5/src/ykenan_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-30 11:40:48.000000 ykenan_file-0.1.5/src/ykenan_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 11:40:48.000000 ykenan_file-0.1.5/src/ykenan_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-30 11:40:48.000000 ykenan_file-0.1.5/src/ykenan_file.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-30 11:40:48.000000 ykenan_file-0.1.5/src/ykenan_file.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 11:46:14.686725 ykenan_file-0.1.6/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      829 2023-04-30 11:46:14.685723 ykenan_file-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-04-21 09:34:27.000000 ykenan_file-0.1.6/README.md
+-rw-rw-rw-   0        0        0      676 2023-04-30 11:45:23.000000 ykenan_file-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       32 2023-03-22 07:40:08.000000 ykenan_file-0.1.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 11:46:14.686725 ykenan_file-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 11:46:14.662724 ykenan_file-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 11:46:14.674723 ykenan_file-0.1.6/src/ykenan_file/
+-rw-rw-rw-   0        0        0    23874 2023-04-30 11:45:10.000000 ykenan_file-0.1.6/src/ykenan_file/__init__.py
+-rw-rw-rw-   0        0        0      157 2023-04-06 01:49:10.000000 ykenan_file-0.1.6/src/ykenan_file/util.py
+drwxrwxrwx   0        0        0        0 2023-04-30 11:46:14.683723 ykenan_file-0.1.6/src/ykenan_file.egg-info/
+-rw-rw-rw-   0        0        0      829 2023-04-30 11:46:14.000000 ykenan_file-0.1.6/src/ykenan_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-30 11:46:14.000000 ykenan_file-0.1.6/src/ykenan_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 11:46:14.000000 ykenan_file-0.1.6/src/ykenan_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-30 11:46:14.000000 ykenan_file-0.1.6/src/ykenan_file.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-30 11:46:14.000000 ykenan_file-0.1.6/src/ykenan_file.egg-info/top_level.txt
```

### Comparing `ykenan_file-0.1.5/LICENSE` & `ykenan_file-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_file-0.1.5/PKG-INFO` & `ykenan_file-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_file
-Version: 0.1.5
+Version: 0.1.6
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_file-0.1.5/pyproject.toml` & `ykenan_file-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_file"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "file", "read", "write"]
 description = "File read and write operations"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `ykenan_file-0.1.5/src/ykenan_file/__init__.py` & `ykenan_file-0.1.6/src/ykenan_file/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,16 +154,17 @@
         :param column: 需要和的列
         :param output_file: Output file path
         :return:
         """
         # 总和
         self.log.debug(f"通过分组计算某列数总和: {group}, {column}")
         column_sum = df.groupby(group)[column].sum().reset_index()
-        group.append(f"{column}_sum")
-        column_sum.columns = group
+        new_column = group.copy()
+        new_column.append(f"{column}_sum")
+        column_sum.columns = new_column
         # 保存文件
         if output_file is not None:
             self.to_file(column_sum, output_file)
         return column_sum
 
     def count_group_by(self, df: DataFrame, group: list, column: str, output_file: str = None) -> DataFrame:
         """
```

### Comparing `ykenan_file-0.1.5/src/ykenan_file.egg-info/PKG-INFO` & `ykenan_file-0.1.6/src/ykenan_file.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-file
-Version: 0.1.5
+Version: 0.1.6
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

