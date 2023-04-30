# Comparing `tmp/mo_files-6.373.23120-py2.py3-none-any.whl.zip` & `tmp/mo_files-6.375.23120-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 15930 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat    19210 b- defN 22-Dec-28 01:01 mo_files/__init__.py
+Zip file size: 15863 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat    18788 b- defN 23-Apr-30 18:14 mo_files/__init__.py
 -rw-rw-rw-  2.0 fat      197 b- defN 22-Dec-05 22:50 mo_files/mimetype.py
--rw-rw-rw-  2.0 fat    11815 b- defN 22-Dec-07 02:58 mo_files/url.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-Apr-30 12:16 mo_files-6.373.23120.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1603 b- defN 23-Apr-30 12:16 mo_files-6.373.23120.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-30 12:16 mo_files-6.373.23120.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-30 12:16 mo_files-6.373.23120.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      649 b- defN 23-Apr-30 12:16 mo_files-6.373.23120.dist-info/RECORD
-8 files, 50318 bytes uncompressed, 14802 bytes compressed:  70.6%
+-rw-rw-rw-  2.0 fat    11814 b- defN 23-Apr-30 18:14 mo_files/url.py
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-Apr-30 18:14 mo_files-6.375.23120.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1603 b- defN 23-Apr-30 18:14 mo_files-6.375.23120.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-30 18:14 mo_files-6.375.23120.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-30 18:14 mo_files-6.375.23120.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      649 b- defN 23-Apr-30 18:14 mo_files-6.375.23120.dist-info/RECORD
+8 files, 49895 bytes uncompressed, 14735 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: mo_files/mimetype.py
 Comment: 
 
 Filename: mo_files/url.py
 Comment: 
 
-Filename: mo_files-6.373.23120.dist-info/LICENSE
+Filename: mo_files-6.375.23120.dist-info/LICENSE
 Comment: 
 
-Filename: mo_files-6.373.23120.dist-info/METADATA
+Filename: mo_files-6.375.23120.dist-info/METADATA
 Comment: 
 
-Filename: mo_files-6.373.23120.dist-info/WHEEL
+Filename: mo_files-6.375.23120.dist-info/WHEEL
 Comment: 
 
-Filename: mo_files-6.373.23120.dist-info/top_level.txt
+Filename: mo_files-6.375.23120.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_files-6.373.23120.dist-info/RECORD
+Filename: mo_files-6.375.23120.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_files/__init__.py

