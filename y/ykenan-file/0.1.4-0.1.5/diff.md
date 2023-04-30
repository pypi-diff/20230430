# Comparing `tmp/ykenan_file-0.1.4.tar.gz` & `tmp/ykenan_file-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_file-0.1.4.tar", last modified: Sun Apr 30 11:06:46 2023, max compression
+gzip compressed data, was "ykenan_file-0.1.5.tar", last modified: Sun Apr 30 11:40:48 2023, max compression
```

## Comparing `ykenan_file-0.1.4.tar` & `ykenan_file-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 11:06:46.346327 ykenan_file-0.1.4/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      829 2023-04-30 11:06:46.346327 ykenan_file-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-04-21 09:34:27.000000 ykenan_file-0.1.4/README.md
--rw-rw-rw-   0        0        0      676 2023-04-30 11:04:10.000000 ykenan_file-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       32 2023-03-22 07:40:08.000000 ykenan_file-0.1.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 11:06:46.346327 ykenan_file-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-30 11:06:46.323328 ykenan_file-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 11:06:46.334326 ykenan_file-0.1.4/src/ykenan_file/
--rw-rw-rw-   0        0        0    23424 2023-04-30 11:03:28.000000 ykenan_file-0.1.4/src/ykenan_file/__init__.py
--rw-rw-rw-   0        0        0      157 2023-04-06 01:49:10.000000 ykenan_file-0.1.4/src/ykenan_file/util.py
-drwxrwxrwx   0        0        0        0 2023-04-30 11:06:46.344326 ykenan_file-0.1.4/src/ykenan_file.egg-info/
--rw-rw-rw-   0        0        0      829 2023-04-30 11:06:46.000000 ykenan_file-0.1.4/src/ykenan_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-30 11:06:46.000000 ykenan_file-0.1.4/src/ykenan_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 11:06:46.000000 ykenan_file-0.1.4/src/ykenan_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-30 11:06:46.000000 ykenan_file-0.1.4/src/ykenan_file.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-30 11:06:46.000000 ykenan_file-0.1.4/src/ykenan_file.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 11:40:48.572468 ykenan_file-0.1.5/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      829 2023-04-30 11:40:48.571468 ykenan_file-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-04-21 09:34:27.000000 ykenan_file-0.1.5/README.md
+-rw-rw-rw-   0        0        0      676 2023-04-30 11:39:51.000000 ykenan_file-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       32 2023-03-22 07:40:08.000000 ykenan_file-0.1.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 11:40:48.572468 ykenan_file-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 11:40:48.548468 ykenan_file-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 11:40:48.560469 ykenan_file-0.1.5/src/ykenan_file/
+-rw-rw-rw-   0        0        0    23829 2023-04-30 11:39:51.000000 ykenan_file-0.1.5/src/ykenan_file/__init__.py
+-rw-rw-rw-   0        0        0      157 2023-04-06 01:49:10.000000 ykenan_file-0.1.5/src/ykenan_file/util.py
+drwxrwxrwx   0        0        0        0 2023-04-30 11:40:48.569468 ykenan_file-0.1.5/src/ykenan_file.egg-info/
+-rw-rw-rw-   0        0        0      829 2023-04-30 11:40:48.000000 ykenan_file-0.1.5/src/ykenan_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-30 11:40:48.000000 ykenan_file-0.1.5/src/ykenan_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 11:40:48.000000 ykenan_file-0.1.5/src/ykenan_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-30 11:40:48.000000 ykenan_file-0.1.5/src/ykenan_file.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-30 11:40:48.000000 ykenan_file-0.1.5/src/ykenan_file.egg-info/top_level.txt
```

### Comparing `ykenan_file-0.1.4/LICENSE` & `ykenan_file-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_file-0.1.4/PKG-INFO` & `ykenan_file-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_file
-Version: 0.1.4
+Version: 0.1.5
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_file-0.1.4/pyproject.toml` & `ykenan_file-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_file"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "file", "read", "write"]
 description = "File read and write operations"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `ykenan_file-0.1.4/src/ykenan_file/__init__.py` & `ykenan_file-0.1.5/src/ykenan_file/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -195,50 +195,59 @@
         :param add_merge_files: 添加 merge 文件
         :return:
         """
         # 总和
         self.log.debug(f"通过分组进行一系列数值计算: {group}, {column}")
         # 个数大小
         column_size = df.groupby(group)[column].size().reset_index()
-        group.append(f"{column}_size")
-        column_size.columns = group
+        new_column = group.copy()
+        new_column.append(f"{column}_size")
+        column_size.columns = new_column
         # 平均值
         column_mean = df.groupby(group)[column].mean().reset_index()
-        group.append(f"{column}_mean")
-        column_mean.columns = group
+        new_column = group.copy()
+        new_column.append(f"{column}_mean")
+        column_mean.columns = new_column
         # 方差 (size == 1 的值为 NaN)
         column_var = df.groupby(group)[column].var().reset_index()
-        group.append(f"{column}_var")
-        column_var.columns = group
+        new_column = group.copy()
+        new_column.append(f"{column}_var")
+        column_var.columns = new_column
         # 标准误差 (size == 1 的值为 NaN)
         column_sem = df.groupby(group)[column].sem().reset_index()
-        group.append(f"{column}_sem")
-        column_sem.columns = group
+        new_column = group.copy()
+        new_column.append(f"{column}_sem")
+        column_sem.columns = new_column
         # 标准偏差 (size == 1 的值为 NaN)
         column_std = df.groupby(group)[column].std().reset_index()
-        group.append(f"{column}_std")
-        column_std.columns = group
+        new_column = group.copy()
+        new_column.append(f"{column}_std")
+        column_std.columns = new_column
         # 中位数值
         column_median = df.groupby(group)[column].median().reset_index()
-        group.append(f"{column}_median")
-        column_median.columns = group
+        new_column = group.copy()
+        new_column.append(f"{column}_median")
+        column_median.columns = new_column
         # 最小值
         column_min = df.groupby(group)[column].min().reset_index()
-        group.append(f"{column}_min")
-        column_min.columns = group
+        new_column = group.copy()
+        new_column.append(f"{column}_min")
+        column_min.columns = new_column
         # 最大值
         column_max = df.groupby(group)[column].max().reset_index()
-        group.append(f"{column}_max")
-        column_max.columns = group
+        new_column = group.copy()
+        new_column.append(f"{column}_max")
+        column_max.columns = new_column
         # 总和
         column_sum = self.sum_group_by(df, group, column)
         # 乘积
         column_prod = df.groupby(group)[column].prod().reset_index()
-        group.append(f"{column}_prod")
-        column_prod.columns = group
+        new_column = group.copy()
+        new_column.append(f"{column}_prod")
+        column_prod.columns = new_column
         # 保存文件
         all_merge_files: list = [column_size, column_mean, column_var, column_sem, column_std,
                                  column_median, column_min, column_max, column_sum, column_prod]
 
         if output_file is not None:
             if add_merge_files is not None:
                 all_merge_files.extend(add_merge_files)
```

### Comparing `ykenan_file-0.1.4/src/ykenan_file.egg-info/PKG-INFO` & `ykenan_file-0.1.5/src/ykenan_file.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-file
-Version: 0.1.4
+Version: 0.1.5
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

