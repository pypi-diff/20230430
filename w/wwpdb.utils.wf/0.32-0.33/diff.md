# Comparing `tmp/wwpdb.utils.wf-0.32.tar.gz` & `tmp/wwpdb.utils.wf-0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.wf-0.32.tar", last modified: Fri Jan 13 20:53:11 2023, max compression
+gzip compressed data, was "wwpdb.utils.wf-0.33.tar", last modified: Sun Apr 30 13:33:39 2023, max compression
```

## Comparing `wwpdb.utils.wf-0.32.tar` & `wwpdb.utils.wf-0.33.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-01-13 20:53:11.772418 wwpdb.utils.wf-0.32/
--rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      745 2023-01-13 20:53:11.772418 wwpdb.utils.wf-0.32/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      485 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-01-13 20:53:11.772418 wwpdb.utils.wf-0.32/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2105 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-01-13 20:53:11.760418 wwpdb.utils.wf-0.32/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-01-13 20:53:11.764418 wwpdb.utils.wf-0.32/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-01-13 20:53:11.764418 wwpdb.utils.wf-0.32/wwpdb/utils/wf/
--rw-r--r--   0 vsts      (1001) docker     (123)     3228 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/DataSelector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4659 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/DataValueContainer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3661 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/WfDataObject.py
--rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-01-13 20:53:11.768418 wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/
--rw-r--r--   0 vsts      (1001) docker     (123)     6846 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/DbApiUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16004 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/DbCommand.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4025 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/DbConnection.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1946 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/LocalDbApi.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3018 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/StatusDbApi.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1281 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/WFEtime.py
--rw-r--r--   0 vsts      (1001) docker     (123)    47461 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/WfDbApi.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4251 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/WfTracking.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11638 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/dbAPI.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-01-13 20:53:11.768418 wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/
--rw-r--r--   0 vsts      (1001) docker     (123)    59797 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/AnnotationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11877 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/ChemCompUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3611 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/DictUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3595 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/DpUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16297 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/EmUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6274 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/FileUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13301 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/FormatUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    35586 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/NmrUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13901 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/PdbxUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3840 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/PrdSearchUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3427 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/ReportUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5580 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/SFConvert.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5698 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/SeqStatsUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11211 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/SeqdbUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1456 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/UtilsBase.py
--rw-r--r--   0 vsts      (1001) docker     (123)    24021 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/ValidationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-01-13 20:53:11.772418 wwpdb.utils.wf-0.32/wwpdb/utils/wf/process/
--rw-r--r--   0 vsts      (1001) docker     (123)    15842 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/process/ActionRegistry.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7456 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/process/ActionRegistryIo.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11325 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/process/ProcessRunner.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/process/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-01-13 20:53:11.772418 wwpdb.utils.wf-0.32/wwpdb/utils/wf/schema/
--rw-r--r--   0 vsts      (1001) docker     (123)    12006 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/schema/WfSchemaMap.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/schema/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11697 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/schema/database_descriptions.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-01-13 20:52:11.000000 wwpdb.utils.wf-0.32/wwpdb/utils/wf/schema/mandatory_items.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-01-13 20:53:11.764418 wwpdb.utils.wf-0.32/wwpdb.utils.wf.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      745 2023-01-13 20:53:11.000000 wwpdb.utils.wf-0.32/wwpdb.utils.wf.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1724 2023-01-13 20:53:11.000000 wwpdb.utils.wf-0.32/wwpdb.utils.wf.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-01-13 20:53:11.000000 wwpdb.utils.wf-0.32/wwpdb.utils.wf.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-01-13 20:52:59.000000 wwpdb.utils.wf-0.32/wwpdb.utils.wf.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-01-13 20:53:11.000000 wwpdb.utils.wf-0.32/wwpdb.utils.wf.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-01-13 20:53:11.000000 wwpdb.utils.wf-0.32/wwpdb.utils.wf.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:33:39.764764 wwpdb.utils.wf-0.33/
+-rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      745 2023-04-30 13:33:39.764764 wwpdb.utils.wf-0.33/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      485 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-04-30 13:33:39.764764 wwpdb.utils.wf-0.33/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2105 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:33:39.752764 wwpdb.utils.wf-0.33/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:33:39.756764 wwpdb.utils.wf-0.33/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:33:39.760764 wwpdb.utils.wf-0.33/wwpdb/utils/wf/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3229 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/DataSelector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4658 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/DataValueContainer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3661 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/WfDataObject.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:33:39.760764 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6846 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/DbApiUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16002 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/DbCommand.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4025 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/DbConnection.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1946 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/LocalDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3018 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/StatusDbApi.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1281 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/WFEtime.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    47456 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/WfDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4251 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/WfTracking.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11637 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/dbAPI.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:33:39.764764 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/
+-rw-r--r--   0 vsts      (1001) docker     (123)    59795 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/AnnotationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11876 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/ChemCompUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3611 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/DictUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3595 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/DpUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16296 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/EmUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6275 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/FileUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13301 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/FormatUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    50817 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/NmrUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13901 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/PdbxUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3840 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/PrdSearchUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3427 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/ReportUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5580 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/SFConvert.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5698 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/SeqStatsUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11212 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/SeqdbUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1456 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/UtilsBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    24022 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/ValidationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:33:39.764764 wwpdb.utils.wf-0.33/wwpdb/utils/wf/process/
+-rw-r--r--   0 vsts      (1001) docker     (123)    15843 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/process/ActionRegistry.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7456 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/process/ActionRegistryIo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11325 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/process/ProcessRunner.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/process/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:33:39.764764 wwpdb.utils.wf-0.33/wwpdb/utils/wf/schema/
+-rw-r--r--   0 vsts      (1001) docker     (123)    12006 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/schema/WfSchemaMap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/schema/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11697 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/schema/database_descriptions.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/schema/mandatory_items.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:33:39.756764 wwpdb.utils.wf-0.33/wwpdb.utils.wf.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      745 2023-04-30 13:33:39.000000 wwpdb.utils.wf-0.33/wwpdb.utils.wf.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1724 2023-04-30 13:33:39.000000 wwpdb.utils.wf-0.33/wwpdb.utils.wf.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-30 13:33:39.000000 wwpdb.utils.wf-0.33/wwpdb.utils.wf.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-30 13:33:29.000000 wwpdb.utils.wf-0.33/wwpdb.utils.wf.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-04-30 13:33:39.000000 wwpdb.utils.wf-0.33/wwpdb.utils.wf.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-04-30 13:33:39.000000 wwpdb.utils.wf-0.33/wwpdb.utils.wf.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.wf-0.32/LICENSE` & `wwpdb.utils.wf-0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/PKG-INFO` & `wwpdb.utils.wf-0.33/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.wf
-Version: 0.32
+Version: 0.33
 Summary: OneDep WF status DB access utilities
 Home-page: https://github.com/rcsb/py-wwpdb_utils_wf
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.wf-0.32/setup.py` & `wwpdb.utils.wf-0.33/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/DataSelector.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/DataSelector.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,17 +79,17 @@
             return False
 
     def getSelectAttributeList(self):
         """Get the list attributes for the current selection"""
         return self.__targetAttributeList
 
     def addSelectCondition(self, attributeName, attributeValue, comparisonOp="equal"):
-        """Add a selection contition to the current selection.
+        """Add a selection condition to the current selection.
 
-        A selction condition contains the following:
+        A selection condition contains the following:
         - attributeName in the target category.
         - attributeValue
         - one of the comparison operators (equals, ...)
 
         Returns:
 
         True for success or False otherwise.
