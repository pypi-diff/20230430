# Comparing `tmp/ReverseShell-0.0.3.tar.gz` & `tmp/ReverseShell-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseShell-0.0.3.tar", last modified: Sun Apr 30 18:19:23 2023, max compression
+gzip compressed data, was "ReverseShell-0.0.4.tar", last modified: Sun Apr 30 19:20:35 2023, max compression
```

## Comparing `ReverseShell-0.0.3.tar` & `ReverseShell-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-30 18:19:23.599891 ReverseShell-0.0.3/
--rw-r--r--   0 kali      (1000) kali      (1000)    35821 2023-04-30 18:10:03.000000 ReverseShell-0.0.3/LICENSE.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       51 2023-04-30 18:10:59.000000 ReverseShell-0.0.3/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     6119 2023-04-30 18:19:23.599891 ReverseShell-0.0.3/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     5044 2023-04-30 23:50:08.000000 ReverseShell-0.0.3/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-30 18:19:23.599891 ReverseShell-0.0.3/ReverseShell.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     6119 2023-04-30 18:19:23.000000 ReverseShell-0.0.3/ReverseShell.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      570 2023-04-30 18:19:23.000000 ReverseShell-0.0.3/ReverseShell.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-30 18:19:23.000000 ReverseShell-0.0.3/ReverseShell.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       51 2023-04-30 18:19:23.000000 ReverseShell-0.0.3/ReverseShell.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-04-30 18:19:23.000000 ReverseShell-0.0.3/ReverseShell.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-04-30 18:19:23.000000 ReverseShell-0.0.3/ReverseShell.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    23199 2023-04-30 18:19:13.000000 ReverseShell-0.0.3/ReverseShell.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-30 18:19:23.599891 ReverseShell-0.0.3/clients/
--rw-r--r--   0 kali      (1000) kali      (1000)     3258 2023-04-30 22:31:00.000000 ReverseShell-0.0.3/clients/shellclientdns.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3698 2023-04-30 22:30:50.000000 ReverseShell-0.0.3/clients/shellclienthttp_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3862 2023-04-30 22:30:42.000000 ReverseShell-0.0.3/clients/shellclienthttps_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4734 2023-04-30 22:30:26.000000 ReverseShell-0.0.3/clients/shellclienthttpsencrypt_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2941 2023-04-30 22:30:34.000000 ReverseShell-0.0.3/clients/shellclientsocketirc.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2153 2023-04-30 22:30:02.000000 ReverseShell-0.0.3/clients/shellclientsockettcp.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2114 2023-04-30 23:10:40.000000 ReverseShell-0.0.3/clients/shellclienttcp.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3125 2023-04-30 22:29:52.000000 ReverseShell-0.0.3/clients/shellclienttcp_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2176 2023-04-30 22:29:44.000000 ReverseShell-0.0.3/clients/shellclientudp.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-30 18:19:23.599891 ReverseShell-0.0.3/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1745 2023-04-30 18:18:55.000000 ReverseShell-0.0.3/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-30 19:20:35.961567 ReverseShell-0.0.4/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35821 2023-04-30 18:10:03.000000 ReverseShell-0.0.4/LICENSE.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       51 2023-04-30 18:10:59.000000 ReverseShell-0.0.4/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     6119 2023-04-30 19:20:35.961567 ReverseShell-0.0.4/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     5044 2023-04-30 23:50:08.000000 ReverseShell-0.0.4/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-30 19:20:35.961567 ReverseShell-0.0.4/ReverseShell.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     6119 2023-04-30 19:20:35.000000 ReverseShell-0.0.4/ReverseShell.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      570 2023-04-30 19:20:35.000000 ReverseShell-0.0.4/ReverseShell.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-30 19:20:35.000000 ReverseShell-0.0.4/ReverseShell.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       51 2023-04-30 19:20:35.000000 ReverseShell-0.0.4/ReverseShell.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-04-30 19:20:35.000000 ReverseShell-0.0.4/ReverseShell.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-04-30 19:20:35.000000 ReverseShell-0.0.4/ReverseShell.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    23201 2023-04-30 19:11:40.000000 ReverseShell-0.0.4/ReverseShell.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-30 19:20:35.961567 ReverseShell-0.0.4/clients/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3258 2023-04-30 22:31:00.000000 ReverseShell-0.0.4/clients/shellclientdns.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3724 2023-04-30 19:18:24.000000 ReverseShell-0.0.4/clients/shellclienthttp_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3888 2023-04-30 19:18:58.000000 ReverseShell-0.0.4/clients/shellclienthttps_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4760 2023-04-30 19:16:33.000000 ReverseShell-0.0.4/clients/shellclienthttpsencrypt_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2941 2023-04-30 22:30:34.000000 ReverseShell-0.0.4/clients/shellclientsocketirc.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2153 2023-04-30 22:30:02.000000 ReverseShell-0.0.4/clients/shellclientsockettcp.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2114 2023-04-30 23:10:40.000000 ReverseShell-0.0.4/clients/shellclienttcp.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3151 2023-04-30 19:19:45.000000 ReverseShell-0.0.4/clients/shellclienttcp_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2176 2023-04-30 22:29:44.000000 ReverseShell-0.0.4/clients/shellclientudp.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-30 19:20:35.961567 ReverseShell-0.0.4/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1745 2023-04-30 19:11:52.000000 ReverseShell-0.0.4/setup.py
```

### Comparing `ReverseShell-0.0.3/LICENSE.txt` & `ReverseShell-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.3/PKG-INFO` & `ReverseShell-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseShell
-Version: 0.0.3
+Version: 0.0.4
 Summary: This package implements an advanced reverse shell console (supports: TCP, UDP, IRC, HTTP and DNS).
 Home-page: https://github.com/mauricelambert/ReverseShell
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `ReverseShell-0.0.3/README.md` & `ReverseShell-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.3/ReverseShell.egg-info/PKG-INFO` & `ReverseShell-0.0.4/ReverseShell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseShell
-Version: 0.0.3
+Version: 0.0.4
 Summary: This package implements an advanced reverse shell console (supports: TCP, UDP, IRC, HTTP and DNS).
 Home-page: https://github.com/mauricelambert/ReverseShell
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `ReverseShell-0.0.3/ReverseShell.egg-info/SOURCES.txt` & `ReverseShell-0.0.4/ReverseShell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.3/ReverseShell.py` & `ReverseShell-0.0.4/ReverseShell.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ###################
 
 """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
 """
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
@@ -90,24 +90,24 @@
     key: if is not None decrypt received data and encrypt
     data to send with the key.
     """
 
     prompt: str = "~$ "
     _set: bool = False
     color: bool = True
+    executables: List[str] = []
+    files: List[str] = []
 
     def __init__(
         self,
         *args,
         key: bytes = None,
         encoding: str = "utf-8" if name != "nt" else "cp437",
     ):
         self.encoding = encoding
-        self.files: List[str] = []
-        self.executables: List[str] = []
         self.key = key and self.init_key(key)
         Cmd.__init__(self)
         BaseRequestHandler.__init__(self, *args)
 
     def recv(self) -> bytes:
         """
         This method gets all packets sent.
