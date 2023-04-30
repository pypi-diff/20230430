# Comparing `tmp/wwpdb.apps.editormodule-0.16.tar.gz` & `tmp/wwpdb.apps.editormodule-0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.editormodule-0.16.tar", last modified: Mon Nov 14 12:59:30 2022, max compression
+gzip compressed data, was "wwpdb.apps.editormodule-0.17.tar", last modified: Sun Apr 30 13:30:17 2023, max compression
```

## Comparing `wwpdb.apps.editormodule-0.16.tar` & `wwpdb.apps.editormodule-0.17.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-14 12:59:30.776774 wwpdb.apps.editormodule-0.16/
--rw-r--r--   0 vsts      (1001) docker     (121)      552 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/LICENSE
--rwxr-xr-x   0 vsts      (1001) docker     (121)      110 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)      757 2022-11-14 12:59:30.776774 wwpdb.apps.editormodule-0.16/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)       51 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/README.md
--rw-r--r--   0 vsts      (1001) docker     (121)      108 2022-11-14 12:59:30.776774 wwpdb.apps.editormodule-0.16/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (121)     2183 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-14 12:59:30.772773 wwpdb.apps.editormodule-0.16/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (121)       65 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-14 12:59:30.772773 wwpdb.apps.editormodule-0.16/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (121)       65 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-14 12:59:30.772773 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/
--rw-r--r--   0 vsts      (1001) docker     (121)      150 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-14 12:59:30.772773 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/config/
--rw-r--r--   0 vsts      (1001) docker     (121)      290 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/config/AccessConfigCifFiles.py
--rw-r--r--   0 vsts      (1001) docker     (121)      170 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/config/AccessTemplateFiles.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7680 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/config/EditorConfig.py
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)   144958 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif
--rw-r--r--   0 vsts      (1001) docker     (121)   209858 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-14 12:59:30.776774 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/depict/
--rwxr-xr-x   0 vsts      (1001) docker     (121)    52449 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/depict/EditorDepict.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-14 12:59:30.776774 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/io/
--rw-r--r--   0 vsts      (1001) docker     (121)     4873 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/io/EditorDataImport.py
--rw-r--r--   0 vsts      (1001) docker     (121)   163312 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/io/PdbxDataIo.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8061 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1616 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-14 12:59:30.776774 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/templates/
--rw-r--r--   0 vsts      (1001) docker     (121)     6211 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html
--rw-r--r--   0 vsts      (1001) docker     (121)      641 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html
--rw-r--r--   0 vsts      (1001) docker     (121)    13947 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html
--rw-r--r--   0 vsts      (1001) docker     (121)    17945 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html
--rw-r--r--   0 vsts      (1001) docker     (121)    15904 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html
--rw-r--r--   0 vsts      (1001) docker     (121)     3502 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/templates/editor_prototyping.html
--rw-r--r--   0 vsts      (1001) docker     (121)     2470 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-14 12:59:30.776774 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/webapp/
--rw-r--r--   0 vsts      (1001) docker     (121)    79034 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/webapp/EditorWebApp.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)    10750 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/webapp/WebRequest.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-14 12:57:55.000000 wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-14 12:59:30.772773 wwpdb.apps.editormodule-0.16/wwpdb.apps.editormodule.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)      757 2022-11-14 12:59:30.000000 wwpdb.apps.editormodule-0.16/wwpdb.apps.editormodule.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1637 2022-11-14 12:59:30.000000 wwpdb.apps.editormodule-0.16/wwpdb.apps.editormodule.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-11-14 12:59:30.000000 wwpdb.apps.editormodule-0.16/wwpdb.apps.editormodule.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-11-14 12:58:59.000000 wwpdb.apps.editormodule-0.16/wwpdb.apps.editormodule.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)      141 2022-11-14 12:59:30.000000 wwpdb.apps.editormodule-0.16/wwpdb.apps.editormodule.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        6 2022-11-14 12:59:30.000000 wwpdb.apps.editormodule-0.16/wwpdb.apps.editormodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.218037 wwpdb.apps.editormodule-0.17/
+-rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/LICENSE
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      110 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      757 2023-04-30 13:30:17.218037 wwpdb.apps.editormodule-0.17/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       51 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-04-30 13:30:17.218037 wwpdb.apps.editormodule-0.17/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2209 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.210037 wwpdb.apps.editormodule-0.17/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.210037 wwpdb.apps.editormodule-0.17/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.210037 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/
+-rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.214037 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      290 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/AccessConfigCifFiles.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      170 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/AccessTemplateFiles.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7680 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/EditorConfig.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   144958 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif
+-rw-r--r--   0 vsts      (1001) docker     (123)   209858 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.214037 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/depict/
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    52449 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/depict/EditorDepict.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.214037 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4873 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/EditorDataImport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   163711 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/PdbxDataIo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8061 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1616 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.218037 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6211 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      641 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html
+-rw-r--r--   0 vsts      (1001) docker     (123)    13947 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html
+-rw-r--r--   0 vsts      (1001) docker     (123)    17945 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html
+-rw-r--r--   0 vsts      (1001) docker     (123)    15904 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     3502 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_prototyping.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     2470 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.218037 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (123)    79034 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/webapp/EditorWebApp.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    10750 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/webapp/WebRequest.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.210037 wwpdb.apps.editormodule-0.17/wwpdb.apps.editormodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      757 2023-04-30 13:30:17.000000 wwpdb.apps.editormodule-0.17/wwpdb.apps.editormodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1637 2023-04-30 13:30:17.000000 wwpdb.apps.editormodule-0.17/wwpdb.apps.editormodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-30 13:30:17.000000 wwpdb.apps.editormodule-0.17/wwpdb.apps.editormodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-30 13:30:03.000000 wwpdb.apps.editormodule-0.17/wwpdb.apps.editormodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-04-30 13:30:17.000000 wwpdb.apps.editormodule-0.17/wwpdb.apps.editormodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-04-30 13:30:17.000000 wwpdb.apps.editormodule-0.17/wwpdb.apps.editormodule.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.editormodule-0.16/LICENSE` & `wwpdb.apps.editormodule-0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.16/PKG-INFO` & `wwpdb.apps.editormodule-0.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.editormodule
-Version: 0.16
+Version: 0.17
 Summary: wwPDB mmCIF form editor module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_editormodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.editormodule-0.16/setup.py` & `wwpdb.apps.editormodule-0.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
     ],
     #
