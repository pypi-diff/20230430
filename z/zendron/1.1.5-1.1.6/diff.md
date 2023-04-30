# Comparing `tmp/zendron-1.1.5.tar.gz` & `tmp/zendron-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zendron-1.1.5.tar", last modified: Sun Apr 30 00:26:11 2023, max compression
+gzip compressed data, was "zendron-1.1.6.tar", last modified: Sun Apr 30 00:31:20 2023, max compression
```

## Comparing `zendron-1.1.5.tar` & `zendron-1.1.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.162971 zendron-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-30 00:25:56.000000 zendron-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-30 00:25:56.000000 zendron-1.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-04-30 00:26:11.158971 zendron-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-04-30 00:25:56.000000 zendron-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.154971 zendron-1.1.5/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:25:56.000000 zendron-1.1.5/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-30 00:25:56.000000 zendron-1.1.5/conf/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.150970 zendron-1.1.5/notes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.150970 zendron-1.1.5/notes/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.154971 zendron-1.1.5/notes/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)   108556 2023-04-30 00:25:56.000000 zendron-1.1.5/notes/assets/images/zotero.api-key.md.zotero-api-key.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.150970 zendron-1.1.5/pods/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.154971 zendron-1.1.5/pods/dendron.markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-30 00:25:56.000000 zendron-1.1.5/pods/dendron.markdown/config.import.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-30 00:25:56.000000 zendron-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 00:26:11.162971 zendron-1.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.150970 zendron-1.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.158971 zendron-1.1.5/src/zendron/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/cache_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/comments_deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.158971 zendron-1.1.5/src/zendron/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/conf/config_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/conf/default_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/front.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/load.py
--rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.150970 zendron-1.1.5/src/zendron/pods/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.158971 zendron-1.1.5/src/zendron/pods/dendron.markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/pods/dendron.markdown/config.import.yml
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/read_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/scratch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/user_citation_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.158971 zendron-1.1.5/src/zendron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-04-30 00:26:11.000000 zendron-1.1.5/src/zendron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-30 00:26:11.000000 zendron-1.1.5/src/zendron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 00:26:11.000000 zendron-1.1.5/src/zendron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-30 00:26:11.000000 zendron-1.1.5/src/zendron.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-30 00:26:11.000000 zendron-1.1.5/src/zendron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 00:26:11.000000 zendron-1.1.5/src/zendron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.044253 zendron-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-30 00:30:55.000000 zendron-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-30 00:30:55.000000 zendron-1.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-04-30 00:31:20.044253 zendron-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-04-30 00:30:55.000000 zendron-1.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.040253 zendron-1.1.6/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:30:55.000000 zendron-1.1.6/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-30 00:30:55.000000 zendron-1.1.6/conf/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.040253 zendron-1.1.6/notes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.040253 zendron-1.1.6/notes/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.040253 zendron-1.1.6/notes/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   108556 2023-04-30 00:30:55.000000 zendron-1.1.6/notes/assets/images/zotero.api-key.md.zotero-api-key.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.040253 zendron-1.1.6/pods/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.040253 zendron-1.1.6/pods/dendron.markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-30 00:30:55.000000 zendron-1.1.6/pods/dendron.markdown/config.import.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-30 00:30:55.000000 zendron-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 00:31:20.044253 zendron-1.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.040253 zendron-1.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.044253 zendron-1.1.6/src/zendron/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/cache_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/comments_deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.044253 zendron-1.1.6/src/zendron/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/conf/config_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/conf/default_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/front.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.040253 zendron-1.1.6/src/zendron/pods/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.044253 zendron-1.1.6/src/zendron/pods/dendron.markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/pods/dendron.markdown/config.import.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/read_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/scratch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/user_citation_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.044253 zendron-1.1.6/src/zendron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-04-30 00:31:20.000000 zendron-1.1.6/src/zendron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-30 00:31:20.000000 zendron-1.1.6/src/zendron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 00:31:20.000000 zendron-1.1.6/src/zendron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-30 00:31:20.000000 zendron-1.1.6/src/zendron.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-30 00:31:20.000000 zendron-1.1.6/src/zendron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 00:31:20.000000 zendron-1.1.6/src/zendron.egg-info/top_level.txt
```

### Comparing `zendron-1.1.5/LICENSE` & `zendron-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/PKG-INFO` & `zendron-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zendron
-Version: 1.1.5
+Version: 1.1.6
 Summary: Import Zotero annotations with Dendron integration
 Author-email: Michael Volk <michaeljvolk7@gmail.com>
 License: MIT License
         
         Copyright (c) [2022] [Michael Volk]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -52,36 +52,36 @@
 - Install the zendron
   - `python -m pip install zendron`
 
 ## Zotero Local Setup
 
 - To start you need [Better BibTeX for Zotero](https://retorque.re/zotero-better-bibtex/installation/)
   - This allows pinning of of bibtex keys.v
-- Go to `Zotero > Settings... > Advanced > General > Config Editor`![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zendron.citation-key.md.zotero-config-editor.png)
-- Accept the risks ![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zendron.citation-key.md.zotero-config-editor-accept-risks.png)
-- In the Search, type `autoPinDelay` and chance the integer value from 0 (default) to 1. ![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zendron.citation-key.md.autoPinDelay-update.png)
+- Go to `Zotero > Settings... > Advanced > General > Config Editor`![](https://github.com/Mjvolk3/Zendron/raw/main/notes/assets/images/zendron.citation-key.md.zotero-config-editor.png)
+- Accept the risks ![](https://github.com/Mjvolk3/Zendron/raw/main/notes/assets/images/zendron.citation-key.md.zotero-config-editor-accept-risks.png)
+- In the Search, type `autoPinDelay` and chance the integer value from 0 (default) to 1. ![](https://github.com/Mjvolk3/Zendron/raw/main/notes/assets/images/zendron.citation-key.md.autoPinDelay-update.png)
 
 ## Zotero API key
 
 - [Zotero API key](https://www.zotero.org/settings/keys)
 - We recommend setting up you Zotero API key with the following settings to allow for full functionality.
   - Personal Library
     - [x] Allow library access.
     - [x] Allow notes access.
     - [x] Allow write access.
   - Default Gropu Permissions
     - [x] Read/Write
 
-![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zotero.api-key.md.zotero-api-key.png)
+![](https://github.com/Mjvolk3/Zendron/raw/main/notes/assets/images/zotero.api-key.md.zotero-api-key.png)
 
 - This key can then be copy pasted in the configuration file. You should add your key to `.gitignore` to prevent others from accessing your Zotoero database. If the key is lost you can always generate a new one.
 
 ## Zotero and File Import Configuration
 
-All zendron configuration is handled in [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml).
+All zendron configuration is handled in [config.yml](https://github.com/Mjvolk3/Zendron/raw/main/conf/config.yaml).
 
 ```yml
 library_id : 4932032 # Zotero library ID
 library_type : group # [user, group] library
 api_key : FoCauOvWMlNdYmpYuY5JplTw # Zotero API key
 collection: null # Name of Zotero Collection, null for entire library
 item_types: [journalArticle, book, preprint, conferencePaper, report] # List of item types according to [pyzotero](https://pyzotero.readthedocs.io/en/latest/)
@@ -105,15 +105,15 @@
 
 ## Basic Usage
 
 There are only two basic commands that work as of now.
 
 - `zendron`
   - This command should only be run in the root directory of the workspace.
-  - This command imports notes according to a defined [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml). Once the command is run the first time the user needs to modify their configuration `./conf/config.yaml`. All required configs are marked with a comment `# STARTER CONFIG` upon initialization.
+  - This command imports notes according to a defined [config.yml](https://github.com/Mjvolk3/Zendron/raw/main/conf/config.yaml). Once the command is run the first time the user needs to modify their configuration `./conf/config.yaml`. All required configs are marked with a comment `# STARTER CONFIG` upon initialization.
   - Notes are imported with a `## Time Created` heading. This allows for stable reference from other notes, within the note vault. We autogenerate a `*.comments.md` that should be used for taking any additional notes within Dendron. Additional notes taken within the meta data file (`notes/zendron.import.<paper-title>.md`), or the `*.annotations.md` will be overwritten after running `zendron` for a second time. All files downstream of import excpet `*.comments.md` should be treated as read only. We have plans to explicitly make them read only soon.
   - Upon import, notes and tags are left as stubs. To create these notes run `> Dendron: Doctor` then `createMissingLinkedNotes`. It is best practice to correc tag warnings before doing this.
 - `zendron remove=true`
   - This command removes imported notes and associated links. This command works by remove all notes downstream fo `dendron_limb`, excpet for `comments.md`. There is some difficult removing other files created becuase these are separate from the `dendron_limb`. These files include `user.*.md`, which comes from bibtex keys, and `tags.*.md` which come from metadata and annotation tags. For now, we don't remove tags, but we do remove bibex keys (`<user.bibtex_key>.md`).
   - There are more complicated removal's that could be desired so we plan to eventually change this from a `bool` to an `str`.
 
 ## Miscellaneous
```

### Comparing `zendron-1.1.5/README.md` & `zendron-1.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,36 +16,36 @@
 - Install the zendron
   - `python -m pip install zendron`
 
 ## Zotero Local Setup
 
 - To start you need [Better BibTeX for Zotero](https://retorque.re/zotero-better-bibtex/installation/)
   - This allows pinning of of bibtex keys.v
-- Go to `Zotero > Settings... > Advanced > General > Config Editor`![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zendron.citation-key.md.zotero-config-editor.png)
-- Accept the risks ![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zendron.citation-key.md.zotero-config-editor-accept-risks.png)
-- In the Search, type `autoPinDelay` and chance the integer value from 0 (default) to 1. ![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zendron.citation-key.md.autoPinDelay-update.png)
+- Go to `Zotero > Settings... > Advanced > General > Config Editor`![](https://github.com/Mjvolk3/Zendron/raw/main/notes/assets/images/zendron.citation-key.md.zotero-config-editor.png)
+- Accept the risks ![](https://github.com/Mjvolk3/Zendron/raw/main/notes/assets/images/zendron.citation-key.md.zotero-config-editor-accept-risks.png)
+- In the Search, type `autoPinDelay` and chance the integer value from 0 (default) to 1. ![](https://github.com/Mjvolk3/Zendron/raw/main/notes/assets/images/zendron.citation-key.md.autoPinDelay-update.png)
 
 ## Zotero API key
 
 - [Zotero API key](https://www.zotero.org/settings/keys)
 - We recommend setting up you Zotero API key with the following settings to allow for full functionality.
   - Personal Library
     - [x] Allow library access.
     - [x] Allow notes access.
     - [x] Allow write access.
   - Default Gropu Permissions
     - [x] Read/Write
 
-![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zotero.api-key.md.zotero-api-key.png)
+![](https://github.com/Mjvolk3/Zendron/raw/main/notes/assets/images/zotero.api-key.md.zotero-api-key.png)
 
 - This key can then be copy pasted in the configuration file. You should add your key to `.gitignore` to prevent others from accessing your Zotoero database. If the key is lost you can always generate a new one.
 
 ## Zotero and File Import Configuration
 
-All zendron configuration is handled in [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml).
+All zendron configuration is handled in [config.yml](https://github.com/Mjvolk3/Zendron/raw/main/conf/config.yaml).
 
 ```yml
 library_id : 4932032 # Zotero library ID
 library_type : group # [user, group] library
 api_key : FoCauOvWMlNdYmpYuY5JplTw # Zotero API key
 collection: null # Name of Zotero Collection, null for entire library
 item_types: [journalArticle, book, preprint, conferencePaper, report] # List of item types according to [pyzotero](https://pyzotero.readthedocs.io/en/latest/)
@@ -69,15 +69,15 @@
 
 ## Basic Usage
 
 There are only two basic commands that work as of now.
 
 - `zendron`
   - This command should only be run in the root directory of the workspace.
-  - This command imports notes according to a defined [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml). Once the command is run the first time the user needs to modify their configuration `./conf/config.yaml`. All required configs are marked with a comment `# STARTER CONFIG` upon initialization.
+  - This command imports notes according to a defined [config.yml](https://github.com/Mjvolk3/Zendron/raw/main/conf/config.yaml). Once the command is run the first time the user needs to modify their configuration `./conf/config.yaml`. All required configs are marked with a comment `# STARTER CONFIG` upon initialization.
   - Notes are imported with a `## Time Created` heading. This allows for stable reference from other notes, within the note vault. We autogenerate a `*.comments.md` that should be used for taking any additional notes within Dendron. Additional notes taken within the meta data file (`notes/zendron.import.<paper-title>.md`), or the `*.annotations.md` will be overwritten after running `zendron` for a second time. All files downstream of import excpet `*.comments.md` should be treated as read only. We have plans to explicitly make them read only soon.
   - Upon import, notes and tags are left as stubs. To create these notes run `> Dendron: Doctor` then `createMissingLinkedNotes`. It is best practice to correc tag warnings before doing this.
 - `zendron remove=true`
   - This command removes imported notes and associated links. This command works by remove all notes downstream fo `dendron_limb`, excpet for `comments.md`. There is some difficult removing other files created becuase these are separate from the `dendron_limb`. These files include `user.*.md`, which comes from bibtex keys, and `tags.*.md` which come from metadata and annotation tags. For now, we don't remove tags, but we do remove bibex keys (`<user.bibtex_key>.md`).
   - There are more complicated removal's that could be desired so we plan to eventually change this from a `bool` to an `str`.
 
 ## Miscellaneous
```

### Comparing `zendron-1.1.5/notes/assets/images/zotero.api-key.md.zotero-api-key.png` & `zendron-1.1.6/notes/assets/images/zotero.api-key.md.zotero-api-key.png`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/pods/dendron.markdown/config.import.yml` & `zendron-1.1.6/pods/dendron.markdown/config.import.yml`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/pyproject.toml` & `zendron-1.1.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=67.7.2", "wheel>=0.40.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zendron"
-version = "1.1.5"
+version = "1.1.6"
 description = "Import Zotero annotations with Dendron integration"
 readme = "README.md"
 authors = [{ name = "Michael Volk", email = "michaeljvolk7@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `zendron-1.1.5/src/zendron/__main__.py` & `zendron-1.1.6/src/zendron/__main__.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/annotations.py` & `zendron-1.1.6/src/zendron/annotations.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/bibtex.py` & `zendron-1.1.6/src/zendron/bibtex.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/cache.py` & `zendron-1.1.6/src/zendron/cache.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/cache_deprecated.py` & `zendron-1.1.6/src/zendron/cache_deprecated.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/comments.py` & `zendron-1.1.6/src/zendron/comments.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/comments_deprecated.py` & `zendron-1.1.6/src/zendron/comments_deprecated.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/conf/config_template.yaml` & `zendron-1.1.6/src/zendron/conf/config_template.yaml`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/config.py` & `zendron-1.1.6/src/zendron/config.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/front.py` & `zendron-1.1.6/src/zendron/front.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/init.py` & `zendron-1.1.6/src/zendron/init.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/items.py` & `zendron-1.1.6/src/zendron/items.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/load.py` & `zendron-1.1.6/src/zendron/load.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/metadata.py` & `zendron-1.1.6/src/zendron/metadata.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/pods/dendron.markdown/config.import.yml` & `zendron-1.1.6/src/zendron/pods/dendron.markdown/config.import.yml`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/read_md.py` & `zendron-1.1.6/src/zendron/read_md.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/remove.py` & `zendron-1.1.6/src/zendron/remove.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/scratch.py` & `zendron-1.1.6/src/zendron/scratch.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/sync.py` & `zendron-1.1.6/src/zendron/sync.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron/user_citation_key.py` & `zendron-1.1.6/src/zendron/user_citation_key.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.5/src/zendron.egg-info/PKG-INFO` & `zendron-1.1.6/src/zendron.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zendron
-Version: 1.1.5
+Version: 1.1.6
 Summary: Import Zotero annotations with Dendron integration
 Author-email: Michael Volk <michaeljvolk7@gmail.com>
 License: MIT License
         
         Copyright (c) [2022] [Michael Volk]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -52,36 +52,36 @@
 - Install the zendron
   - `python -m pip install zendron`
 
 ## Zotero Local Setup
 
 - To start you need [Better BibTeX for Zotero](https://retorque.re/zotero-better-bibtex/installation/)
   - This allows pinning of of bibtex keys.v
-- Go to `Zotero > Settings... > Advanced > General > Config Editor`![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zendron.citation-key.md.zotero-config-editor.png)
-- Accept the risks ![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zendron.citation-key.md.zotero-config-editor-accept-risks.png)
-- In the Search, type `autoPinDelay` and chance the integer value from 0 (default) to 1. ![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zendron.citation-key.md.autoPinDelay-update.png)
+- Go to `Zotero > Settings... > Advanced > General > Config Editor`![](https://github.com/Mjvolk3/Zendron/raw/main/notes/assets/images/zendron.citation-key.md.zotero-config-editor.png)
+- Accept the risks ![](https://github.com/Mjvolk3/Zendron/raw/main/notes/assets/images/zendron.citation-key.md.zotero-config-editor-accept-risks.png)
+- In the Search, type `autoPinDelay` and chance the integer value from 0 (default) to 1. ![](https://github.com/Mjvolk3/Zendron/raw/main/notes/assets/images/zendron.citation-key.md.autoPinDelay-update.png)
 
 ## Zotero API key
 
 - [Zotero API key](https://www.zotero.org/settings/keys)
 - We recommend setting up you Zotero API key with the following settings to allow for full functionality.
   - Personal Library
     - [x] Allow library access.
     - [x] Allow notes access.
     - [x] Allow write access.
   - Default Gropu Permissions
     - [x] Read/Write
 
-![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zotero.api-key.md.zotero-api-key.png)
+![](https://github.com/Mjvolk3/Zendron/raw/main/notes/assets/images/zotero.api-key.md.zotero-api-key.png)
 
 - This key can then be copy pasted in the configuration file. You should add your key to `.gitignore` to prevent others from accessing your Zotoero database. If the key is lost you can always generate a new one.
 
 ## Zotero and File Import Configuration
 
-All zendron configuration is handled in [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml).
+All zendron configuration is handled in [config.yml](https://github.com/Mjvolk3/Zendron/raw/main/conf/config.yaml).
 
 ```yml
 library_id : 4932032 # Zotero library ID
 library_type : group # [user, group] library
 api_key : FoCauOvWMlNdYmpYuY5JplTw # Zotero API key
 collection: null # Name of Zotero Collection, null for entire library
 item_types: [journalArticle, book, preprint, conferencePaper, report] # List of item types according to [pyzotero](https://pyzotero.readthedocs.io/en/latest/)
@@ -105,15 +105,15 @@
 
 ## Basic Usage
 
 There are only two basic commands that work as of now.
 
 - `zendron`
   - This command should only be run in the root directory of the workspace.
-  - This command imports notes according to a defined [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml). Once the command is run the first time the user needs to modify their configuration `./conf/config.yaml`. All required configs are marked with a comment `# STARTER CONFIG` upon initialization.
+  - This command imports notes according to a defined [config.yml](https://github.com/Mjvolk3/Zendron/raw/main/conf/config.yaml). Once the command is run the first time the user needs to modify their configuration `./conf/config.yaml`. All required configs are marked with a comment `# STARTER CONFIG` upon initialization.
   - Notes are imported with a `## Time Created` heading. This allows for stable reference from other notes, within the note vault. We autogenerate a `*.comments.md` that should be used for taking any additional notes within Dendron. Additional notes taken within the meta data file (`notes/zendron.import.<paper-title>.md`), or the `*.annotations.md` will be overwritten after running `zendron` for a second time. All files downstream of import excpet `*.comments.md` should be treated as read only. We have plans to explicitly make them read only soon.
   - Upon import, notes and tags are left as stubs. To create these notes run `> Dendron: Doctor` then `createMissingLinkedNotes`. It is best practice to correc tag warnings before doing this.
 - `zendron remove=true`
   - This command removes imported notes and associated links. This command works by remove all notes downstream fo `dendron_limb`, excpet for `comments.md`. There is some difficult removing other files created becuase these are separate from the `dendron_limb`. These files include `user.*.md`, which comes from bibtex keys, and `tags.*.md` which come from metadata and annotation tags. For now, we don't remove tags, but we do remove bibex keys (`<user.bibtex_key>.md`).
   - There are more complicated removal's that could be desired so we plan to eventually change this from a `bool` to an `str`.
 
 ## Miscellaneous
```

### Comparing `zendron-1.1.5/src/zendron.egg-info/SOURCES.txt` & `zendron-1.1.6/src/zendron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

