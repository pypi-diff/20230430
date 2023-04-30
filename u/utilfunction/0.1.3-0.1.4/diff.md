# Comparing `tmp/utilfunction-0.1.3.tar.gz` & `tmp/utilfunction-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilfunction-0.1.3.tar", last modified: Thu Apr 13 09:26:30 2023, max compression
+gzip compressed data, was "utilfunction-0.1.4.tar", last modified: Sun Apr 30 09:53:40 2023, max compression
```

## Comparing `utilfunction-0.1.3.tar` & `utilfunction-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 09:26:30.438453 utilfunction-0.1.3/
--rw-rw-rw-   0        0        0    11357 2023-04-07 11:02:26.000000 utilfunction-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     3506 2023-04-13 09:26:30.437445 utilfunction-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2636 2023-04-13 09:26:05.000000 utilfunction-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 09:26:30.438453 utilfunction-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1614 2023-04-13 09:24:23.000000 utilfunction-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:26:30.414820 utilfunction-0.1.3/utilfunction/
--rw-rw-rw-   0        0        0      880 2023-04-13 09:23:10.000000 utilfunction-0.1.3/utilfunction/__init__.py
--rw-rw-rw-   0        0        0      758 2023-04-07 12:03:50.000000 utilfunction-0.1.3/utilfunction/astyper.py
--rw-rw-rw-   0        0        0      484 2023-04-13 09:24:19.000000 utilfunction-0.1.3/utilfunction/beep.py
--rw-rw-rw-   0        0        0     1182 2023-04-07 11:44:57.000000 utilfunction-0.1.3/utilfunction/path_finder.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:26:30.434234 utilfunction-0.1.3/utilfunction.egg-info/
--rw-rw-rw-   0        0        0     3506 2023-04-13 09:26:30.000000 utilfunction-0.1.3/utilfunction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-13 09:26:30.000000 utilfunction-0.1.3/utilfunction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 09:26:30.000000 utilfunction-0.1.3/utilfunction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 09:26:30.000000 utilfunction-0.1.3/utilfunction.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 09:26:30.000000 utilfunction-0.1.3/utilfunction.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 09:53:40.406100 utilfunction-0.1.4/
+-rw-rw-rw-   0        0        0    11357 2023-04-07 11:02:26.000000 utilfunction-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     4045 2023-04-30 09:53:40.406100 utilfunction-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3175 2023-04-30 09:53:12.000000 utilfunction-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 09:53:40.407102 utilfunction-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1614 2023-04-30 09:51:54.000000 utilfunction-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 09:53:40.382321 utilfunction-0.1.4/utilfunction/
+-rw-rw-rw-   0        0        0      909 2023-04-30 09:52:29.000000 utilfunction-0.1.4/utilfunction/__init__.py
+-rw-rw-rw-   0        0        0      758 2023-04-07 12:03:50.000000 utilfunction-0.1.4/utilfunction/astyper.py
+-rw-rw-rw-   0        0        0      484 2023-04-13 09:24:19.000000 utilfunction-0.1.4/utilfunction/beep.py
+-rw-rw-rw-   0        0        0     1644 2023-04-30 09:47:33.000000 utilfunction-0.1.4/utilfunction/bib2md.py
+-rw-rw-rw-   0        0        0     1182 2023-04-07 11:44:57.000000 utilfunction-0.1.4/utilfunction/path_finder.py
+drwxrwxrwx   0        0        0        0 2023-04-30 09:53:40.403072 utilfunction-0.1.4/utilfunction.egg-info/
+-rw-rw-rw-   0        0        0     4045 2023-04-30 09:53:40.000000 utilfunction-0.1.4/utilfunction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-04-30 09:53:40.000000 utilfunction-0.1.4/utilfunction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 09:53:40.000000 utilfunction-0.1.4/utilfunction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-30 09:53:40.000000 utilfunction-0.1.4/utilfunction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-30 09:53:40.000000 utilfunction-0.1.4/utilfunction.egg-info/top_level.txt
```

### Comparing `utilfunction-0.1.3/LICENSE` & `utilfunction-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `utilfunction-0.1.3/PKG-INFO` & `utilfunction-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilfunction
-Version: 0.1.3
+Version: 0.1.4
 Summary: The Python package utilfunction wraps and distributes useful functions in an easy-to-use way.
 Home-page: https://github.com/DSDanielPark/utilfunction
 Author: parkminwoo
 Author-email: parkminwoo1991@gmail.com
 Keywords: Utils,Utility,Preprocessing,Analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,18 +15,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Development Status :: 3 - Alpha
+Development Status :: 3 - Alpha <br>
+*Copyright (c) 2023 MinWoo Park*
+<br>
 
 # util-function
-![Util-Func](https://img.shields.io/badge/pypi-utilfunction-blue)
+![Util-Func](https://img.shields.io/badge/pypi-utilfunction-orange)
 ![Pypi Version](https://img.shields.io/pypi/v/utilfunction.svg)
 [![Contributor Covenant](https://img.shields.io/badge/contributor%20covenant-v2.0%20adopted-black.svg)](code_of_conduct.md)
 [![Python Version](https://img.shields.io/badge/python-3.6%2C3.7%2C3.8-black.svg)](code_of_conduct.md)
 ![Code convention](https://img.shields.io/badge/code%20convention-pep8-black)
 
 The Python package utilfunction wraps and distributes useful functions in an easy-to-use way. We have collected functions that are simpler in function than many distributed Python packages or whose category is ambiguous.
 
@@ -43,25 +45,25 @@
 `path_finder.py` - function: find_path <br>
  Find the path of a file or folder. 
 ```python
 from utilfunction import find_path
 
 nii_file_list = find_path('./home', 'file', 'mask.nii.gz')
 ```
-
+<br>
 
 `astyper.py` - function: col_converter <br>
 Restores a column whose array is stored as a string type back to an array type.
 ```python
 from utilfunction import col_convert
 
 df_has_converted_col = col_convert(df, "embedding_arrays")
 ```
 
-
+<br>
 
 `beep.py` - function: beep <br>
 Make beep
 ```python
 from utilfunction import beep
 
 beep()
