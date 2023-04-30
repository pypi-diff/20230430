# Comparing `tmp/EC521_malice_package1-0.2.tar.gz` & `tmp/EC521_malice_package1-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EC521_malice_package1-0.2.tar", last modified: Sun Apr 30 21:18:16 2023, max compression
+gzip compressed data, was "EC521_malice_package1-0.3.tar", last modified: Sun Apr 30 21:54:49 2023, max compression
```

## Comparing `EC521_malice_package1-0.2.tar` & `EC521_malice_package1-0.3.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxr-xr-x   0 noam_met   (501) staff       (20)        0 2023-04-30 21:18:16.720287 EC521_malice_package1-0.2/
-drwxr-xr-x   0 noam_met   (501) staff       (20)        0 2023-04-30 21:18:16.719946 EC521_malice_package1-0.2/EC521_malice_package1.egg-info/
--rw-r--r--   0 noam_met   (501) staff       (20)       63 2023-04-30 21:18:16.000000 EC521_malice_package1-0.2/EC521_malice_package1.egg-info/PKG-INFO
--rw-r--r--   0 noam_met   (501) staff       (20)      188 2023-04-30 21:18:16.000000 EC521_malice_package1-0.2/EC521_malice_package1.egg-info/SOURCES.txt
--rw-r--r--   0 noam_met   (501) staff       (20)        1 2023-04-30 21:18:16.000000 EC521_malice_package1-0.2/EC521_malice_package1.egg-info/dependency_links.txt
--rw-r--r--   0 noam_met   (501) staff       (20)        1 2023-04-30 21:18:16.000000 EC521_malice_package1-0.2/EC521_malice_package1.egg-info/top_level.txt
--rw-r--r--   0 noam_met   (501) staff       (20)       63 2023-04-30 21:18:16.720112 EC521_malice_package1-0.2/PKG-INFO
--rw-r--r--   0 noam_met   (501) staff       (20)       38 2023-04-30 21:18:16.720340 EC521_malice_package1-0.2/setup.cfg
--rw-r--r--   0 noam_met   (501) staff       (20)      209 2023-04-30 21:16:48.000000 EC521_malice_package1-0.2/setup.py
+drwxr-xr-x   0 noam_met   (501) staff       (20)        0 2023-04-30 21:54:49.970345 EC521_malice_package1-0.3/
+drwxr-xr-x   0 noam_met   (501) staff       (20)        0 2023-04-30 21:54:49.969426 EC521_malice_package1-0.3/EC521_malice_package1.egg-info/
+-rw-r--r--   0 noam_met   (501) staff       (20)       63 2023-04-30 21:54:49.000000 EC521_malice_package1-0.3/EC521_malice_package1.egg-info/PKG-INFO
+-rw-r--r--   0 noam_met   (501) staff       (20)      227 2023-04-30 21:54:49.000000 EC521_malice_package1-0.3/EC521_malice_package1.egg-info/SOURCES.txt
+-rw-r--r--   0 noam_met   (501) staff       (20)        1 2023-04-30 21:54:49.000000 EC521_malice_package1-0.3/EC521_malice_package1.egg-info/dependency_links.txt
+-rw-r--r--   0 noam_met   (501) staff       (20)        1 2023-04-30 21:54:49.000000 EC521_malice_package1-0.3/EC521_malice_package1.egg-info/top_level.txt
+-rw-r--r--   0 noam_met   (501) staff       (20)       12 2023-04-30 21:52:54.000000 EC521_malice_package1-0.3/MANIFEST.in
+-rw-r--r--   0 noam_met   (501) staff       (20)       63 2023-04-30 21:54:49.970211 EC521_malice_package1-0.3/PKG-INFO
+-rw-r--r--   0 noam_met   (501) staff       (20)      931 2023-04-30 03:24:31.000000 EC521_malice_package1-0.3/__init__.py
+-rw-r--r--   0 noam_met   (501) staff       (20)      873 2023-04-30 21:13:20.000000 EC521_malice_package1-0.3/mal-example.py
+-rw-r--r--   0 noam_met   (501) staff       (20)       38 2023-04-30 21:54:49.970389 EC521_malice_package1-0.3/setup.cfg
+-rw-r--r--   0 noam_met   (501) staff       (20)      209 2023-04-30 21:54:46.000000 EC521_malice_package1-0.3/setup.py
```

