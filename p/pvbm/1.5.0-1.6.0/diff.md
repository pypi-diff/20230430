# Comparing `tmp/pvbm-1.5.0.tar.gz` & `tmp/pvbm-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvbm-1.5.0.tar", last modified: Sun Apr 30 12:36:42 2023, max compression
+gzip compressed data, was "pvbm-1.6.0.tar", last modified: Sun Apr 30 14:00:18 2023, max compression
```

## Comparing `pvbm-1.5.0.tar` & `pvbm-1.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-04-30 12:36:42.038719 pvbm-1.5.0/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     1255 2023-04-30 12:36:42.038603 pvbm-1.5.0/PKG-INFO
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      993 2023-04-30 12:32:11.000000 pvbm-1.5.0/README.md
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-04-30 12:36:42.038427 pvbm-1.5.0/pvbm.egg-info/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     1255 2023-04-30 12:36:42.000000 pvbm-1.5.0/pvbm.egg-info/PKG-INFO
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      157 2023-04-30 12:36:42.000000 pvbm-1.5.0/pvbm.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-04-30 12:36:42.000000 pvbm-1.5.0/pvbm.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-04-30 12:36:42.000000 pvbm-1.5.0/pvbm.egg-info/requires.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-04-30 12:36:42.000000 pvbm-1.5.0/pvbm.egg-info/top_level.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-04-30 12:36:42.038759 pvbm-1.5.0/setup.cfg
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-04-30 12:36:32.000000 pvbm-1.5.0/setup.py
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-04-30 14:00:18.127006 pvbm-1.6.0/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     1269 2023-04-30 14:00:18.126888 pvbm-1.6.0/PKG-INFO
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     1007 2023-04-30 13:59:40.000000 pvbm-1.6.0/README.md
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-04-30 14:00:18.126704 pvbm-1.6.0/pvbm.egg-info/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     1269 2023-04-30 14:00:18.000000 pvbm-1.6.0/pvbm.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      157 2023-04-30 14:00:18.000000 pvbm-1.6.0/pvbm.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-04-30 14:00:18.000000 pvbm-1.6.0/pvbm.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-04-30 14:00:18.000000 pvbm-1.6.0/pvbm.egg-info/requires.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-04-30 14:00:18.000000 pvbm-1.6.0/pvbm.egg-info/top_level.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-04-30 14:00:18.127042 pvbm-1.6.0/setup.cfg
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-04-30 14:00:02.000000 pvbm-1.6.0/setup.py
```

### Comparing `pvbm-1.5.0/PKG-INFO` & `pvbm-1.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pvbm
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python Vasculature Biomarker toolbox
 Home-page: https://github.com/aim-lab/PVBM
 Author: Jonathan Fhima, Yevgeniy Men
 Author-email: jonathanfh@campus.technion.ac.il
 Description-Content-Type: text/markdown
 
 # Python Vasculature BioMarker toolbox documentation
 
