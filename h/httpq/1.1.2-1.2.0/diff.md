# Comparing `tmp/httpq-1.1.2.tar.gz` & `tmp/httpq-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpq-1.1.2.tar", last modified: Wed Jun  8 19:06:03 2022, max compression
+gzip compressed data, was "httpq-1.2.0.tar", last modified: Sun Apr 30 20:17:17 2023, max compression
```

## Comparing `httpq-1.1.2.tar` & `httpq-1.2.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 19:06:03.149768 httpq-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 19:06:03.145768 httpq-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 19:06:03.149768 httpq-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1317 2022-06-08 19:05:43.000000 httpq-1.1.2/.github/workflows/docs-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-06-08 19:05:43.000000 httpq-1.1.2/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-06-08 19:05:43.000000 httpq-1.1.2/.github/workflows/pytest-cover-run.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-06-08 19:06:03.000000 httpq-1.1.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-06-08 19:06:03.000000 httpq-1.1.2/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-06-08 19:05:43.000000 httpq-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5800 2022-06-08 19:06:03.149768 httpq-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4878 2022-06-08 19:05:43.000000 httpq-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 19:06:03.149768 httpq-1.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-06-08 19:05:43.000000 httpq-1.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-06-08 19:05:43.000000 httpq-1.1.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-06-08 19:05:43.000000 httpq-1.1.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 19:06:03.149768 httpq-1.1.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)     2218 2022-06-08 19:05:43.000000 httpq-1.1.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-06-08 19:05:43.000000 httpq-1.1.2/docs/source/contents.rst
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-06-08 19:05:43.000000 httpq-1.1.2/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 19:06:03.149768 httpq-1.1.2/docs/source/module/
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-06-08 19:05:43.000000 httpq-1.1.2/docs/source/module/httpq.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 19:06:03.149768 httpq-1.1.2/docs/source/writeups/
--rw-r--r--   0 runner    (1001) docker     (121)     6105 2022-06-08 19:05:43.000000 httpq-1.1.2/docs/source/writeups/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6478 2022-06-08 19:05:43.000000 httpq-1.1.2/docs/source/writeups/state-machine.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 19:06:03.149768 httpq-1.1.2/httpq/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-06-08 19:05:43.000000 httpq-1.1.2/httpq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8262 2022-06-08 19:05:43.000000 httpq-1.1.2/httpq/httpq.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 19:06:03.149768 httpq-1.1.2/httpq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5800 2022-06-08 19:06:03.000000 httpq-1.1.2/httpq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-06-08 19:06:03.000000 httpq-1.1.2/httpq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-08 19:06:03.000000 httpq-1.1.2/httpq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-08 19:05:58.000000 httpq-1.1.2/httpq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-06-08 19:06:03.000000 httpq-1.1.2/httpq.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-06-08 19:06:03.000000 httpq-1.1.2/httpq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-08 19:06:03.000000 httpq-1.1.2/httpq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-08 19:05:43.000000 httpq-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-08 19:05:43.000000 httpq-1.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-06-08 19:06:03.153768 httpq-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-06-08 19:05:43.000000 httpq-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 19:06:03.149768 httpq-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-08 19:05:43.000000 httpq-1.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-06-08 19:05:43.000000 httpq-1.1.2/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4343 2022-06-08 19:05:43.000000 httpq-1.1.2/tests/test_httpq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:17:17.593799 httpq-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:17:17.593799 httpq-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:17:17.593799 httpq-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-30 20:17:01.000000 httpq-1.2.0/.github/workflows/docs-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-30 20:17:01.000000 httpq-1.2.0/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-30 20:17:01.000000 httpq-1.2.0/.github/workflows/pytest-cover-run.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-30 20:17:17.000000 httpq-1.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-30 20:17:17.000000 httpq-1.2.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-30 20:17:01.000000 httpq-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-30 20:17:17.593799 httpq-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-04-30 20:17:01.000000 httpq-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:17:17.593799 httpq-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-30 20:17:01.000000 httpq-1.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-30 20:17:01.000000 httpq-1.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-30 20:17:01.000000 httpq-1.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:17:17.593799 httpq-1.2.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-30 20:17:01.000000 httpq-1.2.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-30 20:17:01.000000 httpq-1.2.0/docs/source/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-30 20:17:01.000000 httpq-1.2.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:17:17.593799 httpq-1.2.0/docs/source/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-30 20:17:01.000000 httpq-1.2.0/docs/source/module/httpq.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:17:17.593799 httpq-1.2.0/docs/source/writeups/
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-04-30 20:17:01.000000 httpq-1.2.0/docs/source/writeups/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-04-30 20:17:01.000000 httpq-1.2.0/docs/source/writeups/state-machine.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:17:17.593799 httpq-1.2.0/httpq/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-30 20:17:01.000000 httpq-1.2.0/httpq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-04-30 20:17:01.000000 httpq-1.2.0/httpq/httpq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:17:17.593799 httpq-1.2.0/httpq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-30 20:17:17.000000 httpq-1.2.0/httpq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-30 20:17:17.000000 httpq-1.2.0/httpq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 20:17:17.000000 httpq-1.2.0/httpq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 20:17:11.000000 httpq-1.2.0/httpq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-30 20:17:17.000000 httpq-1.2.0/httpq.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-30 20:17:17.000000 httpq-1.2.0/httpq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 20:17:17.000000 httpq-1.2.0/httpq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-30 20:17:01.000000 httpq-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-30 20:17:01.000000 httpq-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-30 20:17:17.593799 httpq-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-30 20:17:01.000000 httpq-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:17:17.593799 httpq-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 20:17:01.000000 httpq-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-30 20:17:01.000000 httpq-1.2.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-04-30 20:17:01.000000 httpq-1.2.0/tests/test_httpq.py
```

### Comparing `httpq-1.1.2/.github/workflows/docs-publish.yaml` & `httpq-1.2.0/.github/workflows/docs-publish.yaml`

 * *Files identical despite different names*

### Comparing `httpq-1.1.2/.github/workflows/pypi-publish.yaml` & `httpq-1.2.0/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `httpq-1.1.2/.github/workflows/pytest-cover-run.yaml` & `httpq-1.2.0/.github/workflows/pytest-cover-run.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
       - '*'
 
 jobs:
   pytest:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.6, 3.7, 3.8, 3.9, '3.10']
+        python-version: [3.7, 3.8, 3.9, '3.10']
     steps:
     - name: Checks repo out
       uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `httpq-1.1.2/LICENSE` & `httpq-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `httpq-1.1.2/PKG-INFO` & `httpq-1.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: httpq
-Version: 1.1.2
+Version: 1.2.0
 Summary: Parse, modify, and compile HTTP/1.1 messages.
 Home-page: https://github.com/synchronizing/httpq
 Author: Felipe Faria
 Author-email: felipefaria@me.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/synchronizing/httpq/issues
 Project-URL: Documentation, https://synchronizing.github.io/httpq/
 Project-URL: Source Code, https://github.com/synchronizing/httpq/tree/master
 Keywords: httpq
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS
 
 # 🏃‍♂️ httpq
 
@@ -65,59 +64,69 @@
 ```python
 import httpq
 
 req = httpq.Request(
     method="GET",
     target="/get",
     protocol="HTTP/1.1",
-    headers={"Host": "httpbin.org", "Content-Length": 12},
+    headers={
+        "Host": "httpbin.org",
+        "Content-Length": 12,
+        "Accept": ["Accept: application/json", "Accept: text/plain"],
+    },
     body="Hello world!",
 )
 
 resp = httpq.Response(
     protocol="HTTP/1.1",
     status=200,
     reason="OK",
-    headers={"Content-Length": 12},
+    headers={"Content-Length": 12, "Content-Type": "text/plain"},
     body="Hello world!",
 )
 ```
 
 #### `parse`
 
 ```python
 req = httpq.Request.parse(
     b"GET /get HTTP/1.1\r\n"
     b"Host: httpbin.org\r\n"
     b"Content-Length: 12\r\n"
+    b"Accept: application/json\r\n"
+    b"Accept: text/plain\r\n"
     b"\r\n"
     b"Hello world!"
 )
 
 resp = httpq.Response.parse(
     b"HTTP/1.1 200 OK\r\n"
     b"Content-Length: 12\r\n"
+    b"Content-Type: text/plain\r\n"
     b"\r\n"
     b"Hello world!"
 )
 ```
 
 #### `feed`
 
 ```python
 req = httpq.Request()
 req.feed(b"GET /get HTTP/1.1\r\n")
 req.feed(b"Host: httpbin.org\r\n")
 req.feed(b"Content-Length: 18\r\n")
