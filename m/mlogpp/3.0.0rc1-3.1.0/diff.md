# Comparing `tmp/mlogpp-3.0.0rc1.tar.gz` & `tmp/mlogpp-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlogpp-3.0.0rc1.tar", last modified: Sun Oct  2 12:14:10 2022, max compression
+gzip compressed data, was "mlogpp-3.1.0.tar", last modified: Sun Apr 30 07:55:16 2023, max compression
```

## Comparing `mlogpp-3.0.0rc1.tar` & `mlogpp-3.1.0.tar`

### file list

```diff
@@ -1,42 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 12:14:10.266318 mlogpp-3.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7174 2022-10-02 12:14:10.266318 mlogpp-3.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6701 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 12:14:10.262318 mlogpp-3.0.0rc1/mlog_emulator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlog_emulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlog_emulator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlog_emulator/building.py
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlog_emulator/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     9402 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlog_emulator/parser_.py
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlog_emulator/vm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 12:14:10.266318 mlogpp-3.0.0rc1/mlogpp/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3226 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/compile.py
--rw-r--r--   0 runner    (1001) docker     (121)     6732 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2298 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/error.py
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/formatting.py
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/function.py
--rw-r--r--   0 runner    (1001) docker     (121)     1805 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)      875 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4563 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/instruction.py
--rw-r--r--   0 runner    (1001) docker     (121)    10358 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/lexer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/linker.py
--rw-r--r--   0 runner    (1001) docker     (121)    34256 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/node.py
--rw-r--r--   0 runner    (1001) docker     (121)     6514 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)    19391 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/parser_.py
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     4676 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/scope.py
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)     2061 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     2531 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/mlogpp/value.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 12:14:10.266318 mlogpp-3.0.0rc1/mlogpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7174 2022-10-02 12:14:10.000000 mlogpp-3.0.0rc1/mlogpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-10-02 12:14:10.000000 mlogpp-3.0.0rc1/mlogpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-02 12:14:10.000000 mlogpp-3.0.0rc1/mlogpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-02 12:14:10.000000 mlogpp-3.0.0rc1/mlogpp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-02 12:14:10.000000 mlogpp-3.0.0rc1/mlogpp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-02 12:14:10.266318 mlogpp-3.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      930 2022-10-02 12:13:53.000000 mlogpp-3.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:55:16.426504 mlogpp-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-30 07:54:53.000000 mlogpp-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-04-30 07:55:16.426504 mlogpp-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-30 07:54:53.000000 mlogpp-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:55:16.422504 mlogpp-3.1.0/mlog_emulator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlog_emulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlog_emulator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlog_emulator/building.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlog_emulator/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlog_emulator/parser_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlog_emulator/vm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:55:16.426504 mlogpp-3.1.0/mlogpp/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:55:16.426504 mlogpp-3.1.0/mlogpp/asm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/asm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/asm/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/asm/parser_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14174 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/generic_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/instruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/linker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33776 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20324 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/parser_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-30 07:54:53.000000 mlogpp-3.1.0/mlogpp/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:55:16.426504 mlogpp-3.1.0/mlogpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-04-30 07:55:16.000000 mlogpp-3.1.0/mlogpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-30 07:55:16.000000 mlogpp-3.1.0/mlogpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 07:55:16.000000 mlogpp-3.1.0/mlogpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-30 07:55:16.000000 mlogpp-3.1.0/mlogpp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-30 07:55:16.000000 mlogpp-3.1.0/mlogpp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-30 07:54:53.000000 mlogpp-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 07:55:16.426504 mlogpp-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-30 07:54:53.000000 mlogpp-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:55:16.426504 mlogpp-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-30 07:54:53.000000 mlogpp-3.1.0/tests/test_compilation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-30 07:54:53.000000 mlogpp-3.1.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-30 07:54:53.000000 mlogpp-3.1.0/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-04-30 07:54:53.000000 mlogpp-3.1.0/tests/test_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-30 07:54:53.000000 mlogpp-3.1.0/tests/test_linker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-30 07:54:53.000000 mlogpp-3.1.0/tests/test_scopes.py
```

### Comparing `mlogpp-3.0.0rc1/LICENSE` & `mlogpp-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlogpp-3.0.0rc1/PKG-INFO` & `mlogpp-3.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: mlogpp
-Version: 3.0.0rc1
-Summary: statically typed high level mindustry logic language
-Home-page: https://github.com/albi-c/mlog++
-Author: albi-c
-Project-URL: Bug Tracker, https://github.com/albi-c/mlog++/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # mlog++
 
 [![Run Unit Tests](https://github.com/albi-c/mlogpp/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/albi-c/mlogpp/actions/workflows/test.yml)
 
 statically typed high level mindustry logic language
 
 ## Installation:
@@ -26,14 +12,15 @@
 
 ### Options:
 * `-o:f`, `--output-file` - output to file
 * `-o:s`, `--output-stdout` - output to stdout
 * `-o:c`, `--output-clip` - output to clipboard (default)
 * `-v`, `--verbose` - output more information
 * `-l`, `--lines` - print line numbers when output is stdout
+* `-a`, `--assembly` - compile as mlog++ assembly
 * `-V`, `--version` - print version and exit
 
 ## Examples:
 ### Hello, World:
 ```javascript
 print("Hello, World!")
 printflush(message1)
@@ -106,20 +93,37 @@
 print(" ")
 print(b)
 
 printflush(message1)
 ```
 Prints `0 10`
 
+### Assembly:
+```javascript
+{LOOP_LENGTH = 2 + 3}
+
+i = 0
+loop_start:
+    i += 1
+    
+    print(i)
+    print("\n")
+    
+    :loop_start (i < {LOOP_LENGTH})
+
+printflush(message1)
+```
+Prints `1 2 3 4 5`
+
 ### Longer examples can be found in `examples/`
 
 ## Features:
 * variables \
   `num x = 1`
-* types \
+* types 
   * `num`, `str`
   * `Block`, `Unit`,
   * `BlockType`, `UnitType`, `ItemType`, `LiquidType`,
   * `Controller`, `Team`
 * comments \
   `# comment`
 * memory cell access \
@@ -137,14 +141,18 @@
 * ranges \
   `for (i : 5) { print(i) }`
 * break / continue
 * native functions \
   `ubind(@mega)`
 * constants \
   `const VALUE = 30`
+* inline python subset in assembly \
+  `{x = 7 ^ 2}`   
+  `print({y = x // 2})`
+  `{"cell" + x}[0] = y`
 
 ## Native functions:
 * read `result`, `cell`, `position`
     * Read data from `cell` at `position` to `result`
 * write `data`, `cell`, `position`
     * Write `data` to `cell` at `position`
 * draw `operation`, `arg0` ... `arg5`
@@ -173,15 +181,15 @@
     * Commands:
         * enabled `block`, `enabled`
         * shoot `block`, `x`, `y`, `shoot`
         * shootp `block`, `unit`, `shoot`
         * config `block`, `configuration`
         * color `block`, `red`, `green`, `blue`
 * radar `filter0` ... `filter2`, `sort`, `block`, `order`, `result`
-    * Find an unit near `block` and store it in `result`
+    * Find a unit near `block` and store it in `result`
     * Filters:
         * any
         * enemy
         * ally
         * player
         * attacker
         * flying
```

### Comparing `mlogpp-3.0.0rc1/README.md` & `mlogpp-3.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: mlogpp
+Version: 3.1.0
+Summary: statically typed high level mindustry logic language
+Home-page: https://github.com/albi-c/mlog++
+Author: albi-c
+Project-URL: Bug Tracker, https://github.com/albi-c/mlog++/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # mlog++
 
 [![Run Unit Tests](https://github.com/albi-c/mlogpp/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/albi-c/mlogpp/actions/workflows/test.yml)
 
 statically typed high level mindustry logic language
 
 ## Installation:
@@ -12,14 +26,15 @@
 
 ### Options:
 * `-o:f`, `--output-file` - output to file
 * `-o:s`, `--output-stdout` - output to stdout
 * `-o:c`, `--output-clip` - output to clipboard (default)
 * `-v`, `--verbose` - output more information
 * `-l`, `--lines` - print line numbers when output is stdout
+* `-a`, `--assembly` - compile as mlog++ assembly
 * `-V`, `--version` - print version and exit
 
 ## Examples:
 ### Hello, World:
 ```javascript
 print("Hello, World!")
 printflush(message1)
@@ -92,20 +107,37 @@
 print(" ")
 print(b)
 
 printflush(message1)
 ```
 Prints `0 10`
 
+### Assembly:
+```javascript
+{LOOP_LENGTH = 2 + 3}
+
+i = 0
+loop_start:
+    i += 1
+    
+    print(i)
+    print("\n")
+    
+    :loop_start (i < {LOOP_LENGTH})
+
+printflush(message1)
+```
+Prints `1 2 3 4 5`
+
 ### Longer examples can be found in `examples/`
 
 ## Features:
 * variables \
   `num x = 1`
-* types \
+* types 
   * `num`, `str`
   * `Block`, `Unit`,
   * `BlockType`, `UnitType`, `ItemType`, `LiquidType`,
   * `Controller`, `Team`
 * comments \
   `# comment`
 * memory cell access \
@@ -123,14 +155,18 @@
 * ranges \
   `for (i : 5) { print(i) }`
 * break / continue
 * native functions \
   `ubind(@mega)`
 * constants \
   `const VALUE = 30`
+* inline python subset in assembly \
+  `{x = 7 ^ 2}`   
+  `print({y = x // 2})`
+  `{"cell" + x}[0] = y`
 
 ## Native functions:
 * read `result`, `cell`, `position`
     * Read data from `cell` at `position` to `result`
 * write `data`, `cell`, `position`
     * Write `data` to `cell` at `position`
 * draw `operation`, `arg0` ... `arg5`
@@ -159,15 +195,15 @@
     * Commands:
         * enabled `block`, `enabled`
         * shoot `block`, `x`, `y`, `shoot`
         * shootp `block`, `unit`, `shoot`
         * config `block`, `configuration`
         * color `block`, `red`, `green`, `blue`
 * radar `filter0` ... `filter2`, `sort`, `block`, `order`, `result`
-    * Find an unit near `block` and store it in `result`
+    * Find a unit near `block` and store it in `result`
     * Filters:
         * any
         * enemy
         * ally
         * player
         * attacker
         * flying
```

### Comparing `mlogpp-3.0.0rc1/mlog_emulator/building.py` & `mlogpp-3.1.0/mlog_emulator/building.py`

 * *Files identical despite different names*

### Comparing `mlogpp-3.0.0rc1/mlog_emulator/cli.py` & `mlogpp-3.1.0/mlog_emulator/cli.py`

 * *Files identical despite different names*

### Comparing `mlogpp-3.0.0rc1/mlog_emulator/parser_.py` & `mlogpp-3.1.0/mlog_emulator/parser_.py`

 * *Files identical despite different names*

### Comparing `mlogpp-3.0.0rc1/mlog_emulator/vm.py` & `mlogpp-3.1.0/mlog_emulator/vm.py`

 * *Files identical despite different names*

### Comparing `mlogpp-3.0.0rc1/mlogpp/cli.py` & `mlogpp-3.1.0/mlogpp/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,44 +6,54 @@
 import pyperclip
 
 from .lexer import Lexer, Lexer
 from .preprocess import Preprocessor
 from .parser_ import Parser
 from .optimizer import Optimizer
 from .linker import Linker
-from .error import MlogError
-from .compile import compile_code
+from .error import Error
+from .compile import compile_code, compile_asm
 from . import __version__
 
 
-# input/output method
 class IOMethod(enum.Enum):
+    """
+    Method for code input/output.
+    """
+
     FILE = enum.auto()
     STD = enum.auto()
     CLIP = enum.auto()
 
 
-def main():
+def main() -> None:
+    """
+    Parse command line arguments and compile code.
+    """
+
     parser = argparse.ArgumentParser(description="Mindustry logic compiler", prog="mlog++")
 
     parser.add_argument("file", type=str, help="input file [@clip for clipboard]")
 
     parser.add_argument("-o:f", "--output-file", help="write output to a file")
     parser.add_argument("-o:s", "--output-stdout", help="write output to stdout", action="store_true")
     parser.add_argument("-o:c", "--output-clip", help="write output to clipboard (default)", action="store_true")
 
     parser.add_argument("-v", "--verbose", help="print additional information", action="store_true")
     parser.add_argument("-l", "--lines", help="print line numbers when output to stdout is selected", action="store_true")
 
     parser.add_argument("--print-exceptions", help="print all exceptions from the compilation (development only)", action="store_true")
 
+    parser.add_argument("-a", "--assembly", help="compile assembly", action="store_true")
+
     parser.add_argument("-V", "--version", action="version", version=f"mlog++ {__version__}")
 
     args = parser.parse_args()
 
+    # default output method
     output_method = IOMethod.CLIP
     output_file = ""
 
     verbose = False
 
     # parse arguments
     for k, v in vars(args).items():
@@ -61,41 +71,49 @@
                 verbose = v
 
     # check if input file exists
     if not os.path.isfile(args.file) and args.file != "@clip":
         print(f"Error: input file \"{args.file}\" does not exist")
         sys.exit(1)
 
+    # @clip is clipboard input
     if args.file == "@clip":
         code = pyperclip.paste()
     else:
         with open(args.file, "r") as f:
             code = f.read()
 
     try:
-        out = compile_code(code, args.file)
-    except MlogError as e:
+        if args.assembly:
+            out = compile_asm(code, args.file)
+        else:
+            out = compile_code(code, args.file)
+    except Error as e:
         e.print()
+
+        # print the traceback
         if args.print_exceptions:
             raise e
+
         sys.exit(1)
 
     if output_method == IOMethod.FILE:
         # output to file
 
         with open(output_file, "w+") as f:
             f.write(out)
 
     elif output_method == IOMethod.STD:
         # output to stdout
 
-        # check if line numbers should be printed
         if vars(args)["lines"]:
+            # print line numbers
+
             lines = out.splitlines()
-            max_line = len(str(len(lines)))
+            max_line = len(str(len(lines) - 1))
             for i, ln in enumerate(lines):
                 print(f"{str(i).zfill(max_line)}: {ln}")
         else:
             print(out)
 
         if verbose:
             print()
```

### Comparing `mlogpp-3.0.0rc1/mlogpp/constants.py` & `mlogpp-3.1.0/mlogpp/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .value import Type
 
 
+# block names inside of logic processors
 BLOCKS = set("""\
     siliconSmelter, siliconCrucible, kiln, graphitePress, plastaniumCompressor, multiPress, phaseWeaver,
     surgeSmelter, pyratiteMixer, blastMixer, cryofluidMixer,
     melter, separator, disassembler, sporePress, pulverizer, incinerator, coalCentrifuge,
 
     powerSource, powerVoid, itemSource, itemVoid, liquidSource, liquidVoid, payloadSource, payloadVoid, illuminator, heatSource,
     
@@ -36,14 +37,15 @@
     
     message, switchBlock, microProcessor, logicProcessor, hyperProcessor, largeLogicDisplay, logicDisplay, memoryCell, memoryBank,
     canvas,
     
     launchPad, interplanetaryAccelerator
 """.replace(" ", "").replace("\n", "").split(","))
 
+# block names inside the Mindustry code
 BLOCK_IDS = set("""\
     graphite-press, multi-press, silicon-smelter, silicon-crucible, kiln, plastanium-compressor, phase-weaver,
     surge-smelter, cryofluid-mixer, pyratite-mixer, blast-mixer, melter, separator, disassembler, spore-press,
     pulverizer, coal-centrifuge, incinerator,
     
     copper-wall, copper-wall-large, titanium-wall, titanium-wall-large, plastanium-wall, plastanium-wall-large,
     thorium-wall, thorium-wall-large, phase-wall, phase-wall-large, surge-wall, surge-wall-large, door, door-large,
@@ -73,22 +75,27 @@
     
     illuminator, launch-pad, interplanetary-accelerator,
     
     message, switch, micro-processor, logic-processor, hyper-processor, memory-cell, memory-bank, logic-display,
     logic-display-large
 """.replace(" ", "").replace("\n", "").split(","))
 
+# block link names
 BLOCK_LINKS = set()
 for name in BLOCK_IDS:
     if "-" in name:
         spl = name.split("-")
+
+        # filter out "large" from names
         if len(spl) >= 2 and spl[-1] == "large":
             name = spl[-2]
+
         else:
             name = spl[-1]
+
     BLOCK_LINKS.add(name)
 
 ITEMS = set("""\
     scrap, copper, lead, graphite, coal, titanium, thorium, silicon, plastanium,
     phaseFabric, surgeAlloy, sporePod, sand, blastCompound, pyratite, metaglass
 """.replace(" ", "").replace("\n", "").split(","))
 
@@ -106,14 +113,15 @@
     
     risso, minke, bryde, sei, omura,
     retusa, oxynoe, cyerce, aegires, navanax
 """.replace(" ", "").replace("\n", "").split(","))
 
 TEAMS = {"derelict", "sharded", "crux", "malis", "green", "blue"}
 
+# values readable by the sensor command
 SENSOR_READABLE = {
     "totalItems": Type.NUM,
     "firstItem": Type.NUM,
     "totalLiquids": Type.NUM,
     "totalPower": Type.NUM,
     "itemCapacity": Type.NUM,
     "liquidCapacity": Type.NUM,
@@ -157,10 +165,11 @@
     "color": Type.NUM
 } | {
     item: Type.NUM for item in ITEMS
 } | {
     liquid: Type.NUM for liquid in LIQUIDS
 }
 
+# values writable by "." access
 CONTROLLABLE = {
     "enabled", "config", "color"
 }
```

### Comparing `mlogpp-3.0.0rc1/mlogpp/error.py` & `mlogpp-3.1.0/mlogpp/error.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,103 @@
 import enum
 
 from .formatting import Format
 from .util import Position, sanitize
 
 
-class MlogError(Exception):
-    def __init__(self, msg: str, pos: Position = None):
+class Error(Exception):
+    """
+    Compilation error.
+    """
+
+    msg: str
+    pos: Position | None
+
+    def __init__(self, msg: str, pos: Position | None = None):
+        """
+        Args:
+            msg: The message to be displayed.
+            pos: Position at which the error occurred.
+        """
+
         self.message = f"{msg}: {pos}"
 
         self.msg = msg
         self.pos = pos
-    
+
     def print(self):
+        """
+        Print the error message and position.
+        """
+
         if self.pos is not None:
-            print(f"{Format.ERROR}{Format.BOLD}Error{Format.RESET}{Format.ERROR} in file {self.pos.file} on line {self.pos.line}, column {self.pos.start+1}: {self.msg}{Format.RESET}")
+            print(
+                f"{Format.ERROR}{Format.BOLD}Error{Format.RESET}{Format.ERROR} in file {self.pos.file} on line {self.pos.line}, column {self.pos.start + 1}: {self.msg}{Format.RESET}")
             print(f"Here:\n{self.pos.code}\n{self.pos.arrows()}")
         else:
             print(f"{Format.ERROR}{Format.BOLD}Error{Format.RESET}{Format.ERROR}: {self.msg}{Format.RESET}")
 
-
-class Error:
     @staticmethod
     def unexpected_character(pos: Position, ch: str):
-        raise MlogError(f"Unexpected character [{ch}]", pos)
+        raise Error(f"Unexpected character [{ch}]", pos)
 
     @staticmethod
     def already_imported(pos: Position, path: str):
-        raise MlogError(f"Already imported [{path}]", pos)
+        raise Error(f"Already imported [{path}]", pos)
 
     @staticmethod
     def cannot_find_file(pos: Position, path: str):
-        raise MlogError(f"Cannot find file [{path}]", pos)
+        raise Error(f"Cannot find file [{path}]", pos)
 
     @staticmethod
     def unexpected_token(tok: 'Token'):
-        raise MlogError(f"Unexpected token [{sanitize(tok.value)}]", tok.pos)
+        raise Error(f"Unexpected token [{sanitize(tok.value)}]", tok.pos)
 
     @staticmethod
     def unexpected_eof(pos: Position):
-        raise MlogError(f"Unexpected EOF", pos)
+        raise Error(f"Unexpected EOF", pos)
 
     @staticmethod
     def incompatible_types(node: 'Node', a: 'Type', b: 'Type'):
-        raise MlogError(f"Incompatible types [{a.name}, {b.name}]", node.get_pos())
+        raise Error(f"Incompatible types [{a.name}, {b.name}]", node.get_pos())
 
     @staticmethod
     def undefined_function(node: 'Node', func: str):
-        raise MlogError(f"Undefined function [{func}]", node.get_pos())
+        raise Error(f"Undefined function [{func}]", node.get_pos())
 
     @staticmethod
     def already_defined_var(node: 'Node', name: str):
-        raise MlogError(f"Variable [{name}] is already defined", node.get_pos())
+        raise Error(f"Variable [{name}] is already defined", node.get_pos())
 
     @staticmethod
     def undefined_variable(node: 'Node', name: str):
-        raise MlogError(f"Undefined variable [{name}]", node.get_pos())
+        raise Error(f"Undefined variable [{name}]", node.get_pos())
 
     @staticmethod
     def invalid_arg_count(node: 'Node', count: int, expected: int):
-        raise MlogError(f"Invalid number of arguments to function ({count}, expected {expected})", node.get_pos())
+        raise Error(f"Invalid number of arguments to function ({count}, expected {expected})", node.get_pos())
 
     @staticmethod
     def write_to_const(node: 'Node', var: str):
-        raise MlogError(f"Trying to write into a constant [{var}]", node.get_pos())
+        raise Error(f"Trying to write into a constant [{var}]", node.get_pos())
+
+    @staticmethod
+    def custom(pos: Position, message: str):
+        raise Error(message, pos)
+
+
+class InternalError(Exception):
+    """
+    Internal compilation error.
+    """
+
+    @staticmethod
+    def invalid_arg_count(ins: str, count: int, expected: int):
+        raise InternalError(f"Invalid number of arguments to instruction [{ins}] ({count}, expected {expected})")
+
+    @staticmethod
+    def undefined_function(name: str):
+        raise InternalError(f"Undefined function [{name}]")
+
+    @staticmethod
+    def label_not_found(name: str):
+        raise InternalError(f"Label not found [{name}]")
```

### Comparing `mlogpp-3.0.0rc1/mlogpp/generator.py` & `mlogpp-3.1.0/mlogpp/generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from .value import *
 
 
 class Gen:
     """
-    generates temporary values, stores compile time values
+    Generates unnamed values.
     """
 
     VAR_COUNT = 0
     LAB_COUNT = 0
-
     SCOPE_COUNT = 0
 
     @staticmethod
     def reset():
         """
         reset the generator
         """
 
         Gen.VAR_COUNT = 0
         Gen.LAB_COUNT = 0
+        Gen.SCOPE_COUNT = 0
 
     @staticmethod
     def temp_var(type_: Type) -> VariableValue:
         """
         generate a temporary variable
         """
```

### Comparing `mlogpp-3.0.0rc1/mlogpp/preprocess.py` & `mlogpp-3.1.0/mlogpp/preprocess.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 import re
 
 
 class Preprocessor:
     """
-    preprocesses code
+    Resolves constants.
     """
 
     # code regexes
     REGEXES = {
         "CONST": re.compile(r"^const [a-zA-Z_][a-zA-Z_0-9]* = .+$")
     }
 
     @staticmethod
     def preprocess(code: str) -> str:
+        """
+        Resolve constants in code.
+
+        Args:
+            code: The code to be processed.
+
+        Returns:
+            The code with resolved constants.
+        """
+
         consts = {}
         tmp = ""
         for ln in code.splitlines():
             # check if line defines a constant
             if Preprocessor.REGEXES["CONST"].fullmatch(ln):
                 spl = ln.split(" = ", 1)
                 consts[spl[0].split(" ")[1]] = spl[1]
 
                 tmp += "\n"
 
                 continue
             
-            # replace constant references with values
+            # replace constant references with values sorted by length in order to not replace non-equal constants
             for k, v in sorted(consts.items(), key=lambda pair: len(pair[0]), reverse=True):
                 ln = ln.replace(k, v)
             
             tmp += ln + "\n"
         
         return tmp
```

### Comparing `mlogpp-3.0.0rc1/mlogpp/scope.py` & `mlogpp-3.1.0/mlogpp/scope.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,79 @@
 from .value import *
 from .function import *
 from . import constants
 
 
 class Scope:
+    """
+    Scope, contains variable and function definitions.
+    """
+
     name: str | None
     variables: set[VariableValue]
     functions: set[Function]
 
     def __init__(self, name: str | None, variables: set[VariableValue] | None = None, functions: set[Function] | None = None):
         self.name = name
         self.variables = variables if variables is not None else set()
         self.functions = functions if functions is not None else set()
 
-    def add(self, var: VariableValue | Function):
+    def add(self, var: VariableValue | Function) -> None:
+        """
+        Add a variable or function to the scope.
+
+        Args:
+            var: The variable or function to be added.
+        """
+
         if isinstance(var, VariableValue):
             self.variables.add(var)
         elif isinstance(var, Function):
             self.functions.add(var)
 
-    def remove(self, var: VariableValue | Function):
+    def remove(self, var: VariableValue | Function) -> None:
+        """
+        Remove a variable or function from scope.
+
+        Args:
+            var: The variable or function to be removed.
+        """
+
         if isinstance(var, VariableValue):
             self.variables.remove(var)
         elif isinstance(var, Function):
             self.functions.remove(var)
 
     def rename(self, var: str) -> str:
+        """
+        Rename a variable with the scope name.
+
+        Args:
+            var: The variable to be renamed.
+
+        Returns:
+            The renamed variable.
+        """
+
         if self.name is None:
             return var
 
         return f"__s_{self.name}_{var}"
 
     def get(self, name: str) -> VariableValue | Function | None:
+        """
+        Get a variable or function definition.
+
+        Args:
+            name: Name of the variable or function.
+
+        Returns:
+            The variable or function definition, None if nothing is found.
+        """
+
         for var in self.variables:
             if var.name == name:
                 return var
 
         for fun in self.functions:
             if fun.name == name:
                 return fun
@@ -49,14 +87,15 @@
         elif isinstance(var, Function):
             return var in self.functions
 
         return any(var_.name == var for var_ in self.variables) or any(fun.name == var for fun in self.functions)
 
 
 class Scopes:
+    # the default scope, containing global constants and variables
     DEFAULT_SCOPE = Scope(
         None,
         {
             VariableValue(Type.BLOCK, "@this", True),
             VariableValue(Type.NUM, "@thisx", True),
             VariableValue(Type.NUM, "@thisy", True),
             VariableValue(Type.NUM, "@ipt", True),
@@ -68,17 +107,17 @@
             VariableValue(Type.NUM, "@second", True),
             VariableValue(Type.NUM, "@minute", True),
             VariableValue(Type.NUM, "@waveNumber", True),
             VariableValue(Type.NUM, "@waveTime", True),
             VariableValue(Type.NUM, "@mapw", True),
             VariableValue(Type.NUM, "@maph", True),
 
-            VariableValue(Type.NUM, "true", True),
-            VariableValue(Type.NUM, "false", True),
-            VariableValue(Type.NULL, "null", True),
+            VariableValue(Type.NUM, "true", True, NumberValue(1)),
+            VariableValue(Type.NUM, "false", True, NumberValue(0)),
+            VariableValue(Type.NULL, "null", True, NullValue()),
 
             VariableValue(Type.CONTROLLER, "@ctrlProcessor", True),
             VariableValue(Type.CONTROLLER, "@ctrlPlayer", True),
             VariableValue(Type.CONTROLLER, "@ctrlCommand", True),
 
             VariableValue(Type.BLOCK_TYPE, "@solid", True)
         } | {
@@ -91,46 +130,95 @@
             VariableValue(Type.TEAM, "@" + team, True) for team in constants.TEAMS
         }
     )
 
     SCOPES = [DEFAULT_SCOPE, Scope(None)]
 
     @staticmethod
-    def reset():
+    def reset() -> None:
+        """
+        Reset all the scopes.
+        """
+
         Scopes.SCOPES = [Scopes.DEFAULT_SCOPE, Scope(None)]
 
     @staticmethod
-    def push(name: str | None):
+    def push(name: str | None) -> None:
+        """
+        Push a scope to the stack.
+
+        Args:
+            name: Name of the scope to be pushed.
+        """
+
         Scopes.SCOPES.append(Scope(name))
 
     @staticmethod
-    def pop():
+    def pop() -> None:
+        """
+        Pop a scope from the stack.
+        """
+
         Scopes.SCOPES.pop(-1)
 
     @staticmethod
-    def add(var: VariableValue | Function):
+    def add(var: VariableValue | Function) -> None:
+        """
+        Add a variable or function to the top scope on the stack.
+
+        Args:
+            var: The variable or function to be added.
+        """
+
         Scopes.SCOPES[-1].add(var)
 
     @staticmethod
-    def remove(var: VariableValue | Function):
+    def remove(var: VariableValue | Function) -> None:
+        """
+        Remove a variable or function from the top scope on the stack.
+
+        Args:
+            var: The variable or function to be removed.
+        """
+
         Scopes.SCOPES[-1].remove(var)
 
     @staticmethod
     def rename(var: str, declare: bool = False) -> str:
+        """
+        Rename a variable using the scope names.
+
+        Args:
+            var: The variable to be renamed.
+            declare: If true, variable will be renamed using topmost scope, otherwise using first one that contains it.
+
+        Returns:
+            The renamed variable.
+        """
+
         if declare:
             return Scopes.SCOPES[-1].rename(var)
 
         for scope in reversed(Scopes.SCOPES):
             if scope.rename(var) in scope:
                 return scope.rename(var)
 
         return Scopes.SCOPES[0].rename(var)
 
     @staticmethod
     def get(name: str) -> VariableValue | Function | None:
+        """
+        Get a variable or function by name.
+
+        Args:
+            name: Name of the variable or function to be searched for.
+
+        Returns:
+            The variable or function, None if not found.
+        """
         for scope in reversed(Scopes.SCOPES):
             if (var := scope.get(name)) is not None:
                 return var
 
         return None
 
     @staticmethod
```

### Comparing `mlogpp-3.0.0rc1/mlogpp/tokens.py` & `mlogpp-3.1.0/mlogpp/tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import enum
 
 from .util import Position, sanitize
 
 
 class TokenType(enum.Flag):
     """
-    token types
+    Token type.
     """
 
     NONE = enum.auto()
     ID = enum.auto()
     KEYWORD = enum.auto()
     NATIVE = enum.auto()
     STRING = enum.auto()
@@ -26,21 +26,22 @@
     ARROW = enum.auto()
     OPERATOR = enum.auto()
     SET = enum.auto()
 
 
 class Token:
     """
-    token of code
+    Token.
     """
 
     type: TokenType
     value: str
     pos: Position
 
+    # builtin types
     TYPES = (
         "num", "str",
         "Block", "Unit", "Team",
         "BlockType", "UnitType", "ItemType", "LiquidType",
         "Controller"
     )
     BLOCK_STATEMENTS = (
@@ -49,14 +50,15 @@
     )
     STATEMENTS = BLOCK_STATEMENTS + (
         "return", "break", "continue",
         "end",
         "else"
     )
 
+    # reserved keywords
     KEYWORDS = TYPES + STATEMENTS
 
     def __init__(self, type_: TokenType, value: str, pos: Position):
         self.type = type_
         self.value = value
         self.pos = pos
```

### Comparing `mlogpp-3.0.0rc1/mlogpp/util.py` & `mlogpp-3.1.0/mlogpp/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,38 @@
 def sanitize(s: str) -> str:
     """
-    sanitize a string
+    Sanitize a string.
+
+    Args:
+        s: The string to be sanitized.
+
+    Returns:
+        The sanitized string.
     """
 
     return s.replace("\n", "\\n").replace("\t", "\\t").replace("\r", "\\r")
 
 
-def flatten(lst: list) -> list:
+def flatten(lst: list[list]) -> list:
+    """
+    Flatten a two-dimensional list.
+
+    Args:
+        lst: The list to be flattened.
+
+    Returns:
+        The flattened list.
+    """
+
     return [item for sublist in lst for item in sublist]
 
 
 class Position:
     """
-    position in code
+    Position in code.
     """
 
     line: int
     start: int
     end: int
     code: str
     file: str
@@ -26,41 +42,47 @@
         self.start = start
         self.end = end
         self.code = sanitize(code)
         self.file = file
     
     def arrows(self) -> str:
         """
-        generate error arrows
+        Generate error arrows for the position.
+
+        Returns:
+            The generated arrows.
         """
 
         return f"{' ' * self.start}{'^' * (self.end - self.start)}"
     
     def code_section(self) -> str:
         """
-        get code section defined by the position
+        Get the code section in the position.
+
+        Returns:
+            The code section in the position.
         """
 
         return self.code[self.start:self.end]
     
     def __add__(self, other: "Position") -> "Position":
         """
-        create a range of two positions
+        Create a range of two positions.
         """
 
         if self.line == other.line:
             return Position(self.line, min(self.start, other.start), max(self.end, other.end), self.code, self.file)
         elif self.line < other.line:
             return Position(self.line, self.start, len(self.code), self.code, self.file)
         else:
             return Position(other.line, other.start, len(other.code), other.code, self.file)
 
     def __iadd__(self, other: "Position") -> "Position":
         """
-        create a range of two positions
+        Create a range of two positions.
         """
 
         if self.line == other.line:
             self.start = min(self.start, other.start)
             self.end = max(self.end, other.end)
         elif self.line < other.line:
             self.end = len(self.code)
```

### Comparing `mlogpp-3.0.0rc1/mlogpp/value.py` & `mlogpp-3.1.0/mlogpp/value.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+from __future__ import annotations
+
 import enum
 
-from .error import MlogError
+from .error import Error
 
 
 class Type(enum.Flag):
+    """
+    Type of value.
+    """
+
     STR = enum.auto()
     NUM = enum.auto()
     NULL = enum.auto()
 
     BLOCK = enum.auto()
     UNIT = enum.auto()
     TEAM = enum.auto()
@@ -19,14 +25,24 @@
 
     CONTROLLER = enum.auto()
 
     ANY = NUM | STR | NULL | BLOCK | UNIT | TEAM | UNIT_TYPE | ITEM_TYPE | BLOCK_TYPE | LIQUID_TYPE | CONTROLLER
 
     @staticmethod
     def from_code(var: str) -> 'Type':
+        """
+        Create a type from an in-code name without "_"
+
+        Args:
+            var: The in-code name.
+
+        Returns:
+            The created type.
+        """
+
         tok = ""
         last = ""
         for ch in var:
             if ch.upper() == ch and last:
                 tok += "_"
             tok += ch
             last = ch
@@ -37,33 +53,44 @@
 class Value:
     type: Type
 
     def __init__(self, type_: Type):
         self.type = type_
 
     def __str__(self):
-        raise MlogError(f"Invalid value [{repr(self)}]")
+        raise Error(f"Invalid value [{repr(self)}]")
 
     def __hash__(self):
         return hash(self.type)
 
+    @staticmethod
+    def from_(val) -> Value:
+        if isinstance(val, str):
+            return StringValue(val)
+        elif isinstance(val, int | float):
+            return NumberValue(val)
+        return NullValue()
+
 
 class StringValue(Value):
     value: str
 
     __match_args__ = ("value",)
 
     def __init__(self, value: str):
         super().__init__(Type.STR)
 
         self.value = value
 
     def __str__(self):
         return self.value
 
+    def __repr__(self):
+        return f"StringValue(\"{self.value}\")"
+
     def __hash__(self):
         return hash((self.type, self.value))
 
 
 class NumberValue(Value):
     value: int | float
 
@@ -73,14 +100,17 @@
         super().__init__(Type.NUM)
 
         self.value = value
 
     def __str__(self):
         return str(self.value)
 
+    def __repr__(self):
+        return f"NumberValue({self.value})"
+
     def __hash__(self):
         return hash((self.type, self.value))
 
 
 class NullValue(Value):
     value: None
 
@@ -90,14 +120,17 @@
         super().__init__(Type.NULL)
 
         self.value = None
 
     def __str__(self):
         return "null"
 
+    def __repr__(self):
+        return f"NullValue()"
+
     def __hash__(self):
         return hash((self.type, self.value))
 
 
 class BlockValue(Value):
     name: str
 
@@ -107,28 +140,36 @@
         super().__init__(Type.BLOCK)
 
         self.name = name
 
     def __str__(self):
         return self.name
 
+    def __repr__(self):
+        return f"BlockValue({self.value})"
+
     def __hash__(self):
         return hash((self.type, self.name))
 
 
 class VariableValue(Value):
     name: str
     const: bool
+    const_val: Value
 
     __match_args__ = ("name", "type", "const")
 
-    def __init__(self, type_: Type, name: str, const: bool = False):
+    def __init__(self, type_: Type, name: str, const: bool = False, const_val: Value = None):
         super().__init__(type_)
 
         self.name = name
         self.const = const
+        self.const_val = const_val
 
     def __str__(self):
         return self.name
 
+    def __repr__(self):
+        return f"VariableValue({self.name}{' | const' if self.const else ''})"
+
     def __hash__(self):
         return hash((self.type, self.name, self.const))
```

### Comparing `mlogpp-3.0.0rc1/mlogpp.egg-info/PKG-INFO` & `mlogpp-3.1.0/mlogpp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlogpp
-Version: 3.0.0rc1
+Version: 3.1.0
 Summary: statically typed high level mindustry logic language
 Home-page: https://github.com/albi-c/mlog++
 Author: albi-c
 Project-URL: Bug Tracker, https://github.com/albi-c/mlog++/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,14 +26,15 @@
 
 ### Options:
 * `-o:f`, `--output-file` - output to file
 * `-o:s`, `--output-stdout` - output to stdout
 * `-o:c`, `--output-clip` - output to clipboard (default)
 * `-v`, `--verbose` - output more information
 * `-l`, `--lines` - print line numbers when output is stdout
+* `-a`, `--assembly` - compile as mlog++ assembly
 * `-V`, `--version` - print version and exit
 
 ## Examples:
 ### Hello, World:
 ```javascript
 print("Hello, World!")
 printflush(message1)
@@ -106,20 +107,37 @@
 print(" ")
 print(b)
 
 printflush(message1)
 ```
 Prints `0 10`
 
+### Assembly:
+```javascript
+{LOOP_LENGTH = 2 + 3}
+
+i = 0
+loop_start:
+    i += 1
+    
+    print(i)
+    print("\n")
+    
+    :loop_start (i < {LOOP_LENGTH})
+
+printflush(message1)
+```
+Prints `1 2 3 4 5`
+
 ### Longer examples can be found in `examples/`
 
 ## Features:
 * variables \
   `num x = 1`
-* types \
+* types 
   * `num`, `str`
   * `Block`, `Unit`,
   * `BlockType`, `UnitType`, `ItemType`, `LiquidType`,
   * `Controller`, `Team`
 * comments \
   `# comment`
 * memory cell access \
@@ -137,14 +155,18 @@
 * ranges \
   `for (i : 5) { print(i) }`
 * break / continue
 * native functions \
   `ubind(@mega)`
 * constants \
   `const VALUE = 30`
+* inline python subset in assembly \
+  `{x = 7 ^ 2}`   
+  `print({y = x // 2})`
+  `{"cell" + x}[0] = y`
 
 ## Native functions:
 * read `result`, `cell`, `position`
     * Read data from `cell` at `position` to `result`
 * write `data`, `cell`, `position`
     * Write `data` to `cell` at `position`
 * draw `operation`, `arg0` ... `arg5`
@@ -173,15 +195,15 @@
     * Commands:
         * enabled `block`, `enabled`
         * shoot `block`, `x`, `y`, `shoot`
         * shootp `block`, `unit`, `shoot`
         * config `block`, `configuration`
         * color `block`, `red`, `green`, `blue`
 * radar `filter0` ... `filter2`, `sort`, `block`, `order`, `result`
-    * Find an unit near `block` and store it in `result`
+    * Find a unit near `block` and store it in `result`
     * Filters:
         * any
         * enemy
         * ally
         * player
         * attacker
         * flying
```

### Comparing `mlogpp-3.0.0rc1/setup.py` & `mlogpp-3.1.0/setup.py`

 * *Files identical despite different names*