```

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/DataValueContainer.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/DataValueContainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Creative Commons Attribution 3.0 Unported"
 __version__ = "V0.01"
 
 from datetime import datetime, date
 
-# For python 2/3 compatible comparsigon with isinstace
+# For python 2/3 compatible comparison with isinstace
 from builtins import str
 
 
 class DataValueContainer(object):
 
     """Container for data values.
```

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/WfDataObject.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/WfDataObject.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/DbApiUtil.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/DbApiUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/DbCommand.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/DbCommand.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                     if v == "None" or v is None:
                         c = " %s is NULL " % (attribDict[k])
                     else:
                         c = " %s = '%s' " % (attribDict[k], v)
                     ld.append(c)
 
                 elif k == "EXTERNAL_TABLE":
-                    # "EXTERNAL_TABLE" is special designed for SQL syntex
+                    # "EXTERNAL_TABLE" is special designed for SQL syntax
                     # like " column in (select column from another table)"
                     c = "  %s " % (v)
                     ld.append(c)
                 else:
                     if self.__verbose:
                         self.__lfh.write("DbCommand::makeSqlConstraint(): Warning -- %s is not defined in the database.\n" % (k))
                 if len(ld) > 0:
@@ -164,15 +164,15 @@
                     elif len(c) == 2 and str(c[0]).upper() == "LOGOP" and str(c[1]).upper() in self.__logOps:  # noqa: W504
                         constraint += " %s " % str(c[1]).upper()
                     else:
                         if self.__lfh:
                             self.__lfh.write("Constraint error: %s\n" % str(c))
 
         else:
-            #           Just ignore if contraints are entered as None
+            #           Just ignore if constraints are entered as None
             #           if(self.__verbose):
             self.__lfh.write("DbCommand::makeSqlConstraint(): Warning -- constraint type error: %s\n" % str(cType))
 
         return constraint
 
     def makeOrderStr(self, orderList):
         """
@@ -208,15 +208,15 @@
             #            curs.execute("set autocommit=1")
             #            curs.close()
             self.dbState = e.args[0]
             return None
 
     def runSelectSQL(self, query):
         """
-        method to run a SQL query : no checking - just a convience method to
+        method to run a SQL query : no checking - just a simple method to
         get things working
         note that this does not use attrib list = but returns a list of lists.
         """
         returnList = []
 
         if self.__debug:
             self.__lfh.write("\n+DbCommand.runSelectSQL - input query %r\n" % query)
@@ -258,15 +258,15 @@
         subject to the conditions in constraintDef and
         sorted by the list of attributes in orderList [(attrib,type),..].
         An optional selectList=[attrib,attrib] can be provided to limit
         the query selection.
 
         ConstraintDef can be a simple of dictionary of key == value pairs
         which are logically AND'd together, or a more general constraint
-        can be contructed using the compact contraint specification list
+        can be constructed using the compact constraint specification list
         decoded in method makeSqlConstraint() above.
 
         Return a <row list or row dictionary>.
         """
         if orderList is None:
             orderList = []
         if selectList is None:
@@ -394,19 +394,19 @@
             self.__lfh.write("DbCommand::update(): SQL command successfully executed.\n")
         curs.close()
 
         return "ok"
 
     def selectCrossTables(self, selectList, sqlJoinStr, orderBy, constraintList, constraintDef=None):
         """
-        This function is specically for some complicate queries. The
+        This function is specially for some complicate queries. The
         "sql join" is used.
 
         Input selectList, sqlJoinStr, orderBy will be
-        specially definded in WfSchemaMap. constraintDict is {}
+        specially defined in WfSchemaMap. constraintDict is {}
 
         Return a list of rows {dictionaries)
 
         """
 
         attribsCsv = ",".join(["%s" % k for k in selectList])
```

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/DbConnection.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/DbConnection.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/LocalDbApi.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/LocalDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/StatusDbApi.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/StatusDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/WFEtime.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/WFEtime.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/WfDbApi.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/WfDbApi.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,14 @@
             else:
                 return ret
 
         # all retries gone bad
         return None
 
     def runSelectSQL(self, sql):
-
         """
         method to run a query
         """
 
         # self.testConnection()
         for retry in range(1, self.__Nretry):
             ret = self.__db.runSelectSQL(sql)
@@ -427,15 +426,14 @@
             return None
 
         else:
             self.__lfh.write("+WfDbApi::updateStatus(): The data object is not the one of deposition, instance, task. Nothing is updated.\n")
             return "code-bad"
 
     def processStatus(self, depID, instID, classID):
-
         """
         status owner of process
         None : this depID/instID/classID does NOT own the current process
         <value> : the status
         """
 
         try:
@@ -452,15 +450,15 @@
             return None
 
     def getReference(self, depId=None, classId=None, instId=None, taskId=None):
         """
         Get a list of reference data from table wf_reference
         An empty id will be treated as None.
 
-        Retrun a rwo list or dictionary (if only one record)
+        Return a row list or dictionary (if only one record)
         """
 
         tableDef = self.__schemaWf[self.__tableList[4]]
         depId = self.checkId(depId)
         classId = self.checkId(classId)
         instId = self.checkId(instId)
         taskId = self.checkId(taskId)
@@ -508,15 +506,15 @@
         """
         Add or update reference record in the table wf_reference
 
         requirement:
         For a deposition level reference,the classId, instId and taskId should be None
         For a class level reference the instId, taskId should be None
         For a instance level reference taskId should be None
-        For a task level reference all ids ahould be Non-null.
+        For a task level reference all ids should be Non-null.
 
 
         """
 
         tableDef = self.__schemaWf[self.__tableList[4]]
         constraintDict = {}
         updateVal = {}
@@ -793,16 +791,16 @@
            AUTHOR_LIST
            SG_CENTER
            ASSESSION_CODE
            RELATIONSHIP
            ASSOCIATED_IDS
            CORRECTIONS ( for Author's Corrections)
            REQ_CITATION ( for entries requested for release)
-           PROBLEM_TYPE ( for Peorblem/Error entries)
-           PROBLEM_DETAILS ( for Peorblem/Error entries)
+           PROBLEM_TYPE ( for Problem/Error entries)
+           PROBLEM_DETAILS ( for Problem/Error entries)
         Level 2:
            deposition.dep_set_id
            deposition.pdb_id
            deposition.status_code
            deposition.author_release_status_code
            deposition.exp_method
            deposition.annotator_initials
@@ -1069,15 +1067,14 @@
             # no instance
             return 1
         else:
             returnId = rDict[self.__idList[2]]
             return int("%s" % returnId[2:]) + 1
 
     def referenceExist(self, depId=None, classId=None, instId=None, taskId=None, hashId=None, hashVal=None):
-
         """
         Check to see if the reference data still exists
 
         """
 
         tableDef = self.__schemaWf[self.__tableList[4]]
         constraintDict = {}
@@ -1139,15 +1136,15 @@
         This method will insert if the data is new, or update if the data exists
 
         Add or update reference record in the table wf_reference
         requirement:
         For a deposition level reference,the classId, instId and taskId should be None
         For a class level reference the instId, taskId should be None
         For a instance level reference taskId should be None
-        For a task level reference all ids ahould be Non-null.
+        For a task level reference all ids should be Non-null.
         """
 
         refExist = self.referenceExist(depId, classId, instId, taskId, hashId, hashVal)
 
         if refExist:
             self.addReference("update", depId, classId, instId, taskId, hashId, hashVal)
         else:
```

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/WfTracking.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/WfTracking.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/dbapi/dbAPI.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/dbAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
     def runUpdateOnOrdinal(self, table=None, ordinal=None, data=None, run=True):
         """
         Very simple update/insert SQL creator base on ordinal
         table = string
         data = values to insert/update
         where clause is hard wired to ordinal (unique) so can only UPDATE
-            a bad ordinal returns 0 rows udpated
+            a bad ordinal returns 0 rows updated
 
         return number of rows updated
         if run = False : returns the SQL
 
         IMPT : all attribute values MUST BE QUOTED if strings
         """
 
