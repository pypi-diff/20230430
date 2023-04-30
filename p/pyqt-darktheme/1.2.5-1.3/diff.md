# Comparing `tmp/pyqt-darktheme-1.2.5.tar.gz` & `tmp/pyqt-darktheme-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt-darktheme-1.2.5.tar", last modified: Sat Sep 11 15:33:31 2021, max compression
+gzip compressed data, was "pyqt-darktheme-1.3.tar", last modified: Sun Apr 30 12:58:46 2023, max compression
```

## Comparing `pyqt-darktheme-1.2.5.tar` & `pyqt-darktheme-1.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 yongshi   (1000) yongshi   (1000)        0 2021-09-11 15:33:31.155703 pyqt-darktheme-1.2.5/
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)     4513 2021-09-11 15:33:31.155703 pyqt-darktheme-1.2.5/PKG-INFO
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)     3128 2021-09-11 15:25:00.000000 pyqt-darktheme-1.2.5/README.md
-drwxrwxr-x   0 yongshi   (1000) yongshi   (1000)        0 2021-09-11 15:33:31.155703 pyqt-darktheme-1.2.5/darktheme/
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)        0 2021-09-10 20:58:31.000000 pyqt-darktheme-1.2.5/darktheme/__init__.py
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)     2699 2021-09-10 21:04:31.000000 pyqt-darktheme-1.2.5/darktheme/decorators.py
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)     4519 2021-09-11 14:44:33.000000 pyqt-darktheme-1.2.5/darktheme/widget_template.py
-drwxrwxr-x   0 yongshi   (1000) yongshi   (1000)        0 2021-09-11 15:33:31.155703 pyqt-darktheme-1.2.5/pyqt_darktheme.egg-info/
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)     4513 2021-09-11 15:33:31.000000 pyqt-darktheme-1.2.5/pyqt_darktheme.egg-info/PKG-INFO
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)      282 2021-09-11 15:33:31.000000 pyqt-darktheme-1.2.5/pyqt_darktheme.egg-info/SOURCES.txt
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)        1 2021-09-11 15:33:31.000000 pyqt-darktheme-1.2.5/pyqt_darktheme.egg-info/dependency_links.txt
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)        6 2021-09-11 15:33:31.000000 pyqt-darktheme-1.2.5/pyqt_darktheme.egg-info/requires.txt
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)       10 2021-09-11 15:33:31.000000 pyqt-darktheme-1.2.5/pyqt_darktheme.egg-info/top_level.txt
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)       38 2021-09-11 15:33:31.155703 pyqt-darktheme-1.2.5/setup.cfg
--rw-rw-r--   0 yongshi   (1000) yongshi   (1000)      782 2021-09-11 15:25:52.000000 pyqt-darktheme-1.2.5/setup.py
+drwxr-xr-x   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 12:58:46.092514 pyqt-darktheme-1.3/
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)    35149 2023-04-30 09:15:46.000000 pyqt-darktheme-1.3/LICENSE
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     4942 2023-04-30 12:58:46.091514 pyqt-darktheme-1.3/PKG-INFO
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     4425 2023-04-30 12:58:19.000000 pyqt-darktheme-1.3/README.md
+drwxr-xr-x   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 12:58:46.088514 pyqt-darktheme-1.3/darktheme/
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 09:15:46.000000 pyqt-darktheme-1.3/darktheme/__init__.py
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     2699 2023-04-30 10:13:33.000000 pyqt-darktheme-1.3/darktheme/decorators.py
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     2699 2023-04-30 10:13:00.000000 pyqt-darktheme-1.3/darktheme/decorators_pyqt6.py
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     4519 2023-04-30 10:08:51.000000 pyqt-darktheme-1.3/darktheme/widget_template.py
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     4775 2023-04-30 09:57:45.000000 pyqt-darktheme-1.3/darktheme/widget_template_pyqt6.py
+drwxr-xr-x   0 msi-laptop  (1000) msi-laptop  (1000)        0 2023-04-30 12:58:46.090514 pyqt-darktheme-1.3/pyqt_darktheme.egg-info/
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)     4942 2023-04-30 12:58:46.000000 pyqt-darktheme-1.3/pyqt_darktheme.egg-info/PKG-INFO
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)      318 2023-04-30 12:58:46.000000 pyqt-darktheme-1.3/pyqt_darktheme.egg-info/SOURCES.txt
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)        1 2023-04-30 12:58:46.000000 pyqt-darktheme-1.3/pyqt_darktheme.egg-info/dependency_links.txt
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)       10 2023-04-30 12:58:46.000000 pyqt-darktheme-1.3/pyqt_darktheme.egg-info/top_level.txt
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)       38 2023-04-30 12:58:46.092514 pyqt-darktheme-1.3/setup.cfg
+-rw-r--r--   0 msi-laptop  (1000) msi-laptop  (1000)      758 2023-04-30 10:24:35.000000 pyqt-darktheme-1.3/setup.py
```

### Comparing `pyqt-darktheme-1.2.5/darktheme/decorators.py` & `pyqt-darktheme-1.3/darktheme/decorators.py`

 * *Files identical despite different names*

### Comparing `pyqt-darktheme-1.2.5/darktheme/widget_template.py` & `pyqt-darktheme-1.3/darktheme/widget_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,36 +18,36 @@
 
 
 class DarkPalette(QPalette):
     """A Dark palette meant to be used with the Fusion theme."""
     def __init__(self, *__args):
         super().__init__(*__args)
         
