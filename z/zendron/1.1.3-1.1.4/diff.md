# Comparing `tmp/zendron-1.1.3.tar.gz` & `tmp/zendron-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zendron-1.1.3.tar", last modified: Thu Apr 27 08:30:24 2023, max compression
+gzip compressed data, was "zendron-1.1.4.tar", last modified: Sun Apr 30 00:13:43 2023, max compression
```

## Comparing `zendron-1.1.3.tar` & `zendron-1.1.4.tar`

### file list

```diff
@@ -1,54 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.893953 zendron-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 08:30:11.000000 zendron-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-27 08:30:11.000000 zendron-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-04-27 08:30:24.893953 zendron-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-27 08:30:11.000000 zendron-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.889953 zendron-1.1.3/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:11.000000 zendron-1.1.3/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-27 08:30:11.000000 zendron-1.1.3/conf/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-27 08:30:11.000000 zendron-1.1.3/conf/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.889953 zendron-1.1.3/notes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.889953 zendron-1.1.3/notes/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.889953 zendron-1.1.3/notes/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)   108556 2023-04-27 08:30:11.000000 zendron-1.1.3/notes/assets/images/zotero.api-key.md.zotero-api-key.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.889953 zendron-1.1.3/pods/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.889953 zendron-1.1.3/pods/dendron.markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-27 08:30:11.000000 zendron-1.1.3/pods/dendron.markdown/config.import.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-27 08:30:11.000000 zendron-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 08:30:24.893953 zendron-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.889953 zendron-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.893953 zendron-1.1.3/src/zendron/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/cache_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/comments_deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.893953 zendron-1.1.3/src/zendron/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/conf/config_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/conf/default_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/front.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/load.py
--rw-r--r--   0 runner    (1001) docker     (123)    13396 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.889953 zendron-1.1.3/src/zendron/pods/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.893953 zendron-1.1.3/src/zendron/pods/dendron.markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/pods/dendron.markdown/config.import.yml
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/read_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/scratch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-27 08:30:11.000000 zendron-1.1.3/src/zendron/user_citation_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:30:24.893953 zendron-1.1.3/src/zendron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-04-27 08:30:24.000000 zendron-1.1.3/src/zendron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-27 08:30:24.000000 zendron-1.1.3/src/zendron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:30:24.000000 zendron-1.1.3/src/zendron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 08:30:24.000000 zendron-1.1.3/src/zendron.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-27 08:30:24.000000 zendron-1.1.3/src/zendron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 08:30:24.000000 zendron-1.1.3/src/zendron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.746050 zendron-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-30 00:13:23.000000 zendron-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-30 00:13:23.000000 zendron-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-04-30 00:13:43.746050 zendron-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-04-30 00:13:23.000000 zendron-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.738050 zendron-1.1.4/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:23.000000 zendron-1.1.4/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-30 00:13:23.000000 zendron-1.1.4/conf/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.734050 zendron-1.1.4/notes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.734050 zendron-1.1.4/notes/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.738050 zendron-1.1.4/notes/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   108556 2023-04-30 00:13:23.000000 zendron-1.1.4/notes/assets/images/zotero.api-key.md.zotero-api-key.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.734050 zendron-1.1.4/pods/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.738050 zendron-1.1.4/pods/dendron.markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-30 00:13:23.000000 zendron-1.1.4/pods/dendron.markdown/config.import.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-30 00:13:23.000000 zendron-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 00:13:43.746050 zendron-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.734050 zendron-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.742050 zendron-1.1.4/src/zendron/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/cache_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/comments_deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.742050 zendron-1.1.4/src/zendron/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/conf/config_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/conf/default_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/front.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.734050 zendron-1.1.4/src/zendron/pods/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.742050 zendron-1.1.4/src/zendron/pods/dendron.markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/pods/dendron.markdown/config.import.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/read_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/scratch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/user_citation_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.742050 zendron-1.1.4/src/zendron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-04-30 00:13:43.000000 zendron-1.1.4/src/zendron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-30 00:13:43.000000 zendron-1.1.4/src/zendron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 00:13:43.000000 zendron-1.1.4/src/zendron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-30 00:13:43.000000 zendron-1.1.4/src/zendron.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-30 00:13:43.000000 zendron-1.1.4/src/zendron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 00:13:43.000000 zendron-1.1.4/src/zendron.egg-info/top_level.txt
```

### Comparing `zendron-1.1.3/LICENSE` & `zendron-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/PKG-INFO` & `zendron-1.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,45 @@
-Metadata-Version: 2.1
-Name: zendron
-Version: 1.1.3
-Summary: Import Zotero annotations with Dendron integration
-Author-email: Michael Volk <michaeljvolk7@gmail.com>
-License: MIT License
-        
-        Copyright (c) [2022] [Michael Volk]
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/Mjvolk3/Zendron
-Keywords: Zotero,Dendron,Markdown,Notes,Annotations,VSCode
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Zendron
 