@@ -205,25 +205,25 @@
             return False
 
     def runInsertUpdate(self, table=None, depID=None, where=None, data=None, run=True):
         """
         Very simple update/insert SQL creator
         table = string
         data = values to insert/update
-        where clause is hard wired to dep_set_id so can ONLy be used for
-            for tables with unique rows on dep_set_id
-            Ie if the table contains a row with depsetid - then it is update
-                  if not - the data is inserted
+        where clause is hard wired to dep_set_id so can ONLY be used for
+            tables with unique rows on dep_set_id
+            i.e. if the table contains a row with dep_set_id - then it is update
+                 if not - the data is inserted
 
         return number of rows updated
         if run = False : returns the SQL
 
-        if depID is not none - then we test the existance based on depID and the table MUST BE UNIQUE on depID
+        if depID is not none - then we test the existence based on depID and the table MUST BE UNIQUE on depID
           data is added to the row based on the dep_set_id + data
-        if unique is not none - then we test the existance on the synthetic key based on the unique dictionary
+        if unique is not none - then we test the existence on the synthetic key based on the unique dictionary
           data is added to the row based on the where + data
 
 
         IMPT : all attribute values MUST BE QUOTED if strings
         """
 
         if not table:
```

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/AnnotationUtils.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/AnnotationUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Date:    15-Aug-2012
 #
 # Updates:
 #  16-Aug-2012 jdw add dictionary check report
 #  17-Dec-2012 jdw add option to calculation derived categories after solvent adjustment.
 #  26-Jun-2013 jdw add formatCheckPdbxOp() & formatCheckPdbOp()
 #  10-Oct-2013 jdw add miscCheckPdbxOp()
-#  15-Jan-2014 jdw add update the content type for assemlby model files
+#  15-Jan-2014 jdw add update the content type for assembly model files
 #  16-Mar-2014 jdw add specialPositionCheckOp()
 #  11-Jun-2104 jdw ad mergeXyzOp()
 #  11-Jun-2104 tjo modified the check for exit status for mergeXYZop - check last line
 #  14-Sep-2014 jdw add user parameter "deposit" on mergeXyzOp()
 #  14-May-2015 jdw add status load method
 #  20-Jan-2017 ep  add assemblyUpdateDepInfoOp()
 #  15-Feb-2017 ep  add combineCifFilesOp()
@@ -65,15 +65,15 @@
     Current supported operations include:
 
     - Assembly calculations
 
     - Secondary structure
     - Site environment
     - Solvent reorganization
-    - Nucleic acid geometrical features
+    - Nucleic acid geometric features
     - Chemical linkages and cis-peptide linkages
     - Automatic running of mapfix on archive files
     - Automatic lookup of pdbx_database_related
 
     -Various format, dictionary and geometry checks
 
     Each method in this class implements the method calling interface of the
```

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/ChemCompUtils.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/ChemCompUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 class ChemCompUtils(UtilsBase):
     """Utility class to perform file format conversions.
 
     Current supported operations include:
 
     - Chemical component linkage calculation
     - Chemical component assignment
-    - Chemical component instance assignment uppdate
+    - Chemical component instance assignment update
 
     Each method in this class implements the method calling interface of the
     `ProcessRunner()` class.   This interface provides the keyword arguments:
 
     - inputObjectD   dictionary of input objects
     - outputObjectD  dictionary of output objects
     - userParameterD  dictionary of user adjustable parameters
```

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/DictUtils.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/DictUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/DpUtils.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/DpUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/EmUtils.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/EmUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,22 +259,20 @@
         except Exception as _e:  # noqa: F841
             traceback.print_exc(file=self._lfh)
             return False
 
     def mapFixInPlaceCfgOp(self, **kwArgs):
         """execution wrapper for mapfix operations for all maps of a particular type.
 
-        --- using explicit data file selection via configuraton file selection.
+        --- using explicit data file selection via configuration file selection.
 
             map-content-type = one of em-volume, em-mask-volume, em-half-volume, em-additional-volume
             partlist = [1,2,3]
             cmdline-arg-list = ['-voxel ...   ','-voxel .... ','-voxel .... ']
 
-
-
         """
         try:
             (inpObjD, _outObjD, _uD, _pD) = self._getArgs(kwArgs)
             inpCfgPath = inpObjD["src1"].getFilePathReference()
             dataSetId = inpObjD["src1"].getDepositionDataSetId()
             dirPath = inpObjD["src1"].getDirPathReference()
             storageType = inpObjD["src1"].getStorageType()
```

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/FileUtils.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/FileUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             return True
         except Exception as _e:  # noqa: F841
             # if (self._verbose): traceback.print_exc(file=self._lfh)
             return True
 
     def makeDirOp(self, **kwargs):
         """Create the directory path for the file reference in the input object ('src').
-        Set the mode of the directoy according to the value of *mode*.
+        Set the mode of the directory according to the value of *mode*.
 
         Returns:
 
         True for success or False otherwise.
 
         """
         try:
```

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/FormatUtils.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/FormatUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/NmrUtils.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/NmrUtils.py`

 * *Files 18% similar despite different names*

```diff
@@ -66,31 +66,34 @@
 
     def __init__(self, verbose=False, log=sys.stderr):
         super(NmrUtils, self).__init__(verbose, log)
         self.__cleanUp = True
         """Flag to remove any temporary directories created by this class.
         """
         #
-
-    def ccpnExtractOp(self, **kwArgs):  # pylint: disable=unused-argument
-        """Extract PDB and NMRSTAR files from CCPn project"""
-
-        # Disabled as not python3 compatible
-        if self._verbose:
-            self._lfh.write("+NmrUtils.ccpnExtractOp() - DISABLED\n")
-        return False
-
+    # """
+    # @obsolete: DAOTHER-7407: ccpnExtractOp() has never been implemented before
+    # def ccpnExtractOp(self, **kwArgs):  # pylint: disable=unused-argument
+    #     """Extract PDB and NMRSTAR files from CCPn project
+    #     """
+    #
+    #     # Disabled as not python3 compatible
+    #     if self._verbose:
+    #         self._lfh.write("+NmrUtils.ccpnExtractOp() - DISABLED\n")
+    #     return False
+    # """
     def uploadChemicalShiftOp(self, **kwArgs):
         """Performs format check on a list of chemical shift files and concatenates these.
 
         Data sections are assigned to user provided input names corresponding to each input file.
 
         Output is a concatenated chemical shift file,  text status (ok,warning,error) and text list of
         warnings and/or errors.
 
+        @deprecated: since V5.18 (DAOTHER-7407)
         """
         try:
             (inpObjD, outObjD, _uD, _pD) = self._getArgs(kwArgs)
             csPathList = inpObjD["src1"].getValue()
             nameList = inpObjD["src2"].getValue()
             #
             csOutPath = outObjD["dst1"].getFilePathReference()
@@ -140,33 +143,32 @@
     def uploadChemicalShiftAltOp(self, **kwArgs):
         """Performs format check on a list of chemical shift files and concatenates these.
 
         Data sections are assigned to user provided input names corresponding to each input file.
 
         Output is a concatenated chemical shift file, and check report file -
 
+        @deprecated: since V5.18 (DAOTHER-7407)
         """
         try:
             (inpObjD, outObjD, _uD, _pD) = self._getArgs(kwArgs)
             csPathList = []
             csPathListFilePath = inpObjD["src1"].getFilePathReference()
             nameList = []
             nameListFilePath = inpObjD["src2"].getFilePathReference()
             #
