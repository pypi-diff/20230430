# Comparing `tmp/CVAugmentor-0.0.1.tar.gz` & `tmp/CVAugmentor-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CVAugmentor-0.0.1.tar", last modified: Sat Apr 29 08:26:51 2023, max compression
+gzip compressed data, was "CVAugmentor-1.0.0.tar", last modified: Sun Apr 30 08:40:21 2023, max compression
```

## Comparing `CVAugmentor-0.0.1.tar` & `CVAugmentor-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 08:26:51.939247 CVAugmentor-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-04-29 08:26:51.630910 CVAugmentor-0.0.1/CVAugmentor/
--rw-rw-rw-   0        0        0      454 2023-04-29 08:09:39.000000 CVAugmentor-0.0.1/CVAugmentor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 08:26:51.651913 CVAugmentor-0.0.1/CVAugmentor/assets/
--rw-rw-rw-   0        0        0      317 2023-04-29 05:52:52.000000 CVAugmentor-0.0.1/CVAugmentor/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 08:26:51.670904 CVAugmentor-0.0.1/CVAugmentor/assets/main/
--rw-rw-rw-   0        0        0      178 2023-04-29 05:52:49.000000 CVAugmentor-0.0.1/CVAugmentor/assets/main/__init__.py
--rw-rw-rw-   0        0        0    26982 2023-04-29 06:24:52.000000 CVAugmentor-0.0.1/CVAugmentor/assets/main/augmentations_class.py
--rw-rw-rw-   0        0        0     3519 2023-04-27 08:22:59.000000 CVAugmentor-0.0.1/CVAugmentor/assets/main/image_augmentor_class.py
--rw-rw-rw-   0        0        0     6805 2023-04-27 08:38:31.000000 CVAugmentor-0.0.1/CVAugmentor/assets/main/video_augmentor_class.py
-drwxrwxrwx   0        0        0        0 2023-04-29 08:26:51.936294 CVAugmentor-0.0.1/CVAugmentor/assets/utils/
--rw-rw-rw-   0        0        0      143 2023-04-29 05:59:11.000000 CVAugmentor-0.0.1/CVAugmentor/assets/utils/__init__.py
--rw-rw-rw-   0        0        0      858 2023-03-26 09:42:33.000000 CVAugmentor-0.0.1/CVAugmentor/assets/utils/alphanumeric_sorter_class.py
--rw-rw-rw-   0        0        0     1210 2023-04-27 07:28:18.000000 CVAugmentor-0.0.1/CVAugmentor/assets/utils/file_type_checker_class.py
--rw-rw-rw-   0        0        0     6776 2023-04-29 08:09:44.000000 CVAugmentor-0.0.1/CVAugmentor/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-29 08:26:51.649906 CVAugmentor-0.0.1/CVAugmentor.egg-info/
--rw-rw-rw-   0        0        0     3136 2023-04-29 08:26:51.000000 CVAugmentor-0.0.1/CVAugmentor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      569 2023-04-29 08:26:51.000000 CVAugmentor-0.0.1/CVAugmentor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 08:26:51.000000 CVAugmentor-0.0.1/CVAugmentor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 08:26:51.000000 CVAugmentor-0.0.1/CVAugmentor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1108 2023-04-29 06:37:13.000000 CVAugmentor-0.0.1/LICENCE
--rw-rw-rw-   0        0        0     3136 2023-04-29 08:26:51.938228 CVAugmentor-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2581 2023-04-29 08:17:19.000000 CVAugmentor-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-29 08:26:51.939247 CVAugmentor-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1024 2023-04-29 08:26:41.000000 CVAugmentor-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:40:21.915469 CVAugmentor-1.0.0/
+drwxrwxrwx   0        0        0        0 2023-04-30 08:40:21.839448 CVAugmentor-1.0.0/CVAugmentor/
+-rw-rw-rw-   0        0        0      498 2023-04-30 08:40:00.000000 CVAugmentor-1.0.0/CVAugmentor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:40:21.864456 CVAugmentor-1.0.0/CVAugmentor/assets/
+-rw-rw-rw-   0        0        0      317 2023-04-29 05:52:52.000000 CVAugmentor-1.0.0/CVAugmentor/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:40:21.905453 CVAugmentor-1.0.0/CVAugmentor/assets/main/
+-rw-rw-rw-   0        0        0      178 2023-04-29 05:52:49.000000 CVAugmentor-1.0.0/CVAugmentor/assets/main/__init__.py
+-rw-rw-rw-   0        0        0    26982 2023-04-29 09:27:03.000000 CVAugmentor-1.0.0/CVAugmentor/assets/main/augmentations_class.py
+-rw-rw-rw-   0        0        0     3519 2023-04-27 08:22:59.000000 CVAugmentor-1.0.0/CVAugmentor/assets/main/image_augmentor_class.py
+-rw-rw-rw-   0        0        0     6805 2023-04-27 08:38:31.000000 CVAugmentor-1.0.0/CVAugmentor/assets/main/video_augmentor_class.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:40:21.912470 CVAugmentor-1.0.0/CVAugmentor/assets/utils/
+-rw-rw-rw-   0        0        0      143 2023-04-29 05:59:11.000000 CVAugmentor-1.0.0/CVAugmentor/assets/utils/__init__.py
+-rw-rw-rw-   0        0        0      858 2023-03-26 09:42:33.000000 CVAugmentor-1.0.0/CVAugmentor/assets/utils/alphanumeric_sorter_class.py
+-rw-rw-rw-   0        0        0     1210 2023-04-27 07:28:18.000000 CVAugmentor-1.0.0/CVAugmentor/assets/utils/file_type_checker_class.py
+-rw-rw-rw-   0        0        0     6776 2023-04-29 08:09:44.000000 CVAugmentor-1.0.0/CVAugmentor/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:40:21.860465 CVAugmentor-1.0.0/CVAugmentor.egg-info/
+-rw-rw-rw-   0        0        0     3176 2023-04-30 08:40:21.000000 CVAugmentor-1.0.0/CVAugmentor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      569 2023-04-30 08:40:21.000000 CVAugmentor-1.0.0/CVAugmentor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 08:40:21.000000 CVAugmentor-1.0.0/CVAugmentor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-30 08:40:21.000000 CVAugmentor-1.0.0/CVAugmentor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1108 2023-04-29 06:37:13.000000 CVAugmentor-1.0.0/LICENCE
+-rw-rw-rw-   0        0        0     3176 2023-04-30 08:40:21.914449 CVAugmentor-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2621 2023-04-30 08:30:19.000000 CVAugmentor-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 08:40:21.916447 CVAugmentor-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1024 2023-04-30 08:37:59.000000 CVAugmentor-1.0.0/setup.py
```

### Comparing `CVAugmentor-0.0.1/CVAugmentor/assets/main/augmentations_class.py` & `CVAugmentor-1.0.0/CVAugmentor/assets/main/augmentations_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-0.0.1/CVAugmentor/assets/main/image_augmentor_class.py` & `CVAugmentor-1.0.0/CVAugmentor/assets/main/image_augmentor_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-0.0.1/CVAugmentor/assets/main/video_augmentor_class.py` & `CVAugmentor-1.0.0/CVAugmentor/assets/main/video_augmentor_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-0.0.1/CVAugmentor/assets/utils/alphanumeric_sorter_class.py` & `CVAugmentor-1.0.0/CVAugmentor/assets/utils/alphanumeric_sorter_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-0.0.1/CVAugmentor/assets/utils/file_type_checker_class.py` & `CVAugmentor-1.0.0/CVAugmentor/assets/utils/file_type_checker_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-0.0.1/CVAugmentor/pipeline.py` & `CVAugmentor-1.0.0/CVAugmentor/pipeline.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-0.0.1/CVAugmentor.egg-info/PKG-INFO` & `CVAugmentor-1.0.0/CVAugmentor.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CVAugmentor
-Version: 0.0.1
+Version: 1.0.0
 Summary: A package for augmenting images and videos for computer vision tasks
 Home-page: https://github.com/AliKHaliliT/CVAugmentor
 Author: Ali Khalili Tazehkandgheshlagh
 Author-email: ali.khalili.t98@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -29,14 +29,15 @@
     brightness,
     exposure,
     blur,
     noise,
     cutout,
     negative,
 ## Installation