-Version: 1.1.3
 [zendron Github](https://github.com/Mjvolk3/Zendron)
 
+[![PyPI version](https://badge.fury.io/py/zendron.svg)](https://badge.fury.io/py/zendron)
+
 ## Introduction
 
 - This package was developed for porting Zotero annotations and metadata to markdown. These markdown notes are then brought into a [Dendron](https://www.dendron.so/) hierarchy for integration with vault notes. We recommend using the package within [Visual Studio Code](https://code.visualstudio.com/).The end goal is to get a two way sync between notes in Zotero and notes in Dendron, but this has some difficulties and limitations that are taking some time to address. For now only a one way sync from Zotero to Dendron is supported.
 
 ## Install Instructions
 
 - It is recommended to build a [conda env](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) for installation.
 - Install [Dendron CLI](https://wiki.dendron.so/notes/RjBkTbGuKCXJNuE4dyV6G/).
   - `npm install -g @dendronhq/dendron-cli@latest`
 - Install the zendron
   - `python -m pip install zendron`
 
+## Zotero Local Setup
+
+- To start you need [Better BibTeX for Zotero](https://retorque.re/zotero-better-bibtex/installation/)
+  - This allows pinning of of bibtex keys.v
+- Go to `Zotero > Settings... > Advanced > General > Config Editor`![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zendron.citation-key.md.zotero-config-editor.png)
+- Accept the risks ![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zendron.citation-key.md.zotero-config-editor-accept-risks.png)
+- In the Search, type `autoPinDelay` and chance the integer value from 0 (default) to 1. ![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zendron.citation-key.md.autoPinDelay-update.png)
+
 ## Zotero API key
 
 - [Zotero API key](https://www.zotero.org/settings/keys)
 - We recommend setting up you Zotero API key with the following settings to allow for full functionality.
   - Personal Library
     - [x] Allow library access.
     - [x] Allow notes access.
     - [x] Allow write access.
   - Default Gropu Permissions
     - [x] Read/Write
 
-![](./notes/assets/images/zotero.api-key.md.zotero-api-key.png)
+![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zotero.api-key.md.zotero-api-key.png)
 
 - This key can then be copy pasted in the configuration file. You should add your key to `.gitignore` to prevent others from accessing your Zotoero database. If the key is lost you can always generate a new one.
 
 ## Zotero and File Import Configuration
 
 All zendron configuration is handled in [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml).
 
@@ -78,29 +51,41 @@
 item_types: [journalArticle, book, preprint, conferencePaper, report] # List of item types according to [pyzotero](https://pyzotero.readthedocs.io/en/latest/)
 local_image_path: /Users/<username>/Zotero/cache # Local path for importing annotated images
 dendron_limb: zendron.import # Dendron import limb e.g. zendron.import.paper-title.annotations.md
 zotero_comment_title: zendron comment # fixed for now... needed for eventual 2-way sync.
 pod_path: zotero_pod # Name of dendron pod, removed after completion of import. We will later add configuration for this to remain. This will allow for non Dendron users to import markdown Zotero notes in a strucutred hierarchy.
 ```
 
+- `library_id` - Integer identifier of library. This is the number that matches the name of a library.
+  - [User ID](https://www.zotero.org/settings/keys).
+  - For group ID visit [Zotero Groups](https://www.zotero.org/groups/), click on your desired group, and copy the id from the URL.
+- `library_type`: `group` for group libraries and `user` for user library.
+- `api_key`: Use the API Key obtained from [Zotero API KEY](README.md#zotero-api-key).
+- `collection`: This can be the name of any collection or subcollection in the specificed library. If there are multiple collections or sub collections with the same name, the import will arbitrarily choose one. To make sure you are importing the desired collection, make sure the name of the collection is unique in the Zotero library.
+- `item_types`: Zotero item types to import according to [pyzotero](https://pyzotero.readthedocs.io/en/latest/) syntax.
+`local_image_path`: Path to annotated images. `/Users/<username>/Zotero/cache` is the default path on MacOS.
+- `dendron_limb`: This is the period deliminated hierarchy prefix to all file imports for Dendron, e.g. `root.zotero.import.<paper_title>.annotations.md`.
+- `zotero comment title` - IGNORE FOR NOW. Eventually needed for 2-way sync.
+- `pod_path` - IGNORE FOR NOW. Eventually needed for markdown only import, without Dendron integration.
+
 ## Basic Usage
 
 There are only two basic commands that work as of now.
 
 - `zendron`
   - This command should only be run in the root directory of the workspace.
-  - This command imports notes according to a defined [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml). Once the command is run the first time the user needs to modify their configuration `./conf/config.yaml` according the Zotero library specifications and the Zotero API.
-  - Notes are imported with a `## Time Created` heading. This allows for stable reference from other notes, within the note vault. We autogenerate a `*.comments.md` that should be used for taking any additional notes within Dendron. Additional notes taken within the meta data file (`notes/zendron.import.<paper-title>.md`), or the `*.annotations.md` will be overwritten after running `zendron` for a second time.
+  - This command imports notes according to a defined [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml). Once the command is run the first time the user needs to modify their configuration `./conf/config.yaml`. All required configs are marked with a comment `# STARTER CONFIG` upon initialization.
+  - Notes are imported with a `## Time Created` heading. This allows for stable reference from other notes, within the note vault. We autogenerate a `*.comments.md` that should be used for taking any additional notes within Dendron. Additional notes taken within the meta data file (`notes/zendron.import.<paper-title>.md`), or the `*.annotations.md` will be overwritten after running `zendron` for a second time. All files downstream of import excpet `*.comments.md` should be treated as read only. We have plans to explicitly make them read only soon.
+  - Upon import, notes and tags are left as stubs. To create these notes run `> Dendron: Doctor` then `createMissingLinkedNotes`. It is best practice to correc tag warnings before doing this.
 - `zendron remove=true`
-  - This command removes all imported notes and associated links. We run a `createMissingLinkedNotes` following the deletion of Dendron notes to repopulate `tags` and `users` that will be removed on running `zendron-remove`.
+  - This command removes imported notes and associated links. This command works by remove all notes downstream fo `dendron_limb`, excpet for `comments.md`. There is some difficult removing other files created becuase these are separate from the `dendron_limb`. These files include `user.*.md`, which comes from bibtex keys, and `tags.*.md` which come from metadata and annotation tags. For now, we don't remove tags, but we do remove bibex keys (`<user.bibtex_key>.md`).
   - There are more complicated removal's that could be desired so we plan to eventually change this from a `bool` to an `str`.
 
 ## Miscellaneous
 
-- The `zendron_cache` is not currenlty in use. We do an entire relaod each time, so for large libraries performance will be poor.
-  - You an feel free to delete the cache as you please.
+- The `zendron_cache` is used for remove of `<user.bibtex_key>.md`. If it is deleted and you run remove, the `<user.bibtex_key>.md` will not be removed. In this case you can run `zendron` again, then run the `zendron remove=true` again.
 - If there are run that fail, sometimes a `.hydra` with the given configuraiton will be generated in the root dir. This isn't an issue but it contains the API information and should therefore be added to the `.gitignore` as a safeguard. In addition these files can be used to inspect the reason for the faiure.
 - `__main__.log` is generated after running a `zendron`, this can also be deleted as you please. It is also useful for inspecting an failures to import.
 
 ## Troubleshooting
 
 - If you are having trouble with startup you can use this [Zendron-Test](https://github.com/Mjvolk3/Zendron-Test) template and try to reproduce your issues here. Simply click on `Use this template`, clone the repo and try to run `zendron` here. This will allow for us to catch things we overlooked for different user workspace configuration etc. Once you have tried to reproduce issues here please submit an issue on [Zendron](https://github.com/Mjvolk3/Zendron).
```

### Comparing `zendron-1.1.3/notes/assets/images/zotero.api-key.md.zotero-api-key.png` & `zendron-1.1.4/notes/assets/images/zotero.api-key.md.zotero-api-key.png`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/pods/dendron.markdown/config.import.yml` & `zendron-1.1.4/pods/dendron.markdown/config.import.yml`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/pyproject.toml` & `zendron-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=67.7.2", "wheel>=0.40.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zendron"
-version = "1.1.3"
+version = "1.1.4"
 description = "Import Zotero annotations with Dendron integration"
 readme = "README.md"
 authors = [{ name = "Michael Volk", email = "michaeljvolk7@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -24,15 +24,15 @@
     "tomli >= 2.0.1",
     "python-frontmatter >= 1.0.0",
     "html2text >= 2020.1.16",
     "Markdown >= 3.4.1",
     "markdownify >= 0.11.6",
     "importlib-metadata >= 6.6.0"
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/Mjvolk3/Zendron"
```

### Comparing `zendron-1.1.3/src/zendron/__main__.py` & `zendron-1.1.4/src/zendron/__main__.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/src/zendron/annotations.py` & `zendron-1.1.4/src/zendron/annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,20 @@
         annotation_tags = ", ".join(
             [f"#{i['tag']}" for i in self.annotation["data"]["tags"]]
         )
         return annotation_tags
 
     def format_annotation_tags(self, lines: list, annotation_tags: str):
         cfg_annotations_tags_format = True
+
         if annotation_tags != "":
+            if " " in lines:
+                log.warning(
+                    f"Tags should not contain spaces. Please remove spaces in Zotero annotations and sync again. Tag: {annotation_tags}"
+                )
             if cfg_annotations_tags_format:
                 lines.append(f"- Tags: {annotation_tags}")
         return lines
 
     def format_annotation_text(self, lines: list, annotation_text: str):
         if annotation_text == "":
             return lines
```

### Comparing `zendron-1.1.3/src/zendron/bibtex.py` & `zendron-1.1.4/src/zendron/bibtex.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/src/zendron/cache.py` & `zendron-1.1.4/src/zendron/cache.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/src/zendron/cache_deprecated.py` & `zendron-1.1.4/src/zendron/cache_deprecated.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/src/zendron/comments.py` & `zendron-1.1.4/src/zendron/comments.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/src/zendron/comments_deprecated.py` & `zendron-1.1.4/src/zendron/comments_deprecated.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/src/zendron/conf/config_template.yaml` & `zendron-1.1.4/src/zendron/conf/config_template.yaml`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/src/zendron/config.py` & `zendron-1.1.4/src/zendron/config.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/src/zendron/front.py` & `zendron-1.1.4/src/zendron/front.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/src/zendron/init.py` & `zendron-1.1.4/src/zendron/init.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/src/zendron/items.py` & `zendron-1.1.4/src/zendron/items.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/src/zendron/load.py` & `zendron-1.1.4/src/zendron/load.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/src/zendron/metadata.py` & `zendron-1.1.4/src/zendron/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,24 +221,26 @@
         return self._attachment_keys
 
     def get_pdf_attachments(self):
         # TODO for groups only - need another for local. parameterize type of library.
         # TODO deal with multiple attachments... like supplementary.
         library_type = self.metadata["library"]["type"]
         if library_type == "user":
+            pdf_attachment = None
             for att_key in self.attachment_keys:
                 try:
                     link = f"https://www.zotero.org/{self.name}/items/{self.key}/attachment/{att_key}/reader"
                     pdf_attachment = f"[Online PDF attachment]({link})"
                 except KeyError:
                     pdf_attachment = None
                     log.warning(
                         "No PDF attachment... Your metadata should probably have attachments."
                     )
         if library_type == "group":
+            pdf_attachment = None
             for att_key in self.attachment_keys:
                 try:
                     # TODO check if this works for groups
                     link = f"https://www.zotero.org/groups/{self.library_id}/zendron/items/{self.key}/attachment/{att_key}/reader"
                     pdf_attachment = f"[Online PDF attachment]({link})"
                 except KeyError:
                     pdf_attachment = None
@@ -249,15 +251,15 @@
 
     def get_tags(self):
         if self.metadata["data"]["tags"] == []:
             return "No tags"
         for tags in self.metadata["data"]["tags"]:
             if " " in tags["tag"]:
                 log.warning(
-                    f"Tags should not contain spaces. Please remove spaces in Zotero and sync again. Tag: {tags['tag']}. Title Dendron: {self.title_dendron}."
+                    f"Tags should not contain spaces. Please remove spaces in Zotero metadata and sync again. Tag: {tags['tag']}. Title Dendron: {self.title_dendron}."
                 )
         tags = ", ".join([f"#{i['tag']}" for i in self.metadata["data"]["tags"]])
         # TODO Config to convert tags that aren't delimited by '-' to be... On backward sync they can be updated with this. Could be a dangerous operation
         return tags
 
     def get_local_library(self):
         local_library = f"zotero://select/items/{self.library_id}"
```

### Comparing `zendron-1.1.3/src/zendron/pods/dendron.markdown/config.import.yml` & `zendron-1.1.4/src/zendron/pods/dendron.markdown/config.import.yml`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/src/zendron/read_md.py` & `zendron-1.1.4/src/zendron/read_md.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/src/zendron/scratch.py` & `zendron-1.1.4/src/zendron/scratch.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/src/zendron/sync.py` & `zendron-1.1.4/src/zendron/sync.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/src/zendron/user_citation_key.py` & `zendron-1.1.4/src/zendron/user_citation_key.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.3/src/zendron.egg-info/PKG-INFO` & `zendron-1.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zendron
-Version: 1.1.3
+Version: 1.1.4
 Summary: Import Zotero annotations with Dendron integration
 Author-email: Michael Volk <michaeljvolk7@gmail.com>
 License: MIT License
         
         Copyright (c) [2022] [Michael Volk]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,48 +25,57 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/Mjvolk3/Zendron
 Keywords: Zotero,Dendron,Markdown,Notes,Annotations,VSCode
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Zendron
 
-Version: 1.1.3
 [zendron Github](https://github.com/Mjvolk3/Zendron)
 
+[![PyPI version](https://badge.fury.io/py/zendron.svg)](https://badge.fury.io/py/zendron)
+
 ## Introduction
 
 - This package was developed for porting Zotero annotations and metadata to markdown. These markdown notes are then brought into a [Dendron](https://www.dendron.so/) hierarchy for integration with vault notes. We recommend using the package within [Visual Studio Code](https://code.visualstudio.com/).The end goal is to get a two way sync between notes in Zotero and notes in Dendron, but this has some difficulties and limitations that are taking some time to address. For now only a one way sync from Zotero to Dendron is supported.
 
 ## Install Instructions
 
 - It is recommended to build a [conda env](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) for installation.
 - Install [Dendron CLI](https://wiki.dendron.so/notes/RjBkTbGuKCXJNuE4dyV6G/).
   - `npm install -g @dendronhq/dendron-cli@latest`
 - Install the zendron
   - `python -m pip install zendron`
 
+## Zotero Local Setup
+
+- To start you need [Better BibTeX for Zotero](https://retorque.re/zotero-better-bibtex/installation/)
+  - This allows pinning of of bibtex keys.v
+- Go to `Zotero > Settings... > Advanced > General > Config Editor`![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zendron.citation-key.md.zotero-config-editor.png)
+- Accept the risks ![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zendron.citation-key.md.zotero-config-editor-accept-risks.png)
+- In the Search, type `autoPinDelay` and chance the integer value from 0 (default) to 1. ![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zendron.citation-key.md.autoPinDelay-update.png)
+
 ## Zotero API key
 
 - [Zotero API key](https://www.zotero.org/settings/keys)
 - We recommend setting up you Zotero API key with the following settings to allow for full functionality.
   - Personal Library
     - [x] Allow library access.
     - [x] Allow notes access.
     - [x] Allow write access.
   - Default Gropu Permissions
     - [x] Read/Write
 
-![](./notes/assets/images/zotero.api-key.md.zotero-api-key.png)
+![](https://github.com/Mjvolk3/Zendron/blob/main/notes/assets/images/zotero.api-key.md.zotero-api-key.png)
 
 - This key can then be copy pasted in the configuration file. You should add your key to `.gitignore` to prevent others from accessing your Zotoero database. If the key is lost you can always generate a new one.
 
 ## Zotero and File Import Configuration
 
 All zendron configuration is handled in [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml).
 
@@ -78,29 +87,41 @@
 item_types: [journalArticle, book, preprint, conferencePaper, report] # List of item types according to [pyzotero](https://pyzotero.readthedocs.io/en/latest/)
 local_image_path: /Users/<username>/Zotero/cache # Local path for importing annotated images
 dendron_limb: zendron.import # Dendron import limb e.g. zendron.import.paper-title.annotations.md
 zotero_comment_title: zendron comment # fixed for now... needed for eventual 2-way sync.
 pod_path: zotero_pod # Name of dendron pod, removed after completion of import. We will later add configuration for this to remain. This will allow for non Dendron users to import markdown Zotero notes in a strucutred hierarchy.
 ```
 
+- `library_id` - Integer identifier of library. This is the number that matches the name of a library.
+  - [User ID](https://www.zotero.org/settings/keys).
+  - For group ID visit [Zotero Groups](https://www.zotero.org/groups/), click on your desired group, and copy the id from the URL.
+- `library_type`: `group` for group libraries and `user` for user library.
+- `api_key`: Use the API Key obtained from [Zotero API KEY](README.md#zotero-api-key).
+- `collection`: This can be the name of any collection or subcollection in the specificed library. If there are multiple collections or sub collections with the same name, the import will arbitrarily choose one. To make sure you are importing the desired collection, make sure the name of the collection is unique in the Zotero library.
+- `item_types`: Zotero item types to import according to [pyzotero](https://pyzotero.readthedocs.io/en/latest/) syntax.
+`local_image_path`: Path to annotated images. `/Users/<username>/Zotero/cache` is the default path on MacOS.
+- `dendron_limb`: This is the period deliminated hierarchy prefix to all file imports for Dendron, e.g. `root.zotero.import.<paper_title>.annotations.md`.
+- `zotero comment title` - IGNORE FOR NOW. Eventually needed for 2-way sync.
+- `pod_path` - IGNORE FOR NOW. Eventually needed for markdown only import, without Dendron integration.
+
 ## Basic Usage
 
 There are only two basic commands that work as of now.
 
 - `zendron`
   - This command should only be run in the root directory of the workspace.
-  - This command imports notes according to a defined [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml). Once the command is run the first time the user needs to modify their configuration `./conf/config.yaml` according the Zotero library specifications and the Zotero API.
-  - Notes are imported with a `## Time Created` heading. This allows for stable reference from other notes, within the note vault. We autogenerate a `*.comments.md` that should be used for taking any additional notes within Dendron. Additional notes taken within the meta data file (`notes/zendron.import.<paper-title>.md`), or the `*.annotations.md` will be overwritten after running `zendron` for a second time.
+  - This command imports notes according to a defined [config.yml](https://github.com/Mjvolk3/Zendron/blob/main/conf/config.yaml). Once the command is run the first time the user needs to modify their configuration `./conf/config.yaml`. All required configs are marked with a comment `# STARTER CONFIG` upon initialization.
+  - Notes are imported with a `## Time Created` heading. This allows for stable reference from other notes, within the note vault. We autogenerate a `*.comments.md` that should be used for taking any additional notes within Dendron. Additional notes taken within the meta data file (`notes/zendron.import.<paper-title>.md`), or the `*.annotations.md` will be overwritten after running `zendron` for a second time. All files downstream of import excpet `*.comments.md` should be treated as read only. We have plans to explicitly make them read only soon.
+  - Upon import, notes and tags are left as stubs. To create these notes run `> Dendron: Doctor` then `createMissingLinkedNotes`. It is best practice to correc tag warnings before doing this.
 - `zendron remove=true`
-  - This command removes all imported notes and associated links. We run a `createMissingLinkedNotes` following the deletion of Dendron notes to repopulate `tags` and `users` that will be removed on running `zendron-remove`.
+  - This command removes imported notes and associated links. This command works by remove all notes downstream fo `dendron_limb`, excpet for `comments.md`. There is some difficult removing other files created becuase these are separate from the `dendron_limb`. These files include `user.*.md`, which comes from bibtex keys, and `tags.*.md` which come from metadata and annotation tags. For now, we don't remove tags, but we do remove bibex keys (`<user.bibtex_key>.md`).
   - There are more complicated removal's that could be desired so we plan to eventually change this from a `bool` to an `str`.
 
 ## Miscellaneous
 
-- The `zendron_cache` is not currenlty in use. We do an entire relaod each time, so for large libraries performance will be poor.
-  - You an feel free to delete the cache as you please.
+- The `zendron_cache` is used for remove of `<user.bibtex_key>.md`. If it is deleted and you run remove, the `<user.bibtex_key>.md` will not be removed. In this case you can run `zendron` again, then run the `zendron remove=true` again.
 - If there are run that fail, sometimes a `.hydra` with the given configuraiton will be generated in the root dir. This isn't an issue but it contains the API information and should therefore be added to the `.gitignore` as a safeguard. In addition these files can be used to inspect the reason for the faiure.
 - `__main__.log` is generated after running a `zendron`, this can also be deleted as you please. It is also useful for inspecting an failures to import.
 
 ## Troubleshooting
 
 - If you are having trouble with startup you can use this [Zendron-Test](https://github.com/Mjvolk3/Zendron-Test) template and try to reproduce your issues here. Simply click on `Use this template`, clone the repo and try to run `zendron` here. This will allow for us to catch things we overlooked for different user workspace configuration etc. Once you have tried to reproduce issues here please submit an issue on [Zendron](https://github.com/Mjvolk3/Zendron).
```

### Comparing `zendron-1.1.3/src/zendron.egg-info/SOURCES.txt` & `zendron-1.1.4/src/zendron.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 conf/__init__.py
-conf/config.yaml
 conf/default.yaml
-src/../conf/config.yaml
 src/../conf/default.yaml
 src/../notes/assets/images/zotero.api-key.md.zotero-api-key.png
 src/../pods/dendron.markdown/config.import.yml
 src/zendron/__init__.py
 src/zendron/__main__.py
 src/zendron/annotations.py
 src/zendron/bibtex.py
```