+req.feed(b"Accept: application/json\r\n")
+req.feed(b"Accept: text/plain\r\n")
 req.feed(b"\r\n")
 req.feed(b"Hello world!")
 
 resp = httpq.Response()
 resp.feed(b"HTTP/1.1 200 OK\r\n")
 resp.feed(b"Content-Length: 12\r\n")
+resp.feed(b"Content-Type: text/plain\r\n")
 resp.feed(b"\r\n")
 resp.feed(b"Hello world!")
 ```
 
 The feed mechanism comes with a simple built-in state machine. The state machine can be in one of three states:
 
 * `TOP`: The feed cursor is at the top of the message.
@@ -145,15 +154,40 @@
 while resp.state != httpq.state.BODY:
     resp.feed(s.recv(10))
 
 # At this stage we have a response that has read the top line and headers. It's the user's
 # responsibility to keep track of the rest of the message's length. In this case, we'll just
 # use the `Content-Length` header.
 while len(resp.body) != resp.headers["Content-Length"]:
-    body += s.recv(10)
+    resp.feed(s.recv(10))
+
+print(resp)
+```
+
+Outputs:
+
+```
+← HTTP/1.1 200 OK
+← Date: Sun, 12 Mar 2023 03:05:55 GMT
+← Content-Type: application/json
+← Content-Length: 197
+← Connection: keep-alive
+← Server: gunicorn/19.9.0
+← Access-Control-Allow-Origin: *
+← Access-Control-Allow-Credentials: true
+← 
+← {
+←   "args": {}, 
+←   "headers": {
+←     "Host": "httpbin.org", 
+←     "X-Amzn-Trace-Id": "Root=1-640d4193-650c50825ec4415732dacde8"
+←   }, 
+←   "origin": "xx.xx.xx.xxx", 
+←   "url": "http://httpbin.org/get"
+← }
 ```
 
 Note that the feed mechanism is used in conjunction with the `state` property. We can use this parse until the body of the message, and then use the captured headers to parse the body.
 
 ### Modifying and Comparisons
 
 `httpq` also comes with an intuitive method to modify and compare message values:
@@ -225,9 +259,7 @@
 ← Accept: */*
 ← 
 ← Hello world!
 ```
 
 Checkout the documentation for more details.
 
-
-
```

#### html2text {}

```diff
@@ -1,61 +1,71 @@
-Metadata-Version: 2.1 Name: httpq Version: 1.1.2 Summary: Parse, modify, and
+Metadata-Version: 2.1 Name: httpq Version: 1.2.0 Summary: Parse, modify, and
 compile HTTP/1.1 messages. Home-page: https://github.com/synchronizing/httpq
 Author: Felipe Faria Author-email: felipefaria@me.com License: MIT Project-URL:
 Bug Tracker, https://github.com/synchronizing/httpq/issues Project-URL:
 Documentation, https://synchronizing.github.io/httpq/ Project-URL: Source Code,
-https://github.com/synchronizing/httpq/tree/master Keywords: httpq Platform:
-UNKNOWN Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
-OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
-Topic :: Software Development :: Libraries Classifier: Topic :: Utilities
-Requires-Python: >=3.5 Description-Content-Type: text/markdown; charset=UTF-
-8 Provides-Extra: dev License-File: LICENSE License-File: AUTHORS #
-ðââï¸ httpq
+https://github.com/synchronizing/httpq/tree/master Keywords: httpq Classifier:
+Programming Language :: Python :: Implementation :: CPython Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: MIT License Classifier: Natural Language :: English Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Utilities Requires-
+Python: >=3.7 Description-Content-Type: text/markdown; charset=UTF-8 Provides-
+Extra: dev License-File: LICENSE License-File: AUTHORS # ðââï¸ httpq
     [https://github.com/synchronizing/httpq/actions/workflows/pytest-cover-
 run.yaml/badge.svg] [https://github.com/synchronizing/httpq/actions/workflows/
 docs-publish.yaml/badge.svg] [https://coveralls.io/repos/github/synchronizing/
    httpq/badge.svg?branch=master] [https://img.shields.io/badge/License-MIT-
                                   yellow.svg]
 httpq is a small (~32KB) package to parse, modify, and compile HTTP/1.1
 messages with a built-in state machine. ## Installing ``` pip install httpq ```
 ## Documentation Documentation can be found [here](https://
 synchronizing.github.io/httpq/). ## Using `httpq` has three methods to
 initialize a `httpq.Request` and `httpq.Response` object. #### `__init__`
 ```python import httpq req = httpq.Request( method="GET", target="/get",
-protocol="HTTP/1.1", headers={"Host": "httpbin.org", "Content-Length": 12},
-body="Hello world!", ) resp = httpq.Response( protocol="HTTP/1.1", status=200,
-reason="OK", headers={"Content-Length": 12}, body="Hello world!", ) ``` ####
-`parse` ```python req = httpq.Request.parse( b"GET /get HTTP/1.1\r\n" b"Host:
-httpbin.org\r\n" b"Content-Length: 12\r\n" b"\r\n" b"Hello world!" ) resp =
-httpq.Response.parse( b"HTTP/1.1 200 OK\r\n" b"Content-Length: 12\r\n" b"\r\n"
-b"Hello world!" ) ``` #### `feed` ```python req = httpq.Request() req.feed
-(b"GET /get HTTP/1.1\r\n") req.feed(b"Host: httpbin.org\r\n") req.feed
-(b"Content-Length: 18\r\n") req.feed(b"\r\n") req.feed(b"Hello world!") resp =
-httpq.Response() resp.feed(b"HTTP/1.1 200 OK\r\n") resp.feed(b"Content-Length:
-12\r\n") resp.feed(b"\r\n") resp.feed(b"Hello world!") ``` The feed mechanism
-comes with a simple built-in state machine. The state machine can be in one of
-three states: * `TOP`: The feed cursor is at the top of the message. *
-`HEADER`: The feed cursor is at the headers. * `BODY`: The feed cursor is at
+protocol="HTTP/1.1", headers={ "Host": "httpbin.org", "Content-Length": 12,
+"Accept": ["Accept: application/json", "Accept: text/plain"], }, body="Hello
+world!", ) resp = httpq.Response( protocol="HTTP/1.1", status=200, reason="OK",
+headers={"Content-Length": 12, "Content-Type": "text/plain"}, body="Hello
+world!", ) ``` #### `parse` ```python req = httpq.Request.parse( b"GET /get
+HTTP/1.1\r\n" b"Host: httpbin.org\r\n" b"Content-Length: 12\r\n" b"Accept:
+application/json\r\n" b"Accept: text/plain\r\n" b"\r\n" b"Hello world!" ) resp
+= httpq.Response.parse( b"HTTP/1.1 200 OK\r\n" b"Content-Length: 12\r\n"
+b"Content-Type: text/plain\r\n" b"\r\n" b"Hello world!" ) ``` #### `feed`
+```python req = httpq.Request() req.feed(b"GET /get HTTP/1.1\r\n") req.feed
+(b"Host: httpbin.org\r\n") req.feed(b"Content-Length: 18\r\n") req.feed
+(b"Accept: application/json\r\n") req.feed(b"Accept: text/plain\r\n") req.feed
+(b"\r\n") req.feed(b"Hello world!") resp = httpq.Response() resp.feed(b"HTTP/
+1.1 200 OK\r\n") resp.feed(b"Content-Length: 12\r\n") resp.feed(b"Content-Type:
+text/plain\r\n") resp.feed(b"\r\n") resp.feed(b"Hello world!") ``` The feed
+mechanism comes with a simple built-in state machine. The state machine can be
+in one of three states: * `TOP`: The feed cursor is at the top of the message.
+* `HEADER`: The feed cursor is at the headers. * `BODY`: The feed cursor is at
 the body. Once at the body it's the user's responsibility to keep track of the
 message length. ```python import socket import httpq s = socket.socket
 (socket.AF_INET, socket.SOCK_STREAM) s.connect(("httpbin.org", 80)) req =
 httpq.Request( method="GET", target="/get", protocol="HTTP/1.1", headers=
 {"Host": "httpbin.org"}, ) s.sendall(req.raw) resp = httpq.Response() while
 resp.state != httpq.state.BODY: resp.feed(s.recv(10)) # At this stage we have a
 response that has read the top line and headers. It's the user's #
 responsibility to keep track of the rest of the message's length. In this case,
 we'll just # use the `Content-Length` header. while len(resp.body) !=
-resp.headers["Content-Length"]: body += s.recv(10) ``` Note that the feed
-mechanism is used in conjunction with the `state` property. We can use this
-parse until the body of the message, and then use the captured headers to parse
-the body. ### Modifying and Comparisons `httpq` also comes with an intuitive
-method to modify and compare message values: ```python import httpq req =
-httpq.Request( method="GET", target="/get", protocol="HTTP/1.1", headers=
-{"Host": "httpbin.org", "Content-Length": 12}, body="Hello world!", ) resp =
+resp.headers["Content-Length"]: resp.feed(s.recv(10)) print(resp) ``` Outputs:
+``` â HTTP/1.1 200 OK â Date: Sun, 12 Mar 2023 03:05:55 GMT â Content-
+Type: application/json â Content-Length: 197 â Connection: keep-alive â
+Server: gunicorn/19.9.0 â Access-Control-Allow-Origin: * â Access-Control-
+Allow-Credentials: true â â { â "args": {}, â "headers": { â "Host":
+"httpbin.org", â "X-Amzn-Trace-Id": "Root=1-640d4193-
+650c50825ec4415732dacde8" â }, â "origin": "xx.xx.xx.xxx", â "url":
+"http://httpbin.org/get" â } ``` Note that the feed mechanism is used in
+conjunction with the `state` property. We can use this parse until the body of
+the message, and then use the captured headers to parse the body. ### Modifying
+and Comparisons `httpq` also comes with an intuitive method to modify and
+compare message values: ```python import httpq req = httpq.Request
+( method="GET", target="/get", protocol="HTTP/1.1", headers={"Host":
+"httpbin.org", "Content-Length": 12}, body="Hello world!", ) resp =
 httpq.Response( protocol="HTTP/1.1", status=404, reason="Not Found", headers=
 {"Content-Length": 12}, body="Hello world!", ) # string, bytes, and int are all
 valid values for any field. req.method = "POST" req.target = b"/" resp.status =
 200 resp.reason = "OK" resp.headers += {"Accept": "*/*"} ``` Internally every
 value of a request or response is saved as an `Item`, a special object type
 that allows easy setting and comparisons on the fly. ```python resp.status ==
 200 # >>> True resp.status == "200" # >>> True resp.status == b"200" # >>> True
```

