# Comparing `tmp/zendron-1.1.4.tar.gz` & `tmp/zendron-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zendron-1.1.4.tar", last modified: Sun Apr 30 00:13:43 2023, max compression
+gzip compressed data, was "zendron-1.1.5.tar", last modified: Sun Apr 30 00:26:11 2023, max compression
```

## Comparing `zendron-1.1.4.tar` & `zendron-1.1.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.746050 zendron-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-30 00:13:23.000000 zendron-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-30 00:13:23.000000 zendron-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-04-30 00:13:43.746050 zendron-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-04-30 00:13:23.000000 zendron-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.738050 zendron-1.1.4/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:23.000000 zendron-1.1.4/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-30 00:13:23.000000 zendron-1.1.4/conf/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.734050 zendron-1.1.4/notes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.734050 zendron-1.1.4/notes/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.738050 zendron-1.1.4/notes/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)   108556 2023-04-30 00:13:23.000000 zendron-1.1.4/notes/assets/images/zotero.api-key.md.zotero-api-key.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.734050 zendron-1.1.4/pods/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.738050 zendron-1.1.4/pods/dendron.markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-30 00:13:23.000000 zendron-1.1.4/pods/dendron.markdown/config.import.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-30 00:13:23.000000 zendron-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 00:13:43.746050 zendron-1.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.734050 zendron-1.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.742050 zendron-1.1.4/src/zendron/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/cache_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/comments_deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.742050 zendron-1.1.4/src/zendron/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/conf/config_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/conf/default_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/front.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/load.py
--rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.734050 zendron-1.1.4/src/zendron/pods/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.742050 zendron-1.1.4/src/zendron/pods/dendron.markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/pods/dendron.markdown/config.import.yml
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/read_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/scratch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-30 00:13:23.000000 zendron-1.1.4/src/zendron/user_citation_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:13:43.742050 zendron-1.1.4/src/zendron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-04-30 00:13:43.000000 zendron-1.1.4/src/zendron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-30 00:13:43.000000 zendron-1.1.4/src/zendron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 00:13:43.000000 zendron-1.1.4/src/zendron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-30 00:13:43.000000 zendron-1.1.4/src/zendron.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-30 00:13:43.000000 zendron-1.1.4/src/zendron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 00:13:43.000000 zendron-1.1.4/src/zendron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.162971 zendron-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-30 00:25:56.000000 zendron-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-30 00:25:56.000000 zendron-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-04-30 00:26:11.158971 zendron-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-04-30 00:25:56.000000 zendron-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.154971 zendron-1.1.5/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:25:56.000000 zendron-1.1.5/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-30 00:25:56.000000 zendron-1.1.5/conf/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.150970 zendron-1.1.5/notes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.150970 zendron-1.1.5/notes/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.154971 zendron-1.1.5/notes/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   108556 2023-04-30 00:25:56.000000 zendron-1.1.5/notes/assets/images/zotero.api-key.md.zotero-api-key.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.150970 zendron-1.1.5/pods/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.154971 zendron-1.1.5/pods/dendron.markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-30 00:25:56.000000 zendron-1.1.5/pods/dendron.markdown/config.import.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-30 00:25:56.000000 zendron-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 00:26:11.162971 zendron-1.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.150970 zendron-1.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.158971 zendron-1.1.5/src/zendron/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/cache_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/comments_deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.158971 zendron-1.1.5/src/zendron/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/conf/config_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/conf/default_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/front.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.150970 zendron-1.1.5/src/zendron/pods/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.158971 zendron-1.1.5/src/zendron/pods/dendron.markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/pods/dendron.markdown/config.import.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/read_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/scratch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-30 00:25:56.000000 zendron-1.1.5/src/zendron/user_citation_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:26:11.158971 zendron-1.1.5/src/zendron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-04-30 00:26:11.000000 zendron-1.1.5/src/zendron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-30 00:26:11.000000 zendron-1.1.5/src/zendron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 00:26:11.000000 zendron-1.1.5/src/zendron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-30 00:26:11.000000 zendron-1.1.5/src/zendron.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-30 00:26:11.000000 zendron-1.1.5/src/zendron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 00:26:11.000000 zendron-1.1.5/src/zendron.egg-info/top_level.txt
```

### Comparing `zendron-1.1.4/LICENSE` & `zendron-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/PKG-INFO` & `zendron-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zendron
-Version: 1.1.4
+Version: 1.1.5
 Summary: Import Zotero annotations with Dendron integration
 Author-email: Michael Volk <michaeljvolk7@gmail.com>
 License: MIT License
         
         Copyright (c) [2022] [Michael Volk]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,15 +25,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/Mjvolk3/Zendron
 Keywords: Zotero,Dendron,Markdown,Notes,Annotations,VSCode
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Zendron
 
 [zendron Github](https://github.com/Mjvolk3/Zendron)
```

### Comparing `zendron-1.1.4/README.md` & `zendron-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/notes/assets/images/zotero.api-key.md.zotero-api-key.png` & `zendron-1.1.5/notes/assets/images/zotero.api-key.md.zotero-api-key.png`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/pods/dendron.markdown/config.import.yml` & `zendron-1.1.5/pods/dendron.markdown/config.import.yml`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/pyproject.toml` & `zendron-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=67.7.2", "wheel>=0.40.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zendron"
-version = "1.1.4"
+version = "1.1.5"
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
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/Mjvolk3/Zendron"
```

### Comparing `zendron-1.1.4/src/zendron/__main__.py` & `zendron-1.1.5/src/zendron/__main__.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/annotations.py` & `zendron-1.1.5/src/zendron/annotations.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/bibtex.py` & `zendron-1.1.5/src/zendron/bibtex.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/cache.py` & `zendron-1.1.5/src/zendron/cache.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/cache_deprecated.py` & `zendron-1.1.5/src/zendron/cache_deprecated.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/comments.py` & `zendron-1.1.5/src/zendron/comments.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/comments_deprecated.py` & `zendron-1.1.5/src/zendron/comments_deprecated.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/conf/config_template.yaml` & `zendron-1.1.5/src/zendron/conf/config_template.yaml`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/config.py` & `zendron-1.1.5/src/zendron/config.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/front.py` & `zendron-1.1.5/src/zendron/front.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/init.py` & `zendron-1.1.5/src/zendron/init.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/items.py` & `zendron-1.1.5/src/zendron/items.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/load.py` & `zendron-1.1.5/src/zendron/load.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/metadata.py` & `zendron-1.1.5/src/zendron/metadata.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/pods/dendron.markdown/config.import.yml` & `zendron-1.1.5/src/zendron/pods/dendron.markdown/config.import.yml`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/read_md.py` & `zendron-1.1.5/src/zendron/read_md.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/remove.py` & `zendron-1.1.5/src/zendron/remove.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/scratch.py` & `zendron-1.1.5/src/zendron/scratch.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/sync.py` & `zendron-1.1.5/src/zendron/sync.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron/user_citation_key.py` & `zendron-1.1.5/src/zendron/user_citation_key.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.4/src/zendron.egg-info/PKG-INFO` & `zendron-1.1.5/src/zendron.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zendron
-Version: 1.1.4
+Version: 1.1.5
 Summary: Import Zotero annotations with Dendron integration
 Author-email: Michael Volk <michaeljvolk7@gmail.com>
 License: MIT License
         
         Copyright (c) [2022] [Michael Volk]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,15 +25,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/Mjvolk3/Zendron
 Keywords: Zotero,Dendron,Markdown,Notes,Annotations,VSCode
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Zendron
 
 [zendron Github](https://github.com/Mjvolk3/Zendron)
```

### Comparing `zendron-1.1.4/src/zendron.egg-info/SOURCES.txt` & `zendron-1.1.5/src/zendron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

