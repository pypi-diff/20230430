# Comparing `tmp/icommandlib-0.7.0.tar.gz` & `tmp/icommandlib-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icommandlib-0.7.0.tar", last modified: Mon Apr 24 14:37:06 2023, max compression
+gzip compressed data, was "icommandlib-0.8.0.tar", last modified: Sun Apr 30 11:27:33 2023, max compression
```

## Comparing `icommandlib-0.7.0.tar` & `icommandlib-0.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:37:06.337705 icommandlib-0.7.0/
--rw-r--r--   0 root         (0) root         (0)     1524 2023-04-24 14:36:39.000000 icommandlib-0.7.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     3861 2023-04-24 14:36:39.000000 icommandlib-0.7.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-04-24 14:36:39.000000 icommandlib-0.7.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3150 2023-04-24 14:37:06.337705 icommandlib-0.7.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2361 2023-04-24 14:36:39.000000 icommandlib-0.7.0/README.md
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-24 14:36:39.000000 icommandlib-0.7.0/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:37:06.333705 icommandlib-0.7.0/icommandlib/
--rw-r--r--   0 root         (0) root         (0)      216 2023-04-24 14:36:39.000000 icommandlib-0.7.0/icommandlib/__init__.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-04-24 14:36:39.000000 icommandlib-0.7.0/icommandlib/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-04-24 14:36:39.000000 icommandlib-0.7.0/icommandlib/icommand.py
--rw-r--r--   0 root         (0) root         (0)     8395 2023-04-24 14:36:39.000000 icommandlib-0.7.0/icommandlib/iprocess.py
--rw-r--r--   0 root         (0) root         (0)     1705 2023-04-24 14:36:39.000000 icommandlib-0.7.0/icommandlib/messages.py
--rw-r--r--   0 root         (0) root         (0)     1939 2023-04-24 14:36:39.000000 icommandlib-0.7.0/icommandlib/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:37:06.337705 icommandlib-0.7.0/icommandlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3150 2023-04-24 14:37:06.000000 icommandlib-0.7.0/icommandlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      395 2023-04-24 14:37:06.000000 icommandlib-0.7.0/icommandlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 14:37:06.000000 icommandlib-0.7.0/icommandlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-24 14:37:06.000000 icommandlib-0.7.0/icommandlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-24 14:37:06.000000 icommandlib-0.7.0/icommandlib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1136 2023-04-24 14:36:39.000000 icommandlib-0.7.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 14:37:06.337705 icommandlib-0.7.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 14:36:39.000000 icommandlib-0.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 11:27:33.330565 icommandlib-0.8.0/
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-04-30 11:27:01.000000 icommandlib-0.8.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-04-30 11:27:01.000000 icommandlib-0.8.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-04-30 11:27:01.000000 icommandlib-0.8.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-04-30 11:27:33.330565 icommandlib-0.8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-04-30 11:27:01.000000 icommandlib-0.8.0/README.md
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-30 11:27:01.000000 icommandlib-0.8.0/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 11:27:33.326565 icommandlib-0.8.0/icommandlib/
+-rw-r--r--   0 root         (0) root         (0)      216 2023-04-30 11:27:01.000000 icommandlib-0.8.0/icommandlib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2023-04-30 11:27:01.000000 icommandlib-0.8.0/icommandlib/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-04-30 11:27:01.000000 icommandlib-0.8.0/icommandlib/icommand.py
+-rw-r--r--   0 root         (0) root         (0)     8183 2023-04-30 11:27:01.000000 icommandlib-0.8.0/icommandlib/iprocess.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-04-30 11:27:01.000000 icommandlib-0.8.0/icommandlib/messages.py
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-04-30 11:27:01.000000 icommandlib-0.8.0/icommandlib/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 11:27:33.330565 icommandlib-0.8.0/icommandlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-04-30 11:27:33.000000 icommandlib-0.8.0/icommandlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      395 2023-04-30 11:27:33.000000 icommandlib-0.8.0/icommandlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 11:27:33.000000 icommandlib-0.8.0/icommandlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-30 11:27:33.000000 icommandlib-0.8.0/icommandlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-30 11:27:33.000000 icommandlib-0.8.0/icommandlib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-04-30 11:27:01.000000 icommandlib-0.8.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-30 11:27:33.330565 icommandlib-0.8.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-30 11:27:01.000000 icommandlib-0.8.0/setup.py
```

### Comparing `icommandlib-0.7.0/CHANGELOG.md` & `icommandlib-0.8.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # Changelog
 
 
+### 0.8.0
+
+* FEATURE : Save stripshot on IProcessTimeout exceptions.
+
+
 ### 0.7.0
 
 * FEATURE : Added wait for stripshot.
 
 
 ### 0.6.1