+You can install the package using pip:
 ```bash
 pip install CVAugmentor
 ```
 ## Usage
 ### Single Image Augmentation
 ```python
 # Importing the libraries
```

### Comparing `CVAugmentor-0.0.1/CVAugmentor.egg-info/SOURCES.txt` & `CVAugmentor-1.0.0/CVAugmentor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CVAugmentor-0.0.1/LICENCE` & `CVAugmentor-1.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `CVAugmentor-0.0.1/PKG-INFO` & `CVAugmentor-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CVAugmentor
-Version: 0.0.1
+Version: 1.0.0
 Summary: A package for augmenting images and videos for computer vision tasks
 Home-page: https://github.com/AliKHaliliT/CVAugmentor
 Author: Ali Khalili Tazehkandgheshlagh
 Author-email: ali.khalili.t98@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -29,14 +29,15 @@
     brightness,
     exposure,
     blur,
     noise,
     cutout,
     negative,
 ## Installation
+You can install the package using pip:
 ```bash
 pip install CVAugmentor
 ```
 ## Usage
 ### Single Image Augmentation
 ```python
 # Importing the libraries
```

### Comparing `CVAugmentor-0.0.1/README.md` & `CVAugmentor-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     brightness,
     exposure,
     blur,
     noise,
     cutout,
     negative,
 ## Installation
+You can install the package using pip:
 ```bash
 pip install CVAugmentor
 ```
 ## Usage
 ### Single Image Augmentation
 ```python
 # Importing the libraries
```

### Comparing `CVAugmentor-0.0.1/setup.py` & `CVAugmentor-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def readme():
     with open('README.md') as f:
         return f.read()
     
 
 # Defining the setup function
 setup(name='CVAugmentor',
-        version='0.0.1',
+        version='1.0.0',
         description='A package for augmenting images and videos for computer vision tasks',
         long_description=readme(),
         long_description_content_type='text/markdown',
         url='https://github.com/AliKHaliliT/CVAugmentor',
         author='Ali Khalili Tazehkandgheshlagh',
         author_email='ali.khalili.t98@gmail.com',
         license='MIT',
```

