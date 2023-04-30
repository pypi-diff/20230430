# Comparing `tmp/bam-core-2023.4.29.1682791290.tar.gz` & `tmp/bam-core-2023.4.30.1682822740.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bam-core-2023.4.29.1682791290.tar", last modified: Sat Apr 29 18:02:11 2023, max compression
+gzip compressed data, was "bam-core-2023.4.30.1682822740.tar", last modified: Sun Apr 30 02:45:40 2023, max compression
```

## Comparing `bam-core-2023.4.29.1682791290.tar` & `bam-core-2023.4.30.1682822740.tar`

### file list

```diff
@@ -1,32 +1,30 @@
-drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 18:02:11.221729 bam-core-2023.4.29.1682791290/
--rw-r--r--   0 music      (501) staff       (20)       43 2023-04-29 13:48:13.000000 bam-core-2023.4.29.1682791290/MANIFEST.in
--rw-r--r--   0 music      (501) staff       (20)      203 2023-04-29 18:02:11.221161 bam-core-2023.4.29.1682791290/PKG-INFO
--rw-r--r--   0 music      (501) staff       (20)       62 2023-04-29 02:17:40.000000 bam-core-2023.4.29.1682791290/README.md
-drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 18:02:11.211547 bam-core-2023.4.29.1682791290/bam_core/
--rw-r--r--   0 music      (501) staff       (20)        0 2023-04-29 15:27:50.000000 bam-core-2023.4.29.1682791290/bam_core/__init__.py
--rw-r--r--   0 music      (501) staff       (20)       32 2023-04-29 18:01:30.000000 bam-core-2023.4.29.1682791290/bam_core/__version__.py
--rw-r--r--   0 music      (501) staff       (20)      893 2023-04-29 17:49:06.000000 bam-core-2023.4.29.1682791290/bam_core/function.py
-drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 18:02:11.216611 bam-core-2023.4.29.1682791290/bam_core/lib/
--rw-r--r--   0 music      (501) staff       (20)        0 2023-04-28 21:39:14.000000 bam-core-2023.4.29.1682791290/bam_core/lib/__init__.py
--rw-r--r--   0 music      (501) staff       (20)     2559 2023-04-29 14:10:51.000000 bam-core-2023.4.29.1682791290/bam_core/lib/airtable.py
--rw-r--r--   0 music      (501) staff       (20)     6410 2023-04-29 02:40:34.000000 bam-core-2023.4.29.1682791290/bam_core/lib/listmonk.py
--rw-r--r--   0 music      (501) staff       (20)    14799 2023-04-29 13:48:13.000000 bam-core-2023.4.29.1682791290/bam_core/lib/s3.py
--rw-r--r--   0 music      (501) staff       (20)     2199 2023-04-29 14:09:26.000000 bam-core-2023.4.29.1682791290/bam_core/settings.py
-drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 18:02:11.218933 bam-core-2023.4.29.1682791290/bam_core/utils/
--rw-r--r--   0 music      (501) staff       (20)        0 2023-04-28 21:41:46.000000 bam-core-2023.4.29.1682791290/bam_core/utils/__init__.py
--rw-r--r--   0 music      (501) staff       (20)      913 2023-04-28 21:41:46.000000 bam-core-2023.4.29.1682791290/bam_core/utils/etc.py
--rw-r--r--   0 music      (501) staff       (20)        0 2023-04-28 21:41:46.000000 bam-core-2023.4.29.1682791290/bam_core/utils/phone.py
--rw-r--r--   0 music      (501) staff       (20)     6007 2023-04-29 02:21:08.000000 bam-core-2023.4.29.1682791290/bam_core/utils/serde.py
-drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 18:02:11.214660 bam-core-2023.4.29.1682791290/bam_core.egg-info/
--rw-r--r--   0 music      (501) staff       (20)      203 2023-04-29 18:02:11.000000 bam-core-2023.4.29.1682791290/bam_core.egg-info/PKG-INFO
--rw-r--r--   0 music      (501) staff       (20)      545 2023-04-29 18:02:11.000000 bam-core-2023.4.29.1682791290/bam_core.egg-info/SOURCES.txt
--rw-r--r--   0 music      (501) staff       (20)        1 2023-04-29 18:02:11.000000 bam-core-2023.4.29.1682791290/bam_core.egg-info/dependency_links.txt
--rw-r--r--   0 music      (501) staff       (20)       60 2023-04-29 18:02:11.000000 bam-core-2023.4.29.1682791290/bam_core.egg-info/requires.txt
--rw-r--r--   0 music      (501) staff       (20)       15 2023-04-29 18:02:11.000000 bam-core-2023.4.29.1682791290/bam_core.egg-info/top_level.txt
--rw-r--r--   0 music      (501) staff       (20)       59 2023-04-29 15:42:42.000000 bam-core-2023.4.29.1682791290/requirements.txt
--rw-r--r--   0 music      (501) staff       (20)       38 2023-04-29 18:02:11.221849 bam-core-2023.4.29.1682791290/setup.cfg
--rw-r--r--   0 music      (501) staff       (20)      598 2023-04-29 02:48:20.000000 bam-core-2023.4.29.1682791290/setup.py
-drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 18:02:11.220661 bam-core-2023.4.29.1682791290/tests/
--rw-r--r--   0 music      (501) staff       (20)        0 2023-04-29 02:31:15.000000 bam-core-2023.4.29.1682791290/tests/__init__.py
--rw-r--r--   0 music      (501) staff       (20)      392 2023-04-29 14:51:43.000000 bam-core-2023.4.29.1682791290/tests/test_security.py
--rw-r--r--   0 music      (501) staff       (20)      201 2023-04-29 14:51:43.000000 bam-core-2023.4.29.1682791290/tests/test_serde.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 02:45:40.323376 bam-core-2023.4.30.1682822740/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-30 02:45:40.323376 bam-core-2023.4.30.1682822740/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      656 2023-04-30 02:45:18.000000 bam-core-2023.4.30.1682822740/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 02:45:40.319376 bam-core-2023.4.30.1682822740/bam_core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 02:45:18.000000 bam-core-2023.4.30.1682822740/bam_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-30 02:45:40.000000 bam-core-2023.4.30.1682822740/bam_core/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      986 2023-04-30 02:45:18.000000 bam-core-2023.4.30.1682822740/bam_core/function.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 02:45:40.323376 bam-core-2023.4.30.1682822740/bam_core/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 02:45:18.000000 bam-core-2023.4.30.1682822740/bam_core/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2592 2023-04-30 02:45:18.000000 bam-core-2023.4.30.1682822740/bam_core/lib/airtable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6410 2023-04-30 02:45:18.000000 bam-core-2023.4.30.1682822740/bam_core/lib/listmonk.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14799 2023-04-30 02:45:18.000000 bam-core-2023.4.30.1682822740/bam_core/lib/s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-04-30 02:45:18.000000 bam-core-2023.4.30.1682822740/bam_core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 02:45:40.323376 bam-core-2023.4.30.1682822740/bam_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 02:45:18.000000 bam-core-2023.4.30.1682822740/bam_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-04-30 02:45:18.000000 bam-core-2023.4.30.1682822740/bam_core/utils/etc.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 02:45:18.000000 bam-core-2023.4.30.1682822740/bam_core/utils/phone.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6008 2023-04-30 02:45:18.000000 bam-core-2023.4.30.1682822740/bam_core/utils/serde.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 02:45:40.319376 bam-core-2023.4.30.1682822740/bam_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-30 02:45:40.000000 bam-core-2023.4.30.1682822740/bam_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-04-30 02:45:40.000000 bam-core-2023.4.30.1682822740/bam_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-30 02:45:40.000000 bam-core-2023.4.30.1682822740/bam_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-30 02:45:40.000000 bam-core-2023.4.30.1682822740/bam_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-30 02:45:40.000000 bam-core-2023.4.30.1682822740/bam_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-30 02:45:40.323376 bam-core-2023.4.30.1682822740/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-04-30 02:45:18.000000 bam-core-2023.4.30.1682822740/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 02:45:40.323376 bam-core-2023.4.30.1682822740/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 02:45:18.000000 bam-core-2023.4.30.1682822740/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-04-30 02:45:18.000000 bam-core-2023.4.30.1682822740/tests/test_security.py
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-30 02:45:18.000000 bam-core-2023.4.30.1682822740/tests/test_serde.py
```

### Comparing `bam-core-2023.4.29.1682791290/bam_core/lib/airtable.py` & `bam-core-2023.4.30.1682822740/bam_core/lib/airtable.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from pyairtable import Table, formulas as fx, Api
 
 from bam_core import settings
 
 
 class Airtable(object):
