# Comparing `tmp/swim-protocol-0.3.9.tar.gz` & `tmp/swim_protocol-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swim-protocol-0.3.9.tar", last modified: Wed Jul 27 23:57:37 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `swim-protocol-0.3.9.tar` & `swim_protocol-0.4.0.tar`

### file list

```diff
@@ -1,37 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 23:57:37.859172 swim-protocol-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8424 2022-07-27 23:57:37.859172 swim-protocol-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6667 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-07-27 23:57:37.859172 swim-protocol-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2322 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 23:57:37.855172 swim-protocol-0.3.9/swim_protocol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8424 2022-07-27 23:57:37.000000 swim-protocol-0.3.9/swim_protocol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-07-27 23:57:37.000000 swim-protocol-0.3.9/swim_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-27 23:57:37.000000 swim-protocol-0.3.9/swim_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-07-27 23:57:37.000000 swim-protocol-0.3.9/swim_protocol.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-27 23:57:37.000000 swim-protocol-0.3.9/swim_protocol.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 23:57:37.859172 swim-protocol-0.3.9/swimprotocol/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/address.py
--rw-r--r--   0 runner    (1001) docker     (121)     8504 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 23:57:37.859172 swim-protocol-0.3.9/swimprotocol/demo/
--rw-r--r--   0 runner    (1001) docker     (121)     2400 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/demo/changes.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/demo/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     4397 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/demo/screen.py
--rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/listener.py
--rw-r--r--   0 runner    (1001) docker     (121)    11671 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/members.py
--rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/packet.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3261 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (121)     2334 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/sign.py
--rw-r--r--   0 runner    (1001) docker     (121)     1949 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     2611 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 23:57:37.859172 swim-protocol-0.3.9/swimprotocol/udp/
--rw-r--r--   0 runner    (1001) docker     (121)     8469 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4127 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/udp/pack.py
--rw-r--r--   0 runner    (1001) docker     (121)     2978 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/udp/protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)     9389 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/swimprotocol/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 23:57:37.859172 swim-protocol-0.3.9/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2367 2022-07-27 23:57:27.000000 swim-protocol-0.3.9/test/test_shuffle.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/.lvimrc
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/__init__.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/address.py
+-rw-r--r--   0        0        0     8461 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/config.py
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/listener.py
+-rw-r--r--   0        0        0    11701 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/members.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/packet.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/py.typed
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/shuffle.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/sign.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/status.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/transport.py
+-rw-r--r--   0        0        0     9666 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/worker.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/demo/__init__.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/demo/changes.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/demo/log.py
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/demo/screen.py
+-rw-r--r--   0        0        0     8469 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/udp/__init__.py
+-rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/udp/pack.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/swimprotocol/udp/protocol.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/test/test_shuffle.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/README.md
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8745 2020-02-02 00:00:00.000000 swim_protocol-0.4.0/PKG-INFO
```

### Comparing `swim-protocol-0.3.9/LICENSE.md` & `swim_protocol-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.9/PKG-INFO` & `swim_protocol-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,56 @@
 Metadata-Version: 2.1
 Name: swim-protocol
-Version: 0.3.9
+Version: 0.4.0
 Summary: SWIM protocol implementation for exchanging cluster membership status and metadata.
-Home-page: https://github.com/icgood/swim-protocol/
-Author: Ian Good
-Author-email: ian@icgood.net
-License: MIT
+Project-URL: Homepage, https://github.com/icgood/swim-protocol/
+Project-URL: API Documentation, https://icgood.github.io/swim-protocol/
+Author-email: Ian Good <ian@icgood.net>
+License: ## MIT License
+        
+        Copyright (c) 2021 Ian Good
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: ~=3.9
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
 
 swim-protocol
 =============
 
 [SWIM protocol][0] implementation for exchanging cluster membership status and
 metadata.
 