```diff
@@ -3,16 +3,14 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-from __future__ import absolute_import, division, unicode_literals
-
 import base64
 import io
 import os
 import re
 import shutil
 from datetime import datetime
 from mimetypes import MimeTypes
@@ -254,17 +252,15 @@
                 self.parent.create()
             with open(self._filename, "rb") as f:
                 if self.key:
                     return get_module("mo_math.crypto").decrypt(f.read(), self.key)
                 else:
                     return f.read()
         except Exception as e:
-            Log.error(
-                "Problem reading file {{filename}}", filename=self.abs_path, cause=e
-            )
+            Log.error("Problem reading file {{filename}}", filename=self.abs_path, cause=e)
 
     def write_bytes(self, content):
         if not self.parent.exists:
             self.parent.create()
         with open(self._filename, "wb") as f:
             if self.key:
                 f.write(get_module("mo_math.crypto").encrypt(content, self.key))
@@ -276,18 +272,15 @@
         :param content: text, or iterable of text
         :return:
         """
         if not self.parent.exists:
             self.parent.create()
         with open(self._filename, "wb") as f:
             if is_list(content) and self.key:
-                Log.error(
-                    "list of data and keys are not supported, encrypt before sending to"
-                    " file"
-                )
+                Log.error("list of data and keys are not supported, encrypt before sending to file")
 
             if is_list(content):
                 pass
             elif isinstance(content, text):
                 content = [content]
             elif hasattr(content, "__iter__"):
                 pass
@@ -314,17 +307,15 @@
                     path = home_path + path[1::]
 
                 with io.open(path, "rb") as f:
                     for line in f:
                         yield line.decode("utf8").rstrip()
             except Exception as e:
                 Log.error(
-                    "Can not read line from {{filename}}",
-                    filename=self._filename,
-                    cause=e,
+                    "Can not read line from {{filename}}", filename=self._filename, cause=e,
                 )
 
         return output()
 
     def append(self, content, encoding="utf8"):
         """
         add a line to file
@@ -360,51 +351,44 @@
     def delete(self):
         try:
             if os.path.isdir(self._filename):
                 shutil.rmtree(self._filename)
             elif os.path.isfile(self._filename):
                 os.remove(self._filename)
             return self
-        except Exception as e:
-            e = Except.wrap(e)
-            if "The system cannot find the path specified" in e:
+        except Exception as cause:
+            cause = Except.wrap(cause)
+            if (
+                "The system cannot find the path specified" in cause
+                or "The system cannot find the file specified" in cause
+            ):
                 return
-            Log.error("Could not remove file", e)
+            Log.error("Could not remove file", cause)
 
     def backup(self):
         path = self._filename.split("/")
         names = path[-1].split(".")
         if len(names) == 1 or names[0] == "":
-            backup = File(
-                self._filename
-                + ".backup "
-                + datetime.utcnow().strftime("%Y%m%d %H%M%S")
-            )
+            backup = File(self._filename + ".backup " + datetime.utcnow().strftime("%Y%m%d %H%M%S"))
         else:
             backup = File.new_instance(
                 "/".join(path[:-1]),
-                ".".join(names[:-1])
-                + ".backup "
-                + datetime.now().strftime("%Y%m%d %H%M%S")
-                + "."
-                + names[-1],
+                ".".join(names[:-1]) + ".backup " + datetime.now().strftime("%Y%m%d %H%M%S") + "." + names[-1],
             )
         File.copy(self, backup)
         return backup
 
     def create(self):
         try:
             os.makedirs(self.os_path)
         except FileExistsError:
             pass
         except Exception as e:
             Log.error(
-                "Could not make directory {{dir_name}}",
-                dir_name=self._filename,
-                cause=e,
+                "Could not make directory {{dir_name}}", dir_name=self._filename, cause=e,
             )
 
     @property
     def children(self):
         try:
             return [File(self._filename + "/" + c) for c in os.listdir(self.rel_path)]
         except FileNotFoundError:
@@ -501,20 +485,15 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         from mo_threads import Thread
 
-        Thread.run(
-            "delete dir " + self.stem,
-            delete_daemon,
-            file=self,
-            caller_stack=get_stacktrace(1),
-        ).release()
+        Thread.run("delete dir " + self.stem, delete_daemon, file=self, caller_stack=get_stacktrace(1),).release()
 
 
 class TempFile(File):
     """
     A CONTEXT MANAGER FOR AN ALLOCATED, BUT UNOPENED TEMPORARY FILE
     WILL BE DELETED WHEN EXITED
     """
@@ -531,20 +510,15 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         from mo_threads import Thread
 
-        Thread.run(
-            "delete file " + self.rel_path,
-            delete_daemon,
-            file=self,
-            caller_stack=get_stacktrace(1),
-        ).release()
+        Thread.run("delete file " + self.rel_path, delete_daemon, file=self, caller_stack=get_stacktrace(1),).release()
 
 
 def _copy(from_, to_):
     if from_.is_directory():
         for c in os.listdir(from_.os_path):
             _copy(from_ / c, to_ / c)
     else:
@@ -559,20 +533,18 @@
 
 
 def datetime2string(value, format="%Y-%m-%d %H:%M:%S"):
     try:
         return value.strftime(format)
     except Exception as e:
         Log.error(
-            "Can not format {{value}} with {{format}}",
-            value=value,
-            format=format,
-            cause=e,
+            "Can not format {{value}} with {{format}}", value=value, format=format, cause=e,
         )
 
+
 def join_path(*path):
     def scrub(i, p):
         p = p.replace(os.sep, "/")
         if p in ("", "/"):
             return "."
         if p[-1] == "/":
             p = p[:-1]
@@ -633,17 +605,15 @@
                 return
             file.delete()
             return
         except Exception as e:
             e = Except.wrap(e)
             e.trace = e.trace[0:2] + caller_stack
             if num_attempts:
-                Log.warning(
-                    "problem deleting file {{file}}", file=file.abs_path, cause=e
-                )
+                Log.warning("problem deleting file {{file}}", file=file.abs_path, cause=e)
             (Till(seconds=10) | please_stop).wait()
         num_attempts += 1
 
 
 def add_suffix(filename, suffix):
     """
     ADD .suffix TO THE filename (NOT INCLUDING THE FILE EXTENSION)
```

