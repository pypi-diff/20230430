# Comparing `tmp/raw-image-converter-1.0.2.tar.gz` & `tmp/raw-image-converter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raw-image-converter-1.0.2.tar", last modified: Mon Dec  5 09:58:08 2022, max compression
+gzip compressed data, was "raw-image-converter-1.0.3.tar", last modified: Sun Apr 30 07:00:37 2023, max compression
```

## Comparing `raw-image-converter-1.0.2.tar` & `raw-image-converter-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-12-05 09:58:08.281249 raw-image-converter-1.0.2/
--rw-rw-rw-   0        0        0     1074 2021-09-04 21:20:45.000000 raw-image-converter-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2423 2022-12-05 09:58:08.280250 raw-image-converter-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1826 2022-04-18 12:08:48.000000 raw-image-converter-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-12-05 09:58:08.258414 raw-image-converter-1.0.2/raw_image_converter/
--rw-rw-rw-   0        0        0      199 2022-12-05 09:54:38.000000 raw-image-converter-1.0.2/raw_image_converter/__init__.py
--rw-rw-rw-   0        0        0     5015 2022-12-05 09:49:00.000000 raw-image-converter-1.0.2/raw_image_converter/__main__.py
-drwxrwxrwx   0        0        0        0 2022-12-05 09:58:08.279247 raw-image-converter-1.0.2/raw_image_converter.egg-info/
--rw-rw-rw-   0        0        0     2423 2022-12-05 09:58:08.000000 raw-image-converter-1.0.2/raw_image_converter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2022-12-05 09:58:08.000000 raw-image-converter-1.0.2/raw_image_converter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-05 09:58:08.000000 raw-image-converter-1.0.2/raw_image_converter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2022-12-05 09:58:08.000000 raw-image-converter-1.0.2/raw_image_converter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       58 2022-12-05 09:58:08.000000 raw-image-converter-1.0.2/raw_image_converter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2022-12-05 09:58:08.000000 raw-image-converter-1.0.2/raw_image_converter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-05 09:58:08.281249 raw-image-converter-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1118 2022-12-05 09:54:38.000000 raw-image-converter-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:00:37.539960 raw-image-converter-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-30 07:00:23.000000 raw-image-converter-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-30 07:00:37.539960 raw-image-converter-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-30 07:00:23.000000 raw-image-converter-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:00:37.535960 raw-image-converter-1.0.3/raw_image_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-30 07:00:23.000000 raw-image-converter-1.0.3/raw_image_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-30 07:00:23.000000 raw-image-converter-1.0.3/raw_image_converter/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:00:37.539960 raw-image-converter-1.0.3/raw_image_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-30 07:00:37.000000 raw-image-converter-1.0.3/raw_image_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-30 07:00:37.000000 raw-image-converter-1.0.3/raw_image_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 07:00:37.000000 raw-image-converter-1.0.3/raw_image_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-30 07:00:37.000000 raw-image-converter-1.0.3/raw_image_converter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-30 07:00:37.000000 raw-image-converter-1.0.3/raw_image_converter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-30 07:00:37.000000 raw-image-converter-1.0.3/raw_image_converter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 07:00:37.539960 raw-image-converter-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-30 07:00:23.000000 raw-image-converter-1.0.3/setup.py
```

### Comparing `raw-image-converter-1.0.2/LICENSE` & `raw-image-converter-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `raw-image-converter-1.0.2/PKG-INFO` & `raw-image-converter-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,76 @@
-Metadata-Version: 2.1
-Name: raw-image-converter
-Version: 1.0.2
-Summary: Batch conversions of raw images
-Home-page: https://github.com/achimoraites/Python-Image-Converter
-Author: Achilles Moraites
-Author-email: achimoraites@yahoo.gr
-License: MIT
-Keywords: cli,converter,raw,images
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Python Image Converter
-
-## This is a simple Image converter written in Python
-The app is using PIL ,rawpy and imageio . 
-Files are converted to .jpg format 
-
-## Convert for FREE multiple image files
-I saw all kinds of software out there but when you have hundrends of raw images is tedious to convert 
-one by one! Other Options were to get program suits like photoshop or even pay! 
-# Notes
-The .ai files are renamed as .pdf and moved to the converted directory !!! 
-
-
-# What files can be used ?
-### DNG , CR2 , CRW, NEF , PEF, ERF , ORF , PPM , MOS , MRF , MRW , SRW and more!!!
-Personally i convert a lot of .psd , .TIF and .dng files !!! 
-## Speed
-This script is multithreaded and checks if you have already converted an image!
-
-## Install
-
-### Using pip (recommended)
-```bash
-$ pip3 install raw_image_converter
-```
-
-### Running it from the repo
-In that case using an virtual environment is recommended
-
-```bash
- git clone https://github.com/achimoraites/Python-Image-Converter.git [my-app-name]
- cd [my-app-name]
-
- pip install -r requirements.txt
-
- raw_image_converter --s <Enter-Path-Of-Directory>
-```
-## Example usage
-
-```
- # simple usage
- raw_image_converter --s <Enter-Path-Of-Directory>
-
- # set a custom target image format
- raw_image_converter --s <Enter-Path-Of-Directory> --ext '.png'
-```
-- The --s argument is where you set the path to the directory you want to convert! 
-- The --ext argument is where you specify the image format that will be used for the converted images; by default the `.jpg` is used. valid options are:
-    - `.jpg`
-    - `.png`
-
-The application will create a folder 'converted' where all your converted images are located!
-
-And you are done! 
-
-## ScreenShot
-<img src='https://raw.githubusercontent.com/achimoraites/Python-Image-Converter/master/sample.png' alt='Python Image Converter'>
-
+Metadata-Version: 2.1
+Name: raw-image-converter
+Version: 1.0.3
+Summary: Batch conversions of raw images
+Home-page: https://github.com/achimoraites/Python-Image-Converter
+Author: Achilles Moraites
+Author-email: achimoraites@yahoo.gr
+License: MIT
+Keywords: cli,converter,raw,images
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Python Image Converter
+[![PyPI version](https://badge.fury.io/py/raw-image-converter.svg)](https://pypi.org/project/raw-image-converter/)
+
+
+## This is a simple Image converter written in Python
+The app is using PIL ,rawpy and imageio . 
+Files are converted to .jpg format 
+
+## Convert for FREE multiple image files
+I saw all kinds of software out there but when you have hundrends of raw images is tedious to convert 
+one by one! Other Options were to get program suits like photoshop or even pay! 
+# Notes
+The .ai files are renamed as .pdf and moved to the converted directory !!! 
+
+
+# What files can be used ?
+### DNG , CR2 , CRW, NEF , PEF, ERF , ORF , PPM , MOS , MRF , MRW , SRW and more!!!
+Personally i convert a lot of .psd , .TIF and .dng files !!! 
+## Speed
+This script is multithreaded and checks if you have already converted an image!
+
+## Install
+
+### Using pip (recommended)
+```bash
+$ pip3 install raw_image_converter
+```
+
+### Running it from the repo
+In that case using an virtual environment is recommended
+
+```bash
+ git clone https://github.com/achimoraites/Python-Image-Converter.git [my-app-name]
+ cd [my-app-name]
+
+ pip install -r requirements.txt
+
+ raw_image_converter --s <Enter-Path-Of-Directory>
+```
+## Example usage
+
+```
+ # simple usage
+ raw_image_converter --s <Enter-Path-Of-Directory>
+
+ # set a custom target image format
+ raw_image_converter --s <Enter-Path-Of-Directory> --ext '.png'
+```
+- The --s argument is where you set the path to the directory you want to convert! 
+- The --ext argument is where you specify the image format that will be used for the converted images; by default the `.jpg` is used. valid options are:
+    - `.jpg`
+    - `.png`
+
+The application will create a folder 'converted' where all your converted images are located!
+
+And you are done! 
+
+## ScreenShot
+<img src='https://raw.githubusercontent.com/achimoraites/Python-Image-Converter/master/sample.png' alt='Python Image Converter'>
+
```

