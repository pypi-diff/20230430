# Comparing `tmp/exitstatus-2.3.0.tar.gz` & `tmp/exitstatus-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exitstatus-2.3.0.tar", last modified: Wed Nov  2 13:18:29 2022, max compression
+gzip compressed data, was "exitstatus-2.4.0.tar", last modified: Sun Apr 30 18:56:47 2023, max compression
```

## Comparing `exitstatus-2.3.0.tar` & `exitstatus-2.4.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 hagenjt1   (501) staff       (20)        0 2022-11-02 13:18:29.579414 exitstatus-2.3.0/
--rw-r--r--   0 hagenjt1   (501) staff       (20)     1059 2022-11-02 12:56:02.000000 exitstatus-2.3.0/LICENSE.txt
--rw-r--r--   0 hagenjt1   (501) staff       (20)       67 2022-11-02 12:50:49.000000 exitstatus-2.3.0/MANIFEST.in
--rw-r--r--   0 hagenjt1   (501) staff       (20)     3676 2022-11-02 13:18:29.579013 exitstatus-2.3.0/PKG-INFO
--rw-r--r--   0 hagenjt1   (501) staff       (20)     2912 2022-11-02 13:12:19.000000 exitstatus-2.3.0/README.rst
-drwxr-xr-x   0 hagenjt1   (501) staff       (20)        0 2022-11-02 13:18:29.575424 exitstatus-2.3.0/exitstatus/
--rw-r--r--   0 hagenjt1   (501) staff       (20)      351 2022-11-02 12:47:48.000000 exitstatus-2.3.0/exitstatus/__init__.py
--rw-r--r--   0 hagenjt1   (501) staff       (20)       93 2022-11-02 12:46:42.000000 exitstatus-2.3.0/exitstatus/py.typed
-drwxr-xr-x   0 hagenjt1   (501) staff       (20)        0 2022-11-02 13:18:29.578456 exitstatus-2.3.0/exitstatus.egg-info/
--rw-r--r--   0 hagenjt1   (501) staff       (20)     3676 2022-11-02 13:18:29.000000 exitstatus-2.3.0/exitstatus.egg-info/PKG-INFO
--rw-r--r--   0 hagenjt1   (501) staff       (20)      270 2022-11-02 13:18:29.000000 exitstatus-2.3.0/exitstatus.egg-info/SOURCES.txt
--rw-r--r--   0 hagenjt1   (501) staff       (20)        1 2022-11-02 13:18:29.000000 exitstatus-2.3.0/exitstatus.egg-info/dependency_links.txt
--rw-r--r--   0 hagenjt1   (501) staff       (20)        1 2022-11-02 12:40:37.000000 exitstatus-2.3.0/exitstatus.egg-info/not-zip-safe
--rw-r--r--   0 hagenjt1   (501) staff       (20)       11 2022-11-02 13:18:29.000000 exitstatus-2.3.0/exitstatus.egg-info/top_level.txt
--rw-r--r--   0 hagenjt1   (501) staff       (20)      458 2022-11-02 13:12:19.000000 exitstatus-2.3.0/pyproject.toml
--rw-r--r--   0 hagenjt1   (501) staff       (20)       38 2022-11-02 13:18:29.579526 exitstatus-2.3.0/setup.cfg
--rw-r--r--   0 hagenjt1   (501) staff       (20)     1100 2022-11-02 13:12:48.000000 exitstatus-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 18:56:47.491527 exitstatus-2.4.0/
+-rw-rw-rw-   0        0        0     1078 2023-04-30 18:53:02.000000 exitstatus-2.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       70 2023-04-30 18:45:30.000000 exitstatus-2.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3941 2023-04-30 18:56:47.491527 exitstatus-2.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3103 2023-04-30 18:55:17.000000 exitstatus-2.4.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-30 18:56:47.484528 exitstatus-2.4.0/exitstatus/
+-rw-rw-rw-   0        0        0      365 2023-04-30 18:45:30.000000 exitstatus-2.4.0/exitstatus/__init__.py
+-rw-rw-rw-   0        0        0       95 2023-04-30 18:45:30.000000 exitstatus-2.4.0/exitstatus/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-30 18:56:47.489528 exitstatus-2.4.0/exitstatus.egg-info/
+-rw-rw-rw-   0        0        0     3941 2023-04-30 18:56:47.000000 exitstatus-2.4.0/exitstatus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-04-30 18:56:47.000000 exitstatus-2.4.0/exitstatus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 18:56:47.000000 exitstatus-2.4.0/exitstatus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-30 18:56:47.000000 exitstatus-2.4.0/exitstatus.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-04-30 18:56:47.000000 exitstatus-2.4.0/exitstatus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      486 2023-04-30 18:53:02.000000 exitstatus-2.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 18:56:47.491527 exitstatus-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1185 2023-04-30 18:55:17.000000 exitstatus-2.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 18:56:47.490527 exitstatus-2.4.0/tests/
+-rw-rw-rw-   0        0        0      641 2023-04-30 18:45:30.000000 exitstatus-2.4.0/tests/test_exitstatus.py
```

### Comparing `exitstatus-2.3.0/LICENSE.txt` & `exitstatus-2.4.0/LICENSE.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2019-2022 John Hagen
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to
-deal in the Software without restriction, including without limitation the
-rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
-sell copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
-IN THE SOFTWARE.
+Copyright (c) 2019-2023 John Hagen
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to
+deal in the Software without restriction, including without limitation the
+rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
+sell copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
+IN THE SOFTWARE.
```

### Comparing `exitstatus-2.3.0/PKG-INFO` & `exitstatus-2.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,138 +1,144 @@
-Metadata-Version: 2.1
-Name: exitstatus
-Version: 2.3.0
-Summary: POSIX exit status codes
-Home-page: https://github.com/johnthagen/exitstatus
-Author: John Hagen
-Author-email: johnthagen@gmail.com
-License: MIT
-Keywords: exit status POSIX
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Typing :: Typed
-Requires-Python: >=3.8
-License-File: LICENSE.txt
-
-``exitstatus`` - POSIX exit status definitions
-==============================================
-
-.. image:: https://github.com/johnthagen/exitstatus/workflows/python/badge.svg
-    :target: https://github.com/johnthagen/exitstatus/actions
-
-.. image:: https://codeclimate.com/github/johnthagen/exitstatus/badges/gpa.svg
-   :target: https://codeclimate.com/github/johnthagen/exitstatus/
-
-.. image:: https://codeclimate.com/github/johnthagen/exitstatus/badges/issue_count.svg
-   :target: https://codeclimate.com/github/johnthagen/exitstatus/
-
-.. image:: https://codecov.io/github/johnthagen/exitstatus/coverage.svg
-    :target: https://codecov.io/github/johnthagen/exitstatus/
-
-.. image:: https://img.shields.io/pypi/v/exitstatus.svg
-    :target: https://pypi.python.org/pypi/exitstatus/
-
-.. image:: https://img.shields.io/pypi/status/exitstatus.svg
-    :target: https://pypi.python.org/pypi/exitstatus/
-
-.. image:: https://img.shields.io/pypi/pyversions/exitstatus.svg
-    :target: https://pypi.python.org/pypi/exitstatus/
-
-``exitstatus`` provides expressive, portable definitions for the
-`standard POSIX exit codes <https://www.gnu.org/software/libc/manual/html_node/Exit-Status.html>`__.
-While Python does provide some Unix-specific exit status codes in the
-`os module <https://docs.python.org/3/library/os.html#os._exit>`__, they are not portable to
-all platforms and are missing the generic failure case.
-
-
-Installation
-------------
-
-You can install, upgrade, and uninstall ``exitstatus`` with these commands:
-
-.. code:: shell-session
-
-    $ pip install exitstatus
-    $ pip install --upgrade exitstatus
-    $ pip uninstall exitstatus
-
-Usage
------
-
-Exit status codes are defined in a simple to use
-`IntEnum <https://docs.python.org/3/library/enum.html#enum.IntEnum>`__.
-
-.. code:: python
-
-    import sys
-    from exitstatus import ExitStatus
-
-    sys.exit(ExitStatus.success)
-
-Releases
---------
-
-2.3.0 2022-11-02
-^^^^^^^^^^^^^^^^
-
-- Add ``py.typed`` file to package to support Mypy type checking.
-- Refactor the project into an installable package rather than an installable module.
-- Drop support for Python 3.7
-
-2.2.0 2021-11-06
-^^^^^^^^^^^^^^^^
-
-- Support Python 3.10 and drop 3.6.
-
-2.1.0 2020-12-27
-^^^^^^^^^^^^^^^^
-
-- Drop Python 3.5 and support Python 3.9.
-- Switch to GitHub Actions for CI.
-
-2.0.1 2020-04-26
-^^^^^^^^^^^^^^^^
-
-- Update LICENSE file.
-
-2.0.0 2020-03-29
-^^^^^^^^^^^^^^^^
-
-- Drop Python 2.7 support.
-
-1.4.1 2020-03-29
-^^^^^^^^^^^^^^^^
-
-- Add ``python_requires`` field to ``setup.py``.
-
-1.4.0 2019-12-14
-^^^^^^^^^^^^^^^^
-
-- Drop Python 3.4 and support Python 3.8.
-- Include license file.
-
-1.3.0 - 2018-07-09
-^^^^^^^^^^^^^^^^^^
-
-Drop Python 3.3 and support Python 3.7.
-
-1.2.0 - 2016-12-31
-^^^^^^^^^^^^^^^^^^
-
-Support Python 3.6.
-
-1.1.0 - 2016-10-11
-^^^^^^^^^^^^^^^^^^
-
-Add docstrings and simplify checking for ``enum34`` dependency need.
-
-1.0.0 - 2016-06-10
-^^^^^^^^^^^^^^^^^^
-
-Initial release.
+Metadata-Version: 2.1
+Name: exitstatus
+Version: 2.4.0
+Summary: POSIX exit status codes
+Home-page: https://github.com/johnthagen/exitstatus
+Author: John Hagen
+Author-email: johnthagen@gmail.com
+License: MIT
+Keywords: exit status POSIX
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+License-File: LICENSE.txt
+
+``exitstatus`` - POSIX exit status definitions
+==============================================
+
+.. image:: https://github.com/johnthagen/exitstatus/workflows/python/badge.svg
+    :target: https://github.com/johnthagen/exitstatus/actions
+
+.. image:: https://codeclimate.com/github/johnthagen/exitstatus/badges/gpa.svg
+   :target: https://codeclimate.com/github/johnthagen/exitstatus/
+
+.. image:: https://codeclimate.com/github/johnthagen/exitstatus/badges/issue_count.svg
+   :target: https://codeclimate.com/github/johnthagen/exitstatus/
+
+.. image:: https://codecov.io/github/johnthagen/exitstatus/coverage.svg
+    :target: https://codecov.io/github/johnthagen/exitstatus/
+
+.. image:: https://img.shields.io/pypi/v/exitstatus.svg
+    :target: https://pypi.python.org/pypi/exitstatus/
+
+.. image:: https://img.shields.io/pypi/status/exitstatus.svg
+    :target: https://pypi.python.org/pypi/exitstatus/
+
+.. image:: https://img.shields.io/pypi/pyversions/exitstatus.svg
+    :target: https://pypi.python.org/pypi/exitstatus/
+
+``exitstatus`` provides expressive, portable definitions for the
+`standard POSIX exit codes <https://www.gnu.org/software/libc/manual/html_node/Exit-Status.html>`__.
+While Python does provide some Unix-specific exit status codes in the
+`os module <https://docs.python.org/3/library/os.html#os._exit>`__, they are not portable to
+all platforms and are missing the generic failure case.
+
+
+Installation
+------------
+
+You can install, upgrade, and uninstall ``exitstatus`` with these commands:
+
+.. code:: shell-session
+
+    $ pip install exitstatus
+    $ pip install --upgrade exitstatus
+    $ pip uninstall exitstatus
+
+Usage
+-----
+
+Exit status codes are defined in a simple to use
+`IntEnum <https://docs.python.org/3/library/enum.html#enum.IntEnum>`__.
+
+.. code:: python
+
+    import sys
+    from exitstatus import ExitStatus
+
+    sys.exit(ExitStatus.success)
+
+Releases
+--------
+
+2.4.0 (2023-04-30)
+^^^^^^^^^^^^^^^^^^
+
+- Add support for Python 3.11
+
+2.3.0 2022-11-02
+^^^^^^^^^^^^^^^^
+
+- Add ``py.typed`` file to package to support Mypy type checking.
+- Refactor the project into an installable package rather than an installable module.
+- Drop support for Python 3.7
+
+2.2.0 2021-11-06
+^^^^^^^^^^^^^^^^
+
+- Support Python 3.10 and drop 3.6.
+
+2.1.0 2020-12-27
+^^^^^^^^^^^^^^^^
+
+- Drop Python 3.5 and support Python 3.9.
+- Switch to GitHub Actions for CI.
+
+2.0.1 2020-04-26
+^^^^^^^^^^^^^^^^
+
+- Update LICENSE file.
+
+2.0.0 2020-03-29
+^^^^^^^^^^^^^^^^
+
+- Drop Python 2.7 support.
+
+1.4.1 2020-03-29
+^^^^^^^^^^^^^^^^
+
+- Add ``python_requires`` field to ``setup.py``.
+
+1.4.0 2019-12-14
+^^^^^^^^^^^^^^^^
+
+- Drop Python 3.4 and support Python 3.8.
+- Include license file.
+
+1.3.0 - 2018-07-09
+^^^^^^^^^^^^^^^^^^
+
+Drop Python 3.3 and support Python 3.7.
+
+1.2.0 - 2016-12-31
+^^^^^^^^^^^^^^^^^^
+
+Support Python 3.6.
+
+1.1.0 - 2016-10-11
+^^^^^^^^^^^^^^^^^^
+
+Add docstrings and simplify checking for ``enum34`` dependency need.
+
+1.0.0 - 2016-06-10
+^^^^^^^^^^^^^^^^^^
+
+Initial release.
```

### Comparing `exitstatus-2.3.0/README.rst` & `exitstatus-2.4.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,182 +1,194 @@
 00000000: 6060 6578 6974 7374 6174 7573 6060 202d  ``exitstatus`` -
 00000010: 2050 4f53 4958 2065 7869 7420 7374 6174   POSIX exit stat