-[![build](https://github.com/icgood/swim-protocol/actions/workflows/python-package.yml/badge.svg)](https://github.com/icgood/swim-protocol/actions/workflows/python-package.yml)
-[![Coverage Status](https://coveralls.io/repos/github/icgood/swim-protocol/badge.svg?branch=main)](https://coveralls.io/github/icgood/swim-protocol?branch=main)
+[![build](https://github.com/icgood/swim-protocol/actions/workflows/python-check.yml/badge.svg)](https://github.com/icgood/swim-protocol/actions/workflows/python-check.yml)
 [![PyPI](https://img.shields.io/pypi/v/swim-protocol.svg)](https://pypi.python.org/pypi/swim-protocol)
 [![PyPI](https://img.shields.io/pypi/pyversions/swim-protocol.svg)](https://pypi.python.org/pypi/swim-protocol)
+![platforms](https://img.shields.io/badge/platform-linux%20%7C%20macOS%20%7C%20windows-blueviolet)
 [![PyPI](https://img.shields.io/pypi/l/swim-protocol.svg)](https://pypi.python.org/pypi/swim-protocol)
 
 This library is intended to fit into an [asyncio][1] event loop to help
 synchronize a distributed group of processes.
 
 #### [Introduction](https://icgood.github.io/swim-protocol/intro.html)
 
@@ -145,19 +165,28 @@
 private networks should be used if metadata includes any secret data, or that
 secret data should be encrypted separately by the application. Also be aware
 that low [MTU][10] sizes on public networks may affect the ability to
 synchronize larger amounts of metadata.
 
 ## Development
 
-First off, I suggest activating a [venv][3]. Then, install the development
-requirements and a local link to the *swim-protocol* package:
+You will need to do some additional setup to develop and test plugins. Install
+[Hatch][3] to use the CLI examples below.
+
+Run all tests and linters:
 
+```console
+$ hatch run check
 ```
-$ pip install -r requirements-dev.txt
+
+Because this project supports several versions of Python, you can use the
+following to run the checks on all versions:
+
+```console
+$ hatch run all:check
 ```
 
 ### Type Hinting
 
 This project makes heavy use of Python's [type hinting][4] system, with the
 intention of a clean run of [mypy][5]:
 
@@ -167,15 +196,15 @@
 
 No code contribution will be accepted unless it makes every effort to use type
 hinting to the extent possible and common in the rest of the codebase.
 
 [0]: https://www.cs.cornell.edu/projects/Quicksilver/public_pdfs/SWIM.pdf
 [1]: https://docs.python.org/3/library/asyncio.html
 [2]: https://github.com/icgood/swim-protocol/blob/main/swimprotocol/demo/__init__.py
-[3]: https://docs.python.org/3/library/venv.html
+[3]: https://hatch.pypa.io/latest/install/
 [4]: https://docs.python.org/3/library/typing.html
 [5]: http://mypy-lang.org/
 [6]: https://en.wikipedia.org/wiki/Eventual_consistency
 [7]: https://docs.python.org/3/library/hmac.html
 [8]: https://en.wikipedia.org/wiki/Shared_secret
 [9]: https://docs.python.org/3/library/uuid.html#uuid.getnode
 [10]: https://en.wikipedia.org/wiki/Maximum_transmission_unit
@@ -183,28 +212,7 @@
 [12]: https://icgood.github.io/swim-protocol/swimprotocol.html#swimprotocol.transport.load_transport
 [13]: https://docs.docker.com/engine/swarm/how-swarm-mode-works/services/
 [14]: https://icgood.github.io/swim-protocol/swimprotocol.udp.html#docker-services
 
 [100]: https://icgood.github.io/swim-protocol/swimprotocol.udp.html#swimprotocol.udp.UdpConfig
 [101]: https://icgood.github.io/swim-protocol/swimprotocol.html#swimprotocol.members.Member
 [102]: https://icgood.github.io/swim-protocol/swimprotocol.udp.html#swimprotocol.udp.UdpTransport
-## MIT License
-
-Copyright (c) 2021 Ian Good
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
```

### Comparing `swim-protocol-0.3.9/README.md` & `swim_protocol-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 swim-protocol
 =============
 
 [SWIM protocol][0] implementation for exchanging cluster membership status and
 metadata.
 
-[![build](https://github.com/icgood/swim-protocol/actions/workflows/python-package.yml/badge.svg)](https://github.com/icgood/swim-protocol/actions/workflows/python-package.yml)
-[![Coverage Status](https://coveralls.io/repos/github/icgood/swim-protocol/badge.svg?branch=main)](https://coveralls.io/github/icgood/swim-protocol?branch=main)
+[![build](https://github.com/icgood/swim-protocol/actions/workflows/python-check.yml/badge.svg)](https://github.com/icgood/swim-protocol/actions/workflows/python-check.yml)
 [![PyPI](https://img.shields.io/pypi/v/swim-protocol.svg)](https://pypi.python.org/pypi/swim-protocol)
 [![PyPI](https://img.shields.io/pypi/pyversions/swim-protocol.svg)](https://pypi.python.org/pypi/swim-protocol)
+![platforms](https://img.shields.io/badge/platform-linux%20%7C%20macOS%20%7C%20windows-blueviolet)
 [![PyPI](https://img.shields.io/pypi/l/swim-protocol.svg)](https://pypi.python.org/pypi/swim-protocol)
 
 This library is intended to fit into an [asyncio][1] event loop to help
 synchronize a distributed group of processes.
 
 #### [Introduction](https://icgood.github.io/swim-protocol/intro.html)
 
@@ -126,19 +126,28 @@
 private networks should be used if metadata includes any secret data, or that
 secret data should be encrypted separately by the application. Also be aware
 that low [MTU][10] sizes on public networks may affect the ability to
 synchronize larger amounts of metadata.
 
 ## Development
 
-First off, I suggest activating a [venv][3]. Then, install the development
-requirements and a local link to the *swim-protocol* package:
+You will need to do some additional setup to develop and test plugins. Install
+[Hatch][3] to use the CLI examples below.
 
+Run all tests and linters:
+
+```console
+$ hatch run check
 ```
-$ pip install -r requirements-dev.txt
+
+Because this project supports several versions of Python, you can use the
+following to run the checks on all versions:
+
+```console
+$ hatch run all:check
 ```
 
 ### Type Hinting
 
 This project makes heavy use of Python's [type hinting][4] system, with the
 intention of a clean run of [mypy][5]:
 
@@ -148,15 +157,15 @@
 
 No code contribution will be accepted unless it makes every effort to use type
 hinting to the extent possible and common in the rest of the codebase.
 
 [0]: https://www.cs.cornell.edu/projects/Quicksilver/public_pdfs/SWIM.pdf
 [1]: https://docs.python.org/3/library/asyncio.html
 [2]: https://github.com/icgood/swim-protocol/blob/main/swimprotocol/demo/__init__.py
-[3]: https://docs.python.org/3/library/venv.html
+[3]: https://hatch.pypa.io/latest/install/
 [4]: https://docs.python.org/3/library/typing.html
 [5]: http://mypy-lang.org/
 [6]: https://en.wikipedia.org/wiki/Eventual_consistency
 [7]: https://docs.python.org/3/library/hmac.html
 [8]: https://en.wikipedia.org/wiki/Shared_secret
 [9]: https://docs.python.org/3/library/uuid.html#uuid.getnode
 [10]: https://en.wikipedia.org/wiki/Maximum_transmission_unit
```

### Comparing `swim-protocol-0.3.9/swimprotocol/address.py` & `swim_protocol-0.4.0/swimprotocol/address.py`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.9/swimprotocol/config.py` & `swim_protocol-0.4.0/swimprotocol/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 
 from __future__ import annotations
 
 import os
-from abc import ABCMeta
 from argparse import ArgumentParser, Namespace
 from collections.abc import Mapping, Sequence
 from pathlib import Path
 from typing import final, TypeVar, Final, Any, Union, Optional
 
 from .sign import Signatures
 
@@ -38,15 +37,15 @@
 
     def __init__(self, msg: Optional[str] = None, *,
                  wait_hint: float = 60.0) -> None:
         super().__init__(msg)
         self.wait_hint: Final = wait_hint
 
 
-class BaseConfig(metaclass=ABCMeta):
+class BaseConfig:
     """Configure the cluster behavior and characteristics.
     :class:`~swimprotocol.transport.Transport` implementations should
     sub-class to add additional configuration.
 
     Args:
         secret: The shared secret for cluster packet signatures.
         local_name: The unique name of the local cluster member.
```

### Comparing `swim-protocol-0.3.9/swimprotocol/demo/__init__.py` & `swim_protocol-0.4.0/swimprotocol/demo/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 approximately 10 seconds, a metadata field "token" is updated on each cluster
 member, and should be disseminated to all other members.
 
 """
 
 from __future__ import annotations
 
+import sys
+assert sys.platform != 'win32'
+
+# ruff: noqa: E402
+
 import asyncio
 import logging
 import signal
 from argparse import Namespace, ArgumentParser
 from asyncio import CancelledError
 from contextlib import suppress, AsyncExitStack
```

### Comparing `swim-protocol-0.3.9/swimprotocol/demo/changes.py` & `swim_protocol-0.4.0/swimprotocol/demo/changes.py`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.9/swimprotocol/demo/screen.py` & `swim_protocol-0.4.0/swimprotocol/demo/screen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 
 from __future__ import annotations
 
+import sys
+assert sys.platform != 'win32'
+
+# ruff: noqa: E402
+
 import asyncio
 import curses
 import string
 from contextlib import AsyncExitStack
 from curses import wrapper
 from functools import partial
 from threading import Event, Condition
@@ -99,15 +104,15 @@
         stdscr.clear()
         stdscr.timeout(0)
         typed = b''
         while not self.done.is_set():
             stdscr.clear()
             self._render(stdscr)
             stdscr.refresh()
-            for i in range(20):
+            for _ in range(20):
                 with self.ready:
                     if self.ready.wait(timeout=0.05):
                         break
                 ch = stdscr.getch()
                 if _is_printable(ch):
                     typed += bytes([ch])
                     typed = typed[-30:]
```

### Comparing `swim-protocol-0.3.9/swimprotocol/listener.py` & `swim_protocol-0.4.0/swimprotocol/listener.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from __future__ import annotations
 
 import asyncio
 from abc import abstractmethod
-from asyncio import Event
-from collections.abc import Sequence
+from asyncio import Event, Task
+from collections.abc import MutableSet, Sequence
 from contextlib import ExitStack
 from typing import TypeVar, Generic, Protocol, Any, NoReturn
 from weakref import WeakKeyDictionary
 
 __all__ = ['ListenerCallback', 'Listener']
 
 ListenT = TypeVar('ListenT')
@@ -39,23 +39,27 @@
             :meth:`.poll`, and passed to :meth:`.on_notify` callbacks.
 
     """
 
     def __init__(self, cls: type[ListenT]) -> None:
         super().__init__()
         self.event = Event()
+        self._running: MutableSet[Task[Any]] = set()
         self._waiting: WeakKeyDictionary[Event, list[ListenT]] = \
             WeakKeyDictionary()
 
     async def _run_callback_poll(self, callback: ListenerCallback[ListenT]) \
             -> NoReturn:
+        running = self._running
         while True:
             items = await self.poll()
             for item in items:
-                asyncio.create_task(callback(item))
+                task = asyncio.create_task(callback(item))
+                running.add(task)
+                task.add_done_callback(running.discard)
 
     def on_notify(self, callback: ListenerCallback[ListenT]) -> ExitStack:
         """Provides a context manager that causes *callback* to be called when
         a producer calls :meth:`.notify`.
 
         Args:
             callback: The callback function, which will be passed the *item*
```

### Comparing `swim-protocol-0.3.9/swimprotocol/members.py` & `swim_protocol-0.4.0/swimprotocol/members.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 
     def __len__(self) -> int:
         return len(self._members)
 
     def _refresh_statuses(self, member: Member) -> None:
         if not member.local:
             member_status = member.status
-            for status in Status:
+            for status in Status.all_statuses():
                 if member_status & status:
                     self._statuses[status].add(member)
                 else:
                     self._statuses[status].discard(member)
 
     @property
     def local(self) -> Member:
@@ -233,15 +233,15 @@
 
         """
         member = self._members.get(name)
         if member is None:
             member = Member(name, False)
             self._non_local.add(member)
             self._members[name] = member
-            for status in Status:
+            for status in Status.all_statuses():
                 if member.status & status:
                     self._statuses[status].add(member)
         if not member.local and validity is not None \
                 and member._validity != validity:
             member._known_clocks.clear()
             member._validity = validity
         return member
```

### Comparing `swim-protocol-0.3.9/swimprotocol/packet.py` & `swim_protocol-0.4.0/swimprotocol/packet.py`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.9/swimprotocol/shuffle.py` & `swim_protocol-0.4.0/swimprotocol/shuffle.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     to the set elements.
 
     Args:
         init: Initial objects to add.
 
     """
 
-    def __init__(self, /, init: Iterable[ShuffleT] = []) -> None:
+    def __init__(self, /, init: Iterable[ShuffleT] = ()) -> None:
         super().__init__()
         self._weak_vals: WeakKeyDictionary[ShuffleT, ref[ShuffleT]] = \
             WeakKeyDictionary()
         self._weak_vals_rev: WeakValueDictionary[ref[ShuffleT], ShuffleT] = \
             WeakValueDictionary()
         self._indexes: dict[ref[ShuffleT], int] = {}
         self._values: list[ref[ShuffleT]] = []
@@ -87,17 +87,17 @@
             :func:`random.choice`
 
         Raises:
             KeyError: The set was empty.
 
         """
         try:
-            weak_val = random.choice(self._values)
-        except IndexError:
-            raise KeyError('choice from an empty set')
+            weak_val = random.choice(self._values)  # noqa: S311
+        except IndexError as exc:
+            raise KeyError('choice from an empty set') from exc
         val = weak_val()
         assert val is not None
         return val
 
     def __contains__(self, val: object) -> bool:
         return val in self._weak_vals
```

### Comparing `swim-protocol-0.3.9/swimprotocol/sign.py` & `swim_protocol-0.4.0/swimprotocol/sign.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import hashlib
 import hmac
 import secrets
 import uuid
 from typing import Final, Union
 
-from . import __version__
+from .__about__ import __version__
 
 __all__ = ['Signatures']
 
 _SigTuple = tuple[bytes, bytes]
 
 
 class Signatures:
```

### Comparing `swim-protocol-0.3.9/swimprotocol/status.py` & `swim_protocol-0.4.0/swimprotocol/status.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 from __future__ import annotations
 
+from collections.abc import Collection
 from enum import auto, Flag
 
 __all__ = ['Status']
 
 
 class Status(Flag):
     """Possible cluster member :term:`status` values, as well as aggregate
@@ -54,7 +55,12 @@
             raise ValueError(to)
         elif to == Status.SUSPECT and self == Status.OFFLINE:
             return self
         elif to == Status.OFFLINE and self == Status.ONLINE:
             return Status.SUSPECT
         else:
             return to
+
+    @classmethod
+    def all_statuses(cls) -> Collection[Status]:
+        """A collection of all the statuses, including aggregate statuses."""
+        return cls.__members__.values()
```

### Comparing `swim-protocol-0.3.9/swimprotocol/transport.py` & `swim_protocol-0.4.0/swimprotocol/transport.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 
 from __future__ import annotations
 
 from abc import abstractmethod, ABCMeta
 from contextlib import AbstractAsyncContextManager
-from typing import Generic, TypeVar, Final, ClassVar, Optional
-
-from pkg_resources import iter_entry_points, DistributionNotFound
+from importlib.metadata import entry_points
+from typing import Generic, TypeVar, Final, ClassVar
 
 from .config import ConfigT_co, BaseConfig
 from .members import Members
 from .worker import Worker
 
 __all__ = ['TransportT', 'load_transport', 'Transport']
 
@@ -27,26 +26,18 @@
 
     Raises:
         DistributionNotFound: A dependency of the transport entry point was not
             able to be satisfied.
         KeyError: The given name did not exist in the entry point group.
 
     """
-    last_exc: Optional[DistributionNotFound] = None
-    for entry_point in iter_entry_points(group, name):
-        try:
-            transport_type: type[Transport[BaseConfig]] = entry_point.load()
-        except DistributionNotFound as exc:
-            last_exc = exc
-        else:
-            return transport_type
-    if last_exc is not None:
-        raise last_exc
-    else:
-        raise KeyError(f'{name!r} entry point not found in {group!r}')
+    for entry_point in entry_points(group=group, name=name):
+        transport_type: type[Transport[BaseConfig]] = entry_point.load()
+        return transport_type
+    raise KeyError(f'{name!r} entry point not found in {group!r}')
 
 
 class Transport(Generic[ConfigT_co], metaclass=ABCMeta):
     """Interface of the basic functionality needed to act as the
     :term:`transport` layer for the SWIM protocol. The transport layer is
     responsible for sending and receiving :term:`ping`, :term:`ping-req`, and
     :term:`ack` packets for failure detection, and transmitting :term:`gossip`
```

### Comparing `swim-protocol-0.3.9/swimprotocol/udp/__init__.py` & `swim_protocol-0.4.0/swimprotocol/udp/__init__.py`

 * *Files identical despite different names*

### Comparing `swim-protocol-0.3.9/swimprotocol/udp/pack.py` & `swim_protocol-0.4.0/swimprotocol/udp/pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from __future__ import annotations
 
-import pickle
+import pickle  # nosec
 import struct
 from typing import Final, Optional
 
 from ..packet import Packet
 from ..sign import Signatures
 
 __all__ = ['UdpPack']
@@ -34,15 +34,15 @@
         if len(prefix_xor) != _prefix.size:
             raise ValueError(f'{prefix_xor!r} must be {_prefix.size} bytes')
         self.signatures: Final = signatures
         self.pickle_protocol: Final = pickle_protocol
         self.prefix_xor: Final = prefix_xor
 
     def _xor_prefix(self, prefix: bytes) -> bytes:
-        zipped = zip(prefix, self.prefix_xor)
+        zipped = zip(prefix, self.prefix_xor, strict=True)
         return bytes([left ^ right for left, right in zipped])
 
     def pack(self, packet: Packet) -> bytes:
         """Uses :mod:`pickle` to serialize *packet*, generates a digital
         signature of the pickled data, and returns a byte-string that can be
         sent as a raw UDP packet.
 
@@ -94,12 +94,12 @@
         salt = data_view[salt_start:digest_start]
         digest = data_view[digest_start:data_start]
         pickled = data_view[data_start:data_end]
         signatures = self.signatures
         if len(digest) != signatures.digest_size or len(pickled) != data_len:
             return None
         if signatures.verify(pickled, (salt, digest)):
-            packet = pickle.loads(pickled)
+            packet = pickle.loads(pickled)  # noqa: S301
             assert isinstance(packet, Packet)
             return packet
         else:
             return None
```

### Comparing `swim-protocol-0.3.9/swimprotocol/udp/protocol.py` & `swim_protocol-0.4.0/swimprotocol/udp/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 
 from __future__ import annotations
 
 import asyncio
 import logging
-from asyncio import BaseTransport, Condition, DatagramProtocol, \
+from asyncio import BaseTransport, Condition, Task, DatagramProtocol, \
     DatagramTransport
 from collections import deque
+from collections.abc import MutableSet
 from typing import cast, Final, Optional
 
 from .pack import UdpPack
 from ..address import AddressParser
 from ..members import Member
 from ..packet import Packet
 from ..worker import IO
@@ -30,14 +31,15 @@
                  udp_pack: UdpPack) -> None:
         super().__init__()
         self.address_parser: Final = address_parser
         self.udp_pack: Final = udp_pack
         self._transport: Optional[DatagramTransport] = None
         self._queue_lock = Condition()
         self._queue: deque[Packet] = deque()
+        self._running: MutableSet[Task[None]] = set()
 
     @property
     def transport(self) -> DatagramTransport:
         """The current :class:`~asyncio.DatagramTransport` object."""
         transport = self._transport
         assert transport is not None
         return transport
@@ -57,15 +59,18 @@
         See Also:
             :meth:`asyncio.DatagramProtocol.datagram_received`
 
         """
         packet = self.udp_pack.unpack(data)
         if packet is None:
             return
-        asyncio.create_task(self._push(packet))
+        running = self._running
+        task = asyncio.create_task(self._push(packet))
+        running.add(task)
+        task.add_done_callback(running.discard)
 
     def error_received(self, exc: Exception) -> None:
         """Called when a UDP send or receive operation fails.
 
         See Also:
             :meth:`asyncio.DatagramProtocol.error_received`
```

### Comparing `swim-protocol-0.3.9/swimprotocol/worker.py` & `swim_protocol-0.4.0/swimprotocol/worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from __future__ import annotations
 
 import asyncio
 from abc import abstractmethod
 from asyncio import Event, Task, TimeoutError
-from collections.abc import Mapping, Sequence
+from collections.abc import Mapping, MutableSet, Sequence
 from contextlib import suppress
 from typing import final, Protocol, Final, Optional, NoReturn
 from weakref import WeakSet, WeakKeyDictionary
 
 from .config import BaseConfig
 from .members import Member, Members
 from .packet import Packet, Ping, PingReq, Ack, Gossip, GossipAck
@@ -59,21 +59,27 @@
     """
 
     def __init__(self, config: BaseConfig, members: Members, io: IO) -> None:
         super().__init__()
         self.config: Final = config
         self.members: Final = members
         self.io: Final = io
+        self._running: MutableSet[Task[None]] = set()
         self._waiting: WeakKeyDictionary[Member, WeakSet[Event]] = \
             WeakKeyDictionary()
         self._listening: WeakKeyDictionary[Member, WeakSet[Member]] = \
             WeakKeyDictionary()
         self._suspect: WeakKeyDictionary[Member, Task[None]] = \
             WeakKeyDictionary()
 
+    def _run_task(self, task: Task[None]) -> None:
+        running = self._running
+        running.add(task)
+        task.add_done_callback(running.discard)
+
     def _add_waiting(self, member: Member, event: Event) -> None:
         waiting = self._waiting.get(member)
         if waiting is None:
             self._waiting[member] = waiting = WeakSet()
         waiting.add(event)
 
     def _add_listening(self, member: Member, target: Member) -> None:
@@ -177,16 +183,16 @@
         online = await self._wait(target, self.config.ping_timeout)
         if not online:
             count = self.config.ping_req_count
             indirects = self.members.find(
                 count, status=Status.AVAILABLE, exclude={target})
             if indirects:
                 await asyncio.wait([
-                    self.io.send(indirect, PingReq(
-                        source=local.source, target=target.name))
+                    asyncio.create_task(self.io.send(indirect, PingReq(
+                        source=local.source, target=target.name)))
                     for indirect in indirects])
                 online = await self._wait(target, self.config.ping_req_timeout)
         new_status = Status.ONLINE if online else Status.SUSPECT
         self._handle_status(target, new_status)
         self.members.update(target, new_status=new_status)
 
     @final
@@ -216,15 +222,15 @@
            :class:`ping_interval <swimprotocol.config.Config>` seconds.
 
         """
         while True:
             targets = self.members.find(1)
             assert targets
             for target in targets:
-                asyncio.create_task(self.check(target))
+                self._run_task(asyncio.create_task(self.check(target)))
             await asyncio.sleep(self.config.ping_interval)
 
     async def run_dissemination(self) -> NoReturn:
         """Indefinitely send dissemination packets to other cluster members.
 
         .. note::
 
@@ -232,15 +238,15 @@
            called. By default, one random cluster member is chosen every
            :class:`sync_interval <swimprotocol.config.Config>` seconds.
 
         """
         while True:
             targets = self.members.find(1, status=Status.AVAILABLE)
             for target in targets:
-                asyncio.create_task(self.disseminate(target))
+                self._run_task(asyncio.create_task(self.disseminate(target)))
             await asyncio.sleep(self.config.sync_interval)
 
     @final
     async def run(self) -> NoReturn:
         """Indefinitely handle received SWIM protocol packets and, at
         configurable intervals, send failure detection and dissemination
         packets. This method calls :meth:`.run_failure_detection` and
```

### Comparing `swim-protocol-0.3.9/test/test_shuffle.py` & `swim_protocol-0.4.0/test/test_shuffle.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,45 +29,45 @@
     def test_add_many(self) -> None:
         vals = [_T(), _T(), _T()]
         shuffle = WeakShuffle(vals)
         self.assertEqual(3, len(shuffle))
         self.assertEqual(set(vals), set(shuffle))
         for val in vals:
             self.assertIn(val, shuffle)
-        for i in range(100):
+        for _ in range(100):
             self.assertIn(shuffle.choice(), vals)
 
     def test_discard(self) -> None:
         vals = [_T(), _T(), _T()]
         shuffle = WeakShuffle(vals)
         shuffle.discard(vals[1])
         self.assertEqual(2, len(shuffle))
         self.assertEqual(set([vals[0], vals[2]]), set(shuffle))
-        for i in range(100):
+        for _ in range(100):
             self.assertIn(shuffle.choice(), vals)
         shuffle.discard(vals[2])
         self.assertEqual(1, len(shuffle))
         self.assertEqual(set([vals[0]]), set(shuffle))
-        for i in range(100):
+        for _ in range(100):
             self.assertIn(shuffle.choice(), vals)
         shuffle.discard(vals[0])
         self.assertEqual(0, len(shuffle))
         self.assertEqual(set(), set(shuffle))
         self.assertRaises(KeyError, shuffle.choice)
 
     def test_disappear(self) -> None:
         vals = [_T(), _T(), _T()]
         shuffle = WeakShuffle(vals)
         del vals[1]
         self.assertEqual(2, len(shuffle))
         self.assertEqual(set(vals), set(shuffle))
-        for i in range(100):
+        for _ in range(100):
             self.assertIn(shuffle.choice(), vals)
         del vals[1]
         self.assertEqual(1, len(shuffle))
         self.assertEqual(set(vals), set(shuffle))
-        for i in range(100):
+        for _ in range(100):
             self.assertIn(shuffle.choice(), vals)
         del vals
         self.assertEqual(0, len(shuffle))
         self.assertEqual(set(), set(shuffle))
         self.assertRaises(KeyError, shuffle.choice)
```

