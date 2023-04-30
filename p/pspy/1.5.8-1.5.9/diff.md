# Comparing `tmp/pspy-1.5.8.tar.gz` & `tmp/pspy-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pspy-1.5.8.tar", last modified: Thu Jul 28 13:54:22 2022, max compression
+gzip compressed data, was "pspy-1.5.9.tar", last modified: Mon Aug  8 10:05:24 2022, max compression
```

## Comparing `pspy-1.5.8.tar` & `pspy-1.5.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 13:54:22.354007 pspy-1.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-07-28 13:54:15.000000 pspy-1.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-07-28 13:54:15.000000 pspy-1.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4389 2022-07-28 13:54:22.354007 pspy-1.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3059 2022-07-28 13:54:15.000000 pspy-1.5.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 13:54:22.354007 pspy-1.5.8/pspy/
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-07-28 13:54:22.354007 pspy-1.5.8/pspy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 13:54:22.338004 pspy-1.5.8/pspy/cov_fortran/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/cov_fortran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13837 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/cov_fortran/cov_fortran.f90
--rw-r--r--   0 runner    (1001) docker     (121)     7612 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/flat_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 13:54:22.338004 pspy-1.5.8/pspy/mcm_fortran/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/mcm_fortran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11471 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/mcm_fortran/mcm_fortran.f90
--rw-r--r--   0 runner    (1001) docker     (121)    10991 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/pspy_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/so_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     7662 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/so_consistency.py
--rw-r--r--   0 runner    (1001) docker     (121)    33139 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/so_cov.py
--rw-r--r--   0 runner    (1001) docker     (121)     2430 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/so_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)    31552 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/so_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     4392 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/so_map_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)    17469 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/so_mcm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/so_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4785 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/so_mpi.py
--rw-r--r--   0 runner    (1001) docker     (121)    11347 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/so_spectra.py
--rw-r--r--   0 runner    (1001) docker     (121)     5831 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/so_window.py
--rw-r--r--   0 runner    (1001) docker     (121)     6885 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/sph_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 13:54:22.338004 pspy-1.5.8/pspy/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 13:54:22.338004 pspy-1.5.8/pspy/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)   468866 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat
--rw-r--r--   0 runner    (1001) docker     (121)     4807 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/tests/data/generate_test_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/tests/data/parameters_test_data.yml
--rw-r--r--   0 runner    (1001) docker     (121) 12059025 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/tests/data/test_data.pkl
--rw-r--r--   0 runner    (1001) docker     (121)     4115 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/tests/test_pspy_namaster.py
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/tests/test_so_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     3987 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/tests/test_so_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/tests/test_so_spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 13:54:22.354007 pspy-1.5.8/pspy/wigner3j/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/wigner3j/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)   104274 2022-07-28 13:54:15.000000 pspy-1.5.8/pspy/wigner3j/wigner3j_sub.f
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 13:54:22.338004 pspy-1.5.8/pspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4389 2022-07-28 13:54:22.000000 pspy-1.5.8/pspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-07-28 13:54:22.000000 pspy-1.5.8/pspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-28 13:54:22.000000 pspy-1.5.8/pspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-07-28 13:54:22.000000 pspy-1.5.8/pspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-07-28 13:54:22.000000 pspy-1.5.8/pspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 13:54:22.354007 pspy-1.5.8/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)      222 2022-07-28 13:54:15.000000 pspy-1.5.8/scripts/test-pspy
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-07-28 13:54:22.354007 pspy-1.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-07-28 13:54:15.000000 pspy-1.5.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-07-28 13:54:15.000000 pspy-1.5.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 10:05:24.684031 pspy-1.5.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-08-08 10:05:18.000000 pspy-1.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-08-08 10:05:18.000000 pspy-1.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4389 2022-08-08 10:05:24.684031 pspy-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3059 2022-08-08 10:05:18.000000 pspy-1.5.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 10:05:24.684031 pspy-1.5.9/pspy/
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-08-08 10:05:24.684031 pspy-1.5.9/pspy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 10:05:24.668031 pspy-1.5.9/pspy/cov_fortran/
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/cov_fortran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13837 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/cov_fortran/cov_fortran.f90
+-rw-r--r--   0 runner    (1001) docker     (121)     7612 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/flat_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 10:05:24.672031 pspy-1.5.9/pspy/mcm_fortran/
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/mcm_fortran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11471 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/mcm_fortran/mcm_fortran.f90
+-rw-r--r--   0 runner    (1001) docker     (121)    10991 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/pspy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      973 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7662 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31992 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_cov.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2430 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_dict.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31552 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4392 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_map_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17469 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_mcm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4785 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11347 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5831 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_window.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6885 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/sph_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 10:05:24.672031 pspy-1.5.9/pspy/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 10:05:24.672031 pspy-1.5.9/pspy/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)   468866 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     4807 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/tests/data/generate_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/tests/data/parameters_test_data.yml
+-rw-r--r--   0 runner    (1001) docker     (121) 12059025 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/tests/data/test_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (121)     4115 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/tests/test_pspy_namaster.py
+-rw-r--r--   0 runner    (1001) docker     (121)      831 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/tests/test_so_dict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3987 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/tests/test_so_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/tests/test_so_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 10:05:24.684031 pspy-1.5.9/pspy/wigner3j/
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/wigner3j/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)   104274 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/wigner3j/wigner3j_sub.f
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 10:05:24.668031 pspy-1.5.9/pspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4389 2022-08-08 10:05:24.000000 pspy-1.5.9/pspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      979 2022-08-08 10:05:24.000000 pspy-1.5.9/pspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-08 10:05:24.000000 pspy-1.5.9/pspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-08-08 10:05:24.000000 pspy-1.5.9/pspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-08 10:05:24.000000 pspy-1.5.9/pspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 10:05:24.684031 pspy-1.5.9/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      222 2022-08-08 10:05:18.000000 pspy-1.5.9/scripts/test-pspy
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2022-08-08 10:05:24.684031 pspy-1.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-08-08 10:05:18.000000 pspy-1.5.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-08-08 10:05:18.000000 pspy-1.5.9/versioneer.py
```

### Comparing `pspy-1.5.8/LICENSE` & `pspy-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/PKG-INFO` & `pspy-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pspy
-Version: 1.5.8
+Version: 1.5.9
 Summary: Python power spectrum code
 Home-page: https://github.com/simonsobs/pspy
 Author: Simons Observatory Collaboration Power Spectrum Task Force
 License: BSD license
 Description: ====
         pspy
         ====
