# Comparing `tmp/ykenan_file-0.1.3.tar.gz` & `tmp/ykenan_file-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_file-0.1.3.tar", last modified: Sat Apr 29 22:30:10 2023, max compression
+gzip compressed data, was "ykenan_file-0.1.4.tar", last modified: Sun Apr 30 11:06:46 2023, max compression
```

## Comparing `ykenan_file-0.1.3.tar` & `ykenan_file-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 22:30:10.357571 ykenan_file-0.1.3/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      829 2023-04-29 22:30:10.357571 ykenan_file-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-04-21 09:34:27.000000 ykenan_file-0.1.3/README.md
--rw-rw-rw-   0        0        0      676 2023-04-29 22:28:52.000000 ykenan_file-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       32 2023-03-22 07:40:08.000000 ykenan_file-0.1.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 22:30:10.357571 ykenan_file-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-29 22:30:10.333574 ykenan_file-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-29 22:30:10.345573 ykenan_file-0.1.3/src/ykenan_file/
--rw-rw-rw-   0        0        0    23397 2023-04-29 22:28:52.000000 ykenan_file-0.1.3/src/ykenan_file/__init__.py
--rw-rw-rw-   0        0        0      157 2023-04-06 01:49:10.000000 ykenan_file-0.1.3/src/ykenan_file/util.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:30:10.355572 ykenan_file-0.1.3/src/ykenan_file.egg-info/
--rw-rw-rw-   0        0        0      829 2023-04-29 22:30:10.000000 ykenan_file-0.1.3/src/ykenan_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-29 22:30:10.000000 ykenan_file-0.1.3/src/ykenan_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 22:30:10.000000 ykenan_file-0.1.3/src/ykenan_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-29 22:30:10.000000 ykenan_file-0.1.3/src/ykenan_file.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 22:30:10.000000 ykenan_file-0.1.3/src/ykenan_file.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 11:06:46.346327 ykenan_file-0.1.4/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      829 2023-04-30 11:06:46.346327 ykenan_file-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-04-21 09:34:27.000000 ykenan_file-0.1.4/README.md
+-rw-rw-rw-   0        0        0      676 2023-04-30 11:04:10.000000 ykenan_file-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       32 2023-03-22 07:40:08.000000 ykenan_file-0.1.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 11:06:46.346327 ykenan_file-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 11:06:46.323328 ykenan_file-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 11:06:46.334326 ykenan_file-0.1.4/src/ykenan_file/
+-rw-rw-rw-   0        0        0    23424 2023-04-30 11:03:28.000000 ykenan_file-0.1.4/src/ykenan_file/__init__.py
+-rw-rw-rw-   0        0        0      157 2023-04-06 01:49:10.000000 ykenan_file-0.1.4/src/ykenan_file/util.py
+drwxrwxrwx   0        0        0        0 2023-04-30 11:06:46.344326 ykenan_file-0.1.4/src/ykenan_file.egg-info/
+-rw-rw-rw-   0        0        0      829 2023-04-30 11:06:46.000000 ykenan_file-0.1.4/src/ykenan_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-30 11:06:46.000000 ykenan_file-0.1.4/src/ykenan_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 11:06:46.000000 ykenan_file-0.1.4/src/ykenan_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-30 11:06:46.000000 ykenan_file-0.1.4/src/ykenan_file.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-30 11:06:46.000000 ykenan_file-0.1.4/src/ykenan_file.egg-info/top_level.txt
```

### Comparing `ykenan_file-0.1.3/LICENSE` & `ykenan_file-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_file-0.1.3/PKG-INFO` & `ykenan_file-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_file
-Version: 0.1.3
+Version: 0.1.4
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_file-0.1.3/pyproject.toml` & `ykenan_file-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_file"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "file", "read", "write"]
 description = "File read and write operations"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `ykenan_file-0.1.3/src/ykenan_file/__init__.py` & `ykenan_file-0.1.4/src/ykenan_file/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         group.append(f"{column}_count")
         column_sum.columns = group
         # 保存文件
         if output_file is not None:
             self.to_file(column_sum, output_file)
         return column_sum
 
-    def calculation_group_by(self, df: DataFrame, group: list, column: str, on: str, output_file: str = None, add_merge_files: list = None):
+    def calculation_group_by(self, df: DataFrame, group: list, column: str, on: str, output_file: str = None, add_merge_files: list = None) -> DataFrame:
         """
         通过分组进行一系列数值计算
         :param df: DataFrame
         :param group: 分组的列
         :param column: 需要秩的列
         :param on: 合并的列
         :param output_file: Output file path
@@ -234,23 +234,23 @@
         # 乘积
         column_prod = df.groupby(group)[column].prod().reset_index()
         group.append(f"{column}_prod")
         column_prod.columns = group
         # 保存文件
         all_merge_files: list = [column_size, column_mean, column_var, column_sem, column_std,
                                  column_median, column_min, column_max, column_sum, column_prod]
+
         if output_file is not None:
             if add_merge_files is not None:
                 all_merge_files.extend(add_merge_files)
-                self.merge_files(all_merge_files, on=on, output_file=output_file)
+                return self.merge_files(all_merge_files, on=on, output_file=output_file)
             else:
-                self.merge_files(all_merge_files, on=on, output_file=output_file)
-        return all_merge_files
+                return self.merge_files(all_merge_files, on=on, output_file=output_file)
 
-    def merge_files(self, files: list, on: str, output_file: str = None) -> None:
+    def merge_files(self, files: list, on: str, output_file: str = None) -> DataFrame:
         """
         将文件进行合并
         :param files: 多个文件
         :param on: 关键 key
         :param output_file: Output file path
         :return:
         """
@@ -262,14 +262,15 @@
         while i < size:
             self.log.debug(f"将文件进行合并第 {i} 次")
             new_file = pd.merge(new_file, files[i], on=on)
             i += 1
         # 保存文件
         if output_file is not None:
             self.to_file(new_file, output_file)
+        return new_file
 
 
 class Read:
     """
     Read file content
     """
```

### Comparing `ykenan_file-0.1.3/src/ykenan_file.egg-info/PKG-INFO` & `ykenan_file-0.1.4/src/ykenan_file.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-file
-Version: 0.1.3
+Version: 0.1.4
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

