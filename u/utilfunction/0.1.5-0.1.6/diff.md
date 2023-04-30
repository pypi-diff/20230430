# Comparing `tmp/utilfunction-0.1.5.tar.gz` & `tmp/utilfunction-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilfunction-0.1.5.tar", last modified: Sun Apr 30 10:02:38 2023, max compression
+gzip compressed data, was "utilfunction-0.1.6.tar", last modified: Sun Apr 30 10:11:04 2023, max compression
```

## Comparing `utilfunction-0.1.5.tar` & `utilfunction-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 10:02:38.132620 utilfunction-0.1.5/
--rw-rw-rw-   0        0        0    11357 2023-04-07 11:02:26.000000 utilfunction-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     4045 2023-04-30 10:02:38.132620 utilfunction-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3175 2023-04-30 09:53:12.000000 utilfunction-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-30 10:02:38.133626 utilfunction-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1614 2023-04-30 09:57:00.000000 utilfunction-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:02:38.114578 utilfunction-0.1.5/utilfunction/
--rw-rw-rw-   0        0        0      909 2023-04-30 10:02:28.000000 utilfunction-0.1.5/utilfunction/__init__.py
--rw-rw-rw-   0        0        0      758 2023-04-07 12:03:50.000000 utilfunction-0.1.5/utilfunction/astyper.py
--rw-rw-rw-   0        0        0      484 2023-04-13 09:24:19.000000 utilfunction-0.1.5/utilfunction/beep.py
--rw-rw-rw-   0        0        0     1646 2023-04-30 09:56:15.000000 utilfunction-0.1.5/utilfunction/bib2md.py
--rw-rw-rw-   0        0        0     1182 2023-04-07 11:44:57.000000 utilfunction-0.1.5/utilfunction/path_finder.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:02:38.130149 utilfunction-0.1.5/utilfunction.egg-info/
--rw-rw-rw-   0        0        0     4045 2023-04-30 10:02:38.000000 utilfunction-0.1.5/utilfunction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-04-30 10:02:38.000000 utilfunction-0.1.5/utilfunction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 10:02:38.000000 utilfunction-0.1.5/utilfunction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-30 10:02:38.000000 utilfunction-0.1.5/utilfunction.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-30 10:02:38.000000 utilfunction-0.1.5/utilfunction.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 10:11:04.265452 utilfunction-0.1.6/
+-rw-rw-rw-   0        0        0    11357 2023-04-07 11:02:26.000000 utilfunction-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     4045 2023-04-30 10:11:04.264454 utilfunction-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3175 2023-04-30 09:53:12.000000 utilfunction-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 10:11:04.265452 utilfunction-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1614 2023-04-30 10:10:29.000000 utilfunction-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:11:04.246156 utilfunction-0.1.6/utilfunction/
+-rw-rw-rw-   0        0        0      978 2023-04-30 10:10:35.000000 utilfunction-0.1.6/utilfunction/__init__.py
+-rw-rw-rw-   0        0        0      758 2023-04-07 12:03:50.000000 utilfunction-0.1.6/utilfunction/astyper.py
+-rw-rw-rw-   0        0        0      484 2023-04-13 09:24:19.000000 utilfunction-0.1.6/utilfunction/beep.py
+-rw-rw-rw-   0        0        0     1654 2023-04-30 10:09:51.000000 utilfunction-0.1.6/utilfunction/bib2md.py
+-rw-rw-rw-   0        0        0     1182 2023-04-07 11:44:57.000000 utilfunction-0.1.6/utilfunction/path_finder.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:11:04.262457 utilfunction-0.1.6/utilfunction.egg-info/
+-rw-rw-rw-   0        0        0     4045 2023-04-30 10:11:04.000000 utilfunction-0.1.6/utilfunction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-04-30 10:11:04.000000 utilfunction-0.1.6/utilfunction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 10:11:04.000000 utilfunction-0.1.6/utilfunction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-30 10:11:04.000000 utilfunction-0.1.6/utilfunction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-30 10:11:04.000000 utilfunction-0.1.6/utilfunction.egg-info/top_level.txt
```

### Comparing `utilfunction-0.1.5/LICENSE` & `utilfunction-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `utilfunction-0.1.5/PKG-INFO` & `utilfunction-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilfunction
-Version: 0.1.5
+Version: 0.1.6
 Summary: The Python package utilfunction wraps and distributes useful functions in an easy-to-use way.
 Home-page: https://github.com/DSDanielPark/utilfunction
 Author: parkminwoo
 Author-email: parkminwoo1991@gmail.com
 Keywords: Utils,Utility,Preprocessing,Analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `utilfunction-0.1.5/README.md` & `utilfunction-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `utilfunction-0.1.5/setup.py` & `utilfunction-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="utilfunction",
-    version="0.1.5",
+    version="0.1.6",
     author="parkminwoo",
     author_email="parkminwoo1991@gmail.com",
     description="The Python package utilfunction wraps and distributes useful functions in an easy-to-use way.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/DSDanielPark/utilfunction",
     packages=find_packages(),
```

### Comparing `utilfunction-0.1.5/utilfunction/__init__.py` & `utilfunction-0.1.6/utilfunction/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,13 +13,12 @@
 # See the License for the specific language governing permissions and
 # # limitations under the License.
 
 
 from utilfunction.path_finder import find_path
 from utilfunction.astyper import col_convert
 from utilfunction.beep import beep
+from utilfunction.bib2md import convert_bib2md, bib_to_markdown
 
-
-__all__ = ["find_path", "col_convert", "beep", "bib2md", "bib_to_markdown"]
-
-__version__ = "0.1.5"
+__all__ = ["find_path", "col_convert", "beep", "convert_bib2md", "bib_to_markdown"]
+__version__ = "0.1.6"
 __author__ = "MinWoo Park <parkminwoo1991@gmail.com>"
```

### Comparing `utilfunction-0.1.5/utilfunction/astyper.py` & `utilfunction-0.1.6/utilfunction/astyper.py`

 * *Files identical despite different names*

### Comparing `utilfunction-0.1.5/utilfunction/bib2md.py` & `utilfunction-0.1.6/utilfunction/bib2md.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     for k, v in bib_field_dict.items():
         if k ==title_key:
             md_body.append(f'\n## {k.upper()}: {v} \n')
         else:
             md_body.append(f'- **{k}:** {v} \n')
     return md_body
 
-def bib2md(bib_path: str, title_key: str, save_md_path: str) -> list:
+def convert_bib2md(bib_path: str, title_key: str, save_md_path: str) -> list:
     """Convert bib file to markdown format
 
     :param bib_path: Input BIB file path.
     :type bib_path: str
     :param title_key: The key value of the field that will be the main heading of the md file
     :type title_key: str
     :param save_md_path: Output MarkDown file path.
```

### Comparing `utilfunction-0.1.5/utilfunction/path_finder.py` & `utilfunction-0.1.6/utilfunction/path_finder.py`

 * *Files identical despite different names*

### Comparing `utilfunction-0.1.5/utilfunction.egg-info/PKG-INFO` & `utilfunction-0.1.6/utilfunction.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilfunction
-Version: 0.1.5
+Version: 0.1.6
 Summary: The Python package utilfunction wraps and distributes useful functions in an easy-to-use way.
 Home-page: https://github.com/DSDanielPark/utilfunction
 Author: parkminwoo
 Author-email: parkminwoo1991@gmail.com
 Keywords: Utils,Utility,Preprocessing,Analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

