# Comparing `tmp/CVAugmentor-1.0.0.tar.gz` & `tmp/CVAugmentor-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CVAugmentor-1.0.0.tar", last modified: Sun Apr 30 08:40:21 2023, max compression
+gzip compressed data, was "CVAugmentor-1.0.1.tar", last modified: Sun Apr 30 08:56:52 2023, max compression
```

## Comparing `CVAugmentor-1.0.0.tar` & `CVAugmentor-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 08:40:21.915469 CVAugmentor-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-04-30 08:40:21.839448 CVAugmentor-1.0.0/CVAugmentor/
--rw-rw-rw-   0        0        0      498 2023-04-30 08:40:00.000000 CVAugmentor-1.0.0/CVAugmentor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:40:21.864456 CVAugmentor-1.0.0/CVAugmentor/assets/
--rw-rw-rw-   0        0        0      317 2023-04-29 05:52:52.000000 CVAugmentor-1.0.0/CVAugmentor/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:40:21.905453 CVAugmentor-1.0.0/CVAugmentor/assets/main/
--rw-rw-rw-   0        0        0      178 2023-04-29 05:52:49.000000 CVAugmentor-1.0.0/CVAugmentor/assets/main/__init__.py
--rw-rw-rw-   0        0        0    26982 2023-04-29 09:27:03.000000 CVAugmentor-1.0.0/CVAugmentor/assets/main/augmentations_class.py
--rw-rw-rw-   0        0        0     3519 2023-04-27 08:22:59.000000 CVAugmentor-1.0.0/CVAugmentor/assets/main/image_augmentor_class.py
--rw-rw-rw-   0        0        0     6805 2023-04-27 08:38:31.000000 CVAugmentor-1.0.0/CVAugmentor/assets/main/video_augmentor_class.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:40:21.912470 CVAugmentor-1.0.0/CVAugmentor/assets/utils/
--rw-rw-rw-   0        0        0      143 2023-04-29 05:59:11.000000 CVAugmentor-1.0.0/CVAugmentor/assets/utils/__init__.py
--rw-rw-rw-   0        0        0      858 2023-03-26 09:42:33.000000 CVAugmentor-1.0.0/CVAugmentor/assets/utils/alphanumeric_sorter_class.py
--rw-rw-rw-   0        0        0     1210 2023-04-27 07:28:18.000000 CVAugmentor-1.0.0/CVAugmentor/assets/utils/file_type_checker_class.py
--rw-rw-rw-   0        0        0     6776 2023-04-29 08:09:44.000000 CVAugmentor-1.0.0/CVAugmentor/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:40:21.860465 CVAugmentor-1.0.0/CVAugmentor.egg-info/
--rw-rw-rw-   0        0        0     3176 2023-04-30 08:40:21.000000 CVAugmentor-1.0.0/CVAugmentor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      569 2023-04-30 08:40:21.000000 CVAugmentor-1.0.0/CVAugmentor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 08:40:21.000000 CVAugmentor-1.0.0/CVAugmentor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-30 08:40:21.000000 CVAugmentor-1.0.0/CVAugmentor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1108 2023-04-29 06:37:13.000000 CVAugmentor-1.0.0/LICENCE
--rw-rw-rw-   0        0        0     3176 2023-04-30 08:40:21.914449 CVAugmentor-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2621 2023-04-30 08:30:19.000000 CVAugmentor-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-30 08:40:21.916447 CVAugmentor-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1024 2023-04-30 08:37:59.000000 CVAugmentor-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:56:52.000057 CVAugmentor-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-04-30 08:56:51.954043 CVAugmentor-1.0.1/CVAugmentor/
+-rw-rw-rw-   0        0        0      498 2023-04-30 08:40:00.000000 CVAugmentor-1.0.1/CVAugmentor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:56:51.981043 CVAugmentor-1.0.1/CVAugmentor/assets/
+-rw-rw-rw-   0        0        0      317 2023-04-29 05:52:52.000000 CVAugmentor-1.0.1/CVAugmentor/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:56:51.991044 CVAugmentor-1.0.1/CVAugmentor/assets/main/
+-rw-rw-rw-   0        0        0      178 2023-04-29 05:52:49.000000 CVAugmentor-1.0.1/CVAugmentor/assets/main/__init__.py
+-rw-rw-rw-   0        0        0    26982 2023-04-29 09:27:03.000000 CVAugmentor-1.0.1/CVAugmentor/assets/main/augmentations_class.py
+-rw-rw-rw-   0        0        0     3519 2023-04-27 08:22:59.000000 CVAugmentor-1.0.1/CVAugmentor/assets/main/image_augmentor_class.py
+-rw-rw-rw-   0        0        0     6805 2023-04-27 08:38:31.000000 CVAugmentor-1.0.1/CVAugmentor/assets/main/video_augmentor_class.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:56:51.997041 CVAugmentor-1.0.1/CVAugmentor/assets/utils/
+-rw-rw-rw-   0        0        0      143 2023-04-29 05:59:11.000000 CVAugmentor-1.0.1/CVAugmentor/assets/utils/__init__.py
+-rw-rw-rw-   0        0        0      858 2023-03-26 09:42:33.000000 CVAugmentor-1.0.1/CVAugmentor/assets/utils/alphanumeric_sorter_class.py
+-rw-rw-rw-   0        0        0     1210 2023-04-27 07:28:18.000000 CVAugmentor-1.0.1/CVAugmentor/assets/utils/file_type_checker_class.py
+-rw-rw-rw-   0        0        0     6776 2023-04-29 08:09:44.000000 CVAugmentor-1.0.1/CVAugmentor/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:56:51.979043 CVAugmentor-1.0.1/CVAugmentor.egg-info/
+-rw-rw-rw-   0        0        0     3307 2023-04-30 08:56:50.000000 CVAugmentor-1.0.1/CVAugmentor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      569 2023-04-30 08:56:51.000000 CVAugmentor-1.0.1/CVAugmentor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 08:56:50.000000 CVAugmentor-1.0.1/CVAugmentor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-30 08:56:51.000000 CVAugmentor-1.0.1/CVAugmentor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1108 2023-04-29 06:37:13.000000 CVAugmentor-1.0.1/LICENCE
+-rw-rw-rw-   0        0        0     3307 2023-04-30 08:56:51.999044 CVAugmentor-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2731 2023-04-30 08:54:03.000000 CVAugmentor-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 08:56:52.000057 CVAugmentor-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1024 2023-04-30 08:56:22.000000 CVAugmentor-1.0.1/setup.py
```

### Comparing `CVAugmentor-1.0.0/CVAugmentor/assets/main/augmentations_class.py` & `CVAugmentor-1.0.1/CVAugmentor/assets/main/augmentations_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.0/CVAugmentor/assets/main/image_augmentor_class.py` & `CVAugmentor-1.0.1/CVAugmentor/assets/main/image_augmentor_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.0/CVAugmentor/assets/main/video_augmentor_class.py` & `CVAugmentor-1.0.1/CVAugmentor/assets/main/video_augmentor_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.0/CVAugmentor/assets/utils/alphanumeric_sorter_class.py` & `CVAugmentor-1.0.1/CVAugmentor/assets/utils/alphanumeric_sorter_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.0/CVAugmentor/assets/utils/file_type_checker_class.py` & `CVAugmentor-1.0.1/CVAugmentor/assets/utils/file_type_checker_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.0/CVAugmentor/pipeline.py` & `CVAugmentor-1.0.1/CVAugmentor/pipeline.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.0/CVAugmentor.egg-info/PKG-INFO` & `CVAugmentor-1.0.1/CVAugmentor.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: CVAugmentor
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for augmenting images and videos for computer vision tasks
 Home-page: https://github.com/AliKHaliliT/CVAugmentor
 Author: Ali Khalili Tazehkandgheshlagh
 Author-email: ali.khalili.t98@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
