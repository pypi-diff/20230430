# Comparing `tmp/pyqt-darktheme-1.3.tar.gz` & `tmp/pyqt-darktheme-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt-darktheme-1.3.tar", last modified: Sun Apr 30 12:58:46 2023, max compression
+gzip compressed data, was "pyqt-darktheme-1.3.1.tar", last modified: Sun Apr 30 13:09:57 2023, max compression
```

## Comparing `pyqt-darktheme-1.3.tar` & `pyqt-darktheme-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 12:58:46.092514 pyqt-darktheme-1.3/
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)    35149 2023-04-30 09:15:46.000000 pyqt-darktheme-1.3/LICENSE
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     4942 2023-04-30 12:58:46.091514 pyqt-darktheme-1.3/PKG-INFO
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     4425 2023-04-30 12:58:19.000000 pyqt-darktheme-1.3/README.md
-drwxr-xr-x   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 12:58:46.088514 pyqt-darktheme-1.3/darktheme/
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 09:15:46.000000 pyqt-darktheme-1.3/darktheme/__init__.py
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     2699 2023-04-30 10:13:33.000000 pyqt-darktheme-1.3/darktheme/decorators.py
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     2699 2023-04-30 10:13:00.000000 pyqt-darktheme-1.3/darktheme/decorators_pyqt6.py
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     4519 2023-04-30 10:08:51.000000 pyqt-darktheme-1.3/darktheme/widget_template.py
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     4775 2023-04-30 09:57:45.000000 pyqt-darktheme-1.3/darktheme/widget_template_pyqt6.py
-drwxr-xr-x   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 12:58:46.090514 pyqt-darktheme-1.3/pyqt_darktheme.egg-info/
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     4942 2023-04-30 12:58:46.000000 pyqt-darktheme-1.3/pyqt_darktheme.egg-info/PKG-INFO
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)      318 2023-04-30 12:58:46.000000 pyqt-darktheme-1.3/pyqt_darktheme.egg-info/SOURCES.txt
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)        1 2023-04-30 12:58:46.000000 pyqt-darktheme-1.3/pyqt_darktheme.egg-info/dependency_links.txt
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)       10 2023-04-30 12:58:46.000000 pyqt-darktheme-1.3/pyqt_darktheme.egg-info/top_level.txt
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)       38 2023-04-30 12:58:46.092514 pyqt-darktheme-1.3/setup.cfg
--rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)      758 2023-04-30 10:24:35.000000 pyqt-darktheme-1.3/setup.py
+drwxr-xr-x   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 13:09:57.558184 pyqt-darktheme-1.3.1/
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)    35149 2023-04-30 09:15:46.000000 pyqt-darktheme-1.3.1/LICENSE
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     5071 2023-04-30 13:09:57.558184 pyqt-darktheme-1.3.1/PKG-INFO
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     4552 2023-04-30 13:09:10.000000 pyqt-darktheme-1.3.1/README.md
+drwxr-xr-x   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 13:09:57.557184 pyqt-darktheme-1.3.1/darktheme/
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 09:15:46.000000 pyqt-darktheme-1.3.1/darktheme/__init__.py
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     2699 2023-04-30 10:13:33.000000 pyqt-darktheme-1.3.1/darktheme/decorators.py
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     2699 2023-04-30 10:13:00.000000 pyqt-darktheme-1.3.1/darktheme/decorators_pyqt6.py
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     4519 2023-04-30 10:08:51.000000 pyqt-darktheme-1.3.1/darktheme/widget_template.py
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     4775 2023-04-30 09:57:45.000000 pyqt-darktheme-1.3.1/darktheme/widget_template_pyqt6.py
+drwxr-xr-x   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 13:09:57.558184 pyqt-darktheme-1.3.1/pyqt_darktheme.egg-info/
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     5071 2023-04-30 13:09:57.000000 pyqt-darktheme-1.3.1/pyqt_darktheme.egg-info/PKG-INFO
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)      318 2023-04-30 13:09:57.000000 pyqt-darktheme-1.3.1/pyqt_darktheme.egg-info/SOURCES.txt
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)        1 2023-04-30 13:09:57.000000 pyqt-darktheme-1.3.1/pyqt_darktheme.egg-info/dependency_links.txt
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)       10 2023-04-30 13:09:57.000000 pyqt-darktheme-1.3.1/pyqt_darktheme.egg-info/top_level.txt
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)       38 2023-04-30 13:09:57.558184 pyqt-darktheme-1.3.1/setup.cfg
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)      760 2023-04-30 13:04:52.000000 pyqt-darktheme-1.3.1/setup.py
```

### Comparing `pyqt-darktheme-1.3/LICENSE` & `pyqt-darktheme-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqt-darktheme-1.3/PKG-INFO` & `pyqt-darktheme-1.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt-darktheme
-Version: 1.3
+Version: 1.3.1
 Summary: A PyQt dark theme, clickable widgets and cursor decorators
 Home-page: https://github.com/Michael-Yongshi/Gui-Dark-Theme
 Author: Michael-Yongshi
 Author-email: 4registration@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,16 @@
 ![darktheme](https://user-images.githubusercontent.com/39827427/133036509-759bc459-087a-4a1d-a86d-098c410de5bc.png)
 
 ## Test and examples
 Run the 'test_gui.py' (for pyqt5) or 'test_gui_pyqt6.py file to see how it compares to the normal light theme and to test the library on your device.
 
 ## Version
 ### 1.3
+1.3.1   Only some readme edits
+
 1.3.0   Added a pyqt6 implementation, but does not automatically install either PyQt5 or PyQt6 as you can now choose between them
 ### 1.2
 1.2.5   Added a test_gui to showcase the themes and for testing
 
 1.2.4   changed elements for tabs, radio buttons, and checkboxes when they are disabled
 
 1.2.3   Changed folder name to darktheme
@@ -37,14 +39,17 @@
 Make sure you have PyQt5 or PyQt6 installed
 
 ```
 pip install pyqt-darktheme
 ```
 
 ## How to use the dark theme
+
+See the 'test_gui.py' and 'test_gui_pyqt6.py' files for configuration examples
+
 ### Import
 To import the dark theme as a class based on QPalette
 
 PyQt5
 ```
 from darktheme.widget_template import DarkApplication, DarkPalette
 ```
@@ -58,29 +63,34 @@
 #### using DarkPalette
 Create a QApplication object and set the DarkPalette like below
 ```
 app = QApplication()
 app.setPalette(DarkPalette())
 ```
 
-See the 'test_gui.py' file for an example how to make it configurable
-
 #### using DarkApplication
 For an application that is fixed in a dark theme, you can use the DarkApplication class
 ```
 app = QDarkApplication()
 ```
 
 ## How to use the Clickable Widgets
 ### Import
 To import the clickable widgets, i.e. a clickable label widget
+
+For PyQt5
 ```
 from darktheme.widget_template import QClickLabel
 ```
 
+For PyQt6
+```
+from darktheme.widget_template_pyqt6 import QClickLabel
+```
+
 ### Configure
 ```
 label = QClickLabel()
 label.setText('This label is clickable')
 label.clicked.connect(clicklabel)
 
 def clicklabel:
@@ -148,22 +158,22 @@
 ```
 [distutils]
 index-servers=
     pypi
     test
 
 [test]
-repository = https://testpypi.python.org/pypi
+repository = https://test.pypi.org/legacy/
 username = __token__
 password = <PyPI token>
 
 [pypi]
-repository = http://pypi.python.org/pypi
+repository = https://upload.pypi.org/legacy/
 username = __token__
-password = <token_string>
+password = <PyPI token>
 ```
 
 ## Distributions
 
 ```
 python3 -m pip install --upgrade build && python3 -m build
 ```
```

### Comparing `pyqt-darktheme-1.3/README.md` & `pyqt-darktheme-1.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 ![darktheme](https://user-images.githubusercontent.com/39827427/133036509-759bc459-087a-4a1d-a86d-098c410de5bc.png)
 
 ## Test and examples
 Run the 'test_gui.py' (for pyqt5) or 'test_gui_pyqt6.py file to see how it compares to the normal light theme and to test the library on your device.
 
 ## Version
 ### 1.3
+1.3.1   Only some readme edits
+
 1.3.0   Added a pyqt6 implementation, but does not automatically install either PyQt5 or PyQt6 as you can now choose between them
 ### 1.2
 1.2.5   Added a test_gui to showcase the themes and for testing
 
 1.2.4   changed elements for tabs, radio buttons, and checkboxes when they are disabled
 
 1.2.3   Changed folder name to darktheme
@@ -23,14 +25,17 @@
 Make sure you have PyQt5 or PyQt6 installed
 
 ```
 pip install pyqt-darktheme
 ```
 
 ## How to use the dark theme
+
+See the 'test_gui.py' and 'test_gui_pyqt6.py' files for configuration examples
+
 ### Import
 To import the dark theme as a class based on QPalette
 
 PyQt5
 ```
 from darktheme.widget_template import DarkApplication, DarkPalette
 ```
@@ -44,29 +49,34 @@
 #### using DarkPalette
 Create a QApplication object and set the DarkPalette like below
 ```
 app = QApplication()
 app.setPalette(DarkPalette())
 ```
 
-See the 'test_gui.py' file for an example how to make it configurable
-
 #### using DarkApplication
 For an application that is fixed in a dark theme, you can use the DarkApplication class
 ```
 app = QDarkApplication()
 ```
 
 ## How to use the Clickable Widgets
 ### Import
 To import the clickable widgets, i.e. a clickable label widget
+
+For PyQt5
 ```
 from darktheme.widget_template import QClickLabel
 ```
 
+For PyQt6
+```
+from darktheme.widget_template_pyqt6 import QClickLabel
+```
+
 ### Configure
 ```
 label = QClickLabel()
 label.setText('This label is clickable')
 label.clicked.connect(clicklabel)
 
 def clicklabel:
@@ -134,22 +144,22 @@
 ```
 [distutils]
 index-servers=
     pypi
     test
 
 [test]
-repository = https://testpypi.python.org/pypi
+repository = https://test.pypi.org/legacy/
 username = __token__
 password = <PyPI token>
 
 [pypi]
-repository = http://pypi.python.org/pypi
+repository = https://upload.pypi.org/legacy/
 username = __token__
-password = <token_string>
+password = <PyPI token>
 ```
 
 ## Distributions
 
 ```
 python3 -m pip install --upgrade build && python3 -m build
 ```
```

### Comparing `pyqt-darktheme-1.3/darktheme/decorators.py` & `pyqt-darktheme-1.3.1/darktheme/decorators.py`

 * *Files identical despite different names*

### Comparing `pyqt-darktheme-1.3/darktheme/decorators_pyqt6.py` & `pyqt-darktheme-1.3.1/darktheme/decorators_pyqt6.py`

 * *Files identical despite different names*

### Comparing `pyqt-darktheme-1.3/darktheme/widget_template.py` & `pyqt-darktheme-1.3.1/darktheme/widget_template.py`

 * *Files identical despite different names*

### Comparing `pyqt-darktheme-1.3/darktheme/widget_template_pyqt6.py` & `pyqt-darktheme-1.3.1/darktheme/widget_template_pyqt6.py`

 * *Files identical despite different names*

### Comparing `pyqt-darktheme-1.3/pyqt_darktheme.egg-info/PKG-INFO` & `pyqt-darktheme-1.3.1/pyqt_darktheme.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt-darktheme
-Version: 1.3
+Version: 1.3.1
 Summary: A PyQt dark theme, clickable widgets and cursor decorators
 Home-page: https://github.com/Michael-Yongshi/Gui-Dark-Theme
 Author: Michael-Yongshi
 Author-email: 4registration@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,16 @@
 ![darktheme](https://user-images.githubusercontent.com/39827427/133036509-759bc459-087a-4a1d-a86d-098c410de5bc.png)
 
 ## Test and examples
 Run the 'test_gui.py' (for pyqt5) or 'test_gui_pyqt6.py file to see how it compares to the normal light theme and to test the library on your device.
 
 ## Version
 ### 1.3
+1.3.1   Only some readme edits
+
 1.3.0   Added a pyqt6 implementation, but does not automatically install either PyQt5 or PyQt6 as you can now choose between them
 ### 1.2
 1.2.5   Added a test_gui to showcase the themes and for testing
 
 1.2.4   changed elements for tabs, radio buttons, and checkboxes when they are disabled
 
 1.2.3   Changed folder name to darktheme
@@ -37,14 +39,17 @@
 Make sure you have PyQt5 or PyQt6 installed
 
 ```
 pip install pyqt-darktheme
 ```
 
 ## How to use the dark theme
+
+See the 'test_gui.py' and 'test_gui_pyqt6.py' files for configuration examples
+
 ### Import
 To import the dark theme as a class based on QPalette
 
 PyQt5
 ```
 from darktheme.widget_template import DarkApplication, DarkPalette
 ```
@@ -58,29 +63,34 @@
 #### using DarkPalette
 Create a QApplication object and set the DarkPalette like below
 ```
 app = QApplication()
 app.setPalette(DarkPalette())
 ```
 
-See the 'test_gui.py' file for an example how to make it configurable
-
 #### using DarkApplication
 For an application that is fixed in a dark theme, you can use the DarkApplication class
 ```
 app = QDarkApplication()
 ```
 
 ## How to use the Clickable Widgets
 ### Import
 To import the clickable widgets, i.e. a clickable label widget
+
+For PyQt5
 ```
 from darktheme.widget_template import QClickLabel
 ```
 
+For PyQt6
+```
+from darktheme.widget_template_pyqt6 import QClickLabel
+```
+
 ### Configure
 ```
 label = QClickLabel()
 label.setText('This label is clickable')
 label.clicked.connect(clicklabel)
 
 def clicklabel:
@@ -148,22 +158,22 @@
 ```
 [distutils]
 index-servers=
     pypi
     test
 
 [test]
-repository = https://testpypi.python.org/pypi
+repository = https://test.pypi.org/legacy/
 username = __token__
 password = <PyPI token>
 
 [pypi]
-repository = http://pypi.python.org/pypi
+repository = https://upload.pypi.org/legacy/
 username = __token__
-password = <token_string>
+password = <PyPI token>
 ```
 
 ## Distributions
 
 ```
 python3 -m pip install --upgrade build && python3 -m build
 ```
```

### Comparing `pyqt-darktheme-1.3/setup.py` & `pyqt-darktheme-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyqt-darktheme",
-    version="1.3",
+    version="1.3.1",
     author="Michael-Yongshi",
     author_email="4registration@outlook.com",
     description="A PyQt dark theme, clickable widgets and cursor decorators",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Michael-Yongshi/Gui-Dark-Theme",
     packages=setuptools.find_packages(),
```

