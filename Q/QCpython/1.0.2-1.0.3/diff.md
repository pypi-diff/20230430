# Comparing `tmp/QCpython-1.0.2.tar.gz` & `tmp/QCpython-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QCpython-1.0.2.tar", last modified: Thu Jan 26 06:23:39 2023, max compression
+gzip compressed data, was "QCpython-1.0.3.tar", last modified: Sun Apr 30 21:25:58 2023, max compression
```

## Comparing `QCpython-1.0.2.tar` & `QCpython-1.0.3.tar`

### file list

```diff
@@ -1,37 +1,98 @@
-drwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)        0 2023-01-26 06:23:39.285132 QCpython-1.0.2/
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)    31117 2023-01-26 06:23:39.283917 QCpython-1.0.2/PKG-INFO
-drwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)        0 2023-01-26 06:23:38.984804 QCpython-1.0.2/QCpy/
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)    40028 2023-01-26 05:22:46.000000 QCpython-1.0.2/QCpy/QuantumCircuit.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)    17873 2023-01-26 05:22:46.000000 QCpython-1.0.2/QCpy/QuantumGate.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)     1669 2023-01-26 05:22:46.000000 QCpython-1.0.2/QCpy/Qubit.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)    21189 2023-01-26 05:46:26.000000 QCpython-1.0.2/QCpy/Visualizer.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      136 2023-01-26 05:36:40.000000 QCpython-1.0.2/QCpy/__init__.py
-drwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)        0 2023-01-26 06:23:39.028205 QCpython-1.0.2/QCpython.egg-info/
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)    31117 2023-01-26 06:23:38.000000 QCpython-1.0.2/QCpython.egg-info/PKG-INFO
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      559 2023-01-26 06:23:38.000000 QCpython-1.0.2/QCpython.egg-info/SOURCES.txt
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)        1 2023-01-26 06:23:38.000000 QCpython-1.0.2/QCpython.egg-info/dependency_links.txt
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)        5 2023-01-26 06:23:38.000000 QCpython-1.0.2/QCpython.egg-info/top_level.txt
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)    30615 2023-01-26 06:23:23.000000 QCpython-1.0.2/README.md
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)       38 2023-01-26 06:23:39.286131 QCpython-1.0.2/setup.cfg
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      792 2023-01-26 06:23:34.000000 QCpython-1.0.2/setup.py
-drwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)        0 2023-01-26 06:23:39.264843 QCpython-1.0.2/test/
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      718 2023-01-26 05:49:31.000000 QCpython-1.0.2/test/test_01.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      864 2023-01-26 05:49:44.000000 QCpython-1.0.2/test/test_02.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      970 2023-01-26 05:49:54.000000 QCpython-1.0.2/test/test_03.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      678 2023-01-26 05:50:02.000000 QCpython-1.0.2/test/test_04.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      682 2023-01-26 05:50:10.000000 QCpython-1.0.2/test/test_05.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      699 2023-01-26 05:50:17.000000 QCpython-1.0.2/test/test_06.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      708 2023-01-26 05:50:23.000000 QCpython-1.0.2/test/test_07.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      870 2023-01-26 05:50:31.000000 QCpython-1.0.2/test/test_08.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      884 2023-01-26 05:50:43.000000 QCpython-1.0.2/test/test_09.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      972 2023-01-26 05:50:53.000000 QCpython-1.0.2/test/test_10.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      880 2023-01-26 05:51:01.000000 QCpython-1.0.2/test/test_11.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      678 2023-01-26 05:51:08.000000 QCpython-1.0.2/test/test_12.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      700 2023-01-26 05:51:15.000000 QCpython-1.0.2/test/test_13.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      868 2023-01-26 05:51:23.000000 QCpython-1.0.2/test/test_14.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      882 2023-01-26 05:51:32.000000 QCpython-1.0.2/test/test_15.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)     1132 2023-01-26 05:51:39.000000 QCpython-1.0.2/test/test_16.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      800 2023-01-26 05:51:46.000000 QCpython-1.0.2/test/test_17.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      823 2023-01-26 05:51:54.000000 QCpython-1.0.2/test/test_18.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      713 2023-01-26 05:52:01.000000 QCpython-1.0.2/test/test_19.py
--rwxrwxrwx   0 bfreeze   (1000) bfreeze   (1000)      721 2023-01-26 05:52:06.000000 QCpython-1.0.2/test/test_20.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.726928 QCpython-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-30 21:25:46.000000 QCpython-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    33292 2023-04-30 21:25:58.726928 QCpython-1.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.710928 QCpython-1.0.3/QCpy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.714928 QCpython-1.0.3/QCpy/CircuitDrawing/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/CircuitDrawing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/CircuitDrawing/circuitdrawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/CircuitDrawing/gateformatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/CircuitDrawing/quantumgatedraw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.714928 QCpython-1.0.3/QCpy/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.714928 QCpython-1.0.3/QCpy/Core/qmace/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/qmace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/qmace/qmace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/qmace/quantumcircuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41098 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/quantumcircuit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.714928 QCpython-1.0.3/QCpy/Core/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/tools/amplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/tools/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/tools/phaseangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/tools/probabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.714928 QCpython-1.0.3/QCpy/QuantumGate/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/QuantumGate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/QuantumGate/multiqubit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/QuantumGate/singlequbit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.714928 QCpython-1.0.3/QCpy/Visualizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Visualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Visualizer/blochsphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Visualizer/probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Visualizer/qsphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Visualizer/statevector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.718928 QCpython-1.0.3/QCpy/Visualizer/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Visualizer/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Visualizer/tools/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Visualizer/tools/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/qubit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.718928 QCpython-1.0.3/QCpython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33292 2023-04-30 21:25:58.000000 QCpython-1.0.3/QCpython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-30 21:25:58.000000 QCpython-1.0.3/QCpython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 21:25:58.000000 QCpython-1.0.3/QCpython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-30 21:25:58.000000 QCpython-1.0.3/QCpython.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-30 21:25:58.000000 QCpython-1.0.3/QCpython.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    32500 2023-04-30 21:25:46.000000 QCpython-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-30 21:25:58.726928 QCpython-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-30 21:25:46.000000 QCpython-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.718928 QCpython-1.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.722928 QCpython-1.0.3/test/quantumcircuit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_03.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_04.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_05.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_08.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_09.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_13.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_14.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_15.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_19.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_20.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.726928 QCpython-1.0.3/test/quantumgate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_02.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_03.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_04.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_05.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_06.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_07.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_08.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_09.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_13.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_14.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_15.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_17.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_18.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_19.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_20.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_21.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_22.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_23.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.726928 QCpython-1.0.3/test/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/visualizer/__init__.py
```

### Comparing `QCpython-1.0.2/PKG-INFO` & `QCpython-1.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,30 @@
-Metadata-Version: 2.1
-Name: QCpython
-Version: 1.0.2
-Summary: QCpy is a lightweight quantum circuit simulator and visualization of quantum computing.
-Home-page: https://github.com/QCpython/QCpy
-Author: Brennan Freeze, Paris Osuch, Aundre Barras, Soren Richenberg, Suzanne Rivoire
-Author-email: freezebrennan@gmail.com, osuch@sonoma.edu, barras@sonoma.edu, richenbe@sonoma.edu, rivoire@sonoma.edu
-Keywords: quantum computing,physics,visualization,quantum circuit
-Description-Content-Type: text/markdown
-
 # README.md
 
 # QCpy - A Quantum Computing Library for Python
 
 QCpy is an open source python library and collaborative project for flexible simulations and visualizations of quantum circuits. Designed by college students with students in mind, this library contains a powerful set of tools to teach computer scientists about the emerging discipline of quantum computing (QC).
 