### Comparing `httpq-1.1.2/README.md` & `httpq-1.2.0/httpq.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: httpq
+Version: 1.2.0
+Summary: Parse, modify, and compile HTTP/1.1 messages.
+Home-page: https://github.com/synchronizing/httpq
+Author: Felipe Faria
+Author-email: felipefaria@me.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/synchronizing/httpq/issues
+Project-URL: Documentation, https://synchronizing.github.io/httpq/
+Project-URL: Source Code, https://github.com/synchronizing/httpq/tree/master
+Keywords: httpq
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown; charset=UTF-8
+Provides-Extra: dev
+License-File: LICENSE
+License-File: AUTHORS
+
 # 🏃‍♂️ httpq
 
 <p align="center">
 
   <a href="https://github.com/synchronizing/httpq/actions/workflows/pytest-cover-run.yaml">
     <img src="https://github.com/synchronizing/httpq/actions/workflows/pytest-cover-run.yaml/badge.svg">
   </a>
@@ -40,59 +64,69 @@
 ```python
 import httpq
 
 req = httpq.Request(
     method="GET",
     target="/get",
     protocol="HTTP/1.1",
-    headers={"Host": "httpbin.org", "Content-Length": 12},
+    headers={
+        "Host": "httpbin.org",
+        "Content-Length": 12,
+        "Accept": ["Accept: application/json", "Accept: text/plain"],
+    },
     body="Hello world!",
 )
 
 resp = httpq.Response(
     protocol="HTTP/1.1",
     status=200,
     reason="OK",
-    headers={"Content-Length": 12},
+    headers={"Content-Length": 12, "Content-Type": "text/plain"},
     body="Hello world!",
 )
 ```
 
 #### `parse`
 
 ```python
 req = httpq.Request.parse(
     b"GET /get HTTP/1.1\r\n"
     b"Host: httpbin.org\r\n"
     b"Content-Length: 12\r\n"
+    b"Accept: application/json\r\n"
+    b"Accept: text/plain\r\n"
     b"\r\n"
     b"Hello world!"
 )
 
 resp = httpq.Response.parse(
     b"HTTP/1.1 200 OK\r\n"
     b"Content-Length: 12\r\n"
+    b"Content-Type: text/plain\r\n"
     b"\r\n"
     b"Hello world!"
 )
 ```
 
 #### `feed`
 
 ```python
 req = httpq.Request()
 req.feed(b"GET /get HTTP/1.1\r\n")
 req.feed(b"Host: httpbin.org\r\n")
 req.feed(b"Content-Length: 18\r\n")
+req.feed(b"Accept: application/json\r\n")
+req.feed(b"Accept: text/plain\r\n")
 req.feed(b"\r\n")
 req.feed(b"Hello world!")
 
 resp = httpq.Response()
 resp.feed(b"HTTP/1.1 200 OK\r\n")
 resp.feed(b"Content-Length: 12\r\n")
+resp.feed(b"Content-Type: text/plain\r\n")
 resp.feed(b"\r\n")
 resp.feed(b"Hello world!")
 ```
 
 The feed mechanism comes with a simple built-in state machine. The state machine can be in one of three states:
 
 * `TOP`: The feed cursor is at the top of the message.
@@ -120,15 +154,40 @@
 while resp.state != httpq.state.BODY:
     resp.feed(s.recv(10))
 
 # At this stage we have a response that has read the top line and headers. It's the user's
 # responsibility to keep track of the rest of the message's length. In this case, we'll just
 # use the `Content-Length` header.
 while len(resp.body) != resp.headers["Content-Length"]:
-    body += s.recv(10)
+    resp.feed(s.recv(10))
+
+print(resp)
+```
+
+Outputs:
+
+```
+← HTTP/1.1 200 OK
+← Date: Sun, 12 Mar 2023 03:05:55 GMT
+← Content-Type: application/json
+← Content-Length: 197
+← Connection: keep-alive
+← Server: gunicorn/19.9.0
+← Access-Control-Allow-Origin: *
+← Access-Control-Allow-Credentials: true
+← 
+← {
+←   "args": {}, 
+←   "headers": {
+←     "Host": "httpbin.org", 
+←     "X-Amzn-Trace-Id": "Root=1-640d4193-650c50825ec4415732dacde8"
+←   }, 
+←   "origin": "xx.xx.xx.xxx", 
+←   "url": "http://httpbin.org/get"
+← }
 ```
 
 Note that the feed mechanism is used in conjunction with the `state` property. We can use this parse until the body of the message, and then use the captured headers to parse the body.
 
 ### Modifying and Comparisons
 
 `httpq` also comes with an intuitive method to modify and compare message values:
@@ -199,7 +258,8 @@
 ← Content-Length: 12
 ← Accept: */*
 ← 
 ← Hello world!
 ```
 
 Checkout the documentation for more details.