-            ifh = open(csPathListFilePath, "r")
-            for tline in ifh:
-                txt = str(tline[:-1]).strip()
-                csPathList.append(txt)
-            ifh.close()
-            #
-            ifh = open(nameListFilePath, "r")
-            for tline in ifh:
-                txt = str(tline[:-1]).strip()
-                nameList.append(txt)
-            ifh.close()
+            with open(csPathListFilePath, "r") as ifh:
+                for tline in ifh:
+                    txt = str(tline[:-1]).strip()
+                    csPathList.append(txt)
+            #
+            with open(nameListFilePath, "r") as ifh:
+                for tline in ifh:
+                    txt = str(tline[:-1]).strip()
+                    nameList.append(txt)
             #
             csOutPath = outObjD["dst1"].getFilePathReference()
             dirPath = outObjD["dst1"].getDirPathReference()
             chkPath = outObjD["dst2"].getFilePathReference()
 
             logPath = os.path.join(dirPath, "upload-chemical-shift-check.log")
             #
@@ -195,14 +197,15 @@
             traceback.print_exc(file=self._lfh)
             return False
 
     def atomNameCheckCsXyzOp(self, **kwArgs):
         """Performs nomenclature and format check on input CS and XYZ files and returns an updated CS file, a CIF check report,
         status (text=ok,warning,error), and both  warnings and error messages as a list of strings.
 
+        @deprecated: since V5.18 (DAOTHER-7407)
         """
         try:
             (inpObjD, outObjD, _uD, _pD) = self._getArgs(kwArgs)
             csPath = inpObjD["src1"].getFilePathReference()
             xyzPath = inpObjD["src2"].getFilePathReference()
 
             csOutPath = outObjD["dst1"].getFilePathReference()
@@ -246,14 +249,16 @@
             traceback.print_exc(file=self._lfh)
             return False
 
     def atomNameCheckCsXyzAltOp(self, **kwArgs):
         """Performs nomenclature and format check on input CS and XYZ files and returns an updated CS file, a CIF check report.
 
         * workflow version * returns chemical shift file and check report output --
+
+        @deprecated: since V5.18 (DAOTHER-7407)
         """
         try:
             (inpObjD, outObjD, _uD, _pD) = self._getArgs(kwArgs)
             csPath = inpObjD["src1"].getFilePathReference()
             xyzPath = inpObjD["src2"].getFilePathReference()
 
             csOutPath = outObjD["dst1"].getFilePathReference()
@@ -324,29 +329,29 @@
     #   action: nmr-nef-consistency-check
     #   src0.content: nmr-data-config,      src0.format: json
     #   src1.content: nmr-data-nef,         src1.format: nmr-star
     #   src2.content: model,                src2.format: pdbx
     #   prc2.content: model (deposit),      prc2.format: pdbx
     #   dst.content:  nmr-data-nef-report,  dst.format:  json
     def nefConsistencyCheckOp(self, **kwArgs):
-        """Performs consistency check on input NEF with coordinate and outputs a JSON report file, which provides diagnostic information to depositor.
+        """Performs consistency check on input NEF with the coordinates,
+           then outputs a JSON report file, which provides diagnostic information to depositor.
 
         Returns True for success or False for warnings/errors.
 
         """
         try:
             (inpObjD, outObjD, _uD, _pD) = self._getArgs(kwArgs)
             cnfInpPath = inpObjD["src0"].getFilePathReference()
             nefInpPath = inpObjD["src1"].getFilePathReference()
             cifInpPath = inpObjD["src2"].getFilePathReference()
             prcInpPath = inpObjD["prc2"].getFilePathReference()
             logOutPath = outObjD["dst"].getFilePathReference()
             #
             dp = NmrDpUtility(verbose=self._verbose, log=self._lfh)
-            dp.setVerbose(True)
             dp.setSource(nefInpPath)
             dp.addInput(name="coordinate_file_path", value=cifInpPath, type="file")
             dp.addInput(name="proc_coord_file_path", value=prcInpPath, type="file")
 
             if os.path.exists(cnfInpPath):
 
                 with open(cnfInpPath, "r") as file:
@@ -371,29 +376,29 @@
     #   action: nmr-str-consistency-check
     #   src0.content: nmr-data-config,      src0.format: json
     #   src1.content: nmr-data-str,         src1.format: nmr-star
     #   src2.content: model,                src2.format: pdbx
     #   prc2.content: model (deposit),      prc2.format: pdbx
     #   dst.content:  nmr-data-str-report,  dst.format:  json
     def strConsistencyCheckOp(self, **kwArgs):
-        """Performs consistency check on input NMR-STAR V3.2 with coordinate and outputs a JSON report file, which provides diagnostic information to depositor.
+        """Performs consistency check on input NMR-STAR V3.2 with the coordinates,
+           then outputs a JSON report file, which provides diagnostic information to depositor.
 
         Returns True for success or False for warnings/errors.
 
         """
         try:
             (inpObjD, outObjD, _uD, _pD) = self._getArgs(kwArgs)
             cnfInpPath = inpObjD["src0"].getFilePathReference()
             strInpPath = inpObjD["src1"].getFilePathReference()
             cifInpPath = inpObjD["src2"].getFilePathReference()
             prcInpPath = inpObjD["prc2"].getFilePathReference()
             logOutPath = outObjD["dst"].getFilePathReference()
             #
             dp = NmrDpUtility(verbose=self._verbose, log=self._lfh)
-            dp.setVerbose(True)
             dp.setSource(strInpPath)
             dp.addInput(name="coordinate_file_path", value=cifInpPath, type="file")
             dp.addInput(name="proc_coord_file_path", value=prcInpPath, type="file")
 
             if os.path.exists(cnfInpPath):
 
                 with open(cnfInpPath, "r") as file:
@@ -418,29 +423,30 @@
     #   action: nmr-cs-str-check
     #   src1.content: nmr-cs-path-list,     src1.format: string
     #   src2.content: nmr-mr-path-list,     src2.format: string
     #   src3.content: model,                src3.format: pdbx
     #   prc3.content: model (deposit),      prc3.format: pdbx
     #   dst.content:  nmr-data-str-report,  dst.format:  json
     def csStrConsistencyCheckOp(self, **kwArgs):
