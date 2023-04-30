# Comparing `tmp/csle_defender-0.1.9.tar.gz` & `tmp/csle_defender-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_defender-0.1.9.tar", last modified: Tue Mar 21 08:09:34 2023, max compression
+gzip compressed data, was "csle_defender-0.2.0.tar", last modified: Sun Apr 30 12:36:39 2023, max compression
```

## Comparing `csle_defender-0.1.9.tar` & `csle_defender-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:34.737228 csle_defender-0.1.9/
--rw-rw-r--   0 kim       (1000) kim       (1000)      654 2023-03-21 08:09:34.737228 csle_defender-0.1.9/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     3858 2023-01-03 16:53:44.000000 csle_defender-0.1.9/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      673 2023-02-11 20:28:41.000000 csle_defender-0.1.9/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1213 2023-03-21 08:09:34.741228 csle_defender-0.1.9/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2022-11-28 13:03:16.000000 csle_defender-0.1.9/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:34.737228 csle_defender-0.1.9/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:34.737228 csle_defender-0.1.9/src/csle_defender/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2022-11-28 13:03:16.000000 csle_defender-0.1.9/src/csle_defender/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 csle_defender-0.1.9/src/csle_defender/__version__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1197 2022-11-28 13:03:16.000000 csle_defender-0.1.9/src/csle_defender/defender.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:34.737228 csle_defender-0.1.9/src/csle_defender/emulation/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_defender-0.1.9/src/csle_defender/emulation/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1879 2022-11-28 13:03:16.000000 csle_defender-0.1.9/src/csle_defender/emulation/defender_stopping_middleware.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1514 2022-11-28 13:03:16.000000 csle_defender-0.1.9/src/csle_defender/emulation/defender_update_state_middleware.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3034 2022-11-28 13:03:16.000000 csle_defender-0.1.9/src/csle_defender/emulation/emulated_defender.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:34.737228 csle_defender-0.1.9/src/csle_defender.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      654 2023-03-21 08:09:34.000000 csle_defender-0.1.9/src/csle_defender.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      593 2023-03-21 08:09:34.000000 csle_defender-0.1.9/src/csle_defender.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:09:34.000000 csle_defender-0.1.9/src/csle_defender.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:36:05.000000 csle_defender-0.1.9/src/csle_defender.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      177 2023-03-21 08:09:34.000000 csle_defender-0.1.9/src/csle_defender.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       14 2023-03-21 08:09:34.000000 csle_defender-0.1.9/src/csle_defender.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:39.312548 csle_defender-0.2.0/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      654 2023-04-30 12:36:39.312548 csle_defender-0.2.0/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3858 2023-03-28 14:03:22.000000 csle_defender-0.2.0/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      673 2023-03-28 14:03:22.000000 csle_defender-0.2.0/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1213 2023-04-30 12:36:39.312548 csle_defender-0.2.0/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_defender-0.2.0/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:39.308548 csle_defender-0.2.0/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:39.312548 csle_defender-0.2.0/src/csle_defender/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_defender-0.2.0/src/csle_defender/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-04-30 12:35:57.000000 csle_defender-0.2.0/src/csle_defender/__version__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1197 2023-03-28 14:03:22.000000 csle_defender-0.2.0/src/csle_defender/defender.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:39.312548 csle_defender-0.2.0/src/csle_defender/emulation/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_defender-0.2.0/src/csle_defender/emulation/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1879 2023-03-28 14:03:22.000000 csle_defender-0.2.0/src/csle_defender/emulation/defender_stopping_middleware.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1514 2023-03-28 14:03:22.000000 csle_defender-0.2.0/src/csle_defender/emulation/defender_update_state_middleware.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3034 2023-03-28 14:03:22.000000 csle_defender-0.2.0/src/csle_defender/emulation/emulated_defender.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:39.312548 csle_defender-0.2.0/src/csle_defender.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      654 2023-04-30 12:36:38.000000 csle_defender-0.2.0/src/csle_defender.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      593 2023-04-30 12:36:39.000000 csle_defender-0.2.0/src/csle_defender.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-04-30 12:36:38.000000 csle_defender-0.2.0/src/csle_defender.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:36:05.000000 csle_defender-0.2.0/src/csle_defender.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      177 2023-04-30 12:36:39.000000 csle_defender-0.2.0/src/csle_defender.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       14 2023-04-30 12:36:39.000000 csle_defender-0.2.0/src/csle_defender.egg-info/top_level.txt
```

### Comparing `csle_defender-0.1.9/PKG-INFO` & `csle_defender-0.2.0/src/csle_defender.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: csle_defender
-Version: 0.1.9
+Name: csle-defender
+Version: 0.2.0
 Summary: Scripts for emulated defenses in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_defender-0.1.9/README.md` & `csle_defender-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `csle_defender-0.1.9/pyproject.toml` & `csle_defender-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_defender-0.1.9/setup.cfg` & `csle_defender-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-common>=0.1.9
+	csle-common>=0.2.0
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_defender-0.1.9/src/csle_defender/defender.py` & `csle_defender-0.2.0/src/csle_defender/defender.py`

 * *Files identical despite different names*

### Comparing `csle_defender-0.1.9/src/csle_defender/emulation/defender_stopping_middleware.py` & `csle_defender-0.2.0/src/csle_defender/emulation/defender_stopping_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_defender-0.1.9/src/csle_defender/emulation/defender_update_state_middleware.py` & `csle_defender-0.2.0/src/csle_defender/emulation/defender_update_state_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_defender-0.1.9/src/csle_defender/emulation/emulated_defender.py` & `csle_defender-0.2.0/src/csle_defender/emulation/emulated_defender.py`

 * *Files identical despite different names*

### Comparing `csle_defender-0.1.9/src/csle_defender.egg-info/PKG-INFO` & `csle_defender-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: csle-defender
-Version: 0.1.9
+Name: csle_defender
+Version: 0.2.0
 Summary: Scripts for emulated defenses in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_defender-0.1.9/src/csle_defender.egg-info/SOURCES.txt` & `csle_defender-0.2.0/src/csle_defender.egg-info/SOURCES.txt`

 * *Files identical despite different names*