### Comparing `raw-image-converter-1.0.2/README.md` & `raw-image-converter-1.0.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # Python Image Converter
+[![PyPI version](https://badge.fury.io/py/raw-image-converter.svg)](https://pypi.org/project/raw-image-converter/)
+
 
 ## This is a simple Image converter written in Python
 The app is using PIL ,rawpy and imageio . 
 Files are converted to .jpg format 
 
 ## Convert for FREE multiple image files
 I saw all kinds of software out there but when you have hundrends of raw images is tedious to convert
```

### Comparing `raw-image-converter-1.0.2/raw_image_converter/__main__.py` & `raw-image-converter-1.0.3/raw_image_converter/__main__.py`

 * *Files identical despite different names*

### Comparing `raw-image-converter-1.0.2/raw_image_converter.egg-info/PKG-INFO` & `raw-image-converter-1.0.3/raw_image_converter.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,76 @@
-Metadata-Version: 2.1
-Name: raw-image-converter
-Version: 1.0.2
-Summary: Batch conversions of raw images
-Home-page: https://github.com/achimoraites/Python-Image-Converter
-Author: Achilles Moraites
-Author-email: achimoraites@yahoo.gr
-License: MIT
-Keywords: cli,converter,raw,images
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Python Image Converter
-
-## This is a simple Image converter written in Python
-The app is using PIL ,rawpy and imageio . 
-Files are converted to .jpg format 
-
-## Convert for FREE multiple image files
-I saw all kinds of software out there but when you have hundrends of raw images is tedious to convert 
-one by one! Other Options were to get program suits like photoshop or even pay! 
-# Notes
-The .ai files are renamed as .pdf and moved to the converted directory !!! 
-
-
-# What files can be used ?
-### DNG , CR2 , CRW, NEF , PEF, ERF , ORF , PPM , MOS , MRF , MRW , SRW and more!!!
-Personally i convert a lot of .psd , .TIF and .dng files !!! 
-## Speed
-This script is multithreaded and checks if you have already converted an image!
-
-## Install
-
-### Using pip (recommended)
-```bash
-$ pip3 install raw_image_converter
-```
-
-### Running it from the repo
-In that case using an virtual environment is recommended
-
-```bash
- git clone https://github.com/achimoraites/Python-Image-Converter.git [my-app-name]
- cd [my-app-name]
-
- pip install -r requirements.txt
-
- raw_image_converter --s <Enter-Path-Of-Directory>
-```
-## Example usage
-
-```
- # simple usage
- raw_image_converter --s <Enter-Path-Of-Directory>
-
- # set a custom target image format
- raw_image_converter --s <Enter-Path-Of-Directory> --ext '.png'
-```
-- The --s argument is where you set the path to the directory you want to convert! 
-- The --ext argument is where you specify the image format that will be used for the converted images; by default the `.jpg` is used. valid options are:
-    - `.jpg`
-    - `.png`
-
-The application will create a folder 'converted' where all your converted images are located!
-
-And you are done! 
-
-## ScreenShot
-<img src='https://raw.githubusercontent.com/achimoraites/Python-Image-Converter/master/sample.png' alt='Python Image Converter'>
-
+Metadata-Version: 2.1
+Name: raw-image-converter
+Version: 1.0.3
+Summary: Batch conversions of raw images
+Home-page: https://github.com/achimoraites/Python-Image-Converter
+Author: Achilles Moraites
+Author-email: achimoraites@yahoo.gr
+License: MIT
+Keywords: cli,converter,raw,images
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Python Image Converter
+[![PyPI version](https://badge.fury.io/py/raw-image-converter.svg)](https://pypi.org/project/raw-image-converter/)
+
+
+## This is a simple Image converter written in Python
+The app is using PIL ,rawpy and imageio . 
+Files are converted to .jpg format 
+
+## Convert for FREE multiple image files
+I saw all kinds of software out there but when you have hundrends of raw images is tedious to convert 
+one by one! Other Options were to get program suits like photoshop or even pay! 
+# Notes
+The .ai files are renamed as .pdf and moved to the converted directory !!! 
+
+
+# What files can be used ?
+### DNG , CR2 , CRW, NEF , PEF, ERF , ORF , PPM , MOS , MRF , MRW , SRW and more!!!
+Personally i convert a lot of .psd , .TIF and .dng files !!! 
+## Speed
+This script is multithreaded and checks if you have already converted an image!
+
+## Install
+
+### Using pip (recommended)
+```bash
+$ pip3 install raw_image_converter
+```
+
+### Running it from the repo
+In that case using an virtual environment is recommended
+
+```bash
+ git clone https://github.com/achimoraites/Python-Image-Converter.git [my-app-name]
+ cd [my-app-name]
+
+ pip install -r requirements.txt
+
+ raw_image_converter --s <Enter-Path-Of-Directory>
+```
+## Example usage
+
+```
+ # simple usage
+ raw_image_converter --s <Enter-Path-Of-Directory>
+
+ # set a custom target image format
+ raw_image_converter --s <Enter-Path-Of-Directory> --ext '.png'
+```
+- The --s argument is where you set the path to the directory you want to convert! 
+- The --ext argument is where you specify the image format that will be used for the converted images; by default the `.jpg` is used. valid options are:
+    - `.jpg`
+    - `.png`
+
+The application will create a folder 'converted' where all your converted images are located!
+
+And you are done! 
+
+## ScreenShot
+<img src='https://raw.githubusercontent.com/achimoraites/Python-Image-Converter/master/sample.png' alt='Python Image Converter'>
+
```

### Comparing `raw-image-converter-1.0.2/setup.py` & `raw-image-converter-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="raw-image-converter",
-    version="1.0.2",
+    version="1.0.3",
     description="Batch conversions of raw images",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/achimoraites/Python-Image-Converter",
     author="Achilles Moraites",
     author_email="achimoraites@yahoo.gr",
     license="MIT",
@@ -23,14 +23,14 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         'Topic :: Utilities',
     ],
     keywords='cli, converter, raw, images',
     packages=["raw_image_converter"],
     install_requires=["numpy==1.22.3", "rawpy==0.17.1",
-                      "imageio==2.16.2", "Pillow==9.2.0"],
+                      "imageio==2.16.2", "Pillow==9.3.0"],
     entry_points={
         "console_scripts": [
             "raw_image_converter=raw_image_converter.__main__:main",
         ]
     },
 )
```

