# Comparing `tmp/OSFResearchClient-0.1.tar.gz` & `tmp/OSFResearchClient-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OSFResearchClient-0.1.tar", last modified: Sun Apr 30 19:33:52 2023, max compression
+gzip compressed data, was "OSFResearchClient-0.2.tar", last modified: Sun Apr 30 19:51:37 2023, max compression
```

## Comparing `OSFResearchClient-0.1.tar` & `OSFResearchClient-0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 manan      (501) staff       (20)        0 2023-04-30 19:33:52.641315 OSFResearchClient-0.1/
-drwxr-xr-x   0 manan      (501) staff       (20)        0 2023-04-30 19:33:52.634837 OSFResearchClient-0.1/OSFResearchClient.egg-info/
--rw-r--r--   0 manan      (501) staff       (20)      174 2023-04-30 19:33:52.000000 OSFResearchClient-0.1/OSFResearchClient.egg-info/PKG-INFO
--rw-r--r--   0 manan      (501) staff       (20)      229 2023-04-30 19:33:52.000000 OSFResearchClient-0.1/OSFResearchClient.egg-info/SOURCES.txt
--rw-r--r--   0 manan      (501) staff       (20)        1 2023-04-30 19:33:52.000000 OSFResearchClient-0.1/OSFResearchClient.egg-info/dependency_links.txt
--rw-r--r--   0 manan      (501) staff       (20)        9 2023-04-30 19:33:52.000000 OSFResearchClient-0.1/OSFResearchClient.egg-info/requires.txt
--rw-r--r--   0 manan      (501) staff       (20)        7 2023-04-30 19:33:52.000000 OSFResearchClient-0.1/OSFResearchClient.egg-info/top_level.txt
--rw-r--r--   0 manan      (501) staff       (20)      174 2023-04-30 19:33:52.641077 OSFResearchClient-0.1/PKG-INFO
-drwxr-xr-x   0 manan      (501) staff       (20)        0 2023-04-30 19:33:52.640208 OSFResearchClient-0.1/client/
--rw-r--r--   0 manan      (501) staff       (20)     6084 2023-04-30 18:48:49.000000 OSFResearchClient-0.1/client/client.py
--rw-r--r--   0 manan      (501) staff       (20)       38 2023-04-30 19:33:52.641392 OSFResearchClient-0.1/setup.cfg
--rw-r--r--   0 manan      (501) staff       (20)      232 2023-04-30 19:33:41.000000 OSFResearchClient-0.1/setup.py
+drwxr-xr-x   0 manan      (501) staff       (20)        0 2023-04-30 19:51:37.616894 OSFResearchClient-0.2/
+drwxr-xr-x   0 manan      (501) staff       (20)        0 2023-04-30 19:51:37.616162 OSFResearchClient-0.2/OSFResearchClient.egg-info/
+-rw-r--r--   0 manan      (501) staff       (20)      174 2023-04-30 19:51:37.000000 OSFResearchClient-0.2/OSFResearchClient.egg-info/PKG-INFO
+-rw-r--r--   0 manan      (501) staff       (20)      248 2023-04-30 19:51:37.000000 OSFResearchClient-0.2/OSFResearchClient.egg-info/SOURCES.txt
+-rw-r--r--   0 manan      (501) staff       (20)        1 2023-04-30 19:51:37.000000 OSFResearchClient-0.2/OSFResearchClient.egg-info/dependency_links.txt
+-rw-r--r--   0 manan      (501) staff       (20)        9 2023-04-30 19:51:37.000000 OSFResearchClient-0.2/OSFResearchClient.egg-info/requires.txt
+-rw-r--r--   0 manan      (501) staff       (20)        7 2023-04-30 19:51:37.000000 OSFResearchClient-0.2/OSFResearchClient.egg-info/top_level.txt
+-rw-r--r--   0 manan      (501) staff       (20)      174 2023-04-30 19:51:37.616706 OSFResearchClient-0.2/PKG-INFO
+drwxr-xr-x   0 manan      (501) staff       (20)        0 2023-04-30 19:51:37.616468 OSFResearchClient-0.2/client/
+-rw-r--r--   0 manan      (501) staff       (20)       26 2023-04-30 19:51:16.000000 OSFResearchClient-0.2/client/__init__.py
+-rw-r--r--   0 manan      (501) staff       (20)     6084 2023-04-30 18:48:49.000000 OSFResearchClient-0.2/client/client.py
+-rw-r--r--   0 manan      (501) staff       (20)       38 2023-04-30 19:51:37.616958 OSFResearchClient-0.2/setup.cfg
+-rw-r--r--   0 manan      (501) staff       (20)      232 2023-04-30 19:51:32.000000 OSFResearchClient-0.2/setup.py
```

### Comparing `OSFResearchClient-0.1/client/client.py` & `OSFResearchClient-0.2/client/client.py`

 * *Files identical despite different names*

