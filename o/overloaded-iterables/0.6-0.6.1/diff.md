# Comparing `tmp/overloaded-iterables-0.6.tar.gz` & `tmp/overloaded-iterables-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overloaded-iterables-0.6.tar", last modified: Sun Apr 30 21:06:36 2023, max compression
+gzip compressed data, was "overloaded-iterables-0.6.1.tar", last modified: Sun Apr 30 21:21:14 2023, max compression
```

## Comparing `overloaded-iterables-0.6.tar` & `overloaded-iterables-0.6.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 21:06:36.108930 overloaded-iterables-0.6/
--rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.6/LICENSE
--rw-rw-rw-   0        0        0     7861 2023-04-30 21:06:36.109930 overloaded-iterables-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     7150 2023-04-30 20:48:12.000000 overloaded-iterables-0.6/README.md
--rw-rw-rw-   0        0        0      111 2023-04-30 21:06:36.110935 overloaded-iterables-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1475 2023-04-30 21:06:19.000000 overloaded-iterables-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:06:36.095933 overloaded-iterables-0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 21:06:36.100930 overloaded-iterables-0.6/src/overloaded_iterables/
--rw-rw-rw-   0        0        0        0 2023-04-29 23:52:39.000000 overloaded-iterables-0.6/src/overloaded_iterables/__init__.py
--rw-rw-rw-   0        0        0    13051 2023-04-30 20:19:49.000000 overloaded-iterables-0.6/src/overloaded_iterables/classes.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:06:36.108930 overloaded-iterables-0.6/src/overloaded_iterables.egg-info/
--rw-rw-rw-   0        0        0     7861 2023-04-30 21:06:36.000000 overloaded-iterables-0.6/src/overloaded_iterables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-04-30 21:06:36.000000 overloaded-iterables-0.6/src/overloaded_iterables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 21:06:36.000000 overloaded-iterables-0.6/src/overloaded_iterables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-30 21:06:36.000000 overloaded-iterables-0.6/src/overloaded_iterables.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-30 21:06:36.000000 overloaded-iterables-0.6/src/overloaded_iterables.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 21:21:14.487615 overloaded-iterables-0.6.1/
+-rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0     7994 2023-04-30 21:21:14.487615 overloaded-iterables-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7281 2023-04-30 21:17:53.000000 overloaded-iterables-0.6.1/README.md
+-rw-rw-rw-   0        0        0      111 2023-04-30 21:21:14.489616 overloaded-iterables-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1477 2023-04-30 21:20:52.000000 overloaded-iterables-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:21:14.472617 overloaded-iterables-0.6.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 21:21:14.477615 overloaded-iterables-0.6.1/src/overloaded_iterables/
+-rw-rw-rw-   0        0        0        0 2023-04-29 23:52:39.000000 overloaded-iterables-0.6.1/src/overloaded_iterables/__init__.py
+-rw-rw-rw-   0        0        0    13051 2023-04-30 20:19:49.000000 overloaded-iterables-0.6.1/src/overloaded_iterables/classes.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:21:14.486618 overloaded-iterables-0.6.1/src/overloaded_iterables.egg-info/
+-rw-rw-rw-   0        0        0     7994 2023-04-30 21:21:14.000000 overloaded-iterables-0.6.1/src/overloaded_iterables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-04-30 21:21:14.000000 overloaded-iterables-0.6.1/src/overloaded_iterables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 21:21:14.000000 overloaded-iterables-0.6.1/src/overloaded_iterables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-30 21:21:14.000000 overloaded-iterables-0.6.1/src/overloaded_iterables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-30 21:21:14.000000 overloaded-iterables-0.6.1/src/overloaded_iterables.egg-info/top_level.txt
```

### Comparing `overloaded-iterables-0.6/LICENSE` & `overloaded-iterables-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.6/PKG-INFO` & `overloaded-iterables-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: overloaded-iterables
-Version: 0.6
+Version: 0.6.1
 Summary: Overloaded version of the built-in python classes: list and set to include some extra functionalities.
 Home-page: https://github.com/Arkiralor/overloaded_iterables
 Author: Prithoo Medhi
 Author-email: prithoo11335@gmail.com
 License: MIT
 Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot
 Platform: windows
 Platform: ubuntu-linux
 Platform: mac-os
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Overloaded Iterables
 
