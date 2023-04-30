# Comparing `tmp/Quick_Magic-1.6.tar.gz` & `tmp/Quick_Magic-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quick_Magic-1.6.tar", last modified: Sat Apr 29 19:59:39 2023, max compression
+gzip compressed data, was "Quick_Magic-1.7.tar", last modified: Sun Apr 30 10:11:33 2023, max compression
```

## Comparing `Quick_Magic-1.6.tar` & `Quick_Magic-1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:59:39.097901 Quick_Magic-1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-29 19:59:39.097901 Quick_Magic-1.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:59:39.097901 Quick_Magic-1.6/Quick_Magic/
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-29 19:59:29.000000 Quick_Magic-1.6/Quick_Magic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 19:59:29.000000 Quick_Magic-1.6/Quick_Magic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-29 19:59:29.000000 Quick_Magic-1.6/Quick_Magic/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-29 19:59:29.000000 Quick_Magic-1.6/Quick_Magic/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-04-29 19:59:29.000000 Quick_Magic-1.6/Quick_Magic/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-29 19:59:29.000000 Quick_Magic-1.6/Quick_Magic/old_style.py
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-04-29 19:59:29.000000 Quick_Magic-1.6/Quick_Magic/update_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:59:39.097901 Quick_Magic-1.6/Quick_Magic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-29 19:59:39.000000 Quick_Magic-1.6/Quick_Magic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-29 19:59:39.000000 Quick_Magic-1.6/Quick_Magic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 19:59:39.000000 Quick_Magic-1.6/Quick_Magic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 19:59:39.000000 Quick_Magic-1.6/Quick_Magic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 19:59:39.000000 Quick_Magic-1.6/Quick_Magic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-29 19:59:29.000000 Quick_Magic-1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 19:59:39.097901 Quick_Magic-1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-29 19:59:29.000000 Quick_Magic-1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:11:33.442030 Quick_Magic-1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-30 10:11:33.442030 Quick_Magic-1.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:11:33.442030 Quick_Magic-1.7/Quick_Magic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-04-30 10:11:20.000000 Quick_Magic-1.7/Quick_Magic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-30 10:11:20.000000 Quick_Magic-1.7/Quick_Magic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-30 10:11:20.000000 Quick_Magic-1.7/Quick_Magic/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-30 10:11:20.000000 Quick_Magic-1.7/Quick_Magic/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-04-30 10:11:20.000000 Quick_Magic-1.7/Quick_Magic/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-30 10:11:20.000000 Quick_Magic-1.7/Quick_Magic/old_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-04-30 10:11:20.000000 Quick_Magic-1.7/Quick_Magic/update_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:11:33.442030 Quick_Magic-1.7/Quick_Magic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-30 10:11:33.000000 Quick_Magic-1.7/Quick_Magic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-30 10:11:33.000000 Quick_Magic-1.7/Quick_Magic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 10:11:33.000000 Quick_Magic-1.7/Quick_Magic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-30 10:11:33.000000 Quick_Magic-1.7/Quick_Magic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-30 10:11:33.000000 Quick_Magic-1.7/Quick_Magic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-30 10:11:20.000000 Quick_Magic-1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 10:11:33.442030 Quick_Magic-1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-30 10:11:20.000000 Quick_Magic-1.7/setup.py
```

### Comparing `Quick_Magic-1.6/PKG-INFO` & `Quick_Magic-1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quick_Magic
-Version: 1.6
+Version: 1.7
 Summary: Open/Close any application by it's name.
 Home-page: https://github.com/athrvvvv/AppOpener/tree/module
 Download-URL: https://pypi.python.org/pypi/AppOpener
 Author: Athrv Chaulkar
 Author-email: athrvchaulkar@gmail.com
 Maintainer: athrvvvv
 Maintainer-email: athrvchaulkar@gmail.com
```

### Comparing `Quick_Magic-1.6/Quick_Magic/__init__.py` & `Quick_Magic-1.7/Quick_Magic/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 def run(self, output=True):
     print()
     print("'RUN' FUNCTION IS REPLACED BY 'OPEN' FUNCTION")
     print("TRY USING 'OPEN(app_name)'")
     print()
 
 # Open application (Regex implemented)
-def open(self, output=True, match_closest=False):
+def open(self, output=True, match_closest=False, throw_error=False):
     '''
     #### `open` is the function which is used to open applications.
     Examples:
     1: open("whatsapp")
     2: open("whatsapp, telegram")
     3: open("calcu", match_closest=True)
     4: open("whatsapp, telegram", output=False)
@@ -115,17 +115,17 @@
         print()
     else:
         if "," in val:
             splited = val.split(",")
             for i in splited:
                 j = i.strip()
                 if j != "":
-                    features.open_things(j, output=output, match_closest=match_closest)
+                    features.open_things(j, output=output, match_closest=match_closest, throw_error=throw_error)
         else:
-           features.open_things(val, output=output, match_closest=match_closest)
+           features.open_things(val, output=output, match_closest=match_closest, throw_error=throw_error)
 
 # Close any application by just its name :)
 def close(self, output=True, match_closest=False, throw_error=False):
     '''
     #### `close` is the function which is used to close applications.
     Examples:
     1: close("whatsapp")
```

### Comparing `Quick_Magic-1.6/Quick_Magic/check.py` & `Quick_Magic-1.7/Quick_Magic/check.py`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.6/Quick_Magic/commands.py` & `Quick_Magic-1.7/Quick_Magic/commands.py`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.6/Quick_Magic/features.py` & `Quick_Magic-1.7/Quick_Magic/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                     # print("explorer shell:appsFolder\\"+app_name)
                     if output:
                         print("OPENING "+app_name.upper())
             else:
                 if output:
                     if throw_error:
                         # Throwing an error if throw_error is true
-                        raise ValueError(f"{self.upper()} NOT FOUND... TYPE (LS) for list of applications.")
+                        raise AppNotFound(self.upper())
                     else:
                         print(f"{self.upper()} NOT FOUND... TYPE (LS) for list of applications.")
             pass
 
 # EXCEPTION FOR CLOSING FILE EXPLORER
 def close_explorer(output: bool, throw_error: bool, app_name: str):
     handles = []
```

### Comparing `Quick_Magic-1.6/Quick_Magic/old_style.py` & `Quick_Magic-1.7/Quick_Magic/old_style.py`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.6/Quick_Magic/update_list.py` & `Quick_Magic-1.7/Quick_Magic/update_list.py`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.6/Quick_Magic.egg-info/PKG-INFO` & `Quick_Magic-1.7/Quick_Magic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quick-Magic
-Version: 1.6
+Version: 1.7
 Summary: Open/Close any application by it's name.
 Home-page: https://github.com/athrvvvv/AppOpener/tree/module
 Download-URL: https://pypi.python.org/pypi/AppOpener
 Author: Athrv Chaulkar
 Author-email: athrvchaulkar@gmail.com
 Maintainer: athrvvvv
 Maintainer-email: athrvchaulkar@gmail.com
```

### Comparing `Quick_Magic-1.6/README.md` & `Quick_Magic-1.7/README.md`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.6/setup.py` & `Quick_Magic-1.7/setup.py`

 * *Files identical despite different names*