-        """Performs consistency check on input chemical shift/restraint list with coordinate and outputs a JSON report file, which provides diagnostic information to depositor.
+        """Performs consistency check on input chemical shifts/restraints with the coordinates,
+           then outputs a JSON report file, which provides diagnostic information to depositor.
+        @deprecated: Please use csMrMergeOp() for initial file upload since V5.18 (DAOTHER-7407)
 
         Returns True for success or False for warnings/errors.
 
         """
         try:
             (inpObjD, outObjD, _uD, _pD) = self._getArgs(kwArgs)
             csPathList = []
             csPathListFilePath = inpObjD["src1"].getFilePathReference()
             #
-            ifh = open(csPathListFilePath, "r")
-            for tline in ifh:
-                txt = str(tline[:-1]).strip()
-                csPathList.append(txt)
-            ifh.close()
+            with open(csPathListFilePath, "r") as ifh:
+                for tline in ifh:
+                    txt = str(tline[:-1]).strip()
+                    csPathList.append(txt)
             #
             mrPathList = []
             arPathList = []
             mrInpPath = inpObjD["src2"].getFilePathReference()
             #
             if os.path.exists(mrInpPath):
 
@@ -489,15 +495,14 @@
                             arPathList.append({"file_name": mr_file, "file_type": mr_file_type, "original_file_name": mr_orig_file})
             #
             cifInpPath = inpObjD["src3"].getFilePathReference()
             prcInpPath = inpObjD["prc3"].getFilePathReference()
             logOutPath = outObjD["dst"].getFilePathReference()
             #
             dp = NmrDpUtility(verbose=self._verbose, log=self._lfh)
-            dp.setVerbose(True)
             dp.addInput(name="chem_shift_file_path_list", value=csPathList, type="file_list")
             if len(mrPathList) > 0:
                 dp.addInput(name="restraint_file_path_list", value=mrPathList, type="file_list")
             if len(arPathList) > 0:
                 dp.addInput(name="atypical_restraint_file_path_list", value=arPathList, type="file_dict_list")
             dp.addInput(name="coordinate_file_path", value=cifInpPath, type="file")
             dp.addInput(name="proc_coord_file_path", value=prcInpPath, type="file")
@@ -519,27 +524,148 @@
                 self._lfh.write("+NmrUtils.csStrConsistencyCheckOp() - mmCIF input file path:    %s\n" % cifInpPath)
                 self._lfh.write("+NmrUtils.csStrConsistencyCheckOp() - JSON output file path:    %s\n" % logOutPath)
             return stat
         except Exception as _e:  # noqa: F841
             traceback.print_exc(file=self._lfh)
             return False
 
-    # DepUI for NMR unified data: NEF -> NMR-STAR V3.2 conversion and deposition
+    # DepUI for NMR legacy data: Merge chemical shifts and restraints into a single NMR-STAR V3.2 file
+    #   action: nmr-cs-mr-merge
+    #   src1.content: nmr-cs-path-list,           src1.format: string
+    #   src2.content: nmr-cs-auth-file-name-list, src2.format: string
+    #   src3.content: nmr-mr-path-list,           src3.format: json
+    #   src4.content: model,                      src4.format: pdbx
+    #   prc4.content: model (deposit),            prc4.format: pdbx
+    #   dst1.content: nmr-data-str,               dst1.format: nmr-star
+    #   dst2.content:  nmr-data-str-report,       dst2.format: json
+    def csMrMergeOp(self, **kwArgs):
+        """Performs consistency check on input chemical shifts/restraints with the coordinates,
+           then outputs a combined NMR-STAR v3.2 file and a JSON report file, which provides diagnostic information to depositor.
+
+        Returns True for success or False for warnings/errors.
+
+        """
+        try:
+            (inpObjD, outObjD, _uD, _pD) = self._getArgs(kwArgs)
+            csPathList = []
+            csPathListFilePath = inpObjD["src1"].getFilePathReference()
+            csAuthFileNamePath = inpObjD["src2"].getFilePathReference()
+            #
+            with open(csPathListFilePath, "r") as ifh:
+                for tline in ifh:
+                    txt = str(tline[:-1]).strip()
+                    csPathList.append({"file_name": txt, "file_type": "nmr-star"})
+            with open(csAuthFileNamePath, "r") as ifh:
+                for fid, tline in enumerate(ifh):
+                    txt = str(tline[:-1]).strip()
+                    if fid < len(csPathList) and len(txt) > 0:
+                        csPathList[fid]["original_file_name"] = txt
+            #
+            mrPathList = []
+            arPathList = []
+            mrInpPath = inpObjD["src3"].getFilePathReference()
+            #
+            if os.path.exists(mrInpPath):
+
+                with open(mrInpPath, "r") as file:
+                    mr_list = json.loads(file.read())
+
+                datablock_pattern = re.compile(r"\s*data_\S+\s*")
+                sf_anonymous_pattern = re.compile(r"\s*save_\S+\s*")
+                save_pattern = re.compile(r"\s*save_\s*")
+                loop_pattern = re.compile(r"\s*loop_\s*")
+                stop_pattern = re.compile(r"\s*stop_\s*")
+
+                for mr in mr_list:
+                    mr_file = mr["file_name"]
+                    mr_orig_file = mr["original_file_name"]
+                    mr_file_type = mr["file_type"]
+
+                    # mr_orig_file_ext = os.path.splitext(mr_orig_file)[1]
+                    # if (mr_orig_file_ext == '.str' or mr_orig_file_ext == '.nef') and mr_file_type == 'nm-res-oth':
+
+                    if mr_file_type.startswith("nm-res") or mr_file_type.startswith("nm-aux") or mr_file_type.startswith("nm-pea"):
+                        has_datablock = False
+                        has_anonymous_saveframe = False
+                        has_save = False
+                        has_loop = False
+                        has_stop = False
+
+                        with open(mr_file, "r") as ifp:
+                            for line in ifp:
+                                if datablock_pattern.match(line):
+                                    has_datablock = True
+                                elif sf_anonymous_pattern.match(line):
+                                    has_anonymous_saveframe = True
+                                elif save_pattern.match(line):
+                                    has_save = True
+                                elif loop_pattern.match(line):
+                                    has_loop = True
+                                elif stop_pattern.match(line):
+                                    has_stop = True
+
+                            ifp.close()
+
+                        if has_datablock or has_anonymous_saveframe or has_save or has_loop or has_stop:  # NMR-STAR or NEF (DAOTHER-6830)
+                            mrPathList.append(mr_file)
+                        else:
+                            arPathList.append({"file_name": mr_file, "file_type": mr_file_type, "original_file_name": mr_orig_file})
+            #
+            cifInpPath = inpObjD["src4"].getFilePathReference()
+            prcInpPath = inpObjD["prc4"].getFilePathReference()
+            strOutPath = outObjD["dst1"].getFilePathReference()
+            logOutPath = outObjD["dst2"].getFilePathReference()
+            #
+            dp = NmrDpUtility(verbose=self._verbose, log=self._lfh)
+            dp.addInput(name="chem_shift_file_path_list", value=csPathList, type="file_dict_list")
+            if len(mrPathList) > 0:
+                dp.addInput(name="restraint_file_path_list", value=mrPathList, type="file_list")
+            if len(arPathList) > 0:
+                dp.addInput(name="atypical_restraint_file_path_list", value=arPathList, type="file_dict_list")
+            dp.addInput(name="coordinate_file_path", value=cifInpPath, type="file")
+            dp.addInput(name="proc_coord_file_path", value=prcInpPath, type="file")
+
+            dp.addInput(name="nonblk_anomalous_cs", value=True, type="param")
+            dp.addInput(name="nonblk_bad_nterm", value=True, type="param")
+            dp.addInput(name="resolve_conflict", value=True, type="param")
+            dp.addInput(name="check_mandatory_tag", value=False, type="param")
+            dp.addInput(name="merge_any_pk_as_is", value=True, type="param")  # DAOTHER-7407 enabled until Phase 2 release
+
+            dp.setDestination(strOutPath)
+            dp.setLog(logOutPath)
+            stat = dp.op("nmr-cs-mr-merge")
+            #
+            if self._verbose:
+                self._lfh.write("+NmrUtils.csMrMergeOp() - CS file path list:          %s\n" % csPathList)
+                if len(mrPathList) > 0:
+                    self._lfh.write("+NmrUtils.csMrMergeOp() - MR file path list:          %s\n" % mrPathList)
+                if len(arPathList) > 0:
+                    self._lfh.write("+NmrUtils.csMrMergeOp() - AR file path list:          %s\n" % arPathList)
+                self._lfh.write("+NmrUtils.csMrMergeOp() - mmCIF input file path:      %s\n" % cifInpPath)
+                self._lfh.write("+NmrUtils.csMrMergeOp() - NMR-STAR output file path:  %s\n" % strOutPath)
+                self._lfh.write("+NmrUtils.csMrMergeOp() - JSON output file path:      %s\n" % logOutPath)
+            return stat
+        except Exception as _e:  # noqa: F841
+            traceback.print_exc(file=self._lfh)
+            return False
+
+    # DepUI for NMR unified data: NEF -> NMR-STAR V3.2 file conversion and deposition
     #   action: nmr-nef2str-deposit
     #   src0.content: nmr-data-config,      src0.format: json
     #   src1.content: nmr-data-nef,         src1.format: nmr-star
     #   src2.content: model,                src2.format: pdbx
     #   prc2.content: model (deposit),      prc2.format: pdbx
     #   src3.content: nmr-data-nef-report,  src3.format: json
     #   dst1.content: nmr-data-nef,         dst1.format: nmr-star
     #   dst2.content: nmr-data-str,         dst2.format: nmr-star
     #   dst3.content: nmr-data-nef-report,  dst3.format: json
     #   dst4.content: nmr-data-str-report,  dst4.format: json
     def nef2strDepositOp(self, **kwArgs):
-        """Perform NEF to NMR-STAR V3.2 format conversion operation (special processing for deposition sessions)
+        """Perform NEF to NMR-STAR V3.2 file conversion
+        @deprecated: Please use nef2cifDepositOp() for initial file upload since V5.18 (DAOTHER-7407)
 
         Returns True for success or False for warnings/errors.
 
         """
         try:
             (inpObjD, outObjD, _uD, _pD) = self._getArgs(kwArgs)
             cnfInpPath = inpObjD["src0"].getFilePathReference()