## mo_files/url.py

```diff
@@ -2,15 +2,14 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-
 from mo_dots import (
     Data,
     Null,
     coalesce,
     is_data,
     is_list,
     to_data,
```

## Comparing `mo_files-6.373.23120.dist-info/LICENSE` & `mo_files-6.375.23120.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_files-6.373.23120.dist-info/METADATA` & `mo_files-6.375.23120.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-files
-Version: 6.373.23120
+Version: 6.375.23120
 Summary: More Files! Steamlined for UTF8 and JSON.
 Home-page: https://github.com/klahnakoski/mo-files
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
@@ -14,16 +14,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mo-dots (==9.368.23092)
 Requires-Dist: mo-future (==7.340.23006)
-Requires-Dist: mo-json (==6.373.23120)
-Requires-Dist: mo-logs (==7.371.23118)
+Requires-Dist: mo-json (==6.374.23120)
+Requires-Dist: mo-logs (==7.374.23120)
 Requires-Dist: mo-math (==7.368.23092)
 Provides-Extra: tests
 Requires-Dist: mo-testing ; extra == 'tests'
 
 # More Files!
 
 The `File` class makes the default assumption all files have cr-delimited unicode content that is UTF-8 encoded. This is great for JSON files. It also provides better operators over some common file manipulations.
```

## Comparing `mo_files-6.373.23120.dist-info/RECORD` & `mo_files-6.375.23120.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-mo_files/__init__.py,sha256=DiLfUyBBg0dkSHvgD0rGr3497pPr2V7rgVitEaPZqts,19210
+mo_files/__init__.py,sha256=uRs0Mm7MvtvaWEdhfmoDl7kzqlWpNVEvGDJatYBfZmc,18788
 mo_files/mimetype.py,sha256=tXRCYszJ_FHg5-itrS28ZGbPnJ3KgrWAEaFKyPBEUYg,197
-mo_files/url.py,sha256=bBgxPQTtd17GKmP88NBA8d-QmR29CIPqzIWPBYb5OOk,11815
-mo_files-6.373.23120.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
-mo_files-6.373.23120.dist-info/METADATA,sha256=AiedInOPlks5FBspPjej9jZc7etBE6g7EX9uWs6eXtM,1603
-mo_files-6.373.23120.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_files-6.373.23120.dist-info/top_level.txt,sha256=a9fidDIwv-DfFgyRS3H6__1vuNeUpplNr_0iLGosdBA,9
-mo_files-6.373.23120.dist-info/RECORD,,
+mo_files/url.py,sha256=dUFjERY9SeZ2u5jB0zVyWPZGLPX9d9Wmt5fJbn9GGRA,11814
+mo_files-6.375.23120.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
+mo_files-6.375.23120.dist-info/METADATA,sha256=2Xk5Y04UTsMwTsY0VGmhrpgjPaEbr34mJdXCtixtXeA,1603
+mo_files-6.375.23120.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_files-6.375.23120.dist-info/top_level.txt,sha256=a9fidDIwv-DfFgyRS3H6__1vuNeUpplNr_0iLGosdBA,9
+mo_files-6.375.23120.dist-info/RECORD,,
```