+You can download the package using pip:
+
+```txt
+pip install QCpython
+```
+
 ## Recommended Resources on Quantum Computing:
 
 - [Microsoft’s Linear Algebra for Quantum Computing](https://learn.microsoft.com/en-us/azure/quantum/overview-algebra-for-quantum-computing)
 - [IBM’s Quantum Computing: a field guide](https://quantum-computing.ibm.com/composer/docs/iqx/guide/)
 - [Wikipedia: Quantum Computing](https://en.wikipedia.org/wiki/Quantum_computing)
 
 ---
 
 # Qubits
 
-> ## *class* QC.Qubit.`Qubit`(*initial_state=’z’*)
+> ## *class* QCpy.`Qubit`(*initial_state=’z’*)
 
 *Object representation of a qubit.*
 
 ### Parameters:
 
 `initial_state (chr)` - Character input for starting direction in the *x*, *y*, or *z* axis.
 
@@ -100,15 +96,15 @@
 `None`
 
 ### Attributes:
 
 `matrix (np.ndarray)` - matrix representation of Pauli-Z gate.
 
 ```python
-PauliY.matrix = [1+0j, 0+0j], 
+PauliZ.matrix = [1+0j, 0+0j], 
                 [0+0j, -1+0j]
 ```
 
 > ## *class* QC.QuantumGate.`Hadamard`()
 
 *Maps the basis states |0> to |+> and |1> to |->, creating a superposition state if given a computation basis state.*
 
@@ -456,15 +452,15 @@
 Cz.matrix = [1+0j, 0+0j, 0+0j, 0+0j],
             [0+0j, 1+0j, 0+0j, 0+0j],
             [0+0j, 0+0j, 1+0j, 0+0j],
             [0+0j, 0+0j, 0+0j, -1+0j]
 ```
 ---
 # Quantum Circuit
-> ## *class* QC.QuantumCircuit.`QuantumCircuit`(*qubits*, *little_endian=False*, *prep='z'*)
+> ## *class* QCpy.`QuantumCircuit`(*qubits*, *little_endian=False*, *prep='z'*)
 
 *Quantum circuit that represents the state of a quantum system and performs operations on select qubits.*
 
 ### Parameters:
 
 `qubits (int)` - number of qubits in the circuit.
 
@@ -595,14 +591,48 @@
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.   +0.j]
 # [0.707+0.j]]
 ```
 
+> ## QuantumCircuit.`circuitQueue()`
+
+*Returns queue of gates on quantum circuit.*
+
+### Parameters:
+
+`None`
+
+### Returns:
+`queue (list)` - list of gates queued on quantum circuit.
+
+### Example:
+
+```python
+from QCpy import QuantumCircuit
+
+qc = QuantumCircuit(4)
+
+qc.x(0)
+qc.x(1)
+qc.x(2)
+qc.rc3x(0, 1, 2, 3)
+
+print(qc.circuitQueue())
+
+# [('X', 0), ('X', 1), ('X', 2), ('U', 3), ('U', 3), ('cnot', 2, # 3), ('U', 3), ('U', 3), ('swap', 2, 3), ('swap', 1, 2), 
+# ('swap', 1, 2), ('swap', 2, 3), ('cnot', 0, 3), ('U', 3),
+# ('swap', 2, 3), ('swap', 2, 3), ('cnot', 1, 3), ('U', 3), 
+# ('swap', 2, 3), ('swap', 1, 2), ('swap', 1, 2), ('swap', 2, 
+# 3), ('cnot', 0, 3), ('U', 3), ('swap', 2, 3), ('swap', 2, 3),
+#  ('cnot', 1, 3), ('U', 3), ('U', 3), ('U', 3), ('cnot', 2, 3),
+#  ('U', 3), ('U', 3), ('rc3x', 0, 1, 2, 3)]
+```
+
 > ## QuantumCircuit.`probabilities`(*round=3*)
 
 *Returns probabilitiy of the qubits within the quantum circuit.*
 
 ### Parameters:
 
 `round (int)` - rounding the probabilities to the nearest `round`
@@ -1567,15 +1597,15 @@
 # [0.+0.j]]
 ```
 
 # Visualizer
 
 *A collection of classes to visualize the quantum circuit*
 
-> ## *class* QC.Visualizer.QSphere(*circuit*)
+> ## *class* QCpy.Visualizer.QSphere(*circuit*)
 
 *Visualizes the quantum circuit as a q-sphere*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
 
@@ -1612,15 +1642,64 @@
 qc.hadamard(0)
 qc.hadamard(1)
 qc.hadamard(2)
 
 sphere_ex = QSphere(qc)
 sphere_ex.makeSphere(save=False, show=True)
 ```
-> ## *class* QC.Visualizer.StateVector(*circuit*)
+
+> ## *class* QC.Visualizer.BlochSphere(*circuit*)
+
+*Visualizes the quantum state of a single qubit as a sphere*
+
+### Parameters:
+
+`circuit` - the quantum circuit
+
+### Attributes:
+
+`None`
+
+> ## BlochSphere.`makeSphere`(*show_bit=0*, *path="qsphere.png"*, *save=True*, *show=True*, *darkmode=True*)
+
+*Returns a Bloch Sphere that plots the quantum state of a single qubit in a 3D global view*
+
+### Parameters:
+
+`show_bit (int)` - the qubit on the circuit to be visualized, initialized as the 0th bit
+
+`path (str)` - name of the image to be saved
+
+`save (bool)` - pass True for the graph to be saved
+
+`show (bool)` - pass True for the sphere to be shown instead of saved
+
+`darkmode (bool)` - pass True for darkmode, false for lightmode
+
+### Returns:
+
+`None`
+
+### Example:
+
+```python
+from QCpy import QuantumCircuit
+from QCpy.Visualizer import *
+
+qc = QuantumCircuit(3)
+
+qc.hadamard(0)
+qc.hadamard(1)
+qc.hadamard(2)
+
+sphere_ex = BlochSphere(qc)
+sphere_ex.makeSphere(show_bit=1, save=False, show=True)
+```
+
+> ## *class* QCpy.Visualizer.StateVector(*circuit*)
 
 *Visualizes the quantum circuit's quantum amplitutes using a bar graph*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
 
@@ -1658,15 +1737,15 @@
 qc.hadamard(1)
 qc.hadamard(2)
 
 stateVector_ex = StateVector(qc)
 stateVector_ex.makeGraph(save=False, show=True)
 ```
 
-> ## *class* QC.Visualizer.Probabilities(*circuit*)
+> ## *class* QCpy.Visualizer.Probabilities(*circuit*)
 
 *Visualizes the quantum circuit's qubits probability of being measured using a bar graph*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
```

### Comparing `QCpython-1.0.2/QCpy/QuantumCircuit.py` & `QCpython-1.0.3/QCpy/Core/quantumcircuit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 QuantumCircuit.py
 """
-from .Qubit import Qubit
-from .QuantumGate import *
+from ..qubit import Qubit
+from ..QuantumGate import *
+from .tools import amplitude, phaseAngle, probabilities, measure
 import numpy as np
 
 """
 Purpose:
     To apply various quantum gates to a quantum wire given any amount of qubits. With this, to then return the state at any given moment
     alongside calculations to be examined upon.
 Methods:
     __init__:
         Constructor that initilizes the quantum state in a vector given the number of qubits, endian positioning, and prepping of the qubits.
     __operator_matrix__:
         Return a matrix from the tensor product calculation algorithm from any inplaced quantum gate.
     __controlled_phase_handler__:
-        Calls a control and target qubits represented as integers and will then correctly create a system of mathematic implementations of 
+        Calls a control_qubit and target_qubit qubits represented as integers and will then correctly create a system of mathematic implementations of
         any given controlled quantum gate.
     circuit:
         Returns the dictionary representation of the circuit and the values within it.
     amplitude:
         Return a vector of all possible amplitudes for the given state.
     phaseAngle:
         Calculates an array of possible phase angles based off the state. Converts each value using np.angle() function then degree to radian.
@@ -28,49 +29,49 @@
     probabilities:
         Return a matrix with all the probabilities for each state.
     measure:
         Collapes the quantum circuit into classical bits.
     reverse:
         Reverses the quantum state.
     toffoli:
-        A 3-qubit quantum gate that takes in two control qubits and one target qubit.
+        A 3-qubit quantum gate that takes in two control_qubit qubits and one target_qubit qubit.
     rccx:
-        A 3-qubit quantum gate that takes in two control qubits and one target qubit.
+        A 3-qubit quantum gate that takes in two control_qubit qubits and one target_qubit qubit.
     rc3x:
         A 4-qubit quantum gate that is a simplified Toffoli gate and can be used in placed where the Toffoli gate is uncomputed again.
     cnot:
-        A 2-qubit quantum gate that takes in control and target qubits, and will entangle the qubits if the control qubit is greater than 0.
+        A 2-qubit quantum gate that takes in control_qubit and target_qubit qubits, and will entangle the qubits if the control_qubit qubit is greater than 0.
     cr:
-        A 2-qubit quantum gate that takes in control and target qubits to perform calculations upon the state.
+        A 2-qubit quantum gate that takes in control_qubit and target_qubit qubits to perform calculations upon the state.
     cz:
-        A 2-qubit quantum gate that takes in control and target qubits to perform calculations upon the state.
+        A 2-qubit quantum gate that takes in control_qubit and target_qubit qubits to perform calculations upon the state.
     swap:
         A 2-qubit quantum gate that takes in two qubits to swap the qubits values they represent.
     rxx:
         A 2-qubit quantum gate that takes in two qubits and a representation of theta to initialize in the quantum state.
     rzz:
         A 2-qubit quantum gate that takes in two qubits and a representation of theta to initialize in the quantum state.
     customControlPhase:
-        Used to insert single qubit based quantum gates to have a control qubit apart of it and committing to the quantum state.
+        Used to insert single qubit based quantum gates to have a control_qubit qubit apart of it and committing to the quantum state.
     identity:
         Used to confirm value that a qubit is representing and does nothing to manipulate the value of such qubit.
     x:
         Used to invert the value of what a qubit is representing.
     hadamard:
         Used to put a given qubit into superposition.
     y:
         Changes the state of a qubit by pi around the y-axis of a Bloch Sphere.
     z:
         Changes the state of a qubit by pi around the z-axis of a Bloch Sphere.
     phase:
         Commits to a rotation around the z-axis based off of the inputted theta value.
     s:
-        Is a Phase gate where the inputted theta value is given as a constant of theta = pi / 2. 
+        Is a Phase gate where the inputted theta value is given as a constant of theta = pi / 2.
     sdg:
-        Is a Phase gate and inverse of the S gate where the inputted theta value is given as a constant of theta = -pi / 2. 
+        Is a Phase gate and inverse of the S gate where the inputted theta value is given as a constant of theta = -pi / 2.
     t:
         T gate is a special use case gate that in implemented from the P Gate.
     tdg:
         TDG gate is a special use case gate that in implemented from the P Gate and is the inverse of the T gate.
     rz:
         RZ gate commits a rotation around the z-axis for a qubit.
     ry:
@@ -85,778 +86,935 @@
         U gate is given three inputs (theta, phi, and lambda) that allow the inputs to manipulate the base matrix to allow for the position of the enacted qubit
         around the bloch sphere representation.
     custom:
         Will take in a custom single qubit quantum gate and implement it on a qubit.
 --------
 
 """
+
+
 class QuantumCircuit:
-    def __init__(self, qubits: int, little_endian: bool = False, prep: chr = 'z'):
+    def __init__(
+            self,
+            qubits: int,
+            little_endian: bool = False,
+            prep: chr = 'z'):
         """
         Constructor that initilizes the quantum state in a vector given the number of qubits, endian positioning, and prepping of the qubits.
         Args:
-            qubits: 
+            qubits:
                 The number of qubits that will be within the circuit.
             little_endian:
                 a boolean variable to determine the placement of values, as well as determining the inverse of tensor product.
             prep:
 
         ------
         Variables:
-            _little_endian : 
+            _little_endian :
                 the number of qubits on the circuit
             _circuit_size :
                 all the states of the qubits on the circuit
             _probabilities :
                 an array of all the probabilities of the qubits being measured
             _percents :
                 the array of probabilities turned into an array of values adding to 100
             _state :
                 the state values for the qubit being taken into consideration
         """
         if (qubits < 1):
-            exit(f"Error: QuantumCircuit().__init__ -- Quantum Circuit size must be 1 or more qubits. Current number of qubits is: {qubits}")
-        # Determines if tensor calculation of __operator_matrix__ will be reversed or not.
+            exit(
+                f"Error: QuantumCircuit().__init__ -- Quantum Circuit size must be 1 or more qubits. Current number of qubits is: {qubits}")
+        # Determines if tensor calculation of __operator_matrix__ will be
+        # reversed or not.
         self._little_endian = little_endian
         # Gets the number of qubits in play to store for later use.
         self._circuit_size = qubits
-        # Makes tensored vector state of all qubits, and stores it within _state to get a vector of [[1], [0], [0],....2^n].
+        # Makes tensored vector state of all qubits, and stores it within
+        # _state to get a vector of [[1], [0], [0],....2^n].
         self._state = Qubit(prep).state
         # represent the circuit in dict
-        self._circuit = {i:[] for i in range(qubits)}
-        # increases the current vector size on the number of qubits - 1. 
-        for _ in range(qubits-1):
-            # _state is converted into the new lengthed vector based on the kronocker product on the prepped qubit state.
+        self._circuit = []
+        # increases the current vector size on the number of qubits - 1.
+        for _ in range(qubits - 1):
+            # _state is converted into the new lengthed vector based on the
+            # kronocker product on the prepped qubit state.
             self._state = np.kron(self._state, Qubit(prep).state)
-    def __operator_matrix__(self, gate_matrix: np.array, qubit: int, double: bool = False):
+
+    def __operator_matrix__(
+            self,
+            gate_matrix: np.array,
+            qubit: int,
+            double: bool = False):
         """
         Return a matrix from the tensor product calculation algorithm from any inplaced quantum gate.
         Params:
             gate_matrix: np.array
             qubit: integer
             double: boolean
         Returns:
-            operator_matrix (numpy array): 
+            operator_matrix (numpy array):
                 Matrix after final calculation from the tensor product algorithm.
         """
         # Identity matrix is called.
         i_matrix = Identity().matrix
         # gate queue for the computation
         gate_queue = [i_matrix for _ in range(self._circuit_size)]
-        # replaces the placement of the identity gate at the qubit index with the gate to get a correct calculation of final product
+        # replaces the placement of the identity gate at the qubit index with
+        # the gate to get a correct calculation of final product
         gate_queue[qubit] = gate_matrix
-        # if double is true, then CNOT, toffli, or any gate more than one qubit is being asked to be implemented.
+        # if double is true, then CNOT, toffli, or any gate more than one qubit
+        # is being asked to be implemented.
         if double:
-            gate_queue.pop(qubit+1)
-        # if little_endian variable is true to follow IBM and Qiskit notation. Inverses queue of operation.
+            gate_queue.pop(qubit + 1)
+        # if little_endian variable is true to follow IBM and Qiskit notation.
+        # Inverses queue of operation.
         if (self._little_endian):
             gate_queue = gate_queue[::-1]
         # stores final value to be stored into operator_matrix value
         operator_matrix = gate_queue[0]
         # uses np.kron() function to tensor product the queue
         for gate in gate_queue[1:]:
             operator_matrix = np.kron(operator_matrix, gate)
 
         return operator_matrix
-    def __controlled_phase_handler__(self, gate_to_product: np.array, control: int, target: int):
+
+    def __controlled_phase_handler__(
+            self,
+            matrix_to_calculate: np.array,
+            control_qubit: int,
+            target_qubit: int):
         """
-        Calls a control and target qubits represented as integers and will then correctly create a system of mathematic implementations of 
-        any given controlled quantum gate. 
+        Calls a control_qubit and target_qubit represented as integers and will then correctly create a system of mathematic implementations of
+        any given controlled quantum gate.
         Params:
-            gate_to_product: np.array
-            control: integer
-            target: integer
+            matrix_to_calculate: np.array
+            control_qubit: integer
+            target_qubit: integer
         Returns:
             None.
         """
-        # inverse bool variable to determine if controlled gate representation needs to invert for confirming logic structuring.
+        # inverse bool variable to determine if controlled gate representation
+        # needs to invert for confirming logic structuring.
         inverse = False
-        # checking to see if target is less than control indices:
-        if(target < control):
+        # checking to see if target_qubit is less than control_qubit indices:
+        if (target_qubit < control_qubit):
             inverse = True
-        # create temp target variable
-        calculate_matrix = gate_to_product
-        temp_target = target
+        # create temp target_qubit variable
+        temp_target_qubit = target_qubit
         # call from QuantumGate and stores Hadamard gate into variable.
         hadamard = Hadamard().matrix
-        # If target and control qubits are next to each other, then no further logic needs to be done and calls base system.
-        if(abs(target - control) == 1):
-                # calls from called bool variable to see if the base CNOT matrix needs to be inverted to confirm correct logic structuring.
+        # If target_qubit and control_qubit qubits are next to each other, then no further
+        # logic needs to be done and calls base system.
+        if (abs(target_qubit - control_qubit) == 1):
+            # calls from called bool variable to see if the base CNOT matrix
+            # needs to be inverted to confirm correct logic structuring.
             if inverse:
-                # This is implemented due to other controlled gates not needing this implementation.
-                self._state = np.dot(self.__operator_matrix__(hadamard, temp_target), self._state)
-                self._state = np.dot(self.__operator_matrix__(hadamard, temp_target + 1), self._state)
-                # Call to _state to commit a dot product on the state to include the given gate of the method.
-                self._state = np.dot(self.__operator_matrix__(calculate_matrix, temp_target, double=True), self._state)
-                # This is implemented due to other controlled gates not needing this implementation.
-                    
-                self._state = np.dot(self.__operator_matrix__(hadamard, temp_target), self._state)
-                self._state = np.dot(self.__operator_matrix__(hadamard, temp_target + 1), self._state)
-                # used for inversing all other gates that the target is less than the control to make it inversed in logic.
+                # This is implemented due to other controlled gates not needing
+                # this implementation.
+                self._state = np.dot(
+                    self.__operator_matrix__(
+                        hadamard, temp_target_qubit), self._state)
+                self._state = np.dot(
+                    self.__operator_matrix__(
+                        hadamard, temp_target_qubit + 1), self._state)
+                # Call to _state to commit a dot product on the state to
+                # include the given gate of the method.
+                self._state = np.dot(
+                    self.__operator_matrix__(
+                        matrix_to_calculate,
+                        temp_target_qubit,
+                        double=True),
+                    self._state)
+                # This is implemented due to other controlled gates not needing
+                # this implementation.
+
+                self._state = np.dot(
+                    self.__operator_matrix__(
+                        hadamard, temp_target_qubit), self._state)
+                self._state = np.dot(
+                    self.__operator_matrix__(
+                        hadamard, temp_target_qubit + 1), self._state)
+                # used for inversing all other gates that the target_qubit is less
+                # than the control_qubit to make it inversed in logic.
             else:
-                # if not inverse, what the controlled gate is will be enacted on the _state using dot product system.
-                self._state = np.dot(self.__operator_matrix__(calculate_matrix, control, double=True), self._state)
+                # if not inverse, what the controlled gate is will be enacted
+                # on the _state using dot product system.
+                self._state = np.dot(
+                    self.__operator_matrix__(
+                        matrix_to_calculate,
+                        control_qubit,
+                        double=True),
+                    self._state)
             return
-        # while the difference between the temp target and control is not -1 or 1.
-        while(abs(temp_target - control) != 1):
-            # calls from called bool variable to see if the base CNOT matrix needs to be inverted to confirm correct logic structuring.
+        # while the difference between the temp target_qubit and control_qubit is not -1 or
+        # 1.
+        while (abs(temp_target_qubit - control_qubit) != 1):
+            # calls from called bool variable to see if the base CNOT matrix
+            # needs to be inverted to confirm correct logic structuring.
             if inverse:
-                # This is implemented due to other controlled gates not needing this implementation.
-                self.swap(temp_target, temp_target+1)
-                # update temp target position.
-                temp_target += 1
+                # This is implemented due to other controlled gates not needing
+                # this implementation.
+                self.swap(temp_target_qubit, temp_target_qubit + 1)
+                # update temp target_qubit position.
+                temp_target_qubit += 1
             else:
-                # swap the temp target closer to the target.
-                self.swap(temp_target-1, temp_target)
-                # update temp target position.
-                temp_target -= 1
-        # calls from called bool variable to see if the base CNOT matrix needs to be inverted to confirm correct logic structuring.
+                # swap the temp target_qubit closer to the target_qubit.
+                self.swap(temp_target_qubit - 1, temp_target_qubit)
+                # update temp target_qubit position.
+                temp_target_qubit -= 1
+        # calls from called bool variable to see if the base CNOT matrix needs
+        # to be inverted to confirm correct logic structuring.
         if inverse:
             # will create inversed controlled_phase of what is inputted through here, determined if the inversed variable is marked true.
-            # call hadamard gates on control and target variables.
-            self._state = np.dot(self.__operator_matrix__(hadamard, temp_target), self._state)
-            self._state = np.dot(self.__operator_matrix__(hadamard, temp_target + 1), self._state)
-            # Call to _state to commit a dot product on the state to include the given gate of the method.
-            self._state = np.dot(self.__operator_matrix__(calculate_matrix, temp_target, double=True), self._state)
-            # This is implemented due to other controlled gates not needing this implementation.
-            self._state = np.dot(self.__operator_matrix__(hadamard, temp_target), self._state)
-            self._state = np.dot(self.__operator_matrix__(hadamard, temp_target + 1), self._state)
-            # used for inversing all other gates that the target is less than the control to make it inversed in logic.
+            # call hadamard gates on control_qubit and target_qubit variables.
+            self._state = np.dot(
+                self.__operator_matrix__(
+                    hadamard, temp_target_qubit), self._state)
+            self._state = np.dot(
+                self.__operator_matrix__(
+                    hadamard,
+                    temp_target_qubit + 1),
+                self._state)
+            # Call to _state to commit a dot product on the state to include
+            # the given gate of the method.
+            self._state = np.dot(
+                self.__operator_matrix__(
+                    matrix_to_calculate,
+                    temp_target_qubit,
+                    double=True),
+                self._state)
+            # This is implemented due to other controlled gates not needing
+            # this implementation.
+            self._state = np.dot(
+                self.__operator_matrix__(
+                    hadamard, temp_target_qubit),
+                self._state)
+            self._state = np.dot(
+                self.__operator_matrix__(
+                    hadamard,
+                    temp_target_qubit + 1),
+                self._state)
+            # used for inversing all other gates that the target_qubit is less than
+            # the control_qubit to make it inversed in logic.
         else:
-            # if not inverse, what the controlled gate is will be enacted on the _state using dot product system.
-            self._state = np.dot(self.__operator_matrix__(calculate_matrix, control, double=True), self._state)
+            # if not inverse, what the controlled gate is will be enacted on
+            # the _state using dot product system.
+            self._state = np.dot(
+                self.__operator_matrix__(
+                    matrix_to_calculate,
+                    control_qubit,
+                    double=True),
+                self._state)
 
-        # while the temp target does not equal the original target
-        while(temp_target != target):
+        # while the temp target_qubit does not equal the original target_qubit
+        while (temp_target_qubit != target_qubit):
             if inverse:
-                # swap the temp target with the position closer to original target
-                self.swap(temp_target-1, temp_target)
-                # update temp target position
-                temp_target -=1
+                # swap the temp target_qubit with the position closer to original
+                # target_qubit
+                self.swap(temp_target_qubit - 1, temp_target_qubit)
+                # update temp target_qubit position
+                temp_target_qubit -= 1
             else:
-                # swap the temp target with the position closer to original target
-                self.swap(temp_target, temp_target+1)
-                # update temp target position
-                temp_target +=1
+                # swap the temp target_qubit with the position closer to original
+                # target_qubit
+                self.swap(temp_target_qubit, temp_target_qubit + 1)
+                # update temp target_qubit position
+                temp_target_qubit += 1
+
+
+
     def circuit(self):
         """
         Returns the dictionary representation of the circuit and the values within it.
         Params:
             None.
         Returns:
             np.array self._circuit
         """
         return self._circuit
 
-    def amplitude(self, round: int = 3):
+    def amplitude(self, show_bit=-1, round: int = 3, radian: bool = False):
         """
         Return a vector of all possible amplitudes for the given state.
         Params:
-            round: int 
+            show_bit: string or int
+            round: int
+            radian: bool
         Returns:
-            np.around(statevector) (numpy array): 
+            np.around(statevector) (numpy array):
                 Matrix after final calculation from the sqrt(x^2 + y^2) algorithm for finding the amplitude.
         """
-        if (round < 0):
-            exit(f"Error: QuantumCircuit().amplitude -- round placement must be a value greater than 0.")
-        # initial array for return 
-        statevector = []
-        # for loop will go through this statement 2^n times for _state length
-        for i in range(len(self._state)):
-            #calculates sqrt(x^2 + y^2 for amplitude), x = real value, y = imaginary value
-            statevector.append(np.sqrt(np.power(self._state[i].real, 2) + np.power(self._state[i].imag, 2)))
-        # rounds value based off of parameter
-        return np.around(statevector, decimals = round)
-    def phaseAngle(self, round: int = 2, radian: bool = True):
+        return amplitude(self._state, self._circuit_size, show_bit, round, radian)
+
+    def phaseAngle(self, show_bit = -1, round: int = 3, radian: bool = True):
         """
         Calculates an array of possible phase angles based off the state. Converts each value using np.angle() function then degree to radian.
         Params:
+            show_bit: string or int
             round: int
             radian: bool
         Returns:
-            np.around(phaseAngles) (numpy array): 
-                Matrix after final calculation from the  phase angle algorithm.
+            np.around(phaseAngles) (numpy array):
+                Matrix after final calculation from the phase angle algorithm.
         """
-        # if rounding value is less than 0, exits as this is improper.
-        if (round < 0):
-            exit(f"Error: QuantumCircuit().phaseAngle -- round placement must be a value greater than 0.")
-        # 
-        temp = (np.mod(np.angle(self._state), 2*np.pi) * (180/np.pi))
-        if (radian):
-            temp *= (np.pi / 180)
-        return temp
+        return phaseAngle(self._state, self._circuit_size, show_bit, round, radian)
+
     def state(self, round: int = 3):
         """
         Return a numpy array of the current quantum circuit.
         Params:
-            round: int 
+            round: int
         Returns:
-            np.around(self._state) (numpy array): 
+            np.around(self._state) (numpy array):
                 vector of the given state rounded based off of the parameter
         """
         if (round < 0):
-            exit(f"Error: QuantumCircuit().state -- round placement must be a value greater than 0.")
-        return np.around(self._state, decimals = round)
-    def probabilities(self, round: int = 3):
+            exit(
+                f"Error: QuantumCircuit().state -- round placement must be a value greater than 0.")
+        return np.around(self._state, decimals=round)
+    
+    def circuitQueue(self):
+        return self._circuit
+    
+    def circuitSize(self):
+        return self._circuit_size
+
+    def probabilities(self, show_percent: bool = False, show_bit: int = -1, round: int = 3):
         """
         Return a matrix with all the probabilities for each state
         Params:
+            show_percent: bool
+            show_bit: string or int
             round: int
         Returns:
-            prob_matrix (numpy array): 
+            prob_matrix (numpy array):
                 matrix with all the weighted probabilities of being measured
         """
-        if (round < 0):
-            exit(f"Error: QuantumCircuit().probailities -- round placement must be a value greater than 0.")
-        # get the probabilties for the "winner" of the measurement at any single point on the circuit
-        prob_matrix = self._state
-        # collapse the circuit into 1D
-        prob_matrix = prob_matrix.flatten()
-        # square the values to get the probabilities of each qubit state
-        prob_matrix = np.square(prob_matrix)
-        # turn all the complex numbers into real values
-        prob_matrix = np.abs(prob_matrix)
-        prob_matrix = np.around(prob_matrix, decimals=round)
-        return prob_matrix
+        return probabilities(self._state, self._circuit_size, show_percent, show_bit, round)
+
     def measure(self):
         """
         Collapes the quantum circuit into classical bits
         Params:
             None
         Returns:
-            final_state (str): 
+            final_state (str):
                 the winning state displayed in classical bits notation
         """
         # randomly selects the measured state using self.probabilities()
-        prob_matrix = self.probabilities()
-        # number of bits
-        num_bits = self._circuit_size
-        # creates a list of bits in strings
-        state_list = [format(i, 'b').zfill(num_bits) for i in range(2**num_bits)] 
-        # turns state_list from list of strings to list of ints
-        state_list = list(map(int, state_list)) 
-        # numpy.random.choice takes in the list we will select from, size of the returning list,
-        #  and p = weights of each element 
-        final_state = np.random.choice(state_list, 1, p = prob_matrix)
-        # take out the bits from the returned list and convert to a string
-        final_state = str(final_state[0]) 
-        # pad with zeroes if needed
-        final_state = final_state.zfill(num_bits) 
-        # return the final state
-        return final_state
+        return measure(self._state, self._circuit_size, self.probabilities())
+
     def reverse(self):
         """
         Reverses the quantum state.
         Params:
             None.
         Returns:
             None.
         """
         # reverses the entire state, useful for quantum algorithms.
         self._state = self._state[::-1]
     """
     Multiple qubit quantum gates
     """
-    def toffoli(self, control_1: int, control_2: int, target: int):
+
+    def toffoli(self, control_1: int, control_2: int, target_qubit: int):
         """
-        A 3-qubit quantum gate that takes in two control qubits and one target qubit.
+        A 3-qubit quantum gate that takes in two control_qubit qubits and one target_qubit qubit.
         Params:
             control_1: int
             control_2: int
-            target: int
+            target_qubit: int
         Returns:
             None.
         """
         # If circuit is less than 3, means Toffoli gate cannot be allowed.
         if (self._circuit_size < 3):
-            exit(f"Error: QuantumCircuit().toffoli -- Quantum Circuit size must be 3 or more qubits. Current number of qubits is: {self._circuit_size}")
-        # Calls of gates here represent the Toffoli matrix using other quantum gates.
-        self.customControlPhase(control_2,target, Sx().matrix)
-        self.cnot(control_1,control_2)
-        self.customControlPhase(control_2,target, Sxdg().matrix)
+            exit(
+                f"Error: QuantumCircuit().toffoli -- Quantum Circuit size must be 3 or more qubits. Current number of qubits is: {self._circuit_size}")
+        # Calls of gates here represent the Toffoli matrix using other quantum
+        # gates.
+        self.customControlPhase(control_2, target_qubit, Sx().matrix)
+        self.cnot(control_1, control_2)
+        self.customControlPhase(control_2, target_qubit, Sxdg().matrix)
         self.cnot(control_1, control_2)
-        self.customControlPhase(control_1, target, Sx().matrix)
+        self.customControlPhase(control_1, target_qubit, Sx().matrix)
         # append gate to self._circuit
-        self._circuit[control_1].append('toffoli_control')
-        self._circuit[control_2].append('toffoli_control')
-        self._circuit[target].append('toffoli_target')
-    def rccx(self, control_1: int, control_2: int, target: int):
+        self._circuit.append(('toffoli', control_1, control_2, target_qubit))
+
+    def rccx(self, control_1: int, control_2: int, target_qubit: int):
         """
-        A 3-qubit quantum gate that takes in two control qubits and one target qubit.
+        A 3-qubit quantum gate that takes in two control_qubit qubits and one target_qubit qubit.
         Params:
             control_1: int
             control_2: int
-            target: int
+            target_qubit: int
         Returns:
             None.
         """
         # If circuit is less than 3, means RCCX gate cannot be allowed.
         if (self._circuit_size < 3):
-            exit(f"Error: QuantumCircuit().rccx -- Quantum Circuit size must be 3 or more qubits. Current number of qubits is: {self._circuit_size}")
-        # Calls of gates here represent the RCCX matrix using other quantum gates.
-        self.u(target, np.pi / 2, 0, np.pi)
-        self.u(target, 0,0,np.pi / 4)
-        self.cnot(control_2, target)
-        self.u(target, 0,0,(-1 * np.pi) / 4)
-        self.cnot(control_1, target)
-        self.u(target, 0,0,np.pi / 4)
-        self.cnot(control_2, target)
-        self.u(target, 0,0,(-1 * np.pi) / 4)
-        self.u(target, np.pi / 2, 0, np.pi)
-        # append gate to self._circuit
-        self._circuit[control_1].append('rccx_control')
-        self._circuit[control_2].append('rccx_control')
-        self._circuit[target].append('rccx_target')
+            exit(
+                f"Error: QuantumCircuit().rccx -- Quantum Circuit size must be 3 or more qubits. Current number of qubits is: {self._circuit_size}")
+        # Calls of gates here represent the RCCX matrix using other quantum
+        # gates.
+        self.u(target_qubit, np.pi / 2, 0, np.pi)
+        self.u(target_qubit, 0, 0, np.pi / 4)
+        self.cnot(control_2, target_qubit)
+        self.u(target_qubit, 0, 0, (-1 * np.pi) / 4)
+        self.cnot(control_1, target_qubit)
+        self.u(target_qubit, 0, 0, np.pi / 4)
+        self.cnot(control_2, target_qubit)
+        self.u(target_qubit, 0, 0, (-1 * np.pi) / 4)
+        self.u(target_qubit, np.pi / 2, 0, np.pi)
+        # append gate to self._circuit
+        self._circuit.append(('rccx', control_1, control_2, target_qubit))
+
     def rc3x(self, a: int, b: int, c: int, d: int):
         """
         A 4-qubit quantum gate that is a simplified Toffoli gate and can be used in placed where the Toffoli gate is uncomputed again.
         Params:
             a: int
             b: int
             c: int
             d: int
         Returns:
             None.
         """
         # If circuit is less than 4, means RC3X gate cannot be allowed.
         if (self._circuit_size < 4):
-            exit(f"Error: QuantumCircuit().rc3x -- Quantum Circuit size must be 4 or more qubits. Current number of qubits is: {self._circuit_size}")
-        # Calls of gates here represent the RC3X matrix using other quantum gates.
-        self.u(d, np.pi / 2, 0 , np.pi)
-        self.u(d, 0,0,np.pi / 4)
+            exit(
+                f"Error: QuantumCircuit().rc3x -- Quantum Circuit size must be 4 or more qubits. Current number of qubits is: {self._circuit_size}")
+        # Calls of gates here represent the RC3X matrix using other quantum
+        # gates.
+        self.u(d, np.pi / 2, 0, np.pi)
+        self.u(d, 0, 0, np.pi / 4)
         self.cnot(c, d)
-        self.u(d, 0,0,(-1 * np.pi) / 4)
+        self.u(d, 0, 0, (-1 * np.pi) / 4)
         self.u(d, np.pi / 2, 0, np.pi)
         self.cnot(a, d)
-        self.u(d, 0,0,np.pi / 4)
+        self.u(d, 0, 0, np.pi / 4)
         self.cnot(b, d)
-        self.u(d, 0,0, (-1 * np.pi / 4))
+        self.u(d, 0, 0, (-1 * np.pi / 4))
         self.cnot(a, d)
-        self.u(d, 0,0, np.pi / 4)
+        self.u(d, 0, 0, np.pi / 4)
         self.cnot(b, d)
-        self.u(d, 0,0, (-1 * np.pi) / 4)
+        self.u(d, 0, 0, (-1 * np.pi) / 4)
         self.u(d, np.pi / 2, 0, np.pi)
         self.u(d, 0, 0, np.pi / 4)
         self.cnot(c, d)
         self.u(d, 0, 0, (-1 * np.pi / 4))
         self.u(d, np.pi / 2, 0, np.pi)
         # append gate to self._circuit
-        self._circuit[a].append('rc3x_control')
-        self._circuit[b].append('rc3x_control')
-        self._circuit[c].append('rc3x_control')
-        self._circuit[d].append('rc3x_target')
-    def cnot(self, control: int, target: int):
+        self._circuit.append(('rc3x', a, b, c, d))
+
+    def cnot(self, control_qubit: int, target_qubit: int):
         """
-        A 2-qubit quantum gate that takes in control and target qubits, and will entangle the qubits if the control qubit is greater than 0.
+        A 2-qubit quantum gate that takes in control_qubit and target_qubit qubits, and will entangle the qubits if the control_qubit qubit is greater than 0.
         Params:
-            control: int
-            target: int
+            control_qubit: int
+            target_qubit: int
         Returns:
             None.
         """
         # If circuit is less than 2, means CNOT gate cannot be allowed.
         if (self._circuit_size < 2):
-            exit(f"Error: QuantumCircuit().cnot -- Quantum Circuit size must be 2 or more qubits. Current number of qubits is: {self._circuit_size}")
-        # Determines if the little endian or big endian CNOT gate needs to be established for calculations.
+            exit(
+                f"Error: QuantumCircuit().cnot -- Quantum Circuit size must be 2 or more qubits. Current number of qubits is: {self._circuit_size}")
+        # Determines if the little endian or big endian CNOT gate needs to be
+        # established for calculations.
         if self._little_endian:
             cnot_matrix = CNot().matrix
         else:
-            cnot_matrix = CNot(inverse = True).matrix
-        # Sends to __controlled_phase_handler alongside a boolean confirming the gate is indeed a CNOT gate
-        self.__controlled_phase_handler__(cnot_matrix, control, target)
-        # append gate to self._circuit
-        self._circuit[control].append('cnot_control')
-        self._circuit[target].append('cnot_target')
-    def cr(self, control: int, target:int):
+            cnot_matrix = CNot(inverse=True).matrix
+        # Sends to __controlled_phase_handler alongside a boolean confirming
+        # the gate is indeed a CNOT gate
+        self.__controlled_phase_handler__(
+            cnot_matrix, control_qubit, target_qubit)
+        # append gate to self._circuit
+        self._circuit.append(('cnot', control_qubit, target_qubit))
+
+    def cr(self, control_qubit: int, target_qubit: int):
         """
-        A 2-qubit quantum gate that takes in control and target qubits to perform calculations upon the state.
+        A 2-qubit quantum gate that takes in control_qubit and target_qubit qubits to perform calculations upon the state.
         Params:
-            control: int
-            target: int
+            control_qubit: int
+            target_qubit: int
         Returns:
             None.
         """
         # If circuit is less than 2, means CR gate cannot be allowed.
         if (self._circuit_size < 2):
-            exit(f"Error: QuantumCircuit().cr -- Quantum Circuit size must be 2 or more qubits. Current number of qubits is: {self._circuit_size}")
-        self.__controlled_phase_handler__(Cr().matrix, control, target)
+            exit(
+                f"Error: QuantumCircuit().cr -- Quantum Circuit size must be 2 or more qubits. Current number of qubits is: {self._circuit_size}")
+        self.__controlled_phase_handler__(
+            Cr().matrix, control_qubit, target_qubit)
         # append gate to self._circuit
-        self._circuit[control].append('cr_control')
-        self._circuit[target].append('cr_target')
-    def cz(self, control: int, target:int):
+        self._circuit.append(('cr', control_qubit, target_qubit))
+
+    def cz(self, control_qubit: int, target_qubit: int):
         """
-        A 2-qubit quantum gate that takes in control and target qubits to perform calculations upon the state.
+        A 2-qubit quantum gate that takes in control_qubit and target_qubit qubits to perform calculations upon the state.
         Params:
-            control: int
-            target: int
+            control_qubit: int
+            target_qubit: int
         Returns:
             None.
         """
         # If circuit is less than 2, means CZ gate cannot be allowed.
         if (self._circuit_size < 2):
-            exit(f"Error: QuantumCircuit().cz -- Quantum Circuit size must be 2 or more qubits. Current number of qubits is: {self._circuit_size}")
-        self.__controlled_phase_handler__(Cz().matrix, control, target)
+            exit(
+                f"Error: QuantumCircuit().cz -- Quantum Circuit size must be 2 or more qubits. Current number of qubits is: {self._circuit_size}")
+        self.__controlled_phase_handler__(
+            Cz().matrix, control_qubit, target_qubit)
         # append gate to self._circuit
-        self._circuit[control].append('cz_control')
-        self._circuit[target].append('cz_target')
+        self._circuit.append(('cz', control_qubit, target_qubit))
+
     def swap(self, qubit_1: int, qubit_2: int):
         """
         A 2-qubit quantum gate that takes in two qubits to swap the qubits values they represent.
         Params:
             qubit_1: int
             qubit_2: int
         Returns:
             None.
         """
         # If circuit is less than 2, means SWAP gate cannot be allowed.
         if (self._circuit_size < 2):
-            exit(f"Error: QuantumCircuit().swap -- Quantum Circuit size must be 2 or more qubits. Current number of qubits is: {self._circuit_size}")
+            exit(
+                f"Error: QuantumCircuit().swap -- Quantum Circuit size must be 2 or more qubits. Current number of qubits is: {self._circuit_size}")
         # get the swap matrix
         swap_matrix = Swap().matrix
-        # determines if the two values at play are at distance greater than one, if so it will call in private method for larger matrix operations.
-        if(qubit_1 - qubit_2 != 1 and qubit_1 - qubit_2 != -1):
+        # determines if the two values at play are at distance greater than
+        # one, if so it will call in private method for larger matrix
+        # operations.
+        if (qubit_1 - qubit_2 != 1 and qubit_1 - qubit_2 != -1):
             self.__controlled_phase_handler__(swap_matrix, qubit_1, qubit_2)
-        # if qubit_2 is above qubit_1 on the quantum wire, then it will use qubit_2 as the call to __operator_matrix__.
-        elif(qubit_1 > qubit_2):
-            self._state = np.dot(self.__operator_matrix__(swap_matrix, qubit_2, double=True), self._state)
+        # if qubit_2 is above qubit_1 on the quantum wire, then it will use
+        # qubit_2 as the call to __operator_matrix__.
+        elif (qubit_1 > qubit_2):
+            self._state = np.dot(
+                self.__operator_matrix__(
+                    swap_matrix,
+                    qubit_2,
+                    double=True),
+                self._state)
         # simply commits a normal SWAP quantum gate functionality.
         else:
-            self._state = np.dot(self.__operator_matrix__(swap_matrix, qubit_1, double=True), self._state)
+            self._state = np.dot(
+                self.__operator_matrix__(
+                    swap_matrix,
+                    qubit_1,
+                    double=True),
+                self._state)
         # append gate to self._circuit
-        self._circuit[qubit_1].append('swap')
-        self._circuit[qubit_2].append('swap')
+        self._circuit.append(('swap', qubit_1, qubit_2))
+
     def rxx(self, qubit_1: int, qubit_2: int, theta: float = np.pi / 2):
         """
         A 2-qubit quantum gate that takes in two qubits and a representation of theta to initialize in the quantum state.
         Params:
             qubit_1: int
             qubit_2: int
             theta: float
         Returns:
             None.
         """
         # If circuit is less than 2, means RXX gate cannot be allowed.
         if (self._circuit_size < 2):
-            exit(f"Error: QuantumCircuit().rxx -- Quantum Circuit size must be 2 or more qubits. Current number of qubits is: {self._circuit_size}")
+            exit(
+                f"Error: QuantumCircuit().rxx -- Quantum Circuit size must be 2 or more qubits. Current number of qubits is: {self._circuit_size}")
         rxx_matrix = Rxx(theta).matrix
         self.__controlled_phase_handler__(rxx_matrix, qubit_1, qubit_2)
         # append gate to self._circuit
-        self._circuit[qubit_1].append('rxx')
-        self._circuit[qubit_2].append('rxx')
+        self._circuit.append(('rxx', qubit_1, qubit_2))
+
     def rzz(self, qubit_1: int, qubit_2: int, theta: float = np.pi / 2):
         """
         A 2-qubit quantum gate that takes in two qubits and a representation of theta to initialize in the quantum state.
         Params:
             qubit_1: int
             qubit_2: int
             theta: float
         Returns:
             None.
         """
         # If circuit is less than 2, means RZZ gate cannot be allowed.
         if (self._circuit_size < 2):
-            exit(f"Error: QuantumCircuit().rzz -- Quantum Circuit size must be 2 or more qubits. Current number of qubits is: {self._circuit_size}")
+            exit(
+                f"Error: QuantumCircuit().rzz -- Quantum Circuit size must be 2 or more qubits. Current number of qubits is: {self._circuit_size}")
         if (qubit_2 < qubit_1):
             qubit_2, qubit_1 = qubit_1, qubit_2
         rzz_matrix = Rzz(theta).matrix
-        # determines if the two values at play are at distance greater than one, if so it will call in private method for larger matrix operations.
+        # determines if the two values at play are at distance greater than
+        # one, if so it will call in private method for larger matrix
+        # operations.
         self.__controlled_phase_handler__(rzz_matrix, qubit_1, qubit_2)
         # append gate to self._circuit
-        self._circuit[qubit_1].append('rzz')
-        self._circuit[qubit_2].append('rzz')
-    def customControlPhase(self, control: int, target: int, custom_matrix: np.array):
+        self._circuit.append(('rzz', qubit_1, qubit_2))
+
+    def customControlPhase(
+            self,
+            control_qubit: int,
+            target_qubit: int,
+            custom_matrix: np.array):
         """
-        Used to insert single qubit based quantum gates to have a control qubit apart of it and committing to the quantum state.
+        Used to insert single qubit based quantum gates to have a control_qubit qubit apart of it and committing to the quantum state.
         Params:
-            control: int
-            target: int
+            control_qubit: int
+            target_qubit: int
             custom_matrix: np.array
         Returns:
             None.
         """
-        # custom quantum gate can only call in a single qubit based matrix to manipulate the state.
-        if (custom_matrix.shape != (2,2)):
+        # custom quantum gate can only call in a single qubit based matrix to
+        # manipulate the state.
+        if (custom_matrix.shape != (2, 2)):
             exit(f"Error: QuantumCircuit().customControlPhase -- can only include a single qubit based quantum gate (2,2) matrix for state manipulation.")
-        # Determines if the matrix needs to be representing in little or big endian format.
+        # Determines if the matrix needs to be representing in little or big
+        # endian format.
         if self._little_endian:
             # If little endian format is being used.
             controlled_custom_matrix = np.array([
-                        [1+0j, 0+0j, 0+0j, 0+0j],
-                        [0+0j, custom_matrix[0][0], 0+0j, custom_matrix[0][1]],
-                        [0+0j, 0+0j, 1+0j, 0+0j],
-                        [0+0j, custom_matrix[1][0], 0+0j, custom_matrix[1][1]]
-                    ])
-            
+                [1 + 0j, 0 + 0j, 0 + 0j, 0 + 0j],
+                [0 + 0j, custom_matrix[0][0], 0 + 0j, custom_matrix[0][1]],
+                [0 + 0j, 0 + 0j, 1 + 0j, 0 + 0j],
+                [0 + 0j, custom_matrix[1][0], 0 + 0j, custom_matrix[1][1]]
+            ])
+
         else:
             # If big endian format is in being used.
             controlled_custom_matrix = np.array([
-                    [1+0j, 0+0j, 0+0j, 0+0j],
-                    [0+0j, 1+0j, 0+0j, 0+0j],
-                    [0+0j, 0+0j, custom_matrix[0][0], custom_matrix[0][1]],
-                    [0+0j, 0+0j,custom_matrix[1][0], custom_matrix[1][1]]
-                ])
-        self.__controlled_phase_handler__(controlled_custom_matrix, control, target)
-        
+                [1 + 0j, 0 + 0j, 0 + 0j, 0 + 0j],
+                [0 + 0j, 1 + 0j, 0 + 0j, 0 + 0j],
+                [0 + 0j, 0 + 0j, custom_matrix[0][0], custom_matrix[0][1]],
+                [0 + 0j, 0 + 0j, custom_matrix[1][0], custom_matrix[1][1]]
+            ])
+        self.__controlled_phase_handler__(
+            controlled_custom_matrix, control_qubit, target_qubit)
+        self._circuit.append(('C', control_qubit, target_qubit))
+
     """
     Single Qubit Gates
     """
+
     def identity(self, qubit: int):
         """
         Used to confirm value that a qubit is representing and does nothing to manipulate the value of such qubit.
         Params:
             qubit: int
         Returns:
             None.
         """
-        if qubit == None:
-            exit(f"Error: QuantumCircuit().identity -- Must select a qubit to enact on quantum gate.")
-        identity_matrix = Identity().matrix
-        self._state = np.dot(self.__operator_matrix__(identity_matrix, qubit), self._state)
+        if qubit is None:
+            exit(
+                f"Error: QuantumCircuit().identity -- Must select a qubit to enact on quantum gate.")
+        self._state = np.dot(
+            self.__operator_matrix__(
+                Identity().matrix,
+                qubit),
+            self._state)
         # append gate to self._circuit
-        self._circuit[qubit].append('identity')
+        self._circuit.append((Identity().symbol, qubit))
+
     def x(self, qubit: int):
         """
         Used to invert the value of what a qubit is representing.
         Params:
             qubit: int
         Returns:
             None.
         """
-        if qubit == None:
-            exit(f"Error: QuantumCircuit().x -- Must select a qubit to enact on quantum gate.")
+        if qubit is None:
+            exit(
+                f"Error: QuantumCircuit().x -- Must select a qubit to enact on quantum gate.")
         # get the not matrix
-        x_matrix = PauliX().matrix
-        self._state = np.dot(self.__operator_matrix__(x_matrix, qubit), self._state)
+        self._state = np.dot(
+            self.__operator_matrix__(
+                PauliX().matrix, qubit), self._state)
         # append gate to self._circuit
-        self._circuit[qubit].append('x')
+        self._circuit.append((PauliX().symbol, qubit))
+
     def hadamard(self, qubit: int):
         """
         Used to put a given qubit into superposition.
         Params:
             qubit: int
         Returns:
             None.
         """
-        if qubit == None:
-            exit(f"Error: QuantumCircuit().hadamard -- Must select a qubit to enact on quantum gate.")
+        if qubit is None:
+            exit(
+                f"Error: QuantumCircuit().hadamard -- Must select a qubit to enact on quantum gate.")
         # get the hadamard matrix
-        h_matrix = Hadamard().matrix
-        self._state = np.dot(self.__operator_matrix__(h_matrix, qubit), self._state)
+        self._state = np.dot(
+            self.__operator_matrix__(
+                Hadamard().matrix, qubit), self._state)
         # append gate to self._circuit
-        self._circuit[qubit].append('hadamard')
+        self._circuit.append((Hadamard().symbol, qubit))
+
     def y(self, qubit: int):
         """
         Changes the state of a qubit by pi around the y-axis of a Bloch Sphere.
         Params:
             qubit: int
         Returns:
             None.
         """
-        if qubit == None:
-            exit(f"Error: QuantumCircuit().y -- Must select a qubit to enact on quantum gate.")
+        if qubit is None:
+            exit(
+                f"Error: QuantumCircuit().y -- Must select a qubit to enact on quantum gate.")
         # get the Y matrix
-        y_matrix = PauliY().matrix
-        self._state = np.dot(self.__operator_matrix__(y_matrix, qubit), self._state)
+        self._state = np.dot(
+            self.__operator_matrix__(
+                PauliY().matrix, qubit), self._state)
         # append gate to self._circuit
-        self._circuit[qubit].append('y')
+        self._circuit.append(PauliY().symbol)
+
     def z(self, qubit: int):
         """
         Changes the state of a qubit by pi around the z-axis of a Bloch Sphere.
         Params:
             qubit: int
         Returns:
             None.
         """
-        if qubit == None:
-            exit(f"Error: QuantumCircuit().z -- Must select a qubit to enact on quantum gate.")
+        if qubit is None:
+            exit(
+                f"Error: QuantumCircuit().z -- Must select a qubit to enact on quantum gate.")
         # get the Z matrix
-        z_matrix = PauliZ().matrix
-        self._state = np.dot(self.__operator_matrix__(z_matrix, qubit), self._state)
+        self._state = np.dot(
+            self.__operator_matrix__(
+                PauliZ().matrix, qubit), self._state)
         # append gate to self._circuit
-        self._circuit[qubit].append('z')
+        self._circuit.append((PauliZ().symbol, qubit))
+
     def phase(self, qubit: int, theta: float = np.pi / 2):
         """
         Commits to a rotation around the z-axis based off of the inputted theta value.
         Params:
             qubit: int
             theta: float
         Returns:
             None.
         """
-        if qubit == None:
-            exit(f"Error: QuantumCircuit().phase -- Must select a qubit to enact on quantum gate.")
+        if qubit is None:
+            exit(
+                f"Error: QuantumCircuit().phase -- Must select a qubit to enact on quantum gate.")
         # get the Phase matrix
-        phase_matrix = Phase(theta).matrix
-        self._state = np.dot(self.__operator_matrix__(phase_matrix, qubit), self._state)
+        self._state = np.dot(
+            self.__operator_matrix__(
+                Phase(theta).matrix, qubit), self._state)
         # append gate to self._circuit
-        self._circuit[qubit].append('phase')
+        self._circuit.append((Phase(theta).symbol, qubit))
+
     def s(self, qubit: int):
         """
-        Is a Phase gate where the inputted theta value is given as a constant of theta = pi / 2. 
+        Is a Phase gate where the inputted theta value is given as a constant of theta = pi / 2.
         Params:
             qubit: int
         Returns:
             None.
         """
-        if qubit == None:
-            exit(f"Error: QuantumCircuit().s -- Must select a qubit to enact on quantum gate.")
+        if qubit is None:
+            exit(
+                f"Error: QuantumCircuit().s -- Must select a qubit to enact on quantum gate.")
         # get the Phase matrix
-        phase_matrix = S().matrix
-        self._state = np.dot(self.__operator_matrix__(phase_matrix, qubit), self._state)
+        self._state = np.dot(
+            self.__operator_matrix__(
+                S().matrix, qubit), self._state)
         # append gate to self._circuit
-        self._circuit[qubit].append('s')
+        self._circuit.append((S().symbol, qubit))
+
     def sdg(self, qubit: int):
         """
-        Is a Phase gate and inverse of the S gate where the inputted theta value is given as a constant of theta = -pi / 2. 
+        Is a Phase gate and inverse of the S gate where the inputted theta value is given as a constant of theta = -pi / 2.
         Params:
             qubit: int
         Returns:
             None.
         """
-        if qubit == None:
-            exit(f"Error: QuantumCircuit().sdg -- Must select a qubit to enact on quantum gate.")
+        if qubit is None:
+            exit(
+                f"Error: QuantumCircuit().sdg -- Must select a qubit to enact on quantum gate.")
         # get the Sdg matrix
-        sdg_matrix = Sdg().matrix
-        self._state = np.dot(self.__operator_matrix__(sdg_matrix, qubit), self._state)
+        self._state = np.dot(
+            self.__operator_matrix__(
+                Sdg().matrix, qubit), self._state)
         # append gate to self._circuit
-        self._circuit[qubit].append('sdg')
+        self._circuit.append((Sdg().symbol, qubit))
+
     def t(self, qubit: int):
         """
         T gate is a special use case gate that in implemented from the P Gate.
         Params:
             qubit: int
         Returns:
             None.
         """
-        if qubit == None:
-            exit(f"Error: QuantumCircuit().t -- Must select a qubit to enact on quantum gate.")
+        if qubit is None:
+            exit(
+                f"Error: QuantumCircuit().t -- Must select a qubit to enact on quantum gate.")
         # get the T matrix
-        t_matrix = T().matrix
-        self._state = np.dot(self.__operator_matrix__(t_matrix, qubit), self._state)
+        self._state = np.dot(
+            self.__operator_matrix__(
+                T().matrix, qubit), self._state)
         # append gate to self._circuit
-        self._circuit[qubit].append('t')
+        self._circuit.append((T().symbol, qubit))
+
     def tdg(self, qubit: int):
         """
         TDG gate is a special use case gate that in implemented from the P Gate and is the inverse of the T gate.
         Params:
             qubit: int
         Returns:
             None.
         """
-        if qubit == None:
-            exit(f"Error: QuantumCircuit().tdg -- Must select a qubit to enact on quantum gate.")
+        if qubit is None:
+            exit(
+                f"Error: QuantumCircuit().tdg -- Must select a qubit to enact on quantum gate.")
         # get the Tdg matrix
-        tdg_matrix = Tdg().matrix
-        self._state = np.dot(self.__operator_matrix__(tdg_matrix, qubit), self._state)
+        self._state = np.dot(
+            self.__operator_matrix__(
+                Tdg().matrix, qubit), self._state)
         # append gate to self._circuit
-        self._circuit[qubit].append('tdg')
+        self._circuit.append((Tdg().symbol, qubit))
+
     def rz(self, qubit: int, theta: float = np.pi / 2):
         """
         RZ gate commits a rotation around the z-axis for a qubit.
         Params:
             qubit: int
             theta: float
         Returns:
             None.
         """
-        if qubit == None:
-            exit(f"Error: QuantumCircuit().rz -- Must select a qubit to enact on quantum gate.")
+        if qubit is None:
+            exit(
+                f"Error: QuantumCircuit().rz -- Must select a qubit to enact on quantum gate.")
         # get the Rz matrix
-        rz_matrix = Rz(theta).matrix
-        self._state = np.dot(self.__operator_matrix__(rz_matrix, qubit), self._state)
+        self._state = np.dot(
+            self.__operator_matrix__(
+                Rz(theta).matrix, qubit), self._state)
         # append gate to self._circuit
-        self._circuit[qubit].append('rz')
+        self._circuit.append((Rz(theta).matrix, qubit))
+
     def ry(self, qubit: int, theta: float = np.pi / 2):
         """
         RY gate commits a rotation around the y-axis for a qubit.
         Params:
             qubit: int
             theta: float
         Returns:
             None.
         """
-        if qubit == None:
-            exit(f"Error: QuantumCircuit().ry -- Must select a qubit to enact on quantum gate.")
+        if qubit is None:
+            exit(
+                f"Error: QuantumCircuit().ry -- Must select a qubit to enact on quantum gate.")
         # get the Ry matrix
-        ry_matrix = Ry(theta).matrix
-        self._state = np.dot(self.__operator_matrix__(ry_matrix, qubit), self._state)
+        self._state = np.dot(
+            self.__operator_matrix__(
+                Ry(theta).matrix, qubit), self._state)
         # append gate to self._circuit
-        self._circuit[qubit].append('ry')
+        self._circuit.append((Ry().symbol, qubit))
+
     def rx(self, qubit: int, theta: float = np.pi / 2):
         """
         RX gate commits a rotation around the x-axis for a qubit.
         Params:
             qubit: int
             theta: float
         Returns:
             None.
         """
-        if qubit == None:
-            exit(f"Error: QuantumCircuit().rx -- Must select a qubit to enact on quantum gate.")
-        # get the Ry matrix
-        rx_matrix = Rx(theta).matrix
-        self._state = np.dot(self.__operator_matrix__(rx_matrix, qubit), self._state)
+        if qubit is None:
+            exit(
+                f"Error: QuantumCircuit().rx -- Must select a qubit to enact on quantum gate.")
+        # get the Rx matrix
+        self._state = np.dot(
+            self.__operator_matrix__(
+                Rx(theta).matrix, qubit), self._state)
         # append gate to self._circuit
-        self._circuit[qubit].append('rx')
+        self._circuit.append((Rx(theta).matrix, qubit))
+
     def sx(self, qubit: int):
         """
         SX gate is the square root of the Inverse gate (X, PauliX Gate).
         Params:
             qubit: int
         Returns:
             None.
         """
-        if qubit == None:
-            exit(f"Error: QuantumCircuit().sx -- Must select a qubit to enact on quantum gate.")
+        if qubit is None:
+            exit(
+                f"Error: QuantumCircuit().sx -- Must select a qubit to enact on quantum gate.")
         # get the Sx matrix
-        sx_matrix = Sx().matrix
-        self._state = np.dot(self.__operator_matrix__(sx_matrix, qubit), self._state)  
+        self._state = np.dot(
+            self.__operator_matrix__(
+                Sx().matrix, qubit), self._state)
         # append gate to self._circuit
-        self._circuit[qubit].append('sx')                                         
+        self._circuit.append((Sx().symbol, qubit))
+
     def sxdg(self, qubit: int):
         """
         SXDG gate is the negative square root of the Inverse gate (X, PauliX Gate) and inverse of the SX gate.
         Params:
             qubit: int
         Returns:
             None.
         """
-        if qubit == None:
-            exit(f"Error: QuantumCircuit().sxdg -- Must select a qubit to enact on quantum gate.")
+        if qubit is None:
+            exit(
+                f"Error: QuantumCircuit().sxdg -- Must select a qubit to enact on quantum gate.")
         # get the Sxdg matrix
-        sxdg_matrix = Sxdg().matrix
-        self._state = np.dot(self.__operator_matrix__(sxdg_matrix, qubit), self._state)
+        self._state = np.dot(
+            self.__operator_matrix__(
+                Sxdg().matrix, qubit), self._state)
         # append gate to self._circuit
-        self._circuit[qubit].append('sxdg')
-    def u(self, qubit: int, theta: float = np.pi / 2, phi: float = np.pi / 2, lmbda: float = np.pi / 2):
+        self._circuit.append((Sxdg().symbol, qubit))
+
+    def u(
+        self,
+        qubit: int,
+        theta: float = np.pi / 2,
+        phi: float = np.pi / 2,
+            lmbda: float = np.pi / 2):
         """
         U gate is given three inputs (theta, phi, and lambda) that allow the inputs to manipulate the base matrix to allow for the position of the enacted qubit
         around the bloch sphere representation.
         Params:
             qubit: int
             theta: float
             phi: float
             lmbda: float
         Returns:
             None.
         """
-        if qubit == None:
-            exit(f"Error: QuantumCircuit().u -- Must select a qubit to enact on quantum gate.")
+        if qubit is None:
+            exit(
+                f"Error: QuantumCircuit().u -- Must select a qubit to enact on quantum gate.")
         # get the U matrix
-        u_matrix = U(theta, phi, lmbda).matrix
-        self._state = np.dot(self.__operator_matrix__(u_matrix, qubit), self._state)
+        self._state = np.dot(
+            self.__operator_matrix__(
+                U(theta, phi, lmbda).matrix, qubit), self._state)
         # append gate to self._circuit
-        self._circuit[qubit].append('u')
+        self._circuit.append((U().symbol, qubit))
+
     def custom(self, qubit: int, custom_matrix: np.array):
         """
         Will take in a custom single qubit quantum gate and implement it on a qubit.
         Params:
             qubit: int
             custom_matrix: np.array
         Returns:
             None.
         """
         # if gate is not a single qubit, will exit.
-        if (custom_matrix.shape != (2,2)):
+        if (custom_matrix.shape != (2, 2)):
             exit(f"Error: QuantumCircuit().insertGate -- can only include a single qubit based quantum gate (2,2) matrix for state manipulation.")
         # calls gate and will operate on state as per usual
-        self._state = np.dot(self.__operator_matrix__(custom_matrix, qubit), self._state)
+        self._state = np.dot(
+            self.__operator_matrix__(
+                custom_matrix,
+                qubit),
+            self._state)
+        self._circuit.append(('C', qubit))
```

### Comparing `QCpython-1.0.2/QCpy/Qubit.py` & `QCpython-1.0.3/QCpy/qubit.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 Purpose:
 To initialize the values in the QuantumCircuit and to determine the angle of the initial state of the quantum wire.
 Methods
 --------
 None.
 
 """
+
+
 class Qubit:
     def __init__(self, initial_state: chr = 'z'):
         """
         Args:
             initial_state:
                 A character input of either x, y, z to indicate either the qubit's facing to be at either the z axis, y axis, or x axis in true whole value.
         ----
@@ -23,18 +25,21 @@
             Sets a variable in the class object from the argument to determine what the qubits facing is.
         state: 
             Is the variable to store the matrix of what the qubits starting face is and will be called from other systems to determine themselves.
         """
         self._INITIAL_STATE = initial_state
         self.state = None
         # Sets qubit to the z-axis and will face "upwards" or [1,0,...n^2 - 1].
-        if(self._INITIAL_STATE == 'z'):
+        if (self._INITIAL_STATE == 'z'):
             self.state = np.array([[1+0j], [0+0j]], 'F')
             # Sets the qubit to the y-axis.
-        elif(self._INITIAL_STATE == 'y'):
-            self.state = np.array([[0+0j + 1+0j], [(1+0j + 0+0j) * 0+1j]], 'F') / np.sqrt(2)
+        elif (self._INITIAL_STATE == 'y'):
+            self.state = np.array(
+                [[0+0j + 1+0j], [(1+0j + 0+0j) * 0+1j]], 'F') / np.sqrt(2)
             # Sets the qubit to the y-axis.
-        elif(self._INITIAL_STATE == 'x'):
-            self.state = np.array([[0+0j + 1+0j], [1+0j + 0+0j]], 'F') / np.sqrt(2)     
-            # Calls error as no other plane of existence for calculations exists.    
+        elif (self._INITIAL_STATE == 'x'):
+            self.state = np.array(
+                [[0+0j + 1+0j], [1+0j + 0+0j]], 'F') / np.sqrt(2)
+            # Calls error as no other plane of existence for calculations exists.
         else:
-            exit(f"Error: Qubit.__init__() -- Qubit must be initialized in a 0 or 1 state \n Qubit was initialized in state: {initial_state}.")
+            exit(
+                f"Error: Qubit.__init__() -- Qubit must be initialized in a 0 or 1 state \n Qubit was initialized in state: {initial_state}.")
```

### Comparing `QCpython-1.0.2/QCpython.egg-info/PKG-INFO` & `QCpython-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 Metadata-Version: 2.1
 Name: QCpython
-Version: 1.0.2
-Summary: QCpy is a lightweight quantum circuit simulator and visualization of quantum computing.
+Version: 1.0.3
+Summary: QCpy is a comprehensive and user-friendly library for quantum computing, providing a wide range of functionality for quantum algorithms and quantum circuits. It is built on using open-source libraries NumPy and Matplotlib; compatible with Python 3.
 Home-page: https://github.com/QCpython/QCpy
 Author: Brennan Freeze, Paris Osuch, Aundre Barras, Soren Richenberg, Suzanne Rivoire
 Author-email: freezebrennan@gmail.com, osuch@sonoma.edu, barras@sonoma.edu, richenbe@sonoma.edu, rivoire@sonoma.edu
-Keywords: quantum computing,physics,visualization,quantum circuit
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 # README.md
 
 # QCpy - A Quantum Computing Library for Python
 
 QCpy is an open source python library and collaborative project for flexible simulations and visualizations of quantum circuits. Designed by college students with students in mind, this library contains a powerful set of tools to teach computer scientists about the emerging discipline of quantum computing (QC).
 
+You can download the package using pip:
+
+```txt
+pip install QCpython
+```
+
 ## Recommended Resources on Quantum Computing:
 
 - [Microsoft’s Linear Algebra for Quantum Computing](https://learn.microsoft.com/en-us/azure/quantum/overview-algebra-for-quantum-computing)
 - [IBM’s Quantum Computing: a field guide](https://quantum-computing.ibm.com/composer/docs/iqx/guide/)
 - [Wikipedia: Quantum Computing](https://en.wikipedia.org/wiki/Quantum_computing)
 
 ---
 
 # Qubits
 
-> ## *class* QC.Qubit.`Qubit`(*initial_state=’z’*)
+> ## *class* QCpy.`Qubit`(*initial_state=’z’*)
 
 *Object representation of a qubit.*
 
 ### Parameters:
 
 `initial_state (chr)` - Character input for starting direction in the *x*, *y*, or *z* axis.
 
@@ -100,15 +110,15 @@
 `None`
 
 ### Attributes:
 
 `matrix (np.ndarray)` - matrix representation of Pauli-Z gate.
 
 ```python
-PauliY.matrix = [1+0j, 0+0j], 
+PauliZ.matrix = [1+0j, 0+0j], 
                 [0+0j, -1+0j]
 ```
 
 > ## *class* QC.QuantumGate.`Hadamard`()
 
 *Maps the basis states |0> to |+> and |1> to |->, creating a superposition state if given a computation basis state.*
 
@@ -456,15 +466,15 @@
 Cz.matrix = [1+0j, 0+0j, 0+0j, 0+0j],
             [0+0j, 1+0j, 0+0j, 0+0j],
             [0+0j, 0+0j, 1+0j, 0+0j],
             [0+0j, 0+0j, 0+0j, -1+0j]
 ```
 ---
 # Quantum Circuit
-> ## *class* QC.QuantumCircuit.`QuantumCircuit`(*qubits*, *little_endian=False*, *prep='z'*)
+> ## *class* QCpy.`QuantumCircuit`(*qubits*, *little_endian=False*, *prep='z'*)
 
 *Quantum circuit that represents the state of a quantum system and performs operations on select qubits.*
 
 ### Parameters:
 
 `qubits (int)` - number of qubits in the circuit.
 
@@ -595,14 +605,48 @@
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.   +0.j]
 # [0.707+0.j]]
 ```
 
+> ## QuantumCircuit.`circuitQueue()`
+
+*Returns queue of gates on quantum circuit.*
+
+### Parameters:
+
+`None`
+
+### Returns:
+`queue (list)` - list of gates queued on quantum circuit.
+
+### Example:
+
+```python
+from QCpy import QuantumCircuit
+
+qc = QuantumCircuit(4)
+
+qc.x(0)
+qc.x(1)
+qc.x(2)
+qc.rc3x(0, 1, 2, 3)
+
+print(qc.circuitQueue())
+
+# [('X', 0), ('X', 1), ('X', 2), ('U', 3), ('U', 3), ('cnot', 2, # 3), ('U', 3), ('U', 3), ('swap', 2, 3), ('swap', 1, 2), 
+# ('swap', 1, 2), ('swap', 2, 3), ('cnot', 0, 3), ('U', 3),
+# ('swap', 2, 3), ('swap', 2, 3), ('cnot', 1, 3), ('U', 3), 
+# ('swap', 2, 3), ('swap', 1, 2), ('swap', 1, 2), ('swap', 2, 
+# 3), ('cnot', 0, 3), ('U', 3), ('swap', 2, 3), ('swap', 2, 3),
+#  ('cnot', 1, 3), ('U', 3), ('U', 3), ('U', 3), ('cnot', 2, 3),
+#  ('U', 3), ('U', 3), ('rc3x', 0, 1, 2, 3)]
+```
+
 > ## QuantumCircuit.`probabilities`(*round=3*)
 
 *Returns probabilitiy of the qubits within the quantum circuit.*
 
 ### Parameters:
 
 `round (int)` - rounding the probabilities to the nearest `round`
@@ -1567,15 +1611,15 @@
 # [0.+0.j]]
 ```
 
 # Visualizer
 
 *A collection of classes to visualize the quantum circuit*
 
-> ## *class* QC.Visualizer.QSphere(*circuit*)
+> ## *class* QCpy.Visualizer.QSphere(*circuit*)
 
 *Visualizes the quantum circuit as a q-sphere*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
 
@@ -1612,15 +1656,64 @@
 qc.hadamard(0)
 qc.hadamard(1)
 qc.hadamard(2)
 
 sphere_ex = QSphere(qc)
 sphere_ex.makeSphere(save=False, show=True)
 ```
-> ## *class* QC.Visualizer.StateVector(*circuit*)
+
+> ## *class* QC.Visualizer.BlochSphere(*circuit*)
+
+*Visualizes the quantum state of a single qubit as a sphere*
+
+### Parameters:
+
+`circuit` - the quantum circuit
+
+### Attributes:
+
+`None`
+
+> ## BlochSphere.`makeSphere`(*show_bit=0*, *path="qsphere.png"*, *save=True*, *show=True*, *darkmode=True*)
+
+*Returns a Bloch Sphere that plots the quantum state of a single qubit in a 3D global view*
+
+### Parameters:
+
+`show_bit (int)` - the qubit on the circuit to be visualized, initialized as the 0th bit
+
+`path (str)` - name of the image to be saved
+
+`save (bool)` - pass True for the graph to be saved
+
+`show (bool)` - pass True for the sphere to be shown instead of saved
+
+`darkmode (bool)` - pass True for darkmode, false for lightmode
+
+### Returns:
+
+`None`
+
+### Example:
+
+```python
+from QCpy import QuantumCircuit
+from QCpy.Visualizer import *
+
+qc = QuantumCircuit(3)
+
+qc.hadamard(0)
+qc.hadamard(1)
+qc.hadamard(2)
+
+sphere_ex = BlochSphere(qc)
+sphere_ex.makeSphere(show_bit=1, save=False, show=True)
+```
+
+> ## *class* QCpy.Visualizer.StateVector(*circuit*)
 
 *Visualizes the quantum circuit's quantum amplitutes using a bar graph*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
 
@@ -1658,15 +1751,15 @@
 qc.hadamard(1)
 qc.hadamard(2)
 
 stateVector_ex = StateVector(qc)
 stateVector_ex.makeGraph(save=False, show=True)
 ```
 
-> ## *class* QC.Visualizer.Probabilities(*circuit*)
+> ## *class* QCpy.Visualizer.Probabilities(*circuit*)
 
 *Visualizes the quantum circuit's qubits probability of being measured using a bar graph*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
```

### Comparing `QCpython-1.0.2/README.md` & `QCpython-1.0.3/QCpython.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,44 @@
+Metadata-Version: 2.1
+Name: QCpython
+Version: 1.0.3
+Summary: QCpy is a comprehensive and user-friendly library for quantum computing, providing a wide range of functionality for quantum algorithms and quantum circuits. It is built on using open-source libraries NumPy and Matplotlib; compatible with Python 3.
+Home-page: https://github.com/QCpython/QCpy
+Author: Brennan Freeze, Paris Osuch, Aundre Barras, Soren Richenberg, Suzanne Rivoire
+Author-email: freezebrennan@gmail.com, osuch@sonoma.edu, barras@sonoma.edu, richenbe@sonoma.edu, rivoire@sonoma.edu
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # README.md
 
 # QCpy - A Quantum Computing Library for Python
 
 QCpy is an open source python library and collaborative project for flexible simulations and visualizations of quantum circuits. Designed by college students with students in mind, this library contains a powerful set of tools to teach computer scientists about the emerging discipline of quantum computing (QC).
 
+You can download the package using pip:
+
+```txt
+pip install QCpython
+```
+
 ## Recommended Resources on Quantum Computing:
 
 - [Microsoft’s Linear Algebra for Quantum Computing](https://learn.microsoft.com/en-us/azure/quantum/overview-algebra-for-quantum-computing)
 - [IBM’s Quantum Computing: a field guide](https://quantum-computing.ibm.com/composer/docs/iqx/guide/)
 - [Wikipedia: Quantum Computing](https://en.wikipedia.org/wiki/Quantum_computing)
 
 ---
 
 # Qubits
 
-> ## *class* QC.Qubit.`Qubit`(*initial_state=’z’*)
+> ## *class* QCpy.`Qubit`(*initial_state=’z’*)
 
 *Object representation of a qubit.*
 
 ### Parameters:
 
 `initial_state (chr)` - Character input for starting direction in the *x*, *y*, or *z* axis.
 
@@ -90,15 +110,15 @@
 `None`
 
 ### Attributes:
 
 `matrix (np.ndarray)` - matrix representation of Pauli-Z gate.
 
 ```python
-PauliY.matrix = [1+0j, 0+0j], 
+PauliZ.matrix = [1+0j, 0+0j], 
                 [0+0j, -1+0j]
 ```
 
 > ## *class* QC.QuantumGate.`Hadamard`()
 
 *Maps the basis states |0> to |+> and |1> to |->, creating a superposition state if given a computation basis state.*
 
@@ -446,15 +466,15 @@
 Cz.matrix = [1+0j, 0+0j, 0+0j, 0+0j],
             [0+0j, 1+0j, 0+0j, 0+0j],
             [0+0j, 0+0j, 1+0j, 0+0j],
             [0+0j, 0+0j, 0+0j, -1+0j]
 ```
 ---
 # Quantum Circuit
-> ## *class* QC.QuantumCircuit.`QuantumCircuit`(*qubits*, *little_endian=False*, *prep='z'*)
+> ## *class* QCpy.`QuantumCircuit`(*qubits*, *little_endian=False*, *prep='z'*)
 
 *Quantum circuit that represents the state of a quantum system and performs operations on select qubits.*
 
 ### Parameters:
 
 `qubits (int)` - number of qubits in the circuit.
 
@@ -585,14 +605,48 @@
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.   +0.j]
 # [0.707+0.j]]
 ```
 
+> ## QuantumCircuit.`circuitQueue()`
+
+*Returns queue of gates on quantum circuit.*
+
+### Parameters:
+
+`None`
+
+### Returns:
+`queue (list)` - list of gates queued on quantum circuit.
+
+### Example:
+
+```python
+from QCpy import QuantumCircuit
+
+qc = QuantumCircuit(4)
+
+qc.x(0)
+qc.x(1)
+qc.x(2)
+qc.rc3x(0, 1, 2, 3)
+
+print(qc.circuitQueue())
+
+# [('X', 0), ('X', 1), ('X', 2), ('U', 3), ('U', 3), ('cnot', 2, # 3), ('U', 3), ('U', 3), ('swap', 2, 3), ('swap', 1, 2), 
+# ('swap', 1, 2), ('swap', 2, 3), ('cnot', 0, 3), ('U', 3),
+# ('swap', 2, 3), ('swap', 2, 3), ('cnot', 1, 3), ('U', 3), 
+# ('swap', 2, 3), ('swap', 1, 2), ('swap', 1, 2), ('swap', 2, 
+# 3), ('cnot', 0, 3), ('U', 3), ('swap', 2, 3), ('swap', 2, 3),
+#  ('cnot', 1, 3), ('U', 3), ('U', 3), ('U', 3), ('cnot', 2, 3),
+#  ('U', 3), ('U', 3), ('rc3x', 0, 1, 2, 3)]
+```
+
 > ## QuantumCircuit.`probabilities`(*round=3*)
 
 *Returns probabilitiy of the qubits within the quantum circuit.*
 
 ### Parameters:
 
 `round (int)` - rounding the probabilities to the nearest `round`
@@ -1557,15 +1611,15 @@
 # [0.+0.j]]
 ```
 
 # Visualizer
 
 *A collection of classes to visualize the quantum circuit*
 
-> ## *class* QC.Visualizer.QSphere(*circuit*)
+> ## *class* QCpy.Visualizer.QSphere(*circuit*)
 
 *Visualizes the quantum circuit as a q-sphere*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
 
@@ -1602,15 +1656,64 @@
 qc.hadamard(0)
 qc.hadamard(1)
 qc.hadamard(2)
 
 sphere_ex = QSphere(qc)
 sphere_ex.makeSphere(save=False, show=True)
 ```
-> ## *class* QC.Visualizer.StateVector(*circuit*)
+
+> ## *class* QC.Visualizer.BlochSphere(*circuit*)
+
+*Visualizes the quantum state of a single qubit as a sphere*
+
+### Parameters:
+
+`circuit` - the quantum circuit
+
+### Attributes:
+
+`None`
+
+> ## BlochSphere.`makeSphere`(*show_bit=0*, *path="qsphere.png"*, *save=True*, *show=True*, *darkmode=True*)
+
+*Returns a Bloch Sphere that plots the quantum state of a single qubit in a 3D global view*
+
+### Parameters:
+
+`show_bit (int)` - the qubit on the circuit to be visualized, initialized as the 0th bit
+
+`path (str)` - name of the image to be saved
+
+`save (bool)` - pass True for the graph to be saved
+
+`show (bool)` - pass True for the sphere to be shown instead of saved
+
+`darkmode (bool)` - pass True for darkmode, false for lightmode
+
+### Returns:
+
+`None`
+
+### Example:
+
+```python
+from QCpy import QuantumCircuit
+from QCpy.Visualizer import *
+
+qc = QuantumCircuit(3)
+
+qc.hadamard(0)
+qc.hadamard(1)
+qc.hadamard(2)
+
+sphere_ex = BlochSphere(qc)
+sphere_ex.makeSphere(show_bit=1, save=False, show=True)
+```
+
+> ## *class* QCpy.Visualizer.StateVector(*circuit*)
 
 *Visualizes the quantum circuit's quantum amplitutes using a bar graph*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
 
@@ -1648,15 +1751,15 @@
 qc.hadamard(1)
 qc.hadamard(2)
 
 stateVector_ex = StateVector(qc)
 stateVector_ex.makeGraph(save=False, show=True)
 ```
 
-> ## *class* QC.Visualizer.Probabilities(*circuit*)
+> ## *class* QCpy.Visualizer.Probabilities(*circuit*)
 
 *Visualizes the quantum circuit's qubits probability of being measured using a bar graph*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
```

### Comparing `QCpython-1.0.2/test/test_03.py` & `QCpython-1.0.3/test/quantumcircuit/test_qc_10.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,45 @@
 from QCpy import QuantumCircuit
 import numpy as np
 
+
 def inc(x):
-    qc = QuantumCircuit(qubits = x, little_endian = True, prep = 'z')
+    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
     for i in range(x):
-        qc.hadamard(i)  
+        qc.hadamard(i)
     for i in range(x):
-        qc.t(i)
+        qc.tdg(i)
     return qc.state()
 
-def test_03a():
-    assert (inc(1) == np.array([ 0.707+0j, 0.5+0.5j ], 'F').reshape(2, 1)).all(), "test_03a Failed"
-def test_03b():
-    assert (inc(2) == np.array([ 0.5+0j, 0.354+0.354j, 0.354+0.354j, 0+0.5j ], 'F').reshape(4, 1)).all(), "test_03b Failed"
-def test_03c():
-    assert (inc(3) == np.array([ 0.354+0j, 0.25+0.25j, 0.25+0.25j, 0+0.354j, 0.25+0.25j, 0+0.354j, 0+0.354j, -0.25+0.25j ], 'F').reshape(8, 1)).all(), "test_03c Failed"
-def test_03d():
-    assert (inc(4) == np.array([ 0.25+0j, 0.177+0.177j, 0.177+0.177j, 0+0.25j, 0.177+0.177j, 0+0.25j, 0+0.25j, -0.177+0.177j, 0.177+0.177j, 0+0.25j, 0+0.25j, -0.177+0.177j, 0+0.25j, -0.177+0.177j, -0.177+0.177j, -0.25+0j ], 'F').reshape(16, 1)).all(), "test_03d Failed"
+
+def test_10a():
+    assert (
+        inc(1) == np.array([0.707 + 0j, 0.5 - 0.5j], 'F').reshape(2, 1)
+    ).all(), "test_10a Failed on hadamard -> tdg"
+
+
+def test_10b():
+    assert (
+        inc(2) == np.array([
+            0.5 + 0j, 0.354 - 0.354j, 0.354 - 0.354j, 0 - 0.5j
+        ], 'F').reshape(4, 1)
+    ).all(), "test_10b Failed on hadamard -> tdg"
+
+
+def test_10c():
+    assert (
+        inc(3) == np.array([
+            0.354 + 0j, 0.25 - 0.25j, 0.25 - 0.25j, 0 - 0.354j,
+            0.25 - 0.25j, 0 - 0.354j, 0 - 0.354j, -0.25 - 0.25j
+        ], 'F').reshape(8, 1)
+    ).all(), "test_10c Failed on hadamard -> tdg"
+
+
+def test_10d():
+    assert (
+        inc(4) == np.array([
+            0.25 + 0j, 0.177 - 0.177j, 0.177 - 0.177j, 0 - 0.25j,
+            0.177 - 0.177j, 0 - 0.25j, 0 - 0.25j, -0.177 - 0.177j,
+            0.177 - 0.177j, 0 - 0.25j, 0 - 0.25j, -0.177 - 0.177j,
+            0 - 0.25j, -0.177 - 0.177j, -0.177 - 0.177j, -0.25 + 0j
+        ], 'F').reshape(16, 1)
+    ).all(), "test_10d Failed on hadamard -> tdg"
```