-    install_requires=["mmcif", "mmcif.utils", "wwpdb.utils.wf", "wwpdb.utils.db", "wwpdb.utils.session", "wwpdb.io", "wwpdb.utils.config ~= 0.24"],
+    install_requires=["mmcif", "mmcif.utils", "wwpdb.utils.wf", "wwpdb.utils.db", "wwpdb.utils.session", "wwpdb.io", "wwpdb.utils.config ~= 0.24", "wwpdb.utils.dp ~= 0.45"],
     packages=find_packages(exclude=["wwpdb.apps.tests-editormodule"]),
     # Enables Manifest to be used
     include_package_data=True,
     package_data={
         # If any package contains *.md or *.rst ...  files, include them:
         "": ["*.md", "*.rst", "*.txt", "*.cfg", "*.html", "*.cif"],
     },
```

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/config/EditorConfig.py` & `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/EditorConfig.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif` & `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif` & `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/depict/EditorDepict.py` & `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/depict/EditorDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/io/EditorDataImport.py` & `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/EditorDataImport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/io/PdbxDataIo.py` & `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/PdbxDataIo.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,14 +144,15 @@
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
 from mmcif_utils.persist.PdbxDictionaryInfo import PdbxDictionaryInfo, PdbxDictionaryInfoStore, PdbxDictionaryViewInfo
 from wwpdb.apps.editormodule.io.EditorDataImport import EditorDataImport
 from wwpdb.apps.editormodule.io.PdbxMasterViewDictionary import PdbxMasterViewDictionary
 from wwpdb.apps.editormodule.config.EditorConfig import EditorConfig
 from wwpdb.apps.editormodule.config.AccessConfigCifFiles import get_display_view_info_master_cif, get_display_view_info_cif
 from wwpdb.utils.db.DBLoadUtil import DBLoadUtil
+from wwpdb.utils.dp.DepositorSyncUtil import DepositorSyncUtil
 from mmcif.api.DataCategory import DataCategory
 from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
 
 import logging
 
 logger = logging.getLogger(__name__)
 
@@ -691,14 +692,19 @@
 
                 else:
                     # 2015-02-06, ZF -- loading archive model cif file into da_internal database
                     fileSource = str(self.__reqObj.getValue("filesource")).strip().lower()
                     if fileSource in ["archive", "wf-archive", "wf_archive"]:
                         dbLoader = DBLoadUtil(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
                         dbLoader.doLoading([exprtFilePath])
+
+                        # syncing depositor data to database
+                        depId = self.__reqObj.getValue("identifier")
+                        syncdep = DepositorSyncUtil(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
+                        syncdep.syncWithDatabase(depId=depId, modelFilePath=exprtFilePath)
                     # ZF, end DB loading
                     if self.__verbose:
                         logger.info("-- exported updated cif file to %s", exprtFilePath)
                     return True
                 #
             else:
                 return False
```

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py` & `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py` & `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html` & `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html` & `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html` & `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html` & `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html` & `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/templates/editor_prototyping.html` & `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_prototyping.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html` & `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/webapp/EditorWebApp.py` & `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/webapp/EditorWebApp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb/apps/editormodule/webapp/WebRequest.py` & `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/webapp/WebRequest.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb.apps.editormodule.egg-info/PKG-INFO` & `wwpdb.apps.editormodule-0.17/wwpdb.apps.editormodule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.editormodule
-Version: 0.16
+Version: 0.17
 Summary: wwPDB mmCIF form editor module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_editormodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.editormodule-0.16/wwpdb.apps.editormodule.egg-info/SOURCES.txt` & `wwpdb.apps.editormodule-0.17/wwpdb.apps.editormodule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

