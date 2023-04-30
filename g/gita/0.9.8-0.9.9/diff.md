# Comparing `tmp/gita-0.9.8.tar.gz` & `tmp/gita-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gita-0.9.8.tar", last modified: Fri Jun 14 04:48:38 2019, max compression
+gzip compressed data, was "dist/gita-0.9.9.tar", last modified: Fri Jun 14 13:51:42 2019, max compression
```

## Comparing `gita-0.9.8.tar` & `gita-0.9.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 chronos   (1000) chronos   (1000)        0 2019-06-14 04:48:38.000000 gita-0.9.8/
--rw-r--r--   0 chronos   (1000) chronos   (1000)       22 2019-05-08 04:08:28.000000 gita-0.9.8/MANIFEST.in
--rw-r--r--   0 chronos   (1000) chronos   (1000)     8630 2019-06-14 04:48:38.000000 gita-0.9.8/PKG-INFO
--rw-r--r--   0 chronos   (1000) chronos   (1000)     6267 2019-06-14 04:45:59.000000 gita-0.9.8/README.md
-drwxr-xr-x   0 chronos   (1000) chronos   (1000)        0 2019-06-14 04:48:38.000000 gita-0.9.8/gita/
--rw-r--r--   0 chronos   (1000) chronos   (1000)       83 2019-05-08 04:08:28.000000 gita-0.9.8/gita/__init__.py
--rw-r--r--   0 chronos   (1000) chronos   (1000)     6582 2019-06-14 03:47:47.000000 gita-0.9.8/gita/__main__.py
--rw-r--r--   0 chronos   (1000) chronos   (1000)     1207 2019-05-11 03:10:16.000000 gita-0.9.8/gita/cmds.yml
--rw-r--r--   0 chronos   (1000) chronos   (1000)     8879 2019-06-14 03:47:47.000000 gita-0.9.8/gita/utils.py
-drwxr-xr-x   0 chronos   (1000) chronos   (1000)        0 2019-06-14 04:48:38.000000 gita-0.9.8/gita.egg-info/
--rw-r--r--   0 chronos   (1000) chronos   (1000)     8630 2019-06-14 04:48:38.000000 gita-0.9.8/gita.egg-info/PKG-INFO
--rw-r--r--   0 chronos   (1000) chronos   (1000)      262 2019-06-14 04:48:38.000000 gita-0.9.8/gita.egg-info/SOURCES.txt
--rw-r--r--   0 chronos   (1000) chronos   (1000)        1 2019-06-14 04:48:38.000000 gita-0.9.8/gita.egg-info/dependency_links.txt
--rw-r--r--   0 chronos   (1000) chronos   (1000)       45 2019-06-14 04:48:38.000000 gita-0.9.8/gita.egg-info/entry_points.txt
--rw-r--r--   0 chronos   (1000) chronos   (1000)       12 2019-06-14 04:48:38.000000 gita-0.9.8/gita.egg-info/requires.txt
--rw-r--r--   0 chronos   (1000) chronos   (1000)        5 2019-06-14 04:48:38.000000 gita-0.9.8/gita.egg-info/top_level.txt
--rw-r--r--   0 chronos   (1000) chronos   (1000)       38 2019-06-14 04:48:38.000000 gita-0.9.8/setup.cfg
--rw-r--r--   0 chronos   (1000) chronos   (1000)     1233 2019-06-14 03:46:45.000000 gita-0.9.8/setup.py
+drwxr-xr-x   0 chronos   (1000) chronos   (1000)        0 2019-06-14 13:51:42.000000 gita-0.9.9/
+-rw-r--r--   0 chronos   (1000) chronos   (1000)       22 2019-05-08 04:08:28.000000 gita-0.9.9/MANIFEST.in
+-rw-r--r--   0 chronos   (1000) chronos   (1000)     8630 2019-06-14 13:51:42.000000 gita-0.9.9/PKG-INFO
+-rw-r--r--   0 chronos   (1000) chronos   (1000)     6267 2019-06-14 13:39:03.000000 gita-0.9.9/README.md
+drwxr-xr-x   0 chronos   (1000) chronos   (1000)        0 2019-06-14 13:51:42.000000 gita-0.9.9/gita/
+-rw-r--r--   0 chronos   (1000) chronos   (1000)       83 2019-05-08 04:08:28.000000 gita-0.9.9/gita/__init__.py
+-rw-r--r--   0 chronos   (1000) chronos   (1000)     6534 2019-06-14 13:42:08.000000 gita-0.9.9/gita/__main__.py
+-rw-r--r--   0 chronos   (1000) chronos   (1000)     1207 2019-05-11 03:10:16.000000 gita-0.9.9/gita/cmds.yml
+-rw-r--r--   0 chronos   (1000) chronos   (1000)     8876 2019-06-14 13:41:36.000000 gita-0.9.9/gita/utils.py
+drwxr-xr-x   0 chronos   (1000) chronos   (1000)        0 2019-06-14 13:51:42.000000 gita-0.9.9/gita.egg-info/
+-rw-r--r--   0 chronos   (1000) chronos   (1000)     8630 2019-06-14 13:51:41.000000 gita-0.9.9/gita.egg-info/PKG-INFO
+-rw-r--r--   0 chronos   (1000) chronos   (1000)      262 2019-06-14 13:51:41.000000 gita-0.9.9/gita.egg-info/SOURCES.txt
+-rw-r--r--   0 chronos   (1000) chronos   (1000)        1 2019-06-14 13:51:41.000000 gita-0.9.9/gita.egg-info/dependency_links.txt
+-rw-r--r--   0 chronos   (1000) chronos   (1000)       45 2019-06-14 13:51:41.000000 gita-0.9.9/gita.egg-info/entry_points.txt
+-rw-r--r--   0 chronos   (1000) chronos   (1000)       12 2019-06-14 13:51:41.000000 gita-0.9.9/gita.egg-info/requires.txt
+-rw-r--r--   0 chronos   (1000) chronos   (1000)        5 2019-06-14 13:51:41.000000 gita-0.9.9/gita.egg-info/top_level.txt
+-rw-r--r--   0 chronos   (1000) chronos   (1000)       38 2019-06-14 13:51:42.000000 gita-0.9.9/setup.cfg
+-rw-r--r--   0 chronos   (1000) chronos   (1000)     1233 2019-06-14 13:43:40.000000 gita-0.9.9/setup.py
```

### Comparing `gita-0.9.8/PKG-INFO` & `gita-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gita
-Version: 0.9.8
+Version: 0.9.9
 Summary: Manage multiple git repos
 Home-page: https://github.com/nosarthur/gita
 Author: Dong Zhou
 Author-email: zhou.dong@gmail.com
 License: MIT
 Description: [![PyPi version](https://img.shields.io/pypi/v/gita.svg?color=blue)](https://pypi.org/project/gita/)
         [![Build Status](https://travis-ci.org/nosarthur/gita.svg?branch=master)](https://travis-ci.org/nosarthur/gita)
```

### Comparing `gita-0.9.8/README.md` & `gita-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `gita-0.9.8/gita/__main__.py` & `gita-0.9.9/gita/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,15 @@
     Unregister repo(s) from gita
     """
     path_file = utils.get_path_fname()
     if os.path.isfile(path_file):
         repos = utils.get_repos()
         for repo in args.repo:
             del repos[repo]
-        with open(path_file, 'w') as f:
-            f.write(os.pathsep.join(repos.values()))
+        utils.write_to_repo_file(repos, 'w')
 
 
 def f_git_cmd(args: argparse.Namespace):
     """
     Delegate git command/alias defined in `args.cmd`. Asynchronous execution is
     disabled for commands in the `args.async_blacklist`.
     """
```

### Comparing `gita-0.9.8/gita/cmds.yml` & `gita-0.9.9/gita/cmds.yml`

 * *Files identical despite different names*

### Comparing `gita-0.9.8/gita/utils.py` & `gita-0.9.9/gita/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,18 +92,18 @@
 def rename_repo(repos: Dict[str, str], repo: str, new_name: str):
     """
     Write new repo name to file
     """
     path = repos[repo]
     del repos[repo]
     repos[new_name] = path
-    _write_to_repo_file(repos, 'w')
+    write_to_repo_file(repos, 'w')
 
 
-def _write_to_repo_file(repos: Dict[str, str], mode: str):
+def write_to_repo_file(repos: Dict[str, str], mode: str):
     """
     """
     data = ''.join(f'{path},{name}\n' for name, path in repos.items())
     fname = get_path_fname()
     os.makedirs(os.path.dirname(fname), exist_ok=True)
     with open(fname, mode) as f:
         f.write(data)
@@ -117,15 +117,15 @@
     new_paths = set(os.path.abspath(p) for p in new_paths if is_git(p))
     new_paths = new_paths - existing_paths
     if new_paths:
         print(f"Found {len(new_paths)} new repo(s).")
         new_repos = {
                 os.path.basename(os.path.normpath(path)): path
                 for path in new_paths}
-        _write_to_repo_file(new_repos, 'a+')
+        write_to_repo_file(new_repos, 'a+')
     else:
         print('No new repos found!')
 
 
 def get_head(path: str) -> str:
     result = subprocess.run(
         'git rev-parse --abbrev-ref HEAD'.split(),
```

### Comparing `gita-0.9.8/gita.egg-info/PKG-INFO` & `gita-0.9.9/gita.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gita
-Version: 0.9.8
+Version: 0.9.9
 Summary: Manage multiple git repos
 Home-page: https://github.com/nosarthur/gita
 Author: Dong Zhou
 Author-email: zhou.dong@gmail.com
 License: MIT
 Description: [![PyPi version](https://img.shields.io/pypi/v/gita.svg?color=blue)](https://pypi.org/project/gita/)
         [![Build Status](https://travis-ci.org/nosarthur/gita.svg?branch=master)](https://travis-ci.org/nosarthur/gita)
```

### Comparing `gita-0.9.8/setup.py` & `gita-0.9.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 long_description = None
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='gita',
     packages=['gita'],
-    version='0.9.8',
+    version='0.9.9',
     license='MIT',
     description='Manage multiple git repos',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nosarthur/gita',
     platforms=['linux', 'osx', 'win32'],
     keywords=['git', 'manage multiple repositories'],
```