@@ -549,15 +675,14 @@
             logInpPath = inpObjD["src3"].getFilePathReference()
             nefOutPath = outObjD["dst1"].getFilePathReference()
             strOutPath = outObjD["dst2"].getFilePathReference()
             logOutPath1 = outObjD["dst3"].getFilePathReference()
             logOutPath2 = outObjD["dst4"].getFilePathReference()
             #
             dp = NmrDpUtility(verbose=self._verbose, log=self._lfh)
-            dp.setVerbose(True)
             dp.setSource(nefInpPath)
             dp.addInput(name="coordinate_file_path", value=cifInpPath, type="file")
             dp.addInput(name="proc_coord_file_path", value=prcInpPath, type="file")
             dp.addInput(name="report_file_path", value=logInpPath, type="file")
 
             if os.path.exists(cnfInpPath):
 
@@ -576,33 +701,112 @@
             stat = dp.op("nmr-nef2str-deposit")
             #
             if self._verbose:
                 self._lfh.write("+NmrUtils.nef2strDepositOp() - NEF input file path:        %s\n" % nefInpPath)
                 self._lfh.write("+NmrUtils.nef2strDepositOp() - mmCIF input file path:      %s\n" % cifInpPath)
                 self._lfh.write("+NmrUtils.nef2strDepositOp() - JSON input file path:       %s\n" % logInpPath)
                 self._lfh.write("+NmrUtils.nef2strDepositOp() - NEF output file path:       %s\n" % nefOutPath)
-                self._lfh.write("+NmrUtils.nef2strDepositOp() - NMR-STAR V3.2 file path:    %s\n" % strOutPath)
+                self._lfh.write("+NmrUtils.nef2strDepositOp() - NMR-STAR output file path:  %s\n" % strOutPath)
                 self._lfh.write("+NmrUtils.nef2strDepositOp() - JSON output file path 1:    %s\n" % logOutPath1)
                 self._lfh.write("+NmrUtils.nef2strDepositOp() - JSON output file path 2:    %s\n" % logOutPath2)
             return stat
         except Exception as _e:  # noqa: F841
             traceback.print_exc(file=self._lfh)
             return False
 
-    # DepUI for NMR unified data: NMR-STAR V3.2 conversion and deposition
+    # DepUI for NMR unified data: NEF -> CIF formated NMR-STAR V3.2 file conversion and deposition
+    #   action: nmr-nef2cif-deposit
+    #   src0.content: nmr-data-config,            src0.format: json
+    #   src1.content: nmr-data-nef,               src1.format: nmr-star
+    #   src2.content: nmr-cs-auth-file-name-list, src2.format: string
+    #   src3.content: model,                      src3.format: pdbx
+    #   prc3.content: model (deposit),            prc3.format: pdbx
+    #   src4.content: nmr-data-nef-report,        src4.format: json
+    #   dst1.content: nmr-data-nef,               dst1.format: nmr-star
+    #   dst2.content: nmr-data-str,               dst2.format: nmr-star
+    #   dst3.content: nmr-data-str,               dst3.format: pdbx
+    #   dst4.content: nmr-data-nef-report,        dst4.format: json
+    #   dst5.content: nmr-data-str-report,        dst5.format: json
+    def nef2cifDepositOp(self, **kwArgs):
+        """Perform NEF to CIF formated NMR-STAR V3.2 file conversion
+
+        Returns True for success or False for warnings/errors.
+
+        """
+        try:
+            (inpObjD, outObjD, _uD, _pD) = self._getArgs(kwArgs)
+            cnfInpPath = inpObjD["src0"].getFilePathReference()
+            nefInpPath = inpObjD["src1"].getFilePathReference()
+            authFileNamePath = inpObjD["src2"].getFilePathReference()
+            cifInpPath = inpObjD["src3"].getFilePathReference()
+            prcInpPath = inpObjD["prc3"].getFilePathReference()
+            logInpPath = inpObjD["src4"].getFilePathReference()
+            nefOutPath = outObjD["dst1"].getFilePathReference()
+            strOutPath = outObjD["dst2"].getFilePathReference()
+            s2cOutPath = outObjD["dst3"].getFilePathReference()
+            logOutPath1 = outObjD["dst4"].getFilePathReference()
+            logOutPath2 = outObjD["dst5"].getFilePathReference()
+            #
+            originalFileName = None
+            with open(authFileNamePath, "r") as ifh:
+                for tline in ifh:
+                    originalFileName = str(tline[:-1]).strip()
+                    if len(originalFileName) == 0:
+                        originalFileName = None
+                    break
+            #
+            dp = NmrDpUtility(verbose=self._verbose, log=self._lfh)
+            dp.setSource(nefInpPath, originalFileName)
+            dp.addInput(name="coordinate_file_path", value=cifInpPath, type="file")
+            dp.addInput(name="proc_coord_file_path", value=prcInpPath, type="file")
+            dp.addInput(name="report_file_path", value=logInpPath, type="file")
+
+            if os.path.exists(cnfInpPath):
+
+                with open(cnfInpPath, "r") as file:
+                    conf = json.loads(file.read())
+
+                for item in conf.keys():
+                    dp.addInput(name=item, value=conf[item], type="param")
+
+            dp.setDestination(nefOutPath)
+            dp.addOutput(name="nmr-star_file_path", value=strOutPath, type="file")
+            dp.addOutput(name="nmr_cif_file_path", value=s2cOutPath, type="file")
+            dp.addOutput(name="report_file_path", value=logOutPath2, type="file")
+            dp.addOutput(name="insert_entry_id_to_loops", value=True, type="param")
+            dp.addOutput(name="leave_intl_note", value=False, type="param")
+            dp.setLog(logOutPath1)
+            stat = dp.op("nmr-nef2cif-deposit")
+            #
+            if self._verbose:
+                self._lfh.write("+NmrUtils.nef2cifDepositOp() - NEF input file path:               %s\n" % nefInpPath)
+                self._lfh.write("+NmrUtils.nef2cifDepositOp() - mmCIF input file path:             %s\n" % cifInpPath)
+                self._lfh.write("+NmrUtils.nef2cifDepositOp() - JSON input file path:              %s\n" % logInpPath)
+                self._lfh.write("+NmrUtils.nef2cifDepositOp() - NEF output file path:              %s\n" % nefOutPath)
+                self._lfh.write("+NmrUtils.nef2cifDepositOp() - NMR-STAR output file path:         %s\n" % strOutPath)
+                self._lfh.write("+NmrUtils.nef2cifDepositOp() - NMR-STAR in CIF output file path:  %s\n" % s2cOutPath)
+                self._lfh.write("+NmrUtils.nef2cifDepositOp() - JSON output file path 1:           %s\n" % logOutPath1)
+                self._lfh.write("+NmrUtils.nef2cifDepositOp() - JSON output file path 2:           %s\n" % logOutPath2)
+            return stat
+        except Exception as _e:  # noqa: F841
+            traceback.print_exc(file=self._lfh)
+            return False
+
+    # DepUI for NMR unified data: NMR-STAR V3.2 file conversion and deposition
     #   action: nmr-str2str-deposit
     #   src0.content: nmr-data-config,      src0.format: json
     #   src1.content: nmr-data-str,         src1.format: nmr-star
     #   src2.content: model,                src2.format: pdbx
     #   prc2.content: model (deposit),      prc2.format: pdbx
     #   src3.content: nmr-data-str-report,  src3.format: json
     #   dst1.content: nmr-data-str,         dst1.format: nmr-star
     #   dst2.content: nmr-data-str-report,  dst2.format: json
     def str2strDepositOp(self, **kwArgs):