@@ -34,14 +35,15 @@
     negative,
 ## Installation
 You can install the package using pip:
 ```bash
 pip install CVAugmentor
 ```
 ## Usage
+For a detailed usage guide, please refer to the [documentation](https://alikhalilit.github.io/CVAugmentor/).
 ### Single Image Augmentation
 ```python
 # Importing the libraries
 from CVAugmentor import Augmentations as aug
 from CVAugmentor import Pipeline
 
 
@@ -112,7 +114,8 @@
 p = Pipeline()
 
 # Augment the videos
 p.augment(input_path="path/to/input_videos", output_path="path/to/output_videos", target="video", type="batch", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
 ```
 ## License
 This work is licensed under an [MIT](https://choosealicense.com/licenses/mit/) License.
+
```

### Comparing `CVAugmentor-1.0.0/CVAugmentor.egg-info/SOURCES.txt` & `CVAugmentor-1.0.1/CVAugmentor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.0/LICENCE` & `CVAugmentor-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.0/PKG-INFO` & `CVAugmentor-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: CVAugmentor
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for augmenting images and videos for computer vision tasks
 Home-page: https://github.com/AliKHaliliT/CVAugmentor
 Author: Ali Khalili Tazehkandgheshlagh
 Author-email: ali.khalili.t98@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
@@ -34,14 +35,15 @@
     negative,
 ## Installation
 You can install the package using pip:
 ```bash
 pip install CVAugmentor
 ```
 ## Usage
+For a detailed usage guide, please refer to the [documentation](https://alikhalilit.github.io/CVAugmentor/).
 ### Single Image Augmentation
 ```python
 # Importing the libraries
 from CVAugmentor import Augmentations as aug
 from CVAugmentor import Pipeline
 
 
@@ -112,7 +114,8 @@
 p = Pipeline()
 
 # Augment the videos
 p.augment(input_path="path/to/input_videos", output_path="path/to/output_videos", target="video", type="batch", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
 ```
 ## License
 This work is licensed under an [MIT](https://choosealicense.com/licenses/mit/) License.
+
```

### Comparing `CVAugmentor-1.0.0/README.md` & `CVAugmentor-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     negative,
 ## Installation
 You can install the package using pip:
 ```bash
 pip install CVAugmentor
 ```
 ## Usage
+For a detailed usage guide, please refer to the [documentation](https://alikhalilit.github.io/CVAugmentor/).
 ### Single Image Augmentation
 ```python
 # Importing the libraries
 from CVAugmentor import Augmentations as aug
 from CVAugmentor import Pipeline
```

### Comparing `CVAugmentor-1.0.0/setup.py` & `CVAugmentor-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def readme():
     with open('README.md') as f:
         return f.read()
     
 
 # Defining the setup function
 setup(name='CVAugmentor',
-        version='1.0.0',
+        version='1.0.1',
         description='A package for augmenting images and videos for computer vision tasks',
         long_description=readme(),
         long_description_content_type='text/markdown',
         url='https://github.com/AliKHaliliT/CVAugmentor',
         author='Ali Khalili Tazehkandgheshlagh',
         author_email='ali.khalili.t98@gmail.com',
         license='MIT',
```