```

### Comparing `icommandlib-0.7.0/LICENSE.txt` & `icommandlib-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `icommandlib-0.7.0/PKG-INFO` & `icommandlib-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icommandlib
-Version: 0.7.0
+Version: 0.8.0
 Summary: Pythonic interactive command runner.
 Author-email: Colm O'Connor <colm.oconnor.github@gmail.com>
 License: MIT
 Project-URL: homepage, https://hitchdev.com/icommandlib
 Project-URL: documentation, https://hitchdev.com/icommandlib/using
 Project-URL: repository, https://github.com/icommandlib/hitchstory
 Project-URL: changelog, https://hitchdev.com/icommandlib/changelog
```

### Comparing `icommandlib-0.7.0/README.md` & `icommandlib-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `icommandlib-0.7.0/icommandlib/icommand.py` & `icommandlib-0.8.0/icommandlib/icommand.py`

 * *Files identical despite different names*

### Comparing `icommandlib-0.7.0/icommandlib/iprocess.py` & `icommandlib-0.8.0/icommandlib/iprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,18 +136,16 @@
                 self._read()
 
                 if condition_function(self.iscreen):
                     return
 
                 if time.time() - start_time > timeout:
                     raise exceptions.IProcessTimeout(
-                        "Timed out after {0} seconds:\n\n{1}".format(
-                            timeout,
-                            stripshot(self.iscreen.text),
-                        )
+                        timeout,
+                        self.iscreen.stripshot,
                     )
 
                 if not self.running:
                     self._read()
                     raise exceptions.UnexpectedExit(
                         self.exit_code,
                         stripshot(self.iscreen.text),
@@ -240,18 +238,16 @@
             if not self._ptyprocess.isalive():
                 self._ptyprocess.close()
                 self.finished = True
                 return
 
             if time.time() - start_time > timeout:
                 raise exceptions.IProcessTimeout(
-                    "Timed out after {0} seconds:\n\n{1}".format(
-                        timeout,
-                        stripshot(self.iscreen.text),
-                    )
+                    timeout,
+                    self.iscreen.stripshot,
                 )
 
     def wait_for_successful_exit(self, timeout=None):
         """
         Wait until the process exits successfully. Raises exception
         if the process is still open after timeout or it exits
         with an exit code other than 0.
```

### Comparing `icommandlib-0.7.0/icommandlib/messages.py` & `icommandlib-0.8.0/icommandlib/messages.py`

 * *Files identical despite different names*

### Comparing `icommandlib-0.7.0/icommandlib/utils.py` & `icommandlib-0.8.0/icommandlib/utils.py`

 * *Files identical despite different names*

### Comparing `icommandlib-0.7.0/icommandlib.egg-info/PKG-INFO` & `icommandlib-0.8.0/icommandlib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icommandlib
-Version: 0.7.0
+Version: 0.8.0
 Summary: Pythonic interactive command runner.
 Author-email: Colm O'Connor <colm.oconnor.github@gmail.com>
 License: MIT
 Project-URL: homepage, https://hitchdev.com/icommandlib
 Project-URL: documentation, https://hitchdev.com/icommandlib/using
 Project-URL: repository, https://github.com/icommandlib/hitchstory
 Project-URL: changelog, https://hitchdev.com/icommandlib/changelog
```

### Comparing `icommandlib-0.7.0/pyproject.toml` & `icommandlib-0.8.0/pyproject.toml`

 * *Files identical despite different names*