-        """Perform NMR-STAR V3.2 format conversion operation (special processing for deposition sessions)
+        """Perform NMR-STAR V3.2 file conversion
+        @deprecated: Please use str2cifDepositOp() for initial file upload since V5.18 (DAOTHER-7407)
 
         Returns True for success or False for warnings/errors.
 
         """
         try:
             (inpObjD, outObjD, _uD, _pD) = self._getArgs(kwArgs)
             cnfInpPath = inpObjD["src0"].getFilePathReference()
@@ -610,15 +814,14 @@
             cifInpPath = inpObjD["src2"].getFilePathReference()
             prcInpPath = inpObjD["prc2"].getFilePathReference()
             logInpPath = inpObjD["src3"].getFilePathReference()
             strOutPath = outObjD["dst1"].getFilePathReference()
             logOutPath = outObjD["dst2"].getFilePathReference()
             #
             dp = NmrDpUtility(verbose=self._verbose, log=self._lfh)
-            dp.setVerbose(True)
             dp.setSource(strInpPath)
             dp.addInput(name="coordinate_file_path", value=cifInpPath, type="file")
             dp.addInput(name="proc_coord_file_path", value=prcInpPath, type="file")
             dp.addInput(name="report_file_path", value=logInpPath, type="file")
 
             if os.path.exists(cnfInpPath):
 
@@ -631,19 +834,89 @@
             dp.setDestination(strOutPath)
             dp.addOutput(name="insert_entry_id_to_loops", value=True, type="param")
             dp.addOutput(name="leave_intl_note", value=False, type="param")
             dp.setLog(logOutPath)
             stat = dp.op("nmr-str2str-deposit")
             #
             if self._verbose:
-                self._lfh.write("+NmrUtils.str2strDepositOp() - NMR-STAR V3.2 input file path:     %s\n" % strInpPath)
-                self._lfh.write("+NmrUtils.str2strDepositOp() - mmCIF input file path:             %s\n" % cifInpPath)
-                self._lfh.write("+NmrUtils.str2strDepositOp() - JSON input file path:              %s\n" % logInpPath)
-                self._lfh.write("+NmrUtils.str2strDepositOp() - NMR-STAR V3.2 output file path:    %s\n" % strOutPath)
-                self._lfh.write("+NmrUtils.str2strDepositOp() - JSON output file path:             %s\n" % logOutPath)
+                self._lfh.write("+NmrUtils.str2strDepositOp() - NMR-STAR input file path:   %s\n" % strInpPath)
+                self._lfh.write("+NmrUtils.str2strDepositOp() - mmCIF input file path:      %s\n" % cifInpPath)
+                self._lfh.write("+NmrUtils.str2strDepositOp() - JSON input file path:       %s\n" % logInpPath)
+                self._lfh.write("+NmrUtils.str2strDepositOp() - NMR-STAR output file path:  %s\n" % strOutPath)
+                self._lfh.write("+NmrUtils.str2strDepositOp() - JSON output file path:      %s\n" % logOutPath)
+            return stat
+        except Exception as _e:  # noqa: F841
+            traceback.print_exc(file=self._lfh)
+            return False
+
+    # DepUI for NMR unified data: NMR-STAR V3.2 -> CIF file conversion and deposition
+    #   action: nmr-str2cif-deposit
+    #   src0.content: nmr-data-config,            src0.format: json
+    #   src1.content: nmr-data-str,               src1.format: nmr-star
+    #   src2.content: nmr-cs-auth-file-name-list, src2.format: string
+    #   src3.content: model,                      src3.format: pdbx
+    #   prc3.content: model (deposit),            prc3.format: pdbx
+    #   src4.content: nmr-data-str-report,        src4.format: json
+    #   dst1.content: nmr-data-str,               dst1.format: nmr-star
+    #   dst2.content: nmr-data-str,               dst2.format: pdbx
+    #   dst3.content: nmr-data-str-report,        dst3.format: json
+    def str2cifDepositOp(self, **kwArgs):
+        """Perform NMR-STAR V3.2 to CIF file conversion
+
+        Returns True for success or False for warnings/errors.
+
+        """
+        try:
+            (inpObjD, outObjD, _uD, _pD) = self._getArgs(kwArgs)
+            cnfInpPath = inpObjD["src0"].getFilePathReference()
+            strInpPath = inpObjD["src1"].getFilePathReference()
+            authFileNamePath = inpObjD["src2"].getFilePathReference()
+            cifInpPath = inpObjD["src3"].getFilePathReference()
+            prcInpPath = inpObjD["prc3"].getFilePathReference()
+            logInpPath = inpObjD["src4"].getFilePathReference()
+            strOutPath = outObjD["dst1"].getFilePathReference()
+            s2cOutPath = outObjD["dst2"].getFilePathReference()
+            logOutPath = outObjD["dst3"].getFilePathReference()
+            #
+            originalFileName = None
+            with open(authFileNamePath, "r") as ifh:
+                for tline in ifh:
+                    originalFileName = str(tline[:-1]).strip()
+                    if len(originalFileName) == 0:
+                        originalFileName = None
+                    break
+            #
+            dp = NmrDpUtility(verbose=self._verbose, log=self._lfh)
+            dp.setSource(strInpPath, originalFileName)
+            dp.addInput(name="coordinate_file_path", value=cifInpPath, type="file")
+            dp.addInput(name="proc_coord_file_path", value=prcInpPath, type="file")
+            dp.addInput(name="report_file_path", value=logInpPath, type="file")
+
+            if os.path.exists(cnfInpPath):
+
+                with open(cnfInpPath, "r") as file:
+                    conf = json.loads(file.read())
+
+                for item in conf.keys():
+                    dp.addInput(name=item, value=conf[item], type="param")
+
+            dp.setDestination(strOutPath)
+            dp.addOutput(name="nmr_cif_file_path", value=s2cOutPath, type="file")
+            dp.addOutput(name="insert_entry_id_to_loops", value=True, type="param")
+            dp.addOutput(name="leave_intl_note", value=False, type="param")
+            dp.setLog(logOutPath)
+            stat = dp.op("nmr-str2cif-deposit")
+            #
+            if self._verbose:
+                self._lfh.write("+NmrUtils.str2cifDepositOp() - NMR-STAR input file path:          %s\n" % strInpPath)
+                self._lfh.write("+NmrUtils.str2cifDepositOp() - mmCIF input file path:             %s\n" % cifInpPath)
+                self._lfh.write("+NmrUtils.str2cifDepositOp() - JSON input file path:              %s\n" % logInpPath)
+                self._lfh.write("+NmrUtils.str2cifDepositOp() - NMR-STAR output file path:         %s\n" % strOutPath)
+                self._lfh.write("+NmrUtils.str2cifDepositOp() - NMR-STAR in CIF output file path:  %s\n" % s2cOutPath)
+                self._lfh.write("+NmrUtils.str2cifDepositOp() - JSON output file path:             %s\n" % logOutPath)
             return stat
         except Exception as _e:  # noqa: F841
             traceback.print_exc(file=self._lfh)
             return False
 
     # NMR-STAR V3.2 -> NEF conversion and release
     #   action: nmr-str2nef-deposit
@@ -667,15 +940,14 @@
             logOutPath = outObjD["dst0"].getFilePathReference()
             strOutPath = outObjD["dst1"].getFilePathReference()
             nefOutPath = outObjD["dst2"].getFilePathReference()
             logOutPath1 = outObjD["dst3"].getFilePathReference()
             logOutPath2 = outObjD["dst4"].getFilePathReference()
             #
             dp = NmrDpUtility(verbose=self._verbose, log=self._lfh)
-            dp.setVerbose(True)
             dp.setSource(strInpPath)
             dp.addInput(name="coordinate_file_path", value=cifInpPath, type="file")
             dp.addInput(name="nonblk_anomalous_cs", value=True, type="param")
             dp.addInput(name="nonblk_bad_nterm", value=True, type="param")
             dp.addInput(name="resolve_conflict", value=True, type="param")
             dp.addInput(name="check_mandatory_tag", value=True, type="param")
             dp.setLog(logOutPath)
```

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/PdbxUtils.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/PdbxUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/PrdSearchUtils.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/PrdSearchUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/ReportUtils.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/ReportUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Date:    15-Aug-2012
 #
 # Updates:
 #  16-Aug-2012 jdw add dictionary check report
 #  17-Dec-2012 jdw add option to calculation derived categories after solvent adjustment.
 #  26-Jun-2013 jdw add formatCheckPdbxOp() & formatCheckPdbOp()
 #  10-Oct-2013 jdw add miscCheckPdbxOp()
-#  15-Jan-2014 jdw add update the content type for assemlby model files
+#  15-Jan-2014 jdw add update the content type for assembly model files
 #  16-Mar-2014 jdw add specialPositionCheckOp()
 #  11-Jun-2104 jdw ad mergeXyzOp()
 #  11-Jun-2104 tjo modified the check for exit status for mergeXYZop - check last line
 #  14-Sep-2014 jdw add user parameter "deposit" on mergeXyzOp()
 #  14-May-2015 jdw add status load method
 #  20-Jan-2017 ep  add assemblyUpdateDepInfoOp()
 #  15-Feb-2017 ep  add combineCifFilesOp()
```

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/SFConvert.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/SFConvert.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/SeqStatsUtils.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/SeqStatsUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             #
 
         except Exception as _e:  # noqa: F841
             traceback.print_exc(file=self._lfh)
             return False
 
     def updateModelSequenceAssignOp(self, **kwArgs):
-        """Update model coordinate file with aligmnent mapping information.
+        """Update model coordinate file with alignment mapping information.
 
         Returns:
 
         True for success or False otherwise.
 
         """
         try:
