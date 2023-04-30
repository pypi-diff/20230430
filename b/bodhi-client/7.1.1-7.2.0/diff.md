# Comparing `tmp/bodhi_client-7.1.1.tar.gz` & `tmp/bodhi_client-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodhi_client-7.1.1.tar", max compression
+gzip compressed data, was "bodhi_client-7.2.0.tar", max compression
```

## Comparing `bodhi_client-7.1.1.tar` & `bodhi_client-7.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    18018 2022-12-23 15:08:00.000000 bodhi_client-7.1.1/COPYING
--rw-r--r--   0        0        0      935 2022-12-23 15:08:00.000000 bodhi_client-7.1.1/bodhi/client/__init__.py
--rw-r--r--   0        0        0    41042 2022-12-23 15:08:00.000000 bodhi_client-7.1.1/bodhi/client/bindings.py
--rw-r--r--   0        0        0    54744 2023-03-11 13:42:51.000000 bodhi_client-7.1.1/bodhi/client/cli.py
--rw-r--r--   0        0        0      628 2022-12-23 15:08:00.000000 bodhi_client-7.1.1/bodhi/client/constants.py
--rw-r--r--   0        0        0    12718 2022-12-23 15:08:00.000000 bodhi_client-7.1.1/bodhi/client/oidcclient.py
--rwxr-xr-x   0        0        0      236 2022-12-23 15:08:00.000000 bodhi_client-7.1.1/bodhi-client.bash
--rw-r--r--   0        0        0      776 2022-12-23 15:08:00.000000 bodhi_client-7.1.1/docs/Makefile
--rw-r--r--   0        0        0     1115 2022-12-23 15:08:00.000000 bodhi_client-7.1.1/docs/conf.py
--rw-r--r--   0        0        0        0 2022-12-23 15:08:00.000000 bodhi_client-7.1.1/docs/index.rst
--rw-r--r--   0        0        0    18967 2022-12-23 15:08:00.000000 bodhi_client-7.1.1/docs/man_pages/bodhi.rst
--rw-r--r--   0        0        0     1721 2023-03-18 09:15:10.000000 bodhi_client-7.1.1/pyproject.toml
--rw-r--r--   0        0        0       35 2022-12-23 15:08:00.000000 bodhi_client-7.1.1/tests/__init__.py
--rw-r--r--   0        0        0    46000 2022-12-23 15:08:00.000000 bodhi_client-7.1.1/tests/fixtures.py
--rw-r--r--   0        0        0    75076 2023-03-05 14:50:21.000000 bodhi_client-7.1.1/tests/test_bindings.py
--rw-r--r--   0        0        0   119695 2023-03-11 13:42:51.000000 bodhi_client-7.1.1/tests/test_cli.py
--rw-r--r--   0        0        0    15528 2022-12-23 15:08:00.000000 bodhi_client-7.1.1/tests/test_oidcclient.py
--rw-r--r--   0        0        0     2327 2022-12-23 15:08:00.000000 bodhi_client-7.1.1/tests/utils.py
--rw-r--r--   0        0        0     1434 1970-01-01 00:00:00.000000 bodhi_client-7.1.1/PKG-INFO
+-rw-r--r--   0        0        0    18018 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/COPYING
+-rw-r--r--   0        0        0      935 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/bodhi/client/__init__.py
+-rw-r--r--   0        0        0    41042 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/bodhi/client/bindings.py
+-rw-r--r--   0        0        0    54744 2023-04-29 08:18:48.000000 bodhi_client-7.2.0/bodhi/client/cli.py
+-rw-r--r--   0        0        0      628 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/bodhi/client/constants.py
+-rw-r--r--   0        0        0    12718 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/bodhi/client/oidcclient.py
+-rwxr-xr-x   0        0        0      236 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/bodhi-client.bash
+-rw-r--r--   0        0        0      776 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/docs/Makefile
+-rw-r--r--   0        0        0     1115 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/docs/conf.py
+-rw-r--r--   0        0        0        0 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/docs/index.rst
+-rw-r--r--   0        0        0    18967 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/docs/man_pages/bodhi.rst
+-rw-r--r--   0        0        0     1721 2023-04-30 06:59:12.000000 bodhi_client-7.2.0/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/tests/__init__.py
+-rw-r--r--   0        0        0    46000 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/tests/fixtures.py
+-rw-r--r--   0        0        0    75076 2023-04-29 08:18:48.000000 bodhi_client-7.2.0/tests/test_bindings.py
+-rw-r--r--   0        0        0   119695 2023-04-29 08:18:48.000000 bodhi_client-7.2.0/tests/test_cli.py
+-rw-r--r--   0        0        0    15528 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/tests/test_oidcclient.py
+-rw-r--r--   0        0        0     2327 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/tests/utils.py
+-rw-r--r--   0        0        0     1434 1970-01-01 00:00:00.000000 bodhi_client-7.2.0/PKG-INFO
```

### Comparing `bodhi_client-7.1.1/COPYING` & `bodhi_client-7.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.1.1/bodhi/client/__init__.py` & `bodhi_client-7.2.0/bodhi/client/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.1.1/bodhi/client/bindings.py` & `bodhi_client-7.2.0/bodhi/client/bindings.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.1.1/bodhi/client/cli.py` & `bodhi_client-7.2.0/bodhi/client/cli.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.1.1/bodhi/client/constants.py` & `bodhi_client-7.2.0/bodhi/client/constants.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.1.1/bodhi/client/oidcclient.py` & `bodhi_client-7.2.0/bodhi/client/oidcclient.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.1.1/docs/Makefile` & `bodhi_client-7.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.1.1/docs/conf.py` & `bodhi_client-7.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.1.1/docs/man_pages/bodhi.rst` & `bodhi_client-7.2.0/docs/man_pages/bodhi.rst`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.1.1/pyproject.toml` & `bodhi_client-7.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bodhi-client"
-version = "7.1.1"
+version = "7.2.0"
 description = "Bodhi client"
 authors = ["Fedora Infrastructure team"]
 maintainers = ["Fedora Infrastructure Team <infrastructure@lists.fedoraproject.org>"]
 homepage = "https://bodhi.fedoraproject.org/"
 repository = "https://github.com/fedora-infra/bodhi"
 keywords = ["fedora"]
 license = "GPL-2.0-or-later"
```

### Comparing `bodhi_client-7.1.1/tests/fixtures.py` & `bodhi_client-7.2.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.1.1/tests/test_bindings.py` & `bodhi_client-7.2.0/tests/test_bindings.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.1.1/tests/test_cli.py` & `bodhi_client-7.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.1.1/tests/test_oidcclient.py` & `bodhi_client-7.2.0/tests/test_oidcclient.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.1.1/tests/utils.py` & `bodhi_client-7.2.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.1.1/PKG-INFO` & `bodhi_client-7.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodhi-client
-Version: 7.1.1
+Version: 7.2.0
 Summary: Bodhi client
 Home-page: https://bodhi.fedoraproject.org/
 License: GPL-2.0-or-later
 Keywords: fedora
 Author: Fedora Infrastructure team
 Maintainer: Fedora Infrastructure Team
 Maintainer-email: infrastructure@lists.fedoraproject.org
```