-Overloaded version of the built-in python classes: `<list>` and `<set>` to include some extra functionalities as an experiment.
-
-The current iteration contains the following classes
+Overloaded versions of the built-in python classes: `<list>` and `<set>` to include some extra functionalities as an experiment.
 
 ## Specifications
 
 1. __Python Version:__ Python v3.8+
 2. __Code Coverage:__ ![_code coverage_](https://github.com/Arkiralor/overloaded_iterables/blob/master/media/screenshots/coverage.PNG?raw=true)
 3. __Tests Status:__ ![_test status_](https://github.com/Arkiralor/overloaded_iterables/blob/master/media/screenshots/test_results.PNG?raw=true)
 
@@ -37,14 +35,16 @@
 
 ```sh
 python -m pip install overloaded-iterables
 ```
 
 ## Classes
 
+The current iteration contains the following classes
+
 ### 1. OverloadedList
 
 - A non-datatype constrained, single-dimensional collection of values.
 - Inherits solely from Python's built-in `<list>` class.
 
 ```python
 from overloaded_iterables.classes import OverloadedList
@@ -137,50 +137,50 @@
     - Example:
 
         ```python
             _median:float = obj.median()
         ```
 
 8. `<class>.hist()`&nbsp;&nbsp;&nbsp;&nbsp;__(OverloadedList only)__
-    - Plots the histogram of the frequency distribution of the elements in the OverloadedList.
+    - Plots the [histogram](https://en.wikipedia.org/wiki/Histogram) of the frequency distribution of the elements in the OverloadedList.
     - Arguments: `self`, `bins: int | default: 10`, `title: str | default: 'Histogram'`, `x_label: str | default: 'Values --->'`, `y_label: str | default: 'Frequencies --->'`, `save_dir: str | default: None`, `file_name: str | default: None`, `histtype: str | default: 'step'`, `align: str | default: 'mid'`, `orientation: str | default: 'vertical'`, `log_scale: bool | default: False`, `show: bool | default: False`
     - Process:
         - Shows the generated figure if `show` is set to `True`
         - Saves the generated figure if `save_dir` is provided.
     - Returns: `bool`
     - Example:
 
         ```python
-            fig_check:float = obj.hist(show=True, save_dir='figures', file_name='some-figure')
+            fig_check:bool = obj.hist(show=True, save_dir='figures', file_name='some-figure')
         ```
 
 9. `<class>.plot()`&nbsp;&nbsp;&nbsp;&nbsp;__(OverloadedList only)__
-    - Plots the lineplot of the frequency distribution of the elements in the OverloadedList.
+    - Plots the [lineplot](https://en.wikipedia.org/wiki/Line_chart) of the frequency distribution of the elements in the OverloadedList.
     - Arguments: `self`, `title: str | default: 'Line Plot'`, `x_label: str | default: 'Values --->'`, `y_label: str | default: 'Frequencies --->'`, `save_dir: str | default: None`, `file_name: str | default: None`, `color: str | default: '#000000'`, `linewidth: float | default: 1`, `marker: str | default: ','`,  `markerfacecolor: str | default: '#252525'`, `marker_size: float | default: 1.0`, `show: bool | default: False`
     - Process:
         - Shows the generated figure if `show` is set to `True`
         - Saves the generated figure if `save_dir` is provided.
     - Returns: `bool`
     - Example:
 
         ```python
-            fig_check:float = obj.plot(show=True, save_dir='figures', file_name='some-figure')
+            fig_check:bool = obj.plot(show=True, save_dir='figures', file_name='some-figure')
         ```
 
 10. `<class>.scatter()`&nbsp;&nbsp;&nbsp;&nbsp;__(OverloadedList only)__
-    - Plots the scatterplot of the frequency distribution of the elements in the OverloadedList.
+    - Plots the [scatterplot](https://en.wikipedia.org/wiki/Scatter_plot) of the frequency distribution of the elements in the OverloadedList.
     - Arguments: `self`, `title: str | default: 'Scatter Plot'`, `x_label: str | default: 'Values --->'`, `y_label: str | default: 'Frequencies --->'`, `save_dir: str | default: None`, `file_name: str | default: None`, `size: List[float] | default: [1.25]`, `color: str | default: '#000000'`, `marker: str | default: ','`, `line_width: float | default: 2`, `show: bool | default: False`
     - Process:
         - Shows the generated figure if `show` is set to `True`
         - Saves the generated figure if `save_dir` is provided.
     - Returns: `bool`
     - Example:
 
         ```python
-            fig_check:float = obj.scatter(show=True, save_dir='figures', file_name='some-figure')
+            fig_check:bool = obj.scatter(show=True, save_dir='figures', file_name='some-figure')
         ```
 
 11. `<class>.len (property)`
     - Finds and returns the length of the current iterable class object as a property.
     - Arguments: `self`
     - Returns: `int`
     - Example:
```

### Comparing `overloaded-iterables-0.6/README.md` & `overloaded-iterables-0.6.1/src/overloaded_iterables.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,28 @@
-# Overloaded Iterables
+Metadata-Version: 2.1
+Name: overloaded-iterables
+Version: 0.6.1
+Summary: Overloaded version of the built-in python classes: list and set to include some extra functionalities.
+Home-page: https://github.com/Arkiralor/overloaded_iterables
+Author: Prithoo Medhi
+Author-email: prithoo11335@gmail.com
+License: MIT
+Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot
+Platform: windows
+Platform: ubuntu-linux
+Platform: mac-os
+Classifier: Development Status :: 3 - Alpha
+Classifier: Topic :: Utilities
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-Overloaded version of the built-in python classes: `<list>` and `<set>` to include some extra functionalities as an experiment.
+# Overloaded Iterables
 
-The current iteration contains the following classes
+Overloaded versions of the built-in python classes: `<list>` and `<set>` to include some extra functionalities as an experiment.
 
 ## Specifications
 
 1. __Python Version:__ Python v3.8+
 2. __Code Coverage:__ ![_code coverage_](https://github.com/Arkiralor/overloaded_iterables/blob/master/media/screenshots/coverage.PNG?raw=true)
 3. __Tests Status:__ ![_test status_](https://github.com/Arkiralor/overloaded_iterables/blob/master/media/screenshots/test_results.PNG?raw=true)
 
@@ -19,14 +35,16 @@
 
 ```sh
 python -m pip install overloaded-iterables
 ```
 
 ## Classes
 
+The current iteration contains the following classes
+
 ### 1. OverloadedList
 
 - A non-datatype constrained, single-dimensional collection of values.
 - Inherits solely from Python's built-in `<list>` class.
 
 ```python
 from overloaded_iterables.classes import OverloadedList
@@ -119,50 +137,50 @@
     - Example:
 
         ```python
             _median:float = obj.median()
         ```
 
 8. `<class>.hist()`&nbsp;&nbsp;&nbsp;&nbsp;__(OverloadedList only)__
-    - Plots the histogram of the frequency distribution of the elements in the OverloadedList.
+    - Plots the [histogram](https://en.wikipedia.org/wiki/Histogram) of the frequency distribution of the elements in the OverloadedList.
     - Arguments: `self`, `bins: int | default: 10`, `title: str | default: 'Histogram'`, `x_label: str | default: 'Values --->'`, `y_label: str | default: 'Frequencies --->'`, `save_dir: str | default: None`, `file_name: str | default: None`, `histtype: str | default: 'step'`, `align: str | default: 'mid'`, `orientation: str | default: 'vertical'`, `log_scale: bool | default: False`, `show: bool | default: False`
     - Process:
         - Shows the generated figure if `show` is set to `True`
         - Saves the generated figure if `save_dir` is provided.
     - Returns: `bool`
     - Example:
 
         ```python
-            fig_check:float = obj.hist(show=True, save_dir='figures', file_name='some-figure')
+            fig_check:bool = obj.hist(show=True, save_dir='figures', file_name='some-figure')
         ```
 
 9. `<class>.plot()`&nbsp;&nbsp;&nbsp;&nbsp;__(OverloadedList only)__
-    - Plots the lineplot of the frequency distribution of the elements in the OverloadedList.
+    - Plots the [lineplot](https://en.wikipedia.org/wiki/Line_chart) of the frequency distribution of the elements in the OverloadedList.
     - Arguments: `self`, `title: str | default: 'Line Plot'`, `x_label: str | default: 'Values --->'`, `y_label: str | default: 'Frequencies --->'`, `save_dir: str | default: None`, `file_name: str | default: None`, `color: str | default: '#000000'`, `linewidth: float | default: 1`, `marker: str | default: ','`,  `markerfacecolor: str | default: '#252525'`, `marker_size: float | default: 1.0`, `show: bool | default: False`
     - Process:
         - Shows the generated figure if `show` is set to `True`
         - Saves the generated figure if `save_dir` is provided.
     - Returns: `bool`
     - Example:
 
         ```python
-            fig_check:float = obj.plot(show=True, save_dir='figures', file_name='some-figure')
+            fig_check:bool = obj.plot(show=True, save_dir='figures', file_name='some-figure')
         ```
 
 10. `<class>.scatter()`&nbsp;&nbsp;&nbsp;&nbsp;__(OverloadedList only)__
-    - Plots the scatterplot of the frequency distribution of the elements in the OverloadedList.
+    - Plots the [scatterplot](https://en.wikipedia.org/wiki/Scatter_plot) of the frequency distribution of the elements in the OverloadedList.
     - Arguments: `self`, `title: str | default: 'Scatter Plot'`, `x_label: str | default: 'Values --->'`, `y_label: str | default: 'Frequencies --->'`, `save_dir: str | default: None`, `file_name: str | default: None`, `size: List[float] | default: [1.25]`, `color: str | default: '#000000'`, `marker: str | default: ','`, `line_width: float | default: 2`, `show: bool | default: False`
     - Process:
         - Shows the generated figure if `show` is set to `True`
         - Saves the generated figure if `save_dir` is provided.
     - Returns: `bool`
     - Example:
 
         ```python
-            fig_check:float = obj.scatter(show=True, save_dir='figures', file_name='some-figure')
+            fig_check:bool = obj.scatter(show=True, save_dir='figures', file_name='some-figure')
         ```
 
 11. `<class>.len (property)`
     - Finds and returns the length of the current iterable class object as a property.
     - Arguments: `self`
     - Returns: `int`
     - Example:
@@ -176,7 +194,9 @@
     - Arguments: `self`
     - Returns: `OverloadedList, OverloadedList`
     - Example:
 
         ```python
             values: Overloadedlist, frequencies: OverloadedList = obj.frequencies
         ```
+
+
```

### Comparing `overloaded-iterables-0.6/setup.py` & `overloaded-iterables-0.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         encoding="utf-8"
     )as file_obj:
         data = file_obj.read()
     return data
 
 setup(
     name='overloaded-iterables',
-    version='0.6',
+    version='0.6.1',
     description="Overloaded version of the built-in python classes: list and set to include some extra functionalities.",
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     license='MIT',
     author="Prithoo Medhi",
     author_email='prithoo11335@gmail.com',
     packages=find_packages('src'),
@@ -46,13 +46,13 @@
         "windows",
         "ubuntu-linux",
         "mac-os"
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Topic :: Utilities",
-        "License :: OSI Approved :: BSD License",
+        "License :: OSI Approved :: MIT License",
     ],
 )
 
 if __name__=="__main__":
     pass
```

### Comparing `overloaded-iterables-0.6/src/overloaded_iterables/classes.py` & `overloaded-iterables-0.6.1/src/overloaded_iterables/classes.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.6/src/overloaded_iterables.egg-info/PKG-INFO` & `overloaded-iterables-0.6.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,10 @@
-Metadata-Version: 2.1
-Name: overloaded-iterables
-Version: 0.6
-Summary: Overloaded version of the built-in python classes: list and set to include some extra functionalities.
-Home-page: https://github.com/Arkiralor/overloaded_iterables
-Author: Prithoo Medhi
-Author-email: prithoo11335@gmail.com
-License: MIT
-Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot
-Platform: windows
-Platform: ubuntu-linux
-Platform: mac-os
-Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: BSD License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Overloaded Iterables
 
-Overloaded version of the built-in python classes: `<list>` and `<set>` to include some extra functionalities as an experiment.
-
-The current iteration contains the following classes
+Overloaded versions of the built-in python classes: `<list>` and `<set>` to include some extra functionalities as an experiment.
 
 ## Specifications
 
 1. __Python Version:__ Python v3.8+
 2. __Code Coverage:__ ![_code coverage_](https://github.com/Arkiralor/overloaded_iterables/blob/master/media/screenshots/coverage.PNG?raw=true)
 3. __Tests Status:__ ![_test status_](https://github.com/Arkiralor/overloaded_iterables/blob/master/media/screenshots/test_results.PNG?raw=true)
 
@@ -37,14 +17,16 @@
 
 ```sh
 python -m pip install overloaded-iterables
 ```
 
 ## Classes
 
+The current iteration contains the following classes
+
 ### 1. OverloadedList
 
 - A non-datatype constrained, single-dimensional collection of values.
 - Inherits solely from Python's built-in `<list>` class.
 
 ```python
 from overloaded_iterables.classes import OverloadedList
@@ -137,50 +119,50 @@
     - Example:
 
         ```python
             _median:float = obj.median()
         ```
 
 8. `<class>.hist()`&nbsp;&nbsp;&nbsp;&nbsp;__(OverloadedList only)__
-    - Plots the histogram of the frequency distribution of the elements in the OverloadedList.
+    - Plots the [histogram](https://en.wikipedia.org/wiki/Histogram) of the frequency distribution of the elements in the OverloadedList.
     - Arguments: `self`, `bins: int | default: 10`, `title: str | default: 'Histogram'`, `x_label: str | default: 'Values --->'`, `y_label: str | default: 'Frequencies --->'`, `save_dir: str | default: None`, `file_name: str | default: None`, `histtype: str | default: 'step'`, `align: str | default: 'mid'`, `orientation: str | default: 'vertical'`, `log_scale: bool | default: False`, `show: bool | default: False`
     - Process:
         - Shows the generated figure if `show` is set to `True`
         - Saves the generated figure if `save_dir` is provided.
     - Returns: `bool`
     - Example:
 
         ```python
-            fig_check:float = obj.hist(show=True, save_dir='figures', file_name='some-figure')
+            fig_check:bool = obj.hist(show=True, save_dir='figures', file_name='some-figure')
         ```
 
 9. `<class>.plot()`&nbsp;&nbsp;&nbsp;&nbsp;__(OverloadedList only)__
-    - Plots the lineplot of the frequency distribution of the elements in the OverloadedList.
+    - Plots the [lineplot](https://en.wikipedia.org/wiki/Line_chart) of the frequency distribution of the elements in the OverloadedList.
     - Arguments: `self`, `title: str | default: 'Line Plot'`, `x_label: str | default: 'Values --->'`, `y_label: str | default: 'Frequencies --->'`, `save_dir: str | default: None`, `file_name: str | default: None`, `color: str | default: '#000000'`, `linewidth: float | default: 1`, `marker: str | default: ','`,  `markerfacecolor: str | default: '#252525'`, `marker_size: float | default: 1.0`, `show: bool | default: False`
     - Process:
         - Shows the generated figure if `show` is set to `True`
         - Saves the generated figure if `save_dir` is provided.
     - Returns: `bool`
     - Example:
 
         ```python
-            fig_check:float = obj.plot(show=True, save_dir='figures', file_name='some-figure')
+            fig_check:bool = obj.plot(show=True, save_dir='figures', file_name='some-figure')
         ```
 
 10. `<class>.scatter()`&nbsp;&nbsp;&nbsp;&nbsp;__(OverloadedList only)__
-    - Plots the scatterplot of the frequency distribution of the elements in the OverloadedList.
+    - Plots the [scatterplot](https://en.wikipedia.org/wiki/Scatter_plot) of the frequency distribution of the elements in the OverloadedList.
     - Arguments: `self`, `title: str | default: 'Scatter Plot'`, `x_label: str | default: 'Values --->'`, `y_label: str | default: 'Frequencies --->'`, `save_dir: str | default: None`, `file_name: str | default: None`, `size: List[float] | default: [1.25]`, `color: str | default: '#000000'`, `marker: str | default: ','`, `line_width: float | default: 2`, `show: bool | default: False`
     - Process:
         - Shows the generated figure if `show` is set to `True`
         - Saves the generated figure if `save_dir` is provided.
     - Returns: `bool`
     - Example:
 
         ```python
-            fig_check:float = obj.scatter(show=True, save_dir='figures', file_name='some-figure')
+            fig_check:bool = obj.scatter(show=True, save_dir='figures', file_name='some-figure')
         ```
 
 11. `<class>.len (property)`
     - Finds and returns the length of the current iterable class object as a property.
     - Arguments: `self`
     - Returns: `int`
     - Example:
@@ -194,9 +176,7 @@
     - Arguments: `self`
     - Returns: `OverloadedList, OverloadedList`
     - Example:
 
         ```python
             values: Overloadedlist, frequencies: OverloadedList = obj.frequencies
         ```
-
-
```