@@ -69,24 +71,46 @@
 sec=10
 feq=800
 beep(sec, feq)
 ```
 
 <br>
 
+
+`bib2md.py` - function: bib2md <br>
+Convert `bib file` to `markdown file`  
+```python
+from utilfunction import bib2md
+
+bib_path = './sample_data/attention_based.bib'
+save_path = './sample_data/attention_based.md'
+title_key = 'title'
+
+bib2md(bib_path, title_key, save_path)
+
+```
+
+
 # How to Contribute
 Please create a pull request for any function that is useful and simple to reuse. Create a function, and write a tutorial with the same name as the function in the doc folder. Any snippet that you are comfortable with and use often will do. However, some contents may be revised and adjusted later for convenience.
 
 1. Create a Python file containing functions in [`utilfunction folder`](https://github.com/DSDanielPark/utilfunction/tree/main/utifunc). You must include formatting and doc strings in your function.
 2. Write brief explanations and examples in the [`doc folder`](https://github.com/DSDanielPark/utilfunction/tree/main/doc)
 3. Write a one-line code example in README.md
 5. Make a Pull Request
 <br>
 
 Please refer to the `find_path` function in [`path_finder.py`](https://github.com/DSDanielPark/utilfunction/blob/main/utifunc/path_finder.py).
 
 <br>
 
+- Styled with black `black .`
+- Lnted with pylint `pylint --rcfile=setup.cfg util-function/`
+- Type-checked with mypy `mypy util-function/`
+- Pass the pytest unit tests `pytest`
+
+
+
 # Notice
 - This repo goes through a simple QA process, there are no major refactoring plans, and it's not a planned project, so it's in alpha.
 - If there is a reference, please list it at the top of each Python file.
 - Coverage of Python versions is subject to change. However, the code formatting is changed to black during the QA process.
```

### Comparing `utilfunction-0.1.3/README.md` & `utilfunction-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-Development Status :: 3 - Alpha
+Development Status :: 3 - Alpha <br>
+*Copyright (c) 2023 MinWoo Park*
+<br>
 
 # util-function
