# Comparing `tmp/pynamer-0.4.0.tar.gz` & `tmp/pynamer-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-0.4.0.tar", last modified: Thu Apr 27 19:12:20 2023, max compression
+gzip compressed data, was "pynamer-0.5.0.tar", last modified: Sun Apr 30 20:16:46 2023, max compression
```

## Comparing `pynamer-0.4.0.tar` & `pynamer-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 19:12:20.828071 pynamer-0.4.0/
--rw-rw-rw-   0        0        0      161 2023-04-21 18:16:39.000000 pynamer-0.4.0/AUTHORS.md
--rw-rw-rw-   0        0        0     2923 2023-04-27 19:12:05.000000 pynamer-0.4.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2023-04-21 17:08:24.000000 pynamer-0.4.0/LICENSE
--rw-rw-rw-   0        0        0      237 2023-04-25 12:30:17.000000 pynamer-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0    12191 2023-04-27 19:12:20.828071 pynamer-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    10852 2023-04-27 19:11:48.000000 pynamer-0.4.0/README.md
--rw-rw-rw-   0        0        0     2344 2023-04-21 17:08:24.000000 pynamer-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0     1784 2023-04-27 19:12:20.828071 pynamer-0.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-27 19:12:20.743339 pynamer-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 19:12:20.796822 pynamer-0.4.0/src/pynamer/
--rw-rw-rw-   0        0        0       10 2023-04-25 12:29:58.000000 pynamer-0.4.0/src/pynamer/README.md
--rw-rw-rw-   0        0        0     1781 2023-04-27 19:12:06.000000 pynamer-0.4.0/src/pynamer/__init__.py
--rw-rw-rw-   0        0        0       17 2023-04-27 18:25:05.000000 pynamer-0.4.0/src/pynamer/project_count.pickle
-drwxrwxrwx   0        0        0        0 2023-04-27 19:12:20.812451 pynamer-0.4.0/src/pynamer/project_name/
--rw-rw-rw-   0        0        0       37 2023-04-14 21:59:18.000000 pynamer-0.4.0/src/pynamer/project_name/__init__.py
--rw-rw-rw-   0        0        0    12662 2023-04-27 19:11:48.000000 pynamer-0.4.0/src/pynamer/pynamer.py
--rw-rw-rw-   0        0        0  6781803 2023-04-27 18:36:07.000000 pynamer-0.4.0/src/pynamer/pypi_index.txt
--rw-rw-rw-   0        0        0      411 2023-04-26 19:24:01.000000 pynamer-0.4.0/src/pynamer/setup.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 19:12:20.812451 pynamer-0.4.0/src/pynamer.egg-info/
--rw-rw-rw-   0        0        0    12191 2023-04-27 19:12:20.000000 pynamer-0.4.0/src/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-04-27 19:12:20.000000 pynamer-0.4.0/src/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 19:12:20.000000 pynamer-0.4.0/src/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-04-27 19:12:20.000000 pynamer-0.4.0/src/pynamer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       46 2023-04-27 19:12:20.000000 pynamer-0.4.0/src/pynamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-27 19:12:20.000000 pynamer-0.4.0/src/pynamer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 19:12:20.828071 pynamer-0.4.0/tests/
--rw-rw-rw-   0        0        0      300 2023-04-27 19:11:48.000000 pynamer-0.4.0/tests/test_pynamer.py
+drwxrwxrwx   0        0        0        0 2023-04-30 20:16:46.346319 pynamer-0.5.0/
+-rw-rw-rw-   0        0        0      161 2023-04-21 18:16:39.000000 pynamer-0.5.0/AUTHORS.md
+-rw-rw-rw-   0        0        0     3397 2023-04-30 20:16:31.000000 pynamer-0.5.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-04-21 17:08:24.000000 pynamer-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-04-25 12:30:17.000000 pynamer-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    12177 2023-04-30 20:16:46.346319 pynamer-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10845 2023-04-30 20:14:17.000000 pynamer-0.5.0/README.md
+-rw-rw-rw-   0        0        0     2344 2023-04-21 17:08:24.000000 pynamer-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1808 2023-04-30 20:16:46.361953 pynamer-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 20:16:46.265598 pynamer-0.5.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 20:16:46.330677 pynamer-0.5.0/src/pynamer/
+-rw-rw-rw-   0        0        0       10 2023-04-25 12:29:58.000000 pynamer-0.5.0/src/pynamer/README.md
+-rw-rw-rw-   0        0        0     1780 2023-04-30 20:16:31.000000 pynamer-0.5.0/src/pynamer/__init__.py
+-rw-rw-rw-   0        0        0       17 2023-04-30 20:13:43.000000 pynamer-0.5.0/src/pynamer/project_count.pickle
+drwxrwxrwx   0        0        0        0 2023-04-30 20:16:46.346319 pynamer-0.5.0/src/pynamer/project_name/
+-rw-rw-rw-   0        0        0       37 2023-04-14 21:59:18.000000 pynamer-0.5.0/src/pynamer/project_name/__init__.py
+-rw-rw-rw-   0        0        0    20074 2023-04-30 20:12:42.000000 pynamer-0.5.0/src/pynamer/pynamer.py
+-rw-rw-rw-   0        0        0  7243286 2023-04-30 09:18:06.000000 pynamer-0.5.0/src/pynamer/pypi_index.txt
+-rw-rw-rw-   0        0        0      427 2023-04-29 19:54:50.000000 pynamer-0.5.0/src/pynamer/setup.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 20:16:46.330677 pynamer-0.5.0/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0    12177 2023-04-30 20:16:46.000000 pynamer-0.5.0/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-04-30 20:16:46.000000 pynamer-0.5.0/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 20:16:46.000000 pynamer-0.5.0/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-04-30 20:16:46.000000 pynamer-0.5.0/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       64 2023-04-30 20:16:46.000000 pynamer-0.5.0/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-30 20:16:46.000000 pynamer-0.5.0/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 20:16:46.346319 pynamer-0.5.0/tests/
+-rw-rw-rw-   0        0        0      309 2023-04-30 20:14:15.000000 pynamer-0.5.0/tests/test_pynamer.py
```

### Comparing `pynamer-0.4.0/CHANGELOG.md` & `pynamer-0.5.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.5.0 (2023-04-30)
+### Feature
+* Add pypi search function and rich tables ([`089356b`](https://github.com/Stephen-RA-King/pynamer/commit/089356b574a3eca65dfcac69951f335a97e5e063))
+
+### Fix
+* Total projects found ([`4b42701`](https://github.com/Stephen-RA-King/pynamer/commit/4b42701fc9655573918251179b44e21855adc09b))
+
+### Documentation
+* Minor updates ([`1521d13`](https://github.com/Stephen-RA-King/pynamer/commit/1521d13be80aaee3b745ecb2da6362fe4c488b94))
+
 ## v0.4.0 (2023-04-27)
 ### Feature
 * Add generate_pypi_index & pypi_search_index functions ([`96ff544`](https://github.com/Stephen-RA-King/pynamer/commit/96ff54496f8f6455a1a011ac723fd05afa1c547b))
 
 ### Documentation
 * Bump version ([`d985a36`](https://github.com/Stephen-RA-King/pynamer/commit/d985a36edb4ada5f59786e1c55fff832e56ca1ec))
```

### Comparing `pynamer-0.4.0/LICENSE` & `pynamer-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamer-0.4.0/PKG-INFO` & `pynamer-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 0.4.0
+Version: 0.5.0
 Summary: Utility to find an available package name on the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -191,16 +191,16 @@
 zeedonk DOES NOT EXIST
 ```
 
 # Usage
 
 ---
 
-
 Display the options ...
+
 ```commandline
 pynamer --help
 usage: pynamer [-h] [-r] [-d] [-f FILE] [-o OUTPUT] [-a] [projects ...]
 
 Determine if project name is available on pypi with the option to 'register' it for future use if available
 
 positional arguments:
@@ -213,21 +213,14 @@
   -f FILE, --file FILE  File containing a list of projects to analyze
   -o OUTPUT, --output OUTPUT
                         File to output the results to
   -a, --alltests        Perform all tests
   -g, --generate        Generate a new PyPI simple index
 ```
 
-
-
-
-
-
-
-
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://pynamer.readthedocs.io/en/latest/)
 
 -   [**Example Usage**](https://pynamer.readthedocs.io/en/latest/example.html)
```

### Comparing `pynamer-0.4.0/README.md` & `pynamer-0.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -163,16 +163,16 @@
 zeedonk DOES NOT EXIST
 ```
 
 # Usage
 
 ---
 
-
 Display the options ...
+
 ```commandline
 pynamer --help
 usage: pynamer [-h] [-r] [-d] [-f FILE] [-o OUTPUT] [-a] [projects ...]
 
 Determine if project name is available on pypi with the option to 'register' it for future use if available
 
 positional arguments:
@@ -185,21 +185,14 @@
   -f FILE, --file FILE  File containing a list of projects to analyze
   -o OUTPUT, --output OUTPUT
                         File to output the results to
   -a, --alltests        Perform all tests
   -g, --generate        Generate a new PyPI simple index
 ```
 
-
-
-
-
-
-
-
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://pynamer.readthedocs.io/en/latest/)
 
 -   [**Example Usage**](https://pynamer.readthedocs.io/en/latest/example.html)
```

### Comparing `pynamer-0.4.0/pyproject.toml` & `pynamer-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynamer-0.4.0/setup.cfg` & `pynamer-0.5.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -63,50 +63,51 @@
 000003e0: 630d 0a70 6163 6b61 6765 7320 3d20 6669  c..packages = fi
 000003f0: 6e64 3a0d 0a70 726f 6a65 6374 5f75 726c  nd:..project_url
 00000400: 7320 3d20 0d0a 696e 636c 7564 655f 7061  s = ..include_pa
 00000410: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
 00000420: 650d 0a70 7974 686f 6e5f 7265 7175 6972  e..python_requir
 00000430: 6573 203d 203e 3d33 2e39 0d0a 696e 7374  es = >=3.9..inst
 00000440: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
-00000450: 0a09 6a69 6e6a 6132 0d0a 0962 7569 6c64  ..jinja2...build
-00000460: 0d0a 0970 7979 616d 6c0d 0a09 7265 7175  ...pyyaml...requ
-00000470: 6573 7473 0d0a 0974 7769 6e65 0d0a 0974  ests...twine...t
-00000480: 7164 6d0d 0a09 7768 6565 6c0d 0a0d 0a5b  qdm...wheel....[
-00000490: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
-000004a0: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-000004b0: 7372 630d 0a0d 0a5b 6f70 7469 6f6e 732e  src....[options.
-000004c0: 7061 636b 6167 655f 6461 7461 5d0d 0a70  package_data]..p
-000004d0: 796e 616d 6572 203d 200d 0a09 7365 7475  ynamer = ...setu
-000004e0: 702e 7478 740d 0a09 5245 4144 4d45 2e6d  p.txt...README.m
-000004f0: 640d 0a09 7072 6f6a 6563 745f 6e61 6d65  d...project_name
-00000500: 0d0a 0970 726f 6a65 6374 5f6e 616d 652f  ...project_name/
-00000510: 5f5f 696e 6974 5f5f 2e70 790d 0a09 7072  __init__.py...pr
-00000520: 6f6a 6563 745f 636f 756e 742e 7069 636b  oject_count.pick
-00000530: 6c65 0d0a 0970 7970 695f 696e 6465 782e  le...pypi_index.
-00000540: 7478 740d 0a0d 0a5b 6f70 7469 6f6e 732e  txt....[options.
-00000550: 656e 7472 795f 706f 696e 7473 5d0d 0a63  entry_points]..c
-00000560: 6f6e 736f 6c65 5f73 6372 6970 7473 203d  onsole_scripts =
-00000570: 200d 0a09 7079 6e61 6d65 7220 3d20 7079   ...pynamer = py
-00000580: 6e61 6d65 722e 7079 6e61 6d65 723a 6d61  namer.pynamer:ma
-00000590: 696e 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a  in....[flake8]..
-000005a0: 646f 6373 7472 696e 672d 636f 6e76 656e  docstring-conven
-000005b0: 7469 6f6e 203d 206e 756d 7079 0d0a 6d61  tion = numpy..ma
-000005c0: 782d 636f 6d70 6c65 7869 7479 203d 2031  x-complexity = 1
-000005d0: 380d 0a6d 6178 2d6c 696e 652d 6c65 6e67  8..max-line-leng
-000005e0: 7468 203d 2038 380d 0a73 656c 6563 7420  th = 88..select 
-000005f0: 3d20 422c 2042 392c 2043 2c20 442c 2045  = B, B9, C, D, E
-00000600: 2c20 462c 204e 2c20 570d 0a65 7863 6c75  , F, N, W..exclu
-00000610: 6465 203d 2074 6573 7473 2f2a 2c2e 746f  de = tests/*,.to
-00000620: 782f 2a2c 2e6e 6f78 2f2a 2c64 6f63 732f  x/*,.nox/*,docs/
-00000630: 2a2c 2e67 6974 2f2a 2c2e 6769 7468 7562  *,.git/*,.github
-00000640: 2f2a 0d0a 6967 6e6f 7265 203d 200d 0a09  /*..ignore = ...
-00000650: 4532 3033 2c0d 0a09 5735 3033 2c0d 0a09  E203,...W503,...
-00000660: 4634 3031 2c0d 0a70 6572 2d66 696c 652d  F401,..per-file-
-00000670: 6967 6e6f 7265 7320 3d20 0d0a 095f 5f69  ignores = ...__i
-00000680: 6e69 745f 5f2e 7079 3a46 3430 310d 0a09  nit__.py:F401...
-00000690: 7061 7468 6d61 6769 632e 7079 3a46 3430  pathmagic.py:F40
-000006a0: 310d 0a09 7465 7374 5f70 796e 616d 6572  1...test_pynamer
-000006b0: 2e70 793a 4634 3031 0d0a 0970 796e 616d  .py:F401...pynam
-000006c0: 6572 2e70 793a 4634 3031 0d0a 0d0a 5b65  er.py:F401....[e
-000006d0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-000006e0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-000006f0: 203d 2030 0d0a 0d0a                       = 0....
+00000450: 0a09 6a69 6e6a 6132 0d0a 0962 7334 0d0a  ..jinja2...bs4..
+00000460: 0962 7569 6c64 0d0a 0963 6f6c 6f72 616d  .build...coloram
+00000470: 610d 0a09 7079 7961 6d6c 0d0a 0972 6571  a...pyyaml...req
+00000480: 7565 7374 730d 0a09 7269 6368 0d0a 0974  uests...rich...t
+00000490: 7769 6e65 0d0a 0974 7164 6d0d 0a09 7768  wine...tqdm...wh
+000004a0: 6565 6c0d 0a0d 0a5b 6f70 7469 6f6e 732e  eel....[options.
+000004b0: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+000004c0: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
+000004d0: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
+000004e0: 6461 7461 5d0d 0a70 796e 616d 6572 203d  data]..pynamer =
+000004f0: 200d 0a09 7365 7475 702e 7478 740d 0a09   ...setup.txt...
+00000500: 5245 4144 4d45 2e6d 640d 0a09 7072 6f6a  README.md...proj
+00000510: 6563 745f 6e61 6d65 0d0a 0970 726f 6a65  ect_name...proje
+00000520: 6374 5f6e 616d 652f 5f5f 696e 6974 5f5f  ct_name/__init__
+00000530: 2e70 790d 0a09 7072 6f6a 6563 745f 636f  .py...project_co
+00000540: 756e 742e 7069 636b 6c65 0d0a 0970 7970  unt.pickle...pyp
+00000550: 695f 696e 6465 782e 7478 740d 0a0d 0a5b  i_index.txt....[
+00000560: 6f70 7469 6f6e 732e 656e 7472 795f 706f  options.entry_po
+00000570: 696e 7473 5d0d 0a63 6f6e 736f 6c65 5f73  ints]..console_s
+00000580: 6372 6970 7473 203d 200d 0a09 7079 6e61  cripts = ...pyna
+00000590: 6d65 7220 3d20 7079 6e61 6d65 722e 7079  mer = pynamer.py
+000005a0: 6e61 6d65 723a 6d61 696e 0d0a 0d0a 5b66  namer:main....[f
+000005b0: 6c61 6b65 385d 0d0a 646f 6373 7472 696e  lake8]..docstrin
+000005c0: 672d 636f 6e76 656e 7469 6f6e 203d 206e  g-convention = n
+000005d0: 756d 7079 0d0a 6d61 782d 636f 6d70 6c65  umpy..max-comple
+000005e0: 7869 7479 203d 2031 380d 0a6d 6178 2d6c  xity = 18..max-l
+000005f0: 696e 652d 6c65 6e67 7468 203d 2038 380d  ine-length = 88.
+00000600: 0a73 656c 6563 7420 3d20 422c 2042 392c  .select = B, B9,
+00000610: 2043 2c20 442c 2045 2c20 462c 204e 2c20   C, D, E, F, N, 
+00000620: 570d 0a65 7863 6c75 6465 203d 2074 6573  W..exclude = tes
+00000630: 7473 2f2a 2c2e 746f 782f 2a2c 2e6e 6f78  ts/*,.tox/*,.nox
+00000640: 2f2a 2c64 6f63 732f 2a2c 2e67 6974 2f2a  /*,docs/*,.git/*
+00000650: 2c2e 6769 7468 7562 2f2a 0d0a 6967 6e6f  ,.github/*..igno
+00000660: 7265 203d 200d 0a09 4532 3033 2c0d 0a09  re = ...E203,...
+00000670: 5735 3033 2c0d 0a09 4634 3031 2c0d 0a70  W503,...F401,..p
+00000680: 6572 2d66 696c 652d 6967 6e6f 7265 7320  er-file-ignores 
+00000690: 3d20 0d0a 095f 5f69 6e69 745f 5f2e 7079  = ...__init__.py
+000006a0: 3a46 3430 310d 0a09 7061 7468 6d61 6769  :F401...pathmagi
+000006b0: 632e 7079 3a46 3430 310d 0a09 7465 7374  c.py:F401...test
+000006c0: 5f70 796e 616d 6572 2e70 793a 4634 3031  _pynamer.py:F401
+000006d0: 0d0a 0970 796e 616d 6572 2e70 793a 4634  ...pynamer.py:F4
+000006e0: 3031 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  01....[egg_info]
+000006f0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+00000700: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `pynamer-0.4.0/src/pynamer/__init__.py` & `pynamer-0.5.0/src/pynamer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 import pickle
 from importlib.resources import as_file, files
 
 # Third party modules
 import yaml  # type: ignore
 
 __title__ = "pynamer"
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 __author__ = "Stephen R A King"
 __description__ = (
     "Utility to find an available package name on the PyPI repository and register it "
 )
 __email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Stephen R A King"
 
 
 LOGGING_CONFIG = """
 version: 1
-disable_existing_loggers: False
+disable_existing_loggers: True
 handlers:
   console:
     class: logging.StreamHandler
     level: INFO
     stream: ext://sys.stdout
     formatter: basic
   file:
```

### Comparing `pynamer-0.4.0/src/pynamer.egg-info/PKG-INFO` & `pynamer-0.5.0/src/pynamer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 0.4.0
+Version: 0.5.0
 Summary: Utility to find an available package name on the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -191,16 +191,16 @@
 zeedonk DOES NOT EXIST
 ```
 
 # Usage
 
 ---
 
-
 Display the options ...
+
 ```commandline
 pynamer --help
 usage: pynamer [-h] [-r] [-d] [-f FILE] [-o OUTPUT] [-a] [projects ...]
 
 Determine if project name is available on pypi with the option to 'register' it for future use if available
 
 positional arguments:
@@ -213,21 +213,14 @@
   -f FILE, --file FILE  File containing a list of projects to analyze
   -o OUTPUT, --output OUTPUT
                         File to output the results to
   -a, --alltests        Perform all tests
   -g, --generate        Generate a new PyPI simple index
 ```
 
-
-
-
-
-
-
-
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://pynamer.readthedocs.io/en/latest/)
 
 -   [**Example Usage**](https://pynamer.readthedocs.io/en/latest/example.html)
```