-Based on the work published by Fhima, Jonathan, Jan Van Eijgen, Ingeborg Stalmans, Yevgeniy Men, Moti Freiman, and Joachim A. Behar. “PVBM: A Python Vasculature Biomarker Toolbox Based on Retinal Blood Vessel Segmentation.” In Computer Vision–ECCV 2022 Workshops: Tel Aviv, Israel, October 23–27, 2022, Proceedings, Part III, pp. 296-312. Cham: Springer Nature Switzerland, 2023 (https://link.springer.com/chapter/10.1007/978-3-031-25066-8_15).
+Official implementation, based on the work published by Fhima, Jonathan, Jan Van Eijgen, Ingeborg Stalmans, Yevgeniy Men, Moti Freiman, and Joachim A. Behar. “PVBM: A Python Vasculature Biomarker Toolbox Based on Retinal Blood Vessel Segmentation.” In Computer Vision–ECCV 2022 Workshops: Tel Aviv, Israel, October 23–27, 2022, Proceedings, Part III, pp. 296-312. Cham: Springer Nature Switzerland, 2023 (https://link.springer.com/chapter/10.1007/978-3-031-25066-8_15).
     
 ## Description
 
 Eleven biomarkers can be engineered, namely: the area, length, perimeter, number of endpoints, number of intersection points, median tortuosity, median branching angle, capacity dimension, entropy dimension, correlation dimension and singularity length.
 
 Installation
 
-Available on pip, with the command: pip install pvbm
+Available on pip. Run: "pip install pvbm"
 
 pip project: https://pypi.org/project/pvbm/
 
 read the docs: https://pvbm.readthedocs.io/en/latest/
 
 github: https://github.com/aim-lab/PVBM
```

### Comparing `pvbm-1.5.0/README.md` & `pvbm-1.6.0/pvbm.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,27 @@
+Metadata-Version: 2.1
+Name: pvbm
+Version: 1.6.0
+Summary: Python Vasculature Biomarker toolbox
+Home-page: https://github.com/aim-lab/PVBM
+Author: Jonathan Fhima, Yevgeniy Men
+Author-email: jonathanfh@campus.technion.ac.il
+Description-Content-Type: text/markdown
+
 # Python Vasculature BioMarker toolbox documentation
 
-Based on the work published by Fhima, Jonathan, Jan Van Eijgen, Ingeborg Stalmans, Yevgeniy Men, Moti Freiman, and Joachim A. Behar. “PVBM: A Python Vasculature Biomarker Toolbox Based on Retinal Blood Vessel Segmentation.” In Computer Vision–ECCV 2022 Workshops: Tel Aviv, Israel, October 23–27, 2022, Proceedings, Part III, pp. 296-312. Cham: Springer Nature Switzerland, 2023 (https://link.springer.com/chapter/10.1007/978-3-031-25066-8_15).
+Official implementation, based on the work published by Fhima, Jonathan, Jan Van Eijgen, Ingeborg Stalmans, Yevgeniy Men, Moti Freiman, and Joachim A. Behar. “PVBM: A Python Vasculature Biomarker Toolbox Based on Retinal Blood Vessel Segmentation.” In Computer Vision–ECCV 2022 Workshops: Tel Aviv, Israel, October 23–27, 2022, Proceedings, Part III, pp. 296-312. Cham: Springer Nature Switzerland, 2023 (https://link.springer.com/chapter/10.1007/978-3-031-25066-8_15).
     
 ## Description
 
 Eleven biomarkers can be engineered, namely: the area, length, perimeter, number of endpoints, number of intersection points, median tortuosity, median branching angle, capacity dimension, entropy dimension, correlation dimension and singularity length.
 
 Installation
 
-Available on pip, with the command: pip install pvbm
+Available on pip. Run: "pip install pvbm"
 
 pip project: https://pypi.org/project/pvbm/
 
 read the docs: https://pvbm.readthedocs.io/en/latest/
 
 github: https://github.com/aim-lab/PVBM
```

### Comparing `pvbm-1.5.0/pvbm.egg-info/PKG-INFO` & `pvbm-1.6.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,18 @@
-Metadata-Version: 2.1
-Name: pvbm
-Version: 1.5.0
-Summary: Python Vasculature Biomarker toolbox
-Home-page: https://github.com/aim-lab/PVBM
-Author: Jonathan Fhima, Yevgeniy Men
-Author-email: jonathanfh@campus.technion.ac.il
-Description-Content-Type: text/markdown
-
 # Python Vasculature BioMarker toolbox documentation
 
-Based on the work published by Fhima, Jonathan, Jan Van Eijgen, Ingeborg Stalmans, Yevgeniy Men, Moti Freiman, and Joachim A. Behar. “PVBM: A Python Vasculature Biomarker Toolbox Based on Retinal Blood Vessel Segmentation.” In Computer Vision–ECCV 2022 Workshops: Tel Aviv, Israel, October 23–27, 2022, Proceedings, Part III, pp. 296-312. Cham: Springer Nature Switzerland, 2023 (https://link.springer.com/chapter/10.1007/978-3-031-25066-8_15).
+Official implementation, based on the work published by Fhima, Jonathan, Jan Van Eijgen, Ingeborg Stalmans, Yevgeniy Men, Moti Freiman, and Joachim A. Behar. “PVBM: A Python Vasculature Biomarker Toolbox Based on Retinal Blood Vessel Segmentation.” In Computer Vision–ECCV 2022 Workshops: Tel Aviv, Israel, October 23–27, 2022, Proceedings, Part III, pp. 296-312. Cham: Springer Nature Switzerland, 2023 (https://link.springer.com/chapter/10.1007/978-3-031-25066-8_15).
     
 ## Description
 
 Eleven biomarkers can be engineered, namely: the area, length, perimeter, number of endpoints, number of intersection points, median tortuosity, median branching angle, capacity dimension, entropy dimension, correlation dimension and singularity length.
 
 Installation
 
-Available on pip, with the command: pip install pvbm
+Available on pip. Run: "pip install pvbm"
 
 pip project: https://pypi.org/project/pvbm/
 
 read the docs: https://pvbm.readthedocs.io/en/latest/
 
 github: https://github.com/aim-lab/PVBM
```

### Comparing `pvbm-1.5.0/setup.py` & `pvbm-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         return file.read()
 
 long_description = read_readme("README.md")
 
 
 setup(
     name='pvbm',
-    version='1.5.0',
+    version='1.6.0',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "scipy",
         "scikit-image",
         "pillow"
```