```

### Comparing `pspy-1.5.8/README.rst` & `pspy-1.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/cov_fortran/cov_fortran.f90` & `pspy-1.5.9/pspy/cov_fortran/cov_fortran.f90`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/flat_tools.py` & `pspy-1.5.9/pspy/flat_tools.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/mcm_fortran/mcm_fortran.f90` & `pspy-1.5.9/pspy/mcm_fortran/mcm_fortran.f90`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/pspy_utils.py` & `pspy-1.5.9/pspy/pspy_utils.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/so_config.py` & `pspy-1.5.9/pspy/so_config.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/so_consistency.py` & `pspy-1.5.9/pspy/so_consistency.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/so_cov.py` & `pspy-1.5.9/pspy/so_cov.py`

 * *Files 14% similar despite different names*

```diff
@@ -616,64 +616,39 @@
 
     Parameters
     ----------
 
     mbb_inv: 2d array
       the inverse spin0 and 2 mode coupling matrix
     """
-
-    mbb_inv_array = so_mcm.coupling_dict_to_array(mbb_inv)
-    mbb_array = np.linalg.inv(mbb_inv_array)
-    nbins = int(mbb_array.shape[0] / 9)
-    
-    mbb_array_select = np.zeros((4*nbins, 4*nbins))
+    nbins = mbb_inv["spin0xspin0"].shape[0]
+    mbb_inv_array = np.zeros((4*nbins, 4*nbins))
     # TT
-    mbb_array_select[0*nbins:1*nbins, 0*nbins:1*nbins] = mbb_array[0*nbins:1*nbins, 0*nbins:1*nbins]
+    mbb_inv_array[0*nbins:1*nbins, 0*nbins:1*nbins] = mbb_inv["spin0xspin0"]
     # TE
-    mbb_array_select[1*nbins:2*nbins, 1*nbins:2*nbins] = mbb_array[1*nbins:2*nbins, 1*nbins:2*nbins]
+    mbb_inv_array[1*nbins:2*nbins, 1*nbins:2*nbins] = mbb_inv["spin0xspin2"]
     # ET
-    mbb_array_select[2*nbins:3*nbins, 2*nbins:3*nbins] = mbb_array[3*nbins:4*nbins, 3*nbins:4*nbins]
+    mbb_inv_array[2*nbins:3*nbins, 2*nbins:3*nbins] = mbb_inv["spin2xspin0"]
     # EE
-    mbb_array_select[3*nbins:4*nbins, 3*nbins:4*nbins] = mbb_array[5*nbins:6*nbins, 5*nbins:6*nbins]
+    mbb_inv_array[3*nbins:4*nbins, 3*nbins:4*nbins] = mbb_inv["spin2xspin2"][0:nbins, 0:nbins]
 
-    mbb_inv_array = np.linalg.inv(mbb_array_select)
     
     return mbb_inv_array
 
 def extract_EEEBBB_mbb(mbb_inv):
     """this routine extract the E and B part of the mode coupling matrix
 
     Parameters
     ----------
 
     mbb_inv: 2d array
         the inverse spin0 and 2 mode coupling matrix
     """
 
-    mbb_inv_array = so_mcm.coupling_dict_to_array(mbb_inv)
-    mbb_array = np.linalg.inv(mbb_inv_array)
-    nbins = int(mbb_array.shape[0] / 9)
-
-    mbb_array_select = np.zeros((4*nbins, 4*nbins))
-    # EE
-    mbb_array_select[0*nbins:1*nbins, 0*nbins:1*nbins] = mbb_array[5*nbins:6*nbins, 5*nbins:6*nbins]
-    # EB
-    mbb_array_select[1*nbins:2*nbins, 1*nbins:2*nbins] = mbb_array[6*nbins:7*nbins, 6*nbins:7*nbins]
-    # BE
-    mbb_array_select[2*nbins:3*nbins, 2*nbins:3*nbins] = mbb_array[7*nbins:8*nbins, 7*nbins:8*nbins]
-    # BB
-    mbb_array_select[3*nbins:4*nbins, 3*nbins:4*nbins] = mbb_array[8*nbins:9*nbins, 8*nbins:9*nbins]
-    # EE-BB
-    mbb_array_select[0*nbins:1*nbins, 3*nbins:4*nbins] = mbb_array[5*nbins:6*nbins, 8*nbins:9*nbins]
-    # BB-EE
-    mbb_array_select[3*nbins:4*nbins, 0*nbins:1*nbins] = mbb_array[8*nbins:9*nbins, 5*nbins:6*nbins]
-
-    mbb_inv_array = np.linalg.inv(mbb_array_select)
-
-    return mbb_inv_array
+    return mbb_inv["spin2xspin2"]
 
 
 def cov2corr(cov, remove_diag=True):
     """Go from covariance to correlation matrix, also setting the diagonal to zero
 
     Parameters
     ----------