-![Util-Func](https://img.shields.io/badge/pypi-utilfunction-blue)
+![Util-Func](https://img.shields.io/badge/pypi-utilfunction-orange)
 ![Pypi Version](https://img.shields.io/pypi/v/utilfunction.svg)
 [![Contributor Covenant](https://img.shields.io/badge/contributor%20covenant-v2.0%20adopted-black.svg)](code_of_conduct.md)
 [![Python Version](https://img.shields.io/badge/python-3.6%2C3.7%2C3.8-black.svg)](code_of_conduct.md)
 ![Code convention](https://img.shields.io/badge/code%20convention-pep8-black)
 
 The Python package utilfunction wraps and distributes useful functions in an easy-to-use way. We have collected functions that are simpler in function than many distributed Python packages or whose category is ambiguous.
 
@@ -22,25 +24,25 @@
 `path_finder.py` - function: find_path <br>
  Find the path of a file or folder. 
 ```python
 from utilfunction import find_path
 
 nii_file_list = find_path('./home', 'file', 'mask.nii.gz')
 ```
-
+<br>
 
 `astyper.py` - function: col_converter <br>
 Restores a column whose array is stored as a string type back to an array type.
 ```python
 from utilfunction import col_convert
 
 df_has_converted_col = col_convert(df, "embedding_arrays")
 ```
 
-
+<br>
 
 `beep.py` - function: beep <br>
 Make beep
 ```python
 from utilfunction import beep
 
 beep()
@@ -48,24 +50,46 @@
 sec=10
 feq=800
 beep(sec, feq)
 ```
 
 <br>
 
+
+`bib2md.py` - function: bib2md <br>
+Convert `bib file` to `markdown file`  
+```python
+from utilfunction import bib2md
+
+bib_path = './sample_data/attention_based.bib'
+save_path = './sample_data/attention_based.md'
+title_key = 'title'
+
+bib2md(bib_path, title_key, save_path)
+
+```
+
+
 # How to Contribute
 Please create a pull request for any function that is useful and simple to reuse. Create a function, and write a tutorial with the same name as the function in the doc folder. Any snippet that you are comfortable with and use often will do. However, some contents may be revised and adjusted later for convenience.
 
 1. Create a Python file containing functions in [`utilfunction folder`](https://github.com/DSDanielPark/utilfunction/tree/main/utifunc). You must include formatting and doc strings in your function.
 2. Write brief explanations and examples in the [`doc folder`](https://github.com/DSDanielPark/utilfunction/tree/main/doc)
 3. Write a one-line code example in README.md
 5. Make a Pull Request
 <br>
 
 Please refer to the `find_path` function in [`path_finder.py`](https://github.com/DSDanielPark/utilfunction/blob/main/utifunc/path_finder.py).
 
 <br>
 
+- Styled with black `black .`
+- Lnted with pylint `pylint --rcfile=setup.cfg util-function/`
+- Type-checked with mypy `mypy util-function/`
+- Pass the pytest unit tests `pytest`
+
+
+
 # Notice
 - This repo goes through a simple QA process, there are no major refactoring plans, and it's not a planned project, so it's in alpha.
 - If there is a reference, please list it at the top of each Python file.
 - Coverage of Python versions is subject to change. However, the code formatting is changed to black during the QA process.
```

### Comparing `utilfunction-0.1.3/setup.py` & `utilfunction-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="utilfunction",
-    version="0.1.3",
+    version="0.1.4",
     author="parkminwoo",
     author_email="parkminwoo1991@gmail.com",
     description="The Python package utilfunction wraps and distributes useful functions in an easy-to-use way.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/DSDanielPark/utilfunction",
     packages=find_packages(),
```

### Comparing `utilfunction-0.1.3/utilfunction/__init__.py` & `utilfunction-0.1.4/utilfunction/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,11 +15,11 @@
 
 
 from utilfunction.path_finder import find_path
 from utilfunction.astyper import col_convert
 from utilfunction.beep import beep
 
 
-__all__ = ["find_path", "col_convert", "beep"]
+__all__ = ["find_path", "col_convert", "beep", "bib2md", "bib_to_markdown"]
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "MinWoo Park <parkminwoo1991@gmail.com>"
```

### Comparing `utilfunction-0.1.3/utilfunction/astyper.py` & `utilfunction-0.1.4/utilfunction/astyper.py`

 * *Files identical despite different names*

### Comparing `utilfunction-0.1.3/utilfunction/path_finder.py` & `utilfunction-0.1.4/utilfunction/path_finder.py`

 * *Files identical despite different names*

### Comparing `utilfunction-0.1.3/utilfunction.egg-info/PKG-INFO` & `utilfunction-0.1.4/utilfunction.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilfunction
-Version: 0.1.3
+Version: 0.1.4
 Summary: The Python package utilfunction wraps and distributes useful functions in an easy-to-use way.
 Home-page: https://github.com/DSDanielPark/utilfunction
 Author: parkminwoo
 Author-email: parkminwoo1991@gmail.com
 Keywords: Utils,Utility,Preprocessing,Analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,18 +15,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Development Status :: 3 - Alpha
+Development Status :: 3 - Alpha <br>
+*Copyright (c) 2023 MinWoo Park*
+<br>
 
 # util-function
-![Util-Func](https://img.shields.io/badge/pypi-utilfunction-blue)
+![Util-Func](https://img.shields.io/badge/pypi-utilfunction-orange)
 ![Pypi Version](https://img.shields.io/pypi/v/utilfunction.svg)
 [![Contributor Covenant](https://img.shields.io/badge/contributor%20covenant-v2.0%20adopted-black.svg)](code_of_conduct.md)
 [![Python Version](https://img.shields.io/badge/python-3.6%2C3.7%2C3.8-black.svg)](code_of_conduct.md)
 ![Code convention](https://img.shields.io/badge/code%20convention-pep8-black)
 
 The Python package utilfunction wraps and distributes useful functions in an easy-to-use way. We have collected functions that are simpler in function than many distributed Python packages or whose category is ambiguous.
 
@@ -43,25 +45,25 @@
 `path_finder.py` - function: find_path <br>
  Find the path of a file or folder. 
 ```python
 from utilfunction import find_path
 
 nii_file_list = find_path('./home', 'file', 'mask.nii.gz')
 ```
-
+<br>
 
 `astyper.py` - function: col_converter <br>
 Restores a column whose array is stored as a string type back to an array type.
 ```python
 from utilfunction import col_convert
 
 df_has_converted_col = col_convert(df, "embedding_arrays")
 ```
 
-
+<br>
 
 `beep.py` - function: beep <br>
 Make beep
 ```python
 from utilfunction import beep
 
 beep()
@@ -69,24 +71,46 @@
 sec=10
 feq=800
 beep(sec, feq)
 ```
 
 <br>
 
+
+`bib2md.py` - function: bib2md <br>
+Convert `bib file` to `markdown file`  
+```python
+from utilfunction import bib2md
+
+bib_path = './sample_data/attention_based.bib'
+save_path = './sample_data/attention_based.md'
+title_key = 'title'
+
+bib2md(bib_path, title_key, save_path)
+
+```
+
+
 # How to Contribute
 Please create a pull request for any function that is useful and simple to reuse. Create a function, and write a tutorial with the same name as the function in the doc folder. Any snippet that you are comfortable with and use often will do. However, some contents may be revised and adjusted later for convenience.
 
 1. Create a Python file containing functions in [`utilfunction folder`](https://github.com/DSDanielPark/utilfunction/tree/main/utifunc). You must include formatting and doc strings in your function.
 2. Write brief explanations and examples in the [`doc folder`](https://github.com/DSDanielPark/utilfunction/tree/main/doc)
 3. Write a one-line code example in README.md
 5. Make a Pull Request
 <br>
 
 Please refer to the `find_path` function in [`path_finder.py`](https://github.com/DSDanielPark/utilfunction/blob/main/utifunc/path_finder.py).
 
 <br>
 
+- Styled with black `black .`
+- Lnted with pylint `pylint --rcfile=setup.cfg util-function/`
+- Type-checked with mypy `mypy util-function/`
+- Pass the pytest unit tests `pytest`
+
+
+
 # Notice
 - This repo goes through a simple QA process, there are no major refactoring plans, and it's not a planned project, so it's in alpha.
 - If there is a reference, please list it at the top of each Python file.
 - Coverage of Python versions is subject to change. However, the code formatting is changed to black during the QA process.
```

