# Comparing `tmp/EC521_malice_package1-0.1.macosx-10.9-universal2.tar.gz` & `tmp/EC521_malice_package1-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EC521_malice_package1-0.1.macosx-10.9-universal2.tar", last modified: Sun Apr 30 02:53:33 2023, max compression
+gzip compressed data, was "EC521_malice_package1-0.2.tar", last modified: Sun Apr 30 21:18:16 2023, max compression
```

## Comparing `EC521_malice_package1-0.1.macosx-10.9-universal2.tar` & `EC521_malice_package1-0.2.tar`

### file list

```diff
@@ -1,14 +1,9 @@
-drwxr-xr-x   0 noam_met   (501) staff       (20)        0 2023-04-30 02:53:33.486580 ./
-drwxr-xr-x   0 noam_met   (501) staff       (20)        0 2023-04-30 02:53:33.486609 ./Library/
-drwxr-xr-x   0 noam_met   (501) staff       (20)        0 2023-04-30 02:53:33.486640 ./Library/Frameworks/
-drwxr-xr-x   0 noam_met   (501) staff       (20)        0 2023-04-30 02:53:33.486672 ./Library/Frameworks/Python.framework/
-drwxr-xr-x   0 noam_met   (501) staff       (20)        0 2023-04-30 02:53:33.486701 ./Library/Frameworks/Python.framework/Versions/
-drwxr-xr-x   0 noam_met   (501) staff       (20)        0 2023-04-30 02:53:33.486730 ./Library/Frameworks/Python.framework/Versions/3.10/
-drwxr-xr-x   0 noam_met   (501) staff       (20)        0 2023-04-30 02:53:33.486763 ./Library/Frameworks/Python.framework/Versions/3.10/lib/
-drwxr-xr-x   0 noam_met   (501) staff       (20)        0 2023-04-30 02:53:33.486794 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/
-drwxr-xr-x   0 noam_met   (501) staff       (20)        0 2023-04-30 02:53:33.486903 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/
-drwxr-xr-x   0 noam_met   (501) staff       (20)        0 2023-04-30 02:53:33.487577 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/EC521_malice_package1-0.1-py3.10.egg-info/
--rw-r--r--   0 noam_met   (501) staff       (20)       63 2023-04-30 02:53:33.437937 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/EC521_malice_package1-0.1-py3.10.egg-info/PKG-INFO
--rw-r--r--   0 noam_met   (501) staff       (20)      188 2023-04-30 02:53:33.444109 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/EC521_malice_package1-0.1-py3.10.egg-info/SOURCES.txt
--rw-r--r--   0 noam_met   (501) staff       (20)        1 2023-04-30 02:53:33.438063 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/EC521_malice_package1-0.1-py3.10.egg-info/dependency_links.txt
--rw-r--r--   0 noam_met   (501) staff       (20)        1 2023-04-30 02:53:33.438409 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/EC521_malice_package1-0.1-py3.10.egg-info/top_level.txt
+drwxr-xr-x   0 noam_met   (501) staff       (20)        0 2023-04-30 21:18:16.720287 EC521_malice_package1-0.2/
+drwxr-xr-x   0 noam_met   (501) staff       (20)        0 2023-04-30 21:18:16.719946 EC521_malice_package1-0.2/EC521_malice_package1.egg-info/
+-rw-r--r--   0 noam_met   (501) staff       (20)       63 2023-04-30 21:18:16.000000 EC521_malice_package1-0.2/EC521_malice_package1.egg-info/PKG-INFO
+-rw-r--r--   0 noam_met   (501) staff       (20)      188 2023-04-30 21:18:16.000000 EC521_malice_package1-0.2/EC521_malice_package1.egg-info/SOURCES.txt
+-rw-r--r--   0 noam_met   (501) staff       (20)        1 2023-04-30 21:18:16.000000 EC521_malice_package1-0.2/EC521_malice_package1.egg-info/dependency_links.txt
+-rw-r--r--   0 noam_met   (501) staff       (20)        1 2023-04-30 21:18:16.000000 EC521_malice_package1-0.2/EC521_malice_package1.egg-info/top_level.txt
+-rw-r--r--   0 noam_met   (501) staff       (20)       63 2023-04-30 21:18:16.720112 EC521_malice_package1-0.2/PKG-INFO
+-rw-r--r--   0 noam_met   (501) staff       (20)       38 2023-04-30 21:18:16.720340 EC521_malice_package1-0.2/setup.cfg
+-rw-r--r--   0 noam_met   (501) staff       (20)      209 2023-04-30 21:16:48.000000 EC521_malice_package1-0.2/setup.py
```

