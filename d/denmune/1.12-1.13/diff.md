# Comparing `tmp/denmune-1.12.tar.gz` & `tmp/denmune-1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denmune-1.12.tar", last modified: Sat Apr 29 21:47:58 2023, max compression
+gzip compressed data, was "denmune-1.13.tar", last modified: Sat Apr 29 22:56:17 2023, max compression
```

## Comparing `denmune-1.12.tar` & `denmune-1.13.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 21:47:58.755907 denmune-1.12/
--rw-rw-rw-   0        0        0     1498 2021-12-31 23:30:13.000000 denmune-1.12/LICENSE
--rw-rw-rw-   0        0        0       47 2021-12-27 21:52:58.000000 denmune-1.12/MANIFEST.in
--rw-rw-rw-   0        0        0    31198 2023-04-29 21:47:58.756901 denmune-1.12/PKG-INFO
--rw-rw-rw-   0        0        0    30529 2023-04-29 21:17:35.000000 denmune-1.12/README.md
--rw-rw-rw-   0        0        0      108 2021-12-23 20:19:35.000000 denmune-1.12/pyproject.toml
--rw-rw-rw-   0        0        0      808 2023-04-29 21:47:58.763965 denmune-1.12/setup.cfg
--rw-rw-rw-   0        0        0      259 2023-04-29 21:18:51.000000 denmune-1.12/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 21:47:58.698902 denmune-1.12/src/
-drwxrwxrwx   0        0        0        0 2023-04-29 21:47:58.734903 denmune-1.12/src/denmune/
--rw-rw-rw-   0        0        0       28 2022-05-12 02:48:25.000000 denmune-1.12/src/denmune/__init__.py
--rw-rw-rw-   0        0        0    39275 2022-05-12 03:42:03.000000 denmune-1.12/src/denmune/denmune.py
-drwxrwxrwx   0        0        0        0 2023-04-29 21:47:58.752905 denmune-1.12/src/denmune.egg-info/
--rw-rw-rw-   0        0        0    31198 2023-04-29 21:47:58.000000 denmune-1.12/src/denmune.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-04-29 21:47:58.000000 denmune-1.12/src/denmune.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 21:47:58.000000 denmune-1.12/src/denmune.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-04-29 21:47:58.000000 denmune-1.12/src/denmune.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-29 21:47:58.000000 denmune-1.12/src/denmune.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 22:56:17.364383 denmune-1.13/
+-rw-rw-rw-   0        0        0     1498 2021-12-31 23:30:13.000000 denmune-1.13/LICENSE
+-rw-rw-rw-   0        0        0       47 2021-12-27 21:52:58.000000 denmune-1.13/MANIFEST.in
+-rw-rw-rw-   0        0        0    31198 2023-04-29 22:56:17.365388 denmune-1.13/PKG-INFO
+-rw-rw-rw-   0        0        0    30529 2023-04-29 21:17:35.000000 denmune-1.13/README.md
+-rw-rw-rw-   0        0        0      108 2021-12-23 20:19:35.000000 denmune-1.13/pyproject.toml
+-rw-rw-rw-   0        0        0      808 2023-04-29 22:56:17.368386 denmune-1.13/setup.cfg
+-rw-rw-rw-   0        0        0      255 2023-04-29 22:54:58.000000 denmune-1.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:56:17.276063 denmune-1.13/src/
+drwxrwxrwx   0        0        0        0 2023-04-29 22:56:17.311205 denmune-1.13/src/denmune/
+-rw-rw-rw-   0        0        0       28 2022-05-12 02:48:25.000000 denmune-1.13/src/denmune/__init__.py
+-rw-rw-rw-   0        0        0    39275 2022-05-12 03:42:03.000000 denmune-1.13/src/denmune/denmune.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:56:17.348239 denmune-1.13/src/denmune.egg-info/
+-rw-rw-rw-   0        0        0    31198 2023-04-29 22:56:17.000000 denmune-1.13/src/denmune.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-29 22:56:17.000000 denmune-1.13/src/denmune.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 22:56:17.000000 denmune-1.13/src/denmune.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2023-04-29 22:56:17.000000 denmune-1.13/src/denmune.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-29 22:56:17.000000 denmune-1.13/src/denmune.egg-info/top_level.txt
```

### Comparing `denmune-1.12/LICENSE` & `denmune-1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `denmune-1.12/PKG-INFO` & `denmune-1.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: denmune
-Version: 1.12
+Version: 1.13
 Summary: This is the package for DenMune Clustering Algorithm published in paper https://doi.org/10.1016/j.patcog.2020.107589
 Home-page: https://github.com/scikit-learn-contrib/denmune-clustering-algorithm
 Author: Dr. Mohamed Ali Abbas & Prof. Amin  Shoukry
 Author-email: mohamed.alyabbas@outlook.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DenMune: A density-peak clustering algorithm
 DenMune is a clustering algorithm that can find clusters of arbitrary size, shapes and densities in two-dimensions. Higher dimensions are first reduced to 2-D using the t-sne. The algorithm relies on a single parameter K (the number of nearest neighbors). The results show the superiority of the algorithm. Enjoy the simplicity but the power of DenMune.
```