@@ -159,16 +159,16 @@
                 f"\x1b[38;2;37;161;127m{hostname}\x1b[39m@"
                 f"\x1b[38;2;47;99;161m{user}\x1b[39m:"
                 f"\x1b[38;2;246;172;56m{cwd}\x1b[39m$ "
             )
             if self.color
             else f"{hostname}@{user}:{cwd}$ "
         )
-        self.executables = data.get("executables", [])
-        self.files = data.get("files", [])
+        self.__class__.executables = data.get("executables", [])
+        self.__class__.files = data.get("files", [])
         ReverseShell._set = True
 
     def parse_data(self, data: bytes) -> str:
         """
         This function parses TCP data.
         """
```

### Comparing `ReverseShell-0.0.3/clients/shellclientdns.py` & `ReverseShell-0.0.4/clients/shellclientdns.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.3/clients/shellclienthttp_advanced.py` & `ReverseShell-0.0.4/clients/shellclienthttp_advanced.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,17 @@
 from contextlib import suppress
 from subprocess import run, PIPE
 from os import getcwd, environ, listdir, name
 
 
 def get_executables():
     return [
-        listdir(directory)
+        file
         for directory in environ["PATH"].split(":" if name != "nt" else ";")
+        for file in listdir(directory)
         if exists(directory)
     ]
 
 
 format_ = b"POST / HTTP/1.0\r\nContent-Type: {type}\r\nHost: 127.0.0.1\r\nContent-Length: {length}\r\n\r\n"
 
 while True:
