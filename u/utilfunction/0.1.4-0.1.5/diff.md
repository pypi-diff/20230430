# Comparing `tmp/utilfunction-0.1.4.tar.gz` & `tmp/utilfunction-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilfunction-0.1.4.tar", last modified: Sun Apr 30 09:53:40 2023, max compression
+gzip compressed data, was "utilfunction-0.1.5.tar", last modified: Sun Apr 30 10:02:38 2023, max compression
```

## Comparing `utilfunction-0.1.4.tar` & `utilfunction-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 09:53:40.406100 utilfunction-0.1.4/
--rw-rw-rw-   0        0        0    11357 2023-04-07 11:02:26.000000 utilfunction-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     4045 2023-04-30 09:53:40.406100 utilfunction-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3175 2023-04-30 09:53:12.000000 utilfunction-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-30 09:53:40.407102 utilfunction-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1614 2023-04-30 09:51:54.000000 utilfunction-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 09:53:40.382321 utilfunction-0.1.4/utilfunction/
--rw-rw-rw-   0        0        0      909 2023-04-30 09:52:29.000000 utilfunction-0.1.4/utilfunction/__init__.py
--rw-rw-rw-   0        0        0      758 2023-04-07 12:03:50.000000 utilfunction-0.1.4/utilfunction/astyper.py
--rw-rw-rw-   0        0        0      484 2023-04-13 09:24:19.000000 utilfunction-0.1.4/utilfunction/beep.py
--rw-rw-rw-   0        0        0     1644 2023-04-30 09:47:33.000000 utilfunction-0.1.4/utilfunction/bib2md.py
--rw-rw-rw-   0        0        0     1182 2023-04-07 11:44:57.000000 utilfunction-0.1.4/utilfunction/path_finder.py
-drwxrwxrwx   0        0        0        0 2023-04-30 09:53:40.403072 utilfunction-0.1.4/utilfunction.egg-info/
--rw-rw-rw-   0        0        0     4045 2023-04-30 09:53:40.000000 utilfunction-0.1.4/utilfunction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-04-30 09:53:40.000000 utilfunction-0.1.4/utilfunction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 09:53:40.000000 utilfunction-0.1.4/utilfunction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-30 09:53:40.000000 utilfunction-0.1.4/utilfunction.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-30 09:53:40.000000 utilfunction-0.1.4/utilfunction.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 10:02:38.132620 utilfunction-0.1.5/
+-rw-rw-rw-   0        0        0    11357 2023-04-07 11:02:26.000000 utilfunction-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     4045 2023-04-30 10:02:38.132620 utilfunction-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3175 2023-04-30 09:53:12.000000 utilfunction-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 10:02:38.133626 utilfunction-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1614 2023-04-30 09:57:00.000000 utilfunction-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:02:38.114578 utilfunction-0.1.5/utilfunction/
+-rw-rw-rw-   0        0        0      909 2023-04-30 10:02:28.000000 utilfunction-0.1.5/utilfunction/__init__.py
+-rw-rw-rw-   0        0        0      758 2023-04-07 12:03:50.000000 utilfunction-0.1.5/utilfunction/astyper.py
+-rw-rw-rw-   0        0        0      484 2023-04-13 09:24:19.000000 utilfunction-0.1.5/utilfunction/beep.py
+-rw-rw-rw-   0        0        0     1646 2023-04-30 09:56:15.000000 utilfunction-0.1.5/utilfunction/bib2md.py
+-rw-rw-rw-   0        0        0     1182 2023-04-07 11:44:57.000000 utilfunction-0.1.5/utilfunction/path_finder.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:02:38.130149 utilfunction-0.1.5/utilfunction.egg-info/
+-rw-rw-rw-   0        0        0     4045 2023-04-30 10:02:38.000000 utilfunction-0.1.5/utilfunction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-04-30 10:02:38.000000 utilfunction-0.1.5/utilfunction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 10:02:38.000000 utilfunction-0.1.5/utilfunction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-30 10:02:38.000000 utilfunction-0.1.5/utilfunction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-30 10:02:38.000000 utilfunction-0.1.5/utilfunction.egg-info/top_level.txt
```

### Comparing `utilfunction-0.1.4/LICENSE` & `utilfunction-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `utilfunction-0.1.4/PKG-INFO` & `utilfunction-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilfunction
-Version: 0.1.4
+Version: 0.1.5
 Summary: The Python package utilfunction wraps and distributes useful functions in an easy-to-use way.
 Home-page: https://github.com/DSDanielPark/utilfunction
 Author: parkminwoo
 Author-email: parkminwoo1991@gmail.com
 Keywords: Utils,Utility,Preprocessing,Analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `utilfunction-0.1.4/README.md` & `utilfunction-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `utilfunction-0.1.4/setup.py` & `utilfunction-0.1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="utilfunction",
-    version="0.1.4",
+    version="0.1.5",
     author="parkminwoo",
     author_email="parkminwoo1991@gmail.com",
     description="The Python package utilfunction wraps and distributes useful functions in an easy-to-use way.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/DSDanielPark/utilfunction",
     packages=find_packages(),
```

### Comparing `utilfunction-0.1.4/utilfunction/__init__.py` & `utilfunction-0.1.5/utilfunction/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,9 +17,9 @@
 from utilfunction.path_finder import find_path
 from utilfunction.astyper import col_convert
 from utilfunction.beep import beep
 
 
 __all__ = ["find_path", "col_convert", "beep", "bib2md", "bib_to_markdown"]
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 __author__ = "MinWoo Park <parkminwoo1991@gmail.com>"
```

### Comparing `utilfunction-0.1.4/utilfunction/astyper.py` & `utilfunction-0.1.5/utilfunction/astyper.py`

 * *Files identical despite different names*

### Comparing `utilfunction-0.1.4/utilfunction/bib2md.py` & `utilfunction-0.1.5/utilfunction/bib2md.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     :type title_key: str
     :return: List of strings converted to MarkDown format
     :rtype: list
     """
     md_body = []
     for k, v in bib_field_dict.items():
         if k ==title_key:
-            md_body.append(f'## {k.upper()}: {v} \n')
+            md_body.append(f'\n## {k.upper()}: {v} \n')
         else:
             md_body.append(f'- **{k}:** {v} \n')
     return md_body
 
 def bib2md(bib_path: str, title_key: str, save_md_path: str) -> list:
     """Convert bib file to markdown format
```

### Comparing `utilfunction-0.1.4/utilfunction/path_finder.py` & `utilfunction-0.1.5/utilfunction/path_finder.py`

 * *Files identical despite different names*

### Comparing `utilfunction-0.1.4/utilfunction.egg-info/PKG-INFO` & `utilfunction-0.1.5/utilfunction.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilfunction
-Version: 0.1.4
+Version: 0.1.5
 Summary: The Python package utilfunction wraps and distributes useful functions in an easy-to-use way.
 Home-page: https://github.com/DSDanielPark/utilfunction
 Author: parkminwoo
 Author-email: parkminwoo1991@gmail.com
 Keywords: Utils,Utility,Preprocessing,Analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