```

### Comparing `pspy-1.5.8/pspy/so_dict.py` & `pspy-1.5.9/pspy/so_dict.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/so_map.py` & `pspy-1.5.9/pspy/so_map.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/so_map_preprocessing.py` & `pspy-1.5.9/pspy/so_map_preprocessing.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/so_mcm.py` & `pspy-1.5.9/pspy/so_mcm.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/so_misc.py` & `pspy-1.5.9/pspy/so_misc.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/so_mpi.py` & `pspy-1.5.9/pspy/so_mpi.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/so_spectra.py` & `pspy-1.5.9/pspy/so_spectra.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/so_window.py` & `pspy-1.5.9/pspy/so_window.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/sph_tools.py` & `pspy-1.5.9/pspy/sph_tools.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat` & `pspy-1.5.9/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/tests/data/generate_test_data.py` & `pspy-1.5.9/pspy/tests/data/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/tests/data/test_data.pkl` & `pspy-1.5.9/pspy/tests/data/test_data.pkl`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/tests/test_pspy_namaster.py` & `pspy-1.5.9/pspy/tests/test_pspy_namaster.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/tests/test_so_dict.py` & `pspy-1.5.9/pspy/tests/test_so_dict.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/tests/test_so_map.py` & `pspy-1.5.9/pspy/tests/test_so_map.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/tests/test_so_spectra.py` & `pspy-1.5.9/pspy/tests/test_so_spectra.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy/wigner3j/wigner3j_sub.f` & `pspy-1.5.9/pspy/wigner3j/wigner3j_sub.f`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/pspy.egg-info/PKG-INFO` & `pspy-1.5.9/pspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pspy
-Version: 1.5.8
+Version: 1.5.9
 Summary: Python power spectrum code
 Home-page: https://github.com/simonsobs/pspy
 Author: Simons Observatory Collaboration Power Spectrum Task Force
 License: BSD license
 Description: ====
         pspy
         ====
```

### Comparing `pspy-1.5.8/pspy.egg-info/SOURCES.txt` & `pspy-1.5.9/pspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/setup.py` & `pspy-1.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.8/versioneer.py` & `pspy-1.5.9/versioneer.py`

 * *Files identical despite different names*