+
```

#### html2text {}

```diff
@@ -1,49 +1,71 @@
-# ðââï¸ httpq
+Metadata-Version: 2.1 Name: httpq Version: 1.2.0 Summary: Parse, modify, and
+compile HTTP/1.1 messages. Home-page: https://github.com/synchronizing/httpq
+Author: Felipe Faria Author-email: felipefaria@me.com License: MIT Project-URL:
+Bug Tracker, https://github.com/synchronizing/httpq/issues Project-URL:
+Documentation, https://synchronizing.github.io/httpq/ Project-URL: Source Code,
+https://github.com/synchronizing/httpq/tree/master Keywords: httpq Classifier:
+Programming Language :: Python :: Implementation :: CPython Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: MIT License Classifier: Natural Language :: English Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Utilities Requires-
+Python: >=3.7 Description-Content-Type: text/markdown; charset=UTF-8 Provides-
+Extra: dev License-File: LICENSE License-File: AUTHORS # ðââï¸ httpq
     [https://github.com/synchronizing/httpq/actions/workflows/pytest-cover-
 run.yaml/badge.svg] [https://github.com/synchronizing/httpq/actions/workflows/
 docs-publish.yaml/badge.svg] [https://coveralls.io/repos/github/synchronizing/
    httpq/badge.svg?branch=master] [https://img.shields.io/badge/License-MIT-
                                   yellow.svg]
 httpq is a small (~32KB) package to parse, modify, and compile HTTP/1.1
 messages with a built-in state machine. ## Installing ``` pip install httpq ```
 ## Documentation Documentation can be found [here](https://
 synchronizing.github.io/httpq/). ## Using `httpq` has three methods to
 initialize a `httpq.Request` and `httpq.Response` object. #### `__init__`
 ```python import httpq req = httpq.Request( method="GET", target="/get",
-protocol="HTTP/1.1", headers={"Host": "httpbin.org", "Content-Length": 12},
-body="Hello world!", ) resp = httpq.Response( protocol="HTTP/1.1", status=200,
-reason="OK", headers={"Content-Length": 12}, body="Hello world!", ) ``` ####
-`parse` ```python req = httpq.Request.parse( b"GET /get HTTP/1.1\r\n" b"Host:
-httpbin.org\r\n" b"Content-Length: 12\r\n" b"\r\n" b"Hello world!" ) resp =
-httpq.Response.parse( b"HTTP/1.1 200 OK\r\n" b"Content-Length: 12\r\n" b"\r\n"
-b"Hello world!" ) ``` #### `feed` ```python req = httpq.Request() req.feed
-(b"GET /get HTTP/1.1\r\n") req.feed(b"Host: httpbin.org\r\n") req.feed
-(b"Content-Length: 18\r\n") req.feed(b"\r\n") req.feed(b"Hello world!") resp =
-httpq.Response() resp.feed(b"HTTP/1.1 200 OK\r\n") resp.feed(b"Content-Length:
-12\r\n") resp.feed(b"\r\n") resp.feed(b"Hello world!") ``` The feed mechanism
-comes with a simple built-in state machine. The state machine can be in one of
-three states: * `TOP`: The feed cursor is at the top of the message. *
-`HEADER`: The feed cursor is at the headers. * `BODY`: The feed cursor is at
+protocol="HTTP/1.1", headers={ "Host": "httpbin.org", "Content-Length": 12,
+"Accept": ["Accept: application/json", "Accept: text/plain"], }, body="Hello
+world!", ) resp = httpq.Response( protocol="HTTP/1.1", status=200, reason="OK",
+headers={"Content-Length": 12, "Content-Type": "text/plain"}, body="Hello
+world!", ) ``` #### `parse` ```python req = httpq.Request.parse( b"GET /get
+HTTP/1.1\r\n" b"Host: httpbin.org\r\n" b"Content-Length: 12\r\n" b"Accept:
+application/json\r\n" b"Accept: text/plain\r\n" b"\r\n" b"Hello world!" ) resp
+= httpq.Response.parse( b"HTTP/1.1 200 OK\r\n" b"Content-Length: 12\r\n"
+b"Content-Type: text/plain\r\n" b"\r\n" b"Hello world!" ) ``` #### `feed`
+```python req = httpq.Request() req.feed(b"GET /get HTTP/1.1\r\n") req.feed
+(b"Host: httpbin.org\r\n") req.feed(b"Content-Length: 18\r\n") req.feed
+(b"Accept: application/json\r\n") req.feed(b"Accept: text/plain\r\n") req.feed
+(b"\r\n") req.feed(b"Hello world!") resp = httpq.Response() resp.feed(b"HTTP/
+1.1 200 OK\r\n") resp.feed(b"Content-Length: 12\r\n") resp.feed(b"Content-Type:
+text/plain\r\n") resp.feed(b"\r\n") resp.feed(b"Hello world!") ``` The feed
+mechanism comes with a simple built-in state machine. The state machine can be
+in one of three states: * `TOP`: The feed cursor is at the top of the message.
+* `HEADER`: The feed cursor is at the headers. * `BODY`: The feed cursor is at
 the body. Once at the body it's the user's responsibility to keep track of the
 message length. ```python import socket import httpq s = socket.socket
 (socket.AF_INET, socket.SOCK_STREAM) s.connect(("httpbin.org", 80)) req =
 httpq.Request( method="GET", target="/get", protocol="HTTP/1.1", headers=
 {"Host": "httpbin.org"}, ) s.sendall(req.raw) resp = httpq.Response() while
 resp.state != httpq.state.BODY: resp.feed(s.recv(10)) # At this stage we have a
 response that has read the top line and headers. It's the user's #
 responsibility to keep track of the rest of the message's length. In this case,
 we'll just # use the `Content-Length` header. while len(resp.body) !=
-resp.headers["Content-Length"]: body += s.recv(10) ``` Note that the feed
-mechanism is used in conjunction with the `state` property. We can use this
-parse until the body of the message, and then use the captured headers to parse
-the body. ### Modifying and Comparisons `httpq` also comes with an intuitive
-method to modify and compare message values: ```python import httpq req =
-httpq.Request( method="GET", target="/get", protocol="HTTP/1.1", headers=
-{"Host": "httpbin.org", "Content-Length": 12}, body="Hello world!", ) resp =
+resp.headers["Content-Length"]: resp.feed(s.recv(10)) print(resp) ``` Outputs:
+``` â HTTP/1.1 200 OK â Date: Sun, 12 Mar 2023 03:05:55 GMT â Content-
+Type: application/json â Content-Length: 197 â Connection: keep-alive â
+Server: gunicorn/19.9.0 â Access-Control-Allow-Origin: * â Access-Control-
+Allow-Credentials: true â â { â "args": {}, â "headers": { â "Host":
+"httpbin.org", â "X-Amzn-Trace-Id": "Root=1-640d4193-
+650c50825ec4415732dacde8" â }, â "origin": "xx.xx.xx.xxx", â "url":
+"http://httpbin.org/get" â } ``` Note that the feed mechanism is used in
+conjunction with the `state` property. We can use this parse until the body of
+the message, and then use the captured headers to parse the body. ### Modifying
+and Comparisons `httpq` also comes with an intuitive method to modify and
+compare message values: ```python import httpq req = httpq.Request
+( method="GET", target="/get", protocol="HTTP/1.1", headers={"Host":
+"httpbin.org", "Content-Length": 12}, body="Hello world!", ) resp =
 httpq.Response( protocol="HTTP/1.1", status=404, reason="Not Found", headers=
 {"Content-Length": 12}, body="Hello world!", ) # string, bytes, and int are all
 valid values for any field. req.method = "POST" req.target = b"/" resp.status =
 200 resp.reason = "OK" resp.headers += {"Accept": "*/*"} ``` Internally every
 value of a request or response is saved as an `Item`, a special object type
 that allows easy setting and comparisons on the fly. ```python resp.status ==
 200 # >>> True resp.status == "200" # >>> True resp.status == b"200" # >>> True
```

### Comparing `httpq-1.1.2/docs/Makefile` & `httpq-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `httpq-1.1.2/docs/make.bat` & `httpq-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `httpq-1.1.2/docs/source/conf.py` & `httpq-1.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `httpq-1.1.2/docs/source/module/httpq.rst` & `httpq-1.2.0/docs/source/module/httpq.rst`

 * *Files identical despite different names*

### Comparing `httpq-1.1.2/docs/source/writeups/quickstart.rst` & `httpq-1.2.0/docs/source/writeups/quickstart.rst`

 * *Files identical despite different names*

### Comparing `httpq-1.1.2/docs/source/writeups/state-machine.rst` & `httpq-1.2.0/docs/source/writeups/state-machine.rst`

 * *Files identical despite different names*

### Comparing `httpq-1.1.2/httpq/httpq.py` & `httpq-1.2.0/httpq/httpq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,88 @@
 """
 `httpq` implementation.
 """
 
+from __future__ import annotations
+
 import enum
 from abc import ABC, abstractmethod
 from typing import Any, Optional, Union
 
 from toolbox.collections.item import Item, ItemType
-from toolbox.collections.mapping import (
-    ItemDict,
-    ObjectDict,
-    OverloadedDict,
-    UnderscoreAccessDict,
-)
+from toolbox.collections.mapping import ItemDict, MultiEntryDict, ObjectDict, OverloadedDict, UnderscoreAccessDict
 
 
 class state(enum.Enum):
     """
     States of the HTTP request.
     """
 
     TOP = 0
     HEADER = 1
     BODY = 2
 
 
-class Headers(ObjectDict, OverloadedDict, UnderscoreAccessDict, ItemDict):
+class Headers(ItemDict, ObjectDict, OverloadedDict, UnderscoreAccessDict, MultiEntryDict):
+
     """
     Container for HTTP headers.
     """
 
     def _compile(self) -> bytes:
         """
         Compile the headers.
         """
-        return b"%s\r\n" % b"".join(b"%s: %s\r\n" % (k.raw, v.raw) for k, v in self.items())
+        lines = []
+        for k, v in self.items():
+            if isinstance(v, list):
+                string = b"%s: " % k.raw + b", ".join([i.raw for i in self[k]]) + b"\r\n"
+            else:
+                string = b"%s: %s\r\n" % (k.raw, v.raw)
+
+            lines.append(string)
+
+        return b"%s\r\n" % b"".join(lines)
+
+    def __setitem__(self, key: Any, value: Any):
+        """
+        Deletes the previous value of the item and sets the new value.
+
+        Args:
+            key: The key of the item.
+            value: The value of the item.
+        """
+        if key in self:
+            del self[key]
+
+        super().__setitem__(key, value)
+
+    def __defaultsetitem__(self, key: Any, value: Any):
+        """
+        Sets the value of the item without deleting the previous value.
+
+        Args:
+            key: The key of the item.
+            value: The value of the item.
+        """
+        super().__setitem__(key, value)
 
     @property
     def raw(self) -> bytes:
         """
         The raw headers.
         """
         return self._compile()
 
 
 InpType = Optional[ItemType]
 HeadersType = Union[Headers, dict]
 
 
 class Message(ABC):
-
     __slots__ = ("protocol", "headers", "body", "buffer")
 
     def __init__(
         self,
         protocol: InpType = None,
         headers: HeadersType = {},
         body: InpType = None,
@@ -103,39 +132,42 @@
             raise TypeError("Message must be bytes.")
 
         self.buffer += msg
         return self.state
 
     @property
     def state(self) -> state:
-        """
-        Retrieves the state of the HTTP message.
-        """
-
         if self.buffer.count(b"\r\n") > 0 and b"\r\n\r\n" not in self.buffer:
             return state.HEADER
         elif self.buffer.count(b"\r\n") == 0:
             return state.TOP
 
         current = state.TOP
         _, body = self.buffer.split(b"\r\n\r\n", 1)
 
         # Split the message into lines.
         for line in self.buffer.split(b"\r\n"):
-
             # Parses the first line of the HTTP/1.1 msg.
             if current == state.TOP:
                 self._parse_top(line)
                 current = state.HEADER
 
             # Parse the headers of the HTTP/1.1 msg.
             elif current == state.HEADER:
                 if b":" in line:
                     key, value = line.split(b":", 1)
-                    self.headers[key] = value.strip()
+
+                    if b"," in value:
+                        value = value.split(b",")
+                    else:
+                        value = [value]
+
+                    for v in value:
+                        if key not in self.headers or v.strip() not in self.headers[key]:
+                            self.headers.__defaultsetitem__(key, v.strip())
                 else:
                     current = state.BODY
 
         if current == state.BODY:
             self.body = body
 
         return current
@@ -175,14 +207,20 @@
     @property
     def raw(self) -> bytes:
         """
         Returns the raw (bytes) HTTP message.
         """
         return self._compile()
 
+    def __eq__(self, other: Message) -> bool:
+        """
+        Compares two HTTP messages.
+        """
+        return self.raw == other.raw
+
     def __str__(self) -> str:
         """
         Pretty-print of the HTTP message.
         """
 
         if self.__class__ == Request:
             arrow = "→ "
@@ -191,15 +229,14 @@
         else:  # pragma: no cover
             arrow = "? "
 
         return arrow + arrow.join(self._compile().decode("utf-8").rstrip("\r\n").splitlines(True))
 
 
 class Request(Message):
-
     __slots__ = Message.__slots__ + ("method", "target")
 
     def __init__(
         self,
         method: InpType = None,
         target: InpType = None,
         protocol: InpType = None,
@@ -248,15 +285,14 @@
         """
         Compiles the first line of the HTTP request.
         """
         return b"%s %s %s\r\n" % (self.method.raw, self.target.raw, self.protocol.raw)
 
 
 class Response(Message):
-
     __slots__ = Message.__slots__ + ("status", "reason")
 
     def __init__(
         self,
         protocol: InpType = None,
         status: InpType = None,
         reason: InpType = None,
```

### Comparing `httpq-1.1.2/httpq.egg-info/PKG-INFO` & `httpq-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: httpq
-Version: 1.1.2
-Summary: Parse, modify, and compile HTTP/1.1 messages.
-Home-page: https://github.com/synchronizing/httpq
-Author: Felipe Faria
-Author-email: felipefaria@me.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/synchronizing/httpq/issues
-Project-URL: Documentation, https://synchronizing.github.io/httpq/
-Project-URL: Source Code, https://github.com/synchronizing/httpq/tree/master
-Keywords: httpq
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: dev
-License-File: LICENSE
-License-File: AUTHORS
-
 # 🏃‍♂️ httpq
 
 <p align="center">
 
   <a href="https://github.com/synchronizing/httpq/actions/workflows/pytest-cover-run.yaml">
     <img src="https://github.com/synchronizing/httpq/actions/workflows/pytest-cover-run.yaml/badge.svg">
   </a>
@@ -65,59 +40,69 @@
 ```python
 import httpq
 
 req = httpq.Request(
     method="GET",
     target="/get",
     protocol="HTTP/1.1",
-    headers={"Host": "httpbin.org", "Content-Length": 12},
+    headers={
+        "Host": "httpbin.org",
+        "Content-Length": 12,
+        "Accept": ["Accept: application/json", "Accept: text/plain"],
+    },
     body="Hello world!",
 )
 
 resp = httpq.Response(
     protocol="HTTP/1.1",
     status=200,
     reason="OK",
-    headers={"Content-Length": 12},
+    headers={"Content-Length": 12, "Content-Type": "text/plain"},
     body="Hello world!",
 )
 ```
 
 #### `parse`
 
 ```python
 req = httpq.Request.parse(
     b"GET /get HTTP/1.1\r\n"
     b"Host: httpbin.org\r\n"
     b"Content-Length: 12\r\n"
+    b"Accept: application/json\r\n"
+    b"Accept: text/plain\r\n"
     b"\r\n"
     b"Hello world!"
 )
 
 resp = httpq.Response.parse(
     b"HTTP/1.1 200 OK\r\n"
     b"Content-Length: 12\r\n"
+    b"Content-Type: text/plain\r\n"
     b"\r\n"
     b"Hello world!"
 )
 ```
 
 #### `feed`
 
 ```python
 req = httpq.Request()
 req.feed(b"GET /get HTTP/1.1\r\n")
 req.feed(b"Host: httpbin.org\r\n")
 req.feed(b"Content-Length: 18\r\n")
+req.feed(b"Accept: application/json\r\n")
+req.feed(b"Accept: text/plain\r\n")
 req.feed(b"\r\n")
 req.feed(b"Hello world!")
 
 resp = httpq.Response()
 resp.feed(b"HTTP/1.1 200 OK\r\n")
 resp.feed(b"Content-Length: 12\r\n")
+resp.feed(b"Content-Type: text/plain\r\n")
 resp.feed(b"\r\n")
 resp.feed(b"Hello world!")
 ```
 
 The feed mechanism comes with a simple built-in state machine. The state machine can be in one of three states:
 
 * `TOP`: The feed cursor is at the top of the message.
@@ -145,15 +130,40 @@
 while resp.state != httpq.state.BODY:
     resp.feed(s.recv(10))
 
 # At this stage we have a response that has read the top line and headers. It's the user's
 # responsibility to keep track of the rest of the message's length. In this case, we'll just
 # use the `Content-Length` header.
 while len(resp.body) != resp.headers["Content-Length"]:
-    body += s.recv(10)
+    resp.feed(s.recv(10))
+
+print(resp)
+```
+
+Outputs:
+
+```
+← HTTP/1.1 200 OK
+← Date: Sun, 12 Mar 2023 03:05:55 GMT
+← Content-Type: application/json
+← Content-Length: 197
+← Connection: keep-alive
+← Server: gunicorn/19.9.0
+← Access-Control-Allow-Origin: *
+← Access-Control-Allow-Credentials: true
+← 
+← {
+←   "args": {}, 
+←   "headers": {
+←     "Host": "httpbin.org", 
+←     "X-Amzn-Trace-Id": "Root=1-640d4193-650c50825ec4415732dacde8"
+←   }, 
+←   "origin": "xx.xx.xx.xxx", 
+←   "url": "http://httpbin.org/get"
+← }
 ```
 
 Note that the feed mechanism is used in conjunction with the `state` property. We can use this parse until the body of the message, and then use the captured headers to parse the body.
 
 ### Modifying and Comparisons
 
 `httpq` also comes with an intuitive method to modify and compare message values:
@@ -224,10 +234,7 @@
 ← Content-Length: 12
 ← Accept: */*
 ← 
 ← Hello world!
 ```
 
 Checkout the documentation for more details.
-
-
-
```

#### html2text {}

```diff
@@ -1,61 +1,60 @@
-Metadata-Version: 2.1 Name: httpq Version: 1.1.2 Summary: Parse, modify, and
-compile HTTP/1.1 messages. Home-page: https://github.com/synchronizing/httpq
-Author: Felipe Faria Author-email: felipefaria@me.com License: MIT Project-URL:
-Bug Tracker, https://github.com/synchronizing/httpq/issues Project-URL:
-Documentation, https://synchronizing.github.io/httpq/ Project-URL: Source Code,
-https://github.com/synchronizing/httpq/tree/master Keywords: httpq Platform:
-UNKNOWN Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
-OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
-Topic :: Software Development :: Libraries Classifier: Topic :: Utilities
-Requires-Python: >=3.5 Description-Content-Type: text/markdown; charset=UTF-
-8 Provides-Extra: dev License-File: LICENSE License-File: AUTHORS #
-ðââï¸ httpq
+# ðââï¸ httpq
     [https://github.com/synchronizing/httpq/actions/workflows/pytest-cover-
 run.yaml/badge.svg] [https://github.com/synchronizing/httpq/actions/workflows/
 docs-publish.yaml/badge.svg] [https://coveralls.io/repos/github/synchronizing/
    httpq/badge.svg?branch=master] [https://img.shields.io/badge/License-MIT-
                                   yellow.svg]
 httpq is a small (~32KB) package to parse, modify, and compile HTTP/1.1
 messages with a built-in state machine. ## Installing ``` pip install httpq ```
 ## Documentation Documentation can be found [here](https://
 synchronizing.github.io/httpq/). ## Using `httpq` has three methods to
 initialize a `httpq.Request` and `httpq.Response` object. #### `__init__`
 ```python import httpq req = httpq.Request( method="GET", target="/get",
-protocol="HTTP/1.1", headers={"Host": "httpbin.org", "Content-Length": 12},
-body="Hello world!", ) resp = httpq.Response( protocol="HTTP/1.1", status=200,
-reason="OK", headers={"Content-Length": 12}, body="Hello world!", ) ``` ####
-`parse` ```python req = httpq.Request.parse( b"GET /get HTTP/1.1\r\n" b"Host:
-httpbin.org\r\n" b"Content-Length: 12\r\n" b"\r\n" b"Hello world!" ) resp =
-httpq.Response.parse( b"HTTP/1.1 200 OK\r\n" b"Content-Length: 12\r\n" b"\r\n"
-b"Hello world!" ) ``` #### `feed` ```python req = httpq.Request() req.feed
-(b"GET /get HTTP/1.1\r\n") req.feed(b"Host: httpbin.org\r\n") req.feed
-(b"Content-Length: 18\r\n") req.feed(b"\r\n") req.feed(b"Hello world!") resp =
-httpq.Response() resp.feed(b"HTTP/1.1 200 OK\r\n") resp.feed(b"Content-Length:
-12\r\n") resp.feed(b"\r\n") resp.feed(b"Hello world!") ``` The feed mechanism
-comes with a simple built-in state machine. The state machine can be in one of
-three states: * `TOP`: The feed cursor is at the top of the message. *
-`HEADER`: The feed cursor is at the headers. * `BODY`: The feed cursor is at
+protocol="HTTP/1.1", headers={ "Host": "httpbin.org", "Content-Length": 12,
+"Accept": ["Accept: application/json", "Accept: text/plain"], }, body="Hello
+world!", ) resp = httpq.Response( protocol="HTTP/1.1", status=200, reason="OK",
+headers={"Content-Length": 12, "Content-Type": "text/plain"}, body="Hello
+world!", ) ``` #### `parse` ```python req = httpq.Request.parse( b"GET /get
+HTTP/1.1\r\n" b"Host: httpbin.org\r\n" b"Content-Length: 12\r\n" b"Accept:
+application/json\r\n" b"Accept: text/plain\r\n" b"\r\n" b"Hello world!" ) resp
+= httpq.Response.parse( b"HTTP/1.1 200 OK\r\n" b"Content-Length: 12\r\n"
+b"Content-Type: text/plain\r\n" b"\r\n" b"Hello world!" ) ``` #### `feed`
+```python req = httpq.Request() req.feed(b"GET /get HTTP/1.1\r\n") req.feed
+(b"Host: httpbin.org\r\n") req.feed(b"Content-Length: 18\r\n") req.feed
+(b"Accept: application/json\r\n") req.feed(b"Accept: text/plain\r\n") req.feed
+(b"\r\n") req.feed(b"Hello world!") resp = httpq.Response() resp.feed(b"HTTP/
+1.1 200 OK\r\n") resp.feed(b"Content-Length: 12\r\n") resp.feed(b"Content-Type:
+text/plain\r\n") resp.feed(b"\r\n") resp.feed(b"Hello world!") ``` The feed
+mechanism comes with a simple built-in state machine. The state machine can be
+in one of three states: * `TOP`: The feed cursor is at the top of the message.
+* `HEADER`: The feed cursor is at the headers. * `BODY`: The feed cursor is at
 the body. Once at the body it's the user's responsibility to keep track of the
 message length. ```python import socket import httpq s = socket.socket
 (socket.AF_INET, socket.SOCK_STREAM) s.connect(("httpbin.org", 80)) req =
 httpq.Request( method="GET", target="/get", protocol="HTTP/1.1", headers=
 {"Host": "httpbin.org"}, ) s.sendall(req.raw) resp = httpq.Response() while
 resp.state != httpq.state.BODY: resp.feed(s.recv(10)) # At this stage we have a
 response that has read the top line and headers. It's the user's #
 responsibility to keep track of the rest of the message's length. In this case,
 we'll just # use the `Content-Length` header. while len(resp.body) !=
-resp.headers["Content-Length"]: body += s.recv(10) ``` Note that the feed
-mechanism is used in conjunction with the `state` property. We can use this
-parse until the body of the message, and then use the captured headers to parse
-the body. ### Modifying and Comparisons `httpq` also comes with an intuitive
-method to modify and compare message values: ```python import httpq req =
-httpq.Request( method="GET", target="/get", protocol="HTTP/1.1", headers=
-{"Host": "httpbin.org", "Content-Length": 12}, body="Hello world!", ) resp =
+resp.headers["Content-Length"]: resp.feed(s.recv(10)) print(resp) ``` Outputs:
+``` â HTTP/1.1 200 OK â Date: Sun, 12 Mar 2023 03:05:55 GMT â Content-
+Type: application/json â Content-Length: 197 â Connection: keep-alive â
+Server: gunicorn/19.9.0 â Access-Control-Allow-Origin: * â Access-Control-
+Allow-Credentials: true â â { â "args": {}, â "headers": { â "Host":
+"httpbin.org", â "X-Amzn-Trace-Id": "Root=1-640d4193-
+650c50825ec4415732dacde8" â }, â "origin": "xx.xx.xx.xxx", â "url":
+"http://httpbin.org/get" â } ``` Note that the feed mechanism is used in
+conjunction with the `state` property. We can use this parse until the body of
+the message, and then use the captured headers to parse the body. ### Modifying
+and Comparisons `httpq` also comes with an intuitive method to modify and
+compare message values: ```python import httpq req = httpq.Request
+( method="GET", target="/get", protocol="HTTP/1.1", headers={"Host":
+"httpbin.org", "Content-Length": 12}, body="Hello world!", ) resp =
 httpq.Response( protocol="HTTP/1.1", status=404, reason="Not Found", headers=
 {"Content-Length": 12}, body="Hello world!", ) # string, bytes, and int are all
 valid values for any field. req.method = "POST" req.target = b"/" resp.status =
 200 resp.reason = "OK" resp.headers += {"Accept": "*/*"} ``` Internally every
 value of a request or response is saved as an `Item`, a special object type
 that allows easy setting and comparisons on the fly. ```python resp.status ==
 200 # >>> True resp.status == "200" # >>> True resp.status == b"200" # >>> True
```

### Comparing `httpq-1.1.2/httpq.egg-info/SOURCES.txt` & `httpq-1.2.0/httpq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `httpq-1.1.2/setup.cfg` & `httpq-1.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = httpq
 author = Felipe Faria
 author-email = felipefaria@me.com
 summary = Parse, modify, and compile HTTP/1.1 messages.
 description-file = README.md
 description-content-type = text/markdown; charset=UTF-8
-requires-python = >=3.5
+requires-python = >=3.7
 home-page = https://github.com/synchronizing/httpq
 project_urls = 
 	Bug Tracker = https://github.com/synchronizing/httpq/issues
 	Documentation = https://synchronizing.github.io/httpq/
 	Source Code = https://github.com/synchronizing/httpq/tree/master
 license = MIT
 classifier =
```