-00000020: 7573 2064 6566 696e 6974 696f 6e73 0a3d  us definitions.=
+00000020: 7573 2064 6566 696e 6974 696f 6e73 0d0a  us definitions..
 00000030: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000040: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000050: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a2e  =============...
-00000060: 2e20 696d 6167 653a 3a20 6874 7470 733a  . image:: https:
-00000070: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6f68  //github.com/joh
-00000080: 6e74 6861 6765 6e2f 6578 6974 7374 6174  nthagen/exitstat
-00000090: 7573 2f77 6f72 6b66 6c6f 7773 2f70 7974  us/workflows/pyt
-000000a0: 686f 6e2f 6261 6467 652e 7376 670a 2020  hon/badge.svg.  
-000000b0: 2020 3a74 6172 6765 743a 2068 7474 7073    :target: https
-000000c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a6f  ://github.com/jo
-000000d0: 686e 7468 6167 656e 2f65 7869 7473 7461  hnthagen/exitsta
-000000e0: 7475 732f 6163 7469 6f6e 730a 0a2e 2e20  tus/actions.... 
-000000f0: 696d 6167 653a 3a20 6874 7470 733a 2f2f  image:: https://
-00000100: 636f 6465 636c 696d 6174 652e 636f 6d2f  codeclimate.com/
-00000110: 6769 7468 7562 2f6a 6f68 6e74 6861 6765  github/johnthage
-00000120: 6e2f 6578 6974 7374 6174 7573 2f62 6164  n/exitstatus/bad
-00000130: 6765 732f 6770 612e 7376 670a 2020 203a  ges/gpa.svg.   :
-00000140: 7461 7267 6574 3a20 6874 7470 733a 2f2f  target: https://
-00000150: 636f 6465 636c 696d 6174 652e 636f 6d2f  codeclimate.com/
-00000160: 6769 7468 7562 2f6a 6f68 6e74 6861 6765  github/johnthage
-00000170: 6e2f 6578 6974 7374 6174 7573 2f0a 0a2e  n/exitstatus/...
-00000180: 2e20 696d 6167 653a 3a20 6874 7470 733a  . image:: https:
-00000190: 2f2f 636f 6465 636c 696d 6174 652e 636f  //codeclimate.co
-000001a0: 6d2f 6769 7468 7562 2f6a 6f68 6e74 6861  m/github/johntha
-000001b0: 6765 6e2f 6578 6974 7374 6174 7573 2f62  gen/exitstatus/b
-000001c0: 6164 6765 732f 6973 7375 655f 636f 756e  adges/issue_coun
-000001d0: 742e 7376 670a 2020 203a 7461 7267 6574  t.svg.   :target
-000001e0: 3a20 6874 7470 733a 2f2f 636f 6465 636c  : https://codecl
-000001f0: 696d 6174 652e 636f 6d2f 6769 7468 7562  imate.com/github
-00000200: 2f6a 6f68 6e74 6861 6765 6e2f 6578 6974  /johnthagen/exit
-00000210: 7374 6174 7573 2f0a 0a2e 2e20 696d 6167  status/.... imag
-00000220: 653a 3a20 6874 7470 733a 2f2f 636f 6465  e:: https://code
-00000230: 636f 762e 696f 2f67 6974 6875 622f 6a6f  cov.io/github/jo
-00000240: 686e 7468 6167 656e 2f65 7869 7473 7461  hnthagen/exitsta
-00000250: 7475 732f 636f 7665 7261 6765 2e73 7667  tus/coverage.svg
-00000260: 0a20 2020 203a 7461 7267 6574 3a20 6874  .    :target: ht
-00000270: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
-00000280: 2f67 6974 6875 622f 6a6f 686e 7468 6167  /github/johnthag
-00000290: 656e 2f65 7869 7473 7461 7475 732f 0a0a  en/exitstatus/..
-000002a0: 2e2e 2069 6d61 6765 3a3a 2068 7474 7073  .. image:: https
-000002b0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-000002c0: 6f2f 7079 7069 2f76 2f65 7869 7473 7461  o/pypi/v/exitsta
-000002d0: 7475 732e 7376 670a 2020 2020 3a74 6172  tus.svg.    :tar
-000002e0: 6765 743a 2068 7474 7073 3a2f 2f70 7970  get: https://pyp
-000002f0: 692e 7079 7468 6f6e 2e6f 7267 2f70 7970  i.python.org/pyp
-00000300: 692f 6578 6974 7374 6174 7573 2f0a 0a2e  i/exitstatus/...
-00000310: 2e20 696d 6167 653a 3a20 6874 7470 733a  . image:: https:
-00000320: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000330: 2f70 7970 692f 7374 6174 7573 2f65 7869  /pypi/status/exi
-00000340: 7473 7461 7475 732e 7376 670a 2020 2020  tstatus.svg.    
-00000350: 3a74 6172 6765 743a 2068 7474 7073 3a2f  :target: https:/
-00000360: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
-00000370: 2f70 7970 692f 6578 6974 7374 6174 7573  /pypi/exitstatus
-00000380: 2f0a 0a2e 2e20 696d 6167 653a 3a20 6874  /.... image:: ht
-00000390: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-000003a0: 732e 696f 2f70 7970 692f 7079 7665 7273  s.io/pypi/pyvers
-000003b0: 696f 6e73 2f65 7869 7473 7461 7475 732e  ions/exitstatus.
-000003c0: 7376 670a 2020 2020 3a74 6172 6765 743a  svg.    :target:
-000003d0: 2068 7474 7073 3a2f 2f70 7970 692e 7079   https://pypi.py
-000003e0: 7468 6f6e 2e6f 7267 2f70 7970 692f 6578  thon.org/pypi/ex
-000003f0: 6974 7374 6174 7573 2f0a 0a60 6065 7869  itstatus/..``exi
-00000400: 7473 7461 7475 7360 6020 7072 6f76 6964  tstatus`` provid
-00000410: 6573 2065 7870 7265 7373 6976 652c 2070  es expressive, p
-00000420: 6f72 7461 626c 6520 6465 6669 6e69 7469  ortable definiti
-00000430: 6f6e 7320 666f 7220 7468 650a 6073 7461  ons for the.`sta
-00000440: 6e64 6172 6420 504f 5349 5820 6578 6974  ndard POSIX exit
-00000450: 2063 6f64 6573 203c 6874 7470 733a 2f2f   codes <https://
-00000460: 7777 772e 676e 752e 6f72 672f 736f 6674  www.gnu.org/soft
-00000470: 7761 7265 2f6c 6962 632f 6d61 6e75 616c  ware/libc/manual
-00000480: 2f68 746d 6c5f 6e6f 6465 2f45 7869 742d  /html_node/Exit-
-00000490: 5374 6174 7573 2e68 746d 6c3e 605f 5f2e  Status.html>`__.
-000004a0: 0a57 6869 6c65 2050 7974 686f 6e20 646f  .While Python do
-000004b0: 6573 2070 726f 7669 6465 2073 6f6d 6520  es provide some 
-000004c0: 556e 6978 2d73 7065 6369 6669 6320 6578  Unix-specific ex
-000004d0: 6974 2073 7461 7475 7320 636f 6465 7320  it status codes 
-000004e0: 696e 2074 6865 0a60 6f73 206d 6f64 756c  in the.`os modul
-000004f0: 6520 3c68 7474 7073 3a2f 2f64 6f63 732e  e <https://docs.
-00000500: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
-00000510: 7261 7279 2f6f 732e 6874 6d6c 236f 732e  rary/os.html#os.
-00000520: 5f65 7869 743e 605f 5f2c 2074 6865 7920  _exit>`__, they 
-00000530: 6172 6520 6e6f 7420 706f 7274 6162 6c65  are not portable
-00000540: 2074 6f0a 616c 6c20 706c 6174 666f 726d   to.all platform
-00000550: 7320 616e 6420 6172 6520 6d69 7373 696e  s and are missin
-00000560: 6720 7468 6520 6765 6e65 7269 6320 6661  g the generic fa
-00000570: 696c 7572 6520 6361 7365 2e0a 0a0a 496e  ilure case....In
-00000580: 7374 616c 6c61 7469 6f6e 0a2d 2d2d 2d2d  stallation.-----
-00000590: 2d2d 2d2d 2d2d 2d0a 0a59 6f75 2063 616e  -------..You can
-000005a0: 2069 6e73 7461 6c6c 2c20 7570 6772 6164   install, upgrad
-000005b0: 652c 2061 6e64 2075 6e69 6e73 7461 6c6c  e, and uninstall
-000005c0: 2060 6065 7869 7473 7461 7475 7360 6020   ``exitstatus`` 
-000005d0: 7769 7468 2074 6865 7365 2063 6f6d 6d61  with these comma
-000005e0: 6e64 733a 0a0a 2e2e 2063 6f64 653a 3a20  nds:.... code:: 
-000005f0: 7368 656c 6c2d 7365 7373 696f 6e0a 0a20  shell-session.. 
-00000600: 2020 2024 2070 6970 2069 6e73 7461 6c6c     $ pip install
-00000610: 2065 7869 7473 7461 7475 730a 2020 2020   exitstatus.    
-00000620: 2420 7069 7020 696e 7374 616c 6c20 2d2d  $ pip install --
-00000630: 7570 6772 6164 6520 6578 6974 7374 6174  upgrade exitstat
-00000640: 7573 0a20 2020 2024 2070 6970 2075 6e69  us.    $ pip uni
-00000650: 6e73 7461 6c6c 2065 7869 7473 7461 7475  nstall exitstatu
-00000660: 730a 0a55 7361 6765 0a2d 2d2d 2d2d 0a0a  s..Usage.-----..
-00000670: 4578 6974 2073 7461 7475 7320 636f 6465  Exit status code
-00000680: 7320 6172 6520 6465 6669 6e65 6420 696e  s are defined in
-00000690: 2061 2073 696d 706c 6520 746f 2075 7365   a simple to use
-000006a0: 0a60 496e 7445 6e75 6d20 3c68 7474 7073  .`IntEnum <https
-000006b0: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
-000006c0: 7267 2f33 2f6c 6962 7261 7279 2f65 6e75  rg/3/library/enu
-000006d0: 6d2e 6874 6d6c 2365 6e75 6d2e 496e 7445  m.html#enum.IntE
-000006e0: 6e75 6d3e 605f 5f2e 0a0a 2e2e 2063 6f64  num>`__..... cod
-000006f0: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
-00000700: 696d 706f 7274 2073 7973 0a20 2020 2066  import sys.    f
-00000710: 726f 6d20 6578 6974 7374 6174 7573 2069  rom exitstatus i
-00000720: 6d70 6f72 7420 4578 6974 5374 6174 7573  mport ExitStatus
-00000730: 0a0a 2020 2020 7379 732e 6578 6974 2845  ..    sys.exit(E
-00000740: 7869 7453 7461 7475 732e 7375 6363 6573  xitStatus.succes
-00000750: 7329 0a0a 5265 6c65 6173 6573 0a2d 2d2d  s)..Releases.---
-00000760: 2d2d 2d2d 2d0a 0a32 2e33 2e30 2032 3032  -----..2.3.0 202
-00000770: 322d 3131 2d30 320a 5e5e 5e5e 5e5e 5e5e  2-11-02.^^^^^^^^
-00000780: 5e5e 5e5e 5e5e 5e5e 0a0a 2d20 4164 6420  ^^^^^^^^..- Add 
-00000790: 6060 7079 2e74 7970 6564 6060 2066 696c  ``py.typed`` fil
-000007a0: 6520 746f 2070 6163 6b61 6765 2074 6f20  e to package to 
-000007b0: 7375 7070 6f72 7420 4d79 7079 2074 7970  support Mypy typ
-000007c0: 6520 6368 6563 6b69 6e67 2e0a 2d20 5265  e checking..- Re
-000007d0: 6661 6374 6f72 2074 6865 2070 726f 6a65  factor the proje
-000007e0: 6374 2069 6e74 6f20 616e 2069 6e73 7461  ct into an insta
-000007f0: 6c6c 6162 6c65 2070 6163 6b61 6765 2072  llable package r
-00000800: 6174 6865 7220 7468 616e 2061 6e20 696e  ather than an in
-00000810: 7374 616c 6c61 626c 6520 6d6f 6475 6c65  stallable module
-00000820: 2e0a 2d20 4472 6f70 2073 7570 706f 7274  ..- Drop support
-00000830: 2066 6f72 2050 7974 686f 6e20 332e 370a   for Python 3.7.
-00000840: 0a32 2e32 2e30 2032 3032 312d 3131 2d30  .2.2.0 2021-11-0
-00000850: 360a 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  6.^^^^^^^^^^^^^^
-00000860: 5e5e 0a0a 2d20 5375 7070 6f72 7420 5079  ^^..- Support Py
-00000870: 7468 6f6e 2033 2e31 3020 616e 6420 6472  thon 3.10 and dr
-00000880: 6f70 2033 2e36 2e0a 0a32 2e31 2e30 2032  op 3.6...2.1.0 2
-00000890: 3032 302d 3132 2d32 370a 5e5e 5e5e 5e5e  020-12-27.^^^^^^
-000008a0: 5e5e 5e5e 5e5e 5e5e 5e5e 0a0a 2d20 4472  ^^^^^^^^^^..- Dr
-000008b0: 6f70 2050 7974 686f 6e20 332e 3520 616e  op Python 3.5 an
-000008c0: 6420 7375 7070 6f72 7420 5079 7468 6f6e  d support Python
-000008d0: 2033 2e39 2e0a 2d20 5377 6974 6368 2074   3.9..- Switch t
-000008e0: 6f20 4769 7448 7562 2041 6374 696f 6e73  o GitHub Actions
-000008f0: 2066 6f72 2043 492e 0a0a 322e 302e 3120   for CI...2.0.1 
-00000900: 3230 3230 2d30 342d 3236 0a5e 5e5e 5e5e  2020-04-26.^^^^^
-00000910: 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a 0a2d 2055  ^^^^^^^^^^^..- U
-00000920: 7064 6174 6520 4c49 4345 4e53 4520 6669  pdate LICENSE fi
-00000930: 6c65 2e0a 0a32 2e30 2e30 2032 3032 302d  le...2.0.0 2020-
-00000940: 3033 2d32 390a 5e5e 5e5e 5e5e 5e5e 5e5e  03-29.^^^^^^^^^^
-00000950: 5e5e 5e5e 5e5e 0a0a 2d20 4472 6f70 2050  ^^^^^^..- Drop P
-00000960: 7974 686f 6e20 322e 3720 7375 7070 6f72  ython 2.7 suppor
-00000970: 742e 0a0a 312e 342e 3120 3230 3230 2d30  t...1.4.1 2020-0
-00000980: 332d 3239 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e  3-29.^^^^^^^^^^^
-00000990: 5e5e 5e5e 5e0a 0a2d 2041 6464 2060 6070  ^^^^^..- Add ``p
-000009a0: 7974 686f 6e5f 7265 7175 6972 6573 6060  ython_requires``
-000009b0: 2066 6965 6c64 2074 6f20 6060 7365 7475   field to ``setu
-000009c0: 702e 7079 6060 2e0a 0a31 2e34 2e30 2032  p.py``...1.4.0 2
-000009d0: 3031 392d 3132 2d31 340a 5e5e 5e5e 5e5e  019-12-14.^^^^^^
-000009e0: 5e5e 5e5e 5e5e 5e5e 5e5e 0a0a 2d20 4472  ^^^^^^^^^^..- Dr
-000009f0: 6f70 2050 7974 686f 6e20 332e 3420 616e  op Python 3.4 an
-00000a00: 6420 7375 7070 6f72 7420 5079 7468 6f6e  d support Python
-00000a10: 2033 2e38 2e0a 2d20 496e 636c 7564 6520   3.8..- Include 
-00000a20: 6c69 6365 6e73 6520 6669 6c65 2e0a 0a31  license file...1
-00000a30: 2e33 2e30 202d 2032 3031 382d 3037 2d30  .3.0 - 2018-07-0
-00000a40: 390a 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  9.^^^^^^^^^^^^^^
-00000a50: 5e5e 5e5e 0a0a 4472 6f70 2050 7974 686f  ^^^^..Drop Pytho
-00000a60: 6e20 332e 3320 616e 6420 7375 7070 6f72  n 3.3 and suppor
-00000a70: 7420 5079 7468 6f6e 2033 2e37 2e0a 0a31  t Python 3.7...1
-00000a80: 2e32 2e30 202d 2032 3031 362d 3132 2d33  .2.0 - 2016-12-3
-00000a90: 310a 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  1.^^^^^^^^^^^^^^
-00000aa0: 5e5e 5e5e 0a0a 5375 7070 6f72 7420 5079  ^^^^..Support Py
-00000ab0: 7468 6f6e 2033 2e36 2e0a 0a31 2e31 2e30  thon 3.6...1.1.0
-00000ac0: 202d 2032 3031 362d 3130 2d31 310a 5e5e   - 2016-10-11.^^
-00000ad0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
-00000ae0: 0a0a 4164 6420 646f 6373 7472 696e 6773  ..Add docstrings
-00000af0: 2061 6e64 2073 696d 706c 6966 7920 6368   and simplify ch
-00000b00: 6563 6b69 6e67 2066 6f72 2060 6065 6e75  ecking for ``enu
-00000b10: 6d33 3460 6020 6465 7065 6e64 656e 6379  m34`` dependency
-00000b20: 206e 6565 642e 0a0a 312e 302e 3020 2d20   need...1.0.0 - 
-00000b30: 3230 3136 2d30 362d 3130 0a5e 5e5e 5e5e  2016-06-10.^^^^^
-00000b40: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a 0a49  ^^^^^^^^^^^^^..I
-00000b50: 6e69 7469 616c 2072 656c 6561 7365 2e0a  nitial release..
+00000050: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a  ==============..
+00000060: 0d0a 2e2e 2069 6d61 6765 3a3a 2068 7474  .... image:: htt
+00000070: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000080: 6a6f 686e 7468 6167 656e 2f65 7869 7473  johnthagen/exits
+00000090: 7461 7475 732f 776f 726b 666c 6f77 732f  tatus/workflows/
+000000a0: 7079 7468 6f6e 2f62 6164 6765 2e73 7667  python/badge.svg
+000000b0: 0d0a 2020 2020 3a74 6172 6765 743a 2068  ..    :target: h
+000000c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000000d0: 6d2f 6a6f 686e 7468 6167 656e 2f65 7869  m/johnthagen/exi
+000000e0: 7473 7461 7475 732f 6163 7469 6f6e 730d  tstatus/actions.
+000000f0: 0a0d 0a2e 2e20 696d 6167 653a 3a20 6874  ..... image:: ht
+00000100: 7470 733a 2f2f 636f 6465 636c 696d 6174  tps://codeclimat
+00000110: 652e 636f 6d2f 6769 7468 7562 2f6a 6f68  e.com/github/joh
+00000120: 6e74 6861 6765 6e2f 6578 6974 7374 6174  nthagen/exitstat
+00000130: 7573 2f62 6164 6765 732f 6770 612e 7376  us/badges/gpa.sv
+00000140: 670d 0a20 2020 3a74 6172 6765 743a 2068  g..   :target: h
+00000150: 7474 7073 3a2f 2f63 6f64 6563 6c69 6d61  ttps://codeclima
+00000160: 7465 2e63 6f6d 2f67 6974 6875 622f 6a6f  te.com/github/jo
+00000170: 686e 7468 6167 656e 2f65 7869 7473 7461  hnthagen/exitsta
+00000180: 7475 732f 0d0a 0d0a 2e2e 2069 6d61 6765  tus/...... image
+00000190: 3a3a 2068 7474 7073 3a2f 2f63 6f64 6563  :: https://codec
+000001a0: 6c69 6d61 7465 2e63 6f6d 2f67 6974 6875  limate.com/githu
+000001b0: 622f 6a6f 686e 7468 6167 656e 2f65 7869  b/johnthagen/exi
+000001c0: 7473 7461 7475 732f 6261 6467 6573 2f69  tstatus/badges/i
+000001d0: 7373 7565 5f63 6f75 6e74 2e73 7667 0d0a  ssue_count.svg..
+000001e0: 2020 203a 7461 7267 6574 3a20 6874 7470     :target: http
+000001f0: 733a 2f2f 636f 6465 636c 696d 6174 652e  s://codeclimate.
+00000200: 636f 6d2f 6769 7468 7562 2f6a 6f68 6e74  com/github/johnt
+00000210: 6861 6765 6e2f 6578 6974 7374 6174 7573  hagen/exitstatus
+00000220: 2f0d 0a0d 0a2e 2e20 696d 6167 653a 3a20  /...... image:: 
+00000230: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
+00000240: 696f 2f67 6974 6875 622f 6a6f 686e 7468  io/github/johnth
+00000250: 6167 656e 2f65 7869 7473 7461 7475 732f  agen/exitstatus/
+00000260: 636f 7665 7261 6765 2e73 7667 0d0a 2020  coverage.svg..  
+00000270: 2020 3a74 6172 6765 743a 2068 7474 7073    :target: https
+00000280: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6769  ://codecov.io/gi
+00000290: 7468 7562 2f6a 6f68 6e74 6861 6765 6e2f  thub/johnthagen/
+000002a0: 6578 6974 7374 6174 7573 2f0d 0a0d 0a2e  exitstatus/.....
+000002b0: 2e20 696d 6167 653a 3a20 6874 7470 733a  . image:: https:
+000002c0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000002d0: 2f70 7970 692f 762f 6578 6974 7374 6174  /pypi/v/exitstat
+000002e0: 7573 2e73 7667 0d0a 2020 2020 3a74 6172  us.svg..    :tar
+000002f0: 6765 743a 2068 7474 7073 3a2f 2f70 7970  get: https://pyp
+00000300: 692e 7079 7468 6f6e 2e6f 7267 2f70 7970  i.python.org/pyp
+00000310: 692f 6578 6974 7374 6174 7573 2f0d 0a0d  i/exitstatus/...
+00000320: 0a2e 2e20 696d 6167 653a 3a20 6874 7470  ... image:: http
+00000330: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000340: 696f 2f70 7970 692f 7374 6174 7573 2f65  io/pypi/status/e
+00000350: 7869 7473 7461 7475 732e 7376 670d 0a20  xitstatus.svg.. 
+00000360: 2020 203a 7461 7267 6574 3a20 6874 7470     :target: http
+00000370: 733a 2f2f 7079 7069 2e70 7974 686f 6e2e  s://pypi.python.
+00000380: 6f72 672f 7079 7069 2f65 7869 7473 7461  org/pypi/exitsta
+00000390: 7475 732f 0d0a 0d0a 2e2e 2069 6d61 6765  tus/...... image
+000003a0: 3a3a 2068 7474 7073 3a2f 2f69 6d67 2e73  :: https://img.s
+000003b0: 6869 656c 6473 2e69 6f2f 7079 7069 2f70  hields.io/pypi/p
+000003c0: 7976 6572 7369 6f6e 732f 6578 6974 7374  yversions/exitst
+000003d0: 6174 7573 2e73 7667 0d0a 2020 2020 3a74  atus.svg..    :t
+000003e0: 6172 6765 743a 2068 7474 7073 3a2f 2f70  arget: https://p
+000003f0: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
+00000400: 7970 692f 6578 6974 7374 6174 7573 2f0d  ypi/exitstatus/.
+00000410: 0a0d 0a60 6065 7869 7473 7461 7475 7360  ...``exitstatus`
+00000420: 6020 7072 6f76 6964 6573 2065 7870 7265  ` provides expre
+00000430: 7373 6976 652c 2070 6f72 7461 626c 6520  ssive, portable 
+00000440: 6465 6669 6e69 7469 6f6e 7320 666f 7220  definitions for 
+00000450: 7468 650d 0a60 7374 616e 6461 7264 2050  the..`standard P
+00000460: 4f53 4958 2065 7869 7420 636f 6465 7320  OSIX exit codes 
+00000470: 3c68 7474 7073 3a2f 2f77 7777 2e67 6e75  <https://www.gnu
+00000480: 2e6f 7267 2f73 6f66 7477 6172 652f 6c69  .org/software/li
+00000490: 6263 2f6d 616e 7561 6c2f 6874 6d6c 5f6e  bc/manual/html_n
+000004a0: 6f64 652f 4578 6974 2d53 7461 7475 732e  ode/Exit-Status.
+000004b0: 6874 6d6c 3e60 5f5f 2e0d 0a57 6869 6c65  html>`__...While
+000004c0: 2050 7974 686f 6e20 646f 6573 2070 726f   Python does pro
+000004d0: 7669 6465 2073 6f6d 6520 556e 6978 2d73  vide some Unix-s
+000004e0: 7065 6369 6669 6320 6578 6974 2073 7461  pecific exit sta
+000004f0: 7475 7320 636f 6465 7320 696e 2074 6865  tus codes in the
+00000500: 0d0a 606f 7320 6d6f 6475 6c65 203c 6874  ..`os module <ht
+00000510: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
+00000520: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
+00000530: 6f73 2e68 746d 6c23 6f73 2e5f 6578 6974  os.html#os._exit
+00000540: 3e60 5f5f 2c20 7468 6579 2061 7265 206e  >`__, they are n
+00000550: 6f74 2070 6f72 7461 626c 6520 746f 0d0a  ot portable to..
+00000560: 616c 6c20 706c 6174 666f 726d 7320 616e  all platforms an
+00000570: 6420 6172 6520 6d69 7373 696e 6720 7468  d are missing th
+00000580: 6520 6765 6e65 7269 6320 6661 696c 7572  e generic failur
+00000590: 6520 6361 7365 2e0d 0a0d 0a0d 0a49 6e73  e case.......Ins
+000005a0: 7461 6c6c 6174 696f 6e0d 0a2d 2d2d 2d2d  tallation..-----
+000005b0: 2d2d 2d2d 2d2d 2d0d 0a0d 0a59 6f75 2063  -------....You c
+000005c0: 616e 2069 6e73 7461 6c6c 2c20 7570 6772  an install, upgr
+000005d0: 6164 652c 2061 6e64 2075 6e69 6e73 7461  ade, and uninsta
+000005e0: 6c6c 2060 6065 7869 7473 7461 7475 7360  ll ``exitstatus`
+000005f0: 6020 7769 7468 2074 6865 7365 2063 6f6d  ` with these com
+00000600: 6d61 6e64 733a 0d0a 0d0a 2e2e 2063 6f64  mands:...... cod
+00000610: 653a 3a20 7368 656c 6c2d 7365 7373 696f  e:: shell-sessio
+00000620: 6e0d 0a0d 0a20 2020 2024 2070 6970 2069  n....    $ pip i
+00000630: 6e73 7461 6c6c 2065 7869 7473 7461 7475  nstall exitstatu
+00000640: 730d 0a20 2020 2024 2070 6970 2069 6e73  s..    $ pip ins
+00000650: 7461 6c6c 202d 2d75 7067 7261 6465 2065  tall --upgrade e
+00000660: 7869 7473 7461 7475 730d 0a20 2020 2024  xitstatus..    $
+00000670: 2070 6970 2075 6e69 6e73 7461 6c6c 2065   pip uninstall e
+00000680: 7869 7473 7461 7475 730d 0a0d 0a55 7361  xitstatus....Usa
+00000690: 6765 0d0a 2d2d 2d2d 2d0d 0a0d 0a45 7869  ge..-----....Exi
+000006a0: 7420 7374 6174 7573 2063 6f64 6573 2061  t status codes a
+000006b0: 7265 2064 6566 696e 6564 2069 6e20 6120  re defined in a 
+000006c0: 7369 6d70 6c65 2074 6f20 7573 650d 0a60  simple to use..`
+000006d0: 496e 7445 6e75 6d20 3c68 7474 7073 3a2f  IntEnum <https:/
+000006e0: 2f64 6f63 732e 7079 7468 6f6e 2e6f 7267  /docs.python.org
+000006f0: 2f33 2f6c 6962 7261 7279 2f65 6e75 6d2e  /3/library/enum.
+00000700: 6874 6d6c 2365 6e75 6d2e 496e 7445 6e75  html#enum.IntEnu
+00000710: 6d3e 605f 5f2e 0d0a 0d0a 2e2e 2063 6f64  m>`__....... cod
+00000720: 653a 3a20 7079 7468 6f6e 0d0a 0d0a 2020  e:: python....  
+00000730: 2020 696d 706f 7274 2073 7973 0d0a 2020    import sys..  
+00000740: 2020 6672 6f6d 2065 7869 7473 7461 7475    from exitstatu
+00000750: 7320 696d 706f 7274 2045 7869 7453 7461  s import ExitSta
+00000760: 7475 730d 0a0d 0a20 2020 2073 7973 2e65  tus....    sys.e
+00000770: 7869 7428 4578 6974 5374 6174 7573 2e73  xit(ExitStatus.s
+00000780: 7563 6365 7373 290d 0a0d 0a52 656c 6561  uccess)....Relea
+00000790: 7365 730d 0a2d 2d2d 2d2d 2d2d 2d0d 0a0d  ses..--------...
+000007a0: 0a32 2e34 2e30 2028 3230 3233 2d30 342d  .2.4.0 (2023-04-
+000007b0: 3330 290d 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e  30)..^^^^^^^^^^^
+000007c0: 5e5e 5e5e 5e5e 5e0d 0a0d 0a2d 2041 6464  ^^^^^^^....- Add
+000007d0: 2073 7570 706f 7274 2066 6f72 2050 7974   support for Pyt
+000007e0: 686f 6e20 332e 3131 0d0a 0d0a 322e 332e  hon 3.11....2.3.
+000007f0: 3020 3230 3232 2d31 312d 3032 0d0a 5e5e  0 2022-11-02..^^
+00000800: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 0d0a  ^^^^^^^^^^^^^^..
+00000810: 0d0a 2d20 4164 6420 6060 7079 2e74 7970  ..- Add ``py.typ
+00000820: 6564 6060 2066 696c 6520 746f 2070 6163  ed`` file to pac
+00000830: 6b61 6765 2074 6f20 7375 7070 6f72 7420  kage to support 
+00000840: 4d79 7079 2074 7970 6520 6368 6563 6b69  Mypy type checki
+00000850: 6e67 2e0d 0a2d 2052 6566 6163 746f 7220  ng...- Refactor 
+00000860: 7468 6520 7072 6f6a 6563 7420 696e 746f  the project into
+00000870: 2061 6e20 696e 7374 616c 6c61 626c 6520   an installable 
+00000880: 7061 636b 6167 6520 7261 7468 6572 2074  package rather t
+00000890: 6861 6e20 616e 2069 6e73 7461 6c6c 6162  han an installab
+000008a0: 6c65 206d 6f64 756c 652e 0d0a 2d20 4472  le module...- Dr
+000008b0: 6f70 2073 7570 706f 7274 2066 6f72 2050  op support for P
+000008c0: 7974 686f 6e20 332e 370d 0a0d 0a32 2e32  ython 3.7....2.2
+000008d0: 2e30 2032 3032 312d 3131 2d30 360d 0a5e  .0 2021-11-06..^
+000008e0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e0d  ^^^^^^^^^^^^^^^.
+000008f0: 0a0d 0a2d 2053 7570 706f 7274 2050 7974  ...- Support Pyt
+00000900: 686f 6e20 332e 3130 2061 6e64 2064 726f  hon 3.10 and dro
+00000910: 7020 332e 362e 0d0a 0d0a 322e 312e 3020  p 3.6.....2.1.0 
+00000920: 3230 3230 2d31 322d 3237 0d0a 5e5e 5e5e  2020-12-27..^^^^
+00000930: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 0d0a 0d0a  ^^^^^^^^^^^^....
+00000940: 2d20 4472 6f70 2050 7974 686f 6e20 332e  - Drop Python 3.
+00000950: 3520 616e 6420 7375 7070 6f72 7420 5079  5 and support Py
+00000960: 7468 6f6e 2033 2e39 2e0d 0a2d 2053 7769  thon 3.9...- Swi
+00000970: 7463 6820 746f 2047 6974 4875 6220 4163  tch to GitHub Ac
+00000980: 7469 6f6e 7320 666f 7220 4349 2e0d 0a0d  tions for CI....
+00000990: 0a32 2e30 2e31 2032 3032 302d 3034 2d32  .2.0.1 2020-04-2
+000009a0: 360d 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  6..^^^^^^^^^^^^^
+000009b0: 5e5e 5e0d 0a0d 0a2d 2055 7064 6174 6520  ^^^....- Update 
+000009c0: 4c49 4345 4e53 4520 6669 6c65 2e0d 0a0d  LICENSE file....
+000009d0: 0a32 2e30 2e30 2032 3032 302d 3033 2d32  .2.0.0 2020-03-2
+000009e0: 390d 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  9..^^^^^^^^^^^^^
+000009f0: 5e5e 5e0d 0a0d 0a2d 2044 726f 7020 5079  ^^^....- Drop Py
+00000a00: 7468 6f6e 2032 2e37 2073 7570 706f 7274  thon 2.7 support
+00000a10: 2e0d 0a0d 0a31 2e34 2e31 2032 3032 302d  .....1.4.1 2020-
+00000a20: 3033 2d32 390d 0a5e 5e5e 5e5e 5e5e 5e5e  03-29..^^^^^^^^^
+00000a30: 5e5e 5e5e 5e5e 5e0d 0a0d 0a2d 2041 6464  ^^^^^^^....- Add
+00000a40: 2060 6070 7974 686f 6e5f 7265 7175 6972   ``python_requir
+00000a50: 6573 6060 2066 6965 6c64 2074 6f20 6060  es`` field to ``
+00000a60: 7365 7475 702e 7079 6060 2e0d 0a0d 0a31  setup.py``.....1
+00000a70: 2e34 2e30 2032 3031 392d 3132 2d31 340d  .4.0 2019-12-14.
+00000a80: 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  .^^^^^^^^^^^^^^^
+00000a90: 5e0d 0a0d 0a2d 2044 726f 7020 5079 7468  ^....- Drop Pyth
+00000aa0: 6f6e 2033 2e34 2061 6e64 2073 7570 706f  on 3.4 and suppo
+00000ab0: 7274 2050 7974 686f 6e20 332e 382e 0d0a  rt Python 3.8...
+00000ac0: 2d20 496e 636c 7564 6520 6c69 6365 6e73  - Include licens
+00000ad0: 6520 6669 6c65 2e0d 0a0d 0a31 2e33 2e30  e file.....1.3.0
+00000ae0: 202d 2032 3031 382d 3037 2d30 390d 0a5e   - 2018-07-09..^
+00000af0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
+00000b00: 5e0d 0a0d 0a44 726f 7020 5079 7468 6f6e  ^....Drop Python
+00000b10: 2033 2e33 2061 6e64 2073 7570 706f 7274   3.3 and support
+00000b20: 2050 7974 686f 6e20 332e 372e 0d0a 0d0a   Python 3.7.....
+00000b30: 312e 322e 3020 2d20 3230 3136 2d31 322d  1.2.0 - 2016-12-
+00000b40: 3331 0d0a 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  31..^^^^^^^^^^^^
+00000b50: 5e5e 5e5e 5e5e 0d0a 0d0a 5375 7070 6f72  ^^^^^^....Suppor
+00000b60: 7420 5079 7468 6f6e 2033 2e36 2e0d 0a0d  t Python 3.6....
+00000b70: 0a31 2e31 2e30 202d 2032 3031 362d 3130  .1.1.0 - 2016-10
+00000b80: 2d31 310d 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e  -11..^^^^^^^^^^^
+00000b90: 5e5e 5e5e 5e5e 5e0d 0a0d 0a41 6464 2064  ^^^^^^^....Add d
+00000ba0: 6f63 7374 7269 6e67 7320 616e 6420 7369  ocstrings and si
+00000bb0: 6d70 6c69 6679 2063 6865 636b 696e 6720  mplify checking 
+00000bc0: 666f 7220 6060 656e 756d 3334 6060 2064  for ``enum34`` d
+00000bd0: 6570 656e 6465 6e63 7920 6e65 6564 2e0d  ependency need..
+00000be0: 0a0d 0a31 2e30 2e30 202d 2032 3031 362d  ...1.0.0 - 2016-
+00000bf0: 3036 2d31 300d 0a5e 5e5e 5e5e 5e5e 5e5e  06-10..^^^^^^^^^
+00000c00: 5e5e 5e5e 5e5e 5e5e 5e0d 0a0d 0a49 6e69  ^^^^^^^^^....Ini
+00000c10: 7469 616c 2072 656c 6561 7365 2e0d 0a    tial release...
```

### Comparing `exitstatus-2.3.0/exitstatus.egg-info/PKG-INFO` & `exitstatus-2.4.0/exitstatus.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,138 +1,144 @@
-Metadata-Version: 2.1
-Name: exitstatus
-Version: 2.3.0
-Summary: POSIX exit status codes
-Home-page: https://github.com/johnthagen/exitstatus
-Author: John Hagen
-Author-email: johnthagen@gmail.com
-License: MIT
-Keywords: exit status POSIX
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Typing :: Typed
-Requires-Python: >=3.8
-License-File: LICENSE.txt
-
-``exitstatus`` - POSIX exit status definitions
-==============================================
-
-.. image:: https://github.com/johnthagen/exitstatus/workflows/python/badge.svg
-    :target: https://github.com/johnthagen/exitstatus/actions
-
-.. image:: https://codeclimate.com/github/johnthagen/exitstatus/badges/gpa.svg
-   :target: https://codeclimate.com/github/johnthagen/exitstatus/
-
-.. image:: https://codeclimate.com/github/johnthagen/exitstatus/badges/issue_count.svg
-   :target: https://codeclimate.com/github/johnthagen/exitstatus/
-
-.. image:: https://codecov.io/github/johnthagen/exitstatus/coverage.svg
-    :target: https://codecov.io/github/johnthagen/exitstatus/
-
-.. image:: https://img.shields.io/pypi/v/exitstatus.svg
-    :target: https://pypi.python.org/pypi/exitstatus/
-
-.. image:: https://img.shields.io/pypi/status/exitstatus.svg
-    :target: https://pypi.python.org/pypi/exitstatus/
-
-.. image:: https://img.shields.io/pypi/pyversions/exitstatus.svg
-    :target: https://pypi.python.org/pypi/exitstatus/
-
-``exitstatus`` provides expressive, portable definitions for the
-`standard POSIX exit codes <https://www.gnu.org/software/libc/manual/html_node/Exit-Status.html>`__.
-While Python does provide some Unix-specific exit status codes in the
-`os module <https://docs.python.org/3/library/os.html#os._exit>`__, they are not portable to
-all platforms and are missing the generic failure case.
-
-
-Installation
-------------
-
-You can install, upgrade, and uninstall ``exitstatus`` with these commands:
-
-.. code:: shell-session
-
-    $ pip install exitstatus
-    $ pip install --upgrade exitstatus
-    $ pip uninstall exitstatus
-
-Usage
------
-
-Exit status codes are defined in a simple to use
-`IntEnum <https://docs.python.org/3/library/enum.html#enum.IntEnum>`__.
-
-.. code:: python
-
-    import sys
-    from exitstatus import ExitStatus
-
-    sys.exit(ExitStatus.success)
-
-Releases
---------
-
-2.3.0 2022-11-02
-^^^^^^^^^^^^^^^^
-
-- Add ``py.typed`` file to package to support Mypy type checking.
-- Refactor the project into an installable package rather than an installable module.
-- Drop support for Python 3.7
-
-2.2.0 2021-11-06
-^^^^^^^^^^^^^^^^
-
-- Support Python 3.10 and drop 3.6.
-
-2.1.0 2020-12-27
-^^^^^^^^^^^^^^^^
-
-- Drop Python 3.5 and support Python 3.9.
-- Switch to GitHub Actions for CI.
-
-2.0.1 2020-04-26
-^^^^^^^^^^^^^^^^
-
-- Update LICENSE file.
-
-2.0.0 2020-03-29
-^^^^^^^^^^^^^^^^
-
-- Drop Python 2.7 support.
-
-1.4.1 2020-03-29
-^^^^^^^^^^^^^^^^
-
-- Add ``python_requires`` field to ``setup.py``.
-
-1.4.0 2019-12-14
-^^^^^^^^^^^^^^^^
-
-- Drop Python 3.4 and support Python 3.8.
-- Include license file.
-
-1.3.0 - 2018-07-09
-^^^^^^^^^^^^^^^^^^
-
-Drop Python 3.3 and support Python 3.7.
-
-1.2.0 - 2016-12-31
-^^^^^^^^^^^^^^^^^^
-
-Support Python 3.6.
-
-1.1.0 - 2016-10-11
-^^^^^^^^^^^^^^^^^^
-
-Add docstrings and simplify checking for ``enum34`` dependency need.
-
-1.0.0 - 2016-06-10
-^^^^^^^^^^^^^^^^^^
-
-Initial release.
+Metadata-Version: 2.1
+Name: exitstatus
+Version: 2.4.0
+Summary: POSIX exit status codes
+Home-page: https://github.com/johnthagen/exitstatus
+Author: John Hagen
+Author-email: johnthagen@gmail.com
+License: MIT
+Keywords: exit status POSIX
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+License-File: LICENSE.txt
+
+``exitstatus`` - POSIX exit status definitions
+==============================================
+
+.. image:: https://github.com/johnthagen/exitstatus/workflows/python/badge.svg
+    :target: https://github.com/johnthagen/exitstatus/actions
+
+.. image:: https://codeclimate.com/github/johnthagen/exitstatus/badges/gpa.svg
+   :target: https://codeclimate.com/github/johnthagen/exitstatus/
+
+.. image:: https://codeclimate.com/github/johnthagen/exitstatus/badges/issue_count.svg
+   :target: https://codeclimate.com/github/johnthagen/exitstatus/
+
+.. image:: https://codecov.io/github/johnthagen/exitstatus/coverage.svg
+    :target: https://codecov.io/github/johnthagen/exitstatus/
+
+.. image:: https://img.shields.io/pypi/v/exitstatus.svg
+    :target: https://pypi.python.org/pypi/exitstatus/
+
+.. image:: https://img.shields.io/pypi/status/exitstatus.svg
+    :target: https://pypi.python.org/pypi/exitstatus/
+
+.. image:: https://img.shields.io/pypi/pyversions/exitstatus.svg
+    :target: https://pypi.python.org/pypi/exitstatus/
+
+``exitstatus`` provides expressive, portable definitions for the
+`standard POSIX exit codes <https://www.gnu.org/software/libc/manual/html_node/Exit-Status.html>`__.
+While Python does provide some Unix-specific exit status codes in the
+`os module <https://docs.python.org/3/library/os.html#os._exit>`__, they are not portable to
+all platforms and are missing the generic failure case.
+
+
+Installation
+------------
+
+You can install, upgrade, and uninstall ``exitstatus`` with these commands:
+
+.. code:: shell-session
+
+    $ pip install exitstatus
+    $ pip install --upgrade exitstatus
+    $ pip uninstall exitstatus
+
+Usage
+-----
+
+Exit status codes are defined in a simple to use
+`IntEnum <https://docs.python.org/3/library/enum.html#enum.IntEnum>`__.
+
+.. code:: python
+
+    import sys
+    from exitstatus import ExitStatus
+
+    sys.exit(ExitStatus.success)
+
+Releases
+--------
+
+2.4.0 (2023-04-30)
+^^^^^^^^^^^^^^^^^^
+
+- Add support for Python 3.11
+
+2.3.0 2022-11-02
+^^^^^^^^^^^^^^^^
+
+- Add ``py.typed`` file to package to support Mypy type checking.
+- Refactor the project into an installable package rather than an installable module.
+- Drop support for Python 3.7
+
+2.2.0 2021-11-06
+^^^^^^^^^^^^^^^^
+
+- Support Python 3.10 and drop 3.6.
+
+2.1.0 2020-12-27
+^^^^^^^^^^^^^^^^
+
+- Drop Python 3.5 and support Python 3.9.
+- Switch to GitHub Actions for CI.
+
+2.0.1 2020-04-26
+^^^^^^^^^^^^^^^^
+
+- Update LICENSE file.
+
+2.0.0 2020-03-29
+^^^^^^^^^^^^^^^^
+
+- Drop Python 2.7 support.
+
+1.4.1 2020-03-29
+^^^^^^^^^^^^^^^^
+
+- Add ``python_requires`` field to ``setup.py``.
+
+1.4.0 2019-12-14
+^^^^^^^^^^^^^^^^
+
+- Drop Python 3.4 and support Python 3.8.
+- Include license file.
+
+1.3.0 - 2018-07-09
+^^^^^^^^^^^^^^^^^^
+
+Drop Python 3.3 and support Python 3.7.
+
+1.2.0 - 2016-12-31
+^^^^^^^^^^^^^^^^^^
+
+Support Python 3.6.
+
+1.1.0 - 2016-10-11
+^^^^^^^^^^^^^^^^^^
+
+Add docstrings and simplify checking for ``enum34`` dependency need.
+
+1.0.0 - 2016-06-10
+^^^^^^^^^^^^^^^^^^
+
+Initial release.
```

### Comparing `exitstatus-2.3.0/setup.py` & `exitstatus-2.4.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-from pathlib import Path
-
-import setuptools
-
-project_dir = Path(__file__).parent
-
-setuptools.setup(
-    name="exitstatus",
-    version="2.3.0",
-    description="POSIX exit status codes",
-    long_description=project_dir.joinpath("README.rst").read_text(encoding="utf-8"),
-    keywords="exit status POSIX",
-    author="John Hagen",
-    author_email="johnthagen@gmail.com",
-    url="https://github.com/johnthagen/exitstatus",
-    packages=["exitstatus"],
-    package_data={"exitstatus": ["py.typed"]},
-    python_requires=">=3.8",
-    zip_safe=False,
-    license="MIT",
-    license_files=["LICENSE.txt"],
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Typing :: Typed",
-    ],
-)
+from pathlib import Path
+
+import setuptools
+
+project_dir = Path(__file__).parent
+
+setuptools.setup(
+    name="exitstatus",
+    version="2.4.0",
+    description="POSIX exit status codes",
+    long_description=project_dir.joinpath("README.rst").read_text(encoding="utf-8"),
+    keywords="exit status POSIX",
+    author="John Hagen",
+    author_email="johnthagen@gmail.com",
+    url="https://github.com/johnthagen/exitstatus",
+    packages=["exitstatus"],
+    package_data={"exitstatus": ["py.typed"]},
+    python_requires=">=3.8",
+    zip_safe=False,
+    license="MIT",
+    license_files=["LICENSE.txt"],
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Typing :: Typed",
+    ],
+)
```

