# Comparing `tmp/bam-core-2023.4.30.1682823045.tar.gz` & `tmp/bam-core-2023.4.30.1682823612.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bam-core-2023.4.30.1682823045.tar", last modified: Sun Apr 30 02:50:46 2023, max compression
+gzip compressed data, was "bam-core-2023.4.30.1682823612.tar", last modified: Sun Apr 30 03:00:13 2023, max compression
```

## Comparing `bam-core-2023.4.30.1682823045.tar` & `bam-core-2023.4.30.1682823612.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 02:50:46.183879 bam-core-2023.4.30.1682823045/
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-30 02:50:46.183879 bam-core-2023.4.30.1682823045/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      671 2023-04-30 02:50:19.000000 bam-core-2023.4.30.1682823045/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 02:50:46.183879 bam-core-2023.4.30.1682823045/bam_core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 02:50:19.000000 bam-core-2023.4.30.1682823045/bam_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-30 02:50:45.000000 bam-core-2023.4.30.1682823045/bam_core/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)      986 2023-04-30 02:50:19.000000 bam-core-2023.4.30.1682823045/bam_core/function.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 02:50:46.183879 bam-core-2023.4.30.1682823045/bam_core/lib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 02:50:19.000000 bam-core-2023.4.30.1682823045/bam_core/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2592 2023-04-30 02:50:19.000000 bam-core-2023.4.30.1682823045/bam_core/lib/airtable.py
--rw-r--r--   0 runner    (1001) docker     (122)     6410 2023-04-30 02:50:19.000000 bam-core-2023.4.30.1682823045/bam_core/lib/listmonk.py
--rw-r--r--   0 runner    (1001) docker     (122)    14799 2023-04-30 02:50:19.000000 bam-core-2023.4.30.1682823045/bam_core/lib/s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-04-30 02:50:19.000000 bam-core-2023.4.30.1682823045/bam_core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 02:50:46.183879 bam-core-2023.4.30.1682823045/bam_core/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 02:50:19.000000 bam-core-2023.4.30.1682823045/bam_core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      913 2023-04-30 02:50:19.000000 bam-core-2023.4.30.1682823045/bam_core/utils/etc.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 02:50:19.000000 bam-core-2023.4.30.1682823045/bam_core/utils/phone.py
--rw-r--r--   0 runner    (1001) docker     (122)     6008 2023-04-30 02:50:19.000000 bam-core-2023.4.30.1682823045/bam_core/utils/serde.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 02:50:46.183879 bam-core-2023.4.30.1682823045/bam_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-30 02:50:46.000000 bam-core-2023.4.30.1682823045/bam_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      516 2023-04-30 02:50:46.000000 bam-core-2023.4.30.1682823045/bam_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-30 02:50:46.000000 bam-core-2023.4.30.1682823045/bam_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-04-30 02:50:46.000000 bam-core-2023.4.30.1682823045/bam_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-30 02:50:46.000000 bam-core-2023.4.30.1682823045/bam_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-30 02:50:46.183879 bam-core-2023.4.30.1682823045/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      597 2023-04-30 02:50:19.000000 bam-core-2023.4.30.1682823045/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 02:50:46.183879 bam-core-2023.4.30.1682823045/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 02:50:19.000000 bam-core-2023.4.30.1682823045/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      393 2023-04-30 02:50:19.000000 bam-core-2023.4.30.1682823045/tests/test_security.py
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-30 02:50:19.000000 bam-core-2023.4.30.1682823045/tests/test_serde.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:00:13.365269 bam-core-2023.4.30.1682823612/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-30 03:00:13.365269 bam-core-2023.4.30.1682823612/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      671 2023-04-30 02:59:46.000000 bam-core-2023.4.30.1682823612/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:00:13.361269 bam-core-2023.4.30.1682823612/bam_core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 02:59:46.000000 bam-core-2023.4.30.1682823612/bam_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-30 03:00:12.000000 bam-core-2023.4.30.1682823612/bam_core/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      986 2023-04-30 02:59:46.000000 bam-core-2023.4.30.1682823612/bam_core/function.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:00:13.365269 bam-core-2023.4.30.1682823612/bam_core/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 02:59:46.000000 bam-core-2023.4.30.1682823612/bam_core/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2592 2023-04-30 02:59:46.000000 bam-core-2023.4.30.1682823612/bam_core/lib/airtable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6410 2023-04-30 02:59:46.000000 bam-core-2023.4.30.1682823612/bam_core/lib/listmonk.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14799 2023-04-30 02:59:46.000000 bam-core-2023.4.30.1682823612/bam_core/lib/s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-04-30 02:59:46.000000 bam-core-2023.4.30.1682823612/bam_core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:00:13.365269 bam-core-2023.4.30.1682823612/bam_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 02:59:46.000000 bam-core-2023.4.30.1682823612/bam_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-04-30 02:59:46.000000 bam-core-2023.4.30.1682823612/bam_core/utils/etc.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 02:59:46.000000 bam-core-2023.4.30.1682823612/bam_core/utils/phone.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6008 2023-04-30 02:59:46.000000 bam-core-2023.4.30.1682823612/bam_core/utils/serde.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:00:13.361269 bam-core-2023.4.30.1682823612/bam_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-30 03:00:13.000000 bam-core-2023.4.30.1682823612/bam_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-04-30 03:00:13.000000 bam-core-2023.4.30.1682823612/bam_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-30 03:00:13.000000 bam-core-2023.4.30.1682823612/bam_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-04-30 03:00:13.000000 bam-core-2023.4.30.1682823612/bam_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-30 03:00:13.000000 bam-core-2023.4.30.1682823612/bam_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-30 03:00:13.365269 bam-core-2023.4.30.1682823612/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-04-30 02:59:46.000000 bam-core-2023.4.30.1682823612/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:00:13.365269 bam-core-2023.4.30.1682823612/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 02:59:46.000000 bam-core-2023.4.30.1682823612/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-04-30 02:59:46.000000 bam-core-2023.4.30.1682823612/tests/test_security.py
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-30 02:59:46.000000 bam-core-2023.4.30.1682823612/tests/test_serde.py
```

### Comparing `bam-core-2023.4.30.1682823045/README.md` & `bam-core-2023.4.30.1682823612/README.md`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.30.1682823045/bam_core/function.py` & `bam-core-2023.4.30.1682823612/bam_core/function.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.30.1682823045/bam_core/lib/airtable.py` & `bam-core-2023.4.30.1682823612/bam_core/lib/airtable.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.30.1682823045/bam_core/lib/listmonk.py` & `bam-core-2023.4.30.1682823612/bam_core/lib/listmonk.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.30.1682823045/bam_core/lib/s3.py` & `bam-core-2023.4.30.1682823612/bam_core/lib/s3.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.30.1682823045/bam_core/settings.py` & `bam-core-2023.4.30.1682823612/bam_core/settings.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.30.1682823045/bam_core/utils/etc.py` & `bam-core-2023.4.30.1682823612/bam_core/utils/etc.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.30.1682823045/bam_core/utils/serde.py` & `bam-core-2023.4.30.1682823612/bam_core/utils/serde.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.30.1682823045/bam_core.egg-info/SOURCES.txt` & `bam-core-2023.4.30.1682823612/bam_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.30.1682823045/setup.py` & `bam-core-2023.4.30.1682823612/setup.py`

 * *Files identical despite different names*