-
     def __init__(
         self,
         base_id: str = settings.AIRTABLE_BASE_ID,
         token: str = settings.AIRTABLE_TOKEN,
     ):
         self.base_id = base_id
         self.token = token
@@ -63,16 +62,18 @@
 
     @property
     def volunteers(self) -> Table:
         return self.get_table(settings.AIRTABLE_VOLUNTEERS_TABLE_NAME)
 
     @property
     def mesh_requests(self):
-        return self.get_view(settings.AIRTABLE_ASSISTANCE_REQUESTS_TABLE_NAME, settings.AIRTABLE_MESH_VIEW_NAME)
-
+        return self.get_view(
+            settings.AIRTABLE_ASSISTANCE_REQUESTS_TABLE_NAME,
+            settings.AIRTABLE_MESH_VIEW_NAME,
+        )
 
     def filter_table(
         self,
         table: Union[str, Table],
         expressions: List[Any],
         match_any: bool = False,
         sort: List[str] = ["-Date Submitted"],
```

### Comparing `bam-core-2023.4.29.1682791290/bam_core/lib/listmonk.py` & `bam-core-2023.4.30.1682822740/bam_core/lib/listmonk.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682791290/bam_core/lib/s3.py` & `bam-core-2023.4.30.1682822740/bam_core/lib/s3.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682791290/bam_core/settings.py` & `bam-core-2023.4.30.1682822740/bam_core/settings.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682791290/bam_core/utils/etc.py` & `bam-core-2023.4.30.1682822740/bam_core/utils/etc.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682791290/bam_core/utils/serde.py` & `bam-core-2023.4.30.1682822740/bam_core/utils/serde.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,14 +245,15 @@
     """
     csv string > obj
     """
     fileobj = io.StringIO(s)
     reader = csv.DictReader(fileobj)
     return [row for row in reader]
 
+
 SERIALIZERS = {
     "json.gz": obj_to_jsongz,
     "json": obj_to_json,
     "pickle": obj_to_pickle,
     "pickle.gz": obj_to_picklegz,
     "zip": str_to_zip,
     "yaml": obj_to_yaml,
```

### Comparing `bam-core-2023.4.29.1682791290/bam_core.egg-info/SOURCES.txt` & `bam-core-2023.4.30.1682822740/bam_core.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-MANIFEST.in
 README.md
-requirements.txt
 setup.py
 bam_core/__init__.py
 bam_core/__version__.py
 bam_core/function.py
 bam_core/settings.py
 bam_core.egg-info/PKG-INFO
 bam_core.egg-info/SOURCES.txt
```

### Comparing `bam-core-2023.4.29.1682791290/setup.py` & `bam-core-2023.4.30.1682822740/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 from setuptools import setup, find_packages
-
 from bam_core.__version__ import VERSION
 
 reqs = os.path.abspath(
     os.path.join(os.path.dirname(__file__), "requirements.txt")
 )
 with open(reqs) as f:
     install_requires = [req.strip().split("==")[0] for req in f]
```