```

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/SeqdbUtils.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/SeqdbUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         # self.__sessionPath = None
         self.__doAutoProcessFlag = False
         self.__includeSeqAssignFileFlag = False
         #
 
     def mySetup(self, topSessionPath="."):
         """Setup application environment for managing session storage of
-        temporaty data files.
+        temporally data files.
         """
         self.__maxRefAlign = 100
         self.__siteId = getSiteId(defaultSiteId="WWPDB_DEPOLY_TEST")
         #
         self.__reqObj = SeqModInputRequest({}, verbose=self._verbose, log=self._lfh)
         self.__reqObj.setValue("TopSessionPath", topSessionPath)
         self.__reqObj.setValue("WWPDB_SITE_ID", self.__siteId)
```

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/UtilsBase.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/UtilsBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/plugins/ValidationUtils.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/ValidationUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ##
 # File:    ValidationUtils.py
 # Date:    4-Sep-2012
 #
 # Updates:
 #  4-Sep-2012  jdw add validation report method
 #  13-Dec-2012 jdw added method for version 2 of validation module
-#  15-Jan-2014 jdw add annotation context user paramter to validation report
+#  15-Jan-2014 jdw add annotation context user parameter to validation report
 #  24-Jan-2014 jdw add addition report output options
 #  21-Sep-2014 jdw update validationReportTestOp() for NMR
 #  16-Jan-2015 jdw update validationReportTestOp() to test for experimental files -
 #  22-Mar-2015 jdw add entry_id as parameter in validationReportAltOp
 #  16-Sep-2015 jdw add validationReportAllOp
 #
 #  14-Jul-2016 jdw validationReportAllOp() is the only valid entry point here - all others are deprecated.
```

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/process/ActionRegistry.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/process/ActionRegistry.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
 
 
 class ActionRegistry(object):
 
     """Container and manager class for the registry of supported process actions.
 
-    The action registry has the following internal data orgaization:
+    The action registry has the following internal data organization:
 
     - A dictionary with unique action identifier referencing a dictionary with the following content:
 
       + INPUT_INFO_LIST & OUTPUT_INFO_LIST,  list of required features of the input and out
         data objects stored as tuples of (reference_type, (data_type,container_type), selector_type)
       + USER_PARAMETER_DICTIONARY,  container for user settable parameters passed to
         the action method.
@@ -173,28 +173,28 @@
 
     def setUserParameter(self, actionId, paramKey, paramValue):
         """Set a user adjustable parameter for the input action.  The parameter is
         identifiers by *paramKey* and the value is specified as *paramValue*.
 
         Returns:
 
-        True is the parameter setting was succesful or False otherwise.
+        True is the parameter setting was successful or False otherwise.
 
         """
         try:
             self.__D[actionId]["USER_PARAMETER_DICT"][paramKey] = paramValue
             return True
         except Exception as _e:  # noqa: F841
             return False
 
     def getUserParameter(self, actionId, paramKey):
         """Returns:
 
         The value of a user adjustable parameter for the input action.  The
-        user parameteris identified by the *paramKey*.
+        user parameters identified by the *paramKey*.
 
         """
         try:
             return self.__D[actionId]["USER_PARAMETER_DICT"][paramKey]
         except Exception as _e:  # noqa: F841
             return None
```

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/process/ActionRegistryIo.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/process/ActionRegistryIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/process/ProcessRunner.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/process/ProcessRunner.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/schema/WfSchemaMap.py` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/schema/WfSchemaMap.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb/utils/wf/schema/database_descriptions.txt` & `wwpdb.utils.wf-0.33/wwpdb/utils/wf/schema/database_descriptions.txt`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.32/wwpdb.utils.wf.egg-info/PKG-INFO` & `wwpdb.utils.wf-0.33/wwpdb.utils.wf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.wf
-Version: 0.32
+Version: 0.33
 Summary: OneDep WF status DB access utilities
 Home-page: https://github.com/rcsb/py-wwpdb_utils_wf
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.wf-0.32/wwpdb.utils.wf.egg-info/SOURCES.txt` & `wwpdb.utils.wf-0.33/wwpdb.utils.wf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