```

### Comparing `ReverseShell-0.0.3/clients/shellclienthttps_advanced.py` & `ReverseShell-0.0.4/clients/shellclienthttps_advanced.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,17 @@
 from subprocess import run, PIPE
 from ssl import _create_unverified_context
 from os import getcwd, environ, listdir, name
 
 
 def get_executables():
     return [
-        listdir(directory)
+        file
         for directory in environ["PATH"].split(":" if name != "nt" else ";")
+        for file in listdir(directory)
         if exists(directory)
     ]
 
 
 format_ = b"POST / HTTP/1.0\r\nContent-Type: {type}\r\nHost: 127.0.0.1\r\nContent-Length: {length}\r\n\r\n"
 context = _create_unverified_context()
```

### Comparing `ReverseShell-0.0.3/clients/shellclienthttpsencrypt_advanced.py` & `ReverseShell-0.0.4/clients/shellclienthttpsencrypt_advanced.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,17 @@
     if decrypt:
         return bytes(out)
     return iv + bytes(out)
 
 
 def get_executables():
     return [
-        listdir(directory)
+        file
         for directory in environ["PATH"].split(":" if name != "nt" else ";")
+        for file in listdir(directory)
         if exists(directory)
     ]
 
 
 format_ = b"POST / HTTP/1.0\r\nContent-Type: {type}\r\nHost: 127.0.0.1\r\nContent-Length: {length}\r\n\r\n"
 context = _create_unverified_context()
```

### Comparing `ReverseShell-0.0.3/clients/shellclientsocketirc.py` & `ReverseShell-0.0.4/clients/shellclientsocketirc.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.3/clients/shellclientsockettcp.py` & `ReverseShell-0.0.4/clients/shellclientsockettcp.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.3/clients/shellclienttcp.py` & `ReverseShell-0.0.4/clients/shellclienttcp.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.3/clients/shellclienttcp_advanced.py` & `ReverseShell-0.0.4/clients/shellclienttcp_advanced.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,17 @@
 from contextlib import suppress
 from subprocess import run, PIPE
 from os import getcwd, environ, listdir, name
 
 
 def get_executables():
     return [
-        listdir(directory)
+        file
         for directory in environ["PATH"].split(":" if name != "nt" else ";")
+        for file in listdir(directory)
         if exists(directory)
     ]
 
 
 while True:
     with suppress(Exception):
         recevied = b""
```

### Comparing `ReverseShell-0.0.3/clients/shellclientudp.py` & `ReverseShell-0.0.4/clients/shellclientudp.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.3/setup.py` & `ReverseShell-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from glob import glob
 
 setup(
     name="ReverseShell",
-    version="0.0.3",
+    version="0.0.4",
     py_modules=["ReverseShell"],
     install_requires=["PythonToolsKit"],
     author="Maurice Lambert",
     author_email="mauricelambert434@gmail.com",
     maintainer="Maurice Lambert",
     maintainer_email="mauricelambert434@gmail.com",
     description=(
```

