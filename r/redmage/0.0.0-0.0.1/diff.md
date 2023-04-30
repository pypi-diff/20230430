# Comparing `tmp/redmage-0.0.0.tar.gz` & `tmp/redmage-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redmage-0.0.0.tar", last modified: Tue Mar 21 01:03:16 2023, max compression
+gzip compressed data, was "redmage-0.0.1.tar", max compression
```

## Comparing `redmage-0.0.0.tar` & `redmage-0.0.1.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-03-21 01:03:16.261165 redmage-0.0.0/
--rw-r--r--   0 scott     (1000) scott     (1000)     1060 2023-03-21 00:59:06.000000 redmage-0.0.0/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)      417 2023-03-21 01:03:16.260164 redmage-0.0.0/PKG-INFO
--rw-r--r--   0 scott     (1000) scott     (1000)        9 2023-03-21 01:01:14.000000 redmage-0.0.0/README.md
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-03-21 01:03:16.259225 redmage-0.0.0/redmage.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)      417 2023-03-21 01:03:15.000000 redmage-0.0.0/redmage.egg-info/PKG-INFO
--rw-r--r--   0 scott     (1000) scott     (1000)      150 2023-03-21 01:03:15.000000 redmage-0.0.0/redmage.egg-info/SOURCES.txt
--rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-03-21 01:03:15.000000 redmage-0.0.0/redmage.egg-info/dependency_links.txt
--rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-03-21 01:03:15.000000 redmage-0.0.0/redmage.egg-info/top_level.txt
--rw-r--r--   0 scott     (1000) scott     (1000)       38 2023-03-21 01:03:16.261422 redmage-0.0.0/setup.cfg
--rw-r--r--   0 scott     (1000) scott     (1000)      622 2023-03-21 01:01:00.000000 redmage-0.0.0/setup.py
+-rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.0.1/LICENSE
+-rw-r--r--   0        0        0    14529 2023-04-29 20:46:36.265033 redmage-0.0.1/README.md
+-rw-r--r--   0        0        0      624 2023-04-30 18:54:33.311489 redmage-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-04-21 18:11:35.917318 redmage-0.0.1/redmage/__init__.py
+-rw-r--r--   0        0        0     6079 2023-04-30 17:53:11.381924 redmage-0.0.1/redmage/components.py
+-rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.0.1/redmage/convertors.py
+-rw-r--r--   0        0        0     6966 2023-04-30 16:16:06.542830 redmage-0.0.1/redmage/core.py
+-rw-r--r--   0        0        0     9605 2023-04-30 17:34:15.446362 redmage-0.0.1/redmage/elements.py
+-rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.0.1/redmage/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.0.1/redmage/py.typed
+-rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.0.1/redmage/targets.py
+-rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.0.1/redmage/triggers.py
+-rw-r--r--   0        0        0      936 2023-04-04 02:55:52.571857 redmage-0.0.1/redmage/types.py
+-rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.0.1/redmage/utils.py
+-rw-r--r--   0        0        0    15230 1970-01-01 00:00:00.000000 redmage-0.0.1/PKG-INFO
```

### Comparing `redmage-0.0.0/LICENSE` & `redmage-0.0.1/LICENSE`

 * *Files identical despite different names*