-        self.setColor(QPalette.Window, QColor(53, 53, 53))          #dark grey (normal background widgets and main)
+        self.setColor(QPalette.Window, QColor(50, 50, 50))          #dark grey (normal background widgets and main)
         self.setColor(QPalette.WindowText, QColor(255, 255, 255))   #white
         self.setColor(QPalette.Base, QColor(25, 25, 25))            #darker grey (selected text in pop up)
-        self.setColor(QPalette.AlternateBase, QColor(53, 53, 53))   #dark grey (not used far as i can see)
+        self.setColor(QPalette.AlternateBase, QColor(50, 50, 50))   #dark grey (not used far as i can see)
         self.setColor(QPalette.ToolTipBase, QColor(100, 100, 100))  #medium grey (tooltip background)
         self.setColor(QPalette.ToolTipText, QColor(255, 255, 255))  #white (tooltip text)
         self.setColor(QPalette.Text, QColor(255, 255, 255))         #white
-        self.setColor(QPalette.Button, QColor(53, 53, 53))          #dark grey (drop down arrow colour and tabs)
+        self.setColor(QPalette.Button, QColor(50, 50, 50))          #dark grey (drop down arrow colour and tabs)
         self.setColor(QPalette.ButtonText, QColor(255, 255, 255))   #white
         self.setColor(QPalette.BrightText, QColor(255, 0, 0))       #red
         self.setColor(QPalette.Link, QColor(42, 130, 218))          #blue
         self.setColor(QPalette.Highlight, QColor(42, 130, 218))     #blue
         self.setColor(QPalette.HighlightedText, QColor(0, 0, 0))    #black
 
         # If item is disabled, use alternative colours
         # self.setColor(QPalette.Disabled, QPalette.Light, QColor(100, 100, 100))
         # self.setColor(QPalette.Disabled, QPalette.Shadow, QColor(255, 255, 255))
-        self.setColor(QPalette.Disabled, QPalette.Button, QColor(53, 53, 53))       #dark grey
+        self.setColor(QPalette.Disabled, QPalette.Button, QColor(50, 50, 50))       #dark grey
         self.setColor(QPalette.Disabled, QPalette.ButtonText, QColor(25, 25, 25))   #darker grey
-        self.setColor(QPalette.Disabled, QPalette.Base, QColor(53, 53, 53))          #dark grey
+        self.setColor(QPalette.Disabled, QPalette.Base, QColor(50, 50, 50))          #dark grey
         self.setColor(QPalette.Disabled, QPalette.Text, QColor(100, 100, 100))  #medium grey
-        self.setColor(QPalette.Disabled, QPalette.Window, QColor(53, 53, 53))          #dark grey
+        self.setColor(QPalette.Disabled, QPalette.Window, QColor(50, 50, 50))          #dark grey
         self.setColor(QPalette.Disabled, QPalette.WindowText, QColor(100, 100, 100))  #medium grey
 
 class DarkApplication(QApplication):
     """A Dark styled application."""
     def __init__(self, *__args):
         super().__init__(*__args)
```

### Comparing `pyqt-darktheme-1.2.5/setup.py` & `pyqt-darktheme-1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyqt-darktheme",
-    version="1.2.5",
+    version="1.3",
     author="Michael-Yongshi",
     author_email="4registration@outlook.com",
     description="A PyQt dark theme, clickable widgets and cursor decorators",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Michael-Yongshi/Gui-Dark-Theme",
     packages=setuptools.find_packages(),
-    install_requires=[
-        'PyQt5',
-    ],
+    install_requires=[],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.5',
+    python_requires='>=3.7',
 )
```