### Comparing `denmune-1.12/README.md` & `denmune-1.13/README.md`

 * *Files identical despite different names*

### Comparing `denmune-1.12/setup.cfg` & `denmune-1.13/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 656e 6d75 6e65 0d0a 7665 7273   = denmune..vers
-00000020: 696f 6e20 3d20 312e 3132 0d0a 6175 7468  ion = 1.12..auth
+00000020: 696f 6e20 3d20 312e 3133 0d0a 6175 7468  ion = 1.13..auth
 00000030: 6f72 203d 2044 722e 204d 6f68 616d 6564  or = Dr. Mohamed
 00000040: 2041 6c69 2041 6262 6173 2026 2050 726f   Ali Abbas & Pro
 00000050: 662e 2041 6d69 6e20 2053 686f 756b 7279  f. Amin  Shoukry
 00000060: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000070: 206d 6f68 616d 6564 2e61 6c79 6162 6261   mohamed.alyabba
 00000080: 7340 6f75 746c 6f6f 6b2e 636f 6d0d 0a64  s@outlook.com..d
 00000090: 6573 6372 6970 7469 6f6e 203d 2054 6869  escription = Thi
@@ -39,13 +39,13 @@
 00000260: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
 00000270: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
 00000280: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
 00000290: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
 000002a0: 0a09 3d20 7372 630d 0a70 6163 6b61 6765  ..= src..package
 000002b0: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
 000002c0: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-000002d0: 2e36 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .6....[options.p
+000002d0: 2e38 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .8....[options.p
 000002e0: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
 000002f0: 6865 7265 203d 2073 7263 0d0a 0d0a 5b65  here = src....[e
 00000300: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
 00000310: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
 00000320: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `denmune-1.12/src/denmune/denmune.py` & `denmune-1.13/src/denmune/denmune.py`

 * *Files identical despite different names*

### Comparing `denmune-1.12/src/denmune.egg-info/PKG-INFO` & `denmune-1.13/src/denmune.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: denmune
-Version: 1.12
+Version: 1.13
 Summary: This is the package for DenMune Clustering Algorithm published in paper https://doi.org/10.1016/j.patcog.2020.107589
 Home-page: https://github.com/scikit-learn-contrib/denmune-clustering-algorithm
 Author: Dr. Mohamed Ali Abbas & Prof. Amin  Shoukry
 Author-email: mohamed.alyabbas@outlook.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DenMune: A density-peak clustering algorithm
 DenMune is a clustering algorithm that can find clusters of arbitrary size, shapes and densities in two-dimensions. Higher dimensions are first reduced to 2-D using the t-sne. The algorithm relies on a single parameter K (the number of nearest neighbors). The results show the superiority of the algorithm. Enjoy the simplicity but the power of DenMune.
```

